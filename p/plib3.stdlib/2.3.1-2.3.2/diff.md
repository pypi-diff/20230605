# Comparing `tmp/plib3.stdlib-2.3.1.tar.gz` & `tmp/plib3.stdlib-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pdonis/git/plib3-stdlib/dist/tmpciqxsh4d/plib3.stdlib-2.3.1.tar", last modified: Sat May 13 03:53:01 2023, max compression
+gzip compressed data, was "/home/pdonis/git/plib3-stdlib/dist/tmpib3gy09j/plib3.stdlib-2.3.2.tar", last modified: Mon Jun  5 02:05:17 2023, max compression
```

## Comparing `plib3.stdlib-2.3.1.tar` & `plib3.stdlib-2.3.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/stdlib/
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1471 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/systools.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1782 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/timer.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     5799 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/plib/stdlib/classtools.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     5303 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/localize.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      472 2023-05-13 03:47:26.000000 plib3.stdlib-2.3.1/plib/stdlib/__init__.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/stdlib/util/
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      369 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/util/__init__.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     7156 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/util/ModuleProxy.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3143 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/strings.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      592 2022-01-20 06:02:56.000000 plib3.stdlib-2.3.1/plib/stdlib/examples.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1250 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/imp.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1317 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/jsontools.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)    28538 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/iters.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     7720 2023-05-13 03:48:48.000000 plib3.stdlib-2.3.1/plib/stdlib/postinstall.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     6036 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/ostools.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1731 2022-07-29 23:10:48.000000 plib3.stdlib-2.3.1/plib/stdlib/builtins.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3877 2022-07-29 23:10:48.000000 plib3.stdlib-2.3.1/plib/stdlib/_extras.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     4341 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/mail.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1475 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/copytools.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/stdlib/ini/
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2464 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/plib/stdlib/ini/__init__.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3470 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/plib/stdlib/ini/PIniFile.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1714 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/ini/PIniFileSection.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     5544 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/plib/stdlib/ini/PIniInterface.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1210 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/ini/PIniFileOption.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2413 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/ini/PIniFileBase.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2695 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/cmdline.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2069 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.1/plib/stdlib/csvtools.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     8247 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/options.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1956 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/proc.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/stdlib/coll/
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     8392 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/plib/stdlib/coll/__init__.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3534 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/coll/_names.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2957 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/plib/stdlib/coll/_tests.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)    12098 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/coll/_abc.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5617 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/coll/_utils.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3062 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/coll/_seq.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     8582 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/coll/_tuples.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)    19554 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/coll/_mixins.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     8327 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/coll/_bases.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      772 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/mathlib.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/stdlib/decotools/
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5064 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/decotools/IndexedGenerator.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)    42806 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/decotools/__init__.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     6174 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/decotools/MemoizedGenerator.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     6052 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/decotools/DelayedDecorator.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/stdlib/net/
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     3509 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/plib/stdlib/net/__init__.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     6690 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/plib/stdlib/net/client.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     2361 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/plib/stdlib/net/transport.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      537 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/sigs.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5882 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/tztools.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      604 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/stdlib/fdtools.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/test/
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/test/stdlib/
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/test/stdlib/doctests/
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1079 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_Singleton.txt
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3583 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_newlines.txt
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2474 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_builtins.txt
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1984 2022-07-29 23:10:48.000000 plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_abc.txt
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      790 2019-09-24 03:38:20.000000 plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_coll.txt
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     7596 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_normalize_slice.txt
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     4290 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_SortMixin.txt
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1313 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_cached_property.txt
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     4293 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib.txt
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1302 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_sigs.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1392 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractlist.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      282 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/__init__.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      938 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractcontainer.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      721 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/ModuleProxy_testmod.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      852 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_basekeyed.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      870 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractkeyed.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      961 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractmapping.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)    41450 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/abstract_testlib.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1060 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_basedict.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1052 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_baselist.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2121 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_stdlib.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     4228 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_ModuleProxy.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1010 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractdict.py
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      729 2022-07-29 23:10:48.000000 plib3.stdlib-2.3.1/plib/test/stdlib/__main__.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5612 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_ostools.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      946 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_basemapping.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      871 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_basecontainer.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1859 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractsequence.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)    22729 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/mapping_testlib.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      946 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.1/plib/test/stdlib/test_basesequence.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1046 2022-01-05 02:22:10.000000 plib3.stdlib-2.3.1/plib/test/__main__.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/plib/test/support/
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3760 2022-01-04 20:34:28.000000 plib3.stdlib-2.3.1/plib/test/support/__init__.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/examples/
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/examples/pyidserver/
--rwxrwx---   0 pdonis    (1002) pdonis    (1002)     9934 2022-01-09 05:08:44.000000 plib3.stdlib-2.3.1/examples/pyidserver/pyidserver3.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/examples/pyget/
--rwxrwx---   0 pdonis    (1002) pdonis    (1002)     3511 2022-01-03 06:25:27.000000 plib3.stdlib-2.3.1/examples/pyget/pyget3.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/examples/scrips/
--rwxrwx---   0 pdonis    (1002) pdonis    (1002)     6239 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/examples/scrips/scrips3.py
-drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/examples/tzname/
--rwxrwx---   0 pdonis    (1002) pdonis    (1002)     3268 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.1/examples/tzname/tzname3.py
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)    18010 2019-09-20 02:24:51.000000 plib3.stdlib-2.3.1/LICENSE.txt
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     6862 2022-01-22 04:03:34.000000 plib3.stdlib-2.3.1/README.rst
--rw-rw----   0 pdonis    (1002) pdonis    (1002)       38 2022-01-03 05:57:16.000000 plib3.stdlib-2.3.1/MANIFEST.in
--rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      131 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.1/TODO.rst
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     7805 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/PKG-INFO
--rw-rw----   0 pdonis    (1002) pdonis    (1002)      117 2022-01-22 04:03:34.000000 plib3.stdlib-2.3.1/pyproject.toml
--rw-rw----   0 pdonis    (1002) pdonis    (1002)     1639 2023-05-13 03:53:01.000000 plib3.stdlib-2.3.1/setup.cfg
--rw-rw----   0 pdonis    (1002) pdonis    (1002)    90727 2023-05-13 03:52:34.000000 plib3.stdlib-2.3.1/CHANGES.rst
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/stdlib/
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1471 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/systools.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1782 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/timer.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     5799 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/plib/stdlib/classtools.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     5303 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/localize.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      472 2023-06-05 01:47:36.000000 plib3.stdlib-2.3.2/plib/stdlib/__init__.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/stdlib/util/
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      369 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/util/__init__.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     7156 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/util/ModuleProxy.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3143 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/strings.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      592 2022-01-20 06:02:56.000000 plib3.stdlib-2.3.2/plib/stdlib/examples.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1250 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/imp.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1317 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/jsontools.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)    28538 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/iters.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     7720 2023-05-13 21:55:55.000000 plib3.stdlib-2.3.2/plib/stdlib/postinstall.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     6036 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/ostools.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1785 2023-06-05 01:53:21.000000 plib3.stdlib-2.3.2/plib/stdlib/builtins.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3950 2023-06-05 01:51:05.000000 plib3.stdlib-2.3.2/plib/stdlib/_extras.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     4341 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/mail.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1475 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/copytools.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/stdlib/ini/
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2464 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/plib/stdlib/ini/__init__.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3470 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/plib/stdlib/ini/PIniFile.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1714 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/ini/PIniFileSection.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     5544 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/plib/stdlib/ini/PIniInterface.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1210 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/ini/PIniFileOption.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2413 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/ini/PIniFileBase.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2695 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/cmdline.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2069 2022-01-03 06:29:22.000000 plib3.stdlib-2.3.2/plib/stdlib/csvtools.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     8247 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/options.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1956 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/proc.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/stdlib/coll/
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     8392 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/plib/stdlib/coll/__init__.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3534 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/coll/_names.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2957 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/plib/stdlib/coll/_tests.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)    12098 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/coll/_abc.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5617 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/coll/_utils.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3062 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/coll/_seq.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     8582 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/coll/_tuples.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)    19554 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/coll/_mixins.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     8327 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/coll/_bases.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      772 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/mathlib.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/stdlib/decotools/
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5064 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/decotools/IndexedGenerator.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)    42806 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/decotools/__init__.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     6174 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/decotools/MemoizedGenerator.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     6052 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/decotools/DelayedDecorator.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/stdlib/net/
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     3509 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/plib/stdlib/net/__init__.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     6690 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/plib/stdlib/net/client.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     2361 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/plib/stdlib/net/transport.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      537 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/sigs.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5882 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/tztools.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      604 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/stdlib/fdtools.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/test/
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/test/stdlib/
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/test/stdlib/doctests/
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1079 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_Singleton.txt
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3583 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_newlines.txt
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2474 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_builtins.txt
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1984 2022-07-29 23:10:48.000000 plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_abc.txt
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      790 2019-09-24 03:38:20.000000 plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_coll.txt
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     7596 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_normalize_slice.txt
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     4290 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_SortMixin.txt
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1313 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_cached_property.txt
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     4293 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib.txt
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1302 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_sigs.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1392 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractlist.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      282 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/__init__.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      938 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractcontainer.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      721 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/ModuleProxy_testmod.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      852 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_basekeyed.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      870 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractkeyed.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      961 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractmapping.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)    41450 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/abstract_testlib.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1060 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_basedict.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1052 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_baselist.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     2121 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_stdlib.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     4228 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_ModuleProxy.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1010 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractdict.py
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      729 2023-05-13 21:56:17.000000 plib3.stdlib-2.3.2/plib/test/stdlib/__main__.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     5612 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_ostools.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      946 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_basemapping.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      871 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_basecontainer.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1859 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractsequence.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)    22729 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/mapping_testlib.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      946 2022-01-03 06:29:23.000000 plib3.stdlib-2.3.2/plib/test/stdlib/test_basesequence.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     1046 2022-01-05 02:22:10.000000 plib3.stdlib-2.3.2/plib/test/__main__.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/plib/test/support/
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)     3760 2022-01-04 20:34:28.000000 plib3.stdlib-2.3.2/plib/test/support/__init__.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/examples/
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/examples/pyidserver/
+-rwxrwx---   0 pdonis    (1002) pdonis    (1002)     9934 2022-01-09 05:08:44.000000 plib3.stdlib-2.3.2/examples/pyidserver/pyidserver3.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/examples/pyget/
+-rwxrwx---   0 pdonis    (1002) pdonis    (1002)     3511 2022-01-03 06:25:27.000000 plib3.stdlib-2.3.2/examples/pyget/pyget3.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/examples/scrips/
+-rwxrwx---   0 pdonis    (1002) pdonis    (1002)     6239 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/examples/scrips/scrips3.py
+drwxrwx---   0 pdonis    (1002) pdonis    (1002)        0 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/examples/tzname/
+-rwxrwx---   0 pdonis    (1002) pdonis    (1002)     3268 2022-01-03 06:29:49.000000 plib3.stdlib-2.3.2/examples/tzname/tzname3.py
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)    18010 2019-09-20 02:24:51.000000 plib3.stdlib-2.3.2/LICENSE.txt
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     6862 2022-01-22 04:03:34.000000 plib3.stdlib-2.3.2/README.rst
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)       38 2022-01-03 05:57:16.000000 plib3.stdlib-2.3.2/MANIFEST.in
+-rw-rw-r--   0 pdonis    (1002) pdonis    (1002)      131 2018-10-23 04:11:37.000000 plib3.stdlib-2.3.2/TODO.rst
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     7805 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/PKG-INFO
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)      117 2022-01-22 04:03:34.000000 plib3.stdlib-2.3.2/pyproject.toml
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)     1639 2023-06-05 02:05:17.000000 plib3.stdlib-2.3.2/setup.cfg
+-rw-rw----   0 pdonis    (1002) pdonis    (1002)    90957 2023-06-05 01:54:56.000000 plib3.stdlib-2.3.2/CHANGES.rst
```

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/systools.py` & `plib3.stdlib-2.3.2/plib/stdlib/systools.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/timer.py` & `plib3.stdlib-2.3.2/plib/stdlib/timer.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/classtools.py` & `plib3.stdlib-2.3.2/plib/stdlib/classtools.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/localize.py` & `plib3.stdlib-2.3.2/plib/stdlib/localize.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/util/ModuleProxy.py` & `plib3.stdlib-2.3.2/plib/stdlib/util/ModuleProxy.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/strings.py` & `plib3.stdlib-2.3.2/plib/stdlib/strings.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/examples.py` & `plib3.stdlib-2.3.2/plib/stdlib/examples.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/imp.py` & `plib3.stdlib-2.3.2/plib/stdlib/imp.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/jsontools.py` & `plib3.stdlib-2.3.2/plib/stdlib/jsontools.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/iters.py` & `plib3.stdlib-2.3.2/plib/stdlib/iters.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/postinstall.py` & `plib3.stdlib-2.3.2/plib/stdlib/postinstall.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/ostools.py` & `plib3.stdlib-2.3.2/plib/stdlib/ostools.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/builtins.py` & `plib3.stdlib-2.3.2/plib/stdlib/builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     """
     
     global _upgraded
     if not _upgraded:
         import builtins
         from plib.stdlib import _extras
         for extra_name in EXTRA_NAMES:
-            setattr(builtins, extra_name, getattr(_extras, extra_name))
+            if not hasattr(builtins, extra_name):
+                setattr(builtins, extra_name, getattr(_extras, extra_name))
         _upgraded = True
         return "Upgraded built-ins installed!"
     return "Upgrade already performed, nothing to do."
 
 
 upgrade_builtins()
```

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/_extras.py` & `plib3.stdlib-2.3.2/plib/stdlib/_extras.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,18 +118,23 @@
 def last(iterable, default=None, deque=_deque):
     """Return last item in iterable, or default if empty.
     """
     q = deque(iterable, maxlen=1)  # consumes iterable at C speed
     return q[0] if q else default
 
 
-def prod(iterable, mul=_mul):
-    """Return the product of all items in iterable.
-    """
-    return reduce(mul, iterable, 1)
+try:
+    from math import prod
+
+except ImportError:
+    
+    def prod(iterable, mul=_mul):
+        """Return the product of all items in iterable.
+        """
+        return reduce(mul, iterable, 1)
 
 
 def type_from_name(name):
     """Return type object corresponding to ``name``.
     
     Currently searches only the built-in types. No checking is done to
     make sure the returned object is actually a type.
```

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/mail.py` & `plib3.stdlib-2.3.2/plib/stdlib/mail.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/copytools.py` & `plib3.stdlib-2.3.2/plib/stdlib/copytools.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/ini/__init__.py` & `plib3.stdlib-2.3.2/plib/stdlib/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/ini/PIniFile.py` & `plib3.stdlib-2.3.2/plib/stdlib/ini/PIniFile.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/ini/PIniFileSection.py` & `plib3.stdlib-2.3.2/plib/stdlib/ini/PIniFileSection.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/ini/PIniInterface.py` & `plib3.stdlib-2.3.2/plib/stdlib/ini/PIniInterface.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/ini/PIniFileOption.py` & `plib3.stdlib-2.3.2/plib/stdlib/ini/PIniFileOption.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/ini/PIniFileBase.py` & `plib3.stdlib-2.3.2/plib/stdlib/ini/PIniFileBase.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/cmdline.py` & `plib3.stdlib-2.3.2/plib/stdlib/cmdline.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/csvtools.py` & `plib3.stdlib-2.3.2/plib/stdlib/csvtools.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/options.py` & `plib3.stdlib-2.3.2/plib/stdlib/options.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/proc.py` & `plib3.stdlib-2.3.2/plib/stdlib/proc.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/coll/__init__.py` & `plib3.stdlib-2.3.2/plib/stdlib/coll/__init__.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/coll/_names.py` & `plib3.stdlib-2.3.2/plib/stdlib/coll/_names.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/coll/_tests.py` & `plib3.stdlib-2.3.2/plib/stdlib/coll/_tests.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/coll/_abc.py` & `plib3.stdlib-2.3.2/plib/stdlib/coll/_abc.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/coll/_utils.py` & `plib3.stdlib-2.3.2/plib/stdlib/coll/_utils.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/coll/_seq.py` & `plib3.stdlib-2.3.2/plib/stdlib/coll/_seq.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/coll/_tuples.py` & `plib3.stdlib-2.3.2/plib/stdlib/coll/_tuples.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/coll/_mixins.py` & `plib3.stdlib-2.3.2/plib/stdlib/coll/_mixins.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/coll/_bases.py` & `plib3.stdlib-2.3.2/plib/stdlib/coll/_bases.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/mathlib.py` & `plib3.stdlib-2.3.2/plib/stdlib/mathlib.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/decotools/IndexedGenerator.py` & `plib3.stdlib-2.3.2/plib/stdlib/decotools/IndexedGenerator.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/decotools/__init__.py` & `plib3.stdlib-2.3.2/plib/stdlib/decotools/__init__.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/decotools/MemoizedGenerator.py` & `plib3.stdlib-2.3.2/plib/stdlib/decotools/MemoizedGenerator.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/decotools/DelayedDecorator.py` & `plib3.stdlib-2.3.2/plib/stdlib/decotools/DelayedDecorator.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/net/__init__.py` & `plib3.stdlib-2.3.2/plib/stdlib/net/__init__.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/net/client.py` & `plib3.stdlib-2.3.2/plib/stdlib/net/client.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/net/transport.py` & `plib3.stdlib-2.3.2/plib/stdlib/net/transport.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/sigs.py` & `plib3.stdlib-2.3.2/plib/stdlib/sigs.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/tztools.py` & `plib3.stdlib-2.3.2/plib/stdlib/tztools.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/stdlib/fdtools.py` & `plib3.stdlib-2.3.2/plib/stdlib/fdtools.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_Singleton.txt` & `plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_Singleton.txt`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_newlines.txt` & `plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_newlines.txt`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_builtins.txt` & `plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_builtins.txt`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_abc.txt` & `plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_abc.txt`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_coll.txt` & `plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_coll.txt`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_normalize_slice.txt` & `plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_normalize_slice.txt`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_SortMixin.txt` & `plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_SortMixin.txt`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib_cached_property.txt` & `plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib_cached_property.txt`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/doctests/test_stdlib.txt` & `plib3.stdlib-2.3.2/plib/test/stdlib/doctests/test_stdlib.txt`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_sigs.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_sigs.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractlist.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractlist.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractcontainer.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractcontainer.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/ModuleProxy_testmod.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/ModuleProxy_testmod.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_basekeyed.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_basekeyed.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractkeyed.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractkeyed.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractmapping.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractmapping.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/abstract_testlib.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/abstract_testlib.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_basedict.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_basedict.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_baselist.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_baselist.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_stdlib.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_ModuleProxy.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_ModuleProxy.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractdict.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractdict.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/__main__.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_ostools.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_ostools.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_basemapping.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_basemapping.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_basecontainer.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_basecontainer.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_abstractsequence.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_abstractsequence.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/mapping_testlib.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/mapping_testlib.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/stdlib/test_basesequence.py` & `plib3.stdlib-2.3.2/plib/test/stdlib/test_basesequence.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/__main__.py` & `plib3.stdlib-2.3.2/plib/test/__main__.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/plib/test/support/__init__.py` & `plib3.stdlib-2.3.2/plib/test/support/__init__.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/examples/pyidserver/pyidserver3.py` & `plib3.stdlib-2.3.2/examples/pyidserver/pyidserver3.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/examples/pyget/pyget3.py` & `plib3.stdlib-2.3.2/examples/pyget/pyget3.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/examples/scrips/scrips3.py` & `plib3.stdlib-2.3.2/examples/scrips/scrips3.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/examples/tzname/tzname3.py` & `plib3.stdlib-2.3.2/examples/tzname/tzname3.py`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/LICENSE.txt` & `plib3.stdlib-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/README.rst` & `plib3.stdlib-2.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/PKG-INFO` & `plib3.stdlib-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plib3.stdlib
-Version: 2.3.1
+Version: 2.3.2
 Summary: Useful packages and modules to extend the Python 3 standard library.
 Home-page: http://pypi.org/project/plib3.stdlib
 Author: Peter A. Donis
 Author-email: peterdonis@alum.mit.edu
 License: GPLv2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plib3.stdlib-2.3.1/setup.cfg` & `plib3.stdlib-2.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `plib3.stdlib-2.3.1/CHANGES.rst` & `plib3.stdlib-2.3.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 plib3.stdlib Change Log
 =======================
 
+Version 2.3.2
+-------------
+
+- Use built-in ``prod`` function if available (in versions 3.8
+  and above) instead of adding the implementation from the
+  ``_extras`` module to builtins when ``plib.stdlib.builtins``
+  is imported.
+
 Version 2.3.1
 -------------
 
 - Speed up entry points generated by the ``make_entry_points``
   function in the ``postinstall`` module by pre-computing the
   script path.
```

