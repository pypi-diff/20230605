# Comparing `tmp/git2pdf-0.1.6.tar.gz` & `tmp/git2pdf-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2pdf-0.1.6.tar", last modified: Mon Jun  5 15:18:50 2023, max compression
+gzip compressed data, was "git2pdf-0.1.7.tar", last modified: Mon Jun  5 18:08:18 2023, max compression
```

## Comparing `git2pdf-0.1.6.tar` & `git2pdf-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-05 15:18:50.727964 git2pdf-0.1.6/
--rw-r--r--   0 erguncan   (501) staff       (20)     1079 2023-06-04 20:31:55.000000 git2pdf-0.1.6/LICENSE.txt
--rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-05 15:18:50.728073 git2pdf-0.1.6/PKG-INFO
--rw-r--r--   0 erguncan   (501) staff       (20)      389 2023-06-04 20:32:44.000000 git2pdf-0.1.6/README.rst
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-05 15:18:50.726406 git2pdf-0.1.6/git2pdf/
--rw-r--r--   0 erguncan   (501) staff       (20)   757076 2023-06-04 01:56:54.000000 git2pdf-0.1.6/git2pdf/DejaVuSans.ttf
--rw-r--r--   0 erguncan   (501) staff       (20)     5387 2023-06-05 14:44:07.000000 git2pdf-0.1.6/git2pdf/main.py
-drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-05 15:18:50.727811 git2pdf-0.1.6/git2pdf.egg-info/
--rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-05 15:18:50.000000 git2pdf-0.1.6/git2pdf.egg-info/PKG-INFO
--rw-r--r--   0 erguncan   (501) staff       (20)      298 2023-06-05 15:18:50.000000 git2pdf-0.1.6/git2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-05 15:18:50.000000 git2pdf-0.1.6/git2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 erguncan   (501) staff       (20)       47 2023-06-05 15:18:50.000000 git2pdf-0.1.6/git2pdf.egg-info/entry_points.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1.6/git2pdf.egg-info/not-zip-safe
--rw-r--r--   0 erguncan   (501) staff       (20)       15 2023-06-05 15:18:50.000000 git2pdf-0.1.6/git2pdf.egg-info/requires.txt
--rw-r--r--   0 erguncan   (501) staff       (20)        8 2023-06-05 15:18:50.000000 git2pdf-0.1.6/git2pdf.egg-info/top_level.txt
--rw-r--r--   0 erguncan   (501) staff       (20)      713 2023-06-05 15:18:50.728551 git2pdf-0.1.6/setup.cfg
--rw-r--r--   0 erguncan   (501) staff       (20)      322 2023-06-05 15:18:49.000000 git2pdf-0.1.6/setup.py
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-05 18:08:18.388207 git2pdf-0.1.7/
+-rw-r--r--   0 erguncan   (501) staff       (20)     1079 2023-06-04 20:31:55.000000 git2pdf-0.1.7/LICENSE.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-05 18:08:18.388320 git2pdf-0.1.7/PKG-INFO
+-rw-r--r--   0 erguncan   (501) staff       (20)      389 2023-06-04 20:32:44.000000 git2pdf-0.1.7/README.rst
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-05 18:08:18.387043 git2pdf-0.1.7/git2pdf/
+-rw-r--r--   0 erguncan   (501) staff       (20)   757076 2023-06-04 01:56:54.000000 git2pdf-0.1.7/git2pdf/DejaVuSans.ttf
+-rw-r--r--   0 erguncan   (501) staff       (20)    11472 2023-06-05 18:05:36.000000 git2pdf-0.1.7/git2pdf/main.py
+drwxr-xr-x   0 erguncan   (501) staff       (20)        0 2023-06-05 18:08:18.388073 git2pdf-0.1.7/git2pdf.egg-info/
+-rw-r--r--   0 erguncan   (501) staff       (20)      936 2023-06-05 18:08:18.000000 git2pdf-0.1.7/git2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 erguncan   (501) staff       (20)      298 2023-06-05 18:08:18.000000 git2pdf-0.1.7/git2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-05 18:08:18.000000 git2pdf-0.1.7/git2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)       47 2023-06-05 18:08:18.000000 git2pdf-0.1.7/git2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        1 2023-06-04 20:34:17.000000 git2pdf-0.1.7/git2pdf.egg-info/not-zip-safe
+-rw-r--r--   0 erguncan   (501) staff       (20)       15 2023-06-05 18:08:18.000000 git2pdf-0.1.7/git2pdf.egg-info/requires.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)        8 2023-06-05 18:08:18.000000 git2pdf-0.1.7/git2pdf.egg-info/top_level.txt
+-rw-r--r--   0 erguncan   (501) staff       (20)      713 2023-06-05 18:08:18.388937 git2pdf-0.1.7/setup.cfg
+-rw-r--r--   0 erguncan   (501) staff       (20)      322 2023-06-05 18:07:35.000000 git2pdf-0.1.7/setup.py
```

### Comparing `git2pdf-0.1.6/LICENSE.txt` & `git2pdf-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git2pdf-0.1.6/PKG-INFO` & `git2pdf-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2pdf
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generate a PDF with the contents of files in a GitHub repository
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2pdf-0.1.6/git2pdf/DejaVuSans.ttf` & `git2pdf-0.1.7/git2pdf/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `git2pdf-0.1.6/git2pdf.egg-info/PKG-INFO` & `git2pdf-0.1.7/git2pdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2pdf
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generate a PDF with the contents of files in a GitHub repository
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2pdf-0.1.6/setup.cfg` & `git2pdf-0.1.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = git2pdf
-version = 0.1.6
+version = 0.1.7
 description = Generate a PDF with the contents of files in a GitHub repository
 long_description = file: README.rst
 license = MIT
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
```

