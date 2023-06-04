# Comparing `tmp/pigeonsai-0.0.3.tar.gz` & `tmp/pigeonsai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-0.0.3.tar", last modified: Sat Jun  3 00:16:04 2023, max compression
+gzip compressed data, was "pigeonsai-0.0.4.tar", last modified: Sun Jun  4 22:36:37 2023, max compression
```

## Comparing `pigeonsai-0.0.3.tar` & `pigeonsai-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:16:04.799834 pigeonsai-0.0.3/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-03 00:16:04.799669 pigeonsai-0.0.3/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.3/README.md
--rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-03 00:16:04.799885 pigeonsai-0.0.3/setup.cfg
--rw-r--r--   0 ariaattar   (501) staff       (20)     2064 2023-06-03 00:15:54.000000 pigeonsai-0.0.3/setup.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:16:04.797424 pigeonsai-0.0.3/src/
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:16:04.798289 pigeonsai-0.0.3/src/pigeonsai/
--rw-r--r--   0 ariaattar   (501) staff       (20)       32 2023-06-03 00:01:24.000000 pigeonsai-0.0.3/src/pigeonsai/__init__.py
--rw-r--r--   0 ariaattar   (501) staff       (20)     2465 2023-06-03 00:15:50.000000 pigeonsai-0.0.3/src/pigeonsai/pigeonsdb.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:16:04.799105 pigeonsai-0.0.3/src/pigeonsai.egg-info/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-03 00:16:04.000000 pigeonsai-0.0.3/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-03 00:16:04.000000 pigeonsai-0.0.3/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-03 00:16:04.000000 pigeonsai-0.0.3/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       17 2023-06-03 00:16:04.000000 pigeonsai-0.0.3/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-03 00:16:04.000000 pigeonsai-0.0.3/src/pigeonsai.egg-info/top_level.txt
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-03 00:16:04.799273 pigeonsai-0.0.3/tests/
--rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.3/tests/test_pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-04 22:36:37.510321 pigeonsai-0.0.4/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-04 22:36:37.510160 pigeonsai-0.0.4/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.4/README.md
+-rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-04 22:36:37.510368 pigeonsai-0.0.4/setup.cfg
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2064 2023-06-04 22:36:32.000000 pigeonsai-0.0.4/setup.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-04 22:36:37.507977 pigeonsai-0.0.4/src/
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-04 22:36:37.508869 pigeonsai-0.0.4/src/pigeonsai/
+-rw-r--r--   0 ariaattar   (501) staff       (20)       32 2023-06-03 00:01:24.000000 pigeonsai-0.0.4/src/pigeonsai/__init__.py
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2601 2023-06-04 22:33:11.000000 pigeonsai-0.0.4/src/pigeonsai/pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-04 22:36:37.509684 pigeonsai-0.0.4/src/pigeonsai.egg-info/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-04 22:36:37.000000 pigeonsai-0.0.4/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-04 22:36:37.000000 pigeonsai-0.0.4/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-04 22:36:37.000000 pigeonsai-0.0.4/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       17 2023-06-04 22:36:37.000000 pigeonsai-0.0.4/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-04 22:36:37.000000 pigeonsai-0.0.4/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-04 22:36:37.509831 pigeonsai-0.0.4/tests/
+-rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.4/tests/test_pigeonsdb.py
```

### Comparing `pigeonsai-0.0.3/PKG-INFO` & `pigeonsai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.3
+Version: 0.0.4
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.3/README.md` & `pigeonsai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pigeonsai-0.0.3/setup.py` & `pigeonsai-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="0.0.3",
+    version="0.0.4",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-0.0.3/src/pigeonsai/pigeonsdb.py` & `pigeonsai-0.0.4/src/pigeonsai/pigeonsdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,16 @@
             "metadata_filters": metadata_filters,
             "keywords": keywords
         }
 
         response = requests.post(url, headers=headers, data=json.dumps(data))
 
         # print the response
-        print(response.text)
+        res = response.text
+        return res
 
     @staticmethod
     def init(API, DB_Name):
         index_p, connect = PigeonsDB.get_db_info(API, DB_Name)
         if connect:
             PigeonsDB.__connection = connect
             PigeonsDB.__index_p = index_p
@@ -44,20 +45,21 @@
         url = "http://ec2-52-14-162-65.us-east-2.compute.amazonaws.com/api/v1/sdk/get-db-info"
         headers = {"Content-Type": "application/json"}
         data = {"api_key": api_key, "dbname": db_name}
         response = requests.post(url, headers=headers, data=json.dumps(data))
 
         # Extract data from the response
         db_info = response.json().get('DB info', {})
+        print(db_info)
         index_p = db_info.get('s3_identifier')
 
         # Create db object with specific keys
         keys = ['dbname', 'user', 'password', 'host']
         connect = {key: db_info.get(key) for key in keys}
-
+        print(connect)
         return index_p, connect
 
 
     @staticmethod
     def add(documents, metadata_list):
         if PigeonsDB.__connection is None:
             print("Error: Connection not initialized.")
@@ -74,7 +76,8 @@
 
         response = requests.post(url, headers=headers, data=json.dumps(data))
 
         # print the response
         print(response.text)
 
 
+PigeonsDB.get_db_info("psk-5debdb081c6649708218d7b2987b475b", "dbtest1")
```

### Comparing `pigeonsai-0.0.3/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-0.0.4/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.3
+Version: 0.0.4
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.3/tests/test_pigeonsdb.py` & `pigeonsai-0.0.4/tests/test_pigeonsdb.py`

 * *Files identical despite different names*

