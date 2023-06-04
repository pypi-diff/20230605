# Comparing `tmp/astartes-1.0.0rc1.tar.gz` & `tmp/astartes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astartes-1.0.0rc1.tar", last modified: Fri Mar 24 18:57:30 2023, max compression
+gzip compressed data, was "astartes-1.0.1.tar", last modified: Sun Jun  4 23:52:07 2023, max compression
```

## Comparing `astartes-1.0.0rc1.tar` & `astartes-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.714463 astartes-1.0.0rc1/astartes/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17498 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/molecules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.714463 astartes-1.0.0rc1/astartes/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/abstract_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/astartes/samplers/extrapolation/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/dbscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/optisim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/sphere_exclusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/astartes/samplers/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/doptimal.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/duplex.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/kennardstone.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/mtsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/random_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/spxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/astartes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/utils/sampler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.714463 astartes-1.0.0rc1/astartes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-03-24 18:57:30.000000 astartes-1.0.0rc1/astartes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-24 18:57:30.000000 astartes-1.0.0rc1/astartes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 18:57:30.000000 astartes-1.0.0rc1/astartes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-24 18:57:30.000000 astartes-1.0.0rc1/astartes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-24 18:57:30.000000 astartes-1.0.0rc1/astartes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/test/test_astartes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/test/test_molecules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.686536 astartes-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-04 23:51:56.000000 astartes-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-04 23:52:07.686536 astartes-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-06-04 23:51:56.000000 astartes-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.682536 astartes-1.0.1/astartes/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/molecules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.682536 astartes-1.0.1/astartes/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/abstract_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.682536 astartes-1.0.1/astartes/samplers/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/dbscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/optisim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/sphere_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/extrapolation/time_based.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.686536 astartes-1.0.1/astartes/samplers/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/interpolation/kennardstone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/interpolation/mtsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/interpolation/random_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/samplers/interpolation/spxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.686536 astartes-1.0.1/astartes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/utils/convert_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/utils/sampler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-04 23:51:56.000000 astartes-1.0.1/astartes/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:52:07.682536 astartes-1.0.1/astartes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-04 23:52:07.000000 astartes-1.0.1/astartes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-04 23:52:07.000000 astartes-1.0.1/astartes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:52:07.000000 astartes-1.0.1/astartes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-04 23:52:07.000000 astartes-1.0.1/astartes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 23:52:07.000000 astartes-1.0.1/astartes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-04 23:51:56.000000 astartes-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:52:07.686536 astartes-1.0.1/setup.cfg
```

### Comparing `astartes-1.0.0rc1/LICENSE` & `astartes-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0rc1/PKG-INFO` & `astartes-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: astartes
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays
 Author-email: Jackson Burns <jwburns@mit.edu>, Himaghna Bhattacharjee <himaghna@udel.edu>, Kevin Spiekermann <kspieker@mit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/astartes
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: molecules
 Provides-Extra: dev
+Provides-Extra: demos
 License-File: LICENSE
 
 <h1 align="center">astartes</h1> 
 <h3 align="center">Train:Validation:Test Algorithmic Sampling for Molecules and Arbitrary Arrays</h3>
 
 <p align="center">  
-  <img alt="astarteslogo" src="https://github.com/JacksonBurns/astartes/blob/main/astartes_logo.png">
+  <img alt="astarteslogo" src="https://raw.githubusercontent.com/JacksonBurns/astartes/main/astartes_logo.png">
 </p> 
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/JacksonBurns/astartes?style=social">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/astartes">
+  <img alt="PyPI - Total Downloads" src="https://static.pepy.tech/personalized-badge/astartes?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Lifetime%20Downloads">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/astartes">
   <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/astartes?style=plastic">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/JacksonBurns/astartes">
   <img alt="Test Status" src="https://github.com/JacksonBurns/astartes/actions/workflows/run_tests.yml/badge.svg?branch=main&event=schedule">
+  <img alt="Reproduce Paper" src="https://github.com/JacksonBurns/astartes/actions/workflows/reproduce_paper.yml/badge.svg?branch=main&event=schedule">
 </p>
 
 ## Installing `astartes`
 We recommend installing `astartes` within a virtual environment, using either `venv` or `conda` (or other tools) to simplify dependency management. Python versions 3.7, 3.8, 3.9, 3.10, and 3.11 are supported on all platforms.
 
 `astartes` is available on `PyPI` and can be installed using `pip`:
 
@@ -40,47 +42,53 @@
  - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer dependencies and may be more readily compatible in environments with existing workflows).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install "astartes[molecules]"`)
 
 ## Using `astartes`
 `astartes` is designed as a drop-in replacement for `sklearn`'s `train_test_split` function. To switch to `astartes`, change `from sklearn.model_selection import train_test_split` to `from astartes import train_test_split`.
 
-By default, `astartes` will use a random splitting approach identical to that which is implemented in `sklearn`, and a variety of deterministic sampling approaches can be used by specifying one additional argument ot the function:
+By default, `astartes` will split data randomly. Additionally, a variety of algorithmic sampling approaches can be used by specifying the `sampler` argument to the function:
 
 ```python
 X_train, X_test, y_train, y_test = train_test_split(
-  X,
+  X,  # preferably numpy arrays, but astartes will cast it for you
   y,
   sampler = 'kennard_stone',  # any of the supported samplers
 )
 ```
 
+### Paper
+For a comprehensive walkthrough of the theory and implementation of `astartes`, follow [this link](https://github.com/JacksonBurns/astartes/raw/joss-paper/Burns-Spiekermann-Bhattacharjee_astartes.pdf) to read the companion paper.
+
 ### Example Notebooks
 
 Click the badges in the table below to be taken to a live, interactive demo of `astartes`:
 
 | Demo | Link |
 |:---:|---|
-| Using `train_val_test_split` with the `sklearn` example datasets | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Ftrain_val_test_split_example.ipynb) |
-| Cheminformatics sample set partitioning with `astartes` | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2FRDB7_barrier_prediction_example.ipynb) |
+| Using `train_val_test_split` with the `sklearn` example datasets | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Ftrain_val_test_split_sklearn_example%2Ftrain_val_test_split_example.ipynb) |
+| Comparing Sampling Algorithms with Fast Food | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Fsplit_comparisons%2Fsplit_comparisons.ipynb) |
+| Cheminformatics sample set partitioning with `astartes` | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Fbarrier_prediction_with_RDB7%2FRDB7_barrier_prediction_example.ipynb) |
+| Comparing partitioning approaches for alkanes | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Fmlpds_2023_astartes_demo%2Fmlpds_2023_demo.ipynb) |
 
 ### Rational Splitting Algorithms
-While much machine learning is done with a random choice between training/test/validation data, an alternative is the use of so-called "rational" splitting algorithms. These approaches use some similarity-based algorithm to divide data into sets. Some of these algorithms include Kennard-Stone, minimal test set dissimilarity, and sphere exclusion algorithms [as discussed by Tropsha et. al](https://pubs.acs.org/doi/pdf/10.1021/ci300338w) as well as the OptiSim as discussed in [Applied Chemoinformatics: Achievements and Future Opportunities](https://www.wiley.com/en-us/Applied+Chemoinformatics%3A+Achievements+and+Future+Opportunities-p-9783527806546). Some clustering-based splitting techniques have also been introduced, such as [DBSCAN](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1016.890&rep=rep1&type=pdf).
+While much machine learning is done with a random choice between training/validation/test data, an alternative is the use of so-called "rational" splitting algorithms. These approaches use some similarity-based algorithm to divide data into sets. Some of these algorithms include Kennard-Stone, minimal test set dissimilarity, and sphere exclusion algorithms [as discussed by Tropsha et. al](https://pubs.acs.org/doi/pdf/10.1021/ci300338w) as well as the OptiSim as discussed in [Applied Chemoinformatics: Achievements and Future Opportunities](https://www.wiley.com/en-us/Applied+Chemoinformatics%3A+Achievements+and+Future+Opportunities-p-9783527806546). Some clustering-based splitting techniques have also been incorporated, such as [DBSCAN](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1016.890&rep=rep1&type=pdf).
 
-There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-sample data, effectively asking a 'harder question' than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`, as well as the hyperparameters that each algorithm accepts (which are passed in with `hopts`) and a helpful reference for understanding how the hyperparameters work. Note that `random_state` is defined as a keyword argument in `train_test_split` itself, even though these algorithms will use the `random_state` in their own work. Do not provide a `random_state` in the `hopts` dictionary - it will be overwritten by the `random_state` you provide for `train_test_split` (or the default if none is provided).
+There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-sample data, which creates a more challenging task than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`, as well as the hyperparameters that each algorithm accepts (which are passed in with `hopts`) and a helpful reference for understanding how the hyperparameters work. Note that `random_state` is defined as a keyword argument in `train_test_split` itself, even though these algorithms will use the `random_state` in their own work. Do not provide a `random_state` in the `hopts` dictionary - it will be overwritten by the `random_state` you provide for `train_test_split` (or the default if none is provided).
 
 #### Implemented Sampling Algorithms
 
 | Sampler Name | Usage String | Type | Hyperparameters | Reference | Notes |
 |:---:|---|---|---|---|---|
 | Random | 'random' | Interpolative | `shuffle` | [`sklearn train_test_split`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) | This sampler is a direct passthrough to `sklearn`'s `train_test_split`, though it does not currently reproduce splits identically. |
-| Kennard-Stone | 'kennard_stone' | Interpolative | _none_ | [yu9824's `kennard_stone`](https://github.com/yu9824/kennard_stone) | Fully deterministic, no hyperparameters accepted. |
-| Sample set Partitioning based on join X-Y distances (SPXY) | 'spxy' | Interpolative | `distance_metric` | Saldhana et. al [original paper](https://www.sciencedirect.com/science/article/abs/pii/S003991400500192X) | Extension of Kennard Stone that also includes the response when sampling distances. |
-| Scaffold | 'scaffold' | Extrapolative | `explicit_hydrogens`, `include_chirality` | [Bemis-Murcko Scaffold](https://pubs.acs.org/doi/full/10.1021/jm9602928) as implemented in RDKit | This sampler requires SMILES strings as input (use the `molecules` subpackage) |
+| Kennard-Stone | 'kennard_stone' | Interpolative | `metric` | [Kennard & Stone](https://www.tandfonline.com/doi/abs/10.1080/00401706.1969.10490666) | Euclidian distance is used by default, as described in the original paper. |
+| Sample set Partitioning based on joint X-Y distances (SPXY) | 'spxy' | Interpolative | `distance_metric` | Saldhana et. al [original paper](https://www.sciencedirect.com/science/article/abs/pii/S003991400500192X) | Extension of Kennard Stone that also includes the response when sampling distances. |
+| Scaffold | 'scaffold' | Extrapolative | `include_chirality` | [Bemis-Murcko Scaffold](https://pubs.acs.org/doi/full/10.1021/jm9602928) as implemented in RDKit | This sampler requires SMILES strings as input (use the `molecules` subpackage) |
 | Sphere Exclusion | 'sphere_exclusion' | Extrapolative | `metric`, `distance_cutoff` | _custom implementation_ | Variation on Sphere Exclusion for arbitrary-valued vectors. |
+| Time Based | 'time_based' | Extrapolative | _none_ | [Chen et al.](https://pubs.acs.org/doi/full/10.1021/ci200615h), [Sheridan, R. P](https://pubs.acs.org/doi/full/10.1021/ci400084k), [Feinberg et al.](https://pubs.acs.org/doi/full/10.1021/acs.jmedchem.9b02187), [Struble et al.](https://pubs.rsc.org/en/content/articlehtml/2020/re/d0re00071j)  | This sampler requires `labels` to be an iterable of either date or datetime objects. |
 | Optimizable K-Dissimilarity Selection (OptiSim) | 'optisim' | Extrapolative | `n_clusters`, `max_subsample_size`, `distance_cutoff` | _custom implementation_ | Variation on [OptiSim](https://pubs.acs.org/doi/10.1021/ci025662h) for arbitrary-valued vectors. |
 | K-Means | 'kmeans' | Extrapolative | `n_clusters`, `n_init` | [`sklearn KMeans`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) | Passthrough to `sklearn`'s `KMeans`. |
 | Density-Based Spatial Clustering of Applications with Noise (DBSCAN) | 'dbscan' | Extrapolative | `eps`, `min_samples`, `algorithm`, `metric`, `leaf_size` | [`sklearn DBSCAN`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html) | Passthrough to `sklearn`'s `DBSCAN`. |
 | Minimum Test Set Dissimilarity (MTSD) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 | Restricted Boltzmann Machine (RBM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 | Kohonen Self-Organizing Map (SOM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 | SPlit Method | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
@@ -114,17 +122,38 @@
 )
 ```
 
 To see a complete example of using `train_test_split_molecules` with actual chemical data, take a look in the `examples` directory.
 
 Configuration options for the featurization scheme can be found in the documentation for [`AIMSim`](https://vlachosgroup.github.io/AIMSim/README.html#currently-implemented-fingerprints) though most of the critical configuration options are shown above.
 
+### Reproducibility
+`astartes` aims to be completely reproducible across different platforms, Python versions, and dependency configurations - any version of `astartes` v1.x should result in the _exact_ same splits, always.
+To that end, the default behavior of `astartes` is to use `42` as the random seed and _always_ set it.
+Running `astartes` with the default settings will always produce the exact same results.
+We have verified this behavior on Debian Ubuntu, Windows, and Intel Macs from Python versions 3.7 through 3.11 (with appropriate dependencies for each version).
+We are limited in our ability to test on M1 Macs, but from our limited manual testing we achieve perfect reproducbility in all cases _except occasionally_ with `KMeans` on Apple silicon. It has produced _slightly_ different results between platforms regardless of `random_state`, with up to two clusters being assigned differently resulting in data splits which are >99% identical. `astartes` is still consistent between runs on the same platform in all cases.
+
 ## Online Documentation
 [The online documentation](https://JacksonBurns.github.io/astartes/) contains everything you see in this README with an additional tutorial for [moving from `train_test_split` in `sklearn` to `astartes`](https://jacksonburns.github.io/astartes/sklearn_to_astartes.html).
 
+## How to Cite
+If you use `astartes` in your work please use the below citation or the "Cite this repository" button on GitHub:
+> **BibTeX**
+> @software{Burns_astartes,
+>   author = {Burns, Jackson and Spiekermann, Kevin and Bhattacharjee, Himaghna and Vlachos, Dionisios and Green, William},
+>   license = {MIT},
+>   title = {{astartes}},
+>   url = {https://github.com/JacksonBurns/astartes}
+> }
+
+> **APA**
+> Burns, J., Spiekermann, K., Bhattacharjee, H., Vlachos, D., & Green, W. astartes [Computer software]. https://github.com/JacksonBurns/astartes
+
+
 ## Contributing & Developer Notes
 Pull Requests, Bug Reports, and all Contributions are welcome! Please use the appropriate issue or pull request template when making a contribution.
 
 We make use of [the GitHub Discussions page](https://github.com/JacksonBurns/astartes/discussions) to go over potential features to add. Please feel free to stop by if you are looking for something to develop or have an idea for a useful feature!
 
 When submitting a PR, please mark your PR with the "PR Ready for Review" label when you are finished making changes so that the GitHub actions bots can work their magic!
```

### Comparing `astartes-1.0.0rc1/README.md` & `astartes-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 <h1 align="center">astartes</h1> 
 <h3 align="center">Train:Validation:Test Algorithmic Sampling for Molecules and Arbitrary Arrays</h3>
 
 <p align="center">  
-  <img alt="astarteslogo" src="https://github.com/JacksonBurns/astartes/blob/main/astartes_logo.png">
+  <img alt="astarteslogo" src="https://raw.githubusercontent.com/JacksonBurns/astartes/main/astartes_logo.png">
 </p> 
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/JacksonBurns/astartes?style=social">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/astartes">
+  <img alt="PyPI - Total Downloads" src="https://static.pepy.tech/personalized-badge/astartes?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Lifetime%20Downloads">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/astartes">
   <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/astartes?style=plastic">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/JacksonBurns/astartes">
   <img alt="Test Status" src="https://github.com/JacksonBurns/astartes/actions/workflows/run_tests.yml/badge.svg?branch=main&event=schedule">
+  <img alt="Reproduce Paper" src="https://github.com/JacksonBurns/astartes/actions/workflows/reproduce_paper.yml/badge.svg?branch=main&event=schedule">
 </p>
 
 ## Installing `astartes`
 We recommend installing `astartes` within a virtual environment, using either `venv` or `conda` (or other tools) to simplify dependency management. Python versions 3.7, 3.8, 3.9, 3.10, and 3.11 are supported on all platforms.
 
 `astartes` is available on `PyPI` and can be installed using `pip`:
 
@@ -22,47 +23,53 @@
  - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer dependencies and may be more readily compatible in environments with existing workflows).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install "astartes[molecules]"`)
 
 ## Using `astartes`
 `astartes` is designed as a drop-in replacement for `sklearn`'s `train_test_split` function. To switch to `astartes`, change `from sklearn.model_selection import train_test_split` to `from astartes import train_test_split`.
 
-By default, `astartes` will use a random splitting approach identical to that which is implemented in `sklearn`, and a variety of deterministic sampling approaches can be used by specifying one additional argument ot the function:
+By default, `astartes` will split data randomly. Additionally, a variety of algorithmic sampling approaches can be used by specifying the `sampler` argument to the function:
 
 ```python
 X_train, X_test, y_train, y_test = train_test_split(
-  X,
+  X,  # preferably numpy arrays, but astartes will cast it for you
   y,
   sampler = 'kennard_stone',  # any of the supported samplers
 )
 ```
 
+### Paper
+For a comprehensive walkthrough of the theory and implementation of `astartes`, follow [this link](https://github.com/JacksonBurns/astartes/raw/joss-paper/Burns-Spiekermann-Bhattacharjee_astartes.pdf) to read the companion paper.
+
 ### Example Notebooks
 
 Click the badges in the table below to be taken to a live, interactive demo of `astartes`:
 
 | Demo | Link |
 |:---:|---|
-| Using `train_val_test_split` with the `sklearn` example datasets | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Ftrain_val_test_split_example.ipynb) |
-| Cheminformatics sample set partitioning with `astartes` | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2FRDB7_barrier_prediction_example.ipynb) |
+| Using `train_val_test_split` with the `sklearn` example datasets | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Ftrain_val_test_split_sklearn_example%2Ftrain_val_test_split_example.ipynb) |
+| Comparing Sampling Algorithms with Fast Food | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Fsplit_comparisons%2Fsplit_comparisons.ipynb) |
+| Cheminformatics sample set partitioning with `astartes` | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Fbarrier_prediction_with_RDB7%2FRDB7_barrier_prediction_example.ipynb) |
+| Comparing partitioning approaches for alkanes | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Fmlpds_2023_astartes_demo%2Fmlpds_2023_demo.ipynb) |
 
 ### Rational Splitting Algorithms
-While much machine learning is done with a random choice between training/test/validation data, an alternative is the use of so-called "rational" splitting algorithms. These approaches use some similarity-based algorithm to divide data into sets. Some of these algorithms include Kennard-Stone, minimal test set dissimilarity, and sphere exclusion algorithms [as discussed by Tropsha et. al](https://pubs.acs.org/doi/pdf/10.1021/ci300338w) as well as the OptiSim as discussed in [Applied Chemoinformatics: Achievements and Future Opportunities](https://www.wiley.com/en-us/Applied+Chemoinformatics%3A+Achievements+and+Future+Opportunities-p-9783527806546). Some clustering-based splitting techniques have also been introduced, such as [DBSCAN](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1016.890&rep=rep1&type=pdf).
+While much machine learning is done with a random choice between training/validation/test data, an alternative is the use of so-called "rational" splitting algorithms. These approaches use some similarity-based algorithm to divide data into sets. Some of these algorithms include Kennard-Stone, minimal test set dissimilarity, and sphere exclusion algorithms [as discussed by Tropsha et. al](https://pubs.acs.org/doi/pdf/10.1021/ci300338w) as well as the OptiSim as discussed in [Applied Chemoinformatics: Achievements and Future Opportunities](https://www.wiley.com/en-us/Applied+Chemoinformatics%3A+Achievements+and+Future+Opportunities-p-9783527806546). Some clustering-based splitting techniques have also been incorporated, such as [DBSCAN](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1016.890&rep=rep1&type=pdf).
 
-There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-sample data, effectively asking a 'harder question' than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`, as well as the hyperparameters that each algorithm accepts (which are passed in with `hopts`) and a helpful reference for understanding how the hyperparameters work. Note that `random_state` is defined as a keyword argument in `train_test_split` itself, even though these algorithms will use the `random_state` in their own work. Do not provide a `random_state` in the `hopts` dictionary - it will be overwritten by the `random_state` you provide for `train_test_split` (or the default if none is provided).
+There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-sample data, which creates a more challenging task than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`, as well as the hyperparameters that each algorithm accepts (which are passed in with `hopts`) and a helpful reference for understanding how the hyperparameters work. Note that `random_state` is defined as a keyword argument in `train_test_split` itself, even though these algorithms will use the `random_state` in their own work. Do not provide a `random_state` in the `hopts` dictionary - it will be overwritten by the `random_state` you provide for `train_test_split` (or the default if none is provided).
 
 #### Implemented Sampling Algorithms
 
 | Sampler Name | Usage String | Type | Hyperparameters | Reference | Notes |
 |:---:|---|---|---|---|---|
 | Random | 'random' | Interpolative | `shuffle` | [`sklearn train_test_split`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) | This sampler is a direct passthrough to `sklearn`'s `train_test_split`, though it does not currently reproduce splits identically. |
-| Kennard-Stone | 'kennard_stone' | Interpolative | _none_ | [yu9824's `kennard_stone`](https://github.com/yu9824/kennard_stone) | Fully deterministic, no hyperparameters accepted. |
-| Sample set Partitioning based on join X-Y distances (SPXY) | 'spxy' | Interpolative | `distance_metric` | Saldhana et. al [original paper](https://www.sciencedirect.com/science/article/abs/pii/S003991400500192X) | Extension of Kennard Stone that also includes the response when sampling distances. |
-| Scaffold | 'scaffold' | Extrapolative | `explicit_hydrogens`, `include_chirality` | [Bemis-Murcko Scaffold](https://pubs.acs.org/doi/full/10.1021/jm9602928) as implemented in RDKit | This sampler requires SMILES strings as input (use the `molecules` subpackage) |
+| Kennard-Stone | 'kennard_stone' | Interpolative | `metric` | [Kennard & Stone](https://www.tandfonline.com/doi/abs/10.1080/00401706.1969.10490666) | Euclidian distance is used by default, as described in the original paper. |
+| Sample set Partitioning based on joint X-Y distances (SPXY) | 'spxy' | Interpolative | `distance_metric` | Saldhana et. al [original paper](https://www.sciencedirect.com/science/article/abs/pii/S003991400500192X) | Extension of Kennard Stone that also includes the response when sampling distances. |
+| Scaffold | 'scaffold' | Extrapolative | `include_chirality` | [Bemis-Murcko Scaffold](https://pubs.acs.org/doi/full/10.1021/jm9602928) as implemented in RDKit | This sampler requires SMILES strings as input (use the `molecules` subpackage) |
 | Sphere Exclusion | 'sphere_exclusion' | Extrapolative | `metric`, `distance_cutoff` | _custom implementation_ | Variation on Sphere Exclusion for arbitrary-valued vectors. |
+| Time Based | 'time_based' | Extrapolative | _none_ | [Chen et al.](https://pubs.acs.org/doi/full/10.1021/ci200615h), [Sheridan, R. P](https://pubs.acs.org/doi/full/10.1021/ci400084k), [Feinberg et al.](https://pubs.acs.org/doi/full/10.1021/acs.jmedchem.9b02187), [Struble et al.](https://pubs.rsc.org/en/content/articlehtml/2020/re/d0re00071j)  | This sampler requires `labels` to be an iterable of either date or datetime objects. |
 | Optimizable K-Dissimilarity Selection (OptiSim) | 'optisim' | Extrapolative | `n_clusters`, `max_subsample_size`, `distance_cutoff` | _custom implementation_ | Variation on [OptiSim](https://pubs.acs.org/doi/10.1021/ci025662h) for arbitrary-valued vectors. |
 | K-Means | 'kmeans' | Extrapolative | `n_clusters`, `n_init` | [`sklearn KMeans`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) | Passthrough to `sklearn`'s `KMeans`. |
 | Density-Based Spatial Clustering of Applications with Noise (DBSCAN) | 'dbscan' | Extrapolative | `eps`, `min_samples`, `algorithm`, `metric`, `leaf_size` | [`sklearn DBSCAN`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html) | Passthrough to `sklearn`'s `DBSCAN`. |
 | Minimum Test Set Dissimilarity (MTSD) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 | Restricted Boltzmann Machine (RBM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 | Kohonen Self-Organizing Map (SOM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 | SPlit Method | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
@@ -96,17 +103,38 @@
 )
 ```
 
 To see a complete example of using `train_test_split_molecules` with actual chemical data, take a look in the `examples` directory.
 
 Configuration options for the featurization scheme can be found in the documentation for [`AIMSim`](https://vlachosgroup.github.io/AIMSim/README.html#currently-implemented-fingerprints) though most of the critical configuration options are shown above.
 
+### Reproducibility
+`astartes` aims to be completely reproducible across different platforms, Python versions, and dependency configurations - any version of `astartes` v1.x should result in the _exact_ same splits, always.
+To that end, the default behavior of `astartes` is to use `42` as the random seed and _always_ set it.
+Running `astartes` with the default settings will always produce the exact same results.
+We have verified this behavior on Debian Ubuntu, Windows, and Intel Macs from Python versions 3.7 through 3.11 (with appropriate dependencies for each version).
+We are limited in our ability to test on M1 Macs, but from our limited manual testing we achieve perfect reproducbility in all cases _except occasionally_ with `KMeans` on Apple silicon. It has produced _slightly_ different results between platforms regardless of `random_state`, with up to two clusters being assigned differently resulting in data splits which are >99% identical. `astartes` is still consistent between runs on the same platform in all cases.
+
 ## Online Documentation
 [The online documentation](https://JacksonBurns.github.io/astartes/) contains everything you see in this README with an additional tutorial for [moving from `train_test_split` in `sklearn` to `astartes`](https://jacksonburns.github.io/astartes/sklearn_to_astartes.html).
 
+## How to Cite
+If you use `astartes` in your work please use the below citation or the "Cite this repository" button on GitHub:
+> **BibTeX**
+> @software{Burns_astartes,
+>   author = {Burns, Jackson and Spiekermann, Kevin and Bhattacharjee, Himaghna and Vlachos, Dionisios and Green, William},
+>   license = {MIT},
+>   title = {{astartes}},
+>   url = {https://github.com/JacksonBurns/astartes}
+> }
+
+> **APA**
+> Burns, J., Spiekermann, K., Bhattacharjee, H., Vlachos, D., & Green, W. astartes [Computer software]. https://github.com/JacksonBurns/astartes
+
+
 ## Contributing & Developer Notes
 Pull Requests, Bug Reports, and all Contributions are welcome! Please use the appropriate issue or pull request template when making a contribution.
 
 We make use of [the GitHub Discussions page](https://github.com/JacksonBurns/astartes/discussions) to go over potential features to add. Please feel free to stop by if you are looking for something to develop or have an idea for a useful feature!
 
 When submitting a PR, please mark your PR with the "PR Ready for Review" label when you are finished making changes so that the GitHub actions bots can work their magic!
```

### Comparing `astartes-1.0.0rc1/astartes/main.py` & `astartes-1.0.1/astartes/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 
 from astartes.samplers import (
     IMPLEMENTED_EXTRAPOLATION_SAMPLERS,
     IMPLEMENTED_INTERPOLATION_SAMPLERS,
 )
+from astartes.utils.convert_to_array import convert_to_array
 from astartes.utils.exceptions import InvalidConfigurationError
 from astartes.utils.sampler_factory import SamplerFactory
 from astartes.utils.warnings import ImperfectSplittingWarning, NormalizationWarning
 
 # define random seed
 DEFAULT_RANDOM_STATE = 42
 
@@ -40,14 +41,21 @@
         random_state (int, optional): The random seed used throughout astartes.
         hopts (dict, optional): Hyperparameters for the sampler used above. Defaults to {}.
         return_indices (bool, optional): True to return indices of train/test after values. Defaults to False.
 
     Returns:
         np.array: X, y, and labels train/val/test data, or indices.
     """
+    if type(X) is not np.ndarray:
+        X = convert_to_array(X, "X")
+    if y is not None and type(y) is not np.ndarray:
+        y = convert_to_array(y, "y")
+    if labels is not None and type(labels) is not np.ndarray:
+        labels = convert_to_array(labels, "labels")
+
     msg = ""
     if y is not None and len(y) != len(X):
         msg += "len(y)={:d} ".format(len(y))
     if labels is not None and len(labels) != len(X):
         msg += "len(labels)={:d} ".format(len(labels))
     if msg:
         raise InvalidConfigurationError(
@@ -59,30 +67,32 @@
     )
     hopts["random_state"] = (
         random_state if random_state is not None else DEFAULT_RANDOM_STATE
     )
     sampler_factory = SamplerFactory(sampler)
     sampler_instance = sampler_factory.get_sampler(X, y, labels, hopts)
 
-    if sampler in IMPLEMENTED_EXTRAPOLATION_SAMPLERS:
-        return _extrapolative_sampling(
+    if sampler in (*IMPLEMENTED_INTERPOLATION_SAMPLERS, "time_based"):
+        # time_based does extrapolation but does not support random_state
+        # because it always sorts in time order
+        return _interpolative_sampling(
             sampler_instance,
             test_size,
             val_size,
             train_size,
             return_indices,
-            random_state,
         )
     else:
-        return _interpolative_sampling(
+        return _extrapolative_sampling(
             sampler_instance,
             test_size,
             val_size,
             train_size,
             return_indices,
+            random_state,
         )
 
 
 def train_test_split(
     X: np.array,
     y: np.array = None,
     labels: np.array = None,
@@ -152,34 +162,32 @@
     n_test_samples = floor(len(sampler_instance.X) * test_size)
     n_val_samples = floor(len(sampler_instance.X) * val_size)
     # unlike interpolative, cannot calculate n_train_samples here
     # since it will vary based on cluster_lengths
 
     # largest clusters must go into largest set, but smaller ones can optionally
     # be shuffled
-    cluster_counter = None
-    if random_state is None:
-        cluster_counter = sampler_instance.get_sorted_cluster_counter()
-    else:
-        cluster_counter = sampler_instance.get_semi_sorted_cluster_counter(
-            max_shufflable_size=min(n_test_samples, n_val_samples)
-        )
+    cluster_counter = sampler_instance.get_sorted_cluster_counter(
+        max_shufflable_size=min(n_test_samples, n_val_samples)
+        if random_state is not None
+        else None
+    )
 
     test_idxs, val_idxs, train_idxs = (
         np.array([], dtype=int),
         np.array([], dtype=int),
         np.array([], dtype=int),
     )
     for cluster_idx, cluster_length in cluster_counter.items():
         # assemble test first, avoid overfilling
         if (len(test_idxs) + cluster_length) <= n_test_samples:
             test_idxs = np.append(
                 test_idxs, sampler_instance.get_sample_idxs(cluster_length)
             )
-        if (len(val_idxs) + cluster_length) <= n_val_samples:
+        elif (len(val_idxs) + cluster_length) <= n_val_samples:
             val_idxs = np.append(
                 val_idxs, sampler_instance.get_sample_idxs(cluster_length)
             )
         else:  # then balance goes into train
             train_idxs = np.append(
                 train_idxs, sampler_instance.get_sample_idxs(cluster_length)
             )
```

### Comparing `astartes-1.0.0rc1/astartes/molecules.py` & `astartes-1.0.1/astartes/molecules.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,21 @@
         from aimsim.chemical_datastructures import Molecule
         from aimsim.exceptions import LoadingError
 except ImportError:  # pragma: no cover
     raise MoleculesNotInstalledError(
         """To use molecule featurizer, install astartes with pip install astartes[molecules]."""
     )
 
+# at this point we have successfully verified that rdkit is installed, so we can do this:
+from rdkit.rdBase import SeedRandomNumberGenerator
 
 from astartes import train_test_split, train_val_test_split
+from astartes.main import DEFAULT_RANDOM_STATE
+
+SeedRandomNumberGenerator(DEFAULT_RANDOM_STATE)
 
 
 def train_val_test_split_molecules(
     molecules: np.array,
     y: np.array = None,
     labels: np.array = None,
     train_size: float = 0.8,
@@ -53,15 +58,18 @@
         fingerprint (str, optional): Molecular fingerprint to be used from AIMSim. Defaults to "morgan_fingerprint".
         fprints_hopts (dict, optional): Hyperparameters for AIMSim featurization. Defaults to {}.
         return_indices (bool, optional): True to return indices of train/test after the values. Defaults to False.
 
     Returns:
         np.array: X, y, and labels train/val/test data, or indices.
     """
-    X = _featurize(molecules, fingerprint, fprints_hopts)
+    if sampler == "scaffold":
+        X = molecules
+    else:
+        X = _featurize(molecules, fingerprint, fprints_hopts)
     return train_val_test_split(
         X,
         y=y,
         labels=labels,
         test_size=test_size,
         val_size=val_size,
         train_size=train_size,
@@ -100,15 +108,18 @@
         fprints_hopts (dict, optional): Hyperparameters for AIMSim featurization. Defaults to {}.
         return_indices (bool, optional): True to return indices of train/test after the values. Defaults to False.
 
     Returns:
         np.array: X, y, and labels train/test data, or indices.
     """
     # turn the smiles into an input X
-    X = _featurize(molecules, fingerprint, fprints_hopts)
+    if sampler == "scaffold":
+        X = molecules
+    else:
+        X = _featurize(molecules, fingerprint, fprints_hopts)
 
     # call train test split with this input
     return train_test_split(
         X,
         y=y,
         labels=labels,
         test_size=test_size,
```

### Comparing `astartes-1.0.0rc1/astartes/samplers/__init__.py` & `astartes-1.0.1/astartes/samplers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # abstract base classes
 from .abstract_sampler import AbstractSampler
 
 # implementations
-from .extrapolation import DBSCAN, KMeans, OptiSim, Scaffold, SphereExclusion
-from .interpolation import MTSD, SPXY, DOptimal, Duplex, KennardStone, Random
+from .extrapolation import DBSCAN, KMeans, OptiSim, Scaffold, SphereExclusion, TimeBased
+from .interpolation import MTSD, SPXY, KennardStone, Random
 
 IMPLEMENTED_INTERPOLATION_SAMPLERS = (
     "random",
-    # "doptimal",
-    # "duplex",
     "kennard_stone",
     # "mtsd",
     "spxy",
 )
 
 IMPLEMENTED_EXTRAPOLATION_SAMPLERS = (
     "dbscan",
     "scaffold",
     "kmeans",
     "optisim",
     "sphere_exclusion",
+    "time_based",
 )
 
 ALL_SAMPLERS = IMPLEMENTED_EXTRAPOLATION_SAMPLERS + IMPLEMENTED_INTERPOLATION_SAMPLERS
```

### Comparing `astartes-1.0.0rc1/astartes/samplers/extrapolation/dbscan.py` & `astartes-1.0.1/astartes/samplers/extrapolation/dbscan.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0rc1/astartes/samplers/extrapolation/kmeans.py` & `astartes-1.0.1/astartes/samplers/extrapolation/kmeans.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0rc1/astartes/samplers/extrapolation/optisim.py` & `astartes-1.0.1/astartes/samplers/extrapolation/optisim.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0rc1/astartes/samplers/extrapolation/scaffold.py` & `astartes-1.0.1/astartes/samplers/extrapolation/scaffold.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from astartes.samplers import AbstractSampler
 from astartes.utils.warnings import NoMatchingScaffold
 
 
 class Scaffold(AbstractSampler):
     def __init__(self, *args):
+        # ensure that X (i.e. args[0]) contains entries that are either a SMILES string or an RDKit Molecule
         if not isinstance(args[0][0], str) and not isinstance(
             args[0][0], Chem.rdchem.Mol
         ):
             msg = "Scaffold class requires input X to be an iterable of SMILES strings"
             raise TypeError(msg)
 
         super().__init__(*args)
@@ -69,51 +70,51 @@
             scaffold = self.generate_bemis_murcko_scaffold(
                 mol, self.get_config("include_chirality", False)
             )
             scaffolds[scaffold].add(i)
 
         return scaffolds
 
-    def str_to_mol(self, string, explicit_hydrogens=False):
+    def str_to_mol(self, string):
         """
         Converts an InChI or SMILES string to an RDKit molecule.
 
         Params:
             string: The InChI or SMILES string.
-            explicit_hydrogens: Whether to treat hydrogens explicitly.
 
         Returns:
             An RDKit molecule.
         """
         RDKIT_SMILES_PARSER_PARAMS = Chem.SmilesParserParams()
         if string.startswith("InChI"):
-            mol = Chem.MolFromInchi(string, removeHs=not explicit_hydrogens)
+            mol = Chem.MolFromInchi(string, removeHs=True)
         else:
             # Set params here so we don't remove hydrogens with atom mapping
-            RDKIT_SMILES_PARSER_PARAMS.removeHs = not explicit_hydrogens
+            RDKIT_SMILES_PARSER_PARAMS.removeHs = True
             mol = Chem.MolFromSmiles(string, RDKIT_SMILES_PARSER_PARAMS)
 
-        if explicit_hydrogens:
-            return Chem.AddHs(mol)
-        else:
-            return Chem.RemoveHs(mol)
+        # atom map numbers should not be present when creating scaffolds
+        for atom in mol.GetAtoms():
+            atom.SetAtomMapNum(0)
+
+        return mol
 
     def generate_bemis_murcko_scaffold(self, mol, include_chirality=False):
         """
         Compute the Bemis-Murcko scaffold for an RDKit molecule.
 
         Params:
             mol: A smiles string or an RDKit molecule.
             include_chirality: Whether to include chirality.
 
         Returns:
             Bemis-Murcko scaffold
         """
         mol = (
-            self.str_to_mol(mol, self.get_config("explicit_hydrogens", False))
+            self.str_to_mol(mol)
             if isinstance(mol, str)
             else mol
         )
         scaffold = MurckoScaffold.MurckoScaffoldSmiles(
             mol=mol, includeChirality=include_chirality
         )
```

### Comparing `astartes-1.0.0rc1/astartes/samplers/extrapolation/sphere_exclusion.py` & `astartes-1.0.1/astartes/samplers/extrapolation/sphere_exclusion.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0rc1/astartes/samplers/interpolation/random_split.py` & `astartes-1.0.1/astartes/samplers/interpolation/random_split.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0rc1/astartes/samplers/interpolation/spxy.py` & `astartes-1.0.1/astartes/samplers/interpolation/spxy.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0rc1/astartes/utils/exceptions.py` & `astartes-1.0.1/astartes/utils/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,7 +19,15 @@
 
 class SamplerNotImplementedError(RuntimeError):
     """Used when attempting to call a non-existent sampler."""
 
     def __init__(self, message=None):
         self.message = message
         super().__init__(message)
+
+
+class UncastableInputError(RuntimeError):
+    """Used when X, y, or labels cannot be cast to a np.array."""
+
+    def __init__(self, message=None):
+        self.message = message
+        super().__init__(message)
```

### Comparing `astartes-1.0.0rc1/astartes/utils/sampler_factory.py` & `astartes-1.0.1/astartes/utils/sampler_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     SPXY,
     KennardStone,
     KMeans,
     OptiSim,
     Random,
     Scaffold,
     SphereExclusion,
+    TimeBased,
 )
 from astartes.utils.exceptions import SamplerNotImplementedError
 
 
 class SamplerFactory:
     def __init__(self, sampler):
         """Initialize SamplerFactory and copy a lowercased 'sampler' into an attribute.
@@ -50,14 +51,16 @@
             sampler_class = SphereExclusion
         elif self.sampler == "optisim":
             sampler_class = OptiSim
         elif self.sampler == "spxy":
             sampler_class = SPXY
         elif self.sampler == "scaffold":
             sampler_class = Scaffold
+        elif self.sampler == 'time_based':
+            sampler_class = TimeBased
         else:
             possiblity = get_close_matches(
                 self.sampler,
                 ALL_SAMPLERS,
                 n=1,
             )
             addendum = (
```

### Comparing `astartes-1.0.0rc1/astartes/utils/warnings.py` & `astartes-1.0.1/astartes/utils/warnings.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,22 @@
     """Used when a requested split does not add to 1."""
 
     def __init__(self, message=None):
         self.message = message
         super().__init__(message)
 
 
+class ConversionWarning(RuntimeWarning):
+    """Used when passed data is not a numpy array."""
+
+    def __init__(self, message=None):
+        self.message = message
+        super().__init__(message)
+
+
 class NoMatchingScaffold(Warning):
     """
     Used when an RDKit molecule does not match any
     Bemis-Murcko scaffold and returns an empty string.
     """
 
     def __init__(self, message=None):
```

### Comparing `astartes-1.0.0rc1/astartes.egg-info/PKG-INFO` & `astartes-1.0.1/astartes.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: astartes
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays
 Author-email: Jackson Burns <jwburns@mit.edu>, Himaghna Bhattacharjee <himaghna@udel.edu>, Kevin Spiekermann <kspieker@mit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/astartes
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: molecules
 Provides-Extra: dev
+Provides-Extra: demos
 License-File: LICENSE
 
 <h1 align="center">astartes</h1> 
 <h3 align="center">Train:Validation:Test Algorithmic Sampling for Molecules and Arbitrary Arrays</h3>
 
 <p align="center">  
-  <img alt="astarteslogo" src="https://github.com/JacksonBurns/astartes/blob/main/astartes_logo.png">
+  <img alt="astarteslogo" src="https://raw.githubusercontent.com/JacksonBurns/astartes/main/astartes_logo.png">
 </p> 
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/JacksonBurns/astartes?style=social">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/astartes">
+  <img alt="PyPI - Total Downloads" src="https://static.pepy.tech/personalized-badge/astartes?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Lifetime%20Downloads">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/astartes">
   <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/astartes?style=plastic">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/JacksonBurns/astartes">
   <img alt="Test Status" src="https://github.com/JacksonBurns/astartes/actions/workflows/run_tests.yml/badge.svg?branch=main&event=schedule">
+  <img alt="Reproduce Paper" src="https://github.com/JacksonBurns/astartes/actions/workflows/reproduce_paper.yml/badge.svg?branch=main&event=schedule">
 </p>
 
 ## Installing `astartes`
 We recommend installing `astartes` within a virtual environment, using either `venv` or `conda` (or other tools) to simplify dependency management. Python versions 3.7, 3.8, 3.9, 3.10, and 3.11 are supported on all platforms.
 
 `astartes` is available on `PyPI` and can be installed using `pip`:
 
@@ -40,47 +42,53 @@
  - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer dependencies and may be more readily compatible in environments with existing workflows).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install "astartes[molecules]"`)
 
 ## Using `astartes`
 `astartes` is designed as a drop-in replacement for `sklearn`'s `train_test_split` function. To switch to `astartes`, change `from sklearn.model_selection import train_test_split` to `from astartes import train_test_split`.
 
-By default, `astartes` will use a random splitting approach identical to that which is implemented in `sklearn`, and a variety of deterministic sampling approaches can be used by specifying one additional argument ot the function:
+By default, `astartes` will split data randomly. Additionally, a variety of algorithmic sampling approaches can be used by specifying the `sampler` argument to the function:
 
 ```python
 X_train, X_test, y_train, y_test = train_test_split(
-  X,
+  X,  # preferably numpy arrays, but astartes will cast it for you
   y,
   sampler = 'kennard_stone',  # any of the supported samplers
 )
 ```
 
+### Paper
+For a comprehensive walkthrough of the theory and implementation of `astartes`, follow [this link](https://github.com/JacksonBurns/astartes/raw/joss-paper/Burns-Spiekermann-Bhattacharjee_astartes.pdf) to read the companion paper.
+
 ### Example Notebooks
 
 Click the badges in the table below to be taken to a live, interactive demo of `astartes`:
 
 | Demo | Link |
 |:---:|---|
-| Using `train_val_test_split` with the `sklearn` example datasets | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Ftrain_val_test_split_example.ipynb) |
-| Cheminformatics sample set partitioning with `astartes` | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2FRDB7_barrier_prediction_example.ipynb) |
+| Using `train_val_test_split` with the `sklearn` example datasets | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Ftrain_val_test_split_sklearn_example%2Ftrain_val_test_split_example.ipynb) |
+| Comparing Sampling Algorithms with Fast Food | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Fsplit_comparisons%2Fsplit_comparisons.ipynb) |
+| Cheminformatics sample set partitioning with `astartes` | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Fbarrier_prediction_with_RDB7%2FRDB7_barrier_prediction_example.ipynb) |
+| Comparing partitioning approaches for alkanes | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Fmlpds_2023_astartes_demo%2Fmlpds_2023_demo.ipynb) |
 
 ### Rational Splitting Algorithms
-While much machine learning is done with a random choice between training/test/validation data, an alternative is the use of so-called "rational" splitting algorithms. These approaches use some similarity-based algorithm to divide data into sets. Some of these algorithms include Kennard-Stone, minimal test set dissimilarity, and sphere exclusion algorithms [as discussed by Tropsha et. al](https://pubs.acs.org/doi/pdf/10.1021/ci300338w) as well as the OptiSim as discussed in [Applied Chemoinformatics: Achievements and Future Opportunities](https://www.wiley.com/en-us/Applied+Chemoinformatics%3A+Achievements+and+Future+Opportunities-p-9783527806546). Some clustering-based splitting techniques have also been introduced, such as [DBSCAN](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1016.890&rep=rep1&type=pdf).
+While much machine learning is done with a random choice between training/validation/test data, an alternative is the use of so-called "rational" splitting algorithms. These approaches use some similarity-based algorithm to divide data into sets. Some of these algorithms include Kennard-Stone, minimal test set dissimilarity, and sphere exclusion algorithms [as discussed by Tropsha et. al](https://pubs.acs.org/doi/pdf/10.1021/ci300338w) as well as the OptiSim as discussed in [Applied Chemoinformatics: Achievements and Future Opportunities](https://www.wiley.com/en-us/Applied+Chemoinformatics%3A+Achievements+and+Future+Opportunities-p-9783527806546). Some clustering-based splitting techniques have also been incorporated, such as [DBSCAN](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1016.890&rep=rep1&type=pdf).
 
-There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-sample data, effectively asking a 'harder question' than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`, as well as the hyperparameters that each algorithm accepts (which are passed in with `hopts`) and a helpful reference for understanding how the hyperparameters work. Note that `random_state` is defined as a keyword argument in `train_test_split` itself, even though these algorithms will use the `random_state` in their own work. Do not provide a `random_state` in the `hopts` dictionary - it will be overwritten by the `random_state` you provide for `train_test_split` (or the default if none is provided).
+There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-sample data, which creates a more challenging task than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`, as well as the hyperparameters that each algorithm accepts (which are passed in with `hopts`) and a helpful reference for understanding how the hyperparameters work. Note that `random_state` is defined as a keyword argument in `train_test_split` itself, even though these algorithms will use the `random_state` in their own work. Do not provide a `random_state` in the `hopts` dictionary - it will be overwritten by the `random_state` you provide for `train_test_split` (or the default if none is provided).
 
 #### Implemented Sampling Algorithms
 
 | Sampler Name | Usage String | Type | Hyperparameters | Reference | Notes |
 |:---:|---|---|---|---|---|
 | Random | 'random' | Interpolative | `shuffle` | [`sklearn train_test_split`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) | This sampler is a direct passthrough to `sklearn`'s `train_test_split`, though it does not currently reproduce splits identically. |
-| Kennard-Stone | 'kennard_stone' | Interpolative | _none_ | [yu9824's `kennard_stone`](https://github.com/yu9824/kennard_stone) | Fully deterministic, no hyperparameters accepted. |
-| Sample set Partitioning based on join X-Y distances (SPXY) | 'spxy' | Interpolative | `distance_metric` | Saldhana et. al [original paper](https://www.sciencedirect.com/science/article/abs/pii/S003991400500192X) | Extension of Kennard Stone that also includes the response when sampling distances. |
-| Scaffold | 'scaffold' | Extrapolative | `explicit_hydrogens`, `include_chirality` | [Bemis-Murcko Scaffold](https://pubs.acs.org/doi/full/10.1021/jm9602928) as implemented in RDKit | This sampler requires SMILES strings as input (use the `molecules` subpackage) |
+| Kennard-Stone | 'kennard_stone' | Interpolative | `metric` | [Kennard & Stone](https://www.tandfonline.com/doi/abs/10.1080/00401706.1969.10490666) | Euclidian distance is used by default, as described in the original paper. |
+| Sample set Partitioning based on joint X-Y distances (SPXY) | 'spxy' | Interpolative | `distance_metric` | Saldhana et. al [original paper](https://www.sciencedirect.com/science/article/abs/pii/S003991400500192X) | Extension of Kennard Stone that also includes the response when sampling distances. |
+| Scaffold | 'scaffold' | Extrapolative | `include_chirality` | [Bemis-Murcko Scaffold](https://pubs.acs.org/doi/full/10.1021/jm9602928) as implemented in RDKit | This sampler requires SMILES strings as input (use the `molecules` subpackage) |
 | Sphere Exclusion | 'sphere_exclusion' | Extrapolative | `metric`, `distance_cutoff` | _custom implementation_ | Variation on Sphere Exclusion for arbitrary-valued vectors. |
+| Time Based | 'time_based' | Extrapolative | _none_ | [Chen et al.](https://pubs.acs.org/doi/full/10.1021/ci200615h), [Sheridan, R. P](https://pubs.acs.org/doi/full/10.1021/ci400084k), [Feinberg et al.](https://pubs.acs.org/doi/full/10.1021/acs.jmedchem.9b02187), [Struble et al.](https://pubs.rsc.org/en/content/articlehtml/2020/re/d0re00071j)  | This sampler requires `labels` to be an iterable of either date or datetime objects. |
 | Optimizable K-Dissimilarity Selection (OptiSim) | 'optisim' | Extrapolative | `n_clusters`, `max_subsample_size`, `distance_cutoff` | _custom implementation_ | Variation on [OptiSim](https://pubs.acs.org/doi/10.1021/ci025662h) for arbitrary-valued vectors. |
 | K-Means | 'kmeans' | Extrapolative | `n_clusters`, `n_init` | [`sklearn KMeans`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) | Passthrough to `sklearn`'s `KMeans`. |
 | Density-Based Spatial Clustering of Applications with Noise (DBSCAN) | 'dbscan' | Extrapolative | `eps`, `min_samples`, `algorithm`, `metric`, `leaf_size` | [`sklearn DBSCAN`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html) | Passthrough to `sklearn`'s `DBSCAN`. |
 | Minimum Test Set Dissimilarity (MTSD) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 | Restricted Boltzmann Machine (RBM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 | Kohonen Self-Organizing Map (SOM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 | SPlit Method | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
@@ -114,17 +122,38 @@
 )
 ```
 
 To see a complete example of using `train_test_split_molecules` with actual chemical data, take a look in the `examples` directory.
 
 Configuration options for the featurization scheme can be found in the documentation for [`AIMSim`](https://vlachosgroup.github.io/AIMSim/README.html#currently-implemented-fingerprints) though most of the critical configuration options are shown above.
 
+### Reproducibility
+`astartes` aims to be completely reproducible across different platforms, Python versions, and dependency configurations - any version of `astartes` v1.x should result in the _exact_ same splits, always.
+To that end, the default behavior of `astartes` is to use `42` as the random seed and _always_ set it.
+Running `astartes` with the default settings will always produce the exact same results.
+We have verified this behavior on Debian Ubuntu, Windows, and Intel Macs from Python versions 3.7 through 3.11 (with appropriate dependencies for each version).
+We are limited in our ability to test on M1 Macs, but from our limited manual testing we achieve perfect reproducbility in all cases _except occasionally_ with `KMeans` on Apple silicon. It has produced _slightly_ different results between platforms regardless of `random_state`, with up to two clusters being assigned differently resulting in data splits which are >99% identical. `astartes` is still consistent between runs on the same platform in all cases.
+
 ## Online Documentation
 [The online documentation](https://JacksonBurns.github.io/astartes/) contains everything you see in this README with an additional tutorial for [moving from `train_test_split` in `sklearn` to `astartes`](https://jacksonburns.github.io/astartes/sklearn_to_astartes.html).
 
+## How to Cite
+If you use `astartes` in your work please use the below citation or the "Cite this repository" button on GitHub:
+> **BibTeX**
+> @software{Burns_astartes,
+>   author = {Burns, Jackson and Spiekermann, Kevin and Bhattacharjee, Himaghna and Vlachos, Dionisios and Green, William},
+>   license = {MIT},
+>   title = {{astartes}},
+>   url = {https://github.com/JacksonBurns/astartes}
+> }
+
+> **APA**
+> Burns, J., Spiekermann, K., Bhattacharjee, H., Vlachos, D., & Green, W. astartes [Computer software]. https://github.com/JacksonBurns/astartes
+
+
 ## Contributing & Developer Notes
 Pull Requests, Bug Reports, and all Contributions are welcome! Please use the appropriate issue or pull request template when making a contribution.
 
 We make use of [the GitHub Discussions page](https://github.com/JacksonBurns/astartes/discussions) to go over potential features to add. Please feel free to stop by if you are looking for something to develop or have an idea for a useful feature!
 
 When submitting a PR, please mark your PR with the "PR Ready for Review" label when you are finished making changes so that the GitHub actions bots can work their magic!
```

### Comparing `astartes-1.0.0rc1/astartes.egg-info/SOURCES.txt` & `astartes-1.0.1/astartes.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 astartes/samplers/abstract_sampler.py
 astartes/samplers/extrapolation/__init__.py
 astartes/samplers/extrapolation/dbscan.py
 astartes/samplers/extrapolation/kmeans.py
 astartes/samplers/extrapolation/optisim.py
 astartes/samplers/extrapolation/scaffold.py
 astartes/samplers/extrapolation/sphere_exclusion.py
+astartes/samplers/extrapolation/time_based.py
 astartes/samplers/interpolation/__init__.py
-astartes/samplers/interpolation/doptimal.py
-astartes/samplers/interpolation/duplex.py
 astartes/samplers/interpolation/kennardstone.py
 astartes/samplers/interpolation/mtsd.py
 astartes/samplers/interpolation/random_split.py
 astartes/samplers/interpolation/spxy.py
 astartes/utils/__init__.py
+astartes/utils/convert_to_array.py
 astartes/utils/exceptions.py
 astartes/utils/sampler_factory.py
-astartes/utils/warnings.py
-test/test_astartes.py
-test/test_molecules.py
+astartes/utils/warnings.py
```

### Comparing `astartes-1.0.0rc1/pyproject.toml` & `astartes-1.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astartes"
-version = "1.0.0rc1"
+version = "1.0.1"
 authors = [
     { name = "Jackson Burns", email = "jwburns@mit.edu" },
     { name = "Himaghna Bhattacharjee", email = "himaghna@udel.edu" },
     { name = "Kevin Spiekermann", email = "kspieker@mit.edu" },
 ]
 license = { text = "MIT" }
 description = "Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays"
@@ -17,19 +17,20 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 urls = { Homepage = "https://github.com/JacksonBurns/astartes" }
 requires-python = ">=3.7"
-dependencies = ["kennard_stone", "scikit_learn", "numpy", "scipy"]
+dependencies = ["scikit_learn", "numpy", "scipy"]
 
 [project.optional-dependencies]
 molecules = ["aimsim"]
 dev = ["black", "isort", "pytest"]
+demos = ["plotly", "tabulate", "py2opsin", "kaleido"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [tool.isort]
 profile = "black"
```

