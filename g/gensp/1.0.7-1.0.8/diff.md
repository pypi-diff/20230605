# Comparing `tmp/gensp-1.0.7.tar.gz` & `tmp/gensp-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gensp-1.0.7.tar", last modified: Mon Jun  5 04:38:42 2023, max compression
+gzip compressed data, was "gensp-1.0.8.tar", last modified: Mon Jun  5 05:00:55 2023, max compression
```

## Comparing `gensp-1.0.7.tar` & `gensp-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:38:42.550785 gensp-1.0.7/
--rw-r--r--   0 liufangjing   (501) staff       (20)     1260 2023-06-05 04:38:42.550649 gensp-1.0.7/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)      824 2023-06-04 05:43:21.000000 gensp-1.0.7/README.md
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:38:42.549519 gensp-1.0.7/generateStoredProcedure/
--rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:38:09.000000 gensp-1.0.7/generateStoredProcedure/__init__.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     1739 2023-06-05 01:40:55.000000 gensp-1.0.7/generateStoredProcedure/backup.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     1902 2023-06-05 02:50:26.000000 gensp-1.0.7/generateStoredProcedure/compare.py
--rw-r--r--   0 liufangjing   (501) staff       (20)      748 2023-06-05 04:30:15.000000 gensp-1.0.7/generateStoredProcedure/login.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     1998 2023-06-05 03:15:51.000000 gensp-1.0.7/generateStoredProcedure/main.py
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:38:42.550119 gensp-1.0.7/gensp.egg-info/
--rw-r--r--   0 liufangjing   (501) staff       (20)     1260 2023-06-05 04:38:42.000000 gensp-1.0.7/gensp.egg-info/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)      364 2023-06-05 04:38:42.000000 gensp-1.0.7/gensp.egg-info/SOURCES.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-06-05 04:38:42.000000 gensp-1.0.7/gensp.egg-info/dependency_links.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       60 2023-06-05 04:38:42.000000 gensp-1.0.7/gensp.egg-info/entry_points.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       28 2023-06-05 04:38:42.000000 gensp-1.0.7/gensp.egg-info/requires.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       24 2023-06-05 04:38:42.000000 gensp-1.0.7/gensp.egg-info/top_level.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-06-05 04:38:42.550818 gensp-1.0.7/setup.cfg
--rw-r--r--   0 liufangjing   (501) staff       (20)     1589 2023-06-05 04:38:19.000000 gensp-1.0.7/setup.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 05:00:55.781206 gensp-1.0.8/
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1260 2023-06-05 05:00:55.781075 gensp-1.0.8/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)      824 2023-06-04 05:43:21.000000 gensp-1.0.8/README.md
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 05:00:55.780122 gensp-1.0.8/generateStoredProcedure/
+-rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:38:09.000000 gensp-1.0.8/generateStoredProcedure/__init__.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1739 2023-06-05 01:40:55.000000 gensp-1.0.8/generateStoredProcedure/backup.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1902 2023-06-05 02:50:26.000000 gensp-1.0.8/generateStoredProcedure/compare.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-06-05 04:51:56.000000 gensp-1.0.8/generateStoredProcedure/env.yaml
+-rw-r--r--   0 liufangjing   (501) staff       (20)      646 2023-06-05 04:52:00.000000 gensp-1.0.8/generateStoredProcedure/login.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1998 2023-06-05 03:15:51.000000 gensp-1.0.8/generateStoredProcedure/main.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-06-05 05:00:55.780885 gensp-1.0.8/gensp.egg-info/
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1260 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)      397 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/SOURCES.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/dependency_links.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       60 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/entry_points.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       28 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/requires.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       24 2023-06-05 05:00:55.000000 gensp-1.0.8/gensp.egg-info/top_level.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-06-05 05:00:55.781239 gensp-1.0.8/setup.cfg
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1719 2023-06-05 05:00:36.000000 gensp-1.0.8/setup.py
```

### Comparing `gensp-1.0.7/PKG-INFO` & `gensp-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensp
-Version: 1.0.7
+Version: 1.0.8
 Summary: 比对postgres数据库备份的数据，得出新增的存储过程
 Home-page: https://github.com/zerobyte1o1/gensp
 Author: byte
 Author-email: liufangjing_byte@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gensp-1.0.7/README.md` & `gensp-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gensp-1.0.7/generateStoredProcedure/backup.py` & `gensp-1.0.8/generateStoredProcedure/backup.py`

 * *Files identical despite different names*

### Comparing `gensp-1.0.7/generateStoredProcedure/compare.py` & `gensp-1.0.8/generateStoredProcedure/compare.py`

 * *Files identical despite different names*

### Comparing `gensp-1.0.7/generateStoredProcedure/login.py` & `gensp-1.0.8/generateStoredProcedure/login.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import yaml
-import os
+# import os
 from .backup import conn_postgres
 
 
 def login():
-    rootPath = os.path.dirname(os.path.abspath(__file__))
-    configPath = os.path.join(rootPath, "env.yaml")
-    with open(configPath, 'r') as f:
+    
+    with open('env.yaml', 'w+') as f:
         env = yaml.safe_load(f)
     host = input('\033[34m·\033[0mhost: ').strip()
     port = input('\033[34m·\033[0mport: ').strip()
     username = input('\033[34m·\033[0musername: ').strip()
     password = input('\033[34m·\033[0mpassword: ').strip()
     env['login']['host'] = host
     env['login']['port'] = port
```

### Comparing `gensp-1.0.7/generateStoredProcedure/main.py` & `gensp-1.0.8/generateStoredProcedure/main.py`

 * *Files identical despite different names*

### Comparing `gensp-1.0.7/gensp.egg-info/PKG-INFO` & `gensp-1.0.8/gensp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensp
-Version: 1.0.7
+Version: 1.0.8
 Summary: 比对postgres数据库备份的数据，得出新增的存储过程
 Home-page: https://github.com/zerobyte1o1/gensp
 Author: byte
 Author-email: liufangjing_byte@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gensp-1.0.7/setup.py` & `gensp-1.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gensp",  # 包的分发名称，使用字母、数字、_、-
-    version="1.0.7",  # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
+    version="1.0.8",  # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
     author="byte",  # 作者名字
     author_email="liufangjing_byte@163.com",  # 作者邮箱
     description="比对postgres数据库备份的数据，得出新增的存储过程",  # 包的简介描述
     long_description=long_description,  # 包的详细介绍(一般通过加载README.md)
     long_description_content_type="text/markdown",  # 和上条命令配合使用，声明加载的是markdown文件
     url="https://github.com/zerobyte1o1/gensp",  # 项目开源地址，我这里写的是同性交友官网，大家可以写自己真实的开源网址
     packages=setuptools.find_packages(),
     # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
     classifiers=[  # 关于包的其他元数据(metadata)
         "Programming Language :: Python :: 3",  # 该软件包仅与Python3兼容
         "License :: OSI Approved :: MIT License",  # 根据MIT许可证开源
         "Operating System :: OS Independent",  # 与操作系统无关
     ],
+
+    include_package_data=True,
     install_requires=['psycopg2==2.9.6', 'PyYAML==6.0'],  # 依赖的包
+    package_data={
+        'generateStoredProcedure': [
+            'env.yaml',
+        ],
+    },
     entry_points={
         'console_scripts': [
             'gensp = generateStoredProcedure.main:main'
         ]
     },
     python_requires='>=3'
 )
```

