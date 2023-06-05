# Comparing `tmp/porf-0.0.5.tar.gz` & `tmp/porf-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porf-0.0.5.tar", last modified: Mon Jun  5 11:45:23 2023, max compression
+gzip compressed data, was "porf-0.0.6.tar", last modified: Mon Jun  5 11:59:38 2023, max compression
```

## Comparing `porf-0.0.5.tar` & `porf-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 11:45:23.843101 porf-0.0.5/
--rw-rw-rw-   0        0        0     1080 2023-06-05 11:12:13.000000 porf-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1223 2023-06-05 11:45:23.842105 porf-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      689 2023-06-05 11:43:12.000000 porf-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 11:45:23.833093 porf-0.0.5/porf/
--rw-rw-rw-   0        0        0       81 2023-04-12 12:45:30.000000 porf-0.0.5/porf/__init__.py
--rw-rw-rw-   0        0        0     7056 2023-05-10 15:08:44.000000 porf-0.0.5/porf/open_sta_parser.py
--rw-rw-rw-   0        0        0     1984 2023-04-11 13:27:16.000000 porf-0.0.5/porf/run_analyser.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:45:23.840065 porf-0.0.5/porf.egg-info/
--rw-rw-rw-   0        0        0     1223 2023-06-05 11:45:23.000000 porf-0.0.5/porf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-05 11:45:23.000000 porf-0.0.5/porf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 11:45:23.000000 porf-0.0.5/porf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-05 11:45:23.000000 porf-0.0.5/porf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-05 11:45:23.000000 porf-0.0.5/porf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 11:45:23.843101 porf-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1163 2023-06-05 11:45:14.000000 porf-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:59:38.024939 porf-0.0.6/
+-rw-rw-rw-   0        0        0     1080 2023-06-05 11:12:13.000000 porf-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1223 2023-06-05 11:59:38.023941 porf-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2023-06-05 11:43:12.000000 porf-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 11:59:38.012933 porf-0.0.6/porf/
+-rw-rw-rw-   0        0        0       81 2023-04-12 12:45:30.000000 porf-0.0.6/porf/__init__.py
+-rw-rw-rw-   0        0        0     7056 2023-05-10 15:08:44.000000 porf-0.0.6/porf/open_sta_parser.py
+-rw-rw-rw-   0        0        0     1984 2023-04-11 13:27:16.000000 porf-0.0.6/porf/run_analyser.py
+drwxrwxrwx   0        0        0        0 2023-06-05 11:59:38.021897 porf-0.0.6/porf.egg-info/
+-rw-rw-rw-   0        0        0     1223 2023-06-05 11:59:37.000000 porf-0.0.6/porf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-05 11:59:37.000000 porf-0.0.6/porf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 11:59:37.000000 porf-0.0.6/porf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-06-05 11:59:37.000000 porf-0.0.6/porf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-05 11:59:37.000000 porf-0.0.6/porf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 11:59:38.024939 porf-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-06-05 11:59:00.000000 porf-0.0.6/setup.py
```

### Comparing `porf-0.0.5/LICENSE` & `porf-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `porf-0.0.5/PKG-INFO` & `porf-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porf
-Version: 0.0.5
+Version: 0.0.6
 Summary: Parse OpenRoad Files - RPT file parser for Openlane OpenROAD Static Timing Analysis output files.
 Home-page: https://github.com/daquintero/porf
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `porf-0.0.5/README.md` & `porf-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `porf-0.0.5/porf/open_sta_parser.py` & `porf-0.0.6/porf/open_sta_parser.py`

 * *Files identical despite different names*

### Comparing `porf-0.0.5/porf/run_analyser.py` & `porf-0.0.6/porf/run_analyser.py`

 * *Files identical despite different names*

### Comparing `porf-0.0.5/porf.egg-info/PKG-INFO` & `porf-0.0.6/porf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porf
-Version: 0.0.5
+Version: 0.0.6
 Summary: Parse OpenRoad Files - RPT file parser for Openlane OpenROAD Static Timing Analysis output files.
 Home-page: https://github.com/daquintero/porf
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `porf-0.0.5/setup.py` & `porf-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = Path(__file__).parent
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="porf",
-    version="0.0.5",
+    version="0.0.6",
     description="Parse OpenRoad Files - RPT file parser for Openlane OpenROAD Static Timing Analysis output files.",
     extras_require={
         "develop": [
             "sphinx",
             "sphinx_rtd_theme",
             "sphinx_autodoc_typehints",
             "nbsphinx",
@@ -24,15 +24,22 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/daquintero/porf",
     author="Dario Quintero",
     author_email="darioaquintero@gmail.com",
     packages=setuptools.find_packages(),
     include_package_data=True,
-    install_requires=["pandas"],
+    install_requires=[
+        "pandas",
+        "sphinx", # TODO sort this out better
+        "sphinx_rtd_theme",
+        "sphinx_autodoc_typehints",
+        "nbsphinx",
+        "myst_parser"
+    ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
```

