# Comparing `tmp/nonebot_plugin_send_anything_anywhere-0.2.5.tar.gz` & `tmp/nonebot_plugin_send_anything_anywhere-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_send_anything_anywhere-0.2.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_send_anything_anywhere-0.2.6.tar", max compression
```

## Comparing `nonebot_plugin_send_anything_anywhere-0.2.5.tar` & `nonebot_plugin_send_anything_anywhere-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-06-05 14:06:16.499976 nonebot_plugin_send_anything_anywhere-0.2.5/LICENSE
--rw-r--r--   0        0        0     5946 2023-06-05 14:06:16.499976 nonebot_plugin_send_anything_anywhere-0.2.5/README.md
--rw-r--r--   0        0        0     1486 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/__init__.py
--rw-r--r--   0        0        0      181 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/__init__.py
--rw-r--r--   0        0        0     5355 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/kaiheila.py
--rw-r--r--   0        0        0     5537 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/onebot_v11.py
--rw-r--r--   0        0        0     8274 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/onebot_v12.py
--rw-r--r--   0        0        0     5923 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/qqguild.py
--rw-r--r--   0        0        0     5150 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/telegram.py
--rw-r--r--   0        0        0      189 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/types/__init__.py
--rw-r--r--   0        0        0     1972 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/types/common_message_segment.py
--rw-r--r--   0        0        0     1148 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/types/custom_message_segment.py
--rw-r--r--   0        0        0     1847 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/__init__.py
--rw-r--r--   0        0        0     2084 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/auto_select_bot.py
--rw-r--r--   0        0        0      673 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/const.py
--rw-r--r--   0        0        0      492 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/exceptions.py
--rw-r--r--   0        0        0      429 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/helpers.py
--rw-r--r--   0        0        0     6271 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/platform_send_target.py
--rw-r--r--   0        0        0    11997 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/types.py
--rw-r--r--   0        0        0     1756 2023-06-05 14:06:16.507976 nonebot_plugin_send_anything_anywhere-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.5/setup.py
--rw-r--r--   0        0        0     7047 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-05 19:00:20.542423 nonebot_plugin_send_anything_anywhere-0.2.6/LICENSE
+-rw-r--r--   0        0        0     5946 2023-06-05 19:00:20.546424 nonebot_plugin_send_anything_anywhere-0.2.6/README.md
+-rw-r--r--   0        0        0     1486 2023-06-05 19:00:20.546424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-05 19:00:20.546424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/__init__.py
+-rw-r--r--   0        0        0     5355 2023-06-05 19:00:20.546424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/kaiheila.py
+-rw-r--r--   0        0        0     5537 2023-06-05 19:00:20.546424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     8274 2023-06-05 19:00:20.546424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     5923 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/qqguild.py
+-rw-r--r--   0        0        0     5150 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/telegram.py
+-rw-r--r--   0        0        0      189 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/types/__init__.py
+-rw-r--r--   0        0        0     1972 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/types/common_message_segment.py
+-rw-r--r--   0        0        0     1148 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/types/custom_message_segment.py
+-rw-r--r--   0        0        0     1847 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/__init__.py
+-rw-r--r--   0        0        0     2084 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/auto_select_bot.py
+-rw-r--r--   0        0        0      707 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/const.py
+-rw-r--r--   0        0        0      492 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/exceptions.py
+-rw-r--r--   0        0        0      429 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/helpers.py
+-rw-r--r--   0        0        0     6271 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/platform_send_target.py
+-rw-r--r--   0        0        0    11997 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/types.py
+-rw-r--r--   0        0        0     1756 2023-06-05 19:00:20.550424 nonebot_plugin_send_anything_anywhere-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.6/setup.py
+-rw-r--r--   0        0        0     7047 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.6/PKG-INFO
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/LICENSE` & `nonebot_plugin_send_anything_anywhere-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/README.md` & `nonebot_plugin_send_anything_anywhere-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/__init__.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/kaiheila.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/onebot_v11.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/onebot_v12.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/qqguild.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/telegram.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/types/common_message_segment.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/types/common_message_segment.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/types/custom_message_segment.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/types/custom_message_segment.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/__init__.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/auto_select_bot.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/auto_select_bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/const.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 class SupportedAdapters(StrEnum):
     onebot_v11 = "OneBot V11"
     onebot_v12 = "OneBot V12"
     qqguild = "QQ Guild"
     kaiheila = "Kaiheila"
     telegram = "Telegram"
 
+    fake = "fake"  # for nonebug
+
 
 class SupportedPlatform(StrEnum):
     qq_group = "QQ Group"
     qq_private = "QQ Private"
     qq_guild_channel = "QQ Guild Channel"
     qq_guild_direct = "QQ Guild Direct"
     kaiheila_channel = "Kaiheila Channel"
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/platform_send_target.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/platform_send_target.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/types.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/nonebot_plugin_saa/utils/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/pyproject.toml` & `nonebot_plugin_send_anything_anywhere-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-send-anything-anywhere"
-version = "0.2.5"
+version = "0.2.6"
 description = "An adaptor for nonebot2 adaptors"
 authors = ["felinae98 <731499577@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_saa" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/setup.py` & `nonebot_plugin_send_anything_anywhere-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['anyio>=3.6.2,<4.0.0',
  'nonebot2>=2.0.0,<3.0.0',
  'pydantic>=1.10.5,<2.0.0',
  'strenum>=0.4.8,<0.5.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-send-anything-anywhere',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'An adaptor for nonebot2 adaptors',
     'long_description': '<div align="center">\n\n~logo征集中，假装有图片~\n\n# Nonebot Plugin<br>Send Anything Anywhere\n\n你只管业务实现，把发送交给我们\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/felinae98/nonebot-plugin-send-anything-anywhere/test.yml)\n![Codecov](https://img.shields.io/codecov/c/github/felinae98/nonebot-plugin-send-anything-anywhere)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nonebot-plugin-send-anything-anywhere)\n![PyPI](https://img.shields.io/pypi/v/nonebot-plugin-send-anything-anywhere)\n![GitHub](https://img.shields.io/github/license/felinae98/nonebot-plugin-send-anything-anywhere)\n\n</div>\n\n这个插件可以做什么\n\n- 为常见的消息类型提供抽象类，自适应转换成对应 adapter 的消息\n- 提供一套统一的，符合直觉的发送接口\n- 为复杂的消息提供易用的生成接口（规划中）\n\n本插件通过传入 bot 的类型来自适应生成对应 bot adapter 所使用的 Message\n\n## 安装\n\n- 使用 nb-cli 安装  \n  `nb plugin install nonebot-plugin-send-anything-anywhere`\n- 使用 poetry 安装  \n  `poetry add nonebot-plugin-send-anything-anywhere`\n- 使用 pip 安装  \n  `pip install nonebot-plugin-send-anything-anywhere`\n\n## 使用\n\n在 handler 中回复消息的情况：\n\n```python\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    # 直接调用 MessageFactory.send() 在 handler 中回复消息\n    await MessageFactory("你好").send(reply=True, at_sender=True)\n    await MessageFactory("需要回复的内容").send()\n    await matcher.finish()\n```\n\n主动发送的情况：\n\n```python\nfrom nonebot_plugin_saa import TargetQQGroup\n\n# 发送目标为 QQ 号 10000, 以私聊形式发送\ntarget = TargetQQGroup(group_id=2233)\nawait MessageFactory("早上好").send_to(target)\n```\n\n从消息事件中提取发送目标:\n\n```python\nfrom nonebot_plugin_saa import extract_target, get_target\n\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    target = extract_target(event)\n\n@matcher.handle()\nasync def handle(target: PlatformTarget = Depends(get_target)):\n    ...\n```\n\n发送目标的序列化与反序列化:\n\n```python\nfrom nonebot_plugin_saa import PlatformTarget, TargetQQPrivate\n\ntarget = TargetQQPrivate(user_id=112233)\nserialized_target = target.json()\ndeserialized_target = PlatformTarget.deserialize(serialized_target)\nassert deserialized_target == target\n```\n\n## 支持情况\n\n✅:支持 ✖️:支持不了 🚧:等待适配\n\n### 支持的 adapter\n\n| OneBot v11 | OneBot v12 | QQ Guild | Kaiheila |\n| :--------: | :--------: | :------: | :------: |\n|     ✅     |     ✅     |    ✅    |    ✅    |\n\n### 支持的消息类型\n\n|      | OneBot v11 | OneBot v12 | QQ Guild | 开黑啦 |\n| :--: | :--------: | :--------: | :------: | :----: |\n| 文字 |     ✅     |     ✅     |    ✅    |   ✅   |\n| 图片 |     ✅     |     ✅     |    ✅    |   ✅   |\n|  at  |     ✅     |     ✅     |    ✅    |   ✅   |\n| 回复 |     ✅     |     ✅     |    ✅    |   ✅   |\n\n### 支持的发送目标\n\n|                   | OneBot v11 | OneBot v12  | QQ Guild | Kaiheila |\n| :---------------: | :--------: | :---------: | :------: | :------: |\n|       QQ 群       |     ✅     |     ✅      |          |          |\n|      QQ 私聊      |     ✅     |     ✅      |          |          |\n| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |          |\n|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |          |\n|  开黑啦私聊/频道  |            |             |          |    ✅    |\n\n注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用\n\n## 问题与例子\n\n因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的\n\nbefore:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v11.message import MessageSegment as V11MessageSegment\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.adapters.onebot.v12.message import MessageSegment as V12MessageSegment\nfrom nonebot.adapters.onebot.v12.bot import Bot as V12Bot\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v11(event: V11MessageEvent):\n    pic_content = ...\n    msg = V11MessageSegment.image(pic_content) + V11MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n\npic_matcher.handle()\nasync def _handle_v12(bot: V12Bot, event: V12MessageEvent):\n    pic_content = ...\n    pic_file = await bot.upload_file(type=\'data\', name=\'image\', data=pic_content)\n    msg = V12MessageSegment.image(pic_file[\'file_id\']) + V12MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n```\n\n现在只需要:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.internal.adapter.bot import Bot\nfrom nonebot_plugin_saa import Image, Text, MessageFactory\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v12(bot: Bot, event: Union[V12MessageEvent, V11MessageEvent]):\n    pic_content = ...\n    msg_builder = MessageFactory([\n        Image(pic_content), Text("这是你要的图片")\n    ])\n    # or msg_builder = Image(pic_content) + Text("这是你要的图片")\n    await msg_builder.send()\n    await pic_matcher.finish()\n```\n\n## 类似项目\n\n- [nonebot-plugin-all4one](https://github.com/nonepkg/nonebot-plugin-all4one) 解决了类似的问题，但是用了不同路径\n- [nonebot-plugin-params](https://github.com/iyume/nonebot-plugin-params) 通过 Rule 定制订阅的平台，与本插件联合使用也许会有奇效\n\n## License\n\nMIT\n',
     'author': 'felinae98',
     'author_email': '731499577@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.5/PKG-INFO` & `nonebot_plugin_send_anything_anywhere-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-send-anything-anywhere
-Version: 0.2.5
+Version: 0.2.6
 Summary: An adaptor for nonebot2 adaptors
 License: MIT
 Author: felinae98
 Author-email: 731499577@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

