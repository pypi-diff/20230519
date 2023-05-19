# Comparing `tmp/diamond_env-1.0.1.tar.gz` & `tmp/diamond_env-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diamond_env-1.0.1.tar", last modified: Thu May 18 16:04:59 2023, max compression
+gzip compressed data, was "diamond_env-1.0.2.tar", last modified: Fri May 19 14:44:27 2023, max compression
```

## Comparing `diamond_env-1.0.1.tar` & `diamond_env-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-18 16:04:59.674952 diamond_env-1.0.1/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1062 2023-05-18 14:55:53.000000 diamond_env-1.0.1/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5390 2023-05-18 16:04:59.674952 diamond_env-1.0.1/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4949 2023-05-18 16:04:31.000000 diamond_env-1.0.1/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-18 16:04:59.670952 diamond_env-1.0.1/diamond_env/
--rw-r-----   0 danijar  (322066) primarygroup (89939)       57 2023-05-18 14:33:21.000000 diamond_env-1.0.1/diamond_env/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5381 2023-05-18 15:13:47.000000 diamond_env-1.0.1/diamond_env/adapters.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3355 2023-05-18 14:36:03.000000 diamond_env-1.0.1/diamond_env/backend.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6588 2023-05-18 15:02:35.000000 diamond_env-1.0.1/diamond_env/env.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3552 2023-05-18 13:43:21.000000 diamond_env-1.0.1/diamond_env/space.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3094 2023-05-18 15:02:53.000000 diamond_env-1.0.1/diamond_env/task.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2260 2023-05-18 15:03:50.000000 diamond_env-1.0.1/diamond_env/wrappers.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-18 16:04:59.670952 diamond_env-1.0.1/diamond_env.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5390 2023-05-18 16:04:59.000000 diamond_env-1.0.1/diamond_env.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      355 2023-05-18 16:04:59.000000 diamond_env-1.0.1/diamond_env.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-05-18 16:04:59.000000 diamond_env-1.0.1/diamond_env.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       70 2023-05-18 16:04:59.000000 diamond_env-1.0.1/diamond_env.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       22 2023-05-18 16:04:59.000000 diamond_env-1.0.1/diamond_env.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-05-18 16:04:59.674952 diamond_env-1.0.1/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)      791 2023-05-18 16:04:49.000000 diamond_env-1.0.1/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 14:44:27.127121 diamond_env-1.0.2/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1062 2023-05-18 14:55:53.000000 diamond_env-1.0.2/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2023-05-19 14:43:53.000000 diamond_env-1.0.2/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5390 2023-05-19 14:44:27.127121 diamond_env-1.0.2/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4949 2023-05-18 16:04:31.000000 diamond_env-1.0.2/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 14:44:27.123121 diamond_env-1.0.2/diamond_env/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       57 2023-05-18 14:33:21.000000 diamond_env-1.0.2/diamond_env/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5381 2023-05-18 15:13:47.000000 diamond_env-1.0.2/diamond_env/adapters.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3355 2023-05-18 14:36:03.000000 diamond_env-1.0.2/diamond_env/backend.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6588 2023-05-18 15:02:35.000000 diamond_env-1.0.2/diamond_env/env.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3552 2023-05-18 13:43:21.000000 diamond_env-1.0.2/diamond_env/space.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3094 2023-05-18 15:02:53.000000 diamond_env-1.0.2/diamond_env/task.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2260 2023-05-18 15:03:50.000000 diamond_env-1.0.2/diamond_env/wrappers.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 14:44:27.127121 diamond_env-1.0.2/diamond_env.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5390 2023-05-19 14:44:27.000000 diamond_env-1.0.2/diamond_env.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      384 2023-05-19 14:44:27.000000 diamond_env-1.0.2/diamond_env.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-05-19 14:44:27.000000 diamond_env-1.0.2/diamond_env.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       70 2023-05-19 14:44:27.000000 diamond_env-1.0.2/diamond_env.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       22 2023-05-19 14:44:27.000000 diamond_env-1.0.2/diamond_env.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       71 2023-05-18 16:00:58.000000 diamond_env-1.0.2/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-05-19 14:44:27.127121 diamond_env-1.0.2/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      791 2023-05-19 14:43:58.000000 diamond_env-1.0.2/setup.py
```

### Comparing `diamond_env-1.0.1/LICENSE` & `diamond_env-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.1/PKG-INFO` & `diamond_env-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamond_env
-Version: 1.0.1
+Version: 1.0.2
 Summary: Minecraft Diamond Env
 Home-page: http://github.com/danijar/diamond_env
 Author: Danijar Hafner
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `diamond_env-1.0.1/README.md` & `diamond_env-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.1/diamond_env/adapters.py` & `diamond_env-1.0.2/diamond_env/adapters.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.1/diamond_env/backend.py` & `diamond_env-1.0.2/diamond_env/backend.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.1/diamond_env/env.py` & `diamond_env-1.0.2/diamond_env/env.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.1/diamond_env/space.py` & `diamond_env-1.0.2/diamond_env/space.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.1/diamond_env/task.py` & `diamond_env-1.0.2/diamond_env/task.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.1/diamond_env/wrappers.py` & `diamond_env-1.0.2/diamond_env/wrappers.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.1/diamond_env.egg-info/PKG-INFO` & `diamond_env-1.0.2/diamond_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamond-env
-Version: 1.0.1
+Version: 1.0.2
 Summary: Minecraft Diamond Env
 Home-page: http://github.com/danijar/diamond_env
 Author: Danijar Hafner
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `diamond_env-1.0.1/setup.py` & `diamond_env-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 import setuptools
 from setuptools import find_namespace_packages
 
 
 setuptools.setup(
     name='diamond_env',
-    version='1.0.1',
+    version='1.0.2',
     description='Minecraft Diamond Env',
     author='Danijar Hafner',
     url='http://github.com/danijar/diamond_env',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(exclude=['example.py']),
     include_package_data=True,
```

