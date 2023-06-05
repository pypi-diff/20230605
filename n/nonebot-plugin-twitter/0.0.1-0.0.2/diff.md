# Comparing `tmp/nonebot-plugin-twitter-0.0.1.tar.gz` & `tmp/nonebot-plugin-twitter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.0.1.tar", last modified: Sun Jun  4 14:52:00 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.0.2.tar", last modified: Mon Jun  5 07:21:22 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.0.1.tar` & `nonebot-plugin-twitter-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-04 14:51:49.845334 nonebot-plugin-twitter-0.0.1/LICENSE
--rw-r--r--   0        0        0     3761 2023-06-04 14:51:49.845334 nonebot-plugin-twitter-0.0.1/README.md
--rw-r--r--   0        0        0     9207 2023-06-04 14:51:49.845334 nonebot-plugin-twitter-0.0.1/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0      996 2023-06-04 14:51:49.845334 nonebot-plugin-twitter-0.0.1/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      646 2023-06-04 14:51:49.845334 nonebot-plugin-twitter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-05 07:21:14.677302 nonebot-plugin-twitter-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2777 2023-06-05 07:21:14.677302 nonebot-plugin-twitter-0.0.2/README.md
+-rw-r--r--   0        0        0    14471 2023-06-05 07:21:14.677302 nonebot-plugin-twitter-0.0.2/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     1041 2023-06-05 07:21:14.677302 nonebot-plugin-twitter-0.0.2/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      646 2023-06-05 07:21:14.677302 nonebot-plugin-twitter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3145 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.2/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.0.1/LICENSE` & `nonebot-plugin-twitter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.1/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.0.2/nonebot_plugin_twitter/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+import contextlib
 import os
 from nonebot import require,get_driver,get_bot,on_command
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
-from nonebot.permission import SUPERUSER
-from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN,GROUP_OWNER
 from nonebot.adapters.onebot.v11 import Message,MessageEvent,Bot,GroupMessageEvent,MessageSegment
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
 from nonebot.log import logger
 import nonebot
 from nonebot.adapters.onebot.v11.adapter import Adapter
 from nonebot.exception import MatcherException
 from nonebot.plugin import PluginMetadata
 from pathlib import Path
 import json
-import time
+import random
 from httpx import AsyncClient
 import asyncio
 import tweepy
 from .config import Config,__version__
 
+#
 config_dev = Config.parse_obj(get_driver().config)
 
 __plugin_meta__ = PluginMetadata(
     name="twitter 推特订阅",
     description="订阅 twitter 推文",
     usage="""
     """,
@@ -33,94 +33,100 @@
     supported_adapters={"~onebot.v11"},
     extra={
         "author":"nek0us",
         "version":__version__,
         "priority":config_dev.command_priority
     }
 )
-
-if not config_dev.Bearer_Token:
-    logger.warning("Bearer_Token 未配置")
+header = {
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.4951.64 Safari/537.36'}
+if not config_dev.bearer_token:
+    logger.warning("bearer_token 未配置")
     config_dev.plugin_enabled = False
         
 if config_dev.plugin_enabled:
     # Path
     dirpath = Path() / "data" / "twitter"
     dirpath.mkdir(parents=True, exist_ok=True)
     dirpath = Path() / "data" / "twitter" / "cache"
     dirpath.mkdir(parents=True, exist_ok=True)
     dirpath = Path() / "data" / "twitter" / "group_list.json"
     dirpath.touch()
     if not dirpath.stat().st_size:
         dirpath.write_text("{}")
+    pripath = Path() / "data" / "twitter" / "pri_list.json"
+    pripath.touch()
+    if not pripath.stat().st_size:
+        pripath.write_text("{}")
     
     # Twitter token
     client = tweepy.Client(
-        bearer_token=config_dev.Bearer_Token
+        bearer_token=config_dev.bearer_token
     )     
-    if config_dev.Proxy:
-        # Proxy
+    if config_dev.twitter_proxy:
+        # twitter_proxy
         client.session.proxies = {
-            "http":config_dev.Proxy,
-            "https":config_dev.Proxy
+            "http":config_dev.twitter_proxy,
+            "https":config_dev.twitter_proxy
         }
     
-    @scheduler.scheduled_job("interval",minutes=15,id="twitter",misfire_grace_time=600)
+    @scheduler.scheduled_job("interval",minutes=3,id="twitter",misfire_grace_time=180)
     async def now_twitter():
-        task_list = []
+        group_task_list = []
         group_list = json.loads(dirpath.read_text("utf8"))
         for group_num in group_list:
             if group_num and group_list[group_num]["status"] == "on":
-                task_list.extend(
-                    get_status(group_list, group_num, user_id, group_list[group_num][str(user_id)][1])
+                group_task_list.extend(
+                    get_status("group",group_list, group_num, user_id, group_list[group_num][user_id][1])
                     for user_id in group_list[group_num]
                     if user_id != "status"
                 )
-        asyncio.gather(*task_list)
-
-
-# 数据结构
-
-# {
-#     group_num[str]:{
-#         user_id[str]:[
-#             user_name[str],
-#             since_id[int],
-#             r18[bool]
-#             ],
-#         status:"on/off",
+        asyncio.gather(*group_task_list)
         
-#     }
-# }
+        pri_task_list = []
+        pri_list = json.loads(pripath.read_text("utf8"))
+        for qq_num in pri_list:
+            if qq_num and pri_list[qq_num]["status"] == "on":
+                pri_task_list.extend(
+                    get_status("pri",pri_list, qq_num, user_id, pri_list[qq_num][user_id][1])
+                    for user_id in pri_list[qq_num]
+                    if user_id != "status"
+                )
+        asyncio.gather(*pri_task_list)
 
-        
-async def get_status(group_list, group_num, user_id,since_id):
+async def get_status(type_list: str,l_list: list, l_num: str, user_id: str,since_id: int):
+    
+    # 获取推文
     try:
         ne = client.get_users_tweets(
         id=user_id,
         max_results = 5,
         since_id = since_id
         )
         if ne.data:
-            path_res = await get_tweet_for_id(user_id,group_list[group_num][user_id][2],group_list[group_num][user_id][0])
-            task_res = [msg_type(2854196310, path,name=group_list[group_num][user_id][0]) for path in path_res]
+            res = await get_tweet_for_id(ne.data[-1].id,l_list[l_num][user_id][2],l_list[l_num][user_id][0])
+            
             bots = nonebot.get_adapter(Adapter).bots
-            # 发送异步后的数据
             for bot in bots:
                 try:
-                    await bots[bot].send_group_forward_msg(group_id=int(group_num), messages=task_res)
+                    if type_list == "group":
+                        await bots[bot].send_group_forward_msg(group_id=int(l_num), messages=res["task"])
+                    else:
+                        await bots[bot].send_private_forward_msg(user_id=int(l_num), messages=res["task"])
                 except Exception:
                     pass
-                    #await bot.send_group_forward_msg(group_id=event.group_id, messages=task_res)
-            # else:
-            #     await bot.send_private_forward_msg(user_id=event.user_id, messages=aio_task_res)
-
+            l_list[l_num][str(user_id)][1] = ne.data[-1].id
+            if type_list == "group":
+                dirpath.write_text(json.dumps(l_list))
+            else:
+                pripath.write_text(json.dumps(l_list))
             # 清除垃圾
-            for path in path_res:
+            for path in res["path"]:
                 os.unlink(path)
+                os.unlink(path+".jpg")
     except Exception as e:
         pass
     
 async def get_tweet_for_id(id: int,r18: bool,name: str):
     '''
     id: 推文id
     r18：是否发送r18
@@ -130,128 +136,226 @@
                                 ","),
                             expansions=[
                                 'entities.mentions.username',
                                 'attachments.media_keys',
                             ],
                     tweet_fields=["possibly_sensitive"])
     if tweet.data.possibly_sensitive and not r18:
-        raise ValueError("该条为r18，丢弃")
-        # 主要内容
+        logger.info(f"{name} 的推文 {str(id)} 为r18，根据配置跳过")
+        raise ValueError("该条为r18，跳过")
+    
     tweet_json = tweet.includes
     task = []
     # 逐个判断是照片还是视频
-    task.append(MessageSegment.node_custom(
+    task_res = []
+    task_res.append(MessageSegment.node_custom(
         user_id=2854196310,
         nickname=name,
         content=Message(tweet.data.text)
     ))
-    for tweet_single in tweet_json['media']:
-        # 图片
-        if tweet_single['type'] == "photo":
-            # print(tweet_single.url)
-            task.append(get_pic(tweet_single.url))
-            # await twit.send(Message(f"[CQ:image,file=file:///{path}]"))
-            # os.unlink(f"{path}")
-        # 视频
-        elif tweet_single['type'] == "video":
-            # print(tweet_single['variants'][0]['url'])
-            task.append(get_video(tweet_single['variants'][0]['url']))
-            # print(path)
-            # await twit.send(Message(f"[CQ:video,file=file:///{path}]"))
-            # os.unlink(f"{path}")
-    path_res = await asyncio.gather(*task)
-    return path_res
+    if tweet_json:
+        for tweet_single in tweet_json['media']:
+            # 图片
+            if tweet_single['type'] == "photo":
+                task.append(get_pic(tweet_single.url))
+            # 视频
+            elif tweet_single['type'] == "video":
+                task.append(get_video(tweet_single['variants'][0]['url']))
+    try:
+        path_res = await asyncio.gather(*task)
+    except Exception as e:
+        logger.debug(f"下载媒体出现异常：{e}")
+        path_res = []
+    task_res += [msg_type(2854196310, path,name=name) for path in path_res]
+    return {"task":task_res,"path":path_res}
         
         
 def msg_type(user_id:int, task: str,name: str):
+    
     if task.endswith("jpg") or task.endswith("png"):
-        print(f"file:///{task}]")
         return MessageSegment.node_custom(user_id=user_id, nickname=name,
-                                   content=Message(MessageSegment.image(f"file:///{task}")))
+                                   content=Message(MessageSegment.image(f"file://{task}")))
     elif task.endswith("mp4"):
         return MessageSegment.node_custom(user_id=user_id, nickname=name,
                                           content=Message(MessageSegment.video(f"file:///{task}")))        
         
-        #print("色色可不好哦~")
-    # print(f"链接为小蓝鸟：{tweet.data.text}")
-    
-async def get_pic(url: str) -> Path:
+async def get_pic(url: str) -> str:
     path = Path() / "data" / "twitter" / "cache" /  url.split('/').pop()
-    if config_dev.Proxy:
-        async with AsyncClient(proxies=f"http://{config_dev.Proxy}") as client:
+    path = f"{os.getcwd()}/{str(path)}"
+    if config_dev.twitter_proxy:
+        async with AsyncClient(proxies=f"http://{config_dev.twitter_proxy}") as client:
             res = await client.get(url)
             if res.status_code != 200:
                 raise ValueError("图片下载失败")
             with open(path,'wb') as file:
                 file.write(res.read())
-            return path
     else:
         async with AsyncClient() as client:
             res = await client.get(url)
             if res.status_code != 200:
                 raise ValueError("图片下载失败")
             with open(path,'wb') as file:
                 file.write(res.read())
-            return path
+            
+    return path
 
-async def get_video(url: str) -> Path:
-    path = Path() / "data" / "twitter" / "cache" /  url.split('/').pop()
-    if config_dev.Proxy:
-        async with AsyncClient(proxies=f"http://{config_dev.Proxy}") as client:
-            async with client.stream('GET',url) as res:
+async def get_video(url: str) -> str:
+    path = Path() / "data" / "twitter" / "cache" /  f"{str(random.randint(1, 100))}.mp4"
+    path = f"{os.getcwd()}/{str(path)}"
+    if config_dev.twitter_proxy:
+        async with AsyncClient(proxies=f"http://{config_dev.twitter_proxy}") as client:
+            async with client.stream('GET',url,headers=header) as res:
                 if res.status_code != 200:
                     raise ValueError("视频下载失败")
                 with open(path,'wb') as file:
                     async for chunk in res.aiter_bytes():
                         file.write(chunk)
-                return path
     else:
         async with AsyncClient() as client:
-            async with client.stream('GET',url) as res:
+            async with client.stream('GET',url,headers=header) as res:
                 if res.status_code != 200:
                     raise ValueError("视频下载失败")
                 with open(path,'wb') as file:
                     async for chunk in res.aiter_bytes():
                         file.write(chunk)
-                return path
-    
-    
-save = on_command("关注推主",block=True,priority=config_dev.command_priority)
-@save.handle()
-async def save_handle(bot:Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
-    if isinstance(event,GroupMessageEvent):
-        user_id = get_id(arg.extract_plain_text())
-        res = client.get_users_tweets(
-            id=user_id,
-            max_results = 5
-        )
-        since_id = res.data[0].id
-        if user_id == "未找到":
-            group_list = json.loads(dirpath.read_text("utf8"))
-            if str(event.group_id) not in group_list:
-                group_list[str(event.group_id)] = {"status":"on"}
-            group_list[str(event.group_id)][str(user_id)] = [arg.extract_plain_text(),since_id,True]
-            dirpath.write_text(json.dumps(group_list))
-            await matcher.finish(f"绑定成功了")
+    return path
         
 async def get_id(name: str) -> str:
     '''return user_id from user_name'''
     try:
-        return client.get_user(username="nek0us").data.id
-    except:
-        return "未找到"
+        return str(client.get_user(username=name).data.id)
+    except Exception as e:
+        return "未找到"    
+    
+save = on_command("关注推主",block=True,priority=config_dev.command_priority)
+@save.handle()
+async def save_handle(bot:Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
+    data = []
+    if " " in arg.extract_plain_text():
+        data = arg.extract_plain_text().split(" ")
+    else:
+        data.append(arg.extract_plain_text())
+    user_id = await get_id(data[0])
+    
+    if user_id == "未找到":
+        await matcher.finish(f"未找到 {arg}")
         
+    res = client.get_users_tweets(
+        id=user_id,
+        max_results = 5
+    )
+    since_id = res.data[0].id if res.data else 0
+    
+    if isinstance(event,GroupMessageEvent):
+        group_list = json.loads(dirpath.read_text("utf8"))
+        if str(event.group_id) not in group_list:
+            group_list[str(event.group_id)] = {"status":"on"}
+        if len(data) > 1:
+            group_list[str(event.group_id)][user_id] = [data[0],since_id,True]
+        else:
+            group_list[str(event.group_id)][user_id] = [data[0],since_id,False]
+        dirpath.write_text(json.dumps(group_list))
+    else:
+        pri_list = json.loads(pripath.read_text("utf8"))
+        if str(event.user_id) not in pri_list:
+            pri_list[str(event.user_id)] = {"status":"on"}
+        pri_list[str(event.user_id)][user_id] = [data[0],since_id,True]
+        pripath.write_text(json.dumps(pri_list))
+    await matcher.finish(f"订阅 {data[0]} 完成")
         
 
-# 数据结构
+delete = on_command("取关推主",block=True,priority=config_dev.command_priority)
+@delete.handle()
+async def delete_handle(bot:Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
+    user_id = await get_id(arg.extract_plain_text())
+    if user_id == "未找到":
+        await matcher.finish(f"未找到 {arg}")
 
-# {
-#     group_num[str]:{
-#         user_id[str]:[
-#             user_name[str],
-#             since_id[int],
-#             r18[bool]
-#             ],
-#         status:"on/off",
-        
-#     }
-# }
+    if isinstance(event,GroupMessageEvent):
+        group_list = json.loads(dirpath.read_text("utf8"))
+        if str(event.group_id) not in group_list:
+            group_list[str(event.group_id)] = {"status":"on"}
+
+        try:
+            if arg.extract_plain_text() == group_list[str(event.group_id)][user_id][0]:
+                group_list[str(event.group_id)].pop(user_id) 
+            else:
+                raise ValueError("尚未关注 {arg.extract_plain_text()}")
+        except Exception as e:
+            await matcher.finish(f"{e}")
+        dirpath.write_text(json.dumps(group_list))
+    else:
+        pri_list = json.loads(pripath.read_text("utf8"))
+        if str(event.user_id) not in pri_list:
+            pri_list[str(event.user_id)] = {"status":"on"}
+
+        try:
+            if arg.extract_plain_text() == pri_list[str(event.user_id)][user_id][0]:
+                pri_list[str(event.user_id)].pop(user_id) 
+            else:
+                raise ValueError("尚未关注 {arg.extract_plain_text()}")
+        except Exception as e:
+            await matcher.finish(f"{e}")
+        pripath.write_text(json.dumps(pri_list))
+
+    await matcher.finish(f"取关 {arg.extract_plain_text()} 成功")
+    
+follow_list = on_command("推主列表",block=True,priority=config_dev.command_priority)
+@follow_list.handle()
+async def follow_list_handle(bot:Bot,event: MessageEvent,matcher: Matcher):
+    if isinstance(event,GroupMessageEvent):
+        data = json.loads(dirpath.read_text("utf8"))[str(event.group_id)]
+    else:
+        data = json.loads(pripath.read_text("utf8"))[str(event.user_id)]
+    del data["status"]
+    name_list = [data[x][0] for x in data]
+    res = [
+        MessageSegment.node_custom(
+            user_id=2854196310, nickname="推主id", content=Message(x)
+        )
+        for x in name_list
+    ]
+    bots = nonebot.get_adapter(Adapter).bots
+    for bot in bots:
+        with contextlib.suppress(Exception):
+            if event.message_type == "group":
+                await bots[bot].send_group_forward_msg(group_id=int(event.group_id), messages=res)
+            else:
+                await bots[bot].send_private_forward_msg(user_id=int(event.user_id), messages=res)
+    await matcher.finish()
+
+
+async def is_rule(event:MessageEvent) -> bool:
+    if isinstance(event,GroupMessageEvent):
+        if event.sender.role in ["owner","admin"]:
+            return True
+        return False
+    else:
+        return True
+    
+twitter_status = on_command("推特推送",block=True,rule=is_rule,priority=config_dev.command_priority)
+@twitter_status.handle()
+async def twitter_status_handle(bot:Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
+    if isinstance(event,GroupMessageEvent):
+        group_list = json.loads(dirpath.read_text("utf8"))
+        if str(event.group_id) not in group_list:
+            group_list[str(event.group_id)] = {"status":"on"}
+        if arg.extract_plain_text() == "开启":
+            group_list[str(event.group_id)]["status"] = "on"
+            dirpath.write_text(json.dumps(group_list))
+            await matcher.finish("推送已开启")
+        elif arg.extract_plain_text() == "关闭":
+            group_list[str(event.group_id)]["status"] = "off"
+            dirpath.write_text(json.dumps(group_list))
+            await matcher.finish("推送已关闭")
+    else:
+        pri_list = json.loads(pripath.read_text("utf8"))
+        if str(event.user_id) not in pri_list:
+            pri_list[str(event.user_id)] = {"status":"on"}
+        if arg.extract_plain_text() == "开启":
+            pri_list[str(event.user_id)]["status"] = "on"
+            pripath.write_text(json.dumps(pri_list))
+            await matcher.finish("推送已开启")
+        elif arg.extract_plain_text() == "关闭":
+            pri_list[str(event.user_id)]["status"] = "off"
+            pripath.write_text(json.dumps(pri_list))
+            await matcher.finish("推送已关闭")
```

### Comparing `nonebot-plugin-twitter-0.0.1/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.0.2/nonebot_plugin_twitter/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 
 try:
     __version__ = version("nonebot_plugin_bilichat")
 except Exception:
     __version__ = None
 
 class Config(BaseModel):
-    Bearer_Token: Optional[str]
-    Proxy: Optional[str]
+    bearer_token: Optional[str] = ""
+    twitter_proxy: Optional[str] = ""
     command_priority: int = 10
     plugin_enabled: bool = True
     
-    @validator("Bearer_Token")
+    @validator("bearer_token")
     def check_bearer_token(cls,v):
-        if isinstance(str,v):
-            logger.info("Bearer_Token 读取成功")
+        if isinstance(v,str):
+            logger.info("bearer_token 读取成功")
             return v
-    @validator("Proxy")
+    @validator("twitter_proxy")
     def check_proxy(cls,v):
-        if isinstance(str,v):
-            logger.info("Proxy 读取成功")
+        if isinstance(v,str):
+            logger.info("twitter_proxy 读取成功")
             return v
         
     @validator("command_priority")
     def check_command_priority(cls,v):
-        if isinstance(str,v):
+        if isinstance(v,int) and v >= 1:
             logger.info("command_priority 读取成功")
             return v
```

### Comparing `nonebot-plugin-twitter-0.0.1/pyproject.toml` & `nonebot-plugin-twitter-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.0.1"
+version = "0.0.2"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

