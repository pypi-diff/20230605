# Comparing `tmp/yente-3.4.0.tar.gz` & `tmp/yente-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yente-3.4.0.tar", last modified: Sat May  6 20:02:57 2023, max compression
+gzip compressed data, was "yente-3.4.1.tar", last modified: Mon Jun  5 10:40:40 2023, max compression
```

## Comparing `yente-3.4.0.tar` & `yente-3.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:57.002739 yente-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 20:00:22.000000 yente-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-06 20:00:22.000000 yente-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-06 20:02:57.002739 yente-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-06 20:00:22.000000 yente-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 20:02:57.002739 yente-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-06 20:00:22.000000 yente-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:56.990738 yente-3.4.0/yente/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:22.000000 yente-3.4.0/yente/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-06 20:00:22.000000 yente-3.4.0/yente/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-06 20:00:22.000000 yente-3.4.0/yente/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:56.998739 yente-3.4.0/yente/data/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/freebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-06 20:00:22.000000 yente-3.4.0/yente/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-06 20:00:22.000000 yente-3.4.0/yente/reindex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:56.998739 yente-3.4.0/yente/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-06 20:00:22.000000 yente-3.4.0/yente/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:57.002739 yente-3.4.0/yente/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/match.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-06 20:00:22.000000 yente-3.4.0/yente/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:57.002739 yente-3.4.0/yente/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-06 20:00:22.000000 yente-3.4.0/yente/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-06 20:00:22.000000 yente-3.4.0/yente/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-06 20:00:22.000000 yente-3.4.0/yente/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:56.998739 yente-3.4.0/yente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:00:35.000000 yente-3.4.0/yente.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-05 10:38:38.000000 yente-3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-05 10:38:38.000000 yente-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-05 10:40:40.241286 yente-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-05 10:38:38.000000 yente-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:40:40.241286 yente-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-05 10:38:38.000000 yente-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:38.000000 yente-3.4.1/yente/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-05 10:38:38.000000 yente-3.4.1/yente/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-05 10:38:38.000000 yente-3.4.1/yente/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/freebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-05 10:38:38.000000 yente-3.4.1/yente/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 10:38:38.000000 yente-3.4.1/yente/reindex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-05 10:38:38.000000 yente-3.4.1/yente/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-05 10:38:38.000000 yente-3.4.1/yente/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 10:38:38.000000 yente-3.4.1/yente/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-05 10:38:38.000000 yente-3.4.1/yente/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-05 10:38:38.000000 yente-3.4.1/yente/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:38:46.000000 yente-3.4.1/yente.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/top_level.txt
```

### Comparing `yente-3.4.0/LICENSE` & `yente-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/PKG-INFO` & `yente-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.4.0
+Version: 3.4.1
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.4.0/README.md` & `yente-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/setup.py` & `yente-3.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="yente",
-    version="3.4.0",
+    version="3.4.1",
     url="https://opensanctions.org/docs/api/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="OpenSanctions",
     author_email="info@opensanctions.org",
     packages=find_packages(exclude=["examples", "tests"]),
     namespace_packages=[],
     install_requires=[
-        "followthemoney==3.3.0",
-        "nomenklatura==2.11.0",
-        "asyncstdlib==3.10.7",
+        "followthemoney==3.4.0",
+        "nomenklatura==2.14.0",
+        "asyncstdlib==3.10.8",
         "aiocron==1.8",
         "aiocsv==1.2.4",
         "aiofiles==23.1.0",
-        "types-aiofiles==23.1.0.2",
+        "types-aiofiles==23.1.0.3",
         "aiohttp[speedups]==3.8.4",
-        "elasticsearch[async]==8.7.0",
-        "fastapi==0.95.1",
+        "elasticsearch[async]==8.8.0",
+        "fastapi==0.96.0",
         "uvicorn[standard]==0.22.0",
         "python-multipart==0.0.6",
         "email-validator==2.0.0.post2",
         "structlog==23.1.0",
         "pyicu==2.11",
         "jellyfish==0.11.2",
-        "orjson==3.8.11",
+        "orjson==3.9.0",
         "text-unidecode==1.3",
         "click==8.0.4",
         "normality==2.4.0",
         "languagecodes==1.1.1",
-        "countrynames==1.14.3",
+        "countrynames==1.15.0",
         "fingerprints==1.1.0",
         "pantomime==0.6.0",
     ],
     extras_require={
         "dev": [
             "pip>=10.0.0",
             "bump2version",
```

### Comparing `yente-3.4.0/yente/app.py` & `yente-3.4.1/yente/app.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/cli.py` & `yente-3.4.1/yente/cli.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/data/common.py` & `yente-3.4.1/yente/data/common.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/data/dataset.py` & `yente-3.4.1/yente/data/dataset.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/data/entity.py` & `yente-3.4.1/yente/data/entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,18 +21,16 @@
         self.target: bool = data.get("target", False)
         self._first_seen: Optional[str] = data.get("first_seen", None)
         self._last_seen: Optional[str] = data.get("last_seen", None)
 
     def to_dict(self) -> Dict[str, Any]:
         data = super().to_dict()
         data["target"] = self.target
-        if data.get("first_seen") is None:
-            data["first_seen"] = self._first_seen
-        if data.get("last_seen") is None:
-            data["last_seen"] = self._last_seen
+        data["first_seen"] = self._first_seen or data.get("first_seen")
+        data["last_seen"] = self._last_seen or data.get("last_seen")
         return data
 
     @classmethod
     def from_example(cls, example: "EntityExample") -> "Entity":
         data = {"id": example.id, "schema": example.schema_}
         obj = cls(model, data)
         for prop_name, values in example.properties.items():
```

### Comparing `yente-3.4.0/yente/data/freebase.py` & `yente-3.4.1/yente/data/freebase.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/data/loader.py` & `yente-3.4.1/yente/data/loader.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/data/manifest.py` & `yente-3.4.1/yente/data/manifest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from typing import List, Optional, Dict, Any
 from pydantic import BaseModel
 from nomenklatura.dataset import DataCatalog
 
 from yente import settings
 from yente.data.loader import load_yaml_url
 from yente.data.dataset import Dataset
@@ -50,17 +49,15 @@
         return manifest
 
 
 class Catalog(DataCatalog[Dataset]):
     """A collection of datasets, loaded from a manifest."""
 
     instance: Optional["Catalog"] = None
-    lock = asyncio.Lock()
 
     @classmethod
     async def load(cls) -> "Catalog":
-        async with cls.lock:
-            instance = cls(Dataset, {})
-            manifest = await Manifest.load()
-            for dmf in manifest.datasets:
-                instance.make_dataset(dmf)
-            return instance
+        manifest = await Manifest.load()
+        catalog = cls(Dataset, {})
+        for dmf in manifest.datasets:
+            catalog.make_dataset(dmf)
+        return catalog
```

### Comparing `yente-3.4.0/yente/data/util.py` & `yente-3.4.1/yente/data/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from pathlib import Path
 from jellyfish import soundex, levenshtein_distance
 from functools import lru_cache
 from urllib.parse import urlparse
-from normality import WS
 from prefixdate.precision import Precision
 from contextlib import asynccontextmanager
-from aiohttp import ClientSession, ClientTimeout
+from aiohttp import ClientSession, ClientTimeout, TCPConnector
 from typing import AsyncGenerator, Dict, List, Set, Union
 from followthemoney.types import registry
 from nomenklatura.util import fingerprint_name, name_words
 
 
 def expand_dates(dates: List[str]) -> List[str]:
     """Expand a date into less precise versions of itself."""
@@ -91,9 +90,12 @@
 async def http_session() -> AsyncGenerator[ClientSession, None]:
     timeout = ClientTimeout(
         total=84600,
         connect=None,
         sock_connect=None,
         sock_read=None,
     )
-    async with ClientSession(timeout=timeout, trust_env=True) as client:
+    connector = TCPConnector(limit=10)
+    async with ClientSession(
+        timeout=timeout, trust_env=True, connector=connector
+    ) as client:
         yield client
```

### Comparing `yente-3.4.0/yente/logs.py` & `yente-3.4.1/yente/logs.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/resources/favicon.ico` & `yente-3.4.1/yente/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/routers/admin.py` & `yente-3.4.1/yente/routers/admin.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/routers/match.py` & `yente-3.4.1/yente/routers/match.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/routers/reconcile.py` & `yente-3.4.1/yente/routers/reconcile.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/routers/search.py` & `yente-3.4.1/yente/routers/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/routers/util.py` & `yente-3.4.1/yente/routers/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/scoring.py` & `yente-3.4.1/yente/scoring.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/search/base.py` & `yente-3.4.1/yente/search/base.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/search/indexer.py` & `yente-3.4.1/yente/search/indexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,18 @@
     finally:
         await es.close()
         await close_es()
 
 
 def update_index_threaded(force: bool = False) -> None:
     async def update_in_thread() -> None:
-        await update_index(force=force)
+        try:
+            await update_index(force=force)
+        except (Exception, KeyboardInterrupt) as exc:
+            log.exception("Index update error: %s" % exc)
 
     thread = threading.Thread(
         target=asyncio.run,
         args=(update_in_thread(),),
         daemon=True,
     )
     thread.start()
```

### Comparing `yente-3.4.0/yente/search/mapping.py` & `yente-3.4.1/yente/search/mapping.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/search/nested.py` & `yente-3.4.1/yente/search/nested.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/search/queries.py` & `yente-3.4.1/yente/search/queries.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/search/search.py` & `yente-3.4.1/yente/search/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente/settings.py` & `yente-3.4.1/yente/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def env_str(name: str, default: Optional[str] = None) -> Optional[str]:
     """Ensure the env returns a string even on Windows (#100)."""
     value = stringify(env.get(name))
     return default if value is None else value
 
 
-VERSION = "3.4.0"
+VERSION = "3.4.1"
 AUTHOR = "OpenSanctions"
 HOME_PAGE = "https://www.opensanctions.org"
 EMAIL = "info@opensanctions.org"
 CONTACT = {"name": AUTHOR, "url": HOME_PAGE, "email": EMAIL}
 
 TITLE = env_str("YENTE_TITLE") or "yente"
 DESCRIPTION = """
```

### Comparing `yente-3.4.0/yente/util.py` & `yente-3.4.1/yente/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente.egg-info/PKG-INFO` & `yente-3.4.1/yente.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.4.0
+Version: 3.4.1
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.4.0/yente.egg-info/SOURCES.txt` & `yente-3.4.1/yente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yente-3.4.0/yente.egg-info/requires.txt` & `yente-3.4.1/yente.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-followthemoney==3.3.0
-nomenklatura==2.11.0
-asyncstdlib==3.10.7
+followthemoney==3.4.0
+nomenklatura==2.14.0
+asyncstdlib==3.10.8
 aiocron==1.8
 aiocsv==1.2.4
 aiofiles==23.1.0
-types-aiofiles==23.1.0.2
+types-aiofiles==23.1.0.3
 aiohttp[speedups]==3.8.4
-elasticsearch[async]==8.7.0
-fastapi==0.95.1
+elasticsearch[async]==8.8.0
+fastapi==0.96.0
 uvicorn[standard]==0.22.0
 python-multipart==0.0.6
 email-validator==2.0.0.post2
 structlog==23.1.0
 pyicu==2.11
 jellyfish==0.11.2
-orjson==3.8.11
+orjson==3.9.0
 text-unidecode==1.3
 click==8.0.4
 normality==2.4.0
 languagecodes==1.1.1
-countrynames==1.14.3
+countrynames==1.15.0
 fingerprints==1.1.0
 pantomime==0.6.0
 
 [dev]
 pip>=10.0.0
 bump2version
 wheel>=0.29.0
```

