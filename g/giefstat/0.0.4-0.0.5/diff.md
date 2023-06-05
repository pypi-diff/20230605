# Comparing `tmp/giefstat-0.0.4.tar.gz` & `tmp/giefstat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giefstat-0.0.4.tar", last modified: Mon Jun  5 15:08:44 2023, max compression
+gzip compressed data, was "giefstat-0.0.5.tar", last modified: Mon Jun  5 15:34:18 2023, max compression
```

## Comparing `giefstat-0.0.4.tar` & `giefstat-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 15:08:44.304700 giefstat-0.0.4/
--rw-rw-rw-   0        0        0     3561 2023-06-05 15:08:44.303702 giefstat-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3170 2023-06-05 14:19:49.000000 giefstat-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 15:08:44.302706 giefstat-0.0.4/giefstat.egg-info/
--rw-rw-rw-   0        0        0     3561 2023-06-05 15:08:44.000000 giefstat-0.0.4/giefstat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-06-05 15:08:44.000000 giefstat-0.0.4/giefstat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 15:08:44.000000 giefstat-0.0.4/giefstat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-05 15:08:44.000000 giefstat-0.0.4/giefstat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 15:08:44.000000 giefstat-0.0.4/giefstat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 15:08:44.304700 giefstat-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-06-05 15:06:31.000000 giefstat-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.843501 giefstat-0.0.5/
+-rw-rw-rw-   0        0        0     3561 2023-06-05 15:34:18.842503 giefstat-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3170 2023-06-05 14:19:49.000000 giefstat-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.739779 giefstat-0.0.5/giefstat/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:49:40.000000 giefstat-0.0.5/giefstat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.755737 giefstat-0.0.5/giefstat/estimate/
+-rw-rw-rw-   0        0        0     3953 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/__init__.py
+-rw-rw-rw-   0        0        0     5258 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/_univar_encoding.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.757731 giefstat-0.0.5/giefstat/estimate/gief/
+-rw-rw-rw-   0        0        0      414 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.763714 giefstat-0.0.5/giefstat/estimate/gief/entropy/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/entropy/__init__.py
+-rw-rw-rw-   0        0        0      915 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/entropy/cond_entropy.py
+-rw-rw-rw-   0        0        0     2602 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/entropy/marg_entropy.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.773688 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/__init__.py
+-rw-rw-rw-   0        0        0    11405 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/_kraskov.py
+-rw-rw-rw-   0        0        0     2767 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/_ross.py
+-rw-rw-rw-   0        0        0     2651 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/cmi.py
+-rw-rw-rw-   0        0        0     1931 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/mi.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.777678 giefstat-0.0.5/giefstat/estimate/kde/
+-rw-rw-rw-   0        0        0       89 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/kde/__init__.py
+-rw-rw-rw-   0        0        0     3015 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/kde/kde.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.781666 giefstat-0.0.5/giefstat/estimate/mic/
+-rw-rw-rw-   0        0        0      194 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/mic/__init__.py
+-rw-rw-rw-   0        0        0     1718 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/mic/_mic_rmic.py
+-rw-rw-rw-   0        0        0     2802 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/mic/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.785657 giefstat-0.0.5/giefstat/estimate/model_based/
+-rw-rw-rw-   0        0        0      260 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/model_based/__init__.py
+-rw-rw-rw-   0        0        0     4099 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/model_based/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.797623 giefstat-0.0.5/giefstat/estimate/other/
+-rw-rw-rw-   0        0        0      289 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/other/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/other/coefficient.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.811586 giefstat-0.0.5/giefstat/estimate/quant_based/
+-rw-rw-rw-   0        0        0      281 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/quant_based/__init__.py
+-rw-rw-rw-   0        0        0     7282 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/quant_based/_quant_darbellay.py
+-rw-rw-rw-   0        0        0     2111 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/quant_based/mi_classic.py
+-rw-rw-rw-   0        0        0     1700 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/quant_based/mi_darbellay.py
+-rw-rw-rw-   0        0        0       90 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/setting.py
+-rw-rw-rw-   0        0        0     3447 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/util.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.840510 giefstat-0.0.5/giefstat/statistical_tools/
+-rw-rw-rw-   0        0        0      498 2023-06-05 14:19:01.000000 giefstat-0.0.5/giefstat/statistical_tools/__init__.py
+-rw-rw-rw-   0        0        0     3142 2023-06-05 14:19:01.000000 giefstat-0.0.5/giefstat/statistical_tools/surrog_indep_test.py
+-rw-rw-rw-   0        0        0     2692 2023-06-05 14:19:01.000000 giefstat-0.0.5/giefstat/statistical_tools/time_delayed_association.py
+-rw-rw-rw-   0        0        0     1068 2023-06-05 14:19:01.000000 giefstat-0.0.5/giefstat/statistical_tools/util.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.747757 giefstat-0.0.5/giefstat.egg-info/
+-rw-rw-rw-   0        0        0     3561 2023-06-05 15:34:18.000000 giefstat-0.0.5/giefstat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1394 2023-06-05 15:34:18.000000 giefstat-0.0.5/giefstat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:34:18.000000 giefstat-0.0.5/giefstat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-05 15:34:18.000000 giefstat-0.0.5/giefstat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 15:34:18.000000 giefstat-0.0.5/giefstat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:34:18.843501 giefstat-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-06-05 15:34:12.000000 giefstat-0.0.5/setup.py
```

### Comparing `giefstat-0.0.4/PKG-INFO` & `giefstat-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
 Keywords: python,information estimation
 Requires-Python: >=3.8.0
```

### Comparing `giefstat-0.0.4/README.md` & `giefstat-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.4/giefstat.egg-info/PKG-INFO` & `giefstat-0.0.5/giefstat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
 Keywords: python,information estimation
 Requires-Python: >=3.8.0
```

### Comparing `giefstat-0.0.4/setup.py` & `giefstat-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 import os
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "Package for information estimation, independence test, etc."
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text(encoding="utf-8")
 
 setup(
     name="giefstat",
     version=VERSION,
     author="Dreisteine",
     author_email="dreisteine@163.com",
     description=DESCRIPTION,
-    packages=find_packages(include=["gief"]),
+    packages=find_packages(include=["giefstat", "giefstat.*"]),
     install_requires=["scikit-learn==0.24.0", "minepy==1.2.6"],
     keywords=["python", "information estimation"],
     python_requires=">=3.8.0",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ulti-Dreisteine/general-information-estimation-framework",
```

