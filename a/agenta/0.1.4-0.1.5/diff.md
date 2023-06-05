# Comparing `tmp/agenta-0.1.4.tar.gz` & `tmp/agenta-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agenta-0.1.4.tar", max compression
+gzip compressed data, was "agenta-0.1.5.tar", max compression
```

## Comparing `agenta-0.1.4.tar` & `agenta-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.4/README.md
--rw-r--r--   0        0        0       53 2023-05-20 06:49:49.205423 agenta-0.1.4/agenta/__init__.py
--rw-r--r--   0        0        0     3045 2023-05-30 19:16:46.669891 agenta-0.1.4/agenta/agenta.py
--rw-r--r--   0        0        0     6292 2023-05-31 17:19:38.375403 agenta-0.1.4/agenta/cli.py
--rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.4/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.4/agenta/client/__init__.py
--rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.4/agenta/client/api_models.py
--rw-r--r--   0        0        0     1479 2023-05-26 07:44:13.475577 agenta-0.1.4/agenta/client/client.py
--rw-r--r--   0        0        0      550 2023-05-11 14:46:01.166162 agenta-0.1.4/agenta/config.py
--rw-r--r--   0        0        0       91 2023-05-12 12:52:29.405049 agenta-0.1.4/agenta/config.toml
--rw-r--r--   0        0        0      337 2023-05-24 09:05:58.092867 agenta-0.1.4/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.4/agenta/docker/docker-assets/README.md
--rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.4/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     2585 2023-05-27 10:11:21.981693 agenta-0.1.4/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0      482 2023-05-31 17:12:43.842983 agenta-0.1.4/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.4/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.4/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.4/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0      513 2023-05-31 17:20:07.454240 agenta-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 agenta-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.5/README.md
+-rw-r--r--   0        0        0       53 2023-06-05 15:08:40.153249 agenta-0.1.5/agenta/__init__.py
+-rw-r--r--   0        0        0     3079 2023-06-05 15:08:40.153705 agenta-0.1.5/agenta/agenta.py
+-rw-r--r--   0        0        0     2378 2023-06-05 14:29:35.924380 agenta-0.1.5/agenta/cli/helper.py
+-rw-r--r--   0        0        0     2108 2023-06-05 14:29:35.924670 agenta-0.1.5/agenta/cli/main.py
+-rw-r--r--   0        0        0     8450 2023-06-05 14:29:35.924942 agenta-0.1.5/agenta/cli/variant_commands.py
+-rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.5/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.5/agenta/client/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.5/agenta/client/api_models.py
+-rw-r--r--   0        0        0     4355 2023-06-05 14:29:35.925335 agenta-0.1.5/agenta/client/client.py
+-rw-r--r--   0        0        0      641 2023-06-05 14:29:35.925644 agenta-0.1.5/agenta/config.py
+-rw-r--r--   0        0        0      131 2023-06-05 14:29:35.926009 agenta-0.1.5/agenta/config.toml
+-rw-r--r--   0        0        0      337 2023-05-24 09:05:58.092867 agenta-0.1.5/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.5/agenta/docker/docker-assets/README.md
+-rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.5/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     2585 2023-06-05 15:08:40.154263 agenta-0.1.5/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0      482 2023-05-31 17:12:43.842983 agenta-0.1.5/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.5/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.5/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.5/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0      570 2023-06-05 17:24:54.120338 agenta-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 agenta-0.1.5/PKG-INFO
```

### Comparing `agenta-0.1.4/agenta/agenta.py` & `agenta-0.1.5/agenta/agenta.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The code for the Agenta SDK"""
 import argparse
 import functools
 import inspect
 import os
 import sys
 from typing import Any, Callable, Optional
```

### Comparing `agenta-0.1.4/agenta/config.py` & `agenta-0.1.5/agenta/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 # Load the settings from the .toml file
 toml_config = toml.load(f"{Path(__file__).parent}/config.toml")
 
 # Set the environment variables from the TOML configurations
 os.environ["DOCKER_REGISTRY_URL"] = toml_config["docker_registry_url"]
 os.environ["DATABASE_URL"] = toml_config["database_url"]
 os.environ["REGISTRY"] = toml_config["registry"]
+os.environ["BACKEND_ENDPOINT"] = toml_config["backend_endpoint"]
 
 
 class Settings(BaseSettings):
     docker_registry_url: str
     database_url: str
     registry: str
+    backend_endpoint: str
 
 
 settings = Settings()
```

### Comparing `agenta-0.1.4/agenta/docker/docker_utils.py` & `agenta-0.1.5/agenta/docker/docker_utils.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.4/agenta/templates/simple_prompt/app.py` & `agenta-0.1.5/agenta/templates/simple_prompt/app.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.4/pyproject.toml` & `agenta-0.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "agenta"
-version = "0.1.4"
-description = ""
+version = "0.1.5"
+description = "Code for the SDK and CLI for the Agenta Lab platform"
 authors = ["Mahmoud Mabrouk <mahmoudmabrouk.mail@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docker = "^6.1.1"
 click = "^8.1.3"
@@ -19,8 +19,8 @@
 pytest = "^6.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-agenta = "agenta.cli:cli"
+agenta = "agenta.cli.main:cli"
```

### Comparing `agenta-0.1.4/PKG-INFO` & `agenta-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: agenta
-Version: 0.1.4
-Summary: 
+Version: 0.1.5
+Summary: Code for the SDK and CLI for the Agenta Lab platform
 Author: Mahmoud Mabrouk
 Author-email: mahmoudmabrouk.mail@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

