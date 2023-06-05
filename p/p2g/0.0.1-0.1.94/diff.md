# Comparing `tmp/p2g-0.0.1.tar.gz` & `tmp/p2g-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "p2g-0.1.94.tar", max compression
```

## Comparing `p2g-0.0.1.tar` & `p2g-0.1.94.tar`

### file list

```diff
@@ -1,102 +1,80 @@
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 p2g-0.0.1/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0   193645 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57265 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19738 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    22333 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66350 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1141182 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134186 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113644 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    63224 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0    66813 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    24373 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93232 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    31479 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    96547 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48513 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82081 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   182894 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30230 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53680 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   173146 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152123 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0   248480 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444925 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73928 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    96948 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446239 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140912 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13251 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7873 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26964 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86467 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33550 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75504 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69905 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97871 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12909 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   382562 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/p2g_sacsac/__init__.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/p2g_sacsac/__init__.meta.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/p2g_sacsac/example.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 p2g-0.0.1/src/.mypy_cache/3.10/p2g_sacsac/example.meta.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 p2g-0.0.1/src/p2g_sacsac/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 p2g-0.0.1/src/p2g_sacsac/example.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 p2g-0.0.1/LICENSE
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 p2g-0.0.1/README.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 p2g-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 p2g-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0    36156 2023-06-05 00:17:14.589302 p2g-0.1.94/README.rst
+-rwxr-xr-x   0        0        0     1132 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/__init__.py
+-rwxr-xr-x   0        0        0       24 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/__main__.py
+-rwxr-xr-x   0        0        0      688 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/axis.py
+-rwxr-xr-x   0        0        0     1051 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/builtin.py
+-rwxr-xr-x   0        0        0     3308 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/coords.py
+-rwxr-xr-x   0        0        0     3501 2023-06-05 00:11:42.034391 p2g-0.1.94/p2g/debug.py
+-rwxr-xr-x   0        0        0       16 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/doc/authors.org
+-rwxr-xr-x   0        0        0       47 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/doc/authors.rst
+-rwxr-xr-x   0        0        0     6302 2023-06-05 00:11:52.726613 p2g-0.1.94/p2g/doc/haas.org
+-rwxr-xr-x   0        0        0    16060 2023-06-05 00:11:53.614632 p2g-0.1.94/p2g/doc/haas.txt
+-rwxr-xr-x   0        0        0    22547 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/doc/readme.md
+-rwxr-xr-x   0        0        0    24083 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/doc/readme.org
+-rwxr-xr-x   0        0        0    36156 2023-06-05 00:11:53.150622 p2g-0.1.94/p2g/doc/readme.rst
+-rwxr-xr-x   0        0        0     2441 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/err.py
+-rwxr-xr-x   0        0        0     2732 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/examples/csearch.py
+-rwxr-xr-x   0        0        0     2645 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/examples/defs.py
+-rwxr-xr-x   0        0        0     1853 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/examples/probecalibrate.nc
+-rwxr-xr-x   0        0        0     1056 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/examples/probecalibrate.py
+-rwxr-xr-x   0        0        0     9503 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/examples/vicecenter.nc
+-rwxr-xr-x   0        0        0     3928 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/examples/vicecenter.py
+-rwxr-xr-x   0        0        0     1331 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/gbl.py
+-rwxr-xr-x   0        0        0     3537 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/goto.py
+-rw-r--r--   0        0        0     6899 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/haas.py
+-rwxr-xr-x   0        0        0     3342 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/lib.py
+-rwxr-xr-x   0        0        0     4589 2023-06-05 00:15:44.335426 p2g-0.1.94/p2g/main.py
+-rwxr-xr-x   0        0        0    15709 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/makestdvars.py
+-rwxr-xr-x   0        0        0    21488 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/mvarsorig
+-rwxr-xr-x   0        0        0      655 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/nd.py
+-rwxr-xr-x   0        0        0    13271 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/op.py
+-rwxr-xr-x   0        0        0      593 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/opinfo.py
+-rwxr-xr-x   0        0        0     6680 2023-06-04 23:59:54.703683 p2g-0.1.94/p2g/ptest.py
+-rwxr-xr-x   0        0        0     3120 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/scalar.py
+-rwxr-xr-x   0        0        0     6786 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/stat.py
+-rwxr-xr-x   0        0        0     1797 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/symbol.py
+-rwxr-xr-x   0        0        0      211 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/conftest.py
+-rwxr-xr-x   0        0        0       22 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/dummy.py
+-rw-r--r--   0        0        0       45 2023-06-04 22:00:20.282440 p2g-0.1.94/p2g/tests/golden/error_forcefail1.nc
+-rw-r--r--   0        0        0        5 2023-06-05 00:12:49.835800 p2g-0.1.94/p2g/tests/golden/error_xfail_force_fail.nc
+-rwxr-xr-x   0        0        0        3 2023-06-05 00:12:52.067846 p2g-0.1.94/p2g/tests/golden/meta_simple_xfail1.nc
+-rw-r--r--   0        0        0       44 2023-06-05 00:16:03.543825 p2g-0.1.94/p2g/tests/golden/meta_transitory_golden.nc
+-rwxr-xr-x   0        0        0     1538 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/tests/golden/probecalibrate.nc
+-rwxr-xr-x   0        0        0     8152 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/tests/golden/vicecenter.nc
+-rwxr-xr-x   0        0        0      160 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/not_pytest.py
+-rwxr-xr-x   0        0        0     2456 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_axes.py
+-rwxr-xr-x   0        0        0      515 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_basic.py
+-rwxr-xr-x   0        0        0     6023 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_builtins.py
+-rwxr-xr-x   0        0        0      194 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_comment.py
+-rwxr-xr-x   0        0        0     5133 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_coords.py
+-rwxr-xr-x   0        0        0      450 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_edge.py
+-rwxr-xr-x   0        0        0     3131 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_error.py
+-rwxr-xr-x   0        0        0      550 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/tests/test_example.py
+-rwxr-xr-x   0        0        0      728 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_expr.py
+-rwxr-xr-x   0        0        0     1738 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/tests/test_for.py
+-rwxr-xr-x   0        0        0     4751 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/tests/test_func.py
+-rwxr-xr-x   0        0        0     1632 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/tests/test_goto.py
+-rwxr-xr-x   0        0        0       46 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_gvar.py
+-rwxr-xr-x   0        0        0     6920 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/tests/test_interp.py
+-rwxr-xr-x   0        0        0      520 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_linenos.py
+-rwxr-xr-x   0        0        0     3480 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_main.py
+-rwxr-xr-x   0        0        0      493 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/tests/test_makestdvars.py
+-rwxr-xr-x   0        0        0     1850 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_meta.py
+-rwxr-xr-x   0        0        0     1569 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_nt1.py
+-rwxr-xr-x   0        0        0     6314 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_op.py
+-rwxr-xr-x   0        0        0     8637 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/tests/test_smoke.py
+-rwxr-xr-x   0        0        0     1014 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_str.py
+-rwxr-xr-x   0        0        0     1214 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_tuple.py
+-rwxr-xr-x   0        0        0     4162 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/tests/test_vars.py
+-rwxr-xr-x   0        0        0     9126 2023-06-04 23:59:54.699683 p2g-0.1.94/p2g/tests/test_vector.py
+-rwxr-xr-x   0        0        0     1281 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/thanksto
+-rwxr-xr-x   0        0        0     5898 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/vector.py
+-rwxr-xr-x   0        0        0       23 2023-06-05 00:16:24.200254 p2g-0.1.94/p2g/version.py
+-rwxr-xr-x   0        0        0      817 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/visible.py
+-rwxr-xr-x   0        0        0    11396 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/walk.py
+-rwxr-xr-x   0        0        0     3055 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/walkbase.py
+-rwxr-xr-x   0        0        0     4579 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/walkexpr.py
+-rwxr-xr-x   0        0        0     6344 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/walkfunc.py
+-rwxr-xr-x   0        0        0     3426 2023-06-04 23:59:54.707683 p2g-0.1.94/p2g/walkns.py
+-rwxr-xr-x   0        0        0     3895 2023-06-05 00:16:23.940249 p2g-0.1.94/pyproject.toml
+-rw-r--r--   0        0        0    37127 1970-01-01 00:00:00.000000 p2g-0.1.94/PKG-INFO
```

### Comparing `p2g-0.0.1/LICENSE` & `p2g-0.1.94/p2g/thanksto`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,29 @@
-Copyright (c) 2018 The Python Packaging Authority
+The good parts of walk*.py are from:
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
 
+# Python AST interpreter written in Python
+#
+# This module is part of the Pycopy https://github.com/pfalcon/pycopy
+# project.
+#
+# Copyright (c) 2019 Paul Sokolovsky
+#
+# The MIT License
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+# THE SOFTWARE.
```

