# Comparing `tmp/nonebot_plugin_blacklist-0.3.3.tar.gz` & `tmp/nonebot_plugin_blacklist-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blacklist-0.3.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_blacklist-0.3.4.tar", max compression
```

## Comparing `nonebot_plugin_blacklist-0.3.3.tar` & `nonebot_plugin_blacklist-0.3.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-02-25 04:08:00.841498 nonebot_plugin_blacklist-0.3.3/LICENSE
--rw-r--r--   0        0        0     2550 2023-02-25 04:08:00.841498 nonebot_plugin_blacklist-0.3.3/README.md
--rw-r--r--   0        0        0     8537 2023-02-25 04:08:00.841498 nonebot_plugin_blacklist-0.3.3/nonebot_plugin_blacklist/__init__.py
--rw-r--r--   0        0        0      779 2023-02-25 04:08:00.841498 nonebot_plugin_blacklist-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3347 1970-01-01 00:00:00.000000 nonebot_plugin_blacklist-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-05 01:36:00.636122 nonebot_plugin_blacklist-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2550 2023-06-05 01:36:00.636122 nonebot_plugin_blacklist-0.3.4/README.md
+-rw-r--r--   0        0        0     8710 2023-06-05 01:36:00.636122 nonebot_plugin_blacklist-0.3.4/nonebot_plugin_blacklist/__init__.py
+-rw-r--r--   0        0        0      779 2023-06-05 01:36:00.636122 nonebot_plugin_blacklist-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3347 1970-01-01 00:00:00.000000 nonebot_plugin_blacklist-0.3.4/PKG-INFO
```

### Comparing `nonebot_plugin_blacklist-0.3.3/LICENSE` & `nonebot_plugin_blacklist-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blacklist-0.3.3/README.md` & `nonebot_plugin_blacklist-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blacklist-0.3.3/nonebot_plugin_blacklist/__init__.py` & `nonebot_plugin_blacklist-0.3.4/nonebot_plugin_blacklist/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,22 +23,34 @@
 
 file_path = Path() / 'data' / 'blacklist' / 'blacklist.json'
 file_path.parent.mkdir(parents=True, exist_ok=True)
 
 blacklist = (
     json.loads(file_path.read_text('utf-8'))
     if file_path.is_file()
-    else {'grouplist': ['ban_auto_sleep'], 'userlist': []}
+    else {
+        'grouplist': [],
+        'userlist': [],
+        'ban_auto_sleep': True
+    }
 )
 
 
 def save_blacklist() -> None:
     file_path.write_text(json.dumps(blacklist), encoding='utf-8')
 
 
+if not blacklist.get('ban_auto_sleep'):
+    if 'ban_auto_sleep' in blacklist['grouplist']:
+        blacklist.update({'ban_auto_sleep': True})
+    else:
+        blacklist.update({'ban_auto_sleep': False})
+    save_blacklist()
+
+
 def is_number(s: str) -> bool:
     try:
         float(s)
         return True
     except ValueError:
         pass
     try:
@@ -139,15 +151,15 @@
     await check_userlist.finish(f"当前已屏蔽 {len(blacklist['userlist'])} 个用户: {', '.join(blacklist['userlist'])}")
 
 
 check_grouplist = on_command('查看群聊黑名单', permission=SUPERUSER, priority=1, block=True)
 
 @check_grouplist.handle()
 async def check_group_list():
-    await check_grouplist.finish(f"当前已屏蔽 {len(blacklist['grouplist'])} 个群聊: {', '.join(blacklist['grouplist'])}")
+    await check_grouplist.finish(f"自觉静默: {'开' if blacklist['ban_auto_sleep'] else '关'}\n当前已屏蔽 {len(blacklist['grouplist'])} 个群聊: {', '.join(blacklist['grouplist'])}")
 
 
 add_group = on_command('/静默', permission=SUPERUSER, priority=1, block=True)
 
 @add_group.handle()
 async def add_group_(event: GroupMessageEvent):
     handle_blacklist([f'{event.group_id}'], 'add', 'grouplist')
@@ -213,15 +225,15 @@
         await reset_blacklist.finish('黑名单已重置')
     else:
         await reset_blacklist.finish('操作已取消')
 
 
 @on_notice(priority=2, block=False).handle()
 async def _(bot: Bot, event: GroupBanNoticeEvent):
-    if 'ban_auto_sleep' in blacklist['grouplist'] and event.is_tome() and event.duration:
+    if blacklist['ban_auto_sleep'] and event.is_tome() and event.duration:
         handle_blacklist([f'{event.group_id}'], 'add', 'grouplist')
         for superuser in bot.config.superusers:
             await bot.send_private_msg(
                 user_id=int(superuser),
                 message=f'ⓘ在群聊 {event.group_id} 受到禁言, 已自动拉黑该群聊.'
             )
             await asyncio.sleep(random.random()+1)
@@ -229,17 +241,16 @@
 
 ban_auto_sleep = on_command('自觉静默', permission=SUPERUSER, priority=1, block=True)
 
 @ban_auto_sleep.handle()
 async def _(arg: Message = CommandArg()):
     msg = arg.extract_plain_text().strip()
     if not msg or msg.startswith('开'):
-        blacklist['grouplist'].append('ban_auto_sleep')
-        blacklist['grouplist'] = list(set(blacklist['grouplist']))
+        blacklist['ban_auto_sleep'] = True
         text = '自觉静默已开启.'
     elif msg.startswith('关'):
-        blacklist['grouplist'] = [uid for uid in blacklist['grouplist'] if uid not in ['ban_auto_sleep']]
+        blacklist['ban_auto_sleep'] = False
         text = '自觉静默已关闭.'
     else:
         return
     save_blacklist()
     await ban_auto_sleep.finish(text)
```

### Comparing `nonebot_plugin_blacklist-0.3.3/pyproject.toml` & `nonebot_plugin_blacklist-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blacklist"
-version = "0.3.3"
+version = "0.3.4"
 description = "Blacklist in NoneBot2"
 authors = ["月ヶ瀬"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "nonebot_plugin_blacklist" },
 ]
```

### Comparing `nonebot_plugin_blacklist-0.3.3/PKG-INFO` & `nonebot_plugin_blacklist-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blacklist
-Version: 0.3.3
+Version: 0.3.4
 Summary: Blacklist in NoneBot2
 Home-page: https://github.com/tkgs0/nonebot-plugin-blacklist
 License: MIT
 Keywords: nonebot,blacklist
 Author: 月ヶ瀬
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blacklist Version: 0.3.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blacklist Version: 0.3.4 Summary:
 Blacklist in NoneBot2 Home-page: https://github.com/tkgs0/nonebot-plugin-
 blacklist License: MIT Keywords: nonebot,blacklist Author: æã¶ç¬ Requires-
 Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: nonebot-adapter-onebot
```

