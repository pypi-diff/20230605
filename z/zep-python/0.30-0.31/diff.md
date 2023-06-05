# Comparing `tmp/zep_python-0.30.tar.gz` & `tmp/zep_python-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.30.tar", max compression
+gzip compressed data, was "zep_python-0.31.tar", max compression
```

## Comparing `zep_python-0.30.tar` & `zep_python-0.31.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-25 18:34:22.817551 zep_python-0.30/LICENSE
--rw-r--r--   0        0        0     2393 2023-05-25 18:34:22.817551 zep_python-0.30/README.md
--rw-r--r--   0        0        0      872 2023-05-25 18:34:22.821551 zep_python-0.30/pyproject.toml
--rw-r--r--   0        0        0      340 2023-05-25 18:34:22.821551 zep_python-0.30/zep_python/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-25 18:34:22.821551 zep_python-0.30/zep_python/exceptions.py
--rw-r--r--   0        0        0     4956 2023-05-25 18:34:22.821551 zep_python-0.30/zep_python/models.py
--rw-r--r--   0        0        0        0 2023-05-25 18:34:22.821551 zep_python-0.30/zep_python/py.typed
--rw-r--r--   0        0        0    13465 2023-05-25 18:34:22.821551 zep_python-0.30/zep_python/zep_client.py
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 zep_python-0.30/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-05 15:48:33.601814 zep_python-0.31/LICENSE
+-rw-r--r--   0        0        0     2402 2023-06-05 15:48:33.605814 zep_python-0.31/README.md
+-rw-r--r--   0        0        0      872 2023-06-05 15:48:33.605814 zep_python-0.31/pyproject.toml
+-rw-r--r--   0        0        0      389 2023-06-05 15:48:33.605814 zep_python-0.31/zep_python/__init__.py
+-rw-r--r--   0        0        0     1685 2023-06-05 15:48:33.605814 zep_python-0.31/zep_python/exceptions.py
+-rw-r--r--   0        0        0     4882 2023-06-05 15:48:33.605814 zep_python-0.31/zep_python/models.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:48:33.605814 zep_python-0.31/zep_python/py.typed
+-rw-r--r--   0        0        0    13286 2023-06-05 15:48:33.605814 zep_python-0.31/zep_python/zep_client.py
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 zep_python-0.31/PKG-INFO
```

### Comparing `zep_python-0.30/LICENSE` & `zep_python-0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.30/README.md` & `zep_python-0.31/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![Tests](https://github.com/getzep/zep-python/actions/workflows/test.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/test.yml) [![lint](https://github.com/getzep/zep-python/actions/workflows/lint.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/lint.yml) [![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/getzep/zep-python?color=blue)
 
 # Zep: A long-term memory store for conversational AI applications
 
 This is the Python client package for the Zep service. For more information about Zep, see https://github.com/getzep/zep.
 
-Zep documentation: [https://getzep.github.io](https://getzep.github.io/)
+Zep documentation: [https://docs.getzep.com](https://docs.getzep.com/)
 
 ## Installation
 
 ```bash
 pip install zep-python
 ```
 
@@ -21,39 +21,38 @@
 ## Quick Start
 
 Ensure that you have a Zep server running. See https://github.com/getzep/zep.
 
 ```python
 import asyncio
 
-from zep_python import Memory, Message, SearchPayload, ZepClient
+from zep_python import Memory, Message, MemorySearchPayload, ZepClient
 
 base_url = "http://localhost:8000"  # TODO: Replace with Zep API URL
-session_id = "2a2a2a" # an identifier for your user's session.
+session_id = "2a2a2a"  # an identifier for your user's session.
 
 async with ZepClient(base_url) as client:
-
     role = "user"
     content = "who was the first man to go to space?"
     message = Message(role=role, content=content)
     memory = Memory()
     memory.messages = [message]
     # Add a memory
     result = await client.aadd_memory(session_id, memory)
 
     # Long chat histories will automatically be summarized.
     # A summary and chat history are returned with a `get_memory`
     memory = await client.aget_memory(session_id)
     for message in memory.messages:
-         print(message.to_dict())
+        print(message.to_dict())
 
     # Search memory
     # Messages uploaded to Zep are automatically embedded and made available
     # for vector-based similarity search.
-    search_payload = SearchPayload("Who is Yuri Gagarin?")
+    search_payload = MemorySearchPayload("Who is Yuri Gagarin?")
     search_results = await client.asearch_memory(session_id, search_payload)
     for search_result in search_results:
         # Access the 'content' field within the 'message' object.
         message_content = search_result.message
         print(message_content)
 ```
```

### Comparing `zep_python-0.30/pyproject.toml` & `zep_python-0.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.30"
+version = "0.31"
 description = "Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.0"
```

### Comparing `zep_python-0.30/zep_python/exceptions.py` & `zep_python-0.31/zep_python/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
+
+import httpx
 
 
 class ZepClientError(Exception):
     """
     Base exception class for ZepClient errors.
 
     Attributes
@@ -22,26 +24,39 @@
         The response data to be set for the exception, by default None.
     """
 
     def __init__(
         self, message: str, response_data: Optional[Dict[Any, Any]] = None
     ) -> None:
         super().__init__(message)
+        self.message = message
         self.response_data = response_data
 
+    def __str__(self):
+        return f"{self.message}: {self.response_data}"
+
 
 class APIError(ZepClientError):
     """
     Raised when the API response format is unexpected.
 
     Inherits from ZepClientError.
     """
 
-    def __init__(self, message: str) -> None:
-        super().__init__(message)
+    def __init__(
+        self, response: Union[httpx.Response, None] = None, message: str = "API error"
+    ) -> None:
+        if response:
+            response_data = {
+                "status_code": response.status_code,
+                "message": response.text,
+            }
+        else:
+            response_data = None
+        super().__init__(message=message, response_data=response_data)
 
 
 class NotFoundError(ZepClientError):
     """
     Raised when the API response contains no results.
 
     Inherits from ZepClientError.
```

### Comparing `zep_python-0.30/zep_python/models.py` & `zep_python-0.31/zep_python/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,46 +122,43 @@
     created_at: Optional[str] = Field(optional=True, default=None)
     token_count: Optional[int] = Field(optional=True, default=None)
 
     def to_dict(self) -> Dict[str, Any]:
         return self.dict()
 
 
-class SearchPayload(BaseModel):
+class MemorySearchPayload(BaseModel):
     """
     Represents a search payload for querying memory.
 
     Attributes
     ----------
-    meta : Dict[str, Any]
+    metadata : Dict[str, Any]
         Metadata associated with the search query.
     text : str
         The text of the search query.
     """
 
     text: str = Field("A text is required")
-    meta: Optional[Dict[str, Any]] = Field(optional=True, default=None)
+    metadata: Optional[Dict[str, Any]] = Field(optional=True, default=None)
 
 
-class SearchResult(BaseModel):
+class MemorySearchResult(BaseModel):
     """
     Represents a search result from querying memory.
 
     Attributes
     ----------
     message : Optional[Dict[str, Any]]
         The message associated with the search result.
-    meta : Optional[Dict[str, Any]]
+    metadata : Optional[Dict[str, Any]]
         Metadata associated with the search result.
-    score : Optional[float]
-        The score of the search result.
     summary : Optional[str]
         The summary of the search result.
     dist : Optional[float]
         The distance metric of the search result.
     """
 
     message: Optional[Dict[str, Any]] = None
-    meta: Optional[Dict[str, Any]] = None
-    score: Optional[float] = None
+    metadata: Optional[Dict[str, Any]] = None
     summary: Optional[str] = None
     dist: Optional[float] = None
```

### Comparing `zep_python-0.30/zep_python/zep_client.py` & `zep_python-0.31/zep_python/zep_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 from types import TracebackType
 from typing import Any, Dict, List, Optional, Type
 
 import httpx
 
 from zep_python.exceptions import APIError, NotFoundError
-from zep_python.models import Memory, Message, SearchPayload, SearchResult, Summary
+from zep_python.models import (
+    Memory,
+    MemorySearchPayload,
+    MemorySearchResult,
+    Message,
+    Summary,
+)
 
 API_BASE_PATH = "/api/v1"
 
 
 class ZepClient:
     """
     ZepClient class implementation.
@@ -82,15 +88,15 @@
         try:
             messages = [
                 Message.parse_obj(m) for m in response_data.get("messages", None)
             ]
             if len(messages) == 0:
                 raise ValueError("Messages can't be empty")
         except (TypeError, ValueError) as e:
-            raise APIError("Unexpected response format from the API") from e
+            raise APIError(message="Unexpected response format from the API") from e
 
         summary: Optional[Summary] = None
         if response_data.get("summary", None) is not None:
             summary = Summary.parse_obj(response_data["summary"])
 
         memory = Memory(
             messages=messages,
@@ -137,15 +143,15 @@
         params = self._gen_get_params(lastn)
         response = self.client.get(url, params=params)
 
         if response.status_code == 404:
             raise NotFoundError(f"No memory found for session {session_id}")
 
         if response.status_code != 200:
-            raise APIError(f"Unexpected status code: {response.status_code}")
+            raise APIError(response)
 
         response_data = response.json()
 
         return self._parse_get_memory_response(response_data)
 
     async def aget_memory(self, session_id: str, lastn: Optional[int] = None) -> Memory:
         """
@@ -176,15 +182,15 @@
         params = self._gen_get_params(lastn)
         response = await self.aclient.get(url, params=params)
 
         if response.status_code == 404:
             raise NotFoundError(f"No memory found for session {session_id}")
 
         if response.status_code != 200:
-            raise APIError(f"Unexpected status code: {response.status_code}")
+            raise APIError(response)
 
         response_data = response.json()
 
         return self._parse_get_memory_response(response_data)
 
     def add_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
@@ -211,15 +217,15 @@
             raise ValueError("session_id must be provided")
 
         response = self.client.post(
             f"/sessions/{session_id}/memory",
             json=memory_messages.dict(exclude_none=True),
         )
         if response.status_code != 200:
-            raise APIError(f"Unexpected status code: {response.status_code}")
+            raise APIError(response)
 
         return response.text
 
     async def aadd_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
         Asynchronously add memory to the specified session.
 
@@ -244,15 +250,15 @@
             raise ValueError("session_id must be provided")
 
         response = await self.aclient.post(
             f"/sessions/{session_id}/memory",
             json=memory_messages.dict(exclude_none=True),
         )
         if response.status_code != 200:
-            raise APIError(f"Unexpected status code: {response.status_code}")
+            raise APIError(response)
 
         return response.text
 
     def delete_memory(self, session_id: str) -> str:
         """
         Delete memory for the specified session.
 
@@ -275,15 +281,15 @@
             raise ValueError("session_id must be provided")
 
         response = self.client.delete(f"/sessions/{session_id}/memory")
         if response.status_code == 404:
             raise NotFoundError(f"No session found for session {session_id}")
 
         if response.status_code != 200:
-            raise APIError(f"Unexpected status code: {response.status_code}")
+            raise APIError(response)
         return response.text
 
     async def adelete_memory(self, session_id: str) -> str:
         """
         Asynchronously delete memory for the specified session.
 
         Parameters
@@ -305,38 +311,38 @@
             raise ValueError("session_id must be provided")
 
         response = await self.aclient.delete(f"/sessions/{session_id}/memory")
         if response.status_code == 404:
             raise NotFoundError(f"No session found for session {session_id}")
 
         if response.status_code != 200:
-            raise APIError(f"Unexpected status code: {response.status_code}")
+            raise APIError(response)
         return response.text
 
     def search_memory(
         self,
         session_id: str,
-        search_payload: SearchPayload,
+        search_payload: MemorySearchPayload,
         limit: Optional[int] = None,
-    ) -> List[SearchResult]:
+    ) -> List[MemorySearchResult]:
         """
         Search memory for the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session for which memory should be searched.
-        search_payload : SearchPayload
+        search_payload : MemorySearchPayload
             A SearchPayload object representing the search query.
         limit : Optional[int], optional
             The maximum number of search results to return. Defaults to None (no limit).
 
         Returns
         -------
-        List[SearchResult]
+        List[MemorySearchResult]
             A list of SearchResult objects representing the search results.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
@@ -351,38 +357,40 @@
             f"/sessions/{session_id}/search",
             json=search_payload.dict(),
             params=params,
         )
         if response.status_code == 404:
             raise NotFoundError("No query results found")
         if response.status_code != 200:
-            raise APIError(f"Unexpected status code: {response.status_code}")
-        return [SearchResult(**search_result) for search_result in response.json()]
+            raise APIError(response)
+        return [
+            MemorySearchResult(**search_result) for search_result in response.json()
+        ]
 
     async def asearch_memory(
         self,
         session_id: str,
-        search_payload: SearchPayload,
+        search_payload: MemorySearchPayload,
         limit: Optional[int] = None,
-    ) -> List[SearchResult]:
+    ) -> List[MemorySearchResult]:
         """
         Asynchronously search memory for the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session for which memory should be searched.
-        search_payload : SearchPayload
+        search_payload : MemorySearchPayload
             A SearchPayload object representing the search query.
         limit : Optional[int], optional
             The maximum number of search results to return. Defaults to None (no limit).
 
         Returns
         -------
-        List[SearchResult]
+        List[MemorySearchResult]
             A list of SearchResult objects representing the search results.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
@@ -397,16 +405,18 @@
             f"/sessions/{session_id}/search",
             json=search_payload.dict(),
             params=params,
         )
         if response.status_code == 404:
             raise NotFoundError("No query results found")
         if response.status_code != 200:
-            raise APIError(f"Unexpected status code: {response.status_code}")
-        return [SearchResult(**search_result) for search_result in response.json()]
+            raise APIError(response)
+        return [
+            MemorySearchResult(**search_result) for search_result in response.json()
+        ]
 
     async def aclose(self) -> None:
         """
         Asynchronously close the HTTP client.
 
         [Optional] This method may be called when the ZepClient is no longer needed to
         release resources.
```

### Comparing `zep_python-0.30/PKG-INFO` & `zep_python-0.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 0.30
+Version: 0.31
 Summary: Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 
 [![Tests](https://github.com/getzep/zep-python/actions/workflows/test.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/test.yml) [![lint](https://github.com/getzep/zep-python/actions/workflows/lint.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/lint.yml) [![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/getzep/zep-python?color=blue)
 
 # Zep: A long-term memory store for conversational AI applications
 
 This is the Python client package for the Zep service. For more information about Zep, see https://github.com/getzep/zep.
 
-Zep documentation: [https://getzep.github.io](https://getzep.github.io/)
+Zep documentation: [https://docs.getzep.com](https://docs.getzep.com/)
 
 ## Installation
 
 ```bash
 pip install zep-python
 ```
 
@@ -37,39 +37,38 @@
 ## Quick Start
 
 Ensure that you have a Zep server running. See https://github.com/getzep/zep.
 
 ```python
 import asyncio
 
-from zep_python import Memory, Message, SearchPayload, ZepClient
+from zep_python import Memory, Message, MemorySearchPayload, ZepClient
 
 base_url = "http://localhost:8000"  # TODO: Replace with Zep API URL
-session_id = "2a2a2a" # an identifier for your user's session.
+session_id = "2a2a2a"  # an identifier for your user's session.
 
 async with ZepClient(base_url) as client:
-
     role = "user"
     content = "who was the first man to go to space?"
     message = Message(role=role, content=content)
     memory = Memory()
     memory.messages = [message]
     # Add a memory
     result = await client.aadd_memory(session_id, memory)
 
     # Long chat histories will automatically be summarized.
     # A summary and chat history are returned with a `get_memory`
     memory = await client.aget_memory(session_id)
     for message in memory.messages:
-         print(message.to_dict())
+        print(message.to_dict())
 
     # Search memory
     # Messages uploaded to Zep are automatically embedded and made available
     # for vector-based similarity search.
-    search_payload = SearchPayload("Who is Yuri Gagarin?")
+    search_payload = MemorySearchPayload("Who is Yuri Gagarin?")
     search_results = await client.asearch_memory(session_id, search_payload)
     for search_result in search_results:
         # Access the 'content' field within the 'message' object.
         message_content = search_result.message
         print(message_content)
 ```
```

