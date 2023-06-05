# Comparing `tmp/daspython-2.1.0.tar.gz` & `tmp/daspython-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daspython-2.1.0.tar", last modified: Tue May 16 09:00:53 2023, max compression
+gzip compressed data, was "daspython-3.0.0.tar", last modified: Mon Jun  5 14:04:14 2023, max compression
```

## Comparing `daspython-2.1.0.tar` & `daspython-3.0.0.tar`

### file list

```diff
@@ -1,58 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.595900 daspython-2.1.0/
--rw-rw-rw-   0        0        0    35821 2023-03-29 09:37:21.000000 daspython-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     2257 2023-05-16 09:00:53.593873 daspython-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1731 2023-05-15 11:45:51.000000 daspython-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.061349 daspython-2.1.0/daspython/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.155807 daspython-2.1.0/daspython/auth/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/auth/__init__.py
--rw-rw-rw-   0        0        0     1971 2023-05-15 10:28:47.000000 daspython-2.1.0/daspython/auth/authenticate.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.181819 daspython-2.1.0/daspython/client/
--rw-rw-rw-   0        0        0        0 2023-04-06 09:25:32.000000 daspython-2.1.0/daspython/client/__init__.py
--rw-rw-rw-   0        0        0     1001 2023-04-06 09:00:06.000000 daspython-2.1.0/daspython/client/client.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.238739 daspython-2.1.0/daspython/common/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/common/__init__.py
--rw-rw-rw-   0        0        0     6911 2023-05-16 08:32:28.000000 daspython-2.1.0/daspython/common/api.py
--rw-rw-rw-   0        0        0      110 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/common/response.py
--rw-rw-rw-   0        0        0     1936 2023-05-15 15:42:46.000000 daspython-2.1.0/daspython/das.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.258208 daspython-2.1.0/daspython/dastypes/
--rw-rw-rw-   0        0        0        0 2023-04-06 09:20:32.000000 daspython-2.1.0/daspython/dastypes/__init__.py
--rw-rw-rw-   0        0        0       30 2023-04-06 08:46:36.000000 daspython-2.1.0/daspython/dastypes/entry.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.285173 daspython-2.1.0/daspython/services/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.302270 daspython-2.1.0/daspython/services/alcs/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/services/alcs/__init__.py
--rw-rw-rw-   0        0        0      500 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/services/alcs/aclservice.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.317172 daspython-2.1.0/daspython/services/attributes/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/services/attributes/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-05-15 14:06:23.000000 daspython-2.1.0/daspython/services/attributes/attributeservice.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.351971 daspython-2.1.0/daspython/services/digitalobjects/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/services/digitalobjects/__init__.py
--rw-rw-rw-   0        0        0    11310 2023-05-12 15:33:43.000000 daspython-2.1.0/daspython/services/digitalobjects/digitalobjectservice.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.390968 daspython-2.1.0/daspython/services/entries/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/services/entries/__init__.py
--rw-rw-rw-   0        0        0    20424 2023-05-16 08:58:27.000000 daspython-2.1.0/daspython/services/entries/entryservice.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.407952 daspython-2.1.0/daspython/services/entryfields/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/services/entryfields/__init__.py
--rw-rw-rw-   0        0        0      722 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/services/entryfields/entryfieldservice.py
--rw-rw-rw-   0        0        0     1245 2023-05-16 08:33:07.000000 daspython-2.1.0/daspython/services/graphql_server.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.433502 daspython-2.1.0/daspython/services/searches/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/services/searches/__init__.py
--rw-rw-rw-   0        0        0     1960 2023-03-29 09:37:21.000000 daspython-2.1.0/daspython/services/searches/searchservice.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.131256 daspython-2.1.0/daspython.egg-info/
--rw-rw-rw-   0        0        0     2257 2023-05-16 09:00:52.000000 daspython-2.1.0/daspython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1320 2023-05-16 09:00:52.000000 daspython-2.1.0/daspython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 09:00:52.000000 daspython-2.1.0/daspython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-05-16 09:00:52.000000 daspython-2.1.0/daspython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 09:00:52.000000 daspython-2.1.0/daspython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      843 2023-05-16 09:00:03.000000 daspython-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 09:00:53.596897 daspython-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 09:00:53.589815 daspython-2.1.0/tests/
--rw-rw-rw-   0        0        0     1033 2023-05-11 16:51:54.000000 daspython-2.1.0/tests/test_aclservice.py
--rw-rw-rw-   0        0        0     1187 2023-05-11 16:47:49.000000 daspython-2.1.0/tests/test_attributeservice.py
--rw-rw-rw-   0        0        0      526 2023-05-11 16:47:21.000000 daspython-2.1.0/tests/test_authenticate.py
--rw-rw-rw-   0        0        0      700 2023-04-06 09:25:24.000000 daspython-2.1.0/tests/test_dasclient.py
--rw-rw-rw-   0        0        0     1849 2023-05-15 15:25:42.000000 daspython-2.1.0/tests/test_daspython.py
--rw-rw-rw-   0        0        0     2489 2023-05-12 15:34:51.000000 daspython-2.1.0/tests/test_digital_object_service.py
--rw-rw-rw-   0        0        0      861 2023-05-11 16:47:43.000000 daspython-2.1.0/tests/test_entry_field_service.py
--rw-rw-rw-   0        0        0     7078 2023-05-11 16:47:47.000000 daspython-2.1.0/tests/test_entry_service.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.199076 daspython-3.0.0/
+-rw-rw-rw-   0        0        0    35821 2023-03-29 09:37:21.000000 daspython-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2257 2023-06-05 14:04:14.197785 daspython-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1731 2023-05-15 11:45:51.000000 daspython-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:13.874057 daspython-3.0.0/daspython/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:13.962944 daspython-3.0.0/daspython/auth/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/auth/__init__.py
+-rw-rw-rw-   0        0        0     1971 2023-05-15 10:28:47.000000 daspython-3.0.0/daspython/auth/authenticate.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:13.967451 daspython-3.0.0/daspython/client/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:25:32.000000 daspython-3.0.0/daspython/client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.005305 daspython-3.0.0/daspython/common/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/common/__init__.py
+-rw-rw-rw-   0        0        0     6911 2023-05-16 08:32:28.000000 daspython-3.0.0/daspython/common/api.py
+-rw-rw-rw-   0        0        0      110 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/common/response.py
+-rw-rw-rw-   0        0        0    10284 2023-06-05 13:53:53.000000 daspython-3.0.0/daspython/das.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.023876 daspython-3.0.0/daspython/dastypes/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:20:32.000000 daspython-3.0.0/daspython/dastypes/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-04-06 08:46:36.000000 daspython-3.0.0/daspython/dastypes/entry.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.038547 daspython-3.0.0/daspython/services/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.059882 daspython-3.0.0/daspython/services/alcs/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/alcs/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-05-30 09:33:11.000000 daspython-3.0.0/daspython/services/alcs/aclservice.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.084491 daspython-3.0.0/daspython/services/attributes/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/attributes/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-05-15 14:06:23.000000 daspython-3.0.0/daspython/services/attributes/attributeservice.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.115379 daspython-3.0.0/daspython/services/digitalobjects/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/digitalobjects/__init__.py
+-rw-rw-rw-   0        0        0    11308 2023-06-05 08:49:28.000000 daspython-3.0.0/daspython/services/digitalobjects/digitalobjectservice.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.141605 daspython-3.0.0/daspython/services/entries/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/entries/__init__.py
+-rw-rw-rw-   0        0        0    20419 2023-05-30 13:06:15.000000 daspython-3.0.0/daspython/services/entries/entryservice.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.157854 daspython-3.0.0/daspython/services/entryfields/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/entryfields/__init__.py
+-rw-rw-rw-   0        0        0      722 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/entryfields/entryfieldservice.py
+-rw-rw-rw-   0        0        0     1245 2023-05-16 08:33:07.000000 daspython-3.0.0/daspython/services/graphql_server.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.177876 daspython-3.0.0/daspython/services/searches/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/searches/__init__.py
+-rw-rw-rw-   0        0        0     1978 2023-05-30 09:25:46.000000 daspython-3.0.0/daspython/services/searches/searchservice.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:13.936208 daspython-3.0.0/daspython.egg-info/
+-rw-rw-rw-   0        0        0     2257 2023-06-05 14:04:13.000000 daspython-3.0.0/daspython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1263 2023-06-05 14:04:13.000000 daspython-3.0.0/daspython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 14:04:13.000000 daspython-3.0.0/daspython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-06-05 14:04:13.000000 daspython-3.0.0/daspython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 14:04:13.000000 daspython-3.0.0/daspython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      843 2023-06-05 13:54:47.000000 daspython-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 14:04:14.200122 daspython-3.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.195803 daspython-3.0.0/tests/
+-rw-rw-rw-   0        0        0     1018 2023-05-30 09:33:36.000000 daspython-3.0.0/tests/test_aclservice.py
+-rw-rw-rw-   0        0        0     1187 2023-05-11 16:47:49.000000 daspython-3.0.0/tests/test_attributeservice.py
+-rw-rw-rw-   0        0        0      526 2023-05-11 16:47:21.000000 daspython-3.0.0/tests/test_authenticate.py
+-rw-rw-rw-   0        0        0     4936 2023-06-05 11:59:02.000000 daspython-3.0.0/tests/test_das.py
+-rw-rw-rw-   0        0        0     3302 2023-06-05 09:24:46.000000 daspython-3.0.0/tests/test_digital_object_service.py
+-rw-rw-rw-   0        0        0      867 2023-05-30 13:56:08.000000 daspython-3.0.0/tests/test_entry_field_service.py
+-rw-rw-rw-   0        0        0     7078 2023-05-30 09:25:46.000000 daspython-3.0.0/tests/test_entry_service.py
```

### Comparing `daspython-2.1.0/LICENSE` & `daspython-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `daspython-2.1.0/PKG-INFO` & `daspython-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daspython
-Version: 2.1.0
+Version: 3.0.0
 Summary: DAS api client.
 Author: Royal Netherlands Institute for Sea Research
 Project-URL: Homepage, https://git.nioz.nl/ict-projects/das-python
 Project-URL: Bug Tracker, https://git.nioz.nl/ict-projects/das-python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `daspython-2.1.0/README.md` & `daspython-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `daspython-2.1.0/daspython/auth/authenticate.py` & `daspython-3.0.0/daspython/auth/authenticate.py`

 * *Files identical despite different names*

### Comparing `daspython-2.1.0/daspython/common/api.py` & `daspython-3.0.0/daspython/common/api.py`

 * *Files identical despite different names*

### Comparing `daspython-2.1.0/daspython/services/attributes/attributeservice.py` & `daspython-3.0.0/daspython/services/attributes/attributeservice.py`

 * *Files identical despite different names*

### Comparing `daspython-2.1.0/daspython/services/digitalobjects/digitalobjectservice.py` & `daspython-3.0.0/daspython/services/digitalobjects/digitalobjectservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         if response_digital_object is None or response_digital_object.entry is None:
             raise Exception(
                 f'Digital Object not found with the code: {digital_object_code}')
 
         self.__set_digital_object_relation(
             entry_code=entry_code, digital_obj_id=response_digital_object.entry['id'])
 
-    def download_request(self, entry_code: str, digital_object_code_list: list[str] = None):
+    def download_request(self, entry_code: str, digital_object_code_list: list[str] = []):
 
         entry_service = EntryService(self.token)
 
         response = entry_service.get_entry_by_code(entry_code)
         entry = response.entry
 
         if (entry is None):
```

### Comparing `daspython-2.1.0/daspython/services/entries/entryservice.py` & `daspython-3.0.0/daspython/services/entries/entryservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
         -------
             True if the entry was deleted successfully.
         '''
         api_url = f'/api/services/app/Entry/Delete?Id={id}&AttributeId={attributeId}'
         response = self.delete_data(url=api_url)
         return response['result']
 
-    def get_entry_id(self, name: str, attribute_name: str = None, attribute_id: int = None) -> str:
+    def get_entry_id(self, name: str, attribute_name: str = '', attribute_id: int = 0) -> str:
         '''
         Gets the entry identifier based on its name and attribute.
 
         Parameters
         ----------
             name:str
                 Entry's name.
```

### Comparing `daspython-2.1.0/daspython/services/entryfields/entryfieldservice.py` & `daspython-3.0.0/daspython/services/entryfields/entryfieldservice.py`

 * *Files identical despite different names*

### Comparing `daspython-2.1.0/daspython/services/graphql_server.py` & `daspython-3.0.0/daspython/services/graphql_server.py`

 * *Files identical despite different names*

### Comparing `daspython-2.1.0/daspython/services/searches/searchservice.py` & `daspython-3.0.0/daspython/services/searches/searchservice.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,20 @@
         querystring: str (default None)                    
             Your search filter. 
                 Example: 'id(56);displayname(64*)' --> Find the item with a identifier equals 56 and the displayname starts with 64.
         sorting: str (default None)                    
             Sorting expression.
                 Example: 'displayname asc' --> Sort the result by displayname in ascending order.
     '''
-    attributeId: int = None
+    attributeId: int = 0
     maxresultcount: int = 10
     skipcount: int = 0
-    querystring: str = None
-    sorting: str = None
+    querystring: str = ""
+    sorting: str = ""
+    tableName: str = ""
 
 
 class SearchService(ApiMethods):
     '''
     The search engine class that should be used to fetch only entries.
     '''
```

### Comparing `daspython-2.1.0/daspython.egg-info/PKG-INFO` & `daspython-3.0.0/daspython.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daspython
-Version: 2.1.0
+Version: 3.0.0
 Summary: DAS api client.
 Author: Royal Netherlands Institute for Sea Research
 Project-URL: Homepage, https://git.nioz.nl/ict-projects/das-python
 Project-URL: Bug Tracker, https://git.nioz.nl/ict-projects/das-python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `daspython-2.1.0/daspython.egg-info/SOURCES.txt` & `daspython-3.0.0/daspython.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 daspython.egg-info/SOURCES.txt
 daspython.egg-info/dependency_links.txt
 daspython.egg-info/requires.txt
 daspython.egg-info/top_level.txt
 daspython/auth/__init__.py
 daspython/auth/authenticate.py
 daspython/client/__init__.py
-daspython/client/client.py
 daspython/common/__init__.py
 daspython/common/api.py
 daspython/common/response.py
 daspython/dastypes/__init__.py
 daspython/dastypes/entry.py
 daspython/services/__init__.py
 daspython/services/graphql_server.py
@@ -30,12 +29,11 @@
 daspython/services/entryfields/__init__.py
 daspython/services/entryfields/entryfieldservice.py
 daspython/services/searches/__init__.py
 daspython/services/searches/searchservice.py
 tests/test_aclservice.py
 tests/test_attributeservice.py
 tests/test_authenticate.py
-tests/test_dasclient.py
-tests/test_daspython.py
+tests/test_das.py
 tests/test_digital_object_service.py
 tests/test_entry_field_service.py
 tests/test_entry_service.py
```

### Comparing `daspython-2.1.0/pyproject.toml` & `daspython-3.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "daspython"
-version = "2.1.0"
+version = "3.0.0"
 authors = [
   { name="Royal Netherlands Institute for Sea Research" },
 ]
 description = "DAS api client."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `daspython-2.1.0/tests/test_aclservice.py` & `daspython-3.0.0/tests/test_aclservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
     def _get_token(self) -> Token:
         load_dotenv()
         auth = DasAuth(os.getenv("DAS_URL"), os.getenv("DAS_USERNAME"), os.getenv("DAS_PASSWORD"))
         auth.authenticate(bool(os.getenv("CHECK_HTTPS")))
         return auth
 
-    def test_change_ownership(self):
+    def test_change_owner(self):
 
         acl_service = AclService(self._get_token())
 
         payload = ChangeOwnershipRequest()
         payload.attributeId = 55
         payload.entryId = 'f3cfd83d-b95d-4876-9217-312eec681e37'
         payload.newOwnerId = 57
         
-        response = acl_service.ChangeOwnership(request=payload)
+        response = acl_service.change_owner(payload)
 
         self.assertEqual(response, True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `daspython-2.1.0/tests/test_attributeservice.py` & `daspython-3.0.0/tests/test_attributeservice.py`

 * *Files identical despite different names*

### Comparing `daspython-2.1.0/tests/test_authenticate.py` & `daspython-3.0.0/tests/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `daspython-2.1.0/tests/test_entry_field_service.py` & `daspython-3.0.0/tests/test_entry_field_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dotenv import load_dotenv
 from daspython.common.api import Token
 from daspython.auth.authenticate import DasAuth
 from daspython.services.entryfields.entryfieldservice import EntryFieldService, DisplayType
 
 
 class TestEntryService(unittest.TestCase):
+    
     def _get_token(self) -> Token:
         load_dotenv()
         auth = DasAuth(os.getenv("DAS_URL"), os.getenv("DAS_USERNAME"), os.getenv("DAS_PASSWORD"))
         auth.authenticate(bool(os.getenv("CHECK_HTTPS")))
         return auth
 
     def test_getall(self):
```

### Comparing `daspython-2.1.0/tests/test_entry_service.py` & `daspython-3.0.0/tests/test_entry_service.py`

 * *Files identical despite different names*

