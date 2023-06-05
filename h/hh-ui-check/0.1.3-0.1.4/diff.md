# Comparing `tmp/hh_ui_check-0.1.3.tar.gz` & `tmp/hh_ui_check-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hh_ui_check-0.1.3.tar", max compression
+gzip compressed data, was "hh_ui_check-0.1.4.tar", max compression
```

## Comparing `hh_ui_check-0.1.3.tar` & `hh_ui_check-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6273 2023-06-02 05:34:57.983561 hh_ui_check-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-02 03:09:39.424775 hh_ui_check-0.1.3/hh_ui_check/__init__.py
--rwxr-xr-x   0        0        0      640 2023-06-05 06:20:47.720738 hh_ui_check-0.1.3/hh_ui_check/__main__.py
--rw-r--r--   0        0        0     3709 2023-06-02 03:11:51.900039 hh_ui_check-0.1.3/hh_ui_check/diff.py
--rw-r--r--   0        0        0     2088 2023-06-02 03:11:51.915520 hh_ui_check-0.1.3/hh_ui_check/hist_compare.py
--rw-r--r--   0        0        0      479 2023-06-02 03:11:51.921769 hh_ui_check-0.1.3/hh_ui_check/horizen.py
--rw-r--r--   0        0        0      583 2023-06-02 03:11:51.937183 hh_ui_check-0.1.3/hh_ui_check/overlapping.py
--rw-r--r--   0        0        0      447 2023-06-02 03:11:51.942201 hh_ui_check-0.1.3/hh_ui_check/substract.py
--rw-r--r--   0        0        0      441 2023-06-05 06:38:34.290134 hh_ui_check-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6751 1970-01-01 00:00:00.000000 hh_ui_check-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6273 2023-06-02 05:34:57.983561 hh_ui_check-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 03:09:39.424775 hh_ui_check-0.1.4/hh_ui_check/__init__.py
+-rwxr-xr-x   0        0        0      640 2023-06-05 06:20:47.720738 hh_ui_check-0.1.4/hh_ui_check/__main__.py
+-rw-r--r--   0        0        0     3733 2023-06-05 06:42:28.034026 hh_ui_check-0.1.4/hh_ui_check/diff.py
+-rw-r--r--   0        0        0     2112 2023-06-05 06:42:32.130634 hh_ui_check-0.1.4/hh_ui_check/hist_compare.py
+-rw-r--r--   0        0        0      503 2023-06-05 06:42:35.999893 hh_ui_check-0.1.4/hh_ui_check/horizen.py
+-rw-r--r--   0        0        0      607 2023-06-05 06:42:45.982863 hh_ui_check-0.1.4/hh_ui_check/overlapping.py
+-rw-r--r--   0        0        0      471 2023-06-05 06:42:23.464798 hh_ui_check-0.1.4/hh_ui_check/substract.py
+-rw-r--r--   0        0        0      441 2023-06-05 06:42:52.447479 hh_ui_check-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6751 1970-01-01 00:00:00.000000 hh_ui_check-0.1.4/PKG-INFO
```

### Comparing `hh_ui_check-0.1.3/README.md` & `hh_ui_check-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hh_ui_check-0.1.3/hh_ui_check/__main__.py` & `hh_ui_check-0.1.4/hh_ui_check/__main__.py`

 * *Files identical despite different names*

### Comparing `hh_ui_check-0.1.3/hh_ui_check/diff.py` & `hh_ui_check-0.1.4/hh_ui_check/diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 import cv2
 import numpy as np
 
 # 最大要素数量 默认500
 MAX_FEATURES = 500
 GOOD_MATCH_PERCENT = 0.15
```

### Comparing `hh_ui_check-0.1.3/hh_ui_check/hist_compare.py` & `hh_ui_check-0.1.4/hh_ui_check/hist_compare.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 import cv2 as cv
 import numpy as np
 from matplotlib import pyplot as plt
 
 
 def create_rgb_hist(image):
   """"创建 RGB 三通道直方图（直方图矩阵）"""
```

### Comparing `hh_ui_check-0.1.3/hh_ui_check/overlapping.py` & `hh_ui_check-0.1.4/hh_ui_check/overlapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # 两图相减法
 import cv2
 import numpy as np
 
 
 def getOverlapping(image1, image2):
   hh, ww = image1.shape[:2]
```

### Comparing `hh_ui_check-0.1.3/PKG-INFO` & `hh_ui_check-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hh-ui-check
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: 林明超
 Author-email: mingchao.lin@zeekrlife.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

