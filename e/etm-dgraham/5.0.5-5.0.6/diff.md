# Comparing `tmp/etm-dgraham-5.0.5.tar.gz` & `tmp/etm-dgraham-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.0.5.tar", last modified: Mon Jun  5 10:28:37 2023, max compression
+gzip compressed data, was "etm-dgraham-5.0.6.tar", last modified: Mon Jun  5 16:41:52 2023, max compression
```

## Comparing `etm-dgraham-5.0.5.tar` & `etm-dgraham-5.0.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.138224 etm-dgraham-5.0.5/
--rw-r--r--   0 dag        (501) staff       (20)     2380 2023-06-05 10:28:27.000000 etm-dgraham-5.0.5/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.5/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   129427 2023-06-05 10:28:37.138067 etm-dgraham-5.0.5/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   128515 2023-06-04 22:28:52.000000 etm-dgraham-5.0.5/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.5/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.5/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.131060 etm-dgraham-5.0.5/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.5/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.5/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.5/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.133967 etm-dgraham-5.0.5/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.5/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-03 11:21:41.000000 etm-dgraham-5.0.5/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-05 10:28:27.000000 etm-dgraham-5.0.5/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.5/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.5/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.5/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   277778 2023-06-05 10:28:27.000000 etm-dgraham-5.0.5/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37255 2023-05-23 18:01:39.000000 etm-dgraham-5.0.5/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.5/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)    97115 2023-06-05 10:28:27.000000 etm-dgraham-5.0.5/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.136336 etm-dgraham-5.0.5/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   129427 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.5/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.5/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.5/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.5/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.5/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.5/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-05 10:28:37.138263 etm-dgraham-5.0.5/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.5/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.136448 etm-dgraham-5.0.5/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.5/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.137507 etm-dgraham-5.0.5/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.5/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.5/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.5/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.5/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.498357 etm-dgraham-5.0.6/
+-rw-r--r--   0 dag        (501) staff       (20)     2373 2023-06-05 16:41:33.000000 etm-dgraham-5.0.6/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.6/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   129427 2023-06-05 16:41:52.498197 etm-dgraham-5.0.6/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   128515 2023-06-04 22:28:52.000000 etm-dgraham-5.0.6/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.6/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.6/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.488544 etm-dgraham-5.0.6/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.6/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.6/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.6/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.493010 etm-dgraham-5.0.6/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.6/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-03 11:21:41.000000 etm-dgraham-5.0.6/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-05 16:41:33.000000 etm-dgraham-5.0.6/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.6/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.6/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.6/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   277830 2023-06-05 16:41:33.000000 etm-dgraham-5.0.6/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37255 2023-05-23 18:01:39.000000 etm-dgraham-5.0.6/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.6/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    97610 2023-06-05 16:41:33.000000 etm-dgraham-5.0.6/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.495446 etm-dgraham-5.0.6/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   129427 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.6/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.6/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.6/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.6/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.6/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.6/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-05 16:41:52.498393 etm-dgraham-5.0.6/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.6/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.495558 etm-dgraham-5.0.6/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.6/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.497575 etm-dgraham-5.0.6/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.6/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.6/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.6/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.6/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.0.5/CHANGES.txt` & `etm-dgraham-5.0.6/CHANGES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-Recent tagged changes as of 2023-06-05T06:28:25.850318-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.0.5) Daniel Graham
+Recent tagged changes as of 2023-06-05T12:41:31.118562-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.0.6) Daniel Graham
+    345ca4e 2023-06-05 12:41:31 -0400
+    Tagged version 5.0.6.
+
+- 6 hours ago (tag: 5.0.5) Daniel Graham
     9273685 2023-06-05 06:28:25 -0400
     Tagged version 5.0.5.
 
-- 25 minutes ago (tag: 5.0.4) Daniel Graham
+- 7 hours ago (tag: 5.0.4) Daniel Graham
     ea199ac 2023-06-05 06:02:56 -0400
     Tagged version 5.0.4.
 
-- 14 hours ago (tag: 5.0.3) Daniel Graham
+- 20 hours ago (tag: 5.0.3) Daniel Graham
     e0a0d9e 2023-06-04 16:44:49 -0400
     Tagged version 5.0.3.
 
-- 17 hours ago (tag: 5.0.2) Daniel Graham
+- 23 hours ago (tag: 5.0.2) Daniel Graham
     4c5d4bb 2023-06-04 13:26:17 -0400
     Tagged version 5.0.2.
 
-- 18 hours ago (tag: 5.0.1) Daniel Graham
+- 24 hours ago (tag: 5.0.1) Daniel Graham
     b30f0ed 2023-06-04 12:47:15 -0400
     Tagged version 5.0.1.
 
 - 2 days ago (tag: 5.0.0) Daniel Graham
     7bc8090 2023-06-03 07:21:38 -0400
     Tagged version 5.0.0. Use pendulum periods for f and elements of h
     instead of datetimes.
@@ -72,11 +76,7 @@
 - 4 weeks ago (tag: 4.11.17) Daniel Graham
     8a02515 2023-05-09 10:14:28 -0400
     Tagged version 4.11.17.
 
 - 5 weeks ago (tag: 4.11.16) Daniel Graham
     b2310ce 2023-05-01 14:43:18 -0400
     Tagged version 4.11.16.
-
-- 5 weeks ago (tag: 4.11.15) Daniel Graham
-    96aff42 2023-05-01 14:12:10 -0400
-    Tagged version 4.11.15.
```

### Comparing `etm-dgraham-5.0.5/PKG-INFO` & `etm-dgraham-5.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.5
+Version: 5.0.6
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.0.5/README.md` & `etm-dgraham-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/bump.py` & `etm-dgraham-5.0.6/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/docs/index_konnections.md` & `etm-dgraham-5.0.6/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/docs/index_usedtime.md` & `etm-dgraham-5.0.6/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/docs/multiple_timers.md` & `etm-dgraham-5.0.6/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etm/__main__.py` & `etm-dgraham-5.0.6/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etm/data.py` & `etm-dgraham-5.0.6/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etm/ical.py` & `etm-dgraham-5.0.6/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etm/make_examples.py` & `etm-dgraham-5.0.6/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etm/model.py` & `etm-dgraham-5.0.6/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1401,14 +1401,17 @@
         if x in mpr:
             del mpr[x]
         if x in xst:
             del xst[x]
     return mpr == xst
 
 
+def completion_evaluator(s):
+    return f"got {s}"
+
 def datetime_calculator(s):
     """
     s has the format:
 
         x [+-] y
 
     where x is a datetime and y is either a datetime or a timeperiod.
```

### Comparing `etm-dgraham-5.0.5/etm/options.py` & `etm-dgraham-5.0.6/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etm/report.py` & `etm-dgraham-5.0.6/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etm/view.py` & `etm-dgraham-5.0.6/etm/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -623,17 +623,15 @@
 
         def accept_text(buf):
             get_app().layout.focus(ok_button)
             buf.complete_state = None
             return True
 
         def accept():
-            self.set_label('\nworking ...\n')
             get_app().invalidate()
-            time.sleep(.1)
             self.future.set_result(self.text_area.text)
 
         def cancel():
             self.future.set_result(None)
 
         self.text_area = TextArea(
             completer=completer,
@@ -2211,41 +2209,58 @@
             title=title,
             label_text=text,
             default=entry,
             )
         done_str = yield from show_dialog_as_float(dialog)
 
         if not done_str:
-            # None (cancelled) or null string
-            return
+            # show_message('Finish', 'Cancelled')
+            return None
 
         done_parts = [x.strip() for x in done_str.split(':')]
 
+        msg = ""
         num_parts = len(done_parts)
         if num_parts != need:
-            show_message('finish 1', f"Cancelled, {done_str} is invalid")
-            return
+            ok = False
+            msg = f"Cancelled, the entry, {done_str}, is invalid"
 
         elif num_parts == 2:
             num = int(done_parts[0])
             # only return due for instance other than the oldest
             # due = between[num] if num else ""
-            due = between[num]
-            done = parse_datetime(done_parts[1], z='local')[1]
+            if num in range(len(between)):
+                due = between[num]
+            else:
+                msg = f"Cancelled, '{num}' is not in [{', '.join([str(x) for x in range(len(between))])}]"
+
+            ok, res, z = parse_datetime(done_parts[1], z='local')
+            if ok:
+                done = res
+            else:
+                msg = f"Cancelled, '{done_parts[1]}' is not a valid datetime"
+
         elif num_parts == 1:
-            done = parse_datetime(done_str, z='local')[1]
+            ok, res, z = parse_datetime(done_str, z='local')
+            if ok:
+                done = res
+            else:
+                msg = f"Cancelled, '{done_str}' is not a valid datetime"
             due = between[0] if between[0] else done
 
+        if msg:
+            show_message('Finish', msg)
+            return
+
         done = model.date_to_datetime(done)
         due = model.date_to_datetime(due)
 
-
         changed = item.finish_item(doc_id, job, done, due)
 
-        if changed:
+        if not msg and changed:
             if doc_id in dataview.itemcache:
                 del dataview.itemcache[doc_id]
             application.layout.focus(text_area)
             set_text(dataview.show_active_view())
             loop = asyncio.get_event_loop()
             loop.call_later(0, data_changed, loop)
         else:
```

### Comparing `etm-dgraham-5.0.5/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.0.6/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.5
+Version: 5.0.6
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.0.5/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.0.6/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.0.6/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etmlogo.png` & `etm-dgraham-5.0.6/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etmlogo_small.png` & `etm-dgraham-5.0.6/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/etmview_agenda.png` & `etm-dgraham-5.0.6/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/namedcolors.py` & `etm-dgraham-5.0.6/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/new.png` & `etm-dgraham-5.0.6/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/setup.py` & `etm-dgraham-5.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/test/test_parser.py` & `etm-dgraham-5.0.6/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/utilities/colons_to_slashes.py` & `etm-dgraham-5.0.6/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/utilities/etm_in` & `etm-dgraham-5.0.6/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/utilities/inbasket` & `etm-dgraham-5.0.6/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.5/utilities/open_in_mutt` & `etm-dgraham-5.0.6/utilities/open_in_mutt`

 * *Files identical despite different names*

