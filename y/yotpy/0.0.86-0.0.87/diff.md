# Comparing `tmp/yotpy-0.0.86.tar.gz` & `tmp/yotpy-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.86.tar", last modified: Wed May 17 18:40:42 2023, max compression
+gzip compressed data, was "yotpy-0.0.87.tar", last modified: Mon Jun  5 17:54:25 2023, max compression
```

## Comparing `yotpy-0.0.86.tar` & `yotpy-0.0.87.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.86/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.86/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.86/LICENSE
--rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.86/README.md
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.86/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.86/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.86/docs/yotpy.html
--rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.86/pyproject.toml
--rw-r--r--   0        0        0      318 2023-05-17 18:32:02.176845 yotpy-0.0.86/yotpy/__init__.py
--rw-r--r--   0        0        0    33804 2023-05-17 18:33:54.895065 yotpy-0.0.86/yotpy/core.py
--rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.86/yotpy/exceptions.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 yotpy-0.0.86/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.87/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.87/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.87/LICENSE
+-rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.87/README.md
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.87/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.87/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.87/docs/yotpy.html
+-rw-r--r--   0        0        0      847 2023-06-05 17:53:47.739564 yotpy-0.0.87/pyproject.toml
+-rw-r--r--   0        0        0      318 2023-06-05 17:53:59.854921 yotpy-0.0.87/yotpy/__init__.py
+-rw-r--r--   0        0        0    33804 2023-05-30 01:05:45.086759 yotpy-0.0.87/yotpy/core.py
+-rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.87/yotpy/exceptions.py
+-rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 yotpy-0.0.87/PKG-INFO
```

### Comparing `yotpy-0.0.86/.github/workflows/static.yml` & `yotpy-0.0.87/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.86/LICENSE` & `yotpy-0.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.86/docs/search.js` & `yotpy-0.0.87/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.86/docs/yotpy.html` & `yotpy-0.0.87/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.86/pyproject.toml` & `yotpy-0.0.87/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.11",
 ]
 requires = [
     "aiohttp",
     "requests",
+    "openpyxl",
 ]
 keywords = "yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce"
 
 [tool.flit.metadata.urls]
 Documentation = "https://wlk-dev.github.io/yotpy/yotpy.html"
 
 [tool.flit.metadata.requires-extra]
```

### Comparing `yotpy-0.0.86/yotpy/core.py` & `yotpy-0.0.87/yotpy/core.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.86/yotpy/exceptions.py` & `yotpy-0.0.87/yotpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.86/PKG-INFO` & `yotpy-0.0.87/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.86
+Version: 0.0.87
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp
 Requires-Dist: requests
+Requires-Dist: openpyxl
 Project-URL: Documentation, https://wlk-dev.github.io/yotpy/yotpy.html
 
 # Yotpy
 
 An easy-to-use Python wrapper for the Yotpo API. Developed to fill the gap of existing packages that didn't meet specific needs.
 
 ## Installation
```

