# Comparing `tmp/google-csv-helper-1.0.3.tar.gz` & `tmp/google-csv-helper-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-csv-helper-1.0.3.tar", last modified: Mon Jun  5 15:41:36 2023, max compression
+gzip compressed data, was "google-csv-helper-1.0.4.tar", last modified: Mon Jun  5 15:48:17 2023, max compression
```

## Comparing `google-csv-helper-1.0.3.tar` & `google-csv-helper-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:41:36.795565 google-csv-helper-1.0.3/
--rw-r--r--   0 changyy    (501) admin       (80)     3091 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/.gitignore
--rw-r--r--   0 changyy    (501) admin       (80)     1070 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/LICENSE
--rw-r--r--   0 changyy    (501) admin       (80)      728 2023-06-05 15:41:36.795416 google-csv-helper-1.0.3/PKG-INFO
--rw-r--r--   0 changyy    (501) admin       (80)     3276 2023-06-05 14:36:39.000000 google-csv-helper-1.0.3/README.md
--rw-r--r--   0 changyy    (501) admin       (80)      177 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/build.py
-drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:41:36.794352 google-csv-helper-1.0.3/google_csv_helper/
--rw-r--r--   0 changyy    (501) admin       (80)      312 2023-06-05 14:08:43.000000 google-csv-helper-1.0.3/google_csv_helper/__init__.py
--rw-r--r--   0 changyy    (501) admin       (80)     7389 2023-06-05 15:36:22.000000 google-csv-helper-1.0.3/google_csv_helper/adsense_csv_helper.py
--rw-r--r--   0 changyy    (501) admin       (80)     2490 2023-06-05 14:13:19.000000 google-csv-helper-1.0.3/google_csv_helper/cmd.py
--rw-r--r--   0 changyy    (501) admin       (80)     2778 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/google_csv_helper/csv_common.py
--rw-r--r--   0 changyy    (501) admin       (80)     9958 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/google_csv_helper/csv_helper.py
-drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:41:36.795219 google-csv-helper-1.0.3/google_csv_helper.egg-info/
--rw-r--r--   0 changyy    (501) admin       (80)      728 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/PKG-INFO
--rw-r--r--   0 changyy    (501) admin       (80)      470 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/SOURCES.txt
--rw-r--r--   0 changyy    (501) admin       (80)        1 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/dependency_links.txt
--rw-r--r--   0 changyy    (501) admin       (80)       65 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/entry_points.txt
--rw-r--r--   0 changyy    (501) admin       (80)       91 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/requires.txt
--rw-r--r--   0 changyy    (501) admin       (80)       18 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/top_level.txt
--rw-r--r--   0 changyy    (501) admin       (80)       91 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/requirements.txt
--rw-r--r--   0 changyy    (501) admin       (80)       38 2023-06-05 15:41:36.795604 google-csv-helper-1.0.3/setup.cfg
--rw-r--r--   0 changyy    (501) admin       (80)     1735 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/setup.py
+drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:48:17.260429 google-csv-helper-1.0.4/
+-rw-r--r--   0 changyy    (501) admin       (80)     3091 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/.gitignore
+-rw-r--r--   0 changyy    (501) admin       (80)     1070 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/LICENSE
+-rw-r--r--   0 changyy    (501) admin       (80)     3899 2023-06-05 15:48:17.260277 google-csv-helper-1.0.4/PKG-INFO
+-rw-r--r--   0 changyy    (501) admin       (80)     3276 2023-06-05 14:36:39.000000 google-csv-helper-1.0.4/README.md
+-rw-r--r--   0 changyy    (501) admin       (80)      177 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/build.py
+drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:48:17.259291 google-csv-helper-1.0.4/google_csv_helper/
+-rw-r--r--   0 changyy    (501) admin       (80)      312 2023-06-05 15:44:58.000000 google-csv-helper-1.0.4/google_csv_helper/__init__.py
+-rw-r--r--   0 changyy    (501) admin       (80)     7389 2023-06-05 15:36:22.000000 google-csv-helper-1.0.4/google_csv_helper/adsense_csv_helper.py
+-rw-r--r--   0 changyy    (501) admin       (80)     2490 2023-06-05 14:13:19.000000 google-csv-helper-1.0.4/google_csv_helper/cmd.py
+-rw-r--r--   0 changyy    (501) admin       (80)     2778 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/google_csv_helper/csv_common.py
+-rw-r--r--   0 changyy    (501) admin       (80)     9958 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/google_csv_helper/csv_helper.py
+drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:48:17.260084 google-csv-helper-1.0.4/google_csv_helper.egg-info/
+-rw-r--r--   0 changyy    (501) admin       (80)     3899 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/PKG-INFO
+-rw-r--r--   0 changyy    (501) admin       (80)      470 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 changyy    (501) admin       (80)        1 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 changyy    (501) admin       (80)       65 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/entry_points.txt
+-rw-r--r--   0 changyy    (501) admin       (80)       91 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/requires.txt
+-rw-r--r--   0 changyy    (501) admin       (80)       18 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/top_level.txt
+-rw-r--r--   0 changyy    (501) admin       (80)       91 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/requirements.txt
+-rw-r--r--   0 changyy    (501) admin       (80)       38 2023-06-05 15:48:17.260472 google-csv-helper-1.0.4/setup.cfg
+-rw-r--r--   0 changyy    (501) admin       (80)     2064 2023-06-05 15:48:16.000000 google-csv-helper-1.0.4/setup.py
```

### Comparing `google-csv-helper-1.0.3/.gitignore` & `google-csv-helper-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.3/LICENSE` & `google-csv-helper-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.3/README.md` & `google-csv-helper-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.3/google_csv_helper/adsense_csv_helper.py` & `google-csv-helper-1.0.4/google_csv_helper/adsense_csv_helper.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.3/google_csv_helper/cmd.py` & `google-csv-helper-1.0.4/google_csv_helper/cmd.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.3/google_csv_helper/csv_common.py` & `google-csv-helper-1.0.4/google_csv_helper/csv_common.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.3/google_csv_helper/csv_helper.py` & `google-csv-helper-1.0.4/google_csv_helper/csv_helper.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.3/setup.py` & `google-csv-helper-1.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,28 +16,40 @@
                 VERSION = extractVersionInfo.group(1)
 
 PYTHON_REQUIRES = ">=3.10"
 URL = "https://github.com/changyy/google-csv-helper"
 DOWNLOAD_URL = "https://pypi.org/project/google-csv-helper/"
 DESCRIPTION = 'A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.'
 LONG_DESCRIPTION = DESCRIPTION
+LONG_DESCRIPTION_TYPE = 'text/plain'
+try:
+    with open(os.path.join(CWD, "README.md"), 'r') as f:
+        data = f.read()
+        if len(data) > 10:
+            LONG_DESCRIPTION = data
+            LONG_DESCRIPTION_TYPE = 'text/markdown'
+except Exception as e:
+    pass
+
+
 INSTALL_REQUIRES = ['pandas']
 try:
     with open(os.path.join(CWD, "requirements.txt"), 'r') as f:
         INSTALL_REQUIRES = [s.strip() for s in f.read().split("\n")]
 except Exception as e:
     pass
 
 setup(
     name="google-csv-helper", 
     version=VERSION,
     author="Yuan-Yi Chang",
     author_email="<changyy.csie@gmail.com>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
+    long_description_content_type=LONG_DESCRIPTION_TYPE,
     packages=find_packages(),
     install_requires=INSTALL_REQUIRES,
     keywords=['python', 'google', 'csv', 'adsense', 'admob', 'report'],
     python_requires=PYTHON_REQUIRES,
     url=URL,
     download_url=DOWNLOAD_URL,
     entry_points={
```

