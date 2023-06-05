# Comparing `tmp/cuscom-0.2.7.tar.gz` & `tmp/cuscom-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cuscom-0.2.7.tar", last modified: Wed Apr  6 12:17:06 2022, max compression
+gzip compressed data, was "dist/cuscom-1.0.0.tar", last modified: Mon Jun  5 08:49:10 2023, max compression
```

## Comparing `cuscom-0.2.7.tar` & `cuscom-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 12:17:06.000000 cuscom-0.2.7/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-04-06 12:16:42.000000 cuscom-0.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      585 2022-04-06 12:17:06.000000 cuscom-0.2.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      188 2022-04-06 12:16:42.000000 cuscom-0.2.7/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2022-04-06 12:16:55.000000 cuscom-0.2.7/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 12:17:06.000000 cuscom-0.2.7/cuscom.egg-info/
--rw-r--r--   0 root         (0) root         (0)      585 2022-04-06 12:17:06.000000 cuscom-0.2.7/cuscom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2022-04-06 12:17:06.000000 cuscom-0.2.7/cuscom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-06 12:17:06.000000 cuscom-0.2.7/cuscom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2022-04-06 12:17:06.000000 cuscom-0.2.7/cuscom.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-04-06 12:17:06.000000 cuscom-0.2.7/cuscom.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 12:17:06.000000 cuscom-0.2.7/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 12:17:06.000000 cuscom-0.2.7/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-04-06 12:16:42.000000 cuscom-0.2.7/docs/source/description.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-04-06 12:17:06.000000 cuscom-0.2.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1211 2022-04-06 12:16:42.000000 cuscom-0.2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 12:17:06.000000 cuscom-0.2.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 12:17:06.000000 cuscom-0.2.7/src/cuscom/
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-04-06 12:16:42.000000 cuscom-0.2.7/src/cuscom/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 12:17:06.000000 cuscom-0.2.7/src/cuscom/clients/
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-04-06 12:16:42.000000 cuscom-0.2.7/src/cuscom/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1183 2022-04-06 12:16:42.000000 cuscom-0.2.7/src/cuscom/clients/base_client.py
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-04-06 12:16:42.000000 cuscom-0.2.7/src/cuscom/clients/task_client.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-04-06 12:16:42.000000 cuscom-0.2.7/src/cuscom/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 12:17:06.000000 cuscom-0.2.7/src/cuscom/hooks/
--rw-rw-rw-   0 root         (0) root         (0)       74 2022-04-06 12:16:42.000000 cuscom-0.2.7/src/cuscom/hooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2022-04-06 12:16:42.000000 cuscom-0.2.7/src/cuscom/hooks/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 12:17:06.000000 cuscom-0.2.7/src/cuscom/operators/
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-04-06 12:16:42.000000 cuscom-0.2.7/src/cuscom/operators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1325 2022-04-06 12:16:42.000000 cuscom-0.2.7/src/cuscom/operators/custom_kubernetes_pod_operator.py
--rw-rw-rw-   0 root         (0) root         (0)     1663 2022-04-06 12:16:42.000000 cuscom-0.2.7/src/cuscom/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-06-05 08:48:50.000000 cuscom-1.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-05 08:48:50.000000 cuscom-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-05 08:49:10.000000 cuscom-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-05 08:48:50.000000 cuscom-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-05 08:49:00.000000 cuscom-1.0.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      548 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-05 08:48:50.000000 cuscom-1.0.0/docs/source/description.rst
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-05 08:48:50.000000 cuscom-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 08:49:10.000000 cuscom-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2023-06-05 08:48:50.000000 cuscom-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/src/cuscom/
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/src/cuscom/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/clients/base_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/clients/task_client.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/src/cuscom/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/hooks/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/src/cuscom/operators/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/operators/custom_kubernetes_pod_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/utils.py
```

### Comparing `cuscom-0.2.7/cuscom.egg-info/SOURCES.txt` & `cuscom-1.0.0/cuscom.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+LICENSE
 MANIFEST.in
 README.md
 VERSION
+pyproject.toml
 setup.py
 cuscom.egg-info/PKG-INFO
 cuscom.egg-info/SOURCES.txt
 cuscom.egg-info/dependency_links.txt
 cuscom.egg-info/requires.txt
 cuscom.egg-info/top_level.txt
 docs/source/description.rst
```

### Comparing `cuscom-0.2.7/setup.py` & `cuscom-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,13 +33,13 @@
     package_dir={"cuscom": "src/cuscom"},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
     ],
-    install_requires=["apache-airflow[kubernetes, slack]>=1.10.12"],
+    install_requires=["apache-airflow[kubernetes, slack]>=2.0.0"],
     data_files=[(".", ["VERSION"])],
     setup_requires=["pytest-runner"],
     tests_require=["pytest>=4"],
     packages=setuptools.find_packages("src"),
 )
```

### Comparing `cuscom-0.2.7/src/cuscom/clients/base_client.py` & `cuscom-1.0.0/src/cuscom/clients/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         return f"<{self.__class__.__name__}({self.status_code, self.body})>"
 
 
 class Client:
     def __init__(self, base_url):
         self._base_url = base_url
 
-    def request(self, endpoint, method, params=None):
+    def request(self, endpoint, method, **kwargs):
         url = join_url(self._base_url, endpoint)
-        response = requests.api.request(method=method, url=url, params=params)
+        response = requests.api.request(method=method, url=url, **kwargs)
 
         if response.status_code not in [200]:
             raise ClientException.from_response(response, url)
 
         return response.json(object_hook=from_kebab_case_key)
 
     def __repr__(self):
```

### Comparing `cuscom-0.2.7/src/cuscom/clients/task_client.py` & `cuscom-1.0.0/src/cuscom/clients/task_client.py`

 * *Files identical despite different names*

### Comparing `cuscom-0.2.7/src/cuscom/hooks/slack.py` & `cuscom-1.0.0/src/cuscom/hooks/slack.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 from typing import Any, Dict, Optional
 
-from airflow.contrib.operators.slack_webhook_operator import SlackWebhookOperator
-from airflow.models import Connection
-from airflow.hooks.base_hook import BaseHook
-from airflow.models import Variable
+from airflow.providers.slack.operators.slack_webhook import SlackWebhookOperator
+from airflow.models import Connection, Variable
+from airflow.hooks.base import BaseHook
 
 from cuscom.utils import flatten_dict, mask
 from cuscom.exceptions import CuscomException
 
 
 def on_failure(connection: Optional[Connection] = None, msg_template: Optional[str] = None):
     connection = connection or BaseHook.get_connection("slack")
```

### Comparing `cuscom-0.2.7/src/cuscom/operators/custom_kubernetes_pod_operator.py` & `cuscom-1.0.0/src/cuscom/operators/custom_kubernetes_pod_operator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import Any, Dict, List, Optional
 
-from airflow.contrib.operators.kubernetes_pod_operator import KubernetesPodOperator
+from airflow.providers.cncf.kubernetes.operators.kubernetes_pod import KubernetesPodOperator
 from cuscom.hooks import slack
 from cuscom.utils import default_arguments_fn, mask
 
 
 log = logging.getLogger(__name__)
```

### Comparing `cuscom-0.2.7/src/cuscom/utils.py` & `cuscom-1.0.0/src/cuscom/utils.py`

 * *Files identical despite different names*

