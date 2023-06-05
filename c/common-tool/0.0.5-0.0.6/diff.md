# Comparing `tmp/common_tool-0.0.5.tar.gz` & `tmp/common_tool-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_tool-0.0.5.tar", last modified: Mon Jun  5 08:12:32 2023, max compression
+gzip compressed data, was "common_tool-0.0.6.tar", last modified: Mon Jun  5 09:14:05 2023, max compression
```

## Comparing `common_tool-0.0.5.tar` & `common_tool-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 08:12:32.852629 common_tool-0.0.5/
--rw-r--r--   0 donghao    (501) staff       (20)     1065 2022-07-13 09:33:27.000000 common_tool-0.0.5/LICENSE
--rw-r--r--   0 donghao    (501) staff       (20)      601 2023-06-05 08:12:32.852507 common_tool-0.0.5/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      317 2022-07-13 10:19:33.000000 common_tool-0.0.5/README.md
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 08:12:32.851654 common_tool-0.0.5/common_tool/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2022-07-13 09:32:57.000000 common_tool-0.0.5/common_tool/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)      622 2022-07-13 09:32:57.000000 common_tool-0.0.5/common_tool/datetime.py
--rw-r--r--   0 donghao    (501) staff       (20)     3441 2023-05-19 06:59:19.000000 common_tool-0.0.5/common_tool/enum.py
--rw-r--r--   0 donghao    (501) staff       (20)     1464 2023-06-05 01:21:44.000000 common_tool-0.0.5/common_tool/http.py
--rw-r--r--   0 donghao    (501) staff       (20)      246 2023-05-19 06:58:46.000000 common_tool-0.0.5/common_tool/loggers.py
--rw-r--r--   0 donghao    (501) staff       (20)      476 2022-07-13 09:32:57.000000 common_tool-0.0.5/common_tool/math.py
--rw-r--r--   0 donghao    (501) staff       (20)     1162 2022-07-13 09:32:57.000000 common_tool-0.0.5/common_tool/random.py
--rw-r--r--   0 donghao    (501) staff       (20)      402 2022-07-13 09:32:57.000000 common_tool-0.0.5/common_tool/token.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 08:12:32.852156 common_tool-0.0.5/common_tool.egg-info/
--rw-r--r--   0 donghao    (501) staff       (20)      601 2023-06-05 08:12:32.000000 common_tool-0.0.5/common_tool.egg-info/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      391 2023-06-05 08:12:32.000000 common_tool-0.0.5/common_tool.egg-info/SOURCES.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-05 08:12:32.000000 common_tool-0.0.5/common_tool.egg-info/dependency_links.txt
--rw-r--r--   0 donghao    (501) staff       (20)       12 2023-06-05 08:12:32.000000 common_tool-0.0.5/common_tool.egg-info/requires.txt
--rw-r--r--   0 donghao    (501) staff       (20)       17 2023-06-05 08:12:32.000000 common_tool-0.0.5/common_tool.egg-info/top_level.txt
--rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-05 08:12:32.852664 common_tool-0.0.5/setup.cfg
--rw-r--r--   0 donghao    (501) staff       (20)      714 2023-06-05 08:12:28.000000 common_tool-0.0.5/setup.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 08:12:32.852245 common_tool-0.0.5/test/
--rw-r--r--   0 donghao    (501) staff       (20)       97 2022-07-13 10:03:42.000000 common_tool-0.0.5/test/__init__.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 09:14:05.536118 common_tool-0.0.6/
+-rw-r--r--   0 donghao    (501) staff       (20)     1065 2022-07-13 09:33:27.000000 common_tool-0.0.6/LICENSE
+-rw-r--r--   0 donghao    (501) staff       (20)      601 2023-06-05 09:14:05.535966 common_tool-0.0.6/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      317 2022-07-13 10:19:33.000000 common_tool-0.0.6/README.md
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 09:14:05.534775 common_tool-0.0.6/common_tool/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2022-07-13 09:32:57.000000 common_tool-0.0.6/common_tool/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)      622 2022-07-13 09:32:57.000000 common_tool-0.0.6/common_tool/datetime.py
+-rw-r--r--   0 donghao    (501) staff       (20)     3653 2023-06-05 09:13:08.000000 common_tool-0.0.6/common_tool/enum.py
+-rw-r--r--   0 donghao    (501) staff       (20)     1464 2023-06-05 01:21:44.000000 common_tool-0.0.6/common_tool/http.py
+-rw-r--r--   0 donghao    (501) staff       (20)      246 2023-05-19 06:58:46.000000 common_tool-0.0.6/common_tool/loggers.py
+-rw-r--r--   0 donghao    (501) staff       (20)      476 2022-07-13 09:32:57.000000 common_tool-0.0.6/common_tool/math.py
+-rw-r--r--   0 donghao    (501) staff       (20)     1162 2022-07-13 09:32:57.000000 common_tool-0.0.6/common_tool/random.py
+-rw-r--r--   0 donghao    (501) staff       (20)      402 2022-07-13 09:32:57.000000 common_tool-0.0.6/common_tool/token.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 09:14:05.535446 common_tool-0.0.6/common_tool.egg-info/
+-rw-r--r--   0 donghao    (501) staff       (20)      601 2023-06-05 09:14:05.000000 common_tool-0.0.6/common_tool.egg-info/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      391 2023-06-05 09:14:05.000000 common_tool-0.0.6/common_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-05 09:14:05.000000 common_tool-0.0.6/common_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       12 2023-06-05 09:14:05.000000 common_tool-0.0.6/common_tool.egg-info/requires.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       17 2023-06-05 09:14:05.000000 common_tool-0.0.6/common_tool.egg-info/top_level.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-05 09:14:05.536164 common_tool-0.0.6/setup.cfg
+-rw-r--r--   0 donghao    (501) staff       (20)      714 2023-06-05 09:13:16.000000 common_tool-0.0.6/setup.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 09:14:05.535552 common_tool-0.0.6/test/
+-rw-r--r--   0 donghao    (501) staff       (20)       97 2022-07-13 10:03:42.000000 common_tool-0.0.6/test/__init__.py
```

### Comparing `common_tool-0.0.5/LICENSE` & `common_tool-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.5/PKG-INFO` & `common_tool-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common_tool
-Version: 0.0.5
+Version: 0.0.6
 Summary: Basic toolkit packaging
 Home-page: https://github.com/RelaxedDong/dh_common
 Author: donghao
 Author-email: is_simple@163.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `common_tool-0.0.5/common_tool/datetime.py` & `common_tool-0.0.6/common_tool/datetime.py`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.5/common_tool/enum.py` & `common_tool-0.0.6/common_tool/enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,7 +125,13 @@
     def __iter__(self):
         # 当作为django.forms.fields.MultipleChoiceField的choices 要求实例可迭代
         return iter(self.choices)
 
     @classmethod
     def build_verbose_value(cls):
         return [{"verbose": item[1], "value": item[0]} for item in cls]
+
+    @classmethod
+    def get_choices(cls, choices_values=None):
+        if choices_values is None:
+            return cls.choices
+        return [choice for choice in cls.choices if choice[0] in choices_values]
```

### Comparing `common_tool-0.0.5/common_tool/http.py` & `common_tool-0.0.6/common_tool/http.py`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.5/common_tool/random.py` & `common_tool-0.0.6/common_tool/random.py`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.5/common_tool.egg-info/PKG-INFO` & `common_tool-0.0.6/common_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tool
-Version: 0.0.5
+Version: 0.0.6
 Summary: Basic toolkit packaging
 Home-page: https://github.com/RelaxedDong/dh_common
 Author: donghao
 Author-email: is_simple@163.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `common_tool-0.0.5/setup.py` & `common_tool-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 AUTHOR = "donghao"
 AUTHOR_EMAIL = "is_simple@163.com"
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
```

