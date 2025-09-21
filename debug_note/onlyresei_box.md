🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 3
   Final dims: 500x500
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 500x500
🔧 TRANSFORM CONFIG: {'resize': {'enabled': True, 'width': 500, 'height': 500}}
📦 ORIGINAL ANNOTATIONS (3):
   1. cat: x_min=0.0, y_min=21.29355555555556, x_max=26.903999999999996, y_max=103.58822222222223        
   2. cat eye: x_min=5.639999999999997, y_min=46.14866666666667, x_max=8.279999999999996, y_max=53.726444444444446
   3. cat eye: x_min=11.016, y_min=45.69400000000001, x_max=13.607999999999997, y_max=53.27177777777777  

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 3 annotations
   📐 Dimensions: (800, 600) → (500, 500)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 500, 'height': 500}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 500x500
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=500x500
   🎯 FINAL CANVAS DIMENSIONS: (500, 500)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 3 annotations individually
   🔄 Processing annotation 1/3: cat
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat
         📦 Input bbox: x_min=0.0, y_min=21.29355555555556, x_max=26.903999999999996, y_max=103.58822222222223
         📐 Dimensions: (800, 600) → (500, 500)
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
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   width: 26.903999999999996, height: 82.29466666666667
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (500, 500)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 500, 'height': 500}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 500
   target_height: 500
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   width: 26.903999999999996, height: 82.29466666666667
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 500.0, th: 500.0
🎯 STRETCH_TO MODE:
   sx = 500.0 / 800.0 = 0.625
   sy = 500.0 / 600.0 = 0.8333333333333334
📍 BEFORE SCALING:
   x_min: 0.0, x_max: 26.903999999999996
   y_min: 21.29355555555556, y_max: 103.58822222222223
📍 AFTER SCALING:
   x_min: 0.0, x_max: 16.814999999999998
   y_min: 17.744629629629635, y_max: 86.32351851851853
🖼️ CANVAS SIZE: 500.0 x 500.0
✅ RESIZE COMPLETE - NEW CANVAS: 500.0 x 500.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=0.0, y_min=17.744629629629635, x_max=16.814999999999998, y_max=86.32351851851853
   🔄 Processing annotation 2/3: cat eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat eye
         📦 Input bbox: x_min=5.639999999999997, y_min=46.14866666666667, x_max=8.279999999999996, y_max=53.726444444444446
         📐 Dimensions: (800, 600) → (500, 500)
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
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   width: 2.639999999999999, height: 7.577777777777776
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (500, 500)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 500, 'height': 500}
================================================================================
🔢 INITIAL VALUES:
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 500
   target_height: 500
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   width: 2.639999999999999, height: 7.577777777777776
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 500.0, th: 500.0
🎯 STRETCH_TO MODE:
   sx = 500.0 / 800.0 = 0.625
   sy = 500.0 / 600.0 = 0.8333333333333334
📍 BEFORE SCALING:
   x_min: 5.639999999999997, x_max: 8.279999999999996
   y_min: 46.14866666666667, y_max: 53.726444444444446
📍 AFTER SCALING:
   x_min: 3.524999999999998, x_max: 5.174999999999997
   y_min: 38.45722222222223, y_max: 44.77203703703704
🖼️ CANVAS SIZE: 500.0 x 500.0
✅ RESIZE COMPLETE - NEW CANVAS: 500.0 x 500.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=3.524999999999998, y_min=38.45722222222223, x_max=5.174999999999997, y_max=44.77203703703704
   🔄 Processing annotation 3/3: cat eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat eye
         📦 Input bbox: x_min=11.016, y_min=45.69400000000001, x_max=13.607999999999997, y_max=53.27177777777777
         📐 Dimensions: (800, 600) → (500, 500)
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
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   width: 2.591999999999997, height: 7.5777777777777615
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (500, 500)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 500, 'height': 500}
================================================================================
🔢 INITIAL VALUES:
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 500
   target_height: 500
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   width: 2.591999999999997, height: 7.5777777777777615
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 500.0, th: 500.0
🎯 STRETCH_TO MODE:
   sx = 500.0 / 800.0 = 0.625
   sy = 500.0 / 600.0 = 0.8333333333333334
📍 BEFORE SCALING:
   x_min: 11.016, x_max: 13.607999999999997
   y_min: 45.69400000000001, y_max: 53.27177777777777
📍 AFTER SCALING:
   x_min: 6.885, x_max: 8.504999999999999
   y_min: 38.07833333333334, y_max: 44.39314814814814
🖼️ CANVAS SIZE: 500.0 x 500.0
✅ RESIZE COMPLETE - NEW CANVAS: 500.0 x 500.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=6.885, y_min=38.07833333333334, x_max=8.504999999999999, y_max=44.39314814814814
   Original: 3 → Transformed: 3
📦 TRANSFORMED ANNOTATIONS (3):
   1. cat: x_min=0.0, y_min=21.29355555555556, x_max=26.903999999999996, y_max=103.58822222222223        
   2. cat eye: x_min=5.639999999999997, y_min=46.14866666666667, x_max=8.279999999999996, y_max=53.726444444444446
   3. cat eye: x_min=11.016, y_min=45.69400000000001, x_max=13.607999999999997, y_max=53.27177777777777  
✅ NEW DETECTION FUNCTION RESULT: 3 lines

=== 🔍 TRANSFORMATIONS DEBUG :: car.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 500, 'height': 500}}]
transformations type: <class 'list'>
transformations bool: True
🎯 RESIZE-ONLY DETECTED for car.jpg
🖼️ Original image dims: (800, 600)
🖼️ Resized image dims: (500, 500)

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 500, 'height': 500}}]
   Original dims: (800, 600)
   Final dims: (500, 500)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 500, 'height': 500}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 500, 'height': 500}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 500, 'height': 500}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 500, 'height': 500}, 'index': 0}]       
🎯 RESIZE-ONLY: Using tracking system for annotations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: object_detection
   Export format: yolo_detection
   ✅ Using DETECTION mode: yolo_detection
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 500, 'height': 500}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 500, 'height': 500}}, 'original_dims': (800, 600), 'final_dims': (500, 500), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 500, 'height': 500}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 2
   Final dims: 500x500
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 500x500
🔧 TRANSFORM CONFIG: {'resize': {'enabled': True, 'width': 500, 'height': 500}}
📦 ORIGINAL ANNOTATIONS (2):
   1. dog: x_min=0.0, y_min=31.59933333333333, x_max=18.935999999999996, y_max=105.86155555555557        
   2. dog eye: x_min=12.215999999999998, y_min=58.87933333333334, x_max=14.519999999999996, y_max=64.33533333333334

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 2 annotations
   📐 Dimensions: (800, 600) → (500, 500)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 500, 'height': 500}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 500x500
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=500x500
   🎯 FINAL CANVAS DIMENSIONS: (500, 500)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 2 annotations individually
   🔄 Processing annotation 1/2: dog
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog
         📦 Input bbox: x_min=0.0, y_min=31.59933333333333, x_max=18.935999999999996, y_max=105.86155555555557
         📐 Dimensions: (800, 600) → (500, 500)
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
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   width: 18.935999999999996, height: 74.26222222222223
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (500, 500)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 500, 'height': 500}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 500
   target_height: 500
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   width: 18.935999999999996, height: 74.26222222222223
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 500.0, th: 500.0
🎯 STRETCH_TO MODE:
   sx = 500.0 / 800.0 = 0.625
   sy = 500.0 / 600.0 = 0.8333333333333334
📍 BEFORE SCALING:
   x_min: 0.0, x_max: 18.935999999999996
   y_min: 31.59933333333333, y_max: 105.86155555555557
📍 AFTER SCALING:
   x_min: 0.0, x_max: 11.834999999999997
   y_min: 26.332777777777775, y_max: 88.21796296296297
🖼️ CANVAS SIZE: 500.0 x 500.0
✅ RESIZE COMPLETE - NEW CANVAS: 500.0 x 500.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=0.0, y_min=26.332777777777775, x_max=11.834999999999997, y_max=88.21796296296297
   🔄 Processing annotation 2/2: dog eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog eye
         📦 Input bbox: x_min=12.215999999999998, y_min=58.87933333333334, x_max=14.519999999999996, y_max=64.33533333333334
         📐 Dimensions: (800, 600) → (500, 500)
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
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   width: 2.3039999999999985, height: 5.455999999999996
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (500, 500)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 500, 'height': 500}
================================================================================
🔢 INITIAL VALUES:
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 500
   target_height: 500
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   width: 2.3039999999999985, height: 5.455999999999996
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 500.0, th: 500.0
🎯 STRETCH_TO MODE:
   sx = 500.0 / 800.0 = 0.625
   sy = 500.0 / 600.0 = 0.8333333333333334
📍 BEFORE SCALING:
   x_min: 12.215999999999998, x_max: 14.519999999999996
   y_min: 58.87933333333334, y_max: 64.33533333333334
📍 AFTER SCALING:
   x_min: 7.634999999999998, x_max: 9.074999999999998
   y_min: 49.06611111111112, y_max: 53.61277777777779
🖼️ CANVAS SIZE: 500.0 x 500.0
✅ RESIZE COMPLETE - NEW CANVAS: 500.0 x 500.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=7.634999999999998, y_min=49.06611111111112, x_max=9.074999999999998, y_max=53.61277777777779
   Original: 2 → Transformed: 2
📦 TRANSFORMED ANNOTATIONS (2):
   1. dog: x_min=0.0, y_min=31.59933333333333, x_max=18.935999999999996, y_max=105.86155555555557        
   2. dog eye: x_min=12.215999999999998, y_min=58.87933333333334, x_max=14.519999999999996, y_max=64.33533333333334
✅ NEW DETECTION FUNCTION RESULT: 2 lines

=== 🔍 TRANSFORMATIONS DEBUG :: dog.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 500, 'height': 500}}]
transformations type: <class 'list'>
transformations bool: True
🎯 RESIZE-ONLY DETECTED for dog.jpg
🖼️ Original image dims: (800, 600)
🖼️ Resized image dims: (500, 500)

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 500, 'height': 500}}]
   Original dims: (800, 600)
   Final dims: (500, 500)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 500, 'height': 500}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 500, 'height': 500}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 500, 'height': 500}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 500, 'height': 500}, 'index': 0}]       
🎯 RESIZE-ONLY: Using tracking system for annotations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: object_detection
   Export format: yolo_detection
   ✅ Using DETECTION mode: yolo_detection
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 500, 'height': 500}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 500, 'height': 500}}, 'original_dims': (800, 600), 'final_dims': (500, 500), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 500, 'height': 500}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 1
   Final dims: 500x500
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 500x500
🔧 TRANSFORM CONFIG: {'resize': {'enabled': True, 'width': 500, 'height': 500}}
📦 ORIGINAL ANNOTATIONS (1):
   1. dog: x_min=0.0, y_min=20.83888888888889, x_max=24.216, y_max=105.71000000000002

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 1 annotations
   📐 Dimensions: (800, 600) → (500, 500)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 500, 'height': 500}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 500x500
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=500x500
   🎯 FINAL CANVAS DIMENSIONS: (500, 500)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 1 annotations individually
   🔄 Processing annotation 1/1: dog
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog
         📦 Input bbox: x_min=0.0, y_min=20.83888888888889, x_max=24.216, y_max=105.71000000000002       
         📐 Dimensions: (800, 600) → (500, 500)
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
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   width: 24.216, height: 84.87111111111113
📐 DIMENSIONS:
   original_dims: (800, 600)
   new_dims: (500, 500)
🔧 TRANSFORMATION CONFIG:
   1. resize: {'enabled': True, 'width': 500, 'height': 500}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 1
   1. resize: enabled=True, affects_coordinates=True


🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 500
   target_height: 500
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   width: 24.216, height: 84.87111111111113
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 500.0, th: 500.0
🎯 STRETCH_TO MODE:
   sx = 500.0 / 800.0 = 0.625
   sy = 500.0 / 600.0 = 0.8333333333333334
📍 BEFORE SCALING:
   x_min: 0.0, x_max: 24.216
   y_min: 20.83888888888889, y_max: 105.71000000000002
📍 AFTER SCALING:
   x_min: 0.0, x_max: 15.135000000000002
   y_min: 17.36574074074074, y_max: 88.09166666666668
🖼️ CANVAS SIZE: 500.0 x 500.0
✅ RESIZE COMPLETE - NEW CANVAS: 500.0 x 500.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=0.0, y_min=17.36574074074074, x_max=15.135000000000002, y_max=88.09166666666668
   Original: 1 → Transformed: 1
📦 TRANSFORMED ANNOTATIONS (1):
   1. dog: x_min=0.0, y_min=20.83888888888889, x_max=24.216, y_max=105.71000000000002
✅ NEW DETECTION FUNCTION RESULT: 1 lines

=== 📋 WRITING ANNOTATIONS.JSON ===
Total images with annotations: 3
   images\train\cat.jpg: 3 annotations
      First annotation: {'class_id': 0, 'bbox': [0.026904, 0.124882, 0.053808, 0.164589]}
   images\val\car.jpg: 2 annotations
      First annotation: {'class_id': 2, 'bbox': [0.018936, 0.137461, 0.037872, 0.148524]}
   images\test\dog.jpg: 1 annotations
      First annotation: {'class_id': 2, 'bbox': [0.024216, 0.126549, 0.048432, 0.169742]}
INFO:     127.0.0.1:57011 - "POST /api/v1/logs/frontend/batch HTTP/1.1" 200 OK
🔍 DEBUG: Database path being used: V:\stage-1-labeling-app\app-3-fix-release-system-422-error\database.db
🔍 DEBUG: Database exists: True
🔍 DEBUG: SQL query returned 2 projects
INFO:     127.0.0.1:61390 - "POST /api/v1/releases/create HTTP/1.1" 200 OK
INFO:     127.0.0.1:57011 - "OPTIONS /api/transformation/available-transformations?_t=1758457097281 HTTP/1.1" 200 OK
INFO:     127.0.0.1:64768 - "OPTIONS /api/image-transformations/pending?_t=1758457097281 HTTP/1.1" 200 OK
INFO:     127.0.0.1:56004 - "OPTIONS /api/image-transformations/pending?_t=1758457097281 HTTP/1.1" 200 OK
INFO:     127.0.0.1:51245 - "OPTIONS /api/transformation/available-transformations?_t=1758457097281 HTTP/1.1" 200 OK
INFO:     127.0.0.1:57011 - "GET /api/transformation/available-transformations?_t=1758457097281 HTTP/1.1"
 200 OK
INFO:     127.0.0.1:61390 - "GET /api/v1/projects/1/releases HTTP/1.1" 200 OK
INFO:     127.0.0.1:51245 - "GET /api/transformation/available-transformations?_t=1758457097281 HTTP/1.1"
 200 OK
INFO:     127.0.0.1:64768 - "GET /api/image-transformations/pending?_t=1758457097281 HTT