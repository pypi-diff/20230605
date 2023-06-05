# Comparing `tmp/aspectify-0.0.4.tar.gz` & `tmp/aspectify-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspectify-0.0.4.tar", last modified: Fri Jun  2 10:53:04 2023, max compression
+gzip compressed data, was "aspectify-1.0.0.tar", last modified: Mon Jun  5 07:56:29 2023, max compression
```

## Comparing `aspectify-0.0.4.tar` & `aspectify-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 10:53:04.636672 aspectify-0.0.4/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-05-29 07:08:03.000000 aspectify-0.0.4/LICENSE
--rw-rw-r--   0 ruescog   (1008) ruescog   (1011)      111 2023-04-27 10:12:58.000000 aspectify-0.0.4/MANIFEST.in
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     4618 2023-06-02 10:53:04.632672 aspectify-0.0.4/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     3109 2023-06-02 10:13:26.000000 aspectify-0.0.4/README.md
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 10:53:04.632672 aspectify-0.0.4/aspectify/
--rw-r--r--   0 ruescog   (1008) ruescog   (1011)       22 2023-06-02 10:53:01.000000 aspectify-0.0.4/aspectify/__init__.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     1537 2023-06-02 10:53:01.000000 aspectify-0.0.4/aspectify/_modidx.py
--rw-r--r--   0 ruescog   (1008) ruescog   (1011)     5884 2023-06-02 10:53:01.000000 aspectify-0.0.4/aspectify/aop.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      142 2023-05-29 07:42:30.000000 aspectify-0.0.4/aspectify/core.py
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 10:53:04.632672 aspectify-0.0.4/aspectify.egg-info/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     4618 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      361 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/SOURCES.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/dependency_links.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       61 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/entry_points.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-05-29 07:48:24.000000 aspectify-0.0.4/aspectify.egg-info/not-zip-safe
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        7 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/requires.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       10 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/top_level.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      802 2023-06-02 07:38:05.000000 aspectify-0.0.4/settings.ini
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-06-02 10:53:04.636672 aspectify-0.0.4/setup.cfg
--rw-rw-r--   0 ruescog   (1008) ruescog   (1011)     2596 2023-04-27 10:12:58.000000 aspectify-0.0.4/setup.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-05 07:56:29.705858 aspectify-1.0.0/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-05-29 07:08:03.000000 aspectify-1.0.0/LICENSE
+-rw-rw-r--   0 ruescog   (1008) ruescog   (1011)      111 2023-04-27 10:12:58.000000 aspectify-1.0.0/MANIFEST.in
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     4618 2023-06-05 07:56:29.705858 aspectify-1.0.0/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     3109 2023-06-05 07:00:10.000000 aspectify-1.0.0/README.md
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-05 07:56:29.705858 aspectify-1.0.0/aspectify/
+-rw-r--r--   0 ruescog   (1008) ruescog   (1011)       22 2023-06-05 07:55:09.000000 aspectify-1.0.0/aspectify/__init__.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     1520 2023-06-05 07:55:12.000000 aspectify-1.0.0/aspectify/_modidx.py
+-rw-r--r--   0 ruescog   (1008) ruescog   (1011)     5884 2023-06-05 07:55:09.000000 aspectify-1.0.0/aspectify/aop.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      181 2023-06-05 07:55:09.000000 aspectify-1.0.0/aspectify/examples.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      177 2023-06-05 07:22:34.000000 aspectify-1.0.0/aspectify/examples2.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-05 07:56:29.705858 aspectify-1.0.0/aspectify.egg-info/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     4618 2023-06-05 07:56:29.000000 aspectify-1.0.0/aspectify.egg-info/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      388 2023-06-05 07:56:29.000000 aspectify-1.0.0/aspectify.egg-info/SOURCES.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-06-05 07:56:29.000000 aspectify-1.0.0/aspectify.egg-info/dependency_links.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       61 2023-06-05 07:56:29.000000 aspectify-1.0.0/aspectify.egg-info/entry_points.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-05-29 07:48:24.000000 aspectify-1.0.0/aspectify.egg-info/not-zip-safe
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        7 2023-06-05 07:56:29.000000 aspectify-1.0.0/aspectify.egg-info/requires.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       10 2023-06-05 07:56:29.000000 aspectify-1.0.0/aspectify.egg-info/top_level.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      802 2023-06-05 07:55:56.000000 aspectify-1.0.0/settings.ini
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-06-05 07:56:29.705858 aspectify-1.0.0/setup.cfg
+-rw-rw-r--   0 ruescog   (1008) ruescog   (1011)     2596 2023-04-27 10:12:58.000000 aspectify-1.0.0/setup.py
```

### Comparing `aspectify-0.0.4/LICENSE` & `aspectify-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aspectify-0.0.4/PKG-INFO` & `aspectify-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspectify
-Version: 0.0.4
+Version: 1.0.0
 Summary: Apply Aspect Oriented Programming to your Python code
 Home-page: https://github.com/ruescog/aspectify
 Author: ruescog
 Author-email: ruescog@unirioja.es
 License: Apache Software License 2.0
 Description: aspectify
         ================
```

### Comparing `aspectify-0.0.4/README.md` & `aspectify-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aspectify-0.0.4/aspectify/_modidx.py` & `aspectify-1.0.0/aspectify/_modidx.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,8 +11,9 @@
                                'aspectify.aop.Aspect.set_after': ('aop.html#aspect.set_after', 'aspectify/aop.py'),
                                'aspectify.aop.Aspect.set_after_returning': ('aop.html#aspect.set_after_returning', 'aspectify/aop.py'),
                                'aspectify.aop.Aspect.set_after_throwing': ('aop.html#aspect.set_after_throwing', 'aspectify/aop.py'),
                                'aspectify.aop.Aspect.set_around': ('aop.html#aspect.set_around', 'aspectify/aop.py'),
                                'aspectify.aop.Aspect.set_before': ('aop.html#aspect.set_before', 'aspectify/aop.py'),
                                'aspectify.aop.advice': ('aop.html#advice', 'aspectify/aop.py'),
                                'aspectify.aop.is_detectable': ('aop.html#is_detectable', 'aspectify/aop.py')},
-            'aspectify.core': {'aspectify.core.foo': ('core.html#foo', 'aspectify/core.py')}}}
+            'aspectify.examples': {},
+            'aspectify.examples2': {}}}
```

### Comparing `aspectify-0.0.4/aspectify/aop.py` & `aspectify-1.0.0/aspectify/aop.py`

 * *Files identical despite different names*

### Comparing `aspectify-0.0.4/aspectify.egg-info/PKG-INFO` & `aspectify-1.0.0/aspectify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspectify
-Version: 0.0.4
+Version: 1.0.0
 Summary: Apply Aspect Oriented Programming to your Python code
 Home-page: https://github.com/ruescog/aspectify
 Author: ruescog
 Author-email: ruescog@unirioja.es
 License: Apache Software License 2.0
 Description: aspectify
         ================
```

### Comparing `aspectify-0.0.4/settings.ini` & `aspectify-1.0.0/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = aspectify
 lib_name = aspectify
-version = 0.0.4
+version = 1.0.0
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = aspectify
 nbs_path = nbs
 recursive = True
```

### Comparing `aspectify-0.0.4/setup.py` & `aspectify-1.0.0/setup.py`

 * *Files identical despite different names*

