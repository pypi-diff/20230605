# Comparing `tmp/dbt-clickzetta-0.2.3.tar.gz` & `tmp/dbt-clickzetta-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickzetta-0.2.3.tar", last modified: Mon Jun  5 09:18:35 2023, max compression
+gzip compressed data, was "dbt-clickzetta-0.2.4.tar", last modified: Mon Jun  5 09:21:54 2023, max compression
```

## Comparing `dbt-clickzetta-0.2.3.tar` & `dbt-clickzetta-0.2.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.735971 dbt-clickzetta-0.2.3/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 09:18:35.735846 dbt-clickzetta-0.2.3/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/README.md
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.730306 dbt-clickzetta-0.2.3/dbt/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.729590 dbt-clickzetta-0.2.3/dbt/adapters/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.731443 dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/__version__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/column.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7150 2023-06-05 09:18:33.000000 dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/connections.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6952 2023-06-05 07:08:34.000000 dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/impl.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      961 2023-06-05 06:07:50.000000 dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/relation.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.729681 dbt-clickzetta-0.2.3/dbt/include/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.731920 dbt-clickzetta-0.2.3/dbt/include/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/dbt_project.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.732125 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/adapters.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.732705 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.733192 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/incremental/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1655 2023-06-05 08:55:29.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/seed.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/snapshot.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/table.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/view.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.735026 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/any_value.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/array_append.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/array_concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/array_construct.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/assert_not_null.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/bool_or.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/dateadd.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/datediff.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/listagg.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/split_part.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/timestamps.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.3/dbt/include/clickzetta/profile_template.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:18:35.735679 dbt-clickzetta-0.2.3/dbt_clickzetta.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 09:18:35.000000 dbt-clickzetta-0.2.3/dbt_clickzetta.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-06-05 09:18:35.000000 dbt-clickzetta-0.2.3/dbt_clickzetta.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 09:18:35.000000 dbt-clickzetta-0.2.3/dbt_clickzetta.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 09:18:35.000000 dbt-clickzetta-0.2.3/dbt_clickzetta.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-06-05 09:18:35.000000 dbt-clickzetta-0.2.3/dbt_clickzetta.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-06-05 09:18:35.000000 dbt-clickzetta-0.2.3/dbt_clickzetta.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-05 09:18:35.736021 dbt-clickzetta-0.2.3/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-06-05 09:18:33.000000 dbt-clickzetta-0.2.3/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.165266 dbt-clickzetta-0.2.4/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 09:21:54.165137 dbt-clickzetta-0.2.4/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/README.md
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.159366 dbt-clickzetta-0.2.4/dbt/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.158643 dbt-clickzetta-0.2.4/dbt/adapters/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.160337 dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/__version__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/column.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7157 2023-06-05 09:21:52.000000 dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/connections.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6952 2023-06-05 07:08:34.000000 dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/impl.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      961 2023-06-05 06:07:50.000000 dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/relation.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.158732 dbt-clickzetta-0.2.4/dbt/include/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.160797 dbt-clickzetta-0.2.4/dbt/include/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/dbt_project.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.160999 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/adapters.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.161584 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.162276 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/incremental/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1655 2023-06-05 08:55:29.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/seed.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/snapshot.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/table.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/view.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.164294 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/any_value.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/array_append.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/array_concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/array_construct.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/assert_not_null.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/bool_or.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/dateadd.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/datediff.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/listagg.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/split_part.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/timestamps.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.4/dbt/include/clickzetta/profile_template.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 09:21:54.164980 dbt-clickzetta-0.2.4/dbt_clickzetta.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 09:21:54.000000 dbt-clickzetta-0.2.4/dbt_clickzetta.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-06-05 09:21:54.000000 dbt-clickzetta-0.2.4/dbt_clickzetta.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 09:21:54.000000 dbt-clickzetta-0.2.4/dbt_clickzetta.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 09:21:54.000000 dbt-clickzetta-0.2.4/dbt_clickzetta.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-06-05 09:21:54.000000 dbt-clickzetta-0.2.4/dbt_clickzetta.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-06-05 09:21:54.000000 dbt-clickzetta-0.2.4/dbt_clickzetta.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-05 09:21:54.165304 dbt-clickzetta-0.2.4/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-06-05 09:21:52.000000 dbt-clickzetta-0.2.4/setup.py
```

### Comparing `dbt-clickzetta-0.2.3/PKG-INFO` & `dbt-clickzetta-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickzetta
-Version: 0.2.3
+Version: 0.2.4
 Summary: The ClickZetta adapter plugin for dbt
 Home-page: 
 Author: clickzetta
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/__init__.py` & `dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/column.py` & `dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/connections.py` & `dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             bindings: Optional[Any] = None,
             abridge_sql_log: bool = False,
     ) -> Tuple[Connection, Any]:  # type: ignore
         # TODO(hanmiao.li): clickzetta cursor is not support pass bingdings, will support later.
         if bindings:
             cast_bindings = []
             for binding in bindings:
-                cast_bindings.append(str(binding))
+                cast_bindings.append(f"'{str(binding)}'")
             sql = sql % tuple(cast_bindings)
             bindings = None
 
         connection, cursor = self._add_standard_queries(
             [sql],
             auto_begin=auto_begin,
             bindings=bindings,
```

### Comparing `dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/impl.py` & `dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/adapters/clickzetta/relation.py` & `dbt-clickzetta-0.2.4/dbt/adapters/clickzetta/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/adapters.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/incremental/validate.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/seed.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/snapshot.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/materializations/table.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/dateadd.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/datediff.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/listagg.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt/include/clickzetta/macros/utils/split_part.sql` & `dbt-clickzetta-0.2.4/dbt/include/clickzetta/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/dbt_clickzetta.egg-info/PKG-INFO` & `dbt-clickzetta-0.2.4/dbt_clickzetta.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickzetta
-Version: 0.2.3
+Version: 0.2.4
 Summary: The ClickZetta adapter plugin for dbt
 Home-page: 
 Author: clickzetta
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `dbt-clickzetta-0.2.3/dbt_clickzetta.egg-info/SOURCES.txt` & `dbt-clickzetta-0.2.4/dbt_clickzetta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.3/setup.py` & `dbt-clickzetta-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-clickzetta"
-package_version = "0.2.3"
+package_version = "0.2.4"
 dbt_core_version = _get_dbt_core_version()
 description = """The ClickZetta adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

