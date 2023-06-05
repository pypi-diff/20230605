# Comparing `tmp/google_fhir_views-0.9.2-py3-none-any.whl.zip` & `tmp/google_fhir_views-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,84 @@
-Zip file size: 49227 bytes, number of entries: 16
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/views/__init__.py
--rw-r--r--  2.0 unx     8279 b- defN 23-Apr-17 20:06 google/fhir/views/_views_test_base.py
--rw-r--r--  2.0 unx    19442 b- defN 23-Apr-17 20:06 google/fhir/views/bigquery_runner.py
--rw-r--r--  2.0 unx    47444 b- defN 23-Apr-17 20:06 google/fhir/views/bigquery_runner_test.py
--rw-r--r--  2.0 unx    47288 b- defN 23-Apr-17 20:06 google/fhir/views/bigquery_runner_test_v2.py
--rw-r--r--  2.0 unx     2536 b- defN 23-Apr-17 20:06 google/fhir/views/r4.py
--rw-r--r--  2.0 unx      906 b- defN 23-Apr-17 20:06 google/fhir/views/r4_test.py
--rw-r--r--  2.0 unx    15637 b- defN 23-Apr-17 20:06 google/fhir/views/runner_utils.py
--rw-r--r--  2.0 unx    14785 b- defN 23-Apr-17 20:06 google/fhir/views/runner_utils_test.py
--rw-r--r--  2.0 unx     9278 b- defN 23-Apr-17 20:06 google/fhir/views/spark_runner.py
--rw-r--r--  2.0 unx    14043 b- defN 23-Apr-17 20:06 google/fhir/views/spark_runner_test.py
--rw-r--r--  2.0 unx    13469 b- defN 23-Apr-17 20:06 google/fhir/views/views.py
--rw-r--r--  2.0 unx    11666 b- defN 23-Apr-17 20:08 google_fhir_views-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 20:08 google_fhir_views-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-17 20:08 google_fhir_views-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1433 b- defN 23-Apr-17 20:08 google_fhir_views-0.9.2.dist-info/RECORD
-16 files, 206882 bytes uncompressed, 46841 bytes compressed:  77.4%
+Zip file size: 264042 bytes, number of entries: 82
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/views/__init__.py
+-rw-r--r--  2.0 unx     8279 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/views/_views_test_base.py
+-rw-r--r--  2.0 unx    17058 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner.py
+-rw-r--r--  2.0 unx    42114 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner_test.py
+-rw-r--r--  2.0 unx    42637 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner_test_v2.py
+-rw-r--r--  2.0 unx     8420 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/views/bigquery_value_set_manager.py
+-rw-r--r--  2.0 unx     9921 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/views/bigquery_value_set_manager_test.py
+-rw-r--r--  2.0 unx     2536 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/views/r4.py
+-rw-r--r--  2.0 unx      906 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/views/r4_test.py
+-rw-r--r--  2.0 unx    15637 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/views/runner_utils.py
+-rw-r--r--  2.0 unx    14785 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/views/runner_utils_test.py
+-rw-r--r--  2.0 unx     9330 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/views/spark_runner.py
+-rw-r--r--  2.0 unx    14043 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/views/spark_runner_test.py
+-rw-r--r--  2.0 unx    13469 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/views/views.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/views/__init__.py
+-rw-r--r--  2.0 unx     8279 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/views/_views_test_base.py
+-rw-r--r--  2.0 unx    17058 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner.py
+-rw-r--r--  2.0 unx    42114 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner_test.py
+-rw-r--r--  2.0 unx    42637 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner_test_v2.py
+-rw-r--r--  2.0 unx     8420 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/views/bigquery_value_set_manager.py
+-rw-r--r--  2.0 unx     9921 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/views/bigquery_value_set_manager_test.py
+-rw-r--r--  2.0 unx     2536 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/views/r4.py
+-rw-r--r--  2.0 unx      906 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/views/r4_test.py
+-rw-r--r--  2.0 unx    15637 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/views/runner_utils.py
+-rw-r--r--  2.0 unx    14785 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/views/runner_utils_test.py
+-rw-r--r--  2.0 unx    13356 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/views/spark_runner.py
+-rw-r--r--  2.0 unx    18117 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/views/spark_runner_test.py
+-rw-r--r--  2.0 unx     7318 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/views/spark_value_set_manager.py
+-rw-r--r--  2.0 unx     7421 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/views/spark_value_set_manager_test.py
+-rw-r--r--  2.0 unx    13469 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/views/views.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/views/__init__.py
+-rw-r--r--  2.0 unx     8279 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/views/_views_test_base.py
+-rw-r--r--  2.0 unx    17058 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/views/bigquery_runner.py
+-rw-r--r--  2.0 unx    42114 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/views/bigquery_runner_test.py
+-rw-r--r--  2.0 unx    42637 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/views/bigquery_runner_test_v2.py
+-rw-r--r--  2.0 unx     8420 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/views/bigquery_value_set_manager.py
+-rw-r--r--  2.0 unx     9921 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/views/bigquery_value_set_manager_test.py
+-rw-r--r--  2.0 unx     2536 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/views/r4.py
+-rw-r--r--  2.0 unx      906 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/views/r4_test.py
+-rw-r--r--  2.0 unx    15637 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/views/runner_utils.py
+-rw-r--r--  2.0 unx    14785 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/views/runner_utils_test.py
+-rw-r--r--  2.0 unx    13356 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/views/spark_runner.py
+-rw-r--r--  2.0 unx    18117 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/views/spark_runner_test.py
+-rw-r--r--  2.0 unx     7318 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/views/spark_value_set_manager.py
+-rw-r--r--  2.0 unx     7421 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/views/spark_value_set_manager_test.py
+-rw-r--r--  2.0 unx    13469 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/views/views.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/views/__init__.py
+-rw-r--r--  2.0 unx     8279 b- defN 23-May-18 18:49 build/lib/google/fhir/views/_views_test_base.py
+-rw-r--r--  2.0 unx    17058 b- defN 23-May-18 18:51 build/lib/google/fhir/views/bigquery_runner.py
+-rw-r--r--  2.0 unx    42114 b- defN 23-May-18 18:51 build/lib/google/fhir/views/bigquery_runner_test.py
+-rw-r--r--  2.0 unx    42637 b- defN 23-May-18 18:51 build/lib/google/fhir/views/bigquery_runner_test_v2.py
+-rw-r--r--  2.0 unx     8420 b- defN 23-May-18 18:51 build/lib/google/fhir/views/bigquery_value_set_manager.py
+-rw-r--r--  2.0 unx     9921 b- defN 23-May-18 18:51 build/lib/google/fhir/views/bigquery_value_set_manager_test.py
+-rw-r--r--  2.0 unx     2536 b- defN 23-May-18 18:49 build/lib/google/fhir/views/r4.py
+-rw-r--r--  2.0 unx      906 b- defN 23-May-18 18:49 build/lib/google/fhir/views/r4_test.py
+-rw-r--r--  2.0 unx    15637 b- defN 23-May-18 18:51 build/lib/google/fhir/views/runner_utils.py
+-rw-r--r--  2.0 unx    14785 b- defN 23-May-18 18:51 build/lib/google/fhir/views/runner_utils_test.py
+-rw-r--r--  2.0 unx    13356 b- defN 23-Jun-05 20:08 build/lib/google/fhir/views/spark_runner.py
+-rw-r--r--  2.0 unx    18117 b- defN 23-Jun-05 20:08 build/lib/google/fhir/views/spark_runner_test.py
+-rw-r--r--  2.0 unx     7318 b- defN 23-Jun-05 20:08 build/lib/google/fhir/views/spark_value_set_manager.py
+-rw-r--r--  2.0 unx     7421 b- defN 23-Jun-05 20:08 build/lib/google/fhir/views/spark_value_set_manager_test.py
+-rw-r--r--  2.0 unx    13469 b- defN 23-May-18 18:51 build/lib/google/fhir/views/views.py
+-rw-r-----  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/views/__init__.py
+-rw-r-----  2.0 unx     8279 b- defN 23-May-18 18:49 google/fhir/views/_views_test_base.py
+-rw-r-----  2.0 unx    17058 b- defN 23-May-18 18:51 google/fhir/views/bigquery_runner.py
+-rw-r-----  2.0 unx    42114 b- defN 23-May-18 18:51 google/fhir/views/bigquery_runner_test.py
+-rw-r-----  2.0 unx    42637 b- defN 23-May-18 18:51 google/fhir/views/bigquery_runner_test_v2.py
+-rw-r-----  2.0 unx     8420 b- defN 23-May-18 18:51 google/fhir/views/bigquery_value_set_manager.py
+-rw-r-----  2.0 unx     9921 b- defN 23-May-18 18:51 google/fhir/views/bigquery_value_set_manager_test.py
+-rw-r-----  2.0 unx     2536 b- defN 23-May-18 18:49 google/fhir/views/r4.py
+-rw-r-----  2.0 unx      906 b- defN 23-May-18 18:49 google/fhir/views/r4_test.py
+-rw-r-----  2.0 unx    15637 b- defN 23-May-18 18:51 google/fhir/views/runner_utils.py
+-rw-r-----  2.0 unx    14785 b- defN 23-May-18 18:51 google/fhir/views/runner_utils_test.py
+-rw-r--r--  2.0 unx    13356 b- defN 23-Jun-05 20:08 google/fhir/views/spark_runner.py
+-rw-r--r--  2.0 unx    18117 b- defN 23-Jun-05 20:08 google/fhir/views/spark_runner_test.py
+-rw-r--r--  2.0 unx     7318 b- defN 23-Jun-05 20:08 google/fhir/views/spark_value_set_manager.py
+-rw-r--r--  2.0 unx     7421 b- defN 23-Jun-05 20:08 google/fhir/views/spark_value_set_manager_test.py
+-rw-r-----  2.0 unx    13469 b- defN 23-May-18 18:51 google/fhir/views/views.py
+-rw-r--r--  2.0 unx    11839 b- defN 23-Jun-05 20:35 google_fhir_views-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 20:35 google_fhir_views-0.9.3.dist-info/WHEEL
+-rw-r-----  2.0 unx       13 b- defN 23-Jun-05 20:35 google_fhir_views-0.9.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9231 b- defN 23-Jun-05 20:35 google_fhir_views-0.9.3.dist-info/RECORD
+82 files, 1111091 bytes uncompressed, 248618 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -1,7 +1,193 @@
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/_views_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner_test_v2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/bigquery_value_set_manager.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/bigquery_value_set_manager_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/r4.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/r4_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/runner_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/runner_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/spark_runner.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/spark_runner_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/views/views.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/_views_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/bigquery_runner_test_v2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/bigquery_value_set_manager.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/bigquery_value_set_manager_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/r4.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/r4_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/runner_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/runner_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/spark_runner.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/spark_runner_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/spark_value_set_manager.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/spark_value_set_manager_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/views/views.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/_views_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/bigquery_runner.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/bigquery_runner_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/bigquery_runner_test_v2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/bigquery_value_set_manager.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/bigquery_value_set_manager_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/r4.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/r4_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/runner_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/runner_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/spark_runner.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/spark_runner_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/spark_value_set_manager.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/spark_value_set_manager_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/views/views.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/_views_test_base.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/bigquery_runner.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/bigquery_runner_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/bigquery_runner_test_v2.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/bigquery_value_set_manager.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/bigquery_value_set_manager_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/r4.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/r4_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/runner_utils.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/runner_utils_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/spark_runner.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/spark_runner_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/spark_value_set_manager.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/spark_value_set_manager_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/views/views.py
+Comment: 
+
 Filename: google/fhir/views/__init__.py
 Comment: 
 
 Filename: google/fhir/views/_views_test_base.py
 Comment: 
 
 Filename: google/fhir/views/bigquery_runner.py
@@ -9,14 +195,20 @@
 
 Filename: google/fhir/views/bigquery_runner_test.py
 Comment: 
 
 Filename: google/fhir/views/bigquery_runner_test_v2.py
 Comment: 
 
+Filename: google/fhir/views/bigquery_value_set_manager.py
+Comment: 
+
+Filename: google/fhir/views/bigquery_value_set_manager_test.py
+Comment: 
+
 Filename: google/fhir/views/r4.py
 Comment: 
 
 Filename: google/fhir/views/r4_test.py
 Comment: 
 
 Filename: google/fhir/views/runner_utils.py
@@ -27,23 +219,29 @@
 
 Filename: google/fhir/views/spark_runner.py
 Comment: 
 
 Filename: google/fhir/views/spark_runner_test.py
 Comment: 
 
+Filename: google/fhir/views/spark_value_set_manager.py
+Comment: 
+
+Filename: google/fhir/views/spark_value_set_manager_test.py
+Comment: 
+
 Filename: google/fhir/views/views.py
 Comment: 
 
-Filename: google_fhir_views-0.9.2.dist-info/METADATA
+Filename: google_fhir_views-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: google_fhir_views-0.9.2.dist-info/WHEEL
+Filename: google_fhir_views-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: google_fhir_views-0.9.2.dist-info/top_level.txt
+Filename: google_fhir_views-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: google_fhir_views-0.9.2.dist-info/RECORD
+Filename: google_fhir_views-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## google/fhir/views/bigquery_runner.py

```diff
@@ -20,25 +20,23 @@
 """
 
 import re
 from typing import Iterable, Optional, Union, cast, Dict
 
 from google.cloud import bigquery
 import pandas
-import sqlalchemy
-import sqlalchemy_bigquery
 
 from google.fhir.r4.proto.core.resources import value_set_pb2
 from google.fhir.core.fhir_path import _bigquery_interpreter
 from google.fhir.core.fhir_path import _fhir_path_data_types
 from google.fhir.core.fhir_path import expressions
 from google.fhir.core.fhir_path import fhir_path
 from google.fhir.r4.terminology import terminology_service_client
-from google.fhir.r4.terminology import value_set_tables
 from google.fhir.r4.terminology import value_sets
+from google.fhir.views import bigquery_value_set_manager
 from google.fhir.views import runner_utils
 from google.fhir.views import views
 
 
 class BigQueryRunner:
   """FHIR Views runner used to perform queries against BigQuery."""
 
@@ -119,14 +117,20 @@
     elif isinstance(value_set_codes_table, str):
       self._value_set_codes_table = bigquery.table.TableReference.from_string(
           value_set_codes_table, default_project=client.project
       )
     else:
       self._value_set_codes_table = value_set_codes_table
 
+    self._value_set_manager = (
+        bigquery_value_set_manager.BigQueryValueSetManager(
+            client, self._value_set_codes_table
+        )
+    )
+
   def _view_table_names(self, view: views.View) -> Dict[str, str]:
     """Generates the table names for each resource in the view."""
     names = {}
     for structdef_url in view.get_structdef_urls():
       last_slash_index = structdef_url.rfind('/')
       name = (
           structdef_url
@@ -317,36 +321,14 @@
       raise ValueError(
           'Field must be a FHIR CodeableConcept, Coding, or Code; '
           f'got {node_type.url}.'
       )
 
     return self._client.query(count_query).result().to_dataframe()
 
-  def _create_valueset_codes_table_if_not_exists(self) -> bigquery.table.Table:
-    """Creates a table for storing value set code mappings.
-
-    Creates a table named after the `value_set_codes_table` provided at class
-    initialization as described by
-    https://github.com/FHIR/sql-on-fhir/blob/master/sql-on-fhir.md#valueset-support
-
-    If the table already exists, no action is taken.
-
-    Returns:
-      An bigquery.Table object representing the created table.
-    """
-    schema = [
-        bigquery.SchemaField('valueseturi', 'STRING', mode='REQUIRED'),
-        bigquery.SchemaField('valuesetversion', 'STRING', mode='NULLABLE'),
-        bigquery.SchemaField('system', 'STRING', mode='REQUIRED'),
-        bigquery.SchemaField('code', 'STRING', mode='REQUIRED'),
-    ]
-    table = bigquery.Table(self._value_set_codes_table, schema=schema)
-    table.clustering_fields = ['valueseturi', 'code']
-    return self._client.create_table(table, exists_ok=True)
-
   def _build_sql_generator(self, internal_v2: bool, view: views.View):
     """Build a RunnerSqlGenerator depending on the runner version."""
     fhir_context = view.get_fhir_path_context()
     url = list(view.get_structdef_urls())[0]
     struct_def = fhir_context.get_structure_definition(url)
     deps = fhir_context.get_dependency_definitions(url)
     deps.append(struct_def)
@@ -390,30 +372,15 @@
     `materialize_value_set_expansion` below to retrieve an expanded set from
     a terminology server.
 
     Args:
       value_set_protos: An iterable of FHIR ValueSet protos.
       batch_size: The maximum number of rows to insert in a single query.
     """
-    bq_table = self._create_valueset_codes_table_if_not_exists()
-
-    sa_table = _bq_table_to_sqlalchemy_table(bq_table)
-    queries = value_set_tables.valueset_codes_insert_statement_for(
-        value_set_protos, sa_table, batch_size=batch_size
-    )
-
-    # Render the query objects as strings and use the client to execute them.
-    for query in queries:
-      query_string = str(
-          query.compile(
-              dialect=(sqlalchemy_bigquery.BigQueryDialect()),
-              compile_kwargs={'literal_binds': True},
-          )
-      )
-      self._client.query(query_string).result()
+    self._value_set_manager.materialize_value_sets(value_set_protos, batch_size)
 
   def materialize_value_set_expansion(
       self,
       urls: Iterable[str],
       expander: Union[
           terminology_service_client.TerminologyServiceClient,
           value_sets.ValueSetResolver,
@@ -454,37 +421,10 @@
         service to use for each value set URL based on its domain.
       batch_size: The maximum number of rows to insert in a single query.
 
     Raises:
       TypeError: If a `terminology_service_url` is given but `expander` is not a
       TerminologyServiceClient.
     """
-    if terminology_service_url is not None and not isinstance(
-        expander, terminology_service_client.TerminologyServiceClient
-    ):
-      raise TypeError(
-          '`terminology_service_url` can only be given if `expander` is a '
-          'TerminologyServiceClient'
-      )
-
-    if terminology_service_url is not None and isinstance(
-        expander, terminology_service_client.TerminologyServiceClient
-    ):
-      expanded_value_sets = (
-          expander.expand_value_set_url_using_service(
-              url, terminology_service_url
-          )
-          for url in urls
-      )
-    else:
-      expanded_value_sets = (expander.expand_value_set_url(url) for url in urls)
-
-    self.materialize_value_sets(expanded_value_sets, batch_size=batch_size)
-
-
-def _bq_table_to_sqlalchemy_table(
-    bq_table: bigquery.table.Table,
-) -> sqlalchemy.sql.selectable.TableClause:
-  """Converts a BigQuery client Table to an sqlalchemy Table."""
-  table_name = f'{bq_table.project}.{bq_table.dataset_id}.{bq_table.table_id}'
-  columns = [sqlalchemy.column(column.name) for column in bq_table.schema]
-  return sqlalchemy.table(table_name, *columns)
+    self._value_set_manager.materialize_value_set_expansion(
+        urls, expander, terminology_service_url, batch_size
+    )
```

## google/fhir/views/bigquery_runner_test.py

```diff
@@ -23,17 +23,16 @@
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from google.fhir.r4.proto.core.resources import value_set_pb2
 from google.fhir.core.fhir_path import context
 from google.fhir.core.utils import fhir_package
 from google.fhir.r4 import r4_package
-from google.fhir.r4.terminology import terminology_service_client
-from google.fhir.r4.terminology import value_sets
 from google.fhir.views import bigquery_runner
+from google.fhir.views import bigquery_value_set_manager
 from google.fhir.views import r4
 from google.fhir.views import views
 
 
 class BigqueryRunnerTest(parameterized.TestCase):
   _fhir_package: fhir_package.FhirPackage
 
@@ -116,14 +115,16 @@
   ):
     runner = bigquery_runner.BigQueryRunner(
         self.mock_bigquery_client,
         'test_dataset',
         value_set_codes_table=value_set_codes_table,
     )
     self.assertEqual(runner._value_set_codes_table, expected_table_name)
+    self.assertEqual(runner._value_set_manager.value_set_codes_table,  # pylint: disable=protected-access
+                     expected_table_name)
 
   def testNestedSingleFieldInNestedArray_forPatient_returnsArray(self):
     pat = self._views.view_of('Patient')
     simple_view = pat.select({
         'family_names': pat.name.family,
     })
 
@@ -761,168 +762,47 @@
         'COUNT(*) count FROM c, UNNEST(c.target) codings '
         'GROUP BY 1, 2, 3 ORDER BY count DESC'
     )
     self.mock_bigquery_client.query.assert_called_once_with(expected_sql)
     self.assertEqual(expected_mock_df, returned_df)
 
   @mock.patch.object(
-      bigquery_runner.value_set_tables,
-      'valueset_codes_insert_statement_for',
+      bigquery_value_set_manager.BigQueryValueSetManager,
+      'materialize_value_sets',
       autospec=True,
   )
-  def testMaterializeValueSet_withValueSetObject_insertsData(
-      self, mock_valueset_codes_insert_statement_for
+  def testMaterializeValueSet_delegatesToManager(
+      self, mock_materialize_value_sets
   ):
+    """Tests inserting data through mock call."""
     mock_value_sets = [mock.MagicMock(), mock.MagicMock()]
-    mock_insert_statements = [mock.MagicMock(), mock.MagicMock()]
-    mock_valueset_codes_insert_statement_for.return_value = (
-        mock_insert_statements
-    )
-    self.mock_bigquery_client.create_table.return_value = _BqValuesetCodesTable(
-        'vs_project.vs_dataset.vs_table'
-    )
-
-    self.runner.materialize_value_sets(mock_value_sets)
-
-    # Ensure we tried to create the table
-    self.mock_bigquery_client.create_table.assert_called_once()
-
-    # Ensure we called query with the rendered SQL for the two mock queries and
-    # called .result() on the returned job.
-    self.mock_bigquery_client.query.assert_has_calls([
-        mock.call(str(mock_insert_statements[0].compile())),
-        mock.call().result(),
-        mock.call(str(mock_insert_statements[1].compile())),
-        mock.call().result(),
-    ])
-
-    # Ensure we called valueset_codes_insert_statement_for with the
-    # given value sets.
-    args, kwargs = mock_valueset_codes_insert_statement_for.call_args_list[0]
-    expanded_value_sets, table = args
-    self.assertEqual(list(expanded_value_sets), mock_value_sets)
-
-    self.assertEqual(table.name, 'vs_project.vs_dataset.vs_table')
-    for col in ('valueseturi', 'valuesetversion', 'system', 'code'):
-      self.assertIn(col, table.columns)
-    self.assertEqual(kwargs['batch_size'], 500)
 
-  @mock.patch.object(
-      bigquery_runner.value_set_tables,
-      'valueset_codes_insert_statement_for',
-      autospec=True,
-  )
-  def testMaterializeValueSetExpansion_withValueSetUrls_performsExpansionsAndInserts(
-      self, mock_valueset_codes_insert_statement_for
-  ):
-    mock_insert_statements = [mock.MagicMock(), mock.MagicMock()]
-    mock_valueset_codes_insert_statement_for.return_value = (
-        mock_insert_statements
-    )
-    mock_expander = mock.MagicMock()
-    self.mock_bigquery_client.create_table.return_value = _BqValuesetCodesTable(
-        'vs_project.vs_dataset.vs_table'
-    )
-
-    self.runner.materialize_value_set_expansion(
-        ['url-1', 'url-2'], mock_expander
-    )
+    self.runner.materialize_value_sets(mock_value_sets, 100)
 
-    # Ensure we tried to create the table
-    self.mock_bigquery_client.create_table.assert_called_once()
-
-    # Ensure we called query with the rendered SQL for the two mock queries and
-    # called .result() on the returned job.
-    self.mock_bigquery_client.query.assert_has_calls([
-        mock.call(str(mock_insert_statements[0].compile())),
-        mock.call().result(),
-        mock.call(str(mock_insert_statements[1].compile())),
-        mock.call().result(),
-    ])
-    # Ensure we called valueset_codes_insert_statement_for with the value set
-    # expansions for both URLs and with an appropriate table object.
-    args, kwargs = mock_valueset_codes_insert_statement_for.call_args_list[0]
-    expanded_value_sets, table = args
-    self.assertEqual(
-        list(expanded_value_sets),
-        [
-            mock_expander.expand_value_set_url(),
-            mock_expander.expand_value_set_url(),
-        ],
-    )
-    self.assertEqual(table.name, 'vs_project.vs_dataset.vs_table')
-    for col in ('valueseturi', 'valuesetversion', 'system', 'code'):
-      self.assertIn(col, table.columns)
-    self.assertEqual(kwargs['batch_size'], 500)
-
-    # Ensure we call expand_value_set_url with the two URLs.
-    mock_expander.expand_value_set_url.reset()
-    mock_expander.expand_value_set_url.assert_has_calls(
-        [mock.call('url-1'), mock.call('url-2')]
+    mock_materialize_value_sets.assert_called_once_with(
+        mock.ANY, mock_value_sets, 100
     )
 
   @mock.patch.object(
-      bigquery_runner.value_set_tables,
-      'valueset_codes_insert_statement_for',
+      bigquery_value_set_manager.BigQueryValueSetManager,
+      'materialize_value_set_expansion',
       autospec=True,
   )
-  def testMaterializeValueSetExpansion_withTerminologyServiceUrl_usesGivenTerminologyServiceUrl(
-      self, mock_valueset_codes_insert_statement_for
+  def testMaterializeValueSetExpansion_delegatesToManager(
+      self, mock_materialize_value_set_expansion
   ):
-    mock_expander = mock.MagicMock(
-        spec=terminology_service_client.TerminologyServiceClient
-    )
-    self.mock_bigquery_client.create_table.return_value = _BqValuesetCodesTable(
-        'vs_project.vs_dataset.vs_table'
-    )
+    """Tests materialize through mock calls."""
+    mock_expander = mock.MagicMock()
 
     self.runner.materialize_value_set_expansion(
-        ['url-1', 'url-2'],
-        mock_expander,
-        terminology_service_url='http://my-service.com',
-    )
-
-    # Ensure we called valueset_codes_insert_statement_for with the value set
-    # expansions for both URLs and with an appropriate table object.
-    args, _ = mock_valueset_codes_insert_statement_for.call_args_list[0]
-    expanded_value_sets, table = args
-    self.assertEqual(
-        list(expanded_value_sets),
-        [
-            mock_expander.expand_value_set_url_using_service(),
-            mock_expander.expand_value_set_url_using_service(),
-        ],
-    )
-    self.assertEqual(table.name, 'vs_project.vs_dataset.vs_table')
-
-    # Ensure we call expand_value_set_url_using_service with the right URLs.
-    mock_expander.expand_value_set_url.reset()
-    mock_expander.expand_value_set_url_using_service.assert_has_calls([
-        mock.call('url-1', 'http://my-service.com'),
-        mock.call('url-2', 'http://my-service.com'),
-    ])
-
-  def testMaterializeValueSetExpansion_withTerminologyServiceUrlAndValueSetResolver_raisesError(
-      self,
-  ):
-    mock_expander = mock.MagicMock(spec=value_sets.ValueSetResolver)
+        ['url-1', 'url-2'], mock_expander, None, 100
+    )
 
-    with self.assertRaises(TypeError):
-      self.runner.materialize_value_set_expansion(
-          ['url-1', 'url-2'],
-          mock_expander,
-          terminology_service_url='http://my-service.com',
-      )
-
-  def testCreateValusetCodesTableIfNotExists_callsClientCorrectly(self):
-    self.runner._create_valueset_codes_table_if_not_exists()
-
-    expected_table = _BqValuesetCodesTable('vs_project.vs_dataset.vs_table')
-    self.mock_bigquery_client.create_table.assert_called_once_with(
-        expected_table, exists_ok=True
+    mock_materialize_value_set_expansion.assert_called_once_with(
+        mock.ANY, ['url-1', 'url-2'], mock_expander, None, 100
     )
 
   # TODO(b/250691318): Fix an issue where the bq_intepreter generates literals
   # with an extra set of quotes.
   def testFHIRViewsExample_explanationOfBenefit_filteredByValueSet_succeeds(
       self,
   ):
@@ -1150,22 +1030,9 @@
 ON all_.element_offset=matches.element_offset
 ORDER BY all_.element_offset))
 WHERE _anyTrue IS NOT NULL)) AS logic_)""",
         self.runner.to_sql(eob_outpatient_codes),
     )
 
 
-def _BqValuesetCodesTable(name: str) -> bigquery.table.Table:
-  """Builds a BigQuery client table representation of a value set codes table."""
-  schema = [
-      bigquery.SchemaField('valueseturi', 'STRING', mode='REQUIRED'),
-      bigquery.SchemaField('valuesetversion', 'STRING', mode='NULLABLE'),
-      bigquery.SchemaField('system', 'STRING', mode='REQUIRED'),
-      bigquery.SchemaField('code', 'STRING', mode='REQUIRED'),
-  ]
-  table = bigquery.Table(name, schema=schema)
-  table.clustering_fields = ['valueseturi', 'code']
-  return table
-
-
 if __name__ == '__main__':
   absltest.main()
```

## google/fhir/views/bigquery_runner_test_v2.py

```diff
@@ -21,17 +21,16 @@
 from google.cloud import bigquery
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from google.fhir.core.fhir_path import context
 from google.fhir.core.utils import fhir_package
 from google.fhir.r4 import r4_package
-from google.fhir.r4.terminology import terminology_service_client
-from google.fhir.r4.terminology import value_sets
 from google.fhir.views import bigquery_runner
+from google.fhir.views import bigquery_value_set_manager
 from google.fhir.views import r4
 from google.fhir.views import views
 
 
 class BigqueryRunnerTest(parameterized.TestCase):
   """Tests the bigquery runner running on v2."""
 
@@ -118,14 +117,16 @@
     """Tests initializing with a valueset table."""
     runner = bigquery_runner.BigQueryRunner(
         self.mock_bigquery_client,
         'test_dataset',
         value_set_codes_table=value_set_codes_table,
     )
     self.assertEqual(runner._value_set_codes_table, expected_table_name)  # pylint: disable=protected-access
+    self.assertEqual(runner._value_set_manager.value_set_codes_table,  # pylint: disable=protected-access
+                     expected_table_name)
 
   def testNestedSingleFieldInNestedArray_forPatient_returnsArray(self):
     """Tests selecting a single field in a nested array."""
     pat = self._views.view_of('Patient')
     simple_view = pat.select({
         'family_names': pat.name.family,
     })
@@ -282,14 +283,37 @@
         FROM (SELECT SAFE_CAST(telecom_element_.period.start AS TIMESTAMP) AS start
         FROM UNNEST(telecom) AS telecom_element_ WITH OFFSET AS element_offset)
         WHERE start IS NOT NULL) AS telecom,(SELECT id) AS __patientId__ FROM `test_project.test_dataset`.Patient"""
         ),
         telecom,
     )
 
+  def testSimpleSelectWithAllMatches_forPatient_succeeds(self):
+    """Tests selecting an array of dates."""
+    pat = self._views.view_of('Patient')
+    telecom = pat.select(
+        {'name': pat.name.given.all(pat.name.given.matches('regex'))}
+    )
+
+    self.AstAndExpressionTreeTestRunner(
+        textwrap.dedent(
+            """\
+        SELECT *, (SELECT IFNULL(
+        LOGICAL_AND(
+        IFNULL(
+        (SELECT REGEXP_CONTAINS(
+        given_element_, 'regex') AS all_), FALSE)), TRUE) AS all_
+        FROM (SELECT name_element_
+        FROM (SELECT Patient),
+        UNNEST(Patient.name) AS name_element_ WITH OFFSET AS element_offset),
+        UNNEST(name_element_.given) AS given_element_ WITH OFFSET AS element_offset) AS name FROM (SELECT (SELECT id) AS __patientId__,Patient FROM `test_project.test_dataset`.Patient Patient)"""
+        ),
+        telecom,
+    )
+
   def testQueryToDataFrame_forPatient_succeeds(self):
     """Test to_dataframe()."""
     pat = self._views.view_of('Patient')
     simple_view = pat.select(
         {'name': pat.name.given, 'birthDate': pat.birthDate}
     )
 
@@ -974,182 +998,45 @@
           WHERE exists_ IS NOT NULL)) AS logic_))
           USING(__patientId__))"""
         ),
         enc_and_pat_class,
     )
 
   @mock.patch.object(
-      bigquery_runner.value_set_tables,
-      'valueset_codes_insert_statement_for',
+      bigquery_value_set_manager.BigQueryValueSetManager,
+      'materialize_value_sets',
       autospec=True,
   )
-  def testMaterializeValueSet_withValueSetObject_insertsData(
-      self, mock_valueset_codes_insert_statement_for
+  def testMaterializeValueSet_delegatesToManager(
+      self, mock_materialize_value_sets
   ):
     """Tests inserting data through mock call."""
     mock_value_sets = [mock.MagicMock(), mock.MagicMock()]
-    mock_insert_statements = [mock.MagicMock(), mock.MagicMock()]
-    mock_valueset_codes_insert_statement_for.return_value = (
-        mock_insert_statements
-    )
-    self.mock_bigquery_client.create_table.return_value = _BqValuesetCodesTable(
-        'vs_project.vs_dataset.vs_table'
-    )
-
-    self.runner.materialize_value_sets(mock_value_sets)
-
-    # Ensure we tried to create the table
-    self.mock_bigquery_client.create_table.assert_called_once()
-
-    # Ensure we called query with the rendered SQL for the two mock queries and
-    # called .result() on the returned job.
-    self.mock_bigquery_client.query.assert_has_calls([
-        mock.call(str(mock_insert_statements[0].compile())),
-        mock.call().result(),
-        mock.call(str(mock_insert_statements[1].compile())),
-        mock.call().result(),
-    ])
-
-    # Ensure we called valueset_codes_insert_statement_for with the
-    # given value sets.
-    args, kwargs = mock_valueset_codes_insert_statement_for.call_args_list[0]
-    expanded_value_sets, table = args
-    self.assertEqual(list(expanded_value_sets), mock_value_sets)
-
-    self.assertEqual(table.name, 'vs_project.vs_dataset.vs_table')
-    for col in ('valueseturi', 'valuesetversion', 'system', 'code'):
-      self.assertIn(col, table.columns)
-    self.assertEqual(kwargs['batch_size'], 500)
 
-  @mock.patch.object(
-      bigquery_runner.value_set_tables,
-      'valueset_codes_insert_statement_for',
-      autospec=True,
-  )
-  def testMaterializeValueSetExpansion_withValueSetUrls_performsExpansionsAndInserts(
-      self, mock_valueset_codes_insert_statement_for
-  ):
-    """Tests materialize through mock calls."""
-    mock_insert_statements = [mock.MagicMock(), mock.MagicMock()]
-    mock_valueset_codes_insert_statement_for.return_value = (
-        mock_insert_statements
-    )
-    mock_expander = mock.MagicMock()
-    self.mock_bigquery_client.create_table.return_value = _BqValuesetCodesTable(
-        'vs_project.vs_dataset.vs_table'
-    )
+    self.runner.materialize_value_sets(mock_value_sets, 100)
 
-    self.runner.materialize_value_set_expansion(
-        ['url-1', 'url-2'], mock_expander
-    )
-
-    # Ensure we tried to create the table
-    self.mock_bigquery_client.create_table.assert_called_once()
-
-    # Ensure we called query with the rendered SQL for the two mock queries and
-    # called .result() on the returned job.
-    self.mock_bigquery_client.query.assert_has_calls([
-        mock.call(str(mock_insert_statements[0].compile())),
-        mock.call().result(),
-        mock.call(str(mock_insert_statements[1].compile())),
-        mock.call().result(),
-    ])
-    # Ensure we called valueset_codes_insert_statement_for with the value set
-    # expansions for both URLs and with an appropriate table object.
-    args, kwargs = mock_valueset_codes_insert_statement_for.call_args_list[0]
-    expanded_value_sets, table = args
-    self.assertEqual(
-        list(expanded_value_sets),
-        [
-            mock_expander.expand_value_set_url(),
-            mock_expander.expand_value_set_url(),
-        ],
-    )
-    self.assertEqual(table.name, 'vs_project.vs_dataset.vs_table')
-    for col in ('valueseturi', 'valuesetversion', 'system', 'code'):
-      self.assertIn(col, table.columns)
-    self.assertEqual(kwargs['batch_size'], 500)
-
-    # Ensure we call expand_value_set_url with the two URLs.
-    mock_expander.expand_value_set_url.reset()
-    mock_expander.expand_value_set_url.assert_has_calls(
-        [mock.call('url-1'), mock.call('url-2')]
+    mock_materialize_value_sets.assert_called_once_with(
+        mock.ANY, mock_value_sets, 100
     )
 
   @mock.patch.object(
-      bigquery_runner.value_set_tables,
-      'valueset_codes_insert_statement_for',
+      bigquery_value_set_manager.BigQueryValueSetManager,
+      'materialize_value_set_expansion',
       autospec=True,
   )
-  def testMaterializeValueSetExpansion_withTerminologyServiceUrl_usesGivenTerminologyServiceUrl(
-      self, mock_valueset_codes_insert_statement_for
+  def testMaterializeValueSetExpansion_delegatesToManager(
+      self, mock_materialize_value_set_expansion
   ):
-    """Tests materialze value sets with terminology service url."""
-    mock_expander = mock.MagicMock(
-        spec=terminology_service_client.TerminologyServiceClient
-    )
-    self.mock_bigquery_client.create_table.return_value = _BqValuesetCodesTable(
-        'vs_project.vs_dataset.vs_table'
-    )
+    """Tests materialize through mock calls."""
+    mock_expander = mock.MagicMock()
 
     self.runner.materialize_value_set_expansion(
-        ['url-1', 'url-2'],
-        mock_expander,
-        terminology_service_url='http://my-service.com',
-    )
-
-    # Ensure we called valueset_codes_insert_statement_for with the value set
-    # expansions for both URLs and with an appropriate table object.
-    args, _ = mock_valueset_codes_insert_statement_for.call_args_list[0]
-    expanded_value_sets, table = args
-    self.assertEqual(
-        list(expanded_value_sets),
-        [
-            mock_expander.expand_value_set_url_using_service(),
-            mock_expander.expand_value_set_url_using_service(),
-        ],
-    )
-    self.assertEqual(table.name, 'vs_project.vs_dataset.vs_table')
-
-    # Ensure we call expand_value_set_url_using_service with the right URLs.
-    mock_expander.expand_value_set_url.reset()
-    mock_expander.expand_value_set_url_using_service.assert_has_calls([
-        mock.call('url-1', 'http://my-service.com'),
-        mock.call('url-2', 'http://my-service.com'),
-    ])
-
-  def testMaterializeValueSetExpansion_withTerminologyServiceUrlAndValueSetResolver_raisesError(
-      self,
-  ):
-    mock_expander = mock.MagicMock(spec=value_sets.ValueSetResolver)
-
-    with self.assertRaises(TypeError):
-      self.runner.materialize_value_set_expansion(
-          ['url-1', 'url-2'],
-          mock_expander,
-          terminology_service_url='http://my-service.com',
-      )
-
-  def testCreateValusetCodesTableIfNotExists_callsClientCorrectly(self):
-    self.runner._create_valueset_codes_table_if_not_exists()  # pylint: disable=protected-access
-
-    expected_table = _BqValuesetCodesTable('vs_project.vs_dataset.vs_table')
-    self.mock_bigquery_client.create_table.assert_called_once_with(
-        expected_table, exists_ok=True
+        ['url-1', 'url-2'], mock_expander, None, 100
     )
 
-
-def _BqValuesetCodesTable(name: str) -> bigquery.table.Table:
-  """Builds a BigQuery client table representation of a value set codes table."""
-  schema = [
-      bigquery.SchemaField('valueseturi', 'STRING', mode='REQUIRED'),
-      bigquery.SchemaField('valuesetversion', 'STRING', mode='NULLABLE'),
-      bigquery.SchemaField('system', 'STRING', mode='REQUIRED'),
-      bigquery.SchemaField('code', 'STRING', mode='REQUIRED'),
-  ]
-  table = bigquery.Table(name, schema=schema)
-  table.clustering_fields = ['valueseturi', 'code']
-  return table
+    mock_materialize_value_set_expansion.assert_called_once_with(
+        mock.ANY, ['url-1', 'url-2'], mock_expander, None, 100
+    )
 
 
 if __name__ == '__main__':
   absltest.main()
```

## google/fhir/views/spark_runner.py

```diff
@@ -16,23 +16,27 @@
 
 This module allows users to run FHIR Views against Spark. Users may retrieve
 results through the Spark library used here, or create Spark views that
 can be consumed by other tools.
 """
 
 import re
-from typing import Dict, Optional, cast
+from typing import Dict, Iterable, Optional, Union, cast
 
 import pandas
 from sqlalchemy import engine
 
+from google.fhir.r4.proto.core.resources import value_set_pb2
 from google.fhir.core.fhir_path import _fhir_path_data_types
 from google.fhir.core.fhir_path import _spark_interpreter
 from google.fhir.core.fhir_path import expressions
+from google.fhir.r4.terminology import terminology_service_client
+from google.fhir.r4.terminology import value_sets
 from google.fhir.views import runner_utils
+from google.fhir.views import spark_value_set_manager
 from google.fhir.views import views
 
 
 class SparkRunner:
   """FHIR Views runner used to perform queries against Spark."""
 
   def __init__(
@@ -68,14 +72,17 @@
                           if view_dataset is not None else self._fhir_dataset)
     self._value_set_codes_table = (
         value_set_codes_table
         if value_set_codes_table is not None
         else 'value_set_codes'
     )
     self._snake_case_resource_tables = snake_case_resource_tables
+    self._value_set_manager = spark_value_set_manager.SparkValueSetManager(
+        query_engine, self._value_set_codes_table
+    )
 
   def to_sql(
       self,
       view: views.View,
       limit: Optional[int] = None,
       include_patient_id_col: bool = True,
   ) -> str:
@@ -86,15 +93,17 @@
       limit: optional limit to attach to the generated SQL.
       include_patient_id_col: whether to include a __patientId__ column to
         indicate the patient the resource is associated with.
 
     Returns:
       The SQL used to run the given view.
     """
-    encoder = _spark_interpreter.SparkSqlInterpreter()
+    encoder = _spark_interpreter.SparkSqlInterpreter(
+        value_set_codes_table='VALUESET_VIEW',
+    )
 
     dataset = f'{self._fhir_dataset}'
     table_names = self._view_table_names(view)
     sql_generator = runner_utils.RunnerSqlGenerator(
         view, encoder, dataset, table_names
     )
 
@@ -244,7 +253,89 @@
       view_name: the view name passed to the CREATE OR REPLACE VIEW statement.
     """
     view_sql = (
         f'CREATE OR REPLACE VIEW {self._view_dataset}.{view_name} AS\n'
         f'{self.to_sql(view, include_patient_id_col=False)}'
     )
     self._engine.execute(view_sql).fetchall()
+
+  # TODO(b/201107372): Update FHIR-agnostic types to a protocol.
+  def materialize_value_sets(
+      self,
+      value_set_protos: Iterable[value_set_pb2.ValueSet],
+      batch_size: int = 500,
+  ) -> None:
+    """Materialize the given value sets into the value_set_codes_table.
+
+    Then writes these expanded codes into the database
+    named after the `value_set_codes_table` provided at class initialization.
+    Builds a valueset_codes table as described by
+    https://github.com/FHIR/sql-on-fhir/blob/master/sql-on-fhir.md#valueset-support
+
+    The table will be created if it does not already exist.
+
+    The function will avoid inserting duplicate rows if some of the codes are
+    already present in the given table. It will not attempt to perform an
+    'upsert' or modify any existing rows.
+
+    Note that value sets provided to this function should already be expanded,
+    in that they contain the code values to write. Users should also see
+    `materialize_value_set_expansion` below to retrieve an expanded set from
+    a terminology server.
+
+    Args:
+      value_set_protos: An iterable of FHIR ValueSet protos.
+      batch_size: The maximum number of rows to insert in a single query.
+    """
+    self._value_set_manager.materialize_value_sets(value_set_protos, batch_size)
+
+  def materialize_value_set_expansion(
+      self,
+      urls: Iterable[str],
+      expander: Union[
+          terminology_service_client.TerminologyServiceClient,
+          value_sets.ValueSetResolver,
+      ],
+      terminology_service_url: Optional[str] = None,
+      batch_size: int = 500,
+  ) -> None:
+    """Expands a sequence of value set and materializes their expanded codes.
+
+    Expands the given value set URLs to obtain the set of codes they describe.
+    Then writes these expanded codes into the database
+    named after the `value_set_codes_table` provided at class initialization.
+    Builds a valueset_codes table as described by
+    https://github.com/FHIR/sql-on-fhir/blob/master/sql-on-fhir.md#valueset-support
+
+    The table will be created if it does not already exist.
+
+    The function will avoid inserting duplicate rows if some of the codes are
+    already present in the given table. It will not attempt to perform an
+    'upsert' or modify any existing rows.
+
+    Provided as a utility function for user convenience. If `urls` is a large
+    set of URLs, callers may prefer to use multi-processing and/or
+    multi-threading to perform expansion and table insertion of the URLs
+    concurrently. This function performs all expansions and table insertions
+    serially.
+
+    Args:
+      urls: The urls for value sets to expand and materialize.
+      expander: The ValueSetResolver or TerminologyServiceClient to perform
+        value set expansion. A ValueSetResolver may be used to attempt to avoid
+        some network requests by expanding value sets locally. A
+        TerminologyServiceClient will use external terminology services to
+        perform all value set expansions.
+      terminology_service_url: If `expander` is a TerminologyServiceClient, the
+        URL of the terminology service to use when expanding value set URLs. If
+        not given, the client will attempt to infer the correct terminology
+        service to use for each value set URL based on its domain.
+      batch_size: The maximum number of rows to insert in a single query.
+
+    Raises:
+      TypeError: If a `terminology_service_url` is given but `expander` is not a
+      TerminologyServiceClient.
+    """
+    self._value_set_manager.materialize_value_set_expansion(
+        urls, expander, terminology_service_url, batch_size
+    )
+
```

## google/fhir/views/spark_runner_test.py

```diff
@@ -11,27 +11,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for spark_runner."""
 
 import datetime
-
 from typing import Optional
 from unittest import mock
 
 import pandas
 from sqlalchemy import engine
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from google.fhir.core.fhir_path import context
 from google.fhir.r4 import r4_package
 from google.fhir.views import r4
 from google.fhir.views import spark_runner
+from google.fhir.views import spark_value_set_manager
 from google.fhir.views import views
 
 
 _WITH_VALUE_SET_TABLE_INIT_SUCCEEDS_CASES = [
     {
         'testcase_name': 'None_usesDefaultName',
         'value_set_codes_table': None,
@@ -239,15 +239,69 @@
             'WHERE (SELECT EXISTS(*, x -> x IS true) FROM '
             '(SELECT COLLECT_LIST(comparison_) FROM '
             '(SELECT CAST(birthDate AS TIMESTAMP) < '
             "CAST('1960-01-01' AS TIMESTAMP) AS comparison_) "
             'WHERE comparison_ IS NOT NULL))'
         ),
         view=born_before_1960,
-        runner=self.runner
+        runner=self.runner,
+    )
+
+  def testSimpleSelectWithComplexFilterToSql_forPatient_succeeds(self):
+    """Tests filtering with a complex filter."""
+    pats = self._views.view_of('Patient')
+
+    current = pats.address.where(pats.address.period.empty()).first()
+
+    simple_pats = pats.select({
+        'id': pats.id,
+        'gender': pats.gender,
+        'birthdate': pats.birthDate,
+        'street': current.line.first(),
+        'city': current.city,
+        'state': current.state,
+        'zip': current.postalCode,
+    })
+
+    self.AstAndExpressionTreeTestRunner(
+        expected_output=(
+            'SELECT (SELECT id) AS id,(SELECT gender) AS gender,(SELECT'
+            ' CAST(birthDate AS TIMESTAMP) AS birthDate) AS birthdate,(SELECT'
+            ' line_element_ FROM (SELECT FIRST(line_element_) AS line_element_'
+            ' FROM (SELECT line_element_ FROM (SELECT address_element_ FROM'
+            ' (SELECT FIRST(address_element_) AS address_element_ FROM (SELECT'
+            ' address_element_ FROM (SELECT EXPLODE(address_element_) AS'
+            ' address_element_ FROM (SELECT address AS address_element_)) WHERE'
+            ' (SELECT CASE WHEN COUNT(*) = 0 THEN TRUE ELSE FALSE END AS empty_'
+            ' FROM (SELECT address_element_.period) WHERE period IS NOT'
+            ' NULL)))) LATERAL VIEW POSEXPLODE(address_element_.line) AS'
+            ' index_line_element_, line_element_))) AS street,(SELECT'
+            ' address_element_.city FROM (SELECT FIRST(address_element_) AS'
+            ' address_element_ FROM (SELECT address_element_ FROM (SELECT'
+            ' EXPLODE(address_element_) AS address_element_ FROM (SELECT'
+            ' address AS address_element_)) WHERE (SELECT CASE WHEN COUNT(*) ='
+            ' 0 THEN TRUE ELSE FALSE END AS empty_ FROM (SELECT'
+            ' address_element_.period) WHERE period IS NOT NULL)))) AS'
+            ' city,(SELECT address_element_.state FROM (SELECT'
+            ' FIRST(address_element_) AS address_element_ FROM (SELECT'
+            ' address_element_ FROM (SELECT EXPLODE(address_element_) AS'
+            ' address_element_ FROM (SELECT address AS address_element_)) WHERE'
+            ' (SELECT CASE WHEN COUNT(*) = 0 THEN TRUE ELSE FALSE END AS empty_'
+            ' FROM (SELECT address_element_.period) WHERE period IS NOT'
+            ' NULL)))) AS state,(SELECT address_element_.postalCode FROM'
+            ' (SELECT FIRST(address_element_) AS address_element_ FROM (SELECT'
+            ' address_element_ FROM (SELECT EXPLODE(address_element_) AS'
+            ' address_element_ FROM (SELECT address AS address_element_)) WHERE'
+            ' (SELECT CASE WHEN COUNT(*) = 0 THEN TRUE ELSE FALSE END AS empty_'
+            ' FROM (SELECT address_element_.period) WHERE period IS NOT'
+            ' NULL)))) AS zip,(SELECT id) AS __patientId__ FROM'
+            ' `default`.Patient'
+        ),
+        view=simple_pats,
+        runner=self.runner,
     )
 
   def testSimpleSelectWithArrayOfDateToSql_forPatient_succeeds(self):
     """Tests selecting an array of dates."""
     pat = self._views.view_of('Patient')
     telecom = pat.select(
         {'name': pat.name.given, 'telecom': pat.telecom.period.start}
@@ -352,9 +406,46 @@
     expected_sql = (
         'CREATE OR REPLACE VIEW '
         'default.simple_patient_view AS\n'
         f'{self.runner.to_sql(simple_view, include_patient_id_col=False)}'
     )
     self.mock_spark_engine.execute.assert_called_once_with(expected_sql)
 
+  @mock.patch.object(
+      spark_value_set_manager.SparkValueSetManager,
+      'materialize_value_sets',
+      autospec=True,
+  )
+  def testMaterializeValueSet_delegatesToManager(
+      self, mock_materialize_value_sets
+  ):
+    """Tests inserting data through mock call."""
+    mock_value_sets = [mock.MagicMock(), mock.MagicMock()]
+
+    self.runner.materialize_value_sets(mock_value_sets, 100)
+
+    mock_materialize_value_sets.assert_called_once_with(
+        mock.ANY, mock_value_sets, 100
+    )
+
+  @mock.patch.object(
+      spark_value_set_manager.SparkValueSetManager,
+      'materialize_value_set_expansion',
+      autospec=True,
+  )
+  def testMaterializeValueSetExpansion_delegatesToManager(
+      self, mock_materialize_value_set_expansion
+  ):
+    """Tests materialize through mock calls."""
+    mock_expander = mock.MagicMock()
+
+    self.runner.materialize_value_set_expansion(
+        ['url-1', 'url-2'], mock_expander, None, 100
+    )
+
+    mock_materialize_value_set_expansion.assert_called_once_with(
+        mock.ANY, ['url-1', 'url-2'], mock_expander, None, 100
+    )
+
+
 if __name__ == '__main__':
   absltest.main()
```

## Comparing `google_fhir_views-0.9.2.dist-info/METADATA` & `google_fhir_views-0.9.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-fhir-views
-Version: 0.9.2
+Version: 0.9.3
 Summary: Tools to create views of FHIR data for analysis.
 Home-page: https://github.com/google/fhir-py
 Download-URL: https://github.com/google-py/fhir/releases
 Author: Google LLC
 Author-email: google-fhir-pypi@google.com
 License: Apache 2.0
 Keywords: google,fhir,python,healthcare
@@ -12,29 +12,33 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: absl-py (~=1.1)
-Requires-Dist: google-fhir-core (~=0.9.2)
+Requires-Dist: google-fhir-core (~=0.9.3)
 Requires-Dist: immutabledict (~=2.2)
 Requires-Dist: pandas (~=1.1)
 Requires-Dist: protobuf (~=3.19)
 Requires-Dist: python-dateutil (~=2.8)
-Requires-Dist: requests-mock (~=1.9)
 Requires-Dist: requests (~=2.27)
+Requires-Dist: requests-mock (~=1.9)
 Requires-Dist: backports.zoneinfo (~=0.2.1) ; python_version < "3.9"
 Provides-Extra: bigquery
+Requires-Dist: google-fhir-core[bigquery] (~=0.9.3) ; extra == 'bigquery'
 Requires-Dist: google-cloud-bigquery (~=3.1) ; extra == 'bigquery'
-Requires-Dist: google-fhir-core[bigquery] (~=0.9.2) ; extra == 'bigquery'
-Requires-Dist: sqlalchemy-bigquery (~=1.4) ; extra == 'bigquery'
 Requires-Dist: sqlalchemy (~=1.4) ; extra == 'bigquery'
+Requires-Dist: sqlalchemy-bigquery (~=1.4) ; extra == 'bigquery'
 Provides-Extra: r4
-Requires-Dist: google-fhir-r4 (~=0.9.2) ; extra == 'r4'
+Requires-Dist: google-fhir-r4 (~=0.9.3) ; extra == 'r4'
+Provides-Extra: spark
+Requires-Dist: sqlalchemy (~=1.4) ; extra == 'spark'
+Requires-Dist: pandas (>=1.5) ; extra == 'spark'
+Requires-Dist: pyhive (>=0.6) ; extra == 'spark'
 
 # FHIR Views
 
 ## Introduction
 
 FHIR Views is a way to define simple, tabular views over complex FHIR data and
 turn them into queries that use
```

