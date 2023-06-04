# Comparing `tmp/FunPayAPI-1.0.9.tar.gz` & `tmp/FunPayAPI-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FunPayAPI-1.0.9.tar", last modified: Sat Jun  3 08:08:18 2023, max compression
+gzip compressed data, was "FunPayAPI-1.1.0.tar", last modified: Sun Jun  4 23:40:37 2023, max compression
```

## Comparing `FunPayAPI-1.0.9.tar` & `FunPayAPI-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 08:08:18.674287 FunPayAPI-1.0.9/
-drwxrwxrwx   0        0        0        0 2023-06-03 08:08:18.643287 FunPayAPI-1.0.9/FunPayAPI/
--rw-rw-rw-   0        0        0      162 2023-05-15 12:08:20.000000 FunPayAPI-1.0.9/FunPayAPI/__init__.py
--rw-rw-rw-   0        0        0    65511 2023-06-03 08:01:41.000000 FunPayAPI-1.0.9/FunPayAPI/account.py
-drwxrwxrwx   0        0        0        0 2023-06-03 08:08:18.668286 FunPayAPI-1.0.9/FunPayAPI/common/
--rw-rw-rw-   0        0        0        0 2023-05-12 17:46:25.000000 FunPayAPI-1.0.9/FunPayAPI/common/__init__.py
--rw-rw-rw-   0        0        0     4842 2023-05-14 16:49:23.000000 FunPayAPI-1.0.9/FunPayAPI/common/enums.py
--rw-rw-rw-   0        0        0     7842 2023-05-14 23:54:13.000000 FunPayAPI-1.0.9/FunPayAPI/common/exceptions.py
--rw-rw-rw-   0        0        0     8922 2023-05-19 09:07:17.000000 FunPayAPI-1.0.9/FunPayAPI/common/utils.py
--rw-rw-rw-   0        0        0    38978 2023-05-19 09:36:22.000000 FunPayAPI-1.0.9/FunPayAPI/types.py
-drwxrwxrwx   0        0        0        0 2023-06-03 08:08:18.673286 FunPayAPI-1.0.9/FunPayAPI/updater/
--rw-rw-rw-   0        0        0        0 2023-05-12 17:46:18.000000 FunPayAPI-1.0.9/FunPayAPI/updater/__init__.py
--rw-rw-rw-   0        0        0     8216 2023-05-11 19:12:41.000000 FunPayAPI-1.0.9/FunPayAPI/updater/events.py
--rw-rw-rw-   0        0        0    22148 2023-06-03 06:55:19.000000 FunPayAPI-1.0.9/FunPayAPI/updater/runner.py
-drwxrwxrwx   0        0        0        0 2023-06-03 08:08:18.657286 FunPayAPI-1.0.9/FunPayAPI.egg-info/
--rw-rw-rw-   0        0        0     3602 2023-06-03 08:08:18.000000 FunPayAPI-1.0.9/FunPayAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-03 08:08:18.000000 FunPayAPI-1.0.9/FunPayAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 08:08:18.000000 FunPayAPI-1.0.9/FunPayAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-03 08:08:18.000000 FunPayAPI-1.0.9/FunPayAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-03 08:08:18.000000 FunPayAPI-1.0.9/FunPayAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35801 2023-05-11 21:13:41.000000 FunPayAPI-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     3602 2023-06-03 08:08:18.673286 FunPayAPI-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3011 2023-05-12 11:49:15.000000 FunPayAPI-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 08:08:18.674287 FunPayAPI-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-06-03 08:07:47.000000 FunPayAPI-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 23:40:37.272549 FunPayAPI-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-04 23:40:37.238549 FunPayAPI-1.1.0/FunPayAPI/
+-rw-rw-rw-   0        0        0      162 2023-05-15 12:08:20.000000 FunPayAPI-1.1.0/FunPayAPI/__init__.py
+-rw-rw-rw-   0        0        0    65939 2023-06-04 23:35:41.000000 FunPayAPI-1.1.0/FunPayAPI/account.py
+drwxrwxrwx   0        0        0        0 2023-06-04 23:40:37.265549 FunPayAPI-1.1.0/FunPayAPI/common/
+-rw-rw-rw-   0        0        0        0 2023-05-12 17:46:25.000000 FunPayAPI-1.1.0/FunPayAPI/common/__init__.py
+-rw-rw-rw-   0        0        0     4842 2023-05-14 16:49:23.000000 FunPayAPI-1.1.0/FunPayAPI/common/enums.py
+-rw-rw-rw-   0        0        0     7842 2023-05-14 23:54:13.000000 FunPayAPI-1.1.0/FunPayAPI/common/exceptions.py
+-rw-rw-rw-   0        0        0     8922 2023-05-19 09:07:17.000000 FunPayAPI-1.1.0/FunPayAPI/common/utils.py
+-rw-rw-rw-   0        0        0    39128 2023-06-04 23:04:46.000000 FunPayAPI-1.1.0/FunPayAPI/types.py
+drwxrwxrwx   0        0        0        0 2023-06-04 23:40:37.271549 FunPayAPI-1.1.0/FunPayAPI/updater/
+-rw-rw-rw-   0        0        0        0 2023-05-12 17:46:18.000000 FunPayAPI-1.1.0/FunPayAPI/updater/__init__.py
+-rw-rw-rw-   0        0        0     8216 2023-05-11 19:12:41.000000 FunPayAPI-1.1.0/FunPayAPI/updater/events.py
+-rw-rw-rw-   0        0        0    22148 2023-06-03 08:09:27.000000 FunPayAPI-1.1.0/FunPayAPI/updater/runner.py
+drwxrwxrwx   0        0        0        0 2023-06-04 23:40:37.252549 FunPayAPI-1.1.0/FunPayAPI.egg-info/
+-rw-rw-rw-   0        0        0     3602 2023-06-04 23:40:37.000000 FunPayAPI-1.1.0/FunPayAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-04 23:40:37.000000 FunPayAPI-1.1.0/FunPayAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 23:40:37.000000 FunPayAPI-1.1.0/FunPayAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-04 23:40:37.000000 FunPayAPI-1.1.0/FunPayAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 23:40:37.000000 FunPayAPI-1.1.0/FunPayAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35801 2023-05-11 21:13:41.000000 FunPayAPI-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3602 2023-06-04 23:40:37.271549 FunPayAPI-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3011 2023-05-12 11:49:15.000000 FunPayAPI-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 23:40:37.272549 FunPayAPI-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      928 2023-06-04 23:40:15.000000 FunPayAPI-1.1.0/setup.py
```

### Comparing `FunPayAPI-1.0.9/FunPayAPI/account.py` & `FunPayAPI-1.1.0/FunPayAPI/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 from datetime import datetime, timedelta
 import requests
 import logging
 import random
 import string
 import json
 import time
+import re
 
 from . import types
 from .common import exceptions, utils, enums
 
 
 logger = logging.getLogger("FunPayAPI.account")
+PRIVATE_CHAT_ID_RE = re.compile(r"users-\d+-\d+$")
 
 
 class Account:
     """
     Класс для управления аккаунтом FunPay.
 
     :param golden_key: токен (golden_key) аккаунта.
@@ -1348,60 +1350,63 @@
             self.__sorted_categories[game_id] = game_obj
 
     def __parse_messages(self, json_messages: dict, chat_id: int | str,
                          interlocutor_id: Optional[int] = None, interlocutor_username: Optional[str] = None,
                          from_id: int = 0) -> list[types.Message]:
         messages = []
         ids = {self.id: self.username, 0: "FunPay"}
+        badges = {}
         if interlocutor_id is not None:
             ids[interlocutor_id] = interlocutor_username
 
         for i in json_messages:
             if i["id"] < from_id:
                 continue
             author_id = i["author"]
             parser = BeautifulSoup(i["html"], "html.parser")
-            # Если ник написавшего неизвестен, но он есть в HTML-коде сообщения
-            if ids.get(author_id) is None and (author_div := parser.find("div", {"class": "media-user-name"})):
-                author = author_div.find("a").text.strip()
-                ids[author_id] = author
-                if isinstance(chat_id, int) and author_id == interlocutor_id and not interlocutor_username:
-                    interlocutor_username = author
-                    ids[interlocutor_id] = interlocutor_username
 
-            if isinstance(chat_id, int) and (image_link := parser.find("a", {"class": "chat-img-link"})):
+            # Если ник или бейдж написавшего неизвестен, но есть блок с данными об авторе сообщения
+            if None in [ids.get(author_id), badges.get(author_id)] and (author_div := parser.find("div", {"class": "media-user-name"})):
+                if badges.get(author_id) is None:
+                    badge = author_div.find("span")
+                    badges[author_id] = badge.text if badge else 0
+                if ids.get(author_id) is None:
+                    author = author_div.find("a").text.strip()
+                    ids[author_id] = author
+                    if self.chat_id_private(chat_id) and author_id == interlocutor_id and not interlocutor_username:
+                        interlocutor_username = author
+                        ids[interlocutor_id] = interlocutor_username
+
+            if self.chat_id_private and (image_link := parser.find("a", {"class": "chat-img-link"})):
                 image_link = image_link.get("href")
                 message_text = None
             else:
                 image_link = None
                 if author_id == 0:
                     message_text = parser.find("div", {"class": "alert alert-with-icon alert-info"}).text.strip()
                 else:
                     message_text = parser.find("div", {"class": "message-text"}).text
 
             by_bot = False
-            if message_text.startswith(self.__bot_character):
+            if not image_link and message_text.startswith(self.__bot_character):
                 message_text = message_text.replace(self.__bot_character, "", 1)
                 by_bot = True
 
             message_obj = types.Message(i["id"], message_text, chat_id, interlocutor_username,
                                         None, author_id, i["html"], image_link, determine_msg_type=False)
             message_obj.by_bot = by_bot
-
-            if author_id != 0:
-                message_obj.type = types.MessageTypes.NON_SYSTEM
-            else:
-                message_obj.type = message_obj.get_message_type()
+            message_obj.type = types.MessageTypes.NON_SYSTEM if author_id != 0 else message_obj.get_message_type()
             messages.append(message_obj)
 
-        # todo
-        debug_text = ""
         for i in messages:
             i.author = ids.get(i.author_id)
             i.chat_name = interlocutor_username
-            debug_text += f"{i.author} | {i.author_id} | {str(i)[:20]} /\\"
-        logger.debug(debug_text)
+            i.badge = badges.get(i.author_id) if badges.get(i.author_id) != 0 else None
         return messages
 
+    @staticmethod
+    def chat_id_private(chat_id: int | str):
+        return isinstance(chat_id, int) or PRIVATE_CHAT_ID_RE.fullmatch(chat_id)
+
     @property
     def bot_character(self) -> str:
         return self.__bot_character
```

### Comparing `FunPayAPI-1.0.9/FunPayAPI/common/enums.py` & `FunPayAPI-1.1.0/FunPayAPI/common/enums.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.9/FunPayAPI/common/exceptions.py` & `FunPayAPI-1.1.0/FunPayAPI/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.9/FunPayAPI/common/utils.py` & `FunPayAPI-1.1.0/FunPayAPI/common/utils.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.9/FunPayAPI/types.py` & `FunPayAPI-1.1.0/FunPayAPI/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     :type image_link: :obj:`str` or :obj:`None`, опционально
 
     :param determine_msg_type: определять ли тип сообщения.
     :type determine_msg_type: :obj:`bool`, опционально
     """
     def __init__(self, id_: int, text: str | None, chat_id: int | str, chat_name: str | None,
                  author: str | None, author_id: int, html: str,
-                 image_link: str | None = None, determine_msg_type: bool = True):
+                 image_link: str | None = None, determine_msg_type: bool = True, badge_text: Optional[str] = None):
         self.id: int = id_
         """ID сообщения."""
         self.text: str | None = text
         """Текст сообщения."""
         self.chat_id: int | str = chat_id
         """ID чата."""
         self.chat_name: str | None = chat_name
@@ -180,14 +180,16 @@
         """ID автора сообщения."""
         self.html: str = html
         """HTML-код сообщения."""
         self.image_link: str | None = image_link
         """Ссылка на изображение в сообщении (если оно есть)."""
         self.by_bot: bool = False
         """Отправлено ли сообщение с помощью :meth:`FunPayAPI.Account.send_message`?"""
+        self.badge: str | None = badge_text
+        """Текст бэйджика тех. поддержки."""
 
     def get_message_type(self) -> MessageTypes:
         """
         Определяет тип сообщения на основе регулярных выражений из MessageTypesRes.
 
         Внимание! Данный способ определения типа сообщения не является 100% правильным, т.к. он основан на сравнении с
         регулярными выражениями. Возможно ложное "срабатывание", если пользователь напишет "поддельное" сообщение,
```

### Comparing `FunPayAPI-1.0.9/FunPayAPI/updater/events.py` & `FunPayAPI-1.1.0/FunPayAPI/updater/events.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.9/FunPayAPI/updater/runner.py` & `FunPayAPI-1.1.0/FunPayAPI/updater/runner.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.9/FunPayAPI.egg-info/PKG-INFO` & `FunPayAPI-1.1.0/FunPayAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: FunPayAPI
-Version: 1.0.9
+Version: 1.1.0
 Summary: Прослойка между FunPayAPI и клиентом.
 Home-page: https://github.com/woopertail/FunPayAPI
 Author: Woopertail
 Author-email: woopertail@gmail.com
 License: GPL3
 Keywords: funpay bot api tools
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://i.ibb.co/tJKk0QS/Fun-Pay-API-darkmode.png">
 <h1 align="center">FunPay API</h1>
 <h4 align="center">Библиотека для легкого написания ботов FunPay.</h4>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.9 Summary:
+Metadata-Version: 2.1 Name: FunPayAPI Version: 1.1.0 Summary:
 ÐÑÐ¾ÑÐ»Ð¾Ð¹ÐºÐ° Ð¼ÐµÐ¶Ð´Ñ FunPayAPI Ð¸ ÐºÐ»Ð¸ÐµÐ½ÑÐ¾Ð¼. Home-page: https:/
 /github.com/woopertail/FunPayAPI Author: Woopertail Author-email:
 woopertail@gmail.com License: GPL3 Keywords: funpay bot api tools Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown License-File: LICENSE [https://
 i.ibb.co/tJKk0QS/Fun-Pay-API-darkmode.png]
                            ****** FunPay API ******
  *** ÐÐ¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð´Ð»Ñ Ð»ÐµÐ³ÐºÐ¾Ð³Ð¾ Ð½Ð°Ð¿Ð¸ÑÐ°Ð½Ð¸Ñ Ð±Ð¾ÑÐ¾Ð²
                                   FunPay. ***
                     ****** ÐÐ°Ð¶Ð½ÑÐµ ÑÑÑÐ»ÐºÐ¸ ******
                               *** Telegram_ÑÐ°Ñ
```

### Comparing `FunPayAPI-1.0.9/LICENSE` & `FunPayAPI-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.9/PKG-INFO` & `FunPayAPI-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: FunPayAPI
-Version: 1.0.9
+Version: 1.1.0
 Summary: Прослойка между FunPayAPI и клиентом.
 Home-page: https://github.com/woopertail/FunPayAPI
 Author: Woopertail
 Author-email: woopertail@gmail.com
 License: GPL3
 Keywords: funpay bot api tools
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://i.ibb.co/tJKk0QS/Fun-Pay-API-darkmode.png">
 <h1 align="center">FunPay API</h1>
 <h4 align="center">Библиотека для легкого написания ботов FunPay.</h4>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.9 Summary:
+Metadata-Version: 2.1 Name: FunPayAPI Version: 1.1.0 Summary:
 ÐÑÐ¾ÑÐ»Ð¾Ð¹ÐºÐ° Ð¼ÐµÐ¶Ð´Ñ FunPayAPI Ð¸ ÐºÐ»Ð¸ÐµÐ½ÑÐ¾Ð¼. Home-page: https:/
 /github.com/woopertail/FunPayAPI Author: Woopertail Author-email:
 woopertail@gmail.com License: GPL3 Keywords: funpay bot api tools Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown License-File: LICENSE [https://
 i.ibb.co/tJKk0QS/Fun-Pay-API-darkmode.png]
                            ****** FunPay API ******
  *** ÐÐ¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð´Ð»Ñ Ð»ÐµÐ³ÐºÐ¾Ð³Ð¾ Ð½Ð°Ð¿Ð¸ÑÐ°Ð½Ð¸Ñ Ð±Ð¾ÑÐ¾Ð²
                                   FunPay. ***
                     ****** ÐÐ°Ð¶Ð½ÑÐµ ÑÑÑÐ»ÐºÐ¸ ******
                               *** Telegram_ÑÐ°Ñ
```

### Comparing `FunPayAPI-1.0.9/README.md` & `FunPayAPI-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.9/setup.py` & `FunPayAPI-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_desc = f.read()
 
 
 setup(name='FunPayAPI',
-      version="1.0.9",
+      version="1.1.0",
       description='Прослойка между FunPayAPI и клиентом.',
       long_description=long_desc,
       long_description_content_type="text/markdown",
       author='Woopertail',
       author_email='woopertail@gmail.com',
       url='https://github.com/woopertail/FunPayAPI',
       packages=find_packages("."),
       license='GPL3',
       keywords='funpay bot api tools',
       install_requires=['requests==2.28.1', 'beautifulsoup4', 'requests_toolbelt==0.10.1'],
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Programming Language :: Python :: 3',
           'Environment :: Console',
-          'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
+          'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
       ]
 )
```

