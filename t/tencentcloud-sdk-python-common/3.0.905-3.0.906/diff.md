# Comparing `tmp/tencentcloud-sdk-python-common-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-common-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-common-3.0.905.tar", last modified: Fri Jun  2 00:25:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-common-3.0.906.tar", last modified: Mon Jun  5 00:31:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-common-3.0.905.tar` & `tencentcloud-sdk-python-common-3.0.906.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/
--rw-r--r--   0 root         (0) root         (0)     1568 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/sign.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/http/
--rw-r--r--   0 root         (0) root         (0)     4993 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/http/request.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15666 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/credential.py
--rw-r--r--   0 root         (0) root         (0)    18549 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/abstract_client.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/common_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/profile/
--rw-r--r--   0 root         (0) root         (0)     1645 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/profile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/exception/
--rw-r--r--   0 root         (0) root         (0)      760 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/abstract_model.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud_sdk_python_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud_sdk_python_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      837 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud_sdk_python_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud_sdk_python_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud_sdk_python_common.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/tencentcloud_sdk_python_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:25:11.000000 tencentcloud-sdk-python-common-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/sign.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/http/
+-rw-r--r--   0 root         (0) root         (0)     4993 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/http/request.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15666 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/credential.py
+-rw-r--r--   0 root         (0) root         (0)    18549 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/common_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/profile/
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/profile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/exception/
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud_sdk_python_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud_sdk_python_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      837 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud_sdk_python_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud_sdk_python_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud_sdk_python_common.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/tencentcloud_sdk_python_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:31:15.000000 tencentcloud-sdk-python-common-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-common-3.0.905/README.rst` & `tencentcloud-sdk-python-common-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/sign.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/http/request.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/credential.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/abstract_client.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/common_client.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/profile/client_profile.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/profile/http_profile.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/exception/__init__.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/common/abstract_model.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud_sdk_python_common.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud_sdk_python_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.905/tencentcloud_sdk_python_common.egg-info/PKG-INFO` & `tencentcloud-sdk-python-common-3.0.906/tencentcloud_sdk_python_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-common
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Common SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-common-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-common-3.0.906/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-common
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Common SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-common-3.0.905/setup.py` & `tencentcloud-sdk-python-common-3.0.906/setup.py`

 * *Files identical despite different names*

