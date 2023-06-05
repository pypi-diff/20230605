# Comparing `tmp/Signal8-2.7.tar.gz` & `tmp/Signal8-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-2.7.tar", last modified: Mon Jun  5 17:27:55 2023, max compression
+gzip compressed data, was "Signal8-2.8.tar", last modified: Mon Jun  5 17:29:45 2023, max compression
```

## Comparing `Signal8-2.7.tar` & `Signal8-2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:54.990539 Signal8-2.7/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.7/LICENSE
--rw-rw-rw-   0        0        0     4369 2023-06-05 17:27:54.982499 Signal8-2.7/PKG-INFO
--rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:54.854499 Signal8-2.7/Signal8/
--rw-rw-rw-   0        0        0    11223 2023-06-05 17:25:13.000000 Signal8-2.7/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-2.7/Signal8/__init__.py
--rw-rw-rw-   0        0        0      253 2023-06-05 17:26:53.000000 Signal8-2.7/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:54.942497 Signal8-2.7/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.7/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5783 2023-06-05 17:17:47.000000 Signal8-2.7/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2783 2023-06-05 17:25:42.000000 Signal8-2.7/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-2.7/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.7/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12407 2023-06-05 17:15:50.000000 Signal8-2.7/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.7/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:27:54.922499 Signal8-2.7/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4369 2023-06-05 17:27:54.000000 Signal8-2.7/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-05 17:27:54.000000 Signal8-2.7/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:27:54.000000 Signal8-2.7/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 17:27:54.000000 Signal8-2.7/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 17:27:54.991540 Signal8-2.7/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-05 17:27:06.000000 Signal8-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:29:45.432397 Signal8-2.8/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.8/LICENSE
+-rw-rw-rw-   0        0        0     4369 2023-06-05 17:29:45.431397 Signal8-2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 17:29:45.339880 Signal8-2.8/Signal8/
+-rw-rw-rw-   0        0        0    11220 2023-06-05 17:28:53.000000 Signal8-2.8/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-2.8/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-06-05 17:26:53.000000 Signal8-2.8/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:29:45.426399 Signal8-2.8/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.8/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5783 2023-06-05 17:17:47.000000 Signal8-2.8/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2783 2023-06-05 17:25:42.000000 Signal8-2.8/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-2.8/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.8/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12407 2023-06-05 17:15:50.000000 Signal8-2.8/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.8/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:29:45.382879 Signal8-2.8/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4369 2023-06-05 17:29:44.000000 Signal8-2.8/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-05 17:29:45.000000 Signal8-2.8/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 17:29:44.000000 Signal8-2.8/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 17:29:44.000000 Signal8-2.8/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 17:29:45.433400 Signal8-2.8/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-05 17:29:06.000000 Signal8-2.8/setup.py
```

### Comparing `Signal8-2.7/LICENSE` & `Signal8-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-2.7/PKG-INFO` & `Signal8-2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.7
+Version: 2.8
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.7/README.md` & `Signal8-2.8/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-2.7/Signal8/Signal8.py` & `Signal8-2.8/Signal8/Signal8.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import time
 import copy
 import random
 import logging
 import threading
 import numpy as np
 
-# TODO
-from utils.npc import NPC
-from utils.scenario import BaseScenario
-from utils.simple_env import SimpleEnv, make_env
-from utils.core import Agent, Goal, Obstacle, World
-from utils.problems import get_problem_instance
+from .utils.npc import NPC
+from .utils.scenario import BaseScenario
+from .utils.simple_env import SimpleEnv, make_env
+from .utils.core import Agent, Goal, Obstacle, World
+from .utils.problems import get_problem_instance
 
 from gymnasium.utils import EzPickle
 
 
 class raw_env(SimpleEnv, EzPickle):
     def __init__(self, problem_type, num_agents=1, render_mode=None):
```

### Comparing `Signal8-2.7/Signal8/utils/core.py` & `Signal8-2.8/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.7/Signal8/utils/npc.py` & `Signal8-2.8/Signal8/utils/npc.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.7/Signal8/utils/problems.py` & `Signal8-2.8/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.7/Signal8/utils/simple_env.py` & `Signal8-2.8/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.7/Signal8/utils/test_dynamic_obs.py` & `Signal8-2.8/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.7/Signal8.egg-info/PKG-INFO` & `Signal8-2.8/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.7
+Version: 2.8
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.7/Signal8.egg-info/SOURCES.txt` & `Signal8-2.8/Signal8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Signal8-2.7/setup.py` & `Signal8-2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="2.7",
+    version="2.8",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

