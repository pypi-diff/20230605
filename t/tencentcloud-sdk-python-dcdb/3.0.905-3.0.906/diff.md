# Comparing `tmp/tencentcloud-sdk-python-dcdb-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-dcdb-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.905.tar", last modified: Fri Jun  2 00:26:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.906.tar", last modified: Mon Jun  5 00:32:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dcdb-3.0.905.tar` & `tencentcloud-sdk-python-dcdb-3.0.906.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud_sdk_python_dcdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/dcdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/dcdb/v20180411/
--rw-r--r--   0 root         (0) root         (0)    13722 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/dcdb/v20180411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/dcdb/v20180411/__init__.py
--rw-r--r--   0 root         (0) root         (0)   241269 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/dcdb/v20180411/models.py
--rw-r--r--   0 root         (0) root         (0)    70022 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/dcdb/v20180411/dcdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/dcdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:26:50.000000 tencentcloud-sdk-python-dcdb-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud_sdk_python_dcdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/dcdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/dcdb/v20180411/
+-rw-r--r--   0 root         (0) root         (0)    13722 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/dcdb/v20180411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/dcdb/v20180411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   241570 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/dcdb/v20180411/models.py
+-rw-r--r--   0 root         (0) root         (0)    70022 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/dcdb/v20180411/dcdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/dcdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:32:55.000000 tencentcloud-sdk-python-dcdb-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.905/README.rst` & `tencentcloud-sdk-python-dcdb-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/dcdb/v20180411/errorcodes.py` & `tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/dcdb/v20180411/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/dcdb/v20180411/models.py` & `tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/dcdb/v20180411/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -908,21 +908,29 @@
 class CreateDedicatedClusterDCDBInstanceResponse(AbstractModel):
     """CreateDedicatedClusterDCDBInstance返回参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param InstanceIds: 分配资源ID数组
+        :type InstanceIds: list of str
+        :param FlowId: 流程ID
+        :type FlowId: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
+        self.InstanceIds = None
+        self.FlowId = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
+        self.InstanceIds = params.get("InstanceIds")
+        self.FlowId = params.get("FlowId")
         self.RequestId = params.get("RequestId")
 
 
 class CreateHourDCDBInstanceRequest(AbstractModel):
     """CreateHourDCDBInstance请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/dcdb/v20180411/dcdb_client.py` & `tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/dcdb/v20180411/dcdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dcdb-3.0.906/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dcdb-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.906/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.905/setup.py` & `tencentcloud-sdk-python-dcdb-3.0.906/setup.py`

 * *Files identical despite different names*

