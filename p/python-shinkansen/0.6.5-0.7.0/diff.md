# Comparing `tmp/python_shinkansen-0.6.5.tar.gz` & `tmp/python_shinkansen-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_shinkansen-0.6.5.tar", max compression
+gzip compressed data, was "python_shinkansen-0.7.0.tar", max compression
```

## Comparing `python_shinkansen-0.6.5.tar` & `python_shinkansen-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      528 2023-04-05 20:53:12.533555 python_shinkansen-0.6.5/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-05 20:53:21.505843 python_shinkansen-0.6.5/shinkansen/__init__.py
--rw-r--r--   0        0        0     3904 2022-10-25 19:58:12.923345 python_shinkansen-0.6.5/shinkansen/common.py
--rw-r--r--   0        0        0     6478 2022-10-25 20:00:08.857266 python_shinkansen-0.6.5/shinkansen/jws.py
--rw-r--r--   0        0        0    10196 2023-04-05 20:50:03.140433 python_shinkansen-0.6.5/shinkansen/payouts.py
--rw-r--r--   0        0        0     6693 2022-11-14 21:30:40.846241 python_shinkansen-0.6.5/shinkansen/responses.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 python_shinkansen-0.6.5/setup.py
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 python_shinkansen-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      519 2023-06-05 05:46:51.804149 python_shinkansen-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-05 05:46:51.804292 python_shinkansen-0.7.0/shinkansen/__init__.py
+-rw-r--r--   0        0        0     3904 2022-10-25 19:58:12.923345 python_shinkansen-0.7.0/shinkansen/common.py
+-rw-r--r--   0        0        0     6478 2022-10-25 20:00:08.857266 python_shinkansen-0.7.0/shinkansen/jws.py
+-rw-r--r--   0        0        0    12652 2023-06-05 05:39:29.564730 python_shinkansen-0.7.0/shinkansen/payins.py
+-rw-r--r--   0        0        0    10203 2023-06-05 04:29:18.480681 python_shinkansen-0.7.0/shinkansen/payouts.py
+-rw-r--r--   0        0        0     7818 2023-06-05 04:17:49.043149 python_shinkansen-0.7.0/shinkansen/responses.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 python_shinkansen-0.7.0/PKG-INFO
```

### Comparing `python_shinkansen-0.6.5/pyproject.toml` & `python_shinkansen-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "python-shinkansen"
 packages = [
     {include = "shinkansen"}
 ]
-version = "0.6.5"
+version = "0.7.0"
 description = "Python helpers for Shinkansen"
 authors = ["Leonardo Soto M. <leo.soto@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 jwcrypto = "^1.4.0"
-cryptography = ">=37.0.2,<40.0.0"
+cryptography = "^41.0.0"
 requests = "^2.28.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.0"
 black = "^22.6.0"
 pre-commit = "^2.19.0"
 requests-mock = "^1.9.3"
```

### Comparing `python_shinkansen-0.6.5/shinkansen/common.py` & `python_shinkansen-0.7.0/shinkansen/common.py`

 * *Files identical despite different names*

### Comparing `python_shinkansen-0.6.5/shinkansen/jws.py` & `python_shinkansen-0.7.0/shinkansen/jws.py`

 * *Files identical despite different names*

### Comparing `python_shinkansen-0.6.5/shinkansen/payouts.py` & `python_shinkansen-0.7.0/shinkansen/payouts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
-import uuid
 import json
 import os
 import requests
 from typing import Tuple
-from datetime import datetime, timezone
 from .common import *
 from .jws import sign, rsa, x509
-from .responses import PayoutResponse
+from . import responses
 
+PayoutResponse = responses.PayoutResponse  # for backwards compatibility
 PayoutMessageHeader = MessageHeader  # for backwards compatibility
 
 
 class PayoutDebtor:
     """The debtor (origin) of a payout with:
 
     - name: The name of the debtor
```

### Comparing `python_shinkansen-0.6.5/shinkansen/responses.py` & `python_shinkansen-0.7.0/shinkansen/responses.py`

 * *Files 13% similar despite different names*

```diff
@@ -103,14 +103,36 @@
     - shinkansen_transaction_message: Human readable message further explaining the statuse of the transaction
     - response_status: The status of the response. Valid values depend on the transaction type
     - response_message: Human readable message explaining the response status"""
 
     pass  # No extra fields for payout responses
 
 
+@Response.for_transaction_type("payin")
+class PayinResponse(Response):
+    """Payin response with:
+
+    - response_id: The id of the response itself.
+    - transaction_id: The id of the original transaction for this response corresponds to.
+    - shinkansen_transaction_id: The shinkansen assigned id for the original transaction.
+    - shinkansen_transaction_status: The resulting status of the transaction
+    - shinkansen_transaction_message: Human readable message further explaining the statuse of the transaction
+    - response_status: The status of the response. Valid values depend on the transaction type
+    - response_message: Human readable message explaining the response status
+    - expected_settlement_date: When funds are expected to arrive
+    - additional_info: A dict with additional info about the transaction"""
+
+    def __init__(
+        self, **kwargs  # Ignore unexpected fields, so forwards compatibility is easier
+    ):
+        super().__init__(**kwargs)
+        self.expected_settlement_date = kwargs.get("expected_settlement_date")
+        self.additional_info = kwargs.get("additional_info")
+
+
 class ResponseMessage:
     """A response message with:
 
     - header: The header of the message
     - responses: A list of responses contained in the message
     """
```

### Comparing `python_shinkansen-0.6.5/PKG-INFO` & `python_shinkansen-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python-shinkansen
-Version: 0.6.5
+Version: 0.7.0
 Summary: Python helpers for Shinkansen
 Author: Leonardo Soto M.
 Author-email: leo.soto@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cryptography (>=37.0.2,<40.0.0)
+Requires-Dist: cryptography (>=41.0.0,<42.0.0)
 Requires-Dist: jwcrypto (>=1.4.0,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

