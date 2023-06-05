# Comparing `tmp/tabular_pipeline-0.2.1.tar.gz` & `tmp/tabular_pipeline-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabular_pipeline-0.2.1.tar", max compression
+gzip compressed data, was "tabular_pipeline-0.2.2.tar", max compression
```

## Comparing `tabular_pipeline-0.2.1.tar` & `tabular_pipeline-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1323 2023-06-02 17:51:00.351669 tabular_pipeline-0.2.1/README.md
--rw-r--r--   0        0        0      568 2023-06-05 11:26:47.783234 tabular_pipeline-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       33 2023-06-05 09:43:55.077866 tabular_pipeline-0.2.1/tabular_pipeline/__init__.py
--rw-r--r--   0        0        0      461 2023-06-05 10:10:07.880028 tabular_pipeline-0.2.1/tabular_pipeline/pipeline.py
--rw-r--r--   0        0        0     1276 2023-06-05 10:12:57.191952 tabular_pipeline-0.2.1/tabular_pipeline/read.py
--rw-r--r--   0        0        0      411 2023-06-02 17:34:25.107821 tabular_pipeline-0.2.1/tabular_pipeline/schemas.py
--rw-r--r--   0        0        0      929 2023-06-05 09:45:21.279463 tabular_pipeline-0.2.1/tabular_pipeline/settings.py
--rw-r--r--   0        0        0     1447 2023-06-05 09:45:06.154756 tabular_pipeline-0.2.1/tabular_pipeline/steps/__init__.py
--rw-r--r--   0        0        0     1998 2023-06-05 09:44:56.165268 tabular_pipeline-0.2.1/tabular_pipeline/steps/conform.py
--rw-r--r--   0        0        0     1000 2023-06-05 10:13:50.677155 tabular_pipeline-0.2.1/tabular_pipeline/steps/load.py
--rw-r--r--   0        0        0      815 2023-06-02 17:14:24.374765 tabular_pipeline-0.2.1/tabular_pipeline/util.py
--rw-r--r--   0        0        0      671 2023-06-05 09:45:28.161925 tabular_pipeline-0.2.1/tabular_pipeline/write.py
--rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 tabular_pipeline-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1323 2023-06-02 17:51:00.351669 tabular_pipeline-0.2.2/README.md
+-rw-r--r--   0        0        0      521 2023-06-05 14:11:24.888804 tabular_pipeline-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-06-05 09:43:55.077866 tabular_pipeline-0.2.2/tabular_pipeline/__init__.py
+-rw-r--r--   0        0        0      656 2023-06-05 14:01:52.783432 tabular_pipeline-0.2.2/tabular_pipeline/pipeline.py
+-rw-r--r--   0        0        0     1486 2023-06-05 14:09:59.373417 tabular_pipeline-0.2.2/tabular_pipeline/read.py
+-rw-r--r--   0        0        0      411 2023-06-02 17:34:25.107821 tabular_pipeline-0.2.2/tabular_pipeline/schemas.py
+-rw-r--r--   0        0        0      929 2023-06-05 09:45:21.279463 tabular_pipeline-0.2.2/tabular_pipeline/settings.py
+-rw-r--r--   0        0        0     1447 2023-06-05 09:45:06.154756 tabular_pipeline-0.2.2/tabular_pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     1998 2023-06-05 09:44:56.165268 tabular_pipeline-0.2.2/tabular_pipeline/steps/conform.py
+-rw-r--r--   0        0        0     1603 2023-06-05 14:01:43.358642 tabular_pipeline-0.2.2/tabular_pipeline/steps/load.py
+-rw-r--r--   0        0        0      815 2023-06-02 17:14:24.374765 tabular_pipeline-0.2.2/tabular_pipeline/util.py
+-rw-r--r--   0        0        0      671 2023-06-05 09:45:28.161925 tabular_pipeline-0.2.2/tabular_pipeline/write.py
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 tabular_pipeline-0.2.2/PKG-INFO
```

### Comparing `tabular_pipeline-0.2.1/README.md` & `tabular_pipeline-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.1/pyproject.toml` & `tabular_pipeline-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "tabular-pipeline"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["franciscobmacedo <franciscovcbm@gmail.com>"]
 readme = "README.md"
 packages = [{include = "tabular_pipeline"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tablib = {extras = ["xlsx"], version = "^3.4.0"}
 pyyaml = "^6.0"
 pydantic = "^1.10.8"
-typer = {extras = ["all"], version = "^0.9.0"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 ruff = "^0.0.270"
 mypy = "^1.3.0"
```

### Comparing `tabular_pipeline-0.2.1/tabular_pipeline/read.py` & `tabular_pipeline-0.2.2/tabular_pipeline/read.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import os
 import uuid
 from typing import Optional
 
 import yaml
 from tablib import Databook, Dataset
+from io import StringIO
 
 from . import settings
 from .schemas import Schema
 from .schemas import StepChoices
 
 
 def load_schema(session_id: uuid.UUID, file_path: str) -> Schema:
     settings.read_logger.info(f"{session_id}: loading schema")
     with open(file_path, "rb") as fh:
         return Schema(**yaml.load(fh, Loader=yaml.FullLoader))
 
 
-def load_xlsx(file_path: str) -> Dataset:
-    with open(file_path, "rb") as fh:
-        databook = Databook().load(fh, "xlsx")
-    dataset: Dataset = databook.sheets()[
-        0
-    ]  # TODO - for now, one dataset is handled - it should handle many
-    return dataset
-
+def load_xlsx(file: str | bytes) -> Dataset:
+    if isinstance(file, bytes):
+        return Databook().load(file, "xlsx")
+    else:
+        with open(file, "rb") as fh:
+            databook = Databook().load(fh, "xlsx")
+
+    # TODO - for now, one dataset is handled - it should handle many
+    return databook.sheets()[0]
+
+
+def load_csv(file: str | bytes, delimiter: Optional[str] = ",") -> Dataset:
+    if isinstance(file, bytes):
+        file = StringIO(file.decode())
 
-def load_csv(file_path: str, delimiter: Optional[str] = ",") -> Dataset:
-    with open(file_path, "r") as fh:
+        return Dataset().load(file, "csv", delimiter=delimiter)
+    with open(file, "r") as fh:
         # FIXME - delimiter detection is not working
         # if not delimiter:
         # delimiter = detect_csv_delimiter(fh)
         return Dataset().load(fh, format="csv", delimiter=delimiter)
 
 
 def load_step_data(session_id: uuid.UUID, step: StepChoices) -> Dataset:
```

### Comparing `tabular_pipeline-0.2.1/tabular_pipeline/settings.py` & `tabular_pipeline-0.2.2/tabular_pipeline/settings.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.1/tabular_pipeline/steps/__init__.py` & `tabular_pipeline-0.2.2/tabular_pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.1/tabular_pipeline/steps/conform.py` & `tabular_pipeline-0.2.2/tabular_pipeline/steps/conform.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.1/tabular_pipeline/util.py` & `tabular_pipeline-0.2.2/tabular_pipeline/util.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.1/tabular_pipeline/write.py` & `tabular_pipeline-0.2.2/tabular_pipeline/write.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.1/PKG-INFO` & `tabular_pipeline-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: tabular-pipeline
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: franciscobmacedo
 Author-email: franciscovcbm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tablib[xlsx] (>=3.4.0,<4.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Data pipeline
 
 Data pipeline to ingest, conform, normalise, validate and export tabular data files (for now) given yml schema(s) as the only source of truth.
 It should be possible to easily plug it in modern orchestration tools such as Airflow and Dagster.
```

