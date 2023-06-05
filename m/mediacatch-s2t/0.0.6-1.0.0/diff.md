# Comparing `tmp/mediacatch-s2t-0.0.6.tar.gz` & `tmp/mediacatch-s2t-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediacatch-s2t-0.0.6.tar", last modified: Wed May  3 13:37:41 2023, max compression
+gzip compressed data, was "/home/runner/work/mediacatch-s2t/mediacatch-s2t/dist/.tmp-30zie4fq/mediacatch-s2t-1.0.0.tar", last modified: Mon Jun  5 06:41:01 2023, max compression
```

## Comparing `mediacatch-s2t-0.0.6.tar` & `mediacatch-s2t-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/
--rw-rw-r--   0 frederik  (1002) mc       (10000)    10172 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.6/LICENSE
--rw-rw-r--   0 frederik  (1002) mc       (10000)       27 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.6/MANIFEST.in
--rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/PKG-INFO
--rw-rw-r--   0 frederik  (1002) mc       (10000)      795 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.6/README.md
--rw-rw-r--   0 frederik  (1002) mc       (10000)      899 2023-05-03 13:35:20.000000 mediacatch-s2t-0.0.6/pyproject.toml
--rw-rw-r--   0 frederik  (1002) mc       (10000)       38 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/setup.cfg
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/src/
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/src/mediacatch_s2t/
--rw-rw-r--   0 frederik  (1002) mc       (10000)      994 2023-05-03 13:35:01.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t/__init__.py
--rw-rw-r--   0 frederik  (1002) mc       (10000)     1297 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t/__main__.py
--rw-rw-r--   0 frederik  (1002) mc       (10000)    14007 2023-05-03 13:35:01.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t/uploader.py
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/
--rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/PKG-INFO
--rw-rw-r--   0 frederik  (1002) mc       (10000)      445 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/SOURCES.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)        1 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/dependency_links.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)       54 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/entry_points.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)       80 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/requires.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)       15 2023-05-03 13:37:41.000000 mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/top_level.txt
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-05-03 13:37:41.639331 mediacatch-s2t-0.0.6/tests/
--rw-rw-r--   0 frederik  (1002) mc       (10000)    10862 2023-05-03 13:35:01.000000 mediacatch-s2t-0.0.6/tests/test_multipart_upload.py
--rw-rw-r--   0 frederik  (1002) mc       (10000)     2884 2023-05-03 13:35:01.000000 mediacatch-s2t-0.0.6/tests/test_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/tests/test_multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/tests/test_uploader.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mediacatch-s2t-0.0.6/LICENSE` & `mediacatch-s2t-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.0.6/PKG-INFO` & `mediacatch-s2t-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 0.0.6
+Version: 1.0.0
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -200,12 +200,25 @@
 ```bash
 pip install mediacatch_s2t
 
 python -m mediacatch_s2t <api_key> <path/to/your/media/file>
 ```
 
 Or import it as a module
-```bash
+```python
 from mediacatch_s2t.uploader import upload_and_get_transcription
 
+
+'''
+The result will be a JSON object:
+{
+  "url": "url-to-your-transcription",
+  "status": "uploaded",
+  "estimated_processing_time": "your-estimated-time-to-get-your-transcription-done",
+  "message": "The file has been uploaded."
+}
+
+'''
 result = upload_and_get_transcription('path/to/your/media/file', 'api_key')
 ```
+
+
```

### Comparing `mediacatch-s2t-0.0.6/pyproject.toml` & `mediacatch-s2t-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mediacatch-s2t"
-version = "0.0.6"
+version = '1.0.0'
 description = "Upload a media file and get the transcription link."
 readme = "README.md"
 authors = [{ name = "MediaCatch", email = "support@mediacatch.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["mediacatch", "speech to text", "uploader", "nlp"]
 dependencies = [
-    "pymediainfo",
+    "importlib_metadata",
     "requests",
     "rich"
 ]
 requires-python = ">=3.7"
 
     [project.optional-dependencies]
     dev = ["black", "bumpver", "isort", "pip-tools", "pytest", "responses"]
```

### Comparing `mediacatch-s2t-0.0.6/src/mediacatch_s2t/__main__.py` & `mediacatch-s2t-1.0.0/src/mediacatch_s2t/__main__.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.0.6/src/mediacatch_s2t/uploader.py` & `mediacatch-s2t-1.0.0/src/mediacatch_s2t/uploader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import json
+import abc
 import os
 import pathlib
-import shutil
-import tempfile
+import threading
 
 import requests
 import subprocess
 import json
 from typing import NamedTuple
 
 from mediacatch_s2t import (
     URL,
     SINGLE_UPLOAD_ENDPOINT, TRANSCRIPT_ENDPOINT, UPDATE_STATUS_ENDPOINT,
     MULTIPART_UPLOAD_CREATE_ENDPOINT, MULTIPART_UPLOAD_URL_ENDPOINT,
     MULTIPART_UPLOAD_COMPLETE_ENDPOINT,
-    PROCESSING_TIME_RATIO, CHUNK_SIZE_MIN
+    PROCESSING_TIME_RATIO, MULTIPART_FILESIZE
 )
+from mediacatch_s2t.helper import update_myself
 
 
 class FFProbeResult(NamedTuple):
     return_code: int
     json: str
     error: str
 
@@ -33,47 +33,55 @@
     def __str__(self):
         if self.cause:
             return "{}: {}".format(self.message, str(self.cause))
         else:
             return self.message
 
 
-class UploaderBase:
+class UploaderBase(metaclass=abc.ABCMeta):
     def __init__(self, file, api_key, language='da'):
         self.file = file
         self.api_key = api_key
         self.language = language
         self.file_id = None
 
     def _is_file_exist(self):
         return pathlib.Path(self.file).is_file()
 
     def is_multipart_upload(self) -> bool:
         if self._is_file_exist():
             filesize = os.path.getsize(self.file)
-            if filesize > CHUNK_SIZE_MIN:
+            if filesize > MULTIPART_FILESIZE:
                 return True
         return False
 
     def _is_response_error(self, response):
         if response.status_code >= 400:
             if response.status_code == 401:
                 return True, response.json()['message']
             return True, response.json()['message']
         return False, ''
 
     def _make_post_request(self, *args, **kwargs):
-        try:
+        """Make post request with retry mechanism."""
+        call_limit = 3
+        is_error, msg = True, "Have not made a request call."
+        for _call in range(call_limit):
             response = requests.post(*args, **kwargs)
             is_error, msg = self._is_response_error(response)
-            if is_error:
-                raise Exception(msg)
-            return response
-        except Exception as e:
-            raise UploaderException("Error during post request") from e
+            if not is_error:
+                break
+        if is_error:
+            url = kwargs.get('url')
+            if not url:
+                url, *rest = args
+            raise UploaderException(
+                f"Error during post request {url}; {msg}"
+            )
+        return response
 
     @property
     def _transcript_link(self):
         return f"{URL}{TRANSCRIPT_ENDPOINT}?id={self.file_id}&api_key={self.api_key}"
 
     @staticmethod
     def _ffprobe(file_path) -> FFProbeResult:
@@ -119,33 +127,14 @@
         """Estimated processing time in seconds"""
 
         if not isinstance(audio_length, int):
             return 0
         processing_time = PROCESSING_TIME_RATIO * audio_length
         return round(processing_time / 1000)
 
-    def _get_upload_url(self, mime_file):
-        response = self._make_post_request(
-            url=f'{URL}{SINGLE_UPLOAD_ENDPOINT}',
-            json=mime_file,
-            headers={
-                "Content-type": 'application/json',
-                "X-API-KEY": self.api_key
-            }
-        )
-        response_data = json.loads(response.text)
-        url = response_data.get('url')
-        data = response_data.get('fields')
-        _id = response_data.get('id')
-        return {
-            "url": url,
-            "fields": data,
-            "id": _id
-        }
-
     def _post_file(self, url, data):
         with open(self.file, 'rb') as f:
             response = self._make_post_request(
                 url,
                 data=data,
                 files={'file': f}
             )
@@ -158,23 +147,52 @@
             headers={
                 "Content-type": 'application/json',
                 "X-API-KEY": self.api_key
             }
         )
         return self._transcript_link
 
+    @abc.abstractmethod
+    def upload_file(self):
+        result = {
+            "url": "",
+            "status": "uploaded",
+            "estimated_processing_time": 0,
+            "message": "The file has been uploaded."
+        }
+        return result
+
 
 class Uploader(UploaderBase):
     """Uploader Class
 
     This class is to send a file to the API server.
     The API server currently only allows file less than 4gb
     to be sent with this upload class.
     """
 
+    def _get_upload_url(self, mime_file):
+        response = self._make_post_request(
+            url=f'{URL}{SINGLE_UPLOAD_ENDPOINT}',
+            json=mime_file,
+            headers={
+                "Content-type": 'application/json',
+                "X-API-KEY": self.api_key
+            }
+        )
+        response_data = json.loads(response.text)
+        url = response_data.get('url')
+        data = response_data.get('fields')
+        _id = response_data.get('id')
+        return {
+            "url": url,
+            "fields": data,
+            "id": _id
+        }
+
     def upload_file(self):
         result = {
             "url": "",
             "status": "",
             "estimated_processing_time": 0,
             "message": ""
         }
@@ -238,15 +256,14 @@
         self.upload_id: str = ""
 
         self.endpoint_create: str = f"{URL}{MULTIPART_UPLOAD_CREATE_ENDPOINT}"
         self.endpoint_signed_url: str = f"{URL}{MULTIPART_UPLOAD_URL_ENDPOINT}"
         self.endpoint_complete: str = f"{URL}{MULTIPART_UPLOAD_COMPLETE_ENDPOINT}"
         self.headers: dict = self._get_headers()
 
-        self.temp_dir: str = ""
         self.etags: list = []
 
         self.result = {
             "url": "",
             "status": "",
             "estimated_processing_time": 0,
             "message": ""
@@ -254,114 +271,82 @@
 
     def _get_headers(self) -> dict:
         return {
             "Content-type": "application/json",
             "X-API-KEY": self.api_key
         }
 
-    def _create_temp_dir_path(self) -> str:
-        prefix = 'mc_s2t_'
-        if self.file_id:
-            prefix += f"{self.file_id}_"
-        temporary_directory = tempfile.mkdtemp(prefix=prefix)
-        return temporary_directory
-
-    def _get_file_path(self, filename: str) -> str:
-        temp_dir = pathlib.Path(self.temp_dir)
-        filepath = temp_dir / filename
-        return str(filepath)
-
-    def _get_latest_chunk_size(self) -> int:
-        is_odd = self.filesize % self.chunk_maxsize
-        if is_odd:
-            total_chunks_filesize_before_the_last = (
-                    self.chunk_maxsize * (self.total_chunks - 1)
-            )
-            last_chunk_filesize = (
-                    self.filesize - total_chunks_filesize_before_the_last
-            )
-        else:
-            last_chunk_filesize = self.chunk_maxsize
-        return last_chunk_filesize
-
-    def _write_chunk_to_temp_file(self, chunk: bytes, filepath: str) -> None:
-        with open(filepath, 'wb') as f:
-            f.write(chunk)
-        return None
-
     def _set_result_error_message(self, msg) -> None:
         self.result["status"] = "error"
         self.result["message"] = msg
 
     def _set_metadata(self, file_id: str, chunk_maxsize: int,
                       total_chunks: int, upload_id: str) -> None:
         self.file_id = file_id
         self.chunk_maxsize = chunk_maxsize
         self.total_chunks = total_chunks
         self.upload_id = upload_id
         return None
 
-    def _tear_down(self):
-        shutil.rmtree(self.temp_dir)
-
     def create_multipart_upload(self, mime_file: dict) -> dict:
         response = self._make_post_request(
             url=self.endpoint_create,
             headers=self.headers,
             json=mime_file
         )
         data: dict = response.json()
         return {
             "chunk_maxsize": data["chunk_maxsize"],
             "file_id": data["file_id"],
             "total_chunks": data["total_chunks"],
             "upload_id": data["upload_id"]
         }
 
-    def split_file_into_chunks(self) -> None:
-        self.temp_dir = self._create_temp_dir_path()
+    def chop_and_upload_chunk(self) -> None:
+        threads = []
         with open(self.file, 'rb') as f:
             part_number = 0
-            latest_chunk_size = self._get_latest_chunk_size()
             while True:
                 part_number += 1
                 chunk_size = self.chunk_maxsize
-                if part_number == self.total_chunks:
-                    chunk_size = latest_chunk_size
                 chunk = f.read(chunk_size)
                 if not chunk:
                     break
-
-                self._write_chunk_to_temp_file(
-                    chunk=chunk,
-                    filepath=self._get_file_path(str(part_number))
-                )
+                thread = threading.Thread(target=self.upload_part,
+                                          args=(part_number, chunk))
+                threads.append(thread)
+                thread.start()
+        for thread in threads:
+            thread.join()
         return None
 
-    def get_signed_url(self, part_number: int) -> str:
+    def _get_signed_url(self, part_number: int) -> str:
         response = self._make_post_request(
             url=self.endpoint_signed_url,
             headers=self.headers,
             json={
                 "file_id": self.file_id,
                 "upload_id": self.upload_id,
                 "part_number": part_number
             }
         )
         data: dict = response.json()
         return data["url"]
 
-    def upload_chunks(self, part_number: int, url: str) -> str:
-        filepath: str = self._get_file_path(str(part_number))
-        with open(filepath, 'rb') as f:
-            file_data = f.read()
+    def _upload_data_chunk_to_bucket(self, url: str, file_data: bytes) -> str:
         response: requests.Response = requests.put(url=url, data=file_data)
         etag: str = response.headers['ETag']
         return etag
 
+    def upload_part(self, part_number: int, file_data: bytes) -> None:
+        url = self._get_signed_url(part_number)
+        etag = self._upload_data_chunk_to_bucket(url, file_data)
+        self.etags.append({'ETag': etag, 'PartNumber': part_number})
+        return None
+
     def complete_the_upload(self) -> bool:
         response: requests.Response = self._make_post_request(
             url=self.endpoint_complete,
             headers=self.headers,
             json={
                 "file_id": self.file_id,
                 "parts": self.etags
@@ -392,35 +377,34 @@
             meta = self.create_multipart_upload(mime_file)
             self._set_metadata(
                 file_id=meta["file_id"],
                 chunk_maxsize=meta["chunk_maxsize"],
                 total_chunks=meta["total_chunks"],
                 upload_id=meta["upload_id"]
             )
-            self.split_file_into_chunks()
-            for part in range(1, self.total_chunks + 1):
-                url = self.get_signed_url(part)
-                etag = self.upload_chunks(part, url)
-                self.etags.append({'ETag': etag, 'PartNumber': part})
+
+            self.chop_and_upload_chunk()
             self.complete_the_upload()
             transcript_link = self._get_transcript_link()
-            self._tear_down()
         except Exception as e:
             self._set_result_error_message(str(e))
             return self.result
 
         self.result = {
             "url": transcript_link,
             "status": "uploaded",
             "estimated_processing_time": self.estimated_result_time(
                 file_duration),
             "message": "The file has been uploaded."
         }
         return self.result
 
 
-def upload_and_get_transcription(file, api_key, language):
-    is_multipart_upload = UploaderBase(
+def upload_and_get_transcription(file, api_key, language) -> dict:
+    is_multipart_upload: bool = Uploader(
         file, api_key, language).is_multipart_upload()
     if is_multipart_upload:
-        return ChunkedFileUploader(file, api_key, language).upload_file()
-    return Uploader(file, api_key, language).upload_file()
+        result: dict = ChunkedFileUploader(file, api_key, language).upload_file()
+    else:
+        result: dict = Uploader(file, api_key, language).upload_file()
+    update_myself()
+    return result
```

### Comparing `mediacatch-s2t-0.0.6/src/mediacatch_s2t.egg-info/PKG-INFO` & `mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 0.0.6
+Version: 1.0.0
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -200,12 +200,25 @@
 ```bash
 pip install mediacatch_s2t
 
 python -m mediacatch_s2t <api_key> <path/to/your/media/file>
 ```
 
 Or import it as a module
-```bash
+```python
 from mediacatch_s2t.uploader import upload_and_get_transcription
 
+
+'''
+The result will be a JSON object:
+{
+  "url": "url-to-your-transcription",
+  "status": "uploaded",
+  "estimated_processing_time": "your-estimated-time-to-get-your-transcription-done",
+  "message": "The file has been uploaded."
+}
+
+'''
 result = upload_and_get_transcription('path/to/your/media/file', 'api_key')
 ```
+
+
```

### Comparing `mediacatch-s2t-0.0.6/tests/test_multipart_upload.py` & `mediacatch-s2t-1.0.0/tests/test_multipart_upload.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 import responses
 
 from mediacatch_s2t import (
     URL, MULTIPART_UPLOAD_CREATE_ENDPOINT, MULTIPART_UPLOAD_URL_ENDPOINT,
     MULTIPART_UPLOAD_COMPLETE_ENDPOINT,
     UPDATE_STATUS_ENDPOINT
 )
-from mediacatch_s2t.uploader import ChunkedFileUploader, UploaderBase
+from mediacatch_s2t.uploader import (
+    ChunkedFileUploader, Uploader, UploaderException)
 
 
 class TestMultipartUpload:
     create_multipart_url = f"{URL}{MULTIPART_UPLOAD_CREATE_ENDPOINT}"
     get_signed_url = f"{URL}{MULTIPART_UPLOAD_URL_ENDPOINT}"
     complete_upload_url = f"{URL}{MULTIPART_UPLOAD_COMPLETE_ENDPOINT}"
     update_status_url = f"{URL}{UPDATE_STATUS_ENDPOINT}"
     chunk_maxsize = 20480000
-    filesize = (5 * chunk_maxsize) + 10000
+    filesize = (500 * chunk_maxsize) + 10000
     file_id = "644f6676997bc2477563246e"
     upload_id = "2~iRldDSPjP1cJCXg-7NmR9Sd4xpX_Cii"
     mime_file = {
         "duration": 1000,
         "filename": "file-test",
         "file_ext": ".mp4",
         "filesize": filesize,
@@ -41,134 +42,82 @@
     @pytest.fixture(autouse=True)
     def _mock_os_getsize(self):
         with mock.patch("os.path.getsize") as mock_getsize:
             mock_getsize.return_value = self.filesize
             yield mock_getsize
 
     @pytest.fixture(autouse=True)
-    def _mock_create_temp_dir_path(self):
-        with mock.patch("mediacatch_s2t.uploader.ChunkedFileUploader._create_temp_dir_path") as mock_mkdtemp:
-            mock_mkdtemp.return_value = "temp_folder"
-            yield mock_mkdtemp
-
-    @pytest.fixture(autouse=True)
     def _mock_builtins_open(self):
         with mock.patch("builtins.open", mock.mock_open(read_data="data")) as mock_open:
             yield mock_open
 
     @pytest.fixture(autouse=True)
     def _mock_get_duration(self):
         with mock.patch("mediacatch_s2t.uploader.ChunkedFileUploader.get_duration") as mock_duration:
             mock_duration.return_value = 100000, {}
             yield mock_duration
 
     @pytest.fixture(autouse=True)
-    def _mock_get_file_path(self):
-        with mock.patch("mediacatch_s2t.uploader.ChunkedFileUploader._get_file_path") as mock_filepath:
-            mock_filepath.return_value = "temp_folder/1"
-            yield mock_filepath
-
-    @pytest.fixture(autouse=True)
-    def _mock_split_file_into_chunks(self):
-        with mock.patch("mediacatch_s2t.uploader.ChunkedFileUploader.split_file_into_chunks") as mock_split:
-            mock_split.return_value = 1000, {}
-            yield mock_split
+    def _mock_chop_and_upload_chunk(self):
+        with mock.patch("mediacatch_s2t.uploader.ChunkedFileUploader.chop_and_upload_chunk") as mocker:
+            mocker.return_value = None
+            yield mocker
 
-    @pytest.fixture(autouse=True)
-    def _mock_tear_down(self):
-        with mock.patch("mediacatch_s2t.uploader.ChunkedFileUploader._tear_down") as mock_teardown:
-            mock_teardown.return_value = None
-            yield mock_teardown
 
     @pytest.fixture()
     def _mock_endpoints(self):
         with responses.RequestsMock() as resp:
             resp.add(
                 responses.POST,
                 self.create_multipart_url,
                 status=200,
                 json={
                     "file_id": self.file_id,
                     "chunk_maxsize": self.chunk_maxsize,
-                    "total_chunks": 5 + 1,
+                    "total_chunks": 500 + 1,
                     "upload_id": self.upload_id
                 }
             )
             resp.add(
                 responses.POST,
-                url=self.get_signed_url,
-                status=200,
-                json={
-                    "file_id": self.file_id,
-                    "upload_id": self.upload_id,
-                    "part_number": 1,
-                    "url": "http://url-for-upoading.file"
-                }
-            )
-            resp.add(
-                responses.POST,
                 url=self.complete_upload_url,
                 status=201
             )
             resp.add(
                 responses.POST,
                 url=self.update_status_url,
                 status=201
             )
-            resp.add(
-                responses.PUT,
-                url="http://url-for-upoading.file",
-                status=200,
-                headers={
-                    "Etag": "a-test-etag"
-                }
-            )
             yield resp
 
     @responses.activate
     def test_create_multipart_upload_return_success(self):
         responses.add(
             responses.POST,
             self.create_multipart_url,
             status=200,
             json={
                 "file_id": self.file_id,
                 "chunk_maxsize": self.chunk_maxsize,
-                "total_chunks": 5 + 1,
+                "total_chunks": 500 + 1,
                 "upload_id": self.upload_id
             }
         )
         file = ChunkedFileUploader(
             file='file-test.mp4',
             api_key='test-key'
         )
         result = file.create_multipart_upload(self.mime_file)
         assert result == {
             "file_id": self.file_id,
             "chunk_maxsize": self.chunk_maxsize,
-            "total_chunks": 5 + 1,
+            "total_chunks": 500 + 1,
             "upload_id": self.upload_id
         }
 
-    def test_split_into_chunk_give_correct_number_and_filesize(self):
-        chunked_file = ChunkedFileUploader("file-test.mp4", "test-key")
-        assert chunked_file._create_temp_dir_path() == 'temp_folder'
-
-        chunked_file.chunk_maxsize = self.chunk_maxsize
-        chunked_file.filesize = self.filesize
-        chunked_file.total_chunks = 5 + 1
-        latest_chunk_size = chunked_file._get_latest_chunk_size()
-        assert latest_chunk_size == 10000
-
-        chunked_file.chunk_maxsize = self.chunk_maxsize
-        chunked_file.filesize = self.chunk_maxsize
-        chunked_file.total_chunks = 1
-        latest_chunk_size = chunked_file._get_latest_chunk_size()
-        assert latest_chunk_size == self.chunk_maxsize
-
     @responses.activate
     def test_get_signed_url_return_url(self):
         responses.add(
             responses.POST,
             url=self.get_signed_url,
             status=200,
             json={
@@ -178,47 +127,49 @@
                 "url": "signed-upload-url"
             }
         )
         file = ChunkedFileUploader(
             file='file-test.mp4',
             api_key='test-key'
         )
-        result = file.get_signed_url(1)
+        result = file._get_signed_url(1)
         assert result == "signed-upload-url"
 
     @responses.activate
-    def test_upload_chunks_return_etag(self, _mock_get_file_path):
+    @mock.patch("mediacatch_s2t.uploader.ChunkedFileUploader._get_signed_url")
+    def test_upload_part_return_etag(self, mocker):
+        mocker.return_value = "http://signed-upload-url"
+
         responses.add(
             responses.PUT,
-            url="http://url-for-upoading.file",
+            "http://signed-upload-url",
             status=200,
             headers={
-                "Etag": "a-test-etag"
+                'ETag': 'etag-from-s3'
             }
         )
 
-        chunked_file = ChunkedFileUploader("file-test.mp4", "test-key")
-        filepath = chunked_file._get_file_path("1")
-        assert filepath == "temp_folder/1"
-
-        etag = chunked_file.upload_chunks(1, "http://url-for-upoading.file")
-        assert etag == "a-test-etag"
-
+        file = ChunkedFileUploader("file-test.mp4", "test-key")
+        url = file._get_signed_url(1)
+        assert url == "http://signed-upload-url"
+        file_data = b''
+        etag = file._upload_data_chunk_to_bucket(url, file_data)
+        assert etag == 'etag-from-s3'
 
-    def test_upload_file(self, _mock_endpoints, _mock_split_file_into_chunks):
+    def test_upload_file(self, _mock_endpoints):
         chunked_file = ChunkedFileUploader("file-test.mp4", "test-key")
 
         assert chunked_file._is_file_exist() is True
 
         file_duration, msg = chunked_file.get_duration()
         assert file_duration == 100000
 
         assert chunked_file.filename == "file-test"
         assert chunked_file.file_ext == ".mp4"
-        assert chunked_file.filesize == 102410000
+        assert chunked_file.filesize == 10240010000
         assert chunked_file.language == 'da'
 
         mime_file = {
             "duration": file_duration,
             "filename": chunked_file.filename,
             "file_ext": chunked_file.file_ext,
             "filesize": chunked_file.filesize,
@@ -229,24 +180,18 @@
             file_id=meta["file_id"],
             chunk_maxsize=meta["chunk_maxsize"],
             total_chunks=meta["total_chunks"],
             upload_id=meta["upload_id"]
         )
         assert chunked_file.file_id == self.file_id
         assert chunked_file.chunk_maxsize == self.chunk_maxsize
-        assert chunked_file.total_chunks == 6
+        assert chunked_file.total_chunks == 501
         assert chunked_file.upload_id == self.upload_id
 
-        chunked_file.split_file_into_chunks()
-
-        url = chunked_file.get_signed_url(1)
-        assert url == "http://url-for-upoading.file"
-
-        etag = chunked_file.upload_chunks(1, "http://url-for-upoading.file")
-        assert etag == "a-test-etag"
+        chunked_file.chop_and_upload_chunk()
 
         assert chunked_file.complete_the_upload() is True
 
         link = 'https://s2t.mediacatch.io/result?id=644f6676997bc2477563246e&api_key=test-key'
         assert chunked_file._get_transcript_link() == link
 
         result = chunked_file.upload_file()
@@ -254,52 +199,61 @@
             "url": link,
             "status": "uploaded",
             "estimated_processing_time": 10,
             "message": "The file has been uploaded."
         }
 
 
-class TestUploaderBaseMethod:
+class TestUploaderMethod:
     @pytest.fixture()
     def _mock_is_file_exist_true(self):
         with mock.patch(
-                "mediacatch_s2t.uploader.UploaderBase._is_file_exist") as mocker:
+                "mediacatch_s2t.uploader.Uploader._is_file_exist") as mocker:
             mocker.return_value = True
             yield mocker
 
-    @mock.patch("os.path.getsize", return_value=1000000000)
+    @mock.patch("os.path.getsize", return_value=10240010000)
     def test_is_multipart_upload_return_true(self, mocker, _mock_is_file_exist_true):
-        file = UploaderBase("file-test.mp4", "test-key")
+        file = Uploader("file-test.mp4", "test-key")
         assert file.is_multipart_upload() is True
 
     @mock.patch("os.path.getsize", return_value=10)
     def test_is_multipart_upload_return_false(self, mocker, _mock_is_file_exist_true):
-        file = UploaderBase("file-test.mp4", "test-key")
+        file = Uploader("file-test.mp4", "test-key")
         assert file.is_multipart_upload() is False
 
     def test_is_multipart_upload_file_not_exists(self):
-        file = UploaderBase("file-test.mp4", "test-key")
+        file = Uploader("file-test.mp4", "test-key")
         assert file.is_multipart_upload() is False
 
 
     def test_is_response_error_return_true(self):
         response = mock.Mock()
         response.status_code = 401
         response.json.return_value = {"message": "an error 401 test message"}
 
-        file = UploaderBase("file-test.mp4", "test-key")
+        file = Uploader("file-test.mp4", "test-key")
         result = file._is_response_error(response)
         assert result == (True, "an error 401 test message")
 
         response.status_code = 500
         response.json.return_value = {"message": "an error 500 test message"}
         result = file._is_response_error(response)
         assert result == (True, "an error 500 test message")
 
+    @responses.activate
     def test_make_post_request_raise_exception(self):
-        file = UploaderBase("file-test.mp4", "test-key")
-
-        with pytest.raises(Exception) as exc_info:
-            file._make_post_request()
-        assert str(exc_info.value) == "Error from uploader module: Error during post request"
+        responses.add(
+            responses.POST,
+            url="http://test-500",
+            json={"message": "test error 500"},
+            status=500
+        )
 
+        file = Uploader("file-test.mp4", "test-key")
 
+        with pytest.raises(UploaderException) as exc_info:
+            file._make_post_request(url="http://test-500")
+        assert str(exc_info.value) == (
+            "Error from uploader module: Error during post request "
+            "http://test-500; test error 500"
+        )
```

### Comparing `mediacatch-s2t-0.0.6/tests/test_uploader.py` & `mediacatch-s2t-1.0.0/tests/test_uploader.py`

 * *Files identical despite different names*

