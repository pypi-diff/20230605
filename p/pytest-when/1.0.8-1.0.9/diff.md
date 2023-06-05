# Comparing `tmp/pytest_when-1.0.8.tar.gz` & `tmp/pytest_when-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_when-1.0.8.tar", last modified: Wed May 31 21:33:22 2023, max compression
+gzip compressed data, was "pytest_when-1.0.9.tar", last modified: Mon Jun  5 14:15:58 2023, max compression
```

## Comparing `pytest_when-1.0.8.tar` & `pytest_when-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11342 2023-05-31 21:32:46.853017 pytest_when-1.0.8/LICENSE
--rw-r--r--   0        0        0     2866 2023-05-31 21:32:46.853017 pytest_when-1.0.8/README.md
--rw-r--r--   0        0        0     2766 2023-05-31 21:33:22.885145 pytest_when-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-31 21:32:46.853017 pytest_when-1.0.8/pytest_when/__init__.py
--rw-r--r--   0        0        0       45 2023-05-31 21:32:46.853017 pytest_when-1.0.8/pytest_when/plugin.py
--rw-r--r--   0        0        0        0 2023-05-31 21:32:46.853017 pytest_when-1.0.8/pytest_when/py.typed
--rw-r--r--   0        0        0    10675 2023-05-31 21:32:46.853017 pytest_when-1.0.8/pytest_when/when.py
--rw-r--r--   0        0        0        0 2023-05-31 21:32:46.853017 pytest_when-1.0.8/tests/resources/__init__.py
--rw-r--r--   0        0        0      232 2023-05-31 21:32:46.853017 pytest_when-1.0.8/tests/resources/example_module.py
--rw-r--r--   0        0        0     3635 2023-05-31 21:32:46.853017 pytest_when-1.0.8/tests/test_create_call_key.py
--rw-r--r--   0        0        0     6280 2023-05-31 21:32:46.853017 pytest_when-1.0.8/tests/test_integration.py
--rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 pytest_when-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-05 14:15:24.162645 pytest_when-1.0.9/LICENSE
+-rw-r--r--   0        0        0     2866 2023-06-05 14:15:24.162645 pytest_when-1.0.9/README.md
+-rw-r--r--   0        0        0     2766 2023-06-05 14:15:58.726831 pytest_when-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 14:15:24.162645 pytest_when-1.0.9/pytest_when/__init__.py
+-rw-r--r--   0        0        0       45 2023-06-05 14:15:24.162645 pytest_when-1.0.9/pytest_when/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-05 14:15:24.162645 pytest_when-1.0.9/pytest_when/py.typed
+-rw-r--r--   0        0        0    10660 2023-06-05 14:15:24.166645 pytest_when-1.0.9/pytest_when/when.py
+-rw-r--r--   0        0        0        0 2023-06-05 14:15:24.166645 pytest_when-1.0.9/tests/resources/__init__.py
+-rw-r--r--   0        0        0      294 2023-06-05 14:15:24.166645 pytest_when-1.0.9/tests/resources/example_module.py
+-rw-r--r--   0        0        0     3635 2023-06-05 14:15:24.166645 pytest_when-1.0.9/tests/test_create_call_key.py
+-rw-r--r--   0        0        0     6560 2023-06-05 14:15:24.166645 pytest_when-1.0.9/tests/test_integration.py
+-rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 pytest_when-1.0.9/PKG-INFO
```

### Comparing `pytest_when-1.0.8/LICENSE` & `pytest_when-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.8/README.md` & `pytest_when-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.8/pyproject.toml` & `pytest_when-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 dependencies = [
     "pytest>=7.3.1",
     "pytest-mock>=3.10.0",
     "typing-extensions>=4.5.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "1.0.8"
+version = "1.0.9"
 
 [project.entry-points.pytest11]
 pytest-when = "pytest_when.plugin"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/pytest-when"
```

### Comparing `pytest_when-1.0.8/pytest_when/when.py` & `pytest_when-1.0.9/pytest_when/when.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,25 +296,23 @@
         will be called with:
         "a" - as first argument,
         any second argument,
         kwarg1 = "b" (only),
         any kwarg2 kwarg
 
         """
-        is_instance_method = (
-            tuple(
-                inspect.signature(
-                    getattr(
-                        self.cls,
-                        self.method,
-                    )
-                ).parameters
-            )[0]
-            == "self"
+        params = tuple(
+            inspect.signature(
+                getattr(
+                    self.cls,
+                    self.method,
+                )
+            ).parameters
         )
+        is_instance_method = False if not params else params[0] == "self"
         # prepend Markers.any in case of a method (for self arg)
         self.args = (Markers.any, *args) if is_instance_method else args
         self.kwargs = kwargs
         return self
 
     def then_return(self, value: _TargetMethodReturn) -> MagicMock:
         """Return value in case the called_with specification will match the call."""
```

### Comparing `pytest_when-1.0.8/tests/test_create_call_key.py` & `pytest_when-1.0.9/tests/test_create_call_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             d_kw=4,
         )
     ] = 1
     {}[
         create_call_key(
             inspect.signature(foo),
             {"some_inner": "container"},
-            ("some", "list"),
+            ["some", "list"],
             c_kw=3,
             d_kw=4,
         )
     ] = 2
 
 
 def test_should_work_for_class_methods_as_well():
```

### Comparing `pytest_when-1.0.8/tests/test_integration.py` & `pytest_when-1.0.9/tests/test_integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -296,7 +296,17 @@
         example_module.some_foo_with_variadic_args_kwargs(1, a=2) == "Mocked"
     )
     assert (
         example_module.some_foo_with_variadic_args_kwargs(1, a=3)
         == "Not mocked"
     )
     patched_foo.assert_called()
+
+
+def test_should_work_with_foo_without_args(when):
+    patched_foo = (
+        when(example_module, "some_foo_without_args")
+        .called_with()
+        .then_return("Mocked")
+    )
+    assert example_module.some_foo_without_args() == "Mocked"
+    patched_foo.assert_called()
```

### Comparing `pytest_when-1.0.8/PKG-INFO` & `pytest_when-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-when
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utility which makes mocking more readable and controllable
 Author-Email: zhukovgreen <iam+pytest-when@zhukovgreen.pro>
 Project-URL: Repository, https://github.com/zhukovgreen/pytest-when
 Requires-Python: >=3.8
 Requires-Dist: pytest>=7.3.1
 Requires-Dist: pytest-mock>=3.10.0
 Requires-Dist: typing-extensions>=4.5.0
```

