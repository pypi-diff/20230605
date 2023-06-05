# Comparing `tmp/yapx-0.0.1a9.tar.gz` & `tmp/yapx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapx-0.0.1a9.tar", last modified: Wed Jan 18 19:05:20 2023, max compression
+gzip compressed data, was "yapx-0.1.0.tar", last modified: Mon Jun  5 07:36:09 2023, max compression
```

## Comparing `yapx-0.0.1a9.tar` & `yapx-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 19:05:20.040428 yapx-0.0.1a9/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-01-18 19:01:42.000000 yapx-0.0.1a9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-18 19:01:42.000000 yapx-0.0.1a9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2138 2023-01-18 19:05:20.040428 yapx-0.0.1a9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1361 2023-01-18 19:01:42.000000 yapx-0.0.1a9/README.md
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-18 19:01:42.000000 yapx-0.0.1a9/VERSION
--rw-r--r--   0 root         (0) root         (0)     2703 2023-01-18 19:05:20.040428 yapx-0.0.1a9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-18 19:01:42.000000 yapx-0.0.1a9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 19:05:20.036428 yapx-0.0.1a9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 19:05:20.040428 yapx-0.0.1a9/src/yapx/
--rw-r--r--   0 root         (0) root         (0)      392 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 19:05:20.040428 yapx-0.0.1a9/src/yapx/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      468 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      150 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3570 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/actions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     5514 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/arg.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2239 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/argparse_action.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    17589 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/argument_parser.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      126 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     1209 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/types.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     1867 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       24 2023-01-18 19:05:13.000000 yapx-0.0.1a9/src/yapx/__version__.py
--rw-r--r--   0 root         (0) root         (0)     4493 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/actions.py
--rw-r--r--   0 root         (0) root         (0)     6969 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/arg.py
--rw-r--r--   0 root         (0) root         (0)     1400 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/argparse_action.py
--rw-r--r--   0 root         (0) root         (0)    27459 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/argument_parser.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/exceptions.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/py.typed
--rw-r--r--   0 root         (0) root         (0)      598 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/types.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 19:05:20.040428 yapx-0.0.1a9/src/yapx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2138 2023-01-18 19:05:20.000000 yapx-0.0.1a9/src/yapx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-01-18 19:05:20.000000 yapx-0.0.1a9/src/yapx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-18 19:05:20.000000 yapx-0.0.1a9/src/yapx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      559 2023-01-18 19:05:20.000000 yapx-0.0.1a9/src/yapx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-01-18 19:05:20.000000 yapx-0.0.1a9/src/yapx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 07:36:09.949467 yapx-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-06-05 07:31:38.000000 yapx-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6374 2023-06-05 07:36:09.949467 yapx-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4623 2023-06-05 07:31:38.000000 yapx-0.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     4756 2023-06-05 07:31:38.000000 yapx-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 07:36:09.949467 yapx-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 07:36:09.945467 yapx-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 07:36:09.949467 yapx-0.1.0/src/yapx/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-06-05 07:31:38.000000 yapx-0.1.0/src/yapx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 07:36:09.949467 yapx-0.1.0/src/yapx/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      469 2023-06-05 07:32:05.000000 yapx-0.1.0/src/yapx/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-05 07:35:52.000000 yapx-0.1.0/src/yapx/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-06-05 07:32:05.000000 yapx-0.1.0/src/yapx/__pycache__/actions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7273 2023-06-05 07:32:05.000000 yapx-0.1.0/src/yapx/__pycache__/arg.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-06-05 07:32:05.000000 yapx-0.1.0/src/yapx/__pycache__/argparse_action.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    30946 2023-06-05 07:32:06.000000 yapx-0.1.0/src/yapx/__pycache__/argument_parser.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      921 2023-06-05 07:32:05.000000 yapx-0.1.0/src/yapx/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-06-05 07:32:05.000000 yapx-0.1.0/src/yapx/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     5198 2023-06-05 07:32:05.000000 yapx-0.1.0/src/yapx/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-05 07:35:52.000000 yapx-0.1.0/src/yapx/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     4437 2023-06-05 07:31:38.000000 yapx-0.1.0/src/yapx/actions.py
+-rw-r--r--   0 root         (0) root         (0)     9374 2023-06-05 07:31:38.000000 yapx-0.1.0/src/yapx/arg.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-05 07:31:38.000000 yapx-0.1.0/src/yapx/argparse_action.py
+-rw-r--r--   0 root         (0) root         (0)    47449 2023-06-05 07:31:38.000000 yapx-0.1.0/src/yapx/argument_parser.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-06-05 07:31:38.000000 yapx-0.1.0/src/yapx/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 07:31:38.000000 yapx-0.1.0/src/yapx/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-06-05 07:31:38.000000 yapx-0.1.0/src/yapx/types.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2023-06-05 07:31:38.000000 yapx-0.1.0/src/yapx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 07:36:09.949467 yapx-0.1.0/src/yapx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6374 2023-06-05 07:36:09.000000 yapx-0.1.0/src/yapx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-05 07:36:09.000000 yapx-0.1.0/src/yapx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 07:36:09.000000 yapx-0.1.0/src/yapx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      681 2023-06-05 07:36:09.000000 yapx-0.1.0/src/yapx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-05 07:36:09.000000 yapx-0.1.0/src/yapx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 07:36:09.949467 yapx-0.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-06-05 07:31:38.000000 yapx-0.1.0/tests/test_actions.py
+-rw-r--r--   0 root         (0) root         (0)    11966 2023-06-05 07:31:38.000000 yapx-0.1.0/tests/test_add_arguments.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-06-05 07:31:38.000000 yapx-0.1.0/tests/test_add_arguments_future.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-06-05 07:31:38.000000 yapx-0.1.0/tests/test_add_command.py
+-rw-r--r--   0 root         (0) root         (0)     8033 2023-06-05 07:31:38.000000 yapx-0.1.0/tests/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)    22151 2023-06-05 07:31:38.000000 yapx-0.1.0/tests/test_run.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-05 07:31:38.000000 yapx-0.1.0/tests/test_utils.py
```

### Comparing `yapx-0.0.1a9/LICENSE` & `yapx-0.1.0/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,7 @@
+Copyright 2023 Donald Mellenbruch
 
-The MIT License
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-Copyright (c) 2022 Donald Mellenbruch
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `yapx-0.0.1a9/src/yapx/__pycache__/argparse_action.cpython-310.pyc` & `yapx-0.1.0/src/yapx/__pycache__/argparse_action.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jan 18 19:01:42 2023 UTC, .py size: 1400 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1642 c863 7805 0000  o........B.cx...
+00000000: 6f0d 0d0a 0000 0000 5a8f 7d64 7d05 0000  o.......Z.}d}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6404  m.Z.m.Z.m.Z...d.
 00000070: 6405 6c0d 6d0e 5a0e 0100 6406 6701 5a0f  d.l.m.Z...d.g.Z.
@@ -98,43 +98,43 @@
 00000610: 0000 0073 2400 0000 7c01 a000 8802 a101  ...s$...|.......
 00000620: 0100 7401 8300 6a02 6402 6401 8801 6901  ..t...j.d.d...i.
 00000630: 7c01 a401 8e01 0100 6400 5300 2903 4e72  |.......d.S.).Nr
 00000640: 1200 0000 7215 0000 0029 03da 0675 7064  ....r....)...upd
 00000650: 6174 6572 1600 0000 7217 0000 0029 0272  ater....r....).r
 00000660: 1b00 0000 722e 0000 0029 0372 1d00 0000  ....r....).r....
 00000670: 7212 0000 0072 2d00 0000 7215 0000 0072  r....r-...r....r
-00000680: 1e00 0000 7217 0000 002c 0000 0073 0400  ....r....,...s..
+00000680: 1e00 0000 7217 0000 002d 0000 0073 0400  ....r....-...s..
 00000690: 0000 0a01 1a01 7a48 6172 6770 6172 7365  ......zHargparse
 000006a0: 5f61 6374 696f 6e2e 3c6c 6f63 616c 733e  _action.<locals>
 000006b0: 2e5f 6e65 775f 6170 785f 6163 7469 6f6e  ._new_apx_action
 000006c0: 2e3c 6c6f 6361 6c73 3e2e 4e65 7759 6170  .<locals>.NewYap
 000006d0: 7841 6374 696f 6e2e 5f5f 696e 6974 5f5f  xAction.__init__
 000006e0: 2906 7219 0000 0072 2900 0000 722a 0000  ).r....r)...r*..
 000006f0: 0072 0600 0000 7217 0000 0072 2c00 0000  .r....r....r,...
 00000700: 7215 0000 0029 0272 1200 0000 722d 0000  r....).r....r-..
 00000710: 0072 1c00 0000 721e 0000 00da 0d4e 6577  .r....r......New
-00000720: 5961 7078 4163 7469 6f6e 2b00 0000 7304  YapxAction+...s.
+00000720: 5961 7078 4163 7469 6f6e 2c00 0000 7304  YapxAction,...s.
 00000730: 0000 0008 0022 0172 3000 0000 2901 7211  .....".r0...).r.
 00000740: 0000 0029 0272 2d00 0000 7230 0000 00a9  ...).r-...r0....
 00000750: 0172 1200 0000 2901 722d 0000 0072 1e00  .r....).r-...r..
 00000760: 0000 da0f 5f6e 6577 5f61 7078 5f61 6374  ...._new_apx_act
-00000770: 696f 6e2a 0000 0073 0400 0000 1601 0405  ion*...s........
+00000770: 696f 6e2b 0000 0073 0400 0000 1601 0405  ion+...s........
 00000780: 7a28 6172 6770 6172 7365 5f61 6374 696f  z(argparse_actio
 00000790: 6e2e 3c6c 6f63 616c 733e 2e5f 6e65 775f  n.<locals>._new_
 000007a0: 6170 785f 6163 7469 6f6e 7215 0000 0029  apx_actionr....)
 000007b0: 0572 0500 0000 720e 0000 0072 0600 0000  .r....r....r....
 000007c0: 7209 0000 0072 1100 0000 2903 7212 0000  r....r....).r...
 000007d0: 0072 1300 0000 7232 0000 0072 1500 0000  .r....r2...r....
 000007e0: 7231 0000 0072 1e00 0000 720e 0000 0024  r1...r....r....$
-000007f0: 0000 0073 0800 0000 0403 1001 1a02 0e08  ...s............
-00000800: 7228 0000 0029 13da 0861 7267 7061 7273  r(...)...argpars
+000007f0: 0000 0073 0800 0000 0404 1001 1a02 0e08  ...s............
+00000800: 7228 0000 0029 135a 0861 7267 7061 7273  r(...).Z.argpars
 00000810: 6572 0200 0000 7203 0000 0072 0400 0000  er....r....r....
 00000820: da09 6675 6e63 746f 6f6c 7372 0500 0000  ..functoolsr....
 00000830: da06 7479 7069 6e67 7206 0000 0072 0700  ..typingr....r..
 00000840: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
 00000850: 0072 0b00 0000 da05 7479 7065 7372 0d00  .r......typesr..
 00000860: 0000 da07 5f5f 616c 6c5f 5f72 0f00 0000  ....__all__r....
 00000870: 7211 0000 0072 0e00 0000 7215 0000 0072  r....r....r....r
 00000880: 1500 0000 7215 0000 0072 1e00 0000 da08  ....r....r......
 00000890: 3c6d 6f64 756c 653e 0100 0000 731e 0000  <module>....s...
 000008a0: 0014 000c 0120 010c 0206 0214 0310 0302  ..... ..........
-000008b0: 1804 ff06 0102 ff02 0102 ff1a 020e fe    ...............
+000008b0: 1804 ff06 0102 ff02 0202 fe1a 030e fd    ...............
```

### Comparing `yapx-0.0.1a9/src/yapx/actions.py` & `yapx-0.1.0/src/yapx/actions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import collections.abc
 import shlex
-from enum import Enum
-from typing import Any, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Set, Tuple, Type, TypeVar
 
 from .argparse_action import YapxAction, argparse_action
 from .types import ArgumentParser, ArgValueType
-from .utils import coalesce, is_instance, is_subclass
+from .utils import coalesce, try_isinstance, try_issubclass
 
 # @argparse_action
 # # pylint: disable=unused-argument
 # def to_str(
 #     value: ArgValueType,
 #     *,
 #     action: argparse.Action,
@@ -22,159 +21,157 @@
 
 T = TypeVar("T", bound=type)
 
 
 def _split_csv_sequence(
     values: ArgValueType,
     target_type: T,
-) -> Union[None, T, List[T]]:
-    def _cast_type(txt: str, target_type: T) -> T:
-        return (
-            txt
-            if is_instance(txt, target_type)
-            else target_type[txt]
-            if is_subclass(target_type, Enum)
-            else target_type(txt)
-        )
-
+) -> Optional[List[T]]:
     if isinstance(values, str) and values:
         values = [values]
     elif (
         values is None
-        or not is_subclass(type(values), collections.abc.Sequence)
+        or not try_issubclass(type(values), collections.abc.Sequence)
         or len(values) == 0
         or not isinstance(values[0], str)
     ):
         return values
 
     all_values: List[str] = []
 
     list_prefix: str = "list["
     list_suffix: str = "]"
 
+    if all(x.endswith(",") for x in values[:-1]):
+        values = [x.rstrip(",") for x in values]
+
     for value in values:
         value_clean: str = value.strip()
 
         if (
             value_clean
             and value_clean.lower().startswith(list_prefix)
             and value_clean.lower().endswith(list_suffix)
         ):
             all_values.extend(
-                _cast_type(x, target_type=target_type)
-                for x in shlex.split(
-                    value_clean[len(list_prefix) : -len(list_suffix)].strip()
-                )
+                _split_csv_sequence(
+                    values=shlex.split(
+                        value_clean[len(list_prefix) : -len(list_suffix)].strip(),
+                    ),
+                    target_type=target_type,
+                ),
             )
         else:
-            all_values.append(_cast_type(value, target_type=target_type))
+            all_values.append(target_type(value))
 
     return all_values
 
 
-def _get_target_type(action: YapxAction, parser: ArgumentParser) -> type:
-    if not parser:
-        return action.type
-    # pylint: disable=protected-access
-    return parser._inner_type_conversions.get(action.dest, action.type)
-
-
 @argparse_action
-# pylint: disable=unused-argument
 def split_csv(
     values: ArgValueType,
     *,
     action: YapxAction,
     parser: ArgumentParser,
-    **kwargs: Any,
+    **_kwargs: Any,
 ) -> Optional[List[Optional[Any]]]:
     return _split_csv_sequence(
         values,
-        target_type=_get_target_type(action, parser),
+        target_type=parser._inner_type_conversions.get(  # pylint: disable=protected-access
+            action.dest,
+        ),
     )
 
 
 @argparse_action
 def split_csv_to_tuple(
     values: ArgValueType,
     *,
     action: YapxAction,
     parser: ArgumentParser,
-    **kwargs: Any,
+    **_kwargs: Any,
 ) -> Optional[Tuple[Optional[Any], ...]]:
     split_values: Optional[List[Optional[Any]]] = _split_csv_sequence(
         values,
-        target_type=_get_target_type(action, parser),
+        target_type=parser._inner_type_conversions.get(  # pylint: disable=protected-access
+            action.dest,
+        ),
     )
-    if split_values is not None:
-        return tuple(split_values)
-    return None
+
+    if split_values is None:
+        return None
+
+    return tuple(split_values)
 
 
 @argparse_action
 def split_csv_to_set(
     values: ArgValueType,
     *,
     action: YapxAction,
     parser: ArgumentParser,
-    **kwargs: Any,
+    **_kwargs: Any,
 ) -> Optional[Set[Optional[Any]]]:
+    if try_isinstance(values, set):
+        return values
+
     split_values: Optional[List[Optional[Any]]] = _split_csv_sequence(
         values,
-        target_type=_get_target_type(action, parser),
+        target_type=parser._inner_type_conversions.get(  # pylint: disable=protected-access
+            action.dest,
+        ),
     )
-    if split_values is not None:
-        return set(split_values)
-    return None
+    if split_values is None:
+        return None
 
+    return set(split_values)
 
-@argparse_action
-def split_csv_to_dict(
+
+def _split_csv_to_dict(
     values: ArgValueType,
-    *,
-    action: YapxAction,
-    parser: ArgumentParser,
-    **kwargs: Any,
+    kv_separator: str,
+    target_value_type: Optional[Type[Any]] = None,
 ) -> Optional[Dict[str, Optional[Any]]]:
+    if try_isinstance(values, dict):
+        return values
+
     split_values: Optional[List[Optional[Any]]] = _split_csv_sequence(
-        values, target_type=str
+        values,
+        target_type=str,
     )
 
-    if split_values is not None:
-        return {
-            x_split[0].strip(): None
-            if len(x_split) < 2
-            else coalesce(x_split[1].strip(), None, null_or_empty=True)
-            for x in split_values
-            if x
-            for x_split in [x.split(parser.kv_separator, maxsplit=1)]
-        }
-    return None
-
-
-@argparse_action
-def str2enum(
-    values: ArgValueType,
-    *,
-    action: YapxAction,
-    parser: ArgumentParser,
-    **kwargs: Any,
-) -> Optional[Enum]:
-    if values is None:
+    if split_values is None:
         return None
 
-    target_type: Type[Enum] = _get_target_type(action=action, parser=parser)
-    if is_instance(values, target_type):
-        return values
-
-    return target_type[values]
+    return {
+        x_split[0].strip(): (
+            v if v is None or target_value_type is None else target_value_type(v)
+        )
+        for x in split_values
+        if x
+        for x_split in [x.split(kv_separator, maxsplit=1)]
+        for v in [
+            (
+                None
+                if len(x_split) < 2
+                else coalesce(x_split[1].strip(), None, null_or_empty=True)
+            ),
+        ]
+    }
 
 
-@argparse_action(nargs=0)
-def print_help(
+@argparse_action
+def split_csv_to_dict(
     values: ArgValueType,
     *,
+    action: YapxAction,
     parser: ArgumentParser,
-    **kwargs: Any,
-) -> None:
-    parser.print_help()
-    parser.exit()
+    **_kwargs: Any,
+) -> Optional[Dict[str, Optional[Any]]]:
+    return _split_csv_to_dict(
+        values,
+        kv_separator=parser.kv_separator,
+        target_value_type=parser._inner_type_conversions.get(  # pylint: disable=protected-access
+            action.dest,
+            str,
+        ),
+    )
```

### Comparing `yapx-0.0.1a9/src/yapx/arg.py` & `yapx-0.1.0/src/yapx/arg.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,46 @@
 import os
+import sys
 from argparse import Action
 from contextlib import suppress
 from dataclasses import MISSING, Field, dataclass, field, make_dataclass
-from inspect import _empty, signature
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Type, Union
+from inspect import Parameter, _empty, signature
+from pathlib import Path
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    get_type_hints,
+)
 
-from typing_extensions import Literal  # noqa: keep this so eval of `Literal` works...
+import yapx  # pylint: disable=unused-import # noqa: F401
 
 from .types import Dataclass
 
-__all__ = ["arg"]
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=unused-import # noqa: F401
+else:
+    from typing_extensions import Literal  # pylint: disable=unused-import # noqa: F401
+
+if sys.version_info >= (3, 9):
+    from typing import Annotated  # pylint: disable=unused-import # noqa: F401
+else:
+    from typing_extensions import (  # pylint: disable=unused-import # noqa: F401
+        Annotated,
+    )
+
 
+__all__ = ["arg"]
 
-try:
-    from typing import get_type_hints
-except ImportError:
-    from typing_extensions import get_type_hints
 
 ARGPARSE_ARG_METADATA_KEY: str = "_argparse_argument"
 
 
 @dataclass
 class ArgparseArg:
     dest: Optional[str] = None
@@ -32,18 +53,28 @@
     nargs: Optional[str] = None
     const: Optional[Any] = None
     default: Optional[Any] = None
     choices: Optional[Sequence[Any]] = None
     help: Optional[str] = None
     metavar: Optional[str] = None
     pos: Optional[bool] = False
-    _env_var: Optional[str] = None
+    _env_var: Union[None, str, Sequence[str]] = None
 
     def __post_init__(self) -> None:
-        if self.dest and not self.option_strings:
+        self.set_dest(self.dest)
+
+    def set_dest(self, value: Optional[str]) -> None:
+        self.dest = value
+
+        if self.option_strings:
+            if self.pos:
+                self.option_strings = None
+            elif isinstance(self.option_strings, str):
+                self.option_strings = [self.option_strings]
+        elif self.dest and not self.pos:
             self.option_strings = [convert_to_flag_string(self.dest)]
 
     def asdict(self) -> Dict[str, Any]:
         return {k: v for k, v in vars(self).items() if not k.startswith("_")}
 
 
 def arg(
@@ -52,58 +83,98 @@
     pos: Optional[bool] = False,
     group: Optional[str] = None,
     exclusive: Optional[bool] = False,
     flags: Union[None, str, Sequence[str]] = None,
     # pylint: disable=redefined-builtin
     help: Optional[str] = None,
     metavar: Optional[str] = None,
-    action: Optional[Action] = None,
+    action: Union[None, str, Type[Action]] = None,
 ) -> Field:
+    """Provides an interface to modify argument options.
+
+    Args:
+        default: default value for the argument.
+            If not given, argument is required.
+        env: list of environment variables that will provide the argument value.
+        pos: if True, argument is positional (no flags).
+        group: group for the argument.
+        exclusive: if True, this arg cannot be specified along with another exclusive arg in the same group.
+        flags: list of flags to use for the argument.
+        help: help text / description
+        metavar: variable name printed in help text.
+        action: custom action for this argument.
+
+    Examples:
+        >>> import yapx
+        >>> from yapx.types import Annotated
+        ...
+        >>> def say_hello(
+        ...     value = yapx.arg(default='World')
+        ... ):
+        ...     print(f"Hello {value}")
+        ...
+        >>> yapx.run(say_hello, _args=[])
+        Hello World
+
+        >>> import yapx
+        >>> from yapx.types import Annotated
+        ...
+        >>> def say_hello(
+        ...     value: Annotated[str, yapx.arg(default='World')]
+        ... ):
+        ...     print(f"Hello {value}")
+        ...
+        >>> yapx.run(say_hello, _args=[])
+        Hello World
+    """
     if env:
         if isinstance(env, str):
             env = [env]
         for e in env:
             value_from_env = os.getenv(e, None)
             if value_from_env:
                 default = value_from_env
                 break
 
             env_file = os.getenv(e + "_FILE", None)
-            if env_file and os.path.exists(env_file):
-                with open(env_file, encoding="utf8") as f:
-                    value_from_file = f.read().strip()
-                if value_from_file:
-                    default = value_from_file
-                    break
-
-    required = default is MISSING
+            if env_file:
+                env_file_path: Path = Path(env_file)
+                if env_file_path.exists():
+                    value_from_file = env_file_path.read_text(encoding="utf-8").strip()
+                    if value_from_file:
+                        default = value_from_file
+                        break
 
     metadata: Dict[str, ArgparseArg] = {
         ARGPARSE_ARG_METADATA_KEY: ArgparseArg(
             action=action,
             pos=pos,
-            option_strings=[flags] if isinstance(flags, str) else flags,
-            required=required,
+            option_strings=flags,
+            required=bool(default is MISSING),
+            default=(
+                None
+                if default is MISSING
+                else default()
+                if callable(default)
+                else default
+            ),
             group=group,
             exclusive=exclusive,
-            default=(None if required else default() if callable(default) else default),
             help=help,
             metavar=metavar,
             _env_var=env,
-        )
+        ),
     }
 
     kwargs: Dict[str, Any] = {"metadata": metadata}
 
     default_param: str = "default_factory" if callable(default) else "default"
     kwargs[default_param] = default
 
-    fld: Field = field(**kwargs)
-    assert isinstance(fld, Field)
-    return fld
+    return field(**kwargs)
 
 
 def convert_to_command_string(x: str) -> str:
     x = x.strip()
 
     x_prefix: str = "x_"
     under: str = "_"
@@ -124,15 +195,16 @@
     if not x:
         raise ValueError("Expected at least one character")
 
     return x
 
 
 def convert_to_flag_string(x: str) -> str:
-    return "--" + convert_to_command_string(x)
+    cmd_str: str = convert_to_command_string(x)
+    return "--" + cmd_str if len(cmd_str) > 1 else "-" + cmd_str
 
 
 def convert_to_short_flag_string(x: str) -> str:
     return "-" + convert_to_command_string(x)[0]
 
 
 def _eval_type(type_str: str) -> Type[Any]:
@@ -153,31 +225,36 @@
 
 
 def make_dataclass_from_func(
     func: Callable[..., Any],
     base_classes: Optional[Tuple[Type[Dataclass], ...]] = None,
     include_private_params: bool = False,
 ) -> Type[Dataclass]:
-
     if base_classes is None:
         base_classes = ()
 
     fields: List[Tuple[str, Type[Any], Field]] = []
 
     func_signature = signature(func)
     type_hints: Dict[str, Any]
     try:
-        type_hints = get_type_hints(func)
+        include_extras: Dict[str, bool] = {}
+        if sys.version_info >= (3, 9):
+            include_extras["include_extras"] = True
+        type_hints = get_type_hints(func, **include_extras)
     except (TypeError, NameError):
         # this can happen if deferred evaluation is used,
         # via `from __future__ import annotations`
         type_hints = {}
 
+    param: Parameter
     for param in func_signature.parameters.values():
-        if not include_private_params and param.name.startswith("_"):
+        if str(param).startswith("*") or (
+            not include_private_params and param.name.startswith("_")
+        ):
             continue
 
         annotation: Type[Any] = (
             _eval_type(param.annotation)
             if isinstance(param.annotation, str)
             else type_hints.get(param.name, param.annotation)
         )
@@ -211,16 +288,18 @@
                 annotation = Optional[fallback_type]
             else:
                 type_of_default: Type[Any] = type(default_value)
                 if type_of_default in (str, int, float, bool):
                     annotation = type_of_default
                 else:
                     raise TypeError(
-                        f"Provide explicit type annotation for '{param.name}' "
-                        f"(type  of default is '{type_of_default})'"
+                        (
+                            f"Provide explicit type annotation for '{param.name}' "
+                            f"(type  of default is '{type_of_default})'"
+                        ),
                     )
 
         fields.append((param.name, annotation, field_metadata))
 
     dc: Type[Dataclass] = make_dataclass(
         cls_name="Dataclass_" + func.__name__,
         bases=base_classes,
```

### Comparing `yapx-0.0.1a9/src/yapx/argparse_action.py` & `yapx-0.1.0/src/yapx/argparse_action.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,16 @@
             namespace=namespace,
             option_string=option_string,
         )
         setattr(namespace, self.dest, value)
 
 
 def argparse_action(
-    func: Optional[F] = None, **kwargs: Any
+    func: Optional[F] = None,
+    **kwargs: Any,
 ) -> Union[Type[YapxAction], Callable[..., Type[YapxAction]]]:
     if not func:
         return partial(argparse_action, **kwargs)
 
     def _new_apx_action(**wrapper_kwargs: Any) -> Type[YapxAction]:
         class NewYapxAction(YapxAction):
             def __init__(self, **inner_kwargs: Any) -> None:
```

### Comparing `yapx-0.0.1a9/src/yapx.egg-info/SOURCES.txt` & `yapx-0.1.0/src/yapx.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 LICENSE
-MANIFEST.in
 README.md
-VERSION
-setup.cfg
-setup.py
+pyproject.toml
 src/yapx/__init__.py
 src/yapx/__version__.py
 src/yapx/actions.py
 src/yapx/arg.py
 src/yapx/argparse_action.py
 src/yapx/argument_parser.py
 src/yapx/exceptions.py
@@ -23,8 +20,15 @@
 src/yapx/__pycache__/__version__.cpython-310.pyc
 src/yapx/__pycache__/actions.cpython-310.pyc
 src/yapx/__pycache__/arg.cpython-310.pyc
 src/yapx/__pycache__/argparse_action.cpython-310.pyc
 src/yapx/__pycache__/argument_parser.cpython-310.pyc
 src/yapx/__pycache__/exceptions.cpython-310.pyc
 src/yapx/__pycache__/types.cpython-310.pyc
-src/yapx/__pycache__/utils.cpython-310.pyc
+src/yapx/__pycache__/utils.cpython-310.pyc
+tests/test_actions.py
+tests/test_add_arguments.py
+tests/test_add_arguments_future.py
+tests/test_add_command.py
+tests/test_arg.py
+tests/test_run.py
+tests/test_utils.py
```

