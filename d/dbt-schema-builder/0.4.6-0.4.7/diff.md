# Comparing `tmp/dbt-schema-builder-0.4.6.tar.gz` & `tmp/dbt-schema-builder-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-schema-builder-0.4.6.tar", last modified: Wed May 17 13:42:58 2023, max compression
+gzip compressed data, was "dbt-schema-builder-0.4.7.tar", last modified: Mon Jun  5 13:41:08 2023, max compression
```

## Comparing `dbt-schema-builder-0.4.6.tar` & `dbt-schema-builder-0.4.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4022 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/dbt_schema_builder/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6649 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/app.py
--rw-r--r--   0 runner    (1001) docker     (122)    24273 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/queries.py
--rw-r--r--   0 runner    (1001) docker     (122)     9343 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/relation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3904 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2798 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/schema_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/snowflake_keywords.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/dbt_schema_builder/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/templates/model_sql_pii.tpl
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/templates/model_sql_safe.tpl
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-17 13:42:58.733180 dbt-schema-builder-0.4.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5314 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4022 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/dbt_schema_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24281 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9373 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/relation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3904 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/schema_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/snowflake_keywords.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/dbt_schema_builder/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/templates/model_sql_pii.tpl
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/dbt_schema_builder/templates/model_sql_safe.tpl
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-05 13:41:08.000000 dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-05 13:41:08.516207 dbt-schema-builder-0.4.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5314 2023-06-05 13:41:03.000000 dbt-schema-builder-0.4.7/setup.py
```

### Comparing `dbt-schema-builder-0.4.6/LICENSE.txt` & `dbt-schema-builder-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.6/PKG-INFO` & `dbt-schema-builder-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-schema-builder
-Version: 0.4.6
+Version: 0.4.7
 Summary: Automate management of PII redacted schemas for dbt projects.
 Home-page: https://github.com/edx/dbt-schema-builder
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx dbt schema builder
 Platform: UNKNOWN
```

### Comparing `dbt-schema-builder-0.4.6/README.rst` & `dbt-schema-builder-0.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder/app.py` & `dbt-schema-builder-0.4.7/dbt_schema_builder/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Class to represent an application whose data is managed by DBT and provides
     functionality for updating its downstreams. An app can be backed by multiple
     raw schemas.
     """
 
     def __init__(
         self, raw_schemas, app, app_path, design_file_path, current_raw_sources,
-        current_downstream_sources, database
+        current_downstream_sources, database, no_pii=False
     ):
 
         self.raw_schemas = raw_schemas
         self.app = app
         self.app_path = app_path
         self.design_file_path = design_file_path
         self.current_raw_sources = current_raw_sources
@@ -38,30 +38,43 @@
             ],
             "models": [],
         }
 
         # Create a new, empty object to store a new version of our downstream
         # sources so we don't get any tables / models that may have been
         # deleted since the last run.
-        self.new_downstream_sources = {
+        self.new_downstream_sources = self._generate_downstream_sources(database, no_pii)
+
+    def _generate_downstream_sources(self, database, no_pii=False):
+        """
+        Generates the object to store the version of the downstream
+        sources so we don't get any tables / models that may have been
+        deleted since the last run. If no_pii flag is set we will exclude
+        the downstream source name for that.
+        """
+        ret_val = {
             "version": 2,
             "sources": [
                 {
                     "name": self.safe_downstream_source_name,
                     "database": database,
                     "tables": [],
-                },
+                }
+            ],
+            "models": [],
+        }
+        if not no_pii:
+            ret_val['sources'].append(
                 {
                     "name": self.pii_downstream_source_name,
                     "database": database,
                     "tables": [],
-                },
-            ],
-            "models": [],
-        }
+                }
+            )
+        return ret_val
 
     def __repr__(self):
         """
         Makes debugging less of a pain
         """
         return self.app
 
@@ -131,29 +144,22 @@
                     )
 
     def update_trifecta_models(self, relation, no_pii=False):
         """
         Given a relation, add it to the 'trifecta'. These are the PII and safe views
         constructed from the raw data.
         """
-        if no_pii:
-            for relation_name in [
-                relation.new_safe_relation_name,
-            ]:
-                self.add_model_to_new_schema(
-                    relation_name, relation.meta_data
-                )
-        else:
-            for relation_name in [
+        relations = [relation.new_safe_relation_name] if no_pii else [
                 relation.new_pii_relation_name,
                 relation.new_safe_relation_name,
-            ]:
-                self.add_model_to_new_schema(
-                    relation_name, relation.meta_data
-                )
+            ]
+        for relation_name in relations:
+            self.add_model_to_new_schema(
+                relation_name, relation.meta_data
+            )
 
     def add_model_to_new_schema(self, new_relation_name, model_meta_data):
         """
         Add models and their columns to a schema that is currently being generated.
         """
         # Add our table to the "models" list in the new schema
         self.new_schema["models"].append({"name": new_relation_name})
```

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder/builder.py` & `dbt-schema-builder-0.4.7/dbt_schema_builder/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,15 +522,15 @@
                     self.downstream_sources_allow_list
                 )
                 raw_schema.relations.append(relation)
             app_raw_schemas.append(raw_schema)
 
         app_object = App(
             app_raw_schemas, app_destination_schema, app_path, design_file_path, current_raw_sources,
-            current_downstream_sources, app_destination_database
+            current_downstream_sources, app_destination_database, no_pii
         )
 
         logger.info("Building schema for the {} app".format(app_object.app))
 
         self.clean_sql_files(app_object.app, app_path)
 
         # Go through each raw schema that backs this Application, building out
```

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder/queries.py` & `dbt-schema-builder-0.4.7/dbt_schema_builder/queries.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder/relation.py` & `dbt-schema-builder-0.4.7/dbt_schema_builder/relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,27 +85,27 @@
         current_raw_source = None
         current_safe_downstream_source = None
         current_pii_downstream_source = None
 
         if current_raw_sources and "sources" in current_raw_sources:
             for source in current_raw_sources["sources"]:
                 for table in source["tables"]:
-                    if table["name"] == self.source_relation_name:
+                    if table and table["name"] == self.source_relation_name:
                         current_raw_source = table
                         break
 
         if current_downstream_sources and "sources" in current_downstream_sources:
             for source in current_downstream_sources["sources"]:
                 if source["name"] == self.app:
                     for table in source["tables"]:
-                        if table["name"] == self.source_relation_name:
+                        if table and table["name"] == self.source_relation_name:
                             current_safe_downstream_source = table
                 elif source["name"] == "{}_PII".format(self.app):
                     for table in source["tables"]:
-                        if table["name"] == self.source_relation_name:
+                        if table and table["name"] == self.source_relation_name:
                             current_pii_downstream_source = table
 
                 if current_safe_downstream_source and current_pii_downstream_source:
                     break
 
         return (
             current_raw_source,
```

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder/schema.py` & `dbt-schema-builder-0.4.7/dbt_schema_builder/schema.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder/schema_builder.py` & `dbt-schema-builder-0.4.7/dbt_schema_builder/schema_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         help="Which target to load for the given profile",
     )
     base_subparser.add_argument(
         "--nopii",
         required=False,
         action='store_true',
         help="Whether or not to supress PII models and sources",
+        default=False,
     )
     subs = p.add_subparsers(title="Available sub-commands", dest="command")
 
     build_sub = subs.add_parser(
         "build",
         parents=[base_subparser],
         help="Creates or updates schema.yml files from database catalog",
@@ -86,20 +87,16 @@
 def handle(args):
     """
     Execute the given command. Currently only "build" exists, but it can be expanded here.
     """
     parsed = parse_args(args)
 
     if parsed.command == "build":
-        if parsed.nopii:
-            task = SchemaBuilderTask(parsed)
-            task.run(no_pii=True)
-        else:
-            task = SchemaBuilderTask(parsed)
-            task.run()
+        task = SchemaBuilderTask(parsed)
+        task.run(no_pii=parsed.nopii)
 
 
 def main(args=None):
     """
     Do main things.
     """
     if args is None:
```

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder/snowflake_keywords.yml` & `dbt-schema-builder-0.4.7/dbt_schema_builder/snowflake_keywords.yml`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder/templates/model_sql_pii.tpl` & `dbt-schema-builder-0.4.7/dbt_schema_builder/templates/model_sql_pii.tpl`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder/templates/model_sql_safe.tpl` & `dbt-schema-builder-0.4.7/dbt_schema_builder/templates/model_sql_safe.tpl`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/PKG-INFO` & `dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-schema-builder
-Version: 0.4.6
+Version: 0.4.7
 Summary: Automate management of PII redacted schemas for dbt projects.
 Home-page: https://github.com/edx/dbt-schema-builder
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx dbt schema builder
 Platform: UNKNOWN
```

### Comparing `dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/SOURCES.txt` & `dbt-schema-builder-0.4.7/dbt_schema_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.6/requirements/constraints.txt` & `dbt-schema-builder-0.4.7/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.6/setup.py` & `dbt-schema-builder-0.4.7/setup.py`

 * *Files identical despite different names*

