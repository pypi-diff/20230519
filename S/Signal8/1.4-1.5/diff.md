# Comparing `tmp/Signal8-1.4.tar.gz` & `tmp/Signal8-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-1.4.tar", last modified: Fri May 19 19:43:39 2023, max compression
+gzip compressed data, was "Signal8-1.5.tar", last modified: Fri May 19 19:47:26 2023, max compression
```

## Comparing `Signal8-1.4.tar` & `Signal8-1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 19:43:39.541674 Signal8-1.4/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.4/LICENSE
--rw-rw-rw-   0        0        0     4364 2023-05-19 19:43:39.539675 Signal8-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3876 2023-05-19 19:25:10.000000 Signal8-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 19:43:39.483678 Signal8-1.4/Signal8/
--rw-rw-rw-   0        0        0     6515 2023-05-19 19:42:49.000000 Signal8-1.4/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.4/Signal8/__init__.py
--rw-rw-rw-   0        0        0      130 2023-05-19 19:25:12.000000 Signal8-1.4/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:43:39.535676 Signal8-1.4/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.4/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     7867 2023-05-19 19:40:29.000000 Signal8-1.4/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2423 2023-05-19 19:25:16.000000 Signal8-1.4/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.4/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12174 2023-05-19 19:30:46.000000 Signal8-1.4/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:43:39.517676 Signal8-1.4/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4364 2023-05-19 19:43:39.000000 Signal8-1.4/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-19 19:43:39.000000 Signal8-1.4/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 19:43:39.000000 Signal8-1.4/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 19:43:39.000000 Signal8-1.4/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 19:43:39.542675 Signal8-1.4/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-05-19 19:43:26.000000 Signal8-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:47:26.717285 Signal8-1.5/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.5/LICENSE
+-rw-rw-rw-   0        0        0     4364 2023-05-19 19:47:26.715286 Signal8-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3876 2023-05-19 19:25:10.000000 Signal8-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 19:47:26.649416 Signal8-1.5/Signal8/
+-rw-rw-rw-   0        0        0     6509 2023-05-19 19:46:26.000000 Signal8-1.5/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.5/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-05-19 19:25:12.000000 Signal8-1.5/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:47:26.710286 Signal8-1.5/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.5/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     7867 2023-05-19 19:40:29.000000 Signal8-1.5/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2423 2023-05-19 19:25:16.000000 Signal8-1.5/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.5/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12174 2023-05-19 19:30:46.000000 Signal8-1.5/Signal8/utils/simple_env.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:47:26.683767 Signal8-1.5/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4364 2023-05-19 19:47:26.000000 Signal8-1.5/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-19 19:47:26.000000 Signal8-1.5/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:47:26.000000 Signal8-1.5/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 19:47:26.000000 Signal8-1.5/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:47:26.718285 Signal8-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-05-19 19:47:17.000000 Signal8-1.5/setup.py
```

### Comparing `Signal8-1.4/LICENSE` & `Signal8-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-1.4/PKG-INFO` & `Signal8-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.4
+Version: 1.5
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-1.4/README.md` & `Signal8-1.5/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-1.4/Signal8/Signal8.py` & `Signal8-1.5/Signal8/Signal8.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         world.problem_name = problem_name
         
         # set state and color of both agents and landmarks
         for i, agent in enumerate(world.agents):
             if agent.adversary:
                 agent.color = np.array([0.5, 0, 0])
                 agent.state.p_vel = np.zeros(world.dim_p)
-                agent.state.p_pos = np_random.uniform(*zip(*world.dynamic_obctccoenstr[(i+1) % len(world.dynamic_obstacle_constr)]))
+                agent.state.p_pos = np_random.uniform(*zip(*world.dynamic_obstacle_constr[(i+1) % len(world.dynamic_obstacle_constr)]))
                 agent.action_callback = self.get_scripted_action
             else:
                 agent.color = np.array([0, 0.8, 0])
                 agent.state.p_vel = np.zeros(world.dim_p)
                 agent.state.p_pos = np_random.uniform(*zip(*world.start_constr))
                 agent.goal = world.landmarks[0]
                 agent.goal.color = np.array([0, 0, 0.8])
@@ -110,15 +110,15 @@
     def get_problem_scenario(self, world, problem_name):
         problem = get_problem(problem_name, world.dynamic_obstacles)
         world.start_constr = problem['start']
         world.goal_constr = problem['goal']
         world.static_obstacle_constr = problem['static_obs']
         
         if world.dynamic_obstacles:
-            world.dynamic_obstacle_constrproblem['dynamic_obs']
+            world.dynamic_obstacle_constr['dynamic_obs']
     
     # Get scripted action for adversarial agents s.t. they move in a straight line along their constraint
     def get_scripted_action(self, agent, world):
         action = Action()
         action.u = np.zeros(world.dim_p)
         action.c = np.zeros(world.dim_c)
         
@@ -144,8 +144,8 @@
                 if agent.state.p_pos[1] <= constr[0][1]:  # If at bottom constraint, move up
                     action.u[1] = +1.0
                 elif agent.state.p_pos[1] >= constr[1][1]:  # If at top constraint, move down
                     action.u[1] = -1.0
                 else:  # Otherwise, follow the direction of velocity
                     action.u[1] = np.sign(agent.state.p_vel[1])
 
-        return action
+        return action
```

### Comparing `Signal8-1.4/Signal8/utils/core.py` & `Signal8-1.5/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.4/Signal8/utils/problems.py` & `Signal8-1.5/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.4/Signal8/utils/simple_env.py` & `Signal8-1.5/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.4/Signal8.egg-info/PKG-INFO` & `Signal8-1.5/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.4
+Version: 1.5
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-1.4/setup.py` & `Signal8-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="1.4",
+    version="1.5",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

