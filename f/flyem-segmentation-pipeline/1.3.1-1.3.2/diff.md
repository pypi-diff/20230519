# Comparing `tmp/flyem_segmentation_pipeline-1.3.1.tar.gz` & `tmp/flyem_segmentation_pipeline-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyem_segmentation_pipeline-1.3.1.tar", last modified: Fri May 19 17:37:17 2023, max compression
+gzip compressed data, was "flyem_segmentation_pipeline-1.3.2.tar", last modified: Fri May 19 17:45:00 2023, max compression
```

## Comparing `flyem_segmentation_pipeline-1.3.1.tar` & `flyem_segmentation_pipeline-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:37:17.408857 flyem_segmentation_pipeline-1.3.1/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5033 2023-05-19 17:37:17.408929 flyem_segmentation_pipeline-1.3.1/PKG-INFO
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     4364 2023-05-19 17:35:55.000000 flyem_segmentation_pipeline-1.3.1/README.md
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      107 2023-05-19 17:37:17.409142 flyem_segmentation_pipeline-1.3.1/setup.cfg
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1050 2023-05-19 17:37:14.000000 flyem_segmentation_pipeline-1.3.1/setup.py
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:37:17.406939 flyem_segmentation_pipeline-1.3.1/src/
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:37:17.408004 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5033 2023-05-19 17:37:17.000000 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      495 2023-05-19 17:37:17.000000 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)        1 2023-05-19 17:37:17.000000 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       24 2023-05-19 17:37:17.000000 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/requires.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       34 2023-05-19 17:37:17.000000 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:37:17.408500 flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      112 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/__init__.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1228 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/controller.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1256 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/model.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      152 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/view.py
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:37:17.408744 flyem_segmentation_pipeline-1.3.1/src/segmentationUtils/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       43 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationUtils/__init__.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5528 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationUtils/imageUtils.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:45:00.111485 flyem_segmentation_pipeline-1.3.2/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5092 2023-05-19 17:45:00.111539 flyem_segmentation_pipeline-1.3.2/PKG-INFO
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     4423 2023-05-19 17:44:19.000000 flyem_segmentation_pipeline-1.3.2/README.md
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      107 2023-05-19 17:45:00.111749 flyem_segmentation_pipeline-1.3.2/setup.cfg
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1050 2023-05-19 17:44:57.000000 flyem_segmentation_pipeline-1.3.2/setup.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:45:00.109734 flyem_segmentation_pipeline-1.3.2/src/
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:45:00.110715 flyem_segmentation_pipeline-1.3.2/src/flyem_segmentation_pipeline.egg-info/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5092 2023-05-19 17:45:00.000000 flyem_segmentation_pipeline-1.3.2/src/flyem_segmentation_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      495 2023-05-19 17:45:00.000000 flyem_segmentation_pipeline-1.3.2/src/flyem_segmentation_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)        1 2023-05-19 17:45:00.000000 flyem_segmentation_pipeline-1.3.2/src/flyem_segmentation_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       24 2023-05-19 17:45:00.000000 flyem_segmentation_pipeline-1.3.2/src/flyem_segmentation_pipeline.egg-info/requires.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       34 2023-05-19 17:45:00.000000 flyem_segmentation_pipeline-1.3.2/src/flyem_segmentation_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:45:00.111157 flyem_segmentation_pipeline-1.3.2/src/segmentationMVC/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      112 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.2/src/segmentationMVC/__init__.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1228 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.2/src/segmentationMVC/controller.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1256 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.2/src/segmentationMVC/model.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      152 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.2/src/segmentationMVC/view.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:45:00.111377 flyem_segmentation_pipeline-1.3.2/src/segmentationUtils/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       43 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.2/src/segmentationUtils/__init__.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5528 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.2/src/segmentationUtils/imageUtils.py
```

### Comparing `flyem_segmentation_pipeline-1.3.1/PKG-INFO` & `flyem_segmentation_pipeline-1.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyem_segmentation_pipeline
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package based on traditional segmentation algorithms used to segment a fly retina images.
 Home-page: https://github.com/kshvr16/CS410_FlyEM_PyPi
 Author: Sai Harshavardhan Reddy Kona
 Author-email: s.kona001@umb.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kshvr16/CS410_FlyEM_PyPI/issues
 Keywords: medical image,medical image segmentation,fly retina images,electron microscopy images
@@ -81,45 +81,44 @@
 The below sample code reads an image from the input path. 
 ```python
 from segmentationMVC.controller import ImageController
 image_data = ImageController.read("..")
 ```
 Output:
 
-![input image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_input.png)
-
+![input image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_input.png)
 
 The below sample code normalized the input image.
 ```python
 from segmentationMVC.controller import ImageController
 normalized_data = ImageController.normalize(image_data)
 ```
 Output:
 
-![normalized image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_normalize.png)
+![normalized image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_normalize.png)
 
 
 The below sample code crops the input image.
 ```python
 from segmentationMVC.controller import ImageController
 crop_data = ImageController.normalize(normalized_data)
 ```
 Output:
 
-![crop image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_crop.png)
+![crop image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_crop.png)
 
 
 The below sample code smoothens the input image.
 ```python
 from segmentationMVC.controller import ImageController
 smoothed_data = ImageController.smooth(crop_data)
 ```
 Output:
 
-![smoothens image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_smoothen.png)
+![smoothens image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_smoothen.png)
 
 
 To get the complete segmented image, the following will serve as an example.
 ```python
 from segmentationMVC.controller import ImageController
 
 image_data = ImageController.read("..")
@@ -138,8 +137,8 @@
 segmented_image = ImageController.binary_image(closed_binary_mask_data)
 ```
 The variable **segmented_image** in the above sample code stores the result of the segmented image.
 
 
 Output:
 
-![output image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_output.png)
+![output image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_output.png)
```

### Comparing `flyem_segmentation_pipeline-1.3.1/README.md` & `flyem_segmentation_pipeline-1.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,45 +66,44 @@
 The below sample code reads an image from the input path. 
 ```python
 from segmentationMVC.controller import ImageController
 image_data = ImageController.read("..")
 ```
 Output:
 
-![input image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_input.png)
-
+![input image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_input.png)
 
 The below sample code normalized the input image.
 ```python
 from segmentationMVC.controller import ImageController
 normalized_data = ImageController.normalize(image_data)
 ```
 Output:
 
-![normalized image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_normalize.png)
+![normalized image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_normalize.png)
 
 
 The below sample code crops the input image.
 ```python
 from segmentationMVC.controller import ImageController
 crop_data = ImageController.normalize(normalized_data)
 ```
 Output:
 
-![crop image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_crop.png)
+![crop image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_crop.png)
 
 
 The below sample code smoothens the input image.
 ```python
 from segmentationMVC.controller import ImageController
 smoothed_data = ImageController.smooth(crop_data)
 ```
 Output:
 
-![smoothens image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_smoothen.png)
+![smoothens image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_smoothen.png)
 
 
 To get the complete segmented image, the following will serve as an example.
 ```python
 from segmentationMVC.controller import ImageController
 
 image_data = ImageController.read("..")
@@ -123,8 +122,8 @@
 segmented_image = ImageController.binary_image(closed_binary_mask_data)
 ```
 The variable **segmented_image** in the above sample code stores the result of the segmented image.
 
 
 Output:
 
-![output image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_output.png)
+![output image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_output.png)
```

### Comparing `flyem_segmentation_pipeline-1.3.1/setup.py` & `flyem_segmentation_pipeline-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='flyem_segmentation_pipeline',
-    version='1.3.1',
+    version='1.3.2',
     license='MIT',
     author="Sai Harshavardhan Reddy Kona",
     author_email='s.kona001@umb.edu',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/kshvr16/CS410_FlyEM_PyPi',
     description='A package based on traditional segmentation algorithms used to segment a fly retina images.',
```

### Comparing `flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/PKG-INFO` & `flyem_segmentation_pipeline-1.3.2/src/flyem_segmentation_pipeline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyem-segmentation-pipeline
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package based on traditional segmentation algorithms used to segment a fly retina images.
 Home-page: https://github.com/kshvr16/CS410_FlyEM_PyPi
 Author: Sai Harshavardhan Reddy Kona
 Author-email: s.kona001@umb.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kshvr16/CS410_FlyEM_PyPI/issues
 Keywords: medical image,medical image segmentation,fly retina images,electron microscopy images
@@ -81,45 +81,44 @@
 The below sample code reads an image from the input path. 
 ```python
 from segmentationMVC.controller import ImageController
 image_data = ImageController.read("..")
 ```
 Output:
 
-![input image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_input.png)
-
+![input image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_input.png)
 
 The below sample code normalized the input image.
 ```python
 from segmentationMVC.controller import ImageController
 normalized_data = ImageController.normalize(image_data)
 ```
 Output:
 
-![normalized image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_normalize.png)
+![normalized image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_normalize.png)
 
 
 The below sample code crops the input image.
 ```python
 from segmentationMVC.controller import ImageController
 crop_data = ImageController.normalize(normalized_data)
 ```
 Output:
 
-![crop image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_crop.png)
+![crop image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_crop.png)
 
 
 The below sample code smoothens the input image.
 ```python
 from segmentationMVC.controller import ImageController
 smoothed_data = ImageController.smooth(crop_data)
 ```
 Output:
 
-![smoothens image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_smoothen.png)
+![smoothens image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_smoothen.png)
 
 
 To get the complete segmented image, the following will serve as an example.
 ```python
 from segmentationMVC.controller import ImageController
 
 image_data = ImageController.read("..")
@@ -138,8 +137,8 @@
 segmented_image = ImageController.binary_image(closed_binary_mask_data)
 ```
 The variable **segmented_image** in the above sample code stores the result of the segmented image.
 
 
 Output:
 
-![output image](https://github.com/kshvr16/CS410_FlyEM_PyPi/blob/main/docs/sample_output.png)
+![output image](https://raw.githubusercontent.com/kshvr16/CS410_FlyEM_PyPi/master/docs/sample_output.png)
```

### Comparing `flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/controller.py` & `flyem_segmentation_pipeline-1.3.2/src/segmentationMVC/controller.py`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/model.py` & `flyem_segmentation_pipeline-1.3.2/src/segmentationMVC/model.py`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.3.1/src/segmentationUtils/imageUtils.py` & `flyem_segmentation_pipeline-1.3.2/src/segmentationUtils/imageUtils.py`

 * *Files identical despite different names*

