# Comparing `tmp/ch.zbindenonline.weatherstation-1.6.1.tar.gz` & `tmp/ch.zbindenonline.weatherstation-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch.zbindenonline.weatherstation-1.6.1.tar", last modified: Thu Jun  2 17:59:21 2022, max compression
+gzip compressed data, was "ch.zbindenonline.weatherstation-1.7.0.tar", last modified: Mon Jun  5 13:14:09 2023, max compression
```

## Comparing `ch.zbindenonline.weatherstation-1.6.1.tar` & `ch.zbindenonline.weatherstation-1.7.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 building  (1001)      998        0 2022-06-02 17:59:21.804762 ch.zbindenonline.weatherstation-1.6.1/
--rw-r--r--   0 building  (1001)      998     1068 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/LICENSE
--rw-r--r--   0 building  (1001)      998      588 2022-06-02 17:59:21.804762 ch.zbindenonline.weatherstation-1.6.1/PKG-INFO
--rw-r--r--   0 building  (1001)      998      245 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/README.md
-drwxr-xr-x   0 building  (1001)      998        0 2022-06-02 17:59:21.784762 ch.zbindenonline.weatherstation-1.6.1/ch/
--rw-r--r--   0 building  (1001)      998        0 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/__init__.py
-drwxr-xr-x   0 building  (1001)      998        0 2022-06-02 17:59:21.788762 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/
--rw-r--r--   0 building  (1001)      998        0 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/__init__.py
-drwxr-xr-x   0 building  (1001)      998        0 2022-06-02 17:59:21.796762 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/
--rw-r--r--   0 building  (1001)      998        0 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/__init__.py
--rw-r--r--   0 building  (1001)      998     2706 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/config.py
--rw-r--r--   0 building  (1001)      998      280 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/domain.py
--rw-r--r--   0 building  (1001)      998      314 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/logging.py
--rw-r--r--   0 building  (1001)      998     4315 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/measureRepository.py
--rw-r--r--   0 building  (1001)      998     1754 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/publishMeasures.py
--rw-r--r--   0 building  (1001)      998     3239 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/publishPictures.py
--rw-r--r--   0 building  (1001)      998     2609 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/restServiceMeasures.py
--rw-r--r--   0 building  (1001)      998     4467 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/restServicePictures.py
--rw-r--r--   0 building  (1001)      998     1004 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/saveMeasures.py
--rw-r--r--   0 building  (1001)      998     1653 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/sensorService.py
-drwxr-xr-x   0 building  (1001)      998        0 2022-06-02 17:59:21.788762 ch.zbindenonline.weatherstation-1.6.1/ch.zbindenonline.weatherstation.egg-info/
--rw-r--r--   0 building  (1001)      998      588 2022-06-02 17:59:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch.zbindenonline.weatherstation.egg-info/PKG-INFO
--rw-r--r--   0 building  (1001)      998     1644 2022-06-02 17:59:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch.zbindenonline.weatherstation.egg-info/SOURCES.txt
--rw-r--r--   0 building  (1001)      998        1 2022-06-02 17:59:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch.zbindenonline.weatherstation.egg-info/dependency_links.txt
--rw-r--r--   0 building  (1001)      998      226 2022-06-02 17:59:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch.zbindenonline.weatherstation.egg-info/entry_points.txt
--rw-r--r--   0 building  (1001)      998       27 2022-06-02 17:59:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch.zbindenonline.weatherstation.egg-info/requires.txt
--rw-r--r--   0 building  (1001)      998        9 2022-06-02 17:59:21.000000 ch.zbindenonline.weatherstation-1.6.1/ch.zbindenonline.weatherstation.egg-info/top_level.txt
--rw-r--r--   0 building  (1001)      998       38 2022-06-02 17:59:21.804762 ch.zbindenonline.weatherstation-1.6.1/setup.cfg
--rw-r--r--   0 building  (1001)      998      934 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/setup.py
-drwxr-xr-x   0 building  (1001)      998        0 2022-06-02 17:59:21.796762 ch.zbindenonline.weatherstation-1.6.1/tests/
--rw-r--r--   0 building  (1001)      998        0 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/__init__.py
-drwxr-xr-x   0 building  (1001)      998        0 2022-06-02 17:59:21.796762 ch.zbindenonline.weatherstation-1.6.1/tests/ch/
--rw-r--r--   0 building  (1001)      998        0 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/__init__.py
-drwxr-xr-x   0 building  (1001)      998        0 2022-06-02 17:59:21.796762 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/
--rw-r--r--   0 building  (1001)      998        0 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/__init__.py
-drwxr-xr-x   0 building  (1001)      998        0 2022-06-02 17:59:21.804762 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/
--rw-r--r--   0 building  (1001)      998        0 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/__init__.py
--rw-r--r--   0 building  (1001)      998      600 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/mocks.py
--rw-r--r--   0 building  (1001)      998     2535 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_MeasureRepository.py
--rw-r--r--   0 building  (1001)      998     2459 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_config.py
--rw-r--r--   0 building  (1001)      998     3148 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_publishMeasures.py
--rw-r--r--   0 building  (1001)      998     5116 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_publishPictures.py
--rw-r--r--   0 building  (1001)      998     4957 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_restServiceMeasures.py
--rw-r--r--   0 building  (1001)      998    10156 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_restServicePictures.py
--rw-r--r--   0 building  (1001)      998     1605 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_saveMeasures.py
--rw-r--r--   0 building  (1001)      998     3157 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_sensorService.py
--rw-r--r--   0 building  (1001)      998      130 2022-06-02 17:58:21.000000 ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:14:09.964532 ch.zbindenonline.weatherstation-1.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      550 2023-06-05 13:14:09.964532 ch.zbindenonline.weatherstation-1.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:14:09.900533 ch.zbindenonline.weatherstation-1.7.0/ch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:14:09.904533 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:14:09.956532 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2706 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/config.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/domain.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/logging.py
+-rw-r--r--   0 root         (0) root         (0)     4315 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/measureRepository.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/publishMeasures.py
+-rw-r--r--   0 root         (0) root         (0)     3239 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/publishPictures.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/restServiceMeasures.py
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/restServicePictures.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/saveMeasures.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/sensorService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:14:09.904533 ch.zbindenonline.weatherstation-1.7.0/ch.zbindenonline.weatherstation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      550 2023-06-05 13:14:09.000000 ch.zbindenonline.weatherstation-1.7.0/ch.zbindenonline.weatherstation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-05 13:14:09.000000 ch.zbindenonline.weatherstation-1.7.0/ch.zbindenonline.weatherstation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 13:14:09.000000 ch.zbindenonline.weatherstation-1.7.0/ch.zbindenonline.weatherstation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      225 2023-06-05 13:14:09.000000 ch.zbindenonline.weatherstation-1.7.0/ch.zbindenonline.weatherstation.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-05 13:14:09.000000 ch.zbindenonline.weatherstation-1.7.0/ch.zbindenonline.weatherstation.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-05 13:14:09.000000 ch.zbindenonline.weatherstation-1.7.0/ch.zbindenonline.weatherstation.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 13:14:09.964532 ch.zbindenonline.weatherstation-1.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      934 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:14:09.956532 ch.zbindenonline.weatherstation-1.7.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:14:09.956532 ch.zbindenonline.weatherstation-1.7.0/tests/ch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:14:09.960532 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:14:09.964532 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_MeasureRepository.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_publishMeasures.py
+-rw-r--r--   0 root         (0) root         (0)     5116 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_publishPictures.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_restServiceMeasures.py
+-rw-r--r--   0 root         (0) root         (0)    10155 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_restServicePictures.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_saveMeasures.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_sensorService.py
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-05 13:12:52.000000 ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/util.py
```

### Comparing `ch.zbindenonline.weatherstation-1.6.1/LICENSE` & `ch.zbindenonline.weatherstation-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/PKG-INFO` & `ch.zbindenonline.weatherstation-1.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: ch.zbindenonline.weatherstation
-Version: 1.6.1
+Version: 1.7.0
 Summary: Collects data from tinkerforge outdoor weather station and saves it to sqlite database.
-Home-page: UNKNOWN
 Author: Patrick Zbinden
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 License-File: LICENSE
 
 # HomeMeasurement
 source env/bin/activate deactivate
 
@@ -19,8 +17,7 @@
 rm -Rf dist
 
 python3 setup.py sdist bdist_wheel
 
 python3 -m pip install --user --upgrade twine
 
 python3 -m twine upload dist/*
-
```

### Comparing `ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/config.py` & `ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/config.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/measureRepository.py` & `ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/measureRepository.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/publishMeasures.py` & `ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/publishMeasures.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/publishPictures.py` & `ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/publishPictures.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/restServiceMeasures.py` & `ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/restServiceMeasures.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/restServicePictures.py` & `ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/restServicePictures.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/saveMeasures.py` & `ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/saveMeasures.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/ch/zbindenonline/weatherstation/sensorService.py` & `ch.zbindenonline.weatherstation-1.7.0/ch/zbindenonline/weatherstation/sensorService.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/ch.zbindenonline.weatherstation.egg-info/PKG-INFO` & `ch.zbindenonline.weatherstation-1.7.0/ch.zbindenonline.weatherstation.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: ch.zbindenonline.weatherstation
-Version: 1.6.1
+Version: 1.7.0
 Summary: Collects data from tinkerforge outdoor weather station and saves it to sqlite database.
-Home-page: UNKNOWN
 Author: Patrick Zbinden
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 License-File: LICENSE
 
 # HomeMeasurement
 source env/bin/activate deactivate
 
@@ -19,8 +17,7 @@
 rm -Rf dist
 
 python3 setup.py sdist bdist_wheel
 
 python3 -m pip install --user --upgrade twine
 
 python3 -m twine upload dist/*
-
```

### Comparing `ch.zbindenonline.weatherstation-1.6.1/ch.zbindenonline.weatherstation.egg-info/SOURCES.txt` & `ch.zbindenonline.weatherstation-1.7.0/ch.zbindenonline.weatherstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/setup.py` & `ch.zbindenonline.weatherstation-1.7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 try:
     long_description = open("README.md").read()
 except IOError:
     long_description = ""
 
 setup(
     name="ch.zbindenonline.weatherstation",
-    version="1.6.1",
+    version="1.7.0",
     description="Collects data from tinkerforge outdoor weather station and saves it to sqlite database.",
     license="MIT",
     author="Patrick Zbinden",
     packages=find_packages(),
     python_requires='>=3.10',
     install_requires=['requests', 'click', 'tinkerforge'],
     entry_points={
```

### Comparing `ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/mocks.py` & `ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/mocks.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_MeasureRepository.py` & `ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_MeasureRepository.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 import sqlite3
 import tempfile
 import unittest
 
 from ch.zbindenonline.weatherstation.domain import Measure
 from ch.zbindenonline.weatherstation.measureRepository import MeasureRepository
-from .util import date_time
+from tests.ch.zbindenonline.weatherstation.util import date_time
 
 
 def insert_test_data(database):
     conn = sqlite3.connect(database)
     with conn:
         conn.execute("INSERT INTO sensor(id, name) values(1, 'sensor_1')")
         conn.execute(
```

### Comparing `ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_config.py` & `ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_config.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_publishMeasures.py` & `ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_publishMeasures.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_publishPictures.py` & `ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_publishPictures.py`

 * *Files identical despite different names*

### Comparing `ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_restServiceMeasures.py` & `ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_restServiceMeasures.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pytest
 import requests
 from mockito import unstub, when, arg_that
 from requests import HTTPError, RequestException
 
 from ch.zbindenonline.weatherstation.restServiceMeasures import RestServiceMeasures
-from .mocks import MockResponse
+from tests.ch.zbindenonline.weatherstation.mocks import MockResponse
 
 
 class RestServiceMeasuresShould(unittest.TestCase):
 
     def tearDown(self):
         unstub()
 
@@ -24,34 +24,34 @@
 
     def test_login_ok(self):
         when(requests).post('http://testurl/login', data=any, headers=any, timeout=any).thenReturn(
             MockResponse(json_data={"access_jwt": "access_token"}))
 
         service = RestServiceMeasures('http://testurl', 'testuser', 'testpwd')
 
-        self.assertEquals('Bearer access_token', service.headers['Authorization'])
+        self.assertEqual('Bearer access_token', service.headers['Authorization'])
 
     def test_loginRequestException(self):
         when(requests).post('http://testurl/login', data=any, headers=any, timeout=any).thenRaise(
             RequestException('testmessage'))
 
         with self.assertRaises(SystemExit) as se:
             RestServiceMeasures('http://testurl', 'testuser', 'testpwd')
 
-        self.assertEquals(1, se.exception.code)
+        self.assertEqual(1, se.exception.code)
 
     def test_get_sensors(self):
         service = login()
         service_sensors = [{'id': 1, 'name': 'sensor_1'}, {'id': 2, 'name': 'sensor_2'}]
         when(requests).get('http://testurl/sensors', headers=any, timeout=10).thenReturn(
             MockResponse(json_data=service_sensors))
 
         sensors = service.get_sensors()
 
-        self.assertEquals(service_sensors, sensors)
+        self.assertEqual(service_sensors, sensors)
 
     def test_get_sensors_raise_for_status(self):
         service = login()
         when(requests).get('http://testurl/sensors', headers=any, timeout=10).thenReturn(
             MockResponse(status_code=400))
 
         with pytest.raises(HTTPError):
@@ -61,24 +61,24 @@
         service_timestamp = '2021-12-20 14:59'
         when(requests).get('http://testurl/measures/last?sensor=17', headers=any, timeout=10).thenReturn(
             MockResponse(json_data={'measured_at': service_timestamp}))
         service = login()
 
         timestamp = service.get_last_timestamp('17')
 
-        self.assertEquals(service_timestamp, timestamp)
+        self.assertEqual(service_timestamp, timestamp)
 
     def test_get_last_timestamp_defaults_to_1970(self):
         when(requests).get('http://testurl/measures/last?sensor=17', headers=any, timeout=10).thenReturn(
             MockResponse(json_data=None))
         service = login()
 
         timestamp = service.get_last_timestamp('17')
 
-        self.assertEquals('1970-01-01 00:00', timestamp)
+        self.assertEqual('1970-01-01 00:00', timestamp)
 
     def test_get_last_timestamp_raise_for_status(self):
         when(requests).get('http://testurl/measures/last?sensor=17', headers=any, timeout=10).thenReturn(
             MockResponse(status_code=400))
         service = login()
 
         with pytest.raises(HTTPError):
```

### Comparing `ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_restServicePictures.py` & `ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_restServicePictures.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
                                       '6',
                                       'client_id',
                                       'client_secret',
                                       'testuser',
                                       'testpwd')
         with self.assertRaises(SystemExit) as se:
             service.login()
-        self.assertEquals(1, se.exception.code)
+        self.assertEqual(1, se.exception.code)
 
     def test_logout_ok(self):
         when(requests).delete('http://testurl/oauth/token',
                               headers={'User-Agent': 'python', 'Accept': 'application/json'}, timeout=15).thenReturn(
             MockResponse('', 200, True))
         service = RestServicePictures('http://testurl',
                                       '6',
```

### Comparing `ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_saveMeasures.py` & `ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_saveMeasures.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import unittest
 
 from mockito import mock, unstub, when
 
 from ch.zbindenonline.weatherstation.domain import Measure
 from ch.zbindenonline.weatherstation.measureRepository import MeasureRepository
 from ch.zbindenonline.weatherstation.saveMeasures import Main
-from .util import date_time
+from tests.ch.zbindenonline.weatherstation.util import date_time
 
 
 class SaveMeasuresTest(unittest.TestCase):
 
     def setUp(self):
         config_sensors = {'87': {'name': 'aussen'}}
         self.test_dir = tempfile.mkdtemp()
```

### Comparing `ch.zbindenonline.weatherstation-1.6.1/tests/ch/zbindenonline/weatherstation/test_sensorService.py` & `ch.zbindenonline.weatherstation-1.7.0/tests/ch/zbindenonline/weatherstation/test_sensorService.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         when(ow_bricklet).get_sensor_identifiers().thenReturn([7, 19])
         when(ow_bricklet).get_sensor_data(7).thenReturn(SensorData(237, 65))
         when(ow_bricklet).get_sensor_data(19).thenReturn(SensorData(65, 87))
         service = TestSensorService(outdoor_weather_uid, testhost, testport, ip_connection, ow_bricklet)
 
         measures = service.get_measures()
 
-        self.assertEquals(2, len(measures))
+        self.assertEqual(2, len(measures))
         self.assertEqual(23.7, measures[0].temperature)
         self.assertEqual(65, measures[0].humidity)
         self.assertEqual(6.5, measures[1].temperature)
         self.assertEqual(87, measures[1].humidity)
 
     def test_getMeasuresNotOlderThan20Minutes(self):
         testhost = 'testhost'
@@ -68,15 +68,15 @@
         when(ow_bricklet).get_sensor_data(7).thenReturn(SensorData(237, 65, 1200))
         when(ow_bricklet).get_sensor_data(23).thenReturn(SensorData(110, 43, 1199))
         service = TestSensorService(outdoor_weather_uid, testhost, testport, ip_connection, ow_bricklet,
                                     datetime(2022, 1, 6, 14, 23, 0))
 
         measures = service.get_measures()
 
-        self.assertEquals(1, len(measures))
+        self.assertEqual(1, len(measures))
         self.assertEqual(11.0, measures[0].temperature)
         self.assertEqual(43, measures[0].humidity)
         self.assertEqual(datetime(2022, 1, 6, 14, 3, 1), measures[0].measured_at)
 
 
 if __name__ == '__main__':
     unittest.main()
```

