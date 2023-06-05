# Comparing `tmp/motion_python-0.1.54.tar.gz` & `tmp/motion_python-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.54.tar", max compression
+gzip compressed data, was "motion_python-0.1.55.tar", max compression
```

## Comparing `motion_python-0.1.54.tar` & `motion_python-0.1.55.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-03 00:01:31.175881 motion_python-0.1.54/README.md
--rw-r--r--   0        0        0      202 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/component.py
--rw-r--r--   0        0        0    14780 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/execute.py
--rw-r--r--   0        0        0     5209 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/fit_task.py
--rw-r--r--   0        0        0    10437 2023-06-03 00:01:31.175881 motion_python-0.1.54/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-03 00:01:31.179881 motion_python-0.1.54/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-06-03 00:01:31.179881 motion_python-0.1.54/motion/route.py
--rw-r--r--   0        0        0     6283 2023-06-03 00:01:31.179881 motion_python-0.1.54/motion/utils.py
--rw-r--r--   0        0        0     1555 2023-06-03 00:01:55.879995 motion_python-0.1.54/pyproject.toml
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.54/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-05 17:18:54.251162 motion_python-0.1.55/README.md
+-rw-r--r--   0        0        0      202 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/component.py
+-rw-r--r--   0        0        0    14675 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/execute.py
+-rw-r--r--   0        0        0     5209 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/fit_task.py
+-rw-r--r--   0        0        0    10317 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/route.py
+-rw-r--r--   0        0        0     6283 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/utils.py
+-rw-r--r--   0        0        0     1555 2023-06-05 17:19:14.651404 motion_python-0.1.55/pyproject.toml
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.55/PKG-INFO
```

### Comparing `motion_python-0.1.54/README.md` & `motion_python-0.1.55/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.54/motion/cli.py` & `motion_python-0.1.55/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.54/motion/component.py` & `motion_python-0.1.55/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.54/motion/execute.py` & `motion_python-0.1.55/motion/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,16 +294,14 @@
                 cache_result_key = (
                     f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
                 )
                 if self._redis_con.exists(cache_result_key):
                     infer_result = cloudpickle.loads(
                         self._redis_con.get(cache_result_key)
                     )
-                    # Update TTL
-                    self._redis_con.expire(cache_result_key, cache_ttl)
                     route_run = True
 
             # If not in cache or value can't be hashed or
             # user wants to force refresh state, run route
             if not route_run:
                 infer_result = self._infer_routes[key].run(
                     state=self._state, value=value
```

### Comparing `motion_python-0.1.54/motion/fit_task.py` & `motion_python-0.1.55/motion/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.54/motion/instance.py` & `motion_python-0.1.55/motion/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,17 +286,15 @@
         #   no fit ops defined for `multiply`
         ```
 
 
         Args:
             cache_ttl (int, optional):
                 How long the inference result should live in a cache (in
-                seconds). Defaults to 1 day (60 * 60 * 24). The expiration
-                time is extended if there are subsequent infer calls
-                for the same value.
+                seconds). Defaults to 1 day (60 * 60 * 24).
             force_refresh (bool, optional): Read the latest value of the
                 state before running an inference call, otherwise a stale
                 version of the state or a cached result may be used.
                 If you do not want to read from the cache, set force_refresh
                 = True. Defaults to False.
             flush_fit (bool, optional):
                 If True, waits for the fit op to finish executing before
```

### Comparing `motion_python-0.1.54/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.55/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.54/motion/route.py` & `motion_python-0.1.55/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.54/motion/utils.py` & `motion_python-0.1.55/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.54/pyproject.toml` & `motion_python-0.1.55/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.54"
+version = "0.1.55"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.54/PKG-INFO` & `motion_python-0.1.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.54
+Version: 0.1.55
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

