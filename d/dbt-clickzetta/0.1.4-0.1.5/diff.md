# Comparing `tmp/dbt-clickzetta-0.1.4.tar.gz` & `tmp/dbt-clickzetta-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickzetta-0.1.4.tar", last modified: Tue May 30 03:02:44 2023, max compression
+gzip compressed data, was "dbt-clickzetta-0.1.5.tar", last modified: Mon Jun  5 04:09:28 2023, max compression
```

## Comparing `dbt-clickzetta-0.1.4.tar` & `dbt-clickzetta-0.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.471148 dbt-clickzetta-0.1.4/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-30 03:02:44.471010 dbt-clickzetta-0.1.4/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/README.md
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.465518 dbt-clickzetta-0.1.4/dbt/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.464698 dbt-clickzetta-0.1.4/dbt/adapters/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.466684 dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/__version__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/column.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7138 2023-05-29 03:50:21.000000 dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/connections.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6709 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/impl.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1184 2023-05-28 14:31:37.000000 dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/relation.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.464804 dbt-clickzetta-0.1.4/dbt/include/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.467174 dbt-clickzetta-0.1.4/dbt/include/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/dbt_project.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.467427 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/adapters.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.467971 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.468492 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/incremental/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2651 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/seed.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/snapshot.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/table.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/view.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.470259 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/any_value.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/array_append.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/array_concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/array_construct.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/assert_not_null.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/bool_or.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/dateadd.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/datediff.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/listagg.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/split_part.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/timestamps.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.4/dbt/include/clickzetta/profile_template.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 03:02:44.470852 dbt-clickzetta-0.1.4/dbt_clickzetta.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-30 03:02:44.000000 dbt-clickzetta-0.1.4/dbt_clickzetta.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-05-30 03:02:44.000000 dbt-clickzetta-0.1.4/dbt_clickzetta.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-30 03:02:44.000000 dbt-clickzetta-0.1.4/dbt_clickzetta.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-30 03:02:44.000000 dbt-clickzetta-0.1.4/dbt_clickzetta.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-05-30 03:02:44.000000 dbt-clickzetta-0.1.4/dbt_clickzetta.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-05-30 03:02:44.000000 dbt-clickzetta-0.1.4/dbt_clickzetta.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-30 03:02:44.471186 dbt-clickzetta-0.1.4/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-05-30 03:02:39.000000 dbt-clickzetta-0.1.4/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.171998 dbt-clickzetta-0.1.5/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 04:09:28.171857 dbt-clickzetta-0.1.5/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/README.md
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.166030 dbt-clickzetta-0.1.5/dbt/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.165340 dbt-clickzetta-0.1.5/dbt/adapters/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.167272 dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/__version__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/column.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7138 2023-05-29 03:50:21.000000 dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/connections.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6948 2023-06-05 03:45:11.000000 dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/impl.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1184 2023-05-28 14:31:37.000000 dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/relation.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.165430 dbt-clickzetta-0.1.5/dbt/include/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.167859 dbt-clickzetta-0.1.5/dbt/include/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/dbt_project.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.168117 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/adapters.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.168834 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.169402 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/incremental/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2614 2023-06-05 04:09:03.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/seed.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/snapshot.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/table.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/view.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.171079 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/any_value.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/array_append.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/array_concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/array_construct.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/assert_not_null.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/bool_or.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/dateadd.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/datediff.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/listagg.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/split_part.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/timestamps.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.5/dbt/include/clickzetta/profile_template.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 04:09:28.171689 dbt-clickzetta-0.1.5/dbt_clickzetta.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 04:09:28.000000 dbt-clickzetta-0.1.5/dbt_clickzetta.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-06-05 04:09:28.000000 dbt-clickzetta-0.1.5/dbt_clickzetta.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 04:09:28.000000 dbt-clickzetta-0.1.5/dbt_clickzetta.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 04:09:28.000000 dbt-clickzetta-0.1.5/dbt_clickzetta.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-06-05 04:09:28.000000 dbt-clickzetta-0.1.5/dbt_clickzetta.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-06-05 04:09:28.000000 dbt-clickzetta-0.1.5/dbt_clickzetta.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-05 04:09:28.172036 dbt-clickzetta-0.1.5/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-06-05 03:31:20.000000 dbt-clickzetta-0.1.5/setup.py
```

### Comparing `dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/__init__.py` & `dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/column.py` & `dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/connections.py` & `dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/impl.py` & `dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,21 +65,33 @@
 
     @classmethod
     def _catalog_filter_table(cls, table: agate.Table, manifest: Manifest) -> agate.Table:
         lowered = table.rename(column_names=[c.lower() for c in table.column_names])
         return super()._catalog_filter_table(lowered, manifest)
 
     @classmethod
-    def convert_number_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_text_type(cls, agate_table, col_idx):
+        return "string"
+
+    @classmethod
+    def convert_number_type(cls, agate_table, col_idx):
         decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))
-        return 'float64' if decimals else 'int64'
+        return "double" if decimals else "bigint"
+
+    @classmethod
+    def convert_date_type(cls, agate_table, col_idx):
+        return "date"
+
+    @classmethod
+    def convert_time_type(cls, agate_table, col_idx):
+        return "time"
 
     @classmethod
-    def convert_datetime_type(cls, agate_table: agate.Table, col_idx: int) -> str:
-        return 'date'
+    def convert_datetime_type(cls, agate_table, col_idx):
+        return "timestamp"
 
     def quote(self, identifier):
         return "`{}`".format(identifier)
 
     def parse_describe_extended(
             self, relation: BaseRelation, raw_rows: AttrDict
     ) -> List[ClickZettaColumn]:
```

### Comparing `dbt-clickzetta-0.1.4/dbt/adapters/clickzetta/relation.py` & `dbt-clickzetta-0.1.5/dbt/adapters/clickzetta/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/adapters.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/incremental/validate.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/seed.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/seed.sql`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% macro clickzetta__get_binding_char() %}
-  {{ return('?' if target.method == 'odbc' else '%s') }}
+  {{ return('?') }}
 {% endmacro %}
 
 
 {% macro clickzetta__reset_csv_table(model, full_refresh, old_relation, agate_table) %}
     {% if old_relation %}
         {{ adapter.drop_relation(old_relation) }}
     {% endif %}
```

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/snapshot.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/materializations/table.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/dateadd.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/datediff.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/listagg.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt/include/clickzetta/macros/utils/split_part.sql` & `dbt-clickzetta-0.1.5/dbt/include/clickzetta/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/dbt_clickzetta.egg-info/SOURCES.txt` & `dbt-clickzetta-0.1.5/dbt_clickzetta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.4/setup.py` & `dbt-clickzetta-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-clickzetta"
-package_version = "0.1.4"
+package_version = "0.1.5"
 dbt_core_version = _get_dbt_core_version()
 description = """The ClickZetta adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
@@ -64,15 +64,15 @@
     author="clickzetta",
     author_email="",
     url="",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-core~={}".format(dbt_core_version),
-        "clickzetta-connector~=0.8.3",
+        "clickzetta-connector~=0.8.5",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
```

