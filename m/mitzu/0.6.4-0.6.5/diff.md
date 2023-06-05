# Comparing `tmp/mitzu-0.6.4.tar.gz` & `tmp/mitzu-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.4.tar", max compression
+gzip compressed data, was "mitzu-0.6.5.tar", max compression
```

## Comparing `mitzu-0.6.4.tar` & `mitzu-0.6.5.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0     1082 2023-06-04 08:51:48.002334 mitzu-0.6.4/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-06-04 08:51:48.002334 mitzu-0.6.4/README.md
--rw-r--r--   0        0        0     6148 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/.DS_Store
--rw-r--r--   0        0        0      752 2023-06-04 08:52:43.019065 mitzu-0.6.4/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1918 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5148 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6262 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/bigquery_adapter.py
--rw-r--r--   0        0        0     6026 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2533 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     3765 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3298 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/__init__.py
--rw-r--r--   0        0        0     2146 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2412 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
--rw-r--r--   0        0        0     5071 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
--rw-r--r--   0        0        0     4770 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
--rw-r--r--   0        0        0    38550 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     8638 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
--rw-r--r--   0        0        0     9854 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
--rw-r--r--   0        0        0     7361 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
--rw-r--r--   0        0        0     1131 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    40105 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     4963 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     7705 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1835 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/helper.py
--rw-r--r--   0        0        0    53055 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6845 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     2550 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2102 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11933 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7305 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7802 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3289 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1222 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    20802 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/bigquery.png
--rw-r--r--   0        0        0    10321 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    15538 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1305 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7481 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2920 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     1664 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     3432 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4984 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8631 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/model.py
--rw-r--r--   0        0        0      309 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     5435 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    22704 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4428 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    20561 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9628 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/dashboards_page.py
--rw-r--r--   0        0        0    14456 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5929 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5790 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    22007 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10100 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10916 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2382 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1553 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0    10285 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1221 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1751 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     3947 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     5023 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1288 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10095 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11845 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0     9470 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1738 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    35694 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     5090 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3114 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     1955 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     4974 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0      670 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/notification_service.py
--rw-r--r--   0        0        0     2105 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     6708 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/tracking_service.py
--rw-r--r--   0        0        0     4755 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    24085 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25095 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0     4700 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     3422 2023-06-04 08:52:43.015064 mitzu-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-05 05:54:25.801503 mitzu-0.6.5/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-06-05 05:54:25.801503 mitzu-0.6.5/README.md
+-rw-r--r--   0        0        0     6148 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/.DS_Store
+-rw-r--r--   0        0        0      752 2023-06-05 05:55:20.310352 mitzu-0.6.5/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1918 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5148 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6262 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/bigquery_adapter.py
+-rw-r--r--   0        0        0     6026 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2533 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     3765 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3298 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-06-05 05:54:26.197508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/__init__.py
+-rw-r--r--   0        0        0     2146 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2412 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
+-rw-r--r--   0        0        0     5071 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
+-rw-r--r--   0        0        0     4770 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
+-rw-r--r--   0        0        0    38550 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     8638 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
+-rw-r--r--   0        0        0     9854 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
+-rw-r--r--   0        0        0     7361 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0     1131 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    40105 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     4963 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     7705 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1835 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/helper.py
+-rw-r--r--   0        0        0    53055 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6845 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     2550 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2102 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11933 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7305 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7802 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3289 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1222 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    20802 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/bigquery.png
+-rw-r--r--   0        0        0    10321 2023-06-05 05:54:26.201508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    15538 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1305 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7481 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2920 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     1664 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3432 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4984 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8631 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      309 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5435 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    22704 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4428 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    20561 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9628 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/dashboards_page.py
+-rw-r--r--   0        0        0    14456 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5929 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5790 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    22094 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10100 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10698 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2382 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1553 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0    10285 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1221 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1751 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     3947 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     5023 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1288 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10095 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11845 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0     9470 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1738 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    35694 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5090 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3114 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     1955 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     4974 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0      670 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/service/notification_service.py
+-rw-r--r--   0        0        0     2105 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     6708 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/service/tracking_service.py
+-rw-r--r--   0        0        0     4755 2023-06-05 05:54:26.205508 mitzu-0.6.5/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    24085 2023-06-05 05:54:26.209508 mitzu-0.6.5/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25095 2023-06-05 05:54:26.209508 mitzu-0.6.5/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0     4700 2023-06-05 05:54:26.209508 mitzu-0.6.5/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     3422 2023-06-05 05:55:20.310352 mitzu-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.5/PKG-INFO
```

### Comparing `mitzu-0.6.4/LICENSE.txt` & `mitzu-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/README.md` & `mitzu-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/.DS_Store` & `mitzu-0.6.5/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/__init__.py` & `mitzu-0.6.5/mitzu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.4"
+__version__ = "0.6.5"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.4/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.5/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.5/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/bigquery_adapter.py` & `mitzu-0.6.5/mitzu/adapters/bigquery_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.5/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/file_adapter.py` & `mitzu-0.6.5/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.5/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/helper.py` & `mitzu-0.6.5/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.5/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.5/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.5/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.5/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.5/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.5/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.5/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/helper.py` & `mitzu-0.6.5/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/model.py` & `mitzu-0.6.5/mitzu/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/notebook/model_loader.py` & `mitzu-0.6.5/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/project_discovery.py` & `mitzu-0.6.5/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/project_serialization.py` & `mitzu-0.6.5/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/samples/__init__.py` & `mitzu-0.6.5/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/samples/data_ingestion.py` & `mitzu-0.6.5/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.5/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/serialization.py` & `mitzu-0.6.5/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/visualization/charts.py` & `mitzu-0.6.5/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/visualization/common.py` & `mitzu-0.6.5/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/visualization/labels.py` & `mitzu-0.6.5/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/visualization/plot.py` & `mitzu-0.6.5/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/visualization/titles.py` & `mitzu-0.6.5/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/visualization/tooltips.py` & `mitzu-0.6.5/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/visualization/transform_conv.py` & `mitzu-0.6.5/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/visualization/transform_retention.py` & `mitzu-0.6.5/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/.DS_Store` & `mitzu-0.6.5/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.5/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.5/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/logo.png` & `mitzu-0.6.5/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.5/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/bigquery.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/bigquery.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.5/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.5/mitzu/webapp/auth/authorizer.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.5/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.5/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/auth/google.py` & `mitzu-0.6.5/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/cache.py` & `mitzu-0.6.5/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.5/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/configs.py` & `mitzu-0.6.5/mitzu/webapp/configs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/dependencies.py` & `mitzu-0.6.5/mitzu/webapp/dependencies.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/helper.py` & `mitzu-0.6.5/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/model.py` & `mitzu-0.6.5/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/offcanvas.py` & `mitzu-0.6.5/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.5/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.5/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.5/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/dashboards_page.py` & `mitzu-0.6.5/mitzu/webapp/pages/dashboards_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.5/mitzu/webapp/pages/edit_user.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore/explore_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import mitzu.webapp.storage as S
 from mitzu.webapp.helper import MITZU_LOCATION, find_event_field_def, CHILDREN
 import mitzu.webapp.pages.paths as P
 import traceback
 from dash import ctx, html, callback, no_update, dcc
 from dash.dependencies import ALL, Input, Output, State
 from mitzu.webapp.auth.decorator import restricted
+import mitzu.webapp.configs as C
 import flask
 
 from mitzu.webapp.helper import (
     get_final_all_inputs,
 )
 
 NAVBAR_ID = "explore_navbar"
@@ -108,15 +109,16 @@
 
 
 def share_button_navbar_provider(
     id: str, show_share_button=False, path="", **kwargs
 ) -> Optional[bc.Component]:
     if not show_share_button:
         return None
-    url = flask.request.host_url.strip("/") + path
+    host_url = C.HOME_URL if C.HOME_URL else flask.request.host_url
+    url = host_url.strip("/") + path
     return (
         dbc.Button(
             [
                 html.B(className="bi bi-link-45deg"),
                 " Share",
                 dcc.Clipboard(
                     id=CLIPBOARD,
@@ -330,15 +332,15 @@
         discovered_project, all_inputs, metric_type
     )
     metric: Optional[M.Metric] = None
     if metric_type == MTH.MetricType.FUNNEL:
         if len(segments) >= 1:
             metric = M.Conversion(segments)
     elif metric_type == MTH.MetricType.SEGMENTATION:
-        if len(segments) == 1:
+        if len(segments) >= 1:
             metric = segments[0]
     elif metric_type == MTH.MetricType.RETENTION:
         if len(segments) == 2:
             metric = segments[0] >= segments[1]
         elif len(segments) == 1:
             metric = segments[0] >= segments[0]
```

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -264,51 +264,46 @@
         elif metric_type == M.MetricType.RETENTION:
             agg_type, agg_param = M.AggType.RETENTION_RATE, None
         else:
             raise UnsupportedOperation(f"Unsupported Metric Type : {metric_type}")
     else:
         agg_type, agg_param = M.AggType.parse_agg_str(agg_type_val)
 
+    dates_conf = DS.from_all_inputs(discovered_project, all_inputs)
+    time_group = dates_conf.time_group
+    lookback_days = dates_conf.lookback_days
+    start_dt = dates_conf.start_dt
+    end_dt = dates_conf.end_dt
+    resolution = M.Resolution.parse(
+        all_inputs.get(RESOLUTION_DD, M.Resolution.EVERY_EVENT.name)
+    )
+    chart_type_val = all_inputs.get(TH.CHART_TYPE_DD, None)
+    chart_type = M.SimpleChartType.parse(chart_type_val)
+
     if ctx.triggered_id == MTH.METRIC_TYPE_DROPDOWN:
-        start_dt = None
-        end_dt = None
         if metric_type == MTH.MetricType.RETENTION:
-            time_group = M.TimeGroup.WEEK
-            resolution = M.Resolution.ONE_USER_EVENT_PER_MINUTE
-            lookback_days = M.TimeWindow(2, M.TimeGroup.MONTH)
-            time_window = M.TimeWindow(1, M.TimeGroup.WEEK)
+            rtw = M.TimeGroup.WEEK
+            time_window = M.TimeWindow(1, rtw)
+            time_group = M.TimeGroup.TOTAL
+            if resolution == M.Resolution.EVERY_EVENT:
+                # Makes sure cluster doesn't break
+                resolution = M.Resolution.ONE_USER_EVENT_PER_MINUTE
+            chart_type = M.SimpleChartType.LINE
         elif metric_type == MTH.MetricType.FUNNEL:
-            time_group = M.TimeGroup.DAY
-            resolution = M.Resolution.EVERY_EVENT
-            lookback_days = M.TimeWindow(1, M.TimeGroup.MONTH)
-            time_window = M.TimeWindow(1, M.TimeGroup.DAY)
+            time_window = M.TimeWindow(1, M.TimeGroup.WEEK)
         else:
-            time_group = M.TimeGroup.DAY
             resolution = M.Resolution.EVERY_EVENT
-            lookback_days = M.TimeWindow(1, M.TimeGroup.MONTH)
             time_window = M.TimeWindow(1, M.TimeGroup.DAY)
     else:
-        dates_conf = DS.from_all_inputs(discovered_project, all_inputs)
-        time_group = dates_conf.time_group
-        resolution = M.Resolution.parse(
-            all_inputs.get(RESOLUTION_DD, M.Resolution.EVERY_EVENT.name)
-        )
-        lookback_days = dates_conf.lookback_days
-        start_dt = dates_conf.start_dt
-        end_dt = dates_conf.end_dt
         time_window = M.TimeWindow(
             value=all_inputs.get(TIME_WINDOW_INTERVAL, 1),
             period=M.TimeGroup(
                 all_inputs.get(TIME_WINDOW_INTERVAL_STEPS, M.TimeGroup.DAY)
             ),
         )
-
-    chart_type_val = all_inputs.get(TH.CHART_TYPE_DD, None)
-    chart_type = M.SimpleChartType.parse(chart_type_val)
-
     res_config = M.MetricConfig(
         start_dt=parse_datetime_input(start_dt, None),
         end_dt=parse_datetime_input(end_dt, None),
         lookback_days=lookback_days,
         time_group=time_group,
         agg_type=agg_type,
         agg_param=agg_param,
```

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.5/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/home.py` & `mitzu-0.6.5/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/login.py` & `mitzu-0.6.5/mitzu/webapp/pages/login.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.5/mitzu/webapp/pages/manage_connection.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.5/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.5/mitzu/webapp/pages/manage_event_defs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.5/mitzu/webapp/pages/manage_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.5/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/paths.py` & `mitzu-0.6.5/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.5/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.5/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.5/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.5/mitzu/webapp/pages/projects_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/pages/users.py` & `mitzu-0.6.5/mitzu/webapp/pages/users.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/service/events_service.py` & `mitzu-0.6.5/mitzu/webapp/service/events_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.5/mitzu/webapp/service/navbar_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/service/notification_service.py` & `mitzu-0.6.5/mitzu/webapp/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.5/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/service/tracking_service.py` & `mitzu-0.6.5/mitzu/webapp/service/tracking_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/service/user_service.py` & `mitzu-0.6.5/mitzu/webapp/service/user_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/storage.py` & `mitzu-0.6.5/mitzu/webapp/storage.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/storage_model.py` & `mitzu-0.6.5/mitzu/webapp/storage_model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/mitzu/webapp/webapp.py` & `mitzu-0.6.5/mitzu/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.4/pyproject.toml` & `mitzu-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.4"
+version = "0.6.5"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.4/PKG-INFO` & `mitzu-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.4
+Version: 0.6.5
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

