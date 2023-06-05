# Comparing `tmp/remlalib-0.0.7.tar.gz` & `tmp/remlalib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\remlalib-0.0.7.tar", last modified: Mon Jun  5 09:06:44 2023, max compression
+gzip compressed data, was "remlalib-1.0.2.tar", last modified: Mon Jun  5 10:14:41 2023, max compression
```

## Comparing `remlalib-0.0.7.tar` & `remlalib-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:06:44.000000 remlalib-0.0.7/
--rw-rw-rw-   0        0        0     1043 2023-06-05 09:06:44.000000 remlalib-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 09:06:44.000000 remlalib-0.0.7/remlalib/
--rw-rw-rw-   0        0        0       45 2023-06-05 08:48:51.000000 remlalib-0.0.7/remlalib/__init__.py
--rw-rw-rw-   0        0        0       21 2023-06-05 09:06:40.000000 remlalib-0.0.7/remlalib/_version.py
--rw-rw-rw-   0        0        0      133 2023-06-05 09:05:59.000000 remlalib-0.0.7/remlalib/version_util.py
--rw-rw-rw-   0        0        0       40 2023-06-05 08:29:46.000000 remlalib-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1168 2023-06-05 09:06:35.000000 remlalib-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:14:41.439064 remlalib-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-05 10:14:27.000000 remlalib-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-05 10:14:41.439064 remlalib-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 10:14:27.000000 remlalib-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:14:41.439064 remlalib-1.0.2/remlalib/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-05 10:14:27.000000 remlalib-1.0.2/remlalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 10:14:27.000000 remlalib-1.0.2/remlalib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-05 10:14:27.000000 remlalib-1.0.2/remlalib/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:14:41.439064 remlalib-1.0.2/remlalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-05 10:14:41.000000 remlalib-1.0.2/remlalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-05 10:14:41.000000 remlalib-1.0.2/remlalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:14:41.000000 remlalib-1.0.2/remlalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 10:14:41.000000 remlalib-1.0.2/remlalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 10:14:41.000000 remlalib-1.0.2/remlalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 10:14:41.439064 remlalib-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-05 10:14:27.000000 remlalib-1.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `remlalib-0.0.7/PKG-INFO` & `remlalib-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 1.1
-Name: remlalib
-Version: 0.0.7
-Summary: REMLA23 - Team 13 - Lib
-Home-page: https://github.com/remla23-team13/lib
-Author: Team 13
-Author-email: gasparsantosrocha@gmail.com
-License: MIT
-Download-URL: https://github.com/remla23-team13/lib
-Description: UNKNOWN
-Keywords: REMLA,Versioning
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Metadata-Version: 2.1
+Name: remlalib
+Version: 1.0.2
+Summary: REMLA23 - Team 13 - Lib
+Home-page: https://github.com/remla23-team13/lib
+Download-URL: https://github.com/remla23-team13/lib
+Author: Team 13
+Author-email: gasparsantosrocha@gmail.com
+License: MIT
+Keywords: REMLA,Versioning
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.1
+Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE.txt
+
+REMLA23 - Team 13 - Lib
```

### Comparing `remlalib-0.0.7/setup.py` & `remlalib-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from distutils.core import setup
-setup(
-  name = 'remlalib',
-  packages = ['remlalib'],
-  version = open("remlalib/_version.py").readlines()[-1].split()[-1].strip("\"'"),
-  license='MIT',
-  description = 'REMLA23 - Team 13 - Lib',
-  author = 'Team 13',
-  author_email = 'gasparsantosrocha@gmail.com',
-  url = 'https://github.com/remla23-team13/lib',
-  download_url = 'https://github.com/remla23-team13/lib',
-  keywords = ['REMLA', 'Versioning'],
-  install_requires=[
-      'setuptools'
-  ],
-  classifiers=[
-    'Development Status :: 3 - Alpha',
-    'Intended Audience :: Developers',
-    'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.1',
-    'Programming Language :: Python :: 3.2',
-    'Programming Language :: Python :: 3.3',
-    'Programming Language :: Python :: 3.4',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-  ],
+from distutils.core import setup
+setup(
+  name = 'remlalib',
+  packages = ['remlalib'],
+  version = open("remlalib/_version.py").readlines()[-1].split()[-1].strip("\"'"),
+  license='MIT',
+  description = 'REMLA23 - Team 13 - Lib',
+  long_description= 'REMLA23 - Team 13 - Lib',
+  author = 'Team 13',
+  author_email = 'gasparsantosrocha@gmail.com',
+  url = 'https://github.com/remla23-team13/lib',
+  download_url = 'https://github.com/remla23-team13/lib',
+  keywords = ['REMLA', 'Versioning'],
+  install_requires=[
+      'setuptools'
+  ],
+  classifiers=[
+    'Development Status :: 3 - Alpha',
+    'Intended Audience :: Developers',
+    'Topic :: Software Development :: Build Tools',
+    'License :: OSI Approved :: MIT License',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.1',
+    'Programming Language :: Python :: 3.2',
+    'Programming Language :: Python :: 3.3',
+    'Programming Language :: Python :: 3.4',
+    'Programming Language :: Python :: 3.5',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+  ],
 )
```

