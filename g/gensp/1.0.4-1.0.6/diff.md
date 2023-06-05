# Comparing `tmp/gensp-1.0.4.tar.gz` & `tmp/gensp-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gensp-1.0.4.tar", last modified: Mon Jun  5 04:26:28 2023, max compression
+gzip compressed data, was "gensp-1.0.6.tar", last modified: Mon Jun  5 04:35:00 2023, max compression
```

## Comparing `gensp-1.0.4.tar` & `gensp-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:26:28.753991 gensp-1.0.4/
--rw-r--r--   0 liufangjing   (501) staff       (20)     1260 2023-06-05 04:26:28.753860 gensp-1.0.4/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)      824 2023-06-04 05:43:21.000000 gensp-1.0.4/README.md
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:26:28.752863 gensp-1.0.4/generateStoredProcedure/
--rw-r--r--   0 liufangjing   (501) staff       (20)       48 2023-06-03 09:32:55.000000 gensp-1.0.4/generateStoredProcedure/__init__.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     1739 2023-06-05 01:40:55.000000 gensp-1.0.4/generateStoredProcedure/backup.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     1902 2023-06-05 02:50:26.000000 gensp-1.0.4/generateStoredProcedure/compare.py
--rw-r--r--   0 liufangjing   (501) staff       (20)      629 2023-06-05 04:26:07.000000 gensp-1.0.4/generateStoredProcedure/login.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     1998 2023-06-05 03:15:51.000000 gensp-1.0.4/generateStoredProcedure/main.py
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:26:28.753699 gensp-1.0.4/gensp.egg-info/
--rw-r--r--   0 liufangjing   (501) staff       (20)     1260 2023-06-05 04:26:28.000000 gensp-1.0.4/gensp.egg-info/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)      364 2023-06-05 04:26:28.000000 gensp-1.0.4/gensp.egg-info/SOURCES.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-06-05 04:26:28.000000 gensp-1.0.4/gensp.egg-info/dependency_links.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       60 2023-06-05 04:26:28.000000 gensp-1.0.4/gensp.egg-info/entry_points.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       28 2023-06-05 04:26:28.000000 gensp-1.0.4/gensp.egg-info/requires.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       24 2023-06-05 04:26:28.000000 gensp-1.0.4/gensp.egg-info/top_level.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-06-05 04:26:28.754022 gensp-1.0.4/setup.cfg
--rw-r--r--   0 liufangjing   (501) staff       (20)     1589 2023-06-05 04:26:11.000000 gensp-1.0.4/setup.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:35:00.406195 gensp-1.0.6/
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1260 2023-06-05 04:35:00.406031 gensp-1.0.6/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)      824 2023-06-04 05:43:21.000000 gensp-1.0.6/README.md
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:35:00.405206 gensp-1.0.6/generateStoredProcedure/
+-rw-r--r--   0 liufangjing   (501) staff       (20)       48 2023-06-03 09:32:55.000000 gensp-1.0.6/generateStoredProcedure/__init__.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1739 2023-06-05 01:40:55.000000 gensp-1.0.6/generateStoredProcedure/backup.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1902 2023-06-05 02:50:26.000000 gensp-1.0.6/generateStoredProcedure/compare.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)      748 2023-06-05 04:30:15.000000 gensp-1.0.6/generateStoredProcedure/login.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1998 2023-06-05 03:15:51.000000 gensp-1.0.6/generateStoredProcedure/main.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:35:00.405863 gensp-1.0.6/gensp.egg-info/
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1260 2023-06-05 04:35:00.000000 gensp-1.0.6/gensp.egg-info/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)      364 2023-06-05 04:35:00.000000 gensp-1.0.6/gensp.egg-info/SOURCES.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-06-05 04:35:00.000000 gensp-1.0.6/gensp.egg-info/dependency_links.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       60 2023-06-05 04:35:00.000000 gensp-1.0.6/gensp.egg-info/entry_points.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       28 2023-06-05 04:35:00.000000 gensp-1.0.6/gensp.egg-info/requires.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       24 2023-06-05 04:35:00.000000 gensp-1.0.6/gensp.egg-info/top_level.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-06-05 04:35:00.406235 gensp-1.0.6/setup.cfg
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1589 2023-06-05 04:34:38.000000 gensp-1.0.6/setup.py
```

### Comparing `gensp-1.0.4/PKG-INFO` & `gensp-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensp
-Version: 1.0.4
+Version: 1.0.6
 Summary: 比对postgres数据库备份的数据，得出新增的存储过程
 Home-page: https://github.com/zerobyte1o1/gensp
 Author: byte
 Author-email: liufangjing_byte@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gensp-1.0.4/README.md` & `gensp-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gensp-1.0.4/generateStoredProcedure/backup.py` & `gensp-1.0.6/generateStoredProcedure/backup.py`

 * *Files identical despite different names*

### Comparing `gensp-1.0.4/generateStoredProcedure/compare.py` & `gensp-1.0.6/generateStoredProcedure/compare.py`

 * *Files identical despite different names*

### Comparing `gensp-1.0.4/generateStoredProcedure/login.py` & `gensp-1.0.6/generateStoredProcedure/login.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import yaml
+import os
 from .backup import conn_postgres
 
 
 def login():
-    with open('.env.yaml', 'r') as f:
+    rootPath = os.path.dirname(os.path.abspath(__file__))
+    configPath = os.path.join(rootPath, "env.yaml")
+    with open(configPath, 'r') as f:
         env = yaml.safe_load(f)
     host = input('\033[34m·\033[0mhost: ').strip()
     port = input('\033[34m·\033[0mport: ').strip()
     username = input('\033[34m·\033[0musername: ').strip()
     password = input('\033[34m·\033[0mpassword: ').strip()
     env['login']['host'] = host
     env['login']['port'] = port
```

### Comparing `gensp-1.0.4/generateStoredProcedure/main.py` & `gensp-1.0.6/generateStoredProcedure/main.py`

 * *Files identical despite different names*

### Comparing `gensp-1.0.4/gensp.egg-info/PKG-INFO` & `gensp-1.0.6/gensp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensp
-Version: 1.0.4
+Version: 1.0.6
 Summary: 比对postgres数据库备份的数据，得出新增的存储过程
 Home-page: https://github.com/zerobyte1o1/gensp
 Author: byte
 Author-email: liufangjing_byte@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gensp-1.0.4/setup.py` & `gensp-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gensp",  # 包的分发名称，使用字母、数字、_、-
-    version="1.0.4",  # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
+    version="1.0.6",  # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
     author="byte",  # 作者名字
     author_email="liufangjing_byte@163.com",  # 作者邮箱
     description="比对postgres数据库备份的数据，得出新增的存储过程",  # 包的简介描述
     long_description=long_description,  # 包的详细介绍(一般通过加载README.md)
     long_description_content_type="text/markdown",  # 和上条命令配合使用，声明加载的是markdown文件
     url="https://github.com/zerobyte1o1/gensp",  # 项目开源地址，我这里写的是同性交友官网，大家可以写自己真实的开源网址
     packages=setuptools.find_packages(),
```

