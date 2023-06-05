# Comparing `tmp/data_detective_airflow-2.1.1.tar.gz` & `tmp/data_detective_airflow-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_detective_airflow-2.1.1.tar", max compression
+gzip compressed data, was "data_detective_airflow-2.2.0.tar", max compression
```

## Comparing `data_detective_airflow-2.1.1.tar` & `data_detective_airflow-2.2.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1016 2023-05-19 06:47:27.214679 data_detective_airflow-2.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/__init__.py
--rw-r--r--   0        0        0     1833 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/constants.py
--rw-r--r--   0        0        0      380 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/__init__.py
--rw-r--r--   0        0        0      269 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/__init__.py
--rw-r--r--   0        0        0     1205 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/python_dag.py
--rw-r--r--   0        0        0     5798 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/tdag.py
--rw-r--r--   0        0        0     2205 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/yaml_dag.py
--rw-r--r--   0        0        0     2304 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/generator.py
--rw-r--r--   0        0        0      309 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/__init__.py
--rw-r--r--   0        0        0     2246 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/base_result.py
--rw-r--r--   0        0        0     2475 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/pg_result.py
--rw-r--r--   0        0        0     1794 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/pickle_result.py
--rw-r--r--   0        0        0      554 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/__init__.py
--rw-r--r--   0        0        0     2441 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_db_work.py
--rw-r--r--   0        0        0     2445 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_file_work.py
--rw-r--r--   0        0        0     6609 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_work.py
--rw-r--r--   0        0        0     2739 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/file_work.py
--rw-r--r--   0        0        0    10786 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/pg_work.py
--rw-r--r--   0        0        0     4127 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/s3_work.py
--rw-r--r--   0        0        0     7520 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/sftp_work.py
--rw-r--r--   0        0        0     1986 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/__init__.py
--rw-r--r--   0        0        0      591 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/__init__.py
--rw-r--r--   0        0        0      946 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/db_dump.py
--rw-r--r--   0        0        0      854 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/python_dump.py
--rw-r--r--   0        0        0     3189 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/request_dump.py
--rw-r--r--   0        0        0     2537 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/s3_dump.py
--rw-r--r--   0        0        0     3187 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/s3_list_bucket.py
--rw-r--r--   0        0        0      992 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/tsftpoperator.py
--rw-r--r--   0        0        0      261 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/__init__.py
--rw-r--r--   0        0        0     1720 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_loader.py
--rw-r--r--   0        0        0    14341 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_scd1.py
--rw-r--r--   0        0        0     6448 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_scd1_df_update_insert.py
--rw-r--r--   0        0        0     4604 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_single_target_loader.py
--rw-r--r--   0        0        0     6218 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_single_target_utils.py
--rw-r--r--   0        0        0     2782 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/s3_delete.py
--rw-r--r--   0        0        0     2782 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/s3_load.py
--rw-r--r--   0        0        0     4626 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/tbaseoperator.py
--rw-r--r--   0        0        0      287 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/__init__.py
--rw-r--r--   0        0        0     1180 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/append.py
--rw-r--r--   0        0        0     1994 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/pg_sql.py
--rw-r--r--   0        0        0     2002 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/py_transform.py
--rw-r--r--   0        0        0      781 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/__init__.py
--rw-r--r--   0        0        0     1044 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/airflow.py
--rw-r--r--   0        0        0     1570 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/assertions.py
--rw-r--r--   0        0        0     1852 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/datasets.py
--rw-r--r--   0        0        0     2552 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/generate.py
--rw-r--r--   0        0        0     3218 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/generate_df.py
--rw-r--r--   0        0        0     3488 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/test_helper.py
--rw-r--r--   0        0        0     1595 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/test_utils_petl.py
--rw-r--r--   0        0        0      933 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/utils/logging_thread.py
--rw-r--r--   0        0        0      422 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/utils/notnull.py
--rw-r--r--   0        0        0     1223 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/utils/petl_utils.py
--rw-r--r--   0        0        0     2056 2023-05-19 06:47:27.222679 data_detective_airflow-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 data_detective_airflow-2.1.1/setup.py
--rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 data_detective_airflow-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1016 2023-06-05 12:41:04.471918 data_detective_airflow-2.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 12:41:04.471918 data_detective_airflow-2.2.0/data_detective_airflow/__init__.py
+-rw-r--r--   0        0        0     1833 2023-06-05 12:41:04.471918 data_detective_airflow-2.2.0/data_detective_airflow/constants.py
+-rw-r--r--   0        0        0      380 2023-06-05 12:41:04.471918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-05 12:41:04.471918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/dags/__init__.py
+-rw-r--r--   0        0        0     1205 2023-06-05 12:41:04.471918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/dags/python_dag.py
+-rw-r--r--   0        0        0     5798 2023-06-05 12:41:04.471918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/dags/tdag.py
+-rw-r--r--   0        0        0     2205 2023-06-05 12:41:04.471918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/dags/yaml_dag.py
+-rw-r--r--   0        0        0     2304 2023-06-05 12:41:04.471918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/generator.py
+-rw-r--r--   0        0        0      309 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/results/__init__.py
+-rw-r--r--   0        0        0     2246 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/results/base_result.py
+-rw-r--r--   0        0        0     2475 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/results/pg_result.py
+-rw-r--r--   0        0        0     1794 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/results/pickle_result.py
+-rw-r--r--   0        0        0      554 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/__init__.py
+-rw-r--r--   0        0        0     2441 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/base_db_work.py
+-rw-r--r--   0        0        0     2445 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/base_file_work.py
+-rw-r--r--   0        0        0     6609 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/base_work.py
+-rw-r--r--   0        0        0     2739 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/file_work.py
+-rw-r--r--   0        0        0    10786 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/pg_work.py
+-rw-r--r--   0        0        0     4127 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/s3_work.py
+-rw-r--r--   0        0        0     7520 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/sftp_work.py
+-rw-r--r--   0        0        0     1986 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/__init__.py
+-rw-r--r--   0        0        0      591 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/__init__.py
+-rw-r--r--   0        0        0      946 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/db_dump.py
+-rw-r--r--   0        0        0      854 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/python_dump.py
+-rw-r--r--   0        0        0     3189 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/request_dump.py
+-rw-r--r--   0        0        0     2537 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/s3_dump.py
+-rw-r--r--   0        0        0     3187 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/s3_list_bucket.py
+-rw-r--r--   0        0        0      992 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/tsftpoperator.py
+-rw-r--r--   0        0        0      261 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/__init__.py
+-rw-r--r--   0        0        0     1720 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/pg_loader.py
+-rw-r--r--   0        0        0    14341 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/pg_scd1.py
+-rw-r--r--   0        0        0     6448 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/pg_scd1_df_update_insert.py
+-rw-r--r--   0        0        0     4604 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/pg_single_target_loader.py
+-rw-r--r--   0        0        0     6218 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/pg_single_target_utils.py
+-rw-r--r--   0        0        0     2782 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/s3_delete.py
+-rw-r--r--   0        0        0     2782 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/s3_load.py
+-rw-r--r--   0        0        0     4626 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/tbaseoperator.py
+-rw-r--r--   0        0        0      287 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/transformers/__init__.py
+-rw-r--r--   0        0        0     1050 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/transformers/append.py
+-rw-r--r--   0        0        0     1994 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/transformers/pg_sql.py
+-rw-r--r--   0        0        0     2002 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/operators/transformers/py_transform.py
+-rw-r--r--   0        0        0      781 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/__init__.py
+-rw-r--r--   0        0        0     1044 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/airflow.py
+-rw-r--r--   0        0        0     1570 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/assertions.py
+-rw-r--r--   0        0        0     1852 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/datasets.py
+-rw-r--r--   0        0        0     2552 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/generate.py
+-rw-r--r--   0        0        0     3218 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/generate_df.py
+-rw-r--r--   0        0        0     3488 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/test_helper.py
+-rw-r--r--   0        0        0     1595 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/test_utils_petl.py
+-rw-r--r--   0        0        0      933 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/utils/logging_thread.py
+-rw-r--r--   0        0        0      422 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/utils/notnull.py
+-rw-r--r--   0        0        0     1223 2023-06-05 12:41:04.475918 data_detective_airflow-2.2.0/data_detective_airflow/utils/petl_utils.py
+-rw-r--r--   0        0        0     2073 2023-06-05 12:41:04.479919 data_detective_airflow-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 data_detective_airflow-2.2.0/setup.py
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 data_detective_airflow-2.2.0/PKG-INFO
```

### Comparing `data_detective_airflow-2.1.1/README.md` & `data_detective_airflow-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/constants.py` & `data_detective_airflow-2.2.0/data_detective_airflow/constants.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/python_dag.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/dags/python_dag.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/tdag.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/dags/tdag.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/yaml_dag.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/dags/yaml_dag.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/generator.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/generator.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/base_result.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/results/base_result.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/pg_result.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/results/pg_result.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/pickle_result.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/results/pickle_result.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/__init__.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/__init__.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_db_work.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/base_db_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_file_work.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/base_file_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_work.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/base_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/file_work.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/file_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/pg_work.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/pg_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/s3_work.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/s3_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/sftp_work.py` & `data_detective_airflow-2.2.0/data_detective_airflow/dag_generator/works/sftp_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/__init__.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/__init__.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/db_dump.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/db_dump.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/python_dump.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/python_dump.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/request_dump.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/request_dump.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/s3_dump.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/s3_dump.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/s3_list_bucket.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/s3_list_bucket.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/tsftpoperator.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/extractors/tsftpoperator.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_loader.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/pg_loader.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_scd1.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/pg_scd1.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_scd1_df_update_insert.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/pg_scd1_df_update_insert.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_single_target_loader.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/pg_single_target_loader.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_single_target_utils.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/pg_single_target_utils.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/s3_delete.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/s3_delete.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/s3_load.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/sinks/s3_load.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/tbaseoperator.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/tbaseoperator.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/pg_sql.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/transformers/pg_sql.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/py_transform.py` & `data_detective_airflow-2.2.0/data_detective_airflow/operators/transformers/py_transform.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/__init__.py` & `data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/airflow.py` & `data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/airflow.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/assertions.py` & `data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/assertions.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/datasets.py` & `data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/datasets.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/generate.py` & `data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/generate.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/generate_df.py` & `data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/generate_df.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/test_helper.py` & `data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/test_helper.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/test_utils_petl.py` & `data_detective_airflow-2.2.0/data_detective_airflow/test_utilities/test_utils_petl.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/utils/logging_thread.py` & `data_detective_airflow-2.2.0/data_detective_airflow/utils/logging_thread.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/data_detective_airflow/utils/petl_utils.py` & `data_detective_airflow-2.2.0/data_detective_airflow/utils/petl_utils.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.1/pyproject.toml` & `data_detective_airflow-2.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "data_detective_airflow"
 license = "Apache-2.0"
-version = "2.1.1"
+version = "2.2.0"
 description = "Framework with task testing over Apache Airflow"
 authors = ["Tinkoff Data Detective Team"]
 readme = 'README.md'  # Markdown files are supported
 keywords = ["airflow testing result metadata governance catalog data detective"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -17,21 +17,22 @@
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/tinkoff/data-detective/issues"
 "Documentation" = "https://data-detective.dev/docs/data-detective-airflow/intro"
 "Repository" = "https://github.com/tinkoff/data-detective/tree/master/data-detective-airflow"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-apache-airflow = "~2.4"
+apache-airflow = "~2.6"
 apache-airflow-providers-amazon = "*"
+botocore = "^1.29.144"
 apache-airflow-providers-celery = "*"
 apache-airflow-providers-postgres = "*"
 apache-airflow-providers-redis = "*"
 apache-airflow-providers-ssh = "*"
-pandas = "^1.1, <1.6"
+pandas = "~2.0"
 petl = "^1.7"
 
 
 [tool.poetry.dev-dependencies]
 allure-pytest = "*"
 autoflake = "*"
 black = "*"
```

### Comparing `data_detective_airflow-2.1.1/setup.py` & `data_detective_airflow-2.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 
 install_requires = \
 ['apache-airflow-providers-amazon',
  'apache-airflow-providers-celery',
  'apache-airflow-providers-postgres',
  'apache-airflow-providers-redis',
  'apache-airflow-providers-ssh',
- 'apache-airflow>=2.4,<2.5',
- 'pandas>=1.1,<1.6',
+ 'apache-airflow>=2.6,<2.7',
+ 'botocore>=1.29.144,<2.0.0',
+ 'pandas>=2.0,<2.1',
  'petl>=1.7,<2.0']
 
 setup_kwargs = {
     'name': 'data-detective-airflow',
-    'version': '2.1.1',
+    'version': '2.2.0',
     'description': 'Framework with task testing over Apache Airflow',
     'long_description': '## Data Detective Airflow\n\n[Data Detective Airflow](https://github.com/tinkoff/data-detective/tree/master/data-detective-airflow) is a framework\nwhose main idea is to add the concepts of work and result to [Apache Airflow](https://airflow.apache.org/).\nIt supports tasks testing over [Apache Airflow](https://airflow.apache.org/).\nData Detective Airflow allows developers to create workflows in the form of directed acyclic graphs (DAGs) of tasks.\nThe easy-to-use Data Detective Airflow scheduler makes it possible to run tasks and save results into works. \nWork storage support for s3, ftp, local disk and database is also included.\n\n[More information about Data Detective Airflow](https://data-detective.dev/docs/data-detective-airflow/intro)\n\n## Installation\n\n#### Install from [PyPi](https://pypi.org/project/data-detective-airflow/)\n\n```bash\npip install data-detective-airflow\n```\n\nSee example DAG-s in [dags/dags](https://github.com/tinkoff/data-detective/tree/master/data-detective-airflow/dags/dags) folder.\n',
     'author': 'Tinkoff Data Detective Team',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `data_detective_airflow-2.1.1/PKG-INFO` & `data_detective_airflow-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-detective-airflow
-Version: 2.1.1
+Version: 2.2.0
 Summary: Framework with task testing over Apache Airflow
 License: Apache-2.0
 Keywords: airflow testing result metadata governance catalog data detective
 Author: Tinkoff Data Detective Team
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,21 +12,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: apache-airflow (>=2.4,<2.5)
+Requires-Dist: apache-airflow (>=2.6,<2.7)
 Requires-Dist: apache-airflow-providers-amazon
 Requires-Dist: apache-airflow-providers-celery
 Requires-Dist: apache-airflow-providers-postgres
 Requires-Dist: apache-airflow-providers-redis
 Requires-Dist: apache-airflow-providers-ssh
-Requires-Dist: pandas (>=1.1,<1.6)
+Requires-Dist: botocore (>=1.29.144,<2.0.0)
+Requires-Dist: pandas (>=2.0,<2.1)
 Requires-Dist: petl (>=1.7,<2.0)
 Project-URL: Documentation, https://data-detective.dev/docs/data-detective-airflow/intro
 Project-URL: Issue Tracker, https://github.com/tinkoff/data-detective/issues
 Project-URL: Repository, https://github.com/tinkoff/data-detective/tree/master/data-detective-airflow
 Description-Content-Type: text/markdown
 
 ## Data Detective Airflow
```

