# Comparing `tmp/steam-pysigma-2023.6.2.tar.gz` & `tmp/steam-pysigma-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.6.2.tar", last modified: Fri Jun  2 13:10:50 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.6.3.tar", last modified: Mon Jun  5 09:31:51 2023, max compression
```

## Comparing `steam-pysigma-2023.6.2.tar` & `steam-pysigma-2023.6.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 13:10:50.022267 steam-pysigma-2023.6.2/
--rw-rw-rw-   0        0        0     1030 2023-06-02 13:10:50.021268 steam-pysigma-2023.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 13:10:50.022267 steam-pysigma-2023.6.2/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-02 13:08:47.000000 steam-pysigma-2023.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:10:49.984777 steam-pysigma-2023.6.2/steam_pysigma/
--rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.2/steam_pysigma/MainSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.2/steam_pysigma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:10:50.000982 steam-pysigma-2023.6.2/steam_pysigma/comsol/
--rw-rw-rw-   0        0        0    17426 2023-05-25 12:24:48.000000 steam-pysigma-2023.6.2/steam_pysigma/comsol/BuildComsolModel.py
--rw-rw-rw-   0        0        0    15166 2023-05-24 08:17:29.000000 steam-pysigma-2023.6.2/steam_pysigma/comsol/BuildGlobalVariables.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.2/steam_pysigma/comsol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:10:50.004147 steam-pysigma-2023.6.2/steam_pysigma/data/
--rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.2/steam_pysigma/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.2/steam_pysigma/data/DataSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.2/steam_pysigma/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:10:50.007146 steam-pysigma-2023.6.2/steam_pysigma/domain_generator/
--rw-rw-rw-   0        0        0    17229 2023-05-25 12:09:39.000000 steam-pysigma-2023.6.2/steam_pysigma/domain_generator/GeometryMultipole.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.2/steam_pysigma/domain_generator/__init__.py
--rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.6.2/steam_pysigma/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:10:50.010147 steam-pysigma-2023.6.2/steam_pysigma/parsers/
--rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.2/steam_pysigma/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.2/steam_pysigma/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:10:50.014267 steam-pysigma-2023.6.2/steam_pysigma/plotters/
--rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.2/steam_pysigma/plotters/PlotterPysigma.py
--rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.2/steam_pysigma/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.2/steam_pysigma/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:10:50.016268 steam-pysigma-2023.6.2/steam_pysigma/postprocessing/
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.2/steam_pysigma/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.2/steam_pysigma/postprocessing/postprocessing.py
--rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.2/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:10:50.020267 steam-pysigma-2023.6.2/steam_pysigma/utils/
--rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.2/steam_pysigma/utils/Util.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.2/steam_pysigma/utils/__init__.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.2/steam_pysigma/utils/make_folder_if_not_existing.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:10:49.990775 steam-pysigma-2023.6.2/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-06-02 13:10:46.000000 steam-pysigma-2023.6.2/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1005 2023-06-02 13:10:46.000000 steam-pysigma-2023.6.2/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 13:10:46.000000 steam-pysigma-2023.6.2/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-06-02 13:10:46.000000 steam-pysigma-2023.6.2/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-02 13:10:46.000000 steam-pysigma-2023.6.2/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.734510 steam-pysigma-2023.6.3/
+-rw-rw-rw-   0        0        0     1030 2023-06-05 09:31:51.734434 steam-pysigma-2023.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 09:31:51.734510 steam-pysigma-2023.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-05 09:30:46.000000 steam-pysigma-2023.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.695944 steam-pysigma-2023.6.3/steam_pysigma/
+-rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.3/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.3/steam_pysigma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.709087 steam-pysigma-2023.6.3/steam_pysigma/comsol/
+-rw-rw-rw-   0        0        0    17427 2023-06-05 09:30:46.000000 steam-pysigma-2023.6.3/steam_pysigma/comsol/BuildComsolModel.py
+-rw-rw-rw-   0        0        0    15166 2023-05-24 08:17:29.000000 steam-pysigma-2023.6.3/steam_pysigma/comsol/BuildGlobalVariables.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/comsol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.713087 steam-pysigma-2023.6.3/steam_pysigma/data/
+-rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.3/steam_pysigma/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.3/steam_pysigma/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.717198 steam-pysigma-2023.6.3/steam_pysigma/domain_generator/
+-rw-rw-rw-   0        0        0    17229 2023-05-25 12:09:39.000000 steam-pysigma-2023.6.3/steam_pysigma/domain_generator/GeometryMultipole.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/domain_generator/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.6.3/steam_pysigma/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.720199 steam-pysigma-2023.6.3/steam_pysigma/parsers/
+-rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.3/steam_pysigma/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.724328 steam-pysigma-2023.6.3/steam_pysigma/plotters/
+-rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.3/steam_pysigma/plotters/PlotterPysigma.py
+-rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.3/steam_pysigma/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.727329 steam-pysigma-2023.6.3/steam_pysigma/postprocessing/
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.3/steam_pysigma/postprocessing/postprocessing.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.3/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.732328 steam-pysigma-2023.6.3/steam_pysigma/utils/
+-rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.3/steam_pysigma/utils/Util.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.3/steam_pysigma/utils/make_folder_if_not_existing.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.703944 steam-pysigma-2023.6.3/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-06-05 09:31:47.000000 steam-pysigma-2023.6.3/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1005 2023-06-05 09:31:47.000000 steam-pysigma-2023.6.3/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 09:31:47.000000 steam-pysigma-2023.6.3/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-06-05 09:31:47.000000 steam-pysigma-2023.6.3/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-05 09:31:47.000000 steam-pysigma-2023.6.3/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.6.2/PKG-INFO` & `steam-pysigma-2023.6.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: SIGMA,CERN,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.2/README.md` & `steam-pysigma-2023.6.3/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/setup.py` & `steam-pysigma-2023.6.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.6.2",
+    version="2023.6.3",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/MainSIGMA.py` & `steam-pysigma-2023.6.3/steam_pysigma/MainSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/comsol/BuildComsolModel.py` & `steam-pysigma-2023.6.3/steam_pysigma/comsol/BuildComsolModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 
         geom_multipole = GeometryMultipole(self.g, self.roxie_data, model_data, self.bh_curve_database, self.input_conductor_params,
                                            self.settings_dict)
 
         self.domains = geom_multipole.build_magnet()
         self.wedge_areas = geom_multipole.wedge_areas
-        self.plot_magnet()
+        #self.plot_magnet()
         self.connect_create_MPH_model(self.domains)
         self.save_files_java()
         self.save_compile_and_open_bat()
 
     def setup_config_sigma(self):
         cfg = self.g.ConfigSigma()
         cfg.setComsolVersion(self.COMSOL_version)  # for sigma_60
```

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/comsol/BuildGlobalVariables.py` & `steam-pysigma-2023.6.3/steam_pysigma/comsol/BuildGlobalVariables.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/data/DataRoxieParser.py` & `steam-pysigma-2023.6.3/steam_pysigma/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/data/DataSIGMA.py` & `steam-pysigma-2023.6.3/steam_pysigma/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/domain_generator/GeometryMultipole.py` & `steam-pysigma-2023.6.3/steam_pysigma/domain_generator/GeometryMultipole.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/helpers.py` & `steam-pysigma-2023.6.3/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/parsers/ParserRoxie.py` & `steam-pysigma-2023.6.3/steam_pysigma/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/plotters/PlotterPysigma.py` & `steam-pysigma-2023.6.3/steam_pysigma/plotters/PlotterPysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/plotters/PlotterRoxie.py` & `steam-pysigma-2023.6.3/steam_pysigma/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/postprocessing/postprocessing.py` & `steam-pysigma-2023.6.3/steam_pysigma/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/pysigma.py` & `steam-pysigma-2023.6.3/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma/utils/Util.py` & `steam-pysigma-2023.6.3/steam_pysigma/utils/Util.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.2/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.6.3/steam_pysigma.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: SIGMA,CERN,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.2/steam_pysigma.egg-info/SOURCES.txt` & `steam-pysigma-2023.6.3/steam_pysigma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

