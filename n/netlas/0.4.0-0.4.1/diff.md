# Comparing `tmp/netlas-0.4.0.tar.gz` & `tmp/netlas-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlas-0.4.0.tar", last modified: Wed Dec  7 13:42:41 2022, max compression
+gzip compressed data, was "netlas-0.4.1.tar", last modified: Mon Jun  5 08:59:54 2023, max compression
```

## Comparing `netlas-0.4.0.tar` & `netlas-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-12-07 13:42:41.763483 netlas-0.4.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1242 2022-12-07 13:16:10.000000 netlas-0.4.0/CHANGELOG.md
--rw-r--r--   0 user      (1000) user      (1000)     1062 2022-11-25 12:28:45.000000 netlas-0.4.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      102 2022-11-25 12:28:45.000000 netlas-0.4.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3299 2022-12-07 13:42:41.763483 netlas-0.4.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2853 2022-12-07 13:03:53.000000 netlas-0.4.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-12-07 13:42:41.759483 netlas-0.4.0/docs/
--rw-r--r--   0 user      (1000) user      (1000)      634 2022-11-25 12:28:47.000000 netlas-0.4.0/docs/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     2461 2022-12-07 13:03:53.000000 netlas-0.4.0/docs/conf.py
--rw-rw-r--   0 user      (1000) user      (1000)     3028 2022-12-07 13:03:53.000000 netlas-0.4.0/docs/getting_started.rst
--rw-r--r--   0 user      (1000) user      (1000)      244 2022-11-25 12:28:47.000000 netlas-0.4.0/docs/index.rst
--rw-r--r--   0 user      (1000) user      (1000)      795 2022-11-25 12:28:47.000000 netlas-0.4.0/docs/make.bat
--rw-r--r--   0 user      (1000) user      (1000)      264 2022-11-25 12:28:47.000000 netlas-0.4.0/docs/netlas.rst
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-12-07 13:42:41.759483 netlas-0.4.0/netlas/
--rw-r--r--   0 user      (1000) user      (1000)       71 2022-11-25 12:28:47.000000 netlas-0.4.0/netlas/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    12115 2022-12-07 13:03:53.000000 netlas-0.4.0/netlas/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)    10871 2022-12-07 13:03:53.000000 netlas-0.4.0/netlas/client.py
--rw-r--r--   0 user      (1000) user      (1000)      177 2022-11-25 12:28:47.000000 netlas-0.4.0/netlas/exception.py
--rw-rw-r--   0 user      (1000) user      (1000)     5667 2022-12-07 13:03:53.000000 netlas-0.4.0/netlas/helpers.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-12-07 13:42:41.763483 netlas-0.4.0/netlas.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3299 2022-12-07 13:42:41.000000 netlas-0.4.0/netlas.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      440 2022-12-07 13:42:41.000000 netlas-0.4.0/netlas.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-12-07 13:42:41.000000 netlas-0.4.0/netlas.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       48 2022-12-07 13:42:41.000000 netlas-0.4.0/netlas.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)      106 2022-12-07 13:42:41.000000 netlas-0.4.0/netlas.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2022-12-07 13:42:41.000000 netlas-0.4.0/netlas.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)      105 2022-11-25 12:28:45.000000 netlas-0.4.0/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-12-07 13:42:41.763483 netlas-0.4.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      871 2022-12-07 13:12:11.000000 netlas-0.4.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-05 08:59:54.604099 netlas-0.4.1/
+-rw-rw-r--   0 user      (1000) user      (1000)     1242 2022-12-07 13:16:10.000000 netlas-0.4.1/CHANGELOG.md
+-rw-r--r--   0 user      (1000) user      (1000)     1062 2022-11-25 12:28:45.000000 netlas-0.4.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      102 2022-11-25 12:28:45.000000 netlas-0.4.1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3495 2023-06-05 08:59:54.604099 netlas-0.4.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3049 2023-06-05 08:53:21.000000 netlas-0.4.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-05 08:59:54.600099 netlas-0.4.1/docs/
+-rw-r--r--   0 user      (1000) user      (1000)      634 2022-11-25 12:28:47.000000 netlas-0.4.1/docs/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     2461 2022-12-07 13:03:53.000000 netlas-0.4.1/docs/conf.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3218 2023-06-05 08:54:45.000000 netlas-0.4.1/docs/getting_started.rst
+-rw-r--r--   0 user      (1000) user      (1000)      244 2022-11-25 12:28:47.000000 netlas-0.4.1/docs/index.rst
+-rw-r--r--   0 user      (1000) user      (1000)      795 2022-11-25 12:28:47.000000 netlas-0.4.1/docs/make.bat
+-rw-r--r--   0 user      (1000) user      (1000)      264 2022-11-25 12:28:47.000000 netlas-0.4.1/docs/netlas.rst
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-05 08:59:54.604099 netlas-0.4.1/netlas/
+-rw-r--r--   0 user      (1000) user      (1000)       71 2022-11-25 12:28:47.000000 netlas-0.4.1/netlas/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12115 2022-12-07 13:03:53.000000 netlas-0.4.1/netlas/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10871 2022-12-07 13:03:53.000000 netlas-0.4.1/netlas/client.py
+-rw-r--r--   0 user      (1000) user      (1000)      177 2022-11-25 12:28:47.000000 netlas-0.4.1/netlas/exception.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5667 2022-12-07 13:03:53.000000 netlas-0.4.1/netlas/helpers.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-05 08:59:54.604099 netlas-0.4.1/netlas.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3495 2023-06-05 08:59:54.000000 netlas-0.4.1/netlas.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      440 2023-06-05 08:59:54.000000 netlas-0.4.1/netlas.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-05 08:59:54.000000 netlas-0.4.1/netlas.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       48 2023-06-05 08:59:54.000000 netlas-0.4.1/netlas.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)      106 2023-06-05 08:59:54.000000 netlas-0.4.1/netlas.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-06-05 08:59:54.000000 netlas-0.4.1/netlas.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)      105 2023-06-05 08:38:11.000000 netlas-0.4.1/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-05 08:59:54.604099 netlas-0.4.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      871 2023-06-05 08:43:28.000000 netlas-0.4.1/setup.py
```

### Comparing `netlas-0.4.0/CHANGELOG.md` & `netlas-0.4.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `netlas-0.4.0/LICENSE` & `netlas-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netlas-0.4.0/PKG-INFO` & `netlas-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlas
-Version: 0.4.0
+Version: 0.4.1
 Summary: Netlas.io API package
 Home-page: https://github.com/netlas-io/netlas-python
 Author: Netlas Team
 Author-email: support@netlas.io
 Keywords: security,network
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -102,7 +102,19 @@
 -e, --exclude TEXT              Specify comma-separated fields that will be
                                 excluded from the output NOTE: This argument
                                 is mutually exclusive with  arguments:
                                 [include, -i].
 -p, --page INTEGER              Specify data page  [default: 0]
 -h, --help                      Show this message and exit.
 ```
+
+## Bootstraping
+
+You may want to registry your API key.
+
+```
+netlas query savekey YOUR_API_KEY
+```
+netlas as now saved your key, you can now use the CLI as such:
+```
+netlas query 'THE_QUERY'
+```
```

### Comparing `netlas-0.4.0/README.md` & `netlas-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -87,7 +87,19 @@
 -e, --exclude TEXT              Specify comma-separated fields that will be
                                 excluded from the output NOTE: This argument
                                 is mutually exclusive with  arguments:
                                 [include, -i].
 -p, --page INTEGER              Specify data page  [default: 0]
 -h, --help                      Show this message and exit.
 ```
+
+## Bootstraping
+
+You may want to registry your API key.
+
+```
+netlas query savekey YOUR_API_KEY
+```
+netlas as now saved your key, you can now use the CLI as such:
+```
+netlas query 'THE_QUERY'
+```
```

### Comparing `netlas-0.4.0/docs/Makefile` & `netlas-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `netlas-0.4.0/docs/conf.py` & `netlas-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `netlas-0.4.0/docs/getting_started.rst` & `netlas-0.4.1/docs/getting_started.rst`

 * *Files 7% similar despite different names*

```diff
@@ -91,8 +91,24 @@
                                     mutually exclusive with  arguments: [-e,
                                     exclude].
     -e, --exclude TEXT              Specify comma-separated fields that will be
                                     excluded from the output NOTE: This argument
                                     is mutually exclusive with  arguments:
                                     [include, -i].
     -p, --page INTEGER              Specify data page  [default: 0]
-    -h, --help                      Show this message and exit.
+    
+
+Bootstraping:
+------------
+  
+You may want to registry your API key. 
+
+.. code-block:: bash
+
+    netlas query savekey YOUR_API_KEY
+
+
+netlas as now saved your key, you can now use the CLI as such:
+
+.. code-block:: bash
+
+    netlas query 'THE_QUERY'
```

### Comparing `netlas-0.4.0/docs/make.bat` & `netlas-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `netlas-0.4.0/netlas/__main__.py` & `netlas-0.4.1/netlas/__main__.py`

 * *Files identical despite different names*

### Comparing `netlas-0.4.0/netlas/client.py` & `netlas-0.4.1/netlas/client.py`

 * *Files identical despite different names*

### Comparing `netlas-0.4.0/netlas/helpers.py` & `netlas-0.4.1/netlas/helpers.py`

 * *Files identical despite different names*

### Comparing `netlas-0.4.0/netlas.egg-info/PKG-INFO` & `netlas-0.4.1/netlas.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlas
-Version: 0.4.0
+Version: 0.4.1
 Summary: Netlas.io API package
 Home-page: https://github.com/netlas-io/netlas-python
 Author: Netlas Team
 Author-email: support@netlas.io
 Keywords: security,network
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -102,7 +102,19 @@
 -e, --exclude TEXT              Specify comma-separated fields that will be
                                 excluded from the output NOTE: This argument
                                 is mutually exclusive with  arguments:
                                 [include, -i].
 -p, --page INTEGER              Specify data page  [default: 0]
 -h, --help                      Show this message and exit.
 ```
+
+## Bootstraping
+
+You may want to registry your API key.
+
+```
+netlas query savekey YOUR_API_KEY
+```
+netlas as now saved your key, you can now use the CLI as such:
+```
+netlas query 'THE_QUERY'
+```
```

### Comparing `netlas-0.4.0/setup.py` & `netlas-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 DEPENDENCIES = open("requirements.txt", "r").read().split("\n")
 
 setup(
     name="netlas",
-    version="0.4.0",
+    version="0.4.1",
     author="Netlas Team",
     author_email="support@netlas.io",
     description="Netlas.io API package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/netlas-io/netlas-python",
     packages=["netlas"],
```

