# Comparing `tmp/mslex-1.0.1.tar.gz` & `tmp/mslex-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mslex-1.0.1.tar", last modified: Tue May 16 15:55:31 2023, max compression
+gzip compressed data, was "mslex-1.1.0.tar", last modified: Mon Jun  5 17:09:30 2023, max compression
```

## Comparing `mslex-1.0.1.tar` & `mslex-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,181 @@
-drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-05-16 15:55:31.287880 mslex-1.0.1/
--rw-r--r--   0 larry      (502) staff       (20)      161 2023-03-22 17:56:02.000000 mslex-1.0.1/AUTHORS.rst
--rw-r--r--   0 larry      (502) staff       (20)     3497 2023-03-22 17:56:02.000000 mslex-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 larry      (502) staff       (20)       89 2023-03-22 17:56:02.000000 mslex-1.0.1/HISTORY.rst
--rw-r--r--   0 larry      (502) staff       (20)      587 2023-03-22 17:56:02.000000 mslex-1.0.1/LICENSE
--rw-r--r--   0 larry      (502) staff       (20)      262 2023-03-22 17:56:02.000000 mslex-1.0.1/MANIFEST.in
--rw-r--r--   0 larry      (502) staff       (20)     2769 2023-05-16 15:55:31.287925 mslex-1.0.1/PKG-INFO
--rw-r--r--   0 larry      (502) staff       (20)     1973 2023-05-15 20:22:39.000000 mslex-1.0.1/README.rst
-drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-05-16 15:55:31.286569 mslex-1.0.1/docs/
--rw-r--r--   0 larry      (502) staff       (20)      607 2023-03-22 17:56:02.000000 mslex-1.0.1/docs/Makefile
--rw-r--r--   0 larry      (502) staff       (20)       28 2023-03-22 17:56:02.000000 mslex-1.0.1/docs/authors.rst
--rwxr-xr-x   0 larry      (502) staff       (20)     4793 2023-03-22 17:56:02.000000 mslex-1.0.1/docs/conf.py
--rw-r--r--   0 larry      (502) staff       (20)       33 2023-03-22 17:56:02.000000 mslex-1.0.1/docs/contributing.rst
--rw-r--r--   0 larry      (502) staff       (20)       28 2023-03-22 17:56:02.000000 mslex-1.0.1/docs/history.rst
--rw-r--r--   0 larry      (502) staff       (20)      302 2023-03-22 17:56:02.000000 mslex-1.0.1/docs/index.rst
--rw-r--r--   0 larry      (502) staff       (20)     1094 2023-03-22 17:56:02.000000 mslex-1.0.1/docs/installation.rst
--rw-r--r--   0 larry      (502) staff       (20)      767 2023-03-22 17:56:02.000000 mslex-1.0.1/docs/make.bat
--rw-r--r--   0 larry      (502) staff       (20)       27 2023-03-22 17:56:02.000000 mslex-1.0.1/docs/readme.rst
--rw-r--r--   0 larry      (502) staff       (20)       65 2023-03-22 17:56:02.000000 mslex-1.0.1/docs/usage.rst
-drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-05-16 15:55:31.287417 mslex-1.0.1/mslex.egg-info/
--rw-r--r--   0 larry      (502) staff       (20)     2769 2023-05-16 15:55:31.000000 mslex-1.0.1/mslex.egg-info/PKG-INFO
--rw-r--r--   0 larry      (502) staff       (20)      478 2023-05-16 15:55:31.000000 mslex-1.0.1/mslex.egg-info/SOURCES.txt
--rw-r--r--   0 larry      (502) staff       (20)        1 2023-05-16 15:55:31.000000 mslex-1.0.1/mslex.egg-info/dependency_links.txt
--rw-r--r--   0 larry      (502) staff       (20)       48 2023-05-16 15:55:31.000000 mslex-1.0.1/mslex.egg-info/entry_points.txt
--rw-r--r--   0 larry      (502) staff       (20)        1 2023-05-15 20:22:02.000000 mslex-1.0.1/mslex.egg-info/not-zip-safe
--rw-r--r--   0 larry      (502) staff       (20)        6 2023-05-16 15:55:31.000000 mslex-1.0.1/mslex.egg-info/top_level.txt
--rw-r--r--   0 larry      (502) staff       (20)     5324 2023-05-16 15:54:54.000000 mslex-1.0.1/mslex.py
--rw-r--r--   0 larry      (502) staff       (20)      379 2023-05-16 15:55:31.288169 mslex-1.0.1/setup.cfg
--rw-r--r--   0 larry      (502) staff       (20)     1419 2023-05-16 15:54:54.000000 mslex-1.0.1/setup.py
-drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-05-16 15:55:31.287709 mslex-1.0.1/tests/
--rw-r--r--   0 larry      (502) staff       (20)       60 2023-03-22 17:56:02.000000 mslex-1.0.1/tests/__init__.py
--rw-r--r--   0 larry      (502) staff       (20)    12080 2023-05-15 20:19:16.000000 mslex-1.0.1/tests/test_mslex.py
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:30.009098 mslex-1.1.0/
+-rw-r--r--   0 larry      (502) staff       (20)      161 2023-03-22 17:56:02.000000 mslex-1.1.0/AUTHORS.rst
+-rw-r--r--   0 larry      (502) staff       (20)     3497 2023-03-22 17:56:02.000000 mslex-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 larry      (502) staff       (20)       89 2023-03-22 17:56:02.000000 mslex-1.1.0/HISTORY.rst
+-rw-r--r--   0 larry      (502) staff       (20)      587 2023-03-22 17:56:02.000000 mslex-1.1.0/LICENSE
+-rw-r--r--   0 larry      (502) staff       (20)      262 2023-03-22 17:56:02.000000 mslex-1.1.0/MANIFEST.in
+-rw-r--r--   0 larry      (502) staff       (20)     3018 2023-06-05 17:09:30.009168 mslex-1.1.0/PKG-INFO
+-rw-r--r--   0 larry      (502) staff       (20)     2222 2023-06-05 17:01:26.000000 mslex-1.1.0/README.rst
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:29.945849 mslex-1.1.0/docs/
+-rw-r--r--   0 larry      (502) staff       (20)      607 2023-03-22 17:56:02.000000 mslex-1.1.0/docs/Makefile
+-rw-r--r--   0 larry      (502) staff       (20)       28 2023-03-22 17:56:02.000000 mslex-1.1.0/docs/authors.rst
+-rwxr-xr-x   0 larry      (502) staff       (20)     4793 2023-03-22 17:56:02.000000 mslex-1.1.0/docs/conf.py
+-rw-r--r--   0 larry      (502) staff       (20)       33 2023-03-22 17:56:02.000000 mslex-1.1.0/docs/contributing.rst
+-rw-r--r--   0 larry      (502) staff       (20)       28 2023-03-22 17:56:02.000000 mslex-1.1.0/docs/history.rst
+-rw-r--r--   0 larry      (502) staff       (20)      302 2023-03-22 17:56:02.000000 mslex-1.1.0/docs/index.rst
+-rw-r--r--   0 larry      (502) staff       (20)     1094 2023-03-22 17:56:02.000000 mslex-1.1.0/docs/installation.rst
+-rw-r--r--   0 larry      (502) staff       (20)      767 2023-03-22 17:56:02.000000 mslex-1.1.0/docs/make.bat
+-rw-r--r--   0 larry      (502) staff       (20)       27 2023-03-22 17:56:02.000000 mslex-1.1.0/docs/readme.rst
+-rw-r--r--   0 larry      (502) staff       (20)       65 2023-03-22 17:56:02.000000 mslex-1.1.0/docs/usage.rst
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:29.946074 mslex-1.1.0/mslex/
+-rw-r--r--   0 larry      (502) staff       (20)     6111 2023-06-05 17:07:44.000000 mslex-1.1.0/mslex/__init__.py
+-rw-r--r--   0 larry      (502) staff       (20)        0 2023-06-05 17:04:42.000000 mslex-1.1.0/mslex/py.typed
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:29.946964 mslex-1.1.0/mslex.egg-info/
+-rw-r--r--   0 larry      (502) staff       (20)     3018 2023-06-05 17:09:29.000000 mslex-1.1.0/mslex.egg-info/PKG-INFO
+-rw-r--r--   0 larry      (502) staff       (20)     6562 2023-06-05 17:09:29.000000 mslex-1.1.0/mslex.egg-info/SOURCES.txt
+-rw-r--r--   0 larry      (502) staff       (20)        1 2023-06-05 17:09:29.000000 mslex-1.1.0/mslex.egg-info/dependency_links.txt
+-rw-r--r--   0 larry      (502) staff       (20)       48 2023-06-05 17:09:29.000000 mslex-1.1.0/mslex.egg-info/entry_points.txt
+-rw-r--r--   0 larry      (502) staff       (20)        1 2023-05-15 20:22:02.000000 mslex-1.1.0/mslex.egg-info/not-zip-safe
+-rw-r--r--   0 larry      (502) staff       (20)        6 2023-06-05 17:09:29.000000 mslex-1.1.0/mslex.egg-info/top_level.txt
+-rw-r--r--   0 larry      (502) staff       (20)      388 2023-06-05 17:09:30.009537 mslex-1.1.0/setup.cfg
+-rw-r--r--   0 larry      (502) staff       (20)     1459 2023-06-05 17:07:44.000000 mslex-1.1.0/setup.py
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:29.947187 mslex-1.1.0/tests/
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:29.947542 mslex-1.1.0/tests/.mypy_cache/
+-rw-r--r--   0 larry      (502) staff       (20)       34 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/.gitignore
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:29.967456 mslex-1.1.0/tests/.mypy_cache/3.10/
+-rw-r--r--   0 larry      (502) staff       (20)        2 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0 larry      (502) staff       (20)   193642 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1742 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    57262 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1788 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    19735 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1696 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)     3148 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1698 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    25932 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1740 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_thread.meta.json
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:29.969726 mslex-1.1.0/tests/.mypy_cache/3.10/_typeshed/
+-rw-r--r--   0 larry      (502) staff       (20)    96945 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1820 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    14278 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1625 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    22330 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1684 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   165791 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/argparse.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1787 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/argparse.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    66347 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1751 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)  1141179 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1848 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   134183 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1802 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/codecs.meta.json
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:29.991320 mslex-1.1.0/tests/.mypy_cache/3.10/collections/
+-rw-r--r--   0 larry      (502) staff       (20)   446236 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1831 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)     4010 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1662 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   113641 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1726 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/contextlib.meta.json
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:29.992436 mslex-1.1.0/tests/.mypy_cache/3.10/ctypes/
+-rw-r--r--   0 larry      (502) staff       (20)   140909 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1794 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    63221 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1744 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/dataclasses.meta.json
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:30.001228 mslex-1.1.0/tests/.mypy_cache/3.10/email/
+-rw-r--r--   0 larry      (502) staff       (20)     8096 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1723 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    13248 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1659 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)     7870 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1694 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    26961 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1666 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)     9962 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1679 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    86464 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1797 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    33547 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1752 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    66810 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1716 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   139254 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/functools.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1725 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/functools.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    24370 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1713 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/genericpath.meta.json
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:30.002661 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/
+-rw-r--r--   0 larry      (502) staff       (20)     6656 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1697 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    75501 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1845 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    69902 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1856 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/machinery.meta.json
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:30.003333 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/metadata/
+-rw-r--r--   0 larry      (502) staff       (20)    97868 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1862 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    12906 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1679 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    93229 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1807 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   292319 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/itertools.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1727 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/itertools.meta.json
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:30.004085 mslex-1.1.0/tests/.mypy_cache/3.10/logging/
+-rw-r--r--   0 larry      (502) staff       (20)   154238 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1820 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    29330 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1750 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)     7402 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/mslex.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1676 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/mslex.meta.json
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:30.005320 mslex-1.1.0/tests/.mypy_cache/3.10/os/
+-rw-r--r--   0 larry      (502) staff       (20)   351842 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1865 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)     5289 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1654 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    96544 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1816 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    48510 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1752 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    82078 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1746 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   182891 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1838 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    15173 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1682 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    30227 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1694 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    53677 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1746 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    28875 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1731 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   173143 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1806 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   152120 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1785 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/sys.meta.json
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:30.005664 mslex-1.1.0/tests/.mypy_cache/3.10/tests/
+-rw-r--r--   0 larry      (502) staff       (20)     1552 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/tests/__init__.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1583 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/tests/__init__.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    70498 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1716 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    46564 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1675 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   248477 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1757 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   444922 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1823 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    73925 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1747 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/typing_extensions.meta.json
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-06-05 17:09:30.008954 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/
+-rw-r--r--   0 larry      (502) staff       (20)     6439 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1874 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    26115 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1722 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)     8250 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1753 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)   225857 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1873 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    15850 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1784 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    12723 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1793 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    22378 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1740 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    11639 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1783 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    12301 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1735 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    12194 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1756 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)    24129 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0 larry      (502) staff       (20)     1743 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0 larry      (502) staff       (20)      190 2023-05-16 16:34:56.000000 mslex-1.1.0/tests/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0 larry      (502) staff       (20)       60 2023-03-22 17:56:02.000000 mslex-1.1.0/tests/__init__.py
+-rw-r--r--   0 larry      (502) staff       (20)    12080 2023-05-15 20:19:16.000000 mslex-1.1.0/tests/test_mslex.py
```

### Comparing `mslex-1.0.1/CONTRIBUTING.rst` & `mslex-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mslex-1.0.1/LICENSE` & `mslex-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mslex-1.0.1/PKG-INFO` & `mslex-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mslex
-Version: 1.0.1
+Version: 1.1.0
 Summary: shlex for windows
 Home-page: https://github.com/smoofra/mslex
 Author: Lawrence D'Anna
 Author-email: larry@elder-gods.org
 License: Apache Software License 2.0
 Keywords: mslex
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,16 +39,16 @@
 
 * Free software: Apache Software License 2.0
 * Documentation: https://mslex.readthedocs.io.
 
 Features
 --------
 
-This is the missing shlex package for windows shell quoting.   It provides two
-functions -- split and quote -- just like shlex.
+This is the missing shlex package for windows shell quoting.   It provides three
+functions -- split, quote, and join -- just like shlex.
 
 
 Credits
 -------
 
 These are excellent articles to read if you really want to face the
 sanity-melting reality buried under the surface of how windows passes command
@@ -70,14 +70,21 @@
   https://blogs.msdn.microsoft.com/twistylittlepassagesallalike/2011/04/23/everyone-quotes-command-line-arguments-the-wrong-way/
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
+Automatic selection between mslex and shlex
+-------------------------------------------
+
+If you want to automatically use mslex on Windows, and shlex otherwise, check out the `oslex`_ package.
+
+.. _`oslex`: https://pypi.org/project/oslex/
+
 
 =======
 History
 =======
 
 0.1.0 (2019-10-02)
 ------------------
```

### Comparing `mslex-1.0.1/README.rst` & `mslex-1.1.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 * Free software: Apache Software License 2.0
 * Documentation: https://mslex.readthedocs.io.
 
 Features
 --------
 
-This is the missing shlex package for windows shell quoting.   It provides two
-functions -- split and quote -- just like shlex.
+This is the missing shlex package for windows shell quoting.   It provides three
+functions -- split, quote, and join -- just like shlex.
 
 
 Credits
 -------
 
 These are excellent articles to read if you really want to face the
 sanity-melting reality buried under the surface of how windows passes command
@@ -48,7 +48,14 @@
 .. _`Everyone quotes command line arguments the wrong way`:
   https://blogs.msdn.microsoft.com/twistylittlepassagesallalike/2011/04/23/everyone-quotes-command-line-arguments-the-wrong-way/
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+Automatic selection between mslex and shlex
+-------------------------------------------
+
+If you want to automatically use mslex on Windows, and shlex otherwise, check out the `oslex`_ package.
+
+.. _`oslex`: https://pypi.org/project/oslex/
```

### Comparing `mslex-1.0.1/docs/Makefile` & `mslex-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mslex-1.0.1/docs/conf.py` & `mslex-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mslex-1.0.1/docs/installation.rst` & `mslex-1.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mslex-1.0.1/docs/make.bat` & `mslex-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mslex-1.0.1/mslex.egg-info/PKG-INFO` & `mslex-1.1.0/mslex.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mslex
-Version: 1.0.1
+Version: 1.1.0
 Summary: shlex for windows
 Home-page: https://github.com/smoofra/mslex
 Author: Lawrence D'Anna
 Author-email: larry@elder-gods.org
 License: Apache Software License 2.0
 Keywords: mslex
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,16 +39,16 @@
 
 * Free software: Apache Software License 2.0
 * Documentation: https://mslex.readthedocs.io.
 
 Features
 --------
 
-This is the missing shlex package for windows shell quoting.   It provides two
-functions -- split and quote -- just like shlex.
+This is the missing shlex package for windows shell quoting.   It provides three
+functions -- split, quote, and join -- just like shlex.
 
 
 Credits
 -------
 
 These are excellent articles to read if you really want to face the
 sanity-melting reality buried under the surface of how windows passes command
@@ -70,14 +70,21 @@
   https://blogs.msdn.microsoft.com/twistylittlepassagesallalike/2011/04/23/everyone-quotes-command-line-arguments-the-wrong-way/
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
+Automatic selection between mslex and shlex
+-------------------------------------------
+
+If you want to automatically use mslex on Windows, and shlex otherwise, check out the `oslex`_ package.
+
+.. _`oslex`: https://pypi.org/project/oslex/
+
 
 =======
 History
 =======
 
 0.1.0 (2019-10-02)
 ------------------
```

### Comparing `mslex-1.0.1/mslex.py` & `mslex-1.1.0/mslex/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 import itertools
 
 from typing import Iterator, List, Match, TextIO
 
 __all__ = ('split', 'quote')
 
-__version__ = '1.0.1'
+__version__ = '1.1.0'
 
 def iter_arg(peek: Match[str], i: Iterator[Match[str]]) -> Iterator[str]:
     quote_mode = False
     for m in itertools.chain([peek], i):
         space, slashes, quotes, text = m.groups()
         if space:
             if quote_mode:
@@ -136,14 +136,33 @@
                 else:
                     yield onlyslashes
             else:
                 yield text
         yield '"'
     return ''.join(parts())
 
+def join(split_command: List[str], for_cmd: bool = True) -> str:
+    """
+    Quote and concatenate a list of strings for use as a command line in DOS or Windows.
+
+    On windows, before a command line argument becomes a char* in a
+    program's argv, it must be parsed by both cmd.exe, and by
+    CommandLineToArgvW.
+
+    If for_cmd is true, then this will quote the strings so the result will
+    be parsed correctly by cmd.exe and then by CommandLineToArgvW.
+
+    If for_cmd is false, then this will quote the strings so the result will
+    be parsed correctly when passed directly to CommandLineToArgvW.
+
+    For some strings there is no way to quote them so they will
+    parse correctly in both situations.
+    """
+    return ' '.join(quote(arg, for_cmd) for arg in split_command)
+
 def split_cli() -> None:
     import argparse
 
     parser = argparse.ArgumentParser(
         description='split a file into strings using windows-style quoting ')
     parser.add_argument('filename', nargs='?',
                         help='file to split')
```

### Comparing `mslex-1.0.1/setup.py` & `mslex-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     },
     install_requires=requirements,
     license="Apache Software License 2.0",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='mslex',
     name='mslex',
-    py_modules=['mslex'],
+    package_data={'mslex': ['py.typed']},
+    packages=['mslex'],
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/smoofra/mslex',
-    version='1.0.1',
+    version='1.1.0',
     zip_safe=False,
 )
```

### Comparing `mslex-1.0.1/tests/test_mslex.py` & `mslex-1.1.0/tests/test_mslex.py`

 * *Files identical despite different names*

