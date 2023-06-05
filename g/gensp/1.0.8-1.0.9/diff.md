# Comparing `tmp/gensp-1.0.8.tar.gz` & `tmp/gensp-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gensp-1.0.8.tar", last modified: Mon Jun  5 05:00:55 2023, max compression
+gzip compressed data, was "gensp-1.0.9.tar", last modified: Mon Jun  5 05:17:22 2023, max compression
```

## Comparing `gensp-1.0.8.tar` & `gensp-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 05:00:55.781206 gensp-1.0.8/
--rw-r--r--   0 liufangjing   (501) staff       (20)     1260 2023-06-05 05:00:55.781075 gensp-1.0.8/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)      824 2023-06-04 05:43:21.000000 gensp-1.0.8/README.md
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 05:00:55.780122 gensp-1.0.8/generateStoredProcedure/
--rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:38:09.000000 gensp-1.0.8/generateStoredProcedure/__init__.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     1739 2023-06-05 01:40:55.000000 gensp-1.0.8/generateStoredProcedure/backup.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     1902 2023-06-05 02:50:26.000000 gensp-1.0.8/generateStoredProcedure/compare.py
--rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:51:56.000000 gensp-1.0.8/generateStoredProcedure/env.yaml
--rw-r--r--   0 liufangjing   (501) staff       (20)      646 2023-06-05 04:52:00.000000 gensp-1.0.8/generateStoredProcedure/login.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     1998 2023-06-05 03:15:51.000000 gensp-1.0.8/generateStoredProcedure/main.py
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 05:00:55.780885 gensp-1.0.8/gensp.egg-info/
--rw-r--r--   0 liufangjing   (501) staff       (20)     1260 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)      397 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/SOURCES.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/dependency_links.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       60 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/entry_points.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       28 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/requires.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       24 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/top_level.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-06-05 05:00:55.781239 gensp-1.0.8/setup.cfg
--rw-r--r--   0 liufangjing   (501) staff       (20)     1719 2023-06-05 05:00:36.000000 gensp-1.0.8/setup.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 05:17:22.276197 gensp-1.0.9/
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1296 2023-06-05 05:17:22.276080 gensp-1.0.9/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)      824 2023-06-04 05:43:21.000000 gensp-1.0.9/README.md
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 05:17:22.274972 gensp-1.0.9/generateStoredProcedure/
+-rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:38:09.000000 gensp-1.0.9/generateStoredProcedure/__init__.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1739 2023-06-05 01:40:55.000000 gensp-1.0.9/generateStoredProcedure/backup.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1902 2023-06-05 02:50:26.000000 gensp-1.0.9/generateStoredProcedure/compare.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)      645 2023-06-05 05:16:04.000000 gensp-1.0.9/generateStoredProcedure/login.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1998 2023-06-05 03:15:51.000000 gensp-1.0.9/generateStoredProcedure/main.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 05:17:22.275920 gensp-1.0.9/gensp.egg-info/
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1296 2023-06-05 05:17:22.000000 gensp-1.0.9/gensp.egg-info/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)      364 2023-06-05 05:17:22.000000 gensp-1.0.9/gensp.egg-info/SOURCES.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-06-05 05:17:22.000000 gensp-1.0.9/gensp.egg-info/dependency_links.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       61 2023-06-05 05:17:22.000000 gensp-1.0.9/gensp.egg-info/entry_points.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       28 2023-06-05 05:17:22.000000 gensp-1.0.9/gensp.egg-info/requires.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       24 2023-06-05 05:17:22.000000 gensp-1.0.9/gensp.egg-info/top_level.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-06-05 05:17:22.276230 gensp-1.0.9/setup.cfg
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1719 2023-06-05 05:16:17.000000 gensp-1.0.9/setup.py
```

### Comparing `gensp-1.0.8/PKG-INFO` & `gensp-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: gensp
-Version: 1.0.8
+Version: 1.0.9
 Summary: 比对postgres数据库备份的数据，得出新增的存储过程
 Home-page: https://github.com/zerobyte1o1/gensp
 Author: byte
 Author-email: liufangjing_byte@163.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # gensp
@@ -37,7 +39,8 @@
 
 ## Release History
 
 * v0.0.1
     * ADD: Initial version
 
 #
+
```

### Comparing `gensp-1.0.8/README.md` & `gensp-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gensp-1.0.8/generateStoredProcedure/backup.py` & `gensp-1.0.9/generateStoredProcedure/backup.py`

 * *Files identical despite different names*

### Comparing `gensp-1.0.8/generateStoredProcedure/compare.py` & `gensp-1.0.9/generateStoredProcedure/compare.py`

 * *Files identical despite different names*

### Comparing `gensp-1.0.8/generateStoredProcedure/login.py` & `gensp-1.0.9/generateStoredProcedure/login.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import yaml
 # import os
 from .backup import conn_postgres
 
 
 def login():
     
-    with open('env.yaml', 'w+') as f:
+    with open('env.yaml', 'r') as f:
         env = yaml.safe_load(f)
     host = input('\033[34m·\033[0mhost: ').strip()
     port = input('\033[34m·\033[0mport: ').strip()
     username = input('\033[34m·\033[0musername: ').strip()
     password = input('\033[34m·\033[0mpassword: ').strip()
     env['login']['host'] = host
     env['login']['port'] = port
```

### Comparing `gensp-1.0.8/generateStoredProcedure/main.py` & `gensp-1.0.9/generateStoredProcedure/main.py`

 * *Files identical despite different names*

### Comparing `gensp-1.0.8/gensp.egg-info/PKG-INFO` & `gensp-1.0.9/gensp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: gensp
-Version: 1.0.8
+Version: 1.0.9
 Summary: 比对postgres数据库备份的数据，得出新增的存储过程
 Home-page: https://github.com/zerobyte1o1/gensp
 Author: byte
 Author-email: liufangjing_byte@163.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # gensp
@@ -37,7 +39,8 @@
 
 ## Release History
 
 * v0.0.1
     * ADD: Initial version
 
 #
+
```

### Comparing `gensp-1.0.8/setup.py` & `gensp-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gensp",  # 包的分发名称，使用字母、数字、_、-
-    version="1.0.8",  # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
+    version="1.0.9",  # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
     author="byte",  # 作者名字
     author_email="liufangjing_byte@163.com",  # 作者邮箱
     description="比对postgres数据库备份的数据，得出新增的存储过程",  # 包的简介描述
     long_description=long_description,  # 包的详细介绍(一般通过加载README.md)
     long_description_content_type="text/markdown",  # 和上条命令配合使用，声明加载的是markdown文件
     url="https://github.com/zerobyte1o1/gensp",  # 项目开源地址，我这里写的是同性交友官网，大家可以写自己真实的开源网址
     packages=setuptools.find_packages(),
```

