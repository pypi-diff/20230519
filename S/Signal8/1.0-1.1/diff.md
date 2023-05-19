# Comparing `tmp/Signal8-1.0.tar.gz` & `tmp/Signal8-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-1.0.tar", last modified: Fri May 19 16:06:03 2023, max compression
+gzip compressed data, was "Signal8-1.1.tar", last modified: Fri May 19 18:28:19 2023, max compression
```

## Comparing `Signal8-1.0.tar` & `Signal8-1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:06:03.364080 Signal8-1.0/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.0/LICENSE
--rw-rw-rw-   0        0        0     4371 2023-05-19 16:06:03.363079 Signal8-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3881 2023-05-17 21:23:57.000000 Signal8-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 16:06:03.261080 Signal8-1.0/Signal8/
--rw-rw-rw-   0        0        0     6641 2023-05-19 15:56:21.000000 Signal8-1.0/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.0/Signal8/__init__.py
--rw-rw-rw-   0        0        0      136 2023-05-19 05:13:31.000000 Signal8-1.0/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:06:03.359080 Signal8-1.0/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.0/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     7891 2023-05-17 20:35:42.000000 Signal8-1.0/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2459 2023-05-17 19:04:54.000000 Signal8-1.0/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.0/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12585 2023-05-19 05:11:53.000000 Signal8-1.0/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:06:03.312083 Signal8-1.0/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4371 2023-05-19 16:06:02.000000 Signal8-1.0/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-19 16:06:03.000000 Signal8-1.0/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:06:02.000000 Signal8-1.0/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 16:06:02.000000 Signal8-1.0/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 16:06:03.365080 Signal8-1.0/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-05-19 16:04:51.000000 Signal8-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:28:19.983945 Signal8-1.1/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.1/LICENSE
+-rw-rw-rw-   0        0        0     4374 2023-05-19 18:28:19.939014 Signal8-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3884 2023-05-19 18:19:01.000000 Signal8-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 18:28:19.796032 Signal8-1.1/Signal8/
+-rw-rw-rw-   0        0        0     6641 2023-05-19 15:56:21.000000 Signal8-1.1/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.1/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      136 2023-05-19 05:13:31.000000 Signal8-1.1/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:28:19.916017 Signal8-1.1/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.1/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     7891 2023-05-17 20:35:42.000000 Signal8-1.1/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2531 2023-05-19 18:27:46.000000 Signal8-1.1/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.1/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12585 2023-05-19 05:11:53.000000 Signal8-1.1/Signal8/utils/simple_env.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:28:19.903020 Signal8-1.1/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4374 2023-05-19 18:28:17.000000 Signal8-1.1/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-19 18:28:18.000000 Signal8-1.1/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 18:28:17.000000 Signal8-1.1/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 18:28:17.000000 Signal8-1.1/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 18:28:19.983945 Signal8-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-05-19 18:28:14.000000 Signal8-1.1/setup.py
```

### Comparing `Signal8-1.0/LICENSE` & `Signal8-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-1.0/PKG-INFO` & `Signal8-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.0
+Version: 1.1
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # A Fork of Multi-Agent Particle Environment
 
-Sig8 is an adapted version of the Simple environment, originally developed by the Farama Foundation as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
+Signal8 is an adapted version of the Simple environment, originally developed by the Farama Foundation as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
 This repository contains a simple multi-agent environment with continuous observations and a discrete action space, inspired by the Lewis Signaling game. The environment incorporates basic simulated physics to create a scenario where agents must communicate and collaborate effectively to navigate around both static and dynamic adversaries to reach a goal.
 
 ## Installation
 
@@ -26,17 +26,17 @@
 pip install -r requirements.txt
 pip install -e .
 ```
 
 ## Usage
 
 ```
-import signal8
+import Signal8
 
-env = signal8.env(has_dynamic_adversaries=True)
+env = Signal8.env(has_dynamic_adversaries=True)
 env.reset(options={"problem_name": "v_cluster"}))
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
 | :------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
```

### Comparing `Signal8-1.0/README.md` & `Signal8-1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # A Fork of Multi-Agent Particle Environment
 
-Sig8 is an adapted version of the Simple environment, originally developed by the Farama Foundation as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
+Signal8 is an adapted version of the Simple environment, originally developed by the Farama Foundation as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
 This repository contains a simple multi-agent environment with continuous observations and a discrete action space, inspired by the Lewis Signaling game. The environment incorporates basic simulated physics to create a scenario where agents must communicate and collaborate effectively to navigate around both static and dynamic adversaries to reach a goal.
 
 ## Installation
 
@@ -14,17 +14,17 @@
 pip install -r requirements.txt
 pip install -e .
 ```
 
 ## Usage
 
 ```
-import signal8
+import Signal8
 
-env = signal8.env(has_dynamic_adversaries=True)
+env = Signal8.env(has_dynamic_adversaries=True)
 env.reset(options={"problem_name": "v_cluster"}))
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
 | :------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
```

### Comparing `Signal8-1.0/Signal8/Signal8.py` & `Signal8-1.1/Signal8/Signal8.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.0/Signal8/utils/core.py` & `Signal8-1.1/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.0/Signal8/utils/problems.py` & `Signal8-1.1/Signal8/utils/problems.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,24 @@
     },
 }
 
 def get_problem_list():
     return list(problems.keys())
 
 def get_problem(scenario_name, has_dynamic_adversaries):
-    scenario = problems[scenario_name]
+    static_scenario = problems[scenario_name]
     
     if has_dynamic_adversaries:
         dynamic_elements = {
             'v_cluster': {'dynamic_adversary': (((-1, 1), (-0.5, -0.35)), ((-1, 1), (0.35, 0.5)))},
             'h_cluster': {'dynamic_adversary': (((-0.5, -0.35), (-1, 1)), ((0.35, 0.5), (-1, 1)))},
             'v_wall': {'dynamic_adversary': (((-1, 1), (-0.25, -0.075)), ((-1, 1), (0.075, 0.25)))},
             'h_wall': {'dynamic_adversary': (((-0.25, -0.075), (-1, 1)), ((0.075, 0.25), (-1, 1)))},
             'left': {'dynamic_adversary': (((-1, 0.5), (-0.45, -0.55)), ((-1, 0.5), (0.45, 0.55)))},
             'right': {'dynamic_adversary': (((-0.5, 1), (-0.45, -0.55)), ((-0.5, 1), (0.45, 0.55)))},
             'top': {'dynamic_adversary': (((-0.45, -0.55), (-0.5, 1)), ((0.45, 0.55), (-0.5, 1)))},
             'bottom': {'dynamic_adversary': (((-0.45, -0.55), (-1, 0.5)), ((0.45, 0.55), (-1, 0.5)))},
         }
-        scenario.update(dynamic_elements[scenario_name])
+        dynamic_scenario = {**static_scenario, **dynamic_elements[scenario_name]}
+        return dynamic_scenario
         
-    return scenario
+    return static_scenario
```

### Comparing `Signal8-1.0/Signal8/utils/simple_env.py` & `Signal8-1.1/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.0/Signal8.egg-info/PKG-INFO` & `Signal8-1.1/Signal8.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.0
+Version: 1.1
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # A Fork of Multi-Agent Particle Environment
 
-Sig8 is an adapted version of the Simple environment, originally developed by the Farama Foundation as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
+Signal8 is an adapted version of the Simple environment, originally developed by the Farama Foundation as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
 This repository contains a simple multi-agent environment with continuous observations and a discrete action space, inspired by the Lewis Signaling game. The environment incorporates basic simulated physics to create a scenario where agents must communicate and collaborate effectively to navigate around both static and dynamic adversaries to reach a goal.
 
 ## Installation
 
@@ -26,17 +26,17 @@
 pip install -r requirements.txt
 pip install -e .
 ```
 
 ## Usage
 
 ```
-import signal8
+import Signal8
 
-env = signal8.env(has_dynamic_adversaries=True)
+env = Signal8.env(has_dynamic_adversaries=True)
 env.reset(options={"problem_name": "v_cluster"}))
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
 | :------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
```

### Comparing `Signal8-1.0/setup.py` & `Signal8-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="1.0",
+    version="1.1",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

