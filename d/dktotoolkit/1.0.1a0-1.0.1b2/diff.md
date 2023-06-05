# Comparing `tmp/dktotoolkit-1.0.1a0.tar.gz` & `tmp/dktotoolkit-1.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dktotoolkit-1.0.1a0.tar", last modified: Thu Jun  1 18:24:48 2023, max compression
+gzip compressed data, was "dktotoolkit-1.0.1b2.tar", last modified: Fri Jun  2 12:29:18 2023, max compression
```

## Comparing `dktotoolkit-1.0.1a0.tar` & `dktotoolkit-1.0.1b2.tar`

### file list

```diff
@@ -1,21 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:24:48.394357 dktotoolkit-1.0.1a0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)      699 2023-06-01 18:24:48.394357 dktotoolkit-1.0.1a0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:24:48.394357 dktotoolkit-1.0.1a0/dktotoolkit/
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     5985 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/datestr.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/dict.py
--rw-rw-rw-   0 root         (0) root         (0)     2035 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/dotenv2clock.py
--rw-rw-rw-   0 root         (0) root         (0)     4138 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/envvar.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:24:48.394357 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      699 2023-06-01 18:24:48.000000 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2023-06-01 18:24:48.000000 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:24:48.000000 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-01 18:24:48.000000 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-01 18:24:48.000000 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      570 2023-06-01 18:24:48.394357 dktotoolkit-1.0.1a0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/setup.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-02 12:29:18.603287 dktotoolkit-1.0.1b2/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2071 2023-06-02 12:29:18.603287 dktotoolkit-1.0.1b2/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1286 2023-06-02 11:45:29.000000 dktotoolkit-1.0.1b2/README.md
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-02 12:29:18.603287 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2071 2023-06-02 12:29:18.000000 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      202 2023-06-02 12:29:18.000000 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-06-02 12:29:18.000000 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       64 2023-06-02 12:29:18.000000 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-06-02 12:29:18.000000 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/top_level.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      195 2023-06-02 12:29:18.603287 dktotoolkit-1.0.1b2/setup.cfg
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3493 2023-06-02 12:18:24.000000 dktotoolkit-1.0.1b2/setup.py
```

