# Comparing `tmp/fnattr-0.2.6.tar.gz` & `tmp/fnattr-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnattr-0.2.6.tar", last modified: Tue May 30 23:03:44 2023, max compression
+gzip compressed data, was "fnattr-0.2.7.tar", last modified: Mon Jun  5 21:53:09 2023, max compression
```

## Comparing `fnattr-0.2.6.tar` & `fnattr-0.2.7.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-06 18:55:15.000000 fnattr-0.2.6/LICENSE
--rw-rw-r--   0 kevin     (1001) dialout     (20)       31 2023-05-07 00:42:08.000000 fnattr-0.2.6/MANIFEST.in
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5234 2023-05-30 23:03:43.000000 fnattr-0.2.6/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4583 2023-05-30 23:01:41.000000 fnattr-0.2.6/README.md
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:42.000000 fnattr-0.2.6/config/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1638 2023-05-27 20:42:39.000000 fnattr-0.2.6/config/config.toml
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:42.000000 fnattr-0.2.6/doc/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2984 2023-05-30 12:24:39.000000 fnattr-0.2.6/doc/configuration.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)    10407 2023-05-25 00:54:41.000000 fnattr-0.2.6/doc/fna.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4501 2023-05-30 12:57:29.000000 fnattr-0.2.6/doc/keys.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4569 2023-05-30 23:01:46.000000 fnattr-0.2.6/pyproject.toml
--rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-05-30 23:03:43.000000 fnattr-0.2.6/setup.cfg
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:42.000000 fnattr-0.2.6/src/
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:42.000000 fnattr-0.2.6/src/fnattr/
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:42.000000 fnattr-0.2.6/src/fnattr/extra/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4940 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/extra/fnaffle.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4547 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/extra/make_isbn_ranges.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:42.000000 fnattr-0.2.6/src/fnattr/fna/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3520 2023-05-30 23:01:42.000000 fnattr-0.2.6/src/fnattr/fna/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/util/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:42.000000 fnattr-0.2.6/src/fnattr/util/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      778 2023-05-30 23:01:42.000000 fnattr-0.2.6/src/fnattr/util/checksum.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3648 2023-05-30 23:01:42.000000 fnattr-0.2.6/src/fnattr/util/config.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      625 2023-05-30 23:01:42.000000 fnattr-0.2.6/src/fnattr/util/docsplit.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     9200 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/util/duration.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      102 2023-05-30 23:01:43.000000 fnattr-0.2.6/src/fnattr/util/error.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2181 2023-05-30 23:01:43.000000 fnattr-0.2.6/src/fnattr/util/escape.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1082 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/util/fearmat.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1857 2023-05-30 23:01:43.000000 fnattr-0.2.6/src/fnattr/util/io.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3535 2023-05-30 23:01:43.000000 fnattr-0.2.6/src/fnattr/util/multimap.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1063 2023-05-30 23:01:43.000000 fnattr-0.2.6/src/fnattr/util/pytestutil.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1738 2023-05-30 23:01:43.000000 fnattr-0.2.6/src/fnattr/util/registry.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1099 2023-05-30 23:01:43.000000 fnattr-0.2.6/src/fnattr/util/repr.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8107 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/util/sqlite.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      438 2023-05-30 23:01:44.000000 fnattr-0.2.6/src/fnattr/util/typecheck.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1797 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      401 2023-05-30 23:01:44.000000 fnattr-0.2.6/src/fnattr/vlju/testutil.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:44.000000 fnattr-0.2.6/src/fnattr/vlju/types/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      920 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/all.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/doi/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4175 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/doi/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)  1136932 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/doi/org.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/ean/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1687 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/ean/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3214 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/ean/isbn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    40480 2023-05-30 23:01:45.000000 fnattr-0.2.6/src/fnattr/vlju/types/ean/isbn_ranges.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      666 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/ean/ismn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1307 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/ean/issn.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/file/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1998 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/file/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      983 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/info/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2870 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/info/kinds.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/lccn/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1282 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/lccn/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/site/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3990 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/site/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/timestamp/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      888 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/timestamp/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/uri/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8655 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/uri/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/url/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      772 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/url/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vlju/types/urn/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1372 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/urn/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4046 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vlju/types/urn/kinds.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vljum/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8572 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vljum/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2831 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vljum/m.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    10570 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vljum/runner.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:43.000000 fnattr-0.2.6/src/fnattr/vljumap/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1218 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vljumap/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    20919 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vljumap/enc.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1357 2023-05-30 23:01:46.000000 fnattr-0.2.6/src/fnattr/vljumap/factory.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:03:42.000000 fnattr-0.2.6/src/fnattr.egg-info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5234 2023-05-30 23:03:42.000000 fnattr-0.2.6/src/fnattr.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1696 2023-05-30 23:03:42.000000 fnattr-0.2.6/src/fnattr.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-05-30 23:03:42.000000 fnattr-0.2.6/src/fnattr.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       76 2023-05-30 23:03:42.000000 fnattr-0.2.6/src/fnattr.egg-info/entry_points.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        7 2023-05-30 23:03:42.000000 fnattr-0.2.6/src/fnattr.egg-info/top_level.txt
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-06 18:55:15.000000 fnattr-0.2.7/LICENSE
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       31 2023-05-07 00:42:08.000000 fnattr-0.2.7/MANIFEST.in
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5174 2023-06-05 21:53:09.000000 fnattr-0.2.7/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4523 2023-06-03 16:51:05.000000 fnattr-0.2.7/README.md
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/config/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1638 2023-05-27 20:42:39.000000 fnattr-0.2.7/config/vlju.toml
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/doc/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2976 2023-05-31 13:53:09.000000 fnattr-0.2.7/doc/configuration.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10407 2023-05-25 00:54:41.000000 fnattr-0.2.7/doc/fna.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4501 2023-05-30 12:57:29.000000 fnattr-0.2.7/doc/keys.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4647 2023-06-05 20:11:45.000000 fnattr-0.2.7/pyproject.toml
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-06-05 21:53:09.000000 fnattr-0.2.7/setup.cfg
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr/
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr/extra/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5193 2023-06-03 16:43:56.000000 fnattr-0.2.7/src/fnattr/extra/fnaffle.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4547 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/extra/make_isbn_ranges.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr/fna/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3961 2023-06-03 16:43:56.000000 fnattr-0.2.7/src/fnattr/fna/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/util/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:42.000000 fnattr-0.2.7/src/fnattr/util/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      778 2023-05-30 23:01:42.000000 fnattr-0.2.7/src/fnattr/util/checksum.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3735 2023-06-03 16:45:07.000000 fnattr-0.2.7/src/fnattr/util/config.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      625 2023-05-30 23:01:42.000000 fnattr-0.2.7/src/fnattr/util/docsplit.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9200 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/util/duration.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      102 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/error.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2181 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/escape.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1082 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/util/fearmat.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1857 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/io.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3535 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/multimap.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1063 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/pytestutil.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1738 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/registry.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1099 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/repr.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8107 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/util/sqlite.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      438 2023-05-30 23:01:44.000000 fnattr-0.2.7/src/fnattr/util/typecheck.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1797 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      401 2023-05-30 23:01:44.000000 fnattr-0.2.7/src/fnattr/vlju/testutil.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:44.000000 fnattr-0.2.7/src/fnattr/vlju/types/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      920 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/all.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/doi/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4175 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/doi/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)  1136932 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/doi/org.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1687 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3214 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/isbn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    40480 2023-05-30 23:01:45.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/isbn_ranges.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      666 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/ismn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1307 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/issn.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/file/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1998 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/file/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      983 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/info/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2870 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/info/kinds.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/lccn/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1282 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/lccn/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/site/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3990 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/site/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/timestamp/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      888 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/timestamp/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/uri/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8655 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/uri/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/url/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      772 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/url/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/urn/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1372 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/urn/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4046 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/urn/kinds.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vljum/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8666 2023-06-05 17:44:49.000000 fnattr-0.2.7/src/fnattr/vljum/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3007 2023-06-03 16:43:56.000000 fnattr-0.2.7/src/fnattr/vljum/m.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10570 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vljum/runner.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vljumap/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1218 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vljumap/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    22971 2023-06-05 15:10:26.000000 fnattr-0.2.7/src/fnattr/vljumap/enc.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1357 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vljumap/factory.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5174 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1694 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       76 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/entry_points.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        7 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/top_level.txt
```

### Comparing `fnattr-0.2.6/LICENSE` & `fnattr-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/PKG-INFO` & `fnattr-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnattr
-Version: 0.2.6
+Version: 0.2.7
 Summary: Manage key/value metadata in file names.
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/fna
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -97,22 +97,22 @@
 $ fna file '/tmp/My Book.pdf' add isbn 1234567890 json encode
 {"title": ["My Book"], "isbn": ["9781234567897"]}
 ```
 
 ## Configuration
 
 Unless otherwise directed by a command line option,
-`fna` tries to read `vlju/config.toml` or `fna/config.toml`
+`fna` tries to read `fnattr/vlju.toml` or `fnattr/fna.toml`
 from XDG locations (e.g. `$HOME/.config/`).
 The former is shared by all tools using the Vlju
 library, while the latter applies only to the `fna` command.
 
 This file can define keys and classes associated with web sites,
-mapping from a compact ID to a URL. (The other direction does not yet exist.)
-The distribution file `config/config.toml` contains some examples.
+mapping between a compact ID to a URL.
+The distribution file `config/vlju.toml` contains some examples.
 
 See [doc/configuration.md](doc/configuration.md) for more information.
 
 ## Implementation
 
 The current public home for `fna` is
 [https://codeberg.org/datatravelandexperiments/fna](https://codeberg.org/datatravelandexperiments/fna)
@@ -158,8 +158,7 @@
 
 The command line tool `fna`.
 
 ### TODO
 
 - Better error handling. Too much still just raises exceptions.
 - Document operation with `-[EFx]`.
-- Logging options?
```

### Comparing `fnattr-0.2.6/README.md` & `fnattr-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -78,22 +78,22 @@
 $ fna file '/tmp/My Book.pdf' add isbn 1234567890 json encode
 {"title": ["My Book"], "isbn": ["9781234567897"]}
 ```
 
 ## Configuration
 
 Unless otherwise directed by a command line option,
-`fna` tries to read `vlju/config.toml` or `fna/config.toml`
+`fna` tries to read `fnattr/vlju.toml` or `fnattr/fna.toml`
 from XDG locations (e.g. `$HOME/.config/`).
 The former is shared by all tools using the Vlju
 library, while the latter applies only to the `fna` command.
 
 This file can define keys and classes associated with web sites,
-mapping from a compact ID to a URL. (The other direction does not yet exist.)
-The distribution file `config/config.toml` contains some examples.
+mapping between a compact ID to a URL.
+The distribution file `config/vlju.toml` contains some examples.
 
 See [doc/configuration.md](doc/configuration.md) for more information.
 
 ## Implementation
 
 The current public home for `fna` is
 [https://codeberg.org/datatravelandexperiments/fna](https://codeberg.org/datatravelandexperiments/fna)
@@ -139,8 +139,7 @@
 
 The command line tool `fna`.
 
 ### TODO
 
 - Better error handling. Too much still just raises exceptions.
 - Document operation with `-[EFx]`.
-- Logging options?
```

### Comparing `fnattr-0.2.6/config/config.toml` & `fnattr-0.2.7/config/vlju.toml`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/doc/configuration.md` & `fnattr-0.2.7/doc/configuration.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Configuration
 
 Configuration files are in [TOML](https://toml.io/) form.
 
 ## Default configuration files
 
 Unless otherwise directed by a command line option,
-`fna` tries to read `vlju/config.toml` or `fna/config.toml`
+`fna` tries to read `fnattr/vlju.toml` and/or `fnattr/fna.toml`
 under XDG locations (e.g. `$XDG_CONFIG_HOME/` or `$HOME/.config/`).
-The former — the `vlju` subdirectory — is shared by all tools
+The former — `vlju.toml` — is shared by all tools
 using the Vlju library; the latter applies only to the `fna` command.
 
 ## Sections
 
 ### `[option]`
 
 An `[option]` section can contain key-value pairs corresponding
```

### Comparing `fnattr-0.2.6/doc/fna.md` & `fnattr-0.2.7/doc/fna.md`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/doc/keys.md` & `fnattr-0.2.7/doc/keys.md`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/pyproject.toml` & `fnattr-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fnattr"
-version = "0.2.6"
+version = "0.2.7"
 description = "Manage key/value metadata in file names."
 license.text = "MIT License"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
@@ -109,14 +109,15 @@
     "D203",     # one-blank-line-before-class: Conflicts with D211.
     "D212",     # multi-line-summary-first-line: Conflicts with D213.
     "PLR0912",  # too-many-branches: Be direct.
     "PLR0913",  # too-many-arguments: Be direct.
     "PLR2004",  # magic-value-comparison: Be direct.
     "S314", 	# suspicious-xml-element-tree-usage: defusedxml is not builtin.
     "T20",      # flake8-print: I like having output.
+    "TRY400",   # error-instead-of-exception: Don't dump traces on end users.
 ]
 
 [tool.ruff.flake8-annotations]
 allow-star-arg-any = true
 suppress-dummy-args = true
 
 [tool.ruff.flake8-quotes]
```

### Comparing `fnattr-0.2.6/src/fnattr/extra/fnaffle.py` & `fnattr-0.2.7/src/fnattr/extra/fnaffle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: MIT
 """Move files to directories based on matching attributes."""
 
 import argparse
+import logging
 import sys
 
 from collections.abc import Iterable
 from pathlib import Path
 
 from fnattr.util.config import read_cmd_configs, xdg_config
 from fnattr.vljum.m import M
@@ -118,59 +119,62 @@
         '--map',
         '-m',
         metavar='FILE',
         type=str,
         action='append',
         help='Renaming map file.')
     parser.add_argument(
-        '--verbose',
-        '-v',
-        default=False,
-        action='store_true',
-        help='Report renaming.')
+        '--log-level',
+        '-L',
+        metavar='LEVEL',
+        type=str,
+        choices=[c for c in logging.getLevelNamesMapping() if c != 'NOTSET'],
+        default='INFO')
     parser.add_argument(
         'file',
         metavar='FILENAME',
         type=str,
         nargs=argparse.REMAINDER,
         default=[],
         help='File name(s).')
     args = parser.parse_args(argv[1 :])
+    logging.basicConfig(level=getattr(logging, args.log_level.upper()),
+                        format=f'{cmd}: %(levelname)s: %(message)s')
 
     config = read_cmd_configs(cmd, args.config)
     options = config.get('option', {})
     if args.decoder:
         options['decoder'] = args.decoder
     M.configure_options(options)
     M.configure_sites(config.get('site', {}))
 
     try:
         if not args.map:
             args.map = find_map_files(cmd)
         if not args.map:
-            print(f'{cmd}: no map file.')
+            logging.error('%s: no map file', cmd)
             return 1
         maps = read_map_files(args.map)
         for file in args.file:
             m = M().file(file)
             if dst := match_maps(maps, m):
                 if not dst.exists():
                     if not args.dryrun:
                         dst.mkdir(parents=True)
-                    if args.dryrun or args.verbose:
-                        print(f'{dst}: created')
+                    logging.info('%s: created', dst)
                 if not args.dryrun:
                     try:
                         m.with_dir(dst).rename()
-                    except FileExistsError as e:
-                        print(f'{cmd}: file exists: {e}')
+                    except FileExistsError:
+                        logging.error('file exists: %s', file)
                 if args.dryrun or args.verbose:
                     print(f'{dst}: {file}')
             elif args.verbose:
                 print(f'no match for {file}')
     except Exception as e:
-        print(f'{cmd}: Unhandled exception: {type(e).__name__}{e.args}')
-        raise
+        logging.error('Unhandled exception: %s%s', type(e).__name__, e.args)
+        if logging.getLogger().getEffectiveLevel() < logging.INFO:
+            raise
     return 0
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `fnattr-0.2.6/src/fnattr/extra/make_isbn_ranges.py` & `fnattr-0.2.7/src/fnattr/extra/make_isbn_ranges.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/fna/__init__.py` & `fnattr-0.2.7/src/fnattr/fna/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: MIT
 """`fna` command."""
 
 import argparse
+import logging
 import pathlib
 import sys
 
 import fnattr.util.config
 import fnattr.util.io
 import fnattr.vljum.m
 import fnattr.vljum.runner
@@ -38,14 +39,21 @@
     parser.add_argument(
         '--encoder',
         '-e',
         metavar='ENCODER',
         type=str,
         choices=fnattr.vljumap.enc.encoder.keys(),
         help='Default string encoder.')
+    parser.add_argument(
+        '--log-level',
+        '-L',
+        metavar='LEVEL',
+        type=str,
+        choices=[c for c in logging.getLevelNamesMapping() if c != 'NOTSET'],
+        default='INFO')
     mode = parser.add_mutually_exclusive_group()
     mode.add_argument(
         '--dsl',
         '-D',
         dest='mode',
         default='dsl',
         const='dsl',
@@ -77,14 +85,17 @@
         metavar='ARGUMENT',
         type=str,
         nargs=argparse.REMAINDER,
         default=[],
         help='Part of a subcommand, or an expression or statement.')
     args = parser.parse_args(argv[1 :])
 
+    logging.basicConfig(level=getattr(logging, args.log_level.upper()),
+                        format=f'{cmd}: %(levelname)s: %(message)s')
+
     config = fnattr.util.config.read_cmd_configs(cmd, args.config)
     options = config.get('option', {})
     if args.decoder:
         options['decoder'] = args.decoder
     if args.encoder:
         options['encoder'] = args.encoder
     fnattr.vljum.m.M.configure_options(options)
@@ -103,15 +114,16 @@
                 for i in args.argument:
                     fnattr.vljum.m.M.execute(i)
             case 'file':
                 for i in args.argument:
                     with fnattr.util.io.open_input(i) as f:
                         fnattr.vljum.m.M.execute(f.read())
             case _:
-                print(f'{cmd}: Unknown mode: {args.mode}')
+                logging.error('Unknown mode: %s', args.mode)
     except Exception as e:
-        print(f'{cmd}: Unhandled exception: {type(e).__name__}{e.args}')
-        raise
+        logging.error('Unhandled exception: %s%s', type(e).__name__, e.args)
+        if logging.getLogger().getEffectiveLevel() < logging.INFO:
+            raise
     return 0
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `fnattr-0.2.6/src/fnattr/util/checksum.py` & `fnattr-0.2.7/src/fnattr/util/checksum.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/util/config.py` & `fnattr-0.2.7/src/fnattr/util/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: MIT
 """Configuration-file related utilities."""
 
 import contextlib
+import logging
 import os
 import tomllib
 
 from collections.abc import Iterable
 from pathlib import Path
 from typing import Any, Self
 
@@ -77,15 +78,15 @@
     return xdg_config_dirs().find_first(filename)
 
 def read_toml_config(file: Path | str) -> dict | None:
     with Path(file).open('rb') as f:
         try:
             return tomllib.load(f)
         except tomllib.TOMLDecodeError as e:
-            print(f'{file}: {e}')
+            logging.error('%s: %s', file, str(e))
             return None
 
 def read_configs(args: Iterable[Path | str]) -> dict:
     config: dict[str, Any] = {}
     for p in args:
         if c := read_toml_config(p):
             nested_update(config, c)
@@ -98,16 +99,18 @@
             nested_update(config, c)
     return config
 
 def read_cmd_configs(cmd: str, args: Iterable[Path | str]) -> dict:
     if args:
         return read_configs(args)
     return read_xdg_configs([
-        Path('vlju/config.toml'),
-        Path(f'{cmd}/config.toml'),
+        Path('vlju.toml'),
+        Path('fnattr/vlju.toml'),
+        Path(f'{cmd}.toml'),
+        Path(f'fnattr/{cmd}.toml'),
     ])
 
 def nested_update(dst: dict, src: dict) -> dict:
     for k, v in src.items():
         if k in dst and isinstance(dst[k], dict) and isinstance(v, dict):
             nested_update(dst[k], v)
         else:
```

### Comparing `fnattr-0.2.6/src/fnattr/util/docsplit.py` & `fnattr-0.2.7/src/fnattr/util/docsplit.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/util/duration.py` & `fnattr-0.2.7/src/fnattr/util/duration.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/util/escape.py` & `fnattr-0.2.7/src/fnattr/util/escape.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/util/fearmat.py` & `fnattr-0.2.7/src/fnattr/util/fearmat.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/util/io.py` & `fnattr-0.2.7/src/fnattr/util/io.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/util/multimap.py` & `fnattr-0.2.7/src/fnattr/util/multimap.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/util/pytestutil.py` & `fnattr-0.2.7/src/fnattr/util/pytestutil.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/util/registry.py` & `fnattr-0.2.7/src/fnattr/util/registry.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/util/repr.py` & `fnattr-0.2.7/src/fnattr/util/repr.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/util/sqlite.py` & `fnattr-0.2.7/src/fnattr/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/all.py` & `fnattr-0.2.7/src/fnattr/vlju/types/all.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/doi/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/types/doi/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/doi/org.py` & `fnattr-0.2.7/src/fnattr/vlju/types/doi/org.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/ean/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/types/ean/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/ean/isbn.py` & `fnattr-0.2.7/src/fnattr/vlju/types/ean/isbn.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/ean/isbn_ranges.py` & `fnattr-0.2.7/src/fnattr/vlju/types/ean/isbn_ranges.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/ean/ismn.py` & `fnattr-0.2.7/src/fnattr/vlju/types/ean/ismn.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/ean/issn.py` & `fnattr-0.2.7/src/fnattr/vlju/types/ean/issn.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/file/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/info/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/types/info/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/info/kinds.py` & `fnattr-0.2.7/src/fnattr/vlju/types/info/kinds.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/lccn/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/types/lccn/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/site/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/types/site/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/timestamp/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/types/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/uri/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/types/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/url/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/types/url/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/urn/__init__.py` & `fnattr-0.2.7/src/fnattr/vlju/types/urn/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vlju/types/urn/kinds.py` & `fnattr-0.2.7/src/fnattr/vlju/types/urn/kinds.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vljum/__init__.py` & `fnattr-0.2.7/src/fnattr/vljum/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,28 +31,28 @@
         self.factory = copy.copy(self.default_registry['factory'])
         self.encoder = copy.copy(self.default_registry['encoder'])
         self.decoder = copy.copy(self.default_registry['decoder'])
         self.mode = copy.copy(self.default_registry['mode'])
         self._original_path: Path
         self._current_dir: Path
         self._current_suffix: str
-        self._set_path(Path())
+        self.set_path(Path())
         if i is not None:
             if isinstance(i, VljuMap):
                 self.extend(i)
             elif isinstance(i, File):
                 self.file(i.filename())
             elif isinstance(i, Path):
-                self._set_path(i)
+                self.set_path(i)
             elif isinstance(i, str):
                 self.decode(i)
             elif hasattr(i, 'cast_params'):
                 s, d = i.cast_params(type(self))
                 if s:
-                    self._set_path(s)
+                    self.set_path(s)
                 for k, v in d.items():
                     self.add(k, v)
             else:
                 raise TypeError(i)
 
     def cast_params(self, t: object) -> tuple[str | Path, dict]:
         if t is File:
@@ -80,18 +80,20 @@
     def extract(self, *args: str) -> Self:
         return self.submap(args)
 
     def file(self,
              s: str | Path,
              decoder: EncoderArg = None,
              factory: FactoryArg = None) -> Self:
-        self._set_path(s)
-        self.decoder.get(decoder).decode(self,
-                                         self._original_path.stem,
-                                         self.factory.get(factory))
+        self.set_path(s)
+        r = self.decoder.get(decoder).decode_file(self,
+                                                  self._original_path,
+                                                  self.factory.get(factory))
+        self._current_dir = r.directory
+        self._current_suffix = r.suffix
         return self
 
     def order(self, *args: str) -> Self:
         return self.sortkeys(args or None)
 
     def read(self,
              file: PathLike = '-',
@@ -119,15 +121,15 @@
             raise Error(message)
         modified_path = self.filename(encoder, self.mode.get(mode))
         if modified_path.exists():
             if modified_path.samefile(self._original_path):
                 return self
             raise FileExistsError(modified_path)
         self._original_path.rename(modified_path)
-        self._set_path(modified_path)
+        self.set_path(modified_path)
         return self
 
     def reset(self,
               k: str,
               v: VljuArg = None,
               factory: FactoryArg = None) -> Self:
         del self[k]
@@ -194,15 +196,16 @@
     def filename(self,
                  encoder: EncoderArg = None,
                  mode: ModeArg = None) -> Path:
         e = self.encode(encoder, self.mode.get(mode))
         if not e:
             message = 'no file name'
             raise Error(message)
-        return (self._current_dir / e).with_suffix(self._current_suffix)
+        e += self._current_suffix
+        return self._current_dir / e
 
     # Vlju reduction.
 
     def first(self, k: str | type[Vlju]) -> Vlju:
         if isinstance(k, str):
             if k in self:
                 return self[k][0]
@@ -210,15 +213,15 @@
             for _, v in self.pairs():
                 if isinstance(v, k):
                     return v
         return Vlju('')
 
     # Helpers.
 
-    def _set_path(self, s: str | Path) -> Self:
+    def set_path(self, s: str | Path) -> Self:
         if isinstance(s, str):
             s = Path(s)
         self._original_path = s
         self._current_dir = s.parent
         self._current_suffix = s.suffix
         return self
 
@@ -233,19 +236,19 @@
                 u = None
             if u:
                 out.add(k, u)
             else:
                 strings.append((k, str(v)))
         if strings:
             scheme_slashes_re = re.compile(r'\w+://.+')
-            for k, v in strings:
-                if '/' not in v or scheme_slashes_re.fullmatch(v):
-                    t = v
+            for k, s in strings:
+                if '/' not in s or scheme_slashes_re.fullmatch(s):
+                    t = s
                 else:
-                    t = 'http://' + v
+                    t = 'http://' + s
                 u = cls(t)
                 if u and hasattr(u, 'authority') and u.authority():
                     out.add(k, u)
         return out
 
     def _vlju(self, k: str, v: VljuArg, factory: FactoryArg = None) -> Vlju:
         if v is None:
```

### Comparing `fnattr-0.2.6/src/fnattr/vljum/m.py` & `fnattr-0.2.7/src/fnattr/vljum/m.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from collections.abc import Callable, Mapping
 from pathlib import Path
 from typing import Any
 
 from fnattr.util.registry import Registry
 from fnattr.vlju.types.all import VLJU_TYPES, Vlju
-from fnattr.vlju.types.site import site_class
+from fnattr.vlju.types.site import SiteBase, site_class
 from fnattr.vljum import VljuM
 from fnattr.vljumap import enc
 from fnattr.vljumap.factory import (
     LooseMappedFactory,
     MappedFactory,
     default_factory,
 )
@@ -38,21 +38,30 @@
             Registry().update(enc.decoder).set_default('v3'),
         'mode':
             Registry().update({
                 k: k
                 for k in ('short', 'long', 'repr')
             }).set_default('short'),
     }
+    site_classes: dict[str, type[SiteBase]] = {}
 
     @classmethod
     def configure_sites(cls, site: Mapping[str, Mapping[str, Any]]) -> None:
         for k, s in site.items():
             scls = site_class(**s)
             cls.strict_factory.setitem(k, scls)
             cls.loose_factory.setitem(k, scls)
+            cls.site_classes[k] = scls
+
+    @classmethod
+    def from_site_url(cls, url: str) -> tuple[str | None, SiteBase | None]:
+        for k, scls in cls.site_classes.items():
+            if (v := scls.match_url(url)):
+                return k, scls(v)
+        return None, None
 
     @classmethod
     def exports(cls) -> dict[str, Any]:
         x = EXPORTS.copy()
         for k, v in cls.strict_factory.kmap.items():
             x[k] = v
             x[v.__name__] = v
@@ -78,19 +87,19 @@
 
     def f(*args, **kwargs) -> Any:  # noqa: ANN401
         return method(cls(), *args, **kwargs)
 
     return f
 
 EXPORTS: dict[str, Any] = {
-                                                            # Aliases
+    # Aliases
     'Path': Path,
     'V': Vlju,
 } | {
-                                                            # Module definitions
+    # Module definitions
     k: globals()[k]
     for k in ('M', )
 } | {
-                                                            # M() methods
+    # M() methods
     k: _make_free_function(M, k)
     for k in ('add', 'decode', 'file', 'read', 'reset')
 }
```

### Comparing `fnattr-0.2.6/src/fnattr/vljum/runner.py` & `fnattr-0.2.7/src/fnattr/vljum/runner.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vljumap/__init__.py` & `fnattr-0.2.7/src/fnattr/vljumap/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr/vljumap/enc.py` & `fnattr-0.2.7/src/fnattr/vljumap/enc.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,46 +5,65 @@
 import io
 import json as py_json
 import re
 import shlex
 import warnings
 
 from collections.abc import Callable, Generator, Iterable
+from dataclasses import dataclass
+from pathlib import Path
 from typing import NamedTuple
 
 from fnattr.util import escape
 from fnattr.util.error import Error
 from fnattr.util.multimap import MultiMap
 from fnattr.vlju.types.ean.isbn import is_valid_isbn10, is_valid_isbn13
 from fnattr.vljumap import VljuFactory, VljuMap
 
+@dataclass
+class DecodeFileResult:
+    directory: Path
+    stem: str
+    suffix: str
+
 EncodeCallable = Callable[[VljuMap, str | None], str]
 DecodeCallable = Callable[[VljuMap, str, VljuFactory], VljuMap]
+DecodeFileCallable = Callable[[VljuMap, Path, VljuFactory], DecodeFileResult]
 
 class Encoder:
     """Scheme for for encoding and decoding VljuMap."""
 
     def __init__(self,
                  name: str,
                  encode: EncodeCallable | None,
                  decode: DecodeCallable | None,
+                 decode_file: DecodeFileCallable | None = None,
                  desc: str | None = None,
                  description: str | None = None) -> None:
         self.name = name
         self.desc = desc or name
         self.description = description
         self.encode: EncodeCallable = encode or _unimplemented_encode
         self.decode: DecodeCallable = decode or _unimplemented_decode
+        if decode_file:
+            self.decode_file = decode_file
+        else:
+            self.decode_file = self._decode_file
 
     def can_encode(self) -> bool:
         return self.encode != _unimplemented_encode
 
     def can_decode(self) -> bool:
         return self.decode != _unimplemented_decode
 
+    def _decode_file(self, n: VljuMap, p: Path,
+                     f: VljuFactory) -> DecodeFileResult:
+        self.decode(n, p.stem, f)
+        return DecodeFileResult(p.parent, p.stem, p.suffix)
+
 def _unimplemented_decode(_n: VljuMap, _s: str,
                           _factory: VljuFactory) -> VljuMap:
     raise NotImplementedError
 
 def _unimplemented_encode(_n: VljuMap, _mode: str | None = None) -> str:
     raise NotImplementedError
 
@@ -110,16 +129,26 @@
 
 def v3_encode(n: VljuMap, mode: str | None = None) -> str:
     return _v3_enc(V3_CONFIG, n, mode)
 
 def v3_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return _v3_dec(V3_CONFIG, n, s, factory)
 
+def v3_decode_file(n: VljuMap, p: Path,
+                   factory: VljuFactory) -> DecodeFileResult:
+    return _v3_dec_file(V3_CONFIG, n, p, factory)
+
 v3 = _register_encoder(
-    Encoder('v3', v3_encode, v3_decode, V3_DESC, V3_DESCRIPTION))
+    Encoder(
+        'v3',
+        v3_encode,
+        v3_decode,
+        v3_decode_file,
+        desc=V3_DESC,
+        description=V3_DESCRIPTION))
 
 def _v3_enc(config: V3Config, n: VljuMap, mode: str | None) -> str:
     m = n.to_strings(mode)
 
     sequence = config.seq_join.join(m['n'])
     sequence = sequence and f'{config.seq_start}{sequence}{config.seq_end}'
     title_qjoin = config.title_join.translate(
@@ -129,14 +158,28 @@
         for i in m['title'])
     attrs = config.attr_join.join(
         kv_fmt(k, v, config.attr_kv, config.quote) for k,
         v in m.pairs() if k not in ('title', 'n'))
     attrs = attrs and f'{config.attr_start}{attrs}{config.attr_end}'
     return join_non_empty(' ', sequence, title, attrs)
 
+def _v3_dec_file(config: V3Config, n: VljuMap, p: Path,
+                 factory: VljuFactory) -> DecodeFileResult:
+    bad_suffix = (
+        config.attr_end in p.suffix
+        and p.stem.count(config.attr_start) > p.stem.count(config.attr_end))
+    if bad_suffix:
+        stem = p.stem + p.suffix
+        suffix = ''
+    else:
+        stem = p.stem
+        suffix = p.suffix
+    _v3_dec(config, n, stem, factory)
+    return DecodeFileResult(p.parent, stem, suffix)
+
 def _v3_dec(config: V3Config, n: VljuMap, s: str,
             factory: VljuFactory) -> VljuMap:
     return n.add_pairs(_v3_dec_iter(config, s), factory)
 
 def _v3_dec_iter(config: V3Config, s: str) -> Iterable[tuple[str, str]]:
     if config.attr_start in s:
         s, _, attr = s.partition(config.attr_start)
@@ -210,16 +253,26 @@
 
 def win_encode(n: VljuMap, mode: str | None = None) -> str:
     return _v3_enc(WIN_CONFIG, n, mode)
 
 def win_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return _v3_dec(WIN_CONFIG, n, s, factory)
 
+def win_decode_file(n: VljuMap, p: Path,
+                    factory: VljuFactory) -> DecodeFileResult:
+    return _v3_dec_file(WIN_CONFIG, n, p, factory)
+
 win = _register_encoder(
-    Encoder('win', win_encode, win_decode, WIN_DESC, WIN_DESCRIPTION))
+    Encoder(
+        'win',
+        win_encode,
+        win_decode,
+        win_decode_file,
+        desc=WIN_DESC,
+        description=WIN_DESCRIPTION))
 
 ###############################################################################
 #
 # V2 Encoder
 #
 # Same as V3 except attributes are surrounded by ‘{}’ instead of ‘[]’
 # and joined by ‘;’ with no space.
@@ -249,16 +302,26 @@
 
 def v2_encode(n: VljuMap, mode: str | None = None) -> str:
     return _v3_enc(V2_CONFIG, n, mode)
 
 def v2_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return _v3_dec(V2_CONFIG, n, s, factory)
 
+def v2_decode_file(n: VljuMap, p: Path,
+                   factory: VljuFactory) -> DecodeFileResult:
+    return _v3_dec_file(V2_CONFIG, n, p, factory)
+
 v2 = _register_encoder(
-    Encoder('v2', v2_encode, v2_decode, V2_DESC, V2_DESCRIPTION))
+    Encoder(
+        'v2',
+        v2_encode,
+        v2_decode,
+        v2_decode_file,
+        desc=V2_DESC,
+        description=V2_DESCRIPTION))
 
 ###############################################################################
 #
 # V1 Encoder
 #
 ###############################################################################
 
@@ -298,15 +361,16 @@
         v in m.pairs() if k not in ('title', 'a'))
     return spj(r, f'[{attrs}]') if attrs else r
 
 def v1_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return n.add_pairs(_v1_dec_iter(V1_CONFIG, s), factory)
 
 v1 = _register_encoder(
-    Encoder('v1', v1_encode, v1_decode, V1_DESC, V1_DESCRIPTION))
+    Encoder(
+        'v1', v1_encode, v1_decode, desc=V1_DESC, description=V1_DESCRIPTION))
 
 def _v1_enc_author_title(m: MultiMap) -> str:
     author = '; '.join(i for i in m['a'])
     r = f'{author}:' if author else ''
     title = ': '.join(i for i in m['title'])
     return spj(r, title)
 
@@ -357,15 +421,16 @@
         return spj(r, f'lccn={m["lccn"][0]}')
     return r
 
 def v0_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return n.add_pairs(_v0_dec_iter(s), factory)
 
 v0 = _register_encoder(
-    Encoder('v0', v0_encode, v0_decode, V0_DESC, V0_DESCRIPTION))
+    Encoder(
+        'v0', v0_encode, v0_decode, desc=V0_DESC, description=V0_DESCRIPTION))
 
 V0_RE = re.compile(
     r"""
         (?P<rest>.*)
         \b(?:
             (?P<isbn> (?: [0-9]{13} | [0-9]{9}[0-9xX] ) )
         | lccn=(?P<lccn> \S+ )
@@ -429,15 +494,20 @@
     date = m['date'][0] if 'date' in m else ''
     return join_non_empty(' ', title, author, isbn, edition, date)
 
 def sfc_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return n.add_pairs(_sfc_dec_iter(s), factory)
 
 sfc = _register_encoder(
-    Encoder('sfc', sfc_encode, sfc_decode, SFC_DESC, SFC_DESCRIPTION))
+    Encoder(
+        'sfc',
+        sfc_encode,
+        sfc_decode,
+        desc=SFC_DESC,
+        description=SFC_DESCRIPTION))
 
 SFC_TAIL_RE = re.compile(
     r"""
         (?P<prefix> .*)
         (?:
             (?P<date> [12]\d\d\d ) |
             (?: (?P<edition> \d+ ) \w*\s+edition )
@@ -505,15 +575,20 @@
         if isinstance(vl, list):
             for v in vl:
                 yield (k, str(v))
         else:
             yield (k, str(vl))
 
 json = _register_encoder(
-    Encoder('json', json_encode, json_decode, JSON_DESC, JSON_DESCRIPTION))
+    Encoder(
+        'json',
+        json_encode,
+        json_decode,
+        desc=JSON_DESC,
+        description=JSON_DESCRIPTION))
 
 ###############################################################################
 #
 # Shell
 #
 ###############################################################################
 
@@ -528,19 +603,20 @@
     r = []
     for k, vlist in n.get_lists(mode):
         v = ' '.join(shlex.quote(v) for v in vlist if v is not None)
         r.append(f'{k}=({v})')
     return '\n'.join(r)
 
 sh = _register_encoder(
-    Encoder('sh',
-            shell_encode,
-            _unimplemented_decode,
-            SHELL_DESC,
-            SHELL_DESCRIPTION))
+    Encoder(
+        'sh',
+        shell_encode,
+        _unimplemented_decode,
+        desc=SHELL_DESC,
+        description=SHELL_DESCRIPTION))
 
 ###############################################################################
 #
 # value
 #
 ###############################################################################
 
@@ -551,19 +627,20 @@
   Since keys are not represented, decoding is not possible.
 """
 
 def value_encode(n: VljuMap, mode: str | None = None) -> str:
     return '\n'.join((f'{v or k}' for k, v in n.get_pairs(mode)))
 
 value = _register_encoder(
-    Encoder('value',
-            value_encode,
-            _unimplemented_decode,
-            VALUE_DESC,
-            VALUE_DESCRIPTION))
+    Encoder(
+        'value',
+        value_encode,
+        _unimplemented_decode,
+        desc=VALUE_DESC,
+        description=VALUE_DESCRIPTION))
 
 ###############################################################################
 #
 # key/value
 #
 ###############################################################################
 
@@ -584,19 +661,20 @@
 def _keyvalue_dec_iter(s: str) -> Generator[tuple[str, str], None, None]:
     for kv in s.split('\n'):
         if kv:
             k, v = kv.split(':', 1)
             yield (k.strip(), v.strip())
 
 keyvalue = _register_encoder(
-    Encoder('keyvalue',
-            keyvalue_encode,
-            keyvalue_decode,
-            KEYVALUE_DESC,
-            KEYVALUE_DESCRIPTION))
+    Encoder(
+        'keyvalue',
+        keyvalue_encode,
+        keyvalue_decode,
+        desc=KEYVALUE_DESC,
+        description=KEYVALUE_DESCRIPTION))
 
 ###############################################################################
 #
 # csv
 #
 ###############################################################################
 
@@ -610,15 +688,20 @@
 def csv_encode(n: VljuMap, mode: str | None = None) -> str:
     return _csv_enc(n, mode, dialect='unix')
 
 def csv_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return n.add_pairs(_csv_dec_iter(s, dialect='unix'), factory)
 
 csv = _register_encoder(
-    Encoder('csv', csv_encode, csv_decode, CSV_DESC, CSV_DESCRIPTION))
+    Encoder(
+        'csv',
+        csv_encode,
+        csv_decode,
+        desc=CSV_DESC,
+        description=CSV_DESCRIPTION))
 
 def _csv_enc(n: VljuMap, mode: str | None, **kwargs) -> str:
     with io.StringIO() as f:
         w = py_csv.writer(f, **kwargs)
         for kv in n.get_pairs(mode):
             w.writerow(kv)
         return f.getvalue()
```

### Comparing `fnattr-0.2.6/src/fnattr/vljumap/factory.py` & `fnattr-0.2.7/src/fnattr/vljumap/factory.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.6/src/fnattr.egg-info/PKG-INFO` & `fnattr-0.2.7/src/fnattr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnattr
-Version: 0.2.6
+Version: 0.2.7
 Summary: Manage key/value metadata in file names.
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/fna
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -97,22 +97,22 @@
 $ fna file '/tmp/My Book.pdf' add isbn 1234567890 json encode
 {"title": ["My Book"], "isbn": ["9781234567897"]}
 ```
 
 ## Configuration
 
 Unless otherwise directed by a command line option,
-`fna` tries to read `vlju/config.toml` or `fna/config.toml`
+`fna` tries to read `fnattr/vlju.toml` or `fnattr/fna.toml`
 from XDG locations (e.g. `$HOME/.config/`).
 The former is shared by all tools using the Vlju
 library, while the latter applies only to the `fna` command.
 
 This file can define keys and classes associated with web sites,
-mapping from a compact ID to a URL. (The other direction does not yet exist.)
-The distribution file `config/config.toml` contains some examples.
+mapping between a compact ID to a URL.
+The distribution file `config/vlju.toml` contains some examples.
 
 See [doc/configuration.md](doc/configuration.md) for more information.
 
 ## Implementation
 
 The current public home for `fna` is
 [https://codeberg.org/datatravelandexperiments/fna](https://codeberg.org/datatravelandexperiments/fna)
@@ -158,8 +158,7 @@
 
 The command line tool `fna`.
 
 ### TODO
 
 - Better error handling. Too much still just raises exceptions.
 - Document operation with `-[EFx]`.
-- Logging options?
```

### Comparing `fnattr-0.2.6/src/fnattr.egg-info/SOURCES.txt` & `fnattr-0.2.7/src/fnattr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-config/config.toml
+config/vlju.toml
 doc/configuration.md
 doc/fna.md
 doc/keys.md
 src/fnattr.egg-info/PKG-INFO
 src/fnattr.egg-info/SOURCES.txt
 src/fnattr.egg-info/dependency_links.txt
 src/fnattr.egg-info/entry_points.txt
```

