# Comparing `tmp/cashare-0.0.3.tar.gz` & `tmp/cashare-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashare-0.0.3.tar", last modified: Mon Jun  5 11:28:13 2023, max compression
+gzip compressed data, was "cashare-0.0.4.tar", last modified: Mon Jun  5 11:52:56 2023, max compression
```

## Comparing `cashare-0.0.3.tar` & `cashare-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 11:28:13.821217 cashare-0.0.3/
--rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      164 2023-06-05 11:28:13.820219 cashare-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 11:28:13.812241 cashare-0.0.3/cashare/
--rw-rw-rw-   0        0        0        0 2023-03-25 03:03:24.000000 cashare-0.0.3/cashare/__init__.py
--rw-rw-rw-   0        0        0     3269 2023-06-04 12:36:34.000000 cashare-0.0.3/cashare/day_data.py
--rw-rw-rw-   0        0        0       61 2023-06-04 12:22:16.000000 cashare-0.0.3/cashare/dname.py
--rw-rw-rw-   0        0        0     4335 2023-06-05 11:02:22.000000 cashare-0.0.3/cashare/minute_data.py
--rw-rw-rw-   0        0        0      437 2023-06-04 12:32:17.000000 cashare-0.0.3/cashare/stock_list.py
--rw-rw-rw-   0        0        0      430 2023-06-04 12:27:29.000000 cashare-0.0.3/cashare/stock_now.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:28:13.819222 cashare-0.0.3/cashare.egg-info/
--rw-rw-rw-   0        0        0      164 2023-06-05 11:28:13.000000 cashare-0.0.3/cashare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-06-05 11:28:13.000000 cashare-0.0.3/cashare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 11:28:13.000000 cashare-0.0.3/cashare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-05 11:28:13.000000 cashare-0.0.3/cashare.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 11:28:13.000000 cashare-0.0.3/cashare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 11:28:13.821217 cashare-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-06-05 11:27:46.000000 cashare-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:52:56.279824 cashare-0.0.4/
+-rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      164 2023-06-05 11:52:56.278827 cashare-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 11:52:56.270848 cashare-0.0.4/cashare/
+-rw-rw-rw-   0        0        0        0 2023-03-25 03:03:24.000000 cashare-0.0.4/cashare/__init__.py
+-rw-rw-rw-   0        0        0     3269 2023-06-04 12:36:34.000000 cashare-0.0.4/cashare/day_data.py
+-rw-rw-rw-   0        0        0       61 2023-06-04 12:22:16.000000 cashare-0.0.4/cashare/dname.py
+-rw-rw-rw-   0        0        0     4335 2023-06-05 11:02:22.000000 cashare-0.0.4/cashare/minute_data.py
+-rw-rw-rw-   0        0        0      437 2023-06-04 12:32:17.000000 cashare-0.0.4/cashare/stock_list.py
+-rw-rw-rw-   0        0        0      430 2023-06-04 12:27:29.000000 cashare-0.0.4/cashare/stock_now.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:52:56.277829 cashare-0.0.4/cashare.egg-info/
+-rw-rw-rw-   0        0        0      164 2023-06-05 11:52:56.000000 cashare-0.0.4/cashare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-05 11:52:56.000000 cashare-0.0.4/cashare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 11:52:56.000000 cashare-0.0.4/cashare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-05 11:52:56.000000 cashare-0.0.4/cashare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 11:52:56.000000 cashare-0.0.4/cashare.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 11:52:56.279824 cashare-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-06-05 11:52:22.000000 cashare-0.0.4/setup.py
```

### Comparing `cashare-0.0.3/cashare/day_data.py` & `cashare-0.0.4/cashare/day_data.py`

 * *Files identical despite different names*

### Comparing `cashare-0.0.3/cashare/minute_data.py` & `cashare-0.0.4/cashare/minute_data.py`

 * *Files identical despite different names*

