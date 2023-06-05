# Comparing `tmp/calitp_map_utils-2023.5.31.tar.gz` & `tmp/calitp_map_utils-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_map_utils-2023.5.31.tar", max compression
+gzip compressed data, was "calitp_map_utils-2023.6.5.tar", max compression
```

## Comparing `calitp_map_utils-2023.5.31.tar` & `calitp_map_utils-2023.6.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      944 2023-05-31 19:48:46.649796 calitp_map_utils-2023.5.31/README.md
--rw-r--r--   0        0        0     4963 2023-05-31 19:48:46.650512 calitp_map_utils-2023.5.31/calitp_map_utils/__init__.py
--rw-r--r--   0        0        0       44 2023-05-31 19:48:46.650988 calitp_map_utils-2023.5.31/calitp_map_utils/__main__.py
--rw-r--r--   0        0        0     1441 2023-05-31 19:48:46.651582 calitp_map_utils-2023.5.31/calitp_map_utils/cli.py
--rw-r--r--   0        0        0      646 2023-05-31 19:48:54.451038 calitp_map_utils-2023.5.31/pyproject.toml
--rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.31/PKG-INFO
+-rw-r--r--   0        0        0     2387 2023-06-05 15:29:19.429177 calitp_map_utils-2023.6.5/README.md
+-rw-r--r--   0        0        0     4963 2023-06-05 15:00:29.259233 calitp_map_utils-2023.6.5/calitp_map_utils/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-05 15:00:29.259950 calitp_map_utils-2023.6.5/calitp_map_utils/__main__.py
+-rw-r--r--   0        0        0     1441 2023-06-05 15:00:29.260623 calitp_map_utils-2023.6.5/calitp_map_utils/cli.py
+-rw-r--r--   0        0        0      645 2023-06-05 17:00:47.089758 calitp_map_utils-2023.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 calitp_map_utils-2023.6.5/PKG-INFO
```

### Comparing `calitp_map_utils-2023.5.31/calitp_map_utils/__init__.py` & `calitp_map_utils-2023.6.5/calitp_map_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.5.31/calitp_map_utils/cli.py` & `calitp_map_utils-2023.6.5/calitp_map_utils/cli.py`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.5.31/pyproject.toml` & `calitp_map_utils-2023.6.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp_map_utils"
-version = "2023.5.31"
+version = "2023.6.5"
 description = ""
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.9"
 pyyaml = "^6.0"
```

