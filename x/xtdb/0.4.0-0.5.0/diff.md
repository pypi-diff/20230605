# Comparing `tmp/xtdb-0.4.0.tar.gz` & `tmp/xtdb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtdb-0.4.0.tar", max compression
+gzip compressed data, was "xtdb-0.5.0.tar", max compression
```

## Comparing `xtdb-0.4.0.tar` & `xtdb-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-05-31 14:49:53.663241 xtdb-0.4.0/LICENSE
--rw-r--r--   0        0        0     4797 2023-05-31 14:49:53.663241 xtdb-0.4.0/README.md
--rw-r--r--   0        0        0     1567 2023-05-31 14:49:53.667241 xtdb-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/__init__.py
--rw-r--r--   0        0        0      211 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/__main__.py
--rw-r--r--   0        0        0     9555 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/datalog.py
--rw-r--r--   0        0        0      120 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/exceptions.py
--rw-r--r--   0        0        0     1711 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/orm.py
--rw-r--r--   0        0        0     6151 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/query.py
--rw-r--r--   0        0        0    11748 2023-05-31 14:49:53.667241 xtdb-0.4.0/xtdb/session.py
--rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 xtdb-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-05 17:21:07.892303 xtdb-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4797 2023-06-05 17:21:07.892303 xtdb-0.5.0/README.md
+-rw-r--r--   0        0        0     1567 2023-06-05 17:21:07.896303 xtdb-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/__main__.py
+-rw-r--r--   0        0        0    14264 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/datalog.py
+-rw-r--r--   0        0        0      120 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/exceptions.py
+-rw-r--r--   0        0        0     1711 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/orm.py
+-rw-r--r--   0        0        0     6391 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/query.py
+-rw-r--r--   0        0        0    12148 2023-06-05 17:21:07.896303 xtdb-0.5.0/xtdb/session.py
+-rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 xtdb-0.5.0/PKG-INFO
```

### Comparing `xtdb-0.4.0/LICENSE` & `xtdb-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xtdb-0.4.0/README.md` & `xtdb-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `xtdb-0.4.0/pyproject.toml` & `xtdb-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtdb"
-version = "0.4.0"
+version = "0.5.0"
 packages = [{ include = "xtdb" }]
 include  = ["xtdb/**"]
 exclude = [
     "**/.idea",
     "**/.git*",
     "**/.*ignore",
     "**/.flake8",
```

### Comparing `xtdb-0.4.0/xtdb/orm.py` & `xtdb-0.5.0/xtdb/orm.py`

 * *Files identical despite different names*

### Comparing `xtdb-0.4.0/xtdb/query.py` & `xtdb-0.5.0/xtdb/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from dataclasses import dataclass
-from typing import Optional, Type, Union
+from typing import List, Literal, Optional, Tuple, Type, Union
 
 from xtdb.datalog import (
     Avg,
     Clause,
     Count,
     CountDistinct,
     Distinct,
     Find,
     Limit,
     Max,
     Median,
     Min,
     Offset,
     Or,
+    OrderBy,
     Rand,
     Sample,
     Stddev,
     Sum,
     Timeout,
     Variance,
     Where,
@@ -51,14 +52,15 @@
     """
 
     result_type: Type[Base]
 
     _find: Optional[Clause] = None
     _where: Optional[Clause] = None
     _limit: Optional[Limit] = None
+    _order_by: Optional[OrderBy] = None
     _offset: Optional[Offset] = None
     _timeout: Optional[Timeout] = None
 
     _preserved_return_type: bool = True
 
     def where(self, object_type: Type[Base], **kwargs) -> "Query":
         for field_name, value in kwargs.items():
@@ -141,14 +143,19 @@
 
     def sample(self, var: Var, N: int) -> "Query":
         self._preserved_return_type = False
         self._find = self._find & Sample(str(var), N)
 
         return self
 
+    def order_by(self, fields: List[Tuple[str, Literal["asc", "desc"]]]) -> "Query":
+        self._order_by = OrderBy(fields)
+
+        return self
+
     def limit(self, limit: int) -> "Query":
         self._limit = Limit(limit)
 
         return self
 
     def offset(self, offset: int) -> "Query":
         self._offset = Offset(offset)
@@ -197,15 +204,15 @@
             Where(object_type.alias(), f"{sc.alias()}/{field_name}", to_alias) for sc in object_type.subclasses()
         ]
         self._where = self._where & Or(clauses)  # type: ignore
 
     def _compile(self, *, separator=" ") -> str:
         where = self._where & Where(self.result_type.alias(), TYPE_FIELD, f'"{self.result_type.alias()}"')
         find = Find(f"(pull {self.result_type.alias()} [*])") if self._find is None else self._find
-        find_where = find & where & self._limit & self._offset & self._timeout
+        find_where = find & where & self._order_by & self._limit & self._offset & self._timeout
 
         return find_where.compile(separator=separator)
 
     def __str__(self) -> str:
         return self._compile()
 
     def __eq__(self, other):
```

### Comparing `xtdb-0.4.0/xtdb/session.py` & `xtdb-0.5.0/xtdb/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime, timezone
 from enum import Enum
 from typing import Any, Dict, List, Literal, Optional, Type, Union
 
 from requests import HTTPError, Response, Session
-from requests.adapters import HTTPAdapter
+from requests.adapters import DEFAULT_POOLBLOCK, DEFAULT_POOLSIZE, HTTPAdapter
 from urllib3 import Retry
 
 from xtdb.datalog import Clause, FindWhere
 from xtdb.exceptions import XTDBException
 from xtdb.orm import Base, Fn
 from xtdb.query import Query
 
@@ -84,20 +84,34 @@
         self.operations.append(operation)
 
     def json(self, **kwargs):
         return json.dumps({"tx-ops": [op.to_list() for op in self.operations]}, **kwargs)
 
 
 class XTDBClient:
-    def __init__(self, base_url: str):
+    def __init__(
+        self,
+        base_url: str,
+        pool_connections: int = DEFAULT_POOLSIZE,
+        pool_maxsize: int = DEFAULT_POOLSIZE,
+        pool_block: bool = DEFAULT_POOLBLOCK,
+        retries: int = 6,
+        backoff_factor: float = 0.5,
+    ):
         self.base_url = base_url
-
         self._session = Session()
-        self._session.mount("http://", HTTPAdapter(max_retries=Retry(total=6, backoff_factor=0.5)))
-        self._session.mount("https://", HTTPAdapter(max_retries=Retry(total=6, backoff_factor=0.5)))
+
+        adapter = HTTPAdapter(
+            pool_connections=pool_connections,
+            pool_maxsize=pool_maxsize,
+            pool_block=pool_block,
+            max_retries=Retry(total=retries, backoff_factor=backoff_factor),
+        )
+        self._session.mount("http://", adapter)
+        self._session.mount("https://", adapter)
         self._session.headers["Accept"] = "application/json"
         self._session.hooks["response"] = self._verify_response
 
         logger.debug("Initialized HTTP session to %s", self.base_url)
 
     @staticmethod
     def _verify_response(response: Response, *args, **kwargs) -> None:
```

### Comparing `xtdb-0.4.0/PKG-INFO` & `xtdb-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtdb
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python ORM for XTDB.
 Home-page: https://github.com/Donnype/xtdb-py
 Author: Donny Peeters
 Author-email: donny.peeters@hotmail.com
 Maintainer: Donny Peeters
 Maintainer-email: donny.peeters@hotmail.com
 Requires-Python: >=3.8,<4.0
```

