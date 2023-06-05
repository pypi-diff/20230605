# Comparing `tmp/tencentcloud-sdk-python-tbp-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-tbp-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tbp-3.0.905.tar", last modified: Fri Jun  2 00:39:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tbp-3.0.906.tar", last modified: Mon Jun  5 00:42:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tbp-3.0.905.tar` & `tencentcloud-sdk-python-tbp-3.0.906.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud_sdk_python_tbp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud_sdk_python_tbp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud_sdk_python_tbp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190311/
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190311/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190311/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14368 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190311/models.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190311/tbp_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190627/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190627/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190627/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13295 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190627/models.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190627/tbp_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:39:25.000000 tencentcloud-sdk-python-tbp-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14368 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/models.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/tbp_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13544 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/models.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/tbp_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:42:38.000000 tencentcloud-sdk-python-tbp-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/README.rst` & `tencentcloud-sdk-python-tbp-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbp
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Tbp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190311/errorcodes.py` & `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190311/models.py` & `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190311/tbp_client.py` & `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190311/tbp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190627/errorcodes.py` & `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190627/models.py` & `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,25 +291,29 @@
         :type ResponseMessage: :class:`tencentcloud.tbp.v20190627.models.ResponseMessage`
         :param SessionAttributes: 透传字段，由用户自定义的WebService服务返回。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SessionAttributes: str
         :param ResultType: 结果类型 {中间逻辑出错:0; 任务型机器人:1; 问答型机器人:2; 闲聊型机器人:3; 未匹配上，返回预设兜底话术:5; 未匹配上，返回相似问题列表:6}。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResultType: str
+        :param ResponseText: 机器人对话的应答文本。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResponseText: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DialogStatus = None
         self.BotName = None
         self.IntentName = None
         self.SlotInfoList = None
         self.InputText = None
         self.ResponseMessage = None
         self.SessionAttributes = None
         self.ResultType = None
+        self.ResponseText = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.DialogStatus = params.get("DialogStatus")
         self.BotName = params.get("BotName")
         self.IntentName = params.get("IntentName")
@@ -321,8 +325,9 @@
                 self.SlotInfoList.append(obj)
         self.InputText = params.get("InputText")
         if params.get("ResponseMessage") is not None:
             self.ResponseMessage = ResponseMessage()
             self.ResponseMessage._deserialize(params.get("ResponseMessage"))
         self.SessionAttributes = params.get("SessionAttributes")
         self.ResultType = params.get("ResultType")
+        self.ResponseText = params.get("ResponseText")
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/tbp/v20190627/tbp_client.py` & `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/tbp/v20190627/tbp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tbp-3.0.906/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-tbp-3.0.906/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbp
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Tbp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.905/setup.py` & `tencentcloud-sdk-python-tbp-3.0.906/setup.py`

 * *Files identical despite different names*

