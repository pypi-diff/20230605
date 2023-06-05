# Comparing `tmp/mypy-boto3-kms-1.26.25.tar.gz` & `tmp/mypy-boto3-kms-1.26.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kms-1.26.25.tar", last modified: Wed Dec  7 20:47:12 2022, max compression
+gzip compressed data, was "mypy-boto3-kms-1.26.81.tar", last modified: Tue Feb 28 20:28:07 2023, max compression
```

## Comparing `mypy-boto3-kms-1.26.25.tar` & `mypy-boto3-kms-1.26.81.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 20:47:12.005179 mypy-boto3-kms-1.26.25/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-07 20:47:02.000000 mypy-boto3-kms-1.26.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2022-12-07 20:47:12.005179 mypy-boto3-kms-1.26.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16291 2022-12-07 20:47:02.000000 mypy-boto3-kms-1.26.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 20:47:12.005179 mypy-boto3-kms-1.26.25/mypy_boto3_kms/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2022-12-07 20:47:03.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2022-12-07 20:47:02.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      892 2022-12-07 20:47:03.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40515 2022-12-07 20:47:03.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40451 2022-12-07 20:47:03.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2022-12-07 20:47:03.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2022-12-07 20:47:03.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2022-12-07 20:47:03.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2022-12-07 20:47:03.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 20:47:03.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39683 2022-12-07 20:47:04.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39624 2022-12-07 20:47:03.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-07 20:47:02.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 20:47:12.005179 mypy-boto3-kms-1.26.25/mypy_boto3_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2022-12-07 20:47:11.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2022-12-07 20:47:11.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 20:47:11.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 20:47:11.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-07 20:47:11.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-07 20:47:11.000000 mypy-boto3-kms-1.26.25/mypy_boto3_kms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-07 20:47:12.005179 mypy-boto3-kms-1.26.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2022-12-07 20:47:02.000000 mypy-boto3-kms-1.26.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.526319 mypy-boto3-kms-1.26.81/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-02-28 20:28:07.526319 mypy-boto3-kms-1.26.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16290 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.522319 mypy-boto3-kms-1.26.81/mypy_boto3_kms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40515 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40451 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39683 2023-02-28 20:27:45.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39624 2023-02-28 20:27:45.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.526319 mypy-boto3-kms-1.26.81/mypy_boto3_kms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-02-28 20:28:07.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-28 20:28:07.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-28 20:28:07.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 20:28:07.000000 mypy-boto3-kms-1.26.81/mypy_boto3_kms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 20:28:07.526319 mypy-boto3-kms-1.26.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-28 20:27:44.000000 mypy-boto3-kms-1.26.81/setup.py
```

### Comparing `mypy-boto3-kms-1.26.25/LICENSE` & `mypy-boto3-kms-1.26.81/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.26.25/PKG-INFO` & `mypy-boto3-kms-1.26.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.26.25
-Summary: Type annotations for boto3.KMS 1.26.25 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.81
+Summary: Type annotations for boto3.KMS 1.26.81 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.26.25](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kms-1.26.25/README.md` & `mypy-boto3-kms-1.26.81/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.26.25](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/__init__.py` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/__init__.pyi` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/__main__.py` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KMS 1.26.25\nVersion:         1.26.25\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.KMS 1.26.81\nVersion:         1.26.81\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.25")
+    print("1.26.81")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/client.py` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/client.pyi` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/literals.py` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,24 +221,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -324,14 +326,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -346,30 +349,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -455,14 +461,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -496,14 +503,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -545,14 +553,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/literals.pyi` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -219,24 +219,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -322,14 +324,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -344,30 +347,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -453,14 +459,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -494,14 +501,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -543,14 +551,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/paginator.py` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/paginator.pyi` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/type_defs.py` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms/type_defs.pyi` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms.egg-info/PKG-INFO` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.26.25
-Summary: Type annotations for boto3.KMS 1.26.25 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.81
+Summary: Type annotations for boto3.KMS 1.26.81 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.26.25](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kms-1.26.25/mypy_boto3_kms.egg-info/SOURCES.txt` & `mypy-boto3-kms-1.26.81/mypy_boto3_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.26.25/setup.py` & `mypy-boto3-kms-1.26.81/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-kms",
-    version="1.26.25",
+    version="1.26.81",
     packages=["mypy_boto3_kms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KMS 1.26.25 service generated with mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.KMS 1.26.81 service generated with mypy-boto3-builder 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 kms type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_kms": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_kms": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

