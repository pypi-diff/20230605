# Comparing `tmp/TypeDal-0.6.2.tar.gz` & `tmp/typedal-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TypeDal-0.6.2.tar", last modified: Thu Feb  2 12:08:43 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `TypeDal-0.6.2.tar` & `typedal-1.0.0b1.tar`

### file list

```diff
@@ -1,15 +1,340 @@
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-02-02 12:08:43.111335 TypeDal-0.6.2/
--rw-rw-r--   0 robin     (1000) robin     (1000)     8799 2023-02-02 12:08:43.111335 TypeDal-0.6.2/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)     8524 2022-12-12 19:32:56.000000 TypeDal-0.6.2/README.md
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-02-02 12:08:43.111335 TypeDal-0.6.2/TypeDal.egg-info/
--rw-rw-r--   0 robin     (1000) robin     (1000)     8799 2023-02-02 12:08:43.000000 TypeDal-0.6.2/TypeDal.egg-info/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)      226 2023-02-02 12:08:43.000000 TypeDal-0.6.2/TypeDal.egg-info/SOURCES.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-02-02 12:08:43.000000 TypeDal-0.6.2/TypeDal.egg-info/dependency_links.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        6 2023-02-02 12:08:43.000000 TypeDal-0.6.2/TypeDal.egg-info/requires.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        8 2023-02-02 12:08:43.000000 TypeDal-0.6.2/TypeDal.egg-info/top_level.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-02-02 12:08:43.111335 TypeDal-0.6.2/setup.cfg
--rw-rw-r--   0 robin     (1000) robin     (1000)      490 2023-02-02 12:08:13.000000 TypeDal-0.6.2/setup.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-02-02 12:08:43.111335 TypeDal-0.6.2/typedal/
--rw-rw-r--   0 robin     (1000) robin     (1000)      165 2022-12-12 19:03:34.000000 TypeDal-0.6.2/typedal/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     7934 2023-01-05 20:56:10.000000 TypeDal-0.6.2/typedal/core.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3422 2023-02-02 12:06:27.000000 TypeDal-0.6.2/typedal/fields.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 typedal-1.0.0b1/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 typedal-1.0.0b1/coverage.svg
+-rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 typedal-1.0.0b1/example_new.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 typedal-1.0.0b1/example_old.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0   177667 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0   170960 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_decimal.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_decimal.meta.json
+-rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0  1054992 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   123328 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   104160 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    57612 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   142044 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/decimal.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/decimal.meta.json
+-rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    85348 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/numbers.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/numbers.meta.json
+-rw-r--r--   0        0        0    88278 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    75208 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   167175 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    49442 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   168498 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   146267 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   228230 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   416965 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407999 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   128994 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    79298 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70175 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    90277 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350178 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/__init__.data.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/__init__.meta.json
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    33347 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/core.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/core.meta.json
+-rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/fields.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/fields.meta.json
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/pydal_objects.data.json
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180368 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171931 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0    23336 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60676 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1130454 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123317 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109204 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57745 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142208 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    90123 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    85337 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    28767 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0    87488 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75197 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167545 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28480 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49741 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   172768 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   239632 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432234 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57845 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89054 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407988 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128983 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79287 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70579 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91119 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350743 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/__init__.data.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/__init__.meta.json
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    33350 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/core.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/core.meta.json
+-rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/fields.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/fields.meta.json
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    33137 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/core.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/core.meta.json
+-rw-r--r--   0        0        0    30390 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/fields.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/fields.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/121ed75fe9fe5f8e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/19309938546e93ab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/197f3188bc94f91f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1aa1390b5bde1004
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1b34455c399f0006
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1bd1a229a4f4ee7f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1c46d1f378d28fbb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1ca71ee291d82018
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1d6bb777df44b8ec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1dc8423cfb79eaa4
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/20585cf790eae81e
+-rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/221af82ae72a7f27
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/2282e801459c52a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/248c4e1a32c704cb
+-rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/24e1b4aab386ebc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/28b1d8ac7e2aab6b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/2b7f7d266c8efaad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/2dac345be8527adf
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/2f3396c610fd7095
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/31731f8e74291475
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/3826106cf4494de8
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/38d5fd55b14a9d6c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/3afc55a04b8f8bb2
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/4022ee8774ccd98a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/42f9a2406e74c24f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/4696b157ff786f22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/46a88ce266f1ad94
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/4a6edd5010cb9700
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/4d0230e9a81a468
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/52018ba3989fcaf7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/54e6ba8c25a22ffc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/566d94db91d23339
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/5b076d769fa5cacd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/5ceb1580c62ee794
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/6bc90dbb56504f96
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/6f0c8f98e4da1d48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/74e52af774eebdbd
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/75bd1769f6e29ed7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/815ba2cfea236769
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/876d9a8d302e1c46
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/88e2927df9448936
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/8c4d3f5ef14b0167
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/8f8ec552e76f3eab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/95c82d8566c6704c
+-rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/a0739889bf9412e8
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/a225e4df39be9b29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/a2340fd4c9aa1141
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/a513d558646cd439
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/b121e2b70fd66eb8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/b218ff88bc22b626
+-rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/b419496fa9e72887
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/b886c97e4d4117f0
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/bdcdf5c7bbc1d738
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/c06de16f3c7a64cc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/c635f255374598c5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/c671ae94ff3d3e2e
+-rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/cdfecbca581311ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/ce44121ca4091b64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/ced49ec87d10bcb0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/cfc06a1f13c8ab47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/d16c5d29763a704e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/d225ad4c14b8ca60
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/d3a95555c0919160
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/d655bee8ff0a59f2
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/da4811a7730a562a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/dca573767bc8be7e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/e3e29f9eacb7027f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/e46ab4b61bb5d446
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/e5e0cc178d5c9df5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/eb564f7989641958
+-rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/eee2f3c667de6c7a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/f04d0d78a00adfd6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/f2ddc22a4b221f54
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/f879e8c947a6b7a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/faa51a5044a3c279
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c___about___py.html
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c___init___py.html
+-rw-r--r--   0        0        0    96583 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c_core_py.html
+-rw-r--r--   0        0        0    63148 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c_fields_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/style.css
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 typedal-1.0.0b1/src/typedal/__about__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 typedal-1.0.0b1/src/typedal/__init__.py
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 typedal-1.0.0b1/src/typedal/core.py
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 typedal-1.0.0b1/src/typedal/fields.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 typedal-1.0.0b1/tests/__init__.py
+-rw-r--r--   0        0        0     7847 2020-02-02 00:00:00.000000 typedal-1.0.0b1/tests/test_main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.gitignore
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 typedal-1.0.0b1/README.md
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 typedal-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 typedal-1.0.0b1/PKG-INFO
```

### Comparing `TypeDal-0.6.2/PKG-INFO` & `typedal-1.0.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-Metadata-Version: 2.1
-Name: TypeDal
-Version: 0.6.2
-Summary: Typing support for PyDAL
-Home-page: https://github.com/trialandsuccess/TypeDAL
-Author: Robin van der Noord
-Author-email: contact@trialandsuccess.nl
-Requires-Python: >3.10.0
-Description-Content-Type: text/markdown
-
 # TypeDAL
 
+[![PyPI - Version](https://img.shields.io/pypi/v/TypeDal.svg)](https://pypi.org/project/typedal)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/TypeDal.svg)](https://pypi.org/project/typedal)  
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
+[![su6 checks](https://github.com/trialandsuccess/typedal/actions/workflows/su6.yml/badge.svg)](https://github.com/trialandsuccess/typedal/actions)
+![coverage.svg](coverage.svg)
+
 Typing support for [PyDAL](http://web2py.com/books/default/chapter/29/6).
 This package aims to improve the typing support for PyDAL. By using classes instead of the define_table method,
 type hinting the result of queries can improve the experience while developing. In the background, the queries are still
 generated and executed by pydal itself, this package only proves some logic to properly pass calls from class methods to
 the underlying `db.define_table` pydal Tables.
 
 - `TypeDAL` is the replacement class for DAL that manages the code on top of DAL.
@@ -44,16 +41,16 @@
 
 </td>
 
 <td></td>
 <td>
 
 ```python
-from typedal import TypeDAL, TypedTable, TypedField, TypedRows
-from typedal.fields import TextField
+from src.typedal import TypeDAL, TypedTable, TypedField, TypedRows
+from src.typedal.fields import TextField
 from typing import Optional
 
 db = TypeDAL(...)
 ```
 
 </td>
 
@@ -231,8 +228,8 @@
   and `from __future__ import annotations` already does) in a way that this module currently can not handle: all
   annotations are converted to string representations. This makes it very hard to re-evaluate the annotation into the
   original type, since the variable scope is lost (and thus references to variables or other classes are ambiguous or
   simply impossible to find).
 - `TypedField` limitations; Since pydal implements some magic methods to perform queries, some features of typing will
   not work on a typed field: `typing.Optional` or a union (`Field() | None`) will result in errors. The only way to make
   a typedfield optional right now, would be to set `required=False` as an argument yourself. This is also a reason
-  why `typing.get_type_hints` is not a solution for the first caveat.
+  why `typing.get_type_hints` is not a solution for the first caveat.
```

### Comparing `TypeDal-0.6.2/typedal/core.py` & `typedal-1.0.0b1/.ruff_cache/content/a0739889bf9412e8`

 * *Files 5% similar despite different names*

```diff
@@ -1,496 +1,522 @@
-00000000: 696d 706f 7274 2070 7964 616c 0a66 726f  import pydal.fro
-00000010: 6d20 7079 6461 6c2e 6f62 6a65 6374 7320  m pydal.objects 
-00000020: 696d 706f 7274 2052 6f77 2c20 526f 7773  import Row, Rows
-00000030: 2c20 4669 656c 642c 2054 6162 6c65 2020  , Field, Table  
-00000040: 2320 2a3f 0a69 6d70 6f72 7420 7479 7069  # *?.import typi
-00000050: 6e67 0a69 6d70 6f72 7420 7479 7065 730a  ng.import types.
-00000060: 696d 706f 7274 2064 6174 6574 696d 6520  import datetime 
-00000070: 6173 2064 740a 6672 6f6d 2064 6563 696d  as dt.from decim
-00000080: 616c 2069 6d70 6f72 7420 4465 6369 6d61  al import Decima
-00000090: 6c0a 0a42 4153 4943 5f4d 4150 5049 4e47  l..BASIC_MAPPING
-000000a0: 5320 3d20 7b0a 2020 2020 7374 723a 2022  S = {.    str: "
-000000b0: 7374 7269 6e67 222c 0a20 2020 2069 6e74  string",.    int
-000000c0: 3a20 2269 6e74 6567 6572 222c 0a20 2020  : "integer",.   
-000000d0: 2062 6f6f 6c3a 2022 626f 6f6c 6561 6e22   bool: "boolean"
-000000e0: 2c0a 2020 2020 6279 7465 733a 2022 626c  ,.    bytes: "bl
-000000f0: 6f62 222c 0a20 2020 2066 6c6f 6174 3a20  ob",.    float: 
-00000100: 2264 6f75 626c 6522 2c0a 2020 2020 6f62  "double",.    ob
-00000110: 6a65 6374 3a20 226a 736f 6e22 2c0a 2020  ject: "json",.  
-00000120: 2020 4465 6369 6d61 6c3a 2022 6465 6369    Decimal: "deci
-00000130: 6d61 6c28 3130 2c32 2922 2c0a 2020 2020  mal(10,2)",.    
-00000140: 6474 2e64 6174 653a 2022 6461 7465 222c  dt.date: "date",
-00000150: 0a20 2020 2064 742e 7469 6d65 3a20 2274  .    dt.time: "t
-00000160: 696d 6522 2c0a 2020 2020 6474 2e64 6174  ime",.    dt.dat
-00000170: 6574 696d 653a 2022 6461 7465 7469 6d65  etime: "datetime
-00000180: 222c 0a7d 0a0a 0a63 6c61 7373 205f 5479  ",.}...class _Ty
-00000190: 7065 733a 0a20 2020 204e 4f4e 4554 5950  pes:.    NONETYP
-000001a0: 4520 3d20 7479 7065 284e 6f6e 6529 0a0a  E = type(None)..
-000001b0: 0a23 2074 6865 2069 6e70 7574 2061 6e64  .# the input and
-000001c0: 206f 7574 7075 7420 6f66 2054 7970 6544   output of TypeD
-000001d0: 414c 2e64 6566 696e 650a 5420 3d20 7479  AL.define.T = ty
-000001e0: 7069 6e67 2e54 7970 6556 6172 2822 5422  ping.TypeVar("T"
-000001f0: 2c20 7479 7069 6e67 2e54 7970 655b 2254  , typing.Type["T
-00000200: 7970 6564 5461 626c 6522 5d2c 2074 7970  ypedTable"], typ
-00000210: 696e 672e 5479 7065 5b22 5461 626c 6522  ing.Type["Table"
-00000220: 5d29 0a0a 0a63 6c61 7373 2054 7970 6544  ])...class TypeD
-00000230: 414c 2870 7964 616c 2e44 414c 293a 0a20  AL(pydal.DAL):. 
-00000240: 2020 2022 2222 4044 796e 616d 6963 4174     """@DynamicAt
-00000250: 7472 7322 2222 0a0a 2020 2020 6461 6c3a  trs"""..    dal:
-00000260: 2054 6162 6c65 0a0a 2020 2020 6465 6661   Table..    defa
-00000270: 756c 745f 6b77 6172 6773 203d 207b 0a20  ult_kwargs = {. 
-00000280: 2020 2020 2020 2023 2066 6965 6c64 7320         # fields 
-00000290: 6172 6520 2772 6571 7569 7265 6427 2028  are 'required' (
-000002a0: 6e6f 746e 756c 6c29 2062 7920 6465 6661  notnull) by defa
-000002b0: 756c 743a 0a20 2020 2020 2020 2022 6e6f  ult:.        "no
-000002c0: 746e 756c 6c22 3a20 5472 7565 2c0a 2020  tnull": True,.  
-000002d0: 2020 7d0a 0a20 2020 2064 6566 2064 6566    }..    def def
-000002e0: 696e 6528 7365 6c66 2c20 636c 733a 2054  ine(self, cls: T
-000002f0: 2920 2d3e 2054 3a0a 2020 2020 2020 2020  ) -> T:.        
-00000300: 2320 7768 656e 205f 5f66 7574 7572 655f  # when __future_
-00000310: 5f2e 616e 6e6f 7461 7469 6f6e 7320 6973  _.annotations is
-00000320: 2069 6d70 6c65 6d65 6e74 6564 2c20 636c   implemented, cl
-00000330: 732e 5f5f 616e 6e6f 7461 7469 6f6e 735f  s.__annotations_
-00000340: 5f20 7769 6c6c 206e 6f74 2077 6f72 6b20  _ will not work 
-00000350: 616e 796d 6f72 6520 6173 2062 656c 6f77  anymore as below
-00000360: 2e0a 2020 2020 2020 2020 2320 7072 6f70  ..        # prop
-00000370: 6572 2077 6179 2074 6f20 6861 6e64 6c65  er way to handle
-00000380: 2074 6869 7320 776f 756c 6420 6265 2028   this would be (
-00000390: 6275 7420 6769 7665 7320 6572 726f 7220  but gives error 
-000003a0: 7269 6768 7420 6e6f 7720 6475 6520 746f  right now due to
-000003b0: 2054 6162 6c65 2069 6d70 6c65 6d65 6e74   Table implement
-000003c0: 696e 6720 6d61 6769 6320 6d65 7468 6f64  ing magic method
-000003d0: 7329 3a0a 2020 2020 2020 2020 2320 7479  s):.        # ty
-000003e0: 7069 6e67 2e67 6574 5f74 7970 655f 6869  ping.get_type_hi
-000003f0: 6e74 7328 636c 732c 2067 6c6f 6261 6c6e  nts(cls, globaln
-00000400: 733d 4e6f 6e65 2c20 6c6f 6361 6c6e 733d  s=None, localns=
-00000410: 4e6f 6e65 290a 0a20 2020 2020 2020 2023  None)..        #
-00000420: 2064 6972 7479 2077 6179 2028 7769 7468   dirty way (with
-00000430: 2065 7669 6c20 6576 616c 293a 0a20 2020   evil eval):.   
-00000440: 2020 2020 2023 205b 6576 616c 2876 2920       # [eval(v) 
-00000450: 666f 7220 6b2c 2076 2069 6e20 636c 732e  for k, v in cls.
-00000460: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f2e  __annotations__.
-00000470: 6974 656d 7328 295d 0a20 2020 2020 2020  items()].       
-00000480: 2023 2074 6869 7320 686f 7765 7665 7220   # this however 
-00000490: 616c 736f 2073 746f 7073 2077 6f72 6b69  also stops worki
-000004a0: 6e67 2077 6865 6e20 7661 7269 6162 6c65  ng when variable
-000004b0: 7320 6f75 7473 6964 6520 7468 6973 2073  s outside this s
-000004c0: 636f 7065 206f 7220 6576 656e 2072 6566  cope or even ref
-000004d0: 6572 656e 6365 7320 746f 206f 7468 6572  erences to other
-000004e0: 0a20 2020 2020 2020 2023 206f 626a 6563  .        # objec
-000004f0: 7473 2061 7265 2075 7365 642e 2053 6f20  ts are used. So 
-00000500: 666f 7220 6e6f 772c 2074 6869 7320 7061  for now, this pa
-00000510: 636b 6167 6520 7769 6c6c 204e 4f54 2077  ckage will NOT w
-00000520: 6f72 6b20 7768 656e 2066 726f 6d20 5f5f  ork when from __
-00000530: 6675 7475 7265 5f5f 2069 6d70 6f72 7420  future__ import 
-00000540: 616e 6e6f 7461 7469 6f6e 7320 6973 2075  annotations is u
-00000550: 7365 642c 0a20 2020 2020 2020 2023 2061  sed,.        # a
-00000560: 6e64 206d 6967 6874 2062 7265 616b 2069  nd might break i
-00000570: 6e20 7468 6520 6675 7475 7265 2c20 7768  n the future, wh
-00000580: 656e 2074 6869 7320 616e 6e6f 7461 7469  en this annotati
-00000590: 6f6e 7320 6265 6861 7669 6f72 2069 7320  ons behavior is 
-000005a0: 656e 6162 6c65 6420 6279 2064 6566 6175  enabled by defau
-000005b0: 6c74 2e0a 2020 2020 2020 2020 2320 746f  lt..        # to
-000005c0: 646f 3a20 6164 6420 746f 2063 6176 6561  do: add to cavea
-000005d0: 7473 0a0a 2020 2020 2020 2020 2320 6e6f  ts..        # no
-000005e0: 6e2d 616e 6e6f 7461 7465 6420 7661 7269  n-annotated vari
-000005f0: 6162 6c65 7320 6861 7665 2074 6f20 6265  ables have to be
-00000600: 2070 6173 7365 6420 746f 2064 6566 696e   passed to defin
-00000610: 655f 7461 626c 6520 6173 206b 7761 7267  e_table as kwarg
-00000620: 730a 0a20 2020 2020 2020 2074 6162 6c65  s..        table
-00000630: 6e61 6d65 203d 2073 656c 662e 5f74 6f5f  name = self._to_
-00000640: 736e 616b 6528 636c 732e 5f5f 6e61 6d65  snake(cls.__name
-00000650: 5f5f 290a 2020 2020 2020 2020 6669 656c  __).        fiel
-00000660: 6473 203d 205b 0a20 2020 2020 2020 2020  ds = [.         
-00000670: 2020 2073 656c 662e 5f74 6f5f 6669 656c     self._to_fiel
-00000680: 6428 666e 616d 652c 2066 7479 7065 2920  d(fname, ftype) 
-00000690: 666f 7220 666e 616d 652c 2066 7479 7065  for fname, ftype
-000006a0: 2069 6e20 636c 732e 5f5f 616e 6e6f 7461   in cls.__annota
-000006b0: 7469 6f6e 735f 5f2e 6974 656d 7328 290a  tions__.items().
-000006c0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000006d0: 2020 6f74 6865 725f 6b77 6172 6773 203d    other_kwargs =
-000006e0: 207b 0a20 2020 2020 2020 2020 2020 206b   {.            k
-000006f0: 3a20 760a 2020 2020 2020 2020 2020 2020  : v.            
-00000700: 666f 7220 6b2c 2076 2069 6e20 636c 732e  for k, v in cls.
-00000710: 5f5f 6469 6374 5f5f 2e69 7465 6d73 2829  __dict__.items()
-00000720: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000730: 6b20 6e6f 7420 696e 2063 6c73 2e5f 5f61  k not in cls.__a
-00000740: 6e6e 6f74 6174 696f 6e73 5f5f 2061 6e64  nnotations__ and
-00000750: 206e 6f74 206b 2e73 7461 7274 7377 6974   not k.startswit
-00000760: 6828 225f 2229 0a20 2020 2020 2020 207d  h("_").        }
-00000770: 0a0a 2020 2020 2020 2020 7461 626c 6520  ..        table 
-00000780: 3d20 7365 6c66 2e64 6566 696e 655f 7461  = self.define_ta
-00000790: 626c 6528 7461 626c 656e 616d 652c 202a  ble(tablename, *
-000007a0: 6669 656c 6473 2c20 2a2a 6f74 6865 725f  fields, **other_
-000007b0: 6b77 6172 6773 290a 0a20 2020 2020 2020  kwargs)..       
-000007c0: 2063 6c73 2e5f 5f73 6574 5f69 6e74 6572   cls.__set_inter
-000007d0: 6e61 6c73 5f5f 2864 623d 7365 6c66 2c20  nals__(db=self, 
-000007e0: 7461 626c 653d 7461 626c 6529 0a0a 2020  table=table)..  
-000007f0: 2020 2020 2020 2320 7468 6520 4143 5455        # the ACTU
-00000800: 414c 206f 7574 7075 7420 6973 206e 6f74  AL output is not
-00000810: 2054 7970 6564 5461 626c 6520 6275 7420   TypedTable but 
-00000820: 7261 7468 6572 2070 7964 616c 2e54 6162  rather pydal.Tab
-00000830: 6c65 0a20 2020 2020 2020 2023 2062 7574  le.        # but
-00000840: 2074 656c 6c69 6e67 2074 6865 2065 6469   telling the edi
-00000850: 746f 7220 6974 2069 7320 5420 6865 6c70  tor it is T help
-00000860: 7320 7769 7468 2068 696e 7469 6e67 2e0a  s with hinting..
-00000870: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00000880: 6162 6c65 0a0a 2020 2020 6465 6620 5f5f  able..    def __
-00000890: 6361 6c6c 5f5f 2873 656c 662c 202a 6172  call__(self, *ar
-000008a0: 6773 2c20 2a2a 6b77 6172 6773 2920 2d3e  gs, **kwargs) ->
-000008b0: 2070 7964 616c 2e6f 626a 6563 7473 2e53   pydal.objects.S
-000008c0: 6574 3a0a 2020 2020 2020 2020 6172 6773  et:.        args
-000008d0: 203d 206c 6973 7428 6172 6773 290a 2020   = list(args).  
-000008e0: 2020 2020 2020 6966 2061 7267 733a 0a20        if args:. 
-000008f0: 2020 2020 2020 2020 2020 2063 6c73 203d             cls =
-00000900: 2061 7267 735b 305d 0a20 2020 2020 2020   args[0].       
-00000910: 2020 2020 2069 6620 6973 7375 6263 6c61       if issubcla
-00000920: 7373 2874 7970 6528 636c 7329 2c20 7479  ss(type(cls), ty
-00000930: 7065 2920 616e 6420 6973 7375 6263 6c61  pe) and issubcla
-00000940: 7373 2863 6c73 2c20 5479 7065 6454 6162  ss(cls, TypedTab
-00000950: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
-00000960: 2020 2020 2023 2074 6162 6c65 2064 6566       # table def
-00000970: 696e 6564 2077 6974 686f 7574 2040 6462  ined without @db
-00000980: 2e64 6566 696e 6520 6465 636f 7261 746f  .define decorato
-00000990: 7221 0a20 2020 2020 2020 2020 2020 2020  r!.             
-000009a0: 2020 2061 7267 735b 305d 203d 2063 6c73     args[0] = cls
-000009b0: 2e69 6420 213d 204e 6f6e 650a 0a20 2020  .id != None..   
-000009c0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-000009d0: 7228 292e 5f5f 6361 6c6c 5f5f 282a 6172  r().__call__(*ar
-000009e0: 6773 2c20 2a2a 6b77 6172 6773 290a 0a20  gs, **kwargs).. 
-000009f0: 2020 2023 2074 6f64 6f3a 2069 6e73 6572     # todo: inser
-00000a00: 7420 6574 6320 7368 6164 6f77 656e 3f0a  t etc shadowen?.
-00000a10: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00000a20: 640a 2020 2020 6465 6620 5f62 7569 6c64  d.    def _build
-00000a30: 5f66 6965 6c64 2863 6c73 2c20 6e61 6d65  _field(cls, name
-00000a40: 2c20 7479 7065 2c20 2a2a 6b77 293a 0a20  , type, **kw):. 
-00000a50: 2020 2020 2020 2072 6574 7572 6e20 4669         return Fi
-00000a60: 656c 6428 6e61 6d65 2c20 7479 7065 2c20  eld(name, type, 
-00000a70: 2a2a 7b2a 2a63 6c73 2e64 6566 6175 6c74  **{**cls.default
-00000a80: 5f6b 7761 7267 732c 202a 2a6b 777d 290a  _kwargs, **kw}).
-00000a90: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00000aa0: 640a 2020 2020 6465 6620 5f74 6f5f 6669  d.    def _to_fi
-00000ab0: 656c 6428 636c 732c 2066 6e61 6d65 3a20  eld(cls, fname: 
-00000ac0: 7374 722c 2066 7479 7065 3a20 7479 7065  str, ftype: type
-00000ad0: 2c20 2a2a 6b77 293a 0a20 2020 2020 2020  , **kw):.       
-00000ae0: 2066 6e61 6d65 203d 2063 6c73 2e5f 746f   fname = cls._to
-00000af0: 5f73 6e61 6b65 2866 6e61 6d65 290a 0a20  _snake(fname).. 
-00000b00: 2020 2020 2020 2069 6620 6d61 7070 696e         if mappin
-00000b10: 6720 3a3d 2042 4153 4943 5f4d 4150 5049  g := BASIC_MAPPI
-00000b20: 4e47 532e 6765 7428 6674 7970 6529 3a0a  NGS.get(ftype):.
-00000b30: 2020 2020 2020 2020 2020 2020 2320 6261              # ba
-00000b40: 7369 2074 7970 6573 0a20 2020 2020 2020  si types.       
-00000b50: 2020 2020 2072 6574 7572 6e20 636c 732e       return cls.
-00000b60: 5f62 7569 6c64 5f66 6965 6c64 2866 6e61  _build_field(fna
-00000b70: 6d65 2c20 6d61 7070 696e 672c 202a 2a6b  me, mapping, **k
-00000b80: 7729 0a20 2020 2020 2020 2065 6c69 6620  w).        elif 
-00000b90: 6973 696e 7374 616e 6365 2866 7479 7065  isinstance(ftype
-00000ba0: 2c20 5461 626c 6529 3a0a 2020 2020 2020  , Table):.      
-00000bb0: 2020 2020 2020 2320 6462 2e74 6162 6c65        # db.table
-00000bc0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00000bd0: 7572 6e20 636c 732e 5f62 7569 6c64 5f66  urn cls._build_f
-00000be0: 6965 6c64 2866 6e61 6d65 2c20 6622 7265  ield(fname, f"re
-00000bf0: 6665 7265 6e63 6520 7b66 7479 7065 2e5f  ference {ftype._
-00000c00: 7461 626c 656e 616d 657d 222c 202a 2a6b  tablename}", **k
-00000c10: 7729 0a20 2020 2020 2020 2065 6c69 6620  w).        elif 
-00000c20: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
-00000c30: 6674 7970 6529 2c20 7479 7065 2920 616e  ftype), type) an
-00000c40: 6420 6973 7375 6263 6c61 7373 2866 7479  d issubclass(fty
-00000c50: 7065 2c20 5479 7065 6454 6162 6c65 293a  pe, TypedTable):
-00000c60: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
-00000c70: 6f6d 6554 6162 6c65 0a20 2020 2020 2020  omeTable.       
-00000c80: 2020 2020 2073 6e61 6b65 6e61 6d65 203d       snakename =
-00000c90: 2063 6c73 2e5f 746f 5f73 6e61 6b65 2866   cls._to_snake(f
-00000ca0: 7479 7065 2e5f 5f6e 616d 655f 5f29 0a20  type.__name__). 
-00000cb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000cc0: 6e20 636c 732e 5f62 7569 6c64 5f66 6965  n cls._build_fie
-00000cd0: 6c64 2866 6e61 6d65 2c20 6622 7265 6665  ld(fname, f"refe
-00000ce0: 7265 6e63 6520 7b73 6e61 6b65 6e61 6d65  rence {snakename
-00000cf0: 7d22 2c20 2a2a 6b77 290a 2020 2020 2020  }", **kw).      
-00000d00: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00000d10: 6528 6674 7970 652c 2054 7970 6564 4669  e(ftype, TypedFi
-00000d20: 656c 6454 7970 6529 3a0a 2020 2020 2020  eldType):.      
-00000d30: 2020 2020 2020 2320 4669 656c 6454 7970        # FieldTyp
-00000d40: 6528 7479 7065 2c20 2e2e 2e29 0a20 2020  e(type, ...).   
-00000d50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000d60: 6674 7970 652e 5f74 6f5f 6669 656c 6428  ftype._to_field(
-00000d70: 666e 616d 652c 202a 2a6b 7729 0a20 2020  fname, **kw).   
-00000d80: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00000d90: 616e 6365 2866 7479 7065 2c20 7479 7065  ance(ftype, type
-00000da0: 732e 4765 6e65 7269 6341 6c69 6173 293a  s.GenericAlias):
-00000db0: 0a20 2020 2020 2020 2020 2020 2023 206c  .            # l
-00000dc0: 6973 745b 2e2e 2e5d 0a20 2020 2020 2020  ist[...].       
-00000dd0: 2020 2020 205f 6368 696c 6474 7970 6520       _childtype 
-00000de0: 3d20 5479 7065 6446 6965 6c64 5479 7065  = TypedFieldType
-00000df0: 2e5f 636f 6e76 6572 745f 6765 6e65 7269  ._convert_generi
-00000e00: 635f 616c 6961 735f 6c69 7374 2866 7479  c_alias_list(fty
-00000e10: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
-00000e20: 7265 7475 726e 2063 6c73 2e5f 6275 696c  return cls._buil
-00000e30: 645f 6669 656c 6428 666e 616d 652c 2066  d_field(fname, f
-00000e40: 226c 6973 743a 7b5f 6368 696c 6474 7970  "list:{_childtyp
-00000e50: 657d 222c 202a 2a6b 7729 0a20 2020 2020  e}", **kw).     
-00000e60: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00000e70: 6365 2866 7479 7065 2c20 7479 7069 6e67  ce(ftype, typing
-00000e80: 2e5f 556e 696f 6e47 656e 6572 6963 416c  ._UnionGenericAl
-00000e90: 6961 7329 206f 7220 6973 696e 7374 616e  ias) or isinstan
-00000ea0: 6365 280a 2020 2020 2020 2020 2020 2020  ce(.            
-00000eb0: 6674 7970 652c 2074 7970 6573 2e55 6e69  ftype, types.Uni
-00000ec0: 6f6e 5479 7065 0a20 2020 2020 2020 2029  onType.        )
-00000ed0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00000ee0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00000ef0: 7479 7065 5d20 3d3d 2074 7970 6520 7c20  type] == type | 
-00000f00: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00000f10: 206d 6174 6368 2066 7479 7065 2e5f 5f61   match ftype.__a
-00000f20: 7267 735f 5f3a 0a20 2020 2020 2020 2020  rgs__:.         
-00000f30: 2020 2020 2020 2063 6173 6520 285f 6368         case (_ch
-00000f40: 696c 645f 7479 7065 2c20 5f54 7970 6573  ild_type, _Types
-00000f50: 2e4e 4f4e 4554 5950 4529 3a0a 2020 2020  .NONETYPE):.    
-00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 2320 676f 6f64 2075 6e69 6f6e 0a0a 2020  # good union..  
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2020 2320 6966 2061 2066 6965 6c64 2069    # if a field i
-00000fa0: 7320 6f70 7469 6f6e 616c 2c20 6974 2069  s optional, it i
-00000fb0: 7320 6e75 6c6c 6162 6c65 3a0a 2020 2020  s nullable:.    
-00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fd0: 6b77 5b22 6e6f 746e 756c 6c22 5d20 3d20  kw["notnull"] = 
-00000fe0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00000ff0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001000: 2063 6c73 2e5f 746f 5f66 6965 6c64 2866   cls._to_field(f
-00001010: 6e61 6d65 2c20 5f63 6869 6c64 5f74 7970  name, _child_typ
-00001020: 652c 202a 2a6b 7729 0a20 2020 2020 2020  e, **kw).       
-00001030: 2020 2020 2020 2020 2063 6173 6520 6f74           case ot
-00001040: 6865 723a 0a20 2020 2020 2020 2020 2020  her:.           
-00001050: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
-00001060: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00001070: 6f72 2866 2249 6e76 616c 6964 2074 7970  or(f"Invalid typ
-00001080: 6520 756e 696f 6e20 277b 6f74 6865 727d  e union '{other}
-00001090: 2722 290a 2020 2020 2020 2020 656c 7365  '").        else
-000010a0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-000010b0: 746f 646f 3a20 6361 7463 6820 6f74 6865  todo: catch othe
-000010c0: 7220 7479 7065 730a 2020 2020 2020 2020  r types.        
-000010d0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-000010e0: 6c65 6d65 6e74 6564 4572 726f 7228 6622  lementedError(f"
-000010f0: 556e 7375 7070 6f72 7465 6420 7479 7065  Unsupported type
-00001100: 207b 6674 7970 657d 2f7b 7479 7065 2866   {ftype}/{type(f
-00001110: 7479 7065 297d 2229 0a0a 2020 2020 4073  type)}")..    @s
-00001120: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00001130: 6465 6620 5f74 6f5f 736e 616b 6528 6361  def _to_snake(ca
-00001140: 6d65 6c3a 2073 7472 2920 2d3e 2073 7472  mel: str) -> str
-00001150: 3a0a 2020 2020 2020 2020 2320 6874 7470  :.        # http
-00001160: 733a 2f2f 7374 6163 6b6f 7665 7266 6c6f  s://stackoverflo
-00001170: 772e 636f 6d2f 612f 3434 3936 3933 3831  w.com/a/44969381
-00001180: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001190: 2222 2e6a 6f69 6e28 5b22 5f22 202b 2063  "".join(["_" + c
-000011a0: 2e6c 6f77 6572 2829 2069 6620 632e 6973  .lower() if c.is
-000011b0: 7570 7065 7228 2920 656c 7365 2063 2066  upper() else c f
-000011c0: 6f72 2063 2069 6e20 6361 6d65 6c5d 292e  or c in camel]).
-000011d0: 6c73 7472 6970 280a 2020 2020 2020 2020  lstrip(.        
-000011e0: 2020 2020 225f 220a 2020 2020 2020 2020      "_".        
-000011f0: 290a 0a0a 636c 6173 7320 5479 7065 6454  )...class TypedT
-00001200: 6162 6c65 4d65 7461 2874 7970 6529 3a0a  ableMeta(type):.
-00001210: 2020 2020 2320 6d65 7461 2063 6c61 7373      # meta class
-00001220: 2061 6c6c 6f77 7320 6765 7461 7474 7269   allows getattri
-00001230: 6275 7465 206f 6e20 636c 6173 7320 7661  bute on class va
-00001240: 7269 6162 6c65 7320 696e 7374 6561 6420  riables instead 
-00001250: 696e 7374 616e 6365 2076 6172 6961 626c  instance variabl
-00001260: 6573 0a20 2020 2064 6566 205f 5f67 6574  es.    def __get
-00001270: 6174 7472 5f5f 2873 656c 662c 206b 6579  attr__(self, key
-00001280: 293a 0a20 2020 2020 2020 2023 2067 6574  ):.        # get
-00001290: 6174 7472 2069 7320 6f6e 6c79 2063 616c  attr is only cal
-000012a0: 6c65 6420 7768 656e 2067 6574 6174 7472  led when getattr
-000012b0: 6962 7574 6520 6361 6e27 7420 6669 6e64  ibute can't find
-000012c0: 2073 6f6d 6574 6869 6e67 0a20 2020 2020   something.     
-000012d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000012e0: 5f67 6574 5f74 6162 6c65 5f63 6f6c 756d  _get_table_colum
-000012f0: 6e5f 5f28 6b65 7929 0a0a 0a63 6c61 7373  n__(key)...class
-00001300: 2054 7970 6564 5461 626c 6528 5461 626c   TypedTable(Tabl
-00001310: 652c 206d 6574 6163 6c61 7373 3d54 7970  e, metaclass=Typ
-00001320: 6564 5461 626c 654d 6574 6129 3a0a 2020  edTableMeta):.  
-00001330: 2020 6964 3a20 696e 740a 0a20 2020 2023    id: int..    #
-00001340: 2073 6574 2075 7020 6279 2064 622e 6465   set up by db.de
-00001350: 6669 6e65 3a0a 2020 2020 5f5f 6462 3a20  fine:.    __db: 
-00001360: 5479 7065 4441 4c20 3d20 4e6f 6e65 0a20  TypeDAL = None. 
-00001370: 2020 205f 5f74 6162 6c65 3a20 5461 626c     __table: Tabl
-00001380: 6520 3d20 4e6f 6e65 0a0a 2020 2020 4063  e = None..    @c
-00001390: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-000013a0: 6566 205f 5f73 6574 5f69 6e74 6572 6e61  ef __set_interna
-000013b0: 6c73 5f5f 2863 6c73 2c20 6462 2c20 7461  ls__(cls, db, ta
-000013c0: 626c 6529 3a0a 2020 2020 2020 2020 636c  ble):.        cl
-000013d0: 732e 5f5f 6462 203d 2064 620a 2020 2020  s.__db = db.    
-000013e0: 2020 2020 636c 732e 5f5f 7461 626c 6520      cls.__table 
-000013f0: 3d20 7461 626c 650a 0a20 2020 2040 636c  = table..    @cl
-00001400: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00001410: 6620 5f5f 6765 745f 7461 626c 655f 636f  f __get_table_co
-00001420: 6c75 6d6e 5f5f 2863 6c73 2c20 636f 6c29  lumn__(cls, col)
-00001430: 3a0a 2020 2020 2020 2020 2320 6462 2e74  :.        # db.t
-00001440: 6162 6c65 2e63 6f6c 202d 3e20 536f 6d65  able.col -> Some
-00001450: 5479 7065 6454 6162 6c65 2e63 6f6c 2028  TypedTable.col (
-00001460: 7669 6120 5479 7065 6454 6162 6c65 4d65  via TypedTableMe
-00001470: 7461 2e5f 5f67 6574 6174 7472 5f5f 290a  ta.__getattr__).
-00001480: 2020 2020 2020 2020 6966 2063 6c73 2e5f          if cls._
-00001490: 5f74 6162 6c65 3a0a 2020 2020 2020 2020  _table:.        
-000014a0: 2020 2020 7265 7475 726e 2063 6c73 2e5f      return cls._
-000014b0: 5f74 6162 6c65 5b63 6f6c 5d0a 0a20 2020  _table[col]..   
-000014c0: 2064 6566 205f 5f6e 6577 5f5f 2863 6c73   def __new__(cls
-000014d0: 2c20 2a61 2c20 2a2a 6b77 293a 0a20 2020  , *a, **kw):.   
-000014e0: 2020 2020 2023 2077 6865 6e20 652e 672e       # when e.g.
-000014f0: 2054 6162 6c65 2869 643d 3029 2069 7320   Table(id=0) is 
-00001500: 6361 6c6c 6564 2077 6974 686f 7574 2064  called without d
-00001510: 622e 6465 6669 6e65 2c0a 2020 2020 2020  b.define,.      
-00001520: 2020 2320 7468 6973 2063 6174 6368 6573    # this catches
-00001530: 2069 7420 616e 6420 666f 7277 6172 6473   it and forwards
-00001540: 2066 6f72 2070 726f 7065 7220 6265 6861   for proper beha
-00001550: 7669 6f72 0a20 2020 2020 2020 2072 6574  vior.        ret
-00001560: 7572 6e20 636c 732e 5f5f 7461 626c 6528  urn cls.__table(
-00001570: 2a61 2c20 2a2a 6b77 290a 0a20 2020 2040  *a, **kw)..    @
-00001580: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-00001590: 6465 6620 696e 7365 7274 2863 6c73 2c20  def insert(cls, 
-000015a0: 2a2a 6669 656c 6473 293a 0a20 2020 2020  **fields):.     
-000015b0: 2020 2023 2074 6869 7320 6973 206f 6e6c     # this is onl
-000015c0: 7920 6361 6c6c 6564 2077 6865 6e20 6462  y called when db
-000015d0: 2e64 6566 696e 6520 6973 206e 6f74 2075  .define is not u
-000015e0: 7365 6420 6173 2061 2064 6563 6f72 6174  sed as a decorat
-000015f0: 6f72 0a20 2020 2020 2020 2023 2063 6c73  or.        # cls
-00001600: 2e5f 5f74 6162 6c65 2066 756e 6374 696f  .__table functio
-00001610: 6e73 2061 7320 2773 656c 6627 0a20 2020  ns as 'self'.   
-00001620: 2020 2020 2073 7570 6572 2829 2e69 6e73       super().ins
-00001630: 6572 7428 636c 732e 5f5f 7461 626c 652c  ert(cls.__table,
-00001640: 202a 2a66 6965 6c64 7329 0a0a 0a23 2062   **fields)...# b
-00001650: 6163 6b77 6172 6473 2063 6f6d 7061 743a  ackwards compat:
-00001660: 0a54 7970 6564 526f 7720 3d20 5479 7065  .TypedRow = Type
-00001670: 6454 6162 6c65 0a0a 0a63 6c61 7373 2054  dTable...class T
-00001680: 7970 6564 4669 656c 6454 7970 6528 4669  ypedFieldType(Fi
-00001690: 656c 6429 3a0a 2020 2020 5f74 6162 6c65  eld):.    _table
-000016a0: 203d 2022 3c61 6e79 2074 6162 6c65 3e22   = "<any table>"
-000016b0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-000016c0: 5f5f 2873 656c 662c 205f 7479 7065 2c20  __(self, _type, 
-000016d0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-000016e0: 2020 2073 656c 662e 7479 7065 203d 205f     self.type = _
-000016f0: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
-00001700: 662e 6b77 6172 6773 203d 206b 7761 7267  f.kwargs = kwarg
-00001710: 730a 0a20 2020 2064 6566 205f 5f72 6570  s..    def __rep
-00001720: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
-00001730: 2020 2073 203d 2073 656c 662e 5f5f 7374     s = self.__st
-00001740: 725f 5f28 290a 2020 2020 2020 2020 7265  r__().        re
-00001750: 7475 726e 2066 223c 7b73 7d20 7769 7468  turn f"<{s} with
-00001760: 206f 7074 696f 6e73 207b 7365 6c66 2e6b   options {self.k
-00001770: 7761 7267 737d 3e22 0a0a 2020 2020 6465  wargs}>"..    de
-00001780: 6620 5f5f 7374 725f 5f28 7365 6c66 293a  f __str__(self):
-00001790: 0a20 2020 2020 2020 2069 6620 2274 7970  .        if "typ
-000017a0: 6522 2069 6e20 7365 6c66 2e6b 7761 7267  e" in self.kwarg
-000017b0: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-000017c0: 203d 2073 656c 662e 6b77 6172 6773 5b22   = self.kwargs["
-000017d0: 7479 7065 225d 0a20 2020 2020 2020 2065  type"].        e
-000017e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000017f0: 2074 203d 2073 656c 662e 7479 7065 2e5f   t = self.type._
-00001800: 5f6e 616d 655f 5f20 6966 2069 7373 7562  _name__ if issub
-00001810: 636c 6173 7328 7479 7065 2873 656c 662e  class(type(self.
-00001820: 7479 7065 292c 2074 7970 6529 2065 6c73  type), type) els
-00001830: 6520 7365 6c66 2e74 7970 650a 2020 2020  e self.type.    
-00001840: 2020 2020 7265 7475 726e 2066 2254 7970      return f"Typ
-00001850: 6564 4669 656c 642e 7b74 7d22 0a0a 2020  edField.{t}"..  
-00001860: 2020 6465 6620 5f74 6f5f 6669 656c 6428    def _to_field(
-00001870: 7365 6c66 2c20 6e61 6d65 3a20 7374 722c  self, name: str,
-00001880: 202a 2a65 7874 7261 5f6b 7761 7267 7329   **extra_kwargs)
-00001890: 202d 3e20 4669 656c 643a 0a20 2020 2020   -> Field:.     
-000018a0: 2020 206f 7468 6572 5f6b 7761 7267 7320     other_kwargs 
-000018b0: 3d20 7365 6c66 2e6b 7761 7267 732e 636f  = self.kwargs.co
-000018c0: 7079 2829 0a20 2020 2020 2020 206f 7468  py().        oth
-000018d0: 6572 5f6b 7761 7267 732e 7570 6461 7465  er_kwargs.update
-000018e0: 2865 7874 7261 5f6b 7761 7267 7329 0a20  (extra_kwargs). 
-000018f0: 2020 2020 2020 2069 6620 2274 7970 6522         if "type"
-00001900: 2069 6e20 6f74 6865 725f 6b77 6172 6773   in other_kwargs
-00001910: 3a0a 2020 2020 2020 2020 2020 2020 5f74  :.            _t
-00001920: 7970 6520 3d20 6f74 6865 725f 6b77 6172  ype = other_kwar
-00001930: 6773 2e70 6f70 2822 7479 7065 2229 0a20  gs.pop("type"). 
-00001940: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00001950: 2020 2020 2020 2020 205f 7479 7065 203d           _type =
-00001960: 2073 656c 662e 5f74 6f5f 6669 656c 645f   self._to_field_
-00001970: 7479 7065 2873 656c 662e 7479 7065 290a  type(self.type).
-00001980: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001990: 5479 7065 4441 4c2e 5f62 7569 6c64 5f66  TypeDAL._build_f
-000019a0: 6965 6c64 286e 616d 652c 205f 7479 7065  ield(name, _type
-000019b0: 2c20 2a2a 6f74 6865 725f 6b77 6172 6773  , **other_kwargs
-000019c0: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
-000019d0: 686f 640a 2020 2020 6465 6620 5f74 6f5f  hod.    def _to_
-000019e0: 6669 656c 645f 7479 7065 2863 6c73 2c20  field_type(cls, 
-000019f0: 5f74 7970 653a 2074 7970 6529 202d 3e20  _type: type) -> 
-00001a00: 7374 723a 0a20 2020 2020 2020 2023 2074  str:.        # t
-00001a10: 6f64 6f3a 206d 6572 6765 2077 6974 6820  odo: merge with 
-00001a20: 5479 7065 4441 4c2e 5f74 6f5f 6669 656c  TypeDAL._to_fiel
-00001a30: 6420 286b 696e 6461 3f29 0a20 2020 2020  d (kinda?).     
-00001a40: 2020 2069 6620 6d61 7070 696e 6720 3a3d     if mapping :=
-00001a50: 2042 4153 4943 5f4d 4150 5049 4e47 532e   BASIC_MAPPINGS.
-00001a60: 6765 7428 5f74 7970 6529 3a0a 2020 2020  get(_type):.    
-00001a70: 2020 2020 2020 2020 2320 6261 7369 6320          # basic 
-00001a80: 7479 7065 730a 2020 2020 2020 2020 2020  types.          
-00001a90: 2020 7265 7475 726e 206d 6170 7069 6e67    return mapping
-00001aa0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-00001ab0: 7375 6263 6c61 7373 2874 7970 6528 5f74  subclass(type(_t
-00001ac0: 7970 6529 2c20 7479 7065 2920 616e 6420  ype), type) and 
-00001ad0: 6973 7375 6263 6c61 7373 285f 7479 7065  issubclass(_type
-00001ae0: 2c20 5479 7065 6454 6162 6c65 293a 0a20  , TypedTable):. 
-00001af0: 2020 2020 2020 2020 2020 2023 2053 6f6d             # Som
-00001b00: 6554 6162 6c65 0a20 2020 2020 2020 2020  eTable.         
-00001b10: 2020 2073 6e61 6b65 6e61 6d65 203d 2054     snakename = T
-00001b20: 7970 6544 414c 2e5f 746f 5f73 6e61 6b65  ypeDAL._to_snake
-00001b30: 285f 7479 7065 2e5f 5f6e 616d 655f 5f29  (_type.__name__)
-00001b40: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001b50: 7572 6e20 6622 7265 6665 7265 6e63 6520  urn f"reference 
-00001b60: 7b73 6e61 6b65 6e61 6d65 7d22 0a20 2020  {snakename}".   
-00001b70: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00001b80: 616e 6365 285f 7479 7065 2c20 5461 626c  ance(_type, Tabl
-00001b90: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00001ba0: 2320 6462 2e73 6f6d 6574 6162 6c65 0a20  # db.sometable. 
-00001bb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001bc0: 6e20 6622 7265 6665 7265 6e63 6520 7b5f  n f"reference {_
-00001bd0: 7479 7065 2e5f 7461 626c 656e 616d 657d  type._tablename}
-00001be0: 220a 2020 2020 2020 2020 656c 6966 2069  ".        elif i
-00001bf0: 7369 6e73 7461 6e63 6528 5f74 7970 652c  sinstance(_type,
-00001c00: 2074 7970 6573 2e47 656e 6572 6963 416c   types.GenericAl
-00001c10: 6961 7329 3a0a 2020 2020 2020 2020 2020  ias):.          
-00001c20: 2020 2320 6c69 7374 5b74 7970 655d 0a20    # list[type]. 
-00001c30: 2020 2020 2020 2020 2020 205f 6368 696c             _chil
-00001c40: 645f 7479 7065 203d 2063 6c73 2e5f 636f  d_type = cls._co
-00001c50: 6e76 6572 745f 6765 6e65 7269 635f 616c  nvert_generic_al
-00001c60: 6961 735f 6c69 7374 285f 7479 7065 290a  ias_list(_type).
-00001c70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001c80: 726e 2066 226c 6973 743a 7b5f 6368 696c  rn f"list:{_chil
-00001c90: 645f 7479 7065 7d22 0a20 2020 2020 2020  d_type}".       
-00001ca0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00001cb0: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-00001cc0: 656d 656e 7465 6445 7272 6f72 285f 7479  ementedError(_ty
-00001cd0: 7065 290a 0a20 2020 2040 636c 6173 736d  pe)..    @classm
-00001ce0: 6574 686f 640a 2020 2020 6465 6620 5f63  ethod.    def _c
-00001cf0: 6f6e 7665 7274 5f67 656e 6572 6963 5f61  onvert_generic_a
-00001d00: 6c69 6173 5f6c 6973 7428 636c 732c 2066  lias_list(cls, f
-00001d10: 7479 7065 293a 0a20 2020 2020 2020 2023  type):.        #
-00001d20: 2065 2e67 2e20 6c69 7374 5b73 7472 0a20   e.g. list[str. 
-00001d30: 2020 2020 2020 2062 6173 6574 7970 6520         basetype 
-00001d40: 3d20 6674 7970 652e 5f5f 6f72 6967 696e  = ftype.__origin
-00001d50: 5f5f 0a20 2020 2020 2020 2023 2065 2e67  __.        # e.g
-00001d60: 2e20 6c69 7374 0a20 2020 2020 2020 2069  . list.        i
-00001d70: 6620 6261 7365 7479 7065 2069 7320 6e6f  f basetype is no
-00001d80: 7420 6c69 7374 3a0a 2020 2020 2020 2020  t list:.        
-00001d90: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-00001da0: 6c65 6d65 6e74 6564 4572 726f 7228 224f  lementedError("O
-00001db0: 6e6c 7920 7061 7261 6d65 7465 7269 7a65  nly parameterize
-00001dc0: 6420 6c69 7374 2069 7320 6375 7272 656e  d list is curren
-00001dd0: 746c 7920 6176 6169 6c61 626c 652e 2229  tly available.")
-00001de0: 0a20 2020 2020 2020 2063 6869 6c64 7479  .        childty
-00001df0: 7065 203d 2066 7479 7065 2e5f 5f61 7267  pe = ftype.__arg
-00001e00: 735f 5f5b 305d 0a0a 2020 2020 2020 2020  s__[0]..        
-00001e10: 7265 7475 726e 2063 6c73 2e5f 746f 5f66  return cls._to_f
-00001e20: 6965 6c64 5f74 7970 6528 6368 696c 6474  ield_type(childt
-00001e30: 7970 6529 0a0a 0a53 203d 2074 7970 696e  ype)...S = typin
-00001e40: 672e 5479 7065 5661 7228 2253 2229 0a0a  g.TypeVar("S")..
-00001e50: 0a63 6c61 7373 2054 7970 6564 526f 7773  .class TypedRows
-00001e60: 2874 7970 696e 672e 436f 6c6c 6563 7469  (typing.Collecti
-00001e70: 6f6e 5b53 5d2c 2052 6f77 7329 3a0a 2020  on[S], Rows):.  
-00001e80: 2020 2222 220a 2020 2020 4361 6e20 6265    """.    Can be
-00001e90: 2075 7365 6420 6173 2074 6865 2072 6574   used as the ret
-00001ea0: 7572 6e20 7479 7065 206f 6620 6120 2e73  urn type of a .s
-00001eb0: 656c 6563 7428 290a 2020 2020 652e 672e  elect().    e.g.
-00001ec0: 0a0a 2020 2020 7065 6f70 6c65 3a20 5479  ..    people: Ty
-00001ed0: 7065 6452 6f77 735b 5065 7273 6f6e 5d20  pedRows[Person] 
-00001ee0: 3d20 6462 2850 6572 736f 6e29 2e73 656c  = db(Person).sel
-00001ef0: 6563 7428 290a 2020 2020 2222 220a       ect().    """.
+00000000: 0000 0000 0000 0000 0200 0000 0000 0000  ................
+00000010: 0e00 0000 0000 0000 4e6f 6e65 436f 6d70  ........NoneComp
+00000020: 6172 6973 6f6e 3100 0000 0000 0000 436f  arison1.......Co
+00000030: 6d70 6172 6973 6f6e 2074 6f20 604e 6f6e  mparison to `Non
+00000040: 6560 2073 686f 756c 6420 6265 2060 636f  e` should be `co
+00000050: 6e64 2069 7320 6e6f 7420 4e6f 6e65 6001  nd is not None`.
+00000060: 1f00 0000 0000 0000 5265 706c 6163 6520  ........Replace 
+00000070: 7769 7468 2060 636f 6e64 2069 7320 6e6f  with `cond is no
+00000080: 7420 4e6f 6e65 60b7 0900 00bb 0900 0001  t None`.........
+00000090: 0100 0000 0000 0000 ad09 0000 bb09 0000  ................
+000000a0: 0112 0000 0000 0000 0063 6c73 2e69 6420  .........cls.id 
+000000b0: 6973 206e 6f74 204e 6f6e 6503 0000 0000  is not None.....
+000000c0: 0000 0000 0000 00b7 0900 000c 0000 0000  ................
+000000d0: 0000 0055 6e75 7365 6449 6d70 6f72 7427  ...UnusedImport'
+000000e0: 0000 0000 0000 0060 7079 6461 6c2e 6f62  .......`pydal.ob
+000000f0: 6a65 6374 732e 526f 7760 2069 6d70 6f72  jects.Row` impor
+00000100: 7465 6420 6275 7420 756e 7573 6564 0129  ted but unused.)
+00000110: 0000 0000 0000 0052 656d 6f76 6520 756e  .......Remove un
+00000120: 7573 6564 2069 6d70 6f72 743a 2060 7079  used import: `py
+00000130: 6461 6c2e 6f62 6a65 6374 732e 526f 7760  dal.objects.Row`
+00000140: 2700 0000 2a00 0000 0000 0000 0000 0000  '...*...........
+00000150: 0027 0000 0001 0000 0000 0000 0032 0000  .'...........2..
+00000160: 0000 0000 002f 686f 6d65 2f72 6f62 696e  ...../home/robin
+00000170: 2f77 6572 6b2f 4569 6765 6e2f 7479 7065  /werk/Eigen/type
+00000180: 6461 6c2f 7372 632f 7479 7065 6461 6c2f  dal/src/typedal/
+00000190: 636f 7265 2e70 79fe 1e00 0000 0000 0069  core.py........i
+000001a0: 6d70 6f72 7420 7079 6461 6c0a 6672 6f6d  mport pydal.from
+000001b0: 2070 7964 616c 2e6f 626a 6563 7473 2069   pydal.objects i
+000001c0: 6d70 6f72 7420 526f 772c 2052 6f77 732c  mport Row, Rows,
+000001d0: 2046 6965 6c64 2c20 5461 626c 6520 2023   Field, Table  #
+000001e0: 202a 3f0a 696d 706f 7274 2074 7970 696e   *?.import typin
+000001f0: 670a 696d 706f 7274 2074 7970 6573 0a69  g.import types.i
+00000200: 6d70 6f72 7420 6461 7465 7469 6d65 2061  mport datetime a
+00000210: 7320 6474 0a66 726f 6d20 6465 6369 6d61  s dt.from decima
+00000220: 6c20 696d 706f 7274 2044 6563 696d 616c  l import Decimal
+00000230: 0a0a 4241 5349 435f 4d41 5050 494e 4753  ..BASIC_MAPPINGS
+00000240: 203d 207b 0a20 2020 2073 7472 3a20 2273   = {.    str: "s
+00000250: 7472 696e 6722 2c0a 2020 2020 696e 743a  tring",.    int:
+00000260: 2022 696e 7465 6765 7222 2c0a 2020 2020   "integer",.    
+00000270: 626f 6f6c 3a20 2262 6f6f 6c65 616e 222c  bool: "boolean",
+00000280: 0a20 2020 2062 7974 6573 3a20 2262 6c6f  .    bytes: "blo
+00000290: 6222 2c0a 2020 2020 666c 6f61 743a 2022  b",.    float: "
+000002a0: 646f 7562 6c65 222c 0a20 2020 206f 626a  double",.    obj
+000002b0: 6563 743a 2022 6a73 6f6e 222c 0a20 2020  ect: "json",.   
+000002c0: 2044 6563 696d 616c 3a20 2264 6563 696d   Decimal: "decim
+000002d0: 616c 2831 302c 3229 222c 0a20 2020 2064  al(10,2)",.    d
+000002e0: 742e 6461 7465 3a20 2264 6174 6522 2c0a  t.date: "date",.
+000002f0: 2020 2020 6474 2e74 696d 653a 2022 7469      dt.time: "ti
+00000300: 6d65 222c 0a20 2020 2064 742e 6461 7465  me",.    dt.date
+00000310: 7469 6d65 3a20 2264 6174 6574 696d 6522  time: "datetime"
+00000320: 2c0a 7d0a 0a0a 636c 6173 7320 5f54 7970  ,.}...class _Typ
+00000330: 6573 3a0a 2020 2020 4e4f 4e45 5459 5045  es:.    NONETYPE
+00000340: 203d 2074 7970 6528 4e6f 6e65 290a 0a0a   = type(None)...
+00000350: 2320 7468 6520 696e 7075 7420 616e 6420  # the input and 
+00000360: 6f75 7470 7574 206f 6620 5479 7065 4441  output of TypeDA
+00000370: 4c2e 6465 6669 6e65 0a54 203d 2074 7970  L.define.T = typ
+00000380: 696e 672e 5479 7065 5661 7228 2254 222c  ing.TypeVar("T",
+00000390: 2074 7970 696e 672e 5479 7065 5b22 5479   typing.Type["Ty
+000003a0: 7065 6454 6162 6c65 225d 2c20 7479 7069  pedTable"], typi
+000003b0: 6e67 2e54 7970 655b 2254 6162 6c65 225d  ng.Type["Table"]
+000003c0: 290a 0a0a 636c 6173 7320 5479 7065 4441  )...class TypeDA
+000003d0: 4c28 7079 6461 6c2e 4441 4c29 3a0a 2020  L(pydal.DAL):.  
+000003e0: 2020 2222 2240 4479 6e61 6d69 6341 7474    """@DynamicAtt
+000003f0: 7273 2222 220a 0a20 2020 2064 616c 3a20  rs"""..    dal: 
+00000400: 5461 626c 650a 0a20 2020 2064 6566 6175  Table..    defau
+00000410: 6c74 5f6b 7761 7267 7320 3d20 7b0a 2020  lt_kwargs = {.  
+00000420: 2020 2020 2020 2320 6669 656c 6473 2061        # fields a
+00000430: 7265 2027 7265 7175 6972 6564 2720 286e  re 'required' (n
+00000440: 6f74 6e75 6c6c 2920 6279 2064 6566 6175  otnull) by defau
+00000450: 6c74 3a0a 2020 2020 2020 2020 226e 6f74  lt:.        "not
+00000460: 6e75 6c6c 223a 2054 7275 652c 0a20 2020  null": True,.   
+00000470: 207d 0a0a 2020 2020 6465 6620 6465 6669   }..    def defi
+00000480: 6e65 2873 656c 662c 2063 6c73 3a20 5429  ne(self, cls: T)
+00000490: 202d 3e20 543a 0a20 2020 2020 2020 2023   -> T:.        #
+000004a0: 2077 6865 6e20 5f5f 6675 7475 7265 5f5f   when __future__
+000004b0: 2e61 6e6e 6f74 6174 696f 6e73 2069 7320  .annotations is 
+000004c0: 696d 706c 656d 656e 7465 642c 2063 6c73  implemented, cls
+000004d0: 2e5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
+000004e0: 2077 696c 6c20 6e6f 7420 776f 726b 2061   will not work a
+000004f0: 6e79 6d6f 7265 2061 7320 6265 6c6f 772e  nymore as below.
+00000500: 0a20 2020 2020 2020 2023 2070 726f 7065  .        # prope
+00000510: 7220 7761 7920 746f 2068 616e 646c 6520  r way to handle 
+00000520: 7468 6973 2077 6f75 6c64 2062 6520 2862  this would be (b
+00000530: 7574 2067 6976 6573 2065 7272 6f72 2072  ut gives error r
+00000540: 6967 6874 206e 6f77 2064 7565 2074 6f20  ight now due to 
+00000550: 5461 626c 6520 696d 706c 656d 656e 7469  Table implementi
+00000560: 6e67 206d 6167 6963 206d 6574 686f 6473  ng magic methods
+00000570: 293a 0a20 2020 2020 2020 2023 2074 7970  ):.        # typ
+00000580: 696e 672e 6765 745f 7479 7065 5f68 696e  ing.get_type_hin
+00000590: 7473 2863 6c73 2c20 676c 6f62 616c 6e73  ts(cls, globalns
+000005a0: 3d4e 6f6e 652c 206c 6f63 616c 6e73 3d4e  =None, localns=N
+000005b0: 6f6e 6529 0a0a 2020 2020 2020 2020 2320  one)..        # 
+000005c0: 6469 7274 7920 7761 7920 2877 6974 6820  dirty way (with 
+000005d0: 6576 696c 2065 7661 6c29 3a0a 2020 2020  evil eval):.    
+000005e0: 2020 2020 2320 5b65 7661 6c28 7629 2066      # [eval(v) f
+000005f0: 6f72 206b 2c20 7620 696e 2063 6c73 2e5f  or k, v in cls._
+00000600: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 2e69  _annotations__.i
+00000610: 7465 6d73 2829 5d0a 2020 2020 2020 2020  tems()].        
+00000620: 2320 7468 6973 2068 6f77 6576 6572 2061  # this however a
+00000630: 6c73 6f20 7374 6f70 7320 776f 726b 696e  lso stops workin
+00000640: 6720 7768 656e 2076 6172 6961 626c 6573  g when variables
+00000650: 206f 7574 7369 6465 2074 6869 7320 7363   outside this sc
+00000660: 6f70 6520 6f72 2065 7665 6e20 7265 6665  ope or even refe
+00000670: 7265 6e63 6573 2074 6f20 6f74 6865 720a  rences to other.
+00000680: 2020 2020 2020 2020 2320 6f62 6a65 6374          # object
+00000690: 7320 6172 6520 7573 6564 2e20 536f 2066  s are used. So f
+000006a0: 6f72 206e 6f77 2c20 7468 6973 2070 6163  or now, this pac
+000006b0: 6b61 6765 2077 696c 6c20 4e4f 5420 776f  kage will NOT wo
+000006c0: 726b 2077 6865 6e20 6672 6f6d 205f 5f66  rk when from __f
+000006d0: 7574 7572 655f 5f20 696d 706f 7274 2061  uture__ import a
+000006e0: 6e6e 6f74 6174 696f 6e73 2069 7320 7573  nnotations is us
+000006f0: 6564 2c0a 2020 2020 2020 2020 2320 616e  ed,.        # an
+00000700: 6420 6d69 6768 7420 6272 6561 6b20 696e  d might break in
+00000710: 2074 6865 2066 7574 7572 652c 2077 6865   the future, whe
+00000720: 6e20 7468 6973 2061 6e6e 6f74 6174 696f  n this annotatio
+00000730: 6e73 2062 6568 6176 696f 7220 6973 2065  ns behavior is e
+00000740: 6e61 626c 6564 2062 7920 6465 6661 756c  nabled by defaul
+00000750: 742e 0a20 2020 2020 2020 2023 2074 6f64  t..        # tod
+00000760: 6f3a 2061 6464 2074 6f20 6361 7665 6174  o: add to caveat
+00000770: 730a 0a20 2020 2020 2020 2023 206e 6f6e  s..        # non
+00000780: 2d61 6e6e 6f74 6174 6564 2076 6172 6961  -annotated varia
+00000790: 626c 6573 2068 6176 6520 746f 2062 6520  bles have to be 
+000007a0: 7061 7373 6564 2074 6f20 6465 6669 6e65  passed to define
+000007b0: 5f74 6162 6c65 2061 7320 6b77 6172 6773  _table as kwargs
+000007c0: 0a0a 2020 2020 2020 2020 7461 626c 656e  ..        tablen
+000007d0: 616d 6520 3d20 7365 6c66 2e5f 746f 5f73  ame = self._to_s
+000007e0: 6e61 6b65 2863 6c73 2e5f 5f6e 616d 655f  nake(cls.__name_
+000007f0: 5f29 0a20 2020 2020 2020 2066 6965 6c64  _).        field
+00000800: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+00000810: 2020 7365 6c66 2e5f 746f 5f66 6965 6c64    self._to_field
+00000820: 2866 6e61 6d65 2c20 6674 7970 6529 2066  (fname, ftype) f
+00000830: 6f72 2066 6e61 6d65 2c20 6674 7970 6520  or fname, ftype 
+00000840: 696e 2063 6c73 2e5f 5f61 6e6e 6f74 6174  in cls.__annotat
+00000850: 696f 6e73 5f5f 2e69 7465 6d73 2829 0a20  ions__.items(). 
+00000860: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00000870: 206f 7468 6572 5f6b 7761 7267 7320 3d20   other_kwargs = 
+00000880: 7b0a 2020 2020 2020 2020 2020 2020 6b3a  {.            k:
+00000890: 2076 0a20 2020 2020 2020 2020 2020 2066   v.            f
+000008a0: 6f72 206b 2c20 7620 696e 2063 6c73 2e5f  or k, v in cls._
+000008b0: 5f64 6963 745f 5f2e 6974 656d 7328 290a  _dict__.items().
+000008c0: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+000008d0: 206e 6f74 2069 6e20 636c 732e 5f5f 616e   not in cls.__an
+000008e0: 6e6f 7461 7469 6f6e 735f 5f20 616e 6420  notations__ and 
+000008f0: 6e6f 7420 6b2e 7374 6172 7473 7769 7468  not k.startswith
+00000900: 2822 5f22 290a 2020 2020 2020 2020 7d0a  ("_").        }.
+00000910: 0a20 2020 2020 2020 2074 6162 6c65 203d  .        table =
+00000920: 2073 656c 662e 6465 6669 6e65 5f74 6162   self.define_tab
+00000930: 6c65 2874 6162 6c65 6e61 6d65 2c20 2a66  le(tablename, *f
+00000940: 6965 6c64 732c 202a 2a6f 7468 6572 5f6b  ields, **other_k
+00000950: 7761 7267 7329 0a0a 2020 2020 2020 2020  wargs)..        
+00000960: 636c 732e 5f5f 7365 745f 696e 7465 726e  cls.__set_intern
+00000970: 616c 735f 5f28 6462 3d73 656c 662c 2074  als__(db=self, t
+00000980: 6162 6c65 3d74 6162 6c65 290a 0a20 2020  able=table)..   
+00000990: 2020 2020 2023 2074 6865 2041 4354 5541       # the ACTUA
+000009a0: 4c20 6f75 7470 7574 2069 7320 6e6f 7420  L output is not 
+000009b0: 5479 7065 6454 6162 6c65 2062 7574 2072  TypedTable but r
+000009c0: 6174 6865 7220 7079 6461 6c2e 5461 626c  ather pydal.Tabl
+000009d0: 650a 2020 2020 2020 2020 2320 6275 7420  e.        # but 
+000009e0: 7465 6c6c 696e 6720 7468 6520 6564 6974  telling the edit
+000009f0: 6f72 2069 7420 6973 2054 2068 656c 7073  or it is T helps
+00000a00: 2077 6974 6820 6869 6e74 696e 672e 0a20   with hinting.. 
+00000a10: 2020 2020 2020 2072 6574 7572 6e20 7461         return ta
+00000a20: 626c 650a 0a20 2020 2064 6566 205f 5f63  ble..    def __c
+00000a30: 616c 6c5f 5f28 7365 6c66 2c20 2a61 7267  all__(self, *arg
+00000a40: 732c 202a 2a6b 7761 7267 7329 202d 3e20  s, **kwargs) -> 
+00000a50: 7079 6461 6c2e 6f62 6a65 6374 732e 5365  pydal.objects.Se
+00000a60: 743a 0a20 2020 2020 2020 2061 7267 7320  t:.        args 
+00000a70: 3d20 6c69 7374 2861 7267 7329 0a20 2020  = list(args).   
+00000a80: 2020 2020 2069 6620 6172 6773 3a0a 2020       if args:.  
+00000a90: 2020 2020 2020 2020 2020 636c 7320 3d20            cls = 
+00000aa0: 6172 6773 5b30 5d0a 2020 2020 2020 2020  args[0].        
+00000ab0: 2020 2020 6966 2069 7373 7562 636c 6173      if issubclas
+00000ac0: 7328 7479 7065 2863 6c73 292c 2074 7970  s(type(cls), typ
+00000ad0: 6529 2061 6e64 2069 7373 7562 636c 6173  e) and issubclas
+00000ae0: 7328 636c 732c 2054 7970 6564 5461 626c  s(cls, TypedTabl
+00000af0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00000b00: 2020 2020 2320 7461 626c 6520 6465 6669      # table defi
+00000b10: 6e65 6420 7769 7468 6f75 7420 4064 622e  ned without @db.
+00000b20: 6465 6669 6e65 2064 6563 6f72 6174 6f72  define decorator
+00000b30: 210a 2020 2020 2020 2020 2020 2020 2020  !.              
+00000b40: 2020 6172 6773 5b30 5d20 3d20 636c 732e    args[0] = cls.
+00000b50: 6964 2021 3d20 4e6f 6e65 0a0a 2020 2020  id != None..    
+00000b60: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00000b70: 2829 2e5f 5f63 616c 6c5f 5f28 2a61 7267  ().__call__(*arg
+00000b80: 732c 202a 2a6b 7761 7267 7329 0a0a 2020  s, **kwargs)..  
+00000b90: 2020 2320 746f 646f 3a20 696e 7365 7274    # todo: insert
+00000ba0: 2065 7463 2073 6861 646f 7765 6e3f 0a0a   etc shadowen?..
+00000bb0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00000bc0: 0a20 2020 2064 6566 205f 6275 696c 645f  .    def _build_
+00000bd0: 6669 656c 6428 636c 732c 206e 616d 652c  field(cls, name,
+00000be0: 2074 7970 652c 202a 2a6b 7729 3a0a 2020   type, **kw):.  
+00000bf0: 2020 2020 2020 7265 7475 726e 2046 6965        return Fie
+00000c00: 6c64 286e 616d 652c 2074 7970 652c 202a  ld(name, type, *
+00000c10: 2a7b 2a2a 636c 732e 6465 6661 756c 745f  *{**cls.default_
+00000c20: 6b77 6172 6773 2c20 2a2a 6b77 7d29 0a0a  kwargs, **kw})..
+00000c30: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00000c40: 0a20 2020 2064 6566 205f 746f 5f66 6965  .    def _to_fie
+00000c50: 6c64 2863 6c73 2c20 666e 616d 653a 2073  ld(cls, fname: s
+00000c60: 7472 2c20 6674 7970 653a 2074 7970 652c  tr, ftype: type,
+00000c70: 202a 2a6b 7729 3a0a 2020 2020 2020 2020   **kw):.        
+00000c80: 666e 616d 6520 3d20 636c 732e 5f74 6f5f  fname = cls._to_
+00000c90: 736e 616b 6528 666e 616d 6529 0a0a 2020  snake(fname)..  
+00000ca0: 2020 2020 2020 6966 206d 6170 7069 6e67        if mapping
+00000cb0: 203a 3d20 4241 5349 435f 4d41 5050 494e   := BASIC_MAPPIN
+00000cc0: 4753 2e67 6574 2866 7479 7065 293a 0a20  GS.get(ftype):. 
+00000cd0: 2020 2020 2020 2020 2020 2023 2062 6173             # bas
+00000ce0: 6920 7479 7065 730a 2020 2020 2020 2020  i types.        
+00000cf0: 2020 2020 7265 7475 726e 2063 6c73 2e5f      return cls._
+00000d00: 6275 696c 645f 6669 656c 6428 666e 616d  build_field(fnam
+00000d10: 652c 206d 6170 7069 6e67 2c20 2a2a 6b77  e, mapping, **kw
+00000d20: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
+00000d30: 7369 6e73 7461 6e63 6528 6674 7970 652c  sinstance(ftype,
+00000d40: 2054 6162 6c65 293a 0a20 2020 2020 2020   Table):.       
+00000d50: 2020 2020 2023 2064 622e 7461 626c 650a       # db.table.
+00000d60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000d70: 726e 2063 6c73 2e5f 6275 696c 645f 6669  rn cls._build_fi
+00000d80: 656c 6428 666e 616d 652c 2066 2272 6566  eld(fname, f"ref
+00000d90: 6572 656e 6365 207b 6674 7970 652e 5f74  erence {ftype._t
+00000da0: 6162 6c65 6e61 6d65 7d22 2c20 2a2a 6b77  ablename}", **kw
+00000db0: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
+00000dc0: 7373 7562 636c 6173 7328 7479 7065 2866  ssubclass(type(f
+00000dd0: 7479 7065 292c 2074 7970 6529 2061 6e64  type), type) and
+00000de0: 2069 7373 7562 636c 6173 7328 6674 7970   issubclass(ftyp
+00000df0: 652c 2054 7970 6564 5461 626c 6529 3a0a  e, TypedTable):.
+00000e00: 2020 2020 2020 2020 2020 2020 2320 536f              # So
+00000e10: 6d65 5461 626c 650a 2020 2020 2020 2020  meTable.        
+00000e20: 2020 2020 736e 616b 656e 616d 6520 3d20      snakename = 
+00000e30: 636c 732e 5f74 6f5f 736e 616b 6528 6674  cls._to_snake(ft
+00000e40: 7970 652e 5f5f 6e61 6d65 5f5f 290a 2020  ype.__name__).  
+00000e50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000e60: 2063 6c73 2e5f 6275 696c 645f 6669 656c   cls._build_fiel
+00000e70: 6428 666e 616d 652c 2066 2272 6566 6572  d(fname, f"refer
+00000e80: 656e 6365 207b 736e 616b 656e 616d 657d  ence {snakename}
+00000e90: 222c 202a 2a6b 7729 0a20 2020 2020 2020  ", **kw).       
+00000ea0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00000eb0: 2866 7479 7065 2c20 5479 7065 6446 6965  (ftype, TypedFie
+00000ec0: 6c64 5479 7065 293a 0a20 2020 2020 2020  ldType):.       
+00000ed0: 2020 2020 2023 2046 6965 6c64 5479 7065       # FieldType
+00000ee0: 2874 7970 652c 202e 2e2e 290a 2020 2020  (type, ...).    
+00000ef0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00000f00: 7479 7065 2e5f 746f 5f66 6965 6c64 2866  type._to_field(f
+00000f10: 6e61 6d65 2c20 2a2a 6b77 290a 2020 2020  name, **kw).    
+00000f20: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+00000f30: 6e63 6528 6674 7970 652c 2074 7970 6573  nce(ftype, types
+00000f40: 2e47 656e 6572 6963 416c 6961 7329 3a0a  .GenericAlias):.
+00000f50: 2020 2020 2020 2020 2020 2020 2320 6c69              # li
+00000f60: 7374 5b2e 2e2e 5d0a 2020 2020 2020 2020  st[...].        
+00000f70: 2020 2020 5f63 6869 6c64 7479 7065 203d      _childtype =
+00000f80: 2054 7970 6564 4669 656c 6454 7970 652e   TypedFieldType.
+00000f90: 5f63 6f6e 7665 7274 5f67 656e 6572 6963  _convert_generic
+00000fa0: 5f61 6c69 6173 5f6c 6973 7428 6674 7970  _alias_list(ftyp
+00000fb0: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
+00000fc0: 6574 7572 6e20 636c 732e 5f62 7569 6c64  eturn cls._build
+00000fd0: 5f66 6965 6c64 2866 6e61 6d65 2c20 6622  _field(fname, f"
+00000fe0: 6c69 7374 3a7b 5f63 6869 6c64 7479 7065  list:{_childtype
+00000ff0: 7d22 2c20 2a2a 6b77 290a 2020 2020 2020  }", **kw).      
+00001000: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00001010: 6528 6674 7970 652c 2074 7970 696e 672e  e(ftype, typing.
+00001020: 5f55 6e69 6f6e 4765 6e65 7269 6341 6c69  _UnionGenericAli
+00001030: 6173 2920 6f72 2069 7369 6e73 7461 6e63  as) or isinstanc
+00001040: 6528 0a20 2020 2020 2020 2020 2020 2066  e(.            f
+00001050: 7479 7065 2c20 7479 7065 732e 556e 696f  type, types.Unio
+00001060: 6e54 7970 650a 2020 2020 2020 2020 293a  nType.        ):
+00001070: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
+00001080: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00001090: 7970 655d 203d 3d20 7479 7065 207c 204e  ype] == type | N
+000010a0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000010b0: 6d61 7463 6820 6674 7970 652e 5f5f 6172  match ftype.__ar
+000010c0: 6773 5f5f 3a0a 2020 2020 2020 2020 2020  gs__:.          
+000010d0: 2020 2020 2020 6361 7365 2028 5f63 6869        case (_chi
+000010e0: 6c64 5f74 7970 652c 205f 5479 7065 732e  ld_type, _Types.
+000010f0: 4e4f 4e45 5459 5045 293a 0a20 2020 2020  NONETYPE):.     
+00001100: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00001110: 2067 6f6f 6420 756e 696f 6e0a 0a20 2020   good union..   
+00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001130: 2023 2069 6620 6120 6669 656c 6420 6973   # if a field is
+00001140: 206f 7074 696f 6e61 6c2c 2069 7420 6973   optional, it is
+00001150: 206e 756c 6c61 626c 653a 0a20 2020 2020   nullable:.     
+00001160: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00001170: 775b 226e 6f74 6e75 6c6c 225d 203d 2046  w["notnull"] = F
+00001180: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00001190: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000011a0: 636c 732e 5f74 6f5f 6669 656c 6428 666e  cls._to_field(fn
+000011b0: 616d 652c 205f 6368 696c 645f 7479 7065  ame, _child_type
+000011c0: 2c20 2a2a 6b77 290a 2020 2020 2020 2020  , **kw).        
+000011d0: 2020 2020 2020 2020 6361 7365 206f 7468          case oth
+000011e0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+000011f0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
+00001200: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+00001210: 7228 6622 496e 7661 6c69 6420 7479 7065  r(f"Invalid type
+00001220: 2075 6e69 6f6e 2027 7b6f 7468 6572 7d27   union '{other}'
+00001230: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
+00001240: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
+00001250: 6f64 6f3a 2063 6174 6368 206f 7468 6572  odo: catch other
+00001260: 2074 7970 6573 0a20 2020 2020 2020 2020   types.         
+00001270: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+00001280: 656d 656e 7465 6445 7272 6f72 2866 2255  ementedError(f"U
+00001290: 6e73 7570 706f 7274 6564 2074 7970 6520  nsupported type 
+000012a0: 7b66 7479 7065 7d2f 7b74 7970 6528 6674  {ftype}/{type(ft
+000012b0: 7970 6529 7d22 290a 0a20 2020 2040 7374  ype)}")..    @st
+000012c0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+000012d0: 6566 205f 746f 5f73 6e61 6b65 2863 616d  ef _to_snake(cam
+000012e0: 656c 3a20 7374 7229 202d 3e20 7374 723a  el: str) -> str:
+000012f0: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
+00001300: 3a2f 2f73 7461 636b 6f76 6572 666c 6f77  ://stackoverflow
+00001310: 2e63 6f6d 2f61 2f34 3439 3639 3338 310a  .com/a/44969381.
+00001320: 2020 2020 2020 2020 7265 7475 726e 2022          return "
+00001330: 222e 6a6f 696e 285b 225f 2220 2b20 632e  ".join(["_" + c.
+00001340: 6c6f 7765 7228 2920 6966 2063 2e69 7375  lower() if c.isu
+00001350: 7070 6572 2829 2065 6c73 6520 6320 666f  pper() else c fo
+00001360: 7220 6320 696e 2063 616d 656c 5d29 2e6c  r c in camel]).l
+00001370: 7374 7269 7028 0a20 2020 2020 2020 2020  strip(.         
+00001380: 2020 2022 5f22 0a20 2020 2020 2020 2029     "_".        )
+00001390: 0a0a 0a63 6c61 7373 2054 7970 6564 5461  ...class TypedTa
+000013a0: 626c 654d 6574 6128 7479 7065 293a 0a20  bleMeta(type):. 
+000013b0: 2020 2023 206d 6574 6120 636c 6173 7320     # meta class 
+000013c0: 616c 6c6f 7773 2067 6574 6174 7472 6962  allows getattrib
+000013d0: 7574 6520 6f6e 2063 6c61 7373 2076 6172  ute on class var
+000013e0: 6961 626c 6573 2069 6e73 7465 6164 2069  iables instead i
+000013f0: 6e73 7461 6e63 6520 7661 7269 6162 6c65  nstance variable
+00001400: 730a 2020 2020 6465 6620 5f5f 6765 7461  s.    def __geta
+00001410: 7474 725f 5f28 7365 6c66 2c20 6b65 7929  ttr__(self, key)
+00001420: 3a0a 2020 2020 2020 2020 2320 6765 7461  :.        # geta
+00001430: 7474 7220 6973 206f 6e6c 7920 6361 6c6c  ttr is only call
+00001440: 6564 2077 6865 6e20 6765 7461 7474 7269  ed when getattri
+00001450: 6275 7465 2063 616e 2774 2066 696e 6420  bute can't find 
+00001460: 736f 6d65 7468 696e 670a 2020 2020 2020  something.      
+00001470: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+00001480: 6765 745f 7461 626c 655f 636f 6c75 6d6e  get_table_column
+00001490: 5f5f 286b 6579 290a 0a0a 636c 6173 7320  __(key)...class 
+000014a0: 5479 7065 6454 6162 6c65 2854 6162 6c65  TypedTable(Table
+000014b0: 2c20 6d65 7461 636c 6173 733d 5479 7065  , metaclass=Type
+000014c0: 6454 6162 6c65 4d65 7461 293a 0a20 2020  dTableMeta):.   
+000014d0: 2069 643a 2069 6e74 0a0a 2020 2020 2320   id: int..    # 
+000014e0: 7365 7420 7570 2062 7920 6462 2e64 6566  set up by db.def
+000014f0: 696e 653a 0a20 2020 205f 5f64 623a 2054  ine:.    __db: T
+00001500: 7970 6544 414c 203d 204e 6f6e 650a 2020  ypeDAL = None.  
+00001510: 2020 5f5f 7461 626c 653a 2054 6162 6c65    __table: Table
+00001520: 203d 204e 6f6e 650a 0a20 2020 2040 636c   = None..    @cl
+00001530: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00001540: 6620 5f5f 7365 745f 696e 7465 726e 616c  f __set_internal
+00001550: 735f 5f28 636c 732c 2064 622c 2074 6162  s__(cls, db, tab
+00001560: 6c65 293a 0a20 2020 2020 2020 2063 6c73  le):.        cls
+00001570: 2e5f 5f64 6220 3d20 6462 0a20 2020 2020  .__db = db.     
+00001580: 2020 2063 6c73 2e5f 5f74 6162 6c65 203d     cls.__table =
+00001590: 2074 6162 6c65 0a0a 2020 2020 4063 6c61   table..    @cla
+000015a0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+000015b0: 205f 5f67 6574 5f74 6162 6c65 5f63 6f6c   __get_table_col
+000015c0: 756d 6e5f 5f28 636c 732c 2063 6f6c 293a  umn__(cls, col):
+000015d0: 0a20 2020 2020 2020 2023 2064 622e 7461  .        # db.ta
+000015e0: 626c 652e 636f 6c20 2d3e 2053 6f6d 6554  ble.col -> SomeT
+000015f0: 7970 6564 5461 626c 652e 636f 6c20 2876  ypedTable.col (v
+00001600: 6961 2054 7970 6564 5461 626c 654d 6574  ia TypedTableMet
+00001610: 612e 5f5f 6765 7461 7474 725f 5f29 0a20  a.__getattr__). 
+00001620: 2020 2020 2020 2069 6620 636c 732e 5f5f         if cls.__
+00001630: 7461 626c 653a 0a20 2020 2020 2020 2020  table:.         
+00001640: 2020 2072 6574 7572 6e20 636c 732e 5f5f     return cls.__
+00001650: 7461 626c 655b 636f 6c5d 0a0a 2020 2020  table[col]..    
+00001660: 6465 6620 5f5f 6e65 775f 5f28 636c 732c  def __new__(cls,
+00001670: 202a 612c 202a 2a6b 7729 3a0a 2020 2020   *a, **kw):.    
+00001680: 2020 2020 2320 7768 656e 2065 2e67 2e20      # when e.g. 
+00001690: 5461 626c 6528 6964 3d30 2920 6973 2063  Table(id=0) is c
+000016a0: 616c 6c65 6420 7769 7468 6f75 7420 6462  alled without db
+000016b0: 2e64 6566 696e 652c 0a20 2020 2020 2020  .define,.       
+000016c0: 2023 2074 6869 7320 6361 7463 6865 7320   # this catches 
+000016d0: 6974 2061 6e64 2066 6f72 7761 7264 7320  it and forwards 
+000016e0: 666f 7220 7072 6f70 6572 2062 6568 6176  for proper behav
+000016f0: 696f 720a 2020 2020 2020 2020 7265 7475  ior.        retu
+00001700: 726e 2063 6c73 2e5f 5f74 6162 6c65 282a  rn cls.__table(*
+00001710: 612c 202a 2a6b 7729 0a0a 2020 2020 4063  a, **kw)..    @c
+00001720: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00001730: 6566 2069 6e73 6572 7428 636c 732c 202a  ef insert(cls, *
+00001740: 2a66 6965 6c64 7329 3a0a 2020 2020 2020  *fields):.      
+00001750: 2020 2320 7468 6973 2069 7320 6f6e 6c79    # this is only
+00001760: 2063 616c 6c65 6420 7768 656e 2064 622e   called when db.
+00001770: 6465 6669 6e65 2069 7320 6e6f 7420 7573  define is not us
+00001780: 6564 2061 7320 6120 6465 636f 7261 746f  ed as a decorato
+00001790: 720a 2020 2020 2020 2020 2320 636c 732e  r.        # cls.
+000017a0: 5f5f 7461 626c 6520 6675 6e63 7469 6f6e  __table function
+000017b0: 7320 6173 2027 7365 6c66 270a 2020 2020  s as 'self'.    
+000017c0: 2020 2020 7375 7065 7228 292e 696e 7365      super().inse
+000017d0: 7274 2863 6c73 2e5f 5f74 6162 6c65 2c20  rt(cls.__table, 
+000017e0: 2a2a 6669 656c 6473 290a 0a0a 2320 6261  **fields)...# ba
+000017f0: 636b 7761 7264 7320 636f 6d70 6174 3a0a  ckwards compat:.
+00001800: 5479 7065 6452 6f77 203d 2054 7970 6564  TypedRow = Typed
+00001810: 5461 626c 650a 0a0a 636c 6173 7320 5479  Table...class Ty
+00001820: 7065 6446 6965 6c64 5479 7065 2846 6965  pedFieldType(Fie
+00001830: 6c64 293a 0a20 2020 205f 7461 626c 6520  ld):.    _table 
+00001840: 3d20 223c 616e 7920 7461 626c 653e 220a  = "<any table>".
+00001850: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00001860: 5f28 7365 6c66 2c20 5f74 7970 652c 202a  _(self, _type, *
+00001870: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+00001880: 2020 7365 6c66 2e74 7970 6520 3d20 5f74    self.type = _t
+00001890: 7970 650a 2020 2020 2020 2020 7365 6c66  ype.        self
+000018a0: 2e6b 7761 7267 7320 3d20 6b77 6172 6773  .kwargs = kwargs
+000018b0: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
+000018c0: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+000018d0: 2020 7320 3d20 7365 6c66 2e5f 5f73 7472    s = self.__str
+000018e0: 5f5f 2829 0a20 2020 2020 2020 2072 6574  __().        ret
+000018f0: 7572 6e20 6622 3c7b 737d 2077 6974 6820  urn f"<{s} with 
+00001900: 6f70 7469 6f6e 7320 7b73 656c 662e 6b77  options {self.kw
+00001910: 6172 6773 7d3e 220a 0a20 2020 2064 6566  args}>"..    def
+00001920: 205f 5f73 7472 5f5f 2873 656c 6629 3a0a   __str__(self):.
+00001930: 2020 2020 2020 2020 6966 2022 7479 7065          if "type
+00001940: 2220 696e 2073 656c 662e 6b77 6172 6773  " in self.kwargs
+00001950: 3a0a 2020 2020 2020 2020 2020 2020 7420  :.            t 
+00001960: 3d20 7365 6c66 2e6b 7761 7267 735b 2274  = self.kwargs["t
+00001970: 7970 6522 5d0a 2020 2020 2020 2020 656c  ype"].        el
+00001980: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00001990: 7420 3d20 7365 6c66 2e74 7970 652e 5f5f  t = self.type.__
+000019a0: 6e61 6d65 5f5f 2069 6620 6973 7375 6263  name__ if issubc
+000019b0: 6c61 7373 2874 7970 6528 7365 6c66 2e74  lass(type(self.t
+000019c0: 7970 6529 2c20 7479 7065 2920 656c 7365  ype), type) else
+000019d0: 2073 656c 662e 7479 7065 0a20 2020 2020   self.type.     
+000019e0: 2020 2072 6574 7572 6e20 6622 5479 7065     return f"Type
+000019f0: 6446 6965 6c64 2e7b 747d 220a 0a20 2020  dField.{t}"..   
+00001a00: 2064 6566 205f 746f 5f66 6965 6c64 2873   def _to_field(s
+00001a10: 656c 662c 206e 616d 653a 2073 7472 2c20  elf, name: str, 
+00001a20: 2a2a 6578 7472 615f 6b77 6172 6773 2920  **extra_kwargs) 
+00001a30: 2d3e 2046 6965 6c64 3a0a 2020 2020 2020  -> Field:.      
+00001a40: 2020 6f74 6865 725f 6b77 6172 6773 203d    other_kwargs =
+00001a50: 2073 656c 662e 6b77 6172 6773 2e63 6f70   self.kwargs.cop
+00001a60: 7928 290a 2020 2020 2020 2020 6f74 6865  y().        othe
+00001a70: 725f 6b77 6172 6773 2e75 7064 6174 6528  r_kwargs.update(
+00001a80: 6578 7472 615f 6b77 6172 6773 290a 2020  extra_kwargs).  
+00001a90: 2020 2020 2020 6966 2022 7479 7065 2220        if "type" 
+00001aa0: 696e 206f 7468 6572 5f6b 7761 7267 733a  in other_kwargs:
+00001ab0: 0a20 2020 2020 2020 2020 2020 205f 7479  .            _ty
+00001ac0: 7065 203d 206f 7468 6572 5f6b 7761 7267  pe = other_kwarg
+00001ad0: 732e 706f 7028 2274 7970 6522 290a 2020  s.pop("type").  
+00001ae0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00001af0: 2020 2020 2020 2020 5f74 7970 6520 3d20          _type = 
+00001b00: 7365 6c66 2e5f 746f 5f66 6965 6c64 5f74  self._to_field_t
+00001b10: 7970 6528 7365 6c66 2e74 7970 6529 0a0a  ype(self.type)..
+00001b20: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00001b30: 7970 6544 414c 2e5f 6275 696c 645f 6669  ypeDAL._build_fi
+00001b40: 656c 6428 6e61 6d65 2c20 5f74 7970 652c  eld(name, _type,
+00001b50: 202a 2a6f 7468 6572 5f6b 7761 7267 7329   **other_kwargs)
+00001b60: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00001b70: 6f64 0a20 2020 2064 6566 205f 746f 5f66  od.    def _to_f
+00001b80: 6965 6c64 5f74 7970 6528 636c 732c 205f  ield_type(cls, _
+00001b90: 7479 7065 3a20 7479 7065 2920 2d3e 2073  type: type) -> s
+00001ba0: 7472 3a0a 2020 2020 2020 2020 2320 746f  tr:.        # to
+00001bb0: 646f 3a20 6d65 7267 6520 7769 7468 2054  do: merge with T
+00001bc0: 7970 6544 414c 2e5f 746f 5f66 6965 6c64  ypeDAL._to_field
+00001bd0: 2028 6b69 6e64 613f 290a 2020 2020 2020   (kinda?).      
+00001be0: 2020 6966 206d 6170 7069 6e67 203a 3d20    if mapping := 
+00001bf0: 4241 5349 435f 4d41 5050 494e 4753 2e67  BASIC_MAPPINGS.g
+00001c00: 6574 285f 7479 7065 293a 0a20 2020 2020  et(_type):.     
+00001c10: 2020 2020 2020 2023 2062 6173 6963 2074         # basic t
+00001c20: 7970 6573 0a20 2020 2020 2020 2020 2020  ypes.           
+00001c30: 2072 6574 7572 6e20 6d61 7070 696e 670a   return mapping.
+00001c40: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
+00001c50: 7562 636c 6173 7328 7479 7065 285f 7479  ubclass(type(_ty
+00001c60: 7065 292c 2074 7970 6529 2061 6e64 2069  pe), type) and i
+00001c70: 7373 7562 636c 6173 7328 5f74 7970 652c  ssubclass(_type,
+00001c80: 2054 7970 6564 5461 626c 6529 3a0a 2020   TypedTable):.  
+00001c90: 2020 2020 2020 2020 2020 2320 536f 6d65            # Some
+00001ca0: 5461 626c 650a 2020 2020 2020 2020 2020  Table.          
+00001cb0: 2020 736e 616b 656e 616d 6520 3d20 5479    snakename = Ty
+00001cc0: 7065 4441 4c2e 5f74 6f5f 736e 616b 6528  peDAL._to_snake(
+00001cd0: 5f74 7970 652e 5f5f 6e61 6d65 5f5f 290a  _type.__name__).
+00001ce0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001cf0: 726e 2066 2272 6566 6572 656e 6365 207b  rn f"reference {
+00001d00: 736e 616b 656e 616d 657d 220a 2020 2020  snakename}".    
+00001d10: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+00001d20: 6e63 6528 5f74 7970 652c 2054 6162 6c65  nce(_type, Table
+00001d30: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
+00001d40: 2064 622e 736f 6d65 7461 626c 650a 2020   db.sometable.  
+00001d50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001d60: 2066 2272 6566 6572 656e 6365 207b 5f74   f"reference {_t
+00001d70: 7970 652e 5f74 6162 6c65 6e61 6d65 7d22  ype._tablename}"
+00001d80: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+00001d90: 696e 7374 616e 6365 285f 7479 7065 2c20  instance(_type, 
+00001da0: 7479 7065 732e 4765 6e65 7269 6341 6c69  types.GenericAli
+00001db0: 6173 293a 0a20 2020 2020 2020 2020 2020  as):.           
+00001dc0: 2023 206c 6973 745b 7479 7065 5d0a 2020   # list[type].  
+00001dd0: 2020 2020 2020 2020 2020 5f63 6869 6c64            _child
+00001de0: 5f74 7970 6520 3d20 636c 732e 5f63 6f6e  _type = cls._con
+00001df0: 7665 7274 5f67 656e 6572 6963 5f61 6c69  vert_generic_ali
+00001e00: 6173 5f6c 6973 7428 5f74 7970 6529 0a20  as_list(_type). 
+00001e10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001e20: 6e20 6622 6c69 7374 3a7b 5f63 6869 6c64  n f"list:{_child
+00001e30: 5f74 7970 657d 220a 2020 2020 2020 2020  _type}".        
+00001e40: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00001e50: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+00001e60: 6d65 6e74 6564 4572 726f 7228 5f74 7970  mentedError(_typ
+00001e70: 6529 0a0a 2020 2020 4063 6c61 7373 6d65  e)..    @classme
+00001e80: 7468 6f64 0a20 2020 2064 6566 205f 636f  thod.    def _co
+00001e90: 6e76 6572 745f 6765 6e65 7269 635f 616c  nvert_generic_al
+00001ea0: 6961 735f 6c69 7374 2863 6c73 2c20 6674  ias_list(cls, ft
+00001eb0: 7970 6529 3a0a 2020 2020 2020 2020 2320  ype):.        # 
+00001ec0: 652e 672e 206c 6973 745b 7374 720a 2020  e.g. list[str.  
+00001ed0: 2020 2020 2020 6261 7365 7479 7065 203d        basetype =
+00001ee0: 2066 7479 7065 2e5f 5f6f 7269 6769 6e5f   ftype.__origin_
+00001ef0: 5f0a 2020 2020 2020 2020 2320 652e 672e  _.        # e.g.
+00001f00: 206c 6973 740a 2020 2020 2020 2020 6966   list.        if
+00001f10: 2062 6173 6574 7970 6520 6973 206e 6f74   basetype is not
+00001f20: 206c 6973 743a 0a20 2020 2020 2020 2020   list:.         
+00001f30: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+00001f40: 656d 656e 7465 6445 7272 6f72 2822 4f6e  ementedError("On
+00001f50: 6c79 2070 6172 616d 6574 6572 697a 6564  ly parameterized
+00001f60: 206c 6973 7420 6973 2063 7572 7265 6e74   list is current
+00001f70: 6c79 2061 7661 696c 6162 6c65 2e22 290a  ly available.").
+00001f80: 2020 2020 2020 2020 6368 696c 6474 7970          childtyp
+00001f90: 6520 3d20 6674 7970 652e 5f5f 6172 6773  e = ftype.__args
+00001fa0: 5f5f 5b30 5d0a 0a20 2020 2020 2020 2072  __[0]..        r
+00001fb0: 6574 7572 6e20 636c 732e 5f74 6f5f 6669  eturn cls._to_fi
+00001fc0: 656c 645f 7479 7065 2863 6869 6c64 7479  eld_type(childty
+00001fd0: 7065 290a 0a0a 5320 3d20 7479 7069 6e67  pe)...S = typing
+00001fe0: 2e54 7970 6556 6172 2822 5322 290a 0a0a  .TypeVar("S")...
+00001ff0: 636c 6173 7320 5479 7065 6452 6f77 7328  class TypedRows(
+00002000: 7479 7069 6e67 2e43 6f6c 6c65 6374 696f  typing.Collectio
+00002010: 6e5b 535d 2c20 526f 7773 293a 0a20 2020  n[S], Rows):.   
+00002020: 2022 2222 0a20 2020 2043 616e 2062 6520   """.    Can be 
+00002030: 7573 6564 2061 7320 7468 6520 7265 7475  used as the retu
+00002040: 726e 2074 7970 6520 6f66 2061 202e 7365  rn type of a .se
+00002050: 6c65 6374 2829 0a20 2020 2065 2e67 2e0a  lect().    e.g..
+00002060: 0a20 2020 2070 656f 706c 653a 2054 7970  .    people: Typ
+00002070: 6564 526f 7773 5b50 6572 736f 6e5d 203d  edRows[Person] =
+00002080: 2064 6228 5065 7273 6f6e 292e 7365 6c65   db(Person).sele
+00002090: 6374 2829 0a20 2020 2022 2222 0a         ct().    """.
```

