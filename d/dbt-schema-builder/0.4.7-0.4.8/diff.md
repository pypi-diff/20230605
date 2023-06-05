# Comparing `tmp/dbt-schema-builder-0.4.7.tar.gz` & `tmp/dbt-schema-builder-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-schema-builder-0.4.7.tar", last modified: Mon Jun  5 13:41:08 2023, max compression
+gzip compressed data, was "dbt-schema-builder-0.4.8.tar", last modified: Mon Jun  5 17:19:18 2023, max compression
```

## Comparing `dbt-schema-builder-0.4.7.tar` & `dbt-schema-builder-0.4.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4022 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/dbt_schema_builder/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/app.py
--rw-r--r--   0 runner    (1001) docker     (122)    24281 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/queries.py
--rw-r--r--   0 runner    (1001) docker     (122)     9373 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/relation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3904 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/schema_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/snowflake_keywords.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/dbt_schema_builder/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/templates/model_sql_pii.tpl
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/templates/model_sql_safe.tpl
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5314 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:19:18.818346 dbt-schema-builder-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-06-05 17:19:18.818346 dbt-schema-builder-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4022 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:19:18.814346 dbt-schema-builder-0.4.8/dbt_schema_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24281 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9373 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/relation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3904 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/schema_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/snowflake_keywords.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:19:18.818346 dbt-schema-builder-0.4.8/dbt_schema_builder/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/templates/model_sql_pii.tpl
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/dbt_schema_builder/templates/model_sql_safe.tpl
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:19:18.814346 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-05 17:19:18.000000 dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 17:19:18.818346 dbt-schema-builder-0.4.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-05 17:19:18.818346 dbt-schema-builder-0.4.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5314 2023-06-05 17:19:09.000000 dbt-schema-builder-0.4.8/setup.py
```

### Comparing `dbt-schema-builder-0.4.7/LICENSE.txt` & `dbt-schema-builder-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/PKG-INFO` & `dbt-schema-builder-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-schema-builder
-Version: 0.4.7
+Version: 0.4.8
 Summary: Automate management of PII redacted schemas for dbt projects.
 Home-page: https://github.com/edx/dbt-schema-builder
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx dbt schema builder
 Platform: UNKNOWN
```

### Comparing `dbt-schema-builder-0.4.7/README.rst` & `dbt-schema-builder-0.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder/app.py` & `dbt-schema-builder-0.4.8/dbt_schema_builder/app.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder/builder.py` & `dbt-schema-builder-0.4.8/dbt_schema_builder/builder.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder/queries.py` & `dbt-schema-builder-0.4.8/dbt_schema_builder/queries.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder/relation.py` & `dbt-schema-builder-0.4.8/dbt_schema_builder/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder/schema.py` & `dbt-schema-builder-0.4.8/dbt_schema_builder/schema.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder/schema_builder.py` & `dbt-schema-builder-0.4.8/dbt_schema_builder/schema_builder.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder/snowflake_keywords.yml` & `dbt-schema-builder-0.4.8/dbt_schema_builder/snowflake_keywords.yml`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder/templates/model_sql_pii.tpl` & `dbt-schema-builder-0.4.8/dbt_schema_builder/templates/model_sql_pii.tpl`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder/templates/model_sql_safe.tpl` & `dbt-schema-builder-0.4.8/dbt_schema_builder/templates/model_sql_safe.tpl`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/PKG-INFO` & `dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-schema-builder
-Version: 0.4.7
+Version: 0.4.8
 Summary: Automate management of PII redacted schemas for dbt projects.
 Home-page: https://github.com/edx/dbt-schema-builder
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx dbt schema builder
 Platform: UNKNOWN
```

### Comparing `dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/SOURCES.txt` & `dbt-schema-builder-0.4.8/dbt_schema_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/requirements/constraints.txt` & `dbt-schema-builder-0.4.8/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.7/setup.py` & `dbt-schema-builder-0.4.8/setup.py`

 * *Files identical despite different names*

