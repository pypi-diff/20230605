# Comparing `tmp/aiofile-3.8.6.tar.gz` & `tmp/aiofile-3.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofile-3.8.6.tar", last modified: Mon Jun  5 08:19:36 2023, max compression
+gzip compressed data, was "aiofile-3.8.7.tar", last modified: Mon Jun  5 08:26:10 2023, max compression
```

## Comparing `aiofile-3.8.6.tar` & `aiofile-3.8.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-06-05 08:19:36.400135 aiofile-3.8.6/
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    10495 2017-01-04 22:01:15.000000 aiofile-3.8.6/LICENCE
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    10495 2017-01-04 22:01:15.000000 aiofile-3.8.6/LICENCE.md
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      180 2021-12-19 14:06:38.000000 aiofile-3.8.6/MANIFEST.in
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    15493 2023-06-05 08:19:36.400238 aiofile-3.8.6/PKG-INFO
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    14076 2023-06-05 08:18:26.000000 aiofile-3.8.6/README.rst
-drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-06-05 08:19:36.391565 aiofile-3.8.6/aiofile/
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      618 2020-11-13 14:01:29.000000 aiofile-3.8.6/aiofile/__init__.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     9049 2023-06-05 08:16:26.000000 aiofile-3.8.6/aiofile/aio.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        1 2020-08-12 20:03:10.000000 aiofile-3.8.6/aiofile/py.typed
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    10079 2022-11-17 08:29:40.000000 aiofile-3.8.6/aiofile/utils.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      365 2023-06-05 08:19:11.000000 aiofile-3.8.6/aiofile/version.py
-drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-06-05 08:19:36.398839 aiofile-3.8.6/aiofile.egg-info/
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    15493 2023-06-05 08:19:36.000000 aiofile-3.8.6/aiofile.egg-info/PKG-INFO
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      302 2023-06-05 08:19:36.000000 aiofile-3.8.6/aiofile.egg-info/SOURCES.txt
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        1 2023-06-05 08:19:36.000000 aiofile-3.8.6/aiofile.egg-info/dependency_links.txt
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)       77 2023-06-05 08:19:36.000000 aiofile-3.8.6/aiofile.egg-info/requires.txt
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        8 2023-06-05 08:19:36.000000 aiofile-3.8.6/aiofile.egg-info/top_level.txt
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      454 2023-06-05 08:19:36.400796 aiofile-3.8.6/setup.cfg
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1943 2023-06-05 07:16:26.000000 aiofile-3.8.6/setup.py
+drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-06-05 08:26:10.597904 aiofile-3.8.7/
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    10495 2017-01-04 22:01:15.000000 aiofile-3.8.7/LICENCE
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    10495 2017-01-04 22:01:15.000000 aiofile-3.8.7/LICENCE.md
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      180 2021-12-19 14:06:38.000000 aiofile-3.8.7/MANIFEST.in
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    15491 2023-06-05 08:26:10.598028 aiofile-3.8.7/PKG-INFO
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    14074 2023-06-05 08:25:43.000000 aiofile-3.8.7/README.rst
+drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-06-05 08:26:10.593604 aiofile-3.8.7/aiofile/
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      618 2020-11-13 14:01:29.000000 aiofile-3.8.7/aiofile/__init__.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     9049 2023-06-05 08:16:26.000000 aiofile-3.8.7/aiofile/aio.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        1 2020-08-12 20:03:10.000000 aiofile-3.8.7/aiofile/py.typed
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    10079 2022-11-17 08:29:40.000000 aiofile-3.8.7/aiofile/utils.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      365 2023-06-05 08:25:51.000000 aiofile-3.8.7/aiofile/version.py
+drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-06-05 08:26:10.597396 aiofile-3.8.7/aiofile.egg-info/
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    15491 2023-06-05 08:26:10.000000 aiofile-3.8.7/aiofile.egg-info/PKG-INFO
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      302 2023-06-05 08:26:10.000000 aiofile-3.8.7/aiofile.egg-info/SOURCES.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        1 2023-06-05 08:26:10.000000 aiofile-3.8.7/aiofile.egg-info/dependency_links.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)       77 2023-06-05 08:26:10.000000 aiofile-3.8.7/aiofile.egg-info/requires.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        8 2023-06-05 08:26:10.000000 aiofile-3.8.7/aiofile.egg-info/top_level.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      454 2023-06-05 08:26:10.598623 aiofile-3.8.7/setup.cfg
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1943 2023-06-05 07:16:26.000000 aiofile-3.8.7/setup.py
```

### Comparing `aiofile-3.8.6/LICENCE` & `aiofile-3.8.7/LICENCE`

 * *Files identical despite different names*

### Comparing `aiofile-3.8.6/LICENCE.md` & `aiofile-3.8.7/LICENCE.md`

 * *Files identical despite different names*

### Comparing `aiofile-3.8.6/PKG-INFO` & `aiofile-3.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofile
-Version: 3.8.6
+Version: 3.8.7
 Summary: Asynchronous file operations.
 Home-page: http://github.com/mosquito/aiofile
 Author: Dmitry Orlov <me@mosquito.su>
 Author-email: me@mosquito.su
 License: Apache 2
 Keywords: aio,python,asyncio,fileio,io
 Platform: POSIX
@@ -530,19 +530,19 @@
 3. You might manually manage contexts:
 
 .. code-block:: python
 
     import asyncio
 
     from aiofile import async_open
-    from caio import python_aio_asyncio, thread_aio_asyncio
+    from caio import linux_aio_asyncio, thread_aio_asyncio
 
 
     async def main():
-        linux_ctx = python_aio_asyncio.AsyncioContext()
+        linux_ctx = linux_aio_asyncio.AsyncioContext()
         threads_ctx = thread_aio_asyncio.AsyncioContext()
 
         async with async_open("/tmp/test.txt", "w", context=linux_ctx) as afp:
             await afp.write("Hello")
 
         async with async_open("/tmp/test.txt", "r", context=threads_ctx) as afp:
             print(await afp.read())
```

### Comparing `aiofile-3.8.6/README.rst` & `aiofile-3.8.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -493,19 +493,19 @@
 3. You might manually manage contexts:
 
 .. code-block:: python
 
     import asyncio
 
     from aiofile import async_open
-    from caio import python_aio_asyncio, thread_aio_asyncio
+    from caio import linux_aio_asyncio, thread_aio_asyncio
 
 
     async def main():
-        linux_ctx = python_aio_asyncio.AsyncioContext()
+        linux_ctx = linux_aio_asyncio.AsyncioContext()
         threads_ctx = thread_aio_asyncio.AsyncioContext()
 
         async with async_open("/tmp/test.txt", "w", context=linux_ctx) as afp:
             await afp.write("Hello")
 
         async with async_open("/tmp/test.txt", "r", context=threads_ctx) as afp:
             print(await afp.read())
```

### Comparing `aiofile-3.8.6/aiofile/__init__.py` & `aiofile-3.8.7/aiofile/__init__.py`

 * *Files identical despite different names*

### Comparing `aiofile-3.8.6/aiofile/aio.py` & `aiofile-3.8.7/aiofile/aio.py`

 * *Files identical despite different names*

### Comparing `aiofile-3.8.6/aiofile/utils.py` & `aiofile-3.8.7/aiofile/utils.py`

 * *Files identical despite different names*

### Comparing `aiofile-3.8.6/aiofile.egg-info/PKG-INFO` & `aiofile-3.8.7/aiofile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofile
-Version: 3.8.6
+Version: 3.8.7
 Summary: Asynchronous file operations.
 Home-page: http://github.com/mosquito/aiofile
 Author: Dmitry Orlov <me@mosquito.su>
 Author-email: me@mosquito.su
 License: Apache 2
 Keywords: aio,python,asyncio,fileio,io
 Platform: POSIX
@@ -530,19 +530,19 @@
 3. You might manually manage contexts:
 
 .. code-block:: python
 
     import asyncio
 
     from aiofile import async_open
-    from caio import python_aio_asyncio, thread_aio_asyncio
+    from caio import linux_aio_asyncio, thread_aio_asyncio
 
 
     async def main():
-        linux_ctx = python_aio_asyncio.AsyncioContext()
+        linux_ctx = linux_aio_asyncio.AsyncioContext()
         threads_ctx = thread_aio_asyncio.AsyncioContext()
 
         async with async_open("/tmp/test.txt", "w", context=linux_ctx) as afp:
             await afp.write("Hello")
 
         async with async_open("/tmp/test.txt", "r", context=threads_ctx) as afp:
             print(await afp.read())
```

### Comparing `aiofile-3.8.6/setup.py` & `aiofile-3.8.7/setup.py`

 * *Files identical despite different names*

