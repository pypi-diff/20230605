# Comparing `tmp/fire_opal-5.2.1.tar.gz` & `tmp/fire_opal-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fire_opal-5.2.1.tar", max compression
+gzip compressed data, was "fire_opal-5.2.2.tar", max compression
```

## Comparing `fire_opal-5.2.1.tar` & `fire_opal-5.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    36653 2023-05-23 22:28:06.351850 fire_opal-5.2.1/LICENSE
--rw-r--r--   0        0        0      524 2023-05-23 22:28:06.351850 fire_opal-5.2.1/README.md
--rw-r--r--   0        0        0      743 2023-05-23 22:28:25.419901 fire_opal-5.2.1/fireopal/__init__.py
--rw-r--r--   0        0        0      697 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/admin.py
--rw-r--r--   0        0        0     3298 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/config.py
--rw-r--r--   0        0        0      869 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/constants.py
--rw-r--r--   0        0        0      891 2023-05-23 22:28:25.419901 fire_opal-5.2.1/fireopal/functions/__init__.py
--rw-r--r--   0        0        0      818 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/base.py
--rw-r--r--   0        0        0     1478 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/benchmark.py
--rw-r--r--   0        0        0     2711 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/create_calibration_data.py
--rw-r--r--   0        0        0     1435 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/create_mitigation_data.py
--rw-r--r--   0        0        0     1826 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/execute.py
--rw-r--r--   0        0        0     1140 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/read_data.py
--rw-r--r--   0        0        0     1063 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/show_supported_devices.py
--rw-r--r--   0        0        0     2247 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/solve_qaoa.py
--rw-r--r--   0        0        0     1643 2023-05-23 22:28:06.351850 fire_opal-5.2.1/fireopal/functions/validate.py
--rw-r--r--   0        0        0     2740 2023-05-23 22:28:25.411901 fire_opal-5.2.1/pyproject.toml
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 fire_opal-5.2.1/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-06-05 06:17:36.114984 fire_opal-5.2.2/LICENSE
+-rw-r--r--   0        0        0      524 2023-06-05 06:17:36.114984 fire_opal-5.2.2/README.md
+-rw-r--r--   0        0        0      743 2023-06-05 06:17:54.407271 fire_opal-5.2.2/fireopal/__init__.py
+-rw-r--r--   0        0        0      697 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/admin.py
+-rw-r--r--   0        0        0     3298 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/config.py
+-rw-r--r--   0        0        0      869 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/constants.py
+-rw-r--r--   0        0        0      891 2023-06-05 06:17:54.407271 fire_opal-5.2.2/fireopal/functions/__init__.py
+-rw-r--r--   0        0        0      818 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/base.py
+-rw-r--r--   0        0        0     1478 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/benchmark.py
+-rw-r--r--   0        0        0     2711 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/create_calibration_data.py
+-rw-r--r--   0        0        0     1435 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/create_mitigation_data.py
+-rw-r--r--   0        0        0     1826 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/execute.py
+-rw-r--r--   0        0        0     1140 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/read_data.py
+-rw-r--r--   0        0        0     1063 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/show_supported_devices.py
+-rw-r--r--   0        0        0     2247 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/solve_qaoa.py
+-rw-r--r--   0        0        0     1643 2023-06-05 06:17:36.114984 fire_opal-5.2.2/fireopal/functions/validate.py
+-rw-r--r--   0        0        0     2740 2023-06-05 06:17:54.399271 fire_opal-5.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 fire_opal-5.2.2/PKG-INFO
```

### Comparing `fire_opal-5.2.1/LICENSE` & `fire_opal-5.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/README.md` & `fire_opal-5.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/__init__.py` & `fire_opal-5.2.2/fireopal/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/admin.py` & `fire_opal-5.2.2/fireopal/admin.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/config.py` & `fire_opal-5.2.2/fireopal/config.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/constants.py` & `fire_opal-5.2.2/fireopal/constants.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/functions/__init__.py` & `fire_opal-5.2.2/fireopal/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/functions/base.py` & `fire_opal-5.2.2/fireopal/functions/base.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/functions/benchmark.py` & `fire_opal-5.2.2/fireopal/functions/benchmark.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/functions/create_calibration_data.py` & `fire_opal-5.2.2/fireopal/functions/create_calibration_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/functions/create_mitigation_data.py` & `fire_opal-5.2.2/fireopal/functions/create_mitigation_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/functions/execute.py` & `fire_opal-5.2.2/fireopal/functions/execute.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/functions/read_data.py` & `fire_opal-5.2.2/fireopal/functions/read_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/functions/show_supported_devices.py` & `fire_opal-5.2.2/fireopal/functions/show_supported_devices.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/functions/solve_qaoa.py` & `fire_opal-5.2.2/fireopal/functions/solve_qaoa.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/fireopal/functions/validate.py` & `fire_opal-5.2.2/fireopal/functions/validate.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.2.1/pyproject.toml` & `fire_opal-5.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fire-opal"
-version = "5.2.1"
+version = "5.2.2"
 description = "Fire Opal Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
```

### Comparing `fire_opal-5.2.1/PKG-INFO` & `fire_opal-5.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fire-opal
-Version: 5.2.1
+Version: 5.2.2
 Summary: Fire Opal Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

