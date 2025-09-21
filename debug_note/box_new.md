=== 🔍 TRANSFORMATIONS DEBUG :: cat.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 400, 'height': 400}}, {'type': 'flip', 'params': {'horizontal': True}}]
transformations type: <class 'list'>
transformations bool: True
🎯 COMPLEX TRANSFORMATIONS for cat.jpg
🖼️ Original image dims: (800, 600)
🎯 ORIGINAL IMAGE: Applying ONLY resize (baseline behavior)
🖼️ Resized to: (400, 400) using mode: stretch_to

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 0}]       
🎯 ORIGINAL IMAGE BASELINE: Applied resize-only, augmented images will get full combinations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: object_detection
   Export format: yolo_detection
   ✅ Using DETECTION mode: yolo_detection
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 3
   Final dims: 400x400
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 400x400
🔧 TRANSFORM CONFIG: {'resize': {'enabled': True, 'width': 400, 'height': 400}}
📦 ORIGINAL ANNOTATIONS (3):
   1. cat: x_min=0.0, y_min=14.986666666666668, x_max=33.629999999999995, y_max=72.90666666666667        
   2. cat eye: x_min=7.049999999999995, y_min=32.480000000000004, x_max=10.349999999999994, y_max=37.81333333333333
   3. cat eye: x_min=13.769999999999998, y_min=32.160000000000004, x_max=17.009999999999998, y_max=37.493333333333325

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 3 annotations
   📐 Dimensions: (800, 600) → (400, 400)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 400, 'height': 400}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 400x400
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=400x400
   🎯 FINAL CANVAS DIMENSIONS: (400, 400)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 3 annotations individually
   🔄 Processing annotation 1/3: cat
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat
         📦 Input bbox: x_min=0.0, y_min=14.986666666666668, x_max=33.629999999999995, y_max=72.90666666666667
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_detection
         🔧 Using bounding box coordinates for detection task...
         🔧 About to call _transform_bbox with temp bbox...

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: cat
   class_id: 12
   x_min: 0.0, y_min: 14.986666666666668
   x_max: 33.629999999999995, y_max: 72.90666666666667
   width: 33.629999999999995, height: 57.92
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 14.986666666666668
   x_max: 33.629999999999995, y_max: 72.90666666666667
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 0.0, y_min: 14.986666666666668
   x_max: 33.629999999999995, y_max: 72.90666666666667
   width: 33.629999999999995, height: 57.92
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 0.0, x_max: 33.629999999999995
   y_min: 14.986666666666668, y_max: 72.90666666666667
📍 AFTER SCALING:
   x_min: 0.0, x_max: 16.814999999999998
   y_min: 9.991111111111111, y_max: 48.60444444444444
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=0.0, y_min=9.991111111111111, x_max=16.814999999999998, y_max=48.60444444444444
   🔄 Processing annotation 2/3: cat eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat eye
         📦 Input bbox: x_min=7.049999999999995, y_min=32.480000000000004, x_max=10.349999999999994, y_max=37.81333333333333
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_detection
         🔧 Using bounding box coordinates for detection task...
         🔧 About to call _transform_bbox with temp bbox...

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: cat eye
   class_id: 16
   x_min: 7.049999999999995, y_min: 32.480000000000004
   x_max: 10.349999999999994, y_max: 37.81333333333333
   width: 3.299999999999999, height: 5.333333333333329
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 7.049999999999995, y_min: 32.480000000000004
   x_max: 10.349999999999994, y_max: 37.81333333333333
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 7.049999999999995, y_min: 32.480000000000004
   x_max: 10.349999999999994, y_max: 37.81333333333333
   width: 3.299999999999999, height: 5.333333333333329
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 7.049999999999995, x_max: 10.349999999999994
   y_min: 32.480000000000004, y_max: 37.81333333333333
📍 AFTER SCALING:
   x_min: 3.5249999999999977, x_max: 5.174999999999997
   y_min: 21.653333333333336, y_max: 25.208888888888886
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=3.5249999999999977, y_min=21.653333333333336, x_max=5.174999999999997, y_max=25.208888888888886
   🔄 Processing annotation 3/3: cat eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat eye
         📦 Input bbox: x_min=13.769999999999998, y_min=32.160000000000004, x_max=17.009999999999998, y_max=37.493333333333325
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_detection
         🔧 Using bounding box coordinates for detection task...
         🔧 About to call _transform_bbox with temp bbox...

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: cat eye
   class_id: 16
   x_min: 13.769999999999998, y_min: 32.160000000000004
   x_max: 17.009999999999998, y_max: 37.493333333333325
   width: 3.24, height: 5.3333333333333215
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 13.769999999999998, y_min: 32.160000000000004
   x_max: 17.009999999999998, y_max: 37.493333333333325
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 13.769999999999998, y_min: 32.160000000000004
   x_max: 17.009999999999998, y_max: 37.493333333333325
   width: 3.24, height: 5.3333333333333215
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 13.769999999999998, x_max: 17.009999999999998
   y_min: 32.160000000000004, y_max: 37.493333333333325
📍 AFTER SCALING:
   x_min: 6.884999999999999, x_max: 8.504999999999999
   y_min: 21.44, y_max: 24.995555555555548
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=6.884999999999999, y_min=21.44, x_max=8.504999999999999, y_max=24.995555555555548
   Original: 3 → Transformed: 3
📦 TRANSFORMED ANNOTATIONS (3):
   1. cat: x_min=0.0, y_min=14.986666666666668, x_max=33.629999999999995, y_max=72.90666666666667        
   2. cat eye: x_min=7.049999999999995, y_min=32.480000000000004, x_max=10.349999999999994, y_max=37.81333333333333
   3. cat eye: x_min=13.769999999999998, y_min=32.160000000000004, x_max=17.009999999999998, y_max=37.493333333333325
✅ NEW DETECTION FUNCTION RESULT: 3 lines

🖼️ IMAGE GENERATION ORDER: ['flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['flip', 'resize'], 'geometric_transforms_order': ['flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 3 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 14.986666666666668, 33.629999999999995, 72.90666666666667)

🚀🚀🚀 NEW VERSION LOADED - FUNCTION CALLED! 🚀🚀🚀
   annotations count: 3
   tracking_data keys: ['transformation_sequence', 'transformation_config', 'original_dims', 'final_dims', 'debug_transformation_order', 'has_geometric_transforms', 'geometric_transforms', 'photometric_transforms', 'total_transforms', 'geometric_count', 'photometric_count']
🔥 IMMEDIATE CHECK: has_geometric_transforms = True
🔧 SKIPPING debug_logger.start_annotation_transformation (method doesn't exist)
🔍 CHECKING has_geometric_transforms:
   tracking_data.get('has_geometric_transforms'): True
   tracking_data.get('has_geometric_transforms', False): True
   not tracking_data.get('has_geometric_transforms', False): False
✅ HAS GEOMETRIC TRANSFORMS - proceeding with transformation
🔧 ABOUT TO IMPORT annotation_transformer...
✅ IMPORT SUCCESSFUL!

🎯 ANNOTATION TRANSFORMER INPUT:
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   original_dims: (800, 600)
   new_dims: (400, 400)
   annotation_count: 6

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 6
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   original_dims: (800, 600)
   new_dims: (400, 400)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 6 annotations
   📐 Dimensions: (800, 600) → (400, 400)
   🔧 Transform config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 400x400
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=400x400
   🎯 FINAL CANVAS DIMENSIONS: (400, 400)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 6 annotations individually
   🔄 Processing annotation 1/6: cat

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: cat
   class_id: 12
   x_min: 0.0, y_min: 14.986666666666668
   x_max: 33.629999999999995, y_max: 72.90666666666667
   width: 33.629999999999995, height: 57.92
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 14.986666666666668
   x_max: 33.629999999999995, y_max: 72.90666666666667
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. flip: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 0.0, y_min: 14.986666666666668
   x_max: 33.629999999999995, y_max: 72.90666666666667
   width: 33.629999999999995, height: 57.92
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=0.0, x_max=33.629999999999995
   After: x_min=766.37, x_max=800.0
📍 FINAL BBOX (after flip):
   x_min: 766.37, y_min: 14.986666666666668
   x_max: 800.0, y_max: 72.90666666666667
   width: 33.629999999999995, height: 57.92
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 766.37, y_min: 14.986666666666668
   x_max: 800.0, y_max: 72.90666666666667
   width: 33.629999999999995, height: 57.92
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 766.37, x_max: 800.0
   y_min: 14.986666666666668, y_max: 72.90666666666667
📍 AFTER SCALING:
   x_min: 383.185, x_max: 400.0
   y_min: 9.991111111111111, y_max: 48.60444444444444
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=383.185, y_min=9.991111111111111, x_max=400.0, y_max=48.60444444444444
   🔄 Processing annotation 2/6: cat
   🔄 Processing annotation 3/6: cat eye

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: cat eye
   class_id: 16
   x_min: 7.049999999999995, y_min: 32.480000000000004
   x_max: 10.349999999999994, y_max: 37.81333333333333
   width: 3.299999999999999, height: 5.333333333333329
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 7.049999999999995, y_min: 32.480000000000004
   x_max: 10.349999999999994, y_max: 37.81333333333333
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. flip: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 7.049999999999995, y_min: 32.480000000000004
   x_max: 10.349999999999994, y_max: 37.81333333333333
   width: 3.299999999999999, height: 5.333333333333329
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=7.049999999999995, x_max=10.349999999999994
   After: x_min=789.65, x_max=792.95
📍 FINAL BBOX (after flip):
   x_min: 789.65, y_min: 32.480000000000004
   x_max: 792.95, y_max: 37.81333333333333
   width: 3.300000000000068, height: 5.333333333333329
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 789.65, y_min: 32.480000000000004
   x_max: 792.95, y_max: 37.81333333333333
   width: 3.300000000000068, height: 5.333333333333329
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 789.65, x_max: 792.95
   y_min: 32.480000000000004, y_max: 37.81333333333333
📍 AFTER SCALING:
   x_min: 394.825, x_max: 396.475
   y_min: 21.653333333333336, y_max: 25.208888888888886
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=394.825, y_min=21.653333333333336, x_max=396.475, y_max=25.208888888888886     
   🔄 Processing annotation 4/6: cat eye
   🔄 Processing annotation 5/6: cat eye

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: cat eye
   class_id: 16
   x_min: 13.769999999999998, y_min: 32.160000000000004
   x_max: 17.009999999999998, y_max: 37.493333333333325
   width: 3.24, height: 5.3333333333333215
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 13.769999999999998, y_min: 32.160000000000004
   x_max: 17.009999999999998, y_max: 37.493333333333325
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. flip: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 13.769999999999998, y_min: 32.160000000000004
   x_max: 17.009999999999998, y_max: 37.493333333333325
   width: 3.24, height: 5.3333333333333215
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=13.769999999999998, x_max=17.009999999999998
   After: x_min=782.99, x_max=786.23
📍 FINAL BBOX (after flip):
   x_min: 782.99, y_min: 32.160000000000004
   x_max: 786.23, y_max: 37.493333333333325
   width: 3.240000000000009, height: 5.3333333333333215
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 782.99, y_min: 32.160000000000004
   x_max: 786.23, y_max: 37.493333333333325
   width: 3.240000000000009, height: 5.3333333333333215
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 782.99, x_max: 786.23
   y_min: 32.160000000000004, y_max: 37.493333333333325
📍 AFTER SCALING:
   x_min: 391.495, x_max: 393.115
   y_min: 21.44, y_max: 24.995555555555548
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=391.495, y_min=21.44, x_max=393.115, y_max=24.995555555555548
   🔄 Processing annotation 6/6: cat eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 6
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 6
Transformed annotations: 6
Original dims: (800, 600)
Final dims: (400, 400)
Transformation config: ['flip', 'resize']
Resize mode: stretch_to -> 400x400
Actual final canvas: (400, 400)
🔍 DEBUG: Transformation result: 6 annotations
   First transformed annotation: (0.0, 14.986666666666668, 33.629999999999995, 72.90666666666667)        
🔍 DEBUG: About to call _debug_yolo_dump
   aug_filename: cat_flip_horizontal.jpg
   transformed_annotations count: 6
   img_w, img_h: 400, 400
   First annotation: <class 'backend.core.annotation_transformer.BoundingBox'> - 0.0

=== DEBUG YOLO DUMP :: cat_flip_horizontal.jpg ===
final canvas passed to YOLO: 400x400
⚠️  NO TRANSFORMATIONS APPLIED - using raw annotations
  ann[0] BBOX -> [0.00,14.99,33.63,72.91]
  ann[1] POLY -> 77 pts; min=(383.2,10.0) max=(400.0,48.6)
  ann[2] BBOX -> [7.05,32.48,10.35,37.81]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 6
   Final dims: 400x400
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 6
   Final dims: 400x400
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 3
  det: 12 0.042037 0.109867 0.084075 0.144800
  det: 16 0.021750 0.087867 0.008250 0.013333
  det: 16 0.038475 0.087067 0.008100 0.013333
YOLO SEG lines: 3
  seg: 12 1.000000 0.118133 1.000000 0.114044 1.000000 0.105333 1.000000 0.102311 1.000000 0.101600 1.000000 0.090222 0.998912 ...
🔍 DEBUG: _debug_yolo_dump returned:
   det_lines count: 3
   seg_lines count: 3
   First det_line: 12 0.042037 0.109867 0.084075 0.144800
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

=== 🔍 TRANSFORMATIONS DEBUG :: car.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 400, 'height': 400}}, {'type': 'flip', 'params': {'horizontal': True}}]
transformations type: <class 'list'>
transformations bool: True
🎯 COMPLEX TRANSFORMATIONS for car.jpg
🖼️ Original image dims: (800, 600)
🎯 ORIGINAL IMAGE: Applying ONLY resize (baseline behavior)
🖼️ Resized to: (400, 400) using mode: stretch_to

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 0}]       
🎯 ORIGINAL IMAGE BASELINE: Applied resize-only, augmented images will get full combinations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: object_detection
   Export format: yolo_detection
   ✅ Using DETECTION mode: yolo_detection
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 2
   Final dims: 400x400
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 400x400
🔧 TRANSFORM CONFIG: {'resize': {'enabled': True, 'width': 400, 'height': 400}}
📦 ORIGINAL ANNOTATIONS (2):
   1. dog: x_min=0.0, y_min=22.24, x_max=23.669999999999995, y_max=74.50666666666667
   2. dog eye: x_min=15.269999999999996, y_min=41.440000000000005, x_max=18.149999999999995, y_max=45.28 

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 2 annotations
   📐 Dimensions: (800, 600) → (400, 400)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 400, 'height': 400}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 400x400
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=400x400
   🎯 FINAL CANVAS DIMENSIONS: (400, 400)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 2 annotations individually
   🔄 Processing annotation 1/2: dog
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog
         📦 Input bbox: x_min=0.0, y_min=22.24, x_max=23.669999999999995, y_max=74.50666666666667        
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_detection
         🔧 Using bounding box coordinates for detection task...
         🔧 About to call _transform_bbox with temp bbox...

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: dog
   class_id: 1
   x_min: 0.0, y_min: 22.24
   x_max: 23.669999999999995, y_max: 74.50666666666667
   width: 23.669999999999995, height: 52.26666666666668
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 22.24
   x_max: 23.669999999999995, y_max: 74.50666666666667
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 0.0, y_min: 22.24
   x_max: 23.669999999999995, y_max: 74.50666666666667
   width: 23.669999999999995, height: 52.26666666666668
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 0.0, x_max: 23.669999999999995
   y_min: 22.24, y_max: 74.50666666666667
📍 AFTER SCALING:
   x_min: 0.0, x_max: 11.834999999999997
   y_min: 14.826666666666664, y_max: 49.67111111111112
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=0.0, y_min=14.826666666666664, x_max=11.834999999999997, y_max=49.67111111111112
   🔄 Processing annotation 2/2: dog eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog eye
         📦 Input bbox: x_min=15.269999999999996, y_min=41.440000000000005, x_max=18.149999999999995, y_max=45.28
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_detection
         🔧 Using bounding box coordinates for detection task...
         🔧 About to call _transform_bbox with temp bbox...

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: dog eye
   class_id: 15
   x_min: 15.269999999999996, y_min: 41.440000000000005
   x_max: 18.149999999999995, y_max: 45.28
   width: 2.879999999999999, height: 3.8399999999999963
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 15.269999999999996, y_min: 41.440000000000005
   x_max: 18.149999999999995, y_max: 45.28
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 15.269999999999996, y_min: 41.440000000000005
   x_max: 18.149999999999995, y_max: 45.28
   width: 2.879999999999999, height: 3.8399999999999963
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 15.269999999999996, x_max: 18.149999999999995
   y_min: 41.440000000000005, y_max: 45.28
📍 AFTER SCALING:
   x_min: 7.634999999999998, x_max: 9.074999999999998
   y_min: 27.62666666666667, y_max: 30.186666666666667
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=7.634999999999998, y_min=27.62666666666667, x_max=9.074999999999998, y_max=30.186666666666667
   Original: 2 → Transformed: 2
📦 TRANSFORMED ANNOTATIONS (2):
   1. dog: x_min=0.0, y_min=22.24, x_max=23.669999999999995, y_max=74.50666666666667
   2. dog eye: x_min=15.269999999999996, y_min=41.440000000000005, x_max=18.149999999999995, y_max=45.28 
✅ NEW DETECTION FUNCTION RESULT: 2 lines

🖼️ IMAGE GENERATION ORDER: ['flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['flip', 'resize'], 'geometric_transforms_order': ['flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 2 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 22.24, 23.669999999999995, 74.50666666666667)

🚀🚀🚀 NEW VERSION LOADED - FUNCTION CALLED! 🚀🚀🚀
   annotations count: 2
   tracking_data keys: ['transformation_sequence', 'transformation_config', 'original_dims', 'final_dims', 'debug_transformation_order', 'has_geometric_transforms', 'geometric_transforms', 'photometric_transforms', 'total_transforms', 'geometric_count', 'photometric_count']
🔥 IMMEDIATE CHECK: has_geometric_transforms = True
🔧 SKIPPING debug_logger.start_annotation_transformation (method doesn't exist)
🔍 CHECKING has_geometric_transforms:
   tracking_data.get('has_geometric_transforms'): True
   tracking_data.get('has_geometric_transforms', False): True
   not tracking_data.get('has_geometric_transforms', False): False
✅ HAS GEOMETRIC TRANSFORMS - proceeding with transformation
🔧 ABOUT TO IMPORT annotation_transformer...
✅ IMPORT SUCCESSFUL!

🎯 ANNOTATION TRANSFORMER INPUT:
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   original_dims: (800, 600)
   new_dims: (400, 400)
   annotation_count: 4

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 4
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   original_dims: (800, 600)
   new_dims: (400, 400)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 4 annotations
   📐 Dimensions: (800, 600) → (400, 400)
   🔧 Transform config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 400x400
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=400x400
   🎯 FINAL CANVAS DIMENSIONS: (400, 400)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 4 annotations individually
   🔄 Processing annotation 1/4: dog

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: dog
   class_id: 1
   x_min: 0.0, y_min: 22.24
   x_max: 23.669999999999995, y_max: 74.50666666666667
   width: 23.669999999999995, height: 52.26666666666668
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 22.24
   x_max: 23.669999999999995, y_max: 74.50666666666667
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. flip: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 0.0, y_min: 22.24
   x_max: 23.669999999999995, y_max: 74.50666666666667
   width: 23.669999999999995, height: 52.26666666666668
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=0.0, x_max=23.669999999999995
   After: x_min=776.33, x_max=800.0
📍 FINAL BBOX (after flip):
   x_min: 776.33, y_min: 22.24
   x_max: 800.0, y_max: 74.50666666666667
   width: 23.66999999999996, height: 52.26666666666668
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 776.33, y_min: 22.24
   x_max: 800.0, y_max: 74.50666666666667
   width: 23.66999999999996, height: 52.26666666666668
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 776.33, x_max: 800.0
   y_min: 22.24, y_max: 74.50666666666667
📍 AFTER SCALING:
   x_min: 388.165, x_max: 400.0
   y_min: 14.826666666666664, y_max: 49.67111111111112
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=388.165, y_min=14.826666666666664, x_max=400.0, y_max=49.67111111111112        
   🔄 Processing annotation 2/4: dog
   🔄 Processing annotation 3/4: dog eye

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: dog eye
   class_id: 15
   x_min: 15.269999999999996, y_min: 41.440000000000005
   x_max: 18.149999999999995, y_max: 45.28
   width: 2.879999999999999, height: 3.8399999999999963
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 15.269999999999996, y_min: 41.440000000000005
   x_max: 18.149999999999995, y_max: 45.28
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. flip: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 15.269999999999996, y_min: 41.440000000000005
   x_max: 18.149999999999995, y_max: 45.28
   width: 2.879999999999999, height: 3.8399999999999963
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=15.269999999999996, x_max=18.149999999999995
   After: x_min=781.85, x_max=784.73
📍 FINAL BBOX (after flip):
   x_min: 781.85, y_min: 41.440000000000005
   x_max: 784.73, y_max: 45.28
   width: 2.8799999999999955, height: 3.8399999999999963
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 781.85, y_min: 41.440000000000005
   x_max: 784.73, y_max: 45.28
   width: 2.8799999999999955, height: 3.8399999999999963
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 781.85, x_max: 784.73
   y_min: 41.440000000000005, y_max: 45.28
📍 AFTER SCALING:
   x_min: 390.925, x_max: 392.365
   y_min: 27.62666666666667, y_max: 30.186666666666667
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=390.925, y_min=27.62666666666667, x_max=392.365, y_max=30.186666666666667      
   🔄 Processing annotation 4/4: dog eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 4
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 4
Transformed annotations: 4
Original dims: (800, 600)
Final dims: (400, 400)
Transformation config: ['flip', 'resize']
Resize mode: stretch_to -> 400x400
Actual final canvas: (400, 400)
🔍 DEBUG: Transformation result: 4 annotations
   First transformed annotation: (0.0, 22.24, 23.669999999999995, 74.50666666666667)
🔍 DEBUG: About to call _debug_yolo_dump
   aug_filename: car_flip_horizontal.jpg
   transformed_annotations count: 4
   img_w, img_h: 400, 400
   First annotation: <class 'backend.core.annotation_transformer.BoundingBox'> - 0.0

=== DEBUG YOLO DUMP :: car_flip_horizontal.jpg ===
final canvas passed to YOLO: 400x400
⚠️  NO TRANSFORMATIONS APPLIED - using raw annotations
  ann[0] BBOX -> [0.00,22.24,23.67,74.51]
  ann[1] POLY -> 49 pts; min=(388.2,14.8) max=(400.0,49.7)
  ann[2] BBOX -> [15.27,41.44,18.15,45.28]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 4
   Final dims: 400x400
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 4
   Final dims: 400x400
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 2
  det: 1 0.029587 0.120933 0.059175 0.130667
  det: 15 0.041775 0.108400 0.007200 0.009600
YOLO SEG lines: 2
  seg: 1 1.000000 0.124178 1.000000 0.118489 1.000000 0.111733 1.000000 0.099644 1.000000 0.090400 1.000000 0.083467 0.999513 0...
🔍 DEBUG: _debug_yolo_dump returned:
   det_lines count: 2
   seg_lines count: 2
   First det_line: 1 0.029587 0.120933 0.059175 0.130667
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

=== 🔍 TRANSFORMATIONS DEBUG :: dog.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 400, 'height': 400}}, {'type': 'flip', 'params': {'horizontal': True}}]
transformations type: <class 'list'>
transformations bool: True
🎯 COMPLEX TRANSFORMATIONS for dog.jpg
🖼️ Original image dims: (800, 600)
🎯 ORIGINAL IMAGE: Applying ONLY resize (baseline behavior)
🖼️ Resized to: (400, 400) using mode: stretch_to

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 0}]       
🎯 ORIGINAL IMAGE BASELINE: Applied resize-only, augmented images will get full combinations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: object_detection
   Export format: yolo_detection
   ✅ Using DETECTION mode: yolo_detection
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 1
   Final dims: 400x400
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 400x400
🔧 TRANSFORM CONFIG: {'resize': {'enabled': True, 'width': 400, 'height': 400}}
📦 ORIGINAL ANNOTATIONS (1):
   1. dog: x_min=0.0, y_min=14.666666666666666, x_max=30.27, y_max=74.4

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 1 annotations
   📐 Dimensions: (800, 600) → (400, 400)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 400, 'height': 400}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 400x400
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=400x400
   🎯 FINAL CANVAS DIMENSIONS: (400, 400)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 1 annotations individually
   🔄 Processing annotation 1/1: dog
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog
         📦 Input bbox: x_min=0.0, y_min=14.666666666666666, x_max=30.27, y_max=74.4
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_detection
         🔧 Using bounding box coordinates for detection task...
         🔧 About to call _transform_bbox with temp bbox...

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: dog
   class_id: 1
   x_min: 0.0, y_min: 14.666666666666666
   x_max: 30.27, y_max: 74.4
   width: 30.27, height: 59.73333333333334
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 14.666666666666666
   x_max: 30.27, y_max: 74.4
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 0.0, y_min: 14.666666666666666
   x_max: 30.27, y_max: 74.4
   width: 30.27, height: 59.73333333333334
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 0.0, x_max: 30.27
   y_min: 14.666666666666666, y_max: 74.4
📍 AFTER SCALING:
   x_min: 0.0, x_max: 15.135
   y_min: 9.777777777777777, y_max: 49.6
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=0.0, y_min=9.777777777777777, x_max=15.135, y_max=49.6
   Original: 1 → Transformed: 1
📦 TRANSFORMED ANNOTATIONS (1):
   1. dog: x_min=0.0, y_min=14.666666666666666, x_max=30.27, y_max=74.4
✅ NEW DETECTION FUNCTION RESULT: 1 lines

🖼️ IMAGE GENERATION ORDER: ['flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['flip', 'resize'], 'geometric_transforms_order': ['flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 1 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 14.666666666666666, 30.27, 74.4)

🚀🚀🚀 NEW VERSION LOADED - FUNCTION CALLED! 🚀🚀🚀
   annotations count: 1
   tracking_data keys: ['transformation_sequence', 'transformation_config', 'original_dims', 'final_dims', 'debug_transformation_order', 'has_geometric_transforms', 'geometric_transforms', 'photometric_transforms', 'total_transforms', 'geometric_count', 'photometric_count']
🔥 IMMEDIATE CHECK: has_geometric_transforms = True
🔧 SKIPPING debug_logger.start_annotation_transformation (method doesn't exist)
🔍 CHECKING has_geometric_transforms:
   tracking_data.get('has_geometric_transforms'): True
   tracking_data.get('has_geometric_transforms', False): True
   not tracking_data.get('has_geometric_transforms', False): False
✅ HAS GEOMETRIC TRANSFORMS - proceeding with transformation
🔧 ABOUT TO IMPORT annotation_transformer...
✅ IMPORT SUCCESSFUL!

🎯 ANNOTATION TRANSFORMER INPUT:
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   original_dims: (800, 600)
   new_dims: (400, 400)
   annotation_count: 2

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 2
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   original_dims: (800, 600)
   new_dims: (400, 400)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 2 annotations
   📐 Dimensions: (800, 600) → (400, 400)
   🔧 Transform config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 400x400
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=400x400
   🎯 FINAL CANVAS DIMENSIONS: (400, 400)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 2 annotations individually
   🔄 Processing annotation 1/2: dog

🚀 STARTING BBOX TRANSFORMATION
================================================================================
📦 INPUT BBOX:
   class_name: dog
   class_id: 1
   x_min: 0.0, y_min: 14.666666666666666
   x_max: 30.27, y_max: 74.4
   width: 30.27, height: 59.73333333333334
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (400, 400)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 400, 'height': 400}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 14.666666666666666
   x_max: 30.27, y_max: 74.4
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. flip: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 0.0, y_min: 14.666666666666666
   x_max: 30.27, y_max: 74.4
   width: 30.27, height: 59.73333333333334
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=0.0, x_max=30.27
   After: x_min=769.73, x_max=800.0
📍 FINAL BBOX (after flip):
   x_min: 769.73, y_min: 14.666666666666666
   x_max: 800.0, y_max: 74.4
   width: 30.269999999999982, height: 59.73333333333334
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 400
   target_height: 400
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 769.73, y_min: 14.666666666666666
   x_max: 800.0, y_max: 74.4
   width: 30.269999999999982, height: 59.73333333333334
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 STRETCH_TO MODE:
   sx = 400.0 / 800.0 = 0.5
   sy = 400.0 / 600.0 = 0.6666666666666666
📍 BEFORE SCALING:
   x_min: 769.73, x_max: 800.0
   y_min: 14.666666666666666, y_max: 74.4
📍 AFTER SCALING:
   x_min: 384.865, x_max: 400.0
   y_min: 9.777777777777777, y_max: 49.6
🖼️ CANVAS SIZE: 400.0 x 400.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 400.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=384.865, y_min=9.777777777777777, x_max=400.0, y_max=49.6
   🔄 Processing annotation 2/2: dog
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 2
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 2
Transformed annotations: 2
Original dims: (800, 600)
Final dims: (400, 400)
Transformation config: ['flip', 'resize']
Resize mode: stretch_to -> 400x400
Actual final canvas: (400, 400)
🔍 DEBUG: Transformation result: 2 annotations
   First transformed annotation: (0.0, 14.666666666666666, 30.27, 74.4)
🔍 DEBUG: About to call _debug_yolo_dump
   aug_filename: dog_flip_horizontal.jpg
   transformed_annotations count: 2
   img_w, img_h: 400, 400
   First annotation: <class 'backend.core.annotation_transformer.BoundingBox'> - 0.0

=== DEBUG YOLO DUMP :: dog_flip_horizontal.jpg ===
final canvas passed to YOLO: 400x400
⚠️  NO TRANSFORMATIONS APPLIED - using raw annotations
  ann[0] BBOX -> [0.00,14.67,30.27,74.40]
  ann[1] POLY -> 54 pts; min=(384.9,9.8) max=(400.0,49.6)
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 2
   Final dims: 400x400
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 2
   Final dims: 400x400
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 1
  det: 1 0.037837 0.111333 0.075675 0.149333
YOLO SEG lines: 1
  seg: 1 1.000000 0.059822 1.000000 0.054667 0.999663 0.048622 0.997862 0.044533 0.996513 0.041511 0.996437 0.036533 0.994638 0...
🔍 DEBUG: _debug_yolo_dump returned:
   det_lines count: 1
   seg_lines count: 1
   First det_line: 1 0.037837 0.111333 0.075675 0.149333
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

=== 📋 WRITING ANNOTATIONS.JSON ===
Total images with annotations: 6
   images\train\cat.jpg: 3 annotations
      First annotation: {'class_id': 0, 'bbox': [0.042037, 0.109867, 0.084075, 0.1448]}
   images\train\cat_flip_horizontal.jpg: 3 annotations
      First annotation: {'class_id': 12, 'bbox': [0.042037, 0.109867, 0.084075, 0.1448]}
   images\val\car.jpg: 2 annotations
      First annotation: {'class_id': 2, 'bbox': [0.029587, 0.120933, 0.059175, 0.130667]}
   images\val\car_flip_horizontal.jpg: 2 annotations
      First annotation: {'class_id': 1, 'bbox': [0.029587, 0.120933, 0.059175, 0.130667]}
   images\test\dog.jpg: 1 annotations
      First annotation: {'class_id': 2, 'bbox': [0.037837, 0.111333, 0.075675, 0.149333]}
   images\test\dog_flip_horizontal.jpg: 1 annotations
      First annotation: {'class_id': 1, 'bbox': [0.037837, 0.111333, 0.075675, 0.149333]}
INFO:     127.0.0.1:59594 - "POST /api/v1/logs/frontend/batch HTTP/1.1" 200 OK
INFO:     127.0.0.1:63652 - "POST /api/v1/releases/create HTTP/1.1" 200 OK
INFO:     127.0.0.1:59594 - "OPTIONS /api/transformation/available-transformations?_t=1758454420027 HTTP/1.1" 200 OK
INFO:     127.0.0.1:58492 - "OPTIONS /api/image-transformations/pending?_t=1758454420027 HTTP/1.1" 200 OK
INFO:     127.0.0.1:63246 - "OPTIONS /api/image-transformations/pending?_t=1758454420027 HTTP/1.1" 200 OK
INFO:     127.0.0.1:63123 - "OPTIONS /api/transformation/available-transformations?_t=1758454420027 HTTP/1.1" 200 OK
INFO:     127.0.0.1:59594 - "GET /api/transformation/available-transformations?_t=1758454420027 HTTP/1.1"
 200 OK
INFO:     127.0.0.1:63123 - "GET /api/transformation/available-transformations?_t=1758454420027 HTTP/1.1"
 200 OK
INFO:     127.0.0.1:63652 - "GET /api/v1/projects/1/releas