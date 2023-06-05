# Comparing `tmp/scopeton-2.4.tar.gz` & `tmp/scopeton-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scopeton-2.4.tar", last modified: Sun Jun  4 19:11:10 2023, max compression
+gzip compressed data, was "scopeton-2.5.tar", last modified: Mon Jun  5 08:12:02 2023, max compression
```

## Comparing `scopeton-2.4.tar` & `scopeton-2.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-04 19:11:10.741039 scopeton-2.4/
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1086 2023-04-16 07:04:25.000000 scopeton-2.4/LICENSE.txt
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      314 2023-06-04 19:11:10.741039 scopeton-2.4/PKG-INFO
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     2472 2023-04-16 07:49:04.000000 scopeton-2.4/README.md
-drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-04 19:11:10.741039 scopeton-2.4/scopeton/
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       38 2023-04-16 07:04:25.000000 scopeton-2.4/scopeton/__init__.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1068 2023-04-16 07:04:25.000000 scopeton-2.4/scopeton/compat.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       67 2023-06-04 18:13:09.000000 scopeton-2.4/scopeton/constants.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1113 2023-06-04 18:58:02.000000 scopeton-2.4/scopeton/decorators.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       46 2023-06-04 18:11:40.000000 scopeton-2.4/scopeton/glob.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1110 2023-04-16 07:04:25.000000 scopeton-2.4/scopeton/objects.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     3105 2023-04-16 07:04:25.000000 scopeton-2.4/scopeton/qualifier_tree.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     5008 2023-06-04 19:09:04.000000 scopeton-2.4/scopeton/scope.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1320 2023-04-16 07:04:25.000000 scopeton-2.4/scopeton/scopeTools.py
-drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-04 19:11:10.741039 scopeton-2.4/scopeton.egg-info/
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      314 2023-06-04 19:11:10.000000 scopeton-2.4/scopeton.egg-info/PKG-INFO
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      389 2023-06-04 19:11:10.000000 scopeton-2.4/scopeton.egg-info/SOURCES.txt
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        1 2023-06-04 19:11:10.000000 scopeton-2.4/scopeton.egg-info/dependency_links.txt
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        7 2023-06-04 19:11:10.000000 scopeton-2.4/scopeton.egg-info/requires.txt
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        9 2023-06-04 19:11:10.000000 scopeton-2.4/scopeton.egg-info/top_level.txt
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       79 2023-06-04 19:11:10.741039 scopeton-2.4/setup.cfg
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      500 2023-06-04 19:10:25.000000 scopeton-2.4/setup.py
+drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-05 08:12:02.534923 scopeton-2.5/
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1086 2023-04-16 07:04:25.000000 scopeton-2.5/LICENSE.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      314 2023-06-05 08:12:02.534923 scopeton-2.5/PKG-INFO
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     2472 2023-04-16 07:49:04.000000 scopeton-2.5/README.md
+drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-05 08:12:02.534923 scopeton-2.5/scopeton/
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       38 2023-04-16 07:04:25.000000 scopeton-2.5/scopeton/__init__.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1068 2023-04-16 07:04:25.000000 scopeton-2.5/scopeton/compat.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       67 2023-06-04 18:13:09.000000 scopeton-2.5/scopeton/constants.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1113 2023-06-04 18:58:02.000000 scopeton-2.5/scopeton/decorators.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       46 2023-06-04 18:11:40.000000 scopeton-2.5/scopeton/glob.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1110 2023-04-16 07:04:25.000000 scopeton-2.5/scopeton/objects.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     3105 2023-04-16 07:04:25.000000 scopeton-2.5/scopeton/qualifier_tree.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     5161 2023-06-05 08:01:03.000000 scopeton-2.5/scopeton/scope.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1320 2023-04-16 07:04:25.000000 scopeton-2.5/scopeton/scopeTools.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     4521 2023-06-05 08:10:52.000000 scopeton-2.5/scopeton/type_utils.py
+drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-05 08:12:02.534923 scopeton-2.5/scopeton.egg-info/
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      314 2023-06-05 08:12:02.000000 scopeton-2.5/scopeton.egg-info/PKG-INFO
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      412 2023-06-05 08:12:02.000000 scopeton-2.5/scopeton.egg-info/SOURCES.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        1 2023-06-05 08:12:02.000000 scopeton-2.5/scopeton.egg-info/dependency_links.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        7 2023-06-05 08:12:02.000000 scopeton-2.5/scopeton.egg-info/requires.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        9 2023-06-05 08:12:02.000000 scopeton-2.5/scopeton.egg-info/top_level.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       79 2023-06-05 08:12:02.534923 scopeton-2.5/setup.cfg
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      500 2023-06-05 08:11:11.000000 scopeton-2.5/setup.py
```

### Comparing `scopeton-2.4/LICENSE.txt` & `scopeton-2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scopeton-2.4/README.md` & `scopeton-2.5/README.md`

 * *Files identical despite different names*

### Comparing `scopeton-2.4/scopeton/compat.py` & `scopeton-2.5/scopeton/compat.py`

 * *Files identical despite different names*

### Comparing `scopeton-2.4/scopeton/decorators.py` & `scopeton-2.5/scopeton/decorators.py`

 * *Files identical despite different names*

### Comparing `scopeton-2.4/scopeton/objects.py` & `scopeton-2.5/scopeton/objects.py`

 * *Files identical despite different names*

### Comparing `scopeton-2.4/scopeton/qualifier_tree.py` & `scopeton-2.5/scopeton/qualifier_tree.py`

 * *Files identical despite different names*

### Comparing `scopeton-2.4/scopeton/scope.py` & `scopeton-2.5/scopeton/scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from threading import RLock
 
 import typing
 
-from scopeton import compat, glob, constants
+from scopeton import compat, glob, constants, type_utils
 from scopeton.objects import Bean
 from scopeton.qualifier_tree import QualifierTree
 from scopeton.scopeTools import getBean_qualifier, callMethodByName, getClassTree, flatten, ScopetonException
 
 T = typing.TypeVar("T")
 
 
@@ -24,14 +24,17 @@
         self.servicesStarted = False
         self.children = []  # type: typing.List[Scope]
         self.registerInstance(self.__class__, self)
         if parent:
             parent.children.append(self)
 
     def getInstance(self, name: typing.Type[T]) -> T:
+        if type_utils._is_collection(name):
+            args = type_utils._get_type_args(name)
+            return self.getInstances(args[0])
         with self.lock:
             return self._getInstance(getBean_qualifier(name))
 
     def getInstances(self, qualifier: typing.Type[T]) -> typing.List[T]:
         with self.lock:
             beans = self._beans.find_by_qualifier_name(getBean_qualifier(qualifier))
             beans = map(lambda x: self.getInstance(x), beans)
```

### Comparing `scopeton-2.4/scopeton/scopeTools.py` & `scopeton-2.5/scopeton/scopeTools.py`

 * *Files identical despite different names*

