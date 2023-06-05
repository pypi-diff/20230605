# Comparing `tmp/cloudAgnosticPySqsListener-0.9.1.tar.gz` & `tmp/cloudAgnosticPySqsListener-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudAgnosticPySqsListener-0.9.1.tar", last modified: Mon Jun  5 13:00:17 2023, max compression
+gzip compressed data, was "cloudAgnosticPySqsListener-0.9.2.tar", last modified: Mon Jun  5 13:04:15 2023, max compression
```

## Comparing `cloudAgnosticPySqsListener-0.9.1.tar` & `cloudAgnosticPySqsListener-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:00:17.156055 cloudAgnosticPySqsListener-0.9.1/
--rw-r--r--   0 tom        (501) staff       (20)      643 2023-06-05 12:56:47.000000 cloudAgnosticPySqsListener-0.9.1/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     8039 2023-06-05 13:00:17.155863 cloudAgnosticPySqsListener-0.9.1/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     7407 2023-06-05 12:51:08.000000 cloudAgnosticPySqsListener-0.9.1/README.rst
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:00:17.154358 cloudAgnosticPySqsListener-0.9.1/cloudAgnosticPySqsListener.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     8039 2023-06-05 13:00:17.000000 cloudAgnosticPySqsListener-0.9.1/cloudAgnosticPySqsListener.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      349 2023-06-05 13:00:17.000000 cloudAgnosticPySqsListener-0.9.1/cloudAgnosticPySqsListener.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-05 13:00:17.000000 cloudAgnosticPySqsListener-0.9.1/cloudAgnosticPySqsListener.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-06-05 13:00:17.000000 cloudAgnosticPySqsListener-0.9.1/cloudAgnosticPySqsListener.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       26 2023-06-05 13:00:17.000000 cloudAgnosticPySqsListener-0.9.1/cloudAgnosticPySqsListener.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-05 13:00:17.156105 cloudAgnosticPySqsListener-0.9.1/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     2387 2023-06-05 12:57:19.000000 cloudAgnosticPySqsListener-0.9.1/setup.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:00:17.154516 cloudAgnosticPySqsListener-0.9.1/sqs_launcher/
--rw-r--r--   0 tom        (501) staff       (20)     4200 2023-06-05 12:23:15.000000 cloudAgnosticPySqsListener-0.9.1/sqs_launcher/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:00:17.155376 cloudAgnosticPySqsListener-0.9.1/sqs_listener/
--rw-r--r--   0 tom        (501) staff       (20)     9356 2023-06-05 12:24:49.000000 cloudAgnosticPySqsListener-0.9.1/sqs_listener/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4286 2023-06-05 12:21:12.000000 cloudAgnosticPySqsListener-0.9.1/sqs_listener/daemon.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:04:15.412770 cloudAgnosticPySqsListener-0.9.2/
+-rw-r--r--   0 tom        (501) staff       (20)      643 2023-06-05 12:56:47.000000 cloudAgnosticPySqsListener-0.9.2/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     8068 2023-06-05 13:04:15.412603 cloudAgnosticPySqsListener-0.9.2/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     7420 2023-06-05 13:03:42.000000 cloudAgnosticPySqsListener-0.9.2/README.rst
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:04:15.411430 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     8068 2023-06-05 13:04:15.000000 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      349 2023-06-05 13:04:15.000000 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-05 13:04:15.000000 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-06-05 13:04:15.000000 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       26 2023-06-05 13:04:15.000000 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-05 13:04:15.412815 cloudAgnosticPySqsListener-0.9.2/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     2403 2023-06-05 13:04:13.000000 cloudAgnosticPySqsListener-0.9.2/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:04:15.411581 cloudAgnosticPySqsListener-0.9.2/sqs_launcher/
+-rw-r--r--   0 tom        (501) staff       (20)     4200 2023-06-05 12:23:15.000000 cloudAgnosticPySqsListener-0.9.2/sqs_launcher/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:04:15.412184 cloudAgnosticPySqsListener-0.9.2/sqs_listener/
+-rw-r--r--   0 tom        (501) staff       (20)     9356 2023-06-05 12:24:49.000000 cloudAgnosticPySqsListener-0.9.2/sqs_listener/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4286 2023-06-05 12:21:12.000000 cloudAgnosticPySqsListener-0.9.2/sqs_listener/daemon.py
```

### Comparing `cloudAgnosticPySqsListener-0.9.1/LICENSE` & `cloudAgnosticPySqsListener-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudAgnosticPySqsListener-0.9.1/PKG-INFO` & `cloudAgnosticPySqsListener-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cloudAgnosticPySqsListener
-Version: 0.9.1
-Summary: A simple Python SQS utility package
-Home-page: https://github.com/jegesh/python-sqs-listener
+Version: 0.9.2
+Summary: A simple cloud agnostic Python SQS utility package
+Home-page: https://github.com/phedone/python-sqs-listener
 Author: Tom HENEAULT
 Author-email: tom@phedone.com
 License: Apache Software License
 Keywords: aws sqs listener and message launcher
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -27,15 +27,15 @@
 
 This package takes care of the boilerplate involved in listening to an SQS
 queue, as well as sending messages to a queue.  Works with python 2.7 & 3.6+.
 
 Installation
 ~~~~~~~~~~~~
 
-``pip install pySqsListener``
+``pip install cloudAgnosticPySqsListener``
 
 Listening to a queue
 ~~~~~~~~~~~~~~~~~~~~
 
 | Using the listener is very straightforward - just inherit from the
   ``SqsListener`` class and implement the ``handle_message()`` method.
   The queue will be created at runtime if it doesn't already exist.
```

### Comparing `cloudAgnosticPySqsListener-0.9.1/README.rst` & `cloudAgnosticPySqsListener-0.9.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 This package takes care of the boilerplate involved in listening to an SQS
 queue, as well as sending messages to a queue.  Works with python 2.7 & 3.6+.
 
 Installation
 ~~~~~~~~~~~~
 
-``pip install pySqsListener``
+``pip install cloudAgnosticPySqsListener``
 
 Listening to a queue
 ~~~~~~~~~~~~~~~~~~~~
 
 | Using the listener is very straightforward - just inherit from the
   ``SqsListener`` class and implement the ``handle_message()`` method.
   The queue will be created at runtime if it doesn't already exist.
```

### Comparing `cloudAgnosticPySqsListener-0.9.1/cloudAgnosticPySqsListener.egg-info/PKG-INFO` & `cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cloudAgnosticPySqsListener
-Version: 0.9.1
-Summary: A simple Python SQS utility package
-Home-page: https://github.com/jegesh/python-sqs-listener
+Version: 0.9.2
+Summary: A simple cloud agnostic Python SQS utility package
+Home-page: https://github.com/phedone/python-sqs-listener
 Author: Tom HENEAULT
 Author-email: tom@phedone.com
 License: Apache Software License
 Keywords: aws sqs listener and message launcher
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -27,15 +27,15 @@
 
 This package takes care of the boilerplate involved in listening to an SQS
 queue, as well as sending messages to a queue.  Works with python 2.7 & 3.6+.
 
 Installation
 ~~~~~~~~~~~~
 
-``pip install pySqsListener``
+``pip install cloudAgnosticPySqsListener``
 
 Listening to a queue
 ~~~~~~~~~~~~~~~~~~~~
 
 | Using the listener is very straightforward - just inherit from the
   ``SqsListener`` class and implement the ``handle_message()`` method.
   The queue will be created at runtime if it doesn't already exist.
```

### Comparing `cloudAgnosticPySqsListener-0.9.1/setup.py` & `cloudAgnosticPySqsListener-0.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 setup(
     name='cloudAgnosticPySqsListener',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.9.1',
+    version='0.9.2',
 
-    description='A simple Python SQS utility package',
+    description='A simple cloud agnostic Python SQS utility package',
     long_description=long_description,
 
     # The project's main homepage.
-    url='https://github.com/jegesh/python-sqs-listener',
+    url='https://github.com/phedone/python-sqs-listener',
 
     # Author details
     author='Tom HENEAULT',
     author_email='tom@phedone.com',
 
     # Choose your license
     license='Apache Software License',
```

### Comparing `cloudAgnosticPySqsListener-0.9.1/sqs_launcher/__init__.py` & `cloudAgnosticPySqsListener-0.9.2/sqs_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudAgnosticPySqsListener-0.9.1/sqs_listener/__init__.py` & `cloudAgnosticPySqsListener-0.9.2/sqs_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudAgnosticPySqsListener-0.9.1/sqs_listener/daemon.py` & `cloudAgnosticPySqsListener-0.9.2/sqs_listener/daemon.py`

 * *Files identical despite different names*

