
=== 🔍 TRANSFORMATIONS DEBUG :: cat.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, {'type': 'rotate', 'params': {'angle': 29.4}}]
transformations type: <class 'list'>
transformations bool: True
🎯 COMPLEX TRANSFORMATIONS for cat.jpg
🖼️ Original image dims: (800, 600)
🎯 ORIGINAL IMAGE: Applying ONLY resize (baseline behavior)
🖼️ Resized to: (400, 300) using mode: fit_within

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}]
   Original dims: (800, 600)
   Final dims: (400, 300)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 0}]
🎯 ORIGINAL IMAGE BASELINE: Applied resize-only, augmented images will get full combinations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: object_detection
   Export format: yolo_detection
   ✅ Using DETECTION mode: yolo_detection
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, 'original_dims': (800, 600), 'final_dims': (400, 300), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 3
   Final dims: 400x300
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 400x300
🔧 TRANSFORM CONFIG: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
📦 ORIGINAL ANNOTATIONS (3):
   1. cat: x_min=0.0, y_min=14.986666666666668, x_max=33.629999999999995, y_max=72.90666666666667        
   2. cat eye: x_min=7.049999999999995, y_min=32.480000000000004, x_max=10.349999999999994, y_max=37.81333333333333
   3. cat eye: x_min=13.769999999999998, y_min=32.160000000000004, x_max=17.009999999999998, y_max=37.493333333333325

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 3 annotations
   📐 Dimensions: (800, 600) → (400, 300)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: fit_within
   📏 Target size: 400x400
   📏 Original size: 800.0x600.0
   📐 FIT_WITHIN: scale=0.5000, final_canvas=400x300
   🎯 FINAL CANVAS DIMENSIONS: (400, 300)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 3 annotations individually
   🔄 Processing annotation 1/3: cat
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat
         📦 Input bbox: x_min=0.0, y_min=14.986666666666668, x_max=33.629999999999995, y_max=72.90666666666667
         📐 Dimensions: (800, 600) → (400, 300)
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
   new_dims: (400, 300)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}
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
   resize_mode: fit_within
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 0.0, y_min: 14.986666666666668
   x_max: 33.629999999999995, y_max: 72.90666666666667
   width: 33.629999999999995, height: 57.92
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 FIT_WITHIN MODE:
   s = min(400.0/800.0, 400.0/600.0) = min(0.5, 0.6666666666666666) = 0.5
📍 BEFORE SCALING:
   x_min: 0.0, x_max: 33.629999999999995
   y_min: 14.986666666666668, y_max: 72.90666666666667
📍 AFTER SCALING:
   x_min: 0.0, x_max: 16.814999999999998
   y_min: 7.493333333333334, y_max: 36.45333333333333
🖼️ CANVAS SIZE: 400.0 x 300.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 300.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=0.0, y_min=7.493333333333334, x_max=16.814999999999998, y_max=36.45333333333333
   🔄 Processing annotation 2/3: cat eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat eye
         📦 Input bbox: x_min=7.049999999999995, y_min=32.480000000000004, x_max=10.349999999999994, y_max=37.81333333333333
         📐 Dimensions: (800, 600) → (400, 300)
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
   new_dims: (400, 300)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}
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
   resize_mode: fit_within
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 7.049999999999995, y_min: 32.480000000000004
   x_max: 10.349999999999994, y_max: 37.81333333333333
   width: 3.299999999999999, height: 5.333333333333329
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 FIT_WITHIN MODE:
   s = min(400.0/800.0, 400.0/600.0) = min(0.5, 0.6666666666666666) = 0.5
📍 BEFORE SCALING:
   x_min: 7.049999999999995, x_max: 10.349999999999994
   y_min: 32.480000000000004, y_max: 37.81333333333333
📍 AFTER SCALING:
   x_min: 3.5249999999999977, x_max: 5.174999999999997
   y_min: 16.240000000000002, y_max: 18.906666666666666
🖼️ CANVAS SIZE: 400.0 x 300.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 300.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=3.5249999999999977, y_min=16.240000000000002, x_max=5.174999999999997, y_max=18.906666666666666
   🔄 Processing annotation 3/3: cat eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat eye
         📦 Input bbox: x_min=13.769999999999998, y_min=32.160000000000004, x_max=17.009999999999998, y_max=37.493333333333325
         📐 Dimensions: (800, 600) → (400, 300)
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
   new_dims: (400, 300)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}
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
   resize_mode: fit_within
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 13.769999999999998, y_min: 32.160000000000004
   x_max: 17.009999999999998, y_max: 37.493333333333325
   width: 3.24, height: 5.3333333333333215
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 FIT_WITHIN MODE:
   s = min(400.0/800.0, 400.0/600.0) = min(0.5, 0.6666666666666666) = 0.5
📍 BEFORE SCALING:
   x_min: 13.769999999999998, x_max: 17.009999999999998
   y_min: 32.160000000000004, y_max: 37.493333333333325
📍 AFTER SCALING:
   x_min: 6.884999999999999, x_max: 8.504999999999999
   y_min: 16.080000000000002, y_max: 18.746666666666663
🖼️ CANVAS SIZE: 400.0 x 300.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 300.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=6.884999999999999, y_min=16.080000000000002, x_max=8.504999999999999, y_max=18.746666666666663
   Original: 3 → Transformed: 3
📦 TRANSFORMED ANNOTATIONS (3):
   1. cat: x_min=0.0, y_min=14.986666666666668, x_max=33.629999999999995, y_max=72.90666666666667        
   2. cat eye: x_min=7.049999999999995, y_min=32.480000000000004, x_max=10.349999999999994, y_max=37.81333333333333
   3. cat eye: x_min=13.769999999999998, y_min=32.160000000000004, x_max=17.009999999999998, y_max=37.493333333333325
✅ NEW DETECTION FUNCTION RESULT: 3 lines

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']
🔍 DEBUG: Database path being used: V:\stage-1-labeling-app\app-3-fix-release-system-422-error\database.db
🔍 DEBUG: Database exists: True
🔍 DEBUG: SQL query returned 2 projects

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 29.4}}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}]
   Original dims: (800, 600)
   Final dims: (400, 369)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 29.4}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, 'original_dims': (800, 600), 'final_dims': (400, 369), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 3 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 14.986666666666668, 33.629999999999995, 72.90666666666667)

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -29.4}}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}]
   Original dims: (800, 600)
   Final dims: (400, 369)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -29.4}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, 'original_dims': (800, 600), 'final_dims': (400, 369), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 3 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 14.986666666666668, 33.629999999999995, 72.90666666666667)

=== 🔍 TRANSFORMATIONS DEBUG :: car.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, {'type': 'rotate', 'params': {'angle': 29.4}}]
transformations type: <class 'list'>
transformations bool: True
🎯 COMPLEX TRANSFORMATIONS for car.jpg
🖼️ Original image dims: (800, 600)
🎯 ORIGINAL IMAGE: Applying ONLY resize (baseline behavior)
🖼️ Resized to: (400, 300) using mode: fit_within

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}]
   Original dims: (800, 600)
   Final dims: (400, 300)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 0}]
🎯 ORIGINAL IMAGE BASELINE: Applied resize-only, augmented images will get full combinations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: object_detection
   Export format: yolo_detection
   ✅ Using DETECTION mode: yolo_detection
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, 'original_dims': (800, 600), 'final_dims': (400, 300), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 2
   Final dims: 400x300
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 400x300
🔧 TRANSFORM CONFIG: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
📦 ORIGINAL ANNOTATIONS (2):
   1. dog: x_min=0.0, y_min=22.24, x_max=23.669999999999995, y_max=74.50666666666667
   2. dog eye: x_min=15.269999999999996, y_min=41.440000000000005, x_max=18.149999999999995, y_max=45.28 

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 2 annotations
   📐 Dimensions: (800, 600) → (400, 300)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: fit_within
   📏 Target size: 400x400
   📏 Original size: 800.0x600.0
   📐 FIT_WITHIN: scale=0.5000, final_canvas=400x300
   🎯 FINAL CANVAS DIMENSIONS: (400, 300)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 2 annotations individually
   🔄 Processing annotation 1/2: dog
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog
         📦 Input bbox: x_min=0.0, y_min=22.24, x_max=23.669999999999995, y_max=74.50666666666667        
         📐 Dimensions: (800, 600) → (400, 300)
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
   new_dims: (400, 300)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}
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
   resize_mode: fit_within
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 0.0, y_min: 22.24
   x_max: 23.669999999999995, y_max: 74.50666666666667
   width: 23.669999999999995, height: 52.26666666666668
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 FIT_WITHIN MODE:
   s = min(400.0/800.0, 400.0/600.0) = min(0.5, 0.6666666666666666) = 0.5
📍 BEFORE SCALING:
   x_min: 0.0, x_max: 23.669999999999995
   y_min: 22.24, y_max: 74.50666666666667
📍 AFTER SCALING:
   x_min: 0.0, x_max: 11.834999999999997
   y_min: 11.12, y_max: 37.25333333333334
🖼️ CANVAS SIZE: 400.0 x 300.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 300.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=0.0, y_min=11.12, x_max=11.834999999999997, y_max=37.25333333333334
   🔄 Processing annotation 2/2: dog eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog eye
         📦 Input bbox: x_min=15.269999999999996, y_min=41.440000000000005, x_max=18.149999999999995, y_max=45.28
         📐 Dimensions: (800, 600) → (400, 300)
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
   new_dims: (400, 300)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}
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
   resize_mode: fit_within
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 15.269999999999996, y_min: 41.440000000000005
   x_max: 18.149999999999995, y_max: 45.28
   width: 2.879999999999999, height: 3.8399999999999963
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 FIT_WITHIN MODE:
   s = min(400.0/800.0, 400.0/600.0) = min(0.5, 0.6666666666666666) = 0.5
📍 BEFORE SCALING:
   x_min: 15.269999999999996, x_max: 18.149999999999995
   y_min: 41.440000000000005, y_max: 45.28
📍 AFTER SCALING:
   x_min: 7.634999999999998, x_max: 9.074999999999998
   y_min: 20.720000000000002, y_max: 22.64
🖼️ CANVAS SIZE: 400.0 x 300.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 300.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=7.634999999999998, y_min=20.720000000000002, x_max=9.074999999999998, y_max=22.64
   Original: 2 → Transformed: 2
📦 TRANSFORMED ANNOTATIONS (2):
   1. dog: x_min=0.0, y_min=22.24, x_max=23.669999999999995, y_max=74.50666666666667
   2. dog eye: x_min=15.269999999999996, y_min=41.440000000000005, x_max=18.149999999999995, y_max=45.28 
✅ NEW DETECTION FUNCTION RESULT: 2 lines

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 29.4}}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}]
   Original dims: (800, 600)
   Final dims: (400, 369)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 29.4}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, 'original_dims': (800, 600), 'final_dims': (400, 369), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 2 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 22.24, 23.669999999999995, 74.50666666666667)

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -29.4}}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}]
   Original dims: (800, 600)
   Final dims: (400, 369)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -29.4}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, 'original_dims': (800, 600), 'final_dims': (400, 369), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 2 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 22.24, 23.669999999999995, 74.50666666666667)

=== 🔍 TRANSFORMATIONS DEBUG :: dog.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, {'type': 'rotate', 'params': {'angle': 29.4}}]
transformations type: <class 'list'>
transformations bool: True
🎯 COMPLEX TRANSFORMATIONS for dog.jpg
🖼️ Original image dims: (800, 600)
🎯 ORIGINAL IMAGE: Applying ONLY resize (baseline behavior)
🖼️ Resized to: (400, 300) using mode: fit_within

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}]
   Original dims: (800, 600)
   Final dims: (400, 300)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 0}]
🎯 ORIGINAL IMAGE BASELINE: Applied resize-only, augmented images will get full combinations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: object_detection
   Export format: yolo_detection
   ✅ Using DETECTION mode: yolo_detection
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, 'original_dims': (800, 600), 'final_dims': (400, 300), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 1
   Final dims: 400x300
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 400x300
🔧 TRANSFORM CONFIG: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
📦 ORIGINAL ANNOTATIONS (1):
   1. dog: x_min=0.0, y_min=14.666666666666666, x_max=30.27, y_max=74.4

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 1 annotations
   📐 Dimensions: (800, 600) → (400, 300)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: fit_within
   📏 Target size: 400x400
   📏 Original size: 800.0x600.0
   📐 FIT_WITHIN: scale=0.5000, final_canvas=400x300
   🎯 FINAL CANVAS DIMENSIONS: (400, 300)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 1 annotations individually
   🔄 Processing annotation 1/1: dog
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog
         📦 Input bbox: x_min=0.0, y_min=14.666666666666666, x_max=30.27, y_max=74.4
         📐 Dimensions: (800, 600) → (400, 300)
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
   new_dims: (400, 300)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}
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
   resize_mode: fit_within
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 0.0, y_min: 14.666666666666666
   x_max: 30.27, y_max: 74.4
   width: 30.27, height: 59.73333333333334
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 400.0, th: 400.0
🎯 FIT_WITHIN MODE:
   s = min(400.0/800.0, 400.0/600.0) = min(0.5, 0.6666666666666666) = 0.5
📍 BEFORE SCALING:
   x_min: 0.0, x_max: 30.27
   y_min: 14.666666666666666, y_max: 74.4
📍 AFTER SCALING:
   x_min: 0.0, x_max: 15.135
   y_min: 7.333333333333333, y_max: 37.2
🖼️ CANVAS SIZE: 400.0 x 300.0
✅ RESIZE COMPLETE - NEW CANVAS: 400.0 x 300.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=0.0, y_min=7.333333333333333, x_max=15.135, y_max=37.2
   Original: 1 → Transformed: 1
📦 TRANSFORMED ANNOTATIONS (1):
   1. dog: x_min=0.0, y_min=14.666666666666666, x_max=30.27, y_max=74.4
✅ NEW DETECTION FUNCTION RESULT: 1 lines

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 29.4}}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}]
   Original dims: (800, 600)
   Final dims: (400, 369)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 29.4}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, 'original_dims': (800, 600), 'final_dims': (400, 369), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 1 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 14.666666666666666, 30.27, 74.4)

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -29.4}}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}]
   Original dims: (800, 600)
   Final dims: (400, 369)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -29.4}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -29.4}, 'resize': {'enabled': True, 'width': 400, 'height': 400, 'resize_mode': 'fit_within'}}, 'original_dims': (800, 600), 'final_dims': (400, 369), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -29.4}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400, 'resize_mode': 'fit_within'}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 1 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 14.666666666666666, 30.27, 74.4)

=== 📋 WRITING ANNOTATIONS.JSON ===
Total images with annotations: 9
   images\train\cat.jpg: 3 annotations
      First annotation: {'class_id': 0, 'bbox': [0.042037, 0.146489, 0.084075, 0.193067]}
   images\train\cat_rotate-29.jpg: 0 annotations
   images\train\cat_rotate29.jpg: 0 annotations
   images\val\car.jpg: 2 annotations
      First annotation: {'class_id': 2, 'bbox': [0.029587, 0.161244, 0.059175, 0.174222]}
   images\val\car_rotate-29.jpg: 0 annotations
   images\val\car_rotate29.jpg: 0 annotations
   images\test\dog.jpg: 1 annotations
      First annotation: {'class_id': 2, 'bbox': [0.037837, 0.148444, 0.075675, 0.199111]}
   images\test\dog_rotate-29.jpg: 0 annotations
   images\test\dog_rotate29.jpg: 0 annotations
INFO:     127.0.0.1:60341 - "POST /api/v1/releases/create HTTP/1.1" 200 Os