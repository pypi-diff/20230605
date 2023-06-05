# Comparing `tmp/ExtendClass-1.0.3.tar.gz` & `tmp/ExtendClass-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExtendClass-1.0.3.tar", last modified: Mon Jun  5 12:18:44 2023, max compression
+gzip compressed data, was "ExtendClass-1.0.4.tar", last modified: Mon Jun  5 12:28:02 2023, max compression
```

## Comparing `ExtendClass-1.0.3.tar` & `ExtendClass-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-05 12:18:44.490335 ExtendClass-1.0.3/
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-05 12:18:44.490335 ExtendClass-1.0.3/ExtendClass/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2145 2023-06-05 12:18:35.000000 ExtendClass-1.0.3/ExtendClass/Extension.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      418 2023-06-02 14:33:22.000000 ExtendClass-1.0.3/ExtendClass/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-05 12:18:44.490335 ExtendClass-1.0.3/ExtendClass.egg-info/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-06-05 12:18:44.000000 ExtendClass-1.0.3/ExtendClass.egg-info/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      215 2023-06-05 12:18:44.000000 ExtendClass-1.0.3/ExtendClass.egg-info/SOURCES.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-06-05 12:18:44.000000 ExtendClass-1.0.3/ExtendClass.egg-info/dependency_links.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       12 2023-06-05 12:18:44.000000 ExtendClass-1.0.3/ExtendClass.egg-info/top_level.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    35149 2023-06-02 14:05:22.000000 ExtendClass-1.0.3/LICENSE
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-06-05 12:18:44.490335 ExtendClass-1.0.3/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      121 2023-06-02 14:05:22.000000 ExtendClass-1.0.3/README.md
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-06-05 12:18:44.490335 ExtendClass-1.0.3/setup.cfg
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      977 2023-06-05 11:55:45.000000 ExtendClass-1.0.3/setup.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-05 12:28:02.904117 ExtendClass-1.0.4/
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-05 12:28:02.904117 ExtendClass-1.0.4/ExtendClass/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2145 2023-06-05 12:27:46.000000 ExtendClass-1.0.4/ExtendClass/Extension.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      418 2023-06-02 14:33:22.000000 ExtendClass-1.0.4/ExtendClass/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-05 12:28:02.904117 ExtendClass-1.0.4/ExtendClass.egg-info/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-06-05 12:28:02.000000 ExtendClass-1.0.4/ExtendClass.egg-info/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      215 2023-06-05 12:28:02.000000 ExtendClass-1.0.4/ExtendClass.egg-info/SOURCES.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-06-05 12:28:02.000000 ExtendClass-1.0.4/ExtendClass.egg-info/dependency_links.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       12 2023-06-05 12:28:02.000000 ExtendClass-1.0.4/ExtendClass.egg-info/top_level.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    35149 2023-06-02 14:05:22.000000 ExtendClass-1.0.4/LICENSE
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-06-05 12:28:02.904117 ExtendClass-1.0.4/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      540 2023-06-05 12:21:38.000000 ExtendClass-1.0.4/README.md
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-06-05 12:28:02.908117 ExtendClass-1.0.4/setup.cfg
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      977 2023-06-05 12:23:14.000000 ExtendClass-1.0.4/setup.py
```

### Comparing `ExtendClass-1.0.3/ExtendClass/Extension.py` & `ExtendClass-1.0.4/ExtendClass/Extension.py`

 * *Files identical despite different names*

### Comparing `ExtendClass-1.0.3/ExtendClass.egg-info/PKG-INFO` & `ExtendClass-1.0.4/ExtendClass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExtendClass
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python lib to extend classes
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,extend,class,extend class,extendclass,extend-class,extend_class,extendclass
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ExtendClass-1.0.3/LICENSE` & `ExtendClass-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ExtendClass-1.0.3/PKG-INFO` & `ExtendClass-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExtendClass
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python lib to extend classes
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,extend,class,extend class,extendclass,extend-class,extend_class,extendclass
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ExtendClass-1.0.3/setup.py` & `ExtendClass-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'A python lib to extend classes'
 LONG_DESCRIPTION = 'A python lib to extend classes. Inject methods in a class without inheritance. It access protected methods and attributes.'
 
 # Setting up
 setup(
     name="ExtendClass",
     version=VERSION,
```

