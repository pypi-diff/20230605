# Comparing `tmp/qbwc-0.0.1.tar.gz` & `tmp/qbwc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbwc-0.0.1.tar", last modified: Mon Jun  5 01:08:45 2023, max compression
+gzip compressed data, was "qbwc-0.0.2.tar", last modified: Mon Jun  5 01:17:41 2023, max compression
```

## Comparing `qbwc-0.0.1.tar` & `qbwc-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:08:45.177012 qbwc-0.0.1/
--rw-r--r--   0 bill      (1000) bill      (1000)     1077 2023-05-08 15:41:29.000000 qbwc-0.0.1/LICENSE.md
--rw-r--r--   0 bill      (1000) bill      (1000)      103 2023-05-08 15:41:29.000000 qbwc-0.0.1/MANIFEST.in
--rw-r--r--   0 bill      (1000) bill      (1000)     1317 2023-06-05 01:08:45.177012 qbwc-0.0.1/PKG-INFO
--rw-r--r--   0 bill      (1000) bill      (1000)      500 2023-05-08 15:41:29.000000 qbwc-0.0.1/README.md
--rw-r--r--   0 bill      (1000) bill      (1000)      154 2023-06-04 17:36:14.000000 qbwc-0.0.1/pyproject.toml
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:08:45.177012 qbwc-0.0.1/qbwc/
--rw-r--r--   0 bill      (1000) bill      (1000)       43 2023-06-03 02:06:38.000000 qbwc-0.0.1/qbwc/__init__.py
--rw-r--r--   0 bill      (1000) bill      (1000)     1542 2023-06-04 23:43:17.000000 qbwc-0.0.1/qbwc/admin.py
--rw-r--r--   0 bill      (1000) bill      (1000)      918 2023-05-08 15:41:29.000000 qbwc-0.0.1/qbwc/app_settings.py
--rw-r--r--   0 bill      (1000) bill      (1000)      385 2023-05-08 15:41:29.000000 qbwc-0.0.1/qbwc/asgi.py
--rw-r--r--   0 bill      (1000) bill      (1000)      478 2023-06-04 00:23:39.000000 qbwc-0.0.1/qbwc/decorators.py
--rw-r--r--   0 bill      (1000) bill      (1000)      302 2023-06-04 18:11:46.000000 qbwc-0.0.1/qbwc/exceptions.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:08:45.177012 qbwc-0.0.1/qbwc/migrations/
--rw-r--r--   0 bill      (1000) bill      (1000)     6002 2023-06-05 00:30:04.000000 qbwc-0.0.1/qbwc/migrations/0001_initial.py
--rw-r--r--   0 bill      (1000) bill      (1000)        0 2023-06-05 00:30:04.000000 qbwc-0.0.1/qbwc/migrations/__init__.py
--rw-r--r--   0 bill      (1000) bill      (1000)    10200 2023-06-05 01:01:53.000000 qbwc-0.0.1/qbwc/models.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:08:45.177012 qbwc-0.0.1/qbwc/parser/
--rw-r--r--   0 bill      (1000) bill      (1000)      209 2023-06-04 21:51:28.000000 qbwc-0.0.1/qbwc/parser/__init__.py
--rw-r--r--   0 bill      (1000) bill      (1000)     1012 2023-06-05 01:01:53.000000 qbwc-0.0.1/qbwc/parser/parser.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:08:45.177012 qbwc-0.0.1/qbwc/templates/
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:08:45.177012 qbwc-0.0.1/qbwc/templates/qbwc/
--rw-r--r--   0 bill      (1000) bill      (1000)      426 2023-05-08 15:41:29.000000 qbwc-0.0.1/qbwc/templates/qbwc/support.html
--rw-r--r--   0 bill      (1000) bill      (1000)      484 2023-05-08 15:41:29.000000 qbwc-0.0.1/qbwc/urls.py
--rw-r--r--   0 bill      (1000) bill      (1000)        0 2023-06-04 00:20:12.000000 qbwc-0.0.1/qbwc/utils.py
--rw-r--r--   0 bill      (1000) bill      (1000)     8577 2023-06-05 01:01:53.000000 qbwc-0.0.1/qbwc/views.py
--rw-r--r--   0 bill      (1000) bill      (1000)      385 2023-05-08 15:41:29.000000 qbwc-0.0.1/qbwc/wsgi.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:08:45.177012 qbwc-0.0.1/qbwc.egg-info/
--rw-r--r--   0 bill      (1000) bill      (1000)     1317 2023-06-05 01:08:45.000000 qbwc-0.0.1/qbwc.egg-info/PKG-INFO
--rw-r--r--   0 bill      (1000) bill      (1000)      631 2023-06-05 01:08:45.000000 qbwc-0.0.1/qbwc.egg-info/SOURCES.txt
--rw-r--r--   0 bill      (1000) bill      (1000)        1 2023-06-05 01:08:45.000000 qbwc-0.0.1/qbwc.egg-info/dependency_links.txt
--rw-r--r--   0 bill      (1000) bill      (1000)       38 2023-06-05 01:08:45.000000 qbwc-0.0.1/qbwc.egg-info/requires.txt
--rw-r--r--   0 bill      (1000) bill      (1000)       11 2023-06-05 01:08:45.000000 qbwc-0.0.1/qbwc.egg-info/top_level.txt
--rw-r--r--   0 bill      (1000) bill      (1000)      865 2023-06-05 01:08:45.177012 qbwc-0.0.1/setup.cfg
--rw-r--r--   0 bill      (1000) bill      (1000)       38 2023-05-08 15:41:29.000000 qbwc-0.0.1/setup.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:08:45.177012 qbwc-0.0.1/tests/
--rw-r--r--   0 bill      (1000) bill      (1000)      154 2023-06-04 18:11:46.000000 qbwc-0.0.1/tests/__init__.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:08:45.177012 qbwc-0.0.1/tests/test_data/
--rw-r--r--   0 bill      (1000) bill      (1000)        0 2023-06-04 17:39:47.000000 qbwc-0.0.1/tests/test_data/__init__.py
--rw-r--r--   0 bill      (1000) bill      (1000)     2772 2023-06-04 21:21:33.000000 qbwc-0.0.1/tests/test_query_parser.py
--rw-r--r--   0 bill      (1000) bill      (1000)      142 2023-06-04 18:11:46.000000 qbwc-0.0.1/tests/test_tasks.py
--rw-r--r--   0 bill      (1000) bill      (1000)      587 2023-06-04 18:11:46.000000 qbwc-0.0.1/tests/test_tickets.py
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:17:41.117012 qbwc-0.0.2/
+-rw-r--r--   0 bill      (1000) bill      (1000)     1077 2023-05-08 15:41:29.000000 qbwc-0.0.2/LICENSE.md
+-rw-r--r--   0 bill      (1000) bill      (1000)      103 2023-05-08 15:41:29.000000 qbwc-0.0.2/MANIFEST.in
+-rw-r--r--   0 bill      (1000) bill      (1000)     1638 2023-06-05 01:17:41.117012 qbwc-0.0.2/PKG-INFO
+-rw-r--r--   0 bill      (1000) bill      (1000)      821 2023-06-05 01:16:26.000000 qbwc-0.0.2/README.md
+-rw-r--r--   0 bill      (1000) bill      (1000)      154 2023-06-04 17:36:14.000000 qbwc-0.0.2/pyproject.toml
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:17:41.117012 qbwc-0.0.2/qbwc/
+-rw-r--r--   0 bill      (1000) bill      (1000)       43 2023-06-03 02:06:38.000000 qbwc-0.0.2/qbwc/__init__.py
+-rw-r--r--   0 bill      (1000) bill      (1000)     1542 2023-06-04 23:43:17.000000 qbwc-0.0.2/qbwc/admin.py
+-rw-r--r--   0 bill      (1000) bill      (1000)      918 2023-05-08 15:41:29.000000 qbwc-0.0.2/qbwc/app_settings.py
+-rw-r--r--   0 bill      (1000) bill      (1000)      385 2023-05-08 15:41:29.000000 qbwc-0.0.2/qbwc/asgi.py
+-rw-r--r--   0 bill      (1000) bill      (1000)      478 2023-06-04 00:23:39.000000 qbwc-0.0.2/qbwc/decorators.py
+-rw-r--r--   0 bill      (1000) bill      (1000)      302 2023-06-04 18:11:46.000000 qbwc-0.0.2/qbwc/exceptions.py
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:17:41.117012 qbwc-0.0.2/qbwc/migrations/
+-rw-r--r--   0 bill      (1000) bill      (1000)     6002 2023-06-05 00:30:04.000000 qbwc-0.0.2/qbwc/migrations/0001_initial.py
+-rw-r--r--   0 bill      (1000) bill      (1000)        0 2023-06-05 00:30:04.000000 qbwc-0.0.2/qbwc/migrations/__init__.py
+-rw-r--r--   0 bill      (1000) bill      (1000)    10200 2023-06-05 01:01:53.000000 qbwc-0.0.2/qbwc/models.py
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:17:41.117012 qbwc-0.0.2/qbwc/parser/
+-rw-r--r--   0 bill      (1000) bill      (1000)      209 2023-06-04 21:51:28.000000 qbwc-0.0.2/qbwc/parser/__init__.py
+-rw-r--r--   0 bill      (1000) bill      (1000)     1012 2023-06-05 01:01:53.000000 qbwc-0.0.2/qbwc/parser/parser.py
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:17:41.107012 qbwc-0.0.2/qbwc/templates/
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:17:41.117012 qbwc-0.0.2/qbwc/templates/qbwc/
+-rw-r--r--   0 bill      (1000) bill      (1000)      426 2023-05-08 15:41:29.000000 qbwc-0.0.2/qbwc/templates/qbwc/support.html
+-rw-r--r--   0 bill      (1000) bill      (1000)      484 2023-05-08 15:41:29.000000 qbwc-0.0.2/qbwc/urls.py
+-rw-r--r--   0 bill      (1000) bill      (1000)        0 2023-06-04 00:20:12.000000 qbwc-0.0.2/qbwc/utils.py
+-rw-r--r--   0 bill      (1000) bill      (1000)     8577 2023-06-05 01:01:53.000000 qbwc-0.0.2/qbwc/views.py
+-rw-r--r--   0 bill      (1000) bill      (1000)      385 2023-05-08 15:41:29.000000 qbwc-0.0.2/qbwc/wsgi.py
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:17:41.117012 qbwc-0.0.2/qbwc.egg-info/
+-rw-r--r--   0 bill      (1000) bill      (1000)     1638 2023-06-05 01:17:41.000000 qbwc-0.0.2/qbwc.egg-info/PKG-INFO
+-rw-r--r--   0 bill      (1000) bill      (1000)      631 2023-06-05 01:17:41.000000 qbwc-0.0.2/qbwc.egg-info/SOURCES.txt
+-rw-r--r--   0 bill      (1000) bill      (1000)        1 2023-06-05 01:17:41.000000 qbwc-0.0.2/qbwc.egg-info/dependency_links.txt
+-rw-r--r--   0 bill      (1000) bill      (1000)       38 2023-06-05 01:17:41.000000 qbwc-0.0.2/qbwc.egg-info/requires.txt
+-rw-r--r--   0 bill      (1000) bill      (1000)       11 2023-06-05 01:17:41.000000 qbwc-0.0.2/qbwc.egg-info/top_level.txt
+-rw-r--r--   0 bill      (1000) bill      (1000)      865 2023-06-05 01:17:41.117012 qbwc-0.0.2/setup.cfg
+-rw-r--r--   0 bill      (1000) bill      (1000)       38 2023-05-08 15:41:29.000000 qbwc-0.0.2/setup.py
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:17:41.117012 qbwc-0.0.2/tests/
+-rw-r--r--   0 bill      (1000) bill      (1000)      154 2023-06-04 18:11:46.000000 qbwc-0.0.2/tests/__init__.py
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-06-05 01:17:41.117012 qbwc-0.0.2/tests/test_data/
+-rw-r--r--   0 bill      (1000) bill      (1000)        0 2023-06-04 17:39:47.000000 qbwc-0.0.2/tests/test_data/__init__.py
+-rw-r--r--   0 bill      (1000) bill      (1000)     2772 2023-06-04 21:21:33.000000 qbwc-0.0.2/tests/test_query_parser.py
+-rw-r--r--   0 bill      (1000) bill      (1000)      142 2023-06-04 18:11:46.000000 qbwc-0.0.2/tests/test_tasks.py
+-rw-r--r--   0 bill      (1000) bill      (1000)      587 2023-06-04 18:11:46.000000 qbwc-0.0.2/tests/test_tickets.py
```

### Comparing `qbwc-0.0.1/LICENSE.md` & `qbwc-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `qbwc-0.0.1/PKG-INFO` & `qbwc-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbwc
-Version: 0.0.1
+Version: 0.0.2
 Summary: QuickBooks Desktop Webconnector Implementation
 Home-page: https://www.github.com/bill-ash/qbwc
 Author: Bill Ash
 Author-email: bill@overco.net
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -17,30 +17,35 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.9
 License-File: LICENSE.md
 
-## Quickbooks Desktop Webconnector (qbwc)
+## QBWC: Quickbooks Desktop Webconnector 
 
-Django package for syncing and transferring data with external databases via the 
-Quickbooks Webconnector (QBWC). 
+**Experimental**
 
-Implementation includes transfer services for: 
+Django package for syncing data between django application and 
+QuickBooks Desktop via the Quickbooks Webconnector (QBWC). 
+
+Implementation includes transfer services (push, pull, re-sync) for: 
 
 - gl accounts  
 - other name list
-- expenses (credit card transactions)
+- expenses (credit card charges)
+- customers 
+- credit cards 
+- vendors
 
 Road map: 
 
-- bills
-- customers 
-
+- vendor bills
+- journal entries
+- QuickBooks Reports 
 
 ## Installation 
 
 Install the latest development version from github using: 
 
 ```
 pip install git+https://github.com/bill-ash/qbwc
@@ -49,12 +54,16 @@
 or from pypi: 
 
 ```
 pip install qbwc
 ```
 
 
+## Example 
+
+Example directory includes application with sample apps for each of the entites mentioned above. 
 
+Repeated patterns will be abstracted in the `BaseObjectMixin` model and are likely to change.
```

### Comparing `qbwc-0.0.1/qbwc/admin.py` & `qbwc-0.0.2/qbwc/admin.py`

 * *Files identical despite different names*

### Comparing `qbwc-0.0.1/qbwc/app_settings.py` & `qbwc-0.0.2/qbwc/app_settings.py`

 * *Files identical despite different names*

### Comparing `qbwc-0.0.1/qbwc/migrations/0001_initial.py` & `qbwc-0.0.2/qbwc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `qbwc-0.0.1/qbwc/models.py` & `qbwc-0.0.2/qbwc/models.py`

 * *Files identical despite different names*

### Comparing `qbwc-0.0.1/qbwc/parser/parser.py` & `qbwc-0.0.2/qbwc/parser/parser.py`

 * *Files identical despite different names*

### Comparing `qbwc-0.0.1/qbwc/views.py` & `qbwc-0.0.2/qbwc/views.py`

 * *Files identical despite different names*

### Comparing `qbwc-0.0.1/qbwc.egg-info/PKG-INFO` & `qbwc-0.0.2/qbwc.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbwc
-Version: 0.0.1
+Version: 0.0.2
 Summary: QuickBooks Desktop Webconnector Implementation
 Home-page: https://www.github.com/bill-ash/qbwc
 Author: Bill Ash
 Author-email: bill@overco.net
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -17,30 +17,35 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.9
 License-File: LICENSE.md
 
-## Quickbooks Desktop Webconnector (qbwc)
+## QBWC: Quickbooks Desktop Webconnector 
 
-Django package for syncing and transferring data with external databases via the 
-Quickbooks Webconnector (QBWC). 
+**Experimental**
 
-Implementation includes transfer services for: 
+Django package for syncing data between django application and 
+QuickBooks Desktop via the Quickbooks Webconnector (QBWC). 
+
+Implementation includes transfer services (push, pull, re-sync) for: 
 
 - gl accounts  
 - other name list
-- expenses (credit card transactions)
+- expenses (credit card charges)
+- customers 
+- credit cards 
+- vendors
 
 Road map: 
 
-- bills
-- customers 
-
+- vendor bills
+- journal entries
+- QuickBooks Reports 
 
 ## Installation 
 
 Install the latest development version from github using: 
 
 ```
 pip install git+https://github.com/bill-ash/qbwc
@@ -49,12 +54,16 @@
 or from pypi: 
 
 ```
 pip install qbwc
 ```
 
 
+## Example 
+
+Example directory includes application with sample apps for each of the entites mentioned above. 
 
+Repeated patterns will be abstracted in the `BaseObjectMixin` model and are likely to change.
```

### Comparing `qbwc-0.0.1/qbwc.egg-info/SOURCES.txt` & `qbwc-0.0.2/qbwc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbwc-0.0.1/setup.cfg` & `qbwc-0.0.2/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qbwc
-version = 0.0.1
+version = 0.0.2
 description = QuickBooks Desktop Webconnector Implementation
 long_description = file:README.md
 url = https://www.github.com/bill-ash/qbwc
 author = Bill Ash
 author_email = bill@overco.net
 license = MIT
 classifiers =
```

### Comparing `qbwc-0.0.1/tests/test_query_parser.py` & `qbwc-0.0.2/tests/test_query_parser.py`

 * *Files identical despite different names*

### Comparing `qbwc-0.0.1/tests/test_tickets.py` & `qbwc-0.0.2/tests/test_tickets.py`

 * *Files identical despite different names*

