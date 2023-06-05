# Comparing `tmp/action-graph-1.2.6.tar.gz` & `tmp/action-graph-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action-graph-1.2.6.tar", last modified: Sun Jun  4 23:36:50 2023, max compression
+gzip compressed data, was "action-graph-1.2.7.tar", last modified: Mon Jun  5 00:17:07 2023, max compression
```

## Comparing `action-graph-1.2.6.tar` & `action-graph-1.2.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.2.6/LICENSE
--rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.2.6/README.md
--rw-r--r--   0        0        0      684 2023-06-04 23:32:51.361535 action-graph-1.2.6/action_graph/__init__.py
--rw-r--r--   0        0        0     3219 2023-06-04 23:27:52.757522 action-graph-1.2.6/action_graph/action.py
--rw-r--r--   0        0        0     9491 2022-12-14 18:55:20.840750 action-graph-1.2.6/action_graph/agent.py
--rw-r--r--   0        0        0     4630 2022-12-14 19:25:01.486788 action-graph-1.2.6/action_graph/planner.py
--rw-r--r--   0        0        0      832 2023-06-04 23:32:27.506288 action-graph-1.2.6/pyproject.toml
--rwxr-xr-x   0        0        0     1182 2023-06-04 22:59:50.649818 action-graph-1.2.6/tests/01-redundant_precon.py
--rwxr-xr-x   0        0        0     1180 2023-06-04 22:59:48.257783 action-graph-1.2.6/tests/02-multi_feasible.py
--rwxr-xr-x   0        0        0     1371 2023-06-04 22:59:45.617744 action-graph-1.2.6/tests/03-references.py
--rwxr-xr-x   0        0        0      917 2023-06-04 22:59:36.089603 action-graph-1.2.6/tests/04-loop_test.py
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.2.7/LICENSE
+-rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.2.7/README.md
+-rw-r--r--   0        0        0      684 2023-06-05 00:16:34.263737 action-graph-1.2.7/action_graph/__init__.py
+-rw-r--r--   0        0        0     3423 2023-06-05 00:12:55.090353 action-graph-1.2.7/action_graph/action.py
+-rw-r--r--   0        0        0     9491 2022-12-14 18:55:20.840750 action-graph-1.2.7/action_graph/agent.py
+-rw-r--r--   0        0        0     4630 2022-12-14 19:25:01.486788 action-graph-1.2.7/action_graph/planner.py
+-rw-r--r--   0        0        0      832 2023-06-05 00:15:54.391516 action-graph-1.2.7/pyproject.toml
+-rwxr-xr-x   0        0        0     1182 2023-06-04 22:59:50.649818 action-graph-1.2.7/tests/01-redundant_precon.py
+-rwxr-xr-x   0        0        0     1180 2023-06-04 22:59:48.257783 action-graph-1.2.7/tests/02-multi_feasible.py
+-rwxr-xr-x   0        0        0     1371 2023-06-04 22:59:45.617744 action-graph-1.2.7/tests/03-references.py
+-rwxr-xr-x   0        0        0      917 2023-06-04 22:59:36.089603 action-graph-1.2.7/tests/04-loop_test.py
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.2.7/PKG-INFO
```

### Comparing `action-graph-1.2.6/LICENSE` & `action-graph-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.6/README.md` & `action-graph-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.6/action_graph/__init__.py` & `action-graph-1.2.7/action_graph/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 from action_graph.action import Action, ActionStatus, State
 from action_graph.agent import Agent
 
 name = 'action_graph'
-__version__ = '1.2.6'
+__version__ = '1.2.7'
 __all__ = [
     'State',
     'Action',
     'ActionStatus',
     'ActionFailedException',
     'ActionAbortedException',
     'ActionTimedOutException',
```

### Comparing `action-graph-1.2.6/action_graph/action.py` & `action-graph-1.2.7/action_graph/action.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,23 +19,27 @@
     NEUTRAL = auto()
 
 
 class Action():
 
     effects: State = {}
     preconditions: State = {}
+    services = []  # effects whose state value is variable (Ellipsis)
 
     cost: float = 1.0
     status: ActionStatus = ActionStatus.SUCCESS
     timeout: float = 86_400.0  # 24 hours
     allow_async: bool = False
 
     def __init__(self, agent=None) -> None:
         self.agent = agent
         self.__exec_thread: Thread = Thread(target=self.on_execute, args=())
+        for k, v in self.effects.items():
+            if v is Ellipsis:
+                self.services.append(k)
 
     def check_runtime_precondition(self, outcome: State) -> bool:
         return True
 
     def _execute(self, outcome: State):
         self.status = ActionStatus.RUNNING
         self.__exec_thread = Thread(target=self.on_execute, args=(outcome,))
@@ -64,16 +68,17 @@
 
     def on_exit(self, outcome: State = None):
         pass
 
     def apply_effects(self, outcome: State, state: State):
         # update the state with the predicted outcomes
         for k, v in self.effects.items():
-            if v is not Ellipsis:
-                state[k] = v
+            if k in self.services:
+                continue
+            state[k] = v
 
     def __repr__(self) -> str:
         return self.__class__.__name__
 
     def __hash__(self):
         return hash(self.__class__.__name__)
```

### Comparing `action-graph-1.2.6/action_graph/agent.py` & `action-graph-1.2.7/action_graph/agent.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.6/action_graph/planner.py` & `action-graph-1.2.7/action_graph/planner.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.6/pyproject.toml` & `action-graph-1.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 authors = [
     { name = "Bharath Achyutha Rao", email = "bharath.rao@hotmail.com" },
 ]
 name = "action_graph"
-version = "1.2.6"
+version = "1.2.7"
 description = "Autonomous agent for task/action planning and execution"
 readme = "README.md"
 requires-python = ">=3.7,<4.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `action-graph-1.2.6/tests/01-redundant_precon.py` & `action-graph-1.2.7/tests/01-redundant_precon.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.6/tests/02-multi_feasible.py` & `action-graph-1.2.7/tests/02-multi_feasible.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.6/tests/03-references.py` & `action-graph-1.2.7/tests/03-references.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.6/tests/04-loop_test.py` & `action-graph-1.2.7/tests/04-loop_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.6/PKG-INFO` & `action-graph-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action_graph
-Version: 1.2.6
+Version: 1.2.7
 Summary: Autonomous agent for task/action planning and execution
 Author-email: Bharath Achyutha Rao <bharath.rao@hotmail.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Bug Tracker, https://github.com/bharathra/action_graph/issues
```

