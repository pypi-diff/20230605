# Comparing `tmp/pylychee-0.0.1.tar.gz` & `tmp/pylychee-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylychee-0.0.1.tar", last modified: Fri Jun  2 09:21:20 2023, max compression
+gzip compressed data, was "pylychee-0.0.2.tar", last modified: Mon Jun  5 02:22:05 2023, max compression
```

## Comparing `pylychee-0.0.1.tar` & `pylychee-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-02 09:21:20.211053 pylychee-0.0.1/
--rw-r--r--   0 chenhaiou   (501) staff       (20)     1062 2023-06-02 07:13:52.000000 pylychee-0.0.1/LICENSE
--rw-r--r--   0 chenhaiou   (501) staff       (20)      614 2023-06-02 09:21:20.210475 pylychee-0.0.1/PKG-INFO
--rw-r--r--   0 chenhaiou   (501) staff       (20)      135 2023-06-02 07:21:49.000000 pylychee-0.0.1/README.md
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-02 09:21:20.208009 pylychee-0.0.1/lychee/
--rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-02 07:26:50.000000 pylychee-0.0.1/lychee/__init__.py
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-02 09:21:20.208389 pylychee-0.0.1/lychee/apps/
--rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-02 07:27:02.000000 pylychee-0.0.1/lychee/apps/__init__.py
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-02 09:21:20.209722 pylychee-0.0.1/pylychee.egg-info/
--rw-r--r--   0 chenhaiou   (501) staff       (20)      614 2023-06-02 09:21:20.000000 pylychee-0.0.1/pylychee.egg-info/PKG-INFO
--rw-r--r--   0 chenhaiou   (501) staff       (20)      203 2023-06-02 09:21:20.000000 pylychee-0.0.1/pylychee.egg-info/SOURCES.txt
--rw-r--r--   0 chenhaiou   (501) staff       (20)        1 2023-06-02 09:21:20.000000 pylychee-0.0.1/pylychee.egg-info/dependency_links.txt
--rw-r--r--   0 chenhaiou   (501) staff       (20)        7 2023-06-02 09:21:20.000000 pylychee-0.0.1/pylychee.egg-info/top_level.txt
--rw-r--r--   0 chenhaiou   (501) staff       (20)      464 2023-06-02 09:16:18.000000 pylychee-0.0.1/pyproject.toml
--rw-r--r--   0 chenhaiou   (501) staff       (20)       38 2023-06-02 09:21:20.211185 pylychee-0.0.1/setup.cfg
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:22:05.011556 pylychee-0.0.2/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)     1062 2023-06-05 02:15:54.000000 pylychee-0.0.2/LICENSE
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      618 2023-06-05 02:22:05.011182 pylychee-0.0.2/PKG-INFO
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      140 2023-06-05 02:15:54.000000 pylychee-0.0.2/README.md
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:22:05.009215 pylychee-0.0.2/pylychee/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:15:54.000000 pylychee-0.0.2/pylychee/__init__.py
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:22:05.010778 pylychee-0.0.2/pylychee/apps/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:15:54.000000 pylychee-0.0.2/pylychee/apps/__init__.py
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:22:05.010456 pylychee-0.0.2/pylychee.egg-info/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      618 2023-06-05 02:22:04.000000 pylychee-0.0.2/pylychee.egg-info/PKG-INFO
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      207 2023-06-05 02:22:05.000000 pylychee-0.0.2/pylychee.egg-info/SOURCES.txt
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        1 2023-06-05 02:22:04.000000 pylychee-0.0.2/pylychee.egg-info/dependency_links.txt
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        9 2023-06-05 02:22:04.000000 pylychee-0.0.2/pylychee.egg-info/top_level.txt
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      465 2023-06-05 02:21:45.000000 pylychee-0.0.2/pyproject.toml
+-rw-r--r--   0 chenhaiou   (501) staff       (20)       38 2023-06-05 02:22:05.011670 pylychee-0.0.2/setup.cfg
```

### Comparing `pylychee-0.0.1/LICENSE` & `pylychee-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylychee-0.0.1/PKG-INFO` & `pylychee-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pylychee
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK合集
 Author-email: chenhaiou <haiou_chen@sina.cn>
 Project-URL: Homepage, https://github.com/MrLawes/pylychee
 Project-URL: Bug Tracker, https://github.com/MrLawes/lychee/pylychee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Lychee
-Lychee 是一个各种第三方 SDK 的集合体，省去了按照第三方接口文档对接的过程。谢谢你的关注。
+# Pylychee
+Pylychee 是一个各种第三方 SDK 的集合体，省去了按照第三方接口文档对接的过程。谢谢你的关注。
```

### Comparing `pylychee-0.0.1/pylychee.egg-info/PKG-INFO` & `pylychee-0.0.2/pylychee.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pylychee
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK合集
 Author-email: chenhaiou <haiou_chen@sina.cn>
 Project-URL: Homepage, https://github.com/MrLawes/pylychee
 Project-URL: Bug Tracker, https://github.com/MrLawes/lychee/pylychee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Lychee
-Lychee 是一个各种第三方 SDK 的集合体，省去了按照第三方接口文档对接的过程。谢谢你的关注。
+# Pylychee
+Pylychee 是一个各种第三方 SDK 的集合体，省去了按照第三方接口文档对接的过程。谢谢你的关注。
```

