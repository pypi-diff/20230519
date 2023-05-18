# Comparing `tmp/motionrender-0.1.1.tar.gz` & `tmp/motionrender-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motionrender-0.1.1.tar", last modified: Thu May 18 02:33:36 2023, max compression
+gzip compressed data, was "motionrender-1.0.0.tar", last modified: Thu May 18 22:46:47 2023, max compression
```

## Comparing `motionrender-0.1.1.tar` & `motionrender-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 02:33:36.316563 motionrender-0.1.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34523 2023-05-18 02:33:35.000000 motionrender-0.1.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-05-18 02:33:36.316563 motionrender-0.1.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2023-05-18 02:33:35.000000 motionrender-0.1.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 02:33:36.316563 motionrender-0.1.1/motionrender/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-05-18 02:33:35.000000 motionrender-0.1.1/motionrender/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3278 2023-05-18 02:33:35.000000 motionrender-0.1.1/motionrender/plot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1759 2023-05-18 02:33:35.000000 motionrender-0.1.1/motionrender/render.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5978 2023-05-18 02:33:35.000000 motionrender-0.1.1/motionrender/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 02:33:36.316563 motionrender-0.1.1/motionrender.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-05-18 02:33:36.000000 motionrender-0.1.1/motionrender.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-05-18 02:33:36.000000 motionrender-0.1.1/motionrender.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-18 02:33:36.000000 motionrender-0.1.1/motionrender.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-18 02:33:36.000000 motionrender-0.1.1/motionrender.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-18 02:33:36.316563 motionrender-0.1.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-05-18 02:33:35.000000 motionrender-0.1.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 22:46:47.882021 motionrender-1.0.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34523 2023-05-18 22:46:47.000000 motionrender-1.0.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-05-18 22:46:47.882021 motionrender-1.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      712 2023-05-18 22:46:47.000000 motionrender-1.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 22:46:47.878021 motionrender-1.0.0/motionrender/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19869 2023-05-18 22:46:47.000000 motionrender-1.0.0/motionrender/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 22:46:47.882021 motionrender-1.0.0/motionrender.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-05-18 22:46:47.000000 motionrender-1.0.0/motionrender.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-05-18 22:46:47.000000 motionrender-1.0.0/motionrender.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-18 22:46:47.000000 motionrender-1.0.0/motionrender.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-18 22:46:47.000000 motionrender-1.0.0/motionrender.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-18 22:46:47.882021 motionrender-1.0.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-05-18 22:46:47.000000 motionrender-1.0.0/setup.py
```

### Comparing `motionrender-0.1.1/LICENSE` & `motionrender-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `motionrender-0.1.1/PKG-INFO` & `motionrender-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motionrender
-Version: 0.1.1
+Version: 1.0.0
 Summary: A motion tracking 3D movier render
 Author: Derek Harter
 Author-email: Derek.Harter@tamuc.edu
 License: GPL-3
 Keywords: motion tracking,3D rendering
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `motionrender-0.1.1/README.md` & `motionrender-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 Kinet 3D skeletion tracking position estimator.  Data is expected to be
 in a simple csv format, consisting of a timestamp and then 3D position of
 a set of joints. 
 
 The package provides functions to load in data, help convert it to
 the needed format, and render the data as images and movies.  The
 package relies on Python 3 Matplotlib plotting and movie animations
-using the `mpl_toolkits.mplot3d` and `matplotlib.animation`
+using the and `matplotlib.animation`
 libraries.  This package uses mpeg as a back end renderer to create
 the rendered animations.
```

### Comparing `motionrender-0.1.1/motionrender.egg-info/PKG-INFO` & `motionrender-1.0.0/motionrender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motionrender
-Version: 0.1.1
+Version: 1.0.0
 Summary: A motion tracking 3D movier render
 Author: Derek Harter
 Author-email: Derek.Harter@tamuc.edu
 License: GPL-3
 Keywords: motion tracking,3D rendering
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `motionrender-0.1.1/setup.py` & `motionrender-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1'
+VERSION = '1.0.0'
 DESCRIPTION = 'A motion tracking 3D movier render'
 LONG_DESCRIPTION = 'A package that renders movies from 3D motion tracked data, for example from 3D skeleton joint tracking data'
 
 setup(
     name="motionrender",
     version=VERSION,
     description=DESCRIPTION,
```

