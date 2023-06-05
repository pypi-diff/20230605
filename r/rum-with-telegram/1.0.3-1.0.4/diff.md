# Comparing `tmp/rum_with_telegram-1.0.3.tar.gz` & `tmp/rum_with_telegram-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-1.0.3.tar", last modified: Tue May 16 11:41:22 2023, max compression
+gzip compressed data, was "rum_with_telegram-1.0.4.tar", last modified: Mon Jun  5 15:26:09 2023, max compression
```

## Comparing `rum_with_telegram-1.0.3.tar` & `rum_with_telegram-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 11:41:22.267161 rum_with_telegram-1.0.3/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-16 11:41:22.266163 rum_with_telegram-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-1.0.3/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-1.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-16 11:41:22.252200 rum_with_telegram-1.0.3/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-16 11:25:24.000000 rum_with_telegram-1.0.3/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     2092 2023-05-13 13:53:34.000000 rum_with_telegram-1.0.3/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    26650 2023-05-16 11:25:31.000000 rum_with_telegram-1.0.3/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3872 2023-05-14 08:49:50.000000 rum_with_telegram-1.0.3/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1820 2023-05-12 03:02:22.000000 rum_with_telegram-1.0.3/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:41:22.263173 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-16 11:41:22.000000 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-16 11:41:22.000000 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 11:41:22.000000 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-16 11:41:22.000000 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-16 11:41:22.000000 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 11:41:22.267161 rum_with_telegram-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-05-16 11:25:24.000000 rum_with_telegram-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:26:09.985604 rum_with_telegram-1.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-06-05 15:26:09.984633 rum_with_telegram-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-1.0.4/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-1.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-05 15:26:09.971642 rum_with_telegram-1.0.4/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-06-05 15:23:02.000000 rum_with_telegram-1.0.4/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     2121 2023-06-05 15:18:07.000000 rum_with_telegram-1.0.4/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    27612 2023-06-05 15:25:36.000000 rum_with_telegram-1.0.4/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3872 2023-05-14 08:49:50.000000 rum_with_telegram-1.0.4/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1820 2023-05-12 03:02:22.000000 rum_with_telegram-1.0.4/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:26:09.983611 rum_with_telegram-1.0.4/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-06-05 15:26:09.000000 rum_with_telegram-1.0.4/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-06-05 15:26:09.000000 rum_with_telegram-1.0.4/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:26:09.000000 rum_with_telegram-1.0.4/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-05 15:26:09.000000 rum_with_telegram-1.0.4/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-05 15:26:09.000000 rum_with_telegram-1.0.4/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:26:09.986602 rum_with_telegram-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-06-05 15:23:02.000000 rum_with_telegram-1.0.4/setup.py
```

### Comparing `rum_with_telegram-1.0.3/LICENSE` & `rum_with_telegram-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-1.0.3/PKG-INFO` & `rum_with_telegram-1.0.4/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rum_with_telegram
-Version: 1.0.3
+Name: rum-with-telegram
+Version: 1.0.4
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-1.0.3/rum_with_telegram/config.py` & `rum_with_telegram-1.0.4/rum_with_telegram/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     RUM_TO_TG_TAG: str = ""
     RUM_TO_TG: bool = True
     TG_REPLY_POSTURL: bool = True
     TG_USER_ID: int = None
     TG_CHANNEL_URL: str = None  # the url of telegram url
     TG_CHANNEL_ID: int = None
     TG_GROUP_ID: int = None
+    TG_COMMANDS: list = None
 
     def __post_init__(self):
         if self.TG_CHANNEL_URL is None:
             name = self.TG_CHANNEL_NAME.replace("@", "")
             self.TG_CHANNEL_URL = f"https://t.me/{name}"
         self.ADMIN_USERIDS = self.ADMIN_USERIDS or []
         self.BLACK_LIST_PUBKEYS = self.BLACK_LIST_PUBKEYS or []
```

### Comparing `rum_with_telegram-1.0.3/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-1.0.4/rum_with_telegram/data_exchanger.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import base64
 import datetime
 import io
 import json
 import logging
 
 from quorum_data_py import feed, get_trx_type, util
+from quorum_eth_py import RumEthChainBrowser
 from quorum_mininode_py import MiniNode, pvtkey_to_pubkey
 from telegram import Bot, Update
 from telegram.ext import Application, CommandHandler, ContextTypes, MessageHandler, filters
 
 from rum_with_telegram.config import get_config
 from rum_with_telegram.db_handle import DBHandle
 from rum_with_telegram.module import Relation, UsedKey
@@ -554,36 +555,61 @@
                 )
             reply = f"You have exported your data, that is {len(trxs)} trxs in blockchain of rum-group.\nYour private key is:\n```{user.pvtkey}```\nPlease keep it safe."
             self.db.update_user_export_at(userid)
         else:
             reply = "You have not any data in blockchain of rum-group."
         await update.message.reply_text(reply, parse_mode="Markdown")
 
-    async def command_my_nft(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
-        logger.info("start command_my_nft")
-        # TODO
-
-    async def command_grant_nft(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
-        logger.info("start command_grant_nft")
+    async def command_tokens(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
+        logger.info("start command_tokens")
         userid = update.message.from_user.id
-        if userid not in self.config.ADMIN_USERIDS:
-            await update.message.reply_text("You are not admin.")
+        username = update.message.from_user.username
+        user = self.db.init_user(userid, username)
+        used = self.db.get_all(UsedKey, {"user_id": userid}, "user_id") or []
+
+        if not user:
+            logger.warning("command_tokens error %s", userid)
             return
-        # TODO
+
+        address = user.address
+        tokens = RumEthChainBrowser().get_token_list(address)
+        reply = f"Your address: {address}\n"
+        null = True
+        for i in tokens:
+            if i["balance2"] > 0:
+                reply += f'{i["symbol"]} {i["balance2"]}\n'
+                null = False
+        if null:
+            reply += "You have not any token."
+        else:
+            reply += (
+                f"more details view page: https://explorer.rumsystem.net/address/{address}/tokens"
+            )
+        await update.message.reply_text(reply)
+
+    async def set_commands(self):
+        my_commands = self.config.TG_COMMANDS or []
+        commands = await self.app.bot.get_my_commands()
+        flag = False
+        for cmd in commands:
+            if [cmd.command, cmd.description] not in my_commands:
+                flag = True
+                break
+        if flag:
+            await self.app.bot.set_my_commands(my_commands)
+            logger.info("set_commands %s", my_commands)
 
     def run(self):
         self.app.add_handler(CommandHandler("start", self.command_start))
         self.app.add_handler(CommandHandler("profile", self.command_profile))
         self.app.add_handler(CommandHandler("show_pvtkey", self.command_show_pvtkey))
         self.app.add_handler(CommandHandler("new_pvtkey", self.command_new_pvtkey))
         self.app.add_handler(CommandHandler("import_pvtkey", self.command_import_pvtkey))
         self.app.add_handler(CommandHandler("export_data", self.command_export_data))
-        # TODO:
-        self.app.add_handler(CommandHandler("my_nft", self.command_my_nft))
-        self.app.add_handler(CommandHandler("grant_nft", self.command_grant_nft))
+        self.app.add_handler(CommandHandler("tokens", self.command_tokens))
 
         content_filter = (filters.TEXT | filters.PHOTO) & ~filters.COMMAND
         # private chat message:
         # send to tg channel and rum group as new post
         # reply the feed_post_url to user in private chat and the comment of the channel post
         self.app.add_handler(
             MessageHandler(
```

### Comparing `rum_with_telegram-1.0.3/rum_with_telegram/db_handle.py` & `rum_with_telegram-1.0.4/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-1.0.3/rum_with_telegram/module.py` & `rum_with_telegram-1.0.4/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-1.0.3/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rum-with-telegram
-Version: 1.0.3
+Name: rum_with_telegram
+Version: 1.0.4
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-1.0.3/setup.py` & `rum_with_telegram-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="1.0.3",
+    version="1.0.4",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

