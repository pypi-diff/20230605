# Comparing `tmp/cdk-monitoring-constructs-5.0.0.tar.gz` & `tmp/cdk-monitoring-constructs-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-monitoring-constructs-5.0.0.tar", last modified: Thu Jun  1 19:23:37 2023, max compression
+gzip compressed data, was "cdk-monitoring-constructs-5.0.1.tar", last modified: Mon Jun  5 00:36:19 2023, max compression
```

## Comparing `cdk-monitoring-constructs-5.0.0.tar` & `cdk-monitoring-constructs-5.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:23:37.519716 cdk-monitoring-constructs-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-01 19:23:24.000000 cdk-monitoring-constructs-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 19:23:24.000000 cdk-monitoring-constructs-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 19:23:24.000000 cdk-monitoring-constructs-5.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-06-01 19:23:37.519716 cdk-monitoring-constructs-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-06-01 19:23:24.000000 cdk-monitoring-constructs-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 19:23:24.000000 cdk-monitoring-constructs-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:23:37.519716 cdk-monitoring-constructs-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-01 19:23:24.000000 cdk-monitoring-constructs-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:23:37.511716 cdk-monitoring-constructs-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:23:37.519716 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)  4427361 2023-06-01 19:23:24.000000 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:23:37.519716 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-01 19:23:24.000000 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   771731 2023-06-01 19:23:24.000000 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.0.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:23:24.000000 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:23:37.519716 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-06-01 19:23:37.000000 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-01 19:23:37.000000 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:23:37.000000 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-01 19:23:37.000000 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 19:23:37.000000 cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:36:19.433925 cdk-monitoring-constructs-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-05 00:36:08.000000 cdk-monitoring-constructs-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 00:36:08.000000 cdk-monitoring-constructs-5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 00:36:08.000000 cdk-monitoring-constructs-5.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-06-05 00:36:19.433925 cdk-monitoring-constructs-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-06-05 00:36:08.000000 cdk-monitoring-constructs-5.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-05 00:36:08.000000 cdk-monitoring-constructs-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 00:36:19.433925 cdk-monitoring-constructs-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-05 00:36:08.000000 cdk-monitoring-constructs-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:36:19.425924 cdk-monitoring-constructs-5.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:36:19.429924 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)  4427361 2023-06-05 00:36:08.000000 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:36:19.429924 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-05 00:36:08.000000 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   771726 2023-06-05 00:36:08.000000 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.0.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 00:36:08.000000 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:36:19.429924 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-06-05 00:36:19.000000 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-05 00:36:19.000000 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 00:36:19.000000 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-05 00:36:19.000000 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 00:36:19.000000 cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs.egg-info/top_level.txt
```

### Comparing `cdk-monitoring-constructs-5.0.0/LICENSE` & `cdk-monitoring-constructs-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-5.0.0/PKG-INFO` & `cdk-monitoring-constructs-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-monitoring-constructs
-Version: 5.0.0
+Version: 5.0.1
 Summary: cdk-monitoring-constructs
 Home-page: https://github.com/cdklabs/cdk-monitoring-constructs
 Author: CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-monitoring-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -46,15 +46,15 @@
 > https://www.npmjs.com/package/cdk-monitoring-constructs
 
 In your `package.json`:
 
 ```json
 {
   "dependencies": {
-    "cdk-monitoring-constructs": "^4.0.0",
+    "cdk-monitoring-constructs": "^5.0.0",
 
     // peer dependencies of cdk-monitoring-constructs
     "@aws-cdk/aws-apigatewayv2-alpha": "^2.65.0-alpha.0",
     "@aws-cdk/aws-redshift-alpha": "^2.65.0-alpha.0",
     "@aws-cdk/aws-synthetics-alpha": "^2.65.0-alpha.0",
     "aws-cdk-lib": "^2.65.0",
     "constructs": "^10.0.5"
```

### Comparing `cdk-monitoring-constructs-5.0.0/README.md` & `cdk-monitoring-constructs-5.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 > https://www.npmjs.com/package/cdk-monitoring-constructs
 
 In your `package.json`:
 
 ```json
 {
   "dependencies": {
-    "cdk-monitoring-constructs": "^4.0.0",
+    "cdk-monitoring-constructs": "^5.0.0",
 
     // peer dependencies of cdk-monitoring-constructs
     "@aws-cdk/aws-apigatewayv2-alpha": "^2.65.0-alpha.0",
     "@aws-cdk/aws-redshift-alpha": "^2.65.0-alpha.0",
     "@aws-cdk/aws-synthetics-alpha": "^2.65.0-alpha.0",
     "aws-cdk-lib": "^2.65.0",
     "constructs": "^10.0.5"
```

### Comparing `cdk-monitoring-constructs-5.0.0/setup.py` & `cdk-monitoring-constructs-5.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-monitoring-constructs",
-    "version": "5.0.0",
+    "version": "5.0.1",
     "description": "cdk-monitoring-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-monitoring-constructs",
     "long_description_content_type": "text/markdown",
     "author": "CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_monitoring_constructs",
         "cdk_monitoring_constructs._jsii"
     ],
     "package_data": {
         "cdk_monitoring_constructs._jsii": [
-            "cdk-monitoring-constructs@5.0.0.jsii.tgz"
+            "cdk-monitoring-constructs@5.0.1.jsii.tgz"
         ],
         "cdk_monitoring_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs/__init__.py` & `cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 000005a0: 2d6d 6f6e 6974 6f72 696e 672d 636f 6e73  -monitoring-cons
 000005b0: 7472 7563 7473 0a0a 496e 2079 6f75 7220  tructs..In your 
 000005c0: 6070 6163 6b61 6765 2e6a 736f 6e60 3a0a  `package.json`:.
 000005d0: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 6465  .```json.{.  "de
 000005e0: 7065 6e64 656e 6369 6573 223a 207b 0a20  pendencies": {. 
 000005f0: 2020 2022 6364 6b2d 6d6f 6e69 746f 7269     "cdk-monitori
 00000600: 6e67 2d63 6f6e 7374 7275 6374 7322 3a20  ng-constructs": 
-00000610: 225e 342e 302e 3022 2c0a 0a20 2020 202f  "^4.0.0",..    /
+00000610: 225e 352e 302e 3022 2c0a 0a20 2020 202f  "^5.0.0",..    /
 00000620: 2f20 7065 6572 2064 6570 656e 6465 6e63  / peer dependenc
 00000630: 6965 7320 6f66 2063 646b 2d6d 6f6e 6974  ies of cdk-monit
 00000640: 6f72 696e 672d 636f 6e73 7472 7563 7473  oring-constructs
 00000650: 0a20 2020 2022 4061 7773 2d63 646b 2f61  .    "@aws-cdk/a
 00000660: 7773 2d61 7069 6761 7465 7761 7976 322d  ws-apigatewayv2-
 00000670: 616c 7068 6122 3a20 225e 322e 3635 2e30  alpha": "^2.65.0
 00000680: 2d61 6c70 6861 2e30 222c 0a20 2020 2022  -alpha.0",.    "
```

### Comparing `cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs/_jsii/__init__.py` & `cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_redshift_alpha._jsii
 import aws_cdk.aws_synthetics_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "cdk-monitoring-constructs",
-    "5.0.0",
+    "5.0.1",
     __name__[0:-6],
-    "cdk-monitoring-constructs@5.0.0.jsii.tgz",
+    "cdk-monitoring-constructs@5.0.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs.egg-info/PKG-INFO` & `cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-monitoring-constructs
-Version: 5.0.0
+Version: 5.0.1
 Summary: cdk-monitoring-constructs
 Home-page: https://github.com/cdklabs/cdk-monitoring-constructs
 Author: CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-monitoring-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -46,15 +46,15 @@
 > https://www.npmjs.com/package/cdk-monitoring-constructs
 
 In your `package.json`:
 
 ```json
 {
   "dependencies": {
-    "cdk-monitoring-constructs": "^4.0.0",
+    "cdk-monitoring-constructs": "^5.0.0",
 
     // peer dependencies of cdk-monitoring-constructs
     "@aws-cdk/aws-apigatewayv2-alpha": "^2.65.0-alpha.0",
     "@aws-cdk/aws-redshift-alpha": "^2.65.0-alpha.0",
     "@aws-cdk/aws-synthetics-alpha": "^2.65.0-alpha.0",
     "aws-cdk-lib": "^2.65.0",
     "constructs": "^10.0.5"
```

### Comparing `cdk-monitoring-constructs-5.0.0/src/cdk_monitoring_constructs.egg-info/SOURCES.txt` & `cdk-monitoring-constructs-5.0.1/src/cdk_monitoring_constructs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdk_monitoring_constructs/py.typed
 src/cdk_monitoring_constructs.egg-info/PKG-INFO
 src/cdk_monitoring_constructs.egg-info/SOURCES.txt
 src/cdk_monitoring_constructs.egg-info/dependency_links.txt
 src/cdk_monitoring_constructs.egg-info/requires.txt
 src/cdk_monitoring_constructs.egg-info/top_level.txt
 src/cdk_monitoring_constructs/_jsii/__init__.py
-src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.0.0.jsii.tgz
+src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.0.1.jsii.tgz
```

