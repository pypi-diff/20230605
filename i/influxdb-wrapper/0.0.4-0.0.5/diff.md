# Comparing `tmp/influxdb_wrapper-0.0.4.tar.gz` & `tmp/influxdb_wrapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb_wrapper-0.0.4.tar", last modified: Tue May 30 06:25:11 2023, max compression
+gzip compressed data, was "influxdb_wrapper-0.0.5.tar", last modified: Mon Jun  5 06:36:16 2023, max compression
```

## Comparing `influxdb_wrapper-0.0.4.tar` & `influxdb_wrapper-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:11.583121 influxdb_wrapper-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 06:25:11.583121 influxdb_wrapper-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:11.579121 influxdb_wrapper-0.0.4/influxdb_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/influxdb_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/influxdb_wrapper/db_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/influxdb_wrapper/influxdb_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/influxdb_wrapper/mockdb_conn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:11.583121 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 06:25:11.000000 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-30 06:25:11.000000 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:25:11.000000 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 06:25:11.000000 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 06:25:11.000000 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:25:11.583121 influxdb_wrapper-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:11.583121 influxdb_wrapper-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/tests/test_000.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:36:16.986117 influxdb_wrapper-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-05 06:36:16.986117 influxdb_wrapper-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 06:35:56.000000 influxdb_wrapper-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:36:16.986117 influxdb_wrapper-0.0.5/influxdb_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-05 06:35:56.000000 influxdb_wrapper-0.0.5/influxdb_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-05 06:35:56.000000 influxdb_wrapper-0.0.5/influxdb_wrapper/db_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-05 06:35:56.000000 influxdb_wrapper-0.0.5/influxdb_wrapper/influxdb_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-05 06:35:56.000000 influxdb_wrapper-0.0.5/influxdb_wrapper/mockdb_conn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:36:16.986117 influxdb_wrapper-0.0.5/influxdb_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-05 06:36:16.000000 influxdb_wrapper-0.0.5/influxdb_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-05 06:36:16.000000 influxdb_wrapper-0.0.5/influxdb_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:36:16.000000 influxdb_wrapper-0.0.5/influxdb_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 06:36:16.000000 influxdb_wrapper-0.0.5/influxdb_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 06:36:16.000000 influxdb_wrapper-0.0.5/influxdb_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 06:36:16.986117 influxdb_wrapper-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-05 06:35:56.000000 influxdb_wrapper-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:36:16.986117 influxdb_wrapper-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:35:56.000000 influxdb_wrapper-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-05 06:35:56.000000 influxdb_wrapper-0.0.5/tests/test_000.py
```

### Comparing `influxdb_wrapper-0.0.4/PKG-INFO` & `influxdb_wrapper-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: influxdb_wrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: DB management wrapper over influxDB
 Home-page: https://github.com/Phornee/influxdb_wrapper
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Database utilities
 This package contains utilities to access Influx Databases
+It allows to create a influxdb mock... useful for unittesting
```

### Comparing `influxdb_wrapper-0.0.4/influxdb_wrapper/influxdb_conn.py` & `influxdb_wrapper-0.0.5/influxdb_wrapper/influxdb_conn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,38 @@
-from .db_conn import DBConn, DBOpenException, DBExceptionNotOpen, DBGetLockException, DBReleaseLockException
+""" Influx wrapper"""
 from datetime import datetime
-from influxdb import InfluxDBClient
 from copy import deepcopy
+from influxdb import InfluxDBClient
 
+from .db_conn import DBConn, DBOpenException, DBExceptionNotOpen
 
 class InfluxDBConn(DBConn):
+    """ Wrapper over influx API, to make easier to write and read information to/from a influx database
+    """
     def __init__(self):
         super().__init__()
         self.conn = None
 
-    def openConn(self, params, autocommit=True):
+    def open_conn(self, params, autocommit=True):
         host = params['host']
         user = params['user']
         password = params['password']
         bucket = params['bucket']
 
-        self.conn = InfluxDBClient(host=host, username=user, password=password, database=bucket)
+        try:
+            self.conn = InfluxDBClient(host=host, username=user, password=password, database=bucket)
+        except Exception as ex:
+            raise DBOpenException(f'Could not open database. \
+                                    Host={host}, \
+                                    user={user}, \
+                                    password={password}, \
+                                    bucket={bucket}. \
+                                    Error:{ex}') from ex
 
-    def closeConn(self):
+    def close_conn(self):
         self.conn.close()
 
     def insert(self, table, rows):
         if not self.conn:
             raise DBExceptionNotOpen('Database not opened')
 
         points = deepcopy(rows)
@@ -30,41 +41,42 @@
             if 'time' not in point or not point['time']:
                 point['time'] = datetime.utcnow()
 
         self.conn.write_points(points)
 
     def _get_condition_string(self, condition: tuple):
         ret = ''
-        if type(condition[0]) == str:
-            ret = "{}='{}'".format(condition[0], condition[1])
-        elif type(condition[0]) == int:
-            ret = "{}={}".format(condition[0], condition[1])
+        if isinstance(condition[0], str):
+            ret = f"{condition[0]}='{condition[1]}'"
+        elif isinstance(condition[0], int):
+            ret = f"{condition[0]}={condition[1]}"
         return ret
 
     def select(self, table_name: str, tags_conds: tuple, order_by: str = None, order_asc: bool = True, limit: int = 0):
+        """ Get db information
+        Args:
+            table_name (str): Name of the table to be queried
+            tags_conds (tuple): Tuple with (fields, value) to filter the query
+            order_by (str): Field to order by
+            order_asc (bool): If sort order is ASC. DESC if false
+            limit (int): Limit the number of queries retrieved
+        """
+        if self.conn is None:
+            raise DBExceptionNotOpen('Database not opened')
+
         conds_string = ""
 
         if tags_conds:
             conds_string = " WHERE "
 
             conds_string += self._get_condition_string(tags_conds[0])
 
             for cond in tags_conds[1:]:
                 conds_string += " AND " + self._get_condition_string(cond)
 
-        query = """SELECT * from {table} {conditions}
-                ORDER BY {order_by} {direction}
-                LIMIT {limit}""".format(table=table_name,
-                                        conditions=conds_string,
-                                        order_by=order_by,
-                                        direction='ASC' if order_asc else 'DESC',
-                                        limit=limit)
+        query = f"""SELECT * from {table_name} {conds_string}
+                ORDER BY {order_by} {'ASC' if order_asc else 'DESC'}
+                LIMIT {limit}"""
         result_set = self.conn.query(query)
         points = list(result_set.get_points())
 
         return points
-
-    def getLock(self, lockname):
-        raise
-
-    def releaseLock(self, lockname):
-        raise
```

### Comparing `influxdb_wrapper-0.0.4/influxdb_wrapper/mockdb_conn.py` & `influxdb_wrapper-0.0.5/influxdb_wrapper/mockdb_conn.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,48 @@
-from .db_conn import DBConn, DBExceptionNotOpen
+""" Influx mock wrapper"""
+
 from datetime import datetime
 from copy import deepcopy
 
+from .db_conn import DBConn, DBExceptionNotOpen
+
 
 class InfluxMockDBConn(DBConn):
+    """ Wrapper mocking a fake influx connection
+    """
     def __init__(self):
         super().__init__()
         self.db_tables = None
 
-    def openConn(self, params, autocommit=True):
+    def open_conn(self, params, autocommit=True):
         self.db_tables = {}
 
-    def closeConn(self):
-        self.conn.close()
+    def close_conn(self):
+        pass
 
     def insert(self, table, rows):
         if self.db_tables is None:
             raise DBExceptionNotOpen('Database not opened')
 
         points = deepcopy(rows)
         for point in points:
             point["measurement"] = table
             if 'time' not in point or not point['time']:
                 point['time'] = datetime.utcnow()
         self.db_tables[table] = points
 
     def select(self, table_name: str, tags_conds: tuple, order_by: str = None, order_asc: bool = True, limit: int = 0):
+        """ Get db information
+        Args:
+            table_name (str): Name of the table to be queried
+            tags_conds (tuple): Tuple with (fields, value) to filter the query
+            order_by (str): Field to order by
+            order_asc (bool): If sort order is ASC. DESC if false
+            limit (int): Limit the number of queries retrieved
+        """
         if self.db_tables is None:
             raise DBExceptionNotOpen('Database not opened')
 
         result = []
         table = self.db_tables[table_name]
         for row in table:
             fullfills = True
@@ -52,14 +65,7 @@
         if order_by is not None:
             result.sort(reverse=not order_asc, key=lambda x: x[order_by])
 
         # Limit if needed
         result = result[0:limit]
 
         return result
-
-
-    def getLock(self, lockname):
-        raise
-
-    def releaseLock(self, lockname):
-        raise
```

### Comparing `influxdb_wrapper-0.0.4/setup.py` & `influxdb_wrapper-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="influxdb_wrapper",
-    version="0.0.4",
+    version="0.0.5",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="DB management wrapper over influxDB",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/influxdb_wrapper",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'dnspython>=1.16.0',
+        'dnspython==1.16.0',
         'influxdb>=5.3.1',
     ],
     python_requires='>=3.6',
 )
```

