# Comparing `tmp/tbd-calver-versioning-2023.6.5.1.tar.gz` & `tmp/tbd-calver-versioning-2023.6.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tbd-calver-versioning-2023.6.5.1.tar", last modified: Mon Jun  5 13:59:55 2023, max compression
+gzip compressed data, was "tbd-calver-versioning-2023.6.5rc1.tar", last modified: Mon Jun  5 13:58:53 2023, max compression
```

## Comparing `tbd-calver-versioning-2023.6.5.1.tar` & `tbd-calver-versioning-2023.6.5rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:59:55.104657 tbd-calver-versioning-2023.6.5.1/
--rw-r--r--   0 root         (0) root         (0)     4224 2023-06-05 13:59:55.103657 tbd-calver-versioning-2023.6.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3633 2023-05-26 16:53:29.000000 tbd-calver-versioning-2023.6.5.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 13:59:55.104657 tbd-calver-versioning-2023.6.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3641 2023-05-26 18:32:41.000000 tbd-calver-versioning-2023.6.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:59:55.092657 tbd-calver-versioning-2023.6.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:59:55.093657 tbd-calver-versioning-2023.6.5.1/src/bash/
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5.1/src/bash/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:59:55.094657 tbd-calver-versioning-2023.6.5.1/src/bash/bin/
--rw-r--r--   0 root         (0) root         (0)     5763 2023-05-26 18:32:41.000000 tbd-calver-versioning-2023.6.5.1/src/bash/bin/determine_tbd_calver_version_number.sh
--rw-r--r--   0 root         (0) root         (0)      469 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5.1/src/bash/bin/tag_repo_with_version_number.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:59:55.100657 tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/
--rw-r--r--   0 root         (0) root         (0)      326 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/README.md
--rw-r--r--   0 root         (0) root         (0)     1404 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/checkout_git_repo_properly.sh
--rw-r--r--   0 root         (0) root         (0)     1773 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/configure_credential_helper.sh
--rw-r--r--   0 root         (0) root         (0)     1134 2023-05-26 18:32:41.000000 tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/determine_commit_where_branch_created.sh
--rw-r--r--   0 root         (0) root         (0)     3297 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/determine_if_changed_files_match_triggers.sh
--rw-r--r--   0 root         (0) root         (0)      511 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/determine_if_commit_is_merge_commit.sh
--rw-r--r--   0 root         (0) root         (0)     1379 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/get_changed_files_on_branch.sh
--rw-r--r--   0 root         (0) root         (0)      576 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/get_changed_files_since_commit.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:59:55.100657 tbd-calver-versioning-2023.6.5.1/src/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:59:55.102657 tbd-calver-versioning-2023.6.5.1/src/python/tbd_calver_versioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4224 2023-06-05 13:59:55.000000 tbd-calver-versioning-2023.6.5.1/src/python/tbd_calver_versioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      910 2023-06-05 13:59:55.000000 tbd-calver-versioning-2023.6.5.1/src/python/tbd_calver_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 13:59:55.000000 tbd-calver-versioning-2023.6.5.1/src/python/tbd_calver_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-05 13:59:55.000000 tbd-calver-versioning-2023.6.5.1/src/python/tbd_calver_versioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-05 13:59:55.000000 tbd-calver-versioning-2023.6.5.1/src/python/tbd_calver_versioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3083 2023-05-26 16:53:29.000000 tbd-calver-versioning-2023.6.5.1/src/python/tbd_calver_versioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:58:53.951126 tbd-calver-versioning-2023.6.5rc1/
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-06-05 13:58:53.950126 tbd-calver-versioning-2023.6.5rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-05-26 16:53:29.000000 tbd-calver-versioning-2023.6.5rc1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 13:58:53.951126 tbd-calver-versioning-2023.6.5rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-05-26 18:32:41.000000 tbd-calver-versioning-2023.6.5rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:58:53.918127 tbd-calver-versioning-2023.6.5rc1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:58:53.919127 tbd-calver-versioning-2023.6.5rc1/src/bash/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:58:53.926127 tbd-calver-versioning-2023.6.5rc1/src/bash/bin/
+-rw-r--r--   0 root         (0) root         (0)     5763 2023-05-26 18:32:41.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/bin/determine_tbd_calver_version_number.sh
+-rw-r--r--   0 root         (0) root         (0)      469 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/bin/tag_repo_with_version_number.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:58:53.945126 tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/README.md
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/checkout_git_repo_properly.sh
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/configure_credential_helper.sh
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-05-26 18:32:41.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/determine_commit_where_branch_created.sh
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/determine_if_changed_files_match_triggers.sh
+-rw-r--r--   0 root         (0) root         (0)      511 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/determine_if_commit_is_merge_commit.sh
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/get_changed_files_on_branch.sh
+-rw-r--r--   0 root         (0) root         (0)      576 2023-05-26 13:59:12.000000 tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/get_changed_files_since_commit.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:58:53.946126 tbd-calver-versioning-2023.6.5rc1/src/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:58:53.950126 tbd-calver-versioning-2023.6.5rc1/src/python/tbd_calver_versioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-06-05 13:58:53.000000 tbd-calver-versioning-2023.6.5rc1/src/python/tbd_calver_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      910 2023-06-05 13:58:53.000000 tbd-calver-versioning-2023.6.5rc1/src/python/tbd_calver_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 13:58:53.000000 tbd-calver-versioning-2023.6.5rc1/src/python/tbd_calver_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-05 13:58:53.000000 tbd-calver-versioning-2023.6.5rc1/src/python/tbd_calver_versioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-05 13:58:53.000000 tbd-calver-versioning-2023.6.5rc1/src/python/tbd_calver_versioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3083 2023-05-26 16:53:29.000000 tbd-calver-versioning-2023.6.5rc1/src/python/tbd_calver_versioning.py
```

### Comparing `tbd-calver-versioning-2023.6.5.1/PKG-INFO` & `tbd-calver-versioning-2023.6.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbd-calver-versioning
-Version: 2023.6.5.1
+Version: 2023.6.5rc1
 Summary: A set of tools to manage a code repository using trunk based development and CalVer.
 Home-page: https://github.com/taylor-schneider/tbd-calver-versioning
 Author: tschneider
 Author-email: tschneider@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Unix Shell
```

### Comparing `tbd-calver-versioning-2023.6.5.1/README.md` & `tbd-calver-versioning-2023.6.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.6.5.1/setup.py` & `tbd-calver-versioning-2023.6.5rc1/setup.py`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.6.5.1/src/bash/bin/determine_tbd_calver_version_number.sh` & `tbd-calver-versioning-2023.6.5rc1/src/bash/bin/determine_tbd_calver_version_number.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/checkout_git_repo_properly.sh` & `tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/checkout_git_repo_properly.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/configure_credential_helper.sh` & `tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/configure_credential_helper.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/determine_commit_where_branch_created.sh` & `tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/determine_commit_where_branch_created.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/determine_if_changed_files_match_triggers.sh` & `tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/determine_if_changed_files_match_triggers.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/get_changed_files_on_branch.sh` & `tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/get_changed_files_on_branch.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.6.5.1/src/bash/repo_inspection/get_changed_files_since_commit.sh` & `tbd-calver-versioning-2023.6.5rc1/src/bash/repo_inspection/get_changed_files_since_commit.sh`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.6.5.1/src/python/tbd_calver_versioning.egg-info/PKG-INFO` & `tbd-calver-versioning-2023.6.5rc1/src/python/tbd_calver_versioning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbd-calver-versioning
-Version: 2023.6.5.1
+Version: 2023.6.5rc1
 Summary: A set of tools to manage a code repository using trunk based development and CalVer.
 Home-page: https://github.com/taylor-schneider/tbd-calver-versioning
 Author: tschneider
 Author-email: tschneider@live.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Unix Shell
```

### Comparing `tbd-calver-versioning-2023.6.5.1/src/python/tbd_calver_versioning.egg-info/SOURCES.txt` & `tbd-calver-versioning-2023.6.5rc1/src/python/tbd_calver_versioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tbd-calver-versioning-2023.6.5.1/src/python/tbd_calver_versioning.py` & `tbd-calver-versioning-2023.6.5rc1/src/python/tbd_calver_versioning.py`

 * *Files identical despite different names*

