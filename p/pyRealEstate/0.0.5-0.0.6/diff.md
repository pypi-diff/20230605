# Comparing `tmp/pyRealEstate-0.0.5.tar.gz` & `tmp/pyRealEstate-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.0.5.tar", last modified: Mon Jun  5 10:58:31 2023, max compression
+gzip compressed data, was "pyRealEstate-0.0.6.tar", last modified: Mon Jun  5 17:13:53 2023, max compression
```

## Comparing `pyRealEstate-0.0.5.tar` & `pyRealEstate-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:58:31.134799 pyRealEstate-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 10:58:31.134799 pyRealEstate-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:58:31.134799 pyRealEstate-0.0.5/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:58:31.134799 pyRealEstate-0.0.5/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 10:58:31.000000 pyRealEstate-0.0.5/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-05 10:58:31.000000 pyRealEstate-0.0.5/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:58:31.000000 pyRealEstate-0.0.5/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:58:31.000000 pyRealEstate-0.0.5/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 10:58:31.000000 pyRealEstate-0.0.5/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/pypi_description.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 10:58:21.000000 pyRealEstate-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-05 10:58:31.134799 pyRealEstate-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:13:53.332677 pyRealEstate-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-05 17:13:53.332677 pyRealEstate-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:13:53.328677 pyRealEstate-0.0.6/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pyRealEstate/Pre_Processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pyRealEstate/Time_Trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:13:53.332677 pyRealEstate-0.0.6/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-05 17:13:53.000000 pyRealEstate-0.0.6/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-05 17:13:53.000000 pyRealEstate-0.0.6/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:13:53.000000 pyRealEstate-0.0.6/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 17:13:53.000000 pyRealEstate-0.0.6/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 17:13:53.000000 pyRealEstate-0.0.6/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pypi_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 17:13:43.000000 pyRealEstate-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-05 17:13:53.332677 pyRealEstate-0.0.6/setup.cfg
```

### Comparing `pyRealEstate-0.0.5/LICENSE` & `pyRealEstate-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.5/PKG-INFO` & `pyRealEstate-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.5
+Version: 0.0.6
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyRealEstate
 
 pyRealEstate is a package designed for data scientists working in the real estate industry.  This Library aims to provide tools to help in the preprocessing of data, feature engineering and evaluation 
-of AVM's (Automated valuation models). Some of metrics provided in this library are the COD ( coeficient of Disspersion), PRD ( Price Relted Differential) and weighted mean for example. pyRealEstate is still currently under development 
-but is aimed at providing functions to assist in the development and evaluation of AVM's sp please continually check for updates . 
+of AVM's (Automated Valuation Models). Some of the metrics provided in this library are the COD ( Coeficient of Disspersion), PRD ( Price Related Differential) and weighted mean for example. pyRealEstate is still currently under development, please check back for updates frequently. 
 
 ## Installation
 
 Simply run:
 ```
-pip3 install pyRealEstate
+pip install pyRealEstate
 ```
```

### Comparing `pyRealEstate-0.0.5/README.md` & `pyRealEstate-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.5/pyRealEstate/RealEstateMetrics.py` & `pyRealEstate-0.0.6/pyRealEstate/RealEstateMetrics.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pandas as pd 
 import numpy as np
+import pandas as pd 
 import statsmodels.api as sm
 
 
 def weighted_Mean_Sale_Ratio ( y, x ):
   return np.mean(x) / np.mean(y)
 
 def COD( y, x):
```

### Comparing `pyRealEstate-0.0.5/pyRealEstate.egg-info/PKG-INFO` & `pyRealEstate-0.0.6/pyRealEstate.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.5
+Version: 0.0.6
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyRealEstate
 
 pyRealEstate is a package designed for data scientists working in the real estate industry.  This Library aims to provide tools to help in the preprocessing of data, feature engineering and evaluation 
-of AVM's (Automated valuation models). Some of metrics provided in this library are the COD ( coeficient of Disspersion), PRD ( Price Relted Differential) and weighted mean for example. pyRealEstate is still currently under development 
-but is aimed at providing functions to assist in the development and evaluation of AVM's sp please continually check for updates . 
+of AVM's (Automated Valuation Models). Some of the metrics provided in this library are the COD ( Coeficient of Disspersion), PRD ( Price Related Differential) and weighted mean for example. pyRealEstate is still currently under development, please check back for updates frequently. 
 
 ## Installation
 
 Simply run:
 ```
-pip3 install pyRealEstate
+pip install pyRealEstate
 ```
```

### Comparing `pyRealEstate-0.0.5/pypi_description.md` & `pyRealEstate-0.0.6/pypi_description.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # pyRealEstate
 
 pyRealEstate is a package designed for data scientists working in the real estate industry.  This Library aims to provide tools to help in the preprocessing of data, feature engineering and evaluation 
-of AVM's (Automated valuation models). Some of metrics provided in this library are the COD ( coeficient of Disspersion), PRD ( Price Relted Differential) and weighted mean for example. pyRealEstate is still currently under development 
-but is aimed at providing functions to assist in the development and evaluation of AVM's sp please continually check for updates . 
+of AVM's (Automated Valuation Models). Some of the metrics provided in this library are the COD ( Coeficient of Disspersion), PRD ( Price Related Differential) and weighted mean for example. pyRealEstate is still currently under development, please check back for updates frequently. 
 
 ## Installation
 
 Simply run:
 ```
-pip3 install pyRealEstate
+pip install pyRealEstate
 ```
```

### Comparing `pyRealEstate-0.0.5/setup.cfg` & `pyRealEstate-0.0.6/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyRealEstate
-version = 0.0.5
+version = 0.0.6
 author = Joshua Jorgensen
 description = package to assist with data analytics in real estate
 long_description = file: pypi_description.md
 long_description_content_type = text/markdown
 url = https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 classifiers = 
 	Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 	Operating System :: OS Independent
 
 [options]
 install_requires = scikit-learn
 	numpy
 	pandas
 	statsmodels
+	matplotlib
 packages = find:
 python_requires = >=3.4
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

