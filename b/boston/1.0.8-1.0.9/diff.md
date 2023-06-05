# Comparing `tmp/boston-1.0.8.tar.gz` & `tmp/boston-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boston-1.0.8.tar", last modified: Mon May  1 09:38:30 2023, max compression
+gzip compressed data, was "boston-1.0.9.tar", last modified: Mon May  1 09:42:53 2023, max compression
```

## Comparing `boston-1.0.8.tar` & `boston-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 09:38:30.514381 boston-1.0.8/
--rw-rw-rw-   0        0        0       43 2023-05-01 09:37:05.000000 boston-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      451 2023-05-01 09:38:30.513383 boston-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 09:38:30.484380 boston-1.0.8/boston/
--rw-rw-rw-   0        0        0       66 2023-05-01 09:38:12.000000 boston-1.0.8/boston/__init__.py
--rw-rw-rw-   0        0        0      472 2023-05-01 09:30:33.000000 boston-1.0.8/boston/house.py
-drwxrwxrwx   0        0        0        0 2023-05-01 09:38:30.507384 boston-1.0.8/boston.egg-info/
--rw-rw-rw-   0        0        0      451 2023-05-01 09:38:30.000000 boston-1.0.8/boston.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-01 09:38:30.000000 boston-1.0.8/boston.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 09:38:30.000000 boston-1.0.8/boston.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 09:38:30.000000 boston-1.0.8/boston.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 09:38:30.000000 boston-1.0.8/boston.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 09:38:30.510381 boston-1.0.8/resources/
--rw-rw-rw-   0        0        0    35230 2023-04-27 10:15:02.000000 boston-1.0.8/resources/boston_house_prices.csv
--rw-rw-rw-   0        0        0       42 2023-05-01 09:38:30.515383 boston-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-05-01 09:38:16.000000 boston-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:42:53.715569 boston-1.0.9/
+-rw-rw-rw-   0        0        0       43 2023-05-01 09:37:05.000000 boston-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      451 2023-05-01 09:42:53.714597 boston-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 09:42:53.678571 boston-1.0.9/boston/
+-rw-rw-rw-   0        0        0       66 2023-05-01 09:42:29.000000 boston-1.0.9/boston/__init__.py
+-rw-rw-rw-   0        0        0      472 2023-05-01 09:30:33.000000 boston-1.0.9/boston/house.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:42:53.708607 boston-1.0.9/boston.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-05-01 09:42:53.000000 boston-1.0.9/boston.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-01 09:42:53.000000 boston-1.0.9/boston.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:42:53.000000 boston-1.0.9/boston.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 09:42:53.000000 boston-1.0.9/boston.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 09:42:53.000000 boston-1.0.9/boston.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 09:42:53.711569 boston-1.0.9/resources/
+-rw-rw-rw-   0        0        0    35230 2023-04-27 10:15:02.000000 boston-1.0.9/resources/boston_house_prices.csv
+-rw-rw-rw-   0        0        0       42 2023-05-01 09:42:53.716573 boston-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-05-01 09:42:48.000000 boston-1.0.9/setup.py
```

### Comparing `boston-1.0.8/resources/boston_house_prices.csv` & `boston-1.0.9/resources/boston_house_prices.csv`

 * *Files identical despite different names*

### Comparing `boston-1.0.8/setup.py` & `boston-1.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import setuptools
 
 
 setuptools.setup(
     name="boston", # Replace with your own username
-    version="1.0.8",
+    version="1.0.9",
     author="julmubm",
     author_email="dltpdn@gmail.com",
     description="loading boston housing price dataset like sklearn.datasets.load_boston() style.",
     long_description_content_type="text/markdown",
     url="https://github.com/dltpdn/boston",
     install_requires=['pandas'],
     packages=setuptools.find_packages(),
+    package_data={'boston':['resources/boston_house_prices.csv']},
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

