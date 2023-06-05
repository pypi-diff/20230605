# Comparing `tmp/lop_codeingame_cli-0.1.5.tar.gz` & `tmp/lop_codeingame_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lop_codeingame_cli-0.1.5.tar", max compression
+gzip compressed data, was "lop_codeingame_cli-0.1.6.tar", max compression
```

## Comparing `lop_codeingame_cli-0.1.5.tar` & `lop_codeingame_cli-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2023-06-05 02:33:09.815101 lop_codeingame_cli-0.1.5/lop_codeingame_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.5/lop_codeingame_cli/command/__init__.py
--rw-r--r--   0        0        0     1635 2023-06-05 03:26:10.044153 lop_codeingame_cli-0.1.5/lop_codeingame_cli/command/lopauth.py
--rw-r--r--   0        0        0     1474 2023-06-05 03:12:47.984996 lop_codeingame_cli-0.1.5/lop_codeingame_cli/command/lopdownload.py
--rw-r--r--   0        0        0     1099 2023-06-05 03:26:10.035426 lop_codeingame_cli-0.1.5/lop_codeingame_cli/command/lopgenerate.py
--rw-r--r--   0        0        0     1982 2023-06-05 03:26:10.031670 lop_codeingame_cli-0.1.5/lop_codeingame_cli/command/lopsubmit.py
--rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.5/lop_codeingame_cli/enumerations/__init__.py
--rw-r--r--   0        0        0      489 2023-06-04 19:06:25.997115 lop_codeingame_cli-0.1.5/lop_codeingame_cli/enumerations/main.py
--rw-r--r--   0        0        0      244 2023-06-05 02:33:20.323200 lop_codeingame_cli-0.1.5/lop_codeingame_cli/generator/__init__.py
--rw-r--r--   0        0        0     1941 2023-06-05 02:33:28.178434 lop_codeingame_cli-0.1.5/lop_codeingame_cli/generator/base.py
--rw-r--r--   0        0        0      908 2023-06-05 02:33:28.183414 lop_codeingame_cli-0.1.5/lop_codeingame_cli/generator/python.py
--rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.5/lop_codeingame_cli/model/__init__.py
--rw-r--r--   0        0        0      442 2023-06-05 02:34:07.450330 lop_codeingame_cli-0.1.5/lop_codeingame_cli/model/Exercise.py
--rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.5/lop_codeingame_cli/utilities/__init__.py
--rw-r--r--   0        0        0     1678 2023-06-05 02:33:28.187416 lop_codeingame_cli-0.1.5/lop_codeingame_cli/utilities/file.py
--rw-r--r--   0        0        0     1015 2023-06-05 02:33:28.199420 lop_codeingame_cli-0.1.5/lop_codeingame_cli/utilities/request.py
--rw-r--r--   0        0        0      414 2023-06-05 03:31:17.845004 lop_codeingame_cli-0.1.5/lop_codeingame_cli/utilities/variables.py
--rw-r--r--   0        0        0      763 2023-06-05 03:31:30.579799 lop_codeingame_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 02:33:39.080494 lop_codeingame_cli-0.1.5/README.md
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 lop_codeingame_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 02:33:09.815101 lop_codeingame_cli-0.1.6/lop_codeingame_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.6/lop_codeingame_cli/command/__init__.py
+-rw-r--r--   0        0        0     1635 2023-06-05 03:26:10.044153 lop_codeingame_cli-0.1.6/lop_codeingame_cli/command/lopauth.py
+-rw-r--r--   0        0        0     1474 2023-06-05 03:12:47.984996 lop_codeingame_cli-0.1.6/lop_codeingame_cli/command/lopdownload.py
+-rw-r--r--   0        0        0     1099 2023-06-05 03:26:10.035426 lop_codeingame_cli-0.1.6/lop_codeingame_cli/command/lopgenerate.py
+-rw-r--r--   0        0        0     1982 2023-06-05 03:26:10.031670 lop_codeingame_cli-0.1.6/lop_codeingame_cli/command/lopsubmit.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.6/lop_codeingame_cli/enumerations/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-04 19:06:25.997115 lop_codeingame_cli-0.1.6/lop_codeingame_cli/enumerations/main.py
+-rw-r--r--   0        0        0      244 2023-06-05 02:33:20.323200 lop_codeingame_cli-0.1.6/lop_codeingame_cli/generator/__init__.py
+-rw-r--r--   0        0        0     1941 2023-06-05 02:33:28.178434 lop_codeingame_cli-0.1.6/lop_codeingame_cli/generator/base.py
+-rw-r--r--   0        0        0      908 2023-06-05 02:33:28.183414 lop_codeingame_cli-0.1.6/lop_codeingame_cli/generator/python.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.6/lop_codeingame_cli/model/__init__.py
+-rw-r--r--   0        0        0      442 2023-06-05 02:34:07.450330 lop_codeingame_cli-0.1.6/lop_codeingame_cli/model/Exercise.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:23:43.257029 lop_codeingame_cli-0.1.6/lop_codeingame_cli/utilities/__init__.py
+-rw-r--r--   0        0        0     1678 2023-06-05 02:33:28.187416 lop_codeingame_cli-0.1.6/lop_codeingame_cli/utilities/file.py
+-rw-r--r--   0        0        0     1015 2023-06-05 02:33:28.199420 lop_codeingame_cli-0.1.6/lop_codeingame_cli/utilities/request.py
+-rw-r--r--   0        0        0      414 2023-06-05 03:31:17.845004 lop_codeingame_cli-0.1.6/lop_codeingame_cli/utilities/variables.py
+-rw-r--r--   0        0        0      763 2023-06-05 03:42:52.145846 lop_codeingame_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1731 2023-06-05 03:42:40.095786 lop_codeingame_cli-0.1.6/README.md
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 lop_codeingame_cli-0.1.6/PKG-INFO
```

### Comparing `lop_codeingame_cli-0.1.5/lop_codeingame_cli/command/lopauth.py` & `lop_codeingame_cli-0.1.6/lop_codeingame_cli/command/lopauth.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.5/lop_codeingame_cli/command/lopdownload.py` & `lop_codeingame_cli-0.1.6/lop_codeingame_cli/command/lopdownload.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.5/lop_codeingame_cli/command/lopgenerate.py` & `lop_codeingame_cli-0.1.6/lop_codeingame_cli/command/lopgenerate.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.5/lop_codeingame_cli/command/lopsubmit.py` & `lop_codeingame_cli-0.1.6/lop_codeingame_cli/command/lopsubmit.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.5/lop_codeingame_cli/generator/base.py` & `lop_codeingame_cli-0.1.6/lop_codeingame_cli/generator/base.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.5/lop_codeingame_cli/generator/python.py` & `lop_codeingame_cli-0.1.6/lop_codeingame_cli/generator/python.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.5/lop_codeingame_cli/utilities/file.py` & `lop_codeingame_cli-0.1.6/lop_codeingame_cli/utilities/file.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.5/lop_codeingame_cli/utilities/request.py` & `lop_codeingame_cli-0.1.6/lop_codeingame_cli/utilities/request.py`

 * *Files identical despite different names*

### Comparing `lop_codeingame_cli-0.1.5/pyproject.toml` & `lop_codeingame_cli-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lop-codeingame-cli"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["machkouroke <machkour20.mo1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "lop_codeingame_cli"}]
 
 [tool.poetry.dependencies]
```

