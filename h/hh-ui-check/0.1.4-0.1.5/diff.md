# Comparing `tmp/hh_ui_check-0.1.4.tar.gz` & `tmp/hh_ui_check-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hh_ui_check-0.1.4.tar", max compression
+gzip compressed data, was "hh_ui_check-0.1.5.tar", max compression
```

## Comparing `hh_ui_check-0.1.4.tar` & `hh_ui_check-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6273 2023-06-02 05:34:57.983561 hh_ui_check-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-02 03:09:39.424775 hh_ui_check-0.1.4/hh_ui_check/__init__.py
--rwxr-xr-x   0        0        0      640 2023-06-05 06:20:47.720738 hh_ui_check-0.1.4/hh_ui_check/__main__.py
--rw-r--r--   0        0        0     3733 2023-06-05 06:42:28.034026 hh_ui_check-0.1.4/hh_ui_check/diff.py
--rw-r--r--   0        0        0     2112 2023-06-05 06:42:32.130634 hh_ui_check-0.1.4/hh_ui_check/hist_compare.py
--rw-r--r--   0        0        0      503 2023-06-05 06:42:35.999893 hh_ui_check-0.1.4/hh_ui_check/horizen.py
--rw-r--r--   0        0        0      607 2023-06-05 06:42:45.982863 hh_ui_check-0.1.4/hh_ui_check/overlapping.py
--rw-r--r--   0        0        0      471 2023-06-05 06:42:23.464798 hh_ui_check-0.1.4/hh_ui_check/substract.py
--rw-r--r--   0        0        0      441 2023-06-05 06:42:52.447479 hh_ui_check-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6751 1970-01-01 00:00:00.000000 hh_ui_check-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     6273 2023-06-02 05:34:57.983561 hh_ui_check-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 03:09:39.424775 hh_ui_check-0.1.5/hh_ui_check/__init__.py
+-rwxr-xr-x   0        0        0      729 2023-06-05 06:48:39.171611 hh_ui_check-0.1.5/hh_ui_check/__main__.py
+-rw-r--r--   0        0        0     3733 2023-06-05 06:42:28.034026 hh_ui_check-0.1.5/hh_ui_check/diff.py
+-rw-r--r--   0        0        0     2112 2023-06-05 06:42:32.130634 hh_ui_check-0.1.5/hh_ui_check/hist_compare.py
+-rw-r--r--   0        0        0      503 2023-06-05 06:42:35.999893 hh_ui_check-0.1.5/hh_ui_check/horizen.py
+-rw-r--r--   0        0        0      607 2023-06-05 06:42:45.982863 hh_ui_check-0.1.5/hh_ui_check/overlapping.py
+-rw-r--r--   0        0        0      471 2023-06-05 06:42:23.464798 hh_ui_check-0.1.5/hh_ui_check/substract.py
+-rw-r--r--   0        0        0      441 2023-06-05 06:51:05.241298 hh_ui_check-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6751 1970-01-01 00:00:00.000000 hh_ui_check-0.1.5/PKG-INFO
```

### Comparing `hh_ui_check-0.1.4/README.md` & `hh_ui_check-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hh_ui_check-0.1.4/hh_ui_check/diff.py` & `hh_ui_check-0.1.5/hh_ui_check/diff.py`

 * *Files identical despite different names*

### Comparing `hh_ui_check-0.1.4/hh_ui_check/hist_compare.py` & `hh_ui_check-0.1.5/hh_ui_check/hist_compare.py`

 * *Files identical despite different names*

### Comparing `hh_ui_check-0.1.4/hh_ui_check/overlapping.py` & `hh_ui_check-0.1.5/hh_ui_check/overlapping.py`

 * *Files identical despite different names*

### Comparing `hh_ui_check-0.1.4/PKG-INFO` & `hh_ui_check-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hh-ui-check
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: 林明超
 Author-email: mingchao.lin@zeekrlife.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

