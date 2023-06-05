# Comparing `tmp/zachet-0.0.1.tar.gz` & `tmp/zachet-0.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zachet-0.0.1.tar", last modified: Mon Jun  5 15:48:13 2023, max compression
+gzip compressed data, was "zachet-0.0.10.tar", last modified: Mon Jun  5 16:31:18 2023, max compression
```

## Comparing `zachet-0.0.1.tar` & `zachet-0.0.10.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 15:48:13.203258 zachet-0.0.1/
--rw-rw-rw-   0        0        0      122 2023-06-05 15:48:13.204260 zachet-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-06-05 15:48:13.205259 zachet-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      251 2023-06-05 15:36:36.000000 zachet-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:48:13.186705 zachet-0.0.1/zachet/
--rw-rw-rw-   0        0        0       18 2023-06-05 15:45:24.000000 zachet-0.0.1/zachet/__init__.py
--rw-rw-rw-   0        0        0     7213 2023-06-05 15:17:48.000000 zachet-0.0.1/zachet/tvz.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:48:13.203258 zachet-0.0.1/zachet.egg-info/
--rw-rw-rw-   0        0        0      122 2023-06-05 15:48:13.000000 zachet-0.0.1/zachet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-06-05 15:48:13.000000 zachet-0.0.1/zachet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 15:48:13.000000 zachet-0.0.1/zachet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 15:48:13.000000 zachet-0.0.1/zachet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 16:31:18.601826 zachet-0.0.10/
+-rw-rw-rw-   0        0        0      123 2023-06-05 16:31:18.601826 zachet-0.0.10/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-06-05 16:31:18.602825 zachet-0.0.10/setup.cfg
+-rw-rw-rw-   0        0        0      252 2023-06-05 16:29:50.000000 zachet-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:31:18.592131 zachet-0.0.10/zachet/
+-rw-rw-rw-   0        0        0       18 2023-06-05 15:45:24.000000 zachet-0.0.10/zachet/__init__.py
+-rw-rw-rw-   0        0        0     5783 2023-06-05 16:27:49.000000 zachet-0.0.10/zachet/tvz.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:31:18.600826 zachet-0.0.10/zachet.egg-info/
+-rw-rw-rw-   0        0        0      123 2023-06-05 16:31:18.000000 zachet-0.0.10/zachet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-06-05 16:31:18.000000 zachet-0.0.10/zachet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:31:18.000000 zachet-0.0.10/zachet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 16:31:18.000000 zachet-0.0.10/zachet.egg-info/top_level.txt
```

