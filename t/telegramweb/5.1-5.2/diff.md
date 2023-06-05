# Comparing `tmp/telegramweb-5.1.tar.gz` & `tmp/telegramweb-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-5.1.tar", last modified: Mon Jun  5 07:24:09 2023, max compression
+gzip compressed data, was "telegramweb-5.2.tar", last modified: Mon Jun  5 07:34:13 2023, max compression
```

## Comparing `telegramweb-5.1.tar` & `telegramweb-5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:24:09.919227 telegramweb-5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 07:23:53.000000 telegramweb-5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 07:23:53.000000 telegramweb-5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-06-05 07:24:09.919227 telegramweb-5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-05 07:23:53.000000 telegramweb-5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:24:09.919227 telegramweb-5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-05 07:23:53.000000 telegramweb-5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:24:09.919227 telegramweb-5.1/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 07:23:53.000000 telegramweb-5.1/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-05 07:23:53.000000 telegramweb-5.1/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-05 07:23:53.000000 telegramweb-5.1/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-05 07:23:53.000000 telegramweb-5.1/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-05 07:23:53.000000 telegramweb-5.1/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:24:09.919227 telegramweb-5.1/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-05 07:23:53.000000 telegramweb-5.1/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-06-05 07:23:53.000000 telegramweb-5.1/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-06-05 07:23:53.000000 telegramweb-5.1/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:24:09.919227 telegramweb-5.1/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-06-05 07:24:09.000000 telegramweb-5.1/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-05 07:24:09.000000 telegramweb-5.1/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:24:09.000000 telegramweb-5.1/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 07:24:09.000000 telegramweb-5.1/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 07:24:09.000000 telegramweb-5.1/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:34:13.407839 telegramweb-5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 07:33:51.000000 telegramweb-5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 07:33:51.000000 telegramweb-5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-06-05 07:34:13.407839 telegramweb-5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-05 07:33:51.000000 telegramweb-5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:34:13.407839 telegramweb-5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-05 07:33:51.000000 telegramweb-5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:34:13.403839 telegramweb-5.2/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 07:33:51.000000 telegramweb-5.2/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-05 07:33:51.000000 telegramweb-5.2/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-05 07:33:51.000000 telegramweb-5.2/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-05 07:33:51.000000 telegramweb-5.2/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-05 07:33:51.000000 telegramweb-5.2/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:34:13.403839 telegramweb-5.2/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-05 07:33:51.000000 telegramweb-5.2/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-06-05 07:33:51.000000 telegramweb-5.2/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-06-05 07:33:51.000000 telegramweb-5.2/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:34:13.407839 telegramweb-5.2/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-06-05 07:34:13.000000 telegramweb-5.2/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-05 07:34:13.000000 telegramweb-5.2/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:34:13.000000 telegramweb-5.2/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 07:34:13.000000 telegramweb-5.2/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 07:34:13.000000 telegramweb-5.2/telegramweb.egg-info/top_level.txt
```

### Comparing `telegramweb-5.1/LICENSE` & `telegramweb-5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-5.1/PKG-INFO` & `telegramweb-5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 5.1
+Version: 5.2
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Description: <h1 align="center">
           <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telegramweb Version: 5.1 Summary: Python package
+Metadata-Version: 2.1 Name: telegramweb Version: 5.2 Summary: Python package
 for automatically fetching and pushing news by Telegram. Home-page: https://
 github.com/craziks-creator/telegram-web Author: craziks Author-email:
 chandrashekharpanday07@gmail.com License: MIT Description:
                             ****** [Telegram-news]
                                  Telegram-news
                                      ******
   Python package for automatically fetching and pushing news by Telegram. [!
```

### Comparing `telegramweb-5.1/README.md` & `telegramweb-5.2/README.md`

 * *Files identical despite different names*

### Comparing `telegramweb-5.1/setup.py` & `telegramweb-5.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='5.1',
+    version='5.2',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `telegramweb-5.1/telegram_news/__init__.py` & `telegramweb-5.2/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.1/telegram_news/constant.py` & `telegramweb-5.2/telegram_news/constant.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.1/telegram_news/displaypolicy.py` & `telegramweb-5.2/telegram_news/displaypolicy.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import re
 
 
 MAXLEN = 4096
 
 
-def default_policy(item, self, new_table_name, max_len=1000, max_par_num=40):
+def default_policy(item, max_len=1000, max_par_num=40):
     """
     Generate formatted message from item, the default way.
 
     :param item: item dict.
     :param max_len: max message length.
     :param max_par_num: max paragraph number.
     :return: formatted forward message, parse mode (HTML or Markdown), disable web page preview flag.
@@ -53,47 +53,45 @@
         po += item['time']
         po += '\n'
 
     if item['source']:
         po += '[' + item['source'] + ']' + ' '
 
     if item['link']:
-        po += '<a href=\"' + item['link'] + '\">LATEST UPDATE FROM \"' + new_table_name + '\" SECTION</a>'
+        po += '<a href=\"' + item['link'] + '\">LATEST UPDATE FROM OFFICIAL WEBSITE</a>'
 
     po = po.replace('<br>', "")
 
     if len(po) > MAXLEN:
         return "Too long message!\n" + item['id'], parse_mode, disable_web_page_preview
 
     return {
         'text': po,
         'parse_mode': parse_mode,
         'disable_web_page_preview': disable_web_page_preview
     }
 
 
-def best_effort_display_policy(item, self, new_table_name, tag='', max_len=1000, max_par_num=40, suffix='...'):
+def best_effort_display_policy(item, max_len=1000, max_par_num=40, suffix='...'):
     """
     Display as more paragraphs as possible.
     If over max_len, end with suffix.
 
     :param item: item dict.
     :param max_len: max message length.
     :param max_par_num: max paragraph number.
     :param suffix: used for indicating an omission.
     :return: formatted forward message, parse mode (HTML or Markdown), disable web page preview flag.
     """
-    self._table_name = new_table_name
-    rows = self._db.execute("SELECT COUNT(*) FROM information_schema.tables WHERE table_name = :new_table_name ;",
-                                {"new_table_name": new_table_name})
+   
     parse_mode = 'html'
     disable_web_page_preview = 'False'
 
     full = '<b>' + item['title'] + '</b>\n\n' + item['paragraphs'] + item['time'] + '\n' + \
-           '[' + item['source'] + ']' + '<a href=\"' + item['link'] + '\">LATEST UPDATE FROM \"' + new_table_name + '\" SECTION</a>' + ' '
+           '[' + item['source'] + ']' + '<a href=\"' + item['link'] + '\">LATEST UPDATE FROM OFFICIAL WEBSITE</a>' + ' '
 
     # po is the text we want to post
     po = ""
     if item['title']:
         po += '<b>' + item['title'] + '</b>'
         po += '\n\n'
 
@@ -123,15 +121,15 @@
         po += item['time']
         po += '\n'
 
     if item['source']:
         po += '[' + item['source'] + ']' + ' '
 
     if item['link']:
-        po += '<a href=\"' + item['link'] + '\">LATEST UPDATE FROM \"' + new_table_name + '\" SECTION</a>'
+        po += '<a href=\"' + item['link'] + '\">LATEST UPDATE FROM OFFICIAL WEBSITE</a>'
 
     po = po.replace('<br>', "")
 
     if len(po) > 4096:
         return "Too long message!\n" + item['id'], parse_mode, disable_web_page_preview
 
     return {
```

### Comparing `telegramweb-5.1/telegram_news/ratelimit.py` & `telegramweb-5.2/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.1/telegram_news/template/common.py` & `telegramweb-5.2/telegram_news/template/common.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.1/telegram_news/utils.py` & `telegramweb-5.2/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.1/telegramweb.egg-info/PKG-INFO` & `telegramweb-5.2/telegramweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 5.1
+Version: 5.2
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Description: <h1 align="center">
           <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telegramweb Version: 5.1 Summary: Python package
+Metadata-Version: 2.1 Name: telegramweb Version: 5.2 Summary: Python package
 for automatically fetching and pushing news by Telegram. Home-page: https://
 github.com/craziks-creator/telegram-web Author: craziks Author-email:
 chandrashekharpanday07@gmail.com License: MIT Description:
                             ****** [Telegram-news]
                                  Telegram-news
                                      ******
   Python package for automatically fetching and pushing news by Telegram. [!
```

