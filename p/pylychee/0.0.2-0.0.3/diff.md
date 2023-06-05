# Comparing `tmp/pylychee-0.0.2.tar.gz` & `tmp/pylychee-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylychee-0.0.2.tar", last modified: Mon Jun  5 02:22:05 2023, max compression
+gzip compressed data, was "pylychee-0.0.3.tar", last modified: Mon Jun  5 05:46:23 2023, max compression
```

## Comparing `pylychee-0.0.2.tar` & `pylychee-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:22:05.011556 pylychee-0.0.2/
--rw-r--r--   0 chenhaiou   (501) staff       (20)     1062 2023-06-05 02:15:54.000000 pylychee-0.0.2/LICENSE
--rw-r--r--   0 chenhaiou   (501) staff       (20)      618 2023-06-05 02:22:05.011182 pylychee-0.0.2/PKG-INFO
--rw-r--r--   0 chenhaiou   (501) staff       (20)      140 2023-06-05 02:15:54.000000 pylychee-0.0.2/README.md
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:22:05.009215 pylychee-0.0.2/pylychee/
--rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:15:54.000000 pylychee-0.0.2/pylychee/__init__.py
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:22:05.010778 pylychee-0.0.2/pylychee/apps/
--rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:15:54.000000 pylychee-0.0.2/pylychee/apps/__init__.py
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:22:05.010456 pylychee-0.0.2/pylychee.egg-info/
--rw-r--r--   0 chenhaiou   (501) staff       (20)      618 2023-06-05 02:22:04.000000 pylychee-0.0.2/pylychee.egg-info/PKG-INFO
--rw-r--r--   0 chenhaiou   (501) staff       (20)      207 2023-06-05 02:22:05.000000 pylychee-0.0.2/pylychee.egg-info/SOURCES.txt
--rw-r--r--   0 chenhaiou   (501) staff       (20)        1 2023-06-05 02:22:04.000000 pylychee-0.0.2/pylychee.egg-info/dependency_links.txt
--rw-r--r--   0 chenhaiou   (501) staff       (20)        9 2023-06-05 02:22:04.000000 pylychee-0.0.2/pylychee.egg-info/top_level.txt
--rw-r--r--   0 chenhaiou   (501) staff       (20)      465 2023-06-05 02:21:45.000000 pylychee-0.0.2/pyproject.toml
--rw-r--r--   0 chenhaiou   (501) staff       (20)       38 2023-06-05 02:22:05.011670 pylychee-0.0.2/setup.cfg
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 05:46:23.801484 pylychee-0.0.3/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)     1062 2023-06-05 02:15:54.000000 pylychee-0.0.3/LICENSE
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      618 2023-06-05 05:46:23.800882 pylychee-0.0.3/PKG-INFO
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      140 2023-06-05 02:15:54.000000 pylychee-0.0.3/README.md
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 05:46:23.796206 pylychee-0.0.3/pylychee/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:15:54.000000 pylychee-0.0.3/pylychee/__init__.py
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 05:46:23.798106 pylychee-0.0.3/pylychee/apps/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:15:54.000000 pylychee-0.0.3/pylychee/apps/__init__.py
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 05:46:23.799421 pylychee-0.0.3/pylychee/apps/feishu/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)     1013 2023-06-05 04:31:42.000000 pylychee-0.0.3/pylychee/apps/feishu/__init__.py
+-rw-r--r--   0 chenhaiou   (501) staff       (20)     1070 2023-06-05 03:34:28.000000 pylychee-0.0.3/pylychee/apps/feishu/messages.py
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 05:46:23.797703 pylychee-0.0.3/pylychee.egg-info/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      618 2023-06-05 05:46:23.000000 pylychee-0.0.3/pylychee.egg-info/PKG-INFO
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      273 2023-06-05 05:46:23.000000 pylychee-0.0.3/pylychee.egg-info/SOURCES.txt
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        1 2023-06-05 05:46:23.000000 pylychee-0.0.3/pylychee.egg-info/dependency_links.txt
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        9 2023-06-05 05:46:23.000000 pylychee-0.0.3/pylychee.egg-info/top_level.txt
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      572 2023-06-05 05:46:12.000000 pylychee-0.0.3/pyproject.toml
+-rw-r--r--   0 chenhaiou   (501) staff       (20)       38 2023-06-05 05:46:23.801607 pylychee-0.0.3/setup.cfg
```

### Comparing `pylychee-0.0.2/LICENSE` & `pylychee-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylychee-0.0.2/PKG-INFO` & `pylychee-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylychee
-Version: 0.0.2
+Version: 0.0.3
 Summary: SDK合集
 Author-email: chenhaiou <haiou_chen@sina.cn>
 Project-URL: Homepage, https://github.com/MrLawes/pylychee
 Project-URL: Bug Tracker, https://github.com/MrLawes/lychee/pylychee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pylychee-0.0.2/pylychee.egg-info/PKG-INFO` & `pylychee-0.0.3/pylychee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylychee
-Version: 0.0.2
+Version: 0.0.3
 Summary: SDK合集
 Author-email: chenhaiou <haiou_chen@sina.cn>
 Project-URL: Homepage, https://github.com/MrLawes/pylychee
 Project-URL: Bug Tracker, https://github.com/MrLawes/lychee/pylychee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

