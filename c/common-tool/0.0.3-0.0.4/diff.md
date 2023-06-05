# Comparing `tmp/common_tool-0.0.3.tar.gz` & `tmp/common_tool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_tool-0.0.3.tar", last modified: Wed Jul 13 10:18:01 2022, max compression
+gzip compressed data, was "common_tool-0.0.4.tar", last modified: Fri May 19 07:01:33 2023, max compression
```

## Comparing `common_tool-0.0.3.tar` & `common_tool-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2022-07-13 10:18:01.264375 common_tool-0.0.3/
--rw-r--r--   0 donghao    (501) staff       (20)     1065 2022-07-13 09:33:27.000000 common_tool-0.0.3/LICENSE
--rw-r--r--   0 donghao    (501) staff       (20)      686 2022-07-13 10:18:01.264248 common_tool-0.0.3/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      402 2022-07-13 10:17:28.000000 common_tool-0.0.3/README.md
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2022-07-13 10:18:01.263393 common_tool-0.0.3/common_tool/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2022-07-13 09:32:57.000000 common_tool-0.0.3/common_tool/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)      622 2022-07-13 09:32:57.000000 common_tool-0.0.3/common_tool/datetime.py
--rw-r--r--   0 donghao    (501) staff       (20)     3317 2022-07-13 09:32:57.000000 common_tool-0.0.3/common_tool/enum.py
--rw-r--r--   0 donghao    (501) staff       (20)     1464 2022-07-13 09:32:57.000000 common_tool-0.0.3/common_tool/http.py
--rw-r--r--   0 donghao    (501) staff       (20)      246 2022-07-13 09:32:57.000000 common_tool-0.0.3/common_tool/loggers.py
--rw-r--r--   0 donghao    (501) staff       (20)      476 2022-07-13 09:32:57.000000 common_tool-0.0.3/common_tool/math.py
--rw-r--r--   0 donghao    (501) staff       (20)     1162 2022-07-13 09:32:57.000000 common_tool-0.0.3/common_tool/random.py
--rw-r--r--   0 donghao    (501) staff       (20)      402 2022-07-13 09:32:57.000000 common_tool-0.0.3/common_tool/token.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2022-07-13 10:18:01.263878 common_tool-0.0.3/common_tool.egg-info/
--rw-r--r--   0 donghao    (501) staff       (20)      686 2022-07-13 10:18:01.000000 common_tool-0.0.3/common_tool.egg-info/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      391 2022-07-13 10:18:01.000000 common_tool-0.0.3/common_tool.egg-info/SOURCES.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2022-07-13 10:18:01.000000 common_tool-0.0.3/common_tool.egg-info/dependency_links.txt
--rw-r--r--   0 donghao    (501) staff       (20)       12 2022-07-13 10:18:01.000000 common_tool-0.0.3/common_tool.egg-info/requires.txt
--rw-r--r--   0 donghao    (501) staff       (20)       17 2022-07-13 10:18:01.000000 common_tool-0.0.3/common_tool.egg-info/top_level.txt
--rw-r--r--   0 donghao    (501) staff       (20)       38 2022-07-13 10:18:01.264420 common_tool-0.0.3/setup.cfg
--rw-r--r--   0 donghao    (501) staff       (20)      715 2022-07-13 10:17:57.000000 common_tool-0.0.3/setup.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2022-07-13 10:18:01.263969 common_tool-0.0.3/test/
--rw-r--r--   0 donghao    (501) staff       (20)       97 2022-07-13 10:03:42.000000 common_tool-0.0.3/test/__init__.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-05-19 07:01:33.676404 common_tool-0.0.4/
+-rw-r--r--   0 donghao    (501) staff       (20)     1065 2022-07-13 09:33:27.000000 common_tool-0.0.4/LICENSE
+-rw-r--r--   0 donghao    (501) staff       (20)      601 2023-05-19 07:01:33.676283 common_tool-0.0.4/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      317 2022-07-13 10:19:33.000000 common_tool-0.0.4/README.md
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-05-19 07:01:33.675344 common_tool-0.0.4/common_tool/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2022-07-13 09:32:57.000000 common_tool-0.0.4/common_tool/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)      622 2022-07-13 09:32:57.000000 common_tool-0.0.4/common_tool/datetime.py
+-rw-r--r--   0 donghao    (501) staff       (20)     3441 2023-05-19 06:59:19.000000 common_tool-0.0.4/common_tool/enum.py
+-rw-r--r--   0 donghao    (501) staff       (20)     1464 2022-07-13 09:32:57.000000 common_tool-0.0.4/common_tool/http.py
+-rw-r--r--   0 donghao    (501) staff       (20)      246 2023-05-19 06:58:46.000000 common_tool-0.0.4/common_tool/loggers.py
+-rw-r--r--   0 donghao    (501) staff       (20)      476 2022-07-13 09:32:57.000000 common_tool-0.0.4/common_tool/math.py
+-rw-r--r--   0 donghao    (501) staff       (20)     1162 2022-07-13 09:32:57.000000 common_tool-0.0.4/common_tool/random.py
+-rw-r--r--   0 donghao    (501) staff       (20)      402 2022-07-13 09:32:57.000000 common_tool-0.0.4/common_tool/token.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-05-19 07:01:33.675900 common_tool-0.0.4/common_tool.egg-info/
+-rw-r--r--   0 donghao    (501) staff       (20)      601 2023-05-19 07:01:33.000000 common_tool-0.0.4/common_tool.egg-info/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      391 2023-05-19 07:01:33.000000 common_tool-0.0.4/common_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-05-19 07:01:33.000000 common_tool-0.0.4/common_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       12 2023-05-19 07:01:33.000000 common_tool-0.0.4/common_tool.egg-info/requires.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       17 2023-05-19 07:01:33.000000 common_tool-0.0.4/common_tool.egg-info/top_level.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       38 2023-05-19 07:01:33.676454 common_tool-0.0.4/setup.cfg
+-rw-r--r--   0 donghao    (501) staff       (20)      714 2023-05-19 06:59:49.000000 common_tool-0.0.4/setup.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-05-19 07:01:33.676002 common_tool-0.0.4/test/
+-rw-r--r--   0 donghao    (501) staff       (20)       97 2022-07-13 10:03:42.000000 common_tool-0.0.4/test/__init__.py
```

### Comparing `common_tool-0.0.3/LICENSE` & `common_tool-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.3/PKG-INFO` & `common_tool-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common_tool
-Version: 0.0.3
+Version: 0.0.4
 Summary: Basic toolkit packaging
 Home-page: https://github.com/RelaxedDong/dh_common
 Author: donghao
 Author-email: is_simple@163.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,13 +17,9 @@
 
 Install common-tool with pip:
 
 ```bash
 python3 -m pip install --upgrade pip
 python3 -m pip install --upgrade common-tool
 ```
-upload package
-```python
-python3 setup.py sdist bdist_wheel
-twine upload dist/xxx
-```
+
```

### Comparing `common_tool-0.0.3/common_tool/datetime.py` & `common_tool-0.0.4/common_tool/datetime.py`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.3/common_tool/enum.py` & `common_tool-0.0.4/common_tool/enum.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,7 +121,11 @@
             if verbose == v:
                 return value
         raise KeyError(u'没有找到对应的verbose')
 
     def __iter__(self):
         # 当作为django.forms.fields.MultipleChoiceField的choices 要求实例可迭代
         return iter(self.choices)
+
+    @classmethod
+    def build_verbose_value(cls):
+        return [{"verbose": item[1], "value": item[0]} for item in cls]
```

### Comparing `common_tool-0.0.3/common_tool/http.py` & `common_tool-0.0.4/common_tool/http.py`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.3/common_tool/random.py` & `common_tool-0.0.4/common_tool/random.py`

 * *Files identical despite different names*

### Comparing `common_tool-0.0.3/common_tool.egg-info/PKG-INFO` & `common_tool-0.0.4/common_tool.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tool
-Version: 0.0.3
+Version: 0.0.4
 Summary: Basic toolkit packaging
 Home-page: https://github.com/RelaxedDong/dh_common
 Author: donghao
 Author-email: is_simple@163.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,13 +17,9 @@
 
 Install common-tool with pip:
 
 ```bash
 python3 -m pip install --upgrade pip
 python3 -m pip install --upgrade common-tool
 ```
-upload package
-```python
-python3 setup.py sdist bdist_wheel
-twine upload dist/xxx
-```
+
```

### Comparing `common_tool-0.0.3/setup.py` & `common_tool-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "1.2.50"
+VERSION = "0.0.4"
 AUTHOR = "donghao"
 AUTHOR_EMAIL = "is_simple@163.com"
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='common_tool',
-    version='0.0.3',
+    version=VERSION,
     author='donghao',
     author_email=AUTHOR_EMAIL,
     url="https://github.com/RelaxedDong/dh_common",
     description='Basic toolkit packaging',
     packages=find_packages(),
     install_requires=['six>=1.15.0'],
     long_description=long_description,  # 项目的描述 读取README.md文件的信息
```

