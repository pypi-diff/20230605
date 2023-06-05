# Comparing `tmp/tencentcloud-sdk-python-bma-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-bma-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bma-3.0.905.tar", last modified: Fri Jun  2 00:21:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bma-3.0.906.tar", last modified: Mon Jun  5 00:27:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bma-3.0.905.tar` & `tencentcloud-sdk-python-bma-3.0.906.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20210624/
--rw-r--r--   0 root         (0) root         (0)     1829 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20210624/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25791 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20210624/bma_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20210624/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82603 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20210624/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20221115/
--rw-r--r--   0 root         (0) root         (0)     3348 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20221115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10527 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20221115/bma_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20221115/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39167 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20221115/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud_sdk_python_bma.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud_sdk_python_bma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud_sdk_python_bma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/tencentcloud_sdk_python_bma.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:21:09.000000 tencentcloud-sdk-python-bma-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20210624/
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20210624/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25791 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20210624/bma_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20210624/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82603 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20210624/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20221115/
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20221115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10527 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20221115/bma_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20221115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39167 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20221115/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud_sdk_python_bma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud_sdk_python_bma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud_sdk_python_bma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/tencentcloud_sdk_python_bma.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:27:30.000000 tencentcloud-sdk-python-bma-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-bma-3.0.905/README.rst` & `tencentcloud-sdk-python-bma-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20210624/errorcodes.py` & `tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20210624/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20210624/bma_client.py` & `tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20210624/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20210624/models.py` & `tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20210624/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20221115/errorcodes.py` & `tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20221115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20221115/bma_client.py` & `tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20221115/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.905/tencentcloud/bma/v20221115/models.py` & `tencentcloud-sdk-python-bma-3.0.906/tencentcloud/bma/v20221115/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bma-3.0.906/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bma-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-bma-3.0.906/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bma
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Bma SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bma-3.0.905/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-bma-3.0.906/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.905/tencentcloud_sdk_python_bma.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bma-3.0.906/tencentcloud_sdk_python_bma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bma
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Bma SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bma-3.0.905/setup.py` & `tencentcloud-sdk-python-bma-3.0.906/setup.py`

 * *Files identical despite different names*

