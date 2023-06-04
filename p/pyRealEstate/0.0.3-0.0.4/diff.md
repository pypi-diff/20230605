# Comparing `tmp/pyRealEstate-0.0.3.tar.gz` & `tmp/pyRealEstate-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.0.3.tar", last modified: Sun Jun  4 11:35:38 2023, max compression
+gzip compressed data, was "pyRealEstate-0.0.4.tar", last modified: Sun Jun  4 22:28:53 2023, max compression
```

## Comparing `pyRealEstate-0.0.3.tar` & `pyRealEstate-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:35:38.535899 pyRealEstate-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-04 11:35:38.539899 pyRealEstate-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:35:38.535899 pyRealEstate-0.0.3/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:35:38.535899 pyRealEstate-0.0.3/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-04 11:35:38.000000 pyRealEstate-0.0.3/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-04 11:35:38.000000 pyRealEstate-0.0.3/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:35:38.000000 pyRealEstate-0.0.3/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 11:35:38.000000 pyRealEstate-0.0.3/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 11:35:38.000000 pyRealEstate-0.0.3/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/pypi_description.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-04 11:35:38.539899 pyRealEstate-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:28:53.888336 pyRealEstate-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-04 22:28:53.888336 pyRealEstate-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:28:53.888336 pyRealEstate-0.0.4/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:28:53.888336 pyRealEstate-0.0.4/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-04 22:28:53.000000 pyRealEstate-0.0.4/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-04 22:28:53.000000 pyRealEstate-0.0.4/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:28:53.000000 pyRealEstate-0.0.4/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 22:28:53.000000 pyRealEstate-0.0.4/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 22:28:53.000000 pyRealEstate-0.0.4/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/pypi_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-04 22:28:53.888336 pyRealEstate-0.0.4/setup.cfg
```

### Comparing `pyRealEstate-0.0.3/LICENSE` & `pyRealEstate-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.3/PKG-INFO` & `pyRealEstate-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.3
+Version: 0.0.4
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyRealEstate
 
 pyRealEstate is a package designed for data scientists working in the real estate industry.  This Library aims to provide tools to help in the preprocessing of data, feature engineering and evaluation 
 of AVM's (Automated valuation models). Some of metrics provided in this library are the COD ( coeficient of Disspersion), PRD ( Price Relted Differential) and weighted mean for example. pyRealEstate is still currently under development
```

### Comparing `pyRealEstate-0.0.3/README.md` & `pyRealEstate-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.3/pyRealEstate.egg-info/PKG-INFO` & `pyRealEstate-0.0.4/pyRealEstate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.3
+Version: 0.0.4
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyRealEstate
 
 pyRealEstate is a package designed for data scientists working in the real estate industry.  This Library aims to provide tools to help in the preprocessing of data, feature engineering and evaluation 
 of AVM's (Automated valuation models). Some of metrics provided in this library are the COD ( coeficient of Disspersion), PRD ( Price Relted Differential) and weighted mean for example. pyRealEstate is still currently under development
```

### Comparing `pyRealEstate-0.0.3/pypi_description.md` & `pyRealEstate-0.0.4/pypi_description.md`

 * *Files identical despite different names*

