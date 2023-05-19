# Comparing `tmp/improutils-1.1.8.tar.gz` & `tmp/improutils-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "improutils-1.1.8.tar", last modified: Thu Nov 18 09:23:24 2021, max compression
+gzip compressed data, was "improutils-1.1.9.tar", last modified: Mon Apr  4 13:38:10 2022, max compression
```

## Comparing `improutils-1.1.8.tar` & `improutils-1.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-18 09:23:24.722771 improutils-1.1.8/
--rw-r--r--   0 root         (0) root         (0)     1073 2021-11-18 09:14:51.000000 improutils-1.1.8/LICENCE
--rw-r--r--   0 root         (0) root         (0)     1619 2021-11-18 09:23:24.722771 improutils-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1122 2021-11-18 09:14:51.000000 improutils-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-18 09:23:24.722771 improutils-1.1.8/improutils/
--rw-r--r--   0 root         (0) root         (0)      188 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-18 09:23:24.722771 improutils-1.1.8/improutils/acquisition/
--rw-r--r--   0 root         (0) root         (0)       21 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/acquisition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3409 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/acquisition/img_io.py
--rw-r--r--   0 root         (0) root         (0)      813 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/acquisition/pypylon.py
--rw-r--r--   0 root         (0) root         (0)     7804 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/acquisition/pypylon_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-18 09:23:24.722771 improutils-1.1.8/improutils/filtration/
--rw-r--r--   0 root         (0) root         (0)       25 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/filtration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3149 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/filtration/filtration.py
--rw-r--r--   0 root         (0) root         (0)     2897 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/other.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-18 09:23:24.722771 improutils-1.1.8/improutils/perspective/
--rw-r--r--   0 root         (0) root         (0)       30 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/perspective/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2908 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/perspective/coordconversion.py
--rw-r--r--   0 root         (0) root         (0)     1344 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/perspective/heightestimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-18 09:23:24.722771 improutils-1.1.8/improutils/preprocessing/
--rw-r--r--   0 root         (0) root         (0)       52 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/preprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4588 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/preprocessing/calibration.py
--rw-r--r--   0 root         (0) root         (0)     3420 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/preprocessing/contours.py
--rw-r--r--   0 root         (0) root         (0)     5414 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/preprocessing/preprocessing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-18 09:23:24.722771 improutils-1.1.8/improutils/recognition/
--rw-r--r--   0 root         (0) root         (0)       48 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/recognition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2539 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/recognition/image_features.py
--rw-r--r--   0 root         (0) root         (0)      468 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/recognition/ocr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-18 09:23:24.722771 improutils-1.1.8/improutils/segmentation/
--rw-r--r--   0 root         (0) root         (0)       27 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/segmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3451 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/segmentation/segmentation.py
--rw-r--r--   0 root         (0) root         (0)      189 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-18 09:23:24.722771 improutils-1.1.8/improutils/visualisation/
--rw-r--r--   0 root         (0) root         (0)       28 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/visualisation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5374 2021-11-18 09:14:51.000000 improutils-1.1.8/improutils/visualisation/visualisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-18 09:23:24.722771 improutils-1.1.8/improutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1619 2021-11-18 09:23:24.000000 improutils-1.1.8/improutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1009 2021-11-18 09:23:24.000000 improutils-1.1.8/improutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-18 09:23:24.000000 improutils-1.1.8/improutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      137 2021-11-18 09:23:24.000000 improutils-1.1.8/improutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2021-11-18 09:23:24.000000 improutils-1.1.8/improutils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-18 09:23:24.722771 improutils-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1127 2021-11-18 09:20:23.000000 improutils-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 13:38:10.577628 improutils-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)     1073 2022-04-04 13:35:14.000000 improutils-1.1.9/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     1619 2022-04-04 13:38:10.577628 improutils-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1122 2022-04-04 13:35:14.000000 improutils-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 13:38:10.577628 improutils-1.1.9/improutils/
+-rw-r--r--   0 root         (0) root         (0)      188 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 13:38:10.577628 improutils-1.1.9/improutils/acquisition/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/acquisition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/acquisition/img_io.py
+-rw-r--r--   0 root         (0) root         (0)      813 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/acquisition/pypylon.py
+-rw-r--r--   0 root         (0) root         (0)     7804 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/acquisition/pypylon_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 13:38:10.577628 improutils-1.1.9/improutils/filtration/
+-rw-r--r--   0 root         (0) root         (0)       25 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/filtration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3162 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/filtration/filtration.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/other.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 13:38:10.577628 improutils-1.1.9/improutils/perspective/
+-rw-r--r--   0 root         (0) root         (0)       30 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/perspective/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/perspective/coordconversion.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/perspective/heightestimator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 13:38:10.577628 improutils-1.1.9/improutils/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)       52 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/preprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/preprocessing/calibration.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/preprocessing/contours.py
+-rw-r--r--   0 root         (0) root         (0)     5414 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/preprocessing/preprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 13:38:10.577628 improutils-1.1.9/improutils/recognition/
+-rw-r--r--   0 root         (0) root         (0)       48 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/recognition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/recognition/image_features.py
+-rw-r--r--   0 root         (0) root         (0)      468 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/recognition/ocr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 13:38:10.577628 improutils-1.1.9/improutils/segmentation/
+-rw-r--r--   0 root         (0) root         (0)       27 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/segmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/segmentation/segmentation.py
+-rw-r--r--   0 root         (0) root         (0)      189 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 13:38:10.577628 improutils-1.1.9/improutils/visualisation/
+-rw-r--r--   0 root         (0) root         (0)       28 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/visualisation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5374 2022-04-04 13:35:14.000000 improutils-1.1.9/improutils/visualisation/visualisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 13:38:10.577628 improutils-1.1.9/improutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1619 2022-04-04 13:38:10.000000 improutils-1.1.9/improutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1009 2022-04-04 13:38:10.000000 improutils-1.1.9/improutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-04 13:38:10.000000 improutils-1.1.9/improutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      137 2022-04-04 13:38:10.000000 improutils-1.1.9/improutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-04-04 13:38:10.000000 improutils-1.1.9/improutils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-04-04 13:38:10.577628 improutils-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1127 2022-04-04 13:35:14.000000 improutils-1.1.9/setup.py
```

### Comparing `improutils-1.1.8/LICENCE` & `improutils-1.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/PKG-INFO` & `improutils-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: improutils
-Version: 1.1.8
+Version: 1.1.9
 Summary: Package with useful functions for BI-SVZ coursework
 Home-page: https://github.com/ImprolabFIT/improutils_package
 Author: ImproLab
 Author-email: improlab@fit.cvut.cz
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `improutils-1.1.8/README.md` & `improutils-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/acquisition/img_io.py` & `improutils-1.1.9/improutils/acquisition/img_io.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/acquisition/pypylon.py` & `improutils-1.1.9/improutils/acquisition/pypylon.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/acquisition/pypylon_config.py` & `improutils-1.1.9/improutils/acquisition/pypylon_config.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/filtration/filtration.py` & `improutils-1.1.9/improutils/filtration/filtration.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     '''Filters image noise using median algorithm
 
     Parameters
     ----------
     img : numpy.ndarray
         Input image.
     filter_size : int
-        Size of median filter.
+        Odd number - size of median filter.
     Returns
     -------
     Output image.
     '''
     return cv2.medianBlur(img, filter_size)
```

### Comparing `improutils-1.1.8/improutils/other.py` & `improutils-1.1.9/improutils/other.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/perspective/coordconversion.py` & `improutils-1.1.9/improutils/perspective/coordconversion.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/perspective/heightestimator.py` & `improutils-1.1.9/improutils/perspective/heightestimator.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/preprocessing/calibration.py` & `improutils-1.1.9/improutils/preprocessing/calibration.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/preprocessing/contours.py` & `improutils-1.1.9/improutils/preprocessing/contours.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/preprocessing/preprocessing.py` & `improutils-1.1.9/improutils/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/recognition/image_features.py` & `improutils-1.1.9/improutils/recognition/image_features.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/segmentation/segmentation.py` & `improutils-1.1.9/improutils/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils/visualisation/visualisation.py` & `improutils-1.1.9/improutils/visualisation/visualisation.py`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/improutils.egg-info/PKG-INFO` & `improutils-1.1.9/improutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: improutils
-Version: 1.1.8
+Version: 1.1.9
 Summary: Package with useful functions for BI-SVZ coursework
 Home-page: https://github.com/ImprolabFIT/improutils_package
 Author: ImproLab
 Author-email: improlab@fit.cvut.cz
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `improutils-1.1.8/improutils.egg-info/SOURCES.txt` & `improutils-1.1.9/improutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `improutils-1.1.8/setup.py` & `improutils-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 import os        
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 
 if os.environ.get('TARGET_ENV'):
     __version__ = __version__ + ".dev" + os.environ['CI_JOB_ID']
 
 setuptools.setup(
     name="improutils",
     author="ImproLab",
```

