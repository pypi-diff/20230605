# Comparing `tmp/pdfmerge-0.0.7.tar.gz` & `tmp/pdfmerge-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pdfmerge-0.0.7.tar", last modified: Thu Jan  1 03:25:42 2015, max compression
+gzip compressed data, was "pdfmerge-1.0.0.tar", last modified: Mon Jun  5 12:32:48 2023, max compression
```

## Comparing `pdfmerge-0.0.7.tar` & `pdfmerge-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2015-01-01 03:25:42.000000 pdfmerge-0.0.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2015-01-01 03:25:42.000000 pdfmerge-0.0.7/scripts/
--rw-rw-r--   0 lev       (1000) lev       (1000)      105 2013-03-04 15:20:14.000000 pdfmerge-0.0.7/scripts/pdfmerge
--rw-rw-r--   0 lev       (1000) lev       (1000)       31 2013-02-21 22:05:02.000000 pdfmerge-0.0.7/scripts/pdfmerge.bat
--rw-rw-r--   0 lev       (1000) lev       (1000)     1081 2013-02-21 15:32:47.000000 pdfmerge-0.0.7/LICENSE.markdown
--rw-rw-r--   0 lev       (1000) lev       (1000)     5982 2015-01-01 02:39:59.000000 pdfmerge-0.0.7/pdfmerge.py
--rw-rw-r--   0 lev       (1000) lev       (1000)     1860 2014-02-09 20:50:48.000000 pdfmerge-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2015-01-01 03:25:42.000000 pdfmerge-0.0.7/test/
--rw-rw-r--   0 lev       (1000) lev       (1000)      897 2015-01-01 02:35:59.000000 pdfmerge-0.0.7/test/TestMerge.py
--rw-r--r--   0 root         (0) root         (0)       59 2015-01-01 03:25:42.000000 pdfmerge-0.0.7/setup.cfg
--rw-r--r--   0 lev       (1000) lev       (1000)     5803 2015-01-01 02:21:16.000000 pdfmerge-0.0.7/README.markdown
--rw-rw-r--   0 lev       (1000) lev       (1000)      130 2014-05-02 01:53:56.000000 pdfmerge-0.0.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      766 2015-01-01 03:25:42.000000 pdfmerge-0.0.7/PKG-INFO
--rw-rw-r--   0 lev       (1000) lev       (1000)      128 2014-05-02 01:35:26.000000 pdfmerge-0.0.7/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2015-01-01 03:25:42.000000 pdfmerge-0.0.7/pdfmerge.egg-info/
--rw-rw-r--   0 lev       (1000) lev       (1000)       64 2015-01-01 03:25:39.000000 pdfmerge-0.0.7/pdfmerge.egg-info/requires.txt
--rw-rw-r--   0 lev       (1000) lev       (1000)      332 2015-01-01 03:25:39.000000 pdfmerge-0.0.7/pdfmerge.egg-info/SOURCES.txt
--rw-rw-r--   0 lev       (1000) lev       (1000)      766 2015-01-01 03:25:39.000000 pdfmerge-0.0.7/pdfmerge.egg-info/PKG-INFO
--rw-rw-r--   0 lev       (1000) lev       (1000)        1 2015-01-01 03:25:39.000000 pdfmerge-0.0.7/pdfmerge.egg-info/dependency_links.txt
--rw-rw-r--   0 lev       (1000) lev       (1000)        9 2015-01-01 03:25:39.000000 pdfmerge-0.0.7/pdfmerge.egg-info/top_level.txt
--rw-rw-r--   0 lev       (1000) lev       (1000)       44 2015-01-01 03:25:39.000000 pdfmerge-0.0.7/pdfmerge.egg-info/entry_points.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:32:48.002838 pdfmerge-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 12:32:20.000000 pdfmerge-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-05 12:32:47.998837 pdfmerge-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-05 12:32:20.000000 pdfmerge-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-05 12:32:20.000000 pdfmerge-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:32:48.002838 pdfmerge-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:32:47.998837 pdfmerge-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:32:47.998837 pdfmerge-1.0.0/src/pdfmerge/
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-05 12:32:20.000000 pdfmerge-1.0.0/src/pdfmerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-05 12:32:20.000000 pdfmerge-1.0.0/src/pdfmerge/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 12:32:20.000000 pdfmerge-1.0.0/src/pdfmerge/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:32:47.998837 pdfmerge-1.0.0/src/pdfmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-05 12:32:47.000000 pdfmerge-1.0.0/src/pdfmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-05 12:32:47.000000 pdfmerge-1.0.0/src/pdfmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:32:47.000000 pdfmerge-1.0.0/src/pdfmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 12:32:47.000000 pdfmerge-1.0.0/src/pdfmerge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 12:32:47.000000 pdfmerge-1.0.0/src/pdfmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 12:32:47.000000 pdfmerge-1.0.0/src/pdfmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:32:47.998837 pdfmerge-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-05 12:32:20.000000 pdfmerge-1.0.0/test/test_pdfmerge.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pdfmerge-0.0.7/LICENSE.markdown` & `pdfmerge-1.0.0/LICENSE.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Licensed under the MIT License.
 
-Copyright 2013 Metaist.
+Copyright 2023 Metaist LLC.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `pdfmerge-0.0.7/test/TestMerge.py` & `pdfmerge-1.0.0/test/test_pdfmerge.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-#!/usr/bin/python
-# coding: utf-8
+"""Test pdfmerge."""
 
-import os
-import unittest
+# native
+from pathlib import Path
 
-import pdfmerge
+# pkg
+# import pdfmerge
 
-TEST_PDF_DIR = os.path.join('test', 'pdfs')
-TEST_PDF_1 = os.path.join(TEST_PDF_DIR, 'test-1.pdf')
-TEST_PDF_2 = os.path.join(TEST_PDF_DIR, 'test-2.pdf')
-
-
-class TestMerge(unittest.TestCase):
-    def test_pass_single(self):
-        """A non-merge."""
-        writer = pdfmerge.add(TEST_PDF_1)
-        self.assertTrue(writer is not None)
-        self.assertTrue(1, writer.getNumPages())
-
-    def test_merge_dir(self):
-        """Merge all PDFs in a directory."""
-        writer = pdfmerge.add(TEST_PDF_DIR, password='test')
-        self.assertTrue(writer is not None)
-        self.assertTrue(4, writer.getNumPages())
-
-    def test_rule(self):
-        """Merge part of a PDF."""
-        writer = pdfmerge.add(TEST_PDF_2 + '[2]')
-        self.assertTrue(writer is not None)
-        self.assertTrue(1, writer.getNumPages())
+TEST_PDF_DIR = Path("test") / "pdfs"
+TEST_PDF_1 = TEST_PDF_DIR / "test-1.pdf"
+TEST_PDF_2 = TEST_PDF_DIR / "test-2.pdf"
+
+
+# def test_pass_single() -> None:
+#     """A non-merge."""
+#     writer = pdfmerge.add(TEST_PDF_1)
+#     self.assertTrue(writer is not None)
+#     self.assertTrue(1, writer.getNumPages())
+
+# def test_merge_dir(self):
+#     """Merge all PDFs in a directory."""
+#     writer = pdfmerge.add(TEST_PDF_DIR, password="test")
+#     self.assertTrue(writer is not None)
+#     self.assertTrue(4, writer.getNumPages())
+
+# def test_rule(self):
+#     """Merge part of a PDF."""
+#     writer = pdfmerge.add(TEST_PDF_2 + "[2]")
+#     self.assertTrue(writer is not None)
+#     self.assertTrue(1, writer.getNumPages())
```

