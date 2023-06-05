# Comparing `tmp/dbt-upsolver-1.5.23.tar.gz` & `tmp/dbt-upsolver-1.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-upsolver-1.5.23.tar", last modified: Mon May 29 13:34:32 2023, max compression
+gzip compressed data, was "dbt-upsolver-1.5.24.tar", last modified: Mon Jun  5 16:01:33 2023, max compression
```

## Comparing `dbt-upsolver-1.5.23.tar` & `dbt-upsolver-1.5.24.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/adapters/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/connection_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/copy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/target_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/transformation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/include/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/connection.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/materializedview.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/create_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/render_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-29 13:34:31.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-29 13:34:32.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:34:32.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:34:31.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 13:34:32.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 13:34:32.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/adapters/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/connection_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/target_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/transformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/adapters/upsolver/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.743665 dbt-upsolver-1.5.24/dbt/include/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/connection.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/materializedview.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/create_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/render_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/dbt/include/upsolver/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 16:01:33.000000 dbt-upsolver-1.5.24/dbt_upsolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:01:33.747665 dbt-upsolver-1.5.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-05 16:01:20.000000 dbt-upsolver-1.5.24/setup.py
```

### Comparing `dbt-upsolver-1.5.23/LICENSE` & `dbt-upsolver-1.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/PKG-INFO` & `dbt-upsolver-1.5.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 1.5.23
+Version: 1.5.24
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-1.5.23/README.md` & `dbt-upsolver-1.5.24/README.md`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/adapters/upsolver/connections.py` & `dbt-upsolver-1.5.24/dbt/adapters/upsolver/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/adapters/upsolver/impl.py` & `dbt-upsolver-1.5.24/dbt/adapters/upsolver/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,14 +145,22 @@
                 options = Target_options[source.lower()]
             else:
                 options = Copy_options[source.lower()][options_type]
             return options
         except Exception:
             raise dbt.exceptions.ParsingError(f"Undefined option value: {source}")
 
+    @available
+    def merge_tables(self, tables):
+        return agate.Table.merge(tables)
+
+    @available
+    def trim_quotes(self, value):
+        return value.replace('"', '')
+
     def list_relations_without_caching(
         self,
         schema_relation: UpsolverRelation,
         ) -> List[UpsolverRelation]:
         materializations = ["table", "job", "connection", "view"]
         results = agate.Table([],[])
         for type in materializations:
```

### Comparing `dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/connection_options.py` & `dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/connection_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/copy_options.py` & `dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/copy_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/target_options.py` & `dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/target_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/transformation_options.py` & `dbt-upsolver-1.5.24/dbt/adapters/upsolver/options/transformation_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/adapters/upsolver/relation.py` & `dbt-upsolver-1.5.24/dbt/adapters/upsolver/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/adapters.sql` & `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/adapters.sql`

 * *Files 26% similar despite different names*

```diff
@@ -24,27 +24,30 @@
 '''drops a schema in a target database.'''
 /*
   1. If database exists
   2. search all calls of schema, and change include value to False, cascade it to backtrack
 */
 {% endmacro %}
 
+
 {% macro upsolver__get_columns_in_relation(relation) -%}
-'''Returns a list of Columns in a table.'''
-/*
-  1. select as many values from column as needed
-  2. search relations to columns
-  3. where table name is equal to the relation identifier
-  4. if a relation schema exists and table schema is equal to the relation schema
-  5. order in whatever way you want to call.
-  6. create a table by loading result from call
-  7. return new table
-*/
+  {% if relation.type == 'table'  %}
+  {% call statement('get_columns_relation', fetch_result=True, auto_begin=False) -%}
+      SELECT * FROM system.information_schema.columns
+      where "catalog" = {{relation.database}}
+      and "schema" = {{relation.schema}}
+      and AND "table" = {{relation.identifier}}
+
+  {% endcall %}
+  {% endif %}
+
+  {{ return(load_result('get_columns_relation').table) }}
 {% endmacro %}
 
+
 {% macro list_relation_without_caching(schema_relation, relation_type) -%}
   {% set source = relation_type +'s' %}
   {% call statement('list_relation_without_caching', fetch_result=True) -%}
     select
       '{{ schema_relation.database }}' as database,
       name,
       '{{ schema_relation.schema }}' as schema,
@@ -59,18 +62,22 @@
       {% endif %}
   {% endcall %}
   {{ return(load_result('list_relation_without_caching').table) }}
 {% endmacro %}
 
 {% macro upsolver__list_schemas(database) -%}
 '''Returns a table of unique schemas.'''
-/*
-  1. search schemea by specific name
-  2. create a table with names
-*/
+  {% set database = adapter.trim_quotes(database) %}
+  {% call statement('list_schemas', fetch_result=True, auto_begin=False) -%}
+      select schema from system.information_schema.tables
+      where catalog = '{{database}}'
+      group by 1;
+  {% endcall %}
+
+  {{ return(load_result('list_schemas').table) }}
 {% endmacro %}
 
 {% macro upsolver__rename_relation(from_relation, to_relation) -%}
 '''Renames a relation in the database.'''
 /*
   1. Search for a specific relation name
   2. alter table by targeting specific name and passing in new name
@@ -89,7 +96,26 @@
 '''Returns current UTC time'''
 {# docs show not to be implemented currently. #}
 {% endmacro %}
 
 {% macro upsolver__create_arbitrary_object(sql) -%}
     {{ sql }}
 {%- endmacro %}
+
+{% macro upsolver_list_tables(schema_relation) -%}
+  {% call statement('upsolver_list_tables', fetch_result=True) -%}
+    select
+      '{{ schema_relation.database }}' as database,
+      name,
+      '{{ schema_relation.schema }}' as schema,
+      {% if relation_type == 'job' %}
+        'incremental' as type
+      {% else %}
+        '{{ relation_type }}' as type
+      {% endif %}
+    from system.information_schema."{{ source }}"
+      {% if relation_type in ['table', 'view'] %}
+        where schema = '{{ schema_relation.schema }}'
+      {% endif %}
+  {% endcall %}
+  {{ return(load_result('list_relation_without_caching').table) }}
+{% endmacro %}
```

### Comparing `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/connection.sql` & `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/connection.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql` & `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql` & `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql` & `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/incremental.sql` & `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/incremental/incremental.sql`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
   {%- set identifier = model['alias'] -%}
   {%- set model_config = model['config'] -%}
   {%- set incremental_strategy = adapter.get(model_config, 'incremental_strategy', False) -%}
   {%- set sync = adapter.get(model_config, 'sync', False) -%}
   {%- set options = adapter.get(model_config, 'options', {}) -%}
   {%- set source = adapter.get(model_config, 'source') -%}
   {%- set target_type = adapter.get(model_config, 'target_type', 'datalake').lower() -%}
-  {%- set target_schema = adapter.get(model_config, 'target_schema', schema) -%}
   {%- set target_table_alias = adapter.get(model_config, 'target_table_alias', identifier) -%}
   {%- set delete_condition = adapter.get(model_config, 'delete_condition', False) -%}
   {%- set partition_by = adapter.get(model_config, 'partition_by', []) -%}
   {%- set primary_key = adapter.get(model_config, 'primary_key', []) -%}
   {%- set map_columns_by_name = adapter.get(model_config, 'map_columns_by_name', False) -%}
   {%- set job_identifier = identifier + '_job' %}
 
@@ -26,23 +25,26 @@
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
   {{ log("model[config]: " ~ model['config'] ) }}
 
 
   {% if target_type  == 'datalake' %}
+    {%- set target_connection = adapter.get(model_config, 'target_connection', database) -%}
+    {%- set target_schema = adapter.get(model_config, 'target_schema', schema) -%}
     {%- set table_relation = api.Relation.create(identifier=target_table_alias,
-                                                 schema=schema,
-                                                 database=database,
+                                                 schema=target_schema,
+                                                 database=target_connection,
                                                  type='table') -%}
     {%- set into_relation = table_relation -%}
     {%- call statement('create_table_if_not_exists') -%}
       {{ get_create_table_if_not_exists_sql(table_relation, partition_by, primary_key, options) }}
     {%- endcall -%}
   {%- else -%}
+    {%- set target_schema = adapter.require(model_config, 'target_schema') -%}
     {% set target_connection = adapter.require(model_config, 'target_connection') %}
     {%- set into_relation = target_connection + '.' + target_schema + '.' + target_table_alias -%}
   {%- endif %}
 
   {%- if old_relation -%}
     {%- call statement('main') -%}
       {{ get_alter_job_sql(job_identifier, options, incremental_strategy, source) }}
```

### Comparing `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/materializedview.sql` & `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/materializedview.sql`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% materialization materializedview, adapter='upsolver' %}
   {%- set identifier = model['alias'] -%}
   {%- set model_config = model['config'] -%}
   {% set sync = adapter.get(model_config, 'sync', False) %}
   {% set options = adapter.get(model_config, 'options', {}) %}
-  {% set enriched_options = adapter.enrich_options(options, materialized_view, 'target_options') %}
+  {% set enriched_options = adapter.enrich_options(options, 'materialized_view', 'target_options') %}
   {% set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') %}
 
   {%- set old_relation = adapter.get_relation(identifier=identifier,
                                               schema=schema,
                                               database=database) -%}
   {%- set target_relation = api.Relation.create(identifier=identifier,
                                                 schema=schema,
```

### Comparing `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/ater_job.sql` & `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/ater_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/create_table.sql` & `dbt-upsolver-1.5.24/dbt/include/upsolver/macros/materializations/utils/create_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/dbt_upsolver.egg-info/PKG-INFO` & `dbt-upsolver-1.5.24/dbt_upsolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 1.5.23
+Version: 1.5.24
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-1.5.23/dbt_upsolver.egg-info/SOURCES.txt` & `dbt-upsolver-1.5.24/dbt_upsolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.23/setup.py` & `dbt-upsolver-1.5.24/setup.py`

 * *Files identical despite different names*

