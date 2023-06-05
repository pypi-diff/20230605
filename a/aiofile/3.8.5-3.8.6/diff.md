# Comparing `tmp/aiofile-3.8.5.tar.gz` & `tmp/aiofile-3.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofile-3.8.5.tar", last modified: Thu Mar 16 09:01:18 2023, max compression
+gzip compressed data, was "aiofile-3.8.6.tar", last modified: Mon Jun  5 08:19:36 2023, max compression
```

## Comparing `aiofile-3.8.5.tar` & `aiofile-3.8.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mosquito   (501) staff       (20)        0 2023-03-16 09:01:18.657119 aiofile-3.8.5/
--rw-r--r--   0 mosquito   (501) staff       (20)    10495 2023-03-16 06:38:56.000000 aiofile-3.8.5/LICENCE
--rw-r--r--   0 mosquito   (501) staff       (20)    10495 2023-03-16 06:38:56.000000 aiofile-3.8.5/LICENCE.md
--rw-r--r--   0 mosquito   (501) staff       (20)      180 2023-03-16 06:38:56.000000 aiofile-3.8.5/MANIFEST.in
--rw-r--r--   0 mosquito   (501) staff       (20)    15371 2023-03-16 09:01:18.657293 aiofile-3.8.5/PKG-INFO
--rw-r--r--   0 mosquito   (501) staff       (20)    14007 2023-03-16 09:00:30.000000 aiofile-3.8.5/README.rst
-drwxr-xr-x   0 mosquito   (501) staff       (20)        0 2023-03-16 09:01:18.622355 aiofile-3.8.5/aiofile/
--rw-r--r--   0 mosquito   (501) staff       (20)      618 2023-03-16 06:38:56.000000 aiofile-3.8.5/aiofile/__init__.py
--rw-r--r--   0 mosquito   (501) staff       (20)     9049 2023-03-16 06:38:56.000000 aiofile-3.8.5/aiofile/aio.py
--rw-r--r--   0 mosquito   (501) staff       (20)        1 2023-03-16 06:38:56.000000 aiofile-3.8.5/aiofile/py.typed
--rw-r--r--   0 mosquito   (501) staff       (20)    10079 2023-03-16 06:38:56.000000 aiofile-3.8.5/aiofile/utils.py
--rw-r--r--   0 mosquito   (501) staff       (20)      365 2023-03-16 09:00:53.000000 aiofile-3.8.5/aiofile/version.py
-drwxr-xr-x   0 mosquito   (501) staff       (20)        0 2023-03-16 09:01:18.656750 aiofile-3.8.5/aiofile.egg-info/
--rw-r--r--   0 mosquito   (501) staff       (20)    15371 2023-03-16 09:01:18.000000 aiofile-3.8.5/aiofile.egg-info/PKG-INFO
--rw-r--r--   0 mosquito   (501) staff       (20)      302 2023-03-16 09:01:18.000000 aiofile-3.8.5/aiofile.egg-info/SOURCES.txt
--rw-r--r--   0 mosquito   (501) staff       (20)        1 2023-03-16 09:01:18.000000 aiofile-3.8.5/aiofile.egg-info/dependency_links.txt
--rw-r--r--   0 mosquito   (501) staff       (20)       77 2023-03-16 09:01:18.000000 aiofile-3.8.5/aiofile.egg-info/requires.txt
--rw-r--r--   0 mosquito   (501) staff       (20)        8 2023-03-16 09:01:18.000000 aiofile-3.8.5/aiofile.egg-info/top_level.txt
--rw-r--r--   0 mosquito   (501) staff       (20)      454 2023-03-16 09:01:18.658569 aiofile-3.8.5/setup.cfg
--rw-r--r--   0 mosquito   (501) staff       (20)     1893 2023-03-16 08:36:22.000000 aiofile-3.8.5/setup.py
+drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-06-05 08:19:36.400135 aiofile-3.8.6/
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    10495 2017-01-04 22:01:15.000000 aiofile-3.8.6/LICENCE
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    10495 2017-01-04 22:01:15.000000 aiofile-3.8.6/LICENCE.md
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      180 2021-12-19 14:06:38.000000 aiofile-3.8.6/MANIFEST.in
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    15493 2023-06-05 08:19:36.400238 aiofile-3.8.6/PKG-INFO
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    14076 2023-06-05 08:18:26.000000 aiofile-3.8.6/README.rst
+drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-06-05 08:19:36.391565 aiofile-3.8.6/aiofile/
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      618 2020-11-13 14:01:29.000000 aiofile-3.8.6/aiofile/__init__.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     9049 2023-06-05 08:16:26.000000 aiofile-3.8.6/aiofile/aio.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        1 2020-08-12 20:03:10.000000 aiofile-3.8.6/aiofile/py.typed
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    10079 2022-11-17 08:29:40.000000 aiofile-3.8.6/aiofile/utils.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      365 2023-06-05 08:19:11.000000 aiofile-3.8.6/aiofile/version.py
+drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-06-05 08:19:36.398839 aiofile-3.8.6/aiofile.egg-info/
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    15493 2023-06-05 08:19:36.000000 aiofile-3.8.6/aiofile.egg-info/PKG-INFO
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      302 2023-06-05 08:19:36.000000 aiofile-3.8.6/aiofile.egg-info/SOURCES.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        1 2023-06-05 08:19:36.000000 aiofile-3.8.6/aiofile.egg-info/dependency_links.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)       77 2023-06-05 08:19:36.000000 aiofile-3.8.6/aiofile.egg-info/requires.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        8 2023-06-05 08:19:36.000000 aiofile-3.8.6/aiofile.egg-info/top_level.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      454 2023-06-05 08:19:36.400796 aiofile-3.8.6/setup.cfg
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1943 2023-06-05 07:16:26.000000 aiofile-3.8.6/setup.py
```

### Comparing `aiofile-3.8.5/LICENCE` & `aiofile-3.8.6/LICENCE`

 * *Files identical despite different names*

### Comparing `aiofile-3.8.5/LICENCE.md` & `aiofile-3.8.6/LICENCE.md`

 * *Files identical despite different names*

### Comparing `aiofile-3.8.5/PKG-INFO` & `aiofile-3.8.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofile
-Version: 3.8.5
+Version: 3.8.6
 Summary: Asynchronous file operations.
 Home-page: http://github.com/mosquito/aiofile
 Author: Dmitry Orlov <me@mosquito.su>
 Author-email: me@mosquito.su
 License: Apache 2
 Keywords: aio,python,asyncio,fileio,io
 Platform: POSIX
@@ -20,14 +20,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System
 Classifier: Topic :: System :: Operating System
 Provides: aiofile
 Requires-Python: >=3.7, <4
 Provides-Extra: develop
@@ -67,68 +68,68 @@
 
 Development - Stable
 
 
 Features
 --------
 
-* Since version 2.0.0 using `caio`_, is contain linux ``libaio`` and two
+* Since version 2.0.0 using `caio`_, which contains linux ``libaio`` and two
   thread-based implementations (c-based and pure-python).
 * AIOFile has no internal pointer. You should pass ``offset`` and
   ``chunk_size`` for each operation or use helpers (Reader or Writer).
-  The simples way is use ``async_open`` for create object with
+  The simples way is to use ``async_open`` for creating object with
   file-like interface.
 * For Linux using implementation based on `libaio`_.
 * For POSIX (MacOS X and optional Linux) using implementation
-  using on `threadpool`_.
+  based on `threadpool`_.
 * Otherwise using pure-python thread-based implementation.
 * Implementation chooses automatically depending on system compatibility.
 
 .. _caio: https://pypi.org/project/caio
 .. _libaio: https://pagure.io/libaio
 .. _threadpool: https://github.com/mbrossard/threadpool/
 
 
 Limitations
 -----------
 
-* Linux native AIO implementation not able to open special files.
-  Asynchronous operations against special fs like ``/proc/`` ``/sys/`` not
+* Linux native AIO implementation is not able to open special files.
+  Asynchronous operations against special fs like ``/proc/`` ``/sys/`` are not
   supported by the kernel. It's not a `aiofile`s or `caio` issue.
-  To In this cases, you might switch to thread-based implementations
+  In this cases, you might switch to thread-based implementations
   (see troubleshooting_ section).
   However, when used on supported file systems, the linux implementation has a
-  smaller overhead and preferred but it's not a silver bullet.
+  smaller overhead and is preferred but it's not a silver bullet.
 
 Code examples
 -------------
 
 All code examples requires python 3.6+.
 
 High-level API
 ++++++++++++++
 
 ``async_open`` helper
 ~~~~~~~~~~~~~~~~~~~~~
 
-Helper mimics to python python file-like objects, it's returns file like
-object with similar but async methods.
+Helper mimics python file-like objects, it returns file-like
+objects with similar but async methods.
 
 Supported methods:
 
 * ``async def read(length = -1)`` - reading chunk from file, when length is
-  ``-1`` will be read file to the end.
-* ``async def write(data)`` - write chunk to file
-* ``def seek(offset)`` - set file pointer position
+  ``-1``, will be reading file to the end.
+* ``async def write(data)`` - writing chunk to file
+* ``def seek(offset)`` - setting file pointer position
 * ``def tell()`` - returns current file pointer position
 * ``async def readline(size=-1, newline="\n")`` - read chunks until
   newline or EOF. Since version 3.7.0 ``__aiter__`` returns ``LineReader``.
 
-  This method suboptimal for small lines because doesn't reuse read buffer.
-  When you want to read file by lines please avoid to use ``async_open``
+  This method is suboptimal for small lines because it doesn't reuse read buffer.
+  When you want to read file by lines please avoid using ``async_open``
   use ``LineReader`` instead.
 * ``def __aiter__() -> LineReader`` - iterator over lines.
 * ``def iter_chunked(chunk_size: int = 32768) -> Reader`` - iterator over
   chunks.
 * ``.file`` property contains AIOFile object
 
 
@@ -237,15 +238,15 @@
             async for chunk in src.iter_chunked(arguments.chunk_size):
                 await dest.write(chunk)
 
 
     asyncio.run(main(parser.parse_args()))
 
 
-Example with opening already opened file pointer:
+Example with opening already open file pointer:
 
 .. code-block:: python
     :name: test_opened
 
     import asyncio
     from typing import IO, Any
     from aiofile import async_open
@@ -258,16 +259,16 @@
 
 
     with open("test.txt", "w+") as fp:
         asyncio.run(main(fp))
 
 
 Linux native aio doesn't support reading and writing special files
-(e.g. procfs/sysfs/unix pipes/etc.) so you can perform operations with
-this files using compatible context object.
+(e.g. procfs/sysfs/unix pipes/etc.), so you can perform operations with
+these files using compatible context objects.
 
 .. code-block:: python
 
     import asyncio
     from aiofile import async_open
     from caio import thread_aio_asyncio
     from contextlib import AsyncExitStack
@@ -300,23 +301,23 @@
 
 Low-level API
 ++++++++++++++
 
 The `AIOFile` class is a low-level interface for asynchronous file operations, and the read and write methods accept
 an `offset=0` in bytes at which the operation will be performed.
 
-This allows you to do many independent IO operations on an once opened file without moving the virtual carriage.
+This allows you to do many independent IO operations on an once open file without moving the virtual carriage.
 
-For example, you may made 10 concurrent HTTP requests by specifying the `Range` header, and asynchronously write
+For example, you may make 10 concurrent HTTP requests by specifying the `Range` header, and asynchronously write
 one opened file, while the offsets must either be calculated manually, or use 10 instances of `Writer` with
 specified initial offsets.
 
 In order to provide sequential reading and writing, there is `Writer`, `Reader` and `LineReader`. Keep in mind
 `async_open` is not the same as AIOFile, it provides a similar interface for file operations, it simulates methods
-like read or write as it is implemented in a built-in open.
+like read or write as it is implemented in the built-in open.
 
 .. code-block:: python
     :name: test_low_level_api
 
     import asyncio
     from aiofile import AIOFile
 
@@ -331,15 +332,15 @@
 
             await afp.fsync()
 
             assert await afp.read(len(payload) * 10) == payload * 10
 
     asyncio.run(main())
 
-The Low-level API is fact is just little bit sugared ``caio`` API.
+The Low-level API in fact is just little bit sugared ``caio`` API.
 
 .. code-block:: python
 
     import asyncio
     from aiofile import AIOFile
 
 
@@ -505,15 +506,15 @@
 ---------------
 
 The caio ``linux`` implementation works normal for modern linux kernel versions
 and file systems. So you may have problems specific for your environment.
 It's not a bug and might be resolved some ways:
 
 1. Upgrade the kernel
-2. Use compatible file system
+2. Use compatible file systems
 3. Use threads based or pure python implementation.
 
 The caio since version 0.7.0 contains some ways to do this.
 
 1. In runtime use the environment variable ``CAIO_IMPL`` with
 possible values:
 
@@ -529,23 +530,24 @@
 3. You might manually manage contexts:
 
 .. code-block:: python
 
     import asyncio
 
     from aiofile import async_open
-    from caio import linux_aio, thread_aio
+    from caio import python_aio_asyncio, thread_aio_asyncio
 
 
     async def main():
-        linux_ctx = linux_aio.Context()
-        threads_ctx = thread_aio.Context()
+        linux_ctx = python_aio_asyncio.AsyncioContext()
+        threads_ctx = thread_aio_asyncio.AsyncioContext()
 
-        async with async_open("/tmp/test.txt", "a", context=linux_ctx) as afp:
+        async with async_open("/tmp/test.txt", "w", context=linux_ctx) as afp:
             await afp.write("Hello")
 
-        async with async_open("/tmp/test.txt", "a", context=threads_ctx) as afp:
+        async with async_open("/tmp/test.txt", "r", context=threads_ctx) as afp:
             print(await afp.read())
 
 
     asyncio.run(main())
 
+
```

### Comparing `aiofile-3.8.5/README.rst` & `aiofile-3.8.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,68 +31,68 @@
 
 Development - Stable
 
 
 Features
 --------
 
-* Since version 2.0.0 using `caio`_, is contain linux ``libaio`` and two
+* Since version 2.0.0 using `caio`_, which contains linux ``libaio`` and two
   thread-based implementations (c-based and pure-python).
 * AIOFile has no internal pointer. You should pass ``offset`` and
   ``chunk_size`` for each operation or use helpers (Reader or Writer).
-  The simples way is use ``async_open`` for create object with
+  The simples way is to use ``async_open`` for creating object with
   file-like interface.
 * For Linux using implementation based on `libaio`_.
 * For POSIX (MacOS X and optional Linux) using implementation
-  using on `threadpool`_.
+  based on `threadpool`_.
 * Otherwise using pure-python thread-based implementation.
 * Implementation chooses automatically depending on system compatibility.
 
 .. _caio: https://pypi.org/project/caio
 .. _libaio: https://pagure.io/libaio
 .. _threadpool: https://github.com/mbrossard/threadpool/
 
 
 Limitations
 -----------
 
-* Linux native AIO implementation not able to open special files.
-  Asynchronous operations against special fs like ``/proc/`` ``/sys/`` not
+* Linux native AIO implementation is not able to open special files.
+  Asynchronous operations against special fs like ``/proc/`` ``/sys/`` are not
   supported by the kernel. It's not a `aiofile`s or `caio` issue.
-  To In this cases, you might switch to thread-based implementations
+  In this cases, you might switch to thread-based implementations
   (see troubleshooting_ section).
   However, when used on supported file systems, the linux implementation has a
-  smaller overhead and preferred but it's not a silver bullet.
+  smaller overhead and is preferred but it's not a silver bullet.
 
 Code examples
 -------------
 
 All code examples requires python 3.6+.
 
 High-level API
 ++++++++++++++
 
 ``async_open`` helper
 ~~~~~~~~~~~~~~~~~~~~~
 
-Helper mimics to python python file-like objects, it's returns file like
-object with similar but async methods.
+Helper mimics python file-like objects, it returns file-like
+objects with similar but async methods.
 
 Supported methods:
 
 * ``async def read(length = -1)`` - reading chunk from file, when length is
-  ``-1`` will be read file to the end.
-* ``async def write(data)`` - write chunk to file
-* ``def seek(offset)`` - set file pointer position
+  ``-1``, will be reading file to the end.
+* ``async def write(data)`` - writing chunk to file
+* ``def seek(offset)`` - setting file pointer position
 * ``def tell()`` - returns current file pointer position
 * ``async def readline(size=-1, newline="\n")`` - read chunks until
   newline or EOF. Since version 3.7.0 ``__aiter__`` returns ``LineReader``.
 
-  This method suboptimal for small lines because doesn't reuse read buffer.
-  When you want to read file by lines please avoid to use ``async_open``
+  This method is suboptimal for small lines because it doesn't reuse read buffer.
+  When you want to read file by lines please avoid using ``async_open``
   use ``LineReader`` instead.
 * ``def __aiter__() -> LineReader`` - iterator over lines.
 * ``def iter_chunked(chunk_size: int = 32768) -> Reader`` - iterator over
   chunks.
 * ``.file`` property contains AIOFile object
 
 
@@ -201,15 +201,15 @@
             async for chunk in src.iter_chunked(arguments.chunk_size):
                 await dest.write(chunk)
 
 
     asyncio.run(main(parser.parse_args()))
 
 
-Example with opening already opened file pointer:
+Example with opening already open file pointer:
 
 .. code-block:: python
     :name: test_opened
 
     import asyncio
     from typing import IO, Any
     from aiofile import async_open
@@ -222,16 +222,16 @@
 
 
     with open("test.txt", "w+") as fp:
         asyncio.run(main(fp))
 
 
 Linux native aio doesn't support reading and writing special files
-(e.g. procfs/sysfs/unix pipes/etc.) so you can perform operations with
-this files using compatible context object.
+(e.g. procfs/sysfs/unix pipes/etc.), so you can perform operations with
+these files using compatible context objects.
 
 .. code-block:: python
 
     import asyncio
     from aiofile import async_open
     from caio import thread_aio_asyncio
     from contextlib import AsyncExitStack
@@ -264,23 +264,23 @@
 
 Low-level API
 ++++++++++++++
 
 The `AIOFile` class is a low-level interface for asynchronous file operations, and the read and write methods accept
 an `offset=0` in bytes at which the operation will be performed.
 
-This allows you to do many independent IO operations on an once opened file without moving the virtual carriage.
+This allows you to do many independent IO operations on an once open file without moving the virtual carriage.
 
-For example, you may made 10 concurrent HTTP requests by specifying the `Range` header, and asynchronously write
+For example, you may make 10 concurrent HTTP requests by specifying the `Range` header, and asynchronously write
 one opened file, while the offsets must either be calculated manually, or use 10 instances of `Writer` with
 specified initial offsets.
 
 In order to provide sequential reading and writing, there is `Writer`, `Reader` and `LineReader`. Keep in mind
 `async_open` is not the same as AIOFile, it provides a similar interface for file operations, it simulates methods
-like read or write as it is implemented in a built-in open.
+like read or write as it is implemented in the built-in open.
 
 .. code-block:: python
     :name: test_low_level_api
 
     import asyncio
     from aiofile import AIOFile
 
@@ -295,15 +295,15 @@
 
             await afp.fsync()
 
             assert await afp.read(len(payload) * 10) == payload * 10
 
     asyncio.run(main())
 
-The Low-level API is fact is just little bit sugared ``caio`` API.
+The Low-level API in fact is just little bit sugared ``caio`` API.
 
 .. code-block:: python
 
     import asyncio
     from aiofile import AIOFile
 
 
@@ -469,15 +469,15 @@
 ---------------
 
 The caio ``linux`` implementation works normal for modern linux kernel versions
 and file systems. So you may have problems specific for your environment.
 It's not a bug and might be resolved some ways:
 
 1. Upgrade the kernel
-2. Use compatible file system
+2. Use compatible file systems
 3. Use threads based or pure python implementation.
 
 The caio since version 0.7.0 contains some ways to do this.
 
 1. In runtime use the environment variable ``CAIO_IMPL`` with
 possible values:
 
@@ -493,23 +493,22 @@
 3. You might manually manage contexts:
 
 .. code-block:: python
 
     import asyncio
 
     from aiofile import async_open
-    from caio import linux_aio, thread_aio
+    from caio import python_aio_asyncio, thread_aio_asyncio
 
 
     async def main():
-        linux_ctx = linux_aio.Context()
-        threads_ctx = thread_aio.Context()
+        linux_ctx = python_aio_asyncio.AsyncioContext()
+        threads_ctx = thread_aio_asyncio.AsyncioContext()
 
-        async with async_open("/tmp/test.txt", "a", context=linux_ctx) as afp:
+        async with async_open("/tmp/test.txt", "w", context=linux_ctx) as afp:
             await afp.write("Hello")
 
-        async with async_open("/tmp/test.txt", "a", context=threads_ctx) as afp:
+        async with async_open("/tmp/test.txt", "r", context=threads_ctx) as afp:
             print(await afp.read())
 
 
     asyncio.run(main())
-
```

### Comparing `aiofile-3.8.5/aiofile/__init__.py` & `aiofile-3.8.6/aiofile/__init__.py`

 * *Files identical despite different names*

### Comparing `aiofile-3.8.5/aiofile/aio.py` & `aiofile-3.8.6/aiofile/aio.py`

 * *Files identical despite different names*

### Comparing `aiofile-3.8.5/aiofile/utils.py` & `aiofile-3.8.6/aiofile/utils.py`

 * *Files identical despite different names*

### Comparing `aiofile-3.8.5/aiofile.egg-info/PKG-INFO` & `aiofile-3.8.6/aiofile.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofile
-Version: 3.8.5
+Version: 3.8.6
 Summary: Asynchronous file operations.
 Home-page: http://github.com/mosquito/aiofile
 Author: Dmitry Orlov <me@mosquito.su>
 Author-email: me@mosquito.su
 License: Apache 2
 Keywords: aio,python,asyncio,fileio,io
 Platform: POSIX
@@ -20,14 +20,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System
 Classifier: Topic :: System :: Operating System
 Provides: aiofile
 Requires-Python: >=3.7, <4
 Provides-Extra: develop
@@ -67,68 +68,68 @@
 
 Development - Stable
 
 
 Features
 --------
 
-* Since version 2.0.0 using `caio`_, is contain linux ``libaio`` and two
+* Since version 2.0.0 using `caio`_, which contains linux ``libaio`` and two
   thread-based implementations (c-based and pure-python).
 * AIOFile has no internal pointer. You should pass ``offset`` and
   ``chunk_size`` for each operation or use helpers (Reader or Writer).
-  The simples way is use ``async_open`` for create object with
+  The simples way is to use ``async_open`` for creating object with
   file-like interface.
 * For Linux using implementation based on `libaio`_.
 * For POSIX (MacOS X and optional Linux) using implementation
-  using on `threadpool`_.
+  based on `threadpool`_.
 * Otherwise using pure-python thread-based implementation.
 * Implementation chooses automatically depending on system compatibility.
 
 .. _caio: https://pypi.org/project/caio
 .. _libaio: https://pagure.io/libaio
 .. _threadpool: https://github.com/mbrossard/threadpool/
 
 
 Limitations
 -----------
 
-* Linux native AIO implementation not able to open special files.
-  Asynchronous operations against special fs like ``/proc/`` ``/sys/`` not
+* Linux native AIO implementation is not able to open special files.
+  Asynchronous operations against special fs like ``/proc/`` ``/sys/`` are not
   supported by the kernel. It's not a `aiofile`s or `caio` issue.
-  To In this cases, you might switch to thread-based implementations
+  In this cases, you might switch to thread-based implementations
   (see troubleshooting_ section).
   However, when used on supported file systems, the linux implementation has a
-  smaller overhead and preferred but it's not a silver bullet.
+  smaller overhead and is preferred but it's not a silver bullet.
 
 Code examples
 -------------
 
 All code examples requires python 3.6+.
 
 High-level API
 ++++++++++++++
 
 ``async_open`` helper
 ~~~~~~~~~~~~~~~~~~~~~
 
-Helper mimics to python python file-like objects, it's returns file like
-object with similar but async methods.
+Helper mimics python file-like objects, it returns file-like
+objects with similar but async methods.
 
 Supported methods:
 
 * ``async def read(length = -1)`` - reading chunk from file, when length is
-  ``-1`` will be read file to the end.
-* ``async def write(data)`` - write chunk to file
-* ``def seek(offset)`` - set file pointer position
+  ``-1``, will be reading file to the end.
+* ``async def write(data)`` - writing chunk to file
+* ``def seek(offset)`` - setting file pointer position
 * ``def tell()`` - returns current file pointer position
 * ``async def readline(size=-1, newline="\n")`` - read chunks until
   newline or EOF. Since version 3.7.0 ``__aiter__`` returns ``LineReader``.
 
-  This method suboptimal for small lines because doesn't reuse read buffer.
-  When you want to read file by lines please avoid to use ``async_open``
+  This method is suboptimal for small lines because it doesn't reuse read buffer.
+  When you want to read file by lines please avoid using ``async_open``
   use ``LineReader`` instead.
 * ``def __aiter__() -> LineReader`` - iterator over lines.
 * ``def iter_chunked(chunk_size: int = 32768) -> Reader`` - iterator over
   chunks.
 * ``.file`` property contains AIOFile object
 
 
@@ -237,15 +238,15 @@
             async for chunk in src.iter_chunked(arguments.chunk_size):
                 await dest.write(chunk)
 
 
     asyncio.run(main(parser.parse_args()))
 
 
-Example with opening already opened file pointer:
+Example with opening already open file pointer:
 
 .. code-block:: python
     :name: test_opened
 
     import asyncio
     from typing import IO, Any
     from aiofile import async_open
@@ -258,16 +259,16 @@
 
 
     with open("test.txt", "w+") as fp:
         asyncio.run(main(fp))
 
 
 Linux native aio doesn't support reading and writing special files
-(e.g. procfs/sysfs/unix pipes/etc.) so you can perform operations with
-this files using compatible context object.
+(e.g. procfs/sysfs/unix pipes/etc.), so you can perform operations with
+these files using compatible context objects.
 
 .. code-block:: python
 
     import asyncio
     from aiofile import async_open
     from caio import thread_aio_asyncio
     from contextlib import AsyncExitStack
@@ -300,23 +301,23 @@
 
 Low-level API
 ++++++++++++++
 
 The `AIOFile` class is a low-level interface for asynchronous file operations, and the read and write methods accept
 an `offset=0` in bytes at which the operation will be performed.
 
-This allows you to do many independent IO operations on an once opened file without moving the virtual carriage.
+This allows you to do many independent IO operations on an once open file without moving the virtual carriage.
 
-For example, you may made 10 concurrent HTTP requests by specifying the `Range` header, and asynchronously write
+For example, you may make 10 concurrent HTTP requests by specifying the `Range` header, and asynchronously write
 one opened file, while the offsets must either be calculated manually, or use 10 instances of `Writer` with
 specified initial offsets.
 
 In order to provide sequential reading and writing, there is `Writer`, `Reader` and `LineReader`. Keep in mind
 `async_open` is not the same as AIOFile, it provides a similar interface for file operations, it simulates methods
-like read or write as it is implemented in a built-in open.
+like read or write as it is implemented in the built-in open.
 
 .. code-block:: python
     :name: test_low_level_api
 
     import asyncio
     from aiofile import AIOFile
 
@@ -331,15 +332,15 @@
 
             await afp.fsync()
 
             assert await afp.read(len(payload) * 10) == payload * 10
 
     asyncio.run(main())
 
-The Low-level API is fact is just little bit sugared ``caio`` API.
+The Low-level API in fact is just little bit sugared ``caio`` API.
 
 .. code-block:: python
 
     import asyncio
     from aiofile import AIOFile
 
 
@@ -505,15 +506,15 @@
 ---------------
 
 The caio ``linux`` implementation works normal for modern linux kernel versions
 and file systems. So you may have problems specific for your environment.
 It's not a bug and might be resolved some ways:
 
 1. Upgrade the kernel
-2. Use compatible file system
+2. Use compatible file systems
 3. Use threads based or pure python implementation.
 
 The caio since version 0.7.0 contains some ways to do this.
 
 1. In runtime use the environment variable ``CAIO_IMPL`` with
 possible values:
 
@@ -529,23 +530,24 @@
 3. You might manually manage contexts:
 
 .. code-block:: python
 
     import asyncio
 
     from aiofile import async_open
-    from caio import linux_aio, thread_aio
+    from caio import python_aio_asyncio, thread_aio_asyncio
 
 
     async def main():
-        linux_ctx = linux_aio.Context()
-        threads_ctx = thread_aio.Context()
+        linux_ctx = python_aio_asyncio.AsyncioContext()
+        threads_ctx = thread_aio_asyncio.AsyncioContext()
 
-        async with async_open("/tmp/test.txt", "a", context=linux_ctx) as afp:
+        async with async_open("/tmp/test.txt", "w", context=linux_ctx) as afp:
             await afp.write("Hello")
 
-        async with async_open("/tmp/test.txt", "a", context=threads_ctx) as afp:
+        async with async_open("/tmp/test.txt", "r", context=threads_ctx) as afp:
             print(await afp.read())
 
 
     asyncio.run(main())
 
+
```

### Comparing `aiofile-3.8.5/setup.py` & `aiofile-3.8.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Software Development :: Libraries",
         "Topic :: System",
         "Topic :: System :: Operating System",
     ],
     python_requires=">=3.7, <4",
     extras_require={
```

