# Comparing `tmp/pytip-0.1.4-py2.py3-none-any.whl.zip` & `tmp/pytip-0.1.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 18208 bytes, number of entries: 17
--rw-rw-r--  2.0 unx      718 b- defN 23-May-10 01:34 pytip/__init__.py
+Zip file size: 19043 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jun-05 07:28 pytip/__init__.py
 -rw-rw-r--  2.0 unx    42686 b- defN 23-Apr-16 06:56 pytip/data/browsers.json
--rw-rw-r--  2.0 unx      389 b- defN 23-Apr-09 02:24 pytip/tools/__init__.py
--rw-rw-r--  2.0 unx     3639 b- defN 23-May-17 03:48 pytip/tools/item.py
--rw-rw-r--  2.0 unx      854 b- defN 23-Apr-09 01:59 pytip/tools/plot.py
+-rw-rw-r--  2.0 unx      389 b- defN 23-Jun-05 07:16 pytip/tools/__init__.py
+-rw-rw-r--  2.0 unx     3911 b- defN 23-Jun-05 13:26 pytip/tools/item.py
+-rw-rw-r--  2.0 unx      854 b- defN 23-Jun-05 06:53 pytip/tools/plot.py
+-rw-rw-r--  2.0 unx      795 b- defN 23-Jun-05 07:38 pytip/tools/sheet.py
 -rw-rw-r--  2.0 unx     1597 b- defN 23-Apr-09 10:43 pytip/tools/table.py
 -rw-rw-r--  2.0 unx      423 b- defN 23-Apr-16 02:29 pytip/utils/__init__.py
 -rw-rw-r--  2.0 unx     3860 b- defN 23-May-17 02:15 pytip/utils/celery.py
 -rw-rw-r--  2.0 unx     2268 b- defN 23-May-17 02:15 pytip/utils/checker.py
--rw-rw-r--  2.0 unx     1291 b- defN 23-May-17 02:15 pytip/utils/deco.py
--rw-rw-r--  2.0 unx     2983 b- defN 23-Apr-16 07:13 pytip/utils/file.py
+-rw-rw-r--  2.0 unx     1291 b- defN 23-Jun-05 06:52 pytip/utils/deco.py
+-rw-rw-r--  2.0 unx     3269 b- defN 23-Jun-05 07:45 pytip/utils/file.py
 -rw-rw-r--  2.0 unx     1255 b- defN 23-May-17 02:15 pytip/utils/func.py
 -rw-rw-r--  2.0 unx     1823 b- defN 23-Apr-16 08:49 pytip/utils/web.py
--rw-rw-r--  2.0 unx     1081 b- defN 23-May-17 03:49 pytip-0.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-17 03:49 pytip-0.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-May-17 03:49 pytip-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1291 b- defN 23-May-17 03:49 pytip-0.1.4.dist-info/RECORD
-17 files, 66274 bytes uncompressed, 16128 bytes compressed:  75.7%
+-rw-rw-r--  2.0 unx     1152 b- defN 23-Jun-05 13:27 pytip-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-05 13:27 pytip-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jun-05 13:27 pytip-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1367 b- defN 23-Jun-05 13:27 pytip-0.1.5.dist-info/RECORD
+18 files, 67815 bytes uncompressed, 16847 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: pytip/tools/item.py
 Comment: 
 
 Filename: pytip/tools/plot.py
 Comment: 
 
+Filename: pytip/tools/sheet.py
+Comment: 
+
 Filename: pytip/tools/table.py
 Comment: 
 
 Filename: pytip/utils/__init__.py
 Comment: 
 
 Filename: pytip/utils/celery.py
@@ -33,20 +36,20 @@
 
 Filename: pytip/utils/func.py
 Comment: 
 
 Filename: pytip/utils/web.py
 Comment: 
 
-Filename: pytip-0.1.4.dist-info/METADATA
+Filename: pytip-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pytip-0.1.4.dist-info/WHEEL
+Filename: pytip-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pytip-0.1.4.dist-info/top_level.txt
+Filename: pytip-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pytip-0.1.4.dist-info/RECORD
+Filename: pytip-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytip/__init__.py

```diff
@@ -7,17 +7,17 @@
 
 from .utils.celery import Celery
 from .utils.checker import Message, check_folder_file, check_ip
 from .utils.deco import web_retries, elapsed_time
 from .utils.web import FakeAgent
 from .utils.func import progressBar
 from .utils.file import (
-    multiprocess_items, file_download, file_pickle, print_error
+    file_list, multiprocess_items, file_download, file_pickle, print_error
 )
 
 from .tools.plot import plt_ko
 from .tools.table import df_number_column
 from .tools.item import (
     date_to_string, string_to_datetime, divide_chunks,
     password
 )
-
+from .tools.sheet import Excel
```

## pytip/tools/item.py

```diff
@@ -1,10 +1,11 @@
 import re
 import string
 import random
+import pandas
 import datetime
 import itertools
 
 
 REGEX_DATETIME = {
     '[\d]{4}-[\d]{2}-[\d]{2}.[A-Z]{2}[\d]{1,2}:[\d]{1,2}:[\d]{1,2}':
     '%Y-%m-%d.%p%I:%M:%S', # '2022-07-31.AM3:02:30'
@@ -32,14 +33,16 @@
     _return = None
     if date is None:
         _return = datetime.date.today().isoformat()
     elif type(date) == datetime.date:
         _return = date.isoformat()
     elif type(date) == datetime.datetime:
         _return = date.date().isoformat()
+    elif type(date) == pandas._libs.tslibs.timestamps.Timestamp:
+        _return = date.to_pydatetime()
     elif type(date) == str:
         _check = "".join(re.findall(r'[\d]{8}', date))
         _check_re = re.findall('[,-//.]', date)
         if len(_check) == 8:
             _return = f"{_check[:4]}-{_check[4:6]}-{_check[6:]}"
 
         elif len(_check_re) > 0:
@@ -94,12 +97,16 @@
     
     elif type(items) == dict:
         for i in range(0, len(items), n):
             yield dict(itertools.islice(items.items(), i ,i+n))
 
 
 # 문자 난수생성 (비밀번호 생성기)
-def password(length:int=12) -> str:
+def password(length:int=12, not_punct=False) -> str:
     r"""난수문자 생성기 (ex> 비밀번호)
-    length : 생성문자 길이"""
-    letters = string.ascii_letters + string.digits + "!#$%&*+-?@" # string.punctuation
+    length    : 생성문자 길이
+    not_punct : 특수문자 비포함"""
+    if not_punct == True:
+        letters = string.ascii_letters + string.digits
+    else:
+        letters = string.ascii_letters + string.digits + "!#$%&*+-?@" # string.punctuation
     return "".join([random.choice(letters)  for _ in range(length)])
```

## pytip/utils/file.py

```diff
@@ -1,8 +1,9 @@
 import os
+import glob
 import json
 import socket
 import subprocess
 from urllib import request
 import pickle
 import requests
 import termcolor
@@ -20,14 +21,24 @@
         if display:
             items = list(tqdm(pool.imap(funcion, items), total=len(items)))
         else:
             items = pool.map(funcion, items)
         return items
 
 
+def file_list(folder:str=None, filter:str=None) -> list:
+    r"""폴더내 목록 가져오기
+    folder : /home/user
+    filter : 이름필터 """
+    files = glob.glob(folder)
+    if filter:
+        files = [_  for _ in files  if _.find(filter) != -1]
+    return files
+
+
 # http://taewan.kim/tip/python_pickle/
 def file_pickle(
         file_path:str=None,
         option='w', 
         data=None
     ):
     r"""파이썬 객체를 Pickle 로 저장하고 호출
```

## Comparing `pytip-0.1.4.dist-info/METADATA` & `pytip-0.1.5.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytip
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/YongBeomKim/pytip
 Author: momukji lab
 Author-email: ybkim@momukji.com
 License: MIT
 Keywords: pytip
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,14 +20,18 @@
 
 # Python Useful Tip & Tools
 
 [![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](LICENSE)
 [![Docs](https://img.shields.io/badge/docs-stable-blue.svg)](https://domschl.github.io/ml-indie-tools/index.html)
 [![PyPI version fury.io](https://badge.fury.io/py/ml-indie-tools.svg)](https://pypi.python.org/pypi/ml-indie-tools/)
 
+
+## Version
+0.1.5 - Excel worksheet loading, datatime add pandas data
+
 ## Installation
 Based on : https://github.com/YongBeomKim/pytip
 ```bash
 	$ pip install pytip
 	$ pip install -i https://pypi.python.org/pytip pytip
 ```
```

## Comparing `pytip-0.1.4.dist-info/RECORD` & `pytip-0.1.5.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-pytip/__init__.py,sha256=j1C6VrbrG1sGnNR4jZ7d6YZjEF2UkaoLKg3JmNN3hcg,718
+pytip/__init__.py,sha256=ND8y5VE5m721jT6qUMKshbGt9JbY_pBW_csxtAhV6Tc,759
 pytip/data/browsers.json,sha256=fgvByElwtpg9QpigM0ss-Rpjnc_Uql4-3y0gJDB7dVI,42686
 pytip/tools/__init__.py,sha256=KKqbkgk5EkEh_2jwQdxUtXATP6peuk43t9zGBN0lQE8,389
-pytip/tools/item.py,sha256=-O0Q6QaifZdatGtfQaWeJ54K_6ADDzgNDY26A09Ihjo,3639
+pytip/tools/item.py,sha256=5KR19hbhf33Sa8dS1Xh0rWdnpH9-0rWCnJm3ltU1ScQ,3911
 pytip/tools/plot.py,sha256=2pmcMkz5HZ5fD5A5OgPr1_Cs2nTZP1DMcuqSyiSMCZk,854
+pytip/tools/sheet.py,sha256=NVooBA0SERLuBEMpRDbKqAFxyfLOwp1r01CNYlRFDgQ,795
 pytip/tools/table.py,sha256=ddAvODKP7SExPgeEBmeW4QCcZXkDi-aaM3saxqw6vDo,1597
 pytip/utils/__init__.py,sha256=ptGGMFwDewyV4fCaRR3BSwZIGAlug5Z_8xs-scpEDYk,423
 pytip/utils/celery.py,sha256=rPXP3aAxIwkZBpjczcHELJegjMKbrmIUnpZulRdVcpE,3860
 pytip/utils/checker.py,sha256=VR08MkfhL_rhBll-92c1Xo28yaf4tWRfyBJUQlx2axU,2268
 pytip/utils/deco.py,sha256=BmidVhyoZbLKuziGamyA1TSOBGaU2xZy-ijUn6cAJ3g,1291
-pytip/utils/file.py,sha256=vFbfmPdM7-Fr-8SiJoQWeeu-4LTxCMjgYk4ftauMPBY,2983
+pytip/utils/file.py,sha256=X0JxWdMoMJ_-po7GynNSs7ndYsqD6-fg4_0mZWxLxAQ,3269
 pytip/utils/func.py,sha256=fR_GQcYHMtYb0OC98zQ0i9AMVZqGgS3LJUoJZmjuWI0,1255
 pytip/utils/web.py,sha256=lyR6e7iyDIsSCPovTMmbSm8zu1AHEBEk35adIxYklZo,1823
-pytip-0.1.4.dist-info/METADATA,sha256=qlNME_KV-1OLcLyrluZl9P9QzMqHQYhVG8ObMbhjmmM,1081
-pytip-0.1.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-pytip-0.1.4.dist-info/top_level.txt,sha256=jF2tKdrfqmRq7kr--QAKzT5DpQOqrfwdSBO9WrauNHE,6
-pytip-0.1.4.dist-info/RECORD,,
+pytip-0.1.5.dist-info/METADATA,sha256=_p5e9ZYpheytRZZzPuM9nzk6W4VHW9MjMGaIPgJb_Rk,1152
+pytip-0.1.5.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+pytip-0.1.5.dist-info/top_level.txt,sha256=jF2tKdrfqmRq7kr--QAKzT5DpQOqrfwdSBO9WrauNHE,6
+pytip-0.1.5.dist-info/RECORD,,
```

