# Comparing `tmp/gen3_util-0.0.2rc1.tar.gz` & `tmp/gen3_util-0.0.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.2rc1.tar", last modified: Fri May 12 13:39:40 2023, max compression
+gzip compressed data, was "gen3_util-0.0.2rc2.tar", last modified: Mon Jun  5 20:44:26 2023, max compression
```

## Comparing `gen3_util-0.0.2rc1.tar` & `gen3_util-0.0.2rc2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.906822 gen3_util-0.0.2rc1/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc1/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     8996 2023-05-12 13:39:40.906468 gen3_util-0.0.2rc1/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     8311 2023-05-12 13:39:21.000000 gen3_util-0.0.2rc1/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.860794 gen3_util-0.0.2rc1/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.868334 gen3_util-0.0.2rc1/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1819 2023-05-12 00:08:03.000000 gen3_util-0.0.2rc1/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1948 2023-05-12 00:08:03.000000 gen3_util-0.0.2rc1/gen3_util/access/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1869 2023-05-11 17:49:58.000000 gen3_util-0.0.2rc1/gen3_util/access/requestor.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.875286 gen3_util-0.0.2rc1/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      628 2023-05-12 12:59:15.000000 gen3_util-0.0.2rc1/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.878738 gen3_util-0.0.2rc1/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142     3932 2023-05-11 00:12:51.000000 gen3_util-0.0.2rc1/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-05-10 23:46:59.000000 gen3_util-0.0.2rc1/gen3_util/cli/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.880004 gen3_util-0.0.2rc1/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4102 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.885279 gen3_util-0.0.2rc1/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2425 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      485 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.889141 gen3_util-0.0.2rc1/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1270 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-05-12 13:00:59.000000 gen3_util-0.0.2rc1/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      920 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    13289 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.900799 gen3_util-0.0.2rc1/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4117 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1291 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      210 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5483 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      191 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      208 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3248 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.902047 gen3_util-0.0.2rc1/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142      329 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1152 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      204 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      553 2023-05-12 13:11:53.000000 gen3_util-0.0.2rc1/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      207 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.866330 gen3_util-0.0.2rc1/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     8996 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1502 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-05-12 13:39:40.906894 gen3_util-0.0.2rc1/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5580 2023-05-12 13:37:11.000000 gen3_util-0.0.2rc1/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.857640 gen3_util-0.0.2rc1/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.903804 gen3_util-0.0.2rc1/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      108 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2941 2023-05-12 13:32:44.000000 gen3_util-0.0.2rc1/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2047 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/integration/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1225 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.906114 gen3_util-0.0.2rc1/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/unit/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3222 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      867 2023-05-11 22:42:33.000000 gen3_util-0.0.2rc1/tests/unit/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/unit/test_validate_directory.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.632985 gen3_util-0.0.2rc2/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc2/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-05 20:44:26.632799 gen3_util-0.0.2rc2/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6374 2023-05-25 21:06:12.000000 gen3_util-0.0.2rc2/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.589522 gen3_util-0.0.2rc2/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.597962 gen3_util-0.0.2rc2/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1819 2023-05-12 00:08:03.000000 gen3_util-0.0.2rc2/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1948 2023-05-12 00:08:03.000000 gen3_util-0.0.2rc2/gen3_util/access/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1869 2023-05-11 17:49:58.000000 gen3_util-0.0.2rc2/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.603402 gen3_util-0.0.2rc2/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      628 2023-05-12 12:59:15.000000 gen3_util-0.0.2rc2/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.604403 gen3_util-0.0.2rc2/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4355 2023-06-01 15:53:03.000000 gen3_util-0.0.2rc2/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-05-10 23:46:59.000000 gen3_util-0.0.2rc2/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.604880 gen3_util-0.0.2rc2/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4119 2023-06-01 15:00:31.000000 gen3_util-0.0.2rc2/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.606081 gen3_util-0.0.2rc2/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2425 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      485 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.624043 gen3_util-0.0.2rc2/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1270 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-05-12 13:00:59.000000 gen3_util-0.0.2rc2/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      920 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13289 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.627087 gen3_util-0.0.2rc2/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4117 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1291 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      210 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5483 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      191 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      208 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3248 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.628677 gen3_util-0.0.2rc2/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-01 15:31:29.000000 gen3_util-0.0.2rc2/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1660 2023-06-01 15:39:25.000000 gen3_util-0.0.2rc2/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1888 2023-06-01 14:31:34.000000 gen3_util-0.0.2rc2/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1112 2023-06-01 15:38:13.000000 gen3_util-0.0.2rc2/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1040 2023-06-01 14:31:34.000000 gen3_util-0.0.2rc2/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.596214 gen3_util-0.0.2rc2/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1502 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-06-05 20:44:26.000000 gen3_util-0.0.2rc2/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-06-05 20:44:26.633035 gen3_util-0.0.2rc2/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5580 2023-06-05 20:44:08.000000 gen3_util-0.0.2rc2/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.586303 gen3_util-0.0.2rc2/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.630462 gen3_util-0.0.2rc2/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      108 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2941 2023-05-12 13:32:44.000000 gen3_util-0.0.2rc2/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2047 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1225 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-05 20:44:26.632492 gen3_util-0.0.2rc2/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/unit/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3222 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc2/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      867 2023-05-11 22:42:33.000000 gen3_util-0.0.2rc2/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc2/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.2rc1/LICENSE` & `gen3_util-0.0.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/PKG-INFO` & `gen3_util-0.0.2rc2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_util
-Version: 0.0.2rc1
+Version: 0.0.2rc2
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
@@ -214,31 +214,15 @@
 
 * running tests
 
 ```
 
 $ pytest --cov=gen3_util
 
-collected 26 items
-
-tests/integration/test_access.py ..                                                                                                                                           [  7%]
-tests/integration/test_buckets.py .                                                                                                                                           [ 11%]
-tests/integration/test_files.py ..                                                                                                                                            [ 19%]
-tests/integration/test_project.py ...                                                                                                                                         [ 30%]
-tests/unit/test_cli.py .......                                                                                                                                                [ 57%]
-tests/unit/test_coding_conventions.py .                                                                                                                                       [ 61%]
-tests/unit/test_config.py ..                                                                                                                                                  [ 69%]
-tests/unit/test_files.py ...                                                                                                                                                  [ 80%]
-tests/unit/test_meta.py .                                                                                                                                                     [ 84%]
-tests/unit/test_validate_directory.py ....                                                                                                                                    [100%]
-...
-----------------------------------------------------
-TOTAL                              944    114    88%
-
-
+ 88%
 
 
 ```
 
 * pre commit tests
 
 A reasonable set of checks, including running unit tests prior to each commit.  You can run these tests on demand by:
```

### Comparing `gen3_util-0.0.2rc1/README.md` & `gen3_util-0.0.2rc2/gen3_util.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: gen3-util
+Version: 0.0.2rc2
+Summary: Commons utilities
+Home-page: https://github.com/ACED-IDP/gen3_util
+Author: Ellrott Lab
+License: UNKNOWN
+Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
+Project-URL: Source, https://github.com/ACED-IDP/gen3_util
+Keywords: gen3 bioinformatics
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # Gen3 Utilities
 
 Utilities to manage Gen3 schemas, projects and submissions.
 
 ## Installation
 
@@ -194,31 +214,15 @@
 
 * running tests
 
 ```
 
 $ pytest --cov=gen3_util
 
-collected 26 items
-
-tests/integration/test_access.py ..                                                                                                                                           [  7%]
-tests/integration/test_buckets.py .                                                                                                                                           [ 11%]
-tests/integration/test_files.py ..                                                                                                                                            [ 19%]
-tests/integration/test_project.py ...                                                                                                                                         [ 30%]
-tests/unit/test_cli.py .......                                                                                                                                                [ 57%]
-tests/unit/test_coding_conventions.py .                                                                                                                                       [ 61%]
-tests/unit/test_config.py ..                                                                                                                                                  [ 69%]
-tests/unit/test_files.py ...                                                                                                                                                  [ 80%]
-tests/unit/test_meta.py .                                                                                                                                                     [ 84%]
-tests/unit/test_validate_directory.py ....                                                                                                                                    [100%]
-...
-----------------------------------------------------
-TOTAL                              944    114    88%
-
-
+ 88%
 
 
 ```
 
 * pre commit tests
 
 A reasonable set of checks, including running unit tests prior to each commit.  You can run these tests on demand by:
@@ -257,7 +261,9 @@
 
 # this could be maintained as so: export $(cat .env | xargs)
 
 rm -r dist/
 python3  setup.py sdist bdist_wheel
 twine upload dist/*
 ```
+
+
```

### Comparing `gen3_util-0.0.2rc1/gen3_util/access/__init__.py` & `gen3_util-0.0.2rc2/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/access/cli.py` & `gen3_util-0.0.2rc2/gen3_util/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/access/requestor.py` & `gen3_util-0.0.2rc2/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/buckets/__init__.py` & `gen3_util-0.0.2rc2/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/buckets/cli.py` & `gen3_util-0.0.2rc2/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/cli/__init__.py` & `gen3_util-0.0.2rc2/gen3_util/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,31 +76,48 @@
         _common_options(self)
 
     def list_commands(self, ctx):
         """Commands in order of appearance"""
         return self.commands.keys()
 
 
+class CommandOutput(object):
+    """Output object for commands."""
+    def __init__(self):
+        self.obj = None
+
+    def update(self, obj):
+        """Update output with obj."""
+        self.obj = obj
+
+
 class CLIOutput:
     """Ensure output, exceptions and exit code are returned to user consistently."""
     def __init__(self, config: Config):
-        self.output = {}
+        self.output = CommandOutput()
         self.config = config
 
     def __enter__(self):
         return self.output
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         rc = 0
         _ = {}
-        _.update(self.output)
+        if self.output.obj is not None:
+            _.update(self.output.obj.dict())
         if exc_type is not None:
             _['exception'] = f"{str(exc_val)}"
             rc = 1
             logging.getLogger(__name__).exception(exc_val)
         if 'msg' not in _:
             if rc == 1:
                 _['msg'] = 'FAIL'
             else:
                 _['msg'] = 'OK'
+        prune = []
+        for k, v in _.items():
+            if not v:
+                prune.append(k)
+        for k in prune:
+            del _[k]
         print_formatted(self.config, _)
         exit(rc)
```

### Comparing `gen3_util-0.0.2rc1/gen3_util/cli/cli.py` & `gen3_util-0.0.2rc2/gen3_util/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/common/__init__.py` & `gen3_util-0.0.2rc2/gen3_util/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from gen3_util.config import Config
 
 
 def print_formatted(config: Config, output: Mapping) -> None:
     """Print the output, using configured output format"""
 
     if config.output.format == "yaml":
-        print(yaml.dump(output))
+        print(yaml.dump(output, sort_keys=False))
     elif config.output.format == "json":
         print(
             orjson.dumps(
                 output, default=pydantic_encoder, option=orjson.OPT_INDENT_2
             ).decode()
         )
     else:
```

### Comparing `gen3_util-0.0.2rc1/gen3_util/config/__init__.py` & `gen3_util-0.0.2rc2/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/files/__init__.py` & `gen3_util-0.0.2rc2/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/files/cli.py` & `gen3_util-0.0.2rc2/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/files/downloader.py` & `gen3_util-0.0.2rc2/gen3_util/files/downloader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/files/uploader.py` & `gen3_util-0.0.2rc2/gen3_util/files/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/meta/__init__.py` & `gen3_util-0.0.2rc2/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/meta/cli.py` & `gen3_util-0.0.2rc2/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/meta/importer.py` & `gen3_util-0.0.2rc2/gen3_util/meta/importer.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util/meta/validator.py` & `gen3_util-0.0.2rc2/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/gen3_util.egg-info/SOURCES.txt` & `gen3_util-0.0.2rc2/gen3_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/setup.py` & `gen3_util-0.0.2rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2-rc1',  # Required
+    version='0.0.2-rc2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.2rc1/tests/integration/test_access.py` & `gen3_util-0.0.2rc2/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/tests/integration/test_files.py` & `gen3_util-0.0.2rc2/tests/integration/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/tests/integration/test_project.py` & `gen3_util-0.0.2rc2/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/tests/unit/test_cli.py` & `gen3_util-0.0.2rc2/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.2rc2/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/tests/unit/test_config.py` & `gen3_util-0.0.2rc2/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/tests/unit/test_files.py` & `gen3_util-0.0.2rc2/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/tests/unit/test_meta.py` & `gen3_util-0.0.2rc2/tests/unit/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc1/tests/unit/test_validate_directory.py` & `gen3_util-0.0.2rc2/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

