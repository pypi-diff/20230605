# Comparing `tmp/langchainplus_sdk-0.0.3.tar.gz` & `tmp/langchainplus_sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchainplus_sdk-0.0.3.tar", max compression
+gzip compressed data, was "langchainplus_sdk-0.0.4.tar", max compression
```

## Comparing `langchainplus_sdk-0.0.3.tar` & `langchainplus_sdk-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0     8124 2023-06-02 21:13:33.795742 langchainplus_sdk-0.0.3/README.md
--rw-r--r--   0        0        0      529 2023-06-02 21:13:33.795742 langchainplus_sdk-0.0.3/langchainplus_sdk/__init__.py
--rw-r--r--   0        0        0    18507 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/client.py
--rw-r--r--   0        0        0      250 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/evaluation/__init__.py
--rw-r--r--   0        0        0      738 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/evaluation/evaluator.py
--rw-r--r--   0        0        0     1545 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     7178 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/run_trees.py
--rw-r--r--   0        0        0     7001 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/schemas.py
--rw-r--r--   0        0        0     3235 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/langchainplus_sdk/utils.py
--rw-r--r--   0        0        0      782 2023-06-02 21:13:33.799742 langchainplus_sdk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     8124 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/README.md
+-rw-r--r--   0        0        0      529 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      315 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1198 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    12934 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/cli/main.py
+-rw-r--r--   0        0        0    18507 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/client.py
+-rw-r--r--   0        0        0      250 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/evaluation/__init__.py
+-rw-r--r--   0        0        0      738 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1545 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     7178 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/run_trees.py
+-rw-r--r--   0        0        0     7001 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/schemas.py
+-rw-r--r--   0        0        0     3235 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/langchainplus_sdk/utils.py
+-rw-r--r--   0        0        0      879 2023-06-05 18:56:13.160396 langchainplus_sdk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 langchainplus_sdk-0.0.4/PKG-INFO
```

### Comparing `langchainplus_sdk-0.0.3/README.md` & `langchainplus_sdk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.3/langchainplus_sdk/__init__.py` & `langchainplus_sdk-0.0.4/langchainplus_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.3/langchainplus_sdk/client.py` & `langchainplus_sdk-0.0.4/langchainplus_sdk/client.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.3/langchainplus_sdk/evaluation/evaluator.py` & `langchainplus_sdk-0.0.4/langchainplus_sdk/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.3/langchainplus_sdk/evaluation/string_evaluator.py` & `langchainplus_sdk-0.0.4/langchainplus_sdk/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.3/langchainplus_sdk/run_trees.py` & `langchainplus_sdk-0.0.4/langchainplus_sdk/run_trees.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.3/langchainplus_sdk/schemas.py` & `langchainplus_sdk-0.0.4/langchainplus_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.3/langchainplus_sdk/utils.py` & `langchainplus_sdk-0.0.4/langchainplus_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `langchainplus_sdk-0.0.3/pyproject.toml` & `langchainplus_sdk-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 [tool.poetry]
 name = "langchainplus-sdk"
-version = "0.0.3"
+version = "0.0.4"
 description = "Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langchainplus_sdk"}]
 
+[tool.poetry.scripts]
+langchain = "langchainplus_sdk.cli.main:main"
+
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 pydantic = "^1"
 requests = "^2"
 tenacity = "^8.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 mypy = "^1.3.0"
 ruff = "^0.0.270"
 types-requests = "^2.31.0.1"
 pandas-stubs = "^2.0.1.230501"
+types-pyyaml = "^6.0.12.10"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = [
```

### Comparing `langchainplus_sdk-0.0.3/PKG-INFO` & `langchainplus_sdk-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchainplus-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Client library to connect to the LangChainPlus LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

