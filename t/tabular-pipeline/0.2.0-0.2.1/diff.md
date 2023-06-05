# Comparing `tmp/tabular_pipeline-0.2.0.tar.gz` & `tmp/tabular_pipeline-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabular_pipeline-0.2.0.tar", max compression
+gzip compressed data, was "tabular_pipeline-0.2.1.tar", max compression
```

## Comparing `tabular_pipeline-0.2.0.tar` & `tabular_pipeline-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1323 2023-06-02 17:51:00.351669 tabular_pipeline-0.2.0/README.md
--rw-r--r--   0        0        0      568 2023-06-05 09:50:03.629483 tabular_pipeline-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       33 2023-06-05 09:43:55.077866 tabular_pipeline-0.2.0/tabular_pipeline/__init__.py
--rw-r--r--   0        0        0      502 2023-06-05 09:44:06.230859 tabular_pipeline-0.2.0/tabular_pipeline/pipeline.py
--rw-r--r--   0        0        0     1276 2023-06-05 09:44:26.523992 tabular_pipeline-0.2.0/tabular_pipeline/read.py
--rw-r--r--   0        0        0      411 2023-06-02 17:34:25.107821 tabular_pipeline-0.2.0/tabular_pipeline/schemas.py
--rw-r--r--   0        0        0      929 2023-06-05 09:45:21.279463 tabular_pipeline-0.2.0/tabular_pipeline/settings.py
--rw-r--r--   0        0        0     1447 2023-06-05 09:45:06.154756 tabular_pipeline-0.2.0/tabular_pipeline/steps/__init__.py
--rw-r--r--   0        0        0     1998 2023-06-05 09:44:56.165268 tabular_pipeline-0.2.0/tabular_pipeline/steps/conform.py
--rw-r--r--   0        0        0     1001 2023-06-05 09:44:52.345815 tabular_pipeline-0.2.0/tabular_pipeline/steps/load.py
--rw-r--r--   0        0        0      815 2023-06-02 17:14:24.374765 tabular_pipeline-0.2.0/tabular_pipeline/util.py
--rw-r--r--   0        0        0      671 2023-06-05 09:45:28.161925 tabular_pipeline-0.2.0/tabular_pipeline/write.py
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 tabular_pipeline-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1323 2023-06-02 17:51:00.351669 tabular_pipeline-0.2.1/README.md
+-rw-r--r--   0        0        0      568 2023-06-05 11:26:47.783234 tabular_pipeline-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-06-05 09:43:55.077866 tabular_pipeline-0.2.1/tabular_pipeline/__init__.py
+-rw-r--r--   0        0        0      461 2023-06-05 10:10:07.880028 tabular_pipeline-0.2.1/tabular_pipeline/pipeline.py
+-rw-r--r--   0        0        0     1276 2023-06-05 10:12:57.191952 tabular_pipeline-0.2.1/tabular_pipeline/read.py
+-rw-r--r--   0        0        0      411 2023-06-02 17:34:25.107821 tabular_pipeline-0.2.1/tabular_pipeline/schemas.py
+-rw-r--r--   0        0        0      929 2023-06-05 09:45:21.279463 tabular_pipeline-0.2.1/tabular_pipeline/settings.py
+-rw-r--r--   0        0        0     1447 2023-06-05 09:45:06.154756 tabular_pipeline-0.2.1/tabular_pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     1998 2023-06-05 09:44:56.165268 tabular_pipeline-0.2.1/tabular_pipeline/steps/conform.py
+-rw-r--r--   0        0        0     1000 2023-06-05 10:13:50.677155 tabular_pipeline-0.2.1/tabular_pipeline/steps/load.py
+-rw-r--r--   0        0        0      815 2023-06-02 17:14:24.374765 tabular_pipeline-0.2.1/tabular_pipeline/util.py
+-rw-r--r--   0        0        0      671 2023-06-05 09:45:28.161925 tabular_pipeline-0.2.1/tabular_pipeline/write.py
+-rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 tabular_pipeline-0.2.1/PKG-INFO
```

### Comparing `tabular_pipeline-0.2.0/README.md` & `tabular_pipeline-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.0/pyproject.toml` & `tabular_pipeline-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "tabular-pipeline"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["franciscobmacedo <franciscovcbm@gmail.com>"]
 readme = "README.md"
 packages = [{include = "tabular_pipeline"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 tablib = {extras = ["xlsx"], version = "^3.4.0"}
 pyyaml = "^6.0"
 pydantic = "^1.10.8"
 typer = {extras = ["all"], version = "^0.9.0"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
```

### Comparing `tabular_pipeline-0.2.0/tabular_pipeline/read.py` & `tabular_pipeline-0.2.1/tabular_pipeline/read.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.0/tabular_pipeline/settings.py` & `tabular_pipeline-0.2.1/tabular_pipeline/settings.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.0/tabular_pipeline/steps/__init__.py` & `tabular_pipeline-0.2.1/tabular_pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.0/tabular_pipeline/steps/conform.py` & `tabular_pipeline-0.2.1/tabular_pipeline/steps/conform.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.0/tabular_pipeline/steps/load.py` & `tabular_pipeline-0.2.1/tabular_pipeline/steps/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 class Load(Step):
     """
     - load initial file
     - read multiple files (TODO)
     - read multiple sheets within each file (TODO)
     """
-
     step = StepChoices.LOAD
 
     def __init__(self, file_path: str, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.file_path = file_path
 
     def process(self) -> Dataset:
```

### Comparing `tabular_pipeline-0.2.0/tabular_pipeline/util.py` & `tabular_pipeline-0.2.1/tabular_pipeline/util.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.0/tabular_pipeline/write.py` & `tabular_pipeline-0.2.1/tabular_pipeline/write.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.0/PKG-INFO` & `tabular_pipeline-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tabular-pipeline
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: franciscobmacedo
 Author-email: franciscovcbm@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tablib[xlsx] (>=3.4.0,<4.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

