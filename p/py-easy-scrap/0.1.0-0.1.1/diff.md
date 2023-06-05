# Comparing `tmp/py-easy-scrap-0.1.0.tar.gz` & `tmp/py-easy-scrap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-easy-scrap-0.1.0.tar", last modified: Mon Jun  5 02:38:10 2023, max compression
+gzip compressed data, was "py-easy-scrap-0.1.1.tar", last modified: Mon Jun  5 02:51:02 2023, max compression
```

## Comparing `py-easy-scrap-0.1.0.tar` & `py-easy-scrap-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 02:38:10.322398 py-easy-scrap-0.1.0/
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     1077 2023-06-05 00:17:41.000000 py-easy-scrap-0.1.0/LICENSE
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2621 2023-06-05 02:38:10.322398 py-easy-scrap-0.1.0/PKG-INFO
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     1967 2023-06-05 02:37:47.000000 py-easy-scrap-0.1.0/README.md
-drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 02:38:10.322398 py-easy-scrap-0.1.0/py-easy-scrap/
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       61 2023-06-05 02:18:56.000000 py-easy-scrap-0.1.0/py-easy-scrap/__init__.py
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     4114 2023-06-05 02:26:32.000000 py-easy-scrap-0.1.0/py-easy-scrap/basic_functions.py
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     4587 2023-06-05 00:55:06.000000 py-easy-scrap-0.1.0/py-easy-scrap/web_scraping_functions.py
-drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 02:38:10.322398 py-easy-scrap-0.1.0/py_easy_scrap.egg-info/
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2621 2023-06-05 02:38:10.000000 py-easy-scrap-0.1.0/py_easy_scrap.egg-info/PKG-INFO
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      324 2023-06-05 02:38:10.000000 py-easy-scrap-0.1.0/py_easy_scrap.egg-info/SOURCES.txt
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)        1 2023-06-05 02:38:10.000000 py-easy-scrap-0.1.0/py_easy_scrap.egg-info/dependency_links.txt
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       18 2023-06-05 02:38:10.000000 py-easy-scrap-0.1.0/py_easy_scrap.egg-info/requires.txt
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       14 2023-06-05 02:38:10.000000 py-easy-scrap-0.1.0/py_easy_scrap.egg-info/top_level.txt
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      644 2023-06-05 01:08:29.000000 py-easy-scrap-0.1.0/pyproject.toml
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       38 2023-06-05 02:38:10.322398 py-easy-scrap-0.1.0/setup.cfg
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      806 2023-06-05 00:47:39.000000 py-easy-scrap-0.1.0/setup.py
+drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 02:51:02.707237 py-easy-scrap-0.1.1/
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     1077 2023-06-05 00:17:41.000000 py-easy-scrap-0.1.1/LICENSE
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2657 2023-06-05 02:51:02.707237 py-easy-scrap-0.1.1/PKG-INFO
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2003 2023-06-05 02:48:20.000000 py-easy-scrap-0.1.1/README.md
+drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 02:51:02.707237 py-easy-scrap-0.1.1/py_easy_scrap.egg-info/
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2657 2023-06-05 02:51:02.000000 py-easy-scrap-0.1.1/py_easy_scrap.egg-info/PKG-INFO
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      318 2023-06-05 02:51:02.000000 py-easy-scrap-0.1.1/py_easy_scrap.egg-info/SOURCES.txt
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)        1 2023-06-05 02:51:02.000000 py-easy-scrap-0.1.1/py_easy_scrap.egg-info/dependency_links.txt
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       18 2023-06-05 02:51:02.000000 py-easy-scrap-0.1.1/py_easy_scrap.egg-info/requires.txt
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       12 2023-06-05 02:51:02.000000 py-easy-scrap-0.1.1/py_easy_scrap.egg-info/top_level.txt
+drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 02:51:02.707237 py-easy-scrap-0.1.1/pyeasyscrap/
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       61 2023-06-05 02:18:56.000000 py-easy-scrap-0.1.1/pyeasyscrap/__init__.py
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     4114 2023-06-05 02:26:32.000000 py-easy-scrap-0.1.1/pyeasyscrap/basic_functions.py
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     4587 2023-06-05 00:55:06.000000 py-easy-scrap-0.1.1/pyeasyscrap/web_scraping_functions.py
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      644 2023-06-05 02:50:29.000000 py-easy-scrap-0.1.1/pyproject.toml
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       38 2023-06-05 02:51:02.707237 py-easy-scrap-0.1.1/setup.cfg
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      806 2023-06-05 00:47:39.000000 py-easy-scrap-0.1.1/setup.py
```

### Comparing `py-easy-scrap-0.1.0/LICENSE` & `py-easy-scrap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-easy-scrap-0.1.0/PKG-INFO` & `py-easy-scrap-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-easy-scrap
-Version: 0.1.0
+Version: 0.1.1
 Summary: A useful package for web scraping with Selenium
 Home-page: https://github.com/ygalvao/py-easy-scrap
 Author: Yuri Henrique Galvao
 Author-email: Yuri Henrique Galvao <yuri@galvao.ca>
 License: UNKNOWN
 Project-URL: Homepage, https://github.com/ygalvao/py-easy-scrap
 Project-URL: Bug Tracker, https://github.com/ygalvao/py-easy-scrap/issues
@@ -27,20 +27,20 @@
 ```bash
 pip install py-easy-scrap
 ```
 
 ## Requirements
 
 - Python 3.7 or higher
-- Selenium
+- Selenium, along with __GeckoDriver__ (Firefox)
 
 ## Usage
 
 ```python
-import py_easy_scrap as pes
+import pyeasyscrap as pes
 ```
 
 ### Get WebDriver
 
 ```python
 driver = get_webdriver(headless)
 ```
```

### Comparing `py-easy-scrap-0.1.0/README.md` & `py-easy-scrap-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 ```bash
 pip install py-easy-scrap
 ```
 
 ## Requirements
 
 - Python 3.7 or higher
-- Selenium
+- Selenium, along with __GeckoDriver__ (Firefox)
 
 ## Usage
 
 ```python
-import py_easy_scrap as pes
+import pyeasyscrap as pes
 ```
 
 ### Get WebDriver
 
 ```python
 driver = get_webdriver(headless)
 ```
```

### Comparing `py-easy-scrap-0.1.0/py-easy-scrap/basic_functions.py` & `py-easy-scrap-0.1.1/pyeasyscrap/basic_functions.py`

 * *Files identical despite different names*

### Comparing `py-easy-scrap-0.1.0/py-easy-scrap/web_scraping_functions.py` & `py-easy-scrap-0.1.1/pyeasyscrap/web_scraping_functions.py`

 * *Files identical despite different names*

### Comparing `py-easy-scrap-0.1.0/py_easy_scrap.egg-info/PKG-INFO` & `py-easy-scrap-0.1.1/py_easy_scrap.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-easy-scrap
-Version: 0.1.0
+Version: 0.1.1
 Summary: A useful package for web scraping with Selenium
 Home-page: https://github.com/ygalvao/py-easy-scrap
 Author: Yuri Henrique Galvao
 Author-email: Yuri Henrique Galvao <yuri@galvao.ca>
 License: UNKNOWN
 Project-URL: Homepage, https://github.com/ygalvao/py-easy-scrap
 Project-URL: Bug Tracker, https://github.com/ygalvao/py-easy-scrap/issues
@@ -27,20 +27,20 @@
 ```bash
 pip install py-easy-scrap
 ```
 
 ## Requirements
 
 - Python 3.7 or higher
-- Selenium
+- Selenium, along with __GeckoDriver__ (Firefox)
 
 ## Usage
 
 ```python
-import py_easy_scrap as pes
+import pyeasyscrap as pes
 ```
 
 ### Get WebDriver
 
 ```python
 driver = get_webdriver(headless)
 ```
```

### Comparing `py-easy-scrap-0.1.0/pyproject.toml` & `py-easy-scrap-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-easy-scrap"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Yuri Henrique Galvao", email="yuri@galvao.ca" },
 ]
 description = "A useful package for web scraping with Selenium"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `py-easy-scrap-0.1.0/setup.py` & `py-easy-scrap-0.1.1/setup.py`

 * *Files identical despite different names*

