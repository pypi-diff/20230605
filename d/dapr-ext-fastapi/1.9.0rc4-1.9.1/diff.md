# Comparing `tmp/dapr-ext-fastapi-1.9.0rc4.tar.gz` & `tmp/dapr-ext-fastapi-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-fastapi-1.9.0rc4.tar", last modified: Wed Feb 15 22:45:27 2023, max compression
+gzip compressed data, was "dist/dapr-ext-fastapi-1.9.1.tar", last modified: Tue Mar 21 16:28:50 2023, max compression
```

## Comparing `dapr-ext-fastapi-1.9.0rc4.tar` & `dapr-ext-fastapi-1.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-02-15 22:45:07.000000 dapr-ext-fastapi-1.9.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-15 22:45:07.000000 dapr-ext-fastapi-1.9.0rc4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/dapr/ext/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-15 22:45:07.000000 dapr-ext-fastapi-1.9.0rc4/dapr/ext/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-02-15 22:45:07.000000 dapr-ext-fastapi-1.9.0rc4/dapr/ext/fastapi/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-02-15 22:45:07.000000 dapr-ext-fastapi-1.9.0rc4/dapr/ext/fastapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-15 22:45:07.000000 dapr-ext-fastapi-1.9.0rc4/dapr/ext/fastapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/dapr_ext_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/dapr_ext_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/dapr_ext_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/dapr_ext_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/dapr_ext_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/dapr_ext_fastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-15 22:45:27.000000 dapr-ext-fastapi-1.9.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-02-15 22:45:07.000000 dapr-ext-fastapi-1.9.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-03-21 16:28:22.000000 dapr-ext-fastapi-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-21 16:28:22.000000 dapr-ext-fastapi-1.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/dapr/ext/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-21 16:28:22.000000 dapr-ext-fastapi-1.9.1/dapr/ext/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-03-21 16:28:22.000000 dapr-ext-fastapi-1.9.1/dapr/ext/fastapi/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-03-21 16:28:22.000000 dapr-ext-fastapi-1.9.1/dapr/ext/fastapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-21 16:28:22.000000 dapr-ext-fastapi-1.9.1/dapr/ext/fastapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/dapr_ext_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/dapr_ext_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/dapr_ext_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/dapr_ext_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/dapr_ext_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/dapr_ext_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-21 16:28:50.000000 dapr-ext-fastapi-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-21 16:28:22.000000 dapr-ext-fastapi-1.9.1/setup.py
```

### Comparing `dapr-ext-fastapi-1.9.0rc4/LICENSE` & `dapr-ext-fastapi-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-1.9.0rc4/PKG-INFO` & `dapr-ext-fastapi-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-fastapi
-Version: 1.9.0rc4
+Version: 1.9.1
 Summary: The official release of Dapr FastAPI extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-fastapi-1.9.0rc4/dapr/ext/fastapi/__init__.py` & `dapr-ext-fastapi-1.9.1/dapr/ext/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-1.9.0rc4/dapr/ext/fastapi/actor.py` & `dapr-ext-fastapi-1.9.1/dapr/ext/fastapi/actor.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-1.9.0rc4/dapr/ext/fastapi/app.py` & `dapr-ext-fastapi-1.9.1/dapr/ext/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-fastapi-1.9.0rc4/dapr/ext/fastapi/version.py` & `dapr-ext-fastapi-1.9.1/dapr/ext/fastapi/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-__version__ = "1.9.0rc4"
+__version__ = "1.9.1"
```

### Comparing `dapr-ext-fastapi-1.9.0rc4/dapr_ext_fastapi.egg-info/PKG-INFO` & `dapr-ext-fastapi-1.9.1/dapr_ext_fastapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-fastapi
-Version: 1.9.0rc4
+Version: 1.9.1
 Summary: The official release of Dapr FastAPI extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-fastapi-1.9.0rc4/setup.cfg` & `dapr-ext-fastapi-1.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	Source = https://github.com/dapr/python-sdk
 
 [options]
 python_requires = >=3.7
 packages = find_namespace:
 include_package_data = True
 install_requires = 
-	dapr >= 1.9.0rc4
+	dapr >= 1.9.1
 	uvicorn >= 0.11.6
 	fastapi >= 0.60.1
 
 [options.packages.find]
 include = 
 	dapr.*
 exclude =
```

### Comparing `dapr-ext-fastapi-1.9.0rc4/setup.py` & `dapr-ext-fastapi-1.9.1/setup.py`

 * *Files identical despite different names*

