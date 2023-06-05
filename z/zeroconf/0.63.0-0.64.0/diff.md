# Comparing `tmp/zeroconf-0.63.0.tar.gz` & `tmp/zeroconf-0.64.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.63.0.tar", max compression
+gzip compressed data, was "zeroconf-0.64.0.tar", max compression
```

## Comparing `zeroconf-0.63.0.tar` & `zeroconf-0.64.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    51686 2023-05-25 13:00:19.908389 zeroconf-0.63.0/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-05-25 13:00:19.112391 zeroconf-0.63.0/COPYING
--rw-r--r--   0        0        0     4407 2023-05-25 13:00:19.112391 zeroconf-0.63.0/README.rst
--rw-r--r--   0        0        0     1060 2023-05-25 13:00:19.112391 zeroconf-0.63.0/build_ext.py
--rw-r--r--   0        0        0     6770 2023-05-25 13:00:19.112391 zeroconf-0.63.0/docs/Makefile
--rw-r--r--   0        0        0      234 2023-05-25 13:00:19.112391 zeroconf-0.63.0/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-05-25 13:00:19.112391 zeroconf-0.63.0/docs/conf.py
--rw-r--r--   0        0        0      991 2023-05-25 13:00:19.112391 zeroconf-0.63.0/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-05-25 13:00:19.996389 zeroconf-0.63.0/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-05-25 13:00:19.928389 zeroconf-0.63.0/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      545 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0     8567 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39051 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2061 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18218 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    25955 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2573 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    13999 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     1950 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17758 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2355 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    22413 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    25426 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3948 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6904 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4469 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-05-25 13:00:19.116391 zeroconf-0.63.0/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-05-25 13:00:19.116391 zeroconf-0.63.0/tests/__init__.py
--rw-r--r--   0        0        0      668 2023-05-25 13:00:19.116391 zeroconf-0.63.0/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-05-25 13:00:19.116391 zeroconf-0.63.0/tests/services/__init__.py
--rw-r--r--   0        0        0    42950 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/services/test_browser.py
--rw-r--r--   0        0        0    45244 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/services/test_info.py
--rw-r--r--   0        0        0     4157 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/services/test_registry.py
--rw-r--r--   0        0        0     6273 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/services/test_types.py
--rw-r--r--   0        0        0    45016 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_cache.py
--rw-r--r--   0        0        0    29468 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_dns.py
--rw-r--r--   0        0        0     5022 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_exceptions.py
--rw-r--r--   0        0        0    67458 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_protocol.py
--rw-r--r--   0        0        0     9477 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-05-25 13:00:19.120391 zeroconf-0.63.0/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.63.0/setup.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.63.0/PKG-INFO
+-rw-r--r--   0        0        0    52250 2023-06-05 00:23:51.922415 zeroconf-0.64.0/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-06-05 00:23:51.126400 zeroconf-0.64.0/COPYING
+-rw-r--r--   0        0        0     4407 2023-06-05 00:23:51.126400 zeroconf-0.64.0/README.rst
+-rw-r--r--   0        0        0     1060 2023-06-05 00:23:51.126400 zeroconf-0.64.0/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-06-05 00:23:51.126400 zeroconf-0.64.0/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-06-05 00:23:51.126400 zeroconf-0.64.0/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-06-05 00:23:51.126400 zeroconf-0.64.0/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-06-05 00:23:51.126400 zeroconf-0.64.0/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-06-05 00:23:52.006417 zeroconf-0.64.0/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-06-05 00:23:51.942416 zeroconf-0.64.0/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      897 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0    10036 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39337 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2061 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18218 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    24031 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2661 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    14335 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     1950 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17758 2023-06-05 00:23:51.126400 zeroconf-0.64.0/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2355 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    22413 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    26716 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3948 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6904 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4515 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-06-05 00:23:51.130400 zeroconf-0.64.0/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/services/__init__.py
+-rw-r--r--   0        0        0    42949 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/services/test_browser.py
+-rw-r--r--   0        0        0    45240 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/services/test_info.py
+-rw-r--r--   0        0        0     4157 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/services/test_registry.py
+-rw-r--r--   0        0        0     4681 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/services/test_types.py
+-rw-r--r--   0        0        0    44525 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_cache.py
+-rw-r--r--   0        0        0    32162 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_dns.py
+-rw-r--r--   0        0        0     5021 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    67411 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     8849 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-06-05 00:23:51.130400 zeroconf-0.64.0/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.64.0/setup.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.64.0/PKG-INFO
```

### Comparing `zeroconf-0.63.0/CHANGELOG.md` & `zeroconf-0.64.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.64.0 (2023-06-05)
+### Feature
+* Speed up processing incoming records ([#1179](https://github.com/python-zeroconf/python-zeroconf/issues/1179)) ([`d919316`](https://github.com/python-zeroconf/python-zeroconf/commit/d9193160b05beeca3755e19fd377ba13fe37b071))
+
+### Fix
+* Always answer QU questions when the exact same packet is received from different sources in sequence ([#1178](https://github.com/python-zeroconf/python-zeroconf/issues/1178)) ([`74d7ba1`](https://github.com/python-zeroconf/python-zeroconf/commit/74d7ba1aeeae56be087ee8142ee6ca1219744baa))
+
 ## v0.63.0 (2023-05-25)
 ### Feature
 * Small speed up to fetch dns addresses from ServiceInfo ([#1176](https://github.com/python-zeroconf/python-zeroconf/issues/1176)) ([`4deaa6e`](https://github.com/python-zeroconf/python-zeroconf/commit/4deaa6ed7c9161db55bf16ec068ab7260bbd4976))
 * Speed up the service registry ([#1174](https://github.com/python-zeroconf/python-zeroconf/issues/1174)) ([`360ceb2`](https://github.com/python-zeroconf/python-zeroconf/commit/360ceb2548c4c4974ff798aac43a6fff9803ea0e))
 * Improve dns cache performance ([#1172](https://github.com/python-zeroconf/python-zeroconf/issues/1172)) ([`bb496a1`](https://github.com/python-zeroconf/python-zeroconf/commit/bb496a1dd5fa3562c0412cb064d14639a542592e))
 
 ## v0.62.0 (2023-05-04)
```

### Comparing `zeroconf-0.63.0/COPYING` & `zeroconf-0.64.0/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/README.rst` & `zeroconf-0.64.0/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/build_ext.py` & `zeroconf-0.64.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/docs/Makefile` & `zeroconf-0.64.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/docs/conf.py` & `zeroconf-0.64.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/docs/index.rst` & `zeroconf-0.64.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/pyproject.toml` & `zeroconf-0.64.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.63.0"
+version = "0.64.0"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.63.0/src/zeroconf/__init__.py` & `zeroconf-0.64.0/src/zeroconf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.63.0'
+__version__ = '0.64.0'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.63.0/src/zeroconf/_cache.py` & `zeroconf-0.64.0/src/zeroconf/_cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,34 +17,36 @@
     You should have received a copy of the GNU Lesser General Public
     License along with this library; if not, write to the Free Software
     Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301
     USA
 """
 
 import itertools
-from typing import Dict, Iterable, Iterator, List, Optional, Union, cast
+from typing import Dict, Iterable, List, Optional, Set, Tuple, Union, cast
 
 from ._dns import (
     DNSAddress,
     DNSEntry,
     DNSHinfo,
     DNSNsec,
     DNSPointer,
     DNSRecord,
     DNSService,
     DNSText,
 )
 from ._utils.time import current_time_millis
-from .const import _TYPE_PTR
+from .const import _ONE_SECOND, _TYPE_PTR
 
 _UNIQUE_RECORD_TYPES = (DNSAddress, DNSHinfo, DNSPointer, DNSText, DNSService)
 _UniqueRecordsType = Union[DNSAddress, DNSHinfo, DNSPointer, DNSText, DNSService]
 _DNSRecordCacheType = Dict[str, Dict[DNSRecord, DNSRecord]]
 _DNSRecord = DNSRecord
 _str = str
+_float = float
+_int = int
 
 
 def _remove_key(cache: _DNSRecordCacheType, key: _str, record: _DNSRecord) -> None:
     """Remove a key from a DNSRecord cache
 
     This function must be run in from event loop.
     """
@@ -130,27 +132,37 @@
         the event loop.
         """
         store = self.cache.get(entry.key)
         if store is None:
             return None
         return store.get(entry)
 
-    def async_all_by_details(self, name: _str, type_: int, class_: int) -> Iterator[DNSRecord]:
+    def async_all_by_details(self, name: _str, type_: int, class_: int) -> Iterable[DNSRecord]:
         """Gets all matching entries by details.
 
-        This function is not threadsafe and must be called from
+        This function is not thread-safe and must be called from
+        the event loop.
+        """
+        return self._async_all_by_details(name, type_, class_)
+
+    def _async_all_by_details(self, name: _str, type_: int, class_: int) -> List[DNSRecord]:
+        """Gets all matching entries by details.
+
+        This function is not thread-safe and must be called from
         the event loop.
         """
         key = name.lower()
         records = self.cache.get(key)
+        matches: List[DNSRecord] = []
         if records is None:
-            return
-        for entry in records:
-            if _dns_record_matches(entry, key, type_, class_):
-                yield entry
+            return matches
+        for record in records:
+            if _dns_record_matches(record, key, type_, class_):
+                matches.append(record)
+        return matches
 
     def async_entries_with_name(self, name: str) -> Dict[DNSRecord, DNSRecord]:
         """Returns a dict of entries whose key matches the name.
 
         This function is not threadsafe and must be called from
         the event loop.
         """
@@ -222,10 +234,29 @@
                 return record
         return None
 
     def names(self) -> List[str]:
         """Return a copy of the list of current cache names."""
         return list(self.cache)
 
+    def async_mark_unique_records_older_than_1s_to_expire(
+        self, unique_types: Set[Tuple[_str, _int, _int]], answers: Iterable[DNSRecord], now: _float
+    ) -> None:
+        self._async_mark_unique_records_older_than_1s_to_expire(unique_types, answers, now)
+
+    def _async_mark_unique_records_older_than_1s_to_expire(
+        self, unique_types: Set[Tuple[_str, _int, _int]], answers: Iterable[DNSRecord], now: _float
+    ) -> None:
+        # rfc6762#section-10.2 para 2
+        # Since unique is set, all old records with that name, rrtype,
+        # and rrclass that were received more than one second ago are declared
+        # invalid, and marked to expire from the cache in one second.
+        answers_rrset = set(answers)
+        for name, type_, class_ in unique_types:
+            for record in self._async_all_by_details(name, type_, class_):
+                if (now - record.created > _ONE_SECOND) and record not in answers_rrset:
+                    # Expire in 1s
+                    record.set_created_ttl(now, 1)
+
 
 def _dns_record_matches(record: _DNSRecord, key: _str, type_: int, class_: int) -> bool:
     return key == record.key and type_ == record.type and class_ == record.class_
```

### Comparing `zeroconf-0.63.0/src/zeroconf/_core.py` & `zeroconf-0.64.0/src/zeroconf/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 )
 from ._utils.time import current_time_millis, millis_to_seconds
 from .const import (
     _CACHE_CLEANUP_INTERVAL,
     _CHECK_TIME,
     _CLASS_IN,
     _CLASS_UNIQUE,
+    _DUPLICATE_PACKET_SUPPRESSION_INTERVAL,
     _FLAGS_AA,
     _FLAGS_QR_QUERY,
     _FLAGS_QR_RESPONSE,
     _MAX_MSG_ABSOLUTE,
     _MDNS_ADDR,
     _MDNS_ADDR6,
     _MDNS_PORT,
@@ -255,89 +256,94 @@
 
     __slots__ = ('zc', 'data', 'last_time', 'transport', 'sock_description', '_deferred', '_timers')
 
     def __init__(self, zc: 'Zeroconf') -> None:
         self.zc = zc
         self.data: Optional[bytes] = None
         self.last_time: float = 0
+        self.last_message: Optional[DNSIncoming] = None
         self.transport: Optional[_WrappedTransport] = None
         self.sock_description: Optional[str] = None
         self._deferred: Dict[str, List[DNSIncoming]] = {}
         self._timers: Dict[str, asyncio.TimerHandle] = {}
         super().__init__()
 
-    def suppress_duplicate_packet(self, data: bytes, now: float) -> bool:
-        """Suppress duplicate packet if the last one was the same in the last second."""
-        if self.data == data and (now - 1000) < self.last_time:
-            return True
-        self.data = data
-        self.last_time = now
-        return False
-
     def datagram_received(
         self, data: bytes, addrs: Union[Tuple[str, int], Tuple[str, int, int, int]]
     ) -> None:
         assert self.transport is not None
         v6_flow_scope: Union[Tuple[()], Tuple[int, int]] = ()
         data_len = len(data)
+        debug = log.isEnabledFor(logging.DEBUG)
 
         if len(addrs) == 2:
             # https://github.com/python/mypy/issues/1178
             addr, port = addrs  # type: ignore
             scope = None
         else:
             # https://github.com/python/mypy/issues/1178
             addr, port, flow, scope = addrs  # type: ignore
             log.debug('IPv6 scope_id %d associated to the receiving interface', scope)
             v6_flow_scope = (flow, scope)
 
-        now = current_time_millis()
-        if self.suppress_duplicate_packet(data, now):
-            # Guard against duplicate packets
-            log.debug(
-                'Ignoring duplicate message received from %r:%r [socket %s] (%d bytes) as [%r]',
-                addr,
-                port,
-                self.sock_description,
-                data_len,
-                data,
-            )
-            return
-
         if data_len > _MAX_MSG_ABSOLUTE:
             # Guard against oversized packets to ensure bad implementations cannot overwhelm
             # the system.
             log.debug(
                 "Discarding incoming packet with length %s, which is larger "
                 "than the absolute maximum size of %s",
                 data_len,
                 _MAX_MSG_ABSOLUTE,
             )
             return
 
+        now = current_time_millis()
+        if (
+            self.data == data
+            and (now - _DUPLICATE_PACKET_SUPPRESSION_INTERVAL) < self.last_time
+            and self.last_message is not None
+            and not self.last_message.has_qu_question()
+        ):
+            # Guard against duplicate packets
+            if debug:
+                log.debug(
+                    'Ignoring duplicate message with no unicast questions received from %r:%r [socket %s] (%d bytes) as [%r]',
+                    addr,
+                    port,
+                    self.sock_description,
+                    data_len,
+                    data,
+                )
+            return
+
         msg = DNSIncoming(data, (addr, port), scope, now)
+        self.data = data
+        self.last_time = now
+        self.last_message = msg
         if msg.valid:
-            log.debug(
-                'Received from %r:%r [socket %s]: %r (%d bytes) as [%r]',
-                addr,
-                port,
-                self.sock_description,
-                msg,
-                data_len,
-                data,
-            )
+            if debug:
+                log.debug(
+                    'Received from %r:%r [socket %s]: %r (%d bytes) as [%r]',
+                    addr,
+                    port,
+                    self.sock_description,
+                    msg,
+                    data_len,
+                    data,
+                )
         else:
-            log.debug(
-                'Received from %r:%r [socket %s]: (%d bytes) [%r]',
-                addr,
-                port,
-                self.sock_description,
-                data_len,
-                data,
-            )
+            if debug:
+                log.debug(
+                    'Received from %r:%r [socket %s]: (%d bytes) [%r]',
+                    addr,
+                    port,
+                    self.sock_description,
+                    data_len,
+                    data,
+                )
             return
 
         if not msg.is_query():
             self.zc.handle_response(msg)
             return
 
         self.handle_query_or_defer(msg, addr, port, self.transport, v6_flow_scope)
@@ -718,16 +724,16 @@
         now = current_time_millis()
         other_ttl = info.other_ttl if override_ttl is None else override_ttl
         host_ttl = info.host_ttl if override_ttl is None else override_ttl
         out.add_answer_at_time(info.dns_pointer(override_ttl=other_ttl, created=now), 0)
         out.add_answer_at_time(info.dns_service(override_ttl=host_ttl, created=now), 0)
         out.add_answer_at_time(info.dns_text(override_ttl=other_ttl, created=now), 0)
         if broadcast_addresses:
-            for dns_address in info.dns_addresses(override_ttl=host_ttl, created=now):
-                out.add_answer_at_time(dns_address, 0)
+            for record in info.get_address_and_nsec_records(override_ttl=host_ttl, created=now):
+                out.add_answer_at_time(record, 0)
 
     def unregister_service(self, info: ServiceInfo) -> None:
         """Unregister a service.
 
         While it is not expected during normal operation,
         this function may raise EventLoopBlocked if the underlying
         call to `async_unregister_service` cannot be completed.
```

### Comparing `zeroconf-0.63.0/src/zeroconf/_dns.pxd` & `zeroconf-0.64.0/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_dns.py` & `zeroconf-0.64.0/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_exceptions.py` & `zeroconf-0.64.0/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_handlers.py` & `zeroconf-0.64.0/src/zeroconf/_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,38 +22,35 @@
 
 import itertools
 import random
 from collections import deque
 from typing import (
     TYPE_CHECKING,
     Dict,
-    Iterable,
     List,
     NamedTuple,
     Optional,
     Set,
     Tuple,
     Union,
     cast,
 )
 
 from ._cache import DNSCache, _UniqueRecordsType
-from ._dns import DNSAddress, DNSNsec, DNSPointer, DNSQuestion, DNSRecord, DNSRRSet
+from ._dns import DNSAddress, DNSPointer, DNSQuestion, DNSRecord, DNSRRSet
 from ._history import QuestionHistory
 from ._logger import log
 from ._protocol.incoming import DNSIncoming
 from ._protocol.outgoing import DNSOutgoing
-from ._services.info import ServiceInfo
 from ._services.registry import ServiceRegistry
 from ._updates import RecordUpdate, RecordUpdateListener
 from ._utils.time import current_time_millis, millis_to_seconds
 from .const import (
     _ADDRESS_RECORD_TYPES,
     _CLASS_IN,
-    _CLASS_UNIQUE,
     _DNS_OTHER_TTL,
     _DNS_PTR_MIN_TTL,
     _FLAGS_AA,
     _FLAGS_QR_RESPONSE,
     _ONE_SECOND,
     _SERVICE_TYPE_ENUMERATION_NAME,
     _TYPE_A,
@@ -86,23 +83,14 @@
     """A group of answers scheduled to be sent at the same time."""
 
     send_after: float  # Must be sent after this time
     send_before: float  # Must be sent before this time
     answers: _AnswerWithAdditionalsType
 
 
-def construct_nsec_record(name: str, types: List[int], now: float) -> DNSNsec:
-    """Construct an NSEC record for name and a list of dns types.
-
-    This function should only be used for SRV/A/AAAA records
-    which have a TTL of _DNS_OTHER_TTL
-    """
-    return DNSNsec(name, _TYPE_NSEC, _CLASS_IN | _CLASS_UNIQUE, _DNS_OTHER_TTL, name, types, created=now)
-
-
 def construct_outgoing_multicast_answers(answers: _AnswerWithAdditionalsType) -> DNSOutgoing:
     """Add answers and additionals to a DNSOutgoing."""
     out = DNSOutgoing(_FLAGS_QR_RESPONSE | _FLAGS_AA, multicast=True)
     _add_answers_additionals(out, answers)
     return out
 
 
@@ -213,28 +201,14 @@
         Protect the network against excessive packet flooding
         https://datatracker.ietf.org/doc/html/rfc6762#section-14
         """
         maybe_entry = self._cache.async_get_unique(cast(_UniqueRecordsType, record))
         return bool(maybe_entry and self._now - maybe_entry.created < _ONE_SECOND)
 
 
-def _get_address_and_nsec_records(service: ServiceInfo, now: float) -> Set[DNSRecord]:
-    """Build a set of address records and NSEC records for non-present record types."""
-    seen_types: Set[int] = set()
-    records: Set[DNSRecord] = set()
-    for dns_address in service.dns_addresses(created=now):
-        seen_types.add(dns_address.type)
-        records.add(dns_address)
-    missing_types: Set[int] = _ADDRESS_RECORD_TYPES - seen_types
-    if missing_types:
-        assert service.server is not None, "Service server must be set for NSEC record."
-        records.add(construct_nsec_record(service.server, list(missing_types), now))
-    return records
-
-
 class QueryHandler:
     """Query the ServiceRegistry."""
 
     def __init__(self, registry: ServiceRegistry, cache: DNSCache, question_history: QuestionHistory) -> None:
         """Init the query handler."""
         self.registry = registry
         self.cache = cache
@@ -260,17 +234,18 @@
         """Answer PTR/ANY question."""
         for service in self.registry.async_get_infos_type(lower_name):
             # Add recommended additional answers according to
             # https://tools.ietf.org/html/rfc6763#section-12.1.
             dns_pointer = service.dns_pointer(created=now)
             if known_answers.suppresses(dns_pointer):
                 continue
-            additionals: Set[DNSRecord] = {service.dns_service(created=now), service.dns_text(created=now)}
-            additionals |= _get_address_and_nsec_records(service, now)
-            answer_set[dns_pointer] = additionals
+            answer_set[dns_pointer] = {
+                service.dns_service(created=now),
+                service.dns_text(created=now),
+            } | service.get_address_and_nsec_records(created=now)
 
     def _add_address_answers(
         self,
         lower_name: str,
         answer_set: _AnswerWithAdditionalsType,
         known_answers: DNSRRSet,
         now: float,
@@ -287,20 +262,20 @@
                     additionals.add(dns_address)
                 elif not known_answers.suppresses(dns_address):
                     answers.append(dns_address)
             missing_types: Set[int] = _ADDRESS_RECORD_TYPES - seen_types
             if answers:
                 if missing_types:
                     assert service.server is not None, "Service server must be set for NSEC record."
-                    additionals.add(construct_nsec_record(service.server, list(missing_types), now))
+                    additionals.add(service.dns_nsec(list(missing_types), created=now))
                 for answer in answers:
                     answer_set[answer] = additionals
             elif type_ in missing_types:
                 assert service.server is not None, "Service server must be set for NSEC record."
-                answer_set[construct_nsec_record(service.server, list(missing_types), now)] = set()
+                answer_set[service.dns_nsec(list(missing_types), created=now)] = set()
 
     def _answer_question(
         self,
         question: DNSQuestion,
         known_answers: DNSRRSet,
         now: float,
     ) -> _AnswerWithAdditionalsType:
@@ -323,15 +298,15 @@
             service = self.registry.async_get_info_name(question_lower_name)
             if service is not None:
                 if type_ in (_TYPE_SRV, _TYPE_ANY):
                     # Add recommended additional answers according to
                     # https://tools.ietf.org/html/rfc6763#section-12.2.
                     dns_service = service.dns_service(created=now)
                     if not known_answers.suppresses(dns_service):
-                        answer_set[dns_service] = _get_address_and_nsec_records(service, now)
+                        answer_set[dns_service] = service.get_address_and_nsec_records(created=now)
                 if type_ in (_TYPE_TXT, _TYPE_ANY):
                     dns_text = service.dns_text(created=now)
                     if not known_answers.suppresses(dns_text):
                         answer_set[dns_text] = set()
 
         return answer_set
 
@@ -441,15 +416,15 @@
             # This is likely a goodbye since the record is
             # expired and exists in the cache
             elif maybe_entry is not None:
                 updates.append(RecordUpdate(record, maybe_entry))
                 removes.add(record)
 
         if unique_types:
-            self._async_mark_unique_cached_records_older_than_1s_to_expire(unique_types, msg.answers, now)
+            self.cache.async_mark_unique_records_older_than_1s_to_expire(unique_types, msg.answers, now)
 
         if updates:
             self.async_updates(now, updates)
         # The cache adds must be processed AFTER we trigger
         # the updates since we compare existing data
         # with the new data and updating the cache
         # ahead of update_record will cause listeners
@@ -471,36 +446,22 @@
         # ServiceInfo could generate an un-needed query
         # because the data was not yet populated.
         if removes:
             self.cache.async_remove_records(removes)
         if updates:
             self.async_updates_complete(new)
 
-    def _async_mark_unique_cached_records_older_than_1s_to_expire(
-        self, unique_types: Set[Tuple[str, int, int]], answers: Iterable[DNSRecord], now: float
-    ) -> None:
-        # rfc6762#section-10.2 para 2
-        # Since unique is set, all old records with that name, rrtype,
-        # and rrclass that were received more than one second ago are declared
-        # invalid, and marked to expire from the cache in one second.
-        answers_rrset = set(answers)
-        for name, type_, class_ in unique_types:
-            for entry in self.cache.async_all_by_details(name, type_, class_):
-                if (now - entry.created > _ONE_SECOND) and entry not in answers_rrset:
-                    # Expire in 1s
-                    entry.set_created_ttl(now, 1)
-
     def async_add_listener(
         self, listener: RecordUpdateListener, question: Optional[Union[DNSQuestion, List[DNSQuestion]]]
     ) -> None:
         """Adds a listener for a given question.  The listener will have
         its update_record method called when information is available to
         answer the question(s).
 
-        This function is not threadsafe and must be called in the eventloop.
+        This function is not thread-safe and must be called in the eventloop.
         """
         if not isinstance(listener, RecordUpdateListener):
             log.error(  # type: ignore[unreachable]
                 "listeners passed to async_add_listener must inherit from RecordUpdateListener;"
                 " In the future this will fail"
             )
```

### Comparing `zeroconf-0.63.0/src/zeroconf/_history.py` & `zeroconf-0.64.0/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_logger.py` & `zeroconf-0.64.0/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.64.0/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.64.0/src/zeroconf/_protocol/incoming.pxd`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,19 @@
     cdef public cython.uint num_additionals
     cdef public object valid
     cdef public object now
     cdef public object scope_id
     cdef public object source
 
     @cython.locals(
+        question=DNSQuestion
+    )
+    cpdef has_qu_question(self)
+
+    @cython.locals(
         off=cython.uint,
         label_idx=cython.uint,
         length=cython.uint,
         link=cython.uint,
         link_data=cython.uint
     )
     cdef _decode_labels_at_offset(self, unsigned int off, cython.list labels, cython.set seen_pointers)
```

### Comparing `zeroconf-0.63.0/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.64.0/src/zeroconf/_protocol/incoming.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,24 @@
         """Returns true if this is a query."""
         return (self.flags & _FLAGS_QR_MASK) == _FLAGS_QR_QUERY
 
     def is_response(self) -> bool:
         """Returns true if this is a response."""
         return (self.flags & _FLAGS_QR_MASK) == _FLAGS_QR_RESPONSE
 
+    def has_qu_question(self) -> bool:
+        """Returns true if any question is a QU question."""
+        if not self.num_questions:
+            return False
+        for question in self.questions:
+            # QU questions use the same bit as unique
+            if question.unique:
+                return True
+        return False
+
     @property
     def truncated(self) -> bool:
         """Returns true if this is a truncated."""
         return (self.flags & _FLAGS_TC) == _FLAGS_TC
 
     def _initial_parse(self) -> None:
         """Parse the data needed to initalize the packet object."""
```

### Comparing `zeroconf-0.63.0/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.64.0/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.64.0/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_services/__init__.py` & `zeroconf-0.64.0/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_services/browser.py` & `zeroconf-0.64.0/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_services/info.py` & `zeroconf-0.64.0/src/zeroconf/_services/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,19 @@
     USA
 """
 
 import asyncio
 import ipaddress
 import random
 from functools import lru_cache
-from typing import TYPE_CHECKING, Dict, List, Optional, Union, cast
+from typing import TYPE_CHECKING, Dict, List, Optional, Set, Union, cast
 
 from .._dns import (
     DNSAddress,
+    DNSNsec,
     DNSPointer,
     DNSQuestionType,
     DNSRecord,
     DNSService,
     DNSText,
 )
 from .._exceptions import BadTypeInNameException
@@ -43,22 +44,24 @@
     run_coro_with_timeout,
     wait_event_or_timeout,
 )
 from .._utils.name import service_type_name
 from .._utils.net import IPVersion, _encode_address
 from .._utils.time import current_time_millis, millis_to_seconds
 from ..const import (
+    _ADDRESS_RECORD_TYPES,
     _CLASS_IN,
     _CLASS_UNIQUE,
     _DNS_HOST_TTL,
     _DNS_OTHER_TTL,
     _FLAGS_QR_QUERY,
     _LISTENER_TIME,
     _TYPE_A,
     _TYPE_AAAA,
+    _TYPE_NSEC,
     _TYPE_PTR,
     _TYPE_SRV,
     _TYPE_TXT,
 )
 
 # https://datatracker.ietf.org/doc/html/rfc6762#section-5.2
 # The most common case for calling ServiceInfo is from a
@@ -526,14 +529,43 @@
             _TYPE_TXT,
             _CLASS_IN | _CLASS_UNIQUE,
             override_ttl if override_ttl is not None else self.other_ttl,
             self.text,
             created,
         )
 
+    def dns_nsec(
+        self, missing_types: List[int], override_ttl: Optional[int] = None, created: Optional[float] = None
+    ) -> DNSNsec:
+        """Return DNSNsec from ServiceInfo."""
+        return DNSNsec(
+            self.name,
+            _TYPE_NSEC,
+            _CLASS_IN | _CLASS_UNIQUE,
+            override_ttl if override_ttl is not None else self.host_ttl,
+            self.name,
+            missing_types,
+            created,
+        )
+
+    def get_address_and_nsec_records(
+        self, override_ttl: Optional[int] = None, created: Optional[float] = None
+    ) -> Set[DNSRecord]:
+        """Build a set of address records and NSEC records for non-present record types."""
+        seen_types: Set[int] = set()
+        records: Set[DNSRecord] = set()
+        for dns_address in self.dns_addresses(override_ttl, IPVersion.All, created):
+            seen_types.add(dns_address.type)
+            records.add(dns_address)
+        missing_types: Set[int] = _ADDRESS_RECORD_TYPES - seen_types
+        if missing_types:
+            assert self.server is not None, "Service server must be set for NSEC record."
+            records.add(self.dns_nsec(list(missing_types), override_ttl, created))
+        return records
+
     def _get_address_records_from_cache_by_type(self, zc: 'Zeroconf', _type: int) -> List[DNSAddress]:
         """Get the addresses from the cache."""
         if self.server_key is None:
             return []
         return cast("List[DNSAddress]", zc.cache.get_all_by_details(self.server_key, _type, _CLASS_IN))
 
     def set_server_if_missing(self) -> None:
```

### Comparing `zeroconf-0.63.0/src/zeroconf/_services/registry.py` & `zeroconf-0.64.0/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_services/types.py` & `zeroconf-0.64.0/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_updates.py` & `zeroconf-0.64.0/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_utils/__init__.py` & `zeroconf-0.64.0/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.64.0/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_utils/name.py` & `zeroconf-0.64.0/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_utils/net.py` & `zeroconf-0.64.0/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/_utils/time.py` & `zeroconf-0.64.0/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/asyncio.py` & `zeroconf-0.64.0/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/src/zeroconf/const.py` & `zeroconf-0.64.0/src/zeroconf/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 _UNREGISTER_TIME = 125  # ms
 _CHECK_TIME = 175  # ms
 _REGISTER_TIME = 225  # ms
 _LISTENER_TIME = 200  # ms
 _BROWSER_TIME = 1000  # ms
 _DUPLICATE_QUESTION_INTERVAL = _BROWSER_TIME - 1  # ms
+_DUPLICATE_PACKET_SUPPRESSION_INTERVAL = 1000
 _BROWSER_BACKOFF_LIMIT = 3600  # s
 _CACHE_CLEANUP_INTERVAL = 10  # s
 _LOADED_SYSTEM_TIMEOUT = 10  # s
 _STARTUP_TIMEOUT = 9  # s must be lower than _LOADED_SYSTEM_TIMEOUT
 _ONE_SECOND = 1000  # ms
 
 # If the system is loaded or the event
```

### Comparing `zeroconf-0.63.0/tests/__init__.py` & `zeroconf-0.64.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/services/__init__.py` & `zeroconf-0.64.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/services/test_browser.py` & `zeroconf-0.64.0/tests/services/test_browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,14 @@
                         socket.AF_INET6, service_v6_second_address
                     ) in service_info.addresses_by_version(r.IPVersion.V6Only)
                 assert service_info.text == service_text
                 assert service_info.server.lower() == service_server.lower()
                 service_updated_event.set()
 
         def mock_incoming_msg(service_state_change: r.ServiceStateChange) -> r.DNSIncoming:
-
             generated = r.DNSOutgoing(const._FLAGS_QR_RESPONSE)
             assert generated.is_response() is True
 
             if service_state_change == r.ServiceStateChange.Removed:
                 ttl = 0
             else:
                 ttl = 120
@@ -327,15 +326,14 @@
             assert len(zeroconf.listeners) == 0
             zeroconf.remove_all_service_listeners()
             zeroconf.close()
 
 
 class TestServiceBrowserMultipleTypes(unittest.TestCase):
     def test_update_record(self):
-
         service_names = ['name2._type2._tcp.local.', 'name._type._tcp.local.', 'name._type._udp.local']
         service_types = ['_type2._tcp.local.', '_type._tcp.local.', '_type._udp.local.']
 
         service_added_count = 0
         service_removed_count = 0
         service_add_event = Event()
         service_removed_event = Event()
@@ -576,15 +574,15 @@
     # patch the zeroconf send
     with patch.object(zeroconf_browser, "async_send", send):
         # dummy service callback
         def on_service_state_change(zeroconf, service_type, state_change, name):
             pass
 
         browser = ServiceBrowser(zeroconf_browser, type_, [on_service_state_change], delay=5)
-        time.sleep(millis_to_seconds(_services_browser._FIRST_QUERY_DELAY_RANDOM_INTERVAL[1] + 120 + 5))
+        time.sleep(millis_to_seconds(_services_browser._FIRST_QUERY_DELAY_RANDOM_INTERVAL[1] + 120 + 50))
         try:
             assert first_outgoing.questions[0].unicast is True  # type: ignore[union-attr]
             assert second_outgoing.questions[0].unicast is False  # type: ignore[attr-defined]
         finally:
             browser.cancel()
             zeroconf_browser.close()
```

### Comparing `zeroconf-0.63.0/tests/services/test_info.py` & `zeroconf-0.64.0/tests/services/test_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,14 @@
         info.update_record(zc, now, expired_record)
         assert info.properties[b"ci"] == b"2"
         zc.close()
 
     @unittest.skipIf(not has_working_ipv6(), 'Requires IPv6')
     @unittest.skipIf(os.environ.get('SKIP_IPV6'), 'IPv6 tests disabled')
     def test_get_info_partial(self):
-
         zc = r.Zeroconf(interfaces=['127.0.0.1'])
 
         service_name = 'name._type._tcp.local.'
         service_type = '_type._tcp.local.'
         service_server = 'ash-1.local.'
         service_text = b'path=/~matt1/'
         service_address = '10.0.1.2'
@@ -220,15 +219,14 @@
             last_sent = out
             send_event.set()
 
         # patch the zeroconf send
         with patch.object(zc, "async_send", send):
 
             def mock_incoming_msg(records: Iterable[r.DNSRecord]) -> r.DNSIncoming:
-
                 generated = r.DNSOutgoing(const._FLAGS_QR_RESPONSE)
 
                 for record in records:
                     generated.add_answer_at_time(record, 0)
 
                 return r.DNSIncoming(generated.packets()[0])
 
@@ -339,15 +337,14 @@
 
             finally:
                 helper_thread.join()
                 zc.remove_all_service_listeners()
                 zc.close()
 
     def test_get_info_single(self):
-
         zc = r.Zeroconf(interfaces=['127.0.0.1'])
 
         service_name = 'name._type._tcp.local.'
         service_type = '_type._tcp.local.'
         service_server = 'ash-1.local.'
         service_text = b'path=/~matt1/'
         service_address = '10.0.1.2'
@@ -365,15 +362,14 @@
             last_sent = out
             send_event.set()
 
         # patch the zeroconf send
         with patch.object(zc, "async_send", send):
 
             def mock_incoming_msg(records: Iterable[r.DNSRecord]) -> r.DNSIncoming:
-
                 generated = r.DNSOutgoing(const._FLAGS_QR_RESPONSE)
 
                 for record in records:
                     generated.add_answer_at_time(record, 0)
 
                 return r.DNSIncoming(generated.packets()[0])
```

### Comparing `zeroconf-0.63.0/tests/services/test_registry.py` & `zeroconf-0.64.0/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/services/test_types.py` & `zeroconf-0.64.0/tests/services/test_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """Unit tests for zeroconf._services.types."""
 
 import logging
 import os
 import socket
 import sys
 import unittest
-from unittest.mock import patch
 
 import zeroconf as r
 from zeroconf import ServiceInfo, Zeroconf, ZeroconfServiceTypes
 
 from .. import _clear_cache, has_working_ipv6
 
 log = logging.getLogger('zeroconf')
@@ -26,151 +25,134 @@
 
 
 def teardown_module():
     if original_logging_level != logging.NOTSET:
         log.setLevel(original_logging_level)
 
 
-class ServiceTypesQuery(unittest.TestCase):
-    def test_integration_with_listener(self):
+def test_integration_with_listener(disable_duplicate_packet_suppression):
+    type_ = "_test-listen-type._tcp.local."
+    name = "xxxyyy"
+    registration_name = f"{name}.{type_}"
+
+    zeroconf_registrar = Zeroconf(interfaces=['127.0.0.1'])
+    desc = {'path': '/~paulsm/'}
+    info = ServiceInfo(
+        type_,
+        registration_name,
+        80,
+        0,
+        0,
+        desc,
+        "ash-2.local.",
+        addresses=[socket.inet_aton("10.0.1.2")],
+    )
+    zeroconf_registrar.registry.async_add(info)
+    try:
+
+        service_types = ZeroconfServiceTypes.find(interfaces=['127.0.0.1'], timeout=2)
+        assert type_ in service_types
+        _clear_cache(zeroconf_registrar)
+        service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
+        assert type_ in service_types
+
+    finally:
+        zeroconf_registrar.close()
+
+
+@unittest.skipIf(not has_working_ipv6(), 'Requires IPv6')
+@unittest.skipIf(os.environ.get('SKIP_IPV6'), 'IPv6 tests disabled')
+def test_integration_with_listener_v6_records(disable_duplicate_packet_suppression):
+    type_ = "_test-listenv6rec-type._tcp.local."
+    name = "xxxyyy"
+    registration_name = f"{name}.{type_}"
+    addr = "2606:2800:220:1:248:1893:25c8:1946"  # example.com
+
+    zeroconf_registrar = Zeroconf(interfaces=['127.0.0.1'])
+    desc = {'path': '/~paulsm/'}
+    info = ServiceInfo(
+        type_,
+        registration_name,
+        80,
+        0,
+        0,
+        desc,
+        "ash-2.local.",
+        addresses=[socket.inet_pton(socket.AF_INET6, addr)],
+    )
+    zeroconf_registrar.registry.async_add(info)
+    try:
+
+        service_types = ZeroconfServiceTypes.find(interfaces=['127.0.0.1'], timeout=2)
+        assert type_ in service_types
+        _clear_cache(zeroconf_registrar)
+        service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
+        assert type_ in service_types
+
+    finally:
+        zeroconf_registrar.close()
+
+
+@unittest.skipIf(not has_working_ipv6() or sys.platform == 'win32', 'Requires IPv6')
+@unittest.skipIf(os.environ.get('SKIP_IPV6'), 'IPv6 tests disabled')
+def test_integration_with_listener_ipv6(disable_duplicate_packet_suppression):
+    type_ = "_test-listenv6ip-type._tcp.local."
+    name = "xxxyyy"
+    registration_name = f"{name}.{type_}"
+    addr = "2606:2800:220:1:248:1893:25c8:1946"  # example.com
+
+    zeroconf_registrar = Zeroconf(ip_version=r.IPVersion.V6Only)
+    desc = {'path': '/~paulsm/'}
+    info = ServiceInfo(
+        type_,
+        registration_name,
+        80,
+        0,
+        0,
+        desc,
+        "ash-2.local.",
+        addresses=[socket.inet_pton(socket.AF_INET6, addr)],
+    )
+    zeroconf_registrar.registry.async_add(info)
+    try:
+
+        service_types = ZeroconfServiceTypes.find(ip_version=r.IPVersion.V6Only, timeout=2)
+        assert type_ in service_types
+        _clear_cache(zeroconf_registrar)
+        service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
+        assert type_ in service_types
+
+    finally:
+        zeroconf_registrar.close()
+
+
+def test_integration_with_subtype_and_listener(disable_duplicate_packet_suppression):
+    subtype_ = "_subtype._sub"
+    type_ = "_listen._tcp.local."
+    name = "xxxyyy"
+    # Note: discovery returns only DNS-SD type not subtype
+    discovery_type = f"{subtype_}.{type_}"
+    registration_name = f"{name}.{type_}"
+
+    zeroconf_registrar = Zeroconf(interfaces=['127.0.0.1'])
+    desc = {'path': '/~paulsm/'}
+    info = ServiceInfo(
+        discovery_type,
+        registration_name,
+        80,
+        0,
+        0,
+        desc,
+        "ash-2.local.",
+        addresses=[socket.inet_aton("10.0.1.2")],
+    )
+    zeroconf_registrar.registry.async_add(info)
+    try:
+
+        service_types = ZeroconfServiceTypes.find(interfaces=['127.0.0.1'], timeout=2)
+        assert discovery_type in service_types
+        _clear_cache(zeroconf_registrar)
+        service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
+        assert discovery_type in service_types
 
-        type_ = "_test-listen-type._tcp.local."
-        name = "xxxyyy"
-        registration_name = f"{name}.{type_}"
-
-        zeroconf_registrar = Zeroconf(interfaces=['127.0.0.1'])
-        desc = {'path': '/~paulsm/'}
-        info = ServiceInfo(
-            type_,
-            registration_name,
-            80,
-            0,
-            0,
-            desc,
-            "ash-2.local.",
-            addresses=[socket.inet_aton("10.0.1.2")],
-        )
-        zeroconf_registrar.registry.async_add(info)
-        try:
-            with patch.object(
-                zeroconf_registrar.engine.protocols[0], "suppress_duplicate_packet", return_value=False
-            ), patch.object(
-                zeroconf_registrar.engine.protocols[1], "suppress_duplicate_packet", return_value=False
-            ):
-                service_types = ZeroconfServiceTypes.find(interfaces=['127.0.0.1'], timeout=2)
-                assert type_ in service_types
-                _clear_cache(zeroconf_registrar)
-                service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
-                assert type_ in service_types
-
-        finally:
-            zeroconf_registrar.close()
-
-    @unittest.skipIf(not has_working_ipv6(), 'Requires IPv6')
-    @unittest.skipIf(os.environ.get('SKIP_IPV6'), 'IPv6 tests disabled')
-    def test_integration_with_listener_v6_records(self):
-
-        type_ = "_test-listenv6rec-type._tcp.local."
-        name = "xxxyyy"
-        registration_name = f"{name}.{type_}"
-        addr = "2606:2800:220:1:248:1893:25c8:1946"  # example.com
-
-        zeroconf_registrar = Zeroconf(interfaces=['127.0.0.1'])
-        desc = {'path': '/~paulsm/'}
-        info = ServiceInfo(
-            type_,
-            registration_name,
-            80,
-            0,
-            0,
-            desc,
-            "ash-2.local.",
-            addresses=[socket.inet_pton(socket.AF_INET6, addr)],
-        )
-        zeroconf_registrar.registry.async_add(info)
-        try:
-            with patch.object(
-                zeroconf_registrar.engine.protocols[0], "suppress_duplicate_packet", return_value=False
-            ), patch.object(
-                zeroconf_registrar.engine.protocols[1], "suppress_duplicate_packet", return_value=False
-            ):
-                service_types = ZeroconfServiceTypes.find(interfaces=['127.0.0.1'], timeout=2)
-                assert type_ in service_types
-                _clear_cache(zeroconf_registrar)
-                service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
-                assert type_ in service_types
-
-        finally:
-            zeroconf_registrar.close()
-
-    @unittest.skipIf(not has_working_ipv6() or sys.platform == 'win32', 'Requires IPv6')
-    @unittest.skipIf(os.environ.get('SKIP_IPV6'), 'IPv6 tests disabled')
-    def test_integration_with_listener_ipv6(self):
-
-        type_ = "_test-listenv6ip-type._tcp.local."
-        name = "xxxyyy"
-        registration_name = f"{name}.{type_}"
-        addr = "2606:2800:220:1:248:1893:25c8:1946"  # example.com
-
-        zeroconf_registrar = Zeroconf(ip_version=r.IPVersion.V6Only)
-        desc = {'path': '/~paulsm/'}
-        info = ServiceInfo(
-            type_,
-            registration_name,
-            80,
-            0,
-            0,
-            desc,
-            "ash-2.local.",
-            addresses=[socket.inet_pton(socket.AF_INET6, addr)],
-        )
-        zeroconf_registrar.registry.async_add(info)
-        try:
-            with patch.object(
-                zeroconf_registrar.engine.protocols[0], "suppress_duplicate_packet", return_value=False
-            ), patch.object(
-                zeroconf_registrar.engine.protocols[1], "suppress_duplicate_packet", return_value=False
-            ):
-                service_types = ZeroconfServiceTypes.find(ip_version=r.IPVersion.V6Only, timeout=2)
-                assert type_ in service_types
-                _clear_cache(zeroconf_registrar)
-                service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
-                assert type_ in service_types
-
-        finally:
-            zeroconf_registrar.close()
-
-    def test_integration_with_subtype_and_listener(self):
-        subtype_ = "_subtype._sub"
-        type_ = "_listen._tcp.local."
-        name = "xxxyyy"
-        # Note: discovery returns only DNS-SD type not subtype
-        discovery_type = f"{subtype_}.{type_}"
-        registration_name = f"{name}.{type_}"
-
-        zeroconf_registrar = Zeroconf(interfaces=['127.0.0.1'])
-        desc = {'path': '/~paulsm/'}
-        info = ServiceInfo(
-            discovery_type,
-            registration_name,
-            80,
-            0,
-            0,
-            desc,
-            "ash-2.local.",
-            addresses=[socket.inet_aton("10.0.1.2")],
-        )
-        zeroconf_registrar.registry.async_add(info)
-        try:
-            with patch.object(
-                zeroconf_registrar.engine.protocols[0], "suppress_duplicate_packet", return_value=False
-            ), patch.object(
-                zeroconf_registrar.engine.protocols[1], "suppress_duplicate_packet", return_value=False
-            ):
-                service_types = ZeroconfServiceTypes.find(interfaces=['127.0.0.1'], timeout=2)
-                assert discovery_type in service_types
-                _clear_cache(zeroconf_registrar)
-                service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
-                assert discovery_type in service_types
-
-        finally:
-            zeroconf_registrar.close()
+    finally:
+        zeroconf_registrar.close()
```

### Comparing `zeroconf-0.63.0/tests/test_asyncio.py` & `zeroconf-0.64.0/tests/test_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,15 @@
         0,
         desc,
         "ash-2.local.",
         addresses=[socket.inet_aton("10.0.1.3")],
     )
     task = await aiozc.async_update_service(new_info)
     await task
+
     task = await aiozc.async_unregister_service(new_info)
     await task
     await aiozc.async_close()
 
     assert calls == [
         ('add', type_, registration_name),
         ('update', type_, registration_name),
@@ -950,29 +951,17 @@
 
     assert len(zeroconf_registrar.engine.protocols) == 2
     # patch the zeroconf send
     # patch the zeroconf current_time_millis
     # patch the backoff limit to ensure we always get one query every 1/4 of the DNS TTL
     # Disable duplicate question suppression and duplicate packet suppression for this test as it works
     # by asking the same question over and over
-    with patch.object(
-        zeroconf_registrar.engine.protocols[0], "suppress_duplicate_packet", return_value=False
-    ), patch.object(
-        zeroconf_registrar.engine.protocols[1], "suppress_duplicate_packet", return_value=False
-    ), patch.object(
-        zeroconf_browser.engine.protocols[0], "suppress_duplicate_packet", return_value=False
-    ), patch.object(
-        zeroconf_browser.engine.protocols[1], "suppress_duplicate_packet", return_value=False
-    ), patch.object(
-        zeroconf_browser.question_history, "suppresses", return_value=False
-    ), patch.object(
+    with patch.object(zeroconf_browser.question_history, "suppresses", return_value=False), patch.object(
         zeroconf_browser, "async_send", send
-    ), patch(
-        "zeroconf._services.browser.current_time_millis", _new_current_time_millis
-    ), patch.object(
+    ), patch("zeroconf._services.browser.current_time_millis", _new_current_time_millis), patch.object(
         _services_browser, "_BROWSER_BACKOFF_LIMIT", int(expected_ttl / 4)
     ):
         service_added = asyncio.Event()
         service_removed = asyncio.Event()
 
         browser = AsyncServiceBrowser(zeroconf_browser, type_, [on_service_state_change])
```

### Comparing `zeroconf-0.63.0/tests/test_cache.py` & `zeroconf-0.64.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/test_core.py` & `zeroconf-0.64.0/tests/test_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import socket
 import sys
 import threading
 import time
 import unittest
 import unittest.mock
 from typing import Set, cast
-from unittest.mock import patch
+from unittest.mock import MagicMock, patch
 
 import pytest
 
 import zeroconf as r
 from zeroconf import NotRunningException, Zeroconf, _core, const, current_time_millis
 from zeroconf._protocol import outgoing
 from zeroconf.asyncio import AsyncZeroconf
@@ -766,23 +766,93 @@
 
 def test_guard_against_duplicate_packets():
     """Ensure we do not process duplicate packets.
     These packets can quickly overwhelm the system.
     """
     zc = Zeroconf(interfaces=['127.0.0.1'])
     listener = _core.AsyncListener(zc)
-    assert listener.suppress_duplicate_packet(b"first packet", current_time_millis()) is False
-    assert listener.suppress_duplicate_packet(b"first packet", current_time_millis()) is True
-    assert listener.suppress_duplicate_packet(b"first packet", current_time_millis()) is True
-    assert listener.suppress_duplicate_packet(b"first packet", current_time_millis() + 1000) is False
-    assert listener.suppress_duplicate_packet(b"first packet", current_time_millis()) is True
-    assert listener.suppress_duplicate_packet(b"other packet", current_time_millis()) is False
-    assert listener.suppress_duplicate_packet(b"other packet", current_time_millis()) is True
-    assert listener.suppress_duplicate_packet(b"other packet", current_time_millis() + 1000) is False
-    assert listener.suppress_duplicate_packet(b"first packet", current_time_millis()) is False
+    listener.transport = MagicMock()
+
+    query = r.DNSOutgoing(const._FLAGS_QR_QUERY, multicast=True)
+    question = r.DNSQuestion("x._http._tcp.local.", const._TYPE_PTR, const._CLASS_IN)
+    query.add_question(question)
+    packet_with_qm_question = query.packets()[0]
+
+    query3 = r.DNSOutgoing(const._FLAGS_QR_QUERY, multicast=True)
+    question3 = r.DNSQuestion("x._ay._tcp.local.", const._TYPE_PTR, const._CLASS_IN)
+    query3.add_question(question3)
+    packet_with_qm_question2 = query3.packets()[0]
+
+    query2 = r.DNSOutgoing(const._FLAGS_QR_QUERY, multicast=True)
+    question2 = r.DNSQuestion("x._http._tcp.local.", const._TYPE_PTR, const._CLASS_IN)
+    question2.unicast = True
+    query2.add_question(question2)
+    packet_with_qu_question = query2.packets()[0]
+
+    addrs = ("1.2.3.4", 43)
+
+    with patch.object(_core, "current_time_millis") as _current_time_millis, patch.object(
+        listener, "handle_query_or_defer"
+    ) as _handle_query_or_defer:
+        start_time = current_time_millis()
+
+        _current_time_millis.return_value = start_time
+        listener.datagram_received(packet_with_qm_question, addrs)
+        _handle_query_or_defer.assert_called_once()
+        _handle_query_or_defer.reset_mock()
+
+        # Now call with the same packet again and handle_query_or_defer should not fire
+        listener.datagram_received(packet_with_qm_question, addrs)
+        _handle_query_or_defer.assert_not_called()
+        _handle_query_or_defer.reset_mock()
+
+        # Now walk time forward 1000 seconds
+        _current_time_millis.return_value = start_time + 1000
+        # Now call with the same packet again and handle_query_or_defer should fire
+        listener.datagram_received(packet_with_qm_question, addrs)
+        _handle_query_or_defer.assert_called_once()
+        _handle_query_or_defer.reset_mock()
+
+        # Now call with the different packet and handle_query_or_defer should fire
+        listener.datagram_received(packet_with_qm_question2, addrs)
+        _handle_query_or_defer.assert_called_once()
+        _handle_query_or_defer.reset_mock()
+
+        # Now call with the different packet and handle_query_or_defer should fire
+        listener.datagram_received(packet_with_qm_question, addrs)
+        _handle_query_or_defer.assert_called_once()
+        _handle_query_or_defer.reset_mock()
+
+        # Now call with the different packet with qu question and handle_query_or_defer should fire
+        listener.datagram_received(packet_with_qu_question, addrs)
+        _handle_query_or_defer.assert_called_once()
+        _handle_query_or_defer.reset_mock()
+
+        # Now call again with the same packet that has a qu question and handle_query_or_defer should fire
+        listener.datagram_received(packet_with_qu_question, addrs)
+        _handle_query_or_defer.assert_called_once()
+        _handle_query_or_defer.reset_mock()
+
+        log.setLevel(logging.WARNING)
+
+        # Call with the QM packet again
+        listener.datagram_received(packet_with_qm_question, addrs)
+        _handle_query_or_defer.assert_called_once()
+        _handle_query_or_defer.reset_mock()
+
+        # Now call with the same packet again and handle_query_or_defer should not fire
+        listener.datagram_received(packet_with_qm_question, addrs)
+        _handle_query_or_defer.assert_not_called()
+        _handle_query_or_defer.reset_mock()
+
+        # Now call with garbage
+        listener.datagram_received(b'garbage', addrs)
+        _handle_query_or_defer.assert_not_called()
+        _handle_query_or_defer.reset_mock()
+
     zc.close()
 
 
 def test_shutdown_while_register_in_process():
     """Test we can shutdown while registering a service in another thread."""
 
     # instantiate a zeroconf instance
```

### Comparing `zeroconf-0.63.0/tests/test_dns.py` & `zeroconf-0.64.0/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/test_exceptions.py` & `zeroconf-0.64.0/tests/test_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 def teardown_module():
     if original_logging_level != logging.NOTSET:
         log.setLevel(original_logging_level)
 
 
 class Exceptions(unittest.TestCase):
-
     browser = None  # type: Zeroconf
 
     @classmethod
     def setUpClass(cls):
         cls.browser = Zeroconf(interfaces=['127.0.0.1'])
 
     @classmethod
```

### Comparing `zeroconf-0.63.0/tests/test_handlers.py` & `zeroconf-0.64.0/tests/test_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 def teardown_module():
     if original_logging_level != logging.NOTSET:
         log.setLevel(original_logging_level)
 
 
 class TestRegistrar(unittest.TestCase):
     def test_ttl(self):
-
         # instantiate a zeroconf instance
         zc = Zeroconf(interfaces=['127.0.0.1'])
 
         # service definition
         type_ = "_test-srvc-type._tcp.local."
         name = "xxxyyy"
         registration_name = f"{name}.{type_}"
@@ -64,15 +63,15 @@
         )
 
         nbr_answers = nbr_additionals = nbr_authorities = 0
 
         def get_ttl(record_type):
             if expected_ttl is not None:
                 return expected_ttl
-            elif record_type in [const._TYPE_A, const._TYPE_SRV]:
+            elif record_type in [const._TYPE_A, const._TYPE_SRV, const._TYPE_NSEC]:
                 return const._DNS_HOST_TTL
             else:
                 return const._DNS_OTHER_TTL
 
         def _process_outgoing_packet(out):
             """Sends an outgoing packet."""
             nonlocal nbr_answers, nbr_additionals, nbr_authorities
@@ -90,15 +89,15 @@
         # register service with default TTL
         expected_ttl = None
         for _ in range(3):
             _process_outgoing_packet(zc.generate_service_query(info))
         zc.registry.async_add(info)
         for _ in range(3):
             _process_outgoing_packet(zc.generate_service_broadcast(info, None))
-        assert nbr_answers == 12 and nbr_additionals == 0 and nbr_authorities == 3
+        assert nbr_answers == 15 and nbr_additionals == 0 and nbr_authorities == 3
         nbr_answers = nbr_additionals = nbr_authorities = 0
 
         # query
         query = r.DNSOutgoing(const._FLAGS_QR_QUERY | const._FLAGS_AA)
         assert query.is_query() is True
         query.add_question(r.DNSQuestion(info.type, const._TYPE_PTR, const._CLASS_IN))
         query.add_question(r.DNSQuestion(info.name, const._TYPE_SRV, const._CLASS_IN))
@@ -116,27 +115,27 @@
         nbr_answers = nbr_additionals = nbr_authorities = 0
 
         # unregister
         expected_ttl = 0
         zc.registry.async_remove(info)
         for _ in range(3):
             _process_outgoing_packet(zc.generate_service_broadcast(info, 0))
-        assert nbr_answers == 12 and nbr_additionals == 0 and nbr_authorities == 0
+        assert nbr_answers == 15 and nbr_additionals == 0 and nbr_authorities == 0
         nbr_answers = nbr_additionals = nbr_authorities = 0
 
         expected_ttl = None
         for _ in range(3):
             _process_outgoing_packet(zc.generate_service_query(info))
         zc.registry.async_add(info)
         # register service with custom TTL
         expected_ttl = const._DNS_HOST_TTL * 2
         assert expected_ttl != const._DNS_HOST_TTL
         for _ in range(3):
             _process_outgoing_packet(zc.generate_service_broadcast(info, expected_ttl))
-        assert nbr_answers == 12 and nbr_additionals == 0 and nbr_authorities == 3
+        assert nbr_answers == 15 and nbr_additionals == 0 and nbr_authorities == 3
         nbr_answers = nbr_additionals = nbr_authorities = 0
 
         # query
         expected_ttl = None
         query = r.DNSOutgoing(const._FLAGS_QR_QUERY | const._FLAGS_AA)
         query.add_question(r.DNSQuestion(info.type, const._TYPE_PTR, const._CLASS_IN))
         query.add_question(r.DNSQuestion(info.name, const._TYPE_SRV, const._CLASS_IN))
@@ -152,15 +151,15 @@
         nbr_answers = nbr_additionals = nbr_authorities = 0
 
         # unregister
         expected_ttl = 0
         zc.registry.async_remove(info)
         for _ in range(3):
             _process_outgoing_packet(zc.generate_service_broadcast(info, 0))
-        assert nbr_answers == 12 and nbr_additionals == 0 and nbr_authorities == 0
+        assert nbr_answers == 15 and nbr_additionals == 0 and nbr_authorities == 0
         nbr_answers = nbr_additionals = nbr_authorities = 0
         zc.close()
 
     def test_name_conflicts(self):
         # instantiate a zeroconf instance
         zc = Zeroconf(interfaces=['127.0.0.1'])
         type_ = "_homeassistant._tcp.local."
@@ -218,15 +217,14 @@
         info.load_from_cache(zc)
         assert info.addresses == [socket.inet_pton(socket.AF_INET, "1.2.3.4")]
         assert info.properties == {b"version": b"1.0"}
         zc.close()
 
 
 def test_ptr_optimization():
-
     # instantiate a zeroconf instance
     zc = Zeroconf(interfaces=['127.0.0.1'])
 
     # service definition
     type_ = "_test-srvc-type._tcp.local."
     name = "xxxyyy"
     registration_name = f"{name}.{type_}"
@@ -1463,15 +1461,15 @@
         incoming = r.DNSIncoming(outgoing.packets()[0])
         assert info.dns_pointer() in incoming.answers
 
     await aiozc.async_close()
 
 
 @pytest.mark.asyncio
-async def test_response_aggregation_timings_multiple(run_isolated):
+async def test_response_aggregation_timings_multiple(run_isolated, disable_duplicate_packet_suppression):
     """Verify multicast responses that are aggregated do not take longer than 620ms to send.
 
     620ms is the maximum random delay of 120ms and 500ms additional for aggregation."""
     type_2 = "_mservice2._tcp.local."
 
     aiozc = AsyncZeroconf(interfaces=['127.0.0.1'])
     await aiozc.zeroconf.async_wait_for_start()
@@ -1488,17 +1486,15 @@
     query2 = r.DNSOutgoing(const._FLAGS_QR_QUERY, multicast=True)
     question2 = r.DNSQuestion(info2.type, const._TYPE_PTR, const._CLASS_IN)
     query2.add_question(question2)
 
     zc = aiozc.zeroconf
     protocol = zc.engine.protocols[0]
 
-    with unittest.mock.patch.object(aiozc.zeroconf, "async_send") as send_mock, unittest.mock.patch.object(
-        protocol, "suppress_duplicate_packet", return_value=False
-    ):
+    with unittest.mock.patch.object(aiozc.zeroconf, "async_send") as send_mock:
         send_mock.reset_mock()
         protocol.datagram_received(query2.packets()[0], ('127.0.0.1', const._MDNS_PORT))
         await asyncio.sleep(0.2)
         calls = send_mock.mock_calls
         assert len(calls) == 1
         outgoing = send_mock.call_args[0][0]
         incoming = r.DNSIncoming(outgoing.packets()[0])
```

### Comparing `zeroconf-0.63.0/tests/test_history.py` & `zeroconf-0.64.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/test_init.py` & `zeroconf-0.64.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/test_logger.py` & `zeroconf-0.64.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/test_protocol.py` & `zeroconf-0.64.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/test_services.py` & `zeroconf-0.64.0/tests/test_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 import os
 import socket
 import time
 import unittest
 from threading import Event
 from typing import Dict
-from unittest.mock import patch
 
 import pytest
 
 import zeroconf as r
 from zeroconf import Zeroconf
 from zeroconf._services.info import ServiceInfo
 
@@ -33,15 +32,14 @@
 def teardown_module():
     if original_logging_level != logging.NOTSET:
         log.setLevel(original_logging_level)
 
 
 class ListenerTest(unittest.TestCase):
     def test_integration_with_listener_class(self):
-
         sub_service_added = Event()
         service_added = Event()
         service_removed = Event()
         sub_service_updated = Event()
         duplicate_service_added = Event()
 
         subtype_name = "_printer"
@@ -103,121 +101,116 @@
             addresses.append(socket.inet_pton(socket.AF_INET6, "6001:db8::1"))
             addresses.append(socket.inet_pton(socket.AF_INET6, "2001:db8::1"))
         info_service = ServiceInfo(
             subtype, registration_name, port=80, properties=desc, server="ash-2.local.", addresses=addresses
         )
         zeroconf_registrar.register_service(info_service)
 
-        with patch.object(
-            zeroconf_registrar.engine.protocols[0], "suppress_duplicate_packet", return_value=False
-        ), patch.object(
-            zeroconf_registrar.engine.protocols[1], "suppress_duplicate_packet", return_value=False
-        ):
-            try:
-                service_added.wait(1)
-                assert service_added.is_set()
-
-                # short pause to allow multicast timers to expire
-                time.sleep(3)
-
-                zeroconf_browser.add_service_listener(type_, DuplicateListener())
-                duplicate_service_added.wait(
-                    1
-                )  # Ensure a listener for the same type calls back right away from cache
-
-                # clear the answer cache to force query
-                _clear_cache(zeroconf_browser)
-
-                cached_info = ServiceInfo(type_, registration_name)
-                cached_info.load_from_cache(zeroconf_browser)
-                assert cached_info.properties == {}
-
-                # get service info without answer cache
-                info = zeroconf_browser.get_service_info(type_, registration_name)
-                assert info is not None
-                assert info.properties[b'prop_none'] is None
-                assert info.properties[b'prop_string'] == properties['prop_string']
-                assert info.properties[b'prop_float'] == b'1.0'
-                assert info.properties[b'prop_blank'] == properties['prop_blank']
-                assert info.properties[b'prop_true'] == b'1'
-                assert info.properties[b'prop_false'] == b'0'
-                assert info.addresses == addresses[:1]  # no V6 by default
-                assert set(info.addresses_by_version(r.IPVersion.All)) == set(addresses)
-
-                cached_info = ServiceInfo(type_, registration_name)
-                cached_info.load_from_cache(zeroconf_browser)
-                assert cached_info.properties is not None
-
-                # Populate the cache
-                zeroconf_browser.get_service_info(subtype, registration_name)
-
-                # get service info with only the cache
-                cached_info = ServiceInfo(subtype, registration_name)
-                cached_info.load_from_cache(zeroconf_browser)
-                assert cached_info.properties is not None
-                assert cached_info.properties[b'prop_float'] == b'1.0'
-
-                # get service info with only the cache with the lowercase name
-                cached_info = ServiceInfo(subtype, registration_name.lower())
-                cached_info.load_from_cache(zeroconf_browser)
-                # Ensure uppercase output is preserved
-                assert cached_info.name == registration_name
-                assert cached_info.key == registration_name.lower()
-                assert cached_info.properties is not None
-                assert cached_info.properties[b'prop_float'] == b'1.0'
-
-                info = zeroconf_browser.get_service_info(subtype, registration_name)
-                assert info is not None
-                assert info.properties is not None
-                assert info.properties[b'prop_none'] is None
-
-                cached_info = ServiceInfo(subtype, registration_name.lower())
-                cached_info.load_from_cache(zeroconf_browser)
-                assert cached_info.properties is not None
-                assert cached_info.properties[b'prop_none'] is None
-
-                # test TXT record update
-                sublistener = MySubListener()
-
-                zeroconf_browser.add_service_listener(subtype, sublistener)
-
-                properties['prop_blank'] = b'an updated string'
-                desc.update(properties)
-                info_service = ServiceInfo(
-                    subtype,
-                    registration_name,
-                    80,
-                    0,
-                    0,
-                    desc,
-                    "ash-2.local.",
-                    addresses=[socket.inet_aton("10.0.1.2")],
-                )
-                zeroconf_registrar.update_service(info_service)
-
-                sub_service_added.wait(1)  # we cleared the cache above
-                assert sub_service_added.is_set()
-
-                info = zeroconf_browser.get_service_info(type_, registration_name)
-                assert info is not None
-                assert info.properties[b'prop_blank'] == properties['prop_blank']
-
-                cached_info = ServiceInfo(subtype, registration_name)
-                cached_info.load_from_cache(zeroconf_browser)
-                assert cached_info.properties is not None
-                assert cached_info.properties[b'prop_blank'] == properties['prop_blank']
-
-                zeroconf_registrar.unregister_service(info_service)
-                service_removed.wait(1)
-                assert service_removed.is_set()
-
-            finally:
-                zeroconf_registrar.close()
-                zeroconf_browser.remove_service_listener(listener)
-                zeroconf_browser.close()
+        try:
+            service_added.wait(1)
+            assert service_added.is_set()
+
+            # short pause to allow multicast timers to expire
+            time.sleep(3)
+
+            zeroconf_browser.add_service_listener(type_, DuplicateListener())
+            duplicate_service_added.wait(
+                1
+            )  # Ensure a listener for the same type calls back right away from cache
+
+            # clear the answer cache to force query
+            _clear_cache(zeroconf_browser)
+
+            cached_info = ServiceInfo(type_, registration_name)
+            cached_info.load_from_cache(zeroconf_browser)
+            assert cached_info.properties == {}
+
+            # get service info without answer cache
+            info = zeroconf_browser.get_service_info(type_, registration_name)
+            assert info is not None
+            assert info.properties[b'prop_none'] is None
+            assert info.properties[b'prop_string'] == properties['prop_string']
+            assert info.properties[b'prop_float'] == b'1.0'
+            assert info.properties[b'prop_blank'] == properties['prop_blank']
+            assert info.properties[b'prop_true'] == b'1'
+            assert info.properties[b'prop_false'] == b'0'
+            assert info.addresses == addresses[:1]  # no V6 by default
+            assert set(info.addresses_by_version(r.IPVersion.All)) == set(addresses)
+
+            cached_info = ServiceInfo(type_, registration_name)
+            cached_info.load_from_cache(zeroconf_browser)
+            assert cached_info.properties is not None
+
+            # Populate the cache
+            zeroconf_browser.get_service_info(subtype, registration_name)
+
+            # get service info with only the cache
+            cached_info = ServiceInfo(subtype, registration_name)
+            cached_info.load_from_cache(zeroconf_browser)
+            assert cached_info.properties is not None
+            assert cached_info.properties[b'prop_float'] == b'1.0'
+
+            # get service info with only the cache with the lowercase name
+            cached_info = ServiceInfo(subtype, registration_name.lower())
+            cached_info.load_from_cache(zeroconf_browser)
+            # Ensure uppercase output is preserved
+            assert cached_info.name == registration_name
+            assert cached_info.key == registration_name.lower()
+            assert cached_info.properties is not None
+            assert cached_info.properties[b'prop_float'] == b'1.0'
+
+            info = zeroconf_browser.get_service_info(subtype, registration_name)
+            assert info is not None
+            assert info.properties is not None
+            assert info.properties[b'prop_none'] is None
+
+            cached_info = ServiceInfo(subtype, registration_name.lower())
+            cached_info.load_from_cache(zeroconf_browser)
+            assert cached_info.properties is not None
+            assert cached_info.properties[b'prop_none'] is None
+
+            # test TXT record update
+            sublistener = MySubListener()
+
+            zeroconf_browser.add_service_listener(subtype, sublistener)
+
+            properties['prop_blank'] = b'an updated string'
+            desc.update(properties)
+            info_service = ServiceInfo(
+                subtype,
+                registration_name,
+                80,
+                0,
+                0,
+                desc,
+                "ash-2.local.",
+                addresses=[socket.inet_aton("10.0.1.2")],
+            )
+            zeroconf_registrar.update_service(info_service)
+
+            sub_service_added.wait(1)  # we cleared the cache above
+            assert sub_service_added.is_set()
+
+            info = zeroconf_browser.get_service_info(type_, registration_name)
+            assert info is not None
+            assert info.properties[b'prop_blank'] == properties['prop_blank']
+
+            cached_info = ServiceInfo(subtype, registration_name)
+            cached_info.load_from_cache(zeroconf_browser)
+            assert cached_info.properties is not None
+            assert cached_info.properties[b'prop_blank'] == properties['prop_blank']
+
+            zeroconf_registrar.unregister_service(info_service)
+            service_removed.wait(1)
+            assert service_removed.is_set()
+
+        finally:
+            zeroconf_registrar.close()
+            zeroconf_browser.remove_service_listener(listener)
+            zeroconf_browser.close()
 
 
 def test_servicelisteners_raise_not_implemented():
     """Verify service listeners raise when one of the methods is not implemented."""
 
     class MyPartialListener(r.ServiceListener):
         """A listener that does not implement anything."""
```

### Comparing `zeroconf-0.63.0/tests/test_updates.py` & `zeroconf-0.64.0/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/utils/__init__.py` & `zeroconf-0.64.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/utils/test_asyncio.py` & `zeroconf-0.64.0/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/utils/test_name.py` & `zeroconf-0.64.0/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/tests/utils/test_net.py` & `zeroconf-0.64.0/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.63.0/setup.py` & `zeroconf-0.64.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.63.0',
+    'version': '0.64.0',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.63.0/PKG-INFO` & `zeroconf-0.64.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.63.0
+Version: 0.64.0
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

