# Comparing `tmp/alibabacloud_appstream-center20210218_py2-1.0.1.tar.gz` & `tmp/alibabacloud_appstream-center20210218_py2-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_appstream-center20210218_py2-1.0.1.tar", last modified: Wed Dec 14 10:33:26 2022, max compression
+gzip compressed data, was "dist/alibabacloud_appstream-center20210218_py2-1.0.4.tar", last modified: Mon Jun  5 03:36:27 2023, max compression
```

## Comparing `alibabacloud_appstream-center20210218_py2-1.0.1.tar` & `alibabacloud_appstream-center20210218_py2-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 10:33:26.000000 alibabacloud_appstream-center20210218_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       39 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2550 2022-12-14 10:33:26.000000 alibabacloud_appstream-center20210218_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1072 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1155 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 10:33:26.000000 alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2634 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218/client.py
--rw-r--r--   0 root         (0) root         (0)     4767 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 10:33:26.000000 alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2550 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      544 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-14 10:33:26.000000 alibabacloud_appstream-center20210218_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2970 2022-12-14 10:33:25.000000 alibabacloud_appstream-center20210218_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:36:27.000000 alibabacloud_appstream-center20210218_py2-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-05 03:36:26.000000 alibabacloud_appstream-center20210218_py2-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-05 03:36:26.000000 alibabacloud_appstream-center20210218_py2-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-05 03:36:26.000000 alibabacloud_appstream-center20210218_py2-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-06-05 03:36:27.000000 alibabacloud_appstream-center20210218_py2-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-06-05 03:36:26.000000 alibabacloud_appstream-center20210218_py2-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-06-05 03:36:26.000000 alibabacloud_appstream-center20210218_py2-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:36:27.000000 alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 03:36:26.000000 alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4091 2023-06-05 03:36:26.000000 alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218/client.py
+-rw-r--r--   0 root         (0) root         (0)     8482 2023-06-05 03:36:26.000000 alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:36:27.000000 alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-06-05 03:36:27.000000 alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-05 03:36:27.000000 alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 03:36:27.000000 alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-05 03:36:27.000000 alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 03:36:27.000000 alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 03:36:27.000000 alibabacloud_appstream-center20210218_py2-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-06-05 03:36:26.000000 alibabacloud_appstream-center20210218_py2-1.0.4/setup.py
```

### Comparing `alibabacloud_appstream-center20210218_py2-1.0.1/LICENSE` & `alibabacloud_appstream-center20210218_py2-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210218_py2-1.0.1/PKG-INFO` & `alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_appstream-center20210218_py2
-Version: 1.0.1
+Name: alibabacloud-appstream-center20210218-py2
+Version: 1.0.4
 Summary: Alibaba Cloud appstream-center (20210218) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_appstream-center20210218_py2-1.0.1/README-CN.md` & `alibabacloud_appstream-center20210218_py2-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210218_py2-1.0.1/README.md` & `alibabacloud_appstream-center20210218_py2-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218/client.py` & `alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,17 +26,53 @@
     def get_endpoint(self, product_id, region_id, endpoint_rule, network, suffix, endpoint_map, endpoint):
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
+    def expire_login_token_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.end_user_id):
+            body['EndUserId'] = request.end_user_id
+        if not UtilClient.is_unset(request.login_token):
+            body['LoginToken'] = request.login_token
+        if not UtilClient.is_unset(request.office_site_id):
+            body['OfficeSiteId'] = request.office_site_id
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ExpireLoginToken',
+            version='2021-02-18',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            appstream_center_20210218_models.ExpireLoginTokenResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def expire_login_token(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.expire_login_token_with_options(request, runtime)
+
     def get_auth_code_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.auto_create_user):
+            body['AutoCreateUser'] = request.auto_create_user
         if not UtilClient.is_unset(request.end_user_id):
             body['EndUserId'] = request.end_user_id
         if not UtilClient.is_unset(request.external_user_id):
             body['ExternalUserId'] = request.external_user_id
         if not UtilClient.is_unset(request.policy):
             body['Policy'] = request.policy
         req = open_api_models.OpenApiRequest(
```

### Comparing `alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218_py2.egg-info/PKG-INFO` & `alibabacloud_appstream-center20210218_py2-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-appstream-center20210218-py2
-Version: 1.0.1
+Name: alibabacloud_appstream-center20210218_py2
+Version: 1.0.4
 Summary: Alibaba Cloud appstream-center (20210218) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_appstream-center20210218_py2-1.0.1/alibabacloud_appstream_center20210218_py2.egg-info/SOURCES.txt` & `alibabacloud_appstream-center20210218_py2-1.0.4/alibabacloud_appstream_center20210218_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210218_py2-1.0.1/setup.py` & `alibabacloud_appstream-center20210218_py2-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_appstream-center20210218_py2.
 
-Created on 14/12/2022
+Created on 05/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_appstream_center20210218"
 NAME = "alibabacloud_appstream-center20210218_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud appstream-center (20210218) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.0, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

