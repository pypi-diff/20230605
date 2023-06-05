# Comparing `tmp/remlalib-0.0.6.tar.gz` & `tmp/remlalib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\remlalib-0.0.6.tar", last modified: Mon Jun  5 08:58:35 2023, max compression
+gzip compressed data, was "dist\remlalib-0.0.7.tar", last modified: Mon Jun  5 09:06:44 2023, max compression
```

## Comparing `remlalib-0.0.6.tar` & `remlalib-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 08:58:35.000000 remlalib-0.0.6/
--rw-rw-rw-   0        0        0     1043 2023-06-05 08:58:35.000000 remlalib-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 08:58:35.000000 remlalib-0.0.6/remlalib/
--rw-rw-rw-   0        0        0       45 2023-06-05 08:48:51.000000 remlalib-0.0.6/remlalib/__init__.py
--rw-rw-rw-   0        0        0       21 2023-06-05 08:54:56.000000 remlalib-0.0.6/remlalib/_version.py
--rw-rw-rw-   0        0        0      128 2023-06-05 08:58:28.000000 remlalib-0.0.6/remlalib/version_util.py
--rw-rw-rw-   0        0        0       40 2023-06-05 08:29:46.000000 remlalib-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-06-05 08:56:19.000000 remlalib-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:06:44.000000 remlalib-0.0.7/
+-rw-rw-rw-   0        0        0     1043 2023-06-05 09:06:44.000000 remlalib-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 09:06:44.000000 remlalib-0.0.7/remlalib/
+-rw-rw-rw-   0        0        0       45 2023-06-05 08:48:51.000000 remlalib-0.0.7/remlalib/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-06-05 09:06:40.000000 remlalib-0.0.7/remlalib/_version.py
+-rw-rw-rw-   0        0        0      133 2023-06-05 09:05:59.000000 remlalib-0.0.7/remlalib/version_util.py
+-rw-rw-rw-   0        0        0       40 2023-06-05 08:29:46.000000 remlalib-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1168 2023-06-05 09:06:35.000000 remlalib-0.0.7/setup.py
```

### Comparing `remlalib-0.0.6/PKG-INFO` & `remlalib-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: remlalib
-Version: 0.0.6
+Version: 0.0.7
 Summary: REMLA23 - Team 13 - Lib
 Home-page: https://github.com/remla23-team13/lib
 Author: Team 13
 Author-email: gasparsantosrocha@gmail.com
 License: MIT
 Download-URL: https://github.com/remla23-team13/lib
 Description: UNKNOWN
```

### Comparing `remlalib-0.0.6/setup.py` & `remlalib-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
   license='MIT',
   description = 'REMLA23 - Team 13 - Lib',
   author = 'Team 13',
   author_email = 'gasparsantosrocha@gmail.com',
   url = 'https://github.com/remla23-team13/lib',
   download_url = 'https://github.com/remla23-team13/lib',
   keywords = ['REMLA', 'Versioning'],
-  install_requires=[],
+  install_requires=[
+      'setuptools'
+  ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.1',
```

