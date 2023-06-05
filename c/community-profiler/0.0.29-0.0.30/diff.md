# Comparing `tmp/community-profiler-0.0.29.tar.gz` & `tmp/community-profiler-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "community-profiler-0.0.29.tar", last modified: Mon Jun  5 01:29:03 2023, max compression
+gzip compressed data, was "community-profiler-0.0.30.tar", last modified: Mon Jun  5 01:32:31 2023, max compression
```

## Comparing `community-profiler-0.0.29.tar` & `community-profiler-0.0.30.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-06-05 01:29:03.271441 community-profiler-0.0.29/
--rw-r--r--   0 tanl       (501) staff       (20)      627 2023-06-05 01:29:03.271507 community-profiler-0.0.29/PKG-INFO
--rw-r--r--   0 tanl       (501) staff       (20)       21 2023-06-05 01:26:49.000000 community-profiler-0.0.29/README.md
--rw-r--r--   0 tanl       (501) staff       (20)       91 2023-06-05 01:27:57.000000 community-profiler-0.0.29/pyproject.toml
--rw-r--r--   0 tanl       (501) staff       (20)      999 2023-06-05 01:29:03.271818 community-profiler-0.0.29/setup.cfg
-drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-06-05 01:29:03.269413 community-profiler-0.0.29/src/
-drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-06-05 01:29:03.270291 community-profiler-0.0.29/src/community_profiler/
--rw-r--r--   0 tanl       (501) staff       (20)       38 2023-06-05 01:26:49.000000 community-profiler-0.0.29/src/community_profiler/__init__.py
--rw-r--r--   0 tanl       (501) staff       (20)      292 2023-06-05 01:26:49.000000 community-profiler-0.0.29/src/community_profiler/cli.py
--rw-r--r--   0 tanl       (501) staff       (20)        0 2023-06-05 01:26:49.000000 community-profiler-0.0.29/src/community_profiler/profiler.py
--rw-r--r--   0 tanl       (501) staff       (20)        0 2023-06-05 01:26:49.000000 community-profiler-0.0.29/src/community_profiler/util.py
-drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-06-05 01:29:03.271294 community-profiler-0.0.29/src/community_profiler.egg-info/
--rw-r--r--   0 tanl       (501) staff       (20)      627 2023-06-05 01:29:03.000000 community-profiler-0.0.29/src/community_profiler.egg-info/PKG-INFO
--rw-r--r--   0 tanl       (501) staff       (20)      443 2023-06-05 01:29:03.000000 community-profiler-0.0.29/src/community_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 tanl       (501) staff       (20)        1 2023-06-05 01:29:03.000000 community-profiler-0.0.29/src/community_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 tanl       (501) staff       (20)       62 2023-06-05 01:29:03.000000 community-profiler-0.0.29/src/community_profiler.egg-info/entry_points.txt
--rw-r--r--   0 tanl       (501) staff       (20)      125 2023-06-05 01:29:03.000000 community-profiler-0.0.29/src/community_profiler.egg-info/requires.txt
--rw-r--r--   0 tanl       (501) staff       (20)       19 2023-06-05 01:29:03.000000 community-profiler-0.0.29/src/community_profiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 01:32:31.913393 community-profiler-0.0.30/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-05 01:32:09.000000 community-profiler-0.0.30/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-05 01:32:31.913393 community-profiler-0.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 01:32:09.000000 community-profiler-0.0.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 01:32:09.000000 community-profiler-0.0.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-05 01:32:31.913393 community-profiler-0.0.30/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 01:32:31.909393 community-profiler-0.0.30/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 01:32:31.913393 community-profiler-0.0.30/src/community_profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 01:32:09.000000 community-profiler-0.0.30/src/community_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-05 01:32:09.000000 community-profiler-0.0.30/src/community_profiler/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 01:32:09.000000 community-profiler-0.0.30/src/community_profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 01:32:09.000000 community-profiler-0.0.30/src/community_profiler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 01:32:31.913393 community-profiler-0.0.30/src/community_profiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-05 01:32:31.000000 community-profiler-0.0.30/src/community_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-05 01:32:31.000000 community-profiler-0.0.30/src/community_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 01:32:31.000000 community-profiler-0.0.30/src/community_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 01:32:31.000000 community-profiler-0.0.30/src/community_profiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 01:32:31.000000 community-profiler-0.0.30/src/community_profiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 01:32:31.000000 community-profiler-0.0.30/src/community_profiler.egg-info/top_level.txt
```

### Comparing `community-profiler-0.0.29/setup.cfg` & `community-profiler-0.0.30/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = community-profiler
-version = 0.0.29
+version = 0.0.1
 author = Tan Li
 author_email = tan@tanli.dev
 description = Github community profiler
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/litanlitudan/skyagi/tree/main/community-profiler
 project_urls =
```

