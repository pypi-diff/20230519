# Comparing `tmp/Signal8-1.2.tar.gz` & `tmp/Signal8-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-1.2.tar", last modified: Fri May 19 19:32:26 2023, max compression
+gzip compressed data, was "Signal8-1.3.tar", last modified: Fri May 19 19:41:08 2023, max compression
```

## Comparing `Signal8-1.2.tar` & `Signal8-1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.528554 Signal8-1.2/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.2/LICENSE
--rw-rw-rw-   0        0        0     4364 2023-05-19 19:32:26.517553 Signal8-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3876 2023-05-19 19:25:10.000000 Signal8-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.425038 Signal8-1.2/Signal8/
--rw-rw-rw-   0        0        0     6514 2023-05-19 19:29:50.000000 Signal8-1.2/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.2/Signal8/__init__.py
--rw-rw-rw-   0        0        0      130 2023-05-19 19:25:12.000000 Signal8-1.2/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.510555 Signal8-1.2/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.2/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     7873 2023-05-19 19:25:15.000000 Signal8-1.2/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2423 2023-05-19 19:25:16.000000 Signal8-1.2/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.2/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12174 2023-05-19 19:30:46.000000 Signal8-1.2/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.455037 Signal8-1.2/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4364 2023-05-19 19:32:26.000000 Signal8-1.2/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-19 19:32:26.000000 Signal8-1.2/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 19:32:26.000000 Signal8-1.2/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 19:32:26.000000 Signal8-1.2/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 19:32:26.532551 Signal8-1.2/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-05-19 19:32:15.000000 Signal8-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:41:08.766513 Signal8-1.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.3/LICENSE
+-rw-rw-rw-   0        0        0     4364 2023-05-19 19:41:08.765513 Signal8-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3876 2023-05-19 19:25:10.000000 Signal8-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 19:41:08.680516 Signal8-1.3/Signal8/
+-rw-rw-rw-   0        0        0     6516 2023-05-19 19:40:28.000000 Signal8-1.3/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.3/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-05-19 19:25:12.000000 Signal8-1.3/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:41:08.761513 Signal8-1.3/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.3/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     7867 2023-05-19 19:40:29.000000 Signal8-1.3/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2423 2023-05-19 19:25:16.000000 Signal8-1.3/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.3/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12174 2023-05-19 19:30:46.000000 Signal8-1.3/Signal8/utils/simple_env.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:41:08.715516 Signal8-1.3/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4364 2023-05-19 19:41:08.000000 Signal8-1.3/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-19 19:41:08.000000 Signal8-1.3/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:41:08.000000 Signal8-1.3/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 19:41:08.000000 Signal8-1.3/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:41:08.767512 Signal8-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-05-19 19:40:58.000000 Signal8-1.3/setup.py
```

### Comparing `Signal8-1.2/LICENSE` & `Signal8-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-1.2/PKG-INFO` & `Signal8-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.2
+Version: 1.3
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-1.2/README.md` & `Signal8-1.3/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-1.2/Signal8/Signal8.py` & `Signal8-1.3/Signal8/Signal8.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,47 +7,47 @@
 from .utils.simple_env import SimpleEnv, make_env
 from .utils.problems import get_problem, get_problem_list
 
 class raw_env(SimpleEnv, EzPickle):
     def __init__(
         self, 
         agent_radius=0.1,
-        obs_radius=0.1,
         num_obstacles=4,
+        obstacle_radius=0.1,
         dynamic_obstacles=False,
         max_cycles=500, 
         continuous_actions=False, 
         render_mode="human"
         ):
         
         scenario = Scenario()
         world = scenario.make_world(
             agent_radius, 
             num_obstacles, 
-            obs_radius, 
+            obstacle_radius, 
             dynamic_obstacles
             )
         
         super().__init__(
             scenario=scenario, 
             world=world, 
             render_mode=render_mode,
             max_cycles=max_cycles, 
             continuous_actions=continuous_actions,
         )
         
         self.metadata["agent_radius"] = agent_radius
         self.metadata["num_obstacles"] = num_obstacles
-        self.metadata["obs_radius"] = obs_radius
+        self.metadata["obstacle_radius"] = obstacle_radius
         self.metadata["dynamic_obstacles"] = dynamic_obstacles
 
 env = make_env(raw_env)
 
 class Scenario(BaseScenario):
-    def make_world(self, agent_radius, num_obstacles, obs_radius, dynamic_obstacles):
+    def make_world(self, agent_radius, num_obstacles, obstacle_radius, dynamic_obstacles):
         world = World(dynamic_obstacles)
         world.problem_scenarios = get_problem_list()
         
         num_dynamic_obstacles = math.floor(num_obstacles / 2) if dynamic_obstacles else 0
         num_agents = num_dynamic_obstacles + 1
 
         world.agents = [Agent() for _ in range(num_agents)]
@@ -66,67 +66,67 @@
         world.landmarks[0].collide = False
         world.landmarks[0].movable = False
         world.landmarks[0].size = agent_radius
         
         for i, landmark in enumerate(world.landmarks[1:]):
             landmark.name = f"obs_{i}"
             landmark.collide = False
-            landmark.size = obs_radius
+            landmark.size = obstacle_radius
                 
         return world
 
     def reset_world(self, world, np_random, problem_name="v_cluster"):
         self.get_problem_scenario(world, problem_name)
         world.problem_name = problem_name
         
         # set state and color of both agents and landmarks
         for i, agent in enumerate(world.agents):
             if agent.adversary:
                 agent.color = np.array([0.5, 0, 0])
                 agent.state.p_vel = np.zeros(world.dim_p)
-                agent.state.p_pos = np_random.uniform(*zip(*world.dynamic_adversarial_constr[(i+1) % len(world.dynamic_adversarial_constr)]))
+                agent.state.p_pos = np_random.uniform(*zip(*world.dynamic_obctccoenstr[(i+1) % len(world.dyndynamic_obstacle_constr
                 agent.action_callback = self.get_scripted_action
             else:
                 agent.color = np.array([0, 0.8, 0])
                 agent.state.p_vel = np.zeros(world.dim_p)
                 agent.state.p_pos = np_random.uniform(*zip(*world.start_constr))
                 agent.goal = world.landmarks[0]
                 agent.goal.color = np.array([0, 0, 0.8])
                 agent.goal.state.p_vel = np.zeros(world.dim_p)
                 agent.goal.state.p_pos = np_random.uniform(*zip(*world.goal_constr))
                 
         for landmark in world.landmarks[1:]:
             landmark.color = np.array([0.2, 0.2, 0.2])
             landmark.state.p_vel = np.zeros(world.dim_p)
-            landmark.state.p_pos = np_random.uniform(*zip(*world.static_adversarial_constr))
+            landmark.state.p_pos = np_random.uniform(*zip(*world.static_obstacle_constr))
     
     # Do not need to implement this function
     def reward(self, agent, world):
         return 0
 
     def observation(self, agent, world):
         return np.concatenate((agent.state.p_pos, agent.state.p_vel))
     
     # Get constraints on entities given the problem name
     def get_problem_scenario(self, world, problem_name):
         problem = get_problem(problem_name, world.dynamic_obstacles)
         world.start_constr = problem['start']
         world.goal_constr = problem['goal']
-        world.static_adversarial_constr = problem['static_obs']
+        world.static_obstacle_constr = problem['static_obs']
         
         if world.dynamic_obstacles:
-            world.dynamic_adversarial_constr = problem['dynamic_obs']
+            world.dynamic_obstacle_constrproblem['dynamic_obs']
     
     # Get scripted action for adversarial agents s.t. they move in a straight line along their constraint
     def get_scripted_action(self, agent, world):
         action = Action()
         action.u = np.zeros(world.dim_p)
         action.c = np.zeros(world.dim_c)
         
-        constr = world.dynamic_adversarial_constr[int(agent.name[-1])]
+        constr = world.dynamic_obstacle_constrt(agent.name[-1])]
         constr_size = [(abs(point[0]) + abs(point[1])) for point in constr]
         dimension = 'horizontal' if constr_size[0] > constr_size[1] else 'vertical'
 
         # Always start off moving in the positive direction
         if dimension == 'horizontal':
             if (agent.state.p_vel == 0).all():
                 action.u[0] = +1.0
```

### Comparing `Signal8-1.2/Signal8/utils/core.py` & `Signal8-1.3/Signal8/utils/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,16 +101,16 @@
         self.contact_margin = 1e-3
         # problem scenarios
         self.dynamic_obstacles = dynamic_obstacles
         self.problem_scenarios = None
         self.problem_name = None
         self.start_constr = None
         self.goal_constr = None
-        self.static_adversarial_constr = None
-        self.dynamic_adversarial_constr = None
+        self.static_obstacle_constr = None
+        self.dynamic_obstacle_constr = None
         
     # return all entities in the world
     @property
     def entities(self):
         return self.agents + self.landmarks
 
     # return all agents controllable by external policies
```

### Comparing `Signal8-1.2/Signal8/utils/problems.py` & `Signal8-1.3/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.2/Signal8/utils/simple_env.py` & `Signal8-1.3/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.2/Signal8.egg-info/PKG-INFO` & `Signal8-1.3/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.2
+Version: 1.3
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-1.2/setup.py` & `Signal8-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="1.2",
+    version="1.3",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

