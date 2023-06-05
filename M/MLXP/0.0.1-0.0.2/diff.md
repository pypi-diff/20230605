# Comparing `tmp/MLXP-0.0.1.tar.gz` & `tmp/MLXP-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLXP-0.0.1.tar", last modified: Mon Jun  5 18:39:36 2023, max compression
+gzip compressed data, was "MLXP-0.0.2.tar", last modified: Mon Jun  5 18:45:47 2023, max compression
```

## Comparing `MLXP-0.0.1.tar` & `MLXP-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:39:36.386372 MLXP-0.0.1/
-drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:39:36.381449 MLXP-0.0.1/MLXP.egg-info/
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     5185 2023-06-05 18:39:36.000000 MLXP-0.0.1/MLXP.egg-info/PKG-INFO
--rw-r--r--   0 MichaelArbel   (501) staff       (20)      754 2023-06-05 18:39:36.000000 MLXP-0.0.1/MLXP.egg-info/SOURCES.txt
--rw-r--r--   0 MichaelArbel   (501) staff       (20)        1 2023-06-05 18:39:36.000000 MLXP-0.0.1/MLXP.egg-info/dependency_links.txt
--rw-r--r--   0 MichaelArbel   (501) staff       (20)        1 2023-06-05 18:39:36.000000 MLXP-0.0.1/MLXP.egg-info/not-zip-safe
--rw-r--r--   0 MichaelArbel   (501) staff       (20)      115 2023-06-05 18:39:36.000000 MLXP-0.0.1/MLXP.egg-info/requires.txt
--rw-r--r--   0 MichaelArbel   (501) staff       (20)        6 2023-06-05 18:39:36.000000 MLXP-0.0.1/MLXP.egg-info/top_level.txt
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     5185 2023-06-05 18:39:36.386218 MLXP-0.0.1/PKG-INFO
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     3724 2023-06-05 16:08:37.000000 MLXP-0.0.1/README.rst
-drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:39:36.383637 MLXP-0.0.1/mlxpy/
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     1080 2023-06-05 18:39:23.000000 MLXP-0.0.1/mlxpy/__init__.py
-drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:39:36.384336 MLXP-0.0.1/mlxpy/_internal/
--rw-r--r--   0 MichaelArbel   (501) staff       (20)        0 2023-04-27 14:40:31.000000 MLXP-0.0.1/mlxpy/_internal/__init__.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)      296 2023-04-23 16:55:24.000000 MLXP-0.0.1/mlxpy/_internal/_interactive_mode.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     7350 2023-06-05 13:08:20.000000 MLXP-0.0.1/mlxpy/_internal/configure.py
-drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:39:36.385485 MLXP-0.0.1/mlxpy/data_structures/
--rw-r--r--   0 MichaelArbel   (501) staff       (20)        0 2023-04-27 14:40:31.000000 MLXP-0.0.1/mlxpy/data_structures/__init__.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     1528 2023-04-23 16:55:24.000000 MLXP-0.0.1/mlxpy/data_structures/artifacts.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     2860 2023-04-23 16:55:24.000000 MLXP-0.0.1/mlxpy/data_structures/config_dict.py
-drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:39:36.385980 MLXP-0.0.1/mlxpy/data_structures/contrib/
--rw-r--r--   0 MichaelArbel   (501) staff       (20)        0 2023-04-29 05:08:45.000000 MLXP-0.0.1/mlxpy/data_structures/contrib/__init__.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     3065 2023-06-05 13:08:20.000000 MLXP-0.0.1/mlxpy/data_structures/contrib/aggregation_maps.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)      975 2023-04-23 16:55:24.000000 MLXP-0.0.1/mlxpy/data_structures/contrib/artifacts.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)    17788 2023-06-05 13:08:20.000000 MLXP-0.0.1/mlxpy/data_structures/data_dict.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     8648 2023-04-27 14:34:37.000000 MLXP-0.0.1/mlxpy/data_structures/schemas.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     1496 2023-04-23 19:18:06.000000 MLXP-0.0.1/mlxpy/enumerations.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)      641 2023-04-23 19:18:06.000000 MLXP-0.0.1/mlxpy/errors.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)    17263 2023-06-05 13:08:20.000000 MLXP-0.0.1/mlxpy/launcher.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)    12115 2023-06-05 13:08:20.000000 MLXP-0.0.1/mlxpy/logger.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     5818 2023-04-23 19:18:05.000000 MLXP-0.0.1/mlxpy/parser.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     9736 2023-06-05 13:08:20.000000 MLXP-0.0.1/mlxpy/reader.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     9687 2023-04-29 05:08:45.000000 MLXP-0.0.1/mlxpy/scheduler.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)    17159 2023-04-26 11:45:29.000000 MLXP-0.0.1/mlxpy/version_manager.py
--rw-r--r--   0 MichaelArbel   (501) staff       (20)       38 2023-06-05 18:39:36.386421 MLXP-0.0.1/setup.cfg
--rw-r--r--   0 MichaelArbel   (501) staff       (20)     1142 2023-06-05 15:04:50.000000 MLXP-0.0.1/setup.py
+drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:45:47.852235 MLXP-0.0.2/
+drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:45:47.847536 MLXP-0.0.2/MLXP.egg-info/
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     5166 2023-06-05 18:45:47.000000 MLXP-0.0.2/MLXP.egg-info/PKG-INFO
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)      734 2023-06-05 18:45:47.000000 MLXP-0.0.2/MLXP.egg-info/SOURCES.txt
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)        1 2023-06-05 18:45:47.000000 MLXP-0.0.2/MLXP.egg-info/dependency_links.txt
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)        1 2023-06-05 18:45:47.000000 MLXP-0.0.2/MLXP.egg-info/not-zip-safe
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)      115 2023-06-05 18:45:47.000000 MLXP-0.0.2/MLXP.egg-info/requires.txt
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)        5 2023-06-05 18:45:47.000000 MLXP-0.0.2/MLXP.egg-info/top_level.txt
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     5166 2023-06-05 18:45:47.852042 MLXP-0.0.2/PKG-INFO
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     3706 2023-06-05 18:44:24.000000 MLXP-0.0.2/README.rst
+drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:45:47.849520 MLXP-0.0.2/mlxp/
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     1072 2023-06-05 18:45:36.000000 MLXP-0.0.2/mlxp/__init__.py
+drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:45:47.850142 MLXP-0.0.2/mlxp/_internal/
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)        0 2023-04-27 14:40:31.000000 MLXP-0.0.2/mlxp/_internal/__init__.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)      296 2023-04-23 16:55:24.000000 MLXP-0.0.2/mlxp/_internal/_interactive_mode.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     7299 2023-06-05 18:44:02.000000 MLXP-0.0.2/mlxp/_internal/configure.py
+drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:45:47.851226 MLXP-0.0.2/mlxp/data_structures/
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)        0 2023-04-27 14:40:31.000000 MLXP-0.0.2/mlxp/data_structures/__init__.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     1528 2023-04-23 16:55:24.000000 MLXP-0.0.2/mlxp/data_structures/artifacts.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     2860 2023-04-23 16:55:24.000000 MLXP-0.0.2/mlxp/data_structures/config_dict.py
+drwxr-xr-x   0 MichaelArbel   (501) staff       (20)        0 2023-06-05 18:45:47.851773 MLXP-0.0.2/mlxp/data_structures/contrib/
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)        0 2023-04-29 05:08:45.000000 MLXP-0.0.2/mlxp/data_structures/contrib/__init__.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     3064 2023-06-05 18:44:00.000000 MLXP-0.0.2/mlxp/data_structures/contrib/aggregation_maps.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)      974 2023-06-05 18:43:59.000000 MLXP-0.0.2/mlxp/data_structures/contrib/artifacts.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)    17787 2023-06-05 18:44:02.000000 MLXP-0.0.2/mlxp/data_structures/data_dict.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     8637 2023-06-05 18:44:01.000000 MLXP-0.0.2/mlxp/data_structures/schemas.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     1494 2023-06-05 18:44:07.000000 MLXP-0.0.2/mlxp/enumerations.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)      640 2023-06-05 18:40:37.000000 MLXP-0.0.2/mlxp/errors.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)    17222 2023-06-05 18:44:07.000000 MLXP-0.0.2/mlxp/launcher.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)    12107 2023-06-05 18:44:06.000000 MLXP-0.0.2/mlxp/logger.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     5815 2023-06-05 18:44:05.000000 MLXP-0.0.2/mlxp/parser.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     9728 2023-06-05 18:44:04.000000 MLXP-0.0.2/mlxp/reader.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     9686 2023-06-05 18:44:04.000000 MLXP-0.0.2/mlxp/scheduler.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)    17156 2023-06-05 18:44:03.000000 MLXP-0.0.2/mlxp/version_manager.py
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)       38 2023-06-05 18:45:47.852281 MLXP-0.0.2/setup.cfg
+-rw-r--r--   0 MichaelArbel   (501) staff       (20)     1140 2023-06-05 18:44:23.000000 MLXP-0.0.2/setup.py
```

### Comparing `MLXP-0.0.1/MLXP.egg-info/PKG-INFO` & `MLXP-0.0.2/MLXP.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: MLXP
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework for conducting machine learning experiments in python
-Home-page: https://github.com/MichaelArbel/mlxpy
+Home-page: https://github.com/MichaelArbel/mlxp
 Author: Michael Arbel
 Author-email: michael.n.arbel@gmail.com
 License: MIT License
 Description: Introduction
         ^^^^^^^^^^^^
         
-        MLXPy (Machine Learning eXperiments Python) package is an open-source Python framework for managing multiple experiments with a flexible option structure from launching, and logging to querying results. A full documentation is available in the `MLXPy's official  documentation website <https://michaelarbel.github.io/mlxpy/>`_. 
+        MLXP (Machine Learning eXperiments Python) package is an open-source Python framework for managing multiple experiments with a flexible option structure from launching, and logging to querying results. A full documentation is available in the `MLXP's official  documentation website <https://michaelarbel.github.io/mlxp/>`_. 
         
         
         
         Key functionalities
         ^^^^^^^^^^^^^^^^^^^
         
         1. Launching several jobs automatically using `hydra <https://hydra.cc/>`_ and hierarchical configs by adding a single decorator to the main task function.   
@@ -22,68 +22,68 @@
         4. Submitting jobs to a cluster using a job scheduler. 
         5. Exploiting the results of several experiments by easily reading, querying, grouping, and aggregating the output of several jobs. 
         
         
         License
         ^^^^^^^
         
-        MLXPy is distributed under MIT license.
+        MLXP is distributed under MIT license.
         
-        Citing MLXPy
+        Citing MLXP
         ^^^^^^^^^^^^
         
-        Even though this is non-legally binding, the author kindly ask users to cite MLXPy in their publications if they use 
+        Even though this is non-legally binding, the author kindly ask users to cite MLXP in their publications if they use 
         it in their research as follows:
         
         
         .. code-block:: bibtex 
         
-           @Misc{Arbel2023MLXPy,
+           @Misc{Arbel2023MLXP,
              author = {Michae Arbel},
-             title = {MLXPy: },
+             title = {MLXP: },
              howpublished = {Github},
              year = {2023},
-             url = {https://github.com/MichaelArbel/mlxpy}
+             url = {https://github.com/MichaelArbel/mlxp}
            }
         
         
-        Installing MLXPy
+        Installing MLXP
         ^^^^^^^^^^^^^^^^
         
-        You can install MLXPy either from PyPI or by cloning the GitHub.
+        You can install MLXP either from PyPI or by cloning the GitHub.
         
         
         From PyPI
         ---------
         
         You can simply run the following command:
         
         .. code-block:: console
            
-           $ pip install MLXPy
+           $ pip install MLXP
         
         
         From GitHub
         -----------
         
         You can install this package by cloning it from the GitHub repository
         and then installing it with `pip`. 
         
         
         1. Clone the repository:
         
         .. code-block:: console
            
-           $ git clone git@github.com:MichaelArbel/mlxpy.git
+           $ git clone git@github.com:MichaelArbel/mlxp.git
         
         2. Change to the package directory:
         
         .. code-block:: console
            
-           $ cd mlxpy
+           $ cd mlxp
         
         3. Install the requirements using `pip`:
         
         .. code-block:: console
            
            $ pip install -r requirements.txt
         
@@ -94,15 +94,15 @@
            $ pip install .
         
         Note: You may need to use `pip3` instead of `pip` depending on your setup.
         
         
         
         
-        Before installing MLXPy, make sure you the requirements are installed.
+        Before installing MLXP, make sure you the requirements are installed.
         
         
         Requirements
         ------------
         
         
         .. list-table::
@@ -125,17 +125,17 @@
         ^^^^^^^^^^^^^^^
         
         I would like to acknowledge the following contributors for their contributions to the development of this package:
         
         - `Alexandre Zouaoui <https://azouaoui.me/>`_ kindly shared his python implementation for creating job scripts and submiting them to a cluster. His code served as the basis for the implementation of the Scheduler class. While I have significantly modified the process of job submission, by integrating it with MLXpy's launching functionality, I am grateful for Alexandre's contribution which were invaluable to the development of this project.
         
         
-        - `Juliette Marrie <https://www.linkedin.com/in/juliette-marrie-5b8a59179/?originalSubdomain=fr>`_ tested a premature version of MLXPy. I am grateful for her feedback which was extremetly helpful for shaping and improving MLXPy's functionalities.  
+        - `Juliette Marrie <https://www.linkedin.com/in/juliette-marrie-5b8a59179/?originalSubdomain=fr>`_ tested a premature version of MLXP. I am grateful for her feedback which was extremetly helpful for shaping and improving MLXP's functionalities.  
         
-        - `Romain Ménégaux <https://www.linkedin.com/in/romain-menegaux-88a147134/?originalSubdomain=fr>`_ provided valuable feedback and suggestions to improve MLXPy. He also found and reported several bugs in the software which helped improve its quality and stability. 
+        - `Romain Ménégaux <https://www.linkedin.com/in/romain-menegaux-88a147134/?originalSubdomain=fr>`_ provided valuable feedback and suggestions to improve MLXP. He also found and reported several bugs in the software which helped improve its quality and stability.
```

### Comparing `MLXP-0.0.1/MLXP.egg-info/SOURCES.txt` & `MLXP-0.0.2/MLXP.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 setup.py
 MLXP.egg-info/PKG-INFO
 MLXP.egg-info/SOURCES.txt
 MLXP.egg-info/dependency_links.txt
 MLXP.egg-info/not-zip-safe
 MLXP.egg-info/requires.txt
 MLXP.egg-info/top_level.txt
-mlxpy/__init__.py
-mlxpy/enumerations.py
-mlxpy/errors.py
-mlxpy/launcher.py
-mlxpy/logger.py
-mlxpy/parser.py
-mlxpy/reader.py
-mlxpy/scheduler.py
-mlxpy/version_manager.py
-mlxpy/_internal/__init__.py
-mlxpy/_internal/_interactive_mode.py
-mlxpy/_internal/configure.py
-mlxpy/data_structures/__init__.py
-mlxpy/data_structures/artifacts.py
-mlxpy/data_structures/config_dict.py
-mlxpy/data_structures/data_dict.py
-mlxpy/data_structures/schemas.py
-mlxpy/data_structures/contrib/__init__.py
-mlxpy/data_structures/contrib/aggregation_maps.py
-mlxpy/data_structures/contrib/artifacts.py
+mlxp/__init__.py
+mlxp/enumerations.py
+mlxp/errors.py
+mlxp/launcher.py
+mlxp/logger.py
+mlxp/parser.py
+mlxp/reader.py
+mlxp/scheduler.py
+mlxp/version_manager.py
+mlxp/_internal/__init__.py
+mlxp/_internal/_interactive_mode.py
+mlxp/_internal/configure.py
+mlxp/data_structures/__init__.py
+mlxp/data_structures/artifacts.py
+mlxp/data_structures/config_dict.py
+mlxp/data_structures/data_dict.py
+mlxp/data_structures/schemas.py
+mlxp/data_structures/contrib/__init__.py
+mlxp/data_structures/contrib/aggregation_maps.py
+mlxp/data_structures/contrib/artifacts.py
```

### Comparing `MLXP-0.0.1/PKG-INFO` & `MLXP-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: MLXP
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework for conducting machine learning experiments in python
-Home-page: https://github.com/MichaelArbel/mlxpy
+Home-page: https://github.com/MichaelArbel/mlxp
 Author: Michael Arbel
 Author-email: michael.n.arbel@gmail.com
 License: MIT License
 Description: Introduction
         ^^^^^^^^^^^^
         
-        MLXPy (Machine Learning eXperiments Python) package is an open-source Python framework for managing multiple experiments with a flexible option structure from launching, and logging to querying results. A full documentation is available in the `MLXPy's official  documentation website <https://michaelarbel.github.io/mlxpy/>`_. 
+        MLXP (Machine Learning eXperiments Python) package is an open-source Python framework for managing multiple experiments with a flexible option structure from launching, and logging to querying results. A full documentation is available in the `MLXP's official  documentation website <https://michaelarbel.github.io/mlxp/>`_. 
         
         
         
         Key functionalities
         ^^^^^^^^^^^^^^^^^^^
         
         1. Launching several jobs automatically using `hydra <https://hydra.cc/>`_ and hierarchical configs by adding a single decorator to the main task function.   
@@ -22,68 +22,68 @@
         4. Submitting jobs to a cluster using a job scheduler. 
         5. Exploiting the results of several experiments by easily reading, querying, grouping, and aggregating the output of several jobs. 
         
         
         License
         ^^^^^^^
         
-        MLXPy is distributed under MIT license.
+        MLXP is distributed under MIT license.
         
-        Citing MLXPy
+        Citing MLXP
         ^^^^^^^^^^^^
         
-        Even though this is non-legally binding, the author kindly ask users to cite MLXPy in their publications if they use 
+        Even though this is non-legally binding, the author kindly ask users to cite MLXP in their publications if they use 
         it in their research as follows:
         
         
         .. code-block:: bibtex 
         
-           @Misc{Arbel2023MLXPy,
+           @Misc{Arbel2023MLXP,
              author = {Michae Arbel},
-             title = {MLXPy: },
+             title = {MLXP: },
              howpublished = {Github},
              year = {2023},
-             url = {https://github.com/MichaelArbel/mlxpy}
+             url = {https://github.com/MichaelArbel/mlxp}
            }
         
         
-        Installing MLXPy
+        Installing MLXP
         ^^^^^^^^^^^^^^^^
         
-        You can install MLXPy either from PyPI or by cloning the GitHub.
+        You can install MLXP either from PyPI or by cloning the GitHub.
         
         
         From PyPI
         ---------
         
         You can simply run the following command:
         
         .. code-block:: console
            
-           $ pip install MLXPy
+           $ pip install MLXP
         
         
         From GitHub
         -----------
         
         You can install this package by cloning it from the GitHub repository
         and then installing it with `pip`. 
         
         
         1. Clone the repository:
         
         .. code-block:: console
            
-           $ git clone git@github.com:MichaelArbel/mlxpy.git
+           $ git clone git@github.com:MichaelArbel/mlxp.git
         
         2. Change to the package directory:
         
         .. code-block:: console
            
-           $ cd mlxpy
+           $ cd mlxp
         
         3. Install the requirements using `pip`:
         
         .. code-block:: console
            
            $ pip install -r requirements.txt
         
@@ -94,15 +94,15 @@
            $ pip install .
         
         Note: You may need to use `pip3` instead of `pip` depending on your setup.
         
         
         
         
-        Before installing MLXPy, make sure you the requirements are installed.
+        Before installing MLXP, make sure you the requirements are installed.
         
         
         Requirements
         ------------
         
         
         .. list-table::
@@ -125,17 +125,17 @@
         ^^^^^^^^^^^^^^^
         
         I would like to acknowledge the following contributors for their contributions to the development of this package:
         
         - `Alexandre Zouaoui <https://azouaoui.me/>`_ kindly shared his python implementation for creating job scripts and submiting them to a cluster. His code served as the basis for the implementation of the Scheduler class. While I have significantly modified the process of job submission, by integrating it with MLXpy's launching functionality, I am grateful for Alexandre's contribution which were invaluable to the development of this project.
         
         
-        - `Juliette Marrie <https://www.linkedin.com/in/juliette-marrie-5b8a59179/?originalSubdomain=fr>`_ tested a premature version of MLXPy. I am grateful for her feedback which was extremetly helpful for shaping and improving MLXPy's functionalities.  
+        - `Juliette Marrie <https://www.linkedin.com/in/juliette-marrie-5b8a59179/?originalSubdomain=fr>`_ tested a premature version of MLXP. I am grateful for her feedback which was extremetly helpful for shaping and improving MLXP's functionalities.  
         
-        - `Romain Ménégaux <https://www.linkedin.com/in/romain-menegaux-88a147134/?originalSubdomain=fr>`_ provided valuable feedback and suggestions to improve MLXPy. He also found and reported several bugs in the software which helped improve its quality and stability. 
+        - `Romain Ménégaux <https://www.linkedin.com/in/romain-menegaux-88a147134/?originalSubdomain=fr>`_ provided valuable feedback and suggestions to improve MLXP. He also found and reported several bugs in the software which helped improve its quality and stability.
```

### Comparing `MLXP-0.0.1/README.rst` & `MLXP-0.0.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Introduction
 ^^^^^^^^^^^^
 
-MLXPy (Machine Learning eXperiments Python) package is an open-source Python framework for managing multiple experiments with a flexible option structure from launching, and logging to querying results. A full documentation is available in the `MLXPy's official  documentation website <https://michaelarbel.github.io/mlxpy/>`_. 
+MLXP (Machine Learning eXperiments Python) package is an open-source Python framework for managing multiple experiments with a flexible option structure from launching, and logging to querying results. A full documentation is available in the `MLXP's official  documentation website <https://michaelarbel.github.io/mlxp/>`_. 
 
 
 
 Key functionalities
 ^^^^^^^^^^^^^^^^^^^
 
 1. Launching several jobs automatically using `hydra <https://hydra.cc/>`_ and hierarchical configs by adding a single decorator to the main task function.   
@@ -14,68 +14,68 @@
 4. Submitting jobs to a cluster using a job scheduler. 
 5. Exploiting the results of several experiments by easily reading, querying, grouping, and aggregating the output of several jobs. 
 
 
 License
 ^^^^^^^
 
-MLXPy is distributed under MIT license.
+MLXP is distributed under MIT license.
 
-Citing MLXPy
+Citing MLXP
 ^^^^^^^^^^^^
 
-Even though this is non-legally binding, the author kindly ask users to cite MLXPy in their publications if they use 
+Even though this is non-legally binding, the author kindly ask users to cite MLXP in their publications if they use 
 it in their research as follows:
 
 
 .. code-block:: bibtex 
 
-   @Misc{Arbel2023MLXPy,
+   @Misc{Arbel2023MLXP,
      author = {Michae Arbel},
-     title = {MLXPy: },
+     title = {MLXP: },
      howpublished = {Github},
      year = {2023},
-     url = {https://github.com/MichaelArbel/mlxpy}
+     url = {https://github.com/MichaelArbel/mlxp}
    }
 
 
-Installing MLXPy
+Installing MLXP
 ^^^^^^^^^^^^^^^^
 
-You can install MLXPy either from PyPI or by cloning the GitHub.
+You can install MLXP either from PyPI or by cloning the GitHub.
 
 
 From PyPI
 ---------
 
 You can simply run the following command:
 
 .. code-block:: console
    
-   $ pip install MLXPy
+   $ pip install MLXP
 
 
 From GitHub
 -----------
 
 You can install this package by cloning it from the GitHub repository
 and then installing it with `pip`. 
 
 
 1. Clone the repository:
 
 .. code-block:: console
    
-   $ git clone git@github.com:MichaelArbel/mlxpy.git
+   $ git clone git@github.com:MichaelArbel/mlxp.git
 
 2. Change to the package directory:
 
 .. code-block:: console
    
-   $ cd mlxpy
+   $ cd mlxp
 
 3. Install the requirements using `pip`:
 
 .. code-block:: console
    
    $ pip install -r requirements.txt
 
@@ -86,15 +86,15 @@
    $ pip install .
 
 Note: You may need to use `pip3` instead of `pip` depending on your setup.
 
 
 
 
-Before installing MLXPy, make sure you the requirements are installed.
+Before installing MLXP, make sure you the requirements are installed.
 
 
 Requirements
 ------------
 
 
 .. list-table::
@@ -117,17 +117,17 @@
 ^^^^^^^^^^^^^^^
 
 I would like to acknowledge the following contributors for their contributions to the development of this package:
 
 - `Alexandre Zouaoui <https://azouaoui.me/>`_ kindly shared his python implementation for creating job scripts and submiting them to a cluster. His code served as the basis for the implementation of the Scheduler class. While I have significantly modified the process of job submission, by integrating it with MLXpy's launching functionality, I am grateful for Alexandre's contribution which were invaluable to the development of this project.
 
 
-- `Juliette Marrie <https://www.linkedin.com/in/juliette-marrie-5b8a59179/?originalSubdomain=fr>`_ tested a premature version of MLXPy. I am grateful for her feedback which was extremetly helpful for shaping and improving MLXPy's functionalities.  
+- `Juliette Marrie <https://www.linkedin.com/in/juliette-marrie-5b8a59179/?originalSubdomain=fr>`_ tested a premature version of MLXP. I am grateful for her feedback which was extremetly helpful for shaping and improving MLXP's functionalities.  
 
-- `Romain Ménégaux <https://www.linkedin.com/in/romain-menegaux-88a147134/?originalSubdomain=fr>`_ provided valuable feedback and suggestions to improve MLXPy. He also found and reported several bugs in the software which helped improve its quality and stability. 
+- `Romain Ménégaux <https://www.linkedin.com/in/romain-menegaux-88a147134/?originalSubdomain=fr>`_ provided valuable feedback and suggestions to improve MLXP. He also found and reported several bugs in the software which helped improve its quality and stability.
```

### Comparing `MLXP-0.0.1/mlxpy/__init__.py` & `MLXP-0.0.2/mlxp/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from mlxpy.launcher import launch, Context
-from mlxpy.reader import Reader
-from mlxpy.logger import DefaultLogger
-from mlxpy.version_manager import GitVM
+from mlxp.launcher import launch, Context
+from mlxp.reader import Reader
+from mlxp.logger import DefaultLogger
+from mlxp.version_manager import GitVM
 
-from mlxpy.scheduler import Scheduler, SLURMScheduler, OARScheduler
+from mlxp.scheduler import Scheduler, SLURMScheduler, OARScheduler
 
-from mlxpy.data_structures.config_dict import ConfigDict
-from mlxpy.data_structures.data_dict import DataDictList
+from mlxp.data_structures.config_dict import ConfigDict
+from mlxp.data_structures.data_dict import DataDictList
 
 
 __all__ = [
     "launch", 
     "Reader",
     "DefaultLogger",
     "Scheduler",
@@ -20,19 +20,19 @@
     "OARScheduler",
     "SLURMScheduler",
     "GitVM"
 ]
 
 
 
-VERSION = (0, 0, 1)
+VERSION = (0, 0, 2)
 PROJECT = 'MLXP'
 AUTHOR = "Michael Arbel"
 AUTHOR_EMAIL = "michael.n.arbel@gmail.com"
-URL = "https://github.com/MichaelArbel/mlxpy"
+URL = "https://github.com/MichaelArbel/mlxp"
 LICENSE = "MIT License"
 VERSION_TEXT = ".".join(str(x) for x in VERSION)
 COPYRIGHT = "Copyright (C) 2023 " + AUTHOR
 
 
 VERSION_STATUS = ""
 RELEASE = VERSION_TEXT + VERSION_STATUS
```

### Comparing `MLXP-0.0.1/mlxpy/_internal/configure.py` & `MLXP-0.0.2/mlxp/_internal/configure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import omegaconf
 from omegaconf import OmegaConf
-from mlxpy.scheduler import Scheduler
-from mlxpy.enumerations import DefaultSchedulers
+from mlxp.scheduler import Scheduler
+from mlxp.enumerations import DefaultSchedulers
 
-from mlxpy.data_structures.schemas import Metadata
-from mlxpy.data_structures.config_dict import convert_dict, ConfigDict
-from mlxpy._internal._interactive_mode import _bcolors, _printc
+from mlxp.data_structures.schemas import Metadata
+from mlxp.data_structures.config_dict import convert_dict, ConfigDict
+from mlxp._internal._interactive_mode import _bcolors, _printc
 import yaml
 import os
 
 
-def _configure_scheduler(mlxpy_config):
+def _configure_scheduler(mlxp_config):
     while True:
         print("You can either choose one of the job schedulers available by default, ")
 
         print(
             f"or define a custom one by inheriting from the abstract class {Scheduler} (see documentation)  "
         )
 
@@ -34,170 +34,170 @@
         if files_input:
             names = files_input.strip().rsplit(".", 1)
             is_valid = True
             for name in names:
                 if not name.isidentifier():
                     is_valid = False
             if is_valid:
-                omegaconf.OmegaConf.set_struct(mlxpy_config, True)
-                with omegaconf.open_dict(mlxpy_config):
-                    mlxpy_config.mlxpy.scheduler.name = files_input
-                omegaconf.OmegaConf.set_struct(mlxpy_config, False)
+                omegaconf.OmegaConf.set_struct(mlxp_config, True)
+                with omegaconf.open_dict(mlxp_config):
+                    mlxp_config.mlxp.scheduler.name = files_input
+                omegaconf.OmegaConf.set_struct(mlxp_config, False)
                 _printc(_bcolors.OKBLUE, f" Setting Scheduler to {files_input} ")
                 break
             else:
                 _printc(
                     _bcolors.OKBLUE,
                     f" {files_input} is not a valid class identifier. Please try again  ",
                 )
         else:
             break
 
 
-def _ask_configure_scheduler(mlxpy_config, mlxpy_file):
+def _ask_configure_scheduler(mlxp_config, mlxp_file):
     while True:
 
         _printc(
             _bcolors.OKGREEN,
             " Would you like to select a default job scheduler now ?  (y/n):",
         )
         print(
-            f"{_bcolors.OKGREEN}y{_bcolors.ENDC}: The job scheduler configs will be stored in the file {mlxpy_file}"
+            f"{_bcolors.OKGREEN}y{_bcolors.ENDC}: The job scheduler configs will be stored in the file {mlxp_file}"
         )
         print(
             f"{_bcolors.OKGREEN}n{_bcolors.ENDC}: No scheduler will be selected by default."
         )
 
         choice = input(
             f"{_bcolors.OKGREEN}Please enter you answer (y/n):{_bcolors.ENDC}")
 
         if choice == "y":
-            _configure_scheduler(mlxpy_config)
+            _configure_scheduler(mlxp_config)
             break
         elif choice == "n":
 
             _printc(_bcolors.OKBLUE, "No scheduler will be selected by default.")
             _printc(
                 _bcolors.OKBLUE,
                 "To use a scheduler, you will need to select one later.",
             )
             break
         else:
             _printc(_bcolors.OKBLUE, "Invalid choice. Please try again. (y/n)")
 
 
 def _build_config(overrides, config_path):
-    overrides_mlxpy, overrides_config = _process_overrides(overrides)
+    overrides_mlxp, overrides_config = _process_overrides(overrides)
 
 
-    cfg = _get_default_config(config_path, overrides_mlxpy)
+    cfg = _get_default_config(config_path, overrides_mlxp)
 
     cfg = OmegaConf.merge(cfg, overrides_config)
 
     cfg = convert_dict(
         cfg, src_class=omegaconf.dictconfig.DictConfig, dst_class=ConfigDict
     )
 
     return cfg
 
 
 def _add_config_overrides(cfg, overrides):
-    overrides_mlxpy, overrides_config = _process_overrides(overrides)
+    overrides_mlxp, overrides_config = _process_overrides(overrides)
     cfg = convert_dict(
         cfg, src_class=ConfigDict, dst_class=omegaconf.dictconfig.DictConfig
     )   
     cfg = OmegaConf.merge(cfg, overrides_config)
 
     cfg = convert_dict(
         cfg, src_class=omegaconf.dictconfig.DictConfig, dst_class=ConfigDict
     )
     return cfg
 
 
 def _process_overrides(overrides):
-    if "mlxpy" in overrides:
-        overrides_mlxpy = OmegaConf.create({"mlxpy": overrides["mlxpy"]})
-#        cfg = OmegaConf.merge(cfg, overrides_mlxpy)
+    if "mlxp" in overrides:
+        overrides_mlxp = OmegaConf.create({"mlxp": overrides["mlxp"]})
+#        cfg = OmegaConf.merge(cfg, overrides_mlxp)
     else:
-        overrides_mlxpy = None
+        overrides_mlxp = None
 
     overrides = convert_dict(
         overrides, src_class=omegaconf.dictconfig.DictConfig, dst_class=dict
     )
-    if "mlxpy" in overrides:
-        overrides.pop("mlxpy")
+    if "mlxp" in overrides:
+        overrides.pop("mlxp")
     overrides = convert_dict(
         overrides, src_class=dict, dst_class=omegaconf.dictconfig.DictConfig
     )
 
     overrides_config = OmegaConf.create({"config": overrides})
 
-    return overrides_mlxpy, overrides_config
+    return overrides_mlxp, overrides_config
 
 
 def _get_default_config(config_path, overrides):
     default_config = OmegaConf.structured(Metadata)
     conf_dict = OmegaConf.to_container(default_config, resolve=True)
     default_config = OmegaConf.create(conf_dict)
 
     os.makedirs(config_path, exist_ok=True)
-    mlxpy_file = os.path.join(config_path, "mlxpy.yaml")
+    mlxp_file = os.path.join(config_path, "mlxp.yaml")
 
-    if os.path.exists(mlxpy_file):
-        with open(mlxpy_file, "r") as file:
-            mlxpy = OmegaConf.create({"mlxpy": yaml.safe_load(file)})
-        valid_keys = list(default_config["mlxpy"].keys())
-        for key in mlxpy["mlxpy"].keys():
+    if os.path.exists(mlxp_file):
+        with open(mlxp_file, "r") as file:
+            mlxp = OmegaConf.create({"mlxp": yaml.safe_load(file)})
+        valid_keys = list(default_config["mlxp"].keys())
+        for key in mlxp["mlxp"].keys():
             try:
                 assert key in valid_keys
             except AssertionError:
-                msg = f"In the file {mlxpy_file},"
+                msg = f"In the file {mlxp_file},"
                 msg += f"the following field is invalid: {key}\n"
                 msg += f"Valid fields are {valid_keys}\n"
                 raise AssertionError(msg)
 
-        default_config = OmegaConf.merge(default_config, mlxpy)
+        default_config = OmegaConf.merge(default_config, mlxp)
 
-    using_scheduler = default_config.mlxpy.use_scheduler
-    scheduler_name_default = default_config.mlxpy.scheduler.name
+    using_scheduler = default_config.mlxp.use_scheduler
+    scheduler_name_default = default_config.mlxp.scheduler.name
     scheduler_name = scheduler_name_default
-    interactive_mode = default_config.mlxpy.interactive_mode
+    interactive_mode = default_config.mlxp.interactive_mode
     if overrides:
         if "use_scheduler" in overrides:
             using_scheduler = overrides["use_scheduler"]
         if "scheduler" in overrides:
             if "name" in overrides["scheduler"]:
                 scheduler_name = overrides["scheduler"]
         if "interactive_mode" in overrides:
             interactive_mode = overrides["interactive_mode"]
 
     update_default_conifg = False
     if scheduler_name == "NoScheduler":
-        if using_scheduler or not os.path.exists(mlxpy_file):
+        if using_scheduler or not os.path.exists(mlxp_file):
             _printc(_bcolors.OKBLUE, "No scheduler is configured by default ")
             if interactive_mode:
                 _printc(_bcolors.OKBLUE, "Entering interactive mode ")
-                _ask_configure_scheduler(default_config, mlxpy_file)
+                _ask_configure_scheduler(default_config, mlxp_file)
                 _printc(_bcolors.OKBLUE, "Leaving interactive mode ")
                 update_default_conifg = True
             else:
                 pass
 
     else:
         omegaconf.OmegaConf.set_struct(default_config, True)
         with omegaconf.open_dict(default_config):
-            default_config.mlxpy.scheduler.name = scheduler_name
+            default_config.mlxp.scheduler.name = scheduler_name
         omegaconf.OmegaConf.set_struct(default_config, False)
         if scheduler_name_default == "NoScheduler":
             update_default_conifg = True
             _printc(_bcolors.OKBLUE, f"Setting Scheduler to: {scheduler_name} ")
 
-    if not os.path.exists(mlxpy_file) or update_default_conifg:
+    if not os.path.exists(mlxp_file) or update_default_conifg:
         _printc(
             _bcolors.OKBLUE,
-            f"Default settings for mlxpy will be created in {mlxpy_file} ",
+            f"Default settings for mlxp will be created in {mlxp_file} ",
         )
-        mlxpy = OmegaConf.create(default_config["mlxpy"])
-        omegaconf.OmegaConf.save(config=mlxpy, f=mlxpy_file)
+        mlxp = OmegaConf.create(default_config["mlxp"])
+        omegaconf.OmegaConf.save(config=mlxp, f=mlxp_file)
     if overrides:
         default_config = OmegaConf.merge(default_config, overrides)
     return default_config
```

### Comparing `MLXP-0.0.1/mlxpy/data_structures/artifacts.py` & `MLXP-0.0.2/mlxp/data_structures/artifacts.py`

 * *Files identical despite different names*

### Comparing `MLXP-0.0.1/mlxpy/data_structures/config_dict.py` & `MLXP-0.0.2/mlxp/data_structures/config_dict.py`

 * *Files identical despite different names*

### Comparing `MLXP-0.0.1/mlxpy/data_structures/contrib/aggregation_maps.py` & `MLXP-0.0.2/mlxp/data_structures/contrib/aggregation_maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A few aggregation maps."""
 
 import numpy as np
 
 
-from mlxpy.data_structures.data_dict import AggregationMap
+from mlxp.data_structures.data_dict import AggregationMap
 
 
 class Last(AggregationMap):
     """Return the last element of a list."""
 
     def __init__(self, key):
         super().__init__([key], map_name="last")
```

### Comparing `MLXP-0.0.1/mlxpy/data_structures/data_dict.py` & `MLXP-0.0.2/mlxp/data_structures/data_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MutableMapping,
     KeysView,
     ItemsView,
 )
 
 from typing import List, Dict, Tuple, Any
 
-from mlxpy.errors import InvalidKeyError, InvalidAggregationMapError
+from mlxp.errors import InvalidKeyError, InvalidAggregationMapError
 
 LAZYDATA = "LAZYDATA"
 
 
 class AggregationMap:
     """An abstract class whose children can perform aggregations on arrays."""
```

### Comparing `MLXP-0.0.1/mlxpy/data_structures/schemas.py` & `MLXP-0.0.2/mlxp/data_structures/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,16 +228,16 @@
     work_dir: str = os.getcwd()
     logger: Any = None
     scheduler: Any = None
     version_manager: Any = None
 
 
 @dataclass
-class MLXPyConfig:
-    """Default settings of MLXPy.
+class MLXPConfig:
+    """Default settings of MLXP.
 
     .. py:attribute:: logger
         :type: ConfigLogger
 
         The logger's settings.
         (default ConfigLogger)
 
@@ -270,17 +270,17 @@
 
         If true, uses the logger.
         (default True)
 
     .. py:attribute:: interactive_mode
         :type: bool
 
-        A variable controlling MLXPy's interactive mode.
+        A variable controlling MLXP's interactive mode.
 
-            1. If 'interactive_mode==True', MLXPy uses the interactive mode whenever applicable:
+            1. If 'interactive_mode==True', MLXP uses the interactive mode whenever applicable:
 
                 - When 'use_scheduler==True' and 'scheduler.name=="NoScheduler"':
                 Asks the user to select a valid scheduler.
                 - When 'use_version_manager==True': Asks the user:
 
                     - If untracked files should be added.
                     - If uncommitted changes should be committed.
@@ -311,23 +311,23 @@
     .. py:attribute:: info
         :type: Info
 
         Contains config information of the run
         (hostname, command, application,  etc)
         (default Info)
 
-    .. py:attribute:: mlxpy
-        :type: MLXPyConfig
+    .. py:attribute:: mlxp
+        :type: MLXPConfig
 
-        Default settings of MLXPy.
-        (default MLXPyConfig)
+        Default settings of MLXP.
+        (default MLXPConfig)
 
 
     .. py:attribute:: config
         :type: Any
 
         Contains the user's defined configs that are specific to the run.
     """
 
     info: Info = Info()
-    mlxpy: MLXPyConfig = MLXPyConfig()
+    mlxp: MLXPConfig = MLXPConfig()
     config: Any = None
```

### Comparing `MLXP-0.0.1/mlxpy/enumerations.py` & `MLXP-0.0.2/mlxp/enumerations.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,25 @@
     """Types of data that can be returned by the method filter of a Reader object."""
 
     Pandas = "pandas"
     DataDictList = "datadict"
 
 
 class DefaultSchedulers(Enum):
-    """Schedulers supported by default by MLXPy."""
+    """Schedulers supported by default by MLXP."""
 
     OARScheduler = "OARScheduler"
     SLURMScheduler = "SLURMScheduler"
 
 
 class Directories(Enum):
     """The sub-directories created by the logger for each run.
 
     - Metrics: (Value: "metrics") A directory containing the JSON files created when calling the method log_metrics of a Logger object.
-    - Metadata: (Value: "metadata") A directory containing three files 'info.yaml', 'mlxpy.yaml' and 'config.yaml'.
+    - Metadata: (Value: "metadata") A directory containing three files 'info.yaml', 'mlxp.yaml' and 'config.yaml'.
     - Artifacts: (Value: "artifacts") A directory containing sub-directories created when calling the method log_artifacts of a Logger object.
     """
 
     Metrics = "metrics"
     Metadata = "metadata"
     Artifacts = "artifacts"
```

### Comparing `MLXP-0.0.1/mlxpy/errors.py` & `MLXP-0.0.2/mlxp/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Errors raised by MLXPy."""
+"""Errors raised by MLXP."""
 
 
 class JobSubmissionError(Exception):
     """Raised when failed to submit a job using a scheduler."""
 
     pass
```

### Comparing `MLXP-0.0.1/mlxpy/launcher.py` & `MLXP-0.0.2/mlxp/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from omegaconf import DictConfig
 
 from hydra import version
 from hydra._internal.utils import _run_hydra, get_args_parser
 from hydra.core.hydra_config import HydraConfig
 from hydra.types import TaskFunction
 
-from mlxpy.data_structures.config_dict import ConfigDict
-from mlxpy.logger import Logger
-from mlxpy.errors import MissingFieldError
-import mlxpy
+from mlxp.data_structures.config_dict import ConfigDict
+from mlxp.logger import Logger
+from mlxp.errors import MissingFieldError
+import mlxp
 
 from datetime import datetime
 import socket
 import sys
 from dataclasses import dataclass
-from mlxpy._internal.configure import _build_config, _add_config_overrides
+from mlxp._internal.configure import _build_config, _add_config_overrides
 import yaml
 import importlib
-from mlxpy.enumerations import Status
+from mlxp.enumerations import Status
 
 
 _UNSPECIFIED_: Any = object()
 
 
 hydra_defaults_dict = {"hydra.mode": "MULTIRUN",
                        "hydra.output_subdir": "null",
@@ -59,50 +59,50 @@
 ) -> Callable[[TaskFunction], Any]:
     """Create a decorator of the main function to be executed.
 
     :example:
 
     .. code-block:: python
 
-        import mlxpy
+        import mlxp
 
-        @mlxpy.launch(config_path='./configs',
+        @mlxp.launch(config_path='./configs',
                      seeding_function=set_seeds)
-        def my_func(ctx: mlxpy.Context)->None:
+        def my_func(ctx: mlxp.Context)->None:
 
             print(ctx.config)
 
         if __name__ == "__main__":
             my_func()
 
-    :param config_path: The config path, a directory where the default user configuration and MLXPy settings are stored.
+    :param config_path: The config path, a directory where the default user configuration and MLXP settings are stored.
     :param seeding_function:  A callable for setting the seed of random number generators. It is called with the seed option in 'ctx.config.seed' passed to it.
     :type config_path: str (default './configs')
     :type seeding_function: Union[Callable[[Any], None],None] (default None)
     :return: A decorator of the main function to be executed.
     :type: Callable[[TaskFunction], Any]
 
     This function allows four main functionalities:
 
         1. Composing configurations from multiple files using hydra (see hydra-core package).
         This behavior is similar to the decorator hydra.main provided in the hydra-core package:
         https://github.com/facebookresearch/hydra/blob/main/hydra/main.py.
         The configs are contained in a yaml file 'config.yaml' stored in
         the directory 'config_path' passed as argument to this function.
         Unlike hydra.main which decorates functions taking an OmegaConf object,
-        mlxpy.launch  decorates functions with the following signature: main(ctx: mlxpy.Context).
+        mlxp.launch  decorates functions with the following signature: main(ctx: mlxp.Context).
         The ctx object is created on the fly during the execution of the program
         and stores information about the run.
         In particular, the field cfg.config stores the options contained in the config file 'config.yaml'.
-        Additionally, cfg.logger, provides a logger object of the class mlxpy.Logger for logging results of the run.
+        Additionally, cfg.logger, provides a logger object of the class mlxp.Logger for logging results of the run.
         Just like in hydra, it is also possible to override the configs from the command line and
         to sweep over multiple values of a given configuration when executing python code.
         See: https://hydra.cc/docs/intro/ for complete documentation on how to use Hydra.
 
-        2. Seeding: Additionally, mlxpy.launch takes an optional argument 'seeding_function'.
+        2. Seeding: Additionally, mlxp.launch takes an optional argument 'seeding_function'.
         By default, 'seeding_function' is None and does nothing. If a callable object is passed to it, this object is called with the argument cfg.config.seed
         right before calling the decorated function. The user-defined callable is meant to set the seed of any random number generator used in the code.
         In that case, the option 'ctx.config.seed' must be none empty.
 
         3. Submitting jobs to a cluster queue using a scheduler.
         This is achieved by setting the config value scheduler.name to the name of a valid scheduler.
         Two job schedulers are currently supported by default: ['OARScheduler', 'SLURMScheduler' ].
@@ -176,48 +176,48 @@
                     'start_time': now.strftime("%H:%M:%S"),
                     'status': Status.STARTING.value}
 
             
 
             cfg.update({'info': info})
 
-            if cfg.mlxpy.use_version_manager:
-                version_manager = _instance_from_config(cfg.mlxpy.version_manager)
+            if cfg.mlxp.use_version_manager:
+                version_manager = _instance_from_config(cfg.mlxp.version_manager)
                 version_manager._handle_interactive_mode(
-                    cfg.mlxpy.interactive_mode, vm_choices_file)
+                    cfg.mlxp.interactive_mode, vm_choices_file)
                 work_dir = version_manager.make_working_directory()
                 cfg.update({'info': {'version_manager': version_manager.get_info()}})
             else:
                 work_dir = os.getcwd()
 
             cfg.update({'info': {'work_dir': work_dir}})
 
-            if cfg.mlxpy.use_scheduler:
+            if cfg.mlxp.use_scheduler:
 
-                scheduler = _instance_from_config(cfg.mlxpy.scheduler)
-                if not cfg.mlxpy.use_logger:
+                scheduler = _instance_from_config(cfg.mlxp.scheduler)
+                if not cfg.mlxp.use_logger:
                     print("Logger is currently disabled.")
                     print("To use the scheduler, the logger must be enabled")
                     print("Enabling the logger...")
-                    cfg.mlxpy.use_logger = True
+                    cfg.mlxp.use_logger = True
             else:
                 scheduler = None
 
-            if cfg.mlxpy.use_logger:
-                logger = _instance_from_config(cfg.mlxpy.logger)
+            if cfg.mlxp.use_logger:
+                logger = _instance_from_config(cfg.mlxp.logger)
                 log_id = logger.log_id
                 log_dir = logger.log_dir
                 parent_log_dir = logger.parent_log_dir
                 cfg.update({'info': {'logger': logger.get_info()}})
                 cfg.update({'config': _get_configs(log_dir)})
                 #cfg = _add_config_overrides(cfg,overrides)
             else:
                 logger = None
 
-            if cfg.mlxpy.use_scheduler:
+            if cfg.mlxp.use_scheduler:
 
                 main_cmd = _main_job_command(cfg.info.executable,
                                              cfg.info.current_file_path,
                                              work_dir,
                                              parent_log_dir,
                                              log_id)
 
@@ -228,15 +228,15 @@
             else:
 
                 # ## Setting up the working directory
                 cur_dir = os.getcwd()
                 _set_work_dir(work_dir)
 
                 if logger:
-                    cfg.update({'info': _get_mlxpy_configs(log_dir)})
+                    cfg.update({'info': _get_mlxp_configs(log_dir)})
                 try:
 
                     cfg.update({'info': {'status': Status.RUNNING.value}})
                     if logger:
                         logger._log_configs(cfg)
                     if seeding_function:
                         try:
@@ -244,15 +244,15 @@
                         except AssertionError:
                             msg = "Missing field: The 'config' must contain a field 'seed'\n"
                             msg += "provided as argument to the function 'seeding_function' "
                             raise MissingFieldError(msg)
                         seeding_function(cfg.config.seed)
 
                     ctx = Context(config=cfg.config,
-                                  mlxpy=cfg.mlxpy,
+                                  mlxp=cfg.mlxp,
                                   info=cfg.info,
                                   logger=logger)
                     task_function(ctx)
                     now = datetime.now()
                     info = {'end_date': now.strftime("%d/%m/%Y"),
                             'end_time': now.strftime("%H:%M:%S"),
                             'status': Status.COMPLETE.value}
@@ -290,28 +290,28 @@
 
     return composed_decorator
 
 
 @dataclass
 class Context:
     """
-    The contex object passed to the decorated function when using decorator mlxpy.launch.
+    The contex object passed to the decorated function when using decorator mlxp.launch.
 
     .. py:attribute:: config
         :type: ConfigDict
 
         A structure containing project-specific options provided by the user.
         These options are loaded from a yaml file 'config.yaml' contained in the directory 'config_path'
-        provided as argument to the decorator mlxpy.launch. It's content can be overriden from the command line.
+        provided as argument to the decorator mlxp.launch. It's content can be overriden from the command line.
 
-    .. py:attribute:: mlxpy
+    .. py:attribute:: mlxp
         :type: ConfigDict
 
-        A structure containing MLXPy's default settings for the project.
-        Its content is loaded from a yaml file 'mlxpy.yaml' located in the same directory 'config.yaml'.
+        A structure containing MLXP's default settings for the project.
+        Its content is loaded from a yaml file 'mlxp.yaml' located in the same directory 'config.yaml'.
 
     .. py:attribute:: info
         :type: ConfigDict
 
         A structure containing information about the current run: ex. status, start time, hostname, etc.
 
     .. py:attribute:: logger
@@ -319,15 +319,15 @@
 
         A logger object that can be used for logging variables (metrics, checkpoints, artifacts).
         When logging is enabled, these variables are all stored in a uniquely defined directory.
 
     """
 
     config: ConfigDict = None
-    mlxpy: ConfigDict = None
+    mlxp: ConfigDict = None
     info: ConfigDict = None
     logger: Union[Logger, None] = None
 
 
 T = TypeVar('T')
 
 
@@ -349,15 +349,15 @@
 
     return attr
 
 
 def _import_module(module_name):
     module, attr = os.path.splitext(module_name)
     if not attr:
-        return getattr(mlxpy, module)
+        return getattr(mlxp, module)
     else:
         try:
             module = importlib.import_module(module)
             return getattr(module, attr[1:])
         except BaseException:
             try:
                 module = _import_module(module)
@@ -402,16 +402,16 @@
         fn_code.co_firstlineno,
         fn_code.co_lnotab,
         fn_code.co_freevars,
         fn_code.co_cellvars,
     )
 
 
-def _get_mlxpy_configs(log_dir):
-    from mlxpy.enumerations import Directories
+def _get_mlxp_configs(log_dir):
+    from mlxp.enumerations import Directories
     abs_name = os.path.join(log_dir, Directories.Metadata.value, 'info.yaml')
     configs_info = {}
 
     if os.path.isfile(abs_name):
         with open(abs_name, "r") as file:
             configs = yaml.safe_load(file)
             if 'scheduler' in configs:
@@ -421,15 +421,15 @@
             if 'logger' in configs:
                 configs_info.update({'logger': configs['logger']})
 
     return configs_info
 
 
 def _get_configs(log_dir):
-    from mlxpy.enumerations import Directories
+    from mlxp.enumerations import Directories
     abs_name = os.path.join(log_dir, Directories.Metadata.value, 'config.yaml')
     configs = {}
 
     if os.path.isfile(abs_name):
         with open(abs_name, "r") as file:
             configs = yaml.safe_load(file)
 
@@ -440,18 +440,18 @@
 def _main_job_command(executable, current_file_path, work_dir, parent_log_dir, job_id):
     exec_file = os.path.relpath(current_file_path, os.getcwd())
 
     args = _get_overrides()
     values = [
         f"cd {work_dir}",
         f"{executable} {exec_file} {args} \
-            +mlxpy.logger.forced_log_id={job_id}\
-            +mlxpy.logger.parent_log_dir={parent_log_dir} \
-            +mlxpy.use_scheduler={False}\
-            +mlxpy.use_version_manager={False}"
+            +mlxp.logger.forced_log_id={job_id}\
+            +mlxp.logger.parent_log_dir={parent_log_dir} \
+            +mlxp.use_scheduler={False}\
+            +mlxp.use_version_manager={False}"
     ]
 
     values = [f"{val}\n" for val in values]
     return "".join(values)
 
 
 def _get_overrides():
```

### Comparing `MLXP-0.0.1/mlxpy/logger.py` & `MLXP-0.0.2/mlxp/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 import yaml
 import random
 from time import sleep
 import dill as pkl
 from typing import Any, Dict, Union
 import abc
 
-from mlxpy.data_structures.artifacts import Artifact, Checkpoint
-from mlxpy.errors import InvalidKeyError, InvalidArtifactError
-from mlxpy.data_structures.config_dict import ConfigDict
+from mlxp.data_structures.artifacts import Artifact, Checkpoint
+from mlxp.errors import InvalidKeyError, InvalidArtifactError
+from mlxp.data_structures.config_dict import ConfigDict
 
-from mlxpy.enumerations import Directories
+from mlxp.enumerations import Directories
 
 
 class Logger(abc.ABC):
     """A logger that allows saving outputs of the run in a uniquely assigned directory for the specific run.
 
     The logger creates a directory with a default file structure:
 
@@ -91,17 +91,17 @@
     def _log_configs(self, config: ConfigDict) -> None:
         file_name = os.path.join(self.metadata_dir, 'config')
         with open(file_name + ".yaml", "w") as f:
             yaml.dump(config.config.to_dict(), f)
         file_name = os.path.join(self.metadata_dir, 'info')
         with open(file_name + ".yaml", "w") as f:
             yaml.dump(config.info.to_dict(), f)
-        file_name = os.path.join(self.metadata_dir, 'mlxpy')
+        file_name = os.path.join(self.metadata_dir, 'mlxp')
         with open(file_name + ".yaml", "w") as f:
-            yaml.dump(config.mlxpy.to_dict(), f)
+            yaml.dump(config.mlxp.to_dict(), f)
 
     def get_info(self) -> None:
         """Return a dictionary containing information about the logger settings used for the run.
 
         :return: Dictionary containing information about the logger settings used for the run.
         :rtype: Dict[str, Any]
         """
@@ -118,17 +118,17 @@
 
         :param metrics_dict:  Dictonary of scalar values to be saved, the values can be either int, float of string.
         :param log_name: Name of the json file where to save the metric_dict.
         :type metrics_dict: Dict[str, Union[int, float, str]]
         :type log_name: str
         :return: None
         """
-        invalid_names = ["info", "config", "mlxpy"]
+        invalid_names = ["info", "config", "mlxp"]
         try:
-            assert log_name not in ["info", "config", "mlxpy"]
+            assert log_name not in ["info", "config", "mlxp"]
         except AssertionError:
             raise InvalidKeyError(
                 f"The chosen log_nam:  {log_name} is invalid! It must be different from these protected names: {invalid_names} ")
 
         self._log_metrics_key(metrics_dict, log_name)
         file_name = os.path.join(self.metrics_dir, log_name)
         return self._log_metrics(metrics_dict, file_name)
```

### Comparing `MLXP-0.0.1/mlxpy/parser.py` & `MLXP-0.0.2/mlxp/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import ply.lex as lex
 import ply.yacc as yacc
 import ast
 from operator import eq, ge, gt, le, lt, ne
 from tinydb import where, Query
 from tinydb.queries import QueryInstance
 import abc
-from mlxpy.errors import InvalidKeyError
+from mlxp.errors import InvalidKeyError
 
 
-from mlxpy.enumerations import SearchableKeys
+from mlxp.enumerations import SearchableKeys
 
 
 class Parser(abc.ABC):
     """An abstract class for parsing queries. Any parser used by the class Reader must inherit from this abstract class."""
 
     @abc.abstractmethod
     def parse(self, query: str) -> QueryInstance:
@@ -26,15 +26,15 @@
         :rtype: QueryInstance
         :raises SyntaxError: if the query string does not follow expected syntax.
         """
         pass
 
 
 class DefaultParser(Parser):
-    """MLXPy's deafult parser inspired from python's syntax."""
+    """MLXP's deafult parser inspired from python's syntax."""
 
     def __init__(self):
         self.lexer = _Lexer()
         self.parser = _YaccParser()
 
     def parse(self, query: str) -> QueryInstance:
         """Parse a query string into a tinydb QueryInstance object."""
```

### Comparing `MLXP-0.0.1/mlxpy/reader.py` & `MLXP-0.0.2/mlxp/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import os
 import yaml
 
 from tinydb import TinyDB
 from tinydb.storages import JSONStorage
 from tinydb.table import Document
 
-from mlxpy.data_structures.data_dict import DataDictList, DataDict, LAZYDATA
-from mlxpy.parser import Parser, DefaultParser, _is_searchable
+from mlxp.data_structures.data_dict import DataDictList, DataDict, LAZYDATA
+from mlxp.parser import Parser, DefaultParser, _is_searchable
 from typing import Union, Optional
 import pandas as pd
 
 from collections.abc import MutableMapping
-from mlxpy.enumerations import DataFrameType, Directories
+from mlxp.enumerations import DataFrameType, Directories
 
 
 class Reader(object):
     """A class for exploiting the results stored in several runs contained in a same parent directory 'src_dir'.
 
     Once, created, it is possible to query the database using the method 'filter'
     to get the results matching a specific configuration setting.
@@ -131,34 +131,34 @@
         if result_format == DataFrameType.Pandas.value:
             return res.toPandasDF(lazy=False)
         elif result_format == DataFrameType.DataDictList.value:
             return res
 
     @property
     def fields(self) -> pd.DataFrame:
-        """Return all fields of the database except those specific to MLXPy, excluding the fields contained in the file 'mlxpy.yaml'.
+        """Return all fields of the database except those specific to MLXP, excluding the fields contained in the file 'mlxp.yaml'.
 
         return: a dataframe of all fields contained in the database
         rtype: pd.DataFrame
         """
         fields_dict = {
             k: v
             for d in self._fields.all()
             for k, v in d.items()
-            if not k.startswith("mlxpy")
+            if not k.startswith("mlxp")
         }
         df = pd.DataFrame(list(fields_dict.items()), columns=["Fields", "Type"])
         df.set_index("Fields", inplace=True)
         df = df.sort_index()
 
         return df
 
     @property
     def searchable(self) -> pd.DataFrame:
-        """Return all fields of the database that are searchable, excluding the fields contained in the file 'mlxpy.yaml'.
+        """Return all fields of the database that are searchable, excluding the fields contained in the file 'mlxp.yaml'.
 
         return: a dataframe of all fields contained in the database that can be searched using the method filter
         rtype: pd.DataFrame
         """
         fields_dict = {
             k: v for d in self._fields.all() for k, v in d.items() if _is_searchable(k)
         }
@@ -201,15 +201,15 @@
 
     relpath = os.path.relpath(abs_metrics_dir,parent_log_dir)
 
     return os.path.join(src_dir,relpath)
 
 
 def _get_data(path, metadata_file):
-    data = {"config": {}, "info": {}, "mlxpy": {}}
+    data = {"config": {}, "info": {}, "mlxp": {}}
     for key in data:
         fname = os.path.join(path, Directories.Metadata.value, key + ".yaml")
         with open(fname, "r") as file:
             data[key] = yaml.safe_load(file)
 
     metadata_dict = _flatten_dict(data, parent_key="")
```

### Comparing `MLXP-0.0.1/mlxpy/scheduler.py` & `MLXP-0.0.2/mlxp/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import subprocess
 from omegaconf.errors import OmegaConfBaseException
 import abc
 from typing import List, Dict, Any 
 
-from mlxpy.errors import JobSubmissionError
+from mlxp.errors import JobSubmissionError
 
 
 class Scheduler(abc.ABC):
     """An abstract class whose children allow to submit jobs using a particular job scheduler such as OAR or SLURM.
 
     .. py:attribute:: directive
         :type: str
```

### Comparing `MLXP-0.0.1/mlxpy/version_manager.py` & `MLXP-0.0.2/mlxp/version_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import abc
 import subprocess
 import yaml
 from typing import Any, Dict
 
-from mlxpy._internal._interactive_mode import _bcolors, _printc
+from mlxp._internal._interactive_mode import _bcolors, _printc
 
 
 class VersionManager(abc.ABC):
     """An abstract class whose children allow custumizing the working directory of the run."""
 
     def __init__(self):
 
@@ -231,15 +231,15 @@
                     )
                     choice = input(
                         f"{_bcolors.OKGREEN}[Uncommitted changes]: Please enter your choice (a/b/c): {_bcolors.ENDC}"
                     )
                     if choice == "a":
                         _printc(_bcolors.OKBLUE, "Commiting changes....")
                         output_msg = repo.git.commit(
-                            "-a", "-m", "mlxpy: Automatically committing all changes"
+                            "-a", "-m", "mlxp: Automatically committing all changes"
                         )
                         _printc(_bcolors.OKBLUE, output_msg)
 
                         if not repo.is_dirty():
                             _printc(_bcolors.OKBLUE, "No more uncommitted changes!")
                             break
                     elif choice == "b":
@@ -318,15 +318,15 @@
                             # Split user input by commas
                             files_to_add = files_input.split(",")
 
                             # Add selected files
                             for file in files_to_add:
                                 repo.git.add(file.strip())
                             # Commit the changes
-                            # repo.index.commit("mlxpy: Committing selected files ")
+                            # repo.index.commit("mlxp: Committing selected files ")
                             if not repo.untracked_files:
                                 break
                         else:
                             _printc(_bcolors.OKBLUE, "No files added. Skipping...")
                             print(ignore_msg)
                             break
                     elif choice == "b":
```

### Comparing `MLXP-0.0.1/setup.py` & `MLXP-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 ver_dic = {}
 exec(
     compile(
-        open("mlxpy/__init__.py").read(), "mlxpy/__init__.py", "exec"
+        open("mlxp/__init__.py").read(), "mlxp/__init__.py", "exec"
     ),
     ver_dic,
 )
```

