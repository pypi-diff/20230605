# Comparing `tmp/release-gitter-2.0.0.tar.gz` & `tmp/release-gitter-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "release-gitter-2.0.0.tar", last modified: Tue May 23 00:27:11 2023, max compression
+gzip compressed data, was "release-gitter-2.1.0.tar", last modified: Mon Jun  5 19:03:23 2023, max compression
```

## Comparing `release-gitter-2.0.0.tar` & `release-gitter-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:27:11.423229 release-gitter-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     1096 2023-05-23 00:26:39.000000 release-gitter-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5096 2023-05-23 00:27:11.423229 release-gitter-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4445 2023-05-23 00:26:39.000000 release-gitter-2.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)     4691 2023-05-23 00:26:39.000000 release-gitter-2.0.0/pseudo_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:27:11.423229 release-gitter-2.0.0/release_gitter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5096 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)    18254 2023-05-23 00:26:39.000000 release-gitter-2.0.0/release_gitter.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 00:27:11.423229 release-gitter-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1254 2023-05-23 00:26:39.000000 release-gitter-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:03:23.315115 release-gitter-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-06-05 19:02:51.000000 release-gitter-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-06-05 19:03:23.315115 release-gitter-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4445 2023-06-05 19:02:51.000000 release-gitter-2.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-06-05 19:02:51.000000 release-gitter-2.1.0/pseudo_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:03:23.315115 release-gitter-2.1.0/release_gitter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)    18423 2023-06-05 19:02:51.000000 release-gitter-2.1.0/release_gitter.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 19:03:23.315115 release-gitter-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-06-05 19:02:51.000000 release-gitter-2.1.0/setup.py
```

### Comparing `release-gitter-2.0.0/LICENSE` & `release-gitter-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `release-gitter-2.0.0/PKG-INFO` & `release-gitter-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: release-gitter
-Version: 2.0.0
+Version: 2.1.0
 Summary: Easily download releases from sites like Github and Gitea
 Home-page: https://git.iamthefij.com/iamthefij/release-gitter.git
 Download-URL: https://git.iamthefij.com/iamthefij/release-gitter.git/archive/master.tar.gz
 Author: iamthefij
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `release-gitter-2.0.0/README.md` & `release-gitter-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `release-gitter-2.0.0/pseudo_builder.py` & `release-gitter-2.1.0/pseudo_builder.py`

 * *Files identical despite different names*

### Comparing `release-gitter-2.0.0/release_gitter.egg-info/PKG-INFO` & `release-gitter-2.1.0/release_gitter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: release-gitter
-Version: 2.0.0
+Version: 2.1.0
 Summary: Easily download releases from sites like Github and Gitea
 Home-page: https://git.iamthefij.com/iamthefij/release-gitter.git
 Download-URL: https://git.iamthefij.com/iamthefij/release-gitter.git/archive/master.tar.gz
 Author: iamthefij
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `release-gitter-2.0.0/release_gitter.py` & `release-gitter-2.1.0/release_gitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -430,14 +430,15 @@
         "destination",
         metavar="DEST",
         nargs="?",
         type=Path,
         default=Path.cwd(),
         help="Destination directory. Defaults to current directory",
     )
+    parser.add_argument("-v", action="store_true", help="verbose logging")
     parser.add_argument(
         "--hostname",
         help="Git repository hostname",
     )
     parser.add_argument(
         "--owner",
         help="Owner of the repo. If not provided, it will be retrieved from the git url",
@@ -448,15 +449,15 @@
     )
     parser.add_argument(
         "--git-url",
         help="Git repository URL. Overrides `git remote` detection, but not command line options for hostname, owner, and repo",
     )
     parser.add_argument(
         "--version",
-        help="Release version to download. If not provied, it will look for project metadata",
+        help="Release version to download. If not provided, it will look for project metadata",
     )
     parser.add_argument(
         "--prerelease",
         action="store_true",
         help="Include pre-release versions in search",
     )
     parser.add_argument(
@@ -575,14 +576,17 @@
         release,
         args.format,
         version=args.version,
         system_mapping=args.map_system,
         arch_mapping=args.map_arch,
     )
 
+    if args.v:
+        print(f"Downloading {asset['name']} from release {release['name']}")
+
     if args.url_only:
         print(asset["browser_download_url"])
         return
 
     files = download_asset(
         asset,
         extract_files=args.extract_files,
```

### Comparing `release-gitter-2.0.0/setup.py` & `release-gitter-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="release-gitter",
-    version="2.0.0",
+    version="2.1.0",
     description="Easily download releases from sites like Github and Gitea",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.iamthefij.com/iamthefij/release-gitter.git",
     download_url=(
         "https://git.iamthefij.com/iamthefij/release-gitter.git/archive/master.tar.gz"
     ),
```

