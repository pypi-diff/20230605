# Comparing `tmp/qctrl_mloop-3.0.1.tar.gz` & `tmp/qctrl_mloop-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_mloop-3.0.1.tar", max compression
+gzip compressed data, was "qctrl_mloop-3.0.2.tar", max compression
```

## Comparing `qctrl_mloop-3.0.1.tar` & `qctrl_mloop-3.0.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    36653 2023-04-18 07:50:02.996419 qctrl_mloop-3.0.1/LICENSE
--rw-r--r--   0        0        0      213 2023-04-18 07:50:02.996419 qctrl_mloop-3.0.1/README.md
--rw-r--r--   0        0        0     2560 2023-04-18 07:50:21.112614 qctrl_mloop-3.0.1/pyproject.toml
--rw-r--r--   0        0        0      836 2023-04-18 07:50:21.120614 qctrl_mloop-3.0.1/qctrlmloop/__init__.py
--rw-r--r--   0        0        0    15170 2023-04-18 07:50:03.000419 qctrl_mloop-3.0.1/qctrlmloop/controller.py
--rw-r--r--   0        0        0     5984 2023-04-18 07:50:03.000419 qctrl_mloop-3.0.1/qctrlmloop/testing.py
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 qctrl_mloop-3.0.1/setup.py
--rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 qctrl_mloop-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-06-05 06:21:45.569036 qctrl_mloop-3.0.2/LICENSE
+-rw-r--r--   0        0        0      470 2023-06-05 06:21:45.569036 qctrl_mloop-3.0.2/README.md
+-rw-r--r--   0        0        0     2553 2023-06-05 06:22:04.684611 qctrl_mloop-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0      836 2023-06-05 06:22:04.692611 qctrl_mloop-3.0.2/qctrlmloop/__init__.py
+-rw-r--r--   0        0        0    15170 2023-06-05 06:21:45.573036 qctrl_mloop-3.0.2/qctrlmloop/controller.py
+-rw-r--r--   0        0        0     5984 2023-06-05 06:21:45.573036 qctrl_mloop-3.0.2/qctrlmloop/testing.py
+-rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 qctrl_mloop-3.0.2/PKG-INFO
```

### Comparing `qctrl_mloop-3.0.1/LICENSE` & `qctrl_mloop-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_mloop-3.0.1/pyproject.toml` & `qctrl_mloop-3.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "qctrl-mloop"
-version = "3.0.1"
-description = "Q-CTRL Python M-LOOP Adapter"
+version = "3.0.2"
+description = "Q-CTRL M-LOOP Adapter"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 repository = ""
 documentation = "https://docs.q-ctrl.com/boulder-opal/references/qctrl-mloop/"
 keywords = [
@@ -57,15 +57,15 @@
 ]
 packages = [
     { include = "qctrlmloop" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
-qctrl = "^22.0.0"
+qctrl = "^22.0.1"
 M-LOOP = "~3.3.2"
 numpy = "~1.23.5"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.2.0"
```

### Comparing `qctrl_mloop-3.0.1/qctrlmloop/__init__.py` & `qctrl_mloop-3.0.2/qctrlmloop/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """qctrlmloop - integration between Boulder Opal automated closed-loop optimizers and M-LOOP"""
 
 __author__ = "Q-CTRL <support@q-ctrl.com>"
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 
 from .controller import (
     QctrlController,
     qctrl_controller,
 )
 
 __all__ = ["QctrlController", "qctrl_controller"]
```

### Comparing `qctrl_mloop-3.0.1/qctrlmloop/controller.py` & `qctrl_mloop-3.0.2/qctrlmloop/controller.py`

 * *Files identical despite different names*

### Comparing `qctrl_mloop-3.0.1/qctrlmloop/testing.py` & `qctrl_mloop-3.0.2/qctrlmloop/testing.py`

 * *Files identical despite different names*

### Comparing `qctrl_mloop-3.0.1/PKG-INFO` & `qctrl_mloop-3.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qctrl-mloop
-Version: 3.0.1
-Summary: Q-CTRL Python M-LOOP Adapter
+Version: 3.0.2
+Summary: Q-CTRL M-LOOP Adapter
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
 Maintainer-email: support@q-ctrl.com
 Requires-Python: >=3.8,<3.12
@@ -29,22 +29,26 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: M-LOOP (>=3.3.2,<3.4.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
-Requires-Dist: qctrl (>=22.0.0,<23.0.0)
+Requires-Dist: qctrl (>=22.0.1,<23.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com/boulder-opal/references/qctrl-mloop/
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/c/qctrl
 Description-Content-Type: text/markdown
 
 # Q-CTRL M-LOOP Adapter
 
 The Q-CTRL M-LOOP Adapter package allows you to integrate Boulder Opal
 automated closed-loop optimizers with automated closed-loop optimizations
 managed by the open-source package M-LOOP.
 
+See how you can use M-LOOP with Boulder Opal in the user guide [How to manage
+automated closed-loop hardware optimization with
+M-LOOP](https://docs.q-ctrl.com/boulder-opal/user-guides/how-to-manage-automated-closed-loop-hardware-optimization-with-m-loop).
+
```

