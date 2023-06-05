# Comparing `tmp/alibabacloud_resourcemanager20200331-2.1.4.tar.gz` & `tmp/alibabacloud_resourcemanager20200331-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcemanager20200331-2.1.4.tar", last modified: Thu May 18 08:59:18 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcemanager20200331-2.1.5.tar", last modified: Mon Jun  5 05:47:02 2023, max compression
```

## Comparing `alibabacloud_resourcemanager20200331-2.1.4.tar` & `alibabacloud_resourcemanager20200331-2.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/
--rw-r--r--   0 root         (0) root         (0)      887 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2400 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/__init__.py
--rw-r--r--   0 root         (0) root         (0)   388878 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/client.py
--rw-r--r--   0 root         (0) root         (0)   589797 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2400 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2670 2023-05-18 08:59:18.000000 alibabacloud_resourcemanager20200331-2.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:47:02.000000 alibabacloud_resourcemanager20200331-2.1.5/
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-06-05 05:47:02.000000 alibabacloud_resourcemanager20200331-2.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:47:02.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   387119 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/client.py
+-rw-r--r--   0 root         (0) root         (0)   589797 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:47:02.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 05:47:02.000000 alibabacloud_resourcemanager20200331-2.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/setup.py
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.4/ChangeLog.md` & `alibabacloud_resourcemanager20200331-2.1.5/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-18 Version: 2.1.4
+- Supported more language for resourcemanager.
+
 2023-02-22 Version: 2.1.3
 - Supported more language for resourcemanager.
 
 2022-12-01 Version: 2.1.2
 - Supported more language for resourcemanager.
 
 2022-08-03 Version: 2.1.1
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.4/LICENSE` & `alibabacloud_resourcemanager20200331-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.4/PKG-INFO` & `alibabacloud_resourcemanager20200331-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcemanager20200331
-Version: 2.1.4
+Version: 2.1.5
 Summary: Alibaba Cloud ResourceManager (20200331) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.4/README-CN.md` & `alibabacloud_resourcemanager20200331-2.1.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.4/README.md` & `alibabacloud_resourcemanager20200331-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/client.py` & `alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/client.py`

 * *Files 0% similar despite different names*

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

### Comparing `alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331/models.py` & `alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO` & `alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcemanager20200331
-Version: 2.1.4
+Version: 2.1.5
 Summary: Alibaba Cloud ResourceManager (20200331) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.4/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt` & `alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.4/setup.py` & `alibabacloud_resourcemanager20200331-2.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcemanager20200331.
 
-Created on 18/05/2023
+Created on 05/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcemanager20200331"
 NAME = "alibabacloud_resourcemanager20200331" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceManager (20200331) SDK Library for Python"
```

