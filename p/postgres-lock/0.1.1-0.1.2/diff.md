# Comparing `tmp/postgres_lock-0.1.1.tar.gz` & `tmp/postgres_lock-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgres_lock-0.1.1.tar", max compression
+gzip compressed data, was "postgres_lock-0.1.2.tar", max compression
```

## Comparing `postgres_lock-0.1.1.tar` & `postgres_lock-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1496 2023-05-30 13:15:35.574393 postgres_lock-0.1.1/LICENSE
--rw-r--r--   0        0        0     3015 2023-05-31 23:45:03.742762 postgres_lock-0.1.1/README.md
--rw-r--r--   0        0        0      107 2023-05-31 14:20:25.432460 postgres_lock-0.1.1/postgres_lock/__init__.py
--rw-r--r--   0        0        0     1708 2023-05-31 15:47:45.539175 postgres_lock-0.1.1/postgres_lock/asyncpg.py
--rw-r--r--   0        0        0      354 2023-05-31 22:29:05.371623 postgres_lock-0.1.1/postgres_lock/errors.py
--rw-r--r--   0        0        0     8570 2023-05-31 23:33:28.102639 postgres_lock-0.1.1/postgres_lock/lock.py
--rw-r--r--   0        0        0     1796 2023-05-31 14:47:42.602709 postgres_lock-0.1.1/postgres_lock/psycopg2.py
--rw-r--r--   0        0        0     2198 2023-05-31 14:47:42.602709 postgres_lock-0.1.1/postgres_lock/psycopg3.py
--rw-r--r--   0        0        0     2094 2023-05-31 20:08:55.316117 postgres_lock-0.1.1/postgres_lock/sqlalchemy.py
--rw-r--r--   0        0        0      542 2023-05-31 23:46:13.084356 postgres_lock-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3804 1970-01-01 00:00:00.000000 postgres_lock-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-05-30 13:15:35.574393 postgres_lock-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3755 2023-06-05 18:56:38.234398 postgres_lock-0.1.2/README.md
+-rw-r--r--   0        0        0      341 2023-06-02 20:16:52.298972 postgres_lock-0.1.2/postgres_lock/__init__.py
+-rw-r--r--   0        0        0     2443 2023-06-05 17:59:32.127064 postgres_lock-0.1.2/postgres_lock/asyncpg.py
+-rw-r--r--   0        0        0      589 2023-06-05 16:57:57.287722 postgres_lock-0.1.2/postgres_lock/errors.py
+-rw-r--r--   0        0        0     9627 2023-06-05 18:26:09.323824 postgres_lock-0.1.2/postgres_lock/lock.py
+-rw-r--r--   0        0        0     2575 2023-06-05 18:18:16.609045 postgres_lock-0.1.2/postgres_lock/psycopg2.py
+-rw-r--r--   0        0        0     2993 2023-06-05 18:20:32.444223 postgres_lock-0.1.2/postgres_lock/psycopg3.py
+-rw-r--r--   0        0        0     2813 2023-06-05 18:12:25.912861 postgres_lock-0.1.2/postgres_lock/sqlalchemy.py
+-rw-r--r--   0        0        0      542 2023-06-05 18:57:01.854977 postgres_lock-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 postgres_lock-0.1.2/PKG-INFO
```

### Comparing `postgres_lock-0.1.1/LICENSE` & `postgres_lock-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.1/README.md` & `postgres_lock-0.1.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -28,23 +28,25 @@
 - Postgres table locks aren't sufficient for your use-case
 - Postgres row locks don't work on `INSERT`
 - You want to prevent race conditions between `INSERT` and `UPDATE` on the same primary key
 - None of the aforementioned details fit your use-case, but you have Postgres installed and need to prevent race conditions in a distributed system
 
 ### Default operation
 
-By default `postgres-lock` will use `session` lock scope in `blocking` mode. The `session` lock scope
-means only a single database connection can acquire the lock at a time.
+By default `postgres-lock` will use `session` lock scope in `blocking` mode with
+`rollback_on_error` enabled. The `session` lock scope means only a single database connection can
+acquire the lock at a time.
 
 ### Usage
 
 All work revolves around the `Lock` class.
 
 The easiest way to use `Lock` is with `with` or `async with` statements. The lock will be
-released automatically.
+released automatically. If `rollback_on_error` is enabled (default), rollbacks are automatically
+handled prior to release.
 
 _Using `with` and `async with` implies blocking mode._
 
 ```python
 from postgres_lock import Lock
 
 # setup connection
@@ -70,15 +72,23 @@
 
 try:
     # acquire lock
     lock.acquire()
 
     print("Acquired lock!")
 
-    # do something here
+    try:
+        # do something here
+        pass
+
+    except Exception as exc:
+        # handle_error() will rollback the transaction by default
+        lock.handle_error(exc)
+
+        raise exc
 finally:
     # release lock (this is safe to run even if the lock has not been acquired)
     lock.release()
 ```
 
 ### Asynchronous usage (without `async with`)
 
@@ -93,15 +103,23 @@
 
 try:
     # acquire lock
     await lock.acquire_async()
 
     print("Acquired lock!")
 
-    # do something here
+    try:
+        # do something here
+        pass
+
+    except Exception as exc:
+        # handle_error_async() will rollback the transaction by default
+        await lock.handle_error_async(exc)
+
+        raise exc
 finally:
     # release lock (this is safe to run even if the lock has not been acquired)
     await lock.release_async()
 ```
 
 ### Non-blocking mode (supports async as well)
 
@@ -110,41 +128,55 @@
 
 # setup connection
 conn = ...
 
 # create lock
 lock = Lock(conn, "shared-identifier")
 
-try:
-    # acquire lock
-    if lock.acquire(block=False):
-        print("Acquired lock!")
-
-        # do something here
+# acquire lock
+if lock.acquire(block=False):
+    # do something here
+    pass
 
-    else:
-        print("Could not acquire lock!")
+else:
+    # could not acquire lock
+    pass
 
-finally:
-    # release lock (this is safe to run even if the lock has not been acquired)
-    lock.release()
+# release lock (this is safe to run even if the lock has not been acquired)
+lock.release()
 ```
 
 ### Specify the database interface manually
 
 ```python
 from postgres_lock import Lock
 
 # setup connection
 conn = ...
 
 # create and use lock
-with Lock(conn, "shared-identifier", interface="asyncpg"):
-    print("Acquired lock!")
+lock = Lock(conn, "shared-identifier", interface="asyncpg")
 
-    # do something here
+# do things with the lock
+```
+
+### Handle rollbacks manually
+
+```python
+from postgres_lock import Lock
+
+# setup connection
+conn = ...
+
+# create and use lock
+lock = Lock(conn, "shared-identifier", rollback_on_error=False)
+
+# do things with the lock
 ```
 
 ### Changelog
 
+- **0.1.2**
+  - Add Lock.rollback_on_error (default true)
+  - Add Lock.handle_error() & Lock.handle_error_async()
 - **0.1.1**
   - Key can be str or int
```

### Comparing `postgres_lock-0.1.1/postgres_lock/asyncpg.py` & `postgres_lock-0.1.2/postgres_lock/asyncpg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# --------------------------------------------------------------------------------------------------
+# Copyright (c) 2023 Sean Kerr
+# --------------------------------------------------------------------------------------------------
+
 """
 Lock support for asyncpg database interface.
 """
 
 from .lock import Lock
 
 
@@ -37,14 +41,37 @@
 
     result = await lock.conn.fetchval(f"SELECT pg_catalog.{lock_func}({lock.lock_id})")
 
     # lock function returns True/False in unblocking mode, and always None in blocking mode
     return False if result is False else True
 
 
+def handle_error(lock: Lock, exc: BaseException) -> None:
+    """
+    Handle an error.
+
+    Parameters:
+        exc (Exception): Exception.
+    """
+    raise NotImplementedError("ascynpg interface does not support handle_error()")
+
+
+async def handle_error_async(lock: Lock, exc: BaseException) -> None:
+    """
+    Handle an error asynchronously.
+
+    Parameters:
+        exc (Exception): Exception.
+    """
+    if not lock.rollback_on_error:
+        return
+
+    await lock.conn.execute("ROLLBACK")
+
+
 def release(lock: Lock) -> bool:
     """
     This function is not implemented.
 
     Parameters:
         lock (Lock): Lock.
```

### Comparing `postgres_lock-0.1.1/postgres_lock/lock.py` & `postgres_lock-0.1.2/postgres_lock/lock.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# --------------------------------------------------------------------------------------------------
+# Copyright (c) 2023 Sean Kerr
+# --------------------------------------------------------------------------------------------------
+
 from importlib import import_module
 
 from types import ModuleType
 from types import TracebackType
 
 from typing import Any
 from typing import Literal
@@ -43,14 +47,15 @@
     Sharing (locks can or cannot be reacquired from the same scope)
     """
 
     conn: Any
     interface: str
     key: str | int
     lock_id: int
+    rollback_on_error: bool
     scope: str
     shared: bool
 
     blocking_lock_func: str
     nonblocking_lock_func: str
     unlock_func: str
 
@@ -61,34 +66,37 @@
         interface: Literal[
             "auto",
             "asyncpg",
             "psycopg2",
             "psycopg3",
             "sqlalchemy",
         ] = "auto",
+        rollback_on_error: bool = True,
         scope: Literal["session", "transaction"] = "session",
         shared: bool = False,
     ):
         """
         Create a new Lock instance.
 
         Parameters:
             conn (object): Database connection.
             key (str|int): Unique lock key.
             interface (str): Database interface.
+            rollback_on_error (bool): Rollback if an error occurs while in a `with` statement.
             scope (str): Lock scope.
             shared (bool): Use a shared lock.
         """
         self.conn = conn
         self.interface = interface
         self.impl = self._load_impl()
         self.key = key
         self.lock_id = str(int(hashlib.sha1(str(key).encode("utf-8")).hexdigest(), 16))[
             :18
         ]
+        self.rollback_on_error = rollback_on_error
         self.scope = scope
         self._locked = False
         self._ref_count = 0
         self._shared = shared
 
         infix = "_xact"
         suffix = ""
@@ -139,14 +147,32 @@
             )
 
         self._locked = await self.impl.acquire_async(self, block=block)
         self._ref_count += 1
 
         return self._locked
 
+    def handle_error(self, exc: BaseException) -> None:
+        """
+        Handle an error.
+
+        Parameters:
+            exc (Exception): Exception.
+        """
+        return self.impl.handle_error(self, exc)
+
+    async def handle_error_async(self, exc: BaseException) -> None:
+        """
+        Handle an error asynchronously.
+
+        Parameters:
+            exc (Exception): Exception.
+        """
+        return await self.impl.handle_error_async(self, exc)
+
     @property
     def locked(self) -> bool:
         """
         Returns the lock status.
 
         Returns:
             bool: Locked status.
@@ -280,14 +306,17 @@
         Exit the context manager.
 
         Parameters:
             Exception type (Type[BaseException]): Type of exception that was raised.
             Exception (BaseException): Exception that was raised.
             Traceback (TracebackType): Traceback.
         """
+        if exc:
+            await self.impl.handle_error_async(self, exc)
+
         await self.impl.release_async(self)
 
         if exc:
             raise exc
 
     def __enter__(self) -> bool:
         """
@@ -305,11 +334,14 @@
         Exit the context manager.
 
         Parameters:
             Exception type (Type[BaseException]): Type of exception that was raised.
             Exception (BaseException): Exception that was raised.
             Traceback (TracebackType): Traceback.
         """
+        if exc:
+            self.impl.handle_error(self, exc)
+
         self.impl.release(self)
 
         if exc:
             raise exc
```

### Comparing `postgres_lock-0.1.1/postgres_lock/psycopg2.py` & `postgres_lock-0.1.2/postgres_lock/psycopg2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# --------------------------------------------------------------------------------------------------
+# Copyright (c) 2023 Sean Kerr
+# --------------------------------------------------------------------------------------------------
+
 """
 Lock support for psycopg2 database interface.
 """
 
 from .lock import Lock
 
 
@@ -20,14 +24,15 @@
 
     if not block:
         lock_func = lock.nonblocking_lock_func
 
     cursor = lock.conn.cursor()
     cursor.execute(f"SELECT pg_catalog.{lock_func}({lock.lock_id})")
     result, *_ = cursor.fetchone()
+    cursor.close()
 
     # lock function returns True/False in unblocking mode, and always None in blocking mode
     return False if result is False else True
 
 
 async def acquire_async(lock: Lock, block: bool = True) -> bool:
     """
@@ -39,27 +44,53 @@
 
     Raises:
         NotImplementedError: This function is not implemented.
     """
     raise NotImplementedError("psycopg2 interface does not support acquire_async()")
 
 
+def handle_error(lock: Lock, exc: BaseException) -> None:
+    """
+    Handle an error.
+
+    Parameters:
+        exc (Exception): Exception.
+    """
+    if not lock.rollback_on_error:
+        return
+
+    lock.conn.rollback()
+
+
+async def handle_error_async(lock: Lock, exc: BaseException) -> None:
+    """
+    Handle an error asynchronously.
+
+    Parameters:
+        exc (Exception): Exception.
+    """
+    raise NotImplementedError(
+        "psycopg2 interface does not support handle_error_async()"
+    )
+
+
 def release(lock: Lock) -> bool:
     """
     Release the lock.
 
     Parameters:
         lock (Lock): Lock.
 
     Returns:
         bool: True, if the lock was released, otherwise False.
     """
     cursor = lock.conn.cursor()
     cursor.execute(f"SELECT pg_catalog.{lock.unlock_func}({lock.lock_id})")
     result, *_ = cursor.fetchone()
+    cursor.close()
 
     return result
 
 
 async def release_async(lock: Lock) -> None:
     """
     This function is not implemented.
```

### Comparing `postgres_lock-0.1.1/postgres_lock/psycopg3.py` & `postgres_lock-0.1.2/postgres_lock/psycopg3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# --------------------------------------------------------------------------------------------------
+# Copyright (c) 2023 Sean Kerr
+# --------------------------------------------------------------------------------------------------
+
 """
 Lock support for psycopg3 database interface.
 """
 
 from .lock import Lock
 
 
@@ -20,14 +24,15 @@
 
     if not block:
         lock_func = lock.nonblocking_lock_func
 
     cursor = lock.conn.cursor()
     cursor.execute(f"SELECT pg_catalog.{lock_func}({lock.lock_id})")
     result, *_ = cursor.fetchone()
+    cursor.close()
 
     # lock function returns True/False in unblocking mode, and always None in blocking mode
     return False if result is False else True
 
 
 async def acquire_async(lock: Lock, block: bool = True) -> bool:
     """
@@ -46,32 +51,60 @@
         lock_func = lock.nonblocking_lock_func
 
     cursor = lock.conn.cursor()
 
     await cursor.execute(f"SELECT pg_catalog.{lock_func}({lock.lock_id})")
 
     result, *_ = await cursor.fetchone()
+    cursor.close()
 
     # lock function returns True/False in unblocking mode, and always None in blocking mode
     return False if result is False else True
 
 
+def handle_error(lock: Lock, exc: BaseException) -> None:
+    """
+    Handle an error.
+
+    Parameters:
+        exc (Exception): Exception.
+    """
+    if not lock.rollback_on_error:
+        return
+
+    lock.conn.rollback()
+
+
+async def handle_error_async(lock: Lock, exc: BaseException) -> None:
+    """
+    Handle an error asynchronously.
+
+    Parameters:
+        exc (Exception): Exception.
+    """
+    if not lock.rollback_on_error:
+        return
+
+    await lock.conn.rollback()
+
+
 def release(lock: Lock) -> bool:
     """
     Release the lock.
 
     Parameters:
         lock (Lock): Lock.
 
     Returns:
         bool: True, if the lock was released, otherwise False.
     """
     cursor = lock.conn.cursor()
     cursor.execute(f"SELECT pg_catalog.{lock.unlock_func}({lock.lock_id})")
     result, *_ = cursor.fetchone()
+    cursor.close()
 
     return result
 
 
 async def release_async(lock: Lock) -> bool:
     """
     Release the lock asynchronously.
@@ -83,9 +116,10 @@
         bool: True, if the lock was released, otherwise False.
     """
     cursor = lock.conn.cursor()
 
     await cursor.execute(f"SELECT pg_catalog.{lock.unlock_func}({lock.lock_id})")
 
     result, *_ = await cursor.fetchone()
+    cursor.close()
 
     return result
```

### Comparing `postgres_lock-0.1.1/postgres_lock/sqlalchemy.py` & `postgres_lock-0.1.2/postgres_lock/sqlalchemy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# --------------------------------------------------------------------------------------------------
+# Copyright (c) 2023 Sean Kerr
+# --------------------------------------------------------------------------------------------------
+
 """
 Lock support for sqlalchemy database interface.
 """
 
 from sqlalchemy import text
 
 from .lock import Lock
@@ -51,14 +55,40 @@
         await lock.conn.execute(text(f"SELECT pg_catalog.{lock_func}({lock.lock_id})"))
     ).scalar()
 
     # lock function returns True/False in unblocking mode, and always None in blocking mode
     return False if result is False else True
 
 
+def handle_error(lock: Lock, exc: BaseException) -> None:
+    """
+    Handle an error.
+
+    Parameters:
+        exc (Exception): Exception.
+    """
+    if not lock.rollback_on_error:
+        return
+
+    lock.conn.rollback()
+
+
+async def handle_error_async(lock: Lock, exc: BaseException) -> None:
+    """
+    Handle an error asynchronously.
+
+    Parameters:
+        exc (Exception): Exception.
+    """
+    if not lock.rollback_on_error:
+        return
+
+    await lock.conn.rollback()
+
+
 def release(lock: Lock) -> bool:
     """
     Release the lock.
 
     Parameters:
         lock (Lock): Lock.
```

### Comparing `postgres_lock-0.1.1/pyproject.toml` & `postgres_lock-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgres-lock"
-version = "0.1.1"
+version = "0.1.2"
 description = "Lock mechanism implemented with Postgres advisory locks."
 license = "BSD-3-Clause"
 authors = ["Sean Kerr <sean@code-box.org>"]
 readme = "README.md"
 repository = "https://github.com/seankerr/py-postgres-lock"
 keywords = ["postgres", "postgresql", "distributed", "lock"]
 packages = [{include = "postgres_lock"}]
```

### Comparing `postgres_lock-0.1.1/PKG-INFO` & `postgres_lock-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgres-lock
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lock mechanism implemented with Postgres advisory locks.
 Home-page: https://github.com/seankerr/py-postgres-lock
 License: BSD-3-Clause
 Keywords: postgres,postgresql,distributed,lock
 Author: Sean Kerr
 Author-email: sean@code-box.org
 Requires-Python: >=3.7,<4.0
@@ -48,23 +48,25 @@
 - Postgres table locks aren't sufficient for your use-case
 - Postgres row locks don't work on `INSERT`
 - You want to prevent race conditions between `INSERT` and `UPDATE` on the same primary key
 - None of the aforementioned details fit your use-case, but you have Postgres installed and need to prevent race conditions in a distributed system
 
 ### Default operation
 
-By default `postgres-lock` will use `session` lock scope in `blocking` mode. The `session` lock scope
-means only a single database connection can acquire the lock at a time.
+By default `postgres-lock` will use `session` lock scope in `blocking` mode with
+`rollback_on_error` enabled. The `session` lock scope means only a single database connection can
+acquire the lock at a time.
 
 ### Usage
 
 All work revolves around the `Lock` class.
 
 The easiest way to use `Lock` is with `with` or `async with` statements. The lock will be
-released automatically.
+released automatically. If `rollback_on_error` is enabled (default), rollbacks are automatically
+handled prior to release.
 
 _Using `with` and `async with` implies blocking mode._
 
 ```python
 from postgres_lock import Lock
 
 # setup connection
@@ -90,15 +92,23 @@
 
 try:
     # acquire lock
     lock.acquire()
 
     print("Acquired lock!")
 
-    # do something here
+    try:
+        # do something here
+        pass
+
+    except Exception as exc:
+        # handle_error() will rollback the transaction by default
+        lock.handle_error(exc)
+
+        raise exc
 finally:
     # release lock (this is safe to run even if the lock has not been acquired)
     lock.release()
 ```
 
 ### Asynchronous usage (without `async with`)
 
@@ -113,15 +123,23 @@
 
 try:
     # acquire lock
     await lock.acquire_async()
 
     print("Acquired lock!")
 
-    # do something here
+    try:
+        # do something here
+        pass
+
+    except Exception as exc:
+        # handle_error_async() will rollback the transaction by default
+        await lock.handle_error_async(exc)
+
+        raise exc
 finally:
     # release lock (this is safe to run even if the lock has not been acquired)
     await lock.release_async()
 ```
 
 ### Non-blocking mode (supports async as well)
 
@@ -130,42 +148,56 @@
 
 # setup connection
 conn = ...
 
 # create lock
 lock = Lock(conn, "shared-identifier")
 
-try:
-    # acquire lock
-    if lock.acquire(block=False):
-        print("Acquired lock!")
-
-        # do something here
+# acquire lock
+if lock.acquire(block=False):
+    # do something here
+    pass
 
-    else:
-        print("Could not acquire lock!")
+else:
+    # could not acquire lock
+    pass
 
-finally:
-    # release lock (this is safe to run even if the lock has not been acquired)
-    lock.release()
+# release lock (this is safe to run even if the lock has not been acquired)
+lock.release()
 ```
 
 ### Specify the database interface manually
 
 ```python
 from postgres_lock import Lock
 
 # setup connection
 conn = ...
 
 # create and use lock
-with Lock(conn, "shared-identifier", interface="asyncpg"):
-    print("Acquired lock!")
+lock = Lock(conn, "shared-identifier", interface="asyncpg")
 
-    # do something here
+# do things with the lock
+```
+
+### Handle rollbacks manually
+
+```python
+from postgres_lock import Lock
+
+# setup connection
+conn = ...
+
+# create and use lock
+lock = Lock(conn, "shared-identifier", rollback_on_error=False)
+
+# do things with the lock
 ```
 
 ### Changelog
 
+- **0.1.2**
+  - Add Lock.rollback_on_error (default true)
+  - Add Lock.handle_error() & Lock.handle_error_async()
 - **0.1.1**
   - Key can be str or int
```

