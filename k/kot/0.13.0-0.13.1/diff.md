# Comparing `tmp/kot-0.13.0.tar.gz` & `tmp/kot-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kot-0.13.0.tar", last modified: Mon Jun  5 17:35:14 2023, max compression
+gzip compressed data, was "kot-0.13.1.tar", last modified: Mon Jun  5 17:37:59 2023, max compression
```

## Comparing `kot-0.13.0.tar` & `kot-0.13.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:35:14.208277 kot-0.13.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-05 17:35:04.000000 kot-0.13.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-05 17:35:14.208277 kot-0.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-05 17:35:04.000000 kot-0.13.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:35:14.208277 kot-0.13.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-05 17:35:04.000000 kot-0.13.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:35:14.204277 kot-0.13.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:35:14.204277 kot-0.13.0/src/kot/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 17:35:04.000000 kot-0.13.0/src/kot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-06-05 17:35:04.000000 kot-0.13.0/src/kot/kot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:35:14.208277 kot-0.13.0/src/kot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-05 17:35:14.000000 kot-0.13.0/src/kot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-05 17:35:14.000000 kot-0.13.0/src/kot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:35:14.000000 kot-0.13.0/src/kot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:35:14.000000 kot-0.13.0/src/kot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:35:14.000000 kot-0.13.0/src/kot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 17:35:14.000000 kot-0.13.0/src/kot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 17:35:14.000000 kot-0.13.0/src/kot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:37:59.235211 kot-0.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-05 17:37:48.000000 kot-0.13.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-05 17:37:59.231211 kot-0.13.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-05 17:37:48.000000 kot-0.13.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:37:59.235211 kot-0.13.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-05 17:37:48.000000 kot-0.13.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:37:59.231211 kot-0.13.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:37:59.231211 kot-0.13.1/src/kot/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 17:37:48.000000 kot-0.13.1/src/kot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-06-05 17:37:48.000000 kot-0.13.1/src/kot/kot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:37:59.231211 kot-0.13.1/src/kot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-05 17:37:58.000000 kot-0.13.1/src/kot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-05 17:37:59.000000 kot-0.13.1/src/kot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:37:58.000000 kot-0.13.1/src/kot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:37:58.000000 kot-0.13.1/src/kot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:37:58.000000 kot-0.13.1/src/kot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 17:37:58.000000 kot-0.13.1/src/kot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 17:37:58.000000 kot-0.13.1/src/kot.egg-info/top_level.txt
```

### Comparing `kot-0.13.0/LICENSE` & `kot-0.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kot-0.13.0/PKG-INFO` & `kot-0.13.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.13.0
+Version: 0.13.1
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

### Comparing `kot-0.13.0/README.md` & `kot-0.13.1/README.md`

 * *Files identical despite different names*

### Comparing `kot-0.13.0/setup.py` & `kot-0.13.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='kot',
-version='0.13.0',
+version='0.13.1',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KOT',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `kot-0.13.0/src/kot/kot.py` & `kot-0.13.1/src/kot/kot.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,16 +136,16 @@
         except OSError:
             if not os.path.isdir(self.location):
                 raise
 
     def clear_cache(self):
         self.cache = {}
         for each_file in self.open_files_db.dict():
-            print(each_file)
-            os.remove(each_file)
+            if os.path.exists(each_file):
+                os.remove(each_file)
         self.open_files_db.delete_all()
 
 
 
     def encrypt(self, key, message):
         #Serializing the message
         message = pickle.dumps(message)
```

### Comparing `kot-0.13.0/src/kot.egg-info/PKG-INFO` & `kot-0.13.1/src/kot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.13.0
+Version: 0.13.1
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

