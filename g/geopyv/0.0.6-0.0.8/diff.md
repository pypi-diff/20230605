# Comparing `tmp/geopyv-0.0.6.tar.gz` & `tmp/geopyv-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopyv-0.0.6.tar", last modified: Fri May 19 15:00:56 2023, max compression
+gzip compressed data, was "geopyv-0.0.8.tar", last modified: Mon Jun  5 12:07:21 2023, max compression
```

## Comparing `geopyv-0.0.6.tar` & `geopyv-0.0.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.348039 geopyv-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-19 15:00:42.000000 geopyv-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-19 15:00:42.000000 geopyv-0.0.6/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-19 15:00:42.000000 geopyv-0.0.6/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 15:00:42.000000 geopyv-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-19 15:00:56.348039 geopyv-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-19 15:00:42.000000 geopyv-0.0.6/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   167778 2023-05-19 15:00:42.000000 geopyv-0.0.6/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-19 15:00:42.000000 geopyv-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-19 15:00:42.000000 geopyv-0.0.6/basictest.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-19 15:00:42.000000 geopyv-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 15:00:56.348039 geopyv-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-19 15:00:42.000000 geopyv-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.340039 geopyv-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.344039 geopyv-0.0.6/src/geopyv/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    28277 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.344039 geopyv-0.0.6/src/geopyv/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/geometry/exclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/geometry/meshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/geometry/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.344039 geopyv-0.0.6/src/geopyv/gui/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.348039 geopyv-0.0.6/src/geopyv/gui/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/selectors/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/selectors/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/selectors/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/selectors/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    71629 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    25568 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39385 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    47603 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/speckle.py
--rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.344039 geopyv-0.0.6/src/geopyv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-19 15:00:56.000000 geopyv-0.0.6/src/geopyv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-19 15:00:56.000000 geopyv-0.0.6/src/geopyv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:00:56.000000 geopyv-0.0.6/src/geopyv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-19 15:00:56.000000 geopyv-0.0.6/src/geopyv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 15:00:56.000000 geopyv-0.0.6/src/geopyv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.664438 geopyv-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-05 12:07:12.000000 geopyv-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-05 12:07:12.000000 geopyv-0.0.8/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-05 12:07:12.000000 geopyv-0.0.8/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 12:07:12.000000 geopyv-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-05 12:07:21.664438 geopyv-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-05 12:07:12.000000 geopyv-0.0.8/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   167782 2023-06-05 12:07:12.000000 geopyv-0.0.8/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-05 12:07:12.000000 geopyv-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-06-05 12:07:12.000000 geopyv-0.0.8/basictest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 12:07:12.000000 geopyv-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 12:07:21.664438 geopyv-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-05 12:07:12.000000 geopyv-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.652438 geopyv-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.660438 geopyv-0.0.8/src/geopyv/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.664438 geopyv-0.0.8/src/geopyv/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/geometry/exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/geometry/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/geometry/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.664438 geopyv-0.0.8/src/geopyv/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.664438 geopyv-0.0.8/src/geopyv/gui/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/selectors/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/selectors/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/selectors/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/gui/selectors/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71779 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27589 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39437 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49305 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/speckle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-06-05 12:07:12.000000 geopyv-0.0.8/src/geopyv/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:07:21.664438 geopyv-0.0.8/src/geopyv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-05 12:07:21.000000 geopyv-0.0.8/src/geopyv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-05 12:07:21.000000 geopyv-0.0.8/src/geopyv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:07:21.000000 geopyv-0.0.8/src/geopyv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-05 12:07:21.000000 geopyv-0.0.8/src/geopyv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 12:07:21.000000 geopyv-0.0.8/src/geopyv.egg-info/top_level.txt
```

### Comparing `geopyv-0.0.6/.gitignore` & `geopyv-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/CMakeLists.txt` & `geopyv-0.0.8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/LICENSE` & `geopyv-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/PKG-INFO` & `geopyv-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopyv
-Version: 0.0.6
+Version: 0.0.8
 Summary: A PIV/DIC analysis package for Python.
 Author-email: Sam Stanier <sas229@cam.ac.uk>, Jonathan Smith <jdks2@cam.ac.uk>
 Project-URL: Homepage, https://github.com/sas229/geopyv
 Project-URL: Bug Tracker, https://github.com/sas229/geopyv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `geopyv-0.0.6/Pipfile` & `geopyv-0.0.8/Pipfile`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/Pipfile.lock` & `geopyv-0.0.8/Pipfile.lock`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969774514167037%*

 * *Differences: {"'default'": "{'docutils': {'hashes': "*

 * *              "['sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6', "*

 * *              "'sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b'], "*

 * *              "'version': '==0.20.1'}, 'pre-commit': {'hashes': "*

 * *              "['sha256:66e37bec2d882de1f17f88075047ef8962581f83c234ac08da21a0c58953d1f0', "*

 * *              "'sha256:8056bc52181efadf4aac792b1f4f255dfd2fb5a350ded7335d251a68561e8cb6'], "*

 * *              "'version': '==3.3. […]*

```diff
@@ -281,19 +281,19 @@
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:a428f10de4de4774389734c986a01b4af2d802d26717108b0f1b9356862937c5",
-                "sha256:f75a5a52fbcacd81b47e42888ad2b380748aaccfb3f13af0fe69deb759f01eb6"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.20"
+            "version": "==0.20.1"
         },
         "filelock": {
             "hashes": [
                 "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
                 "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
@@ -773,19 +773,19 @@
                 "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.5.1"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:218e9e3f7f7f3271ebc355a15598a4d3893ad9fc7b57fe446db75644543323b9",
-                "sha256:733f78c9a056cdd169baa6cd4272d51ecfda95346ef8a89bf93712706021b907"
+                "sha256:66e37bec2d882de1f17f88075047ef8962581f83c234ac08da21a0c58953d1f0",
+                "sha256:8056bc52181efadf4aac792b1f4f255dfd2fb5a350ded7335d251a68561e8cb6"
             ],
             "index": "pypi",
-            "version": "==3.3.1"
+            "version": "==3.3.2"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
                 "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
             "markers": "python_version >= '3.6'",
@@ -805,19 +805,19 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:bc6926958617caafb8d3e07180f53aef29bd43ce913952c0991c4793b673b07c",
-                "sha256:bf0d2844c75e9510119142cfc4aba20c0043121a736010f47f2500a7fb2134c0"
+                "sha256:3e4710eac2986826fa05c3e52671a0fd403280458e64545c9ac4720ddc9c6302",
+                "sha256:840c304e2d0928d6273eadea1ef28bf0a6447fb308ae8b683dbd67042fd4b7ca"
             ],
             "markers": "python_full_version >= '3.6.8'",
-            "version": "==3.1.0b1"
+            "version": "==3.1.0b2"
         },
         "pyside6": {
             "hashes": [
                 "sha256:13e8e96aa7a89840575505f50b9635e6450bf413ff46288d1085b3a9f8b225c1",
                 "sha256:5102c57841b15facb0aeca1f23d689ebc528a609bf5fb907f1ef2747f6415001",
                 "sha256:7242fe09aaeb3399152fa1c6c25098b93df945620a4bd81a37de0ecb2f64fd5d",
                 "sha256:c1c7244a4e83b3a4ea965f4a85776ebc64fa3c9b4af77ad70b22e64ccec3d451",
@@ -1004,19 +1004,19 @@
                 "sha256:ebf15355a4dba46037dfd65b7350f014ceb1f13c05e814eda2c9f5fd731afc08"
             ],
             "index": "pypi",
             "version": "==0.12.2"
         },
         "setuptools": {
             "hashes": [
-                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
-                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
+                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
+                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.7.2"
+            "version": "==67.8.0"
         },
         "shapely": {
             "hashes": [
                 "sha256:01224899ff692a62929ef1a3f5fe389043e262698a708ab7569f43a99a48ae82",
                 "sha256:05c51a29336e604c084fb43ae5dbbfa2c0ef9bd6fedeae0a0d02c7b57a56ba46",
                 "sha256:09d6c7763b1bee0d0a2b84bb32a4c25c6359ad1ac582a62d8b211e89de986154",
                 "sha256:193a398d81c97a62fc3634a1a33798a58fd1dcf4aead254d080b273efbb7e3ff",
@@ -1155,18 +1155,18 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "trimesh": {
             "hashes": [
-                "sha256:bfc97269e4cd358b418521aedc05bc9f7b9ea4e819ed843126c980c9663b59c7",
-                "sha256:fa016a6406c62e834374e99bc4494ac1bd1063b0497ce519543efcf3c4fa794f"
+                "sha256:c2d1addcf502522488890440dcdc4ed673c4df95d00e2a567ebc1229d0c186d1",
+                "sha256:f2a22d1e3dba12947927b285dbba216b30ff8993a3f947d1eca5742765fe594a"
             ],
-            "version": "==3.21.6"
+            "version": "==3.21.7"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version < '3.11'",
@@ -1518,19 +1518,19 @@
                 "sha256:99522ca3e365cac527b44bde033f64c6945d90eb9f769703caaec52b09bbd3ff"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.8.0"
         },
         "docutils": {
             "hashes": [
-                "sha256:a428f10de4de4774389734c986a01b4af2d802d26717108b0f1b9356862937c5",
-                "sha256:f75a5a52fbcacd81b47e42888ad2b380748aaccfb3f13af0fe69deb759f01eb6"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.20"
+            "version": "==0.20.1"
         },
         "exceptiongroup": {
             "hashes": [
                 "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
@@ -2093,19 +2093,19 @@
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:218e9e3f7f7f3271ebc355a15598a4d3893ad9fc7b57fe446db75644543323b9",
-                "sha256:733f78c9a056cdd169baa6cd4272d51ecfda95346ef8a89bf93712706021b907"
+                "sha256:66e37bec2d882de1f17f88075047ef8962581f83c234ac08da21a0c58953d1f0",
+                "sha256:8056bc52181efadf4aac792b1f4f255dfd2fb5a350ded7335d251a68561e8cb6"
             ],
             "index": "pypi",
-            "version": "==3.3.1"
+            "version": "==3.3.2"
         },
         "prompt-toolkit": {
             "hashes": [
                 "sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b",
                 "sha256:45ea77a2f7c60418850331366c81cf6b5b9cf4c7fd34616f733c5427e6abbb1f"
             ],
             "markers": "python_full_version >= '3.7.0'",
@@ -2184,19 +2184,19 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:bc6926958617caafb8d3e07180f53aef29bd43ce913952c0991c4793b673b07c",
-                "sha256:bf0d2844c75e9510119142cfc4aba20c0043121a736010f47f2500a7fb2134c0"
+                "sha256:3e4710eac2986826fa05c3e52671a0fd403280458e64545c9ac4720ddc9c6302",
+                "sha256:840c304e2d0928d6273eadea1ef28bf0a6447fb308ae8b683dbd67042fd4b7ca"
             ],
             "markers": "python_full_version >= '3.6.8'",
-            "version": "==3.1.0b1"
+            "version": "==3.1.0b2"
         },
         "pyside6": {
             "hashes": [
                 "sha256:13e8e96aa7a89840575505f50b9635e6450bf413ff46288d1085b3a9f8b225c1",
                 "sha256:5102c57841b15facb0aeca1f23d689ebc528a609bf5fb907f1ef2747f6415001",
                 "sha256:7242fe09aaeb3399152fa1c6c25098b93df945620a4bd81a37de0ecb2f64fd5d",
                 "sha256:c1c7244a4e83b3a4ea965f4a85776ebc64fa3c9b4af77ad70b22e64ccec3d451",
@@ -2416,19 +2416,19 @@
                 "sha256:fae8a7b898c42dffe3f7361c40d5952b6bf32d10c4569098d276b4c547905ee1"
             ],
             "index": "pypi",
             "version": "==1.10.1"
         },
         "setuptools": {
             "hashes": [
-                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
-                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
+                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
+                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.7.2"
+            "version": "==67.8.0"
         },
         "shiboken6": {
             "hashes": [
                 "sha256:1bba668221a5cf40186cea93ced018cf788d7476d50968a3f073ebbe41ce712d",
                 "sha256:2d7fe6534a51ec9c96b82fc6275cf75e85ab29276a9778aed756465f81adf0c1",
                 "sha256:46ff977f96c9d45dba3c3a313628356fd40e4423bb65bf2d9870b73396fad8be",
                 "sha256:6e2874ea013d4cea7819935977bffa4c634ebcaabcb5287798df9f0c2f10c4c0",
```

### Comparing `geopyv-0.0.6/README.md` & `geopyv-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/basictest.py` & `geopyv-0.0.8/basictest.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/pyproject.toml` & `geopyv-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "cmake",
     "ninja"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geopyv"
-version = "0.0.6"
+version = "0.0.8"
 authors = [
   { name="Sam Stanier", email="sas229@cam.ac.uk" },
   { name="Jonathan Smith", email="jdks2@cam.ac.uk" },
 ]
 description = "A PIV/DIC analysis package for Python."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `geopyv-0.0.6/src/geopyv/__init__.py` & `geopyv-0.0.8/src/geopyv/__init__.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/calibration.py` & `geopyv-0.0.8/src/geopyv/calibration.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/check.py` & `geopyv-0.0.8/src/geopyv/check.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/field.py` & `geopyv-0.0.8/src/geopyv/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -324,14 +324,15 @@
         series=None,
         target_particles=1000,
         track=True,
         boundary=None,
         exclusions=[],
         coordinates=None,
         volumes=None,
+        stresses=np.zeros(6),
     ):
         """
         Initialisation of geopyv field object.
 
         Parameters
         ----------
         series : gp.sequence.Sequence object or gp.mesh.Mesh object
@@ -348,14 +349,23 @@
             List to define the particle auto-distribution mesh exclusions.
             Shape of `numpy.ndarray` (N,2).
         coordinates : numpy.ndarray (N,2), optional
             Array of coordinates to define the initial particle positions.
         volumes : numpy.ndarray (N,), optional
             Array of volumes for particle representation.
             Defaults to np.ones(N) i.e. measure of volumetric strain.
+        stresses : numpy.ndarray (N,6) or (2,6) or (6,), optional.
+            Stress state specification. If:
+            (N,6) - individual particle specification (where N is the number
+                    of particles).
+            (2,6) - linearly varying stress field with depth (1st row and 2nd
+                    row vertically highest and lowest respectively, according
+                    to the boundary definition.
+            (6,)  - uniform stress field.
+            Defaults to np.zeros(6).
 
         Note ::
         Two kwargs groups for particle distribution:
         if coordinates is not None:
             1. User-defined : coordinates, volumes.
         else:
             2. Auto-distributed: boundary, exclusions, target_particles.
@@ -465,14 +475,36 @@
                 self._report(check, "TypeError")
         if volumes:
             self._report(gp.check._check_dim(volumes, "volumes", 1), "ValueError")
             self._report(
                 gp.check._check_axis(volumes, "volumes", 0, [np.shape(coordinates)[0]]),
                 "ValueError",
             )
+        check = gp.check._check_type(stresses, "stresses", [np.ndarray])
+        if check:
+            try:
+                stresses = np.asarray(stresses)
+                self._report(
+                    gp.check._conversion(stresses, "stresses", np.ndarray, False),
+                    "Warning",
+                )
+            except Exception:
+                self._report(check, "TypeError")
+        if coordinates is not None:
+            self._report(
+                gp.check._check_axis(
+                    stresses, "stresses", 0, [6, 2, np.shape(coordinates)[0]]
+                ),
+                "ValueError",
+            )
+        else:
+            self._report(
+                gp.check._check_axis(stresses, "stresses", 0, [6, 2]), "ValueError"
+            )
+
         self._report(gp.check._check_type(track, "track", [bool]), "TypeError")
 
         # Store.
         if series.data["type"] == "Sequence":
             self._series_type = "Sequence"
             if "file_settings" in series.data:
                 if series.data["file_settings"]["save_by_reference"]:
@@ -583,30 +615,34 @@
                 "Generating mesh using gmsh with approximately {n} particles.".format(
                     n=self._target_particles
                 )
             )
 
             self._initial_mesh()
             self._distribute_particles()
+            self._stress_state(stresses)
             log.info(
                 "Field generated with {p} particles.".format(p=len(self._coordinates))
             )
             self._field = {
                 "nodes": self._nodes,
                 "elements": self._elements,
                 "coordinates": self._coordinates,
                 "volumes": self._volumes,
+                "stresses": self._stresses,
             }
         else:
             self._coordinates = coordinates
             self._volumes = volumes
+            self._stress_state(stresses)
             log.info("Using user-specified field.")
             self._field = {
                 "coordinates": self._coordinates,
                 "volumes": self._volumes,
+                "stresses": self._stresses,
             }
 
         self.data.update({"field": self._field})
         self._initialised = True
 
     def _initial_mesh(self):
         """
@@ -657,15 +693,21 @@
     def _distribute_particles(self):
         self._coordinates = np.mean(self._nodes[self._elements[:, :3]], axis=1)
         M = np.ones((len(self._elements[:, :3]), 3, 3))
         M[:, 1] = self._nodes[self._elements[:, :3]][:, :, 0]
         M[:, 2] = self._nodes[self._elements[:, :3]][:, :, 1]
         self._volumes = abs(0.5 * np.linalg.det(M))
 
-    def solve(self, *, model=None, statev=None, props=None):
+    def solve(
+        self,
+        *,
+        model=None,
+        state=None,
+        parameters=None,
+    ):
         """
         Method to solve for the field.
 
         Returns
         -------
         solved : bool
             Boolean to indicate if the particle instances have been solved.
@@ -677,18 +719,19 @@
             particle_no, dual_line=True, bar="blocks", title="Solving particles..."
         ) as bar:
             for i in range(particle_no):
                 particle = gp.particle.Particle(
                     series=self._series,
                     coordinate_0=self._coordinates[i],
                     volume_0=self._volumes[i],
+                    stress_0=self._stresses[i],
                     track=self._track,
                 )
                 _particle_solved = particle.solve(
-                    model=model, statev=statev, props=props
+                    model=model, state=state, parameters=parameters
                 )
                 if _particle_solved is False:
                     self._unsolvable = True
                     self.data["unsolvable"] = self._unsolvable
                     return self.solved
                 self._particles[i] = particle.data
                 self._vol_totals += self._particles[i]["results"]["volumes"]
@@ -702,14 +745,27 @@
             self.data.update({"works": self._works})
 
         self.data.update({"particles": self._particles, "volumes": self._vol_totals})
         self.solved = True
         self.data["solved"] = self.solved
         return self.solved
 
+    def _stress_state(self, stresses):
+        if np.shape(stresses)[0] == np.shape(self._coordinates)[0]:
+            self._stresses = stresses
+        elif np.shape(stresses)[0] == 2:
+            self._stresses = stresses[0] + (stresses[1] - stresses[0]) * (
+                (
+                    (self._coordinates[:, 1] - np.min(self._boundary[:, 1]))
+                    / (np.max(self._boundary[:, 1]) - np.min(self._boundary[:, 1]))
+                )[:, np.newaxis]
+            )
+        else:
+            self._stresses = np.tile(stresses, (np.shape(self._coordinates)[0], 1))
+
     @staticmethod
     def _uniform_remesh(
         size,
         boundary,
         segments,
         curves,
         target_particles,
```

### Comparing `geopyv-0.0.6/src/geopyv/geometry/exclusions.py` & `geopyv-0.0.8/src/geopyv/geometry/exclusions.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/geometry/meshing.py` & `geopyv-0.0.8/src/geopyv/geometry/meshing.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/geometry/utilities.py` & `geopyv-0.0.8/src/geopyv/geometry/utilities.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/gui/selectors/coordinate.py` & `geopyv-0.0.8/src/geopyv/gui/selectors/coordinate.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/gui/selectors/file.py` & `geopyv-0.0.8/src/geopyv/gui/selectors/file.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/gui/selectors/folder.py` & `geopyv-0.0.8/src/geopyv/gui/selectors/folder.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/gui/selectors/image.py` & `geopyv-0.0.8/src/geopyv/gui/selectors/image.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/image.py` & `geopyv-0.0.8/src/geopyv/image.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/io.py` & `geopyv-0.0.8/src/geopyv/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     .. note::
         * Any .pyv object can be loaded with this function.
         * The data object will be loaded into a `ObjectResults` instance where
           `Object` represents the instance type that generated the data. For example,
           data from a `Subset` instance will be loaded into a `SubsetResults` instance.
 
     """
-    if directory is None:
+    cwd = os.getcwd()
+    if directory is None and cwd not in filename:
         directory = os.getcwd()
     if filename is None:
         dialog = gp.gui.selectors.file.FileSelector()
         filepath = dialog.get_path("Select geopyv data file", directory)
     else:
         ext = ".pyv"
         # filepath = filename + ext
@@ -98,15 +99,15 @@
             "File does not exist at the path supplied:\n{filepath}".format(
                 filepath=filepath
             )
         )
         raise FileExistsError
 
 
-def save(*, object, filename=None):
+def save(*, object, directory=None, filename=None):
     """
 
     Function to save data from a geopyv object. If no filename is
     provided, the host OS default file browser will be used to allow
     the user to choose a filename and storage location.
 
 
@@ -119,15 +120,17 @@
 
 
     .. note::
         * Any geopyv object can be passed to this function.
         * Do not include the .pyv extension in the `filename` argument.
 
     """
-    directory = os.getcwd()
+    cwd = os.getcwd()
+    if directory is None and cwd not in filename:
+        directory = os.getcwd()
     if filename is None:
         log.error(
             "No filename provided."
         )  # Add a method to select the filename here...
         return False
     if isinstance(object, gp.object.Object):
         solved = object.data["solved"]
@@ -236,15 +239,15 @@
 
     Private method to open a file dialog and select a folder.
 
     """
     directory = os.getcwd()
     dialog = gp.gui.selectors.folder.FolderSelector()
     folder_path = dialog.get_path(directory, message)
-    return folder_path
+    return folder_path[len(directory) :]
 
 
 def _get_image_dir():
     """
 
     Private method to get the `image_dir`.
```

### Comparing `geopyv-0.0.6/src/geopyv/log.py` & `geopyv-0.0.8/src/geopyv/log.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/mesh.py` & `geopyv-0.0.8/src/geopyv/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -904,28 +904,32 @@
         """
         # Check if solved.
         if self.data["solved"] is True:
             log.error("Mesh has already been solved. Cannot be solved again.")
             return
 
         # Check inputs.
+        if template is None:
+            template = gp.templates.Circle(50)
+        types = [gp.templates.Circle, gp.templates.Square]
+        self._report(gp.check._check_type(template, "template", types), "TypeError")
         if self._report(
             gp.check._check_type(seed_coord, "seed_coord", [np.ndarray]), "Warning"
         ):
-            seed_coord = gp.gui.selectors.coordinate.CoordinateSelector()
+            selector = gp.gui.selectors.coordinate.CoordinateSelector()
+            seed_coord = selector.select(self._f_img, template)
         elif self._report(gp.check._check_dim(seed_coord, "seed_coord", 1), "Warning"):
-            seed_coord = gp.gui.selectors.coordinate.CoordinateSelector()
+            selector = gp.gui.selectors.coordinate.CoordinateSelector()
+            seed_coord = selector.select(self._f_img, template)
         elif self._report(
             gp.check._check_axis(seed_coord, "seed_coord", 0, [2]), "Warning"
         ):
-            seed_coord = gp.gui.selectors.coordinate.CoordinateSelector()
-        if template is None:
-            template = gp.templates.Circle(50)
-        types = [gp.templates.Circle, gp.templates.Square]
-        self._report(gp.check._check_type(template, "template", types), "TypeError")
+            selector = gp.gui.selectors.coordinate.CoordinateSelector()
+            seed_coord = selector.select(self._f_img, template)
+
         check = gp.check._check_type(max_norm, "max_norm", [float])
         if check:
             try:
                 max_norm = float(max_norm)
                 self._report(
                     gp.check._conversion(max_norm, "max_norm", float), "Warning"
                 )
@@ -1508,15 +1512,14 @@
         """
 
         A = np.ones((np.shape(self._elements)[0], 3, 4))
         A[:, 1:, 0] = np.mean(self._nodes[self._elements], axis=1)
         A[:, 1:, 1:] = self._nodes[self._elements][:, :3, :2].transpose(0, 2, 1)
 
         return A
-        # return zeta, eta, theta, A
 
     def _shape_function(self):
         if self._mesh_order == 1:
             N = np.asarray([1 / 3, 1 / 3, 1 / 3])
             dN = np.asarray([[1, 0, -1], [0, 1, -1]])
             d2N = None
         elif self._mesh_order == 2:
```

### Comparing `geopyv-0.0.6/src/geopyv/particle.py` & `geopyv-0.0.8/src/geopyv/particle.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 import logging
 import numpy as np
 import geopyv as gp
 from geopyv.object import Object
 import re
 import shapely
 from alive_progress import alive_bar
+import math
+
+try:
+    import models
+except Exception:
+    pass
 
 log = logging.getLogger(__name__)
 
 
 class ParticleBase(Object):
     """
     Particle base class to be used as a mixin. Contains plot functionality.
@@ -218,14 +224,15 @@
                     quantity,
                     "quantity",
                     [
                         "coordinates",
                         "warps",
                         "volumes",
                         "stresses",
+                        "works",
                     ],
                 ),
                 "ValueError",
             )
         self._report(
             gp.check._check_type(components, "components", [list, type(None)]),
             "TypeError",
@@ -287,15 +294,15 @@
 
     def __init__(
         self,
         *,
         series=None,
         coordinate_0=np.zeros(2),
         warp_0=np.zeros(12),
-        stress_0=np.zeros(3),
+        stress_0=np.zeros(6),
         volume_0=1.0,
         track=True,
     ):
         """Initialisation of geopyv particle object.
 
         Parameters
         ----------
@@ -325,26 +332,15 @@
                     gp.sequence.SequenceResults,
                     gp.mesh.Mesh,
                     gp.mesh.MeshResults,
                 ],
             ),
             "TypeError",
         )
-        if self._report(
-            gp.check._check_type(coordinate_0, "coordinate_0", [np.ndarray]), "Warning"
-        ):
-            coordinate_0 = gp.gui.selectors.coordinate.CoordinateSelector()
-        elif self._report(
-            gp.check._check_dim(coordinate_0, "coordinate_0", 1), "Warning"
-        ):
-            coordinate_0 = gp.gui.selectors.coordinate.CoordinateSelector()
-        elif self._report(
-            gp.check._check_axis(coordinate_0, "coordinate_0", 0, [2]), "Warning"
-        ):
-            coordinate_0 = gp.gui.selectors.coordinate.CoordinateSelector()
+
         check = gp.check._check_type(warp_0, "warp_0", [np.ndarray])
         if check:
             try:
                 warp_0 = np.asarray(warp_0)
                 self._report(
                     gp.check._conversion(warp_0, "warp_0", np.ndarray), "Warning"
                 )
@@ -387,27 +383,48 @@
             else:
                 self._series = series.data["meshes"]
         else:
             self._series_type = "Mesh"
             self._series = np.asarray([series.data])
         self._mesh_order = self._series[0]["mesh_order"]
         self._track = track
+        if self._report(
+            gp.check._check_type(coordinate_0, "coordinate_0", [np.ndarray]), "Warning"
+        ):
+            selector = gp.gui.selectors.coordinate.CoordinateSelector()
+            f_img = gp.image.Image(filepath=self._series[0]["images"]["f_img"])
+            coordinate_0 = selector.select(f_img, gp.templates.Circle(20))
+        elif self._report(
+            gp.check._check_dim(coordinate_0, "coordinate_0", 1), "Warning"
+        ):
+            selector = gp.gui.selectors.coordinate.CoordinateSelector()
+            f_img = gp.image.Image(filepath=self._series[0]["images"]["f_img"])
+            coordinate_0 = selector.select(f_img, gp.templates.Circle(20))
+        elif self._report(
+            gp.check._check_axis(coordinate_0, "coordinate_0", 0, [2]), "Warning"
+        ):
+            selector = gp.gui.selectors.coordinate.CoordinateSelector()
+            f_img = gp.image.Image(filepath=self._series[0]["images"]["f_img"])
+            coordinate_0 = selector.select(f_img, gp.templates.Circle(20))
 
         if self._series[0]["mask"][int(coordinate_0[1]), int(coordinate_0[0])] == 0:
             log.warning(
                 "`coordinate_0` keyword argument value out of boundary.\n"
                 "Select `coordinate_0`..."
             )
-            coordinate_0 = gp.gui.selectors.coordinate.CoordinateSelector()
+            selector = gp.gui.selectors.coordinate.CoordinateSelector()
+            f_img = gp.image.Image(filepath=self._series[0]["images"]["f_img"])
+            coordinate_0 = selector.select(f_img, gp.templates.Circle(20))
 
         self._coordinates = np.zeros((len(self._series) + 1, 2))
         self._warps = np.zeros((len(self._series) + 1, 6 * self._mesh_order))
         self._volumes = np.zeros(len(self._series) + 1)
-        self._stresses = np.zeros((len(self._series) + 1, 3))
+        self._stresses = np.zeros((len(self._series) + 1, 6))
         self._works = np.zeros(len(self._series) + 1)
+        self._strains = np.zeros((len(self._series) + 1, 6))
 
         self._coordinates[0] = coordinate_0
         self._warps[0] = warp_0[: np.shape(self._warps)[1]]
         self._volumes[0] = volume_0
         self._stresses[0] = stress_0
 
         self._reference_index = 0
@@ -421,24 +438,26 @@
             "track": self._track,
             "coordinate_0": self._coordinates[0],
             "warp_0": self._warps[0],
             "volume_0": self._volumes[0],
             "image_0": self._series[0]["images"]["f_img"],
         }
 
-    def solve(self, *, model=None, statev=None, props=None):  # model, statev, props):
+    def solve(
+        self, *, model=None, state=None, parameters=None
+    ):  # model, state, parameters):
         """
 
         Method to solve for the particle.
 
         """
-        self.data.update({"props": props, "statev": statev})
+        self.data.update({"parameters": parameters, "state": state})
         self.solved += self._strain_path()
         if model:
-            self.solved += self._stress_path(model, statev, props)
+            self.solved += self._stress_path(model, state, parameters)
         self._results = {
             "coordinates": self._coordinates,
             "warps": self._warps,
             "volumes": self._volumes,
             "stresses": self._stresses,
             "works": self._works,
         }
@@ -461,15 +480,15 @@
         """
         elements = self._series[m]["elements"]
         nodes = self._series[m]["nodes"]
         centroids = self._series[m]["centroids"]
         flag = False
         diff = centroids - self._coordinates[self._reference_index]
         dist = np.einsum("ij,ij->i", diff, diff)
-        dist_sorted = np.argpartition(dist, 10)
+        dist_sorted = np.argpartition(dist, math.ceil(0.05 * len(dist)))
         for index in dist_sorted:
             poly = shapely.Polygon(nodes[elements[index]][:3])
             point = shapely.Point(self._coordinates[self._reference_index])
             if poly.intersects(point):
                 flag = True
                 break
         if flag is False:
@@ -642,82 +661,110 @@
                     ],
                     [dz[1, 0] ** 2, 2 * dz[1, 0] * dz[1, 1], dz[1, 1] ** 2],
                 ]
             )
 
             self._warp_inc[6:] = (K_x_inv @ K_u).flatten()
 
-    def _strain_path(self):
-        """
-        Private method to calculate the particle strain path.
+    def _check_update(self, m):
+        if int(
+            re.findall(
+                r"\d+",
+                self._series[self._reference_index]["images"]["f_img"],
+            )[-1]
+        ) != int(re.findall(r"\d+", self._series[m]["images"]["f_img"])[-1]):
+            self._reference_index = m
+            self._reference_update_register.append(m)
 
-        """
+    def _strain_path(self):
         self._reference_update_register = []
+        self._incs = np.zeros((len(self._series) + 1, 6 * self._mesh_order))
         for m in range(np.shape(self._series)[0]):
-            # Reference update check.
-            if int(
-                re.findall(
-                    r"\d+",
-                    self._series[self._reference_index]["images"]["f_img"],
-                )[-1]
-            ) != int(re.findall(r"\d+", self._series[m]["images"]["f_img"])[-1]):
-                self._reference_index = m
-                self._reference_update_register.append(m)
-            # Mesh bearings.
+            self._check_update(m)
             tri_idx = self._element_locator(m)
-            # Interpolation.
             self._warp_increment(m, tri_idx)
-            # print(self._warp_inc)
-            # Updates.
+            self._incs[m + 1] = self._warp_inc
             self._coordinates[m + 1] = self._coordinates[
                 self._reference_index
             ] + self._warp_inc[:2] * int(self._track)
-            self._warps[m + 1] = self._warps[self._reference_index] + self._warp_inc
-            self._volumes[m + 1] = (
-                self._volumes[self._reference_index]
-                * (1 + self._warp_inc[2])
-                * (1 + self._warp_inc[5])
+            self._warps[m + 1, :2] = (
+                self._warps[self._reference_index, :2] + self._warp_inc[:2]
             )
-
-        return True
-
-    def _stress_path(self, model, statev, props):
-        if model == "Hooke":
-            self._E = props["E"]
-            self._G = props["G"]
-            self._nu = props["nu"]
-            stiffness = np.asarray(
-                [
-                    [
-                        self._E / (1 - self._nu**2),
-                        self._E * self._nu / (1 - self._nu**2),
-                        0,
-                    ],
-                    [
-                        self._E * self._nu / (1 - self._nu**2),
-                        self._E / (1 - self._nu**2),
-                        0,
-                    ],
-                    [0, 0, self._G],
-                ]
+            self._warps[m + 1, 2] = self._warps[self._reference_index, 2] + np.log(
+                1 + self._warp_inc[2]
+            )
+            self._warps[m + 1, 3] = (
+                self._warps[self._reference_index, 3] + self._warp_inc[3]
             )
-            delta_ep = np.zeros((np.shape(self._warps)[0] - 1, 3))
-            delta_ep[:, 0] = np.diff(self._warps[:, 2])
-            delta_ep[:, 1] = np.diff(self._warps[:, 5])
-            delta_ep[:, 2] = np.diff((self._warps[:, 3] + self._warps[:, 4]))
-            # delta_vol = np.diff(self._volumes)
-            self._stresses[1:] = self._stresses[0] + np.cumsum(
-                delta_ep @ stiffness, axis=0
+            self._warps[m + 1, 4] = (
+                self._warps[self._reference_index, 4] + self._warp_inc[4]
             )
-            self._works[1:] = (
-                np.sum(self._stresses[1:] * delta_ep, axis=-1) * self._volumes[1:]
+            self._warps[m + 1, 5] = self._warps[self._reference_index, 5] + np.log(
+                1 + self._warp_inc[5]
             )
+            self._volumes[m + 1] = self._volumes[self._reference_index] * (
+                (1 + self._warp_inc[2]) * (1 + self._warp_inc[5])
+                - self._warp_inc[3] * self._warp_inc[4]
+            )
+        self._strain_def()
+        return True
+
+    def _stress_path(self, model, state, parameters):
+        if model == "LinearElastic":
+            # Put input checks here!
+            model = models.LinearElastic(
+                parameters=parameters,
+                state=state,
+                # log_severity = "verbose"
+            )
+        if model == "MCC":
+            # Put input checks here!
+            model = models.MCC(
+                parameters=parameters,
+                state=state,
+                # log_severity = "verbose"
+            )
+        elif model == "SMCC":
+            # Put input checks here!
+            model = models.SMCC(
+                parameters=parameters,
+                state=state,
+                # log_severity = "verbose"
+            )
+        strain_incs = np.diff(self._strains, axis=0)
+        ps = []
+        qs = []
+        model.set_sigma_prime_tilde(self._stresses[0].T)
+        model.set_Delta_epsilon_tilde(strain_incs[0])
+        ps.append(model.p_prime)
+        qs.append(model.q)
+        for i in range(np.shape(self._series)[0]):
+            try:
+                model.set_sigma_prime_tilde(self._stresses[i].T)
+                model.set_Delta_epsilon_tilde(-1 * strain_incs[i])
+                model.solve()
+            except Exception:
+                log.error("geomat error. Stress path curtailed.")
+                raise ValueError("geomat error. Stress path curtailed.")
+            ps.append(model.p_prime)
+            qs.append(model.q)
+            self._stresses[i + 1] = model.sigma_prime_tilde
+        self._works[1:] = (
+            np.sum(self._stresses[1:] * strain_incs, axis=-1) * self._volumes[1:]
+        )
+        self._ps = np.asarray(ps)
+        self._qs = np.asarray(qs)
 
         return True
 
+    def _strain_def(self):
+        self._strains[:, 0] = self._warps[:, 2]
+        self._strains[:, 1] = self._warps[:, 5]
+        self._strains[:, 5] = self._warps[:, 3] + self._warps[:, 4]
+
 
 class ParticleResults(ParticleBase):
     """
     ParticleResults class for geopyv.
 
     Parameters
     ----------
```

### Comparing `geopyv-0.0.6/src/geopyv/plots.py` & `geopyv-0.0.8/src/geopyv/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1157,14 +1157,15 @@
     # General formatting.
     # Legend.
     plt.legend(bbox_to_anchor=(0.05, 0.95), loc="upper left", borderaxespad=0)
 
     # Logscale.
     ax.set_xscale(scale)
     ax.set_yscale("log")
+    ax.grid(which="both")
 
     # Limit control.
     if xlim is not None:
         ax.set_xlim(xlim)
     if ylim is not None:
         ax.set_ylim(ylim)
 
@@ -1274,14 +1275,15 @@
     # General formatting.
     # Legend.
     plt.legend(bbox_to_anchor=(0.05, 0.95), loc="upper left", borderaxespad=0)
 
     # Logscale.
     ax.set_xscale(scale)
     ax.set_yscale("log")
+    ax.grid(which="both")
 
     # Limit control.
     if xlim is not None:
         ax.set_xlim(xlim)
     if ylim is not None:
         ax.set_ylim(ylim)
```

### Comparing `geopyv-0.0.6/src/geopyv/sequence.py` & `geopyv-0.0.8/src/geopyv/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -859,14 +859,15 @@
         seed_tolerance=0.9,
         alpha=0.5,
         track=False,
         hard_boundary=True,
         rigid=False,
         subset_size_compensation=False,
         guide=False,
+        sequential=False,
     ):
         """
         Method to solve for the sequence.
 
         Parameters
         ----------
         seed_coord : numpy.ndarray (2,)
@@ -1089,14 +1090,16 @@
         self._mesh_order = mesh_order
         self._tolerance = tolerance
         self._seed_tolerance = seed_tolerance
         self._alpha = alpha
         self._track = track
         self._hard_boundary = hard_boundary
         self._rigid = rigid
+        self._guide = guide
+        self._sequential = sequential
         self._subset_size_compensation = subset_size_compensation
         self._seed_warp = np.zeros(6 * self._subset_order)
 
         # Solve.
         _f_index = 0
         _g_index = 1
         _f_img = gp.image.Image(self._image_dir + self._images[_f_index])
@@ -1148,18 +1151,18 @@
                         "mesh_"
                         + str(self._image_indices[_f_index])
                         + "_"
                         + str(self._image_indices[_g_index])
                     )
                 else:
                     self.data["meshes"][_g_index - 1] = mesh.data
-                if track:
+                if self._track:
                     self._boundary_tags = mesh._boundary_tags
                     self._exclusions_tags = mesh._exclusions_tags
-                if guide:
+                if self._guide:
                     seed = gp.particle.Particle(
                         series=mesh, coordinate_0=self._seed_coord
                     )
                     seed.solve()
                     self._seed_warp[
                         : 6 * min(self._mesh_order, self._subset_order)
                     ] = seed.data["results"]["warps"][
@@ -1167,14 +1170,18 @@
                     ]
                 _g_index += 1  # Iterate the target image index.
                 del _g_img
                 if _g_index != len(self._image_indices):
                     _g_img = gp.image.Image(self._image_dir + self._images[_g_index])
                 else:
                     self.solved = True
+                if self._sequential:
+                    _f_index = _g_index - 1
+                    del _f_img
+                    _f_img = gp.image.Image(self._image_dir + self._images[_f_index])
             elif _f_index + 1 < _g_index:
                 _f_index = _g_index - 1
                 if self._track:
                     self._tracking(_f_index)
                 del _f_img
                 _f_img = gp.image.Image(self._image_dir + self._images[_f_index])
             else:
@@ -1228,14 +1235,22 @@
                 )
                 subset = gp.subset.Subset(
                     f_img=f_img,
                     g_img=g_img,
                     f_coord=centre,
                     template=gp.templates.Circle(50),
                 )
+                subset.solve(
+                    subset.solve(warp_0=self._exclusions[i][0].data["results"]["p"])
+                )
+                if subset.data["solved"] is not True:
+                    subset.solve()
+                    if subset.data["solved"] is not True:
+                        log.error("Could not track rigid exclusion.")
+                        raise ValueError("Could not track rigid exclusion.")
                 subset.solve()
                 warp = subset.data["results"]["p"].flatten()
                 theta = (warp[3] - warp[4]) / 2
                 rot = np.asarray(
                     [[np.cos(theta), np.sin(theta)], [-np.sin(theta), np.cos(theta)]]
                 )
                 centre += warp[:2]
@@ -1286,7 +1301,31 @@
         geopyv data dict from Sequence object.
 
     """
 
     def __init__(self, data):
         """Initialisation of geopyv SequenceResults class."""
         self.data = data
+
+    def load(self):
+        """Load all meshes in sequence object mesh directory."""
+        try:
+            _meshes = glob.glob(
+                "*.pyv", root_dir=self.data["file_settings"]["mesh_dir"]
+            )
+            _mesh_tars = [int(re.findall(r"\d+", x)[-1]) for x in _meshes]
+            _mesh_indices_arguments = np.argsort(_mesh_tars)
+            self._meshes = np.asarray(
+                [_meshes[index] for index in _mesh_indices_arguments], dtype=object
+            )
+        except Exception:
+            log.error(
+                "Issues encountered recognising mesh file names. "
+                "Please refer to the documentation for naming guidance."
+            )
+        self._images = self.data["file_settings"]["images"][
+            : np.shape(self._meshes)[0] + 1
+        ]
+        self.data["solved"] = True
+        self.data["unsolvable"] = False
+        self.data["meshes"] = self._meshes
+        self.data["file_settings"]["images"]
```

### Comparing `geopyv-0.0.6/src/geopyv/speckle.py` & `geopyv-0.0.8/src/geopyv/speckle.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,19 +170,24 @@
             "noise": self._noise,
             "tmi": self._tmi,
             "speckle_size": self._speckle_size,
         }
 
     def solve(
         self,
+        *,
+        wrap=False,
     ):
+        self._wrap = wrap
         [self.X, self.Y] = np.meshgrid(range(self._image_size), range(self._image_size))
         self._ref_speckle = self._speckle_distribution()
         self._mult()
-        self.data.update({"ref_speckle": self._ref_speckle, "pm": self._pm})
+        self.data.update(
+            {"wrap": self._wrap, "ref_speckle": self._ref_speckle, "pm": self._pm}
+        )
         self._image_generation()
         self.solved = True
         self.data["solved"] = True
 
     def _speckle_distribution(self):
         raw_grid = np.zeros((self._image_size, self._image_size))
         speckles = []
@@ -228,14 +233,16 @@
         with alive_bar(
             self._image_no, dual_line=True, bar="blocks", title="Generating images..."
         ) as bar:
             for i in range(self._image_no):
                 _tar_speckle = (
                     self._warp(i, self._ref_speckle)[:, :2] + self._ref_speckle
                 )
+                if self._wrap:
+                    _tar_speckle %= self._image_size
                 _grid = self._grid(i, _tar_speckle)
                 self._create(i, _grid)
                 bar()
 
     def _grid(self, i, _tar_speckle):
         grid = np.zeros((self._image_size, self._image_size))
         if self.noisem[i, 0] != 0.0:
```

### Comparing `geopyv-0.0.6/src/geopyv/subset.py` & `geopyv-0.0.8/src/geopyv/subset.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,26 +268,29 @@
             gp.check._check_type(f_img, "f_img", [gp.image.Image]), "Warning"
         ):
             f_img = gp.io._load_f_img()
         if self._report(
             gp.check._check_type(g_img, "g_img", [gp.image.Image]), "Warning"
         ):
             g_img = gp.io._load_g_img()
+        if template is None:
+            template = gp.templates.Circle(50)
+        types = [gp.templates.Circle, gp.templates.Square]
+        self._report(gp.check._check_type(template, "template", types), "TypeError")
         if self._report(
             gp.check._check_type(f_coord, "f_coord", [np.ndarray]), "Warning"
         ):
-            f_coord = gp.gui.selectors.coordinate.CoordinateSelector()
+            selector = gp.gui.selectors.coordinate.CoordinateSelector()
+            f_coord = selector.select(f_img, template)
         elif self._report(gp.check._check_dim(f_coord, "f_coord", 1), "Warning"):
-            f_coord = gp.gui.selectors.coordinate.CoordinateSelector()
+            selector = gp.gui.selectors.coordinate.CoordinateSelector()
+            f_coord = selector.select(f_img, template)
         elif self._report(gp.check._check_axis(f_coord, "f_coord", 0, [2]), "Warning"):
-            f_coord = gp.gui.selectors.coordinate.CoordinateSelector()
-        if template is None:
-            template = gp.templates.Circle(50)
-        types = [gp.templates.Circle, gp.templates.Square]
-        self._report(gp.check._check_type(template, "template", types), "TypeError")
+            selector = gp.gui.selectors.coordinate.CoordinateSelector()
+            f_coord = selector.select(f_img, template)
 
         # Store.
         self._initialised = False
         self._f_coord = f_coord
         self._f_img = f_img
         self._g_img = g_img
         self._template = template
@@ -414,16 +417,17 @@
 
 
         .. seealso::
             :meth:`~_get_initial_guess_size`
             :meth:`~_get_initial_guess`
 
         """
-        # Check other control parameters.
         log.debug("Solving geopyv Subset object.")
+
+        # Check input.
         check = gp.check._check_type(max_norm, "max_norm", [float])
         if check:
             try:
                 max_norm = float(max_norm)
                 self._report(
                     gp.check._conversion(max_norm, "max_norm", float), "Warning"
                 )
```

### Comparing `geopyv-0.0.6/src/geopyv/templates.py` & `geopyv-0.0.8/src/geopyv/templates.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv/validation.py` & `geopyv-0.0.8/src/geopyv/validation.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.6/src/geopyv.egg-info/PKG-INFO` & `geopyv-0.0.8/src/geopyv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopyv
-Version: 0.0.6
+Version: 0.0.8
 Summary: A PIV/DIC analysis package for Python.
 Author-email: Sam Stanier <sas229@cam.ac.uk>, Jonathan Smith <jdks2@cam.ac.uk>
 Project-URL: Homepage, https://github.com/sas229/geopyv
 Project-URL: Bug Tracker, https://github.com/sas229/geopyv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `geopyv-0.0.6/src/geopyv.egg-info/SOURCES.txt` & `geopyv-0.0.8/src/geopyv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

