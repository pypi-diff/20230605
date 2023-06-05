# Comparing `tmp/switchboard-1.6.3.tar.gz` & `tmp/switchboard-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/switchboard-1.6.3.tar", last modified: Thu Mar  2 21:27:33 2023, max compression
+gzip compressed data, was "dist/switchboard-1.6.4.tar", last modified: Mon Jun  5 20:05:02 2023, max compression
```

## Comparing `switchboard-1.6.3.tar` & `switchboard-1.6.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 21:27:33.000000 switchboard-1.6.3/
--rw-r--r--   0 root         (0) root         (0)    10834 2022-03-02 19:31:43.000000 switchboard-1.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2022-03-02 19:31:43.000000 switchboard-1.6.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5965 2023-03-02 21:27:33.000000 switchboard-1.6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5065 2023-03-02 21:08:31.000000 switchboard-1.6.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-02 21:27:33.000000 switchboard-1.6.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1601 2023-03-02 21:08:31.000000 switchboard-1.6.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard/
--rw-r--r--   0 root         (0) root         (0)      376 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard/admin/
--rw-r--r--   0 root         (0) root         (0)     6533 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/admin/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42936 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/admin/index.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard/admin/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-02 19:31:43.000000 switchboard-1.6.3/switchboard/admin/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/admin/utils.py
--rw-r--r--   0 root         (0) root         (0)    10473 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/base.py
--rw-r--r--   0 root         (0) root         (0)     2217 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/builtins.py
--rw-r--r--   0 root         (0) root         (0)    13257 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/conditions.py
--rw-r--r--   0 root         (0) root         (0)      730 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/decorators.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/helpers.py
--rw-r--r--   0 root         (0) root         (0)     9996 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/manager.py
--rw-r--r--   0 root         (0) root         (0)     1377 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/middleware.py
--rw-r--r--   0 root         (0) root         (0)    15957 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/models.py
--rw-r--r--   0 root         (0) root         (0)     1183 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/proxy.py
--rw-r--r--   0 root         (0) root         (0)     1329 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/settings.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/signals.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/template_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-02 19:31:43.000000 switchboard-1.6.3/switchboard/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard/tests/admin/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-02 19:31:43.000000 switchboard-1.6.3/switchboard/tests/admin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2270 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/tests/admin/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    14236 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/tests/test_base.py
--rw-r--r--   0 root         (0) root         (0)     5427 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/tests/test_builtins.py
--rw-r--r--   0 root         (0) root         (0)    13989 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/tests/test_conditions.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/tests/test_decorators.py
--rw-r--r--   0 root         (0) root         (0)    27738 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/tests/test_manager.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/tests/test_middleware.py
--rw-r--r--   0 root         (0) root         (0)    17577 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     1547 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/tests/test_testutils.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-03-02 21:08:31.000000 switchboard-1.6.3/switchboard/testutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5965 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1094 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 21:10:06.000000 switchboard-1.6.3/switchboard.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-02 21:27:33.000000 switchboard-1.6.3/switchboard.egg-info/top_level.txt
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-06-05 20:05:02.000000 switchboard-1.6.4/
+-rw-r--r--   0 brondsem   (502) staff       (20)    10834 2019-05-17 17:43:22.000000 switchboard-1.6.4/LICENSE
+-rw-r--r--   0 brondsem   (502) staff       (20)       55 2019-07-10 21:43:35.000000 switchboard-1.6.4/MANIFEST.in
+-rw-r--r--   0 brondsem   (502) staff       (20)     5965 2023-06-05 20:05:02.000000 switchboard-1.6.4/PKG-INFO
+-rw-r--r--   0 brondsem   (502) staff       (20)     5065 2022-03-18 16:19:22.000000 switchboard-1.6.4/README.md
+-rw-r--r--   0 brondsem   (502) staff       (20)       38 2023-06-05 20:05:02.000000 switchboard-1.6.4/setup.cfg
+-rw-r--r--   0 brondsem   (502) staff       (20)     1596 2023-06-05 20:03:46.000000 switchboard-1.6.4/setup.py
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-06-05 20:05:02.000000 switchboard-1.6.4/switchboard/
+-rw-r--r--   0 brondsem   (502) staff       (20)      376 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/__init__.py
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-06-05 20:05:02.000000 switchboard-1.6.4/switchboard/admin/
+-rw-r--r--   0 brondsem   (502) staff       (20)     6533 2023-01-10 17:46:12.000000 switchboard-1.6.4/switchboard/admin/__init__.py
+-rw-r--r--   0 brondsem   (502) staff       (20)    42936 2022-06-20 18:58:47.000000 switchboard-1.6.4/switchboard/admin/index.tpl
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-06-05 20:05:02.000000 switchboard-1.6.4/switchboard/admin/templates/
+-rw-r--r--   0 brondsem   (502) staff       (20)        0 2019-05-17 17:43:22.000000 switchboard-1.6.4/switchboard/admin/templates/__init__.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     1650 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/admin/utils.py
+-rw-r--r--   0 brondsem   (502) staff       (20)    10473 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/base.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     2217 2023-06-05 16:36:27.000000 switchboard-1.6.4/switchboard/builtins.py
+-rw-r--r--   0 brondsem   (502) staff       (20)    13257 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/conditions.py
+-rw-r--r--   0 brondsem   (502) staff       (20)      730 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/decorators.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     2434 2023-06-05 20:03:26.000000 switchboard-1.6.4/switchboard/helpers.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     9996 2022-06-20 18:58:47.000000 switchboard-1.6.4/switchboard/manager.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     1377 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/middleware.py
+-rw-r--r--   0 brondsem   (502) staff       (20)    16490 2023-06-05 20:03:26.000000 switchboard-1.6.4/switchboard/models.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     1183 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/proxy.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     1329 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/settings.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     2533 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/signals.py
+-rw-r--r--   0 brondsem   (502) staff       (20)      812 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/template_helpers.py
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-06-05 20:05:02.000000 switchboard-1.6.4/switchboard/tests/
+-rw-r--r--   0 brondsem   (502) staff       (20)        0 2019-05-17 17:43:22.000000 switchboard-1.6.4/switchboard/tests/__init__.py
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-06-05 20:05:02.000000 switchboard-1.6.4/switchboard/tests/admin/
+-rw-r--r--   0 brondsem   (502) staff       (20)        0 2019-07-31 20:55:21.000000 switchboard-1.6.4/switchboard/tests/admin/__init__.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     2270 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/tests/admin/test_utils.py
+-rw-r--r--   0 brondsem   (502) staff       (20)    14236 2023-01-10 17:46:12.000000 switchboard-1.6.4/switchboard/tests/test_base.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     5427 2023-06-05 16:36:27.000000 switchboard-1.6.4/switchboard/tests/test_builtins.py
+-rw-r--r--   0 brondsem   (502) staff       (20)    13989 2023-01-10 17:46:12.000000 switchboard-1.6.4/switchboard/tests/test_conditions.py
+-rw-r--r--   0 brondsem   (502) staff       (20)      917 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/tests/test_decorators.py
+-rw-r--r--   0 brondsem   (502) staff       (20)    27738 2023-01-10 17:46:12.000000 switchboard-1.6.4/switchboard/tests/test_manager.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     1277 2023-01-10 17:46:12.000000 switchboard-1.6.4/switchboard/tests/test_middleware.py
+-rw-r--r--   0 brondsem   (502) staff       (20)    17577 2023-01-10 17:46:12.000000 switchboard-1.6.4/switchboard/tests/test_models.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     1547 2023-01-10 17:46:12.000000 switchboard-1.6.4/switchboard/tests/test_testutils.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     1872 2022-06-20 18:02:43.000000 switchboard-1.6.4/switchboard/testutils.py
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-06-05 20:05:02.000000 switchboard-1.6.4/switchboard.egg-info/
+-rw-r--r--   0 brondsem   (502) staff       (20)     5965 2023-06-05 20:05:00.000000 switchboard-1.6.4/switchboard.egg-info/PKG-INFO
+-rw-r--r--   0 brondsem   (502) staff       (20)     1094 2023-06-05 20:05:02.000000 switchboard-1.6.4/switchboard.egg-info/SOURCES.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)        1 2023-06-05 20:05:00.000000 switchboard-1.6.4/switchboard.egg-info/dependency_links.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)        1 2019-07-12 18:45:29.000000 switchboard-1.6.4/switchboard.egg-info/not-zip-safe
+-rw-r--r--   0 brondsem   (502) staff       (20)       60 2023-06-05 20:05:01.000000 switchboard-1.6.4/switchboard.egg-info/requires.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)       12 2023-06-05 20:05:01.000000 switchboard-1.6.4/switchboard.egg-info/top_level.txt
```

### Comparing `switchboard-1.6.3/LICENSE` & `switchboard-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/PKG-INFO` & `switchboard-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchboard
-Version: 1.6.3
+Version: 1.6.4
 Summary: Feature flipper for Pyramid, Pylons, or TurboGears apps.
 Home-page: https://github.com/switchboardpy/switchboard/
 Download-URL: https://github.com/switchboardpy/switchboard/releases
 Author: Kyle Adams
 Author-email: kadams54@users.noreply.github.com
 License: Apache License
 Keywords: switches feature flipper pyramid pylons turbogears
```

### Comparing `switchboard-1.6.3/README.md` & `switchboard-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/setup.py` & `switchboard-1.6.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
-VERSION = '1.6.3'
+VERSION = '1.6.4'
 INSTALL_REQUIRES = [
-    'pymongo >= 3, < 4',
+    'pymongo >= 3',
     'blinker >= 1.2',
     'WebOb >= 0.9',
     'Mako >= 0.9',
     'bottle >= 0.12.8',
 ]
 
 this_directory = Path(__file__).parent
```

### Comparing `switchboard-1.6.3/switchboard/admin/__init__.py` & `switchboard-1.6.4/switchboard/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/admin/index.tpl` & `switchboard-1.6.4/switchboard/admin/index.tpl`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/admin/utils.py` & `switchboard-1.6.4/switchboard/admin/utils.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/base.py` & `switchboard-1.6.4/switchboard/base.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/builtins.py` & `switchboard-1.6.4/switchboard/builtins.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/conditions.py` & `switchboard-1.6.4/switchboard/conditions.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/decorators.py` & `switchboard-1.6.4/switchboard/decorators.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/helpers.py` & `switchboard-1.6.4/switchboard/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,53 +44,48 @@
                 results.append(d)
         return results or None
 
     def _update_partial(self, old, new):
         for k, v in new.items():
             old[k] = v
 
-    def update(self, spec, update, upsert=False):
+    def update_one(self, spec, update, upsert=False):
         current = self.find_one(spec)
         if not current:
             if upsert:
+                update = update.get('$set', update)
                 spec.update(update)
-                return self.save(spec)
-            else:
-                return {
-                    'err': None,
-                    'n': 1,
-                    'ok': 1.0,
-                    'updatedExisting': True
-                }
-        for k, v in update.items():
-            if k == '$set':
-                self._update_partial(current, v)
-            else:
-                current[k] = v
+                return self.insert_one(spec)
+        else:
+            for k, v in update.items():
+                if k == '$set':
+                    self._update_partial(current, v)
+                else:
+                    current[k] = v
+
         return {
             'err': None,
             'n': 1,
             'ok': 1.0,
             'updatedExisting': True
         }
 
-    def remove(self, spec):
+    def delete_one(self, spec):
         doc = self.find_one(spec)
         if doc:
             self._data.remove(doc)
             return {'err': None, 'n': 1, 'ok': 1.0}
 
-    def save(self, document):
-        if not document.get('_id'):
+    def insert_one(self, document):
+        _id = document.get('_id')
+        if not _id:
             _id = str(len(self._data))
             document['_id'] = _id
-            self._data.append(document)
-        else:
-            _id = document['_id']
-            self.update({'_id': _id}, document)
+
+        self._data.append(document)
         return _id
 
     def drop(self):
         self._data = []
 
     def count(self):
         return len(self._data)
```

### Comparing `switchboard-1.6.3/switchboard/manager.py` & `switchboard-1.6.4/switchboard/manager.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/middleware.py` & `switchboard-1.6.4/switchboard/middleware.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/models.py` & `switchboard-1.6.4/switchboard/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 from datetime import datetime
 import logging
 
 from blinker import signal
 from pymongo import DESCENDING
+from pymongo.results import InsertOneResult
 
 from .settings import settings
 from .helpers import MockCollection
 
 log = logging.getLogger(__name__)
 
 DISABLED = 1
@@ -46,15 +47,25 @@
 
     def save(self):
         if hasattr(self, '_id'):
             previous = self.get(_id=self._id)
         else:
             previous = None
         self.pre_save.send(previous)
-        _id = self.c.save(self.to_bson())
+
+        if not previous:
+            result = self.c.insert_one(self.to_bson())
+            # When pymongo's implementation of insert_one is used, it returns an InsertOneResult
+            # instead of a plain _id, so we need to check the type to return the proper value
+            _id = result.inserted_id if type(result) is InsertOneResult else result
+        else:
+            document = self.to_bson()
+            _id = document['_id']
+            self.c.update_one({'_id': _id}, {'$set': document})
+
         if not hasattr(self, '_id'):
             self._id = _id
         self.post_save.send(self)
         return _id
 
     def delete(self):
         return self.remove(key=self.key)
@@ -83,15 +94,15 @@
         if not result:
             created = True
             result = kwargs
             result.update(defaults)
             # Do an upsert here instead of a straight create to avoid a race
             # condition with another instance creating the same record at
             # nearly the same time.
-            cls.update(result, result, upsert=True)
+            cls.update(result, {'$set': result}, upsert=True)
             result = cls.c.find_one(kwargs)
             instance = cls(**result)
         else:
             created = False
             instance = cls(**result)
         return instance, created
 
@@ -105,24 +116,24 @@
         Mimics a subset of PyMongo's Collection.update functionality. The spec
         is used to search for the document to update, document contains the
         values to be updated, and upsert specifies whether to do an insert if
         the original document is not found.
         '''
         previous = cls.get(**spec)
         cls.pre_save.send(previous)
-        result = cls.c.update(spec, document, upsert=upsert)
+        result = cls.c.update_one(spec, document, upsert=upsert)
         current = cls.get(**spec)
         cls.post_save.send(current)
         return result
 
     @classmethod
     def remove(cls, **kwargs):
         instance = cls.get(**kwargs)
         cls.pre_delete.send(instance)
-        result = cls.c.remove(kwargs)
+        result = cls.c.delete_one(kwargs)
         cls.post_delete.send(instance)
         return result
 
     @classmethod
     def all(cls):
         return [cls(**s) for s in cls.c.find()]
 
@@ -189,15 +200,15 @@
         if delta and (delta['added'] or delta['deleted'] or delta['changed']):
             doc = dict(
                 switch_id=self._id,
                 timestamp=datetime.utcnow(),
                 delta=delta,
                 **kwargs
             )
-            self._versioned_collection().save(doc)
+            self._versioned_collection().insert_one(doc)
 
     def _unpack_delta(self, version):
         '''
         Helper function that makes it easier to access the data nested with a
         delta. Returns a tuple of (delta, added, deleted, changed).
         '''
         delta = version.get('delta', {})
```

### Comparing `switchboard-1.6.3/switchboard/proxy.py` & `switchboard-1.6.4/switchboard/proxy.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/settings.py` & `switchboard-1.6.4/switchboard/settings.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/signals.py` & `switchboard-1.6.4/switchboard/signals.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/template_helpers.py` & `switchboard-1.6.4/switchboard/template_helpers.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/tests/admin/test_utils.py` & `switchboard-1.6.4/switchboard/tests/admin/test_utils.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/tests/test_base.py` & `switchboard-1.6.4/switchboard/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/tests/test_builtins.py` & `switchboard-1.6.4/switchboard/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/tests/test_conditions.py` & `switchboard-1.6.4/switchboard/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/tests/test_decorators.py` & `switchboard-1.6.4/switchboard/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/tests/test_manager.py` & `switchboard-1.6.4/switchboard/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/tests/test_middleware.py` & `switchboard-1.6.4/switchboard/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/tests/test_models.py` & `switchboard-1.6.4/switchboard/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/tests/test_testutils.py` & `switchboard-1.6.4/switchboard/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard/testutils.py` & `switchboard-1.6.4/switchboard/testutils.py`

 * *Files identical despite different names*

### Comparing `switchboard-1.6.3/switchboard.egg-info/PKG-INFO` & `switchboard-1.6.4/switchboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchboard
-Version: 1.6.3
+Version: 1.6.4
 Summary: Feature flipper for Pyramid, Pylons, or TurboGears apps.
 Home-page: https://github.com/switchboardpy/switchboard/
 Download-URL: https://github.com/switchboardpy/switchboard/releases
 Author: Kyle Adams
 Author-email: kadams54@users.noreply.github.com
 License: Apache License
 Keywords: switches feature flipper pyramid pylons turbogears
```

### Comparing `switchboard-1.6.3/switchboard.egg-info/SOURCES.txt` & `switchboard-1.6.4/switchboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

