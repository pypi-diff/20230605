# Comparing `tmp/daspython-3.0.0.tar.gz` & `tmp/daspython-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daspython-3.0.0.tar", last modified: Mon Jun  5 14:04:14 2023, max compression
+gzip compressed data, was "daspython-3.0.1.tar", last modified: Mon Jun  5 14:45:16 2023, max compression
```

## Comparing `daspython-3.0.0.tar` & `daspython-3.0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.199076 daspython-3.0.0/
--rw-rw-rw-   0        0        0    35821 2023-03-29 09:37:21.000000 daspython-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     2257 2023-06-05 14:04:14.197785 daspython-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1731 2023-05-15 11:45:51.000000 daspython-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:13.874057 daspython-3.0.0/daspython/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:13.962944 daspython-3.0.0/daspython/auth/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/auth/__init__.py
--rw-rw-rw-   0        0        0     1971 2023-05-15 10:28:47.000000 daspython-3.0.0/daspython/auth/authenticate.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:13.967451 daspython-3.0.0/daspython/client/
--rw-rw-rw-   0        0        0        0 2023-04-06 09:25:32.000000 daspython-3.0.0/daspython/client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.005305 daspython-3.0.0/daspython/common/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/common/__init__.py
--rw-rw-rw-   0        0        0     6911 2023-05-16 08:32:28.000000 daspython-3.0.0/daspython/common/api.py
--rw-rw-rw-   0        0        0      110 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/common/response.py
--rw-rw-rw-   0        0        0    10284 2023-06-05 13:53:53.000000 daspython-3.0.0/daspython/das.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.023876 daspython-3.0.0/daspython/dastypes/
--rw-rw-rw-   0        0        0        0 2023-04-06 09:20:32.000000 daspython-3.0.0/daspython/dastypes/__init__.py
--rw-rw-rw-   0        0        0       30 2023-04-06 08:46:36.000000 daspython-3.0.0/daspython/dastypes/entry.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.038547 daspython-3.0.0/daspython/services/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.059882 daspython-3.0.0/daspython/services/alcs/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/alcs/__init__.py
--rw-rw-rw-   0        0        0      944 2023-05-30 09:33:11.000000 daspython-3.0.0/daspython/services/alcs/aclservice.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.084491 daspython-3.0.0/daspython/services/attributes/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/attributes/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-05-15 14:06:23.000000 daspython-3.0.0/daspython/services/attributes/attributeservice.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.115379 daspython-3.0.0/daspython/services/digitalobjects/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/digitalobjects/__init__.py
--rw-rw-rw-   0        0        0    11308 2023-06-05 08:49:28.000000 daspython-3.0.0/daspython/services/digitalobjects/digitalobjectservice.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.141605 daspython-3.0.0/daspython/services/entries/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/entries/__init__.py
--rw-rw-rw-   0        0        0    20419 2023-05-30 13:06:15.000000 daspython-3.0.0/daspython/services/entries/entryservice.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.157854 daspython-3.0.0/daspython/services/entryfields/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/entryfields/__init__.py
--rw-rw-rw-   0        0        0      722 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/entryfields/entryfieldservice.py
--rw-rw-rw-   0        0        0     1245 2023-05-16 08:33:07.000000 daspython-3.0.0/daspython/services/graphql_server.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.177876 daspython-3.0.0/daspython/services/searches/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.0/daspython/services/searches/__init__.py
--rw-rw-rw-   0        0        0     1978 2023-05-30 09:25:46.000000 daspython-3.0.0/daspython/services/searches/searchservice.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:13.936208 daspython-3.0.0/daspython.egg-info/
--rw-rw-rw-   0        0        0     2257 2023-06-05 14:04:13.000000 daspython-3.0.0/daspython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1263 2023-06-05 14:04:13.000000 daspython-3.0.0/daspython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 14:04:13.000000 daspython-3.0.0/daspython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-06-05 14:04:13.000000 daspython-3.0.0/daspython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-05 14:04:13.000000 daspython-3.0.0/daspython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      843 2023-06-05 13:54:47.000000 daspython-3.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-05 14:04:14.200122 daspython-3.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-05 14:04:14.195803 daspython-3.0.0/tests/
--rw-rw-rw-   0        0        0     1018 2023-05-30 09:33:36.000000 daspython-3.0.0/tests/test_aclservice.py
--rw-rw-rw-   0        0        0     1187 2023-05-11 16:47:49.000000 daspython-3.0.0/tests/test_attributeservice.py
--rw-rw-rw-   0        0        0      526 2023-05-11 16:47:21.000000 daspython-3.0.0/tests/test_authenticate.py
--rw-rw-rw-   0        0        0     4936 2023-06-05 11:59:02.000000 daspython-3.0.0/tests/test_das.py
--rw-rw-rw-   0        0        0     3302 2023-06-05 09:24:46.000000 daspython-3.0.0/tests/test_digital_object_service.py
--rw-rw-rw-   0        0        0      867 2023-05-30 13:56:08.000000 daspython-3.0.0/tests/test_entry_field_service.py
--rw-rw-rw-   0        0        0     7078 2023-05-30 09:25:46.000000 daspython-3.0.0/tests/test_entry_service.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.452886 daspython-3.0.1/
+-rw-rw-rw-   0        0        0    35821 2023-03-29 09:37:21.000000 daspython-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2257 2023-06-05 14:45:16.451887 daspython-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1731 2023-05-15 11:45:51.000000 daspython-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.344953 daspython-3.0.1/daspython/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.390960 daspython-3.0.1/daspython/auth/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/auth/__init__.py
+-rw-rw-rw-   0        0        0     1971 2023-05-15 10:28:47.000000 daspython-3.0.1/daspython/auth/authenticate.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.393963 daspython-3.0.1/daspython/client/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:25:32.000000 daspython-3.0.1/daspython/client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.402983 daspython-3.0.1/daspython/common/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/common/__init__.py
+-rw-rw-rw-   0        0        0     6911 2023-05-16 08:32:28.000000 daspython-3.0.1/daspython/common/api.py
+-rw-rw-rw-   0        0        0      110 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/common/response.py
+-rw-rw-rw-   0        0        0    10430 2023-06-05 14:40:57.000000 daspython-3.0.1/daspython/das.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.409059 daspython-3.0.1/daspython/dastypes/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:20:32.000000 daspython-3.0.1/daspython/dastypes/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-04-06 08:46:36.000000 daspython-3.0.1/daspython/dastypes/entry.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.414121 daspython-3.0.1/daspython/services/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.418455 daspython-3.0.1/daspython/services/alcs/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/services/alcs/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-05-30 09:33:11.000000 daspython-3.0.1/daspython/services/alcs/aclservice.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.421457 daspython-3.0.1/daspython/services/attributes/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/services/attributes/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-05-15 14:06:23.000000 daspython-3.0.1/daspython/services/attributes/attributeservice.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.424489 daspython-3.0.1/daspython/services/digitalobjects/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/services/digitalobjects/__init__.py
+-rw-rw-rw-   0        0        0    11308 2023-06-05 08:49:28.000000 daspython-3.0.1/daspython/services/digitalobjects/digitalobjectservice.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.427457 daspython-3.0.1/daspython/services/entries/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/services/entries/__init__.py
+-rw-rw-rw-   0        0        0    20419 2023-05-30 13:06:15.000000 daspython-3.0.1/daspython/services/entries/entryservice.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.431803 daspython-3.0.1/daspython/services/entryfields/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/services/entryfields/__init__.py
+-rw-rw-rw-   0        0        0      722 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/services/entryfields/entryfieldservice.py
+-rw-rw-rw-   0        0        0     1245 2023-05-16 08:33:07.000000 daspython-3.0.1/daspython/services/graphql_server.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.434800 daspython-3.0.1/daspython/services/searches/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-3.0.1/daspython/services/searches/__init__.py
+-rw-rw-rw-   0        0        0     1978 2023-05-30 09:25:46.000000 daspython-3.0.1/daspython/services/searches/searchservice.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.384965 daspython-3.0.1/daspython.egg-info/
+-rw-rw-rw-   0        0        0     2257 2023-06-05 14:45:16.000000 daspython-3.0.1/daspython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1263 2023-06-05 14:45:16.000000 daspython-3.0.1/daspython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 14:45:16.000000 daspython-3.0.1/daspython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-06-05 14:45:16.000000 daspython-3.0.1/daspython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 14:45:16.000000 daspython-3.0.1/daspython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      843 2023-06-05 14:44:59.000000 daspython-3.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 14:45:16.453884 daspython-3.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 14:45:16.449886 daspython-3.0.1/tests/
+-rw-rw-rw-   0        0        0     1018 2023-05-30 09:33:36.000000 daspython-3.0.1/tests/test_aclservice.py
+-rw-rw-rw-   0        0        0     1187 2023-05-11 16:47:49.000000 daspython-3.0.1/tests/test_attributeservice.py
+-rw-rw-rw-   0        0        0      526 2023-05-11 16:47:21.000000 daspython-3.0.1/tests/test_authenticate.py
+-rw-rw-rw-   0        0        0     4936 2023-06-05 11:59:02.000000 daspython-3.0.1/tests/test_das.py
+-rw-rw-rw-   0        0        0     3302 2023-06-05 09:24:46.000000 daspython-3.0.1/tests/test_digital_object_service.py
+-rw-rw-rw-   0        0        0      867 2023-05-30 13:56:08.000000 daspython-3.0.1/tests/test_entry_field_service.py
+-rw-rw-rw-   0        0        0     7078 2023-05-30 09:25:46.000000 daspython-3.0.1/tests/test_entry_service.py
```

### Comparing `daspython-3.0.0/LICENSE` & `daspython-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/PKG-INFO` & `daspython-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daspython
-Version: 3.0.0
+Version: 3.0.1
 Summary: DAS api client.
 Author: Royal Netherlands Institute for Sea Research
 Project-URL: Homepage, https://git.nioz.nl/ict-projects/das-python
 Project-URL: Bug Tracker, https://git.nioz.nl/ict-projects/das-python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `daspython-3.0.0/README.md` & `daspython-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/daspython/auth/authenticate.py` & `daspython-3.0.1/daspython/auth/authenticate.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/daspython/common/api.py` & `daspython-3.0.1/daspython/common/api.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/daspython/das.py` & `daspython-3.0.1/daspython/das.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,23 @@
 from daspython.common.api import Token
 from daspython.services.entryfields.entryfieldservice import DisplayType, EntryFieldService
 from daspython.services.searches.searchservice import SearchEntriesRequest, SearchService
 
 class DasClient():
 
     __token: Token
+    __is_authenticated: bool
+
+    @property
+    def is_authenticated(self):
+        return self.__is_authenticated
 
     def __init__(self, username:str, password:str, base_url:str, check_https:bool=True):
         auth = DasAuth(base_url, username, password)
-        auth.authenticate(check_https)
+        self.__is_authenticated = auth.authenticate(check_https)
         self.__token = auth
 
 
     def get_attribute_name(self, attribute_id:int):
         """
         Gets the name of an attribute by its id
```

### Comparing `daspython-3.0.0/daspython/services/alcs/aclservice.py` & `daspython-3.0.1/daspython/services/alcs/aclservice.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/daspython/services/attributes/attributeservice.py` & `daspython-3.0.1/daspython/services/attributes/attributeservice.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/daspython/services/digitalobjects/digitalobjectservice.py` & `daspython-3.0.1/daspython/services/digitalobjects/digitalobjectservice.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/daspython/services/entries/entryservice.py` & `daspython-3.0.1/daspython/services/entries/entryservice.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/daspython/services/entryfields/entryfieldservice.py` & `daspython-3.0.1/daspython/services/entryfields/entryfieldservice.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/daspython/services/graphql_server.py` & `daspython-3.0.1/daspython/services/graphql_server.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/daspython/services/searches/searchservice.py` & `daspython-3.0.1/daspython/services/searches/searchservice.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/daspython.egg-info/PKG-INFO` & `daspython-3.0.1/daspython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daspython
-Version: 3.0.0
+Version: 3.0.1
 Summary: DAS api client.
 Author: Royal Netherlands Institute for Sea Research
 Project-URL: Homepage, https://git.nioz.nl/ict-projects/das-python
 Project-URL: Bug Tracker, https://git.nioz.nl/ict-projects/das-python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `daspython-3.0.0/daspython.egg-info/SOURCES.txt` & `daspython-3.0.1/daspython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/pyproject.toml` & `daspython-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "daspython"
-version = "3.0.0"
+version = "3.0.1"
 authors = [
   { name="Royal Netherlands Institute for Sea Research" },
 ]
 description = "DAS api client."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `daspython-3.0.0/tests/test_aclservice.py` & `daspython-3.0.1/tests/test_aclservice.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/tests/test_attributeservice.py` & `daspython-3.0.1/tests/test_attributeservice.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/tests/test_authenticate.py` & `daspython-3.0.1/tests/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/tests/test_das.py` & `daspython-3.0.1/tests/test_das.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/tests/test_digital_object_service.py` & `daspython-3.0.1/tests/test_digital_object_service.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/tests/test_entry_field_service.py` & `daspython-3.0.1/tests/test_entry_field_service.py`

 * *Files identical despite different names*

### Comparing `daspython-3.0.0/tests/test_entry_service.py` & `daspython-3.0.1/tests/test_entry_service.py`

 * *Files identical despite different names*

