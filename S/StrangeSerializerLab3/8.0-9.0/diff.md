# Comparing `tmp/StrangeSerializerLab3-8.0.tar.gz` & `tmp/StrangeSerializerLab3-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StrangeSerializerLab3-8.0.tar", last modified: Thu Jun  1 10:33:04 2023, max compression
+gzip compressed data, was "StrangeSerializerLab3-9.0.tar", last modified: Thu Jun  1 10:34:53 2023, max compression
```

## Comparing `StrangeSerializerLab3-8.0.tar` & `StrangeSerializerLab3-9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:33:04.486120 StrangeSerializerLab3-8.0/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:33:04.482120 StrangeSerializerLab3-8.0/PKG-INFO
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:33:04.478120 StrangeSerializerLab3-8.0/StrangeSerializerLab3/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)     7080 2023-06-01 07:24:02.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3/AdditionalFunctions.py
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      415 2023-06-01 10:30:38.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3/StrangeFactory.py
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:33:04.482120 StrangeSerializerLab3-8.0/StrangeSerializerLab3/StrangeJSON/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      588 2023-06-01 09:39:28.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3/StrangeJSON/StrangeJsonSerializer.py
--rw-rw-r--   0 mihail    (1000) mihail    (1000)     1442 2023-06-01 08:44:19.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3/StrangeJSON/parser.py
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:33:04.482120 StrangeSerializerLab3-8.0/StrangeSerializerLab3/StrangeXML/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      600 2023-06-01 09:39:28.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3/StrangeXML/StrangeXmlSerializer.py
--rw-rw-r--   0 mihail    (1000) mihail    (1000)     3114 2023-06-01 08:46:03.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3/StrangeXML/parser.py
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      300 2023-06-01 10:32:56.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3/__init__.py
-drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:33:04.482120 StrangeSerializerLab3-8.0/StrangeSerializerLab3.egg-info/
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:33:04.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3.egg-info/PKG-INFO
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      510 2023-06-01 10:33:04.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3.egg-info/SOURCES.txt
--rw-rw-r--   0 mihail    (1000) mihail    (1000)        1 2023-06-01 10:33:04.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3.egg-info/dependency_links.txt
--rw-rw-r--   0 mihail    (1000) mihail    (1000)       89 2023-06-01 10:33:04.000000 StrangeSerializerLab3-8.0/StrangeSerializerLab3.egg-info/top_level.txt
--rw-rw-r--   0 mihail    (1000) mihail    (1000)       38 2023-06-01 10:33:04.486120 StrangeSerializerLab3-8.0/setup.cfg
--rw-rw-r--   0 mihail    (1000) mihail    (1000)      486 2023-06-01 10:33:01.000000 StrangeSerializerLab3-8.0/setup.py
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:34:53.661159 StrangeSerializerLab3-9.0/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:34:53.661159 StrangeSerializerLab3-9.0/PKG-INFO
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:34:53.657158 StrangeSerializerLab3-9.0/StrangeSerializerLab3/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)     7080 2023-06-01 07:24:02.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3/AdditionalFunctions.py
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      415 2023-06-01 10:30:38.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3/StrangeFactory.py
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:34:53.657158 StrangeSerializerLab3-9.0/StrangeSerializerLab3/StrangeJSON/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      622 2023-06-01 10:34:49.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3/StrangeJSON/StrangeJsonSerializer.py
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)     1442 2023-06-01 08:44:19.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3/StrangeJSON/parser.py
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:34:53.657158 StrangeSerializerLab3-9.0/StrangeSerializerLab3/StrangeXML/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      633 2023-06-01 10:34:49.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3/StrangeXML/StrangeXmlSerializer.py
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)     3114 2023-06-01 08:46:03.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3/StrangeXML/parser.py
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      300 2023-06-01 10:32:56.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3/__init__.py
+drwxrwxr-x   0 mihail    (1000) mihail    (1000)        0 2023-06-01 10:34:53.657158 StrangeSerializerLab3-9.0/StrangeSerializerLab3.egg-info/
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      261 2023-06-01 10:34:53.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3.egg-info/PKG-INFO
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      510 2023-06-01 10:34:53.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)        1 2023-06-01 10:34:53.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)       89 2023-06-01 10:34:53.000000 StrangeSerializerLab3-9.0/StrangeSerializerLab3.egg-info/top_level.txt
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)       38 2023-06-01 10:34:53.661159 StrangeSerializerLab3-9.0/setup.cfg
+-rw-rw-r--   0 mihail    (1000) mihail    (1000)      486 2023-06-01 10:34:49.000000 StrangeSerializerLab3-9.0/setup.py
```

### Comparing `StrangeSerializerLab3-8.0/StrangeSerializerLab3/AdditionalFunctions.py` & `StrangeSerializerLab3-9.0/StrangeSerializerLab3/AdditionalFunctions.py`

 * *Files identical despite different names*

### Comparing `StrangeSerializerLab3-8.0/StrangeSerializerLab3/StrangeJSON/parser.py` & `StrangeSerializerLab3-9.0/StrangeSerializerLab3/StrangeJSON/parser.py`

 * *Files identical despite different names*

### Comparing `StrangeSerializerLab3-8.0/StrangeSerializerLab3/StrangeXML/StrangeXmlSerializer.py` & `StrangeSerializerLab3-9.0/StrangeSerializerLab3/StrangeXML/StrangeXmlSerializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from StrangeSerializerLab3.AdditionalFunctions import serialize, deserialize
-from parser import dumps_from_dict
+from StrangeSerializerLab3.StrangeXML.parser import dumps_from_dict
 
 
 class StrangeXmlSerializer:
     @staticmethod
     def dump(obj, file_name):
         with open(file_name, 'w') as file:
             file.write(StrangeXmlSerializer.dumps(obj))
```

### Comparing `StrangeSerializerLab3-8.0/StrangeSerializerLab3/StrangeXML/parser.py` & `StrangeSerializerLab3-9.0/StrangeSerializerLab3/StrangeXML/parser.py`

 * *Files identical despite different names*

