# Comparing `tmp/watchmen_storage_rds-16.5.2.tar.gz` & `tmp/watchmen_storage_rds-16.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_rds-16.5.2.tar", max compression
+gzip compressed data, was "watchmen_storage_rds-16.5.3.tar", max compression
```

## Comparing `watchmen_storage_rds-16.5.2.tar` & `watchmen_storage_rds-16.5.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      455 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/pyproject.toml
--rw-r--r--   0        0        0      643 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/__init__.py
--rw-r--r--   0        0        0      652 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/dbscript_builder.py
--rw-r--r--   0        0        0      518 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/ext_types.py
--rw-r--r--   0        0        0      672 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/settings.py
--rw-r--r--   0        0        0      941 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/sort_build.py
--rw-r--r--   0        0        0    17290 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/storage_rds.py
--rw-r--r--   0        0        0    22699 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/table_defs.py
--rw-r--r--   0        0        0     2249 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/table_defs_helper.py
--rw-r--r--   0        0        0    22999 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/topic_data_storage_rds.py
--rw-r--r--   0        0        0     8191 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/topic_table_generate.py
--rw-r--r--   0        0        0      916 2023-05-23 07:54:10.448672 watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/types.py
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 watchmen_storage_rds-16.5.2/PKG-INFO
+-rw-r--r--   0        0        0      455 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/pyproject.toml
+-rw-r--r--   0        0        0      643 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/__init__.py
+-rw-r--r--   0        0        0      652 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/dbscript_builder.py
+-rw-r--r--   0        0        0      518 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/ext_types.py
+-rw-r--r--   0        0        0      672 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/settings.py
+-rw-r--r--   0        0        0      941 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/sort_build.py
+-rw-r--r--   0        0        0    17832 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/storage_rds.py
+-rw-r--r--   0        0        0    22728 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/table_defs.py
+-rw-r--r--   0        0        0     2249 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/table_defs_helper.py
+-rw-r--r--   0        0        0    22999 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/topic_data_storage_rds.py
+-rw-r--r--   0        0        0     8191 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/topic_table_generate.py
+-rw-r--r--   0        0        0      916 2023-06-05 01:29:03.564124 watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/types.py
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 watchmen_storage_rds-16.5.3/PKG-INFO
```

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/__init__.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/dbscript_builder.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/dbscript_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/ext_types.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/ext_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/settings.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/sort_build.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/sort_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/storage_rds.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/storage_rds.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from watchmen_model.common import DataPage
 from watchmen_storage import ask_disable_compiled_cache, ColumnNameLiteral, Entity, EntityColumnAggregateArithmetic, \
 	EntityCriteria, EntityCriteriaExpression, EntityDeleter, EntityDistinctValuesFinder, EntityFinder, EntityHelper, \
 	EntityId, EntityIdHelper, EntityList, EntityNotFoundException, EntityPager, EntitySort, \
 	EntityStraightAggregateColumn, EntityStraightColumn, EntityStraightValuesFinder, EntityUpdater, \
 	TooManyEntitiesFoundException, TransactionalStorageSPI, UnexpectedStorageException, \
-	UnsupportedStraightColumnException
+	UnsupportedStraightColumnException, EntityLimitedFinder
 from watchmen_utilities import ArrayHelper, is_blank, serialize_to_json
 from .settings import ask_connection_leak_time_in_seconds, ask_detect_connection_leak_enabled, \
 	ask_print_connection_leak_interval
 from .table_defs import find_table
 from .types import SQLAlchemyStatement, get_column_type
 
 logger = getLogger(__name__)
@@ -300,14 +300,23 @@
 		return ArrayHelper(results).map(lambda x: dict(x)).map(finder.shaper.deserialize).to_list()
 
 	def find(self, finder: EntityFinder) -> EntityList:
 		table = self.find_table(finder.name)
 		statement = select(table)
 		return self.find_on_statement_by_finder(table, statement, finder)
 
+	def find_limited(self, finder: EntityLimitedFinder) -> EntityList:
+		table = self.find_table(finder.name)
+		statement = select(table)
+		statement = self.build_criteria_for_statement([table], statement, finder.criteria)
+		statement = self.build_sort_for_statement(statement, finder.sort)
+		statement = self.build_offset_for_statement(statement, finder.limit, 1)
+		results = self.connection.execute(statement).mappings().all()
+		return ArrayHelper(results).map(lambda x: dict(x)).map(finder.shaper.deserialize).to_list()
+
 	def find_distinct_values(self, finder: EntityDistinctValuesFinder) -> EntityList:
 		table = self.find_table(finder.name)
 		if len(finder.distinctColumnNames) != 1 or not finder.distinctValueOnSingleColumn:
 			statement = select(*ArrayHelper(finder.distinctColumnNames).map(text).to_list()).select_from(table)
 		else:
 			statement = select(distinct(text(finder.distinctColumnNames[0]))).select_from(table)
 		return self.find_on_statement_by_finder(table, statement, finder)
```

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/table_defs.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/table_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
 	'collector_table_config', meta_data,
 	create_pk('config_id'), create_str('name', 50),
 	create_str('table_name', 50), create_json('primary_key'), create_str('object_key', 50),
 	create_str('model_name', 50), create_str('parent_name', 50), create_json('join_keys'),
 	create_json('conditions'), create_str('label', 50),
 	create_json('depend_on'), create_int('triggered'),
 	create_str('audit_column', 50), create_str('data_source_id', 50),
-	create_int('is_list'),
+	create_json('json_columns'), create_int('is_list'),
 	create_tenant_id(), *create_tuple_audit_columns(),
 	create_optimistic_lock()
 )
 table_trigger_event = Table(
 	'trigger_event', meta_data,
 	create_pk('event_trigger_id', Integer),
 	create_date('start_time'), create_date('end_time'),
```

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/table_defs_helper.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/table_defs_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/topic_data_storage_rds.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/topic_data_storage_rds.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/topic_table_generate.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/topic_table_generate.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.2/src/watchmen_storage_rds/types.py` & `watchmen_storage_rds-16.5.3/src/watchmen_storage_rds/types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.2/PKG-INFO` & `watchmen_storage_rds-16.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-rds
-Version: 16.5.2
+Version: 16.5.3
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (==1.4.35)
-Requires-Dist: watchmen-storage (==16.5.2)
+Requires-Dist: watchmen-storage (==16.5.3)
```

