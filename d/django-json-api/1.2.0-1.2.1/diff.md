# Comparing `tmp/django-json-api-1.2.0.tar.gz` & `tmp/django-json-api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-json-api-1.2.0.tar", last modified: Fri Mar 24 11:14:42 2023, max compression
+gzip compressed data, was "django-json-api-1.2.1.tar", last modified: Mon Jun  5 14:09:50 2023, max compression
```

## Comparing `django-json-api-1.2.0.tar` & `django-json-api-1.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-24 11:14:42.654075 django-json-api-1.2.0/
--rw-r--r--   0 alex       (501) staff       (20)     1066 2023-01-18 16:50:13.000000 django-json-api-1.2.0/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)       44 2023-01-18 16:50:13.000000 django-json-api-1.2.0/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     5338 2023-03-24 11:14:42.653328 django-json-api-1.2.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     4846 2023-03-24 11:13:10.000000 django-json-api-1.2.0/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-24 11:14:42.614319 django-json-api-1.2.0/django_json_api/
--rw-r--r--   0 alex       (501) staff       (20)       41 2023-01-18 16:50:13.000000 django-json-api-1.2.0/django_json_api/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1353 2023-03-24 11:13:10.000000 django-json-api-1.2.0/django_json_api/base.py
--rw-r--r--   0 alex       (501) staff       (20)     4280 2023-03-24 10:06:22.000000 django-json-api-1.2.0/django_json_api/client.py
--rw-r--r--   0 alex       (501) staff       (20)     7113 2023-01-18 16:50:13.000000 django-json-api-1.2.0/django_json_api/django.py
--rw-r--r--   0 alex       (501) staff       (20)     4002 2023-01-18 16:50:13.000000 django-json-api-1.2.0/django_json_api/fields.py
--rw-r--r--   0 alex       (501) staff       (20)     8201 2023-03-24 11:13:10.000000 django-json-api-1.2.0/django_json_api/manager.py
--rw-r--r--   0 alex       (501) staff       (20)    10356 2023-01-18 16:50:13.000000 django-json-api-1.2.0/django_json_api/models.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-24 11:14:42.622222 django-json-api-1.2.0/django_json_api/resources/
--rw-r--r--   0 alex       (501) staff       (20)        6 2023-03-24 11:13:10.000000 django-json-api-1.2.0/django_json_api/resources/VERSION
--rw-r--r--   0 alex       (501) staff       (20)     4479 2023-01-18 16:50:13.000000 django-json-api-1.2.0/django_json_api/rest_framework.py
--rw-r--r--   0 alex       (501) staff       (20)      185 2023-01-18 16:50:13.000000 django-json-api-1.2.0/django_json_api/version.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-24 11:14:42.621277 django-json-api-1.2.0/django_json_api.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     5338 2023-03-24 11:14:42.000000 django-json-api-1.2.0/django_json_api.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      863 2023-03-24 11:14:42.000000 django-json-api-1.2.0/django_json_api.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-03-24 11:14:42.000000 django-json-api-1.2.0/django_json_api.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      500 2023-03-24 11:14:42.000000 django-json-api-1.2.0/django_json_api.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       22 2023-03-24 11:14:42.000000 django-json-api-1.2.0/django_json_api.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)      703 2023-01-18 16:50:13.000000 django-json-api-1.2.0/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)       86 2023-01-18 16:50:13.000000 django-json-api-1.2.0/requirements.txt
--rw-r--r--   0 alex       (501) staff       (20)      200 2023-01-18 16:50:13.000000 django-json-api-1.2.0/requirements_dev.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-03-24 11:14:42.654314 django-json-api-1.2.0/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     1258 2023-01-18 16:50:13.000000 django-json-api-1.2.0/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-24 11:14:42.648327 django-json-api-1.2.0/tests/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)       90 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/apps.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-24 11:14:42.652231 django-json-api-1.2.0/tests/migrations/
--rw-r--r--   0 alex       (501) staff       (20)     1030 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/migrations/0001_initial.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1969 2023-03-24 11:13:10.000000 django-json-api-1.2.0/tests/models.py
--rw-r--r--   0 alex       (501) staff       (20)      309 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/settings.py
--rw-r--r--   0 alex       (501) staff       (20)     8727 2023-03-24 10:06:22.000000 django-json-api-1.2.0/tests/test_client.py
--rw-r--r--   0 alex       (501) staff       (20)     4135 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/test_django.py
--rw-r--r--   0 alex       (501) staff       (20)     5973 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/test_fields.py
--rw-r--r--   0 alex       (501) staff       (20)    15770 2023-03-24 11:13:10.000000 django-json-api-1.2.0/tests/test_manager.py
--rw-r--r--   0 alex       (501) staff       (20)    20310 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/test_models.py
--rw-r--r--   0 alex       (501) staff       (20)     4597 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/test_rest_framework.py
--rw-r--r--   0 alex       (501) staff       (20)      809 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/test_version.py
--rw-r--r--   0 alex       (501) staff       (20)      566 2023-01-18 16:50:13.000000 django-json-api-1.2.0/tests/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-05 14:09:50.222684 django-json-api-1.2.1/
+-rw-r--r--   0 alex       (501) staff       (20)     1066 2023-01-18 16:50:13.000000 django-json-api-1.2.1/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)       44 2023-01-18 16:50:13.000000 django-json-api-1.2.1/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     5338 2023-06-05 14:09:50.222050 django-json-api-1.2.1/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     4846 2023-03-24 11:13:10.000000 django-json-api-1.2.1/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-05 14:09:50.188064 django-json-api-1.2.1/django_json_api/
+-rw-r--r--   0 alex       (501) staff       (20)       41 2023-01-18 16:50:13.000000 django-json-api-1.2.1/django_json_api/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1353 2023-03-24 11:13:10.000000 django-json-api-1.2.1/django_json_api/base.py
+-rw-r--r--   0 alex       (501) staff       (20)     4280 2023-03-24 10:06:22.000000 django-json-api-1.2.1/django_json_api/client.py
+-rw-r--r--   0 alex       (501) staff       (20)     7113 2023-01-18 16:50:13.000000 django-json-api-1.2.1/django_json_api/django.py
+-rw-r--r--   0 alex       (501) staff       (20)     4002 2023-01-18 16:50:13.000000 django-json-api-1.2.1/django_json_api/fields.py
+-rw-r--r--   0 alex       (501) staff       (20)     8288 2023-06-05 14:03:49.000000 django-json-api-1.2.1/django_json_api/manager.py
+-rw-r--r--   0 alex       (501) staff       (20)    10356 2023-01-18 16:50:13.000000 django-json-api-1.2.1/django_json_api/models.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-05 14:09:50.197197 django-json-api-1.2.1/django_json_api/resources/
+-rw-r--r--   0 alex       (501) staff       (20)        6 2023-06-05 14:03:49.000000 django-json-api-1.2.1/django_json_api/resources/VERSION
+-rw-r--r--   0 alex       (501) staff       (20)     4479 2023-01-18 16:50:13.000000 django-json-api-1.2.1/django_json_api/rest_framework.py
+-rw-r--r--   0 alex       (501) staff       (20)      185 2023-01-18 16:50:13.000000 django-json-api-1.2.1/django_json_api/version.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-05 14:09:50.196298 django-json-api-1.2.1/django_json_api.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     5338 2023-06-05 14:09:50.000000 django-json-api-1.2.1/django_json_api.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      863 2023-06-05 14:09:50.000000 django-json-api-1.2.1/django_json_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-05 14:09:50.000000 django-json-api-1.2.1/django_json_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)      500 2023-06-05 14:09:50.000000 django-json-api-1.2.1/django_json_api.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       22 2023-06-05 14:09:50.000000 django-json-api-1.2.1/django_json_api.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)      703 2023-01-18 16:50:13.000000 django-json-api-1.2.1/pyproject.toml
+-rw-r--r--   0 alex       (501) staff       (20)       86 2023-01-18 16:50:13.000000 django-json-api-1.2.1/requirements.txt
+-rw-r--r--   0 alex       (501) staff       (20)      200 2023-01-18 16:50:13.000000 django-json-api-1.2.1/requirements_dev.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-05 14:09:50.222865 django-json-api-1.2.1/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     1258 2023-01-18 16:50:13.000000 django-json-api-1.2.1/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-05 14:09:50.218946 django-json-api-1.2.1/tests/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)       90 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/apps.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-05 14:09:50.221336 django-json-api-1.2.1/tests/migrations/
+-rw-r--r--   0 alex       (501) staff       (20)     1030 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/migrations/0001_initial.py
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/migrations/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1969 2023-03-24 11:13:10.000000 django-json-api-1.2.1/tests/models.py
+-rw-r--r--   0 alex       (501) staff       (20)      309 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/settings.py
+-rw-r--r--   0 alex       (501) staff       (20)     8727 2023-03-24 10:06:22.000000 django-json-api-1.2.1/tests/test_client.py
+-rw-r--r--   0 alex       (501) staff       (20)     4135 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/test_django.py
+-rw-r--r--   0 alex       (501) staff       (20)     5973 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/test_fields.py
+-rw-r--r--   0 alex       (501) staff       (20)    15770 2023-03-24 11:13:10.000000 django-json-api-1.2.1/tests/test_manager.py
+-rw-r--r--   0 alex       (501) staff       (20)    20310 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/test_models.py
+-rw-r--r--   0 alex       (501) staff       (20)     4597 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/test_rest_framework.py
+-rw-r--r--   0 alex       (501) staff       (20)      809 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/test_version.py
+-rw-r--r--   0 alex       (501) staff       (20)      566 2023-01-18 16:50:13.000000 django-json-api-1.2.1/tests/utils.py
```

### Comparing `django-json-api-1.2.0/LICENSE` & `django-json-api-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/PKG-INFO` & `django-json-api-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-json-api
-Version: 1.2.0
+Version: 1.2.1
 Summary: JSON API specification for Django services
 Home-page: https://github.com/share-work/django-json-api
 Author: Sharework
 Author-email: root@sharework.co
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-json-api-1.2.0/README.md` & `django-json-api-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/django_json_api/base.py` & `django-json-api-1.2.1/django_json_api/base.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/django_json_api/client.py` & `django-json-api-1.2.1/django_json_api/client.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/django_json_api/django.py` & `django-json-api-1.2.1/django_json_api/django.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/django_json_api/fields.py` & `django-json-api-1.2.1/django_json_api/fields.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/django_json_api/manager.py` & `django-json-api-1.2.1/django_json_api/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,27 @@
         base, *nested_path = lookup.split("__", 1)
         base_lookup_to_nested_lookups[base].extend(nested_path)
     return base_lookup_to_nested_lookups
 
 
 class JSONAPIManager:
     def __init__(self, model, **kwargs):
-        self.client = JSONAPIClient(auth=model._meta.auth)
         self.model = model
+        self.client = self._get_client()
         self._fields = kwargs.get("fields", {})
         self._prefetch_related = kwargs.get("prefetch_related", [])
         self._include = kwargs.get("include", [])
         self._include = sorted(list(set(self._include) | self._prepared_prefetch_for_include))
         self._filters = kwargs.get("filters", {})
         self._sort = kwargs.get("sort", [])
         self._cache = None
 
+    def _get_client(self) -> JSONAPIClient:
+        return JSONAPIClient(auth=self.model._meta.auth)
+
     def modify(self, **kwargs) -> "JSONAPIManager":
         _fields = {
             **self._fields,
             **kwargs.get("fields", {}),
         }
         _filters = {
             **self._filters,
@@ -81,15 +84,15 @@
             filters=self._filters,
             include=self._include or None,
             fields=self._fields,
             sort=self._sort,
         )
 
     def _fetch_iterate(self) -> Iterator:
-        client = JSONAPIClient()
+        client = self._get_client()
         client.session.headers["X-No-Count"] = "true"
         page_size = getattr(self.model._meta, "page_size", 50)
         page_number = 1
         while True:
             try:
                 page = client.get(
                     self.resource_type,
```

### Comparing `django-json-api-1.2.0/django_json_api/models.py` & `django-json-api-1.2.1/django_json_api/models.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/django_json_api/rest_framework.py` & `django-json-api-1.2.1/django_json_api/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/django_json_api.egg-info/PKG-INFO` & `django-json-api-1.2.1/django_json_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-json-api
-Version: 1.2.0
+Version: 1.2.1
 Summary: JSON API specification for Django services
 Home-page: https://github.com/share-work/django-json-api
 Author: Sharework
 Author-email: root@sharework.co
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-json-api-1.2.0/django_json_api.egg-info/SOURCES.txt` & `django-json-api-1.2.1/django_json_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/pyproject.toml` & `django-json-api-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/setup.py` & `django-json-api-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/tests/migrations/0001_initial.py` & `django-json-api-1.2.1/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/tests/models.py` & `django-json-api-1.2.1/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/tests/test_client.py` & `django-json-api-1.2.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/tests/test_django.py` & `django-json-api-1.2.1/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/tests/test_fields.py` & `django-json-api-1.2.1/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/tests/test_manager.py` & `django-json-api-1.2.1/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/tests/test_models.py` & `django-json-api-1.2.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/tests/test_rest_framework.py` & `django-json-api-1.2.1/tests/test_rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/tests/test_version.py` & `django-json-api-1.2.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `django-json-api-1.2.0/tests/utils.py` & `django-json-api-1.2.1/tests/utils.py`

 * *Files identical despite different names*

