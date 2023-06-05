# Comparing `tmp/vantiqsdk-1.1.2.tar.gz` & `tmp/vantiqsdk-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantiqsdk-1.1.2.tar", last modified: Thu Jun  9 23:39:32 2022, max compression
+gzip compressed data, was "vantiqsdk-1.1.3.tar", last modified: Mon Jun  5 19:39:11 2023, max compression
```

## Comparing `vantiqsdk-1.1.2.tar` & `vantiqsdk-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-06-09 23:39:32.009218 vantiqsdk-1.1.2/
--rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-05-09 21:51:11.000000 vantiqsdk-1.1.2/LICENSE.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       31 2022-05-09 21:51:11.000000 vantiqsdk-1.1.2/MANIFEST.in
--rw-r--r--   0 fcarter    (501) staff       (20)     5637 2022-06-09 23:39:32.009368 vantiqsdk-1.1.2/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)     4043 2022-06-09 23:38:56.000000 vantiqsdk-1.1.2/README.md
--rw-r--r--   0 fcarter    (501) staff       (20)      103 2022-05-09 21:51:11.000000 vantiqsdk-1.1.2/pyproject.toml
--rw-r--r--   0 fcarter    (501) staff       (20)      663 2022-06-09 23:39:32.010728 vantiqsdk-1.1.2/setup.cfg
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-06-09 23:39:32.000694 vantiqsdk-1.1.2/src/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-06-09 23:39:32.000812 vantiqsdk-1.1.2/src/main/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-06-09 23:39:32.003134 vantiqsdk-1.1.2/src/main/python/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2022-06-09 23:39:32.008811 vantiqsdk-1.1.2/src/main/python/vantiqsdk.egg-info/
--rw-r--r--   0 fcarter    (501) staff       (20)     5637 2022-06-09 23:39:31.000000 vantiqsdk-1.1.2/src/main/python/vantiqsdk.egg-info/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)      331 2022-06-09 23:39:31.000000 vantiqsdk-1.1.2/src/main/python/vantiqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 fcarter    (501) staff       (20)        1 2022-06-09 23:39:31.000000 vantiqsdk-1.1.2/src/main/python/vantiqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       30 2022-06-09 23:39:31.000000 vantiqsdk-1.1.2/src/main/python/vantiqsdk.egg-info/requires.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       10 2022-06-09 23:39:31.000000 vantiqsdk-1.1.2/src/main/python/vantiqsdk.egg-info/top_level.txt
--rw-r--r--   0 fcarter    (501) staff       (20)    64973 2022-05-25 22:06:45.000000 vantiqsdk-1.1.2/src/main/python/vantiqsdk.py
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2023-06-05 19:39:11.755235 vantiqsdk-1.1.3/
+-rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-05-09 21:51:11.000000 vantiqsdk-1.1.3/LICENSE.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       31 2022-05-09 21:51:11.000000 vantiqsdk-1.1.3/MANIFEST.in
+-rw-r--r--   0 fcarter    (501) staff       (20)     5728 2023-06-05 19:39:11.755381 vantiqsdk-1.1.3/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)     4134 2023-06-01 23:15:56.000000 vantiqsdk-1.1.3/README.md
+-rw-r--r--   0 fcarter    (501) staff       (20)      103 2022-05-09 21:51:11.000000 vantiqsdk-1.1.3/pyproject.toml
+-rw-r--r--   0 fcarter    (501) staff       (20)      663 2023-06-05 19:39:11.758949 vantiqsdk-1.1.3/setup.cfg
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2023-06-05 19:39:11.714578 vantiqsdk-1.1.3/src/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2023-06-05 19:39:11.714756 vantiqsdk-1.1.3/src/main/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2023-06-05 19:39:11.752368 vantiqsdk-1.1.3/src/main/python/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2023-06-05 19:39:11.754905 vantiqsdk-1.1.3/src/main/python/vantiqsdk.egg-info/
+-rw-r--r--   0 fcarter    (501) staff       (20)     5728 2023-06-05 19:39:11.000000 vantiqsdk-1.1.3/src/main/python/vantiqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)      331 2023-06-05 19:39:11.000000 vantiqsdk-1.1.3/src/main/python/vantiqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)        1 2023-06-05 19:39:11.000000 vantiqsdk-1.1.3/src/main/python/vantiqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       30 2023-06-05 19:39:11.000000 vantiqsdk-1.1.3/src/main/python/vantiqsdk.egg-info/requires.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       10 2023-06-05 19:39:11.000000 vantiqsdk-1.1.3/src/main/python/vantiqsdk.egg-info/top_level.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)    64973 2022-05-25 22:06:45.000000 vantiqsdk-1.1.3/src/main/python/vantiqsdk.py
```

### Comparing `vantiqsdk-1.1.2/LICENSE.txt` & `vantiqsdk-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vantiqsdk-1.1.2/PKG-INFO` & `vantiqsdk-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqsdk
-Version: 1.1.2
+Version: 1.1.3
 Summary: SDK for working with the Vantiq system
 Home-page: https://github.com/vantiq/vantiq-python-sdk
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -115,19 +115,19 @@
 ```commandline
 ./gradlew.bat test
 ```
 
 in a windows environment.
 
 The tests run will run a mocked version. To execute tests against a _live_ server,
-define the following gradle properties:
+define the following gradle properties in your ~/.gradle/gradle.properties file:
 
 ```properties
 # Python project values
-TestVantiqServer=<Vantiq server url>
+TestVantiqServer=<Vantiq server url> # Only do the base URL. Ex http://localhost:8080/
 TestAccessToken=<access token from that Vantiq system>
 TestVantiqUsername=<Vantiq user name>
 TestVantiqPassword=<Password for that Vantiq user>
 ```
 
 Alternatively, when running directly, use the following environment variables:
```

### Comparing `vantiqsdk-1.1.2/README.md` & `vantiqsdk-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -99,19 +99,19 @@
 ```commandline
 ./gradlew.bat test
 ```
 
 in a windows environment.
 
 The tests run will run a mocked version. To execute tests against a _live_ server,
-define the following gradle properties:
+define the following gradle properties in your ~/.gradle/gradle.properties file:
 
 ```properties
 # Python project values
-TestVantiqServer=<Vantiq server url>
+TestVantiqServer=<Vantiq server url> # Only do the base URL. Ex http://localhost:8080/
 TestAccessToken=<access token from that Vantiq system>
 TestVantiqUsername=<Vantiq user name>
 TestVantiqPassword=<Password for that Vantiq user>
 ```
 
 Alternatively, when running directly, use the following environment variables:
```

### Comparing `vantiqsdk-1.1.2/setup.cfg` & `vantiqsdk-1.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vantiqsdk
-version = 1.1.2
+version = 1.1.3
 description = SDK for working with the Vantiq system
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/vantiq/vantiq-python-sdk
 author = Vantiq, Inc
 author_email = fcarter@vantiq.com
 license = MIT
```

### Comparing `vantiqsdk-1.1.2/src/main/python/vantiqsdk.egg-info/PKG-INFO` & `vantiqsdk-1.1.3/src/main/python/vantiqsdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqsdk
-Version: 1.1.2
+Version: 1.1.3
 Summary: SDK for working with the Vantiq system
 Home-page: https://github.com/vantiq/vantiq-python-sdk
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -115,19 +115,19 @@
 ```commandline
 ./gradlew.bat test
 ```
 
 in a windows environment.
 
 The tests run will run a mocked version. To execute tests against a _live_ server,
-define the following gradle properties:
+define the following gradle properties in your ~/.gradle/gradle.properties file:
 
 ```properties
 # Python project values
-TestVantiqServer=<Vantiq server url>
+TestVantiqServer=<Vantiq server url> # Only do the base URL. Ex http://localhost:8080/
 TestAccessToken=<access token from that Vantiq system>
 TestVantiqUsername=<Vantiq user name>
 TestVantiqPassword=<Password for that Vantiq user>
 ```
 
 Alternatively, when running directly, use the following environment variables:
```

### Comparing `vantiqsdk-1.1.2/src/main/python/vantiqsdk.py` & `vantiqsdk-1.1.3/src/main/python/vantiqsdk.py`

 * *Files identical despite different names*

