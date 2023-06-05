# Comparing `tmp/quicly-1.0.77.tar.gz` & `tmp/quicly-1.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quicly-1.0.77.tar", last modified: Thu Sep 30 07:36:54 2021, max compression
+gzip compressed data, was "quicly-1.0.78.tar", last modified: Mon Jun  5 02:37:23 2023, max compression
```

## Comparing `quicly-1.0.77.tar` & `quicly-1.0.78.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 mux        (501) staff       (20)        0 2021-09-30 07:36:54.663350 quicly-1.0.77/
--rw-r--r--   0 mux        (501) staff       (20)       64 2021-08-27 06:57:49.000000 quicly-1.0.77/MANIFEST.in
--rw-r--r--   0 mux        (501) staff       (20)      561 2021-09-30 07:36:54.663085 quicly-1.0.77/PKG-INFO
-drwxr-xr-x   0 mux        (501) staff       (20)        0 2021-09-30 07:36:54.659668 quicly-1.0.77/quicly/
--rw-rw-r--   0 mux        (501) staff       (20)        0 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/__init__.py
--rw-r--r--   0 mux        (501) staff       (20)     4318 2021-08-27 00:29:13.000000 quicly-1.0.77/quicly/apiclient.py
--rw-rw-r--   0 mux        (501) staff       (20)     1167 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/cache.py
-drwxr-xr-x   0 mux        (501) staff       (20)        0 2021-09-30 07:36:54.662005 quicly-1.0.77/quicly/conf/
--rw-rw-r--   0 mux        (501) staff       (20)      202 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/conf/code.json
--rw-r--r--   0 mux        (501) staff       (20)      204 2021-08-27 00:29:13.000000 quicly-1.0.77/quicly/conf/conf.json
-drwxr-xr-x   0 mux        (501) staff       (20)        0 2021-09-30 07:36:54.662533 quicly-1.0.77/quicly/conf/i18n/
--rw-rw-r--   0 mux        (501) staff       (20)      482 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/conf/i18n/zh-cn.json
--rw-r--r--   0 mux        (501) staff       (20)     3969 2021-08-27 00:29:13.000000 quicly-1.0.77/quicly/conf.py
--rw-rw-r--   0 mux        (501) staff       (20)     2492 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/decorator.py
--rw-rw-r--   0 mux        (501) staff       (20)     1072 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/hashutils.py
--rw-rw-r--   0 mux        (501) staff       (20)     1138 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/inspectutils.py
--rw-rw-r--   0 mux        (501) staff       (20)     4184 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/jsonutils.py
--rw-rw-r--   0 mux        (501) staff       (20)      499 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/limits.py
--rw-rw-r--   0 mux        (501) staff       (20)      540 2021-09-30 01:33:23.000000 quicly-1.0.77/quicly/logutils.py
--rw-rw-r--   0 mux        (501) staff       (20)     5215 2021-09-30 02:55:54.000000 quicly-1.0.77/quicly/mail.py
--rw-rw-r--   0 mux        (501) staff       (20)     6228 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/model.py
--rw-rw-r--   0 mux        (501) staff       (20)    21488 2021-08-26 09:23:50.000000 quicly-1.0.77/quicly/mongodb.py
--rw-rw-r--   0 mux        (501) staff       (20)     2837 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/patterns.py
--rw-rw-r--   0 mux        (501) staff       (20)     2923 2021-08-25 10:59:44.000000 quicly-1.0.77/quicly/plugin_flask_server.py
--rw-rw-r--   0 mux        (501) staff       (20)    13147 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/redisio.py
--rw-rw-r--   0 mux        (501) staff       (20)     5086 2021-08-25 10:57:03.000000 quicly-1.0.77/quicly/result.py
--rw-rw-r--   0 mux        (501) staff       (20)     1126 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/script.py
--rw-rw-r--   0 mux        (501) staff       (20)    33163 2021-08-27 07:16:58.000000 quicly-1.0.77/quicly/server.py
--rw-rw-r--   0 mux        (501) staff       (20)     4504 2021-08-26 06:49:09.000000 quicly-1.0.77/quicly/session.py
--rw-rw-r--   0 mux        (501) staff       (20)     6320 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/typingutils.py
--rw-rw-r--   0 mux        (501) staff       (20)     5665 2021-08-25 10:46:29.000000 quicly-1.0.77/quicly/urlutils.py
--rw-rw-r--   0 mux        (501) staff       (20)      622 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/uuidutils.py
--rw-rw-r--   0 mux        (501) staff       (20)    19088 2021-08-24 15:40:35.000000 quicly-1.0.77/quicly/value.py
-drwxr-xr-x   0 mux        (501) staff       (20)        0 2021-09-30 07:36:54.661180 quicly-1.0.77/quicly.egg-info/
--rw-r--r--   0 mux        (501) staff       (20)      561 2021-09-30 07:36:54.000000 quicly-1.0.77/quicly.egg-info/PKG-INFO
--rw-r--r--   0 mux        (501) staff       (20)      722 2021-09-30 07:36:54.000000 quicly-1.0.77/quicly.egg-info/SOURCES.txt
--rw-r--r--   0 mux        (501) staff       (20)        1 2021-09-30 07:36:54.000000 quicly-1.0.77/quicly.egg-info/dependency_links.txt
--rw-r--r--   0 mux        (501) staff       (20)       70 2021-09-30 07:36:54.000000 quicly-1.0.77/quicly.egg-info/requires.txt
--rw-r--r--   0 mux        (501) staff       (20)        7 2021-09-30 07:36:54.000000 quicly-1.0.77/quicly.egg-info/top_level.txt
--rw-rw-r--   0 mux        (501) staff       (20)       70 2021-08-27 06:41:38.000000 quicly-1.0.77/requirements.txt
--rw-r--r--   0 mux        (501) staff       (20)       38 2021-09-30 07:36:54.663430 quicly-1.0.77/setup.cfg
--rw-rw-r--   0 mux        (501) staff       (20)     2998 2021-08-27 06:50:27.000000 quicly-1.0.77/setup.py
--rw-rw-r--   0 mux        (501) staff       (20)       48 2021-08-24 15:40:35.000000 quicly-1.0.77/version.json
+drwxrwxrwx   0        0        0        0 2023-06-05 02:37:23.007965 quicly-1.0.78/
+-rw-rw-rw-   0        0        0       64 2023-06-05 02:34:23.000000 quicly-1.0.78/MANIFEST.in
+-rw-rw-rw-   0        0        0      720 2023-06-05 02:37:23.006965 quicly-1.0.78/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 02:37:22.996965 quicly-1.0.78/quicly/
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/__init__.py
+-rw-rw-rw-   0        0        0     4318 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/apiclient.py
+-rw-rw-rw-   0        0        0     1167 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/cache.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:37:23.004966 quicly-1.0.78/quicly/conf/
+-rw-rw-rw-   0        0        0      202 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/conf/code.json
+-rw-rw-rw-   0        0        0      190 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/conf/conf.json
+drwxrwxrwx   0        0        0        0 2023-06-05 02:37:23.005966 quicly-1.0.78/quicly/conf/i18n/
+-rw-rw-rw-   0        0        0      482 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/conf/i18n/zh-cn.json
+-rw-rw-rw-   0        0        0     3969 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/conf.py
+-rw-rw-rw-   0        0        0     2492 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/decorator.py
+-rw-rw-rw-   0        0        0     9024 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/dingtalk.py
+-rw-rw-rw-   0        0        0     1072 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/hashutils.py
+-rw-rw-rw-   0        0        0     1138 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/inspectutils.py
+-rw-rw-rw-   0        0        0     4184 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/jsonutils.py
+-rw-rw-rw-   0        0        0      499 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/limits.py
+-rw-rw-rw-   0        0        0      540 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/logutils.py
+-rw-rw-rw-   0        0        0     5215 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/mail.py
+-rw-rw-rw-   0        0        0     6228 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/model.py
+-rw-rw-rw-   0        0        0    21488 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/mongodb.py
+-rw-rw-rw-   0        0        0     2837 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/patterns.py
+-rw-rw-rw-   0        0        0     2923 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/plugin_flask_server.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/qyweixin.py
+-rw-rw-rw-   0        0        0    13147 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/redisio.py
+-rw-rw-rw-   0        0        0     5086 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/result.py
+-rw-rw-rw-   0        0        0     1126 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/script.py
+-rw-rw-rw-   0        0        0    33163 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/server.py
+-rw-rw-rw-   0        0        0     4504 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/session.py
+-rw-rw-rw-   0        0        0     6320 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/typingutils.py
+-rw-rw-rw-   0        0        0     5665 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/urlutils.py
+-rw-rw-rw-   0        0        0      622 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/uuidutils.py
+-rw-rw-rw-   0        0        0    19088 2023-06-05 02:34:23.000000 quicly-1.0.78/quicly/value.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:37:23.002965 quicly-1.0.78/quicly.egg-info/
+-rw-rw-rw-   0        0        0      720 2023-06-05 02:37:22.000000 quicly-1.0.78/quicly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2023-06-05 02:37:22.000000 quicly-1.0.78/quicly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 02:37:22.000000 quicly-1.0.78/quicly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-05 02:37:22.000000 quicly-1.0.78/quicly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 02:37:22.000000 quicly-1.0.78/quicly.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-06-05 02:34:23.000000 quicly-1.0.78/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 02:37:23.007965 quicly-1.0.78/setup.cfg
+-rw-rw-rw-   0        0        0     3192 2023-06-05 02:35:59.000000 quicly-1.0.78/setup.py
+-rw-rw-rw-   0        0        0       48 2023-06-05 02:34:23.000000 quicly-1.0.78/version.json
```

### Comparing `quicly-1.0.77/PKG-INFO` & `quicly-1.0.78/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-Metadata-Version: 2.1
-Name: quicly
-Version: 1.0.77
-Summary: UNKNOWN
-Home-page: https://gitee.com/muxiaofei/quicly
-Author: muxiaofei
-Author-email: muxiaofei@gmail.com
-License: UNKNOWN
-Keywords: quicly
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/x-rst
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: quicly
+Version: 1.0.78
+Home-page: https://gitee.com/muxiaofei/quicly
+Author: muxiaofei
+Author-email: muxiaofei@gmail.com
+Keywords: quicly
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/x-rst
```

### Comparing `quicly-1.0.77/quicly/apiclient.py` & `quicly-1.0.78/quicly/apiclient.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/cache.py` & `quicly-1.0.78/quicly/cache.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/conf.py` & `quicly-1.0.78/quicly/conf.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/decorator.py` & `quicly-1.0.78/quicly/decorator.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/hashutils.py` & `quicly-1.0.78/quicly/hashutils.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/inspectutils.py` & `quicly-1.0.78/quicly/inspectutils.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/jsonutils.py` & `quicly-1.0.78/quicly/jsonutils.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/logutils.py` & `quicly-1.0.78/quicly/logutils.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/mail.py` & `quicly-1.0.78/quicly/mail.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/model.py` & `quicly-1.0.78/quicly/model.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/mongodb.py` & `quicly-1.0.78/quicly/mongodb.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/patterns.py` & `quicly-1.0.78/quicly/patterns.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/plugin_flask_server.py` & `quicly-1.0.78/quicly/plugin_flask_server.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/redisio.py` & `quicly-1.0.78/quicly/redisio.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/result.py` & `quicly-1.0.78/quicly/result.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/script.py` & `quicly-1.0.78/quicly/script.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/server.py` & `quicly-1.0.78/quicly/server.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/session.py` & `quicly-1.0.78/quicly/session.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/typingutils.py` & `quicly-1.0.78/quicly/typingutils.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/urlutils.py` & `quicly-1.0.78/quicly/urlutils.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/uuidutils.py` & `quicly-1.0.78/quicly/uuidutils.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly/value.py` & `quicly-1.0.78/quicly/value.py`

 * *Files identical despite different names*

### Comparing `quicly-1.0.77/quicly.egg-info/PKG-INFO` & `quicly-1.0.78/quicly.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-Metadata-Version: 2.1
-Name: quicly
-Version: 1.0.77
-Summary: UNKNOWN
-Home-page: https://gitee.com/muxiaofei/quicly
-Author: muxiaofei
-Author-email: muxiaofei@gmail.com
-License: UNKNOWN
-Keywords: quicly
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/x-rst
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: quicly
+Version: 1.0.78
+Home-page: https://gitee.com/muxiaofei/quicly
+Author: muxiaofei
+Author-email: muxiaofei@gmail.com
+Keywords: quicly
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/x-rst
```

### Comparing `quicly-1.0.77/quicly.egg-info/SOURCES.txt` & `quicly-1.0.78/quicly.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 setup.py
 version.json
 quicly/__init__.py
 quicly/apiclient.py
 quicly/cache.py
 quicly/conf.py
 quicly/decorator.py
+quicly/dingtalk.py
 quicly/hashutils.py
 quicly/inspectutils.py
 quicly/jsonutils.py
 quicly/limits.py
 quicly/logutils.py
 quicly/mail.py
 quicly/model.py
 quicly/mongodb.py
 quicly/patterns.py
 quicly/plugin_flask_server.py
+quicly/qyweixin.py
 quicly/redisio.py
 quicly/result.py
 quicly/script.py
 quicly/server.py
 quicly/session.py
 quicly/typingutils.py
 quicly/urlutils.py
```

### Comparing `quicly-1.0.77/setup.py` & `quicly-1.0.78/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import requests
 import re
 import sys
 import json
 import setuptools
 
 
 root = os.path.dirname(os.path.abspath(__file__))
@@ -25,14 +24,16 @@
 
         info[k] = v
 
   return info
 
 
 def getver(name, major=None, minor=None, patch=None):
+  import requests
+
   pattern = '{} {}'.format(name, '\\.'.join([f'({x})' if isinstance(x, int) else '(\\d+)' for x in (major, minor, patch)]))
 
   res = requests.get(f'https://pypi.org/project/{name}/')
   items = re.findall(pattern, res.content.decode())
   if not items:
     major = major if isinstance(major, int) else 0
     minor = minor if isinstance(minor, int) else 0
@@ -94,17 +95,21 @@
     description="",
     long_description="",
     long_description_content_type="text/x-rst",
     url=url,
     packages=setuptools.find_packages(),
     classifiers=[
       "Programming Language :: Python :: 3",
+      "Programming Language :: Python :: 3.6",
       "Programming Language :: Python :: 3.7",
       "Programming Language :: Python :: 3.8",
       "Programming Language :: Python :: 3.9",
+      "Programming Language :: Python :: 3.10",
+      "Programming Language :: Python :: 3.11",
+      "Programming Language :: Python :: 3.12",
       "License :: OSI Approved :: MIT License",
       "Operating System :: OS Independent",
     ],
     install_requires=requirements,
   )
```

