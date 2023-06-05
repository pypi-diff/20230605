# Comparing `tmp/hello50-1.1.9.tar.gz` & `tmp/hello50-1.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello50-1.1.9.tar", last modified: Mon Jun  5 17:15:04 2023, max compression
+gzip compressed data, was "hello50-1.1.90.tar", last modified: Mon Jun  5 17:24:20 2023, max compression
```

## Comparing `hello50-1.1.9.tar` & `hello50-1.1.90.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:15:04.010384 hello50-1.1.9/
--rw-rw-rw-   0        0        0      512 2023-06-05 17:15:04.010384 hello50-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-06-04 21:31:36.000000 hello50-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 17:15:03.994384 hello50-1.1.9/hello/
--rw-rw-rw-   0        0        0       66 2023-06-05 16:22:12.000000 hello50-1.1.9/hello/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:15:04.006383 hello50-1.1.9/hello/db/
--rw-rw-rw-   0        0        0  1808440 2023-05-11 11:20:27.000000 hello50-1.1.9/hello/db/quran_simple.json
--rw-rw-rw-   0        0        0      285 2023-06-05 17:10:56.000000 hello50-1.1.9/hello/index.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:15:04.005384 hello50-1.1.9/hello50.egg-info/
--rw-rw-rw-   0        0        0      512 2023-06-05 17:15:03.000000 hello50-1.1.9/hello50.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-06-05 17:15:03.000000 hello50-1.1.9/hello50.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:15:03.000000 hello50-1.1.9/hello50.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 17:15:03.000000 hello50-1.1.9/hello50.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 17:15:03.000000 hello50-1.1.9/hello50.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 17:15:04.010384 hello50-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-06-05 17:14:52.000000 hello50-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:24:20.054276 hello50-1.1.90/
+-rw-rw-rw-   0        0        0      515 2023-06-05 17:24:20.029277 hello50-1.1.90/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-06-04 21:31:36.000000 hello50-1.1.90/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 17:24:20.013277 hello50-1.1.90/hello/
+-rw-rw-rw-   0        0        0       95 2023-06-05 17:23:17.000000 hello50-1.1.90/hello/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:24:20.026277 hello50-1.1.90/hello/db/
+-rw-rw-rw-   0        0        0  1808440 2023-05-11 11:20:27.000000 hello50-1.1.90/hello/db/quran_simple.json
+-rw-rw-rw-   0        0        0      392 2023-06-05 17:23:09.000000 hello50-1.1.90/hello/index.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:24:20.025277 hello50-1.1.90/hello50.egg-info/
+-rw-rw-rw-   0        0        0      515 2023-06-05 17:24:19.000000 hello50-1.1.90/hello50.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-06-05 17:24:19.000000 hello50-1.1.90/hello50.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 17:24:19.000000 hello50-1.1.90/hello50.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 17:24:19.000000 hello50-1.1.90/hello50.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 17:24:19.000000 hello50-1.1.90/hello50.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 17:24:20.054276 hello50-1.1.90/setup.cfg
+-rw-rw-rw-   0        0        0     1109 2023-06-05 17:24:08.000000 hello50-1.1.90/setup.py
```

### Comparing `hello50-1.1.9/PKG-INFO` & `hello50-1.1.90/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hello50
-Version: 1.1.9
-Summary: Hello world shit!!!!
+Version: 1.1.90
+Summary: Hello world 000000!!!!
 Author: Malik
 Author-email: myemail46926213@gmail.com
 Keywords: python,hello
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `hello50-1.1.9/hello/db/quran_simple.json` & `hello50-1.1.90/hello/db/quran_simple.json`

 * *Files identical despite different names*

### Comparing `hello50-1.1.9/hello50.egg-info/PKG-INFO` & `hello50-1.1.90/hello50.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hello50
-Version: 1.1.9
-Summary: Hello world shit!!!!
+Version: 1.1.90
+Summary: Hello world 000000!!!!
 Author: Malik
 Author-email: myemail46926213@gmail.com
 Keywords: python,hello
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `hello50-1.1.9/setup.py` & `hello50-1.1.90/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os, glob
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.9'
-DESCRIPTION = 'Hello world shit!!!!'
+VERSION = '1.1.90'
+DESCRIPTION = 'Hello world 000000!!!!'
 LONG_DESCRIPTION = 'Hello world 3~~~~~'
 
 # Setting up
 setup(
     name="hello50",
     version=VERSION,
     author="Malik",
```

