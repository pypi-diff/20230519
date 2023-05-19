# Comparing `tmp/dknovautils-0.1.5.tar.gz` & `tmp/dknovautils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.1.5.tar", last modified: Fri May 12 06:46:19 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.1.6.tar", last modified: Fri May 19 02:09:17 2023, max compression
```

## Comparing `dknovautils-0.1.5.tar` & `dknovautils-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-12 06:46:19.000000 dknovautils-0.1.5/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2523 2023-05-12 05:07:32.000000 dknovautils-0.1.5/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     8651 2023-05-12 06:46:18.000000 dknovautils-0.1.5/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      103 2023-05-04 04:54:01.000000 dknovautils-0.1.5/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1153 2023-05-07 16:31:40.000000 dknovautils-0.1.5/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-05-12 06:46:18.000000 dknovautils-0.1.5/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      501 2023-05-07 13:41:47.000000 dknovautils-0.1.5/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.1.5/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.1.5/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.1.5/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.1.5/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-12 06:46:19.000000 dknovautils-0.1.5/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.1.5/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-05-12 06:46:19.000000 dknovautils-0.1.5/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1159 2023-05-12 06:46:18.000000 dknovautils-0.1.5/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-19 02:09:17.000000 dknovautils-0.1.6/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-19 02:09:17.000000 dknovautils-0.1.6/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2523 2023-05-12 05:07:32.000000 dknovautils-0.1.6/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     8676 2023-05-19 02:09:12.000000 dknovautils-0.1.6/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      103 2023-05-04 04:54:01.000000 dknovautils-0.1.6/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1153 2023-05-07 16:31:40.000000 dknovautils-0.1.6/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-05-19 02:09:12.000000 dknovautils-0.1.6/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      501 2023-05-07 13:41:47.000000 dknovautils-0.1.6/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.1.6/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.1.6/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.1.6/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-19 02:09:17.000000 dknovautils-0.1.6/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-05-19 02:09:15.000000 dknovautils-0.1.6/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-19 02:09:15.000000 dknovautils-0.1.6/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-05-19 02:09:15.000000 dknovautils-0.1.6/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-05-19 02:09:15.000000 dknovautils-0.1.6/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-19 02:09:15.000000 dknovautils-0.1.6/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.1.6/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-19 02:09:17.000000 dknovautils-0.1.6/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.1.6/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-05-19 02:09:17.000000 dknovautils-0.1.6/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1159 2023-05-19 02:09:12.000000 dknovautils-0.1.6/setup.py
```

### Comparing `dknovautils-0.1.5/dknovautils/commons.py` & `dknovautils-0.1.6/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.5/dknovautils/dkat.py` & `dknovautils-0.1.6/dknovautils/dkat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
+from typing import Any
 import dknovautils
 from dknovautils.commons import *
 
 
-DkAppVer = '0.1.5'
+DkAppVer = '0.1.6'
 
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
@@ -273,18 +274,18 @@
             dts = dts[:(10)]
         else:
             AT.never()
 
         return dts
 
     @staticmethod
-    def assert_(b: bool, s: str = None):
+    def assert_(b: Any, s: str = None):
         # 改成完善的形式
 
-        assert isinstance(b, bool)
+        # assert isinstance(b, bool)
 
         if b:
             return
 
         AT._AstErrorCnt_ += 1
         msg = _unknown_err if s is None else s
```

### Comparing `dknovautils-0.1.5/dknovautils/dkipy.py` & `dknovautils-0.1.6/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.5/dknovautils/dk_imports.py` & `dknovautils-0.1.6/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.5/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.1.6/dknovautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.1.5/PKG-INFO` & `dknovautils-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.1.5/setup.py` & `dknovautils-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.1.5'
+DkAppVer = '0.1.6'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

