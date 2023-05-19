# Comparing `tmp/Signal8-1.6.tar.gz` & `tmp/Signal8-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-1.6.tar", last modified: Fri May 19 19:57:14 2023, max compression
+gzip compressed data, was "Signal8-1.7.tar", last modified: Fri May 19 20:00:02 2023, max compression
```

## Comparing `Signal8-1.6.tar` & `Signal8-1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 19:57:14.962546 Signal8-1.6/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.6/LICENSE
--rw-rw-rw-   0        0        0     4364 2023-05-19 19:57:14.960529 Signal8-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3876 2023-05-19 19:25:10.000000 Signal8-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 19:57:14.796539 Signal8-1.6/Signal8/
--rw-rw-rw-   0        0        0     6515 2023-05-19 19:55:48.000000 Signal8-1.6/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.6/Signal8/__init__.py
--rw-rw-rw-   0        0        0      130 2023-05-19 19:25:12.000000 Signal8-1.6/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:57:14.935530 Signal8-1.6/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.6/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     7867 2023-05-19 19:40:29.000000 Signal8-1.6/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2423 2023-05-19 19:25:16.000000 Signal8-1.6/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.6/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12174 2023-05-19 19:30:46.000000 Signal8-1.6/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:57:14.882531 Signal8-1.6/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4364 2023-05-19 19:57:14.000000 Signal8-1.6/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-19 19:57:14.000000 Signal8-1.6/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 19:57:14.000000 Signal8-1.6/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 19:57:14.000000 Signal8-1.6/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 19:57:14.962546 Signal8-1.6/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-05-19 19:57:08.000000 Signal8-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:00:02.033506 Signal8-1.7/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.7/LICENSE
+-rw-rw-rw-   0        0        0     4364 2023-05-19 20:00:02.032508 Signal8-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3876 2023-05-19 19:25:10.000000 Signal8-1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 20:00:01.972507 Signal8-1.7/Signal8/
+-rw-rw-rw-   0        0        0     6519 2023-05-19 19:59:38.000000 Signal8-1.7/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.7/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-05-19 19:25:12.000000 Signal8-1.7/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:00:02.027544 Signal8-1.7/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.7/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     7867 2023-05-19 19:40:29.000000 Signal8-1.7/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2423 2023-05-19 19:25:16.000000 Signal8-1.7/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.7/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12174 2023-05-19 19:30:46.000000 Signal8-1.7/Signal8/utils/simple_env.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:00:02.001507 Signal8-1.7/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4364 2023-05-19 20:00:01.000000 Signal8-1.7/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-19 20:00:01.000000 Signal8-1.7/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 20:00:01.000000 Signal8-1.7/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 20:00:01.000000 Signal8-1.7/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 20:00:02.034507 Signal8-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-05-19 19:59:53.000000 Signal8-1.7/setup.py
```

### Comparing `Signal8-1.6/LICENSE` & `Signal8-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-1.6/PKG-INFO` & `Signal8-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.6
+Version: 1.7
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-1.6/README.md` & `Signal8-1.7/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-1.6/Signal8/Signal8.py` & `Signal8-1.7/Signal8/Signal8.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 import numpy as np
 
 from gymnasium.utils import EzPickle
-from utils.scenario import BaseScenario
-from utils.core import Agent, Landmark, World, Action
-from utils.simple_env import SimpleEnv, make_env
-from utils.problems import get_problem, get_problem_list
+from .utils.scenario import BaseScenario
+from .utils.core import Agent, Landmark, World, Action
+from .utils.simple_env import SimpleEnv, make_env
+from .utils.problems import get_problem, get_problem_list
 
 class raw_env(SimpleEnv, EzPickle):
     def __init__(
         self, 
         agent_radius=0.1,
         num_obstacles=4,
         obstacle_radius=0.1,
```

### Comparing `Signal8-1.6/Signal8/utils/core.py` & `Signal8-1.7/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.6/Signal8/utils/problems.py` & `Signal8-1.7/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.6/Signal8/utils/simple_env.py` & `Signal8-1.7/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.6/Signal8.egg-info/PKG-INFO` & `Signal8-1.7/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.6
+Version: 1.7
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-1.6/setup.py` & `Signal8-1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="1.6",
+    version="1.7",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

