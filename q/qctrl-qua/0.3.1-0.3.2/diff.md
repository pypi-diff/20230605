# Comparing `tmp/qctrl_qua-0.3.1.tar.gz` & `tmp/qctrl_qua-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_qua-0.3.1.tar", max compression
+gzip compressed data, was "qctrl_qua-0.3.2.tar", max compression
```

## Comparing `qctrl_qua-0.3.1.tar` & `qctrl_qua-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    36653 2023-04-18 07:49:10.745215 qctrl_qua-0.3.1/LICENSE
--rw-r--r--   0        0        0      131 2023-04-18 07:49:10.745215 qctrl_qua-0.3.1/README.md
--rw-r--r--   0        0        0     2736 2023-04-18 07:49:29.630591 qctrl_qua-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      818 2023-04-18 07:49:29.634591 qctrl_qua-0.3.1/qctrlqua/__init__.py
--rw-r--r--   0        0        0     3978 2023-04-18 07:49:10.745215 qctrl_qua-0.3.1/qctrlqua/qua_config_gen.py
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 qctrl_qua-0.3.1/setup.py
--rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 qctrl_qua-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-06-05 06:32:16.751138 qctrl_qua-0.3.2/LICENSE
+-rw-r--r--   0        0        0      349 2023-06-05 06:32:16.751138 qctrl_qua-0.3.2/README.md
+-rw-r--r--   0        0        0     2729 2023-06-05 06:32:36.867369 qctrl_qua-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      818 2023-06-05 06:32:36.875369 qctrl_qua-0.3.2/qctrlqua/__init__.py
+-rw-r--r--   0        0        0     3978 2023-06-05 06:32:16.751138 qctrl_qua-0.3.2/qctrlqua/qua_config_gen.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 qctrl_qua-0.3.2/PKG-INFO
```

### Comparing `qctrl_qua-0.3.1/LICENSE` & `qctrl_qua-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_qua-0.3.1/pyproject.toml` & `qctrl_qua-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "qctrl-qua"
-version = "0.3.1"
-description = "Q-CTRL Python QUA Adapter"
+version = "0.3.2"
+description = "Q-CTRL QUA Adapter"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
 documentation = "https://docs.q-ctrl.com/boulder-opal/references/qctrl-qua/"
```

### Comparing `qctrl_qua-0.3.1/qctrlqua/__init__.py` & `qctrl_qua-0.3.2/qctrlqua/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 
 """
 The Q-CTRL QUA Adapter package allows you to integrate Boulder Opal with the QUA
 quantum computing language.
 """
 
 __author__ = "Q-CTRL <support@q-ctrl.com>"
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 from .qua_config_gen import add_pulse_to_config
 
 __all__ = ["add_pulse_to_config"]
```

### Comparing `qctrl_qua-0.3.1/qctrlqua/qua_config_gen.py` & `qctrl_qua-0.3.2/qctrlqua/qua_config_gen.py`

 * *Files identical despite different names*

### Comparing `qctrl_qua-0.3.1/PKG-INFO` & `qctrl_qua-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qctrl-qua
-Version: 0.3.1
-Summary: Q-CTRL Python QUA Adapter
+Version: 0.3.2
+Summary: Q-CTRL QUA Adapter
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
 Maintainer-email: support@q-ctrl.com
@@ -39,10 +39,14 @@
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
 Description-Content-Type: text/markdown
 
 # Q-CTRL QUA Adapter
 
-The Q-CTRL QUA Adapter package allows you to integrate Boulder Opal with the QUA
-quantum computing language.
+The Q-CTRL QUA Adapter package allows you to integrate Boulder Opal with the
+QUA quantum computing language.
+
+See how you can do that in the user guide [How to integrate Boulder Opal with
+QUA from Quantum
+Machines](https://docs.q-ctrl.com/boulder-opal/user-guides/how-to-integrate-boulder-opal-with-qua-from-quantum-machines).
```

