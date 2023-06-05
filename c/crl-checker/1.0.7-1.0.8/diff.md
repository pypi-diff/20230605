# Comparing `tmp/crl_checker-1.0.7.tar.gz` & `tmp/crl_checker-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crl_checker-1.0.7.tar", max compression
+gzip compressed data, was "crl_checker-1.0.8.tar", max compression
```

## Comparing `crl_checker-1.0.7.tar` & `crl_checker-1.0.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1096 2023-03-27 18:24:04.323146 crl_checker-1.0.7/LICENSE
--rw-r--r--   0        0        0     1251 2023-03-27 18:24:04.323146 crl_checker-1.0.7/README.md
--rw-r--r--   0        0        0     1897 2023-03-27 18:24:04.323146 crl_checker-1.0.7/crl_checker/__init__.py
--rw-r--r--   0        0        0     1669 2023-03-27 18:24:11.747207 crl_checker-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2632 1970-01-01 00:00:00.000000 crl_checker-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-05 20:23:06.503595 crl_checker-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1251 2023-06-05 20:23:06.503595 crl_checker-1.0.8/README.md
+-rw-r--r--   0        0        0     1897 2023-06-05 20:23:06.503595 crl_checker-1.0.8/crl_checker/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-05 20:23:13.850164 crl_checker-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 crl_checker-1.0.8/PKG-INFO
```

### Comparing `crl_checker-1.0.7/LICENSE` & `crl_checker-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crl_checker-1.0.7/README.md` & `crl_checker-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `crl_checker-1.0.7/crl_checker/__init__.py` & `crl_checker-1.0.8/crl_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `crl_checker-1.0.7/pyproject.toml` & `crl_checker-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crl-checker"
-version = "1.0.7"
+version = "1.0.8"
 description = "Check if certificate is revoked using the x509 CRL extension"
 authors = ["Michal Sadowski <misad90@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
@@ -21,15 +21,15 @@
 repository = "https://github.com/fulder/crl-checker"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/fulder/crl-checker/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-cryptography = ">=39.0.1,<41.0.0"
+cryptography = ">=39.0.1,<42.0.0"
 requests = "^2.28.2"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
```

