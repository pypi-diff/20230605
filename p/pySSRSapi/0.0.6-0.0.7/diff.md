# Comparing `tmp/pySSRSapi-0.0.6.tar.gz` & `tmp/pySSRSapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySSRSapi-0.0.6.tar", last modified: Sun Jun  4 21:45:30 2023, max compression
+gzip compressed data, was "pySSRSapi-0.0.7.tar", last modified: Mon Jun  5 11:25:08 2023, max compression
```

## Comparing `pySSRSapi-0.0.6.tar` & `pySSRSapi-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-04 21:45:30.504766 pySSRSapi-0.0.6/
--rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-04 21:45:30.504436 pySSRSapi-0.0.6/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.6/README.md
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-04 21:45:30.500290 pySSRSapi-0.0.6/pySSRSapi/
--rw-r--r--   0 quaik8     (501) staff       (20)     9324 2023-06-04 21:44:56.000000 pySSRSapi-0.0.6/pySSRSapi/__init__.py
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-04 21:45:30.503459 pySSRSapi-0.0.6/pySSRSapi.egg-info/
--rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-04 21:45:30.000000 pySSRSapi-0.0.6/pySSRSapi.egg-info/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-04 21:45:30.000000 pySSRSapi-0.0.6/pySSRSapi.egg-info/SOURCES.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-04 21:45:30.000000 pySSRSapi-0.0.6/pySSRSapi.egg-info/dependency_links.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-04 21:45:30.000000 pySSRSapi-0.0.6/pySSRSapi.egg-info/requires.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-04 21:45:30.000000 pySSRSapi-0.0.6/pySSRSapi.egg-info/top_level.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-04 21:45:30.504859 pySSRSapi-0.0.6/setup.cfg
--rw-r--r--   0 quaik8     (501) staff       (20)      791 2023-06-04 21:45:20.000000 pySSRSapi-0.0.6/setup.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 11:25:08.622521 pySSRSapi-0.0.7/
+-rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-05 11:25:08.622248 pySSRSapi-0.0.7/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.7/README.md
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 11:25:08.619617 pySSRSapi-0.0.7/pySSRSapi/
+-rw-r--r--   0 quaik8     (501) staff       (20)     9442 2023-06-05 11:24:52.000000 pySSRSapi-0.0.7/pySSRSapi/__init__.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-05 11:25:08.621666 pySSRSapi-0.0.7/pySSRSapi.egg-info/
+-rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-05 11:25:08.000000 pySSRSapi-0.0.7/pySSRSapi.egg-info/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-05 11:25:08.000000 pySSRSapi-0.0.7/pySSRSapi.egg-info/SOURCES.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-05 11:25:08.000000 pySSRSapi-0.0.7/pySSRSapi.egg-info/dependency_links.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-05 11:25:08.000000 pySSRSapi-0.0.7/pySSRSapi.egg-info/requires.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-05 11:25:08.000000 pySSRSapi-0.0.7/pySSRSapi.egg-info/top_level.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-05 11:25:08.622597 pySSRSapi-0.0.7/setup.cfg
+-rw-r--r--   0 quaik8     (501) staff       (20)      791 2023-06-05 11:25:00.000000 pySSRSapi-0.0.7/setup.py
```

### Comparing `pySSRSapi-0.0.6/PKG-INFO` & `pySSRSapi-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pySSRSapi-0.0.6/pySSRSapi/__init__.py` & `pySSRSapi-0.0.7/pySSRSapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,21 @@
     def __post(self, endpoint: str, data: Folder|Datasource, args: str = ''):
         response = requests.post(self.url + endpoint + args, json=data.to_obj(), auth=self.basic_auth, headers=self.headers)
         object_hook = self.__getEndpointClass(endpoint=endpoint).from_json
         if response.status_code == 201:
             return json.loads(response.content, object_hook=object_hook)
         return False
     
+    def __delete(self, endpoint: str, args: str = ''):
+        response = requests.delete(self.url + endpoint + args, auth=self.basic_auth, headers=self.headers)
+        if response.status_code == 204:
+            return True
+        return False
+        
+    
     # USER
     def getUser(self):
         return self.__get(endpoint=EP_ME)
     
     # FOLDER
     def getFolders(self):
         return self.__get(endpoint=EP_FOLDERS)
@@ -225,19 +232,16 @@
     
     # def editFolder(self, id: str, folder: Folder):
     #     response = requests.patch(self.url + EP_FOLDERS + '(' + id + ')', json=folder, auth=self.basic_auth, headers=self.headers)
     #     if response.status_code == 204:
     #         return self.getFolderById(id = id)
     #     return False
 
-    # def deleteFolder(self, id: str):
-    #     response = requests.delete(self.url + EP_FOLDERS + '(' + id + ')', auth=self.basic_auth, headers=self.headers)
-    #     if response.status_code == 204:
-    #         return True
-    #     return False
+    def deleteFolder(self, id: str):
+        return self.__delete(endpoint=EP_FOLDERS, args='(' + id + ')')
     
     # # DATASOURCE
     # def getDatasources(self):
     #     response = requests.get(self.url + EP_DATASOURCES, auth=self.basic_auth, headers=self.headers)
     #     if response.status_code == 200:
     #         value = json.loads(response.content)['value']
     #         return json.loads(json.dumps(value), object_hook=Datasource.from_json)
```

### Comparing `pySSRSapi-0.0.6/pySSRSapi.egg-info/PKG-INFO` & `pySSRSapi-0.0.7/pySSRSapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pySSRSapi-0.0.6/setup.py` & `pySSRSapi-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pySSRSapi',
-    version='0.0.6',
+    version='0.0.7',
     description='Python SSRS API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='SSRS, API',
     author='quaik8',
     author_email='mail@example.com',
     url='https://pypi.org/project/pySSRSapi/',
```

