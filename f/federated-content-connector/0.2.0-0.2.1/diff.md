# Comparing `tmp/federated-content-connector-0.2.0.tar.gz` & `tmp/federated-content-connector-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "federated-content-connector-0.2.0.tar", last modified: Wed May 31 15:40:03 2023, max compression
+gzip compressed data, was "federated-content-connector-0.2.1.tar", last modified: Mon Jun  5 16:00:23 2023, max compression
```

## Comparing `federated-content-connector-0.2.0.tar` & `federated-content-connector-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:40:03.569457 federated-content-connector-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)      808 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-05-31 15:40:03.569457 federated-content-connector-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:40:03.565457 federated-content-connector-0.2.0/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:40:03.565457 federated-content-connector-0.2.0/federated_content_connector/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/filters/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:40:03.565457 federated-content-connector-0.2.0/federated_content_connector/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:40:03.561457 federated-content-connector-0.2.0/federated_content_connector/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:40:03.565457 federated-content-connector-0.2.0/federated_content_connector/templates/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/templates/federated_content_connector/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/federated_content_connector/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:40:03.565457 federated-content-connector-0.2.0/federated_content_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-05-31 15:40:03.000000 federated-content-connector-0.2.0/federated_content_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-05-31 15:40:03.000000 federated-content-connector-0.2.0/federated_content_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 15:40:03.000000 federated-content-connector-0.2.0/federated_content_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-31 15:40:03.000000 federated-content-connector-0.2.0/federated_content_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 15:40:03.000000 federated-content-connector-0.2.0/federated_content_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-31 15:40:03.000000 federated-content-connector-0.2.0/federated_content_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-31 15:40:03.000000 federated-content-connector-0.2.0/federated_content_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:40:03.565457 federated-content-connector-0.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-31 15:40:03.569457 federated-content-connector-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:40:03.569457 federated-content-connector-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-05-31 15:39:54.000000 federated-content-connector-0.2.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8226 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.068028 federated-content-connector-0.2.1/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/federated_content_connector/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/filters/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/federated_content_connector/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.068028 federated-content-connector-0.2.1/federated_content_connector/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/federated_content_connector/templates/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/templates/federated_content_connector/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/federated_content_connector/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/federated_content_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8226 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-05 16:00:23.000000 federated-content-connector-0.2.1/federated_content_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 16:00:23.072028 federated-content-connector-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-05 16:00:15.000000 federated-content-connector-0.2.1/tests/test_models.py
```

### Comparing `federated-content-connector-0.2.0/CHANGELOG.rst` & `federated-content-connector-0.2.1/CHANGELOG.rst`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+0.2.1 – 2023-06-5
+------------------
+* Fixed issue with product source data type
+
 0.2.0 – 2023-05-31
 ------------------
 * Added support for stage and prod landing pages via settings
 
 0.1.1 – 2023-05-26
 ------------------
 * Fixes for PyPI description markup.
```

### Comparing `federated-content-connector-0.2.0/LICENSE.txt` & `federated-content-connector-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.0/PKG-INFO` & `federated-content-connector-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 0.2.0
+Version: 0.2.1
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+0.2.1 – 2023-06-5
+------------------
+* Fixed issue with product source data type
+
 0.2.0 – 2023-05-31
 ------------------
 * Added support for stage and prod landing pages via settings
 
 0.1.1 – 2023-05-26
 ------------------
 * Fixes for PyPI description markup.
```

### Comparing `federated-content-connector-0.2.0/README.rst` & `federated-content-connector-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.0/federated_content_connector/apps.py` & `federated-content-connector-0.2.1/federated_content_connector/apps.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.0/federated_content_connector/filters/pipeline.py` & `federated-content-connector-0.2.1/federated_content_connector/filters/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,11 +29,12 @@
         Pipeline step that modifies the course home url for externally hosted courses
         """
         course_key_str = '{}+{}'.format(course_key.org, course_key.course)
         course_data = get_course_data(course_key_str, ['course_type', 'product_source'])
         if course_data:
             course_type = course_data.get('course_type')
             product_source = course_data.get('product_source')
-            if course_type == EXEC_ED_COURSE_TYPE and product_source == PRODUCT_SOURCE_2U:
+            product_source_slug = product_source['slug'] if isinstance(product_source, dict) else product_source
+            if course_type == EXEC_ED_COURSE_TYPE and product_source_slug == PRODUCT_SOURCE_2U:
                 course_home_url = getattr(settings, 'EXEC_ED_LANDING_PAGE', EXEC_ED_LANDING_PAGE)
 
         return {'course_key': course_key, 'course_home_url': course_home_url}
```

### Comparing `federated-content-connector-0.2.0/federated_content_connector/templates/federated_content_connector/base.html` & `federated-content-connector-0.2.1/federated_content_connector/templates/federated_content_connector/base.html`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.0/federated_content_connector.egg-info/PKG-INFO` & `federated-content-connector-0.2.1/federated_content_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 0.2.0
+Version: 0.2.1
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+0.2.1 – 2023-06-5
+------------------
+* Fixed issue with product source data type
+
 0.2.0 – 2023-05-31
 ------------------
 * Added support for stage and prod landing pages via settings
 
 0.1.1 – 2023-05-26
 ------------------
 * Fixes for PyPI description markup.
```

### Comparing `federated-content-connector-0.2.0/federated_content_connector.egg-info/SOURCES.txt` & `federated-content-connector-0.2.1/federated_content_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.0/requirements/constraints.txt` & `federated-content-connector-0.2.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-0.2.0/setup.py` & `federated-content-connector-0.2.1/setup.py`

 * *Files identical despite different names*

