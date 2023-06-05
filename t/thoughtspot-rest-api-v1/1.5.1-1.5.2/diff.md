# Comparing `tmp/thoughtspot_rest_api_v1-1.5.1.tar.gz` & `tmp/thoughtspot_rest_api_v1-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtspot_rest_api_v1-1.5.1.tar", last modified: Tue May 30 19:45:39 2023, max compression
+gzip compressed data, was "thoughtspot_rest_api_v1-1.5.2.tar", last modified: Mon Jun  5 14:38:39 2023, max compression
```

## Comparing `thoughtspot_rest_api_v1-1.5.1.tar` & `thoughtspot_rest_api_v1-1.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-30 19:45:39.677397 thoughtspot_rest_api_v1-1.5.1/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.5.1/LICENSE
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-05-30 19:45:39.677472 thoughtspot_rest_api_v1-1.5.1/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365    28536 2023-03-17 18:28:57.000000 thoughtspot_rest_api_v1-1.5.1/README.md
--rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.1/pyproject.toml
--rw-r--r--   0 bryant.howell (535524999) 1339924365      884 2023-05-30 19:45:39.677800 thoughtspot_rest_api_v1-1.5.1/setup.cfg
--rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.1/setup.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-30 19:45:39.672979 thoughtspot_rest_api_v1-1.5.1/src/
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-30 19:45:39.676064 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/
--rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/__init__.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-05-30 16:27:14.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/_version.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/details_objects.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    75771 2023-05-15 15:24:30.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/tsrestapiv1.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    24853 2023-05-30 19:44:47.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/tsrestapiv2.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-30 19:45:39.677267 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-05-30 19:45:39.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2023-05-30 19:45:39.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2023-05-30 19:45:39.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-05-30 19:45:39.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/requires.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2023-05-30 19:45:39.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-06-05 14:38:39.535963 thoughtspot_rest_api_v1-1.5.2/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.5.2/LICENSE
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-06-05 14:38:39.536029 thoughtspot_rest_api_v1-1.5.2/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    28536 2023-03-17 18:28:57.000000 thoughtspot_rest_api_v1-1.5.2/README.md
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.2/pyproject.toml
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      884 2023-06-05 14:38:39.536336 thoughtspot_rest_api_v1-1.5.2/setup.cfg
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.2/setup.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-06-05 14:38:39.532449 thoughtspot_rest_api_v1-1.5.2/src/
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-06-05 14:38:39.534448 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/__init__.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-06-05 14:34:57.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/_version.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/details_objects.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    75805 2023-06-05 14:38:31.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/tsrestapiv1.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    24853 2023-05-30 19:44:47.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/tsrestapiv2.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-06-05 14:38:39.535833 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-06-05 14:38:39.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2023-06-05 14:38:39.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2023-06-05 14:38:39.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-06-05 14:38:39.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/requires.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2023-06-05 14:38:39.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
```

### Comparing `thoughtspot_rest_api_v1-1.5.1/LICENSE` & `thoughtspot_rest_api_v1-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.1/PKG-INFO` & `thoughtspot_rest_api_v1-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot_rest_api_v1
-Version: 1.5.1
+Version: 1.5.2
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
```

### Comparing `thoughtspot_rest_api_v1-1.5.1/README.md` & `thoughtspot_rest_api_v1-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.1/setup.cfg` & `thoughtspot_rest_api_v1-1.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = thoughtspot_rest_api_v1
-version = 1.5.1
+version = 1.5.2
 description = Library implementing the ThoughtSpot V1 REST API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 author = Bryant Howell
 author_email = bryant.howell@thoughtspot.com
 license = MIT
```

### Comparing `thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/details_objects.py` & `thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/details_objects.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/tsrestapiv1.py` & `thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/tsrestapiv1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1401,15 +1401,15 @@
              'auth_token': auth_token,
              'redirect_url': redirect_url,  # need to url encode
 
         }
 
         url = self.base_url + endpoint
 
-        response = self.requests_session.post(url=url, data=post_params)
+        response = self.requests_session.post(url=url, data=post_params, headers={'Accept': 'text/plain'})
         response.raise_for_status()
         return response
     #
     # USER Methods
     #
 
     def user_get(self, user_id: Optional[str] = None, name: Optional[str] = None) -> Union[Dict, List]:
```

### Comparing `thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/tsrestapiv2.py` & `thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/tsrestapiv2.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO` & `thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot-rest-api-v1
-Version: 1.5.1
+Version: 1.5.2
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
```

### Comparing `thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt` & `thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

