# Comparing `tmp/watchmen_collector_kernel-16.5.2.tar.gz` & `tmp/watchmen_collector_kernel-16.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_collector_kernel-16.5.2.tar", max compression
+gzip compressed data, was "watchmen_collector_kernel-16.5.3.tar", max compression
```

## Comparing `watchmen_collector_kernel-16.5.2.tar` & `watchmen_collector_kernel-16.5.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/LICENSE
--rw-r--r--   0        0        0     1197 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/__init__.py
--rw-r--r--   0        0        0      263 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/common/__init__.py
--rw-r--r--   0        0        0      302 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/common/constants.py
--rw-r--r--   0        0        0      697 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/common/settings.py
--rw-r--r--   0        0        0      666 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/__init__.py
--rw-r--r--   0        0        0      495 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/change_data_json.py
--rw-r--r--   0        0        0       99 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/change_data_json_history.py
--rw-r--r--   0        0        0      330 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/change_data_record.py
--rw-r--r--   0        0        0      106 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/change_data_record_history.py
--rw-r--r--   0        0        0      288 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/collector_model_config.py
--rw-r--r--   0        0        0     2143 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/collector_table_config.py
--rw-r--r--   0        0        0      264 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/competitive_lock.py
--rw-r--r--   0        0        0     1942 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/condition.py
--rw-r--r--   0        0        0     1362 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/scheduled_task.py
--rw-r--r--   0        0        0       93 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/scheduled_task_history.py
--rw-r--r--   0        0        0      251 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/trigger_event.py
--rw-r--r--   0        0        0      175 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/trigger_model.py
--rw-r--r--   0        0        0      229 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/trigger_table.py
--rw-r--r--   0        0        0      426 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/__init__.py
--rw-r--r--   0        0        0     2360 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/criteria_builder.py
--rw-r--r--   0        0        0     2873 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/data_capture.py
--rw-r--r--   0        0        0     2928 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/extract_source.py
--rw-r--r--   0        0        0     2452 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/extract_utils.py
--rw-r--r--   0        0        0     1142 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/lock_clean.py
--rw-r--r--   0        0        0      842 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/lock_helper.py
--rw-r--r--   0        0        0     1673 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/task_housekeeping.py
--rw-r--r--   0        0        0     3634 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/task_service.py
--rw-r--r--   0        0        0     6790 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/trigger_collector.py
--rw-r--r--   0        0        0     1173 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/__init__.py
--rw-r--r--   0        0        0     1774 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_json_history_service.py
--rw-r--r--   0        0        0     8464 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_json_service.py
--rw-r--r--   0        0        0     1845 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_record_history_service.py
--rw-r--r--   0        0        0     7953 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_record_service.py
--rw-r--r--   0        0        0     3830 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/collector_model_config_service.py
--rw-r--r--   0        0        0     5659 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/collector_table_config_service.py
--rw-r--r--   0        0        0     2534 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/competitive_lock_service.py
--rw-r--r--   0        0        0     1586 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py
--rw-r--r--   0        0        0     6825 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/scheduled_task_service.py
--rw-r--r--   0        0        0     3099 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_event_service.py
--rw-r--r--   0        0        0     3219 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_model_service.py
--rw-r--r--   0        0        0     3779 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_table_service.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 watchmen_collector_kernel-16.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/LICENSE
+-rw-r--r--   0        0        0     1197 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/__init__.py
+-rw-r--r--   0        0        0      263 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/common/__init__.py
+-rw-r--r--   0        0        0      302 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/common/constants.py
+-rw-r--r--   0        0        0      697 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/common/settings.py
+-rw-r--r--   0        0        0      666 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/change_data_json.py
+-rw-r--r--   0        0        0       99 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/change_data_json_history.py
+-rw-r--r--   0        0        0      330 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/change_data_record.py
+-rw-r--r--   0        0        0      106 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/change_data_record_history.py
+-rw-r--r--   0        0        0      288 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/collector_model_config.py
+-rw-r--r--   0        0        0     2907 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/collector_table_config.py
+-rw-r--r--   0        0        0      264 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/competitive_lock.py
+-rw-r--r--   0        0        0     1942 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/condition.py
+-rw-r--r--   0        0        0     1362 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/scheduled_task.py
+-rw-r--r--   0        0        0       93 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/scheduled_task_history.py
+-rw-r--r--   0        0        0      251 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/trigger_event.py
+-rw-r--r--   0        0        0      175 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/trigger_model.py
+-rw-r--r--   0        0        0      229 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/trigger_table.py
+-rw-r--r--   0        0        0      426 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/__init__.py
+-rw-r--r--   0        0        0     2360 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/criteria_builder.py
+-rw-r--r--   0        0        0     2873 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/data_capture.py
+-rw-r--r--   0        0        0     6560 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/extract_source.py
+-rw-r--r--   0        0        0     2452 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/extract_utils.py
+-rw-r--r--   0        0        0     1142 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/lock_clean.py
+-rw-r--r--   0        0        0      842 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/lock_helper.py
+-rw-r--r--   0        0        0     1673 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/task_housekeeping.py
+-rw-r--r--   0        0        0     3821 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/task_service.py
+-rw-r--r--   0        0        0     6790 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/trigger_collector.py
+-rw-r--r--   0        0        0     1173 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     1774 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/change_data_json_history_service.py
+-rw-r--r--   0        0        0     8464 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/change_data_json_service.py
+-rw-r--r--   0        0        0     1845 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/change_data_record_history_service.py
+-rw-r--r--   0        0        0     7953 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/change_data_record_service.py
+-rw-r--r--   0        0        0     3830 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/collector_model_config_service.py
+-rw-r--r--   0        0        0     5882 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/collector_table_config_service.py
+-rw-r--r--   0        0        0     2534 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/competitive_lock_service.py
+-rw-r--r--   0        0        0     1586 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py
+-rw-r--r--   0        0        0     6825 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/scheduled_task_service.py
+-rw-r--r--   0        0        0     3099 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/trigger_event_service.py
+-rw-r--r--   0        0        0     3219 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/trigger_model_service.py
+-rw-r--r--   0        0        0     3779 2023-06-05 01:29:03.496123 watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/trigger_table_service.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 watchmen_collector_kernel-16.5.3/PKG-INFO
```

### Comparing `watchmen_collector_kernel-16.5.2/LICENSE` & `watchmen_collector_kernel-16.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/pyproject.toml` & `watchmen_collector_kernel-16.5.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-collector-kernel"
-version = "16.5.2"
+version = "16.5.3"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_collector_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.23.3"
-watchmen-data-kernel = "16.5.2"
-watchmen-storage-mysql = { version = "16.5.2", optional = true }
-watchmen-storage-oracle = { version = "16.5.2", optional = true }
-watchmen-storage-mongodb = { version = "16.5.2", optional = true }
-watchmen-storage-mssql = { version = "16.5.2", optional = true }
-watchmen-storage-postgresql = { version = "16.5.2", optional = true }
-watchmen-storage-oss = { version = "16.5.2", optional = true }
-watchmen-storage-s3 = { version = "16.5.2", optional = true }
+watchmen-data-kernel = "16.5.3"
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

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/common/settings.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/__init__.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/collector_table_config.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/collector_table_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,37 @@
 
 
 class Dependence(Storable, BaseModel):
 	modelName: str
 	objectKey: str  # the dependent column
 
 
+class JsonColumn(Storable, BaseModel):
+	columnName: str = None
+	ignoredPath: List[str] = None
+	needFlatten: bool = None
+	flattenPath: List[str] = None
+
+
+def construct_json_column(json_column: Union[JsonColumn, Dict]) -> Optional[JsonColumn]:
+	if json_column is None:
+		return None
+	elif isinstance(json_column, JsonColumn):
+		return json_column
+	else:
+		return JsonColumn(**json_column)
+
+
+def construct_json_columns(json_columns: Optional[List[Union[JsonColumn, Dict]]]) -> Optional[List[JsonColumn]]:
+	if json_columns is None:
+		return None
+	else:
+		return ArrayHelper(json_columns).map(lambda x: construct_json_column(x)).to_list()
+
+
 def construct_join_key(join_key: Union[JoinKey, Dict]) -> Optional[JoinKey]:
 	if join_key is None:
 		return None
 	elif isinstance(join_key, JoinKey):
 		return join_key
 	else:
 		return JoinKey(**join_key)
@@ -58,21 +81,24 @@
 	sequenceKey: str = None
 	modelName: str = None
 	parentName: str = None
 	label: str = None
 	joinKeys: List[JoinKey] = []
 	dependOn: List[Dependence] = []
 	auditColumn: str = None
+	jsonColumns: List[JsonColumn] = None
 	conditions: List[Condition] = []
 	dataSourceId: str = None
 	isList: bool = False
 	triggered: bool = False
 
 	def __setattr__(self, name, value):
 		if name == 'joinKeys':
 			super().__setattr__(name, construct_join_keys(value))
 		elif name == 'dependOn':
 			super().__setattr__(name, construct_depend_on(value))
 		elif name == 'conditions':
 			super().__setattr__(name, construct_conditions(value))
+		elif name == 'jsonColumns':
+			super().__setattr__(name, construct_json_columns(value))
 		else:
 			super().__setattr__(name, value)
```

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/condition.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/condition.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/scheduled_task.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/model/scheduled_task.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/criteria_builder.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/criteria_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/data_capture.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/data_capture.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/extract_utils.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/extract_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/lock_clean.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/lock_clean.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/lock_helper.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/lock_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/task_housekeeping.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/task_housekeeping.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/task_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/task_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from logging import getLogger
 from traceback import format_exc
 from typing import Callable, Dict, Optional, List
 
 from watchmen_auth import PrincipalService
 from watchmen_collector_kernel.model import ScheduledTask
 from watchmen_collector_kernel.model.scheduled_task import Dependence
@@ -78,7 +79,14 @@
 		                                                              tenant_id)
 
 
 def get_task_service(storage: TransactionalStorageSPI,
                      snowflake_generator: SnowflakeGenerator,
                      principal_service: PrincipalService) -> TaskService:
 	return TaskService(storage, snowflake_generator, principal_service)
+
+
+# for collector prepare
+def save_json_to_local(topic_name: str, content: Dict):
+	file_path = f'{topic_name}.json'
+	with open(file_path, 'w') as f:
+		json.dump([content], f)
```

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/trigger_collector.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/service/trigger_collector.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/__init__.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_json_history_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/change_data_json_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_json_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/change_data_json_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_record_history_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/change_data_record_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_record_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/change_data_record_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/collector_model_config_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/collector_model_config_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/collector_table_config_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/collector_table_config_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 			'primary_key': config.primaryKey,
 			'object_key': config.objectKey,
 			'model_name': config.modelName,
 			'parent_name': config.parentName,
 			'join_keys': ArrayHelper(config.joinKeys).map(lambda x: x.to_dict()).to_list(),
 			'depend_on': ArrayHelper(config.dependOn).map(lambda x: x.to_dict()).to_list(),
 			'conditions': ArrayHelper(config.conditions).map(lambda x: x.to_dict()).to_list(),
+			'json_columns': ArrayHelper(config.jsonColumns).map(lambda x: x.to_dict()).to_list(),
 			'label': config.label,
 			'audit_column': config.auditColumn,
 			'data_source_id': config.dataSourceId,
 			'is_list': config.isList,
 			'triggered': config.triggered
 		})
 
@@ -39,14 +40,15 @@
 			primaryKey=row.get('primary_key'),
 			objectKey=row.get('object_key'),
 			modelName=row.get('model_name'),
 			parentName=row.get('parent_name'),
 			joinKeys=row.get('join_keys'),
 			dependOn=row.get('depend_on'),
 			conditions=row.get('conditions'),
+			jsonColumns=row.get('json_columns'),
 			label=row.get('label'),
 			auditColumn=row.get('audit_column'),
 			dataSourceId=row.get('data_source_id'),
 			isList=row.get('is_list'),
 			triggered=row.get('triggered')
 		))
 
@@ -153,15 +155,17 @@
 
 	def find_by_model_name(self,
 	                       model_name: str) -> Optional[List[CollectorTableConfig]]:
 		# noinspection PyTypeChecker
 		return self.storage.find(self.get_entity_finder(
 			criteria=[
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tenant_id'), right=self.principalService.get_tenant_id()),
-				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='model_name'), right=model_name)]
+				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='model_name'), right=model_name),
+				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='triggered'), right=True)
+			]
 		))
 
 
 def get_collector_table_config_service(storage: TransactionalStorageSPI,
                                        snowflake_generator: SnowflakeGenerator,
                                        principal_service: PrincipalService
                                        ) -> CollectorTableConfigService:
```

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/competitive_lock_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/competitive_lock_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/scheduled_task_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/scheduled_task_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_event_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/trigger_event_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_model_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/trigger_model_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_table_service.py` & `watchmen_collector_kernel-16.5.3/src/watchmen_collector_kernel/storage/trigger_table_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.2/PKG-INFO` & `watchmen_collector_kernel-16.5.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-collector-kernel
-Version: 16.5.2
+Version: 16.5.3
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
-Requires-Dist: watchmen-data-kernel (==16.5.2)
-Requires-Dist: watchmen-storage-mongodb (==16.5.2) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.2) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.2) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.2) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.2) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.2) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.2) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.5.3)
+Requires-Dist: watchmen-storage-mongodb (==16.5.3) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.3) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.3) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.3) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.3) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.3) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.3) ; extra == "s3"
```

