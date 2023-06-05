# Comparing `tmp/airtable_view_fetcher-0.3.2.tar.gz` & `tmp/airtable_view_fetcher-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtable_view_fetcher-0.3.2.tar", last modified: Mon Jun  5 12:59:46 2023, max compression
+gzip compressed data, was "airtable_view_fetcher-0.4.0.tar", last modified: Mon Jun  5 13:17:24 2023, max compression
```

## Comparing `airtable_view_fetcher-0.3.2.tar` & `airtable_view_fetcher-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:46.359633 airtable_view_fetcher-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 12:59:32.000000 airtable_view_fetcher-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-05 12:59:46.359633 airtable_view_fetcher-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-05 12:59:32.000000 airtable_view_fetcher-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:46.359633 airtable_view_fetcher-0.3.2/airtable_view_fetcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:32.000000 airtable_view_fetcher-0.3.2/airtable_view_fetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-05 12:59:32.000000 airtable_view_fetcher-0.3.2/airtable_view_fetcher/fetch_airtable_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:46.359633 airtable_view_fetcher-0.3.2/airtable_view_fetcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-05 12:59:46.000000 airtable_view_fetcher-0.3.2/airtable_view_fetcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-05 12:59:46.000000 airtable_view_fetcher-0.3.2/airtable_view_fetcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:59:46.000000 airtable_view_fetcher-0.3.2/airtable_view_fetcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-05 12:59:46.000000 airtable_view_fetcher-0.3.2/airtable_view_fetcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 12:59:46.000000 airtable_view_fetcher-0.3.2/airtable_view_fetcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 12:59:46.000000 airtable_view_fetcher-0.3.2/airtable_view_fetcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:59:46.359633 airtable_view_fetcher-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-05 12:59:32.000000 airtable_view_fetcher-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:24.681886 airtable_view_fetcher-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 13:17:10.000000 airtable_view_fetcher-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-05 13:17:24.681886 airtable_view_fetcher-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-05 13:17:10.000000 airtable_view_fetcher-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:24.677886 airtable_view_fetcher-0.4.0/airtable_view_fetcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:10.000000 airtable_view_fetcher-0.4.0/airtable_view_fetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-05 13:17:10.000000 airtable_view_fetcher-0.4.0/airtable_view_fetcher/fetch_airtable_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:17:24.681886 airtable_view_fetcher-0.4.0/airtable_view_fetcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-05 13:17:24.000000 airtable_view_fetcher-0.4.0/airtable_view_fetcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-05 13:17:24.000000 airtable_view_fetcher-0.4.0/airtable_view_fetcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:17:24.000000 airtable_view_fetcher-0.4.0/airtable_view_fetcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-05 13:17:24.000000 airtable_view_fetcher-0.4.0/airtable_view_fetcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 13:17:24.000000 airtable_view_fetcher-0.4.0/airtable_view_fetcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:17:24.000000 airtable_view_fetcher-0.4.0/airtable_view_fetcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:17:24.681886 airtable_view_fetcher-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-05 13:17:10.000000 airtable_view_fetcher-0.4.0/setup.py
```

### Comparing `airtable_view_fetcher-0.3.2/LICENSE` & `airtable_view_fetcher-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airtable_view_fetcher-0.3.2/README.md` & `airtable_view_fetcher-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `airtable_view_fetcher-0.3.2/airtable_view_fetcher/fetch_airtable_data.py` & `airtable_view_fetcher-0.4.0/airtable_view_fetcher/fetch_airtable_data.py`

 * *Files identical despite different names*

### Comparing `airtable_view_fetcher-0.3.2/setup.py` & `airtable_view_fetcher-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='airtable_view_fetcher',
-    version='0.3.2',
+    version='0.4.0',
     description='Tool to scrape data from an Airtable shared view',
     url='https://github.com/vartur/airtable_view_fetcher',
     author='Vincent Artur',
     author_email='6145191+vartur@users.noreply.github.com',
     packages=['airtable_view_fetcher'],
     install_requires=[
         'requests',
```

