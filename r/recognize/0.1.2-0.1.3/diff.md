# Comparing `tmp/recognize-0.1.2.tar.gz` & `tmp/recognize-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognize-0.1.2.tar", max compression
+gzip compressed data, was "recognize-0.1.3.tar", max compression
```

## Comparing `recognize-0.1.2.tar` & `recognize-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.2/README.md
--rw-r--r--   0        0        0      411 2023-06-05 12:03:56.314307 recognize-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.2/recognize/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.2/recognize/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.2/recognize/commands/lib/__init__.py
--rw-r--r--   0        0        0     3067 2023-06-05 12:03:45.080067 recognize-0.1.2/recognize/commands/lib/client.py
--rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.2/recognize/commands/lib/entries.py
--rw-r--r--   0        0        0      848 2023-06-05 10:43:58.881956 recognize-0.1.2/recognize/commands/lib/helpers.py
--rw-r--r--   0        0        0     2397 2023-06-05 10:43:58.803222 recognize-0.1.2/recognize/commands/search.py
--rw-r--r--   0        0        0      854 2023-06-05 10:43:58.853929 recognize-0.1.2/recognize/commands/upload.py
--rw-r--r--   0        0        0      192 2023-06-05 10:55:55.812878 recognize-0.1.2/recognize/main.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 recognize-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.3/README.md
+-rw-r--r--   0        0        0      411 2023-06-05 12:43:55.168193 recognize-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.3/recognize/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.3/recognize/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.3/recognize/commands/lib/__init__.py
+-rw-r--r--   0        0        0     3175 2023-06-05 12:43:33.169448 recognize-0.1.3/recognize/commands/lib/client.py
+-rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.3/recognize/commands/lib/entries.py
+-rw-r--r--   0        0        0      946 2023-06-05 12:42:10.133402 recognize-0.1.3/recognize/commands/lib/helpers.py
+-rw-r--r--   0        0        0     2397 2023-06-05 10:43:58.803222 recognize-0.1.3/recognize/commands/search.py
+-rw-r--r--   0        0        0      854 2023-06-05 10:43:58.853929 recognize-0.1.3/recognize/commands/upload.py
+-rw-r--r--   0        0        0      192 2023-06-05 10:55:55.812878 recognize-0.1.3/recognize/main.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 recognize-0.1.3/PKG-INFO
```

### Comparing `recognize-0.1.2/recognize/commands/lib/client.py` & `recognize-0.1.3/recognize/commands/lib/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,20 @@
 
         with httpx.stream("POST", url, params={
             "response_type": response_type
         }, files=files) as response, \
                 open(output_file, "wb") as output:
             self._process_response(output, response)
 
-    async def upload_files(self, base_path, file_paths: Generator[str, None, None]) -> None:
+    async def upload_files(self, base_path, file_paths: Generator[str, None, None], max_concurrent_uploads: int = 50) -> None:
         """Upload files concurrently to a given URL."""
         url = urljoin(self.url, f"upload/{base_path}")
-        tasks = [upload_file(file_path, url) for file_path in file_paths]
+        semaphore = asyncio.Semaphore(max_concurrent_uploads)
+
+        tasks = [upload_file(semaphore, file_path, url) for file_path in file_paths]
 
         with rich.progress.Progress(
                 "[progress.percentage]{task.percentage:>3.0f}%",
                 rich.progress.BarColumn(bar_width=None),
                 rich.progress.MofNCompleteColumn(),
                 rich.progress.TransferSpeedColumn(),
                 rich.progress.TimeRemainingColumn(),
```

### Comparing `recognize-0.1.2/recognize/commands/lib/helpers.py` & `recognize-0.1.3/recognize/commands/lib/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 import re
+from asyncio import Semaphore
 from pathlib import Path
 from typing import Generator
 
 import httpx
 
 
-async def upload_file(file_path: str, url: str) -> str:
+async def upload_file(semaphore: Semaphore, file_path: str, url: str) -> str:
     """Asynchronously upload a file to a given URL."""
     with open(file_path, 'rb') as fp:
         files = {'file': (fp.name, fp)}
 
         async with httpx.AsyncClient() as client:
-            async with client.stream('POST', url, files=files) as response:
-                response.raise_for_status()  # Ensure we get a 2xx response
-                return file_path
+            async with semaphore:
+                async with client.stream('POST', url, files=files) as response:
+                    response.raise_for_status()  # Ensure we get a 2xx response
+                    return file_path
 
 
 def find_files(filepath: Path) -> Generator[str, None, None]:
     pattern = re.compile(r'\.(jpeg|jpg|png|mp4|mov)$')
 
     for root, dirs, files in os.walk(filepath.absolute()):
         for file in files:
```

### Comparing `recognize-0.1.2/recognize/commands/search.py` & `recognize-0.1.3/recognize/commands/search.py`

 * *Files identical despite different names*

### Comparing `recognize-0.1.2/recognize/commands/upload.py` & `recognize-0.1.3/recognize/commands/upload.py`

 * *Files identical despite different names*

