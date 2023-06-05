# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.905.tar", last modified: Fri Jun  2 00:23:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.906.tar", last modified: Mon Jun  5 00:29:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.905.tar` & `tencentcloud-sdk-python-cdn-3.0.906.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21972 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   572032 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:23:04.000000 tencentcloud-sdk-python-cdn-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21972 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   573199 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:29:16.000000 tencentcloud-sdk-python-cdn-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.905/README.rst` & `tencentcloud-sdk-python-cdn-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.905'
+__version__ = '3.0.906'
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.905/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.906/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10981,14 +10981,17 @@
         :type BasePath: str
         :param PathRules: 回源路径重写规则配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type PathRules: list of PathRule
         :param PathBasedOrigin: 分路径回源配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type PathBasedOrigin: list of PathBasedOriginRule
+        :param Sni: HTTPS回源SNI配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Sni: :class:`tencentcloud.cdn.v20180606.models.OriginSni`
         :param AdvanceHttps: HTTPS回源高级配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type AdvanceHttps: :class:`tencentcloud.cdn.v20180606.models.AdvanceHttps`
         :param OriginCompany: 对象存储回源厂商，当源站类型为第三方存储源站(third_party)时必填，可选值包括以下:
 aws_s3: AWS S3
 ali_oss: 阿里云 OSS
 hw_obs: 华为 OBS
@@ -11004,14 +11007,15 @@
         self.OriginPullProtocol = None
         self.BackupOrigins = None
         self.BackupOriginType = None
         self.BackupServerName = None
         self.BasePath = None
         self.PathRules = None
         self.PathBasedOrigin = None
+        self.Sni = None
         self.AdvanceHttps = None
         self.OriginCompany = None
 
 
     def _deserialize(self, params):
         self.Origins = params.get("Origins")
         self.OriginType = params.get("OriginType")
@@ -11030,14 +11034,17 @@
                 self.PathRules.append(obj)
         if params.get("PathBasedOrigin") is not None:
             self.PathBasedOrigin = []
             for item in params.get("PathBasedOrigin"):
                 obj = PathBasedOriginRule()
                 obj._deserialize(item)
                 self.PathBasedOrigin.append(obj)
+        if params.get("Sni") is not None:
+            self.Sni = OriginSni()
+            self.Sni._deserialize(params.get("Sni"))
         if params.get("AdvanceHttps") is not None:
             self.AdvanceHttps = AdvanceHttps()
             self.AdvanceHttps._deserialize(params.get("AdvanceHttps"))
         self.OriginCompany = params.get("OriginCompany")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
@@ -11214,14 +11221,45 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class OriginSni(AbstractModel):
+    """HTTPS回源SNI
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Switch: 是否开启HTTPS回源SNI。
+开启：on，
+关闭：off
+        :type Switch: str
+        :param ServerName: 回源域名。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ServerName: str
+        """
+        self.Switch = None
+        self.ServerName = None
+
+
+    def _deserialize(self, params):
+        self.Switch = params.get("Switch")
+        self.ServerName = params.get("ServerName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class OssPrivateAccess(AbstractModel):
     """oss回源鉴权
 
     """
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.906/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.905/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.906/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.905/setup.py` & `tencentcloud-sdk-python-cdn-3.0.906/setup.py`

 * *Files identical despite different names*

