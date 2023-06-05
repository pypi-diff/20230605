# Comparing `tmp/tapioca-wrapper-2.1.0.tar.gz` & `tmp/tapioca-wrapper-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapioca-wrapper-2.1.0.tar", last modified: Fri Mar 18 19:09:27 2022, max compression
+gzip compressed data, was "tapioca-wrapper-2.2.0.tar", last modified: Mon Jun  5 14:39:29 2023, max compression
```

## Comparing `tapioca-wrapper-2.1.0.tar` & `tapioca-wrapper-2.2.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxr-x   0 fjsj      (1000) fjsj      (1000)        0 2022-03-18 19:09:27.092841 tapioca-wrapper-2.1.0/
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     1086 2021-06-17 18:23:39.000000 tapioca-wrapper-2.1.0/LICENSE
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     1001 2022-03-18 19:09:27.092841 tapioca-wrapper-2.1.0/PKG-INFO
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     2403 2021-06-17 18:23:39.000000 tapioca-wrapper-2.1.0/README.md
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)       38 2022-03-18 19:09:27.092841 tapioca-wrapper-2.1.0/setup.cfg
--rwxrwxr-x   0 fjsj      (1000) fjsj      (1000)     2230 2021-06-17 18:23:39.000000 tapioca-wrapper-2.1.0/setup.py
-drwxrwxr-x   0 fjsj      (1000) fjsj      (1000)        0 2022-03-18 19:09:27.092841 tapioca-wrapper-2.1.0/tapioca/
--rwxrwxr-x   0 fjsj      (1000) fjsj      (1000)      269 2022-03-18 19:07:41.000000 tapioca-wrapper-2.1.0/tapioca/__init__.py
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     5659 2022-03-17 20:52:09.000000 tapioca-wrapper-2.1.0/tapioca/adapters.py
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)      947 2021-06-17 18:23:39.000000 tapioca-wrapper-2.1.0/tapioca/exceptions.py
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     1240 2021-06-17 18:23:39.000000 tapioca-wrapper-2.1.0/tapioca/serializers.py
--rwxrwxr-x   0 fjsj      (1000) fjsj      (1000)    12525 2022-03-18 19:07:41.000000 tapioca-wrapper-2.1.0/tapioca/tapioca.py
-drwxrwxr-x   0 fjsj      (1000) fjsj      (1000)        0 2022-03-18 19:09:27.092841 tapioca-wrapper-2.1.0/tapioca_wrapper.egg-info/
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)     1001 2022-03-18 19:09:26.000000 tapioca-wrapper-2.1.0/tapioca_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)      362 2022-03-18 19:09:26.000000 tapioca-wrapper-2.1.0/tapioca_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)        1 2022-03-18 19:09:26.000000 tapioca-wrapper-2.1.0/tapioca_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)        1 2022-03-18 19:09:26.000000 tapioca-wrapper-2.1.0/tapioca_wrapper.egg-info/not-zip-safe
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)       64 2022-03-18 19:09:26.000000 tapioca-wrapper-2.1.0/tapioca_wrapper.egg-info/requires.txt
--rw-rw-r--   0 fjsj      (1000) fjsj      (1000)        8 2022-03-18 19:09:26.000000 tapioca-wrapper-2.1.0/tapioca_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:39:29.341877 tapioca-wrapper-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-05 14:39:29.341877 tapioca-wrapper-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:39:29.341877 tapioca-wrapper-2.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2227 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:39:29.337877 tapioca-wrapper-2.2.0/tapioca/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      269 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tapioca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tapioca/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tapioca/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tapioca/serializers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12525 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tapioca/tapioca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:39:29.337877 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:39:29.000000 tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:39:29.341877 tapioca-wrapper-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tests/test_serializers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23822 2023-06-05 14:39:13.000000 tapioca-wrapper-2.2.0/tests/test_tapioca.py
```

### Comparing `tapioca-wrapper-2.1.0/LICENSE` & `tapioca-wrapper-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tapioca-wrapper-2.1.0/PKG-INFO` & `tapioca-wrapper-2.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: tapioca-wrapper
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python API client generator
 Home-page: https://github.com/vintasoftware/tapioca-wrapper
 Author: Filipe Ximenes
 Author-email: filipeximenes@gmail.com
 License: MIT
-Description: 
-        Tapioca provides an easy way to make explorable Python API wrappers.
-        APIs wrapped by Tapioca follow a simple interaction pattern that works uniformly so developers don't need to learn how to use a new coding interface/style for each service API.
-        
-        Source code hosted on Github: https://github.com/vintasoftware/tapioca-wrapper
-        
-        Documentation hosted by Readthedocs: http://tapioca-wrapper.readthedocs.io/en/stable/
-        
 Keywords: tapioca,wrapper,api
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+
+Tapioca provides an easy way to make explorable Python API wrappers.
+APIs wrapped by Tapioca follow a simple interaction pattern that works uniformly so
+developers don't need to learn how to use a new coding interface/style for each service API.
+
+Source code hosted on Github: https://github.com/vintasoftware/tapioca-wrapper
+
+Documentation hosted by Readthedocs: http://tapioca-wrapper.readthedocs.io/en/stable/
```

### Comparing `tapioca-wrapper-2.1.0/README.md` & `tapioca-wrapper-2.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Tapioca-Wrapper
 
 [![Join the chat at https://gitter.im/vintasoftware/tapioca-wrapper](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/vintasoftware/tapioca-wrapper?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
-[![Build Status](https://travis-ci.org/vintasoftware/tapioca-wrapper.svg?branch=master)](https://travis-ci.org/vintasoftware/tapioca-wrapper)
+[![Build Status](https://github.com/vintasoftware/tapioca-wrapper/actions/workflows/build.yml/badge.svg)](https://github.com/vintasoftware/tapioca-wrapper/actions/workflows/build.yml)
 [![Coverage Status](https://coveralls.io/repos/vintasoftware/tapioca-wrapper/badge.svg?branch=master&service=github)](https://coveralls.io/github/vintasoftware/tapioca-wrapper?branch=master)
 [![Current version at PyPI](https://img.shields.io/pypi/v/tapioca-wrapper.svg)](https://pypi.python.org/pypi/tapioca-wrapper)
 ![Supported Python Versions](https://img.shields.io/pypi/pyversions/tapioca-wrapper.svg)
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/vintasoftware/tapioca-wrapper/master/LICENSE)
 
 ![](docs/static/logo.png)
 
@@ -19,14 +19,31 @@
 
 ## Flavours
 
 You can find the full list of available tapioca clients [here](http://tapioca-wrapper.readthedocs.org/en/stable/flavours.html).
 
 To create new flavours, refer to [Building a wrapper](http://tapioca-wrapper.readthedocs.org/en/stable/buildingawrapper.html) in the documentation. There is also a [cookiecutter template](https://github.com/vintasoftware/cookiecutter-tapioca) to help bootstraping new API clients.
 
+## Contributing
+
+### Setup dev environment
+
+Tapioca-Wrapper is ready for development with [Dev Container](https://code.visualstudio.com/docs/devcontainers/tutorial). After downloading the code you just need to use "Reopen in Container option and after building run `make setup-devcontainer` just once.
+
+### How to Release:
+
+#### Pre release:
+- Include the changes in `docs/source/changelog.rst`
+- Update the version in `tapioca/__init__.py`
+
+#### Release:
+- Run the github action [build](https://github.com/vintasoftware/tapioca-wrapper/actions/workflows/build-release.yml)
+
+#### Post release:
+- Create tag with the version number to deploy the docs
 
 ## Other resources
 
 - [Contributors](https://github.com/vintasoftware/tapioca-wrapper/graphs/contributors)
 - [Changelog](http://tapioca-wrapper.readthedocs.org/en/stable/changelog.html)
 - [Blog post explaining the basics about Tapioca](http://www.vinta.com.br/blog/2016/python-api-clients-with-tapioca/)
```

### Comparing `tapioca-wrapper-2.1.0/setup.py` & `tapioca-wrapper-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 
 import re
 import os
 import sys
 
 description = """
 Tapioca provides an easy way to make explorable Python API wrappers.
-APIs wrapped by Tapioca follow a simple interaction pattern that works uniformly so developers don't need to learn how to use a new coding interface/style for each service API.
+APIs wrapped by Tapioca follow a simple interaction pattern that works uniformly so
+developers don't need to learn how to use a new coding interface/style for each service API.
 
 Source code hosted on Github: https://github.com/vintasoftware/tapioca-wrapper
 
 Documentation hosted by Readthedocs: http://tapioca-wrapper.readthedocs.io/en/stable/
 """
 
 package = 'tapioca'
 requirements = [
     'requests[security]>=2.6',
-    'arrow>=0.6.0,<1',
+    'arrow>=0.6.0',
     'six>=1',
     'xmltodict>=0.9.2'
 ]
 test_requirements = [
     'responses>=0.5',
     'mock>=1.3,<1.4'
 ]
```

### Comparing `tapioca-wrapper-2.1.0/tapioca/adapters.py` & `tapioca-wrapper-2.2.0/tapioca/adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,14 @@
         if not data and response.content.strip():
             data = json.loads(response.content.decode('utf-8'))
 
         if data:
             return data.get('error', None)
 
 
-
 class XMLAdapterMixin(object):
 
     def _input_branches_to_xml_bytestring(self, data):
         if isinstance(data, Mapping):
             return xmltodict.unparse(
                 data, **self._xmltodict_unparse_kwargs).encode('utf-8')
         try:
```

### Comparing `tapioca-wrapper-2.1.0/tapioca/exceptions.py` & `tapioca-wrapper-2.2.0/tapioca/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapioca-wrapper-2.1.0/tapioca/serializers.py` & `tapioca-wrapper-2.2.0/tapioca/serializers.py`

 * *Files identical despite different names*

### Comparing `tapioca-wrapper-2.1.0/tapioca/tapioca.py` & `tapioca-wrapper-2.2.0/tapioca/tapioca.py`

 * *Files identical despite different names*

### Comparing `tapioca-wrapper-2.1.0/tapioca_wrapper.egg-info/PKG-INFO` & `tapioca-wrapper-2.2.0/tapioca_wrapper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: tapioca-wrapper
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python API client generator
 Home-page: https://github.com/vintasoftware/tapioca-wrapper
 Author: Filipe Ximenes
 Author-email: filipeximenes@gmail.com
 License: MIT
-Description: 
-        Tapioca provides an easy way to make explorable Python API wrappers.
-        APIs wrapped by Tapioca follow a simple interaction pattern that works uniformly so developers don't need to learn how to use a new coding interface/style for each service API.
-        
-        Source code hosted on Github: https://github.com/vintasoftware/tapioca-wrapper
-        
-        Documentation hosted by Readthedocs: http://tapioca-wrapper.readthedocs.io/en/stable/
-        
 Keywords: tapioca,wrapper,api
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+
+Tapioca provides an easy way to make explorable Python API wrappers.
+APIs wrapped by Tapioca follow a simple interaction pattern that works uniformly so
+developers don't need to learn how to use a new coding interface/style for each service API.
+
+Source code hosted on Github: https://github.com/vintasoftware/tapioca-wrapper
+
+Documentation hosted by Readthedocs: http://tapioca-wrapper.readthedocs.io/en/stable/
```

