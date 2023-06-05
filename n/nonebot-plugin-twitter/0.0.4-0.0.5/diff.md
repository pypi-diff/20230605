# Comparing `tmp/nonebot-plugin-twitter-0.0.4.tar.gz` & `tmp/nonebot-plugin-twitter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.0.4.tar", last modified: Mon Jun  5 11:30:46 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.0.5.tar", last modified: Mon Jun  5 15:35:44 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.0.4.tar` & `nonebot-plugin-twitter-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-05 11:30:37.923668 nonebot-plugin-twitter-0.0.4/LICENSE
--rw-r--r--   0        0        0     2777 2023-06-05 11:30:37.923668 nonebot-plugin-twitter-0.0.4/README.md
--rw-r--r--   0        0        0    14977 2023-06-05 11:30:37.923668 nonebot-plugin-twitter-0.0.4/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     1041 2023-06-05 11:30:37.923668 nonebot-plugin-twitter-0.0.4/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      646 2023-06-05 11:30:37.923668 nonebot-plugin-twitter-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3145 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-05 15:35:33.871221 nonebot-plugin-twitter-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3127 2023-06-05 15:35:33.871221 nonebot-plugin-twitter-0.0.5/README.md
+-rw-r--r--   0        0        0    15454 2023-06-05 15:35:33.871221 nonebot-plugin-twitter-0.0.5/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     1041 2023-06-05 15:35:33.871221 nonebot-plugin-twitter-0.0.5/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      646 2023-06-05 15:35:33.871221 nonebot-plugin-twitter-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.5/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.0.4/LICENSE` & `nonebot-plugin-twitter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.4/README.md` & `nonebot-plugin-twitter-0.0.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -67,28 +67,33 @@
 
 </details>
 
 ## ⚙️ 配置
 
 申请 [twitter api](https://developer.twitter.com/zh-cn/docs/twitter-ads-api/getting-started) 权限
 
-生成 Bearer Token
+生成并记录 [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
+
+[![pCPufJ0.png](https://s1.ax1x.com/2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0)
  
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bearer_token | 是 | 无 | api token |
+| bearer_token | 是 | 无 | Bearer Token |
 | twitter_proxy | 否 | 无 | proxy |
 | command_priority | 否 | 10 | 命令优先级 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | 关注推主 | 无 | 否 | 群聊/私聊 | 关注，指令格式：“关注推主 <推主id> [r18]” r18为可选参数，不开启和默认为不推送r18推文|
 | 取关推主 | 无 | 否 | 群聊/私聊 | 取关切割 |
 | 推主列表 | 无 | 否 | 群聊/私聊 | 展示列表 |
 | 推特推送关闭 | 群管 | 否 | 群聊/私聊 | 关闭推送 |
 | 推特推送开启 | 群管 | 否 | 群聊/私聊 | 开启推送 |
+### 效果图
+[![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/pCPuhWV.png)](https://imgse.com/i/pCPuhWV)
+[![pCPu4zT.png](https://s1.ax1x.com/2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT)
 ### 注意事项
 1.消息为合并转发发送，存在延迟和发送失败的可能
```

#### html2text {}

```diff
@@ -8,20 +8,25 @@
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter
 poetry poetry add nonebot-plugin-twitter   conda conda install nonebot-plugin-
 twitter  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
 âï¸ éç½® ç³è¯· [twitter api](https://developer.twitter.com/zh-cn/docs/
-twitter-ads-api/getting-started) æé çæ Bearer Token å¨ nonebot2
+twitter-ads-api/getting-started) æé çæå¹¶è®°å½ [Bearer Token](https://
+developer.twitter.com/en/portal/dashboard) [![pCPufJ0.png](https://s1.ax1x.com/
+2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0) å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | bearer_token | æ¯ | æ 
-| api token | | twitter_proxy | å¦ | æ  | proxy | | command_priority | å¦ |
-10 | å½ä»¤ä¼åçº§ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@
-| èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ 
-| å¦ | ç¾¤è/ç§è | å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id>
-[r18]â r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| |
-åå³æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ 
-| å¦ | ç¾¤è/ç§è | å±ç¤ºåè¡¨ | | æ¨ç¹æ¨éå³é­ | ç¾¤ç®¡ | å¦ |
-ç¾¤è/ç§è | å³é­æ¨é | | æ¨ç¹æ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/
-ç§è | å¼å¯æ¨é | ### æ³¨æäºé¡¹
+| Bearer Token | | twitter_proxy | å¦ | æ  | proxy | | command_priority | å¦
+| 10 | å½ä»¤ä¼åçº§ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
+éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
+å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
+å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
+r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| | åå³æ¨ä¸» |
+æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ  | å¦ | ç¾¤è/
+ç§è | å±ç¤ºåè¡¨ | | æ¨ç¹æ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
+å³é­æ¨é | | æ¨ç¹æ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
+å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
+pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
+2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
 1.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
```

### Comparing `nonebot-plugin-twitter-0.0.4/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.0.5/nonebot_plugin_twitter/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,16 +122,17 @@
                     pass
             l_list[l_num][str(user_id)][1] = ne.data[-1].id
             if type_list == "group":
                 dirpath.write_text(json.dumps(l_list))
             else:
                 pripath.write_text(json.dumps(l_list))
             # 清除垃圾
+            await asyncio.sleep(50)
             for path in res["path"]:
-                os.unlink(path)
+                os.unlink(path) 
                 os.unlink(path+".jpg")
     except Exception as e:
         pass
     
 async def get_tweet_for_id(id: int,r18: bool,name: str):
     '''
     id: 推文id
@@ -144,22 +145,22 @@
                                 'entities.mentions.username',
                                 'attachments.media_keys',
                             ],
                     tweet_fields=["possibly_sensitive"])
     if tweet.data.possibly_sensitive and not r18:
         logger.info(f"{name} 的推文 {str(id)} 为r18，根据配置跳过")
         raise ValueError("该条为r18，跳过")
-    
+    username = await get_user_name(name)
     tweet_json = tweet.includes
     task = []
     # 逐个判断是照片还是视频
     task_res = []
     task_res.append(MessageSegment.node_custom(
         user_id=2854196310,
-        nickname=name,
+        nickname=username,
         content=Message(tweet.data.text)
     ))
     if tweet_json:
         for tweet_single in tweet_json['media']:
             # 图片
             if tweet_single['type'] == "photo":
                 task.append(get_pic(tweet_single.url))
@@ -222,20 +223,27 @@
                     raise ValueError("视频下载失败")
                 with open(path,'wb') as file:
                     async for chunk in res.aiter_bytes():
                         file.write(chunk)
     return path
         
 async def get_id(name: str) -> str:
-    '''return user_id from user_name'''
+    '''return user_id from name'''
     try:
         return str(client.get_user(username=name).data.id)
     except Exception as e:
         return "未找到"    
     
+async def get_user_name(name) -> str:
+    '''return user_name from name'''
+    try:
+        return client.get_user(username=name).data.name
+    except Exception as e:
+        return "未找到name" 
+    
 save = on_command("关注推主",block=True,priority=config_dev.command_priority)
 @save.handle()
 async def save_handle(bot:Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
     data = []
     if " " in arg.extract_plain_text():
         data = arg.extract_plain_text().split(" ")
     else:
@@ -262,15 +270,16 @@
         dirpath.write_text(json.dumps(group_list))
     else:
         pri_list = json.loads(pripath.read_text("utf8"))
         if str(event.user_id) not in pri_list:
             pri_list[str(event.user_id)] = {"status":"on"}
         pri_list[str(event.user_id)][user_id] = [data[0],since_id,True]
         pripath.write_text(json.dumps(pri_list))
-    await matcher.finish(f"订阅 {data[0]} 完成")
+    username = await get_user_name(data[0])
+    await matcher.finish(f"id:{data[0]}\nname:{username}\n订阅成功")
         
 
 delete = on_command("取关推主",block=True,priority=config_dev.command_priority)
 @delete.handle()
 async def delete_handle(bot:Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
     user_id = await get_id(arg.extract_plain_text())
     if user_id == "未找到":
@@ -310,19 +319,23 @@
 async def follow_list_handle(bot:Bot,event: MessageEvent,matcher: Matcher):
     if isinstance(event,GroupMessageEvent):
         data = json.loads(dirpath.read_text("utf8"))[str(event.group_id)]
     else:
         data = json.loads(pripath.read_text("utf8"))[str(event.user_id)]
     del data["status"]
     name_list = [data[x][0] for x in data]
+    username_list = []
+    for x in name_list:
+        username_list.append(await get_user_name(x))
+    
     res = [
         MessageSegment.node_custom(
-            user_id=2854196310, nickname="推主id", content=Message(x)
+            user_id=2854196310, nickname=username, content=Message(name)
         )
-        for x in name_list
+        for name,username in zip(name_list,username_list)
     ]
     bots = nonebot.get_adapter(Adapter).bots
     for bot in bots:
         with contextlib.suppress(Exception):
             if event.message_type == "group":
                 await bots[bot].send_group_forward_msg(group_id=int(event.group_id), messages=res)
             else:
```

### Comparing `nonebot-plugin-twitter-0.0.4/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.0.5/nonebot_plugin_twitter/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.4/pyproject.toml` & `nonebot-plugin-twitter-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.0.4"
+version = "0.0.5"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-twitter-0.0.4/PKG-INFO` & `nonebot-plugin-twitter-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.0.4
+Version: 0.0.5
 Summary: NoneBot2 plugin for twitter
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-twitter
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-twitter
 Description-Content-Type: text/markdown
@@ -78,29 +78,34 @@
 
 </details>
 
 ## ⚙️ 配置
 
 申请 [twitter api](https://developer.twitter.com/zh-cn/docs/twitter-ads-api/getting-started) 权限
 
-生成 Bearer Token
+生成并记录 [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
+
+[![pCPufJ0.png](https://s1.ax1x.com/2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0)
  
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bearer_token | 是 | 无 | api token |
+| bearer_token | 是 | 无 | Bearer Token |
 | twitter_proxy | 否 | 无 | proxy |
 | command_priority | 否 | 10 | 命令优先级 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | 关注推主 | 无 | 否 | 群聊/私聊 | 关注，指令格式：“关注推主 <推主id> [r18]” r18为可选参数，不开启和默认为不推送r18推文|
 | 取关推主 | 无 | 否 | 群聊/私聊 | 取关切割 |
 | 推主列表 | 无 | 否 | 群聊/私聊 | 展示列表 |
 | 推特推送关闭 | 群管 | 否 | 群聊/私聊 | 关闭推送 |
 | 推特推送开启 | 群管 | 否 | 群聊/私聊 | 开启推送 |
+### 效果图
+[![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/pCPuhWV.png)](https://imgse.com/i/pCPuhWV)
+[![pCPu4zT.png](https://s1.ax1x.com/2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT)
 ### 注意事项
 1.消息为合并转发发送，存在延迟和发送失败的可能
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.0.5 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
@@ -13,20 +13,25 @@
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter
 poetry poetry add nonebot-plugin-twitter   conda conda install nonebot-plugin-
 twitter  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
 âï¸ éç½® ç³è¯· [twitter api](https://developer.twitter.com/zh-cn/docs/
-twitter-ads-api/getting-started) æé çæ Bearer Token å¨ nonebot2
+twitter-ads-api/getting-started) æé çæå¹¶è®°å½ [Bearer Token](https://
+developer.twitter.com/en/portal/dashboard) [![pCPufJ0.png](https://s1.ax1x.com/
+2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0) å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | bearer_token | æ¯ | æ 
-| api token | | twitter_proxy | å¦ | æ  | proxy | | command_priority | å¦ |
-10 | å½ä»¤ä¼åçº§ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@
-| èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ 
-| å¦ | ç¾¤è/ç§è | å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id>
-[r18]â r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| |
-åå³æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ 
-| å¦ | ç¾¤è/ç§è | å±ç¤ºåè¡¨ | | æ¨ç¹æ¨éå³é­ | ç¾¤ç®¡ | å¦ |
-ç¾¤è/ç§è | å³é­æ¨é | | æ¨ç¹æ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/
-ç§è | å¼å¯æ¨é | ### æ³¨æäºé¡¹
+| Bearer Token | | twitter_proxy | å¦ | æ  | proxy | | command_priority | å¦
+| 10 | å½ä»¤ä¼åçº§ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
+éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
+å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
+å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
+r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| | åå³æ¨ä¸» |
+æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ  | å¦ | ç¾¤è/
+ç§è | å±ç¤ºåè¡¨ | | æ¨ç¹æ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
+å³é­æ¨é | | æ¨ç¹æ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
+å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
+pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
+2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
 1.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
```

