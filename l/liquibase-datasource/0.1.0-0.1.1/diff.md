# Comparing `tmp/liquibase-datasource-0.1.0.tar.gz` & `tmp/liquibase-datasource-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liquibase-datasource-0.1.0.tar", last modified: Mon Jun  5 12:26:37 2023, max compression
+gzip compressed data, was "liquibase-datasource-0.1.1.tar", last modified: Mon Jun  5 12:48:41 2023, max compression
```

## Comparing `liquibase-datasource-0.1.0.tar` & `liquibase-datasource-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-05 12:26:37.778737 liquibase-datasource-0.1.0/
--rw-r--r--   0 jiyi       (501) staff       (20)      267 2023-06-05 12:26:37.778575 liquibase-datasource-0.1.0/PKG-INFO
-drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-05 12:26:37.778401 liquibase-datasource-0.1.0/liquibase_datasource.egg-info/
--rw-r--r--   0 jiyi       (501) staff       (20)      267 2023-06-05 12:26:37.000000 liquibase-datasource-0.1.0/liquibase_datasource.egg-info/PKG-INFO
--rw-r--r--   0 jiyi       (501) staff       (20)      227 2023-06-05 12:26:37.000000 liquibase-datasource-0.1.0/liquibase_datasource.egg-info/SOURCES.txt
--rw-r--r--   0 jiyi       (501) staff       (20)        1 2023-06-05 12:26:37.000000 liquibase-datasource-0.1.0/liquibase_datasource.egg-info/dependency_links.txt
--rw-r--r--   0 jiyi       (501) staff       (20)       23 2023-06-05 12:26:37.000000 liquibase-datasource-0.1.0/liquibase_datasource.egg-info/requires.txt
--rw-r--r--   0 jiyi       (501) staff       (20)        1 2023-06-05 12:26:37.000000 liquibase-datasource-0.1.0/liquibase_datasource.egg-info/top_level.txt
--rw-r--r--   0 jiyi       (501) staff       (20)       38 2023-06-05 12:26:37.778784 liquibase-datasource-0.1.0/setup.cfg
--rw-r--r--   0 jiyi       (501) staff       (20)      441 2023-06-05 12:13:27.000000 liquibase-datasource-0.1.0/setup.py
+drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-05 12:48:41.303323 liquibase-datasource-0.1.1/
+-rw-r--r--   0 jiyi       (501) staff       (20)      267 2023-06-05 12:48:41.303161 liquibase-datasource-0.1.1/PKG-INFO
+drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-05 12:48:41.302960 liquibase-datasource-0.1.1/liquibase_datasource.egg-info/
+-rw-r--r--   0 jiyi       (501) staff       (20)      267 2023-06-05 12:48:41.000000 liquibase-datasource-0.1.1/liquibase_datasource.egg-info/PKG-INFO
+-rw-r--r--   0 jiyi       (501) staff       (20)      227 2023-06-05 12:48:41.000000 liquibase-datasource-0.1.1/liquibase_datasource.egg-info/SOURCES.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)        1 2023-06-05 12:48:41.000000 liquibase-datasource-0.1.1/liquibase_datasource.egg-info/dependency_links.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)       50 2023-06-05 12:48:41.000000 liquibase-datasource-0.1.1/liquibase_datasource.egg-info/requires.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)        1 2023-06-05 12:48:41.000000 liquibase-datasource-0.1.1/liquibase_datasource.egg-info/top_level.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)       38 2023-06-05 12:48:41.303371 liquibase-datasource-0.1.1/setup.cfg
+-rw-r--r--   0 jiyi       (501) staff       (20)      490 2023-06-05 12:46:07.000000 liquibase-datasource-0.1.1/setup.py
```

