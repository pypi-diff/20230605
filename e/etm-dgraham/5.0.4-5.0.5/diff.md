# Comparing `tmp/etm-dgraham-5.0.4.tar.gz` & `tmp/etm-dgraham-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.0.4.tar", last modified: Mon Jun  5 10:03:11 2023, max compression
+gzip compressed data, was "etm-dgraham-5.0.5.tar", last modified: Mon Jun  5 10:28:37 2023, max compression
```

## Comparing `etm-dgraham-5.0.4.tar` & `etm-dgraham-5.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.253251 etm-dgraham-5.0.4/
--rw-r--r--   0 dag        (501) staff       (20)     2381 2023-06-05 10:02:58.000000 etm-dgraham-5.0.4/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.4/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   129427 2023-06-05 10:03:11.253104 etm-dgraham-5.0.4/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   128515 2023-06-04 22:28:52.000000 etm-dgraham-5.0.4/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.4/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.4/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.246649 etm-dgraham-5.0.4/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.4/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.4/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.4/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.249471 etm-dgraham-5.0.4/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.4/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-03 11:21:41.000000 etm-dgraham-5.0.4/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-05 10:02:58.000000 etm-dgraham-5.0.4/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.4/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.4/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.4/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   277773 2023-06-04 20:44:52.000000 etm-dgraham-5.0.4/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37255 2023-05-23 18:01:39.000000 etm-dgraham-5.0.4/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.4/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)    97128 2023-06-05 10:02:58.000000 etm-dgraham-5.0.4/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.251456 etm-dgraham-5.0.4/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   129427 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-05 10:03:11.000000 etm-dgraham-5.0.4/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.4/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.4/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.4/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.4/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.4/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.4/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-05 10:03:11.253315 etm-dgraham-5.0.4/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.4/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.251554 etm-dgraham-5.0.4/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.4/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:03:11.252610 etm-dgraham-5.0.4/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.4/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.4/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.4/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.4/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.138224 etm-dgraham-5.0.5/
+-rw-r--r--   0 dag        (501) staff       (20)     2380 2023-06-05 10:28:27.000000 etm-dgraham-5.0.5/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.5/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   129427 2023-06-05 10:28:37.138067 etm-dgraham-5.0.5/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   128515 2023-06-04 22:28:52.000000 etm-dgraham-5.0.5/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.5/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.5/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.131060 etm-dgraham-5.0.5/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.5/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.5/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.5/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.133967 etm-dgraham-5.0.5/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.5/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-03 11:21:41.000000 etm-dgraham-5.0.5/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-05 10:28:27.000000 etm-dgraham-5.0.5/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.5/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.5/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.5/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   277778 2023-06-05 10:28:27.000000 etm-dgraham-5.0.5/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37255 2023-05-23 18:01:39.000000 etm-dgraham-5.0.5/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.5/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    97115 2023-06-05 10:28:27.000000 etm-dgraham-5.0.5/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.136336 etm-dgraham-5.0.5/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   129427 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-05 10:28:37.000000 etm-dgraham-5.0.5/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.5/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.5/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.5/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.5/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.5/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.5/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-05 10:28:37.138263 etm-dgraham-5.0.5/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.5/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.136448 etm-dgraham-5.0.5/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.5/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 10:28:37.137507 etm-dgraham-5.0.5/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.5/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.5/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.5/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.5/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.0.4/CHANGES.txt` & `etm-dgraham-5.0.5/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-Recent tagged changes as of 2023-06-05T06:02:56.173684-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.0.4) Daniel Graham
+Recent tagged changes as of 2023-06-05T06:28:25.850318-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.0.5) Daniel Graham
+    9273685 2023-06-05 06:28:25 -0400
+    Tagged version 5.0.5.
+
+- 25 minutes ago (tag: 5.0.4) Daniel Graham
     ea199ac 2023-06-05 06:02:56 -0400
     Tagged version 5.0.4.
 
-- 13 hours ago (tag: 5.0.3) Daniel Graham
+- 14 hours ago (tag: 5.0.3) Daniel Graham
     e0a0d9e 2023-06-04 16:44:49 -0400
     Tagged version 5.0.3.
 
 - 17 hours ago (tag: 5.0.2) Daniel Graham
     4c5d4bb 2023-06-04 13:26:17 -0400
     Tagged version 5.0.2.
 
-- 17 hours ago (tag: 5.0.1) Daniel Graham
+- 18 hours ago (tag: 5.0.1) Daniel Graham
     b30f0ed 2023-06-04 12:47:15 -0400
     Tagged version 5.0.1.
 
 - 2 days ago (tag: 5.0.0) Daniel Graham
     7bc8090 2023-06-03 07:21:38 -0400
     Tagged version 5.0.0. Use pendulum periods for f and elements of h
     instead of datetimes.
@@ -72,11 +76,7 @@
 - 5 weeks ago (tag: 4.11.16) Daniel Graham
     b2310ce 2023-05-01 14:43:18 -0400
     Tagged version 4.11.16.
 
 - 5 weeks ago (tag: 4.11.15) Daniel Graham
     96aff42 2023-05-01 14:12:10 -0400
     Tagged version 4.11.15.
-
-- 5 weeks ago (tag: 4.11.14) Daniel Graham
-    b437f7b 2023-04-28 08:24:55 -0400
-    Tagged version 4.11.14.
```

### Comparing `etm-dgraham-5.0.4/PKG-INFO` & `etm-dgraham-5.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.4
+Version: 5.0.5
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.0.4/README.md` & `etm-dgraham-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/bump.py` & `etm-dgraham-5.0.5/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/docs/index_konnections.md` & `etm-dgraham-5.0.5/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/docs/index_usedtime.md` & `etm-dgraham-5.0.5/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/docs/multiple_timers.md` & `etm-dgraham-5.0.5/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etm/__main__.py` & `etm-dgraham-5.0.5/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etm/data.py` & `etm-dgraham-5.0.5/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etm/ical.py` & `etm-dgraham-5.0.5/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etm/make_examples.py` & `etm-dgraham-5.0.5/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etm/model.py` & `etm-dgraham-5.0.5/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2266,15 +2266,15 @@
         self.currcal()
         timer_database.stop()
 
     def set_etmdir(self, etmdir):
         self.etmdir = etmdir
         self.backupdir = os.path.join(self.etmdir, 'backups')
         # need these files for backups
-        self.dbfile = os.path.normpath(os.path.join(etmdir, 'db.json'))
+        self.dbfile = os.path.normpath(os.path.join(etmdir, 'etm.json'))
         self.cfgfile = os.path.normpath(os.path.join(etmdir, 'cfg.yaml'))
         self.settings = settings
         if 'keep_current' in self.settings and self.settings['keep_current']:
             self.currfile = os.path.normpath(os.path.join(etmdir, 'current.txt'))
         else:
             self.currfile = None
         if 'keep_next' in self.settings and self.settings['keep_next']:
@@ -2421,32 +2421,32 @@
         self.konnected = list(set(konnected))
 
 
     def handle_backups(self):
         removefiles = []
         timestamp = pendulum.now('UTC').format("YYYY-MM-DD")
         filelist = os.listdir(self.backupdir)
-        # deal with db.json
+        # deal with etm.json
         dbmtime = os.path.getctime(self.dbfile)
         zipfiles = [x for x in filelist if x.startswith('db')]
         zipfiles.sort(reverse=True)
         if zipfiles:
             lastdbtime = os.path.getctime(os.path.join(self.backupdir, zipfiles[0]))
         else:
             lastdbtime = None
 
         if lastdbtime is None or dbmtime > lastdbtime:
-            backupfile = os.path.join(self.backupdir, f"db-{timestamp}.json")
-            zipfile = os.path.join(self.backupdir, f"db-{timestamp}.zip")
+            backupfile = os.path.join(self.backupdir, f"etm-{timestamp}.json")
+            zipfile = os.path.join(self.backupdir, f"etm-{timestamp}.zip")
             shutil.copy2(self.dbfile, backupfile)
             with ZipFile(zipfile, 'w', compression=ZIP_DEFLATED, compresslevel=6) as zip:
                 zip.write(backupfile, os.path.basename(backupfile))
             os.remove(backupfile)
             logger.info(f"backed up {self.dbfile} to {zipfile}")
-            zipfiles.insert(0, f"db-{timestamp}.zip")
+            zipfiles.insert(0, f"etm-{timestamp}.zip")
             zipfiles.sort(reverse=True)
             removefiles.extend([os.path.join(self.backupdir, x) for x in zipfiles[7:]])
         else:
             logger.info(f"{self.dbfile} unchanged - skipping backup")
 
         # deal with cfg.yaml
         cfgmtime = os.path.getctime(self.cfgfile)
```

### Comparing `etm-dgraham-5.0.4/etm/options.py` & `etm-dgraham-5.0.5/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etm/report.py` & `etm-dgraham-5.0.5/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etm/view.py` & `etm-dgraham-5.0.5/etm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -2402,15 +2402,15 @@
 
 
 @bindings.add('c-t', 'c-t', filter=is_viewing & is_item_view)
 def do_whatever(*event):
     """
     For testing whatever
     """
-    dataview.update_datetimes_to_periods()
+    dataview.handle_backups()
     set_text(dataview.show_active_view())
 
 
 @bindings.add('v', filter=is_viewing)
 def refresh_views(*event):
     """
     Refresh all views to fit current window dimensions and redraw the active view
```

### Comparing `etm-dgraham-5.0.4/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.0.5/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.4
+Version: 5.0.5
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.0.4/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.0.5/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.0.5/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etmlogo.png` & `etm-dgraham-5.0.5/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etmlogo_small.png` & `etm-dgraham-5.0.5/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/etmview_agenda.png` & `etm-dgraham-5.0.5/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/namedcolors.py` & `etm-dgraham-5.0.5/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/new.png` & `etm-dgraham-5.0.5/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/setup.py` & `etm-dgraham-5.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/test/test_parser.py` & `etm-dgraham-5.0.5/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/utilities/colons_to_slashes.py` & `etm-dgraham-5.0.5/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/utilities/etm_in` & `etm-dgraham-5.0.5/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/utilities/inbasket` & `etm-dgraham-5.0.5/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.4/utilities/open_in_mutt` & `etm-dgraham-5.0.5/utilities/open_in_mutt`

 * *Files identical despite different names*

