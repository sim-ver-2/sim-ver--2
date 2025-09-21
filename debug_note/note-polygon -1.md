 'app.frontend.ui', 'app.frontend.navigation', 'app.frontend.validation']

=== 🔍 TRANSFORMATIONS DEBUG :: cat.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 400, 'height': 400}}, {'type': 'rotate', 'params': {'angle': 21.9}}]
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
   Task type: segmentation
   Export format: yolo_segmentation
   ✅ Using SEGMENTATION mode: yolo_segmentation
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 3
   Final dims: 400x400
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 400x400

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
         📦 Input bbox: x_min=0.0, y_min=22.480000000000004, x_max=67.25999999999999, y_max=109.36       
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 77 points...
         🔧 _transform_polygon returned: Polygon(points=[(0.0, 70.88000000000001), (0.0, 68.42666666666668), (0.0, 63.2), (0.0, 61.38666666666667), (0.0, 60.959999999999994), (0.0, 54.13333333333334), (0.8699999999999961, 47.413333333333334), (1.8299999999999963, 42.720000000000006), (2.849999999999996, 36.64), (3.2699999999999956, 33.440000000000005), (3.4499999999999957, 30.133333333333333), (3.389999999999996, 26.720000000000002), (2.9699999999999944, 22.560000000000002), (2.6699999999999955, 17.119999999999997), (3.0899999999999954, 14.986666666666668), (4.349999999999996, 16.586666666666666), (6.689999999999994, 18.93333333333333), (8.549999999999997, 22.24), (10.049999999999997, 22.77333333333333), (12.629999999999995, 22.77333333333333), (15.089999999999996, 22.560000000000002), (16.949999999999996, 21.386666666666663), (19.049999999999997, 17.546666666666667), (21.689999999999998, 17.013333333333335), (21.629999999999995, 19.893333333333334), (20.789999999999996, 23.62666666666667), (20.249999999999996, 28.10666666666667), (20.009999999999998, 32.160000000000004), (20.129999999999995, 35.36), (20.009999999999998, 39.2), (19.709999999999994, 44.0), (20.789999999999996, 45.38666666666667), (22.409999999999997, 46.34666666666667), (23.849999999999994, 48.693333333333335), (25.589999999999996, 50.29333333333333), (24.929999999999996, 52.85333333333333), (22.709999999999997, 50.61333333333333), (21.209999999999997, 48.373333333333335), (20.669999999999998, 48.160000000000004), (22.589999999999996, 51.04), (23.49, 53.17333333333333), (23.61, 55.413333333333334), (22.409999999999997, 55.94666666666667), (21.809999999999995, 53.6), (21.029999999999998, 52.32), (20.069999999999997, 50.720000000000006), (19.769999999999996, 50.29333333333333), (20.069999999999997, 53.17333333333333), (21.029999999999998, 54.34666666666667), (23.13, 55.2), (24.629999999999995, 54.666666666666664), (26.07, 54.986666666666665), (28.049999999999997, 56.58666666666667), (33.14999999999999, 60.00000000000001), (33.629999999999995, 61.28), (33.269999999999996, 62.34666666666667), (30.509999999999998, 62.239999999999995), (28.289999999999992, 62.34666666666667), (24.75, 62.45333333333333), (24.09, 62.45333333333333), (24.03, 64.69333333333334), (23.669999999999995, 67.35999999999999), (22.409999999999997, 69.06666666666668), (20.49, 70.24000000000001), (18.749999999999996, 68.96000000000001), (17.969999999999995, 66.4), (17.489999999999995, 64.26666666666667), (17.249999999999993, 62.77333333333334), (14.909999999999997, 62.56), (10.709999999999996, 63.09333333333334), (6.5099999999999945, 62.77333333333334), (5.369999999999996, 62.77333333333334), (5.669999999999995, 65.97333333333333), (5.369999999999996, 69.17333333333332), (3.929999999999995, 70.88000000000001), (2.069999999999996, 72.90666666666667), (0.8099999999999947, 72.37333333333333)], class_name='cat', class_id=12, confidence=1.0)
         📦 Updated bounding box: x_min=0.0, y_min=14.986666666666668, x_max=33.629999999999995, y_max=72.90666666666667
         📦 Updated annotation with 77 transformed points
   🔄 Processing annotation 2/3: cat eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat eye
         📦 Input bbox: x_min=14.09999999999999, y_min=48.720000000000006, x_max=20.69999999999999, y_max=56.72
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 8 points...
         🔧 _transform_polygon returned: Polygon(points=[(8.909999999999998, 37.81333333333333), (7.589999999999995, 36.64), (7.049999999999995, 34.72), (7.169999999999998, 32.906666666666666), (8.969999999999995, 32.480000000000004), (9.989999999999995, 33.440000000000005), (10.349999999999994, 35.04), (9.989999999999995, 36.64)], class_name='cat eye', class_id=16, confidence=1.0)
         📦 Updated bounding box: x_min=7.049999999999995, y_min=32.480000000000004, x_max=10.349999999999994, y_max=37.81333333333333
         📦 Updated annotation with 8 transformed points
   🔄 Processing annotation 3/3: cat eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: cat eye
         📦 Input bbox: x_min=27.539999999999996, y_min=48.24000000000001, x_max=34.019999999999996, y_max=56.239999999999995
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 6 points...
         🔧 _transform_polygon returned: Polygon(points=[(13.769999999999998, 36.53333333333334), (13.949999999999994, 33.86666666666666), (15.449999999999998, 32.160000000000004), (16.65, 33.120000000000005), (17.009999999999998, 35.67999999999999), (16.109999999999996, 37.493333333333325)], class_name='cat eye', class_id=16, confidence=1.0)
         📦 Updated bounding box: x_min=13.769999999999998, y_min=32.160000000000004, x_max=17.009999999999998, y_max=37.493333333333325
         📦 Updated annotation with 6 transformed points
   Original: 3 → Transformed: 3
✅ NEW SEGMENTATION FUNCTION RESULT: 3 lines

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 21.9}}, {'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 21.9}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}   
🔍 DEBUG: About to transform 3 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 14.986666666666668, 33.629999999999995, 72.90666666666667)

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -21.9}}, {'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -21.9}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 3 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 14.986666666666668, 33.629999999999995, 72.90666666666667)

=== 🔍 TRANSFORMATIONS DEBUG :: car.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 400, 'height': 400}}, {'type': 'rotate', 'params': {'angle': 21.9}}]
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
   Task type: segmentation
   Export format: yolo_segmentation
   ✅ Using SEGMENTATION mode: yolo_segmentation
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 2
   Final dims: 400x400
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 400x400

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
         📦 Input bbox: x_min=0.0, y_min=33.36, x_max=47.33999999999999, y_max=111.76000000000002        
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 49 points...
         🔧 _transform_polygon returned: Polygon(points=[(0.0, 74.50666666666667), (0.0, 71.09333333333333), (0.0, 67.03999999999999), (0.0, 59.78666666666667), (0.0, 54.239999999999995), (0.0, 50.08), (0.389999999999995, 47.413333333333334), (0.32999999999999563, 44.74666666666667), (1.5899999999999948, 42.61333333333333), (3.149999999999995, 40.373333333333335), (4.469999999999995, 37.6), (5.489999999999995, 35.46666666666667), (6.089999999999996, 34.50666666666667), (6.7499999999999964, 33.54666666666667), (7.529999999999994, 29.06666666666667), (8.549999999999997, 25.866666666666664), (9.089999999999995, 24.8), (10.409999999999997, 24.479999999999997), (12.749999999999995, 28.000000000000004), (14.369999999999996, 32.906666666666666), (15.209999999999996, 32.8), (15.869999999999994, 31.733333333333334), (16.349999999999998, 29.706666666666667), (16.65, 28.10666666666667), (17.369999999999997, 25.546666666666667), (18.929999999999996, 22.453333333333333), (20.789999999999996, 22.24), (20.729999999999997, 25.759999999999998), (20.669999999999998, 30.880000000000003), (20.189999999999998, 34.29333333333334), (20.49, 35.78666666666667), (21.93, 37.92), (22.889999999999997, 41.54666666666667), (22.829999999999995, 44.64), (23.49, 47.30666666666667), (23.669999999999995, 52.42666666666666), (22.289999999999996, 54.02666666666667), (19.889999999999997, 54.239999999999995), (18.209999999999997, 54.239999999999995), (17.129999999999995, 54.56), (14.849999999999994, 56.48), (15.509999999999994, 59.57333333333334), (15.809999999999997, 61.17333333333333), (15.989999999999998, 63.2), (15.989999999999998, 65.12), (16.709999999999997, 68.74666666666667), (17.009999999999998, 70.77333333333334), (17.129999999999995, 72.90666666666667), (16.889999999999997, 74.4)], class_name='dog', class_id=1, confidence=1.0)
         📦 Updated bounding box: x_min=0.0, y_min=22.24, x_max=23.669999999999995, y_max=74.50666666666667
         📦 Updated annotation with 49 transformed points
   🔄 Processing annotation 2/2: dog eye
      🎯 _TRANSFORM_SINGLE_ANNOTATION called
         📦 Annotation type: Annotation
         📦 Annotation full type: <class 'database.models.Annotation'>
         📦 Class: dog eye
         📦 Input bbox: x_min=30.539999999999992, y_min=62.16000000000001, x_max=36.29999999999999, y_max=67.92
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 7 points...
         🔧 _transform_polygon returned: Polygon(points=[(15.269999999999996, 43.67999999999999), (15.389999999999995, 42.720000000000006), (16.589999999999996, 41.440000000000005), (18.089999999999996, 42.08), (18.149999999999995, 43.46666666666667), (17.549999999999997, 45.28), (16.109999999999996, 45.28)], class_name='dog eye', class_id=15, confidence=1.0)
         📦 Updated bounding box: x_min=15.269999999999996, y_min=41.440000000000005, x_max=18.149999999999995, y_max=45.28
         📦 Updated annotation with 7 transformed points
   Original: 2 → Transformed: 2
✅ NEW SEGMENTATION FUNCTION RESULT: 2 lines

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']
INFO:     127.0.0.1:50941 - "POST /api/v1/logs/frontend/batch HTTP/1.1" 200 OK

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 21.9}}, {'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 21.9}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}   
🔍 DEBUG: About to transform 2 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 22.24, 23.669999999999995, 74.50666666666667)

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -21.9}}, {'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -21.9}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 2 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 22.24, 23.669999999999995, 74.50666666666667)

=== 🔍 TRANSFORMATIONS DEBUG :: dog.jpg ===
transformations variable: [{'type': 'resize', 'params': {'width': 400, 'height': 400}}, {'type': 'rotate', 'params': {'angle': 21.9}}]
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
   Task type: segmentation
   Export format: yolo_segmentation
   ✅ Using SEGMENTATION mode: yolo_segmentation
🎯 RELEASES.PY: Using NEW FUNCTIONS with internal transformation!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['resize'], 'geometric_transforms_order': ['resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 0}], 'photometric_transforms': [], 'total_transforms': 1, 'geometric_count': 1, 'photometric_count': 0}
🎯 NEW SEGMENTATION FUNCTION CALLED!
   Annotations: 1
   Final dims: 400x400
   Has transform_config: True
   Original dims: (800, 600)
🔧 TRANSFORMING ANNOTATIONS: (800, 600) → 400x400

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
         📦 Input bbox: x_min=0.0, y_min=22.0, x_max=60.54, y_max=111.60000000000001
         📐 Dimensions: (800, 600) → (400, 400)
         🔍 isinstance(annotation, BoundingBox): False
         🔍 BoundingBox type: <class 'core.annotation_transformer.BoundingBox'>
         🔧 Detected database annotation - label_mode: yolo_segmentation
         🔧 Using segmentation data for segmentation task...
         🔧 About to call _transform_polygon with 54 points...
         🔧 _transform_polygon returned: Polygon(points=[(0.0, 35.89333333333333), (0.0, 32.8), (0.26999999999999624, 29.173333333333336), (1.7099999999999955, 26.720000000000002), (2.7899999999999965, 24.90666666666667), (2.849999999999996, 21.92), (4.289999999999996, 18.080000000000002), (5.729999999999997, 16.479999999999997), (7.529999999999994, 15.306666666666667), (10.589999999999996, 14.666666666666666), (12.209999999999997, 15.2), (16.409999999999997, 14.773333333333333), (18.029999999999998, 16.586666666666666), (19.949999999999996, 19.14666666666667), (21.689999999999998, 22.133333333333333), (23.249999999999996, 24.479999999999997), (23.97, 26.720000000000002), (24.269999999999996, 30.24), (24.869999999999994, 32.58666666666666), (26.07, 35.14666666666666), (26.490000000000002, 38.88), (26.249999999999993, 41.440000000000005), (24.99, 45.28), (24.209999999999994, 47.413333333333334), (24.689999999999998, 50.50666666666667), (25.589999999999996, 52.53333333333334), (26.729999999999997, 55.30666666666667), (27.089999999999996, 56.58666666666667), (27.929999999999993, 54.773333333333326), (28.89, 51.25333333333334), (29.429999999999996, 50.82666666666667), (30.029999999999994, 52.21333333333334), (30.27, 54.45333333333333), (30.209999999999997, 56.58666666666667), (29.309999999999995, 59.25333333333334), (28.169999999999998, 60.85333333333333), (28.289999999999992, 64.37333333333333), (28.11, 66.93333333333334), (28.289999999999992, 69.81333333333333), (28.169999999999998, 73.01333333333334), (27.989999999999995, 74.4), (5.909999999999997, 74.4), (6.149999999999994, 71.73333333333332), (5.309999999999997, 70.24000000000001), (4.709999999999995, 66.61333333333334), (4.589999999999996, 63.413333333333334), (4.049999999999995, 60.10666666666666), (2.9699999999999944, 56.266666666666666), (2.1299999999999955, 51.25333333333334), (2.1899999999999946, 47.413333333333334), (2.3699999999999948, 45.919999999999995), (1.8899999999999957, 43.67999999999999), (1.5299999999999954, 41.22666666666667), (0.5099999999999958, 38.45333333333333)], class_name='dog', class_id=1, confidence=1.0)
         📦 Updated bounding box: x_min=0.0, y_min=14.666666666666666, x_max=30.27, y_max=74.4
         📦 Updated annotation with 54 transformed points
   Original: 1 → Transformed: 1
✅ NEW SEGMENTATION FUNCTION RESULT: 1 lines

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': 21.9}}, {'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': 21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': 21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': 21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': 21.9}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': 21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': 21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}   
🔍 DEBUG: About to transform 1 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 14.666666666666666, 30.27, 74.4)

🖼️ IMAGE GENERATION ORDER: ['rotate', 'resize']

🔍 TRACKING FUNCTION INPUT:
   Transformations: [{'type': 'rotate', 'params': {'angle': -21.9}}, {'type': 'resize', 'params': {'width': 400, 'height': 400}}]
   Original dims: (800, 600)
   Final dims: (400, 400)
🎯 RESIZE CONFIG ALREADY EXISTS: {'enabled': True, 'width': 400, 'height': 400}

📍 ANNOTATION TRACKING ORDER: ['rotate', 'resize']
🔧 GEOMETRIC TRANSFORMS ORDER: ['rotate', 'resize']
🔍 TRANSFORMATION CONFIG DETAILS: {'rotate': {'enabled': True, 'angle': -21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}

🎯 TRACKING FUNCTION OUTPUT:
   transformation_config: {'rotate': {'enabled': True, 'angle': -21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}
   Has geometric transforms: True
   Geometric transforms: [{'type': 'rotate', 'params': {'angle': -21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}]
🎯 RELEASES.PY: Using ADVANCED transformation system for annotations!
   📊 Tracking data: {'transformation_sequence': [{'index': 0, 'type': 'rotate', 'params': {'angle': -21.9}, 'is_geometric': True, 'is_photometric': False}, {'index': 1, 'type': 'resize', 'params': {'width': 400, 'height': 400}, 'is_geometric': True, 'is_photometric': False}], 'transformation_config': {'rotate': {'enabled': True, 'angle': -21.9}, 'resize': {'enabled': True, 'width': 400, 'height': 400}}, 'original_dims': (800, 600), 'final_dims': (400, 400), 'debug_transformation_order': {'annotation_config_order': ['rotate', 'resize'], 'geometric_transforms_order': ['rotate', 'resize'], 'orders_match': True, 'duplicate_resize_detected': False}, 'has_geometric_transforms': True, 'geometric_transforms': [{'type': 'rotate', 'params': {'angle': -21.9}, 'index': 0}, {'type': 'resize', 'params': {'width': 400, 'height': 400}, 'index': 1}], 'photometric_transforms': [], 'total_transforms': 2, 'geometric_count': 2, 'photometric_count': 0}
🔍 DEBUG: About to transform 1 annotations
   First annotation type: <class 'database.models.Annotation'>
   First annotation attrs: ['class_id', 'class_name', 'confidence', 'created_at', 'id', 'image', 'image_id', 'is_auto_generated', 'is_verified', 'metadata', 'model_id', 'registry', 'segmentation', 'updated_at', 'x_max', 'x_min', 'y_max', 'y_min']
   First annotation coords: (0.0, 14.666666666666666, 30.27, 74.4)

=== 📋 WRITING ANNOTATIONS.JSON ===
Total images with annotations: 9
   images\train\cat.jpg: 3 annotations
      First annotation: {'class_id': 0, 'polygon': [0.0, 0.1772, 0.0, 0.171067, 0.0, 0.158, 0.0, 0.153467, 0.0, 0.1524, 0.0, 0.135333, 0.002175, 0.118533, 0.004575, 0.1068, 0.007125, 0.0916, 0.008175, 0.0836, 0.008625, 0.075333, 0.008475, 0.0668, 0.007425, 0.0564, 0.006675, 0.0428, 0.007725, 0.037467, 0.010875, 0.041467, 0.016725, 0.047333, 0.021375, 0.0556, 0.025125, 0.056933, 0.031575, 0.056933, 0.037725, 0.0564, 0.042375, 0.053467, 0.047625, 0.043867, 0.054225, 0.042533, 0.054075, 0.049733, 0.051975, 0.059067, 0.050625, 0.070267, 0.050025, 0.0804, 0.050325, 0.0884, 0.050025, 0.098, 0.049275, 0.11, 0.051975, 0.113467, 0.056025, 0.115867, 0.059625, 0.121733, 0.063975, 0.125733, 0.062325, 0.132133, 0.056775, 0.126533, 0.053025, 0.120933, 0.051675, 0.1204, 0.056475, 0.1276, 0.058725, 0.132933, 0.059025, 0.138533, 0.056025, 0.139867, 0.054525, 0.134, 0.052575, 0.1308, 0.050175, 0.1268, 0.049425, 0.125733, 0.050175, 0.132933, 0.052575, 0.135867, 0.057825, 0.138, 0.061575, 0.136667, 0.065175, 0.137467, 0.070125, 0.141467, 0.082875, 0.15, 0.084075, 0.1532, 0.083175, 0.155867, 0.076275, 0.1556, 0.070725, 0.155867, 0.061875, 0.156133, 0.060225, 0.156133, 0.060075, 0.161733, 0.059175, 0.1684, 0.056025, 0.172667, 0.051225, 0.1756, 0.046875, 0.1724, 0.044925, 0.166, 0.043725, 0.160667, 0.043125, 0.156933, 0.037275, 0.1564, 0.026775, 0.157733, 0.016275, 0.156933, 0.013425, 0.156933, 0.014175, 0.164933, 0.013425, 0.172933, 0.009825, 0.1772, 0.005175, 0.182267, 0.002025, 0.180933]}
   images\train\cat_rotate-21.jpg: 0 annotations
   images\train\cat_rotate21.jpg: 0 annotations
   images\val\car.jpg: 2 annotations
      First annotation: {'class_id': 2, 'polygon': [0.0, 0.186267, 0.0, 0.177733, 0.0, 0.1676, 0.0, 0.149467, 0.0, 0.1356, 0.0, 0.1252, 0.000975, 0.118533, 0.000825, 0.111867, 0.003975, 0.106533, 0.007875, 0.100933, 0.011175, 0.094, 0.013725, 0.088667, 0.015225, 0.086267, 0.016875, 0.083867, 0.018825, 0.072667, 0.021375, 0.064667, 0.022725, 0.062, 0.026025, 0.0612, 0.031875, 0.07, 0.035925, 0.082267, 0.038025, 0.082, 0.039675, 0.079333, 0.040875, 0.074267, 0.041625, 0.070267, 0.043425, 0.063867, 0.047325, 0.056133, 0.051975, 0.0556, 0.051825, 0.0644, 0.051675, 0.0772, 0.050475, 0.085733, 0.051225, 0.089467, 0.054825, 0.0948, 0.057225, 0.103867, 0.057075, 0.1116, 0.058725, 0.118267, 0.059175, 0.131067, 0.055725, 0.135067, 0.049725, 0.1356, 0.045525, 0.1356, 0.042825, 0.1364, 0.037125, 0.1412, 0.038775, 0.148933, 0.039525, 0.152933, 0.039975, 0.158, 0.039975, 0.1628, 0.041775, 0.171867, 0.042525, 0.176933, 0.042825, 0.182267, 0.042225, 0.186]}
   images\val\car_rotate-21.jpg: 0 annotations
   images\val\car_rotate21.jpg: 0 annotations
   images\test\dog.jpg: 1 annotations
      First annotation: {'class_id': 2, 'polygon': [0.0, 0.089733, 0.0, 0.082, 0.000675, 0.072933, 0.004275, 0.0668, 0.006975, 0.062267, 0.007125, 0.0548, 0.010725, 0.0452, 0.014325, 0.0412, 0.018825, 0.038267, 0.026475, 0.036667, 0.030525, 0.038, 0.041025, 0.036933, 0.045075, 0.041467, 0.049875, 0.047867, 0.054225, 0.055333, 0.058125, 0.0612, 0.059925, 0.0668, 0.060675, 0.0756, 0.062175, 0.081467, 0.065175, 0.087867, 0.066225, 0.0972, 0.065625, 0.1036, 0.062475, 0.1132, 0.060525, 0.118533, 0.061725, 0.126267, 0.063975, 0.131333, 0.066825, 0.138267, 0.067725, 0.141467, 0.069825, 0.136933, 0.072225, 0.128133, 0.073575, 0.127067, 0.075075, 0.130533, 0.075675, 0.136133, 0.075525, 0.141467, 0.073275, 0.148133, 0.070425, 0.152133, 0.070725, 0.160933, 0.070275, 0.167333, 0.070725, 0.174533, 0.070425, 0.182533, 0.069975, 0.186, 0.014775, 0.186, 0.015375, 0.179333, 0.013275, 0.1756, 0.011775, 0.166533, 0.011475, 0.158533, 0.010125, 0.150267, 0.007425, 0.140667, 0.005325, 0.128133, 0.005475, 0.118533, 0.005925, 0.1148, 0.004725, 0.1092, 0.003825, 0.103067, 0.001275, 0.096133]}
   images\test\dog_rotate-21.jpg: 0 annotations
   images\test\dog_rotate21.jpg: 0 annotations
INFO:     127.0.0.1:58546 - "POST /api/v1/releases/create HTTP/1.1" 200 OK
INFO:     127.0.0.1:50941 - "OPTIONS /api/transformation/available-transformations?_t=1758452157238 HTTP/1.1" 200 OK