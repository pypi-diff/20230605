# Comparing `tmp/recognize-0.1.3.tar.gz` & `tmp/recognize-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognize-0.1.3.tar", max compression
+gzip compressed data, was "recognize-0.1.4.tar", max compression
```

## Comparing `recognize-0.1.3.tar` & `recognize-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.3/README.md
--rw-r--r--   0        0        0      411 2023-06-05 12:43:55.168193 recognize-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.3/recognize/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.3/recognize/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.3/recognize/commands/lib/__init__.py
--rw-r--r--   0        0        0     3175 2023-06-05 12:43:33.169448 recognize-0.1.3/recognize/commands/lib/client.py
--rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.3/recognize/commands/lib/entries.py
--rw-r--r--   0        0        0      946 2023-06-05 12:42:10.133402 recognize-0.1.3/recognize/commands/lib/helpers.py
--rw-r--r--   0        0        0     2397 2023-06-05 10:43:58.803222 recognize-0.1.3/recognize/commands/search.py
--rw-r--r--   0        0        0      854 2023-06-05 10:43:58.853929 recognize-0.1.3/recognize/commands/upload.py
--rw-r--r--   0        0        0      192 2023-06-05 10:55:55.812878 recognize-0.1.3/recognize/main.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 recognize-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.4/README.md
+-rw-r--r--   0        0        0      411 2023-06-05 14:03:36.046511 recognize-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.4/recognize/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.4/recognize/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.4/recognize/commands/lib/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-05 14:02:35.284880 recognize-0.1.4/recognize/commands/lib/client.py
+-rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.4/recognize/commands/lib/entries.py
+-rw-r--r--   0        0        0     1187 2023-06-05 13:50:58.064038 recognize-0.1.4/recognize/commands/lib/helpers.py
+-rw-r--r--   0        0        0     2397 2023-06-05 10:43:58.803222 recognize-0.1.4/recognize/commands/search.py
+-rw-r--r--   0        0        0      883 2023-06-05 13:56:21.298465 recognize-0.1.4/recognize/commands/upload.py
+-rw-r--r--   0        0        0      192 2023-06-05 13:59:14.826793 recognize-0.1.4/recognize/main.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 recognize-0.1.4/PKG-INFO
```

### Comparing `recognize-0.1.3/recognize/commands/lib/client.py` & `recognize-0.1.4/recognize/commands/lib/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import asyncio
+import os
 from pathlib import Path
 from typing import List, IO, Generator
 from urllib.parse import urljoin
 
 import httpx
 import rich
 
 from .entries import LabelEntryType
 from .helpers import upload_file
 
 
 class DataAPI:
     def __init__(self):
-        self.url = "https://xxihhslish.execute-api.eu-west-2.amazonaws.com/prod/"
+        self.url = os.getenv("ML_API_URL", "https://xxihhslish.execute-api.eu-west-2.amazonaws.com/prod/")
 
     def keyword_search(self, keywords: List[str], output_file: Path, response_type: str):
         url = urljoin(self.url, "search/")
 
         with httpx.stream("GET", url, params={
             "keywords": ",".join(keywords),
             "response_type": response_type
@@ -51,21 +52,21 @@
 
         tasks = [upload_file(semaphore, file_path, url) for file_path in file_paths]
 
         with rich.progress.Progress(
                 "[progress.percentage]{task.percentage:>3.0f}%",
                 rich.progress.BarColumn(bar_width=None),
                 rich.progress.MofNCompleteColumn(),
-                rich.progress.TransferSpeedColumn(),
                 rich.progress.TimeRemainingColumn(),
         ) as progress:
-            download_task = progress.add_task("Upload", total=len(tasks))
+            download_task = progress.add_task(description="Uploading files...", total=len(tasks))
 
-            for response in await asyncio.gather(*tasks):
-                progress.console.print(f"Uploaded: {response}")
+            for task in asyncio.as_completed(tasks):
+                path, success = await task
+                progress.console.print(f"{'[bold blue]Uploaded' if success else '[bold red]Failed'}: {path}")
                 progress.update(download_task, advance=1)
 
     @staticmethod
     def _process_response(output, response):
         total = int(response.headers.get("Content-Length"))
 
         with rich.progress.Progress(
```

### Comparing `recognize-0.1.3/recognize/commands/lib/helpers.py` & `recognize-0.1.4/recognize/commands/lib/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import os
 import re
 from asyncio import Semaphore
 from pathlib import Path
-from typing import Generator
+from typing import Generator, Tuple
 
 import httpx
+from httpx import HTTPStatusError
 
 
-async def upload_file(semaphore: Semaphore, file_path: str, url: str) -> str:
+async def upload_file(semaphore: Semaphore, file_path: str, url: str) -> Tuple[str, bool]:
     """Asynchronously upload a file to a given URL."""
     with open(file_path, 'rb') as fp:
         files = {'file': (fp.name, fp)}
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=120.0) as client:
             async with semaphore:
                 async with client.stream('POST', url, files=files) as response:
-                    response.raise_for_status()  # Ensure we get a 2xx response
-                    return file_path
+                    try:
+                        response.raise_for_status()
+                        return file_path, True
+                    except HTTPStatusError:  # Ensure we get a 2xx response
+                        return file_path, False
 
 
 def find_files(filepath: Path) -> Generator[str, None, None]:
-    pattern = re.compile(r'\.(jpeg|jpg|png|mp4|mov)$')
-
+    # pattern = re.compile(r'\.(jpeg|jpg|png|mp4|mov)$')
+    pattern = re.compile(r'\.(mp4|mov)$')
     for root, dirs, files in os.walk(filepath.absolute()):
         for file in files:
             lowered = file.lower()
 
             if re.search(pattern, lowered):
                 yield os.path.join(root, file)
```

### Comparing `recognize-0.1.3/recognize/commands/search.py` & `recognize-0.1.4/recognize/commands/search.py`

 * *Files identical despite different names*

### Comparing `recognize-0.1.3/recognize/commands/upload.py` & `recognize-0.1.4/recognize/commands/upload.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 
 
 @app.command()
 def directory(
         path: Annotated[Path, typer.Argument()]
 ):
     """
-    Uploads all files of types png, jpeg, mp4, and mov from a given directory.
+    Uploads all files of types mp4, and mov from a given directory. In the future we will handle: png, jpeg
 
     :param path: The directory path from which files will be retrieved and uploaded.
     :return: None
     """
     files = find_files(path)
     asyncio.run(api.upload_files(path.absolute().name, files))
```

