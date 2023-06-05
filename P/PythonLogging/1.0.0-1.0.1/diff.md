# Comparing `tmp/PythonLogging-1.0.0.tar.gz` & `tmp/PythonLogging-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonLogging-1.0.0.tar", last modified: Mon Jun  5 16:01:07 2023, max compression
+gzip compressed data, was "PythonLogging-1.0.1.tar", last modified: Mon Jun  5 16:02:25 2023, max compression
```

## Comparing `PythonLogging-1.0.0.tar` & `PythonLogging-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:07.685479 PythonLogging-1.0.0/
--rw-rw-rw-   0        0        0     1960 2023-06-05 16:01:07.684476 PythonLogging-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:07.662447 PythonLogging-1.0.0/PythonLogging/
--rw-rw-rw-   0        0        0     1591 2023-06-05 16:00:50.000000 PythonLogging-1.0.0/PythonLogging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:01:07.683473 PythonLogging-1.0.0/PythonLogging.egg-info/
--rw-rw-rw-   0        0        0     1960 2023-06-05 16:01:07.000000 PythonLogging-1.0.0/PythonLogging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-05 16:01:07.000000 PythonLogging-1.0.0/PythonLogging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:01:07.000000 PythonLogging-1.0.0/PythonLogging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-05 16:01:07.000000 PythonLogging-1.0.0/PythonLogging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1545 2023-06-05 15:58:57.000000 PythonLogging-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 16:01:07.685479 PythonLogging-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-06-05 16:00:14.000000 PythonLogging-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:02:25.691034 PythonLogging-1.0.1/
+-rw-rw-rw-   0        0        0     1956 2023-06-05 16:02:25.690028 PythonLogging-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 16:02:25.675096 PythonLogging-1.0.1/PythonLogging/
+-rw-rw-rw-   0        0        0     1591 2023-06-05 16:00:50.000000 PythonLogging-1.0.1/PythonLogging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:02:25.688069 PythonLogging-1.0.1/PythonLogging.egg-info/
+-rw-rw-rw-   0        0        0     1956 2023-06-05 16:02:25.000000 PythonLogging-1.0.1/PythonLogging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-06-05 16:02:25.000000 PythonLogging-1.0.1/PythonLogging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:02:25.000000 PythonLogging-1.0.1/PythonLogging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-05 16:02:25.000000 PythonLogging-1.0.1/PythonLogging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1541 2023-06-05 16:02:04.000000 PythonLogging-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:02:25.691034 PythonLogging-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-06-05 16:02:21.000000 PythonLogging-1.0.1/setup.py
```

### Comparing `PythonLogging-1.0.0/PKG-INFO` & `PythonLogging-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonLogging
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple logging library for easy log file management
 Home-page: https://github.com/SForces/PythonLogging
 Author: Osman TUNA
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -37,18 +37,17 @@
     - None (no return value) if the log message is successfully written.
     - Error message if the log file path is not selected using `logfile_path()`.
 
 ## Installation
 
 You can install PythonLogging using pip:
 
+```bash
 pip install PythonLogging
-
-sql
-Copy code
+```
 
 ## Usage
 
 To use PythonLogging, you need to first specify the log file path using the `logfile_path()` function. You can provide a path pattern with date and time placeholders to create log files with dynamic names. For example:
 
 ```python
 import PythonLogging
```

### Comparing `PythonLogging-1.0.0/PythonLogging/__init__.py` & `PythonLogging-1.0.1/PythonLogging/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonLogging-1.0.0/PythonLogging.egg-info/PKG-INFO` & `PythonLogging-1.0.1/PythonLogging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonLogging
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple logging library for easy log file management
 Home-page: https://github.com/SForces/PythonLogging
 Author: Osman TUNA
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -37,18 +37,17 @@
     - None (no return value) if the log message is successfully written.
     - Error message if the log file path is not selected using `logfile_path()`.
 
 ## Installation
 
 You can install PythonLogging using pip:
 
+```bash
 pip install PythonLogging
-
-sql
-Copy code
+```
 
 ## Usage
 
 To use PythonLogging, you need to first specify the log file path using the `logfile_path()` function. You can provide a path pattern with date and time placeholders to create log files with dynamic names. For example:
 
 ```python
 import PythonLogging
```

### Comparing `PythonLogging-1.0.0/README.md` & `PythonLogging-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,18 +25,17 @@
     - None (no return value) if the log message is successfully written.
     - Error message if the log file path is not selected using `logfile_path()`.
 
 ## Installation
 
 You can install PythonLogging using pip:
 
+```bash
 pip install PythonLogging
-
-sql
-Copy code
+```
 
 ## Usage
 
 To use PythonLogging, you need to first specify the log file path using the `logfile_path()` function. You can provide a path pattern with date and time placeholders to create log files with dynamic names. For example:
 
 ```python
 import PythonLogging
```

### Comparing `PythonLogging-1.0.0/setup.py` & `PythonLogging-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PythonLogging",
-    version="1.0.0",
+    version="1.0.1",
     author="Osman TUNA",
     description="A simple logging library for easy log file management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SForces/PythonLogging",
     packages=["PythonLogging"],
     classifiers=[
```

