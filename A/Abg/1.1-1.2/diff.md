# Comparing `tmp/Abg-1.1.tar.gz` & `tmp/Abg-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-1.1.tar", last modified: Sun May 28 18:12:46 2023, max compression
+gzip compressed data, was "Abg-1.2.tar", last modified: Mon Jun  5 15:18:56 2023, max compression
```

## Comparing `Abg-1.1.tar` & `Abg-1.2.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-28 18:05:19.000000 Abg-1.1/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/conversation/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-28 18:05:19.000000 Abg-1.1/Abg/conversation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5532 2023-05-28 18:05:19.000000 Abg-1.1/Abg/conversation/conversation.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-05-28 18:05:19.000000 Abg-1.1/Abg/conversation/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/helpers/
--rw-r--r--   0 root         (0) root         (0)      818 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3181 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/lock.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2471 2023-05-28 18:05:19.000000 Abg-1.1/Abg/helpers/pyro_progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/inline/
--rw-r--r--   0 root         (0) root         (0)      280 2023-05-28 18:05:19.000000 Abg-1.1/Abg/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6245 2023-05-28 18:05:19.000000 Abg-1.1/Abg/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4268 2023-05-28 18:05:19.000000 Abg-1.1/Abg/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-05-28 18:05:19.000000 Abg-1.1/Abg/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/patch/
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11748 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-05-28 18:05:19.000000 Abg-1.1/Abg/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 18:12:46.280024 Abg-1.1/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4983 2023-05-28 18:12:46.000000 Abg-1.1/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      721 2023-05-28 18:12:46.000000 Abg-1.1/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 18:12:46.000000 Abg-1.1/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-28 18:12:46.000000 Abg-1.1/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-28 18:05:19.000000 Abg-1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4983 2023-05-28 18:12:46.280024 Abg-1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3268 2023-05-28 18:05:19.000000 Abg-1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 18:12:46.280024 Abg-1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3052 2023-05-28 18:12:24.000000 Abg-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.309213 Abg-1.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-05 15:18:31.000000 Abg-1.2/Abg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/chat_status/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-05 15:18:31.000000 Abg-1.2/Abg/chat_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5273 2023-06-05 15:18:31.000000 Abg-1.2/Abg/chat_status/chat_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/conversation/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-05 15:18:31.000000 Abg-1.2/Abg/conversation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2023-06-05 15:18:31.000000 Abg-1.2/Abg/conversation/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      824 2023-06-05 15:18:31.000000 Abg-1.2/Abg/conversation/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/helpers/
+-rw-r--r--   0 root         (0) root         (0)      844 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/human_read.py
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/lock.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/pyro_progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/inline/
+-rw-r--r--   0 root         (0) root         (0)      280 2023-06-05 15:18:31.000000 Abg-1.2/Abg/inline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6245 2023-06-05 15:18:31.000000 Abg-1.2/Abg/inline/inline_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     4268 2023-06-05 15:18:31.000000 Abg-1.2/Abg/inline/inline_pagination_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2023-06-05 15:18:31.000000 Abg-1.2/Abg/inline/reply_keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/patch/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/patch/bound/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/bound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11748 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/bound/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.309213 Abg-1.2/Abg/patch/methods/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/methods/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/methods/send_as_file.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/methods/send_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5827 2023-06-05 15:18:56.000000 Abg-1.2/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      798 2023-06-05 15:18:56.000000 Abg-1.2/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 15:18:56.000000 Abg-1.2/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-05 15:18:56.000000 Abg-1.2/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5827 2023-06-05 15:18:56.309213 Abg-1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-06-05 15:18:31.000000 Abg-1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 15:18:56.309213 Abg-1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-05 15:18:31.000000 Abg-1.2/setup.py
```

### Comparing `Abg-1.1/Abg/conversation/conversation.py` & `Abg-1.2/Abg/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/conversation/errors.py` & `Abg-1.2/Abg/conversation/errors.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/helpers/__init__.py` & `Abg-1.2/Abg/helpers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 
 along with Abg.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 from .helpers import *
 from .http_helper import *
+from .human_read import *
 from .parser import *
 from .pyro_progress import *
```

### Comparing `Abg-1.1/Abg/helpers/helpers.py` & `Abg-1.2/Abg/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/helpers/http_helper.py` & `Abg-1.2/Abg/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/helpers/parser.py` & `Abg-1.2/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/helpers/pyro_progress.py` & `Abg-1.2/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/inline/inline_keyboard.py` & `Abg-1.2/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/inline/inline_pagination_keyboard.py` & `Abg-1.2/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/inline/reply_keyboard.py` & `Abg-1.2/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/patch/bound/message.py` & `Abg-1.2/Abg/patch/bound/message.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/patch/methods/edit_message_text.py` & `Abg-1.2/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/patch/methods/send_as_file.py` & `Abg-1.2/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg/patch/methods/send_message.py` & `Abg-1.2/Abg/patch/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `Abg-1.1/Abg.egg-info/PKG-INFO` & `Abg-1.2/Abg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,125 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 1.1
-Summary: add-on for pyrogram
+Version: 1.2
+Summary: pyrogram helpers / add-on for pyrogram
 Home-page: https://github.com/Abishnoi69
-Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
 License: MIT
+Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abg
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/wiki
+Description: # ᴀʙɢ-ᴘʏʀᴏ :->
+        
+        > sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
+        > 
+        • Conversation in pyrogram
+        
+        ```python
+          from Abg.conversation import Askclient
+          from pyrogram import Client, filters
+          
+          app = Client("my_account")
+          read = Askclient(app)
+        
+          @app.on_message(filters.command("start"))
+          async def start(c: app, m: Message):
+            answer = await read.ask(m, text)
+            if answer.text:
+             print(answer.text)
+            await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
+        
+          app.run()
+        ```
+        >
+        • Keyboards
+        
+        ```python
+        from Abg.inline import InlineKeyboard, InlineButton
+        
+        
+        keyboard = InlineKeyboard(row_width=3)
+        keyboard.add(
+            InlineButton('1', 'inline_keyboard:1'),
+            InlineButton('2', 'inline_keyboard:2'),
+            InlineButton('3', 'inline_keyboard:3'),
+            InlineButton('4', 'inline_keyboard:4'),
+            InlineButton('5', 'inline_keyboard:5'),
+            InlineButton('6', 'inline_keyboard:6'),
+            InlineButton('7', 'inline_keyboard:7')
+        )
+        ```
+        
+        #### Result
+        
+        <p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
+        
+        
+        ### ɪɴsᴛᴀʟʟɪɴɢ :->
+        
+        ```bash
+        pip3 install Abg
+        ```
+        
+        <details>
+        <summary><h3>
+        - <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/Abg/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/Abg/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴇxᴀᴍᴘʟᴇ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/Abg/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ :-></b>
+        </h3></summary>
+        <a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
+        </details>
+        
+        
+        ━━━━━━━━━━━━━━━━━━━━
+        ## ɴᴏᴛᴇ :->
+        
+        - This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
+        - My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
+        - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
+        
+        ━━━━━━━━━━━━━━━━━━━━ 
+         
+        <details>
+        <summary><h3>
+        - <b>ᴄʀᴇᴅɪᴛs :-></b>
+        </h3></summary>
+        
+        ➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
+        
+        ➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
+          
+        ➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
+        ━━━━━━━━━━━━━━━━━━━━
+        </details>
+        
 Keywords: telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -30,111 +134,7 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ᴀʙɢ-ᴘʏʀᴏ :->
-
-> sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
-> 
-• Conversation in pyrogram
-
-```python
-  from Abg.conversation import Askclient
-  from pyrogram import Client, filters
-  
-  app = Client("my_account")
-  read = Askclient(app)
-
-  @app.on_message(filters.command("start"))
-  async def start(c: app, m: Message):
-    answer = await read.ask(m, text)
-    if answer.text:
-     print(answer.text)
-    await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
-
-  app.run()
-```
->
-• Keyboards
-
-```python
-from Abg.inline import InlineKeyboard, InlineButton
-
-
-keyboard = InlineKeyboard(row_width=3)
-keyboard.add(
-    InlineButton('1', 'inline_keyboard:1'),
-    InlineButton('2', 'inline_keyboard:2'),
-    InlineButton('3', 'inline_keyboard:3'),
-    InlineButton('4', 'inline_keyboard:4'),
-    InlineButton('5', 'inline_keyboard:5'),
-    InlineButton('6', 'inline_keyboard:6'),
-    InlineButton('7', 'inline_keyboard:7')
-)
-```
-
-#### Result
-
-<p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
-
-
-### ɪɴsᴛᴀʟʟɪɴɢ :->
-
-```bash
-pip3 install Abg
-```
-
-<details>
-<summary><h3>
-- <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/Abg/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/Abg/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴇxᴀᴍᴘʟᴇ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/Abg/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ :-></b>
-</h3></summary>
-<a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
-</details>
-
-
-━━━━━━━━━━━━━━━━━━━━
-## ɴᴏᴛᴇ :->
-
-- This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
-- My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
-- ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
-
-━━━━━━━━━━━━━━━━━━━━ 
- 
-<details>
-<summary><h3>
-- <b>ᴄʀᴇᴅɪᴛs :-></b>
-</h3></summary>
-
-➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
-
-➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
-  
-➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
-━━━━━━━━━━━━━━━━━━━━
-</details>
```

#### html2text {}

```diff
@@ -1,31 +1,15 @@
-Metadata-Version: 2.1 Name: Abg Version: 1.1 Summary: add-on for pyrogram Home-
-page: https://github.com/Abishnoi69 Download-URL: https://github.com/
-Abishnoi69/Abg/releases/latest Author: Abishnoi1M Author-email:
-Abishnoi69@Abg.org License: MIT Project-URL: Tracker, https://github.com/
+Metadata-Version: 2.1 Name: Abg Version: 1.2 Summary: pyrogram helpers / add-on
+for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi1M
+Author-email: Abishnoi69@Abg.org License: MIT Download-URL: https://github.com/
+Abishnoi69/Abg/releases/latest Project-URL: Tracker, https://github.com/
 Abishnoi69/Abg/issues Project-URL: Community, https://t.me/Abg Project-URL:
 Source, https://github.com/Abishnoi69/Abg Project-URL: Documentation, https://
-github.com/Abishnoi69/Abg/wiki Keywords: telegram bot chat messenger mtproto
-api client library python conversation keyboard userbot patch Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: Implementation Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet
-Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Software Development :: Libraries :: Application Frameworks Requires-Python:
-~=3.7 Description-Content-Type: text/markdown License-File: LICENSE # á´ÊÉ¢-
-á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´
+github.com/Abishnoi69/Abg/wiki Description: # á´ÊÉ¢-á´ÊÊá´ :-> >
+sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´
 [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] > â¢ Conversation in pyrogram ```python
 from Abg.conversation import Askclient from pyrogram import Client, filters app
 = Client("my_account") read = Askclient(app) @app.on_message(filters.command
 ("start")) async def start(c: app, m: Message): answer = await read.ask(m,
 text) if answer.text: print(answer.text) await answer.reply("Éª É¢á´á´
 á´É´sá´¡á´Ê..") app.run() ``` > â¢ Keyboards ```python from Abg.inline
 import InlineKeyboard, InlineButton keyboard = InlineKeyboard(row_width=3)
@@ -52,8 +36,25 @@
 ExonMusicBot) - á´É´á´á´Ê Êá´ÊÊ â¡
 ââââââââââââââââââââ
 **** - á´Êá´á´Éªá´s :-> ****
 â¥ [ðð»ðððððð] â¬ [https://img.shields.io/badge/
 á´ÊÉªsÊÉ´á´Éª-90302f?logo=github] â¥ [ðÊÊá´É¢Êá´á´] â¬ [https://
 img.shields.io/badge/Pyrogram-90302f?logo=github] â¥ [ðá´Éªá´á´Ê] â¬
 [https://img.shields.io/badge/SPiDER-90302f?logo=github]
-ââââââââââââââââââââ
+ââââââââââââââââââââ  Keywords:
+telegram bot chat messenger mtproto api client library python conversation
+keyboard userbot patch Platform: UNKNOWN Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: Implementation Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Internet Classifier: Topic ::
+Communications Classifier: Topic :: Communications :: Chat Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Topic :: Software Development ::
+Libraries :: Application Frameworks Requires-Python: ~=3.7 Description-Content-
+Type: text/markdown
```

### Comparing `Abg-1.1/PKG-INFO` & `Abg-1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,125 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 1.1
-Summary: add-on for pyrogram
+Version: 1.2
+Summary: pyrogram helpers / add-on for pyrogram
 Home-page: https://github.com/Abishnoi69
-Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
 License: MIT
+Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abg
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/wiki
+Description: # ᴀʙɢ-ᴘʏʀᴏ :->
+        
+        > sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
+        > 
+        • Conversation in pyrogram
+        
+        ```python
+          from Abg.conversation import Askclient
+          from pyrogram import Client, filters
+          
+          app = Client("my_account")
+          read = Askclient(app)
+        
+          @app.on_message(filters.command("start"))
+          async def start(c: app, m: Message):
+            answer = await read.ask(m, text)
+            if answer.text:
+             print(answer.text)
+            await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
+        
+          app.run()
+        ```
+        >
+        • Keyboards
+        
+        ```python
+        from Abg.inline import InlineKeyboard, InlineButton
+        
+        
+        keyboard = InlineKeyboard(row_width=3)
+        keyboard.add(
+            InlineButton('1', 'inline_keyboard:1'),
+            InlineButton('2', 'inline_keyboard:2'),
+            InlineButton('3', 'inline_keyboard:3'),
+            InlineButton('4', 'inline_keyboard:4'),
+            InlineButton('5', 'inline_keyboard:5'),
+            InlineButton('6', 'inline_keyboard:6'),
+            InlineButton('7', 'inline_keyboard:7')
+        )
+        ```
+        
+        #### Result
+        
+        <p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
+        
+        
+        ### ɪɴsᴛᴀʟʟɪɴɢ :->
+        
+        ```bash
+        pip3 install Abg
+        ```
+        
+        <details>
+        <summary><h3>
+        - <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/Abg/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/Abg/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴇxᴀᴍᴘʟᴇ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/Abg/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ :-></b>
+        </h3></summary>
+        <a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
+        </details>
+        
+        
+        ━━━━━━━━━━━━━━━━━━━━
+        ## ɴᴏᴛᴇ :->
+        
+        - This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
+        - My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
+        - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
+        
+        ━━━━━━━━━━━━━━━━━━━━ 
+         
+        <details>
+        <summary><h3>
+        - <b>ᴄʀᴇᴅɪᴛs :-></b>
+        </h3></summary>
+        
+        ➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
+        
+        ➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
+          
+        ➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
+        ━━━━━━━━━━━━━━━━━━━━
+        </details>
+        
 Keywords: telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -30,111 +134,7 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ᴀʙɢ-ᴘʏʀᴏ :->
-
-> sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
-> 
-• Conversation in pyrogram
-
-```python
-  from Abg.conversation import Askclient
-  from pyrogram import Client, filters
-  
-  app = Client("my_account")
-  read = Askclient(app)
-
-  @app.on_message(filters.command("start"))
-  async def start(c: app, m: Message):
-    answer = await read.ask(m, text)
-    if answer.text:
-     print(answer.text)
-    await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
-
-  app.run()
-```
->
-• Keyboards
-
-```python
-from Abg.inline import InlineKeyboard, InlineButton
-
-
-keyboard = InlineKeyboard(row_width=3)
-keyboard.add(
-    InlineButton('1', 'inline_keyboard:1'),
-    InlineButton('2', 'inline_keyboard:2'),
-    InlineButton('3', 'inline_keyboard:3'),
-    InlineButton('4', 'inline_keyboard:4'),
-    InlineButton('5', 'inline_keyboard:5'),
-    InlineButton('6', 'inline_keyboard:6'),
-    InlineButton('7', 'inline_keyboard:7')
-)
-```
-
-#### Result
-
-<p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
-
-
-### ɪɴsᴛᴀʟʟɪɴɢ :->
-
-```bash
-pip3 install Abg
-```
-
-<details>
-<summary><h3>
-- <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/Abg/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/Abg/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴇxᴀᴍᴘʟᴇ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/Abg/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ :-></b>
-</h3></summary>
-<a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
-</details>
-
-
-━━━━━━━━━━━━━━━━━━━━
-## ɴᴏᴛᴇ :->
-
-- This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
-- My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
-- ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
-
-━━━━━━━━━━━━━━━━━━━━ 
- 
-<details>
-<summary><h3>
-- <b>ᴄʀᴇᴅɪᴛs :-></b>
-</h3></summary>
-
-➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
-
-➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
-  
-➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
-━━━━━━━━━━━━━━━━━━━━
-</details>
```

#### html2text {}

```diff
@@ -1,31 +1,15 @@
-Metadata-Version: 2.1 Name: Abg Version: 1.1 Summary: add-on for pyrogram Home-
-page: https://github.com/Abishnoi69 Download-URL: https://github.com/
-Abishnoi69/Abg/releases/latest Author: Abishnoi1M Author-email:
-Abishnoi69@Abg.org License: MIT Project-URL: Tracker, https://github.com/
+Metadata-Version: 2.1 Name: Abg Version: 1.2 Summary: pyrogram helpers / add-on
+for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi1M
+Author-email: Abishnoi69@Abg.org License: MIT Download-URL: https://github.com/
+Abishnoi69/Abg/releases/latest Project-URL: Tracker, https://github.com/
 Abishnoi69/Abg/issues Project-URL: Community, https://t.me/Abg Project-URL:
 Source, https://github.com/Abishnoi69/Abg Project-URL: Documentation, https://
-github.com/Abishnoi69/Abg/wiki Keywords: telegram bot chat messenger mtproto
-api client library python conversation keyboard userbot patch Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: Implementation Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet
-Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Software Development :: Libraries :: Application Frameworks Requires-Python:
-~=3.7 Description-Content-Type: text/markdown License-File: LICENSE # á´ÊÉ¢-
-á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´
+github.com/Abishnoi69/Abg/wiki Description: # á´ÊÉ¢-á´ÊÊá´ :-> >
+sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´
 [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] > â¢ Conversation in pyrogram ```python
 from Abg.conversation import Askclient from pyrogram import Client, filters app
 = Client("my_account") read = Askclient(app) @app.on_message(filters.command
 ("start")) async def start(c: app, m: Message): answer = await read.ask(m,
 text) if answer.text: print(answer.text) await answer.reply("Éª É¢á´á´
 á´É´sá´¡á´Ê..") app.run() ``` > â¢ Keyboards ```python from Abg.inline
 import InlineKeyboard, InlineButton keyboard = InlineKeyboard(row_width=3)
@@ -52,8 +36,25 @@
 ExonMusicBot) - á´É´á´á´Ê Êá´ÊÊ â¡
 ââââââââââââââââââââ
 **** - á´Êá´á´Éªá´s :-> ****
 â¥ [ðð»ðððððð] â¬ [https://img.shields.io/badge/
 á´ÊÉªsÊÉ´á´Éª-90302f?logo=github] â¥ [ðÊÊá´É¢Êá´á´] â¬ [https://
 img.shields.io/badge/Pyrogram-90302f?logo=github] â¥ [ðá´Éªá´á´Ê] â¬
 [https://img.shields.io/badge/SPiDER-90302f?logo=github]
-ââââââââââââââââââââ
+ââââââââââââââââââââ  Keywords:
+telegram bot chat messenger mtproto api client library python conversation
+keyboard userbot patch Platform: UNKNOWN Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: Implementation Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Internet Classifier: Topic ::
+Communications Classifier: Topic :: Communications :: Chat Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Topic :: Software Development ::
+Libraries :: Application Frameworks Requires-Python: ~=3.7 Description-Content-
+Type: text/markdown
```

### Comparing `Abg-1.1/README.md` & `Abg-1.2/README.md`

 * *Files identical despite different names*

### Comparing `Abg-1.1/setup.py` & `Abg-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="1.1",
-    description="add-on for pyrogram",
+    version="1.2",
+    description="pyrogram helpers / add-on for pyrogram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi1M",
     author_email="Abishnoi69@Abg.org", 
     license="MIT",
```

