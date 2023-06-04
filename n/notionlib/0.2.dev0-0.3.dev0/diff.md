# Comparing `tmp/notionlib-0.2.dev0.tar.gz` & `tmp/notionlib-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notionlib-0.2.dev0.tar", last modified: Sun Jun  4 20:45:48 2023, max compression
+gzip compressed data, was "notionlib-0.3.dev0.tar", last modified: Sun Jun  4 22:14:19 2023, max compression
```

## Comparing `notionlib-0.2.dev0.tar` & `notionlib-0.3.dev0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 20:45:48.138593 notionlib-0.2.dev0/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       52 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/AUTHORS
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       17 2022-07-14 21:45:57.000000 notionlib-0.2.dev0/BUGS.md
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       56 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/CHANGES.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1092 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/LICENSE
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      397 2022-07-14 21:45:57.000000 notionlib-0.2.dev0/MANIFEST.in
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     3822 2023-06-04 20:45:48.138593 notionlib-0.2.dev0/PKG-INFO
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      465 2023-06-04 20:37:53.000000 notionlib-0.2.dev0/PUBLISH_HOWTO.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     2901 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/README.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      228 2022-07-14 21:45:57.000000 notionlib-0.2.dev0/TODO.md
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 20:45:48.134592 notionlib-0.2.dev0/docs/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7618 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/Makefile
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      287 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/api.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      126 2022-07-14 21:45:57.000000 notionlib-0.2.dev0/docs/api_TODO_MODULE_NAME.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)    10912 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/conf.py
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     5257 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/developer.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      779 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/index.rst
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      864 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/init_sphinx.sh
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      207 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/intro.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7738 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/make.bat
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 20:45:48.138593 notionlib-0.2.dev0/notionlib/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1177 2023-06-04 20:36:54.000000 notionlib-0.2.dev0/notionlib/__init__.py
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)    23555 2023-06-04 20:30:01.000000 notionlib-0.2.dev0/notionlib/notion.py
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 20:45:48.138593 notionlib-0.2.dev0/notionlib.egg-info/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     3822 2023-06-04 20:45:48.000000 notionlib-0.2.dev0/notionlib.egg-info/PKG-INFO
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      462 2023-06-04 20:45:48.000000 notionlib-0.2.dev0/notionlib.egg-info/SOURCES.txt
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)        1 2023-06-04 20:45:48.000000 notionlib-0.2.dev0/notionlib.egg-info/dependency_links.txt
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       10 2023-06-04 20:45:48.000000 notionlib-0.2.dev0/notionlib.egg-info/top_level.txt
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       76 2023-06-04 20:45:17.000000 notionlib-0.2.dev0/pyproject.toml
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       15 2022-07-24 14:13:07.000000 notionlib-0.2.dev0/requirements.txt
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      946 2023-06-04 20:45:48.138593 notionlib-0.2.dev0/setup.cfg
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)     2922 2022-07-14 22:35:14.000000 notionlib-0.2.dev0/setup.py
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 22:14:19.382359 notionlib-0.3.dev0/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       52 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/AUTHORS
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       17 2022-07-14 21:45:57.000000 notionlib-0.3.dev0/BUGS.md
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       56 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/CHANGES.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1092 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/LICENSE
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      397 2022-07-14 21:45:57.000000 notionlib-0.3.dev0/MANIFEST.in
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     3822 2023-06-04 22:14:19.386359 notionlib-0.3.dev0/PKG-INFO
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      465 2023-06-04 20:37:53.000000 notionlib-0.3.dev0/PUBLISH_HOWTO.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     2901 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/README.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      228 2022-07-14 21:45:57.000000 notionlib-0.3.dev0/TODO.md
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 22:14:19.382359 notionlib-0.3.dev0/docs/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7618 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/docs/Makefile
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      287 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/docs/api.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      126 2022-07-14 21:45:57.000000 notionlib-0.3.dev0/docs/api_TODO_MODULE_NAME.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)    10912 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/docs/conf.py
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     5257 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/docs/developer.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      779 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/docs/index.rst
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      864 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/docs/init_sphinx.sh
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      207 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/docs/intro.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7738 2022-07-14 22:06:12.000000 notionlib-0.3.dev0/docs/make.bat
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 22:14:19.382359 notionlib-0.3.dev0/notionlib/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1177 2023-06-04 22:12:49.000000 notionlib-0.3.dev0/notionlib/__init__.py
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)    23718 2023-06-04 22:10:24.000000 notionlib-0.3.dev0/notionlib/notion.py
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 22:14:19.382359 notionlib-0.3.dev0/notionlib.egg-info/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     3822 2023-06-04 22:14:19.000000 notionlib-0.3.dev0/notionlib.egg-info/PKG-INFO
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      462 2023-06-04 22:14:19.000000 notionlib-0.3.dev0/notionlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)        1 2023-06-04 22:14:19.000000 notionlib-0.3.dev0/notionlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       10 2023-06-04 22:14:19.000000 notionlib-0.3.dev0/notionlib.egg-info/top_level.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       76 2023-06-04 20:45:17.000000 notionlib-0.3.dev0/pyproject.toml
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       15 2022-07-24 14:13:07.000000 notionlib-0.3.dev0/requirements.txt
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      946 2023-06-04 22:14:19.386359 notionlib-0.3.dev0/setup.cfg
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)     2922 2022-07-14 22:35:14.000000 notionlib-0.3.dev0/setup.py
```

### Comparing `notionlib-0.2.dev0/LICENSE` & `notionlib-0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `notionlib-0.2.dev0/PKG-INFO` & `notionlib-0.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionlib
-Version: 0.2.dev0
+Version: 0.3.dev0
 Summary: An unofficial Python 3 client for the Notion.so API
 Home-page: https://github.com/jdhp/notion-lib
 Download-URL: 
 Author: Jérémie DECOCK
 Author-email: jd.jdhp@gmail.com
 Maintainer: Jérémie DECOCK
 Maintainer-email: jd.jdhp@gmail.com
```

### Comparing `notionlib-0.2.dev0/README.rst` & `notionlib-0.3.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `notionlib-0.2.dev0/docs/Makefile` & `notionlib-0.3.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `notionlib-0.2.dev0/docs/conf.py` & `notionlib-0.3.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `notionlib-0.2.dev0/docs/developer.rst` & `notionlib-0.3.dev0/docs/developer.rst`

 * *Files identical despite different names*

### Comparing `notionlib-0.2.dev0/docs/index.rst` & `notionlib-0.3.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `notionlib-0.2.dev0/docs/init_sphinx.sh` & `notionlib-0.3.dev0/docs/init_sphinx.sh`

 * *Files identical despite different names*

### Comparing `notionlib-0.2.dev0/docs/make.bat` & `notionlib-0.3.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `notionlib-0.2.dev0/notionlib/__init__.py` & `notionlib-0.3.dev0/notionlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,13 +30,13 @@
 # X.YbN # Beta release         
 # X.YrcN # Release Candidate   
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '0.2.dev0'
+__version__ = '0.3.dev0'
 
 def get_version():
     return __version__
 
 __all__ = ['TODO']
```

### Comparing `notionlib-0.2.dev0/notionlib/notion.py` & `notionlib-0.3.dev0/notionlib/notion.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 SLEEP_ERROR_SEC = 1
 
 
 class Notion:
 
     def __init__(self, api_token):
         self.api_token = api_token
-        #self.api_version = "2022-06-28" # Breaks everything!
-        self.api_version = "2021-08-16"
+        self.api_version = "2022-06-28" # Breaks everything!
+        #self.api_version = "2021-08-16"
 
 
     @property
     def request_header(self):
         header_dict = {
             "Authorization": f"Bearer {self.api_token}",
             "Content-Type": "application/json",
@@ -72,15 +72,15 @@
 
         for k, v in resp.json()["properties"].items():
             value_dict[k] = self.parse_database_property_object(v)
 
         return value_dict
 
 
-    def query_a_database(self, notion_db_id, return_dataframe=False, ignored_properties=None, ignored_properties_type=None, timeout=60):
+    def query_a_database(self, notion_db_id, data_dict=None, return_dataframe=False, ignored_properties=None, ignored_properties_type=None, timeout=60):
         """
         Gets a list of Pages contained in the database.
 
         https://developers.notion.com/reference/post-database-query
 
         Parameters
         ----------
@@ -105,30 +105,34 @@
         """        
         RESERVED_PROPERTY_NAMES = ("created_by", "created_time", "last_edited_by", "last_edited_time", "page_id")
 
         notion_page_dict_list = []
 
         url = f"https://api.notion.com/v1/databases/{notion_db_id}/query"
 
-        requests_data_dict = {
-            "page_size": 100
-        }
+        if data_dict is None:
+            requests_data_dict = {
+                "page_size": 100
+            }
+        else:
+            requests_data_dict = data_dict
 
         if ignored_properties_type is None:
             ignored_properties_type = []
         elif isinstance(ignored_properties_type, str):
             ignored_properties_type = [ignored_properties_type]
 
         if ignored_properties is None:
             ignored_properties = []
         elif isinstance(ignored_properties, str):
             ignored_properties = [ignored_properties]
 
         has_more = True
         while has_more:
+            #print(len(notion_page_dict_list))
             is_successful_request = False
             retry = 10
             while (is_successful_request==False) and (retry > 0):
                 resp = requests.post(url, headers=self.request_header, data=json.dumps(requests_data_dict, default=str), timeout=timeout)
 
                 if resp.status_code == 200:
                     is_successful_request = True
@@ -576,8 +580,8 @@
             # https://developers.notion.com/reference/property-value-object#url-property-values
             self.check_value_type(value, str)
             property_dict["url"] = value
 
         else:
             raise ValueError(f'Unknown property type "{type}"')
 
-        return property_dict
+        return property_dict
```

### Comparing `notionlib-0.2.dev0/notionlib.egg-info/PKG-INFO` & `notionlib-0.3.dev0/notionlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionlib
-Version: 0.2.dev0
+Version: 0.3.dev0
 Summary: An unofficial Python 3 client for the Notion.so API
 Home-page: https://github.com/jdhp/notion-lib
 Download-URL: 
 Author: Jérémie DECOCK
 Author-email: jd.jdhp@gmail.com
 Maintainer: Jérémie DECOCK
 Maintainer-email: jd.jdhp@gmail.com
```

### Comparing `notionlib-0.2.dev0/setup.cfg` & `notionlib-0.3.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `notionlib-0.2.dev0/setup.py` & `notionlib-0.3.dev0/setup.py`

 * *Files identical despite different names*

