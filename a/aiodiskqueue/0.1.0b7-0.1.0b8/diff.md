# Comparing `tmp/aiodiskqueue-0.1.0b7.tar.gz` & `tmp/aiodiskqueue-0.1.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0b7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0b8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0b7.tar` & `aiodiskqueue-0.1.0b8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0b7/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0b7/.github/workflows/main.yml
--rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0b7/.github/workflows/release.yml
--rw-r--r--   0        0        0      136 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b7/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0b7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0b7/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0b7/LICENSE
--rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0b7/Makefile
--rw-r--r--   0        0        0     2752 2023-06-02 22:45:46.710613 aiodiskqueue-0.1.0b7/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0b7/docs/Makefile
--rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0b7/docs/_static/custom.css
--rw-r--r--   0        0        0      267 2023-05-30 15:23:45.131006 aiodiskqueue-0.1.0b7/docs/api.rst
--rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0b7/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0b7/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0b7/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0b7/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b7/examples/basic_usage.py
--rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b7/examples/multiple_consumers.py
--rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b7/examples/single_consumer.py
--rw-r--r--   0        0        0        0 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b7/measurements/__init__.py
--rw-r--r--   0        0        0    51690 2023-06-02 12:59:19.828870 aiodiskqueue-0.1.0b7/measurements/analysis.ipynb
--rw-r--r--   0        0        0      353 2023-06-01 20:15:41.824468 aiodiskqueue-0.1.0b7/measurements/config.toml
--rw-r--r--   0        0        0       17 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b7/measurements/requirements.txt
--rw-r--r--   0        0        0     7078 2023-06-02 22:02:42.961153 aiodiskqueue-0.1.0b7/measurements/run.py
--rw-r--r--   0        0        0     1055 2023-06-02 22:08:23.472217 aiodiskqueue-0.1.0b7/pyproject.toml
--rw-r--r--   0        0        0      277 2023-06-02 22:06:54.677164 aiodiskqueue-0.1.0b7/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0      230 2023-06-02 22:07:35.456683 aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/__init__.py
--rw-r--r--   0        0        0     1097 2023-06-01 19:01:40.067544 aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/base.py
--rw-r--r--   0        0        0     3503 2023-06-02 12:59:11.304713 aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/dbm.py
--rw-r--r--   0        0        0     3353 2023-06-01 19:01:40.071544 aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/simple.py
--rw-r--r--   0        0        0     2198 2023-06-01 19:43:16.734632 aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/sqlite.py
--rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b7/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0     7955 2023-06-02 22:36:25.575233 aiodiskqueue-0.1.0b7/src/aiodiskqueue/queues.py
--rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0b7/src/aiodiskqueue/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0b7/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 19:01:40.071544 aiodiskqueue-0.1.0b7/tests/engines/__init__.py
--rw-r--r--   0        0        0     1910 2023-06-01 19:01:40.071544 aiodiskqueue-0.1.0b7/tests/engines/test_base.py
--rw-r--r--   0        0        0      637 2023-06-02 22:11:12.239200 aiodiskqueue-0.1.0b7/tests/engines/test_dbm.py
--rw-r--r--   0        0        0      714 2023-06-02 22:18:18.574682 aiodiskqueue-0.1.0b7/tests/engines/test_simple.py
--rw-r--r--   0        0        0      405 2023-06-02 22:10:58.483256 aiodiskqueue-0.1.0b7/tests/engines/test_sqlite.py
--rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b7/tests/factories.py
--rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0b7/tests/helpers.py
--rw-r--r--   0        0        0     3495 2023-06-02 22:13:13.350859 aiodiskqueue-0.1.0b7/tests/test_integration.py
--rw-r--r--   0        0        0     8469 2023-06-02 22:33:56.531565 aiodiskqueue-0.1.0b7/tests/test_queues.py
--rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0b7/tests/test_utils.py
--rw-r--r--   0        0        0      459 2023-06-02 22:24:25.114342 aiodiskqueue-0.1.0b7/tox.ini
--rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0b7/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0b8/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0b8/.github/workflows/main.yml
+-rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0b8/.github/workflows/release.yml
+-rw-r--r--   0        0        0      136 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b8/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0b8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0b8/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0b8/LICENSE
+-rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0b8/Makefile
+-rw-r--r--   0        0        0     2899 2023-06-03 13:34:43.520022 aiodiskqueue-0.1.0b8/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0b8/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0b8/docs/_static/custom.css
+-rw-r--r--   0        0        0      267 2023-05-30 15:23:45.131006 aiodiskqueue-0.1.0b8/docs/api.rst
+-rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0b8/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0b8/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0b8/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0b8/examples/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b8/examples/basic_usage.py
+-rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b8/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b8/examples/single_consumer.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b8/measurements/__init__.py
+-rw-r--r--   0        0        0    47249 2023-06-03 13:21:48.237118 aiodiskqueue-0.1.0b8/measurements/analysis.ipynb
+-rw-r--r--   0        0        0      396 2023-06-03 12:47:40.471333 aiodiskqueue-0.1.0b8/measurements/config.toml
+-rw-r--r--   0        0        0       17 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b8/measurements/requirements.txt
+-rw-r--r--   0        0        0     7041 2023-06-03 13:31:27.872382 aiodiskqueue-0.1.0b8/measurements/run.py
+-rw-r--r--   0        0        0     1055 2023-06-02 22:08:23.472217 aiodiskqueue-0.1.0b8/pyproject.toml
+-rw-r--r--   0        0        0      258 2023-06-03 12:38:59.334856 aiodiskqueue-0.1.0b8/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-02 22:07:35.456683 aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/__init__.py
+-rw-r--r--   0        0        0     1067 2023-06-03 13:31:27.656383 aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/base.py
+-rw-r--r--   0        0        0     3473 2023-06-03 13:31:27.732383 aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/dbm.py
+-rw-r--r--   0        0        0     3473 2023-06-03 13:31:27.768383 aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/simple.py
+-rw-r--r--   0        0        0     2168 2023-06-03 13:31:27.824383 aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/sqlite.py
+-rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b8/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0     7937 2023-06-03 13:31:27.696383 aiodiskqueue-0.1.0b8/src/aiodiskqueue/queues.py
+-rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0b8/src/aiodiskqueue/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0b8/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:01:40.071544 aiodiskqueue-0.1.0b8/tests/engines/__init__.py
+-rw-r--r--   0        0        0     1791 2023-06-03 12:32:51.568346 aiodiskqueue-0.1.0b8/tests/engines/test_base.py
+-rw-r--r--   0        0        0      635 2023-06-03 12:32:56.692325 aiodiskqueue-0.1.0b8/tests/engines/test_dbm.py
+-rw-r--r--   0        0        0      714 2023-06-02 22:18:18.574682 aiodiskqueue-0.1.0b8/tests/engines/test_simple.py
+-rw-r--r--   0        0        0      405 2023-06-02 22:10:58.483256 aiodiskqueue-0.1.0b8/tests/engines/test_sqlite.py
+-rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b8/tests/factories.py
+-rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0b8/tests/helpers.py
+-rw-r--r--   0        0        0     3510 2023-06-03 13:31:27.916382 aiodiskqueue-0.1.0b8/tests/test_integration.py
+-rw-r--r--   0        0        0     8469 2023-06-02 22:33:56.531565 aiodiskqueue-0.1.0b8/tests/test_queues.py
+-rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0b8/tests/test_utils.py
+-rw-r--r--   0        0        0      459 2023-06-02 22:24:25.114342 aiodiskqueue-0.1.0b8/tox.ini
+-rw-r--r--   0        0        0     3863 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0b8/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0b7/.github/workflows/main.yml` & `aiodiskqueue-0.1.0b8/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/.github/workflows/release.yml` & `aiodiskqueue-0.1.0b8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/LICENSE` & `aiodiskqueue-0.1.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/README.rst` & `aiodiskqueue-0.1.0b8/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -43,26 +43,36 @@
 
 You can install this library directly from PyPI with the following command:
 
 .. code:: shell
 
     pip install aiodiskqueue
 
-storage Engines
+
+Logging
+-------
+
+The name of the logger for all logging by this library is: ``aiodiskqueue``.
+
+Storage Engines
 ---------------
 
-Support different storage engines. The default engine is `DbmEngine`.
+aiodiskqueue support different storage engines. The default engine is `DbmEngine`.
+
+We measured the throughput for a typical load scenario (5 producers, 1 consumer) with each storage engine:
 
-- `DbmEngine`: Stores the queue in a DBM database. Consistent throughput even at higher volumes and much faster then Sqlite
-- `SqliteEngine`: Stores the queue in a SQlite database. Consistent throughput even at higher volumes and also process safe
-- `PickledList`: Stores the queue in a pickled list. Very fast at smaller volumes, but does not scale well
-- `PickleSequence`: Stores the queue in a list of pickled items. Very fast for putting and at smaller volumes, does not scale well
+|chart|
 
+- `DbmEngine`: Consistent throughput at low and high volumes and about 3 x faster then Sqlite
+- `PickledList`: Very fast at low volumes, but does not scale well
+- `SqliteEngine`: Consistent throughput at low and high volumes. Relatively slow.
 
+The scripts for running the measurements and generating this chart can be found in the measurements folder.
 
+.. |chart| image:: https://imgpile.com/images/9luzXk.png
 .. |release| image:: https://img.shields.io/pypi/v/aiodiskqueue?label=release
    :target: https://pypi.org/project/aiodiskqueue/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodiskqueue
    :target: https://pypi.org/project/aiodiskqueue/
 .. |tests| image:: https://github.com/ErikKalkoken/aiodiskqueue/actions/workflows/main.yml/badge.svg
    :target: https://github.com/ErikKalkoken/aiodiskqueue/actions
 .. |codecov| image:: https://codecov.io/gh/ErikKalkoken/aiodiskqueue/branch/main/graph/badge.svg?token=V43h7hl1Te
```

### Comparing `aiodiskqueue-0.1.0b7/docs/Makefile` & `aiodiskqueue-0.1.0b8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/docs/conf.py` & `aiodiskqueue-0.1.0b8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/docs/make.bat` & `aiodiskqueue-0.1.0b8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0b8/examples/multiple_consumers.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/examples/single_consumer.py` & `aiodiskqueue-0.1.0b8/examples/single_consumer.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/measurements/run.py` & `aiodiskqueue-0.1.0b8/measurements/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import tomllib
 
 import aiodiskqueue
 
 logging.basicConfig(level="INFO", format="%(asctime)s | %(levelname)s | %(message)s")
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("aiodiskqueue")
 
 ITEM_SIZE = 256
 
 
 @dataclass(frozen=True)
 class Measurement:
     FILENAME = "measurements.csv"
@@ -195,20 +195,20 @@
     if max_items:
         item_counts = [
             count for count in config["common"]["items"] if count <= max_items
         ]
     else:
         item_counts = config["common"]["items"]
 
-    for cls_storage_engine in [
-        aiodiskqueue.engines.PickledList,
-        aiodiskqueue.engines.PickleSequence,
-        aiodiskqueue.engines.DbmEngine,
-        # aiodiskqueue.engines.SqliteEngine,
-    ]:
+    engines = [
+        getattr(aiodiskqueue.engines, engine_name)
+        for engine_name in config["common"]["engines"]
+    ]
+
+    for cls_storage_engine in engines:
         for profile in profiles:
             for item_count in item_counts:
                 await runner(
                     data_path,
                     item_count,
                     profile["producers"],
                     profile["consumers"],
```

### Comparing `aiodiskqueue-0.1.0b7/pyproject.toml` & `aiodiskqueue-0.1.0b8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/base.py` & `aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Engines for storing the queues on disk."""
 
 import logging
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, List
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("aiodiskqueue")
 
 
 class _FifoStorageEngine(ABC):
     """Base class for all storage engines implementing a FIFO queue."""
 
     def __init__(self, data_path: Path) -> None:
         self._data_path = data_path
@@ -19,23 +19,23 @@
         """Initialize data file."""
 
     @abstractmethod
     async def fetch_all(self) -> List[Any]:
         """Return all items in data file."""
 
     @abstractmethod
-    async def add_item(self, item: Any, items: List[Any]):
+    async def add_item(self, item: Any):
         """Append one item to end of data file.
 
         Args:
             item: Item to be appended
             items: All items including the one to be appended
         """
 
     @abstractmethod
-    async def remove_item(self, items: List[Any]):
+    async def remove_item(self):
         """Remove item from start of data file.
 
         Args:
             item: Item to be removed
             items: All items not including the one to be removed
         """
```

### Comparing `aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/dbm.py` & `aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/dbm.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 except ImportError:
     has_aiodbm = False
 else:
     has_aiodbm = True
 
 from .base import _FifoStorageEngine
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("aiodiskqueue")
 
 if has_aiodbm:
 
     class DbmEngine(_FifoStorageEngine):
         """A queue storage engine using DBM."""
 
         def __init__(self, data_path: Path) -> None:
@@ -48,15 +48,15 @@
                         item = await self._get_obj(db, item_key)
                         items.append(item)
             except dbm.error:
                 items = []
 
             return items
 
-        async def add_item(self, item: Any, items: List[Any]):
+        async def add_item(self, item: Any):
             async with aiodbm.open(self._data_path_2, "w") as db:
                 tail_id = await self._get_obj(db, self.TAIL_ID_KEY)
                 if tail_id:
                     item_id = tail_id + 1
                     is_first = False
                 else:
                     item_id = 1
@@ -64,15 +64,15 @@
 
                 await self._set_obj(db, self._make_item_key(item_id), item)
                 await self._set_obj(db, self.TAIL_ID_KEY, item_id)
 
                 if is_first:
                     await self._set_obj(db, self.HEAD_ID_KEY, item_id)
 
-        async def remove_item(self, items: List[Any]):
+        async def remove_item(self):
             async with aiodbm.open(self._data_path_2, "w") as db:
                 head_id = await self._get_obj(db, self.HEAD_ID_KEY)
                 tail_id = await self._get_obj(db, self.TAIL_ID_KEY)
                 if not head_id or not tail_id:
                     raise ValueError("Nothing to remove from an empty database")
                 item_key = self._make_item_key(head_id)
                 await db.delete(item_key)
```

### Comparing `aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/simple.py` & `aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, List
 
 import aiofiles
 import aiofiles.os
 
 from .base import _FifoStorageEngine
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("aiodiskqueue")
 
 
 class PickledList(_FifoStorageEngine):
     """This engine stores items as one singular pickled list of items."""
 
     async def initialize(self):
         await self._save_all_items([])
@@ -34,18 +34,22 @@
             logger.exception(
                 "Data file is corrupt and has been backed up: %s", backup_path
             )
             return []
 
         return queue
 
-    async def add_item(self, item: Any, items: List[Any]):
+    async def add_item(self, item: Any):
+        items = await self.fetch_all()
+        items.append(item)
         await self._save_all_items(items)
 
-    async def remove_item(self, items: List[Any]):
+    async def remove_item(self):
+        items = await self.fetch_all()
+        items.pop(0)
         await self._save_all_items(items)
 
     async def _save_all_items(self, items: List[Any]):
         async with aiofiles.open(self._data_path, "wb", buffering=0) as file:
             await file.write(pickle.dumps(items))
         logger.debug("Wrote queue with %d items: %s", len(items), self._data_path)
 
@@ -79,19 +83,21 @@
                         "Data file is corrupt and has been backed up: %s", backup_path
                     )
                     return []
                 else:
                     items.append(item)
         return items
 
-    async def add_item(self, item: Any, items: List[Any]):
+    async def add_item(self, item: Any):
         async with aiofiles.open(self._data_path, "ab", buffering=0) as file:
             await file.write(pickle.dumps(item))
 
-    async def remove_item(self, items: List[Any]):
+    async def remove_item(self):
+        items = await self.fetch_all()
+        items.pop(0)
         await self._save_all_items(items)
 
     async def _save_all_items(self, items: List[Any]):
         with io.BytesIO() as buffer:
             for item in items:
                 pickle.dump(item, buffer)
             buffer.seek(0)
```

### Comparing `aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/sqlite.py` & `aiodiskqueue-0.1.0b8/src/aiodiskqueue/engines/sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 except ImportError:
     has_aiosqlite = False
 else:
     has_aiosqlite = True
 
 from .base import _FifoStorageEngine
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("aiodiskqueue")
 
 if has_aiosqlite:
 
     class SqliteEngine(_FifoStorageEngine):
         """A queue storage engine using Sqlite."""
 
         async def initialize(self):
@@ -47,25 +47,25 @@
                             item = pickle.loads(row[0])
                             items.append(item)
             except sqlite3.OperationalError:
                 pass
 
             return items
 
-        async def add_item(self, item: Any, items: List[Any]):
+        async def add_item(self, item: Any):
             data = pickle.dumps(item)
             async with aiosqlite.connect(self._data_path, isolation_level=None) as db:
                 await db.execute(
                     """
                     INSERT INTO queue (item) VALUES (?);
                     """,
                     (data,),
                 )
 
-        async def remove_item(self, items: List[Any]):
+        async def remove_item(self):
             async with aiosqlite.connect(self._data_path, isolation_level=None) as db:
                 await db.execute(
                     """
                         DELETE FROM queue
                         ORDER BY rowid
                         LIMIT 1;
                     """
```

### Comparing `aiodiskqueue-0.1.0b7/src/aiodiskqueue/queues.py` & `aiodiskqueue-0.1.0b8/src/aiodiskqueue/queues.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, Union
 
 from aiodiskqueue.engines.base import _FifoStorageEngine
 from aiodiskqueue.engines.dbm import DbmEngine
 from aiodiskqueue.exceptions import QueueEmpty, QueueFull
 from aiodiskqueue.utils import NoDirectInstantiation
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("aiodiskqueue")
 
 
 class Queue(metaclass=NoDirectInstantiation):
     """A persistent AsyncIO FIFO queue.
 
     The content of a queue is stored on disk in a data file.
     This file only exists temporarily while there are items in the queue.
@@ -87,15 +87,15 @@
         else raise :class:`.QueueEmpty`.
         """
         async with self._queue_lock:
             if not self._queue:
                 raise QueueEmpty()
 
             item = self._queue.pop(0)
-            await self._storage_engine.remove_item(self._queue)
+            await self._storage_engine.remove_item()
             size = self.qsize()
             self._peak_size = max(self._peak_size, size)
 
         if self._maxsize:
             async with self._has_free_slots:
                 self._has_free_slots.notify()
 
@@ -134,15 +134,15 @@
         Args:
             item: Any Python object that can be pickled
         """
         async with self._queue_lock:
             if self._maxsize and self.qsize() >= self._maxsize:
                 raise QueueFull
             self._queue.append(item)
-            await self._storage_engine.add_item(item, self._queue)
+            await self._storage_engine.add_item(item)
             async with self._tasks_are_finished:
                 self._unfinished_tasks += 1
 
         async with self._has_new_item:
             self._has_new_item.notify()
 
     def qsize(self) -> int:
```

### Comparing `aiodiskqueue-0.1.0b7/src/aiodiskqueue/utils.py` & `aiodiskqueue-0.1.0b8/src/aiodiskqueue/utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/tests/engines/test_base.py` & `aiodiskqueue-0.1.0b8/tests/engines/test_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,47 +10,47 @@
         # then
         self.assertTrue(self.data_path.exists())
 
     async def test_can_add_item_item_to_new_db(self):
         # given
         await self.engine.initialize()
         # when
-        await self.engine.add_item("alpha", ["alpha"])
+        await self.engine.add_item("alpha")
         # then
         items = await self.engine.fetch_all()
         self.assertListEqual(items, ["alpha"])
 
     async def test_can_add_item_multiple_items_to_new_db(self):
         # given
         await self.engine.initialize()
         # when
-        await self.engine.add_item("alpha", ["alpha"])
-        await self.engine.add_item("bravo", ["alpha", "bravo"])
-        await self.engine.add_item("charlie", ["alpha", "bravo", "charlie"])
+        await self.engine.add_item("alpha")
+        await self.engine.add_item("bravo")
+        await self.engine.add_item("charlie")
         # then
         items = await self.engine.fetch_all()
         self.assertListEqual(items, ["alpha", "bravo", "charlie"])
 
     async def test_roundtrip_for_single_item(self):
         # given
         await self.engine.initialize()
         # when
-        await self.engine.add_item("alpha", [])
-        await self.engine.remove_item([])
+        await self.engine.add_item("alpha")
+        await self.engine.remove_item()
         # then
         items = await self.engine.fetch_all()
         self.assertListEqual(items, [])
 
     async def test_roundtrip_for_multiple_item(self):
         # given
         await self.engine.initialize()
         # when
-        await self.engine.add_item("alpha", ["alpha"])
-        await self.engine.add_item("bravo", ["alpha", "bravo"])
-        await self.engine.remove_item(["bravo"])
+        await self.engine.add_item("alpha")
+        await self.engine.add_item("bravo")
+        await self.engine.remove_item()
         # then
         items = await self.engine.fetch_all()
         self.assertListEqual(items, ["bravo"])
 
     async def test_fetch_all_one_missing_file_returns_empty_list(self):
         # when
         items = await self.engine.fetch_all()
```

### Comparing `aiodiskqueue-0.1.0b7/tests/engines/test_dbm.py` & `aiodiskqueue-0.1.0b8/tests/engines/test_dbm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,11 +13,11 @@
         self.engine = DbmEngine(self.data_path)
 
     async def test_raise_error_when_trying_to_remove_item_from_empty_queue(self):
         # given
         await self.engine.initialize()
         # when/then
         with self.assertRaises(ValueError):
-            await self.engine.remove_item([])
+            await self.engine.remove_item()
 
     async def test_can_initialize(self):
         pass  # disable test for now
```

### Comparing `aiodiskqueue-0.1.0b7/tests/engines/test_simple.py` & `aiodiskqueue-0.1.0b8/tests/engines/test_simple.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/tests/factories.py` & `aiodiskqueue-0.1.0b8/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/tests/test_integration.py` & `aiodiskqueue-0.1.0b8/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from unittest import skipIf
 
 import aiodiskqueue
 
 from .factories import ItemFactory
 from .helpers import QueueAsyncioTestCase
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("aiodiskqueue")
 
 
 async def producer(
     source_queue: asyncio.Queue, disk_queue: aiodiskqueue.Queue, num: int
 ):
     logger.debug("Starting producer %d", num)
     while True:
@@ -85,15 +85,15 @@
 
 class TestIntegration(QueueAsyncioTestCase):
     async def test_with_default_storage_engine(self):
         source_items, result_items = await run_test(self.data_path)
         self.assertSetEqual(source_items, result_items)
 
     @skipIf(not hasattr(aiodiskqueue.engines, "PickledList"), "aiofiles not installed")
-    async def test_with_dbm_engine(self):
+    async def test_with_pickled_list_engine(self):
         source_items, result_items = await run_test(
             self.data_path, aiodiskqueue.engines.PickledList
         )
         self.assertSetEqual(source_items, result_items)
 
     @skipIf(
         not hasattr(aiodiskqueue.engines, "PickleSequence"), "aiofiles not installed"
```

### Comparing `aiodiskqueue-0.1.0b7/tests/test_queues.py` & `aiodiskqueue-0.1.0b8/tests/test_queues.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/tests/test_utils.py` & `aiodiskqueue-0.1.0b8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b7/PKG-INFO` & `aiodiskqueue-0.1.0b8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0b7
+Version: 0.1.0b8
 Summary: Persistent queue for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -66,26 +66,36 @@
 
 You can install this library directly from PyPI with the following command:
 
 .. code:: shell
 
     pip install aiodiskqueue
 
-storage Engines
+
+Logging
+-------
+
+The name of the logger for all logging by this library is: ``aiodiskqueue``.
+
+Storage Engines
 ---------------
 
-Support different storage engines. The default engine is `DbmEngine`.
+aiodiskqueue support different storage engines. The default engine is `DbmEngine`.
+
+We measured the throughput for a typical load scenario (5 producers, 1 consumer) with each storage engine:
 
-- `DbmEngine`: Stores the queue in a DBM database. Consistent throughput even at higher volumes and much faster then Sqlite
-- `SqliteEngine`: Stores the queue in a SQlite database. Consistent throughput even at higher volumes and also process safe
-- `PickledList`: Stores the queue in a pickled list. Very fast at smaller volumes, but does not scale well
-- `PickleSequence`: Stores the queue in a list of pickled items. Very fast for putting and at smaller volumes, does not scale well
+|chart|
 
+- `DbmEngine`: Consistent throughput at low and high volumes and about 3 x faster then Sqlite
+- `PickledList`: Very fast at low volumes, but does not scale well
+- `SqliteEngine`: Consistent throughput at low and high volumes. Relatively slow.
 
+The scripts for running the measurements and generating this chart can be found in the measurements folder.
 
+.. |chart| image:: https://imgpile.com/images/9luzXk.png
 .. |release| image:: https://img.shields.io/pypi/v/aiodiskqueue?label=release
    :target: https://pypi.org/project/aiodiskqueue/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodiskqueue
    :target: https://pypi.org/project/aiodiskqueue/
 .. |tests| image:: https://github.com/ErikKalkoken/aiodiskqueue/actions/workflows/main.yml/badge.svg
    :target: https://github.com/ErikKalkoken/aiodiskqueue/actions
 .. |codecov| image:: https://codecov.io/gh/ErikKalkoken/aiodiskqueue/branch/main/graph/badge.svg?token=V43h7hl1Te
```

