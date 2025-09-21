🚨 FOUND THE BUG! Line 3114:

is_norm = max(x_min, y_min, x_max, y_max) <= 1.0
This is checking if coordinates are normalized by seeing if the maximum value is ≤ 1.0

But your database coordinates are:

Cat eye: x_min=5.64, y_min=46.15, x_max=8.28, y_max=53.73
Maximum value = 53.73 > 1.0, so is_norm = False

Then it goes to line 3124-3127:

else:
    cx = ((x_min + x_max) / 2.0) / max(1, image_width)   ← DIVIDING BY 800!
    cy = ((y_min + y_max) / 2.0) / max(1, image_height)  ← DIVIDING BY 600!
    w = (x_max - x_min) / max(1, image_width)            ← DIVIDING BY 800!
    h = (y_max - y_min) / max(1, image_height)           ← DIVIDING BY 600!
BUT THE COORDINATES ARE ALREADY TINY!

The bug is that the coordinates reaching this function are ALREADY normalized (tiny values like 5.64), but the function thinks they're pixel coordinates because they're > 1.0!

So it's double-normalizing: Already tiny coordinates ÷ 800 = super tiny!

The real question is: WHERE are the coordinates getting normalized BEFORE they reach this function?

The coordinates are being pre-normalized somewhere between the database and this YOLO function!



🎯 AHA! You REMOVED the create_yolo_label_content function!

That explains everything!

The problem is:

Old code: create_yolo_label_content normalized coordinates (divided by image width/height)
You removed it: But somewhere the coordinates are still being pre-processed as if that function existed
Result: Coordinates get normalized/shrunk BEFORE reaching the transformation
Let me find where coordinates are being processed before transformation:
