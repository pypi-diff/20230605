# Comparing `tmp/nonebot_plugin_genshin_cos-0.1.7.tar.gz` & `tmp/nonebot_plugin_genshin_cos-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshin_cos-0.1.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshin_cos-0.1.8.tar", max compression
```

## Comparing `nonebot_plugin_genshin_cos-0.1.7.tar` & `nonebot_plugin_genshin_cos-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1085 2023-03-28 09:06:05.557316 nonebot_plugin_genshin_cos-0.1.7/LICENSE
--rw-r--r--   0        0        0     8860 2023-05-07 00:52:02.221268 nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/__init__.py
--rw-r--r--   0        0        0      269 2023-04-27 05:00:12.292105 nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/config.py
--rw-r--r--   0        0        0   459180 2023-04-08 07:01:06.461588 nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
--rw-r--r--   0        0        0    11068 2023-05-07 00:51:33.291947 nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/utils.py
--rw-r--r--   0        0        0      661 2023-05-07 00:52:27.173270 nonebot_plugin_genshin_cos-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3634 2023-04-27 05:19:54.659437 nonebot_plugin_genshin_cos-0.1.7/README.md
--rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-03-28 09:06:05.557316 nonebot_plugin_genshin_cos-0.1.8/LICENSE
+-rw-r--r--   0        0        0     8905 2023-06-05 05:33:05.302878 nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-05 05:24:06.712318 nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/config.py
+-rw-r--r--   0        0        0   459180 2023-06-05 05:24:06.718316 nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
+-rw-r--r--   0        0        0    11068 2023-06-05 05:24:06.719317 nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/utils.py
+-rw-r--r--   0        0        0      661 2023-06-05 05:38:03.920857 nonebot_plugin_genshin_cos-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3636 2023-06-05 05:24:06.711314 nonebot_plugin_genshin_cos-0.1.8/README.md
+-rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_genshin_cos-0.1.7/LICENSE` & `nonebot_plugin_genshin_cos-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/__init__.py` & `nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from nonebot.adapters.onebot.v11 import MessageSegment, MessageEvent, Bot, Message, GroupMessageEvent
 from nonebot.plugin import on_regex, PluginMetadata
 from nonebot.permission import SUPERUSER
-from nonebot.params import Arg
+from nonebot.params import Arg, RegexGroup
 from nonebot.exception import ActionFailed
 from nonebot.typing import T_State
 from nonebot import get_driver
 from .utils import get_cos, WriteError, check_cd, GetGenShinCos, log
 from nonebot.log import logger
+from typing import Tuple, Any
 from .config import Config
 from re import I
 import re
 from datetime import datetime, timedelta
 
 __plugin_meta__ = PluginMetadata(
     name="米游社cos",
@@ -149,17 +150,17 @@
             await download_cos.finish(f"出错了:<{exc}>")
 
 
 max = Config.parse_obj(get_driver().config.dict()).cos_max
 
 
 @send_cos.handle()
-async def handle(bot: Bot, event: MessageEvent, state: T_State):
+async def handle(bot: Bot, event: MessageEvent, args: Tuple[Any, ...] = RegexGroup()):
     global user_data
-    args = list(state['_matched_groups'])
+    args = list(args)
     img = get_cos()
     out_cd, deletime, user_data = check_cd(event.user_id, user_data)
     if out_cd:
         if not args[2]:
             await send_cos.send("获取图片中…请稍等")
             if not await img.randow_cos_img():
                 await send_cos.finish("未获取到图片")
```

### Comparing `nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF` & `nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/utils.py` & `nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.7/pyproject.toml` & `nonebot_plugin_genshin_cos-0.1.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-genshin-cos"
-version = "0.1.7"
+version = "0.1.8"
 description = "米游社原神cos图获取"
 authors = ["Cvandia <106718176+Cvandia@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_genshin_cos"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_genshin_cos-0.1.7/README.md` & `nonebot_plugin_genshin_cos-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 ### 指令：
 | 指令 | 需要@ | 范围 | 说明 |权限|
 |:-----:|:----:|:----:|:----:|:----:|
 |原神cos|否|私聊、群聊|随机发送x张cos图，如：米游社cos x3|任何|
 |下载cos|否|私聊、群聊|爬取cos图片至本地,如：下载cos|超管|
 |cosplus|否|私聊、群聊|通过playwright获取cos图|任何|
 |xmx|否|私聊、群聊|？？？？？s|超管|
+
 **注意**
 
 指令触发方式是正则匹配的，不需要加指令前缀
 
 ## 🌙 未来
  - [x] 缓慢更新，最近学业繁忙哦~
  - [x] 随机发送cos图片
```

### Comparing `nonebot_plugin_genshin_cos-0.1.7/PKG-INFO` & `nonebot_plugin_genshin_cos-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshin-cos
-Version: 0.1.7
+Version: 0.1.8
 Summary: 米游社原神cos图获取
 License: MIT
 Author: Cvandia
 Author-email: 106718176+Cvandia@users.noreply.github.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -117,14 +117,15 @@
 ### 指令：
 | 指令 | 需要@ | 范围 | 说明 |权限|
 |:-----:|:----:|:----:|:----:|:----:|
 |原神cos|否|私聊、群聊|随机发送x张cos图，如：米游社cos x3|任何|
 |下载cos|否|私聊、群聊|爬取cos图片至本地,如：下载cos|超管|
 |cosplus|否|私聊、群聊|通过playwright获取cos图|任何|
 |xmx|否|私聊、群聊|？？？？？s|超管|
+
 **注意**
 
 指令触发方式是正则匹配的，不需要加指令前缀
 
 ## 🌙 未来
  - [x] 缓慢更新，最近学业繁忙哦~
  - [x] 随机发送cos图片
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.1.8 Summary:
 ç±³æ¸¸ç¤¾åç¥coså¾è·å License: MIT Author: Cvandia Author-email:
 106718176+Cvandia@users.noreply.github.com Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0) Requires-Dist: httpx (>=0.19.0) Requires-
```

