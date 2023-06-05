# Comparing `tmp/alltime_athletics_python-0.4.0.tar.gz` & `tmp/alltime_athletics_python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alltime_athletics_python-0.4.0.tar", max compression
+gzip compressed data, was "alltime_athletics_python-0.5.0.tar", max compression
```

## Comparing `alltime_athletics_python-0.4.0.tar` & `alltime_athletics_python-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-01 06:57:21.506681 alltime_athletics_python-0.4.0/LICENSE
--rw-r--r--   0        0        0      299 2023-06-01 06:57:21.522140 alltime_athletics_python-0.4.0/alltime_athletics_python/__init__.py
--rw-r--r--   0        0        0     3205 2023-06-01 06:58:25.637564 alltime_athletics_python-0.4.0/alltime_athletics_python/get_content.py
--rw-r--r--   0        0        0     1915 2023-06-01 06:58:25.645679 alltime_athletics_python-0.4.0/alltime_athletics_python/get_content_urls.py
--rw-r--r--   0        0        0     3342 2023-06-05 07:05:46.470276 alltime_athletics_python-0.4.0/alltime_athletics_python/io.py
--rw-r--r--   0        0        0    10197 2023-06-05 06:57:35.426514 alltime_athletics_python-0.4.0/alltime_athletics_python/pipes.py
--rw-r--r--   0        0        0        0 2023-06-01 06:57:21.524099 alltime_athletics_python-0.4.0/alltime_athletics_python/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-06-01 06:57:21.523437 alltime_athletics_python-0.4.0/alltime_athletics_python/utils/config.py
--rw-r--r--   0        0        0      736 2023-06-01 06:57:21.525381 alltime_athletics_python-0.4.0/alltime_athletics_python/utils/logger.py
--rw-r--r--   0        0        0      924 2023-06-05 07:08:54.895206 alltime_athletics_python-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 alltime_athletics_python-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-01 06:57:21.506681 alltime_athletics_python-0.5.0/LICENSE
+-rw-r--r--   0        0        0      299 2023-06-01 06:57:21.522140 alltime_athletics_python-0.5.0/alltime_athletics_python/__init__.py
+-rw-r--r--   0        0        0     3205 2023-06-01 06:58:25.637564 alltime_athletics_python-0.5.0/alltime_athletics_python/get_content.py
+-rw-r--r--   0        0        0     1915 2023-06-01 06:58:25.645679 alltime_athletics_python-0.5.0/alltime_athletics_python/get_content_urls.py
+-rw-r--r--   0        0        0     3443 2023-06-05 07:12:25.924111 alltime_athletics_python-0.5.0/alltime_athletics_python/io.py
+-rw-r--r--   0        0        0    10197 2023-06-05 06:57:35.426514 alltime_athletics_python-0.5.0/alltime_athletics_python/pipes.py
+-rw-r--r--   0        0        0        0 2023-06-01 06:57:21.524099 alltime_athletics_python-0.5.0/alltime_athletics_python/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-01 06:57:21.523437 alltime_athletics_python-0.5.0/alltime_athletics_python/utils/config.py
+-rw-r--r--   0        0        0      736 2023-06-01 06:57:21.525381 alltime_athletics_python-0.5.0/alltime_athletics_python/utils/logger.py
+-rw-r--r--   0        0        0      924 2023-06-05 07:13:51.551849 alltime_athletics_python-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 alltime_athletics_python-0.5.0/PKG-INFO
```

### Comparing `alltime_athletics_python-0.4.0/LICENSE` & `alltime_athletics_python-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.4.0/alltime_athletics_python/get_content.py` & `alltime_athletics_python-0.5.0/alltime_athletics_python/get_content.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.4.0/alltime_athletics_python/get_content_urls.py` & `alltime_athletics_python-0.5.0/alltime_athletics_python/get_content_urls.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.4.0/alltime_athletics_python/io.py` & `alltime_athletics_python-0.5.0/alltime_athletics_python/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,27 +42,29 @@
         for content in list_of_content:
             Path(os.path.join(folder, content.folder)).mkdir(
                 parents=True, exist_ok=True
             )
             content.df.to_csv(os.path.join(folder, content.folder, content.filename))
 
 
-def import_running_only_events() -> pl.DataFrame:
+def import_running_only_events(data_root: str = "data") -> pl.DataFrame:
     df_men = import_running_only_events_sex(
-        pipe_rename_columns_names_men, "men"
+        data_root, pipe_rename_columns_names_men, "men"
     ).with_columns(pl.lit("men").alias("sex"))
     df_women = import_running_only_events_sex(
-        pipe_rename_columns_names_women, "women"
+        data_root, pipe_rename_columns_names_women, "women"
     ).with_columns(pl.lit("women").alias("sex"))
 
     return pl.concat([df_women, df_men])
 
 
 def import_running_only_events_sex(
-    pipe_rename_column_names: Callable[[pl.DataFrame], pl.DataFrame], sex: str
+    data_root: str,
+    pipe_rename_column_names: Callable[[pl.DataFrame], pl.DataFrame],
+    sex: str,
 ) -> pl.DataFrame:
     return pl.concat(
         [
             pl.read_csv(event, infer_schema_length=10000)
             .pipe(pipe_assign_file_name, event)
             .pipe(pipe_rename_column_names)
             .pipe(pipe_fix_dtype)
@@ -73,25 +75,25 @@
             .pipe(pipe_get_percentage_wrt_world_record)
             .pipe(pipe_assign_sprint_middle_long_distance)
             .pipe(pipe_assign_has_hurdles_or_not)
             .pipe(pipe_assign_track_event_or_not)
             .pipe(pipe_fix_issue_with_half_marathon_distance)
             .pipe(pipe_drop_unwanted_columns)
             .pipe(pipe_get_wr_strength_by_comparing_with_tenth)
-            for event in get_running_only_files(sex)
+            for event in get_running_only_files(data_root, sex)
         ],
         how="diagonal",
     )
 
 
-def get_running_only_files(sex: str) -> list[str]:
+def get_running_only_files(data_root: str, sex: str) -> list[str]:
     return [
         f
         for f in glob.glob(  # Get all csv files recursively.
-            f"../data/{sex}/standard/*/legal/0*.csv", recursive=True
+            f"{data_root}/{sex}/standard/*/legal/0*.csv", recursive=True
         )
         if (
             "metres" in f
             or "00m" in f
             or "Mile" in f
             or "One hour" in f
             or "km" in f
```

### Comparing `alltime_athletics_python-0.4.0/alltime_athletics_python/pipes.py` & `alltime_athletics_python-0.5.0/alltime_athletics_python/pipes.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.4.0/alltime_athletics_python/utils/config.py` & `alltime_athletics_python-0.5.0/alltime_athletics_python/utils/config.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.4.0/alltime_athletics_python/utils/logger.py` & `alltime_athletics_python-0.5.0/alltime_athletics_python/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.4.0/pyproject.toml` & `alltime_athletics_python-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alltime_athletics_python"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.2"
 lxml = "^4.9.2"
```

### Comparing `alltime_athletics_python-0.4.0/PKG-INFO` & `alltime_athletics_python-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alltime-athletics-python
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

