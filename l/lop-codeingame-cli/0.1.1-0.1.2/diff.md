# Comparing `tmp/lop_codeingame_cli-0.1.1.tar.gz` & `tmp/lop_codeingame_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lop_codeingame_cli-0.1.1.tar", max compression
+gzip compressed data, was "lop_codeingame_cli-0.1.2.tar", max compression
```

## Comparing `lop_codeingame_cli-0.1.1.tar` & `lop_codeingame_cli-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2023-06-05 02:33:09.815101 lop_codeingame_cli-0.1.1/lop_codeingame_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.1/lop_codeingame_cli/command/__init__.py
--rw-r--r--   0        0        0     1599 2023-06-05 02:33:20.318200 lop_codeingame_cli-0.1.1/lop_codeingame_cli/command/lopauth.py
--rw-r--r--   0        0        0     1453 2023-06-05 02:34:42.312309 lop_codeingame_cli-0.1.1/lop_codeingame_cli/command/lopdownload.py
--rw-r--r--   0        0        0     1078 2023-06-05 02:33:28.194419 lop_codeingame_cli-0.1.1/lop_codeingame_cli/command/lopgenerate.py
--rw-r--r--   0        0        0     1961 2023-06-05 02:33:20.309968 lop_codeingame_cli-0.1.1/lop_codeingame_cli/command/lopsubmit.py
--rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.1/lop_codeingame_cli/enumerations/__init__.py
--rw-r--r--   0        0        0      489 2023-06-04 19:06:25.997115 lop_codeingame_cli-0.1.1/lop_codeingame_cli/enumerations/main.py
--rw-r--r--   0        0        0      244 2023-06-05 02:33:20.323200 lop_codeingame_cli-0.1.1/lop_codeingame_cli/generator/__init__.py
--rw-r--r--   0        0        0     1941 2023-06-05 02:33:28.178434 lop_codeingame_cli-0.1.1/lop_codeingame_cli/generator/base.py
--rw-r--r--   0        0        0      908 2023-06-05 02:33:28.183414 lop_codeingame_cli-0.1.1/lop_codeingame_cli/generator/python.py
--rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.1/lop_codeingame_cli/model/__init__.py
--rw-r--r--   0        0        0      442 2023-06-05 02:34:07.450330 lop_codeingame_cli-0.1.1/lop_codeingame_cli/model/Exercise.py
--rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.1/lop_codeingame_cli/utilities/__init__.py
--rw-r--r--   0        0        0     1678 2023-06-05 02:33:28.187416 lop_codeingame_cli-0.1.1/lop_codeingame_cli/utilities/file.py
--rw-r--r--   0        0        0     1015 2023-06-05 02:33:28.199420 lop_codeingame_cli-0.1.1/lop_codeingame_cli/utilities/request.py
--rw-r--r--   0        0        0      413 2023-06-04 21:48:54.530260 lop_codeingame_cli-0.1.1/lop_codeingame_cli/utilities/variables.py
--rw-r--r--   0        0        0      586 2023-06-05 02:51:22.907078 lop_codeingame_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 02:33:39.080494 lop_codeingame_cli-0.1.1/README.md
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 lop_codeingame_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 02:33:09.815101 lop_codeingame_cli-0.1.2/lop_codeingame_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.2/lop_codeingame_cli/command/__init__.py
+-rw-r--r--   0        0        0     1599 2023-06-05 02:33:20.318200 lop_codeingame_cli-0.1.2/lop_codeingame_cli/command/lopauth.py
+-rw-r--r--   0        0        0     1453 2023-06-05 02:34:42.312309 lop_codeingame_cli-0.1.2/lop_codeingame_cli/command/lopdownload.py
+-rw-r--r--   0        0        0     1078 2023-06-05 02:33:28.194419 lop_codeingame_cli-0.1.2/lop_codeingame_cli/command/lopgenerate.py
+-rw-r--r--   0        0        0     1961 2023-06-05 02:33:20.309968 lop_codeingame_cli-0.1.2/lop_codeingame_cli/command/lopsubmit.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.2/lop_codeingame_cli/enumerations/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-04 19:06:25.997115 lop_codeingame_cli-0.1.2/lop_codeingame_cli/enumerations/main.py
+-rw-r--r--   0        0        0      244 2023-06-05 02:33:20.323200 lop_codeingame_cli-0.1.2/lop_codeingame_cli/generator/__init__.py
+-rw-r--r--   0        0        0     1941 2023-06-05 02:33:28.178434 lop_codeingame_cli-0.1.2/lop_codeingame_cli/generator/base.py
+-rw-r--r--   0        0        0      908 2023-06-05 02:33:28.183414 lop_codeingame_cli-0.1.2/lop_codeingame_cli/generator/python.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.2/lop_codeingame_cli/model/__init__.py
+-rw-r--r--   0        0        0      442 2023-06-05 02:34:07.450330 lop_codeingame_cli-0.1.2/lop_codeingame_cli/model/Exercise.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.2/lop_codeingame_cli/utilities/__init__.py
+-rw-r--r--   0        0        0     1678 2023-06-05 02:33:28.187416 lop_codeingame_cli-0.1.2/lop_codeingame_cli/utilities/file.py
+-rw-r--r--   0        0        0     1015 2023-06-05 02:33:28.199420 lop_codeingame_cli-0.1.2/lop_codeingame_cli/utilities/request.py
+-rw-r--r--   0        0        0      413 2023-06-04 21:48:54.530260 lop_codeingame_cli-0.1.2/lop_codeingame_cli/utilities/variables.py
+-rw-r--r--   0        0        0      587 2023-06-05 02:54:46.087498 lop_codeingame_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 02:33:39.080494 lop_codeingame_cli-0.1.2/README.md
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 lop_codeingame_cli-0.1.2/PKG-INFO
```

### Comparing `lop_codeingame_cli-0.1.1/lop_codeingame_cli/command/lopauth.py` & `lop_codeingame_cli-0.1.2/lop_codeingame_cli/command/lopauth.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.1/lop_codeingame_cli/command/lopdownload.py` & `lop_codeingame_cli-0.1.2/lop_codeingame_cli/command/lopdownload.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.1/lop_codeingame_cli/command/lopgenerate.py` & `lop_codeingame_cli-0.1.2/lop_codeingame_cli/command/lopgenerate.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.1/lop_codeingame_cli/command/lopsubmit.py` & `lop_codeingame_cli-0.1.2/lop_codeingame_cli/command/lopsubmit.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.1/lop_codeingame_cli/generator/base.py` & `lop_codeingame_cli-0.1.2/lop_codeingame_cli/generator/base.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.1/lop_codeingame_cli/generator/python.py` & `lop_codeingame_cli-0.1.2/lop_codeingame_cli/generator/python.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.1/lop_codeingame_cli/utilities/file.py` & `lop_codeingame_cli-0.1.2/lop_codeingame_cli/utilities/file.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.1/lop_codeingame_cli/utilities/request.py` & `lop_codeingame_cli-0.1.2/lop_codeingame_cli/utilities/request.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.1/pyproject.toml` & `lop_codeingame_cli-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lop-codeingame-cli"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["machkouroke <machkour20.mo1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "lop_codeingame_cli"}]
 
 [tool.poetry.dependencies]
@@ -15,13 +15,13 @@
 pydantic = "^1.10.8"
 pyyaml = "^6.0"
 websocket-client = "^1.5.2"
 clint = "^0.5.1"
 
 
 [tool.poetry.scripts]
-lopdowload = "lop_codeingame_cli.command:lopdownload"
+lopdownload = "lop_codeingame_cli.command:lopdownload"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lop_codeingame_cli-0.1.1/PKG-INFO` & `lop_codeingame_cli-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lop-codeingame-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: machkouroke
 Author-email: machkour20.mo1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

