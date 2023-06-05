# Comparing `tmp/highyield-1.1.0.tar.gz` & `tmp/highyield-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highyield-1.1.0.tar", last modified: Mon May 22 21:03:54 2023, max compression
+gzip compressed data, was "highyield-1.1.1.tar", last modified: Mon Jun  5 16:59:28 2023, max compression
```

## Comparing `highyield-1.1.0.tar` & `highyield-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-22 21:03:54.406242 highyield-1.1.0/
--rw-r--r--   0 v1         (502) wheel        (0)    35129 2023-01-06 21:21:15.000000 highyield-1.1.0/LICENSE
--rw-r--r--   0 v1         (502) wheel        (0)       29 2023-01-06 21:17:34.000000 highyield-1.1.0/MANIFEST.in
--rw-r--r--   0 v1         (502) wheel        (0)     1976 2023-05-22 21:03:54.406113 highyield-1.1.0/PKG-INFO
--rw-r--r--   0 v1         (502) wheel        (0)     1465 2023-05-22 20:36:54.000000 highyield-1.1.0/README.md
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-22 21:03:54.404762 highyield-1.1.0/highyield/
--rw-r--r--   0 v1         (502) wheel        (0)      198 2023-01-06 23:04:04.000000 highyield-1.1.0/highyield/__init__.py
--rw-r--r--   0 v1         (502) wheel        (0)     2138 2023-05-22 20:40:49.000000 highyield-1.1.0/highyield/basics.py
--rw-r--r--   0 v1         (502) wheel        (0)     3057 2023-05-22 20:51:33.000000 highyield-1.1.0/highyield/converter.py
--rw-r--r--   0 v1         (502) wheel        (0)     4256 2023-05-22 20:28:18.000000 highyield-1.1.0/highyield/copy.py
--rw-r--r--   0 v1         (502) wheel        (0)     1679 2023-05-22 20:28:31.000000 highyield-1.1.0/highyield/create.py
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-22 21:03:54.405820 highyield-1.1.0/highyield/data/
--rw-r--r--   0 v1         (502) wheel        (0)     1906 2023-01-03 23:05:21.000000 highyield-1.1.0/highyield/data/RR.csv
--rw-r--r--   0 v1         (502) wheel        (0)      346 2023-01-07 14:41:36.000000 highyield-1.1.0/highyield/imports.py
--rw-r--r--   0 v1         (502) wheel        (0)     1516 2023-05-22 20:28:53.000000 highyield-1.1.0/highyield/pdf.py
--rw-r--r--   0 v1         (502) wheel        (0)     1328 2023-05-22 20:29:48.000000 highyield-1.1.0/highyield/rename.py
--rw-r--r--   0 v1         (502) wheel        (0)     4842 2023-05-22 20:35:23.000000 highyield-1.1.0/highyield/tts.py
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-22 21:03:54.405703 highyield-1.1.0/highyield.egg-info/
--rw-r--r--   0 v1         (502) wheel        (0)     1976 2023-05-22 21:03:54.000000 highyield-1.1.0/highyield.egg-info/PKG-INFO
--rw-r--r--   0 v1         (502) wheel        (0)      449 2023-05-22 21:03:54.000000 highyield-1.1.0/highyield.egg-info/SOURCES.txt
--rw-r--r--   0 v1         (502) wheel        (0)        1 2023-05-22 21:03:54.000000 highyield-1.1.0/highyield.egg-info/dependency_links.txt
--rw-r--r--   0 v1         (502) wheel        (0)        1 2023-01-06 23:47:02.000000 highyield-1.1.0/highyield.egg-info/not-zip-safe
--rw-r--r--   0 v1         (502) wheel        (0)       39 2023-05-22 21:03:54.000000 highyield-1.1.0/highyield.egg-info/requires.txt
--rw-r--r--   0 v1         (502) wheel        (0)       10 2023-05-22 21:03:54.000000 highyield-1.1.0/highyield.egg-info/top_level.txt
--rw-r--r--   0 v1         (502) wheel        (0)      103 2023-01-06 22:57:09.000000 highyield-1.1.0/pyproject.toml
--rw-r--r--   0 v1         (502) wheel        (0)       38 2023-05-22 21:03:54.406278 highyield-1.1.0/setup.cfg
--rw-r--r--   0 v1         (502) wheel        (0)     1013 2023-05-22 20:37:41.000000 highyield-1.1.0/setup.py
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-06-05 16:59:28.461531 highyield-1.1.1/
+-rw-r--r--   0 v1         (502) wheel        (0)    35129 2023-01-06 21:21:15.000000 highyield-1.1.1/LICENSE
+-rw-r--r--   0 v1         (502) wheel        (0)       29 2023-01-06 21:17:34.000000 highyield-1.1.1/MANIFEST.in
+-rw-r--r--   0 v1         (502) wheel        (0)     2074 2023-06-05 16:59:28.461359 highyield-1.1.1/PKG-INFO
+-rw-r--r--   0 v1         (502) wheel        (0)     1563 2023-06-05 01:08:22.000000 highyield-1.1.1/README.md
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-06-05 16:59:28.459658 highyield-1.1.1/highyield/
+-rw-r--r--   0 v1         (502) wheel        (0)      448 2023-06-05 00:57:05.000000 highyield-1.1.1/highyield/__init__.py
+-rw-r--r--   0 v1         (502) wheel        (0)     2138 2023-05-22 20:40:49.000000 highyield-1.1.1/highyield/basics.py
+-rw-r--r--   0 v1         (502) wheel        (0)     3057 2023-05-22 20:51:33.000000 highyield-1.1.1/highyield/converter.py
+-rw-r--r--   0 v1         (502) wheel        (0)     4256 2023-05-22 20:28:18.000000 highyield-1.1.1/highyield/copy.py
+-rw-r--r--   0 v1         (502) wheel        (0)     1679 2023-05-22 20:28:31.000000 highyield-1.1.1/highyield/create.py
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-06-05 16:59:28.461031 highyield-1.1.1/highyield/data/
+-rw-r--r--   0 v1         (502) wheel        (0)     1906 2023-01-03 23:05:21.000000 highyield-1.1.1/highyield/data/RR.csv
+-rw-r--r--   0 v1         (502) wheel        (0)      683 2023-06-05 00:37:25.000000 highyield-1.1.1/highyield/ds.py
+-rw-r--r--   0 v1         (502) wheel        (0)      346 2023-01-07 14:41:36.000000 highyield-1.1.1/highyield/imports.py
+-rw-r--r--   0 v1         (502) wheel        (0)     1516 2023-05-22 20:28:53.000000 highyield-1.1.1/highyield/pdf.py
+-rw-r--r--   0 v1         (502) wheel        (0)     1328 2023-05-22 20:29:48.000000 highyield-1.1.1/highyield/rename.py
+-rw-r--r--   0 v1         (502) wheel        (0)     4842 2023-05-22 20:35:23.000000 highyield-1.1.1/highyield/tts.py
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-06-05 16:59:28.460879 highyield-1.1.1/highyield.egg-info/
+-rw-r--r--   0 v1         (502) wheel        (0)     2074 2023-06-05 16:59:28.000000 highyield-1.1.1/highyield.egg-info/PKG-INFO
+-rw-r--r--   0 v1         (502) wheel        (0)      465 2023-06-05 16:59:28.000000 highyield-1.1.1/highyield.egg-info/SOURCES.txt
+-rw-r--r--   0 v1         (502) wheel        (0)        1 2023-06-05 16:59:28.000000 highyield-1.1.1/highyield.egg-info/dependency_links.txt
+-rw-r--r--   0 v1         (502) wheel        (0)        1 2023-01-06 23:47:02.000000 highyield-1.1.1/highyield.egg-info/not-zip-safe
+-rw-r--r--   0 v1         (502) wheel        (0)       47 2023-06-05 16:59:28.000000 highyield-1.1.1/highyield.egg-info/requires.txt
+-rw-r--r--   0 v1         (502) wheel        (0)       10 2023-06-05 16:59:28.000000 highyield-1.1.1/highyield.egg-info/top_level.txt
+-rw-r--r--   0 v1         (502) wheel        (0)      103 2023-01-06 22:57:09.000000 highyield-1.1.1/pyproject.toml
+-rw-r--r--   0 v1         (502) wheel        (0)       38 2023-06-05 16:59:28.461572 highyield-1.1.1/setup.cfg
+-rw-r--r--   0 v1         (502) wheel        (0)     1032 2023-06-05 00:37:45.000000 highyield-1.1.1/setup.py
```

### Comparing `highyield-1.1.0/LICENSE` & `highyield-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `highyield-1.1.0/PKG-INFO` & `highyield-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highyield
-Version: 1.1.0
+Version: 1.1.1
 Summary: Collection of high-yield functions intended to simplify and automate specific tasks.
 Home-page: https://github.com/kenf1/High-Yield
 Author: KF
 Author-email: kenfv1@outlook.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -37,17 +37,18 @@
 python3 -m pip install highyield
 ```
 
 ### Dependencies
 
 The table below lists the dependencies for each module within this package:
 
-| Module    | Packages             |
-| --------- | -------------------- |
-| basics    | os, requests         |
-| converter | os, pandas, docx2pdf |
-| copy      | os, shutil, pandas   |
-| create    | os, shutil           |
-| imports   | importlib, pandas    |
-| pdf       | os, pypdf            |
-| rename    | os, re               |
-| tts       | pyttsx3, pandas      |
+|Module|Module description|Dependencies|
+|---|---|---|
+|basics|Automation tasks|os, requests|
+|converter|Convert from 1 file format to another|os, pandas, docx2pdf|
+|copy|Copy & paste local files|os, shutil, pandas|
+|create|Create folder(s) + structure from template|os, shutil|
+|ds|Data Science|seaborn|
+|imports|Import packaged files|importlib, pandas|
+|pdf|Work with pdf files|os, pypdf|
+|rename|Automate renaming files|os, re|
+|tts|Text to speech|pyttsx3, pandas|
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: highyield Version: 1.1.0 Summary: Collection of
+Metadata-Version: 2.1 Name: highyield Version: 1.1.1 Summary: Collection of
 high-yield functions intended to simplify and automate specific tasks. Home-
 page: https://github.com/kenf1/High-Yield Author: KF Author-email:
 kenfv1@outlook.com License: GPLv3 Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE ## highyield
 [https://raw.githubusercontent.com/kenf1/Rendered/main/Hex_Sticker/High-
@@ -13,11 +13,14 @@
 Rendered/highyield%20Documentation/) `highyield` is a Python package containing
 a collection of high-yield functions (grouped by modules) intended to simplify
 and automate specific tasks. This package requires Python >= 3.8 due to
 reliance on [`pandas` package](https://pypi.org/project/pandas/). ### Install
 To install, open the terminal and type in the following. For Windows and Linux:
 ```{python} pip install highyield ``` For macOS: ```{python} python3 -m pip
 install highyield ``` ### Dependencies The table below lists the dependencies
-for each module within this package: | Module | Packages | | --------- | ------
--------------- | | basics | os, requests | | converter | os, pandas, docx2pdf |
-| copy | os, shutil, pandas | | create | os, shutil | | imports | importlib,
-pandas | | pdf | os, pypdf | | rename | os, re | | tts | pyttsx3, pandas |
+for each module within this package: |Module|Module description|Dependencies|
+|---|---|---| |basics|Automation tasks|os, requests| |converter|Convert from 1
+file format to another|os, pandas, docx2pdf| |copy|Copy & paste local files|os,
+shutil, pandas| |create|Create folder(s) + structure from template|os, shutil|
+|ds|Data Science|seaborn| |imports|Import packaged files|importlib, pandas|
+|pdf|Work with pdf files|os, pypdf| |rename|Automate renaming files|os, re|
+|tts|Text to speech|pyttsx3, pandas|
```

### Comparing `highyield-1.1.0/README.md` & `highyield-1.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 python3 -m pip install highyield
 ```
 
 ### Dependencies
 
 The table below lists the dependencies for each module within this package:
 
-| Module    | Packages             |
-| --------- | -------------------- |
-| basics    | os, requests         |
-| converter | os, pandas, docx2pdf |
-| copy      | os, shutil, pandas   |
-| create    | os, shutil           |
-| imports   | importlib, pandas    |
-| pdf       | os, pypdf            |
-| rename    | os, re               |
-| tts       | pyttsx3, pandas      |
+|Module|Module description|Dependencies|
+|---|---|---|
+|basics|Automation tasks|os, requests|
+|converter|Convert from 1 file format to another|os, pandas, docx2pdf|
+|copy|Copy & paste local files|os, shutil, pandas|
+|create|Create folder(s) + structure from template|os, shutil|
+|ds|Data Science|seaborn|
+|imports|Import packaged files|importlib, pandas|
+|pdf|Work with pdf files|os, pypdf|
+|rename|Automate renaming files|os, re|
+|tts|Text to speech|pyttsx3, pandas|
```

#### html2text {}

```diff
@@ -6,12 +6,15 @@
 (https://kenf1.github.io/Rendered/highyield%20Documentation/) `highyield` is a
 Python package containing a collection of high-yield functions (grouped by
 modules) intended to simplify and automate specific tasks. This package
 requires Python >= 3.8 due to reliance on [`pandas` package](https://pypi.org/
 project/pandas/). ### Install To install, open the terminal and type in the
 following. For Windows and Linux: ```{python} pip install highyield ``` For
 macOS: ```{python} python3 -m pip install highyield ``` ### Dependencies The
-table below lists the dependencies for each module within this package: |
-Module | Packages | | --------- | -------------------- | | basics | os,
-requests | | converter | os, pandas, docx2pdf | | copy | os, shutil, pandas | |
-create | os, shutil | | imports | importlib, pandas | | pdf | os, pypdf | |
-rename | os, re | | tts | pyttsx3, pandas |
+table below lists the dependencies for each module within this package:
+|Module|Module description|Dependencies| |---|---|---| |basics|Automation
+tasks|os, requests| |converter|Convert from 1 file format to another|os,
+pandas, docx2pdf| |copy|Copy & paste local files|os, shutil, pandas|
+|create|Create folder(s) + structure from template|os, shutil| |ds|Data
+Science|seaborn| |imports|Import packaged files|importlib, pandas| |pdf|Work
+with pdf files|os, pypdf| |rename|Automate renaming files|os, re| |tts|Text to
+speech|pyttsx3, pandas|
```

### Comparing `highyield-1.1.0/highyield/basics.py` & `highyield-1.1.1/highyield/basics.py`

 * *Files identical despite different names*

### Comparing `highyield-1.1.0/highyield/converter.py` & `highyield-1.1.1/highyield/converter.py`

 * *Files identical despite different names*

### Comparing `highyield-1.1.0/highyield/copy.py` & `highyield-1.1.1/highyield/copy.py`

 * *Files identical despite different names*

### Comparing `highyield-1.1.0/highyield/create.py` & `highyield-1.1.1/highyield/create.py`

 * *Files identical despite different names*

### Comparing `highyield-1.1.0/highyield/data/RR.csv` & `highyield-1.1.1/highyield/data/RR.csv`

 * *Files identical despite different names*

### Comparing `highyield-1.1.0/highyield/pdf.py` & `highyield-1.1.1/highyield/pdf.py`

 * *Files identical despite different names*

### Comparing `highyield-1.1.0/highyield/rename.py` & `highyield-1.1.1/highyield/rename.py`

 * *Files identical despite different names*

### Comparing `highyield-1.1.0/highyield/tts.py` & `highyield-1.1.1/highyield/tts.py`

 * *Files identical despite different names*

### Comparing `highyield-1.1.0/highyield.egg-info/PKG-INFO` & `highyield-1.1.1/highyield.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highyield
-Version: 1.1.0
+Version: 1.1.1
 Summary: Collection of high-yield functions intended to simplify and automate specific tasks.
 Home-page: https://github.com/kenf1/High-Yield
 Author: KF
 Author-email: kenfv1@outlook.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -37,17 +37,18 @@
 python3 -m pip install highyield
 ```
 
 ### Dependencies
 
 The table below lists the dependencies for each module within this package:
 
-| Module    | Packages             |
-| --------- | -------------------- |
-| basics    | os, requests         |
-| converter | os, pandas, docx2pdf |
-| copy      | os, shutil, pandas   |
-| create    | os, shutil           |
-| imports   | importlib, pandas    |
-| pdf       | os, pypdf            |
-| rename    | os, re               |
-| tts       | pyttsx3, pandas      |
+|Module|Module description|Dependencies|
+|---|---|---|
+|basics|Automation tasks|os, requests|
+|converter|Convert from 1 file format to another|os, pandas, docx2pdf|
+|copy|Copy & paste local files|os, shutil, pandas|
+|create|Create folder(s) + structure from template|os, shutil|
+|ds|Data Science|seaborn|
+|imports|Import packaged files|importlib, pandas|
+|pdf|Work with pdf files|os, pypdf|
+|rename|Automate renaming files|os, re|
+|tts|Text to speech|pyttsx3, pandas|
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: highyield Version: 1.1.0 Summary: Collection of
+Metadata-Version: 2.1 Name: highyield Version: 1.1.1 Summary: Collection of
 high-yield functions intended to simplify and automate specific tasks. Home-
 page: https://github.com/kenf1/High-Yield Author: KF Author-email:
 kenfv1@outlook.com License: GPLv3 Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE ## highyield
 [https://raw.githubusercontent.com/kenf1/Rendered/main/Hex_Sticker/High-
@@ -13,11 +13,14 @@
 Rendered/highyield%20Documentation/) `highyield` is a Python package containing
 a collection of high-yield functions (grouped by modules) intended to simplify
 and automate specific tasks. This package requires Python >= 3.8 due to
 reliance on [`pandas` package](https://pypi.org/project/pandas/). ### Install
 To install, open the terminal and type in the following. For Windows and Linux:
 ```{python} pip install highyield ``` For macOS: ```{python} python3 -m pip
 install highyield ``` ### Dependencies The table below lists the dependencies
-for each module within this package: | Module | Packages | | --------- | ------
--------------- | | basics | os, requests | | converter | os, pandas, docx2pdf |
-| copy | os, shutil, pandas | | create | os, shutil | | imports | importlib,
-pandas | | pdf | os, pypdf | | rename | os, re | | tts | pyttsx3, pandas |
+for each module within this package: |Module|Module description|Dependencies|
+|---|---|---| |basics|Automation tasks|os, requests| |converter|Convert from 1
+file format to another|os, pandas, docx2pdf| |copy|Copy & paste local files|os,
+shutil, pandas| |create|Create folder(s) + structure from template|os, shutil|
+|ds|Data Science|seaborn| |imports|Import packaged files|importlib, pandas|
+|pdf|Work with pdf files|os, pypdf| |rename|Automate renaming files|os, re|
+|tts|Text to speech|pyttsx3, pandas|
```

### Comparing `highyield-1.1.0/setup.py` & `highyield-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text()
 
 setup(name="highyield",
-      version="1.1.0",
+      version="1.1.1",
       description="Collection of high-yield functions intended to simplify and automate specific tasks.",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/kenf1/High-Yield",
       author="KF",
       author_email="kenfv1@outlook.com",
       license="GPLv3",
@@ -19,13 +19,14 @@
       classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent"
       ],
       install_requires=[
         "pandas",
+        "seaborn",
         "pyttsx3",
         "docx2pdf",
         "pypdf",
         "requests"
       ],
       zip_safe=False)
```

