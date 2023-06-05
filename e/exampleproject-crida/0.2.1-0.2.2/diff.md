# Comparing `tmp/exampleproject_crida-0.2.1.tar.gz` & `tmp/exampleproject_crida-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exampleproject_crida-0.2.1.tar", max compression
+gzip compressed data, was "exampleproject_crida-0.2.2.tar", max compression
```

## Comparing `exampleproject_crida-0.2.1.tar` & `exampleproject_crida-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-05 08:42:00.330913 exampleproject_crida-0.2.1/exampleproject_crida/__init__.py
--rw-r--r--   0        0        0      502 2023-06-05 13:28:27.012013 exampleproject_crida-0.2.1/exampleproject_crida/example_usage.py
--rw-r--r--   0        0        0      311 2023-06-05 14:05:05.476869 exampleproject_crida-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      301 2023-06-05 14:04:37.087593 exampleproject_crida-0.2.1/README_repository.md
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 exampleproject_crida-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 08:42:00.330913 exampleproject_crida-0.2.2/exampleproject_crida/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-05 13:28:27.012013 exampleproject_crida-0.2.2/exampleproject_crida/example_usage.py
+-rw-r--r--   0        0        0      311 2023-06-05 14:09:10.802628 exampleproject_crida-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      302 2023-06-05 14:07:57.148446 exampleproject_crida-0.2.2/README_repository.md
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 exampleproject_crida-0.2.2/PKG-INFO
```

### Comparing `exampleproject_crida-0.2.1/PKG-INFO` & `exampleproject_crida-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: exampleproject-crida
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Sergi Mas-Pujol
 Author-email: smas@e-crida.enaire.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Example of how to publish a repository
 
 Author: Sergi Mas-Pujol \
 Last update: 05/06/2023
 
-# Summary 
+## Summary 
 
 This repository is intended to be used as an example of how to publish a 
 repository in PyPi.org, using Poetry
 
 The project link to this development is called: 
 ``
 exampleproject
```

