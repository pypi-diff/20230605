# Comparing `tmp/toshiba-ac-0.3.2.tar.gz` & `tmp/toshiba-ac-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toshiba-ac-0.3.2.tar", last modified: Thu Mar  2 22:17:48 2023, max compression
+gzip compressed data, was "toshiba-ac-0.3.3.tar", last modified: Mon Jun  5 21:03:08 2023, max compression
```

## Comparing `toshiba-ac-0.3.2.tar` & `toshiba-ac-0.3.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:17:48.042574 toshiba-ac-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-02 22:17:48.042574 toshiba-ac-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-02 22:17:48.042574 toshiba-ac-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:17:48.042574 toshiba-ac-0.3.2/toshiba_ac/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/toshiba_ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-02 22:17:48.042574 toshiba-ac-0.3.2/toshiba_ac/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:17:48.042574 toshiba-ac-0.3.2/toshiba_ac/device/
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/toshiba_ac/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18311 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/toshiba_ac/device/fcu_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/toshiba_ac/device/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/toshiba_ac/device/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/toshiba_ac/device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:17:48.042574 toshiba-ac-0.3.2/toshiba_ac/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/toshiba_ac/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/toshiba_ac/utils/amqp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/toshiba_ac/utils/http_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:17:48.042574 toshiba-ac-0.3.2/toshiba_ac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-02 22:17:48.000000 toshiba-ac-0.3.2/toshiba_ac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-02 22:17:48.000000 toshiba-ac-0.3.2/toshiba_ac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 22:17:48.000000 toshiba-ac-0.3.2/toshiba_ac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-02 22:17:48.000000 toshiba-ac-0.3.2/toshiba_ac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-02 22:17:48.000000 toshiba-ac-0.3.2/toshiba_ac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    79711 2023-03-02 22:17:47.000000 toshiba-ac-0.3.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:03:08.942465 toshiba-ac-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-05 21:03:08.942465 toshiba-ac-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-05 21:03:08.942465 toshiba-ac-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:03:08.942465 toshiba-ac-0.3.3/toshiba_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/toshiba_ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-05 21:03:08.942465 toshiba-ac-0.3.3/toshiba_ac/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:03:08.938465 toshiba-ac-0.3.3/toshiba_ac/device/
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/toshiba_ac/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18311 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/toshiba_ac/device/fcu_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/toshiba_ac/device/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/toshiba_ac/device/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/toshiba_ac/device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:03:08.942465 toshiba-ac-0.3.3/toshiba_ac/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/toshiba_ac/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/toshiba_ac/utils/amqp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/toshiba_ac/utils/http_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:03:08.938465 toshiba-ac-0.3.3/toshiba_ac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-05 21:03:08.000000 toshiba-ac-0.3.3/toshiba_ac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-05 21:03:08.000000 toshiba-ac-0.3.3/toshiba_ac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:03:08.000000 toshiba-ac-0.3.3/toshiba_ac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 21:03:08.000000 toshiba-ac-0.3.3/toshiba_ac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 21:03:08.000000 toshiba-ac-0.3.3/toshiba_ac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    79711 2023-06-05 21:03:07.000000 toshiba-ac-0.3.3/versioneer.py
```

### Comparing `toshiba-ac-0.3.2/LICENSE.txt` & `toshiba-ac-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/PKG-INFO` & `toshiba-ac-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toshiba-ac
-Version: 0.3.2
+Version: 0.3.3
 Summary: Toshiba AC controller - allows to control Toshiba HVAC systems with WiFi
 Home-page: https://github.com/KaSroka/Toshiba-AC-control
 Author: Kamil Sroka
 Author-email: kamilsroka92@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/KaSroka/Toshiba-AC-control/issues
 Keywords: toshiba,ac,hvac
```

### Comparing `toshiba-ac-0.3.2/README.md` & `toshiba-ac-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/setup.cfg` & `toshiba-ac-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/toshiba_ac/device/__init__.py` & `toshiba-ac-0.3.3/toshiba_ac/device/__init__.py`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/toshiba_ac/device/fcu_state.py` & `toshiba-ac-0.3.3/toshiba_ac/device/fcu_state.py`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/toshiba_ac/device/features.py` & `toshiba-ac-0.3.3/toshiba_ac/device/features.py`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/toshiba_ac/device/properties.py` & `toshiba-ac-0.3.3/toshiba_ac/device/properties.py`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/toshiba_ac/device_manager.py` & `toshiba-ac-0.3.3/toshiba_ac/device_manager.py`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/toshiba_ac/utils/__init__.py` & `toshiba-ac-0.3.3/toshiba_ac/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/toshiba_ac/utils/amqp_api.py` & `toshiba-ac-0.3.3/toshiba_ac/utils/amqp_api.py`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/toshiba_ac/utils/http_api.py` & `toshiba-ac-0.3.3/toshiba_ac/utils/http_api.py`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/toshiba_ac.egg-info/PKG-INFO` & `toshiba-ac-0.3.3/toshiba_ac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toshiba-ac
-Version: 0.3.2
+Version: 0.3.3
 Summary: Toshiba AC controller - allows to control Toshiba HVAC systems with WiFi
 Home-page: https://github.com/KaSroka/Toshiba-AC-control
 Author: Kamil Sroka
 Author-email: kamilsroka92@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/KaSroka/Toshiba-AC-control/issues
 Keywords: toshiba,ac,hvac
```

### Comparing `toshiba-ac-0.3.2/toshiba_ac.egg-info/SOURCES.txt` & `toshiba-ac-0.3.3/toshiba_ac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toshiba-ac-0.3.2/versioneer.py` & `toshiba-ac-0.3.3/versioneer.py`

 * *Files identical despite different names*

