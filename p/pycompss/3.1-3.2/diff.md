# Comparing `tmp/pycompss-3.1.tar.gz` & `tmp/pycompss-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompss-3.1.tar", last modified: Fri Nov 11 14:27:49 2022, max compression
+gzip compressed data, was "pycompss-3.2.tar", last modified: Fri May 19 12:44:38 2023, max compression
```

## Comparing `pycompss-3.1.tar` & `pycompss-3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-11-11 14:27:49.770184 pycompss-3.1/
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)    11406 2022-11-11 14:27:49.000000 pycompss-3.1/LICENSE.txt
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)      156 2022-11-11 14:27:49.000000 pycompss-3.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3658 2022-11-11 14:27:49.770184 pycompss-3.1/PKG-INFO
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     2044 2022-11-11 14:27:49.000000 pycompss-3.1/README.rst
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)        4 2022-11-11 14:27:49.000000 pycompss-3.1/VERSION.txt
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     9934 2022-11-11 14:27:49.000000 pycompss-3.1/backend.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-11-11 14:27:49.770184 pycompss-3.1/pycompss.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3658 2022-11-11 14:27:49.000000 pycompss-3.1/pycompss.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      241 2022-11-11 14:27:49.000000 pycompss-3.1/pycompss.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2022-11-11 14:27:49.000000 pycompss-3.1/pycompss.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)       11 2022-11-11 14:27:49.000000 pycompss-3.1/pycompss.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2022-11-11 14:27:49.000000 pycompss-3.1/pycompss.egg-info/top_level.txt
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     1535 2022-11-11 14:27:49.000000 pycompss-3.1/pycompssenv
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)       38 2022-11-11 14:27:49.770184 pycompss-3.1/setup.cfg
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     4859 2022-11-11 14:27:49.000000 pycompss-3.1/setup.py
--rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)       37 2022-11-11 14:27:49.000000 pycompss-3.1/url
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-19 12:44:38.295219 pycompss-3.2/
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)    11406 2023-05-19 12:44:38.000000 pycompss-3.2/LICENSE.txt
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)      156 2023-05-19 12:44:38.000000 pycompss-3.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3658 2023-05-19 12:44:38.295219 pycompss-3.2/PKG-INFO
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     2044 2023-05-19 12:44:38.000000 pycompss-3.2/README.rst
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)        4 2023-05-19 12:44:38.000000 pycompss-3.2/VERSION.txt
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     9934 2023-05-19 12:44:38.000000 pycompss-3.2/backend.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-19 12:44:38.295219 pycompss-3.2/pycompss.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3658 2023-05-19 12:44:38.000000 pycompss-3.2/pycompss.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      241 2023-05-19 12:44:38.000000 pycompss-3.2/pycompss.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-05-19 12:44:38.000000 pycompss-3.2/pycompss.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)       11 2023-05-19 12:44:38.000000 pycompss-3.2/pycompss.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-05-19 12:44:38.000000 pycompss-3.2/pycompss.egg-info/top_level.txt
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     1535 2023-05-19 12:44:38.000000 pycompss-3.2/pycompssenv
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)       38 2023-05-19 12:44:38.295219 pycompss-3.2/setup.cfg
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)     4859 2023-05-19 12:44:38.000000 pycompss-3.2/setup.py
+-rwxrwxrwx   0 jenkins   (1001) jenkins   (1001)       37 2023-05-19 12:44:38.000000 pycompss-3.2/url
```

### Comparing `pycompss-3.1/LICENSE.txt` & `pycompss-3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycompss-3.1/PKG-INFO` & `pycompss-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompss
-Version: 3.1
+Version: 3.2
 Summary: Python Binding for COMP Superscalar Runtime
 Home-page: http://compss.bsc.es
 Author: The COMPSs team
 Author-email: support-compss@bsc.es
 Maintainer: The COMPSs team
 Maintainer-email: support-compss@bsc.es
 License: Apache 2.0
```

### Comparing `pycompss-3.1/README.rst` & `pycompss-3.2/README.rst`

 * *Files identical despite different names*

### Comparing `pycompss-3.1/backend.py` & `pycompss-3.2/backend.py`

 * *Files identical despite different names*

### Comparing `pycompss-3.1/pycompss.egg-info/PKG-INFO` & `pycompss-3.2/pycompss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompss
-Version: 3.1
+Version: 3.2
 Summary: Python Binding for COMP Superscalar Runtime
 Home-page: http://compss.bsc.es
 Author: The COMPSs team
 Author-email: support-compss@bsc.es
 Maintainer: The COMPSs team
 Maintainer-email: support-compss@bsc.es
 License: Apache 2.0
```

### Comparing `pycompss-3.1/pycompssenv` & `pycompss-3.2/pycompssenv`

 * *Files identical despite different names*

### Comparing `pycompss-3.1/setup.py` & `pycompss-3.2/setup.py`

 * *Files identical despite different names*

