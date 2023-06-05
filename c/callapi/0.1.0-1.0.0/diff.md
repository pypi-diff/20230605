# Comparing `tmp/callapi-0.1.0.tar.gz` & `tmp/callapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\callapi-0.1.0.tar", last modified: Sun Jun  4 17:01:47 2023, max compression
+gzip compressed data, was "dist\callapi-1.0.0.tar", last modified: Mon Jun  5 08:19:00 2023, max compression
```

## Comparing `callapi-0.1.0.tar` & `callapi-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:01:47.993466 callapi-0.1.0/
--rw-rw-rw-   0        0        0      213 2023-06-04 17:01:47.992468 callapi-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 17:01:47.974741 callapi-0.1.0/callapi/
--rw-rw-rw-   0        0        0       55 2023-06-04 16:59:19.000000 callapi-0.1.0/callapi/__init.py
--rw-rw-rw-   0        0        0      130 2023-06-04 16:59:18.000000 callapi-0.1.0/callapi/callapi.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:01:47.991468 callapi-0.1.0/callapi.egg-info/
--rw-rw-rw-   0        0        0      213 2023-06-04 17:01:47.000000 callapi-0.1.0/callapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-06-04 17:01:47.000000 callapi-0.1.0/callapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:01:47.000000 callapi-0.1.0/callapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-04 17:01:47.000000 callapi-0.1.0/callapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-04 17:01:47.000000 callapi-0.1.0/callapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:01:47.993466 callapi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      216 2023-06-04 16:59:18.000000 callapi-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:19:00.822038 callapi-1.0.0/
+-rw-rw-rw-   0        0        0      292 2023-06-05 08:19:00.821040 callapi-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 08:19:00.819046 callapi-1.0.0/callapi.egg-info/
+-rw-rw-rw-   0        0        0      292 2023-06-05 08:19:00.000000 callapi-1.0.0/callapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-06-05 08:19:00.000000 callapi-1.0.0/callapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 08:19:00.000000 callapi-1.0.0/callapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 08:19:00.000000 callapi-1.0.0/callapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 08:19:00.000000 callapi-1.0.0/callapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 08:19:00.822038 callapi-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      369 2023-06-05 08:16:36.000000 callapi-1.0.0/setup.py
```

