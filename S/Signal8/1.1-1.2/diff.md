# Comparing `tmp/Signal8-1.1.tar.gz` & `tmp/Signal8-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-1.1.tar", last modified: Fri May 19 18:28:19 2023, max compression
+gzip compressed data, was "Signal8-1.2.tar", last modified: Fri May 19 19:32:26 2023, max compression
```

## Comparing `Signal8-1.1.tar` & `Signal8-1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 18:28:19.983945 Signal8-1.1/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.1/LICENSE
--rw-rw-rw-   0        0        0     4374 2023-05-19 18:28:19.939014 Signal8-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3884 2023-05-19 18:19:01.000000 Signal8-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 18:28:19.796032 Signal8-1.1/Signal8/
--rw-rw-rw-   0        0        0     6641 2023-05-19 15:56:21.000000 Signal8-1.1/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.1/Signal8/__init__.py
--rw-rw-rw-   0        0        0      136 2023-05-19 05:13:31.000000 Signal8-1.1/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:28:19.916017 Signal8-1.1/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.1/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     7891 2023-05-17 20:35:42.000000 Signal8-1.1/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2531 2023-05-19 18:27:46.000000 Signal8-1.1/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.1/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12585 2023-05-19 05:11:53.000000 Signal8-1.1/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:28:19.903020 Signal8-1.1/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4374 2023-05-19 18:28:17.000000 Signal8-1.1/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-19 18:28:18.000000 Signal8-1.1/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 18:28:17.000000 Signal8-1.1/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 18:28:17.000000 Signal8-1.1/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 18:28:19.983945 Signal8-1.1/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-05-19 18:28:14.000000 Signal8-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.528554 Signal8-1.2/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.2/LICENSE
+-rw-rw-rw-   0        0        0     4364 2023-05-19 19:32:26.517553 Signal8-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3876 2023-05-19 19:25:10.000000 Signal8-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.425038 Signal8-1.2/Signal8/
+-rw-rw-rw-   0        0        0     6514 2023-05-19 19:29:50.000000 Signal8-1.2/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.2/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-05-19 19:25:12.000000 Signal8-1.2/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.510555 Signal8-1.2/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.2/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     7873 2023-05-19 19:25:15.000000 Signal8-1.2/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2423 2023-05-19 19:25:16.000000 Signal8-1.2/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.2/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12174 2023-05-19 19:30:46.000000 Signal8-1.2/Signal8/utils/simple_env.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.455037 Signal8-1.2/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4364 2023-05-19 19:32:26.000000 Signal8-1.2/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-19 19:32:26.000000 Signal8-1.2/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:32:26.000000 Signal8-1.2/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 19:32:26.000000 Signal8-1.2/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:32:26.532551 Signal8-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-05-19 19:32:15.000000 Signal8-1.2/setup.py
```

### Comparing `Signal8-1.1/LICENSE` & `Signal8-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-1.1/PKG-INFO` & `Signal8-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.1
-Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.
+Version: 1.2
+Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # A Fork of Multi-Agent Particle Environment
 
 Signal8 is an adapted version of the Simple environment, originally developed by the Farama Foundation as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
-This repository contains a simple multi-agent environment with continuous observations and a discrete action space, inspired by the Lewis Signaling game. The environment incorporates basic simulated physics to create a scenario where agents must communicate and collaborate effectively to navigate around both static and dynamic adversaries to reach a goal.
+This repository contains a simple multi-agent environment with continuous observations and a discrete action space, inspired by the Lewis Signaling game. The environment incorporates basic simulated physics to create a scenario where agents must communicate and collaborate effectively to navigate around both static and dynamic obstacles to reach a goal.
 
 ## Installation
 
 ```
 git clone https://github.com/ethanmclark1/signal8.git
 cd signal8
 pip install -r requirements.txt
@@ -28,15 +28,15 @@
 ```
 
 ## Usage
 
 ```
 import Signal8
 
-env = Signal8.env(has_dynamic_adversaries=True)
+env = Signal8.env(dynamic_obstacles=True)
 env.reset(options={"problem_name": "v_cluster"}))
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
 | :------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
```

### Comparing `Signal8-1.1/README.md` & `Signal8-1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # A Fork of Multi-Agent Particle Environment
 
 Signal8 is an adapted version of the Simple environment, originally developed by the Farama Foundation as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
-This repository contains a simple multi-agent environment with continuous observations and a discrete action space, inspired by the Lewis Signaling game. The environment incorporates basic simulated physics to create a scenario where agents must communicate and collaborate effectively to navigate around both static and dynamic adversaries to reach a goal.
+This repository contains a simple multi-agent environment with continuous observations and a discrete action space, inspired by the Lewis Signaling game. The environment incorporates basic simulated physics to create a scenario where agents must communicate and collaborate effectively to navigate around both static and dynamic obstacles to reach a goal.
 
 ## Installation
 
 ```
 git clone https://github.com/ethanmclark1/signal8.git
 cd signal8
 pip install -r requirements.txt
@@ -16,15 +16,15 @@
 ```
 
 ## Usage
 
 ```
 import Signal8
 
-env = Signal8.env(has_dynamic_adversaries=True)
+env = Signal8.env(dynamic_obstacles=True)
 env.reset(options={"problem_name": "v_cluster"}))
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
 | :------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
```

### Comparing `Signal8-1.1/Signal8/Signal8.py` & `Signal8-1.2/Signal8/Signal8.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,74 +7,74 @@
 from .utils.simple_env import SimpleEnv, make_env
 from .utils.problems import get_problem, get_problem_list
 
 class raw_env(SimpleEnv, EzPickle):
     def __init__(
         self, 
         agent_radius=0.1,
-        adversary_radius=0.1,
-        num_adversaries=4,
-        has_dynamic_adversaries=False,
+        obs_radius=0.1,
+        num_obstacles=4,
+        dynamic_obstacles=False,
         max_cycles=500, 
         continuous_actions=False, 
         render_mode="human"
         ):
         
         scenario = Scenario()
         world = scenario.make_world(
             agent_radius, 
-            num_adversaries, 
-            adversary_radius, 
-            has_dynamic_adversaries
+            num_obstacles, 
+            obs_radius, 
+            dynamic_obstacles
             )
         
         super().__init__(
             scenario=scenario, 
             world=world, 
             render_mode=render_mode,
             max_cycles=max_cycles, 
             continuous_actions=continuous_actions,
         )
         
         self.metadata["agent_radius"] = agent_radius
-        self.metadata["num_adversaries"] = num_adversaries
-        self.metadata["adversary_radius"] = adversary_radius
-        self.metadata["has_dynamic_adversaries"] = has_dynamic_adversaries
+        self.metadata["num_obstacles"] = num_obstacles
+        self.metadata["obs_radius"] = obs_radius
+        self.metadata["dynamic_obstacles"] = dynamic_obstacles
 
 env = make_env(raw_env)
 
 class Scenario(BaseScenario):
-    def make_world(self, agent_radius, num_adversaries, adversary_radius, has_dynamic_adversaries):
-        world = World(has_dynamic_adversaries)
+    def make_world(self, agent_radius, num_obstacles, obs_radius, dynamic_obstacles):
+        world = World(dynamic_obstacles)
         world.problem_scenarios = get_problem_list()
         
-        num_dynamic_adversaries = math.floor(num_adversaries / 2) if has_dynamic_adversaries else 0
-        num_agents = num_dynamic_adversaries + 1
+        num_dynamic_obstacles = math.floor(num_obstacles / 2) if dynamic_obstacles else 0
+        num_agents = num_dynamic_obstacles + 1
 
         world.agents = [Agent() for _ in range(num_agents)]
         for i, agent in enumerate(world.agents):
             agent.adversary = True if i > 0 else False
             base_name = "adversary" if agent.adversary else "agent"
             base_index = i - 1 if agent.adversary else 0
             agent.name = f"{base_name}_{base_index}"
             agent.collide = False
             agent.silent = True
             agent.blind = agent.adversary
             agent.size = agent_radius
         
-        world.landmarks = [Landmark() for _ in range(num_adversaries - num_dynamic_adversaries + 1)]
+        world.landmarks = [Landmark() for _ in range(num_obstacles - num_dynamic_obstacles + 1)]
         world.landmarks[0].name = "goal_0"
         world.landmarks[0].collide = False
         world.landmarks[0].movable = False
         world.landmarks[0].size = agent_radius
         
         for i, landmark in enumerate(world.landmarks[1:]):
-            landmark.name = f"obstacle_{i}"
+            landmark.name = f"obs_{i}"
             landmark.collide = False
-            landmark.size = adversary_radius
+            landmark.size = obs_radius
                 
         return world
 
     def reset_world(self, world, np_random, problem_name="v_cluster"):
         self.get_problem_scenario(world, problem_name)
         world.problem_name = problem_name
         
@@ -104,21 +104,21 @@
         return 0
 
     def observation(self, agent, world):
         return np.concatenate((agent.state.p_pos, agent.state.p_vel))
     
     # Get constraints on entities given the problem name
     def get_problem_scenario(self, world, problem_name):
-        problem = get_problem(problem_name, world.has_dynamic_adversaries)
+        problem = get_problem(problem_name, world.dynamic_obstacles)
         world.start_constr = problem['start']
         world.goal_constr = problem['goal']
-        world.static_adversarial_constr = problem['static_adversary']
+        world.static_adversarial_constr = problem['static_obs']
         
-        if world.has_dynamic_adversaries:
-            world.dynamic_adversarial_constr = problem['dynamic_adversary']
+        if world.dynamic_obstacles:
+            world.dynamic_adversarial_constr = problem['dynamic_obs']
     
     # Get scripted action for adversarial agents s.t. they move in a straight line along their constraint
     def get_scripted_action(self, agent, world):
         action = Action()
         action.u = np.zeros(world.dim_p)
         action.c = np.zeros(world.dim_c)
```

### Comparing `Signal8-1.1/Signal8/utils/core.py` & `Signal8-1.2/Signal8/utils/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         # action
         self.action = Action()
         # script behavior to execute
         self.action_callback = None
 
 
 class World:  # multi-agent world
-    def __init__(self, has_dynamic_adversaries=False):
+    def __init__(self, dynamic_obstacles=False):
         # list of agents and entities (can change at execution-time!)
         self.agents = []
         self.landmarks = []
         # communication channel dimensionality
         self.dim_c = 0
         # position dimensionality
         self.dim_p = 2
@@ -96,15 +96,15 @@
         self.dt = 0.1
         # physical damping
         self.damping = 0.25
         # contact response parameters
         self.contact_force = 1e2
         self.contact_margin = 1e-3
         # problem scenarios
-        self.has_dynamic_adversaries = has_dynamic_adversaries
+        self.dynamic_obstacles = dynamic_obstacles
         self.problem_scenarios = None
         self.problem_name = None
         self.start_constr = None
         self.goal_constr = None
         self.static_adversarial_constr = None
         self.dynamic_adversarial_constr = None
```

### Comparing `Signal8-1.1/Signal8/utils/problems.py` & `Signal8-1.2/Signal8/utils/problems.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 problems = {
     'v_cluster': {
         'start': ((-0.15, 0.15), (-1, -0.80)),
         'goal': ((-0.15, 0.15), (0.80, 1)),
-        'static_adversary': ((-0.15, 0.15), (-0.15, 0.15))
+        'static_obs': ((-0.15, 0.15), (-0.15, 0.15))
     },
     'h_cluster': {
         'start': ((-1, -0.80), (-0.15, 0.15)),
         'goal': ((0.80, 1), (-0.15, 0.15)),
-        'static_adversary': ((-0.15, 0.15), (-0.15, 0.15))
+        'static_obs': ((-0.15, 0.15), (-0.15, 0.15))
     },
     'v_wall': {
         'start': ((-1, 1), (-1, -0.80)),
         'goal': ((-1, 1), (0.80, 1)),
-        'static_adversary': ((-0.6, 0.6), (-0.075, 0.075))
+        'static_obs': ((-0.6, 0.6), (-0.075, 0.075))
     },
     'h_wall': {
         'start': ((-1, -0.80), (-1, 1)),
         'goal': ((0.80, 1), (-1, 1)),
-        'static_adversary': ((-0.075, 0.075), (-0.6, 0.6))
+        'static_obs': ((-0.075, 0.075), (-0.6, 0.6))
     },
     'left': {
         'start': ((0, 1), (-1, -0.80)),
         'goal': ((0, 1), (0.80, 1)),
-        'static_adversary': ((-1, 0), (-1, 1))
+        'static_obs': ((-1, 0), (-1, 1))
     },
     'right': {
         'start': ((-1, 0), (-1, -0.80)),
         'goal': ((-1, 0), (0.80, 1)),
-        'static_adversary': ((0, 1), (-1, 1))
+        'static_obs': ((0, 1), (-1, 1))
     },
     'top': {
         'start': ((-1, -0.80), (-1, 0)),
         'goal': ((0.80, 1), (-1, 0)),
-        'static_adversary': ((-1, 1), (0, 1))
+        'static_obs': ((-1, 1), (0, 1))
     },
     'bottom': {
         'start': ((-1, -0.80), (0, 1)),
         'goal': ((0.80, 1), (0, 1)),
-        'static_adversary': ((-1, 1), (-1, 0))
+        'static_obs': ((-1, 1), (-1, 0))
     },
 }
 
 def get_problem_list():
     return list(problems.keys())
 
-def get_problem(scenario_name, has_dynamic_adversaries):
+def get_problem(scenario_name, dynamic_obstacles):
     static_scenario = problems[scenario_name]
     
-    if has_dynamic_adversaries:
+    if dynamic_obstacles:
         dynamic_elements = {
-            'v_cluster': {'dynamic_adversary': (((-1, 1), (-0.5, -0.35)), ((-1, 1), (0.35, 0.5)))},
-            'h_cluster': {'dynamic_adversary': (((-0.5, -0.35), (-1, 1)), ((0.35, 0.5), (-1, 1)))},
-            'v_wall': {'dynamic_adversary': (((-1, 1), (-0.25, -0.075)), ((-1, 1), (0.075, 0.25)))},
-            'h_wall': {'dynamic_adversary': (((-0.25, -0.075), (-1, 1)), ((0.075, 0.25), (-1, 1)))},
-            'left': {'dynamic_adversary': (((-1, 0.5), (-0.45, -0.55)), ((-1, 0.5), (0.45, 0.55)))},
-            'right': {'dynamic_adversary': (((-0.5, 1), (-0.45, -0.55)), ((-0.5, 1), (0.45, 0.55)))},
-            'top': {'dynamic_adversary': (((-0.45, -0.55), (-0.5, 1)), ((0.45, 0.55), (-0.5, 1)))},
-            'bottom': {'dynamic_adversary': (((-0.45, -0.55), (-1, 0.5)), ((0.45, 0.55), (-1, 0.5)))},
+            'v_cluster': {'dynamic_obs': (((-1, 1), (-0.5, -0.35)), ((-1, 1), (0.35, 0.5)))},
+            'h_cluster': {'dynamic_obs': (((-0.5, -0.35), (-1, 1)), ((0.35, 0.5), (-1, 1)))},
+            'v_wall': {'dynamic_obs': (((-1, 1), (-0.25, -0.075)), ((-1, 1), (0.075, 0.25)))},
+            'h_wall': {'dynamic_obs': (((-0.25, -0.075), (-1, 1)), ((0.075, 0.25), (-1, 1)))},
+            'left': {'dynamic_obs': (((-1, 0.5), (-0.45, -0.55)), ((-1, 0.5), (0.45, 0.55)))},
+            'right': {'dynamic_obs': (((-0.5, 1), (-0.45, -0.55)), ((-0.5, 1), (0.45, 0.55)))},
+            'top': {'dynamic_obs': (((-0.45, -0.55), (-0.5, 1)), ((0.45, 0.55), (-0.5, 1)))},
+            'bottom': {'dynamic_obs': (((-0.45, -0.55), (-1, 0.5)), ((0.45, 0.55), (-1, 0.5)))},
         }
         dynamic_scenario = {**static_scenario, **dynamic_elements[scenario_name]}
         return dynamic_scenario
         
     return static_scenario
```

### Comparing `Signal8-1.1/Signal8/utils/simple_env.py` & `Signal8-1.2/Signal8/utils/simple_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import os
-import copy
-
 import gymnasium
 import numpy as np
 import pygame
 from gymnasium import spaces
 from gymnasium.utils import seeding
 
 from pettingzoo import AECEnv
@@ -125,23 +122,14 @@
         self.np_random, seed = seeding.np_random(seed)
 
     def observe(self, agent):
         return self.scenario.observation(
             self.world.agents[self._index_map[agent]], self.world
         ).astype(np.float32)
         
-    def get_init_conditions(self):
-        world = self.unwrapped.world
-        start = world.agents[0].state.p_pos
-        goal = world.agents[0].goal.state.p_pos
-        obstacles = copy.copy(world.landmarks)
-        obstacles.remove(world.agents[0].goal)
-        obstacles = np.array([obstacle.state.p_pos for obstacle in obstacles])
-        return start, goal, obstacles
-
     def state(self):
         states = tuple(
             self.scenario.observation(
                 self.world.agents[self._index_map[agent]], self.world
             ).astype(np.float32)
             for agent in self.possible_agents
         )
```

### Comparing `Signal8-1.1/Signal8.egg-info/PKG-INFO` & `Signal8-1.2/Signal8.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.1
-Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.
+Version: 1.2
+Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # A Fork of Multi-Agent Particle Environment
 
 Signal8 is an adapted version of the Simple environment, originally developed by the Farama Foundation as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
-This repository contains a simple multi-agent environment with continuous observations and a discrete action space, inspired by the Lewis Signaling game. The environment incorporates basic simulated physics to create a scenario where agents must communicate and collaborate effectively to navigate around both static and dynamic adversaries to reach a goal.
+This repository contains a simple multi-agent environment with continuous observations and a discrete action space, inspired by the Lewis Signaling game. The environment incorporates basic simulated physics to create a scenario where agents must communicate and collaborate effectively to navigate around both static and dynamic obstacles to reach a goal.
 
 ## Installation
 
 ```
 git clone https://github.com/ethanmclark1/signal8.git
 cd signal8
 pip install -r requirements.txt
@@ -28,15 +28,15 @@
 ```
 
 ## Usage
 
 ```
 import Signal8
 
-env = Signal8.env(has_dynamic_adversaries=True)
+env = Signal8.env(dynamic_obstacles=True)
 env.reset(options={"problem_name": "v_cluster"}))
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
 | :------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
```

### Comparing `Signal8-1.1/setup.py` & `Signal8-1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="1.1",
+    version="1.2",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
-    description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.",
+    description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
     ],
```

