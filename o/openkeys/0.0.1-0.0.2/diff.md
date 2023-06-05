# Comparing `tmp/openkeys-0.0.1.tar.gz` & `tmp/openkeys-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openkeys-0.0.1.tar", last modified: Mon Jun  5 04:24:23 2023, max compression
+gzip compressed data, was "openkeys-0.0.2.tar", last modified: Mon Jun  5 04:59:22 2023, max compression
```

## Comparing `openkeys-0.0.1.tar` & `openkeys-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       13 2023-06-05 04:10:04.505926 openkeys-0.0.1/README.md
--rw-r--r--   0        0        0      459 2023-06-05 04:23:43.120200 openkeys-0.0.1/__init__.py
--rw-r--r--   0        0        0      374 2023-06-05 04:24:23.367102 openkeys-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 openkeys-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-06-05 04:10:04.505926 openkeys-0.0.2/README.md
+-rw-r--r--   0        0        0      475 2023-06-05 04:56:46.139948 openkeys-0.0.2/__init__.py
+-rw-r--r--   0        0        0      353 2023-06-05 04:59:22.742981 openkeys-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 openkeys-0.0.2/PKG-INFO
```

