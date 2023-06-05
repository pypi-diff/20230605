# Comparing `tmp/alibabacloud_appstream-center20210218-1.0.1.tar.gz` & `tmp/alibabacloud_appstream-center20210218-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_appstream-center20210218-1.0.1.tar", last modified: Wed Dec 14 10:34:07 2022, max compression
+gzip compressed data, was "dist/alibabacloud_appstream-center20210218-1.0.4.tar", last modified: Mon Jun  5 03:37:28 2023, max compression
```

## Comparing `alibabacloud_appstream-center20210218-1.0.1.tar` & `alibabacloud_appstream-center20210218-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 10:34:07.000000 alibabacloud_appstream-center20210218-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       39 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2406 2022-12-14 10:34:07.000000 alibabacloud_appstream-center20210218-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1061 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1146 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 10:34:07.000000 alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4618 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218/client.py
--rw-r--r--   0 root         (0) root         (0)     4789 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 10:34:07.000000 alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2406 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      524 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-14 10:34:07.000000 alibabacloud_appstream-center20210218-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2677 2022-12-14 10:34:06.000000 alibabacloud_appstream-center20210218-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8220 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218/client.py
+-rw-r--r--   0 root         (0) root         (0)     8498 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-06-05 03:37:28.000000 alibabacloud_appstream-center20210218-1.0.4/setup.py
```

### Comparing `alibabacloud_appstream-center20210218-1.0.1/LICENSE` & `alibabacloud_appstream-center20210218-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210218-1.0.1/PKG-INFO` & `alibabacloud_appstream-center20210218-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_appstream-center20210218
-Version: 1.0.1
+Version: 1.0.4
 Summary: Alibaba Cloud appstream-center (20210218) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_appstream-center20210218-1.0.1/README-CN.md` & `alibabacloud_appstream-center20210218-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210218-1.0.1/README.md` & `alibabacloud_appstream-center20210218-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218/models.py` & `alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,165 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict
 
 
+class ExpireLoginTokenRequest(TeaModel):
+    def __init__(
+        self,
+        end_user_id: str = None,
+        login_token: str = None,
+        office_site_id: str = None,
+        session_id: str = None,
+    ):
+        self.end_user_id = end_user_id
+        self.login_token = login_token
+        self.office_site_id = office_site_id
+        self.session_id = session_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_user_id is not None:
+            result['EndUserId'] = self.end_user_id
+        if self.login_token is not None:
+            result['LoginToken'] = self.login_token
+        if self.office_site_id is not None:
+            result['OfficeSiteId'] = self.office_site_id
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndUserId') is not None:
+            self.end_user_id = m.get('EndUserId')
+        if m.get('LoginToken') is not None:
+            self.login_token = m.get('LoginToken')
+        if m.get('OfficeSiteId') is not None:
+            self.office_site_id = m.get('OfficeSiteId')
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        return self
+
+
+class ExpireLoginTokenResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ExpireLoginTokenResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ExpireLoginTokenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ExpireLoginTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetAuthCodeRequest(TeaModel):
     def __init__(
         self,
+        auto_create_user: bool = None,
         end_user_id: str = None,
         external_user_id: str = None,
         policy: str = None,
     ):
+        self.auto_create_user = auto_create_user
         self.end_user_id = end_user_id
         self.external_user_id = external_user_id
         self.policy = policy
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.auto_create_user is not None:
+            result['AutoCreateUser'] = self.auto_create_user
         if self.end_user_id is not None:
             result['EndUserId'] = self.end_user_id
         if self.external_user_id is not None:
             result['ExternalUserId'] = self.external_user_id
         if self.policy is not None:
             result['Policy'] = self.policy
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AutoCreateUser') is not None:
+            self.auto_create_user = m.get('AutoCreateUser')
         if m.get('EndUserId') is not None:
             self.end_user_id = m.get('EndUserId')
         if m.get('ExternalUserId') is not None:
             self.external_user_id = m.get('ExternalUserId')
         if m.get('Policy') is not None:
             self.policy = m.get('Policy')
         return self
```

### Comparing `alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218.egg-info/PKG-INFO` & `alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-appstream-center20210218
-Version: 1.0.1
+Version: 1.0.4
 Summary: Alibaba Cloud appstream-center (20210218) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_appstream-center20210218-1.0.1/alibabacloud_appstream_center20210218.egg-info/SOURCES.txt` & `alibabacloud_appstream-center20210218-1.0.4/alibabacloud_appstream_center20210218.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210218-1.0.1/setup.py` & `alibabacloud_appstream-center20210218-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_appstream-center20210218.
 
-Created on 14/12/2022
+Created on 05/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_appstream_center20210218"
 NAME = "alibabacloud_appstream-center20210218" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud appstream-center (20210218) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

