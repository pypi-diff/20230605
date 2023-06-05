# Comparing `tmp/generallibrary-2.9.8.tar.gz` & `tmp/generallibrary-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generallibrary-2.9.8.tar", last modified: Thu Sep  8 19:28:01 2022, max compression
+gzip compressed data, was "generallibrary-2.9.9.tar", last modified: Fri Sep  9 10:43:54 2022, max compression
```

## Comparing `generallibrary-2.9.8.tar` & `generallibrary-2.9.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:28:01.644840 generallibrary-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-08 19:27:29.000000 generallibrary-2.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-08 19:27:36.000000 generallibrary-2.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    44018 2022-09-08 19:28:01.644840 generallibrary-2.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    40983 2022-09-08 19:28:00.000000 generallibrary-2.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:28:01.644840 generallibrary-2.9.8/generallibrary/
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/analyze.py
--rw-r--r--   0 runner    (1001) docker     (121)     8386 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/code.py
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/context.py
--rw-r--r--   0 runner    (1001) docker     (121)    18138 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)    39904 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/diagram.py
--rw-r--r--   0 runner    (1001) docker     (121)    11368 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10553 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/iterables.py
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/object.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:28:01.644840 generallibrary-2.9.8/generallibrary/objinfo/
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/objinfo/children.py
--rw-r--r--   0 runner    (1001) docker     (121)     8509 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/objinfo/objinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/objinfo/origin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/objinfo/parents.py
--rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/objinfo/properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/objinfo/type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:28:01.644840 generallibrary-2.9.8/generallibrary/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/calltable_objinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/calltable_origin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/positional.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_code.py
--rw-r--r--   0 runner    (1001) docker     (121)     5033 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)    14037 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_diagram.py
--rw-r--r--   0 runner    (1001) docker     (121)    21436 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_generallibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)    12966 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_iterables.py
--rw-r--r--   0 runner    (1001) docker     (121)    15490 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (121)     2708 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     8316 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     5809 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/test/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/text.py
--rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     7696 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     5900 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/values.py
--rw-r--r--   0 runner    (1001) docker     (121)     7036 2022-09-08 19:25:41.000000 generallibrary-2.9.8/generallibrary/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:28:01.644840 generallibrary-2.9.8/generallibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    44018 2022-09-08 19:28:01.000000 generallibrary-2.9.8/generallibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-09-08 19:28:01.000000 generallibrary-2.9.8/generallibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 19:28:01.000000 generallibrary-2.9.8/generallibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-08 19:28:01.000000 generallibrary-2.9.8/generallibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-08 19:28:01.000000 generallibrary-2.9.8/generallibrary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-09-08 19:26:11.000000 generallibrary-2.9.8/metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 19:28:01.644840 generallibrary-2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-09-08 19:27:36.000000 generallibrary-2.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 10:43:54.701752 generallibrary-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-09 10:43:21.000000 generallibrary-2.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-09 10:43:30.000000 generallibrary-2.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    44188 2022-09-09 10:43:54.701752 generallibrary-2.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    41145 2022-09-09 10:43:53.000000 generallibrary-2.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 10:43:54.697752 generallibrary-2.9.9/generallibrary/
+-rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8386 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/code.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18138 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39904 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11279 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10553 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/iterables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/object.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 10:43:54.697752 generallibrary-2.9.9/generallibrary/objinfo/
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/objinfo/children.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8509 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/objinfo/objinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/objinfo/origin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/objinfo/parents.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/objinfo/properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/objinfo/type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 10:43:54.697752 generallibrary-2.9.9/generallibrary/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/calltable_objinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/calltable_origin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/positional.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5033 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14037 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21436 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_generallibrary.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12988 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_iterables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15512 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2730 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8338 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/test/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7696 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5900 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/values.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7036 2022-09-09 10:41:22.000000 generallibrary-2.9.9/generallibrary/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 10:43:54.697752 generallibrary-2.9.9/generallibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    44188 2022-09-09 10:43:54.000000 generallibrary-2.9.9/generallibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-09-09 10:43:54.000000 generallibrary-2.9.9/generallibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 10:43:54.000000 generallibrary-2.9.9/generallibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-09 10:43:54.000000 generallibrary-2.9.9/generallibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-09 10:43:54.000000 generallibrary-2.9.9/generallibrary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-09-09 10:41:55.000000 generallibrary-2.9.9/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-09 10:43:54.701752 generallibrary-2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-09-09 10:43:30.000000 generallibrary-2.9.9/setup.py
```

### Comparing `generallibrary-2.9.8/LICENSE` & `generallibrary-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/PKG-INFO` & `generallibrary-2.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generallibrary
-Version: 2.9.8
+Version: 2.9.9
 Summary: Random useful code categorized into modules.
 Home-page: https://github.com/ManderaGeneral/generallibrary
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Description: # generallibrary
         Random useful code categorized into modules.
@@ -17,286 +17,287 @@
         ├─ <a href='#Attributes'>Attributes</a>
         ├─ <a href='#Contributions'>Contributions</a>
         └─ <a href='#Todo'>Todo</a>
         </pre>
         
         
         ## Installation
-        | Command                             | <a href='https://pypi.org/project/generalimport'>generalimport</a>   | <a href='https://pypi.org/project/packaging'>packaging</a>   | <a href='https://pypi.org/project/pyperclip'>pyperclip</a>   | <a href='https://pypi.org/project/tabulate'>tabulate</a>   | <a href='https://pypi.org/project/pytz'>pytz</a>   | <a href='https://pypi.org/project/dill'>dill</a>   | <a href='https://pypi.org/project/matplotlib'>matplotlib</a>   | <a href='https://pypi.org/project/networkx'>networkx</a>   | <a href='https://pypi.org/project/pandas'>pandas</a>   |
-        |:------------------------------------|:---------------------------------------------------------------------|:-------------------------------------------------------------|:-------------------------------------------------------------|:-----------------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------------------|:-----------------------------------------------------------|:-------------------------------------------------------|
-        | `pip install generallibrary`        | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                        | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | No                                                     |
-        | `pip install generallibrary[table]` | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                        | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    |
-        | `pip install generallibrary[full]`  | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                        | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    |
+        | Command                             | <a href='https://pypi.org/project/generalimport'>generalimport</a>   | <a href='https://pypi.org/project/packaging'>packaging</a>   | <a href='https://pypi.org/project/pyperclip'>pyperclip</a>   | <a href='https://pypi.org/project/pytz'>pytz</a>   | <a href='https://pypi.org/project/dill'>dill</a>   | <a href='https://pypi.org/project/matplotlib'>matplotlib</a>   | <a href='https://pypi.org/project/networkx'>networkx</a>   | <a href='https://pypi.org/project/pandas'>pandas</a>   | <a href='https://pypi.org/project/tabulate'>tabulate</a>   |
+        |:------------------------------------|:---------------------------------------------------------------------|:-------------------------------------------------------------|:-------------------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------------------|:-----------------------------------------------------------|:-------------------------------------------------------|:-----------------------------------------------------------|
+        | `pip install generallibrary`        | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | No                                                     | No                                                         |
+        | `pip install generallibrary[table]` | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    | Yes                                                        |
+        | `pip install generallibrary[full]`  | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    | Yes                                                        |
         
         ## Information
         | Package                                                            | Ver                                               | Latest Release        | Python                                                                                                                                                                                  | Platform        |   Lvl | Todo                                                       | Cover   |
         |:-------------------------------------------------------------------|:--------------------------------------------------|:----------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:-----------------------------------------------------------|:--------|
-        | [generallibrary](https://github.com/ManderaGeneral/generallibrary) | [2.9.8](https://pypi.org/project/generallibrary/) | 2022-09-08 21:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/) | Windows, Ubuntu |     1 | [6](https://github.com/ManderaGeneral/generallibrary#Todo) | 94.0 %  |
+        | [generallibrary](https://github.com/ManderaGeneral/generallibrary) | [2.9.9](https://pypi.org/project/generallibrary/) | 2022-09-09 12:43 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/) | Windows, Ubuntu |     1 | [6](https://github.com/ManderaGeneral/generallibrary#Todo) | 93.9 %  |
         
         ## Attributes
         <pre>
-        <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/__init__.py#L1'>Module: generallibrary</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L204'>Class: AutoInitBases</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L10'>Class: BoolStr</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L93'>Class: CallTable</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L138'>Method: generate</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L142'>Method: generate_with_args</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L146'>Method: generate_with_funcs</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L106'>Method: set_args</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L101'>Method: set_funcs</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L139'>Class: CodeLine</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L157'>Method: get_lines</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L172'>Method: text</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L230'>Class: DataClass</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L223'>Method: field_dict</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L217'>Method: field_values</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L61'>Class: Date</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L83'>Method: get_timezone_obj</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L87'>Method: now</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L6'>Class: DecoContext</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L17'>Method: after</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L14'>Method: before</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L84'>Class: EmptyContext</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L158'>Class: EnvVar</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L174'>Property: value</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L187'>Class: HierarchyStorer</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L28'>Class: Log</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L245'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L76'>Method: configure_file</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L80'>Method: configure_stream</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L61'>Method: critical</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L57'>Method: debug</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L60'>Method: error</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L58'>Method: info</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L88'>Method: is_root</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L84'>Method: loggers</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L309'>Method: recycle_clear</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L314'>Method: recycle_clear_all</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L59'>Method: warning</a> <b>(Untested)</b>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L542'>Class: Markdown</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L613'>Method: add_code_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L579'>Method: add_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L608'>Method: add_list_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L619'>Method: add_pre_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L599'>Method: add_table_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L588'>Method: get_all_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L572'>Method: get_section_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L555'>Method: link</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L624'>Method: wrap_with_tags</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L503'>Class: NetworkDiagram</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L526'>Method: get_spouse</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L511'>Method: get_spouses</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L161'>Method: add_node</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/parents.py#L59'>Method: check_if_parent_eligible</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L141'>Method: defined_by_parent</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L241'>Method: disconnect</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L116'>Method: doc</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L52'>Method: file</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L28'>Method: from_base</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L21'>Method: from_builtin</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L36'>Method: from_class</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L51'>Method: from_instance</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L58'>Method: from_module</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L252'>Method: get_all</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L181'>Method: get_child</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L350'>Method: get_children</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L91'>Method: get_definition_line</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L132'>Method: get_index</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L103'>Method: get_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L207'>Method: get_node</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L388'>Method: get_nodes</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L269'>Method: get_ordered</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L233'>Method: get_ordered_index</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L85'>Method: get_origin</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L194'>Method: get_parent</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L369'>Method: get_parents</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L220'>Method: get_sibling</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L405'>Method: get_siblings</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L91'>Method: graph</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L62'>Method: identifier</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L17'>Method: internal</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L34'>Method: is_class</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L28'>Method: is_function</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L50'>Method: is_instance</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L59'>Method: is_method</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L22'>Method: is_module</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L44'>Method: is_property</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L43'>Method: module</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L75'>Method: print_link_to_obj</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L26'>Method: private</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L34'>Method: protected</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L9'>Method: public</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L170'>Method: remove_node</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L145'>Method: set_index</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L316'>Method: set_parent</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/parents.py#L7'>Method: spawn_parents</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L8'>Method: type</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L455'>Method: view</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L385'>Class: Operators</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L396'>Method: deco_define_comparisons</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L225'>Class: PythonVersion</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L231'>Property: version</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L212'>Class: Recycle</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L245'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L309'>Method: recycle_clear</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L314'>Method: recycle_clear_all</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L40'>Class: RedirectStdout</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L22'>Class: SigInfo</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L265'>Method: call</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L48'>Property: callableObject</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L52'>Method: class_from_callable</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L178'>Property: defaults</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L220'>Method: getIndexFromName</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L146'>Property: leadingArgNames</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L126'>Property: names</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L136'>Property: namesRequired</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L131'>Property: namesWithoutDefaults</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L141'>Property: namesWithoutPacked</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L227'>Property: packedArgs</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L164'>Property: packedArgsName</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L232'>Property: packedKwargs</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L171'>Property: packedKwargsName</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L85'>Property: parameters</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L204'>Property: positionalArgNames</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L188'>Property: positionalOnlyArgNames</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L197'>Property: positionalOnlyOppositeArgNames</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L212'>Property: positionalOppositeArgNames</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L75'>Property: positional_extra</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L237'>Property: unpackedArgs</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L248'>Property: unpackedKwargs</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L5'>Class: SortedList</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L32'>Method: add</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L49'>Method: remove</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L292'>Class: Storable</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L302'>Method: copy_node</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L297'>Method: load_node</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L294'>Method: save_node</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L11'>Class: Timer</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L41'>Method: deco</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L32'>Method: print</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L19'>Method: reset</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L26'>Method: seconds</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L432'>Class: TreeDiagram</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L455'>Method: view</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L15'>Class: Ver</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L29'>Method: bump</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L213'>Class: VerInfo</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L177'>Property: caseSensitive</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L191'>Property: pathDelimiter</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L205'>Property: pathRootHasColon</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L198'>Property: pathRootIsDelimiter</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L184'>Property: positionalArgument</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L139'>Property: pythonAlpha</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L144'>Property: pythonBeta</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L149'>Property: pythonCandidate</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L154'>Property: pythonFinal</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L108'>Property: pythonMajor</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L118'>Property: pythonMicro</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L113'>Property: pythonMinor</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L159'>Property: pythonReleaseKeyword</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L123'>Property: pythonReleaseLevel</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L129'>Property: pythonSerial</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L134'>Property: pythonSerialString</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L164'>Property: pythonString</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L169'>Property: pythonVersion</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L202'>Function: auto_deco</a> <b>(Untested)</b>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L121'>Function: cache_clear</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L40'>Function: calculate</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L135'>Function: call_base_hooks</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L38'>Function: ceil</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L47'>Function: clamp</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L17'>Class: classproperty</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L121'>Function: clipboard_copy</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L134'>Function: clipboard_get</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L291'>Function: combine</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L16'>Function: comma_and_and</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L20'>Function: comma_and_or</a> <b>(Untested)</b>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L129'>Function: confineTo</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L178'>Function: debug</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L337'>Function: deco_bound_defaults</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L15'>Function: deco_cache</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L303'>Function: deco_cast_parameters</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L357'>Function: deco_extend</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L280'>Function: deco_optional_suppress</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L368'>Function: deco_propagate_while</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L418'>Function: deco_require</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L63'>Function: defaults</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L91'>Function: depth</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L334'>Function: dict_insert</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L154'>Function: dir_appearance_order</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L104'>Function: doubleRectify</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/serialize.py#L24'>Function: dumps</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L261'>Function: exclusive</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L122'>Function: extend_list_in_dict</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L319'>Function: flatten</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L34'>Function: floor</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L167'>Function: get</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L164'>Function: getBaseClassNames</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L132'>Function: getBaseClasses</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L126'>Function: get_attrs_from_bases</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L255'>Function: get_definition_line</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L146'>Function: get_free_index</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L182'>Function: get_index</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L78'>Function: get_items</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L197'>Function: get_launch_options</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L210'>Function: get_origin</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L228'>Function: get_rows</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L70'>Function: get_values</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/object.py#L8'>Function: getsize</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L176'>Function: hasMethod</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L88'>Function: hook</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L266'>Function: inclusive</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L151'>Function: initBases</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L78'>Function: inrange</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/object.py#L34'>Function: interconnect</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L86'>Function: is_iterable</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L106'>Function: iter_first_value</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L117'>Function: join_with_str</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/serialize.py#L30'>Function: loads</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L46'>Function: match</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L314'>Function: pivot_list</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L25'>Function: plur_sing</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L231'>Function: print_link</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L246'>Function: print_link_to_obj</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L92'>Function: rectify</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L194'>Function: remove</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L282'>Function: remove_duplicates</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L36'>Function: replace</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L42'>Function: round_</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L61'>Function: sign</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L53'>Function: sleep</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L304'>Function: split_list</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L5'>Function: strToDynamicType</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L326'>Function: subtract_list</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L319'>Function: terminal</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L104'>Function: typeChecker</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L271'>Function: unique_obj_in_list</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L134'>Function: update_dict_in_dict</a>
-        └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L6'>Function: wrapper_transfer</a>
+        <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/__init__.py#L1'>Module: generallibrary</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L202'>Class: AutoInitBases</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L10'>Class: BoolStr</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L91'>Class: CallTable</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L136'>Method: generate</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L140'>Method: generate_with_args</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L144'>Method: generate_with_funcs</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L104'>Method: set_args</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L99'>Method: set_funcs</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L139'>Class: CodeLine</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L157'>Method: get_lines</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L172'>Method: text</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L230'>Class: DataClass</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L223'>Method: field_dict</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L217'>Method: field_values</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L61'>Class: Date</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L83'>Method: get_timezone_obj</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L87'>Method: now</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L6'>Class: DecoContext</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L17'>Method: after</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L14'>Method: before</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L82'>Class: EmptyContext</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L158'>Class: EnvVar</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L174'>Property: value</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L187'>Class: HierarchyStorer</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L28'>Class: Log</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L243'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L76'>Method: configure_file</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L80'>Method: configure_stream</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L61'>Method: critical</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L57'>Method: debug</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L60'>Method: error</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L58'>Method: info</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L88'>Method: is_root</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L84'>Method: loggers</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L307'>Method: recycle_clear</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L312'>Method: recycle_clear_all</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L59'>Method: warning</a> <b>(Untested)</b>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L542'>Class: Markdown</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L613'>Method: add_code_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L579'>Method: add_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L608'>Method: add_list_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L619'>Method: add_pre_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L599'>Method: add_table_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L588'>Method: get_all_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L572'>Method: get_section_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L555'>Method: link</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L624'>Method: wrap_with_tags</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L503'>Class: NetworkDiagram</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L526'>Method: get_spouse</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L511'>Method: get_spouses</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L161'>Method: add_node</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/parents.py#L59'>Method: check_if_parent_eligible</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L141'>Method: defined_by_parent</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L241'>Method: disconnect</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L116'>Method: doc</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L52'>Method: file</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L28'>Method: from_base</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L21'>Method: from_builtin</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L36'>Method: from_class</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L51'>Method: from_instance</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L58'>Method: from_module</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L252'>Method: get_all</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L181'>Method: get_child</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L350'>Method: get_children</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L91'>Method: get_definition_line</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L132'>Method: get_index</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L103'>Method: get_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L207'>Method: get_node</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L388'>Method: get_nodes</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L269'>Method: get_ordered</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L233'>Method: get_ordered_index</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L85'>Method: get_origin</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L194'>Method: get_parent</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L369'>Method: get_parents</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L220'>Method: get_sibling</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L405'>Method: get_siblings</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L91'>Method: graph</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L62'>Method: identifier</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L17'>Method: internal</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L34'>Method: is_class</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L28'>Method: is_function</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L50'>Method: is_instance</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L59'>Method: is_method</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L22'>Method: is_module</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L44'>Method: is_property</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L43'>Method: module</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L75'>Method: print_link_to_obj</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L26'>Method: private</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L34'>Method: protected</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L9'>Method: public</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L170'>Method: remove_node</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L145'>Method: set_index</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L316'>Method: set_parent</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/parents.py#L7'>Method: spawn_parents</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L8'>Method: type</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L455'>Method: view</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L385'>Class: Operators</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L396'>Method: deco_define_comparisons</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L225'>Class: PythonVersion</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L231'>Property: version</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L210'>Class: Recycle</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L243'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L307'>Method: recycle_clear</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L312'>Method: recycle_clear_all</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L40'>Class: RedirectStdout</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L22'>Class: SigInfo</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L265'>Method: call</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L48'>Property: callableObject</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L52'>Method: class_from_callable</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L178'>Property: defaults</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L220'>Method: getIndexFromName</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L146'>Property: leadingArgNames</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L126'>Property: names</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L136'>Property: namesRequired</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L131'>Property: namesWithoutDefaults</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L141'>Property: namesWithoutPacked</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L227'>Property: packedArgs</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L164'>Property: packedArgsName</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L232'>Property: packedKwargs</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L171'>Property: packedKwargsName</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L85'>Property: parameters</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L204'>Property: positionalArgNames</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L188'>Property: positionalOnlyArgNames</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L197'>Property: positionalOnlyOppositeArgNames</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L212'>Property: positionalOppositeArgNames</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L75'>Property: positional_extra</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L237'>Property: unpackedArgs</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L248'>Property: unpackedKwargs</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L5'>Class: SortedList</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L32'>Method: add</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L49'>Method: remove</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L292'>Class: Storable</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L302'>Method: copy_node</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L297'>Method: load_node</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L294'>Method: save_node</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L11'>Class: Timer</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L41'>Method: deco</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L32'>Method: print</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L19'>Method: reset</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L26'>Method: seconds</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L432'>Class: TreeDiagram</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L455'>Method: view</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L15'>Class: Ver</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L29'>Method: bump</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L213'>Class: VerInfo</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L177'>Property: caseSensitive</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L191'>Property: pathDelimiter</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L205'>Property: pathRootHasColon</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L198'>Property: pathRootIsDelimiter</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L184'>Property: positionalArgument</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L139'>Property: pythonAlpha</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L144'>Property: pythonBeta</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L149'>Property: pythonCandidate</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L154'>Property: pythonFinal</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L108'>Property: pythonMajor</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L118'>Property: pythonMicro</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L113'>Property: pythonMinor</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L159'>Property: pythonReleaseKeyword</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L123'>Property: pythonReleaseLevel</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L129'>Property: pythonSerial</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L134'>Property: pythonSerialString</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L164'>Property: pythonString</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L169'>Property: pythonVersion</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L200'>Function: auto_deco</a> <b>(Untested)</b>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L121'>Function: cache_clear</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L38'>Function: calculate</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L135'>Function: call_base_hooks</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L38'>Function: ceil</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L47'>Function: clamp</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L15'>Class: classproperty</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L121'>Function: clipboard_copy</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L134'>Function: clipboard_get</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L291'>Function: combine</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L16'>Function: comma_and_and</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L20'>Function: comma_and_or</a> <b>(Untested)</b>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L129'>Function: confineTo</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L178'>Function: debug</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L337'>Function: deco_bound_defaults</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L15'>Function: deco_cache</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L303'>Function: deco_cast_parameters</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L321'>Function: deco_cast_to_self</a> <b>(Untested)</b>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L357'>Function: deco_extend</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L280'>Function: deco_optional_suppress</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L368'>Function: deco_propagate_while</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L418'>Function: deco_require</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L61'>Function: defaults</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L91'>Function: depth</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L334'>Function: dict_insert</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L154'>Function: dir_appearance_order</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L104'>Function: doubleRectify</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/serialize.py#L24'>Function: dumps</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L261'>Function: exclusive</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L122'>Function: extend_list_in_dict</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L319'>Function: flatten</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L34'>Function: floor</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L167'>Function: get</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L164'>Function: getBaseClassNames</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L132'>Function: getBaseClasses</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L126'>Function: get_attrs_from_bases</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L255'>Function: get_definition_line</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L146'>Function: get_free_index</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L182'>Function: get_index</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L78'>Function: get_items</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L197'>Function: get_launch_options</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L210'>Function: get_origin</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L228'>Function: get_rows</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L70'>Function: get_values</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/object.py#L8'>Function: getsize</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L176'>Function: hasMethod</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L88'>Function: hook</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L266'>Function: inclusive</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L149'>Function: initBases</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L78'>Function: inrange</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/object.py#L34'>Function: interconnect</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L86'>Function: is_iterable</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L106'>Function: iter_first_value</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L117'>Function: join_with_str</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/serialize.py#L30'>Function: loads</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L46'>Function: match</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L314'>Function: pivot_list</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L25'>Function: plur_sing</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L231'>Function: print_link</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L246'>Function: print_link_to_obj</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L92'>Function: rectify</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L194'>Function: remove</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L282'>Function: remove_duplicates</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L36'>Function: replace</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L42'>Function: round_</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L61'>Function: sign</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L53'>Function: sleep</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L304'>Function: split_list</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L5'>Function: strToDynamicType</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L326'>Function: subtract_list</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L317'>Function: terminal</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L104'>Function: typeChecker</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L271'>Function: unique_obj_in_list</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L134'>Function: update_dict_in_dict</a>
+        └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L6'>Function: wrapper_transfer</a>
         </pre>
         
         ## Contributions
         Issue-creation and discussion is most welcome!
         
         Pull requests are **not wanted**, please discuss with me before investing any time.
         
         ## Todo
         | Module                                                                                                                      | Message                                                                                                                                                                        |
         |:----------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L1'>versions.py</a>        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L17'>Use Ver in each part of VerInfo.</a>                                     |
+        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L1'>test_time.py</a> | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L34'>Fix time casting to wrong day when past midnight.</a>              |
         | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/diagram.py#L1'>diagram.py</a>          | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/diagram.py#L446'>Shared dict for NetworkDiagram, resolve logic with multiple parents.</a> |
-        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L1'>test_time.py</a> | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L33'>Fix time casting to wrong day when past midnight.</a>              |
-        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L1'>objinfo.py</a>  | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L24'>Recycle ObjInfo.</a>                                              |
+        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L1'>versions.py</a>        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L17'>Use Ver in each part of VerInfo.</a>                                     |
         | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L1'>code.py</a>                | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L51'>Make Log use __name__ from previous frame so it doesn't write to root.</a>   |
         | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L1'>code.py</a>                | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L77'>Use another delimiter than , in Log and make sure it can handle quotes.</a>  |
+        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L1'>objinfo.py</a>  | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L24'>Recycle ObjInfo.</a>                                              |
         
         <sup>
-        Generated 2022-09-08 21:28 CEST for commit <a href='https://github.com/ManderaGeneral/generallibrary/commit/c5749cb'>c5749cb</a>.
+        Generated 2022-09-09 12:43 CEST for commit <a href='https://github.com/ManderaGeneral/generallibrary/commit/62348b6'>62348b6</a>.
         </sup>
         
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,44 +1,43 @@
-Metadata-Version: 2.1 Name: generallibrary Version: 2.9.8 Summary: Random
+Metadata-Version: 2.1 Name: generallibrary Version: 2.9.9 Summary: Random
 useful code categorized into modules. Home-page: https://github.com/
 ManderaGeneral/generallibrary Author: Rickard "Mandera" Abraham Author-email:
 rickard.abraham@gmail.com License: mit Description: # generallibrary Random
 useful code categorized into modules. ## Contents
         generallibrary
         ââ Installation
         ââ Information
         ââ Attributes
         ââ Contributions
         ââ Todo
-## Installation | Command | generalimport | packaging | pyperclip | tabulate |
-pytz | dill | matplotlib | networkx | pandas | |:------------------------------
-------|:---------------------------------------------------------------------|:
--------------------------------------------------------------|:----------------
----------------------------------------------|:--------------------------------
----------------------------|:--------------------------------------------------
--|:---------------------------------------------------|:-----------------------
-----------------------------------------|:-------------------------------------
-----------------------|:-------------------------------------------------------
-| | `pip install generallibrary` | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
-Yes | No | | `pip install generallibrary[table]` | Yes | Yes | Yes | Yes | Yes
-| Yes | Yes | Yes | Yes | | `pip install generallibrary[full]` | Yes | Yes |
-Yes | Yes | Yes | Yes | Yes | Yes | Yes | ## Information | Package | Ver |
-Latest Release | Python | Platform | Lvl | Todo | Cover | |:-------------------
-------------------------------------------------|:-----------------------------
----------------------|:----------------------|:--------------------------------
+## Installation | Command | generalimport | packaging | pyperclip | pytz | dill
+| matplotlib | networkx | pandas | tabulate | |:-------------------------------
+-----|:---------------------------------------------------------------------|:-
+------------------------------------------------------------|:-----------------
+--------------------------------------------|:---------------------------------
+------------------|:---------------------------------------------------|:------
+---------------------------------------------------------|:--------------------
+---------------------------------------|:--------------------------------------
+-----------------|:-----------------------------------------------------------
+| | `pip install generallibrary` | Yes | Yes | Yes | Yes | Yes | Yes | Yes | No
+| No | | `pip install generallibrary[table]` | Yes | Yes | Yes | Yes | Yes |
+Yes | Yes | Yes | Yes | | `pip install generallibrary[full]` | Yes | Yes | Yes
+| Yes | Yes | Yes | Yes | Yes | Yes | ## Information | Package | Ver | Latest
+Release | Python | Platform | Lvl | Todo | Cover | |:--------------------------
+-----------------------------------------|:------------------------------------
+--------------|:----------------------|:---------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------|:----
-------------|------:|:---------------------------------------------------------
---|:--------| | [generallibrary](https://github.com/ManderaGeneral/
-generallibrary) | [2.9.8](https://pypi.org/project/generallibrary/) | 2022-09-
-08 21:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
-[3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://
-www.python.org/downloads/release/python-3100/) | Windows, Ubuntu | 1 | [6]
-(https://github.com/ManderaGeneral/generallibrary#Todo) | 94.0 % | ##
-Attributes
+------------------------------------------------------------------|:-----------
+-----|------:|:-----------------------------------------------------------|:---
+-----| | [generallibrary](https://github.com/ManderaGeneral/generallibrary) |
+[2.9.9](https://pypi.org/project/generallibrary/) | 2022-09-09 12:43 CEST |
+[3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://
+www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/
+downloads/release/python-3100/) | Windows, Ubuntu | 1 | [6](https://github.com/
+ManderaGeneral/generallibrary#Todo) | 93.9 % | ## Attributes
         Module:_generallibrary
         ââ Class:_AutoInitBases
         ââ Class:_BoolStr
         ââ Class:_CallTable
         â  ââ Method:_generate
         â  ââ Method:_generate_with_args
         â  ââ Method:_generate_with_funcs
@@ -214,14 +213,15 @@
         ââ Function:_comma_and_and
         ââ Function:_comma_and_or (Untested)
         ââ Function:_confineTo
         ââ Function:_debug
         ââ Function:_deco_bound_defaults
         ââ Function:_deco_cache
         ââ Function:_deco_cast_parameters
+        ââ Function:_deco_cast_to_self (Untested)
         ââ Function:_deco_extend
         ââ Function:_deco_optional_suppress
         ââ Function:_deco_propagate_while
         ââ Function:_deco_require
         ââ Function:_defaults
         ââ Function:_depth
         ââ Function:_dict_insert
@@ -277,20 +277,20 @@
         ââ Function:_wrapper_transfer
 ## Contributions Issue-creation and discussion is most welcome! Pull requests
 are **not wanted**, please discuss with me before investing any time. ## Todo |
 Module | Message | |:----------------------------------------------------------
 ------------------------------------------------------------------|:-----------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-------| | versions.py | Use_Ver_in_each_part_of_VerInfo. | | diagram.py |
-Shared_dict_for_NetworkDiagram,_resolve_logic_with_multiple_parents. | |
-test_time.py | Fix_time_casting_to_wrong_day_when_past_midnight. | | objinfo.py
-| Recycle_ObjInfo. | | code.py | Make_Log_use___name___from_previous_frame_so
-it_doesn't_write_to_root. | | code.py | Use_another_delimiter_than_,_in_Log_and
-make_sure_it_can_handle_quotes. | Generated 2022-09-08 21:28 CEST for commit
-c5749cb. Platform: UNKNOWN Classifier: Topic :: Software Development ::
+------| | test_time.py | Fix_time_casting_to_wrong_day_when_past_midnight. | |
+diagram.py | Shared_dict_for_NetworkDiagram,_resolve_logic_with_multiple
+parents. | | versions.py | Use_Ver_in_each_part_of_VerInfo. | | code.py | Make
+Log_use___name___from_previous_frame_so_it_doesn't_write_to_root. | | code.py |
+Use_another_delimiter_than_,_in_Log_and_make_sure_it_can_handle_quotes. | |
+objinfo.py | Recycle_ObjInfo. | Generated 2022-09-09 12:43 CEST for commit
+62348b6. Platform: UNKNOWN Classifier: Topic :: Software Development ::
 Libraries Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 :: Linux Description-Content-Type: text/markdown Provides-Extra: table
 Provides-Extra: full
```

### Comparing `generallibrary-2.9.8/README.md` & `generallibrary-2.9.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,280 +9,281 @@
 ├─ <a href='#Attributes'>Attributes</a>
 ├─ <a href='#Contributions'>Contributions</a>
 └─ <a href='#Todo'>Todo</a>
 </pre>
 
 
 ## Installation
-| Command                             | <a href='https://pypi.org/project/generalimport'>generalimport</a>   | <a href='https://pypi.org/project/packaging'>packaging</a>   | <a href='https://pypi.org/project/pyperclip'>pyperclip</a>   | <a href='https://pypi.org/project/tabulate'>tabulate</a>   | <a href='https://pypi.org/project/pytz'>pytz</a>   | <a href='https://pypi.org/project/dill'>dill</a>   | <a href='https://pypi.org/project/matplotlib'>matplotlib</a>   | <a href='https://pypi.org/project/networkx'>networkx</a>   | <a href='https://pypi.org/project/pandas'>pandas</a>   |
-|:------------------------------------|:---------------------------------------------------------------------|:-------------------------------------------------------------|:-------------------------------------------------------------|:-----------------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------------------|:-----------------------------------------------------------|:-------------------------------------------------------|
-| `pip install generallibrary`        | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                        | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | No                                                     |
-| `pip install generallibrary[table]` | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                        | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    |
-| `pip install generallibrary[full]`  | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                        | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    |
+| Command                             | <a href='https://pypi.org/project/generalimport'>generalimport</a>   | <a href='https://pypi.org/project/packaging'>packaging</a>   | <a href='https://pypi.org/project/pyperclip'>pyperclip</a>   | <a href='https://pypi.org/project/pytz'>pytz</a>   | <a href='https://pypi.org/project/dill'>dill</a>   | <a href='https://pypi.org/project/matplotlib'>matplotlib</a>   | <a href='https://pypi.org/project/networkx'>networkx</a>   | <a href='https://pypi.org/project/pandas'>pandas</a>   | <a href='https://pypi.org/project/tabulate'>tabulate</a>   |
+|:------------------------------------|:---------------------------------------------------------------------|:-------------------------------------------------------------|:-------------------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------------------|:-----------------------------------------------------------|:-------------------------------------------------------|:-----------------------------------------------------------|
+| `pip install generallibrary`        | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | No                                                     | No                                                         |
+| `pip install generallibrary[table]` | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    | Yes                                                        |
+| `pip install generallibrary[full]`  | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    | Yes                                                        |
 
 ## Information
 | Package                                                            | Ver                                               | Latest Release        | Python                                                                                                                                                                                  | Platform        |   Lvl | Todo                                                       | Cover   |
 |:-------------------------------------------------------------------|:--------------------------------------------------|:----------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:-----------------------------------------------------------|:--------|
-| [generallibrary](https://github.com/ManderaGeneral/generallibrary) | [2.9.8](https://pypi.org/project/generallibrary/) | 2022-09-08 21:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/) | Windows, Ubuntu |     1 | [6](https://github.com/ManderaGeneral/generallibrary#Todo) | 94.0 %  |
+| [generallibrary](https://github.com/ManderaGeneral/generallibrary) | [2.9.9](https://pypi.org/project/generallibrary/) | 2022-09-09 12:43 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/) | Windows, Ubuntu |     1 | [6](https://github.com/ManderaGeneral/generallibrary#Todo) | 93.9 %  |
 
 ## Attributes
 <pre>
-<a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/__init__.py#L1'>Module: generallibrary</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L204'>Class: AutoInitBases</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L10'>Class: BoolStr</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L93'>Class: CallTable</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L138'>Method: generate</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L142'>Method: generate_with_args</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L146'>Method: generate_with_funcs</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L106'>Method: set_args</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L101'>Method: set_funcs</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L139'>Class: CodeLine</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L157'>Method: get_lines</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L172'>Method: text</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L230'>Class: DataClass</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L223'>Method: field_dict</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L217'>Method: field_values</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L61'>Class: Date</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L83'>Method: get_timezone_obj</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L87'>Method: now</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L6'>Class: DecoContext</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L17'>Method: after</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L14'>Method: before</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L84'>Class: EmptyContext</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L158'>Class: EnvVar</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L174'>Property: value</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L187'>Class: HierarchyStorer</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L28'>Class: Log</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L245'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L76'>Method: configure_file</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L80'>Method: configure_stream</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L61'>Method: critical</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L57'>Method: debug</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L60'>Method: error</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L58'>Method: info</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L88'>Method: is_root</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L84'>Method: loggers</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L309'>Method: recycle_clear</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L314'>Method: recycle_clear_all</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L59'>Method: warning</a> <b>(Untested)</b>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L542'>Class: Markdown</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L613'>Method: add_code_lines</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L579'>Method: add_lines</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L608'>Method: add_list_lines</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L619'>Method: add_pre_lines</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L599'>Method: add_table_lines</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L588'>Method: get_all_lines</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L572'>Method: get_section_lines</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L555'>Method: link</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L624'>Method: wrap_with_tags</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L503'>Class: NetworkDiagram</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L526'>Method: get_spouse</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L511'>Method: get_spouses</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L161'>Method: add_node</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/parents.py#L59'>Method: check_if_parent_eligible</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L141'>Method: defined_by_parent</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L241'>Method: disconnect</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L116'>Method: doc</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L52'>Method: file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L28'>Method: from_base</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L21'>Method: from_builtin</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L36'>Method: from_class</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L51'>Method: from_instance</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L58'>Method: from_module</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L252'>Method: get_all</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L181'>Method: get_child</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L350'>Method: get_children</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L91'>Method: get_definition_line</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L132'>Method: get_index</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L103'>Method: get_lines</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L207'>Method: get_node</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L388'>Method: get_nodes</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L269'>Method: get_ordered</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L233'>Method: get_ordered_index</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L85'>Method: get_origin</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L194'>Method: get_parent</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L369'>Method: get_parents</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L220'>Method: get_sibling</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L405'>Method: get_siblings</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L91'>Method: graph</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L62'>Method: identifier</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L17'>Method: internal</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L34'>Method: is_class</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L28'>Method: is_function</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L50'>Method: is_instance</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L59'>Method: is_method</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L22'>Method: is_module</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L44'>Method: is_property</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L43'>Method: module</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L75'>Method: print_link_to_obj</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L26'>Method: private</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L34'>Method: protected</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L9'>Method: public</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L170'>Method: remove_node</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L145'>Method: set_index</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L316'>Method: set_parent</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/parents.py#L7'>Method: spawn_parents</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L8'>Method: type</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L455'>Method: view</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L385'>Class: Operators</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L396'>Method: deco_define_comparisons</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L225'>Class: PythonVersion</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L231'>Property: version</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L212'>Class: Recycle</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L245'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L309'>Method: recycle_clear</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L314'>Method: recycle_clear_all</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L40'>Class: RedirectStdout</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L22'>Class: SigInfo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L265'>Method: call</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L48'>Property: callableObject</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L52'>Method: class_from_callable</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L178'>Property: defaults</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L220'>Method: getIndexFromName</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L146'>Property: leadingArgNames</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L126'>Property: names</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L136'>Property: namesRequired</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L131'>Property: namesWithoutDefaults</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L141'>Property: namesWithoutPacked</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L227'>Property: packedArgs</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L164'>Property: packedArgsName</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L232'>Property: packedKwargs</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L171'>Property: packedKwargsName</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L85'>Property: parameters</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L204'>Property: positionalArgNames</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L188'>Property: positionalOnlyArgNames</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L197'>Property: positionalOnlyOppositeArgNames</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L212'>Property: positionalOppositeArgNames</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L75'>Property: positional_extra</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L237'>Property: unpackedArgs</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L248'>Property: unpackedKwargs</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L5'>Class: SortedList</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L32'>Method: add</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L49'>Method: remove</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L292'>Class: Storable</a> <b>(Untested)</b>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L302'>Method: copy_node</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L297'>Method: load_node</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L294'>Method: save_node</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L11'>Class: Timer</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L41'>Method: deco</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L32'>Method: print</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L19'>Method: reset</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L26'>Method: seconds</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L432'>Class: TreeDiagram</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L455'>Method: view</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L15'>Class: Ver</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L29'>Method: bump</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L213'>Class: VerInfo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L177'>Property: caseSensitive</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L191'>Property: pathDelimiter</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L205'>Property: pathRootHasColon</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L198'>Property: pathRootIsDelimiter</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L184'>Property: positionalArgument</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L139'>Property: pythonAlpha</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L144'>Property: pythonBeta</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L149'>Property: pythonCandidate</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L154'>Property: pythonFinal</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L108'>Property: pythonMajor</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L118'>Property: pythonMicro</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L113'>Property: pythonMinor</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L159'>Property: pythonReleaseKeyword</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L123'>Property: pythonReleaseLevel</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L129'>Property: pythonSerial</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L134'>Property: pythonSerialString</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L164'>Property: pythonString</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L169'>Property: pythonVersion</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L202'>Function: auto_deco</a> <b>(Untested)</b>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L121'>Function: cache_clear</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L40'>Function: calculate</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L135'>Function: call_base_hooks</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L38'>Function: ceil</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L47'>Function: clamp</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L17'>Class: classproperty</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L121'>Function: clipboard_copy</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L134'>Function: clipboard_get</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L291'>Function: combine</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L16'>Function: comma_and_and</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L20'>Function: comma_and_or</a> <b>(Untested)</b>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L129'>Function: confineTo</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L178'>Function: debug</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L337'>Function: deco_bound_defaults</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L15'>Function: deco_cache</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L303'>Function: deco_cast_parameters</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L357'>Function: deco_extend</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L280'>Function: deco_optional_suppress</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L368'>Function: deco_propagate_while</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L418'>Function: deco_require</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L63'>Function: defaults</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L91'>Function: depth</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L334'>Function: dict_insert</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L154'>Function: dir_appearance_order</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L104'>Function: doubleRectify</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/serialize.py#L24'>Function: dumps</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L261'>Function: exclusive</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L122'>Function: extend_list_in_dict</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L319'>Function: flatten</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L34'>Function: floor</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L167'>Function: get</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L164'>Function: getBaseClassNames</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L132'>Function: getBaseClasses</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L126'>Function: get_attrs_from_bases</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L255'>Function: get_definition_line</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L146'>Function: get_free_index</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L182'>Function: get_index</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L78'>Function: get_items</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L197'>Function: get_launch_options</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L210'>Function: get_origin</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L228'>Function: get_rows</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L70'>Function: get_values</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/object.py#L8'>Function: getsize</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L176'>Function: hasMethod</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L88'>Function: hook</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L266'>Function: inclusive</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L151'>Function: initBases</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L78'>Function: inrange</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/object.py#L34'>Function: interconnect</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L86'>Function: is_iterable</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L106'>Function: iter_first_value</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L117'>Function: join_with_str</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/serialize.py#L30'>Function: loads</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L46'>Function: match</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L314'>Function: pivot_list</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L25'>Function: plur_sing</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L231'>Function: print_link</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L246'>Function: print_link_to_obj</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L92'>Function: rectify</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L194'>Function: remove</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L282'>Function: remove_duplicates</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L36'>Function: replace</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L42'>Function: round_</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L61'>Function: sign</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L53'>Function: sleep</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L304'>Function: split_list</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L5'>Function: strToDynamicType</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L326'>Function: subtract_list</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L319'>Function: terminal</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L104'>Function: typeChecker</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L271'>Function: unique_obj_in_list</a>
-├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L134'>Function: update_dict_in_dict</a>
-└─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L6'>Function: wrapper_transfer</a>
+<a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/__init__.py#L1'>Module: generallibrary</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L202'>Class: AutoInitBases</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L10'>Class: BoolStr</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L91'>Class: CallTable</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L136'>Method: generate</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L140'>Method: generate_with_args</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L144'>Method: generate_with_funcs</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L104'>Method: set_args</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L99'>Method: set_funcs</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L139'>Class: CodeLine</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L157'>Method: get_lines</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L172'>Method: text</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L230'>Class: DataClass</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L223'>Method: field_dict</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L217'>Method: field_values</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L61'>Class: Date</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L83'>Method: get_timezone_obj</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L87'>Method: now</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L6'>Class: DecoContext</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L17'>Method: after</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L14'>Method: before</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L82'>Class: EmptyContext</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L158'>Class: EnvVar</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L174'>Property: value</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L187'>Class: HierarchyStorer</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L28'>Class: Log</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L243'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L76'>Method: configure_file</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L80'>Method: configure_stream</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L61'>Method: critical</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L57'>Method: debug</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L60'>Method: error</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L58'>Method: info</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L88'>Method: is_root</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L84'>Method: loggers</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L307'>Method: recycle_clear</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L312'>Method: recycle_clear_all</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L59'>Method: warning</a> <b>(Untested)</b>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L542'>Class: Markdown</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L613'>Method: add_code_lines</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L579'>Method: add_lines</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L608'>Method: add_list_lines</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L619'>Method: add_pre_lines</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L599'>Method: add_table_lines</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L588'>Method: get_all_lines</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L572'>Method: get_section_lines</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L555'>Method: link</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L624'>Method: wrap_with_tags</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L503'>Class: NetworkDiagram</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L526'>Method: get_spouse</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L511'>Method: get_spouses</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L161'>Method: add_node</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/parents.py#L59'>Method: check_if_parent_eligible</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L141'>Method: defined_by_parent</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L241'>Method: disconnect</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L116'>Method: doc</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L52'>Method: file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L28'>Method: from_base</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L21'>Method: from_builtin</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L36'>Method: from_class</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L51'>Method: from_instance</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L58'>Method: from_module</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L252'>Method: get_all</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L181'>Method: get_child</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L350'>Method: get_children</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L91'>Method: get_definition_line</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L132'>Method: get_index</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L103'>Method: get_lines</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L207'>Method: get_node</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L388'>Method: get_nodes</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L269'>Method: get_ordered</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L233'>Method: get_ordered_index</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L85'>Method: get_origin</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L194'>Method: get_parent</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L369'>Method: get_parents</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L220'>Method: get_sibling</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L405'>Method: get_siblings</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L91'>Method: graph</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L62'>Method: identifier</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L17'>Method: internal</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L34'>Method: is_class</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L28'>Method: is_function</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L50'>Method: is_instance</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L59'>Method: is_method</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L22'>Method: is_module</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L44'>Method: is_property</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L43'>Method: module</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L75'>Method: print_link_to_obj</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L26'>Method: private</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L34'>Method: protected</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L9'>Method: public</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L170'>Method: remove_node</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L145'>Method: set_index</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L316'>Method: set_parent</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/parents.py#L7'>Method: spawn_parents</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L8'>Method: type</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L455'>Method: view</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L385'>Class: Operators</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L396'>Method: deco_define_comparisons</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L225'>Class: PythonVersion</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L231'>Property: version</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L210'>Class: Recycle</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L243'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L307'>Method: recycle_clear</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L312'>Method: recycle_clear_all</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L40'>Class: RedirectStdout</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L22'>Class: SigInfo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L265'>Method: call</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L48'>Property: callableObject</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L52'>Method: class_from_callable</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L178'>Property: defaults</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L220'>Method: getIndexFromName</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L146'>Property: leadingArgNames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L126'>Property: names</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L136'>Property: namesRequired</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L131'>Property: namesWithoutDefaults</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L141'>Property: namesWithoutPacked</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L227'>Property: packedArgs</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L164'>Property: packedArgsName</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L232'>Property: packedKwargs</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L171'>Property: packedKwargsName</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L85'>Property: parameters</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L204'>Property: positionalArgNames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L188'>Property: positionalOnlyArgNames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L197'>Property: positionalOnlyOppositeArgNames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L212'>Property: positionalOppositeArgNames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L75'>Property: positional_extra</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L237'>Property: unpackedArgs</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L248'>Property: unpackedKwargs</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L5'>Class: SortedList</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L32'>Method: add</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L49'>Method: remove</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L292'>Class: Storable</a> <b>(Untested)</b>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L302'>Method: copy_node</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L297'>Method: load_node</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L294'>Method: save_node</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L11'>Class: Timer</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L41'>Method: deco</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L32'>Method: print</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L19'>Method: reset</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L26'>Method: seconds</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L432'>Class: TreeDiagram</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L455'>Method: view</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L15'>Class: Ver</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L29'>Method: bump</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L213'>Class: VerInfo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L177'>Property: caseSensitive</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L191'>Property: pathDelimiter</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L205'>Property: pathRootHasColon</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L198'>Property: pathRootIsDelimiter</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L184'>Property: positionalArgument</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L139'>Property: pythonAlpha</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L144'>Property: pythonBeta</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L149'>Property: pythonCandidate</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L154'>Property: pythonFinal</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L108'>Property: pythonMajor</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L118'>Property: pythonMicro</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L113'>Property: pythonMinor</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L159'>Property: pythonReleaseKeyword</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L123'>Property: pythonReleaseLevel</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L129'>Property: pythonSerial</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L134'>Property: pythonSerialString</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L164'>Property: pythonString</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L169'>Property: pythonVersion</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L200'>Function: auto_deco</a> <b>(Untested)</b>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L121'>Function: cache_clear</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L38'>Function: calculate</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L135'>Function: call_base_hooks</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L38'>Function: ceil</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L47'>Function: clamp</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L15'>Class: classproperty</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L121'>Function: clipboard_copy</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L134'>Function: clipboard_get</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L291'>Function: combine</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L16'>Function: comma_and_and</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L20'>Function: comma_and_or</a> <b>(Untested)</b>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L129'>Function: confineTo</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L178'>Function: debug</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L337'>Function: deco_bound_defaults</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L15'>Function: deco_cache</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L303'>Function: deco_cast_parameters</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L321'>Function: deco_cast_to_self</a> <b>(Untested)</b>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L357'>Function: deco_extend</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L280'>Function: deco_optional_suppress</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L368'>Function: deco_propagate_while</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L418'>Function: deco_require</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L61'>Function: defaults</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L91'>Function: depth</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L334'>Function: dict_insert</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L154'>Function: dir_appearance_order</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L104'>Function: doubleRectify</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/serialize.py#L24'>Function: dumps</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L261'>Function: exclusive</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L122'>Function: extend_list_in_dict</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L319'>Function: flatten</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L34'>Function: floor</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L167'>Function: get</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L164'>Function: getBaseClassNames</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L132'>Function: getBaseClasses</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L126'>Function: get_attrs_from_bases</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L255'>Function: get_definition_line</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L146'>Function: get_free_index</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L182'>Function: get_index</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L78'>Function: get_items</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L197'>Function: get_launch_options</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L210'>Function: get_origin</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L228'>Function: get_rows</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L70'>Function: get_values</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/object.py#L8'>Function: getsize</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L176'>Function: hasMethod</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L88'>Function: hook</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L266'>Function: inclusive</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L149'>Function: initBases</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L78'>Function: inrange</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/object.py#L34'>Function: interconnect</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L86'>Function: is_iterable</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L106'>Function: iter_first_value</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L117'>Function: join_with_str</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/serialize.py#L30'>Function: loads</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L46'>Function: match</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L314'>Function: pivot_list</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L25'>Function: plur_sing</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L231'>Function: print_link</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L246'>Function: print_link_to_obj</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L92'>Function: rectify</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L194'>Function: remove</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L282'>Function: remove_duplicates</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L36'>Function: replace</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L42'>Function: round_</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L61'>Function: sign</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L53'>Function: sleep</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L304'>Function: split_list</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L5'>Function: strToDynamicType</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L326'>Function: subtract_list</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L317'>Function: terminal</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L104'>Function: typeChecker</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L271'>Function: unique_obj_in_list</a>
+├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L134'>Function: update_dict_in_dict</a>
+└─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L6'>Function: wrapper_transfer</a>
 </pre>
 
 ## Contributions
 Issue-creation and discussion is most welcome!
 
 Pull requests are **not wanted**, please discuss with me before investing any time.
 
 ## Todo
 | Module                                                                                                                      | Message                                                                                                                                                                        |
 |:----------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L1'>versions.py</a>        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L17'>Use Ver in each part of VerInfo.</a>                                     |
+| <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L1'>test_time.py</a> | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L34'>Fix time casting to wrong day when past midnight.</a>              |
 | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/diagram.py#L1'>diagram.py</a>          | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/diagram.py#L446'>Shared dict for NetworkDiagram, resolve logic with multiple parents.</a> |
-| <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L1'>test_time.py</a> | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L33'>Fix time casting to wrong day when past midnight.</a>              |
-| <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L1'>objinfo.py</a>  | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L24'>Recycle ObjInfo.</a>                                              |
+| <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L1'>versions.py</a>        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L17'>Use Ver in each part of VerInfo.</a>                                     |
 | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L1'>code.py</a>                | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L51'>Make Log use __name__ from previous frame so it doesn't write to root.</a>   |
 | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L1'>code.py</a>                | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L77'>Use another delimiter than , in Log and make sure it can handle quotes.</a>  |
+| <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L1'>objinfo.py</a>  | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L24'>Recycle ObjInfo.</a>                                              |
 
 <sup>
-Generated 2022-09-08 21:28 CEST for commit <a href='https://github.com/ManderaGeneral/generallibrary/commit/c5749cb'>c5749cb</a>.
+Generated 2022-09-09 12:43 CEST for commit <a href='https://github.com/ManderaGeneral/generallibrary/commit/62348b6'>62348b6</a>.
 </sup>
```

#### html2text {}

```diff
@@ -1,40 +1,39 @@
 # generallibrary Random useful code categorized into modules. ## Contents
 generallibrary
 ââ Installation
 ââ Information
 ââ Attributes
 ââ Contributions
 ââ Todo
-## Installation | Command | generalimport | packaging | pyperclip | tabulate |
-pytz | dill | matplotlib | networkx | pandas | |:------------------------------
-------|:---------------------------------------------------------------------|:
--------------------------------------------------------------|:----------------
----------------------------------------------|:--------------------------------
----------------------------|:--------------------------------------------------
--|:---------------------------------------------------|:-----------------------
-----------------------------------------|:-------------------------------------
-----------------------|:-------------------------------------------------------
-| | `pip install generallibrary` | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
-Yes | No | | `pip install generallibrary[table]` | Yes | Yes | Yes | Yes | Yes
-| Yes | Yes | Yes | Yes | | `pip install generallibrary[full]` | Yes | Yes |
-Yes | Yes | Yes | Yes | Yes | Yes | Yes | ## Information | Package | Ver |
-Latest Release | Python | Platform | Lvl | Todo | Cover | |:-------------------
-------------------------------------------------|:-----------------------------
----------------------|:----------------------|:--------------------------------
+## Installation | Command | generalimport | packaging | pyperclip | pytz | dill
+| matplotlib | networkx | pandas | tabulate | |:-------------------------------
+-----|:---------------------------------------------------------------------|:-
+------------------------------------------------------------|:-----------------
+--------------------------------------------|:---------------------------------
+------------------|:---------------------------------------------------|:------
+---------------------------------------------------------|:--------------------
+---------------------------------------|:--------------------------------------
+-----------------|:-----------------------------------------------------------
+| | `pip install generallibrary` | Yes | Yes | Yes | Yes | Yes | Yes | Yes | No
+| No | | `pip install generallibrary[table]` | Yes | Yes | Yes | Yes | Yes |
+Yes | Yes | Yes | Yes | | `pip install generallibrary[full]` | Yes | Yes | Yes
+| Yes | Yes | Yes | Yes | Yes | Yes | ## Information | Package | Ver | Latest
+Release | Python | Platform | Lvl | Todo | Cover | |:--------------------------
+-----------------------------------------|:------------------------------------
+--------------|:----------------------|:---------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------|:----
-------------|------:|:---------------------------------------------------------
---|:--------| | [generallibrary](https://github.com/ManderaGeneral/
-generallibrary) | [2.9.8](https://pypi.org/project/generallibrary/) | 2022-09-
-08 21:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
-[3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://
-www.python.org/downloads/release/python-3100/) | Windows, Ubuntu | 1 | [6]
-(https://github.com/ManderaGeneral/generallibrary#Todo) | 94.0 % | ##
-Attributes
+------------------------------------------------------------------|:-----------
+-----|------:|:-----------------------------------------------------------|:---
+-----| | [generallibrary](https://github.com/ManderaGeneral/generallibrary) |
+[2.9.9](https://pypi.org/project/generallibrary/) | 2022-09-09 12:43 CEST |
+[3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://
+www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/
+downloads/release/python-3100/) | Windows, Ubuntu | 1 | [6](https://github.com/
+ManderaGeneral/generallibrary#Todo) | 93.9 % | ## Attributes
 Module:_generallibrary
 ââ Class:_AutoInitBases
 ââ Class:_BoolStr
 ââ Class:_CallTable
 â  ââ Method:_generate
 â  ââ Method:_generate_with_args
 â  ââ Method:_generate_with_funcs
@@ -210,14 +209,15 @@
 ââ Function:_comma_and_and
 ââ Function:_comma_and_or (Untested)
 ââ Function:_confineTo
 ââ Function:_debug
 ââ Function:_deco_bound_defaults
 ââ Function:_deco_cache
 ââ Function:_deco_cast_parameters
+ââ Function:_deco_cast_to_self (Untested)
 ââ Function:_deco_extend
 ââ Function:_deco_optional_suppress
 ââ Function:_deco_propagate_while
 ââ Function:_deco_require
 ââ Function:_defaults
 ââ Function:_depth
 ââ Function:_dict_insert
@@ -273,14 +273,14 @@
 ââ Function:_wrapper_transfer
 ## Contributions Issue-creation and discussion is most welcome! Pull requests
 are **not wanted**, please discuss with me before investing any time. ## Todo |
 Module | Message | |:----------------------------------------------------------
 ------------------------------------------------------------------|:-----------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-------| | versions.py | Use_Ver_in_each_part_of_VerInfo. | | diagram.py |
-Shared_dict_for_NetworkDiagram,_resolve_logic_with_multiple_parents. | |
-test_time.py | Fix_time_casting_to_wrong_day_when_past_midnight. | | objinfo.py
-| Recycle_ObjInfo. | | code.py | Make_Log_use___name___from_previous_frame_so
-it_doesn't_write_to_root. | | code.py | Use_another_delimiter_than_,_in_Log_and
-make_sure_it_can_handle_quotes. | Generated 2022-09-08 21:28 CEST for commit
-c5749cb.
+------| | test_time.py | Fix_time_casting_to_wrong_day_when_past_midnight. | |
+diagram.py | Shared_dict_for_NetworkDiagram,_resolve_logic_with_multiple
+parents. | | versions.py | Use_Ver_in_each_part_of_VerInfo. | | code.py | Make
+Log_use___name___from_previous_frame_so_it_doesn't_write_to_root. | | code.py |
+Use_another_delimiter_than_,_in_Log_and_make_sure_it_can_handle_quotes. | |
+objinfo.py | Recycle_ObjInfo. | Generated 2022-09-09 12:43 CEST for commit
+62348b6.
```

### Comparing `generallibrary-2.9.8/generallibrary/__init__.py` & `generallibrary-2.9.9/generallibrary/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 from generalimport import *
 
-GeneralImporter("pandas")
+generalimport("pandas", "tabulate")
 
 # from generallibrary.analyze import bayesian
 from generallibrary.iterables import SortedList, get_values, is_iterable, depth, iter_first_value, iter_first_value, join_with_str, extend_list_in_dict, update_dict_in_dict, get_free_index, get_rows, exclusive, inclusive, unique_obj_in_list, combine, remove_duplicates, get_index, get, get_items, split_list, pivot_list, remove, flatten, subtract_list, dict_insert
 from generallibrary.object import getsize, interconnect
 from generallibrary.text import comma_and_and, comma_and_or, plur_sing, replace, match
 from generallibrary.time import Timer, sleep, Date
 from generallibrary.types import strToDynamicType, typeChecker, getBaseClasses, getBaseClassNames, hasMethod, HierarchyStorer
 from generallibrary.functions import CallTable, calculate, defaults, EmptyContext, classproperty, initBases, AutoInitBases, Recycle, \
     terminal, auto_deco
-from generallibrary.decorators import deco_optional_suppress, deco_cache, deco_cast_parameters, deco_bound_defaults, deco_extend, deco_propagate_while, Operators, wrapper_transfer, SigInfo, deco_require
+from generallibrary.decorators import deco_optional_suppress, deco_cache, deco_cast_parameters, deco_bound_defaults, deco_extend, deco_propagate_while, Operators, wrapper_transfer, SigInfo, deco_require, deco_cast_to_self
 from generallibrary.values import BoolStr, floor, ceil, round_, clamp, sign, inrange, rectify, doubleRectify, confineTo, EnvVar, get_launch_options
 from generallibrary.diagram import TreeDiagram, Markdown, NetworkDiagram, Storable
 from generallibrary.code import debug, CodeLine, clipboard_copy, clipboard_get, print_link, print_link_to_obj, get_definition_line, get_origin, Log
 from generallibrary.versions import VerInfo, PythonVersion, Ver
 from generallibrary.objinfo.objinfo import ObjInfo, hook, cache_clear, call_base_hooks, DataClass, get_attrs_from_bases, dir_appearance_order
 from generallibrary.serialize import dumps, loads
 from generallibrary.context import DecoContext, RedirectStdout
```

### Comparing `generallibrary-2.9.8/generallibrary/code.py` & `generallibrary-2.9.9/generallibrary/code.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/context.py` & `generallibrary-2.9.9/generallibrary/context.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/decorators.py` & `generallibrary-2.9.9/generallibrary/decorators.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/diagram.py` & `generallibrary-2.9.9/generallibrary/diagram.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/functions.py` & `generallibrary-2.9.9/generallibrary/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
+
 from generallibrary.decorators import wrapper_transfer, SigInfo
 from generallibrary.iterables import remove
 
 import re
 
 import json
 import subprocess
 import sys
 from collections import ChainMap
 
 import pandas as pd
 
-# pandas = import_module("pandas", error=False)
-# importlib.import_module(name="pandas")
-
 
 class classproperty:
     """ Just like @property but for a class method.
         @classproperty
         def foo(cls):
             return cls.bar
         https://stackoverflow.com/a/13624858/3936044 """
```

### Comparing `generallibrary-2.9.8/generallibrary/iterables.py` & `generallibrary-2.9.9/generallibrary/iterables.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/object.py` & `generallibrary-2.9.9/generallibrary/object.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/objinfo/children.py` & `generallibrary-2.9.9/generallibrary/objinfo/children.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/objinfo/objinfo.py` & `generallibrary-2.9.9/generallibrary/objinfo/objinfo.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/objinfo/origin.py` & `generallibrary-2.9.9/generallibrary/objinfo/origin.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/objinfo/parents.py` & `generallibrary-2.9.9/generallibrary/objinfo/parents.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/objinfo/properties.py` & `generallibrary-2.9.9/generallibrary/objinfo/properties.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/objinfo/type.py` & `generallibrary-2.9.9/generallibrary/objinfo/type.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/serialize.py` & `generallibrary-2.9.9/generallibrary/serialize.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/test/calltable_objinfo.py` & `generallibrary-2.9.9/generallibrary/test/calltable_objinfo.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/test/calltable_origin.py` & `generallibrary-2.9.9/generallibrary/test/calltable_origin.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/test/positional.py` & `generallibrary-2.9.9/generallibrary/test/positional.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/test/test_code.py` & `generallibrary-2.9.9/generallibrary/test/test_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from generallibrary.code import *
-from generallibrary.versions import VerInfo
+from generallibrary import VerInfo
 
 import unittest
 
 
 class CodeTest(unittest.TestCase):
     @unittest.skipIf(VerInfo().linux, "Clipboard - Couldn't get to work in linux VM, maybe works in normal linux environment.")
     def test_clipboard(self):
```

### Comparing `generallibrary-2.9.8/generallibrary/test/test_context.py` & `generallibrary-2.9.9/generallibrary/test/test_context.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/test/test_dataclass.py` & `generallibrary-2.9.9/generallibrary/test/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/test/test_decorators.py` & `generallibrary-2.9.9/generallibrary/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/test/test_diagram.py` & `generallibrary-2.9.9/generallibrary/test/test_diagram.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/test/test_functions.py` & `generallibrary-2.9.9/generallibrary/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/test/test_iterables.py` & `generallibrary-2.9.9/generallibrary/test/test_iterables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import generallibrary
 from generallibrary.iterables import *
 
 import unittest
 
 
 class IterablesTest(unittest.TestCase):
     def test_get_keys(self):
```

### Comparing `generallibrary-2.9.8/generallibrary/test/test_object.py` & `generallibrary-2.9.9/generallibrary/test/test_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import generallibrary
 from generallibrary.object import *
 from generallibrary.objinfo.objinfo import *
 from generallibrary.functions import initBases, AutoInitBases
 
 import unittest
 
 
@@ -379,15 +380,15 @@
         self.assertEqual(False, ObjInfo(_Bar.self).from_module())
 
         objInfo = ObjInfo(_Bar())
         self.assertEqual(True, objInfo.get_child(filt=lambda node: node.name == "instance_var", traverse_excluded=True).from_instance())
         self.assertEqual(True, objInfo.get_child(filt=lambda node: node.name == "self", traverse_excluded=True).from_base())
 
     def test_get_definition_line(self):
-        self.assertEqual(22, ObjInfo(ObjectTest).get_definition_line())
+        self.assertEqual(23, ObjInfo(ObjectTest).get_definition_line())
 
     def test_get_origin(self):
         class FooBar:
             @property
             def test(self):
                 return
```

### Comparing `generallibrary-2.9.8/generallibrary/test/test_serialize.py` & `generallibrary-2.9.9/generallibrary/test/test_serialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import generallibrary
 from generallibrary.serialize import *
 
 import unittest
 
 
 class SerializeTest(unittest.TestCase):
     def test_serialize(self):
```

### Comparing `generallibrary-2.9.8/generallibrary/test/test_text.py` & `generallibrary-2.9.9/generallibrary/test/test_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import generallibrary
 from generallibrary.text import *
 
 import unittest
 
 
 class CodeTest(unittest.TestCase):
     def test_comma_and_and(self):
```

### Comparing `generallibrary-2.9.8/generallibrary/test/test_time.py` & `generallibrary-2.9.9/generallibrary/test/test_time.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import generallibrary
 from generallibrary.time import *
 
 import unittest
 
 
 class TimeTest(unittest.TestCase):
     def test_timerAndSleep(self):
```

### Comparing `generallibrary-2.9.8/generallibrary/test/test_types.py` & `generallibrary-2.9.9/generallibrary/test/test_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import generallibrary
 from generallibrary.types import *
 
 import unittest
 
 
 class InheritStr(str):
     pass
```

### Comparing `generallibrary-2.9.8/generallibrary/test/test_values.py` & `generallibrary-2.9.9/generallibrary/test/test_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import generallibrary
 from generallibrary.values import *
 
 import unittest
 
 
 class ValuesTest(unittest.TestCase):
     def test_BoolStr(self):
```

### Comparing `generallibrary-2.9.8/generallibrary/test/test_versions.py` & `generallibrary-2.9.9/generallibrary/test/test_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+import generallibrary
 from generallibrary.versions import *
 
 import unittest
 import os
 
 
 class VersionsTest(unittest.TestCase):
```

### Comparing `generallibrary-2.9.8/generallibrary/text.py` & `generallibrary-2.9.9/generallibrary/text.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/time.py` & `generallibrary-2.9.9/generallibrary/time.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/types.py` & `generallibrary-2.9.9/generallibrary/types.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/values.py` & `generallibrary-2.9.9/generallibrary/values.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary/versions.py` & `generallibrary-2.9.9/generallibrary/versions.py`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/generallibrary.egg-info/PKG-INFO` & `generallibrary-2.9.9/generallibrary.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generallibrary
-Version: 2.9.8
+Version: 2.9.9
 Summary: Random useful code categorized into modules.
 Home-page: https://github.com/ManderaGeneral/generallibrary
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Description: # generallibrary
         Random useful code categorized into modules.
@@ -17,286 +17,287 @@
         ├─ <a href='#Attributes'>Attributes</a>
         ├─ <a href='#Contributions'>Contributions</a>
         └─ <a href='#Todo'>Todo</a>
         </pre>
         
         
         ## Installation
-        | Command                             | <a href='https://pypi.org/project/generalimport'>generalimport</a>   | <a href='https://pypi.org/project/packaging'>packaging</a>   | <a href='https://pypi.org/project/pyperclip'>pyperclip</a>   | <a href='https://pypi.org/project/tabulate'>tabulate</a>   | <a href='https://pypi.org/project/pytz'>pytz</a>   | <a href='https://pypi.org/project/dill'>dill</a>   | <a href='https://pypi.org/project/matplotlib'>matplotlib</a>   | <a href='https://pypi.org/project/networkx'>networkx</a>   | <a href='https://pypi.org/project/pandas'>pandas</a>   |
-        |:------------------------------------|:---------------------------------------------------------------------|:-------------------------------------------------------------|:-------------------------------------------------------------|:-----------------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------------------|:-----------------------------------------------------------|:-------------------------------------------------------|
-        | `pip install generallibrary`        | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                        | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | No                                                     |
-        | `pip install generallibrary[table]` | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                        | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    |
-        | `pip install generallibrary[full]`  | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                        | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    |
+        | Command                             | <a href='https://pypi.org/project/generalimport'>generalimport</a>   | <a href='https://pypi.org/project/packaging'>packaging</a>   | <a href='https://pypi.org/project/pyperclip'>pyperclip</a>   | <a href='https://pypi.org/project/pytz'>pytz</a>   | <a href='https://pypi.org/project/dill'>dill</a>   | <a href='https://pypi.org/project/matplotlib'>matplotlib</a>   | <a href='https://pypi.org/project/networkx'>networkx</a>   | <a href='https://pypi.org/project/pandas'>pandas</a>   | <a href='https://pypi.org/project/tabulate'>tabulate</a>   |
+        |:------------------------------------|:---------------------------------------------------------------------|:-------------------------------------------------------------|:-------------------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------|:---------------------------------------------------------------|:-----------------------------------------------------------|:-------------------------------------------------------|:-----------------------------------------------------------|
+        | `pip install generallibrary`        | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | No                                                     | No                                                         |
+        | `pip install generallibrary[table]` | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    | Yes                                                        |
+        | `pip install generallibrary[full]`  | Yes                                                                  | Yes                                                          | Yes                                                          | Yes                                                | Yes                                                | Yes                                                            | Yes                                                        | Yes                                                    | Yes                                                        |
         
         ## Information
         | Package                                                            | Ver                                               | Latest Release        | Python                                                                                                                                                                                  | Platform        |   Lvl | Todo                                                       | Cover   |
         |:-------------------------------------------------------------------|:--------------------------------------------------|:----------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|------:|:-----------------------------------------------------------|:--------|
-        | [generallibrary](https://github.com/ManderaGeneral/generallibrary) | [2.9.8](https://pypi.org/project/generallibrary/) | 2022-09-08 21:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/) | Windows, Ubuntu |     1 | [6](https://github.com/ManderaGeneral/generallibrary#Todo) | 94.0 %  |
+        | [generallibrary](https://github.com/ManderaGeneral/generallibrary) | [2.9.9](https://pypi.org/project/generallibrary/) | 2022-09-09 12:43 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/) | Windows, Ubuntu |     1 | [6](https://github.com/ManderaGeneral/generallibrary#Todo) | 93.9 %  |
         
         ## Attributes
         <pre>
-        <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/__init__.py#L1'>Module: generallibrary</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L204'>Class: AutoInitBases</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L10'>Class: BoolStr</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L93'>Class: CallTable</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L138'>Method: generate</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L142'>Method: generate_with_args</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L146'>Method: generate_with_funcs</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L106'>Method: set_args</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L101'>Method: set_funcs</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L139'>Class: CodeLine</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L157'>Method: get_lines</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L172'>Method: text</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L230'>Class: DataClass</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L223'>Method: field_dict</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L217'>Method: field_values</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L61'>Class: Date</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L83'>Method: get_timezone_obj</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L87'>Method: now</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L6'>Class: DecoContext</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L17'>Method: after</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L14'>Method: before</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L84'>Class: EmptyContext</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L158'>Class: EnvVar</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L174'>Property: value</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L187'>Class: HierarchyStorer</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L28'>Class: Log</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L245'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L76'>Method: configure_file</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L80'>Method: configure_stream</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L61'>Method: critical</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L57'>Method: debug</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L60'>Method: error</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L58'>Method: info</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L88'>Method: is_root</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L84'>Method: loggers</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L309'>Method: recycle_clear</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L314'>Method: recycle_clear_all</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L59'>Method: warning</a> <b>(Untested)</b>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L542'>Class: Markdown</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L613'>Method: add_code_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L579'>Method: add_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L608'>Method: add_list_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L619'>Method: add_pre_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L599'>Method: add_table_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L588'>Method: get_all_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L572'>Method: get_section_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L555'>Method: link</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L624'>Method: wrap_with_tags</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L503'>Class: NetworkDiagram</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L526'>Method: get_spouse</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L511'>Method: get_spouses</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L161'>Method: add_node</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/parents.py#L59'>Method: check_if_parent_eligible</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L141'>Method: defined_by_parent</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L241'>Method: disconnect</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L116'>Method: doc</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L52'>Method: file</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L28'>Method: from_base</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L21'>Method: from_builtin</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L36'>Method: from_class</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L51'>Method: from_instance</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/origin.py#L58'>Method: from_module</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L252'>Method: get_all</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L181'>Method: get_child</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L350'>Method: get_children</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L91'>Method: get_definition_line</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L132'>Method: get_index</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L103'>Method: get_lines</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L207'>Method: get_node</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L388'>Method: get_nodes</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L269'>Method: get_ordered</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L233'>Method: get_ordered_index</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L85'>Method: get_origin</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L194'>Method: get_parent</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L369'>Method: get_parents</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L220'>Method: get_sibling</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L405'>Method: get_siblings</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L91'>Method: graph</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L62'>Method: identifier</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L17'>Method: internal</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L34'>Method: is_class</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L28'>Method: is_function</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L50'>Method: is_instance</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L59'>Method: is_method</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L22'>Method: is_module</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L44'>Method: is_property</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L43'>Method: module</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L75'>Method: print_link_to_obj</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L26'>Method: private</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L34'>Method: protected</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/properties.py#L9'>Method: public</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L170'>Method: remove_node</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L145'>Method: set_index</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L316'>Method: set_parent</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/parents.py#L7'>Method: spawn_parents</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/type.py#L8'>Method: type</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L455'>Method: view</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L385'>Class: Operators</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L396'>Method: deco_define_comparisons</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L225'>Class: PythonVersion</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L231'>Property: version</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L212'>Class: Recycle</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L245'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L309'>Method: recycle_clear</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L314'>Method: recycle_clear_all</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/context.py#L40'>Class: RedirectStdout</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L22'>Class: SigInfo</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L265'>Method: call</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L48'>Property: callableObject</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L52'>Method: class_from_callable</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L178'>Property: defaults</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L220'>Method: getIndexFromName</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L146'>Property: leadingArgNames</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L126'>Property: names</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L136'>Property: namesRequired</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L131'>Property: namesWithoutDefaults</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L141'>Property: namesWithoutPacked</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L227'>Property: packedArgs</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L164'>Property: packedArgsName</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L232'>Property: packedKwargs</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L171'>Property: packedKwargsName</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L85'>Property: parameters</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L204'>Property: positionalArgNames</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L188'>Property: positionalOnlyArgNames</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L197'>Property: positionalOnlyOppositeArgNames</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L212'>Property: positionalOppositeArgNames</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L75'>Property: positional_extra</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L237'>Property: unpackedArgs</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L248'>Property: unpackedKwargs</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L5'>Class: SortedList</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L32'>Method: add</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L49'>Method: remove</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L292'>Class: Storable</a> <b>(Untested)</b>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L302'>Method: copy_node</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L297'>Method: load_node</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L294'>Method: save_node</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L11'>Class: Timer</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L41'>Method: deco</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L32'>Method: print</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L19'>Method: reset</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L26'>Method: seconds</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L432'>Class: TreeDiagram</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/diagram.py#L455'>Method: view</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L15'>Class: Ver</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L29'>Method: bump</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L213'>Class: VerInfo</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L177'>Property: caseSensitive</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L191'>Property: pathDelimiter</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L205'>Property: pathRootHasColon</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L198'>Property: pathRootIsDelimiter</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L184'>Property: positionalArgument</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L139'>Property: pythonAlpha</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L144'>Property: pythonBeta</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L149'>Property: pythonCandidate</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L154'>Property: pythonFinal</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L108'>Property: pythonMajor</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L118'>Property: pythonMicro</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L113'>Property: pythonMinor</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L159'>Property: pythonReleaseKeyword</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L123'>Property: pythonReleaseLevel</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L129'>Property: pythonSerial</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L134'>Property: pythonSerialString</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L164'>Property: pythonString</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/versions.py#L169'>Property: pythonVersion</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L202'>Function: auto_deco</a> <b>(Untested)</b>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L121'>Function: cache_clear</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L40'>Function: calculate</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L135'>Function: call_base_hooks</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L38'>Function: ceil</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L47'>Function: clamp</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L17'>Class: classproperty</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L121'>Function: clipboard_copy</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L134'>Function: clipboard_get</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L291'>Function: combine</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L16'>Function: comma_and_and</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L20'>Function: comma_and_or</a> <b>(Untested)</b>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L129'>Function: confineTo</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L178'>Function: debug</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L337'>Function: deco_bound_defaults</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L15'>Function: deco_cache</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L303'>Function: deco_cast_parameters</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L357'>Function: deco_extend</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L280'>Function: deco_optional_suppress</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L368'>Function: deco_propagate_while</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L418'>Function: deco_require</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L63'>Function: defaults</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L91'>Function: depth</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L334'>Function: dict_insert</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L154'>Function: dir_appearance_order</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L104'>Function: doubleRectify</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/serialize.py#L24'>Function: dumps</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L261'>Function: exclusive</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L122'>Function: extend_list_in_dict</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L319'>Function: flatten</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L34'>Function: floor</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L167'>Function: get</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L164'>Function: getBaseClassNames</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L132'>Function: getBaseClasses</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L126'>Function: get_attrs_from_bases</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L255'>Function: get_definition_line</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L146'>Function: get_free_index</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L182'>Function: get_index</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L78'>Function: get_items</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L197'>Function: get_launch_options</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L210'>Function: get_origin</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L228'>Function: get_rows</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L70'>Function: get_values</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/object.py#L8'>Function: getsize</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L176'>Function: hasMethod</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/objinfo/objinfo.py#L88'>Function: hook</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L266'>Function: inclusive</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L151'>Function: initBases</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L78'>Function: inrange</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/object.py#L34'>Function: interconnect</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L86'>Function: is_iterable</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L106'>Function: iter_first_value</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L117'>Function: join_with_str</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/serialize.py#L30'>Function: loads</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L46'>Function: match</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L314'>Function: pivot_list</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L25'>Function: plur_sing</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L231'>Function: print_link</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/code.py#L246'>Function: print_link_to_obj</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L92'>Function: rectify</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L194'>Function: remove</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L282'>Function: remove_duplicates</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/text.py#L36'>Function: replace</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L42'>Function: round_</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/values.py#L61'>Function: sign</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/time.py#L53'>Function: sleep</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L304'>Function: split_list</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L5'>Function: strToDynamicType</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L326'>Function: subtract_list</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/functions.py#L319'>Function: terminal</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/types.py#L104'>Function: typeChecker</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L271'>Function: unique_obj_in_list</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/iterables.py#L134'>Function: update_dict_in_dict</a>
-        └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/c5749cb/generallibrary/decorators.py#L6'>Function: wrapper_transfer</a>
+        <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/__init__.py#L1'>Module: generallibrary</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L202'>Class: AutoInitBases</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L10'>Class: BoolStr</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L91'>Class: CallTable</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L136'>Method: generate</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L140'>Method: generate_with_args</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L144'>Method: generate_with_funcs</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L104'>Method: set_args</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L99'>Method: set_funcs</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L139'>Class: CodeLine</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L157'>Method: get_lines</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L172'>Method: text</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L230'>Class: DataClass</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L223'>Method: field_dict</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L217'>Method: field_values</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L61'>Class: Date</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L83'>Method: get_timezone_obj</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L87'>Method: now</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L6'>Class: DecoContext</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L17'>Method: after</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L14'>Method: before</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L82'>Class: EmptyContext</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L158'>Class: EnvVar</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L174'>Property: value</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L187'>Class: HierarchyStorer</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L28'>Class: Log</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L243'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L76'>Method: configure_file</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L80'>Method: configure_stream</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L61'>Method: critical</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L57'>Method: debug</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L60'>Method: error</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L58'>Method: info</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L88'>Method: is_root</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L84'>Method: loggers</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L307'>Method: recycle_clear</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L312'>Method: recycle_clear_all</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L59'>Method: warning</a> <b>(Untested)</b>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L542'>Class: Markdown</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L613'>Method: add_code_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L579'>Method: add_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L608'>Method: add_list_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L619'>Method: add_pre_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L599'>Method: add_table_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L588'>Method: get_all_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L572'>Method: get_section_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L555'>Method: link</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L624'>Method: wrap_with_tags</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L503'>Class: NetworkDiagram</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L526'>Method: get_spouse</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L511'>Method: get_spouses</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L19'>Class: ObjInfo</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L161'>Method: add_node</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/parents.py#L59'>Method: check_if_parent_eligible</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L141'>Method: defined_by_parent</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L241'>Method: disconnect</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L116'>Method: doc</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L52'>Method: file</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L28'>Method: from_base</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L21'>Method: from_builtin</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L36'>Method: from_class</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L51'>Method: from_instance</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/origin.py#L58'>Method: from_module</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L252'>Method: get_all</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L181'>Method: get_child</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L350'>Method: get_children</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L91'>Method: get_definition_line</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L132'>Method: get_index</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L103'>Method: get_lines</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L207'>Method: get_node</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L388'>Method: get_nodes</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L269'>Method: get_ordered</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L233'>Method: get_ordered_index</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L85'>Method: get_origin</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L194'>Method: get_parent</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L369'>Method: get_parents</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L220'>Method: get_sibling</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L405'>Method: get_siblings</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L91'>Method: graph</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L62'>Method: identifier</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L17'>Method: internal</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L34'>Method: is_class</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L28'>Method: is_function</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L50'>Method: is_instance</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L59'>Method: is_method</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L22'>Method: is_module</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L44'>Method: is_property</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L43'>Method: module</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L75'>Method: print_link_to_obj</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L26'>Method: private</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L34'>Method: protected</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/properties.py#L9'>Method: public</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L170'>Method: remove_node</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L145'>Method: set_index</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L316'>Method: set_parent</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/parents.py#L7'>Method: spawn_parents</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/type.py#L8'>Method: type</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L455'>Method: view</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L385'>Class: Operators</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L396'>Method: deco_define_comparisons</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L225'>Class: PythonVersion</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L231'>Property: version</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L210'>Class: Recycle</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L243'>Method: assert_max_one_missing_name</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L307'>Method: recycle_clear</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L312'>Method: recycle_clear_all</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/context.py#L40'>Class: RedirectStdout</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L22'>Class: SigInfo</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L265'>Method: call</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L48'>Property: callableObject</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L52'>Method: class_from_callable</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L178'>Property: defaults</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L220'>Method: getIndexFromName</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L146'>Property: leadingArgNames</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L126'>Property: names</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L136'>Property: namesRequired</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L131'>Property: namesWithoutDefaults</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L141'>Property: namesWithoutPacked</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L227'>Property: packedArgs</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L164'>Property: packedArgsName</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L232'>Property: packedKwargs</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L171'>Property: packedKwargsName</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L85'>Property: parameters</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L204'>Property: positionalArgNames</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L188'>Property: positionalOnlyArgNames</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L197'>Property: positionalOnlyOppositeArgNames</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L212'>Property: positionalOppositeArgNames</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L75'>Property: positional_extra</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L237'>Property: unpackedArgs</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L248'>Property: unpackedKwargs</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L5'>Class: SortedList</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L32'>Method: add</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L49'>Method: remove</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L292'>Class: Storable</a> <b>(Untested)</b>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L302'>Method: copy_node</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L297'>Method: load_node</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L294'>Method: save_node</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L11'>Class: Timer</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L41'>Method: deco</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L32'>Method: print</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L19'>Method: reset</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L26'>Method: seconds</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L432'>Class: TreeDiagram</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/diagram.py#L455'>Method: view</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L15'>Class: Ver</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L29'>Method: bump</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L213'>Class: VerInfo</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L177'>Property: caseSensitive</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L191'>Property: pathDelimiter</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L205'>Property: pathRootHasColon</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L198'>Property: pathRootIsDelimiter</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L184'>Property: positionalArgument</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L139'>Property: pythonAlpha</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L144'>Property: pythonBeta</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L149'>Property: pythonCandidate</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L154'>Property: pythonFinal</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L108'>Property: pythonMajor</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L118'>Property: pythonMicro</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L113'>Property: pythonMinor</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L159'>Property: pythonReleaseKeyword</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L123'>Property: pythonReleaseLevel</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L129'>Property: pythonSerial</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L134'>Property: pythonSerialString</a>
+        │  ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L164'>Property: pythonString</a>
+        │  └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/versions.py#L169'>Property: pythonVersion</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L200'>Function: auto_deco</a> <b>(Untested)</b>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L121'>Function: cache_clear</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L38'>Function: calculate</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L135'>Function: call_base_hooks</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L38'>Function: ceil</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L47'>Function: clamp</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L15'>Class: classproperty</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L121'>Function: clipboard_copy</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L134'>Function: clipboard_get</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L291'>Function: combine</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L16'>Function: comma_and_and</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L20'>Function: comma_and_or</a> <b>(Untested)</b>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L129'>Function: confineTo</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L178'>Function: debug</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L337'>Function: deco_bound_defaults</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L15'>Function: deco_cache</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L303'>Function: deco_cast_parameters</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L321'>Function: deco_cast_to_self</a> <b>(Untested)</b>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L357'>Function: deco_extend</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L280'>Function: deco_optional_suppress</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L368'>Function: deco_propagate_while</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L418'>Function: deco_require</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L61'>Function: defaults</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L91'>Function: depth</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L334'>Function: dict_insert</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L154'>Function: dir_appearance_order</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L104'>Function: doubleRectify</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/serialize.py#L24'>Function: dumps</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L261'>Function: exclusive</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L122'>Function: extend_list_in_dict</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L319'>Function: flatten</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L34'>Function: floor</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L167'>Function: get</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L164'>Function: getBaseClassNames</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L132'>Function: getBaseClasses</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L126'>Function: get_attrs_from_bases</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L255'>Function: get_definition_line</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L146'>Function: get_free_index</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L182'>Function: get_index</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L78'>Function: get_items</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L197'>Function: get_launch_options</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L210'>Function: get_origin</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L228'>Function: get_rows</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L70'>Function: get_values</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/object.py#L8'>Function: getsize</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L176'>Function: hasMethod</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/objinfo/objinfo.py#L88'>Function: hook</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L266'>Function: inclusive</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L149'>Function: initBases</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L78'>Function: inrange</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/object.py#L34'>Function: interconnect</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L86'>Function: is_iterable</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L106'>Function: iter_first_value</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L117'>Function: join_with_str</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/serialize.py#L30'>Function: loads</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L46'>Function: match</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L314'>Function: pivot_list</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L25'>Function: plur_sing</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L231'>Function: print_link</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/code.py#L246'>Function: print_link_to_obj</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L92'>Function: rectify</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L194'>Function: remove</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L282'>Function: remove_duplicates</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/text.py#L36'>Function: replace</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L42'>Function: round_</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/values.py#L61'>Function: sign</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/time.py#L53'>Function: sleep</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L304'>Function: split_list</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L5'>Function: strToDynamicType</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L326'>Function: subtract_list</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/functions.py#L317'>Function: terminal</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/types.py#L104'>Function: typeChecker</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L271'>Function: unique_obj_in_list</a>
+        ├─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/iterables.py#L134'>Function: update_dict_in_dict</a>
+        └─ <a href='https://github.com/ManderaGeneral/generallibrary/blob/62348b6/generallibrary/decorators.py#L6'>Function: wrapper_transfer</a>
         </pre>
         
         ## Contributions
         Issue-creation and discussion is most welcome!
         
         Pull requests are **not wanted**, please discuss with me before investing any time.
         
         ## Todo
         | Module                                                                                                                      | Message                                                                                                                                                                        |
         |:----------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L1'>versions.py</a>        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L17'>Use Ver in each part of VerInfo.</a>                                     |
+        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L1'>test_time.py</a> | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L34'>Fix time casting to wrong day when past midnight.</a>              |
         | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/diagram.py#L1'>diagram.py</a>          | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/diagram.py#L446'>Shared dict for NetworkDiagram, resolve logic with multiple parents.</a> |
-        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L1'>test_time.py</a> | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/test/test_time.py#L33'>Fix time casting to wrong day when past midnight.</a>              |
-        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L1'>objinfo.py</a>  | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L24'>Recycle ObjInfo.</a>                                              |
+        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L1'>versions.py</a>        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/versions.py#L17'>Use Ver in each part of VerInfo.</a>                                     |
         | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L1'>code.py</a>                | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L51'>Make Log use __name__ from previous frame so it doesn't write to root.</a>   |
         | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L1'>code.py</a>                | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/code.py#L77'>Use another delimiter than , in Log and make sure it can handle quotes.</a>  |
+        | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L1'>objinfo.py</a>  | <a href='https://github.com/ManderaGeneral/generallibrary/blob/master/generallibrary/objinfo/objinfo.py#L24'>Recycle ObjInfo.</a>                                              |
         
         <sup>
-        Generated 2022-09-08 21:28 CEST for commit <a href='https://github.com/ManderaGeneral/generallibrary/commit/c5749cb'>c5749cb</a>.
+        Generated 2022-09-09 12:43 CEST for commit <a href='https://github.com/ManderaGeneral/generallibrary/commit/62348b6'>62348b6</a>.
         </sup>
         
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,44 +1,43 @@
-Metadata-Version: 2.1 Name: generallibrary Version: 2.9.8 Summary: Random
+Metadata-Version: 2.1 Name: generallibrary Version: 2.9.9 Summary: Random
 useful code categorized into modules. Home-page: https://github.com/
 ManderaGeneral/generallibrary Author: Rickard "Mandera" Abraham Author-email:
 rickard.abraham@gmail.com License: mit Description: # generallibrary Random
 useful code categorized into modules. ## Contents
         generallibrary
         ââ Installation
         ââ Information
         ââ Attributes
         ââ Contributions
         ââ Todo
-## Installation | Command | generalimport | packaging | pyperclip | tabulate |
-pytz | dill | matplotlib | networkx | pandas | |:------------------------------
-------|:---------------------------------------------------------------------|:
--------------------------------------------------------------|:----------------
----------------------------------------------|:--------------------------------
----------------------------|:--------------------------------------------------
--|:---------------------------------------------------|:-----------------------
-----------------------------------------|:-------------------------------------
-----------------------|:-------------------------------------------------------
-| | `pip install generallibrary` | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
-Yes | No | | `pip install generallibrary[table]` | Yes | Yes | Yes | Yes | Yes
-| Yes | Yes | Yes | Yes | | `pip install generallibrary[full]` | Yes | Yes |
-Yes | Yes | Yes | Yes | Yes | Yes | Yes | ## Information | Package | Ver |
-Latest Release | Python | Platform | Lvl | Todo | Cover | |:-------------------
-------------------------------------------------|:-----------------------------
----------------------|:----------------------|:--------------------------------
+## Installation | Command | generalimport | packaging | pyperclip | pytz | dill
+| matplotlib | networkx | pandas | tabulate | |:-------------------------------
+-----|:---------------------------------------------------------------------|:-
+------------------------------------------------------------|:-----------------
+--------------------------------------------|:---------------------------------
+------------------|:---------------------------------------------------|:------
+---------------------------------------------------------|:--------------------
+---------------------------------------|:--------------------------------------
+-----------------|:-----------------------------------------------------------
+| | `pip install generallibrary` | Yes | Yes | Yes | Yes | Yes | Yes | Yes | No
+| No | | `pip install generallibrary[table]` | Yes | Yes | Yes | Yes | Yes |
+Yes | Yes | Yes | Yes | | `pip install generallibrary[full]` | Yes | Yes | Yes
+| Yes | Yes | Yes | Yes | Yes | Yes | ## Information | Package | Ver | Latest
+Release | Python | Platform | Lvl | Todo | Cover | |:--------------------------
+-----------------------------------------|:------------------------------------
+--------------|:----------------------|:---------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------|:----
-------------|------:|:---------------------------------------------------------
---|:--------| | [generallibrary](https://github.com/ManderaGeneral/
-generallibrary) | [2.9.8](https://pypi.org/project/generallibrary/) | 2022-09-
-08 21:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
-[3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://
-www.python.org/downloads/release/python-3100/) | Windows, Ubuntu | 1 | [6]
-(https://github.com/ManderaGeneral/generallibrary#Todo) | 94.0 % | ##
-Attributes
+------------------------------------------------------------------|:-----------
+-----|------:|:-----------------------------------------------------------|:---
+-----| | [generallibrary](https://github.com/ManderaGeneral/generallibrary) |
+[2.9.9](https://pypi.org/project/generallibrary/) | 2022-09-09 12:43 CEST |
+[3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://
+www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/
+downloads/release/python-3100/) | Windows, Ubuntu | 1 | [6](https://github.com/
+ManderaGeneral/generallibrary#Todo) | 93.9 % | ## Attributes
         Module:_generallibrary
         ââ Class:_AutoInitBases
         ââ Class:_BoolStr
         ââ Class:_CallTable
         â  ââ Method:_generate
         â  ââ Method:_generate_with_args
         â  ââ Method:_generate_with_funcs
@@ -214,14 +213,15 @@
         ââ Function:_comma_and_and
         ââ Function:_comma_and_or (Untested)
         ââ Function:_confineTo
         ââ Function:_debug
         ââ Function:_deco_bound_defaults
         ââ Function:_deco_cache
         ââ Function:_deco_cast_parameters
+        ââ Function:_deco_cast_to_self (Untested)
         ââ Function:_deco_extend
         ââ Function:_deco_optional_suppress
         ââ Function:_deco_propagate_while
         ââ Function:_deco_require
         ââ Function:_defaults
         ââ Function:_depth
         ââ Function:_dict_insert
@@ -277,20 +277,20 @@
         ââ Function:_wrapper_transfer
 ## Contributions Issue-creation and discussion is most welcome! Pull requests
 are **not wanted**, please discuss with me before investing any time. ## Todo |
 Module | Message | |:----------------------------------------------------------
 ------------------------------------------------------------------|:-----------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-------| | versions.py | Use_Ver_in_each_part_of_VerInfo. | | diagram.py |
-Shared_dict_for_NetworkDiagram,_resolve_logic_with_multiple_parents. | |
-test_time.py | Fix_time_casting_to_wrong_day_when_past_midnight. | | objinfo.py
-| Recycle_ObjInfo. | | code.py | Make_Log_use___name___from_previous_frame_so
-it_doesn't_write_to_root. | | code.py | Use_another_delimiter_than_,_in_Log_and
-make_sure_it_can_handle_quotes. | Generated 2022-09-08 21:28 CEST for commit
-c5749cb. Platform: UNKNOWN Classifier: Topic :: Software Development ::
+------| | test_time.py | Fix_time_casting_to_wrong_day_when_past_midnight. | |
+diagram.py | Shared_dict_for_NetworkDiagram,_resolve_logic_with_multiple
+parents. | | versions.py | Use_Ver_in_each_part_of_VerInfo. | | code.py | Make
+Log_use___name___from_previous_frame_so_it_doesn't_write_to_root. | | code.py |
+Use_another_delimiter_than_,_in_Log_and_make_sure_it_can_handle_quotes. | |
+objinfo.py | Recycle_ObjInfo. | Generated 2022-09-09 12:43 CEST for commit
+62348b6. Platform: UNKNOWN Classifier: Topic :: Software Development ::
 Libraries Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 :: Linux Description-Content-Type: text/markdown Provides-Extra: table
 Provides-Extra: full
```

### Comparing `generallibrary-2.9.8/generallibrary.egg-info/SOURCES.txt` & `generallibrary-2.9.9/generallibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generallibrary-2.9.8/metadata.json` & `generallibrary-2.9.9/metadata.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.93125%*

 * *Differences: {"'extras_require'": "{'table': {insert: [(1, 'tabulate')]}, 'full': {insert: [(1, 'tabulate')]}}",*

 * * "'install_requires'": '{delete: [3]}',*

 * * "'version'": "'2.9.9'"}*

```diff
@@ -1,30 +1,31 @@
 {
     "description": "Random useful code categorized into modules.",
     "enabled": true,
     "extras_require": {
         "full": [
-            "pandas"
+            "pandas",
+            "tabulate"
         ],
         "table": [
-            "pandas"
+            "pandas",
+            "tabulate"
         ]
     },
     "install_requires": [
         "generalimport",
         "packaging",
         "pyperclip",
-        "tabulate",
         "pytz",
         "dill",
         "matplotlib",
         "networkx"
     ],
     "manifest": [],
     "name": "generallibrary",
     "private": false,
     "target": "python",
     "topics": [
         "library"
     ],
-    "version": "2.9.8"
+    "version": "2.9.9"
 }
```

### Comparing `generallibrary-2.9.8/setup.py` & `generallibrary-2.9.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,34 +7,33 @@
 except FileNotFoundError:
     long_description = 'Readme missing'
 
 setup(
     name="generallibrary",
     author='Rickard "Mandera" Abraham',
     author_email="rickard.abraham@gmail.com",
-    version="2.9.8",
+    version="2.9.9",
     description="Random useful code categorized into modules.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'generalimport',
         'packaging',
         'pyperclip',
-        'tabulate',
         'pytz',
         'dill',
         'matplotlib',
         'networkx',
     ],
     url="https://github.com/ManderaGeneral/generallibrary",
     license="mit",
     packages=find_namespace_packages(exclude=("build*", "dist*")),
     extras_require={
-        'table': ['pandas'],
-        'full': ['pandas'],
+        'table': ['pandas', 'tabulate'],
+        'full': ['pandas', 'tabulate'],
     },
     classifiers=[
         'Topic :: Software Development :: Libraries',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: MIT License',
```

