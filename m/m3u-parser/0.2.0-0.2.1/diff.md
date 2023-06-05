# Comparing `tmp/m3u_parser-0.2.0.tar.gz` & `tmp/m3u_parser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3u_parser-0.2.0.tar", last modified: Sat May  7 14:46:19 2022, max compression
+gzip compressed data, was "m3u_parser-0.2.1.tar", last modified: Mon Jun  5 07:30:53 2023, max compression
```

## Comparing `m3u_parser-0.2.0.tar` & `m3u_parser-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 pawan     (1000) pawan     (1000)        0 2022-05-07 14:46:19.963033 m3u_parser-0.2.0/
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)     1056 2020-11-20 14:51:56.000000 m3u_parser-0.2.0/LICENSE.txt
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)     7556 2022-05-07 14:46:19.962642 m3u_parser-0.2.0/PKG-INFO
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)     6860 2022-05-07 14:43:49.000000 m3u_parser-0.2.0/README.md
-drwxrwxrwx   0 pawan     (1000) pawan     (1000)        0 2022-05-07 14:46:19.956644 m3u_parser-0.2.0/m3u_parser/
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)       57 2022-05-07 14:43:49.000000 m3u_parser-0.2.0/m3u_parser/__init__.py
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)     5715 2021-12-29 12:29:38.000000 m3u_parser-0.2.0/m3u_parser/helper.py
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)    19351 2021-12-31 17:52:16.000000 m3u_parser-0.2.0/m3u_parser/m3u_parser.py
-drwxrwxrwx   0 pawan     (1000) pawan     (1000)        0 2022-05-07 14:46:19.961739 m3u_parser-0.2.0/m3u_parser.egg-info/
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)     7556 2022-05-07 14:46:19.000000 m3u_parser-0.2.0/m3u_parser.egg-info/PKG-INFO
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)      283 2022-05-07 14:46:19.000000 m3u_parser-0.2.0/m3u_parser.egg-info/SOURCES.txt
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)        1 2022-05-07 14:46:19.000000 m3u_parser-0.2.0/m3u_parser.egg-info/dependency_links.txt
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)       35 2022-05-07 14:46:19.000000 m3u_parser-0.2.0/m3u_parser.egg-info/requires.txt
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)       11 2022-05-07 14:46:19.000000 m3u_parser-0.2.0/m3u_parser.egg-info/top_level.txt
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)      297 2021-08-28 15:14:40.000000 m3u_parser-0.2.0/pyproject.toml
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)       38 2022-05-07 14:46:19.963239 m3u_parser-0.2.0/setup.cfg
--rwxrwxrwx   0 pawan     (1000) pawan     (1000)     3144 2022-05-07 14:43:49.000000 m3u_parser-0.2.0/setup.py
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-05 07:30:53.567622 m3u_parser-0.2.1/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     1056 2023-05-27 16:53:27.000000 m3u_parser-0.2.1/LICENSE.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     7238 2023-06-05 07:30:53.567489 m3u_parser-0.2.1/PKG-INFO
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     6562 2023-06-05 07:16:33.000000 m3u_parser-0.2.1/README.md
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-05 07:30:53.566439 m3u_parser-0.2.1/m3u_parser/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       57 2023-06-05 07:16:25.000000 m3u_parser-0.2.1/m3u_parser/__init__.py
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     6018 2023-06-05 07:14:16.000000 m3u_parser-0.2.1/m3u_parser/helper.py
+-rwxr-xr-x   0 blokchainaholic   (501) staff       (20)    19283 2023-06-05 07:23:26.000000 m3u_parser-0.2.1/m3u_parser/m3u_parser.py
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-05 07:30:53.567253 m3u_parser-0.2.1/m3u_parser.egg-info/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     7238 2023-06-05 07:30:53.000000 m3u_parser-0.2.1/m3u_parser.egg-info/PKG-INFO
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)      283 2023-06-05 07:30:53.000000 m3u_parser-0.2.1/m3u_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)        1 2023-06-05 07:30:53.000000 m3u_parser-0.2.1/m3u_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       35 2023-06-05 07:30:53.000000 m3u_parser-0.2.1/m3u_parser.egg-info/requires.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       11 2023-06-05 07:30:53.000000 m3u_parser-0.2.1/m3u_parser.egg-info/top_level.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)      297 2023-05-27 16:53:27.000000 m3u_parser-0.2.1/pyproject.toml
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       38 2023-06-05 07:30:53.567669 m3u_parser-0.2.1/setup.cfg
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     3129 2023-06-05 07:30:37.000000 m3u_parser-0.2.1/setup.py
```

### Comparing `m3u_parser-0.2.0/LICENSE.txt` & `m3u_parser-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `m3u_parser-0.2.0/m3u_parser/helper.py` & `m3u_parser-0.2.1/m3u_parser/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import csv
 import ipaddress
 import re
 from typing import Union
+import logging
 from urllib.parse import urlsplit, urlunsplit
 
 # URLValidator
 ul = '\u00a1-\uffff'  # Unicode letters range (must not be a raw string).
 
 # IP patterns
 ipv4_re = r'(?:0|25[0-5]|2[0-4]\d|1\d?\d?|[1-9]\d?)(?:\.(?:0|25[0-5]|2[0-4]\d|1\d?\d?|[1-9]\d?)){3}'
@@ -189,7 +190,17 @@
                     return False
 
         if splitted_url.hostname is None or len(splitted_url.hostname) > 253:
             return False
     except ValidationError:
         return False
     return True
+
+
+def setup_logger():
+    logger = logging.getLogger("m3u_parser")
+    handler = logging.StreamHandler()
+    formatter = logging.Formatter("%(levelname)s: %(message)s")
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+    logger.setLevel(logging.INFO)
+    return logger
```

### Comparing `m3u_parser-0.2.0/m3u_parser/m3u_parser.py` & `m3u_parser-0.2.1/m3u_parser/m3u_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #!/usr/bin/env python3
 
 import asyncio
 import json
-import logging
 import random
 import re
 import ssl
-import sys
 import time
 from typing import Union
 
 import aiohttp
 import pycountry
 import requests
 
 try:
-    from helper import get_by_regex, is_valid_url, ndict_to_csv, run_until_completed, streams_regex
+    from helper import get_by_regex, is_valid_url, ndict_to_csv, run_until_completed, streams_regex, setup_logger
 except ModuleNotFoundError:
-    from .helper import get_by_regex, is_valid_url, ndict_to_csv, run_until_completed, streams_regex
+    from .helper import get_by_regex, is_valid_url, ndict_to_csv, run_until_completed, streams_regex, setup_logger
 
 ssl.match_hostname = lambda cert, hostname: hostname == cert["subjectAltName"][0][1]
-logging.basicConfig(stream=sys.stdout, level=logging.INFO, format="%(levelname)s: %(message)s")
+
+logger = setup_logger()
 
 
 class M3uParser:
     """A parser for m3u files.
 
     It parses the contents of m3u file to a list of streams information which can be saved as a JSON/CSV file.
 
@@ -81,35 +80,35 @@
         :type check_live: bool
         :rtype: None
 
         """
         self._check_live = check_live
         self._enforce_schema = enforce_schema
         if is_valid_url(path):
-            logging.info("Started parsing m3u link...")
+            logger.info("Started parsing m3u link...")
             try:
                 self._content = requests.get(path).text
             except:
-                logging.error("Cannot read anything from the url!!!")
+                logger.error("Cannot read anything from the url!!!")
                 return
         else:
-            logging.info("Started parsing m3u file...")
+            logger.info("Started parsing m3u file...")
             try:
                 with open(path, encoding="utf-8", errors="ignore") as fp:
                     self._content = fp.read()
             except FileNotFoundError:
-                logging.error("File doesn't exist!!!")
+                logger.error("File doesn't exist!!!")
                 return
 
         # splitting contents into lines to parse them
         self._lines = [line.strip("\n\r") for line in self._content.split("\n") if line.strip("\n\r") != ""]
         if len(self._lines) > 0:
             self._parse_lines()
         else:
-            logging.error("No content to parse!!!")
+            logger.error("No content to parse!!!")
 
     @staticmethod
     async def _run_until_completed(tasks):
         for res in run_until_completed(tasks):
             _ = await res
 
     def _parse_lines(self):
@@ -125,15 +124,15 @@
         self._streams_info_backup = self._streams_info.copy()
         self._loop.run_until_complete(asyncio.sleep(0))
         while self._loop.is_running():
             time.sleep(0.3)
             if not self._loop.is_running():
                 self._loop.close()
                 break
-        logging.info("Parsing completed !!!")
+        logger.info("Parsing completed !!!")
 
     async def _parse_line(self, line_num: int):
         line_info = self._lines[line_num]
         stream_link = ""
         streams_link = []
         status = "BAD"
         try:
@@ -236,18 +235,18 @@
         :rtype: None
         """
         key_0, key_1 = [""] * 2
         if nested_key:
             try:
                 key_0, key_1 = key.split(key_splitter)
             except ValueError:
-                logging.error("Nested key must be in the format <key><key_splitter><nested_key>")
+                logger.error("Nested key must be in the format <key><key_splitter><nested_key>")
                 return
         if not filters:
-            logging.error("Filter word/s missing!!!")
+            logger.error("Filter word/s missing!!!")
             return
         if not isinstance(filters, list):
             filters = [filters]
         any_or_all = any if retrieve else all
         not_operator = lambda x: x if retrieve else not x
         try:
             self._streams_info = list(
@@ -261,15 +260,15 @@
                         )
                         for fltr in filters
                     ),
                     self._streams_info,
                 )
             )
         except AttributeError:
-            logging.error("Key given is not nested !!!")
+            logger.error("Key given is not nested !!!")
 
     def reset_operations(self):
         """Reset the stream information list to initial state before various operations.
 
         :rtype: None
         """
         self._streams_info = self._streams_info_backup.copy()
@@ -340,24 +339,24 @@
         :rtype: None
         """
         key_0, key_1 = [""] * 2
         if nested_key:
             try:
                 key_0, key_1 = key.split(key_splitter)
             except ValueError:
-                logging.error("Nested key must be in the format <key><key_splitter><nested_key>")
+                logger.error("Nested key must be in the format <key><key_splitter><nested_key>")
                 return
         try:
             self._streams_info = sorted(
                 self._streams_info,
                 key=lambda stream_info: stream_info[key_0][key_1] if nested_key else stream_info[key],
                 reverse=not asc,
             )
         except KeyError:
-            logging.error("Key not found!!!")
+            logger.error("Key not found!!!")
 
     def get_json(self, indent: int = 4):
         """Get the streams information as json.
 
         :param indent: Int value for indentation.
         :type indent: int
         :return: json of the streams_info list
@@ -382,15 +381,15 @@
 
         :param random_shuffle: To shuffle the streams information list before returning the random stream information.
         :type random_shuffle: bool
         :return: A random stream info
         :rtype: dict
         """
         if not len(self._streams_info):
-            logging.error("No streams information so could not get any random stream.")
+            logger.error("No streams information so could not get any random stream.")
             return
         if random_shuffle:
             random.shuffle(self._streams_info)
         return random.choice(self._streams_info)
 
     def _get_m3u_content(self) -> str:
         """Save the streams information list to m3u file.
@@ -440,41 +439,41 @@
             if ext in name:
                 return name
             else:
                 return name + ".%s" % ext
 
         filename = with_extension(filename, format)
         if len(self._streams_info) == 0:
-            logging.info("Either parsing is not done or no stream info was found after parsing !!!")
+            logger.info("Either parsing is not done or no stream info was found after parsing !!!")
             return
-        logging.info("Saving to file: %s" % filename)
+        logger.info("Saving to file: %s" % filename)
         if format == "json":
             data = json.dumps(self._streams_info, indent=4)
             with open(filename, mode="w", encoding="utf-8") as fp:
                 fp.write(data)
-            logging.info("Saved to file: %s" % filename)
+            logger.info("Saved to file: %s" % filename)
 
         elif format == "csv":
             if self._enforce_schema:
                 ndict_to_csv(self._streams_info, filename)
-                logging.info("Saved to file: %s" % filename)
+                logger.info("Saved to file: %s" % filename)
             else:
-                logging.info("Saving to csv file not supported if the schema was not forced (enforce_schema) !!!")
+                logger.info("Saving to csv file not supported if the schema was not forced (enforce_schema) !!!")
 
         elif format == "m3u":
             content = self._get_m3u_content()
             with open(filename, mode="w", encoding="utf-8") as fp:
                 fp.write(content)
-            logging.info("Saved to file: %s" % filename)
+            logger.info("Saved to file: %s" % filename)
         else:
-            logging.error("Unrecognised format!!!")
+            logger.error("Unrecognised format!!!")
 
 
 if __name__ == "__main__":
-    url = "/home/pawan/Downloads/ru.m3u"
+    url = "https://iptv-org.github.io/iptv/countries/np.m3u"
     useragent = (
         "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.75 Safari/537.36"
     )
     parser = M3uParser(timeout=5, useragent=useragent)
     parser.parse_m3u(url)
     parser.remove_by_extension("mp4")
     parser.filter_by("status", "GOOD")
```

### Comparing `m3u_parser-0.2.0/setup.py` & `m3u_parser-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import io
 import os
 import sys
 from shutil import rmtree
 
-from setuptools import Command, find_packages, setup
+from setuptools import Command, setup
 
 # Package meta-data.
 NAME = "m3u_parser"
 DESCRIPTION = "A useful package for parsing m3u files or links"
 URL = "https://github.com/pawanpaudel93/m3u_parser"
 EMAIL = "pawanpaudel93@gmail.com"
 AUTHOR = "Pawan Paudel"
 REQUIRES_PYTHON = ">=3.0"
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 
 REQUIRED = ["requests", "asyncio", "aiohttp", "pycountry"]
 
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

