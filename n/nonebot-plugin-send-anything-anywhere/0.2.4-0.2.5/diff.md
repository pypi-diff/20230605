# Comparing `tmp/nonebot_plugin_send_anything_anywhere-0.2.4.tar.gz` & `tmp/nonebot_plugin_send_anything_anywhere-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_send_anything_anywhere-0.2.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_send_anything_anywhere-0.2.5.tar", max compression
```

## Comparing `nonebot_plugin_send_anything_anywhere-0.2.4.tar` & `nonebot_plugin_send_anything_anywhere-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/LICENSE
--rw-r--r--   0        0        0     5946 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/README.md
--rw-r--r--   0        0        0      929 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/__init__.py
--rw-r--r--   0        0        0       70 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/__init__.py
--rw-r--r--   0        0        0     5355 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/kaiheila.py
--rw-r--r--   0        0        0     5537 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/onebot_v11.py
--rw-r--r--   0        0        0     8274 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/onebot_v12.py
--rw-r--r--   0        0        0     5923 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/qqguild.py
--rw-r--r--   0        0        0      189 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/types/__init__.py
--rw-r--r--   0        0        0     1955 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/types/common_message_segment.py
--rw-r--r--   0        0        0     1148 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/types/custom_message_segment.py
--rw-r--r--   0        0        0     1741 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/__init__.py
--rw-r--r--   0        0        0     2093 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/auto_select_bot.py
--rw-r--r--   0        0        0      553 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/const.py
--rw-r--r--   0        0        0      449 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/exceptions.py
--rw-r--r--   0        0        0      429 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/helpers.py
--rw-r--r--   0        0        0     5586 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/platform_send_target.py
--rw-r--r--   0        0        0    11545 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/types.py
--rw-r--r--   0        0        0     1703 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6929 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.4/setup.py
--rw-r--r--   0        0        0     7012 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-05 14:06:16.499976 nonebot_plugin_send_anything_anywhere-0.2.5/LICENSE
+-rw-r--r--   0        0        0     5946 2023-06-05 14:06:16.499976 nonebot_plugin_send_anything_anywhere-0.2.5/README.md
+-rw-r--r--   0        0        0     1486 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/__init__.py
+-rw-r--r--   0        0        0     5355 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/kaiheila.py
+-rw-r--r--   0        0        0     5537 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     8274 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     5923 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/qqguild.py
+-rw-r--r--   0        0        0     5150 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/telegram.py
+-rw-r--r--   0        0        0      189 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/types/__init__.py
+-rw-r--r--   0        0        0     1972 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/types/common_message_segment.py
+-rw-r--r--   0        0        0     1148 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/types/custom_message_segment.py
+-rw-r--r--   0        0        0     1847 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/__init__.py
+-rw-r--r--   0        0        0     2084 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/auto_select_bot.py
+-rw-r--r--   0        0        0      673 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/const.py
+-rw-r--r--   0        0        0      492 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/exceptions.py
+-rw-r--r--   0        0        0      429 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/helpers.py
+-rw-r--r--   0        0        0     6271 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/platform_send_target.py
+-rw-r--r--   0        0        0    11997 2023-06-05 14:06:16.503976 nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/types.py
+-rw-r--r--   0        0        0     1756 2023-06-05 14:06:16.507976 nonebot_plugin_send_anything_anywhere-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.5/setup.py
+-rw-r--r--   0        0        0     7047 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.5/PKG-INFO
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/LICENSE` & `nonebot_plugin_send_anything_anywhere-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/README.md` & `nonebot_plugin_send_anything_anywhere-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/kaiheila.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/onebot_v11.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/onebot_v11.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             full_msg = msg
         message_to_send = Message()
         for message_segment_factory in full_msg:
             message_segment = await message_segment_factory.build(bot)
             message_to_send += message_segment
         await bot.send_msg(message=message_to_send, **target.arg_dict(bot))
 
-    @AggregatedMessageFactory.register_aggragated_sender(adapter)
+    @AggregatedMessageFactory.register_aggregated_sender(adapter)
     async def aggregate_send(
         bot: Bot,
         message_factories: List[MessageFactory],
         target: PlatformTarget,
         event: Optional[Event],
     ):
         assert isinstance(bot, BotOB11)
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/onebot_v12.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/qqguild.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/types/common_message_segment.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/types/common_message_segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 
 class Image(MessageSegmentFactory):
     """图片消息段"""
 
     data: ImageData
 
     def __init__(
-        self, image: Union[str, bytes, Path, BytesIO], name: str = "image"
+        self,
+        image: Union[str, bytes, Path, BytesIO],
+        name: str = "image",
     ) -> None:
         """图片消息段
 
         支持多种格式的数据
 
         参数:
             image: str 为图片 URL，bytes 为图片数据，Path 为图片路径，BytesIO 为图片文件流
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/types/custom_message_segment.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/types/custom_message_segment.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/__init__.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 )
 from .platform_send_target import (
     TargetQQGroup,
     PlatformTarget,
     TargetQQPrivate,
     TargetOB12Unknow,
     TargetQQGuildDirect,
+    TargetTelegramForum,
     TargetQQGuildChannel,
+    TargetTelegramCommon,
     TargetKaiheilaChannel,
     TargetKaiheilaPrivate,
     AllSupportedPlatformTarget,
     get_target,
     extract_target,
     register_sender,
     register_convert_to_arg,
@@ -56,12 +58,14 @@
     "TargetQQGroup",
     "TargetQQPrivate",
     "TargetQQGuildChannel",
     "TargetQQGuildDirect",
     "TargetKaiheilaChannel",
     "TargetKaiheilaPrivate",
     "TargetOB12Unknow",
+    "TargetTelegramCommon",
+    "TargetTelegramForum",
     "AllSupportedPlatformTarget",
     "auto_select_bot",
     "register_list_targets",
     "enable_auto_select_bot",
 ]
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/auto_select_bot.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/auto_select_bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import random
 from collections import defaultdict
 from typing import Dict, List, Callable, Awaitable
 
 from nonebot import get_bots
 from nonebot.adapters import Bot
 
+from .exceptions import NoBotFound
 from .const import SupportedAdapters
 from .helpers import extract_adapter_type
 from .platform_send_target import PlatformTarget, TargetQQGuildDirect
 
 BOT_CACHE: Dict[PlatformTarget, List[Bot]] = defaultdict(list)
 
 ListTargetsFunc = Callable[[Bot], Awaitable[List[PlatformTarget]]]
@@ -70,10 +71,10 @@
 
     # TODO: 通过更方便的方式判断当前 Target 是否支持
     if isinstance(target, TargetQQGuildDirect):
         raise NotImplementedError("暂不支持私聊")
 
     bots = BOT_CACHE.get(target)
     if not bots:
-        raise RuntimeError("无法获取到发送目标对应的 bot")
+        raise NoBotFound()
 
     return random.choice(bots)
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/platform_send_target.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/platform_send_target.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 import json
 from abc import ABC
-from typing_extensions import Self
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Type,
     Tuple,
     Union,
     Literal,
     Callable,
     ClassVar,
     Optional,
     Awaitable,
+    cast,
 )
 
 from pydantic import BaseModel
 from nonebot.adapters import Bot, Event
 
 from .helpers import extract_adapter_type
 from .const import SupportedAdapters, SupportedPlatform
 
 if TYPE_CHECKING:
     from .types import MessageFactory
 
 
 class PlatformTarget(BaseModel, ABC):
-    _deseriazer_map: ClassVar[Dict[SupportedPlatform, Type["PlatformTarget"]]] = {}
+    _deseriazer_map: ClassVar[
+        Dict[SupportedPlatform, Type["AllSupportedPlatformTarget"]]
+    ] = {}
     platform_type: SupportedPlatform
 
     class Config:
         frozen = True
         orm_mode = True
 
     def __init_subclass__(cls) -> None:
         assert isinstance(cls.__fields__["platform_type"].default, SupportedPlatform)
+        cls = cast(Type["AllSupportedPlatformTarget"], cls)
         cls._deseriazer_map[cls.__fields__["platform_type"].default] = cls
         return super().__init_subclass__()
 
     def arg_dict(self, bot: Bot):
         adapter_type = extract_adapter_type(bot)
         if (self.platform_type, adapter_type) not in convert_to_arg_map.keys():
             raise RuntimeError(
-                f"PlatformTarget {self.platform_type} not support {adapter_type}"
+                f"PlatformTarget {self.platform_type} not support {adapter_type}",
             )
         return convert_to_arg_map[(self.platform_type, adapter_type)](self)
 
     @classmethod
-    def deserialize(cls, source: Union[str, dict]) -> Self:
+    def deserialize(cls, source: Any) -> "AllSupportedPlatformTarget":
         if isinstance(source, str):
             raw_obj = json.loads(source)
         else:
             raw_obj = source
             assert raw_obj.get("platform_type")
         platform_type = SupportedPlatform(raw_obj["platform_type"])
         return cls._deseriazer_map[platform_type].parse_obj(raw_obj)
@@ -147,23 +150,53 @@
 
     platform_type: Literal[
         SupportedPlatform.kaiheila_private
     ] = SupportedPlatform.kaiheila_private
     user_id: str
 
 
+class TargetTelegramCommon(PlatformTarget):
+    """Telegram 普通对话
+
+    参数
+        user_id: 对话ID
+    """
+
+    platform_type: Literal[
+        SupportedPlatform.telegram_common
+    ] = SupportedPlatform.telegram_common
+    chat_id: Union[int, str]
+
+
+class TargetTelegramForum(PlatformTarget):
+    """Telegram 频道
+
+    参数
+        chat_id: 频道ID
+        message_thread_id: 板块ID
+    """
+
+    platform_type: Literal[
+        SupportedPlatform.telegram_forum
+    ] = SupportedPlatform.telegram_forum
+    chat_id: int
+    message_thread_id: int
+
+
 # this union type is for deserialize pydantic model with nested PlatformTarget
 AllSupportedPlatformTarget = Union[
     TargetQQGroup,
     TargetQQPrivate,
     TargetQQGuildChannel,
     TargetQQGuildDirect,
     TargetKaiheilaPrivate,
     TargetKaiheilaChannel,
     TargetOB12Unknow,
+    TargetTelegramCommon,
+    TargetTelegramForum,
 ]
 
 
 ConvertToArg = Callable[[PlatformTarget], Dict[str, Any]]
 convert_to_arg_map: Dict[Tuple[SupportedPlatform, SupportedAdapters], ConvertToArg] = {}
 
 
@@ -186,15 +219,15 @@
 
     return wrapper
 
 
 def extract_target(event: Event) -> PlatformTarget:
     "从事件中提取出发送目标，如果不能提取就抛出错误"
     for event_type in event.__class__.mro():
-        if event_type in extractor_map.keys():
+        if event_type in extractor_map:
             if not issubclass(event_type, Event):
                 break
             return extractor_map[event_type](event)
     raise RuntimeError(f"event {event.__class__} not supported")
 
 
 def get_target(event: Event) -> Optional[PlatformTarget]:
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/types.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/nonebot_plugin_saa/utils/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,21 @@
     List,
     Type,
     Union,
     TypeVar,
     Callable,
     ClassVar,
     Iterable,
+    NoReturn,
     Optional,
     Awaitable,
     cast,
 )
 
+from nonebot.exception import FinishedException
 from nonebot.matcher import current_bot, current_event
 from nonebot.adapters import Bot, Event, Message, MessageSegment
 
 from .auto_select_bot import get_bot
 from .const import SupportedAdapters
 from .helpers import extract_adapter_type
 from .exceptions import FallbackToDefault, AdapterNotInstalled
@@ -36,15 +38,17 @@
 CustomBuildFunc = Union[
     Callable[[], Union[MessageSegment, Awaitable[MessageSegment]]],
     Callable[[Bot], Union[MessageSegment, Awaitable[MessageSegment]]],
 ]
 
 
 async def do_build(
-    msf: "MessageSegmentFactory", builder: BuildFunc, bot: Bot
+    msf: "MessageSegmentFactory",
+    builder: BuildFunc,
+    bot: Bot,
 ) -> MessageSegment:
     if len(signature(builder).parameters) == 1:
         builder = cast(
             Callable[
                 ["MessageSegmentFactory"],
                 Union[MessageSegment, Awaitable[MessageSegment]],
             ],
@@ -57,20 +61,18 @@
                 ["MessageSegmentFactory", Bot],
                 Union[MessageSegment, Awaitable[MessageSegment]],
             ],
             builder,
         )
         res = builder(msf, bot)
     else:
-        raise RuntimeError()
+        raise RuntimeError
     if asyncio.iscoroutine(res):
         return await res
-    else:
-        res = cast(MessageSegment, res)
-        return res
+    return cast(MessageSegment, res)
 
 
 async def do_build_custom(builder: CustomBuildFunc, bot: Bot) -> MessageSegment:
     if len(signature(builder).parameters) == 0:
         builder = cast(
             Callable[[], Union[MessageSegment, Awaitable[MessageSegment]]],
             builder,
@@ -79,20 +81,18 @@
     elif len(signature(builder).parameters) == 1:
         builder = cast(
             Callable[[Bot], Union[MessageSegment, Awaitable[MessageSegment]]],
             builder,
         )
         res = builder(bot)
     else:
-        raise RuntimeError()
+        raise RuntimeError
     if asyncio.iscoroutine(res):
         return await res
-    else:
-        res = cast(MessageSegment, res)
-        return res
+    return cast(MessageSegment, res)
 
 
 class MessageSegmentFactory(ABC):
     _builders: ClassVar[
         Dict[
             SupportedAdapters,
             Union[
@@ -102,38 +102,43 @@
         ]
     ]
 
     data: dict
     _custom_builders: Dict[SupportedAdapters, CustomBuildFunc]
 
     def _register_custom_builder(
-        self, adapter: SupportedAdapters, ms: Union[MessageSegment, CustomBuildFunc]
+        self,
+        adapter: SupportedAdapters,
+        ms: Union[MessageSegment, CustomBuildFunc],
     ):
         if isinstance(ms, MessageSegment):
             self._custom_builders[adapter] = lambda _: ms
         else:
             self._custom_builders[adapter] = ms
 
     def _get_custom_builder(
-        self, adapter: SupportedAdapters
+        self,
+        adapter: SupportedAdapters,
     ) -> Optional[CustomBuildFunc]:
         return self._custom_builders.get(adapter)
 
     def __init__(self) -> None:
         self._custom_builders = {}
 
     def __init_subclass__(cls) -> None:
         cls._builders = {}
         return super().__init_subclass__()
 
     def __eq__(self, other: Self) -> bool:
         return self.data == other.data
 
     def overwrite(
-        self, adapter: SupportedAdapters, ms: Union[MessageSegment, CustomBuildFunc]
+        self,
+        adapter: SupportedAdapters,
+        ms: Union[MessageSegment, CustomBuildFunc],
     ) -> Self:
         "为某个 adapter 重写产生的 MessageSegment 或重写产生 MessageSegment 的方法"
         self._register_custom_builder(adapter, ms)
         return self
 
     async def build(self, bot: Bot) -> MessageSegment:
         adapter_name = extract_adapter_type(bot)
@@ -161,37 +166,40 @@
 
     @classmethod
     def get_text_factory(cls):
         return cls._text_factory
 
     @classmethod
     def register_adapter_message(
-        cls, adapter: SupportedAdapters, message_class: Type[Message]
+        cls,
+        adapter: SupportedAdapters,
+        message_class: Type[Message],
     ):
         cls._message_registry[adapter] = message_class
 
     async def build(self, bot: Bot) -> Message:
         warn(DeprecationWarning("MessageFactory.build is deprecated"))
         return await self._build(bot)
 
     async def _build(self, bot: Bot) -> Message:
         adapter_name = extract_adapter_type(bot)
         if message_type := self._message_registry.get(adapter_name):
             ms: List[MessageSegment] = await asyncio.gather(
-                *[ms_factory.build(bot) for ms_factory in self]
+                *[ms_factory.build(bot) for ms_factory in self],
             )
             return message_type(ms)
         raise AdapterNotInstalled(adapter_name)
 
     def __init__(self, message: Union[str, Iterable[TMSF], TMSF]):
         super().__init__()
 
         if message is None:
             return
-        elif isinstance(message, str):
+
+        if isinstance(message, str):
             self.append(self.get_text_factory()(message))
         elif isinstance(message, MessageSegmentFactory):
             self.append(message)
         elif isinstance(message, Iterable):
             self.extend(message)
 
     def __add__(self: TMF, other: Union[str, TMSF, Iterable[TMSF]]) -> TMF:
@@ -227,24 +235,29 @@
 
         return self
 
     def copy(self: TMF) -> TMF:
         return deepcopy(self)
 
     async def send(self, *, at_sender=False, reply=False):
-        "回复消息，仅能用在事件相应器中"
+        "回复消息，仅能用在事件响应器中"
         try:
             event = current_event.get()
             bot = current_bot.get()
-        except LookupError:
-            raise RuntimeError("send() 仅能在事件相应器中使用，主动发送消息请使用 send_to")
+        except LookupError as e:
+            raise RuntimeError("send() 仅能在事件响应器中使用，主动发送消息请使用 send_to") from e
 
         target = extract_target(event)
         await self._do_send(bot, target, event, at_sender, reply)
 
+    async def finish(self, *, at_sender=False, reply=False, **kwargs) -> NoReturn:
+        """与 `matcher.finish()` 作用相同，仅能用在事件响应器中"""
+        await self.send(at_sender=at_sender, reply=reply, **kwargs)
+        raise FinishedException
+
     async def send_to(self, target: PlatformTarget, bot: Optional[Bot] = None):
         if bot is None:
             bot = get_bot(target)
         await self._do_send(bot, target, None, False, False)
 
     async def _do_send(
         self,
@@ -253,87 +266,94 @@
         event: Optional[Event],
         at_sender: bool,
         reply: bool,
     ):
         adapter = extract_adapter_type(bot)
         if not (sender := sender_map[adapter]):
             raise RuntimeError(
-                f"send method for {adapter} not registerd"
+                f"send method for {adapter} not registered",
             )  # pragma: no cover
         await sender(bot, self, target, event, at_sender, reply)
 
 
 AggregatedSender = Callable[
-    [Bot, List[MessageFactory], PlatformTarget, Optional[Event]], Awaitable[None]
+    [Bot, List[MessageFactory], PlatformTarget, Optional[Event]],
+    Awaitable[None],
 ]
 
 
 class AggregatedMessageFactory:
     message_factories: List[MessageFactory]
     sender: ClassVar[Dict[SupportedAdapters, AggregatedSender]] = {}
 
     def __init__(
-        self, msgs: List[Union[MessageFactory, MessageSegmentFactory]]
+        self,
+        msgs: List[Union[MessageFactory, MessageSegmentFactory]],
     ) -> None:
         self.message_factories = []
         for msg in msgs:
             if isinstance(msg, MessageSegmentFactory):
                 self.message_factories.append(MessageFactory(msg))
             else:
                 self.message_factories.append(msg)
 
     def __eq__(self, other: Self):
         return self.message_factories == other.message_factories
 
     @classmethod
-    def register_aggragated_sender(cls, adapter: SupportedAdapters):
+    def register_aggregated_sender(cls, adapter: SupportedAdapters):
         def wrapper(func: AggregatedSender):
             cls.sender[adapter] = func
             return func
 
         return wrapper
 
     async def _send_aggregated_message_default(
-        self, bot: Bot, target: PlatformTarget, event: Optional[Event]
+        self,
+        bot: Bot,
+        target: PlatformTarget,
+        event: Optional[Event],
     ):
         for msg_fac in self.message_factories:
-            await msg_fac._do_send(bot, target, event, False, False)
+            await msg_fac._do_send(bot, target, event, False, False)  # noqa: SLF001
 
     async def _do_send(self, bot: Bot, target: PlatformTarget, event: Optional[Event]):
         adapter = extract_adapter_type(bot)
         if sender := self.__class__.sender.get(adapter):  # custom aggregate sender
             try:
                 return await sender(bot, self.message_factories, target, event)
             except FallbackToDefault:
                 await self._send_aggregated_message_default(bot, target, event)
         # fallback
         await self._send_aggregated_message_default(bot, target, event)
+        return None
 
     async def send(self):
-        "回复消息，仅能用在事件相应器中"
+        "回复消息，仅能用在事件响应器中"
         try:
             event = current_event.get()
             bot = current_bot.get()
-        except LookupError:
-            raise RuntimeError("send() 仅能在事件相应器中使用，主动发送消息请使用 send_to")
+        except LookupError as e:
+            raise RuntimeError("send() 仅能在事件响应器中使用，主动发送消息请使用 send_to") from e
 
         target = extract_target(event)
         await self._do_send(bot, target, event)
 
     async def send_to(self, target: PlatformTarget, bot: Optional[Bot] = None):
         if bot is None:
             bot = get_bot(target)
         await self._do_send(bot, target, None)
 
 
 def register_ms_adapter(
-    adapter: SupportedAdapters, ms_factory: Type[TMSF]
+    adapter: SupportedAdapters,
+    ms_factory: Type[TMSF],
 ) -> Callable[[BuildFunc], BuildFunc]:
     def decorator(builder: BuildFunc) -> BuildFunc:
-        ms_factory._builders[adapter] = builder
+        ms_factory._builders[adapter] = builder  # noqa: SLF001
         return builder
 
     return decorator
 
 
 def assamble_message_factory(
     origin_msg_factory: MessageFactory,
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/pyproject.toml` & `nonebot_plugin_send_anything_anywhere-0.2.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-send-anything-anywhere"
-version = "0.2.4"
+version = "0.2.5"
 description = "An adaptor for nonebot2 adaptors"
 authors = ["felinae98 <731499577@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_saa" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -16,17 +16,18 @@
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = "^2.0.0rc1"
+nonebot2 = "^2.0.0"
 strenum = "^0.4.8"
 pydantic = "^1.10.5"
+anyio = "^3.6.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.20.2"
 ipdb = "^0.13.9"
 pip = "^23.0"
 pytest-cov = "^4.0.0"
 nonebug = "^0.3.1"
@@ -37,14 +38,15 @@
 [tool.poetry.group.adapters]
 optional = true
 
 [tool.poetry.group.adapters.dependencies]
 nonebot-adapter-onebot = "^2.2.2"
 nonebot-adapter-qqguild = ">=0.2.1"
 nonebot-adapter-kaiheila = { version = "^0.2.4", python = ">=3.9" }
+nonebot-adapter-telegram = "^0.1.0b12"
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310"]
 include = '\.pyi?$'
 extend-exclude = '''
 '''
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/setup.py` & `nonebot_plugin_send_anything_anywhere-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,22 @@
  'nonebot_plugin_saa.types',
  'nonebot_plugin_saa.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['nonebot2>=2.0.0rc1,<3.0.0',
+['anyio>=3.6.2,<4.0.0',
+ 'nonebot2>=2.0.0,<3.0.0',
  'pydantic>=1.10.5,<2.0.0',
  'strenum>=0.4.8,<0.5.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-send-anything-anywhere',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'An adaptor for nonebot2 adaptors',
     'long_description': '<div align="center">\n\n~logo征集中，假装有图片~\n\n# Nonebot Plugin<br>Send Anything Anywhere\n\n你只管业务实现，把发送交给我们\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/felinae98/nonebot-plugin-send-anything-anywhere/test.yml)\n![Codecov](https://img.shields.io/codecov/c/github/felinae98/nonebot-plugin-send-anything-anywhere)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nonebot-plugin-send-anything-anywhere)\n![PyPI](https://img.shields.io/pypi/v/nonebot-plugin-send-anything-anywhere)\n![GitHub](https://img.shields.io/github/license/felinae98/nonebot-plugin-send-anything-anywhere)\n\n</div>\n\n这个插件可以做什么\n\n- 为常见的消息类型提供抽象类，自适应转换成对应 adapter 的消息\n- 提供一套统一的，符合直觉的发送接口\n- 为复杂的消息提供易用的生成接口（规划中）\n\n本插件通过传入 bot 的类型来自适应生成对应 bot adapter 所使用的 Message\n\n## 安装\n\n- 使用 nb-cli 安装  \n  `nb plugin install nonebot-plugin-send-anything-anywhere`\n- 使用 poetry 安装  \n  `poetry add nonebot-plugin-send-anything-anywhere`\n- 使用 pip 安装  \n  `pip install nonebot-plugin-send-anything-anywhere`\n\n## 使用\n\n在 handler 中回复消息的情况：\n\n```python\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    # 直接调用 MessageFactory.send() 在 handler 中回复消息\n    await MessageFactory("你好").send(reply=True, at_sender=True)\n    await MessageFactory("需要回复的内容").send()\n    await matcher.finish()\n```\n\n主动发送的情况：\n\n```python\nfrom nonebot_plugin_saa import TargetQQGroup\n\n# 发送目标为 QQ 号 10000, 以私聊形式发送\ntarget = TargetQQGroup(group_id=2233)\nawait MessageFactory("早上好").send_to(target)\n```\n\n从消息事件中提取发送目标:\n\n```python\nfrom nonebot_plugin_saa import extract_target, get_target\n\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    target = extract_target(event)\n\n@matcher.handle()\nasync def handle(target: PlatformTarget = Depends(get_target)):\n    ...\n```\n\n发送目标的序列化与反序列化:\n\n```python\nfrom nonebot_plugin_saa import PlatformTarget, TargetQQPrivate\n\ntarget = TargetQQPrivate(user_id=112233)\nserialized_target = target.json()\ndeserialized_target = PlatformTarget.deserialize(serialized_target)\nassert deserialized_target == target\n```\n\n## 支持情况\n\n✅:支持 ✖️:支持不了 🚧:等待适配\n\n### 支持的 adapter\n\n| OneBot v11 | OneBot v12 | QQ Guild | Kaiheila |\n| :--------: | :--------: | :------: | :------: |\n|     ✅     |     ✅     |    ✅    |    ✅    |\n\n### 支持的消息类型\n\n|      | OneBot v11 | OneBot v12 | QQ Guild | 开黑啦 |\n| :--: | :--------: | :--------: | :------: | :----: |\n| 文字 |     ✅     |     ✅     |    ✅    |   ✅   |\n| 图片 |     ✅     |     ✅     |    ✅    |   ✅   |\n|  at  |     ✅     |     ✅     |    ✅    |   ✅   |\n| 回复 |     ✅     |     ✅     |    ✅    |   ✅   |\n\n### 支持的发送目标\n\n|                   | OneBot v11 | OneBot v12  | QQ Guild | Kaiheila |\n| :---------------: | :--------: | :---------: | :------: | :------: |\n|       QQ 群       |     ✅     |     ✅      |          |          |\n|      QQ 私聊      |     ✅     |     ✅      |          |          |\n| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |          |\n|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |          |\n|  开黑啦私聊/频道  |            |             |          |    ✅    |\n\n注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用\n\n## 问题与例子\n\n因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的\n\nbefore:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v11.message import MessageSegment as V11MessageSegment\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.adapters.onebot.v12.message import MessageSegment as V12MessageSegment\nfrom nonebot.adapters.onebot.v12.bot import Bot as V12Bot\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v11(event: V11MessageEvent):\n    pic_content = ...\n    msg = V11MessageSegment.image(pic_content) + V11MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n\npic_matcher.handle()\nasync def _handle_v12(bot: V12Bot, event: V12MessageEvent):\n    pic_content = ...\n    pic_file = await bot.upload_file(type=\'data\', name=\'image\', data=pic_content)\n    msg = V12MessageSegment.image(pic_file[\'file_id\']) + V12MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n```\n\n现在只需要:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.internal.adapter.bot import Bot\nfrom nonebot_plugin_saa import Image, Text, MessageFactory\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v12(bot: Bot, event: Union[V12MessageEvent, V11MessageEvent]):\n    pic_content = ...\n    msg_builder = MessageFactory([\n        Image(pic_content), Text("这是你要的图片")\n    ])\n    # or msg_builder = Image(pic_content) + Text("这是你要的图片")\n    await msg_builder.send()\n    await pic_matcher.finish()\n```\n\n## 类似项目\n\n- [nonebot-plugin-all4one](https://github.com/nonepkg/nonebot-plugin-all4one) 解决了类似的问题，但是用了不同路径\n- [nonebot-plugin-params](https://github.com/iyume/nonebot-plugin-params) 通过 Rule 定制订阅的平台，与本插件联合使用也许会有奇效\n\n## License\n\nMIT\n',
     'author': 'felinae98',
     'author_email': '731499577@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.4/PKG-INFO` & `nonebot_plugin_send_anything_anywhere-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-send-anything-anywhere
-Version: 0.2.4
+Version: 0.2.5
 Summary: An adaptor for nonebot2 adaptors
 License: MIT
 Author: felinae98
 Author-email: 731499577@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
+Requires-Dist: anyio (>=3.6.2,<4.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: strenum (>=0.4.8,<0.5.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 ~logo征集中，假装有图片~
```

