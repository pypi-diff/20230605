# Comparing `tmp/databaseRestoreIntegrity-1.0.3.tar.gz` & `tmp/databaseRestoreIntegrity-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databaseRestoreIntegrity-1.0.3.tar", last modified: Mon Jun  5 09:45:56 2023, max compression
+gzip compressed data, was "databaseRestoreIntegrity-1.0.4.tar", last modified: Mon Jun  5 09:49:07 2023, max compression
```

## Comparing `databaseRestoreIntegrity-1.0.3.tar` & `databaseRestoreIntegrity-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:45:56.886667 databaseRestoreIntegrity-1.0.3/
--rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 02:34:52.000000 databaseRestoreIntegrity-1.0.3/LICENSE.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 03:13:57.000000 databaseRestoreIntegrity-1.0.3/MANIFEST.in
--rw-r--r--   0 mhasan     (502) staff       (20)     3613 2023-06-05 09:45:56.886751 databaseRestoreIntegrity-1.0.3/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)     1921 2023-06-05 05:47:06.000000 databaseRestoreIntegrity-1.0.3/README.md
--rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 03:25:16.000000 databaseRestoreIntegrity-1.0.3/pyproject.toml
--rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-05 09:45:56.891979 databaseRestoreIntegrity-1.0.3/setup.cfg
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:45:56.878491 databaseRestoreIntegrity-1.0.3/src/
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:45:56.882068 databaseRestoreIntegrity-1.0.3/src/databaseRestoreIntegrity/
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 03:23:11.000000 databaseRestoreIntegrity-1.0.3/src/databaseRestoreIntegrity/__init__.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2558 2023-06-05 09:35:28.000000 databaseRestoreIntegrity-1.0.3/src/databaseRestoreIntegrity/mysql.py
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:45:56.886173 databaseRestoreIntegrity-1.0.3/src/databaseRestoreIntegrity.egg-info/
--rw-r--r--   0 mhasan     (502) staff       (20)     3613 2023-06-05 09:45:56.000000 databaseRestoreIntegrity-1.0.3/src/databaseRestoreIntegrity.egg-info/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)      345 2023-06-05 09:45:56.000000 databaseRestoreIntegrity-1.0.3/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-05 09:45:56.000000 databaseRestoreIntegrity-1.0.3/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
--rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-05 09:45:56.000000 databaseRestoreIntegrity-1.0.3/src/databaseRestoreIntegrity.egg-info/top_level.txt
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:49:07.879921 databaseRestoreIntegrity-1.0.4/
+-rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 02:34:52.000000 databaseRestoreIntegrity-1.0.4/LICENSE.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 03:13:57.000000 databaseRestoreIntegrity-1.0.4/MANIFEST.in
+-rw-r--r--   0 mhasan     (502) staff       (20)     3651 2023-06-05 09:49:07.880046 databaseRestoreIntegrity-1.0.4/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)     1959 2023-06-05 09:48:07.000000 databaseRestoreIntegrity-1.0.4/README.md
+-rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 03:25:16.000000 databaseRestoreIntegrity-1.0.4/pyproject.toml
+-rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-05 09:49:07.881384 databaseRestoreIntegrity-1.0.4/setup.cfg
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:49:07.866582 databaseRestoreIntegrity-1.0.4/src/
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:49:07.876012 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity/
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 03:23:11.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity/__init__.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2558 2023-06-05 09:35:28.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity/mysql.py
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-05 09:49:07.879468 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/
+-rw-r--r--   0 mhasan     (502) staff       (20)     3651 2023-06-05 09:49:07.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)      345 2023-06-05 09:49:07.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-05 09:49:07.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-05 09:49:07.000000 databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/top_level.txt
```

### Comparing `databaseRestoreIntegrity-1.0.3/LICENSE.txt` & `databaseRestoreIntegrity-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.3/PKG-INFO` & `databaseRestoreIntegrity-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
@@ -53,15 +53,16 @@
 database1._create_tmp_table('actual_rds')
 
 def check_consistency():
     unconsistent_tabels = []
     conn = database.connection()
     check_consistency = conn.cursor()
     check_consistency.execute("USE restore_consistency")
-    check_consistency.execute("SELECT tables_name,records_count FROM (SELECT tables_name,records_count FROM restore_rds UNION ALL SELECT tables_name,records_count FROM actual_rds) tbl GROUP BY tables_name, records_count HAVING count(*) = 1 ORDER BY tables_name")
+    check_consistency.execute("SELECT tables_name,records_count,hostname FROM (SELECT tables_name,records_count,hostname FROM restore_rds UNION ALL SELECT tables_name,records_count,hostname FROM actual_rds) tbl GROUP BY tables_name, hostname, records_count HAVING count(*) = 1 ORDER BY tables_name")
+
     result = check_consistency.fetchall()
     print(tabulate(result, headers=['tables_name', 'records_count'], tablefmt='psql'))
 check_consistency()
 ```
```

### Comparing `databaseRestoreIntegrity-1.0.3/README.md` & `databaseRestoreIntegrity-1.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 database1._create_tmp_table('actual_rds')
 
 def check_consistency():
     unconsistent_tabels = []
     conn = database.connection()
     check_consistency = conn.cursor()
     check_consistency.execute("USE restore_consistency")
-    check_consistency.execute("SELECT tables_name,records_count FROM (SELECT tables_name,records_count FROM restore_rds UNION ALL SELECT tables_name,records_count FROM actual_rds) tbl GROUP BY tables_name, records_count HAVING count(*) = 1 ORDER BY tables_name")
+    check_consistency.execute("SELECT tables_name,records_count,hostname FROM (SELECT tables_name,records_count,hostname FROM restore_rds UNION ALL SELECT tables_name,records_count,hostname FROM actual_rds) tbl GROUP BY tables_name, hostname, records_count HAVING count(*) = 1 ORDER BY tables_name")
+
     result = check_consistency.fetchall()
     print(tabulate(result, headers=['tables_name', 'records_count'], tablefmt='psql'))
 check_consistency()
 ```
```

### Comparing `databaseRestoreIntegrity-1.0.3/setup.cfg` & `databaseRestoreIntegrity-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = databaseRestoreIntegrity
-version = 1.0.3
+version = 1.0.4
 author = Maihraj Hasan
 author_email = maihrajhasan@gmail.com
 description = A package to check mysql restore integrity check
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `databaseRestoreIntegrity-1.0.3/src/databaseRestoreIntegrity/mysql.py` & `databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity/mysql.py`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.3/src/databaseRestoreIntegrity.egg-info/PKG-INFO` & `databaseRestoreIntegrity-1.0.4/src/databaseRestoreIntegrity.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
@@ -53,15 +53,16 @@
 database1._create_tmp_table('actual_rds')
 
 def check_consistency():
     unconsistent_tabels = []
     conn = database.connection()
     check_consistency = conn.cursor()
     check_consistency.execute("USE restore_consistency")
-    check_consistency.execute("SELECT tables_name,records_count FROM (SELECT tables_name,records_count FROM restore_rds UNION ALL SELECT tables_name,records_count FROM actual_rds) tbl GROUP BY tables_name, records_count HAVING count(*) = 1 ORDER BY tables_name")
+    check_consistency.execute("SELECT tables_name,records_count,hostname FROM (SELECT tables_name,records_count,hostname FROM restore_rds UNION ALL SELECT tables_name,records_count,hostname FROM actual_rds) tbl GROUP BY tables_name, hostname, records_count HAVING count(*) = 1 ORDER BY tables_name")
+
     result = check_consistency.fetchall()
     print(tabulate(result, headers=['tables_name', 'records_count'], tablefmt='psql'))
 check_consistency()
 ```
```

