# Comparing `tmp/classwork-0.0.6.tar.gz` & `tmp/classwork-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classwork-0.0.6.tar", max compression
+gzip compressed data, was "classwork-0.0.7.tar", max compression
```

## Comparing `classwork-0.0.6.tar` & `classwork-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-06-03 17:09:04.784909 classwork-0.0.6/LICENSE.md
--rw-r--r--   0        0        0     4534 2023-06-05 02:18:46.252572 classwork-0.0.6/README.md
--rw-r--r--   0        0        0      161 2023-06-03 15:43:24.017838 classwork-0.0.6/classwork/__init__.py
--rw-r--r--   0        0        0    12765 2023-06-05 02:11:06.603814 classwork-0.0.6/classwork/main.py
--rw-r--r--   0        0        0     3700 2023-06-05 02:11:24.504052 classwork-0.0.6/classwork/utils.py
--rw-r--r--   0        0        0      473 2023-06-05 01:11:15.309982 classwork-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5306 1970-01-01 00:00:00.000000 classwork-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-03 17:09:04.784909 classwork-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0     4534 2023-06-05 02:18:46.252572 classwork-0.0.7/README.md
+-rw-r--r--   0        0        0      161 2023-06-03 15:43:24.017838 classwork-0.0.7/classwork/__init__.py
+-rw-r--r--   0        0        0    12765 2023-06-05 02:11:06.603814 classwork-0.0.7/classwork/main.py
+-rw-r--r--   0        0        0     3700 2023-06-05 02:11:24.504052 classwork-0.0.7/classwork/utils.py
+-rw-r--r--   0        0        0      474 2023-06-05 02:27:36.212063 classwork-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 classwork-0.0.7/PKG-INFO
```

### Comparing `classwork-0.0.6/LICENSE.md` & `classwork-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `classwork-0.0.6/README.md` & `classwork-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `classwork-0.0.6/classwork/main.py` & `classwork-0.0.7/classwork/main.py`

 * *Files identical despite different names*

### Comparing `classwork-0.0.6/classwork/utils.py` & `classwork-0.0.7/classwork/utils.py`

 * *Files identical despite different names*

### Comparing `classwork-0.0.6/PKG-INFO` & `classwork-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: classwork
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple Python module to help distribute you tasks across multiple brokers as microservices
 License: MIT
 Author: Anthony Mugendi
 Author-email: ngurumugz@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hashids (==1.3.1)
 Requires-Dist: nats-py (==2.2.0)
-Requires-Dist: numpy (==1.23.5)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: termcolor2 (>=0.0.3,<0.0.4)
 Requires-Dist: typjson (==0.0.32)
 Description-Content-Type: text/markdown
 
 <!--
  Copyright (c) 2023 Anthony Mugendi
```

