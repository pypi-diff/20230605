# Comparing `tmp/hello50-1.0.2.tar.gz` & `tmp/hello50-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello50-1.0.2.tar", last modified: Sun Jun  4 21:42:56 2023, max compression
+gzip compressed data, was "hello50-1.0.3.tar", last modified: Mon Jun  5 16:00:28 2023, max compression
```

## Comparing `hello50-1.0.2.tar` & `hello50-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 21:42:56.400070 hello50-1.0.2/
--rw-rw-rw-   0        0        0      514 2023-06-04 21:42:56.396071 hello50-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-06-04 21:31:36.000000 hello50-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 21:42:56.255256 hello50-1.0.2/hello/
--rw-rw-rw-   0        0        0       43 2023-06-04 21:37:05.000000 hello50-1.0.2/hello/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-04 21:28:42.000000 hello50-1.0.2/hello/index.py
-drwxrwxrwx   0        0        0        0 2023-06-04 21:42:56.390034 hello50-1.0.2/hello50.egg-info/
--rw-rw-rw-   0        0        0      514 2023-06-04 21:42:55.000000 hello50-1.0.2/hello50.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-06-04 21:42:56.000000 hello50-1.0.2/hello50.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 21:42:55.000000 hello50-1.0.2/hello50.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 21:42:55.000000 hello50-1.0.2/hello50.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 21:42:55.000000 hello50-1.0.2/hello50.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 21:42:56.400070 hello50-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1006 2023-06-04 21:41:48.000000 hello50-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:00:28.764629 hello50-1.0.3/
+-rw-rw-rw-   0        0        0      512 2023-06-05 16:00:28.763485 hello50-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-06-04 21:31:36.000000 hello50-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 16:00:28.746516 hello50-1.0.3/hello/
+-rw-rw-rw-   0        0        0       49 2023-06-05 15:59:35.000000 hello50-1.0.3/hello/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-04 21:28:42.000000 hello50-1.0.3/hello/index.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:00:28.762485 hello50-1.0.3/hello50.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-06-05 16:00:27.000000 hello50-1.0.3/hello50.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-06-05 16:00:27.000000 hello50-1.0.3/hello50.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:00:27.000000 hello50-1.0.3/hello50.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 16:00:27.000000 hello50-1.0.3/hello50.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 16:00:27.000000 hello50-1.0.3/hello50.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:00:28.764629 hello50-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2023-06-05 16:00:13.000000 hello50-1.0.3/setup.py
```

### Comparing `hello50-1.0.2/PKG-INFO` & `hello50-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hello50
-Version: 1.0.2
+Version: 1.0.3
 Summary: Hello world shit!!!!
 Author: Malik
 Author-email: myemail46926213@gmail.com
 Keywords: python,hello
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
-Hello world 000~~~~~
+Hello world 3~~~~~
```

### Comparing `hello50-1.0.2/hello50.egg-info/PKG-INFO` & `hello50-1.0.3/hello50.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hello50
-Version: 1.0.2
+Version: 1.0.3
 Summary: Hello world shit!!!!
 Author: Malik
 Author-email: myemail46926213@gmail.com
 Keywords: python,hello
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
-Hello world 000~~~~~
+Hello world 3~~~~~
```

### Comparing `hello50-1.0.2/setup.py` & `hello50-1.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'Hello world shit!!!!'
-LONG_DESCRIPTION = 'Hello world 000~~~~~'
+LONG_DESCRIPTION = 'Hello world 3~~~~~'
 
 # Setting up
 setup(
     name="hello50",
     version=VERSION,
     author="Malik",
     author_email="myemail46926213@gmail.com",
@@ -27,8 +27,14 @@
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
+
+
+"""
+twine upload dist/*
+
+"""
```

