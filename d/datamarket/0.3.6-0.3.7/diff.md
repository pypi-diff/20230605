# Comparing `tmp/datamarket-0.3.6.tar.gz` & `tmp/datamarket-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.3.6.tar", last modified: Mon May 29 09:27:43 2023, max compression
+gzip compressed data, was "datamarket-0.3.7.tar", last modified: Mon Jun  5 14:01:03 2023, max compression
```

## Comparing `datamarket-0.3.6.tar` & `datamarket-0.3.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:27:43.046264 datamarket-0.3.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.3.6/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-05-29 09:27:43.046264 datamarket-0.3.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-25 14:26:25.000000 datamarket-0.3.6/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-29 09:27:43.046264 datamarket-0.3.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-05-29 09:27:28.000000 datamarket-0.3.6/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:27:43.042264 datamarket-0.3.6/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:27:43.042264 datamarket-0.3.6/src/datamarket/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.3.6/src/datamarket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:27:43.046264 datamarket-0.3.6/src/datamarket/interfaces/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.3.6/src/datamarket/interfaces/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.3.6/src/datamarket/interfaces/alchemy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.3.6/src/datamarket/interfaces/drive.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.3.6/src/datamarket/interfaces/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.3.6/src/datamarket/interfaces/proxy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.3.6/src/datamarket/interfaces/tinybird.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:27:43.046264 datamarket-0.3.6/src/datamarket/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-26 09:46:08.000000 datamarket-0.3.6/src/datamarket/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-05-25 14:18:08.000000 datamarket-0.3.6/src/datamarket/utils/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2355 2023-05-29 09:23:53.000000 datamarket-0.3.6/src/datamarket/utils/selenium.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:27:43.042264 datamarket-0.3.6/src/datamarket.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-05-29 09:27:43.000000 datamarket-0.3.6/src/datamarket.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-05-29 09:27:43.000000 datamarket-0.3.6/src/datamarket.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-29 09:27:43.000000 datamarket-0.3.6/src/datamarket.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-29 09:27:43.000000 datamarket-0.3.6/src/datamarket.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-29 09:27:43.000000 datamarket-0.3.6/src/datamarket.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 14:01:03.076609 datamarket-0.3.7/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.3.7/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-06-05 14:01:03.076609 datamarket-0.3.7/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-25 14:26:25.000000 datamarket-0.3.7/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-05 14:01:03.076609 datamarket-0.3.7/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-06-05 14:00:43.000000 datamarket-0.3.7/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 14:01:03.072609 datamarket-0.3.7/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 14:01:03.072609 datamarket-0.3.7/src/datamarket/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.3.7/src/datamarket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 14:01:03.076609 datamarket-0.3.7/src/datamarket/interfaces/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.3.7/src/datamarket/interfaces/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.3.7/src/datamarket/interfaces/alchemy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.3.7/src/datamarket/interfaces/drive.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.3.7/src/datamarket/interfaces/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.3.7/src/datamarket/interfaces/proxy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.3.7/src/datamarket/interfaces/tinybird.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 14:01:03.076609 datamarket-0.3.7/src/datamarket/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-26 09:46:08.000000 datamarket-0.3.7/src/datamarket/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-05-25 14:18:08.000000 datamarket-0.3.7/src/datamarket/utils/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2550 2023-06-05 14:00:07.000000 datamarket-0.3.7/src/datamarket/utils/selenium.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 14:01:03.072609 datamarket-0.3.7/src/datamarket.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-06-05 14:01:03.000000 datamarket-0.3.7/src/datamarket.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-06-05 14:01:03.000000 datamarket-0.3.7/src/datamarket.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-05 14:01:03.000000 datamarket-0.3.7/src/datamarket.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-06-05 14:01:03.000000 datamarket-0.3.7/src/datamarket.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-06-05 14:01:03.000000 datamarket-0.3.7/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.3.6/LICENSE` & `datamarket-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.6/PKG-INFO` & `datamarket-0.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.3.6
+Version: 0.3.7
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.3.6/README.md` & `datamarket-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.6/setup.py` & `datamarket-0.3.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "stem",
     "pydrive",
     "undetected_chromedriver",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.3.6",
+    version="0.3.7",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.3.6/src/datamarket/interfaces/alchemy.py` & `datamarket-0.3.7/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.6/src/datamarket/interfaces/drive.py` & `datamarket-0.3.7/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.6/src/datamarket/interfaces/ftp.py` & `datamarket-0.3.7/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.6/src/datamarket/interfaces/proxy.py` & `datamarket-0.3.7/src/datamarket/interfaces/proxy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.6/src/datamarket/interfaces/tinybird.py` & `datamarket-0.3.7/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.6/src/datamarket/utils/main.py` & `datamarket-0.3.7/src/datamarket/utils/main.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.6/src/datamarket/utils/selenium.py` & `datamarket-0.3.7/src/datamarket/utils/selenium.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 
 
 def get_driver(chrome_options=None):
     options = uc.ChromeOptions()
 
     if isinstance(chrome_options, list):
         for option in chrome_options:
-            options.add_argument(option)
+            if isinstance(option, dict):
+                for name, value in option["experimental"].items():
+                    options.add_experimental_option(name, value)
+            else:
+                options.add_argument(option)
 
     return uc.Chrome(version_main=get_chromedriver_version(),
                      options=options)
 
 
 def wait(driver, css_selector, timeout=30):
     logger.info(f"waiting for {css_selector}...")
```

### Comparing `datamarket-0.3.6/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.3.7/src/datamarket.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.3.6
+Version: 0.3.7
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.3.6/src/datamarket.egg-info/SOURCES.txt` & `datamarket-0.3.7/src/datamarket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

