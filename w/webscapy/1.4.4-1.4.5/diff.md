# Comparing `tmp/webscapy-1.4.4.tar.gz` & `tmp/webscapy-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscapy-1.4.4.tar", last modified: Wed May 31 07:22:49 2023, max compression
+gzip compressed data, was "webscapy-1.4.5.tar", last modified: Mon Jun  5 07:13:06 2023, max compression
```

## Comparing `webscapy-1.4.4.tar` & `webscapy-1.4.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 07:22:49.769841 webscapy-1.4.4/
--rw-rw-rw-   0        0        0     5648 2023-05-31 07:22:49.766813 webscapy-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     5353 2023-05-31 07:21:46.000000 webscapy-1.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 07:22:49.769841 webscapy-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-05-31 07:22:30.000000 webscapy-1.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:22:49.686485 webscapy-1.4.4/webscapy/
--rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.4.4/webscapy/__init__.py
--rw-rw-rw-   0        0        0     5412 2023-05-31 07:15:48.000000 webscapy-1.4.4/webscapy/webscapy.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:22:49.763784 webscapy-1.4.4/webscapy.egg-info/
--rw-rw-rw-   0        0        0     5648 2023-05-31 07:22:49.000000 webscapy-1.4.4/webscapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-31 07:22:49.000000 webscapy-1.4.4/webscapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 07:22:49.000000 webscapy-1.4.4/webscapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-31 07:22:49.000000 webscapy-1.4.4/webscapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-31 07:22:49.000000 webscapy-1.4.4/webscapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 07:13:06.572716 webscapy-1.4.5/
+-rw-rw-rw-   0        0        0     5648 2023-06-05 07:13:06.570702 webscapy-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5353 2023-05-31 07:21:46.000000 webscapy-1.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 07:13:06.572716 webscapy-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-06-05 07:12:10.000000 webscapy-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:13:06.518150 webscapy-1.4.5/webscapy/
+-rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.4.5/webscapy/__init__.py
+-rw-rw-rw-   0        0        0     5412 2023-05-31 07:15:48.000000 webscapy-1.4.5/webscapy/webscapy.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:13:06.566263 webscapy-1.4.5/webscapy.egg-info/
+-rw-rw-rw-   0        0        0     5648 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       38 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 07:13:06.000000 webscapy-1.4.5/webscapy.egg-info/top_level.txt
```

### Comparing `webscapy-1.4.4/PKG-INFO` & `webscapy-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscapy
-Version: 1.4.4
+Version: 1.4.5
 Summary: Selenium built for scraping instead of testing
 Author: Rahul Raj
 Project-URL: Documentation, https://pypi.org/project/webscapy/
 Project-URL: Source, https://pypi.org/project/webscapy/
 Description-Content-Type: text/markdown
 
 # Webscapy: Selenium Configured for Webscraping
```

### Comparing `webscapy-1.4.4/README.md` & `webscapy-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `webscapy-1.4.4/setup.py` & `webscapy-1.4.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="webscapy",
-    version="1.4.4",
+    version="1.4.5",
     description="Selenium built for scraping instead of testing",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Rahul Raj",
     packages=["webscapy"],
     zip_safe=False,
     project_urls={
         "Documentation": "https://pypi.org/project/webscapy/",
         "Source": "https://pypi.org/project/webscapy/",
-    }
+    },
+    install_requires=[
+        "selenium",
+        "webdriver_manager",
+        "uc-browser"
+    ]
 )
```

### Comparing `webscapy-1.4.4/webscapy/webscapy.py` & `webscapy-1.4.5/webscapy/webscapy.py`

 * *Files identical despite different names*

### Comparing `webscapy-1.4.4/webscapy.egg-info/PKG-INFO` & `webscapy-1.4.5/webscapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscapy
-Version: 1.4.4
+Version: 1.4.5
 Summary: Selenium built for scraping instead of testing
 Author: Rahul Raj
 Project-URL: Documentation, https://pypi.org/project/webscapy/
 Project-URL: Source, https://pypi.org/project/webscapy/
 Description-Content-Type: text/markdown
 
 # Webscapy: Selenium Configured for Webscraping
```

