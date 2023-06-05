# Comparing `tmp/antchain_stlr-2.3.1.tar.gz` & `tmp/antchain_stlr-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_stlr-2.3.1.tar", last modified: Mon Jun  5 05:58:19 2023, max compression
+gzip compressed data, was "dist/antchain_stlr-2.4.0.tar", last modified: Mon Jun  5 11:46:59 2023, max compression
```

## Comparing `antchain_stlr-2.3.1.tar` & `antchain_stlr-2.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:58:19.000000 antchain_stlr-2.3.1/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-05 05:58:18.000000 antchain_stlr-2.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 05:58:18.000000 antchain_stlr-2.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-05 05:58:19.000000 antchain_stlr-2.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-05 05:58:18.000000 antchain_stlr-2.3.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-05 05:58:18.000000 antchain_stlr-2.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:58:19.000000 antchain_stlr-2.3.1/antchain_sdk_stlr/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 05:58:18.000000 antchain_stlr-2.3.1/antchain_sdk_stlr/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104373 2023-06-05 05:58:18.000000 antchain_stlr-2.3.1/antchain_sdk_stlr/client.py
--rw-r--r--   0 root         (0) root         (0)   243563 2023-06-05 05:58:18.000000 antchain_stlr-2.3.1/antchain_sdk_stlr/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:58:19.000000 antchain_stlr-2.3.1/antchain_stlr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-05 05:58:19.000000 antchain_stlr-2.3.1/antchain_stlr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-05 05:58:19.000000 antchain_stlr-2.3.1/antchain_stlr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 05:58:19.000000 antchain_stlr-2.3.1/antchain_stlr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-05 05:58:19.000000 antchain_stlr-2.3.1/antchain_stlr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-05 05:58:19.000000 antchain_stlr-2.3.1/antchain_stlr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 05:58:19.000000 antchain_stlr-2.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-05 05:58:18.000000 antchain_stlr-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_sdk_stlr/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/antchain_sdk_stlr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   106791 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/antchain_sdk_stlr/client.py
+-rw-r--r--   0 root         (0) root         (0)   247416 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/antchain_sdk_stlr/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/antchain_stlr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 11:46:59.000000 antchain_stlr-2.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-05 11:46:58.000000 antchain_stlr-2.4.0/setup.py
```

### Comparing `antchain_stlr-2.3.1/LICENSE` & `antchain_stlr-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.3.1/PKG-INFO` & `antchain_stlr-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_stlr
-Version: 2.3.1
+Version: 2.4.0
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.3.1/README-CN.md` & `antchain_stlr-2.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.3.1/README.md` & `antchain_stlr-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.3.1/antchain_sdk_stlr/client.py` & `antchain_stlr-2.4.0/antchain_sdk_stlr/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.3.1',
+                    'sdk_version': '2.4.0',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.3.1',
+                    'sdk_version': '2.4.0',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -2377,14 +2377,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             stlr_models.DetailEcarEnterprisememberResponse(),
             await self.do_request_async('1.0', 'antchain.carbon.ecar.enterprisemember.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def query_ecar_offsetaccount(
+        self,
+        request: stlr_models.QueryEcarOffsetaccountRequest,
+    ) -> stlr_models.QueryEcarOffsetaccountResponse:
+        """
+        Description: 碳补偿项目账户查询，根据账户DID和项目编码查询账户信息
+        Summary: 碳补偿项目账户查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_ecar_offsetaccount_ex(request, headers, runtime)
+
+    async def query_ecar_offsetaccount_async(
+        self,
+        request: stlr_models.QueryEcarOffsetaccountRequest,
+    ) -> stlr_models.QueryEcarOffsetaccountResponse:
+        """
+        Description: 碳补偿项目账户查询，根据账户DID和项目编码查询账户信息
+        Summary: 碳补偿项目账户查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_ecar_offsetaccount_ex_async(request, headers, runtime)
+
+    def query_ecar_offsetaccount_ex(
+        self,
+        request: stlr_models.QueryEcarOffsetaccountRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryEcarOffsetaccountResponse:
+        """
+        Description: 碳补偿项目账户查询，根据账户DID和项目编码查询账户信息
+        Summary: 碳补偿项目账户查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryEcarOffsetaccountResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.offsetaccount.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_ecar_offsetaccount_ex_async(
+        self,
+        request: stlr_models.QueryEcarOffsetaccountRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryEcarOffsetaccountResponse:
+        """
+        Description: 碳补偿项目账户查询，根据账户DID和项目编码查询账户信息
+        Summary: 碳补偿项目账户查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryEcarOffsetaccountResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.offsetaccount.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_third_cert(
         self,
         request: stlr_models.QueryThirdCertRequest,
     ) -> stlr_models.QueryThirdCertResponse:
         """
         Description: 三方平台调用此接口，查询用户的证书信息
         Summary: 证书查询
```

### Comparing `antchain_stlr-2.3.1/antchain_sdk_stlr/models.py` & `antchain_stlr-2.4.0/antchain_sdk_stlr/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6200,14 +6200,126 @@
         if m.get('mobile') is not None:
             self.mobile = m.get('mobile')
         if m.get('register_time') is not None:
             self.register_time = m.get('register_time')
         return self
 
 
+class QueryEcarOffsetaccountRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        project_no: str = None,
+        account_did: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 碳普惠项目编码
+        self.project_no = project_no
+        # 账户DID
+        self.account_did = account_did
+
+    def validate(self):
+        self.validate_required(self.project_no, 'project_no')
+        self.validate_required(self.account_did, 'account_did')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.project_no is not None:
+            result['project_no'] = self.project_no
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('project_no') is not None:
+            self.project_no = m.get('project_no')
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        return self
+
+
+class QueryEcarOffsetaccountResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        project_no: str = None,
+        account_did: str = None,
+        offset_balance: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 碳普惠项目编码
+        self.project_no = project_no
+        # 账户DID
+        self.account_did = account_did
+        # 账户减碳量余额
+        self.offset_balance = offset_balance
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.project_no is not None:
+            result['project_no'] = self.project_no
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
+        if self.offset_balance is not None:
+            result['offset_balance'] = self.offset_balance
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('project_no') is not None:
+            self.project_no = m.get('project_no')
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        if m.get('offset_balance') is not None:
+            self.offset_balance = m.get('offset_balance')
+        return self
+
+
 class QueryThirdCertRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         product_id: str = None,
         certification_type: str = None,
```

### Comparing `antchain_stlr-2.3.1/antchain_stlr.egg-info/PKG-INFO` & `antchain_stlr-2.4.0/antchain_stlr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-stlr
-Version: 2.3.1
+Version: 2.4.0
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.3.1/setup.py` & `antchain_stlr-2.4.0/setup.py`

 * *Files identical despite different names*

