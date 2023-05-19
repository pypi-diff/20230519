# Comparing `tmp/pytest-vulture-2.0.2.tar.gz` & `tmp/pytest-vulture-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-vulture-2.0.2.tar", last modified: Wed Oct 12 14:16:16 2022, max compression
+gzip compressed data, was "pytest-vulture-2.1.0.tar", last modified: Fri May 19 14:53:15 2023, max compression
```

## Comparing `pytest-vulture-2.0.2.tar` & `pytest-vulture-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-10-12 14:16:16.163218 pytest-vulture-2.0.2/
--rw-rw-r--   0 root         (0) root         (0)     1068 2022-10-04 08:10:30.000000 pytest-vulture-2.0.2/LICENSE
--rw-rw-r--   0 root         (0) root         (0)     2502 2022-10-12 14:16:16.163218 pytest-vulture-2.0.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2046 2022-10-12 14:10:16.000000 pytest-vulture-2.0.2/README.rst
--rw-rw-r--   0 root         (0) root         (0)      647 2022-10-12 14:16:16.163218 pytest-vulture-2.0.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1647 2022-10-12 13:56:29.000000 pytest-vulture-2.0.2/setup.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-10-12 14:16:16.159218 pytest-vulture-2.0.2/src/
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-10-12 14:16:16.163218 pytest-vulture-2.0.2/src/pytest_vulture/
--rw-rw-r--   0 root         (0) root         (0)      557 2022-10-04 08:10:30.000000 pytest-vulture-2.0.2/src/pytest_vulture/__init__.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-10-12 14:16:16.163218 pytest-vulture-2.0.2/src/pytest_vulture/conf/
--rw-rw-r--   0 root         (0) root         (0)       66 2022-10-04 08:10:30.000000 pytest-vulture-2.0.2/src/pytest_vulture/conf/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      951 2022-10-11 15:38:28.000000 pytest-vulture-2.0.2/src/pytest_vulture/conf/base.py
--rw-rw-r--   0 root         (0) root         (0)     1404 2022-10-11 15:38:28.000000 pytest-vulture-2.0.2/src/pytest_vulture/conf/package.py
--rw-rw-r--   0 root         (0) root         (0)     1608 2022-10-11 15:36:03.000000 pytest-vulture-2.0.2/src/pytest_vulture/conf/reader.py
--rw-rw-r--   0 root         (0) root         (0)     2657 2022-10-11 15:38:28.000000 pytest-vulture-2.0.2/src/pytest_vulture/conf/vulture.py
--rw-rw-r--   0 root         (0) root         (0)     2509 2022-10-12 14:07:59.000000 pytest-vulture-2.0.2/src/pytest_vulture/plugin.py
--rw-rw-r--   0 root         (0) root         (0)     6101 2022-10-12 12:45:02.000000 pytest-vulture-2.0.2/src/pytest_vulture/setup_manager.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-10-12 14:16:16.163218 pytest-vulture-2.0.2/src/pytest_vulture/vulture/
--rw-rw-r--   0 root         (0) root         (0)       22 2022-10-04 08:10:30.000000 pytest-vulture-2.0.2/src/pytest_vulture/vulture/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3467 2022-10-12 12:45:02.000000 pytest-vulture-2.0.2/src/pytest_vulture/vulture/comment.py
--rw-rw-r--   0 root         (0) root         (0)     4101 2022-10-12 12:45:02.000000 pytest-vulture-2.0.2/src/pytest_vulture/vulture/manager.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-10-12 14:16:16.163218 pytest-vulture-2.0.2/src/pytest_vulture.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     2502 2022-10-12 14:16:16.000000 pytest-vulture-2.0.2/src/pytest_vulture.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      674 2022-10-12 14:16:16.000000 pytest-vulture-2.0.2/src/pytest_vulture.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2022-10-12 14:16:16.000000 pytest-vulture-2.0.2/src/pytest_vulture.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       43 2022-10-12 14:16:16.000000 pytest-vulture-2.0.2/src/pytest_vulture.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)      392 2022-10-12 14:16:16.000000 pytest-vulture-2.0.2/src/pytest_vulture.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       15 2022-10-12 14:16:16.000000 pytest-vulture-2.0.2/src/pytest_vulture.egg-info/top_level.txt
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/
+-rw-rw-r--   0 root         (0) root         (0)     1068 2022-10-04 08:10:30.000000 pytest-vulture-2.1.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     2502 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2046 2022-10-12 14:10:16.000000 pytest-vulture-2.1.0/README.rst
+-rw-rw-r--   0 root         (0) root         (0)      647 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1648 2023-05-19 14:50:10.000000 pytest-vulture-2.1.0/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/src/
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/src/pytest_vulture/
+-rw-rw-r--   0 root         (0) root         (0)      557 2022-10-04 08:10:30.000000 pytest-vulture-2.1.0/src/pytest_vulture/__init__.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/src/pytest_vulture/conf/
+-rw-rw-r--   0 root         (0) root         (0)       66 2022-10-04 08:10:30.000000 pytest-vulture-2.1.0/src/pytest_vulture/conf/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      951 2022-10-11 15:38:28.000000 pytest-vulture-2.1.0/src/pytest_vulture/conf/base.py
+-rw-rw-r--   0 root         (0) root         (0)     1626 2023-05-19 14:50:10.000000 pytest-vulture-2.1.0/src/pytest_vulture/conf/package.py
+-rw-rw-r--   0 root         (0) root         (0)     1608 2022-10-11 15:36:03.000000 pytest-vulture-2.1.0/src/pytest_vulture/conf/reader.py
+-rw-rw-r--   0 root         (0) root         (0)     2657 2022-10-11 15:38:28.000000 pytest-vulture-2.1.0/src/pytest_vulture/conf/vulture.py
+-rw-rw-r--   0 root         (0) root         (0)     2509 2022-10-12 14:07:59.000000 pytest-vulture-2.1.0/src/pytest_vulture/plugin.py
+-rw-rw-r--   0 root         (0) root         (0)     6851 2023-05-19 14:50:10.000000 pytest-vulture-2.1.0/src/pytest_vulture/setup_manager.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/src/pytest_vulture/vulture/
+-rw-rw-r--   0 root         (0) root         (0)       22 2022-10-04 08:10:30.000000 pytest-vulture-2.1.0/src/pytest_vulture/vulture/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3471 2023-05-19 14:50:10.000000 pytest-vulture-2.1.0/src/pytest_vulture/vulture/comment.py
+-rw-rw-r--   0 root         (0) root         (0)     4101 2022-10-12 12:45:02.000000 pytest-vulture-2.1.0/src/pytest_vulture/vulture/manager.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-19 14:53:15.718685 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     2502 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      674 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       43 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)      392 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       15 2023-05-19 14:53:15.000000 pytest-vulture-2.1.0/src/pytest_vulture.egg-info/top_level.txt
```

### Comparing `pytest-vulture-2.0.2/LICENSE` & `pytest-vulture-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.0.2/PKG-INFO` & `pytest-vulture-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-vulture
-Version: 2.0.2
+Version: 2.1.0
 Summary: A pytest plugin to checks dead code with vulture
 Home-page: https://github.com/Gatewatcher/pytest-vulture
 Author: Abadie Moran
 Author-email: moran.abadie@gatewatcher.com
 Maintainer: Abadie Moran
 Maintainer-email: moran.abadie@gatewatcher.com
 License: MIT
```

### Comparing `pytest-vulture-2.0.2/README.rst` & `pytest-vulture-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.0.2/setup.cfg` & `pytest-vulture-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.0.2/setup.py` & `pytest-vulture-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """pytest-vulture
 =============
 Plugin for py.test for doing vulture tests
 """
 import os
+
 from pathlib import Path
 
 from setuptools import (
     find_packages,
     setup,
 )
 
@@ -40,15 +41,15 @@
     "pytest11": [
         "vulture = pytest_vulture.plugin",
     ]
 } if not IS_TEST else {}
 
 setup(
     name='pytest-vulture',
-    version='2.0.2',
+    version='2.1.0',
     include_package_data=True,
     author='Abadie Moran',
     author_email='moran.abadie@gatewatcher.com',
     maintainer='Abadie Moran',
     maintainer_email='moran.abadie@gatewatcher.com',
     license='MIT',
     url='https://github.com/Gatewatcher/pytest-vulture',
```

### Comparing `pytest-vulture-2.0.2/src/pytest_vulture/__init__.py` & `pytest-vulture-2.1.0/src/pytest_vulture/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.0.2/src/pytest_vulture/conf/base.py` & `pytest-vulture-2.1.0/src/pytest_vulture/conf/base.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.0.2/src/pytest_vulture/conf/reader.py` & `pytest-vulture-2.1.0/src/pytest_vulture/conf/reader.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.0.2/src/pytest_vulture/conf/vulture.py` & `pytest-vulture-2.1.0/src/pytest_vulture/conf/vulture.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.0.2/src/pytest_vulture/plugin.py` & `pytest-vulture-2.1.0/src/pytest_vulture/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.0.2/src/pytest_vulture/vulture/comment.py` & `pytest-vulture-2.1.0/src/pytest_vulture/vulture/comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         except AttributeError:
             return 0
 
     def __reset(self, path: Path):
         self._path = path
         self._ignored_lines = []
         try:
-            self._content = self._path.read_text(encoding="utf-8")
+            self._content = self._path.read_text(encoding="utf-8-sig")
             self._tree = ast.parse(self._content)
             content_split = self._content.split("\n")
             index_line = 0
             for elem in content_split:
                 if self._VULTURE_IGNORE in elem:
                     self._ignored_lines.append(index_line + 1)
                 index_line += 1
```

### Comparing `pytest-vulture-2.0.2/src/pytest_vulture/vulture/manager.py` & `pytest-vulture-2.1.0/src/pytest_vulture/vulture/manager.py`

 * *Files identical despite different names*

### Comparing `pytest-vulture-2.0.2/src/pytest_vulture.egg-info/PKG-INFO` & `pytest-vulture-2.1.0/src/pytest_vulture.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-vulture
-Version: 2.0.2
+Version: 2.1.0
 Summary: A pytest plugin to checks dead code with vulture
 Home-page: https://github.com/Gatewatcher/pytest-vulture
 Author: Abadie Moran
 Author-email: moran.abadie@gatewatcher.com
 Maintainer: Abadie Moran
 Maintainer-email: moran.abadie@gatewatcher.com
 License: MIT
```

### Comparing `pytest-vulture-2.0.2/src/pytest_vulture.egg-info/SOURCES.txt` & `pytest-vulture-2.1.0/src/pytest_vulture.egg-info/SOURCES.txt`

 * *Files identical despite different names*

