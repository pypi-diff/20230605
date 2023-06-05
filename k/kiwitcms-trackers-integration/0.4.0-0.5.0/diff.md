# Comparing `tmp/kiwitcms-trackers-integration-0.4.0.tar.gz` & `tmp/kiwitcms-trackers-integration-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwitcms-trackers-integration-0.4.0.tar", last modified: Thu Feb 16 22:20:35 2023, max compression
+gzip compressed data, was "kiwitcms-trackers-integration-0.5.0.tar", last modified: Mon Jun  5 21:35:10 2023, max compression
```

## Comparing `kiwitcms-trackers-integration-0.4.0.tar` & `kiwitcms-trackers-integration-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-16 22:20:35.813750 kiwitcms-trackers-integration-0.4.0/
--rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2022-08-18 19:28:40.000000 kiwitcms-trackers-integration-0.4.0/LICENSE
--rw-rw-r--   0 senko     (1001) senko     (1001)       79 2022-08-18 19:48:30.000000 kiwitcms-trackers-integration-0.4.0/MANIFEST.in
--rw-r--r--   0 senko     (1001) senko     (1001)     1870 2023-02-16 22:20:35.814750 kiwitcms-trackers-integration-0.4.0/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)     1085 2023-02-16 22:20:11.000000 kiwitcms-trackers-integration-0.4.0/README.rst
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-16 22:20:35.813750 kiwitcms-trackers-integration-0.4.0/kiwitcms_trackers_integration.egg-info/
--rw-r--r--   0 senko     (1001) senko     (1001)     1870 2023-02-16 22:20:35.000000 kiwitcms-trackers-integration-0.4.0/kiwitcms_trackers_integration.egg-info/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)      688 2023-02-16 22:20:35.000000 kiwitcms-trackers-integration-0.4.0/kiwitcms_trackers_integration.egg-info/SOURCES.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-02-16 22:20:35.000000 kiwitcms-trackers-integration-0.4.0/kiwitcms_trackers_integration.egg-info/dependency_links.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       73 2023-02-16 22:20:35.000000 kiwitcms-trackers-integration-0.4.0/kiwitcms_trackers_integration.egg-info/entry_points.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-02-16 22:20:35.000000 kiwitcms-trackers-integration-0.4.0/kiwitcms_trackers_integration.egg-info/not-zip-safe
--rw-r--r--   0 senko     (1001) senko     (1001)       39 2023-02-16 22:20:35.000000 kiwitcms-trackers-integration-0.4.0/kiwitcms_trackers_integration.egg-info/top_level.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-08-18 19:48:30.000000 kiwitcms-trackers-integration-0.4.0/requirements.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      102 2023-02-16 22:20:35.814750 kiwitcms-trackers-integration-0.4.0/setup.cfg
--rw-r--r--   0 senko     (1001) senko     (1001)     1717 2023-02-16 22:20:11.000000 kiwitcms-trackers-integration-0.4.0/setup.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-16 22:20:35.813750 kiwitcms-trackers-integration-0.4.0/tcms_settings_dir/
--rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-08-18 19:48:30.000000 kiwitcms-trackers-integration-0.4.0/tcms_settings_dir/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      597 2022-10-13 08:16:09.000000 kiwitcms-trackers-integration-0.4.0/tcms_settings_dir/trackers_integration.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-16 22:20:35.813750 kiwitcms-trackers-integration-0.4.0/trackers_integration/
--rw-rw-r--   0 senko     (1001) senko     (1001)      133 2022-09-19 20:57:12.000000 kiwitcms-trackers-integration-0.4.0/trackers_integration/__init__.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-16 22:20:35.813750 kiwitcms-trackers-integration-0.4.0/trackers_integration/issuetracker/
--rw-rw-r--   0 senko     (1001) senko     (1001)      381 2022-10-13 08:16:09.000000 kiwitcms-trackers-integration-0.4.0/trackers_integration/issuetracker/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     7441 2023-02-16 21:59:55.000000 kiwitcms-trackers-integration-0.4.0/trackers_integration/issuetracker/mantis.py
--rw-r--r--   0 senko     (1001) senko     (1001)     6965 2023-02-16 21:59:55.000000 kiwitcms-trackers-integration-0.4.0/trackers_integration/issuetracker/openproject.py
--rw-rw-r--   0 senko     (1001) senko     (1001)       16 2022-08-19 20:19:11.000000 kiwitcms-trackers-integration-0.4.0/trackers_integration/menu.py
--rw-rw-r--   0 senko     (1001) senko     (1001)       17 2022-08-19 20:19:11.000000 kiwitcms-trackers-integration-0.4.0/trackers_integration/urls.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-06-05 21:35:10.938888 kiwitcms-trackers-integration-0.5.0/
+-rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2022-08-18 19:28:40.000000 kiwitcms-trackers-integration-0.5.0/LICENSE
+-rw-rw-r--   0 senko     (1001) senko     (1001)       79 2022-08-18 19:48:30.000000 kiwitcms-trackers-integration-0.5.0/MANIFEST.in
+-rw-r--r--   0 senko     (1001) senko     (1001)     2061 2023-06-05 21:35:10.938888 kiwitcms-trackers-integration-0.5.0/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)     1276 2023-06-05 21:34:52.000000 kiwitcms-trackers-integration-0.5.0/README.rst
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-06-05 21:35:10.937888 kiwitcms-trackers-integration-0.5.0/kiwitcms_trackers_integration.egg-info/
+-rw-r--r--   0 senko     (1001) senko     (1001)     2061 2023-06-05 21:35:10.000000 kiwitcms-trackers-integration-0.5.0/kiwitcms_trackers_integration.egg-info/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)      688 2023-06-05 21:35:10.000000 kiwitcms-trackers-integration-0.5.0/kiwitcms_trackers_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-06-05 21:35:10.000000 kiwitcms-trackers-integration-0.5.0/kiwitcms_trackers_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       73 2023-06-05 21:35:10.000000 kiwitcms-trackers-integration-0.5.0/kiwitcms_trackers_integration.egg-info/entry_points.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-06-05 21:35:10.000000 kiwitcms-trackers-integration-0.5.0/kiwitcms_trackers_integration.egg-info/not-zip-safe
+-rw-r--r--   0 senko     (1001) senko     (1001)       39 2023-06-05 21:35:10.000000 kiwitcms-trackers-integration-0.5.0/kiwitcms_trackers_integration.egg-info/top_level.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-08-18 19:48:30.000000 kiwitcms-trackers-integration-0.5.0/requirements.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)      102 2023-06-05 21:35:10.938888 kiwitcms-trackers-integration-0.5.0/setup.cfg
+-rw-r--r--   0 senko     (1001) senko     (1001)     1717 2023-06-05 21:34:01.000000 kiwitcms-trackers-integration-0.5.0/setup.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-06-05 21:35:10.937888 kiwitcms-trackers-integration-0.5.0/tcms_settings_dir/
+-rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-08-18 19:48:30.000000 kiwitcms-trackers-integration-0.5.0/tcms_settings_dir/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      424 2023-05-10 15:35:00.000000 kiwitcms-trackers-integration-0.5.0/tcms_settings_dir/trackers_integration.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-06-05 21:35:10.938888 kiwitcms-trackers-integration-0.5.0/trackers_integration/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      133 2022-09-19 20:57:12.000000 kiwitcms-trackers-integration-0.5.0/trackers_integration/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-06-05 21:35:10.938888 kiwitcms-trackers-integration-0.5.0/trackers_integration/issuetracker/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      381 2022-10-13 08:16:09.000000 kiwitcms-trackers-integration-0.5.0/trackers_integration/issuetracker/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     7441 2023-02-16 21:59:55.000000 kiwitcms-trackers-integration-0.5.0/trackers_integration/issuetracker/mantis.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     6965 2023-02-16 21:59:55.000000 kiwitcms-trackers-integration-0.5.0/trackers_integration/issuetracker/openproject.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)       16 2022-08-19 20:19:11.000000 kiwitcms-trackers-integration-0.5.0/trackers_integration/menu.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)       17 2022-08-19 20:19:11.000000 kiwitcms-trackers-integration-0.5.0/trackers_integration/urls.py
```

### Comparing `kiwitcms-trackers-integration-0.4.0/LICENSE` & `kiwitcms-trackers-integration-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwitcms-trackers-integration-0.4.0/PKG-INFO` & `kiwitcms-trackers-integration-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-trackers-integration
-Version: 0.4.0
+Version: 0.5.0
 Summary: Integration between Kiwi TCMS and various Issue Trackers
 Home-page: https://github.com/kiwitcms/trackers-integration/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Framework :: Django
@@ -39,14 +39,22 @@
 
 This package provides extra integration between Kiwi TCMS and
 various Issue Trackers.
 
 Changelog
 ---------
 
+v0.5.0 (6 Jun 2023)
+~~~~~~~~~~~~~~~~~~~
+
+- Fix typo in module name listed in settings. Closes
+  `Issue #34 <https://github.com/kiwitcms/trackers-integration/issues/34>`_
+  (Stefan Weiberg)
+
+
 v0.4.0 (16 Feb 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Remove IntegrationThread classes due to refactoring in Kiwi TCMS 12.1
 
 
 v0.3.0 (13 Oct 2022)
```

### Comparing `kiwitcms-trackers-integration-0.4.0/README.rst` & `kiwitcms-trackers-integration-0.5.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 
 This package provides extra integration between Kiwi TCMS and
 various Issue Trackers.
 
 Changelog
 ---------
 
+v0.5.0 (6 Jun 2023)
+~~~~~~~~~~~~~~~~~~~
+
+- Fix typo in module name listed in settings. Closes
+  `Issue #34 <https://github.com/kiwitcms/trackers-integration/issues/34>`_
+  (Stefan Weiberg)
+
+
 v0.4.0 (16 Feb 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Remove IntegrationThread classes due to refactoring in Kiwi TCMS 12.1
 
 
 v0.3.0 (13 Oct 2022)
```

### Comparing `kiwitcms-trackers-integration-0.4.0/kiwitcms_trackers_integration.egg-info/PKG-INFO` & `kiwitcms-trackers-integration-0.5.0/kiwitcms_trackers_integration.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-trackers-integration
-Version: 0.4.0
+Version: 0.5.0
 Summary: Integration between Kiwi TCMS and various Issue Trackers
 Home-page: https://github.com/kiwitcms/trackers-integration/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Framework :: Django
@@ -39,14 +39,22 @@
 
 This package provides extra integration between Kiwi TCMS and
 various Issue Trackers.
 
 Changelog
 ---------
 
+v0.5.0 (6 Jun 2023)
+~~~~~~~~~~~~~~~~~~~
+
+- Fix typo in module name listed in settings. Closes
+  `Issue #34 <https://github.com/kiwitcms/trackers-integration/issues/34>`_
+  (Stefan Weiberg)
+
+
 v0.4.0 (16 Feb 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Remove IntegrationThread classes due to refactoring in Kiwi TCMS 12.1
 
 
 v0.3.0 (13 Oct 2022)
```

### Comparing `kiwitcms-trackers-integration-0.4.0/kiwitcms_trackers_integration.egg-info/SOURCES.txt` & `kiwitcms-trackers-integration-0.5.0/kiwitcms_trackers_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiwitcms-trackers-integration-0.4.0/setup.py` & `kiwitcms-trackers-integration-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 continue
             requires.append(line.strip())
         return requires
 
 
 setup(
     name="kiwitcms-trackers-integration",
-    version="0.4.0",
+    version="0.5.0",
     description="Integration between Kiwi TCMS and various Issue Trackers",
     long_description=get_long_description(),
     author="Kiwi TCMS",
     author_email="info@kiwitcms.org",
     url="https://github.com/kiwitcms/trackers-integration/",
     license="GPLv3+",
     install_requires=get_install_requires("requirements.txt"),
```

### Comparing `kiwitcms-trackers-integration-0.4.0/trackers_integration/issuetracker/mantis.py` & `kiwitcms-trackers-integration-0.5.0/trackers_integration/issuetracker/mantis.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-trackers-integration-0.4.0/trackers_integration/issuetracker/openproject.py` & `kiwitcms-trackers-integration-0.5.0/trackers_integration/issuetracker/openproject.py`

 * *Files identical despite different names*

