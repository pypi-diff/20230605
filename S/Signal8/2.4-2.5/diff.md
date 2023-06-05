# Comparing `tmp/Signal8-2.4.tar.gz` & `tmp/Signal8-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-2.4.tar", last modified: Mon Jun  5 16:10:27 2023, max compression
+gzip compressed data, was "Signal8-2.5.tar", last modified: Mon Jun  5 16:19:00 2023, max compression
```

## Comparing `Signal8-2.4.tar` & `Signal8-2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:10:27.561843 Signal8-2.4/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.4/LICENSE
--rw-rw-rw-   0        0        0     4369 2023-06-05 16:10:27.558843 Signal8-2.4/PKG-INFO
--rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 16:10:27.460845 Signal8-2.4/Signal8/
--rw-rw-rw-   0        0        0    11151 2023-06-05 16:08:37.000000 Signal8-2.4/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-2.4/Signal8/__init__.py
--rw-rw-rw-   0        0        0      238 2023-06-05 16:05:24.000000 Signal8-2.4/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:10:27.554845 Signal8-2.4/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.4/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5811 2023-06-02 21:00:42.000000 Signal8-2.4/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2783 2023-06-01 21:15:18.000000 Signal8-2.4/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     5020 2023-06-05 15:51:06.000000 Signal8-2.4/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.4/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12412 2023-06-05 16:05:19.000000 Signal8-2.4/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.4/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:10:27.524845 Signal8-2.4/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4369 2023-06-05 16:10:27.000000 Signal8-2.4/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-05 16:10:27.000000 Signal8-2.4/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:10:27.000000 Signal8-2.4/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 16:10:27.000000 Signal8-2.4/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 16:10:27.562845 Signal8-2.4/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-05 16:08:42.000000 Signal8-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:19:00.715335 Signal8-2.5/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.5/LICENSE
+-rw-rw-rw-   0        0        0     4369 2023-06-05 16:19:00.698337 Signal8-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 16:19:00.616335 Signal8-2.5/Signal8/
+-rw-rw-rw-   0        0        0    11151 2023-06-05 16:08:37.000000 Signal8-2.5/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       72 2023-06-05 16:17:41.000000 Signal8-2.5/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      238 2023-06-05 16:05:24.000000 Signal8-2.5/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:19:00.694334 Signal8-2.5/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.5/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5811 2023-06-02 21:00:42.000000 Signal8-2.5/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2783 2023-06-01 21:15:18.000000 Signal8-2.5/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     5020 2023-06-05 15:51:06.000000 Signal8-2.5/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.5/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12412 2023-06-05 16:05:19.000000 Signal8-2.5/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.5/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:19:00.645334 Signal8-2.5/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4369 2023-06-05 16:19:00.000000 Signal8-2.5/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-05 16:19:00.000000 Signal8-2.5/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:19:00.000000 Signal8-2.5/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 16:19:00.000000 Signal8-2.5/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 16:19:00.715335 Signal8-2.5/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-05 16:17:46.000000 Signal8-2.5/setup.py
```

### Comparing `Signal8-2.4/LICENSE` & `Signal8-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-2.4/PKG-INFO` & `Signal8-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.4
+Version: 2.5
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.4/README.md` & `Signal8-2.5/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-2.4/Signal8/Signal8.py` & `Signal8-2.5/Signal8/Signal8.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.4/Signal8/utils/core.py` & `Signal8-2.5/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.4/Signal8/utils/npc.py` & `Signal8-2.5/Signal8/utils/npc.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.4/Signal8/utils/problems.py` & `Signal8-2.5/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.4/Signal8/utils/simple_env.py` & `Signal8-2.5/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.4/Signal8/utils/test_dynamic_obs.py` & `Signal8-2.5/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.4/Signal8.egg-info/PKG-INFO` & `Signal8-2.5/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.4
+Version: 2.5
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.4/Signal8.egg-info/SOURCES.txt` & `Signal8-2.5/Signal8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Signal8-2.4/setup.py` & `Signal8-2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="2.4",
+    version="2.5",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

