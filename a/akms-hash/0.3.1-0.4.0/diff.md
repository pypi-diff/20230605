# Comparing `tmp/akms-hash-0.3.1.tar.gz` & `tmp/akms-hash-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akms-hash-0.3.1.tar", last modified: Sun Nov 13 02:13:16 2022, max compression
+gzip compressed data, was "akms-hash-0.4.0.tar", last modified: Mon Jun  5 13:19:40 2023, max compression
```

## Comparing `akms-hash-0.3.1.tar` & `akms-hash-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2022-11-13 02:13:16.363661 akms-hash-0.3.1/
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      461 2022-11-13 02:13:16.363429 akms-hash-0.3.1/PKG-INFO
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)       39 2022-11-08 13:45:43.000000 akms-hash-0.3.1/README.md
-drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2022-11-13 02:13:16.362594 akms-hash-0.3.1/akms_hash/
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      109 2022-11-11 22:34:57.000000 akms-hash-0.3.1/akms_hash/__init__.py
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      649 2022-11-13 01:55:35.000000 akms-hash-0.3.1/akms_hash/main.py
-drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2022-11-13 02:13:16.363223 akms-hash-0.3.1/akms_hash.egg-info/
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      461 2022-11-13 02:13:16.000000 akms-hash-0.3.1/akms_hash.egg-info/PKG-INFO
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      205 2022-11-13 02:13:16.000000 akms-hash-0.3.1/akms_hash.egg-info/SOURCES.txt
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)        1 2022-11-13 02:13:16.000000 akms-hash-0.3.1/akms_hash.egg-info/dependency_links.txt
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)       10 2022-11-13 02:13:16.000000 akms-hash-0.3.1/akms_hash.egg-info/top_level.txt
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      113 2022-11-12 20:05:38.000000 akms-hash-0.3.1/pyproject.toml
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)       38 2022-11-13 02:13:16.363708 akms-hash-0.3.1/setup.cfg
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      683 2022-11-13 02:13:07.000000 akms-hash-0.3.1/setup.py
+drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2023-06-05 13:19:40.883102 akms-hash-0.4.0/
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      643 2023-06-05 13:19:40.882854 akms-hash-0.4.0/PKG-INFO
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      224 2023-06-05 13:18:40.000000 akms-hash-0.4.0/README.md
+drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2023-06-05 13:19:40.881626 akms-hash-0.4.0/akms_hash/
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      109 2022-11-11 22:34:57.000000 akms-hash-0.4.0/akms_hash/__init__.py
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      649 2022-11-13 01:55:35.000000 akms-hash-0.4.0/akms_hash/main.py
+drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2023-06-05 13:19:40.882634 akms-hash-0.4.0/akms_hash.egg-info/
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      643 2023-06-05 13:19:40.000000 akms-hash-0.4.0/akms_hash.egg-info/PKG-INFO
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      205 2023-06-05 13:19:40.000000 akms-hash-0.4.0/akms_hash.egg-info/SOURCES.txt
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)        1 2023-06-05 13:19:40.000000 akms-hash-0.4.0/akms_hash.egg-info/dependency_links.txt
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)       10 2023-06-05 13:19:40.000000 akms-hash-0.4.0/akms_hash.egg-info/top_level.txt
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      113 2022-11-12 20:05:38.000000 akms-hash-0.4.0/pyproject.toml
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)       38 2023-06-05 13:19:40.883151 akms-hash-0.4.0/setup.cfg
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      680 2023-06-05 13:18:40.000000 akms-hash-0.4.0/setup.py
```

### Comparing `akms-hash-0.3.1/akms_hash/main.py` & `akms-hash-0.4.0/akms_hash/main.py`

 * *Files identical despite different names*

### Comparing `akms-hash-0.3.1/setup.py` & `akms-hash-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="akms-hash",
-    version="0.3.1",
+    version="0.4.0",
     author="apinanyogaratnam",
     author_email="apinanapinan@icloud.com",
     description="An API Key hashing library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/apinanyogaratnam/akms-hash",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.10.4",
+    python_requires=">=3.8",
     install_requires=[],
 )
```

