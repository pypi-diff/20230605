# Comparing `tmp/tagging_module-0.0.7.tar.gz` & `tmp/tagging_module-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagging_module-0.0.7.tar", last modified: Fri May 26 11:45:37 2023, max compression
+gzip compressed data, was "tagging_module-0.0.8.tar", last modified: Mon Jun  5 15:07:04 2023, max compression
```

## Comparing `tagging_module-0.0.7.tar` & `tagging_module-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 11:45:37.863945 tagging_module-0.0.7/
--rw-rw-rw-   0        0        0       61 2023-05-26 11:32:18.000000 tagging_module-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2082 2023-05-26 11:45:37.862949 tagging_module-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-05-26 11:21:14.000000 tagging_module-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 11:45:37.863945 tagging_module-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-05-26 11:45:20.000000 tagging_module-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:45:37.852937 tagging_module-0.0.7/tagging_module/
--rw-rw-rw-   0        0        0        0 2023-05-21 13:22:58.000000 tagging_module-0.0.7/tagging_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:45:37.861947 tagging_module-0.0.7/tagging_module/config/
--rw-rw-rw-   0        0        0     4001 2023-05-21 13:22:58.000000 tagging_module-0.0.7/tagging_module/config/rules.yml
--rw-rw-rw-   0        0        0      783 2023-05-26 08:25:07.000000 tagging_module-0.0.7/tagging_module/tagging_service.py
--rw-rw-rw-   0        0        0     1394 2023-05-21 13:22:58.000000 tagging_module-0.0.7/tagging_module/tagging_system.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:45:37.860952 tagging_module-0.0.7/tagging_module.egg-info/
--rw-rw-rw-   0        0        0     2082 2023-05-26 11:45:37.000000 tagging_module-0.0.7/tagging_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-05-26 11:45:37.000000 tagging_module-0.0.7/tagging_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 11:45:37.000000 tagging_module-0.0.7/tagging_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 11:45:37.000000 tagging_module-0.0.7/tagging_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-26 11:45:37.000000 tagging_module-0.0.7/tagging_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 15:07:04.417549 tagging_module-0.0.8/
+-rw-rw-rw-   0        0        0       61 2023-05-26 11:32:18.000000 tagging_module-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2082 2023-06-05 15:07:04.416549 tagging_module-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-05-26 11:21:14.000000 tagging_module-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:07:04.417549 tagging_module-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-06-05 15:04:29.000000 tagging_module-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:07:04.357987 tagging_module-0.0.8/tagging_module/
+-rw-rw-rw-   0        0        0        0 2023-05-21 13:22:58.000000 tagging_module-0.0.8/tagging_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:07:04.414549 tagging_module-0.0.8/tagging_module/config/
+-rw-rw-rw-   0        0        0     6366 2023-06-05 14:13:55.000000 tagging_module-0.0.8/tagging_module/config/rules.yml
+-rw-rw-rw-   0        0        0      783 2023-05-26 08:25:07.000000 tagging_module-0.0.8/tagging_module/tagging_service.py
+-rw-rw-rw-   0        0        0     1394 2023-06-05 13:59:50.000000 tagging_module-0.0.8/tagging_module/tagging_system.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:07:04.413553 tagging_module-0.0.8/tagging_module.egg-info/
+-rw-rw-rw-   0        0        0     2082 2023-06-05 15:07:04.000000 tagging_module-0.0.8/tagging_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-06-05 15:07:04.000000 tagging_module-0.0.8/tagging_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:07:04.000000 tagging_module-0.0.8/tagging_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 15:07:04.000000 tagging_module-0.0.8/tagging_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-05 15:07:04.000000 tagging_module-0.0.8/tagging_module.egg-info/top_level.txt
```

### Comparing `tagging_module-0.0.7/PKG-INFO` & `tagging_module-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagging_module
-Version: 0.0.7
+Version: 0.0.8
 Summary: A lightweight rule based tech content tagging module for Python
 Author: aditya-xq
 Author-email: adityavivek.xq@gmail.com
 Description-Content-Type: text/markdown
 
 # Tagging Module
 A lightweight rule based tech content tagging module for Python
```

### Comparing `tagging_module-0.0.7/README.md` & `tagging_module-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tagging_module-0.0.7/setup.py` & `tagging_module-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tagging_module',
-    version='0.0.7',
+    version='0.0.8',
     author='aditya-xq',
     author_email='adityavivek.xq@gmail.com',
     description='A lightweight rule based tech content tagging module for Python',
     packages=['tagging_module', 'tagging_module.config'],
     package_data={
         'tagging_module': ['config/rules.yml'],
     },
```

### Comparing `tagging_module-0.0.7/tagging_module/tagging_service.py` & `tagging_module-0.0.8/tagging_module/tagging_service.py`

 * *Files identical despite different names*

### Comparing `tagging_module-0.0.7/tagging_module/tagging_system.py` & `tagging_module-0.0.8/tagging_module/tagging_system.py`

 * *Files identical despite different names*

### Comparing `tagging_module-0.0.7/tagging_module.egg-info/PKG-INFO` & `tagging_module-0.0.8/tagging_module.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagging-module
-Version: 0.0.7
+Version: 0.0.8
 Summary: A lightweight rule based tech content tagging module for Python
 Author: aditya-xq
 Author-email: adityavivek.xq@gmail.com
 Description-Content-Type: text/markdown
 
 # Tagging Module
 A lightweight rule based tech content tagging module for Python
```

