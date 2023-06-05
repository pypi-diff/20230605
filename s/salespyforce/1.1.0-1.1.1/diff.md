# Comparing `tmp/salespyforce-1.1.0.tar.gz` & `tmp/salespyforce-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salespyforce-1.1.0.tar", last modified: Mon May 29 19:57:38 2023, max compression
+gzip compressed data, was "salespyforce-1.1.1.tar", last modified: Mon Jun  5 18:12:07 2023, max compression
```

## Comparing `salespyforce-1.1.0.tar` & `salespyforce-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.447479 salespyforce-1.1.0/
--rw-r--r--   0 shurtj     (501) staff       (20)     1071 2023-01-22 19:54:55.000000 salespyforce-1.1.0/LICENSE
--rw-r--r--   0 shurtj     (501) staff       (20)     9175 2023-05-29 19:57:38.446785 salespyforce-1.1.0/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)     7818 2023-05-24 20:39:33.000000 salespyforce-1.1.0/README.md
--rw-r--r--   0 shurtj     (501) staff       (20)      569 2023-05-23 21:22:33.000000 salespyforce-1.1.0/pyproject.toml
--rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-05-29 19:57:38.447782 salespyforce-1.1.0/setup.cfg
--rw-r--r--   0 shurtj     (501) staff       (20)     3153 2023-05-08 21:41:53.000000 salespyforce-1.1.0/setup.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.415876 salespyforce-1.1.0/src/
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.423567 salespyforce-1.1.0/src/salespyforce/
--rw-r--r--   0 shurtj     (501) staff       (20)     2031 2023-05-08 21:19:50.000000 salespyforce-1.1.0/src/salespyforce/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5763 2023-02-17 19:12:52.000000 salespyforce-1.1.0/src/salespyforce/api.py
--rw-r--r--   0 shurtj     (501) staff       (20)     7494 2023-03-13 21:18:18.000000 salespyforce-1.1.0/src/salespyforce/chatter.py
--rw-r--r--   0 shurtj     (501) staff       (20)    45246 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/core.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.434429 salespyforce-1.1.0/src/salespyforce/errors/
--rw-r--r--   0 shurtj     (501) staff       (20)      320 2023-03-13 21:37:03.000000 salespyforce-1.1.0/src/salespyforce/errors/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    17057 2023-03-13 21:39:59.000000 salespyforce-1.1.0/src/salespyforce/errors/exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)      479 2023-02-22 22:06:11.000000 salespyforce-1.1.0/src/salespyforce/errors/handlers.py
--rw-r--r--   0 shurtj     (501) staff       (20)    21657 2023-02-22 22:09:03.000000 salespyforce-1.1.0/src/salespyforce/knowledge.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.441744 salespyforce-1.1.0/src/salespyforce/utils/
--rw-r--r--   0 shurtj     (501) staff       (20)      292 2023-03-13 21:51:57.000000 salespyforce-1.1.0/src/salespyforce/utils/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5697 2023-03-16 21:08:51.000000 salespyforce-1.1.0/src/salespyforce/utils/core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5661 2023-03-14 20:43:01.000000 salespyforce-1.1.0/src/salespyforce/utils/helper.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11799 2023-01-22 21:52:54.000000 salespyforce-1.1.0/src/salespyforce/utils/log_utils.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.445539 salespyforce-1.1.0/src/salespyforce/utils/tests/
--rw-r--r--   0 shurtj     (501) staff       (20)      242 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4772 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/resources.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1416 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/test_instantiate_object.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1840 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/test_sobjects.py
--rw-r--r--   0 shurtj     (501) staff       (20)      709 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/test_soql.py
--rw-r--r--   0 shurtj     (501) staff       (20)      809 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/test_sosl.py
--rw-r--r--   0 shurtj     (501) staff       (20)      733 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/version.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.429594 salespyforce-1.1.0/src/salespyforce.egg-info/
--rw-r--r--   0 shurtj     (501) staff       (20)     9175 2023-05-29 19:57:38.000000 salespyforce-1.1.0/src/salespyforce.egg-info/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)      930 2023-05-29 19:57:38.000000 salespyforce-1.1.0/src/salespyforce.egg-info/SOURCES.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-05-29 19:57:38.000000 salespyforce-1.1.0/src/salespyforce.egg-info/dependency_links.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      272 2023-05-29 19:57:38.000000 salespyforce-1.1.0/src/salespyforce.egg-info/requires.txt
--rw-r--r--   0 shurtj     (501) staff       (20)       13 2023-05-29 19:57:38.000000 salespyforce-1.1.0/src/salespyforce.egg-info/top_level.txt
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.241243 salespyforce-1.1.1/
+-rw-r--r--   0 shurtj     (501) staff       (20)     1071 2023-01-22 19:54:55.000000 salespyforce-1.1.1/LICENSE
+-rw-r--r--   0 shurtj     (501) staff       (20)     9175 2023-06-05 18:12:07.240569 salespyforce-1.1.1/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)     7818 2023-05-24 20:39:33.000000 salespyforce-1.1.1/README.md
+-rw-r--r--   0 shurtj     (501) staff       (20)      569 2023-05-23 21:22:33.000000 salespyforce-1.1.1/pyproject.toml
+-rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-06-05 18:12:07.241491 salespyforce-1.1.1/setup.cfg
+-rw-r--r--   0 shurtj     (501) staff       (20)     3153 2023-05-08 21:41:53.000000 salespyforce-1.1.1/setup.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.204679 salespyforce-1.1.1/src/
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.214633 salespyforce-1.1.1/src/salespyforce/
+-rw-r--r--   0 shurtj     (501) staff       (20)     2031 2023-05-08 21:19:50.000000 salespyforce-1.1.1/src/salespyforce/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5763 2023-02-17 19:12:52.000000 salespyforce-1.1.1/src/salespyforce/api.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     7494 2023-03-13 21:18:18.000000 salespyforce-1.1.1/src/salespyforce/chatter.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    45246 2023-05-29 19:55:32.000000 salespyforce-1.1.1/src/salespyforce/core.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.223830 salespyforce-1.1.1/src/salespyforce/errors/
+-rw-r--r--   0 shurtj     (501) staff       (20)      320 2023-03-13 21:37:03.000000 salespyforce-1.1.1/src/salespyforce/errors/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    17057 2023-03-13 21:39:59.000000 salespyforce-1.1.1/src/salespyforce/errors/exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      479 2023-02-22 22:06:11.000000 salespyforce-1.1.1/src/salespyforce/errors/handlers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    21657 2023-02-22 22:09:03.000000 salespyforce-1.1.1/src/salespyforce/knowledge.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.230941 salespyforce-1.1.1/src/salespyforce/utils/
+-rw-r--r--   0 shurtj     (501) staff       (20)      292 2023-03-13 21:51:57.000000 salespyforce-1.1.1/src/salespyforce/utils/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5674 2023-05-30 16:42:44.000000 salespyforce-1.1.1/src/salespyforce/utils/core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5661 2023-03-14 20:43:01.000000 salespyforce-1.1.1/src/salespyforce/utils/helper.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11799 2023-01-22 21:52:54.000000 salespyforce-1.1.1/src/salespyforce/utils/log_utils.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.238634 salespyforce-1.1.1/src/salespyforce/utils/tests/
+-rw-r--r--   0 shurtj     (501) staff       (20)      242 2023-05-29 19:55:32.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4772 2023-05-29 19:55:32.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/resources.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1422 2023-05-30 16:43:26.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/test_instantiate_object.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1846 2023-05-30 16:43:21.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/test_sobjects.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      715 2023-05-30 16:43:15.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/test_soql.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      815 2023-05-30 16:43:07.000000 salespyforce-1.1.1/src/salespyforce/utils/tests/test_sosl.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      733 2023-06-05 18:08:21.000000 salespyforce-1.1.1/src/salespyforce/utils/version.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-06-05 18:12:07.219722 salespyforce-1.1.1/src/salespyforce.egg-info/
+-rw-r--r--   0 shurtj     (501) staff       (20)     9175 2023-06-05 18:12:06.000000 salespyforce-1.1.1/src/salespyforce.egg-info/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)      930 2023-06-05 18:12:06.000000 salespyforce-1.1.1/src/salespyforce.egg-info/SOURCES.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-06-05 18:12:06.000000 salespyforce-1.1.1/src/salespyforce.egg-info/dependency_links.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      272 2023-06-05 18:12:06.000000 salespyforce-1.1.1/src/salespyforce.egg-info/requires.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)       13 2023-06-05 18:12:06.000000 salespyforce-1.1.1/src/salespyforce.egg-info/top_level.txt
```

### Comparing `salespyforce-1.1.0/LICENSE` & `salespyforce-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/PKG-INFO` & `salespyforce-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salespyforce
-Version: 1.1.0
+Version: 1.1.1
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
-Metadata-Version: 2.1 Name: salespyforce Version: 1.1.0 Summary: A Python
+Metadata-Version: 2.1 Name: salespyforce Version: 1.1.1 Summary: A Python
 toolset for performing Salesforce API calls Home-page: https://github.com/
 jeffshurtliff/salespyforce Author: Jeff Shurtliff Author-email:
 jeff.shurtliff@rsa.com Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/salespyforce/issues Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
```

### Comparing `salespyforce-1.1.0/README.md` & `salespyforce-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/pyproject.toml` & `salespyforce-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/setup.py` & `salespyforce-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/src/salespyforce/__init__.py` & `salespyforce-1.1.1/src/salespyforce/__init__.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/src/salespyforce/api.py` & `salespyforce-1.1.1/src/salespyforce/api.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/src/salespyforce/chatter.py` & `salespyforce-1.1.1/src/salespyforce/chatter.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/src/salespyforce/core.py` & `salespyforce-1.1.1/src/salespyforce/core.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/src/salespyforce/errors/exceptions.py` & `salespyforce-1.1.1/src/salespyforce/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/src/salespyforce/knowledge.py` & `salespyforce-1.1.1/src/salespyforce/knowledge.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/src/salespyforce/utils/core_utils.py` & `salespyforce-1.1.1/src/salespyforce/utils/core_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-:Module:            khoros.utils.core_utils
+:Module:            salespyforce.utils.core_utils
 :Synopsis:          Collection of supporting utilities and functions to complement the primary modules
 :Usage:             ``from salespyforce.utils import core_utils``
 :Example:           ``encoded_string = core_utils.encode_url(decoded_string)``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     16 Mar 2023
+:Modified Date:     29 May 2023
 """
 
 import random
 import string
 import os.path
 import warnings
 import urllib.parse
@@ -53,16 +53,14 @@
     """
     warnings.warn(warn_msg, UserWarning)
 
 
 def get_file_type(file_path):
     """This function attempts to identify if a given file path is for a YAML or JSON file.
 
-    .. versionadded:: 2.2.0
-
     :param file_path: The full path to the file
     :type file_path: str
     :returns: The file type in string format (e.g. ``yaml`` or ``json``)
     :raises: :py:exc:`FileNotFoundError`, :py:exc:`khoros.errors.exceptions.UnknownFileTypeError`
     """
     file_type = 'unknown'
     if os.path.isfile(file_path):
```

### Comparing `salespyforce-1.1.0/src/salespyforce/utils/helper.py` & `salespyforce-1.1.1/src/salespyforce/utils/helper.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/src/salespyforce/utils/log_utils.py` & `salespyforce-1.1.1/src/salespyforce/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/src/salespyforce/utils/tests/resources.py` & `salespyforce-1.1.1/src/salespyforce/utils/tests/resources.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.1.0/src/salespyforce/utils/tests/test_instantiate_object.py` & `salespyforce-1.1.1/src/salespyforce/utils/tests/test_instantiate_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-:Module:         khoros.utils.tests.test_instantiate_object
+:Module:         salespyforce.utils.tests.test_instantiate_object
 :Synopsis:       This module is used by pytest to test instantiating the core object
 :Created By:     Jeff Shurtliff
 :Last Modified:  Jeff Shurtliff
 :Modified Date:  29 May 2023
 """
 
 from . import resources
```

### Comparing `salespyforce-1.1.0/src/salespyforce/utils/tests/test_sobjects.py` & `salespyforce-1.1.1/src/salespyforce/utils/tests/test_sobjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-:Module:         khoros.utils.tests.test_sobjects
+:Module:         salespyforce.utils.tests.test_sobjects
 :Synopsis:       This module is used by pytest to test basic sObject-related methods
 :Created By:     Jeff Shurtliff
 :Last Modified:  Jeff Shurtliff
 :Modified Date:  29 May 2023
 """
 
 import requests
```

### Comparing `salespyforce-1.1.0/src/salespyforce/utils/tests/test_soql.py` & `salespyforce-1.1.1/src/salespyforce/utils/tests/test_soql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-:Module:         khoros.utils.tests.test_sobjects
+:Module:         salespyforce.utils.tests.test_sobjects
 :Synopsis:       This module is used by pytest to test performing SOQL queries
 :Created By:     Jeff Shurtliff
 :Last Modified:  Jeff Shurtliff
 :Modified Date:  29 May 2023
 """
 
 from . import resources
```

### Comparing `salespyforce-1.1.0/src/salespyforce/utils/tests/test_sosl.py` & `salespyforce-1.1.1/src/salespyforce/utils/tests/test_sosl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-:Module:         khoros.utils.tests.test_sobjects
+:Module:         salespyforce.utils.tests.test_sobjects
 :Synopsis:       This module is used by pytest to test performing SOQL queries
 :Created By:     Jeff Shurtliff
 :Last Modified:  Jeff Shurtliff
 :Modified Date:  29 May 2023
 """
 
 import requests
```

### Comparing `salespyforce-1.1.0/src/salespyforce/utils/version.py` & `salespyforce-1.1.1/src/salespyforce/utils/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 """
 :Module:            salespyforce.utils.version
 :Synopsis:          This simple script contains the package version
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     27 May 2023
+:Modified Date:     05 Jun 2023
 """
 
 from . import log_utils
 
 # Initialize logging
 logger = log_utils.initialize_logging(__name__)
 
 # Define special and global variables
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 
 def get_full_version():
     """This function returns the current full version of the ``salespyforce`` package."""
     return __version__
```

### Comparing `salespyforce-1.1.0/src/salespyforce.egg-info/PKG-INFO` & `salespyforce-1.1.1/src/salespyforce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salespyforce
-Version: 1.1.0
+Version: 1.1.1
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
-Metadata-Version: 2.1 Name: salespyforce Version: 1.1.0 Summary: A Python
+Metadata-Version: 2.1 Name: salespyforce Version: 1.1.1 Summary: A Python
 toolset for performing Salesforce API calls Home-page: https://github.com/
 jeffshurtliff/salespyforce Author: Jeff Shurtliff Author-email:
 jeff.shurtliff@rsa.com Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/salespyforce/issues Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
```

### Comparing `salespyforce-1.1.0/src/salespyforce.egg-info/SOURCES.txt` & `salespyforce-1.1.1/src/salespyforce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

