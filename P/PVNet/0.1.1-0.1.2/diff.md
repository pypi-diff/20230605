# Comparing `tmp/PVNet-0.1.1.tar.gz` & `tmp/PVNet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-0.1.1.tar", last modified: Mon Jun  5 15:31:05 2023, max compression
+gzip compressed data, was "PVNet-0.1.2.tar", last modified: Mon Jun  5 16:07:41 2023, max compression
```

## Comparing `PVNet-0.1.1.tar` & `PVNet-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:31:05.057915 PVNet-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 15:30:51.000000 PVNet-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 15:30:51.000000 PVNet-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 15:31:05.057915 PVNet-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:31:05.057915 PVNet-0.1.1/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 15:31:05.000000 PVNet-0.1.1/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-05 15:31:05.000000 PVNet-0.1.1/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:31:05.000000 PVNet-0.1.1/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 15:31:05.000000 PVNet-0.1.1/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 15:31:05.000000 PVNet-0.1.1/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-05 15:30:51.000000 PVNet-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:31:05.057915 PVNet-0.1.1/pvnet/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 15:30:51.000000 PVNet-0.1.1/pvnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-05 15:30:51.000000 PVNet-0.1.1/pvnet/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-05 15:30:51.000000 PVNet-0.1.1/pvnet/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-05 15:30:51.000000 PVNet-0.1.1/pvnet/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-05 15:30:51.000000 PVNet-0.1.1/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-05 15:30:51.000000 PVNet-0.1.1/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-05 15:30:51.000000 PVNet-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-05 15:30:51.000000 PVNet-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 15:30:51.000000 PVNet-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:31:05.057915 PVNet-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-05 15:30:51.000000 PVNet-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:31:05.057915 PVNet-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:30:51.000000 PVNet-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-05 15:30:51.000000 PVNet-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-05 15:30:51.000000 PVNet-0.1.1/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:07:41.785820 PVNet-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 16:07:29.000000 PVNet-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 16:07:29.000000 PVNet-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 16:07:41.785820 PVNet-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:07:41.785820 PVNet-0.1.2/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 16:07:41.000000 PVNet-0.1.2/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-05 16:07:41.000000 PVNet-0.1.2/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:07:41.000000 PVNet-0.1.2/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 16:07:41.000000 PVNet-0.1.2/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 16:07:41.000000 PVNet-0.1.2/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-05 16:07:29.000000 PVNet-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:07:41.785820 PVNet-0.1.2/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-05 16:07:29.000000 PVNet-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-05 16:07:29.000000 PVNet-0.1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-05 16:07:29.000000 PVNet-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:07:41.785820 PVNet-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-05 16:07:29.000000 PVNet-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:07:41.785820 PVNet-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:07:29.000000 PVNet-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-05 16:07:29.000000 PVNet-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-05 16:07:29.000000 PVNet-0.1.2/tests/test_app.py
```

### Comparing `PVNet-0.1.1/LICENSE` & `PVNet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.1/PKG-INFO` & `PVNet-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 0.1.1
+Version: 0.1.2
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-0.1.1/PVNet.egg-info/PKG-INFO` & `PVNet-0.1.2/PVNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 0.1.1
+Version: 0.1.2
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-0.1.1/README.md` & `PVNet-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.1/pvnet/app.py` & `PVNet-0.1.2/pvnet/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         )
 
         forecasts.append(forecast)
 
     return forecasts
 
 
-def app(t0=None, apply_adjuster=False, gsp_ids=gsp_ids, write_predictions=True):
+def app(t0=None, apply_adjuster=True, gsp_ids=gsp_ids, write_predictions=True):
     """Inference function for production
 
     This app expects these evironmental variables to be available:
         - DB_URL
         - NWP_ZARR_PATH
         - SATELLITE_ZARR_PATH
     Args:
```

### Comparing `PVNet-0.1.1/pvnet/callbacks.py` & `PVNet-0.1.2/pvnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.1/pvnet/optimizers.py` & `PVNet-0.1.2/pvnet/optimizers.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.1/pvnet/training.py` & `PVNet-0.1.2/pvnet/training.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.1/pvnet/utils.py` & `PVNet-0.1.2/pvnet/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.1/setup.py` & `PVNet-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.1/tests/conftest.py` & `PVNet-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.1/tests/test_app.py` & `PVNet-0.1.2/tests/test_app.py`

 * *Files identical despite different names*

