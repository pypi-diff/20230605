# Comparing `tmp/muffin-0.98.3.tar.gz` & `tmp/muffin-0.98.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.98.3.tar", max compression
+gzip compressed data, was "muffin-0.98.5.tar", max compression
```

## Comparing `muffin-0.98.3.tar` & `muffin-0.98.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-06-05 09:51:52.939155 muffin-0.98.3/README.rst
--rw-r--r--   0        0        0      982 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/__init__.py
--rw-r--r--   0        0        0     5257 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/app.py
--rw-r--r--   0        0        0       71 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/errors.py
--rw-r--r--   0        0        0     3754 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/handler.py
--rw-r--r--   0        0        0     8805 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/manage.py
--rw-r--r--   0        0        0     2857 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/py.typed
--rw-r--r--   0        0        0     2705 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/types.py
--rw-r--r--   0        0        0     2888 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/utils.py
--rw-r--r--   0        0        0     2990 2023-06-05 09:51:52.943155 muffin-0.98.3/pyproject.toml
--rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.98.3/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-06-05 13:17:23.378887 muffin-0.98.5/README.rst
+-rw-r--r--   0        0        0      982 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/__init__.py
+-rw-r--r--   0        0        0     5257 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/errors.py
+-rw-r--r--   0        0        0     3781 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/handler.py
+-rw-r--r--   0        0        0     8805 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/manage.py
+-rw-r--r--   0        0        0     2857 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/py.typed
+-rw-r--r--   0        0        0     2705 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/types.py
+-rw-r--r--   0        0        0     2888 2023-06-05 13:17:23.382887 muffin-0.98.5/muffin/utils.py
+-rw-r--r--   0        0        0     2990 2023-06-05 13:17:23.382887 muffin-0.98.5/pyproject.toml
+-rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.98.5/PKG-INFO
```

### Comparing `muffin-0.98.3/README.rst` & `muffin-0.98.5/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.98.3/muffin/__init__.py` & `muffin-0.98.5/muffin/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.3/muffin/app.py` & `muffin-0.98.5/muffin/app.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.3/muffin/errors.py` & `muffin-0.98.5/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.3/muffin/handler.py` & `muffin-0.98.5/muffin/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,39 +84,37 @@
 
     """
 
     methods: Optional[TMethods] = None
 
     @classmethod
     def __route__(
-        cls,
-        router: "Router",
-        *paths: str,
-        methods: Optional[TMethodsArg] = None,
-        **params,
+        cls, router: Router, *paths: str, methods: Optional[TMethodsArg] = None, **params
     ):
         """Check for registered methods."""
         router.bind(cls, *paths, methods=methods or cls.methods, **params)
         for _, method in inspect.getmembers(cls, lambda m: hasattr(m, "__route__")):
-            cpaths, cparams = method.__route__
-            router.bind(cls, *cpaths, __meth__=method.__name__, **cparams)
+            paths, methods = method.__route__
+            router.bind(cls, *paths, methods=methods, method=method.__name__)
 
         return cls
 
-    def __call__(self, request: "Request", **opts) -> Awaitable:
+    def __call__(self, request: Request, *, method: Optional[str] = None, **_) -> Awaitable:
         """Dispatch the given request by HTTP method."""
-        method = getattr(self, opts.get("__meth__") or request.method.lower())
-        return method(request)
+        process = getattr(self, method or request.method.lower())
+        return process(request)
 
     @staticmethod
-    def route(*paths: str, **params) -> Callable[[TVCallable], TVCallable]:
+    def route(
+        *paths: str, methods: Optional[TMethodsArg] = None
+    ) -> Callable[[TVCallable], TVCallable]:
         """Mark a method as a route."""
 
         def wrapper(method):
             """Wrap a method."""
-            method.__route__ = paths, params
+            method.__route__ = paths, methods
             return method
 
         return wrapper
 
 
 route_method = Handler.route
```

### Comparing `muffin-0.98.3/muffin/manage.py` & `muffin-0.98.5/muffin/manage.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.3/muffin/plugins.py` & `muffin-0.98.5/muffin/plugins.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.3/muffin/pytest.py` & `muffin-0.98.5/muffin/pytest.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.3/muffin/utils.py` & `muffin-0.98.5/muffin/utils.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.3/pyproject.toml` & `muffin-0.98.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.98.3"
+version = "0.98.5"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin-0.98.3/PKG-INFO` & `muffin-0.98.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.98.3
+Version: 0.98.5
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

