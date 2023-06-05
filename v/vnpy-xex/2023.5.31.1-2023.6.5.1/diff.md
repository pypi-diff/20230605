# Comparing `tmp/vnpy_xex-2023.5.31.1.tar.gz` & `tmp/vnpy_xex-2023.6.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_xex-2023.5.31.1.tar", last modified: Wed May 31 01:36:22 2023, max compression
+gzip compressed data, was "vnpy_xex-2023.6.5.1.tar", last modified: Mon Jun  5 10:03:45 2023, max compression
```

## Comparing `vnpy_xex-2023.5.31.1.tar` & `vnpy_xex-2023.6.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-05-31 01:36:22.562964 vnpy_xex-2023.5.31.1/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.5.31.1/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1008 2023-05-31 01:36:22.563068 vnpy_xex-2023.5.31.1/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.5.31.1/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      994 2023-05-31 01:36:22.563659 vnpy_xex-2023.5.31.1/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.5.31.1/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-05-31 01:36:22.559061 vnpy_xex-2023.5.31.1/vnpy_xex/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.5.31.1/vnpy_xex/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    23922 2023-05-30 10:05:30.000000 vnpy_xex-2023.5.31.1/vnpy_xex/xex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-05-31 01:36:22.562760 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1008 2023-05-31 01:36:22.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-05-31 01:36:22.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-31 01:36:22.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-05-31 01:36:22.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-05-31 01:36:22.000000 vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-05 10:03:45.676872 vnpy_xex-2023.6.5.1/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.5.1/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-05 10:03:45.676976 vnpy_xex-2023.6.5.1/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.5.1/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      994 2023-06-05 10:03:45.677477 vnpy_xex-2023.6.5.1/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.5.1/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-05 10:03:45.673759 vnpy_xex-2023.6.5.1/vnpy_xex/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.5.1/vnpy_xex/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    23960 2023-06-05 10:02:35.000000 vnpy_xex-2023.6.5.1/vnpy_xex/xex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-05 10:03:45.676659 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-05 10:03:45.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-05 10:03:45.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-05 10:03:45.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-05 10:03:45.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-05 10:03:45.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/top_level.txt
```

### Comparing `vnpy_xex-2023.5.31.1/LICENSE` & `vnpy_xex-2023.6.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.5.31.1/PKG-INFO` & `vnpy_xex-2023.6.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_xex
-Version: 2023.5.31.1
+Version: 2023.6.5.1
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_xex-2023.5.31.1/setup.cfg` & `vnpy_xex-2023.6.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_xex
-version = 2023.5.31.1
+version = 2023.6.05.1
 url = https://github.com/monk-after-90s/vnpy_xex
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = gateway of xex exchange for vnpy
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_xex-2023.5.31.1/vnpy_xex/__init__.py` & `vnpy_xex-2023.6.5.1/vnpy_xex/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.5.31.1/vnpy_xex/xex_gateway.py` & `vnpy_xex-2023.6.5.1/vnpy_xex/xex_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import hashlib
 import hmac
 import json
 import time
-import urllib
 from asyncio import run_coroutine_threadsafe
 from copy import copy
 from datetime import datetime, timedelta
 from enum import Enum
 from threading import Lock
 from vnpy_websocket import WebsocketClient
 import pytz
@@ -346,14 +345,15 @@
             orderid: str = str(self.connect_time + self._new_order_id())
 
             # 推送提交中事件
             order: OrderData = req.create_order_data(
                 orderid,
                 self.gateway_name
             )
+            order.datetime = datetime.now(CHINA_TZ)
             self.gateway.on_order(order)
             order_params.append({"isCreate": True,
                                  "symbol": req.symbol,
                                  "price": req.price,
                                  "totalAmount": format(req.volume, ".5f"),
                                  "tradeType": ORDERTYPE_VT2XEX[req.type],
                                  "direction": DIRECTION_VT2XEX[req.direction],
```

### Comparing `vnpy_xex-2023.5.31.1/vnpy_xex.egg-info/PKG-INFO` & `vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-xex
-Version: 2023.5.31.1
+Version: 2023.6.5.1
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

