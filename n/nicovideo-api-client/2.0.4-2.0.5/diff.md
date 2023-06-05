# Comparing `tmp/nicovideo_api_client-2.0.4.tar.gz` & `tmp/nicovideo_api_client-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicovideo_api_client-2.0.4.tar", max compression
+gzip compressed data, was "nicovideo_api_client-2.0.5.tar", max compression
```

## Comparing `nicovideo_api_client-2.0.4.tar` & `nicovideo_api_client-2.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1593 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/README.md
--rw-r--r--   0        0        0        0 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/__init__.py
--rw-r--r--   0        0        0      843 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/field.py
--rw-r--r--   0        0        0     1892 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/filter.py
--rw-r--r--   0        0        0     5731 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/json_filter.py
--rw-r--r--   0        0        0      734 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/limit.py
--rw-r--r--   0        0        0     4143 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/request.py
--rw-r--r--   0        0        0     4006 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/result.py
--rw-r--r--   0        0        0     5749 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/simple_filter.py
--rw-r--r--   0        0        0     3951 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/snapshot_search_api_v2.py
--rw-r--r--   0        0        0      882 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/sort.py
--rw-r--r--   0        0        0     5716 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/targets.py
--rw-r--r--   0        0        0     1342 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/user_agent.py
--rw-r--r--   0        0        0     2833 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/constants.py
--rw-r--r--   0        0        0     1446 2023-04-12 09:46:50.494626 nicovideo_api_client-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 nicovideo_api_client-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1593 2023-06-05 01:41:07.040930 nicovideo_api_client-2.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 01:41:07.040930 nicovideo_api_client-2.0.5/nicovideo_api_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:41:07.040930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:41:07.040930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/__init__.py
+-rw-r--r--   0        0        0      843 2023-06-05 01:41:07.040930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/field.py
+-rw-r--r--   0        0        0     1892 2023-06-05 01:41:07.040930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/filter.py
+-rw-r--r--   0        0        0     5731 2023-06-05 01:41:07.040930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/json_filter.py
+-rw-r--r--   0        0        0      734 2023-06-05 01:41:07.040930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/limit.py
+-rw-r--r--   0        0        0     4143 2023-06-05 01:41:07.044930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/request.py
+-rw-r--r--   0        0        0     4006 2023-06-05 01:41:07.044930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/result.py
+-rw-r--r--   0        0        0     5749 2023-06-05 01:41:07.044930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/simple_filter.py
+-rw-r--r--   0        0        0     3951 2023-06-05 01:41:07.044930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/snapshot_search_api_v2.py
+-rw-r--r--   0        0        0      882 2023-06-05 01:41:07.044930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/sort.py
+-rw-r--r--   0        0        0     5716 2023-06-05 01:41:07.044930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/targets.py
+-rw-r--r--   0        0        0     1342 2023-06-05 01:41:07.044930 nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/user_agent.py
+-rw-r--r--   0        0        0     2833 2023-06-05 01:41:07.044930 nicovideo_api_client-2.0.5/nicovideo_api_client/constants.py
+-rw-r--r--   0        0        0     1446 2023-06-05 01:41:29.449175 nicovideo_api_client-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 nicovideo_api_client-2.0.5/PKG-INFO
```

### Comparing `nicovideo_api_client-2.0.4/README.md` & `nicovideo_api_client-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/field.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/field.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/filter.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/filter.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/json_filter.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/json_filter.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/limit.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/limit.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/request.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/request.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/result.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/result.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/simple_filter.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/simple_filter.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/snapshot_search_api_v2.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/snapshot_search_api_v2.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/sort.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/sort.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/targets.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/targets.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/user_agent.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/api/v2/user_agent.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/nicovideo_api_client/constants.py` & `nicovideo_api_client-2.0.5/nicovideo_api_client/constants.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.4/pyproject.toml` & `nicovideo_api_client-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nicovideo_api_client"
-version = "2.0.4"
+version = "2.0.5"
 description = "ニコニコ動画 スナップショット検索APIv2の Python クライアント"
 authors = ["Javakky <iemura.java@gmail.com>"]
 homepage = "https://github.com/Javakky/NicoApiClient"
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python",
@@ -17,15 +17,15 @@
 requests = "^2.26.0"
 urllib3 = "^1.26.6"
 
 [tool.poetry.dev-dependencies]
 sphinx-rtd-theme = "^1.2.0"
 pytest = "^7.2.1"
 Sphinx = "^6.1.3"
-taskipy = "^1.10.3"
+taskipy = "^1.11.0"
 pyproject-flake8 = "^6.0.0.post1"
 install = "^1.3.5"
 black = "^23.1"
 isort = "5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `nicovideo_api_client-2.0.4/PKG-INFO` & `nicovideo_api_client-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: nicovideo-api-client
-Version: 2.0.4
+Version: 2.0.5
 Summary: ニコニコ動画 スナップショット検索APIv2の Python クライアント
 Home-page: https://github.com/Javakky/NicoApiClient
 Author: Javakky
 Author-email: iemura.java@gmail.com
 Requires-Python: >=3.10.2,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # NicoApiClient
```

