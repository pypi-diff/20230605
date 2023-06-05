# Comparing `tmp/stewchef-0.1.4.tar.gz` & `tmp/stewchef-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stewchef-0.1.4.tar", max compression
+gzip compressed data, was "stewchef-0.1.5.tar", max compression
```

## Comparing `stewchef-0.1.4.tar` & `stewchef-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5808 2023-04-12 10:26:35.957338 stewchef-0.1.4/README.md
--rw-r--r--   0        0        0      490 2023-04-13 13:38:43.970900 stewchef-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.4/stewchef/__init__.py
--rw-r--r--   0        0        0    13128 2023-04-12 10:17:17.299510 stewchef-0.1.4/stewchef/main.py
--rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 stewchef-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5808 2023-04-12 10:26:35.957338 stewchef-0.1.5/README.md
+-rw-r--r--   0        0        0      507 2023-06-05 13:56:13.581250 stewchef-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.5/stewchef/__init__.py
+-rw-r--r--   0        0        0    13122 2023-06-05 13:55:53.342057 stewchef-0.1.5/stewchef/main.py
+-rw-r--r--   0        0        0     6583 1970-01-01 00:00:00.000000 stewchef-0.1.5/PKG-INFO
```

### Comparing `stewchef-0.1.4/README.md` & `stewchef-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `stewchef-0.1.4/stewchef/main.py` & `stewchef-0.1.5/stewchef/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import subprocess, os
 import typer
 from bs4 import BeautifulSoup
 from rich import print
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.pretty import pprint
-import tomllib
+import tomli
 import requests
 import time
 from difflib import Differ
 
 MAX_ITER = 10000
 app = typer.Typer()
 
@@ -244,15 +244,15 @@
     will be committed to the Wiki given at the API endpoint
     """
     # Statistics counters
     total_pages_edited = 0
 
     # Read config.toml
     with open(config_path, "rb") as f:
-        config = tomllib.load(f)
+        config = tomli.load(f)
 
     URL = config["server"]["url"]
 
     USER = config["bot"]["user"]
     PASSWORD = config["bot"]["password"]
 
     with Progress(SpinnerColumn(), TextColumn("[progress.description]{task.description}"), transient=True) as progress:
@@ -305,15 +305,15 @@
     Retrieve, modify and, if specified, save a single page of the Wiki
     given at the API endpoint by the Wiki page's title.
     """
     print("[bold blue]Cooking up a single serving![/bold blue]")
     # Read config.toml
     try:
         with open(config_path, "rb") as f:
-            config = tomllib.load(f)
+            config = tomli.load(f)
     except FileNotFoundError:
         print(f"[bold red]ERROR![/bold red] Config file not found.. Read the documentation for more information.")
         raise typer.Exit()
 
     URL = config["server"]["url"]
 
     USER = config["bot"]["user"]
```

### Comparing `stewchef-0.1.4/PKG-INFO` & `stewchef-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: stewchef
-Version: 0.1.4
+Version: 0.1.5
 Summary: A MediaWiki API wrapper for RegiSoup
 Author: pengu5055
 Author-email: urbancmarko1@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
 Requires-Dist: regisoup (>=0.1.10,<0.2.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # **StewChef: Cook up some RegiSoup**
 
 `StewChef` is a MediaWiki API wrapper for [`RegiSoup`](https://pypi.org/project/regisoup/). It was developed since I came to the realization that I cannot edit the contents of a Wiki's `.xml` dump manually as each `<text>` block is also given a size in bytes and a `sha1` hash. The next easiest approach was to edit pages while they are already on the Wiki and that is possible through MediaWiki's API.
```

