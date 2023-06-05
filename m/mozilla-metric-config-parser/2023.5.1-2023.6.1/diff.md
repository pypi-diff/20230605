# Comparing `tmp/mozilla-metric-config-parser-2023.5.1.tar.gz` & `tmp/mozilla-metric-config-parser-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-metric-config-parser-2023.5.1.tar", last modified: Tue May  2 19:28:57 2023, max compression
+gzip compressed data, was "mozilla-metric-config-parser-2023.6.1.tar", last modified: Mon Jun  5 20:19:37 2023, max compression
```

## Comparing `mozilla-metric-config-parser-2023.5.1.tar` & `mozilla-metric-config-parser-2023.6.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:28:57.550532 mozilla-metric-config-parser-2023.5.1/
--rw-r--r--   0 root         (0) root         (0)    16725 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-05-02 19:28:57.550532 mozilla-metric-config-parser-2023.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:28:57.542532 mozilla-metric-config-parser-2023.5.1/metric_config_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/alert.py
--rw-r--r--   0 root         (0) root         (0)     7048 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/analysis.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/cli.py
--rw-r--r--   0 root         (0) root         (0)    22870 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/config.py
--rw-r--r--   0 root         (0) root         (0)     8172 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/data_source.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/definition.py
--rw-r--r--   0 root         (0) root         (0)     3493 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/dimension.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/errors.py
--rw-r--r--   0 root         (0) root         (0)     9608 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/experiment.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/exposure_signal.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/function.py
--rw-r--r--   0 root         (0) root         (0)    12463 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/metric.py
--rw-r--r--   0 root         (0) root         (0)     3130 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/metric_group.py
--rw-r--r--   0 root         (0) root         (0)     6640 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/outcome.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/parameter.py
--rw-r--r--   0 root         (0) root         (0)     3278 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/population.py
--rw-r--r--   0 root         (0) root         (0)      317 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/pre_treatment.py
--rw-r--r--   0 root         (0) root         (0)     5138 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/project.py
--rw-r--r--   0 root         (0) root         (0)     8103 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/segment.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/sql.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/statistic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:28:57.542532 mozilla-metric-config-parser-2023.5.1/metric_config_parser/templates/
--rw-r--r--   0 root         (0) root         (0)      145 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/templates/data_source_query.sql
--rw-r--r--   0 root         (0) root         (0)     2691 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/templates/metrics_query.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:28:57.546532 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5118 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:28:57.546532 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2272 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/integration/test_config_integration.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_alert.py
--rw-r--r--   0 root         (0) root         (0)    19957 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)    12702 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     9856 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_experiment.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_function.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     8522 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    11358 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_outcomes.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_population.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_project.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_sql.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/metric_config_parser/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:28:57.550532 mozilla-metric-config-parser-2023.5.1/mozilla_metric_config_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-05-02 19:28:57.000000 mozilla-metric-config-parser-2023.5.1/mozilla_metric_config_parser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1941 2023-05-02 19:28:57.000000 mozilla-metric-config-parser-2023.5.1/mozilla_metric_config_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 19:28:57.000000 mozilla-metric-config-parser-2023.5.1/mozilla_metric_config_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-02 19:28:57.000000 mozilla-metric-config-parser-2023.5.1/mozilla_metric_config_parser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-02 19:28:57.000000 mozilla-metric-config-parser-2023.5.1/mozilla_metric_config_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-02 19:28:57.000000 mozilla-metric-config-parser-2023.5.1/mozilla_metric_config_parser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-02 19:28:57.550532 mozilla-metric-config-parser-2023.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1540 2023-05-02 19:28:48.000000 mozilla-metric-config-parser-2023.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/
+-rw-r--r--   0 root         (0) root         (0)    16725 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.800196 mozilla-metric-config-parser-2023.6.1/metric_config_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/alert.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/cli.py
+-rw-r--r--   0 root         (0) root         (0)    26273 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/config.py
+-rw-r--r--   0 root         (0) root         (0)     8172 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/definition.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/dimension.py
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9608 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/exposure_signal.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/function.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/metric.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/metric_group.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/population.py
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/pre_treatment.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/project.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/segment.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/sql.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/statistic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/metric_config_parser/templates/
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/templates/data_source_query.sql
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/templates/metrics_query.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     4708 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/integration/test_config_integration.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)    19957 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    12702 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     9856 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_experiment.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_function.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_outcomes.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_population.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_sql.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-05 20:19:37.808196 mozilla-metric-config-parser-2023.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/setup.py
```

### Comparing `mozilla-metric-config-parser-2023.5.1/LICENSE` & `mozilla-metric-config-parser-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/PKG-INFO` & `mozilla-metric-config-parser-2023.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2023.5.1
+Version: 2023.6.1
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/alert.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/analysis.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/cli.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/cli.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/config.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import datetime as dt
+import shutil
+import tempfile
 from copy import deepcopy
+from datetime import datetime
 from pathlib import Path
 from typing import List, Optional, Union
 
 import attr
 import jinja2
 import toml
 from git import Repo
@@ -261,156 +264,103 @@
             spec=AnalysisSpec.from_dict(config_dict),
             last_modified=dt.datetime.fromtimestamp(path.stat().st_mtime, UTC),
             is_private=is_private,
         )
 
 
 @attr.s(auto_attribs=True)
+class Repository:
+    """Local repository config files are loaded from."""
+
+    path: Path
+    repo: Repo
+    main_branch: str
+    # indicates whether repository lives in a temporary directory that should be removed on del
+    is_tmp_repo: bool = False
+
+    def __del__(self):
+        # remove the temporary directories repos have been saved in
+        if self.is_tmp_repo:
+            git_dir = Path(self.repo.git_dir)
+            # don't delete repos that come from local directories
+            if git_dir.parent.exists():
+                shutil.rmtree(git_dir.parent)
+
+
+@attr.s(auto_attribs=True)
 class ConfigCollection:
     """
     Collection of experiment-specific configurations pulled in
     from an external GitHub repository.
     """
 
     configs: List[Config] = attr.Factory(list)
     outcomes: List[Outcome] = attr.Factory(list)
     defaults: List[DefaultConfig] = attr.Factory(list)
     definitions: List[DefinitionConfig] = attr.Factory(list)
     functions: Optional[FunctionsSpec] = None
+    repos: List[Repository] = []  # repos configs were loaded from
+    is_private: bool = False
 
     repo_url = "https://github.com/mozilla/metric-hub"
 
     @classmethod
     def from_github_repo(
         cls,
         repo_url: Optional[str] = None,
         is_private: bool = False,
         path: Optional[str] = None,
         depth: Optional[int] = None,
     ) -> "ConfigCollection":
         """Pull in external config files."""
-        # download files to tmp directory
-        with TemporaryDirectory() as tmp_dir:
-            if repo_url is not None and Path(repo_url).exists() and Path(repo_url).is_dir():
-                if path:
-                    repo = Repo(repo_url)
-                else:
-                    repo_path = Path(repo_url)
-                    dir_path = Path()
-                    depth = depth or 3
-
-                    # check if parent folder is a repository until search depth is exceeded
-                    while depth > 0:
-                        try:
-                            repo = Repo(repo_path)
-                        except InvalidGitRepositoryError:
-                            dir_path = Path(repo_path.name) / dir_path
-                            repo_path = repo_path.parent
-                            depth -= 1
-                        else:
-                            depth = 0
-
-                    repo = Repo(repo_path)
-                    path = str(dir_path)
-                    repo_url = str(repo_path)
-
-                tmp_dir = Path(repo_url)
+        # download files to a persisted tmp directory
+        tmp_dir = None
+        is_tmp_repo = False
+        if repo_url is not None and Path(repo_url).exists() and Path(repo_url).is_dir():
+            if path:
+                repo = Repo(repo_url)
             else:
-                if repo_url is not None and "/tree/" in repo_url:
-                    repo_url, tree = repo_url.split("/tree/")
-                    branch, path = tree.split("/", 1)
-                    repo = Repo.clone_from(repo_url or cls.repo_url, tmp_dir)
-                    repo.git.checkout(branch)
-                else:
-                    repo = Repo.clone_from(repo_url or cls.repo_url, tmp_dir)
-
-            external_configs = []
-
-            if path is not None:
-                tmp_dir = tmp_dir / path
-
-            for config_file in tmp_dir.glob("*.toml"):
-                last_modified = next(repo.iter_commits("HEAD", paths=config_file)).committed_date
-                config_json = toml.load(config_file)
-
-                if "project" in config_json:
-                    # opmon spec
-                    spec: DefinitionSpecSub = MonitoringSpec.from_dict(config_json)
-                else:
-                    spec = AnalysisSpec.from_dict(config_json)
-                    spec.experiment.is_private = spec.experiment.is_private or is_private
-
-                external_configs.append(
-                    Config(
-                        config_file.stem,
-                        spec,
-                        UTC.localize(dt.datetime.utcfromtimestamp(last_modified)),
-                        is_private=is_private,
-                    )
-                )
+                repo_path = Path(repo_url)
+                dir_path = Path()
+                depth = depth or 3
+
+                # check if parent folder is a repository until search depth is exceeded
+                while depth > 0:
+                    try:
+                        repo = Repo(repo_path)
+                    except InvalidGitRepositoryError:
+                        dir_path = Path(repo_path.name) / dir_path
+                        repo_path = repo_path.parent
+                        depth -= 1
+                    else:
+                        depth = 0
+
+                repo = Repo(repo_path)
+                path = str(dir_path)
+                repo_url = str(repo_path)
 
-            outcomes = []
-            for outcome_file in tmp_dir.glob(f"{OUTCOMES_DIR}/*/*.toml"):
-                commit_hash = next(repo.iter_commits("HEAD", paths=outcome_file)).hexsha
-
-                outcomes.append(
-                    Outcome(
-                        slug=outcome_file.stem,
-                        spec=OutcomeSpec.from_dict(toml.load(outcome_file)),
-                        platform=outcome_file.parent.name,
-                        commit_hash=commit_hash,
-                        is_private=is_private,
-                    )
-                )
-
-            default_configs = []
-            for default_config_file in tmp_dir.glob(f"{DEFAULTS_DIR}/*.toml"):
-                last_modified = next(
-                    repo.iter_commits("HEAD", paths=default_config_file)
-                ).committed_date
-
-                default_config_json = toml.load(default_config_file)
-
-                if "project" in default_config_json:
-                    # opmon spec
-                    spec = MonitoringSpec.from_dict(default_config_json)
-                else:
-                    spec = AnalysisSpec.from_dict(default_config_json)
-                    spec.experiment.is_private = spec.experiment.is_private or is_private
-
-                default_configs.append(
-                    DefaultConfig(
-                        default_config_file.stem,
-                        spec,
-                        UTC.localize(dt.datetime.utcfromtimestamp(last_modified)),
-                        is_private=is_private,
-                    )
-                )
-
-            definitions = []
-            for definitions_config_file in tmp_dir.glob(f"{DEFINITIONS_DIR}/*.toml"):
-                last_modified = next(
-                    repo.iter_commits("HEAD", paths=definitions_config_file)
-                ).committed_date
-
-                definitions.append(
-                    DefinitionConfig(
-                        definitions_config_file.stem,
-                        DefinitionSpec.from_dict(toml.load(definitions_config_file)),
-                        UTC.localize(dt.datetime.utcfromtimestamp(last_modified)),
-                        platform=definitions_config_file.stem,
-                        is_private=is_private,
-                    )
-                )
-
-            functions_spec = None
-            for functions_file in tmp_dir.glob(f"{DEFINITIONS_DIR}/{FUNCTIONS_FILE}"):
-                functions_spec = FunctionsSpec.from_dict(toml.load(functions_file))
+            tmp_dir = Path(repo_url)
+        else:
+            tmp_dir = Path(tempfile.mkdtemp())
+            is_tmp_repo = True
+            if repo_url is not None and "/tree/" in repo_url:
+                repo_url, tree = repo_url.split("/tree/")
+                branch, path = tree.split("/", 1)
+                repo = Repo.clone_from(repo_url or cls.repo_url, tmp_dir)
+                repo.git.checkout(branch)
+            else:
+                repo = Repo.clone_from(repo_url or cls.repo_url, tmp_dir)
 
-        return cls(external_configs, outcomes, default_configs, definitions, functions_spec)
+        return ConfigCollection.from_local_repo(
+            repo=repo,
+            path=path,
+            is_private=is_private,
+            main_branch=repo.active_branch.name,
+            is_tmp_repo=is_tmp_repo,
+        )
 
     @classmethod
     def from_github_repos(
         cls, repo_urls: Optional[List[str]] = None, is_private: bool = False
     ) -> "ConfigCollection":
         """Load configs from the provided repos."""
         if repo_urls is None or len(repo_urls) < 1:
@@ -422,14 +372,165 @@
             if configs is None:
                 configs = ConfigCollection.from_github_repo(repo, is_private=is_private)
             else:
                 collection = ConfigCollection.from_github_repo(repo, is_private=is_private)
                 configs.merge(collection)
         return configs or ConfigCollection.from_github_repo()
 
+    @classmethod
+    def from_local_repo(
+        cls, repo, path, is_private, main_branch, is_tmp_repo=False
+    ) -> "ConfigCollection":
+        """Load configs from a local repository."""
+
+        if path:
+            files_path = Path(repo.git_dir).parent / path
+        else:
+            files_path = Path(repo.git_dir).parent
+
+        external_configs = []
+        for config_file in files_path.glob("*.toml"):
+            last_modified = next(repo.iter_commits("HEAD", paths=config_file)).committed_date
+            config_json = toml.load(config_file)
+
+            if "project" in config_json:
+                # opmon spec
+                spec: DefinitionSpecSub = MonitoringSpec.from_dict(config_json)
+            else:
+                spec = AnalysisSpec.from_dict(config_json)
+                spec.experiment.is_private = spec.experiment.is_private or is_private
+
+            external_configs.append(
+                Config(
+                    config_file.stem,
+                    spec,
+                    UTC.localize(dt.datetime.utcfromtimestamp(last_modified)),
+                    is_private=is_private,
+                )
+            )
+
+        outcomes = []
+        for outcome_file in files_path.glob(f"{OUTCOMES_DIR}/*/*.toml"):
+            commit_hash = next(repo.iter_commits("HEAD", paths=outcome_file)).hexsha
+
+            outcomes.append(
+                Outcome(
+                    slug=outcome_file.stem,
+                    spec=OutcomeSpec.from_dict(toml.load(outcome_file)),
+                    platform=outcome_file.parent.name,
+                    commit_hash=commit_hash,
+                    is_private=is_private,
+                )
+            )
+
+        default_configs = []
+        for default_config_file in files_path.glob(f"{DEFAULTS_DIR}/*.toml"):
+            last_modified = next(
+                repo.iter_commits("HEAD", paths=default_config_file)
+            ).committed_date
+
+            default_config_json = toml.load(default_config_file)
+
+            if "project" in default_config_json:
+                # opmon spec
+                spec = MonitoringSpec.from_dict(default_config_json)
+            else:
+                spec = AnalysisSpec.from_dict(default_config_json)
+                spec.experiment.is_private = spec.experiment.is_private or is_private
+
+            default_configs.append(
+                DefaultConfig(
+                    default_config_file.stem,
+                    spec,
+                    UTC.localize(dt.datetime.utcfromtimestamp(last_modified)),
+                    is_private=is_private,
+                )
+            )
+
+        definitions = []
+        for definitions_config_file in files_path.glob(f"{DEFINITIONS_DIR}/*.toml"):
+            last_modified = next(
+                repo.iter_commits("HEAD", paths=definitions_config_file)
+            ).committed_date
+
+            definitions.append(
+                DefinitionConfig(
+                    definitions_config_file.stem,
+                    DefinitionSpec.from_dict(toml.load(definitions_config_file)),
+                    UTC.localize(dt.datetime.utcfromtimestamp(last_modified)),
+                    platform=definitions_config_file.stem,
+                    is_private=is_private,
+                )
+            )
+
+        functions_spec = None
+        for functions_file in files_path.glob(f"{DEFINITIONS_DIR}/{FUNCTIONS_FILE}"):
+            functions_spec = FunctionsSpec.from_dict(toml.load(functions_file))
+
+        return cls(
+            external_configs,
+            outcomes,
+            default_configs,
+            definitions,
+            functions_spec,
+            repos=[
+                Repository(repo=repo, path=path, main_branch=main_branch, is_tmp_repo=is_tmp_repo)
+            ],
+            is_private=is_private,
+        )
+
+    def as_of(self, timestamp: datetime) -> "ConfigCollection":
+        """Get configs as they were at the provided timestamp."""
+        config_collection = None
+
+        # configs can be loaded from multiple different repos
+        for repo in self.repos:
+            # copy the original repo to a temporary path were we can go back in history
+            with TemporaryDirectory() as tmp_dir:
+                git_dir = Path(repo.repo.git_dir)
+                shutil.copytree(git_dir.parent, tmp_dir, dirs_exist_ok=True)
+                tmp_repo = Repo(tmp_dir)
+
+                # find the commit that got added just before the `timestamp`
+                rev = "HEAD"  # use the HEAD commit by default if no other commits exist
+
+                # make sure the most recent commit is checked out by checking out the main branch
+                tmp_repo.git.checkout(repo.main_branch)
+
+                # start iterating through all commits starting at HEAD
+                for commit in tmp_repo.iter_commits("HEAD"):
+                    # check if the commit timestamp is older than the reference timestamp
+                    if commit.committed_datetime <= timestamp:
+                        rev = commit.hexsha
+                        break
+
+                if commit:
+                    # if there is no commit that is older than the reference timestamp,
+                    # use the oldest commit that we could find (= last commit)
+                    rev = commit.hexsha
+
+                # checkout that commit
+                tmp_repo.git.checkout(rev)
+
+                # load configs as they were at the time of the commit
+                configs = self.from_local_repo(
+                    tmp_repo, repo.path, self.is_private, repo.main_branch, is_tmp_repo=True
+                )
+                configs.repos = [repo]  # point to the original repo, instead of the temporary one
+
+                if config_collection is None:
+                    config_collection = configs
+                else:
+                    config_collection.merge(configs)
+
+        if config_collection is None:
+            return self
+
+        return config_collection
+
     def spec_for_outcome(self, slug: str, platform: str) -> Optional[OutcomeSpec]:
         """Return the spec for a specific outcome"""
         for outcome in self.outcomes:
             if outcome.slug == slug and outcome.platform == platform:
                 return outcome.spec
 
         return None
@@ -614,7 +715,9 @@
             if slug not in slugs:
                 functions[slug] = function
 
         if self.functions is None:
             self.functions = FunctionsSpec(functions=functions)
         else:
             self.functions.functions = functions
+
+        self.repos += other.repos
```

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/data_source.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/data_source.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/definition.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/definition.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/dimension.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/dimension.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/errors.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/experiment.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/exposure_signal.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/function.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/metric.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/metric_group.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/metric_group.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/monitoring.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/outcome.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/outcome.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/parameter.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/parameter.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/population.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/project.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/segment.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/segment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/sql.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/templates/metrics_query.sql` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/templates/metrics_query.sql`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/conftest.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_alert.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_analysis.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_config.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_experiment.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_function.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_metric.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_monitoring.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_outcomes.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_population.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_project.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/tests/test_sql.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/metric_config_parser/util.py` & `mozilla-metric-config-parser-2023.6.1/metric_config_parser/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 @contextmanager
 def TemporaryDirectory():
     name = Path(tempfile.mkdtemp())
     try:
         yield name
     finally:
-        shutil.rmtree(name)
+        if name.exists():
+            shutil.rmtree(name)
 
 
 def parse_date(yyyy_mm_dd: Optional[str]) -> Optional[datetime]:
     if not yyyy_mm_dd:
         return None
     return datetime.strptime(yyyy_mm_dd, "%Y-%m-%d").replace(tzinfo=pytz.utc)
```

### Comparing `mozilla-metric-config-parser-2023.5.1/mozilla_metric_config_parser.egg-info/PKG-INFO` & `mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2023.5.1
+Version: 2023.6.1
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `mozilla-metric-config-parser-2023.5.1/mozilla_metric_config_parser.egg-info/SOURCES.txt` & `mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.5.1/setup.py` & `mozilla-metric-config-parser-2023.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,9 +60,9 @@
     long_description=text_from_file("README.md"),
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     entry_points="""
         [console_scripts]
         metric-config-parser=metric_config_parser.cli:cli
     """,
-    version="2023.5.1",
+    version="2023.6.1",
 )
```

