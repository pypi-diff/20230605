# Comparing `tmp/nonebot-plugin-imgexploration-0.3.1.tar.gz` & `tmp/nonebot-plugin-imgexploration-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-imgexploration-0.3.1.tar", last modified: Fri May 19 04:37:04 2023, max compression
+gzip compressed data, was "nonebot-plugin-imgexploration-0.3.2.tar", last modified: Mon Jun  5 11:01:22 2023, max compression
```

## Comparing `nonebot-plugin-imgexploration-0.3.1.tar` & `nonebot-plugin-imgexploration-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 04:37:04.397222 nonebot-plugin-imgexploration-0.3.1/
--rw-rw-rw-   0        0        0     1088 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0      166 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2894 2023-05-19 04:37:04.396222 nonebot-plugin-imgexploration-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2141 2023-05-19 03:39:31.000000 nonebot-plugin-imgexploration-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 04:37:04.387222 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration/
--rw-rw-rw-   0        0        0     4314 2023-05-19 03:39:52.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration/__init__.py
--rw-rw-rw-   0        0        0    20816 2023-05-19 04:33:54.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration/imgexploration.py
-drwxrwxrwx   0        0        0        0 2023-05-19 04:37:04.394223 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/
--rw-rw-rw-   0        0        0     2894 2023-05-19 04:37:04.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-05-19 04:37:04.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 04:37:04.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-05-19 04:37:04.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-05-19 04:37:04.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      613 2023-05-19 04:36:57.000000 nonebot-plugin-imgexploration-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 04:37:04.397222 nonebot-plugin-imgexploration-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     8696 2023-05-19 04:36:57.000000 nonebot-plugin-imgexploration-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:01:22.874954 nonebot-plugin-imgexploration-0.3.2/
+-rw-rw-rw-   0        0        0     1088 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      166 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2894 2023-06-05 11:01:22.874954 nonebot-plugin-imgexploration-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2141 2023-05-19 03:39:31.000000 nonebot-plugin-imgexploration-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 11:01:22.865773 nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration/
+-rw-rw-rw-   0        0        0     4363 2023-06-05 11:00:54.000000 nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration/__init__.py
+-rw-rw-rw-   0        0        0    20816 2023-05-19 04:33:54.000000 nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration/imgexploration.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:01:22.872772 nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration.egg-info/
+-rw-rw-rw-   0        0        0     2894 2023-06-05 11:01:22.000000 nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-06-05 11:01:22.000000 nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 11:01:22.000000 nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-06-05 11:01:22.000000 nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-06-05 11:01:22.000000 nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      613 2023-06-05 10:59:51.000000 nonebot-plugin-imgexploration-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 11:01:22.875955 nonebot-plugin-imgexploration-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     8696 2023-06-05 10:59:51.000000 nonebot-plugin-imgexploration-0.3.2/setup.py
```

### Comparing `nonebot-plugin-imgexploration-0.3.1/LICENSE.txt` & `nonebot-plugin-imgexploration-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-imgexploration-0.3.1/PKG-INFO` & `nonebot-plugin-imgexploration-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-imgexploration
-Version: 0.3.1
+Version: 0.3.2
 Summary: Nonebot2 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图
 Home-page: https://github.com/cpuopt/nonebot_plugin_imgexploration
 Author: cpufan
 Author-email: cpufan2001@gmail.com
 Keywords: nonebot nonebot-plugin imagesearch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.3.1
+Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.3.2
 Summary: Nonebot2
 æä»¶ï¼GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ Home-
 page: https://github.com/cpuopt/nonebot_plugin_imgexploration Author: cpufan
 Author-email: cpufan2001@gmail.com Keywords: nonebot nonebot-plugin imagesearch
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `nonebot-plugin-imgexploration-0.3.1/README.md` & `nonebot-plugin-imgexploration-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration/__init__.py` & `nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import nonebot
 import httpx
 from typing import Union
-from nonebot import on_command
+from nonebot import on_command,require
 from nonebot.log import logger
 from nonebot.typing import T_State
 from nonebot.params import Arg, CommandArg
+from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import Bot, Message, MessageSegment, GroupMessageEvent, PrivateMessageEvent
+require("nonebot_plugin_guild_patch")
 from nonebot_plugin_guild_patch import GuildMessageEvent
 from .imgexploration import Imgexploration
-from nonebot.plugin import PluginMetadata
+
 
 __plugin_meta__ = PluginMetadata(name="查找图片出处", description="通过saucenao、ascii2d、Google、Yandx查询图片出处", usage="command:搜图")
 
 proxy_port = getattr(nonebot.get_driver().config, "proxy_port", None)
 saucenao_apikey = getattr(nonebot.get_driver().config, "saucenao_apikey", "a778025bd4644780c9edd82970484548786fb583")
 google_cookies = getattr(nonebot.get_driver().config, "google_cookies","")
```

### Comparing `nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration/imgexploration.py` & `nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration/imgexploration.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/PKG-INFO` & `nonebot-plugin-imgexploration-0.3.2/nonebot_plugin_imgexploration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-imgexploration
-Version: 0.3.1
+Version: 0.3.2
 Summary: Nonebot2 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图
 Home-page: https://github.com/cpuopt/nonebot_plugin_imgexploration
 Author: cpufan
 Author-email: cpufan2001@gmail.com
 Keywords: nonebot nonebot-plugin imagesearch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.3.1
+Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.3.2
 Summary: Nonebot2
 æä»¶ï¼GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ Home-
 page: https://github.com/cpuopt/nonebot_plugin_imgexploration Author: cpufan
 Author-email: cpufan2001@gmail.com Keywords: nonebot nonebot-plugin imagesearch
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `nonebot-plugin-imgexploration-0.3.1/pyproject.toml` & `nonebot-plugin-imgexploration-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-imgexploration"
-version = "0.3.1"
+version = "0.3.2"
 description = "Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图"
 authors = ["cpufan"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_imgexploration"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot-plugin-imgexploration-0.3.1/setup.py` & `nonebot-plugin-imgexploration-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
     # Required
-    version="0.3.1",
+    version="0.3.2",
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     # Optional
     description="Nonebot2 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图",
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
```

