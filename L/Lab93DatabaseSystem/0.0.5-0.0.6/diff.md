# Comparing `tmp/Lab93DatabaseSystem-0.0.5.tar.gz` & `tmp/Lab93DatabaseSystem-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lab93DatabaseSystem-0.0.5.tar", last modified: Sun May 14 20:06:50 2023, max compression
+gzip compressed data, was "Lab93DatabaseSystem-0.0.6.tar", last modified: Mon Jun  5 17:15:13 2023, max compression
```

## Comparing `Lab93DatabaseSystem-0.0.5.tar` & `Lab93DatabaseSystem-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.772989 Lab93DatabaseSystem-0.0.5/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      915 2023-05-14 20:06:50.769656 Lab93DatabaseSystem-0.0.5/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      626 2023-05-14 20:06:13.000000 Lab93DatabaseSystem-0.0.5/pyproject.toml
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      386 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.5/readme.md
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-05-14 20:06:50.772989 Lab93DatabaseSystem-0.0.5/setup.cfg
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.749656 Lab93DatabaseSystem-0.0.5/src/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.756322 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     5724 2023-05-14 19:22:15.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.762989 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.769656 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     8791 2023-05-14 20:03:54.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      928 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.759656 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      915 2023-05-14 20:06:50.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      469 2023-05-14 20:06:50.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/SOURCES.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-05-14 20:06:50.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/dependency_links.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       20 2023-05-14 20:06:50.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/top_level.txt
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-05 17:15:13.735054 Lab93DatabaseSystem-0.0.6/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      915 2023-06-05 17:15:13.735054 Lab93DatabaseSystem-0.0.6/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      626 2023-06-05 17:14:32.000000 Lab93DatabaseSystem-0.0.6/pyproject.toml
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      386 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.6/readme.md
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-06-05 17:15:13.735054 Lab93DatabaseSystem-0.0.6/setup.cfg
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-05 17:15:13.715053 Lab93DatabaseSystem-0.0.6/src/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-05 17:15:13.718386 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     6388 2023-05-14 21:05:47.000000 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-05 17:15:13.728387 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem/submodules/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-05 17:15:13.731721 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem/submodules/DatabaseAPI/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)    14938 2023-06-05 17:13:45.000000 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      928 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem/submodules/DatabaseAPI/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem/submodules/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-05 17:15:13.728387 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem.egg-info/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      915 2023-06-05 17:15:13.000000 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem.egg-info/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      469 2023-06-05 17:15:13.000000 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem.egg-info/SOURCES.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-06-05 17:15:13.000000 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem.egg-info/dependency_links.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       20 2023-06-05 17:15:13.000000 Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem.egg-info/top_level.txt
```

### Comparing `Lab93DatabaseSystem-0.0.5/PKG-INFO` & `Lab93DatabaseSystem-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lab93DatabaseSystem
-Version: 0.0.5
+Version: 0.0.6
 Summary: An API for object persistence scriptability.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/guyyatsu/Lab93-DatabaseSystem
 Project-URL: Bug Tracker, https://github.com/guyyatsu/Lab93-DatabaseSystem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Lab93DatabaseSystem-0.0.5/pyproject.toml` & `Lab93DatabaseSystem-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Lab93DatabaseSystem"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Hunter Dale", email="hunter@guyyatsu.me" },
 ]
 
 description = "An API for object persistence scriptability."
 readme = "readme.md"
 requires-python = ">=3.10"
```

### Comparing `Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/__init__.py` & `Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 new and unique columns to this table provided they do not conflict with the
 schema.
 """
 
 
 ''' In-House framework for interacting with database objects. '''
 from .submodules.DatabaseAPI import SQLite3
+from Lab93Cryptogram import CryptographyMethodsAPI
 
 
 def buildAdministratorDatabase( database: str="./sqlite3.db", **config ):
     """
     The buildAdministratorDatabase function requires a string, `database`,
     that defines a path to a .db file, and an optional config dictionary.
 
@@ -123,7 +124,20 @@
                 column_type = config[table]["columns"][column]
                 SQLite3.newColumn( database,
                                    table=str(table),
                                    column=str(column),
                                    column_type=column_type, ); print(
                     f"    --{str(column).title()} column created."
                 )
+
+def populateAdministratorDatabase( database: str="./sqlite3.db",
+                                   keyfile:  str="./keyfile.key" ):
+
+    while True:
+        username = str(input(f"Type the name of the user to update credentials for: "))
+        credentials_entry = SQLite3.selectRow( database,
+                                                column='*',
+                                                table='credentials',
+                                                header='username',
+                                                value=username       )[0]
+        if len( credentials_entry ) > 0: pass
+
```

### Comparing `Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py` & `Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py`

 * *Files identical despite different names*

### Comparing `Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/PKG-INFO` & `Lab93DatabaseSystem-0.0.6/src/Lab93DatabaseSystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lab93DatabaseSystem
-Version: 0.0.5
+Version: 0.0.6
 Summary: An API for object persistence scriptability.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/guyyatsu/Lab93-DatabaseSystem
 Project-URL: Bug Tracker, https://github.com/guyyatsu/Lab93-DatabaseSystem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

