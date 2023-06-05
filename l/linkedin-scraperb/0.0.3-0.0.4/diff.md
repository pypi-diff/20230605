# Comparing `tmp/linkedin_scraperb-0.0.3.tar.gz` & `tmp/linkedin_scraperb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedin_scraperb-0.0.3.tar", last modified: Mon Jun  5 11:28:29 2023, max compression
+gzip compressed data, was "linkedin_scraperb-0.0.4.tar", last modified: Mon Jun  5 14:37:37 2023, max compression
```

## Comparing `linkedin_scraperb-0.0.3.tar` & `linkedin_scraperb-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 11:28:29.064715 linkedin_scraperb-0.0.3/
--rw-rw-rw-   0        0        0    35823 2023-05-31 08:44:40.000000 linkedin_scraperb-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    11395 2023-06-05 11:28:29.065710 linkedin_scraperb-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12093 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-05 11:28:29.032739 linkedin_scraperb-0.0.3/linkedin_scraperb/
--rw-rw-rw-   0        0        0      412 2023-06-05 11:28:22.000000 linkedin_scraperb-0.0.3/linkedin_scraperb/__init__.py
--rw-rw-rw-   0        0        0     1605 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.3/linkedin_scraperb/actions.py
--rw-rw-rw-   0        0        0    16380 2023-05-31 12:20:29.000000 linkedin_scraperb-0.0.3/linkedin_scraperb/company.py
--rw-rw-rw-   0        0        0      100 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.3/linkedin_scraperb/constants.py
--rw-rw-rw-   0        0        0     3830 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.3/linkedin_scraperb/job_search.py
--rw-rw-rw-   0        0        0     3628 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.3/linkedin_scraperb/jobs.py
--rw-rw-rw-   0        0        0     4327 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.3/linkedin_scraperb/objects.py
--rw-rw-rw-   0        0        0    16747 2023-06-05 10:04:08.000000 linkedin_scraperb-0.0.3/linkedin_scraperb/person.py
--rw-rw-rw-   0        0        0       30 2023-05-31 08:44:40.000000 linkedin_scraperb-0.0.3/linkedin_scraperb/selectors.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:28:29.063750 linkedin_scraperb-0.0.3/linkedin_scraperb.egg-info/
--rw-rw-rw-   0        0        0    11395 2023-06-05 11:28:28.000000 linkedin_scraperb-0.0.3/linkedin_scraperb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-06-05 11:28:28.000000 linkedin_scraperb-0.0.3/linkedin_scraperb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 11:28:28.000000 linkedin_scraperb-0.0.3/linkedin_scraperb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-05 11:28:28.000000 linkedin_scraperb-0.0.3/linkedin_scraperb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-05 11:28:28.000000 linkedin_scraperb-0.0.3/linkedin_scraperb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2023-06-05 11:28:29.067708 linkedin_scraperb-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-06-05 11:28:14.000000 linkedin_scraperb-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:37:37.781476 linkedin_scraperb-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-05-31 08:44:40.000000 linkedin_scraperb-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      440 2023-06-05 14:37:37.781476 linkedin_scraperb-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12093 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 14:37:37.751555 linkedin_scraperb-0.0.4/linkedin_scraperb/
+-rw-rw-rw-   0        0        0      412 2023-06-05 14:37:31.000000 linkedin_scraperb-0.0.4/linkedin_scraperb/__init__.py
+-rw-rw-rw-   0        0        0     1605 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.4/linkedin_scraperb/actions.py
+-rw-rw-rw-   0        0        0    16380 2023-05-31 12:20:29.000000 linkedin_scraperb-0.0.4/linkedin_scraperb/company.py
+-rw-rw-rw-   0        0        0      100 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.4/linkedin_scraperb/constants.py
+-rw-rw-rw-   0        0        0     3830 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.4/linkedin_scraperb/job_search.py
+-rw-rw-rw-   0        0        0     3628 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.4/linkedin_scraperb/jobs.py
+-rw-rw-rw-   0        0        0     4327 2023-05-31 12:20:25.000000 linkedin_scraperb-0.0.4/linkedin_scraperb/objects.py
+-rw-rw-rw-   0        0        0    16747 2023-06-05 10:04:08.000000 linkedin_scraperb-0.0.4/linkedin_scraperb/person.py
+-rw-rw-rw-   0        0        0       30 2023-05-31 08:44:40.000000 linkedin_scraperb-0.0.4/linkedin_scraperb/selectors.py
+drwxrwxrwx   0        0        0        0 2023-06-05 14:37:37.779481 linkedin_scraperb-0.0.4/linkedin_scraperb.egg-info/
+-rw-rw-rw-   0        0        0      440 2023-06-05 14:37:37.000000 linkedin_scraperb-0.0.4/linkedin_scraperb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-06-05 14:37:37.000000 linkedin_scraperb-0.0.4/linkedin_scraperb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 14:37:37.000000 linkedin_scraperb-0.0.4/linkedin_scraperb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-05 14:37:37.000000 linkedin_scraperb-0.0.4/linkedin_scraperb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-05 14:37:37.000000 linkedin_scraperb-0.0.4/linkedin_scraperb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       87 2023-06-05 14:37:37.790452 linkedin_scraperb-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-06-05 14:37:25.000000 linkedin_scraperb-0.0.4/setup.py
```

### Comparing `linkedin_scraperb-0.0.3/LICENSE` & `linkedin_scraperb-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linkedin_scraperb-0.0.3/README.rst` & `linkedin_scraperb-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `linkedin_scraperb-0.0.3/linkedin_scraperb/actions.py` & `linkedin_scraperb-0.0.4/linkedin_scraperb/actions.py`

 * *Files identical despite different names*

### Comparing `linkedin_scraperb-0.0.3/linkedin_scraperb/company.py` & `linkedin_scraperb-0.0.4/linkedin_scraperb/company.py`

 * *Files identical despite different names*

### Comparing `linkedin_scraperb-0.0.3/linkedin_scraperb/job_search.py` & `linkedin_scraperb-0.0.4/linkedin_scraperb/job_search.py`

 * *Files identical despite different names*

### Comparing `linkedin_scraperb-0.0.3/linkedin_scraperb/jobs.py` & `linkedin_scraperb-0.0.4/linkedin_scraperb/jobs.py`

 * *Files identical despite different names*

### Comparing `linkedin_scraperb-0.0.3/linkedin_scraperb/objects.py` & `linkedin_scraperb-0.0.4/linkedin_scraperb/objects.py`

 * *Files identical despite different names*

### Comparing `linkedin_scraperb-0.0.3/linkedin_scraperb/person.py` & `linkedin_scraperb-0.0.4/linkedin_scraperb/person.py`

 * *Files identical despite different names*

### Comparing `linkedin_scraperb-0.0.3/setup.py` & `linkedin_scraperb-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,31 +4,35 @@
 from os import path
 import re
 
 here = path.abspath(path.dirname(__file__))
 
 version = re.search(
     '^__version__\s*=\s*"(.*)"',
-    open('./linkedin_scraperb/__init__.py').read(),
+    open('linkedin_scraperb/__init__.py').read(),
     re.M
     ).group(1)
 
 # Get the long description from the README file
-with open('./README.md', encoding='utf-8') as f:
-    long_description = f.read()
+#with open('README.md', encoding='utf-8') as f:
+#    long_description = f.read()
 
 setup( 
     name = 'linkedin_scraperb', 
     packages = ['linkedin_scraperb'], # this must be the same as the name above 
     version = version, 
     description = 'Scrapes user data from Linkedin (this is a branch)', 
-    long_description = long_description,
+    long_description = 'OK',
     long_description_content_type='text/markdown',
     author = 'Joey Sham', 
     author_email = 'sham.joey@gmail.com', 
     url = 'https://github.com/RRohjansRsm/linkedin_scraper', # use the URL to the github repo 
     download_url = 'https://github.com/RRohjansRsm/linkedin_scraper/archive/refs/tags/' + version + '.tar.gz', 
     keywords = ['linkedin', 'scraping', 'scraper'],
     classifiers = [], 
-    install_requires=[package.split("\n")[0] for package in open("./requirements.txt", "r").readlines()]
+    install_requires=[
+        'selenium'
+        'requests'
+        'lxml'
+    ]
 )
```

