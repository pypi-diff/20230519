# Comparing `tmp/visionai-data-format-1.0.2.tar.gz` & `tmp/visionai-data-format-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-data-format-1.0.2.tar", last modified: Thu May 18 04:05:31 2023, max compression
+gzip compressed data, was "visionai-data-format-1.0.3.tar", last modified: Fri May 19 03:53:54 2023, max compression
```

## Comparing `visionai-data-format-1.0.2.tar` & `visionai-data-format-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.398867 visionai-data-format-1.0.2/
--rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-18 04:05:31.398720 visionai-data-format-1.0.2/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)       69 2023-05-12 07:07:09.000000 visionai-data-format-1.0.2/README.md
--rw-r--r--   0 christian   (501) staff       (20)       38 2023-05-18 04:05:31.399041 visionai-data-format-1.0.2/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)      577 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/setup.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.386900 visionai-data-format-1.0.2/tests/
--rw-r--r--   0 christian   (501) staff       (20)     2176 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/tests/test_schemas.py
--rw-r--r--   0 christian   (501) staff       (20)     4731 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/tests/test_validators.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.389034 visionai-data-format-1.0.2/visionai_data_format/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     1400 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/bdd_to_vai.py
--rw-r--r--   0 christian   (501) staff       (20)     7696 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/coco_to_vai.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.394590 visionai-data-format-1.0.2/visionai_data_format/schemas/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     2551 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 christian   (501) staff       (20)     1657 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/common.py
--rw-r--r--   0 christian   (501) staff       (20)      994 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/ontology.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.394933 visionai-data-format-1.0.2/visionai_data_format/schemas/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)    39355 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/utils/validators.py
--rw-r--r--   0 christian   (501) staff       (20)    27992 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.397991 visionai-data-format-1.0.2/visionai_data_format/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)      494 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/utils/calculation.py
--rw-r--r--   0 christian   (501) staff       (20)    10506 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/checker.py
--rw-r--r--   0 christian   (501) staff       (20)      761 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/classes.py
--rw-r--r--   0 christian   (501) staff       (20)      335 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/common.py
--rw-r--r--   0 christian   (501) staff       (20)     6877 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/converter.py
--rw-r--r--   0 christian   (501) staff       (20)     4059 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/resize.py
--rw-r--r--   0 christian   (501) staff       (20)     1991 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/utils/validator.py
--rw-r--r--   0 christian   (501) staff       (20)     2274 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 christian   (501) staff       (20)     6237 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/vai_to_coco.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.392839 visionai-data-format-1.0.2/visionai_data_format.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-18 04:05:31.000000 visionai-data-format-1.0.2/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     1122 2023-05-18 04:05:31.000000 visionai-data-format-1.0.2/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2023-05-18 04:05:31.000000 visionai-data-format-1.0.2/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       40 2023-05-18 04:05:31.000000 visionai-data-format-1.0.2/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 christian   (501) staff       (20)       21 2023-05-18 04:05:31.000000 visionai-data-format-1.0.2/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-19 03:53:54.983232 visionai-data-format-1.0.3/
+-rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-19 03:53:54.982615 visionai-data-format-1.0.3/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)       69 2023-05-12 07:07:09.000000 visionai-data-format-1.0.3/README.md
+-rw-r--r--   0 christian   (501) staff       (20)       38 2023-05-19 03:53:54.983292 visionai-data-format-1.0.3/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)      577 2023-05-19 03:23:30.000000 visionai-data-format-1.0.3/setup.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-19 03:53:54.976587 visionai-data-format-1.0.3/tests/
+-rw-r--r--   0 christian   (501) staff       (20)     2176 2023-05-18 02:48:45.000000 visionai-data-format-1.0.3/tests/test_schemas.py
+-rw-r--r--   0 christian   (501) staff       (20)     4731 2023-05-18 02:48:45.000000 visionai-data-format-1.0.3/tests/test_validators.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-19 03:53:54.977909 visionai-data-format-1.0.3/visionai_data_format/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     1400 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/bdd_to_vai.py
+-rw-r--r--   0 christian   (501) staff       (20)     7775 2023-05-19 03:23:30.000000 visionai-data-format-1.0.3/visionai_data_format/coco_to_vai.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-19 03:53:54.980481 visionai-data-format-1.0.3/visionai_data_format/schemas/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     2551 2023-05-18 02:48:45.000000 visionai-data-format-1.0.3/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)     1657 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/schemas/common.py
+-rw-r--r--   0 christian   (501) staff       (20)      994 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-19 03:53:54.980869 visionai-data-format-1.0.3/visionai_data_format/schemas/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)    39355 2023-05-18 02:48:45.000000 visionai-data-format-1.0.3/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 christian   (501) staff       (20)    27992 2023-05-18 02:48:45.000000 visionai-data-format-1.0.3/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-19 03:53:54.982383 visionai-data-format-1.0.3/visionai_data_format/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)      494 2023-05-18 02:48:45.000000 visionai-data-format-1.0.3/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 christian   (501) staff       (20)    10506 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/utils/checker.py
+-rw-r--r--   0 christian   (501) staff       (20)      761 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/utils/classes.py
+-rw-r--r--   0 christian   (501) staff       (20)      335 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/utils/common.py
+-rw-r--r--   0 christian   (501) staff       (20)     6927 2023-05-19 03:23:30.000000 visionai-data-format-1.0.3/visionai_data_format/utils/converter.py
+-rw-r--r--   0 christian   (501) staff       (20)     4059 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/utils/resize.py
+-rw-r--r--   0 christian   (501) staff       (20)     1991 2023-05-18 02:48:45.000000 visionai-data-format-1.0.3/visionai_data_format/utils/validator.py
+-rw-r--r--   0 christian   (501) staff       (20)     2274 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 christian   (501) staff       (20)     6237 2023-05-18 02:48:43.000000 visionai-data-format-1.0.3/visionai_data_format/vai_to_coco.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-19 03:53:54.979489 visionai-data-format-1.0.3/visionai_data_format.egg-info/
+-rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-19 03:53:54.000000 visionai-data-format-1.0.3/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     1122 2023-05-19 03:53:54.000000 visionai-data-format-1.0.3/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2023-05-19 03:53:54.000000 visionai-data-format-1.0.3/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (501) staff       (20)       40 2023-05-19 03:53:54.000000 visionai-data-format-1.0.3/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 christian   (501) staff       (20)       21 2023-05-19 03:53:54.000000 visionai-data-format-1.0.3/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai-data-format-1.0.2/setup.py` & `visionai-data-format-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "visionai-data-format"
-PACKAGE_VERSION = "1.0.2"
+PACKAGE_VERSION = "1.0.3"
 DESC = "converter tool for visionai format"
 REQUIRED = ["pydantic"]
 REQUIRES_PYTHON = ">=3.7, <4"
 EXTRAS = {
     "test": [
         "pytest",
         "mock",
```

### Comparing `visionai-data-format-1.0.2/tests/test_schemas.py` & `visionai-data-format-1.0.3/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/tests/test_validators.py` & `visionai-data-format-1.0.3/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/bdd_to_vai.py` & `visionai-data-format-1.0.3/visionai_data_format/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/coco_to_vai.py` & `visionai-data-format-1.0.3/visionai_data_format/coco_to_vai.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
                             val=bbox,
                             stream=sensor_name,
                         )
                     ]
                 )
             )
         }
+
         frames[image_name].objects.update(objects_under_frames)
 
         # to vision_ai: objects
         object_under_objects = {
             object_id: Object(
                 name=class_id_name_dict[str(anno["category_id"])],
                 type=class_id_name_dict[str(anno["category_id"])],
@@ -156,16 +157,17 @@
             uri=uri,
             type=StreamType.camera,
             description="Frontal camera",
         )
     }
     # to vision_ai:
     for image_name, frame_obj in frames.items():
+        current_frame_objects = getattr(frame_obj, "objects", None) or {}
         objects_per_image = {
-            object_id: objects[object_id] for object_id in frame_obj.objects
+            object_id: objects[object_id] for object_id in current_frame_objects
         }
 
         new_image_name = f"{int(image_name):012d}"
         vision_ai_data_dict[new_image_name] = VisionAIModel(
             visionai=VisionAI(
                 frame_intervals=[
                     FrameInterval(frame_start=frame_num, frame_end=frame_num)
```

### Comparing `visionai-data-format-1.0.2/visionai_data_format/schemas/bdd_schema.py` & `visionai-data-format-1.0.3/visionai_data_format/schemas/bdd_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/schemas/coco_schema.py` & `visionai-data-format-1.0.3/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/schemas/common.py` & `visionai-data-format-1.0.3/visionai_data_format/schemas/common.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/schemas/ontology.py` & `visionai-data-format-1.0.3/visionai_data_format/schemas/ontology.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/schemas/utils/validators.py` & `visionai-data-format-1.0.3/visionai_data_format/schemas/utils/validators.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/schemas/visionai_schema.py` & `visionai-data-format-1.0.3/visionai_data_format/schemas/visionai_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/utils/checker.py` & `visionai-data-format-1.0.3/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/utils/classes.py` & `visionai-data-format-1.0.3/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/utils/converter.py` & `visionai-data-format-1.0.3/visionai_data_format/utils/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,16 @@
     cur_data["dataset"] = container_name
 
     frame_list = list()
     for frame_key, frame_data in vai_data.frames.items():
         cur_data["name"] = frame_key + ".jpg"
         labels = []
         idx = 0
-        for obj_id, obj_data in frame_data.objects.items():
+        objects = getattr(frame_data, "objects", None) or {}
+        for obj_id, obj_data in objects.items():
             classes = vai_data.objects.get(obj_id).type
             bboxes = obj_data.object_data.bbox or [] if obj_data.object_data else []
             for bbox in bboxes:
                 geometry = bbox.val
 
                 label = dict()
                 label["category"] = classes
```

### Comparing `visionai-data-format-1.0.2/visionai_data_format/utils/resize.py` & `visionai-data-format-1.0.3/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/utils/validator.py` & `visionai-data-format-1.0.3/visionai_data_format/utils/validator.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/vai_to_bdd.py` & `visionai-data-format-1.0.3/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format/vai_to_coco.py` & `visionai-data-format-1.0.3/visionai_data_format/vai_to_coco.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.2/visionai_data_format.egg-info/SOURCES.txt` & `visionai-data-format-1.0.3/visionai_data_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

