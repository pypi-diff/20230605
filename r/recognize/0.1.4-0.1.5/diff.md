# Comparing `tmp/recognize-0.1.4.tar.gz` & `tmp/recognize-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognize-0.1.4.tar", max compression
+gzip compressed data, was "recognize-0.1.5.tar", max compression
```

## Comparing `recognize-0.1.4.tar` & `recognize-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.4/README.md
--rw-r--r--   0        0        0      411 2023-06-05 14:03:36.046511 recognize-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.4/recognize/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.4/recognize/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.4/recognize/commands/lib/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-05 14:02:35.284880 recognize-0.1.4/recognize/commands/lib/client.py
--rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.4/recognize/commands/lib/entries.py
--rw-r--r--   0        0        0     1187 2023-06-05 13:50:58.064038 recognize-0.1.4/recognize/commands/lib/helpers.py
--rw-r--r--   0        0        0     2397 2023-06-05 10:43:58.803222 recognize-0.1.4/recognize/commands/search.py
--rw-r--r--   0        0        0      883 2023-06-05 13:56:21.298465 recognize-0.1.4/recognize/commands/upload.py
--rw-r--r--   0        0        0      192 2023-06-05 13:59:14.826793 recognize-0.1.4/recognize/main.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 recognize-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.5/README.md
+-rw-r--r--   0        0        0      411 2023-06-05 15:51:01.923676 recognize-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.5/recognize/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.5/recognize/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.5/recognize/commands/lib/__init__.py
+-rw-r--r--   0        0        0     3403 2023-06-05 15:43:18.737969 recognize-0.1.5/recognize/commands/lib/client.py
+-rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.5/recognize/commands/lib/entries.py
+-rw-r--r--   0        0        0     1187 2023-06-05 13:50:58.064038 recognize-0.1.5/recognize/commands/lib/helpers.py
+-rw-r--r--   0        0        0     2940 2023-06-05 15:23:37.455666 recognize-0.1.5/recognize/commands/search.py
+-rw-r--r--   0        0        0     1046 2023-06-05 15:23:37.447161 recognize-0.1.5/recognize/commands/upload.py
+-rw-r--r--   0        0        0      192 2023-06-05 13:59:14.826793 recognize-0.1.5/recognize/main.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 recognize-0.1.5/PKG-INFO
```

### Comparing `recognize-0.1.4/recognize/commands/lib/client.py` & `recognize-0.1.5/recognize/commands/lib/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 import rich
 
 from .entries import LabelEntryType
 from .helpers import upload_file
 
 
 class DataAPI:
-    def __init__(self):
-        self.url = os.getenv("ML_API_URL", "https://xxihhslish.execute-api.eu-west-2.amazonaws.com/prod/")
+    def __init__(self, dev: bool = False):
+        self.url = "https://w8hbh06bwj.execute-api.eu-west-2.amazonaws.com/prod/" if not dev else os.getenv(
+            "ML_API_URL", "https://q6550ddu16.execute-api.eu-west-2.amazonaws.com/prod/")
 
     def keyword_search(self, keywords: List[str], output_file: Path, response_type: str):
         url = urljoin(self.url, "search/")
 
         with httpx.stream("GET", url, params={
             "keywords": ",".join(keywords),
             "response_type": response_type
@@ -41,15 +42,16 @@
 
         with httpx.stream("POST", url, params={
             "response_type": response_type
         }, files=files) as response, \
                 open(output_file, "wb") as output:
             self._process_response(output, response)
 
-    async def upload_files(self, base_path, file_paths: Generator[str, None, None], max_concurrent_uploads: int = 50) -> None:
+    async def upload_files(self, base_path, file_paths: Generator[str, None, None],
+                           max_concurrent_uploads: int = 50) -> None:
         """Upload files concurrently to a given URL."""
         url = urljoin(self.url, f"upload/{base_path}")
         semaphore = asyncio.Semaphore(max_concurrent_uploads)
 
         tasks = [upload_file(semaphore, file_path, url) for file_path in file_paths]
 
         with rich.progress.Progress(
```

### Comparing `recognize-0.1.4/recognize/commands/lib/helpers.py` & `recognize-0.1.5/recognize/commands/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `recognize-0.1.4/recognize/commands/search.py` & `recognize-0.1.5/recognize/commands/search.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,60 +5,69 @@
 from typing_extensions import Annotated
 
 from .lib.client import DataAPI
 from .lib.entries import LabelEntryType
 
 short_help_description = "Commands that allow you to search through analysed content."
 app = typer.Typer(help=short_help_description, short_help=short_help_description)
-api = DataAPI()
 
 
 @app.command()
 def keywords(
         words: Annotated[List[str], typer.Argument()],
         output: Annotated[Path, typer.Option()],
-        json: Annotated[bool, typer.Option("--json")] = False
+        json: Annotated[bool, typer.Option("--json")] = False,
+        dev: Annotated[bool, typer.Option("--dev")] = False
 ):
     """
     Execute a keyword search.
 
     :param words: A list of keywords to search for.
     :param output: The output path where the search results will be stored.
     :param json: An optional flag indicating whether the output should be in JSON format. If False, the output is CSV.
+    :param dev: An optional flag indicating whether to use the dev stack. Uses dev stack if True.
     :return: The result of the search operation.
     """
+    api = DataAPI(dev=dev)
     return api.keyword_search(words, output, response_type="csv" if not json else "json")
 
 
 @app.command()
 def entry(
         entry_type: Annotated[LabelEntryType, typer.Argument()],
         output: Annotated[Path, typer.Option()],
-        json: Annotated[bool, typer.Option("--json")] = False
+        json: Annotated[bool, typer.Option("--json")] = False,
+        dev: Annotated[bool, typer.Option("--dev")] = False
 ):
     """
     Execute a search for entries of a specific type.
 
     :param entry_type: The type of entries to search for.
     :param output: The output path where the search results will be stored.
     :param json: An optional flag indicating whether the output should be in JSON format. If False, the output is CSV.
+    :param dev: An optional flag indicating whether to use the dev stack. Uses dev stack if True.
     :return: The result of the search operation.
     """
+    api = DataAPI(dev=dev)
     return api.entry_search(entry_type, output, response_type="csv" if not json else "json")
 
 
 @app.command()
 def faces(
         image_file: Annotated[Path, typer.Argument()],
         output: Annotated[Path, typer.Option()],
-        json: Annotated[bool, typer.Option("--json")] = False
+        json: Annotated[bool, typer.Option("--json")] = False,
+        dev: Annotated[bool, typer.Option("--dev")] = False
 ):
     """
     Execute a face search using a provided image file.
 
     :param image_file: The path to the image file that will be used for the face search.
     :param output: The output path where the search results will be stored.
     :param json: An optional flag indicating whether the output should be in JSON format. If False, the output is CSV.
+    :param dev: An optional flag indicating whether to use the dev stack. Uses dev stack if True.
     :return: The result of the search operation.
     """
+    api = DataAPI(dev=dev)
+
     with open(image_file, 'rb') as fp:
         return api.faces_search(fp, output, response_type="csv" if not json else "json")
```

### Comparing `recognize-0.1.4/recognize/commands/upload.py` & `recognize-0.1.5/recognize/commands/upload.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 
 from .lib.client import DataAPI
 from .lib.helpers import find_files
 
 short_help_description = "Commands that allow you to upload to files and folders into the S3 bucket for analysis."
 help_description = "Commands that allow you to upload to files and folders into the S3 bucket for analysis."
 app = typer.Typer(help=help_description, short_help=short_help_description)
-api = DataAPI()
 
 
 @app.command()
 def directory(
-        path: Annotated[Path, typer.Argument()]
+        path: Annotated[Path, typer.Argument()],
+        dev: Annotated[bool, typer.Option("--dev")] = False
 ):
     """
     Uploads all files of types mp4, and mov from a given directory. In the future we will handle: png, jpeg
 
     :param path: The directory path from which files will be retrieved and uploaded.
+    :param dev: An optional flag indicating whether to use the dev stack. Uses dev stack if True.
     :return: None
     """
+    api = DataAPI()
     files = find_files(path)
     asyncio.run(api.upload_files(path.absolute().name, files))
```

