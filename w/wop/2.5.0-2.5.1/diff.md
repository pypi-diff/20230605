# Comparing `tmp/wop-2.5.0.tar.gz` & `tmp/wop-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wop-2.5.0.tar", last modified: Tue May 23 08:11:06 2023, max compression
+gzip compressed data, was "D:\rlafage\workspace\WhatsOpt-CLI\dist\.tmp-kffn7p5p\wop-2.5.1.tar", last modified: Mon Jun  5 19:32:20 2023, max compression
```

## Comparing `wop-2.5.0.tar` & `wop-2.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 08:11:06.900708 wop-2.5.0/
--rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.5.0/LICENSE
--rw-rw-rw-   0        0        0      851 2023-05-23 08:11:06.900708 wop-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 08:11:06.900708 wop-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1481 2023-04-14 19:05:22.000000 wop-2.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:11:06.867009 wop-2.5.0/tests/
--rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_convert_utils.py
--rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.5.0/tests/test_mooptimization.py
--rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_push_command.py
--rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_push_utils.py
--rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_upload_utils.py
--rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_utils.py
--rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.5.0/tests/test_whatsopt_client.py
--rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.5.0/tests/test_wop.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:11:06.890628 wop-2.5.0/whatsopt/
--rw-rw-rw-   0        0        0       23 2023-05-23 08:10:57.000000 wop-2.5.0/whatsopt/__init__.py
--rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.5.0/whatsopt/convert_utils.py
--rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.5.0/whatsopt/logging.py
--rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.5.0/whatsopt/mooptimization.py
--rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.5.0/whatsopt/optimization.py
--rw-rw-rw-   0        0        0      232 2023-04-12 16:39:47.000000 wop-2.5.0/whatsopt/publish_utils.py
--rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.5.0/whatsopt/push_command.py
--rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.5.0/whatsopt/push_utils.py
--rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.5.0/whatsopt/show_utils.py
--rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.5.0/whatsopt/upload_utils.py
--rw-rw-rw-   0        0        0     6025 2023-05-15 12:58:25.000000 wop-2.5.0/whatsopt/utils.py
--rw-rw-rw-   0        0        0    40617 2023-05-23 08:10:57.000000 wop-2.5.0/whatsopt/whatsopt_client.py
--rw-rw-rw-   0        0        0    13395 2023-05-23 08:10:57.000000 wop-2.5.0/whatsopt/wop.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:11:06.900708 wop-2.5.0/wop.egg-info/
--rw-rw-rw-   0        0        0      851 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 08:11:06.000000 wop-2.5.0/wop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2019-12-02 13:07:07.000000 wop-2.5.0/wop.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-05 19:32:20.069787 wop-2.5.1/
+-rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.5.1/LICENSE
+-rw-rw-rw-   0        0        0      851 2023-06-05 19:32:20.069787 wop-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 19:32:20.069787 wop-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1481 2023-04-14 19:05:22.000000 wop-2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:32:20.005787 wop-2.5.1/tests/
+-rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_convert_utils.py
+-rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.5.1/tests/test_mooptimization.py
+-rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_push_command.py
+-rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_push_utils.py
+-rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_upload_utils.py
+-rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_utils.py
+-rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.5.1/tests/test_whatsopt_client.py
+-rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_wop.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:32:20.045788 wop-2.5.1/whatsopt/
+-rw-rw-rw-   0        0        0       23 2023-06-05 19:22:39.000000 wop-2.5.1/whatsopt/__init__.py
+-rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.5.1/whatsopt/convert_utils.py
+-rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.5.1/whatsopt/logging.py
+-rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.5.1/whatsopt/mooptimization.py
+-rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.5.1/whatsopt/optimization.py
+-rw-rw-rw-   0        0        0      422 2023-06-05 19:01:08.000000 wop-2.5.1/whatsopt/publish_utils.py
+-rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.5.1/whatsopt/push_command.py
+-rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.5.1/whatsopt/push_utils.py
+-rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.5.1/whatsopt/show_utils.py
+-rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.5.1/whatsopt/upload_utils.py
+-rw-rw-rw-   0        0        0     6025 2023-05-15 12:58:25.000000 wop-2.5.1/whatsopt/utils.py
+-rw-rw-rw-   0        0        0    40617 2023-06-01 14:22:21.000000 wop-2.5.1/whatsopt/whatsopt_client.py
+-rw-rw-rw-   0        0        0    13395 2023-06-05 19:01:08.000000 wop-2.5.1/whatsopt/wop.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:32:20.065788 wop-2.5.1/wop.egg-info/
+-rw-rw-rw-   0        0        0      851 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2019-12-02 13:07:07.000000 wop-2.5.1/wop.egg-info/zip-safe
```

### Comparing `wop-2.5.0/LICENSE` & `wop-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/PKG-INFO` & `wop-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wop
-Version: 2.5.0
+Version: 2.5.1
 Summary: WhatsOpt web application command line client
 Home-page: https://github.com/OneraHub/WhatsOpt-CLI
 Download-URL: https://github.com/OneraHub/WhatsOpt-CLI/releases
 Author: Rémi Lafage
 Author-email: remi.lafage@onera.fr
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wop-2.5.0/README.md` & `wop-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/setup.py` & `wop-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/tests/test_convert_utils.py` & `wop-2.5.1/tests/test_convert_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/tests/test_push_command.py` & `wop-2.5.1/tests/test_push_command.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/tests/test_push_utils.py` & `wop-2.5.1/tests/test_push_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/tests/test_upload_utils.py` & `wop-2.5.1/tests/test_upload_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/tests/test_utils.py` & `wop-2.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/tests/test_wop.py` & `wop-2.5.1/tests/test_wop.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/whatsopt/convert_utils.py` & `wop-2.5.1/whatsopt/convert_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/whatsopt/mooptimization.py` & `wop-2.5.1/whatsopt/mooptimization.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/whatsopt/optimization.py` & `wop-2.5.1/whatsopt/optimization.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/whatsopt/push_command.py` & `wop-2.5.1/whatsopt/push_command.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/whatsopt/push_utils.py` & `wop-2.5.1/whatsopt/push_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/whatsopt/show_utils.py` & `wop-2.5.1/whatsopt/show_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/whatsopt/upload_utils.py` & `wop-2.5.1/whatsopt/upload_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/whatsopt/utils.py` & `wop-2.5.1/whatsopt/utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/whatsopt/whatsopt_client.py` & `wop-2.5.1/whatsopt/whatsopt_client.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.0/whatsopt/wop.py` & `wop-2.5.1/whatsopt/wop.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
             wop.pull_mda_json(analysis_id)
     else:
         if project_id:
             error("Bad option --project-id which works only with option --json enabled")
             exit(-1)
         current_id = get_analysis_id()
         if current_id and analysis_id != current_id:
-            wop.merge_fetch_mda(analysis_id, options)
+            wop.pull_source_mda(analysis_id, options)
         else:
             wop.pull_mda(analysis_id, options)
 
 
 @wop.command()
 @click.option(
     "-n",
```

### Comparing `wop-2.5.0/wop.egg-info/PKG-INFO` & `wop-2.5.1/wop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wop
-Version: 2.5.0
+Version: 2.5.1
 Summary: WhatsOpt web application command line client
 Home-page: https://github.com/OneraHub/WhatsOpt-CLI
 Download-URL: https://github.com/OneraHub/WhatsOpt-CLI/releases
 Author: Rémi Lafage
 Author-email: remi.lafage@onera.fr
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wop-2.5.0/wop.egg-info/SOURCES.txt` & `wop-2.5.1/wop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

