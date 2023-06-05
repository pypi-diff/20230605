# Comparing `tmp/nonebug_saa-0.1.0.tar.gz` & `tmp/nonebug_saa-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebug_saa-0.1.0.tar", max compression
+gzip compressed data, was "nonebug_saa-0.2.1.tar", max compression
```

## Comparing `nonebug_saa-0.1.0.tar` & `nonebug_saa-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      175 2023-03-26 08:27:44.709877 nonebug_saa-0.1.0/README.md
--rw-r--r--   0        0        0     1265 2023-03-26 08:27:44.709877 nonebug_saa-0.1.0/nonebot_plugin_saa/nonebug/__init__.py
--rw-r--r--   0        0        0     1224 2023-03-26 08:27:44.709877 nonebug_saa-0.1.0/nonebot_plugin_saa/nonebug/fixtures.py
--rw-r--r--   0        0        0     1071 2023-03-26 08:27:44.709877 nonebug_saa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 nonebug_saa-0.1.0/setup.py
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 nonebug_saa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      175 2023-03-26 08:26:02.032585 nonebug_saa-0.2.1/README.md
+-rw-r--r--   0        0        0     1338 2023-05-08 13:44:44.608904 nonebug_saa-0.2.1/nonebug_saa/__init__.py
+-rw-r--r--   0        0        0     1657 2023-06-05 15:05:01.455854 nonebug_saa-0.2.1/nonebug_saa/fixtures.py
+-rw-r--r--   0        0        0     1049 2023-06-05 15:06:15.843448 nonebug_saa-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 nonebug_saa-0.2.1/PKG-INFO
```

### Comparing `nonebug_saa-0.1.0/nonebot_plugin_saa/nonebug/__init__.py` & `nonebug_saa-0.2.1/nonebug_saa/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Optional
 
+from nonebot import require
 from nonebot.adapters import Bot, Event
 from nonebug.mixin.call_api import ApiContext
 
-from nonebot_plugin_saa import (
+require("nonebot_plugin_saa")
+
+from nonebot_plugin_saa import (  # noqa: E402
     MessageFactory,
     PlatformTarget,
     AggregatedMessageFactory,
     extract_target,
 )
```

### Comparing `nonebug_saa-0.1.0/pyproject.toml` & `nonebug_saa-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "nonebug-saa"
-version = "0.1.0"
+version = "0.2.1"
 description = "A nonebug helper for nonebot-plugin-send-anything-anything"
 authors = ["felinae98 <me@felinae98.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/felinae98/nonebug-saa"
-packages = [{include = "nonebot_plugin_saa"}]
+packages = [{include = "nonebug_saa"}]
 repository = ""
 documentation = ""
 keywords = []
 classifiers = ["Framework :: Pytest"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 nonebug = "^0.3.1"
 pytest-mock = "^3.10.0"
-nonebot-plugin-send-anything-anywhere = "^0.2.2"
+nonebot-plugin-send-anything-anywhere = "^0.2.4"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
 black = "^22.3.0"
 nonemoji = "^0.1.2"
 pre-commit = "^2.16.0"
 
 [tool.poetry.plugins.pytest11]
-saa_nonebug = "nonebot_plugin_saa.nonebug.fixtures"
+saa_nonebug = "nonebug_saa.fixtures"
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
 extend-exclude = '''
 '''
```

### Comparing `nonebug_saa-0.1.0/PKG-INFO` & `nonebug_saa-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebug-saa
-Version: 0.1.0
+Version: 0.2.1
 Summary: A nonebug helper for nonebot-plugin-send-anything-anything
 Home-page: https://github.com/felinae98/nonebug-saa
 License: MIT
 Author: felinae98
 Author-email: me@felinae98.cn
 Requires-Python: >=3.10,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.2,<0.3.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.4,<0.3.0)
 Requires-Dist: nonebug (>=0.3.1,<0.4.0)
 Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 ~logo征集中，假装有图片~
```

