# Comparing `tmp/dbt-clickzetta-0.1.7.tar.gz` & `tmp/dbt-clickzetta-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickzetta-0.1.7.tar", last modified: Mon Jun  5 06:11:06 2023, max compression
+gzip compressed data, was "dbt-clickzetta-0.1.8.tar", last modified: Mon Jun  5 06:47:26 2023, max compression
```

## Comparing `dbt-clickzetta-0.1.7.tar` & `dbt-clickzetta-0.1.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.634896 dbt-clickzetta-0.1.7/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 06:11:06.634756 dbt-clickzetta-0.1.7/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/README.md
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.629757 dbt-clickzetta-0.1.7/dbt/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.629026 dbt-clickzetta-0.1.7/dbt/adapters/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.630795 dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/__version__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/column.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7138 2023-05-29 03:50:21.000000 dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/connections.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6909 2023-06-05 05:29:58.000000 dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/impl.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      961 2023-06-05 06:07:50.000000 dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/relation.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.629123 dbt-clickzetta-0.1.7/dbt/include/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.631251 dbt-clickzetta-0.1.7/dbt/include/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/dbt_project.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.631450 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/adapters.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.631908 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.632399 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/incremental/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2635 2023-06-05 06:11:02.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/seed.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/snapshot.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/table.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/view.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.634026 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/any_value.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/array_append.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/array_concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/array_construct.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/assert_not_null.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/bool_or.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/dateadd.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/datediff.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/listagg.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/split_part.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/timestamps.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.7/dbt/include/clickzetta/profile_template.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:11:06.634604 dbt-clickzetta-0.1.7/dbt_clickzetta.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 06:11:06.000000 dbt-clickzetta-0.1.7/dbt_clickzetta.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-06-05 06:11:06.000000 dbt-clickzetta-0.1.7/dbt_clickzetta.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 06:11:06.000000 dbt-clickzetta-0.1.7/dbt_clickzetta.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 06:11:06.000000 dbt-clickzetta-0.1.7/dbt_clickzetta.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-06-05 06:11:06.000000 dbt-clickzetta-0.1.7/dbt_clickzetta.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-06-05 06:11:06.000000 dbt-clickzetta-0.1.7/dbt_clickzetta.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-05 06:11:06.634937 dbt-clickzetta-0.1.7/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-06-05 06:11:02.000000 dbt-clickzetta-0.1.7/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.496684 dbt-clickzetta-0.1.8/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 06:47:26.496525 dbt-clickzetta-0.1.8/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/README.md
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.417085 dbt-clickzetta-0.1.8/dbt/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.416021 dbt-clickzetta-0.1.8/dbt/adapters/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.418405 dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/__version__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/column.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7138 2023-05-29 03:50:21.000000 dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/connections.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7216 2023-06-05 06:47:23.000000 dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/impl.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      961 2023-06-05 06:07:50.000000 dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/relation.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.416182 dbt-clickzetta-0.1.8/dbt/include/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.419027 dbt-clickzetta-0.1.8/dbt/include/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/dbt_project.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.419616 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/adapters.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.439152 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.457659 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/incremental/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2614 2023-06-05 06:23:07.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/seed.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/snapshot.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/table.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/view.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.495532 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/any_value.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/array_append.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/array_concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/array_construct.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/assert_not_null.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/bool_or.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/dateadd.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/datediff.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/listagg.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/split_part.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/timestamps.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.8/dbt/include/clickzetta/profile_template.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 06:47:26.496323 dbt-clickzetta-0.1.8/dbt_clickzetta.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 06:47:26.000000 dbt-clickzetta-0.1.8/dbt_clickzetta.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-06-05 06:47:26.000000 dbt-clickzetta-0.1.8/dbt_clickzetta.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 06:47:26.000000 dbt-clickzetta-0.1.8/dbt_clickzetta.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 06:47:26.000000 dbt-clickzetta-0.1.8/dbt_clickzetta.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-06-05 06:47:26.000000 dbt-clickzetta-0.1.8/dbt_clickzetta.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-06-05 06:47:26.000000 dbt-clickzetta-0.1.8/dbt_clickzetta.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-05 06:47:26.496731 dbt-clickzetta-0.1.8/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-06-05 06:47:23.000000 dbt-clickzetta-0.1.8/setup.py
```

### Comparing `dbt-clickzetta-0.1.7/PKG-INFO` & `dbt-clickzetta-0.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickzetta
-Version: 0.1.7
+Version: 0.1.8
 Summary: The ClickZetta adapter plugin for dbt
 Home-page: 
 Author: clickzetta
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/__init__.py` & `dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/column.py` & `dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/connections.py` & `dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/impl.py` & `dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from dbt.utils import executor, AttrDict
 
 GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME = "get_columns_in_relation_raw"
 LIST_SCHEMAS_MACRO_NAME = "list_schemas"
 LIST_RELATIONS_MACRO_NAME = "list_relations_without_caching"
 LIST_RELATIONS_SHOW_TABLES_MACRO_NAME = "list_relations_show_tables_without_caching"
 DESCRIBE_TABLE_EXTENDED_MACRO_NAME = "describe_table_extended_without_caching"
+DROP_RELATION_MACRO_NAME = "drop_relation"
 
 TABLE_OR_VIEW_NOT_FOUND_MESSAGES = (
     "[TABLE_OR_VIEW_NOT_FOUND]",
     "Table or view not found",
     "NoSuchTableException",
 )
 
@@ -131,14 +132,21 @@
 
     def check_schema_exists(self, database, schema):
         results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": database})
 
         exists = True if schema in [row[0] for row in results] else False
         return exists
 
+    def drop_relation(self, relation: BaseRelation):
+        if relation.type is None:
+            raise dbt.RelationTypeNullError(relation)
+
+        self.cache_dropped(relation)
+        self.execute_macro(DROP_RELATION_MACRO_NAME, kwargs={"relation": relation})
+
     def list_relations_without_caching(self, schema_relation: ClickZettaRelation) \
             -> List[ClickZettaRelation]:  # type: ignore
         kwargs = {"schema_relation": schema_relation}
         try:
             results = self.execute_macro(LIST_RELATIONS_MACRO_NAME, kwargs=kwargs)
         except DbtDatabaseError as exc:
             if "Object does not exist" in str(exc):
```

### Comparing `dbt-clickzetta-0.1.7/dbt/adapters/clickzetta/relation.py` & `dbt-clickzetta-0.1.8/dbt/adapters/clickzetta/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/adapters.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/incremental/validate.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/seed.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/seed.sql`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% macro clickzetta__get_binding_char() %}
   {{ return('?') }}
 {% endmacro %}
 
 
--- {% macro clickzetta__reset_csv_table(model, full_refresh, old_relation, agate_table) %}
---     {% if old_relation %}
---         {{ adapter.drop_relation(old_relation) }}
---     {% endif %}
---     {% set sql = create_csv_table(model, agate_table) %}
---     {{ return(sql) }}
--- {% endmacro %}
+{% macro clickzetta__reset_csv_table(model, full_refresh, old_relation, agate_table) %}
+    {% if old_relation %}
+        {{ adapter.drop_relation(old_relation) }}
+    {% endif %}
+    {% set sql = create_csv_table(model, agate_table) %}
+    {{ return(sql) }}
+{% endmacro %}
 
 
 {% macro clickzetta__load_csv_rows(model, agate_table) %}
 
   {% set batch_size = get_batch_size() %}
   {% set column_override = model['config'].get('column_types', {}) %}
```

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/snapshot.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/materializations/table.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/dateadd.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/datediff.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/listagg.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt/include/clickzetta/macros/utils/split_part.sql` & `dbt-clickzetta-0.1.8/dbt/include/clickzetta/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/dbt_clickzetta.egg-info/PKG-INFO` & `dbt-clickzetta-0.1.8/dbt_clickzetta.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickzetta
-Version: 0.1.7
+Version: 0.1.8
 Summary: The ClickZetta adapter plugin for dbt
 Home-page: 
 Author: clickzetta
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `dbt-clickzetta-0.1.7/dbt_clickzetta.egg-info/SOURCES.txt` & `dbt-clickzetta-0.1.8/dbt_clickzetta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.7/setup.py` & `dbt-clickzetta-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-clickzetta"
-package_version = "0.1.7"
+package_version = "0.1.8"
 dbt_core_version = _get_dbt_core_version()
 description = """The ClickZetta adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

