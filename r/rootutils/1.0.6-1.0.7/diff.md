# Comparing `tmp/rootutils-1.0.6.tar.gz` & `tmp/rootutils-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootutils-1.0.6.tar", last modified: Sat May 13 17:54:25 2023, max compression
+gzip compressed data, was "rootutils-1.0.7.tar", last modified: Fri May 19 13:05:07 2023, max compression
```

## Comparing `rootutils-1.0.6.tar` & `rootutils-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:54:25.455986 rootutils-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-13 17:54:12.000000 rootutils-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-13 17:54:25.455986 rootutils-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-13 17:54:12.000000 rootutils-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-13 17:54:12.000000 rootutils-1.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:54:25.455986 rootutils-1.0.6/rootutils/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-13 17:54:12.000000 rootutils-1.0.6/rootutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-13 17:54:12.000000 rootutils-1.0.6/rootutils/rootutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:54:25.455986 rootutils-1.0.6/rootutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-13 17:54:25.000000 rootutils-1.0.6/rootutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-13 17:54:25.000000 rootutils-1.0.6/rootutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:54:25.000000 rootutils-1.0.6/rootutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-13 17:54:25.000000 rootutils-1.0.6/rootutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-13 17:54:25.000000 rootutils-1.0.6/rootutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 17:54:25.455986 rootutils-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-13 17:54:12.000000 rootutils-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:54:25.455986 rootutils-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 17:54:12.000000 rootutils-1.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 17:54:12.000000 rootutils-1.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-13 17:54:12.000000 rootutils-1.0.6/tests/test_rootutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:05:07.055478 rootutils-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 13:04:50.000000 rootutils-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-19 13:05:07.055478 rootutils-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-19 13:04:50.000000 rootutils-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-19 13:04:50.000000 rootutils-1.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:05:07.051478 rootutils-1.0.7/rootutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-19 13:04:50.000000 rootutils-1.0.7/rootutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-19 13:04:50.000000 rootutils-1.0.7/rootutils/rootutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:05:07.051478 rootutils-1.0.7/rootutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-19 13:05:07.000000 rootutils-1.0.7/rootutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-19 13:05:07.000000 rootutils-1.0.7/rootutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:05:07.000000 rootutils-1.0.7/rootutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 13:05:07.000000 rootutils-1.0.7/rootutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 13:05:07.000000 rootutils-1.0.7/rootutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:05:07.055478 rootutils-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-19 13:04:50.000000 rootutils-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:05:07.055478 rootutils-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:04:50.000000 rootutils-1.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:04:50.000000 rootutils-1.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-19 13:04:50.000000 rootutils-1.0.7/tests/test_rootutils.py
```

### Comparing `rootutils-1.0.6/LICENSE` & `rootutils-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rootutils-1.0.6/PKG-INFO` & `rootutils-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootutils
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple package for easy project root setup
 Home-page: https://github.com/ashleve/rootutils
 Author: ashleve
 Author-email: ashlevegalaxy@gmail.com
 License: MIT
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `rootutils-1.0.6/README.md` & `rootutils-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rootutils-1.0.6/rootutils/rootutils.py` & `rootutils-1.0.7/rootutils/rootutils.py`

 * *Files identical despite different names*

### Comparing `rootutils-1.0.6/rootutils.egg-info/PKG-INFO` & `rootutils-1.0.7/rootutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootutils
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple package for easy project root setup
 Home-page: https://github.com/ashleve/rootutils
 Author: ashleve
 Author-email: ashlevegalaxy@gmail.com
 License: MIT
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `rootutils-1.0.6/setup.py` & `rootutils-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="rootutils",
-    version="1.0.6",
+    version="1.0.7",
     license="MIT",
     description="Simple package for easy project root setup",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ashleve/rootutils",
     author="ashleve",
     author_email="ashlevegalaxy@gmail.com",
```

### Comparing `rootutils-1.0.6/tests/test_rootutils.py` & `rootutils-1.0.7/tests/test_rootutils.py`

 * *Files identical despite different names*

