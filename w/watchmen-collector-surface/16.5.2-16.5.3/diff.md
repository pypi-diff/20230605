# Comparing `tmp/watchmen_collector_surface-16.5.2.tar.gz` & `tmp/watchmen_collector_surface-16.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_collector_surface-16.5.2.tar", max compression
+gzip compressed data, was "watchmen_collector_surface-16.5.3.tar", max compression
```

## Comparing `watchmen_collector_surface-16.5.2.tar` & `watchmen_collector_surface-16.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/LICENSE
--rw-r--r--   0        0        0     1247 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/pyproject.toml
--rw-r--r--   0        0        0      106 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/__init__.py
--rw-r--r--   0        0        0      188 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/cdc/__init__.py
--rw-r--r--   0        0        0     5306 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/cdc/monitor_event.py
--rw-r--r--   0        0        0    11506 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/cdc/post_json.py
--rw-r--r--   0        0        0    10062 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/cdc/record_to_json.py
--rw-r--r--   0        0        0     7538 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/cdc/table_extractor.py
--rw-r--r--   0        0        0       65 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/connects/__init__.py
--rw-r--r--   0        0        0     4829 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/connects/s3_connector.py
--rw-r--r--   0        0        0        0 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/data/__init__.py
--rw-r--r--   0        0        0     3988 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/data/config_router.py
--rw-r--r--   0        0        0     2034 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/data/task_router.py
--rw-r--r--   0        0        0     1450 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/data/trigger_router.py
--rw-r--r--   0        0        0      258 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/main.py
--rw-r--r--   0        0        0     1716 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/settings.py
--rw-r--r--   0        0        0     1230 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/surface.py
--rw-r--r--   0        0        0       46 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/task/__init__.py
--rw-r--r--   0        0        0     2329 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/task/handler.py
--rw-r--r--   0        0        0     2737 2023-05-23 07:54:10.400669 watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/task/task_listener.py
--rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 watchmen_collector_surface-16.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.496123 watchmen_collector_surface-16.5.3/LICENSE
+-rw-r--r--   0        0        0     1247 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/__init__.py
+-rw-r--r--   0        0        0      188 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/cdc/__init__.py
+-rw-r--r--   0        0        0     5306 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/cdc/monitor_event.py
+-rw-r--r--   0        0        0    11506 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/cdc/post_json.py
+-rw-r--r--   0        0        0    10062 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/cdc/record_to_json.py
+-rw-r--r--   0        0        0     7551 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/cdc/table_extractor.py
+-rw-r--r--   0        0        0       65 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/connects/__init__.py
+-rw-r--r--   0        0        0     4829 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/connects/s3_connector.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/data/__init__.py
+-rw-r--r--   0        0        0     3988 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/data/config_router.py
+-rw-r--r--   0        0        0     2034 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/data/task_router.py
+-rw-r--r--   0        0        0     1450 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/data/trigger_router.py
+-rw-r--r--   0        0        0      258 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/main.py
+-rw-r--r--   0        0        0     1716 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/settings.py
+-rw-r--r--   0        0        0     1230 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/surface.py
+-rw-r--r--   0        0        0       46 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/task/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/task/handler.py
+-rw-r--r--   0        0        0     2737 2023-06-05 01:29:03.500123 watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/task/task_listener.py
+-rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 watchmen_collector_surface-16.5.3/PKG-INFO
```

### Comparing `watchmen_collector_surface-16.5.2/LICENSE` & `watchmen_collector_surface-16.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/pyproject.toml` & `watchmen_collector_surface-16.5.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-collector-surface"
-version = "16.5.2"
+version = "16.5.3"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_collector_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-collector-kernel = "16.5.2"
-watchmen-pipeline-kernel = "16.5.2"
-watchmen-rest = "16.5.2"
-watchmen-storage-mysql = { version = "16.5.2", optional = true }
-watchmen-storage-oracle = { version = "16.5.2", optional = true }
-watchmen-storage-mongodb = { version = "16.5.2", optional = true }
-watchmen-storage-mssql = { version = "16.5.2", optional = true }
-watchmen-storage-postgresql = { version = "16.5.2", optional = true }
-watchmen-storage-oss = { version = "16.5.2", optional = true }
-watchmen-storage-s3 = { version = "16.5.2", optional = true }
+watchmen-collector-kernel = "16.5.3"
+watchmen-pipeline-kernel = "16.5.3"
+watchmen-rest = "16.5.3"
+watchmen-storage-mysql = { version = "16.5.3", optional = true }
+watchmen-storage-oracle = { version = "16.5.3", optional = true }
+watchmen-storage-mongodb = { version = "16.5.3", optional = true }
+watchmen-storage-mssql = { version = "16.5.3", optional = true }
+watchmen-storage-postgresql = { version = "16.5.3", optional = true }
+watchmen-storage-oss = { version = "16.5.3", optional = true }
+watchmen-storage-s3 = { version = "16.5.3", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/cdc/monitor_event.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/cdc/monitor_event.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/cdc/post_json.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/cdc/post_json.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/cdc/record_to_json.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/cdc/record_to_json.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/cdc/table_extractor.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/cdc/table_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from logging import getLogger
 from threading import Thread
 from typing import Tuple, Dict, List, Any
 from time import sleep
 
 import numpy as np
 
-from watchmen_collector_kernel.common import COMMA
 from watchmen_collector_kernel.model import TriggerEvent, ChangeDataRecord, TriggerTable, CollectorTableConfig, \
 	Condition
 from watchmen_collector_kernel.service import try_lock_nowait, unlock, SourceTableExtractor, CriteriaBuilder, \
 	build_audit_column_criteria
 from watchmen_collector_kernel.service.extract_utils import cal_array2d_diff, build_data_id, get_data_id
 from watchmen_collector_kernel.service.lock_helper import get_resource_lock
 from watchmen_collector_kernel.storage import get_trigger_table_service, get_competitive_lock_service, \
@@ -106,21 +105,21 @@
 								criteria
 							)
 							existed_records = self.change_data_record_service.find_existed_records(
 								trigger.tableTriggerId)
 							if existed_records:
 								diff_records: List[List] = self.get_diff(source_records, existed_records)
 								logger.info(
-									f'source_records: {len(source_records)}, existed_records: {len(existed_records)}, diffs: {len(diff_records)}'
+									f'table_name: {config.tableName}, source_records: {len(source_records)}, existed_records: {len(existed_records)}, diffs: {len(diff_records)}'
 								)
 								for diff_record in diff_records:
 									self.save_change_data_record(trigger, build_data_id(config.primaryKey, diff_record))
 							else:
 								logger.info(
-									f'source_records: {len(source_records)}, existed_records: {len(existed_records)}'
+									f'table_name: {config.tableName}, source_records: {len(source_records)}, existed_records: {len(existed_records)}'
 								)
 								ArrayHelper(source_records).map(
 									lambda record: self.save_change_data_record(trigger, get_data_id(config.primaryKey, record)))
 							data_count = ArrayHelper(source_records).size()
 							self.trigger_table_service.update_table_trigger(self.set_extracted(trigger, data_count))
 							break
 				finally:
```

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/connects/s3_connector.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/connects/s3_connector.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/data/config_router.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/data/config_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/data/task_router.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/data/task_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/data/trigger_router.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/data/trigger_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/settings.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/surface.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/surface.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/task/handler.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/task/handler.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/src/watchmen_collector_surface/task/task_listener.py` & `watchmen_collector_surface-16.5.3/src/watchmen_collector_surface/task/task_listener.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.2/PKG-INFO` & `watchmen_collector_surface-16.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-collector-surface
-Version: 16.5.2
+Version: 16.5.3
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,17 +14,17 @@
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
-Requires-Dist: watchmen-collector-kernel (==16.5.2)
-Requires-Dist: watchmen-pipeline-kernel (==16.5.2)
-Requires-Dist: watchmen-rest (==16.5.2)
-Requires-Dist: watchmen-storage-mongodb (==16.5.2) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.2) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.2) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.2) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.2) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.2) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.2) ; extra == "s3"
+Requires-Dist: watchmen-collector-kernel (==16.5.3)
+Requires-Dist: watchmen-pipeline-kernel (==16.5.3)
+Requires-Dist: watchmen-rest (==16.5.3)
+Requires-Dist: watchmen-storage-mongodb (==16.5.3) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.3) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.3) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.3) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.3) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.3) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.3) ; extra == "s3"
```

