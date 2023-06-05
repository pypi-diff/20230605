# Comparing `tmp/ANBUtils-1.5.1.tar.gz` & `tmp/ANBUtils-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ANBUtils-1.5.1.tar", last modified: Mon Jun  5 13:00:07 2023, max compression
+gzip compressed data, was "dist/ANBUtils-1.5.2.tar", last modified: Mon Jun  5 18:31:50 2023, max compression
```

## Comparing `ANBUtils-1.5.1.tar` & `ANBUtils-1.5.2.tar`

### file list

```diff
@@ -1,10 +1,19 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-05 13:00:07.075465 ANBUtils-1.5.1/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-05 13:00:07.075084 ANBUtils-1.5.1/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)      123 2023-06-05 13:00:07.000000 ANBUtils-1.5.1/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      167 2023-06-05 13:00:07.000000 ANBUtils-1.5.1/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-05 13:00:07.000000 ANBUtils-1.5.1/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-05 13:00:07.000000 ANBUtils-1.5.1/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-05 13:00:07.000000 ANBUtils-1.5.1/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)      123 2023-06-05 13:00:07.075289 ANBUtils-1.5.1/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-05 13:00:07.075527 ANBUtils-1.5.1/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      405 2023-06-05 12:58:59.000000 ANBUtils-1.5.1/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-05 18:31:50.858740 ANBUtils-1.5.2/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-05 18:31:50.856636 ANBUtils-1.5.2/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)      860 2023-06-05 18:30:11.000000 ANBUtils-1.5.2/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     2483 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)     5637 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/db_worker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      478 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)      236 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/environ_cheker.py
+-rw-r--r--   0 redbson    (501) staff       (20)     2050 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)      667 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/messager.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1626 2023-06-05 18:09:00.000000 ANBUtils-1.5.2/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-05 18:31:50.858099 ANBUtils-1.5.2/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)      215 2023-06-05 18:31:50.000000 ANBUtils-1.5.2/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      333 2023-06-05 18:31:50.000000 ANBUtils-1.5.2/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-05 18:31:50.000000 ANBUtils-1.5.2/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-05 18:31:50.000000 ANBUtils-1.5.2/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-05 18:31:50.000000 ANBUtils-1.5.2/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)      215 2023-06-05 18:31:50.858528 ANBUtils-1.5.2/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-05 18:31:50.858835 ANBUtils-1.5.2/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      405 2023-06-05 18:30:16.000000 ANBUtils-1.5.2/setup.py
```

