# Comparing `tmp/py-easy-scrap-0.1.2.tar.gz` & `tmp/py-easy-scrap-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-easy-scrap-0.1.2.tar", last modified: Mon Jun  5 02:56:13 2023, max compression
+gzip compressed data, was "py-easy-scrap-0.1.3.tar", last modified: Mon Jun  5 03:04:15 2023, max compression
```

## Comparing `py-easy-scrap-0.1.2.tar` & `py-easy-scrap-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 02:56:13.012585 py-easy-scrap-0.1.2/
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     1077 2023-06-05 00:17:41.000000 py-easy-scrap-0.1.2/LICENSE
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2657 2023-06-05 02:56:13.012585 py-easy-scrap-0.1.2/PKG-INFO
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2003 2023-06-05 02:48:20.000000 py-easy-scrap-0.1.2/README.md
-drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 02:56:13.012585 py-easy-scrap-0.1.2/py_easy_scrap.egg-info/
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2657 2023-06-05 02:56:12.000000 py-easy-scrap-0.1.2/py_easy_scrap.egg-info/PKG-INFO
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      318 2023-06-05 02:56:13.000000 py-easy-scrap-0.1.2/py_easy_scrap.egg-info/SOURCES.txt
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)        1 2023-06-05 02:56:12.000000 py-easy-scrap-0.1.2/py_easy_scrap.egg-info/dependency_links.txt
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       18 2023-06-05 02:56:12.000000 py-easy-scrap-0.1.2/py_easy_scrap.egg-info/requires.txt
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       12 2023-06-05 02:56:12.000000 py-easy-scrap-0.1.2/py_easy_scrap.egg-info/top_level.txt
-drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 02:56:13.012585 py-easy-scrap-0.1.2/pyeasyscrap/
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       92 2023-06-05 02:55:27.000000 py-easy-scrap-0.1.2/pyeasyscrap/__init__.py
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     4114 2023-06-05 02:26:32.000000 py-easy-scrap-0.1.2/pyeasyscrap/basic_functions.py
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     4587 2023-06-05 00:55:06.000000 py-easy-scrap-0.1.2/pyeasyscrap/web_scraping_functions.py
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      644 2023-06-05 02:55:47.000000 py-easy-scrap-0.1.2/pyproject.toml
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       38 2023-06-05 02:56:13.012585 py-easy-scrap-0.1.2/setup.cfg
--rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      806 2023-06-05 02:55:52.000000 py-easy-scrap-0.1.2/setup.py
+drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 03:04:15.823674 py-easy-scrap-0.1.3/
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     1077 2023-06-05 00:17:41.000000 py-easy-scrap-0.1.3/LICENSE
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2819 2023-06-05 03:04:15.823674 py-easy-scrap-0.1.3/PKG-INFO
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2165 2023-06-05 03:03:29.000000 py-easy-scrap-0.1.3/README.md
+drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 03:04:15.823674 py-easy-scrap-0.1.3/py_easy_scrap.egg-info/
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     2819 2023-06-05 03:04:15.000000 py-easy-scrap-0.1.3/py_easy_scrap.egg-info/PKG-INFO
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      318 2023-06-05 03:04:15.000000 py-easy-scrap-0.1.3/py_easy_scrap.egg-info/SOURCES.txt
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)        1 2023-06-05 03:04:15.000000 py-easy-scrap-0.1.3/py_easy_scrap.egg-info/dependency_links.txt
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       18 2023-06-05 03:04:15.000000 py-easy-scrap-0.1.3/py_easy_scrap.egg-info/requires.txt
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       12 2023-06-05 03:04:15.000000 py-easy-scrap-0.1.3/py_easy_scrap.egg-info/top_level.txt
+drwxrwxr-x   0 yhgalvao  (1000) yhgalvao  (1000)        0 2023-06-05 03:04:15.823674 py-easy-scrap-0.1.3/pyeasyscrap/
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       61 2023-06-05 03:00:22.000000 py-easy-scrap-0.1.3/pyeasyscrap/__init__.py
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     4114 2023-06-05 02:26:32.000000 py-easy-scrap-0.1.3/pyeasyscrap/basic_functions.py
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)     4588 2023-06-05 03:00:12.000000 py-easy-scrap-0.1.3/pyeasyscrap/web_scraping_functions.py
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      644 2023-06-05 03:04:02.000000 py-easy-scrap-0.1.3/pyproject.toml
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)       38 2023-06-05 03:04:15.823674 py-easy-scrap-0.1.3/setup.cfg
+-rw-rw-r--   0 yhgalvao  (1000) yhgalvao  (1000)      806 2023-06-05 03:03:58.000000 py-easy-scrap-0.1.3/setup.py
```

### Comparing `py-easy-scrap-0.1.2/LICENSE` & `py-easy-scrap-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-easy-scrap-0.1.2/PKG-INFO` & `py-easy-scrap-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-easy-scrap
-Version: 0.1.2
+Version: 0.1.3
 Summary: A useful package for web scraping with Selenium
 Home-page: https://github.com/ygalvao/py-easy-scrap
 Author: Yuri Henrique Galvao
 Author-email: Yuri Henrique Galvao <yuri@galvao.ca>
 License: UNKNOWN
 Project-URL: Homepage, https://github.com/ygalvao/py-easy-scrap
 Project-URL: Bug Tracker, https://github.com/ygalvao/py-easy-scrap/issues
@@ -31,52 +31,58 @@
 ## Requirements
 
 - Python 3.7 or higher
 - Selenium, along with __GeckoDriver__ (Firefox)
 
 ## Usage
 
+In your project directory, create a new directory for your logs - it can be just called 'logs':
+```bash
+mkdir logs
+```
+
+Then, import the package:
 ```python
 import pyeasyscrap as pes
 ```
 
 ### Get WebDriver
 
 ```python
-driver = get_webdriver(headless)
+driver = pes.get_webdriver(headless)
 ```
 This will return an instance of webdriver.Firefox (GeckoDriver).
 
 ### Get Element
 
 ```python
-element = get_element(driver, value="element_xpath")
+element = pes.get_element(driver, value="element_xpath")
 ```
 
 This will return the web element found using the specified driver and value. By default, this function uses 'XPATH' as the method of searching. However, you can change this by providing 'ID' or 'LINK_TEXT' as the 'by' argument.
 
 Please be aware that the method of searching ('XPATH', 'ID', or 'LINK_TEXT') highly depends on the webpage structure. Therefore, it is essential to inspect the webpage beforehand.
 
 Also, please remember to replace `"element_xpath"` with the actual Xpath, ID, or link text of the element you want to find.
 
 
 ### Scroll to Element
 
 ```python
-scroll_to(driver, element)
+pes.scroll_to(driver, element)
 ```
 
 This will use JavaScript to scroll the view of the given webdriver to the specified web element.
 
 ### Ask for Data
 
 ```python
 required_data = ("username", "password")
 file_name_no_extension = "user_credentials"
-ask_for_data(required_data, file_name_no_extension)
+pes.ask_for_data(required_data, file_name_no_extension)
 ```
 
 This will return a dictionary containing the collected data and will create a JSON configuration (.conf) file.
 
 ### Check File
 
 ```python
```

### Comparing `py-easy-scrap-0.1.2/README.md` & `py-easy-scrap-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,52 +13,58 @@
 ## Requirements
 
 - Python 3.7 or higher
 - Selenium, along with __GeckoDriver__ (Firefox)
 
 ## Usage
 
+In your project directory, create a new directory for your logs - it can be just called 'logs':
+```bash
+mkdir logs
+```
+
+Then, import the package:
 ```python
 import pyeasyscrap as pes
 ```
 
 ### Get WebDriver
 
 ```python
-driver = get_webdriver(headless)
+driver = pes.get_webdriver(headless)
 ```
 This will return an instance of webdriver.Firefox (GeckoDriver).
 
 ### Get Element
 
 ```python
-element = get_element(driver, value="element_xpath")
+element = pes.get_element(driver, value="element_xpath")
 ```
 
 This will return the web element found using the specified driver and value. By default, this function uses 'XPATH' as the method of searching. However, you can change this by providing 'ID' or 'LINK_TEXT' as the 'by' argument.
 
 Please be aware that the method of searching ('XPATH', 'ID', or 'LINK_TEXT') highly depends on the webpage structure. Therefore, it is essential to inspect the webpage beforehand.
 
 Also, please remember to replace `"element_xpath"` with the actual Xpath, ID, or link text of the element you want to find.
 
 
 ### Scroll to Element
 
 ```python
-scroll_to(driver, element)
+pes.scroll_to(driver, element)
 ```
 
 This will use JavaScript to scroll the view of the given webdriver to the specified web element.
 
 ### Ask for Data
 
 ```python
 required_data = ("username", "password")
 file_name_no_extension = "user_credentials"
-ask_for_data(required_data, file_name_no_extension)
+pes.ask_for_data(required_data, file_name_no_extension)
 ```
 
 This will return a dictionary containing the collected data and will create a JSON configuration (.conf) file.
 
 ### Check File
 
 ```python
```

### Comparing `py-easy-scrap-0.1.2/py_easy_scrap.egg-info/PKG-INFO` & `py-easy-scrap-0.1.3/py_easy_scrap.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-easy-scrap
-Version: 0.1.2
+Version: 0.1.3
 Summary: A useful package for web scraping with Selenium
 Home-page: https://github.com/ygalvao/py-easy-scrap
 Author: Yuri Henrique Galvao
 Author-email: Yuri Henrique Galvao <yuri@galvao.ca>
 License: UNKNOWN
 Project-URL: Homepage, https://github.com/ygalvao/py-easy-scrap
 Project-URL: Bug Tracker, https://github.com/ygalvao/py-easy-scrap/issues
@@ -31,52 +31,58 @@
 ## Requirements
 
 - Python 3.7 or higher
 - Selenium, along with __GeckoDriver__ (Firefox)
 
 ## Usage
 
+In your project directory, create a new directory for your logs - it can be just called 'logs':
+```bash
+mkdir logs
+```
+
+Then, import the package:
 ```python
 import pyeasyscrap as pes
 ```
 
 ### Get WebDriver
 
 ```python
-driver = get_webdriver(headless)
+driver = pes.get_webdriver(headless)
 ```
 This will return an instance of webdriver.Firefox (GeckoDriver).
 
 ### Get Element
 
 ```python
-element = get_element(driver, value="element_xpath")
+element = pes.get_element(driver, value="element_xpath")
 ```
 
 This will return the web element found using the specified driver and value. By default, this function uses 'XPATH' as the method of searching. However, you can change this by providing 'ID' or 'LINK_TEXT' as the 'by' argument.
 
 Please be aware that the method of searching ('XPATH', 'ID', or 'LINK_TEXT') highly depends on the webpage structure. Therefore, it is essential to inspect the webpage beforehand.
 
 Also, please remember to replace `"element_xpath"` with the actual Xpath, ID, or link text of the element you want to find.
 
 
 ### Scroll to Element
 
 ```python
-scroll_to(driver, element)
+pes.scroll_to(driver, element)
 ```
 
 This will use JavaScript to scroll the view of the given webdriver to the specified web element.
 
 ### Ask for Data
 
 ```python
 required_data = ("username", "password")
 file_name_no_extension = "user_credentials"
-ask_for_data(required_data, file_name_no_extension)
+pes.ask_for_data(required_data, file_name_no_extension)
 ```
 
 This will return a dictionary containing the collected data and will create a JSON configuration (.conf) file.
 
 ### Check File
 
 ```python
```

### Comparing `py-easy-scrap-0.1.2/pyeasyscrap/basic_functions.py` & `py-easy-scrap-0.1.3/pyeasyscrap/basic_functions.py`

 * *Files identical despite different names*

### Comparing `py-easy-scrap-0.1.2/pyeasyscrap/web_scraping_functions.py` & `py-easy-scrap-0.1.3/pyeasyscrap/web_scraping_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from selenium import webdriver
 from selenium.webdriver.firefox.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support import expected_conditions as EC
-from basic_functions import *
+from .basic_functions import *
 
 headless = False if '--show-browser' in args else True if '--headless' in args else confirm('Do you want the browser to be headless (i.e., you won\'t see it)? [y/n] ')
 
 def get_webdriver(headless:bool)->object:
     """
     Sets up and returns a selenium webdriver object with desired configurations. Uses GeckoDriver (Firefox).
```

### Comparing `py-easy-scrap-0.1.2/pyproject.toml` & `py-easy-scrap-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-easy-scrap"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Yuri Henrique Galvao", email="yuri@galvao.ca" },
 ]
 description = "A useful package for web scraping with Selenium"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `py-easy-scrap-0.1.2/setup.py` & `py-easy-scrap-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 setup(
     name='py-easy-scrap',
-    version='0.1.2',
+    version='0.1.3',
     url='https://github.com/ygalvao/py-easy-scrap',
     author='Yuri Henrique Galvao',
     author_email='yuri@galvao.ca',
     description='A useful package for web scraping with Selenium',
     packages=find_packages(),
     install_requires=[
         'selenium',
```

