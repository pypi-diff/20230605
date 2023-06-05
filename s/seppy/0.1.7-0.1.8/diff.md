# Comparing `tmp/seppy-0.1.7.tar.gz` & `tmp/seppy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppy-0.1.7.tar", last modified: Tue Apr  4 06:01:12 2023, max compression
+gzip compressed data, was "/home/gieseler/uni/serpentine/SEPpy/dist/.tmp-fri4pg9e/seppy-0.1.8.tar", last modified: Mon Jun  5 08:27:01 2023, max compression
```

## Comparing `seppy-0.1.7.tar` & `seppy-0.1.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.602693 seppy-0.1.7/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1520 2022-10-03 14:02:11.000000 seppy-0.1.7/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-10-03 14:02:11.000000 seppy-0.1.7/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3994 2023-04-04 06:01:12.602693 seppy-0.1.7/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3242 2023-03-28 13:55:24.000000 seppy-0.1.7/README.rst
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.598693 seppy-0.1.7/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-10-03 14:02:11.000000 seppy-0.1.7/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2292 2022-10-03 14:02:11.000000 seppy-0.1.7/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      277 2022-10-03 14:02:11.000000 seppy-0.1.7/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-10-03 14:02:11.000000 seppy-0.1.7/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.598693 seppy-0.1.7/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1473 2022-10-03 14:02:11.000000 seppy-0.1.7/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-10-03 14:02:11.000000 seppy-0.1.7/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-10-03 14:02:11.000000 seppy-0.1.7/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      141 2023-04-04 04:46:10.000000 seppy-0.1.7/requirements.txt
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.598693 seppy-0.1.7/seppy/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      254 2022-10-03 14:02:11.000000 seppy-0.1.7/seppy/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.594693 seppy-0.1.7/seppy/data/
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.602693 seppy-0.1.7/seppy/data/test/
--rw-------   0 gieseler  (1000) gieseler  (1000)   180858 2022-08-29 08:28:05.000000 seppy-0.1.7/seppy/data/test/epi21106.rl2
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   401828 2023-03-28 13:18:22.000000 seppy-0.1.7/seppy/data/test/psp_isois-epihi_l2-het-rates60_20210531_v15.cdf
--rw-------   0 gieseler  (1000) gieseler  (1000)   167882 2023-03-28 12:40:18.000000 seppy-0.1.7/seppy/data/test/sept_ahead_ele_sun_2006_318_1min_l2_v03.dat
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   278505 2023-03-28 12:00:02.000000 seppy-0.1.7/seppy/data/test/soho_erne-hed_l2-1min_20211028_v01.cdf
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    59249 2023-03-28 13:39:21.000000 seppy-0.1.7/seppy/data/test/solo_l2_mag-rtn-normal-1-minute_20210712_v01.cdf
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   215082 2022-09-19 08:48:15.000000 seppy-0.1.7/seppy/data/test/sta_l1_het_20211028_v01.cdf
--rw-------   0 gieseler  (1000) gieseler  (1000)    30939 2023-03-28 09:18:01.000000 seppy-0.1.7/seppy/data/test/wi_sfsp_3dp_00000000_v01.cdf
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    67008 2022-06-28 15:22:09.000000 seppy-0.1.7/seppy/data/test/wi_sfsp_3dp_20200213_v01.cdf
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.602693 seppy-0.1.7/seppy/loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    22263 2023-04-04 04:45:49.000000 seppy-0.1.7/seppy/loader/psp.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    19542 2023-04-04 04:57:34.000000 seppy-0.1.7/seppy/loader/soho.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3054 2022-10-03 14:02:11.000000 seppy-0.1.7/seppy/loader/solo.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    24339 2023-04-04 05:29:42.000000 seppy-0.1.7/seppy/loader/stereo.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    18229 2023-03-28 08:59:59.000000 seppy-0.1.7/seppy/loader/wind.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.602693 seppy-0.1.7/seppy/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-10-03 14:02:11.000000 seppy-0.1.7/seppy/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6682 2023-03-28 13:40:32.000000 seppy-0.1.7/seppy/tests/test_loader.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2942 2023-03-28 12:33:40.000000 seppy-0.1.7/seppy/tests/test_tools.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.602693 seppy-0.1.7/seppy/tools/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    98073 2023-03-28 09:37:44.000000 seppy-0.1.7/seppy/tools/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3139 2022-11-28 10:06:29.000000 seppy-0.1.7/seppy/tools/swaves.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6529 2022-11-11 11:40:09.000000 seppy-0.1.7/seppy/tools/widgets.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.602693 seppy-0.1.7/seppy/util/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     9431 2023-03-28 08:57:53.000000 seppy-0.1.7/seppy/util/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-04-04 06:01:12.000000 seppy-0.1.7/seppy/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-04 06:01:12.598693 seppy-0.1.7/seppy.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3994 2023-04-04 06:01:12.000000 seppy-0.1.7/seppy.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1089 2023-04-04 06:01:12.000000 seppy-0.1.7/seppy.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-04-04 06:01:12.000000 seppy-0.1.7/seppy.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-10-03 14:19:00.000000 seppy-0.1.7/seppy.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      226 2023-04-04 06:01:12.000000 seppy-0.1.7/seppy.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        6 2023-04-04 06:01:12.000000 seppy-0.1.7/seppy.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2019 2023-04-04 06:01:12.602693 seppy-0.1.7/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      656 2022-10-03 14:02:11.000000 seppy-0.1.7/setup.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1288 2022-10-03 14:02:11.000000 seppy-0.1.7/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.870232 seppy-0.1.8/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1520 2022-10-03 14:02:11.000000 seppy-0.1.8/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-10-03 14:02:11.000000 seppy-0.1.8/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3994 2023-06-05 08:27:01.870232 seppy-0.1.8/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3242 2023-03-28 13:55:24.000000 seppy-0.1.8/README.rst
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.854232 seppy-0.1.8/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-10-03 14:02:11.000000 seppy-0.1.8/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2292 2022-10-03 14:02:11.000000 seppy-0.1.8/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      277 2022-10-03 14:02:11.000000 seppy-0.1.8/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-10-03 14:02:11.000000 seppy-0.1.8/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.854232 seppy-0.1.8/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1473 2022-10-03 14:02:11.000000 seppy-0.1.8/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-10-03 14:02:11.000000 seppy-0.1.8/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-10-03 14:02:11.000000 seppy-0.1.8/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      149 2023-06-05 08:09:24.000000 seppy-0.1.8/requirements.txt
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.854232 seppy-0.1.8/seppy/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      254 2022-10-03 14:02:11.000000 seppy-0.1.8/seppy/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.850232 seppy-0.1.8/seppy/data/
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.866232 seppy-0.1.8/seppy/data/test/
+-rw-------   0 gieseler  (1000) gieseler  (1000)   180858 2022-08-29 08:28:05.000000 seppy-0.1.8/seppy/data/test/epi21106.rl2
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   401828 2023-03-28 13:18:22.000000 seppy-0.1.8/seppy/data/test/psp_isois-epihi_l2-het-rates60_20210531_v15.cdf
+-rw-------   0 gieseler  (1000) gieseler  (1000)   167882 2023-03-28 12:40:18.000000 seppy-0.1.8/seppy/data/test/sept_ahead_ele_sun_2006_318_1min_l2_v03.dat
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   278505 2023-03-28 12:00:02.000000 seppy-0.1.8/seppy/data/test/soho_erne-hed_l2-1min_20211028_v01.cdf
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    59249 2023-03-28 13:39:21.000000 seppy-0.1.8/seppy/data/test/solo_l2_mag-rtn-normal-1-minute_20210712_v01.cdf
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   215082 2022-09-19 08:48:15.000000 seppy-0.1.8/seppy/data/test/sta_l1_het_20211028_v01.cdf
+-rw-------   0 gieseler  (1000) gieseler  (1000)    30939 2023-03-28 09:18:01.000000 seppy-0.1.8/seppy/data/test/wi_sfsp_3dp_00000000_v01.cdf
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    67008 2022-06-28 15:22:09.000000 seppy-0.1.8/seppy/data/test/wi_sfsp_3dp_20200213_v01.cdf
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.866232 seppy-0.1.8/seppy/loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    22263 2023-04-04 04:45:49.000000 seppy-0.1.8/seppy/loader/psp.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    19542 2023-04-04 04:57:34.000000 seppy-0.1.8/seppy/loader/soho.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3054 2022-10-03 14:02:11.000000 seppy-0.1.8/seppy/loader/solo.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    24339 2023-04-04 05:29:42.000000 seppy-0.1.8/seppy/loader/stereo.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    18229 2023-03-28 08:59:59.000000 seppy-0.1.8/seppy/loader/wind.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.866232 seppy-0.1.8/seppy/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-10-03 14:02:11.000000 seppy-0.1.8/seppy/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6682 2023-03-28 13:40:32.000000 seppy-0.1.8/seppy/tests/test_loader.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2942 2023-03-28 12:33:40.000000 seppy-0.1.8/seppy/tests/test_tools.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.866232 seppy-0.1.8/seppy/tools/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   113492 2023-06-01 13:52:09.000000 seppy-0.1.8/seppy/tools/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3139 2023-06-01 13:52:21.000000 seppy-0.1.8/seppy/tools/swaves.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6845 2023-06-01 13:52:54.000000 seppy-0.1.8/seppy/tools/widgets.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.866232 seppy-0.1.8/seppy/util/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    13476 2023-06-02 15:57:32.000000 seppy-0.1.8/seppy/util/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-05 08:27:01.000000 seppy-0.1.8/seppy/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-05 08:27:01.854232 seppy-0.1.8/seppy.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3994 2023-06-05 08:27:01.000000 seppy-0.1.8/seppy.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1089 2023-06-05 08:27:01.000000 seppy-0.1.8/seppy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-05 08:27:01.000000 seppy-0.1.8/seppy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-10-03 14:19:00.000000 seppy-0.1.8/seppy.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      232 2023-06-05 08:27:01.000000 seppy-0.1.8/seppy.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        6 2023-06-05 08:27:01.000000 seppy-0.1.8/seppy.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2027 2023-06-05 08:27:01.870232 seppy-0.1.8/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      656 2022-10-03 14:02:11.000000 seppy-0.1.8/setup.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1288 2022-10-03 14:02:11.000000 seppy-0.1.8/tox.ini
```

### Comparing `seppy-0.1.7/LICENSE.rst` & `seppy-0.1.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/PKG-INFO` & `seppy-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seppy
-Version: 0.1.7
+Version: 0.1.8
 Summary: SEPpy
 Home-page: https://github.com/serpentine-h2020/SEPpy
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seppy-0.1.7/README.rst` & `seppy-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/docs/Makefile` & `seppy-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/docs/conf.py` & `seppy-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/docs/make.bat` & `seppy-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/licenses/LICENSE.rst` & `seppy-0.1.8/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/licenses/TEMPLATE_LICENSE.rst` & `seppy-0.1.8/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/data/test/epi21106.rl2` & `seppy-0.1.8/seppy/data/test/epi21106.rl2`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/data/test/psp_isois-epihi_l2-het-rates60_20210531_v15.cdf` & `seppy-0.1.8/seppy/data/test/psp_isois-epihi_l2-het-rates60_20210531_v15.cdf`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/data/test/sept_ahead_ele_sun_2006_318_1min_l2_v03.dat` & `seppy-0.1.8/seppy/data/test/sept_ahead_ele_sun_2006_318_1min_l2_v03.dat`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/data/test/soho_erne-hed_l2-1min_20211028_v01.cdf` & `seppy-0.1.8/seppy/data/test/soho_erne-hed_l2-1min_20211028_v01.cdf`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/data/test/solo_l2_mag-rtn-normal-1-minute_20210712_v01.cdf` & `seppy-0.1.8/seppy/data/test/solo_l2_mag-rtn-normal-1-minute_20210712_v01.cdf`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/data/test/sta_l1_het_20211028_v01.cdf` & `seppy-0.1.8/seppy/data/test/sta_l1_het_20211028_v01.cdf`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/data/test/wi_sfsp_3dp_00000000_v01.cdf` & `seppy-0.1.8/seppy/data/test/wi_sfsp_3dp_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/data/test/wi_sfsp_3dp_20200213_v01.cdf` & `seppy-0.1.8/seppy/data/test/wi_sfsp_3dp_20200213_v01.cdf`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/loader/psp.py` & `seppy-0.1.8/seppy/loader/psp.py`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/loader/soho.py` & `seppy-0.1.8/seppy/loader/soho.py`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/loader/solo.py` & `seppy-0.1.8/seppy/loader/solo.py`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/loader/stereo.py` & `seppy-0.1.8/seppy/loader/stereo.py`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/loader/wind.py` & `seppy-0.1.8/seppy/loader/wind.py`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/tests/test_loader.py` & `seppy-0.1.8/seppy/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/tests/test_tools.py` & `seppy-0.1.8/seppy/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/tools/__init__.py` & `seppy-0.1.8/seppy/tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,23 @@
 from seppy.loader.solo import epd_load
 from seppy.loader.stereo import calc_av_en_flux_HET as calc_av_en_flux_ST_HET
 from seppy.loader.stereo import calc_av_en_flux_SEPT, stereo_load
 from seppy.loader.wind import wind3dp_load
 from seppy.util import *
 
 
-# TODO: This should be handled better, don't ignore all UserWarnings!
 # This is to get rid of this specific warning:
 # /home/user/xyz/serpentine/notebooks/sep_analysis_tools/read_swaves.py:96: UserWarning: The input coordinates to pcolormesh are interpreted as
 # cell centers, but are not monotonically increasing or decreasing. This may lead to incorrectly calculated cell edges, in which
 # case, please supply explicit cell edges to pcolormesh.
 # colormesh = ax.pcolormesh( time_arr, freq[::-1], data_arr[::-1], vmin = 0, vmax = 0.5*np.max(data_arr), cmap = 'inferno' )
-warnings.filterwarnings("ignore", category=UserWarning)
+warnings.filterwarnings(action="ignore",
+                        message="The input coordinates to pcolormesh are interpreted as cell centers, but are not monotonically increasing or \
+                        decreasing. This may lead to incorrectly calculated cell edges, in which case, please supply explicit cell edges to pcolormesh.",
+                        category=UserWarning)
 
 
 class Event:
 
     def __init__(self, start_date, end_date, spacecraft, sensor,
                  species, data_level, data_path, viewing=None, radio_spacecraft=None,
                  threshold=None):
@@ -45,15 +47,15 @@
             spacecraft = "stb"
 
         if sensor in ["ERNE-HED"]:
             sensor = "ERNE"
 
         if species in ("protons", "ions"):
             species = 'p'
-        if species == "electrons":
+        if species in ("electrons", "electron"):
             species = 'e'
 
         self.start_date = start_date
         self.end_date = end_date
         self.spacecraft = spacecraft.lower()
         self.sensor = sensor.lower()
         self.species = species.lower()
@@ -86,19 +88,32 @@
 
         # I think it could be worth considering to run self.choose_data(viewing) when the object is created,
         # because now it has to be run inside self.print_energies() to make sure that either
         # self.current_df, self.current_df_i or self.current_df_e exists, because print_energies() needs column
         # names from the dataframe.
         self.load_all_viewing()
 
+        # Check that the data that was loaded is valid. If not, give a warning.
+        self.validate_data()
+
         # Download radio cdf files ONLY if asked to
         if self.radio_spacecraft is not None:
             from seppy.tools.swaves import get_swaves
             self.radio_files = get_swaves(start_date, end_date)
 
+    def validate_data(self):
+        """
+        Provide an error msg if this object is initialized with a combination that yields invalid data products.
+        """
+
+        # Data products for SolO/STEP before 22 Oct 2021 are no reliable for non-Pixel Averaged data
+        if self.spacecraft == "solo" and self.sensor == "step":
+            if self.start_date < pd.to_datetime("2021-10-22").date():
+                warnings.warn("WARNING! SolO/STEP particle data is not included yet for individual Pixels for dates preceding 2022-10-22.")
+
     def update_onset_attributes(self, flux_series, onset_stats, onset_found, peak_flux, peak_time, fig, bg_mean):
         """
         Method to update onset-related attributes, that are None by default and only have values after analyse() has been run.
         """
         self.flux_series = flux_series
         self.onset_stats = onset_stats
         self.onset_found = onset_found
@@ -135,24 +150,37 @@
     # I suggest we at some point erase the arguments ´spacecraft´ and ´threshold´ due to them not being used.
     # `viewing` and `autodownload` are actually the only necessary input variables for this function, the rest
     # are class attributes, and should probably be cleaned up at some point
     def load_data(self, spacecraft, sensor, viewing, data_level,
                   autodownload=True, threshold=None):
 
         if self.spacecraft == 'solo':
-            df_i, df_e, energs = epd_load(sensor=sensor,
-                                          viewing=viewing,
-                                          level=data_level,
-                                          startdate=self.start_date,
-                                          enddate=self.end_date,
-                                          path=self.data_path,
-                                          autodownload=autodownload)
 
-            self.update_viewing(viewing)
-            return df_i, df_e, energs
+            if self.sensor in ("ept", "het"):
+                df_i, df_e, meta = epd_load(sensor=sensor,
+                                            viewing=viewing,
+                                            level=data_level,
+                                            startdate=self.start_date,
+                                            enddate=self.end_date,
+                                            path=self.data_path,
+                                            autodownload=autodownload)
+                # self.update_viewing(viewing) Why is viewing updated here?
+                return df_i, df_e, meta
+
+            elif self.sensor == "step":
+                df, meta = epd_load(sensor=sensor,
+                                    viewing="None",
+                                    level=data_level,
+                                    startdate=self.start_date,
+                                    enddate=self.end_date,
+                                    path=self.data_path,
+                                    autodownload=autodownload)
+
+                # self.update_viewing(viewing) Why is viewing updated here?
+                return df, meta
 
         if self.spacecraft[:2].lower() == 'st':
             if self.sensor == 'sept':
                 if self.species in ["p", "i"]:
                     df_i, channels_dict_df_i = stereo_load(instrument=self.sensor,
                                                            startdate=self.start_date,
                                                            enddate=self.end_date,
@@ -332,15 +360,15 @@
                 self.df_i_south, self.df_e_south, self.energies_south =\
                     self.load_data(self.spacecraft, self.sensor,
                                    'south', self.data_level)
 
             elif self.sensor == 'step':
 
                 self.df_step, self.energies_step =\
-                    self.load_data(self.spacecraft, self.sensor, 'None',
+                    self.load_data(self.spacecraft, self.sensor, self.viewing,
                                    self.data_level)
 
         if self.spacecraft[:2].lower() == 'st':
 
             if self.sensor == 'sept':
 
                 self.df_i_sun, self.df_e_sun, self.energies_i_sun, self.energies_e_sun =\
@@ -457,14 +485,31 @@
 
             elif viewing == 'south':
 
                 self.current_df_i = self.df_i_south
                 self.current_df_e = self.df_e_south
                 self.current_energies = self.energies_south
 
+            elif "Pixel" in viewing:
+
+                # All viewings are contained in the same dataframe, choose the pixel (viewing) here
+                pixel = self.viewing.split(' ')[1]
+
+                # Pixel info is in format NN in the dataframe, 1 -> 01 while 12 -> 12
+                if len(pixel) == 1:
+                    pixel = f"0{pixel}"
+
+                # Pixel length more than 2 means "averaged" -> called "Avg" in the dataframe
+                elif len(pixel) > 2:
+                    pixel = "Avg"
+
+                self.current_df_i = self.df_step[[col for col in self.df_step.columns if f"Magnet_{pixel}_Flux" in col]]
+                self.current_df_e = self.df_step[[col for col in self.df_step.columns if f"Electron_{pixel}_Flux" in col]]
+                self.current_energies = self.energies_step
+
         if self.spacecraft[:2].lower() == 'st':
             if self.sensor == 'sept':
                 if viewing == 'sun':
 
                     self.current_df_i = self.df_i_sun
                     self.current_df_e = self.df_e_sun
                     self.current_i_energies = self.energies_i_sun
@@ -1127,14 +1172,15 @@
             if (background_range[0] < xlim[0] - datetime.timedelta(days=1) and background_range[0] < xlim[1] - datetime.timedelta(days=1)) or \
                (background_range[1] > xlim[0] + datetime.timedelta(days=1) and background_range[1] > xlim[1] + datetime.timedelta(days=1)):
                 background_warning = "NOTICE that your background_range is separated from plot_range by over a day.\nIf this was intentional you may ignore this warning."
                 warnings.warn(message=background_warning)
 
         if (self.spacecraft[:2].lower() == 'st' and self.sensor == 'sept') \
                 or (self.spacecraft.lower() == 'psp' and self.sensor.startswith('isois')) \
+                or (self.spacecraft.lower() == 'solo' and self.sensor == 'step') \
                 or (self.spacecraft.lower() == 'solo' and self.sensor == 'ept') \
                 or (self.spacecraft.lower() == 'solo' and self.sensor == 'het') \
                 or (self.spacecraft.lower() == 'wind' and self.sensor == '3dp') \
                 or (self.spacecraft.lower() == 'bepi'):
             self.viewing_used = viewing
             self.choose_data(viewing)
         elif (self.spacecraft[:2].lower() == 'st' and self.sensor == 'het'):
@@ -1175,14 +1221,34 @@
                 elif self.species == 'e':
 
                     df_flux, en_channel_string =\
                         self.calc_av_en_flux_EPT(self.current_df_e,
                                                  self.current_energies,
                                                  channels)
 
+            elif self.sensor == "step":
+
+                if len(channels) > 1:
+                    not_implemented_msg = "Multiple channel averaging not yet supported for STEP! Please choose only one channel."
+                    raise Exception(not_implemented_msg)
+
+                en_channel_string = self.get_channel_energy_values("str")[channels[0]]
+
+                if self.species in ('p', 'i'):
+                    channel_id = self.current_df_i.columns[channels[0]]
+                    df_flux = pd.DataFrame(data={
+                        "flux": self.current_df_i[channel_id]
+                    }, index=self.current_df_i.index)
+
+                elif self.species == 'e':
+                    channel_id = self.current_df_e.columns[channels[0]]
+                    df_flux = pd.DataFrame(data={
+                        "flux": self.current_df_e[channel_id]
+                    }, index=self.current_df_e.index)
+
             else:
                 invalid_sensor_msg = "Invalid sensor!"
                 raise Exception(invalid_sensor_msg)
 
         if self.spacecraft[:2] == 'st':
 
             # Super ugly implementation, but easiest to just wrap both sept and het calculators
@@ -1362,15 +1428,16 @@
         self.update_onset_attributes(flux_series, onset_stats, onset_found, peak_flux.values[0], peak_time, fig, bg_mean)
 
         return flux_series, onset_stats, onset_found, peak_flux, peak_time, fig, bg_mean
 
     # For backwards compatibility, make a copy of the `find_onset` function that is called `analyse` (which was its old name).
     analyse = copy.copy(find_onset)
 
-    def dynamic_spectrum(self, view, cmap: str = 'magma', xlim: tuple = None, resample: str = None, save: bool = False) -> None:
+    def dynamic_spectrum(self, view, cmap: str = 'magma', xlim: tuple = None, resample: str = None, save: bool = False,
+                         other=None) -> None:
         """
         Shows all the different energy channels in a single 2D plot, and color codes the corresponding intensity*energy^2 by a colormap.
 
         Parameters:
         -----------
         view : str or None
                 The viewing direction of the sensor
@@ -1380,23 +1447,118 @@
                 Pandas-compatible datetime strings for the start and stop of the figure
         resample : str
                 Pandas-compatibe resampling string, e.g. '10min' or '30s'
         save : bool
                 Saves the image
         """
 
+        def get_yaxis_bin_boundaries(e_lows, e_highs, y_multiplier, is_solohetions):
+            """
+            Helper function to produce the bin boundaries for dynamic spectrum y-axis.
+            """
+
+            # For any other sc+instrument combination than solo+HET in the current version, there is no need to complicate setting bin boundaries
+            if not is_solohetions:
+                return np.append(e_lows, e_highs[-1]) * y_multiplier
+
+            # Init the boundaries. For SolO/HET there are more boundaries than channels
+            yaxis_bin_boundaries = np.zeros(len(e_lows)+2)
+            yaxis_idx = 0
+            chooser_idx = yaxis_idx
+            while yaxis_idx < len(yaxis_bin_boundaries)-1:  # this loop will not go to the final index of the array
+
+                # Set the first boundary as simply the first val of lower energy boundaries and continue
+                if yaxis_idx==0:
+                    yaxis_bin_boundaries[yaxis_idx] = e_lows[chooser_idx]
+                    yaxis_idx += 1
+                    chooser_idx += 1
+                    continue
+
+                # If the lower boundary now is the same as the last bins higher boundary, then set that as the boundary
+                if e_lows[chooser_idx] == e_highs[chooser_idx-1]:
+                    yaxis_bin_boundaries[yaxis_idx] = e_lows[chooser_idx]
+                    yaxis_idx += 1
+                    chooser_idx += 1
+
+                # ...if not, set the last higher boundary as the boundary, the next lower boundary as the next boundary and continue business as usual
+                else:
+                    yaxis_bin_boundaries[yaxis_idx] = e_highs[chooser_idx-1]
+                    yaxis_bin_boundaries[yaxis_idx+1] = e_lows[chooser_idx]
+
+                    yaxis_idx += 2
+                    chooser_idx += 1
+
+            # Finally the last boundary is the final boundary of e_highs:
+            yaxis_bin_boundaries[-1] = e_highs[-1]
+
+            return yaxis_bin_boundaries * y_multiplier
+
+        def combine_grids_and_ybins(grid, grid1, y_arr, y_arr1):
+            # solo/het lowest electron channel partially overlaps with ept highest channel -> erase the "extra" bin where overlapping hapens
+            if self.spacecraft == "solo" and (self.sensor == "het" or other.sensor == "het") and self.species in ("electrons", "electron", 'e'):
+
+                grid1 = np.append(grid, grid1, axis=0)[:-1]
+
+                # This deletes the first entry of y_arr1
+                y_arr1 = np.delete(y_arr1, 0, axis=0)
+                y_arr1 = np.append(y_arr, y_arr1)
+
+            # There is a gap between the highest solo/ept proton channel and the lowest het ion channel -> add extra row to grid
+            # filled with nans to compensate
+            elif self.spacecraft == "solo" and (self.sensor == "het" or other.sensor == "het") and self.species == 'p':
+
+                nans = np.array([[np.nan for i in range(len(grid[0]))]])
+                grid = np.append(grid, nans, axis=0)
+                grid1 = np.append(grid, grid1, axis=0)[:-2]
+                y_arr1 = np.append(y_arr, y_arr1)
+
+            else:
+
+                grid1 = np.append(grid, grid1, axis=0)
+                y_arr1 = np.append(y_arr, y_arr1)
+
+            return grid1, y_arr1
+
         # Event attributes
         spacecraft = self.spacecraft.lower()
         instrument = self.sensor.lower()
         species = self.species
 
+        # Boolean value for checking if y-axis requires a white stripe
+        is_solohetions = (spacecraft == "solo" and instrument == "het" and species == 'p')
+
+        # This method has to be run before doing anything else to make sure that the viewing is correct
         self.choose_data(view)
 
         if self.spacecraft == "solo":
-            if species in ("electron", 'e'):
+
+            if instrument == "step":
+
+                # All viewings are contained in the same dataframe, choose the pixel (viewing) here
+                pixel = self.viewing.split(' ')[1]
+
+                # Pixel info is in format NN in the dataframe, 1 -> 01 while 12 -> 12
+                if len(pixel) == 1:
+                    pixel = f"0{pixel}"
+
+                # Pixel length more than 2 means "averaged" -> called "Avg" in the dataframe
+                elif len(pixel) > 2:
+                    pixel = "Avg"
+
+                if species in ("electron", 'e'):
+                    particle_data = self.df_step[[col for col in self.df_step.columns if f"Electron_{pixel}_Flux" in col]]
+                    s_identifier = "electrons"
+
+                # Step's "Magnet" channel deflects electrons -> measures all positive ions
+                else:
+                    particle_data = self.df_step[[col for col in self.df_step.columns if f"Magnet_{pixel}_Flux" in col]]
+                    s_identifier = "ions"
+
+            # EPT and HET data come in almost identical containers, they need not be differentiated
+            elif species in ("electron", 'e'):
                 particle_data = self.current_df_e["Electron_Flux"]
                 s_identifier = "electrons"
             else:
                 try:
                     particle_data = self.current_df_i["Ion_Flux"]
                     s_identifier = "ions"
                 except KeyError:
@@ -1448,66 +1610,84 @@
                     s_identifier = "electrons"
                 else:
                     # change flux units from '#/cm2-ster-eV-sec' to '#/cm2-ster-MeV-sec'
                     particle_data = self.current_df_i*1e6
                     s_identifier = "protons"
 
         # These particle instruments will have keVs on their y-axis
-        LOW_ENERGY_SENSORS = ("sept", "ept")
+        LOW_ENERGY_SENSORS = ("sept", "step", "ept")
 
-        if instrument in LOW_ENERGY_SENSORS:
-            y_multiplier = 1e-3  # keV
-            y_unit = "keV"
+        # For a single instrument, check if low or high energy instrument, but for joint dynamic spectrum
+        # always use MeVs as the unit, because the y-axis is going to range over a large number of values
+        if not other:
+            if instrument in LOW_ENERGY_SENSORS:
+                y_multiplier = 1e-3  # keV
+                y_unit = "keV"
+            else:
+                y_multiplier = 1e-6  # MeV
+                y_unit = "MeV"
         else:
             y_multiplier = 1e-6  # MeV
             y_unit = "MeV"
 
         # Resample only if requested
         if resample is not None:
             particle_data = resample_df(df=particle_data, resample=resample)
 
         if xlim is None:
             df = particle_data[:]
             t_start, t_end = df.index[0], df.index[-1]
         else:
-            # td is added to the end to avert white pixels at the end of the plot
+            # td is added to the start and the end to avert white pixels at the end of the plot
             td_str = resample if resample is not None else '0s'
             td = pd.Timedelta(value=td_str)
             t_start, t_end = pd.to_datetime(xlim[0]), pd.to_datetime(xlim[1])
-            df = particle_data.loc[(particle_data.index >= t_start) & (particle_data.index <= (t_end+td))]
+            df = particle_data.loc[(particle_data.index >= (t_start-td)) & (particle_data.index <= (t_end+td))]
 
         # In practice this seeks the date on which the highest flux is observed
         date_of_event = df.iloc[np.argmax(df[df.columns[0]])].name.date()
 
         # Assert time and channel bins
         time = df.index
 
         # The low and high ends of each energy channel
         e_lows, e_highs = self.get_channel_energy_values()  # this function return energy in eVs
 
         # The mean energy of each channel in eVs
         mean_energies = np.sqrt(np.multiply(e_lows, e_highs))
 
-        # Energy boundaries of plotted bins in keVs are the y-axis:
-        y_arr = np.append(e_lows, e_highs[-1]) * y_multiplier
+        # Boundaries of plotted bins in keVs are the y-axis:
+        y_arr = get_yaxis_bin_boundaries(e_lows, e_highs, y_multiplier, is_solohetions)
 
         # Set image pixel length and height
         image_len = len(time)
         image_hei = len(y_arr)-1
 
         # Init the grid
         grid = np.zeros((image_len, image_hei))
 
         # Display energy in MeVs -> multiplier squared is 1e-6*1e-6 = 1e-12
-        energy_multiplier_squared = 1e-12
+        ENERGY_MULTIPLIER_SQUARED = 1e-12
 
         # Assign grid bins -> intensity * energy^2
-        for i, channel in enumerate(df):
+        if is_solohetions:
+            for i, channel in enumerate(df):
+
+                if i<5:
+                    grid[:, i] = df[channel]*(mean_energies[i]*mean_energies[i]*ENERGY_MULTIPLIER_SQUARED)
+                elif i==5:
+                    grid[:, i] = np.nan
+                    grid[:, i+1] = df[channel]*(mean_energies[i]*mean_energies[i]*ENERGY_MULTIPLIER_SQUARED)
+                else:
+                    grid[:, i+1] = df[channel]*(mean_energies[i]*mean_energies[i]*ENERGY_MULTIPLIER_SQUARED)
 
-            grid[:, i] = df[channel]*(mean_energies[i]*mean_energies[i]*energy_multiplier_squared)  # Intensity*Energy^2, and energy is in eV -> tranform to keV or MeV
+        else:
+            for i, channel in enumerate(df):
+
+                grid[:, i] = df[channel]*(mean_energies[i]*mean_energies[i]*ENERGY_MULTIPLIER_SQUARED)  # Intensity*Energy^2, and energy is in eV -> tranform to keV or MeV
 
         # Finally cut the last entry and transpose the grid so that it can be plotted correctly
         grid = grid[:-1, :]
         grid = grid.T
 
         maskedgrid = np.where(grid == 0, 0, 1)
         maskedgrid = np.ma.masked_where(maskedgrid == 1, maskedgrid)
@@ -1538,47 +1718,163 @@
             # plt.subplots_adjust(wspace=-1, hspace=-1.8)
 
             # Colorbar
             cb = fig.colorbar(colormesh, orientation='vertical', ax=ax[0])
             clabel = "Intensity" + "\n" + "[dB]"
             cb.set_label(clabel)
 
-        # Colormesh
-        cplot = ax[DYN_SPEC_INDX].pcolormesh(time, y_arr, grid, shading='auto', cmap=cmap, norm=normscale)
-        greymesh = ax[DYN_SPEC_INDX].pcolormesh(time, y_arr, maskedgrid, shading='auto', cmap='Greys', vmin=-1, vmax=1)
+        ax[DYN_SPEC_INDX].set_yscale('log')
 
         # Colorbar
-        cb = fig.colorbar(cplot, orientation='vertical', ax=ax[DYN_SPEC_INDX])
-        clabel = r"Intensity $\cdot$ $E^{2}$" + "\n" + r"[MeV/(cm$^{2}$ sr s)]"
-        cb.set_label(clabel)
+        if not other:
 
-        # y-axis settings
-        ax[DYN_SPEC_INDX].set_yscale('log')
-        ax[DYN_SPEC_INDX].set_ylim(np.nanmin(y_arr), np.nanmax(y_arr))
-        ax[DYN_SPEC_INDX].set_yticks([yval for yval in y_arr])
-        ax[DYN_SPEC_INDX].yaxis.set_major_formatter(ScalarFormatter(useMathText=True))
+            # Colormesh
+            cplot = ax[DYN_SPEC_INDX].pcolormesh(time, y_arr, grid, shading='auto', cmap=cmap, norm=normscale)
+            greymesh = ax[DYN_SPEC_INDX].pcolormesh(time, y_arr, maskedgrid, shading='auto', cmap='Greys', vmin=-1, vmax=1)
+
+            cb = fig.colorbar(cplot, orientation='vertical', ax=ax[DYN_SPEC_INDX])
+            clabel = r"Intensity $\cdot$ $E^{2}$" + "\n" + r"[MeV/(cm$^{2}$ sr s)]"
+            cb.set_label(clabel)
+
+            # y-axis settings
+            ax[DYN_SPEC_INDX].set_ylim(np.nanmin(y_arr), np.nanmax(y_arr))
+            ax[DYN_SPEC_INDX].set_yticks([yval for yval in y_arr])
+            ax[DYN_SPEC_INDX].set_ylabel(f"Energy [{y_unit}]")
+
+        # Format of y-axis: for single instrument use pretty numbers, for joint spectrum only powers of ten
+        if not other:
+            ax[DYN_SPEC_INDX].yaxis.set_major_formatter(ScalarFormatter(useMathText=True))
+        else:
+            ax[DYN_SPEC_INDX].yaxis.set_major_formatter(ScalarFormatter(useMathText=False))
 
         # gets rid of minor ticks and labels
         ax[DYN_SPEC_INDX].yaxis.set_tick_params(length=0, width=0, which='minor', labelsize=0.)
-        ax[DYN_SPEC_INDX].yaxis.set_tick_params(length=9., width=1.5, which='major')
-
-        ax[DYN_SPEC_INDX].set_ylabel(f"Energy [{y_unit}]")
+        ax[DYN_SPEC_INDX].yaxis.set_tick_params(length=12., width=2.0, which='major')
 
         # x-axis settings
         # ax[DYN_SPEC_INDX].set_xlabel("Time [HH:MM \nm-d]")
         ax[DYN_SPEC_INDX].xaxis_date()
         ax[DYN_SPEC_INDX].set_xlim(t_start, t_end)
         # ax[DYN_SPEC_INDX].xaxis.set_major_locator(mdates.HourLocator(interval = 1))
         # utc_dt_format1 = DateFormatter('%H:%M \n%m-%d')
         utc_dt_format1 = DateFormatter('%H:%M\n%b %d\n%Y')
         ax[DYN_SPEC_INDX].xaxis.set_major_formatter(utc_dt_format1)
         # ax.xaxis.set_minor_locator(mdates.MinuteLocator(interval = 5))
 
+        # Expand the spectrum to a second instrument (for now only for solo/ept + step or het)
+        if other and self.sensor == "ept" and other.sensor == "het":
+
+            is_solohetions = (other.sensor == "het" and species == 'p')
+
+            # This method has to be run before doing anything else to make sure that the viewing is correct
+            other.choose_data(other.viewing)
+
+            # EPT and HET data come in almost identical containers, they need not be differentiated
+            if species in ("electron", 'e'):
+                particle_data1 = other.current_df_e["Electron_Flux"]
+            else:
+                try:
+                    particle_data1 = other.current_df_i["Ion_Flux"]
+                except KeyError:
+                    particle_data1 = other.current_df_i["H_Flux"]
+
+            # Resample only if requested
+            if resample is not None:
+                particle_data1 = resample_df(df=particle_data1, resample=resample)
+
+            if xlim is None:
+                df1 = particle_data1[:]
+                # t_start, t_end = df.index[0], df.index[-1]
+            else:
+                # td is added to the start and the end to avert white pixels at the end of the plot
+                td_str = resample if resample is not None else '0s'
+                td = pd.Timedelta(value=td_str)
+                t_start, t_end = pd.to_datetime(xlim[0]), pd.to_datetime(xlim[1])
+                df1 = particle_data1.loc[(particle_data1.index >= (t_start-td)) & (particle_data1.index <= (t_end+td))]
+
+            # Assert time and channel bins
+            time1 = df.index
+
+            # The low and high ends of each energy channel
+            e_lows1, e_highs1 = other.get_channel_energy_values()  # this function return energy in eVs
+
+            # The mean energy of each channel in eVs
+            mean_energies1 = np.sqrt(np.multiply(e_lows1, e_highs1))
+
+            # Boundaries of plotted bins in keVs are the y-axis:
+            y_arr1 = get_yaxis_bin_boundaries(e_lows1, e_highs1, y_multiplier, is_solohetions)
+
+            # Set image pixel height (length was already set before)
+            # For solohet+ions we do not subtract 1 here, because there is an energy gap between EPT highest channel and
+            # HET lowest channel, hence requiring one "empty" bin in between
+            image_hei1 = len(y_arr1)+1 if is_solohetions else len(y_arr1)
+
+            # Init the grid
+            grid1 = np.zeros((image_len, image_hei1))
+
+            # Assign grid bins -> intensity * energy^2
+            if is_solohetions:
+                for i, channel in enumerate(df1):
+
+                    if i<5:
+                        grid1[:, i] = df1[channel]*(mean_energies1[i]*mean_energies1[i]*ENERGY_MULTIPLIER_SQUARED)
+                    elif i==5:
+                        grid1[:, i] = np.nan
+                        grid1[:, i+1] = df1[channel]*(mean_energies1[i]*mean_energies1[i]*ENERGY_MULTIPLIER_SQUARED)
+                    else:
+                        grid1[:, i+1] = df1[channel]*(mean_energies1[i]*mean_energies1[i]*ENERGY_MULTIPLIER_SQUARED)
+
+            else:
+                for i, channel in enumerate(df1):
+
+                    grid1[:, i] = df1[channel]*(mean_energies1[i]*mean_energies1[i]*ENERGY_MULTIPLIER_SQUARED)  # Intensity*Energy^2, and energy is in eV -> transform to keV or MeV
+
+            # Finally cut the last entry and transpose the grid1 so that it can be plotted correctly
+            grid1 = grid1[:-1, :]
+            grid1 = grid1.T
+
+            # grids and y-axis has to be fused together so they can be plotted in the same colormesh
+            grid1, y_arr1 = combine_grids_and_ybins(grid, grid1, y_arr, y_arr1)
+
+            maskedgrid1 = np.where(grid1 == 0, 0, 1)
+            maskedgrid1= np.ma.masked_where(maskedgrid1 == 1, maskedgrid1)
+
+            # return time1, y_arr1, grid1
+            # Colormesh
+            cplot1 = ax[DYN_SPEC_INDX].pcolormesh(time1, y_arr1, grid1, shading='auto', cmap=cmap, norm=normscale)
+            greymesh1 = ax[DYN_SPEC_INDX].pcolormesh(time1, y_arr1, maskedgrid1, shading='auto', cmap='Greys', vmin=-1, vmax=1)
+
+            # Updating the colorbar
+            cb = fig.colorbar(cplot1, orientation='vertical', ax=ax[DYN_SPEC_INDX])
+            clabel = r"Intensity $\cdot$ $E^{2}$" + "\n" + r"[MeV/(cm$^{2}$ sr s)]"
+            cb.set_label(clabel)
+
+            # y-axis settings
+            ax[DYN_SPEC_INDX].set_yscale('log')
+            ax[DYN_SPEC_INDX].set_ylim(np.nanmin(y_arr), np.nanmax(y_arr1))
+
+            # Set a rougher tickscale
+            energy_tick_powers = (-1, 1, 3) if species in ("electron", 'e') else (-1, 2, 4)
+            yticks = np.logspace(start=energy_tick_powers[0], stop=energy_tick_powers[1], num=energy_tick_powers[2])
+
+            # First one sets the ticks in place and the second one enlarges the tick labels (not the ticks, the numbers next to them)
+            ax[DYN_SPEC_INDX].set_yticks([yval for yval in yticks])
+            ax[DYN_SPEC_INDX].tick_params(axis='y', labelsize=32)
+
+            ax[DYN_SPEC_INDX].set_ylabel(f"Energy [{y_unit}]")
+
+            # Introduce minor ticks back
+            ax[DYN_SPEC_INDX].yaxis.set_tick_params(length=8., width=1.2, which='minor', labelsize=0.)
+
+            fig.set_size_inches((27, 18))
+
         # Title
-        if view is not None:
+        if view is not None and other:
+            title = f"{spacecraft.upper()}/{instrument.upper()}+{other.sensor.upper()} ({view}) {s_identifier}, {date_of_event}"
+        elif view:
             title = f"{spacecraft.upper()}/{instrument.upper()} ({view}) {s_identifier}, {date_of_event}"
         else:
             title = f"{spacecraft.upper()}/{instrument.upper()} {s_identifier}, {date_of_event}"
 
         if self.radio_spacecraft is None:
             ax[0].set_title(title)
         else:
@@ -1636,28 +1932,40 @@
         radial_distance_value = np.round(position.radius.value, 2)
 
         METERS_PER_AU = 1 * u.AU.to(u.m)
 
         self.choose_data(view)
 
         if self.spacecraft == "solo":
-            if species in ["electron", 'e']:
-                particle_data = self.current_df_e["Electron_Flux"]
-                s_identifier = "electrons"
-            else:
-                try:
-                    particle_data = self.current_df_i["Ion_Flux"]
+            if self.sensor == "step":
+
+                if species in ("electron", 'e'):
+                    particle_data = self.current_df_e
+                    s_identifier = "electrons"
+                else:
+                    particle_data = self.current_df_i
                     s_identifier = "ions"
-                except KeyError:
-                    particle_data = self.current_df_i["H_Flux"]
-                    s_identifier = "protons"
+
+            else:
+
+                if species in ("electron", 'e'):
+                    particle_data = self.current_df_e["Electron_Flux"]
+                    s_identifier = "electrons"
+                else:
+                    try:
+                        particle_data = self.current_df_i["Ion_Flux"]
+                        s_identifier = "ions"
+                    except KeyError:
+                        particle_data = self.current_df_i["H_Flux"]
+                        s_identifier = "protons"
+
             sc_identifier = "Solar Orbiter"
 
         if self.spacecraft[:2] == "st":
-            if species in ["electron", 'e']:
+            if species in ("electron", 'e'):
                 if instrument == "sept":
                     particle_data = self.current_df_e[[ch for ch in self.current_df_e.columns if ch[:2] == "ch"]]
                 else:
                     particle_data = self.current_df_e[[ch for ch in self.current_df_e.columns if "Flux" in ch]]
                 s_identifier = "electrons"
             else:
                 if instrument == "sept":
@@ -1866,15 +2174,15 @@
                 # The relevant part here is sliderobject["old"]! It saves the previous value of the slider!
                 timedelta_sec = shift_coefficients[i]*(slider.value - sliderobject["old"])
 
                 # Update the time value
                 line.set_xdata(line.get_xdata() - pd.Timedelta(seconds=timedelta_sec))
 
             # Update the path label artist
-            text.set_text(f"R={radial_distance_value:.2f} AU\nL = {slider.value} AU")
+            text.set_text(f"R={radial_distance_value:.2f} AU\nL = {np.round(slider.value,2)} AU")
 
             # Effectively this refreshes the figure
             fig.canvas.draw_idle()
 
         def normalize_axes(button):
             """
             this function connects the button to switching visibility of natural / normed curves
@@ -1916,44 +2224,43 @@
         lower_bounds : list of lower bounds of each energy channel in eVs
         higher_bounds : list of higher bounds of each energy channel in eVs
         """
 
         # First check by spacecraft, then by sensor
         if self.spacecraft == "solo":
 
-            # All solo energies are in the same object
+            # STEP, ETP and HET energies are in the same object
             energy_dict = self.current_energies
 
-            if self.species == 'e':
+            if self.species in ("electron", 'e'):
                 energy_ranges = energy_dict["Electron_Bins_Text"]
+
             else:
-                try:
-                    energy_ranges = energy_dict["Ion_Bins_Text"]
-                except KeyError:
-                    energy_ranges = energy_dict["H_Bins_Text"]
+                p_identifier =  "Ion_Bins_Text" if self.sensor == "ept" else "H_Bins_Text" if self.sensor == "het" else "Bins_Text"
+                energy_ranges = energy_dict[p_identifier]
 
             # Each element in the list is also a list with len==1, so fix that
             energy_ranges = [element[0] for element in energy_ranges]
 
         if self.spacecraft[:2] == "st":
 
             # STEREO/SEPT energies come in two different objects
             if self.sensor == "sept":
-                if self.species == 'e':
+                if self.species in ("electron", 'e'):
                     energy_df = self.current_e_energies
                 else:
                     energy_df = self.current_i_energies
 
                 energy_ranges = energy_df["ch_strings"].values
 
             # STEREO/HET energies all in the same dictionary
             else:
                 energy_dict = self.current_energies
 
-                if self.species == 'e':
+                if self.species in ("electron", 'e'):
                     energy_ranges = energy_dict["Electron_Bins_Text"]
                 else:
                     energy_ranges = energy_dict["Proton_Bins_Text"]
 
                 # Each element in the list is also a list with len==1, so fix that
                 energy_ranges = [element[0] for element in energy_ranges]
 
@@ -1993,15 +2300,15 @@
                     energies_high = energies + self.meta[f"Electron_Chan{chan}_Energy_DELTAPLUS"].filter(like=f"_P{self.viewing}").values
 
                     # Round the numbers to one decimal place
                     energies_low_rounded = np.round(energies_low, 1)
                     energies_high_rounded = np.round(energies_high, 1)
 
                     # I think nan values should be removed at this point. However, if we were to do that, then print_energies()
-                    # will not work anymore since tha number of channels and channel energy ranges won't be the same.
+                    # will not work anymore since the number of channels and channel energy ranges won't be the same.
                     # In the current state PSP/ISOIS-EPILO cannot be examined with dynamic_spectrum(), because there are nan values
                     # in the channel energy ranges.
                     # energies_low_rounded = np.array([val for val in energies_low_rounded if not np.isnan(val)])
                     # energies_high_rounded = np.array([val for val in energies_high_rounded if not np.isnan(val)])
 
                     # produce energy range strings from low and high boundaries
                     energy_ranges = np.array([str(energies_low_rounded[i]) + ' - ' + str(energies_high_rounded[i]) + " keV" for i in range(len(energies_low_rounded))])
@@ -2137,17 +2444,23 @@
         if self.species in ['p', 'i', 'H', "proton", "ion"]:
             channel_names = self.current_df_i.columns
             SOLO_EPT_CHANNELS_AMOUNT = 64
             SOLO_HET_CHANNELS_AMOUNT = 36
 
         # Extract only the numbers from channel names
         if self.spacecraft == "solo":
+
+            if self.sensor == "step":
+                channel_names = list(channel_names)
+                channel_numbers = np.array([int(name.split('_')[-1]) for name in channel_names])
+
             if self.sensor == "ept":
                 channel_names = [name[1] for name in channel_names[:SOLO_EPT_CHANNELS_AMOUNT]]
                 channel_numbers = np.array([int(name.split('_')[-1]) for name in channel_names])
+
             if self.sensor == "het":
                 channel_names = [name[1] for name in channel_names[:SOLO_HET_CHANNELS_AMOUNT]]
                 channel_numbers = np.array([int(name.split('_')[-1]) for name in channel_names])
 
         if self.spacecraft in ["sta", "stb"] or self.sensor == "erne":
             channel_numbers = np.array([int(name.split('_')[-1]) for name in channel_names])
```

### Comparing `seppy-0.1.7/seppy/tools/swaves.py` & `seppy-0.1.8/seppy/tools/swaves.py`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/seppy/tools/widgets.py` & `seppy-0.1.8/seppy/tools/widgets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 A library to run the interactive user interface in SEP event onset determination notebooks.
 
 @Author: Christian Palmroos <chospa@utu.fi>
-@Last updated: 2022-11-03
+@Last updated: 2023-03-24
 """
 
 
 # from importlib.resources import path
 import ipywidgets as widgets
 
 # a list of available spacecraft:
 list_of_sc = ["PSP", "SOHO", "Solar Orbiter", "STEREO-A", "STEREO-B", "Wind"]
 
 stereo_instr = ["SEPT", "HET"]  # ["LET", "SEPT", "HET"]
-solo_instr = ["EPT", "HET"]
+solo_instr = ["STEP", "EPT", "HET"]
 bepi_instr = ["SIXS-P"]
 soho_instr = ["ERNE-HED", "EPHIN"]
 psp_instr = ["isois-epihi", "isois-epilo"]
 wind_instr = ["3DP"]
 
 sensor_dict = {
     "STEREO-A": stereo_instr,
@@ -28,14 +28,16 @@
     "PSP": psp_instr,
     "Wind": wind_instr
 }
 
 view_dict = {
     ("STEREO-A", "SEPT"): ("sun", "asun", "north", "south"),
     ("STEREO-B", "SEPT"): ("sun", "asun", "north", "south"),
+    ("Solar Orbiter", "STEP"): ("Pixel averaged", "Pixel 1", "Pixel 2", "Pixel 3", "Pixel 4", "Pixel 5", "Pixel 6", "Pixel 7", "Pixel 8", "Pixel 9", "Pixel 10",
+                                "Pixel 11", "Pixel 12", "Pixel 13", "Pixel 14", "Pixel 15"),
     ("Solar Orbiter", "EPT"): ("sun", "asun", "north", "south"),
     ("Solar Orbiter", "HET"): ("sun", "asun", "north", "south"),
     ("Bepicolombo", "SIXS-P"): (0, 1, 2, 3, 4),
     ("PSP", "isois-epihi"): ("A", "B"),
     ("PSP", "isois-epilo"): ('3', '7'),  # ('0', '1', '2', '3', '4', '5', '6', '7')
     ("Wind", "3DP"): ('omnidirectional', 'sector 0', 'sector 1', 'sector 2', 'sector 3', 'sector 4', 'sector 5', 'sector 6', 'sector 7')
 }
@@ -43,14 +45,15 @@
 species_dict = {
     ("STEREO-A", "LET"): ("protons", "electrons"),
     ("STEREO-A", "SEPT"): ("ions", "electrons"),
     ("STEREO-A", "HET"): ("protons", "electrons"),
     ("STEREO-B", "LET"): ("protons", "electrons"),
     ("STEREO-B", "SEPT"): ("ions", "electrons"),
     ("STEREO-B", "HET"): ("protons", "electrons"),
+    ("Solar Orbiter", "STEP"): ("ions", "electrons"),
     ("Solar Orbiter", "EPT"): ("ions", "electrons"),
     ("Solar Orbiter", "HET"): ("protons", "electrons"),
     ("Bepicolombo", "SIXS-P"): ("protons", "electrons"),
     ("SOHO", "ERNE-HED"): ("protons",),
     ("SOHO", "EPHIN"): ("electrons",),
     ("PSP", "isois-epihi"): ("protons", "electrons"),
     ("PSP", "isois-epilo"): ("electrons",),
```

### Comparing `seppy-0.1.7/seppy.egg-info/PKG-INFO` & `seppy-0.1.8/seppy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seppy
-Version: 0.1.7
+Version: 0.1.8
 Summary: SEPpy
 Home-page: https://github.com/serpentine-h2020/SEPpy
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seppy-0.1.7/seppy.egg-info/SOURCES.txt` & `seppy-0.1.8/seppy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/setup.cfg` & `seppy-0.1.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 setup_requires = setuptools_scm
 install_requires = 
 	astropy
 	bs4
-	cdflib
+	cdflib < 1.0.0
 	datetime
 	drms
 	h5netcdf
 	ipykernel
 	ipywidgets
 	lxml
 	matplotlib
```

### Comparing `seppy-0.1.7/setup.py` & `seppy-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `seppy-0.1.7/tox.ini` & `seppy-0.1.8/tox.ini`

 * *Files identical despite different names*

