# Comparing `tmp/watchmen_storage_mysql-16.5.2.tar.gz` & `tmp/watchmen_storage_mysql-16.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_mysql-16.5.2.tar", max compression
+gzip compressed data, was "watchmen_storage_mysql-16.5.3.tar", max compression
```

## Comparing `watchmen_storage_mysql-16.5.2.tar` & `watchmen_storage_mysql-16.5.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.440672 watchmen_storage_mysql-16.5.2/LICENSE
--rw-r--r--   0        0        0      485 2023-05-23 07:54:10.440672 watchmen_storage_mysql-16.5.2/pyproject.toml
--rw-r--r--   0        0        0      258 2023-05-23 07:54:10.440672 watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/__init__.py
--rw-r--r--   0        0        0     2836 2023-05-23 07:54:10.440672 watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/data_source_mysql.py
--rw-r--r--   0        0        0     2197 2023-05-23 07:54:10.440672 watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/script_builder_mysql.py
--rw-r--r--   0        0        0     5301 2023-05-23 07:54:10.440672 watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/storage_mysql.py
--rw-r--r--   0        0        0     1965 2023-05-23 07:54:10.440672 watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/storage_mysql_configuration.py
--rw-r--r--   0        0        0     8699 2023-05-23 07:54:10.440672 watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/table_creator.py
--rw-r--r--   0        0        0    11939 2023-05-23 07:54:10.440672 watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/where_build.py
--rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 watchmen_storage_mysql-16.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.548124 watchmen_storage_mysql-16.5.3/LICENSE
+-rw-r--r--   0        0        0      485 2023-06-05 01:29:03.552124 watchmen_storage_mysql-16.5.3/pyproject.toml
+-rw-r--r--   0        0        0      258 2023-06-05 01:29:03.556124 watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/__init__.py
+-rw-r--r--   0        0        0     2836 2023-06-05 01:29:03.556124 watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/data_source_mysql.py
+-rw-r--r--   0        0        0     2197 2023-06-05 01:29:03.556124 watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/script_builder_mysql.py
+-rw-r--r--   0        0        0     5301 2023-06-05 01:29:03.556124 watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/storage_mysql.py
+-rw-r--r--   0        0        0     1965 2023-06-05 01:29:03.556124 watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/storage_mysql_configuration.py
+-rw-r--r--   0        0        0     8699 2023-06-05 01:29:03.556124 watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/table_creator.py
+-rw-r--r--   0        0        0    11939 2023-06-05 01:29:03.556124 watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/where_build.py
+-rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 watchmen_storage_mysql-16.5.3/PKG-INFO
```

### Comparing `watchmen_storage_mysql-16.5.2/LICENSE` & `watchmen_storage_mysql-16.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/data_source_mysql.py` & `watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/data_source_mysql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/script_builder_mysql.py` & `watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/script_builder_mysql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/storage_mysql.py` & `watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/storage_mysql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/storage_mysql_configuration.py` & `watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/storage_mysql_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/table_creator.py` & `watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/table_creator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.2/src/watchmen_storage_mysql/where_build.py` & `watchmen_storage_mysql-16.5.3/src/watchmen_storage_mysql/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.2/PKG-INFO` & `watchmen_storage_mysql-16.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-mysql
-Version: 16.5.2
+Version: 16.5.3
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0)
 Requires-Dist: cryptography (>=36.0.2,<37.0.0)
-Requires-Dist: watchmen-storage-rds (==16.5.2)
+Requires-Dist: watchmen-storage-rds (==16.5.3)
```

