# Comparing `tmp/pyjar-0.1.0.tar.gz` & `tmp/pyjar-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjar-0.1.0.tar", max compression
+gzip compressed data, was "pyjar-0.1.1.tar", max compression
```

## Comparing `pyjar-0.1.0.tar` & `pyjar-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-06-05 02:46:06.042658 pyjar-0.1.0/LICENSE
--rw-r--r--   0        0        0      896 2023-06-05 02:46:06.042722 pyjar-0.1.0/README.md
--rw-r--r--   0        0        0      925 2023-06-05 02:46:06.042990 pyjar-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1616 2023-06-05 02:46:06.043126 pyjar-0.1.0/src/pyjar/__init__.py
--rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 pyjar-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-06-05 02:46:06.042658 pyjar-0.1.1/LICENSE
+-rw-r--r--   0        0        0      898 2023-06-05 02:52:51.873959 pyjar-0.1.1/README.md
+-rw-r--r--   0        0        0      925 2023-06-05 02:54:51.053829 pyjar-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1616 2023-06-05 02:46:06.043126 pyjar-0.1.1/src/pyjar/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 02:54:35.598967 pyjar-0.1.1/src/pyjar/py.typed
+-rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 pyjar-0.1.1/PKG-INFO
```

### Comparing `pyjar-0.1.0/LICENSE` & `pyjar-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjar-0.1.0/README.md` & `pyjar-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 the new pickles to be byte-for-byte-identical to the old ones.
 
 ## installation
 
 😄
 
 You can `pip install pyjar` if you really want to, but you can also just
-copy this public-domain code from `src/jar/__init__.py` directly into
+copy this public-domain code from `src/pyjar/__init__.py` directly into
 your own project. You can even give it a name you like better.
 
 
 ## usage
 
 ```
 from pyjar import jar
```

### Comparing `pyjar-0.1.0/pyproject.toml` & `pyjar-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyjar"
-version = "0.1.0"
+version = "0.1.1"
 description = "Move Python things to other modules, mostly for backward-compatibility"
 authors = ["Peter Gaultney <petergaultney@gmail.com>"]
 license = "unlicense"
 readme = "README.md"
 packages = [{include = "pyjar", from="src"}]
 include = ["py.typed"]
```

### Comparing `pyjar-0.1.0/src/pyjar/__init__.py` & `pyjar-0.1.1/src/pyjar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjar-0.1.0/PKG-INFO` & `pyjar-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjar
-Version: 0.1.0
+Version: 0.1.1
 Summary: Move Python things to other modules, mostly for backward-compatibility
 License: Unlicense
 Author: Peter Gaultney
 Author-email: petergaultney@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 the new pickles to be byte-for-byte-identical to the old ones.
 
 ## installation
 
 😄
 
 You can `pip install pyjar` if you really want to, but you can also just
-copy this public-domain code from `src/jar/__init__.py` directly into
+copy this public-domain code from `src/pyjar/__init__.py` directly into
 your own project. You can even give it a name you like better.
 
 
 ## usage
 
 ```
 from pyjar import jar
```

