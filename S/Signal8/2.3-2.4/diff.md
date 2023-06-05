# Comparing `tmp/Signal8-2.3.tar.gz` & `tmp/Signal8-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-2.3.tar", last modified: Fri Jun  2 17:26:37 2023, max compression
+gzip compressed data, was "Signal8-2.4.tar", last modified: Mon Jun  5 16:10:27 2023, max compression
```

## Comparing `Signal8-2.3.tar` & `Signal8-2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:26:37.788918 Signal8-2.3/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.3/LICENSE
--rw-rw-rw-   0        0        0     4369 2023-06-02 17:26:37.786918 Signal8-2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 17:26:37.691919 Signal8-2.3/Signal8/
--rw-rw-rw-   0        0        0    11040 2023-06-02 17:25:14.000000 Signal8-2.3/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-2.3/Signal8/__init__.py
--rw-rw-rw-   0        0        0      238 2023-06-02 17:05:00.000000 Signal8-2.3/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:26:37.781920 Signal8-2.3/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.3/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5811 2023-05-31 18:22:02.000000 Signal8-2.3/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2783 2023-06-01 21:15:18.000000 Signal8-2.3/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     4402 2023-06-02 17:06:17.000000 Signal8-2.3/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.3/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12529 2023-06-02 16:26:33.000000 Signal8-2.3/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.3/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:26:37.747919 Signal8-2.3/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4369 2023-06-02 17:26:37.000000 Signal8-2.3/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-02 17:26:37.000000 Signal8-2.3/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:26:37.000000 Signal8-2.3/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 17:26:37.000000 Signal8-2.3/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 17:26:37.788918 Signal8-2.3/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-02 17:25:17.000000 Signal8-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:10:27.561843 Signal8-2.4/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.4/LICENSE
+-rw-rw-rw-   0        0        0     4369 2023-06-05 16:10:27.558843 Signal8-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 16:10:27.460845 Signal8-2.4/Signal8/
+-rw-rw-rw-   0        0        0    11151 2023-06-05 16:08:37.000000 Signal8-2.4/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-2.4/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      238 2023-06-05 16:05:24.000000 Signal8-2.4/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:10:27.554845 Signal8-2.4/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.4/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5811 2023-06-02 21:00:42.000000 Signal8-2.4/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2783 2023-06-01 21:15:18.000000 Signal8-2.4/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     5020 2023-06-05 15:51:06.000000 Signal8-2.4/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.4/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12412 2023-06-05 16:05:19.000000 Signal8-2.4/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.4/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:10:27.524845 Signal8-2.4/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4369 2023-06-05 16:10:27.000000 Signal8-2.4/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-05 16:10:27.000000 Signal8-2.4/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:10:27.000000 Signal8-2.4/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 16:10:27.000000 Signal8-2.4/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:10:27.562845 Signal8-2.4/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-05 16:08:42.000000 Signal8-2.4/setup.py
```

### Comparing `Signal8-2.3/LICENSE` & `Signal8-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-2.3/PKG-INFO` & `Signal8-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.3
+Version: 2.4
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.3/README.md` & `Signal8-2.4/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-2.3/Signal8/Signal8.py` & `Signal8-2.4/Signal8/Signal8.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,44 +3,47 @@
 import random
 import logging
 import threading
 import numpy as np
 
 from .utils.npc import NPC
 from .utils.scenario import BaseScenario
-from .utils.core import Agent, Goal, Obstacle, World
 from .utils.simple_env import SimpleEnv, make_env
-from .utils.problems import get_problem, get_problem_list
+from .utils.core import Agent, Goal, Obstacle, World
+from .utils.problems import get_problem_config
 
 from gymnasium.utils import EzPickle
 
 
 class raw_env(SimpleEnv, EzPickle):
-    def __init__(self, num_agents=1, render_mode=None):
+    def __init__(self, problem_type, num_agents=1, render_mode=None):
+        
+        if problem_type not in {'disaster_response', 'precision_farming'}:
+            raise ValueError("Signal8 only supports 'disaster_response' and 'precision_farming' problem types.")
         
         if num_agents > 2:
             raise ValueError("Signal8 currently can only support up to 2 agents.")
         
         scenario = Scenario()
-        world = scenario.make_world(num_agents)
+        world = scenario.make_world(problem_type, num_agents)
         
         super().__init__(
             scenario=scenario, 
             world=world, 
             render_mode=render_mode,
             max_cycles=500, 
         )
         
 env = make_env(raw_env)
 
 class Scenario(BaseScenario):
-    def make_world(self, num_agents):
+    def make_world(self, problem_type, num_agents):
         world = World()
         self._add_logger()
-        world.problem_scenarios = get_problem_list()
+        world.problem_type = problem_type
         
         self.npc = []
         self.obstacle_locks = []
         self.scripted_obstacle_threads = []
         self.scripted_obstacle_running = False
 
         world.agents = [Agent() for _ in range(num_agents)]
@@ -59,19 +62,16 @@
         world.obstacles = [Obstacle() for _ in range(4)]
         for i, obstacle in enumerate(world.obstacles):
             obstacle.name = f"obs_{i}"
                 
         return world
     
     # Get constraints on entities given the problem name
-    def _set_problem_scenario(self, world, np_random, problem_name):
-        if problem_name is None:
-            problem_name = np_random.choice(world.problem_scenarios)
-        problem = get_problem(problem_name)
-        world.problem_name = problem_name
+    def _set_problem_scenario(self, world, np_random, scenario_num):
+        problem = get_problem_config(world.problem_type, scenario_num, np_random)
         world.start_constr = problem['start']
         world.goal_constr = problem['goal']
         world.static_obstacle_constr = problem['static_obs']
         world.dynamic_obstacle_constr = problem['dynamic_obs']
     
     """
     Returns goal constraints that haven't been selected to be used as an obstacle
@@ -127,15 +127,15 @@
             additional_obstacles = [Obstacle() for _ in range(len(world.obstacles), num_total_obstacles)]
             [setattr(obstacle, 'name', f"obs_{i+len(world.obstacles)}") for i, obstacle in enumerate(additional_obstacles)]
             world.obstacles.extend(additional_obstacles)
     
     # Reset position of obstacles
     def _reset_obstacles(self, world, np_random, leftover_entities):
         temp_static_obs_constr = copy.copy(world.static_obstacle_constr)
-        if world.problem_name.startswith('precision_farming'):
+        if world.problem_type.startswith('precision_farming'):
             temp_static_obs_constr += leftover_entities
         temp_dynamic_obs_constr = copy.copy(world.dynamic_obstacle_constr)
         
         num_dynamic_obs = len(temp_dynamic_obs_constr)        
         self._match_obstacles_to_problem(world, len(temp_static_obs_constr))
 
         for i, obstacle in enumerate(world.obstacles):
```

### Comparing `Signal8-2.3/Signal8/utils/core.py` & `Signal8-2.4/Signal8/utils/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         # physical damping
         self.damping = 0.25
         # contact response parameters
         self.contact_force = 1e2
         self.contact_margin = 1e-3
         # problem scenarios
         self.problem_scenarios = []
-        self.problem_name = None
+        self.problem_type = None
         self.start_constr = None
         self.goal_constr = None
         self.static_obstacle_constr = None
         self.dynamic_obstacle_constr = None
         
     # return all entities in the world
     @property
```

### Comparing `Signal8-2.3/Signal8/utils/npc.py` & `Signal8-2.4/Signal8/utils/npc.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.3/Signal8/utils/simple_env.py` & `Signal8-2.4/Signal8/utils/simple_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,50 +48,35 @@
         self.seed()
 
         self.max_cycles = max_cycles
         self.scenario = scenario
         self.world = world
         self.local_ratio = local_ratio
 
-        self.scenario.reset_world(self.world, self.np_random)
         self.agents = [agent.name for agent in self.world.agents]
         self.possible_agents = self.agents[:]
         self._index_map = {agent.name: idx for idx, agent in enumerate(self.world.agents)}
 
         self._agent_selector = agent_selector(self.agents)
 
         # set spaces
         self.action_spaces = dict()
         self.observation_spaces = dict()
-        state_dim = 0
+        obs_dim = 14 if world.problem_type == 'disaster_response' else 24
         for agent in self.world.agents:
-            if agent.movable:
-                space_dim = self.world.dim_p * 2 + 1
-            else:
-                space_dim = 1
-
-            obs_dim = len(self.scenario.observation(agent, self.world))
-            state_dim += obs_dim
+            space_dim = self.world.dim_p * 2 + 1
             self.action_spaces[agent.name] = spaces.Discrete(space_dim)
             self.observation_spaces[agent.name] = spaces.Box(
                 low=-np.float32(1),
                 high=+np.float32(1),
                 shape=(obs_dim,),
                 dtype=np.float32,
             )
-
-        self.state_space = spaces.Box(
-            low=-np.float32(1),
-            high=+np.float32(1),
-            shape=(state_dim,),
-            dtype=np.float32,
-        )
-
+            
         self.steps = 0
-
         self.current_actions = [None] * self.num_agents
 
     def observation_space(self, agent):
         return self.observation_spaces[agent]
 
     def action_space(self, agent):
         return self.action_spaces[agent]
@@ -112,17 +97,23 @@
             for agent in self.possible_agents
         )
         return np.concatenate(states, axis=None)
 
     def reset(self, seed=None, return_info=False, options=None):        
         if seed is not None:
             self.seed(seed=seed)
+            
+        if 'scenario_num' not in options:
+            raise ValueError("Must provide a scenario_num to reset the environment with.")
+        
+        scenario_num = options['scenario_num']
+        if not 0 <= scenario_num <= 3:
+            raise ValueError("scenario_num must be between 0 and 3.")
         
-        problem_scenario = options['problem_name']
-        self.scenario.reset_world(self.world, self.np_random, problem_scenario)
+        self.scenario.reset_world(self.world, self.np_random, scenario_num)
 
         self.agents = self.possible_agents[:]
         # PettingZoo Gymansium requires rewards to be set
         # even if they are not used
         self.rewards = {name: 0.0 for name in self.agents}
         self._cumulative_rewards = {name: 0.0 for name in self.agents}
         self.terminations = {name: False for name in self.agents}
```

### Comparing `Signal8-2.3/Signal8/utils/test_dynamic_obs.py` & `Signal8-2.4/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.3/Signal8.egg-info/PKG-INFO` & `Signal8-2.4/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.3
+Version: 2.4
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.3/Signal8.egg-info/SOURCES.txt` & `Signal8-2.4/Signal8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Signal8-2.3/setup.py` & `Signal8-2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="2.3",
+    version="2.4",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

