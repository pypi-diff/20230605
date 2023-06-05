# Comparing `tmp/aquarium-python-api-2.0.2.tar.gz` & `tmp/aquarium-python-api-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquarium-python-api-2.0.2.tar", last modified: Mon Jun  5 09:41:05 2023, max compression
+gzip compressed data, was "dist/aquarium-python-api-2.0.3.tar", last modified: Mon Jun  5 10:12:25 2023, max compression
```

## Comparing `aquarium-python-api-2.0.2.tar` & `aquarium-python-api-2.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 09:41:05.175207 aquarium-python-api-2.0.2/
--rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.2/LICENSE.md
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-05 09:41:05.175576 aquarium-python-api-2.0.2/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.2/README.md
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 09:41:05.145030 aquarium-python-api-2.0.2/aquarium/
--rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.0.2/aquarium/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)    12529 2023-06-05 09:35:55.000000 aquarium-python-api-2.0.2/aquarium/aquarium.py
--rw-r--r--   0 yann       (501) staff       (20)      364 2023-06-05 08:31:35.000000 aquarium-python-api-2.0.2/aquarium/auth.py
--rw-r--r--   0 yann       (501) staff       (20)     3399 2022-11-09 16:10:59.000000 aquarium-python-api-2.0.2/aquarium/edge.py
--rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.2/aquarium/element.py
--rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.2/aquarium/entity.py
--rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.2/aquarium/exceptions.py
--rw-r--r--   0 yann       (501) staff       (20)    27572 2023-06-05 09:32:37.000000 aquarium-python-api-2.0.2/aquarium/item.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 09:41:05.168399 aquarium-python-api-2.0.2/aquarium/items/
--rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.2/aquarium/items/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.2/aquarium/items/asset.py
--rw-r--r--   0 yann       (501) staff       (20)     5092 2023-04-15 09:03:56.000000 aquarium-python-api-2.0.2/aquarium/items/organisation.py
--rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.2/aquarium/items/playlist.py
--rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.2/aquarium/items/project.py
--rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.2/aquarium/items/shot.py
--rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.2/aquarium/items/task.py
--rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.2/aquarium/items/template.py
--rw-r--r--   0 yann       (501) staff       (20)     4029 2023-06-05 09:29:59.000000 aquarium-python-api-2.0.2/aquarium/items/user.py
--rw-r--r--   0 yann       (501) staff       (20)     1595 2023-06-05 09:30:04.000000 aquarium-python-api-2.0.2/aquarium/items/usergroup.py
--rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.2/aquarium/tools.py
--rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.2/aquarium/utils.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 09:41:05.174483 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-05 09:41:04.000000 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)      703 2023-06-05 09:41:04.000000 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yann       (501) staff       (20)        1 2023-06-05 09:41:04.000000 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yann       (501) staff       (20)      123 2023-06-05 09:41:04.000000 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/requires.txt
--rw-r--r--   0 yann       (501) staff       (20)        9 2023-06-05 09:41:04.000000 aquarium-python-api-2.0.2/aquarium_python_api.egg-info/top_level.txt
--rw-r--r--   0 yann       (501) staff       (20)     1280 2023-06-05 09:41:05.177946 aquarium-python-api-2.0.2/setup.cfg
--rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.2/setup.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:12:25.695484 aquarium-python-api-2.0.3/
+-rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.3/LICENSE.md
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-05 10:12:25.695887 aquarium-python-api-2.0.3/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.3/README.md
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:12:25.669954 aquarium-python-api-2.0.3/aquarium/
+-rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.0.3/aquarium/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)    12505 2023-06-05 10:02:50.000000 aquarium-python-api-2.0.3/aquarium/aquarium.py
+-rw-r--r--   0 yann       (501) staff       (20)      364 2023-06-05 08:31:35.000000 aquarium-python-api-2.0.3/aquarium/auth.py
+-rw-r--r--   0 yann       (501) staff       (20)     3351 2023-06-05 10:10:06.000000 aquarium-python-api-2.0.3/aquarium/edge.py
+-rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.3/aquarium/element.py
+-rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.3/aquarium/entity.py
+-rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.3/aquarium/exceptions.py
+-rw-r--r--   0 yann       (501) staff       (20)    27404 2023-06-05 10:06:41.000000 aquarium-python-api-2.0.3/aquarium/item.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:12:25.689102 aquarium-python-api-2.0.3/aquarium/items/
+-rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.3/aquarium/items/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.3/aquarium/items/asset.py
+-rw-r--r--   0 yann       (501) staff       (20)     5068 2023-06-05 10:10:16.000000 aquarium-python-api-2.0.3/aquarium/items/organisation.py
+-rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.3/aquarium/items/playlist.py
+-rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.3/aquarium/items/project.py
+-rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.3/aquarium/items/shot.py
+-rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.3/aquarium/items/task.py
+-rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.3/aquarium/items/template.py
+-rw-r--r--   0 yann       (501) staff       (20)     4029 2023-06-05 09:29:59.000000 aquarium-python-api-2.0.3/aquarium/items/user.py
+-rw-r--r--   0 yann       (501) staff       (20)     1559 2023-06-05 10:10:25.000000 aquarium-python-api-2.0.3/aquarium/items/usergroup.py
+-rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.3/aquarium/tools.py
+-rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.3/aquarium/utils.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-05 10:12:25.694871 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-05 10:12:25.000000 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)      703 2023-06-05 10:12:25.000000 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yann       (501) staff       (20)        1 2023-06-05 10:12:25.000000 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yann       (501) staff       (20)      123 2023-06-05 10:12:25.000000 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/requires.txt
+-rw-r--r--   0 yann       (501) staff       (20)        9 2023-06-05 10:12:25.000000 aquarium-python-api-2.0.3/aquarium_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yann       (501) staff       (20)     1280 2023-06-05 10:12:25.697665 aquarium-python-api-2.0.3/setup.cfg
+-rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.3/setup.py
```

### Comparing `aquarium-python-api-2.0.2/LICENSE.md` & `aquarium-python-api-2.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/PKG-INFO` & `aquarium-python-api-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.2
+Version: 2.0.3
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.2/README.md` & `aquarium-python-api-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/__init__.py` & `aquarium-python-api-2.0.3/aquarium/__init__.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/aquarium.py` & `aquarium-python-api-2.0.3/aquarium/aquarium.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
         """
 
         payload = dict(email=email)
         if name != None:
             payload['name'] = name
 
         user = self.do_request(
-            'POST', 'users', data=json.dumps(payload))
+            'POST', 'users', json=payload)
 
         user = self.cast(user)
         return user
 
     def upload_file(self, path=''):
         """
         Uploads a file on the server
@@ -354,15 +354,15 @@
 
         :returns:   List of item, edge or VIEW used in the meshql query
         :rtype:     list
         """
         logger.debug('Send query : meshql : %s / aliases : %r',
                      meshql, aliases)
         data=dict(query=meshql, aliases=aliases)
-        result=self.do_request('POST', 'query', data=json.dumps(data))
+        result=self.do_request('POST', 'query', json=data)
         return result
 
     def get_file(self, file_path):
         """
         Get stored file on Aquarium server
 
         :param      file_path:     The file path from item property (Exemple: `/files/file_id.jpg`)
```

### Comparing `aquarium-python-api-2.0.2/aquarium/edge.py` & `aquarium-python-api-2.0.3/aquarium/edge.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-import json
 from .tools import to_string_url
 from .entity import Entity
 
 
 class Edge(Entity):
     """
     This class describes an Edge object child of Aquarium class.
@@ -40,15 +39,15 @@
         :rtype:     :class:`~aquarium.edge.Edge`
         """
         payload = dict(fromKey=from_key,
                        toKey=to_key,
                        type=type,
                        data=data)
 
-        result = self.do_request('POST', 'edges', data=json.dumps(payload))
+        result = self.do_request('POST', 'edges', json=payload)
         result = self.parent.cast(result)
         return result
 
     def replace_data(self, data={}):
         """
         Replace the edge data with new ones
 
@@ -60,15 +59,15 @@
         :type       data:  dictionary
 
         :returns:   Edge object
         :rtype:     :class:`~aquarium.edge.Edge`
         """
         data = dict(data=data)
         result = self.do_request(
-            'PUT', 'edges/'+self._key, data=json.dumps(data))
+            'PUT', 'edges/'+self._key, json=data)
         result = self.parent.cast(result)
         return result
 
     def update_data(self, data={}):
         """
         Update the edge data by merging the existing ones with the new ones
 
@@ -76,15 +75,15 @@
         :type       data:  dictionary
 
         :returns:   Edge object
         :rtype:     :class:`~aquarium.edge.Edge`
         """
         data = dict(data=data)
         result = self.do_request(
-            'PATCH', 'edges/'+self._key, data=json.dumps(data))
+            'PATCH', 'edges/'+self._key, json=data)
         result = self.parent.cast(result)
         return result
 
     def get(self, populate=False):
         """
         Get the edge by its _key
```

### Comparing `aquarium-python-api-2.0.2/aquarium/element.py` & `aquarium-python-api-2.0.3/aquarium/element.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/entity.py` & `aquarium-python-api-2.0.3/aquarium/entity.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/exceptions.py` & `aquarium-python-api-2.0.3/aquarium/exceptions.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/item.py` & `aquarium-python-api-2.0.3/aquarium/item.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         :type       path:  string, optional
 
         :returns:   Item object
         :rtype:     :class:`~aquarium.item.Item` or subclass : :class:`~aquarium.items.asset.Asset` | :class:`~aquarium.items.project.Project` | :class:`~aquarium.items.shot.Shot` | :class:`~aquarium.items.task.Task` | :class:`~aquarium.items.template.Template` | :class:`~aquarium.items.user.User` | :class:`~aquarium.items.usergroup.Usergroup`
         """
 
         payload = dict(type=type, data=data)
-        result = self.do_request('POST', 'items', data=json.dumps(payload))
+        result = self.do_request('POST', 'items', json=payload)
         result = self.parent.cast(result)
 
         if path != None:
             upload = result.upload_file(path=path)
             if upload != None:
                 for key in upload.data:
                     result.data[key] = upload.data[key]
@@ -85,15 +85,15 @@
         if apply_template is not None:
             payload["applyTemplate"] = apply_template
 
         if template_key:
             payload["templateKey"] = template_key
 
         result = self.do_request(
-            'POST', 'items/'+self._key+'/append', data=json.dumps(payload))
+            'POST', 'items/'+self._key+'/append', json=payload)
         result = self.parent.element(result)
 
         if path != None:
             upload = result.item.upload_file(path=path)
             if upload != None:
                 for key in upload.data:
                     result.item.data[key] = upload.data[key]
@@ -112,15 +112,15 @@
         :returns:   List of item and/or edge or VIEW used in the meshql query
         :rtype:     list
         """
         logger.debug('Send traverse : meshql : %s / aliases : %r',
                      meshql, aliases)
         data = dict(query=meshql, aliases=aliases)
         result = self.do_request(
-            'POST', 'items/'+self._key+'/traverse', data=json.dumps(data))
+            'POST', 'items/'+self._key+'/traverse', json=data)
         return result
 
     def traverse_trashed(self, meshql='', aliases={}):
         """
         Execute a traverse from the current item on trashed_items
 
         :param      meshql:        The meshql string
@@ -131,15 +131,15 @@
         :returns:   List of item and/or edge or VIEW used in the meshql query
         :rtype:     list
         """
         logger.debug('Send traverse trashed_items : meshql : %s / aliases : %r',
                      meshql, aliases)
         data = dict(query=meshql, aliases=aliases)
         result = self.do_request(
-            'POST', 'trashed_items/'+self._key+'/traverse', data=json.dumps(data))
+            'POST', 'trashed_items/'+self._key+'/traverse', json=data)
         return result
 
     def replace_data(self, data={}):
         """
         Replace the item data with new ones
 
         .. danger::
@@ -151,15 +151,15 @@
 
         :returns:   Item object
         :rtype:     :class:`~aquarium.item.Item`
         """
         logger.debug('Replacing data on item %s with %r', self._key, data)
         data = dict(data=data)
         result = self.do_request(
-            'PUT', 'items/'+self._key, data=json.dumps(data))
+            'PUT', 'items/'+self._key, json=data)
 
         result = self.parent.cast(result)
         return result
 
     def update_data(self, data={}):
         """
         Update the item data by merging the existing ones with the new ones
@@ -169,15 +169,15 @@
 
         :returns:   Item object
         :rtype:     :class:`~aquarium.item.Item`
         """
         logger.debug('Updating data on item %s with %r', self._key, data)
         data = dict(data=data)
         result = self.do_request(
-            'PATCH', 'items/'+self._key, data=json.dumps(data))
+            'PATCH', 'items/'+self._key, json=data)
         result = self.parent.cast(result)
         return result
 
     def copy(self, parent_key=''):
         """
         Copie the item into the parent
 
@@ -186,15 +186,15 @@
 
         :returns:   List of new items object
         :rtype:     List of :class:`~aquarium.item.Item` or subclass : :class:`~aquarium.items.asset.Asset` | :class:`~aquarium.items.project.Project` | :class:`~aquarium.items.shot.Shot` | :class:`~aquarium.items.task.Task` | :class:`~aquarium.items.template.Template` | :class:`~aquarium.items.user.User` | :class:`~aquarium.items.usergroup.Usergroup`
         """
         logger.debug('Copy item %s into %s', self._key, parent_key)
         data = dict(targetKey=parent_key)
         result = self.do_request(
-            'POST', 'items/'+self._key+'/copy', data=json.dumps(data))
+            'POST', 'items/'+self._key+'/copy', json=data)
 
         result = [self.parent.cast(data) for data in result]
         return result
 
     def convert_to_template(self, parent_key=''):
         """
         Convert an item and its hierarchy to a template into a parent
@@ -205,15 +205,15 @@
         :returns:   template object
         :rtype:     :class:`~aquarium.items.template.Template`
         """
         logger.debug('Converting item %s to template in %s',
                      self._key, parent_key)
         data = dict(parentKey=parent_key)
         result = self.do_request(
-            'POST', 'items/'+self._key+'/convertToTemplate', data=json.dumps(data))
+            'POST', 'items/'+self._key+'/convertToTemplate', json=data)
         result = self.parent.cast(result)
         return result
 
     def apply_template(self, template_key=''):
         """
         Apply a template on the item
 
@@ -222,15 +222,15 @@
 
         :returns:   Item object
         :rtype:     :class:`~aquarium.item.Item` or subclass : :class:`~aquarium.items.asset.Asset` | :class:`~aquarium.items.project.Project` | :class:`~aquarium.items.shot.Shot` | :class:`~aquarium.items.task.Task` | :class:`~aquarium.items.template.Template` | :class:`~aquarium.items.user.User` | :class:`~aquarium.items.usergroup.Usergroup`
         """
         logger.debug('Apply template %s on item %s', template_key, self._key)
         data = dict(templateKey=template_key)
         result = self.do_request(
-            'POST', 'items/'+self._key+'/template', data=json.dumps(data))
+            'POST', 'items/'+self._key+'/template', json=data)
         result = self.parent.cast(result)
         return result
 
     def reapply_template(self, template_key=None):
         """
         Re-apply the specific template
 
@@ -402,15 +402,15 @@
             'userKey': participant_key,
             'data': {
                 'permissions': permissions
             },
             'propagate': propagate
         }
         result = self.do_request(
-            'POST', 'items/{0}/permissions'.format(self._key), data=json.dumps(data))
+            'POST', 'items/{0}/permissions'.format(self._key), json=data)
         result['user'] = self.parent.cast(result['user'])
         return result
 
     def remove_permission(self, participant_key):
         """
         Remove an existing permission from an item. It's like unsharing an item to an existing user, usergroup or organisation.
 
@@ -420,15 +420,15 @@
         :returns:   A dict with the {user: participant, edge: the removed permission edge}
         :rtype:     dict
         """
         data = {
             'userKey': participant_key
         }
         result = self.do_request(
-            'DELETE', 'items/{0}/permissions'.format(self._key), data=json.dumps(data))
+            'DELETE', 'items/{0}/permissions'.format(self._key), json=data)
         result['user'] = self.parent.cast(result['user'])
         return result
 
     def update_permission(self, participant_key, permissions, propagate=True):
         """
         Update an existing permission on an item.
 
@@ -450,15 +450,15 @@
             'data': {
                 'permissions': permissions
             },
             'propagate': propagate
 
         }
         result = self.do_request(
-            'PATCH', 'items/{0}/permissions'.format(self._key), data=json.dumps(data))
+            'PATCH', 'items/{0}/permissions'.format(self._key), json=data)
         result['user'] = self.parent.cast(result['user'])
         return result
 
     def get_parents(self, limit = 50, offset = 0):
         """
         Gets the parents of the item
 
@@ -552,15 +552,15 @@
                      self._key, old_parent_key, new_parent_key)
         data = dict(
             oldParentKey=old_parent_key,
             newParentKey=new_parent_key
         )
 
         result = self.do_request(
-            'PUT', 'items/'+self._key+'/move', data=json.dumps(data))
+            'PUT', 'items/'+self._key+'/move', json=data)
         result = self.parent.element(result)
         return result
 
     def trash(self):
         """
         Move item to the trash
 
@@ -679,15 +679,15 @@
         :param      content:  The json content
         :type       content:  dictionary
 
         :returns:   Dictionary of imported items and edges
         :rtype:     dictionary
         """
         result = self.do_request(
-            'POST', 'items/'+self._key+'/import/json', data=json.dumps(content))
+            'POST', 'items/'+self._key+'/import/json', json=content)
         return result
 
     def export_json(self):
         """
         Export item hierarchy to json
 
         :returns:   Exported items and edges
```

### Comparing `aquarium-python-api-2.0.2/aquarium/items/asset.py` & `aquarium-python-api-2.0.3/aquarium/items/asset.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/items/organisation.py` & `aquarium-python-api-2.0.3/aquarium/items/organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-import json
 from ..item import Item
 
 
 class Organisation(Item):
     """
     This class describes an Organisation object child of Item class.
     """
@@ -104,15 +103,15 @@
         """
 
         payload = dict(userKey=user_key)
 
         member = self.do_request(
             'POST', 'organisations/{organisationKey}/members'.format(
                 organisationKey=self._key
-            ), data=json.dumps(payload))
+            ), json=payload)
 
         member = self.parent.cast(member)
 
         return member
 
     def create_member(self, email, name=None):
         """
```

### Comparing `aquarium-python-api-2.0.2/aquarium/items/playlist.py` & `aquarium-python-api-2.0.3/aquarium/items/playlist.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/items/project.py` & `aquarium-python-api-2.0.3/aquarium/items/project.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/items/task.py` & `aquarium-python-api-2.0.3/aquarium/items/task.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/items/template.py` & `aquarium-python-api-2.0.3/aquarium/items/template.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/items/user.py` & `aquarium-python-api-2.0.3/aquarium/items/user.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/items/usergroup.py` & `aquarium-python-api-2.0.3/aquarium/items/usergroup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-import json
 from ..item import Item
 import logging
 logger = logging.getLogger(__name__)
 
 
 class Usergroup(Item):
     """
@@ -32,15 +31,15 @@
 
         :returns:   Membership edge object
         :rtype:     dictionary
         """
         logger.debug('Add user %s to usergroup %s', user_key, self._key)
         payload = dict(userKey=user_key)
         result = self.do_request(
-            'POST', 'usergroups/'+self._key, data=json.dumps(payload))
+            'POST', 'usergroups/'+self._key, json=payload)
         return result
 
     def remove_user(self, user_key=''):
         """
         Remove an user from the user group
 
         :param      user_key:  The user key
@@ -48,9 +47,9 @@
 
         :returns:   Deleted membership edge object
         :rtype:     dictionary
         """
         logger.debug('Remove user %s to usergroup %s', user_key, self._key)
         payload = dict(userKey=user_key)
         result = self.do_request(
-            'DELETE', 'usergroups/'+self._key, data=json.dumps(payload))
+            'DELETE', 'usergroups/'+self._key, json=payload)
         return result
```

### Comparing `aquarium-python-api-2.0.2/aquarium/tools.py` & `aquarium-python-api-2.0.3/aquarium/tools.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium/utils.py` & `aquarium-python-api-2.0.3/aquarium/utils.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/aquarium_python_api.egg-info/PKG-INFO` & `aquarium-python-api-2.0.3/aquarium_python_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.2
+Version: 2.0.3
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.2/aquarium_python_api.egg-info/SOURCES.txt` & `aquarium-python-api-2.0.3/aquarium_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.2/setup.cfg` & `aquarium-python-api-2.0.3/setup.cfg`

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
-version = 2.0.2
+version = 2.0.3
 author = Fatfish Lab
 author_email = lab@fatfi.sh
 keywords = fatfish, lab, aquarium, studio, project, management, nodal, sdk, rest, cgi, vfx, api, python
 license = gpl-3.0
 license_file = LICENSE.md
 platform = any
 python_requires = '>=2.4'
```

