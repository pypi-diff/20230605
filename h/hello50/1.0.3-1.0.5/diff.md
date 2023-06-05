# Comparing `tmp/hello50-1.0.3.tar.gz` & `tmp/hello50-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello50-1.0.3.tar", last modified: Mon Jun  5 16:00:28 2023, max compression
+gzip compressed data, was "hello50-1.0.5.tar", last modified: Mon Jun  5 16:22:43 2023, max compression
```

## Comparing `hello50-1.0.3.tar` & `hello50-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:00:28.764629 hello50-1.0.3/
--rw-rw-rw-   0        0        0      512 2023-06-05 16:00:28.763485 hello50-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-06-04 21:31:36.000000 hello50-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 16:00:28.746516 hello50-1.0.3/hello/
--rw-rw-rw-   0        0        0       49 2023-06-05 15:59:35.000000 hello50-1.0.3/hello/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-04 21:28:42.000000 hello50-1.0.3/hello/index.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:00:28.762485 hello50-1.0.3/hello50.egg-info/
--rw-rw-rw-   0        0        0      512 2023-06-05 16:00:27.000000 hello50-1.0.3/hello50.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-06-05 16:00:27.000000 hello50-1.0.3/hello50.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:00:27.000000 hello50-1.0.3/hello50.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 16:00:27.000000 hello50-1.0.3/hello50.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 16:00:27.000000 hello50-1.0.3/hello50.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 16:00:28.764629 hello50-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1041 2023-06-05 16:00:13.000000 hello50-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:22:43.932964 hello50-1.0.5/
+-rw-rw-rw-   0        0        0      512 2023-06-05 16:22:43.931964 hello50-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-06-04 21:31:36.000000 hello50-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 16:22:43.911991 hello50-1.0.5/hello/
+-rw-rw-rw-   0        0        0       66 2023-06-05 16:22:12.000000 hello50-1.0.5/hello/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-06-05 16:22:19.000000 hello50-1.0.5/hello/index.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:22:43.930964 hello50-1.0.5/hello50.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-06-05 16:22:43.000000 hello50-1.0.5/hello50.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-06-05 16:22:43.000000 hello50-1.0.5/hello50.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:22:43.000000 hello50-1.0.5/hello50.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 16:22:43.000000 hello50-1.0.5/hello50.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 16:22:43.000000 hello50-1.0.5/hello50.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:22:43.932964 hello50-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-06-05 16:22:34.000000 hello50-1.0.5/setup.py
```

### Comparing `hello50-1.0.3/PKG-INFO` & `hello50-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello50
-Version: 1.0.3
+Version: 1.0.5
 Summary: Hello world shit!!!!
 Author: Malik
 Author-email: myemail46926213@gmail.com
 Keywords: python,hello
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hello50-1.0.3/hello50.egg-info/PKG-INFO` & `hello50-1.0.5/hello50.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello50
-Version: 1.0.3
+Version: 1.0.5
 Summary: Hello world shit!!!!
 Author: Malik
 Author-email: myemail46926213@gmail.com
 Keywords: python,hello
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hello50-1.0.3/setup.py` & `hello50-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.3'
+VERSION = '1.0.5'
 DESCRIPTION = 'Hello world shit!!!!'
 LONG_DESCRIPTION = 'Hello world 3~~~~~'
 
 # Setting up
 setup(
     name="hello50",
     version=VERSION,
@@ -31,10 +31,11 @@
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
 
 
 """
+python setup.py sdist
 twine upload dist/*
 
 """
```

