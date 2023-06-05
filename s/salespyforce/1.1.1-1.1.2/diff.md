# Comparing `tmp/salespyforce-1.1.1.tar.gz` & `tmp/salespyforce-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salespyforce-1.1.1.tar", last modified: Mon Jun  5 18:12:07 2023, max compression
+gzip compressed data, was "salespyforce-1.1.2.tar", last modified: Mon Jun  5 18:18:57 2023, max compression
```

## Comparing `salespyforce-1.1.1.tar` & `salespyforce-1.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.241243 salespyforce-1.1.1/
--rw-r--r--   0 shurtj     (501) staff       (20)     1071 2023-01-22 19:54:55.000000 salespyforce-1.1.1/LICENSE
--rw-r--r--   0 shurtj     (501) staff       (20)     9175 2023-06-05 18:12:07.240569 salespyforce-1.1.1/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)     7818 2023-05-24 20:39:33.000000 salespyforce-1.1.1/README.md
--rw-r--r--   0 shurtj     (501) staff       (20)      569 2023-05-23 21:22:33.000000 salespyforce-1.1.1/pyproject.toml
--rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-06-05 18:12:07.241491 salespyforce-1.1.1/setup.cfg
--rw-r--r--   0 shurtj     (501) staff       (20)     3153 2023-05-08 21:41:53.000000 salespyforce-1.1.1/setup.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.204679 salespyforce-1.1.1/src/
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.214633 salespyforce-1.1.1/src/salespyforce/
--rw-r--r--   0 shurtj     (501) staff       (20)     2031 2023-05-08 21:19:50.000000 salespyforce-1.1.1/src/salespyforce/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5763 2023-02-17 19:12:52.000000 salespyforce-1.1.1/src/salespyforce/api.py
--rw-r--r--   0 shurtj     (501) staff       (20)     7494 2023-03-13 21:18:18.000000 salespyforce-1.1.1/src/salespyforce/chatter.py
--rw-r--r--   0 shurtj     (501) staff       (20)    45246 2023-05-29 19:55:32.000000 salespyforce-1.1.1/src/salespyforce/core.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.223830 salespyforce-1.1.1/src/salespyforce/errors/
--rw-r--r--   0 shurtj     (501) staff       (20)      320 2023-03-13 21:37:03.000000 salespyforce-1.1.1/src/salespyforce/errors/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    17057 2023-03-13 21:39:59.000000 salespyforce-1.1.1/src/salespyforce/errors/exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)      479 2023-02-22 22:06:11.000000 salespyforce-1.1.1/src/salespyforce/errors/handlers.py
--rw-r--r--   0 shurtj     (501) staff       (20)    21657 2023-02-22 22:09:03.000000 salespyforce-1.1.1/src/salespyforce/knowledge.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.230941 salespyforce-1.1.1/src/salespyforce/utils/
--rw-r--r--   0 shurtj     (501) staff       (20)      292 2023-03-13 21:51:57.000000 salespyforce-1.1.1/src/salespyforce/utils/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5674 2023-05-30 16:42:44.000000 salespyforce-1.1.1/src/salespyforce/utils/core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5661 2023-03-14 20:43:01.000000 salespyforce-1.1.1/src/salespyforce/utils/helper.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11799 2023-01-22 21:52:54.000000 salespyforce-1.1.1/src/salespyforce/utils/log_utils.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.238634 salespyforce-1.1.1/src/salespyforce/utils/tests/
--rw-r--r--   0 shurtj     (501) staff       (20)      242 2023-05-29 19:55:32.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4772 2023-05-29 19:55:32.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/resources.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1422 2023-05-30 16:43:26.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/test_instantiate_object.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1846 2023-05-30 16:43:21.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/test_sobjects.py
--rw-r--r--   0 shurtj     (501) staff       (20)      715 2023-05-30 16:43:15.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/test_soql.py
--rw-r--r--   0 shurtj     (501) staff       (20)      815 2023-05-30 16:43:07.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/test_sosl.py
--rw-r--r--   0 shurtj     (501) staff       (20)      733 2023-06-05 18:08:21.000000 salespyforce-1.1.1/src/salespyforce/utils/version.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.219722 salespyforce-1.1.1/src/salespyforce.egg-info/
--rw-r--r--   0 shurtj     (501) staff       (20)     9175 2023-06-05 18:12:06.000000 salespyforce-1.1.1/src/salespyforce.egg-info/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)      930 2023-06-05 18:12:06.000000 salespyforce-1.1.1/src/salespyforce.egg-info/SOURCES.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-06-05 18:12:06.000000 salespyforce-1.1.1/src/salespyforce.egg-info/dependency_links.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      272 2023-06-05 18:12:06.000000 salespyforce-1.1.1/src/salespyforce.egg-info/requires.txt
--rw-r--r--   0 shurtj     (501) staff       (20)       13 2023-06-05 18:12:06.000000 salespyforce-1.1.1/src/salespyforce.egg-info/top_level.txt
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:18:57.135625 salespyforce-1.1.2/
+-rw-r--r--   0 shurtj     (501) staff       (20)     1071 2023-01-22 19:54:55.000000 salespyforce-1.1.2/LICENSE
+-rw-r--r--   0 shurtj     (501) staff       (20)     9175 2023-06-05 18:18:57.134584 salespyforce-1.1.2/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)     7818 2023-05-24 20:39:33.000000 salespyforce-1.1.2/README.md
+-rw-r--r--   0 shurtj     (501) staff       (20)      569 2023-06-05 18:15:28.000000 salespyforce-1.1.2/pyproject.toml
+-rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-06-05 18:18:57.135866 salespyforce-1.1.2/setup.cfg
+-rw-r--r--   0 shurtj     (501) staff       (20)     3153 2023-05-08 21:41:53.000000 salespyforce-1.1.2/setup.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:18:57.097536 salespyforce-1.1.2/src/
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:18:57.107647 salespyforce-1.1.2/src/salespyforce/
+-rw-r--r--   0 shurtj     (501) staff       (20)     2031 2023-05-08 21:19:50.000000 salespyforce-1.1.2/src/salespyforce/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5763 2023-02-17 19:12:52.000000 salespyforce-1.1.2/src/salespyforce/api.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     7494 2023-03-13 21:18:18.000000 salespyforce-1.1.2/src/salespyforce/chatter.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    45246 2023-05-29 19:55:32.000000 salespyforce-1.1.2/src/salespyforce/core.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:18:57.117694 salespyforce-1.1.2/src/salespyforce/errors/
+-rw-r--r--   0 shurtj     (501) staff       (20)      320 2023-03-13 21:37:03.000000 salespyforce-1.1.2/src/salespyforce/errors/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    17057 2023-03-13 21:39:59.000000 salespyforce-1.1.2/src/salespyforce/errors/exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      479 2023-02-22 22:06:11.000000 salespyforce-1.1.2/src/salespyforce/errors/handlers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    21657 2023-02-22 22:09:03.000000 salespyforce-1.1.2/src/salespyforce/knowledge.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:18:57.124355 salespyforce-1.1.2/src/salespyforce/utils/
+-rw-r--r--   0 shurtj     (501) staff       (20)      292 2023-03-13 21:51:57.000000 salespyforce-1.1.2/src/salespyforce/utils/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5674 2023-05-30 16:42:44.000000 salespyforce-1.1.2/src/salespyforce/utils/core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5661 2023-03-14 20:43:01.000000 salespyforce-1.1.2/src/salespyforce/utils/helper.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11799 2023-01-22 21:52:54.000000 salespyforce-1.1.2/src/salespyforce/utils/log_utils.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:18:57.132497 salespyforce-1.1.2/src/salespyforce/utils/tests/
+-rw-r--r--   0 shurtj     (501) staff       (20)      242 2023-05-29 19:55:32.000000 salespyforce-1.1.2/src/salespyforce/utils/tests/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4772 2023-05-29 19:55:32.000000 salespyforce-1.1.2/src/salespyforce/utils/tests/resources.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1422 2023-05-30 16:43:26.000000 salespyforce-1.1.2/src/salespyforce/utils/tests/test_instantiate_object.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1846 2023-05-30 16:43:21.000000 salespyforce-1.1.2/src/salespyforce/utils/tests/test_sobjects.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      715 2023-05-30 16:43:15.000000 salespyforce-1.1.2/src/salespyforce/utils/tests/test_soql.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      815 2023-05-30 16:43:07.000000 salespyforce-1.1.2/src/salespyforce/utils/tests/test_sosl.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      733 2023-06-05 18:17:02.000000 salespyforce-1.1.2/src/salespyforce/utils/version.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:18:57.113231 salespyforce-1.1.2/src/salespyforce.egg-info/
+-rw-r--r--   0 shurtj     (501) staff       (20)     9175 2023-06-05 18:18:56.000000 salespyforce-1.1.2/src/salespyforce.egg-info/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)      930 2023-06-05 18:18:56.000000 salespyforce-1.1.2/src/salespyforce.egg-info/SOURCES.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-06-05 18:18:56.000000 salespyforce-1.1.2/src/salespyforce.egg-info/dependency_links.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      272 2023-06-05 18:18:56.000000 salespyforce-1.1.2/src/salespyforce.egg-info/requires.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)       13 2023-06-05 18:18:56.000000 salespyforce-1.1.2/src/salespyforce.egg-info/top_level.txt
```

### Comparing `salespyforce-1.1.1/LICENSE` & `salespyforce-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/PKG-INFO` & `salespyforce-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salespyforce
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python toolset for performing Salesforce API calls
 Home-page: https://github.com/jeffshurtliff/salespyforce
 Author: Jeff Shurtliff
 Author-email: jeff.shurtliff@rsa.com
 Project-URL: Issue Tracker, https://github.com/jeffshurtliff/salespyforce/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salespyforce Version: 1.1.1 Summary: A Python
+Metadata-Version: 2.1 Name: salespyforce Version: 1.1.2 Summary: A Python
 toolset for performing Salesforce API calls Home-page: https://github.com/
 jeffshurtliff/salespyforce Author: Jeff Shurtliff Author-email:
 jeff.shurtliff@rsa.com Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/salespyforce/issues Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
```

### Comparing `salespyforce-1.1.1/README.md` & `salespyforce-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/pyproject.toml` & `salespyforce-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "salespyforce"
-version = "1.0.0"
+version = "1.1.2"
 description = "A Python toolset for performing Salesforce API calls"
 authors = ["Jeff Shurtliff <jeff.shurtliff@rsa.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `salespyforce-1.1.1/setup.py` & `salespyforce-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/__init__.py` & `salespyforce-1.1.2/src/salespyforce/__init__.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/api.py` & `salespyforce-1.1.2/src/salespyforce/api.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/chatter.py` & `salespyforce-1.1.2/src/salespyforce/chatter.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/core.py` & `salespyforce-1.1.2/src/salespyforce/core.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/errors/exceptions.py` & `salespyforce-1.1.2/src/salespyforce/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/knowledge.py` & `salespyforce-1.1.2/src/salespyforce/knowledge.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/utils/core_utils.py` & `salespyforce-1.1.2/src/salespyforce/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/utils/helper.py` & `salespyforce-1.1.2/src/salespyforce/utils/helper.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/utils/log_utils.py` & `salespyforce-1.1.2/src/salespyforce/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/utils/tests/resources.py` & `salespyforce-1.1.2/src/salespyforce/utils/tests/resources.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/utils/tests/test_instantiate_object.py` & `salespyforce-1.1.2/src/salespyforce/utils/tests/test_instantiate_object.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/utils/tests/test_sobjects.py` & `salespyforce-1.1.2/src/salespyforce/utils/tests/test_sobjects.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/utils/tests/test_soql.py` & `salespyforce-1.1.2/src/salespyforce/utils/tests/test_soql.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/utils/tests/test_sosl.py` & `salespyforce-1.1.2/src/salespyforce/utils/tests/test_sosl.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.1/src/salespyforce/utils/version.py` & `salespyforce-1.1.2/src/salespyforce/utils/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from . import log_utils
 
 # Initialize logging
 logger = log_utils.initialize_logging(__name__)
 
 # Define special and global variables
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 
 def get_full_version():
     """This function returns the current full version of the ``salespyforce`` package."""
     return __version__
```

### Comparing `salespyforce-1.1.1/src/salespyforce.egg-info/PKG-INFO` & `salespyforce-1.1.2/src/salespyforce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salespyforce
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python toolset for performing Salesforce API calls
 Home-page: https://github.com/jeffshurtliff/salespyforce
 Author: Jeff Shurtliff
 Author-email: jeff.shurtliff@rsa.com
 Project-URL: Issue Tracker, https://github.com/jeffshurtliff/salespyforce/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salespyforce Version: 1.1.1 Summary: A Python
+Metadata-Version: 2.1 Name: salespyforce Version: 1.1.2 Summary: A Python
 toolset for performing Salesforce API calls Home-page: https://github.com/
 jeffshurtliff/salespyforce Author: Jeff Shurtliff Author-email:
 jeff.shurtliff@rsa.com Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/salespyforce/issues Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
```

### Comparing `salespyforce-1.1.1/src/salespyforce.egg-info/SOURCES.txt` & `salespyforce-1.1.2/src/salespyforce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

