# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.905.tar", last modified: Fri Jun  2 00:42:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.906.tar", last modified: Mon Jun  5 00:44:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.905.tar` & `tencentcloud-sdk-python-tke-3.0.906.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:42:14.000000 tencentcloud-sdk-python-tke-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:42:14.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)   183327 2023-06-02 00:42:14.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19455 2023-06-02 00:42:14.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:42:14.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   671889 2023-06-02 00:42:14.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:42:14.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:42:14.000000 tencentcloud-sdk-python-tke-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:42:15.000000 tencentcloud-sdk-python-tke-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:44:49.000000 tencentcloud-sdk-python-tke-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:44:49.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)   183327 2023-06-05 00:44:49.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19455 2023-06-05 00:44:49.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:44:49.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   671889 2023-06-05 00:44:49.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:44:49.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:44:49.000000 tencentcloud-sdk-python-tke-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:44:50.000000 tencentcloud-sdk-python-tke-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tke-3.0.905/README.rst` & `tencentcloud-sdk-python-tke-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.905/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.906/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.905/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.906/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.905/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.906/tencentcloud/tke/v20180525/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.906/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.906/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.905/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.906/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.905/setup.py` & `tencentcloud-sdk-python-tke-3.0.906/setup.py`

 * *Files identical despite different names*

