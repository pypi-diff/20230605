# Comparing `tmp/ezq-3.0.3.tar.gz` & `tmp/ezq-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezq-3.0.3.tar", last modified: Mon May 22 02:34:44 2023, max compression
+gzip compressed data, was "ezq-3.0.4.tar", last modified: Mon Jun  5 03:12:14 2023, max compression
```

## Comparing `ezq-3.0.3.tar` & `ezq-3.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:44.530097 ezq-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-22 02:34:26.000000 ezq-3.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-22 02:34:44.530097 ezq-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-05-22 02:34:26.000000 ezq-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-22 02:34:26.000000 ezq-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:34:44.530097 ezq-3.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:44.530097 ezq-3.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:44.530097 ezq-3.0.3/src/ezq/
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-05-22 02:34:26.000000 ezq-3.0.3/src/ezq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:44.530097 ezq-3.0.3/src/ezq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-22 02:34:44.000000 ezq-3.0.3/src/ezq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-22 02:34:44.000000 ezq-3.0.3/src/ezq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:34:44.000000 ezq-3.0.3/src/ezq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 02:34:44.000000 ezq-3.0.3/src/ezq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 02:34:44.000000 ezq-3.0.3/src/ezq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:34:44.530097 ezq-3.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-22 02:34:26.000000 ezq-3.0.3/test/test_ezq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-22 02:34:26.000000 ezq-3.0.3/test/test_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:12:14.001636 ezq-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-05 03:11:55.000000 ezq-3.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-06-05 03:12:14.001636 ezq-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-05 03:11:55.000000 ezq-3.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-05 03:11:55.000000 ezq-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 03:12:14.001636 ezq-3.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:12:13.997636 ezq-3.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:12:13.997636 ezq-3.0.4/src/ezq/
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-06-05 03:11:55.000000 ezq-3.0.4/src/ezq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 03:11:55.000000 ezq-3.0.4/src/ezq/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:12:14.001636 ezq-3.0.4/src/ezq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-06-05 03:12:13.000000 ezq-3.0.4/src/ezq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-05 03:12:13.000000 ezq-3.0.4/src/ezq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 03:12:13.000000 ezq-3.0.4/src/ezq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 03:12:13.000000 ezq-3.0.4/src/ezq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 03:12:13.000000 ezq-3.0.4/src/ezq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:12:14.001636 ezq-3.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-05 03:11:55.000000 ezq-3.0.4/test/test_ezq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-05 03:11:55.000000 ezq-3.0.4/test/test_iter.py
```

### Comparing `ezq-3.0.3/LICENSE.md` & `ezq-3.0.4/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2021 Metaist LLC.
+Copyright 2023 Metaist LLC.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `ezq-3.0.3/PKG-INFO` & `ezq-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezq
-Version: 3.0.3
+Version: 3.0.4
 Summary: Simple wrapper for python multiprocessing and threading.
 Author-email: Metaist LLC <metaist@metaist.com>
 License: MIT
 Project-URL: Homepage, https://github.com/metaist/ezq
 Project-URL: Documentation, https://metaist.github.io/ezq/
 Project-URL: Repository, https://github.com/metaist/ezq.git
 Project-URL: Changelog, https://github.com/metaist/ezq/blob/main/CHANGELOG.md
@@ -17,14 +17,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # ezq
 
@@ -47,15 +49,15 @@
 [1]: https://docs.python.org/3/library/concurrent.futures.html
 [2]: https://docs.python.org/3/library/multiprocessing.html
 [3]: https://docs.python.org/3/library/threading.html
 
 ## Install
 
 ```bash
-pip install ezq
+python -m pip install ezq
 ```
 
 ## Example: Quick Start
 
 If you just want to apply a function to some inputs, you can use `ezq.map()` to run it on all available CPUs and get the results back.
 
 ```python
```

### Comparing `ezq-3.0.3/README.md` & `ezq-3.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 [1]: https://docs.python.org/3/library/concurrent.futures.html
 [2]: https://docs.python.org/3/library/multiprocessing.html
 [3]: https://docs.python.org/3/library/threading.html
 
 ## Install
 
 ```bash
-pip install ezq
+python -m pip install ezq
 ```
 
 ## Example: Quick Start
 
 If you just want to apply a function to some inputs, you can use `ezq.map()` to run it on all available CPUs and get the results back.
 
 ```python
```

### Comparing `ezq-3.0.3/src/ezq/__init__.py` & `ezq-3.0.4/src/ezq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,13 @@
-#!/usr/bin/env python
-# coding: utf-8
 """Simple wrapper for python `multiprocessing` and `threading`.
 
 .. include:: ../../README.md
    :start-line: 4
 """
 
-__all__ = (
-    "Task",
-    "Context",
-    "ContextName",
-    "Msg",
-    "END_MSG",
-    "MsgQ",
-    "NUM_CPUS",
-    "NUM_THREADS",
-    "IS_MACOS",
-    "Worker",
-    "Q",
-    "run",
-    "run_thread",
-    "map",
-)
-
 # native
 from dataclasses import dataclass
 from operator import attrgetter
 from os import cpu_count
 from platform import system
 from queue import Empty
 from queue import Queue as ThreadSafeQueue
@@ -42,14 +23,34 @@
 from typing import TYPE_CHECKING
 from typing import Union
 
 # lib
 from multiprocess import Process  # type: ignore
 from multiprocess import Queue
 
+__all__ = (
+    "__version__",
+    "Task",
+    "Context",
+    "ContextName",
+    "Msg",
+    "END_MSG",
+    "MsgQ",
+    "NUM_CPUS",
+    "NUM_THREADS",
+    "IS_MACOS",
+    "Worker",
+    "Q",
+    "run",
+    "run_thread",
+    "map",
+)
+
+__version__ = "3.0.4"
+
 Task = Callable[..., Any]
 """Task function signature (any `Callable`)."""
 
 Context = Union[Process, Thread]
 """Execution contexts (`Process`, `Thread`)."""
 
 ContextName = Literal["process", "thread"]
@@ -68,14 +69,15 @@
 
     order: int = 0
     """Optional ordering of messages."""
 
 
 # NOTE: The python `queue.Queue` is not properly a generic.
 # See: https://stackoverflow.com/a/48554601
+# TODO [2024-10-14]: @ py3.8 EOL remove this conditional
 if TYPE_CHECKING:  # pragma: no cover
     MsgQ = Union[Queue[Msg], ThreadSafeQueue]  # pylint: disable=unsubscriptable-object
 else:
     MsgQ = Queue
 
 END_MSG: Msg = Msg(kind="END")
 """Message that indicates no future messages will be sent."""
```

### Comparing `ezq-3.0.3/src/ezq.egg-info/PKG-INFO` & `ezq-3.0.4/src/ezq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezq
-Version: 3.0.3
+Version: 3.0.4
 Summary: Simple wrapper for python multiprocessing and threading.
 Author-email: Metaist LLC <metaist@metaist.com>
 License: MIT
 Project-URL: Homepage, https://github.com/metaist/ezq
 Project-URL: Documentation, https://metaist.github.io/ezq/
 Project-URL: Repository, https://github.com/metaist/ezq.git
 Project-URL: Changelog, https://github.com/metaist/ezq/blob/main/CHANGELOG.md
@@ -17,14 +17,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # ezq
 
@@ -47,15 +49,15 @@
 [1]: https://docs.python.org/3/library/concurrent.futures.html
 [2]: https://docs.python.org/3/library/multiprocessing.html
 [3]: https://docs.python.org/3/library/threading.html
 
 ## Install
 
 ```bash
-pip install ezq
+python -m pip install ezq
 ```
 
 ## Example: Quick Start
 
 If you just want to apply a function to some inputs, you can use `ezq.map()` to run it on all available CPUs and get the results back.
 
 ```python
```

### Comparing `ezq-3.0.3/test/test_ezq.py` & `ezq-3.0.4/test/test_ezq.py`

 * *Files identical despite different names*

### Comparing `ezq-3.0.3/test/test_iter.py` & `ezq-3.0.4/test/test_iter.py`

 * *Files identical despite different names*

