# Comparing `tmp/dapr-ext-workflow-0.1.0.tar.gz` & `tmp/dapr-ext-workflow-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-workflow-0.1.0.tar", last modified: Mon Jun  5 19:26:19 2023, max compression
+gzip compressed data, was "dist/dapr-ext-workflow-0.1.0rc1.tar", last modified: Thu Jun  1 16:51:50 2023, max compression
```

## Comparing `dapr-ext-workflow-0.1.0.tar` & `dapr-ext-workflow-0.1.0rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/dapr/ext/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/dapr/ext/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/dapr/ext/workflow/dapr_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/dapr/ext/workflow/dapr_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/dapr/ext/workflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/dapr/ext/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/dapr/ext/workflow/workflow_activity_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/dapr/ext/workflow/workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/dapr/ext/workflow/workflow_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/dapr/ext/workflow/workflow_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/dapr_ext_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/dapr_ext_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/dapr_ext_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/dapr_ext_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/dapr_ext_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/dapr_ext_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-05 19:26:19.000000 dapr-ext-workflow-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-05 19:26:03.000000 dapr-ext-workflow-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/dapr_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/dapr_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_activity_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-01 16:51:50.000000 dapr-ext-workflow-0.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-01 16:51:31.000000 dapr-ext-workflow-0.1.0rc1/setup.py
```

### Comparing `dapr-ext-workflow-0.1.0/LICENSE` & `dapr-ext-workflow-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.1.0/PKG-INFO` & `dapr-ext-workflow-0.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: The official release of Dapr Python SDK Workflow Authoring Extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-0.1.0/dapr/ext/workflow/__init__.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.1.0/dapr/ext/workflow/dapr_workflow_client.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/dapr_workflow_client.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.1.0/dapr/ext/workflow/dapr_workflow_context.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/dapr_workflow_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.1.0/dapr/ext/workflow/util.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/util.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.1.0/dapr/ext/workflow/version.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.0rc1"
```

### Comparing `dapr-ext-workflow-0.1.0/dapr/ext/workflow/workflow_activity_context.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_activity_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.1.0/dapr/ext/workflow/workflow_context.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.1.0/dapr/ext/workflow/workflow_runtime.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_runtime.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.1.0/dapr/ext/workflow/workflow_state.py` & `dapr-ext-workflow-0.1.0rc1/dapr/ext/workflow/workflow_state.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.1.0/dapr_ext_workflow.egg-info/PKG-INFO` & `dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: The official release of Dapr Python SDK Workflow Authoring Extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-0.1.0/dapr_ext_workflow.egg-info/SOURCES.txt` & `dapr-ext-workflow-0.1.0rc1/dapr_ext_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.1.0/setup.cfg` & `dapr-ext-workflow-0.1.0rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	Source = https://github.com/dapr/python-sdk
 
 [options]
 python_requires = >=3.7
 packages = find_namespace:
 include_package_data = True
 install_requires = 
-	dapr >= 1.10.0
+	dapr >= 1.10.0rc1
 	durabletask >= 0.1.0a2
 
 [options.packages.find]
 include = 
 	dapr.*
 exclude = 
 	tests
```

### Comparing `dapr-ext-workflow-0.1.0/setup.py` & `dapr-ext-workflow-0.1.0rc1/setup.py`

 * *Files identical despite different names*

