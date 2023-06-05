# Comparing `tmp/install_release-0.3.4.tar.gz` & `tmp/install_release-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install_release-0.3.4.tar", max compression
+gzip compressed data, was "install_release-0.3.5.tar", max compression
```

## Comparing `install_release-0.3.4.tar` & `install_release-0.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      295 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/Makefile
--rw-r--r--   0        0        0       22 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/__init__.py
--rw-r--r--   0        0        0     5070 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/cli.py
--rw-r--r--   0        0        0     9143 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/cli_interact.py
--rw-r--r--   0        0        0     1288 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/constants.py
--rw-r--r--   0        0        0     7473 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/core.py
--rw-r--r--   0        0        0     2221 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/data.py
--rw-r--r--   0        0        0     2285 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/state.py
--rw-r--r--   0        0        0     7351 2023-05-26 06:56:39.234911 install_release-0.3.4/InstallRelease/utils.py
--rw-r--r--   0        0        0    35149 2023-05-26 06:56:39.234911 install_release-0.3.4/LICENSE
--rw-r--r--   0        0        0     8430 2023-05-26 06:56:39.234911 install_release-0.3.4/README.md
--rw-r--r--   0        0        0      927 2023-05-26 06:56:39.234911 install_release-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     9295 1970-01-01 00:00:00.000000 install_release-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      295 2023-06-05 14:41:39.285812 install_release-0.3.5/InstallRelease/Makefile
+-rw-r--r--   0        0        0       22 2023-06-05 14:41:39.285812 install_release-0.3.5/InstallRelease/__init__.py
+-rw-r--r--   0        0        0     5070 2023-06-05 14:41:39.285812 install_release-0.3.5/InstallRelease/cli.py
+-rw-r--r--   0        0        0     9143 2023-06-05 14:41:39.285812 install_release-0.3.5/InstallRelease/cli_interact.py
+-rw-r--r--   0        0        0     1288 2023-06-05 14:41:39.285812 install_release-0.3.5/InstallRelease/constants.py
+-rw-r--r--   0        0        0     7473 2023-06-05 14:41:39.285812 install_release-0.3.5/InstallRelease/core.py
+-rw-r--r--   0        0        0     2221 2023-06-05 14:41:39.285812 install_release-0.3.5/InstallRelease/data.py
+-rw-r--r--   0        0        0     2285 2023-06-05 14:41:39.285812 install_release-0.3.5/InstallRelease/state.py
+-rw-r--r--   0        0        0     7351 2023-06-05 14:41:39.285812 install_release-0.3.5/InstallRelease/utils.py
+-rw-r--r--   0        0        0    35149 2023-06-05 14:41:39.285812 install_release-0.3.5/LICENSE
+-rw-r--r--   0        0        0     8430 2023-06-05 14:41:39.285812 install_release-0.3.5/README.md
+-rw-r--r--   0        0        0      928 2023-06-05 14:41:39.285812 install_release-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     9296 1970-01-01 00:00:00.000000 install_release-0.3.5/PKG-INFO
```

### Comparing `install_release-0.3.4/InstallRelease/cli.py` & `install_release-0.3.5/InstallRelease/cli.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.4/InstallRelease/cli_interact.py` & `install_release-0.3.5/InstallRelease/cli_interact.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.4/InstallRelease/constants.py` & `install_release-0.3.5/InstallRelease/constants.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.4/InstallRelease/core.py` & `install_release-0.3.5/InstallRelease/core.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.4/InstallRelease/data.py` & `install_release-0.3.5/InstallRelease/data.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.4/InstallRelease/state.py` & `install_release-0.3.5/InstallRelease/state.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.4/InstallRelease/utils.py` & `install_release-0.3.5/InstallRelease/utils.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.4/LICENSE` & `install_release-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `install_release-0.3.4/README.md` & `install_release-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `install_release-0.3.4/pyproject.toml` & `install_release-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [virtualenvs]
 in-project = true
 
 [tool.poetry]
 name = "install-release"
-version = "0.3.4"
+version = "0.3.5"
 readme = "README.md"
 description = "A cli tool to install tools based on your device info directly from github releases and keep them updated."
 authors = ["Rishang <rishangbhavsarcs@gmail.com>"]
 packages = [
   { include = "InstallRelease" }
 ]
 homepage = "https://github.com/Rishang/install-releases"
@@ -17,15 +17,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 rich = "*"
 requests = "*"
 python-magic = "^0.4.27"
-typer = ">=0.7.0,<0.8.0"
+typer = ">=0.9.0,<0.14.0"
 
 [tool.poetry.scripts]
 install-release = "InstallRelease.cli:app"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 mypy = "*"
```

### Comparing `install_release-0.3.4/PKG-INFO` & `install_release-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-release
-Version: 0.3.4
+Version: 0.3.5
 Summary: A cli tool to install tools based on your device info directly from github releases and keep them updated.
 Home-page: https://github.com/Rishang/install-releases
 Author: Rishang
 Author-email: rishangbhavsarcs@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: requests
 Requires-Dist: rich
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer (>=0.9.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # install-release 🚀
 [![Python Version](https://img.shields.io/badge/Python-3.8_to_3.10-xx.svg)](https://shields.io/) [![Downloads](https://static.pepy.tech/personalized-badge/install-release?&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/install-release)
 
 `install-release` is a cli tool to install any tool for your device directly from their github releases and keep them updated. you can consider it as a small package manager for github releases.
```

