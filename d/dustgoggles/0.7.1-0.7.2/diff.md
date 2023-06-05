# Comparing `tmp/dustgoggles-0.7.1.tar.gz` & `tmp/dustgoggles-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dustgoggles-0.7.1.tar", last modified: Tue May 23 10:03:42 2023, max compression
+gzip compressed data, was "dustgoggles-0.7.2.tar", last modified: Mon Jun  5 13:54:05 2023, max compression
```

## Comparing `dustgoggles-0.7.1.tar` & `dustgoggles-0.7.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-23 17:27:12.689968 dustgoggles-0.7.1/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1524 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/LICENSE
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      326 2023-05-23 17:27:12.686968 dustgoggles-0.7.1/PKG-INFO
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-23 17:27:12.206017 dustgoggles-0.7.1/dustgoggles/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       22 2023-05-23 17:20:52.000000 dustgoggles-0.7.1/dustgoggles/__init__.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-23 17:27:12.566031 dustgoggles-0.7.1/dustgoggles/codex/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/codex/__init__.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3518 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/codex/_array_holding_area.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5794 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/codex/codecs.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    33342 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/codex/implements.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3351 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/codex/memutilz.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     8366 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/composition.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5842 2023-05-23 17:19:20.000000 dustgoggles-0.7.1/dustgoggles/dynamic.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3738 2023-05-17 00:39:32.000000 dustgoggles-0.7.1/dustgoggles/func.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5422 2023-02-21 14:57:17.000000 dustgoggles-0.7.1/dustgoggles/mosaic.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     8593 2023-05-23 17:19:20.000000 dustgoggles-0.7.1/dustgoggles/pivot.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     4035 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/scrape.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    13514 2023-05-23 17:19:20.000000 dustgoggles-0.7.1/dustgoggles/structures.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-23 17:27:12.654385 dustgoggles-0.7.1/dustgoggles/test_utils/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       20 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/test_utils/__init__.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     2519 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/test_utils/core.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-23 17:27:12.351568 dustgoggles-0.7.1/dustgoggles.egg-info/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      326 2023-05-23 17:27:11.000000 dustgoggles-0.7.1/dustgoggles.egg-info/PKG-INFO
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      602 2023-05-23 17:27:11.000000 dustgoggles-0.7.1/dustgoggles.egg-info/SOURCES.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)        1 2023-05-23 17:27:11.000000 dustgoggles-0.7.1/dustgoggles.egg-info/dependency_links.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       87 2023-05-23 17:27:11.000000 dustgoggles-0.7.1/dustgoggles.egg-info/requires.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       12 2023-05-23 17:27:11.000000 dustgoggles-0.7.1/dustgoggles.egg-info/top_level.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       38 2023-05-23 17:27:12.691966 dustgoggles-0.7.1/setup.cfg
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      494 2023-05-23 17:20:52.000000 dustgoggles-0.7.1/setup.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     1524 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/LICENSE
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      326 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/PKG-INFO
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 13:54:05.427861 dustgoggles-0.7.2/dustgoggles/
+-rw-r--r--   0 sierra    (1000) sierra    (1000)       22 2023-06-05 13:50:03.000000 dustgoggles-0.7.2/dustgoggles/__init__.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/dustgoggles/codex/
+-rw-r--r--   0 sierra    (1000) sierra    (1000)        0 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/codex/__init__.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     3518 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/codex/_array_holding_area.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     5794 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/codex/codecs.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)    33342 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/codex/implements.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     3351 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/codex/memutilz.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     9250 2023-05-30 13:53:39.000000 dustgoggles-0.7.2/dustgoggles/composition.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     6086 2023-05-30 13:53:39.000000 dustgoggles-0.7.2/dustgoggles/dynamic.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     3738 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/func.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     5422 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/mosaic.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     8586 2023-06-05 13:31:46.000000 dustgoggles-0.7.2/dustgoggles/pivot.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     4035 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/scrape.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)    13514 2023-05-30 13:53:39.000000 dustgoggles-0.7.2/dustgoggles/structures.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/dustgoggles/test_utils/
+-rw-r--r--   0 sierra    (1000) sierra    (1000)       20 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/test_utils/__init__.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     2519 2023-05-30 13:48:19.000000 dustgoggles-0.7.2/dustgoggles/test_utils/core.py
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     2036 2023-05-30 13:53:39.000000 dustgoggles-0.7.2/dustgoggles/tracker.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/dustgoggles.egg-info/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      326 2023-06-05 13:54:05.000000 dustgoggles-0.7.2/dustgoggles.egg-info/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      625 2023-06-05 13:54:05.000000 dustgoggles-0.7.2/dustgoggles.egg-info/SOURCES.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2023-06-05 13:54:05.000000 dustgoggles-0.7.2/dustgoggles.egg-info/dependency_links.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       87 2023-06-05 13:54:05.000000 dustgoggles-0.7.2/dustgoggles.egg-info/requires.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       12 2023-06-05 13:54:05.000000 dustgoggles-0.7.2/dustgoggles.egg-info/top_level.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2023-06-05 13:54:05.431861 dustgoggles-0.7.2/setup.cfg
+-rw-r--r--   0 sierra    (1000) sierra    (1000)      494 2023-06-05 13:50:03.000000 dustgoggles-0.7.2/setup.py
```

### Comparing `dustgoggles-0.7.1/LICENSE` & `dustgoggles-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.1/dustgoggles/codex/_array_holding_area.py` & `dustgoggles-0.7.2/dustgoggles/codex/_array_holding_area.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.1/dustgoggles/codex/codecs.py` & `dustgoggles-0.7.2/dustgoggles/codex/codecs.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.1/dustgoggles/codex/implements.py` & `dustgoggles-0.7.2/dustgoggles/codex/implements.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.1/dustgoggles/codex/memutilz.py` & `dustgoggles-0.7.2/dustgoggles/codex/memutilz.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.1/dustgoggles/composition.py` & `dustgoggles-0.7.2/dustgoggles/composition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from operator import attrgetter
 from typing import Optional, Union, Mapping, Any, Callable, Sequence, Hashable
 
 from cytoolz import identity, keyfilter, first
 
 from dustgoggles.func import naturals
 from dustgoggles.structures import enumerate_as_mapping, reindex_mapping
+from dustgoggles.tracker import TrivialTracker
 
 
 class Composition:
     """
     class defining a composition of steps, optionally with
     additional input, output, and i/o points ("inserts" and "sends") --
     conceptually like a signal processing chain but _not_ designed for
@@ -18,38 +19,57 @@
         self,
         steps: Optional[
             Union[Mapping[Any, Callable], Sequence[Callable]]
         ] = None,
         sends: Optional[Union[Mapping[Any, Sequence], Sequence]] = None,
         inserts: Optional[
             Union[Mapping[Any, Mapping], Sequence[Mapping]]
-        ] = None
+        ] = None,
+        name: Optional[str] = None,
+        tracker: Optional[TrivialTracker] = None
     ):
+        self.name = "untitled Composition" if name is None else name
+        if tracker is not None:
+            tracker.name = self.name
+        self.tracker = tracker
         if steps is None:
             steps = [identity]
         self.steps = enumerate_as_mapping(steps)
+        self.tracker = tracker
         # sends and inserts could be defaultdicts, but in this case the
         # representation is ugly and the convenience is small.
         self.sends = enumerate_as_mapping(sends)
         self.inserts = enumerate_as_mapping(inserts)
+        if self.tracker is not None:
+            for k in self.steps.keys():
+                self._add_track_send(k)
 
     def _check_for_step(self, step_name: Hashable) -> Any:
         if step_name not in self.steps.keys():
             raise KeyError(f"{step_name} is not an element of the pipeline.")
         return self.steps[step_name]
 
-    def add_step(self, step, name=None):
+    def add_step(self, step: Callable, name: Optional[Hashable] = None):
         """
         add step with name "name" -- by default, length of the pipeline + 1.
         if no step with that name currently exists, add it to the end of the
         pipeline; otherwise, replace the current step at "name".
         """
         if name is None:
             name = len(self.steps) + 1
         self.steps[name] = step
+        self._add_track_send(name)
+
+    def _add_track_send(self, step_name: Hashable):
+        if self.tracker is None:
+            return
+        self.add_send(
+            step_name,
+            pipe=_track_factory(self.tracker, step_name, self.steps[step_name])
+        )
 
     def reindex(self):
         self.steps = reindex_mapping(self.steps)
 
     @property
     def index(self):
         return tuple(self.steps.keys())
@@ -220,7 +240,15 @@
         return me_string
 
     def __repr__(self):
         return self.__str__()
 
     def __call__(self, *args, **kwargs):
         return self.execute(*args, **kwargs)
+
+
+def _track_factory(tracker, step, func):
+
+    def track(_):
+        return tracker.track(func, step=step)
+
+    return track
```

### Comparing `dustgoggles-0.7.1/dustgoggles/dynamic.py` & `dustgoggles-0.7.2/dustgoggles/dynamic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """utilities for dynamic function generation and code introspection"""
 import datetime as dt
 import traceback
 from inspect import getsource, signature, Signature
-from types import FunctionType, CodeType
+from types import FunctionType, CodeType, MethodType
 from typing import Optional, Callable, MutableSequence
 
 from cytoolz import nth
 
 from dustgoggles.func import optionalize
 
 
@@ -24,15 +24,15 @@
 #  to engage in really high call volume, you could also just explicitly call
 #  the wrapped function...
 def digsource(obj: Callable):
     """
     wrapper for inspect.getsource that attempts to work on objects like
     Dynamic, functools.partial, etc.
     """
-    if isinstance(obj, FunctionType):
+    if isinstance(obj, (FunctionType, MethodType)):
         return getsource(obj)
     if "func" in dir(obj):
         # noinspection PyUnresolvedReferences
         return getsource(obj.func)
     raise TypeError(f"cannot get source for type {type(obj)}")
 
 
@@ -55,15 +55,15 @@
     globals_ = globals_ if globals_ is not None else globals()
     return FunctionType(code, globals_)
 
 
 def exc_report(exc):
     if exc is None:
         return {}
-    stack = traceback.extract_stack()[:-3]
+    stack = traceback.extract_tb(exc.__traceback__)[:-2]
     return {
         "exception": exc,
         "lineno": tuple([a.lineno for a in stack]),
         "stack": tuple([a.name for a in stack]),
         "time": dt.datetime.now().isoformat()[:-3],
     }
 
@@ -157,19 +157,24 @@
             return self.__class__.__name__
         return f"{self.__class__.__name__} {signature(self.func)}"
 
     def __repr__(self):
         return self.__str__()
 
     @classmethod
-    def from_function(cls, func: FunctionType, *init_args, **init_kwargs):
+    def from_function(cls, func: Callable, *init_args, **init_kwargs):
         # TODO: some of this boilerplate could be reduced with a bunch of
         #  fancy getattr overrides
         dynamic = super().__new__(cls)
-        dynamic.source = digsource(func)
+        try:
+            dynamic.source = getsource(func)
+        except TypeError:  # it's some kind of weirdo callable
+            # noinspection PyUnresolvedReferences
+            func = func.__call__
+            dynamic.source = getsource(func)
         dynamic.code = func.__code__
         dynamic.func = func
         dynamic.__signature__ = signature(dynamic.func)
         dynamic.__name__ = dynamic.func.__name__
         dynamic.globals_ = func.__globals__
         dynamic.__init__(*init_args, **init_kwargs)
         return dynamic
```

### Comparing `dustgoggles-0.7.1/dustgoggles/func.py` & `dustgoggles-0.7.2/dustgoggles/func.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.1/dustgoggles/mosaic.py` & `dustgoggles-0.7.2/dustgoggles/mosaic.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.1/dustgoggles/pivot.py` & `dustgoggles-0.7.2/dustgoggles/pivot.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,31 +69,30 @@
     elif how == "columns":
         axis = 1
     else:
         raise ValueError(f"unknown how {how}")
     try:
         constant_indices = df.nunique(axis=axis, dropna=dropna) <= 1
     except TypeError:
-        constant_indices = []
+        if axis == 1:
+            raise NotImplementedError("nested fields not supported columnwise")
+        constant_indices = pd.Series(False, df.columns)
         for c in df.columns:
             if isinstance(df[c].iloc[0], list):
                 test_series = df[c].map(tuple)
             else:
                 test_series = df[c]
             if test_series.nunique(dropna=dropna) <= 1:
-                constant_indices.append(c)
-
+                constant_indices.loc[c] = True
     if axis == 0:
-        var_indices = [c for c in df.columns if c not in constant_indices]
         constants = df.loc[:, constant_indices]
-        variables = df.loc[:, var_indices]
+        variables = df.loc[:, ~constant_indices]
     else:
-        var_indices = [c for c in df.indices if c not in constant_indices]
         constants = df.loc[constant_indices]
-        variables = df.loc[var_indices]
+        variables = df.loc[~constant_indices]
     if to_dict:
         constants = constants.iloc[0].to_dict()
     if drop_constants:
         return constants, variables
     return constants, df
```

### Comparing `dustgoggles-0.7.1/dustgoggles/scrape.py` & `dustgoggles-0.7.2/dustgoggles/scrape.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.1/dustgoggles/structures.py` & `dustgoggles-0.7.2/dustgoggles/structures.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.1/dustgoggles/test_utils/core.py` & `dustgoggles-0.7.2/dustgoggles/test_utils/core.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.1/dustgoggles.egg-info/SOURCES.txt` & `dustgoggles-0.7.2/dustgoggles.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 dustgoggles/composition.py
 dustgoggles/dynamic.py
 dustgoggles/func.py
 dustgoggles/mosaic.py
 dustgoggles/pivot.py
 dustgoggles/scrape.py
 dustgoggles/structures.py
+dustgoggles/tracker.py
 dustgoggles.egg-info/PKG-INFO
 dustgoggles.egg-info/SOURCES.txt
 dustgoggles.egg-info/dependency_links.txt
 dustgoggles.egg-info/requires.txt
 dustgoggles.egg-info/top_level.txt
 dustgoggles/codex/__init__.py
 dustgoggles/codex/_array_holding_area.py
```

