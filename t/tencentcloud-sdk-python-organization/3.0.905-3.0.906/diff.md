# Comparing `tmp/tencentcloud-sdk-python-organization-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-organization-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.905.tar", last modified: Fri Jun  2 00:35:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.906.tar", last modified: Mon Jun  5 00:39:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-organization-3.0.905.tar` & `tencentcloud-sdk-python-organization-3.0.906.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/
--rw-r--r--   0 root         (0) root         (0)      764 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20210331/
--rw-r--r--   0 root         (0) root         (0)    17475 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20210331/organization_client.py
--rw-r--r--   0 root         (0) root         (0)     8203 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20210331/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20210331/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55554 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20210331/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20181225/
--rw-r--r--   0 root         (0) root         (0)    19620 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20181225/organization_client.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20181225/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20181225/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30659 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20181225/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud_sdk_python_organization.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      738 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/tencentcloud_sdk_python_organization.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:35:56.000000 tencentcloud-sdk-python-organization-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/
+-rw-r--r--   0 root         (0) root         (0)      764 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20210331/
+-rw-r--r--   0 root         (0) root         (0)    17475 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20210331/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)     8203 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20210331/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20210331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55554 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20210331/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20181225/
+-rw-r--r--   0 root         (0) root         (0)    19620 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20181225/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20181225/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20181225/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30659 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20181225/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud_sdk_python_organization.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/tencentcloud_sdk_python_organization.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:39:39.000000 tencentcloud-sdk-python-organization-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-organization-3.0.905/README.rst` & `tencentcloud-sdk-python-organization-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20210331/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20210331/organization_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20210331/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20210331/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20210331/models.py` & `tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20210331/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20181225/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20181225/organization_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20181225/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20181225/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.905/tencentcloud/organization/v20181225/models.py` & `tencentcloud-sdk-python-organization-3.0.906/tencentcloud/organization/v20181225/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-organization-3.0.906/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-organization-3.0.905/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-organization-3.0.906/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.905/tencentcloud_sdk_python_organization.egg-info/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.906/tencentcloud_sdk_python_organization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.906/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.905/setup.py` & `tencentcloud-sdk-python-organization-3.0.906/setup.py`

 * *Files identical despite different names*

