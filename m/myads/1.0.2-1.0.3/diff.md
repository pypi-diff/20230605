# Comparing `tmp/myads-1.0.2.tar.gz` & `tmp/myads-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myads-1.0.2.tar", last modified: Mon Jun  5 01:14:49 2023, max compression
+gzip compressed data, was "myads-1.0.3.tar", last modified: Mon Jun  5 16:59:51 2023, max compression
```

## Comparing `myads-1.0.2.tar` & `myads-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.252777 myads-1.0.2/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4735 2023-06-05 01:14:49.252777 myads-1.0.2/PKG-INFO
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4241 2023-06-05 01:04:37.000000 myads-1.0.2/README.md
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      865 2023-06-05 01:13:52.000000 myads-1.0.2/pyproject.toml
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       38 2023-06-05 01:14:49.252777 myads-1.0.2/setup.cfg
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.248777 myads-1.0.2/src/
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.248777 myads-1.0.2/src/myads/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      769 2023-03-12 18:51:04.000000 myads-1.0.2/src/myads/__init__.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.252777 myads-1.0.2/src/myads/cite_tracker/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      614 2023-06-05 00:53:50.000000 myads-1.0.2/src/myads/cite_tracker/__init__.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     6631 2023-06-05 01:10:30.000000 myads-1.0.2/src/myads/cite_tracker/check.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2276 2023-04-19 21:46:53.000000 myads-1.0.2/src/myads/cite_tracker/report.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     3282 2023-06-05 00:51:56.000000 myads-1.0.2/src/myads/cite_tracker/users.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     9957 2023-04-19 21:46:45.000000 myads-1.0.2/src/myads/query.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.252777 myads-1.0.2/src/myads/scripts/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2620 2023-06-05 01:05:08.000000 myads-1.0.2/src/myads/scripts/myads.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 01:14:49.248777 myads-1.0.2/src/myads.egg-info/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4735 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/PKG-INFO
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      424 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/SOURCES.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        1 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/dependency_links.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       51 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/entry_points.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       30 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/requires.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        6 2023-06-05 01:14:49.000000 myads-1.0.2/src/myads.egg-info/top_level.txt
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4735 2023-06-05 16:59:51.447956 myads-1.0.3/PKG-INFO
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4241 2023-06-05 01:04:37.000000 myads-1.0.3/README.md
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      865 2023-06-05 16:58:49.000000 myads-1.0.3/pyproject.toml
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       38 2023-06-05 16:59:51.447956 myads-1.0.3/setup.cfg
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/src/
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/src/myads/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      769 2023-03-12 18:51:04.000000 myads-1.0.3/src/myads/__init__.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/src/myads/cite_tracker/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      614 2023-06-05 00:53:50.000000 myads-1.0.3/src/myads/cite_tracker/__init__.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     6631 2023-06-05 01:10:30.000000 myads-1.0.3/src/myads/cite_tracker/check.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2276 2023-04-19 21:46:53.000000 myads-1.0.3/src/myads/cite_tracker/report.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     3282 2023-06-05 00:51:56.000000 myads-1.0.3/src/myads/cite_tracker/users.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     9957 2023-04-19 21:46:45.000000 myads-1.0.3/src/myads/query.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/src/myads/scripts/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2622 2023-06-05 16:57:37.000000 myads-1.0.3/src/myads/scripts/myads.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/src/myads.egg-info/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4735 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/PKG-INFO
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      424 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/SOURCES.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        1 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/dependency_links.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       51 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/entry_points.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       30 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/requires.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        6 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/top_level.txt
```

### Comparing `myads-1.0.2/PKG-INFO` & `myads-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myads
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple ADS API query package and citation tracker
 Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/stuartmcalpine/myADS
 Project-URL: repository, https://github.com/stuartmcalpine/myADS
 Keywords: nasa-ads,citations,astronomy,ads,python,arxiv
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myads-1.0.2/README.md` & `myads-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `myads-1.0.2/pyproject.toml` & `myads-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 dependencies = [
     'requests',
     'toml',
     'tabulate>=0.9.0'
 ]
 requires-python = ">=3.7"
-version = "1.0.2"
+version = "1.0.3"
 keywords = ["nasa-ads", "citations", "astronomy", "ads", "python", "arxiv"]
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 
 [project.scripts]
 myads = "myads.scripts.myads:main"
```

### Comparing `myads-1.0.2/src/myads/__init__.py` & `myads-1.0.3/src/myads/__init__.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.2/src/myads/cite_tracker/__init__.py` & `myads-1.0.3/src/myads/cite_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.2/src/myads/cite_tracker/check.py` & `myads-1.0.3/src/myads/cite_tracker/check.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.2/src/myads/cite_tracker/report.py` & `myads-1.0.3/src/myads/cite_tracker/report.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.2/src/myads/cite_tracker/users.py` & `myads-1.0.3/src/myads/cite_tracker/users.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.2/src/myads/query.py` & `myads-1.0.3/src/myads/query.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.2/src/myads/scripts/myads.py` & `myads-1.0.3/src/myads/scripts/myads.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     # Check options
     check_parser.add_argument(
         "--verbose", help="True for more output", action="store_true"
     )
 
     args = parser.parse_args()
 
-    if args.subcommand == "user":
+    if args.subcommand == "author":
 
         # Add a user to the database
         if args.user_subparser == "add":
             cite_tracker.add_user()
 
         # Remove a user from the database
         elif args.user_subparser == "remove":
```

### Comparing `myads-1.0.2/src/myads.egg-info/PKG-INFO` & `myads-1.0.3/src/myads.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myads
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple ADS API query package and citation tracker
 Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/stuartmcalpine/myADS
 Project-URL: repository, https://github.com/stuartmcalpine/myADS
 Keywords: nasa-ads,citations,astronomy,ads,python,arxiv
 Classifier: Programming Language :: Python :: 3
```

