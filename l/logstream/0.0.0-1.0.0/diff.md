# Comparing `tmp/logstream-0.0.0.tar.gz` & `tmp/logstream-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/krink/logstream/dist/tmp5pzkqd7l/logstream-0.0.0.tar", last modified: Mon Dec 20 22:44:55 2021, max compression
+gzip compressed data, was "/Users/krink/git/logstream/dist/.tmp-hkg3cgwi/logstream-1.0.0.tar", last modified: Sun Jun  4 23:59:24 2023, max compression
```

## Comparing `logstream-0.0.0.tar` & `logstream-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 krink      (501) staff       (20)        0 2021-12-20 22:44:55.896900 logstream-0.0.0/
--rw-r--r--   0 krink      (501) staff       (20)      759 2021-12-20 22:44:55.897059 logstream-0.0.0/PKG-INFO
--rw-r--r--   0 krink      (501) staff       (20)      434 2021-12-20 22:43:09.000000 logstream-0.0.0/README.md
--rw-r--r--   0 krink      (501) staff       (20)      724 2021-12-20 22:44:55.897650 logstream-0.0.0/setup.cfg
--rw-r--r--   0 krink      (501) staff       (20)      595 2021-12-20 22:28:04.000000 logstream-0.0.0/setup.py
-drwxr-xr-x   0 krink      (501) staff       (20)        0 2021-12-20 22:44:55.893660 logstream-0.0.0/src/
-drwxr-xr-x   0 krink      (501) staff       (20)        0 2021-12-20 22:44:55.894998 logstream-0.0.0/src/logstream/
--rw-r--r--   0 krink      (501) staff       (20)      107 2021-12-20 22:18:17.000000 logstream-0.0.0/src/logstream/__init__.py
--rw-r--r--   0 krink      (501) staff       (20)      137 2021-12-20 22:18:39.000000 logstream-0.0.0/src/logstream/__main__.py
--rwxr-xr-x   0 krink      (501) staff       (20)     3020 2021-12-20 22:39:13.000000 logstream-0.0.0/src/logstream/logstream.py
-drwxr-xr-x   0 krink      (501) staff       (20)        0 2021-12-20 22:44:55.896695 logstream-0.0.0/src/logstream.egg-info/
--rw-r--r--   0 krink      (501) staff       (20)      759 2021-12-20 22:44:55.000000 logstream-0.0.0/src/logstream.egg-info/PKG-INFO
--rw-r--r--   0 krink      (501) staff       (20)      295 2021-12-20 22:44:55.000000 logstream-0.0.0/src/logstream.egg-info/SOURCES.txt
--rw-r--r--   0 krink      (501) staff       (20)        1 2021-12-20 22:44:55.000000 logstream-0.0.0/src/logstream.egg-info/dependency_links.txt
--rw-r--r--   0 krink      (501) staff       (20)       56 2021-12-20 22:44:55.000000 logstream-0.0.0/src/logstream.egg-info/entry_points.txt
--rw-r--r--   0 krink      (501) staff       (20)       10 2021-12-20 22:44:55.000000 logstream-0.0.0/src/logstream.egg-info/top_level.txt
+drwxr-xr-x   0 krink      (501) staff       (20)        0 2023-06-04 23:59:24.030995 logstream-1.0.0/
+-rw-r--r--   0 krink      (501) staff       (20)      723 2023-06-04 23:59:24.031158 logstream-1.0.0/PKG-INFO
+-rw-r--r--   0 krink      (501) staff       (20)     1243 2023-06-04 23:39:50.000000 logstream-1.0.0/README.md
+drwxr-xr-x   0 krink      (501) staff       (20)        0 2023-06-04 23:59:24.026709 logstream-1.0.0/python/
+drwxr-xr-x   0 krink      (501) staff       (20)        0 2023-06-04 23:59:24.028775 logstream-1.0.0/python/logstream/
+-rw-r--r--   0 krink      (501) staff       (20)      107 2021-12-20 22:18:17.000000 logstream-1.0.0/python/logstream/__init__.py
+-rw-r--r--   0 krink      (501) staff       (20)      127 2021-12-21 04:36:25.000000 logstream-1.0.0/python/logstream/__main__.py
+-rwxr-xr-x   0 krink      (501) staff       (20)     3046 2023-06-04 23:35:23.000000 logstream-1.0.0/python/logstream/logstream.py
+drwxr-xr-x   0 krink      (501) staff       (20)        0 2023-06-04 23:59:24.030690 logstream-1.0.0/python/logstream.egg-info/
+-rw-r--r--   0 krink      (501) staff       (20)      723 2023-06-04 23:59:24.000000 logstream-1.0.0/python/logstream.egg-info/PKG-INFO
+-rw-r--r--   0 krink      (501) staff       (20)      319 2023-06-04 23:59:24.000000 logstream-1.0.0/python/logstream.egg-info/SOURCES.txt
+-rw-r--r--   0 krink      (501) staff       (20)        1 2023-06-04 23:59:24.000000 logstream-1.0.0/python/logstream.egg-info/dependency_links.txt
+-rw-r--r--   0 krink      (501) staff       (20)       55 2023-06-04 23:59:24.000000 logstream-1.0.0/python/logstream.egg-info/entry_points.txt
+-rw-r--r--   0 krink      (501) staff       (20)       10 2023-06-04 23:59:24.000000 logstream-1.0.0/python/logstream.egg-info/top_level.txt
+-rw-r--r--   0 krink      (501) staff       (20)      730 2023-06-04 23:59:24.032283 logstream-1.0.0/setup.cfg
+-rw-r--r--   0 krink      (501) staff       (20)      595 2023-06-04 23:44:34.000000 logstream-1.0.0/setup.py
```

### Comparing `logstream-0.0.0/PKG-INFO` & `logstream-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: logstream
-Version: 0.0.0
+Version: 1.0.0
 Summary: operating system syslog data and/or tail log files.
 Home-page: https://gitlab.com/krink/logstream
 Author: Karl Rink
 Author-email: karl@rink.us
-License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/krink/logstream/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Python command line tool to logstream operating syslog data and/or log files.
-
```

### Comparing `logstream-0.0.0/setup.cfg` & `logstream-1.0.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = logstream-pkg-krink
-version = 0.0.0
+version = 1.0.0
 author = Karl Rink
 author_email = karl@rink.us
 description = logstream command
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/krink/logstream
 project_urls = 
@@ -16,18 +16,18 @@
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: System Administrators
 	Topic :: Utilities
 
 [options]
 package_dir = 
-	= src
+	= python
 packages = find:
 python_requires = >=3.6
 
 [options.packages.find]
-where = src
+where = python
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `logstream-0.0.0/setup.py` & `logstream-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     name = "logstream",
     packages = ["logstream"],
     entry_points = {
         "console_scripts": ['logstream = logstream.logstream:main']
         },
-    version = '0.0.0',
+    version = '1.0.0',
     description = "operating system syslog data and/or tail log files.",
     long_description = "Python command line tool to logstream operating syslog data and/or log files.",
     author = "Karl Rink",
     author_email = "karl@rink.us",
     url = "https://gitlab.com/krink/logstream",
     install_requires = []
     )
```

### Comparing `logstream-0.0.0/src/logstream/logstream.py` & `logstream-1.0.0/python/logstream/logstream.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """logstream: command."""
 
 from __future__ import absolute_import
 
-__version__ = '0.0.0'
+__version__ = '1.0.0'
 
 import sys
 from subprocess import Popen, PIPE, STDOUT
 import time
 
 if sys.version_info[0] < 3:
     raise Exception("Python 3 Please")
 
 usage = "Usage: " + sys.argv[0] + """
 
     --help
     --version
     --format [type]
 
-    type darwin:
+    os darwin:
         [default|compact|json|ndjson|syslog]
 
-    type linux:
+    os linux:
         [short|short-full|short-unix|verbose|export]
         [json|json-pretty|json-sse|json-seq]
 
+    os windows:
+        TODO
+
     --tail file
 
 """
 
 
 def stream(formatting=None):
     """stream: operating systems syslog data stream."""
```

### Comparing `logstream-0.0.0/src/logstream.egg-info/PKG-INFO` & `logstream-1.0.0/python/logstream.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: logstream
-Version: 0.0.0
+Version: 1.0.0
 Summary: operating system syslog data and/or tail log files.
 Home-page: https://gitlab.com/krink/logstream
 Author: Karl Rink
 Author-email: karl@rink.us
-License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/krink/logstream/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Python command line tool to logstream operating syslog data and/or log files.
-
```

