# Comparing `tmp/watchmen_storage-16.5.2.tar.gz` & `tmp/watchmen_storage-16.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage-16.5.2.tar", max compression
+gzip compressed data, was "watchmen_storage-16.5.3.tar", max compression
```

## Comparing `watchmen_storage-16.5.2.tar` & `watchmen_storage-16.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/LICENSE
--rw-r--r--   0        0        0      492 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/pyproject.toml
--rw-r--r--   0        0        0     2196 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/__init__.py
--rw-r--r--   0        0        0     4917 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/competitive_worker_id_generator.py
--rw-r--r--   0        0        0     5549 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/data_source_helper.py
--rw-r--r--   0        0        0     1819 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/free_storage_types.py
--rw-r--r--   0        0        0      211 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/secrets_manager.py
--rw-r--r--   0        0        0      730 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/secrets_manager_aws.py
--rw-r--r--   0        0        0     1096 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/settings.py
--rw-r--r--   0        0        0     2750 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/snowflake.py
--rw-r--r--   0        0        0      232 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/snowflake_worker_id_generator.py
--rw-r--r--   0        0        0        0 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/__init__.py
--rw-r--r--   0        0        0    10150 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/ast_vister.py
--rw-r--r--   0        0        0     2632 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/parse_sql.py
--rw-r--r--   0        0        0      890 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/query_performance_service.py
--rw-r--r--   0        0        0     1441 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/topic_generator.py
--rw-r--r--   0        0        0     7259 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/storage_based_worker_id_generator.py
--rw-r--r--   0        0        0      721 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/storage_exception.py
--rw-r--r--   0        0        0     5884 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/storage_spi.py
--rw-r--r--   0        0        0     4645 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/storage_types.py
--rw-r--r--   0        0        0      630 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/topic_utils.py
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 watchmen_storage-16.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/LICENSE
+-rw-r--r--   0        0        0      492 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/__init__.py
+-rw-r--r--   0        0        0     4917 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/competitive_worker_id_generator.py
+-rw-r--r--   0        0        0     5549 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/data_source_helper.py
+-rw-r--r--   0        0        0     1819 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/free_storage_types.py
+-rw-r--r--   0        0        0      211 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/secrets_manager.py
+-rw-r--r--   0        0        0      730 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/secrets_manager_aws.py
+-rw-r--r--   0        0        0     1096 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/settings.py
+-rw-r--r--   0        0        0     2750 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/snowflake.py
+-rw-r--r--   0        0        0      232 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/snowflake_worker_id_generator.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/__init__.py
+-rw-r--r--   0        0        0    10150 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/ast_vister.py
+-rw-r--r--   0        0        0     2632 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/parse_sql.py
+-rw-r--r--   0        0        0      890 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/query_performance_service.py
+-rw-r--r--   0        0        0     1441 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/topic_generator.py
+-rw-r--r--   0        0        0     7259 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/storage_based_worker_id_generator.py
+-rw-r--r--   0        0        0      721 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/storage_exception.py
+-rw-r--r--   0        0        0     5998 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/storage_spi.py
+-rw-r--r--   0        0        0     4717 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/storage_types.py
+-rw-r--r--   0        0        0      630 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/topic_utils.py
+-rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 watchmen_storage-16.5.3/PKG-INFO
```

### Comparing `watchmen_storage-16.5.2/LICENSE` & `watchmen_storage-16.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/__init__.py` & `watchmen_storage-16.5.3/src/watchmen_storage/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 from .storage_spi import StorageSPI, TopicDataStorageSPI, TransactionalStorageSPI
 from .storage_types import ColumnNameLiteral, ComputedLiteral, ComputedLiteralOperator, Entity, \
 	EntityColumnAggregateArithmetic, EntityColumnName, EntityColumnValue, EntityCriteria, EntityCriteriaExpression, \
 	EntityCriteriaJoint, EntityCriteriaJointConjunction, EntityCriteriaOperator, EntityCriteriaStatement, \
 	EntityDeleter, EntityDistinctValuesFinder, EntityFinder, EntityHelper, EntityId, EntityIdHelper, EntityList, \
 	EntityName, EntityPager, EntityRow, EntityShaper, EntitySort, EntitySortColumn, EntitySortMethod, \
 	EntityStraightAggregateColumn, EntityStraightColumn, EntityStraightValuesFinder, EntityUpdate, EntityUpdater, \
-	Literal, EntityColumnType
+	Literal, EntityColumnType, EntityLimitedFinder
 from .topic_utils import as_table_name
```

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/competitive_worker_id_generator.py` & `watchmen_storage-16.5.3/src/watchmen_storage/competitive_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/data_source_helper.py` & `watchmen_storage-16.5.3/src/watchmen_storage/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/free_storage_types.py` & `watchmen_storage-16.5.3/src/watchmen_storage/free_storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/secrets_manager_aws.py` & `watchmen_storage-16.5.3/src/watchmen_storage/secrets_manager_aws.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/settings.py` & `watchmen_storage-16.5.3/src/watchmen_storage/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/snowflake.py` & `watchmen_storage-16.5.3/src/watchmen_storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/ast_vister.py` & `watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/ast_vister.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/parse_sql.py` & `watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/parse_sql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/query_performance_service.py` & `watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/query_performance_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/topic_generator.py` & `watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/topic_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/storage_based_worker_id_generator.py` & `watchmen_storage-16.5.3/src/watchmen_storage/storage_based_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/storage_exception.py` & `watchmen_storage-16.5.3/src/watchmen_storage/storage_exception.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/storage_spi.py` & `watchmen_storage-16.5.3/src/watchmen_storage/storage_spi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional
 
 from watchmen_model.admin import Factor, Topic
 from watchmen_model.common import DataPage
 from .free_storage_types import FreeAggregatePager, FreeAggregator, FreeFinder, FreePager
 from .storage_types import Entity, EntityDeleter, EntityDistinctValuesFinder, EntityFinder, EntityHelper, EntityId, \
-	EntityIdHelper, EntityList, EntityPager, EntityStraightValuesFinder, EntityUpdater
+	EntityIdHelper, EntityList, EntityPager, EntityStraightValuesFinder, EntityUpdater, EntityLimitedFinder
 
 
 class StorageSPI(ABC):
 	@abstractmethod
 	def connect(self) -> None:
 		"""
 		connect when not connected, or do nothing if connected.
@@ -110,14 +110,18 @@
 		pass
 
 	@abstractmethod
 	def find(self, finder: EntityFinder) -> EntityList:
 		pass
 
 	@abstractmethod
+	def find_limited(self, finder: EntityLimitedFinder) -> EntityList:
+		pass
+
+	@abstractmethod
 	def find_distinct_values(self, finder: EntityDistinctValuesFinder) -> EntityList:
 		"""
 		filled values with given distinct columns, returns an entity list.
 		entity is deserialized by shaper
 		"""
 		pass
```

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/storage_types.py` & `watchmen_storage-16.5.3/src/watchmen_storage/storage_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,18 @@
 
 
 class EntityFinder(EntityHelper):
 	criteria: Optional[EntityCriteria] = None
 	sort: Optional[EntitySort] = None
 
 
+class EntityLimitedFinder(EntityFinder):
+	limit: Optional[int] = None
+
+
 class EntityDistinctValuesFinder(EntityFinder):
 	distinctColumnNames: List[EntityColumnName] = None
 	distinctValueOnSingleColumn: bool = False  # distinct value when it is True and only one column assigned
 
 
 class EntityColumnType(str, Enum):
 	INTEGER = 'integer',
```

### Comparing `watchmen_storage-16.5.2/src/watchmen_storage/topic_utils.py` & `watchmen_storage-16.5.3/src/watchmen_storage/topic_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.2/PKG-INFO` & `watchmen_storage-16.5.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage
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
 Requires-Dist: boto3 (>=1.24.20,<2.0.0)
 Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
-Requires-Dist: watchmen-model (==16.5.2)
+Requires-Dist: watchmen-model (==16.5.3)
```

