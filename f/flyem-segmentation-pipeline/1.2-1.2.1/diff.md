# Comparing `tmp/flyem_segmentation_pipeline-1.2.tar.gz` & `tmp/flyem_segmentation_pipeline-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyem_segmentation_pipeline-1.2.tar", last modified: Fri May 19 16:16:20 2023, max compression
+gzip compressed data, was "flyem_segmentation_pipeline-1.2.1.tar", last modified: Fri May 19 16:32:24 2023, max compression
```

## Comparing `flyem_segmentation_pipeline-1.2.tar` & `flyem_segmentation_pipeline-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:16:20.662844 flyem_segmentation_pipeline-1.2/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1571 2023-05-19 16:16:20.662970 flyem_segmentation_pipeline-1.2/PKG-INFO
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      904 2023-05-19 15:34:25.000000 flyem_segmentation_pipeline-1.2/README.md
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      107 2023-05-19 16:16:20.663288 flyem_segmentation_pipeline-1.2/setup.cfg
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1048 2023-05-19 16:16:09.000000 flyem_segmentation_pipeline-1.2/setup.py
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:16:20.661081 flyem_segmentation_pipeline-1.2/src/
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:16:20.662065 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1571 2023-05-19 16:16:20.000000 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      495 2023-05-19 16:16:20.000000 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)        1 2023-05-19 16:16:20.000000 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       24 2023-05-19 16:16:20.000000 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/requires.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       34 2023-05-19 16:16:20.000000 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:16:20.662514 flyem_segmentation_pipeline-1.2/src/segmentationMVC/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      112 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationMVC/__init__.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1228 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationMVC/controller.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1256 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationMVC/model.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      152 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationMVC/view.py
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:16:20.662741 flyem_segmentation_pipeline-1.2/src/segmentationUtils/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       43 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationUtils/__init__.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5528 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationUtils/imageUtils.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:32:24.015736 flyem_segmentation_pipeline-1.2.1/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     2030 2023-05-19 16:32:24.015794 flyem_segmentation_pipeline-1.2.1/PKG-INFO
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1361 2023-05-19 16:31:28.000000 flyem_segmentation_pipeline-1.2.1/README.md
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      107 2023-05-19 16:32:24.015996 flyem_segmentation_pipeline-1.2.1/setup.cfg
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1050 2023-05-19 16:32:14.000000 flyem_segmentation_pipeline-1.2.1/setup.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:32:24.013980 flyem_segmentation_pipeline-1.2.1/src/
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:32:24.014963 flyem_segmentation_pipeline-1.2.1/src/flyem_segmentation_pipeline.egg-info/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     2030 2023-05-19 16:32:23.000000 flyem_segmentation_pipeline-1.2.1/src/flyem_segmentation_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      495 2023-05-19 16:32:23.000000 flyem_segmentation_pipeline-1.2.1/src/flyem_segmentation_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)        1 2023-05-19 16:32:23.000000 flyem_segmentation_pipeline-1.2.1/src/flyem_segmentation_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       24 2023-05-19 16:32:23.000000 flyem_segmentation_pipeline-1.2.1/src/flyem_segmentation_pipeline.egg-info/requires.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       34 2023-05-19 16:32:23.000000 flyem_segmentation_pipeline-1.2.1/src/flyem_segmentation_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:32:24.015407 flyem_segmentation_pipeline-1.2.1/src/segmentationMVC/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      112 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2.1/src/segmentationMVC/__init__.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1228 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2.1/src/segmentationMVC/controller.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1256 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2.1/src/segmentationMVC/model.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      152 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2.1/src/segmentationMVC/view.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:32:24.015634 flyem_segmentation_pipeline-1.2.1/src/segmentationUtils/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       43 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2.1/src/segmentationUtils/__init__.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5528 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2.1/src/segmentationUtils/imageUtils.py
```

### Comparing `flyem_segmentation_pipeline-1.2/PKG-INFO` & `flyem_segmentation_pipeline-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyem_segmentation_pipeline
-Version: 1.2
+Version: 1.2.1
 Summary: A package based on traditional segmentation algorithms used to segment a fly retina images.
 Home-page: https://github.com/kshvr16/CS410_FlyEM_PyPi
 Author: Sai Harshavardhan Reddy Kona
 Author-email: s.kona001@umb.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kshvr16/CS410_FlyEM_PyPI/issues
 Keywords: medical image,medical image segmentation,fly retina images,electron microscopy images
@@ -30,15 +30,22 @@
 
 ## Package Installation
 
 Install this python package by executing the following command.
 ```bash
   pip install flyem_segmentation_pipeline
 ```
+If the above command throws any error, please run the following command and install the dependency packages individually.
+```bash
+pip install flyem_segmentation_pipeling --no-deps
+```
 
 
 ## Required Python packages
 
 * [numpy](https://pypi.org/project/numpy/)
 * [mahotas](https://pypi.org/project/mahotas/)
 * [matplotlib](https://pypi.org/project/matplotlib/)
 * [scikit-image](https://pypi.org/project/scikit-image/)
+
+    ## Dependency package issues
+All the above-mentioned packages are required to use this package, but due to the version issues with numpy and mahotas, during installation only matplotlib and scikit-image are installed; numpy and mahotas has to be installed separately.
```

### Comparing `flyem_segmentation_pipeline-1.2/setup.py` & `flyem_segmentation_pipeline-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='flyem_segmentation_pipeline',
-    version='1.2',
+    version='1.2.1',
     license='MIT',
     author="Sai Harshavardhan Reddy Kona",
     author_email='s.kona001@umb.edu',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/kshvr16/CS410_FlyEM_PyPi',
     description='A package based on traditional segmentation algorithms used to segment a fly retina images.',
```

### Comparing `flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/PKG-INFO` & `flyem_segmentation_pipeline-1.2.1/src/flyem_segmentation_pipeline.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flyem-segmentation-pipeline
-Version: 1.2
+Version: 1.2.1
 Summary: A package based on traditional segmentation algorithms used to segment a fly retina images.
 Home-page: https://github.com/kshvr16/CS410_FlyEM_PyPi
 Author: Sai Harshavardhan Reddy Kona
 Author-email: s.kona001@umb.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kshvr16/CS410_FlyEM_PyPI/issues
 Keywords: medical image,medical image segmentation,fly retina images,electron microscopy images
@@ -30,15 +30,22 @@
 
 ## Package Installation
 
 Install this python package by executing the following command.
 ```bash
   pip install flyem_segmentation_pipeline
 ```
+If the above command throws any error, please run the following command and install the dependency packages individually.
+```bash
+pip install flyem_segmentation_pipeling --no-deps
+```
 
 
 ## Required Python packages
 
 * [numpy](https://pypi.org/project/numpy/)
 * [mahotas](https://pypi.org/project/mahotas/)
 * [matplotlib](https://pypi.org/project/matplotlib/)
 * [scikit-image](https://pypi.org/project/scikit-image/)
+
+    ## Dependency package issues
+All the above-mentioned packages are required to use this package, but due to the version issues with numpy and mahotas, during installation only matplotlib and scikit-image are installed; numpy and mahotas has to be installed separately.
```

### Comparing `flyem_segmentation_pipeline-1.2/src/segmentationMVC/controller.py` & `flyem_segmentation_pipeline-1.2.1/src/segmentationMVC/controller.py`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.2/src/segmentationMVC/model.py` & `flyem_segmentation_pipeline-1.2.1/src/segmentationMVC/model.py`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.2/src/segmentationUtils/imageUtils.py` & `flyem_segmentation_pipeline-1.2.1/src/segmentationUtils/imageUtils.py`

 * *Files identical despite different names*

