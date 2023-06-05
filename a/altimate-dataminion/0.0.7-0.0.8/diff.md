# Comparing `tmp/altimate_dataminion-0.0.7.tar.gz` & `tmp/altimate_dataminion-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altimate_dataminion-0.0.7.tar", max compression
+gzip compressed data, was "altimate_dataminion-0.0.8.tar", max compression
```

## Comparing `altimate_dataminion-0.0.7.tar` & `altimate_dataminion-0.0.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0       67 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/README.md
--rw-r--r--   0        0        0      197 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/base/__init__.py
--rw-r--r--   0        0        0     6650 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/base/dialect.py
--rw-r--r--   0        0        0     3365 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/base/extractor.py
--rw-r--r--   0        0        0     4767 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/base/metadata_profiler.py
--rw-r--r--   0        0        0     4400 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/base/profiler.py
--rw-r--r--   0        0        0     3462 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/base/source.py
--rw-r--r--   0        0        0     6657 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/base/ssh_source.py
--rw-r--r--   0        0        0     2710 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/config_factory.py
--rw-r--r--   0        0        0     1344 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/constants.py
--rw-r--r--   0        0        0        0 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/duckdb/__init__.py
--rw-r--r--   0        0        0     7220 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/duckdb/dialect.py
--rw-r--r--   0        0        0     2694 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/duckdb/extractor.py
--rw-r--r--   0        0        0     4793 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/duckdb/metadata_profiler.py
--rw-r--r--   0        0        0     3119 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/duckdb/profiler.py
--rw-r--r--   0        0        0        0 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/postgresql/__init__.py
--rw-r--r--   0        0        0     7331 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/postgresql/dialect.py
--rw-r--r--   0        0        0      331 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/postgresql/extractor.py
--rw-r--r--   0        0        0     1190 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/postgresql/profiler.py
--rw-r--r--   0        0        0     5988 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/postgresql/source.py
--rw-r--r--   0        0        0        0 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/s3/__init__.py
--rw-r--r--   0        0        0     2196 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/s3/csv_source_dialect.py
--rw-r--r--   0        0        0      361 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/s3/extractor.py
--rw-r--r--   0        0        0     2252 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/s3/json_source_dialect.py
--rw-r--r--   0        0        0     1872 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/s3/parquet_source_dialect.py
--rw-r--r--   0        0        0      939 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/s3/profiler.py
--rw-r--r--   0        0        0     7685 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/s3/source.py
--rw-r--r--   0        0        0      390 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/s3/utils.py
--rw-r--r--   0        0        0     1289 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/shared_models.py
--rw-r--r--   0        0        0        0 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/snowflake/__init__.py
--rw-r--r--   0        0        0    13760 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/snowflake/dialect.py
--rw-r--r--   0        0        0     1083 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/snowflake/profiler.py
--rw-r--r--   0        0        0     7361 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_models/snowflake/source.py
--rw-r--r--   0        0        0      260 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/__init__.py
--rw-r--r--   0        0        0      134 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/base_builder.py
--rw-r--r--   0        0        0     4269 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/column_metrics_query_builder.py
--rw-r--r--   0        0        0      548 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/custom_query_builder.py
--rw-r--r--   0        0        0     1146 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/metadata_query_builder.py
--rw-r--r--   0        0        0      912 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/performance_query_builder.py
--rw-r--r--   0        0        0     1637 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/s3_column_metrics_query_builder.py
--rw-r--r--   0        0        0     2127 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/s3_schema_query_builder.py
--rw-r--r--   0        0        0     1052 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/s3_table_query_builder.py
--rw-r--r--   0        0        0     2091 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/schema_query_builder.py
--rw-r--r--   0        0        0     1381 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/table_query_builder.py
--rw-r--r--   0        0        0      999 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/builders/utils.py
--rw-r--r--   0        0        0      603 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/exceptions.py
--rw-r--r--   0        0        0     4239 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/factory.py
--rw-r--r--   0        0        0     2308 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/main.py
--rw-r--r--   0        0        0        0 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/metrics/__init__.py
--rw-r--r--   0        0        0     2101 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/metrics/column_metric_type.py
--rw-r--r--   0        0        0      385 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/metrics/metadata_metric_type.py
--rw-r--r--   0        0        0      390 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/metrics/performance_metric_type.py
--rw-r--r--   0        0        0      363 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/metrics/schema_metric_type.py
--rw-r--r--   0        0        0      256 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/metrics/table_metric_type.py
--rw-r--r--   0        0        0        0 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/transformer/__init__.py
--rw-r--r--   0        0        0     1716 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/transformer/base.py
--rw-r--r--   0        0        0     2061 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/transformer/duckdb_schema.py
--rw-r--r--   0        0        0     2295 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/transformer/metrics.py
--rw-r--r--   0        0        0     2129 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/transformer/schema.py
--rw-r--r--   0        0        0      394 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/utils.py
--rw-r--r--   0        0        0        0 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/validator/__init__.py
--rw-r--r--   0        0        0     2207 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/validator/mappers.py
--rw-r--r--   0        0        0     1952 2023-06-04 23:24:34.594343 altimate_dataminion-0.0.7/altimate_profiler/validator/utils.py
--rw-r--r--   0        0        0      764 2023-06-04 23:24:34.598343 altimate_dataminion-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 altimate_dataminion-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       67 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/README.md
+-rw-r--r--   0        0        0      197 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/base/__init__.py
+-rw-r--r--   0        0        0     6650 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/base/dialect.py
+-rw-r--r--   0        0        0     3365 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/base/extractor.py
+-rw-r--r--   0        0        0     4767 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/base/metadata_profiler.py
+-rw-r--r--   0        0        0     4400 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/base/profiler.py
+-rw-r--r--   0        0        0     3577 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/base/source.py
+-rw-r--r--   0        0        0     6741 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/base/ssh_source.py
+-rw-r--r--   0        0        0     2710 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/config_factory.py
+-rw-r--r--   0        0        0     1344 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/constants.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/duckdb/__init__.py
+-rw-r--r--   0        0        0     7220 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/duckdb/dialect.py
+-rw-r--r--   0        0        0     2694 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/duckdb/extractor.py
+-rw-r--r--   0        0        0     4793 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/duckdb/metadata_profiler.py
+-rw-r--r--   0        0        0     3119 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/duckdb/profiler.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/postgresql/__init__.py
+-rw-r--r--   0        0        0     7331 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/postgresql/dialect.py
+-rw-r--r--   0        0        0      331 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/postgresql/extractor.py
+-rw-r--r--   0        0        0     1190 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/postgresql/profiler.py
+-rw-r--r--   0        0        0     6275 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/postgresql/source.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/s3/__init__.py
+-rw-r--r--   0        0        0     2196 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/s3/csv_source_dialect.py
+-rw-r--r--   0        0        0      361 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/s3/extractor.py
+-rw-r--r--   0        0        0     2252 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/s3/json_source_dialect.py
+-rw-r--r--   0        0        0     1872 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/s3/parquet_source_dialect.py
+-rw-r--r--   0        0        0      939 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/s3/profiler.py
+-rw-r--r--   0        0        0     7685 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/s3/source.py
+-rw-r--r--   0        0        0      390 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/s3/utils.py
+-rw-r--r--   0        0        0     1289 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/shared_models.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/snowflake/__init__.py
+-rw-r--r--   0        0        0    13760 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/snowflake/dialect.py
+-rw-r--r--   0        0        0     1083 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/snowflake/profiler.py
+-rw-r--r--   0        0        0     7675 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_models/snowflake/source.py
+-rw-r--r--   0        0        0      260 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_profiler/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_profiler/builders/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_profiler/builders/base_builder.py
+-rw-r--r--   0        0        0     4269 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_profiler/builders/column_metrics_query_builder.py
+-rw-r--r--   0        0        0      548 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_profiler/builders/custom_query_builder.py
+-rw-r--r--   0        0        0     1146 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_profiler/builders/metadata_query_builder.py
+-rw-r--r--   0        0        0      912 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_profiler/builders/performance_query_builder.py
+-rw-r--r--   0        0        0     1637 2023-06-05 17:34:31.154370 altimate_dataminion-0.0.8/altimate_profiler/builders/s3_column_metrics_query_builder.py
+-rw-r--r--   0        0        0     2127 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/builders/s3_schema_query_builder.py
+-rw-r--r--   0        0        0     1052 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/builders/s3_table_query_builder.py
+-rw-r--r--   0        0        0     2091 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/builders/schema_query_builder.py
+-rw-r--r--   0        0        0     1381 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/builders/table_query_builder.py
+-rw-r--r--   0        0        0      999 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/builders/utils.py
+-rw-r--r--   0        0        0      603 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/exceptions.py
+-rw-r--r--   0        0        0     4239 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/factory.py
+-rw-r--r--   0        0        0     2308 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/main.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/metrics/__init__.py
+-rw-r--r--   0        0        0     2101 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/metrics/column_metric_type.py
+-rw-r--r--   0        0        0      385 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/metrics/metadata_metric_type.py
+-rw-r--r--   0        0        0      390 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/metrics/performance_metric_type.py
+-rw-r--r--   0        0        0      363 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/metrics/schema_metric_type.py
+-rw-r--r--   0        0        0      256 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/metrics/table_metric_type.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/transformer/__init__.py
+-rw-r--r--   0        0        0     1716 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/transformer/base.py
+-rw-r--r--   0        0        0     2061 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/transformer/duckdb_schema.py
+-rw-r--r--   0        0        0     2295 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/transformer/metrics.py
+-rw-r--r--   0        0        0     2129 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/transformer/schema.py
+-rw-r--r--   0        0        0      394 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/validator/__init__.py
+-rw-r--r--   0        0        0     2207 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/validator/mappers.py
+-rw-r--r--   0        0        0     1952 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/altimate_profiler/validator/utils.py
+-rw-r--r--   0        0        0      764 2023-06-05 17:34:31.158370 altimate_dataminion-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 altimate_dataminion-0.0.8/PKG-INFO
```

### Comparing `altimate_dataminion-0.0.7/altimate_models/base/dialect.py` & `altimate_dataminion-0.0.8/altimate_models/base/dialect.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/base/extractor.py` & `altimate_dataminion-0.0.8/altimate_models/base/extractor.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/base/metadata_profiler.py` & `altimate_dataminion-0.0.8/altimate_models/base/metadata_profiler.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/base/profiler.py` & `altimate_dataminion-0.0.8/altimate_models/base/profiler.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/base/source.py` & `altimate_dataminion-0.0.8/altimate_models/base/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 class DataSource(BaseModel):
     id: Optional[Text]
     name: Text
     type: Text
     description: Optional[Text]
     connection_info: Optional[Text]
     connection_hash: Optional[Text]
+    statement_timeout_in_ms: Optional[int]
 
     @classmethod
     def prompt(cls, data_store_config: Dict):
         raise NotImplementedError()
 
     def cred_prompt(self):
         raise NotImplementedError()
@@ -60,29 +61,32 @@
 
     def update_credentials(self, key: str):
         raise NotImplementedError()
 
     def override_schema(self, schema):
         raise NotImplementedError()
 
+    def get_connect_args(self):
+        return {"connect_timeout": DEFAULT_CLIENT_DB_CONNECTION_TIMEOUT}
+
     @contextmanager
     def get_engine(self):
         """
         has to be run as a context manager
         or else the tunnel will close
         """
         if not "sqlalchemy" in sys.modules:
             raise ImportError(
                 "sqlalchemy is not installed. Please install sqlalchemy to test connections"
             )
         with self.get_bound_host_and_port() as conn_args:
             # connect_args might not be supported by all dialects
             engine = create_engine(
                 self.get_connection_string(**conn_args),
-                connect_args={"connect_timeout": DEFAULT_CLIENT_DB_CONNECTION_TIMEOUT},
+                connect_args=self.get_connect_args(),
             )
             try:
                 yield engine
                 # the ssh tunnel would close up after the outer context manager exits
             except Exception as e:
                 # re-raise the exceptions here so as to not catch them here and silently fail
                 raise e
```

### Comparing `altimate_dataminion-0.0.7/altimate_models/base/ssh_source.py` & `altimate_dataminion-0.0.8/altimate_models/base/ssh_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
 
     def update_credentials(self, key: str):
         return self.original_ds.update_credentials(key)
 
     def override_schema(self, schema):
         return self.original_ds.override_schema(schema)
 
+    def get_connect_args(self):
+        return self.original_ds.get_connect_args()
+
     # delegator to the original datasource object. This should catch any methods not
     # overridden above (baseclass does not have specific methods that are part of
     # pg or snowflake implementations eg. host/port or warehouse etc)
     # and use the original datasource to generate responses
     def __getattr__(self, prop_or_func):
         # we are also delegating properties so we need to handle them separately
         # these are not functions but actual values so instead of the method wrapper
```

### Comparing `altimate_dataminion-0.0.7/altimate_models/config_factory.py` & `altimate_dataminion-0.0.8/altimate_models/config_factory.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/constants.py` & `altimate_dataminion-0.0.8/altimate_models/constants.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/duckdb/dialect.py` & `altimate_dataminion-0.0.8/altimate_models/duckdb/dialect.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/duckdb/extractor.py` & `altimate_dataminion-0.0.8/altimate_models/duckdb/extractor.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/duckdb/metadata_profiler.py` & `altimate_dataminion-0.0.8/altimate_models/duckdb/metadata_profiler.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/duckdb/profiler.py` & `altimate_dataminion-0.0.8/altimate_models/duckdb/profiler.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/postgresql/dialect.py` & `altimate_dataminion-0.0.8/altimate_models/postgresql/dialect.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/postgresql/profiler.py` & `altimate_dataminion-0.0.8/altimate_models/postgresql/profiler.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/postgresql/source.py` & `altimate_dataminion-0.0.8/altimate_models/postgresql/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,7 +152,15 @@
     def update_credentials(self, credentials: str):
         _user, _pass = credentials.split(":")
         self.user = _user
         self.password = _pass
 
     def override_schema(self, schema):
         return schema
+
+    def get_connect_args(self):
+        connect_args = super().get_connect_args()
+        if self.statement_timeout_in_ms is not None:
+            connect_args[
+                "options"
+            ] = f"-c statement_timeout={self.statement_timeout_in_ms}"
+        return connect_args
```

### Comparing `altimate_dataminion-0.0.7/altimate_models/s3/csv_source_dialect.py` & `altimate_dataminion-0.0.8/altimate_models/s3/csv_source_dialect.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/s3/json_source_dialect.py` & `altimate_dataminion-0.0.8/altimate_models/s3/json_source_dialect.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/s3/parquet_source_dialect.py` & `altimate_dataminion-0.0.8/altimate_models/s3/parquet_source_dialect.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/s3/profiler.py` & `altimate_dataminion-0.0.8/altimate_models/s3/profiler.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/s3/source.py` & `altimate_dataminion-0.0.8/altimate_models/s3/source.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/shared_models.py` & `altimate_dataminion-0.0.8/altimate_models/shared_models.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/snowflake/dialect.py` & `altimate_dataminion-0.0.8/altimate_models/snowflake/dialect.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/snowflake/profiler.py` & `altimate_dataminion-0.0.8/altimate_models/snowflake/profiler.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_models/snowflake/source.py` & `altimate_dataminion-0.0.8/altimate_models/snowflake/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,7 +184,15 @@
     def update_credentials(self, credentials: str):
         _user, _pass = credentials.split(":")
         self.user = _user
         self.password = _pass
 
     def override_schema(self, schema):
         return schema
+
+    def get_connect_args(self):
+        connect_args = super().get_connect_args()
+        if self.statement_timeout_in_ms is not None:
+            connect_args["session_parameters"] = {
+                "STATEMENT_TIMEOUT_IN_SECONDS": self.statement_timeout_in_ms // 1000
+            }
+        return connect_args
```

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/builders/column_metrics_query_builder.py` & `altimate_dataminion-0.0.8/altimate_profiler/builders/column_metrics_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/builders/custom_query_builder.py` & `altimate_dataminion-0.0.8/altimate_profiler/builders/custom_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/builders/metadata_query_builder.py` & `altimate_dataminion-0.0.8/altimate_profiler/builders/metadata_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/builders/performance_query_builder.py` & `altimate_dataminion-0.0.8/altimate_profiler/builders/performance_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/builders/s3_column_metrics_query_builder.py` & `altimate_dataminion-0.0.8/altimate_profiler/builders/s3_column_metrics_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/builders/s3_schema_query_builder.py` & `altimate_dataminion-0.0.8/altimate_profiler/builders/s3_schema_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/builders/s3_table_query_builder.py` & `altimate_dataminion-0.0.8/altimate_profiler/builders/s3_table_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/builders/schema_query_builder.py` & `altimate_dataminion-0.0.8/altimate_profiler/builders/schema_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/builders/table_query_builder.py` & `altimate_dataminion-0.0.8/altimate_profiler/builders/table_query_builder.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/builders/utils.py` & `altimate_dataminion-0.0.8/altimate_profiler/builders/utils.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/exceptions.py` & `altimate_dataminion-0.0.8/altimate_profiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/factory.py` & `altimate_dataminion-0.0.8/altimate_profiler/factory.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/main.py` & `altimate_dataminion-0.0.8/altimate_profiler/main.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/metrics/column_metric_type.py` & `altimate_dataminion-0.0.8/altimate_profiler/metrics/column_metric_type.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/transformer/base.py` & `altimate_dataminion-0.0.8/altimate_profiler/transformer/base.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/transformer/duckdb_schema.py` & `altimate_dataminion-0.0.8/altimate_profiler/transformer/duckdb_schema.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/transformer/metrics.py` & `altimate_dataminion-0.0.8/altimate_profiler/transformer/metrics.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/transformer/schema.py` & `altimate_dataminion-0.0.8/altimate_profiler/transformer/schema.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/validator/mappers.py` & `altimate_dataminion-0.0.8/altimate_profiler/validator/mappers.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/altimate_profiler/validator/utils.py` & `altimate_dataminion-0.0.8/altimate_profiler/validator/utils.py`

 * *Files identical despite different names*

### Comparing `altimate_dataminion-0.0.7/pyproject.toml` & `altimate_dataminion-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "altimate-dataminion"
-version = "0.0.7"
+version = "0.0.8"
 description = "Internal package. Use this at your own risk, support not guaranteed"
 authors = ["Shardul Sardesai <shardul@altimate.ai>"]
 readme = "README.md"
 packages = [{include = "altimate_profiler"}, {include = "altimate_models"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `altimate_dataminion-0.0.7/PKG-INFO` & `altimate_dataminion-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altimate-dataminion
-Version: 0.0.7
+Version: 0.0.8
 Summary: Internal package. Use this at your own risk, support not guaranteed
 Author: Shardul Sardesai
 Author-email: shardul@altimate.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

