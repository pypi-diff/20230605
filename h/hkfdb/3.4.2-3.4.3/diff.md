# Comparing `tmp/hkfdb-3.4.2.tar.gz` & `tmp/hkfdb-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.4.2.tar", last modified: Mon Jun  5 05:24:32 2023, max compression
+gzip compressed data, was "hkfdb-3.4.3.tar", last modified: Mon Jun  5 12:38:05 2023, max compression
```

## Comparing `hkfdb-3.4.2.tar` & `hkfdb-3.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 05:24:32.232151 hkfdb-3.4.2/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.4.2/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-06-05 05:24:32.231992 hkfdb-3.4.2/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.4.2/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 05:24:32.230877 hkfdb-3.4.2/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   107582 2023-06-05 05:21:10.000000 hkfdb-3.4.2/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.4.2/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 05:24:32.231817 hkfdb-3.4.2/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-06-05 05:24:31.000000 hkfdb-3.4.2/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-05 05:24:32.000000 hkfdb-3.4.2/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-05 05:24:31.000000 hkfdb-3.4.2/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       44 2023-06-05 05:24:31.000000 hkfdb-3.4.2/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-05 05:24:31.000000 hkfdb-3.4.2/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-05 05:24:32.232199 hkfdb-3.4.2/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      763 2023-06-05 05:23:11.000000 hkfdb-3.4.2/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 12:38:05.811287 hkfdb-3.4.3/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.4.3/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-06-05 12:38:05.811020 hkfdb-3.4.3/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.4.3/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 12:38:05.810064 hkfdb-3.4.3/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   107897 2023-06-05 12:36:51.000000 hkfdb-3.4.3/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.4.3/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 12:38:05.810834 hkfdb-3.4.3/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-06-05 12:38:05.000000 hkfdb-3.4.3/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-05 12:38:05.000000 hkfdb-3.4.3/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-05 12:38:05.000000 hkfdb-3.4.3/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       44 2023-06-05 12:38:05.000000 hkfdb-3.4.3/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-05 12:38:05.000000 hkfdb-3.4.3/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-05 12:38:05.811336 hkfdb-3.4.3/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      763 2023-06-05 12:37:22.000000 hkfdb-3.4.3/setup.py
```

### Comparing `hkfdb-3.4.2/LICENSE` & `hkfdb-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.4.2/PKG-INFO` & `hkfdb-3.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.4.2
+Version: 3.4.3
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.4.2/README.md` & `hkfdb-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.4.2/hkfdb/Database.py` & `hkfdb-3.4.3/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1460,16 +1460,15 @@
 
                 return df
 
         else:
             err_msg =  'index_name missing'
             print(err_msg)
 
-    def get_hk_stock_plate_const(self, plate_name):
-
+    def get_hk_stock_plate_const(self, plate_name, sort_mkt_cap=False):
         if len(plate_name) > 0:
 
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'hk_stock_plate_const'
             plate_name_str = 'plate_name=' + plate_name
             link_str = link_url + plate_name_str + '&' + token_str + '&' + database_str
@@ -1480,21 +1479,26 @@
 
                 result = json.loads(json.loads(response.content).replace("'", "\""))
 
                 df = pd.DataFrame(result)
                 df['code'] = df['code'].astype(str)
                 df['code'] = df['code'].str.zfill(5)
 
+                if sort_mkt_cap:
+                    info = self.get_basic_hk_stock_info()
+                    info = info[['code', 'market_capital']]
+                    df = pd.merge(df, info, on='code', how='inner')
+                    df = df.sort_values(by='market_capital', ascending=False)
+
                 return df
 
         else:
-            err_msg =  'index_name missing'
+            err_msg = 'index_name missing'
             print(err_msg)
 
-
     def get_all_hk_index_name(self):
 
         link_url = 'http://www.hkfdb.net/data_api?'
         token_str = 'token=' + str(self.authToken)
         database_str = 'database=' + 'all_hk_index_name'
         link_str = link_url + '&' + token_str + '&' + database_str
```

### Comparing `hkfdb-3.4.2/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.4.3/hkfdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.4.2
+Version: 3.4.3
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

