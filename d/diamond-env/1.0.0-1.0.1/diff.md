# Comparing `tmp/diamond_env-1.0.0.tar.gz` & `tmp/diamond_env-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diamond_env-1.0.0.tar", last modified: Thu May 18 16:01:53 2023, max compression
+gzip compressed data, was "diamond_env-1.0.1.tar", last modified: Thu May 18 16:04:59 2023, max compression
```

## Comparing `diamond_env-1.0.0.tar` & `diamond_env-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-18 16:01:53.231707 diamond_env-1.0.0/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1062 2023-05-18 14:55:53.000000 diamond_env-1.0.0/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5390 2023-05-18 16:01:53.231707 diamond_env-1.0.0/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4949 2023-05-18 15:59:28.000000 diamond_env-1.0.0/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-18 16:01:53.231707 diamond_env-1.0.0/diamond_env/
--rw-r-----   0 danijar  (322066) primarygroup (89939)       57 2023-05-18 14:33:21.000000 diamond_env-1.0.0/diamond_env/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5381 2023-05-18 15:13:47.000000 diamond_env-1.0.0/diamond_env/adapters.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3355 2023-05-18 14:36:03.000000 diamond_env-1.0.0/diamond_env/backend.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6588 2023-05-18 15:02:35.000000 diamond_env-1.0.0/diamond_env/env.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3552 2023-05-18 13:43:21.000000 diamond_env-1.0.0/diamond_env/space.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3094 2023-05-18 15:02:53.000000 diamond_env-1.0.0/diamond_env/task.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2260 2023-05-18 15:03:50.000000 diamond_env-1.0.0/diamond_env/wrappers.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-18 16:01:53.231707 diamond_env-1.0.0/diamond_env.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5390 2023-05-18 16:01:53.000000 diamond_env-1.0.0/diamond_env.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      355 2023-05-18 16:01:53.000000 diamond_env-1.0.0/diamond_env.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-05-18 16:01:53.000000 diamond_env-1.0.0/diamond_env.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       70 2023-05-18 16:01:53.000000 diamond_env-1.0.0/diamond_env.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       22 2023-05-18 16:01:53.000000 diamond_env-1.0.0/diamond_env.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-05-18 16:01:53.231707 diamond_env-1.0.0/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)      791 2023-05-18 16:01:40.000000 diamond_env-1.0.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-18 16:04:59.674952 diamond_env-1.0.1/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1062 2023-05-18 14:55:53.000000 diamond_env-1.0.1/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5390 2023-05-18 16:04:59.674952 diamond_env-1.0.1/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4949 2023-05-18 16:04:31.000000 diamond_env-1.0.1/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-18 16:04:59.670952 diamond_env-1.0.1/diamond_env/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       57 2023-05-18 14:33:21.000000 diamond_env-1.0.1/diamond_env/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5381 2023-05-18 15:13:47.000000 diamond_env-1.0.1/diamond_env/adapters.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3355 2023-05-18 14:36:03.000000 diamond_env-1.0.1/diamond_env/backend.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6588 2023-05-18 15:02:35.000000 diamond_env-1.0.1/diamond_env/env.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3552 2023-05-18 13:43:21.000000 diamond_env-1.0.1/diamond_env/space.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3094 2023-05-18 15:02:53.000000 diamond_env-1.0.1/diamond_env/task.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2260 2023-05-18 15:03:50.000000 diamond_env-1.0.1/diamond_env/wrappers.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-18 16:04:59.670952 diamond_env-1.0.1/diamond_env.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5390 2023-05-18 16:04:59.000000 diamond_env-1.0.1/diamond_env.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      355 2023-05-18 16:04:59.000000 diamond_env-1.0.1/diamond_env.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-05-18 16:04:59.000000 diamond_env-1.0.1/diamond_env.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       70 2023-05-18 16:04:59.000000 diamond_env-1.0.1/diamond_env.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       22 2023-05-18 16:04:59.000000 diamond_env-1.0.1/diamond_env.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-05-18 16:04:59.674952 diamond_env-1.0.1/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      791 2023-05-18 16:04:49.000000 diamond_env-1.0.1/setup.py
```

### Comparing `diamond_env-1.0.0/LICENSE` & `diamond_env-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.0/PKG-INFO` & `diamond_env-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamond_env
-Version: 1.0.0
+Version: 1.0.1
 Summary: Minecraft Diamond Env
 Home-page: http://github.com/danijar/diamond_env
 Author: Danijar Hafner
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -21,15 +21,15 @@
 The Minecraft Diamond Environment used by
 [DreamerV3](https://danijar.com/dreamerv3), the first reinforcement learning
 algorithm to collect diamonds in Minecraft without human data or manually
 crafter curricula. We propose this environment as a standarized benchmark for
 reinforcement learning research that poses more interesting challenges than
 many of the popular existing benchmarks.
 
-![Minecraft Diamond Environment](https://github.com/danijar/diamond_env/assets/2111293/3643ab8e-7a3d-4cb8-a008-512ec34e3ba8)
+![Minecraft Diamond Environment](https://github.com/danijar/diamond_env/assets/2111293/4f5de275-7d84-4f6d-8515-ca2ee826ea9a)
 
 ## Overview
 
 In the Diamond Env, the agent plays Mincraft to accomplish 12 milestones
 leading up to collecting a diamond just from sparse rewards, which poses an
 exploration challenge. Moreover, each episode plays out in a unique randomly
 generated 3D world, requiring agents to generalize.
```

### Comparing `diamond_env-1.0.0/README.md` & `diamond_env-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 The Minecraft Diamond Environment used by
 [DreamerV3](https://danijar.com/dreamerv3), the first reinforcement learning
 algorithm to collect diamonds in Minecraft without human data or manually
 crafter curricula. We propose this environment as a standarized benchmark for
 reinforcement learning research that poses more interesting challenges than
 many of the popular existing benchmarks.
 
-![Minecraft Diamond Environment](https://github.com/danijar/diamond_env/assets/2111293/3643ab8e-7a3d-4cb8-a008-512ec34e3ba8)
+![Minecraft Diamond Environment](https://github.com/danijar/diamond_env/assets/2111293/4f5de275-7d84-4f6d-8515-ca2ee826ea9a)
 
 ## Overview
 
 In the Diamond Env, the agent plays Mincraft to accomplish 12 milestones
 leading up to collecting a diamond just from sparse rewards, which poses an
 exploration challenge. Moreover, each episode plays out in a unique randomly
 generated 3D world, requiring agents to generalize.
```

### Comparing `diamond_env-1.0.0/diamond_env/adapters.py` & `diamond_env-1.0.1/diamond_env/adapters.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.0/diamond_env/backend.py` & `diamond_env-1.0.1/diamond_env/backend.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.0/diamond_env/env.py` & `diamond_env-1.0.1/diamond_env/env.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.0/diamond_env/space.py` & `diamond_env-1.0.1/diamond_env/space.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.0/diamond_env/task.py` & `diamond_env-1.0.1/diamond_env/task.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.0/diamond_env/wrappers.py` & `diamond_env-1.0.1/diamond_env/wrappers.py`

 * *Files identical despite different names*

### Comparing `diamond_env-1.0.0/diamond_env.egg-info/PKG-INFO` & `diamond_env-1.0.1/diamond_env.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamond-env
-Version: 1.0.0
+Version: 1.0.1
 Summary: Minecraft Diamond Env
 Home-page: http://github.com/danijar/diamond_env
 Author: Danijar Hafner
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -21,15 +21,15 @@
 The Minecraft Diamond Environment used by
 [DreamerV3](https://danijar.com/dreamerv3), the first reinforcement learning
 algorithm to collect diamonds in Minecraft without human data or manually
 crafter curricula. We propose this environment as a standarized benchmark for
 reinforcement learning research that poses more interesting challenges than
 many of the popular existing benchmarks.
 
-![Minecraft Diamond Environment](https://github.com/danijar/diamond_env/assets/2111293/3643ab8e-7a3d-4cb8-a008-512ec34e3ba8)
+![Minecraft Diamond Environment](https://github.com/danijar/diamond_env/assets/2111293/4f5de275-7d84-4f6d-8515-ca2ee826ea9a)
 
 ## Overview
 
 In the Diamond Env, the agent plays Mincraft to accomplish 12 milestones
 leading up to collecting a diamond just from sparse rewards, which poses an
 exploration challenge. Moreover, each episode plays out in a unique randomly
 generated 3D world, requiring agents to generalize.
```

### Comparing `diamond_env-1.0.0/setup.py` & `diamond_env-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 import setuptools
 from setuptools import find_namespace_packages
 
 
 setuptools.setup(
     name='diamond_env',
-    version='1.0.0',
+    version='1.0.1',
     description='Minecraft Diamond Env',
     author='Danijar Hafner',
     url='http://github.com/danijar/diamond_env',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(exclude=['example.py']),
     include_package_data=True,
```

