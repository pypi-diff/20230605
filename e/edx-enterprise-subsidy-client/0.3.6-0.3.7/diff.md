# Comparing `tmp/edx-enterprise-subsidy-client-0.3.6.tar.gz` & `tmp/edx-enterprise-subsidy-client-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-subsidy-client-0.3.6.tar", last modified: Thu Jun  1 07:21:15 2023, max compression
+gzip compressed data, was "edx-enterprise-subsidy-client-0.3.7.tar", last modified: Mon Jun  5 14:03:18 2023, max compression
```

## Comparing `edx-enterprise-subsidy-client-0.3.6.tar` & `edx-enterprise-subsidy-client-0.3.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9179 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11665 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9179 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-01 07:21:15.000000 edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-01 07:21:15.539397 edx-enterprise-subsidy-client-0.3.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 07:21:15.535397 edx-enterprise-subsidy-client-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-06-01 07:21:10.000000 edx-enterprise-subsidy-client-0.3.6/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 14:03:18.840982 edx-enterprise-subsidy-client-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9259 2023-06-05 14:03:18.840982 edx-enterprise-subsidy-client-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 14:03:18.840982 edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11665 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 14:03:18.840982 edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9259 2023-06-05 14:03:18.000000 edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-06-05 14:03:18.000000 edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 14:03:18.000000 edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 14:03:18.000000 edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-05 14:03:18.000000 edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-05 14:03:18.000000 edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 14:03:18.840982 edx-enterprise-subsidy-client-0.3.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-05 14:03:18.844982 edx-enterprise-subsidy-client-0.3.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 14:03:18.840982 edx-enterprise-subsidy-client-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-06-05 14:03:14.000000 edx-enterprise-subsidy-client-0.3.7/tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.3.6/CHANGELOG.rst` & `edx-enterprise-subsidy-client-0.3.7/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
-[0.3.6]
+[0.3.7]
 *******
+* feat: upgrade many python dependencies, notably Django 3.2.19
 
+[0.3.6]
+*******
 * feat: pass idempotency key during transaction creation (pt. 2)
 
 [0.3.5]
 *******
 * feat: pass idempotency key during transaction creation
 
 [0.3.3]
```

### Comparing `edx-enterprise-subsidy-client-0.3.6/LICENSE` & `edx-enterprise-subsidy-client-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.6/LICENSE.txt` & `edx-enterprise-subsidy-client-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.6/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.6
+Version: 0.3.7
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,17 +223,20 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
-[0.3.6]
+[0.3.7]
 *******
+* feat: upgrade many python dependencies, notably Django 3.2.19
 
+[0.3.6]
+*******
 * feat: pass idempotency key during transaction creation (pt. 2)
 
 [0.3.5]
 *******
 * feat: pass idempotency key during transaction creation
 
 [0.3.3]
```

### Comparing `edx-enterprise-subsidy-client-0.3.6/README.rst` & `edx-enterprise-subsidy-client-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client/client.py` & `edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.6
+Version: 0.3.7
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,17 +223,20 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
-[0.3.6]
+[0.3.7]
 *******
+* feat: upgrade many python dependencies, notably Django 3.2.19
 
+[0.3.6]
+*******
 * feat: pass idempotency key during transaction creation (pt. 2)
 
 [0.3.5]
 *******
 * feat: pass idempotency key during transaction creation
 
 [0.3.3]
```

### Comparing `edx-enterprise-subsidy-client-0.3.6/edx_enterprise_subsidy_client.egg-info/SOURCES.txt` & `edx-enterprise-subsidy-client-0.3.7/edx_enterprise_subsidy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.6/requirements/constraints.txt` & `edx-enterprise-subsidy-client-0.3.7/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.6/setup.py` & `edx-enterprise-subsidy-client-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.6/tests/test_client.py` & `edx-enterprise-subsidy-client-0.3.7/tests/test_client.py`

 * *Files identical despite different names*

