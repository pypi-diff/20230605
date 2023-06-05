# Comparing `tmp/bayanpy-0.7.3.tar.gz` & `tmp/bayanpy-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.7.3.tar", last modified: Mon May 22 15:34:46 2023, max compression
+gzip compressed data, was "bayanpy-0.7.4.tar", last modified: Mon Jun  5 18:05:59 2023, max compression
```

## Comparing `bayanpy-0.7.3.tar` & `bayanpy-0.7.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-22 15:34:46.476622 bayanpy-0.7.3/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.7.3/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-22 15:34:46.476622 bayanpy-0.7.3/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5350 2023-05-07 16:54:32.000000 bayanpy-0.7.3/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-22 15:34:46.476622 bayanpy-0.7.3/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    59427 2023-05-20 16:15:23.000000 bayanpy-0.7.3/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.7.3/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-22 15:34:46.476622 bayanpy-0.7.3/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-22 15:34:46.000000 bayanpy-0.7.3/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-22 15:34:46.000000 bayanpy-0.7.3/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-22 15:34:46.000000 bayanpy-0.7.3/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-22 15:34:46.000000 bayanpy-0.7.3/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-22 15:34:46.000000 bayanpy-0.7.3/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-22 15:34:46.476622 bayanpy-0.7.3/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-22 15:34:21.000000 bayanpy-0.7.3/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-06-05 18:05:59.114945 bayanpy-0.7.4/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.7.4/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-06-05 18:05:59.114945 bayanpy-0.7.4/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5350 2023-05-07 16:54:32.000000 bayanpy-0.7.4/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-06-05 18:05:59.114945 bayanpy-0.7.4/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    59427 2023-05-20 16:15:23.000000 bayanpy-0.7.4/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.7.4/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-06-05 18:05:59.114945 bayanpy-0.7.4/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-06-05 18:05:59.000000 bayanpy-0.7.4/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-06-05 18:05:59.000000 bayanpy-0.7.4/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-06-05 18:05:59.000000 bayanpy-0.7.4/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-06-05 18:05:59.000000 bayanpy-0.7.4/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-06-05 18:05:59.000000 bayanpy-0.7.4/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-06-05 18:05:59.114945 bayanpy-0.7.4/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-06-05 18:05:41.000000 bayanpy-0.7.4/setup.py
```

### Comparing `bayanpy-0.7.3/LICENSE` & `bayanpy-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.7.3/README.md` & `bayanpy-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `bayanpy-0.7.3/bayanpy/BayanImplied.py` & `bayanpy-0.7.4/bayanpy/BayanImplied.py`

 * *Files identical despite different names*

### Comparing `bayanpy-0.7.3/setup.py` & `bayanpy-0.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.7.3",
+    version="0.7.4",
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
```

