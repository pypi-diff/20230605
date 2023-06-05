# Comparing `tmp/EdgeGPT-0.8.2.tar.gz` & `tmp/EdgeGPT-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.8.2.tar", last modified: Mon Jun  5 11:28:10 2023, max compression
+gzip compressed data, was "EdgeGPT-0.9.0.tar", last modified: Mon Jun  5 14:09:57 2023, max compression
```

## Comparing `EdgeGPT-0.8.2.tar` & `EdgeGPT-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:28:10.242767 EdgeGPT-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-05 11:27:40.000000 EdgeGPT-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 11:28:10.242767 EdgeGPT-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-05 11:28:10.242767 EdgeGPT-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-05 11:27:40.000000 EdgeGPT-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:28:10.242767 EdgeGPT-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:28:10.242767 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 11:28:10.000000 EdgeGPT-0.8.2/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34817 2023-06-05 11:27:40.000000 EdgeGPT-0.8.2/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-05 11:27:40.000000 EdgeGPT-0.8.2/src/EdgeUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 11:27:40.000000 EdgeGPT-0.8.2/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:09:57.142855 EdgeGPT-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 14:09:57.142855 EdgeGPT-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-05 14:09:56.000000 EdgeGPT-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-05 14:09:57.142855 EdgeGPT-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:09:57.138855 EdgeGPT-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:09:57.138855 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-05 14:09:57.000000 EdgeGPT-0.9.0/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/EdgeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:09:57.142855 EdgeGPT-0.9.0/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/conversation_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-05 14:09:16.000000 EdgeGPT-0.9.0/src/helpers/utilities.py
```

### Comparing `EdgeGPT-0.8.2/LICENSE` & `EdgeGPT-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.8.2/PKG-INFO` & `EdgeGPT-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.8.2
+Version: 0.9.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.2 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.9.0 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.8.2/README.md` & `EdgeGPT-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.8.2/setup.py` & `EdgeGPT-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.8.2",
+    version="0.9.0",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
@@ -25,20 +25,20 @@
         "console_scripts": [
             "edge-gpt = EdgeGPT:main",
             "edge-gpt-image = ImageGen:main",
         ],
     },
     install_requires=[
         "httpx[socks]>=0.24.0",
+        "aiohttp",
         "websockets",
         "rich",
         "certifi",
         "prompt_toolkit",
         "requests",
-        "aiofiles",
         "BingImageCreator>=0.3.0",
     ],
     long_description=Path.open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["EdgeGPT", "EdgeUtils", "ImageGen"],
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
```

### Comparing `EdgeGPT-0.8.2/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.9.0/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.8.2
+Version: 0.9.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.2 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.9.0 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.8.2/src/EdgeUtils.py` & `EdgeGPT-0.9.0/src/EdgeUtils.py`

 * *Files identical despite different names*

