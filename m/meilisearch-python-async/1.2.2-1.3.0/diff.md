# Comparing `tmp/meilisearch_python_async-1.2.2.tar.gz` & `tmp/meilisearch_python_async-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.2.2.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.3.0.tar", max compression
```

## Comparing `meilisearch_python_async-1.2.2.tar` & `meilisearch_python_async-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/LICENSE
--rw-r--r--   0        0        0     4641 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/README.md
--rw-r--r--   0        0        0      151 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2759 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0       18 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/_version.py
--rw-r--r--   0        0        0    22123 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     1886 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    86427 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     1576 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0      392 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1285 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-05-10 15:31:30.214418 meilisearch_python_async-1.2.2/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0      769 2023-05-10 15:31:30.218418 meilisearch_python_async-1.2.2/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-05-10 15:31:30.218418 meilisearch_python_async-1.2.2/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-05-10 15:31:30.218418 meilisearch_python_async-1.2.2/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    11610 2023-05-10 15:31:30.218418 meilisearch_python_async-1.2.2/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2184 2023-05-10 15:31:30.218418 meilisearch_python_async-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 meilisearch_python_async-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5759 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/README.md
+-rw-r--r--   0        0        0      151 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2759 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0       18 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/meilisearch_python_async/_version.py
+-rw-r--r--   0        0        0    22205 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     1886 2023-06-05 09:37:57.637488 meilisearch_python_async-1.3.0/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    89041 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     1576 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0      392 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1285 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     1119 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0      769 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    11471 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2286 2023-06-05 09:37:57.641488 meilisearch_python_async-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6968 1970-01-01 00:00:00.000000 meilisearch_python_async-1.3.0/PKG-INFO
```

### Comparing `meilisearch_python_async-1.2.2/LICENSE` & `meilisearch_python_async-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.2/README.md` & `meilisearch_python_async-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -117,14 +117,36 @@
     exhaustive_nb_hits = bool,
     facets_distributionn = None,
     processing_time_ms = 5,
     query = "galaxy",
 )
 ```
 
+## Benchmark
+
+The following benchmarks compare this library to the official
+[Meilisearch Python](https://github.com/meilisearch/meilisearch-python) library. Note that all
+of the performance gains seen are achieved by taking advantage of asyncio. This means that if your
+code is not taking advantage of asyncio or blocking the event loop the gains here will not be seen
+and the performance between the two libraries will be very close to the same.
+
+### Add Documents in Batches
+
+This test compares how long it takes to send 1 million documents in batches of 1 thousand to the
+Meilisearch server for indexing (lower is better). The time does not take into account how long
+Meilisearch takes to index the documents since that is outside of the library functionality.
+
+![Add Documents in Batches](https://raw.githubusercontent.com/sanders41/meilisearch-python-async/main/assets/add_in_batches.png)
+
+### Muiltiple Searches
+
+This test compares how long it takes to complete 1000 searches (lower is better)
+
+![Multiple Searches](https://raw.githubusercontent.com/sanders41/meilisearch-python-async/main/assets/searches.png)
+
 ## Documentation
 
 See our [docs](https://meilisearch-python-async.paulsanders.dev) for the full documentation.
 
 ## Contributing
 
 Contributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)
```

### Comparing `meilisearch_python_async-1.2.2/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.3.0/meilisearch_python_async/_http_requests.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.2/meilisearch_python_async/client.py` & `meilisearch_python_async-1.3.0/meilisearch_python_async/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import json
-from datetime import datetime
+from datetime import datetime, timezone
 from ssl import SSLContext
 from types import TracebackType
-from typing import Any, Type
+from typing import Any
 
 import jwt
 from httpx import AsyncClient
 
 from meilisearch_python_async._http_requests import HttpRequests
 from meilisearch_python_async.errors import InvalidRestriction, MeilisearchApiError
 from meilisearch_python_async.index import Index
@@ -61,16 +61,16 @@
         self._http_requests = HttpRequests(self.http_client)
 
     async def __aenter__(self) -> Client:
         return self
 
     async def __aexit__(
         self,
-        et: Type[BaseException] | None,
-        ev: Type[BaseException] | None,
+        et: type[BaseException] | None,
+        ev: type[BaseException] | None,
         traceback: TracebackType | None,
     ) -> None:
         await self.aclose()
 
     async def aclose(self) -> None:
         """Closes the client.
 
@@ -145,15 +145,17 @@
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     await client.delete_index_if_exists()
         """
         url = f"indexes/{uid}"
         response = await self._http_requests.delete(url)
-        status = await wait_for_task(self.http_client, response.json()["taskUid"])
+        status = await wait_for_task(
+            self.http_client, response.json()["taskUid"], timeout_in_ms=100000
+        )
         if status.status == "succeeded":
             return True
         return False
 
     def generate_tenant_token(
         self,
         search_rules: dict[str, Any] | list[str],
@@ -181,18 +183,18 @@
 
             InvalidRestriction: If the restrictions are less strict than the permissions allowed
                 in the API key.
             KeyNotFoundError: If no API search key is found.
 
         Examples:
 
-            >>> from datetime import datetime, timedelta
+            >>> from datetime import datetime, timedelta, timezone
             >>> from meilisearch_python_async import Client
             >>>
-            >>> expires_at = datetime.utcnow() + timedelta(days=7)
+            >>> expires_at = datetime.now(tz=timezone.utc) + timedelta(days=7)
             >>>
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     token = client.generate_tenant_token(
             >>>         search_rules = ["*"], api_key=api_key, expires_at=expires_at
             >>>     )
         """
         # if Client._valid_uuid(api_key.key) is False:
@@ -205,15 +207,15 @@
                         "Invalid index. The token cannot be less restrictive than the API key"
                     )
 
         payload: dict[str, Any] = {"searchRules": search_rules}
 
         payload["apiKeyUid"] = api_key.uid
         if expires_at:
-            if expires_at <= datetime.utcnow():
+            if expires_at <= datetime.now(tz=timezone.utc):
                 raise ValueError("expires_at must be a time in the future")
 
             payload["exp"] = int(datetime.timestamp(expires_at))
 
         return jwt.encode(payload, api_key.key, algorithm="HS256")
 
     async def get_indexes(self) -> list[Index] | None:
```

### Comparing `meilisearch_python_async-1.2.2/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.3.0/meilisearch_python_async/errors.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.2/meilisearch_python_async/index.py` & `meilisearch_python_async-1.3.0/meilisearch_python_async/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     await index.delete_if_exists()
         """
         response = await self.delete()
-        status = await wait_for_task(self.http_client, response.task_uid)
+        status = await wait_for_task(self.http_client, response.task_uid, timeout_in_ms=100000)
         if status.status == "succeeded":
             return True
 
         return False
 
     async def update(self, primary_key: str) -> Index:
         """Update the index primary key.
@@ -390,24 +390,31 @@
         """
         url = f"{self._documents_url}/{document_id}"
         response = await self._http_requests.get(url)
 
         return response.json()
 
     async def get_documents(
-        self, *, offset: int = 0, limit: int = 20, fields: list[str] | None = None
+        self,
+        *,
+        offset: int = 0,
+        limit: int = 20,
+        fields: list[str] | None = None,
+        filter: str | list[str | list[str]] | None = None,
     ) -> DocumentsInfo:
         """Get a batch documents from the index.
 
         Args:
 
             offset: Number of documents to skip. Defaults to 0.
             limit: Maximum number of documents returnedd. Defaults to 20.
             fields: Document attributes to show. If this value is None then all
                 attributes are retrieved. Defaults to None.
+            filter: Filter value information. Defaults to None. Note: This parameter can only be
+                used with Meilisearch >= v1.2.0
 
         Returns:
 
             Documents info.
 
         Raises:
 
@@ -423,19 +430,30 @@
             >>>     documents = await index.get_documents()
         """
         parameters: dict[str, Any] = {
             "offset": offset,
             "limit": limit,
         }
 
+        if not filter:
+            if fields:
+                parameters["fields"] = ",".join(fields)
+
+            url = f"{self._documents_url}?{urlencode(parameters)}"
+            response = await self._http_requests.get(url)
+
+            return DocumentsInfo(**response.json())
+
         if fields:
-            parameters["fields"] = ",".join(fields)
+            parameters["fields"] = fields
 
-        url = f"{self._documents_url}?{urlencode(parameters)}"
-        response = await self._http_requests.get(url)
+        parameters["filter"] = filter
+
+        url = f"{self._documents_url}/fetch"
+        response = await self._http_requests.post(url, body=parameters)
 
         return DocumentsInfo(**response.json())
 
     async def add_documents(
         self, documents: list[dict[str, Any]], primary_key: str | None = None
     ) -> TaskInfo:
         """Add documents to the index.
@@ -1303,14 +1321,75 @@
             >>>     await index.delete_documents(["1234", "5678"])
         """
         url = f"{self._documents_url}/delete-batch"
         response = await self._http_requests.post(url, ids)
 
         return TaskInfo(**response.json())
 
+    async def delete_documents_by_filter(self, filter: str | list[str | list[str]]) -> TaskInfo:
+        """Delete documents from the index by filter.
+
+        Args:
+
+            filter: The filter value information.
+
+        Returns:
+
+            The details of the task status.
+
+        Raises:
+
+            MeilisearchCommunicationError: If there was an error communicating with the server.
+            MeilisearchApiError: If the Meilisearch API returned an error.
+
+        Examples:
+
+            >>> from meilisearch_python_async import Client
+            >>> async with Client("http://localhost.com", "masterKey") as client:
+            >>>     index = client.index("movies")
+            >>>     await index.delete_documents_by_filter("genre=horor"))
+        """
+        url = f"{self._documents_url}/delete"
+        response = await self._http_requests.post(url, body={"filter": filter})
+
+        return TaskInfo(**response.json())
+
+    async def delete_documents_in_batches_by_filter(
+        self, filters: list[str | list[str | list[str]]]
+    ) -> list[TaskInfo]:
+        """Delete batches of documents from the index by filter.
+
+        Args:
+
+            filters: A list of filter value information.
+
+        Returns:
+
+            The a list of details of the task statuses.
+
+        Raises:
+
+            MeilisearchCommunicationError: If there was an error communicating with the server.
+            MeilisearchApiError: If the Meilisearch API returned an error.
+
+        Examples:
+
+            >>> from meilisearch_python_async import Client
+            >>> async with Client("http://localhost.com", "masterKey") as client:
+            >>>     index = client.index("movies")
+            >>>     await index.delete_documents_in_batches_by_filter(
+            >>>         [
+            >>>             "genre=horor"),
+            >>>             "release_date=1520035200"),
+            >>>         ]
+            >>>     )
+        """
+        tasks = [self.delete_documents_by_filter(filter) for filter in filters]
+        return await gather(*tasks)
+
     async def delete_all_documents(self) -> TaskInfo:
         """Delete all documents from the index.
 
         Returns:
 
             The details of the task status.
 
@@ -2331,25 +2410,25 @@
         if (
             csv_delimiter
             and len(csv_delimiter) != 1
             or csv_delimiter
             and not csv_delimiter.isascii()
         ):
             raise ValueError("csv_delimiter must be a single ascii character")
-        with open(file_path, mode="r") as f:
+        with open(file_path) as f:
             if csv_delimiter:
                 documents = await loop.run_in_executor(
                     None, partial(DictReader, f, delimiter=csv_delimiter)
                 )
             else:
                 documents = await loop.run_in_executor(None, partial(DictReader, f))
             return list(documents)
 
     if file_path.suffix == ".ndjson":
-        with open(file_path, mode="r") as f:
+        with open(file_path) as f:
             return [await loop.run_in_executor(None, partial(json.loads, x)) for x in f]
 
     async with aiofiles.open(file_path, mode="r") as f:  # type: ignore
         data = await f.read()  # type: ignore
         documents = await loop.run_in_executor(None, partial(json.loads, data))
 
         if not isinstance(documents, list):
```

### Comparing `meilisearch_python_async-1.2.2/meilisearch_python_async/models/client.py` & `meilisearch_python_async-1.3.0/meilisearch_python_async/models/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.2/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.3.0/meilisearch_python_async/models/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.2/meilisearch_python_async/models/settings.py` & `meilisearch_python_async-1.3.0/meilisearch_python_async/models/settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.2/meilisearch_python_async/models/task.py` & `meilisearch_python_async-1.3.0/meilisearch_python_async/models/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.2/meilisearch_python_async/task.py` & `meilisearch_python_async-1.3.0/meilisearch_python_async/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,16 +288,14 @@
     else:
         while True:
             response = await http_requests.get(url)
             status = TaskStatus(**response.json())
             if status.status in ("succeeded", "failed"):
                 return status
             await sleep(interval_in_ms / 1000)
-            time_delta = datetime.now() - start_time
-            elapsed_time = time_delta.seconds * 1000 + time_delta.microseconds / 1000
 
 
 def _get_client(client: AsyncClient | Client) -> AsyncClient:
     if isinstance(client, AsyncClient):
         return client
 
     return client.http_client
```

### Comparing `meilisearch_python_async-1.2.2/pyproject.toml` & `meilisearch_python_async-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.2.2"
+version = "1.3.0"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
@@ -33,22 +33,25 @@
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.8.0"
 mypy = ">=0.981"
 pre-commit = ">=2.20.0"
 pytest = ">=7.1.3"
 pytest-cov = ">=4.0.0"
-tox = ">=3.26.0"
 pytest-asyncio = ">=0.19.0"
 types-aiofiles = ">=22.1.0"
 mkdocs = ">=1.2.4"
 mkdocs-material = ">=8.2.7"
 mkdocstrings = {version = ">=0.19.0", extras = ["python"]}
 ruff = ">=0.0.259"
-tomli = {version = "2.0.1", python = "<3.11"}
+tomli = {version = ">=2.0.1", python = "<3.11"}
+
+[tool.poetry.group.benchmark.dependencies]
+meilisearch = ">=0.26.0"
+rich = ">=13.3.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
@@ -82,11 +85,12 @@
 plugins = ["pydantic.mypy"]
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 disallow_untyped_defs = false
 
 [tool.ruff]
-select=["E", "F", "T201", "T203", "I001"]
+select=["E", "F", "UP", "I001", "T201", "T203"]
 ignore=["E501"]
 line-length = 100
+target-version = "py37"
 fix = true
```

### Comparing `meilisearch_python_async-1.2.2/PKG-INFO` & `meilisearch_python_async-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.2.2
+Version: 1.3.0
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -14,19 +14,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: PyJWT (>=2.3.0)
 Requires-Dist: aiofiles (>=0.7)
 Requires-Dist: camel-converter (>=1.0.0)
 Requires-Dist: httpx (>=0.17)
 Requires-Dist: pydantic (>=1.8)
 Project-URL: Documentation, https://meilisearch-python-async.paulsanders.dev
@@ -152,14 +147,36 @@
     exhaustive_nb_hits = bool,
     facets_distributionn = None,
     processing_time_ms = 5,
     query = "galaxy",
 )
 ```
 
+## Benchmark
+
+The following benchmarks compare this library to the official
+[Meilisearch Python](https://github.com/meilisearch/meilisearch-python) library. Note that all
+of the performance gains seen are achieved by taking advantage of asyncio. This means that if your
+code is not taking advantage of asyncio or blocking the event loop the gains here will not be seen
+and the performance between the two libraries will be very close to the same.
+
+### Add Documents in Batches
+
+This test compares how long it takes to send 1 million documents in batches of 1 thousand to the
+Meilisearch server for indexing (lower is better). The time does not take into account how long
+Meilisearch takes to index the documents since that is outside of the library functionality.
+
+![Add Documents in Batches](https://raw.githubusercontent.com/sanders41/meilisearch-python-async/main/assets/add_in_batches.png)
+
+### Muiltiple Searches
+
+This test compares how long it takes to complete 1000 searches (lower is better)
+
+![Multiple Searches](https://raw.githubusercontent.com/sanders41/meilisearch-python-async/main/assets/searches.png)
+
 ## Documentation
 
 See our [docs](https://meilisearch-python-async.paulsanders.dev) for the full documentation.
 
 ## Contributing
 
 Contributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)
```

