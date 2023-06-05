# Comparing `tmp/reduct_py-1.4.0-py3-none-any.whl.zip` & `tmp/reduct_py-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10242 bytes, number of entries: 10
--rw-r--r--  2.0 unx      320 b- defN 23-May-29 21:15 reduct/__init__.py
--rw-r--r--  2.0 unx    11150 b- defN 23-May-29 21:15 reduct/bucket.py
--rw-r--r--  2.0 unx     6151 b- defN 23-May-29 21:15 reduct/client.py
--rw-r--r--  2.0 unx      481 b- defN 23-May-29 21:15 reduct/error.py
--rw-r--r--  2.0 unx     3188 b- defN 23-May-29 21:15 reduct/http.py
--rw-r--r--  2.0 unx     1069 b- defN 23-May-29 21:15 reduct_py-1.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5002 b- defN 23-May-29 21:15 reduct_py-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 21:15 reduct_py-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-29 21:15 reduct_py-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      758 b- defN 23-May-29 21:15 reduct_py-1.4.0.dist-info/RECORD
-10 files, 28218 bytes uncompressed, 8964 bytes compressed:  68.2%
+Zip file size: 10327 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      320 b- defN 23-Jun-05 21:18 reduct/__init__.py
+-rw-r--r--  2.0 unx    11150 b- defN 23-Jun-05 21:18 reduct/bucket.py
+-rw-r--r--  2.0 unx     6151 b- defN 23-Jun-05 21:18 reduct/client.py
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-05 21:18 reduct/error.py
+-rw-r--r--  2.0 unx     3430 b- defN 23-Jun-05 21:18 reduct/http.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jun-05 21:18 reduct_py-1.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5002 b- defN 23-Jun-05 21:18 reduct_py-1.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 21:18 reduct_py-1.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 21:18 reduct_py-1.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jun-05 21:18 reduct_py-1.4.1.dist-info/RECORD
+10 files, 28460 bytes uncompressed, 9049 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: reduct/error.py
 Comment: 
 
 Filename: reduct/http.py
 Comment: 
 
-Filename: reduct_py-1.4.0.dist-info/LICENSE
+Filename: reduct_py-1.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: reduct_py-1.4.0.dist-info/METADATA
+Filename: reduct_py-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: reduct_py-1.4.0.dist-info/WHEEL
+Filename: reduct_py-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: reduct_py-1.4.0.dist-info/top_level.txt
+Filename: reduct_py-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: reduct_py-1.4.0.dist-info/RECORD
+Filename: reduct_py-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reduct/http.py

```diff
@@ -10,57 +10,65 @@
 
 API_PREFIX = "/api/v1"
 
 
 class HttpClient:
     """Wrapper for HTTP calls"""
 
+    FILE_SIZE_FOR_100_CONTINUE = 256_000
+
     def __init__(
         self, url: str, api_token: Optional[str] = None, timeout: Optional[float] = None
     ):
         self.url = url + API_PREFIX
         self.api_token = api_token
         self.headers = (
             {"Authorization": f"Bearer {api_token}"} if api_token is not None else {}
         )
         self.timeout = ClientTimeout(timeout)
+        self.request_count = 0
 
     @asynccontextmanager
     async def request(
         self, method: str, path: str = "", **kwargs
     ) -> AsyncIterator[ClientResponse]:
         """HTTP request with ReductError exception"""
 
         extra_headers = {}
+        expect100 = False
 
         if "content_length" in kwargs:
             content_length = kwargs["content_length"]
             extra_headers["Content-Length"] = str(content_length)
-            if content_length > 256_000:
+            if content_length > self.FILE_SIZE_FOR_100_CONTINUE:
                 # Use 100-continue for large files
-                extra_headers["Expect"] = "100-continue"
+                expect100 = True
 
             del kwargs["content_length"]
 
         if "content_type" in kwargs:
             extra_headers["Content-Type"] = str(kwargs["content_type"])
             del kwargs["content_type"]
 
         if "labels" in kwargs:
             if kwargs["labels"]:
                 for name, value in kwargs["labels"].items():
                     extra_headers[f"x-reduct-label-{name}"] = str(value)
             del kwargs["labels"]
 
-        async with aiohttp.ClientSession(timeout=self.timeout) as session:
+        connector = aiohttp.TCPConnector(force_close=True)
+        async with aiohttp.ClientSession(
+            timeout=self.timeout, connector=connector
+        ) as session:
             try:
                 async with session.request(
                     method,
                     f"{self.url}{path.strip()}",
                     headers=dict(self.headers, **extra_headers),
+                    expect100=expect100,
                     **kwargs,
                 ) as response:
                     if response.ok:
                         yield response
                     else:
                         if "x-reduct-error" in response.headers:
                             raise ReductError(
```

## Comparing `reduct_py-1.4.0.dist-info/LICENSE` & `reduct_py-1.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `reduct_py-1.4.0.dist-info/METADATA` & `reduct_py-1.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reduct-py
-Version: 1.4.0
+Version: 1.4.1
 Summary: ReductStore Client SDK for Python
 Author: Ciaran Moyne
 Author-email: Alexey Timin <atimin@gmail.com>
 Maintainer-email: Alexey Timin <atimin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alexey Timin
```

