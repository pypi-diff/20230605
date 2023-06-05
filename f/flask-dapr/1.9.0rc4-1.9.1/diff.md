# Comparing `tmp/flask-dapr-1.9.0rc4.tar.gz` & `tmp/flask-dapr-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask-dapr-1.9.0rc4.tar", last modified: Wed Feb 15 22:45:21 2023, max compression
+gzip compressed data, was "dist/flask-dapr-1.9.1.tar", last modified: Tue Mar 21 16:28:41 2023, max compression
```

## Comparing `flask-dapr-1.9.0rc4.tar` & `flask-dapr-1.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-02-15 22:45:07.000000 flask-dapr-1.9.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-15 22:45:07.000000 flask-dapr-1.9.0rc4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/flask_dapr/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-15 22:45:07.000000 flask-dapr-1.9.0rc4/flask_dapr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-02-15 22:45:07.000000 flask-dapr-1.9.0rc4/flask_dapr/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-02-15 22:45:07.000000 flask-dapr-1.9.0rc4/flask_dapr/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-15 22:45:07.000000 flask-dapr-1.9.0rc4/flask_dapr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/flask_dapr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/flask_dapr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/flask_dapr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/flask_dapr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/flask_dapr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/flask_dapr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/flask_dapr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-15 22:45:21.000000 flask-dapr-1.9.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-15 22:45:07.000000 flask-dapr-1.9.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-03-21 16:28:22.000000 flask-dapr-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-21 16:28:22.000000 flask-dapr-1.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/flask_dapr/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-21 16:28:22.000000 flask-dapr-1.9.1/flask_dapr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-03-21 16:28:22.000000 flask-dapr-1.9.1/flask_dapr/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-21 16:28:22.000000 flask-dapr-1.9.1/flask_dapr/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-21 16:28:22.000000 flask-dapr-1.9.1/flask_dapr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/flask_dapr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/flask_dapr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/flask_dapr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/flask_dapr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/flask_dapr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/flask_dapr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/flask_dapr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-21 16:28:41.000000 flask-dapr-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-21 16:28:22.000000 flask-dapr-1.9.1/setup.py
```

### Comparing `flask-dapr-1.9.0rc4/LICENSE` & `flask-dapr-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-dapr-1.9.0rc4/PKG-INFO` & `flask-dapr-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: flask-dapr
-Version: 1.9.0rc4
+Version: 1.9.1
 Summary: The official release of Dapr Python SDK Flask Extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `flask-dapr-1.9.0rc4/README.rst` & `flask-dapr-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `flask-dapr-1.9.0rc4/flask_dapr/__init__.py` & `flask-dapr-1.9.1/flask_dapr/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-dapr-1.9.0rc4/flask_dapr/actor.py` & `flask-dapr-1.9.1/flask_dapr/actor.py`

 * *Files identical despite different names*

### Comparing `flask-dapr-1.9.0rc4/flask_dapr/app.py` & `flask-dapr-1.9.1/flask_dapr/app.py`

 * *Files identical despite different names*

### Comparing `flask-dapr-1.9.0rc4/flask_dapr/version.py` & `flask-dapr-1.9.1/flask_dapr/version.py`

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

### Comparing `flask-dapr-1.9.0rc4/flask_dapr.egg-info/PKG-INFO` & `flask-dapr-1.9.1/flask_dapr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: flask-dapr
-Version: 1.9.0rc4
+Version: 1.9.1
 Summary: The official release of Dapr Python SDK Flask Extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `flask-dapr-1.9.0rc4/setup.cfg` & `flask-dapr-1.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,13 +21,13 @@
 [options]
 python_requires = >=3.7
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
 	Flask >= 1.1
-	dapr >= 1.9.0rc4
+	dapr >= 1.9.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `flask-dapr-1.9.0rc4/setup.py` & `flask-dapr-1.9.1/setup.py`

 * *Files identical despite different names*

