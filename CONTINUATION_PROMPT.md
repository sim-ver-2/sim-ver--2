# 🔄 ANNOTATION BUG INVESTIGATION - CONTINUATION PROMPT

**Use this prompt to continue our annotation transformation debugging session:**

---

## **CONTEXT RESTORATION PROMPT**

```
I'm continuing our annotation transformation bug investigation. Here's what we've discovered:

**CRITICAL BUG**: Annotations appear 7x smaller than expected after transformation.

**EVIDENCE**:
- Database stores correct pixel coordinates: Dog eye (454.5,288.5) to (502.5,324.5) = 48x36 pixels on 800x600 image
- Expected YOLO output: ~0.06 x 0.06 (6% x 6%)  
- Actual YOLO output: 0.008250 x 0.013333 (0.8% x 1.3%) - 7x SMALLER!

**WHAT WE'VE FIXED**:
- ✅ BoundingBox @dataclass decorator issue
- ✅ debug_logger crashes in annotation_transformer.py
- ✅ Confirmed transformations execute without errors
- ✅ Verified YOLO normalization math works correctly
- ✅ Confirmed database stores pixel coordinates (not normalized)
- ✅ User uses stretch_to resize mode only

**ROOT CAUSE IDENTIFIED**: Coordinates are being PRE-NORMALIZED/SHRUNK by 56x BEFORE reaching transformation! The transformation itself works correctly.

**EVIDENCE**: 
- Database: Cat eye (317.5, 204.5) to (372.5, 254.5) = 55x50 pixels ✅
- Transformation input: Cat eye (5.64, 46.15) to (8.28, 53.73) = 2.6x7.6 pixels ❌ (56x smaller!)
- Bug location: Between database loading and transformation function

**CURRENT STATE**:
- Repository: /workspace/project/sim-ver--1
- Branch: fix-annotation-transformations  
- Backend running on port 12000
- Files modified: annotation_transformer.py, releases.py
- Debug files: debug_note/onlyresei_box.md, ANNOTATION_BUG_REPORT.md

**IMMEDIATE TASK**: Find where coordinates get shrunk from 317.5 → 5.64 between database and transformation. The create_yolo_label_content function was removed but coordinates are still being pre-processed.

**KEY QUESTION**: What code is normalizing/shrinking database coordinates before they reach the transformation function?

Continue debugging from where we left off - focus on the resize scaling calculation.
```

---

**Save this prompt to restore our debugging session context in future conversations.**