
=== 🔍 TRANSFORMATIONS DEBUG :: cat.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}}, {'type': 'rotate', 'params': {'angle': 63.1}}, {'type': 'flip', 'params': {'horizontal': True}}]
transformations type: <class 'list'>
transformations bool: True
🎯 COMPLEX TRANSFORMATIONS for cat.jpg
🖼️ Original image dims: (800, 600)
🎯 ORIGINAL IMAGE: Applying ONLY resize (baseline behavior)
🖼️ Resized to: (1024, 1023) using mode: stretch_to

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 0}]     
🎯 ORIGINAL IMAGE BASELINE: Applied resize-only, augmented images will get full combinations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: segmentation
   Export format: yolo_segmentation
   ✅ Using SEGMENTATION mode: yolo_segmentation
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 3
   Final dims: 1024x1023
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 1024x1023

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 3 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 3 annotations individually
   🔄 Processing annotation 1/3: cat
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat
         📦 Input bbox: x_min=0.0, y_min=12.48888888888889, x_max=21.018749999999997, y_max=60.75555555555556
         📐 Dimensions: (800, 600) → (1024, 1023)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 77 points...
         🔧 _transform_polygon returned: Polygon(points=[(0.0, 100.70866666666669), (0.0, 97.22288888888892), (0.0, 89.79666666666668), (0.0, 87.22022222222223), (0.0, 86.614), (0.0, 76.91444444444447), (0.6959999999999968, 67.36644444444445), (1.4639999999999969, 60.698000000000015), (2.279999999999997, 52.059333333333335), (2.615999999999996, 47.512666666666675), (2.7599999999999967, 42.81444444444445), (2.711999999999997, 37.96466666666667), (2.375999999999996, 32.05400000000001), (2.135999999999996, 24.324666666666666), (2.4719999999999964, 21.29355555555556), (3.479999999999997, 23.56688888888889), (5.351999999999996, 26.901111111111106), (6.839999999999998, 31.59933333333333), (8.039999999999997, 32.35711111111111), (10.103999999999997, 32.35711111111111), (12.072, 32.05400000000001), (13.559999999999995, 30.386888888888887), (15.239999999999998, 24.93088888888889), (17.352, 24.173111111111115), (17.304, 28.265111111111114), (16.631999999999998, 33.56955555555556), (16.2, 39.93488888888889), (16.008, 45.69400000000001), (16.103999999999996, 50.24066666666667), (16.008, 55.69666666666668), (15.767999999999995, 62.51666666666668), (16.631999999999998, 64.4868888888889), (17.927999999999997, 65.8508888888889), (19.079999999999995, 69.18511111111113), (20.471999999999998, 71.45844444444445), (19.943999999999996, 75.09577777777778), (18.168, 71.9131111111111), (16.967999999999996, 68.73044444444446), (16.535999999999998, 68.42733333333335), (18.072, 72.51933333333334), (18.791999999999998, 75.55044444444445), (18.888, 78.73311111111111), (17.927999999999997, 79.4908888888889), (17.447999999999997, 76.15666666666668), (16.823999999999998, 74.33800000000001), (16.055999999999997, 72.06466666666668), (15.815999999999997, 71.45844444444445), (16.055999999999997, 75.55044444444445), (16.823999999999998, 77.21755555555556), (18.503999999999998, 78.43000000000002), (19.703999999999997, 77.67222222222223), (20.855999999999998, 78.1268888888889), (22.44, 80.40022222222224), (26.519999999999992, 85.25000000000001), (26.903999999999996, 87.06866666666667), (26.615999999999996, 88.58422222222224), (24.407999999999998, 88.43266666666668), (22.631999999999994, 88.58422222222224), (19.8, 88.73577777777778), (19.272000000000002, 88.73577777777778), (19.224, 91.91844444444446), (18.935999999999996, 95.70733333333332), (17.927999999999997, 98.13222222222224), (16.392, 99.79933333333337), (14.999999999999998, 97.98066666666669), (14.375999999999998, 94.34333333333335), (13.991999999999996, 91.31222222222223), (13.799999999999995, 89.19044444444445), (11.927999999999997, 88.88733333333334), (8.567999999999996, 89.64511111111112), (5.207999999999995, 89.19044444444445), (4.295999999999997, 89.19044444444445), (4.535999999999996, 93.7371111111111), (4.295999999999997, 98.28377777777776), (3.1439999999999957, 100.70866666666669), (1.6559999999999968, 103.58822222222223), (0.6479999999999959, 102.83044444444445)], class_name='cat', class_id=12, confidence=1.0)
         📦 Updated bounding box: x_min=0.0, y_min=21.29355555555556, x_max=26.903999999999996, y_max=103.58822222222223
         📦 Updated annotation with 77 transformed points
   🔄 Processing annotation 2/3: cat eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat eye
         📦 Input bbox: x_min=4.406249999999997, y_min=27.06666666666667, x_max=6.4687499999999964, y_max=31.511111111111113
         📐 Dimensions: (800, 600) → (1024, 1023)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 8 points...
         🔧 _transform_polygon returned: Polygon(points=[(7.127999999999998, 53.726444444444446), (6.071999999999996, 52.059333333333335), (5.639999999999997, 49.33133333333333), (5.735999999999999, 46.75488888888889), (7.175999999999997, 46.14866666666667), (7.991999999999996, 47.512666666666675), (8.279999999999996, 49.786), (7.991999999999996, 52.059333333333335)], class_name='cat eye', class_id=16, confidence=1.0)
         📦 Updated bounding box: x_min=5.639999999999997, y_min=46.14866666666667, x_max=8.279999999999996, y_max=53.726444444444446
         📦 Updated annotation with 8 transformed points
   🔄 Processing annotation 3/3: cat eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat eye
         📦 Input bbox: x_min=8.60625, y_min=26.800000000000004, x_max=10.631249999999998, y_max=31.24444444444444
         📐 Dimensions: (800, 600) → (1024, 1023)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 6 points...
         🔧 _transform_polygon returned: Polygon(points=[(11.016, 51.90777777777779), (11.159999999999995, 48.11888888888888), (12.359999999999998, 45.69400000000001), (13.32, 47.05800000000001), (13.607999999999997, 50.69533333333332), (12.887999999999998, 53.27177777777777)], class_name='cat eye', class_id=16, confidence=1.0)
         📦 Updated bounding box: x_min=11.016, y_min=45.69400000000001, x_max=13.607999999999997, y_max=53.27177777777777
         📦 Updated annotation with 6 transformed points
   Original: 3 → Transformed: 3
✅ NEW SEGMENTATION FUNCTION RESULT: 3 lines

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 63.1}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 3 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 21.29355555555556, 26.903999999999996, 103.58822222222223)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 6

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 6
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 6 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 6 annotations individually
   🔄 Processing annotation 1/6: cat

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   width: 26.903999999999996, height: 82.29466666666667
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-400.0, -278.70644444444446), (-373.096, -278.70644444444446), (-400.0, -196.4117777777778), (-373.096, -196.4117777777778)]
   corner 0: (-400.0, -278.70644444444446) → (467.57583491589537, -182.81548101762837)
   corner 1: (-373.096, -278.70644444444446) → (479.74813833521955, -158.82256028112965)
   corner 2: (-400.0, -196.4117777777778) → (394.18565448287745, -145.58251742638498)
   corner 3: (-373.096, -196.4117777777778) → (406.35795790220163, -121.58959668988626)
   all x coords: [467.57583491589537, 479.74813833521955, 394.18565448287745, 406.35795790220163]        
   all y coords: [-182.81548101762837, -158.82256028112965, -145.58251742638498, -121.58959668988626]    
   new bounds: x_min=394.18565448287745, x_max=479.74813833521955, y_min=-182.81548101762837, y_max=-121.58959668988626
📍 FINAL BBOX (after rotation):
   x_min: 394.18565448287745, y_min: -182.81548101762837
   x_max: 479.74813833521955, y_max: -121.58959668988626
   width: 85.5624838523421, height: 61.22588432774211
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 394.18565448287745, y_min: -182.81548101762837
   x_max: 479.74813833521955, y_max: -121.58959668988626
   width: 85.5624838523421, height: 61.22588432774211
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 394.18565448287745, x_max: 479.74813833521955
   y_min: -182.81548101762837, y_max: -121.58959668988626
📍 AFTER SCALING:
   x_min: 504.55763773808314, x_max: 614.077617069081
   y_min: -311.7003951350564, y_max: -207.3102623562561
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=504.55763773808314, y_min=-311.7003951350564, x_max=614.077617069081, y_max=-207.3102623562561
   🔄 Processing annotation 2/6: cat
   🔄 Processing annotation 3/6: cat eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   width: 2.639999999999999, height: 7.577777777777776
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-394.36, -253.85133333333334), (-391.72, -253.85133333333334), (-394.36, -246.27355555555556), (-391.72, -246.27355555555556)]
   corner 0: (-394.36, -253.85133333333334) → (447.96183998946185, -166.5404279801873)
   corner 1: (-391.72, -253.85133333333334) → (449.1562676220449, -164.1860825020296)
   corner 2: (-394.36, -246.27355555555556) → (441.2039964873423, -163.11197829406916)
   corner 3: (-391.72, -246.27355555555556) → (442.3984241199254, -160.75763281591145)
   all x coords: [447.96183998946185, 449.1562676220449, 441.2039964873423, 442.3984241199254]
   all y coords: [-166.5404279801873, -164.1860825020296, -163.11197829406916, -160.75763281591145]      
   new bounds: x_min=441.2039964873423, x_max=449.1562676220449, y_min=-166.5404279801873, y_max=-160.75763281591145
📍 FINAL BBOX (after rotation):
   x_min: 441.2039964873423, y_min: -166.5404279801873
   x_max: 449.1562676220449, y_max: -160.75763281591145
   width: 7.952271134702585, height: 5.7827951642758535
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 441.2039964873423, y_min: -166.5404279801873
   x_max: 449.1562676220449, y_max: -160.75763281591145
   width: 7.952271134702585, height: 5.7827951642758535
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 441.2039964873423, x_max: 449.1562676220449
   y_min: -166.5404279801873, y_max: -160.75763281591145
📍 AFTER SCALING:
   x_min: 564.7411155037981, x_max: 574.9200225562174
   y_min: -283.95142970621936, y_max: -274.09176395112905
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=564.7411155037981, y_min=-283.95142970621936, x_max=574.9200225562174, y_max=-274.09176395112905
   🔄 Processing annotation 4/6: cat eye
   🔄 Processing annotation 5/6: cat eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   width: 2.591999999999997, height: 7.5777777777777615
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-388.984, -254.30599999999998), (-386.392, -254.30599999999998), (-388.984, -246.72822222222223), (-386.392, -246.72822222222223)]
   corner 0: (-388.984, -254.30599999999998) → (450.79959959684913, -161.9518314421968)
   corner 1: (-386.392, -254.30599999999998) → (451.97231036338525, -159.6402922454601)
   corner 2: (-388.984, -246.72822222222223) → (444.04175609472964, -158.5233817560786)
   corner 3: (-386.392, -246.72822222222223) → (445.21446686126575, -156.2118425593419)
   all x coords: [450.79959959684913, 451.97231036338525, 444.04175609472964, 445.21446686126575]        
   all y coords: [-161.9518314421968, -159.6402922454601, -158.5233817560786, -156.2118425593419]        
   new bounds: x_min=444.04175609472964, x_max=451.97231036338525, y_min=-161.9518314421968, y_max=-156.2118425593419
📍 FINAL BBOX (after rotation):
   x_min: 444.04175609472964, y_min: -161.9518314421968
   x_max: 451.97231036338525, y_max: -156.2118425593419
   width: 7.930554268655612, height: 5.739988882854902
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 444.04175609472964, y_min: -161.9518314421968
   x_max: 451.97231036338525, y_max: -156.2118425593419
   width: 7.930554268655612, height: 5.739988882854902
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 444.04175609472964, x_max: 451.97231036338525
   y_min: -161.9518314421968, y_max: -156.2118425593419
📍 AFTER SCALING:
   x_min: 568.373447801254, x_max: 578.5245572651331
   y_min: -276.12787260894555, y_max: -266.34119156367797
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=568.373447801254, y_min=-276.12787260894555, x_max=578.5245572651331, y_max=-266.34119156367797
   🔄 Processing annotation 6/6: cat eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 6
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 6
Transformed annotations: 6
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 6 annotations
   First transformed annotation: (0.0, 21.29355555555556, 26.903999999999996, 103.58822222222223)        

=== DEBUG YOLO DUMP :: cat_rotate63.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,21.29,26.90,103.59]
  ann[1] POLY -> 77 pts; min=(505.5,0.0) max=(605.3,0.0)
  ann[2] BBOX -> [5.64,46.15,8.28,53.73]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 6
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 6
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 3
  det: 12 0.013137 0.061037 0.026273 0.080444
  det: 16 0.006797 0.048815 0.002578 0.007407
  det: 16 0.012023 0.048370 0.002531 0.007407
YOLO SEG lines: 3
  seg: 12 0.495942 0.000000 0.499828 0.000000 0.508106 0.000000 0.510978 0.000000 0.511654 0.000000 0.522467 0.000000 0.533504 ...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['flip', 'resize'], 'geometric_transforms_order': ['flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 3 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 21.29355555555556, 26.903999999999996, 103.58822222222223)

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
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 6

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 6
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 6 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 6 annotations individually
   🔄 Processing annotation 1/6: cat

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
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
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   width: 26.903999999999996, height: 82.29466666666667
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=0.0, x_max=26.903999999999996
   After: x_min=773.096, x_max=800.0
📍 FINAL BBOX (after flip):
   x_min: 773.096, y_min: 21.29355555555556
   x_max: 800.0, y_max: 103.58822222222223
   width: 26.903999999999996, height: 82.29466666666667
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 773.096, y_min: 21.29355555555556
   x_max: 800.0, y_max: 103.58822222222223
   width: 26.903999999999996, height: 82.29466666666667
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 773.096, x_max: 800.0
   y_min: 21.29355555555556, y_max: 103.58822222222223
📍 AFTER SCALING:
   x_min: 989.5628800000001, x_max: 1024.0
   y_min: 36.305512222222234, y_max: 176.6179188888889
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=989.5628800000001, y_min=36.305512222222234, x_max=1024.0, y_max=176.6179188888889
   🔄 Processing annotation 2/6: cat
   🔄 Processing annotation 3/6: cat eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
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
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   width: 2.639999999999999, height: 7.577777777777776
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=5.639999999999997, x_max=8.279999999999996
   After: x_min=791.72, x_max=794.36
📍 FINAL BBOX (after flip):
   x_min: 791.72, y_min: 46.14866666666667
   x_max: 794.36, y_max: 53.726444444444446
   width: 2.6399999999999864, height: 7.577777777777776
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 791.72, y_min: 46.14866666666667
   x_max: 794.36, y_max: 53.726444444444446
   width: 2.6399999999999864, height: 7.577777777777776
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 791.72, x_max: 794.36
   y_min: 46.14866666666667, y_max: 53.726444444444446
📍 AFTER SCALING:
   x_min: 1013.4016, x_max: 1016.7808
   y_min: 78.68347666666668, y_max: 91.60358777777779
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=1013.4016, y_min=78.68347666666668, x_max=1016.7808, y_max=91.60358777777779   
   🔄 Processing annotation 4/6: cat eye
   🔄 Processing annotation 5/6: cat eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
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
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   width: 2.591999999999997, height: 7.5777777777777615
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=11.016, x_max=13.607999999999997
   After: x_min=786.392, x_max=788.984
📍 FINAL BBOX (after flip):
   x_min: 786.392, y_min: 45.69400000000001
   x_max: 788.984, y_max: 53.27177777777777
   width: 2.5919999999999845, height: 7.5777777777777615
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 786.392, y_min: 45.69400000000001
   x_max: 788.984, y_max: 53.27177777777777
   width: 2.5919999999999845, height: 7.5777777777777615
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 786.392, x_max: 788.984
   y_min: 45.69400000000001, y_max: 53.27177777777777
📍 AFTER SCALING:
   x_min: 1006.5817600000001, x_max: 1009.89952
   y_min: 77.90827000000002, y_max: 90.8283811111111
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=1006.5817600000001, y_min=77.90827000000002, x_max=1009.89952, y_max=90.8283811111111
   🔄 Processing annotation 6/6: cat eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 6
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 6
Transformed annotations: 6
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['flip', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 6 annotations
   First transformed annotation: (0.0, 21.29355555555556, 26.903999999999996, 103.58822222222223)        

=== DEBUG YOLO DUMP :: cat_flip_horizontal.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,21.29,26.90,103.59]
  ann[1] POLY -> 77 pts; min=(989.6,36.3) max=(1024.0,176.6)
  ann[2] BBOX -> [5.64,46.15,8.28,53.73]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 6
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 6
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 3
  det: 12 0.013137 0.061037 0.026273 0.080444
  det: 16 0.006797 0.048815 0.002578 0.007407
  det: 16 0.012023 0.048370 0.002531 0.007407
YOLO SEG lines: 3
  seg: 12 1.000000 0.167848 1.000000 0.162038 1.000000 0.149661 1.000000 0.145367 1.000000 0.144357 1.000000 0.128191 0.999130 ...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -63.1}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 3 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 21.29355555555556, 26.903999999999996, 103.58822222222223)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 6

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 6
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 6 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 6 annotations individually
   🔄 Processing annotation 1/6: cat

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   width: 26.903999999999996, height: 82.29466666666667
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-400.0, -278.70644444444446), (-373.096, -278.70644444444446), (-400.0, -196.4117777777778), (-373.096, -196.4117777777778)]
   corner 0: (-400.0, -278.70644444444446) → (-29.523602365321494, 530.6225426665429)
   corner 1: (-373.096, -278.70644444444446) → (-17.351298945997257, 506.6296219300442)
   corner 2: (-400.0, -196.4117777777778) → (43.86657806769642, 567.8555062577864)
   corner 3: (-373.096, -196.4117777777778) → (56.0388814870206, 543.8625855212877)
   all x coords: [-29.523602365321494, -17.351298945997257, 43.86657806769642, 56.0388814870206]
   all y coords: [530.6225426665429, 506.6296219300442, 567.8555062577864, 543.8625855212877]
   new bounds: x_min=-29.523602365321494, x_max=56.0388814870206, y_min=506.6296219300442, y_max=567.8555062577864
📍 FINAL BBOX (after rotation):
   x_min: -29.523602365321494, y_min: 506.6296219300442
   x_max: 56.0388814870206, y_max: 567.8555062577864
   width: 85.5624838523421, height: 61.225884327742165
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: -29.523602365321494, y_min: 506.6296219300442
   x_max: 56.0388814870206, y_max: 567.8555062577864
   width: 85.5624838523421, height: 61.225884327742165
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: -29.523602365321494, x_max: 56.0388814870206
   y_min: 506.6296219300442, y_max: 567.8555062577864
📍 AFTER SCALING:
   x_min: -37.79021102761151, x_max: 71.72976830338638
   y_min: 863.8035053907254, y_max: 968.1936381695258
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=-37.79021102761151, y_min=863.8035053907254, x_max=71.72976830338638, y_max=968.1936381695258
   🔄 Processing annotation 2/6: cat
   🔄 Processing annotation 3/6: cat eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   width: 2.639999999999999, height: 7.577777777777776
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-394.36, -253.85133333333334), (-391.72, -253.85133333333334), (-394.36, -246.27355555555556), (-391.72, -246.27355555555556)]
   corner 0: (-394.36, -253.85133333333334) → (-4.806143917851045, 536.8381195700372)
   corner 1: (-391.72, -253.85133333333334) → (-3.611716285267903, 534.4837740918795)
   corner 2: (-394.36, -246.27355555555556) → (1.9516995842685105, 540.2665692561552)
   corner 3: (-391.72, -246.27355555555556) → (3.146127216851596, 537.9122237779975)
   all x coords: [-4.806143917851045, -3.611716285267903, 1.9516995842685105, 3.146127216851596]
   all y coords: [536.8381195700372, 534.4837740918795, 540.2665692561552, 537.9122237779975]
   new bounds: x_min=-4.806143917851045, x_max=3.146127216851596, y_min=534.4837740918795, y_max=540.2665692561552
📍 FINAL BBOX (after rotation):
   x_min: -4.806143917851045, y_min: 534.4837740918795
   x_max: 3.146127216851596, y_max: 540.2665692561552
   width: 7.952271134702642, height: 5.78279516427574
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: -4.806143917851045, y_min: 534.4837740918795
   x_max: 3.146127216851596, y_max: 540.2665692561552
   width: 7.952271134702642, height: 5.78279516427574
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: -4.806143917851045, x_max: 3.146127216851596
   y_min: 534.4837740918795, y_max: 540.2665692561552
📍 AFTER SCALING:
   x_min: -6.151864214849338, x_max: 4.027042837570043
   y_min: 911.2948348266546, y_max: 921.1545005817446
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=-6.151864214849338, y_min=911.2948348266546, x_max=4.027042837570043, y_max=921.1545005817446
   🔄 Processing annotation 4/6: cat eye
   🔄 Processing annotation 5/6: cat eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   width: 2.591999999999997, height: 7.5777777777777615
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-388.984, -254.30599999999998), (-386.392, -254.30599999999998), (-388.984, -246.72822222222223), (-386.392, -246.72822222222223)]
   corner 0: (-388.984, -254.30599999999998) → (-2.7793255307179834, 531.8381090697123)
   corner 1: (-386.392, -254.30599999999998) → (-1.6066147641818702, 529.5265698729756)
   corner 2: (-388.984, -246.72822222222223) → (3.9785179714015158, 535.2665587558306)
   corner 3: (-386.392, -246.72822222222223) → (5.151228737937629, 532.9550195590939)
   all x coords: [-2.7793255307179834, -1.6066147641818702, 3.9785179714015158, 5.151228737937629]       
   all y coords: [531.8381090697123, 529.5265698729756, 535.2665587558306, 532.9550195590939]
   new bounds: x_min=-2.7793255307179834, x_max=5.151228737937629, y_min=529.5265698729756, y_max=535.2665587558306
📍 FINAL BBOX (after rotation):
   x_min: -2.7793255307179834, y_min: 529.5265698729756
   x_max: 5.151228737937629, y_max: 535.2665587558306
   width: 7.930554268655612, height: 5.739988882854959
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: -2.7793255307179834, y_min: 529.5265698729756
   x_max: 5.151228737937629, y_max: 535.2665587558306
   width: 7.930554268655612, height: 5.739988882854959
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: -2.7793255307179834, x_max: 5.151228737937629
   y_min: 529.5265698729756, y_max: 535.2665587558306
📍 AFTER SCALING:
   x_min: -3.5575366793190186, x_max: 6.593572784560165
   y_min: 902.8428016334235, y_max: 912.6294826786913
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=-3.5575366793190186, y_min=902.8428016334235, x_max=6.593572784560165, y_max=912.6294826786913
   🔄 Processing annotation 6/6: cat eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 6
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 6
Transformed annotations: 6
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 6 annotations
   First transformed annotation: (0.0, 21.29355555555556, 26.903999999999996, 103.58822222222223)        

=== DEBUG YOLO DUMP :: cat_rotate-63.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,21.29,26.90,103.59]
  ann[1] POLY -> 77 pts; min=(0.0,880.5) max=(61.3,966.6)
  ann[2] BBOX -> [5.64,46.15,8.28,53.73]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 6
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 6
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 3
  det: 12 0.013137 0.061037 0.026273 0.080444
  det: 16 0.006797 0.048815 0.002578 0.007407
  det: 16 0.012023 0.048370 0.002531 0.007407
YOLO SEG lines: 3
  seg: 12 0.051623 0.944254 0.047737 0.941626 0.039459 0.936026 0.036587 0.934083 0.035911 0.933626 0.025099 0.926312 0.014849 ...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['rotate', 'flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 63.1}}, {'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 2, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'flip', 'resize'], 'geometric_transforms_order': ['rotate', 'flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}], 'photometric_transforms': [], 'total_transforms': 3, 'geometric_count': 3, 'photometric_count': 0}
🔍 DEBUG: About to transform 3 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 21.29355555555556, 26.903999999999996, 103.58822222222223)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 6

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 6
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 6 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 6 annotations individually
   🔄 Processing annotation 1/6: cat

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   width: 26.903999999999996, height: 82.29466666666667
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-400.0, -278.70644444444446), (-373.096, -278.70644444444446), (-400.0, -196.4117777777778), (-373.096, -196.4117777777778)]
   corner 0: (-400.0, -278.70644444444446) → (467.57583491589537, -182.81548101762837)
   corner 1: (-373.096, -278.70644444444446) → (479.74813833521955, -158.82256028112965)
   corner 2: (-400.0, -196.4117777777778) → (394.18565448287745, -145.58251742638498)
   corner 3: (-373.096, -196.4117777777778) → (406.35795790220163, -121.58959668988626)
   all x coords: [467.57583491589537, 479.74813833521955, 394.18565448287745, 406.35795790220163]        
   all y coords: [-182.81548101762837, -158.82256028112965, -145.58251742638498, -121.58959668988626]    
   new bounds: x_min=394.18565448287745, x_max=479.74813833521955, y_min=-182.81548101762837, y_max=-121.58959668988626
📍 FINAL BBOX (after rotation):
   x_min: 394.18565448287745, y_min: -182.81548101762837
   x_max: 479.74813833521955, y_max: -121.58959668988626
   width: 85.5624838523421, height: 61.22588432774211
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 394.18565448287745, y_min: -182.81548101762837
   x_max: 479.74813833521955, y_max: -121.58959668988626
   width: 85.5624838523421, height: 61.22588432774211
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=394.18565448287745, x_max=479.74813833521955
   After: x_min=320.25186166478045, x_max=405.81434551712255
📍 FINAL BBOX (after flip):
   x_min: 320.25186166478045, y_min: -182.81548101762837
   x_max: 405.81434551712255, y_max: -121.58959668988626
   width: 85.5624838523421, height: 61.22588432774211
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 320.25186166478045, y_min: -182.81548101762837
   x_max: 405.81434551712255, y_max: -121.58959668988626
   width: 85.5624838523421, height: 61.22588432774211
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 320.25186166478045, x_max: 405.81434551712255
   y_min: -182.81548101762837, y_max: -121.58959668988626
📍 AFTER SCALING:
   x_min: 409.92238293091896, x_max: 519.4423622619169
   y_min: -311.7003951350564, y_max: -207.3102623562561
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=409.92238293091896, y_min=-311.7003951350564, x_max=519.4423622619169, y_max=-207.3102623562561
   🔄 Processing annotation 2/6: cat
   🔄 Processing annotation 3/6: cat eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   width: 2.639999999999999, height: 7.577777777777776
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-394.36, -253.85133333333334), (-391.72, -253.85133333333334), (-394.36, -246.27355555555556), (-391.72, -246.27355555555556)]
   corner 0: (-394.36, -253.85133333333334) → (447.96183998946185, -166.5404279801873)
   corner 1: (-391.72, -253.85133333333334) → (449.1562676220449, -164.1860825020296)
   corner 2: (-394.36, -246.27355555555556) → (441.2039964873423, -163.11197829406916)
   corner 3: (-391.72, -246.27355555555556) → (442.3984241199254, -160.75763281591145)
   all x coords: [447.96183998946185, 449.1562676220449, 441.2039964873423, 442.3984241199254]
   all y coords: [-166.5404279801873, -164.1860825020296, -163.11197829406916, -160.75763281591145]      
   new bounds: x_min=441.2039964873423, x_max=449.1562676220449, y_min=-166.5404279801873, y_max=-160.75763281591145
📍 FINAL BBOX (after rotation):
   x_min: 441.2039964873423, y_min: -166.5404279801873
   x_max: 449.1562676220449, y_max: -160.75763281591145
   width: 7.952271134702585, height: 5.7827951642758535
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 441.2039964873423, y_min: -166.5404279801873
   x_max: 449.1562676220449, y_max: -160.75763281591145
   width: 7.952271134702585, height: 5.7827951642758535
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=441.2039964873423, x_max=449.1562676220449
   After: x_min=350.8437323779551, x_max=358.7960035126577
📍 FINAL BBOX (after flip):
   x_min: 350.8437323779551, y_min: -166.5404279801873
   x_max: 358.7960035126577, y_max: -160.75763281591145
   width: 7.952271134702585, height: 5.7827951642758535
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 350.8437323779551, y_min: -166.5404279801873
   x_max: 358.7960035126577, y_max: -160.75763281591145
   width: 7.952271134702585, height: 5.7827951642758535
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 350.8437323779551, x_max: 358.7960035126577
   y_min: -166.5404279801873, y_max: -160.75763281591145
📍 AFTER SCALING:
   x_min: 449.0799774437826, x_max: 459.25888449620186
   y_min: -283.95142970621936, y_max: -274.09176395112905
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=449.0799774437826, y_min=-283.95142970621936, x_max=459.25888449620186, y_max=-274.09176395112905
   🔄 Processing annotation 4/6: cat eye
   🔄 Processing annotation 5/6: cat eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   width: 2.591999999999997, height: 7.5777777777777615
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-388.984, -254.30599999999998), (-386.392, -254.30599999999998), (-388.984, -246.72822222222223), (-386.392, -246.72822222222223)]
   corner 0: (-388.984, -254.30599999999998) → (450.79959959684913, -161.9518314421968)
   corner 1: (-386.392, -254.30599999999998) → (451.97231036338525, -159.6402922454601)
   corner 2: (-388.984, -246.72822222222223) → (444.04175609472964, -158.5233817560786)
   corner 3: (-386.392, -246.72822222222223) → (445.21446686126575, -156.2118425593419)
   all x coords: [450.79959959684913, 451.97231036338525, 444.04175609472964, 445.21446686126575]        
   all y coords: [-161.9518314421968, -159.6402922454601, -158.5233817560786, -156.2118425593419]        
   new bounds: x_min=444.04175609472964, x_max=451.97231036338525, y_min=-161.9518314421968, y_max=-156.2118425593419
📍 FINAL BBOX (after rotation):
   x_min: 444.04175609472964, y_min: -161.9518314421968
   x_max: 451.97231036338525, y_max: -156.2118425593419
   width: 7.930554268655612, height: 5.739988882854902
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 444.04175609472964, y_min: -161.9518314421968
   x_max: 451.97231036338525, y_max: -156.2118425593419
   width: 7.930554268655612, height: 5.739988882854902
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=444.04175609472964, x_max=451.97231036338525
   After: x_min=348.02768963661475, x_max=355.95824390527036
📍 FINAL BBOX (after flip):
   x_min: 348.02768963661475, y_min: -161.9518314421968
   x_max: 355.95824390527036, y_max: -156.2118425593419
   width: 7.930554268655612, height: 5.739988882854902
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 348.02768963661475, y_min: -161.9518314421968
   x_max: 355.95824390527036, y_max: -156.2118425593419
   width: 7.930554268655612, height: 5.739988882854902
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 348.02768963661475, x_max: 355.95824390527036
   y_min: -161.9518314421968, y_max: -156.2118425593419
📍 AFTER SCALING:
   x_min: 445.4754427348669, x_max: 455.6265521987461
   y_min: -276.12787260894555, y_max: -266.34119156367797
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=445.4754427348669, y_min=-276.12787260894555, x_max=455.6265521987461, y_max=-266.34119156367797
   🔄 Processing annotation 6/6: cat eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 6
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 6
Transformed annotations: 6
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'flip', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 6 annotations
   First transformed annotation: (0.0, 21.29355555555556, 26.903999999999996, 103.58822222222223)        

=== DEBUG YOLO DUMP :: cat_rotate63_flip_horizontal.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,21.29,26.90,103.59]
  ann[1] POLY -> 77 pts; min=(418.7,0.0) max=(518.5,0.0)
  ann[2] BBOX -> [5.64,46.15,8.28,53.73]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 6
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 6
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 3
  det: 12 0.013137 0.061037 0.026273 0.080444
  det: 16 0.006797 0.048815 0.002578 0.007407
  det: 16 0.012023 0.048370 0.002531 0.007407
YOLO SEG lines: 3
  seg: 12 0.504058 0.000000 0.500172 0.000000 0.491894 0.000000 0.489022 0.000000 0.488346 0.000000 0.477533 0.000000 0.466496 ...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['rotate', 'flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -63.1}}, {'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 2, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'flip', 'resize'], 'geometric_transforms_order': ['rotate', 'flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}], 'photometric_transforms': [], 'total_transforms': 3, 'geometric_count': 3, 'photometric_count': 0}
🔍 DEBUG: About to transform 3 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 21.29355555555556, 26.903999999999996, 103.58822222222223)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 6

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 6
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 6 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 6 annotations individually
   🔄 Processing annotation 1/6: cat

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 21.29355555555556
   x_max: 26.903999999999996, y_max: 103.58822222222223
   width: 26.903999999999996, height: 82.29466666666667
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-400.0, -278.70644444444446), (-373.096, -278.70644444444446), (-400.0, -196.4117777777778), (-373.096, -196.4117777777778)]
   corner 0: (-400.0, -278.70644444444446) → (-29.523602365321494, 530.6225426665429)
   corner 1: (-373.096, -278.70644444444446) → (-17.351298945997257, 506.6296219300442)
   corner 2: (-400.0, -196.4117777777778) → (43.86657806769642, 567.8555062577864)
   corner 3: (-373.096, -196.4117777777778) → (56.0388814870206, 543.8625855212877)
   all x coords: [-29.523602365321494, -17.351298945997257, 43.86657806769642, 56.0388814870206]
   all y coords: [530.6225426665429, 506.6296219300442, 567.8555062577864, 543.8625855212877]
   new bounds: x_min=-29.523602365321494, x_max=56.0388814870206, y_min=506.6296219300442, y_max=567.8555062577864
📍 FINAL BBOX (after rotation):
   x_min: -29.523602365321494, y_min: 506.6296219300442
   x_max: 56.0388814870206, y_max: 567.8555062577864
   width: 85.5624838523421, height: 61.225884327742165
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: -29.523602365321494, y_min: 506.6296219300442
   x_max: 56.0388814870206, y_max: 567.8555062577864
   width: 85.5624838523421, height: 61.225884327742165
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=-29.523602365321494, x_max=56.0388814870206
   After: x_min=743.9611185129794, x_max=829.5236023653215
📍 FINAL BBOX (after flip):
   x_min: 743.9611185129794, y_min: 506.6296219300442
   x_max: 829.5236023653215, y_max: 567.8555062577864
   width: 85.5624838523421, height: 61.225884327742165
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 743.9611185129794, y_min: 506.6296219300442
   x_max: 829.5236023653215, y_max: 567.8555062577864
   width: 85.5624838523421, height: 61.225884327742165
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 743.9611185129794, x_max: 829.5236023653215
   y_min: 506.6296219300442, y_max: 567.8555062577864
📍 AFTER SCALING:
   x_min: 952.2702316966137, x_max: 1061.7902110276116
   y_min: 863.8035053907254, y_max: 968.1936381695258
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=952.2702316966137, y_min=863.8035053907254, x_max=1061.7902110276116, y_max=968.1936381695258
   🔄 Processing annotation 2/6: cat
   🔄 Processing annotation 3/6: cat eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 5.639999999999997, y_min: 46.14866666666667
   x_max: 8.279999999999996, y_max: 53.726444444444446
   width: 2.639999999999999, height: 7.577777777777776
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-394.36, -253.85133333333334), (-391.72, -253.85133333333334), (-394.36, -246.27355555555556), (-391.72, -246.27355555555556)]
   corner 0: (-394.36, -253.85133333333334) → (-4.806143917851045, 536.8381195700372)
   corner 1: (-391.72, -253.85133333333334) → (-3.611716285267903, 534.4837740918795)
   corner 2: (-394.36, -246.27355555555556) → (1.9516995842685105, 540.2665692561552)
   corner 3: (-391.72, -246.27355555555556) → (3.146127216851596, 537.9122237779975)
   all x coords: [-4.806143917851045, -3.611716285267903, 1.9516995842685105, 3.146127216851596]
   all y coords: [536.8381195700372, 534.4837740918795, 540.2665692561552, 537.9122237779975]
   new bounds: x_min=-4.806143917851045, x_max=3.146127216851596, y_min=534.4837740918795, y_max=540.2665692561552
📍 FINAL BBOX (after rotation):
   x_min: -4.806143917851045, y_min: 534.4837740918795
   x_max: 3.146127216851596, y_max: 540.2665692561552
   width: 7.952271134702642, height: 5.78279516427574
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: -4.806143917851045, y_min: 534.4837740918795
   x_max: 3.146127216851596, y_max: 540.2665692561552
   width: 7.952271134702642, height: 5.78279516427574
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=-4.806143917851045, x_max=3.146127216851596
   After: x_min=796.8538727831484, x_max=804.806143917851
📍 FINAL BBOX (after flip):
   x_min: 796.8538727831484, y_min: 534.4837740918795
   x_max: 804.806143917851, y_max: 540.2665692561552
   width: 7.952271134702642, height: 5.78279516427574
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 796.8538727831484, y_min: 534.4837740918795
   x_max: 804.806143917851, y_max: 540.2665692561552
   width: 7.952271134702642, height: 5.78279516427574
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 796.8538727831484, x_max: 804.806143917851
   y_min: 534.4837740918795, y_max: 540.2665692561552
📍 AFTER SCALING:
   x_min: 1019.97295716243, x_max: 1030.1518642148494
   y_min: 911.2948348266546, y_max: 921.1545005817446
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=1019.97295716243, y_min=911.2948348266546, x_max=1030.1518642148494, y_max=921.1545005817446
   🔄 Processing annotation 4/6: cat eye
   🔄 Processing annotation 5/6: cat eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 11.016, y_min: 45.69400000000001
   x_max: 13.607999999999997, y_max: 53.27177777777777
   width: 2.591999999999997, height: 7.5777777777777615
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-388.984, -254.30599999999998), (-386.392, -254.30599999999998), (-388.984, -246.72822222222223), (-386.392, -246.72822222222223)]
   corner 0: (-388.984, -254.30599999999998) → (-2.7793255307179834, 531.8381090697123)
   corner 1: (-386.392, -254.30599999999998) → (-1.6066147641818702, 529.5265698729756)
   corner 2: (-388.984, -246.72822222222223) → (3.9785179714015158, 535.2665587558306)
   corner 3: (-386.392, -246.72822222222223) → (5.151228737937629, 532.9550195590939)
   all x coords: [-2.7793255307179834, -1.6066147641818702, 3.9785179714015158, 5.151228737937629]       
   all y coords: [531.8381090697123, 529.5265698729756, 535.2665587558306, 532.9550195590939]
   new bounds: x_min=-2.7793255307179834, x_max=5.151228737937629, y_min=529.5265698729756, y_max=535.2665587558306
📍 FINAL BBOX (after rotation):
   x_min: -2.7793255307179834, y_min: 529.5265698729756
   x_max: 5.151228737937629, y_max: 535.2665587558306
   width: 7.930554268655612, height: 5.739988882854959
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: -2.7793255307179834, y_min: 529.5265698729756
   x_max: 5.151228737937629, y_max: 535.2665587558306
   width: 7.930554268655612, height: 5.739988882854959
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=-2.7793255307179834, x_max=5.151228737937629
   After: x_min=794.8487712620624, x_max=802.779325530718
📍 FINAL BBOX (after flip):
   x_min: 794.8487712620624, y_min: 529.5265698729756
   x_max: 802.779325530718, y_max: 535.2665587558306
   width: 7.9305542686555555, height: 5.739988882854959
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 794.8487712620624, y_min: 529.5265698729756
   x_max: 802.779325530718, y_max: 535.2665587558306
   width: 7.9305542686555555, height: 5.739988882854959
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 794.8487712620624, x_max: 802.779325530718
   y_min: 529.5265698729756, y_max: 535.2665587558306
📍 AFTER SCALING:
   x_min: 1017.40642721544, x_max: 1027.5575366793191
   y_min: 902.8428016334235, y_max: 912.6294826786913
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=1017.40642721544, y_min=902.8428016334235, x_max=1027.5575366793191, y_max=912.6294826786913
   🔄 Processing annotation 6/6: cat eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 6
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 6
Transformed annotations: 6
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'flip', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 6 annotations
   First transformed annotation: (0.0, 21.29355555555556, 26.903999999999996, 103.58822222222223)        

=== DEBUG YOLO DUMP :: cat_rotate-63_flip_horizontal.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,21.29,26.90,103.59]
  ann[1] POLY -> 77 pts; min=(962.7,880.5) max=(1024.0,966.6)
  ann[2] BBOX -> [5.64,46.15,8.28,53.73]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 6
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 6
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 3
  det: 12 0.013137 0.061037 0.026273 0.080444
  det: 16 0.006797 0.048815 0.002578 0.007407
  det: 16 0.012023 0.048370 0.002531 0.007407
YOLO SEG lines: 3
  seg: 12 0.948377 0.944254 0.952263 0.941626 0.960541 0.936026 0.963413 0.934083 0.964089 0.933626 0.974901 0.926312 0.985151 ...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

=== 🔍 TRANSFORMATIONS DEBUG :: car.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}}, {'type': 'rotate', 'params': {'angle': 63.1}}, {'type': 'flip', 'params': {'horizontal': True}}]
transformations type: <class 'list'>
transformations bool: True
🎯 COMPLEX TRANSFORMATIONS for car.jpg
🖼️ Original image dims: (800, 600)
🎯 ORIGINAL IMAGE: Applying ONLY resize (baseline behavior)
🖼️ Resized to: (1024, 1023) using mode: stretch_to

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 0}]     
🎯 ORIGINAL IMAGE BASELINE: Applied resize-only, augmented images will get full combinations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: segmentation
   Export format: yolo_segmentation
   ✅ Using SEGMENTATION mode: yolo_segmentation
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 1024x1023

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 2 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 2 annotations individually
   🔄 Processing annotation 1/2: dog
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog
         📦 Input bbox: x_min=0.0, y_min=18.53333333333333, x_max=14.793749999999996, y_max=62.088888888888896
         📐 Dimensions: (800, 600) → (1024, 1023)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 49 points...
         🔧 _transform_polygon returned: Polygon(points=[(0.0, 105.86155555555557), (0.0, 101.01177777777778), (0.0, 95.25266666666666), (0.0, 84.94688888888889), (0.0, 77.066), (0.0, 71.15533333333333), (0.311999999999996, 67.36644444444445), (0.2639999999999965, 63.57755555555556), (1.2719999999999958, 60.54644444444445), (2.519999999999996, 57.363777777777784), (3.5759999999999965, 53.42333333333334), (4.391999999999996, 50.39222222222223), (4.871999999999997, 49.028222222222226), (5.399999999999998, 47.66422222222222), (6.023999999999996, 41.2988888888889), (6.839999999999998, 36.75222222222222), (7.271999999999996, 35.23666666666667), (8.327999999999998, 34.782), (10.199999999999996, 39.78333333333334), (11.495999999999997, 46.75488888888889), (12.167999999999997, 46.60333333333333), (12.695999999999994, 45.08777777777778), (13.079999999999998, 42.208222222222226), (13.32, 39.93488888888889), (13.895999999999999, 36.29755555555556), (15.143999999999997, 31.90244444444445), (16.631999999999998, 31.59933333333333), (16.583999999999996, 36.60066666666667), (16.535999999999998, 43.875333333333344), (16.151999999999997, 48.72511111111112), (16.392, 50.8468888888889), (17.544, 53.87800000000001), (18.311999999999998, 59.0308888888889), (18.263999999999996, 63.42600000000001), (18.791999999999998, 67.21488888888891), (18.935999999999996, 74.48955555555555), (17.831999999999997, 76.7628888888889), (15.911999999999999, 77.066), (14.567999999999998, 77.066), (13.703999999999997, 77.52066666666667), (11.879999999999995, 80.24866666666667), (12.407999999999996, 84.6437777777778), (12.647999999999998, 86.91711111111113), (12.791999999999998, 89.79666666666668), (12.791999999999998, 92.52466666666668), (13.367999999999997, 97.67755555555556), (13.607999999999997, 100.55711111111114), (13.703999999999997, 103.58822222222223), (13.511999999999999, 105.71000000000002)], class_name='dog', class_id=1, confidence=1.0)
         📦 Updated bounding box: x_min=0.0, y_min=31.59933333333333, x_max=18.935999999999996, y_max=105.86155555555557
         📦 Updated annotation with 49 transformed points
   🔄 Processing annotation 2/2: dog eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog eye
         📦 Input bbox: x_min=9.543749999999998, y_min=34.53333333333334, x_max=11.343749999999996, y_max=37.733333333333334
         📐 Dimensions: (800, 600) → (1024, 1023)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 7 points...
         🔧 _transform_polygon returned: Polygon(points=[(12.215999999999998, 62.062), (12.311999999999996, 60.698000000000015), (13.271999999999998, 58.87933333333334), (14.471999999999998, 59.78866666666667), (14.519999999999996, 61.758888888888904), (14.039999999999997, 64.33533333333334), (12.887999999999998, 64.33533333333334)], class_name='dog eye', class_id=15, confidence=1.0)
         📦 Updated bounding box: x_min=12.215999999999998, y_min=58.87933333333334, x_max=14.519999999999996, y_max=64.33533333333334
         📦 Updated annotation with 7 transformed points
   Original: 2 → Transformed: 2
✅ NEW SEGMENTATION FUNCTION RESULT: 2 lines

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 63.1}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 2 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 31.59933333333333, 18.935999999999996, 105.86155555555557)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 4

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 4
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 4 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 4 annotations individually
   🔄 Processing annotation 1/4: dog

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   width: 18.935999999999996, height: 74.26222222222223
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-400.0, -268.40066666666667), (-381.064, -268.40066666666667), (-400.0, -194.13844444444442), (-381.064, -194.13844444444442)]
   corner 0: (-400.0, -268.40066666666667) → (458.3851677530128, -178.15278944450768)
   corner 1: (-381.064, -268.40066666666667) → (466.95247140854076, -161.26571142390333)
   corner 2: (-400.0, -194.13844444444442) → (392.15830143224156, -144.55398252054954)
   corner 3: (-381.064, -194.13844444444442) → (400.7256050877695, -127.66690449994519)
   all x coords: [458.3851677530128, 466.95247140854076, 392.15830143224156, 400.7256050877695]
   all y coords: [-178.15278944450768, -161.26571142390333, -144.55398252054954, -127.66690449994519]    
   new bounds: x_min=392.15830143224156, x_max=466.95247140854076, y_min=-178.15278944450768, y_max=-127.66690449994519
📍 FINAL BBOX (after rotation):
   x_min: 392.15830143224156, y_min: -178.15278944450768
   x_max: 466.95247140854076, y_max: -127.66690449994519
   width: 74.7941699762992, height: 50.485884944562486
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 392.15830143224156, y_min: -178.15278944450768
   x_max: 466.95247140854076, y_max: -127.66690449994519
   width: 74.7941699762992, height: 50.485884944562486
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 392.15830143224156, x_max: 466.95247140854076
   y_min: -178.15278944450768, y_max: -127.66690449994519
📍 AFTER SCALING:
   x_min: 501.9626258332692, x_max: 597.6991634029322
   y_min: -303.7505060028856, y_max: -217.67207217240656
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=501.9626258332692, y_min=-303.7505060028856, x_max=597.6991634029322, y_max=-217.67207217240656
   🔄 Processing annotation 2/4: dog
   🔄 Processing annotation 3/4: dog eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   width: 2.3039999999999985, height: 5.455999999999996
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-387.784, -241.12066666666666), (-385.48, -241.12066666666666), (-387.784, -235.66466666666668), (-385.48, -235.66466666666668)]
   corner 0: (-387.784, -241.12066666666666) → (439.5838735543353, -154.91617195282493)
   corner 1: (-385.48, -241.12066666666666) → (440.62628312458963, -152.8614704446145)
   corner 2: (-387.784, -235.66466666666668) → (434.71822623280923, -152.44768817881982)
   corner 3: (-385.48, -235.66466666666668) → (435.76063580306356, -150.39298667060945)
   all x coords: [439.5838735543353, 440.62628312458963, 434.71822623280923, 435.76063580306356]
   all y coords: [-154.91617195282493, -152.8614704446145, -152.44768817881982, -150.39298667060945]     
   new bounds: x_min=434.71822623280923, x_max=440.62628312458963, y_min=-154.91617195282493, y_max=-150.39298667060945
📍 FINAL BBOX (after rotation):
   x_min: 434.71822623280923, y_min: -154.91617195282493
   x_max: 440.62628312458963, y_max: -150.39298667060945
   width: 5.908056891780404, height: 4.523185282215479
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 434.71822623280923, y_min: -154.91617195282493
   x_max: 440.62628312458963, y_max: -150.39298667060945
   width: 5.908056891780404, height: 4.523185282215479
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 434.71822623280923, x_max: 440.62628312458963
   y_min: -154.91617195282493, y_max: -150.39298667060945
📍 AFTER SCALING:
   x_min: 556.4393295779959, x_max: 564.0016423994747
   y_min: -264.13207317956653, y_max: -256.42004227338913
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=556.4393295779959, y_min=-264.13207317956653, x_max=564.0016423994747, y_max=-256.42004227338913
   🔄 Processing annotation 4/4: dog eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 4
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 4
Transformed annotations: 4
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 4 annotations
   First transformed annotation: (0.0, 31.59933333333333, 18.935999999999996, 105.86155555555557)        

=== DEBUG YOLO DUMP :: car_rotate63.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,31.60,18.94,105.86]
  ann[1] POLY -> 49 pts; min=(502.0,0.0) max=(596.4,0.0)
  ann[2] BBOX -> [12.22,58.88,14.52,64.34]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 4
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 4
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 2
  det: 1 0.009246 0.067185 0.018492 0.072593
  det: 15 0.013055 0.060222 0.002250 0.005333
YOLO SEG lines: 2
  seg: 1 0.490198 0.000000 0.495604 0.000000 0.502024 0.000000 0.513512 0.000000 0.522298 0.000000 0.528887 0.000000 0.533287 0...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['flip', 'resize'], 'geometric_transforms_order': ['flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 2 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 31.59933333333333, 18.935999999999996, 105.86155555555557)

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
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 4

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 4
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 4 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 4 annotations individually
   🔄 Processing annotation 1/4: dog

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
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
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   width: 18.935999999999996, height: 74.26222222222223
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=0.0, x_max=18.935999999999996
   After: x_min=781.064, x_max=800.0
📍 FINAL BBOX (after flip):
   x_min: 781.064, y_min: 31.59933333333333
   x_max: 800.0, y_max: 105.86155555555557
   width: 18.936000000000035, height: 74.26222222222223
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 781.064, y_min: 31.59933333333333
   x_max: 800.0, y_max: 105.86155555555557
   width: 18.936000000000035, height: 74.26222222222223
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 781.064, x_max: 800.0
   y_min: 31.59933333333333, y_max: 105.86155555555557
📍 AFTER SCALING:
   x_min: 999.76192, x_max: 1024.0
   y_min: 53.87686333333333, y_max: 180.49395222222225
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=999.76192, y_min=53.87686333333333, x_max=1024.0, y_max=180.49395222222225     
   🔄 Processing annotation 2/4: dog
   🔄 Processing annotation 3/4: dog eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
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
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   width: 2.3039999999999985, height: 5.455999999999996
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=12.215999999999998, x_max=14.519999999999996
   After: x_min=785.48, x_max=787.784
📍 FINAL BBOX (after flip):
   x_min: 785.48, y_min: 58.87933333333334
   x_max: 787.784, y_max: 64.33533333333334
   width: 2.3039999999999736, height: 5.455999999999996
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 785.48, y_min: 58.87933333333334
   x_max: 787.784, y_max: 64.33533333333334
   width: 2.3039999999999736, height: 5.455999999999996
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 785.48, x_max: 787.784
   y_min: 58.87933333333334, y_max: 64.33533333333334
📍 AFTER SCALING:
   x_min: 1005.4144, x_max: 1008.36352
   y_min: 100.38926333333335, y_max: 109.69174333333335
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=1005.4144, y_min=100.38926333333335, x_max=1008.36352, y_max=109.69174333333335
   🔄 Processing annotation 4/4: dog eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 4
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 4
Transformed annotations: 4
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['flip', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 4 annotations
   First transformed annotation: (0.0, 31.59933333333333, 18.935999999999996, 105.86155555555557)        

=== DEBUG YOLO DUMP :: car_flip_horizontal.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,31.60,18.94,105.86]
  ann[1] POLY -> 49 pts; min=(999.8,53.9) max=(1024.0,180.5)
  ann[2] BBOX -> [12.22,58.88,14.52,64.34]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 4
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 4
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 2
  det: 1 0.009246 0.067185 0.018492 0.072593
  det: 15 0.013055 0.060222 0.002250 0.005333
YOLO SEG lines: 2
  seg: 1 1.000000 0.176436 1.000000 0.168353 1.000000 0.158754 1.000000 0.141578 1.000000 0.128443 1.000000 0.118592 0.999610 0...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -63.1}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 2 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 31.59933333333333, 18.935999999999996, 105.86155555555557)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 4

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 4
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 4 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 4 annotations individually
   🔄 Processing annotation 1/4: dog

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   width: 18.935999999999996, height: 74.26222222222223
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-400.0, -268.40066666666667), (-381.064, -268.40066666666667), (-400.0, -194.13844444444442), (-381.064, -194.13844444444442)]
   corner 0: (-400.0, -268.40066666666667) → (-20.332935202438932, 535.2852342396636)
   corner 1: (-381.064, -268.40066666666667) → (-11.765631546910981, 518.3981562190593)
   corner 2: (-400.0, -194.13844444444442) → (45.89393111833232, 568.8840411636218)
   corner 3: (-381.064, -194.13844444444442) → (54.46123477386027, 551.9969631430174)
   all x coords: [-20.332935202438932, -11.765631546910981, 45.89393111833232, 54.46123477386027]        
   all y coords: [535.2852342396636, 518.3981562190593, 568.8840411636218, 551.9969631430174]
   new bounds: x_min=-20.332935202438932, x_max=54.46123477386027, y_min=518.3981562190593, y_max=568.8840411636218
📍 FINAL BBOX (after rotation):
   x_min: -20.332935202438932, y_min: 518.3981562190593
   x_max: 54.46123477386027, y_max: 568.8840411636218
   width: 74.7941699762992, height: 50.485884944562486
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: -20.332935202438932, y_min: 518.3981562190593
   x_max: 54.46123477386027, y_max: 568.8840411636218
   width: 74.7941699762992, height: 50.485884944562486
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: -20.332935202438932, x_max: 54.46123477386027
   y_min: 518.3981562190593, y_max: 568.8840411636218
📍 AFTER SCALING:
   x_min: -26.026157059121832, x_max: 69.71038051054114
   y_min: 883.8688563534961, y_max: 969.9472901839752
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=-26.026157059121832, y_min=883.8688563534961, x_max=69.71038051054114, y_max=969.9472901839752
   🔄 Processing annotation 2/4: dog
   🔄 Processing annotation 3/4: dog eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   width: 2.3039999999999985, height: 5.455999999999996
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-387.784, -241.12066666666666), (-385.48, -241.12066666666666), (-387.784, -235.66466666666668), (-385.48, -235.66466666666668)]
   corner 0: (-387.784, -241.12066666666666) → (9.522243814144076, 536.7334544880317)
   corner 1: (-385.48, -241.12066666666666) → (10.564653384398412, 534.6787529798214)
   corner 2: (-387.784, -235.66466666666668) → (14.387891135670088, 539.2019382620368)
   corner 3: (-385.48, -235.66466666666668) → (15.430300705924424, 537.1472367538265)
   all x coords: [9.522243814144076, 10.564653384398412, 14.387891135670088, 15.430300705924424]
   all y coords: [536.7334544880317, 534.6787529798214, 539.2019382620368, 537.1472367538265]
   new bounds: x_min=9.522243814144076, x_max=15.430300705924424, y_min=534.6787529798214, y_max=539.2019382620368
📍 FINAL BBOX (after rotation):
   x_min: 9.522243814144076, y_min: 534.6787529798214
   x_max: 15.430300705924424, y_max: 539.2019382620368
   width: 5.9080568917803475, height: 4.523185282215422
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 9.522243814144076, y_min: 534.6787529798214
   x_max: 15.430300705924424, y_max: 539.2019382620368
   width: 5.9080568917803475, height: 4.523185282215422
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 9.522243814144076, x_max: 15.430300705924424
   y_min: 534.6787529798214, y_max: 539.2019382620368
📍 AFTER SCALING:
   x_min: 12.188472082104418, x_max: 19.750784903583263
   y_min: 911.6272738305955, y_max: 919.3393047367729
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=12.188472082104418, y_min=911.6272738305955, x_max=19.750784903583263, y_max=919.3393047367729
   🔄 Processing annotation 4/4: dog eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 4
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 4
Transformed annotations: 4
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 4 annotations
   First transformed annotation: (0.0, 31.59933333333333, 18.935999999999996, 105.86155555555557)        

=== DEBUG YOLO DUMP :: car_rotate-63.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,31.60,18.94,105.86]
  ann[1] POLY -> 49 pts; min=(0.0,887.4) max=(66.4,969.9)
  ann[2] BBOX -> [12.22,58.88,14.52,64.34]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 4
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 4
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 2
  det: 1 0.009246 0.067185 0.018492 0.072593
  det: 15 0.013055 0.060222 0.002250 0.005333
YOLO SEG lines: 2
  seg: 1 0.057367 0.948140 0.051961 0.944483 0.045541 0.940140 0.034053 0.932369 0.025268 0.926427 0.018679 0.921970 0.014632 0...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['rotate', 'flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -63.1}}, {'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 2, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'flip', 'resize'], 'geometric_transforms_order': ['rotate', 'flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}], 'photometric_transforms': [], 'total_transforms': 3, 'geometric_count': 3, 'photometric_count': 0}
🔍 DEBUG: About to transform 2 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 31.59933333333333, 18.935999999999996, 105.86155555555557)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 4

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 4
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 4 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 4 annotations individually
   🔄 Processing annotation 1/4: dog

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   width: 18.935999999999996, height: 74.26222222222223
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-400.0, -268.40066666666667), (-381.064, -268.40066666666667), (-400.0, -194.13844444444442), (-381.064, -194.13844444444442)]
   corner 0: (-400.0, -268.40066666666667) → (-20.332935202438932, 535.2852342396636)
   corner 1: (-381.064, -268.40066666666667) → (-11.765631546910981, 518.3981562190593)
   corner 2: (-400.0, -194.13844444444442) → (45.89393111833232, 568.8840411636218)
   corner 3: (-381.064, -194.13844444444442) → (54.46123477386027, 551.9969631430174)
   all x coords: [-20.332935202438932, -11.765631546910981, 45.89393111833232, 54.46123477386027]        
   all y coords: [535.2852342396636, 518.3981562190593, 568.8840411636218, 551.9969631430174]
   new bounds: x_min=-20.332935202438932, x_max=54.46123477386027, y_min=518.3981562190593, y_max=568.8840411636218
📍 FINAL BBOX (after rotation):
   x_min: -20.332935202438932, y_min: 518.3981562190593
   x_max: 54.46123477386027, y_max: 568.8840411636218
   width: 74.7941699762992, height: 50.485884944562486
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: -20.332935202438932, y_min: 518.3981562190593
   x_max: 54.46123477386027, y_max: 568.8840411636218
   width: 74.7941699762992, height: 50.485884944562486
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=-20.332935202438932, x_max=54.46123477386027
   After: x_min=745.5387652261397, x_max=820.3329352024389
📍 FINAL BBOX (after flip):
   x_min: 745.5387652261397, y_min: 518.3981562190593
   x_max: 820.3329352024389, y_max: 568.8840411636218
   width: 74.79416997629914, height: 50.485884944562486
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 745.5387652261397, y_min: 518.3981562190593
   x_max: 820.3329352024389, y_max: 568.8840411636218
   width: 74.79416997629914, height: 50.485884944562486
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 745.5387652261397, x_max: 820.3329352024389
   y_min: 518.3981562190593, y_max: 568.8840411636218
📍 AFTER SCALING:
   x_min: 954.2896194894589, x_max: 1050.0261570591217
   y_min: 883.8688563534961, y_max: 969.9472901839752
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=954.2896194894589, y_min=883.8688563534961, x_max=1050.0261570591217, y_max=969.9472901839752
   🔄 Processing annotation 2/4: dog
   🔄 Processing annotation 3/4: dog eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   width: 2.3039999999999985, height: 5.455999999999996
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-387.784, -241.12066666666666), (-385.48, -241.12066666666666), (-387.784, -235.66466666666668), (-385.48, -235.66466666666668)]
   corner 0: (-387.784, -241.12066666666666) → (9.522243814144076, 536.7334544880317)
   corner 1: (-385.48, -241.12066666666666) → (10.564653384398412, 534.6787529798214)
   corner 2: (-387.784, -235.66466666666668) → (14.387891135670088, 539.2019382620368)
   corner 3: (-385.48, -235.66466666666668) → (15.430300705924424, 537.1472367538265)
   all x coords: [9.522243814144076, 10.564653384398412, 14.387891135670088, 15.430300705924424]
   all y coords: [536.7334544880317, 534.6787529798214, 539.2019382620368, 537.1472367538265]
   new bounds: x_min=9.522243814144076, x_max=15.430300705924424, y_min=534.6787529798214, y_max=539.2019382620368
📍 FINAL BBOX (after rotation):
   x_min: 9.522243814144076, y_min: 534.6787529798214
   x_max: 15.430300705924424, y_max: 539.2019382620368
   width: 5.9080568917803475, height: 4.523185282215422
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 9.522243814144076, y_min: 534.6787529798214
   x_max: 15.430300705924424, y_max: 539.2019382620368
   width: 5.9080568917803475, height: 4.523185282215422
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=9.522243814144076, x_max=15.430300705924424
   After: x_min=784.5696992940756, x_max=790.4777561858559
📍 FINAL BBOX (after flip):
   x_min: 784.5696992940756, y_min: 534.6787529798214
   x_max: 790.4777561858559, y_max: 539.2019382620368
   width: 5.9080568917803475, height: 4.523185282215422
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 784.5696992940756, y_min: 534.6787529798214
   x_max: 790.4777561858559, y_max: 539.2019382620368
   width: 5.9080568917803475, height: 4.523185282215422
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 784.5696992940756, x_max: 790.4777561858559
   y_min: 534.6787529798214, y_max: 539.2019382620368
📍 AFTER SCALING:
   x_min: 1004.2492150964167, x_max: 1011.8115279178957
   y_min: 911.6272738305955, y_max: 919.3393047367729
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=1004.2492150964167, y_min=911.6272738305955, x_max=1011.8115279178957, y_max=919.3393047367729
   🔄 Processing annotation 4/4: dog eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 4
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 4
Transformed annotations: 4
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'flip', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 4 annotations
   First transformed annotation: (0.0, 31.59933333333333, 18.935999999999996, 105.86155555555557)        

=== DEBUG YOLO DUMP :: car_rotate-63_flip_horizontal.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,31.60,18.94,105.86]
  ann[1] POLY -> 49 pts; min=(957.6,887.4) max=(1024.0,969.9)
  ann[2] BBOX -> [12.22,58.88,14.52,64.34]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 4
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 4
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 2
  det: 1 0.009246 0.067185 0.018492 0.072593
  det: 15 0.013055 0.060222 0.002250 0.005333
YOLO SEG lines: 2
  seg: 1 0.942633 0.948140 0.948039 0.944483 0.954459 0.940140 0.965947 0.932369 0.974732 0.926427 0.981321 0.921970 0.985368 0...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['rotate', 'flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 63.1}}, {'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 2, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'flip', 'resize'], 'geometric_transforms_order': ['rotate', 'flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}], 'photometric_transforms': [], 'total_transforms': 3, 'geometric_count': 3, 'photometric_count': 0}
🔍 DEBUG: About to transform 2 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 31.59933333333333, 18.935999999999996, 105.86155555555557)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 4

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 4
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 4 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 4 annotations individually
   🔄 Processing annotation 1/4: dog

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 31.59933333333333
   x_max: 18.935999999999996, y_max: 105.86155555555557
   width: 18.935999999999996, height: 74.26222222222223
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-400.0, -268.40066666666667), (-381.064, -268.40066666666667), (-400.0, -194.13844444444442), (-381.064, -194.13844444444442)]
   corner 0: (-400.0, -268.40066666666667) → (458.3851677530128, -178.15278944450768)
   corner 1: (-381.064, -268.40066666666667) → (466.95247140854076, -161.26571142390333)
   corner 2: (-400.0, -194.13844444444442) → (392.15830143224156, -144.55398252054954)
   corner 3: (-381.064, -194.13844444444442) → (400.7256050877695, -127.66690449994519)
   all x coords: [458.3851677530128, 466.95247140854076, 392.15830143224156, 400.7256050877695]
   all y coords: [-178.15278944450768, -161.26571142390333, -144.55398252054954, -127.66690449994519]    
   new bounds: x_min=392.15830143224156, x_max=466.95247140854076, y_min=-178.15278944450768, y_max=-127.66690449994519
📍 FINAL BBOX (after rotation):
   x_min: 392.15830143224156, y_min: -178.15278944450768
   x_max: 466.95247140854076, y_max: -127.66690449994519
   width: 74.7941699762992, height: 50.485884944562486
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 392.15830143224156, y_min: -178.15278944450768
   x_max: 466.95247140854076, y_max: -127.66690449994519
   width: 74.7941699762992, height: 50.485884944562486
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=392.15830143224156, x_max=466.95247140854076
   After: x_min=333.04752859145924, x_max=407.84169856775844
📍 FINAL BBOX (after flip):
   x_min: 333.04752859145924, y_min: -178.15278944450768
   x_max: 407.84169856775844, y_max: -127.66690449994519
   width: 74.7941699762992, height: 50.485884944562486
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 333.04752859145924, y_min: -178.15278944450768
   x_max: 407.84169856775844, y_max: -127.66690449994519
   width: 74.7941699762992, height: 50.485884944562486
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 333.04752859145924, x_max: 407.84169856775844
   y_min: -178.15278944450768, y_max: -127.66690449994519
📍 AFTER SCALING:
   x_min: 426.3008365970678, x_max: 522.0373741667308
   y_min: -303.7505060028856, y_max: -217.67207217240656
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=426.3008365970678, y_min=-303.7505060028856, x_max=522.0373741667308, y_max=-217.67207217240656
   🔄 Processing annotation 2/4: dog
   🔄 Processing annotation 3/4: dog eye

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 12.215999999999998, y_min: 58.87933333333334
   x_max: 14.519999999999996, y_max: 64.33533333333334
   width: 2.3039999999999985, height: 5.455999999999996
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-387.784, -241.12066666666666), (-385.48, -241.12066666666666), (-387.784, -235.66466666666668), (-385.48, -235.66466666666668)]
   corner 0: (-387.784, -241.12066666666666) → (439.5838735543353, -154.91617195282493)
   corner 1: (-385.48, -241.12066666666666) → (440.62628312458963, -152.8614704446145)
   corner 2: (-387.784, -235.66466666666668) → (434.71822623280923, -152.44768817881982)
   corner 3: (-385.48, -235.66466666666668) → (435.76063580306356, -150.39298667060945)
   all x coords: [439.5838735543353, 440.62628312458963, 434.71822623280923, 435.76063580306356]
   all y coords: [-154.91617195282493, -152.8614704446145, -152.44768817881982, -150.39298667060945]     
   new bounds: x_min=434.71822623280923, x_max=440.62628312458963, y_min=-154.91617195282493, y_max=-150.39298667060945
📍 FINAL BBOX (after rotation):
   x_min: 434.71822623280923, y_min: -154.91617195282493
   x_max: 440.62628312458963, y_max: -150.39298667060945
   width: 5.908056891780404, height: 4.523185282215479
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 434.71822623280923, y_min: -154.91617195282493
   x_max: 440.62628312458963, y_max: -150.39298667060945
   width: 5.908056891780404, height: 4.523185282215479
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=434.71822623280923, x_max=440.62628312458963
   After: x_min=359.37371687541037, x_max=365.28177376719077
📍 FINAL BBOX (after flip):
   x_min: 359.37371687541037, y_min: -154.91617195282493
   x_max: 365.28177376719077, y_max: -150.39298667060945
   width: 5.908056891780404, height: 4.523185282215479
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 359.37371687541037, y_min: -154.91617195282493
   x_max: 365.28177376719077, y_max: -150.39298667060945
   width: 5.908056891780404, height: 4.523185282215479
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 359.37371687541037, x_max: 365.28177376719077
   y_min: -154.91617195282493, y_max: -150.39298667060945
📍 AFTER SCALING:
   x_min: 459.99835760052525, x_max: 467.5606704220042
   y_min: -264.13207317956653, y_max: -256.42004227338913
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=459.99835760052525, y_min=-264.13207317956653, x_max=467.5606704220042, y_max=-256.42004227338913
   🔄 Processing annotation 4/4: dog eye
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 4
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 4
Transformed annotations: 4
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'flip', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 4 annotations
   First transformed annotation: (0.0, 31.59933333333333, 18.935999999999996, 105.86155555555557)        

=== DEBUG YOLO DUMP :: car_rotate63_flip_horizontal.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,31.60,18.94,105.86]
  ann[1] POLY -> 49 pts; min=(427.6,0.0) max=(522.0,0.0)
  ann[2] BBOX -> [12.22,58.88,14.52,64.34]
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 4
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 4
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 2
  det: 1 0.009246 0.067185 0.018492 0.072593
  det: 15 0.013055 0.060222 0.002250 0.005333
YOLO SEG lines: 2
  seg: 1 0.509802 0.000000 0.504396 0.000000 0.497976 0.000000 0.486488 0.000000 0.477702 0.000000 0.471113 0.000000 0.466713 0...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

=== 🔍 TRANSFORMATIONS DEBUG :: dog.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}}, {'type': 'rotate', 'params': {'angle': 63.1}}, {'type': 'flip', 'params': {'horizontal': True}}]
transformations type: <class 'list'>
transformations bool: True
🎯 COMPLEX TRANSFORMATIONS for dog.jpg
🖼️ Original image dims: (800, 600)
🎯 ORIGINAL IMAGE: Applying ONLY resize (baseline behavior)
🖼️ Resized to: (1024, 1023) using mode: stretch_to

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 0}]     
🎯 ORIGINAL IMAGE BASELINE: Applied resize-only, augmented images will get full combinations!
🔍 LABEL MODE DETECTION:
   Config exists: True
   Task type: segmentation
   Export format: yolo_segmentation
   ✅ Using SEGMENTATION mode: yolo_segmentation
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 1
   Final dims: 1024x1023
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 1024x1023

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 1 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 1 annotations individually
   🔄 Processing annotation 1/1: dog
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog
         📦 Input bbox: x_min=0.0, y_min=12.222222222222221, x_max=18.91875, y_max=62.00000000000001     
         📐 Dimensions: (800, 600) → (1024, 1023)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 54 points...
         🔧 _transform_polygon returned: Polygon(points=[(0.0, 50.998444444444445), (0.0, 46.60333333333333), (0.215999999999997, 41.45044444444445), (1.3679999999999966, 37.96466666666667), (2.231999999999997, 35.38822222222223), (2.279999999999997, 31.144666666666673), (3.4319999999999964, 25.68866666666667), (4.583999999999998, 23.41533333333333), (6.023999999999996, 21.748222222222225), (8.471999999999998, 20.83888888888889), (9.767999999999997, 21.596666666666668), (13.127999999999998, 20.990444444444446), (14.424, 23.56688888888889), (15.959999999999996, 27.204222222222228), (17.352, 31.447777777777784), (18.599999999999998, 34.782), (19.176, 37.96466666666667), (19.415999999999997, 42.966), (19.895999999999994, 46.30022222222222), (20.855999999999998, 49.93755555555555), (21.192000000000004, 55.24200000000001), (20.999999999999996, 58.87933333333334), (19.991999999999997, 64.33533333333334), (19.367999999999995, 67.36644444444445), (19.752, 71.76155555555556), (20.471999999999998, 74.64111111111113), (21.383999999999997, 78.58155555555557), (21.671999999999997, 80.40022222222224), (22.343999999999998, 77.82377777777778), (23.112, 72.82244444444446), (23.543999999999997, 72.21622222222223), (24.023999999999997, 74.18644444444446), (24.216, 77.36911111111112), (24.168, 80.40022222222224), (23.447999999999997, 84.18911111111112), (22.535999999999998, 86.46244444444444), (22.631999999999994, 91.46377777777778), (22.488000000000003, 95.10111111111112), (22.631999999999994, 99.19311111111111), (22.535999999999998, 103.73977777777779), (22.392, 105.71000000000002), (4.727999999999997, 105.71000000000002), (4.9199999999999955, 101.9211111111111), (4.2479999999999976, 99.79933333333337), (3.767999999999996, 94.64644444444447), (3.671999999999997, 90.09977777777779), (3.2399999999999967, 85.40155555555556), (2.375999999999996, 79.94555555555557), (1.7039999999999964, 72.82244444444446), (1.7519999999999956, 67.36644444444445), (1.8959999999999957, 65.24466666666667), (1.5119999999999965, 62.062), (1.2239999999999964, 58.57622222222222), (0.40799999999999664, 54.63577777777778)], class_name='dog', class_id=1, confidence=1.0)
         📦 Updated bounding box: x_min=0.0, y_min=20.83888888888889, x_max=24.216, y_max=105.71000000000002
         📦 Updated annotation with 54 transformed points
   Original: 1 → Transformed: 1
✅ NEW SEGMENTATION FUNCTION RESULT: 1 lines

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 63.1}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 1 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 20.83888888888889, 24.216, 105.71000000000002)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 2

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 2
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 2 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': 63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 2 annotations individually
   🔄 Processing annotation 1/2: dog

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   width: 24.216, height: 84.87111111111113
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-400.0, -279.1611111111111), (-375.784, -279.1611111111111), (-400.0, -194.28999999999996), (-375.784, -194.28999999999996)]
   corner 0: (-400.0, -279.1611111111111) → (467.9813055260225, -183.02118799879543)
   corner 1: (-375.784, -279.1611111111111) → (478.9374644467166, -161.42541902187554)
   corner 2: (-400.0, -194.28999999999996) → (392.29345830228397, -144.6225515142719)
   corner 3: (-375.784, -194.28999999999996) → (403.24961722297803, -123.026782537352)
   all x coords: [467.9813055260225, 478.9374644467166, 392.29345830228397, 403.24961722297803]
   all y coords: [-183.02118799879543, -161.42541902187554, -144.6225515142719, -123.026782537352]       
   new bounds: x_min=392.29345830228397, x_max=478.9374644467166, y_min=-183.02118799879543, y_max=-123.026782537352
📍 FINAL BBOX (after rotation):
   x_min: 392.29345830228397, y_min: -183.02118799879543
   x_max: 478.9374644467166, y_max: -123.026782537352
   width: 86.64400614443264, height: 59.99440546144342
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 392.29345830228397, y_min: -183.02118799879543
   x_max: 478.9374644467166, y_max: -123.026782537352
   width: 86.64400614443264, height: 59.99440546144342
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 392.29345830228397, x_max: 478.9374644467166
   y_min: -183.02118799879543, y_max: -123.026782537352
📍 AFTER SCALING:
   x_min: 502.1356266269235, x_max: 613.0399544917973
   y_min: -312.05112553794623, y_max: -209.76066422618518
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=502.1356266269235, y_min=-312.05112553794623, x_max=613.0399544917973, y_max=-209.76066422618518
   🔄 Processing annotation 2/2: dog
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 2
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 2
Transformed annotations: 2
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 2 annotations
   First transformed annotation: (0.0, 20.83888888888889, 24.216, 105.71000000000002)

=== DEBUG YOLO DUMP :: dog_rotate63.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,20.84,24.22,105.71]
  ann[1] POLY -> 54 pts; min=(504.9,0.0) max=(606.4,0.0)
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 1
  det: 1 0.011824 0.061852 0.023648 0.082963
YOLO SEG lines: 1
  seg: 1 0.551356 0.000000 0.556256 0.000000 0.562122 0.000000 0.566659 0.000000 0.570020 0.000000 0.574778 0.000000 0.581511 0...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['flip', 'resize'], 'geometric_transforms_order': ['flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'flip', 'params': {'horizontal': True}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 1 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 20.83888888888889, 24.216, 105.71000000000002)

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
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 2

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 2
   transformation_config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 2 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 2 annotations individually
   🔄 Processing annotation 1/2: dog

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. flip: {'enabled': True, 'horizontal': True}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
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
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   width: 24.216, height: 84.87111111111113
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=0.0, x_max=24.216
   After: x_min=775.784, x_max=800.0
📍 FINAL BBOX (after flip):
   x_min: 775.784, y_min: 20.83888888888889
   x_max: 800.0, y_max: 105.71000000000002
   width: 24.216000000000008, height: 84.87111111111113
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 775.784, y_min: 20.83888888888889
   x_max: 800.0, y_max: 105.71000000000002
   width: 24.216000000000008, height: 84.87111111111113
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 775.784, x_max: 800.0
   y_min: 20.83888888888889, y_max: 105.71000000000002
📍 AFTER SCALING:
   x_min: 993.00352, x_max: 1024.0
   y_min: 35.53030555555556, y_max: 180.23555000000005
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=993.00352, y_min=35.53030555555556, x_max=1024.0, y_max=180.23555000000005     
   🔄 Processing annotation 2/2: dog
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 2
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 2
Transformed annotations: 2
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['flip', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 2 annotations
   First transformed annotation: (0.0, 20.83888888888889, 24.216, 105.71000000000002)

=== DEBUG YOLO DUMP :: dog_flip_horizontal.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,20.84,24.22,105.71]
  ann[1] POLY -> 54 pts; min=(993.0,35.5) max=(1024.0,180.2)
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 1
  det: 1 0.011824 0.061852 0.023648 0.082963
YOLO SEG lines: 1
  seg: 1 1.000000 0.084997 1.000000 0.077672 0.999730 0.069084 0.998290 0.063274 0.997210 0.058980 0.997150 0.051908 0.995710 0...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -63.1}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 1 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 20.83888888888889, 24.216, 105.71000000000002)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 2

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 2
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 2 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': -63.1}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 2 annotations individually
   🔄 Processing annotation 1/2: dog

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 2
   1. rotate: enabled=True, affects_coordinates=True
   2. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   width: 24.216, height: 84.87111111111113
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-400.0, -279.1611111111111), (-375.784, -279.1611111111111), (-400.0, -194.28999999999996), (-375.784, -194.28999999999996)]
   corner 0: (-400.0, -279.1611111111111) → (-29.929072975448605, 530.4168356853759)
   corner 1: (-375.784, -279.1611111111111) → (-18.972914054754483, 508.821066708456)
   corner 2: (-400.0, -194.28999999999996) → (45.75877424828991, 568.8154721698994)
   corner 3: (-375.784, -194.28999999999996) → (56.71493316898409, 547.2197031929795)
   all x coords: [-29.929072975448605, -18.972914054754483, 45.75877424828991, 56.71493316898409]        
   all y coords: [530.4168356853759, 508.821066708456, 568.8154721698994, 547.2197031929795]
   new bounds: x_min=-29.929072975448605, x_max=56.71493316898409, y_min=508.821066708456, y_max=568.8154721698994
📍 FINAL BBOX (after rotation):
   x_min: -29.929072975448605, y_min: 508.821066708456
   x_max: 56.71493316898409, y_max: 568.8154721698994
   width: 86.6440061444327, height: 59.99440546144342
✅ ROTATION COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: -29.929072975448605, y_min: 508.821066708456
   x_max: 56.71493316898409, y_max: 568.8154721698994
   width: 86.6440061444327, height: 59.99440546144342
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: -29.929072975448605, x_max: 56.71493316898409
   y_min: 508.821066708456, y_max: 568.8154721698994
📍 AFTER SCALING:
   x_min: -38.309213408574216, x_max: 72.59511445629964
   y_min: 867.5399187379174, y_max: 969.8303800496785
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=-38.309213408574216, y_min=867.5399187379174, x_max=72.59511445629964, y_max=969.8303800496785
   🔄 Processing annotation 2/2: dog
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 2
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 2
Transformed annotations: 2
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 2 annotations
   First transformed annotation: (0.0, 20.83888888888889, 24.216, 105.71000000000002)

=== DEBUG YOLO DUMP :: dog_rotate-63.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,20.84,24.22,105.71]
  ann[1] POLY -> 54 pts; min=(0.0,884.5) max=(71.5,962.6)
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 1
  det: 1 0.011824 0.061852 0.023648 0.082963
YOLO SEG lines: 1
  seg: 1 0.000000 0.906770 0.000000 0.903456 0.000000 0.899249 0.000000 0.894909 0.000000 0.891682 0.000000 0.888410 0.000000 0...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['rotate', 'flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -63.1}}, {'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 2, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'flip', 'resize'], 'geometric_transforms_order': ['rotate', 'flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}], 'photometric_transforms': [], 'total_transforms': 3, 'geometric_count': 3, 'photometric_count': 0}
🔍 DEBUG: About to transform 1 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 20.83888888888889, 24.216, 105.71000000000002)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 2

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 2
   transformation_config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 2 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': -63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 2 annotations individually
   🔄 Processing annotation 1/2: dog

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': -63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: -63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   width: 24.216, height: 84.87111111111113
🔄 ROTATION CALCULATIONS:
   angle_rad: -1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: -0.8917975296052141
   corners (relative to center): [(-400.0, -279.1611111111111), (-375.784, -279.1611111111111), (-400.0, -194.28999999999996), (-375.784, -194.28999999999996)]
   corner 0: (-400.0, -279.1611111111111) → (-29.929072975448605, 530.4168356853759)
   corner 1: (-375.784, -279.1611111111111) → (-18.972914054754483, 508.821066708456)
   corner 2: (-400.0, -194.28999999999996) → (45.75877424828991, 568.8154721698994)
   corner 3: (-375.784, -194.28999999999996) → (56.71493316898409, 547.2197031929795)
   all x coords: [-29.929072975448605, -18.972914054754483, 45.75877424828991, 56.71493316898409]        
   all y coords: [530.4168356853759, 508.821066708456, 568.8154721698994, 547.2197031929795]
   new bounds: x_min=-29.929072975448605, x_max=56.71493316898409, y_min=508.821066708456, y_max=568.8154721698994
📍 FINAL BBOX (after rotation):
   x_min: -29.929072975448605, y_min: 508.821066708456
   x_max: 56.71493316898409, y_max: 568.8154721698994
   width: 86.6440061444327, height: 59.99440546144342
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: -29.929072975448605, y_min: 508.821066708456
   x_max: 56.71493316898409, y_max: 568.8154721698994
   width: 86.6440061444327, height: 59.99440546144342
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=-29.929072975448605, x_max=56.71493316898409
   After: x_min=743.2850668310159, x_max=829.9290729754487
📍 FINAL BBOX (after flip):
   x_min: 743.2850668310159, y_min: 508.821066708456
   x_max: 829.9290729754487, y_max: 568.8154721698994
   width: 86.64400614443275, height: 59.99440546144342
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 743.2850668310159, y_min: 508.821066708456
   x_max: 829.9290729754487, y_max: 568.8154721698994
   width: 86.64400614443275, height: 59.99440546144342
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 743.2850668310159, x_max: 829.9290729754487
   y_min: 508.821066708456, y_max: 568.8154721698994
📍 AFTER SCALING:
   x_min: 951.4048855437004, x_max: 1062.3092134085744
   y_min: 867.5399187379174, y_max: 969.8303800496785
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=951.4048855437004, y_min=867.5399187379174, x_max=1062.3092134085744, y_max=969.8303800496785
   🔄 Processing annotation 2/2: dog
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 2
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 2
Transformed annotations: 2
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'flip', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 2 annotations
   First transformed annotation: (0.0, 20.83888888888889, 24.216, 105.71000000000002)

=== DEBUG YOLO DUMP :: dog_rotate-63_flip_horizontal.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,20.84,24.22,105.71]
  ann[1] POLY -> 54 pts; min=(952.5,884.5) max=(1024.0,962.6)
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 1
  det: 1 0.011824 0.061852 0.023648 0.082963
YOLO SEG lines: 1
  seg: 1 1.000000 0.906770 1.000000 0.903456 1.000000 0.899249 1.000000 0.894909 1.000000 0.891682 1.000000 0.888410 1.000000 0...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

🖼️ IMAGE GENERATION ORDER: ['rotate', 'flip', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 63.1}}, {'type': 'flip', 'params': {'horizontal': True}}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}}]
   Original dims: (800, 600)
   Final dims: (1024, 1023)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 1024, 'height': 1023}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'flip', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'flip', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 63.1}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'flip', 'params': {'horizontal': True}, 'is_geometric': True, 'is_photometric': False}, {'index': 2, 'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}, 'original_dims': (800, 600), 'final_dims': (1024, 1023), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'flip', 'resize'], 'geometric_transforms_order': ['rotate', 'flip', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 63.1}, 'index': 0}, {'type': 'flip', 'params': {'horizontal': True}, 'index': 1}, {'type': 'resize', 'params': {'width': 1024, 'height': 1023}, 'index': 2}], 'photometric_transforms': [], 'total_transforms': 3, 'geometric_count': 3, 'photometric_count': 0}
🔍 DEBUG: About to transform 1 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 20.83888888888889, 24.216, 105.71000000000002)

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
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   annotation_count: 2

🔧 ABOUT TO CALL update_annotations_for_transformations:
   annotations count: 2
   transformation_config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   original_dims: (800, 600)
   new_dims: (1024, 1023)
   affine_matrix: None
   debug_tracking: True

🔄 UPDATE_ANNOTATIONS_FOR_TRANSFORMATIONS CALLED!
   📊 Input: 2 annotations
   📐 Dimensions: (800, 600) → (1024, 1023)
   🔧 Transform config: {'rotate': {'enabled': True, 'angle': 63.1}, 'flip': {'enabled': True, 'horizontal': True}, 'resize': {'enabled': True, 'width': 1024, 'height': 1023}}
   🎯 Has affine matrix: False
   🎯 RESIZE MODE: stretch_to
   📏 Target size: 1024x1023
   📏 Original size: 800.0x600.0
   📐 STRETCH_TO: final_canvas=1024x1023
   🎯 FINAL CANVAS DIMENSIONS: (1024, 1023)
   🔧 USING LEGACY/SEQUENTIAL TRANSFORMATION PATH
   📊 Processing 2 annotations individually
   🔄 Processing annotation 1/2: dog

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
   new_dims: (1024, 1023)
🔧 TRANSFORMATION CONFIG:
   1. rotate: {'enabled': True, 'angle': 63.1}
   2. flip: {'enabled': True, 'horizontal': True}
   3. resize: {'enabled': True, 'width': 1024, 'height': 1023}
================================================================================
🔢 INITIAL VALUES:
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   current_width: 800, current_height: 600

🔄 TRANSFORMATION SEQUENCE:
   Total transformations: 3
   1. rotate: enabled=True, affects_coordinates=True
   2. flip: enabled=True, affects_coordinates=True
   3. resize: enabled=True, affects_coordinates=True


🔄 ROTATION TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   angle: 63.1 degrees
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before rotation):
   x_min: 0.0, y_min: 20.83888888888889
   x_max: 24.216, y_max: 105.71000000000002
   width: 24.216, height: 84.87111111111113
🔄 ROTATION CALCULATIONS:
   angle_rad: 1.101302758008422
   center: (400.0, 300.0)
   cos_a: 0.45243470931178265, sin_a: 0.8917975296052141
   corners (relative to center): [(-400.0, -279.1611111111111), (-375.784, -279.1611111111111), (-400.0, -194.28999999999996), (-375.784, -194.28999999999996)]
   corner 0: (-400.0, -279.1611111111111) → (467.9813055260225, -183.02118799879543)
   corner 1: (-375.784, -279.1611111111111) → (478.9374644467166, -161.42541902187554)
   corner 2: (-400.0, -194.28999999999996) → (392.29345830228397, -144.6225515142719)
   corner 3: (-375.784, -194.28999999999996) → (403.24961722297803, -123.026782537352)
   all x coords: [467.9813055260225, 478.9374644467166, 392.29345830228397, 403.24961722297803]
   all y coords: [-183.02118799879543, -161.42541902187554, -144.6225515142719, -123.026782537352]       
   new bounds: x_min=392.29345830228397, x_max=478.9374644467166, y_min=-183.02118799879543, y_max=-123.026782537352
📍 FINAL BBOX (after rotation):
   x_min: 392.29345830228397, y_min: -183.02118799879543
   x_max: 478.9374644467166, y_max: -123.026782537352
   width: 86.64400614443264, height: 59.99440546144342
✅ ROTATION COMPLETE
============================================================

🔄 FLIP TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   horizontal: True
   vertical: False
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before flip):
   x_min: 392.29345830228397, y_min: -183.02118799879543
   x_max: 478.9374644467166, y_max: -123.026782537352
   width: 86.64400614443264, height: 59.99440546144342
🔄 APPLYING HORIZONTAL FLIP:
   Before: x_min=392.29345830228397, x_max=478.9374644467166
   After: x_min=321.0625355532834, x_max=407.70654169771603
📍 FINAL BBOX (after flip):
   x_min: 321.0625355532834, y_min: -183.02118799879543
   x_max: 407.70654169771603, y_max: -123.026782537352
   width: 86.64400614443264, height: 59.99440546144342
✅ FLIP COMPLETE
============================================================

🔍 RESIZE TRANSFORMATION DEBUG
============================================================
📊 INPUT PARAMETERS:
   target_width: 1024
   target_height: 1023
   resize_mode: stretch_to
   current_width: 800
   current_height: 600
📍 ORIGINAL BBOX (before resize):
   x_min: 321.0625355532834, y_min: -183.02118799879543
   x_max: 407.70654169771603, y_max: -123.026782537352
   width: 86.64400614443264, height: 59.99440546144342
🔢 FLOAT CONVERSIONS:
   source_w: 800.0, source_h: 600.0
   tw: 1024.0, th: 1023.0
🎯 STRETCH_TO MODE:
   sx = 1024.0 / 800.0 = 1.28
   sy = 1023.0 / 600.0 = 1.705
📍 BEFORE SCALING:
   x_min: 321.0625355532834, x_max: 407.70654169771603
   y_min: -183.02118799879543, y_max: -123.026782537352
📍 AFTER SCALING:
   x_min: 410.96004550820277, x_max: 521.8643733730765
   y_min: -312.05112553794623, y_max: -209.76066422618518
🖼️ CANVAS SIZE: 1024.0 x 1023.0
✅ RESIZE COMPLETE - NEW CANVAS: 1024.0 x 1023.0
============================================================

🔧 FINAL CLIPPING AND VALIDATION:
   Before clipping: x_min=410.96004550820277, y_min=-312.05112553794623, x_max=521.8643733730765, y_max=-209.76066422618518
   🔄 Processing annotation 2/2: dog
🔧 update_annotations_for_transformations RETURNED:
   transformed_annotations count: 2
   transformer_debug keys: ['transformation_method', 'transformation_config', 'original_dims', 'new_dims', 'actual_final_canvas_dims', 'annotation_steps', 'actual_canvas_dimensions']

=== ANNOTATION TRANSFORMATION RESULTS ===
Original annotations: 2
Transformed annotations: 2
Original dims: (800, 600)
Final dims: (1024, 1023)
Transformation config: ['rotate', 'flip', 'resize']
Resize mode: stretch_to -> 1024x1023
Actual final canvas: (1024, 1023)
🔍 DEBUG: Transformation result: 2 annotations
   First transformed annotation: (0.0, 20.83888888888889, 24.216, 105.71000000000002)

=== DEBUG YOLO DUMP :: dog_rotate63_flip_horizontal.jpg ===
final canvas passed to YOLO: 1024x1023
✅ USING ANNOTATIONS AS-IS (assuming already transformed if needed)
  ann[0] BBOX -> [0.00,20.84,24.22,105.71]
  ann[1] POLY -> 54 pts; min=(417.6,0.0) max=(519.1,0.0)
🎯 NEW DETECTION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 2
   Final dims: 1024x1023
   Has transform_config: False
   Original dims: None
⚠️  NO TRANSFORMATION - using raw annotations
YOLO DET lines: 1
  det: 1 0.011824 0.061852 0.023648 0.082963
YOLO SEG lines: 1
  seg: 1 0.448644 0.000000 0.443744 0.000000 0.437878 0.000000 0.433341 0.000000 0.429980 0.000000 0.425222 0.000000 0.418489 0...
❌ INVALID LOG CATEGORY: 'errors.debug' is not in the 17-log-file plan!
📋 Valid categories: ['app.backend', 'app.api', 'app.startup', 'app.database', 'operations.images', 'operations.datasets', 'operations.exports', 'operations.operations', 'operations.annotations', 'operations.releases', 'operations.transformations', 'errors.system', 'errors.validation', 'app.frontend.interactions', 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

=== 📋 WRITING ANNOTATIONS.JSON ===
Total images with annotations: 18
   images\train\cat.jpg: 3 annotations
      First annotation: {'class_id': 0, 'polygon': [0.0, 0.098444, 0.0, 0.095037, 0.0, 0.087778, 0.0, 0.085259, 0.0, 0.084667, 0.0, 0.075185, 0.00068, 0.065852, 0.00143, 0.059333, 0.002227, 0.050889, 0.002555, 0.046444, 0.002695, 0.041852, 0.002648, 0.037111, 0.00232, 0.031333, 0.002086, 0.023778, 0.002414, 0.020815, 0.003398, 0.023037, 0.005227, 0.026296, 0.00668, 0.030889, 0.007852, 0.03163, 0.009867, 0.03163, 0.011789, 0.031333, 0.013242, 0.029704, 0.014883, 0.02437, 0.016945, 0.02363, 0.016898, 0.02763, 0.016242, 0.032815, 0.01582, 0.039037, 0.015633, 0.044667, 0.015727, 0.049111, 0.015633, 0.054444, 0.015398, 0.061111, 0.016242, 0.063037, 0.017508, 0.06437, 0.018633, 0.06763, 0.019992, 0.069852, 0.019477, 0.073407, 0.017742, 0.070296, 0.01657, 0.067185, 0.016148, 0.066889, 0.017648, 0.070889, 0.018352, 0.073852, 0.018445, 0.076963, 0.017508, 0.077704, 0.017039, 0.074444, 0.01643, 0.072667, 0.01568, 0.070444, 0.015445, 0.069852, 0.01568, 0.073852, 0.01643, 0.075481, 0.01807, 0.076667, 0.019242, 0.075926, 0.020367, 0.07637, 0.021914, 0.078593, 0.025898, 0.083333, 0.026273, 0.085111, 0.025992, 0.086593, 0.023836, 0.086444, 0.022102, 0.086593, 0.019336, 0.086741, 0.01882, 0.086741, 0.018773, 0.089852, 0.018492, 0.093556, 0.017508, 0.095926, 0.016008, 0.097556, 0.014648, 0.095778, 0.014039, 0.092222, 0.013664, 0.089259, 0.013477, 0.087185, 0.011648, 0.086889, 0.008367, 0.08763, 0.005086, 0.087185, 0.004195, 0.087185, 0.00443, 0.09163, 0.004195, 0.096074, 0.00307, 0.098444, 0.001617, 0.101259, 0.000633, 0.100519]}
   images\train\cat_flip_horizontal.jpg: 3 annotations
      First annotation: {'class_id': 12, 'polygon': [1.0, 0.167848, 1.0, 0.162038, 1.0, 0.149661, 1.0, 0.145367, 1.0, 0.144357, 1.0, 0.128191, 0.99913, 0.112277, 0.99817, 0.101163, 0.99715, 0.086766, 0.99673, 0.079188, 0.99655, 0.071357, 0.99661, 0.063274, 0.99703, 0.053423, 0.99733, 0.040541, 0.99691, 0.035489, 0.99565, 0.039278, 0.99331, 0.044835, 0.99145, 0.052666, 0.98995, 0.053929, 0.98737, 0.053929, 0.98491, 0.053423, 0.98305, 0.050645, 0.98095, 0.041551, 0.97831, 0.040289, 0.97837, 0.047109, 0.97921, 0.055949, 0.97975, 0.066558, 0.97999, 0.076157, 0.97987, 0.083734, 0.97999, 0.092828, 0.98029, 0.104194, 0.97921, 0.107478, 0.97759, 0.109751, 0.97615, 0.115309, 0.97441, 0.119097, 0.97507, 0.12516, 0.97729, 0.119855, 0.97879, 0.114551, 0.97933, 0.114046, 0.97741, 0.120866, 0.97651, 0.125917, 0.97639, 0.131222, 0.97759, 0.132485, 0.97819, 0.126928, 0.97897, 0.123897, 0.97993, 0.120108, 0.98023, 0.119097, 0.97993, 0.125917, 0.97897, 0.128696, 0.97687, 0.130717, 0.97537, 0.129454, 0.97393, 0.130211, 0.97195, 0.134, 0.96685, 0.142083, 0.96637, 0.145114, 0.96673, 0.14764, 0.96949, 0.147388, 0.97171, 0.14764, 0.97525, 0.147893, 0.97591, 0.147893, 0.97597, 0.153197, 0.97633, 0.159512, 0.97759, 0.163554, 0.97951, 0.166332, 0.98125, 0.163301, 0.98203, 0.157239, 0.98251, 0.152187, 0.98275, 0.148651, 0.98509, 0.148146, 0.98929, 0.149409, 0.99349, 0.148651, 0.99463, 0.148651, 0.99433, 0.156229, 0.99463, 0.163806, 0.99607, 0.167848, 0.99793, 0.172647, 0.99919, 0.171384]}
   images\train\cat_rotate-63.jpg: 3 annotations
      First annotation: {'class_id': 12, 'polygon': [0.051623, 0.944254, 0.047737, 0.941626, 0.039459, 0.936026, 0.036587, 0.934083, 0.035911, 0.933626, 0.025099, 0.926312, 0.014849, 0.918078, 0.007849, 0.911908, 0.0, 0.904181, 0.0, 0.900253, 0.0, 0.896497, 0.0, 0.892911, 0.0, 0.888953, 0.0, 0.883482, 0.0, 0.880697, 0.0, 0.880913, 0.0, 0.880644, 0.0, 0.881976, 0.0, 0.880763, 0.0, 0.877696, 0.0, 0.874542, 0.0, 0.871073, 0.0, 0.864462, 0.0, 0.860751, 0.0, 0.863908, 0.0, 0.868907, 0.0, 0.874349, 0.0, 0.878977, 0.004472, 0.882263, 0.010499, 0.88652, 0.017966, 0.892019, 0.020651, 0.892221, 0.022905, 0.891323, 0.027273, 0.892125, 0.030594, 0.89177, 0.034351, 0.895298, 0.029798, 0.895537, 0.025572, 0.894921, 0.02499, 0.895335, 0.03042, 0.896137, 0.034206, 0.897353, 0.037808, 0.89961, 0.03811, 0.901608, 0.034122, 0.899807, 0.031741, 0.899363, 0.028773, 0.898791, 0.027961, 0.89869, 0.032659, 0.901419, 0.034951, 0.901535, 0.037253, 0.899952, 0.037087, 0.897597, 0.038245, 0.896228, 0.041675, 0.895588, 0.049389, 0.89318, 0.051633, 0.893981, 0.05316, 0.895552, 0.051742, 0.898719, 0.050907, 0.901473, 0.049474, 0.905797, 0.049176, 0.906582, 0.052696, 0.909053, 0.056757, 0.912338, 0.05889, 0.915665, 0.05988, 0.919205, 0.057065, 0.919902, 0.052658, 0.918087, 0.049062, 0.916372, 0.046588, 0.915058, 0.045191, 0.917612, 0.044136, 0.923177, 0.041729, 0.927828, 0.041213, 0.929184, 0.046417, 0.932256, 0.05135, 0.936041, 0.053401, 0.939581, 0.05577, 0.943964, 0.054355, 0.944891]}
   images\train\cat_rotate-63_flip_horizontal.jpg: 3 annotations
      First annotation: {'class_id': 12, 'polygon': [0.948377, 0.944254, 0.952263, 0.941626, 0.960541, 0.936026, 0.963413, 0.934083, 0.964089, 0.933626, 0.974901, 0.926312, 0.985151, 0.918078, 0.992151, 0.911908, 1.0, 0.904181, 1.0, 0.900253, 1.0, 0.896497, 1.0, 0.892911, 1.0, 0.888953, 1.0, 0.883482, 1.0, 0.880697, 1.0, 0.880913, 1.0, 0.880644, 1.0, 0.881976, 1.0, 0.880763, 1.0, 0.877696, 1.0, 0.874542, 1.0, 0.871073, 1.0, 0.864462, 1.0, 0.860751, 1.0, 0.863908, 1.0, 0.868907, 1.0, 0.874349, 1.0, 0.878977, 0.995528, 0.882263, 0.989501, 0.88652, 0.982034, 0.892019, 0.979349, 0.892221, 0.977095, 0.891323, 0.972727, 0.892125, 0.969406, 0.89177, 0.965649, 0.895298, 0.970202, 0.895537, 0.974428, 0.894921, 0.97501, 0.895335, 0.96958, 0.896137, 0.965794, 0.897353, 0.962192, 0.89961, 0.96189, 0.901608, 0.965878, 0.899807, 0.968259, 0.899363, 0.971227, 0.898791, 0.972039, 0.89869, 0.967341, 0.901419, 0.965049, 0.901535, 0.962747, 0.899952, 0.962913, 0.897597, 0.961755, 0.896228, 0.958325, 0.895588, 0.950611, 0.89318, 0.948367, 0.893981, 0.94684, 0.895552, 0.948258, 0.898719, 0.949093, 0.901473, 0.950526, 0.905797, 0.950824, 0.906582, 0.947304, 0.909053, 0.943243, 0.912338, 0.94111, 0.915665, 0.94012, 0.919205, 0.942935, 0.919902, 0.947342, 0.918087, 0.950938, 0.916372, 0.953412, 0.915058, 0.954809, 0.917612, 0.955864, 0.923177, 0.958271, 0.927828, 0.958787, 0.929184, 0.953583, 0.932256, 0.94865, 0.936041, 0.946599, 0.939581, 0.94423, 0.943964, 0.945645, 0.944891]}
   images\train\cat_rotate63.jpg: 3 annotations
      First annotation: {'class_id': 12, 'polygon': [0.495942, 0.0, 0.499828, 0.0, 0.508106, 0.0, 0.510978, 0.0, 0.511654, 0.0, 0.522467, 0.0, 0.533504, 0.0, 0.541372, 0.0, 0.551463, 0.0, 0.556722, 0.0, 0.56204, 0.0, 0.567419, 0.0, 0.573818, 0.0, 0.582299, 0.0, 0.585868, 0.0, 0.583904, 0.0, 0.581246, 0.0, 0.57685, 0.0, 0.576684, 0.0, 0.577851, 0.0, 0.579302, 0.0, 0.582002, 0.0, 0.589034, 0.0, 0.591073, 0.0, 0.586484, 0.0, 0.580191, 0.0, 0.572851, 0.0, 0.566323, 0.0, 0.561309, 0.0, 0.555172, 0.0, 0.547434, 0.0, 0.545726, 0.0, 0.544939, 0.0, 0.541873, 0.0, 0.540126, 0.0, 0.535773, 0.0, 0.538317, 0.0, 0.541186, 0.0, 0.541279, 0.0, 0.537587, 0.0, 0.534615, 0.0, 0.531121, 0.0, 0.529734, 0.0, 0.533179, 0.0, 0.534853, 0.0, 0.536953, 0.0, 0.537493, 0.0, 0.533067, 0.0, 0.531643, 0.0, 0.531242, 0.0, 0.532765, 0.0, 0.53291, 0.0, 0.531272, 0.0, 0.528173, 0.0, 0.526363, 0.0, 0.52451, 0.0, 0.52343, 0.0, 0.522257, 0.0, 0.520487, 0.0, 0.520188, 0.0, 0.516613, 0.0, 0.512226, 0.0, 0.508953, 0.0, 0.506226, 0.0, 0.507466, 0.0, 0.511168, 0.0, 0.51433, 0.0, 0.516586, 0.0, 0.515866, 0.0, 0.513121, 0.0, 0.511727, 0.0, 0.511212, 0.0, 0.506279, 0.0, 0.501075, 0.0, 0.49772, 0.0, 0.493669, 0.0, 0.493943, 0.0]}
   images\train\cat_rotate63_flip_horizontal.jpg: 3 annotations
      First annotation: {'class_id': 12, 'polygon': [0.504058, 0.0, 0.500172, 0.0, 0.491894, 0.0, 0.489022, 0.0, 0.488346, 0.0, 0.477533, 0.0, 0.466496, 0.0, 0.458628, 0.0, 0.448537, 0.0, 0.443278, 0.0, 0.43796, 0.0, 0.432581, 0.0, 0.426182, 0.0, 0.417701, 0.0, 0.414132, 0.0, 0.416096, 0.0, 0.418754, 0.0, 0.42315, 0.0, 0.423316, 0.0, 0.422149, 0.0, 0.420698, 0.0, 0.417998, 0.0, 0.410966, 0.0, 0.408927, 0.0, 0.413516, 0.0, 0.419809, 0.0, 0.427149, 0.0, 0.433677, 0.0, 0.438691, 0.0, 0.444828, 0.0, 0.452566, 0.0, 0.454274, 0.0, 0.455061, 0.0, 0.458127, 0.0, 0.459874, 0.0, 0.464227, 0.0, 0.461683, 0.0, 0.458814, 0.0, 0.458721, 0.0, 0.462413, 0.0, 0.465385, 0.0, 0.468879, 0.0, 0.470266, 0.0, 0.466821, 0.0, 0.465147, 0.0, 0.463047, 0.0, 0.462507, 0.0, 0.466933, 0.0, 0.468357, 0.0, 0.468758, 0.0, 0.467235, 0.0, 0.46709, 0.0, 0.468728, 0.0, 0.471827, 0.0, 0.473637, 0.0, 0.47549, 0.0, 0.47657, 0.0, 0.477743, 0.0, 0.479513, 0.0, 0.479812, 0.0, 0.483387, 0.0, 0.487774, 0.0, 0.491047, 0.0, 0.493774, 0.0, 0.492534, 0.0, 0.488832, 0.0, 0.48567, 0.0, 0.483414, 0.0, 0.484134, 0.0, 0.486879, 0.0, 0.488273, 0.0, 0.488788, 0.0, 0.493721, 0.0, 0.498925, 0.0, 0.50228, 0.0, 0.506331, 0.0, 0.506057, 0.0]}
   images\val\car.jpg: 2 annotations
      First annotation: {'class_id': 2, 'polygon': [0.0, 0.103481, 0.0, 0.098741, 0.0, 0.093111, 0.0, 0.083037, 0.0, 0.075333, 0.0, 0.069556, 0.000305, 0.065852, 0.000258, 0.062148, 0.001242, 0.059185, 0.002461, 0.056074, 0.003492, 0.052222, 0.004289, 0.049259, 0.004758, 0.047926, 0.005273, 0.046593, 0.005883, 0.04037, 0.00668, 0.035926, 0.007102, 0.034444, 0.008133, 0.034, 0.009961, 0.038889, 0.011227, 0.045704, 0.011883, 0.045556, 0.012398, 0.044074, 0.012773, 0.041259, 0.013008, 0.039037, 0.01357, 0.035481, 0.014789, 0.031185, 0.016242, 0.030889, 0.016195, 0.035778, 0.016148, 0.042889, 0.015773, 0.04763, 0.016008, 0.049704, 0.017133, 0.052667, 0.017883, 0.057704, 0.017836, 0.062, 0.018352, 0.065704, 0.018492, 0.072815, 0.017414, 0.075037, 0.015539, 0.075333, 0.014227, 0.075333, 0.013383, 0.075778, 0.011602, 0.078444, 0.012117, 0.082741, 0.012352, 0.084963, 0.012492, 0.087778, 0.012492, 0.090444, 0.013055, 0.095481, 0.013289, 0.098296, 0.013383, 0.101259, 0.013195, 0.103333]}
   images\val\car_flip_horizontal.jpg: 2 annotations
      First annotation: {'class_id': 1, 'polygon': [1.0, 0.176436, 1.0, 0.168353, 1.0, 0.158754, 1.0, 0.141578, 1.0, 0.128443, 1.0, 0.118592, 0.99961, 0.112277, 0.99967, 0.105963, 0.99841, 0.100911, 0.99685, 0.095606, 0.99553, 0.089039, 0.99451, 0.083987, 0.99391, 0.081714, 0.99325, 0.07944, 0.99247, 0.068831, 0.99145, 0.061254, 0.99091, 0.058728, 0.98959, 0.05797, 0.98725, 0.066306, 0.98563, 0.077925, 0.98479, 0.077672, 0.98413, 0.075146, 0.98365, 0.070347, 0.98335, 0.066558, 0.98263, 0.060496, 0.98107, 0.053171, 0.97921, 0.052666, 0.97927, 0.061001, 0.97933, 0.073126, 0.97981, 0.081209, 0.97951, 0.084745, 0.97807, 0.089797, 0.97711, 0.098385, 0.97717, 0.10571, 0.97651, 0.112025, 0.97633, 0.124149, 0.97771, 0.127938, 0.98011, 0.128443, 0.98179, 0.128443, 0.98287, 0.129201, 0.98515, 0.133748, 0.98449, 0.141073, 0.98419, 0.144862, 0.98401, 0.149661, 0.98401, 0.154208, 0.98329, 0.162796, 0.98299, 0.167595, 0.98287, 0.172647, 0.98311, 0.176183]}
   images\val\car_rotate-63.jpg: 2 annotations
      First annotation: {'class_id': 1, 'polygon': [0.057367, 0.94814, 0.051961, 0.944483, 0.045541, 0.94014, 0.034053, 0.932369, 0.025268, 0.926427, 0.018679, 0.92197, 0.014632, 0.918649, 0.010381, 0.915863, 0.007572, 0.912079, 0.00473, 0.907824, 0.000934, 0.903284, 0.0, 0.899785, 0.0, 0.898043, 0.0, 0.89623, 0.0, 0.890502, 0.0, 0.885861, 0.0, 0.884076, 0.0, 0.882164, 0.0, 0.883153, 0.0, 0.886483, 0.0, 0.88537, 0.0, 0.883443, 0.0, 0.880701, 0.0, 0.87863, 0.0, 0.875031, 0.0, 0.869862, 0.0, 0.867421, 0.0, 0.871264, 0.0, 0.876821, 0.002809, 0.881049, 0.00531, 0.882292, 0.009341, 0.882865, 0.015519, 0.885609, 0.020392, 0.888995, 0.024914, 0.891067, 0.033105, 0.896339, 0.035015, 0.899694, 0.034267, 0.902776, 0.033506, 0.904774, 0.033525, 0.906401, 0.035534, 0.911169, 0.040732, 0.913698, 0.043402, 0.915056, 0.046694, 0.917013, 0.049735, 0.91907, 0.055805, 0.9221, 0.05915, 0.923914, 0.062583, 0.926057, 0.06484, 0.927943]}
   images\val\car_rotate-63_flip_horizontal.jpg: 2 annotations
      First annotation: {'class_id': 1, 'polygon': [0.942633, 0.94814, 0.948039, 0.944483, 0.954459, 0.94014, 0.965947, 0.932369, 0.974732, 0.926427, 0.981321, 0.92197, 0.985368, 0.918649, 0.989619, 0.915863, 0.992428, 0.912079, 0.99527, 0.907824, 0.999066, 0.903284, 1.0, 0.899785, 1.0, 0.898043, 1.0, 0.89623, 1.0, 0.890502, 1.0, 0.885861, 1.0, 0.884076, 1.0, 0.882164, 1.0, 0.883153, 1.0, 0.886483, 1.0, 0.88537, 1.0, 0.883443, 1.0, 0.880701, 1.0, 0.87863, 1.0, 0.875031, 1.0, 0.869862, 1.0, 0.867421, 1.0, 0.871264, 1.0, 0.876821, 0.997191, 0.881049, 0.99469, 0.882292, 0.990659, 0.882865, 0.984481, 0.885609, 0.979608, 0.888995, 0.975086, 0.891067, 0.966895, 0.896339, 0.964985, 0.899694, 0.965733, 0.902776, 0.966494, 0.904774, 0.966475, 0.906401, 0.964466, 0.911169, 0.959268, 0.913698, 0.956598, 0.915056, 0.953306, 0.917013, 0.950265, 0.91907, 0.944195, 0.9221, 0.94085, 0.923914, 0.937417, 0.926057, 0.93516, 0.927943]}
   images\val\car_rotate63.jpg: 2 annotations
      First annotation: {'class_id': 1, 'polygon': [0.490198, 0.0, 0.495604, 0.0, 0.502024, 0.0, 0.513512, 0.0, 0.522298, 0.0, 0.528887, 0.0, 0.533287, 0.0, 0.537483, 0.0, 0.541432, 0.0, 0.545686, 0.0, 0.550676, 0.0, 0.554516, 0.0, 0.556308, 0.0, 0.558127, 0.0, 0.565576, 0.0, 0.571106, 0.0, 0.573039, 0.0, 0.574143, 0.0, 0.569627, 0.0, 0.562588, 0.0, 0.563137, 0.0, 0.565125, 0.0, 0.568553, 0.0, 0.571222, 0.0, 0.575603, 0.0, 0.581208, 0.0, 0.582388, 0.0, 0.576785, 0.0, 0.568649, 0.0, 0.563025, 0.0, 0.560796, 0.0, 0.558068, 0.0, 0.552758, 0.0, 0.547832, 0.0, 0.543907, 0.0, 0.535879, 0.0, 0.53272, 0.0, 0.531297, 0.0, 0.530536, 0.0, 0.529541, 0.0, 0.525468, 0.0, 0.520868, 0.0, 0.518469, 0.0, 0.515341, 0.0, 0.5123, 0.0, 0.506881, 0.0, 0.503807, 0.0, 0.500482, 0.0, 0.498008, 0.0]}
   images\val\car_rotate63_flip_horizontal.jpg: 2 annotations
      First annotation: {'class_id': 1, 'polygon': [0.509802, 0.0, 0.504396, 0.0, 0.497976, 0.0, 0.486488, 0.0, 0.477702, 0.0, 0.471113, 0.0, 0.466713, 0.0, 0.462517, 0.0, 0.458568, 0.0, 0.454314, 0.0, 0.449324, 0.0, 0.445484, 0.0, 0.443692, 0.0, 0.441873, 0.0, 0.434424, 0.0, 0.428894, 0.0, 0.426961, 0.0, 0.425857, 0.0, 0.430373, 0.0, 0.437412, 0.0, 0.436863, 0.0, 0.434875, 0.0, 0.431447, 0.0, 0.428778, 0.0, 0.424397, 0.0, 0.418792, 0.0, 0.417612, 0.0, 0.423215, 0.0, 0.431351, 0.0, 0.436975, 0.0, 0.439204, 0.0, 0.441932, 0.0, 0.447242, 0.0, 0.452168, 0.0, 0.456093, 0.0, 0.464121, 0.0, 0.46728, 0.0, 0.468703, 0.0, 0.469464, 0.0, 0.470459, 0.0, 0.474532, 0.0, 0.479132, 0.0, 0.481531, 0.0, 0.484659, 0.0, 0.4877, 0.0, 0.493119, 0.0, 0.496193, 0.0, 0.499518, 0.0, 0.501992, 0.0]}
   images\test\dog.jpg: 1 annotations
      First annotation: {'class_id': 2, 'polygon': [0.0, 0.049852, 0.0, 0.045556, 0.000211, 0.040519, 0.001336, 0.037111, 0.00218, 0.034593, 0.002227, 0.030444, 0.003352, 0.025111, 0.004477, 0.022889, 0.005883, 0.021259, 0.008273, 0.02037, 0.009539, 0.021111, 0.01282, 0.020519, 0.014086, 0.023037, 0.015586, 0.026593, 0.016945, 0.030741, 0.018164, 0.034, 0.018727, 0.037111, 0.018961, 0.042, 0.01943, 0.045259, 0.020367, 0.048815, 0.020695, 0.054, 0.020508, 0.057556, 0.019523, 0.062889, 0.018914, 0.065852, 0.019289, 0.070148, 0.019992, 0.072963, 0.020883, 0.076815, 0.021164, 0.078593, 0.02182, 0.076074, 0.02257, 0.071185, 0.022992, 0.070593, 0.023461, 0.072519, 0.023648, 0.07563, 0.023602, 0.078593, 0.022898, 0.082296, 0.022008, 0.084519, 0.022102, 0.089407, 0.021961, 0.092963, 0.022102, 0.096963, 0.022008, 0.101407, 0.021867, 0.103333, 0.004617, 0.103333, 0.004805, 0.09963, 0.004148, 0.097556, 0.00368, 0.092519, 0.003586, 0.088074, 0.003164, 0.083481, 0.00232, 0.078148, 0.001664, 0.071185, 0.001711, 0.065852, 0.001852, 0.063778, 0.001477, 0.060667, 0.001195, 0.057259, 0.000398, 0.053407]}
   images\test\dog_flip_horizontal.jpg: 1 annotations
      First annotation: {'class_id': 1, 'polygon': [1.0, 0.084997, 1.0, 0.077672, 0.99973, 0.069084, 0.99829, 0.063274, 0.99721, 0.05898, 0.99715, 0.051908, 0.99571, 0.042814, 0.99427, 0.039026, 0.99247, 0.036247, 0.98941, 0.034731, 0.98779, 0.035994, 0.98359, 0.034984, 0.98197, 0.039278, 0.98005, 0.04534, 0.97831, 0.052413, 0.97675, 0.05797, 0.97603, 0.063274, 0.97573, 0.07161, 0.97513, 0.077167, 0.97393, 0.083229, 0.97351, 0.09207, 0.97375, 0.098132, 0.97501, 0.107226, 0.97579, 0.112277, 0.97531, 0.119603, 0.97441, 0.124402, 0.97327, 0.130969, 0.97291, 0.134, 0.97207, 0.129706, 0.97111, 0.121371, 0.97057, 0.12036, 0.96997, 0.123644, 0.96973, 0.128949, 0.96979, 0.134, 0.97069, 0.140315, 0.97183, 0.144104, 0.97171, 0.15244, 0.97189, 0.158502, 0.97171, 0.165322, 0.97183, 0.1729, 0.97201, 0.176183, 0.99409, 0.176183, 0.99385, 0.169869, 0.99469, 0.166332, 0.99529, 0.157744, 0.99541, 0.150166, 0.99595, 0.142336, 0.99703, 0.133243, 0.99787, 0.121371, 0.99781, 0.112277, 0.99763, 0.108741, 0.99811, 0.103437, 0.99847, 0.097627, 0.99949, 0.09106]}
   images\test\dog_rotate-63.jpg: 1 annotations
      First annotation: {'class_id': 1, 'polygon': [0.0, 0.90677, 0.0, 0.903456, 0.0, 0.899249, 0.0, 0.894909, 0.0, 0.891682, 0.0, 0.88841, 0.0, 0.882584, 0.0, 0.879158, 0.0, 0.87576, 0.0, 0.871436, 0.0, 0.870081, 0.0, 0.86463, 0.0, 0.864646, 0.0, 0.865106, 0.0, 0.866237, 0.0, 0.866896, 0.0, 0.86844, 0.0, 0.871855, 0.002224, 0.873655, 0.006821, 0.874971, 0.012924, 0.878472, 0.016871, 0.8815, 0.022383, 0.887112, 0.025409, 0.890325, 0.030525, 0.893069, 0.034142, 0.89417, 0.039051, 0.895786, 0.041241, 0.896729, 0.038749, 0.893787, 0.033608, 0.888875, 0.033177, 0.887775, 0.035644, 0.888548, 0.039301, 0.890662, 0.042653, 0.893019, 0.046469, 0.896946, 0.048487, 0.900016, 0.054117, 0.903645, 0.05809, 0.906601, 0.062733, 0.909473, 0.067747, 0.913044, 0.069862, 0.914744, 0.059872, 0.940998, 0.055757, 0.937856, 0.053012, 0.937255, 0.046996, 0.934083, 0.041874, 0.930797, 0.036392, 0.927896, 0.029821, 0.925066, 0.021501, 0.920694, 0.015446, 0.916508, 0.013162, 0.914695, 0.009397, 0.912865, 0.005348, 0.910665, 0.000494, 0.908906]}
   images\test\dog_rotate-63_flip_horizontal.jpg: 1 annotations
      First annotation: {'class_id': 1, 'polygon': [1.0, 0.90677, 1.0, 0.903456, 1.0, 0.899249, 1.0, 0.894909, 1.0, 0.891682, 1.0, 0.88841, 1.0, 0.882584, 1.0, 0.879158, 1.0, 0.87576, 1.0, 0.871436, 1.0, 0.870081, 1.0, 0.86463, 1.0, 0.864646, 1.0, 0.865106, 1.0, 0.866237, 1.0, 0.866896, 1.0, 0.86844, 1.0, 0.871855, 0.997776, 0.873655, 0.993179, 0.874971, 0.987076, 0.878472, 0.983129, 0.8815, 0.977617, 0.887112, 0.974591, 0.890325, 0.969475, 0.893069, 0.965858, 0.89417, 0.960949, 0.895786, 0.958759, 0.896729, 0.961251, 0.893787, 0.966392, 0.888875, 0.966823, 0.887775, 0.964356, 0.888548, 0.960699, 0.890662, 0.957347, 0.893019, 0.953531, 0.896946, 0.951513, 0.900016, 0.945883, 0.903645, 0.94191, 0.906601, 0.937267, 0.909473, 0.932253, 0.913044, 0.930138, 0.914744, 0.940128, 0.940998, 0.944243, 0.937856, 0.946988, 0.937255, 0.953004, 0.934083, 0.958126, 0.930797, 0.963608, 0.927896, 0.970179, 0.925066, 0.978499, 0.920694, 0.984554, 0.916508, 0.986838, 0.914695, 0.990603, 0.912865, 0.994652, 0.910665, 0.999506, 0.908906]}
   images\test\dog_rotate63.jpg: 1 annotations
      First annotation: {'class_id': 1, 'polygon': [0.551356, 0.0, 0.556256, 0.0, 0.562122, 0.0, 0.566659, 0.0, 0.57002, 0.0, 0.574778, 0.0, 0.581511, 0.0, 0.584697, 0.0, 0.58737, 0.0, 0.589768, 0.0, 0.589656, 0.0, 0.592232, 0.0, 0.590093, 0.0, 0.586907, 0.0, 0.582964, 0.0, 0.579953, 0.0, 0.576731, 0.0, 0.571291, 0.0, 0.567846, 0.0, 0.564334, 0.0, 0.558611, 0.0, 0.554448, 0.0, 0.547795, 0.0, 0.544064, 0.0, 0.539381, 0.0, 0.536579, 0.0, 0.532702, 0.0, 0.530837, 0.0, 0.534089, 0.0, 0.540099, 0.0, 0.541019, 0.0, 0.539094, 0.0, 0.535655, 0.0, 0.532249, 0.0, 0.527618, 0.0, 0.524568, 0.0, 0.519047, 0.0, 0.514911, 0.0, 0.510431, 0.0, 0.505308, 0.0, 0.50303, 0.0, 0.493041, 0.0, 0.497373, 0.0, 0.499358, 0.0, 0.504831, 0.0, 0.509845, 0.0, 0.514838, 0.0, 0.520431, 0.0, 0.527992, 0.0, 0.534101, 0.0, 0.536548, 0.0, 0.539878, 0.0, 0.543601, 0.0, 0.547532, 0.0]}
   images\test\dog_rotate63_flip_horizontal.jpg: 1 annotations
      First annotation: {'class_id': 1, 'polygon': [0.448644, 0.0, 0.443744, 0.0, 0.437878, 0.0, 0.433341, 0.0, 0.42998, 0.0, 0.425222, 0.0, 0.418489, 0.0, 0.415303, 0.0, 0.41263, 0.0, 0.410232, 0.0, 0.410344, 0.0, 0.407768, 0.0, 0.409907, 0.0, 0.413093, 0.0, 0.417036, 0.0, 0.420047, 0.0, 0.423269, 0.0, 0.428709, 0.0, 0.432154, 0.0, 0.435666, 0.0, 0.441389, 0.0, 0.445552, 0.0, 0.452205, 0.0, 0.455936, 0.0, 0.460619, 0.0, 0.463421, 0.0, 0.467298, 0.0, 0.469163, 0.0, 0.465911, 0.0, 0.459901, 0.0, 0.458981, 0.0, 0.460906, 0.0, 0.464345, 0.0, 0.467751, 0.0, 0.472382, 0.0, 0.475432, 0.0, 0.480953, 0.0, 0.485089, 0.0, 0.489569, 0.0, 0.494692, 0.0, 0.49697, 0.0, 0.506959, 0.0, 0.502627, 0.0, 0.500642, 0.0, 0.495169, 0.0, 0.490155, 0.0, 0.485162, 0.0, 0.479569, 0.0, 0.472008, 0.0, 0.465899, 0.0, 0.463452, 0.0, 0.460122, 0.0, 0.456399, 0.0, 0.452468, 0.0]}