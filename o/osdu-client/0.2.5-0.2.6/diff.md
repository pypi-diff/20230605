# Comparing `tmp/osdu_client-0.2.5.tar.gz` & `tmp/osdu_client-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osdu_client-0.2.5.tar", last modified: Fri Sep  9 04:53:19 2022, max compression
+gzip compressed data, was "osdu_client-0.2.6.tar", last modified: Mon Jun  5 19:11:44 2023, max compression
```

## Comparing `osdu_client-0.2.5.tar` & `osdu_client-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 04:53:19.343246 osdu_client-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-09-09 04:53:19.343246 osdu_client-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-09-09 04:53:13.000000 osdu_client-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-09 04:53:19.343246 osdu_client-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-09-09 04:53:13.000000 osdu_client-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 04:53:19.331246 osdu_client-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 04:53:19.335246 osdu_client-0.2.5/src/osdu_client/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 04:53:19.343246 osdu_client-0.2.5/src/osdu_client/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/services/base_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/services/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2707 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/services/entitlements_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/services/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/services/legal_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/services/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    17580 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/services/sdms_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/services/search_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-09-09 04:53:13.000000 osdu_client-0.2.5/src/osdu_client/services/storage_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 04:53:19.339246 osdu_client-0.2.5/src/osdu_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-09-09 04:53:19.000000 osdu_client-0.2.5/src/osdu_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-09-09 04:53:19.000000 osdu_client-0.2.5/src/osdu_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 04:53:19.000000 osdu_client-0.2.5/src/osdu_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-09 04:53:19.000000 osdu_client-0.2.5/src/osdu_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-09 04:53:19.000000 osdu_client-0.2.5/src/osdu_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:44.885796 osdu_client-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-05 19:11:40.000000 osdu_client-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-05 19:11:44.885796 osdu_client-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-05 19:11:40.000000 osdu_client-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 19:11:44.885796 osdu_client-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-05 19:11:40.000000 osdu_client-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:44.881795 osdu_client-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:44.885796 osdu_client-0.2.6/src/osdu_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:44.885796 osdu_client-0.2.6/src/osdu_client/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/entitlements_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/legal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/sdms_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/storage_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:44.885796 osdu_client-0.2.6/src/osdu_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-05 19:11:44.000000 osdu_client-0.2.6/src/osdu_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-05 19:11:44.000000 osdu_client-0.2.6/src/osdu_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:11:44.000000 osdu_client-0.2.6/src/osdu_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 19:11:44.000000 osdu_client-0.2.6/src/osdu_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 19:11:44.000000 osdu_client-0.2.6/src/osdu_client.egg-info/top_level.txt
```

### Comparing `osdu_client-0.2.5/PKG-INFO` & `osdu_client-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 Metadata-Version: 2.1
 Name: osdu_client
-Version: 0.2.5
+Version: 0.2.6
 Summary: OSDU API Client
 Home-page: https://github.com/micmurawski/osdu-client/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
-Description: # Introduction
-        
-        [![pypi](https://img.shields.io/pypi/v/osdu-client.svg)](https://pypi.org/project/osdu-client/)
-        
-        `osdu-client` is a python library implementing a simple OSDU client. With abstracted out authorization backend.
-        
-        # Instalation
-        ```
-        pip install osdu-client
-        ```
-        
-        # Example
-        OSDU API client can be adjusted to specific OSDU deployment by defining auth backend according to `AuthBackendInterface` methods.
-        
-        
-        
-        ```python
-        from typing import AnyStr, Dict
-        
-        from osdu_client import OSDUAPI
-        from osdu_client.auth import AuthBackendInterface
-        
-        
-        class AuthBackend(AuthBackendInterface):
-            def __init__(self, headers, base_url) -> None:
-                self._headers = headers
-                self._base_url = base_url
-        
-            def get_headers(self) -> Dict:
-                return self._headers
-        
-            def get_base_url(self) -> AnyStr:
-                return self._osdu_base_url
-        
-            def get_sd_connection_params(self, log_level: int = None) -> Dict:
-                return {}
-        
-        
-        auth_backend = AuthBackend(
-            headers={"Authorization": "Bearer XYZ"},
-            base_url="https://exmaple.com"
-        )
-        
-        storage_client = OSDUAPI.client('storage', auth_backend=auth_backend)
-        response = storage_client.get_record_versions(id="123")
-        
-        ```
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Introduction
+
+[![pypi](https://img.shields.io/pypi/v/osdu-client.svg)](https://pypi.org/project/osdu-client/)
+
+`osdu-client` is a python library implementing a simple OSDU client with an abstracted-out authorization backend.
+
+# Instalation
+```
+pip install osdu-client
+```
+
+# Example
+OSDU API client can be adjusted to specific OSDU deployment by defining auth backend according to `AuthBackendInterface` methods.
+
+
+
+```python
+from typing import AnyStr, Dict
+
+from osdu_client import OSDUAPI
+from osdu_client.auth import AuthBackendInterface
+
+
+class AuthBackend(AuthBackendInterface):
+    def __init__(self, headers, base_url) -> None:
+        self._headers = headers
+        self._base_url = base_url
+
+    def get_headers(self) -> Dict:
+        return self._headers
+
+    def get_base_url(self) -> AnyStr:
+        return self._osdu_base_url
+
+    def get_sd_connection_params(self, log_level: int = None) -> Dict:
+        return {}
+
+
+auth_backend = AuthBackend(
+    headers={"Authorization": "Bearer XYZ"},
+    base_url="https://exmaple.com"
+)
+
+storage_client = OSDUAPI.client('storage', auth_backend=auth_backend)
+response = storage_client.get_record_versions(id="123")
+
+```
+
```

### Comparing `osdu_client-0.2.5/README.md` & `osdu_client-0.2.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Introduction
 
 [![pypi](https://img.shields.io/pypi/v/osdu-client.svg)](https://pypi.org/project/osdu-client/)
 
-`osdu-client` is a python library implementing a simple OSDU client. With abstracted out authorization backend.
+`osdu-client` is a python library implementing a simple OSDU client with an abstracted-out authorization backend.
 
 # Instalation
 ```
 pip install osdu-client
 ```
 
 # Example
```

### Comparing `osdu_client-0.2.5/setup.py` & `osdu_client-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def get_dependencies():
     with open("requirements.txt", encoding="utf-8") as fh:
         return fh.read().splitlines()
 
 
 setup(
     name='osdu_client',
-    version='0.2.5',
+    version='0.2.6',
     author="Michal Murawski",
     author_email="mmurawski777@gmail.com",
     description="OSDU API Client",
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     url="https://github.com/micmurawski/osdu-client/",
     package_dir={"": "src"},
```

### Comparing `osdu_client-0.2.5/src/osdu_client/auth.py` & `osdu_client-0.2.6/src/osdu_client/auth.py`

 * *Files identical despite different names*

### Comparing `osdu_client-0.2.5/src/osdu_client/client.py` & `osdu_client-0.2.6/src/osdu_client/client.py`

 * *Files identical despite different names*

### Comparing `osdu_client-0.2.5/src/osdu_client/services/dataset_api.py` & `osdu_client-0.2.6/src/osdu_client/services/dataset_api.py`

 * *Files identical despite different names*

### Comparing `osdu_client-0.2.5/src/osdu_client/services/entitlements_api.py` & `osdu_client-0.2.6/src/osdu_client/services/entitlements_api.py`

 * *Files identical despite different names*

### Comparing `osdu_client-0.2.5/src/osdu_client/services/schema_api.py` & `osdu_client-0.2.6/src/osdu_client/services/schema_api.py`

 * *Files identical despite different names*

### Comparing `osdu_client-0.2.5/src/osdu_client/services/sdms_api.py` & `osdu_client-0.2.6/src/osdu_client/services/sdms_api.py`

 * *Files identical despite different names*

### Comparing `osdu_client-0.2.5/src/osdu_client/services/search_api.py` & `osdu_client-0.2.6/src/osdu_client/services/search_api.py`

 * *Files identical despite different names*

### Comparing `osdu_client-0.2.5/src/osdu_client/services/storage_api.py` & `osdu_client-0.2.6/src/osdu_client/services/storage_api.py`

 * *Files identical despite different names*

### Comparing `osdu_client-0.2.5/src/osdu_client.egg-info/PKG-INFO` & `osdu_client-0.2.6/src/osdu_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 Metadata-Version: 2.1
 Name: osdu-client
-Version: 0.2.5
+Version: 0.2.6
 Summary: OSDU API Client
 Home-page: https://github.com/micmurawski/osdu-client/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
-Description: # Introduction
-        
-        [![pypi](https://img.shields.io/pypi/v/osdu-client.svg)](https://pypi.org/project/osdu-client/)
-        
-        `osdu-client` is a python library implementing a simple OSDU client. With abstracted out authorization backend.
-        
-        # Instalation
-        ```
-        pip install osdu-client
-        ```
-        
-        # Example
-        OSDU API client can be adjusted to specific OSDU deployment by defining auth backend according to `AuthBackendInterface` methods.
-        
-        
-        
-        ```python
-        from typing import AnyStr, Dict
-        
-        from osdu_client import OSDUAPI
-        from osdu_client.auth import AuthBackendInterface
-        
-        
-        class AuthBackend(AuthBackendInterface):
-            def __init__(self, headers, base_url) -> None:
-                self._headers = headers
-                self._base_url = base_url
-        
-            def get_headers(self) -> Dict:
-                return self._headers
-        
-            def get_base_url(self) -> AnyStr:
-                return self._osdu_base_url
-        
-            def get_sd_connection_params(self, log_level: int = None) -> Dict:
-                return {}
-        
-        
-        auth_backend = AuthBackend(
-            headers={"Authorization": "Bearer XYZ"},
-            base_url="https://exmaple.com"
-        )
-        
-        storage_client = OSDUAPI.client('storage', auth_backend=auth_backend)
-        response = storage_client.get_record_versions(id="123")
-        
-        ```
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Introduction
+
+[![pypi](https://img.shields.io/pypi/v/osdu-client.svg)](https://pypi.org/project/osdu-client/)
+
+`osdu-client` is a python library implementing a simple OSDU client with an abstracted-out authorization backend.
+
+# Instalation
+```
+pip install osdu-client
+```
+
+# Example
+OSDU API client can be adjusted to specific OSDU deployment by defining auth backend according to `AuthBackendInterface` methods.
+
+
+
+```python
+from typing import AnyStr, Dict
+
+from osdu_client import OSDUAPI
+from osdu_client.auth import AuthBackendInterface
+
+
+class AuthBackend(AuthBackendInterface):
+    def __init__(self, headers, base_url) -> None:
+        self._headers = headers
+        self._base_url = base_url
+
+    def get_headers(self) -> Dict:
+        return self._headers
+
+    def get_base_url(self) -> AnyStr:
+        return self._osdu_base_url
+
+    def get_sd_connection_params(self, log_level: int = None) -> Dict:
+        return {}
+
+
+auth_backend = AuthBackend(
+    headers={"Authorization": "Bearer XYZ"},
+    base_url="https://exmaple.com"
+)
+
+storage_client = OSDUAPI.client('storage', auth_backend=auth_backend)
+response = storage_client.get_record_versions(id="123")
+
+```
+
```

### Comparing `osdu_client-0.2.5/src/osdu_client.egg-info/SOURCES.txt` & `osdu_client-0.2.6/src/osdu_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 src/osdu_client/__init__.py
 src/osdu_client/auth.py
 src/osdu_client/client.py
 src/osdu_client/exceptions.py
```

