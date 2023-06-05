# Comparing `tmp/skyler_cli-0.4.2.tar.gz` & `tmp/skyler_cli-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyler_cli-0.4.2.tar", max compression
+gzip compressed data, was "skyler_cli-0.4.3.tar", max compression
```

## Comparing `skyler_cli-0.4.2.tar` & `skyler_cli-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      294 2023-03-26 23:05:28.146296 skyler_cli-0.4.2/README.md
--rw-r--r--   0        0        0      757 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/cli/__init__.py
--rw-r--r--   0        0        0      978 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/cli/main.py
--rw-r--r--   0        0        0        0 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/core/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/__init__.py
--rw-r--r--   0        0        0     6150 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system.py
--rw-r--r--   0        0        0      868 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system_template/.bashrc
--rw-r--r--   0        0        0        0 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system_template/__init__.py
--rw-r--r--   0        0        0     8340 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system_template/compton.conf
--rw-r--r--   0        0        0     9445 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system_template/i3_config
--rw-r--r--   0        0        0       42 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system_template/inputrc
--rw-r--r--   0        0        0       44 2023-03-26 23:05:28.150297 skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system_template/tmux.conf
--rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 skyler_cli-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      321 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/README.md
+-rw-r--r--   0        0        0      757 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/cli/__init__.py
+-rw-r--r--   0        0        0      978 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/__init__.py
+-rw-r--r--   0        0        0     6150 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system.py
+-rw-r--r--   0        0        0      868 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system_template/.bashrc
+-rw-r--r--   0        0        0        0 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system_template/__init__.py
+-rw-r--r--   0        0        0     8340 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system_template/compton.conf
+-rw-r--r--   0        0        0     9445 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system_template/i3_config
+-rw-r--r--   0        0        0       42 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system_template/inputrc
+-rw-r--r--   0        0        0       44 2023-06-05 02:24:22.470787 skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system_template/tmux.conf
+-rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 skyler_cli-0.4.3/PKG-INFO
```

### Comparing `skyler_cli-0.4.2/pyproject.toml` & `skyler_cli-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skyler-cli"
-version = "0.4.2"
+version = "0.4.3"
 description = "Skyler's toolbox of handy CLI utils"
 authors = ["bouldersky <skyarnold1@me.com>"]
 readme = "README.md"
 packages = [{include = "skyler_cli", from = "src"}]
 
 [tool.poetry.scripts]
 sc = "skyler_cli.cli.main:app"
```

### Comparing `skyler_cli-0.4.2/src/skyler_cli/cli/main.py` & `skyler_cli-0.4.3/src/skyler_cli/cli/main.py`

 * *Files identical despite different names*

### Comparing `skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system.py` & `skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system.py`

 * *Files identical despite different names*

### Comparing `skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system_template/.bashrc` & `skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system_template/.bashrc`

 * *Files identical despite different names*

### Comparing `skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system_template/compton.conf` & `skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system_template/compton.conf`

 * *Files identical despite different names*

### Comparing `skyler_cli-0.4.2/src/skyler_cli/core/bootstrap/system_template/i3_config` & `skyler_cli-0.4.3/src/skyler_cli/core/bootstrap/system_template/i3_config`

 * *Files identical despite different names*

### Comparing `skyler_cli-0.4.2/PKG-INFO` & `skyler_cli-0.4.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyler-cli
-Version: 0.4.2
+Version: 0.4.3
 Summary: Skyler's toolbox of handy CLI utils
 Author: bouldersky
 Author-email: skyarnold1@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,9 +14,9 @@
 Description-Content-Type: text/markdown
 
 # Skyler's CLI
 [![Test](https://github.com/bouldersky/skylers-cli/actions/workflows/test.yml/badge.svg)](https://github.com/bouldersky/skylers-cli/actions/workflows/test.yml)
 
 This is a modular CLI tool box that I tailor to my needs over time. It includes:
 
-- Nothing! Just this readme for now
+- A command to bootstrap all my . files onto a new workstation
```

