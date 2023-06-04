# Comparing `tmp/lambda_zip-1.23011102.tar.gz` & `tmp/lambda_zip-1.23060401.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jsw/src/lambda_zipper/dist/.tmp-bhr4wrrd/lambda_zip-1.23011102.tar", last modified: Wed Jan 11 12:50:17 2023, max compression
+gzip compressed data, was "/Users/jsw/src/lambda_zipper/dist/.tmp-uxhdlh3_/lambda_zip-1.23060401.tar", last modified: Sun Jun  4 23:09:22 2023, max compression
```

## Comparing `lambda_zip-1.23011102.tar` & `lambda_zip-1.23060401.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 jsw        (501) staff       (20)        0 2023-01-11 12:50:17.608637 lambda_zip-1.23011102/
--rw-r--r--   0 jsw        (501) staff       (20)     1070 2022-01-27 11:21:43.000000 lambda_zip-1.23011102/LICENSE
--rw-r--r--   0 jsw        (501) staff       (20)      251 2023-01-11 12:50:17.608339 lambda_zip-1.23011102/PKG-INFO
--rw-r--r--   0 jsw        (501) staff       (20)     4218 2022-01-27 11:05:08.000000 lambda_zip-1.23011102/README.md
-drwxr-xr-x   0 jsw        (501) staff       (20)        0 2023-01-11 12:50:17.606114 lambda_zip-1.23011102/lambda_zip/
--rw-r--r--   0 jsw        (501) staff       (20)    10490 2023-01-11 12:48:13.000000 lambda_zip-1.23011102/lambda_zip/__init__.py
-drwxr-xr-x   0 jsw        (501) staff       (20)        0 2023-01-11 12:50:17.607963 lambda_zip-1.23011102/lambda_zip.egg-info/
--rw-r--r--   0 jsw        (501) staff       (20)      251 2023-01-11 12:50:17.000000 lambda_zip-1.23011102/lambda_zip.egg-info/PKG-INFO
--rw-r--r--   0 jsw        (501) staff       (20)      270 2023-01-11 12:50:17.000000 lambda_zip-1.23011102/lambda_zip.egg-info/SOURCES.txt
--rw-r--r--   0 jsw        (501) staff       (20)        1 2023-01-11 12:50:17.000000 lambda_zip-1.23011102/lambda_zip.egg-info/dependency_links.txt
--rw-r--r--   0 jsw        (501) staff       (20)       58 2023-01-11 12:50:17.000000 lambda_zip-1.23011102/lambda_zip.egg-info/entry_points.txt
--rw-r--r--   0 jsw        (501) staff       (20)       21 2023-01-11 12:50:17.000000 lambda_zip-1.23011102/lambda_zip.egg-info/requires.txt
--rw-r--r--   0 jsw        (501) staff       (20)       11 2023-01-11 12:50:17.000000 lambda_zip-1.23011102/lambda_zip.egg-info/top_level.txt
--rw-r--r--   0 jsw        (501) staff       (20)       90 2021-11-21 17:38:52.000000 lambda_zip-1.23011102/pyproject.toml
--rw-r--r--   0 jsw        (501) staff       (20)       38 2023-01-11 12:50:17.608729 lambda_zip-1.23011102/setup.cfg
--rw-r--r--   0 jsw        (501) staff       (20)      523 2023-01-11 12:49:55.000000 lambda_zip-1.23011102/setup.py
+drwxr-xr-x   0 jsw        (501) staff       (20)        0 2023-06-04 23:09:22.960961 lambda_zip-1.23060401/
+-rw-r--r--   0 jsw        (501) staff       (20)     1070 2022-01-27 11:21:43.000000 lambda_zip-1.23060401/LICENSE
+-rw-r--r--   0 jsw        (501) staff       (20)      251 2023-06-04 23:09:22.960205 lambda_zip-1.23060401/PKG-INFO
+-rw-r--r--   0 jsw        (501) staff       (20)     7366 2023-04-30 19:38:34.000000 lambda_zip-1.23060401/README.md
+drwxr-xr-x   0 jsw        (501) staff       (20)        0 2023-06-04 23:09:22.955343 lambda_zip-1.23060401/lambda_zip/
+-rw-r--r--   0 jsw        (501) staff       (20)    28519 2023-06-04 21:25:35.000000 lambda_zip-1.23060401/lambda_zip/__init__.py
+-rw-r--r--   0 jsw        (501) staff       (20)     1018 2023-04-29 21:33:09.000000 lambda_zip-1.23060401/lambda_zip/aws_lambda_function.py
+-rw-r--r--   0 jsw        (501) staff       (20)     3403 2023-06-03 23:31:09.000000 lambda_zip-1.23060401/lambda_zip/aws_lambda_layer.py
+-rw-r--r--   0 jsw        (501) staff       (20)     3616 2023-06-04 11:42:44.000000 lambda_zip-1.23060401/lambda_zip/aws_lambda_layer_version.py
+drwxr-xr-x   0 jsw        (501) staff       (20)        0 2023-06-04 23:09:22.959097 lambda_zip-1.23060401/lambda_zip.egg-info/
+-rw-r--r--   0 jsw        (501) staff       (20)      251 2023-06-04 23:09:22.000000 lambda_zip-1.23060401/lambda_zip.egg-info/PKG-INFO
+-rw-r--r--   0 jsw        (501) staff       (20)      374 2023-06-04 23:09:22.000000 lambda_zip-1.23060401/lambda_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 jsw        (501) staff       (20)        1 2023-06-04 23:09:22.000000 lambda_zip-1.23060401/lambda_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 jsw        (501) staff       (20)       58 2023-06-04 23:09:22.000000 lambda_zip-1.23060401/lambda_zip.egg-info/entry_points.txt
+-rw-r--r--   0 jsw        (501) staff       (20)       38 2023-06-04 23:09:22.000000 lambda_zip-1.23060401/lambda_zip.egg-info/requires.txt
+-rw-r--r--   0 jsw        (501) staff       (20)       11 2023-06-04 23:09:22.000000 lambda_zip-1.23060401/lambda_zip.egg-info/top_level.txt
+-rw-r--r--   0 jsw        (501) staff       (20)       90 2021-11-21 17:38:52.000000 lambda_zip-1.23060401/pyproject.toml
+-rw-r--r--   0 jsw        (501) staff       (20)       38 2023-06-04 23:09:22.961184 lambda_zip-1.23060401/setup.cfg
+-rw-r--r--   0 jsw        (501) staff       (20)      592 2023-06-04 23:01:13.000000 lambda_zip-1.23060401/setup.py
```

### Comparing `lambda_zip-1.23011102/LICENSE` & `lambda_zip-1.23060401/LICENSE`

 * *Files identical despite different names*

