# Comparing `tmp/tabular_pipeline-0.2.2.tar.gz` & `tmp/tabular_pipeline-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabular_pipeline-0.2.2.tar", max compression
+gzip compressed data, was "tabular_pipeline-0.2.3.tar", max compression
```

## Comparing `tabular_pipeline-0.2.2.tar` & `tabular_pipeline-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1323 2023-06-02 17:51:00.351669 tabular_pipeline-0.2.2/README.md
--rw-r--r--   0        0        0      521 2023-06-05 14:11:24.888804 tabular_pipeline-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       33 2023-06-05 09:43:55.077866 tabular_pipeline-0.2.2/tabular_pipeline/__init__.py
--rw-r--r--   0        0        0      656 2023-06-05 14:01:52.783432 tabular_pipeline-0.2.2/tabular_pipeline/pipeline.py
--rw-r--r--   0        0        0     1486 2023-06-05 14:09:59.373417 tabular_pipeline-0.2.2/tabular_pipeline/read.py
--rw-r--r--   0        0        0      411 2023-06-02 17:34:25.107821 tabular_pipeline-0.2.2/tabular_pipeline/schemas.py
--rw-r--r--   0        0        0      929 2023-06-05 09:45:21.279463 tabular_pipeline-0.2.2/tabular_pipeline/settings.py
--rw-r--r--   0        0        0     1447 2023-06-05 09:45:06.154756 tabular_pipeline-0.2.2/tabular_pipeline/steps/__init__.py
--rw-r--r--   0        0        0     1998 2023-06-05 09:44:56.165268 tabular_pipeline-0.2.2/tabular_pipeline/steps/conform.py
--rw-r--r--   0        0        0     1603 2023-06-05 14:01:43.358642 tabular_pipeline-0.2.2/tabular_pipeline/steps/load.py
--rw-r--r--   0        0        0      815 2023-06-02 17:14:24.374765 tabular_pipeline-0.2.2/tabular_pipeline/util.py
--rw-r--r--   0        0        0      671 2023-06-05 09:45:28.161925 tabular_pipeline-0.2.2/tabular_pipeline/write.py
--rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 tabular_pipeline-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1323 2023-06-02 17:51:00.351669 tabular_pipeline-0.2.3/README.md
+-rw-r--r--   0        0        0      521 2023-06-05 15:07:40.887803 tabular_pipeline-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-06-05 09:43:55.077866 tabular_pipeline-0.2.3/tabular_pipeline/__init__.py
+-rw-r--r--   0        0        0      658 2023-06-05 14:31:12.520295 tabular_pipeline-0.2.3/tabular_pipeline/pipeline.py
+-rw-r--r--   0        0        0     1489 2023-06-05 15:07:23.691477 tabular_pipeline-0.2.3/tabular_pipeline/read.py
+-rw-r--r--   0        0        0      411 2023-06-02 17:34:25.107821 tabular_pipeline-0.2.3/tabular_pipeline/schemas.py
+-rw-r--r--   0        0        0      929 2023-06-05 09:45:21.279463 tabular_pipeline-0.2.3/tabular_pipeline/settings.py
+-rw-r--r--   0        0        0     1447 2023-06-05 09:45:06.154756 tabular_pipeline-0.2.3/tabular_pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     1998 2023-06-05 09:44:56.165268 tabular_pipeline-0.2.3/tabular_pipeline/steps/conform.py
+-rw-r--r--   0        0        0     1603 2023-06-05 14:01:43.358642 tabular_pipeline-0.2.3/tabular_pipeline/steps/load.py
+-rw-r--r--   0        0        0      815 2023-06-02 17:14:24.374765 tabular_pipeline-0.2.3/tabular_pipeline/util.py
+-rw-r--r--   0        0        0      671 2023-06-05 09:45:28.161925 tabular_pipeline-0.2.3/tabular_pipeline/write.py
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 tabular_pipeline-0.2.3/PKG-INFO
```

### Comparing `tabular_pipeline-0.2.2/README.md` & `tabular_pipeline-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.2/pyproject.toml` & `tabular_pipeline-0.2.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tabular-pipeline"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["franciscobmacedo <franciscovcbm@gmail.com>"]
 readme = "README.md"
 packages = [{include = "tabular_pipeline"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tabular_pipeline-0.2.2/tabular_pipeline/pipeline.py` & `tabular_pipeline-0.2.3/tabular_pipeline/pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 def standardise(
     schema: str,
     file_path: str | None = None,
     file_name: str | None = None,
     file_content: bytes | None = None,
 ):
     session_id = uuid.uuid4()
-    schema = load_schema(session_id, schema)
+    _schema = load_schema(session_id, schema)
     loader = Load(
         session_id=session_id,
         file_path=file_path,
         file_name=file_name,
         file_content=file_content,
     )
-    conformer = Conform(session_id=session_id, schema=schema)
+    conformer = Conform(session_id=session_id, schema=_schema)
     # TODO - normaliser, validator
 
     loader.run()
     conformer.run()
     return conformer.dataset.export("xlsx")
```

### Comparing `tabular_pipeline-0.2.2/tabular_pipeline/read.py` & `tabular_pipeline-0.2.3/tabular_pipeline/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,26 @@
     settings.read_logger.info(f"{session_id}: loading schema")
     with open(file_path, "rb") as fh:
         return Schema(**yaml.load(fh, Loader=yaml.FullLoader))
 
 
 def load_xlsx(file: str | bytes) -> Dataset:
     if isinstance(file, bytes):
-        return Databook().load(file, "xlsx")
+        databook = Databook().load(file, "xlsx")
     else:
         with open(file, "rb") as fh:
             databook = Databook().load(fh, "xlsx")
 
     # TODO - for now, one dataset is handled - it should handle many
     return databook.sheets()[0]
 
 
 def load_csv(file: str | bytes, delimiter: Optional[str] = ",") -> Dataset:
     if isinstance(file, bytes):
         file = StringIO(file.decode())
-
         return Dataset().load(file, "csv", delimiter=delimiter)
     with open(file, "r") as fh:
         # FIXME - delimiter detection is not working
         # if not delimiter:
         # delimiter = detect_csv_delimiter(fh)
         return Dataset().load(fh, format="csv", delimiter=delimiter)
```

### Comparing `tabular_pipeline-0.2.2/tabular_pipeline/settings.py` & `tabular_pipeline-0.2.3/tabular_pipeline/settings.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.2/tabular_pipeline/steps/__init__.py` & `tabular_pipeline-0.2.3/tabular_pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.2/tabular_pipeline/steps/conform.py` & `tabular_pipeline-0.2.3/tabular_pipeline/steps/conform.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.2/tabular_pipeline/steps/load.py` & `tabular_pipeline-0.2.3/tabular_pipeline/steps/load.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.2/tabular_pipeline/util.py` & `tabular_pipeline-0.2.3/tabular_pipeline/util.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.2/tabular_pipeline/write.py` & `tabular_pipeline-0.2.3/tabular_pipeline/write.py`

 * *Files identical despite different names*

### Comparing `tabular_pipeline-0.2.2/PKG-INFO` & `tabular_pipeline-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabular-pipeline
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: franciscobmacedo
 Author-email: franciscovcbm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

