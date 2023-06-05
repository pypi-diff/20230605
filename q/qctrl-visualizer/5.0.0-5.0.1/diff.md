# Comparing `tmp/qctrl_visualizer-5.0.0.tar.gz` & `tmp/qctrl_visualizer-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_visualizer-5.0.0.tar", max compression
+gzip compressed data, was "qctrl_visualizer-5.0.1.tar", max compression
```

## Comparing `qctrl_visualizer-5.0.0.tar` & `qctrl_visualizer-5.0.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    36653 2023-03-30 01:36:38.078539 qctrl_visualizer-5.0.0/LICENSE
--rw-r--r--   0        0        0       82 2023-03-30 01:36:38.078539 qctrl_visualizer-5.0.0/README.md
--rw-r--r--   0        0        0     2823 2023-03-30 01:36:54.983681 qctrl_visualizer-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     2294 2023-03-30 01:36:54.995681 qctrl_visualizer-5.0.0/qctrlvisualizer/__init__.py
--rw-r--r--   0        0        0    23319 2023-03-30 01:36:38.082540 qctrl_visualizer-5.0.0/qctrlvisualizer/bloch.py
--rw-r--r--   0        0        0     9661 2023-03-30 01:36:38.082540 qctrl_visualizer-5.0.0/qctrlvisualizer/confidence_ellipses.py
--rw-r--r--   0        0        0    19934 2023-03-30 01:36:38.086540 qctrl_visualizer-5.0.0/qctrlvisualizer/controls.py
--rw-r--r--   0        0        0     4966 2023-03-30 01:36:38.086540 qctrl_visualizer-5.0.0/qctrlvisualizer/cost_histories.py
--rw-r--r--   0        0        0     7355 2023-03-30 01:36:38.086540 qctrl_visualizer-5.0.0/qctrlvisualizer/density_matrix.py
--rw-r--r--   0        0        0     8483 2023-03-30 01:36:38.086540 qctrl_visualizer-5.0.0/qctrlvisualizer/filter_functions.py
--rw-r--r--   0        0        0     6553 2023-03-30 01:36:38.086540 qctrl_visualizer-5.0.0/qctrlvisualizer/histogram.py
--rw-r--r--   0        0        0    12895 2023-03-30 01:36:38.086540 qctrl_visualizer-5.0.0/qctrlvisualizer/populations.py
--rw-r--r--   0        0        0     4147 2023-03-30 01:36:38.086540 qctrl_visualizer-5.0.0/qctrlvisualizer/style.py
--rw-r--r--   0        0        0     5525 2023-03-30 01:36:38.086540 qctrl_visualizer-5.0.0/qctrlvisualizer/utils.py
--rw-r--r--   0        0        0     5858 2023-03-30 01:36:38.086540 qctrl_visualizer-5.0.0/qctrlvisualizer/wigner_function.py
--rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 qctrl_visualizer-5.0.0/setup.py
--rw-r--r--   0        0        0     2198 1970-01-01 00:00:00.000000 qctrl_visualizer-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-06-05 06:19:46.075615 qctrl_visualizer-5.0.1/LICENSE
+-rw-r--r--   0        0        0      755 2023-06-05 06:19:46.075615 qctrl_visualizer-5.0.1/README.md
+-rw-r--r--   0        0        0     2841 2023-06-05 06:20:04.463800 qctrl_visualizer-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2367 2023-06-05 06:20:04.471799 qctrl_visualizer-5.0.1/qctrlvisualizer/__init__.py
+-rw-r--r--   0        0        0    23319 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/bloch.py
+-rw-r--r--   0        0        0    13992 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/confidence_ellipses.py
+-rw-r--r--   0        0        0    19934 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/controls.py
+-rw-r--r--   0        0        0     4966 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/cost_histories.py
+-rw-r--r--   0        0        0     7355 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/density_matrix.py
+-rw-r--r--   0        0        0     8486 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/filter_functions.py
+-rw-r--r--   0        0        0     6553 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/histogram.py
+-rw-r--r--   0        0        0    12895 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/populations.py
+-rw-r--r--   0        0        0     4147 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/style.py
+-rw-r--r--   0        0        0     5525 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/utils.py
+-rw-r--r--   0        0        0     5858 2023-06-05 06:19:46.079615 qctrl_visualizer-5.0.1/qctrlvisualizer/wigner_function.py
+-rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 qctrl_visualizer-5.0.1/PKG-INFO
```

### Comparing `qctrl_visualizer-5.0.0/LICENSE` & `qctrl_visualizer-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.0/pyproject.toml` & `qctrl_visualizer-5.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-visualizer"
-version = "5.0.0"
+version = "5.0.1"
 description = "Q-CTRL Visualizer"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -60,23 +60,24 @@
     { include = "qctrlvisualizer" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 matplotlib = ">=3.6.3"
 numpy = "^1.23.5"
+scipy = ">=1.9.3"
 qctrl-commons = "^18.0.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
-mypy = "^1.1.1"
-pytest = "^7.2.2"
+mypy = "^1.2.0"
+pytest = "^7.3.1"
 pylint = "^2.17.1"
-pre-commit = "^2.9.3"
+pre-commit = "^3.2.2"
 sphinx = "^5.3.0"
 tomli = "^2.0.1"
 qctrl-sphinx-theme = "~0.1.3"
 docopt = "~0.6.2"
 
 [[tool.poetry.source]]
 name = 'Q-CTRL PyPI'
```

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/__init__.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,18 @@
 )
 
 from .bloch import (
     display_bloch_sphere,
     display_bloch_sphere_from_bloch_vectors,
     display_bloch_sphere_from_density_matrices,
 )
-from .confidence_ellipses import plot_confidence_ellipses
+from .confidence_ellipses import (
+    confidence_ellipse_matrix,
+    plot_confidence_ellipses,
+)
 from .controls import (
     plot_controls,
     plot_sequences,
     plot_smooth_controls,
 )
 from .cost_histories import (
     plot_cost_histories,
@@ -52,14 +55,15 @@
     QCTRL_STYLE_COLORS,
     get_qctrl_style,
 )
 from .wigner_function import plot_wigner_function
 
 __all__ = [
     "QCTRL_STYLE_COLORS",
+    "confidence_ellipse_matrix",
     "display_bloch_sphere",
     "display_bloch_sphere_from_bloch_vectors",
     "display_bloch_sphere_from_density_matrices",
     "get_qctrl_style",
     "plot_confidence_ellipses",
     "plot_controls",
     "plot_cost_histories",
@@ -71,8 +75,8 @@
     "plot_population_distributions",
     "plot_bitstring_probabilities_histogram",
     "plot_sequences",
     "plot_smooth_controls",
     "plot_wigner_function",
 ]
 
-__version__ = "5.0.0"
+__version__ = "5.0.1"
```

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/bloch.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/bloch.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/controls.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/controls.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/cost_histories.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/cost_histories.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/density_matrix.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/density_matrix.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/filter_functions.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/filter_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     Examples
     --------
     Compare the filter functions of a primitive control scheme to BB1. The primitive scheme is
     sensitive to amplitude noise, whereas BB1 suppresses amplitude noise.
     The Hamiltonian of the system is
 
     .. math::
-        H(t) = \frac{1 + \beta(t)}{2} [\Omega(t) \sigma_- + \Omega^* \sigma_+] ,
+        H(t) = \frac{1 + \beta(t)}{2} [\Omega(t) \sigma_- + \Omega^*(t) \sigma_+] ,
 
     where :math:`\Omega(t)` is the time-dependent Rabi rate implementing each control scheme
     and :math:`\beta(t)` is a fractional time-dependent amplitude fluctuation process. ::
 
         import numpy as np
         from qctrl import Qctrl
         from qctrlvisualizer import plot_filter_functions
```

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/histogram.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/histogram.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/populations.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/populations.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/style.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/style.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/utils.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.0/qctrlvisualizer/wigner_function.py` & `qctrl_visualizer-5.0.1/qctrlvisualizer/wigner_function.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-5.0.0/PKG-INFO` & `qctrl_visualizer-5.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-visualizer
-Version: 5.0.0
+Version: 5.0.1
 Summary: Q-CTRL Visualizer
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -31,16 +31,27 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: matplotlib (>=3.6.3)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: qctrl-commons (>=18.0.0,<19.0.0)
+Requires-Dist: scipy (>=1.9.3)
 Project-URL: Documentation, https://docs.q-ctrl.com/boulder-opal/references/qctrl-visualizer/
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Description-Content-Type: text/markdown
 
 # Q-CTRL Visualizer
 
-Provides visualization of data for Q-CTRL's Python products.
+The Q-CTRL Visualizer offers broad functionality to visually engage with
+quantum dynamics and quantum controls.  These tools can help you develop
+understanding and intuition, and ultimately support the implementation of your
+quantum controls. See the topic [Visualizing your data using the Q-CTRL
+Visualizer](https://docs.q-ctrl.com/boulder-opal/topics/visualizing-your-data-using-the-q-ctrl-visualizer)
+in the Q-CTRL documentation for more information.
+
+The Q-CTRL Visualizer is meant to be used with the Q-CTRL products Boulder
+Opal, Fire Opal, and Open Controls. See how you can get started with [Boulder
+Opal](https://docs.q-ctrl.com/boulder-opal/get-started) and [Fire
+Opal](https://docs.q-ctrl.com/fire-opal/get-started) today.
```

