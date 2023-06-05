# Comparing `tmp/erdgen-0.0.1rc3.tar.gz` & `tmp/erdgen-0.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdgen-0.0.1rc3.tar", last modified: Sun Jun  4 00:50:21 2023, max compression
+gzip compressed data, was "erdgen-0.0.1rc4.tar", last modified: Mon Jun  5 16:13:15 2023, max compression
```

## Comparing `erdgen-0.0.1rc3.tar` & `erdgen-0.0.1rc4.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-04 00:50:21.336350 erdgen-0.0.1rc3/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1068 2023-06-02 00:24:03.000000 erdgen-0.0.1rc3/LICENSE
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      169 2023-06-02 18:44:51.000000 erdgen-0.0.1rc3/MANIFEST.in
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4546 2023-06-04 00:50:21.336350 erdgen-0.0.1rc3/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3963 2023-06-04 00:49:31.000000 erdgen-0.0.1rc3/README.md
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-04 00:50:21.332350 erdgen-0.0.1rc3/erdgen/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc3/erdgen/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       87 2023-06-02 00:24:03.000000 erdgen-0.0.1rc3/erdgen/__main__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      419 2023-06-02 00:24:03.000000 erdgen-0.0.1rc3/erdgen/erdgen.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-04 00:50:21.336350 erdgen-0.0.1rc3/erdgen/src/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3004 2023-06-02 18:44:51.000000 erdgen-0.0.1rc3/erdgen/src/_.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc3/erdgen/src/__init__.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-04 00:50:21.336350 erdgen-0.0.1rc3/erdgen.egg-info/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4546 2023-06-04 00:50:21.000000 erdgen-0.0.1rc3/erdgen.egg-info/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      281 2023-06-04 00:50:21.000000 erdgen-0.0.1rc3/erdgen.egg-info/SOURCES.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-04 00:50:21.000000 erdgen-0.0.1rc3/erdgen.egg-info/dependency_links.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-04 00:50:21.000000 erdgen-0.0.1rc3/erdgen.egg-info/requires.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        7 2023-06-04 00:50:21.000000 erdgen-0.0.1rc3/erdgen.egg-info/top_level.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-04 00:50:21.336350 erdgen-0.0.1rc3/setup.cfg
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      962 2023-06-04 00:48:14.000000 erdgen-0.0.1rc3/setup.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1068 2023-06-02 00:24:03.000000 erdgen-0.0.1rc4/LICENSE
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      197 2023-06-05 16:12:49.000000 erdgen-0.0.1rc4/MANIFEST.in
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4578 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3995 2023-06-05 16:12:49.000000 erdgen-0.0.1rc4/README.md
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/erdgen/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc4/erdgen/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       87 2023-06-02 00:24:03.000000 erdgen-0.0.1rc4/erdgen/__main__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      419 2023-06-02 00:24:03.000000 erdgen-0.0.1rc4/erdgen/erdgen.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/erdgen/src/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3004 2023-06-02 18:44:51.000000 erdgen-0.0.1rc4/erdgen/src/_.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc4/erdgen/src/__init__.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/erdgen.egg-info/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4578 2023-06-05 16:13:15.000000 erdgen-0.0.1rc4/erdgen.egg-info/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      320 2023-06-05 16:13:15.000000 erdgen-0.0.1rc4/erdgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-05 16:13:15.000000 erdgen-0.0.1rc4/erdgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-05 16:13:15.000000 erdgen-0.0.1rc4/erdgen.egg-info/requires.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        7 2023-06-05 16:13:15.000000 erdgen-0.0.1rc4/erdgen.egg-info/top_level.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/setup.cfg
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      992 2023-06-05 16:12:49.000000 erdgen-0.0.1rc4/setup.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-05 16:13:15.302172 erdgen-0.0.1rc4/tests/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-04 00:27:25.000000 erdgen-0.0.1rc4/tests/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2315 2023-06-05 16:12:49.000000 erdgen-0.0.1rc4/tests/test_erdgen.py
```

### Comparing `erdgen-0.0.1rc3/LICENSE` & `erdgen-0.0.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `erdgen-0.0.1rc3/PKG-INFO` & `erdgen-0.0.1rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -118,14 +118,20 @@
 
 ### Install Packages
 
 ```bash
 pip install -r requirements.txt
 ```
 
+## Test
+
+```bash
+make test
+```
+
 ## Format
 
 ```bash
 make format
 ```
 
 ```bash
```

### Comparing `erdgen-0.0.1rc3/README.md` & `erdgen-0.0.1rc4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,20 @@
 
 ### Install Packages
 
 ```bash
 pip install -r requirements.txt
 ```
 
+## Test
+
+```bash
+make test
+```
+
 ## Format
 
 ```bash
 make format
 ```
 
 ```bash
```

### Comparing `erdgen-0.0.1rc3/erdgen/src/_.py` & `erdgen-0.0.1rc4/erdgen/src/_.py`

 * *Files identical despite different names*

### Comparing `erdgen-0.0.1rc3/erdgen.egg-info/PKG-INFO` & `erdgen-0.0.1rc4/erdgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -118,14 +118,20 @@
 
 ### Install Packages
 
 ```bash
 pip install -r requirements.txt
 ```
 
+## Test
+
+```bash
+make test
+```
+
 ## Format
 
 ```bash
 make format
 ```
 
 ```bash
```

### Comparing `erdgen-0.0.1rc3/setup.py` & `erdgen-0.0.1rc4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Andrew Moss",
     author_email="andrew.moss@neofinancial.com",
     python_requires=">=3.6",
     name="erdgen",
-    version="0.0.1rc3",
+    version="0.0.1rc4",
     description="Generate a DBML ERD from DBT YML relationships",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
@@ -22,8 +22,9 @@
     license="MIT license",
     packages=find_packages(include=["erdgen", "erdgen.*"]),
     url="https://github.com/neo-andrew-moss/erdgen",
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["click", "PyYAML", "Jinja2", "typing_extensions"],
+    tests_require=["pytest"],
 )
```

