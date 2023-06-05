# Comparing `tmp/pycup-0.1.6.1.tar.gz` & `tmp/pycup-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pycup-0.1.6.1.tar", last modified: Wed Apr 19 17:33:58 2023, max compression
+gzip compressed data, was "dist\pycup-0.1.7.tar", last modified: Mon Jun  5 15:17:06 2023, max compression
```

## Comparing `pycup-0.1.6.1.tar` & `pycup-0.1.7.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 17:33:58.471872 pycup-0.1.6.1/
--rw-rw-rw-   0        0        0     6333 2023-04-19 17:33:58.470872 pycup-0.1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     5077 2023-04-19 15:26:08.000000 pycup-0.1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 17:33:58.454869 pycup-0.1.6.1/pycup/
--rw-rw-rw-   0        0        0    17161 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/GLUE.py
--rw-rw-rw-   0        0        0    38271 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/GWO.py
--rw-rw-rw-   0        0        0    33260 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/MFO.py
--rw-rw-rw-   0        0        0    14600 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/MODE.py
--rw-rw-rw-   0        0        0    24212 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/MOPSO.py
--rw-rw-rw-   0        0        0    14937 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/NSGA2.py
--rw-rw-rw-   0        0        0    19287 2023-04-19 17:27:49.000000 pycup-0.1.6.1/pycup/PESTclasses.py
--rw-rw-rw-   0        0        0    35498 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/PSO.py
--rw-rw-rw-   0        0        0    15659 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/Reslib.py
--rw-rw-rw-   0        0        0    30073 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/SCA.py
--rw-rw-rw-   0        0        0    32941 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/SOA.py
--rw-rw-rw-   0        0        0    32160 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/SSA.py
--rw-rw-rw-   0        0        0     5757 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/TOPSIS.py
--rw-rw-rw-   0        0        0    33343 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/TSA.py
--rw-rw-rw-   0        0        0    32912 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/WOA.py
--rw-rw-rw-   0        0        0      946 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/__init__.py
--rw-rw-rw-   0        0        0    10042 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/calc_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:33:58.467872 pycup-0.1.6.1/pycup/document/
--rw-rw-rw-   0        0        0   826264 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/document/Documentation.pdf
--rw-rw-rw-   0        0        0     4027 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/evaluation_metrics.py
--rw-rw-rw-   0        0        0    53886 2023-04-19 17:14:13.000000 pycup-0.1.6.1/pycup/integrate.py
--rw-rw-rw-   0        0        0     7263 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/multi_jobs.py
--rw-rw-rw-   0        0        0   125408 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/plot.py
--rw-rw-rw-   0        0        0      460 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/progress_bar.py
--rw-rw-rw-   0        0        0    10352 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/sampling.py
--rw-rw-rw-   0        0        0    18935 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/save.py
--rw-rw-rw-   0        0        0     2068 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/template.py
--rw-rw-rw-   0        0        0        0 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/test.py
--rw-rw-rw-   0        0        0     6055 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/test_functions.py
--rw-rw-rw-   0        0        0    69170 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/uncertainty_analysis_fun.py
--rw-rw-rw-   0        0        0    17048 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/utilize.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:33:58.464925 pycup-0.1.6.1/pycup.egg-info/
--rw-rw-rw-   0        0        0     6333 2023-04-19 17:33:58.000000 pycup-0.1.6.1/pycup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-19 17:33:58.000000 pycup-0.1.6.1/pycup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 17:33:58.000000 pycup-0.1.6.1/pycup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-19 17:33:58.000000 pycup-0.1.6.1/pycup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 17:33:58.000000 pycup-0.1.6.1/pycup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 17:33:58.471872 pycup-0.1.6.1/setup.cfg
--rw-rw-rw-   0        0        0      955 2023-04-19 17:32:30.000000 pycup-0.1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:17:06.656476 pycup-0.1.7/
+-rw-rw-rw-   0        0        0     6366 2023-06-05 15:17:06.655476 pycup-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5112 2023-06-05 15:14:54.000000 pycup-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 15:17:06.641472 pycup-0.1.7/pycup/
+-rw-rw-rw-   0        0        0    17161 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/GLUE.py
+-rw-rw-rw-   0        0        0    38271 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/GWO.py
+-rw-rw-rw-   0        0        0    33260 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/MFO.py
+-rw-rw-rw-   0        0        0    14600 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/MODE.py
+-rw-rw-rw-   0        0        0    26156 2023-06-05 14:09:02.000000 pycup-0.1.7/pycup/MOMFO.py
+-rw-rw-rw-   0        0        0    24212 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/MOPSO.py
+-rw-rw-rw-   0        0        0    14937 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/NSGA2.py
+-rw-rw-rw-   0        0        0    19287 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/PESTclasses.py
+-rw-rw-rw-   0        0        0    35498 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/PSO.py
+-rw-rw-rw-   0        0        0    15659 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/Reslib.py
+-rw-rw-rw-   0        0        0    30073 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/SCA.py
+-rw-rw-rw-   0        0        0    32941 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/SOA.py
+-rw-rw-rw-   0        0        0    32160 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/SSA.py
+-rw-rw-rw-   0        0        0     5757 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/TOPSIS.py
+-rw-rw-rw-   0        0        0    33343 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/TSA.py
+-rw-rw-rw-   0        0        0    32912 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/WOA.py
+-rw-rw-rw-   0        0        0      975 2023-06-05 14:17:37.000000 pycup-0.1.7/pycup/__init__.py
+-rw-rw-rw-   0        0        0    10042 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/calc_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:17:06.652475 pycup-0.1.7/pycup/document/
+-rw-rw-rw-   0        0        0   826264 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/document/Documentation.pdf
+-rw-rw-rw-   0        0        0     4027 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/evaluation_metrics.py
+-rw-rw-rw-   0        0        0    53886 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/integrate.py
+-rw-rw-rw-   0        0        0     7263 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/multi_jobs.py
+-rw-rw-rw-   0        0        0   125408 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/plot.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/progress_bar.py
+-rw-rw-rw-   0        0        0    10352 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/sampling.py
+-rw-rw-rw-   0        0        0    19081 2023-06-05 14:17:37.000000 pycup-0.1.7/pycup/save.py
+-rw-rw-rw-   0        0        0     2068 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/template.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/test.py
+-rw-rw-rw-   0        0        0     6055 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/test_functions.py
+-rw-rw-rw-   0        0        0    69170 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/uncertainty_analysis_fun.py
+-rw-rw-rw-   0        0        0    17048 2023-06-05 14:05:02.000000 pycup-0.1.7/pycup/utilize.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:17:06.650474 pycup-0.1.7/pycup.egg-info/
+-rw-rw-rw-   0        0        0     6366 2023-06-05 15:17:06.000000 pycup-0.1.7/pycup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-06-05 15:17:06.000000 pycup-0.1.7/pycup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:17:06.000000 pycup-0.1.7/pycup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-05 15:17:06.000000 pycup-0.1.7/pycup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 15:17:06.000000 pycup-0.1.7/pycup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:17:06.656476 pycup-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-06-05 14:17:37.000000 pycup-0.1.7/setup.py
```

### Comparing `pycup-0.1.6.1/PKG-INFO` & `pycup-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pycup
-Version: 0.1.6.1
+Version: 0.1.7
 Summary: An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.
 Home-page: https://github.com/QianyangWang/PyCUP
 Author: Qianyang Wang
 Author-email: wqy07010944@hotmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/QianyangWang/PyCUP/DOCUMENT
 Project-URL: Source, https://github.com/QianyangWang/PyCUP/pycup
 Description: # PyCUP
         
-        <img src="https://img.shields.io/badge/Version-0.1.6-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
+        <img src="https://img.shields.io/badge/Version-0.1.7-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
         
         This is an open-source package designed for (environmental) model calibration and uncertainty analysis. The current version is the very first version, we welcome all comments, suggestions, and improvements.
         
-        ## v 0.1.6 Update
+        ## v 0.1.7 Update
         
-        PyCUP now supports a basic integration with PEST++ calibration project for a more convenient model-agnostic calibration process. The pycup.integrate.PESTconvertor can generate an objective function, which can read/write the parameter file, run the commandline, read the simulation results with the PEST++ instruction files. The function can be used by PyCUP algorithms so that users can do the calibration without writting the objective function and IO functions by themselves. As the PyCUP algorithms have mechanisms differ from which used by PEST++, some settings in PEST++ control file will be ignored. More details can be found in the example in documentations in the repository.
+        A new superior algorithm MOMFO (multi-objective moth-flame optimizer)  based on archive and crowding distance non-domination sort, and its elite-opposition improved version (EO-MOMFO) have been designed and provided in the new version. The elite opposition mechanism was modified based on the concept of non-domination and was embedded for updating the flame population of MOMFO. The implemented MOMFO has a similar principle as the current literature, although with some differences in details, while the elite-opposition version is original in this package.
         
         ## What does it have
         
         ### (1) For model calibration/optimization
         
         1. Single-objective heuristic algorithms including PSO, GWO, MFO, SOA, SCA, SSA, TSA, and WOA.
         2. Multi-objective heuristic algorithms including MOPSO, MODE, and NSGA-II.
@@ -40,15 +40,15 @@
         2. Recording and resuming during the calibration task.
         3. Several result plotting functions.
         4. A special simulation result object  for multi-station & multi-event results (of environmental models) in pycup.ResLib.
         
         ### (4) Package/Tools integration
         
         1. PyCUP can be linked to spotpy database for post-processing, a pycup objective function can also be generated from the spotpy objective function using the module named pycup.integrate.
-        2. The required objective function for pycup calibration can be easily generated using a PEST++ optimization project with/without a tsproc.exe. The PESTconvertor object in pycup.integrate provides several APIs for reading PEST++ files such as .pst, .ins, and .tpl.
+        2. A basic integration with PEST++ IO operations for model-agnostic calibrations. Details and  limitations are provided in the specific documentation. The required objective function for pycup calibration can be easily generated using a PEST++ optimization project with/without a tsproc.exe. The PESTconvertor object in pycup.integrate provides several APIs for reading PEST++ files such as .pst, .ins, and .tpl.
         
         ## How to install
         
         ​	The project has been uploaded onto the PyPI https://pypi.org/project/pycup/ . Or install the .whl file in the dist folder.
         
         ```
         pip install pycup
@@ -72,15 +72,15 @@
         lb = -100 * np.ones(30)
         ub = 100 * np.ones(30)
         cp.SSA.run(pop = 1000, dim = 30, lb = lb, ub = ub, MaxIter = 30, fun = uni_fun1)
         ```
         
         ## Example SWMM (Storm Water Management Model) calibration projects
         
-        ***IMPORTANT: PLEASE OPEN YOUR PYCHARM OR COMMAND LINE WITH THE ADMINISTRATOR RIGHTS BEFORE EXECUTING THE EXAMPLE PROJECT***
+        ***IMPORTANT: PLEASE OPEN YOUR IDE (e.g. PYCHARM) OR COMMAND LINE WITH THE ADMINISTRATOR RIGHTS BEFORE EXECUTING THE EXAMPLE PROJECT***
         
         #### Location: https://github.com/QianyangWang/PyCUP
         
         1. The example in folder 'Example01-GLUE' contains an SWMM calibration project using single-processing GLUE. Install the dependencies (for example: pip install swmm-api==0.2.0.18.3, pip install pyswmm). Execute the 'Calibrate.py' to calibrate the model. Then, execute the 'PostProcessing.py' for uncertainty analysis.
         2. The example in folder 'Example02-multiprocessing' contains an SWMM calibration project using multi-processing EOGWO.
         3. The example in folder 'Example03-multiobjective' contains an SWMM multi-objective calibration project using EOMOPSO. 
         4. The example in folder 'Example04-validation&prediction' shows how to use our (Ensemble)Validator/(Ensemble)Predictor objects for the validation and prediction of the model using the calibrated parameter (set).
```

### Comparing `pycup-0.1.6.1/README.md` & `pycup-0.1.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # PyCUP
 
-<img src="https://img.shields.io/badge/Version-0.1.6-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
+<img src="https://img.shields.io/badge/Version-0.1.7-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
 
 This is an open-source package designed for (environmental) model calibration and uncertainty analysis. The current version is the very first version, we welcome all comments, suggestions, and improvements.
 
-## v 0.1.6 Update
+## v 0.1.7 Update
 
-PyCUP now supports a basic integration with PEST++ calibration project for a more convenient model-agnostic calibration process. The pycup.integrate.PESTconvertor can generate an objective function, which can read/write the parameter file, run the commandline, read the simulation results with the PEST++ instruction files. The function can be used by PyCUP algorithms so that users can do the calibration without writting the objective function and IO functions by themselves. As the PyCUP algorithms have mechanisms differ from which used by PEST++, some settings in PEST++ control file will be ignored. More details can be found in the example in documentations in the repository.
+A new superior algorithm MOMFO (multi-objective moth-flame optimizer)  based on archive and crowding distance non-domination sort, and its elite-opposition improved version (EO-MOMFO) have been designed and provided in the new version. The elite opposition mechanism was modified based on the concept of non-domination and was embedded for updating the flame population of MOMFO. The implemented MOMFO has a similar principle as the current literature, although with some differences in details, while the elite-opposition version is original in this package.
 
 ## What does it have
 
 ### (1) For model calibration/optimization
 
 1. Single-objective heuristic algorithms including PSO, GWO, MFO, SOA, SCA, SSA, TSA, and WOA.
 2. Multi-objective heuristic algorithms including MOPSO, MODE, and NSGA-II.
@@ -30,15 +30,15 @@
 2. Recording and resuming during the calibration task.
 3. Several result plotting functions.
 4. A special simulation result object  for multi-station & multi-event results (of environmental models) in pycup.ResLib.
 
 ### (4) Package/Tools integration
 
 1. PyCUP can be linked to spotpy database for post-processing, a pycup objective function can also be generated from the spotpy objective function using the module named pycup.integrate.
-2. The required objective function for pycup calibration can be easily generated using a PEST++ optimization project with/without a tsproc.exe. The PESTconvertor object in pycup.integrate provides several APIs for reading PEST++ files such as .pst, .ins, and .tpl.
+2. A basic integration with PEST++ IO operations for model-agnostic calibrations. Details and  limitations are provided in the specific documentation. The required objective function for pycup calibration can be easily generated using a PEST++ optimization project with/without a tsproc.exe. The PESTconvertor object in pycup.integrate provides several APIs for reading PEST++ files such as .pst, .ins, and .tpl.
 
 ## How to install
 
 ​	The project has been uploaded onto the PyPI https://pypi.org/project/pycup/ . Or install the .whl file in the dist folder.
 
 ```
 pip install pycup
@@ -62,15 +62,15 @@
 lb = -100 * np.ones(30)
 ub = 100 * np.ones(30)
 cp.SSA.run(pop = 1000, dim = 30, lb = lb, ub = ub, MaxIter = 30, fun = uni_fun1)
 ```
 
 ## Example SWMM (Storm Water Management Model) calibration projects
 
-***IMPORTANT: PLEASE OPEN YOUR PYCHARM OR COMMAND LINE WITH THE ADMINISTRATOR RIGHTS BEFORE EXECUTING THE EXAMPLE PROJECT***
+***IMPORTANT: PLEASE OPEN YOUR IDE (e.g. PYCHARM) OR COMMAND LINE WITH THE ADMINISTRATOR RIGHTS BEFORE EXECUTING THE EXAMPLE PROJECT***
 
 #### Location: https://github.com/QianyangWang/PyCUP
 
 1. The example in folder 'Example01-GLUE' contains an SWMM calibration project using single-processing GLUE. Install the dependencies (for example: pip install swmm-api==0.2.0.18.3, pip install pyswmm). Execute the 'Calibrate.py' to calibrate the model. Then, execute the 'PostProcessing.py' for uncertainty analysis.
 2. The example in folder 'Example02-multiprocessing' contains an SWMM calibration project using multi-processing EOGWO.
 3. The example in folder 'Example03-multiobjective' contains an SWMM multi-objective calibration project using EOMOPSO. 
 4. The example in folder 'Example04-validation&prediction' shows how to use our (Ensemble)Validator/(Ensemble)Predictor objects for the validation and prediction of the model using the calibrated parameter (set).
```

### Comparing `pycup-0.1.6.1/pycup/GLUE.py` & `pycup-0.1.7/pycup/GLUE.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/GWO.py` & `pycup-0.1.7/pycup/GWO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/MFO.py` & `pycup-0.1.7/pycup/MFO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/MODE.py` & `pycup-0.1.7/pycup/MODE.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/MOPSO.py` & `pycup-0.1.7/pycup/MOPSO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/NSGA2.py` & `pycup-0.1.7/pycup/NSGA2.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/PESTclasses.py` & `pycup-0.1.7/pycup/PESTclasses.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/PSO.py` & `pycup-0.1.7/pycup/PSO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/Reslib.py` & `pycup-0.1.7/pycup/Reslib.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/SCA.py` & `pycup-0.1.7/pycup/SCA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/SOA.py` & `pycup-0.1.7/pycup/SOA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/SSA.py` & `pycup-0.1.7/pycup/SSA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/TOPSIS.py` & `pycup-0.1.7/pycup/TOPSIS.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/TSA.py` & `pycup-0.1.7/pycup/TSA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/WOA.py` & `pycup-0.1.7/pycup/WOA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/__init__.py` & `pycup-0.1.7/pycup/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 from . import PSO
 from . import MOPSO
 from . import GLUE
 from . import GWO
 from . import MFO
 from . import MODE
 from . import NSGA2
+from . import MOMFO
 from . import utilize
 from . import TOPSIS
 from . import Reslib
 from . import calc_utils
 from . import integrate
 from . import PESTclasses
 
 
 
 __all__ = ['evaluation_metrics','utilize', 'multi_jobs','plot','progress_bar',
            'sampling','save','test_functions','uncertainty_analysis_fun',
-           'WOA','TSA','SCA','SOA','SSA','PSO','GLUE','GWO','MFO',
+           'WOA','TSA','SCA','SOA','SSA','PSO','GLUE','GWO','MFO',"MOMFO",
            'MOPSO','MODE','NSGA2','template', 'TOPSIS',"Reslib","calc_utils","integrate",
            "PESTclasses"]
```

### Comparing `pycup-0.1.6.1/pycup/calc_utils.py` & `pycup-0.1.7/pycup/calc_utils.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/document/Documentation.pdf` & `pycup-0.1.7/pycup/document/Documentation.pdf`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/evaluation_metrics.py` & `pycup-0.1.7/pycup/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/integrate.py` & `pycup-0.1.7/pycup/integrate.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/multi_jobs.py` & `pycup-0.1.7/pycup/multi_jobs.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/plot.py` & `pycup-0.1.7/pycup/plot.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/sampling.py` & `pycup-0.1.7/pycup/sampling.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/save.py` & `pycup-0.1.7/pycup/save.py`

 * *Files 0% similar despite different names*

```diff
@@ -475,15 +475,17 @@
         self.iteration = iteration
         self.mode = mode
 
 
 class MOswarmRecord(RecordSaver):
 
     def __init__(self,pop,dim,lb,ub,hf,hs,hr,X,iteration,n_obj,V=None,
-                 archive=None,arFits=None,arRes=None,Pbest=None,fitnessPbest=None,fitnessGbest = None,GbestPositon=None,fitness=None,res=None):
+                 archive=None,arFits=None,arRes=None,Pbest=None,fitnessPbest=None,
+                 fitnessGbest = None,GbestPositon=None,fitness=None,res=None,Xs=None,
+                 fitnessS=None,resS=None):
         self.pop = pop
         self.dim = dim
         self.lb = lb
         self.ub = ub
         self.hf = hf
         self.hs = hs
         self.hr = hr
@@ -496,7 +498,10 @@
         self.archive = archive
         self.arFits = arFits
         self.arRes = arRes
         self.Pbest = Pbest
         self.fitnessPbest = fitnessPbest
         self.GbestPositon = GbestPositon
         self.fitnessGbest = fitnessGbest
+        self.Xs=Xs
+        self.fitnessS=fitnessS
+        self.resS=resS
```

### Comparing `pycup-0.1.6.1/pycup/template.py` & `pycup-0.1.7/pycup/template.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/test_functions.py` & `pycup-0.1.7/pycup/test_functions.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/uncertainty_analysis_fun.py` & `pycup-0.1.7/pycup/uncertainty_analysis_fun.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup/utilize.py` & `pycup-0.1.7/pycup/utilize.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6.1/pycup.egg-info/PKG-INFO` & `pycup-0.1.7/pycup.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pycup
-Version: 0.1.6.1
+Version: 0.1.7
 Summary: An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.
 Home-page: https://github.com/QianyangWang/PyCUP
 Author: Qianyang Wang
 Author-email: wqy07010944@hotmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/QianyangWang/PyCUP/DOCUMENT
 Project-URL: Source, https://github.com/QianyangWang/PyCUP/pycup
 Description: # PyCUP
         
-        <img src="https://img.shields.io/badge/Version-0.1.6-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
+        <img src="https://img.shields.io/badge/Version-0.1.7-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
         
         This is an open-source package designed for (environmental) model calibration and uncertainty analysis. The current version is the very first version, we welcome all comments, suggestions, and improvements.
         
-        ## v 0.1.6 Update
+        ## v 0.1.7 Update
         
-        PyCUP now supports a basic integration with PEST++ calibration project for a more convenient model-agnostic calibration process. The pycup.integrate.PESTconvertor can generate an objective function, which can read/write the parameter file, run the commandline, read the simulation results with the PEST++ instruction files. The function can be used by PyCUP algorithms so that users can do the calibration without writting the objective function and IO functions by themselves. As the PyCUP algorithms have mechanisms differ from which used by PEST++, some settings in PEST++ control file will be ignored. More details can be found in the example in documentations in the repository.
+        A new superior algorithm MOMFO (multi-objective moth-flame optimizer)  based on archive and crowding distance non-domination sort, and its elite-opposition improved version (EO-MOMFO) have been designed and provided in the new version. The elite opposition mechanism was modified based on the concept of non-domination and was embedded for updating the flame population of MOMFO. The implemented MOMFO has a similar principle as the current literature, although with some differences in details, while the elite-opposition version is original in this package.
         
         ## What does it have
         
         ### (1) For model calibration/optimization
         
         1. Single-objective heuristic algorithms including PSO, GWO, MFO, SOA, SCA, SSA, TSA, and WOA.
         2. Multi-objective heuristic algorithms including MOPSO, MODE, and NSGA-II.
@@ -40,15 +40,15 @@
         2. Recording and resuming during the calibration task.
         3. Several result plotting functions.
         4. A special simulation result object  for multi-station & multi-event results (of environmental models) in pycup.ResLib.
         
         ### (4) Package/Tools integration
         
         1. PyCUP can be linked to spotpy database for post-processing, a pycup objective function can also be generated from the spotpy objective function using the module named pycup.integrate.
-        2. The required objective function for pycup calibration can be easily generated using a PEST++ optimization project with/without a tsproc.exe. The PESTconvertor object in pycup.integrate provides several APIs for reading PEST++ files such as .pst, .ins, and .tpl.
+        2. A basic integration with PEST++ IO operations for model-agnostic calibrations. Details and  limitations are provided in the specific documentation. The required objective function for pycup calibration can be easily generated using a PEST++ optimization project with/without a tsproc.exe. The PESTconvertor object in pycup.integrate provides several APIs for reading PEST++ files such as .pst, .ins, and .tpl.
         
         ## How to install
         
         ​	The project has been uploaded onto the PyPI https://pypi.org/project/pycup/ . Or install the .whl file in the dist folder.
         
         ```
         pip install pycup
@@ -72,15 +72,15 @@
         lb = -100 * np.ones(30)
         ub = 100 * np.ones(30)
         cp.SSA.run(pop = 1000, dim = 30, lb = lb, ub = ub, MaxIter = 30, fun = uni_fun1)
         ```
         
         ## Example SWMM (Storm Water Management Model) calibration projects
         
-        ***IMPORTANT: PLEASE OPEN YOUR PYCHARM OR COMMAND LINE WITH THE ADMINISTRATOR RIGHTS BEFORE EXECUTING THE EXAMPLE PROJECT***
+        ***IMPORTANT: PLEASE OPEN YOUR IDE (e.g. PYCHARM) OR COMMAND LINE WITH THE ADMINISTRATOR RIGHTS BEFORE EXECUTING THE EXAMPLE PROJECT***
         
         #### Location: https://github.com/QianyangWang/PyCUP
         
         1. The example in folder 'Example01-GLUE' contains an SWMM calibration project using single-processing GLUE. Install the dependencies (for example: pip install swmm-api==0.2.0.18.3, pip install pyswmm). Execute the 'Calibrate.py' to calibrate the model. Then, execute the 'PostProcessing.py' for uncertainty analysis.
         2. The example in folder 'Example02-multiprocessing' contains an SWMM calibration project using multi-processing EOGWO.
         3. The example in folder 'Example03-multiobjective' contains an SWMM multi-objective calibration project using EOMOPSO. 
         4. The example in folder 'Example04-validation&prediction' shows how to use our (Ensemble)Validator/(Ensemble)Predictor objects for the validation and prediction of the model using the calibrated parameter (set).
```

### Comparing `pycup-0.1.6.1/pycup.egg-info/SOURCES.txt` & `pycup-0.1.7/pycup.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 pycup/GLUE.py
 pycup/GWO.py
 pycup/MFO.py
 pycup/MODE.py
+pycup/MOMFO.py
 pycup/MOPSO.py
 pycup/NSGA2.py
 pycup/PESTclasses.py
 pycup/PSO.py
 pycup/Reslib.py
 pycup/SCA.py
 pycup/SOA.py
```

### Comparing `pycup-0.1.6.1/setup.py` & `pycup-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open(r"README.md",encoding="utf-8") as f:
   long_description = f.read()
 
 
 setup(
     name='pycup',
-  version='0.1.6.1',
+  version='0.1.7',
   description='An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Qianyang Wang',
   author_email='wqy07010944@hotmail.com',
   url='https://github.com/QianyangWang/PyCUP',
   license='MIT License',
```

