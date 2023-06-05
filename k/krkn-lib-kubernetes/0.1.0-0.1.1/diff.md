# Comparing `tmp/krkn_lib_kubernetes-0.1.0.tar.gz` & `tmp/krkn_lib_kubernetes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krkn_lib_kubernetes-0.1.0.tar", max compression
+gzip compressed data, was "krkn_lib_kubernetes-0.1.1.tar", max compression
```

## Comparing `krkn_lib_kubernetes-0.1.0.tar` & `krkn_lib_kubernetes-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10173 2023-05-03 16:09:53.570611 krkn_lib_kubernetes-0.1.0/LICENSE
--rw-r--r--   0        0        0      122 2023-05-03 16:09:53.570611 krkn_lib_kubernetes-0.1.0/README.md
--rw-r--r--   0        0        0      592 2023-05-03 16:11:00.741863 krkn_lib_kubernetes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       63 2023-05-03 16:09:53.574611 krkn_lib_kubernetes-0.1.0/src/krkn_lib_kubernetes/__init__.py
--rw-r--r--   0        0        0    43400 2023-05-03 16:11:07.518169 krkn_lib_kubernetes-0.1.0/src/krkn_lib_kubernetes/client.py
--rw-r--r--   0        0        0     1739 2023-05-03 16:09:53.574611 krkn_lib_kubernetes-0.1.0/src/krkn_lib_kubernetes/resources.py
--rw-r--r--   0        0        0    26784 2023-05-03 16:11:07.506169 krkn_lib_kubernetes-0.1.0/src/krkn_lib_kubernetes/test_client.py
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 krkn_lib_kubernetes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-06-05 12:21:29.934886 krkn_lib_kubernetes-0.1.1/LICENSE
+-rw-r--r--   0        0        0      122 2023-06-05 12:21:29.934886 krkn_lib_kubernetes-0.1.1/README.md
+-rw-r--r--   0        0        0      592 2023-06-05 12:22:36.457806 krkn_lib_kubernetes-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-06-05 12:21:29.934886 krkn_lib_kubernetes-0.1.1/src/krkn_lib_kubernetes/__init__.py
+-rw-r--r--   0        0        0    43738 2023-06-05 12:22:40.558231 krkn_lib_kubernetes-0.1.1/src/krkn_lib_kubernetes/client.py
+-rw-r--r--   0        0        0     1739 2023-06-05 12:21:29.938887 krkn_lib_kubernetes-0.1.1/src/krkn_lib_kubernetes/resources.py
+-rw-r--r--   0        0        0    26784 2023-06-05 12:22:40.550230 krkn_lib_kubernetes-0.1.1/src/krkn_lib_kubernetes/test_client.py
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 krkn_lib_kubernetes-0.1.1/PKG-INFO
```

### Comparing `krkn_lib_kubernetes-0.1.0/LICENSE` & `krkn_lib_kubernetes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `krkn_lib_kubernetes-0.1.0/pyproject.toml` & `krkn_lib_kubernetes-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krkn-lib-kubernetes"
-version = "v0.1.0"
+version = "v0.1.1"
 description = "Kubernetes library for Kraken"
 authors = ["Red Hat Chaos Team"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/redhat-chaos/krkn"
 #packages = [{include= "src/krkn_lib_kubernetes"}]
 
@@ -15,10 +15,10 @@
 sphinxnotes-markdown-builder="^0.5.6"
 requests="^2.29.0"
 
 [tool.poetry.group.test.dependencies]
 jinja2 = "^3.1.2"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `krkn_lib_kubernetes-0.1.0/src/krkn_lib_kubernetes/client.py` & `krkn_lib_kubernetes-0.1.1/src/krkn_lib_kubernetes/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,14 +438,21 @@
         :param container: container where the command
                must be executed (optional default `None`)
         :param base_command: base command that must be executed
                along the parameters (optional, default `bash -c`)
         :return: the command stdout
         """
         exec_command = []
+        # this check makes no sense since the type has been declared in the
+        # method signature, but unfortunately python do not enforce on type
+        # checks at compile time so this check
+        # ensures that the command variable is actually a list.
+        if not isinstance(command, list):
+            command = [command]
+
         if base_command is None:
             exec_command = ["bash", "-c"]
             exec_command.extend(command)
         else:
             exec_command.append(base_command)
             exec_command.extend(command)
```

### Comparing `krkn_lib_kubernetes-0.1.0/src/krkn_lib_kubernetes/resources.py` & `krkn_lib_kubernetes-0.1.1/src/krkn_lib_kubernetes/resources.py`

 * *Files identical despite different names*

### Comparing `krkn_lib_kubernetes-0.1.0/src/krkn_lib_kubernetes/test_client.py` & `krkn_lib_kubernetes-0.1.1/src/krkn_lib_kubernetes/test_client.py`

 * *Files identical despite different names*

### Comparing `krkn_lib_kubernetes-0.1.0/PKG-INFO` & `krkn_lib_kubernetes-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krkn-lib-kubernetes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Kubernetes library for Kraken
 Home-page: https://github.com/redhat-chaos/krkn
 License: Apache-2.0
 Author: Red Hat Chaos Team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

