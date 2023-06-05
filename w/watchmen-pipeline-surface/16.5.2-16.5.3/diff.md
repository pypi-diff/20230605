# Comparing `tmp/watchmen_pipeline_surface-16.5.2.tar.gz` & `tmp/watchmen_pipeline_surface-16.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_pipeline_surface-16.5.2.tar", max compression
+gzip compressed data, was "watchmen_pipeline_surface-16.5.3.tar", max compression
```

## Comparing `watchmen_pipeline_surface-16.5.2.tar` & `watchmen_pipeline_surface-16.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/LICENSE
--rw-r--r--   0        0        0     1388 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/pyproject.toml
--rw-r--r--   0        0        0      102 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/__init__.py
--rw-r--r--   0        0        0       99 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/connectors/__init__.py
--rw-r--r--   0        0        0      854 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/connectors/handler.py
--rw-r--r--   0        0        0     1218 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/connectors/kafka.py
--rw-r--r--   0        0        0     1689 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/connectors/rabbitmq.py
--rw-r--r--   0        0        0        0 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/data/__init__.py
--rw-r--r--   0        0        0     1619 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/data/monitor_log_router.py
--rw-r--r--   0        0        0     1727 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/data/pipeline_trigger_router.py
--rw-r--r--   0        0        0     2742 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/data/topic_snapshot_adhoc_router.py
--rw-r--r--   0        0        0     5996 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/data/topic_trigger_router.py
--rw-r--r--   0        0        0      370 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/main.py
--rw-r--r--   0        0        0     1637 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/settings.py
--rw-r--r--   0        0        0     1162 2023-05-23 07:54:10.424671 watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/surface.py
--rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 watchmen_pipeline_surface-16.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/LICENSE
+-rw-r--r--   0        0        0     1388 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/__init__.py
+-rw-r--r--   0        0        0       99 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/connectors/__init__.py
+-rw-r--r--   0        0        0      854 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/connectors/handler.py
+-rw-r--r--   0        0        0     1218 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/connectors/kafka.py
+-rw-r--r--   0        0        0     1689 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/connectors/rabbitmq.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/data/__init__.py
+-rw-r--r--   0        0        0     1619 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/data/monitor_log_router.py
+-rw-r--r--   0        0        0     1727 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/data/pipeline_trigger_router.py
+-rw-r--r--   0        0        0     2742 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/data/topic_snapshot_adhoc_router.py
+-rw-r--r--   0        0        0     5996 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/data/topic_trigger_router.py
+-rw-r--r--   0        0        0      370 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/main.py
+-rw-r--r--   0        0        0     1637 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/settings.py
+-rw-r--r--   0        0        0     1162 2023-06-05 01:29:03.532124 watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/surface.py
+-rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 watchmen_pipeline_surface-16.5.3/PKG-INFO
```

### Comparing `watchmen_pipeline_surface-16.5.2/LICENSE` & `watchmen_pipeline_surface-16.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_surface-16.5.2/pyproject.toml` & `watchmen_pipeline_surface-16.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "watchmen-pipeline-surface"
-version = "16.5.2"
+version = "16.5.3"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_pipeline_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-pipeline-kernel = "16.5.2"
-watchmen-rest = "16.5.2"
-watchmen-storage-mysql = { version = "16.5.2", optional = true }
-watchmen-storage-oracle = { version = "16.5.2", optional = true }
-watchmen-storage-mongodb = { version = "16.5.2", optional = true }
-watchmen-storage-mssql = { version = "16.5.2", optional = true }
-watchmen-storage-postgresql = { version = "16.5.2", optional = true }
+watchmen-pipeline-kernel = "16.5.3"
+watchmen-rest = "16.5.3"
+watchmen-storage-mysql = { version = "16.5.3", optional = true }
+watchmen-storage-oracle = { version = "16.5.3", optional = true }
+watchmen-storage-mongodb = { version = "16.5.3", optional = true }
+watchmen-storage-mssql = { version = "16.5.3", optional = true }
+watchmen-storage-postgresql = { version = "16.5.3", optional = true }
 kafka-python = { version = "^2.0.2", optional = true }
 aiokafka = { version = "^0.7.2", optional = true }
 aio-pika = { version = "^7.1.2", optional = true }
 requests = { version = "^2.27.1", optional = true }
 
 [tool.poetry.dev-dependencies]
```

### Comparing `watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/connectors/handler.py` & `watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/connectors/handler.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/connectors/kafka.py` & `watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/connectors/kafka.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/connectors/rabbitmq.py` & `watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/connectors/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/data/monitor_log_router.py` & `watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/data/monitor_log_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/data/pipeline_trigger_router.py` & `watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/data/pipeline_trigger_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/data/topic_snapshot_adhoc_router.py` & `watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/data/topic_snapshot_adhoc_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/data/topic_trigger_router.py` & `watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/data/topic_trigger_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/settings.py` & `watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_surface-16.5.2/src/watchmen_pipeline_surface/surface.py` & `watchmen_pipeline_surface-16.5.3/src/watchmen_pipeline_surface/surface.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_surface-16.5.2/PKG-INFO` & `watchmen_pipeline_surface-16.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-pipeline-surface
-Version: 16.5.2
+Version: 16.5.3
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +21,14 @@
 Provides-Extra: postgresql
 Provides-Extra: rabbitmq
 Provides-Extra: standard-ext-writer
 Requires-Dist: aio-pika (>=7.1.2,<8.0.0) ; extra == "rabbitmq"
 Requires-Dist: aiokafka (>=0.7.2,<0.8.0) ; extra == "kafka"
 Requires-Dist: kafka-python (>=2.0.2,<3.0.0) ; extra == "kafka"
 Requires-Dist: requests (>=2.27.1,<3.0.0) ; extra == "standard-ext-writer"
-Requires-Dist: watchmen-pipeline-kernel (==16.5.2)
-Requires-Dist: watchmen-rest (==16.5.2)
-Requires-Dist: watchmen-storage-mongodb (==16.5.2) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.2) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.2) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.2) ; extra == "oracle"
-Requires-Dist: watchmen-storage-postgresql (==16.5.2) ; extra == "postgresql"
+Requires-Dist: watchmen-pipeline-kernel (==16.5.3)
+Requires-Dist: watchmen-rest (==16.5.3)
+Requires-Dist: watchmen-storage-mongodb (==16.5.3) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.3) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.3) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.3) ; extra == "oracle"
+Requires-Dist: watchmen-storage-postgresql (==16.5.3) ; extra == "postgresql"
```

