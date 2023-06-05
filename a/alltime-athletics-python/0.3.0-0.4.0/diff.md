# Comparing `tmp/alltime_athletics_python-0.3.0.tar.gz` & `tmp/alltime_athletics_python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alltime_athletics_python-0.3.0.tar", max compression
+gzip compressed data, was "alltime_athletics_python-0.4.0.tar", max compression
```

## Comparing `alltime_athletics_python-0.3.0.tar` & `alltime_athletics_python-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-01 06:57:21.506681 alltime_athletics_python-0.3.0/LICENSE
--rw-r--r--   0        0        0      299 2023-06-01 06:57:21.522140 alltime_athletics_python-0.3.0/alltime_athletics_python/__init__.py
--rw-r--r--   0        0        0     3205 2023-06-01 06:58:25.637564 alltime_athletics_python-0.3.0/alltime_athletics_python/get_content.py
--rw-r--r--   0        0        0     1915 2023-06-01 06:58:25.645679 alltime_athletics_python-0.3.0/alltime_athletics_python/get_content_urls.py
--rw-r--r--   0        0        0     3342 2023-06-05 07:05:46.470276 alltime_athletics_python-0.3.0/alltime_athletics_python/io.py
--rw-r--r--   0        0        0    10197 2023-06-05 06:57:35.426514 alltime_athletics_python-0.3.0/alltime_athletics_python/pipes.py
--rw-r--r--   0        0        0        0 2023-06-01 06:57:21.524099 alltime_athletics_python-0.3.0/alltime_athletics_python/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-06-01 06:57:21.523437 alltime_athletics_python-0.3.0/alltime_athletics_python/utils/config.py
--rw-r--r--   0        0        0      736 2023-06-01 06:57:21.525381 alltime_athletics_python-0.3.0/alltime_athletics_python/utils/logger.py
--rw-r--r--   0        0        0      924 2023-06-05 07:06:17.634912 alltime_athletics_python-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 alltime_athletics_python-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-01 06:57:21.506681 alltime_athletics_python-0.4.0/LICENSE
+-rw-r--r--   0        0        0      299 2023-06-01 06:57:21.522140 alltime_athletics_python-0.4.0/alltime_athletics_python/__init__.py
+-rw-r--r--   0        0        0     3205 2023-06-01 06:58:25.637564 alltime_athletics_python-0.4.0/alltime_athletics_python/get_content.py
+-rw-r--r--   0        0        0     1915 2023-06-01 06:58:25.645679 alltime_athletics_python-0.4.0/alltime_athletics_python/get_content_urls.py
+-rw-r--r--   0        0        0     3342 2023-06-05 07:05:46.470276 alltime_athletics_python-0.4.0/alltime_athletics_python/io.py
+-rw-r--r--   0        0        0    10197 2023-06-05 06:57:35.426514 alltime_athletics_python-0.4.0/alltime_athletics_python/pipes.py
+-rw-r--r--   0        0        0        0 2023-06-01 06:57:21.524099 alltime_athletics_python-0.4.0/alltime_athletics_python/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-01 06:57:21.523437 alltime_athletics_python-0.4.0/alltime_athletics_python/utils/config.py
+-rw-r--r--   0        0        0      736 2023-06-01 06:57:21.525381 alltime_athletics_python-0.4.0/alltime_athletics_python/utils/logger.py
+-rw-r--r--   0        0        0      924 2023-06-05 07:08:54.895206 alltime_athletics_python-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 alltime_athletics_python-0.4.0/PKG-INFO
```

### Comparing `alltime_athletics_python-0.3.0/LICENSE` & `alltime_athletics_python-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.3.0/alltime_athletics_python/get_content.py` & `alltime_athletics_python-0.4.0/alltime_athletics_python/get_content.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.3.0/alltime_athletics_python/get_content_urls.py` & `alltime_athletics_python-0.4.0/alltime_athletics_python/get_content_urls.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.3.0/alltime_athletics_python/io.py` & `alltime_athletics_python-0.4.0/alltime_athletics_python/io.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.3.0/alltime_athletics_python/pipes.py` & `alltime_athletics_python-0.4.0/alltime_athletics_python/pipes.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.3.0/alltime_athletics_python/utils/config.py` & `alltime_athletics_python-0.4.0/alltime_athletics_python/utils/config.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.3.0/alltime_athletics_python/utils/logger.py` & `alltime_athletics_python-0.4.0/alltime_athletics_python/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.3.0/pyproject.toml` & `alltime_athletics_python-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "alltime_athletics_python"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.2"
 lxml = "^4.9.2"
 html5lib = "^1.1"
 rich = "^13.4.1"
+polars = "^0.18.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.1"
 ruff = "^0.0.253"
 black = "^23.1.0"
 pyclean = "^2.2.0"
 pre-commit = "^3.1.1"
 ipykernel = "^6.16.1"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 rich = "^13.3.2"
-polars = "^0.18.0"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 ignore = [
```

