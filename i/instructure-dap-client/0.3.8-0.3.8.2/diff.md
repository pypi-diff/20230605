# Comparing `tmp/instructure-dap-client-0.3.8.tar.gz` & `tmp/instructure-dap-client-0.3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructure-dap-client-0.3.8.tar", last modified: Thu May 11 13:18:16 2023, max compression
+gzip compressed data, was "instructure-dap-client-0.3.8.2.tar", last modified: Mon Jun  5 14:39:23 2023, max compression
```

## Comparing `instructure-dap-client-0.3.8.tar` & `instructure-dap-client-0.3.8.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.039677 instructure-dap-client-0.3.8/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1079 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19535 2023-05-11 13:18:16.039974 instructure-dap-client-0.3.8/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18685 2023-04-29 10:55:22.000000 instructure-dap-client-0.3.8/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.011392 instructure-dap-client-0.3.8/dap/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      524 2023-05-11 13:17:51.000000 instructure-dap-client-0.3.8/dap/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4416 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8/dap/__main__.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.014308 instructure-dap-client-0.3.8/dap/actions/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/actions/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1064 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.8/dap/actions/drop_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      572 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.8/dap/actions/init_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      573 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.8/dap/actions/sync_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    21450 2023-05-11 13:12:25.000000 instructure-dap-client-0.3.8/dap/api.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2980 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.8/dap/arguments.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.022678 instructure-dap-client-0.3.8/dap/commands/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8/dap/commands/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      491 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8/dap/commands/abstract_db_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2011 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/base.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6751 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.8/dap/commands/commands.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2611 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.8/dap/commands/commonargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      502 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/dbargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1175 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/dropdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1361 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/initdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/queryargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1695 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/syncdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      889 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/timestampargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5928 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.8/dap/concurrency.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6428 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8/dap/conversion_common.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      635 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/conversion_nonperf.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      701 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/conversion_perf.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3261 2023-05-11 13:12:25.000000 instructure-dap-client-0.3.8/dap/dap_error.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18466 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8/dap/dap_types.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.028488 instructure-dap-client-0.3.8/dap/database/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/database/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2318 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/database/base_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2442 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.8/dap/database/connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1121 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.8/dap/database/database_errors.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3835 2023-04-19 07:03:02.000000 instructure-dap-client-0.3.8/dap/database/database_operations.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2751 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/database/init_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3671 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/database/sync_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5861 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8/dap/downloader.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      684 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8/dap/log.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.031249 instructure-dap-client-0.3.8/dap/model/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8/dap/model/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      987 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8/dap/model/ddl.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    16280 2023-05-07 19:02:41.000000 instructure-dap-client-0.3.8/dap/model/meta_table.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7091 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8/dap/model/metadata.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      932 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8/dap/networking.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1353 2023-04-05 14:04:38.000000 instructure-dap-client-0.3.8/dap/payload.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-25 19:15:30.000000 instructure-dap-client-0.3.8/dap/py.typed
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.032922 instructure-dap-client-0.3.8/dap/replicator/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 14:59:52.000000 instructure-dap-client-0.3.8/dap/replicator/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2571 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/replicator/sql.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1355 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8/dap/timer.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1450 2023-03-27 20:20:03.000000 instructure-dap-client-0.3.8/dap/timestamp.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.039004 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19535 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1408 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       51 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/entry_points.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      153 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-05-11 13:17:30.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/zip-safe
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-04-25 19:13:58.000000 instructure-dap-client-0.3.8/pyproject.toml
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1254 2023-05-11 13:18:16.041196 instructure-dap-client-0.3.8/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-07-21 14:42:23.000000 instructure-dap-client-0.3.8/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.738480 instructure-dap-client-0.3.8.2/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1079 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8.2/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19537 2023-06-05 14:39:23.738777 instructure-dap-client-0.3.8.2/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18685 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.710516 instructure-dap-client-0.3.8.2/dap/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      526 2023-06-05 14:38:28.000000 instructure-dap-client-0.3.8.2/dap/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4682 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/__main__.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.713461 instructure-dap-client-0.3.8.2/dap/actions/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8.2/dap/actions/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1064 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/actions/drop_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      572 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/actions/init_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      573 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/actions/sync_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    21555 2023-06-01 21:13:57.000000 instructure-dap-client-0.3.8.2/dap/api.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2997 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/arguments.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.722763 instructure-dap-client-0.3.8.2/dap/commands/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8.2/dap/commands/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      491 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/commands/abstract_db_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2011 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8.2/dap/commands/base.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6751 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.8.2/dap/commands/commands.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2842 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/commands/commonargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      502 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8.2/dap/commands/dbargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1119 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/commands/dropdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1370 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/commands/initdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8.2/dap/commands/queryargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1704 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/commands/syncdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      889 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8.2/dap/commands/timestampargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5928 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.8.2/dap/concurrency.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8018 2023-06-05 14:37:38.000000 instructure-dap-client-0.3.8.2/dap/conversion_common.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      635 2023-06-01 13:11:03.000000 instructure-dap-client-0.3.8.2/dap/conversion_nonperf.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      701 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8.2/dap/conversion_perf.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3688 2023-06-01 21:13:57.000000 instructure-dap-client-0.3.8.2/dap/dap_error.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18466 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8.2/dap/dap_types.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.728778 instructure-dap-client-0.3.8.2/dap/database/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2318 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/base_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2442 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1121 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/database_errors.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3835 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/database_operations.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2751 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/init_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3671 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/sync_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5861 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/downloader.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      684 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8.2/dap/log.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.731267 instructure-dap-client-0.3.8.2/dap/model/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8.2/dap/model/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      987 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/model/ddl.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    16280 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/model/meta_table.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7091 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8.2/dap/model/metadata.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      932 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8.2/dap/networking.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1353 2023-04-05 14:04:38.000000 instructure-dap-client-0.3.8.2/dap/payload.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-25 19:15:30.000000 instructure-dap-client-0.3.8.2/dap/py.typed
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.732664 instructure-dap-client-0.3.8.2/dap/replicator/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 14:59:52.000000 instructure-dap-client-0.3.8.2/dap/replicator/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2571 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/replicator/sql.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1355 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8.2/dap/timer.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2264 2023-06-05 14:37:38.000000 instructure-dap-client-0.3.8.2/dap/timestamp.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.737695 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19537 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1408 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       51 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/entry_points.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      153 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/zip-safe
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-04-25 19:13:58.000000 instructure-dap-client-0.3.8.2/pyproject.toml
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1254 2023-06-05 14:39:23.739981 instructure-dap-client-0.3.8.2/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-07-21 14:42:23.000000 instructure-dap-client-0.3.8.2/setup.py
```

### Comparing `instructure-dap-client-0.3.8/LICENSE` & `instructure-dap-client-0.3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/PKG-INFO` & `instructure-dap-client-0.3.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructure-dap-client
-Version: 0.3.8
+Version: 0.3.8.2
 Summary: Data Access Platform client library
 Author: Levente Hunyadi
 Author-email: levente.hunyadi@instructure.com
 Maintainer: Edina Tipter
 Maintainer-email: edina.tipter@instructure.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `instructure-dap-client-0.3.8/README.md` & `instructure-dap-client-0.3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/__init__.py` & `instructure-dap-client-0.3.8.2/dap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 Data Access Platform Client Library.
 
 Data Access Platform (DAP) acts as a single source of data for analytics at Instructure. It provides efficient access
 to data collected across various educational products in bulk with high fidelity and low latency, adhering to
 a canonical data model.
 """
 
-__version__ = "0.3.8"
+__version__ = "0.3.8.2"
 __author__ = "Levente Hunyadi"
 __copyright__ = "Copyright 2022-2023, Instructure, Inc."
 __license__ = "MIT"
 __maintainer__ = "Edina Tipter"
 __email__ = "edina.tipter@instructure.com"
 __status__ = "Beta"
```

### Comparing `instructure-dap-client-0.3.8/dap/__main__.py` & `instructure-dap-client-0.3.8.2/dap/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,20 +104,28 @@
     if parser:
         parser.parse_args(namespace=args)
 
     logging.basicConfig(level=getattr(logging, args.loglevel.upper(), logging.INFO))
     logger = logging.getLogger("dap")
     logger.propagate = False
     handler = logging.StreamHandler()
+    
     default_format = "%(asctime)s - %(levelname)s - %(message)s"
     debug_format = default_format + " (%(filename)s:%(lineno)d)"
     handler.setFormatter(
         LevelFormatter({logging.DEBUG: debug_format, logging.INFO: default_format})
     )
+    if args.logfile:
+        file_handler = logging.FileHandler(args.logfile, "a")
+        file_handler.setFormatter(
+            LevelFormatter({logging.DEBUG: debug_format, logging.INFO: default_format})
+        )
+        logger.addHandler(file_handler)
     logger.addHandler(handler)
+    
 
     asyncio.run(dapCommand.execute(args))
 
 
 def console_entry() -> None:
     logger = logging.getLogger("dap")
```

### Comparing `instructure-dap-client-0.3.8/dap/actions/drop_db.py` & `instructure-dap-client-0.3.8.2/dap/actions/drop_db.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/actions/init_db.py` & `instructure-dap-client-0.3.8.2/dap/actions/init_db.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/actions/sync_db.py` & `instructure-dap-client-0.3.8.2/dap/actions/sync_db.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/api.py` & `instructure-dap-client-0.3.8.2/dap/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 import aiofiles
 import aiohttp
 import jwt
 from strong_typing.serialization import json_dump_string, json_to_object, object_to_json
 
 from . import __version__
 from .dap_error import (
+    AccountDisabledError,
     AccountNotOnboardedError,
     AuthenticationError,
     NotFoundError,
     OutOfRangeError,
     ProcessingError,
     ServerError,
-    AccountDisabledError,
+    SnapshotRequiredError,
     ValidationError,
 )
 from .dap_types import (
     CompleteIncrementalJob,
     CompleteSnapshotJob,
     Credentials,
     DownloadTableDataResult,
@@ -189,14 +190,15 @@
 
     def _map_to_error_type(
         self, status_code: int, response_body: Any
     ) -> Union[
         ValidationError,
         NotFoundError,
         OutOfRangeError,
+        SnapshotRequiredError,
         AuthenticationError,
         AccountDisabledError,
         AccountNotOnboardedError,
         ProcessingError,
         ServerError,
     ]:
         """
@@ -217,14 +219,15 @@
                 )
             else:
                 return json_to_object(
                     Union[  # type: ignore
                         ValidationError,
                         NotFoundError,
                         OutOfRangeError,
+                        SnapshotRequiredError,
                         ProcessingError,
                     ],
                     response_body_error,
                 )
         except:
             return ServerError(response_body_error)
```

### Comparing `instructure-dap-client-0.3.8/dap/arguments.py` & `instructure-dap-client-0.3.8.2/dap/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         return EnvironmentDefault(var, **kwargs)
 
     return _environment_default
 
 
 class Arguments(argparse.Namespace):
     loglevel: str
+    logfile: str
 
     base_url: str
     client_id: str
     client_secret: str
 
     connection_string: str
```

### Comparing `instructure-dap-client-0.3.8/dap/commands/base.py` & `instructure-dap-client-0.3.8.2/dap/commands/base.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/commands/commands.py` & `instructure-dap-client-0.3.8.2/dap/commands/commands.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/commands/commonargs.py` & `instructure-dap-client-0.3.8.2/dap/commands/commonargs.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 
 
 class OAuthCredentialsArgumentRegistrar(ArgumentRegistrar):
     def register(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "--client-id",
             metavar="ClientID",
-            help="OAuth Client ID",
+            help="OAuth client ID obtained from the Identity Service.",
             action=environment_default("DAP_CLIENT_ID"),  # type: ignore
         )
 
         parser.add_argument(
             "--client-secret",
             metavar="ClientSecret",
-            help="OAuth Client Secret",
+            help="OAuth client secret obtained from the Identity Service.",
             action=environment_default("DAP_CLIENT_SECRET"),  # type: ignore
         )
 
 
 class LogLevelArgumentRegistrar(ArgumentRegistrar):
     def register(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
@@ -72,14 +72,19 @@
                     logging.ERROR,
                     logging.CRITICAL,
                 )
             ],
             default=log_level_name(logging.INFO),
             help="Sets log verbosity.",
         )
+        parser.add_argument(
+            "--logfile",
+            metavar="LogFile",
+            help="Sets the path of the file to save logs to.",
+        )
 
 
 class HelpArgumentRegistrar(ArgumentRegistrar):
     def register(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
-            "--help", "-h", action=_HelpAction, help="show this help message and exit"
+            "--help", "-h", action=_HelpAction, help="Show this help message and exit."
         )
```

### Comparing `instructure-dap-client-0.3.8/dap/commands/dropdb_command.py` & `instructure-dap-client-0.3.8.2/dap/commands/dropdb_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def _create_parser(
         self, subparsers: Optional[argparse._SubParsersAction]
     ) -> Optional[argparse.ArgumentParser]:
         if subparsers is not None:
             return subparsers.add_parser(
                 "dropdb",
-                help="Drops the given table from the DB that was previously created with the 'initdb' command.",
+                help="Drops a table from the database.",
                 formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             )
         else:
             return None
 
     def _can_execute_impl(self, args: Arguments) -> bool:
         return args.command == "dropdb"
```

### Comparing `instructure-dap-client-0.3.8/dap/commands/initdb_command.py` & `instructure-dap-client-0.3.8.2/dap/commands/initdb_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def _create_parser(
         self, subparsers: Optional[argparse._SubParsersAction]
     ) -> Optional[argparse.ArgumentParser]:
         if subparsers is not None:
             return subparsers.add_parser(
                 "initdb",
-                help="Performs a snapshot query of a table and sends the result into a DB.",
+                help="Performs a snapshot query of a table and persists the result in the database.",
                 formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             )
         else:
             return None
 
     def _can_execute_impl(self, args: Arguments) -> bool:
         return args.command == "initdb"
```

### Comparing `instructure-dap-client-0.3.8/dap/commands/queryargs.py` & `instructure-dap-client-0.3.8.2/dap/commands/queryargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/commands/syncdb_command.py` & `instructure-dap-client-0.3.8.2/dap/commands/syncdb_command.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def _create_parser(
         self, subparsers: Optional[argparse._SubParsersAction]
     ) -> Optional[argparse.ArgumentParser]:
         if subparsers is not None:
             return subparsers.add_parser(
                 "syncdb",
-                help="Performs an incremental query of a table and sends the result into a DB.",
+                help="Performs an incremental query of a table and persists the result in the database.",
                 formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             )
         else:
             return None
 
     def _can_execute_impl(self, args: Arguments) -> bool:
         return args.command == "syncdb"
```

### Comparing `instructure-dap-client-0.3.8/dap/commands/timestampargs.py` & `instructure-dap-client-0.3.8.2/dap/commands/timestampargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/concurrency.py` & `instructure-dap-client-0.3.8.2/dap/concurrency.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/conversion_common.py` & `instructure-dap-client-0.3.8.2/dap/conversion_common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,41 @@
+import logging
+import typing
+from datetime import datetime
 from typing import Any, Callable, Dict, Optional, Type, TypeVar
 
 import orjson
 from sqlalchemy import ARRAY, JSON, TIMESTAMP, BigInteger, Boolean, Column, Double
 from sqlalchemy import Enum as SqlEnum
 from sqlalchemy import Float, Integer, SmallInteger, String
 from sqlalchemy.sql.type_api import TypeEngine
 from strong_typing.core import JsonType
 
-from .timestamp import valid_naive_datetime
+from .timestamp import clamp_naive_datetime, valid_naive_datetime
 
 T = TypeVar("T")
 
+logger = logging.getLogger("dap")
+
 JsonRecord = Dict[str, Dict[str, JsonType]]
+DateTimeConverter = Callable[[str], datetime]
 JsonTypeCast = Callable[[JsonType], Any]
 RecordExtractor = Callable[[JsonRecord], Any]
 
 
+def _handle_exceptional_datetime(record_json: JsonRecord, column_name: str) -> datetime:
+    key = record_json["key"]
+    value = typing.cast(str, record_json["value"][column_name])
+    clamped_value = clamp_naive_datetime(value)
+    logger.warning(
+        f"Timestamp format error encountered in record {key}: {value} converted to {clamped_value}"
+    )
+    return clamped_value
+
+
 def _get_primary_extractor(
     column_name: str, type_cast: Optional[JsonTypeCast]
 ) -> RecordExtractor:
     """
     Helps extract a value to be inserted into a primary key column.
 
     :returns: A lambda function that extracts the value from a JSON record.
@@ -29,40 +45,69 @@
         return lambda record_json: record_json["key"][column_name]
     else:
         cast = type_cast  # hint to type checker
         return lambda record_json: cast(record_json["key"][column_name])
 
 
 def _get_required_extractor(
-    column_name: str, type_cast: Optional[JsonTypeCast]
+    column_name: str,
+    column_type: Type[TypeEngine],
+    type_cast: Optional[JsonTypeCast],
 ) -> RecordExtractor:
     """
     Helps extract a required value to be inserted into a non-nullable column.
 
     :returns: A lambda function that extracts the value from a JSON record.
     """
 
     if type_cast is None:
         return lambda record_json: record_json["value"][column_name]
+    elif column_type is TIMESTAMP:
+        cast = type_cast  # hint to type checker
+
+        def _get_required_timestamp_value(record_json: JsonRecord) -> datetime:
+            value = record_json["value"][column_name]
+            try:
+                return cast(value)
+            except ValueError:
+                return _handle_exceptional_datetime(record_json, column_name)
+
+        return _get_required_timestamp_value
     else:
         cast = type_cast  # hint to type checker
         return lambda record_json: cast(record_json["value"][column_name])
 
 
 def _get_optional_extractor(
-    column_name: str, type_cast: Optional[JsonTypeCast]
+    column_name: str, column_type: Type[TypeEngine], type_cast: Optional[JsonTypeCast]
 ) -> RecordExtractor:
     """
     Helps extract an optional value to be inserted into a nullable column.
 
     :returns: A lambda function that extracts the value from a JSON record.
     """
 
     if type_cast is None:
         return lambda record_json: record_json["value"].get(column_name)
+    elif column_type is TIMESTAMP:
+        cast = type_cast  # hint to type checker
+
+        def _get_optional_timestamp_value(
+            record_json: JsonRecord,
+        ) -> Optional[datetime]:
+            value = record_json["value"].get(column_name)
+            if value is None:
+                return None
+
+            try:
+                return cast(value)
+            except ValueError:
+                return _handle_exceptional_datetime(record_json, column_name)
+
+        return _get_optional_timestamp_value
     else:
         cast = type_cast  # hint to type checker
 
         def _get_optional_value(record_json: JsonRecord) -> Optional[Any]:
             value = record_json["value"].get(column_name)
             if value is None:
                 return None
@@ -101,17 +146,17 @@
 
     # make sure to return a single lambda that takes a record and returns the value directly
     # perform as much pre-processing outside the lambda as possible, avoid expensive computations within the lambda
     column_name = col.name
     if col.primary_key:
         return _get_primary_extractor(column_name, type_cast)
     elif col.nullable:
-        return _get_optional_extractor(column_name, type_cast)
+        return _get_optional_extractor(column_name, column_type, type_cast)
     else:
-        return _get_required_extractor(column_name, type_cast)
+        return _get_required_extractor(column_name, column_type, type_cast)
 
 
 def get_type_cast(column_type: Type[TypeEngine]) -> Optional[JsonTypeCast]:
     type_cast: Optional[JsonTypeCast]
     if (
         column_type is Integer
         or column_type is SmallInteger
```

### Comparing `instructure-dap-client-0.3.8/dap/conversion_nonperf.py` & `instructure-dap-client-0.3.8.2/dap/conversion_nonperf.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/conversion_perf.py` & `instructure-dap-client-0.3.8.2/dap/conversion_perf.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/dap_error.py` & `instructure-dap-client-0.3.8.2/dap/dap_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Any, Literal
+from typing import Any, Literal, Optional
 
 from strong_typing.schema import json_schema_type
 
 
 @json_schema_type
 @dataclass
 class ServerError(Exception):
@@ -103,15 +103,30 @@
     Raised when data is queried outside of the allowed time range.
 
     :param since: The earliest permitted timestamp.
     :param until: The latest permitted timestamp.
     """
 
     since: datetime
-    until: datetime
+    until: Optional[datetime]
+
+
+@json_schema_type
+@dataclass
+class SnapshotRequiredError(OperationError):
+    """
+    Raised when data is queried outside of the allowed time range, and the table was reloaded recently.
+    A new snapshot is required to keep data consistency.
+
+    :param since: The earliest permitted timestamp.
+    :param until: The latest permitted timestamp.
+    """
+
+    since: datetime
+    until: Optional[datetime]
 
 
 @json_schema_type
 @dataclass
 class ProcessingError(OperationError):
     """
     Raised when a job has terminated due to an unexpected error.
```

### Comparing `instructure-dap-client-0.3.8/dap/dap_types.py` & `instructure-dap-client-0.3.8.2/dap/dap_types.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/database/base_processor.py` & `instructure-dap-client-0.3.8.2/dap/database/base_processor.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/database/connection.py` & `instructure-dap-client-0.3.8.2/dap/database/connection.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/database/database_errors.py` & `instructure-dap-client-0.3.8.2/dap/database/database_errors.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/database/database_operations.py` & `instructure-dap-client-0.3.8.2/dap/database/database_operations.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/database/init_processor.py` & `instructure-dap-client-0.3.8.2/dap/database/init_processor.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/database/sync_processor.py` & `instructure-dap-client-0.3.8.2/dap/database/sync_processor.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/downloader.py` & `instructure-dap-client-0.3.8.2/dap/downloader.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/log.py` & `instructure-dap-client-0.3.8.2/dap/log.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/model/ddl.py` & `instructure-dap-client-0.3.8.2/dap/model/ddl.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/model/meta_table.py` & `instructure-dap-client-0.3.8.2/dap/model/meta_table.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/model/metadata.py` & `instructure-dap-client-0.3.8.2/dap/model/metadata.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/networking.py` & `instructure-dap-client-0.3.8.2/dap/networking.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/payload.py` & `instructure-dap-client-0.3.8.2/dap/payload.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/replicator/sql.py` & `instructure-dap-client-0.3.8.2/dap/replicator/sql.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/timer.py` & `instructure-dap-client-0.3.8.2/dap/timer.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/dap/timestamp.py` & `instructure-dap-client-0.3.8.2/dap/timestamp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+import re
 from datetime import datetime, timezone
 
+# pattern to accept extended ISO 8601 date-time string
+_extended_iso_pattern = re.compile(
+    r"^(\+\d{5,6}|-\d{4,6})-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}([.]\d+)?(([+-]\d{2}:\d{2})|Z)?$"
+)
+
 
 def valid_utc_datetime(s: str) -> datetime:
     """
     Converts a string into a UTC datetime instance.
 
     :param s: An ISO 8601 timestamp string.
     :returns: A time zone aware datetime instance with time zone UTC.
@@ -29,7 +35,27 @@
     # fromisoformat(...) supports military time zone designator "Zulu" to stand for UTC only in Python 3.11 and later
     if s.endswith("Z"):
         # remove time zone suffix "Z" (UTC) and parse into naive datetime
         return datetime.fromisoformat(s[:-1])
     else:
         # parse as time zone aware datetime, convert to UTC, and cast to naive datetime
         return datetime.fromisoformat(s).astimezone(timezone.utc).replace(tzinfo=None)
+
+
+def clamp_naive_datetime(s: str) -> datetime:
+    """
+    Converts a string into a naive datetime instance, clamping dates outside RFC 3339 range.
+
+    :param s: An ISO 8601 timestamp string.
+    :returns: A naive datetime instance that is implicitly assumed to be in time zone UTC.
+    """
+
+    # check for expansion of the year representation
+    if re.match(_extended_iso_pattern, s):
+        if s.startswith("+"):
+            # clamp at maximum date
+            return datetime.max
+        else:
+            # clamp at minimum date
+            return datetime.min
+    else:
+        return valid_naive_datetime(s)
```

### Comparing `instructure-dap-client-0.3.8/instructure_dap_client.egg-info/PKG-INFO` & `instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructure-dap-client
-Version: 0.3.8
+Version: 0.3.8.2
 Summary: Data Access Platform client library
 Author: Levente Hunyadi
 Author-email: levente.hunyadi@instructure.com
 Maintainer: Edina Tipter
 Maintainer-email: edina.tipter@instructure.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `instructure-dap-client-0.3.8/instructure_dap_client.egg-info/SOURCES.txt` & `instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8/setup.cfg` & `instructure-dap-client-0.3.8.2/setup.cfg`

 * *Files identical despite different names*

