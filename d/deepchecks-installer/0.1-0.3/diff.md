# Comparing `tmp/deepchecks-installer-0.1.tar.gz` & `tmp/deepchecks-installer-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deepchecks-installer-0.1.tar", last modified: Tue May  9 15:50:18 2023, max compression
+gzip compressed data, was "dist/deepchecks-installer-0.3.tar", last modified: Mon Jun  5 18:43:08 2023, max compression
```

## Comparing `deepchecks-installer-0.1.tar` & `deepchecks-installer-0.3.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 itaygabbay   (501) staff       (20)        0 2023-05-09 15:50:18.055679 deepchecks-installer-0.1/
--rw-r--r--   0 itaygabbay   (501) staff       (20)      192 2023-05-09 15:50:18.055524 deepchecks-installer-0.1/PKG-INFO
--rw-r--r--   0 itaygabbay   (501) staff       (20)      756 2023-05-09 15:49:33.000000 deepchecks-installer-0.1/cli.py
-drwxr-xr-x   0 itaygabbay   (501) staff       (20)        0 2023-05-09 15:50:18.055308 deepchecks-installer-0.1/deepchecks_installer.egg-info/
--rw-r--r--   0 itaygabbay   (501) staff       (20)      192 2023-05-09 15:50:18.000000 deepchecks-installer-0.1/deepchecks_installer.egg-info/PKG-INFO
--rw-r--r--   0 itaygabbay   (501) staff       (20)      281 2023-05-09 15:50:18.000000 deepchecks-installer-0.1/deepchecks_installer.egg-info/SOURCES.txt
--rw-r--r--   0 itaygabbay   (501) staff       (20)        1 2023-05-09 15:50:18.000000 deepchecks-installer-0.1/deepchecks_installer.egg-info/dependency_links.txt
--rw-r--r--   0 itaygabbay   (501) staff       (20)       51 2023-05-09 15:50:18.000000 deepchecks-installer-0.1/deepchecks_installer.egg-info/entry_points.txt
--rw-r--r--   0 itaygabbay   (501) staff       (20)        9 2023-05-09 15:50:18.000000 deepchecks-installer-0.1/deepchecks_installer.egg-info/requires.txt
--rw-r--r--   0 itaygabbay   (501) staff       (20)        4 2023-05-09 15:50:18.000000 deepchecks-installer-0.1/deepchecks_installer.egg-info/top_level.txt
--rw-r--r--   0 itaygabbay   (501) staff       (20)       38 2023-05-09 15:50:18.055735 deepchecks-installer-0.1/setup.cfg
--rw-r--r--   0 itaygabbay   (501) staff       (20)      308 2023-05-09 15:44:48.000000 deepchecks-installer-0.1/setup.py
+drwxr-xr-x   0 itaygabbay   (501) staff       (20)        0 2023-06-05 18:43:08.192499 deepchecks-installer-0.3/
+-rw-r--r--   0 itaygabbay   (501) staff       (20)       44 2023-06-05 18:42:46.000000 deepchecks-installer-0.3/MANIFEST.in
+-rw-r--r--   0 itaygabbay   (501) staff       (20)       62 2023-06-05 18:43:08.192350 deepchecks-installer-0.3/PKG-INFO
+drwxr-xr-x   0 itaygabbay   (501) staff       (20)        0 2023-06-05 18:43:08.191045 deepchecks-installer-0.3/deepchecks_installer/
+-rw-r--r--   0 itaygabbay   (501) staff       (20)        0 2023-06-05 18:13:53.000000 deepchecks-installer-0.3/deepchecks_installer/__init__.py
+-rw-r--r--   0 itaygabbay   (501) staff       (20)      756 2023-06-05 18:13:53.000000 deepchecks-installer-0.3/deepchecks_installer/cli.py
+-rwxr-xr-x   0 itaygabbay   (501) staff       (20)     7440 2023-06-05 18:13:52.000000 deepchecks-installer-0.3/deepchecks_installer/deploy-oss.sh
+drwxr-xr-x   0 itaygabbay   (501) staff       (20)        0 2023-06-05 18:43:08.192159 deepchecks-installer-0.3/deepchecks_installer.egg-info/
+-rw-r--r--   0 itaygabbay   (501) staff       (20)       62 2023-06-05 18:43:08.000000 deepchecks-installer-0.3/deepchecks_installer.egg-info/PKG-INFO
+-rw-r--r--   0 itaygabbay   (501) staff       (20)      382 2023-06-05 18:43:08.000000 deepchecks-installer-0.3/deepchecks_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 itaygabbay   (501) staff       (20)        1 2023-06-05 18:43:08.000000 deepchecks-installer-0.3/deepchecks_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 itaygabbay   (501) staff       (20)       71 2023-06-05 18:43:08.000000 deepchecks-installer-0.3/deepchecks_installer.egg-info/entry_points.txt
+-rw-r--r--   0 itaygabbay   (501) staff       (20)        9 2023-06-05 18:43:08.000000 deepchecks-installer-0.3/deepchecks_installer.egg-info/requires.txt
+-rw-r--r--   0 itaygabbay   (501) staff       (20)       21 2023-06-05 18:43:08.000000 deepchecks-installer-0.3/deepchecks_installer.egg-info/top_level.txt
+-rw-r--r--   0 itaygabbay   (501) staff       (20)       38 2023-06-05 18:43:08.192549 deepchecks-installer-0.3/setup.cfg
+-rw-r--r--   0 itaygabbay   (501) staff       (20)      423 2023-06-05 18:40:19.000000 deepchecks-installer-0.3/setup.py
```

### Comparing `deepchecks-installer-0.1/cli.py` & `deepchecks-installer-0.3/deepchecks_installer/cli.py`

 * *Files identical despite different names*

