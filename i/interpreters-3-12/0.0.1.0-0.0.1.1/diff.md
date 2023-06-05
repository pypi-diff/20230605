# Comparing `tmp/interpreters_3_12-0.0.1.0.tar.gz` & `tmp/interpreters_3_12-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpreters_3_12-0.0.1.0.tar", last modified: Mon Jun  5 17:29:18 2023, max compression
+gzip compressed data, was "interpreters_3_12-0.0.1.1.tar", last modified: Mon Jun  5 17:40:31 2023, max compression
```

## Comparing `interpreters_3_12-0.0.1.0.tar` & `interpreters_3_12-0.0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2023-06-05 17:29:18.888988 interpreters_3_12-0.0.1.0/
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     1298 2023-04-19 20:43:12.000000 interpreters_3_12-0.0.1.0/LICENSE
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     1516 2023-06-05 17:29:18.888988 interpreters_3_12-0.0.1.0/PKG-INFO
--rw-rw-r--   0 esnow     (1000) esnow     (1000)      869 2023-06-02 21:33:23.000000 interpreters_3_12-0.0.1.0/README.md
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     1389 2023-06-05 17:27:59.000000 interpreters_3_12-0.0.1.0/pyproject.toml
--rw-rw-r--   0 esnow     (1000) esnow     (1000)       38 2023-06-05 17:29:18.888988 interpreters_3_12-0.0.1.0/setup.cfg
--rw-rw-r--   0 esnow     (1000) esnow     (1000)      285 2023-06-05 17:10:41.000000 interpreters_3_12-0.0.1.0/setup.py
-drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2023-06-05 17:29:18.888988 interpreters_3_12-0.0.1.0/src/
--rw-rw-r--   0 esnow     (1000) esnow     (1000)    62391 2023-06-05 17:10:41.000000 interpreters_3_12-0.0.1.0/src/_channels.c
--rw-rw-r--   0 esnow     (1000) esnow     (1000)    21822 2023-06-05 17:09:35.000000 interpreters_3_12-0.0.1.0/src/_interpreters.c
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     5792 2023-06-05 17:10:41.000000 interpreters_3_12-0.0.1.0/src/interpreters.py
-drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2023-06-05 17:29:18.888988 interpreters_3_12-0.0.1.0/src/interpreters_3_12.egg-info/
--rw-rw-r--   0 esnow     (1000) esnow     (1000)     1516 2023-06-05 17:29:18.000000 interpreters_3_12-0.0.1.0/src/interpreters_3_12.egg-info/PKG-INFO
--rw-rw-r--   0 esnow     (1000) esnow     (1000)      277 2023-06-05 17:29:18.000000 interpreters_3_12-0.0.1.0/src/interpreters_3_12.egg-info/SOURCES.txt
--rw-rw-r--   0 esnow     (1000) esnow     (1000)        1 2023-06-05 17:29:18.000000 interpreters_3_12-0.0.1.0/src/interpreters_3_12.egg-info/dependency_links.txt
--rw-rw-r--   0 esnow     (1000) esnow     (1000)       37 2023-06-05 17:29:18.000000 interpreters_3_12-0.0.1.0/src/interpreters_3_12.egg-info/top_level.txt
+drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2023-06-05 17:40:31.194535 interpreters_3_12-0.0.1.1/
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)     1298 2023-04-19 20:43:12.000000 interpreters_3_12-0.0.1.1/LICENSE
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)     1516 2023-06-05 17:40:31.194535 interpreters_3_12-0.0.1.1/PKG-INFO
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)      869 2023-06-02 21:33:23.000000 interpreters_3_12-0.0.1.1/README.md
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)     1389 2023-06-05 17:39:44.000000 interpreters_3_12-0.0.1.1/pyproject.toml
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)       38 2023-06-05 17:40:31.194535 interpreters_3_12-0.0.1.1/setup.cfg
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)      285 2023-06-05 17:10:41.000000 interpreters_3_12-0.0.1.1/setup.py
+drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2023-06-05 17:40:31.194535 interpreters_3_12-0.0.1.1/src/
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)    62475 2023-06-05 17:37:57.000000 interpreters_3_12-0.0.1.1/src/_channels.c
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)    21910 2023-06-05 17:37:31.000000 interpreters_3_12-0.0.1.1/src/_interpreters.c
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)     5792 2023-06-05 17:10:41.000000 interpreters_3_12-0.0.1.1/src/interpreters.py
+drwxrwxr-x   0 esnow     (1000) esnow     (1000)        0 2023-06-05 17:40:31.194535 interpreters_3_12-0.0.1.1/src/interpreters_3_12.egg-info/
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)     1516 2023-06-05 17:40:31.000000 interpreters_3_12-0.0.1.1/src/interpreters_3_12.egg-info/PKG-INFO
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)      277 2023-06-05 17:40:31.000000 interpreters_3_12-0.0.1.1/src/interpreters_3_12.egg-info/SOURCES.txt
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)        1 2023-06-05 17:40:31.000000 interpreters_3_12-0.0.1.1/src/interpreters_3_12.egg-info/dependency_links.txt
+-rw-rw-r--   0 esnow     (1000) esnow     (1000)       37 2023-06-05 17:40:31.000000 interpreters_3_12-0.0.1.1/src/interpreters_3_12.egg-info/top_level.txt
```

### Comparing `interpreters_3_12-0.0.1.0/LICENSE` & `interpreters_3_12-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `interpreters_3_12-0.0.1.0/PKG-INFO` & `interpreters_3_12-0.0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpreters_3_12
-Version: 0.0.1.0
+Version: 0.0.1.1
 Summary: Use this module to try out multiple interpreters and a per-interpreter GIL in Python 3.12.  Do not use this for anything important.
 Author-email: Eric Snow <ericsnowcurrently@gmail.com>
 Project-URL: Homepage, https://github.com/ericsnowcurrently/interpreters
 Project-URL: Bug Tracker, https://github.com/ericsnowcurrently/interpreters/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `interpreters_3_12-0.0.1.0/README.md` & `interpreters_3_12-0.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `interpreters_3_12-0.0.1.0/pyproject.toml` & `interpreters_3_12-0.0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # We use setuptools because hatchling doesn't build extension modules.
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "interpreters_3_12"
-version = "0.0.1.0"
+version = "0.0.1.1"
 authors = [
   { name="Eric Snow", email="ericsnowcurrently@gmail.com" },
 ]
 description = "Use this module to try out multiple interpreters and a per-interpreter GIL in Python 3.12.  Do not use this for anything important."
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `interpreters_3_12-0.0.1.0/src/_channels.c` & `interpreters_3_12-0.0.1.1/src/_channels.c`

 * *Files 0% similar despite different names*

```diff
@@ -2458,7 +2458,13 @@
 };
 
 PyMODINIT_FUNC
 PyInit__xxinterpchannels(void)
 {
     return PyModuleDef_Init(&moduledef);
 }
+
+PyMODINIT_FUNC
+PyInit__channels(void)
+{
+    return PyModuleDef_Init(&moduledef);
+}
```

### Comparing `interpreters_3_12-0.0.1.0/src/_interpreters.c` & `interpreters_3_12-0.0.1.1/src/_interpreters.c`

 * *Files 1% similar despite different names*

```diff
@@ -859,7 +859,13 @@
 };
 
 PyMODINIT_FUNC
 PyInit__xxsubinterpreters(void)
 {
     return PyModuleDef_Init(&moduledef);
 }
+
+PyMODINIT_FUNC
+PyInit__interpreters(void)
+{
+    return PyModuleDef_Init(&moduledef);
+}
```

### Comparing `interpreters_3_12-0.0.1.0/src/interpreters.py` & `interpreters_3_12-0.0.1.1/src/interpreters.py`

 * *Files identical despite different names*

### Comparing `interpreters_3_12-0.0.1.0/src/interpreters_3_12.egg-info/PKG-INFO` & `interpreters_3_12-0.0.1.1/src/interpreters_3_12.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpreters-3-12
-Version: 0.0.1.0
+Version: 0.0.1.1
 Summary: Use this module to try out multiple interpreters and a per-interpreter GIL in Python 3.12.  Do not use this for anything important.
 Author-email: Eric Snow <ericsnowcurrently@gmail.com>
 Project-URL: Homepage, https://github.com/ericsnowcurrently/interpreters
 Project-URL: Bug Tracker, https://github.com/ericsnowcurrently/interpreters/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

