# Comparing `tmp/recognize-0.1.1.tar.gz` & `tmp/recognize-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognize-0.1.1.tar", max compression
+gzip compressed data, was "recognize-0.1.2.tar", max compression
```

## Comparing `recognize-0.1.1.tar` & `recognize-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.1/README.md
--rw-r--r--   0        0        0      411 2023-06-05 11:12:36.636256 recognize-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.1/recognize/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.1/recognize/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.1/recognize/commands/lib/__init__.py
--rw-r--r--   0        0        0     3112 2023-06-05 10:43:58.831563 recognize-0.1.1/recognize/commands/lib/client.py
--rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.1/recognize/commands/lib/entries.py
--rw-r--r--   0        0        0      848 2023-06-05 10:43:58.881956 recognize-0.1.1/recognize/commands/lib/helpers.py
--rw-r--r--   0        0        0     2397 2023-06-05 10:43:58.803222 recognize-0.1.1/recognize/commands/search.py
--rw-r--r--   0        0        0      854 2023-06-05 10:43:58.853929 recognize-0.1.1/recognize/commands/upload.py
--rw-r--r--   0        0        0      192 2023-06-05 10:55:55.812878 recognize-0.1.1/recognize/main.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 recognize-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.2/README.md
+-rw-r--r--   0        0        0      411 2023-06-05 12:03:56.314307 recognize-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.2/recognize/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.2/recognize/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.2/recognize/commands/lib/__init__.py
+-rw-r--r--   0        0        0     3067 2023-06-05 12:03:45.080067 recognize-0.1.2/recognize/commands/lib/client.py
+-rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.2/recognize/commands/lib/entries.py
+-rw-r--r--   0        0        0      848 2023-06-05 10:43:58.881956 recognize-0.1.2/recognize/commands/lib/helpers.py
+-rw-r--r--   0        0        0     2397 2023-06-05 10:43:58.803222 recognize-0.1.2/recognize/commands/search.py
+-rw-r--r--   0        0        0      854 2023-06-05 10:43:58.853929 recognize-0.1.2/recognize/commands/upload.py
+-rw-r--r--   0        0        0      192 2023-06-05 10:55:55.812878 recognize-0.1.2/recognize/main.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 recognize-0.1.2/PKG-INFO
```

### Comparing `recognize-0.1.1/recognize/commands/lib/client.py` & `recognize-0.1.2/recognize/commands/lib/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 from .entries import LabelEntryType
 from .helpers import upload_file
 
 
 class DataAPI:
     def __init__(self):
-        # self.url = "https://xxihhslish.execute-api.eu-west-2.amazonaws.com/prod/"
-        self.url = "http://127.0.0.1:8000"
+        self.url = "https://xxihhslish.execute-api.eu-west-2.amazonaws.com/prod/"
 
     def keyword_search(self, keywords: List[str], output_file: Path, response_type: str):
         url = urljoin(self.url, "search/")
 
         with httpx.stream("GET", url, params={
             "keywords": ",".join(keywords),
             "response_type": response_type
```

### Comparing `recognize-0.1.1/recognize/commands/lib/helpers.py` & `recognize-0.1.2/recognize/commands/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `recognize-0.1.1/recognize/commands/search.py` & `recognize-0.1.2/recognize/commands/search.py`

 * *Files identical despite different names*

### Comparing `recognize-0.1.1/recognize/commands/upload.py` & `recognize-0.1.2/recognize/commands/upload.py`

 * *Files identical despite different names*

