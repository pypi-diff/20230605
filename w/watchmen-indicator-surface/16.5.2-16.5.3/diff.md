# Comparing `tmp/watchmen_indicator_surface-16.5.2.tar.gz` & `tmp/watchmen_indicator_surface-16.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_indicator_surface-16.5.2.tar", max compression
+gzip compressed data, was "watchmen_indicator_surface-16.5.3.tar", max compression
```

## Comparing `watchmen_indicator_surface-16.5.2.tar` & `watchmen_indicator_surface-16.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1025 2023-05-23 07:54:10.408670 watchmen_indicator_surface-16.5.2/pyproject.toml
--rw-r--r--   0        0        0       48 2023-05-23 07:54:10.408670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 07:54:10.408670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/data/__init__.py
--rw-r--r--   0        0        0     8936 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/data/objective_data_router.py
--rw-r--r--   0        0        0      541 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/main.py
--rw-r--r--   0        0        0        0 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/__init__.py
--rw-r--r--   0        0        0     6015 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py
--rw-r--r--   0        0        0     7181 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/bucket_router.py
--rw-r--r--   0        0        0     9156 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/derived_objective_router.py
--rw-r--r--   0        0        0     7904 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/indicator_router.py
--rw-r--r--   0        0        0    12699 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/objective_router.py
--rw-r--r--   0        0        0     5673 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/subject_router.py
--rw-r--r--   0        0        0      471 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/settings.py
--rw-r--r--   0        0        0       80 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/util/__init__.py
--rw-r--r--   0        0        0     2038 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/util/trans.py
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 watchmen_indicator_surface-16.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/data/__init__.py
+-rw-r--r--   0        0        0     8936 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/data/objective_data_router.py
+-rw-r--r--   0        0        0      541 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/main.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/__init__.py
+-rw-r--r--   0        0        0     6015 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py
+-rw-r--r--   0        0        0     7181 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/bucket_router.py
+-rw-r--r--   0        0        0     9156 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/derived_objective_router.py
+-rw-r--r--   0        0        0     7904 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/indicator_router.py
+-rw-r--r--   0        0        0    12699 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/objective_router.py
+-rw-r--r--   0        0        0     5673 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/subject_router.py
+-rw-r--r--   0        0        0      471 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/settings.py
+-rw-r--r--   0        0        0       80 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/util/__init__.py
+-rw-r--r--   0        0        0     2038 2023-06-05 01:29:03.512123 watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/util/trans.py
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 watchmen_indicator_surface-16.5.3/PKG-INFO
```

### Comparing `watchmen_indicator_surface-16.5.2/pyproject.toml` & `watchmen_indicator_surface-16.5.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "watchmen-indicator-surface"
-version = "16.5.2"
+version = "16.5.3"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_indicator_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-indicator-kernel = "16.5.2"
-watchmen-rest = "16.5.2"
-watchmen-storage-mysql = { version = "16.5.2", optional = true }
-watchmen-storage-oracle = { version = "16.5.2", optional = true }
-watchmen-storage-mongodb = { version = "16.5.2", optional = true }
-watchmen-storage-mssql = { version = "16.5.2", optional = true }
-watchmen-storage-postgresql = { version = "16.5.2", optional = true }
+watchmen-indicator-kernel = "16.5.3"
+watchmen-rest = "16.5.3"
+watchmen-storage-mysql = { version = "16.5.3", optional = true }
+watchmen-storage-oracle = { version = "16.5.3", optional = true }
+watchmen-storage-mongodb = { version = "16.5.3", optional = true }
+watchmen-storage-mssql = { version = "16.5.3", optional = true }
+watchmen-storage-postgresql = { version = "16.5.3", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/data/objective_data_router.py` & `watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/data/objective_data_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/main.py` & `watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/main.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py` & `watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/bucket_router.py` & `watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/bucket_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/derived_objective_router.py` & `watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/derived_objective_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/indicator_router.py` & `watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/indicator_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/objective_router.py` & `watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/objective_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/subject_router.py` & `watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/meta/subject_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/util/trans.py` & `watchmen_indicator_surface-16.5.3/src/watchmen_indicator_surface/util/trans.py`

 * *Files identical despite different names*

