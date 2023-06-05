# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.905.tar", last modified: Fri Jun  2 00:28:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.906.tar", last modified: Mon Jun  5 00:34:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.905.tar` & `tencentcloud-sdk-python-essbasic-3.0.906.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16533 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    51460 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   232146 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:28:38.000000 tencentcloud-sdk-python-essbasic-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    51478 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   232146 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:34:32.000000 tencentcloud-sdk-python-essbasic-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ChannelCreateEmbedWebUrl(self, request):
-        """本接口（ChannelCreateEmbedWebUrl）用于创建嵌入web的链接
+        """本接口（ChannelCreateEmbedWebUrl）用于创建常规模块嵌入web的链接
         本接口支持创建：创建印章，创建模板，修改模板，预览模板，预览合同流程的web链接
         进入web连接后与当前控制台操作保持一致
 
         :param request: Request instance for ChannelCreateEmbedWebUrl.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateEmbedWebUrlRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateEmbedWebUrlResponse`
 
@@ -300,15 +300,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ChannelCreateFlowSignUrl(self, request):
-        """创建个人H5签署链接，请联系客户经理申请使用<br/>
+        """创建个人签署H5签署链接，请联系客户经理申请使用<br/>
         该接口用于发起合同后，生成C端签署人的签署链接<br/>
         注意：该接口目前签署人类型仅支持个人签署方（PERSON）<br/>
         注意：该接口可生成签署链接的C端签署人必须仅有手写签名和时间类型的签署控件<br/>
         注意：该接口返回的签署链接是用于APP集成的场景，支持APP打开或浏览器直接打开，不支持微信小程序嵌入。微信小程序请使用小程序跳转或半屏弹窗的方式<br/>
 
         :param request: Request instance for ChannelCreateFlowSignUrl.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateFlowSignUrlRequest`
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20210526/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.906/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.906/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.905/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.906/setup.py`

 * *Files identical despite different names*

