# Comparing `tmp/dune_client-1.0.0.tar.gz` & `tmp/dune_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_client-1.0.0.tar", last modified: Tue Mar 21 10:54:06 2023, max compression
+gzip compressed data, was "dune_client-1.1.1.tar", last modified: Mon Jun  5 15:33:58 2023, max compression
```

## Comparing `dune_client-1.0.0.tar` & `dune_client-1.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:06.863910 dune_client-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-21 10:53:55.000000 dune_client-1.0.0/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:06.855910 dune_client-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:06.859910 dune_client-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-21 10:53:55.000000 dune_client-1.0.0/.github/workflows/cla.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-21 10:53:55.000000 dune_client-1.0.0/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-21 10:53:55.000000 dune_client-1.0.0/.github/workflows/py-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-21 10:53:55.000000 dune_client-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-21 10:53:55.000000 dune_client-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-21 10:53:55.000000 dune_client-1.0.0/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-21 10:53:55.000000 dune_client-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-21 10:53:55.000000 dune_client-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-21 10:54:06.863910 dune_client-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-21 10:53:55.000000 dune_client-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:06.859910 dune_client-1.0.0/dune_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/client_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:06.863910 dune_client-1.0.0/dune_client/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/file/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-21 10:53:55.000000 dune_client-1.0.0/dune_client/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:06.863910 dune_client-1.0.0/dune_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-21 10:54:06.000000 dune_client-1.0.0/dune_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-21 10:54:06.000000 dune_client-1.0.0/dune_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 10:54:06.000000 dune_client-1.0.0/dune_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 10:54:06.000000 dune_client-1.0.0/dune_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-21 10:54:06.000000 dune_client-1.0.0/dune_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-21 10:54:06.000000 dune_client-1.0.0/dune_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-21 10:53:55.000000 dune_client-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:06.863910 dune_client-1.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-21 10:53:55.000000 dune_client-1.0.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-21 10:53:55.000000 dune_client-1.0.0/requirements/prod.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-21 10:54:06.863910 dune_client-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-21 10:53:55.000000 dune_client-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:06.855910 dune_client-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:06.863910 dune_client-1.0.0/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-21 10:53:55.000000 dune_client-1.0.0/tests/e2e/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-03-21 10:53:55.000000 dune_client-1.0.0/tests/e2e/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:54:06.863910 dune_client-1.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-03-21 10:53:55.000000 dune_client-1.0.0/tests/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-03-21 10:53:55.000000 dune_client-1.0.0/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-21 10:53:55.000000 dune_client-1.0.0/tests/unit/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-03-21 10:53:55.000000 dune_client-1.0.0/tests/unit/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 15:33:40.000000 dune_client-1.1.1/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.327243 dune_client-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.331243 dune_client-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 15:33:40.000000 dune_client-1.1.1/.github/workflows/cla.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 15:33:40.000000 dune_client-1.1.1/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-05 15:33:40.000000 dune_client-1.1.1/.github/workflows/py-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 15:33:40.000000 dune_client-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 15:33:40.000000 dune_client-1.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 15:33:40.000000 dune_client-1.1.1/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 15:33:40.000000 dune_client-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-05 15:33:40.000000 dune_client-1.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-05 15:33:58.335243 dune_client-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-05 15:33:40.000000 dune_client-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/dune_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/client_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/dune_client/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/file/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/dune_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-05 15:33:40.000000 dune_client-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-05 15:33:40.000000 dune_client-1.1.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 15:33:40.000000 dune_client-1.1.1/requirements/prod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-05 15:33:58.339243 dune_client-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:33:40.000000 dune_client-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.327243 dune_client-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/e2e/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/e2e/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/unit/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/unit/test_types.py
```

### Comparing `dune_client-1.0.0/.github/workflows/cla.yaml` & `dune_client-1.1.1/.github/workflows/cla.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/.github/workflows/pull-request.yaml` & `dune_client-1.1.1/.github/workflows/pull-request.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/.github/workflows/py-publish.yaml` & `dune_client-1.1.1/.github/workflows/py-publish.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/LICENSE` & `dune_client-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/Makefile` & `dune_client-1.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/PKG-INFO` & `dune_client-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune_client
-Version: 1.0.0
+Version: 1.1.1
 Summary: A simple framework for interacting with Dune Analytics official API service.
 Home-page: https://github.com/cowprotocol/dune-client
 Author: Benjamin H. Smith
 Author-email: ben@cow.fi
 License: Apache License Version 2.0
 Project-URL: Tracker, https://github.com/cowprotocol/dune-client/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dune_client-1.0.0/README.md` & `dune_client-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/dune_client/base_client.py` & `dune_client-1.1.1/dune_client/base_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     and provides some convenient functions to use in other clients
     """
 
     BASE_URL = "https://api.dune.com"
     API_PATH = "/api/v1"
     DEFAULT_TIMEOUT = 10
 
-    def __init__(self, api_key: str):
+    def __init__(self, api_key: str, performance: str = "medium"):
         self.token = api_key
+        self.performance = performance
         self.logger = logging.getLogger(__name__)
         logging.basicConfig(format="%(asctime)s %(levelname)s %(name)s %(message)s")
 
     def default_headers(self) -> Dict[str, str]:
         """Return default headers containing Dune Api token"""
         return {"x-dune-api-key": self.token}
```

### Comparing `dune_client-1.0.0/dune_client/client.py` & `dune_client-1.1.1/dune_client/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Framework built on Dune's API Documentation
 https://duneanalytics.notion.site/API-Documentation-1b93d16e0fa941398e15047f643e003a
 """
 from __future__ import annotations
 
 import time
 from io import BytesIO
-from typing import Any
+from typing import Any, Optional, Union
 
 import requests
 from requests import Response, JSONDecodeError
 
 from dune_client.base_client import BaseDuneClient
 from dune_client.interface import DuneInterface
 from dune_client.models import (
@@ -46,43 +46,50 @@
             # Others can't. Only raise HTTP error for not decodable errors
             response.raise_for_status()
             raise ValueError("Unreachable since previous line raises") from err
 
     def _route_url(self, route: str) -> str:
         return f"{self.BASE_URL}{self.API_PATH}/{route}"
 
-    def _get(self, route: str) -> Any:
+    def _get(self, route: str, params: Optional[Any] = None) -> Any:
         url = self._route_url(route)
         self.logger.debug(f"GET received input url={url}")
         response = requests.get(
             url,
             headers={"x-dune-api-key": self.token},
             timeout=self.DEFAULT_TIMEOUT,
+            params=params,
         )
         return self._handle_response(response)
 
     def _post(self, route: str, params: Any) -> Any:
         url = self._route_url(route)
         self.logger.debug(f"POST received input url={url}, params={params}")
         response = requests.post(
             url=url,
             json=params,
             headers={"x-dune-api-key": self.token},
             timeout=self.DEFAULT_TIMEOUT,
         )
         return self._handle_response(response)
 
-    def execute(self, query: Query) -> ExecutionResponse:
+    def execute(
+        self, query: Query, performance: Optional[str] = None
+    ) -> ExecutionResponse:
         """Post's to Dune API for execute `query`"""
+        self.logger.info(
+            f"executing {query.query_id} on {performance or self.performance} cluster"
+        )
         response_json = self._post(
             route=f"query/{query.query_id}/execute",
             params={
                 "query_parameters": {
                     p.key: p.to_dict()["value"] for p in query.parameters()
-                }
+                },
+                "performance": performance or self.performance,
             },
         )
         try:
             return ExecutionResponse.from_dict(response_json)
         except KeyError as err:
             raise DuneError(response_json, "ExecutionResponse", err) from err
 
@@ -118,65 +125,116 @@
             url,
             headers={"x-dune-api-key": self.token},
             timeout=self.DEFAULT_TIMEOUT,
         )
         response.raise_for_status()
         return ExecutionResultCSV(data=BytesIO(response.content))
 
+    def get_latest_result(self, query: Union[Query, str, int]) -> ResultsResponse:
+        """
+        GET the latest results for a query_id without having to execute the query again.
+
+        :param query: :class:`Query` object OR query id as string | int
+
+        https://dune.com/docs/api/api-reference/latest_results/
+        """
+        if isinstance(query, Query):
+            params = {
+                f"params.{p.key}": p.to_dict()["value"] for p in query.parameters()
+            }
+            query_id = query.query_id
+        else:
+            params = None
+            query_id = int(query)
+
+        response_json = self._get(
+            route=f"query/{query_id}/results",
+            params=params,
+        )
+        try:
+            return ResultsResponse.from_dict(response_json)
+        except KeyError as err:
+            raise DuneError(response_json, "ResultsResponse", err) from err
+
     def cancel_execution(self, job_id: str) -> bool:
         """POST Execution Cancellation to Dune API for `job_id` (aka `execution_id`)"""
         response_json = self._post(route=f"execution/{job_id}/cancel", params=None)
         try:
             # No need to make a dataclass for this since it's just a boolean.
             success: bool = response_json["success"]
             return success
         except KeyError as err:
             raise DuneError(response_json, "CancellationResponse", err) from err
 
-    def _refresh(self, query: Query, ping_frequency: int = 5) -> str:
-        job_id = self.execute(query).execution_id
+    def _refresh(
+        self,
+        query: Query,
+        ping_frequency: int = 5,
+        performance: Optional[str] = None,
+    ) -> str:
+        job_id = self.execute(query=query, performance=performance).execution_id
         status = self.get_status(job_id)
         while status.state not in ExecutionState.terminal_states():
             self.logger.info(
                 f"waiting for query execution {job_id} to complete: {status}"
             )
             time.sleep(ping_frequency)
             status = self.get_status(job_id)
         if status.state == ExecutionState.FAILED:
             self.logger.error(status)
             raise QueryFailed(f"{status}. Perhaps your query took too long to run!")
 
         return job_id
 
-    def refresh(self, query: Query, ping_frequency: int = 5) -> ResultsResponse:
+    def refresh(
+        self,
+        query: Query,
+        ping_frequency: int = 5,
+        performance: Optional[str] = None,
+    ) -> ResultsResponse:
         """
         Executes a Dune `query`, waits until execution completes,
         fetches and returns the results.
         Sleeps `ping_frequency` seconds between each status request.
         """
-        job_id = self._refresh(query, ping_frequency=ping_frequency)
+        job_id = self._refresh(
+            query,
+            ping_frequency=ping_frequency,
+            performance=performance,
+        )
         return self.get_result(job_id)
 
-    def refresh_csv(self, query: Query, ping_frequency: int = 5) -> ExecutionResultCSV:
+    def refresh_csv(
+        self,
+        query: Query,
+        ping_frequency: int = 5,
+        performance: Optional[str] = None,
+    ) -> ExecutionResultCSV:
         """
         Executes a Dune query, waits till execution completes,
         fetches and the results in CSV format
         (use it load the data directly in pandas.from_csv() or similar frameworks)
         """
-        job_id = self._refresh(query, ping_frequency=ping_frequency)
+        job_id = self._refresh(
+            query,
+            ping_frequency=ping_frequency,
+            performance=performance,
+        )
         return self.get_result_csv(job_id)
 
-    def refresh_into_dataframe(self, query: Query) -> Any:
+    def refresh_into_dataframe(
+        self, query: Query, performance: Optional[str] = None
+    ) -> Any:
         """
         Execute a Dune Query, waits till execution completes,
         fetched and returns the result as a Pandas DataFrame
 
         This is a convenience method that uses refresh_csv underneath
         """
         try:
             import pandas  # type: ignore # pylint: disable=import-outside-toplevel
         except ImportError as exc:
             raise ImportError(
                 "dependency failure, pandas is required but missing"
             ) from exc
-        data = self.refresh_csv(query).data
+        data = self.refresh_csv(query, performance=performance).data
         return pandas.read_csv(data)
```

### Comparing `dune_client-1.0.0/dune_client/client_async.py` & `dune_client-1.1.1/dune_client/client_async.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """"
 Async Dune Client Class responsible for refreshing Dune Queries
 Framework built on Dune's API Documentation
 https://duneanalytics.notion.site/API-Documentation-1b93d16e0fa941398e15047f643e003a
 """
 from __future__ import annotations
 import asyncio
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 from aiohttp import (
     ClientSession,
     ClientResponse,
     ContentTypeError,
     TCPConnector,
     ClientTimeout,
@@ -33,21 +33,23 @@
     """
     An asynchronous interface for Dune API with a few convenience methods
     combining the use of endpoints (e.g. refresh)
     """
 
     _connection_limit = 3
 
-    def __init__(self, api_key: str, connection_limit: int = 3):
+    def __init__(
+        self, api_key: str, connection_limit: int = 3, performance: str = "medium"
+    ):
         """
         api_key - Dune API key
         connection_limit - number of parallel requests to execute.
         For non-pro accounts Dune allows only up to 3 requests but that number can be increased.
         """
-        super().__init__(api_key=api_key)
+        super().__init__(api_key=api_key, performance=performance)
         self._connection_limit = connection_limit
         self._session: Optional[ClientSession] = None
 
     async def _create_session(self) -> ClientSession:
         conn = TCPConnector(limit=self._connection_limit)
         return ClientSession(
             connector=conn,
@@ -81,40 +83,49 @@
             self.logger.debug(f"received response {response_json}")
             return response_json
         except ContentTypeError as err:
             # Others can't. Only raise HTTP error for not decodable errors
             response.raise_for_status()
             raise ValueError("Unreachable since previous line raises") from err
 
-    async def _get(self, url: str) -> Any:
+    async def _get(self, url: str, params: Optional[Any] = None) -> Any:
         if self._session is None:
             raise ValueError("Client is not connected; call `await cl.connect()`")
         self.logger.debug(f"GET received input url={url}")
         response = await self._session.get(
             url=f"{self.API_PATH}{url}",
             headers=self.default_headers(),
+            params=params,
         )
         return await self._handle_response(response)
 
     async def _post(self, url: str, params: Any) -> Any:
         if self._session is None:
             raise ValueError("Client is not connected; call `await cl.connect()`")
         self.logger.debug(f"POST received input url={url}, params={params}")
         response = await self._session.post(
             url=f"{self.API_PATH}{url}",
             json=params,
             headers=self.default_headers(),
         )
         return await self._handle_response(response)
 
-    async def execute(self, query: Query) -> ExecutionResponse:
+    async def execute(
+        self, query: Query, performance: Optional[str] = None
+    ) -> ExecutionResponse:
         """Post's to Dune API for execute `query`"""
+        params = query.request_format()
+        params["performance"] = performance or self.performance
+
+        self.logger.info(
+            f"executing {query.query_id} on {performance or self.performance} cluster"
+        )
         response_json = await self._post(
             url=f"/query/{query.query_id}/execute",
-            params=query.request_format(),
+            params=params,
         )
         try:
             return ExecutionResponse.from_dict(response_json)
         except KeyError as err:
             raise DuneError(response_json, "ExecutionResponse", err) from err
 
     async def get_status(self, job_id: str) -> ExecutionStatusResponse:
@@ -131,31 +142,60 @@
         """GET results from Dune API for `job_id` (aka `execution_id`)"""
         response_json = await self._get(url=f"/execution/{job_id}/results")
         try:
             return ResultsResponse.from_dict(response_json)
         except KeyError as err:
             raise DuneError(response_json, "ResultsResponse", err) from err
 
+    async def get_latest_result(self, query: Union[Query, str, int]) -> ResultsResponse:
+        """
+        GET the latest results for a query_id without having to execute the query again.
+
+        https://dune.com/docs/api/api-reference/latest_results/
+        """
+        if isinstance(query, Query):
+            params = {
+                f"params.{p.key}": p.to_dict()["value"] for p in query.parameters()
+            }
+            query_id = query.query_id
+        else:
+            params = None
+            query_id = int(query)
+
+        response_json = await self._get(
+            url=f"/query/{query_id}/results",
+            params=params,
+        )
+        try:
+            return ResultsResponse.from_dict(response_json)
+        except KeyError as err:
+            raise DuneError(response_json, "ResultsResponse", err) from err
+
     async def cancel_execution(self, job_id: str) -> bool:
         """POST Execution Cancellation to Dune API for `job_id` (aka `execution_id`)"""
         response_json = await self._post(url=f"/execution/{job_id}/cancel", params=None)
         try:
             # No need to make a dataclass for this since it's just a boolean.
             success: bool = response_json["success"]
             return success
         except KeyError as err:
             raise DuneError(response_json, "CancellationResponse", err) from err
 
-    async def refresh(self, query: Query, ping_frequency: int = 5) -> ResultsResponse:
+    async def refresh(
+        self,
+        query: Query,
+        ping_frequency: int = 5,
+        performance: Optional[str] = None,
+    ) -> ResultsResponse:
         """
         Executes a Dune `query`, waits until execution completes,
         fetches and returns the results.
         Sleeps `ping_frequency` seconds between each status request.
         """
-        job_id = (await self.execute(query)).execution_id
+        job_id = (await self.execute(query=query, performance=performance)).execution_id
         status = await self.get_status(job_id)
         while status.state not in ExecutionState.terminal_states():
             self.logger.info(
                 f"waiting for query execution {job_id} to complete: {status}"
             )
             await asyncio.sleep(ping_frequency)
             status = await self.get_status(job_id)
```

### Comparing `dune_client-1.0.0/dune_client/file/base.py` & `dune_client-1.1.1/dune_client/file/base.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/dune_client/file/interface.py` & `dune_client-1.1.1/dune_client/file/interface.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/dune_client/interface.py` & `dune_client-1.1.1/dune_client/interface.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/dune_client/models.py` & `dune_client-1.1.1/dune_client/models.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/dune_client/query.py` & `dune_client-1.1.1/dune_client/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Data Class Representing a Dune Query
 """
 import urllib.parse
 from dataclasses import dataclass
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, Union
 
 from dune_client.types import QueryParameter
 
 
 @dataclass
 class Query:
     """Basic data structure constituting a Dune Analytics Query."""
@@ -37,12 +37,12 @@
     def __hash__(self) -> int:
         """
         This contains the query ID and the values of relevant parameters.
         Thus, it is unique for caching purposes
         """
         return self.url().__hash__()
 
-    def request_format(self) -> Dict[str, Dict[str, str]]:
+    def request_format(self) -> Dict[str, Union[Dict[str, str], str, None]]:
         """Transforms Query objects to params to pass in API"""
         return {
             "query_parameters": {p.key: p.to_dict()["value"] for p in self.parameters()}
         }
```

### Comparing `dune_client-1.0.0/dune_client/types.py` & `dune_client-1.1.1/dune_client/types.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/dune_client.egg-info/PKG-INFO` & `dune_client-1.1.1/dune_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-client
-Version: 1.0.0
+Version: 1.1.1
 Summary: A simple framework for interacting with Dune Analytics official API service.
 Home-page: https://github.com/cowprotocol/dune-client
 Author: Benjamin H. Smith
 Author-email: ben@cow.fi
 License: Apache License Version 2.0
 Project-URL: Tracker, https://github.com/cowprotocol/dune-client/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dune_client-1.0.0/dune_client.egg-info/SOURCES.txt` & `dune_client-1.1.1/dune_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/setup.cfg` & `dune_client-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/tests/e2e/test_async_client.py` & `dune_client-1.1.1/tests/e2e/test_async_client.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/tests/e2e/test_client.py` & `dune_client-1.1.1/tests/e2e/test_client.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/tests/unit/test_file.py` & `dune_client-1.1.1/tests/unit/test_file.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/tests/unit/test_models.py` & `dune_client-1.1.1/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/tests/unit/test_query.py` & `dune_client-1.1.1/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.0.0/tests/unit/test_types.py` & `dune_client-1.1.1/tests/unit/test_types.py`

 * *Files identical despite different names*

