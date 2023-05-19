# Comparing `tmp/ipydex-0.8.1.tar.gz` & `tmp/ipydex-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ipydex-0.8.1.tar", last modified: Mon May 27 22:01:10 2019, max compression
+gzip compressed data, was "dist/ipydex-0.8.2.tar", last modified: Mon May 27 22:15:16 2019, max compression
```

## Comparing `ipydex-0.8.1.tar` & `ipydex-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ck        (1000) ck        (1000)        0 2019-05-27 22:01:10.000000 ipydex-0.8.1/
-drwxr-xr-x   0 ck        (1000) ck        (1000)        0 2019-05-27 22:01:10.000000 ipydex-0.8.1/ipydex/
--rw-r--r--   0 ck        (1000) ck        (1000)    12802 2019-05-27 20:45:09.000000 ipydex-0.8.1/ipydex/displaytools.py
--rw-r--r--   0 ck        (1000) ck        (1000)       22 2019-05-27 22:00:17.000000 ipydex-0.8.1/ipydex/release.py
--rw-r--r--   0 ck        (1000) ck        (1000)       53 2017-11-11 16:35:29.000000 ipydex-0.8.1/ipydex/__init__.py
--rw-r--r--   0 ck        (1000) ck        (1000)    25408 2019-05-21 14:25:12.000000 ipydex-0.8.1/ipydex/core.py
--rw-r--r--   0 ck        (1000) ck        (1000)       45 2017-09-08 22:23:02.000000 ipydex-0.8.1/MANIFEST.in
--rw-r--r--   0 ck        (1000) ck        (1000)       38 2019-05-27 22:01:10.000000 ipydex-0.8.1/setup.cfg
--rw-r--r--   0 ck        (1000) ck        (1000)      602 2019-05-27 22:01:10.000000 ipydex-0.8.1/PKG-INFO
--rw-r--r--   0 ck        (1000) ck        (1000)     2155 2017-11-11 16:19:05.000000 ipydex-0.8.1/README.rst
-drwxr-xr-x   0 ck        (1000) ck        (1000)        0 2019-05-27 22:01:10.000000 ipydex-0.8.1/ipydex.egg-info/
--rw-r--r--   0 ck        (1000) ck        (1000)        7 2019-05-27 22:01:10.000000 ipydex-0.8.1/ipydex.egg-info/top_level.txt
--rw-r--r--   0 ck        (1000) ck        (1000)      301 2019-05-27 22:01:10.000000 ipydex-0.8.1/ipydex.egg-info/SOURCES.txt
--rw-r--r--   0 ck        (1000) ck        (1000)      602 2019-05-27 22:01:10.000000 ipydex-0.8.1/ipydex.egg-info/PKG-INFO
--rw-r--r--   0 ck        (1000) ck        (1000)       15 2019-05-27 22:01:10.000000 ipydex-0.8.1/ipydex.egg-info/requires.txt
--rw-r--r--   0 ck        (1000) ck        (1000)        1 2017-09-08 20:55:11.000000 ipydex-0.8.1/ipydex.egg-info/not-zip-safe
--rw-r--r--   0 ck        (1000) ck        (1000)        1 2019-05-27 22:01:10.000000 ipydex-0.8.1/ipydex.egg-info/dependency_links.txt
--rw-r--r--   0 ck        (1000) ck        (1000)      917 2019-05-27 22:00:01.000000 ipydex-0.8.1/setup.py
--rw-r--r--   0 ck        (1000) ck        (1000)       15 2017-10-06 12:33:00.000000 ipydex-0.8.1/requirements.txt
+drwxr-xr-x   0 ck        (1000) ck        (1000)        0 2019-05-27 22:15:16.000000 ipydex-0.8.2/
+drwxr-xr-x   0 ck        (1000) ck        (1000)        0 2019-05-27 22:15:16.000000 ipydex-0.8.2/ipydex/
+-rw-r--r--   0 ck        (1000) ck        (1000)    12802 2019-05-27 20:45:09.000000 ipydex-0.8.2/ipydex/displaytools.py
+-rw-r--r--   0 ck        (1000) ck        (1000)       22 2019-05-27 22:15:11.000000 ipydex-0.8.2/ipydex/release.py
+-rw-r--r--   0 ck        (1000) ck        (1000)      195 2019-05-27 22:13:33.000000 ipydex-0.8.2/ipydex/__init__.py
+-rw-r--r--   0 ck        (1000) ck        (1000)    25408 2019-05-21 14:25:12.000000 ipydex-0.8.2/ipydex/core.py
+-rw-r--r--   0 ck        (1000) ck        (1000)       45 2017-09-08 22:23:02.000000 ipydex-0.8.2/MANIFEST.in
+-rw-r--r--   0 ck        (1000) ck        (1000)       38 2019-05-27 22:15:16.000000 ipydex-0.8.2/setup.cfg
+-rw-r--r--   0 ck        (1000) ck        (1000)      602 2019-05-27 22:15:16.000000 ipydex-0.8.2/PKG-INFO
+-rw-r--r--   0 ck        (1000) ck        (1000)     2155 2017-11-11 16:19:05.000000 ipydex-0.8.2/README.rst
+drwxr-xr-x   0 ck        (1000) ck        (1000)        0 2019-05-27 22:15:16.000000 ipydex-0.8.2/ipydex.egg-info/
+-rw-r--r--   0 ck        (1000) ck        (1000)        7 2019-05-27 22:15:16.000000 ipydex-0.8.2/ipydex.egg-info/top_level.txt
+-rw-r--r--   0 ck        (1000) ck        (1000)      301 2019-05-27 22:15:16.000000 ipydex-0.8.2/ipydex.egg-info/SOURCES.txt
+-rw-r--r--   0 ck        (1000) ck        (1000)      602 2019-05-27 22:15:16.000000 ipydex-0.8.2/ipydex.egg-info/PKG-INFO
+-rw-r--r--   0 ck        (1000) ck        (1000)       15 2019-05-27 22:15:16.000000 ipydex-0.8.2/ipydex.egg-info/requires.txt
+-rw-r--r--   0 ck        (1000) ck        (1000)        1 2017-09-08 20:55:11.000000 ipydex-0.8.2/ipydex.egg-info/not-zip-safe
+-rw-r--r--   0 ck        (1000) ck        (1000)        1 2019-05-27 22:15:16.000000 ipydex-0.8.2/ipydex.egg-info/dependency_links.txt
+-rw-r--r--   0 ck        (1000) ck        (1000)      917 2019-05-27 22:00:01.000000 ipydex-0.8.2/setup.py
+-rw-r--r--   0 ck        (1000) ck        (1000)       15 2017-10-06 12:33:00.000000 ipydex-0.8.2/requirements.txt
```

### Comparing `ipydex-0.8.1/ipydex/displaytools.py` & `ipydex-0.8.2/ipydex/displaytools.py`

 * *Files identical despite different names*

### Comparing `ipydex-0.8.1/ipydex/core.py` & `ipydex-0.8.2/ipydex/core.py`

 * *Files identical despite different names*

### Comparing `ipydex-0.8.1/PKG-INFO` & `ipydex-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ipydex
-Version: 0.8.1
+Version: 0.8.2
 Summary: IPython based debugging and exploring tool
 Home-page: http://github.com/cknoll/ipydex
 Author: cknoll
 Author-email: carsten.knoll@tu-dresden.de
 License: GPLv3+
 Description: UNKNOWN
 Keywords: ipython embedded excepthook debugger
```

### Comparing `ipydex-0.8.1/README.rst` & `ipydex-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `ipydex-0.8.1/ipydex.egg-info/PKG-INFO` & `ipydex-0.8.2/ipydex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ipydex
-Version: 0.8.1
+Version: 0.8.2
 Summary: IPython based debugging and exploring tool
 Home-page: http://github.com/cknoll/ipydex
 Author: cknoll
 Author-email: carsten.knoll@tu-dresden.de
 License: GPLv3+
 Description: UNKNOWN
 Keywords: ipython embedded excepthook debugger
```

### Comparing `ipydex-0.8.1/setup.py` & `ipydex-0.8.2/setup.py`

 * *Files identical despite different names*

