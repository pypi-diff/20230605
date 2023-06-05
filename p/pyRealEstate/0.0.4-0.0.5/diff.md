# Comparing `tmp/pyRealEstate-0.0.4.tar.gz` & `tmp/pyRealEstate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.0.4.tar", last modified: Sun Jun  4 22:28:53 2023, max compression
+gzip compressed data, was "pyRealEstate-0.0.5.tar", last modified: Mon Jun  5 10:58:31 2023, max compression
```

## Comparing `pyRealEstate-0.0.4.tar` & `pyRealEstate-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:28:53.888336 pyRealEstate-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-04 22:28:53.888336 pyRealEstate-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:28:53.888336 pyRealEstate-0.0.4/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:28:53.888336 pyRealEstate-0.0.4/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-04 22:28:53.000000 pyRealEstate-0.0.4/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-04 22:28:53.000000 pyRealEstate-0.0.4/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:28:53.000000 pyRealEstate-0.0.4/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 22:28:53.000000 pyRealEstate-0.0.4/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 22:28:53.000000 pyRealEstate-0.0.4/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/pypi_description.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-04 22:28:40.000000 pyRealEstate-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-04 22:28:53.888336 pyRealEstate-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:58:31.134799 pyRealEstate-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 10:58:31.134799 pyRealEstate-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:58:31.134799 pyRealEstate-0.0.5/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:58:31.134799 pyRealEstate-0.0.5/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 10:58:31.000000 pyRealEstate-0.0.5/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-05 10:58:31.000000 pyRealEstate-0.0.5/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:58:31.000000 pyRealEstate-0.0.5/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:58:31.000000 pyRealEstate-0.0.5/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 10:58:31.000000 pyRealEstate-0.0.5/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/pypi_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-05 10:58:31.134799 pyRealEstate-0.0.5/setup.cfg
```

### Comparing `pyRealEstate-0.0.4/LICENSE` & `pyRealEstate-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.4/PKG-INFO` & `pyRealEstate-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.4
+Version: 0.0.5
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
@@ -13,13 +13,13 @@
 
 # pyRealEstate
 
 pyRealEstate is a package designed for data scientists working in the real estate industry.  This Library aims to provide tools to help in the preprocessing of data, feature engineering and evaluation 
 of AVM's (Automated valuation models). Some of metrics provided in this library are the COD ( coeficient of Disspersion), PRD ( Price Relted Differential) and weighted mean for example. pyRealEstate is still currently under development 
 but is aimed at providing functions to assist in the development and evaluation of AVM's sp please continually check for updates . 
 
-## Instilation
+## Installation
 
 Simply run:
 ```
 pip3 install pyRealEstate
 ```
```

### Comparing `pyRealEstate-0.0.4/README.md` & `pyRealEstate-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyRealEstate
 
 pyRealEstate is a library designed for data scientists working in the real estate industry. pyRealEstate is still currently under development but is aimed at providing functions to assist in the development and evaluation of AVM's. Below are some instructions on how to get started with pyRealEstate and some helpful links to descriptions and examples of all of PyRealEstates functionality 
 
-## Instillation
+## Installation
 
 the pyRealEstate package is available on [PyPi](https://pypi.org/project/pyRealEstate). Simply run: 
 ```
-pip3 install pyRealEstate
+pip install pyRealEstate
 ```
 ## AVM Evalutation Metrics
 pyRealEstate can provide metrics on the evaluation of your AVM( AAutomated Valuation Model) such as the weighted mean sale ratio, COD (Coefficient Of Disspersion), and PRD ( Price Related Differential) please visit the wiki for detailed documentation [pyRealEstate Evaluation](https://github.com/Joshua-Data-Wizard/PyRealEstate/wiki/AVM-Evaluation-Metrics)
```

### Comparing `pyRealEstate-0.0.4/pyRealEstate/RealEstateMetrics.py` & `pyRealEstate-0.0.5/pyRealEstate/RealEstateMetrics.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.4/pyRealEstate.egg-info/PKG-INFO` & `pyRealEstate-0.0.5/pyRealEstate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.4
+Version: 0.0.5
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
@@ -13,13 +13,13 @@
 
 # pyRealEstate
 
 pyRealEstate is a package designed for data scientists working in the real estate industry.  This Library aims to provide tools to help in the preprocessing of data, feature engineering and evaluation 
 of AVM's (Automated valuation models). Some of metrics provided in this library are the COD ( coeficient of Disspersion), PRD ( Price Relted Differential) and weighted mean for example. pyRealEstate is still currently under development 
 but is aimed at providing functions to assist in the development and evaluation of AVM's sp please continually check for updates . 
 
-## Instilation
+## Installation
 
 Simply run:
 ```
 pip3 install pyRealEstate
 ```
```

### Comparing `pyRealEstate-0.0.4/pypi_description.md` & `pyRealEstate-0.0.5/pypi_description.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyRealEstate
 
 pyRealEstate is a package designed for data scientists working in the real estate industry.  This Library aims to provide tools to help in the preprocessing of data, feature engineering and evaluation 
 of AVM's (Automated valuation models). Some of metrics provided in this library are the COD ( coeficient of Disspersion), PRD ( Price Relted Differential) and weighted mean for example. pyRealEstate is still currently under development 
 but is aimed at providing functions to assist in the development and evaluation of AVM's sp please continually check for updates . 
 
-## Instilation
+## Installation
 
 Simply run:
 ```
 pip3 install pyRealEstate
 ```
```

### Comparing `pyRealEstate-0.0.4/setup.cfg` & `pyRealEstate-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyRealEstate
-version = 0.0.4
+version = 0.0.5
 author = Joshua Jorgensen
 description = package to assist with data analytics in real estate
 long_description = file: pypi_description.md
 long_description_content_type = text/markdown
 url = https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 classifiers = 
 	Programming Language :: Python :: 3
```

