# Comparing `tmp/alltime_athletics_python-0.5.0.tar.gz` & `tmp/alltime_athletics_python-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alltime_athletics_python-0.5.0.tar", max compression
+gzip compressed data, was "alltime_athletics_python-0.6.0.tar", max compression
```

## Comparing `alltime_athletics_python-0.5.0.tar` & `alltime_athletics_python-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-01 06:57:21.506681 alltime_athletics_python-0.5.0/LICENSE
--rw-r--r--   0        0        0      299 2023-06-01 06:57:21.522140 alltime_athletics_python-0.5.0/alltime_athletics_python/__init__.py
--rw-r--r--   0        0        0     3205 2023-06-01 06:58:25.637564 alltime_athletics_python-0.5.0/alltime_athletics_python/get_content.py
--rw-r--r--   0        0        0     1915 2023-06-01 06:58:25.645679 alltime_athletics_python-0.5.0/alltime_athletics_python/get_content_urls.py
--rw-r--r--   0        0        0     3443 2023-06-05 07:12:25.924111 alltime_athletics_python-0.5.0/alltime_athletics_python/io.py
--rw-r--r--   0        0        0    10197 2023-06-05 06:57:35.426514 alltime_athletics_python-0.5.0/alltime_athletics_python/pipes.py
--rw-r--r--   0        0        0        0 2023-06-01 06:57:21.524099 alltime_athletics_python-0.5.0/alltime_athletics_python/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-06-01 06:57:21.523437 alltime_athletics_python-0.5.0/alltime_athletics_python/utils/config.py
--rw-r--r--   0        0        0      736 2023-06-01 06:57:21.525381 alltime_athletics_python-0.5.0/alltime_athletics_python/utils/logger.py
--rw-r--r--   0        0        0      924 2023-06-05 07:13:51.551849 alltime_athletics_python-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 alltime_athletics_python-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-01 06:57:21.506681 alltime_athletics_python-0.6.0/LICENSE
+-rw-r--r--   0        0        0      299 2023-06-01 06:57:21.522140 alltime_athletics_python-0.6.0/alltime_athletics_python/__init__.py
+-rw-r--r--   0        0        0     3205 2023-06-01 06:58:25.637564 alltime_athletics_python-0.6.0/alltime_athletics_python/get_content.py
+-rw-r--r--   0        0        0     1915 2023-06-01 06:58:25.645679 alltime_athletics_python-0.6.0/alltime_athletics_python/get_content_urls.py
+-rw-r--r--   0        0        0     3445 2023-06-05 07:19:13.675960 alltime_athletics_python-0.6.0/alltime_athletics_python/io.py
+-rw-r--r--   0        0        0    10197 2023-06-05 06:57:35.426514 alltime_athletics_python-0.6.0/alltime_athletics_python/pipes.py
+-rw-r--r--   0        0        0        0 2023-06-01 06:57:21.524099 alltime_athletics_python-0.6.0/alltime_athletics_python/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-01 06:57:21.523437 alltime_athletics_python-0.6.0/alltime_athletics_python/utils/config.py
+-rw-r--r--   0        0        0      736 2023-06-01 06:57:21.525381 alltime_athletics_python-0.6.0/alltime_athletics_python/utils/logger.py
+-rw-r--r--   0        0        0      924 2023-06-05 07:19:47.146074 alltime_athletics_python-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 alltime_athletics_python-0.6.0/PKG-INFO
```

### Comparing `alltime_athletics_python-0.5.0/LICENSE` & `alltime_athletics_python-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.5.0/alltime_athletics_python/get_content.py` & `alltime_athletics_python-0.6.0/alltime_athletics_python/get_content.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.5.0/alltime_athletics_python/get_content_urls.py` & `alltime_athletics_python-0.6.0/alltime_athletics_python/get_content_urls.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.5.0/alltime_athletics_python/io.py` & `alltime_athletics_python-0.6.0/alltime_athletics_python/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         for content in list_of_content:
             Path(os.path.join(folder, content.folder)).mkdir(
                 parents=True, exist_ok=True
             )
             content.df.to_csv(os.path.join(folder, content.folder, content.filename))
 
 
-def import_running_only_events(data_root: str = "data") -> pl.DataFrame:
+def import_running_only_events(data_root: str = "./data") -> pl.DataFrame:
     df_men = import_running_only_events_sex(
         data_root, pipe_rename_columns_names_men, "men"
     ).with_columns(pl.lit("men").alias("sex"))
     df_women = import_running_only_events_sex(
         data_root, pipe_rename_columns_names_women, "women"
     ).with_columns(pl.lit("women").alias("sex"))
```

### Comparing `alltime_athletics_python-0.5.0/alltime_athletics_python/pipes.py` & `alltime_athletics_python-0.6.0/alltime_athletics_python/pipes.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.5.0/alltime_athletics_python/utils/config.py` & `alltime_athletics_python-0.6.0/alltime_athletics_python/utils/config.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.5.0/alltime_athletics_python/utils/logger.py` & `alltime_athletics_python-0.6.0/alltime_athletics_python/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.5.0/pyproject.toml` & `alltime_athletics_python-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alltime_athletics_python"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.2"
 lxml = "^4.9.2"
```

### Comparing `alltime_athletics_python-0.5.0/PKG-INFO` & `alltime_athletics_python-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alltime-athletics-python
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

