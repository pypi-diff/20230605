# Comparing `tmp/lnbits_extension-0.10.8.1.tar.gz` & `tmp/lnbits_extension-0.10.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnbits_extension-0.10.8.1.tar", max compression
+gzip compressed data, was "lnbits_extension-0.10.8.2.tar", max compression
```

## Comparing `lnbits_extension-0.10.8.1.tar` & `lnbits_extension-0.10.8.2.tar`

### file list

```diff
@@ -1,4 +1,13 @@
--rw-r--r--   0        0        0        0 2023-06-05 05:31:23.395019 lnbits_extension-0.10.8.1/extension/__init__.py
--rw-r--r--   0        0        0     2659 2023-06-05 06:38:38.770630 lnbits_extension-0.10.8.1/extension/extension.py
--rw-r--r--   0        0        0     2539 2023-06-05 06:47:23.533932 lnbits_extension-0.10.8.1/pyproject.toml
--rw-r--r--   0        0        0     1168 1970-01-01 00:00:00.000000 lnbits_extension-0.10.8.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 05:31:23.395019 lnbits_extension-0.10.8.2/extension/__init__.py
+-rw-r--r--   0        0        0     2659 2023-06-05 06:38:38.770630 lnbits_extension-0.10.8.2/extension/extension.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:04:05.894505 lnbits_extension-0.10.8.2/lib/__init__.py
+-rw-r--r--   0        0        0    15869 2023-06-05 08:04:05.894505 lnbits_extension-0.10.8.2/lib/db.py
+-rw-r--r--   0        0        0     2206 2023-06-05 08:04:05.894505 lnbits_extension-0.10.8.2/lib/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:04:05.904505 lnbits_extension-0.10.8.2/lib/lib/__init__.py
+-rw-r--r--   0        0        0    15869 2023-06-05 08:04:05.904505 lnbits_extension-0.10.8.2/lib/lib/db.py
+-rw-r--r--   0        0        0     2206 2023-06-05 08:04:05.904505 lnbits_extension-0.10.8.2/lib/lib/helpers.py
+-rw-r--r--   0        0        0      538 2023-06-05 08:04:05.904505 lnbits_extension-0.10.8.2/lib/lib/settings.py
+-rw-r--r--   0        0        0     2480 2023-06-05 08:04:05.904505 lnbits_extension-0.10.8.2/lib/pyproject.toml
+-rw-r--r--   0        0        0      538 2023-06-05 08:04:05.891172 lnbits_extension-0.10.8.2/lib/settings.py
+-rw-r--r--   0        0        0     2561 2023-06-05 08:15:20.310808 lnbits_extension-0.10.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1168 1970-01-01 00:00:00.000000 lnbits_extension-0.10.8.2/PKG-INFO
```

### Comparing `lnbits_extension-0.10.8.1/extension/extension.py` & `lnbits_extension-0.10.8.2/extension/extension.py`

 * *Files identical despite different names*

### Comparing `lnbits_extension-0.10.8.1/pyproject.toml` & `lnbits_extension-0.10.8.2/lib/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 [tool.poetry]
-name = "lnbits-extension"
-version = "0.10.8.1"
+name = "lib"
+version = "0.10.8"
 description = "LNbits, free and open-source Lightning wallet and accounts system."
 authors = ["Alan Bits <alan@lnbits.com>"]
-packages = [
-  { include = "./extension"}
-]
 
 [tool.poetry.dependencies]
 python = "^3.10 | ^3.9"
 jinja2 = "3.0.1"
 lnurl = "0.3.6"
 psycopg2-binary = "2.9.1"
 pydantic = "1.10.4"
```

### Comparing `lnbits_extension-0.10.8.1/PKG-INFO` & `lnbits_extension-0.10.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnbits-extension
-Version: 0.10.8.1
+Version: 0.10.8.2
 Summary: LNbits, free and open-source Lightning wallet and accounts system.
 Author: Alan Bits
 Author-email: alan@lnbits.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

