# Comparing `tmp/flyem_segmentation_pipeline-1.3.0.tar.gz` & `tmp/flyem_segmentation_pipeline-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyem_segmentation_pipeline-1.3.0.tar", last modified: Fri May 19 17:32:58 2023, max compression
+gzip compressed data, was "flyem_segmentation_pipeline-1.3.1.tar", last modified: Fri May 19 17:37:17 2023, max compression
```

## Comparing `flyem_segmentation_pipeline-1.3.0.tar` & `flyem_segmentation_pipeline-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:32:58.770829 flyem_segmentation_pipeline-1.3.0/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5038 2023-05-19 17:32:58.770885 flyem_segmentation_pipeline-1.3.0/PKG-INFO
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     4369 2023-05-19 17:29:09.000000 flyem_segmentation_pipeline-1.3.0/README.md
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      107 2023-05-19 17:32:58.771084 flyem_segmentation_pipeline-1.3.0/setup.cfg
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1050 2023-05-19 17:32:52.000000 flyem_segmentation_pipeline-1.3.0/setup.py
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:32:58.768819 flyem_segmentation_pipeline-1.3.0/src/
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:32:58.769709 flyem_segmentation_pipeline-1.3.0/src/flyem_segmentation_pipeline.egg-info/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5038 2023-05-19 17:32:58.000000 flyem_segmentation_pipeline-1.3.0/src/flyem_segmentation_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      495 2023-05-19 17:32:58.000000 flyem_segmentation_pipeline-1.3.0/src/flyem_segmentation_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)        1 2023-05-19 17:32:58.000000 flyem_segmentation_pipeline-1.3.0/src/flyem_segmentation_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       24 2023-05-19 17:32:58.000000 flyem_segmentation_pipeline-1.3.0/src/flyem_segmentation_pipeline.egg-info/requires.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       34 2023-05-19 17:32:58.000000 flyem_segmentation_pipeline-1.3.0/src/flyem_segmentation_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:32:58.770428 flyem_segmentation_pipeline-1.3.0/src/segmentationMVC/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      112 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.0/src/segmentationMVC/__init__.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1228 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.0/src/segmentationMVC/controller.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1256 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.0/src/segmentationMVC/model.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      152 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.0/src/segmentationMVC/view.py
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:32:58.770700 flyem_segmentation_pipeline-1.3.0/src/segmentationUtils/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       43 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.0/src/segmentationUtils/__init__.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5528 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.0/src/segmentationUtils/imageUtils.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:37:17.408857 flyem_segmentation_pipeline-1.3.1/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5033 2023-05-19 17:37:17.408929 flyem_segmentation_pipeline-1.3.1/PKG-INFO
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     4364 2023-05-19 17:35:55.000000 flyem_segmentation_pipeline-1.3.1/README.md
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      107 2023-05-19 17:37:17.409142 flyem_segmentation_pipeline-1.3.1/setup.cfg
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1050 2023-05-19 17:37:14.000000 flyem_segmentation_pipeline-1.3.1/setup.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:37:17.406939 flyem_segmentation_pipeline-1.3.1/src/
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:37:17.408004 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5033 2023-05-19 17:37:17.000000 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      495 2023-05-19 17:37:17.000000 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)        1 2023-05-19 17:37:17.000000 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       24 2023-05-19 17:37:17.000000 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/requires.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       34 2023-05-19 17:37:17.000000 flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:37:17.408500 flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      112 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/__init__.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1228 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/controller.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1256 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/model.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      152 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/view.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 17:37:17.408744 flyem_segmentation_pipeline-1.3.1/src/segmentationUtils/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       43 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationUtils/__init__.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5528 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.3.1/src/segmentationUtils/imageUtils.py
```

### Comparing `flyem_segmentation_pipeline-1.3.0/PKG-INFO` & `flyem_segmentation_pipeline-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flyem_segmentation_pipeline
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package based on traditional segmentation algorithms used to segment a fly retina images.
 Home-page: https://github.com/kshvr16/CS410_FlyEM_PyPi
 Author: Sai Harshavardhan Reddy Kona
 Author-email: s.kona001@umb.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kshvr16/CS410_FlyEM_PyPI/issues
 Keywords: medical image,medical image segmentation,fly retina images,electron microscopy images
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# CS410_FlyEM_PyPi
+# CS410_FlyEM
 This repository hosts the segmentation pipeline to segment fly retina images using traditional segmentation algorithms.
 
 
 ## Authors
 
 * [Prof. Daniel Haehn](https://github.com/haehn)
 * [Sai Harshavardhan Reddy Kona](https://github.com/kshvr16)
```

### Comparing `flyem_segmentation_pipeline-1.3.0/README.md` & `flyem_segmentation_pipeline-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CS410_FlyEM_PyPi
+# CS410_FlyEM
 This repository hosts the segmentation pipeline to segment fly retina images using traditional segmentation algorithms.
 
 
 ## Authors
 
 * [Prof. Daniel Haehn](https://github.com/haehn)
 * [Sai Harshavardhan Reddy Kona](https://github.com/kshvr16)
```

### Comparing `flyem_segmentation_pipeline-1.3.0/setup.py` & `flyem_segmentation_pipeline-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='flyem_segmentation_pipeline',
-    version='1.3.0',
+    version='1.3.1',
     license='MIT',
     author="Sai Harshavardhan Reddy Kona",
     author_email='s.kona001@umb.edu',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/kshvr16/CS410_FlyEM_PyPi',
     description='A package based on traditional segmentation algorithms used to segment a fly retina images.',
```

### Comparing `flyem_segmentation_pipeline-1.3.0/src/flyem_segmentation_pipeline.egg-info/PKG-INFO` & `flyem_segmentation_pipeline-1.3.1/src/flyem_segmentation_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flyem-segmentation-pipeline
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package based on traditional segmentation algorithms used to segment a fly retina images.
 Home-page: https://github.com/kshvr16/CS410_FlyEM_PyPi
 Author: Sai Harshavardhan Reddy Kona
 Author-email: s.kona001@umb.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kshvr16/CS410_FlyEM_PyPI/issues
 Keywords: medical image,medical image segmentation,fly retina images,electron microscopy images
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# CS410_FlyEM_PyPi
+# CS410_FlyEM
 This repository hosts the segmentation pipeline to segment fly retina images using traditional segmentation algorithms.
 
 
 ## Authors
 
 * [Prof. Daniel Haehn](https://github.com/haehn)
 * [Sai Harshavardhan Reddy Kona](https://github.com/kshvr16)
```

### Comparing `flyem_segmentation_pipeline-1.3.0/src/segmentationMVC/controller.py` & `flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/controller.py`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.3.0/src/segmentationMVC/model.py` & `flyem_segmentation_pipeline-1.3.1/src/segmentationMVC/model.py`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.3.0/src/segmentationUtils/imageUtils.py` & `flyem_segmentation_pipeline-1.3.1/src/segmentationUtils/imageUtils.py`

 * *Files identical despite different names*

