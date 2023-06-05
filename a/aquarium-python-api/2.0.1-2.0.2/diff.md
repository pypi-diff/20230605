# Comparing `tmp/aquarium-python-api-2.0.1.tar.gz` & `tmp/aquarium-python-api-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquarium-python-api-2.0.1.tar", last modified: Sun Jun  4 09:16:07 2023, max compression
+gzip compressed data, was "dist/aquarium-python-api-2.0.2.tar", last modified: Mon Jun  5 09:41:05 2023, max compression
```

## Comparing `aquarium-python-api-2.0.1.tar` & `aquarium-python-api-2.0.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-04 09:16:07.279075 aquarium-python-api-2.0.1/
--rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.1/LICENSE.md
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-04 09:16:07.279320 aquarium-python-api-2.0.1/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.1/README.md
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-04 09:16:07.257981 aquarium-python-api-2.0.1/aquarium/
--rw-r--r--   0 yann       (501) staff       (20)      917 2021-02-01 10:01:21.000000 aquarium-python-api-2.0.1/aquarium/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)    12537 2023-04-15 09:11:35.000000 aquarium-python-api-2.0.1/aquarium/aquarium.py
--rw-r--r--   0 yann       (501) staff       (20)     3399 2022-11-09 16:10:59.000000 aquarium-python-api-2.0.1/aquarium/edge.py
--rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.1/aquarium/element.py
--rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.1/aquarium/entity.py
--rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.1/aquarium/exceptions.py
--rw-r--r--   0 yann       (501) staff       (20)    26695 2023-06-04 09:10:20.000000 aquarium-python-api-2.0.1/aquarium/item.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-04 09:16:07.273574 aquarium-python-api-2.0.1/aquarium/items/
--rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.1/aquarium/items/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.1/aquarium/items/asset.py
--rw-r--r--   0 yann       (501) staff       (20)     5092 2023-04-15 09:03:56.000000 aquarium-python-api-2.0.1/aquarium/items/organisation.py
--rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.1/aquarium/items/playlist.py
--rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.1/aquarium/items/project.py
--rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.1/aquarium/items/shot.py
--rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.1/aquarium/items/task.py
--rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.1/aquarium/items/template.py
--rw-r--r--   0 yann       (501) staff       (20)     4087 2022-11-05 08:59:00.000000 aquarium-python-api-2.0.1/aquarium/items/user.py
--rw-r--r--   0 yann       (501) staff       (20)     1653 2021-02-19 09:03:04.000000 aquarium-python-api-2.0.1/aquarium/items/usergroup.py
--rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.1/aquarium/tools.py
--rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.1/aquarium/utils.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-04 09:16:07.278419 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-04 09:16:06.000000 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)      686 2023-06-04 09:16:06.000000 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yann       (501) staff       (20)        1 2023-06-04 09:16:06.000000 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yann       (501) staff       (20)      123 2023-06-04 09:16:06.000000 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/requires.txt
--rw-r--r--   0 yann       (501) staff       (20)        9 2023-06-04 09:16:06.000000 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/top_level.txt
--rw-r--r--   0 yann       (501) staff       (20)     1280 2023-06-04 09:16:07.280346 aquarium-python-api-2.0.1/setup.cfg
--rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.1/setup.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 09:41:05.175207 aquarium-python-api-2.0.2/
+-rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.2/LICENSE.md
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-05 09:41:05.175576 aquarium-python-api-2.0.2/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.2/README.md
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 09:41:05.145030 aquarium-python-api-2.0.2/aquarium/
+-rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.0.2/aquarium/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)    12529 2023-06-05 09:35:55.000000 aquarium-python-api-2.0.2/aquarium/aquarium.py
+-rw-r--r--   0 yann       (501) staff       (20)      364 2023-06-05 08:31:35.000000 aquarium-python-api-2.0.2/aquarium/auth.py
+-rw-r--r--   0 yann       (501) staff       (20)     3399 2022-11-09 16:10:59.000000 aquarium-python-api-2.0.2/aquarium/edge.py
+-rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.2/aquarium/element.py
+-rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.2/aquarium/entity.py
+-rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.2/aquarium/exceptions.py
+-rw-r--r--   0 yann       (501) staff       (20)    27572 2023-06-05 09:32:37.000000 aquarium-python-api-2.0.2/aquarium/item.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 09:41:05.168399 aquarium-python-api-2.0.2/aquarium/items/
+-rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.2/aquarium/items/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.2/aquarium/items/asset.py
+-rw-r--r--   0 yann       (501) staff       (20)     5092 2023-04-15 09:03:56.000000 aquarium-python-api-2.0.2/aquarium/items/organisation.py
+-rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.2/aquarium/items/playlist.py
+-rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.2/aquarium/items/project.py
+-rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.2/aquarium/items/shot.py
+-rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.2/aquarium/items/task.py
+-rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.2/aquarium/items/template.py
+-rw-r--r--   0 yann       (501) staff       (20)     4029 2023-06-05 09:29:59.000000 aquarium-python-api-2.0.2/aquarium/items/user.py
+-rw-r--r--   0 yann       (501) staff       (20)     1595 2023-06-05 09:30:04.000000 aquarium-python-api-2.0.2/aquarium/items/usergroup.py
+-rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.2/aquarium/tools.py
+-rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.2/aquarium/utils.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 09:41:05.174483 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-05 09:41:04.000000 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)      703 2023-06-05 09:41:04.000000 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yann       (501) staff       (20)        1 2023-06-05 09:41:04.000000 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yann       (501) staff       (20)      123 2023-06-05 09:41:04.000000 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/requires.txt
+-rw-r--r--   0 yann       (501) staff       (20)        9 2023-06-05 09:41:04.000000 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yann       (501) staff       (20)     1280 2023-06-05 09:41:05.177946 aquarium-python-api-2.0.2/setup.cfg
+-rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.2/setup.py
```

### Comparing `aquarium-python-api-2.0.1/LICENSE.md` & `aquarium-python-api-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/PKG-INFO` & `aquarium-python-api-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.1
+Version: 2.0.2
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.1/README.md` & `aquarium-python-api-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/__init__.py` & `aquarium-python-api-2.0.2/aquarium/__init__.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/aquarium.py` & `aquarium-python-api-2.0.2/aquarium/aquarium.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # -*- coding: utf-8 -*-
-from . import JSON_CONTENT_TYPE
+import os
+import mimetypes
+
+from .auth import AquariumAuth
 from .item import Item
 from .edge import Edge
 from .tools import evaluate
 from .items.user import User
 from .items.template import Template
 from .items.project import Project
 from .items.task import Task
@@ -75,14 +78,15 @@
         # Session
         self.session=requests.Session()
 
         self.api_url=api_url
         self.api_version=api_version
         self.token=token
         self.domain=domain
+
         # Classes
         self.element=Element(parent=self)
         self.item=Item(parent=self)
         self.edge=Edge(parent=self)
         self.utils=Utils()
         # SubClasses
         self.user=User(parent=self)
@@ -109,24 +113,19 @@
         """
         token=self.token
 
         decoding=True
         if 'decoding' in kwargs:
             decoding=kwargs.pop('decoding')
 
+        headers=None
         if 'headers' in kwargs:
             headers=kwargs.pop('headers')
             if headers is not None:
                 headers.update(dict(authorization=token))
-        else:
-            headers=dict(authorization=token)
-            headers.update(JSON_CONTENT_TYPE)
-
-        if (self.domain):
-            headers['aquarium-domain'] = self.domain
 
         args=list(args)
         typ=args[0]
         path = self.api_url
 
         if len(args) > 1:
             is_files = args[1].find('/files/') >= 0
@@ -137,16 +136,15 @@
                     api_version=self.api_version,
                     endpoint=args[1]
                 ))
         else:
             path = urljoin(path, self.api_version)
 
         logger.debug('Send request : %s %s', typ, path)
-        self.session.headers.update(headers)
-        response=self.session.request(typ, path, **kwargs)
+        response=self.session.request(typ, path, headers=headers, auth=AquariumAuth(self.token, self.domain), **kwargs)
         evaluate(response)
         if decoding:
             response=response.json()
         return response
 
     def cast(self, data={}):
         """
@@ -328,17 +326,22 @@
         :param      path:  The path of the file to upload
         :type       path:  string
 
         :returns:   The file metadata on Aquarium
         :rtype:     dictionary
         """
         logger.debug('Upload file : %s', path)
-        files=dict(file=open(path, 'rb'))
-        result = self.do_request('POST', 'upload', headers={'Content-Type': None}, files=files)
-        files['file'].close()
+
+        file = open(path, 'rb')
+        filename = os.path.basename(path)
+        file_content_type = mimetypes.guess_type(filename)
+
+        files=dict(file=(filename, file, file_content_type))
+        result = self.do_request('POST', 'upload', files=files)
+        file.close()
         return result
 
     def query(self, meshql='', aliases={}):
         """
         Query entities
 
         .. tip::
```

### Comparing `aquarium-python-api-2.0.1/aquarium/edge.py` & `aquarium-python-api-2.0.2/aquarium/edge.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/element.py` & `aquarium-python-api-2.0.2/aquarium/element.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/entity.py` & `aquarium-python-api-2.0.2/aquarium/entity.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/exceptions.py` & `aquarium-python-api-2.0.2/aquarium/exceptions.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/item.py` & `aquarium-python-api-2.0.2/aquarium/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-from . import URL_CONTENT_TYPE
 import json
 import re
 import os
-from .tools import to_string_url
 from .tools import jsonify
 from .entity import Entity
 from .exceptions import Deprecated
+import mimetypes
 import logging
 logger = logging.getLogger(__name__)
 
 
 class Item(Entity):
     """
     This class describes an Item object child of Aquarium class.
@@ -249,43 +248,57 @@
             'POST', 'templates/{templateKey}/sync/{itemKey}'.format(
                 templateKey=template_key,
                 itemKey=self._key
             ))
         result = self.parent.cast(result)
         return result
 
-    def get(self, populate=False, versions=False):
+    def get(self, populate=False, history=False):
         """
         Get item object with its _key
 
         :param      populate:  Populate `item.createdBy` and `item.updatedBy` with User object
         :type       populate:  boolean
-        :param      versions:  Get previous item's data versions
-        :type       versions:  boolean, optional
+        :param      history:   Get previous item's data history
+        :type       history:   boolean, optional
 
         :returns:   Item object
         :rtype:     :class:`~aquarium.item.Item` or subclass : :class:`~aquarium.items.asset.Asset` | :class:`~aquarium.items.project.Project` | :class:`~aquarium.items.shot.Shot` | :class:`~aquarium.items.task.Task` | :class:`~aquarium.items.template.Template` | :class:`~aquarium.items.user.User` | :class:`~aquarium.items.usergroup.Usergroup`
         """
-        result = self.do_request('GET', 'items/{0}/?populate={1}&versions={2}'.format(
-            self._key, int(populate), int(versions)), headers=URL_CONTENT_TYPE)
+
+        params = {
+            'populate': populate,
+            'history': history
+        }
+
+        jsonify(params)
+
+        result = self.do_request('GET', 'items/{0}/'.format(
+            self._key), params=params)
         result = self.parent.cast(result)
         return result
 
     def get_history(self, populate=False):
         """
         Get the previous item's data history
 
         :param      populate:  Populate `item.createdBy` and `item.updatedBy` with User object
         :type       populate:  boolean, optional
 
         :returns:   The versions values
         :rtype:     list
         """
+        params = {
+            'populate': populate
+        }
+
+        jsonify(params)
+
         result = self.do_request(
-            'GET', 'items/{0}/history?populate={1}'.format(self._key, to_string_url(populate)))
+            'GET', 'items/{0}/history'.format(self._key), params=params)
         result = [self.parent.cast(data) for data in result]
         return result
 
     def get_versions(self, populate=False):
         """
         Alias of :func:`~aquarium.items.item.get_history`
         """
@@ -298,25 +311,38 @@
         :param      key:  The destination key
         :type       key:  string
 
         :returns:   List of item Object
         :rtype:     list of :class:`~aquarium.item.Item` or subclass : :class:`~aquarium.items.asset.Asset` | :class:`~aquarium.items.project.Project` | :class:`~aquarium.items.shot.Shot` | :class:`~aquarium.items.task.Task` | :class:`~aquarium.items.template.Template` | :class:`~aquarium.items.user.User` | :class:`~aquarium.items.usergroup.Usergroup`
         """
         result = self.do_request(
-            'GET', 'items/'+self._key+'/path/'+key, headers=URL_CONTENT_TYPE)
+            'GET', 'items/'+self._key+'/path/'+key)
         result = [self.parent.cast(data) for data in result]
         return result
 
     def get_permissions(self, sort=None, populate=False, offset=0, limit=50, depth=1, includeMembers=False):
         """
         Gets the permissions of the item
 
+        .. warning::
+            We are improving the behavior of depth and includeMembers parameters.
+            Feel free to reach our support if you have any questions.
 
+        :param      sort:  Sort participants with a meshQL expression. Example: 'item.data.name ASC'
+        :type       sort:  boolean, optional
         :param      populate:  Populate with User object
         :type       populate:  boolean, optional
+        :param      offset:  Number of skipped items. Used for pagination
+        :type       offset:  integer, optional
+        :param      limit:  Maximum limit of returned items
+        :type       limit:  integer, optional
+        :param      depth:  Get deeper participants.
+        :type       depth:  integer, optional
+        :param      includeMembers:  Include members of the current item
+        :type       includeMembers:  boolean, optional
 
         :returns:   List of edge and user
         :rtype:     list
         """
         params = dict(
             populate=populate,
             offset=offset,
@@ -496,15 +522,15 @@
         result = [self.parent.element(data) for data in result]
         return result
 
     def get_trash(self, meshql='# -($Child)> *'):
         """
         Gets the trashed items
 
-        :param      meshql:  The meshql string. Default is "# -($Child)> *"
+        :param      meshql:  The meshql string. Default is : # -($Child)> *
         :type       meshql:  string, optional
 
         :returns:   List of trashed item and edge object
         :rtype:     list of {item: :class:`~aquarium.item.Item`, edge: :class:`~aquarium.edge.Edge`}
         """
         result = self.traverse_trashed(meshql)
         result = [self.parent.element(data) for data in result]
@@ -572,15 +598,15 @@
             The item will be completely deleted. You can use :func:`~aquarium.item.Item.trash` instead
 
         :returns:   Deleted item object from API
         :rtype:     dictionary
         """
         logger.debug('Delete item %s', self._key)
         result = self.do_request(
-            'DELETE', 'items/'+self._key, headers=URL_CONTENT_TYPE)
+            'DELETE', 'items/'+self._key)
         return result
 
     def upload_file(self, path='', data = {}, message = None):
         """
         Upload a file on the item
 
         .. warning::
@@ -596,22 +622,26 @@
         :type       message:  string
 
         :returns:   Item object
         :rtype:     :class:`~aquarium.item.Item`
         """
         logger.debug('Upload file %s on item %s with data %s', path, self._key, data)
 
+        file = open(path, 'rb')
+        filename = os.path.basename(path)
+        file_content_type = mimetypes.guess_type(filename)
+
         files = dict(
-            file=open(path, 'rb'),
+            file=(filename, file, file_content_type),
             data=(None, json.dumps(data), 'text/plain'),
             message=(None, message, 'text/plain')
         )
         result = self.do_request(
-            'POST', 'items/'+self._key+'/upload', headers={'Content-Type': None}, files=files)
-        files['file'].close()
+            'POST', 'items/'+self._key+'/upload', files=files)
+        file.close()
         result = self.parent.cast(result)
         return result
 
     def download_file(self, path, versionKey=None):
         """
         Download the item's file to the path
 
@@ -623,15 +653,15 @@
         logger.debug('Download from item %s to file %s', self._key, path)
 
         url = 'items/{_key}/download'.format(_key=self._key)
         if (versionKey != None):
             url = '{url}?versionKey=${versionKey}'.format(versionKey=versionKey)
 
         result = self.do_request(
-            'GET', url, headers=URL_CONTENT_TYPE, decoding=False)
+            'GET', url, decoding=False)
 
         if (os.path.isdir(path)):
             content_disposition = result.headers['content-disposition']
             filename = re.findall('filename="(.+)"', content_disposition)
             print(content_disposition)
             if len(filename) > 0:
                 path = os.path.join(path, str(filename[0]))
```

### Comparing `aquarium-python-api-2.0.1/aquarium/items/asset.py` & `aquarium-python-api-2.0.2/aquarium/items/asset.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/items/organisation.py` & `aquarium-python-api-2.0.2/aquarium/items/organisation.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/items/playlist.py` & `aquarium-python-api-2.0.2/aquarium/items/playlist.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/items/project.py` & `aquarium-python-api-2.0.2/aquarium/items/project.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/items/task.py` & `aquarium-python-api-2.0.2/aquarium/items/task.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/items/template.py` & `aquarium-python-api-2.0.2/aquarium/items/template.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/items/user.py` & `aquarium-python-api-2.0.2/aquarium/items/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-from .. import URL_CONTENT_TYPE
 from ..item import Item
 from ..element import Element
 import logging
 logger = logging.getLogger(__name__)
 
 
 class User(Item):
@@ -23,15 +22,15 @@
         :returns: Dictionary User object
         :rtype: Dict {user: :class:`~aquarium.items.user.User`}
         """
         logging.debug('Connect user %s', email)
         # Authenticate and retrieve the access token
         payload = dict(email=email, password=password)
         result = self.do_request(
-            'POST', 'signin', headers=URL_CONTENT_TYPE, data=payload)
+            'POST', 'signin', data=payload)
 
        # Store authentification information
         token = result.pop("token")
         self.parent.token = token
         result = self.parent.element(result)
 
         return result
```

### Comparing `aquarium-python-api-2.0.1/aquarium/items/usergroup.py` & `aquarium-python-api-2.0.2/aquarium/items/usergroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 import json
-from .. import URL_CONTENT_TYPE
 from ..item import Item
 import logging
 logger = logging.getLogger(__name__)
 
 
 class Usergroup(Item):
     """
@@ -15,15 +14,15 @@
         """
         Get the users of the user group
 
         :returns:   List of User object
         :rtype:     List of :class:`~aquarium.items.user.User`
         """
         result = self.do_request(
-            'GET', 'usergroups/'+self._key, headers=URL_CONTENT_TYPE)
+            'GET', 'usergroups/'+self._key)
 
         result = [self.parent.cast(data) for data in result]
         return result
 
     def add_user(self, user_key=''):
         """
         Add an user in the user group
```

### Comparing `aquarium-python-api-2.0.1/aquarium/tools.py` & `aquarium-python-api-2.0.2/aquarium/tools.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium/utils.py` & `aquarium-python-api-2.0.2/aquarium/utils.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.1/aquarium_python_api.egg-info/PKG-INFO` & `aquarium-python-api-2.0.2/aquarium_python_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.1
+Version: 2.0.2
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.1/aquarium_python_api.egg-info/SOURCES.txt` & `aquarium-python-api-2.0.2/aquarium_python_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.md
 README.md
 setup.cfg
 setup.py
 aquarium/__init__.py
 aquarium/aquarium.py
+aquarium/auth.py
 aquarium/edge.py
 aquarium/element.py
 aquarium/entity.py
 aquarium/exceptions.py
 aquarium/item.py
 aquarium/tools.py
 aquarium/utils.py
```

### Comparing `aquarium-python-api-2.0.1/setup.cfg` & `aquarium-python-api-2.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://docs.fatfish.app/dev/python/index.html
 project_urls = 
 	Documentation = https://docs.fatfish.app/dev/python/index.html
 	Source = https://github.com/fatfish-lab/aquarium-python-api
 	Aquarium = https://fatfi.sh/aquarium
-version = 2.0.1
+version = 2.0.2
 author = Fatfish Lab
 author_email = lab@fatfi.sh
 keywords = fatfish, lab, aquarium, studio, project, management, nodal, sdk, rest, cgi, vfx, api, python
 license = gpl-3.0
 license_file = LICENSE.md
 platform = any
 python_requires = '>=2.4'
```

