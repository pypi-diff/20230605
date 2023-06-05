# Comparing `tmp/hello50-1.0.5.tar.gz` & `tmp/hello50-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello50-1.0.5.tar", last modified: Mon Jun  5 16:22:43 2023, max compression
+gzip compressed data, was "hello50-1.1.0.tar", last modified: Mon Jun  5 16:29:48 2023, max compression
```

## Comparing `hello50-1.0.5.tar` & `hello50-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:22:43.932964 hello50-1.0.5/
--rw-rw-rw-   0        0        0      512 2023-06-05 16:22:43.931964 hello50-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-06-04 21:31:36.000000 hello50-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 16:22:43.911991 hello50-1.0.5/hello/
--rw-rw-rw-   0        0        0       66 2023-06-05 16:22:12.000000 hello50-1.0.5/hello/__init__.py
--rw-rw-rw-   0        0        0      180 2023-06-05 16:22:19.000000 hello50-1.0.5/hello/index.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:22:43.930964 hello50-1.0.5/hello50.egg-info/
--rw-rw-rw-   0        0        0      512 2023-06-05 16:22:43.000000 hello50-1.0.5/hello50.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-06-05 16:22:43.000000 hello50-1.0.5/hello50.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:22:43.000000 hello50-1.0.5/hello50.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 16:22:43.000000 hello50-1.0.5/hello50.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 16:22:43.000000 hello50-1.0.5/hello50.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 16:22:43.932964 hello50-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-06-05 16:22:34.000000 hello50-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:29:48.346017 hello50-1.1.0/
+-rw-rw-rw-   0        0        0      512 2023-06-05 16:29:48.273140 hello50-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-06-04 21:31:36.000000 hello50-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 16:29:48.251138 hello50-1.1.0/hello/
+-rw-rw-rw-   0        0        0       66 2023-06-05 16:22:12.000000 hello50-1.1.0/hello/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:29:48.270139 hello50-1.1.0/hello/db/
+-rw-rw-rw-   0        0        0  1808440 2023-05-11 11:20:27.000000 hello50-1.1.0/hello/db/quran_simple.json
+-rw-rw-rw-   0        0        0      266 2023-06-05 16:28:56.000000 hello50-1.1.0/hello/index.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:29:48.269137 hello50-1.1.0/hello50.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-06-05 16:29:47.000000 hello50-1.1.0/hello50.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-06-05 16:29:48.000000 hello50-1.1.0/hello50.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:29:47.000000 hello50-1.1.0/hello50.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 16:29:47.000000 hello50-1.1.0/hello50.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 16:29:47.000000 hello50-1.1.0/hello50.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:29:48.346017 hello50-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-06-05 16:29:33.000000 hello50-1.1.0/setup.py
```

### Comparing `hello50-1.0.5/PKG-INFO` & `hello50-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello50
-Version: 1.0.5
+Version: 1.1.0
 Summary: Hello world shit!!!!
 Author: Malik
 Author-email: myemail46926213@gmail.com
 Keywords: python,hello
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hello50-1.0.5/hello50.egg-info/PKG-INFO` & `hello50-1.1.0/hello50.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello50
-Version: 1.0.5
+Version: 1.1.0
 Summary: Hello world shit!!!!
 Author: Malik
 Author-email: myemail46926213@gmail.com
 Keywords: python,hello
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hello50-1.0.5/setup.py` & `hello50-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 import codecs
-import os
+import os, glob
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.5'
+VERSION = '1.1.0'
 DESCRIPTION = 'Hello world shit!!!!'
 LONG_DESCRIPTION = 'Hello world 3~~~~~'
 
 # Setting up
 setup(
     name="hello50",
     version=VERSION,
@@ -26,15 +26,16 @@
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-    ]
+    ],
+    data_files=glob.glob('hello/db/**')
 )
 
 
 """
 python setup.py sdist
 twine upload dist/*
```

