# Comparing `tmp/lokii-1.1.4.tar.gz` & `tmp/lokii-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokii-1.1.4.tar", last modified: Mon Jun  5 15:30:27 2023, max compression
+gzip compressed data, was "lokii-1.1.5.tar", last modified: Mon Jun  5 15:37:12 2023, max compression
```

## Comparing `lokii-1.1.4.tar` & `lokii-1.1.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.423995 lokii-1.1.4/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.1.4/LICENSE
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-05 15:30:27.423995 lokii-1.1.4/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     5434 2023-06-02 08:01:36.000000 lokii-1.1.4/README.md
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.411995 lokii-1.1.4/lokii/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       77 2023-06-05 15:29:57.000000 lokii-1.1.4/lokii/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.1.4/lokii/__main__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3176 2023-06-02 08:01:36.000000 lokii-1.1.4/lokii/cli.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2142 2023-06-04 11:01:51.000000 lokii-1.1.4/lokii/config.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.415995 lokii-1.1.4/lokii/exec/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.4/lokii/exec/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2620 2023-05-31 14:39:03.000000 lokii-1.1.4/lokii/exec/node_executor.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.415995 lokii-1.1.4/lokii/logger/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.4/lokii/logger/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1268 2023-06-02 08:52:49.000000 lokii-1.1.4/lokii/logger/color.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.1.4/lokii/logger/context.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      877 2023-06-03 07:10:34.000000 lokii-1.1.4/lokii/logger/formatter.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.1.4/lokii/logger/progress.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     7475 2023-06-04 18:47:42.000000 lokii-1.1.4/lokii/main.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.415995 lokii-1.1.4/lokii/model/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.4/lokii/model/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      943 2023-06-02 08:01:36.000000 lokii-1.1.4/lokii/model/group_module.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-31 14:39:03.000000 lokii-1.1.4/lokii/model/node_module.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.415995 lokii-1.1.4/lokii/parse/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.4/lokii/parse/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      709 2023-05-31 14:39:03.000000 lokii-1.1.4/lokii/parse/base_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3109 2023-06-03 07:18:23.000000 lokii-1.1.4/lokii/parse/group_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2928 2023-06-03 07:15:57.000000 lokii-1.1.4/lokii/parse/node_parser.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.419995 lokii-1.1.4/lokii/storage/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.4/lokii/storage/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      983 2023-06-02 08:01:36.000000 lokii-1.1.4/lokii/storage/batch_iterator.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4972 2023-06-05 15:29:19.000000 lokii-1.1.4/lokii/storage/data_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      888 2023-06-05 15:28:47.000000 lokii-1.1.4/lokii/storage/temp_storage.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.419995 lokii-1.1.4/lokii/util/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.4/lokii/util/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2160 2023-05-31 14:39:03.000000 lokii-1.1.4/lokii/util/graph_analyzer.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1464 2023-05-31 14:39:03.000000 lokii-1.1.4/lokii/util/module_file_loader.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.1.4/lokii/util/perf_timer_context.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.415995 lokii-1.1.4/lokii.egg-info/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-05 15:30:27.000000 lokii-1.1.4/lokii.egg-info/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1341 2023-06-05 15:30:27.000000 lokii-1.1.4/lokii.egg-info/SOURCES.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-06-05 15:30:27.000000 lokii-1.1.4/lokii.egg-info/dependency_links.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-06-05 15:30:27.000000 lokii-1.1.4/lokii.egg-info/entry_points.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.1.4/lokii.egg-info/not-zip-safe
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       71 2023-06-05 15:30:27.000000 lokii-1.1.4/lokii.egg-info/requires.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-06-05 15:30:27.000000 lokii-1.1.4/lokii.egg-info/top_level.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       84 2023-06-05 15:30:27.423995 lokii-1.1.4/setup.cfg
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1664 2023-06-04 11:07:21.000000 lokii-1.1.4/setup.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.419995 lokii-1.1.4/tests/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.1.4/tests/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2501 2023-06-02 08:01:36.000000 lokii-1.1.4/tests/conftest.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.419995 lokii-1.1.4/tests/exec/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.4/tests/exec/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1098 2023-05-31 14:39:03.000000 lokii-1.1.4/tests/exec/test_node_executor.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.419995 lokii-1.1.4/tests/parse/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.4/tests/parse/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2230 2023-06-02 08:01:36.000000 lokii-1.1.4/tests/parse/test_group_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3165 2023-05-31 14:39:03.000000 lokii-1.1.4/tests/parse/test_node_parser.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.419995 lokii-1.1.4/tests/storage/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.4/tests/storage/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4195 2023-06-02 09:34:04.000000 lokii-1.1.4/tests/storage/test_data_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.1.4/tests/storage/test_temp_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3345 2023-06-03 05:56:09.000000 lokii-1.1.4/tests/test_cli.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:30:27.423995 lokii-1.1.4/tests/util/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.4/tests/util/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      953 2023-05-31 14:39:03.000000 lokii-1.1.4/tests/util/test_graph_analyzer.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.1.4/tests/util/test_module_file_loader.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.1.4/tests/util/test_perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.1.5/LICENSE
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-05 15:37:12.910365 lokii-1.1.5/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     5434 2023-06-02 08:01:36.000000 lokii-1.1.5/README.md
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.902366 lokii-1.1.5/lokii/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       77 2023-06-05 15:37:06.000000 lokii-1.1.5/lokii/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/__main__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3176 2023-06-02 08:01:36.000000 lokii-1.1.5/lokii/cli.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2142 2023-06-04 11:01:51.000000 lokii-1.1.5/lokii/config.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.902366 lokii-1.1.5/lokii/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2620 2023-05-31 14:39:03.000000 lokii-1.1.5/lokii/exec/node_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.906365 lokii-1.1.5/lokii/logger/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/logger/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1268 2023-06-02 08:52:49.000000 lokii-1.1.5/lokii/logger/color.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/logger/context.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      877 2023-06-03 07:10:34.000000 lokii-1.1.5/lokii/logger/formatter.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/logger/progress.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     7475 2023-06-04 18:47:42.000000 lokii-1.1.5/lokii/main.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.906365 lokii-1.1.5/lokii/model/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/model/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      943 2023-06-02 08:01:36.000000 lokii-1.1.5/lokii/model/group_module.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-31 14:39:03.000000 lokii-1.1.5/lokii/model/node_module.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.906365 lokii-1.1.5/lokii/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      709 2023-05-31 14:39:03.000000 lokii-1.1.5/lokii/parse/base_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3109 2023-06-03 07:18:23.000000 lokii-1.1.5/lokii/parse/group_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2928 2023-06-03 07:15:57.000000 lokii-1.1.5/lokii/parse/node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.906365 lokii-1.1.5/lokii/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      983 2023-06-02 08:01:36.000000 lokii-1.1.5/lokii/storage/batch_iterator.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     5065 2023-06-05 15:36:58.000000 lokii-1.1.5/lokii/storage/data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      888 2023-06-05 15:28:47.000000 lokii-1.1.5/lokii/storage/temp_storage.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.906365 lokii-1.1.5/lokii/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2160 2023-05-31 14:39:03.000000 lokii-1.1.5/lokii/util/graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1464 2023-05-31 14:39:03.000000 lokii-1.1.5/lokii/util/module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/util/perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.902366 lokii-1.1.5/lokii.egg-info/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1341 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/SOURCES.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/dependency_links.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/entry_points.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.1.5/lokii.egg-info/not-zip-safe
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       71 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/requires.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/top_level.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       84 2023-06-05 15:37:12.910365 lokii-1.1.5/setup.cfg
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1664 2023-06-04 11:07:21.000000 lokii-1.1.5/setup.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/tests/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2501 2023-06-02 08:01:36.000000 lokii-1.1.5/tests/conftest.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/tests/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1098 2023-05-31 14:39:03.000000 lokii-1.1.5/tests/exec/test_node_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/tests/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2230 2023-06-02 08:01:36.000000 lokii-1.1.5/tests/parse/test_group_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3165 2023-05-31 14:39:03.000000 lokii-1.1.5/tests/parse/test_node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/tests/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4195 2023-06-02 09:34:04.000000 lokii-1.1.5/tests/storage/test_data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/storage/test_temp_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3345 2023-06-03 05:56:09.000000 lokii-1.1.5/tests/test_cli.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/tests/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      953 2023-05-31 14:39:03.000000 lokii-1.1.5/tests/util/test_graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/util/test_module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/util/test_perf_timer_context.py
```

### Comparing `lokii-1.1.4/LICENSE` & `lokii-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/PKG-INFO` & `lokii-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lokii
-Version: 1.1.4
+Version: 1.1.5
 Summary: Generate, Load, Develop and Test with consistent relational datasets!
 Home-page: https://github.com/dorukerenaktas/lokii
 Author: Doruk Eren Aktaş
 Author-email: dorukerenaktas@gmail.com
 License: MIT License
 Keywords: data generation,relational datasets,development environment,testing,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lokii-1.1.4/README.md` & `lokii-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/cli.py` & `lokii-1.1.5/lokii/cli.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/config.py` & `lokii-1.1.5/lokii/config.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/exec/node_executor.py` & `lokii-1.1.5/lokii/exec/node_executor.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/logger/color.py` & `lokii-1.1.5/lokii/logger/color.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/logger/context.py` & `lokii-1.1.5/lokii/logger/context.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/logger/formatter.py` & `lokii-1.1.5/lokii/logger/formatter.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/logger/progress.py` & `lokii-1.1.5/lokii/logger/progress.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/main.py` & `lokii-1.1.5/lokii/main.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/model/group_module.py` & `lokii-1.1.5/lokii/model/group_module.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/model/node_module.py` & `lokii-1.1.5/lokii/model/node_module.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/parse/base_parser.py` & `lokii-1.1.5/lokii/parse/base_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/parse/group_parser.py` & `lokii-1.1.5/lokii/parse/group_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/parse/node_parser.py` & `lokii-1.1.5/lokii/parse/node_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/storage/batch_iterator.py` & `lokii-1.1.5/lokii/storage/batch_iterator.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/storage/data_storage.py` & `lokii-1.1.5/lokii/storage/data_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,23 +95,24 @@
         Creates a table for given node name in local relational database. If there is a table
         with the same node name it will drop all data and create a fresh one. Given files will
         be concatenated and inserted in the fresh table.
 
         :param name: node name of the module
         :param files: list of generated file paths
         """
-        if len(files) == 0:
-            return
-
         with self.connect() as conn:
             assert "." not in name, "Node names can not contain dot(.) = %s" % name
 
             # concatenate and insert file contents in a fresh table
             q = "CREATE OR REPLACE TABLE %s AS SELECT * FROM read_json_auto(%s);"
-            conn.execute(q % (name, files)).fetchall()
+            q = q % (name, files)
+            if len(files) == 0:
+                q = "CREATE OR REPLACE TABLE %s(id INTEGER);"
+                q = q % name
+            conn.execute(q).fetchall()
 
     def export(self, out_path: str, fmt: str) -> None:
         """
         Exports all generated tables to given file format.
 
         :param out_path: folder path of the exported files
         :param fmt: file format of the exported files
```

### Comparing `lokii-1.1.4/lokii/storage/temp_storage.py` & `lokii-1.1.5/lokii/storage/temp_storage.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/util/graph_analyzer.py` & `lokii-1.1.5/lokii/util/graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/util/module_file_loader.py` & `lokii-1.1.5/lokii/util/module_file_loader.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii/util/perf_timer_context.py` & `lokii-1.1.5/lokii/util/perf_timer_context.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/lokii.egg-info/PKG-INFO` & `lokii-1.1.5/lokii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lokii
-Version: 1.1.4
+Version: 1.1.5
 Summary: Generate, Load, Develop and Test with consistent relational datasets!
 Home-page: https://github.com/dorukerenaktas/lokii
 Author: Doruk Eren Aktaş
 Author-email: dorukerenaktas@gmail.com
 License: MIT License
 Keywords: data generation,relational datasets,development environment,testing,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lokii-1.1.4/lokii.egg-info/SOURCES.txt` & `lokii-1.1.5/lokii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/setup.py` & `lokii-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/tests/conftest.py` & `lokii-1.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/tests/exec/test_node_executor.py` & `lokii-1.1.5/tests/exec/test_node_executor.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/tests/parse/test_group_parser.py` & `lokii-1.1.5/tests/parse/test_group_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/tests/parse/test_node_parser.py` & `lokii-1.1.5/tests/parse/test_node_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/tests/storage/test_data_storage.py` & `lokii-1.1.5/tests/storage/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/tests/test_cli.py` & `lokii-1.1.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/tests/util/test_graph_analyzer.py` & `lokii-1.1.5/tests/util/test_graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/tests/util/test_module_file_loader.py` & `lokii-1.1.5/tests/util/test_module_file_loader.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.4/tests/util/test_perf_timer_context.py` & `lokii-1.1.5/tests/util/test_perf_timer_context.py`

 * *Files identical despite different names*

