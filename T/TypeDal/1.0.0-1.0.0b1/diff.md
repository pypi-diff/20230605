# Comparing `tmp/typedal-1.0.0.tar.gz` & `tmp/typedal-1.0.0b1.tar.gz`

## Comparing `typedal-1.0.0.tar` & `typedal-1.0.0b1.tar`

### file list

```diff
@@ -1,340 +1,340 @@
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 typedal-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 typedal-1.0.0/coverage.svg
--rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 typedal-1.0.0/example_new.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 typedal-1.0.0/example_old.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 typedal-1.0.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0   177667 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   170960 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1054992 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   123328 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   104160 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    57612 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   142044 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    85348 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0    88278 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    75208 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   167175 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    49442 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   168498 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   146267 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   228230 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   416965 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407999 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   128994 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    79298 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70175 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    90277 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350178 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/__init__.data.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/__init__.meta.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/typedal/__about__.data.json
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/typedal/__init__.data.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/typedal/__init__.meta.json
--rw-r--r--   0        0        0    33347 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/typedal/core.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/typedal/core.meta.json
--rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/typedal/fields.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/typedal/fields.meta.json
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/typedal/pydal_objects.data.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180368 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171931 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0    23336 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60676 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1130454 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123317 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109204 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57745 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142208 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    90123 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    85337 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    28767 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0    87488 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75197 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167545 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28480 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49741 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   172768 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239632 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432234 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57845 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    89054 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407988 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128983 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79287 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70579 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91119 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350743 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/src/__init__.data.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/src/__init__.meta.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/src/typedal/__about__.data.json
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/src/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/src/typedal/__init__.data.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/src/typedal/__init__.meta.json
--rw-r--r--   0        0        0    33350 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/src/typedal/core.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/src/typedal/core.meta.json
--rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/src/typedal/fields.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/src/typedal/fields.meta.json
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typedal/__about__.data.json
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typedal/__init__.data.json
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typedal/__init__.meta.json
--rw-r--r--   0        0        0    33137 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typedal/core.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typedal/core.meta.json
--rw-r--r--   0        0        0    30390 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typedal/fields.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-1.0.0/.mypy_cache/3.11/typedal/fields.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 typedal-1.0.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 typedal-1.0.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 typedal-1.0.0/.pytest_cache/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 typedal-1.0.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 typedal-1.0.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.0.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/121ed75fe9fe5f8e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/19309938546e93ab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/197f3188bc94f91f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/1aa1390b5bde1004
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/1b34455c399f0006
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/1bd1a229a4f4ee7f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/1c46d1f378d28fbb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/1ca71ee291d82018
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/1d6bb777df44b8ec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/1dc8423cfb79eaa4
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/20585cf790eae81e
--rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/221af82ae72a7f27
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/2282e801459c52a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/248c4e1a32c704cb
--rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/24e1b4aab386ebc8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/28b1d8ac7e2aab6b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/2b7f7d266c8efaad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/2dac345be8527adf
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/2f3396c610fd7095
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/31731f8e74291475
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/3826106cf4494de8
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/38d5fd55b14a9d6c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/3afc55a04b8f8bb2
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/4022ee8774ccd98a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/42f9a2406e74c24f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/4696b157ff786f22
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/46a88ce266f1ad94
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/4a6edd5010cb9700
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/4d0230e9a81a468
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/52018ba3989fcaf7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/54e6ba8c25a22ffc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/566d94db91d23339
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/5b076d769fa5cacd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/5ceb1580c62ee794
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/6bc90dbb56504f96
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/6f0c8f98e4da1d48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/74e52af774eebdbd
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/75bd1769f6e29ed7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/815ba2cfea236769
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/876d9a8d302e1c46
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/88e2927df9448936
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/8c4d3f5ef14b0167
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/8f8ec552e76f3eab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/95c82d8566c6704c
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/a0739889bf9412e8
--rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/a225e4df39be9b29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/a2340fd4c9aa1141
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/a513d558646cd439
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/b121e2b70fd66eb8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/b218ff88bc22b626
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/b419496fa9e72887
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/b886c97e4d4117f0
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/bdcdf5c7bbc1d738
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/c06de16f3c7a64cc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/c635f255374598c5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/c671ae94ff3d3e2e
--rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/cdfecbca581311ee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/ce44121ca4091b64
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/ced49ec87d10bcb0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/cfc06a1f13c8ab47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/d16c5d29763a704e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/d225ad4c14b8ca60
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/d3a95555c0919160
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/d655bee8ff0a59f2
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/da4811a7730a562a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/dca573767bc8be7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/e3e29f9eacb7027f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/e46ab4b61bb5d446
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/e5e0cc178d5c9df5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/eb564f7989641958
--rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/eee2f3c667de6c7a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/f04d0d78a00adfd6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/f2ddc22a4b221f54
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/f879e8c947a6b7a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0/.ruff_cache/content/faa51a5044a3c279
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/d_0ccc93afd6526b6c___about___py.html
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/d_0ccc93afd6526b6c___init___py.html
--rw-r--r--   0        0        0    96583 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/d_0ccc93afd6526b6c_core_py.html
--rw-r--r--   0        0        0    63148 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/d_0ccc93afd6526b6c_fields_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 typedal-1.0.0/htmlcov/style.css
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 typedal-1.0.0/src/typedal/__about__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 typedal-1.0.0/src/typedal/__init__.py
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 typedal-1.0.0/src/typedal/core.py
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 typedal-1.0.0/src/typedal/fields.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 typedal-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     7847 2020-02-02 00:00:00.000000 typedal-1.0.0/tests/test_main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 typedal-1.0.0/.gitignore
--rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 typedal-1.0.0/README.md
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 typedal-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 typedal-1.0.0/PKG-INFO
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

### Comparing `typedal-1.0.0/CHANGELOG.md` & `typedal-1.0.0b1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
-## v1.0.0 (2023-06-05)
-Refactored pre-1.0 code and added [su6](https://github.com/robinvandernoord/su6-checker) checker tool.  
-Moved to `pyproject.toml` based build system.
-
+## v1.0.0-beta.1 (2023-06-05)
 ### Feature
 * **su6:** Add github workflow with checkers ([`d462387`](https://github.com/trialandsuccess/TypeDAL/commit/d46238705b27137ed60806eca5c53d8c2940052f))
 * **tests:** Moved tests.py to pytest ([`de33d20`](https://github.com/trialandsuccess/TypeDAL/commit/de33d2053e6499c4a8628cfc4b8813b5a649c584))
 * **define:** Pass extra kwargs (e.g. format) to define_table ([`bb692dc`](https://github.com/trialandsuccess/TypeDAL/commit/bb692dc1b2a9c18e45bcb70771b7435df8a39c8e))
 * **TypedRows:** Subscriptable return type for .select() ([`7b674b0`](https://github.com/trialandsuccess/TypeDAL/commit/7b674b07d4e61f4ead5d3f006e018b1aa66c10e7))
 * Add specific Fields, experimented with __future__.annotations (does not work right now) and general improvements ([`9af27c2`](https://github.com/trialandsuccess/TypeDAL/commit/9af27c254bf2ad7bd3bfa80e66b6e08e82f8f13a))
```

### Comparing `typedal-1.0.0/coverage.svg` & `typedal-1.0.0b1/coverage.svg`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/example_new.py` & `typedal-1.0.0b1/example_new.py`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/example_old.py` & `typedal-1.0.0b1/example_old.py`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_ast.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_ast.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_codecs.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_codecs.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_collections_abc.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_collections_abc.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_ctypes.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_ctypes.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_decimal.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_decimal.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/abc.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/abc.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/array.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/array.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/builtins.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/builtins.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/codecs.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/codecs.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/contextlib.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/contextlib.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/dataclasses.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/dataclasses.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/datetime.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/datetime.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/datetime.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/decimal.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/decimal.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/enum.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/enum.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/genericpath.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/genericpath.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/io.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/io.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/mmap.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/mmap.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/numbers.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/numbers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/numbers.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/pathlib.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/pathlib.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/pickle.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/pickle.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/posixpath.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/posixpath.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/re.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/re.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/sre_compile.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/sre_compile.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/sre_constants.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/sre_constants.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/sre_parse.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/sre_parse.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/subprocess.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/subprocess.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/sys.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/sys.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/time.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/time.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/types.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/types.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/typing.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/typing.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/typing_extensions.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/typing_extensions.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_typeshed/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/collections/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/collections/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/collections/abc.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/collections/abc.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/ctypes/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/ctypes/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/charset.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/charset.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/contentmanager.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/contentmanager.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/errors.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/errors.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/header.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/header.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/message.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/message.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/policy.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/email/policy.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/importlib/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/importlib/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/importlib/abc.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/importlib/abc.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/importlib/machinery.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/importlib/machinery.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/os/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/os/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/os/path.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/os/path.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/typedal/__about__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/typedal/__about__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/typedal/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/typedal/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/typedal/core.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/typedal/core.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/typedal/fields.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/typedal/fields.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/fields.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/typedal/pydal_objects.data.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/pydal_objects.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_ast.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_ast.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_codecs.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_codecs.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_collections_abc.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_collections_abc.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_ctypes.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_ctypes.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_decimal.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_decimal.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/abc.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/abc.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/array.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/array.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/builtins.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/builtins.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/codecs.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/codecs.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/contextlib.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/contextlib.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/dataclasses.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/dataclasses.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/datetime.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/datetime.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/decimal.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/decimal.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/enum.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/enum.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/genericpath.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/genericpath.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/io.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/io.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/mmap.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/mmap.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/numbers.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/numbers.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/pathlib.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/pathlib.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/pickle.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/pickle.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/posixpath.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/posixpath.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/re.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/re.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/sre_compile.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/sre_compile.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/sre_constants.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/sre_constants.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/sre_parse.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/sre_parse.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/subprocess.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/subprocess.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/sys.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/sys.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/time.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/time.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/types.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/types.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typing.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typing.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typing_extensions.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typing_extensions.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_typeshed/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/collections/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/collections/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/collections/abc.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/collections/abc.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/ctypes/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/ctypes/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/charset.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/charset.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/contentmanager.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/contentmanager.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/errors.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/errors.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/header.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/header.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/message.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/message.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/policy.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/email/policy.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/importlib/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/importlib/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/importlib/abc.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/importlib/abc.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/importlib/machinery.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/importlib/machinery.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/os/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/os/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/os/path.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/os/path.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/src/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/src/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/src/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/src/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/src/typedal/__about__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/src/typedal/__about__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/src/typedal/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/src/typedal/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/src/typedal/core.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/src/typedal/core.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/src/typedal/fields.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/src/typedal/fields.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/fields.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typedal/__about__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typedal/__about__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typedal/__init__.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typedal/__init__.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typedal/core.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typedal/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typedal/core.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typedal/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typedal/fields.data.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.mypy_cache/3.11/typedal/fields.meta.json` & `typedal-1.0.0b1/.mypy_cache/3.11/typedal/fields.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/1b34455c399f0006` & `typedal-1.0.0b1/.ruff_cache/content/1b34455c399f0006`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/20585cf790eae81e` & `typedal-1.0.0b1/.ruff_cache/content/20585cf790eae81e`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/221af82ae72a7f27` & `typedal-1.0.0b1/.ruff_cache/content/221af82ae72a7f27`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/24e1b4aab386ebc8` & `typedal-1.0.0b1/.ruff_cache/content/24e1b4aab386ebc8`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/2f3396c610fd7095` & `typedal-1.0.0b1/.ruff_cache/content/2f3396c610fd7095`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/3826106cf4494de8` & `typedal-1.0.0b1/.ruff_cache/content/3826106cf4494de8`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/38d5fd55b14a9d6c` & `typedal-1.0.0b1/.ruff_cache/content/38d5fd55b14a9d6c`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/4022ee8774ccd98a` & `typedal-1.0.0b1/.ruff_cache/content/4022ee8774ccd98a`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/75bd1769f6e29ed7` & `typedal-1.0.0b1/.ruff_cache/content/75bd1769f6e29ed7`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/a0739889bf9412e8` & `typedal-1.0.0b1/.ruff_cache/content/a0739889bf9412e8`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/a225e4df39be9b29` & `typedal-1.0.0b1/.ruff_cache/content/a225e4df39be9b29`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/b419496fa9e72887` & `typedal-1.0.0b1/.ruff_cache/content/b419496fa9e72887`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/bdcdf5c7bbc1d738` & `typedal-1.0.0b1/.ruff_cache/content/bdcdf5c7bbc1d738`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/c06de16f3c7a64cc` & `typedal-1.0.0b1/.ruff_cache/content/c06de16f3c7a64cc`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/cdfecbca581311ee` & `typedal-1.0.0b1/.ruff_cache/content/cdfecbca581311ee`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/da4811a7730a562a` & `typedal-1.0.0b1/.ruff_cache/content/da4811a7730a562a`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/.ruff_cache/content/eee2f3c667de6c7a` & `typedal-1.0.0b1/.ruff_cache/content/eee2f3c667de6c7a`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/coverage_html.js` & `typedal-1.0.0b1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/d_0ccc93afd6526b6c___about___py.html` & `typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c___about___py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/d_0ccc93afd6526b6c___init___py.html` & `typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c___init___py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/d_0ccc93afd6526b6c_core_py.html` & `typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c_core_py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/d_0ccc93afd6526b6c_fields_py.html` & `typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c_fields_py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/favicon_32.png` & `typedal-1.0.0b1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/index.html` & `typedal-1.0.0b1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/keybd_closed.png` & `typedal-1.0.0b1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/keybd_open.png` & `typedal-1.0.0b1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/status.json` & `typedal-1.0.0b1/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/htmlcov/style.css` & `typedal-1.0.0b1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/src/typedal/core.py` & `typedal-1.0.0b1/src/typedal/core.py`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/src/typedal/fields.py` & `typedal-1.0.0b1/src/typedal/fields.py`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/tests/test_main.py` & `typedal-1.0.0b1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/README.md` & `typedal-1.0.0b1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # TypeDAL
 
-[![PyPI - Version](https://img.shields.io/pypi/v/TypeDAL.svg)](https://pypi.org/project/TypeDAL)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/TypeDAL.svg)](https://pypi.org/project/TypeDAL)  
+[![PyPI - Version](https://img.shields.io/pypi/v/TypeDal.svg)](https://pypi.org/project/typedal)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/TypeDal.svg)](https://pypi.org/project/typedal)  
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
-[![su6 checks](https://github.com/trialandsuccess/TypeDAL/actions/workflows/su6.yml/badge.svg?branch=development)](https://github.com/trialandsuccess/TypeDAL/actions)
+[![su6 checks](https://github.com/trialandsuccess/typedal/actions/workflows/su6.yml/badge.svg)](https://github.com/trialandsuccess/typedal/actions)
 ![coverage.svg](coverage.svg)
 
 Typing support for [PyDAL](http://web2py.com/books/default/chapter/29/6).
 This package aims to improve the typing support for PyDAL. By using classes instead of the define_table method,
 type hinting the result of queries can improve the experience while developing. In the background, the queries are still
 generated and executed by pydal itself, this package only proves some logic to properly pass calls from class methods to
 the underlying `db.define_table` pydal Tables.
```

### Comparing `typedal-1.0.0/pyproject.toml` & `typedal-1.0.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0/PKG-INFO` & `typedal-1.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TypeDal
-Version: 1.0.0
+Version: 1.0.0b1
 Summary: Typing support for PyDAL
 Project-URL: Documentation, https://github.com/trialandsuccess/TypeDAL#readme
 Project-URL: Issues, https://github.com/trialandsuccess/TypeDAL/issues
 Project-URL: Source, https://github.com/trialandsuccess/TypeDAL
 Author-email: Robin van der Noord <contact@trialandsuccess.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -20,19 +20,19 @@
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: python-semantic-release; extra == 'dev'
 Requires-Dist: su6[all]; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # TypeDAL
 
-[![PyPI - Version](https://img.shields.io/pypi/v/TypeDAL.svg)](https://pypi.org/project/TypeDAL)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/TypeDAL.svg)](https://pypi.org/project/TypeDAL)  
+[![PyPI - Version](https://img.shields.io/pypi/v/TypeDal.svg)](https://pypi.org/project/typedal)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/TypeDal.svg)](https://pypi.org/project/typedal)  
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
-[![su6 checks](https://github.com/trialandsuccess/TypeDAL/actions/workflows/su6.yml/badge.svg?branch=development)](https://github.com/trialandsuccess/TypeDAL/actions)
+[![su6 checks](https://github.com/trialandsuccess/typedal/actions/workflows/su6.yml/badge.svg)](https://github.com/trialandsuccess/typedal/actions)
 ![coverage.svg](coverage.svg)
 
 Typing support for [PyDAL](http://web2py.com/books/default/chapter/29/6).
 This package aims to improve the typing support for PyDAL. By using classes instead of the define_table method,
 type hinting the result of queries can improve the experience while developing. In the background, the queries are still
 generated and executed by pydal itself, this package only proves some logic to properly pass calls from class methods to
 the underlying `db.define_table` pydal Tables.
```

