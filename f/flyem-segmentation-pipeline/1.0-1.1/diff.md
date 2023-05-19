# Comparing `tmp/flyem_segmentation_pipeline-1.0.tar.gz` & `tmp/flyem_segmentation_pipeline-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyem_segmentation_pipeline-1.0.tar", last modified: Fri May 19 15:35:27 2023, max compression
+gzip compressed data, was "flyem_segmentation_pipeline-1.1.tar", last modified: Fri May 19 16:11:50 2023, max compression
```

## Comparing `flyem_segmentation_pipeline-1.0.tar` & `flyem_segmentation_pipeline-1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 15:35:27.702382 flyem_segmentation_pipeline-1.0/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      240 2023-05-19 15:35:27.702437 flyem_segmentation_pipeline-1.0/PKG-INFO
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      904 2023-05-19 15:34:25.000000 flyem_segmentation_pipeline-1.0/README.md
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      107 2023-05-19 15:35:27.702636 flyem_segmentation_pipeline-1.0/setup.cfg
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      487 2023-05-19 15:33:32.000000 flyem_segmentation_pipeline-1.0/setup.py
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 15:35:27.700691 flyem_segmentation_pipeline-1.0/src/
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 15:35:27.701622 flyem_segmentation_pipeline-1.0/src/flyem_segmentation_pipeline.egg-info/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      240 2023-05-19 15:35:27.000000 flyem_segmentation_pipeline-1.0/src/flyem_segmentation_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      495 2023-05-19 15:35:27.000000 flyem_segmentation_pipeline-1.0/src/flyem_segmentation_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)        1 2023-05-19 15:35:27.000000 flyem_segmentation_pipeline-1.0/src/flyem_segmentation_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       38 2023-05-19 15:35:27.000000 flyem_segmentation_pipeline-1.0/src/flyem_segmentation_pipeline.egg-info/requires.txt
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       34 2023-05-19 15:35:27.000000 flyem_segmentation_pipeline-1.0/src/flyem_segmentation_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 15:35:27.702059 flyem_segmentation_pipeline-1.0/src/segmentationMVC/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      112 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.0/src/segmentationMVC/__init__.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1228 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.0/src/segmentationMVC/controller.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1256 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.0/src/segmentationMVC/model.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)      152 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.0/src/segmentationMVC/view.py
-drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 15:35:27.702278 flyem_segmentation_pipeline-1.0/src/segmentationUtils/
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)       43 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.0/src/segmentationUtils/__init__.py
--rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5528 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.0/src/segmentationUtils/imageUtils.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:11:50.215978 flyem_segmentation_pipeline-1.1/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      683 2023-05-19 16:11:50.216038 flyem_segmentation_pipeline-1.1/PKG-INFO
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      904 2023-05-19 15:34:25.000000 flyem_segmentation_pipeline-1.1/README.md
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      107 2023-05-19 16:11:50.216247 flyem_segmentation_pipeline-1.1/setup.cfg
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1036 2023-05-19 16:11:26.000000 flyem_segmentation_pipeline-1.1/setup.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:11:50.213731 flyem_segmentation_pipeline-1.1/src/
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:11:50.214638 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      683 2023-05-19 16:11:50.000000 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      495 2023-05-19 16:11:50.000000 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)        1 2023-05-19 16:11:50.000000 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       24 2023-05-19 16:11:50.000000 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/requires.txt
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       34 2023-05-19 16:11:50.000000 flyem_segmentation_pipeline-1.1/src/flyem_segmentation_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:11:50.215474 flyem_segmentation_pipeline-1.1/src/segmentationMVC/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      112 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationMVC/__init__.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1228 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationMVC/controller.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     1256 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationMVC/model.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)      152 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationMVC/view.py
+drwxr-xr-x   0 nikhilaharsha   (501) staff       (20)        0 2023-05-19 16:11:50.215828 flyem_segmentation_pipeline-1.1/src/segmentationUtils/
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)       43 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationUtils/__init__.py
+-rw-r--r--   0 nikhilaharsha   (501) staff       (20)     5528 2023-05-19 07:03:45.000000 flyem_segmentation_pipeline-1.1/src/segmentationUtils/imageUtils.py
```

### Comparing `flyem_segmentation_pipeline-1.0/README.md` & `flyem_segmentation_pipeline-1.1/README.md`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.0/src/segmentationMVC/controller.py` & `flyem_segmentation_pipeline-1.1/src/segmentationMVC/controller.py`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.0/src/segmentationMVC/model.py` & `flyem_segmentation_pipeline-1.1/src/segmentationMVC/model.py`

 * *Files identical despite different names*

### Comparing `flyem_segmentation_pipeline-1.0/src/segmentationUtils/imageUtils.py` & `flyem_segmentation_pipeline-1.1/src/segmentationUtils/imageUtils.py`

 * *Files identical despite different names*

