# Comparing `tmp/sans-1.1.4.tar.gz` & `tmp/sans-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sans-1.1.4.tar", last modified: Thu May 25 07:09:21 2023, max compression
+gzip compressed data, was "sans-1.2.0.tar", last modified: Sun Jun  4 22:58:05 2023, max compression
```

## Comparing `sans-1.1.4.tar` & `sans-1.2.0.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.472500 sans-1.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.464500 sans-1.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.468500 sans-1.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-25 07:09:08.000000 sans-1.1.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 07:09:08.000000 sans-1.1.4/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-25 07:09:08.000000 sans-1.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-25 07:09:08.000000 sans-1.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-25 07:09:08.000000 sans-1.1.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-25 07:09:08.000000 sans-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-25 07:09:21.472500 sans-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-25 07:09:08.000000 sans-1.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.468500 sans-1.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 07:09:08.000000 sans-1.1.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 07:09:08.000000 sans-1.1.4/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-25 07:09:08.000000 sans-1.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 07:09:08.000000 sans-1.1.4/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 07:09:08.000000 sans-1.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-25 07:09:08.000000 sans-1.1.4/docs/limiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 07:09:08.000000 sans-1.1.4/docs/lock.rst
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-25 07:09:08.000000 sans-1.1.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 07:09:08.000000 sans-1.1.4/docs/response.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-25 07:09:08.000000 sans-1.1.4/docs/url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-25 07:09:08.000000 sans-1.1.4/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-25 07:09:08.000000 sans-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 07:09:08.000000 sans-1.1.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.468500 sans-1.1.4/sans/
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-25 07:09:08.000000 sans-1.1.4/sans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-25 07:09:08.000000 sans-1.1.4/sans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 07:09:08.000000 sans-1.1.4/sans/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-25 07:09:08.000000 sans-1.1.4/sans/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-25 07:09:08.000000 sans-1.1.4/sans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-05-25 07:09:08.000000 sans-1.1.4/sans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-25 07:09:08.000000 sans-1.1.4/sans/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-25 07:09:08.000000 sans-1.1.4/sans/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-25 07:09:08.000000 sans-1.1.4/sans/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-25 07:09:08.000000 sans-1.1.4/sans/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:08.000000 sans-1.1.4/sans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-25 07:09:08.000000 sans-1.1.4/sans/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-25 07:09:08.000000 sans-1.1.4/sans/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-25 07:09:08.000000 sans-1.1.4/sans/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:09:21.472500 sans-1.1.4/sans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 07:09:21.000000 sans-1.1.4/sans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:09:21.472500 sans-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-25 07:09:08.000000 sans-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.938731 sans-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.922731 sans-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.926731 sans-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-04 22:57:54.000000 sans-1.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-04 22:57:54.000000 sans-1.2.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-04 22:57:54.000000 sans-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-04 22:57:54.000000 sans-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-04 22:57:54.000000 sans-1.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-04 22:57:54.000000 sans-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-04 22:58:05.934731 sans-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-04 22:57:54.000000 sans-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.934731 sans-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-04 22:57:54.000000 sans-1.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 22:57:54.000000 sans-1.2.0/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-04 22:57:54.000000 sans-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-04 22:57:54.000000 sans-1.2.0/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-04 22:57:54.000000 sans-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-04 22:57:54.000000 sans-1.2.0/docs/limiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-04 22:57:54.000000 sans-1.2.0/docs/lock.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-04 22:57:54.000000 sans-1.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-04 22:57:54.000000 sans-1.2.0/docs/response.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-04 22:57:54.000000 sans-1.2.0/docs/url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 22:57:54.000000 sans-1.2.0/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-04 22:57:54.000000 sans-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-04 22:57:54.000000 sans-1.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.934731 sans-1.2.0/sans/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-04 22:57:54.000000 sans-1.2.0/sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-04 22:57:54.000000 sans-1.2.0/sans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-04 22:57:54.000000 sans-1.2.0/sans/_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-04 22:57:54.000000 sans-1.2.0/sans/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-04 22:57:54.000000 sans-1.2.0/sans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27979 2023-06-04 22:57:54.000000 sans-1.2.0/sans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-04 22:57:54.000000 sans-1.2.0/sans/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-04 22:57:54.000000 sans-1.2.0/sans/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14295 2023-06-04 22:57:54.000000 sans-1.2.0/sans/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 22:57:54.000000 sans-1.2.0/sans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-04 22:57:54.000000 sans-1.2.0/sans/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-04 22:57:54.000000 sans-1.2.0/sans/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-04 22:57:54.000000 sans-1.2.0/sans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.934731 sans-1.2.0/sans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 22:58:05.938731 sans-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-04 22:57:54.000000 sans-1.2.0/setup.py
```

### Comparing `sans-1.1.4/.github/workflows/codeql-analysis.yml` & `sans-1.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sans-1.1.4/.github/workflows/pythonpublish.yml` & `sans-1.2.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `sans-1.1.4/.gitignore` & `sans-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sans-1.1.4/.pre-commit-config.yaml` & `sans-1.2.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-toml
     -   id: check-added-large-files
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.269
+    rev: v0.0.270
     hooks:
     -   id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
 -   repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.309
+    rev: v1.1.311
     hooks:
     -   id: pyright
         additional_dependencies:
             # required dependencies
         -   httpx ~= 0.23
         -   importlib_metadata >= 1.4.0; python_version < "3.8"
 
@@ -33,11 +33,12 @@
 
             # [json]
         -   xmltodict ~= 0.13
 
             # typing
         -   typing_extensions
         -   lxml-stubs @ https://github.com/lxml/lxml-stubs/archive/master.zip#egg=lxml-stubs
+        -   anyio[trio]
 ci:
     skip:
     # CI doesn't like pip scripts calling their own node, so skip this for now
     -   pyright
```

### Comparing `sans-1.1.4/LICENSE` & `sans-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sans-1.1.4/PKG-INFO` & `sans-1.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.1.4
+Version: 1.2.0
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,140 +42,150 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: <4.0,>=3.7.0
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: lxml
 Provides-Extra: json
 License-File: LICENSE
 
-sans
-====
+# sans
 
-|pypi| |Code style: black| |Build Status| |Documentation Status|
+[![pypi](https://img.shields.io/pypi/v/sans.svg) ![Licensed under the MIT License](https://img.shields.io/pypi/l/sans.svg)](https://pypi.org/project/sans/)
+[![Downloads](https://static.pepy.tech/badge/sans)](https://pepy.tech/project/sans)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Zephyrkul/sans/master.svg)](https://results.pre-commit.ci/latest/github/Zephyrkul/sans/master)
+[![Documentation Status](https://readthedocs.org/projects/sans/badge/?version=latest)](http://sans.readthedocs.org/en/latest/?badge=latest)
 
-**S**\ ynchronous / **A**\ synchronous **N**\ ation\ **S**\ tates
+**S**ynchronous / **A**synchronous **N**ation**S**tates
 
-A `fully typed <https://docs.python.org/3/library/typing.html>`_ extension for `HTTPX <https://www.python-httpx.org/>`_ for the `NationStates API <https://www.nationstates.net/pages/api.html>`_.
+A [fully typed](https://docs.python.org/3/library/typing.html>) extension for [HTTPX](https://www.python-httpx.org/) for the [NationStates API](https://www.nationstates.net/pages/api.html).
 
-Installing
-----------
+## Installing
 
-.. code::
-
-   python3 -m pip install -U sans
+```sh
+python3 -m pip install -U sans
+```
 
 Development version:
 
-.. code::
-
-   python3 -m pip install -U https://github.com/zephyrkul/sans/archive/master.zip#egg=sans
-
-Examples
---------
-
-Synchronous
-~~~~~~~~~~~
-
-.. code:: python
-
-   import sans
-   from xml.etree import ElementTree as ET
-
-   def main():
-      sans.set_agent("Darcania")
+```sh
+python3 -m pip install -U https://github.com/zephyrkul/sans/archive/master.zip#egg=sans
+```
+
+## Examples
+
+### Synchronous
+
+```py
+import sans
+from xml.etree import ElementTree as ET
+
+def main():
+   sans.set_agent("Darcania")
+   request = sans.Nation(
+      "darcania",
+      "fullname population flag census",
+      mode="score",
+      scale="65 66",
+   )
+   root = sans.get(request).xml
+   sans.indent(root)
+   print(ET.tostring(root, encoding="unicode"))
+
+   with sans.stream("GET", sans.RegionsDump()) as response:
+      for region in response.iter_xml():
+         sans.indent(region)
+         print(ET.tostring(region, encoding="unicode"))
+
+if __name__ == "__main__":
+   main()
+```
+
+### Asynchronous
+
+```py
+import asyncio
+import sans
+from xml.etree import ElementTree as ET
+
+async def main():
+   sans.set_agent("Darcania")
+   async with sans.AsyncClient() as client:
       request = sans.Nation(
          "darcania",
          "fullname population flag census",
          mode="score",
          scale="65 66",
       )
-      root = sans.get(request).xml
+      root = (await client.send(request)).xml
       sans.indent(root)
       print(ET.tostring(root, encoding="unicode"))
 
-      with sans.stream("GET", sans.RegionsDump()) as response:
-         for region in response.iter_xml():
+      async with client.stream("GET", sans.RegionsDump()) as response:
+         async for region in response.aiter_xml():
             sans.indent(region)
             print(ET.tostring(region, encoding="unicode"))
 
-   if __name__ == "__main__":
-      main()
-
-Asynchronous
-~~~~~~~~~~~~
-
-.. code:: python
-
-   import asyncio
-   import sans
-   from xml.etree import ElementTree as ET
-
-   async def main():
-      sans.set_agent("Darcania")
-      async with sans.AsyncClient() as client:
-         request = sans.Nation(
-            "darcania",
-            "fullname population flag census",
-            mode="score",
-            scale="65 66",
-         )
-         root = (await client.send(request)).xml
-         sans.indent(root)
-         print(ET.tostring(root, encoding="unicode"))
-
-         async with client.stream("GET", sans.RegionsDump()) as response:
-            async for region in response.aiter_xml():
-               sans.indent(region)
-               print(ET.tostring(region, encoding="unicode"))
-
-   if __name__ == "__main__":
-      asyncio.run(main())
-
-Command Line
-------------
-
-.. code::
-
-   $ sans --nation darcania census --scale "65 66" --mode score --agent Darcania
-
+if __name__ == "__main__":
+   asyncio.run(main())
+```
+
+### Authentication
+
+```py
+auth = sans.NSAuth(password="hunter2")
+sans.get(sans.Nation("testlandia", "ping"), auth=auth)
+# X-Autologin is automatically retrieved and stored for when the auth object is re-used
+print(auth.autologin)
+# X-Pin is cached internally for repeated requests
+root = sans.get(sans.Nation("testlandia", "packs"), auth=auth).xml
+```
+
+### Telegrams
+
+```py
+limiter = sans.TelegramLimiter(recruitment=False)
+# The Telegram API can be used without a TelegramLimiter, but marking it ahead of time can save an API call.
+response = sans.get(sans.Telegram(client="abcd1234", tgid="1234", key="abcdef1234567890", to="testlandia"), auth=limiter)
+assert response.content = b"queued"
+```
+
+## Command Line
+
+```xml
+sans --nation darcania census --scale "65 66" --mode score --agent Darcania
+<NATION id="darcania">
    <CENSUS>
       <SCALE id="65">
-         <SCORE>4949.00</SCORE>
+         <SCORE>8145.00</SCORE>
       </SCALE>
       <SCALE id="66">
-         <SCORE>130.00</SCORE>
+         <SCORE>0.00</SCORE>
       </SCALE>
    </CENSUS>
+</NATION>
 
-   $ sans --nation testlandia fullname
-
+sans --nation testlandia fullname
+<NATION id="testlandia">
    <FULLNAME>The Hive Mind of Testlandia</FULLNAME>
+</NATION>
 
-   sans --region "the north pacific" numnations lastupdate
-
-   <LASTUPDATE>1683650325</LASTUPDATE>
-   <NUMNATIONS>10503</NUMNATIONS>
+sans --region "the north pacific" numnations lastupdate
+<REGION id="the_north_pacific">
+   <LASTUPDATE>1685681810</LASTUPDATE>
+   <NUMNATIONS>9535</NUMNATIONS>
+</REGION>
+
+sans --quit
+No query provided. Exiting...
+```
 
-   $ sans --quit
-   No query provided. Exiting...
+## Requirements
 
-Requirements
-------------
-
--  Python 3.7+
--  httpx
-
-.. |pypi| image:: https://img.shields.io/pypi/v/sans.svg
-   :target: https://pypi.python.org/pypi/sans
-   :alt: pypi version
-.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/ambv/black
-.. |Build Status| image:: https://results.pre-commit.ci/badge/github/Zephyrkul/sans/master.svg
-   :target: https://results.pre-commit.ci/latest/github/Zephyrkul/sans/master
-   :alt: pre-commit.ci status
-.. |Documentation Status| image:: https://readthedocs.org/projects/sans/badge/?version=latest
-   :target: http://sans.readthedocs.org/en/latest/?badge=latest
+- [Python 3.7+](https://www.python.org/)
+- [httpx](https://pypi.org/project/httpx/)
```

### Comparing `sans-1.1.4/docs/Makefile` & `sans-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sans-1.1.4/docs/conf.py` & `sans-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.4/docs/make.bat` & `sans-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sans-1.1.4/pyproject.toml` & `sans-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         'wheel',
     ]
     build-backend = 'setuptools.build_meta'
 
 [project]
     name = 'sans'
     description = 'Synchronous / Asynchronous HTTPX extension for NationStates'
-    readme = 'README.rst'
+    readme = 'README.md'
     requires-python = '>=3.7.0,<4.0'
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Framework :: AsyncIO',
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Developers',
         'Natural Language :: English',
```

### Comparing `sans-1.1.4/sans/__init__.py` & `sans-1.2.0/sans/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,20 +24,18 @@
 
 import sys as _sys
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing_extensions import Literal
 
-from . import _state
 from .auth import *
 from .client import *
 from .errors import *
-from .limiter import *
-from .lock import *
+from .limiter import RateLimiter as RateLimiter, TelegramLimiter as TelegramLimiter
 from .response import *
 from .url import *
 from .utils import *
 
 if _sys.version_info < (3, 8):
     from importlib_metadata import metadata as _metadata
 else:
@@ -70,18 +68,27 @@
         Not recommended: https://www.nationstates.net/pages/api.html#terms
 
     Returns
     -------
     The actual newly set agent, including attached additional script information.
     """
 
-    if _state.agent and not _force:
+    if RateLimiter._agent and not _force:
         raise RuntimeError("Agent cannot be re-set")
-    import sys
-
-    import httpx
-
-    _state.agent = (
-        f"{new_agent} Python/{sys.version_info[0]}.{sys.version_info[1]} "
-        f"httpx/{httpx.__version__} sans/{__version__}"
-    )
-    return _state.agent
+    if not new_agent:
+        RateLimiter._agent = ""
+    else:
+        import sys
+
+        import httpx
+
+        RateLimiter._agent = (
+            f"{new_agent} Python/{sys.version_info[0]}.{sys.version_info[1]} "
+            f"httpx/{httpx.__version__} sans/{__version__}"
+        )
+    return RateLimiter._agent
+
+
+for obj in list(globals().values()):
+    if getattr(obj, "__module__", "").startswith(__name__):
+        obj.__module__ = __name__
+del obj  # type: ignore
```

### Comparing `sans-1.1.4/sans/auth.py` & `sans-1.2.0/sans/auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
-from httpx import Request, Response
+from typing import overload
+
+import httpx
 
 from .limiter import RateLimiter
 from .url import API_URL
 
 try:
     # guard against reloading
     _PINS  # type: ignore  # noqa: B018
@@ -12,15 +14,25 @@
     _PINS: dict[str, str] = {}
 
 
 __all__ = ["NSAuth"]
 
 
 class NSAuth(RateLimiter):
-    def __init__(self, *, password: str | None = None, autologin: str | None = None):
+    @overload
+    def __init__(self, *, password: str) -> None:
+        ...
+
+    @overload
+    def __init__(self, *, autologin: str) -> None:
+        ...
+
+    def __init__(
+        self, *, password: str | None = None, autologin: str | None = None
+    ) -> None:
         self._password = password
         self.autologin = autologin
 
     @property
     def password(self) -> str | None:
         return self._password
 
@@ -36,31 +48,40 @@
 
     @autologin.setter
     def autologin(self, value: str | None) -> None:
         if value:
             self._password = None  # no longer needed
         self._autologin = value
 
-    def _request_hook(self, request: Request) -> Request:
+    def _request_hook(self, request: httpx.Request) -> httpx.Request:
         params = request.url.params
         nation = params.get("nation")
         if not nation:
             return request
         headers = request.headers
         if self._autologin:
             headers["X-Autologin"] = self._autologin
             pin = _PINS.get(self._autologin)
             if pin:
                 headers["X-Pin"] = pin
         elif self._password:
             headers["X-Password"] = self._password
-        request = Request("POST", API_URL, headers=headers, data=params)
+        try:
+            is_empty = not request.content
+        except httpx.RequestNotRead:
+            pass  # don't override content
+        else:
+            if is_empty and ("c" in params or request.method == "POST"):
+                # coerce a POST request
+                headers.pop("Content-Type", None)
+                headers.pop("Content-Length", None)
+                request = httpx.Request("POST", API_URL, headers=headers, data=params)
         return super()._request_hook(request)
 
-    def _response_hook(self, response: Response) -> None:
-        autologin = response.headers.get("X-Autologin")
+    def _response_hook(self, response: httpx.Response) -> None:
+        autologin: str | None = response.headers.get("X-Autologin")
         if autologin:
             self.autologin = autologin
             pin = response.headers.get("X-Pin")
             if pin:
                 _PINS[autologin] = pin
         return super()._response_hook(response)
```

### Comparing `sans-1.1.4/sans/client.py` & `sans-1.2.0/sans/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from functools import wraps
-from typing import TYPE_CHECKING, Callable, NewType, TypeVar
+from operator import methodcaller
+from typing import TYPE_CHECKING, Callable, TypeVar
 
 if TYPE_CHECKING:
     from typing_extensions import ParamSpec
 
     _P = ParamSpec("_P")
     _R = TypeVar("_R")
 
@@ -24,31 +25,45 @@
     "options",
     "patch",
     "post",
     "put",
     "request",
     "stream",
 ]
-ClientType = NewType("ClientType", httpx.Client)
-AsyncClientType = NewType("AsyncClientType", httpx.AsyncClient)
 _limiter = RateLimiter()
 
 
-def _ensure_auth(wrapped: Callable[_P, _R]) -> Callable[_P, _R]:
+def _ensure_auth(
+    wrapped: Callable[_P, _R], *, force_auth: bool = False
+) -> Callable[_P, _R]:
+    setter = methodcaller(
+        "__setitem__" if force_auth else "setdefault", "auth", _limiter
+    )
+
     @wraps(wrapped)
     def inner(*args: _P.args, **kwargs: _P.kwargs) -> _R:
-        if "auth" not in kwargs:
-            kwargs["auth"] = _limiter
+        setter(kwargs)
         return wrapped(*args, **kwargs)
 
     return inner
 
 
-Client = _ensure_auth(httpx.Client)
-AsyncClient = _ensure_auth(httpx.AsyncClient)
+class Client(httpx.Client):
+    __doc__ = httpx.Client.__doc__
+    __init__ = _ensure_auth(httpx.Client.__init__, force_auth=True)
+
+
+class AsyncClient(httpx.AsyncClient):
+    __doc__ = httpx.AsyncClient.__doc__
+    __init__ = _ensure_auth(httpx.AsyncClient.__init__, force_auth=True)
+
+
+# backwards compatibility
+ClientType = Client
+AsyncClientType = AsyncClient
 
 request = _ensure_auth(httpx.request)
 delete = _ensure_auth(httpx.delete)
 get = _ensure_auth(httpx.get)
 head = _ensure_auth(httpx.head)
 options = _ensure_auth(httpx.options)
 patch = _ensure_auth(httpx.patch)
```

### Comparing `sans-1.1.4/sans/client.pyi` & `sans-1.2.0/sans/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import (
     Any,
     AsyncContextManager,
     Callable,
     Collection,
     ContextManager,
     Mapping,
-    NewType,
     overload,
 )
 from typing_extensions import TypedDict
 
 import httpx
 from httpx._types import (
     AuthTypes,
@@ -61,15 +60,37 @@
     @auth.setter
     def auth(self, auth: RateLimiter) -> None: ...
     @property
     def event_hooks(self) -> _EventHooks: ...
     @event_hooks.setter
     def event_hooks(self, value: _EventHooksParam) -> None: ...
 
-class _ClientType(_ClientMixin, httpx.Client):
+class Client(_ClientMixin, httpx.Client):
+    def __init__(
+        self,
+        *,
+        params: QueryParamTypes = ...,
+        headers: HeaderTypes = ...,
+        cookies: CookieTypes = ...,
+        verify: VerifyTypes = ...,
+        cert: CertTypes = ...,
+        http1: bool = ...,
+        http2: bool = ...,
+        proxies: ProxiesTypes = ...,
+        mounts: Mapping[str, httpx.BaseTransport] = ...,
+        timeout: TimeoutTypes = ...,
+        follow_redirects: bool = ...,
+        limits: httpx.Limits = ...,
+        max_redirects: int = ...,
+        event_hooks: _EventHooksParam = ...,
+        base_url: URLTypes = ...,
+        transport: httpx.BaseTransport = ...,
+        app: Callable[..., Any] = ...,
+        trust_env: bool = ...,
+    ) -> None: ...
     @overload
     def request(
         self,
         method: str,
         url: URLTypes,
         *,
         content: RequestContent = ...,
@@ -359,15 +380,37 @@
         cookies: CookieTypes = ...,
         auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> ContextManager[httpx.Response]: ...
 
-class _AsyncClientType(_ClientMixin, httpx.AsyncClient):
+class AsyncClient(_ClientMixin, httpx.AsyncClient):
+    def __init__(
+        self,
+        *,
+        params: QueryParamTypes = ...,
+        headers: HeaderTypes = ...,
+        cookies: CookieTypes = ...,
+        verify: VerifyTypes = ...,
+        cert: CertTypes = ...,
+        http1: bool = ...,
+        http2: bool = ...,
+        proxies: ProxiesTypes = ...,
+        mounts: Mapping[str, httpx.BaseTransport] = ...,
+        timeout: TimeoutTypes = ...,
+        follow_redirects: bool = ...,
+        limits: httpx.Limits = ...,
+        max_redirects: int = ...,
+        event_hooks: Mapping[str, Collection[Callable[..., Any]]] = ...,
+        base_url: URLTypes = ...,
+        transport: httpx.BaseTransport = ...,
+        app: Callable[..., Any] = ...,
+        trust_env: bool = ...,
+    ) -> None: ...
     @overload
     async def request(
         self,
         method: str,
         url: URLTypes,
         *,
         content: RequestContent = ...,
@@ -657,110 +700,18 @@
         cookies: CookieTypes = ...,
         auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> AsyncContextManager[httpx.Response]: ...
 
-ClientType = NewType("ClientType", _ClientType)
-AsyncClientType = NewType("AsyncClientType", _AsyncClientType)
+ClientType = Client
+AsyncClientType = AsyncClient
 
 @overload
-def Client(
-    *,
-    auth: RateLimiter = ...,
-    params: QueryParamTypes = ...,
-    headers: HeaderTypes = ...,
-    cookies: CookieTypes = ...,
-    verify: VerifyTypes = ...,
-    cert: CertTypes = ...,
-    http1: bool = ...,
-    http2: bool = ...,
-    proxies: ProxiesTypes = ...,
-    mounts: Mapping[str, httpx.BaseTransport] = ...,
-    timeout: TimeoutTypes = ...,
-    follow_redirects: bool = ...,
-    limits: httpx.Limits = ...,
-    max_redirects: int = ...,
-    event_hooks: _EventHooksParam = ...,
-    base_url: URLTypes = ...,
-    transport: httpx.BaseTransport = ...,
-    app: Callable[..., Any] = ...,
-    trust_env: bool = ...,
-) -> ClientType: ...
-@overload
-def Client(
-    *,
-    auth: AuthTypes | None,
-    params: QueryParamTypes = ...,
-    headers: HeaderTypes = ...,
-    cookies: CookieTypes = ...,
-    verify: VerifyTypes = ...,
-    cert: CertTypes = ...,
-    http1: bool = ...,
-    http2: bool = ...,
-    proxies: ProxiesTypes = ...,
-    mounts: Mapping[str, httpx.BaseTransport] = ...,
-    timeout: TimeoutTypes = ...,
-    follow_redirects: bool = ...,
-    limits: httpx.Limits = ...,
-    max_redirects: int = ...,
-    event_hooks: Mapping[str, list[Callable[..., Any]]] = ...,
-    base_url: URLTypes = ...,
-    transport: httpx.BaseTransport = ...,
-    app: Callable[..., Any] = ...,
-    trust_env: bool = ...,
-) -> httpx.Client: ...
-@overload
-def AsyncClient(
-    *,
-    auth: RateLimiter = ...,
-    params: QueryParamTypes = ...,
-    headers: HeaderTypes = ...,
-    cookies: CookieTypes = ...,
-    verify: VerifyTypes = ...,
-    cert: CertTypes = ...,
-    http1: bool = ...,
-    http2: bool = ...,
-    proxies: ProxiesTypes = ...,
-    mounts: Mapping[str, httpx.BaseTransport] = ...,
-    timeout: TimeoutTypes = ...,
-    follow_redirects: bool = ...,
-    limits: httpx.Limits = ...,
-    max_redirects: int = ...,
-    event_hooks: Mapping[str, Collection[Callable[..., Any]]] = ...,
-    base_url: URLTypes = ...,
-    transport: httpx.BaseTransport = ...,
-    app: Callable[..., Any] = ...,
-    trust_env: bool = ...,
-) -> AsyncClientType: ...
-@overload
-def AsyncClient(
-    *,
-    auth: AuthTypes | None,
-    params: QueryParamTypes = ...,
-    headers: HeaderTypes = ...,
-    cookies: CookieTypes = ...,
-    verify: VerifyTypes = ...,
-    cert: CertTypes = ...,
-    http1: bool = ...,
-    http2: bool = ...,
-    proxies: ProxiesTypes = ...,
-    mounts: Mapping[str, httpx.BaseTransport] = ...,
-    timeout: TimeoutTypes = ...,
-    follow_redirects: bool = ...,
-    limits: httpx.Limits = ...,
-    max_redirects: int = ...,
-    event_hooks: _EventHooksParam = ...,
-    base_url: URLTypes = ...,
-    transport: httpx.BaseTransport = ...,
-    app: Callable[..., Any] = ...,
-    trust_env: bool = ...,
-) -> httpx.AsyncClient: ...
-@overload
 def request(
     method: str,
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
     data: RequestData = ...,
```

### Comparing `sans-1.1.4/sans/decoder.py` & `sans-1.2.0/sans/decoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from __future__ import annotations
 
 import codecs
 import zlib
 from functools import reduce
-from operator import itemgetter
-from typing import TYPE_CHECKING, Iterable
+from typing import Iterable
 from xml.etree.ElementTree import Element, XMLParser, XMLPullParser
 
-if TYPE_CHECKING:
-    from typing_extensions import Literal
-
 
 def _reducer(final: bool):
     def inner(data: bytes, decoder: codecs.IncrementalDecoder) -> bytes:
         return decoder.decode(data, final)  # type: ignore
 
     return inner
 
@@ -49,32 +45,32 @@
             )
         self._pull_parser = XMLPullParser(["start", "end"])
         self._path: list[Element] = []
 
     def decode(self, data: bytes) -> Iterable[Element]:
         data = reduce(_reducer(False), self._decoder_chain, data)
         self._pull_parser.feed(data)
-        return map(itemgetter(1), self._read_events())
+        return self._read_events()
 
     def flush(self) -> Iterable[Element]:
         data = reduce(_reducer(True), self._decoder_chain, b"")
         self._pull_parser.feed(data)
         self._pull_parser.close()
-        return map(itemgetter(1), self._read_events())
+        return self._read_events()
 
-    def _read_events(self) -> Iterable[tuple[Literal["end"], Element]]:
+    def _read_events(self) -> Iterable[Element]:
         element: Element
         path = self._path
         for event, element in self._pull_parser.read_events():
             if event == "start":
                 path.append(element)
             elif event == "end":
                 path.pop()
                 if len(path) == 1:
-                    yield event, element
+                    yield element
                     path[0].clear()
 
 
 try:
     from lxml.etree import (
         XMLParser as LXMLParser,
         _Element as LElement,
```

### Comparing `sans-1.1.4/sans/errors.py` & `sans-1.2.0/sans/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     _, best = match
     if best is type(original):
         return original
     # bypass __init__
     _new = best.__new__(best)
     _new.__dict__.update(original.__dict__)
     _new.args = original.args
-    return _new.with_traceback(original.__traceback__)
+    return _new
 
 
 class ClientError(_HTTPStatusError):
     """
     :exc:`httpx.HTTPStatusError` for 4XX: Client Error status codes.
     """
```

### Comparing `sans-1.1.4/sans/lock.py` & `sans-1.2.0/sans/_lock.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,172 +1,250 @@
 from __future__ import annotations
 
 import asyncio
 import threading
+import time
+import weakref
 from collections import deque
 from contextvars import Context, copy_context
 from functools import partial
 from operator import add
-from time import monotonic
-from typing import TYPE_CHECKING, Any, Callable, Mapping, TypeVar
+from typing import TYPE_CHECKING, Any, Awaitable, Callable
+
+import anyio
+import sniffio
+from anyio.lowlevel import cancel_shielded_checkpoint, checkpoint_if_cancelled
 
 if TYPE_CHECKING:
-    from typing_extensions import Literal
+    from typing_extensions import TypeVarTuple, Unpack
+
+    _Ts = TypeVarTuple("_Ts")
 
 __all__ = ["ResetLock"]
 
 
-_KT = TypeVar("_KT")
+def _threading_sleep_forever(callback_deque: deque[Callable[[], Any]]):
+    lock = threading.Lock()
+    with lock:
+        callback_deque.append(lock.release)
+        try:
+            lock.acquire()
+        finally:
+            callback_deque.remove(lock.release)
 
 
-def _get_as_int(mapping: Mapping[_KT, Any], key: _KT, default: int) -> int:
+async def _asyncio_sleep_forever(callback_deque: deque[Callable[[], Any]]) -> None:
+    future = asyncio.get_running_loop().create_future()
+    release = partial(future.get_loop().call_soon_threadsafe, future.set_result, None)
+    callback_deque.append(release)
     try:
-        return int(mapping[key])
-    except (KeyError, ValueError):
-        return default
+        await future
+    finally:
+        callback_deque.remove(release)
+
+
+try:
+    import trio
+except ImportError:
+    pass
+else:
+
+    @trio.lowlevel.enable_ki_protection
+    async def _trio_sleep_forever(
+        callback_deque: deque[Callable[[], Any]]
+    ) -> Awaitable[None]:
+        task = trio.lowlevel.current_task()
+        release = partial(
+            trio.lowlevel.current_trio_token().run_sync_soon,
+            trio.lowlevel.reschedule,
+            task,
+        )
+        callback_deque.append(release)
 
+        try:
+            return await trio.lowlevel.wait_task_rescheduled(
+                lambda _: trio.lowlevel.Abort.SUCCEEDED
+            )
+        finally:
+            callback_deque.remove(release)
+
+
+class _ThreadTimer(threading.Timer):
+    def __init__(
+        self,
+        delay: float,
+        callback: Callable[[Unpack[_Ts]], Any],
+        *args: Unpack[_Ts],
+        context: Context | None = None,
+    ) -> None:
+        if not context:
+            context = copy_context()
+        super().__init__(delay, context.run, (callback, *args))
 
-class _Timer(threading.Timer):
     def when(self) -> float:
         # when the timer completes if started at this very moment
-        return monotonic() + self.interval
+        return self.interval + time.monotonic()
 
     def run(self) -> None:
         # freeze .when() at the current time
-        self.when = partial(add, monotonic(), self.interval)
-        return super().run()
+        self.when = partial(add, self.interval, time.monotonic())
+        try:
+            return super().run()
+        finally:
+            self.when = time.monotonic
+            del self.function, self.args, self.kwargs
 
 
 # I would love to make this utilize a semaphore instead
 # However, since multiple clients can exist on one machine,
 # locking and checking the headers sequentially is a requirement
 class ResetLock:
     """
-    Combination :class:`asyncio.Lock` and :class:`threading.Lock`
-    for ratelimiting purposes.
+    Combination :class:`asyncio.Lock`, :class:`trio.Lock`, and :class:`threading.Lock`
+    for ratelimiting purposes. Works based on a FIFO queue.
 
     Usage::
 
         lock = ResetLock()
         [async] with lock.maybe_lock(url):
             response = ...
             lock.maybe_defer(response.headers)
 
     Note that, when using :mod:`httpx`,
     using :class:`RateLimiter` will manage a global lock for you.
     """
 
+    __deferred: _ThreadTimer | None = None
+
+    def __finalizer(self) -> None:
+        pass
+
     def __init__(self):
-        self.__deferred: asyncio.TimerHandle | _Timer | None = None
         self._lock = threading.Lock()
-        self._waiters: deque[asyncio.Future[Literal[True]]] = deque()
+        self._waiters: deque[Callable[[], Any]] = deque()
 
     def _wake_up_next(self):
         try:
-            next_fut = next(iter(self._waiters))
+            release = next(iter(self._waiters))
         except StopIteration:
             return
-        if next_fut.done():
-            return
-        try:
-            loop = asyncio.get_running_loop()
-        except RuntimeError:
-            loop = None
-        next_loop = next_fut.get_loop()
-        if next_loop == loop:
-            next_fut.set_result(True)
         else:
-            next_loop.call_soon_threadsafe(next_fut.set_result, True)
+            release()
 
     async def __aenter__(self) -> None:
         acquire = self._lock.acquire
-        future_factory = asyncio.get_running_loop().create_future
-        waiters_append = self._waiters.append
-        waiters_remove = self._waiters.remove
-        while not acquire(False):
-            fut = future_factory()
-            waiters_append(fut)
-            try:
-                try:
-                    await fut
-                finally:
-                    waiters_remove(fut)
-            except asyncio.CancelledError:
+        waiters = self._waiters
+        sleep_forever: Callable[
+            [deque[Callable[[], Any]]], Awaitable[None]
+        ] = globals()[f"_{sniffio.current_async_library()}_sleep_forever"]
+        await checkpoint_if_cancelled()
+        if not waiters:
+            if acquire(False):
+                await cancel_shielded_checkpoint()
+                return
+        try:
+            await sleep_forever(waiters)
+        except anyio.get_cancelled_exc_class():
+            if not self._lock.locked():
                 self._wake_up_next()
-                raise
+            raise
+        else:
+            # We were just rescheduled, so the lock is about to be released
+            acquire()
 
     async def __aexit__(self, *_):
         self.release()
 
     def __enter__(self) -> bool:
-        return self._lock.acquire()
+        acquire = self._lock.acquire
+        waiters = self._waiters
+        if not waiters:
+            if acquire(False):
+                return True
+        _threading_sleep_forever(waiters)
+        return acquire()
 
     def __exit__(self, *_):
         self.release()
 
     @property
     def deferred(self) -> float | None:
         """
-        Returns when the lock is scheduled to be released according to internal monotonic clocks,
+        Returns when the lock is scheduled to be released in seconds from now,
         or None if the lock isn't deferred.
+
+        Note that this is only the *schedule* - the value could be
+        0.0 or even negative if the deferring thread falls behind.
         """
         if self.__deferred:
-            return self.__deferred.when()
+            return time.monotonic() - self.__deferred.when()
         # return None
 
-    # write-only property
-    @partial(property, None)
-    def _deferred(self, value: asyncio.TimerHandle | _Timer | None):
+    _deferred = property(deferred.fget)
+
+    @_deferred.setter
+    def _deferred(self, value: _ThreadTimer):
         assert self.locked()
-        if self.__deferred:
-            self.__deferred.cancel()
+        self.__finalizer()
+        value.start()
         self.__deferred = value
+        self.__finalizer = weakref.finalize(self, value.finished.set)
 
     @_deferred.deleter
     def _deferred(self) -> None:
         assert self.locked()
-        if self.__deferred:
-            self.__deferred.cancel()
-        self.__deferred = None
+        self.__finalizer()
+        del self.__deferred
 
-    def maybe_defer(self, response_headers: Mapping[str, str]) -> None:
+    def defer(self, delay: float) -> None:
         if not self.locked():
             return
-        try:
-            call_later = asyncio.get_running_loop().call_later  # type: ignore
-        except RuntimeError:
-
-            def call_later(
-                delay: float,
-                callback: Callable[..., Any],
-                *args: Any,
-                context: Context | None = None,
-            ) -> _Timer | asyncio.TimerHandle:
-                if not context:
-                    context = copy_context()
-                timer = _Timer(delay, context.run, (callback, *args))
-                timer.start()
-                return timer
-
-        xra = _get_as_int(response_headers, "Retry-After", 0)
-        if xra:
-            self._deferred = call_later(xra, self._release)
-            return
-        xrlr = _get_as_int(response_headers, "RateLimit-Remaining", 1)
-        if xrlr:
-            return
-        xrlr = _get_as_int(response_headers, "RateLimit-Reset", 0)
-        self._deferred = call_later(xrlr, self._release)
+        self._deferred = _ThreadTimer(delay, self._release)
 
     def locked(self):
         return self._lock.locked()
 
     def release(self):
         if self.deferred is not None:
             return
         self._wake_up_next()
         self._lock.release()
 
     def _release(self):
         del self._deferred
         self._wake_up_next()
         self._lock.release()
+
+
+if __name__ == "__main__":
+    from concurrent.futures import ThreadPoolExecutor
+
+    from anyio.lowlevel import checkpoint
+
+    async def main():
+        lock = ResetLock()
+
+        def target(lock=lock):
+            print("before threading lock")
+            with lock:
+                print("during threading lock")
+                lock.defer(1)
+            print("after threading lock")
+
+        async def async_target(lock=lock):
+            lib = sniffio.current_async_library()
+            print(f"before {lib} lock")
+            async with lock:
+                print(f"during {lib} lock")
+                lock.defer(1)
+                await checkpoint()
+            print(f"after {lib} lock")
+
+        with ThreadPoolExecutor() as pool:
+            async with anyio.create_task_group() as group:
+                for _ in range(5):
+                    group.start_soon(async_target)
+                    pool.submit(target)
+                    await checkpoint()
+
+    anyio.run(main, backend="asyncio")
+    anyio.run(main, backend="trio")
```

### Comparing `sans-1.1.4/sans/response.py` & `sans-1.2.0/sans/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,8 +101,8 @@
                 self._lxml = decoder.flush()
             return self._lxml
 
     def raise_for_status(self) -> None:
         try:
             return super().raise_for_status()
         except httpx.HTTPStatusError as exc:
-            raise narrow(exc) from None
+            raise narrow(exc).with_traceback(exc.__traceback__) from None
```

### Comparing `sans-1.1.4/sans/url.py` & `sans-1.2.0/sans/url.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "World",
     "WA",
     "Command",
     "Shard",
     "NationsDump",
     "RegionsDump",
     "CardsDump",
+    "Telegram",
 ]
 
 
 def Nation(nation: str, *shards: str | _Shard, **parameters: str) -> httpx.URL:
     return World(*shards, nation=nation, **parameters)
 
 
@@ -44,29 +45,31 @@
             query.update(shard)
         else:
             q.append(str(shard))
     q_str = " ".join(map(str, filter(None, q)))
     if q_str:
         query["q"] = q_str
     query.update(parameters)
-    if query.get("a", "").lower() == "sendtg":
-        raise RuntimeError("sans does not currently support the telegram API.")
     return API_URL.copy_with(params=query)
 
 
 def WA(
     wa: Literal[1, "1", 2, "2"], *shards: str | _Shard, **parameters: str
 ) -> httpx.URL:
     return World(*shards, wa=str(wa), **parameters)
 
 
 def Command(nation: str, c: str, **parameters: str) -> httpx.URL:
     return World(nation=nation, c=c, **parameters)
 
 
+def Telegram(client: str, tgid: str, key: str, to: str):
+    return World(a="sendtg", client=client, tgid=tgid, key=key, to=to)
+
+
 def Shard(q: str, **parameters: str) -> _Shard:
     parameters["q"] = q
     return parameters  # type: ignore
 
 
 # https://www.nationstates.net/archive/nations/2018-09-30-nations-xml.gz
 def NationsDump(date: _date | None = None) -> httpx.URL:
```

### Comparing `sans-1.1.4/sans/utils.py` & `sans-1.2.0/sans/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 from __future__ import annotations
 
 import sys
+from contextlib import ExitStack
 from typing import Any, Coroutine, overload
 from xml.etree import ElementTree as etree
 
 import httpx
 
 from .auth import NSAuth
-from .client import AsyncClientType, ClientType
+from .client import AsyncClient, Client
 from .response import Response
 from .url import Command
 
 __all__ = ["prepare_and_execute", "indent"]
 
 
 @overload
 def prepare_and_execute(
-    client: ClientType, auth: NSAuth, nation: str, c: str, **parameters: str
+    client: Client | None, auth: NSAuth, nation: str, c: str, **parameters: str
 ) -> Response:
     ...
 
 
 @overload
 async def prepare_and_execute(
-    client: AsyncClientType, auth: NSAuth, nation: str, c: str, **parameters: str
+    client: AsyncClient, auth: NSAuth, nation: str, c: str, **parameters: str
 ) -> Response:
     ...
 
 
 def prepare_and_execute(
-    client: ClientType | AsyncClientType,
+    client: Client | AsyncClient | None,
     auth: NSAuth,
     nation: str,
     c: str,
     **parameters: str,
 ) -> Response | Coroutine[Any, Any, Response]:
     if isinstance(client, httpx.AsyncClient):
         return _prepare_async(client, auth, nation, c, **parameters)
-    request = Command(nation, c, **parameters, mode="prepare")
-    response = client.get(request, auth=auth)
-    response.raise_for_status()
-    token: str = response.xml.find("SUCCESS").text  # type: ignore
-    request = Command(nation, c, **parameters, mode="execute", token=token)
-    return client.get(request, auth=auth)
+    with ExitStack() as stack:
+        if not client:
+            client = stack.enter_context(Client())
+        request = Command(nation, c, **parameters, mode="prepare")
+        response = client.get(request, auth=auth)
+        response.raise_for_status()
+        token: str = response.xml.find("SUCCESS").text  # type: ignore
+        request = Command(nation, c, **parameters, mode="execute", token=token)
+        return client.get(request, auth=auth)
+    # pyright incorrectly believes this line is reachable
+    assert False  # noqa: B011
 
 
 async def _prepare_async(
-    client: AsyncClientType, auth: NSAuth, nation: str, c: str, **parameters: str
+    client: AsyncClient, auth: NSAuth, nation: str, c: str, **parameters: str
 ) -> Response:
     request = Command(nation, c, **parameters, mode="prepare")
     response = await client.get(request, auth=auth)
     response.raise_for_status()
     token: str = response.xml.find("SUCCESS").text  # type: ignore
     request = Command(nation, c, **parameters, mode="execute", token=token)
     return await client.get(request, auth=auth)
```

### Comparing `sans-1.1.4/sans.egg-info/PKG-INFO` & `sans-1.2.0/sans.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.1.4
+Version: 1.2.0
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,140 +42,150 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: <4.0,>=3.7.0
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: lxml
 Provides-Extra: json
 License-File: LICENSE
 
-sans
-====
+# sans
 
-|pypi| |Code style: black| |Build Status| |Documentation Status|
+[![pypi](https://img.shields.io/pypi/v/sans.svg) ![Licensed under the MIT License](https://img.shields.io/pypi/l/sans.svg)](https://pypi.org/project/sans/)
+[![Downloads](https://static.pepy.tech/badge/sans)](https://pepy.tech/project/sans)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Zephyrkul/sans/master.svg)](https://results.pre-commit.ci/latest/github/Zephyrkul/sans/master)
+[![Documentation Status](https://readthedocs.org/projects/sans/badge/?version=latest)](http://sans.readthedocs.org/en/latest/?badge=latest)
 
-**S**\ ynchronous / **A**\ synchronous **N**\ ation\ **S**\ tates
+**S**ynchronous / **A**synchronous **N**ation**S**tates
 
-A `fully typed <https://docs.python.org/3/library/typing.html>`_ extension for `HTTPX <https://www.python-httpx.org/>`_ for the `NationStates API <https://www.nationstates.net/pages/api.html>`_.
+A [fully typed](https://docs.python.org/3/library/typing.html>) extension for [HTTPX](https://www.python-httpx.org/) for the [NationStates API](https://www.nationstates.net/pages/api.html).
 
-Installing
-----------
+## Installing
 
-.. code::
-
-   python3 -m pip install -U sans
+```sh
+python3 -m pip install -U sans
+```
 
 Development version:
 
-.. code::
-
-   python3 -m pip install -U https://github.com/zephyrkul/sans/archive/master.zip#egg=sans
-
-Examples
---------
-
-Synchronous
-~~~~~~~~~~~
-
-.. code:: python
-
-   import sans
-   from xml.etree import ElementTree as ET
-
-   def main():
-      sans.set_agent("Darcania")
+```sh
+python3 -m pip install -U https://github.com/zephyrkul/sans/archive/master.zip#egg=sans
+```
+
+## Examples
+
+### Synchronous
+
+```py
+import sans
+from xml.etree import ElementTree as ET
+
+def main():
+   sans.set_agent("Darcania")
+   request = sans.Nation(
+      "darcania",
+      "fullname population flag census",
+      mode="score",
+      scale="65 66",
+   )
+   root = sans.get(request).xml
+   sans.indent(root)
+   print(ET.tostring(root, encoding="unicode"))
+
+   with sans.stream("GET", sans.RegionsDump()) as response:
+      for region in response.iter_xml():
+         sans.indent(region)
+         print(ET.tostring(region, encoding="unicode"))
+
+if __name__ == "__main__":
+   main()
+```
+
+### Asynchronous
+
+```py
+import asyncio
+import sans
+from xml.etree import ElementTree as ET
+
+async def main():
+   sans.set_agent("Darcania")
+   async with sans.AsyncClient() as client:
       request = sans.Nation(
          "darcania",
          "fullname population flag census",
          mode="score",
          scale="65 66",
       )
-      root = sans.get(request).xml
+      root = (await client.send(request)).xml
       sans.indent(root)
       print(ET.tostring(root, encoding="unicode"))
 
-      with sans.stream("GET", sans.RegionsDump()) as response:
-         for region in response.iter_xml():
+      async with client.stream("GET", sans.RegionsDump()) as response:
+         async for region in response.aiter_xml():
             sans.indent(region)
             print(ET.tostring(region, encoding="unicode"))
 
-   if __name__ == "__main__":
-      main()
-
-Asynchronous
-~~~~~~~~~~~~
-
-.. code:: python
-
-   import asyncio
-   import sans
-   from xml.etree import ElementTree as ET
-
-   async def main():
-      sans.set_agent("Darcania")
-      async with sans.AsyncClient() as client:
-         request = sans.Nation(
-            "darcania",
-            "fullname population flag census",
-            mode="score",
-            scale="65 66",
-         )
-         root = (await client.send(request)).xml
-         sans.indent(root)
-         print(ET.tostring(root, encoding="unicode"))
-
-         async with client.stream("GET", sans.RegionsDump()) as response:
-            async for region in response.aiter_xml():
-               sans.indent(region)
-               print(ET.tostring(region, encoding="unicode"))
-
-   if __name__ == "__main__":
-      asyncio.run(main())
-
-Command Line
-------------
-
-.. code::
-
-   $ sans --nation darcania census --scale "65 66" --mode score --agent Darcania
-
+if __name__ == "__main__":
+   asyncio.run(main())
+```
+
+### Authentication
+
+```py
+auth = sans.NSAuth(password="hunter2")
+sans.get(sans.Nation("testlandia", "ping"), auth=auth)
+# X-Autologin is automatically retrieved and stored for when the auth object is re-used
+print(auth.autologin)
+# X-Pin is cached internally for repeated requests
+root = sans.get(sans.Nation("testlandia", "packs"), auth=auth).xml
+```
+
+### Telegrams
+
+```py
+limiter = sans.TelegramLimiter(recruitment=False)
+# The Telegram API can be used without a TelegramLimiter, but marking it ahead of time can save an API call.
+response = sans.get(sans.Telegram(client="abcd1234", tgid="1234", key="abcdef1234567890", to="testlandia"), auth=limiter)
+assert response.content = b"queued"
+```
+
+## Command Line
+
+```xml
+sans --nation darcania census --scale "65 66" --mode score --agent Darcania
+<NATION id="darcania">
    <CENSUS>
       <SCALE id="65">
-         <SCORE>4949.00</SCORE>
+         <SCORE>8145.00</SCORE>
       </SCALE>
       <SCALE id="66">
-         <SCORE>130.00</SCORE>
+         <SCORE>0.00</SCORE>
       </SCALE>
    </CENSUS>
+</NATION>
 
-   $ sans --nation testlandia fullname
-
+sans --nation testlandia fullname
+<NATION id="testlandia">
    <FULLNAME>The Hive Mind of Testlandia</FULLNAME>
+</NATION>
 
-   sans --region "the north pacific" numnations lastupdate
-
-   <LASTUPDATE>1683650325</LASTUPDATE>
-   <NUMNATIONS>10503</NUMNATIONS>
+sans --region "the north pacific" numnations lastupdate
+<REGION id="the_north_pacific">
+   <LASTUPDATE>1685681810</LASTUPDATE>
+   <NUMNATIONS>9535</NUMNATIONS>
+</REGION>
+
+sans --quit
+No query provided. Exiting...
+```
 
-   $ sans --quit
-   No query provided. Exiting...
+## Requirements
 
-Requirements
-------------
-
--  Python 3.7+
--  httpx
-
-.. |pypi| image:: https://img.shields.io/pypi/v/sans.svg
-   :target: https://pypi.python.org/pypi/sans
-   :alt: pypi version
-.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/ambv/black
-.. |Build Status| image:: https://results.pre-commit.ci/badge/github/Zephyrkul/sans/master.svg
-   :target: https://results.pre-commit.ci/latest/github/Zephyrkul/sans/master
-   :alt: pre-commit.ci status
-.. |Documentation Status| image:: https://readthedocs.org/projects/sans/badge/?version=latest
-   :target: http://sans.readthedocs.org/en/latest/?badge=latest
+- [Python 3.7+](https://www.python.org/)
+- [httpx](https://pypi.org/project/httpx/)
```

### Comparing `sans-1.1.4/sans.egg-info/SOURCES.txt` & `sans-1.2.0/sans.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
-README.rst
+README.md
 pyproject.toml
 requirements.txt
 setup.py
 .github/workflows/codeql-analysis.yml
 .github/workflows/pythonpublish.yml
 docs/Makefile
 docs/auth.rst
@@ -17,22 +17,21 @@
 docs/lock.rst
 docs/make.bat
 docs/response.rst
 docs/url.rst
 docs/utils.rst
 sans/__init__.py
 sans/__main__.py
-sans/_state.py
+sans/_lock.py
 sans/auth.py
 sans/client.py
 sans/client.pyi
 sans/decoder.py
 sans/errors.py
 sans/limiter.py
-sans/lock.py
 sans/py.typed
 sans/response.py
 sans/url.py
 sans/utils.py
 sans.egg-info/PKG-INFO
 sans.egg-info/SOURCES.txt
 sans.egg-info/dependency_links.txt
```

