# Comparing `tmp/exampleproject_crida-0.2.0.tar.gz` & `tmp/exampleproject_crida-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exampleproject_crida-0.2.0.tar", max compression
+gzip compressed data, was "exampleproject_crida-0.2.1.tar", max compression
```

## Comparing `exampleproject_crida-0.2.0.tar` & `exampleproject_crida-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-05 08:42:00.330913 exampleproject_crida-0.2.0/exampleproject_crida/__init__.py
--rw-r--r--   0        0        0      502 2023-06-05 13:28:27.012013 exampleproject_crida-0.2.0/exampleproject_crida/example_usage.py
--rw-r--r--   0        0        0      300 2023-06-05 13:57:16.519618 exampleproject_crida-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      490 2023-06-05 13:42:45.470166 exampleproject_crida-0.2.0/README.md
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 exampleproject_crida-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 08:42:00.330913 exampleproject_crida-0.2.1/exampleproject_crida/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-05 13:28:27.012013 exampleproject_crida-0.2.1/exampleproject_crida/example_usage.py
+-rw-r--r--   0        0        0      311 2023-06-05 14:05:05.476869 exampleproject_crida-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      301 2023-06-05 14:04:37.087593 exampleproject_crida-0.2.1/README_repository.md
+-rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 exampleproject_crida-0.2.1/PKG-INFO
```

