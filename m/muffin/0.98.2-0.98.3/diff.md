# Comparing `tmp/muffin-0.98.2.tar.gz` & `tmp/muffin-0.98.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.98.2.tar", max compression
+gzip compressed data, was "muffin-0.98.3.tar", max compression
```

## Comparing `muffin-0.98.2.tar` & `muffin-0.98.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-05-23 08:30:43.619541 muffin-0.98.2/README.rst
--rw-r--r--   0        0        0      982 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/__init__.py
--rw-r--r--   0        0        0     5237 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/app.py
--rw-r--r--   0        0        0       71 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/errors.py
--rw-r--r--   0        0        0     3754 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/handler.py
--rw-r--r--   0        0        0     8805 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/manage.py
--rw-r--r--   0        0        0     2857 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/py.typed
--rw-r--r--   0        0        0     2705 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/types.py
--rw-r--r--   0        0        0     2748 2023-05-23 08:30:43.619541 muffin-0.98.2/muffin/utils.py
--rw-r--r--   0        0        0     2990 2023-05-23 08:30:43.619541 muffin-0.98.2/pyproject.toml
--rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.98.2/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-06-05 09:51:52.939155 muffin-0.98.3/README.rst
+-rw-r--r--   0        0        0      982 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/__init__.py
+-rw-r--r--   0        0        0     5257 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/errors.py
+-rw-r--r--   0        0        0     3754 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/handler.py
+-rw-r--r--   0        0        0     8805 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/manage.py
+-rw-r--r--   0        0        0     2857 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/py.typed
+-rw-r--r--   0        0        0     2705 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/types.py
+-rw-r--r--   0        0        0     2888 2023-06-05 09:51:52.939155 muffin-0.98.3/muffin/utils.py
+-rw-r--r--   0        0        0     2990 2023-06-05 09:51:52.943155 muffin-0.98.3/pyproject.toml
+-rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.98.3/PKG-INFO
```

### Comparing `muffin-0.98.2/README.rst` & `muffin-0.98.3/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.98.2/muffin/__init__.py` & `muffin-0.98.3/muffin/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.2/muffin/app.py` & `muffin-0.98.3/muffin/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         """Support background tasks."""
         await self.lifespan(scope, receive, send)
         bgtasks = BACKGROUND_TASK.get()
         if bgtasks is not None:
             await aio_wait(*bgtasks)
             BACKGROUND_TASK.set(None)
 
-    def import_submodules(self, *submodules: str, silent: bool = False):
+    def import_submodules(self, *submodules: str, silent: bool = False, **kwargs):
         """Automatically import submodules.
 
         .. code-block:: python
 
             # Somewhere in package "__init__.py" file
 
             # import all submodules
@@ -129,15 +129,15 @@
 
             # ignore import errors
             app.import_submodules(silent=True)
 
         """
         parent_frame = stack()[1][0]
         package_name = parent_frame.f_locals["__name__"]
-        return import_submodules(package_name, *submodules, silent=silent)
+        return import_submodules(package_name, *submodules, silent=silent, **kwargs)
 
     def run_after_response(self, *tasks: Awaitable):
         """Await the given awaitable after the response is completed.
 
         .. code-block:: python
 
             from muffin import Application
```

### Comparing `muffin-0.98.2/muffin/errors.py` & `muffin-0.98.3/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.2/muffin/handler.py` & `muffin-0.98.3/muffin/handler.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.2/muffin/manage.py` & `muffin-0.98.3/muffin/manage.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.2/muffin/plugins.py` & `muffin-0.98.3/muffin/plugins.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.2/muffin/pytest.py` & `muffin-0.98.3/muffin/pytest.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.2/muffin/utils.py` & `muffin-0.98.3/muffin/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import pkgutil
 import sys
 import threading
 from collections import OrderedDict
 from contextlib import suppress
 from logging import getLogger
-from typing import TYPE_CHECKING, Callable, Coroutine, Dict, TypeVar
+from typing import TYPE_CHECKING, Callable, Coroutine, Dict, Iterable, TypeVar
 
 from asgi_tools.utils import is_awaitable, to_awaitable
 from sniffio import current_async_library
 
 from muffin.errors import InvalidAppError
 
 if TYPE_CHECKING:
@@ -73,22 +73,24 @@
     if aiolib == "asyncio":
         return asyncio.run(corofn(*args, **kwargs))
 
     return AIOLIBS[aiolib].run(lambda: corofn(*args, **kwargs))
 
 
 def import_submodules(
-    package_name: str, *module_names: str, silent: bool = False
+    package_name: str, *module_names: str, silent: bool = False, exclude: Iterable[str] = ()
 ) -> Dict[str, ModuleType]:
     """Import all submodules by the given package name."""
     package = sys.modules[package_name]
     res = {}
-    for module_name in module_names or (
-        name for _, name, _ in pkgutil.walk_packages(package.__path__)
-    ):
+    to_import = module_names or (name for _, name, _ in pkgutil.walk_packages(package.__path__))
+    if exclude:
+        to_import = (name for name in to_import if name not in exclude)
+
+    for module_name in to_import:
         try:
             res[module_name] = importlib.import_module(f"{package_name}.{module_name}")
         except ImportError:
             if not silent:
                 raise
 
             logger.debug("Failed to import module: %s", f"{package_name}.{module_name}")
```

### Comparing `muffin-0.98.2/pyproject.toml` & `muffin-0.98.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.98.2"
+version = "0.98.3"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin-0.98.2/PKG-INFO` & `muffin-0.98.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.98.2
+Version: 0.98.3
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

