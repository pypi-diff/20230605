# Comparing `tmp/cnert-0.7.0.tar.gz` & `tmp/cnert-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnert-0.7.0.tar", max compression
+gzip compressed data, was "cnert-0.7.1.tar", max compression
```

## Comparing `cnert-0.7.0.tar` & `cnert-0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.7.0/LICENSE
--rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.7.0/LICENSE.apache2
--rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.7.0/LICENSE.mit
--rw-r--r--   0        0        0     7748 2023-05-10 14:30:59.900805 cnert-0.7.0/README.md
--rw-r--r--   0        0        0     3150 2023-05-31 09:55:13.663823 cnert-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    26246 2023-05-31 09:55:13.694605 cnert-0.7.0/src/cnert/__init__.py
--rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.7.0/src/cnert/py.typed
--rw-r--r--   0        0        0     9512 1970-01-01 00:00:00.000000 cnert-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.7.1/LICENSE
+-rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.7.1/LICENSE.apache2
+-rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.7.1/LICENSE.mit
+-rw-r--r--   0        0        0     7748 2023-05-10 14:30:59.900805 cnert-0.7.1/README.md
+-rw-r--r--   0        0        0     3150 2023-06-05 11:18:50.120161 cnert-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    26231 2023-06-05 11:18:50.151985 cnert-0.7.1/src/cnert/__init__.py
+-rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.7.1/src/cnert/py.typed
+-rw-r--r--   0        0        0     9512 1970-01-01 00:00:00.000000 cnert-0.7.1/PKG-INFO
```

### Comparing `cnert-0.7.0/LICENSE.apache2` & `cnert-0.7.1/LICENSE.apache2`

 * *Files identical despite different names*

### Comparing `cnert-0.7.0/LICENSE.mit` & `cnert-0.7.1/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `cnert-0.7.0/README.md` & `cnert-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cnert-0.7.0/pyproject.toml` & `cnert-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cnert"
-version = "0.7.0"
+version = "0.7.1"
 description = "Cnert is trying to be a simple API for creating TLS Certificates testing purposes."
 authors = ["Maarten <ikmaarten@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maartenq/cnert"
 repository = "https://github.com/maartenq/cnert"
 documentation = "https://cnert.readthedocs.io/en/latest/"
@@ -35,15 +35,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Testing :: Mocking",
     "Topic :: Software Development :: Testing",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-cryptography = "^40.0.0"
+cryptography = "^41.0.0"
 idna = "^3.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 coverage = {extras = ["toml"], version = "^7.1.0"}
 mypy = "^1.0.0"
 pre-commit = "^3.0.4"
```

### Comparing `cnert-0.7.0/src/cnert/__init__.py` & `cnert-0.7.1/src/cnert/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# cnert/__init__.py=serial_number,
+# cnert/__init__.py
 
 from __future__ import annotations  # for Python 3.7-3.9
 
 from datetime import datetime, timedelta
 from ipaddress import ip_address, ip_network
 
 import idna
@@ -12,15 +12,15 @@
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.x509.oid import ExtendedKeyUsageOID, NameOID
 
 """
 Cnert makes TLS private keys, CSRs, private CAs and certificates.
 """
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 __title__ = "Cnert"
 __description__ = (
     "Cnert makes TLS private keys, CSRs, private CAs and certificates."
 )
 __uri__ = "https://github.com/maartenq/cnert"
 __author__ = "Maarten"
 __email__ = "ikmaarten@gmail.com"
```

### Comparing `cnert-0.7.0/PKG-INFO` & `cnert-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnert
-Version: 0.7.0
+Version: 0.7.1
 Summary: Cnert is trying to be a simple API for creating TLS Certificates testing purposes.
 Home-page: https://github.com/maartenq/cnert
 License: MIT
 Keywords: certificate,X.509,TLS,cryptography,testing
 Author: Maarten
 Author-email: ikmaarten@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Mocking
-Requires-Dist: cryptography (>=40.0.0,<41.0.0)
+Requires-Dist: cryptography (>=41.0.0,<42.0.0)
 Requires-Dist: idna (>=3.3,<4.0)
 Project-URL: Documentation, https://cnert.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/maartenq/cnert
 Description-Content-Type: text/markdown
 
 # cnert
```

