# Comparing `tmp/bsc_utils-1.0.0.tar.gz` & `tmp/bsc_utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsc_utils-1.0.0.tar", last modified: Mon May 15 03:18:10 2023, max compression
+gzip compressed data, was "bsc_utils-1.0.1.tar", last modified: Mon Jun  5 06:44:39 2023, max compression
```

## Comparing `bsc_utils-1.0.0.tar` & `bsc_utils-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 03:18:10.492605 bsc_utils-1.0.0/
--rw-rw-rw-   0        0        0       26 2023-05-15 03:09:29.000000 bsc_utils-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      547 2023-05-15 03:18:10.491609 bsc_utils-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-15 02:48:57.000000 bsc_utils-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 03:18:10.475559 bsc_utils-1.0.0/bsc_utils/
--rw-rw-rw-   0        0        0       21 2023-05-15 03:16:58.000000 bsc_utils-1.0.0/bsc_utils/__init__.py
--rw-rw-rw-   0        0        0      402 2023-05-12 03:53:41.000000 bsc_utils-1.0.0/bsc_utils/config.py
--rw-rw-rw-   0        0        0     1917 2023-05-12 08:33:35.000000 bsc_utils-1.0.0/bsc_utils/database.py
--rw-rw-rw-   0        0        0       44 2023-05-12 08:32:56.000000 bsc_utils-1.0.0/bsc_utils/exceptions.py
--rw-rw-rw-   0        0        0      193 2023-04-24 03:32:31.000000 bsc_utils-1.0.0/bsc_utils/helpers.py
--rw-rw-rw-   0        0        0        0 2023-04-20 06:45:05.000000 bsc_utils-1.0.0/bsc_utils/visual.py
-drwxrwxrwx   0        0        0        0 2023-05-15 03:18:10.488595 bsc_utils-1.0.0/bsc_utils.egg-info/
--rw-rw-rw-   0        0        0      547 2023-05-15 03:18:10.000000 bsc_utils-1.0.0/bsc_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-15 03:18:10.000000 bsc_utils-1.0.0/bsc_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 03:18:10.000000 bsc_utils-1.0.0/bsc_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-05-15 03:18:10.000000 bsc_utils-1.0.0/bsc_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 03:18:10.000000 bsc_utils-1.0.0/bsc_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-05-12 08:51:05.000000 bsc_utils-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 03:18:10.493608 bsc_utils-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1083 2023-05-15 03:04:43.000000 bsc_utils-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:44:39.296527 bsc_utils-1.0.1/
+-rw-rw-rw-   0        0        0       26 2023-05-15 03:09:29.000000 bsc_utils-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      547 2023-06-05 06:44:39.291513 bsc_utils-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-15 02:48:57.000000 bsc_utils-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 06:44:39.202776 bsc_utils-1.0.1/bsc_utils/
+-rw-rw-rw-   0        0        0       21 2023-06-05 06:41:30.000000 bsc_utils-1.0.1/bsc_utils/__init__.py
+-rw-rw-rw-   0        0        0      402 2023-05-12 03:53:41.000000 bsc_utils-1.0.1/bsc_utils/config.py
+-rw-rw-rw-   0        0        0     2240 2023-06-01 09:15:36.000000 bsc_utils-1.0.1/bsc_utils/database.py
+-rw-rw-rw-   0        0        0       44 2023-05-12 08:32:56.000000 bsc_utils-1.0.1/bsc_utils/exceptions.py
+-rw-rw-rw-   0        0        0      298 2023-06-05 06:40:42.000000 bsc_utils-1.0.1/bsc_utils/helpers.py
+-rw-rw-rw-   0        0        0     2171 2023-06-05 06:40:42.000000 bsc_utils-1.0.1/bsc_utils/visual.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:44:39.281988 bsc_utils-1.0.1/bsc_utils.egg-info/
+-rw-rw-rw-   0        0        0      547 2023-06-05 06:44:38.000000 bsc_utils-1.0.1/bsc_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-06-05 06:44:38.000000 bsc_utils-1.0.1/bsc_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 06:44:38.000000 bsc_utils-1.0.1/bsc_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-06-05 06:44:38.000000 bsc_utils-1.0.1/bsc_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 06:44:38.000000 bsc_utils-1.0.1/bsc_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      128 2023-06-05 06:40:42.000000 bsc_utils-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 06:44:39.297029 bsc_utils-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1083 2023-05-15 03:04:43.000000 bsc_utils-1.0.1/setup.py
```

### Comparing `bsc_utils-1.0.0/PKG-INFO` & `bsc_utils-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsc_utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Util Functions for BSC Quants
 Home-page: https://github.com/dang-trung/bsc-utils
 Author: Trung Dang
 Author-email: trungd@bsc.com.vn
 Maintainer: Trung Dang
 Maintainer-email: trungd@bsc.com.vn
 License: MIT
```

### Comparing `bsc_utils-1.0.0/bsc_utils/database.py` & `bsc_utils-1.0.1/bsc_utils/database.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from typing import Union
 
 import sqlite3
 import oracledb
+import pandas as pd
 import pymssql
 
 import bsc_utils.config as config
 from bsc_utils.helpers import dict_factory
 from bsc_utils.exceptions import NotDatabaseError
 
 
@@ -38,34 +39,48 @@
 
 
 def query(
     database: Database,
     query: str,
     params: Union[list, tuple] = None,
     fetch: bool = True,
-    as_dict: bool = True
-):
-
+    as_df: bool = True,
+    index_col: str = None
+) -> Union[list, pd.DataFrame]:
     con = connect(database)
-    if database == Database.MSSQL and as_dict:
-        cur = con.cursor(as_dict)
+    if database == Database.MSSQL:
+        cur = con.cursor(as_dict=True)
 
-    if database == Database.SQLITE and as_dict:
+    if database == Database.SQLITE:
         con.row_factory = dict_factory
         cur = con.cursor()
 
     if database == Database.ORACLE:
         cur = con.cursor()
 
     cur.execute(query) if params is None else (
         cur.executemany(query, params)
         if isinstance(params, list) else cur.execute(query, params)
     )
 
-    if database == Database.ORACLE and as_dict:
+    if database == Database.ORACLE:
         cols = [col[0] for col in cur.description]
         cur.rowfactory = lambda *args: dict(zip(cols, args))
 
-    obj = cur.fetchall() if fetch else None
+    obj = None
+    if fetch:
+        obj = cur.fetchall()
+        if as_df:
+            obj = make_tabular(obj, index_col)
+            
     con.commit()
     con.close()
+
     return obj
+
+
+def make_tabular(obj: list[dict], index_col: str) -> pd.DataFrame:
+    df = pd.DataFrame(obj)
+    if index_col:
+        df.set_index(index_col, inplace=True)
+
+    return df
```

### Comparing `bsc_utils-1.0.0/bsc_utils.egg-info/PKG-INFO` & `bsc_utils-1.0.1/bsc_utils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsc-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Util Functions for BSC Quants
 Home-page: https://github.com/dang-trung/bsc-utils
 Author: Trung Dang
 Author-email: trungd@bsc.com.vn
 Maintainer: Trung Dang
 Maintainer-email: trungd@bsc.com.vn
 License: MIT
```

### Comparing `bsc_utils-1.0.0/setup.py` & `bsc_utils-1.0.1/setup.py`

 * *Files identical despite different names*

