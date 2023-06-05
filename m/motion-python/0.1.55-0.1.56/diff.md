# Comparing `tmp/motion_python-0.1.55.tar.gz` & `tmp/motion_python-0.1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.55.tar", max compression
+gzip compressed data, was "motion_python-0.1.56.tar", max compression
```

## Comparing `motion_python-0.1.55.tar` & `motion_python-0.1.56.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-05 17:18:54.251162 motion_python-0.1.55/README.md
--rw-r--r--   0        0        0      202 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/component.py
--rw-r--r--   0        0        0    14675 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/execute.py
--rw-r--r--   0        0        0     5209 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/fit_task.py
--rw-r--r--   0        0        0    10317 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/route.py
--rw-r--r--   0        0        0     6283 2023-06-05 17:18:54.251162 motion_python-0.1.55/motion/utils.py
--rw-r--r--   0        0        0     1555 2023-06-05 17:19:14.651404 motion_python-0.1.55/pyproject.toml
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.55/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-05 18:15:48.822358 motion_python-0.1.56/README.md
+-rw-r--r--   0        0        0      221 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/component.py
+-rw-r--r--   0        0        0    14675 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/execute.py
+-rw-r--r--   0        0        0     5209 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/fit_task.py
+-rw-r--r--   0        0        0    10317 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/route.py
+-rw-r--r--   0        0        0     7616 2023-06-05 18:15:48.826358 motion_python-0.1.56/motion/utils.py
+-rw-r--r--   0        0        0     1572 2023-06-05 18:16:09.062633 motion_python-0.1.56/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.56/PKG-INFO
```

### Comparing `motion_python-0.1.55/README.md` & `motion_python-0.1.56/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.55/motion/component.py` & `motion_python-0.1.56/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.55/motion/execute.py` & `motion_python-0.1.56/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.55/motion/fit_task.py` & `motion_python-0.1.56/motion/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.55/motion/instance.py` & `motion_python-0.1.56/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.55/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.56/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.55/motion/route.py` & `motion_python-0.1.56/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.55/motion/utils.py` & `motion_python-0.1.56/motion/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,59 @@
         kwargs.setdefault("port", int(os.getenv("MOTION_REDIS_PORT", "6379")))
         kwargs.setdefault("db", int(os.getenv("MOTION_REDIS_DB", "0")))
         kwargs.setdefault("password", os.getenv("MOTION_REDIS_PASSWORD", None))
 
         super().__init__(**kwargs)
 
 
+def clear_instance(instance_name: str) -> bool:
+    """Clears the state and cached results associated with a component instance.
+
+    Usage:
+    ```python
+    from motion import clear_instance
+
+    clear_instance("Counter__default")
+    ```
+
+    Args:
+        instance (str): Instance name of the component to clear.
+            In the form `componentname__instancename`.
+
+    Raises:
+        ValueError:
+            If the instance name is not in the form
+            `componentname__instancename`.
+
+    Returns:
+        bool: True if the instance existed, False otherwise.
+    """
+    if "__" not in instance_name:
+        raise ValueError("Instance must be in the form `componentname__instancename`.")
+
+    rp = RedisParams()
+    redis_con = redis.Redis(host=rp.host, port=rp.port, password=rp.password, db=rp.db)
+
+    # Check if the instance exists
+    if not redis_con.exists(f"MOTION_VERSION:{instance_name}"):
+        return False
+
+    # Delete the instance state, version, and cached results
+    redis_con.delete(f"MOTION_STATE:{instance_name}")
+    redis_con.delete(f"MOTION_VERSION:{instance_name}")
+
+    results_to_delete = redis_con.keys(f"MOTION_RESULT:{instance_name}/*")
+    pipeline = redis_con.pipeline()
+    for result in results_to_delete:
+        pipeline.delete(result)
+    pipeline.execute()
+
+    return True
+
+
 class CustomDict(dict):
     def __init__(
         self,
         component_name: str,
         dict_type: str,
         *args: Any,
         **kwargs: Any,
```

### Comparing `motion_python-0.1.55/pyproject.toml` & `motion_python-0.1.56/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.55"
+version = "0.1.56"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 colorlog = "^6.7.0"
 pydantic = "^1.10.7"
 cloudpickle = "^2.0"
 redis = "^4.5.5"
 psutil = "^5.9.5"
+rich = "^13.4.1"
 
 [tool.poetry.group.dev.dependencies]
 poetry-types = "^0.3.5"
 pytest = "^7.2.2"
 mypy = "^1.1.1"
 coverage = {extras = ["toml"], version = "^7.2.3"}
 pre-commit = "^3.2.1"
```

### Comparing `motion_python-0.1.55/PKG-INFO` & `motion_python-0.1.56/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.55
+Version: 0.1.56
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloudpickle (>=2.0,<3.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: redis (>=4.5.5,<5.0.0)
+Requires-Dist: rich (>=13.4.1,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Motion
 
 [![motion](https://github.com/dm4ml/motion/workflows/motion/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"motion")
 [![lint (via ruff)](https://github.com/dm4ml/motion/workflows/lint/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"lint")
 [![docs](https://github.com/dm4ml/motion/workflows/docs/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"docs")
```

