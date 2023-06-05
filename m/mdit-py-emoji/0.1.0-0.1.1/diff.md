# Comparing `tmp/mdit-py-emoji-0.1.0.tar.gz` & `tmp/mdit-py-emoji-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdit-py-emoji-0.1.0.tar", last modified: Tue Sep 27 05:54:30 2022, max compression
+gzip compressed data, was "mdit-py-emoji-0.1.1.tar", last modified: Mon Jun  5 10:20:42 2023, max compression
```

## Comparing `mdit-py-emoji-0.1.0.tar` & `mdit-py-emoji-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-27 05:54:22.615885 mdit-py-emoji-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-09-27 05:54:22.615885 mdit-py-emoji-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-09-27 05:54:22.615885 mdit-py-emoji-0.1.0/mdit_py_emoji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    53374 2022-09-27 05:54:22.615885 mdit-py-emoji-0.1.0/mdit_py_emoji/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-09-27 05:54:22.615885 mdit-py-emoji-0.1.0/mdit_py_emoji/rule.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-09-27 05:54:22.615885 mdit-py-emoji-0.1.0/pyproject.toml
--rw-------   0 runner    (1001) docker     (121)     2203 2022-09-27 05:54:30.651859 mdit-py-emoji-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 10:20:26.653090 mdit-py-emoji-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2169 2023-06-05 10:20:26.653090 mdit-py-emoji-0.1.1/README.md
+-rw-r--r--   0        0        0     1492 2023-06-05 10:20:26.653090 mdit-py-emoji-0.1.1/mdit_py_emoji/__init__.py
+-rw-r--r--   0        0        0    53374 2023-06-05 10:20:26.653090 mdit-py-emoji-0.1.1/mdit_py_emoji/data.py
+-rw-r--r--   0        0        0     2619 2023-06-05 10:20:26.653090 mdit-py-emoji-0.1.1/mdit_py_emoji/rule.py
+-rw-r--r--   0        0        0      753 2023-06-05 10:20:26.653090 mdit-py-emoji-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 mdit-py-emoji-0.1.1/PKG-INFO
```

### Comparing `mdit-py-emoji-0.1.0/LICENSE` & `mdit-py-emoji-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit-py-emoji-0.1.0/README.md` & `mdit-py-emoji-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,28 @@
 
 [![PyPI](https://img.shields.io/pypi/v/mdit-py-emoji)](https://pypi.org/project/mdit-py-emoji)
 [![Python Version](https://img.shields.io/pypi/pyversions/mdit-py-emoji)](https://pypi.org/project/mdit-py-emoji)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License](https://img.shields.io/github/license/BlueGlassBlock/mdit-py-emoji)](https://github.com/BlueGlassBlock/mdit-py-emoji/blob/master/LICENSE)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+[![codecov](https://codecov.io/github/BlueGlassBlock/mdit-py-emoji/branch/master/graph/badge.svg?token=3ZY58Z5IS1)](https://codecov.io/github/BlueGlassBlock/mdit-py-emoji)
 
 </div>
 
+## Installation
+
+Choose your favorite!
+
+```sh
+pip install mdit-py-emoji
+pdm add mdit-py-emoji
+poetry add mdit-py-emoji
+```
+
 ## Usage
 
 Use it just like other plugins!
 
 ```python
 from markdown_it import MarkdownIt
 from mdit_py_emoji import emoji_plugin
```

### Comparing `mdit-py-emoji-0.1.0/mdit_py_emoji/__init__.py` & `mdit-py-emoji-0.1.1/mdit_py_emoji/__init__.py`

 * *Files identical despite different names*

### Comparing `mdit-py-emoji-0.1.0/mdit_py_emoji/data.py` & `mdit-py-emoji-0.1.1/mdit_py_emoji/data.py`

 * *Files identical despite different names*

### Comparing `mdit-py-emoji-0.1.0/mdit_py_emoji/rule.py` & `mdit-py-emoji-0.1.1/mdit_py_emoji/rule.py`

 * *Files identical despite different names*

### Comparing `mdit-py-emoji-0.1.0/pyproject.toml` & `mdit-py-emoji-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [project]
 name = "mdit-py-emoji"
-version = "0.1.0"
+version = "0.1.1"
 description = "Emoji plugin for markdown-it-py."
 authors = [
     { name = "BlueGlassBlock", email = "blueglassblock@outlook.com" },
 ]
 dependencies = [
-    "markdown-it-py<3.0.0,>=1.0.0",
+    "markdown-it-py<4.0.0,>=1.0.0",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 
 [project.license]
 text = "MIT"
 
-[project.optional-dependencies]
-
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
 ]
 build-backend = "pdm.pep517.api"
 
 [tool.pdm.dev-dependencies]
```

### Comparing `mdit-py-emoji-0.1.0/PKG-INFO` & `mdit-py-emoji-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mdit-py-emoji
-Version: 0.1.0
+Version: 0.1.1
 Summary: Emoji plugin for markdown-it-py.
 License: MIT
 Author-email: BlueGlassBlock <blueglassblock@outlook.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 <div align=center>
 
 # mdit-py-emoji
@@ -16,17 +16,28 @@
 
 [![PyPI](https://img.shields.io/pypi/v/mdit-py-emoji)](https://pypi.org/project/mdit-py-emoji)
 [![Python Version](https://img.shields.io/pypi/pyversions/mdit-py-emoji)](https://pypi.org/project/mdit-py-emoji)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License](https://img.shields.io/github/license/BlueGlassBlock/mdit-py-emoji)](https://github.com/BlueGlassBlock/mdit-py-emoji/blob/master/LICENSE)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+[![codecov](https://codecov.io/github/BlueGlassBlock/mdit-py-emoji/branch/master/graph/badge.svg?token=3ZY58Z5IS1)](https://codecov.io/github/BlueGlassBlock/mdit-py-emoji)
 
 </div>
 
+## Installation
+
+Choose your favorite!
+
+```sh
+pip install mdit-py-emoji
+pdm add mdit-py-emoji
+poetry add mdit-py-emoji
+```
+
 ## Usage
 
 Use it just like other plugins!
 
 ```python
 from markdown_it import MarkdownIt
 from mdit_py_emoji import emoji_plugin
```

