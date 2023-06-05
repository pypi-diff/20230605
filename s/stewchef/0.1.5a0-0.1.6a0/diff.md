# Comparing `tmp/stewchef-0.1.5a0.tar.gz` & `tmp/stewchef-0.1.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stewchef-0.1.5a0.tar", max compression
+gzip compressed data, was "stewchef-0.1.6a0.tar", max compression
```

## Comparing `stewchef-0.1.5a0.tar` & `stewchef-0.1.6a0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5808 2023-04-12 10:26:35.957338 stewchef-0.1.5a0/README.md
--rw-r--r--   0        0        0      508 2023-06-05 15:07:46.762019 stewchef-0.1.5a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.5a0/stewchef/__init__.py
--rw-r--r--   0        0        0    13217 2023-06-05 15:06:56.473772 stewchef-0.1.5a0/stewchef/main.py
--rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 stewchef-0.1.5a0/PKG-INFO
+-rw-r--r--   0        0        0     5808 2023-04-12 10:26:35.957338 stewchef-0.1.6a0/README.md
+-rw-r--r--   0        0        0      508 2023-06-05 15:14:25.443979 stewchef-0.1.6a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.6a0/stewchef/__init__.py
+-rw-r--r--   0        0        0    13217 2023-06-05 15:06:56.473772 stewchef-0.1.6a0/stewchef/main.py
+-rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 stewchef-0.1.6a0/PKG-INFO
```

### Comparing `stewchef-0.1.5a0/README.md` & `stewchef-0.1.6a0/README.md`

 * *Files identical despite different names*

### Comparing `stewchef-0.1.5a0/stewchef/main.py` & `stewchef-0.1.6a0/stewchef/main.py`

 * *Files identical despite different names*

### Comparing `stewchef-0.1.5a0/PKG-INFO` & `stewchef-0.1.6a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stewchef
-Version: 0.1.5a0
+Version: 0.1.6a0
 Summary: A MediaWiki API wrapper for RegiSoup
 Author: pengu5055
 Author-email: urbancmarko1@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

