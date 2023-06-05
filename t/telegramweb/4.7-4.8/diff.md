# Comparing `tmp/telegramweb-4.7.tar.gz` & `tmp/telegramweb-4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-4.7.tar", last modified: Mon Jun  5 06:05:34 2023, max compression
+gzip compressed data, was "telegramweb-4.8.tar", last modified: Mon Jun  5 06:20:32 2023, max compression
```

## Comparing `telegramweb-4.7.tar` & `telegramweb-4.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:05:34.558307 telegramweb-4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 06:05:18.000000 telegramweb-4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 06:05:18.000000 telegramweb-4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-06-05 06:05:34.558307 telegramweb-4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-05 06:05:18.000000 telegramweb-4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 06:05:34.558307 telegramweb-4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-05 06:05:18.000000 telegramweb-4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:05:34.558307 telegramweb-4.7/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 06:05:18.000000 telegramweb-4.7/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-05 06:05:18.000000 telegramweb-4.7/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-05 06:05:18.000000 telegramweb-4.7/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-05 06:05:18.000000 telegramweb-4.7/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-05 06:05:18.000000 telegramweb-4.7/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:05:34.558307 telegramweb-4.7/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-05 06:05:18.000000 telegramweb-4.7/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-06-05 06:05:18.000000 telegramweb-4.7/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-06-05 06:05:18.000000 telegramweb-4.7/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:05:34.558307 telegramweb-4.7/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-06-05 06:05:34.000000 telegramweb-4.7/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-05 06:05:34.000000 telegramweb-4.7/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:05:34.000000 telegramweb-4.7/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 06:05:34.000000 telegramweb-4.7/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 06:05:34.000000 telegramweb-4.7/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:20:32.777333 telegramweb-4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 06:20:17.000000 telegramweb-4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 06:20:17.000000 telegramweb-4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-06-05 06:20:32.777333 telegramweb-4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-05 06:20:17.000000 telegramweb-4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 06:20:32.777333 telegramweb-4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-05 06:20:17.000000 telegramweb-4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:20:32.773333 telegramweb-4.8/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 06:20:17.000000 telegramweb-4.8/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-05 06:20:17.000000 telegramweb-4.8/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-05 06:20:17.000000 telegramweb-4.8/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-05 06:20:17.000000 telegramweb-4.8/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-05 06:20:17.000000 telegramweb-4.8/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:20:32.773333 telegramweb-4.8/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-05 06:20:17.000000 telegramweb-4.8/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-06-05 06:20:17.000000 telegramweb-4.8/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-06-05 06:20:17.000000 telegramweb-4.8/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:20:32.773333 telegramweb-4.8/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-06-05 06:20:32.000000 telegramweb-4.8/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-05 06:20:32.000000 telegramweb-4.8/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:20:32.000000 telegramweb-4.8/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 06:20:32.000000 telegramweb-4.8/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 06:20:32.000000 telegramweb-4.8/telegramweb.egg-info/top_level.txt
```

### Comparing `telegramweb-4.7/LICENSE` & `telegramweb-4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-4.7/PKG-INFO` & `telegramweb-4.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: telegramweb
-Version: 4.7
-Summary: Python package for automatically fetching and pushing news by Telegram.
-Home-page: https://github.com/craziks-creator/telegram-web
-Author: craziks
-Author-email: chandrashekharpanday07@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Education
-Classifier: Topic :: Office/Business :: News/Diary
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
   <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
   <br>Telegram-news<br>
 </h1>
 
 <div align="center">
 
@@ -285,9 +261,7 @@
 Feel free to contact with me if you have any question. Also welcome any contribute.
 
 If you build a channel by this, don't forget to share that good news with us!
 
 ## License
 
 Licensed under the MIT License.
-
-
```

### Comparing `telegramweb-4.7/README.md` & `telegramweb-4.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,588 +1,778 @@
-00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
-00000010: 7222 3e0a 2020 3c69 6d67 2073 7263 3d22  r">.  <img src="
-00000020: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00000030: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00000040: 6d2f 4553 575a 592f 7465 6c65 6772 616d  m/ESWZY/telegram
-00000050: 2d6e 6577 732f 6d61 7374 6572 2f64 6f63  -news/master/doc
-00000060: 732f 696d 6167 6573 2f62 616e 6e65 722e  s/images/banner.
-00000070: 706e 6722 2061 6c74 3d22 5465 6c65 6772  png" alt="Telegr
-00000080: 616d 2d6e 6577 7322 3e0a 2020 3c62 723e  am-news">.  <br>
-00000090: 5465 6c65 6772 616d 2d6e 6577 733c 6272  Telegram-news<br
-000000a0: 3e0a 3c2f 6831 3e0a 0a3c 6469 7620 616c  >.</h1>..<div al
-000000b0: 6967 6e3d 2263 656e 7465 7222 3e0a 0a50  ign="center">..P
-000000c0: 7974 686f 6e20 7061 636b 6167 6520 666f  ython package fo
-000000d0: 7220 6175 746f 6d61 7469 6361 6c6c 7920  r automatically 
-000000e0: 6665 7463 6869 6e67 2061 6e64 2070 7573  fetching and pus
-000000f0: 6869 6e67 206e 6577 7320 6279 2054 656c  hing news by Tel
-00000100: 6567 7261 6d2e 0a0a 5b21 5b50 7950 495d  egram...[![PyPI]
-00000110: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000120: 656c 6473 2e69 6f2f 7079 7069 2f76 2f74  elds.io/pypi/v/t
-00000130: 656c 6567 7261 6d2d 6e65 7773 295d 2868  elegram-news)](h
-00000140: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000150: 7072 6f6a 6563 742f 7465 6c65 6772 616d  project/telegram
-00000160: 2d6e 6577 732f 290a 215b 5079 5049 202d  -news/).![PyPI -
-00000170: 2050 7974 686f 6e20 5665 7273 696f 6e5d   Python Version]
-00000180: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000190: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
-000001a0: 6572 7369 6f6e 732f 7465 6c65 6772 616d  ersions/telegram
-000001b0: 2d6e 6577 733f 6c6f 676f 3d70 7974 686f  -news?logo=pytho
-000001c0: 6e29 0a5b 215b 4c69 6365 6e73 655d 2868  n).[![License](h
-000001d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000001e0: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
-000001f0: 656e 7365 2f45 5357 5a59 2f74 656c 6567  ense/ESWZY/teleg
-00000200: 7261 6d2d 6e65 7773 295d 2868 7474 7073  ram-news)](https
-00000210: 3a2f 2f67 6974 6875 622e 636f 6d2f 4553  ://github.com/ES
-00000220: 575a 592f 7465 6c65 6772 616d 2d6e 6577  WZY/telegram-new
-00000230: 732f 626c 6f62 2f6d 6173 7465 722f 4c49  s/blob/master/LI
-00000240: 4345 4e53 4529 0a21 5b50 7950 4920 2d20  CENSE).![PyPI - 
-00000250: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
-00000260: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000270: 6f2f 7079 7069 2f64 6d2f 7465 6c65 6772  o/pypi/dm/telegr
-00000280: 616d 2d6e 6577 7329 0a0a 5b21 5b42 7569  am-news)..[![Bui
-00000290: 6c64 2053 7461 7475 735d 2868 7474 7073  ld Status](https
-000002a0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000002b0: 6f2f 7472 6176 6973 2f45 5357 5a59 2f74  o/travis/ESWZY/t
-000002c0: 656c 6567 7261 6d2d 6e65 7773 2f6d 6173  elegram-news/mas
-000002d0: 7465 723f 6c6f 676f 3d74 7261 7669 7329  ter?logo=travis)
-000002e0: 5d28 6874 7470 733a 2f2f 7472 6176 6973  ](https://travis
-000002f0: 2d63 692e 6f72 672f 4553 575a 592f 7465  -ci.org/ESWZY/te
-00000300: 6c65 6772 616d 2d6e 6577 7329 0a5b 215b  legram-news).[![
-00000310: 436f 6461 6379 2042 6164 6765 5d28 6874  Codacy Badge](ht
-00000320: 7470 733a 2f2f 6170 692e 636f 6461 6379  tps://api.codacy
-00000330: 2e63 6f6d 2f70 726f 6a65 6374 2f62 6164  .com/project/bad
-00000340: 6765 2f47 7261 6465 2f33 6330 3766 6564  ge/Grade/3c07fed
-00000350: 3532 3564 6134 3265 3839 6464 3364 3033  525da42e89dd3d03
-00000360: 3736 3435 3762 3464 3229 5d28 6874 7470  76457b4d2)](http
-00000370: 733a 2f2f 6170 702e 636f 6461 6379 2e63  s://app.codacy.c
-00000380: 6f6d 2f6d 616e 7561 6c2f 4553 575a 592f  om/manual/ESWZY/
-00000390: 7465 6c65 6772 616d 2d6e 6577 733f 7574  telegram-news?ut
-000003a0: 6d5f 736f 7572 6365 3d67 6974 6875 622e  m_source=github.
-000003b0: 636f 6d26 7574 6d5f 6d65 6469 756d 3d72  com&utm_medium=r
-000003c0: 6566 6572 7261 6c26 7574 6d5f 636f 6e74  eferral&utm_cont
-000003d0: 656e 743d 4553 575a 592f 7465 6c65 6772  ent=ESWZY/telegr
-000003e0: 616d 2d6e 6577 7326 7574 6d5f 6361 6d70  am-news&utm_camp
-000003f0: 6169 676e 3d42 6164 6765 5f47 7261 6465  aign=Badge_Grade
-00000400: 5f44 6173 6862 6f61 7264 290a 215b 4c61  _Dashboard).![La
-00000410: 7374 2063 6f6d 6d69 745d 2868 7474 7073  st commit](https
-00000420: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000430: 6f2f 6769 7468 7562 2f6c 6173 742d 636f  o/github/last-co
-00000440: 6d6d 6974 2f45 5357 5a59 2f74 656c 6567  mmit/ESWZY/teleg
-00000450: 7261 6d2d 6e65 7773 290a 5b21 5b68 7474  ram-news).[![htt
-00000460: 7073 3a2f 2f74 2e6d 652f 6573 777a 795d  ps://t.me/eswzy]
-00000470: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000480: 656c 6473 2e69 6f2f 6261 6467 652f 5465  elds.io/badge/Te
-00000490: 6c65 6772 616d 2d45 5357 5a59 2d62 6c75  legram-ESWZY-blu
-000004a0: 652e 7376 673f 6c6f 676f 3d74 656c 6567  e.svg?logo=teleg
-000004b0: 7261 6d29 5d28 6874 7470 733a 2f2f 742e  ram)](https://t.
-000004c0: 6d65 2f65 7377 7a79 290a 0a3c 2f64 6976  me/eswzy)..</div
-000004d0: 3e0a 0a23 2320 496e 7472 6f64 7563 7469  >..## Introducti
-000004e0: 6f6e 0a0a 5468 6973 2069 7320 6120 6561  on..This is a ea
-000004f0: 7379 2d74 6f2d 6c65 6172 6e2c 2066 6c65  sy-to-learn, fle
-00000500: 7869 626c 6520 616e 6420 7374 616e 6461  xible and standa
-00000510: 7264 697a 6564 206d 6573 7361 6765 2066  rdized message f
-00000520: 6574 6368 696e 6720 616e 6420 7075 7368  etching and push
-00000530: 696e 6720 6672 616d 6577 6f72 6b2c 2065  ing framework, e
-00000540: 7370 6563 6961 6c6c 7920 666f 7220 5b54  specially for [T
-00000550: 656c 6567 7261 6d5d 2868 7474 703a 2f2f  elegram](http://
-00000560: 7777 772e 7465 6c65 6772 616d 2e6f 7267  www.telegram.org
-00000570: 2920 616e 6420 5b54 656c 6567 7261 6d20  ) and [Telegram 
-00000580: 426f 745d 2868 7474 7073 3a2f 2f63 6f72  Bot](https://cor
-00000590: 652e 7465 6c65 6772 616d 2e6f 7267 2f62  e.telegram.org/b
-000005a0: 6f74 7329 2e0a 0a54 6865 2074 6172 6765  ots)...The targe
-000005b0: 7420 6e65 7773 2073 6f75 7263 6520 6361  t news source ca
-000005c0: 6e20 6265 2048 544d 4c20 7061 6765 2c20  n be HTML page, 
-000005d0: 4a53 4f4e 2061 6e64 2058 4d4c 2e20 5765  JSON and XML. We
-000005e0: 2061 6c73 6f20 7072 6f76 6964 6520 6375   also provide cu
-000005f0: 7374 6f6d 697a 6564 2070 726f 6365 7373  stomized process
-00000600: 2066 6f72 2075 6e6b 6e6f 776e 2064 6174   for unknown dat
-00000610: 6120 666f 726d 6174 2e0a 0a50 7573 6820  a format...Push 
-00000620: 7468 6520 6c61 7465 7374 206e 6577 7320  the latest news 
-00000630: 746f 2079 6f75 7220 6368 616e 6e65 6c20  to your channel 
-00000640: 6f72 2067 726f 7570 206f 6e63 6520 6974  or group once it
-00000650: 2068 6170 7065 6e73 210a 0a23 2320 496e   happens!..## In
-00000660: 7374 616c 6c0a 0a60 6060 7368 656c 6c0a  stall..```shell.
-00000670: 2420 7069 7020 696e 7374 616c 6c20 7465  $ pip install te
-00000680: 6c65 6772 616d 2d6e 6577 730a 6060 600a  legram-news.```.
-00000690: 0a4f 722c 2079 6f75 2063 616e 2069 6e73  .Or, you can ins
-000006a0: 7461 6c6c 2062 7920 636c 6f6e 696e 6720  tall by cloning 
-000006b0: 7468 6973 2072 6570 6f73 6974 6f72 793a  this repository:
-000006c0: 0a0a 6060 6073 6865 6c6c 0a24 2067 6974  ..```shell.$ git
-000006d0: 2063 6c6f 6e65 2068 7474 7073 3a2f 2f67   clone https://g
-000006e0: 6974 6875 622e 636f 6d2f 4553 575a 592f  ithub.com/ESWZY/
-000006f0: 7465 6c65 6772 616d 2d6e 6577 732e 6769  telegram-news.gi
-00000700: 740a 2420 6364 2074 656c 6567 7261 6d2d  t.$ cd telegram-
-00000710: 6e65 7773 0a24 2070 7974 686f 6e20 7365  news.$ python se
-00000720: 7475 702e 7079 2069 6e73 7461 6c6c 0a60  tup.py install.`
-00000730: 6060 0a0a 2323 2050 7265 7061 7265 0a0a  ``..## Prepare..
-00000740: 4974 2064 6f65 7320 6e6f 7420 6e65 6564  It does not need
-00000750: 206d 7563 6820 736f 2074 6861 7420 796f   much so that yo
-00000760: 7520 6361 6e20 7275 6e20 796f 7572 2063  u can run your c
-00000770: 6f64 6520 616e 7977 6865 7265 2e0a 0a46  ode anywhere...F
-00000780: 6972 7374 2c20 6173 6b20 5b40 426f 7446  irst, ask [@BotF
-00000790: 6174 6865 725d 2868 7474 7073 3a2f 2f74  ather](https://t
-000007a0: 2e6d 652f 626f 7466 6174 6865 7229 2066  .me/botfather) f
-000007b0: 6f72 2061 2062 6f74 2061 6e64 2062 6f74  or a bot and bot
-000007c0: 2074 6f6b 656e 2e20 4166 7465 7220 7468   token. After th
-000007d0: 6174 2c20 6372 6561 7465 2061 2070 7562  at, create a pub
-000007e0: 6c69 6320 5b63 6861 6e6e 656c 5d28 6874  lic [channel](ht
-000007f0: 7470 733a 2f2f 7465 6c65 6772 616d 2e6f  tps://telegram.o
-00000800: 7267 2f74 6f75 722f 6368 616e 6e65 6c73  rg/tour/channels
-00000810: 2920 6f72 205b 6772 6f75 705d 2868 7474  ) or [group](htt
-00000820: 7073 3a2f 2f74 656c 6567 7261 6d2e 6f72  ps://telegram.or
-00000830: 672f 746f 7572 2f67 726f 7570 7329 2c20  g/tour/groups), 
-00000840: 616e 6420 7265 6d65 6d62 6572 2063 6861  and remember cha
-00000850: 7420 6964 2079 6f75 206a 7573 7420 6e61  t id you just na
-00000860: 6d65 642e 2044 6f20 6e6f 7420 666f 7267  med. Do not forg
-00000870: 6574 2074 6f20 696e 7669 7465 2079 6f75  et to invite you
-00000880: 7220 626f 7420 696e 746f 2079 6f75 7220  r bot into your 
-00000890: 6368 616e 6e65 6c20 6f72 2067 726f 7570  channel or group
-000008a0: 2061 6e64 206d 616b 6520 6974 2061 6e20   and make it an 
-000008b0: 6164 6d69 6e2e 0a0a 596f 7520 616c 736f  admin...You also
-000008c0: 206e 6565 6420 6120 5351 4c20 6461 7461   need a SQL data
-000008d0: 6261 7365 2e20 416e 7920 5351 4c20 6461  base. Any SQL da
-000008e0: 7461 6261 7365 2069 7320 4f4b 2e20 4573  tabase is OK. Es
-000008f0: 7065 6369 616c 6c79 2c20 4920 7265 636f  pecially, I reco
-00000900: 6d6d 656e 6420 5b50 6f73 7467 7265 5351  mmend [PostgreSQ
-00000910: 4c5d 2868 7474 7073 3a2f 2f77 7777 2e70  L](https://www.p
-00000920: 6f73 7467 7265 7371 6c2e 6f72 672f 292e  ostgresql.org/).
-00000930: 0a0a 2323 2051 7569 636b 2064 6570 6c6f  ..## Quick deplo
-00000940: 7920 6f6e 2048 6572 6f6b 750a 0a43 6c69  y on Heroku..Cli
-00000950: 636b 20f0 9f91 8720 6275 7474 6f6e 2074  ck .... button t
-00000960: 6f20 6465 706c 6f79 2061 6e20 6578 616d  o deploy an exam
-00000970: 706c 6520 666f 7220 6672 6565 2e20 5079  ple for free. Py
-00000980: 7468 6f6e 2065 6e76 6972 6f6e 6d65 6e74  thon environment
-00000990: 2061 6e64 2050 6f73 7467 7265 5351 4c20   and PostgreSQL 
-000009a0: 6461 7461 6261 7365 2068 6176 6520 6265  database have be
-000009b0: 656e 2070 7265 7061 7265 642e 0a0a 3c61  en prepared...<a
-000009c0: 2068 7265 663d 2268 7474 7073 3a2f 2f68   href="https://h
-000009d0: 6572 6f6b 752e 636f 6d2f 6465 706c 6f79  eroku.com/deploy
-000009e0: 3f74 656d 706c 6174 653d 6874 7470 733a  ?template=https:
-000009f0: 2f2f 6769 7468 7562 2e63 6f6d 2f45 5357  //github.com/ESW
-00000a00: 5a59 2f74 656c 6567 7261 6d2d 6e65 7773  ZY/telegram-news
-00000a10: 2d67 6574 7469 6e67 2d73 7461 7274 6564  -getting-started
-00000a20: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
-00000a30: 7474 7073 3a2f 2f77 7777 2e68 6572 6f6b  ttps://www.herok
-00000a40: 7563 646e 2e63 6f6d 2f64 6570 6c6f 792f  ucdn.com/deploy/
-00000a50: 6275 7474 6f6e 2e73 7667 2220 616c 743d  button.svg" alt=
-00000a60: 2244 6570 6c6f 7922 3e0a 3c2f 613e 0a0a  "Deploy">.</a>..
-00000a70: 4166 7465 7220 6465 706c 6f79 6d65 6e74  After deployment
-00000a80: 2c20 7374 6172 7420 7468 6520 776f 726b  , start the work
-00000a90: 6572 2069 6e20 2252 6573 6f75 7263 6573  er in "Resources
-00000aa0: 2220 7461 622c 2061 6e64 2074 6865 6e20  " tab, and then 
-00000ab0: 796f 7520 6361 6e20 7365 6520 7468 6520  you can see the 
-00000ac0: 6566 6665 6374 2069 6e20 796f 7572 2063  effect in your c
-00000ad0: 6861 6e6e 656c 2f67 726f 7570 2c20 7768  hannel/group, wh
-00000ae0: 6963 6820 636f 6e74 6169 6e73 2062 6f74  ich contains bot
-00000af0: 6820 5343 4d50 206e 6577 7320 616e 6420  h SCMP news and 
-00000b00: 5769 6b69 206e 6577 7320 6174 2073 616d  Wiki news at sam
-00000b10: 6520 7469 6d65 2e0a 0a23 2320 5573 6167  e time...## Usag
-00000b20: 650a 0a54 686f 7365 2061 7265 2033 2065  e..Those are 3 e
-00000b30: 7861 6d70 6c65 7320 666f 7220 796f 7520  xamples for you 
-00000b40: 746f 2075 6e64 6572 7374 616e 6420 686f  to understand ho
-00000b50: 7720 746f 2075 7365 2074 6865 2066 7261  w to use the fra
-00000b60: 6d65 776f 726b 2e0a 0a23 2323 2042 6173  mework...### Bas
-00000b70: 6963 2045 7861 6d70 6c65 0a0a 6060 6070  ic Example..```p
-00000b80: 7974 686f 6e0a 696d 706f 7274 206f 730a  ython.import os.
-00000b90: 6672 6f6d 2073 716c 616c 6368 656d 7920  from sqlalchemy 
-00000ba0: 696d 706f 7274 2063 7265 6174 655f 656e  import create_en
-00000bb0: 6769 6e65 0a66 726f 6d20 7371 6c61 6c63  gine.from sqlalc
-00000bc0: 6865 6d79 2e6f 726d 2069 6d70 6f72 7420  hemy.orm import 
-00000bd0: 5365 7373 696f 6e0a 0a66 726f 6d20 7465  Session..from te
-00000be0: 6c65 6772 616d 5f6e 6577 732e 7465 6d70  legram_news.temp
-00000bf0: 6c61 7465 2069 6d70 6f72 7420 496e 666f  late import Info
-00000c00: 4578 7472 6163 746f 722c 204e 6577 7350  Extractor, NewsP
-00000c10: 6f73 746d 616e 0a0a 2320 5468 7265 6520  ostman..# Three 
-00000c20: 7265 7175 6972 6564 2066 6965 6c64 733a  required fields:
-00000c30: 0a23 2059 6f75 7220 626f 7420 746f 6b65  .# Your bot toke
-00000c40: 6e20 6f62 7461 696e 6564 2066 726f 6d20  n obtained from 
-00000c50: 4042 6f74 4661 7468 6572 0a62 6f74 5f74  @BotFather.bot_t
-00000c60: 6f6b 656e 203d 206f 732e 6765 7465 6e76  oken = os.getenv
-00000c70: 2822 544f 4b45 4e22 290a 2320 4164 6420  ("TOKEN").# Add 
-00000c80: 796f 7572 2062 6f74 7320 696e 746f 2061  your bots into a
-00000c90: 2063 6861 6e6e 656c 2061 7320 616e 2061   channel as an a
-00000ca0: 646d 696e 6973 7472 6174 6f72 0a63 6861  dministrator.cha
-00000cb0: 6e6e 656c 203d 206f 732e 6765 7465 6e76  nnel = os.getenv
-00000cc0: 2822 4348 414e 4e45 4c22 290a 2320 596f  ("CHANNEL").# Yo
-00000cd0: 7572 2064 6174 6162 6173 6520 746f 2073  ur database to s
-00000ce0: 746f 7265 206f 6c64 206d 6573 7361 6765  tore old message
-00000cf0: 732e 0a44 4154 4142 4153 455f 5552 4c20  s..DATABASE_URL 
-00000d00: 3d20 6f73 2e67 6574 656e 7628 2244 4154  = os.getenv("DAT
-00000d10: 4142 4153 455f 5552 4c22 290a 0a23 2043  ABASE_URL")..# C
-00000d20: 7265 6174 6520 6120 6461 7461 6261 7365  reate a database
-00000d30: 2073 6573 7369 6f6e 0a65 6e67 696e 6520   session.engine 
-00000d40: 3d20 6372 6561 7465 5f65 6e67 696e 6528  = create_engine(
-00000d50: 4441 5441 4241 5345 5f55 524c 290a 6462  DATABASE_URL).db
-00000d60: 203d 2053 6573 7369 6f6e 2862 696e 643d   = Session(bind=
-00000d70: 656e 6769 6e65 2e63 6f6e 6e65 6374 2829  engine.connect()
-00000d80: 290a 0a23 2054 6865 206e 6577 7320 736f  )..# The news so
-00000d90: 7572 6365 0a75 726c 203d 2022 6874 7470  urce.url = "http
-00000da0: 733a 2f2f 656e 2e77 696b 696e 6577 732e  s://en.wikinews.
-00000db0: 6f72 672f 7769 6b69 2f4d 6169 6e5f 5061  org/wiki/Main_Pa
-00000dc0: 6765 220a 7461 6720 3d20 2257 696b 6920  ge".tag = "Wiki 
-00000dd0: 4e65 7773 220a 7461 626c 655f 6e61 6d65  News".table_name
-00000de0: 203d 2022 7769 6b69 6e65 7773 220a 0a23   = "wikinews"..#
-00000df0: 2049 6e66 6f20 6578 7472 6163 746f 7220   Info extractor 
-00000e00: 746f 2070 726f 6365 7373 2064 6174 6120  to process data 
-00000e10: 666f 726d 6174 0a69 6520 3d20 496e 666f  format.ie = Info
-00000e20: 4578 7472 6163 746f 7228 290a 0a23 2053  Extractor()..# S
-00000e30: 656c 6563 7420 7365 6c65 6374 2065 6c65  elect select ele
-00000e40: 6d65 6e74 2062 7920 4353 532d 6261 7365  ment by CSS-base
-00000e50: 6420 7365 6c65 6374 6f72 0a69 652e 7365  d selector.ie.se
-00000e60: 745f 6c69 7374 5f73 656c 6563 746f 7228  t_list_selector(
-00000e70: 2723 4d61 696e 5061 6765 5f6c 6174 6573  '#MainPage_lates
-00000e80: 745f 6e65 7773 5f74 6578 7420 3e20 756c  t_news_text > ul
-00000e90: 203e 206c 6927 290a 6965 2e73 6574 5f74   > li').ie.set_t
-00000ea0: 6974 6c65 5f73 656c 6563 746f 7228 2723  itle_selector('#
-00000eb0: 6669 7273 7448 6561 6469 6e67 2729 0a69  firstHeading').i
-00000ec0: 652e 7365 745f 7061 7261 6772 6170 685f  e.set_paragraph_
-00000ed0: 7365 6c65 6374 6f72 2827 236d 772d 636f  selector('#mw-co
-00000ee0: 6e74 656e 742d 7465 7874 203e 2064 6976  ntent-text > div
-00000ef0: 203e 2070 3a6e 6f74 2870 3a6e 7468 2d63   > p:not(p:nth-c
-00000f00: 6869 6c64 2831 2929 2729 0a69 652e 7365  hild(1))').ie.se
-00000f10: 745f 7469 6d65 5f73 656c 6563 746f 7228  t_time_selector(
-00000f20: 2723 6d77 2d63 6f6e 7465 6e74 2d74 6578  '#mw-content-tex
-00000f30: 7420 3e20 6469 7620 3e20 703a 6e74 682d  t > div > p:nth-
-00000f40: 6368 696c 6428 3129 203e 2073 7472 6f6e  child(1) > stron
-00000f50: 6727 290a 6965 2e73 6574 5f73 6f75 7263  g').ie.set_sourc
-00000f60: 655f 7365 6c65 6374 6f72 2827 7370 616e  e_selector('span
-00000f70: 2e73 6f75 7263 6554 656d 706c 6174 6527  .sourceTemplate'
-00000f80: 290a 0a23 2053 6574 2061 206d 6178 206c  )..# Set a max l
-00000f90: 656e 6774 6820 666f 7220 706f 7374 2c20  ength for post, 
-00000fa0: 4d61 7820 6973 2034 3039 360a 6965 2e6d  Max is 4096.ie.m
-00000fb0: 6178 5f70 6f73 745f 6c65 6e67 7468 203d  ax_post_length =
-00000fc0: 2032 3030 300a 0a23 204e 6577 7320 706f   2000..# News po
-00000fd0: 7374 6d61 6e20 746f 206d 616e 6167 6520  stman to manage 
-00000fe0: 7365 6e64 696e 6720 6166 6661 6972 0a6e  sending affair.n
-00000ff0: 7020 3d20 4e65 7773 506f 7374 6d61 6e28  p = NewsPostman(
-00001000: 6c69 7374 5552 4c73 3d5b 7572 6c2c 205d  listURLs=[url, ]
-00001010: 2c20 7365 6e64 4c69 7374 3d5b 6368 616e  , sendList=[chan
-00001020: 6e65 6c2c 205d 2c20 6462 3d64 622c 2074  nel, ], db=db, t
-00001030: 6167 3d74 6167 290a 6e70 2e73 6574 5f62  ag=tag).np.set_b
-00001040: 6f74 5f74 6f6b 656e 2862 6f74 5f74 6f6b  ot_token(bot_tok
-00001050: 656e 290a 6e70 2e73 6574 5f65 7874 7261  en).np.set_extra
-00001060: 6374 6f72 2869 6529 0a6e 702e 7365 745f  ctor(ie).np.set_
-00001070: 7461 626c 655f 6e61 6d65 2874 6162 6c65  table_name(table
-00001080: 5f6e 616d 6529 0a0a 2320 5374 6172 7420  _name)..# Start 
-00001090: 746f 2077 6f72 6b21 0a6e 702e 706f 6c6c  to work!.np.poll
-000010a0: 2829 0a60 6060 0a0a 5479 7069 6361 6c20  ().```..Typical 
-000010b0: 7265 7375 6c74 733a 0a0a 3c64 6976 2061  results:..<div a
-000010c0: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-000010d0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-000010e0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-000010f0: 7263 6f6e 7465 6e74 2e63 6f6d 2f45 5357  rcontent.com/ESW
-00001100: 5a59 2f74 656c 6567 7261 6d2d 6e65 7773  ZY/telegram-news
-00001110: 2f6d 6173 7465 722f 646f 6373 2f69 6d61  /master/docs/ima
-00001120: 6765 732f 6465 6d6f 312e 706e 6722 2061  ges/demo1.png" a
-00001130: 6c74 3d22 4465 6d6f 2031 2220 7769 6474  lt="Demo 1" widt
-00001140: 683d 2234 3025 223e 0a20 203c 696d 6720  h="40%">.  <img 
-00001150: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00001160: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00001170: 6e74 2e63 6f6d 2f45 5357 5a59 2f74 656c  nt.com/ESWZY/tel
-00001180: 6567 7261 6d2d 6e65 7773 2f6d 6173 7465  egram-news/maste
-00001190: 722f 646f 6373 2f69 6d61 6765 732f 6465  r/docs/images/de
-000011a0: 6d6f 322e 706e 6722 2061 6c74 3d22 4465  mo2.png" alt="De
-000011b0: 6d6f 2032 2220 7769 6474 683d 2234 3025  mo 2" width="40%
-000011c0: 223e 0a3c 2f64 6976 3e0a 0a23 2323 2041  ">.</div>..### A
-000011d0: 6476 616e 6365 6420 4578 616d 706c 650a  dvanced Example.
-000011e0: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-000011f0: 7420 6f73 0a66 726f 6d20 7371 6c61 6c63  t os.from sqlalc
-00001200: 6865 6d79 2069 6d70 6f72 7420 6372 6561  hemy import crea
-00001210: 7465 5f65 6e67 696e 650a 6672 6f6d 2073  te_engine.from s
-00001220: 716c 616c 6368 656d 792e 6f72 6d20 696d  qlalchemy.orm im
-00001230: 706f 7274 2053 6573 7369 6f6e 0a66 726f  port Session.fro
-00001240: 6d20 7465 6c65 6772 616d 5f6e 6577 732e  m telegram_news.
-00001250: 7465 6d70 6c61 7465 2069 6d70 6f72 7420  template import 
-00001260: 496e 666f 4578 7472 6163 746f 722c 204e  InfoExtractor, N
-00001270: 6577 7350 6f73 746d 616e 0a62 6f74 5f74  ewsPostman.bot_t
-00001280: 6f6b 656e 203d 206f 732e 6765 7465 6e76  oken = os.getenv
-00001290: 2822 544f 4b45 4e22 290a 6368 616e 6e65  ("TOKEN").channe
-000012a0: 6c20 3d20 6f73 2e67 6574 656e 7628 2243  l = os.getenv("C
-000012b0: 4841 4e4e 454c 2229 0a44 4154 4142 4153  HANNEL").DATABAS
-000012c0: 455f 5552 4c20 3d20 6f73 2e67 6574 656e  E_URL = os.geten
-000012d0: 7628 2244 4154 4142 4153 455f 5552 4c22  v("DATABASE_URL"
-000012e0: 290a 656e 6769 6e65 203d 2063 7265 6174  ).engine = creat
-000012f0: 655f 656e 6769 6e65 2844 4154 4142 4153  e_engine(DATABAS
-00001300: 455f 5552 4c29 0a64 6220 3d20 5365 7373  E_URL).db = Sess
-00001310: 696f 6e28 6269 6e64 3d65 6e67 696e 652e  ion(bind=engine.
-00001320: 636f 6e6e 6563 7428 2929 0a0a 2320 4162  connect())..# Ab
-00001330: 6f76 6520 636f 6465 2069 7320 6173 2073  ove code is as s
-00001340: 616d 6520 6173 2074 6865 2062 6173 6963  ame as the basic
-00001350: 2065 7861 6d70 6c65 2c20 796f 7520 6361   example, you ca
-00001360: 6e20 7265 7573 6520 7468 6f73 6520 636f  n reuse those co
-00001370: 6465 2064 6972 6563 746c 790a 0a75 726c  de directly..url
-00001380: 5f32 203d 2022 6874 7470 733a 2f2f 7777  _2 = "https://ww
-00001390: 772e 636e 6265 7461 2e63 6f6d 2f22 0a74  w.cnbeta.com/".t
-000013a0: 6167 5f32 203d 2022 636e 4265 7461 220a  ag_2 = "cnBeta".
-000013b0: 7461 626c 655f 6e61 6d65 5f32 203d 2022  table_name_2 = "
-000013c0: 636e 6265 7461 6e65 7773 220a 0a69 655f  cnbetanews"..ie_
-000013d0: 3220 3d20 496e 666f 4578 7472 6163 746f  2 = InfoExtracto
-000013e0: 7228 290a 6965 5f32 2e73 6574 5f6c 6973  r().ie_2.set_lis
-000013f0: 745f 7365 6c65 6374 6f72 2827 2e69 7465  t_selector('.ite
-00001400: 6d73 2d61 7265 6120 3e20 6469 7620 3e20  ms-area > div > 
-00001410: 646c 203e 2064 7420 3e20 6127 290a 6965  dl > dt > a').ie
-00001420: 5f32 2e73 6574 5f74 6974 6c65 5f73 656c  _2.set_title_sel
-00001430: 6563 746f 7228 2768 6561 6465 7220 3e20  ector('header > 
-00001440: 6831 2729 0a0a 2320 5365 6c65 6374 206d  h1')..# Select m
-00001450: 616e 7920 7461 7267 6574 2061 7420 7361  any target at sa
-00001460: 6d65 2074 696d 6520 2020 200a 6965 5f32  me time    .ie_2
-00001470: 2e73 6574 5f70 6172 6167 7261 7068 5f73  .set_paragraph_s
-00001480: 656c 6563 746f 7228 2764 6976 2e63 6e62  elector('div.cnb
-00001490: 6574 612d 6172 7469 636c 652d 626f 6479  eta-article-body
-000014a0: 203e 2064 6976 2e61 7274 6963 6c65 2d73   > div.article-s
-000014b0: 756d 6d61 7279 203e 2070 2c20 2720 2023  ummary > p, '  #
-000014c0: 2053 756d 6d61 7279 206f 6e6c 790a 2020   Summary only.  
-000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014e0: 2020 2020 2020 2020 2020 2764 6976 2e63            'div.c
-000014f0: 6e62 6574 612d 6172 7469 636c 652d 626f  nbeta-article-bo
-00001500: 6479 203e 2064 6976 2e61 7274 6963 6c65  dy > div.article
-00001510: 2d63 6f6e 7465 6e74 203e 2070 2729 2020  -content > p')  
-00001520: 2023 2043 6f6e 7465 6e74 206f 6e6c 790a   # Content only.
-00001530: 6965 5f32 2e73 6574 5f74 696d 655f 7365  ie_2.set_time_se
-00001540: 6c65 6374 6f72 2827 6865 6164 6572 203e  lector('header >
-00001550: 2064 6976 203e 2073 7061 6e3a 6e74 682d   div > span:nth-
-00001560: 6368 696c 6428 3129 2729 0a69 655f 322e  child(1)').ie_2.
-00001570: 7365 745f 736f 7572 6365 5f73 656c 6563  set_source_selec
-00001580: 746f 7228 2768 6561 6465 7220 3e20 6469  tor('header > di
-00001590: 7620 3e20 7370 616e 2e73 6f75 7263 6527  v > span.source'
-000015a0: 290a 0a23 2053 656c 6563 7420 696d 6167  )..# Select imag
-000015b0: 6520 746f 2064 6973 706c 6179 2c20 7468  e to display, th
-000015c0: 656e 2074 6865 206d 6178 206c 656e 6774  en the max lengt
-000015d0: 6820 6973 2064 6f77 6e20 746f 2031 3032  h is down to 102
-000015e0: 340a 6965 5f32 2e73 6574 5f69 6d61 6765  4.ie_2.set_image
-000015f0: 5f73 656c 6563 746f 7228 2764 6976 2e63  _selector('div.c
-00001600: 6e62 6574 612d 6172 7469 636c 652d 626f  nbeta-article-bo
-00001610: 6479 203e 2064 6976 2e61 7274 6963 6c65  dy > div.article
-00001620: 2d73 756d 6d61 7279 203e 2070 2069 6d67  -summary > p img
-00001630: 2c20 2720 2023 2046 726f 6d20 7375 6d6d  , '  # From summ
-00001640: 6172 7920 6f6e 6c79 0a20 2020 2020 2020  ary only.       
-00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2027 6469 762e 636e 6265 7461 2d61 7274   'div.cnbeta-art
-00001670: 6963 6c65 2d62 6f64 7920 3e20 6469 762e  icle-body > div.
-00001680: 6172 7469 636c 652d 636f 6e74 656e 7420  article-content 
-00001690: 3e20 7020 696d 6727 2920 2020 2320 4672  > p img')   # Fr
-000016a0: 6f6d 2063 6f6e 7465 6e74 206f 6e6c 790a  om content only.
-000016b0: 6965 5f32 2e6d 6178 5f70 6f73 745f 6c65  ie_2.max_post_le
-000016c0: 6e67 7468 203d 2031 3030 300a 0a6e 705f  ngth = 1000..np_
-000016d0: 3220 3d20 4e65 7773 506f 7374 6d61 6e28  2 = NewsPostman(
-000016e0: 6c69 7374 5552 4c73 3d5b 7572 6c5f 322c  listURLs=[url_2,
-000016f0: 205d 2c20 7365 6e64 4c69 7374 3d5b 6368   ], sendList=[ch
-00001700: 616e 6e65 6c5d 2c20 7461 673d 7461 675f  annel], tag=tag_
-00001710: 322c 2064 623d 6462 290a 6e70 5f32 2e73  2, db=db).np_2.s
-00001720: 6574 5f65 7874 7261 6374 6f72 2869 655f  et_extractor(ie_
-00001730: 3229 0a6e 705f 322e 7365 745f 7461 626c  2).np_2.set_tabl
-00001740: 655f 6e61 6d65 2874 6162 6c65 5f6e 616d  e_name(table_nam
-00001750: 655f 3229 0a6e 705f 322e 706f 6c6c 2829  e_2).np_2.poll()
-00001760: 0a60 6060 0a0a 5479 7069 6361 6c20 7265  .```..Typical re
-00001770: 7375 6c74 733a 0a0a 3c64 6976 2061 6c69  sults:..<div ali
-00001780: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
-00001790: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000017a0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-000017b0: 6f6e 7465 6e74 2e63 6f6d 2f45 5357 5a59  ontent.com/ESWZY
-000017c0: 2f74 656c 6567 7261 6d2d 6e65 7773 2f6d  /telegram-news/m
-000017d0: 6173 7465 722f 646f 6373 2f69 6d61 6765  aster/docs/image
-000017e0: 732f 6465 6d6f 332e 706e 6722 2061 6c74  s/demo3.png" alt
-000017f0: 3d22 4465 6d6f 2033 2220 7769 6474 683d  ="Demo 3" width=
-00001800: 2234 3025 223e 0a20 203c 696d 6720 7372  "40%">.  <img sr
-00001810: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-00001820: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00001830: 2e63 6f6d 2f45 5357 5a59 2f74 656c 6567  .com/ESWZY/teleg
-00001840: 7261 6d2d 6e65 7773 2f6d 6173 7465 722f  ram-news/master/
-00001850: 646f 6373 2f69 6d61 6765 732f 6465 6d6f  docs/images/demo
-00001860: 342e 706e 6722 2061 6c74 3d22 4465 6d6f  4.png" alt="Demo
-00001870: 2034 2220 7769 6474 683d 2234 3025 223e   4" width="40%">
-00001880: 0a3c 2f64 6976 3e0a 0a23 2323 2041 6476  .</div>..### Adv
-00001890: 616e 6365 6420 4578 616d 706c 6520 666f  anced Example fo
-000018a0: 7220 4a53 4f4e 2061 6e64 2058 4d4c 0a0a  r JSON and XML..
-000018b0: 5468 6520 6861 6e64 6c65 2066 6f72 204a  The handle for J
-000018c0: 534f 4e20 616e 6420 584d 4c20 6172 6520  SON and XML are 
-000018d0: 7175 6974 6520 7369 6d69 6c61 722e 2059  quite similar. Y
-000018e0: 6f75 2063 616e 2063 6f6e 7665 7274 2058  ou can convert X
-000018f0: 4d4c 2074 6f20 4a53 4f4e 2062 7920 6675  ML to JSON by fu
-00001900: 6e63 7469 6f6e 2060 7465 6c65 6772 616d  nction `telegram
-00001910: 5f6e 6577 732e 7574 696c 732e 786d 6c5f  _news.utils.xml_
-00001920: 746f 5f6a 736f 6e60 2c20 616e 6420 7573  to_json`, and us
-00001930: 6520 604e 6577 7350 6f73 746d 616e 4a53  e `NewsPostmanJS
-00001940: 4f4e 6020 616e 6420 6049 6e66 6f45 7874  ON` and `InfoExt
-00001950: 7261 6374 6f72 4a53 4f4e 602e 204f 722c  ractorJSON`. Or,
-00001960: 2079 6f75 2063 616e 2075 7365 2060 4e65   you can use `Ne
-00001970: 7773 506f 7374 6d61 6e58 4d4c 6020 616e  wsPostmanXML` an
-00001980: 6420 6049 6e66 6f45 7874 7261 6374 6f72  d `InfoExtractor
-00001990: 584d 4c60 2064 6972 6563 746c 792e 0a0a  XML` directly...
-000019a0: 596f 7520 7368 6f75 6c64 2075 7365 206b  You should use k
-000019b0: 6579 206c 6973 7420 746f 2072 6563 7572  ey list to recur
-000019c0: 7369 7665 6c79 2072 6f75 7465 2074 6f20  sively route to 
-000019d0: 7468 6520 696e 666f 726d 6174 696f 6e20  the information 
-000019e0: 796f 7520 7761 6e74 2e0a 0a60 6060 7079  you want...```py
-000019f0: 7468 6f6e 0a69 6d70 6f72 7420 6861 7368  thon.import hash
-00001a00: 6c69 620a 696d 706f 7274 206a 736f 6e0a  lib.import json.
-00001a10: 696d 706f 7274 206f 730a 6672 6f6d 2073  import os.from s
-00001a20: 716c 616c 6368 656d 7920 696d 706f 7274  qlalchemy import
-00001a30: 2063 7265 6174 655f 656e 6769 6e65 0a66   create_engine.f
-00001a40: 726f 6d20 7371 6c61 6c63 6865 6d79 2e6f  rom sqlalchemy.o
-00001a50: 726d 2069 6d70 6f72 7420 5365 7373 696f  rm import Sessio
-00001a60: 6e0a 6672 6f6d 2074 656c 6567 7261 6d5f  n.from telegram_
-00001a70: 6e65 7773 2e74 656d 706c 6174 6520 696d  news.template im
-00001a80: 706f 7274 2049 6e66 6f45 7874 7261 6374  port InfoExtract
-00001a90: 6f72 4a53 4f4e 2c20 4e65 7773 506f 7374  orJSON, NewsPost
-00001aa0: 6d61 6e4a 534f 4e0a 6672 6f6d 2074 656c  manJSON.from tel
-00001ab0: 6567 7261 6d5f 6e65 7773 2e75 7469 6c73  egram_news.utils
-00001ac0: 2069 6d70 6f72 7420 786d 6c5f 746f 5f6a   import xml_to_j
-00001ad0: 736f 6e0a 626f 745f 746f 6b65 6e20 3d20  son.bot_token = 
-00001ae0: 6f73 2e67 6574 656e 7628 2254 4f4b 454e  os.getenv("TOKEN
-00001af0: 2229 0a63 6861 6e6e 656c 203d 206f 732e  ").channel = os.
-00001b00: 6765 7465 6e76 2822 4348 414e 4e45 4c22  getenv("CHANNEL"
-00001b10: 290a 4441 5441 4241 5345 5f55 524c 203d  ).DATABASE_URL =
-00001b20: 206f 732e 6765 7465 6e76 2822 4441 5441   os.getenv("DATA
-00001b30: 4241 5345 5f55 524c 2229 0a65 6e67 696e  BASE_URL").engin
-00001b40: 6520 3d20 6372 6561 7465 5f65 6e67 696e  e = create_engin
-00001b50: 6528 4441 5441 4241 5345 5f55 524c 290a  e(DATABASE_URL).
-00001b60: 6462 203d 2053 6573 7369 6f6e 2862 696e  db = Session(bin
-00001b70: 643d 656e 6769 6e65 2e63 6f6e 6e65 6374  d=engine.connect
-00001b80: 2829 290a 0a75 726c 5f33 203d 2022 6874  ())..url_3 = "ht
-00001b90: 7470 733a 2f2f 7777 772e 7363 6d70 2e63  tps://www.scmp.c
-00001ba0: 6f6d 2f72 7373 2f39 312f 6665 6564 220a  om/rss/91/feed".
-00001bb0: 7461 675f 3320 3d20 2253 434d 5022 0a74  tag_3 = "SCMP".t
-00001bc0: 6162 6c65 5f6e 616d 655f 3320 3d20 2273  able_name_3 = "s
-00001bd0: 636d 706e 6577 7322 0a0a 6965 5f33 203d  cmpnews"..ie_3 =
-00001be0: 2049 6e66 6f45 7874 7261 6374 6f72 4a53   InfoExtractorJS
-00001bf0: 4f4e 2829 0a0a 2320 5072 652d 7072 6f63  ON()..# Pre-proc
-00001c00: 6573 7320 7468 6520 584d 4c20 7374 7269  ess the XML stri
-00001c10: 6e67 2c20 636f 6e76 6572 7420 746f 204a  ng, convert to J
-00001c20: 534f 4e20 7374 7269 6e67 0a64 6566 206c  SON string.def l
-00001c30: 6973 745f 7072 655f 7072 6f63 6573 7328  ist_pre_process(
-00001c40: 7465 7874 293a 0a20 2020 2074 6578 7420  text):.    text 
-00001c50: 3d20 6a73 6f6e 2e6c 6f61 6473 2878 6d6c  = json.loads(xml
-00001c60: 5f74 6f5f 6a73 6f6e 2874 6578 7429 290a  _to_json(text)).
-00001c70: 2020 2020 7265 7475 726e 206a 736f 6e2e      return json.
-00001c80: 6475 6d70 7328 7465 7874 290a 6965 5f33  dumps(text).ie_3
-00001c90: 2e73 6574 5f6c 6973 745f 7072 655f 7072  .set_list_pre_pr
-00001ca0: 6f63 6573 735f 706f 6c69 6379 286c 6973  ocess_policy(lis
-00001cb0: 745f 7072 655f 7072 6f63 6573 7329 0a0a  t_pre_process)..
-00001cc0: 2320 526f 7574 6520 6279 206b 6579 206c  # Route by key l
-00001cd0: 6973 740a 6965 5f33 2e73 6574 5f6c 6973  ist.ie_3.set_lis
-00001ce0: 745f 726f 7574 6572 285b 2772 7373 272c  t_router(['rss',
-00001cf0: 2027 6368 616e 6e65 6c27 2c20 2769 7465   'channel', 'ite
-00001d00: 6d27 5d29 0a69 655f 332e 7365 745f 6c69  m']).ie_3.set_li
-00001d10: 6e6b 5f72 6f75 7465 7228 5b27 6c69 6e6b  nk_router(['link
-00001d20: 275d 290a 6965 5f33 2e73 6574 5f74 6974  ']).ie_3.set_tit
-00001d30: 6c65 5f72 6f75 7465 7228 5b27 7469 746c  le_router(['titl
-00001d40: 6527 5d29 0a69 655f 332e 7365 745f 7061  e']).ie_3.set_pa
-00001d50: 7261 6772 6170 6873 5f72 6f75 7465 7228  ragraphs_router(
-00001d60: 5b27 6465 7363 7269 7074 696f 6e27 5d29  ['description'])
-00001d70: 0a69 655f 332e 7365 745f 7469 6d65 5f72  .ie_3.set_time_r
-00001d80: 6f75 7465 7228 5b27 7075 6244 6174 6527  outer(['pubDate'
-00001d90: 5d29 0a69 655f 332e 7365 745f 736f 7572  ]).ie_3.set_sour
-00001da0: 6365 5f72 6f75 7465 7228 5b27 6175 7468  ce_router(['auth
-00001db0: 6f72 275d 290a 6965 5f33 2e73 6574 5f69  or']).ie_3.set_i
-00001dc0: 6d61 6765 5f72 6f75 7465 7228 5b27 6d65  mage_router(['me
-00001dd0: 6469 613a 7468 756d 626e 6169 6c27 2c20  dia:thumbnail', 
-00001de0: 2740 7572 6c27 5d29 0a0a 2320 4375 7374  '@url'])..# Cust
-00001df0: 6f6d 697a 6520 4944 2066 6f72 206e 6577  omize ID for new
-00001e00: 7320 6974 656d 0a64 6566 2069 645f 706f  s item.def id_po
-00001e10: 6c69 6379 286c 696e 6b29 3a0a 2020 2020  licy(link):.    
-00001e20: 7265 7475 726e 2068 6173 686c 6962 2e6d  return hashlib.m
-00001e30: 6435 286c 696e 6b2e 656e 636f 6465 2822  d5(link.encode("
-00001e40: 7574 662d 3822 2929 2e68 6578 6469 6765  utf-8")).hexdige
-00001e50: 7374 2829 0a69 655f 332e 7365 745f 6964  st().ie_3.set_id
-00001e60: 5f70 6f6c 6963 7928 6964 5f70 6f6c 6963  _policy(id_polic
-00001e70: 7929 0a0a 6e70 5f33 203d 204e 6577 7350  y)..np_3 = NewsP
-00001e80: 6f73 746d 616e 4a53 4f4e 286c 6973 7455  ostmanJSON(listU
-00001e90: 524c 733d 5b75 726c 5f33 5d2c 2073 656e  RLs=[url_3], sen
-00001ea0: 644c 6973 743d 5b63 6861 6e6e 656c 5d2c  dList=[channel],
-00001eb0: 2064 623d 6462 2c20 7461 673d 7461 675f   db=db, tag=tag_
-00001ec0: 3329 0a6e 705f 332e 7365 745f 6578 7472  3).np_3.set_extr
-00001ed0: 6163 746f 7228 6965 5f33 290a 6e70 5f33  actor(ie_3).np_3
-00001ee0: 2e73 6574 5f74 6162 6c65 5f6e 616d 6528  .set_table_name(
-00001ef0: 7461 626c 655f 6e61 6d65 5f33 290a 6e70  table_name_3).np
-00001f00: 5f33 2e70 6f6c 6c28 290a 6060 600a 0a54  _3.poll().```..T
-00001f10: 7970 6963 616c 2072 6573 756c 7473 3a0a  ypical results:.
-00001f20: 0a3c 6469 7620 616c 6967 6e3d 2263 656e  .<div align="cen
-00001f30: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
-00001f40: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00001f50: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00001f60: 636f 6d2f 4553 575a 592f 7465 6c65 6772  com/ESWZY/telegr
-00001f70: 616d 2d6e 6577 732f 6d61 7374 6572 2f64  am-news/master/d
-00001f80: 6f63 732f 696d 6167 6573 2f64 656d 6f35  ocs/images/demo5
-00001f90: 2e70 6e67 2220 616c 743d 2244 656d 6f20  .png" alt="Demo 
-00001fa0: 3522 2077 6964 7468 3d22 3430 2522 3e0a  5" width="40%">.
-00001fb0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00001fc0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00001fd0: 6572 636f 6e74 656e 742e 636f 6d2f 4553  ercontent.com/ES
-00001fe0: 575a 592f 7465 6c65 6772 616d 2d6e 6577  WZY/telegram-new
-00001ff0: 732f 6d61 7374 6572 2f64 6f63 732f 696d  s/master/docs/im
-00002000: 6167 6573 2f64 656d 6f36 2e70 6e67 2220  ages/demo6.png" 
-00002010: 616c 743d 2244 656d 6f20 3622 2077 6964  alt="Demo 6" wid
-00002020: 7468 3d22 3430 2522 3e0a 3c2f 6469 763e  th="40%">.</div>
-00002030: 0a0a 2323 2320 5061 7261 6c6c 656c 2050  ..### Parallel P
-00002040: 726f 6772 616d 0a0a 4966 2079 6f75 2075  rogram..If you u
-00002050: 7365 2074 6865 2073 616d 6520 6461 7461  se the same data
-00002060: 6261 7365 2061 6e64 2073 656e 6420 746f  base and send to
-00002070: 2074 6865 2073 616d 6520 6368 616e 6e65   the same channe
-00002080: 6c2c 2079 6f75 2063 616e 2073 696d 706c  l, you can simpl
-00002090: 7920 6a6f 696e 7420 6561 6368 2070 6172  y joint each par
-000020a0: 7420 6f66 2063 6f64 6520 626c 6f63 6b2c  t of code block,
-000020b0: 2061 6e64 2063 616c 6c20 6070 6f6c 6c28   and call `poll(
-000020c0: 2960 2066 756e 6374 696f 6e20 7369 6d75  )` function simu
-000020d0: 6c74 616e 656f 7573 6c79 2e0a 0a41 6e20  ltaneously...An 
-000020e0: 6578 616d 706c 6520 796f 7520 6361 6e20  example you can 
-000020f0: 6669 6e64 2069 6e20 6f75 7220 4865 726f  find in our Hero
-00002100: 6b75 2064 6570 6c6f 7920 7465 6d70 6c61  ku deploy templa
-00002110: 7465 2072 6570 6f3a 200a 0a68 7474 7073  te repo: ..https
-00002120: 3a2f 2f67 6974 6875 622e 636f 6d2f 4553  ://github.com/ES
-00002130: 575a 592f 7465 6c65 6772 616d 2d6e 6577  WZY/telegram-new
-00002140: 732d 6765 7474 696e 672d 7374 6172 7465  s-getting-starte
-00002150: 642f 626c 6f62 2f6d 6173 7465 722f 6d61  d/blob/master/ma
-00002160: 696e 2e70 790a 0a23 2320 4578 616d 706c  in.py..## Exampl
-00002170: 6520 4368 616e 6e65 6c0a 0a41 2054 656c  e Channel..A Tel
-00002180: 6567 7261 6d20 6368 616e 6e65 6c20 6f66  egram channel of
-00002190: 205b 6261 7369 6320 6578 616d 706c 655d   [basic example]
-000021a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000021b0: 636f 6d2f 4553 575a 592f 7465 6c65 6772  com/ESWZY/telegr
-000021c0: 616d 2d6e 6577 7323 6261 7369 632d 6578  am-news#basic-ex
-000021d0: 616d 706c 6529 2066 6f72 2045 6e67 6c69  ample) for Engli
-000021e0: 7368 2057 696b 696e 6577 733a 205b 7e7e  sh Wikinews: [~~
-000021f0: 4077 696b 696e 6577 735f 656e 7e7e 5d28  @wikinews_en~~](
-00002200: 6874 7470 733a 2f2f 742e 6d65 2f6a 6f69  https://t.me/joi
-00002210: 6e63 6861 742f 5437 5462 4a55 5770 6755  nchat/T7TbJUWpgU
-00002220: 7047 6d61 7259 2920 2869 6e20 456e 676c  pGmarY) (in Engl
-00002230: 6973 6829 0a0a 4120 5465 6c65 6772 616d  ish)..A Telegram
-00002240: 2063 6861 6e6e 656c 2066 6f72 2072 6561   channel for rea
-00002250: 6c74 696d 6520 6561 7274 6871 7561 6b65  ltime earthquake
-00002260: 2077 6172 6e69 6e67 2070 6f77 6572 6564   warning powered
-00002270: 2062 7920 5465 6c65 6772 616d 2d6e 6577   by Telegram-new
-00002280: 733a 205b 4065 6172 7468 7175 616b 655f  s: [@earthquake_
-00002290: 616c 6572 745d 2868 7474 7073 3a2f 2f74  alert](https://t
-000022a0: 2e6d 652f 732f 6561 7274 6871 7561 6b65  .me/s/earthquake
-000022b0: 5f61 6c65 7274 2920 2869 6e20 4368 696e  _alert) (in Chin
-000022c0: 6573 6529 0a0a 2323 2054 4f44 4f0a 0a2d  ese)..## TODO..-
-000022d0: 205b 785d 2048 544d 4c20 6974 656d 206c   [x] HTML item l
-000022e0: 6973 740a 2d20 5b78 5d20 4a53 4f4e 2069  ist.- [x] JSON i
-000022f0: 7465 6d20 6c69 7374 0a2d 205b 785d 2058  tem list.- [x] X
-00002300: 4d4c 2069 7465 6d20 6c69 7374 0a2d 205b  ML item list.- [
-00002310: 785d 2053 656e 6420 496d 6167 650a 2d20  x] Send Image.- 
-00002320: 5b78 5d20 5365 6e64 2056 6964 656f 0a2d  [x] Send Video.-
-00002330: 205b 785d 2053 656e 6420 6d65 6469 6120   [x] Send media 
-00002340: 6772 6f75 700a 2d20 5b20 5d20 5365 6e64  group.- [ ] Send
-00002350: 2066 696c 650a 2d20 5b20 5d20 5365 6e64   file.- [ ] Send
-00002360: 2061 7564 696f 0a2d 205b 785d 2046 696c   audio.- [x] Fil
-00002370: 6520 7365 6e64 696e 6720 7265 7472 790a  e sending retry.
-00002380: 2d20 5b20 5d20 4343 2061 7320 652d 6d61  - [ ] CC as e-ma
-00002390: 696c 0a2d 205b 205d 2057 6562 686f 6f6b  il.- [ ] Webhook
-000023a0: 0a2d 205b 205d 2055 7064 6174 6520 6d65  .- [ ] Update me
-000023b0: 7373 6167 6520 6279 206d 6573 7361 6765  ssage by message
-000023c0: 2049 440a 2d20 5b20 5d20 446f 6375 6d65   ID.- [ ] Docume
-000023d0: 6e74 0a2d 205b 205d 2047 5549 0a0a 2323  nt.- [ ] GUI..##
-000023e0: 2046 6565 6462 6163 6b0a 0a46 6565 6c20   Feedback..Feel 
-000023f0: 6672 6565 2074 6f20 636f 6e74 6163 7420  free to contact 
-00002400: 7769 7468 206d 6520 6966 2079 6f75 2068  with me if you h
-00002410: 6176 6520 616e 7920 7175 6573 7469 6f6e  ave any question
-00002420: 2e20 416c 736f 2077 656c 636f 6d65 2061  . Also welcome a
-00002430: 6e79 2063 6f6e 7472 6962 7574 652e 0a0a  ny contribute...
-00002440: 4966 2079 6f75 2062 7569 6c64 2061 2063  If you build a c
-00002450: 6861 6e6e 656c 2062 7920 7468 6973 2c20  hannel by this, 
-00002460: 646f 6e27 7420 666f 7267 6574 2074 6f20  don't forget to 
-00002470: 7368 6172 6520 7468 6174 2067 6f6f 6420  share that good 
-00002480: 6e65 7773 2077 6974 6820 7573 210a 0a23  news with us!..#
-00002490: 2320 4c69 6365 6e73 650a 0a4c 6963 656e  # License..Licen
-000024a0: 7365 6420 756e 6465 7220 7468 6520 4d49  sed under the MI
-000024b0: 5420 4c69 6365 6e73 652e 0a              T License..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7465 6c65  : 2.1.Name: tele
+00000020: 6772 616d 7765 620a 5665 7273 696f 6e3a  gramweb.Version:
+00000030: 2034 2e38 0a53 756d 6d61 7279 3a20 5079   4.8.Summary: Py
+00000040: 7468 6f6e 2070 6163 6b61 6765 2066 6f72  thon package for
+00000050: 2061 7574 6f6d 6174 6963 616c 6c79 2066   automatically f
+00000060: 6574 6368 696e 6720 616e 6420 7075 7368  etching and push
+00000070: 696e 6720 6e65 7773 2062 7920 5465 6c65  ing news by Tele
+00000080: 6772 616d 2e0a 486f 6d65 2d70 6167 653a  gram..Home-page:
+00000090: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000000a0: 636f 6d2f 6372 617a 696b 732d 6372 6561  com/craziks-crea
+000000b0: 746f 722f 7465 6c65 6772 616d 2d77 6562  tor/telegram-web
+000000c0: 0a41 7574 686f 723a 2063 7261 7a69 6b73  .Author: craziks
+000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 2063  .Author-email: c
+000000e0: 6861 6e64 7261 7368 656b 6861 7270 616e  handrashekharpan
+000000f0: 6461 7930 3740 676d 6169 6c2e 636f 6d0a  day07@gmail.com.
+00000100: 4c69 6365 6e73 653a 204d 4954 0a44 6573  License: MIT.Des
+00000110: 6372 6970 7469 6f6e 3a20 3c68 3120 616c  cription: <h1 al
+00000120: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000130: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000140: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00000150: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000160: 636f 6d2f 4553 575a 592f 7465 6c65 6772  com/ESWZY/telegr
+00000170: 616d 2d6e 6577 732f 6d61 7374 6572 2f64  am-news/master/d
+00000180: 6f63 732f 696d 6167 6573 2f62 616e 6e65  ocs/images/banne
+00000190: 722e 706e 6722 2061 6c74 3d22 5465 6c65  r.png" alt="Tele
+000001a0: 6772 616d 2d6e 6577 7322 3e0a 2020 2020  gram-news">.    
+000001b0: 2020 2020 2020 3c62 723e 5465 6c65 6772        <br>Telegr
+000001c0: 616d 2d6e 6577 733c 6272 3e0a 2020 2020  am-news<br>.    
+000001d0: 2020 2020 3c2f 6831 3e0a 2020 2020 2020      </h1>.      
+000001e0: 2020 0a20 2020 2020 2020 203c 6469 7620    .        <div 
+000001f0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000200: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000210: 2050 7974 686f 6e20 7061 636b 6167 6520   Python package 
+00000220: 666f 7220 6175 746f 6d61 7469 6361 6c6c  for automaticall
+00000230: 7920 6665 7463 6869 6e67 2061 6e64 2070  y fetching and p
+00000240: 7573 6869 6e67 206e 6577 7320 6279 2054  ushing news by T
+00000250: 656c 6567 7261 6d2e 0a20 2020 2020 2020  elegram..       
+00000260: 200a 2020 2020 2020 2020 5b21 5b50 7950   .        [![PyP
+00000270: 495d 2868 7474 7073 3a2f 2f69 6d67 2e73  I](https://img.s
+00000280: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00000290: 2f74 656c 6567 7261 6d2d 6e65 7773 295d  /telegram-news)]
+000002a0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000002b0: 672f 7072 6f6a 6563 742f 7465 6c65 6772  g/project/telegr
+000002c0: 616d 2d6e 6577 732f 290a 2020 2020 2020  am-news/).      
+000002d0: 2020 215b 5079 5049 202d 2050 7974 686f    ![PyPI - Pytho
+000002e0: 6e20 5665 7273 696f 6e5d 2868 7474 7073  n Version](https
+000002f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000300: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
+00000310: 732f 7465 6c65 6772 616d 2d6e 6577 733f  s/telegram-news?
+00000320: 6c6f 676f 3d70 7974 686f 6e29 0a20 2020  logo=python).   
+00000330: 2020 2020 205b 215b 4c69 6365 6e73 655d       [![License]
+00000340: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000350: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+00000360: 6963 656e 7365 2f45 5357 5a59 2f74 656c  icense/ESWZY/tel
+00000370: 6567 7261 6d2d 6e65 7773 295d 2868 7474  egram-news)](htt
+00000380: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000390: 4553 575a 592f 7465 6c65 6772 616d 2d6e  ESWZY/telegram-n
+000003a0: 6577 732f 626c 6f62 2f6d 6173 7465 722f  ews/blob/master/
+000003b0: 4c49 4345 4e53 4529 0a20 2020 2020 2020  LICENSE).       
+000003c0: 2021 5b50 7950 4920 2d20 446f 776e 6c6f   ![PyPI - Downlo
+000003d0: 6164 735d 2868 7474 7073 3a2f 2f69 6d67  ads](https://img
+000003e0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+000003f0: 2f64 6d2f 7465 6c65 6772 616d 2d6e 6577  /dm/telegram-new
+00000400: 7329 0a20 2020 2020 2020 200a 2020 2020  s).        .    
+00000410: 2020 2020 5b21 5b42 7569 6c64 2053 7461      [![Build Sta
+00000420: 7475 735d 2868 7474 7073 3a2f 2f69 6d67  tus](https://img
+00000430: 2e73 6869 656c 6473 2e69 6f2f 7472 6176  .shields.io/trav
+00000440: 6973 2f45 5357 5a59 2f74 656c 6567 7261  is/ESWZY/telegra
+00000450: 6d2d 6e65 7773 2f6d 6173 7465 723f 6c6f  m-news/master?lo
+00000460: 676f 3d74 7261 7669 7329 5d28 6874 7470  go=travis)](http
+00000470: 733a 2f2f 7472 6176 6973 2d63 692e 6f72  s://travis-ci.or
+00000480: 672f 4553 575a 592f 7465 6c65 6772 616d  g/ESWZY/telegram
+00000490: 2d6e 6577 7329 0a20 2020 2020 2020 205b  -news).        [
+000004a0: 215b 436f 6461 6379 2042 6164 6765 5d28  ![Codacy Badge](
+000004b0: 6874 7470 733a 2f2f 6170 692e 636f 6461  https://api.coda
+000004c0: 6379 2e63 6f6d 2f70 726f 6a65 6374 2f62  cy.com/project/b
+000004d0: 6164 6765 2f47 7261 6465 2f33 6330 3766  adge/Grade/3c07f
+000004e0: 6564 3532 3564 6134 3265 3839 6464 3364  ed525da42e89dd3d
+000004f0: 3033 3736 3435 3762 3464 3229 5d28 6874  0376457b4d2)](ht
+00000500: 7470 733a 2f2f 6170 702e 636f 6461 6379  tps://app.codacy
+00000510: 2e63 6f6d 2f6d 616e 7561 6c2f 4553 575a  .com/manual/ESWZ
+00000520: 592f 7465 6c65 6772 616d 2d6e 6577 733f  Y/telegram-news?
+00000530: 7574 6d5f 736f 7572 6365 3d67 6974 6875  utm_source=githu
+00000540: 622e 636f 6d26 7574 6d5f 6d65 6469 756d  b.com&utm_medium
+00000550: 3d72 6566 6572 7261 6c26 7574 6d5f 636f  =referral&utm_co
+00000560: 6e74 656e 743d 4553 575a 592f 7465 6c65  ntent=ESWZY/tele
+00000570: 6772 616d 2d6e 6577 7326 7574 6d5f 6361  gram-news&utm_ca
+00000580: 6d70 6169 676e 3d42 6164 6765 5f47 7261  mpaign=Badge_Gra
+00000590: 6465 5f44 6173 6862 6f61 7264 290a 2020  de_Dashboard).  
+000005a0: 2020 2020 2020 215b 4c61 7374 2063 6f6d        ![Last com
+000005b0: 6d69 745d 2868 7474 7073 3a2f 2f69 6d67  mit](https://img
+000005c0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+000005d0: 7562 2f6c 6173 742d 636f 6d6d 6974 2f45  ub/last-commit/E
+000005e0: 5357 5a59 2f74 656c 6567 7261 6d2d 6e65  SWZY/telegram-ne
+000005f0: 7773 290a 2020 2020 2020 2020 5b21 5b68  ws).        [![h
+00000600: 7474 7073 3a2f 2f74 2e6d 652f 6573 777a  ttps://t.me/eswz
+00000610: 795d 2868 7474 7073 3a2f 2f69 6d67 2e73  y](https://img.s
+00000620: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000630: 5465 6c65 6772 616d 2d45 5357 5a59 2d62  Telegram-ESWZY-b
+00000640: 6c75 652e 7376 673f 6c6f 676f 3d74 656c  lue.svg?logo=tel
+00000650: 6567 7261 6d29 5d28 6874 7470 733a 2f2f  egram)](https://
+00000660: 742e 6d65 2f65 7377 7a79 290a 2020 2020  t.me/eswzy).    
+00000670: 2020 2020 0a20 2020 2020 2020 203c 2f64      .        </d
+00000680: 6976 3e0a 2020 2020 2020 2020 0a20 2020  iv>.        .   
+00000690: 2020 2020 2023 2320 496e 7472 6f64 7563       ## Introduc
+000006a0: 7469 6f6e 0a20 2020 2020 2020 200a 2020  tion.        .  
+000006b0: 2020 2020 2020 5468 6973 2069 7320 6120        This is a 
+000006c0: 6561 7379 2d74 6f2d 6c65 6172 6e2c 2066  easy-to-learn, f
+000006d0: 6c65 7869 626c 6520 616e 6420 7374 616e  lexible and stan
+000006e0: 6461 7264 697a 6564 206d 6573 7361 6765  dardized message
+000006f0: 2066 6574 6368 696e 6720 616e 6420 7075   fetching and pu
+00000700: 7368 696e 6720 6672 616d 6577 6f72 6b2c  shing framework,
+00000710: 2065 7370 6563 6961 6c6c 7920 666f 7220   especially for 
+00000720: 5b54 656c 6567 7261 6d5d 2868 7474 703a  [Telegram](http:
+00000730: 2f2f 7777 772e 7465 6c65 6772 616d 2e6f  //www.telegram.o
+00000740: 7267 2920 616e 6420 5b54 656c 6567 7261  rg) and [Telegra
+00000750: 6d20 426f 745d 2868 7474 7073 3a2f 2f63  m Bot](https://c
+00000760: 6f72 652e 7465 6c65 6772 616d 2e6f 7267  ore.telegram.org
+00000770: 2f62 6f74 7329 2e0a 2020 2020 2020 2020  /bots)..        
+00000780: 0a20 2020 2020 2020 2054 6865 2074 6172  .        The tar
+00000790: 6765 7420 6e65 7773 2073 6f75 7263 6520  get news source 
+000007a0: 6361 6e20 6265 2048 544d 4c20 7061 6765  can be HTML page
+000007b0: 2c20 4a53 4f4e 2061 6e64 2058 4d4c 2e20  , JSON and XML. 
+000007c0: 5765 2061 6c73 6f20 7072 6f76 6964 6520  We also provide 
+000007d0: 6375 7374 6f6d 697a 6564 2070 726f 6365  customized proce
+000007e0: 7373 2066 6f72 2075 6e6b 6e6f 776e 2064  ss for unknown d
+000007f0: 6174 6120 666f 726d 6174 2e0a 2020 2020  ata format..    
+00000800: 2020 2020 0a20 2020 2020 2020 2050 7573      .        Pus
+00000810: 6820 7468 6520 6c61 7465 7374 206e 6577  h the latest new
+00000820: 7320 746f 2079 6f75 7220 6368 616e 6e65  s to your channe
+00000830: 6c20 6f72 2067 726f 7570 206f 6e63 6520  l or group once 
+00000840: 6974 2068 6170 7065 6e73 210a 2020 2020  it happens!.    
+00000850: 2020 2020 0a20 2020 2020 2020 2023 2320      .        ## 
+00000860: 496e 7374 616c 6c0a 2020 2020 2020 2020  Install.        
+00000870: 0a20 2020 2020 2020 2060 6060 7368 656c  .        ```shel
+00000880: 6c0a 2020 2020 2020 2020 2420 7069 7020  l.        $ pip 
+00000890: 696e 7374 616c 6c20 7465 6c65 6772 616d  install telegram
+000008a0: 2d6e 6577 730a 2020 2020 2020 2020 6060  -news.        ``
+000008b0: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
+000008c0: 2020 204f 722c 2079 6f75 2063 616e 2069     Or, you can i
+000008d0: 6e73 7461 6c6c 2062 7920 636c 6f6e 696e  nstall by clonin
+000008e0: 6720 7468 6973 2072 6570 6f73 6974 6f72  g this repositor
+000008f0: 793a 0a20 2020 2020 2020 200a 2020 2020  y:.        .    
+00000900: 2020 2020 6060 6073 6865 6c6c 0a20 2020      ```shell.   
+00000910: 2020 2020 2024 2067 6974 2063 6c6f 6e65       $ git clone
+00000920: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000930: 636f 6d2f 4553 575a 592f 7465 6c65 6772  com/ESWZY/telegr
+00000940: 616d 2d6e 6577 732e 6769 740a 2020 2020  am-news.git.    
+00000950: 2020 2020 2420 6364 2074 656c 6567 7261      $ cd telegra
+00000960: 6d2d 6e65 7773 0a20 2020 2020 2020 2024  m-news.        $
+00000970: 2070 7974 686f 6e20 7365 7475 702e 7079   python setup.py
+00000980: 2069 6e73 7461 6c6c 0a20 2020 2020 2020   install.       
+00000990: 2060 6060 0a20 2020 2020 2020 200a 2020   ```.        .  
+000009a0: 2020 2020 2020 2323 2050 7265 7061 7265        ## Prepare
+000009b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000009c0: 2020 4974 2064 6f65 7320 6e6f 7420 6e65    It does not ne
+000009d0: 6564 206d 7563 6820 736f 2074 6861 7420  ed much so that 
+000009e0: 796f 7520 6361 6e20 7275 6e20 796f 7572  you can run your
+000009f0: 2063 6f64 6520 616e 7977 6865 7265 2e0a   code anywhere..
+00000a00: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000a10: 2046 6972 7374 2c20 6173 6b20 5b40 426f   First, ask [@Bo
+00000a20: 7446 6174 6865 725d 2868 7474 7073 3a2f  tFather](https:/
+00000a30: 2f74 2e6d 652f 626f 7466 6174 6865 7229  /t.me/botfather)
+00000a40: 2066 6f72 2061 2062 6f74 2061 6e64 2062   for a bot and b
+00000a50: 6f74 2074 6f6b 656e 2e20 4166 7465 7220  ot token. After 
+00000a60: 7468 6174 2c20 6372 6561 7465 2061 2070  that, create a p
+00000a70: 7562 6c69 6320 5b63 6861 6e6e 656c 5d28  ublic [channel](
+00000a80: 6874 7470 733a 2f2f 7465 6c65 6772 616d  https://telegram
+00000a90: 2e6f 7267 2f74 6f75 722f 6368 616e 6e65  .org/tour/channe
+00000aa0: 6c73 2920 6f72 205b 6772 6f75 705d 2868  ls) or [group](h
+00000ab0: 7474 7073 3a2f 2f74 656c 6567 7261 6d2e  ttps://telegram.
+00000ac0: 6f72 672f 746f 7572 2f67 726f 7570 7329  org/tour/groups)
+00000ad0: 2c20 616e 6420 7265 6d65 6d62 6572 2063  , and remember c
+00000ae0: 6861 7420 6964 2079 6f75 206a 7573 7420  hat id you just 
+00000af0: 6e61 6d65 642e 2044 6f20 6e6f 7420 666f  named. Do not fo
+00000b00: 7267 6574 2074 6f20 696e 7669 7465 2079  rget to invite y
+00000b10: 6f75 7220 626f 7420 696e 746f 2079 6f75  our bot into you
+00000b20: 7220 6368 616e 6e65 6c20 6f72 2067 726f  r channel or gro
+00000b30: 7570 2061 6e64 206d 616b 6520 6974 2061  up and make it a
+00000b40: 6e20 6164 6d69 6e2e 0a20 2020 2020 2020  n admin..       
+00000b50: 200a 2020 2020 2020 2020 596f 7520 616c   .        You al
+00000b60: 736f 206e 6565 6420 6120 5351 4c20 6461  so need a SQL da
+00000b70: 7461 6261 7365 2e20 416e 7920 5351 4c20  tabase. Any SQL 
+00000b80: 6461 7461 6261 7365 2069 7320 4f4b 2e20  database is OK. 
+00000b90: 4573 7065 6369 616c 6c79 2c20 4920 7265  Especially, I re
+00000ba0: 636f 6d6d 656e 6420 5b50 6f73 7467 7265  commend [Postgre
+00000bb0: 5351 4c5d 2868 7474 7073 3a2f 2f77 7777  SQL](https://www
+00000bc0: 2e70 6f73 7467 7265 7371 6c2e 6f72 672f  .postgresql.org/
+00000bd0: 292e 0a20 2020 2020 2020 200a 2020 2020  )..        .    
+00000be0: 2020 2020 2323 2051 7569 636b 2064 6570      ## Quick dep
+00000bf0: 6c6f 7920 6f6e 2048 6572 6f6b 750a 2020  loy on Heroku.  
+00000c00: 2020 2020 2020 0a20 2020 2020 2020 2043        .        C
+00000c10: 6c69 636b 20f0 9f91 8720 6275 7474 6f6e  lick .... button
+00000c20: 2074 6f20 6465 706c 6f79 2061 6e20 6578   to deploy an ex
+00000c30: 616d 706c 6520 666f 7220 6672 6565 2e20  ample for free. 
+00000c40: 5079 7468 6f6e 2065 6e76 6972 6f6e 6d65  Python environme
+00000c50: 6e74 2061 6e64 2050 6f73 7467 7265 5351  nt and PostgreSQ
+00000c60: 4c20 6461 7461 6261 7365 2068 6176 6520  L database have 
+00000c70: 6265 656e 2070 7265 7061 7265 642e 0a20  been prepared.. 
+00000c80: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000c90: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000ca0: 2f68 6572 6f6b 752e 636f 6d2f 6465 706c  /heroku.com/depl
+00000cb0: 6f79 3f74 656d 706c 6174 653d 6874 7470  oy?template=http
+00000cc0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f45  s://github.com/E
+00000cd0: 5357 5a59 2f74 656c 6567 7261 6d2d 6e65  SWZY/telegram-ne
+00000ce0: 7773 2d67 6574 7469 6e67 2d73 7461 7274  ws-getting-start
+00000cf0: 6564 223e 0a20 2020 2020 2020 2020 203c  ed">.          <
+00000d00: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000d10: 2f77 7777 2e68 6572 6f6b 7563 646e 2e63  /www.herokucdn.c
+00000d20: 6f6d 2f64 6570 6c6f 792f 6275 7474 6f6e  om/deploy/button
+00000d30: 2e73 7667 2220 616c 743d 2244 6570 6c6f  .svg" alt="Deplo
+00000d40: 7922 3e0a 2020 2020 2020 2020 3c2f 613e  y">.        </a>
+00000d50: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000d60: 2020 4166 7465 7220 6465 706c 6f79 6d65    After deployme
+00000d70: 6e74 2c20 7374 6172 7420 7468 6520 776f  nt, start the wo
+00000d80: 726b 6572 2069 6e20 2252 6573 6f75 7263  rker in "Resourc
+00000d90: 6573 2220 7461 622c 2061 6e64 2074 6865  es" tab, and the
+00000da0: 6e20 796f 7520 6361 6e20 7365 6520 7468  n you can see th
+00000db0: 6520 6566 6665 6374 2069 6e20 796f 7572  e effect in your
+00000dc0: 2063 6861 6e6e 656c 2f67 726f 7570 2c20   channel/group, 
+00000dd0: 7768 6963 6820 636f 6e74 6169 6e73 2062  which contains b
+00000de0: 6f74 6820 5343 4d50 206e 6577 7320 616e  oth SCMP news an
+00000df0: 6420 5769 6b69 206e 6577 7320 6174 2073  d Wiki news at s
+00000e00: 616d 6520 7469 6d65 2e0a 2020 2020 2020  ame time..      
+00000e10: 2020 0a20 2020 2020 2020 2023 2320 5573    .        ## Us
+00000e20: 6167 650a 2020 2020 2020 2020 0a20 2020  age.        .   
+00000e30: 2020 2020 2054 686f 7365 2061 7265 2033       Those are 3
+00000e40: 2065 7861 6d70 6c65 7320 666f 7220 796f   examples for yo
+00000e50: 7520 746f 2075 6e64 6572 7374 616e 6420  u to understand 
+00000e60: 686f 7720 746f 2075 7365 2074 6865 2066  how to use the f
+00000e70: 7261 6d65 776f 726b 2e0a 2020 2020 2020  ramework..      
+00000e80: 2020 0a20 2020 2020 2020 2023 2323 2042    .        ### B
+00000e90: 6173 6963 2045 7861 6d70 6c65 0a20 2020  asic Example.   
+00000ea0: 2020 2020 200a 2020 2020 2020 2020 6060       .        ``
+00000eb0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00000ec0: 696d 706f 7274 206f 730a 2020 2020 2020  import os.      
+00000ed0: 2020 6672 6f6d 2073 716c 616c 6368 656d    from sqlalchem
+00000ee0: 7920 696d 706f 7274 2063 7265 6174 655f  y import create_
+00000ef0: 656e 6769 6e65 0a20 2020 2020 2020 2066  engine.        f
+00000f00: 726f 6d20 7371 6c61 6c63 6865 6d79 2e6f  rom sqlalchemy.o
+00000f10: 726d 2069 6d70 6f72 7420 5365 7373 696f  rm import Sessio
+00000f20: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
+00000f30: 2020 2066 726f 6d20 7465 6c65 6772 616d     from telegram
+00000f40: 5f6e 6577 732e 7465 6d70 6c61 7465 2069  _news.template i
+00000f50: 6d70 6f72 7420 496e 666f 4578 7472 6163  mport InfoExtrac
+00000f60: 746f 722c 204e 6577 7350 6f73 746d 616e  tor, NewsPostman
+00000f70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000f80: 2020 2320 5468 7265 6520 7265 7175 6972    # Three requir
+00000f90: 6564 2066 6965 6c64 733a 0a20 2020 2020  ed fields:.     
+00000fa0: 2020 2023 2059 6f75 7220 626f 7420 746f     # Your bot to
+00000fb0: 6b65 6e20 6f62 7461 696e 6564 2066 726f  ken obtained fro
+00000fc0: 6d20 4042 6f74 4661 7468 6572 0a20 2020  m @BotFather.   
+00000fd0: 2020 2020 2062 6f74 5f74 6f6b 656e 203d       bot_token =
+00000fe0: 206f 732e 6765 7465 6e76 2822 544f 4b45   os.getenv("TOKE
+00000ff0: 4e22 290a 2020 2020 2020 2020 2320 4164  N").        # Ad
+00001000: 6420 796f 7572 2062 6f74 7320 696e 746f  d your bots into
+00001010: 2061 2063 6861 6e6e 656c 2061 7320 616e   a channel as an
+00001020: 2061 646d 696e 6973 7472 6174 6f72 0a20   administrator. 
+00001030: 2020 2020 2020 2063 6861 6e6e 656c 203d         channel =
+00001040: 206f 732e 6765 7465 6e76 2822 4348 414e   os.getenv("CHAN
+00001050: 4e45 4c22 290a 2020 2020 2020 2020 2320  NEL").        # 
+00001060: 596f 7572 2064 6174 6162 6173 6520 746f  Your database to
+00001070: 2073 746f 7265 206f 6c64 206d 6573 7361   store old messa
+00001080: 6765 732e 0a20 2020 2020 2020 2044 4154  ges..        DAT
+00001090: 4142 4153 455f 5552 4c20 3d20 6f73 2e67  ABASE_URL = os.g
+000010a0: 6574 656e 7628 2244 4154 4142 4153 455f  etenv("DATABASE_
+000010b0: 5552 4c22 290a 2020 2020 2020 2020 0a20  URL").        . 
+000010c0: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+000010d0: 6120 6461 7461 6261 7365 2073 6573 7369  a database sessi
+000010e0: 6f6e 0a20 2020 2020 2020 2065 6e67 696e  on.        engin
+000010f0: 6520 3d20 6372 6561 7465 5f65 6e67 696e  e = create_engin
+00001100: 6528 4441 5441 4241 5345 5f55 524c 290a  e(DATABASE_URL).
+00001110: 2020 2020 2020 2020 6462 203d 2053 6573          db = Ses
+00001120: 7369 6f6e 2862 696e 643d 656e 6769 6e65  sion(bind=engine
+00001130: 2e63 6f6e 6e65 6374 2829 290a 2020 2020  .connect()).    
+00001140: 2020 2020 0a20 2020 2020 2020 2023 2054      .        # T
+00001150: 6865 206e 6577 7320 736f 7572 6365 0a20  he news source. 
+00001160: 2020 2020 2020 2075 726c 203d 2022 6874         url = "ht
+00001170: 7470 733a 2f2f 656e 2e77 696b 696e 6577  tps://en.wikinew
+00001180: 732e 6f72 672f 7769 6b69 2f4d 6169 6e5f  s.org/wiki/Main_
+00001190: 5061 6765 220a 2020 2020 2020 2020 7461  Page".        ta
+000011a0: 6720 3d20 2257 696b 6920 4e65 7773 220a  g = "Wiki News".
+000011b0: 2020 2020 2020 2020 7461 626c 655f 6e61          table_na
+000011c0: 6d65 203d 2022 7769 6b69 6e65 7773 220a  me = "wikinews".
+000011d0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000011e0: 2023 2049 6e66 6f20 6578 7472 6163 746f   # Info extracto
+000011f0: 7220 746f 2070 726f 6365 7373 2064 6174  r to process dat
+00001200: 6120 666f 726d 6174 0a20 2020 2020 2020  a format.       
+00001210: 2069 6520 3d20 496e 666f 4578 7472 6163   ie = InfoExtrac
+00001220: 746f 7228 290a 2020 2020 2020 2020 0a20  tor().        . 
+00001230: 2020 2020 2020 2023 2053 656c 6563 7420         # Select 
+00001240: 7365 6c65 6374 2065 6c65 6d65 6e74 2062  select element b
+00001250: 7920 4353 532d 6261 7365 6420 7365 6c65  y CSS-based sele
+00001260: 6374 6f72 0a20 2020 2020 2020 2069 652e  ctor.        ie.
+00001270: 7365 745f 6c69 7374 5f73 656c 6563 746f  set_list_selecto
+00001280: 7228 2723 4d61 696e 5061 6765 5f6c 6174  r('#MainPage_lat
+00001290: 6573 745f 6e65 7773 5f74 6578 7420 3e20  est_news_text > 
+000012a0: 756c 203e 206c 6927 290a 2020 2020 2020  ul > li').      
+000012b0: 2020 6965 2e73 6574 5f74 6974 6c65 5f73    ie.set_title_s
+000012c0: 656c 6563 746f 7228 2723 6669 7273 7448  elector('#firstH
+000012d0: 6561 6469 6e67 2729 0a20 2020 2020 2020  eading').       
+000012e0: 2069 652e 7365 745f 7061 7261 6772 6170   ie.set_paragrap
+000012f0: 685f 7365 6c65 6374 6f72 2827 236d 772d  h_selector('#mw-
+00001300: 636f 6e74 656e 742d 7465 7874 203e 2064  content-text > d
+00001310: 6976 203e 2070 3a6e 6f74 2870 3a6e 7468  iv > p:not(p:nth
+00001320: 2d63 6869 6c64 2831 2929 2729 0a20 2020  -child(1))').   
+00001330: 2020 2020 2069 652e 7365 745f 7469 6d65       ie.set_time
+00001340: 5f73 656c 6563 746f 7228 2723 6d77 2d63  _selector('#mw-c
+00001350: 6f6e 7465 6e74 2d74 6578 7420 3e20 6469  ontent-text > di
+00001360: 7620 3e20 703a 6e74 682d 6368 696c 6428  v > p:nth-child(
+00001370: 3129 203e 2073 7472 6f6e 6727 290a 2020  1) > strong').  
+00001380: 2020 2020 2020 6965 2e73 6574 5f73 6f75        ie.set_sou
+00001390: 7263 655f 7365 6c65 6374 6f72 2827 7370  rce_selector('sp
+000013a0: 616e 2e73 6f75 7263 6554 656d 706c 6174  an.sourceTemplat
+000013b0: 6527 290a 2020 2020 2020 2020 0a20 2020  e').        .   
+000013c0: 2020 2020 2023 2053 6574 2061 206d 6178       # Set a max
+000013d0: 206c 656e 6774 6820 666f 7220 706f 7374   length for post
+000013e0: 2c20 4d61 7820 6973 2034 3039 360a 2020  , Max is 4096.  
+000013f0: 2020 2020 2020 6965 2e6d 6178 5f70 6f73        ie.max_pos
+00001400: 745f 6c65 6e67 7468 203d 2032 3030 300a  t_length = 2000.
+00001410: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001420: 2023 204e 6577 7320 706f 7374 6d61 6e20   # News postman 
+00001430: 746f 206d 616e 6167 6520 7365 6e64 696e  to manage sendin
+00001440: 6720 6166 6661 6972 0a20 2020 2020 2020  g affair.       
+00001450: 206e 7020 3d20 4e65 7773 506f 7374 6d61   np = NewsPostma
+00001460: 6e28 6c69 7374 5552 4c73 3d5b 7572 6c2c  n(listURLs=[url,
+00001470: 205d 2c20 7365 6e64 4c69 7374 3d5b 6368   ], sendList=[ch
+00001480: 616e 6e65 6c2c 205d 2c20 6462 3d64 622c  annel, ], db=db,
+00001490: 2074 6167 3d74 6167 290a 2020 2020 2020   tag=tag).      
+000014a0: 2020 6e70 2e73 6574 5f62 6f74 5f74 6f6b    np.set_bot_tok
+000014b0: 656e 2862 6f74 5f74 6f6b 656e 290a 2020  en(bot_token).  
+000014c0: 2020 2020 2020 6e70 2e73 6574 5f65 7874        np.set_ext
+000014d0: 7261 6374 6f72 2869 6529 0a20 2020 2020  ractor(ie).     
+000014e0: 2020 206e 702e 7365 745f 7461 626c 655f     np.set_table_
+000014f0: 6e61 6d65 2874 6162 6c65 5f6e 616d 6529  name(table_name)
+00001500: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001510: 2020 2320 5374 6172 7420 746f 2077 6f72    # Start to wor
+00001520: 6b21 0a20 2020 2020 2020 206e 702e 706f  k!.        np.po
+00001530: 6c6c 2829 0a20 2020 2020 2020 2060 6060  ll().        ```
+00001540: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001550: 2020 5479 7069 6361 6c20 7265 7375 6c74    Typical result
+00001560: 733a 0a20 2020 2020 2020 200a 2020 2020  s:.        .    
+00001570: 2020 2020 3c64 6976 2061 6c69 676e 3d22      <div align="
+00001580: 6365 6e74 6572 223e 0a20 2020 2020 2020  center">.       
+00001590: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+000015a0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+000015b0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f45  sercontent.com/E
+000015c0: 5357 5a59 2f74 656c 6567 7261 6d2d 6e65  SWZY/telegram-ne
+000015d0: 7773 2f6d 6173 7465 722f 646f 6373 2f69  ws/master/docs/i
+000015e0: 6d61 6765 732f 6465 6d6f 312e 706e 6722  mages/demo1.png"
+000015f0: 2061 6c74 3d22 4465 6d6f 2031 2220 7769   alt="Demo 1" wi
+00001600: 6474 683d 2234 3025 223e 0a20 2020 2020  dth="40%">.     
+00001610: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+00001620: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00001630: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00001640: 2f45 5357 5a59 2f74 656c 6567 7261 6d2d  /ESWZY/telegram-
+00001650: 6e65 7773 2f6d 6173 7465 722f 646f 6373  news/master/docs
+00001660: 2f69 6d61 6765 732f 6465 6d6f 322e 706e  /images/demo2.pn
+00001670: 6722 2061 6c74 3d22 4465 6d6f 2032 2220  g" alt="Demo 2" 
+00001680: 7769 6474 683d 2234 3025 223e 0a20 2020  width="40%">.   
+00001690: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+000016a0: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+000016b0: 2041 6476 616e 6365 6420 4578 616d 706c   Advanced Exampl
+000016c0: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
+000016d0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+000016e0: 2020 2020 2069 6d70 6f72 7420 6f73 0a20       import os. 
+000016f0: 2020 2020 2020 2066 726f 6d20 7371 6c61         from sqla
+00001700: 6c63 6865 6d79 2069 6d70 6f72 7420 6372  lchemy import cr
+00001710: 6561 7465 5f65 6e67 696e 650a 2020 2020  eate_engine.    
+00001720: 2020 2020 6672 6f6d 2073 716c 616c 6368      from sqlalch
+00001730: 656d 792e 6f72 6d20 696d 706f 7274 2053  emy.orm import S
+00001740: 6573 7369 6f6e 0a20 2020 2020 2020 2066  ession.        f
+00001750: 726f 6d20 7465 6c65 6772 616d 5f6e 6577  rom telegram_new
+00001760: 732e 7465 6d70 6c61 7465 2069 6d70 6f72  s.template impor
+00001770: 7420 496e 666f 4578 7472 6163 746f 722c  t InfoExtractor,
+00001780: 204e 6577 7350 6f73 746d 616e 0a20 2020   NewsPostman.   
+00001790: 2020 2020 2062 6f74 5f74 6f6b 656e 203d       bot_token =
+000017a0: 206f 732e 6765 7465 6e76 2822 544f 4b45   os.getenv("TOKE
+000017b0: 4e22 290a 2020 2020 2020 2020 6368 616e  N").        chan
+000017c0: 6e65 6c20 3d20 6f73 2e67 6574 656e 7628  nel = os.getenv(
+000017d0: 2243 4841 4e4e 454c 2229 0a20 2020 2020  "CHANNEL").     
+000017e0: 2020 2044 4154 4142 4153 455f 5552 4c20     DATABASE_URL 
+000017f0: 3d20 6f73 2e67 6574 656e 7628 2244 4154  = os.getenv("DAT
+00001800: 4142 4153 455f 5552 4c22 290a 2020 2020  ABASE_URL").    
+00001810: 2020 2020 656e 6769 6e65 203d 2063 7265      engine = cre
+00001820: 6174 655f 656e 6769 6e65 2844 4154 4142  ate_engine(DATAB
+00001830: 4153 455f 5552 4c29 0a20 2020 2020 2020  ASE_URL).       
+00001840: 2064 6220 3d20 5365 7373 696f 6e28 6269   db = Session(bi
+00001850: 6e64 3d65 6e67 696e 652e 636f 6e6e 6563  nd=engine.connec
+00001860: 7428 2929 0a20 2020 2020 2020 200a 2020  t()).        .  
+00001870: 2020 2020 2020 2320 4162 6f76 6520 636f        # Above co
+00001880: 6465 2069 7320 6173 2073 616d 6520 6173  de is as same as
+00001890: 2074 6865 2062 6173 6963 2065 7861 6d70   the basic examp
+000018a0: 6c65 2c20 796f 7520 6361 6e20 7265 7573  le, you can reus
+000018b0: 6520 7468 6f73 6520 636f 6465 2064 6972  e those code dir
+000018c0: 6563 746c 790a 2020 2020 2020 2020 0a20  ectly.        . 
+000018d0: 2020 2020 2020 2075 726c 5f32 203d 2022         url_2 = "
+000018e0: 6874 7470 733a 2f2f 7777 772e 636e 6265  https://www.cnbe
+000018f0: 7461 2e63 6f6d 2f22 0a20 2020 2020 2020  ta.com/".       
+00001900: 2074 6167 5f32 203d 2022 636e 4265 7461   tag_2 = "cnBeta
+00001910: 220a 2020 2020 2020 2020 7461 626c 655f  ".        table_
+00001920: 6e61 6d65 5f32 203d 2022 636e 6265 7461  name_2 = "cnbeta
+00001930: 6e65 7773 220a 2020 2020 2020 2020 0a20  news".        . 
+00001940: 2020 2020 2020 2069 655f 3220 3d20 496e         ie_2 = In
+00001950: 666f 4578 7472 6163 746f 7228 290a 2020  foExtractor().  
+00001960: 2020 2020 2020 6965 5f32 2e73 6574 5f6c        ie_2.set_l
+00001970: 6973 745f 7365 6c65 6374 6f72 2827 2e69  ist_selector('.i
+00001980: 7465 6d73 2d61 7265 6120 3e20 6469 7620  tems-area > div 
+00001990: 3e20 646c 203e 2064 7420 3e20 6127 290a  > dl > dt > a').
+000019a0: 2020 2020 2020 2020 6965 5f32 2e73 6574          ie_2.set
+000019b0: 5f74 6974 6c65 5f73 656c 6563 746f 7228  _title_selector(
+000019c0: 2768 6561 6465 7220 3e20 6831 2729 0a20  'header > h1'). 
+000019d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000019e0: 2320 5365 6c65 6374 206d 616e 7920 7461  # Select many ta
+000019f0: 7267 6574 2061 7420 7361 6d65 2074 696d  rget at same tim
+00001a00: 6520 2020 200a 2020 2020 2020 2020 6965  e    .        ie
+00001a10: 5f32 2e73 6574 5f70 6172 6167 7261 7068  _2.set_paragraph
+00001a20: 5f73 656c 6563 746f 7228 2764 6976 2e63  _selector('div.c
+00001a30: 6e62 6574 612d 6172 7469 636c 652d 626f  nbeta-article-bo
+00001a40: 6479 203e 2064 6976 2e61 7274 6963 6c65  dy > div.article
+00001a50: 2d73 756d 6d61 7279 203e 2070 2c20 2720  -summary > p, ' 
+00001a60: 2023 2053 756d 6d61 7279 206f 6e6c 790a   # Summary only.
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a90: 2020 2020 2764 6976 2e63 6e62 6574 612d      'div.cnbeta-
+00001aa0: 6172 7469 636c 652d 626f 6479 203e 2064  article-body > d
+00001ab0: 6976 2e61 7274 6963 6c65 2d63 6f6e 7465  iv.article-conte
+00001ac0: 6e74 203e 2070 2729 2020 2023 2043 6f6e  nt > p')   # Con
+00001ad0: 7465 6e74 206f 6e6c 790a 2020 2020 2020  tent only.      
+00001ae0: 2020 6965 5f32 2e73 6574 5f74 696d 655f    ie_2.set_time_
+00001af0: 7365 6c65 6374 6f72 2827 6865 6164 6572  selector('header
+00001b00: 203e 2064 6976 203e 2073 7061 6e3a 6e74   > div > span:nt
+00001b10: 682d 6368 696c 6428 3129 2729 0a20 2020  h-child(1)').   
+00001b20: 2020 2020 2069 655f 322e 7365 745f 736f       ie_2.set_so
+00001b30: 7572 6365 5f73 656c 6563 746f 7228 2768  urce_selector('h
+00001b40: 6561 6465 7220 3e20 6469 7620 3e20 7370  eader > div > sp
+00001b50: 616e 2e73 6f75 7263 6527 290a 2020 2020  an.source').    
+00001b60: 2020 2020 0a20 2020 2020 2020 2023 2053      .        # S
+00001b70: 656c 6563 7420 696d 6167 6520 746f 2064  elect image to d
+00001b80: 6973 706c 6179 2c20 7468 656e 2074 6865  isplay, then the
+00001b90: 206d 6178 206c 656e 6774 6820 6973 2064   max length is d
+00001ba0: 6f77 6e20 746f 2031 3032 340a 2020 2020  own to 1024.    
+00001bb0: 2020 2020 6965 5f32 2e73 6574 5f69 6d61      ie_2.set_ima
+00001bc0: 6765 5f73 656c 6563 746f 7228 2764 6976  ge_selector('div
+00001bd0: 2e63 6e62 6574 612d 6172 7469 636c 652d  .cnbeta-article-
+00001be0: 626f 6479 203e 2064 6976 2e61 7274 6963  body > div.artic
+00001bf0: 6c65 2d73 756d 6d61 7279 203e 2070 2069  le-summary > p i
+00001c00: 6d67 2c20 2720 2023 2046 726f 6d20 7375  mg, '  # From su
+00001c10: 6d6d 6172 7920 6f6e 6c79 0a20 2020 2020  mmary only.     
+00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c30: 2020 2020 2020 2020 2020 2027 6469 762e             'div.
+00001c40: 636e 6265 7461 2d61 7274 6963 6c65 2d62  cnbeta-article-b
+00001c50: 6f64 7920 3e20 6469 762e 6172 7469 636c  ody > div.articl
+00001c60: 652d 636f 6e74 656e 7420 3e20 7020 696d  e-content > p im
+00001c70: 6727 2920 2020 2320 4672 6f6d 2063 6f6e  g')   # From con
+00001c80: 7465 6e74 206f 6e6c 790a 2020 2020 2020  tent only.      
+00001c90: 2020 6965 5f32 2e6d 6178 5f70 6f73 745f    ie_2.max_post_
+00001ca0: 6c65 6e67 7468 203d 2031 3030 300a 2020  length = 1000.  
+00001cb0: 2020 2020 2020 0a20 2020 2020 2020 206e        .        n
+00001cc0: 705f 3220 3d20 4e65 7773 506f 7374 6d61  p_2 = NewsPostma
+00001cd0: 6e28 6c69 7374 5552 4c73 3d5b 7572 6c5f  n(listURLs=[url_
+00001ce0: 322c 205d 2c20 7365 6e64 4c69 7374 3d5b  2, ], sendList=[
+00001cf0: 6368 616e 6e65 6c5d 2c20 7461 673d 7461  channel], tag=ta
+00001d00: 675f 322c 2064 623d 6462 290a 2020 2020  g_2, db=db).    
+00001d10: 2020 2020 6e70 5f32 2e73 6574 5f65 7874      np_2.set_ext
+00001d20: 7261 6374 6f72 2869 655f 3229 0a20 2020  ractor(ie_2).   
+00001d30: 2020 2020 206e 705f 322e 7365 745f 7461       np_2.set_ta
+00001d40: 626c 655f 6e61 6d65 2874 6162 6c65 5f6e  ble_name(table_n
+00001d50: 616d 655f 3229 0a20 2020 2020 2020 206e  ame_2).        n
+00001d60: 705f 322e 706f 6c6c 2829 0a20 2020 2020  p_2.poll().     
+00001d70: 2020 2060 6060 0a20 2020 2020 2020 200a     ```.        .
+00001d80: 2020 2020 2020 2020 5479 7069 6361 6c20          Typical 
+00001d90: 7265 7375 6c74 733a 0a20 2020 2020 2020  results:.       
+00001da0: 200a 2020 2020 2020 2020 3c64 6976 2061   .        <div a
+00001db0: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00001dc0: 2020 2020 2020 2020 203c 696d 6720 7372           <img sr
+00001dd0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00001de0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001df0: 2e63 6f6d 2f45 5357 5a59 2f74 656c 6567  .com/ESWZY/teleg
+00001e00: 7261 6d2d 6e65 7773 2f6d 6173 7465 722f  ram-news/master/
+00001e10: 646f 6373 2f69 6d61 6765 732f 6465 6d6f  docs/images/demo
+00001e20: 332e 706e 6722 2061 6c74 3d22 4465 6d6f  3.png" alt="Demo
+00001e30: 2033 2220 7769 6474 683d 2234 3025 223e   3" width="40%">
+00001e40: 0a20 2020 2020 2020 2020 203c 696d 6720  .          <img 
+00001e50: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00001e60: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00001e70: 6e74 2e63 6f6d 2f45 5357 5a59 2f74 656c  nt.com/ESWZY/tel
+00001e80: 6567 7261 6d2d 6e65 7773 2f6d 6173 7465  egram-news/maste
+00001e90: 722f 646f 6373 2f69 6d61 6765 732f 6465  r/docs/images/de
+00001ea0: 6d6f 342e 706e 6722 2061 6c74 3d22 4465  mo4.png" alt="De
+00001eb0: 6d6f 2034 2220 7769 6474 683d 2234 3025  mo 4" width="40%
+00001ec0: 223e 0a20 2020 2020 2020 203c 2f64 6976  ">.        </div
+00001ed0: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
+00001ee0: 2020 2023 2323 2041 6476 616e 6365 6420     ### Advanced 
+00001ef0: 4578 616d 706c 6520 666f 7220 4a53 4f4e  Example for JSON
+00001f00: 2061 6e64 2058 4d4c 0a20 2020 2020 2020   and XML.       
+00001f10: 200a 2020 2020 2020 2020 5468 6520 6861   .        The ha
+00001f20: 6e64 6c65 2066 6f72 204a 534f 4e20 616e  ndle for JSON an
+00001f30: 6420 584d 4c20 6172 6520 7175 6974 6520  d XML are quite 
+00001f40: 7369 6d69 6c61 722e 2059 6f75 2063 616e  similar. You can
+00001f50: 2063 6f6e 7665 7274 2058 4d4c 2074 6f20   convert XML to 
+00001f60: 4a53 4f4e 2062 7920 6675 6e63 7469 6f6e  JSON by function
+00001f70: 2060 7465 6c65 6772 616d 5f6e 6577 732e   `telegram_news.
+00001f80: 7574 696c 732e 786d 6c5f 746f 5f6a 736f  utils.xml_to_jso
+00001f90: 6e60 2c20 616e 6420 7573 6520 604e 6577  n`, and use `New
+00001fa0: 7350 6f73 746d 616e 4a53 4f4e 6020 616e  sPostmanJSON` an
+00001fb0: 6420 6049 6e66 6f45 7874 7261 6374 6f72  d `InfoExtractor
+00001fc0: 4a53 4f4e 602e 204f 722c 2079 6f75 2063  JSON`. Or, you c
+00001fd0: 616e 2075 7365 2060 4e65 7773 506f 7374  an use `NewsPost
+00001fe0: 6d61 6e58 4d4c 6020 616e 6420 6049 6e66  manXML` and `Inf
+00001ff0: 6f45 7874 7261 6374 6f72 584d 4c60 2064  oExtractorXML` d
+00002000: 6972 6563 746c 792e 0a20 2020 2020 2020  irectly..       
+00002010: 200a 2020 2020 2020 2020 596f 7520 7368   .        You sh
+00002020: 6f75 6c64 2075 7365 206b 6579 206c 6973  ould use key lis
+00002030: 7420 746f 2072 6563 7572 7369 7665 6c79  t to recursively
+00002040: 2072 6f75 7465 2074 6f20 7468 6520 696e   route to the in
+00002050: 666f 726d 6174 696f 6e20 796f 7520 7761  formation you wa
+00002060: 6e74 2e0a 2020 2020 2020 2020 0a20 2020  nt..        .   
+00002070: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
+00002080: 2020 2020 2020 2069 6d70 6f72 7420 6861         import ha
+00002090: 7368 6c69 620a 2020 2020 2020 2020 696d  shlib.        im
+000020a0: 706f 7274 206a 736f 6e0a 2020 2020 2020  port json.      
+000020b0: 2020 696d 706f 7274 206f 730a 2020 2020    import os.    
+000020c0: 2020 2020 6672 6f6d 2073 716c 616c 6368      from sqlalch
+000020d0: 656d 7920 696d 706f 7274 2063 7265 6174  emy import creat
+000020e0: 655f 656e 6769 6e65 0a20 2020 2020 2020  e_engine.       
+000020f0: 2066 726f 6d20 7371 6c61 6c63 6865 6d79   from sqlalchemy
+00002100: 2e6f 726d 2069 6d70 6f72 7420 5365 7373  .orm import Sess
+00002110: 696f 6e0a 2020 2020 2020 2020 6672 6f6d  ion.        from
+00002120: 2074 656c 6567 7261 6d5f 6e65 7773 2e74   telegram_news.t
+00002130: 656d 706c 6174 6520 696d 706f 7274 2049  emplate import I
+00002140: 6e66 6f45 7874 7261 6374 6f72 4a53 4f4e  nfoExtractorJSON
+00002150: 2c20 4e65 7773 506f 7374 6d61 6e4a 534f  , NewsPostmanJSO
+00002160: 4e0a 2020 2020 2020 2020 6672 6f6d 2074  N.        from t
+00002170: 656c 6567 7261 6d5f 6e65 7773 2e75 7469  elegram_news.uti
+00002180: 6c73 2069 6d70 6f72 7420 786d 6c5f 746f  ls import xml_to
+00002190: 5f6a 736f 6e0a 2020 2020 2020 2020 626f  _json.        bo
+000021a0: 745f 746f 6b65 6e20 3d20 6f73 2e67 6574  t_token = os.get
+000021b0: 656e 7628 2254 4f4b 454e 2229 0a20 2020  env("TOKEN").   
+000021c0: 2020 2020 2063 6861 6e6e 656c 203d 206f       channel = o
+000021d0: 732e 6765 7465 6e76 2822 4348 414e 4e45  s.getenv("CHANNE
+000021e0: 4c22 290a 2020 2020 2020 2020 4441 5441  L").        DATA
+000021f0: 4241 5345 5f55 524c 203d 206f 732e 6765  BASE_URL = os.ge
+00002200: 7465 6e76 2822 4441 5441 4241 5345 5f55  tenv("DATABASE_U
+00002210: 524c 2229 0a20 2020 2020 2020 2065 6e67  RL").        eng
+00002220: 696e 6520 3d20 6372 6561 7465 5f65 6e67  ine = create_eng
+00002230: 696e 6528 4441 5441 4241 5345 5f55 524c  ine(DATABASE_URL
+00002240: 290a 2020 2020 2020 2020 6462 203d 2053  ).        db = S
+00002250: 6573 7369 6f6e 2862 696e 643d 656e 6769  ession(bind=engi
+00002260: 6e65 2e63 6f6e 6e65 6374 2829 290a 2020  ne.connect()).  
+00002270: 2020 2020 2020 0a20 2020 2020 2020 2075        .        u
+00002280: 726c 5f33 203d 2022 6874 7470 733a 2f2f  rl_3 = "https://
+00002290: 7777 772e 7363 6d70 2e63 6f6d 2f72 7373  www.scmp.com/rss
+000022a0: 2f39 312f 6665 6564 220a 2020 2020 2020  /91/feed".      
+000022b0: 2020 7461 675f 3320 3d20 2253 434d 5022    tag_3 = "SCMP"
+000022c0: 0a20 2020 2020 2020 2074 6162 6c65 5f6e  .        table_n
+000022d0: 616d 655f 3320 3d20 2273 636d 706e 6577  ame_3 = "scmpnew
+000022e0: 7322 0a20 2020 2020 2020 200a 2020 2020  s".        .    
+000022f0: 2020 2020 6965 5f33 203d 2049 6e66 6f45      ie_3 = InfoE
+00002300: 7874 7261 6374 6f72 4a53 4f4e 2829 0a20  xtractorJSON(). 
+00002310: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002320: 2320 5072 652d 7072 6f63 6573 7320 7468  # Pre-process th
+00002330: 6520 584d 4c20 7374 7269 6e67 2c20 636f  e XML string, co
+00002340: 6e76 6572 7420 746f 204a 534f 4e20 7374  nvert to JSON st
+00002350: 7269 6e67 0a20 2020 2020 2020 2064 6566  ring.        def
+00002360: 206c 6973 745f 7072 655f 7072 6f63 6573   list_pre_proces
+00002370: 7328 7465 7874 293a 0a20 2020 2020 2020  s(text):.       
+00002380: 2020 2020 2074 6578 7420 3d20 6a73 6f6e       text = json
+00002390: 2e6c 6f61 6473 2878 6d6c 5f74 6f5f 6a73  .loads(xml_to_js
+000023a0: 6f6e 2874 6578 7429 290a 2020 2020 2020  on(text)).      
+000023b0: 2020 2020 2020 7265 7475 726e 206a 736f        return jso
+000023c0: 6e2e 6475 6d70 7328 7465 7874 290a 2020  n.dumps(text).  
+000023d0: 2020 2020 2020 6965 5f33 2e73 6574 5f6c        ie_3.set_l
+000023e0: 6973 745f 7072 655f 7072 6f63 6573 735f  ist_pre_process_
+000023f0: 706f 6c69 6379 286c 6973 745f 7072 655f  policy(list_pre_
+00002400: 7072 6f63 6573 7329 0a20 2020 2020 2020  process).       
+00002410: 200a 2020 2020 2020 2020 2320 526f 7574   .        # Rout
+00002420: 6520 6279 206b 6579 206c 6973 740a 2020  e by key list.  
+00002430: 2020 2020 2020 6965 5f33 2e73 6574 5f6c        ie_3.set_l
+00002440: 6973 745f 726f 7574 6572 285b 2772 7373  ist_router(['rss
+00002450: 272c 2027 6368 616e 6e65 6c27 2c20 2769  ', 'channel', 'i
+00002460: 7465 6d27 5d29 0a20 2020 2020 2020 2069  tem']).        i
+00002470: 655f 332e 7365 745f 6c69 6e6b 5f72 6f75  e_3.set_link_rou
+00002480: 7465 7228 5b27 6c69 6e6b 275d 290a 2020  ter(['link']).  
+00002490: 2020 2020 2020 6965 5f33 2e73 6574 5f74        ie_3.set_t
+000024a0: 6974 6c65 5f72 6f75 7465 7228 5b27 7469  itle_router(['ti
+000024b0: 746c 6527 5d29 0a20 2020 2020 2020 2069  tle']).        i
+000024c0: 655f 332e 7365 745f 7061 7261 6772 6170  e_3.set_paragrap
+000024d0: 6873 5f72 6f75 7465 7228 5b27 6465 7363  hs_router(['desc
+000024e0: 7269 7074 696f 6e27 5d29 0a20 2020 2020  ription']).     
+000024f0: 2020 2069 655f 332e 7365 745f 7469 6d65     ie_3.set_time
+00002500: 5f72 6f75 7465 7228 5b27 7075 6244 6174  _router(['pubDat
+00002510: 6527 5d29 0a20 2020 2020 2020 2069 655f  e']).        ie_
+00002520: 332e 7365 745f 736f 7572 6365 5f72 6f75  3.set_source_rou
+00002530: 7465 7228 5b27 6175 7468 6f72 275d 290a  ter(['author']).
+00002540: 2020 2020 2020 2020 6965 5f33 2e73 6574          ie_3.set
+00002550: 5f69 6d61 6765 5f72 6f75 7465 7228 5b27  _image_router(['
+00002560: 6d65 6469 613a 7468 756d 626e 6169 6c27  media:thumbnail'
+00002570: 2c20 2740 7572 6c27 5d29 0a20 2020 2020  , '@url']).     
+00002580: 2020 200a 2020 2020 2020 2020 2320 4375     .        # Cu
+00002590: 7374 6f6d 697a 6520 4944 2066 6f72 206e  stomize ID for n
+000025a0: 6577 7320 6974 656d 0a20 2020 2020 2020  ews item.       
+000025b0: 2064 6566 2069 645f 706f 6c69 6379 286c   def id_policy(l
+000025c0: 696e 6b29 3a0a 2020 2020 2020 2020 2020  ink):.          
+000025d0: 2020 7265 7475 726e 2068 6173 686c 6962    return hashlib
+000025e0: 2e6d 6435 286c 696e 6b2e 656e 636f 6465  .md5(link.encode
+000025f0: 2822 7574 662d 3822 2929 2e68 6578 6469  ("utf-8")).hexdi
+00002600: 6765 7374 2829 0a20 2020 2020 2020 2069  gest().        i
+00002610: 655f 332e 7365 745f 6964 5f70 6f6c 6963  e_3.set_id_polic
+00002620: 7928 6964 5f70 6f6c 6963 7929 0a20 2020  y(id_policy).   
+00002630: 2020 2020 200a 2020 2020 2020 2020 6e70       .        np
+00002640: 5f33 203d 204e 6577 7350 6f73 746d 616e  _3 = NewsPostman
+00002650: 4a53 4f4e 286c 6973 7455 524c 733d 5b75  JSON(listURLs=[u
+00002660: 726c 5f33 5d2c 2073 656e 644c 6973 743d  rl_3], sendList=
+00002670: 5b63 6861 6e6e 656c 5d2c 2064 623d 6462  [channel], db=db
+00002680: 2c20 7461 673d 7461 675f 3329 0a20 2020  , tag=tag_3).   
+00002690: 2020 2020 206e 705f 332e 7365 745f 6578       np_3.set_ex
+000026a0: 7472 6163 746f 7228 6965 5f33 290a 2020  tractor(ie_3).  
+000026b0: 2020 2020 2020 6e70 5f33 2e73 6574 5f74        np_3.set_t
+000026c0: 6162 6c65 5f6e 616d 6528 7461 626c 655f  able_name(table_
+000026d0: 6e61 6d65 5f33 290a 2020 2020 2020 2020  name_3).        
+000026e0: 6e70 5f33 2e70 6f6c 6c28 290a 2020 2020  np_3.poll().    
+000026f0: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+00002700: 0a20 2020 2020 2020 2054 7970 6963 616c  .        Typical
+00002710: 2072 6573 756c 7473 3a0a 2020 2020 2020   results:.      
+00002720: 2020 0a20 2020 2020 2020 203c 6469 7620    .        <div 
+00002730: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00002740: 2020 2020 2020 2020 2020 3c69 6d67 2073            <img s
+00002750: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002760: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002770: 742e 636f 6d2f 4553 575a 592f 7465 6c65  t.com/ESWZY/tele
+00002780: 6772 616d 2d6e 6577 732f 6d61 7374 6572  gram-news/master
+00002790: 2f64 6f63 732f 696d 6167 6573 2f64 656d  /docs/images/dem
+000027a0: 6f35 2e70 6e67 2220 616c 743d 2244 656d  o5.png" alt="Dem
+000027b0: 6f20 3522 2077 6964 7468 3d22 3430 2522  o 5" width="40%"
+000027c0: 3e0a 2020 2020 2020 2020 2020 3c69 6d67  >.          <img
+000027d0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+000027e0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+000027f0: 656e 742e 636f 6d2f 4553 575a 592f 7465  ent.com/ESWZY/te
+00002800: 6c65 6772 616d 2d6e 6577 732f 6d61 7374  legram-news/mast
+00002810: 6572 2f64 6f63 732f 696d 6167 6573 2f64  er/docs/images/d
+00002820: 656d 6f36 2e70 6e67 2220 616c 743d 2244  emo6.png" alt="D
+00002830: 656d 6f20 3622 2077 6964 7468 3d22 3430  emo 6" width="40
+00002840: 2522 3e0a 2020 2020 2020 2020 3c2f 6469  %">.        </di
+00002850: 763e 0a20 2020 2020 2020 200a 2020 2020  v>.        .    
+00002860: 2020 2020 2323 2320 5061 7261 6c6c 656c      ### Parallel
+00002870: 2050 726f 6772 616d 0a20 2020 2020 2020   Program.       
+00002880: 200a 2020 2020 2020 2020 4966 2079 6f75   .        If you
+00002890: 2075 7365 2074 6865 2073 616d 6520 6461   use the same da
+000028a0: 7461 6261 7365 2061 6e64 2073 656e 6420  tabase and send 
+000028b0: 746f 2074 6865 2073 616d 6520 6368 616e  to the same chan
+000028c0: 6e65 6c2c 2079 6f75 2063 616e 2073 696d  nel, you can sim
+000028d0: 706c 7920 6a6f 696e 7420 6561 6368 2070  ply joint each p
+000028e0: 6172 7420 6f66 2063 6f64 6520 626c 6f63  art of code bloc
+000028f0: 6b2c 2061 6e64 2063 616c 6c20 6070 6f6c  k, and call `pol
+00002900: 6c28 2960 2066 756e 6374 696f 6e20 7369  l()` function si
+00002910: 6d75 6c74 616e 656f 7573 6c79 2e0a 2020  multaneously..  
+00002920: 2020 2020 2020 0a20 2020 2020 2020 2041        .        A
+00002930: 6e20 6578 616d 706c 6520 796f 7520 6361  n example you ca
+00002940: 6e20 6669 6e64 2069 6e20 6f75 7220 4865  n find in our He
+00002950: 726f 6b75 2064 6570 6c6f 7920 7465 6d70  roku deploy temp
+00002960: 6c61 7465 2072 6570 6f3a 200a 2020 2020  late repo: .    
+00002970: 2020 2020 0a20 2020 2020 2020 2068 7474      .        htt
+00002980: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002990: 4553 575a 592f 7465 6c65 6772 616d 2d6e  ESWZY/telegram-n
+000029a0: 6577 732d 6765 7474 696e 672d 7374 6172  ews-getting-star
+000029b0: 7465 642f 626c 6f62 2f6d 6173 7465 722f  ted/blob/master/
+000029c0: 6d61 696e 2e70 790a 2020 2020 2020 2020  main.py.        
+000029d0: 0a20 2020 2020 2020 2023 2320 4578 616d  .        ## Exam
+000029e0: 706c 6520 4368 616e 6e65 6c0a 2020 2020  ple Channel.    
+000029f0: 2020 2020 0a20 2020 2020 2020 2041 2054      .        A T
+00002a00: 656c 6567 7261 6d20 6368 616e 6e65 6c20  elegram channel 
+00002a10: 6f66 205b 6261 7369 6320 6578 616d 706c  of [basic exampl
+00002a20: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00002a30: 622e 636f 6d2f 4553 575a 592f 7465 6c65  b.com/ESWZY/tele
+00002a40: 6772 616d 2d6e 6577 7323 6261 7369 632d  gram-news#basic-
+00002a50: 6578 616d 706c 6529 2066 6f72 2045 6e67  example) for Eng
+00002a60: 6c69 7368 2057 696b 696e 6577 733a 205b  lish Wikinews: [
+00002a70: 7e7e 4077 696b 696e 6577 735f 656e 7e7e  ~~@wikinews_en~~
+00002a80: 5d28 6874 7470 733a 2f2f 742e 6d65 2f6a  ](https://t.me/j
+00002a90: 6f69 6e63 6861 742f 5437 5462 4a55 5770  oinchat/T7TbJUWp
+00002aa0: 6755 7047 6d61 7259 2920 2869 6e20 456e  gUpGmarY) (in En
+00002ab0: 676c 6973 6829 0a20 2020 2020 2020 200a  glish).        .
+00002ac0: 2020 2020 2020 2020 4120 5465 6c65 6772          A Telegr
+00002ad0: 616d 2063 6861 6e6e 656c 2066 6f72 2072  am channel for r
+00002ae0: 6561 6c74 696d 6520 6561 7274 6871 7561  ealtime earthqua
+00002af0: 6b65 2077 6172 6e69 6e67 2070 6f77 6572  ke warning power
+00002b00: 6564 2062 7920 5465 6c65 6772 616d 2d6e  ed by Telegram-n
+00002b10: 6577 733a 205b 4065 6172 7468 7175 616b  ews: [@earthquak
+00002b20: 655f 616c 6572 745d 2868 7474 7073 3a2f  e_alert](https:/
+00002b30: 2f74 2e6d 652f 732f 6561 7274 6871 7561  /t.me/s/earthqua
+00002b40: 6b65 5f61 6c65 7274 2920 2869 6e20 4368  ke_alert) (in Ch
+00002b50: 696e 6573 6529 0a20 2020 2020 2020 200a  inese).        .
+00002b60: 2020 2020 2020 2020 2323 2054 4f44 4f0a          ## TODO.
+00002b70: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00002b80: 202d 205b 785d 2048 544d 4c20 6974 656d   - [x] HTML item
+00002b90: 206c 6973 740a 2020 2020 2020 2020 2d20   list.        - 
+00002ba0: 5b78 5d20 4a53 4f4e 2069 7465 6d20 6c69  [x] JSON item li
+00002bb0: 7374 0a20 2020 2020 2020 202d 205b 785d  st.        - [x]
+00002bc0: 2058 4d4c 2069 7465 6d20 6c69 7374 0a20   XML item list. 
+00002bd0: 2020 2020 2020 202d 205b 785d 2053 656e         - [x] Sen
+00002be0: 6420 496d 6167 650a 2020 2020 2020 2020  d Image.        
+00002bf0: 2d20 5b78 5d20 5365 6e64 2056 6964 656f  - [x] Send Video
+00002c00: 0a20 2020 2020 2020 202d 205b 785d 2053  .        - [x] S
+00002c10: 656e 6420 6d65 6469 6120 6772 6f75 700a  end media group.
+00002c20: 2020 2020 2020 2020 2d20 5b20 5d20 5365          - [ ] Se
+00002c30: 6e64 2066 696c 650a 2020 2020 2020 2020  nd file.        
+00002c40: 2d20 5b20 5d20 5365 6e64 2061 7564 696f  - [ ] Send audio
+00002c50: 0a20 2020 2020 2020 202d 205b 785d 2046  .        - [x] F
+00002c60: 696c 6520 7365 6e64 696e 6720 7265 7472  ile sending retr
+00002c70: 790a 2020 2020 2020 2020 2d20 5b20 5d20  y.        - [ ] 
+00002c80: 4343 2061 7320 652d 6d61 696c 0a20 2020  CC as e-mail.   
+00002c90: 2020 2020 202d 205b 205d 2057 6562 686f       - [ ] Webho
+00002ca0: 6f6b 0a20 2020 2020 2020 202d 205b 205d  ok.        - [ ]
+00002cb0: 2055 7064 6174 6520 6d65 7373 6167 6520   Update message 
+00002cc0: 6279 206d 6573 7361 6765 2049 440a 2020  by message ID.  
+00002cd0: 2020 2020 2020 2d20 5b20 5d20 446f 6375        - [ ] Docu
+00002ce0: 6d65 6e74 0a20 2020 2020 2020 202d 205b  ment.        - [
+00002cf0: 205d 2047 5549 0a20 2020 2020 2020 200a   ] GUI.        .
+00002d00: 2020 2020 2020 2020 2323 2046 6565 6462          ## Feedb
+00002d10: 6163 6b0a 2020 2020 2020 2020 0a20 2020  ack.        .   
+00002d20: 2020 2020 2046 6565 6c20 6672 6565 2074       Feel free t
+00002d30: 6f20 636f 6e74 6163 7420 7769 7468 206d  o contact with m
+00002d40: 6520 6966 2079 6f75 2068 6176 6520 616e  e if you have an
+00002d50: 7920 7175 6573 7469 6f6e 2e20 416c 736f  y question. Also
+00002d60: 2077 656c 636f 6d65 2061 6e79 2063 6f6e   welcome any con
+00002d70: 7472 6962 7574 652e 0a20 2020 2020 2020  tribute..       
+00002d80: 200a 2020 2020 2020 2020 4966 2079 6f75   .        If you
+00002d90: 2062 7569 6c64 2061 2063 6861 6e6e 656c   build a channel
+00002da0: 2062 7920 7468 6973 2c20 646f 6e27 7420   by this, don't 
+00002db0: 666f 7267 6574 2074 6f20 7368 6172 6520  forget to share 
+00002dc0: 7468 6174 2067 6f6f 6420 6e65 7773 2077  that good news w
+00002dd0: 6974 6820 7573 210a 2020 2020 2020 2020  ith us!.        
+00002de0: 0a20 2020 2020 2020 2023 2320 4c69 6365  .        ## Lice
+00002df0: 6e73 650a 2020 2020 2020 2020 0a20 2020  nse.        .   
+00002e00: 2020 2020 204c 6963 656e 7365 6420 756e       Licensed un
+00002e10: 6465 7220 7468 6520 4d49 5420 4c69 6365  der the MIT Lice
+00002e20: 6e73 652e 0a20 2020 2020 2020 200a 506c  nse..        .Pl
+00002e30: 6174 666f 726d 3a20 554e 4b4e 4f57 4e0a  atform: UNKNOWN.
+00002e40: 436c 6173 7369 6669 6572 3a20 4465 7665  Classifier: Deve
+00002e50: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
+00002e60: 3a20 3320 2d20 416c 7068 610a 436c 6173  : 3 - Alpha.Clas
+00002e70: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
+00002e80: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00002e90: 3a3a 204d 4954 204c 6963 656e 7365 0a43  :: MIT License.C
+00002ea0: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
+00002eb0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00002ec0: 5320 496e 6465 7065 6e64 656e 740a 436c  S Independent.Cl
+00002ed0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00002ee0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00002ef0: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
+00002f00: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00002f10: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00002f20: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00002f30: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00002f40: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00002f50: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00002f60: 2033 2e31 310a 436c 6173 7369 6669 6572   3.11.Classifier
+00002f70: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00002f80: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00002f90: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
+00002fa0: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+00002fb0: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00002fc0: 6572 730a 436c 6173 7369 6669 6572 3a20  ers.Classifier: 
+00002fd0: 546f 7069 6320 3a3a 2045 6475 6361 7469  Topic :: Educati
+00002fe0: 6f6e 0a43 6c61 7373 6966 6965 723a 2054  on.Classifier: T
+00002ff0: 6f70 6963 203a 3a20 4f66 6669 6365 2f42  opic :: Office/B
+00003000: 7573 696e 6573 7320 3a3a 204e 6577 732f  usiness :: News/
+00003010: 4469 6172 790a 436c 6173 7369 6669 6572  Diary.Classifier
+00003020: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
+00003030: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
+00003040: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
+00003050: 5079 7468 6f6e 204d 6f64 756c 6573 0a52  Python Modules.R
+00003060: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+00003070: 3e3d 332e 380a 4465 7363 7269 7074 696f  >=3.8.Descriptio
+00003080: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00003090: 7465 7874 2f6d 6172 6b64 6f77 6e0a       text/markdown.
```

### Comparing `telegramweb-4.7/setup.py` & `telegramweb-4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='4.7',
+    version='4.8',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `telegramweb-4.7/telegram_news/__init__.py` & `telegramweb-4.8/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.7/telegram_news/constant.py` & `telegramweb-4.8/telegram_news/constant.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.7/telegram_news/displaypolicy.py` & `telegramweb-4.8/telegram_news/displaypolicy.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         po += item['time']
         po += '\n'
 
     if item['source']:
         po += '[' + item['source'] + ']' + ' '
 
     if item['link']:
-        po += '<a href=\"' + item['link'] + '\">LATEST UPDATE FROM OFFICIAL WEBSITE</a>'
+        po += '<a href=\"' + item['link'] + '\">LATEST UPDATE FROM ' + tag + ' SECTION</a>'
 
     po = po.replace('<br>', "")
 
     if len(po) > 4096:
         return "Too long message!\n" + item['id'], parse_mode, disable_web_page_preview
 
     return {
```

### Comparing `telegramweb-4.7/telegram_news/ratelimit.py` & `telegramweb-4.8/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.7/telegram_news/template/common.py` & `telegramweb-4.8/telegram_news/template/common.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.7/telegram_news/utils.py` & `telegramweb-4.8/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.7/telegramweb.egg-info/PKG-INFO` & `telegramweb-4.8/telegramweb.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,646 +1,778 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7465 6c65  : 2.1.Name: tele
 00000020: 6772 616d 7765 620a 5665 7273 696f 6e3a  gramweb.Version:
-00000030: 2034 2e37 0a53 756d 6d61 7279 3a20 5079   4.7.Summary: Py
+00000030: 2034 2e38 0a53 756d 6d61 7279 3a20 5079   4.8.Summary: Py
 00000040: 7468 6f6e 2070 6163 6b61 6765 2066 6f72  thon package for
 00000050: 2061 7574 6f6d 6174 6963 616c 6c79 2066   automatically f
 00000060: 6574 6368 696e 6720 616e 6420 7075 7368  etching and push
 00000070: 696e 6720 6e65 7773 2062 7920 5465 6c65  ing news by Tele
 00000080: 6772 616d 2e0a 486f 6d65 2d70 6167 653a  gram..Home-page:
 00000090: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 000000a0: 636f 6d2f 6372 617a 696b 732d 6372 6561  com/craziks-crea
 000000b0: 746f 722f 7465 6c65 6772 616d 2d77 6562  tor/telegram-web
 000000c0: 0a41 7574 686f 723a 2063 7261 7a69 6b73  .Author: craziks
 000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 2063  .Author-email: c
 000000e0: 6861 6e64 7261 7368 656b 6861 7270 616e  handrashekharpan
 000000f0: 6461 7930 3740 676d 6169 6c2e 636f 6d0a  day07@gmail.com.
-00000100: 4c69 6365 6e73 653a 204d 4954 0a50 6c61  License: MIT.Pla
-00000110: 7466 6f72 6d3a 2055 4e4b 4e4f 574e 0a43  tform: UNKNOWN.C
-00000120: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-00000130: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000140: 2033 202d 2041 6c70 6861 0a43 6c61 7373   3 - Alpha.Class
-00000150: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-00000160: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000170: 3a20 4d49 5420 4c69 6365 6e73 650a 436c  : MIT License.Cl
-00000180: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
-00000190: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-000001a0: 2049 6e64 6570 656e 6465 6e74 0a43 6c61   Independent.Cla
-000001b0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000001c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001d0: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
-000001e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000001f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000200: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000210: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
-00000220: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000230: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000240: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
-00000250: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000260: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000270: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
-00000280: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000290: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-000002a0: 7273 0a43 6c61 7373 6966 6965 723a 2054  rs.Classifier: T
-000002b0: 6f70 6963 203a 3a20 4564 7563 6174 696f  opic :: Educatio
-000002c0: 6e0a 436c 6173 7369 6669 6572 3a20 546f  n.Classifier: To
-000002d0: 7069 6320 3a3a 204f 6666 6963 652f 4275  pic :: Office/Bu
-000002e0: 7369 6e65 7373 203a 3a20 4e65 7773 2f44  siness :: News/D
-000002f0: 6961 7279 0a43 6c61 7373 6966 6965 723a  iary.Classifier:
-00000300: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
-00000310: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
-00000320: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
-00000330: 7974 686f 6e20 4d6f 6475 6c65 730a 5265  ython Modules.Re
-00000340: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
-00000350: 3d33 2e38 0a44 6573 6372 6970 7469 6f6e  =3.8.Description
-00000360: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-00000370: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
-00000380: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-00000390: 5345 0a0a 3c68 3120 616c 6967 6e3d 2263  SE..<h1 align="c
-000003a0: 656e 7465 7222 3e0a 2020 3c69 6d67 2073  enter">.  <img s
-000003b0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-000003c0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-000003d0: 742e 636f 6d2f 4553 575a 592f 7465 6c65  t.com/ESWZY/tele
-000003e0: 6772 616d 2d6e 6577 732f 6d61 7374 6572  gram-news/master
-000003f0: 2f64 6f63 732f 696d 6167 6573 2f62 616e  /docs/images/ban
-00000400: 6e65 722e 706e 6722 2061 6c74 3d22 5465  ner.png" alt="Te
-00000410: 6c65 6772 616d 2d6e 6577 7322 3e0a 2020  legram-news">.  
-00000420: 3c62 723e 5465 6c65 6772 616d 2d6e 6577  <br>Telegram-new
-00000430: 733c 6272 3e0a 3c2f 6831 3e0a 0a3c 6469  s<br>.</h1>..<di
-00000440: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-00000450: 3e0a 0a50 7974 686f 6e20 7061 636b 6167  >..Python packag
-00000460: 6520 666f 7220 6175 746f 6d61 7469 6361  e for automatica
-00000470: 6c6c 7920 6665 7463 6869 6e67 2061 6e64  lly fetching and
-00000480: 2070 7573 6869 6e67 206e 6577 7320 6279   pushing news by
-00000490: 2054 656c 6567 7261 6d2e 0a0a 5b21 5b50   Telegram...[![P
-000004a0: 7950 495d 2868 7474 7073 3a2f 2f69 6d67  yPI](https://img
-000004b0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000004c0: 2f76 2f74 656c 6567 7261 6d2d 6e65 7773  /v/telegram-news
-000004d0: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
-000004e0: 6f72 672f 7072 6f6a 6563 742f 7465 6c65  org/project/tele
-000004f0: 6772 616d 2d6e 6577 732f 290a 215b 5079  gram-news/).![Py
-00000500: 5049 202d 2050 7974 686f 6e20 5665 7273  PI - Python Vers
-00000510: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
-00000520: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000530: 2f70 7976 6572 7369 6f6e 732f 7465 6c65  /pyversions/tele
-00000540: 6772 616d 2d6e 6577 733f 6c6f 676f 3d70  gram-news?logo=p
-00000550: 7974 686f 6e29 0a5b 215b 4c69 6365 6e73  ython).[![Licens
-00000560: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
-00000570: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000580: 2f6c 6963 656e 7365 2f45 5357 5a59 2f74  /license/ESWZY/t
-00000590: 656c 6567 7261 6d2d 6e65 7773 295d 2868  elegram-news)](h
-000005a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000005b0: 6d2f 4553 575a 592f 7465 6c65 6772 616d  m/ESWZY/telegram
-000005c0: 2d6e 6577 732f 626c 6f62 2f6d 6173 7465  -news/blob/maste
-000005d0: 722f 4c49 4345 4e53 4529 0a21 5b50 7950  r/LICENSE).![PyP
-000005e0: 4920 2d20 446f 776e 6c6f 6164 735d 2868  I - Downloads](h
-000005f0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000600: 6473 2e69 6f2f 7079 7069 2f64 6d2f 7465  ds.io/pypi/dm/te
-00000610: 6c65 6772 616d 2d6e 6577 7329 0a0a 5b21  legram-news)..[!
-00000620: 5b42 7569 6c64 2053 7461 7475 735d 2868  [Build Status](h
-00000630: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000640: 6473 2e69 6f2f 7472 6176 6973 2f45 5357  ds.io/travis/ESW
-00000650: 5a59 2f74 656c 6567 7261 6d2d 6e65 7773  ZY/telegram-news
-00000660: 2f6d 6173 7465 723f 6c6f 676f 3d74 7261  /master?logo=tra
-00000670: 7669 7329 5d28 6874 7470 733a 2f2f 7472  vis)](https://tr
-00000680: 6176 6973 2d63 692e 6f72 672f 4553 575a  avis-ci.org/ESWZ
-00000690: 592f 7465 6c65 6772 616d 2d6e 6577 7329  Y/telegram-news)
-000006a0: 0a5b 215b 436f 6461 6379 2042 6164 6765  .[![Codacy Badge
-000006b0: 5d28 6874 7470 733a 2f2f 6170 692e 636f  ](https://api.co
-000006c0: 6461 6379 2e63 6f6d 2f70 726f 6a65 6374  dacy.com/project
-000006d0: 2f62 6164 6765 2f47 7261 6465 2f33 6330  /badge/Grade/3c0
-000006e0: 3766 6564 3532 3564 6134 3265 3839 6464  7fed525da42e89dd
-000006f0: 3364 3033 3736 3435 3762 3464 3229 5d28  3d0376457b4d2)](
-00000700: 6874 7470 733a 2f2f 6170 702e 636f 6461  https://app.coda
-00000710: 6379 2e63 6f6d 2f6d 616e 7561 6c2f 4553  cy.com/manual/ES
-00000720: 575a 592f 7465 6c65 6772 616d 2d6e 6577  WZY/telegram-new
-00000730: 733f 7574 6d5f 736f 7572 6365 3d67 6974  s?utm_source=git
-00000740: 6875 622e 636f 6d26 7574 6d5f 6d65 6469  hub.com&utm_medi
-00000750: 756d 3d72 6566 6572 7261 6c26 7574 6d5f  um=referral&utm_
-00000760: 636f 6e74 656e 743d 4553 575a 592f 7465  content=ESWZY/te
-00000770: 6c65 6772 616d 2d6e 6577 7326 7574 6d5f  legram-news&utm_
-00000780: 6361 6d70 6169 676e 3d42 6164 6765 5f47  campaign=Badge_G
-00000790: 7261 6465 5f44 6173 6862 6f61 7264 290a  rade_Dashboard).
-000007a0: 215b 4c61 7374 2063 6f6d 6d69 745d 2868  ![Last commit](h
-000007b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000007c0: 6473 2e69 6f2f 6769 7468 7562 2f6c 6173  ds.io/github/las
-000007d0: 742d 636f 6d6d 6974 2f45 5357 5a59 2f74  t-commit/ESWZY/t
-000007e0: 656c 6567 7261 6d2d 6e65 7773 290a 5b21  elegram-news).[!
-000007f0: 5b68 7474 7073 3a2f 2f74 2e6d 652f 6573  [https://t.me/es
-00000800: 777a 795d 2868 7474 7073 3a2f 2f69 6d67  wzy](https://img
-00000810: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000820: 652f 5465 6c65 6772 616d 2d45 5357 5a59  e/Telegram-ESWZY
-00000830: 2d62 6c75 652e 7376 673f 6c6f 676f 3d74  -blue.svg?logo=t
-00000840: 656c 6567 7261 6d29 5d28 6874 7470 733a  elegram)](https:
-00000850: 2f2f 742e 6d65 2f65 7377 7a79 290a 0a3c  //t.me/eswzy)..<
-00000860: 2f64 6976 3e0a 0a23 2320 496e 7472 6f64  /div>..## Introd
-00000870: 7563 7469 6f6e 0a0a 5468 6973 2069 7320  uction..This is 
-00000880: 6120 6561 7379 2d74 6f2d 6c65 6172 6e2c  a easy-to-learn,
-00000890: 2066 6c65 7869 626c 6520 616e 6420 7374   flexible and st
-000008a0: 616e 6461 7264 697a 6564 206d 6573 7361  andardized messa
-000008b0: 6765 2066 6574 6368 696e 6720 616e 6420  ge fetching and 
-000008c0: 7075 7368 696e 6720 6672 616d 6577 6f72  pushing framewor
-000008d0: 6b2c 2065 7370 6563 6961 6c6c 7920 666f  k, especially fo
-000008e0: 7220 5b54 656c 6567 7261 6d5d 2868 7474  r [Telegram](htt
-000008f0: 703a 2f2f 7777 772e 7465 6c65 6772 616d  p://www.telegram
-00000900: 2e6f 7267 2920 616e 6420 5b54 656c 6567  .org) and [Teleg
-00000910: 7261 6d20 426f 745d 2868 7474 7073 3a2f  ram Bot](https:/
-00000920: 2f63 6f72 652e 7465 6c65 6772 616d 2e6f  /core.telegram.o
-00000930: 7267 2f62 6f74 7329 2e0a 0a54 6865 2074  rg/bots)...The t
-00000940: 6172 6765 7420 6e65 7773 2073 6f75 7263  arget news sourc
-00000950: 6520 6361 6e20 6265 2048 544d 4c20 7061  e can be HTML pa
-00000960: 6765 2c20 4a53 4f4e 2061 6e64 2058 4d4c  ge, JSON and XML
-00000970: 2e20 5765 2061 6c73 6f20 7072 6f76 6964  . We also provid
-00000980: 6520 6375 7374 6f6d 697a 6564 2070 726f  e customized pro
-00000990: 6365 7373 2066 6f72 2075 6e6b 6e6f 776e  cess for unknown
-000009a0: 2064 6174 6120 666f 726d 6174 2e0a 0a50   data format...P
-000009b0: 7573 6820 7468 6520 6c61 7465 7374 206e  ush the latest n
-000009c0: 6577 7320 746f 2079 6f75 7220 6368 616e  ews to your chan
-000009d0: 6e65 6c20 6f72 2067 726f 7570 206f 6e63  nel or group onc
-000009e0: 6520 6974 2068 6170 7065 6e73 210a 0a23  e it happens!..#
-000009f0: 2320 496e 7374 616c 6c0a 0a60 6060 7368  # Install..```sh
-00000a00: 656c 6c0a 2420 7069 7020 696e 7374 616c  ell.$ pip instal
-00000a10: 6c20 7465 6c65 6772 616d 2d6e 6577 730a  l telegram-news.
-00000a20: 6060 600a 0a4f 722c 2079 6f75 2063 616e  ```..Or, you can
-00000a30: 2069 6e73 7461 6c6c 2062 7920 636c 6f6e   install by clon
-00000a40: 696e 6720 7468 6973 2072 6570 6f73 6974  ing this reposit
-00000a50: 6f72 793a 0a0a 6060 6073 6865 6c6c 0a24  ory:..```shell.$
-00000a60: 2067 6974 2063 6c6f 6e65 2068 7474 7073   git clone https
-00000a70: 3a2f 2f67 6974 6875 622e 636f 6d2f 4553  ://github.com/ES
-00000a80: 575a 592f 7465 6c65 6772 616d 2d6e 6577  WZY/telegram-new
-00000a90: 732e 6769 740a 2420 6364 2074 656c 6567  s.git.$ cd teleg
-00000aa0: 7261 6d2d 6e65 7773 0a24 2070 7974 686f  ram-news.$ pytho
-00000ab0: 6e20 7365 7475 702e 7079 2069 6e73 7461  n setup.py insta
-00000ac0: 6c6c 0a60 6060 0a0a 2323 2050 7265 7061  ll.```..## Prepa
-00000ad0: 7265 0a0a 4974 2064 6f65 7320 6e6f 7420  re..It does not 
-00000ae0: 6e65 6564 206d 7563 6820 736f 2074 6861  need much so tha
-00000af0: 7420 796f 7520 6361 6e20 7275 6e20 796f  t you can run yo
-00000b00: 7572 2063 6f64 6520 616e 7977 6865 7265  ur code anywhere
-00000b10: 2e0a 0a46 6972 7374 2c20 6173 6b20 5b40  ...First, ask [@
-00000b20: 426f 7446 6174 6865 725d 2868 7474 7073  BotFather](https
-00000b30: 3a2f 2f74 2e6d 652f 626f 7466 6174 6865  ://t.me/botfathe
-00000b40: 7229 2066 6f72 2061 2062 6f74 2061 6e64  r) for a bot and
-00000b50: 2062 6f74 2074 6f6b 656e 2e20 4166 7465   bot token. Afte
-00000b60: 7220 7468 6174 2c20 6372 6561 7465 2061  r that, create a
-00000b70: 2070 7562 6c69 6320 5b63 6861 6e6e 656c   public [channel
-00000b80: 5d28 6874 7470 733a 2f2f 7465 6c65 6772  ](https://telegr
-00000b90: 616d 2e6f 7267 2f74 6f75 722f 6368 616e  am.org/tour/chan
-00000ba0: 6e65 6c73 2920 6f72 205b 6772 6f75 705d  nels) or [group]
-00000bb0: 2868 7474 7073 3a2f 2f74 656c 6567 7261  (https://telegra
-00000bc0: 6d2e 6f72 672f 746f 7572 2f67 726f 7570  m.org/tour/group
-00000bd0: 7329 2c20 616e 6420 7265 6d65 6d62 6572  s), and remember
-00000be0: 2063 6861 7420 6964 2079 6f75 206a 7573   chat id you jus
-00000bf0: 7420 6e61 6d65 642e 2044 6f20 6e6f 7420  t named. Do not 
-00000c00: 666f 7267 6574 2074 6f20 696e 7669 7465  forget to invite
-00000c10: 2079 6f75 7220 626f 7420 696e 746f 2079   your bot into y
-00000c20: 6f75 7220 6368 616e 6e65 6c20 6f72 2067  our channel or g
-00000c30: 726f 7570 2061 6e64 206d 616b 6520 6974  roup and make it
-00000c40: 2061 6e20 6164 6d69 6e2e 0a0a 596f 7520   an admin...You 
-00000c50: 616c 736f 206e 6565 6420 6120 5351 4c20  also need a SQL 
-00000c60: 6461 7461 6261 7365 2e20 416e 7920 5351  database. Any SQ
-00000c70: 4c20 6461 7461 6261 7365 2069 7320 4f4b  L database is OK
-00000c80: 2e20 4573 7065 6369 616c 6c79 2c20 4920  . Especially, I 
-00000c90: 7265 636f 6d6d 656e 6420 5b50 6f73 7467  recommend [Postg
-00000ca0: 7265 5351 4c5d 2868 7474 7073 3a2f 2f77  reSQL](https://w
-00000cb0: 7777 2e70 6f73 7467 7265 7371 6c2e 6f72  ww.postgresql.or
-00000cc0: 672f 292e 0a0a 2323 2051 7569 636b 2064  g/)...## Quick d
-00000cd0: 6570 6c6f 7920 6f6e 2048 6572 6f6b 750a  eploy on Heroku.
-00000ce0: 0a43 6c69 636b 20f0 9f91 8720 6275 7474  .Click .... butt
-00000cf0: 6f6e 2074 6f20 6465 706c 6f79 2061 6e20  on to deploy an 
-00000d00: 6578 616d 706c 6520 666f 7220 6672 6565  example for free
-00000d10: 2e20 5079 7468 6f6e 2065 6e76 6972 6f6e  . Python environ
-00000d20: 6d65 6e74 2061 6e64 2050 6f73 7467 7265  ment and Postgre
-00000d30: 5351 4c20 6461 7461 6261 7365 2068 6176  SQL database hav
-00000d40: 6520 6265 656e 2070 7265 7061 7265 642e  e been prepared.
-00000d50: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00000d60: 3a2f 2f68 6572 6f6b 752e 636f 6d2f 6465  ://heroku.com/de
-00000d70: 706c 6f79 3f74 656d 706c 6174 653d 6874  ploy?template=ht
-00000d80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000d90: 2f45 5357 5a59 2f74 656c 6567 7261 6d2d  /ESWZY/telegram-
-00000da0: 6e65 7773 2d67 6574 7469 6e67 2d73 7461  news-getting-sta
-00000db0: 7274 6564 223e 0a20 203c 696d 6720 7372  rted">.  <img sr
-00000dc0: 633d 2268 7474 7073 3a2f 2f77 7777 2e68  c="https://www.h
-00000dd0: 6572 6f6b 7563 646e 2e63 6f6d 2f64 6570  erokucdn.com/dep
-00000de0: 6c6f 792f 6275 7474 6f6e 2e73 7667 2220  loy/button.svg" 
-00000df0: 616c 743d 2244 6570 6c6f 7922 3e0a 3c2f  alt="Deploy">.</
-00000e00: 613e 0a0a 4166 7465 7220 6465 706c 6f79  a>..After deploy
-00000e10: 6d65 6e74 2c20 7374 6172 7420 7468 6520  ment, start the 
-00000e20: 776f 726b 6572 2069 6e20 2252 6573 6f75  worker in "Resou
-00000e30: 7263 6573 2220 7461 622c 2061 6e64 2074  rces" tab, and t
-00000e40: 6865 6e20 796f 7520 6361 6e20 7365 6520  hen you can see 
-00000e50: 7468 6520 6566 6665 6374 2069 6e20 796f  the effect in yo
-00000e60: 7572 2063 6861 6e6e 656c 2f67 726f 7570  ur channel/group
-00000e70: 2c20 7768 6963 6820 636f 6e74 6169 6e73  , which contains
-00000e80: 2062 6f74 6820 5343 4d50 206e 6577 7320   both SCMP news 
-00000e90: 616e 6420 5769 6b69 206e 6577 7320 6174  and Wiki news at
-00000ea0: 2073 616d 6520 7469 6d65 2e0a 0a23 2320   same time...## 
-00000eb0: 5573 6167 650a 0a54 686f 7365 2061 7265  Usage..Those are
-00000ec0: 2033 2065 7861 6d70 6c65 7320 666f 7220   3 examples for 
-00000ed0: 796f 7520 746f 2075 6e64 6572 7374 616e  you to understan
-00000ee0: 6420 686f 7720 746f 2075 7365 2074 6865  d how to use the
-00000ef0: 2066 7261 6d65 776f 726b 2e0a 0a23 2323   framework...###
-00000f00: 2042 6173 6963 2045 7861 6d70 6c65 0a0a   Basic Example..
-00000f10: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00000f20: 206f 730a 6672 6f6d 2073 716c 616c 6368   os.from sqlalch
-00000f30: 656d 7920 696d 706f 7274 2063 7265 6174  emy import creat
-00000f40: 655f 656e 6769 6e65 0a66 726f 6d20 7371  e_engine.from sq
-00000f50: 6c61 6c63 6865 6d79 2e6f 726d 2069 6d70  lalchemy.orm imp
-00000f60: 6f72 7420 5365 7373 696f 6e0a 0a66 726f  ort Session..fro
-00000f70: 6d20 7465 6c65 6772 616d 5f6e 6577 732e  m telegram_news.
-00000f80: 7465 6d70 6c61 7465 2069 6d70 6f72 7420  template import 
-00000f90: 496e 666f 4578 7472 6163 746f 722c 204e  InfoExtractor, N
-00000fa0: 6577 7350 6f73 746d 616e 0a0a 2320 5468  ewsPostman..# Th
-00000fb0: 7265 6520 7265 7175 6972 6564 2066 6965  ree required fie
-00000fc0: 6c64 733a 0a23 2059 6f75 7220 626f 7420  lds:.# Your bot 
-00000fd0: 746f 6b65 6e20 6f62 7461 696e 6564 2066  token obtained f
-00000fe0: 726f 6d20 4042 6f74 4661 7468 6572 0a62  rom @BotFather.b
-00000ff0: 6f74 5f74 6f6b 656e 203d 206f 732e 6765  ot_token = os.ge
-00001000: 7465 6e76 2822 544f 4b45 4e22 290a 2320  tenv("TOKEN").# 
-00001010: 4164 6420 796f 7572 2062 6f74 7320 696e  Add your bots in
-00001020: 746f 2061 2063 6861 6e6e 656c 2061 7320  to a channel as 
-00001030: 616e 2061 646d 696e 6973 7472 6174 6f72  an administrator
-00001040: 0a63 6861 6e6e 656c 203d 206f 732e 6765  .channel = os.ge
-00001050: 7465 6e76 2822 4348 414e 4e45 4c22 290a  tenv("CHANNEL").
-00001060: 2320 596f 7572 2064 6174 6162 6173 6520  # Your database 
-00001070: 746f 2073 746f 7265 206f 6c64 206d 6573  to store old mes
-00001080: 7361 6765 732e 0a44 4154 4142 4153 455f  sages..DATABASE_
-00001090: 5552 4c20 3d20 6f73 2e67 6574 656e 7628  URL = os.getenv(
-000010a0: 2244 4154 4142 4153 455f 5552 4c22 290a  "DATABASE_URL").
-000010b0: 0a23 2043 7265 6174 6520 6120 6461 7461  .# Create a data
-000010c0: 6261 7365 2073 6573 7369 6f6e 0a65 6e67  base session.eng
-000010d0: 696e 6520 3d20 6372 6561 7465 5f65 6e67  ine = create_eng
-000010e0: 696e 6528 4441 5441 4241 5345 5f55 524c  ine(DATABASE_URL
-000010f0: 290a 6462 203d 2053 6573 7369 6f6e 2862  ).db = Session(b
-00001100: 696e 643d 656e 6769 6e65 2e63 6f6e 6e65  ind=engine.conne
-00001110: 6374 2829 290a 0a23 2054 6865 206e 6577  ct())..# The new
-00001120: 7320 736f 7572 6365 0a75 726c 203d 2022  s source.url = "
-00001130: 6874 7470 733a 2f2f 656e 2e77 696b 696e  https://en.wikin
-00001140: 6577 732e 6f72 672f 7769 6b69 2f4d 6169  ews.org/wiki/Mai
-00001150: 6e5f 5061 6765 220a 7461 6720 3d20 2257  n_Page".tag = "W
-00001160: 696b 6920 4e65 7773 220a 7461 626c 655f  iki News".table_
-00001170: 6e61 6d65 203d 2022 7769 6b69 6e65 7773  name = "wikinews
-00001180: 220a 0a23 2049 6e66 6f20 6578 7472 6163  "..# Info extrac
-00001190: 746f 7220 746f 2070 726f 6365 7373 2064  tor to process d
-000011a0: 6174 6120 666f 726d 6174 0a69 6520 3d20  ata format.ie = 
-000011b0: 496e 666f 4578 7472 6163 746f 7228 290a  InfoExtractor().
-000011c0: 0a23 2053 656c 6563 7420 7365 6c65 6374  .# Select select
-000011d0: 2065 6c65 6d65 6e74 2062 7920 4353 532d   element by CSS-
-000011e0: 6261 7365 6420 7365 6c65 6374 6f72 0a69  based selector.i
-000011f0: 652e 7365 745f 6c69 7374 5f73 656c 6563  e.set_list_selec
-00001200: 746f 7228 2723 4d61 696e 5061 6765 5f6c  tor('#MainPage_l
-00001210: 6174 6573 745f 6e65 7773 5f74 6578 7420  atest_news_text 
-00001220: 3e20 756c 203e 206c 6927 290a 6965 2e73  > ul > li').ie.s
-00001230: 6574 5f74 6974 6c65 5f73 656c 6563 746f  et_title_selecto
-00001240: 7228 2723 6669 7273 7448 6561 6469 6e67  r('#firstHeading
-00001250: 2729 0a69 652e 7365 745f 7061 7261 6772  ').ie.set_paragr
-00001260: 6170 685f 7365 6c65 6374 6f72 2827 236d  aph_selector('#m
-00001270: 772d 636f 6e74 656e 742d 7465 7874 203e  w-content-text >
-00001280: 2064 6976 203e 2070 3a6e 6f74 2870 3a6e   div > p:not(p:n
-00001290: 7468 2d63 6869 6c64 2831 2929 2729 0a69  th-child(1))').i
-000012a0: 652e 7365 745f 7469 6d65 5f73 656c 6563  e.set_time_selec
-000012b0: 746f 7228 2723 6d77 2d63 6f6e 7465 6e74  tor('#mw-content
-000012c0: 2d74 6578 7420 3e20 6469 7620 3e20 703a  -text > div > p:
-000012d0: 6e74 682d 6368 696c 6428 3129 203e 2073  nth-child(1) > s
-000012e0: 7472 6f6e 6727 290a 6965 2e73 6574 5f73  trong').ie.set_s
-000012f0: 6f75 7263 655f 7365 6c65 6374 6f72 2827  ource_selector('
-00001300: 7370 616e 2e73 6f75 7263 6554 656d 706c  span.sourceTempl
-00001310: 6174 6527 290a 0a23 2053 6574 2061 206d  ate')..# Set a m
-00001320: 6178 206c 656e 6774 6820 666f 7220 706f  ax length for po
-00001330: 7374 2c20 4d61 7820 6973 2034 3039 360a  st, Max is 4096.
-00001340: 6965 2e6d 6178 5f70 6f73 745f 6c65 6e67  ie.max_post_leng
-00001350: 7468 203d 2032 3030 300a 0a23 204e 6577  th = 2000..# New
-00001360: 7320 706f 7374 6d61 6e20 746f 206d 616e  s postman to man
-00001370: 6167 6520 7365 6e64 696e 6720 6166 6661  age sending affa
-00001380: 6972 0a6e 7020 3d20 4e65 7773 506f 7374  ir.np = NewsPost
-00001390: 6d61 6e28 6c69 7374 5552 4c73 3d5b 7572  man(listURLs=[ur
-000013a0: 6c2c 205d 2c20 7365 6e64 4c69 7374 3d5b  l, ], sendList=[
-000013b0: 6368 616e 6e65 6c2c 205d 2c20 6462 3d64  channel, ], db=d
-000013c0: 622c 2074 6167 3d74 6167 290a 6e70 2e73  b, tag=tag).np.s
-000013d0: 6574 5f62 6f74 5f74 6f6b 656e 2862 6f74  et_bot_token(bot
-000013e0: 5f74 6f6b 656e 290a 6e70 2e73 6574 5f65  _token).np.set_e
-000013f0: 7874 7261 6374 6f72 2869 6529 0a6e 702e  xtractor(ie).np.
-00001400: 7365 745f 7461 626c 655f 6e61 6d65 2874  set_table_name(t
-00001410: 6162 6c65 5f6e 616d 6529 0a0a 2320 5374  able_name)..# St
-00001420: 6172 7420 746f 2077 6f72 6b21 0a6e 702e  art to work!.np.
-00001430: 706f 6c6c 2829 0a60 6060 0a0a 5479 7069  poll().```..Typi
-00001440: 6361 6c20 7265 7375 6c74 733a 0a0a 3c64  cal results:..<d
-00001450: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
-00001460: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
-00001470: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00001480: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00001490: 2f45 5357 5a59 2f74 656c 6567 7261 6d2d  /ESWZY/telegram-
-000014a0: 6e65 7773 2f6d 6173 7465 722f 646f 6373  news/master/docs
-000014b0: 2f69 6d61 6765 732f 6465 6d6f 312e 706e  /images/demo1.pn
-000014c0: 6722 2061 6c74 3d22 4465 6d6f 2031 2220  g" alt="Demo 1" 
-000014d0: 7769 6474 683d 2234 3025 223e 0a20 203c  width="40%">.  <
-000014e0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000014f0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00001500: 6f6e 7465 6e74 2e63 6f6d 2f45 5357 5a59  ontent.com/ESWZY
-00001510: 2f74 656c 6567 7261 6d2d 6e65 7773 2f6d  /telegram-news/m
-00001520: 6173 7465 722f 646f 6373 2f69 6d61 6765  aster/docs/image
-00001530: 732f 6465 6d6f 322e 706e 6722 2061 6c74  s/demo2.png" alt
-00001540: 3d22 4465 6d6f 2032 2220 7769 6474 683d  ="Demo 2" width=
-00001550: 2234 3025 223e 0a3c 2f64 6976 3e0a 0a23  "40%">.</div>..#
-00001560: 2323 2041 6476 616e 6365 6420 4578 616d  ## Advanced Exam
-00001570: 706c 650a 0a60 6060 7079 7468 6f6e 0a69  ple..```python.i
-00001580: 6d70 6f72 7420 6f73 0a66 726f 6d20 7371  mport os.from sq
-00001590: 6c61 6c63 6865 6d79 2069 6d70 6f72 7420  lalchemy import 
-000015a0: 6372 6561 7465 5f65 6e67 696e 650a 6672  create_engine.fr
-000015b0: 6f6d 2073 716c 616c 6368 656d 792e 6f72  om sqlalchemy.or
-000015c0: 6d20 696d 706f 7274 2053 6573 7369 6f6e  m import Session
-000015d0: 0a66 726f 6d20 7465 6c65 6772 616d 5f6e  .from telegram_n
-000015e0: 6577 732e 7465 6d70 6c61 7465 2069 6d70  ews.template imp
-000015f0: 6f72 7420 496e 666f 4578 7472 6163 746f  ort InfoExtracto
-00001600: 722c 204e 6577 7350 6f73 746d 616e 0a62  r, NewsPostman.b
-00001610: 6f74 5f74 6f6b 656e 203d 206f 732e 6765  ot_token = os.ge
-00001620: 7465 6e76 2822 544f 4b45 4e22 290a 6368  tenv("TOKEN").ch
-00001630: 616e 6e65 6c20 3d20 6f73 2e67 6574 656e  annel = os.geten
-00001640: 7628 2243 4841 4e4e 454c 2229 0a44 4154  v("CHANNEL").DAT
-00001650: 4142 4153 455f 5552 4c20 3d20 6f73 2e67  ABASE_URL = os.g
-00001660: 6574 656e 7628 2244 4154 4142 4153 455f  etenv("DATABASE_
-00001670: 5552 4c22 290a 656e 6769 6e65 203d 2063  URL").engine = c
-00001680: 7265 6174 655f 656e 6769 6e65 2844 4154  reate_engine(DAT
-00001690: 4142 4153 455f 5552 4c29 0a64 6220 3d20  ABASE_URL).db = 
-000016a0: 5365 7373 696f 6e28 6269 6e64 3d65 6e67  Session(bind=eng
-000016b0: 696e 652e 636f 6e6e 6563 7428 2929 0a0a  ine.connect())..
-000016c0: 2320 4162 6f76 6520 636f 6465 2069 7320  # Above code is 
-000016d0: 6173 2073 616d 6520 6173 2074 6865 2062  as same as the b
-000016e0: 6173 6963 2065 7861 6d70 6c65 2c20 796f  asic example, yo
-000016f0: 7520 6361 6e20 7265 7573 6520 7468 6f73  u can reuse thos
-00001700: 6520 636f 6465 2064 6972 6563 746c 790a  e code directly.
-00001710: 0a75 726c 5f32 203d 2022 6874 7470 733a  .url_2 = "https:
-00001720: 2f2f 7777 772e 636e 6265 7461 2e63 6f6d  //www.cnbeta.com
-00001730: 2f22 0a74 6167 5f32 203d 2022 636e 4265  /".tag_2 = "cnBe
-00001740: 7461 220a 7461 626c 655f 6e61 6d65 5f32  ta".table_name_2
-00001750: 203d 2022 636e 6265 7461 6e65 7773 220a   = "cnbetanews".
-00001760: 0a69 655f 3220 3d20 496e 666f 4578 7472  .ie_2 = InfoExtr
-00001770: 6163 746f 7228 290a 6965 5f32 2e73 6574  actor().ie_2.set
-00001780: 5f6c 6973 745f 7365 6c65 6374 6f72 2827  _list_selector('
-00001790: 2e69 7465 6d73 2d61 7265 6120 3e20 6469  .items-area > di
-000017a0: 7620 3e20 646c 203e 2064 7420 3e20 6127  v > dl > dt > a'
-000017b0: 290a 6965 5f32 2e73 6574 5f74 6974 6c65  ).ie_2.set_title
-000017c0: 5f73 656c 6563 746f 7228 2768 6561 6465  _selector('heade
-000017d0: 7220 3e20 6831 2729 0a0a 2320 5365 6c65  r > h1')..# Sele
-000017e0: 6374 206d 616e 7920 7461 7267 6574 2061  ct many target a
-000017f0: 7420 7361 6d65 2074 696d 6520 2020 200a  t same time    .
-00001800: 6965 5f32 2e73 6574 5f70 6172 6167 7261  ie_2.set_paragra
-00001810: 7068 5f73 656c 6563 746f 7228 2764 6976  ph_selector('div
-00001820: 2e63 6e62 6574 612d 6172 7469 636c 652d  .cnbeta-article-
-00001830: 626f 6479 203e 2064 6976 2e61 7274 6963  body > div.artic
-00001840: 6c65 2d73 756d 6d61 7279 203e 2070 2c20  le-summary > p, 
-00001850: 2720 2023 2053 756d 6d61 7279 206f 6e6c  '  # Summary onl
-00001860: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-00001870: 2020 2020 2020 2020 2020 2020 2020 2764                'd
-00001880: 6976 2e63 6e62 6574 612d 6172 7469 636c  iv.cnbeta-articl
-00001890: 652d 626f 6479 203e 2064 6976 2e61 7274  e-body > div.art
-000018a0: 6963 6c65 2d63 6f6e 7465 6e74 203e 2070  icle-content > p
-000018b0: 2729 2020 2023 2043 6f6e 7465 6e74 206f  ')   # Content o
-000018c0: 6e6c 790a 6965 5f32 2e73 6574 5f74 696d  nly.ie_2.set_tim
-000018d0: 655f 7365 6c65 6374 6f72 2827 6865 6164  e_selector('head
-000018e0: 6572 203e 2064 6976 203e 2073 7061 6e3a  er > div > span:
-000018f0: 6e74 682d 6368 696c 6428 3129 2729 0a69  nth-child(1)').i
-00001900: 655f 322e 7365 745f 736f 7572 6365 5f73  e_2.set_source_s
-00001910: 656c 6563 746f 7228 2768 6561 6465 7220  elector('header 
-00001920: 3e20 6469 7620 3e20 7370 616e 2e73 6f75  > div > span.sou
-00001930: 7263 6527 290a 0a23 2053 656c 6563 7420  rce')..# Select 
-00001940: 696d 6167 6520 746f 2064 6973 706c 6179  image to display
-00001950: 2c20 7468 656e 2074 6865 206d 6178 206c  , then the max l
-00001960: 656e 6774 6820 6973 2064 6f77 6e20 746f  ength is down to
-00001970: 2031 3032 340a 6965 5f32 2e73 6574 5f69   1024.ie_2.set_i
-00001980: 6d61 6765 5f73 656c 6563 746f 7228 2764  mage_selector('d
-00001990: 6976 2e63 6e62 6574 612d 6172 7469 636c  iv.cnbeta-articl
-000019a0: 652d 626f 6479 203e 2064 6976 2e61 7274  e-body > div.art
-000019b0: 6963 6c65 2d73 756d 6d61 7279 203e 2070  icle-summary > p
-000019c0: 2069 6d67 2c20 2720 2023 2046 726f 6d20   img, '  # From 
-000019d0: 7375 6d6d 6172 7920 6f6e 6c79 0a20 2020  summary only.   
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 2020 2020 2027 6469 762e 636e 6265 7461       'div.cnbeta
-00001a00: 2d61 7274 6963 6c65 2d62 6f64 7920 3e20  -article-body > 
-00001a10: 6469 762e 6172 7469 636c 652d 636f 6e74  div.article-cont
-00001a20: 656e 7420 3e20 7020 696d 6727 2920 2020  ent > p img')   
-00001a30: 2320 4672 6f6d 2063 6f6e 7465 6e74 206f  # From content o
-00001a40: 6e6c 790a 6965 5f32 2e6d 6178 5f70 6f73  nly.ie_2.max_pos
-00001a50: 745f 6c65 6e67 7468 203d 2031 3030 300a  t_length = 1000.
-00001a60: 0a6e 705f 3220 3d20 4e65 7773 506f 7374  .np_2 = NewsPost
-00001a70: 6d61 6e28 6c69 7374 5552 4c73 3d5b 7572  man(listURLs=[ur
-00001a80: 6c5f 322c 205d 2c20 7365 6e64 4c69 7374  l_2, ], sendList
-00001a90: 3d5b 6368 616e 6e65 6c5d 2c20 7461 673d  =[channel], tag=
-00001aa0: 7461 675f 322c 2064 623d 6462 290a 6e70  tag_2, db=db).np
-00001ab0: 5f32 2e73 6574 5f65 7874 7261 6374 6f72  _2.set_extractor
-00001ac0: 2869 655f 3229 0a6e 705f 322e 7365 745f  (ie_2).np_2.set_
-00001ad0: 7461 626c 655f 6e61 6d65 2874 6162 6c65  table_name(table
-00001ae0: 5f6e 616d 655f 3229 0a6e 705f 322e 706f  _name_2).np_2.po
-00001af0: 6c6c 2829 0a60 6060 0a0a 5479 7069 6361  ll().```..Typica
-00001b00: 6c20 7265 7375 6c74 733a 0a0a 3c64 6976  l results:..<div
-00001b10: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00001b20: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
-00001b30: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00001b40: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f45  sercontent.com/E
-00001b50: 5357 5a59 2f74 656c 6567 7261 6d2d 6e65  SWZY/telegram-ne
-00001b60: 7773 2f6d 6173 7465 722f 646f 6373 2f69  ws/master/docs/i
-00001b70: 6d61 6765 732f 6465 6d6f 332e 706e 6722  mages/demo3.png"
-00001b80: 2061 6c74 3d22 4465 6d6f 2033 2220 7769   alt="Demo 3" wi
-00001b90: 6474 683d 2234 3025 223e 0a20 203c 696d  dth="40%">.  <im
-00001ba0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00001bb0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00001bc0: 7465 6e74 2e63 6f6d 2f45 5357 5a59 2f74  tent.com/ESWZY/t
-00001bd0: 656c 6567 7261 6d2d 6e65 7773 2f6d 6173  elegram-news/mas
-00001be0: 7465 722f 646f 6373 2f69 6d61 6765 732f  ter/docs/images/
-00001bf0: 6465 6d6f 342e 706e 6722 2061 6c74 3d22  demo4.png" alt="
-00001c00: 4465 6d6f 2034 2220 7769 6474 683d 2234  Demo 4" width="4
-00001c10: 3025 223e 0a3c 2f64 6976 3e0a 0a23 2323  0%">.</div>..###
-00001c20: 2041 6476 616e 6365 6420 4578 616d 706c   Advanced Exampl
-00001c30: 6520 666f 7220 4a53 4f4e 2061 6e64 2058  e for JSON and X
-00001c40: 4d4c 0a0a 5468 6520 6861 6e64 6c65 2066  ML..The handle f
-00001c50: 6f72 204a 534f 4e20 616e 6420 584d 4c20  or JSON and XML 
-00001c60: 6172 6520 7175 6974 6520 7369 6d69 6c61  are quite simila
-00001c70: 722e 2059 6f75 2063 616e 2063 6f6e 7665  r. You can conve
-00001c80: 7274 2058 4d4c 2074 6f20 4a53 4f4e 2062  rt XML to JSON b
-00001c90: 7920 6675 6e63 7469 6f6e 2060 7465 6c65  y function `tele
-00001ca0: 6772 616d 5f6e 6577 732e 7574 696c 732e  gram_news.utils.
-00001cb0: 786d 6c5f 746f 5f6a 736f 6e60 2c20 616e  xml_to_json`, an
-00001cc0: 6420 7573 6520 604e 6577 7350 6f73 746d  d use `NewsPostm
-00001cd0: 616e 4a53 4f4e 6020 616e 6420 6049 6e66  anJSON` and `Inf
-00001ce0: 6f45 7874 7261 6374 6f72 4a53 4f4e 602e  oExtractorJSON`.
-00001cf0: 204f 722c 2079 6f75 2063 616e 2075 7365   Or, you can use
-00001d00: 2060 4e65 7773 506f 7374 6d61 6e58 4d4c   `NewsPostmanXML
-00001d10: 6020 616e 6420 6049 6e66 6f45 7874 7261  ` and `InfoExtra
-00001d20: 6374 6f72 584d 4c60 2064 6972 6563 746c  ctorXML` directl
-00001d30: 792e 0a0a 596f 7520 7368 6f75 6c64 2075  y...You should u
-00001d40: 7365 206b 6579 206c 6973 7420 746f 2072  se key list to r
-00001d50: 6563 7572 7369 7665 6c79 2072 6f75 7465  ecursively route
-00001d60: 2074 6f20 7468 6520 696e 666f 726d 6174   to the informat
-00001d70: 696f 6e20 796f 7520 7761 6e74 2e0a 0a60  ion you want...`
-00001d80: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00001d90: 6861 7368 6c69 620a 696d 706f 7274 206a  hashlib.import j
-00001da0: 736f 6e0a 696d 706f 7274 206f 730a 6672  son.import os.fr
-00001db0: 6f6d 2073 716c 616c 6368 656d 7920 696d  om sqlalchemy im
-00001dc0: 706f 7274 2063 7265 6174 655f 656e 6769  port create_engi
-00001dd0: 6e65 0a66 726f 6d20 7371 6c61 6c63 6865  ne.from sqlalche
-00001de0: 6d79 2e6f 726d 2069 6d70 6f72 7420 5365  my.orm import Se
-00001df0: 7373 696f 6e0a 6672 6f6d 2074 656c 6567  ssion.from teleg
-00001e00: 7261 6d5f 6e65 7773 2e74 656d 706c 6174  ram_news.templat
-00001e10: 6520 696d 706f 7274 2049 6e66 6f45 7874  e import InfoExt
-00001e20: 7261 6374 6f72 4a53 4f4e 2c20 4e65 7773  ractorJSON, News
-00001e30: 506f 7374 6d61 6e4a 534f 4e0a 6672 6f6d  PostmanJSON.from
-00001e40: 2074 656c 6567 7261 6d5f 6e65 7773 2e75   telegram_news.u
-00001e50: 7469 6c73 2069 6d70 6f72 7420 786d 6c5f  tils import xml_
-00001e60: 746f 5f6a 736f 6e0a 626f 745f 746f 6b65  to_json.bot_toke
-00001e70: 6e20 3d20 6f73 2e67 6574 656e 7628 2254  n = os.getenv("T
-00001e80: 4f4b 454e 2229 0a63 6861 6e6e 656c 203d  OKEN").channel =
-00001e90: 206f 732e 6765 7465 6e76 2822 4348 414e   os.getenv("CHAN
-00001ea0: 4e45 4c22 290a 4441 5441 4241 5345 5f55  NEL").DATABASE_U
-00001eb0: 524c 203d 206f 732e 6765 7465 6e76 2822  RL = os.getenv("
-00001ec0: 4441 5441 4241 5345 5f55 524c 2229 0a65  DATABASE_URL").e
-00001ed0: 6e67 696e 6520 3d20 6372 6561 7465 5f65  ngine = create_e
-00001ee0: 6e67 696e 6528 4441 5441 4241 5345 5f55  ngine(DATABASE_U
-00001ef0: 524c 290a 6462 203d 2053 6573 7369 6f6e  RL).db = Session
-00001f00: 2862 696e 643d 656e 6769 6e65 2e63 6f6e  (bind=engine.con
-00001f10: 6e65 6374 2829 290a 0a75 726c 5f33 203d  nect())..url_3 =
-00001f20: 2022 6874 7470 733a 2f2f 7777 772e 7363   "https://www.sc
-00001f30: 6d70 2e63 6f6d 2f72 7373 2f39 312f 6665  mp.com/rss/91/fe
-00001f40: 6564 220a 7461 675f 3320 3d20 2253 434d  ed".tag_3 = "SCM
-00001f50: 5022 0a74 6162 6c65 5f6e 616d 655f 3320  P".table_name_3 
-00001f60: 3d20 2273 636d 706e 6577 7322 0a0a 6965  = "scmpnews"..ie
-00001f70: 5f33 203d 2049 6e66 6f45 7874 7261 6374  _3 = InfoExtract
-00001f80: 6f72 4a53 4f4e 2829 0a0a 2320 5072 652d  orJSON()..# Pre-
-00001f90: 7072 6f63 6573 7320 7468 6520 584d 4c20  process the XML 
-00001fa0: 7374 7269 6e67 2c20 636f 6e76 6572 7420  string, convert 
-00001fb0: 746f 204a 534f 4e20 7374 7269 6e67 0a64  to JSON string.d
-00001fc0: 6566 206c 6973 745f 7072 655f 7072 6f63  ef list_pre_proc
-00001fd0: 6573 7328 7465 7874 293a 0a20 2020 2074  ess(text):.    t
-00001fe0: 6578 7420 3d20 6a73 6f6e 2e6c 6f61 6473  ext = json.loads
-00001ff0: 2878 6d6c 5f74 6f5f 6a73 6f6e 2874 6578  (xml_to_json(tex
-00002000: 7429 290a 2020 2020 7265 7475 726e 206a  t)).    return j
-00002010: 736f 6e2e 6475 6d70 7328 7465 7874 290a  son.dumps(text).
-00002020: 6965 5f33 2e73 6574 5f6c 6973 745f 7072  ie_3.set_list_pr
-00002030: 655f 7072 6f63 6573 735f 706f 6c69 6379  e_process_policy
-00002040: 286c 6973 745f 7072 655f 7072 6f63 6573  (list_pre_proces
-00002050: 7329 0a0a 2320 526f 7574 6520 6279 206b  s)..# Route by k
-00002060: 6579 206c 6973 740a 6965 5f33 2e73 6574  ey list.ie_3.set
-00002070: 5f6c 6973 745f 726f 7574 6572 285b 2772  _list_router(['r
-00002080: 7373 272c 2027 6368 616e 6e65 6c27 2c20  ss', 'channel', 
-00002090: 2769 7465 6d27 5d29 0a69 655f 332e 7365  'item']).ie_3.se
-000020a0: 745f 6c69 6e6b 5f72 6f75 7465 7228 5b27  t_link_router(['
-000020b0: 6c69 6e6b 275d 290a 6965 5f33 2e73 6574  link']).ie_3.set
-000020c0: 5f74 6974 6c65 5f72 6f75 7465 7228 5b27  _title_router(['
-000020d0: 7469 746c 6527 5d29 0a69 655f 332e 7365  title']).ie_3.se
-000020e0: 745f 7061 7261 6772 6170 6873 5f72 6f75  t_paragraphs_rou
-000020f0: 7465 7228 5b27 6465 7363 7269 7074 696f  ter(['descriptio
-00002100: 6e27 5d29 0a69 655f 332e 7365 745f 7469  n']).ie_3.set_ti
-00002110: 6d65 5f72 6f75 7465 7228 5b27 7075 6244  me_router(['pubD
-00002120: 6174 6527 5d29 0a69 655f 332e 7365 745f  ate']).ie_3.set_
-00002130: 736f 7572 6365 5f72 6f75 7465 7228 5b27  source_router(['
-00002140: 6175 7468 6f72 275d 290a 6965 5f33 2e73  author']).ie_3.s
-00002150: 6574 5f69 6d61 6765 5f72 6f75 7465 7228  et_image_router(
-00002160: 5b27 6d65 6469 613a 7468 756d 626e 6169  ['media:thumbnai
-00002170: 6c27 2c20 2740 7572 6c27 5d29 0a0a 2320  l', '@url'])..# 
-00002180: 4375 7374 6f6d 697a 6520 4944 2066 6f72  Customize ID for
-00002190: 206e 6577 7320 6974 656d 0a64 6566 2069   news item.def i
-000021a0: 645f 706f 6c69 6379 286c 696e 6b29 3a0a  d_policy(link):.
-000021b0: 2020 2020 7265 7475 726e 2068 6173 686c      return hashl
-000021c0: 6962 2e6d 6435 286c 696e 6b2e 656e 636f  ib.md5(link.enco
-000021d0: 6465 2822 7574 662d 3822 2929 2e68 6578  de("utf-8")).hex
-000021e0: 6469 6765 7374 2829 0a69 655f 332e 7365  digest().ie_3.se
-000021f0: 745f 6964 5f70 6f6c 6963 7928 6964 5f70  t_id_policy(id_p
-00002200: 6f6c 6963 7929 0a0a 6e70 5f33 203d 204e  olicy)..np_3 = N
-00002210: 6577 7350 6f73 746d 616e 4a53 4f4e 286c  ewsPostmanJSON(l
-00002220: 6973 7455 524c 733d 5b75 726c 5f33 5d2c  istURLs=[url_3],
-00002230: 2073 656e 644c 6973 743d 5b63 6861 6e6e   sendList=[chann
-00002240: 656c 5d2c 2064 623d 6462 2c20 7461 673d  el], db=db, tag=
-00002250: 7461 675f 3329 0a6e 705f 332e 7365 745f  tag_3).np_3.set_
-00002260: 6578 7472 6163 746f 7228 6965 5f33 290a  extractor(ie_3).
-00002270: 6e70 5f33 2e73 6574 5f74 6162 6c65 5f6e  np_3.set_table_n
-00002280: 616d 6528 7461 626c 655f 6e61 6d65 5f33  ame(table_name_3
-00002290: 290a 6e70 5f33 2e70 6f6c 6c28 290a 6060  ).np_3.poll().``
-000022a0: 600a 0a54 7970 6963 616c 2072 6573 756c  `..Typical resul
-000022b0: 7473 3a0a 0a3c 6469 7620 616c 6967 6e3d  ts:..<div align=
-000022c0: 2263 656e 7465 7222 3e0a 2020 3c69 6d67  "center">.  <img
-000022d0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-000022e0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-000022f0: 656e 742e 636f 6d2f 4553 575a 592f 7465  ent.com/ESWZY/te
-00002300: 6c65 6772 616d 2d6e 6577 732f 6d61 7374  legram-news/mast
-00002310: 6572 2f64 6f63 732f 696d 6167 6573 2f64  er/docs/images/d
-00002320: 656d 6f35 2e70 6e67 2220 616c 743d 2244  emo5.png" alt="D
-00002330: 656d 6f20 3522 2077 6964 7468 3d22 3430  emo 5" width="40
-00002340: 2522 3e0a 2020 3c69 6d67 2073 7263 3d22  %">.  <img src="
-00002350: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00002360: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00002370: 6d2f 4553 575a 592f 7465 6c65 6772 616d  m/ESWZY/telegram
-00002380: 2d6e 6577 732f 6d61 7374 6572 2f64 6f63  -news/master/doc
-00002390: 732f 696d 6167 6573 2f64 656d 6f36 2e70  s/images/demo6.p
-000023a0: 6e67 2220 616c 743d 2244 656d 6f20 3622  ng" alt="Demo 6"
-000023b0: 2077 6964 7468 3d22 3430 2522 3e0a 3c2f   width="40%">.</
-000023c0: 6469 763e 0a0a 2323 2320 5061 7261 6c6c  div>..### Parall
-000023d0: 656c 2050 726f 6772 616d 0a0a 4966 2079  el Program..If y
-000023e0: 6f75 2075 7365 2074 6865 2073 616d 6520  ou use the same 
-000023f0: 6461 7461 6261 7365 2061 6e64 2073 656e  database and sen
-00002400: 6420 746f 2074 6865 2073 616d 6520 6368  d to the same ch
-00002410: 616e 6e65 6c2c 2079 6f75 2063 616e 2073  annel, you can s
-00002420: 696d 706c 7920 6a6f 696e 7420 6561 6368  imply joint each
-00002430: 2070 6172 7420 6f66 2063 6f64 6520 626c   part of code bl
-00002440: 6f63 6b2c 2061 6e64 2063 616c 6c20 6070  ock, and call `p
-00002450: 6f6c 6c28 2960 2066 756e 6374 696f 6e20  oll()` function 
-00002460: 7369 6d75 6c74 616e 656f 7573 6c79 2e0a  simultaneously..
-00002470: 0a41 6e20 6578 616d 706c 6520 796f 7520  .An example you 
-00002480: 6361 6e20 6669 6e64 2069 6e20 6f75 7220  can find in our 
-00002490: 4865 726f 6b75 2064 6570 6c6f 7920 7465  Heroku deploy te
-000024a0: 6d70 6c61 7465 2072 6570 6f3a 200a 0a68  mplate repo: ..h
-000024b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000024c0: 6d2f 4553 575a 592f 7465 6c65 6772 616d  m/ESWZY/telegram
-000024d0: 2d6e 6577 732d 6765 7474 696e 672d 7374  -news-getting-st
-000024e0: 6172 7465 642f 626c 6f62 2f6d 6173 7465  arted/blob/maste
-000024f0: 722f 6d61 696e 2e70 790a 0a23 2320 4578  r/main.py..## Ex
-00002500: 616d 706c 6520 4368 616e 6e65 6c0a 0a41  ample Channel..A
-00002510: 2054 656c 6567 7261 6d20 6368 616e 6e65   Telegram channe
-00002520: 6c20 6f66 205b 6261 7369 6320 6578 616d  l of [basic exam
-00002530: 706c 655d 2868 7474 7073 3a2f 2f67 6974  ple](https://git
-00002540: 6875 622e 636f 6d2f 4553 575a 592f 7465  hub.com/ESWZY/te
-00002550: 6c65 6772 616d 2d6e 6577 7323 6261 7369  legram-news#basi
-00002560: 632d 6578 616d 706c 6529 2066 6f72 2045  c-example) for E
-00002570: 6e67 6c69 7368 2057 696b 696e 6577 733a  nglish Wikinews:
-00002580: 205b 7e7e 4077 696b 696e 6577 735f 656e   [~~@wikinews_en
-00002590: 7e7e 5d28 6874 7470 733a 2f2f 742e 6d65  ~~](https://t.me
-000025a0: 2f6a 6f69 6e63 6861 742f 5437 5462 4a55  /joinchat/T7TbJU
-000025b0: 5770 6755 7047 6d61 7259 2920 2869 6e20  WpgUpGmarY) (in 
-000025c0: 456e 676c 6973 6829 0a0a 4120 5465 6c65  English)..A Tele
-000025d0: 6772 616d 2063 6861 6e6e 656c 2066 6f72  gram channel for
-000025e0: 2072 6561 6c74 696d 6520 6561 7274 6871   realtime earthq
-000025f0: 7561 6b65 2077 6172 6e69 6e67 2070 6f77  uake warning pow
-00002600: 6572 6564 2062 7920 5465 6c65 6772 616d  ered by Telegram
-00002610: 2d6e 6577 733a 205b 4065 6172 7468 7175  -news: [@earthqu
-00002620: 616b 655f 616c 6572 745d 2868 7474 7073  ake_alert](https
-00002630: 3a2f 2f74 2e6d 652f 732f 6561 7274 6871  ://t.me/s/earthq
-00002640: 7561 6b65 5f61 6c65 7274 2920 2869 6e20  uake_alert) (in 
-00002650: 4368 696e 6573 6529 0a0a 2323 2054 4f44  Chinese)..## TOD
-00002660: 4f0a 0a2d 205b 785d 2048 544d 4c20 6974  O..- [x] HTML it
-00002670: 656d 206c 6973 740a 2d20 5b78 5d20 4a53  em list.- [x] JS
-00002680: 4f4e 2069 7465 6d20 6c69 7374 0a2d 205b  ON item list.- [
-00002690: 785d 2058 4d4c 2069 7465 6d20 6c69 7374  x] XML item list
-000026a0: 0a2d 205b 785d 2053 656e 6420 496d 6167  .- [x] Send Imag
-000026b0: 650a 2d20 5b78 5d20 5365 6e64 2056 6964  e.- [x] Send Vid
-000026c0: 656f 0a2d 205b 785d 2053 656e 6420 6d65  eo.- [x] Send me
-000026d0: 6469 6120 6772 6f75 700a 2d20 5b20 5d20  dia group.- [ ] 
-000026e0: 5365 6e64 2066 696c 650a 2d20 5b20 5d20  Send file.- [ ] 
-000026f0: 5365 6e64 2061 7564 696f 0a2d 205b 785d  Send audio.- [x]
-00002700: 2046 696c 6520 7365 6e64 696e 6720 7265   File sending re
-00002710: 7472 790a 2d20 5b20 5d20 4343 2061 7320  try.- [ ] CC as 
-00002720: 652d 6d61 696c 0a2d 205b 205d 2057 6562  e-mail.- [ ] Web
-00002730: 686f 6f6b 0a2d 205b 205d 2055 7064 6174  hook.- [ ] Updat
-00002740: 6520 6d65 7373 6167 6520 6279 206d 6573  e message by mes
-00002750: 7361 6765 2049 440a 2d20 5b20 5d20 446f  sage ID.- [ ] Do
-00002760: 6375 6d65 6e74 0a2d 205b 205d 2047 5549  cument.- [ ] GUI
-00002770: 0a0a 2323 2046 6565 6462 6163 6b0a 0a46  ..## Feedback..F
-00002780: 6565 6c20 6672 6565 2074 6f20 636f 6e74  eel free to cont
-00002790: 6163 7420 7769 7468 206d 6520 6966 2079  act with me if y
-000027a0: 6f75 2068 6176 6520 616e 7920 7175 6573  ou have any ques
-000027b0: 7469 6f6e 2e20 416c 736f 2077 656c 636f  tion. Also welco
-000027c0: 6d65 2061 6e79 2063 6f6e 7472 6962 7574  me any contribut
-000027d0: 652e 0a0a 4966 2079 6f75 2062 7569 6c64  e...If you build
-000027e0: 2061 2063 6861 6e6e 656c 2062 7920 7468   a channel by th
-000027f0: 6973 2c20 646f 6e27 7420 666f 7267 6574  is, don't forget
-00002800: 2074 6f20 7368 6172 6520 7468 6174 2067   to share that g
-00002810: 6f6f 6420 6e65 7773 2077 6974 6820 7573  ood news with us
-00002820: 210a 0a23 2320 4c69 6365 6e73 650a 0a4c  !..## License..L
-00002830: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
-00002840: 6520 4d49 5420 4c69 6365 6e73 652e 0a0a  e MIT License...
-00002850: 0a                                       .
+00000100: 4c69 6365 6e73 653a 204d 4954 0a44 6573  License: MIT.Des
+00000110: 6372 6970 7469 6f6e 3a20 3c68 3120 616c  cription: <h1 al
+00000120: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000130: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000140: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00000150: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000160: 636f 6d2f 4553 575a 592f 7465 6c65 6772  com/ESWZY/telegr
+00000170: 616d 2d6e 6577 732f 6d61 7374 6572 2f64  am-news/master/d
+00000180: 6f63 732f 696d 6167 6573 2f62 616e 6e65  ocs/images/banne
+00000190: 722e 706e 6722 2061 6c74 3d22 5465 6c65  r.png" alt="Tele
+000001a0: 6772 616d 2d6e 6577 7322 3e0a 2020 2020  gram-news">.    
+000001b0: 2020 2020 2020 3c62 723e 5465 6c65 6772        <br>Telegr
+000001c0: 616d 2d6e 6577 733c 6272 3e0a 2020 2020  am-news<br>.    
+000001d0: 2020 2020 3c2f 6831 3e0a 2020 2020 2020      </h1>.      
+000001e0: 2020 0a20 2020 2020 2020 203c 6469 7620    .        <div 
+000001f0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000200: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000210: 2050 7974 686f 6e20 7061 636b 6167 6520   Python package 
+00000220: 666f 7220 6175 746f 6d61 7469 6361 6c6c  for automaticall
+00000230: 7920 6665 7463 6869 6e67 2061 6e64 2070  y fetching and p
+00000240: 7573 6869 6e67 206e 6577 7320 6279 2054  ushing news by T
+00000250: 656c 6567 7261 6d2e 0a20 2020 2020 2020  elegram..       
+00000260: 200a 2020 2020 2020 2020 5b21 5b50 7950   .        [![PyP
+00000270: 495d 2868 7474 7073 3a2f 2f69 6d67 2e73  I](https://img.s
+00000280: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00000290: 2f74 656c 6567 7261 6d2d 6e65 7773 295d  /telegram-news)]
+000002a0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000002b0: 672f 7072 6f6a 6563 742f 7465 6c65 6772  g/project/telegr
+000002c0: 616d 2d6e 6577 732f 290a 2020 2020 2020  am-news/).      
+000002d0: 2020 215b 5079 5049 202d 2050 7974 686f    ![PyPI - Pytho
+000002e0: 6e20 5665 7273 696f 6e5d 2868 7474 7073  n Version](https
+000002f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000300: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
+00000310: 732f 7465 6c65 6772 616d 2d6e 6577 733f  s/telegram-news?
+00000320: 6c6f 676f 3d70 7974 686f 6e29 0a20 2020  logo=python).   
+00000330: 2020 2020 205b 215b 4c69 6365 6e73 655d       [![License]
+00000340: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000350: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+00000360: 6963 656e 7365 2f45 5357 5a59 2f74 656c  icense/ESWZY/tel
+00000370: 6567 7261 6d2d 6e65 7773 295d 2868 7474  egram-news)](htt
+00000380: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000390: 4553 575a 592f 7465 6c65 6772 616d 2d6e  ESWZY/telegram-n
+000003a0: 6577 732f 626c 6f62 2f6d 6173 7465 722f  ews/blob/master/
+000003b0: 4c49 4345 4e53 4529 0a20 2020 2020 2020  LICENSE).       
+000003c0: 2021 5b50 7950 4920 2d20 446f 776e 6c6f   ![PyPI - Downlo
+000003d0: 6164 735d 2868 7474 7073 3a2f 2f69 6d67  ads](https://img
+000003e0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+000003f0: 2f64 6d2f 7465 6c65 6772 616d 2d6e 6577  /dm/telegram-new
+00000400: 7329 0a20 2020 2020 2020 200a 2020 2020  s).        .    
+00000410: 2020 2020 5b21 5b42 7569 6c64 2053 7461      [![Build Sta
+00000420: 7475 735d 2868 7474 7073 3a2f 2f69 6d67  tus](https://img
+00000430: 2e73 6869 656c 6473 2e69 6f2f 7472 6176  .shields.io/trav
+00000440: 6973 2f45 5357 5a59 2f74 656c 6567 7261  is/ESWZY/telegra
+00000450: 6d2d 6e65 7773 2f6d 6173 7465 723f 6c6f  m-news/master?lo
+00000460: 676f 3d74 7261 7669 7329 5d28 6874 7470  go=travis)](http
+00000470: 733a 2f2f 7472 6176 6973 2d63 692e 6f72  s://travis-ci.or
+00000480: 672f 4553 575a 592f 7465 6c65 6772 616d  g/ESWZY/telegram
+00000490: 2d6e 6577 7329 0a20 2020 2020 2020 205b  -news).        [
+000004a0: 215b 436f 6461 6379 2042 6164 6765 5d28  ![Codacy Badge](
+000004b0: 6874 7470 733a 2f2f 6170 692e 636f 6461  https://api.coda
+000004c0: 6379 2e63 6f6d 2f70 726f 6a65 6374 2f62  cy.com/project/b
+000004d0: 6164 6765 2f47 7261 6465 2f33 6330 3766  adge/Grade/3c07f
+000004e0: 6564 3532 3564 6134 3265 3839 6464 3364  ed525da42e89dd3d
+000004f0: 3033 3736 3435 3762 3464 3229 5d28 6874  0376457b4d2)](ht
+00000500: 7470 733a 2f2f 6170 702e 636f 6461 6379  tps://app.codacy
+00000510: 2e63 6f6d 2f6d 616e 7561 6c2f 4553 575a  .com/manual/ESWZ
+00000520: 592f 7465 6c65 6772 616d 2d6e 6577 733f  Y/telegram-news?
+00000530: 7574 6d5f 736f 7572 6365 3d67 6974 6875  utm_source=githu
+00000540: 622e 636f 6d26 7574 6d5f 6d65 6469 756d  b.com&utm_medium
+00000550: 3d72 6566 6572 7261 6c26 7574 6d5f 636f  =referral&utm_co
+00000560: 6e74 656e 743d 4553 575a 592f 7465 6c65  ntent=ESWZY/tele
+00000570: 6772 616d 2d6e 6577 7326 7574 6d5f 6361  gram-news&utm_ca
+00000580: 6d70 6169 676e 3d42 6164 6765 5f47 7261  mpaign=Badge_Gra
+00000590: 6465 5f44 6173 6862 6f61 7264 290a 2020  de_Dashboard).  
+000005a0: 2020 2020 2020 215b 4c61 7374 2063 6f6d        ![Last com
+000005b0: 6d69 745d 2868 7474 7073 3a2f 2f69 6d67  mit](https://img
+000005c0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+000005d0: 7562 2f6c 6173 742d 636f 6d6d 6974 2f45  ub/last-commit/E
+000005e0: 5357 5a59 2f74 656c 6567 7261 6d2d 6e65  SWZY/telegram-ne
+000005f0: 7773 290a 2020 2020 2020 2020 5b21 5b68  ws).        [![h
+00000600: 7474 7073 3a2f 2f74 2e6d 652f 6573 777a  ttps://t.me/eswz
+00000610: 795d 2868 7474 7073 3a2f 2f69 6d67 2e73  y](https://img.s
+00000620: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000630: 5465 6c65 6772 616d 2d45 5357 5a59 2d62  Telegram-ESWZY-b
+00000640: 6c75 652e 7376 673f 6c6f 676f 3d74 656c  lue.svg?logo=tel
+00000650: 6567 7261 6d29 5d28 6874 7470 733a 2f2f  egram)](https://
+00000660: 742e 6d65 2f65 7377 7a79 290a 2020 2020  t.me/eswzy).    
+00000670: 2020 2020 0a20 2020 2020 2020 203c 2f64      .        </d
+00000680: 6976 3e0a 2020 2020 2020 2020 0a20 2020  iv>.        .   
+00000690: 2020 2020 2023 2320 496e 7472 6f64 7563       ## Introduc
+000006a0: 7469 6f6e 0a20 2020 2020 2020 200a 2020  tion.        .  
+000006b0: 2020 2020 2020 5468 6973 2069 7320 6120        This is a 
+000006c0: 6561 7379 2d74 6f2d 6c65 6172 6e2c 2066  easy-to-learn, f
+000006d0: 6c65 7869 626c 6520 616e 6420 7374 616e  lexible and stan
+000006e0: 6461 7264 697a 6564 206d 6573 7361 6765  dardized message
+000006f0: 2066 6574 6368 696e 6720 616e 6420 7075   fetching and pu
+00000700: 7368 696e 6720 6672 616d 6577 6f72 6b2c  shing framework,
+00000710: 2065 7370 6563 6961 6c6c 7920 666f 7220   especially for 
+00000720: 5b54 656c 6567 7261 6d5d 2868 7474 703a  [Telegram](http:
+00000730: 2f2f 7777 772e 7465 6c65 6772 616d 2e6f  //www.telegram.o
+00000740: 7267 2920 616e 6420 5b54 656c 6567 7261  rg) and [Telegra
+00000750: 6d20 426f 745d 2868 7474 7073 3a2f 2f63  m Bot](https://c
+00000760: 6f72 652e 7465 6c65 6772 616d 2e6f 7267  ore.telegram.org
+00000770: 2f62 6f74 7329 2e0a 2020 2020 2020 2020  /bots)..        
+00000780: 0a20 2020 2020 2020 2054 6865 2074 6172  .        The tar
+00000790: 6765 7420 6e65 7773 2073 6f75 7263 6520  get news source 
+000007a0: 6361 6e20 6265 2048 544d 4c20 7061 6765  can be HTML page
+000007b0: 2c20 4a53 4f4e 2061 6e64 2058 4d4c 2e20  , JSON and XML. 
+000007c0: 5765 2061 6c73 6f20 7072 6f76 6964 6520  We also provide 
+000007d0: 6375 7374 6f6d 697a 6564 2070 726f 6365  customized proce
+000007e0: 7373 2066 6f72 2075 6e6b 6e6f 776e 2064  ss for unknown d
+000007f0: 6174 6120 666f 726d 6174 2e0a 2020 2020  ata format..    
+00000800: 2020 2020 0a20 2020 2020 2020 2050 7573      .        Pus
+00000810: 6820 7468 6520 6c61 7465 7374 206e 6577  h the latest new
+00000820: 7320 746f 2079 6f75 7220 6368 616e 6e65  s to your channe
+00000830: 6c20 6f72 2067 726f 7570 206f 6e63 6520  l or group once 
+00000840: 6974 2068 6170 7065 6e73 210a 2020 2020  it happens!.    
+00000850: 2020 2020 0a20 2020 2020 2020 2023 2320      .        ## 
+00000860: 496e 7374 616c 6c0a 2020 2020 2020 2020  Install.        
+00000870: 0a20 2020 2020 2020 2060 6060 7368 656c  .        ```shel
+00000880: 6c0a 2020 2020 2020 2020 2420 7069 7020  l.        $ pip 
+00000890: 696e 7374 616c 6c20 7465 6c65 6772 616d  install telegram
+000008a0: 2d6e 6577 730a 2020 2020 2020 2020 6060  -news.        ``
+000008b0: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
+000008c0: 2020 204f 722c 2079 6f75 2063 616e 2069     Or, you can i
+000008d0: 6e73 7461 6c6c 2062 7920 636c 6f6e 696e  nstall by clonin
+000008e0: 6720 7468 6973 2072 6570 6f73 6974 6f72  g this repositor
+000008f0: 793a 0a20 2020 2020 2020 200a 2020 2020  y:.        .    
+00000900: 2020 2020 6060 6073 6865 6c6c 0a20 2020      ```shell.   
+00000910: 2020 2020 2024 2067 6974 2063 6c6f 6e65       $ git clone
+00000920: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000930: 636f 6d2f 4553 575a 592f 7465 6c65 6772  com/ESWZY/telegr
+00000940: 616d 2d6e 6577 732e 6769 740a 2020 2020  am-news.git.    
+00000950: 2020 2020 2420 6364 2074 656c 6567 7261      $ cd telegra
+00000960: 6d2d 6e65 7773 0a20 2020 2020 2020 2024  m-news.        $
+00000970: 2070 7974 686f 6e20 7365 7475 702e 7079   python setup.py
+00000980: 2069 6e73 7461 6c6c 0a20 2020 2020 2020   install.       
+00000990: 2060 6060 0a20 2020 2020 2020 200a 2020   ```.        .  
+000009a0: 2020 2020 2020 2323 2050 7265 7061 7265        ## Prepare
+000009b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000009c0: 2020 4974 2064 6f65 7320 6e6f 7420 6e65    It does not ne
+000009d0: 6564 206d 7563 6820 736f 2074 6861 7420  ed much so that 
+000009e0: 796f 7520 6361 6e20 7275 6e20 796f 7572  you can run your
+000009f0: 2063 6f64 6520 616e 7977 6865 7265 2e0a   code anywhere..
+00000a00: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000a10: 2046 6972 7374 2c20 6173 6b20 5b40 426f   First, ask [@Bo
+00000a20: 7446 6174 6865 725d 2868 7474 7073 3a2f  tFather](https:/
+00000a30: 2f74 2e6d 652f 626f 7466 6174 6865 7229  /t.me/botfather)
+00000a40: 2066 6f72 2061 2062 6f74 2061 6e64 2062   for a bot and b
+00000a50: 6f74 2074 6f6b 656e 2e20 4166 7465 7220  ot token. After 
+00000a60: 7468 6174 2c20 6372 6561 7465 2061 2070  that, create a p
+00000a70: 7562 6c69 6320 5b63 6861 6e6e 656c 5d28  ublic [channel](
+00000a80: 6874 7470 733a 2f2f 7465 6c65 6772 616d  https://telegram
+00000a90: 2e6f 7267 2f74 6f75 722f 6368 616e 6e65  .org/tour/channe
+00000aa0: 6c73 2920 6f72 205b 6772 6f75 705d 2868  ls) or [group](h
+00000ab0: 7474 7073 3a2f 2f74 656c 6567 7261 6d2e  ttps://telegram.
+00000ac0: 6f72 672f 746f 7572 2f67 726f 7570 7329  org/tour/groups)
+00000ad0: 2c20 616e 6420 7265 6d65 6d62 6572 2063  , and remember c
+00000ae0: 6861 7420 6964 2079 6f75 206a 7573 7420  hat id you just 
+00000af0: 6e61 6d65 642e 2044 6f20 6e6f 7420 666f  named. Do not fo
+00000b00: 7267 6574 2074 6f20 696e 7669 7465 2079  rget to invite y
+00000b10: 6f75 7220 626f 7420 696e 746f 2079 6f75  our bot into you
+00000b20: 7220 6368 616e 6e65 6c20 6f72 2067 726f  r channel or gro
+00000b30: 7570 2061 6e64 206d 616b 6520 6974 2061  up and make it a
+00000b40: 6e20 6164 6d69 6e2e 0a20 2020 2020 2020  n admin..       
+00000b50: 200a 2020 2020 2020 2020 596f 7520 616c   .        You al
+00000b60: 736f 206e 6565 6420 6120 5351 4c20 6461  so need a SQL da
+00000b70: 7461 6261 7365 2e20 416e 7920 5351 4c20  tabase. Any SQL 
+00000b80: 6461 7461 6261 7365 2069 7320 4f4b 2e20  database is OK. 
+00000b90: 4573 7065 6369 616c 6c79 2c20 4920 7265  Especially, I re
+00000ba0: 636f 6d6d 656e 6420 5b50 6f73 7467 7265  commend [Postgre
+00000bb0: 5351 4c5d 2868 7474 7073 3a2f 2f77 7777  SQL](https://www
+00000bc0: 2e70 6f73 7467 7265 7371 6c2e 6f72 672f  .postgresql.org/
+00000bd0: 292e 0a20 2020 2020 2020 200a 2020 2020  )..        .    
+00000be0: 2020 2020 2323 2051 7569 636b 2064 6570      ## Quick dep
+00000bf0: 6c6f 7920 6f6e 2048 6572 6f6b 750a 2020  loy on Heroku.  
+00000c00: 2020 2020 2020 0a20 2020 2020 2020 2043        .        C
+00000c10: 6c69 636b 20f0 9f91 8720 6275 7474 6f6e  lick .... button
+00000c20: 2074 6f20 6465 706c 6f79 2061 6e20 6578   to deploy an ex
+00000c30: 616d 706c 6520 666f 7220 6672 6565 2e20  ample for free. 
+00000c40: 5079 7468 6f6e 2065 6e76 6972 6f6e 6d65  Python environme
+00000c50: 6e74 2061 6e64 2050 6f73 7467 7265 5351  nt and PostgreSQ
+00000c60: 4c20 6461 7461 6261 7365 2068 6176 6520  L database have 
+00000c70: 6265 656e 2070 7265 7061 7265 642e 0a20  been prepared.. 
+00000c80: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000c90: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000ca0: 2f68 6572 6f6b 752e 636f 6d2f 6465 706c  /heroku.com/depl
+00000cb0: 6f79 3f74 656d 706c 6174 653d 6874 7470  oy?template=http
+00000cc0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f45  s://github.com/E
+00000cd0: 5357 5a59 2f74 656c 6567 7261 6d2d 6e65  SWZY/telegram-ne
+00000ce0: 7773 2d67 6574 7469 6e67 2d73 7461 7274  ws-getting-start
+00000cf0: 6564 223e 0a20 2020 2020 2020 2020 203c  ed">.          <
+00000d00: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000d10: 2f77 7777 2e68 6572 6f6b 7563 646e 2e63  /www.herokucdn.c
+00000d20: 6f6d 2f64 6570 6c6f 792f 6275 7474 6f6e  om/deploy/button
+00000d30: 2e73 7667 2220 616c 743d 2244 6570 6c6f  .svg" alt="Deplo
+00000d40: 7922 3e0a 2020 2020 2020 2020 3c2f 613e  y">.        </a>
+00000d50: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000d60: 2020 4166 7465 7220 6465 706c 6f79 6d65    After deployme
+00000d70: 6e74 2c20 7374 6172 7420 7468 6520 776f  nt, start the wo
+00000d80: 726b 6572 2069 6e20 2252 6573 6f75 7263  rker in "Resourc
+00000d90: 6573 2220 7461 622c 2061 6e64 2074 6865  es" tab, and the
+00000da0: 6e20 796f 7520 6361 6e20 7365 6520 7468  n you can see th
+00000db0: 6520 6566 6665 6374 2069 6e20 796f 7572  e effect in your
+00000dc0: 2063 6861 6e6e 656c 2f67 726f 7570 2c20   channel/group, 
+00000dd0: 7768 6963 6820 636f 6e74 6169 6e73 2062  which contains b
+00000de0: 6f74 6820 5343 4d50 206e 6577 7320 616e  oth SCMP news an
+00000df0: 6420 5769 6b69 206e 6577 7320 6174 2073  d Wiki news at s
+00000e00: 616d 6520 7469 6d65 2e0a 2020 2020 2020  ame time..      
+00000e10: 2020 0a20 2020 2020 2020 2023 2320 5573    .        ## Us
+00000e20: 6167 650a 2020 2020 2020 2020 0a20 2020  age.        .   
+00000e30: 2020 2020 2054 686f 7365 2061 7265 2033       Those are 3
+00000e40: 2065 7861 6d70 6c65 7320 666f 7220 796f   examples for yo
+00000e50: 7520 746f 2075 6e64 6572 7374 616e 6420  u to understand 
+00000e60: 686f 7720 746f 2075 7365 2074 6865 2066  how to use the f
+00000e70: 7261 6d65 776f 726b 2e0a 2020 2020 2020  ramework..      
+00000e80: 2020 0a20 2020 2020 2020 2023 2323 2042    .        ### B
+00000e90: 6173 6963 2045 7861 6d70 6c65 0a20 2020  asic Example.   
+00000ea0: 2020 2020 200a 2020 2020 2020 2020 6060       .        ``
+00000eb0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00000ec0: 696d 706f 7274 206f 730a 2020 2020 2020  import os.      
+00000ed0: 2020 6672 6f6d 2073 716c 616c 6368 656d    from sqlalchem
+00000ee0: 7920 696d 706f 7274 2063 7265 6174 655f  y import create_
+00000ef0: 656e 6769 6e65 0a20 2020 2020 2020 2066  engine.        f
+00000f00: 726f 6d20 7371 6c61 6c63 6865 6d79 2e6f  rom sqlalchemy.o
+00000f10: 726d 2069 6d70 6f72 7420 5365 7373 696f  rm import Sessio
+00000f20: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
+00000f30: 2020 2066 726f 6d20 7465 6c65 6772 616d     from telegram
+00000f40: 5f6e 6577 732e 7465 6d70 6c61 7465 2069  _news.template i
+00000f50: 6d70 6f72 7420 496e 666f 4578 7472 6163  mport InfoExtrac
+00000f60: 746f 722c 204e 6577 7350 6f73 746d 616e  tor, NewsPostman
+00000f70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000f80: 2020 2320 5468 7265 6520 7265 7175 6972    # Three requir
+00000f90: 6564 2066 6965 6c64 733a 0a20 2020 2020  ed fields:.     
+00000fa0: 2020 2023 2059 6f75 7220 626f 7420 746f     # Your bot to
+00000fb0: 6b65 6e20 6f62 7461 696e 6564 2066 726f  ken obtained fro
+00000fc0: 6d20 4042 6f74 4661 7468 6572 0a20 2020  m @BotFather.   
+00000fd0: 2020 2020 2062 6f74 5f74 6f6b 656e 203d       bot_token =
+00000fe0: 206f 732e 6765 7465 6e76 2822 544f 4b45   os.getenv("TOKE
+00000ff0: 4e22 290a 2020 2020 2020 2020 2320 4164  N").        # Ad
+00001000: 6420 796f 7572 2062 6f74 7320 696e 746f  d your bots into
+00001010: 2061 2063 6861 6e6e 656c 2061 7320 616e   a channel as an
+00001020: 2061 646d 696e 6973 7472 6174 6f72 0a20   administrator. 
+00001030: 2020 2020 2020 2063 6861 6e6e 656c 203d         channel =
+00001040: 206f 732e 6765 7465 6e76 2822 4348 414e   os.getenv("CHAN
+00001050: 4e45 4c22 290a 2020 2020 2020 2020 2320  NEL").        # 
+00001060: 596f 7572 2064 6174 6162 6173 6520 746f  Your database to
+00001070: 2073 746f 7265 206f 6c64 206d 6573 7361   store old messa
+00001080: 6765 732e 0a20 2020 2020 2020 2044 4154  ges..        DAT
+00001090: 4142 4153 455f 5552 4c20 3d20 6f73 2e67  ABASE_URL = os.g
+000010a0: 6574 656e 7628 2244 4154 4142 4153 455f  etenv("DATABASE_
+000010b0: 5552 4c22 290a 2020 2020 2020 2020 0a20  URL").        . 
+000010c0: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+000010d0: 6120 6461 7461 6261 7365 2073 6573 7369  a database sessi
+000010e0: 6f6e 0a20 2020 2020 2020 2065 6e67 696e  on.        engin
+000010f0: 6520 3d20 6372 6561 7465 5f65 6e67 696e  e = create_engin
+00001100: 6528 4441 5441 4241 5345 5f55 524c 290a  e(DATABASE_URL).
+00001110: 2020 2020 2020 2020 6462 203d 2053 6573          db = Ses
+00001120: 7369 6f6e 2862 696e 643d 656e 6769 6e65  sion(bind=engine
+00001130: 2e63 6f6e 6e65 6374 2829 290a 2020 2020  .connect()).    
+00001140: 2020 2020 0a20 2020 2020 2020 2023 2054      .        # T
+00001150: 6865 206e 6577 7320 736f 7572 6365 0a20  he news source. 
+00001160: 2020 2020 2020 2075 726c 203d 2022 6874         url = "ht
+00001170: 7470 733a 2f2f 656e 2e77 696b 696e 6577  tps://en.wikinew
+00001180: 732e 6f72 672f 7769 6b69 2f4d 6169 6e5f  s.org/wiki/Main_
+00001190: 5061 6765 220a 2020 2020 2020 2020 7461  Page".        ta
+000011a0: 6720 3d20 2257 696b 6920 4e65 7773 220a  g = "Wiki News".
+000011b0: 2020 2020 2020 2020 7461 626c 655f 6e61          table_na
+000011c0: 6d65 203d 2022 7769 6b69 6e65 7773 220a  me = "wikinews".
+000011d0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000011e0: 2023 2049 6e66 6f20 6578 7472 6163 746f   # Info extracto
+000011f0: 7220 746f 2070 726f 6365 7373 2064 6174  r to process dat
+00001200: 6120 666f 726d 6174 0a20 2020 2020 2020  a format.       
+00001210: 2069 6520 3d20 496e 666f 4578 7472 6163   ie = InfoExtrac
+00001220: 746f 7228 290a 2020 2020 2020 2020 0a20  tor().        . 
+00001230: 2020 2020 2020 2023 2053 656c 6563 7420         # Select 
+00001240: 7365 6c65 6374 2065 6c65 6d65 6e74 2062  select element b
+00001250: 7920 4353 532d 6261 7365 6420 7365 6c65  y CSS-based sele
+00001260: 6374 6f72 0a20 2020 2020 2020 2069 652e  ctor.        ie.
+00001270: 7365 745f 6c69 7374 5f73 656c 6563 746f  set_list_selecto
+00001280: 7228 2723 4d61 696e 5061 6765 5f6c 6174  r('#MainPage_lat
+00001290: 6573 745f 6e65 7773 5f74 6578 7420 3e20  est_news_text > 
+000012a0: 756c 203e 206c 6927 290a 2020 2020 2020  ul > li').      
+000012b0: 2020 6965 2e73 6574 5f74 6974 6c65 5f73    ie.set_title_s
+000012c0: 656c 6563 746f 7228 2723 6669 7273 7448  elector('#firstH
+000012d0: 6561 6469 6e67 2729 0a20 2020 2020 2020  eading').       
+000012e0: 2069 652e 7365 745f 7061 7261 6772 6170   ie.set_paragrap
+000012f0: 685f 7365 6c65 6374 6f72 2827 236d 772d  h_selector('#mw-
+00001300: 636f 6e74 656e 742d 7465 7874 203e 2064  content-text > d
+00001310: 6976 203e 2070 3a6e 6f74 2870 3a6e 7468  iv > p:not(p:nth
+00001320: 2d63 6869 6c64 2831 2929 2729 0a20 2020  -child(1))').   
+00001330: 2020 2020 2069 652e 7365 745f 7469 6d65       ie.set_time
+00001340: 5f73 656c 6563 746f 7228 2723 6d77 2d63  _selector('#mw-c
+00001350: 6f6e 7465 6e74 2d74 6578 7420 3e20 6469  ontent-text > di
+00001360: 7620 3e20 703a 6e74 682d 6368 696c 6428  v > p:nth-child(
+00001370: 3129 203e 2073 7472 6f6e 6727 290a 2020  1) > strong').  
+00001380: 2020 2020 2020 6965 2e73 6574 5f73 6f75        ie.set_sou
+00001390: 7263 655f 7365 6c65 6374 6f72 2827 7370  rce_selector('sp
+000013a0: 616e 2e73 6f75 7263 6554 656d 706c 6174  an.sourceTemplat
+000013b0: 6527 290a 2020 2020 2020 2020 0a20 2020  e').        .   
+000013c0: 2020 2020 2023 2053 6574 2061 206d 6178       # Set a max
+000013d0: 206c 656e 6774 6820 666f 7220 706f 7374   length for post
+000013e0: 2c20 4d61 7820 6973 2034 3039 360a 2020  , Max is 4096.  
+000013f0: 2020 2020 2020 6965 2e6d 6178 5f70 6f73        ie.max_pos
+00001400: 745f 6c65 6e67 7468 203d 2032 3030 300a  t_length = 2000.
+00001410: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001420: 2023 204e 6577 7320 706f 7374 6d61 6e20   # News postman 
+00001430: 746f 206d 616e 6167 6520 7365 6e64 696e  to manage sendin
+00001440: 6720 6166 6661 6972 0a20 2020 2020 2020  g affair.       
+00001450: 206e 7020 3d20 4e65 7773 506f 7374 6d61   np = NewsPostma
+00001460: 6e28 6c69 7374 5552 4c73 3d5b 7572 6c2c  n(listURLs=[url,
+00001470: 205d 2c20 7365 6e64 4c69 7374 3d5b 6368   ], sendList=[ch
+00001480: 616e 6e65 6c2c 205d 2c20 6462 3d64 622c  annel, ], db=db,
+00001490: 2074 6167 3d74 6167 290a 2020 2020 2020   tag=tag).      
+000014a0: 2020 6e70 2e73 6574 5f62 6f74 5f74 6f6b    np.set_bot_tok
+000014b0: 656e 2862 6f74 5f74 6f6b 656e 290a 2020  en(bot_token).  
+000014c0: 2020 2020 2020 6e70 2e73 6574 5f65 7874        np.set_ext
+000014d0: 7261 6374 6f72 2869 6529 0a20 2020 2020  ractor(ie).     
+000014e0: 2020 206e 702e 7365 745f 7461 626c 655f     np.set_table_
+000014f0: 6e61 6d65 2874 6162 6c65 5f6e 616d 6529  name(table_name)
+00001500: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001510: 2020 2320 5374 6172 7420 746f 2077 6f72    # Start to wor
+00001520: 6b21 0a20 2020 2020 2020 206e 702e 706f  k!.        np.po
+00001530: 6c6c 2829 0a20 2020 2020 2020 2060 6060  ll().        ```
+00001540: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001550: 2020 5479 7069 6361 6c20 7265 7375 6c74    Typical result
+00001560: 733a 0a20 2020 2020 2020 200a 2020 2020  s:.        .    
+00001570: 2020 2020 3c64 6976 2061 6c69 676e 3d22      <div align="
+00001580: 6365 6e74 6572 223e 0a20 2020 2020 2020  center">.       
+00001590: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+000015a0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+000015b0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f45  sercontent.com/E
+000015c0: 5357 5a59 2f74 656c 6567 7261 6d2d 6e65  SWZY/telegram-ne
+000015d0: 7773 2f6d 6173 7465 722f 646f 6373 2f69  ws/master/docs/i
+000015e0: 6d61 6765 732f 6465 6d6f 312e 706e 6722  mages/demo1.png"
+000015f0: 2061 6c74 3d22 4465 6d6f 2031 2220 7769   alt="Demo 1" wi
+00001600: 6474 683d 2234 3025 223e 0a20 2020 2020  dth="40%">.     
+00001610: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+00001620: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00001630: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00001640: 2f45 5357 5a59 2f74 656c 6567 7261 6d2d  /ESWZY/telegram-
+00001650: 6e65 7773 2f6d 6173 7465 722f 646f 6373  news/master/docs
+00001660: 2f69 6d61 6765 732f 6465 6d6f 322e 706e  /images/demo2.pn
+00001670: 6722 2061 6c74 3d22 4465 6d6f 2032 2220  g" alt="Demo 2" 
+00001680: 7769 6474 683d 2234 3025 223e 0a20 2020  width="40%">.   
+00001690: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+000016a0: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+000016b0: 2041 6476 616e 6365 6420 4578 616d 706c   Advanced Exampl
+000016c0: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
+000016d0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+000016e0: 2020 2020 2069 6d70 6f72 7420 6f73 0a20       import os. 
+000016f0: 2020 2020 2020 2066 726f 6d20 7371 6c61         from sqla
+00001700: 6c63 6865 6d79 2069 6d70 6f72 7420 6372  lchemy import cr
+00001710: 6561 7465 5f65 6e67 696e 650a 2020 2020  eate_engine.    
+00001720: 2020 2020 6672 6f6d 2073 716c 616c 6368      from sqlalch
+00001730: 656d 792e 6f72 6d20 696d 706f 7274 2053  emy.orm import S
+00001740: 6573 7369 6f6e 0a20 2020 2020 2020 2066  ession.        f
+00001750: 726f 6d20 7465 6c65 6772 616d 5f6e 6577  rom telegram_new
+00001760: 732e 7465 6d70 6c61 7465 2069 6d70 6f72  s.template impor
+00001770: 7420 496e 666f 4578 7472 6163 746f 722c  t InfoExtractor,
+00001780: 204e 6577 7350 6f73 746d 616e 0a20 2020   NewsPostman.   
+00001790: 2020 2020 2062 6f74 5f74 6f6b 656e 203d       bot_token =
+000017a0: 206f 732e 6765 7465 6e76 2822 544f 4b45   os.getenv("TOKE
+000017b0: 4e22 290a 2020 2020 2020 2020 6368 616e  N").        chan
+000017c0: 6e65 6c20 3d20 6f73 2e67 6574 656e 7628  nel = os.getenv(
+000017d0: 2243 4841 4e4e 454c 2229 0a20 2020 2020  "CHANNEL").     
+000017e0: 2020 2044 4154 4142 4153 455f 5552 4c20     DATABASE_URL 
+000017f0: 3d20 6f73 2e67 6574 656e 7628 2244 4154  = os.getenv("DAT
+00001800: 4142 4153 455f 5552 4c22 290a 2020 2020  ABASE_URL").    
+00001810: 2020 2020 656e 6769 6e65 203d 2063 7265      engine = cre
+00001820: 6174 655f 656e 6769 6e65 2844 4154 4142  ate_engine(DATAB
+00001830: 4153 455f 5552 4c29 0a20 2020 2020 2020  ASE_URL).       
+00001840: 2064 6220 3d20 5365 7373 696f 6e28 6269   db = Session(bi
+00001850: 6e64 3d65 6e67 696e 652e 636f 6e6e 6563  nd=engine.connec
+00001860: 7428 2929 0a20 2020 2020 2020 200a 2020  t()).        .  
+00001870: 2020 2020 2020 2320 4162 6f76 6520 636f        # Above co
+00001880: 6465 2069 7320 6173 2073 616d 6520 6173  de is as same as
+00001890: 2074 6865 2062 6173 6963 2065 7861 6d70   the basic examp
+000018a0: 6c65 2c20 796f 7520 6361 6e20 7265 7573  le, you can reus
+000018b0: 6520 7468 6f73 6520 636f 6465 2064 6972  e those code dir
+000018c0: 6563 746c 790a 2020 2020 2020 2020 0a20  ectly.        . 
+000018d0: 2020 2020 2020 2075 726c 5f32 203d 2022         url_2 = "
+000018e0: 6874 7470 733a 2f2f 7777 772e 636e 6265  https://www.cnbe
+000018f0: 7461 2e63 6f6d 2f22 0a20 2020 2020 2020  ta.com/".       
+00001900: 2074 6167 5f32 203d 2022 636e 4265 7461   tag_2 = "cnBeta
+00001910: 220a 2020 2020 2020 2020 7461 626c 655f  ".        table_
+00001920: 6e61 6d65 5f32 203d 2022 636e 6265 7461  name_2 = "cnbeta
+00001930: 6e65 7773 220a 2020 2020 2020 2020 0a20  news".        . 
+00001940: 2020 2020 2020 2069 655f 3220 3d20 496e         ie_2 = In
+00001950: 666f 4578 7472 6163 746f 7228 290a 2020  foExtractor().  
+00001960: 2020 2020 2020 6965 5f32 2e73 6574 5f6c        ie_2.set_l
+00001970: 6973 745f 7365 6c65 6374 6f72 2827 2e69  ist_selector('.i
+00001980: 7465 6d73 2d61 7265 6120 3e20 6469 7620  tems-area > div 
+00001990: 3e20 646c 203e 2064 7420 3e20 6127 290a  > dl > dt > a').
+000019a0: 2020 2020 2020 2020 6965 5f32 2e73 6574          ie_2.set
+000019b0: 5f74 6974 6c65 5f73 656c 6563 746f 7228  _title_selector(
+000019c0: 2768 6561 6465 7220 3e20 6831 2729 0a20  'header > h1'). 
+000019d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000019e0: 2320 5365 6c65 6374 206d 616e 7920 7461  # Select many ta
+000019f0: 7267 6574 2061 7420 7361 6d65 2074 696d  rget at same tim
+00001a00: 6520 2020 200a 2020 2020 2020 2020 6965  e    .        ie
+00001a10: 5f32 2e73 6574 5f70 6172 6167 7261 7068  _2.set_paragraph
+00001a20: 5f73 656c 6563 746f 7228 2764 6976 2e63  _selector('div.c
+00001a30: 6e62 6574 612d 6172 7469 636c 652d 626f  nbeta-article-bo
+00001a40: 6479 203e 2064 6976 2e61 7274 6963 6c65  dy > div.article
+00001a50: 2d73 756d 6d61 7279 203e 2070 2c20 2720  -summary > p, ' 
+00001a60: 2023 2053 756d 6d61 7279 206f 6e6c 790a   # Summary only.
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a90: 2020 2020 2764 6976 2e63 6e62 6574 612d      'div.cnbeta-
+00001aa0: 6172 7469 636c 652d 626f 6479 203e 2064  article-body > d
+00001ab0: 6976 2e61 7274 6963 6c65 2d63 6f6e 7465  iv.article-conte
+00001ac0: 6e74 203e 2070 2729 2020 2023 2043 6f6e  nt > p')   # Con
+00001ad0: 7465 6e74 206f 6e6c 790a 2020 2020 2020  tent only.      
+00001ae0: 2020 6965 5f32 2e73 6574 5f74 696d 655f    ie_2.set_time_
+00001af0: 7365 6c65 6374 6f72 2827 6865 6164 6572  selector('header
+00001b00: 203e 2064 6976 203e 2073 7061 6e3a 6e74   > div > span:nt
+00001b10: 682d 6368 696c 6428 3129 2729 0a20 2020  h-child(1)').   
+00001b20: 2020 2020 2069 655f 322e 7365 745f 736f       ie_2.set_so
+00001b30: 7572 6365 5f73 656c 6563 746f 7228 2768  urce_selector('h
+00001b40: 6561 6465 7220 3e20 6469 7620 3e20 7370  eader > div > sp
+00001b50: 616e 2e73 6f75 7263 6527 290a 2020 2020  an.source').    
+00001b60: 2020 2020 0a20 2020 2020 2020 2023 2053      .        # S
+00001b70: 656c 6563 7420 696d 6167 6520 746f 2064  elect image to d
+00001b80: 6973 706c 6179 2c20 7468 656e 2074 6865  isplay, then the
+00001b90: 206d 6178 206c 656e 6774 6820 6973 2064   max length is d
+00001ba0: 6f77 6e20 746f 2031 3032 340a 2020 2020  own to 1024.    
+00001bb0: 2020 2020 6965 5f32 2e73 6574 5f69 6d61      ie_2.set_ima
+00001bc0: 6765 5f73 656c 6563 746f 7228 2764 6976  ge_selector('div
+00001bd0: 2e63 6e62 6574 612d 6172 7469 636c 652d  .cnbeta-article-
+00001be0: 626f 6479 203e 2064 6976 2e61 7274 6963  body > div.artic
+00001bf0: 6c65 2d73 756d 6d61 7279 203e 2070 2069  le-summary > p i
+00001c00: 6d67 2c20 2720 2023 2046 726f 6d20 7375  mg, '  # From su
+00001c10: 6d6d 6172 7920 6f6e 6c79 0a20 2020 2020  mmary only.     
+00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c30: 2020 2020 2020 2020 2020 2027 6469 762e             'div.
+00001c40: 636e 6265 7461 2d61 7274 6963 6c65 2d62  cnbeta-article-b
+00001c50: 6f64 7920 3e20 6469 762e 6172 7469 636c  ody > div.articl
+00001c60: 652d 636f 6e74 656e 7420 3e20 7020 696d  e-content > p im
+00001c70: 6727 2920 2020 2320 4672 6f6d 2063 6f6e  g')   # From con
+00001c80: 7465 6e74 206f 6e6c 790a 2020 2020 2020  tent only.      
+00001c90: 2020 6965 5f32 2e6d 6178 5f70 6f73 745f    ie_2.max_post_
+00001ca0: 6c65 6e67 7468 203d 2031 3030 300a 2020  length = 1000.  
+00001cb0: 2020 2020 2020 0a20 2020 2020 2020 206e        .        n
+00001cc0: 705f 3220 3d20 4e65 7773 506f 7374 6d61  p_2 = NewsPostma
+00001cd0: 6e28 6c69 7374 5552 4c73 3d5b 7572 6c5f  n(listURLs=[url_
+00001ce0: 322c 205d 2c20 7365 6e64 4c69 7374 3d5b  2, ], sendList=[
+00001cf0: 6368 616e 6e65 6c5d 2c20 7461 673d 7461  channel], tag=ta
+00001d00: 675f 322c 2064 623d 6462 290a 2020 2020  g_2, db=db).    
+00001d10: 2020 2020 6e70 5f32 2e73 6574 5f65 7874      np_2.set_ext
+00001d20: 7261 6374 6f72 2869 655f 3229 0a20 2020  ractor(ie_2).   
+00001d30: 2020 2020 206e 705f 322e 7365 745f 7461       np_2.set_ta
+00001d40: 626c 655f 6e61 6d65 2874 6162 6c65 5f6e  ble_name(table_n
+00001d50: 616d 655f 3229 0a20 2020 2020 2020 206e  ame_2).        n
+00001d60: 705f 322e 706f 6c6c 2829 0a20 2020 2020  p_2.poll().     
+00001d70: 2020 2060 6060 0a20 2020 2020 2020 200a     ```.        .
+00001d80: 2020 2020 2020 2020 5479 7069 6361 6c20          Typical 
+00001d90: 7265 7375 6c74 733a 0a20 2020 2020 2020  results:.       
+00001da0: 200a 2020 2020 2020 2020 3c64 6976 2061   .        <div a
+00001db0: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00001dc0: 2020 2020 2020 2020 203c 696d 6720 7372           <img sr
+00001dd0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00001de0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001df0: 2e63 6f6d 2f45 5357 5a59 2f74 656c 6567  .com/ESWZY/teleg
+00001e00: 7261 6d2d 6e65 7773 2f6d 6173 7465 722f  ram-news/master/
+00001e10: 646f 6373 2f69 6d61 6765 732f 6465 6d6f  docs/images/demo
+00001e20: 332e 706e 6722 2061 6c74 3d22 4465 6d6f  3.png" alt="Demo
+00001e30: 2033 2220 7769 6474 683d 2234 3025 223e   3" width="40%">
+00001e40: 0a20 2020 2020 2020 2020 203c 696d 6720  .          <img 
+00001e50: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00001e60: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00001e70: 6e74 2e63 6f6d 2f45 5357 5a59 2f74 656c  nt.com/ESWZY/tel
+00001e80: 6567 7261 6d2d 6e65 7773 2f6d 6173 7465  egram-news/maste
+00001e90: 722f 646f 6373 2f69 6d61 6765 732f 6465  r/docs/images/de
+00001ea0: 6d6f 342e 706e 6722 2061 6c74 3d22 4465  mo4.png" alt="De
+00001eb0: 6d6f 2034 2220 7769 6474 683d 2234 3025  mo 4" width="40%
+00001ec0: 223e 0a20 2020 2020 2020 203c 2f64 6976  ">.        </div
+00001ed0: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
+00001ee0: 2020 2023 2323 2041 6476 616e 6365 6420     ### Advanced 
+00001ef0: 4578 616d 706c 6520 666f 7220 4a53 4f4e  Example for JSON
+00001f00: 2061 6e64 2058 4d4c 0a20 2020 2020 2020   and XML.       
+00001f10: 200a 2020 2020 2020 2020 5468 6520 6861   .        The ha
+00001f20: 6e64 6c65 2066 6f72 204a 534f 4e20 616e  ndle for JSON an
+00001f30: 6420 584d 4c20 6172 6520 7175 6974 6520  d XML are quite 
+00001f40: 7369 6d69 6c61 722e 2059 6f75 2063 616e  similar. You can
+00001f50: 2063 6f6e 7665 7274 2058 4d4c 2074 6f20   convert XML to 
+00001f60: 4a53 4f4e 2062 7920 6675 6e63 7469 6f6e  JSON by function
+00001f70: 2060 7465 6c65 6772 616d 5f6e 6577 732e   `telegram_news.
+00001f80: 7574 696c 732e 786d 6c5f 746f 5f6a 736f  utils.xml_to_jso
+00001f90: 6e60 2c20 616e 6420 7573 6520 604e 6577  n`, and use `New
+00001fa0: 7350 6f73 746d 616e 4a53 4f4e 6020 616e  sPostmanJSON` an
+00001fb0: 6420 6049 6e66 6f45 7874 7261 6374 6f72  d `InfoExtractor
+00001fc0: 4a53 4f4e 602e 204f 722c 2079 6f75 2063  JSON`. Or, you c
+00001fd0: 616e 2075 7365 2060 4e65 7773 506f 7374  an use `NewsPost
+00001fe0: 6d61 6e58 4d4c 6020 616e 6420 6049 6e66  manXML` and `Inf
+00001ff0: 6f45 7874 7261 6374 6f72 584d 4c60 2064  oExtractorXML` d
+00002000: 6972 6563 746c 792e 0a20 2020 2020 2020  irectly..       
+00002010: 200a 2020 2020 2020 2020 596f 7520 7368   .        You sh
+00002020: 6f75 6c64 2075 7365 206b 6579 206c 6973  ould use key lis
+00002030: 7420 746f 2072 6563 7572 7369 7665 6c79  t to recursively
+00002040: 2072 6f75 7465 2074 6f20 7468 6520 696e   route to the in
+00002050: 666f 726d 6174 696f 6e20 796f 7520 7761  formation you wa
+00002060: 6e74 2e0a 2020 2020 2020 2020 0a20 2020  nt..        .   
+00002070: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
+00002080: 2020 2020 2020 2069 6d70 6f72 7420 6861         import ha
+00002090: 7368 6c69 620a 2020 2020 2020 2020 696d  shlib.        im
+000020a0: 706f 7274 206a 736f 6e0a 2020 2020 2020  port json.      
+000020b0: 2020 696d 706f 7274 206f 730a 2020 2020    import os.    
+000020c0: 2020 2020 6672 6f6d 2073 716c 616c 6368      from sqlalch
+000020d0: 656d 7920 696d 706f 7274 2063 7265 6174  emy import creat
+000020e0: 655f 656e 6769 6e65 0a20 2020 2020 2020  e_engine.       
+000020f0: 2066 726f 6d20 7371 6c61 6c63 6865 6d79   from sqlalchemy
+00002100: 2e6f 726d 2069 6d70 6f72 7420 5365 7373  .orm import Sess
+00002110: 696f 6e0a 2020 2020 2020 2020 6672 6f6d  ion.        from
+00002120: 2074 656c 6567 7261 6d5f 6e65 7773 2e74   telegram_news.t
+00002130: 656d 706c 6174 6520 696d 706f 7274 2049  emplate import I
+00002140: 6e66 6f45 7874 7261 6374 6f72 4a53 4f4e  nfoExtractorJSON
+00002150: 2c20 4e65 7773 506f 7374 6d61 6e4a 534f  , NewsPostmanJSO
+00002160: 4e0a 2020 2020 2020 2020 6672 6f6d 2074  N.        from t
+00002170: 656c 6567 7261 6d5f 6e65 7773 2e75 7469  elegram_news.uti
+00002180: 6c73 2069 6d70 6f72 7420 786d 6c5f 746f  ls import xml_to
+00002190: 5f6a 736f 6e0a 2020 2020 2020 2020 626f  _json.        bo
+000021a0: 745f 746f 6b65 6e20 3d20 6f73 2e67 6574  t_token = os.get
+000021b0: 656e 7628 2254 4f4b 454e 2229 0a20 2020  env("TOKEN").   
+000021c0: 2020 2020 2063 6861 6e6e 656c 203d 206f       channel = o
+000021d0: 732e 6765 7465 6e76 2822 4348 414e 4e45  s.getenv("CHANNE
+000021e0: 4c22 290a 2020 2020 2020 2020 4441 5441  L").        DATA
+000021f0: 4241 5345 5f55 524c 203d 206f 732e 6765  BASE_URL = os.ge
+00002200: 7465 6e76 2822 4441 5441 4241 5345 5f55  tenv("DATABASE_U
+00002210: 524c 2229 0a20 2020 2020 2020 2065 6e67  RL").        eng
+00002220: 696e 6520 3d20 6372 6561 7465 5f65 6e67  ine = create_eng
+00002230: 696e 6528 4441 5441 4241 5345 5f55 524c  ine(DATABASE_URL
+00002240: 290a 2020 2020 2020 2020 6462 203d 2053  ).        db = S
+00002250: 6573 7369 6f6e 2862 696e 643d 656e 6769  ession(bind=engi
+00002260: 6e65 2e63 6f6e 6e65 6374 2829 290a 2020  ne.connect()).  
+00002270: 2020 2020 2020 0a20 2020 2020 2020 2075        .        u
+00002280: 726c 5f33 203d 2022 6874 7470 733a 2f2f  rl_3 = "https://
+00002290: 7777 772e 7363 6d70 2e63 6f6d 2f72 7373  www.scmp.com/rss
+000022a0: 2f39 312f 6665 6564 220a 2020 2020 2020  /91/feed".      
+000022b0: 2020 7461 675f 3320 3d20 2253 434d 5022    tag_3 = "SCMP"
+000022c0: 0a20 2020 2020 2020 2074 6162 6c65 5f6e  .        table_n
+000022d0: 616d 655f 3320 3d20 2273 636d 706e 6577  ame_3 = "scmpnew
+000022e0: 7322 0a20 2020 2020 2020 200a 2020 2020  s".        .    
+000022f0: 2020 2020 6965 5f33 203d 2049 6e66 6f45      ie_3 = InfoE
+00002300: 7874 7261 6374 6f72 4a53 4f4e 2829 0a20  xtractorJSON(). 
+00002310: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002320: 2320 5072 652d 7072 6f63 6573 7320 7468  # Pre-process th
+00002330: 6520 584d 4c20 7374 7269 6e67 2c20 636f  e XML string, co
+00002340: 6e76 6572 7420 746f 204a 534f 4e20 7374  nvert to JSON st
+00002350: 7269 6e67 0a20 2020 2020 2020 2064 6566  ring.        def
+00002360: 206c 6973 745f 7072 655f 7072 6f63 6573   list_pre_proces
+00002370: 7328 7465 7874 293a 0a20 2020 2020 2020  s(text):.       
+00002380: 2020 2020 2074 6578 7420 3d20 6a73 6f6e       text = json
+00002390: 2e6c 6f61 6473 2878 6d6c 5f74 6f5f 6a73  .loads(xml_to_js
+000023a0: 6f6e 2874 6578 7429 290a 2020 2020 2020  on(text)).      
+000023b0: 2020 2020 2020 7265 7475 726e 206a 736f        return jso
+000023c0: 6e2e 6475 6d70 7328 7465 7874 290a 2020  n.dumps(text).  
+000023d0: 2020 2020 2020 6965 5f33 2e73 6574 5f6c        ie_3.set_l
+000023e0: 6973 745f 7072 655f 7072 6f63 6573 735f  ist_pre_process_
+000023f0: 706f 6c69 6379 286c 6973 745f 7072 655f  policy(list_pre_
+00002400: 7072 6f63 6573 7329 0a20 2020 2020 2020  process).       
+00002410: 200a 2020 2020 2020 2020 2320 526f 7574   .        # Rout
+00002420: 6520 6279 206b 6579 206c 6973 740a 2020  e by key list.  
+00002430: 2020 2020 2020 6965 5f33 2e73 6574 5f6c        ie_3.set_l
+00002440: 6973 745f 726f 7574 6572 285b 2772 7373  ist_router(['rss
+00002450: 272c 2027 6368 616e 6e65 6c27 2c20 2769  ', 'channel', 'i
+00002460: 7465 6d27 5d29 0a20 2020 2020 2020 2069  tem']).        i
+00002470: 655f 332e 7365 745f 6c69 6e6b 5f72 6f75  e_3.set_link_rou
+00002480: 7465 7228 5b27 6c69 6e6b 275d 290a 2020  ter(['link']).  
+00002490: 2020 2020 2020 6965 5f33 2e73 6574 5f74        ie_3.set_t
+000024a0: 6974 6c65 5f72 6f75 7465 7228 5b27 7469  itle_router(['ti
+000024b0: 746c 6527 5d29 0a20 2020 2020 2020 2069  tle']).        i
+000024c0: 655f 332e 7365 745f 7061 7261 6772 6170  e_3.set_paragrap
+000024d0: 6873 5f72 6f75 7465 7228 5b27 6465 7363  hs_router(['desc
+000024e0: 7269 7074 696f 6e27 5d29 0a20 2020 2020  ription']).     
+000024f0: 2020 2069 655f 332e 7365 745f 7469 6d65     ie_3.set_time
+00002500: 5f72 6f75 7465 7228 5b27 7075 6244 6174  _router(['pubDat
+00002510: 6527 5d29 0a20 2020 2020 2020 2069 655f  e']).        ie_
+00002520: 332e 7365 745f 736f 7572 6365 5f72 6f75  3.set_source_rou
+00002530: 7465 7228 5b27 6175 7468 6f72 275d 290a  ter(['author']).
+00002540: 2020 2020 2020 2020 6965 5f33 2e73 6574          ie_3.set
+00002550: 5f69 6d61 6765 5f72 6f75 7465 7228 5b27  _image_router(['
+00002560: 6d65 6469 613a 7468 756d 626e 6169 6c27  media:thumbnail'
+00002570: 2c20 2740 7572 6c27 5d29 0a20 2020 2020  , '@url']).     
+00002580: 2020 200a 2020 2020 2020 2020 2320 4375     .        # Cu
+00002590: 7374 6f6d 697a 6520 4944 2066 6f72 206e  stomize ID for n
+000025a0: 6577 7320 6974 656d 0a20 2020 2020 2020  ews item.       
+000025b0: 2064 6566 2069 645f 706f 6c69 6379 286c   def id_policy(l
+000025c0: 696e 6b29 3a0a 2020 2020 2020 2020 2020  ink):.          
+000025d0: 2020 7265 7475 726e 2068 6173 686c 6962    return hashlib
+000025e0: 2e6d 6435 286c 696e 6b2e 656e 636f 6465  .md5(link.encode
+000025f0: 2822 7574 662d 3822 2929 2e68 6578 6469  ("utf-8")).hexdi
+00002600: 6765 7374 2829 0a20 2020 2020 2020 2069  gest().        i
+00002610: 655f 332e 7365 745f 6964 5f70 6f6c 6963  e_3.set_id_polic
+00002620: 7928 6964 5f70 6f6c 6963 7929 0a20 2020  y(id_policy).   
+00002630: 2020 2020 200a 2020 2020 2020 2020 6e70       .        np
+00002640: 5f33 203d 204e 6577 7350 6f73 746d 616e  _3 = NewsPostman
+00002650: 4a53 4f4e 286c 6973 7455 524c 733d 5b75  JSON(listURLs=[u
+00002660: 726c 5f33 5d2c 2073 656e 644c 6973 743d  rl_3], sendList=
+00002670: 5b63 6861 6e6e 656c 5d2c 2064 623d 6462  [channel], db=db
+00002680: 2c20 7461 673d 7461 675f 3329 0a20 2020  , tag=tag_3).   
+00002690: 2020 2020 206e 705f 332e 7365 745f 6578       np_3.set_ex
+000026a0: 7472 6163 746f 7228 6965 5f33 290a 2020  tractor(ie_3).  
+000026b0: 2020 2020 2020 6e70 5f33 2e73 6574 5f74        np_3.set_t
+000026c0: 6162 6c65 5f6e 616d 6528 7461 626c 655f  able_name(table_
+000026d0: 6e61 6d65 5f33 290a 2020 2020 2020 2020  name_3).        
+000026e0: 6e70 5f33 2e70 6f6c 6c28 290a 2020 2020  np_3.poll().    
+000026f0: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+00002700: 0a20 2020 2020 2020 2054 7970 6963 616c  .        Typical
+00002710: 2072 6573 756c 7473 3a0a 2020 2020 2020   results:.      
+00002720: 2020 0a20 2020 2020 2020 203c 6469 7620    .        <div 
+00002730: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00002740: 2020 2020 2020 2020 2020 3c69 6d67 2073            <img s
+00002750: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002760: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002770: 742e 636f 6d2f 4553 575a 592f 7465 6c65  t.com/ESWZY/tele
+00002780: 6772 616d 2d6e 6577 732f 6d61 7374 6572  gram-news/master
+00002790: 2f64 6f63 732f 696d 6167 6573 2f64 656d  /docs/images/dem
+000027a0: 6f35 2e70 6e67 2220 616c 743d 2244 656d  o5.png" alt="Dem
+000027b0: 6f20 3522 2077 6964 7468 3d22 3430 2522  o 5" width="40%"
+000027c0: 3e0a 2020 2020 2020 2020 2020 3c69 6d67  >.          <img
+000027d0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+000027e0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+000027f0: 656e 742e 636f 6d2f 4553 575a 592f 7465  ent.com/ESWZY/te
+00002800: 6c65 6772 616d 2d6e 6577 732f 6d61 7374  legram-news/mast
+00002810: 6572 2f64 6f63 732f 696d 6167 6573 2f64  er/docs/images/d
+00002820: 656d 6f36 2e70 6e67 2220 616c 743d 2244  emo6.png" alt="D
+00002830: 656d 6f20 3622 2077 6964 7468 3d22 3430  emo 6" width="40
+00002840: 2522 3e0a 2020 2020 2020 2020 3c2f 6469  %">.        </di
+00002850: 763e 0a20 2020 2020 2020 200a 2020 2020  v>.        .    
+00002860: 2020 2020 2323 2320 5061 7261 6c6c 656c      ### Parallel
+00002870: 2050 726f 6772 616d 0a20 2020 2020 2020   Program.       
+00002880: 200a 2020 2020 2020 2020 4966 2079 6f75   .        If you
+00002890: 2075 7365 2074 6865 2073 616d 6520 6461   use the same da
+000028a0: 7461 6261 7365 2061 6e64 2073 656e 6420  tabase and send 
+000028b0: 746f 2074 6865 2073 616d 6520 6368 616e  to the same chan
+000028c0: 6e65 6c2c 2079 6f75 2063 616e 2073 696d  nel, you can sim
+000028d0: 706c 7920 6a6f 696e 7420 6561 6368 2070  ply joint each p
+000028e0: 6172 7420 6f66 2063 6f64 6520 626c 6f63  art of code bloc
+000028f0: 6b2c 2061 6e64 2063 616c 6c20 6070 6f6c  k, and call `pol
+00002900: 6c28 2960 2066 756e 6374 696f 6e20 7369  l()` function si
+00002910: 6d75 6c74 616e 656f 7573 6c79 2e0a 2020  multaneously..  
+00002920: 2020 2020 2020 0a20 2020 2020 2020 2041        .        A
+00002930: 6e20 6578 616d 706c 6520 796f 7520 6361  n example you ca
+00002940: 6e20 6669 6e64 2069 6e20 6f75 7220 4865  n find in our He
+00002950: 726f 6b75 2064 6570 6c6f 7920 7465 6d70  roku deploy temp
+00002960: 6c61 7465 2072 6570 6f3a 200a 2020 2020  late repo: .    
+00002970: 2020 2020 0a20 2020 2020 2020 2068 7474      .        htt
+00002980: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002990: 4553 575a 592f 7465 6c65 6772 616d 2d6e  ESWZY/telegram-n
+000029a0: 6577 732d 6765 7474 696e 672d 7374 6172  ews-getting-star
+000029b0: 7465 642f 626c 6f62 2f6d 6173 7465 722f  ted/blob/master/
+000029c0: 6d61 696e 2e70 790a 2020 2020 2020 2020  main.py.        
+000029d0: 0a20 2020 2020 2020 2023 2320 4578 616d  .        ## Exam
+000029e0: 706c 6520 4368 616e 6e65 6c0a 2020 2020  ple Channel.    
+000029f0: 2020 2020 0a20 2020 2020 2020 2041 2054      .        A T
+00002a00: 656c 6567 7261 6d20 6368 616e 6e65 6c20  elegram channel 
+00002a10: 6f66 205b 6261 7369 6320 6578 616d 706c  of [basic exampl
+00002a20: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00002a30: 622e 636f 6d2f 4553 575a 592f 7465 6c65  b.com/ESWZY/tele
+00002a40: 6772 616d 2d6e 6577 7323 6261 7369 632d  gram-news#basic-
+00002a50: 6578 616d 706c 6529 2066 6f72 2045 6e67  example) for Eng
+00002a60: 6c69 7368 2057 696b 696e 6577 733a 205b  lish Wikinews: [
+00002a70: 7e7e 4077 696b 696e 6577 735f 656e 7e7e  ~~@wikinews_en~~
+00002a80: 5d28 6874 7470 733a 2f2f 742e 6d65 2f6a  ](https://t.me/j
+00002a90: 6f69 6e63 6861 742f 5437 5462 4a55 5770  oinchat/T7TbJUWp
+00002aa0: 6755 7047 6d61 7259 2920 2869 6e20 456e  gUpGmarY) (in En
+00002ab0: 676c 6973 6829 0a20 2020 2020 2020 200a  glish).        .
+00002ac0: 2020 2020 2020 2020 4120 5465 6c65 6772          A Telegr
+00002ad0: 616d 2063 6861 6e6e 656c 2066 6f72 2072  am channel for r
+00002ae0: 6561 6c74 696d 6520 6561 7274 6871 7561  ealtime earthqua
+00002af0: 6b65 2077 6172 6e69 6e67 2070 6f77 6572  ke warning power
+00002b00: 6564 2062 7920 5465 6c65 6772 616d 2d6e  ed by Telegram-n
+00002b10: 6577 733a 205b 4065 6172 7468 7175 616b  ews: [@earthquak
+00002b20: 655f 616c 6572 745d 2868 7474 7073 3a2f  e_alert](https:/
+00002b30: 2f74 2e6d 652f 732f 6561 7274 6871 7561  /t.me/s/earthqua
+00002b40: 6b65 5f61 6c65 7274 2920 2869 6e20 4368  ke_alert) (in Ch
+00002b50: 696e 6573 6529 0a20 2020 2020 2020 200a  inese).        .
+00002b60: 2020 2020 2020 2020 2323 2054 4f44 4f0a          ## TODO.
+00002b70: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00002b80: 202d 205b 785d 2048 544d 4c20 6974 656d   - [x] HTML item
+00002b90: 206c 6973 740a 2020 2020 2020 2020 2d20   list.        - 
+00002ba0: 5b78 5d20 4a53 4f4e 2069 7465 6d20 6c69  [x] JSON item li
+00002bb0: 7374 0a20 2020 2020 2020 202d 205b 785d  st.        - [x]
+00002bc0: 2058 4d4c 2069 7465 6d20 6c69 7374 0a20   XML item list. 
+00002bd0: 2020 2020 2020 202d 205b 785d 2053 656e         - [x] Sen
+00002be0: 6420 496d 6167 650a 2020 2020 2020 2020  d Image.        
+00002bf0: 2d20 5b78 5d20 5365 6e64 2056 6964 656f  - [x] Send Video
+00002c00: 0a20 2020 2020 2020 202d 205b 785d 2053  .        - [x] S
+00002c10: 656e 6420 6d65 6469 6120 6772 6f75 700a  end media group.
+00002c20: 2020 2020 2020 2020 2d20 5b20 5d20 5365          - [ ] Se
+00002c30: 6e64 2066 696c 650a 2020 2020 2020 2020  nd file.        
+00002c40: 2d20 5b20 5d20 5365 6e64 2061 7564 696f  - [ ] Send audio
+00002c50: 0a20 2020 2020 2020 202d 205b 785d 2046  .        - [x] F
+00002c60: 696c 6520 7365 6e64 696e 6720 7265 7472  ile sending retr
+00002c70: 790a 2020 2020 2020 2020 2d20 5b20 5d20  y.        - [ ] 
+00002c80: 4343 2061 7320 652d 6d61 696c 0a20 2020  CC as e-mail.   
+00002c90: 2020 2020 202d 205b 205d 2057 6562 686f       - [ ] Webho
+00002ca0: 6f6b 0a20 2020 2020 2020 202d 205b 205d  ok.        - [ ]
+00002cb0: 2055 7064 6174 6520 6d65 7373 6167 6520   Update message 
+00002cc0: 6279 206d 6573 7361 6765 2049 440a 2020  by message ID.  
+00002cd0: 2020 2020 2020 2d20 5b20 5d20 446f 6375        - [ ] Docu
+00002ce0: 6d65 6e74 0a20 2020 2020 2020 202d 205b  ment.        - [
+00002cf0: 205d 2047 5549 0a20 2020 2020 2020 200a   ] GUI.        .
+00002d00: 2020 2020 2020 2020 2323 2046 6565 6462          ## Feedb
+00002d10: 6163 6b0a 2020 2020 2020 2020 0a20 2020  ack.        .   
+00002d20: 2020 2020 2046 6565 6c20 6672 6565 2074       Feel free t
+00002d30: 6f20 636f 6e74 6163 7420 7769 7468 206d  o contact with m
+00002d40: 6520 6966 2079 6f75 2068 6176 6520 616e  e if you have an
+00002d50: 7920 7175 6573 7469 6f6e 2e20 416c 736f  y question. Also
+00002d60: 2077 656c 636f 6d65 2061 6e79 2063 6f6e   welcome any con
+00002d70: 7472 6962 7574 652e 0a20 2020 2020 2020  tribute..       
+00002d80: 200a 2020 2020 2020 2020 4966 2079 6f75   .        If you
+00002d90: 2062 7569 6c64 2061 2063 6861 6e6e 656c   build a channel
+00002da0: 2062 7920 7468 6973 2c20 646f 6e27 7420   by this, don't 
+00002db0: 666f 7267 6574 2074 6f20 7368 6172 6520  forget to share 
+00002dc0: 7468 6174 2067 6f6f 6420 6e65 7773 2077  that good news w
+00002dd0: 6974 6820 7573 210a 2020 2020 2020 2020  ith us!.        
+00002de0: 0a20 2020 2020 2020 2023 2320 4c69 6365  .        ## Lice
+00002df0: 6e73 650a 2020 2020 2020 2020 0a20 2020  nse.        .   
+00002e00: 2020 2020 204c 6963 656e 7365 6420 756e       Licensed un
+00002e10: 6465 7220 7468 6520 4d49 5420 4c69 6365  der the MIT Lice
+00002e20: 6e73 652e 0a20 2020 2020 2020 200a 506c  nse..        .Pl
+00002e30: 6174 666f 726d 3a20 554e 4b4e 4f57 4e0a  atform: UNKNOWN.
+00002e40: 436c 6173 7369 6669 6572 3a20 4465 7665  Classifier: Deve
+00002e50: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
+00002e60: 3a20 3320 2d20 416c 7068 610a 436c 6173  : 3 - Alpha.Clas
+00002e70: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
+00002e80: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00002e90: 3a3a 204d 4954 204c 6963 656e 7365 0a43  :: MIT License.C
+00002ea0: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
+00002eb0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00002ec0: 5320 496e 6465 7065 6e64 656e 740a 436c  S Independent.Cl
+00002ed0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00002ee0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00002ef0: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
+00002f00: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00002f10: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00002f20: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00002f30: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00002f40: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00002f50: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00002f60: 2033 2e31 310a 436c 6173 7369 6669 6572   3.11.Classifier
+00002f70: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00002f80: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00002f90: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
+00002fa0: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+00002fb0: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00002fc0: 6572 730a 436c 6173 7369 6669 6572 3a20  ers.Classifier: 
+00002fd0: 546f 7069 6320 3a3a 2045 6475 6361 7469  Topic :: Educati
+00002fe0: 6f6e 0a43 6c61 7373 6966 6965 723a 2054  on.Classifier: T
+00002ff0: 6f70 6963 203a 3a20 4f66 6669 6365 2f42  opic :: Office/B
+00003000: 7573 696e 6573 7320 3a3a 204e 6577 732f  usiness :: News/
+00003010: 4469 6172 790a 436c 6173 7369 6669 6572  Diary.Classifier
+00003020: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
+00003030: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
+00003040: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
+00003050: 5079 7468 6f6e 204d 6f64 756c 6573 0a52  Python Modules.R
+00003060: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+00003070: 3e3d 332e 380a 4465 7363 7269 7074 696f  >=3.8.Descriptio
+00003080: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00003090: 7465 7874 2f6d 6172 6b64 6f77 6e0a       text/markdown.
```

