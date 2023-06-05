# Comparing `tmp/solo_epd_loader-0.2.2.tar.gz` & `tmp/solo_epd_loader-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solo_epd_loader-0.2.2.tar", last modified: Thu May 25 07:45:48 2023, max compression
+gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-6qydycbe/solo_epd_loader-0.2.3.tar", last modified: Mon Jun  5 09:24:51 2023, max compression
```

## Comparing `solo_epd_loader-0.2.2.tar` & `solo_epd_loader-0.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.558088 solo_epd_loader-0.2.2/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.2/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.2/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-05-25 07:45:48.558088 solo_epd_loader-0.2.2/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16581 2023-05-23 14:42:04.000000 solo_epd_loader-0.2.2/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.2/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.554088 solo_epd_loader-0.2.2/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.2/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.2/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.2/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.2/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.554088 solo_epd_loader-0.2.2/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.2/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.2/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.2/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.2/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.554088 solo_epd_loader-0.2.2/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.2/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.2/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.2/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2302 2023-05-25 07:45:48.562088 solo_epd_loader-0.2.2/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.2/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.558088 solo_epd_loader-0.2.2/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    37798 2022-11-16 14:15:40.000000 solo_epd_loader-0.2.2/solo_epd_loader/__init__ (STEP UPDATE).py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    44832 2023-05-25 07:34:00.000000 solo_epd_loader-0.2.2/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.558088 solo_epd_loader-0.2.2/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.2/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-25 07:45:48.558088 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      653 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      188 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-05-25 07:45:48.000000 solo_epd_loader-0.2.2/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.2/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.788886 solo_epd_loader-0.2.3/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.3/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.3/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-06-05 09:24:51.788886 solo_epd_loader-0.2.3/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16581 2023-05-23 14:42:04.000000 solo_epd_loader-0.2.3/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.3/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.780886 solo_epd_loader-0.2.3/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.3/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.3/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.3/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.3/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.780886 solo_epd_loader-0.2.3/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.3/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.3/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.3/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.3/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.784886 solo_epd_loader-0.2.3/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.3/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.3/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.3/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-05 09:24:51.788886 solo_epd_loader-0.2.3/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.3/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.784886 solo_epd_loader-0.2.3/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    37798 2022-11-16 14:15:40.000000 solo_epd_loader-0.2.3/solo_epd_loader/__init__ (STEP UPDATE).py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    44832 2023-05-25 07:34:00.000000 solo_epd_loader-0.2.3/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.788886 solo_epd_loader-0.2.3/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.3/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 09:24:51.788886 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17529 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      653 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-05 09:24:51.000000 solo_epd_loader-0.2.3/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.3/tox.ini
```

### Comparing `solo_epd_loader-0.2.2/LICENSE.rst` & `solo_epd_loader-0.2.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/PKG-INFO` & `solo_epd_loader-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.2.2/README.rst` & `solo_epd_loader-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/code_of_conduct.md` & `solo_epd_loader-0.2.3/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/docs/Makefile` & `solo_epd_loader-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/docs/conf.py` & `solo_epd_loader-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/docs/make.bat` & `solo_epd_loader-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/examples/gh2021_fig_2.png` & `solo_epd_loader-0.2.3/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.2.3/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/gh2021_fig_2.png` & `solo_epd_loader-0.2.3/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/gh2021_fig_2a.png` & `solo_epd_loader-0.2.3/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/licenses/LICENSE.rst` & `solo_epd_loader-0.2.3/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.2.3/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/setup.cfg` & `solo_epd_loader-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 setup_requires = setuptools_scm
 install_requires = 
 	astropy
 	bs4
-	cdflib
+	cdflib<1.0
 	datetime
 	drms
 	h5netcdf
 	lxml
 	matplotlib
 	numpy
 	pandas
```

### Comparing `solo_epd_loader-0.2.2/setup.py` & `solo_epd_loader-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/solo_epd_loader/__init__ (STEP UPDATE).py` & `solo_epd_loader-0.2.3/solo_epd_loader/__init__ (STEP UPDATE).py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/solo_epd_loader/__init__.py` & `solo_epd_loader-0.2.3/solo_epd_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.2.3/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.2.2/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.2.3/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.2/tox.ini` & `solo_epd_loader-0.2.3/tox.ini`

 * *Files identical despite different names*

