# Comparing `tmp/qctrl_experiment_scheduler-0.2.0.tar.gz` & `tmp/qctrl_experiment_scheduler-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_experiment_scheduler-0.2.0.tar", max compression
+gzip compressed data, was "qctrl_experiment_scheduler-0.2.1.tar", max compression
```

## Comparing `qctrl_experiment_scheduler-0.2.0.tar` & `qctrl_experiment_scheduler-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    36653 2023-04-07 23:09:17.455388 qctrl_experiment_scheduler-0.2.0/LICENSE
--rw-r--r--   0        0        0      176 2023-04-07 23:09:17.455388 qctrl_experiment_scheduler-0.2.0/README.md
--rw-r--r--   0        0        0     2674 2023-04-07 23:09:38.867300 qctrl_experiment_scheduler-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     1181 2023-04-07 23:09:38.879299 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/__init__.py
--rwxr-xr-x   0        0        0    18587 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/graph.py
--rw-r--r--   0        0        0     8557 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/graph_traversal.py
--rw-r--r--   0        0        0    11004 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/node.py
--rwxr-xr-x   0        0        0      990 2023-04-07 23:09:38.875300 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/__init__.py
--rw-r--r--   0        0        0    20987 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/amplitude_calibration.py
--rw-r--r--   0        0        0    16619 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/simulation_backend.py
--rw-r--r--   0        0        0     7209 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/variable.py
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 qctrl_experiment_scheduler-0.2.0/setup.py
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 qctrl_experiment_scheduler-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-06-05 06:32:28.198427 qctrl_experiment_scheduler-0.2.1/LICENSE
+-rw-r--r--   0        0        0      695 2023-06-05 06:32:28.198427 qctrl_experiment_scheduler-0.2.1/README.md
+-rw-r--r--   0        0        0     2691 2023-06-05 06:32:48.050586 qctrl_experiment_scheduler-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1181 2023-06-05 06:32:48.054586 qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/__init__.py
+-rwxr-xr-x   0        0        0    18581 2023-06-05 06:32:28.198427 qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/graph.py
+-rw-r--r--   0        0        0     8557 2023-06-05 06:32:28.198427 qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/graph_traversal.py
+-rw-r--r--   0        0        0    11004 2023-06-05 06:32:28.198427 qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/node.py
+-rwxr-xr-x   0        0        0      990 2023-06-05 06:32:48.058586 qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/predefined/__init__.py
+-rw-r--r--   0        0        0    21033 2023-06-05 06:32:28.198427 qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/predefined/amplitude_calibration.py
+-rw-r--r--   0        0        0    16628 2023-06-05 06:32:28.198427 qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/predefined/simulation_backend.py
+-rw-r--r--   0        0        0     7209 2023-06-05 06:32:28.198427 qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/variable.py
+-rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 qctrl_experiment_scheduler-0.2.1/PKG-INFO
```

### Comparing `qctrl_experiment_scheduler-0.2.0/LICENSE` & `qctrl_experiment_scheduler-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.2.0/pyproject.toml` & `qctrl_experiment_scheduler-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-experiment-scheduler"
-version = "0.2.0"
+version = "0.2.1"
 description = "Q-CTRL Experiment Scheduler"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -67,29 +67,30 @@
 YouTube = "https://www.youtube.com/qctrl"
 GitHub = "https://github.com/qctrl"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 numpy = "^1.23.5"
 networkx = "^2.7"
-qctrl = "^22.0.0"
+qctrl = "^22.0.1"
 qctrl-commons = "^18.0.0"
 qctrl-visualizer = "^5.0.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 mypy = "^1.1.1"
 pre-commit = "^2.9.3"
 pylint = "^2.17.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 qctrl-sphinx-theme = "~0.1.2"
 sphinx = "^5.0.0"
 sphinx-reredirects = "^0.0.1"
+tomli = "^2.0.1"
 
 [tool.black]
 exclude = '''
 (
   /(
     | \.github
     | docs
```

### Comparing `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/__init__.py` & `qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """
 Q-CTRL Experiment Scheduler
 """
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = "Q-CTRL <support@q-ctrl.com>"
 
 from qctrlexperimentscheduler.graph import (
     CalibrationGraph,
     CalibrationProtocol,
 )
 from qctrlexperimentscheduler.graph_traversal import Verbosity
```

### Comparing `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/graph.py` & `qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
             np.max(text_box_sizes) * 72 * scaling * pixels * plt.rcParams["figure.dpi"]
         )
 
         plotting_graph = nx.DiGraph()
         plotting_graph.add_nodes_from(nodes)
         plotting_graph.add_edges_from(edges)
 
-        layout = nx.kamada_kawai_layout(plotting_graph)
+        layout = nx.spiral_layout(plotting_graph)
 
         draw_nodes = nx.draw_networkx_nodes(
             G=plotting_graph,
             pos=layout,
             node_size=node_size,
             node_color=QCTRL_STYLE_COLORS[0],
             ax=axis,
```

### Comparing `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/graph_traversal.py` & `qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/graph_traversal.py`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/node.py` & `qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/node.py`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/__init__.py` & `qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/predefined/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/amplitude_calibration.py` & `qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/predefined/amplitude_calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,61 +49,61 @@
 
     The methods of this class contain all the operations that an
     amplitude calibration requires. Specifically, it needs the capability
     of performing three kinds of experiments:
 
     1. A repetition of N :math:`\pi`-pulses followed by a measurement.
     2. A repetition of N :math:`\pi/2`-pulses followed by a measurement.
-    3. One pi/2-pulse followed by N :math:`\pi`-pulses and a measurement.
+    3. One :math:`\pi/2`-pulse followed by N :math:`\pi`-pulses and a measurement.
 
     Each of these functions should take the parameters of the Gaussian
     pulses used (amplitude and DRAG coefficient) as well as the number of
     repetitions N of each experiment. The result is then returned in the
     form of the fraction of the results in the state :math:`|1\rangle`.
     """
 
     def pi_pulse_experiment(
         self,
         amplitude: np.ndarray,
         drag: np.ndarray,
         repetition_count: int,
         shot_count: Optional[int] = None,
     ):
-        """
-        Run a series of pi pulses in the backend.
+        r"""
+        Run a series of :math:`\pi` pulses in the backend.
 
         This is an abstract method and should not be called directly.
         """
         raise NotImplementedError
 
     def pi_2_pulse_experiment(
         self,
         amplitude: np.ndarray,
         drag: np.ndarray,
         repetition_count: int,
         shot_count: Optional[int] = None,
     ):
-        """
-        Run a series of pi/2 pulses in the backend.
+        r"""
+        Run a series of :math:`\pi/2` pulses in the backend.
 
         This is an abstract method and should not be called directly.
         """
         raise NotImplementedError
 
     def pi_2_and_pi_pulse_experiment(
         self,
         pi_2_pulse_amplitude: np.ndarray,
         pi_2_pulse_drag: np.ndarray,
         pi_pulse_amplitude: np.ndarray,
         pi_pulse_drag: np.ndarray,
         repetition_count: int,
         shot_count: Optional[int] = None,
     ):
-        """
-        Run a pi / 2 pulse followed by a series of pi pulses in the backend.
+        r"""
+        Run a :math:`\pi/2` pulse followed by a series of :math:`\pi` pulses in the backend.
 
         This is an abstract method and should not be called directly.
         """
         raise NotImplementedError
 
 
 def _fit_parameters(
```

### Comparing `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/simulation_backend.py` & `qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/predefined/simulation_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         self,
         amplitude: np.ndarray,
         drag: np.ndarray,
         repetition_count: int,
         shot_count: Optional[int] = None,
     ) -> np.ndarray:
         r"""
-        Run a simulation of a series of Gaussian pi pulses applied to a qubit
+        Run a simulation of a series of Gaussian :math:`\pi` pulses applied to a qubit
         initially in state :math:`|0\rangle`.
 
         Parameters
         ----------
         amplitude : np.ndarray
             Value of amplitudes of the pi pulse. Must be a 1D array.
         drag : np.ndarray
```

### Comparing `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/variable.py` & `qctrl_experiment_scheduler-0.2.1/qctrlexperimentscheduler/variable.py`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.2.0/PKG-INFO` & `qctrl_experiment_scheduler-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-experiment-scheduler
-Version: 0.2.0
+Version: 0.2.1
 Summary: Q-CTRL Experiment Scheduler
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -30,22 +30,30 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: networkx (>=2.7,<3.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: qctrl (>=22.0.0,<23.0.0)
+Requires-Dist: qctrl (>=22.0.1,<23.0.0)
 Requires-Dist: qctrl-commons (>=18.0.0,<19.0.0)
 Requires-Dist: qctrl-visualizer (>=5.0.0,<6.0.0)
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
 Description-Content-Type: text/markdown
 
 # Q-CTRL Experiment Scheduler
 
-The Q-CTRL Experiment Scheduler provides convenience functionality to use
-Q-CTRL software in a series of interdependent calibration experiments.
+The Q-CTRL Experiment Scheduler package for Boulder Opal allows you to automate
+the workflow of complex calibration procedures. The scheduler will take into
+account the dependency between different parts of the calibration, the status
+of each of these parts, and the parameters that you are most interested in the
+calibration. With this information, it will determine the sequence that the
+calibrations have to be executed and run them for you.
+
+The Q-CTRL Experiment Scheduler was developed to be used with the quantum
+control software toolset Boulder Opal. See how you can [get started with
+Boulder Opal](https://docs.q-ctrl.com/boulder-opal/get-started) today.
```

