# Comparing `tmp/PythonLogging-1.0.1.tar.gz` & `tmp/PythonLogging-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonLogging-1.0.1.tar", last modified: Mon Jun  5 16:02:25 2023, max compression
+gzip compressed data, was "PythonLogging-1.0.2.tar", last modified: Mon Jun  5 16:13:26 2023, max compression
```

## Comparing `PythonLogging-1.0.1.tar` & `PythonLogging-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:02:25.691034 PythonLogging-1.0.1/
--rw-rw-rw-   0        0        0     1956 2023-06-05 16:02:25.690028 PythonLogging-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 16:02:25.675096 PythonLogging-1.0.1/PythonLogging/
--rw-rw-rw-   0        0        0     1591 2023-06-05 16:00:50.000000 PythonLogging-1.0.1/PythonLogging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:02:25.688069 PythonLogging-1.0.1/PythonLogging.egg-info/
--rw-rw-rw-   0        0        0     1956 2023-06-05 16:02:25.000000 PythonLogging-1.0.1/PythonLogging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-05 16:02:25.000000 PythonLogging-1.0.1/PythonLogging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:02:25.000000 PythonLogging-1.0.1/PythonLogging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-05 16:02:25.000000 PythonLogging-1.0.1/PythonLogging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1541 2023-06-05 16:02:04.000000 PythonLogging-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 16:02:25.691034 PythonLogging-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-06-05 16:02:21.000000 PythonLogging-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:13:26.025016 PythonLogging-1.0.2/
+-rw-rw-rw-   0        0        0     1956 2023-06-05 16:13:26.024012 PythonLogging-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 16:13:26.000558 PythonLogging-1.0.2/PythonLogging/
+-rw-rw-rw-   0        0        0     1643 2023-06-05 16:13:05.000000 PythonLogging-1.0.2/PythonLogging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:13:26.022013 PythonLogging-1.0.2/PythonLogging.egg-info/
+-rw-rw-rw-   0        0        0     1956 2023-06-05 16:13:25.000000 PythonLogging-1.0.2/PythonLogging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-06-05 16:13:25.000000 PythonLogging-1.0.2/PythonLogging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:13:25.000000 PythonLogging-1.0.2/PythonLogging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-05 16:13:25.000000 PythonLogging-1.0.2/PythonLogging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1541 2023-06-05 16:02:04.000000 PythonLogging-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:13:26.026015 PythonLogging-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-06-05 16:12:40.000000 PythonLogging-1.0.2/setup.py
```

### Comparing `PythonLogging-1.0.1/PKG-INFO` & `PythonLogging-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonLogging
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple logging library for easy log file management
 Home-page: https://github.com/SForces/PythonLogging
 Author: Osman TUNA
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `PythonLogging-1.0.1/PythonLogging/__init__.py` & `PythonLogging-1.0.2/PythonLogging/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         return "File type must be '.txt', not anything else!"
     if os.path.exists(formatted_path):
         return f"Path '{formatted_path}' already exists!"
     else:
         os.makedirs(os.path.dirname(formatted_path), exist_ok=True)  # Yeni dizini oluştur
         with open(formatted_path, "w") as f:
             pass
+        os.makedirs("PythonLogging",exist_ok=True)
         with open("PythonLogging/path.ini", "w") as f:
             f.write(formatted_path)
 def log(logmsg: str):
     """
     Writes a log message to the specified log file.
     if log file unspecified, you have to use 'PythonLogging.logfile_path('yourpath')'
```

### Comparing `PythonLogging-1.0.1/PythonLogging.egg-info/PKG-INFO` & `PythonLogging-1.0.2/PythonLogging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonLogging
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple logging library for easy log file management
 Home-page: https://github.com/SForces/PythonLogging
 Author: Osman TUNA
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `PythonLogging-1.0.1/README.md` & `PythonLogging-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PythonLogging-1.0.1/setup.py` & `PythonLogging-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PythonLogging",
-    version="1.0.1",
+    version="1.0.2",
     author="Osman TUNA",
     description="A simple logging library for easy log file management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SForces/PythonLogging",
     packages=["PythonLogging"],
     classifiers=[
```

