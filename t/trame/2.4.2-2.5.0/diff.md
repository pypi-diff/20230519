# Comparing `tmp/trame-2.4.2.tar.gz` & `tmp/trame-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-2.4.2.tar", last modified: Thu May 11 14:41:33 2023, max compression
+gzip compressed data, was "trame-2.5.0.tar", last modified: Fri May 19 01:00:04 2023, max compression
```

## Comparing `trame-2.4.2.tar` & `trame-2.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:41:33.780425 trame-2.4.2/
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-11 14:41:28.000000 trame-2.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 14:41:28.000000 trame-2.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6855 2023-05-11 14:41:33.780425 trame-2.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6117 2023-05-11 14:41:28.000000 trame-2.4.2/README.rst
--rw-r--r--   0 root         (0) root         (0)     1151 2023-05-11 14:41:33.780425 trame-2.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 14:41:28.000000 trame-2.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:41:33.772425 trame-2.4.2/trame/
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-11 14:41:28.000000 trame-2.4.2/trame/LICENSE
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-11 14:41:28.000000 trame-2.4.2/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:41:33.776425 trame-2.4.2/trame/app/
--rw-r--r--   0 root         (0) root         (0)     2388 2023-05-11 14:41:28.000000 trame-2.4.2/trame/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-05-11 14:41:28.000000 trame-2.4.2/trame/app/asynchronous.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-05-11 14:41:28.000000 trame-2.4.2/trame/app/demo.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-05-11 14:41:28.000000 trame-2.4.2/trame/app/dev.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-11 14:41:28.000000 trame-2.4.2/trame/app/file_upload.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-05-11 14:41:28.000000 trame-2.4.2/trame/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-05-11 14:41:28.000000 trame-2.4.2/trame/app/mimetypes.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-05-11 14:41:28.000000 trame-2.4.2/trame/app/singleton.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-05-11 14:41:28.000000 trame-2.4.2/trame/app/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:41:33.776425 trame-2.4.2/trame/assets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 14:41:28.000000 trame-2.4.2/trame/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4337 2023-05-11 14:41:28.000000 trame-2.4.2/trame/assets/local.py
--rw-r--r--   0 root         (0) root         (0)     4362 2023-05-11 14:41:28.000000 trame-2.4.2/trame/assets/remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:41:33.780425 trame-2.4.2/trame/env/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 14:41:28.000000 trame-2.4.2/trame/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-05-11 14:41:28.000000 trame-2.4.2/trame/env/paraview.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-05-11 14:41:28.000000 trame-2.4.2/trame/env/utils.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-05-11 14:41:28.000000 trame-2.4.2/trame/env/venv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:41:33.780425 trame-2.4.2/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 14:41:28.000000 trame-2.4.2/trame/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:41:33.780425 trame-2.4.2/trame/tools/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 14:41:28.000000 trame-2.4.2/trame/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-05-11 14:41:28.000000 trame-2.4.2/trame/tools/app.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-05-11 14:41:28.000000 trame-2.4.2/trame/tools/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:41:33.780425 trame-2.4.2/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-11 14:41:28.000000 trame-2.4.2/trame/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:41:33.780425 trame-2.4.2/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 14:41:28.000000 trame-2.4.2/trame/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:41:33.772425 trame-2.4.2/trame.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6855 2023-05-11 14:41:33.000000 trame-2.4.2/trame.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      707 2023-05-11 14:41:33.000000 trame-2.4.2/trame.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 14:41:33.000000 trame-2.4.2/trame.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      260 2023-05-11 14:41:33.000000 trame-2.4.2/trame.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-11 14:41:33.000000 trame-2.4.2/trame.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:00:04.598214 trame-2.5.0/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-19 00:59:59.000000 trame-2.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 00:59:59.000000 trame-2.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6855 2023-05-19 01:00:04.598214 trame-2.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6117 2023-05-19 00:59:59.000000 trame-2.5.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-05-19 01:00:04.598214 trame-2.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 00:59:59.000000 trame-2.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:00:04.590214 trame-2.5.0/trame/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-19 00:59:59.000000 trame-2.5.0/trame/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-19 00:59:59.000000 trame-2.5.0/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:00:04.594214 trame-2.5.0/trame/app/
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-05-19 00:59:59.000000 trame-2.5.0/trame/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-05-19 00:59:59.000000 trame-2.5.0/trame/app/asynchronous.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-05-19 00:59:59.000000 trame-2.5.0/trame/app/demo.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-05-19 00:59:59.000000 trame-2.5.0/trame/app/dev.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-19 00:59:59.000000 trame-2.5.0/trame/app/file_upload.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-05-19 00:59:59.000000 trame-2.5.0/trame/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-05-19 00:59:59.000000 trame-2.5.0/trame/app/mimetypes.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-05-19 00:59:59.000000 trame-2.5.0/trame/app/singleton.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-05-19 00:59:59.000000 trame-2.5.0/trame/app/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:00:04.594214 trame-2.5.0/trame/assets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-19 00:59:59.000000 trame-2.5.0/trame/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4337 2023-05-19 00:59:59.000000 trame-2.5.0/trame/assets/local.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-05-19 00:59:59.000000 trame-2.5.0/trame/assets/remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:00:04.594214 trame-2.5.0/trame/env/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 00:59:59.000000 trame-2.5.0/trame/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-05-19 00:59:59.000000 trame-2.5.0/trame/env/paraview.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-05-19 00:59:59.000000 trame-2.5.0/trame/env/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-05-19 00:59:59.000000 trame-2.5.0/trame/env/venv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:00:04.594214 trame-2.5.0/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-19 00:59:59.000000 trame-2.5.0/trame/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:00:04.598214 trame-2.5.0/trame/tools/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-19 00:59:59.000000 trame-2.5.0/trame/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-05-19 00:59:59.000000 trame-2.5.0/trame/tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-05-19 00:59:59.000000 trame-2.5.0/trame/tools/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:00:04.598214 trame-2.5.0/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-19 00:59:59.000000 trame-2.5.0/trame/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:00:04.598214 trame-2.5.0/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-19 00:59:59.000000 trame-2.5.0/trame/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:00:04.590214 trame-2.5.0/trame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6855 2023-05-19 01:00:04.000000 trame-2.5.0/trame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      707 2023-05-19 01:00:04.000000 trame-2.5.0/trame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 01:00:04.000000 trame-2.5.0/trame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      253 2023-05-19 01:00:04.000000 trame-2.5.0/trame.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-19 01:00:04.000000 trame-2.5.0/trame.egg-info/top_level.txt
```

### Comparing `trame-2.4.2/LICENSE` & `trame-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/PKG-INFO` & `trame-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 2.4.2
+Version: 2.5.0
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-2.4.2/README.rst` & `trame-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/LICENSE` & `trame-2.5.0/trame/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/app/__init__.py` & `trame-2.5.0/trame/app/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/app/demo.py` & `trame-2.5.0/trame/app/demo.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/app/dev.py` & `trame-2.5.0/trame/app/dev.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/app/file_upload.py` & `trame-2.5.0/trame/app/file_upload.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/app/jupyter.py` & `trame-2.5.0/trame/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/app/mimetypes.py` & `trame-2.5.0/trame/app/mimetypes.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/app/singleton.py` & `trame-2.5.0/trame/app/singleton.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/app/testing.py` & `trame-2.5.0/trame/app/testing.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/assets/local.py` & `trame-2.5.0/trame/assets/local.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/assets/remote.py` & `trame-2.5.0/trame/assets/remote.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/env/paraview.py` & `trame-2.5.0/trame/env/paraview.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/env/utils.py` & `trame-2.5.0/trame/env/utils.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/env/venv.py` & `trame-2.5.0/trame/env/venv.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/tools/app.py` & `trame-2.5.0/trame/tools/app.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame/tools/www.py` & `trame-2.5.0/trame/tools/www.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.2/trame.egg-info/PKG-INFO` & `trame-2.5.0/trame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 2.4.2
+Version: 2.5.0
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-2.4.2/trame.egg-info/SOURCES.txt` & `trame-2.5.0/trame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

