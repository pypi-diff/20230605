# Comparing `tmp/python-freckle-client-0.4.0.tar.gz` & `tmp/python-freckle-client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-freckle-client-0.4.0.tar", last modified: Sun Aug 25 12:07:27 2019, max compression
+gzip compressed data, was "python-freckle-client-0.5.0.tar", last modified: Mon Jun  5 06:54:51 2023, max compression
```

## Comparing `python-freckle-client-0.4.0.tar` & `python-freckle-client-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/
--rw-r--r--   0 martin     (501) staff       (20)     2663 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1083 2019-08-25 12:01:52.000000 python-freckle-client-0.4.0/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)      239 2019-08-25 12:03:07.000000 python-freckle-client-0.4.0/AUTHORS
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/freckle_client/
--rw-r--r--   0 martin     (501) staff       (20)     4177 2019-08-25 12:01:52.000000 python-freckle-client-0.4.0/freckle_client/client.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/freckle_client/tests/
--rw-r--r--   0 martin     (501) staff       (20)        0 2019-08-25 12:01:52.000000 python-freckle-client-0.4.0/freckle_client/tests/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)       66 2019-08-25 12:01:52.000000 python-freckle-client-0.4.0/freckle_client/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      410 2019-08-25 12:01:52.000000 python-freckle-client-0.4.0/freckle_client/exceptions.py
--rw-r--r--   0 martin     (501) staff       (20)      241 2019-08-25 12:01:52.000000 python-freckle-client-0.4.0/MANIFEST.in
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/python_freckle_client.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     2663 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/python_freckle_client.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)      409 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/python_freckle_client.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)       23 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/python_freckle_client.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)       15 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/python_freckle_client.egg-info/top_level.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/python_freckle_client.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)     1829 2019-08-25 12:06:56.000000 python-freckle-client-0.4.0/setup.py
--rw-r--r--   0 martin     (501) staff       (20)      980 2019-08-25 12:01:52.000000 python-freckle-client-0.4.0/CHANGELOG.txt
--rw-r--r--   0 martin     (501) staff       (20)      124 2019-08-25 12:07:27.000000 python-freckle-client-0.4.0/setup.cfg
--rw-r--r--   0 martin     (501) staff       (20)     1697 2019-08-25 12:01:52.000000 python-freckle-client-0.4.0/README.rst
+drwxr-xr-x   0 amandabizzinotto   (501) staff       (20)        0 2023-06-05 06:54:51.029675 python-freckle-client-0.5.0/
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)      239 2023-06-05 03:45:14.000000 python-freckle-client-0.5.0/AUTHORS
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)     1070 2023-06-05 06:21:46.000000 python-freckle-client-0.5.0/CHANGELOG.txt
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)     1083 2023-06-05 03:45:14.000000 python-freckle-client-0.5.0/LICENSE
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)      241 2023-06-05 03:45:14.000000 python-freckle-client-0.5.0/MANIFEST.in
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)     2056 2023-06-05 06:54:51.029550 python-freckle-client-0.5.0/PKG-INFO
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)     1667 2023-06-05 06:19:25.000000 python-freckle-client-0.5.0/README.rst
+drwxr-xr-x   0 amandabizzinotto   (501) staff       (20)        0 2023-06-05 06:54:51.028231 python-freckle-client-0.5.0/freckle_client/
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)       96 2023-06-05 06:49:27.000000 python-freckle-client-0.5.0/freckle_client/__init__.py
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)     5293 2023-06-05 06:34:38.000000 python-freckle-client-0.5.0/freckle_client/client.py
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)      393 2023-06-05 06:13:21.000000 python-freckle-client-0.5.0/freckle_client/exceptions.py
+drwxr-xr-x   0 amandabizzinotto   (501) staff       (20)        0 2023-06-05 06:54:51.028482 python-freckle-client-0.5.0/freckle_client/tests/
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)       32 2023-06-05 05:55:30.000000 python-freckle-client-0.5.0/freckle_client/tests/__init__.py
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)      657 2023-06-05 06:12:02.000000 python-freckle-client-0.5.0/pyproject.toml
+drwxr-xr-x   0 amandabizzinotto   (501) staff       (20)        0 2023-06-05 06:54:51.029338 python-freckle-client-0.5.0/python_freckle_client.egg-info/
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)     2056 2023-06-05 06:54:50.000000 python-freckle-client-0.5.0/python_freckle_client.egg-info/PKG-INFO
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)      414 2023-06-05 06:54:51.000000 python-freckle-client-0.5.0/python_freckle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)        1 2023-06-05 06:54:50.000000 python-freckle-client-0.5.0/python_freckle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)       47 2023-06-05 06:54:50.000000 python-freckle-client-0.5.0/python_freckle_client.egg-info/requires.txt
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)       15 2023-06-05 06:54:50.000000 python-freckle-client-0.5.0/python_freckle_client.egg-info/top_level.txt
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)       38 2023-06-05 06:54:51.029716 python-freckle-client-0.5.0/setup.cfg
+-rw-r--r--   0 amandabizzinotto   (501) staff       (20)     1918 2023-06-05 06:49:06.000000 python-freckle-client-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-freckle-client-0.4.0/PKG-INFO` & `python-freckle-client-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 Metadata-Version: 2.1
 Name: python-freckle-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A super simple Freckle/Noko API client implementation.
 Home-page: https://github.com/bitmazk/freckle-client
 Author: Martin Brochhaus
 Author-email: mbrochh@gmail.com
 License: The MIT License
-Description: Freckle Client
-        ==============
-        
-        A super simple Freckle/Noko API client implementation.
-        
-        Installation
-        ------------
-        
-        To get the latest stable release from PyPi
-        
-        .. code-block:: bash
-        
-            pip install python-freckle-client
-        
-        To get the latest commit from GitHub
-        
-        .. code-block:: bash
-        
-            pip install -e git+git://github.com/bitmazk/python-freckle-client.git#egg=freckle_client
-        
-        
-        Usage
-        -----
-        
-        Just import the client, create an instance and call the ``fetch_json`` method: 
-        
-        .. code-block:: python
-        
-            from freckle_client.client import FreckleClient
-        
-            client = FreckleClient('account_name', 'api_token')
-            entries = client.fetch_json(
-                'entries',
-                query_params={
-                    'per_page': 1000,
-                    'search[from]': '2015-01-01',
-                    'search[to]': '2015-01-31',
-                    'search[projects]': [1423, 24545, ],
-                }
-            )
-        
-        Or if you want to use the V2 API:
-        
-        .. code-block:: python
-        
-            from freckle_client.client import FreckleClientV2
-        
-            client = FreckleClientV2('access_token')
-            entries = client.fetch_json(
-                'entries',
-                query_params={
-                    'per_page': 1000,
-                    'search[from]': '2015-01-01',
-                    'search[to]': '2015-01-31',
-                    'search[projects]': [1423, 24545, ],
-                }
-            )
-        
-        
-        Contribute
-        ----------
-        
-        If you want to contribute to this project, please perform the following steps
-        
-        .. code-block:: bash
-        
-            # Fork this repository
-            # Clone your fork
-            mkvirtualenv -p python2.7 freckle-client
-            make develop
-        
-            git co -b feature_branch master
-            # Implement your feature and tests
-            git add . && git commit
-            git push -u origin feature_branch
-            # Send us a pull request for your feature branch
-        
 Keywords: nokotime,noko,api,client
 Platform: OS Independent
 Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS
+
+Freckle Client
+==============
+
+A super simple Freckle/Noko API client implementation.
+
+Installation
+------------
+
+To get the latest stable release from PyPi
+
+.. code-block:: bash
+
+    pip install python-freckle-client
+
+To get the latest commit from GitHub
+
+.. code-block:: bash
+
+    pip install -e git+git://github.com/bitmazk/python-freckle-client.git#egg=freckle_client
+
+
+Usage
+-----
+
+Just import the client, create an instance and call the ``fetch_json`` method: 
+
+.. code-block:: python
+
+    from freckle_client.client import FreckleClient
+
+    client = FreckleClient('account_name', 'api_token')
+    entries = client.fetch_json(
+        'entries',
+        query_params={
+            'per_page': 1000,
+            'search[from]': '2015-01-01',
+            'search[to]': '2015-01-31',
+            'search[projects]': [1423, 24545, ],
+        }
+    )
+
+Or if you want to use the V2 API:
+
+.. code-block:: python
+
+    from freckle_client.client import FreckleClientV2
+
+    client = FreckleClientV2('access_token')
+    entries = client.fetch_json(
+        'entries',
+        query_params={
+            'search[from]': '2015-01-01',
+            'search[to]': '2015-01-31',
+            'search[projects]': [1423, 24545, ],
+        }
+    )
+
+
+Contribute
+----------
+
+If you want to contribute to this project, please perform the following steps
+
+.. code-block:: bash
+
+    # Fork this repository
+    # Clone your fork
+    mkvirtualenv -p python3.8 freckle-client
+    make develop
+
+    git co -b feature_branch master
+    # Implement your feature and tests
+    git add . && git commit
+    git push -u origin feature_branch
+    # Send us a pull request for your feature branch
```

### Comparing `python-freckle-client-0.4.0/LICENSE` & `python-freckle-client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-freckle-client-0.4.0/python_freckle_client.egg-info/PKG-INFO` & `python-freckle-client-0.5.0/python_freckle_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 Metadata-Version: 2.1
 Name: python-freckle-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A super simple Freckle/Noko API client implementation.
 Home-page: https://github.com/bitmazk/freckle-client
 Author: Martin Brochhaus
 Author-email: mbrochh@gmail.com
 License: The MIT License
-Description: Freckle Client
-        ==============
-        
-        A super simple Freckle/Noko API client implementation.
-        
-        Installation
-        ------------
-        
-        To get the latest stable release from PyPi
-        
-        .. code-block:: bash
-        
-            pip install python-freckle-client
-        
-        To get the latest commit from GitHub
-        
-        .. code-block:: bash
-        
-            pip install -e git+git://github.com/bitmazk/python-freckle-client.git#egg=freckle_client
-        
-        
-        Usage
-        -----
-        
-        Just import the client, create an instance and call the ``fetch_json`` method: 
-        
-        .. code-block:: python
-        
-            from freckle_client.client import FreckleClient
-        
-            client = FreckleClient('account_name', 'api_token')
-            entries = client.fetch_json(
-                'entries',
-                query_params={
-                    'per_page': 1000,
-                    'search[from]': '2015-01-01',
-                    'search[to]': '2015-01-31',
-                    'search[projects]': [1423, 24545, ],
-                }
-            )
-        
-        Or if you want to use the V2 API:
-        
-        .. code-block:: python
-        
-            from freckle_client.client import FreckleClientV2
-        
-            client = FreckleClientV2('access_token')
-            entries = client.fetch_json(
-                'entries',
-                query_params={
-                    'per_page': 1000,
-                    'search[from]': '2015-01-01',
-                    'search[to]': '2015-01-31',
-                    'search[projects]': [1423, 24545, ],
-                }
-            )
-        
-        
-        Contribute
-        ----------
-        
-        If you want to contribute to this project, please perform the following steps
-        
-        .. code-block:: bash
-        
-            # Fork this repository
-            # Clone your fork
-            mkvirtualenv -p python2.7 freckle-client
-            make develop
-        
-            git co -b feature_branch master
-            # Implement your feature and tests
-            git add . && git commit
-            git push -u origin feature_branch
-            # Send us a pull request for your feature branch
-        
 Keywords: nokotime,noko,api,client
 Platform: OS Independent
 Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS
+
+Freckle Client
+==============
+
+A super simple Freckle/Noko API client implementation.
+
+Installation
+------------
+
+To get the latest stable release from PyPi
+
+.. code-block:: bash
+
+    pip install python-freckle-client
+
+To get the latest commit from GitHub
+
+.. code-block:: bash
+
+    pip install -e git+git://github.com/bitmazk/python-freckle-client.git#egg=freckle_client
+
+
+Usage
+-----
+
+Just import the client, create an instance and call the ``fetch_json`` method: 
+
+.. code-block:: python
+
+    from freckle_client.client import FreckleClient
+
+    client = FreckleClient('account_name', 'api_token')
+    entries = client.fetch_json(
+        'entries',
+        query_params={
+            'per_page': 1000,
+            'search[from]': '2015-01-01',
+            'search[to]': '2015-01-31',
+            'search[projects]': [1423, 24545, ],
+        }
+    )
+
+Or if you want to use the V2 API:
+
+.. code-block:: python
+
+    from freckle_client.client import FreckleClientV2
+
+    client = FreckleClientV2('access_token')
+    entries = client.fetch_json(
+        'entries',
+        query_params={
+            'search[from]': '2015-01-01',
+            'search[to]': '2015-01-31',
+            'search[projects]': [1423, 24545, ],
+        }
+    )
+
+
+Contribute
+----------
+
+If you want to contribute to this project, please perform the following steps
+
+.. code-block:: bash
+
+    # Fork this repository
+    # Clone your fork
+    mkvirtualenv -p python3.8 freckle-client
+    make develop
+
+    git co -b feature_branch master
+    # Implement your feature and tests
+    git add . && git commit
+    git push -u origin feature_branch
+    # Send us a pull request for your feature branch
```

### Comparing `python-freckle-client-0.4.0/setup.py` & `python-freckle-client-0.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- encoding: utf-8 -*-
+# flake8: noqa
+# pylint: skip-file
 """
 Python setup file for the freckle_client app.
 
 In order to register your app at pypi.python.org, create an account at
 pypi.python.org and login, then register your new app like so:
 
     python setup.py register
@@ -24,44 +26,50 @@
 freckle_client/__init__.py and re-run the above command.
 
 For more information on creating source distributions, see
 http://docs.python.org/2/distutils/sourcedist.html
 
 """
 import os
-from setuptools import setup, find_packages
-import freckle_client as app
 
+from setuptools import find_packages, setup
+
+import freckle_client as app
 
 dev_requires = [
-    'flake8',
+    "black",
+    "flake8",
+    "isort",
+    "mypy",
+    "pylint",
 ]
 
 install_requires = [
-    'requests',
+    "requests",
 ]
 
 
 def read(fname):
     try:
         return open(os.path.join(os.path.dirname(__file__), fname)).read()
     except IOError:
-        return ''
+        return ""
+
 
 setup(
     name="python-freckle-client",
     version=app.__version__,
-    description='A super simple Freckle/Noko API client implementation.',
-    long_description=read('README.rst'),
-    license='The MIT License',
-    platforms=['OS Independent'],
-    keywords='nokotime, noko, api, client',
-    author='Martin Brochhaus',
-    author_email='mbrochh@gmail.com',
+    description="A super simple Freckle/Noko API client implementation.",
+    long_description=read("README.rst"),
+    license="The MIT License",
+    platforms=["OS Independent"],
+    keywords="nokotime, noko, api, client",
+    author="Martin Brochhaus",
+    author_email="mbrochh@gmail.com",
     url="https://github.com/bitmazk/freckle-client",
     packages=find_packages(),
     include_package_data=True,
     install_requires=install_requires,
     extras_require={
-        'dev': dev_requires,
+        "dev": dev_requires,
     },
 )
```

### Comparing `python-freckle-client-0.4.0/CHANGELOG.txt` & `python-freckle-client-0.5.0/CHANGELOG.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+=== 0.5.0 ===
+
+* Handle successful No Content response
+* Handle pagination on the v2 API
+
 === 0.4.0 ===
 
 * Uses new application name & URL (nokotime.com)
 
 === 0.3.X ===
 
 * prepared app for Python3.x
```

### Comparing `python-freckle-client-0.4.0/README.rst` & `python-freckle-client-0.5.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
     from freckle_client.client import FreckleClientV2
 
     client = FreckleClientV2('access_token')
     entries = client.fetch_json(
         'entries',
         query_params={
-            'per_page': 1000,
             'search[from]': '2015-01-01',
             'search[to]': '2015-01-31',
             'search[projects]': [1423, 24545, ],
         }
     )
 
 
@@ -62,15 +61,15 @@
 
 If you want to contribute to this project, please perform the following steps
 
 .. code-block:: bash
 
     # Fork this repository
     # Clone your fork
-    mkvirtualenv -p python2.7 freckle-client
+    mkvirtualenv -p python3.8 freckle-client
     make develop
 
     git co -b feature_branch master
     # Implement your feature and tests
     git add . && git commit
     git push -u origin feature_branch
     # Send us a pull request for your feature branch
```

