# Comparing `tmp/tencentcloud-sdk-python-batch-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-batch-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.905.tar", last modified: Fri Jun  2 00:20:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.906.tar", last modified: Mon Jun  5 00:26:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-batch-3.0.905.tar` & `tencentcloud-sdk-python-batch-3.0.906.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-02 00:20:27.000000 tencentcloud-sdk-python-batch-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud/batch/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud/batch/v20170312/
--rw-r--r--   0 root         (0) root         (0)     8555 2023-06-02 00:20:27.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud/batch/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:20:27.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud/batch/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   194613 2023-06-02 00:20:27.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud/batch/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)    31537 2023-06-02 00:20:27.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud/batch/v20170312/batch_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:20:27.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud/batch/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:20:27.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud_sdk_python_batch.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/tencentcloud_sdk_python_batch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-02 00:20:27.000000 tencentcloud-sdk-python-batch-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:20:28.000000 tencentcloud-sdk-python-batch-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/
+-rw-r--r--   0 root         (0) root         (0)     8555 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   194613 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)    31537 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:26:55.000000 tencentcloud-sdk-python-batch-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-batch-3.0.905/README.rst` & `tencentcloud-sdk-python-batch-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.905/tencentcloud/batch/v20170312/errorcodes.py` & `tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.905/tencentcloud/batch/v20170312/models.py` & `tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.905/tencentcloud/batch/v20170312/batch_client.py` & `tencentcloud-sdk-python-batch-3.0.906/tencentcloud/batch/v20170312/batch_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-batch-3.0.906/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-batch-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.906/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.905/tencentcloud_sdk_python_batch.egg-info/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.906/tencentcloud_sdk_python_batch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.905/setup.py` & `tencentcloud-sdk-python-batch-3.0.906/setup.py`

 * *Files identical despite different names*

