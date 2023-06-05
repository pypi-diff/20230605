# Comparing `tmp/tfc-1.0.4.tar.gz` & `tmp/tfc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfc-1.0.4.tar", last modified: Sun May 28 15:29:28 2023, max compression
+gzip compressed data, was "tfc-1.0.5.tar", last modified: Mon Jun  5 18:47:06 2023, max compression
```

## Comparing `tfc-1.0.4.tar` & `tfc-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.593680 tfc-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-28 15:29:14.000000 tfc-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-28 15:29:14.000000 tfc-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-05-28 15:29:28.593680 tfc-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-28 15:29:14.000000 tfc-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-28 15:29:14.000000 tfc-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 15:29:28.593680 tfc-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-28 15:29:14.000000 tfc-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.589680 tfc-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.589680 tfc-1.0.4/src/tfc/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26145 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/mtfc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utfc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.589680 tfc-1.0.4/src/tfc/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.593680 tfc-1.0.4/src/tfc/utils/BF/
--rw-r--r--   0 runner    (1001) docker     (123)    44710 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/BF.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/BF.h
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/BF.i
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/BF.py
--rw-r--r--   0 runner    (1001) docker     (123)    46499 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/BF_Py.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109459 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/BF/numpy.i
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/CeSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/Html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/Latex.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/MakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/MayaviMakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    25995 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/PlotlyMakePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    58246 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/TFCUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-28 15:29:14.000000 tfc-1.0.4/src/tfc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:29:28.589680 tfc-1.0.4/src/tfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-05-28 15:29:28.000000 tfc-1.0.4/src/tfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-28 15:29:28.000000 tfc-1.0.4/src/tfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:29:28.000000 tfc-1.0.4/src/tfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-28 15:29:28.000000 tfc-1.0.4/src/tfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-28 15:29:28.000000 tfc-1.0.4/src/tfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.847995 tfc-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 18:46:59.000000 tfc-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 18:46:59.000000 tfc-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-06-05 18:47:06.847995 tfc-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-05 18:46:59.000000 tfc-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-05 18:47:00.000000 tfc-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 18:47:06.847995 tfc-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-05 18:47:00.000000 tfc-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.843995 tfc-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.843995 tfc-1.0.5/src/tfc/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26145 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/mtfc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utfc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.847995 tfc-1.0.5/src/tfc/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.847995 tfc-1.0.5/src/tfc/utils/BF/
+-rw-r--r--   0 runner    (1001) docker     (123)    44710 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/BF.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/BF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/BF.i
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/BF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46499 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/BF_Py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109459 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/BF/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/CeSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/Html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/Latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/MakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/MayaviMakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25995 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/PlotlyMakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58232 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/TFCUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-05 18:47:00.000000 tfc-1.0.5/src/tfc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:47:06.847995 tfc-1.0.5/src/tfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-06-05 18:47:06.000000 tfc-1.0.5/src/tfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-05 18:47:06.000000 tfc-1.0.5/src/tfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:47:06.000000 tfc-1.0.5/src/tfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-05 18:47:06.000000 tfc-1.0.5/src/tfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 18:47:06.000000 tfc-1.0.5/src/tfc.egg-info/top_level.txt
```

### Comparing `tfc-1.0.4/LICENSE` & `tfc-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/PKG-INFO` & `tfc-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfc
-Version: 1.0.4
+Version: 1.0.5
 Summary: Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.
 Home-page: https://github.com/leakec/tfc.git
 Author: Carl Leake and Hunter Johnston
 Author-email: leakec57@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -80,15 +80,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.4},
+    version = {1.0.5},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.4/README.md` & `tfc-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.4},
+    version = {1.0.5},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.4/pyproject.toml` & `tfc-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/setup.py` & `tfc-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/mtfc.py` & `tfc-1.0.5/src/tfc/mtfc.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utfc.py` & `tfc-1.0.5/src/tfc/utfc.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/BF/BF.cxx` & `tfc-1.0.5/src/tfc/utils/BF/BF.cxx`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/BF/BF.h` & `tfc-1.0.5/src/tfc/utils/BF/BF.h`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/BF/BF.i` & `tfc-1.0.5/src/tfc/utils/BF/BF.i`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/BF/BF.py` & `tfc-1.0.5/src/tfc/utils/BF/BF.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/BF/BF_Py.py` & `tfc-1.0.5/src/tfc/utils/BF/BF_Py.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/BF/numpy.i` & `tfc-1.0.5/src/tfc/utils/BF/numpy.i`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/CeSolver.py` & `tfc-1.0.5/src/tfc/utils/CeSolver.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/Html.py` & `tfc-1.0.5/src/tfc/utils/Html.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/Latex.py` & `tfc-1.0.5/src/tfc/utils/Latex.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/MakePlot.py` & `tfc-1.0.5/src/tfc/utils/MakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/MayaviMakePlot.py` & `tfc-1.0.5/src/tfc/utils/MayaviMakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/PlotlyMakePlot.py` & `tfc-1.0.5/src/tfc/utils/PlotlyMakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc/utils/TFCUtils.py` & `tfc-1.0.5/src/tfc/utils/TFCUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from jax._src.api_util import flatten_fun
 from jax._src.tree_util import tree_flatten
 from jax.core import get_aval, eval_jaxpr
 from jax.interpreters.partial_eval import trace_to_jaxpr_nounits, PartialVal
 from jax.experimental.host_callback import id_tap
 from typing import Any, Callable, Optional, Union, cast
 from .types import uint, List, Literal, Tuple, TypedDict, Path, Dict
-from jaxtyping.pytree_type import PyTree
+from jaxtyping import PyTree
 from typing import cast
 
 # Types that can be added to a TFCDict
 TFCDictAddable = Union[np.ndarray, Dict[Any, Any], "TFCDict"]
 
 # Types that can be added to a TFCDictRobust
 TFCDictRobustAddable = Union[np.ndarray, Dict[Any, Any], "TFCDictRobust"]
@@ -1718,16 +1718,16 @@
 
     # Run the command and print how to restart
     if user_mode:
         os.system(
             f"(criu dump --unpriviledged -t {pid} -D {str(path.absolute())} --shell-job --leave-running &) &"
         )
         print(
-            f'Creating a checkpoint. To restart run: "sudo criu restore -D {str(path.absolute())} --shell-job'
+            f"Creating a checkpoint. To restart run: sudo criu restore -D {str(path.absolute())} --shell-job"
         )
     else:
         os.system(
             f"(sudo criu dump -t {pid} -D {str(path.absolute())} --shell-job --leave-running &) &"
         )
         print(
-            f'Creating a checkpoint. To restart run: "sudo criu restore -D {str(path.absolute())} --shell-job'
+            f"Creating a checkpoint. To restart run: sudo criu restore -D {str(path.absolute())} --shell-job"
         )
```

### Comparing `tfc-1.0.4/src/tfc/utils/types.py` & `tfc-1.0.5/src/tfc/utils/types.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.4/src/tfc.egg-info/PKG-INFO` & `tfc-1.0.5/src/tfc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfc
-Version: 1.0.4
+Version: 1.0.5
 Summary: Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.
 Home-page: https://github.com/leakec/tfc.git
 Author: Carl Leake and Hunter Johnston
 Author-email: leakec57@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -80,15 +80,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.4},
+    version = {1.0.5},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.4/src/tfc.egg-info/SOURCES.txt` & `tfc-1.0.5/src/tfc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

