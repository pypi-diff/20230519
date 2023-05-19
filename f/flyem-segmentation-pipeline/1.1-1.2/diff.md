# Comparing `tmp/flyem_segmentation_pipeline-1.1.tar.gz` & `tmp/flyem_segmentation_pipeline-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyem_segmentation_pipeline-1.1.tar", last modified: Fri May 19 16:11:50 2023, max compression
+gzip compressed data, was "flyem_segmentation_pipeline-1.2.tar", last modified: Fri May 19 16:16:20 2023, max compression
```

## Comparing `flyem_segmentation_pipeline-1.1.tar` & `flyem_segmentation_pipeline-1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:11:50.215978 flyem_segmentation_pipeline-1.1/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      683 2023-05-19 16:11:50.216038 flyem_segmentation_pipeline-1.1/PKG-INFO
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      904 2023-05-19 15:34:25.000000 flyem_segmentation_pipeline-1.1/README.md
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      107 2023-05-19 16:11:50.216247 flyem_segmentation_pipeline-1.1/setup.cfg
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1036 2023-05-19 16:11:26.000000 flyem_segmentation_pipeline-1.1/setup.py
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:11:50.213731 flyem_segmentation_pipeline-1.1/src/
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:11:50.214638 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      683 2023-05-19 16:11:50.000000 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      495 2023-05-19 16:11:50.000000 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)        1 2023-05-19 16:11:50.000000 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       24 2023-05-19 16:11:50.000000 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/requires.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       34 2023-05-19 16:11:50.000000 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:11:50.215474 flyem_segmentation_pipeline-1.1/src/segmentationMVC/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      112 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationMVC/__init__.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1228 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationMVC/controller.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1256 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationMVC/model.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      152 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationMVC/view.py
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:11:50.215828 flyem_segmentation_pipeline-1.1/src/segmentationUtils/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       43 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationUtils/__init__.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5528 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationUtils/imageUtils.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:16:20.662844 flyem_segmentation_pipeline-1.2/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1571 2023-05-19 16:16:20.662970 flyem_segmentation_pipeline-1.2/PKG-INFO
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      904 2023-05-19 15:34:25.000000 flyem_segmentation_pipeline-1.2/README.md
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      107 2023-05-19 16:16:20.663288 flyem_segmentation_pipeline-1.2/setup.cfg
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1048 2023-05-19 16:16:09.000000 flyem_segmentation_pipeline-1.2/setup.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:16:20.661081 flyem_segmentation_pipeline-1.2/src/
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:16:20.662065 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1571 2023-05-19 16:16:20.000000 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      495 2023-05-19 16:16:20.000000 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)        1 2023-05-19 16:16:20.000000 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       24 2023-05-19 16:16:20.000000 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/requires.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       34 2023-05-19 16:16:20.000000 flyem_segmentation_pipeline-1.2/src/flyem_segmentation_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:16:20.662514 flyem_segmentation_pipeline-1.2/src/segmentationMVC/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      112 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationMVC/__init__.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1228 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationMVC/controller.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1256 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationMVC/model.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      152 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationMVC/view.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:16:20.662741 flyem_segmentation_pipeline-1.2/src/segmentationUtils/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       43 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationUtils/__init__.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5528 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.2/src/segmentationUtils/imageUtils.py
```

### Comparing `flyem_segmentation_pipeline-1.1/README.md` & `flyem_segmentation_pipeline-1.2/README.md`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.1/setup.py` & `flyem_segmentation_pipeline-1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='flyem_segmentation_pipeline',
-    version='1.1',
+    version='1.2',
     license='MIT',
     author="Sai Harshavardhan Reddy Kona",
     author_email='s.kona001@umb.edu',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/kshvr16/CS410_FlyEM_PyPi',
     description='A package based on traditional segmentation algorithms used to segment a fly retina images.',
-    long_description='file: README.md',
+    long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     project_urls={
         'Bug Tracker': 'https://github.com/kshvr16/CS410_FlyEM_PyPI/issues',
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

### Comparing `flyem_segmentation_pipeline-1.1/src/segmentationMVC/controller.py` & `flyem_segmentation_pipeline-1.2/src/segmentationMVC/controller.py`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.1/src/segmentationMVC/model.py` & `flyem_segmentation_pipeline-1.2/src/segmentationMVC/model.py`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.1/src/segmentationUtils/imageUtils.py` & `flyem_segmentation_pipeline-1.2/src/segmentationUtils/imageUtils.py`

 * *Files identical despite different names*

