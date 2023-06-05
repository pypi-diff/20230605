# Comparing `tmp/etm-dgraham-5.0.3.tar.gz` & `tmp/etm-dgraham-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.0.3.tar", last modified: Sun Jun  4 20:49:09 2023, max compression
+gzip compressed data, was "etm-dgraham-5.0.4.tar", last modified: Mon Jun  5 10:03:11 2023, max compression
```

## Comparing `etm-dgraham-5.0.3.tar` & `etm-dgraham-5.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.990183 etm-dgraham-5.0.3/
--rw-r--r--   0 dag        (501) staff       (20)     2383 2023-06-04 20:44:52.000000 etm-dgraham-5.0.3/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.3/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   129426 2023-06-04 20:49:09.990045 etm-dgraham-5.0.3/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   128514 2023-06-04 16:47:17.000000 etm-dgraham-5.0.3/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.3/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.3/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.982389 etm-dgraham-5.0.3/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.3/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.3/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.3/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.986434 etm-dgraham-5.0.3/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.3/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-03 11:21:41.000000 etm-dgraham-5.0.3/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-04 20:44:52.000000 etm-dgraham-5.0.3/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.3/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.3/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.3/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   277773 2023-06-04 20:44:52.000000 etm-dgraham-5.0.3/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37255 2023-05-23 18:01:39.000000 etm-dgraham-5.0.3/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.3/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)    97060 2023-06-04 20:44:52.000000 etm-dgraham-5.0.3/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.988593 etm-dgraham-5.0.3/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   129426 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.3/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.3/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.3/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.3/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.3/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.3/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-04 20:49:09.990218 etm-dgraham-5.0.3/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.3/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.988688 etm-dgraham-5.0.3/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.3/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.989522 etm-dgraham-5.0.3/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.3/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.3/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.3/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.3/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.253251 etm-dgraham-5.0.4/
+-rw-r--r--   0 dag        (501) staff       (20)     2381 2023-06-05 10:02:58.000000 etm-dgraham-5.0.4/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.4/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   129427 2023-06-05 10:03:11.253104 etm-dgraham-5.0.4/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   128515 2023-06-04 22:28:52.000000 etm-dgraham-5.0.4/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.4/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.4/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.246649 etm-dgraham-5.0.4/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.4/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.4/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.4/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.249471 etm-dgraham-5.0.4/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.4/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-03 11:21:41.000000 etm-dgraham-5.0.4/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-05 10:02:58.000000 etm-dgraham-5.0.4/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.4/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.4/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.4/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   277773 2023-06-04 20:44:52.000000 etm-dgraham-5.0.4/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37255 2023-05-23 18:01:39.000000 etm-dgraham-5.0.4/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.4/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    97128 2023-06-05 10:02:58.000000 etm-dgraham-5.0.4/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.251456 etm-dgraham-5.0.4/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   129427 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.4/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.4/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.4/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.4/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.4/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.4/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-05 10:03:11.253315 etm-dgraham-5.0.4/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.4/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.251554 etm-dgraham-5.0.4/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.4/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.252610 etm-dgraham-5.0.4/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.4/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.4/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.4/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.4/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.0.3/CHANGES.txt` & `etm-dgraham-5.0.4/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-Recent tagged changes as of 2023-06-04T16:44:49.898199-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.0.3) Daniel Graham
+Recent tagged changes as of 2023-06-05T06:02:56.173684-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.0.4) Daniel Graham
+    ea199ac 2023-06-05 06:02:56 -0400
+    Tagged version 5.0.4.
+
+- 13 hours ago (tag: 5.0.3) Daniel Graham
     e0a0d9e 2023-06-04 16:44:49 -0400
     Tagged version 5.0.3.
 
-- 3 hours ago (tag: 5.0.2) Daniel Graham
+- 17 hours ago (tag: 5.0.2) Daniel Graham
     4c5d4bb 2023-06-04 13:26:17 -0400
     Tagged version 5.0.2.
 
-- 4 hours ago (tag: 5.0.1) Daniel Graham
+- 17 hours ago (tag: 5.0.1) Daniel Graham
     b30f0ed 2023-06-04 12:47:15 -0400
     Tagged version 5.0.1.
 
-- 33 hours ago (tag: 5.0.0) Daniel Graham
+- 2 days ago (tag: 5.0.0) Daniel Graham
     7bc8090 2023-06-03 07:21:38 -0400
     Tagged version 5.0.0. Use pendulum periods for f and elements of h
     instead of datetimes.
 
-- 8 days ago (tag: 4.12.9) Daniel Graham
+- 9 days ago (tag: 4.12.9) Daniel Graham
     b8fbc47 2023-05-27 13:45:19 -0400
     Tagged version 4.12.9.
 
-- 9 days ago (tag: 4.12.8) Daniel Graham
+- 10 days ago (tag: 4.12.8) Daniel Graham
     b0316d5 2023-05-26 13:50:15 -0400
     Tagged version 4.12.8.
 
-- 10 days ago (tag: 4.12.7) Daniel Graham
+- 11 days ago (tag: 4.12.7) Daniel Graham
     442ff98 2023-05-25 13:53:52 -0400
     Tagged version 4.12.7.
 
-- 12 days ago (tag: 4.12.6) Daniel Graham
+- 13 days ago (tag: 4.12.6) Daniel Graham
     3da7332 2023-05-23 14:01:37 -0400
     Tagged version 4.12.6.
 
 - 2 weeks ago (tag: 4.12.5) Daniel Graham
     f0c24d8 2023-05-21 15:08:06 -0400
     Tagged version 4.12.5.
 
@@ -53,15 +57,15 @@
     Tagged version 4.12.1. Added display for all-day events to busy
     view
 
 - 3 weeks ago (tag: 4.12.0) Daniel Graham
     ce2ab09 2023-05-13 12:46:39 -0400
     Tagged version 4.12.0. Added engaged view
 
-- 3 weeks ago (tag: 4.11.18) Daniel Graham
+- 4 weeks ago (tag: 4.11.18) Daniel Graham
     cd5482a 2023-05-11 12:20:48 -0400
     Tagged version 4.11.18.
 
 - 4 weeks ago (tag: 4.11.17) Daniel Graham
     8a02515 2023-05-09 10:14:28 -0400
     Tagged version 4.11.17.
 
@@ -72,11 +76,7 @@
 - 5 weeks ago (tag: 4.11.15) Daniel Graham
     96aff42 2023-05-01 14:12:10 -0400
     Tagged version 4.11.15.
 
 - 5 weeks ago (tag: 4.11.14) Daniel Graham
     b437f7b 2023-04-28 08:24:55 -0400
     Tagged version 4.11.14.
-
-- 5 weeks ago (tag: 4.11.13) Daniel Graham
-    4c47483 2023-04-28 08:14:27 -0400
-    Tagged version 4.11.13.
```

### Comparing `etm-dgraham-5.0.3/PKG-INFO` & `etm-dgraham-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.3
+Version: 5.0.4
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -93,15 +93,15 @@
 			- [anniversary substitutions](#anniversary-substitutions)
         -   [archived reminders](#archived-reminders)
         -   [configuration](#configuration)
         -   [data storage](#data-storage)
 
 # Overview {#overview}
 
-*etm* began life in 2013 as *etm-qt* sporting a gui based on *Qt*. The intent was to provide an app supporting GTD (David Allen's Getting Things Done) and exploiting the power of python-dateutil. The name changed to *etmtk* in 2014 when *Tk* replaced *Qt*. Development of *etmtk* continued until 2019 when name changed to *etm-dgraham*, to honor the PyPi naming convention, and the interface changed to a terminal based one based on *promt_toolkit*. Features have changed over the years but the text based interface and basic format of the reminders has changed very little. The goal has always been to be the Swiss Army Knife of tools for managing reminders.
+*etm* began life in 2013 as *etm-qt* sporting a gui based on *Qt*. The intent was to provide an app supporting GTD (David Allen's Getting Things Done) and exploiting the power of python-dateutil. The name changed to *etmtk* in 2014 when *Tk* replaced *Qt*. Development of *etmtk* continued until 2019 when name changed to *etm-dgraham*, to honor the PyPi naming convention, and the interface changed to a terminal based one based on *prompt_toolkit*. Features have changed over the years but the text based interface and basic format of the reminders has changed very little. The goal has always been to be the Swiss Army Knife of tools for managing reminders.
 
 ## Reminders {#reminders}
 
 *etm* offers a simple way to manage your events, tasks and other reminders.
 
 Rather than filling out fields in a form to create or edit reminders, a simple text-based format is used. Each reminder in *etm* begins with a *type character* followed by a brief *summary* of the item and then, perhaps, by one or more *@key value* pairs to specify other attributes of the reminder. Mnemonics are used to make the keys easy to remember, e.g, @s for scheduled datetime, @l for location, @d for description and so forth.
```

### Comparing `etm-dgraham-5.0.3/README.md` & `etm-dgraham-5.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 			- [anniversary substitutions](#anniversary-substitutions)
         -   [archived reminders](#archived-reminders)
         -   [configuration](#configuration)
         -   [data storage](#data-storage)
 
 # Overview {#overview}
 
-*etm* began life in 2013 as *etm-qt* sporting a gui based on *Qt*. The intent was to provide an app supporting GTD (David Allen's Getting Things Done) and exploiting the power of python-dateutil. The name changed to *etmtk* in 2014 when *Tk* replaced *Qt*. Development of *etmtk* continued until 2019 when name changed to *etm-dgraham*, to honor the PyPi naming convention, and the interface changed to a terminal based one based on *promt_toolkit*. Features have changed over the years but the text based interface and basic format of the reminders has changed very little. The goal has always been to be the Swiss Army Knife of tools for managing reminders.
+*etm* began life in 2013 as *etm-qt* sporting a gui based on *Qt*. The intent was to provide an app supporting GTD (David Allen's Getting Things Done) and exploiting the power of python-dateutil. The name changed to *etmtk* in 2014 when *Tk* replaced *Qt*. Development of *etmtk* continued until 2019 when name changed to *etm-dgraham*, to honor the PyPi naming convention, and the interface changed to a terminal based one based on *prompt_toolkit*. Features have changed over the years but the text based interface and basic format of the reminders has changed very little. The goal has always been to be the Swiss Army Knife of tools for managing reminders.
 
 ## Reminders {#reminders}
 
 *etm* offers a simple way to manage your events, tasks and other reminders.
 
 Rather than filling out fields in a form to create or edit reminders, a simple text-based format is used. Each reminder in *etm* begins with a *type character* followed by a brief *summary* of the item and then, perhaps, by one or more *@key value* pairs to specify other attributes of the reminder. Mnemonics are used to make the keys easy to remember, e.g, @s for scheduled datetime, @l for location, @d for description and so forth.
```

### Comparing `etm-dgraham-5.0.3/bump.py` & `etm-dgraham-5.0.4/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/docs/index_konnections.md` & `etm-dgraham-5.0.4/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/docs/index_usedtime.md` & `etm-dgraham-5.0.4/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/docs/multiple_timers.md` & `etm-dgraham-5.0.4/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etm/__main__.py` & `etm-dgraham-5.0.4/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etm/data.py` & `etm-dgraham-5.0.4/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etm/ical.py` & `etm-dgraham-5.0.4/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etm/make_examples.py` & `etm-dgraham-5.0.4/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etm/model.py` & `etm-dgraham-5.0.4/etm/model.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etm/options.py` & `etm-dgraham-5.0.4/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etm/report.py` & `etm-dgraham-5.0.4/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etm/view.py` & `etm-dgraham-5.0.4/etm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -2164,15 +2164,15 @@
         entry = "1 : now"
         due = ""
 
 
     elif repeating:
         already_done = [x.end for x in hsh.get('h', [])]
         need = 2
-        between = [x[0] for x in model.item_instances(hsh, hsh['s'], pendulum.now().replace(hour=0, minute=0, second=0, microsecond=0)) if x[0] not in already_done]
+        between = [x[0] for x in model.item_instances(hsh, model.date_to_datetime(hsh['s']), pendulum.now().replace(hour=0, minute=0, second=0, microsecond=0)) if x[0] not in already_done]
         logger.debug(f"between: {between}")
         values_list = []
         # values.append( (0, format_datetime(between[0][0])[1]) )
         count = -1
         for x in between:
             count += 1
             values_list.append(f"   {count}: {format_datetime(x)[1]}")
@@ -2192,15 +2192,15 @@
         entry = "0 : now"
         due = ""
 
     else:
         need = 1
         between = [hsh.get('s', None)]
         entry =  "now"
-        due = hsh.get('s', "")
+        # due = hsh.get('s', "")
         start = f"\nDue: {format_datetime(hsh['s'])[1]}" if 's' in hsh else ""
 
         text= f"""\
 Selected: {hsh['itemtype']} {hsh['summary']}{start}
 
 Enter <completion datetime>
         """
@@ -2232,14 +2232,15 @@
             due = between[num]
             done = parse_datetime(done_parts[1], z='local')[1]
         elif num_parts == 1:
             done = parse_datetime(done_str, z='local')[1]
             due = between[0] if between[0] else done
 
         done = model.date_to_datetime(done)
+        due = model.date_to_datetime(due)
 
 
         changed = item.finish_item(doc_id, job, done, due)
 
         if changed:
             if doc_id in dataview.itemcache:
                 del dataview.itemcache[doc_id]
```

### Comparing `etm-dgraham-5.0.3/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.0.4/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.3
+Version: 5.0.4
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -93,15 +93,15 @@
 			- [anniversary substitutions](#anniversary-substitutions)
         -   [archived reminders](#archived-reminders)
         -   [configuration](#configuration)
         -   [data storage](#data-storage)
 
 # Overview {#overview}
 
-*etm* began life in 2013 as *etm-qt* sporting a gui based on *Qt*. The intent was to provide an app supporting GTD (David Allen's Getting Things Done) and exploiting the power of python-dateutil. The name changed to *etmtk* in 2014 when *Tk* replaced *Qt*. Development of *etmtk* continued until 2019 when name changed to *etm-dgraham*, to honor the PyPi naming convention, and the interface changed to a terminal based one based on *promt_toolkit*. Features have changed over the years but the text based interface and basic format of the reminders has changed very little. The goal has always been to be the Swiss Army Knife of tools for managing reminders.
+*etm* began life in 2013 as *etm-qt* sporting a gui based on *Qt*. The intent was to provide an app supporting GTD (David Allen's Getting Things Done) and exploiting the power of python-dateutil. The name changed to *etmtk* in 2014 when *Tk* replaced *Qt*. Development of *etmtk* continued until 2019 when name changed to *etm-dgraham*, to honor the PyPi naming convention, and the interface changed to a terminal based one based on *prompt_toolkit*. Features have changed over the years but the text based interface and basic format of the reminders has changed very little. The goal has always been to be the Swiss Army Knife of tools for managing reminders.
 
 ## Reminders {#reminders}
 
 *etm* offers a simple way to manage your events, tasks and other reminders.
 
 Rather than filling out fields in a form to create or edit reminders, a simple text-based format is used. Each reminder in *etm* begins with a *type character* followed by a brief *summary* of the item and then, perhaps, by one or more *@key value* pairs to specify other attributes of the reminder. Mnemonics are used to make the keys easy to remember, e.g, @s for scheduled datetime, @l for location, @d for description and so forth.
```

### Comparing `etm-dgraham-5.0.3/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.0.4/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.0.4/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etmlogo.png` & `etm-dgraham-5.0.4/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etmlogo_small.png` & `etm-dgraham-5.0.4/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/etmview_agenda.png` & `etm-dgraham-5.0.4/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/namedcolors.py` & `etm-dgraham-5.0.4/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/new.png` & `etm-dgraham-5.0.4/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/setup.py` & `etm-dgraham-5.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/test/test_parser.py` & `etm-dgraham-5.0.4/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/utilities/colons_to_slashes.py` & `etm-dgraham-5.0.4/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/utilities/etm_in` & `etm-dgraham-5.0.4/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/utilities/inbasket` & `etm-dgraham-5.0.4/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.3/utilities/open_in_mutt` & `etm-dgraham-5.0.4/utilities/open_in_mutt`

 * *Files identical despite different names*

