# Comparing `tmp/databricks-feature-lookup-0.5.0.tar.gz` & `tmp/databricks-feature-lookup-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-feature-lookup-0.5.0.tar", last modified: Wed May 17 21:54:31 2023, max compression
+gzip compressed data, was "databricks-feature-lookup-0.5.1.tar", last modified: Fri Jun  2 00:29:56 2023, max compression
```

## Comparing `databricks-feature-lookup-0.5.0.tar` & `databricks-feature-lookup-0.5.1.tar`

### file list

```diff
@@ -1,84 +1,80 @@
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.681590 databricks-feature-lookup-0.5.0/
--rw-r--r--   0 avesh.singh   (502) staff       (20)     2414 2022-08-15 17:42:42.000000 databricks-feature-lookup-0.5.0/LICENSE.md
--rw-r--r--   0 avesh.singh   (502) staff       (20)      426 2022-08-15 17:42:42.000000 databricks-feature-lookup-0.5.0/NOTICE.md
--rw-r--r--   0 avesh.singh   (502) staff       (20)     4219 2023-05-17 21:54:31.681404 databricks-feature-lookup-0.5.0/PKG-INFO
--rw-r--r--   0 avesh.singh   (502) staff       (20)     3488 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/README.md
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.654343 databricks-feature-lookup-0.5.0/databricks/
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.656854 databricks-feature-lookup-0.5.0/databricks/_feature_store_pkg_metadata/
--rw-r--r--   0 avesh.singh   (502) staff       (20)      166 2022-11-08 00:41:08.000000 databricks-feature-lookup-0.5.0/databricks/_feature_store_pkg_metadata/__init__.py
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.657193 databricks-feature-lookup-0.5.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/
--rw-r--r--   0 avesh.singh   (502) staff       (20)        0 2022-11-08 00:41:08.000000 databricks-feature-lookup-0.5.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.658837 databricks-feature-lookup-0.5.0/databricks/feature_store/
--rw-r--r--   0 avesh.singh   (502) staff       (20)     1980 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/__init__.py
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.667921 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/
--rw-r--r--   0 avesh.singh   (502) staff       (20)        0 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/__init__.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     1309 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/_feature_store_object.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     1489 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/_proto_enum_entity.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      444 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/cloud.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     3039 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/column_info.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      913 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/data_type.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     2553 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_column_info.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     3971 2023-04-20 18:30:22.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_functions_for_serving.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)    19367 2023-04-26 18:25:23.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_spec.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      715 2023-03-13 18:56:02.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_spec_constants.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     1544 2023-04-26 18:25:23.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_table_info.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     4065 2023-04-26 18:25:23.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_tables_for_serving.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      673 2023-05-04 17:42:39.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/function_info.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     1978 2023-04-20 23:09:44.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/on_demand_column_info.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     6817 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/online_feature_table.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     5484 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/online_store_for_serving.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      489 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/query_mode.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      855 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/source_data_column_info.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      659 2023-05-16 17:08:40.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/store_type.py
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.668459 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/
--rw-r--r--   0 avesh.singh   (502) staff       (20)     7556 2023-05-04 17:42:39.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/feature_function_executor.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     2817 2023-04-21 16:15:58.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/feature_function_loader.py
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.669018 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/utils/
--rw-r--r--   0 avesh.singh   (502) staff       (20)        0 2023-04-21 16:15:58.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/utils/__init__.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     1855 2023-04-21 16:15:58.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/utils/codegen_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      139 2023-05-17 20:30:14.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_lookup_version.py
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.670990 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/
--rw-r--r--   0 avesh.singh   (502) staff       (20)      753 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/__init__.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     7961 2023-05-16 17:08:40.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)    21707 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      923 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_engine.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     2832 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     7533 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     2130 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)    32490 2023-05-16 17:08:40.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/mlflow_model.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     2066 2023-05-04 17:42:39.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/mlflow_model_constants.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)    10759 2023-04-23 22:18:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/online_lookup_client.py
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.671747 databricks-feature-lookup-0.5.0/databricks/feature_store/protos/
--rw-r--r--   0 avesh.singh   (502) staff       (20)        0 2022-08-15 17:42:42.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/protos/__init__.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     6396 2023-05-17 21:53:22.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/protos/feature_spec_pb2.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)    21337 2023-05-17 21:53:22.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/protos/feature_store_serving_pb2.py
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.677855 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/
--rw-r--r--   0 avesh.singh   (502) staff       (20)        0 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/__init__.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     3871 2023-04-26 02:11:21.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/converter_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     1736 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/cosmosdb_type_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      949 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/cosmosdb_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      765 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/data_type_details_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     1739 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/dynamodb_type_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     4955 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/dynamodb_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     3117 2023-05-17 18:04:44.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/feature_function_type_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      347 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/feature_serving_patch.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     2317 2023-05-04 17:42:39.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/feature_spec_test_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     2631 2023-04-11 17:04:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/metrics_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)    11740 2023-04-26 02:11:21.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/pandas_type_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     8049 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/serving_test_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     1278 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/sql_type_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      374 2023-05-05 16:47:48.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/test_utils_common.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)    10305 2023-04-20 18:30:22.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/uc_utils.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     1539 2023-04-03 22:23:57.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/utils_common.py
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.679374 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/
--rw-r--r--   0 avesh.singh   (502) staff       (20)     4219 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/PKG-INFO
--rw-r--r--   0 avesh.singh   (502) staff       (20)     3511 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/SOURCES.txt
--rw-r--r--   0 avesh.singh   (502) staff       (20)        1 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/dependency_links.txt
--rw-r--r--   0 avesh.singh   (502) staff       (20)      107 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/requires.txt
--rw-r--r--   0 avesh.singh   (502) staff       (20)       11 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/top_level.txt
--rw-r--r--   0 avesh.singh   (502) staff       (20)       38 2023-05-17 21:54:31.681653 databricks-feature-lookup-0.5.0/setup.cfg
--rw-r--r--   0 avesh.singh   (502) staff       (20)     2724 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/setup.py
-drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.680943 databricks-feature-lookup-0.5.0/tests/
--rw-r--r--   0 avesh.singh   (502) staff       (20)    88854 2023-05-16 17:08:40.000000 databricks-feature-lookup-0.5.0/tests/test_mlflow_model.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)      369 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/tests/test_mlflow_model_constants.py
--rw-r--r--   0 avesh.singh   (502) staff       (20)     8686 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/tests/test_online_lookup_client.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.701452 databricks-feature-lookup-0.5.1/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2414 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.5.1/LICENSE.md
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      426 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.5.1/NOTICE.md
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4219 2023-06-02 00:29:56.701206 databricks-feature-lookup-0.5.1/PKG-INFO
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3488 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/README.md
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.678924 databricks-feature-lookup-0.5.1/databricks/
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.681159 databricks-feature-lookup-0.5.1/databricks/_feature_store_pkg_metadata/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      166 2022-10-06 23:48:00.000000 databricks-feature-lookup-0.5.1/databricks/_feature_store_pkg_metadata/__init__.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.681487 databricks-feature-lookup-0.5.1/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-lookup-0.5.1/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.682835 databricks-feature-lookup-0.5.1/databricks/feature_store/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1980 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/__init__.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.689335 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1309 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/_feature_store_object.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1489 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/_proto_enum_entity.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      444 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/cloud.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3039 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      913 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/data_type.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2553 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3971 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_functions_for_serving.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    19367 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_spec.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      715 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_spec_constants.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1544 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_table_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4065 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_tables_for_serving.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      673 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/function_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1978 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/on_demand_column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     6817 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/online_feature_table.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     5484 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/online_store_for_serving.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      489 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/query_mode.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      855 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/source_data_column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      659 2023-05-26 16:28:51.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/store_type.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.689891 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     7556 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/feature_function_executor.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2817 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/feature_function_loader.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.690350 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/utils/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/utils/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1855 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/utils/codegen_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      139 2023-06-02 00:01:27.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_lookup_version.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.692380 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      753 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     8034 2023-05-31 17:19:14.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    21707 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      923 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2832 2023-01-13 00:17:50.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_mysql_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     7533 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_sql_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2130 2023-01-13 00:17:50.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    32490 2023-05-26 16:28:51.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/mlflow_model.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2066 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/mlflow_model_constants.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    10759 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/online_lookup_client.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.693372 databricks-feature-lookup-0.5.1/databricks/feature_store/protos/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/protos/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     6396 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/protos/feature_spec_pb2.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    21337 2023-05-26 16:28:51.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/protos/feature_store_serving_pb2.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.699525 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3871 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/converter_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1736 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/cosmosdb_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      803 2023-05-31 17:19:14.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/cosmosdb_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      765 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/data_type_details_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1739 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/dynamodb_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4955 2023-06-02 00:01:27.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/dynamodb_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3117 2023-05-26 16:28:51.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/feature_function_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      347 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/feature_serving_patch.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2317 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/feature_spec_test_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2631 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/metrics_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    11740 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/pandas_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     8049 2023-01-13 00:17:50.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/serving_test_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1278 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/sql_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      374 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/test_utils_common.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    10305 2023-04-17 17:28:49.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/uc_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1539 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/utils_common.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.700920 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4219 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/PKG-INFO
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3412 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/SOURCES.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        1 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/dependency_links.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      107 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/requires.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)       11 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/top_level.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)       38 2023-06-02 00:29:56.701519 databricks-feature-lookup-0.5.1/setup.cfg
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2724 2023-01-13 00:17:50.000000 databricks-feature-lookup-0.5.1/setup.py
```

### Comparing `databricks-feature-lookup-0.5.0/LICENSE.md` & `databricks-feature-lookup-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/PKG-INFO` & `databricks-feature-lookup-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-lookup
-Version: 0.5.0
+Version: 0.5.1
 Summary: Databricks Feature Store Feature Lookup Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `databricks-feature-lookup-0.5.0/README.md` & `databricks-feature-lookup-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/__init__.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/_feature_store_object.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/_feature_store_object.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/_proto_enum_entity.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/_proto_enum_entity.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/column_info.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/data_type.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/data_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_column_info.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_functions_for_serving.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_functions_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_spec.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_spec_constants.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_spec_constants.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_table_info.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_table_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_tables_for_serving.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_tables_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/function_info.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/function_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/on_demand_column_info.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/on_demand_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/online_feature_table.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/online_feature_table.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/online_store_for_serving.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/online_store_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/source_data_column_info.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/source_data_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/store_type.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/store_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/feature_function_executor.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/feature_function_executor.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/feature_function_loader.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/feature_function_loader.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/utils/codegen_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/utils/codegen_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/__init__.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 import functools
 import logging
 from typing import Any, List
 
 import numpy as np
 import pandas as pd
 from azure.cosmos import CosmosClient
-from azure.cosmos.exceptions import CosmosResourceNotFoundError
 
 from databricks.feature_store.entities.online_feature_table import OnlineFeatureTable
 from databricks.feature_store.entities.query_mode import QueryMode
 from databricks.feature_store.lookup_engine.lookup_engine import LookupEngine
 from databricks.feature_store.utils.cosmosdb_type_utils import (
     COSMOSDB_DATA_TYPE_CONVERTER_FACTORY,
 )
 from databricks.feature_store.utils.cosmosdb_utils import (
     FEATURE_STORE_SENTINEL_ID_VALUE,
     PARTITION_KEY,
     PATHS,
     PRIMARY_KEY_PROPERTY_NAME_VALUE,
-    is_read_item_not_found_error,
+    is_not_found_error,
     to_cosmosdb_primary_key,
 )
 from databricks.feature_store.utils.metrics_utils import (
     NAN_FEATURE_COUNT,
     LookupClientMetrics,
     lookup_call_maybe_with_metrics,
 )
@@ -106,16 +105,19 @@
 
             # As of azure-cosmos==4.2.0 (the minimum required version), `client.read_item` retries up to either of:
             # 30 seconds of timeout or 9 total attempts. Thus, no manual retry handling needs to be done.
             return self._container_client.read_item(
                 item=FEATURE_STORE_SENTINEL_ID_VALUE, partition_key=cosmosdb_primary_key
             )
         except Exception as e:
-            # Return None if the error was caused by read_item finding no result. Otherwise, re-raise the error.
-            if is_read_item_not_found_error(e):
+            # Return None if the error was caused by read_item finding no result. Otherwise,
+            # re-raise the error.
+            # The existence of the CosmosDB container is validated during __init__, so any NotFound
+            # is caused by a missing item.
+            if is_not_found_error(e):
                 return None
             _logger.warning(
                 f"Encountered error reading from {self.online_table_name}:\n{e}"
             )
             raise e
 
     def _run_lookup_cosmosdb_query(
```

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_engine.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_mysql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_sql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/mlflow_model.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/mlflow_model.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/mlflow_model_constants.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/mlflow_model_constants.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/online_lookup_client.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/online_lookup_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/protos/feature_spec_pb2.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/protos/feature_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/protos/feature_store_serving_pb2.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/protos/feature_store_serving_pb2.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/converter_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/converter_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/cosmosdb_type_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/cosmosdb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/data_type_details_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/data_type_details_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/dynamodb_type_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/dynamodb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/dynamodb_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/dynamodb_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/feature_function_type_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/feature_function_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/feature_spec_test_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/feature_spec_test_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/metrics_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/pandas_type_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/pandas_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/serving_test_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/serving_test_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/sql_type_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/sql_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/uc_utils.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/uc_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/utils_common.py` & `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/utils_common.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/PKG-INFO` & `databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-lookup
-Version: 0.5.0
+Version: 0.5.1
 Summary: Databricks Feature Store Feature Lookup Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/SOURCES.txt` & `databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,11 +59,8 @@
 databricks/feature_store/utils/test_utils_common.py
 databricks/feature_store/utils/uc_utils.py
 databricks/feature_store/utils/utils_common.py
 databricks_feature_lookup.egg-info/PKG-INFO
 databricks_feature_lookup.egg-info/SOURCES.txt
 databricks_feature_lookup.egg-info/dependency_links.txt
 databricks_feature_lookup.egg-info/requires.txt
-databricks_feature_lookup.egg-info/top_level.txt
-tests/test_mlflow_model.py
-tests/test_mlflow_model_constants.py
-tests/test_online_lookup_client.py
+databricks_feature_lookup.egg-info/top_level.txt
```

### Comparing `databricks-feature-lookup-0.5.0/setup.py` & `databricks-feature-lookup-0.5.1/setup.py`

 * *Files identical despite different names*

