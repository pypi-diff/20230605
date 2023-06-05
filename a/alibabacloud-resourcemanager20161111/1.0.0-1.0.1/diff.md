# Comparing `tmp/alibabacloud_resourcemanager20161111-1.0.0.tar.gz` & `tmp/alibabacloud_resourcemanager20161111-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcemanager20161111-1.0.0.tar", last modified: Wed Aug  3 06:28:50 2022, max compression
+gzip compressed data, was "dist/alibabacloud_resourcemanager20161111-1.0.1.tar", last modified: Mon Jun  5 10:44:48 2023, max compression
```

## Comparing `alibabacloud_resourcemanager20161111-1.0.0.tar` & `alibabacloud_resourcemanager20161111-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2400 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1058 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111/
--rw-r--r--   0 root         (0) root         (0)       21 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   168434 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111/client.py
--rw-r--r--   0 root         (0) root         (0)   298591 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2400 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      503 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2670 2022-08-03 06:28:50.000000 alibabacloud_resourcemanager20161111-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   166675 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111/client.py
+-rw-r--r--   0 root         (0) root         (0)   298591 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-05 10:44:48.000000 alibabacloud_resourcemanager20161111-1.0.1/setup.py
```

### Comparing `alibabacloud_resourcemanager20161111-1.0.0/LICENSE` & `alibabacloud_resourcemanager20161111-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20161111-1.0.0/PKG-INFO` & `alibabacloud_resourcemanager20161111-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcemanager20161111
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ResourceManager (20161111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20161111-1.0.0/README-CN.md` & `alibabacloud_resourcemanager20161111-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20161111-1.0.0/README.md` & `alibabacloud_resourcemanager20161111-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111/client.py` & `alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,39 +18,14 @@
     """
     def __init__(
         self, 
         config: open_api_models.Config,
     ):
         super().__init__(config)
         self._endpoint_rule = 'central'
-        self._endpoint_map = {
-            'ap-northeast-1': 'resourcemanager.ap-northeast-1.aliyuncs.com',
-            'ap-south-1': 'resourcemanager.ap-south-1.aliyuncs.com',
-            'ap-southeast-1': 'resourcemanager.ap-southeast-1.aliyuncs.com',
-            'ap-southeast-2': 'resourcemanager.ap-southeast-2.aliyuncs.com',
-            'ap-southeast-3': 'resourcemanager.ap-southeast-3.aliyuncs.com',
-            'ap-southeast-5': 'resourcemanager.ap-southeast-5.aliyuncs.com',
-            'cn-beijing': 'resourcemanager.cn-beijing.aliyuncs.com',
-            'cn-chengdu': 'resourcemanager.cn-chengdu.aliyuncs.com',
-            'cn-hangzhou-finance': 'resourcemanager.cn-hangzhou-finance.aliyuncs.com',
-            'cn-hongkong': 'resourcemanager.cn-hongkong.aliyuncs.com',
-            'cn-huhehaote': 'resourcemanager.cn-huhehaote.aliyuncs.com',
-            'cn-north-2-gov-1': 'resourcemanager.cn-north-2-gov-1.aliyuncs.com',
-            'cn-qingdao': 'resourcemanager.cn-qingdao.aliyuncs.com',
-            'cn-shanghai-finance-1': 'resourcemanager.cn-shanghai-finance-1.aliyuncs.com',
-            'cn-shenzhen': 'resourcemanager.cn-shenzhen.aliyuncs.com',
-            'cn-shenzhen-finance-1': 'resourcemanager.cn-shenzhen-finance-1.aliyuncs.com',
-            'cn-wulanchabu': 'resourcemanager.cn-wulanchabu.aliyuncs.com',
-            'cn-zhangjiakou': 'resourcemanager.cn-zhangjiakou.aliyuncs.com',
-            'eu-central-1': 'resourcemanager.eu-central-1.aliyuncs.com',
-            'eu-west-1': 'resourcemanager.eu-west-1.aliyuncs.com',
-            'me-east-1': 'resourcemanager.me-east-1.aliyuncs.com',
-            'us-east-1': 'resourcemanager.us-east-1.aliyuncs.com',
-            'us-west-1': 'resourcemanager.us-west-1.aliyuncs.com'
-        }
         self.check_config(config)
         self._endpoint = self.get_endpoint('resourcemanager', self._region_id, self._endpoint_rule, self._network, self._suffix, self._endpoint_map, self._endpoint)
 
     def get_endpoint(
         self,
         product_id: str,
         region_id: str,
```

### Comparing `alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111/models.py` & `alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20161111-1.0.0/alibabacloud_resourcemanager20161111.egg-info/PKG-INFO` & `alibabacloud_resourcemanager20161111-1.0.1/alibabacloud_resourcemanager20161111.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcemanager20161111
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ResourceManager (20161111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20161111-1.0.0/setup.py` & `alibabacloud_resourcemanager20161111-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcemanager20161111.
 
-Created on 03/08/2022
+Created on 05/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcemanager20161111"
 NAME = "alibabacloud_resourcemanager20161111" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceManager (20161111) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

