# Comparing `tmp/pySSRSapi-0.0.7.tar.gz` & `tmp/pySSRSapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySSRSapi-0.0.7.tar", last modified: Mon Jun  5 11:25:08 2023, max compression
+gzip compressed data, was "pySSRSapi-0.0.8.tar", last modified: Mon Jun  5 15:51:49 2023, max compression
```

## Comparing `pySSRSapi-0.0.7.tar` & `pySSRSapi-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 11:25:08.622521 pySSRSapi-0.0.7/
--rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-05 11:25:08.622248 pySSRSapi-0.0.7/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.7/README.md
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 11:25:08.619617 pySSRSapi-0.0.7/pySSRSapi/
--rw-r--r--   0 quaik8     (501) staff       (20)     9442 2023-06-05 11:24:52.000000 pySSRSapi-0.0.7/pySSRSapi/__init__.py
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 11:25:08.621666 pySSRSapi-0.0.7/pySSRSapi.egg-info/
--rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-05 11:25:08.000000 pySSRSapi-0.0.7/pySSRSapi.egg-info/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-05 11:25:08.000000 pySSRSapi-0.0.7/pySSRSapi.egg-info/SOURCES.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-05 11:25:08.000000 pySSRSapi-0.0.7/pySSRSapi.egg-info/dependency_links.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-05 11:25:08.000000 pySSRSapi-0.0.7/pySSRSapi.egg-info/requires.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-05 11:25:08.000000 pySSRSapi-0.0.7/pySSRSapi.egg-info/top_level.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-05 11:25:08.622597 pySSRSapi-0.0.7/setup.cfg
--rw-r--r--   0 quaik8     (501) staff       (20)      791 2023-06-05 11:25:00.000000 pySSRSapi-0.0.7/setup.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 15:51:49.382212 pySSRSapi-0.0.8/
+-rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-05 15:51:49.381864 pySSRSapi-0.0.8/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.8/README.md
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 15:51:49.378140 pySSRSapi-0.0.8/pySSRSapi/
+-rw-r--r--   0 quaik8     (501) staff       (20)    10102 2023-06-05 15:51:23.000000 pySSRSapi-0.0.8/pySSRSapi/__init__.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 15:51:49.381082 pySSRSapi-0.0.8/pySSRSapi.egg-info/
+-rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-05 15:51:49.000000 pySSRSapi-0.0.8/pySSRSapi.egg-info/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-05 15:51:49.000000 pySSRSapi-0.0.8/pySSRSapi.egg-info/SOURCES.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-05 15:51:49.000000 pySSRSapi-0.0.8/pySSRSapi.egg-info/dependency_links.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-05 15:51:49.000000 pySSRSapi-0.0.8/pySSRSapi.egg-info/requires.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-05 15:51:49.000000 pySSRSapi-0.0.8/pySSRSapi.egg-info/top_level.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-05 15:51:49.382379 pySSRSapi-0.0.8/setup.cfg
+-rw-r--r--   0 quaik8     (501) staff       (20)      791 2023-06-05 15:51:38.000000 pySSRSapi-0.0.8/setup.py
```

### Comparing `pySSRSapi-0.0.7/PKG-INFO` & `pySSRSapi-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pySSRSapi-0.0.7/pySSRSapi/__init__.py` & `pySSRSapi-0.0.8/pySSRSapi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 
 EP_API = '/api/v2.0'
 EP_ME = '/me'
 EP_FOLDERS = '/folders'
 EP_DATASOURCES = '/datasources'
 EP_REPORTS = '/reports'
 
+class BadRequestException(Exception):
+    pass
+
+class NotFoundException(Exception):
+    pass
+
+class AlreadyExistsException(Exception):
+    pass
+
 class User:
     def __init__(self, Id: str, Username: str, DisplayName: str):
         self.Id = Id
         self.Username = Username
         self.DisplayName = DisplayName
         
     def __iter__(self):
@@ -165,14 +174,25 @@
 class Api:
     def __init__(self, url: str, user: str, password: str):
         self.url = url + EP_API
         self.basic_auth = HTTPBasicAuth(user, password)
         self.headers = {'Content-type': 'application/json;charset=UTF-8'}
         
     # REQUESTS
+    def __raiseException(self, statuts_code: int):
+        match statuts_code:
+            case 400:
+                raise BadRequestException('Bad request')
+            case 404:
+                raise NotFoundException('Not found')
+            case 409:
+                raise AlreadyExistsException('Already exists')
+            case _:
+                raise Exception('An error has occurred')
+        
     def __getEndpointClass(self, endpoint: str):
         if endpoint == EP_ME:
             return User
         elif endpoint == EP_FOLDERS:
             return Folder
         elif endpoint == EP_DATASOURCES:
             return Datasource
@@ -183,29 +203,31 @@
         if response.status_code == 200:
             response_obj = json.loads(response.content)
             if 'value' in response_obj:
                 value = json.loads(response.content)['value']
                 return json.loads(json.dumps(value), object_hook=object_hook)
             else:
                 return json.loads(response.content, object_hook=object_hook)
-        return False
+            
+        self.__raiseException(response.status_code)
     
     def __post(self, endpoint: str, data: Folder|Datasource, args: str = ''):
         response = requests.post(self.url + endpoint + args, json=data.to_obj(), auth=self.basic_auth, headers=self.headers)
         object_hook = self.__getEndpointClass(endpoint=endpoint).from_json
         if response.status_code == 201:
             return json.loads(response.content, object_hook=object_hook)
-        return False
+        
+        self.__raiseException(response.status_code)
     
     def __delete(self, endpoint: str, args: str = ''):
         response = requests.delete(self.url + endpoint + args, auth=self.basic_auth, headers=self.headers)
         if response.status_code == 204:
             return True
-        return False
         
+        self.__raiseException(response.status_code)
     
     # USER
     def getUser(self):
         return self.__get(endpoint=EP_ME)
     
     # FOLDER
     def getFolders(self):
@@ -268,13 +290,13 @@
     # def deleteDatasource(self, id: str):
     #     response = requests.delete(self.url + EP_DATASOURCES + '(' + id + ')', auth=self.basic_auth, headers=self.headers)
     #     if response.status_code == 204:
     #         return True
     #     return False
     
     # # REPORT
-    
+
 # def getB64EncodedFile(path):
 #     with open(path, 'rb') as f:
 #         byte_content = f.read()
 #     base64_bytes = base64.b64encode(byte_content)
 #     return base64_bytes.decode('utf-8')
```

### Comparing `pySSRSapi-0.0.7/pySSRSapi.egg-info/PKG-INFO` & `pySSRSapi-0.0.8/pySSRSapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pySSRSapi-0.0.7/setup.py` & `pySSRSapi-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pySSRSapi',
-    version='0.0.7',
+    version='0.0.8',
     description='Python SSRS API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='SSRS, API',
     author='quaik8',
     author_email='mail@example.com',
     url='https://pypi.org/project/pySSRSapi/',
```

