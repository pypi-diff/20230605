# Comparing `tmp/genki_signals-0.1.1.tar.gz` & `tmp/genki_signals-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genki_signals-0.1.1.tar", last modified: Fri May 19 17:57:56 2023, max compression
+gzip compressed data, was "genki_signals-1.0.0.tar", last modified: Mon Jun  5 11:34:19 2023, max compression
```

## Comparing `genki_signals-0.1.1.tar` & `genki_signals-1.0.0.tar`

### file list

```diff
@@ -1,47 +1,52 @@
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.071357 genki_signals-0.1.1/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1108 2023-05-19 17:57:56.071144 genki_signals-0.1.1/PKG-INFO
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      592 2023-05-19 11:53:35.000000 genki_signals-0.1.1/README.md
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.062967 genki_signals-0.1.1/genki_signals/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      537 2023-05-19 17:56:29.000000 genki_signals-0.1.1/genki_signals/__init__.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     8700 2023-05-10 16:26:33.000000 genki_signals-0.1.1/genki_signals/buffers.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2233 2023-05-16 15:12:05.000000 genki_signals-0.1.1/genki_signals/dead_reckoning.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     8182 2023-05-10 13:32:35.000000 genki_signals-0.1.1/genki_signals/filters.py
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.065029 genki_signals-0.1.1/genki_signals/frontends/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       94 2023-05-19 15:44:12.000000 genki_signals-0.1.1/genki_signals/frontends/__init__.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      429 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/frontends/base.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)    11322 2023-05-19 17:56:29.000000 genki_signals-0.1.1/genki_signals/frontends/visualization.py
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.068276 genki_signals-0.1.1/genki_signals/functions/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      964 2023-05-19 17:56:29.000000 genki_signals-0.1.1/genki_signals/functions/__init__.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     5492 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/arithmetic.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1666 2023-05-19 15:08:48.000000 genki_signals-0.1.1/genki_signals/functions/base.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3197 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/filters.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)    13660 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/geometry.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2433 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/inference.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      880 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/serialization.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3702 2023-05-19 17:56:29.000000 genki_signals-0.1.1/genki_signals/functions/shape.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1946 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/waveforms.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     4756 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/windowed.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1008 2023-05-16 15:12:05.000000 genki_signals-0.1.1/genki_signals/fusion.py
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.068524 genki_signals-0.1.1/genki_signals/models/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2445 2023-05-04 16:25:52.000000 genki_signals-0.1.1/genki_signals/models/letter_detection_model.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2489 2023-05-16 14:58:32.000000 genki_signals-0.1.1/genki_signals/recorders.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     5542 2023-05-19 15:08:48.000000 genki_signals-0.1.1/genki_signals/session.py
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.070824 genki_signals-0.1.1/genki_signals/sources/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      660 2023-05-19 17:56:29.000000 genki_signals-0.1.1/genki_signals/sources/__init__.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      376 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/base.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     4871 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/ble.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2301 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/dataframe.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      337 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/generators.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     4828 2023-05-19 15:21:22.000000 genki_signals-0.1.1/genki_signals/sources/local.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2596 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/sampler.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3935 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/wave.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3393 2023-05-19 15:08:48.000000 genki_signals-0.1.1/genki_signals/system.py
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.064196 genki_signals-0.1.1/genki_signals.egg-info/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1108 2023-05-19 17:57:56.000000 genki_signals-0.1.1/genki_signals.egg-info/PKG-INFO
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1200 2023-05-19 17:57:56.000000 genki_signals-0.1.1/genki_signals.egg-info/SOURCES.txt
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)        1 2023-05-19 17:57:56.000000 genki_signals-0.1.1/genki_signals.egg-info/dependency_links.txt
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      115 2023-05-19 17:57:56.000000 genki_signals-0.1.1/genki_signals.egg-info/requires.txt
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       14 2023-05-19 17:57:56.000000 genki_signals-0.1.1/genki_signals.egg-info/top_level.txt
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       31 2023-05-17 15:55:12.000000 genki_signals-0.1.1/pyproject.toml
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       38 2023-05-19 17:57:56.071423 genki_signals-0.1.1/setup.cfg
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1625 2023-05-19 17:57:45.000000 genki_signals-0.1.1/setup.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-06-05 11:34:19.683950 genki_signals-1.0.0/
+-rw-r--r--   0 egill      (501) staff       (20)     1108 2023-06-05 11:34:19.683779 genki_signals-1.0.0/PKG-INFO
+-rw-r--r--   0 egill      (501) staff       (20)      592 2023-05-19 11:25:16.000000 genki_signals-1.0.0/README.md
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-06-05 11:34:19.677153 genki_signals-1.0.0/genki_signals/
+-rw-r--r--   0 egill      (501) staff       (20)      732 2023-06-05 11:23:23.000000 genki_signals-1.0.0/genki_signals/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)     9626 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/buffers.py
+-rw-r--r--   0 egill      (501) staff       (20)     2233 2023-04-26 14:10:30.000000 genki_signals-1.0.0/genki_signals/dead_reckoning.py
+-rw-r--r--   0 egill      (501) staff       (20)     8182 2023-04-26 14:10:30.000000 genki_signals-1.0.0/genki_signals/filters.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-06-05 11:34:19.678818 genki_signals-1.0.0/genki_signals/frontends/
+-rw-r--r--   0 egill      (501) staff       (20)       95 2023-05-30 15:29:15.000000 genki_signals-1.0.0/genki_signals/frontends/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)      429 2023-05-19 15:11:59.000000 genki_signals-1.0.0/genki_signals/frontends/base.py
+-rw-r--r--   0 egill      (501) staff       (20)    11707 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/frontends/visualization.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-06-05 11:34:19.681148 genki_signals-1.0.0/genki_signals/functions/
+-rw-r--r--   0 egill      (501) staff       (20)      964 2023-05-23 13:33:31.000000 genki_signals-1.0.0/genki_signals/functions/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)     5812 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/functions/arithmetic.py
+-rw-r--r--   0 egill      (501) staff       (20)     1666 2023-05-19 15:11:59.000000 genki_signals-1.0.0/genki_signals/functions/base.py
+-rw-r--r--   0 egill      (501) staff       (20)     3200 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/functions/filters.py
+-rw-r--r--   0 egill      (501) staff       (20)    13660 2023-05-19 15:11:59.000000 genki_signals-1.0.0/genki_signals/functions/geometry.py
+-rw-r--r--   0 egill      (501) staff       (20)     2584 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/functions/inference.py
+-rw-r--r--   0 egill      (501) staff       (20)      966 2023-06-01 14:29:01.000000 genki_signals-1.0.0/genki_signals/functions/serialization.py
+-rw-r--r--   0 egill      (501) staff       (20)     3680 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/functions/shape.py
+-rw-r--r--   0 egill      (501) staff       (20)     2015 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/functions/waveforms.py
+-rw-r--r--   0 egill      (501) staff       (20)     4769 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/functions/windowed.py
+-rw-r--r--   0 egill      (501) staff       (20)     1008 2023-04-26 14:10:30.000000 genki_signals-1.0.0/genki_signals/fusion.py
+-rw-r--r--   0 egill      (501) staff       (20)     3097 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/recorders.py
+-rw-r--r--   0 egill      (501) staff       (20)     5843 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/session.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-06-05 11:34:19.682707 genki_signals-1.0.0/genki_signals/sources/
+-rw-r--r--   0 egill      (501) staff       (20)      660 2023-05-23 13:33:31.000000 genki_signals-1.0.0/genki_signals/sources/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)      376 2023-05-19 15:11:59.000000 genki_signals-1.0.0/genki_signals/sources/base.py
+-rw-r--r--   0 egill      (501) staff       (20)     4839 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/sources/ble.py
+-rw-r--r--   0 egill      (501) staff       (20)     2301 2023-05-19 15:11:59.000000 genki_signals-1.0.0/genki_signals/sources/dataframe.py
+-rw-r--r--   0 egill      (501) staff       (20)      337 2023-05-19 15:11:59.000000 genki_signals-1.0.0/genki_signals/sources/generators.py
+-rw-r--r--   0 egill      (501) staff       (20)     4800 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/sources/local.py
+-rw-r--r--   0 egill      (501) staff       (20)     2597 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/sources/sampler.py
+-rw-r--r--   0 egill      (501) staff       (20)     3935 2023-05-19 15:11:59.000000 genki_signals-1.0.0/genki_signals/sources/wave.py
+-rw-r--r--   0 egill      (501) staff       (20)     3792 2023-06-05 11:11:23.000000 genki_signals-1.0.0/genki_signals/system.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-06-05 11:34:19.678017 genki_signals-1.0.0/genki_signals.egg-info/
+-rw-r--r--   0 egill      (501) staff       (20)     1108 2023-06-05 11:34:19.000000 genki_signals-1.0.0/genki_signals.egg-info/PKG-INFO
+-rw-r--r--   0 egill      (501) staff       (20)     1352 2023-06-05 11:34:19.000000 genki_signals-1.0.0/genki_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 egill      (501) staff       (20)        1 2023-06-05 11:34:19.000000 genki_signals-1.0.0/genki_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 egill      (501) staff       (20)      115 2023-06-05 11:34:19.000000 genki_signals-1.0.0/genki_signals.egg-info/requires.txt
+-rw-r--r--   0 egill      (501) staff       (20)       20 2023-06-05 11:34:19.000000 genki_signals-1.0.0/genki_signals.egg-info/top_level.txt
+-rw-r--r--   0 egill      (501) staff       (20)       31 2023-04-26 14:10:30.000000 genki_signals-1.0.0/pyproject.toml
+-rw-r--r--   0 egill      (501) staff       (20)       38 2023-06-05 11:34:19.684010 genki_signals-1.0.0/setup.cfg
+-rw-r--r--   0 egill      (501) staff       (20)     1549 2023-06-05 11:11:23.000000 genki_signals-1.0.0/setup.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-06-05 11:34:19.674574 genki_signals-1.0.0/tests/
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-06-05 11:34:19.683558 genki_signals-1.0.0/tests/signal_functions/
+-rw-r--r--   0 egill      (501) staff       (20)        0 2023-05-19 15:11:59.000000 genki_signals-1.0.0/tests/signal_functions/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)     4137 2023-06-05 11:11:23.000000 genki_signals-1.0.0/tests/signal_functions/test_arithmetic.py
+-rw-r--r--   0 egill      (501) staff       (20)      891 2023-06-05 11:11:23.000000 genki_signals-1.0.0/tests/signal_functions/test_geometry.py
+-rw-r--r--   0 egill      (501) staff       (20)     1047 2023-06-05 11:11:23.000000 genki_signals-1.0.0/tests/signal_functions/test_serialization.py
+-rw-r--r--   0 egill      (501) staff       (20)     4957 2023-06-05 11:11:23.000000 genki_signals-1.0.0/tests/signal_functions/test_shape.py
```

### Comparing `genki_signals-0.1.1/PKG-INFO` & `genki_signals-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genki_signals
-Version: 0.1.1
+Version: 1.0.0
 Summary: A library for realtime signal processing and machine learning
 Home-page: https://github.com/genkiinstruments/genki-signals
 Author: Genki Instruments
 Author-email: genki@genkiinstruments.com
 Keywords: Signal Processing,Machine Learning,Realtime
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `genki_signals-0.1.1/README.md` & `genki_signals-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.1/genki_signals/buffers.py` & `genki_signals-1.0.0/genki_signals/buffers.py`

 * *Files 10% similar despite different names*

```diff
@@ -196,15 +196,36 @@
 
     # ==============
     # Serialization
     # ==============
 
     @classmethod
     def from_dataframe(cls, df, maxlen=None):
-        return cls(maxlen=maxlen, data={k: df[k].values for k in df.columns})
+        split = re.compile(r"(?P<name>\D+)_(?P<number>(\d+)(_\d+)?(_\d+)?)")
+        data = {}
+        composite_data = {}
+        for col in df.columns:
+            m = split.match(col)
+            if m is not None:
+                name, number = m.groupdict()["name"], m.groupdict()["number"]
+                number = tuple(map(int, number.split("_")))
+                if name not in composite_data:
+                    composite_data[name] = []
+                composite_data[name].append((number, df[col].values))
+            else:
+                data[col] = df[col].values
+        for name, values in composite_data.items():
+            values = sorted(values, key=lambda x: x[0])
+            pt_shape = tuple(d + 1 for d in values[-1][0])
+            t_shape = values[0][1].shape
+            arr = np.zeros((*pt_shape, *t_shape), dtype=values[0][1].dtype)
+            for idx, pts in values:
+                arr[idx] = pts
+            data[name] = arr
+        return cls(maxlen=maxlen, data=data)
 
     def to_dataframe(self):
         flat_data = {}
         for k, v in self._data.items():
             if v.ndim == 1:
                 flat_data[k] = v
             elif v.ndim == 2:
```

### Comparing `genki_signals-0.1.1/genki_signals/dead_reckoning.py` & `genki_signals-1.0.0/genki_signals/dead_reckoning.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.1/genki_signals/filters.py` & `genki_signals-1.0.0/genki_signals/filters.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.1/genki_signals/frontends/visualization.py` & `genki_signals-1.0.0/genki_signals/frontends/visualization.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 from __future__ import annotations
 
 import math
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from typing import Literal
 
-import cv2
 import bqplot as bq
+import cv2
 import ipywidgets
-from ipywidgets import Image
 from IPython.display import display
+from ipywidgets import Image
 
 from genki_signals.buffers import DataBuffer
-from genki_signals.system import System
 from genki_signals.frontends.base import FrontendBase
+from genki_signals.system import System
 
 
-class WidgetFrontend(FrontendBase):
-    def __init__(self, system: System, widgets: list[PlottableWidget] = None):
-        super().__init__(system)
-
-        self.widgets = widgets or []
-        self.update_callbacks = {id(widget): widget.update for widget in widgets or []}
-
-    def register_update_callback(self, id, update_fn):
-        self.update_callbacks[id] = update_fn
-
-    def deregister_update_callback(self, id):
-        self.update_callbacks.pop(id)
+class WidgetDashboard:
+    """
+    A simple dashboard for displaying multiple widgets in a grid.
+    """
 
-    def update(self, data: DataBuffer):
-        for update_fn in self.update_callbacks.values():
-            update_fn(data)
+    def __init__(self, widgets: list[PlottableWidget]):
+        self.widgets = widgets
 
     def _ipython_display_(self):
         n = math.ceil(math.sqrt(len(self.widgets)))
         rows = []
         for i in range(n):
             cols = []
             for j in range(n):
@@ -42,81 +33,97 @@
                     cols.append(self.widgets[i * n + j].widget)
                 except IndexError:
                     pass
             rows.append(ipywidgets.HBox(cols))
         return display(ipywidgets.VBox(rows))
 
 
-class PlottableWidget(ABC):
-    def __init__(self):
+class PlottableWidget(FrontendBase):
+    """
+    A base class for jupyter frontends.
+    """
+
+    def __init__(self, system: System):
+        super().__init__(system)
+
         self.widget = None
 
     @abstractmethod
     def update(self, data: DataBuffer):
         pass
 
     def _ipython_display_(self):
         return display(self.widget)
 
 
 class Video(PlottableWidget):
-    def __init__(self, video_key: str):
-        super().__init__()
+    def __init__(self, system: System, video_key: str):
+        super().__init__(system)
 
         self.video_key = video_key
         self.widget = Image(format="jpeg")
 
     def update(self, data: DataBuffer):
-        value = data[self.video_key][..., -1].transpose(2, 1, 0)
+        transpose = (2, 1, 0) if data[self.video_key].ndim == 4 else (1, 0)  # rgb or grayscale
+        value = data[self.video_key][..., -1].transpose(transpose)
         _, jpeg_image = cv2.imencode(".jpeg", value)
         self.widget.value = jpeg_image.tobytes()
 
 
 class Line(PlottableWidget):
     """A line plot of a signal w.r.t. some 1D signal."""
 
     def __init__(
         self,
+        system: System,
         x_access: str | tuple[str, int],
         y_access: str | tuple[str, int] | tuple[str, list[int]],
         x_scale: Literal["linear", "log"] = "linear",
         y_scale: Literal["linear", "log"] = "linear",
         x_range: tuple[float, float] = (None, None),
         y_range: tuple[float, float] = (None, None),
         n_visible_points: int = 200,
+        flip_x: bool = False,
+        flip_y: bool = False,
     ):
         """
         Args:
             x_access: The key of a 1D signal or key index pair of 2D signal which should map to a 1D signal,
                       defines how to access the the x-axis data
             y_access: The key of a signal or key index/indices pair of a 2D signal, defines how to access
                       the y-axis data
             x_scale:  The scale of the x-axis, either "linear" or "log"
             y_scale:  The scale of the y-axis, either "linear" or "log"
             x_range:  The range of the x-axis, defaults to the range of the data at any given time i.e. (min(x), max(x))
             y_range:  The range of the y-axis, defaults to the range of the data at any given time i.e. (min(y), max(y))
             n_visible_points: The number of points to show on the plot
+            flip_x:   If x-axis is inverted or not
+            flip_y:   If y-axis is inverted or not
         """
-        super().__init__()
+        super().__init__(system)
 
         if isinstance(x_access, str):
             x_access = (x_access, None)
         if isinstance(y_access, str):
             y_access = (y_access, None)
 
         x_range = {"min": x_range[0], "max": x_range[1]}
         y_range = {"min": y_range[0], "max": y_range[1]}
 
         self.buffer = DataBuffer(maxlen=n_visible_points)
 
         self.x_key, self.x_idx = x_access
         self.y_key, self.y_idx = y_access
 
-        x_scale = bq.LinearScale(**x_range) if x_scale == "linear" else bq.LogScale(**x_range)
-        y_scale = bq.LinearScale(**y_range) if y_scale == "linear" else bq.LogScale(**y_range)
+        x_scale = (
+            bq.LinearScale(**x_range, reverse=flip_x) if x_scale == "linear" else bq.LogScale(**x_range, reverse=flip_x)
+        )
+        y_scale = (
+            bq.LinearScale(**y_range, reverse=flip_y) if y_scale == "linear" else bq.LogScale(**y_range, reverse=flip_y)
+        )
         self.x_axis = bq.Axis(
             scale=x_scale, label=f"{self.x_key}_{self.x_idx}" if self.x_idx is not None else self.x_key
         )
         self.y_axis = bq.Axis(scale=y_scale, orientation="vertical", label=self.y_key)
         self.line = bq.Lines(x=[], y=[], scales={"x": x_scale, "y": y_scale})
 
         self.widget = bq.Figure(marks=[self.line], axes=[self.x_axis, self.y_axis])
@@ -135,51 +142,60 @@
 
 
 class Scatter(PlottableWidget):
     """A scatter plot of a 1D signal w.r.t. some 1D signal."""
 
     def __init__(
         self,
+        system: System,
         x_access: str | tuple[str, int],
         y_access: str | tuple[str, int],
         x_scale: Literal["linear", "log"] = "linear",
         y_scale: Literal["linear", "log"] = "linear",
         x_range: tuple[float, float] = (None, None),
         y_range: tuple[float, float] = (None, None),
         n_visible_points: int = 200,
+        flip_x: bool = False,
+        flip_y: bool = False,
     ):
         """
         Args:
             x_access: The key of a 1D signal or key index pair of 2D signal which should map to a 1D signal,
                       defines how to access the the x-axis data
             y_access: The key of a 1D signal or key index pair of a 2D signal, which should map to a 1D signal,
                       defines how to access the y-axis data
             x_scale:  The scale of the x-axis, either "linear" or "log"
             y_scale:  The scale of the y-axis, either "linear" or "log"
             x_range:  The range of the x-axis, defaults to the range of the data at any given time i.e. (min(x), max(x))
             y_range:  The range of the y-axis, defaults to the range of the data at any given time i.e. (min(y), max(y))
             n_visible_points: The number of points to show on the plot
+            flip_x:   If x-axis is inverted or not
+            flip_y:   If y-axis is inverted or not
         """
-        super().__init__()
+        super().__init__(system)
 
         if isinstance(x_access, str):
             x_access = (x_access, None)
         if isinstance(y_access, str):
             y_access = (y_access, None)
 
         x_range = {"min": x_range[0], "max": x_range[1]}
         y_range = {"min": y_range[0], "max": y_range[1]}
 
         self.buffer = DataBuffer(maxlen=n_visible_points)
 
         self.x_key, self.x_idx = x_access
         self.y_key, self.y_idx = y_access
 
-        x_scale = bq.LinearScale(**x_range) if x_scale == "linear" else bq.LogScale(**x_range)
-        y_scale = bq.LinearScale(**y_range) if y_scale == "linear" else bq.LogScale(**y_range)
+        x_scale = (
+            bq.LinearScale(**x_range, reverse=flip_x) if x_scale == "linear" else bq.LogScale(**x_range, reverse=flip_x)
+        )
+        y_scale = (
+            bq.LinearScale(**y_range, reverse=flip_y) if y_scale == "linear" else bq.LogScale(**y_range, reverse=flip_y)
+        )
         self.x_axis = bq.Axis(scale=x_scale, label=self.x_key if self.x_idx is None else f"{self.x_key}_{self.x_idx}")
         self.y_axis = bq.Axis(
             scale=y_scale,
             orientation="vertical",
             label=self.y_key if self.y_idx is None else f"{self.y_key}_{self.y_idx}",
         )
         self.scatter = bq.Scatter(x=[], y=[], scales={"x": x_scale, "y": y_scale})
@@ -199,39 +215,43 @@
 
 
 class Histogram(PlottableWidget):
     """A histogram of values from a 1D signal over some lookback window."""
 
     def __init__(
         self,
+        system: System,
         y_access: str | tuple[str, int],
+        x_range: tuple[float, float] = (None, None),
         y_range: tuple[float, float] = (None, None),
         bin_count: int = 10,
         lookback_size: int = 100,
     ):
         """
         Args:
             y_access: The key of a 1D signal or key index pair of a 2D signal, should map to a 1D signal,
                       defines how to access the y-axis data
+            x_range:  The range of the x-axis, defaults to the range of the data at any given time i.e. (min(x), max(x))
             y_range:  The range of the y-axis, defaults to the range of the data at any given time i.e. (min(y), max(y))
             bin_count: The number of bins in the histogram
             lookback_size: The number of points to look back when computing the histogram
         """
-        super().__init__()
+        super().__init__(system)
 
         if isinstance(y_access, str):
             y_access = (y_access, None)
 
+        x_range = {"min": x_range[0], "max": x_range[1]}
         y_range = {"min": y_range[0], "max": y_range[1]}
 
         self.buffer = DataBuffer(maxlen=lookback_size)
 
         self.y_key, self.y_idx = y_access
 
-        x_scale = bq.LinearScale()
+        x_scale = bq.LinearScale(**x_range)
         y_scale = bq.LinearScale(**y_range)
         self.x_axis = bq.Axis(scale=x_scale, tick_format="0.2f")
         self.y_axis = bq.Axis(scale=y_scale, orientation="vertical", label=self.y_key)
         self.hist = bq.Hist(sample=[], bins=bin_count, scales={"sample": x_scale, "count": y_scale})
         self.widget = bq.Figure(marks=[self.hist], axes=[self.x_axis, self.y_axis], padding_y=0)
 
     def update(self, data: DataBuffer):
@@ -241,25 +261,26 @@
 
 
 class Bar(PlottableWidget):
     """A bar plot of values from a 2D signal, where each bar represents a different index of the signal."""
 
     def __init__(
         self,
+        system: System,
         y_access: str | tuple[str, list[int]],
         x_names: list[str] = None,
         y_range: tuple[float, float] = (None, None),
     ):
         """
         Args:
             y_access: The key or key indices of a signal, defines how to access the y-axis data
             y_range:  The range of the y-axis, defaults to the range of the data at any given time i.e. (min(y), max(y))
             x_names:  The names of the bars on the x-axis
         """
-        super().__init__()
+        super().__init__(system)
 
         if isinstance(y_access, str):
             y_access = (y_access, None)
 
         y_range = {"min": y_range[0], "max": y_range[1]}
 
         self.y_key, self.y_idx = y_access
@@ -274,22 +295,7 @@
 
     def update(self, data: DataBuffer):
         with self.bars.hold_sync():
             data = data[self.y_key] if self.y_idx is None else data[self.y_key][self.y_idx]
             if self.x_names is None:  # we cannot know how many bars there are beforehand
                 self.bars.x = list(range(data.shape[0]))
             self.bars.y = data[..., -1]
-
-
-# TODO: Implement WebFrontend
-# class WebFrontend(FrontendBase):
-#     def __init__(self, system: System, port):
-#         super().__init__(system)
-#         self.port = port
-
-#         self.app = Flask(__name__)
-
-#     def update(self, data: DataBuffer):
-#         self.socket.emit("data", data)
-
-#     def run(self):
-#         self.app.run(port=self.port)
```

### Comparing `genki_signals-0.1.1/genki_signals/functions/__init__.py` & `genki_signals-1.0.0/genki_signals/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.1/genki_signals/functions/arithmetic.py` & `genki_signals-1.0.0/genki_signals/functions/arithmetic.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     def __call__(self, x):
         return x * self.scale_factor
 
 
 class Sum(SignalFunction):
     """Sum multiple signals"""
+
     def __init__(self, *inputs: SignalName, name: str):
         super().__init__(*inputs, name=name)
 
     def __call__(self, *inputs):
         return sum(inputs)
 
 
@@ -95,26 +96,32 @@
         input_b: SignalName,
         name: str,
         use_trapz: bool = True,
     ):
         super().__init__(input_a, input_b, name=name, params={"use_trapz": use_trapz})
         self.trapezoid = use_trapz
         self.state = 0.0
+        self.last_a = None
         self.last_b = None
 
     def __call__(self, a, b):
         if self.trapezoid:
-            val = self.state + integrate.cumulative_trapezoid(y=a, x=b, initial=0.0, axis=-1)
+            prepend_a = a[..., 0:1] if self.last_a is None else self.last_a
+            prepend_b = b[..., 0:1] if self.last_b is None else self.last_b
+            a = np.concatenate([prepend_a, a], axis=-1)
+            b = np.concatenate([prepend_b, b], axis=-1)
+            val = self.state + integrate.cumulative_trapezoid(y=a, x=b, axis=-1)
         else:
             prepend_b = b[..., 0:1] if self.last_b is None else self.last_b
             db = np.diff(b, prepend=prepend_b)
-            val = self.state + a.cumsum(axis=-1) * db
+            val = self.state + (a * db).cumsum(axis=-1)
 
         if len(val) > 0:
-            self.state = val[..., -1]
+            self.state = val[..., -1:]
+            self.last_a = a[..., -1:]
             self.last_b = b[..., -1:]
 
         return val
 
 
 class Differentiate(SignalFunction):
     """
```

### Comparing `genki_signals-0.1.1/genki_signals/functions/base.py` & `genki_signals-1.0.0/genki_signals/functions/base.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.1/genki_signals/functions/filters.py` & `genki_signals-1.0.0/genki_signals/functions/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         return self.filter.process(x).squeeze()
 
 
 class HighPassFilter(SignalFunction):
     """
     High pass filter a signal. This is implemented as a butterworth filter.
     """
+
     def __init__(
         self,
         input_signal: SignalName,
         name: str,
         order: int,
         cutoff_freq: float,
         sample_rate: int,
@@ -55,14 +56,15 @@
         return val
 
 
 class BandPassFilter(SignalFunction):
     """
     Band pass filter a signal. This is implemented as a butterworth filter.
     """
+
     def __init__(
         self,
         input_signal: SignalName,
         name: str,
         order: int,
         cutoff_freq: float,
         sample_rate: int,
@@ -78,14 +80,15 @@
         return val
 
 
 class LowPassFilter(SignalFunction):
     """
     Low pass filter a signal. This is implemented as a butterworth filter.
     """
+
     def __init__(
         self,
         input_signal: SignalName,
         name: str,
         order: int,
         cutoff_freq: float,
         sample_rate: int,
```

### Comparing `genki_signals-0.1.1/genki_signals/functions/geometry.py` & `genki_signals-1.0.0/genki_signals/functions/geometry.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.1/genki_signals/functions/inference.py` & `genki_signals-1.0.0/genki_signals/functions/inference.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,36 +27,39 @@
     ):
         super().__init__(
             input_signal, name=name, params={"model": model_filename, "stateful": stateful, "init_state": init_state}
         )
         self.stateful = stateful
         self.state = init_state
         self.session = InferenceSession(model_filename)
+        self.input_names = [inp.name for inp in self.session.get_inputs()]
+        self.output_names = [out.name for out in self.session.get_outputs()]
 
     def __call__(self, x):
         # x shape (6, 16, t)
         x = x[np.newaxis, ..., -1]  # note doesn't work offline
         if self.stateful:
             output, self.state = self.session.run(
-                ["output", "output_state"],
+                self.output_names,
                 {
-                    "input": x.astype(np.float32),
-                    "input_state": self.state.astype(np.float32),
+                    self.input_names[0]: x.astype(np.float32),
+                    self.input_names[1]: self.state.astype(np.float32),
                 },
             )
         else:
-            output, output_extra = self.session.run(["output", "output_extra"], {"input": x.astype(np.float32)})
-        return output[0, ..., None]
+            output = self.session.run(self.output_names, {self.input_names[0]: x.astype(np.float32)})
+        return output[0][..., None]
 
 
 class WindowedInference(WindowedSignalFunction, SignalFunction):
     """
     Run real-time inference using an ONNX model. Operates on a single input signal, and on a
     window of samples at a time, window_kwargs specify the windowing parameters (window_length and window_overlap).
     """
+
     def __init__(self, input_signal: SignalName, name: str, model_filename, **window_kwargs):
         super().__init__(input_signal, name=name, params={"model_filename": model_filename, **window_kwargs})
         self.init_windowing(**window_kwargs)
         self.session = InferenceSession(model_filename)
 
     def windowed_fn(self, x):
         x = x.T[np.newaxis, ...]
```

### Comparing `genki_signals-0.1.1/genki_signals/functions/serialization.py` & `genki_signals-1.0.0/genki_signals/functions/serialization.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numpy as np
+
 from genki_signals.functions.base import SignalFunction
 import genki_signals.functions as f
 
 
 def encode_signal_fn(obj):
     """
     JSON encoder for SignalFunction objects, to be used with json.dump.
@@ -10,14 +12,16 @@
         return {
             "__signal_function__": True,
             "type": obj.__class__.__name__,
             "inputs": obj.input_signals,
             "name": obj.name,
             "params": obj.params,
         }
+    elif isinstance(obj, np.ndarray):
+        return obj.tolist()
     else:
         type_name = obj.__class__.__name__
         raise TypeError(f"Object of type '{type_name}' is not JSON serializable")
 
 
 def decode_signal_fn(obj):
     """
```

### Comparing `genki_signals-0.1.1/genki_signals/functions/shape.py` & `genki_signals-1.0.0/genki_signals/functions/shape.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,14 +101,8 @@
                 else:
                     fn_inputs.append(args[self.input_signals.index(fn_input)])
             fn_output = fn(*fn_inputs)
             internal_outputs[fn.name] = fn_output
         return internal_outputs[self.signal_fns[-1].name]
 
 
-__all__ = [
-    "ExtractDimension",
-    "Concatenate",
-    "Stack",
-    "Reshape",
-    "Combine"
-]
+__all__ = ["ExtractDimension", "Concatenate", "Stack", "Reshape", "Combine"]
```

### Comparing `genki_signals-0.1.1/genki_signals/functions/waveforms.py` & `genki_signals-1.0.0/genki_signals/functions/waveforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,44 +4,53 @@
 from genki_signals.functions.base import SignalFunction, SignalName
 
 
 class SineWave(SignalFunction):
     """
     Generate a sine wave from an input signal (usually time)
     """
+
     def __init__(self, input_signal: SignalName, name: str, amplitude: float, frequency: float, phase: float):
-        super().__init__(input_signal, name=name, params={"amplitude": amplitude, "frequency": frequency, "phase": phase})
+        super().__init__(
+            input_signal, name=name, params={"amplitude": amplitude, "frequency": frequency, "phase": phase}
+        )
         self.amplitude = amplitude
         self.frequency = frequency
         self.phase = phase
 
     def __call__(self, input_signal):
         return self.amplitude * np.sin(2 * np.pi * self.frequency * input_signal + self.phase)
 
 
 class SquareWave(SignalFunction):
     """
     Generate a square wave from an input signal (usually time)
     """
+
     def __init__(self, input_signal: SignalName, name: str, amplitude: float, frequency: float, phase: float):
-        super().__init__(input_signal, name=name, params={"amplitude": amplitude, "frequency": frequency, "phase": phase})
+        super().__init__(
+            input_signal, name=name, params={"amplitude": amplitude, "frequency": frequency, "phase": phase}
+        )
         self.amplitude = amplitude
         self.frequency = frequency
         self.phase = phase
 
     def __call__(self, input_signal):
         return self.amplitude * signal.square(2 * np.pi * self.frequency * input_signal + self.phase)
 
 
 class TriangleWave(SignalFunction):
     """
     Generate a triangular wave from an input signal (usually time)
     """
+
     def __init__(self, input_signal: SignalName, name: str, amplitude: float, frequency: float, phase: float):
-        super().__init__(input_signal, name=name, params={"amplitude": amplitude, "frequency": frequency, "phase": phase})
+        super().__init__(
+            input_signal, name=name, params={"amplitude": amplitude, "frequency": frequency, "phase": phase}
+        )
         self.amplitude = amplitude
         self.frequency = frequency
         self.phase = phase
 
     def __call__(self, input_signal):
         return self.amplitude * signal.sawtooth(2 * np.pi * self.frequency * input_signal + self.phase, 0.5)
```

### Comparing `genki_signals-0.1.1/genki_signals/functions/windowed.py` & `genki_signals-1.0.0/genki_signals/functions/windowed.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     return signal.repeat(factor, axis=-1)
 
 
 class SampleRate(SignalFunction):
     """
     Calculate the sample rate of an input signal (presumably timestamps)
     """
+
     def __init__(
         self,
         input_signal: SignalName = "timestamp",
         name: str = "sample_rate",
         unit_multiplier: float = 1,
     ):
         super().__init__(input_signal, name=name, params={"unit_multiplier": unit_multiplier})
@@ -33,14 +34,15 @@
         return rate * self.unit_multiplier
 
 
 class WindowedSignalFunction(ABC):
     """
     Base class for signal functions that operate on a sliding window of their input signal
     """
+
     def init_windowing(
         self,
         window_size: int,
         output_shape: tuple[int],
         window_overlap: int = 0,
         default_value: float = 0.0,
         upsample: bool = False,
@@ -143,12 +145,8 @@
             self.buffer.extend(init_vals)
 
         self.buffer.extend(sig)
         out = self.buffer.popleft(sig.shape[-1])
         return out
 
 
-__all__ = [
-    "SampleRate",
-    "FourierTransform",
-    "Delay",
-]
+__all__ = ["SampleRate", "FourierTransform", "Delay", "WindowedSignalFunction"]
```

### Comparing `genki_signals-0.1.1/genki_signals/fusion.py` & `genki_signals-1.0.0/genki_signals/fusion.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.1/genki_signals/recorders.py` & `genki_signals-1.0.0/genki_signals/recorders.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,30 +57,50 @@
     def write(self, data: DataBuffer):
         self.wavefile.writeframes(data["audio"].tobytes())
 
     def stop(self):
         self.wavefile.close()
 
 
-class CsvFileRecorder(Recorder):
+class DataFrameRecorder(Recorder):
     def __init__(self, path, rec_buffer_size=1_000_000):
         self.path = path
         self.rec_buffer_size = rec_buffer_size
         self._has_written_file = False
         self._recording_buffer = DataBuffer()
 
     def _flush_to_file(self):
         df = self._recording_buffer.to_dataframe()
         if self._has_written_file:
-            df.to_csv(self.path, mode="a", header=False, index=False)
+            self.serialize_frame(df, initial_frame=False)
         else:
-            df.to_csv(self.path, index=False)
+            self.serialize_frame(df, initial_frame=True)
             self._has_written_file = True
         self._recording_buffer.clear()
 
+    @abc.abstractmethod
+    def serialize_frame(self, frame, initial_frame=False):
+        pass
+
     def write(self, data: DataBuffer):
         self._recording_buffer.extend(data)
         if len(self._recording_buffer) > self.rec_buffer_size:
             self._flush_to_file()
 
     def stop(self):
         self._flush_to_file()
+
+
+class CsvFileRecorder(DataFrameRecorder):
+    def serialize_frame(self, df, initial_frame=False):
+        if initial_frame:
+            df.to_csv(self.path, index=False)
+        else:
+            df.to_csv(self.path, mode="a", header=False, index=False)
+
+
+class ParquetFileRecorder(DataFrameRecorder):
+    def serialize_frame(self, df, initial_frame=False):
+        if initial_frame:
+            df.to_parquet(self.path, index=False)
+        else:
+            df.to_parquet(self.path, mode="a", index=False)
```

### Comparing `genki_signals-0.1.1/genki_signals/session.py` & `genki_signals-1.0.0/genki_signals/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pickle
 import sys
 import wave
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
+import pandas as pd
 
 from genki_signals.buffers import DataBuffer
 from genki_signals.functions.serialization import encode_signal_fn, decode_signal_fn
 from genki_signals.functions.base import compute_signal_functions
 
 
 def read_json_file(p: Path | str):
@@ -98,14 +99,18 @@
         if self.datafile_extension in [".pickle", ".pkl"]:
             with open(self.raw_data_path, "rb") as FILE:
                 self._raw_data = pickle.load(FILE)
         elif self.datafile_extension == ".wav":
             wavefile = wave.open(self.raw_data_path.as_posix(), "rb")
             data = wavefile.readframes(wavefile.getnframes())
             self._raw_data = DataBuffer(data={"audio": np.frombuffer(data, np.int16)})
+        elif self.datafile_extension == ".parquet":
+            self._raw_data = DataBuffer.from_dataframe(pd.read_parquet(self.raw_data_path))
+        elif self.datafile_extension == ".csv":
+            self._raw_data = DataBuffer.from_dataframe(pd.read_csv(self.raw_data_path))
         else:
             raise NotImplementedError(f"Loading data from {self._datafile_extension} is not implemented")
 
     def _load_metadata(self):
         self._metadata = read_json_file(self.metadata_path)
 
     def _write_metadata(self):
@@ -169,8 +174,8 @@
         return compute_signal_functions(self.raw_data, self.functions)
 
     def get_parameters(self):
         return dict(
             (f"{fn.name}.{param_name}", param_value)
             for fn in self.functions
             for param_name, param_value in fn.params.items()
-        )
+        )
```

### Comparing `genki_signals-0.1.1/genki_signals/sources/__init__.py` & `genki_signals-1.0.0/genki_signals/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.1/genki_signals/sources/ble.py` & `genki_signals-1.0.0/genki_signals/sources/ble.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 from genki_signals.buffers import DataBuffer
 from genki_signals.sources.base import SamplerBase, SignalSource
 
 
 async def find_ble_address(device_name: str = None):
     """
-        A function to find ble addresses of devices
+    A function to find ble addresses of devices
 
-        Args:
-            device_name: The name of the device
+    Args:
+        device_name: The name of the device
 
-        Returns:
-            If device_name is given:
-                returns ble address of device with device name: device_name
-            Else:
-                returns all devices
+    Returns:
+        If device_name is given:
+            returns ble address of device with device name: device_name
+        Else:
+            returns all devices
     """
     devices = await BleakScanner.discover()
     if device_name is None:
         return [device.details for device in devices]
     for device in devices:
         if device.name == device_name:
             return str(device.address)
```

### Comparing `genki_signals-0.1.1/genki_signals/sources/dataframe.py` & `genki_signals-1.0.0/genki_signals/sources/dataframe.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.1/genki_signals/sources/local.py` & `genki_signals-1.0.0/genki_signals/sources/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 from genki_signals.sources.base import SignalSource, SamplerBase
 
 
 class MouseSource(SignalSource):
     """
     Signal source that samples the mouse position.
     """
+
     def __init__(self):
         import pynput
 
         self.mouse = pynput.mouse.Controller()
 
     def __call__(self):
         return np.array(self.mouse.position)
 
 
 class KeyboardSource(SignalSource):
     """
     Signal source that samples whether a specified set of keys are being pressed or not.
     """
+
     def __init__(self, keys):
         import pynput
 
         self.keys = keys
         self.listener = pynput.keyboard.Listener(on_press=self.on_press, on_release=self.on_release)
         self.is_pressing = None
 
@@ -111,46 +113,43 @@
         self.stream = None
         self.buffer = Queue()
         self.is_active = False
         self.followers = followers
         self.signal_names = [self.key]
 
     def start(self):
+        for source in self.followers.values():
+            source.start()
         self.stream = self.pa.open(
             format=self.format,
             channels=self.mic_info["maxInputChannels"],
             rate=self.sample_rate,
             input=True,
             frames_per_buffer=self.chunk_size,
             stream_callback=self.receive,
         )
-        for source in self.followers.values():
-            source.start()
         self.stream.start_stream()
         self.is_active = True
 
     def stop(self):
         self.stream.stop_stream()
         self.stream.close()
         for source in self.followers.values():
             source.stop()
         self.is_active = False
 
     def receive(self, in_data, frame_count, time_info, status):
         # TODO: Use the info from other params somehow (particularly time_info)
         from pyaudio import paContinue
 
-        data = {
-            "timestamp": np.array([time.time()]),
-            self.key: np.frombuffer(in_data, dtype=np.int16)
-        }
+        data = {"timestamp": np.array([time.time()]), self.key: np.frombuffer(in_data, dtype=np.int16)}
         for name, source in self.followers.items():
             d = source()
-            d.pop("timestamp", None)
             if isinstance(d, dict):
+                d.pop("timestamp", None)
                 for key, value in d.items():
                     data[f"{name}_{key}"] = np.array([value]).T
             else:
                 data[name] = np.array([d]).T
         self.buffer.put(data)
         return in_data, paContinue
```

### Comparing `genki_signals-0.1.1/genki_signals/sources/sampler.py` & `genki_signals-1.0.0/genki_signals/sources/sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self._stop_event.set()
 
 
 class Sampler(SamplerBase):
     """
     A data source that samples data from other sources at a given rate.
     """
+
     def __init__(self, sources, sample_rate, sleep_time=1e-6, timestamp_key="timestamp"):
         self.sources = sources
         self.is_active = False
         self.buffer = Queue()
         self.start_time = None
         self.timestamp_key = timestamp_key
         self._busy_loop = None
```

### Comparing `genki_signals-0.1.1/genki_signals/sources/wave.py` & `genki_signals-1.0.0/genki_signals/sources/wave.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.1/genki_signals/system.py` & `genki_signals-1.0.0/genki_signals/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,19 +33,25 @@
     def __repr__(self):
         return f"System({self.source}, {self.functions})"
 
     def _busy_loop(self):
         while self.is_active:
             new_data = self._read()
             if len(new_data) > 0:
-                for feed in self.data_feeds.values():
+                # We extract the current data feeds into a list
+                # to prevent errors if a feed is deregistered or new feed added
+                # while we are iterating over them.
+                current_feeds = list(self.data_feeds.values())
+                for feed in current_feeds:
                     feed(new_data)
             time.sleep(1 / self.update_rate)
 
     def register_data_feed(self, feed_id, callback):
+        if feed_id in self.data_feeds:
+            raise ValueError(f"Feed with id {feed_id} already exists")
         self.data_feeds[feed_id] = callback
 
     def deregister_data_feed(self, feed_id):
         self.data_feeds.pop(feed_id)
 
     def start(self):
         self.source.start()
@@ -72,16 +78,18 @@
     def start_recording(self, path, recorder=None, **metadata):
         path = Path(path)
         Session.create_session(path, self, metadata)
 
         if recorder is None:
             if isinstance(self.source, MicSource):
                 recorder = WavFileRecorder(
-                    (path / "raw_data.wav").as_posix(), self.source.sample_rate, self.source.n_channels,
-                    self.source.sample_width
+                    (path / "raw_data.wav").as_posix(),
+                    self.source.sample_rate,
+                    self.source.n_channels,
+                    self.source.sample_width,
                 )
             else:
                 recorder = PickleRecorder(path / "raw_data.pickle")
         self.recorder = recorder
         self.is_recording = True
 
     def stop_recording(self):
```

### Comparing `genki_signals-0.1.1/genki_signals.egg-info/PKG-INFO` & `genki_signals-1.0.0/genki_signals.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genki-signals
-Version: 0.1.1
+Version: 1.0.0
 Summary: A library for realtime signal processing and machine learning
 Home-page: https://github.com/genkiinstruments/genki-signals
 Author: Genki Instruments
 Author-email: genki@genkiinstruments.com
 Keywords: Signal Processing,Machine Learning,Realtime
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `genki_signals-0.1.1/setup.py` & `genki_signals-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 import re
 import setuptools
 
 
 # Hacky way to get the version string from the __init__ file, can't import it since it hasn't been "built" yet
-VERSIONFILE="genki_signals/__init__.py"
-getversion = re.search( r"^__version__ = ['\"]([^'\"]*)['\"]", open(VERSIONFILE, "rt").read(), re.M)
+VERSIONFILE = "genki_signals/__init__.py"
+getversion = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", open(VERSIONFILE, "rt").read(), re.M)
 if getversion:
     version = getversion.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 short_description = "A library for realtime signal processing and machine learning"
 long_description = open("README.md").read()
 
-print()
-print("Version: ", version)
-print("Short description: ", short_description)
-print("Long description: ", long_description[:100], "...")
-print()
-
 setuptools.setup(
     name="genki_signals",
     version=version,
     description=short_description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_files=["LICENSE"],
     url="https://github.com/genkiinstruments/genki-signals",
-    python_requires='>=3.9',
+    python_requires=">=3.9",
     install_requires=[
         "numpy",
         "pandas",
         "scipy",
         "onnx",
         "onnxruntime",
         "opencv-python",
@@ -42,14 +36,15 @@
         "ahrs",
         "imufusion",
         "bleak",
         "genki_wave",
     ],
     author="Genki Instruments",
     author_email="genki@genkiinstruments.com",
-    keywords = ["Signal Processing", "Machine Learning", "Realtime"],
-    classifiers = [
+    keywords=["Signal Processing", "Machine Learning", "Realtime"],
+    packages=setuptools.find_packages(exclude=("tests", "test", "examples")),
+    classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
-)
+)
```

