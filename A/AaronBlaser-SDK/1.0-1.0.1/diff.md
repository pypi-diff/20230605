# Comparing `tmp/AaronBlaser-SDK-1.0.tar.gz` & `tmp/AaronBlaser-SDK-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AaronBlaser-SDK-1.0.tar", last modified: Mon Jun  5 01:19:48 2023, max compression
+gzip compressed data, was "AaronBlaser-SDK-1.0.1.tar", last modified: Mon Jun  5 01:24:10 2023, max compression
```

## Comparing `AaronBlaser-SDK-1.0.tar` & `AaronBlaser-SDK-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 01:19:48.748790 AaronBlaser-SDK-1.0/
-drwxrwxrwx   0        0        0        0 2023-06-05 01:19:48.743087 AaronBlaser-SDK-1.0/AaronBlaser_SDK.egg-info/
--rw-rw-rw-   0        0        0     2964 2023-06-05 01:19:48.000000 AaronBlaser-SDK-1.0/AaronBlaser_SDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-06-05 01:19:48.000000 AaronBlaser-SDK-1.0/AaronBlaser_SDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 01:19:48.000000 AaronBlaser-SDK-1.0/AaronBlaser_SDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-06-05 01:19:48.000000 AaronBlaser-SDK-1.0/AaronBlaser_SDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-05 01:19:48.000000 AaronBlaser-SDK-1.0/AaronBlaser_SDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2964 2023-06-05 01:19:48.746079 AaronBlaser-SDK-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2551 2023-06-05 00:47:52.000000 AaronBlaser-SDK-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 01:19:48.744083 AaronBlaser-SDK-1.0/lordoftherings/
--rw-rw-rw-   0        0        0       42 2023-06-05 00:58:43.000000 AaronBlaser-SDK-1.0/lordoftherings/__init__.py
--rw-rw-rw-   0        0        0    10611 2023-06-04 23:37:00.000000 AaronBlaser-SDK-1.0/lordoftherings/lordoftherings.py
--rw-rw-rw-   0        0        0       42 2023-06-05 01:19:48.748790 AaronBlaser-SDK-1.0/setup.cfg
--rw-rw-rw-   0        0        0      770 2023-06-05 01:18:08.000000 AaronBlaser-SDK-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:19:48.746079 AaronBlaser-SDK-1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-05 00:03:15.000000 AaronBlaser-SDK-1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     8526 2023-06-05 01:09:01.000000 AaronBlaser-SDK-1.0/tests/test_lordoftherings.py
--rw-rw-rw-   0        0        0     2081 2023-06-05 01:10:16.000000 AaronBlaser-SDK-1.0/tests/test_usage.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:24:10.904014 AaronBlaser-SDK-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-05 01:24:10.900024 AaronBlaser-SDK-1.0.1/AaronBlaser_SDK.egg-info/
+-rw-rw-rw-   0        0        0     2971 2023-06-05 01:24:10.000000 AaronBlaser-SDK-1.0.1/AaronBlaser_SDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-06-05 01:24:10.000000 AaronBlaser-SDK-1.0.1/AaronBlaser_SDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 01:24:10.000000 AaronBlaser-SDK-1.0.1/AaronBlaser_SDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-06-05 01:24:10.000000 AaronBlaser-SDK-1.0.1/AaronBlaser_SDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-05 01:24:10.000000 AaronBlaser-SDK-1.0.1/AaronBlaser_SDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2971 2023-06-05 01:24:10.903020 AaronBlaser-SDK-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2556 2023-06-05 01:23:29.000000 AaronBlaser-SDK-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 01:24:10.901023 AaronBlaser-SDK-1.0.1/lordoftherings/
+-rw-rw-rw-   0        0        0       42 2023-06-05 00:58:43.000000 AaronBlaser-SDK-1.0.1/lordoftherings/__init__.py
+-rw-rw-rw-   0        0        0    10611 2023-06-04 23:37:00.000000 AaronBlaser-SDK-1.0.1/lordoftherings/lordoftherings.py
+-rw-rw-rw-   0        0        0       42 2023-06-05 01:24:10.904014 AaronBlaser-SDK-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      772 2023-06-05 01:23:15.000000 AaronBlaser-SDK-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:24:10.903020 AaronBlaser-SDK-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-05 00:03:15.000000 AaronBlaser-SDK-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     8526 2023-06-05 01:09:01.000000 AaronBlaser-SDK-1.0.1/tests/test_lordoftherings.py
+-rw-rw-rw-   0        0        0     2081 2023-06-05 01:10:16.000000 AaronBlaser-SDK-1.0.1/tests/test_usage.py
```

### Comparing `AaronBlaser-SDK-1.0/AaronBlaser_SDK.egg-info/PKG-INFO` & `AaronBlaser-SDK-1.0.1/AaronBlaser_SDK.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: AaronBlaser-SDK
-Version: 1.0
+Version: 1.0.1
 Summary: SDK for the lord of the rings API
 Home-page: https://github.com/ablaser5/AaronBlaser-SDK
 Author: Aaron Blaser
 Author-email: ablaser5@comcast.net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
 # LordOfTheRings SDK
 
 ## Installation
 
 ```bash
-pip install lord_of_the_rings
+pip install AaronBlaser-SDK==1.0.1
 ```
 
 ## Usage
 
 1. Import the LordOfTheRings class
 
 ```python
```

### Comparing `AaronBlaser-SDK-1.0/PKG-INFO` & `AaronBlaser-SDK-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: AaronBlaser-SDK
-Version: 1.0
+Version: 1.0.1
 Summary: SDK for the lord of the rings API
 Home-page: https://github.com/ablaser5/AaronBlaser-SDK
 Author: Aaron Blaser
 Author-email: ablaser5@comcast.net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
 # LordOfTheRings SDK
 
 ## Installation
 
 ```bash
-pip install lord_of_the_rings
+pip install AaronBlaser-SDK==1.0.1
 ```
 
 ## Usage
 
 1. Import the LordOfTheRings class
 
 ```python
```

### Comparing `AaronBlaser-SDK-1.0/README.md` & `AaronBlaser-SDK-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # LordOfTheRings SDK
 
 ## Installation
 
 ```bash
-pip install lord_of_the_rings
+pip install AaronBlaser-SDK==1.0.1
 ```
 
 ## Usage
 
 1. Import the LordOfTheRings class
 
 ```python
```

### Comparing `AaronBlaser-SDK-1.0/lordoftherings/lordoftherings.py` & `AaronBlaser-SDK-1.0.1/lordoftherings/lordoftherings.py`

 * *Files identical despite different names*

### Comparing `AaronBlaser-SDK-1.0/setup.py` & `AaronBlaser-SDK-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AaronBlaser-SDK",
-    version="1.0",
+    version="1.0.1",
     author="Aaron Blaser",
     author_email="ablaser5@comcast.net",
     description="SDK for the lord of the rings API",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/ablaser5/AaronBlaser-SDK",
     packages=find_packages(),
```

### Comparing `AaronBlaser-SDK-1.0/tests/test_lordoftherings.py` & `AaronBlaser-SDK-1.0.1/tests/test_lordoftherings.py`

 * *Files identical despite different names*

### Comparing `AaronBlaser-SDK-1.0/tests/test_usage.py` & `AaronBlaser-SDK-1.0.1/tests/test_usage.py`

 * *Files identical despite different names*

