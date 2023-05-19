# Comparing `tmp/libheader-1.0.2.tar.gz` & `tmp/libheader-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libheader-1.0.2.tar", last modified: Thu May 18 23:38:05 2023, max compression
+gzip compressed data, was "libheader-1.0.3.tar", last modified: Thu May 18 23:54:03 2023, max compression
```

## Comparing `libheader-1.0.2.tar` & `libheader-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:38:05.327624 libheader-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-18 23:38:05.327624 libheader-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-18 23:37:49.000000 libheader-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:38:05.323624 libheader-1.0.2/libheader/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-18 23:37:49.000000 libheader-1.0.2/libheader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-18 23:37:49.000000 libheader-1.0.2/libheader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-18 23:37:49.000000 libheader-1.0.2/libheader/gcclh.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-18 23:37:49.000000 libheader-1.0.2/libheader/lh.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-18 23:37:49.000000 libheader-1.0.2/libheader/makelh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:38:05.327624 libheader-1.0.2/libheader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-18 23:38:05.000000 libheader-1.0.2/libheader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-18 23:38:05.000000 libheader-1.0.2/libheader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:38:05.000000 libheader-1.0.2/libheader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 23:38:05.000000 libheader-1.0.2/libheader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:38:05.327624 libheader-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-18 23:37:49.000000 libheader-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:54:03.082989 libheader-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-18 23:54:03.082989 libheader-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-18 23:53:52.000000 libheader-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:54:03.082989 libheader-1.0.3/libheader/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 23:53:52.000000 libheader-1.0.3/libheader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-18 23:53:52.000000 libheader-1.0.3/libheader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-18 23:53:52.000000 libheader-1.0.3/libheader/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-18 23:53:52.000000 libheader-1.0.3/libheader/gcclh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-18 23:53:52.000000 libheader-1.0.3/libheader/lh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-18 23:53:52.000000 libheader-1.0.3/libheader/makelh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:54:03.082989 libheader-1.0.3/libheader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-18 23:54:03.000000 libheader-1.0.3/libheader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 23:54:03.000000 libheader-1.0.3/libheader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:54:03.000000 libheader-1.0.3/libheader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 23:54:03.000000 libheader-1.0.3/libheader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:54:03.082989 libheader-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-18 23:53:52.000000 libheader-1.0.3/setup.py
```

### Comparing `libheader-1.0.2/PKG-INFO` & `libheader-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libheader
-Version: 1.0.2
+Version: 1.0.3
 Summary: A new file format that makes C easier.
 Home-page: https://github.com/wk1093/libheader
 Author: Wyatt Kloos
 Author-email: wyattk1093@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `libheader-1.0.2/README.md` & `libheader-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `libheader-1.0.2/libheader/gcclh.py` & `libheader-1.0.3/libheader/gcclh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!python3
-from libheader import lh
+from . import lh
 import os
 import sys
 
 # forward all arguments to gcc, other than custom libs: '--lh=[filename]' if there are spaces in the filename, they must be in quotes
 gccargs = sys.argv[1:]
 customlibs = []
```

### Comparing `libheader-1.0.2/libheader.egg-info/PKG-INFO` & `libheader-1.0.3/libheader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libheader
-Version: 1.0.2
+Version: 1.0.3
 Summary: A new file format that makes C easier.
 Home-page: https://github.com/wk1093/libheader
 Author: Wyatt Kloos
 Author-email: wyattk1093@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `libheader-1.0.2/setup.py` & `libheader-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='libheader',
-    version='1.0.2',    
+    version='1.0.3',    
     description='A new file format that makes C easier.',
     url='https://github.com/wk1093/libheader',
     author='Wyatt Kloos',
     author_email='wyattk1093@gmail.com',
     license='BSD 2-clause',
     packages=['libheader'],
     install_requires=[],
```

