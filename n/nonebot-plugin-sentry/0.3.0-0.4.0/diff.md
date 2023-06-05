# Comparing `tmp/nonebot_plugin_sentry-0.3.0.tar.gz` & `tmp/nonebot_plugin_sentry-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sentry-0.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_sentry-0.4.0.tar", max compression
```

## Comparing `nonebot_plugin_sentry-0.3.0.tar` & `nonebot_plugin_sentry-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1413 2023-04-14 09:29:05.547658 nonebot_plugin_sentry-0.3.0/README.md
--rw-r--r--   0        0        0     1131 2023-04-14 09:29:05.547658 nonebot_plugin_sentry-0.3.0/__init__.py
--rw-r--r--   0        0        0     1071 2023-04-14 09:29:05.547658 nonebot_plugin_sentry-0.3.0/config.py
--rw-r--r--   0        0        0      844 2023-04-14 09:29:05.547658 nonebot_plugin_sentry-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 nonebot_plugin_sentry-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1413 2023-06-05 08:16:27.647737 nonebot_plugin_sentry-0.4.0/README.md
+-rw-r--r--   0        0        0     1544 2023-06-05 08:16:27.651737 nonebot_plugin_sentry-0.4.0/__init__.py
+-rw-r--r--   0        0        0     1071 2023-06-05 08:16:27.651737 nonebot_plugin_sentry-0.4.0/config.py
+-rw-r--r--   0        0        0      804 2023-06-05 08:16:27.651737 nonebot_plugin_sentry-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2453 1970-01-01 00:00:00.000000 nonebot_plugin_sentry-0.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_sentry-0.3.0/README.md` & `nonebot_plugin_sentry-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sentry-0.3.0/__init__.py` & `nonebot_plugin_sentry-0.4.0/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @Author         : yanyongyu
 @Date           : 2020-11-23 18:44:25
 @LastEditors    : yanyongyu
-@LastEditTime   : 2023-03-30 19:58:06
+@LastEditTime   : 2023-06-05 16:07:18
 @Description    : Sentry plugin
 @GitHub         : https://github.com/yanyongyu
 """
 __author__ = "yanyongyu"
 
 import sentry_sdk
 from nonebot import get_driver
 from nonebot.log import logger
+from nonebot.plugin import PluginMetadata
 from sentry_sdk.integrations.logging import EventHandler, BreadcrumbHandler
 
 from .config import Config
 
+__plugin_meta__ = PluginMetadata(
+    name="Sentry日志监控",
+    description="使用Sentry监控机器人日志并处理报错",
+    usage="在配置文件中填写Sentry DSN即可启用",
+    type="application",
+    homepage="https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry",
+    config=Config,
+    supported_adapters=None,
+)
+
 driver = get_driver()
 global_config = driver.config
 config = Config(**global_config.dict())
 
 
 def init_sentry(config: Config):
     sentry_config = {
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_sentry-0.3.0/config.py` & `nonebot_plugin_sentry-0.4.0/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sentry-0.3.0/pyproject.toml` & `nonebot_plugin_sentry-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-sentry"
-version = "0.3.0"
+version = "0.4.0"
 description = "Push your bot errors to Sentry.io"
 license = "MIT"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 readme = "README.md"
 homepage = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry"
 repository = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry"
 documentation = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry#readme"
@@ -12,14 +12,12 @@
 packages = [
     { include = "nonebot_plugin_sentry/*.py", from = ".." }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 sentry-sdk = "^1.0.0"
-nonebot2 = "^2.0.0-alpha.6"
-
-[tool.poetry.dev-dependencies]
+nonebot2 = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_sentry-0.3.0/PKG-INFO` & `nonebot_plugin_sentry-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sentry
-Version: 0.3.0
+Version: 0.4.0
 Summary: Push your bot errors to Sentry.io
 Home-page: https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry
 License: MIT
 Keywords: nonebot,nonebot2,sentry
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot2 (>=2.0.0-alpha.6,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: sentry-sdk (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry#readme
 Project-URL: Repository, https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry
 Description-Content-Type: text/markdown
 
 <!--
  * @Author         : yanyongyu
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sentry Version: 0.3.0 Summary: Push
+Metadata-Version: 2.1 Name: nonebot-plugin-sentry Version: 0.4.0 Summary: Push
 your bot errors to Sentry.io Home-page: https://github.com/cscs181/QQ-GitHub-
 Bot/tree/master/src/plugins/nonebot_plugin_sentry License: MIT Keywords:
 nonebot,nonebot2,sentry Author: yanyongyu Author-email: yyy@nonebot.dev
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot2 (>=2.0.0-alpha.6,<3.0.0) Requires-Dist: sentry-sdk
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: sentry-sdk
 (>=1.0.0,<2.0.0) Project-URL: Documentation, https://github.com/cscs181/QQ-
 GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry#readme Project-URL:
 Repository, https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/
 nonebot_plugin_sentry Description-Content-Type: text/markdown
                               [nonebot] [sentry]
          # nonebot-plugin-sentry _â¨ å¨ Sentry.io ä¸è¿è¡ NoneBot
                     æå¡æ¥å¿æ¥çãéè¯¯å¤ç â¨_
```

