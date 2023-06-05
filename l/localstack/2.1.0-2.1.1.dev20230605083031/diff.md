# Comparing `tmp/localstack-2.1.0.tar.gz` & `tmp/localstack-2.1.1.dev20230605083031.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-2.1.0.tar", last modified: Thu May 25 10:11:40 2023, max compression
+gzip compressed data, was "localstack-2.1.1.dev20230605083031.tar", last modified: Mon Jun  5 08:33:37 2023, max compression
```

## Comparing `localstack-2.1.0.tar` & `localstack-2.1.1.dev20230605083031.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-25 10:11:40.877507 localstack-2.1.0/
--rw-rw-r--   0 runner    (1000) runner    (1001)    11400 2023-05-25 10:11:40.877507 localstack-2.1.0/PKG-INFO
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-25 10:11:40.877507 localstack-2.1.0/localstack.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)    11400 2023-05-25 10:11:40.000000 localstack-2.1.0/localstack.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-05-25 10:11:40.000000 localstack-2.1.0/localstack.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-05-25 10:11:40.000000 localstack-2.1.0/localstack.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)      169 2023-05-25 10:11:40.000000 localstack-2.1.0/localstack.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-05-25 10:11:40.000000 localstack-2.1.0/localstack.egg-info/top_level.txt
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-25 10:11:40.877507 localstack-2.1.0/localstack_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)       50 2023-05-25 10:11:40.000000 localstack-2.1.0/localstack_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-05-25 10:11:40.877507 localstack-2.1.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-05-25 10:08:10.000000 localstack-2.1.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-05 08:33:37.209971 localstack-2.1.1.dev20230605083031/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    11394 2023-06-05 08:33:37.209971 localstack-2.1.1.dev20230605083031/PKG-INFO
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-05 08:33:37.209971 localstack-2.1.1.dev20230605083031/localstack.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    11394 2023-06-05 08:33:37.000000 localstack-2.1.1.dev20230605083031/localstack.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-06-05 08:33:37.000000 localstack-2.1.1.dev20230605083031/localstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-06-05 08:33:37.000000 localstack-2.1.1.dev20230605083031/localstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)      223 2023-06-05 08:33:37.000000 localstack-2.1.1.dev20230605083031/localstack.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-06-05 08:33:37.000000 localstack-2.1.1.dev20230605083031/localstack.egg-info/top_level.txt
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-05 08:33:37.209971 localstack-2.1.1.dev20230605083031/localstack_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-06-05 08:33:36.000000 localstack-2.1.1.dev20230605083031/localstack_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-06-05 08:33:37.209971 localstack-2.1.1.dev20230605083031/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-06-05 08:30:17.000000 localstack-2.1.1.dev20230605083031/setup.py
```

### Comparing `localstack-2.1.0/PKG-INFO` & `localstack-2.1.1.dev20230605083031/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.1.0
+Version: 2.1.1.dev20230605083031
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Emulators
 Description-Content-Type: text/markdown
 Provides-Extra: runtime
 Provides-Extra: full
 
 <p align="center">
-:zap: We are thrilled to announce <a href="https://localstack.cloud/blog/2023-03-29-announcing-localstack-2.0-general-availability/">LocalStack 2.0</a> which brings new features, enhancements and bugfixes :zap:
+:zap: We are thrilled to announce <a href="https://discuss.localstack.cloud/t/localstack-release-v2-1-0/357">LocalStack 2.1</a> which brings new features, enhancements and bugfixes :zap:
 </p>
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/localstack/localstack/master/doc/localstack-readme-banner.svg" alt="LocalStack - A fully functional local cloud stack">
 </p>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.1.0 Summary: LocalStack - A
-fully functional local Cloud stack Home-page: https://github.com/localstack/
-localstack Author: LocalStack Contributors Author-email: info@localstack.cloud
-License: Apache License 2.0 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Topic :: Internet Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Emulators Description-Content-Type: text/
-markdown Provides-Extra: runtime Provides-Extra: full
-  :zap: We are thrilled to announce LocalStack_2.0 which brings new features,
+Metadata-Version: 2.1 Name: localstack Version: 2.1.1.dev20230605083031
+Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
+github.com/localstack/localstack Author: LocalStack Contributors Author-email:
+info@localstack.cloud License: Apache License 2.0 Classifier: Programming
+Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Topic :: Internet Classifier: Topic :: Software
+Development :: Testing Classifier: Topic :: System :: Emulators Description-
+Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
+  :zap: We are thrilled to announce LocalStack_2.1 which brings new features,
                         enhancements and bugfixes :zap:
               [LocalStack - A fully functional local cloud stack]
  [CircleCI] [Coverage_Status] [PyPI_Version] [Docker_Pulls] [PyPi_downloads]
 [Backers_on_Open_Collective] [Sponsors_on_Open_Collective] [PyPI_License] [Code
                             style:_black] [Twitter]
 LocalStack provides an easy-to-use test/mocking framework for developing cloud
                                  applications.
```

### Comparing `localstack-2.1.0/localstack.egg-info/PKG-INFO` & `localstack-2.1.1.dev20230605083031/localstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.1.0
+Version: 2.1.1.dev20230605083031
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Emulators
 Description-Content-Type: text/markdown
 Provides-Extra: runtime
 Provides-Extra: full
 
 <p align="center">
-:zap: We are thrilled to announce <a href="https://localstack.cloud/blog/2023-03-29-announcing-localstack-2.0-general-availability/">LocalStack 2.0</a> which brings new features, enhancements and bugfixes :zap:
+:zap: We are thrilled to announce <a href="https://discuss.localstack.cloud/t/localstack-release-v2-1-0/357">LocalStack 2.1</a> which brings new features, enhancements and bugfixes :zap:
 </p>
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/localstack/localstack/master/doc/localstack-readme-banner.svg" alt="LocalStack - A fully functional local cloud stack">
 </p>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.1.0 Summary: LocalStack - A
-fully functional local Cloud stack Home-page: https://github.com/localstack/
-localstack Author: LocalStack Contributors Author-email: info@localstack.cloud
-License: Apache License 2.0 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Topic :: Internet Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Emulators Description-Content-Type: text/
-markdown Provides-Extra: runtime Provides-Extra: full
-  :zap: We are thrilled to announce LocalStack_2.0 which brings new features,
+Metadata-Version: 2.1 Name: localstack Version: 2.1.1.dev20230605083031
+Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
+github.com/localstack/localstack Author: LocalStack Contributors Author-email:
+info@localstack.cloud License: Apache License 2.0 Classifier: Programming
+Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Topic :: Internet Classifier: Topic :: Software
+Development :: Testing Classifier: Topic :: System :: Emulators Description-
+Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
+  :zap: We are thrilled to announce LocalStack_2.1 which brings new features,
                         enhancements and bugfixes :zap:
               [LocalStack - A fully functional local cloud stack]
  [CircleCI] [Coverage_Status] [PyPI_Version] [Docker_Pulls] [PyPi_downloads]
 [Backers_on_Open_Collective] [Sponsors_on_Open_Collective] [PyPI_License] [Code
                             style:_black] [Twitter]
 LocalStack provides an easy-to-use test/mocking framework for developing cloud
                                  applications.
```

### Comparing `localstack-2.1.0/setup.py` & `localstack-2.1.1.dev20230605083031/setup.py`

 * *Files identical despite different names*

