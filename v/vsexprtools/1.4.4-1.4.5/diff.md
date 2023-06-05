# Comparing `tmp/vsexprtools-1.4.4.tar.gz` & `tmp/vsexprtools-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsexprtools-1.4.4.tar", last modified: Thu May  4 22:00:22 2023, max compression
+gzip compressed data, was "vsexprtools-1.4.5.tar", last modified: Mon Jun  5 13:58:53 2023, max compression
```

## Comparing `vsexprtools-1.4.4.tar` & `vsexprtools-1.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:22.552593 vsexprtools-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 22:00:22.552593 vsexprtools-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 22:00:22.552593 vsexprtools-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:22.552593 vsexprtools-1.4.4/vsexprtools/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/exprop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/polyfills.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:22.552593 vsexprtools-1.4.4/vsexprtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 22:00:22.000000 vsexprtools-1.4.4/vsexprtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-04 22:00:22.000000 vsexprtools-1.4.4/vsexprtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:00:22.000000 vsexprtools-1.4.4/vsexprtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 22:00:22.000000 vsexprtools-1.4.4/vsexprtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 22:00:22.000000 vsexprtools-1.4.4/vsexprtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:53.353233 vsexprtools-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-05 13:58:53.353233 vsexprtools-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 13:58:53.353233 vsexprtools-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:53.353233 vsexprtools-1.4.5/vsexprtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/exprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/polyfills.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-06-05 13:58:30.000000 vsexprtools-1.4.5/vsexprtools/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:58:53.353233 vsexprtools-1.4.5/vsexprtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-05 13:58:53.000000 vsexprtools-1.4.5/vsexprtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-05 13:58:53.000000 vsexprtools-1.4.5/vsexprtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:58:53.000000 vsexprtools-1.4.5/vsexprtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 13:58:53.000000 vsexprtools-1.4.5/vsexprtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 13:58:53.000000 vsexprtools-1.4.5/vsexprtools.egg-info/top_level.txt
```

### Comparing `vsexprtools-1.4.4/LICENSE` & `vsexprtools-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.4/PKG-INFO` & `vsexprtools-1.4.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsexprtools
-Version: 1.4.4
+Version: 1.4.5
 Summary: VapourSynth functions and helpers for writing RPN expressions.
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-exprtools
 Project-URL: Documentation, https://vsexprtools.encode.moe/en/latest/
```

### Comparing `vsexprtools-1.4.4/setup.cfg` & `vsexprtools-1.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.4/setup.py` & `vsexprtools-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.4/vsexprtools/exprop.py` & `vsexprtools-1.4.5/vsexprtools/exprop.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from itertools import cycle
 from math import isqrt
 from typing import Any, Iterable, Iterator, Literal, SupportsFloat, SupportsIndex, overload
 
 from vstools import (
     ColorRange, ConvMode, CustomEnum, CustomIndexError, FuncExceptT, HoldsVideoFormatT, PlanesT, StrArrOpt, StrList,
-    VideoFormatT, VideoNodeIterable, flatten, get_lowest_value, get_neutral_value, get_peak_value, vs
+    VideoFormatT, VideoNodeIterable, flatten, get_lowest_value, get_neutral_value, get_peak_value, vs, get_sample_type
 )
 
 from .util import ExprVarRangeT, ExprVars, ExprVarsT, complexpr_available
 
 __all__ = [
     'ExprOp', 'ExprToken', 'ExprList'
 ]
@@ -21,14 +21,15 @@
 
 
 class ExprToken(ExprTokenBase, CustomEnum):
     LumaMin = 'ymin'
     ChromaMin = 'cmin'
     Lumamax = 'ymax'
     Chromamax = 'cmax'
+    RangeDiff = 'range_diff'
     RangeHalf = 'range_half'
     RangeSize = 'range_size'
     RangeMin = 'range_min'
     LumaRangeMin = 'yrange_min'
     ChromaRangeMin = 'crange_min'
     RangeMax = 'range_max'
     LumaRangeMax = 'yrange_max'
@@ -53,14 +54,19 @@
 
         if self is ExprToken.Lumamax:
             return get_peak_value(clip, False, ColorRange.LIMITED)
 
         if self is ExprToken.Chromamax:
             return get_peak_value(clip, True, ColorRange.LIMITED)
 
+        if self is ExprToken.RangeDiff:
+            if get_sample_type(clip) is vs.FLOAT:
+                return 0.0
+            return get_neutral_value(clip, chroma)
+
         if self is ExprToken.RangeHalf:
             return get_neutral_value(clip, chroma)
 
         if self is ExprToken.RangeSize:
             return (val := get_peak_value(clip)) + (1 - (val <= 1.0))
 
         if self is ExprToken.RangeMin:
```

### Comparing `vsexprtools-1.4.4/vsexprtools/funcs.py` & `vsexprtools-1.4.5/vsexprtools/funcs.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.4/vsexprtools/manager.py` & `vsexprtools-1.4.5/vsexprtools/manager.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.4/vsexprtools/operators.py` & `vsexprtools-1.4.5/vsexprtools/operators.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.4/vsexprtools/polyfills.py` & `vsexprtools-1.4.5/vsexprtools/polyfills.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.4/vsexprtools/util.py` & `vsexprtools-1.4.5/vsexprtools/util.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.4/vsexprtools/variables.py` & `vsexprtools-1.4.5/vsexprtools/variables.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.4/vsexprtools.egg-info/PKG-INFO` & `vsexprtools-1.4.5/vsexprtools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsexprtools
-Version: 1.4.4
+Version: 1.4.5
 Summary: VapourSynth functions and helpers for writing RPN expressions.
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-exprtools
 Project-URL: Documentation, https://vsexprtools.encode.moe/en/latest/
```

