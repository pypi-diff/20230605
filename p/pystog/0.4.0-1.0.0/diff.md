# Comparing `tmp/pystog-0.4.0.tar.gz` & `tmp/pystog-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystog-0.4.0.tar", last modified: Sun Jun  4 22:53:01 2023, max compression
+gzip compressed data, was "dist/pystog-1.0.0.tar", last modified: Wed Dec 30 16:48:17 2020, max compression
```

## Comparing `pystog-0.4.0.tar` & `pystog-1.0.0.tar`

### file list

```diff
@@ -1,47 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:53:01.000000 pystog-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-04 22:49:11.000000 pystog-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-04 22:49:11.000000 pystog-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-04 22:53:01.000000 pystog-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-06-04 22:49:11.000000 pystog-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:53:01.000000 pystog-0.4.0/pystog/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-04 22:49:11.000000 pystog-0.4.0/pystog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-04 22:53:01.000000 pystog-0.4.0/pystog/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-06-04 22:49:11.000000 pystog-0.4.0/pystog/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-06-04 22:49:11.000000 pystog-0.4.0/pystog/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20994 2023-06-04 22:49:11.000000 pystog-0.4.0/pystog/fourier_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-04 22:49:11.000000 pystog-0.4.0/pystog/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-04 22:49:11.000000 pystog-0.4.0/pystog/pre_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    53289 2023-06-04 22:49:11.000000 pystog-0.4.0/pystog/stog.py
--rw-r--r--   0 runner    (1001) docker     (123)    25383 2023-06-04 22:49:11.000000 pystog-0.4.0/pystog/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-04 22:49:11.000000 pystog-0.4.0/pystog/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:53:01.000000 pystog-0.4.0/pystog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-04 22:53:01.000000 pystog-0.4.0/pystog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-04 22:53:01.000000 pystog-0.4.0/pystog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:53:01.000000 pystog-0.4.0/pystog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-04 22:53:01.000000 pystog-0.4.0/pystog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 22:53:01.000000 pystog-0.4.0/pystog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 22:53:01.000000 pystog-0.4.0/pystog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-04 22:49:11.000000 pystog-0.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-04 22:49:11.000000 pystog-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-04 22:53:01.000000 pystog-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-04 22:49:11.000000 pystog-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:53:01.000000 pystog-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/create_test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15256 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:53:01.000000 pystog-0.4.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34234 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_data/argon.gr
--rw-r--r--   0 runner    (1001) docker     (123)    48445 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_data/argon.real_space.dat
--rw-r--r--   0 runner    (1001) docker     (123)    81850 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_data/argon.reciprocal_space.dat
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_data/nickel.gr
--rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_data/nickel.real_space.dat
--rw-r--r--   0 runner    (1001) docker     (123)    88077 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_data/nickel.reciprocal_space.dat
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_fourier_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    45909 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_stog.py
--rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-04 22:49:11.000000 pystog-0.4.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68632 2023-06-04 22:49:11.000000 pystog-0.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 16:48:17.000000 pystog-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (116)       75 2020-12-30 16:47:19.000000 pystog-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      624 2020-12-30 16:48:17.000000 pystog-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5298 2020-12-30 16:47:19.000000 pystog-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 16:48:17.000000 pystog-1.0.0/pystog/
+-rw-r--r--   0 runner    (1001) docker     (116)      319 2020-12-30 16:47:19.000000 pystog-1.0.0/pystog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      497 2020-12-30 16:48:17.000000 pystog-1.0.0/pystog/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6344 2020-12-30 16:47:19.000000 pystog-1.0.0/pystog/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12508 2020-12-30 16:47:19.000000 pystog-1.0.0/pystog/converter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20950 2020-12-30 16:47:19.000000 pystog-1.0.0/pystog/fourier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4002 2020-12-30 16:47:19.000000 pystog-1.0.0/pystog/io.py
+-rw-r--r--   0 runner    (1001) docker     (116)    55789 2020-12-30 16:47:19.000000 pystog-1.0.0/pystog/stog.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25193 2020-12-30 16:47:19.000000 pystog-1.0.0/pystog/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (116)      795 2020-12-30 16:47:19.000000 pystog-1.0.0/pystog/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 16:48:17.000000 pystog-1.0.0/pystog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      624 2020-12-30 16:48:17.000000 pystog-1.0.0/pystog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      871 2020-12-30 16:48:17.000000 pystog-1.0.0/pystog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-30 16:48:17.000000 pystog-1.0.0/pystog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       99 2020-12-30 16:48:17.000000 pystog-1.0.0/pystog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       44 2020-12-30 16:48:17.000000 pystog-1.0.0/pystog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2020-12-30 16:48:17.000000 pystog-1.0.0/pystog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2020-12-30 16:47:19.000000 pystog-1.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       44 2020-12-30 16:47:19.000000 pystog-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      262 2020-12-30 16:48:17.000000 pystog-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2138 2020-12-30 16:47:19.000000 pystog-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 16:48:17.000000 pystog-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      786 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/create_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6453 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/materials.py
+-rw-r--r--   0 runner    (1001) docker     (116)      698 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/runner.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14394 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 16:48:17.000000 pystog-1.0.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    34234 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_data/argon.gr
+-rw-r--r--   0 runner    (1001) docker     (116)    48445 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_data/argon.real_space.dat
+-rw-r--r--   0 runner    (1001) docker     (116)    81850 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_data/argon.reciprocal_space.dat
+-rw-r--r--   0 runner    (1001) docker     (116)    12231 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_data/nickel.gr
+-rw-r--r--   0 runner    (1001) docker     (116)    18895 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_data/nickel.real_space.dat
+-rw-r--r--   0 runner    (1001) docker     (116)    88077 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_data/nickel.reciprocal_space.dat
+-rw-r--r--   0 runner    (1001) docker     (116)     8478 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_fourier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    44119 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_stog.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17881 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4383 2020-12-30 16:47:19.000000 pystog-1.0.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    68632 2020-12-30 16:47:19.000000 pystog-1.0.0/versioneer.py
```

### Comparing `pystog-0.4.0/PKG-INFO` & `pystog-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: pystog
-Version: 0.4.0
+Version: 1.0.0
 Summary: Manipulate total scattering functions
 Home-page: https://github.com/neutrons/pystog
 Author: Marshall McDonnell (marshallmcdonnell),Mathieu Doucet (mdoucet),Ross Whitfield (rosswhitfield),Pete Peterson (peterfpeterson),Yuanpeng Zhang (Kvieta1990)
 Author-email: mcdonnellmt@ornl.gov
 License: GPL License (version 3)
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
```

### Comparing `pystog-0.4.0/README.md` & `pystog-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,133 +3,84 @@
 
 | Health | Release | Other  |
 |--------|---------|------------|
 | [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fneutrons%2Fpystog%2Fbadge%3Fref%3Dmaster&style=plastic)](https://actions-badge.atrox.dev/neutrons/pystog/goto?ref=master) | [![PyPI version](https://badge.fury.io/py/pystog.svg)](https://badge.fury.io/py/pystog) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/neutrons/pystog/master?filepath=tutorials) |
 | [![codecov](https://codecov.io/gh/neutrons/pystog/branch/master/graph/badge.svg)](https://codecov.io/gh/neutrons/pystog) | [![Anaconda-Server Badge](https://anaconda.org/neutrons/pystog/badges/version.svg)](https://anaconda.org/neutrons/pystog)| [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)  |
 |[![Documentation Status](https://readthedocs.org/projects/pystog/badge/?version=latest)](https://pystog.readthedocs.io/en/latest/?badge=latest) | [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) |  |
 
-From total scattering functions, we have reciprocal-space structure factors and real-space pair distribution functions that are related via a Fourier transform.
-PyStoG is a package that allows for:
+From total scattering functions, we have reciprocal-space structure factors and real-space pair distribution functions that are related via a Fourier transform. PyStoG is a package that allows for:
 1. Converting between the various functions used by different "communities" (ie researchers who study crystalline versus amorphous or glass materials). Conversions are for either real-space or reciprocal-space.
 2. Perform the transform between the different available functions of choice
 3. Fourier filter to remove spurious artificats in the data (ie aphysical, sub-angstrom low-r peaks in G(r) from experiments)
 
-![alt text](https://raw.githubusercontent.com/neutrons/pystog/master/images/sofq_to_gofr.png)
+![alt text](https://raw.githubusercontent.com/marshallmcdonnell/mantid_total_scattering/master/images/sofq_to_gofr.png)
 
 
-The name **PyStoG** comes from the fact that this is a _Pythonized_ version of **StoG**, a ~30 year old Fortran program that is part of the [RMCProfile software suite](http://www.rmcprofile.org/Main_Page).
-**StoG** means **"S(Q) to G(r)"** for the fact that it takes recirpocal-space S(Q) patterns from files and transforms them into a single G(r) pattern.
-The original *StoG* program has been developed, in reverse chronological order, by:
+The name **PyStoG** comes from the fact that this is a _Pythonized_ version of **StoG**, a ~30 year old Fortran program that is part of the [RMCProfile software suite](http://www.rmcprofile.org/Main_Page). **StoG** means **"S(Q) to G(r)"** for the fact that it takes recirpocal-space S(Q) patterns from files and transforms them into a single G(r) pattern. The original *StoG* program has been developed, in reverse chronological order, by:
 
  * Matthew Tucker and Martin Dove (~2009)
  * Spencer Howells (~1989)
  * Jack Carpenter (prior to 1989)
  
  A current state of the **StoG** program is kept in the `fortran` directory of this package.
 
-This project was initially just a "sandbox" for taking the capabilities of **StoG** and migrating them over to the [Mantid Framework](https://github.com/mantidproject/mantid).
-Yet, with more and more use cases, **PyStoG** was further developed as the stand-alone project it is now.
-Yet, migration to the Mantid Framework is still a goal since it feeds into the [ADDIE project](https://github.com/neutrons/addie)
+This project was initially just a "sandbox" for taking the capabilities of **StoG** and migrating them over to the [Mantid Framework](https://github.com/mantidproject/mantid). Yet, with more and more use cases, **PyStoG** was further developed as the stand-alone project it is now. Yet, migration to the Mantid Framework is still a goal since it feeds into the [ADDIE project](https://github.com/neutrons/addie)
 
 ## Installation
 
-Installation is available via [`pip`](https://pip.pypa.io/en/stable/):
-`pip install pystog`
+Installation is available via `pip`. 
 
-And [conda](https://docs.conda.io/en/latest/):
-`conda install -c neutrons pystog`
+```bash 
+pip install pystog
+```
+
+or for a local install
+```bash
+pip install pystog --user #locally installed in $HOME/.local
+```
+For a development environment, you can use [`virtualenv`](https://virtualenv.pypa.io/en/latest/) to setup an isolated environemnt, namely `ENV`:
+
+```bash
+python -m virtualenv /path/to/ENV
+source /path/to/ENV/bin/activate
+pip install pystog
+```
+
+Also, [`direnv`](https://github.com/direnv/direnv) is a useful and recommended way to manage the virtual environment. You can simply use an `.envrc` file which contains:
+
+`layout python3`
+
+Then, once inside the development directory, just install via `pip` as described above.
 
 ## Getting started
 
 Once installed, you can access the packages classes that perform the function manipulation. 
 
 ```python
 import pystog
 from pystog import Converter
 from pystog import Transformer
 from pystog import FourierFilter
 from pystog import StoG
 ```
 ** WARNING: Testing of the CLI is still ongoing**
 
-Also, there is a beta-version of a python script in the package that can be run on JSON input files and operates similarly to the original **StoG** program.
-This is `python cli` and can be used as follows:
+Also, there is a beta-version of a python script in the package that can be run on JSON input files and operates similarly to the original **StoG** program, only with extra `matplotlib` visualization of the output. This is `python cli` and can be used as follows:
 
 ```bash
 pystog_cli --json <input json>
 ```
-An example JSON can be found [here](https://github.com/neutrons/pystog/blob/master/data/examples/argon_pystog.json)
+An example JSON can be found [here](https://github.com/marshallmcdonnell/pystog/blob/master/data/examples/argon_pystog.json)
 
 ### Documentation
 The official documentation is hosted on readthedocs.org: [https://pystog.readthedocs.io/en/latest/](https://pystog.readthedocs.io/en/latest/)
 
 Also, a useful example reference is the [PDFFourierTransform](http://docs.mantidproject.org/nightly/algorithms/PDFFourierTransform-v1.html) algorithm in the Mantid Framework that has similar yet limited capabilities.
 
-Finally, tutorials in the form of Jupyter Notebooks can be launched via Binder by clicking the badge here [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/neutrons/pystog/master?filepath=tutorials) or at the top of the page.
-
-## Development
-
-The following are ways to setup the virtual environment, lint and test the package.
+Finally, tutorials in the form of Jupyter Notebooks can be launched via Binder by clicking the badge here [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/marshallmcdonnell/pystog/master?filepath=tutorials) or at the top of the page.
 
-### Virtual environment setup
+## Running the tests
+From the parent directory of the module, run:
 
-#### Using pipenv (recommended)
-With [pipenv](https://pipenv.pypa.io/en/latest/) installed, run the following:
 ```bash
-pipenv install --dev .
+python setup.py test
 ```
-
-#### Using virtualenv
-You can use [`virtualenv`](https://virtualenv.pypa.io/en/latest/) to setup an environment, here named `ENV`:
-
-```bash
-python -m virtualenv /path/to/ENV
-source /path/to/ENV/bin/activate
-pip install pystog
-```
-
-#### Using direnv
-Also, [`direnv`](https://github.com/direnv/direnv) is a useful and recommended way to manage the virtual environment.
-You can simply use an `.envrc` file which contains:
-
-`layout python3`
-
-Then, once inside the development directory, just install via `pip` as described above.
-
-### Testing
-[pytest](https://docs.pytest.org/en/latest/) is used to write the test suite.
-[Tox](https://tox.readthedocs.io/en/latest/) is the general tool for running both linting and testing (single and multiple python version testing).
-[pyenv](https://github.com/pyenv/pyenv) is the recommended tool for python version management.
-From the parent directory of the module, run:
-
-`pytest`
-
-Using pipenv:
-`pipenv run pytest`
-
-Using tox for a single python version,
-where `py<XY>` is one of [py36, py37, py38, py39]:
-`tox -e py<XY>`
-
-or with pipenv:
-`pipenv run tox -e py<XY>`
-
-Using tox for all stages of testing (all python versions and linting), just run:
-`tox`
-NOTE: You must have the version of python installed to run a test suite against that verion via tox.
-Recommended way to install python versions is `pyenv`
-
-### Linting
-[Flake8](https://flake8.pycqa.org/en/latest/) is used for style guide enforcement (i.e. linting):
-
-From the parent directory of the module, run:
-
-`flake8 .`
-
-Using pipenv and flake8:
-`pipenv run flake8 .`
-
-Using tox
-`tox -e lint`
-
-Using pipenv and tox:
-`pipenv run tox -e lint`
```

### Comparing `pystog-0.4.0/pystog/converter.py` & `pystog-1.0.0/pystog/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 Converter
 ==========
 
 This module defines the Converter class
 that converts functions in the same space
 """
 
+from __future__ import (absolute_import, division, print_function)
 import numpy as np
 
 
 class Converter:
-    """
-    The Converter class is used to convert between
+    """The Converter class is used to convert between
     either different reciprocal space functions or
     different real space functions
 
     :examples:
 
     >>> import numpy
     >>> from pystog import Converter
@@ -38,16 +38,15 @@
         out = np.zeros_like(numerator)
         out[mask] = numerator[mask] / denominator[mask]
         return out
 
     # Reciprocal Space Conversions
 
     def F_to_S(self, q, fq, dfq=None, **kwargs):
-        """
-        Converts from :math:`Q[S(Q)-1]` to :math:`S(Q)`
+        """Converts from :math:`Q[S(Q)-1]` to :math:`S(Q)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq: :math:`Q[S(Q)-1]` vector
         :type fq: numpy.array or list
         :param dfq: uncertainty vector
         :type dfq: numpy.array or list
@@ -56,16 +55,15 @@
         :rtype: (numpy.array, numpy.array)
         """
         if dfq is None:
             dfq = np.zeros_like(fq)
         return (self._safe_divide(fq, q) + 1., self._safe_divide(dfq, q))
 
     def F_to_FK(self, q, fq, dfq=None, **kwargs):
-        """
-        Converts from :math:`Q[S(Q)-1]` to :math:`F(Q)`
+        """Converts from :math:`Q[S(Q)-1]` to :math:`F(Q)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq: :math:`Q[S(Q)-1]` vector
         :type fq: numpy.array or list
         :param dfq: uncertainty vector
         :type dfq: numpy.array or list
@@ -75,17 +73,15 @@
         """
         if dfq is None:
             dfq = np.zeros_like(fq)
         return (kwargs['<b_coh>^2'] * self._safe_divide(fq, q),
                 kwargs['<b_coh>^2'] * self._safe_divide(dfq, q))
 
     def F_to_DCS(self, q, fq, dfq=None, **kwargs):
-        """
-        Converts from :math:`Q[S(Q)-1]` to
-        :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
+        """Converts from :math:`Q[S(Q)-1]` to :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq: :math:`Q[S(Q)-1]` vector
         :type fq: numpy.array or list
         :param dfq: uncertainty vector
         :type dfq: numpy.array or list
@@ -95,16 +91,15 @@
         :rtype: (numpy.array, numpy.array)
         """
         fq, dfq = self.F_to_FK(q, fq, dfq, **kwargs)
         return self.FK_to_DCS(q, fq, dfq, **kwargs)
 
     # S(Q)
     def S_to_F(self, q, sq, dsq=None, **kwargs):
-        """
-        Convert :math:`S(Q)` to :math:`Q[S(Q)-1]`
+        """Convert :math:`S(Q)` to :math:`Q[S(Q)-1]`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param sq: :math:`S(Q)` vector
         :type sq: numpy.array or list
         :param dfq: uncertainty vector
         :type dfq: numpy.array or list
@@ -115,16 +110,15 @@
         :rtype: (numpy.array, numpy.array)
         """
         if dsq is None:
             dsq = np.zeros_like(sq)
         return (q * (sq - 1.), q * dsq)
 
     def S_to_FK(self, q, sq, dsq=None, **kwargs):
-        """
-        Convert :math:`S(Q)` to :math:`F(Q)`
+        """Convert :math:`S(Q)` to :math:`F(Q)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param sq: :math:`S(Q)` vector
         :type sq: numpy.array or list
         :param dsq: uncertainty vector
         :type dsq: numpy.array or list
@@ -132,16 +126,15 @@
         :return: (:math:`F(Q)` vector, uncertainty vector)
         :rtype: (numpy.array, numpy.array)
         """
         fq, dfq = self.S_to_F(q, sq, dsq)
         return self.F_to_FK(q, fq, dfq, **kwargs)
 
     def S_to_DCS(self, q, sq, dsq=None, **kwargs):
-        """
-        Convert :math:`S(Q)` to :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
+        """Convert :math:`S(Q)` to :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param sq: :math:`S(Q)` vector
         :type sq: numpy.array or list
         :param dsq: uncertainty vector
         :type dsq: numpy.array or list
@@ -151,16 +144,15 @@
         :rtype: (numpy.array, numpy.array)
         """
         fq, dfq = self.S_to_FK(q, sq, dsq, **kwargs)
         return self.FK_to_DCS(q, fq, dfq, **kwargs)
 
     # Keen's F(Q)
     def FK_to_F(self, q, fq_keen, dfq_keen=None, **kwargs):
-        """
-        Convert :math:`F(Q)` to :math:`Q[S(Q)-1]`
+        """Convert :math:`F(Q)` to :math:`Q[S(Q)-1]`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq_keen: :math:`F(Q)` vector
         :type fq_keen: numpy.array or list
         :param dfq_keen: uncertainty vector
         :type dfq_keen: numpy.array or list
@@ -170,16 +162,15 @@
         """
         if dfq_keen is None:
             dfq_keen = np.zeros_like(fq_keen)
         return (q * fq_keen / kwargs['<b_coh>^2'],
                 q * dfq_keen / kwargs['<b_coh>^2'])
 
     def FK_to_S(self, q, fq_keen, dfq_keen=None, **kwargs):
-        """
-        Convert :math:`F(Q)` to :math:`S(Q)`
+        """Convert :math:`F(Q)` to :math:`S(Q)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq_keen: :math:`F(Q)` vector
         :type fq_keen: numpy.array or list
         :param dfq_keen: uncertainty vector
         :type dfq_keen: numpy.array or list
@@ -187,16 +178,15 @@
         :return: (:math:`S(Q)` vector, uncertainty vector)
         :rtype: (numpy.array, numpy.array)
         """
         fq, dfq = self.FK_to_F(q, fq_keen, dfq_keen, **kwargs)
         return self.F_to_S(q, fq, dfq)
 
     def FK_to_DCS(self, q, fq, dfq=None, **kwargs):
-        """
-        Convert :math:`F(Q)` to :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
+        """Convert :math:`F(Q)` to :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq: :math:`F(Q)` vector
         :type fq: numpy.array or list
         :param dfq: uncertainty vector
         :type dfq: numpy.array or list
@@ -205,16 +195,15 @@
                  uncertainty vector)
         :rtype: (numpy.array, numpy.array)
         """
         return fq + kwargs['<b_tot^2>'], dfq
 
     # Differential cross-section = d_simga / d_Omega
     def DCS_to_F(self, q, dcs, ddcs=None, **kwargs):
-        """
-        Convert :math:`\\frac{d \\sigma}{d \\Omega}(Q)` to :math:`Q[S(Q)-1]`
+        """Convert :math:`\\frac{d \\sigma}{d \\Omega}(Q)` to :math:`Q[S(Q)-1]`
 
         :param q: Q-space vector
         :type q: numpy.array or list
         :param dcs: :math:`\\frac{d \\sigma}{d \\Omega}(Q)` vector
         :type dcs: numpy.array or list
         :param ddcs: uncertainty vector
         :type ddcs: numpy.array or list
@@ -222,16 +211,15 @@
         :return: (:math:`Q[S(Q)-1]` vector, uncertainty vector)
         :rtype: (numpy.array, numpy.array)
         """
         fq, dfq = self.DCS_to_FK(q, dcs, ddcs, **kwargs)
         return self.FK_to_F(q, fq, dfq, **kwargs)
 
     def DCS_to_S(self, q, dcs, ddcs=None, **kwargs):
-        """
-        Convert :math:`\\frac{d \\sigma}{d \\Omega}(Q)` to :math:`S(Q)`
+        """Convert :math:`\\frac{d \\sigma}{d \\Omega}(Q)` to :math:`S(Q)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param dcs: :math:`\\frac{d \\sigma}{d \\Omega}(Q)` vector
         :type dcs: numpy.array or list
         :param ddcs: uncertainty vector
         :type ddcs: numpy.array or list
@@ -239,16 +227,15 @@
         :return: (:math:`S(Q)` vector, uncertainty vector)
         :rtype: (numpy.array, numpy.array)
         """
         fq, dfq = self.DCS_to_FK(q, dcs, ddcs, **kwargs)
         return self.FK_to_S(q, fq, dfq, **kwargs)
 
     def DCS_to_FK(self, q, dcs, ddcs=None, **kwargs):
-        """
-        Convert :math:`\\frac{d \\sigma}{d \\Omega}(Q)` to :math:`F(Q)`
+        """Convert :math:`\\frac{d \\sigma}{d \\Omega}(Q)` to :math:`F(Q)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq: :math:`\\frac{d \\sigma}{d \\Omega}(Q)` vector
         :type fq: numpy.array or list
         :param ddcs: uncertainty vector
         :type ddcs: numpy.array or list
@@ -258,16 +245,15 @@
         """
         return (dcs - kwargs['<b_tot^2>'], ddcs)
 
     # Real Space Conversions
 
     # G(r) = PDF
     def G_to_GK(self, r, gr, dgr=None, **kwargs):
-        r"""
-        Convert :math:`G_{PDFFIT}(r)` to :math:`G_{Keen Version}(r)`
+        r"""Convert :math:`G_{PDFFIT}(r)` to :math:`G_{Keen Version}(r)`
 
         :param r: r-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{PDFFIT}(r)` vector
         :type gr: numpy.array or list
         :param dgr: uncertainty vector :math:`\Delta g(r)`
         :type dgr: numpy.array or list
@@ -278,16 +264,15 @@
         factor = kwargs['<b_coh>^2'] / (4. * np.pi * kwargs['rho'])
         if dgr is None:
             dgr = np.zeros_like(gr)
         return (factor * self._safe_divide(gr, r),
                 factor * self._safe_divide(dgr, r))
 
     def G_to_g(self, r, gr, dgr=None, **kwargs):
-        r"""
-        Convert :math:`G_{PDFFIT}(r)` to :math:`g(r)`
+        r"""Convert :math:`G_{PDFFIT}(r)` to :math:`g(r)`
 
         :param r: r-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{PDFFIT}(r)` vector
         :type gr: numpy.array or list
         :param dgr: uncertainty vector :math:`\Delta g(r)`
         :type dgr: numpy.array or list
@@ -299,16 +284,15 @@
         if dgr is None:
             dgr = np.zeros_like(gr)
         return (self._safe_divide(gr, factor * r) + 1.,
                 self._safe_divide(dgr, factor * r))
 
     # Keen's G(r)
     def GK_to_G(self, r, gr, dgr=None, **kwargs):
-        r"""
-        Convert :math:`G_{Keen Version}(r)` to :math:`G_{PDFFIT}(r)`
+        r"""Convert :math:`G_{Keen Version}(r)` to :math:`G_{PDFFIT}(r)`
 
         :param r: r-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{Keen Version}(r)` vector
         :type gr: numpy.array or list
         :param dgr: uncertainty vector :math:`\Delta g(r)`
         :type dgr: numpy.array or list
@@ -318,16 +302,15 @@
         """
         factor = (4. * np.pi * kwargs['rho']) / kwargs['<b_coh>^2']
         if dgr is None:
             dgr = np.zeros_like(gr)
         return (factor * r * gr, factor * r * dgr)
 
     def GK_to_g(self, r, gr, dgr=None, **kwargs):
-        r"""
-        Convert :math:`G_{Keen Version}(r)` to :math:`g(r)`
+        r"""Convert :math:`G_{Keen Version}(r)` to :math:`g(r)`
 
         :param r: r-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{Keen Version}(r)` vector
         :type gr: numpy.array or list
         :param dgr: uncertainty vector :math:`\Delta g(r)`
         :type dgr: numpy.array or list
@@ -336,16 +319,15 @@
         :rtype: (numpy.array, numpy.array)
         """
         _gr, _dgr = self.GK_to_G(r, gr, dgr=dgr, **kwargs)
         return self.G_to_g(r, _gr, dgr=_dgr, **kwargs)
 
     # g(r)
     def g_to_G(self, r, gr, dgr=None, **kwargs):
-        r"""
-        Convert :math:`g(r)` to :math:`G_{PDFFIT}(r)`
+        r"""Convert :math:`g(r)` to :math:`G_{PDFFIT}(r)`
 
         :param r: r-space vector
         :type r: numpy.array or list
         :param gr: :math:`g(r)` vector
         :type gr: numpy.array or list
         :param dgr: uncertainty vector :math:`\Delta g(r)`
         :type dgr: numpy.array or list
@@ -355,16 +337,15 @@
         """
         factor = 4. * np.pi * r * kwargs['rho']
         if dgr is None:
             dgr = np.zeros_like(gr)
         return (factor * (gr - 1.), factor * dgr)
 
     def g_to_GK(self, r, gr, dgr=None, **kwargs):
-        r"""
-        Convert :math:`g(r)` to :math:`G_{Keen Version}(r)`
+        r"""Convert :math:`g(r)` to :math:`G_{Keen Version}(r)`
 
         :param r: r-space vector
         :type r: numpy.array or list
         :param gr: :math:`g(r)` vector
         :type gr: numpy.array or list
         :param dgr: uncertainty vector :math:`\Delta g(r)`
         :type dgr: numpy.array or list
```

### Comparing `pystog-0.4.0/pystog/fourier_filter.py` & `pystog-1.0.0/pystog/fourier_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 ==============
 
 This module defines the FourierFilter class
 that performs the Fourier filter for a
 given range to exclude.
 """
 
+
+from __future__ import (absolute_import, division, print_function)
+
 import numpy as np
 
 from pystog.converter import Converter
 from pystog.transformer import Transformer
 
 
 class FourierFilter:
-    """
-    The FourierFilter class is used to exlude a given
+    """The FourierFilter class is used to exlude a given
     range in the current function by a back Fourier Transform
     of that section, followed by a difference from the non-excluded
     function, and then a forward transform of the difference function
     Can currently do:
     a real space function -> reciprocal space function -> real space function
 
     :examples:
@@ -36,16 +38,15 @@
 
     def __init__(self):
         self.converter = Converter()
         self.transformer = Transformer()
 
     # g(r)
     def g_using_F(self, r, gr, q, fq, cutoff, dgr=None, dfq=None, **kwargs):
-        """
-        Fourier filters real space :math:`g(r)`
+        """Fourier filters real space :math:`g(r)`
         using the reciprocal space :math:`Q[S(Q)-1]`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`g(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -96,16 +97,15 @@
 
         # Transform delta_F(Q) for g(r) with low-r removed
         r, gr, dgr = self.transformer.F_to_g(q, fq, r, dfq=dfq, **kwargs)
 
         return q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr
 
     def g_using_S(self, r, gr, q, sq, cutoff, dgr=None, dsq=None, **kwargs):
-        """
-        Fourier filters real space :math:`g(r)`
+        """Fourier filters real space :math:`g(r)`
         using the reciprocal space :math:`S(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`g(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -129,16 +129,15 @@
         q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr = self.g_using_F(
             r, gr, q, fq, cutoff, dgr=dgr, dfq=dfq, **kwargs)
         sq_ft, dsq_ft = self.converter.F_to_S(q_ft, fq_ft, dfq=dfq_ft)
         sq, dsq = self.converter.F_to_S(q, fq, dfq=dfq)
         return q_ft, sq_ft, q, sq, r, gr, dsq_ft, dsq, dgr
 
     def g_using_FK(self, r, gr, q, fq, cutoff, dgr=None, dfq=None, **kwargs):
-        """
-        Fourier filters real space :math:`g(r)`
+        """Fourier filters real space :math:`g(r)`
         using the reciprocal space :math:`F(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`g(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -163,16 +162,15 @@
             r, gr, q, fq, cutoff, dgr=dgr, dfq=dfq, **kwargs)
         fq_ft, dfq_ft = self.converter.F_to_FK(
             q_ft, fq_ft, dfq=dfq_ft, **kwargs)
         fq, dfq = self.converter.F_to_FK(q, fq, dfq=dfq, **kwargs)
         return q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr
 
     def g_using_DCS(self, r, gr, q, dcs, cutoff, dgr=None, ddcs=None, **kwargs):
-        """
-        Fourier filters real space :math:`g(r)`
+        """Fourier filters real space :math:`g(r)`
         using the reciprocal space
         :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`g(r)` vector
         :type gr: numpy.array or list
@@ -202,16 +200,15 @@
         dcs_ft, ddcs_ft = self.converter.F_to_DCS(
             q_ft, fq_ft, dfq=dfq_ft, **kwargs)
         dcs, ddcs = self.converter.F_to_DCS(q_ft, fq, dfq=dfq, **kwargs)
         return q_ft, dcs_ft, q, dcs, r, gr, ddcs_ft, ddcs, dgr
 
     # G(R) = PDF
     def G_using_F(self, r, gr, q, fq, cutoff, dgr=None, dfq=None, **kwargs):
-        """
-        Fourier filters real space :math:`G_{PDFFIT}(r)`
+        """Fourier filters real space :math:`G_{PDFFIT}(r)`
         using the reciprocal space :math:`Q[S(Q)-1]`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{PDFFIT}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -240,16 +237,15 @@
         gr, dgr = self.converter.G_to_g(r, gr, dgr=dgr, **kwargs)
         q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr = self.g_using_F(
             r, gr, q, fq, cutoff, dgr=dgr, dfq=dfq, **kwargs)
         gr, dgr = self.converter.g_to_G(r, gr, dgr=dgr, **kwargs)
         return q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr
 
     def G_using_S(self, r, gr, q, sq, cutoff, dgr=None, dsq=None, **kwargs):
-        """
-        Fourier filters real space :math:`G_{PDFFIT}(r)`
+        """Fourier filters real space :math:`G_{PDFFIT}(r)`
         using the reciprocal space :math:`S(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{PDFFIT}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -279,16 +275,15 @@
         q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr = self.G_using_F(
             r, gr, q, fq, cutoff, dgr=dgr, dfq=dfq, **kwargs)
         sq_ft, dsq_ft = self.converter.F_to_S(q_ft, fq_ft, dfq_ft)
         sq, dsq = self.converter.F_to_S(q, fq, dfq)
         return q_ft, sq_ft, q, sq, r, gr, dsq_ft, dsq, dgr
 
     def G_using_FK(self, r, gr, q, fq, cutoff, dgr=None, dfq=None, **kwargs):
-        """
-        Fourier filters real space :math:`G_{PDFFIT}(r)`
+        """Fourier filters real space :math:`G_{PDFFIT}(r)`
         using the reciprocal space :math:`F(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{PDFFIT}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -319,16 +314,15 @@
             r, gr, q, fq, cutoff, dgr=dgr, dfq=dfq, **kwargs)
         fq_ft, dfq_ft = self.converter.F_to_FK(
             q_ft, fq_ft, dfq=dfq_ft, **kwargs)
         fq, dfq = self.converter.F_to_FK(q, fq, dfq=dfq, **kwargs)
         return q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr
 
     def G_using_DCS(self, r, gr, q, dcs, cutoff, dgr=None, ddcs=None, **kwargs):
-        """
-        Fourier filters real space :math:`G_{PDFFIT}(r)`
+        """Fourier filters real space :math:`G_{PDFFIT}(r)`
         using the reciprocal space
         :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{PDFFIT}(r)` vector
         :type gr: numpy.array or list
@@ -358,16 +352,15 @@
         dcs_ft, ddcs_ft = self.converter.F_to_DCS(
             q_ft, fq_ft, dfq=dfq_ft, **kwargs)
         dcs, ddcs = self.converter.F_to_DCS(q, fq, dfq=dfq, **kwargs)
         return q_ft, dcs_ft, q, dcs, r, gr, ddcs_ft, ddcs, dgr
 
     # Keen's G(r)
     def GK_using_F(self, r, gr, q, fq, cutoff, dgr=None, dfq=None, **kwargs):
-        """
-        Fourier filters real space :math:`G_{Keen Version}(r)`
+        """Fourier filters real space :math:`G_{Keen Version}(r)`
         using the reciprocal space :math:`Q[S(Q)-1]`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{Keen Version}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -397,16 +390,15 @@
         gr, dgr = self.converter.GK_to_g(r, gr, dgr=dgr, **kwargs)
         q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr = self.g_using_F(
             r, gr, q, fq, cutoff, dgr=dgr, dfq=dfq, **kwargs)
         gr, dgr = self.converter.g_to_GK(r, gr, dgr=dgr, **kwargs)
         return q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr
 
     def GK_using_S(self, r, gr, q, sq, cutoff, dgr=None, dsq=None, **kwargs):
-        """
-        Fourier filters real space :math:`G_{Keen Version}(r)`
+        """Fourier filters real space :math:`G_{Keen Version}(r)`
         using the reciprocal space :math:`S(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{Keen Version}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -437,16 +429,15 @@
         q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr = self.GK_using_F(
             r, gr, q, fq, cutoff, dgr=dgr, dfq=dfq, **kwargs)
         sq_ft, dsq_ft = self.converter.F_to_S(q_ft, fq_ft, dfq=dfq_ft)
         sq, dsq = self.converter.F_to_S(q, fq, dfq=dfq)
         return q_ft, sq_ft, q, sq, r, gr, dsq_ft, dsq, dgr
 
     def GK_using_FK(self, r, gr, q, fq, cutoff, dgr=None, dfq=None, **kwargs):
-        """
-        Fourier filters real space :math:`G_{Keen Version}(r)`
+        """Fourier filters real space :math:`G_{Keen Version}(r)`
         using the reciprocal space :math:`F(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{Keen Version}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -479,16 +470,15 @@
         fq_ft, dfq_ft = self.converter.F_to_FK(
             q_ft, fq_ft, dfq=dfq_ft, **kwargs)
         fq, dfq = self.converter.F_to_FK(q, fq, dfq=dfq, **kwargs)
         return q_ft, fq_ft, q, fq, r, gr, dfq_ft, dfq, dgr
 
     def GK_using_DCS(self, r, gr, q, dcs, cutoff, dgr=None, ddcs=None,
                      **kwargs):
-        """
-        Fourier filters real space :math:`G_{Keen Version}(r)`
+        """Fourier filters real space :math:`G_{Keen Version}(r)`
         using the reciprocal space
         :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{Keen Version}(r)` vector
         :type gr: numpy.array or list
```

### Comparing `pystog-0.4.0/pystog/io.py` & `pystog-1.0.0/pystog/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,78 @@
 import json
 import argparse
 from pystog.utils import RealSpaceChoices, ReciprocalSpaceChoices
 
 
-def get_cli_parser():
-    """
-    Create the argument parser for the CLI
-
-    :return: Argument parser for PyStoG CLI
-    :rtype: argparse.ArgumentParser
-    """
+def get_cli_args():
     parser = argparse.ArgumentParser()
-
-    parser.add_argument(
-        "--json",
-        type=str,
-        default=None,
-        help="Read JSON input file for arguments")
-
-    parser.add_argument(
-        "--density",
-        type=float,
-        help="Number density (atoms/angstroms^3")
-
+    parser.add_argument("--json", type=str, default=None,
+                        help="Read JSON input file for arguments")
+    parser.add_argument("--density", type=float,
+                        help="Number density (atoms/angstroms^3")
     parser.add_argument(
         "-f",
         "--filename",
         nargs='*',
         action='append',
         default=list(),
         dest='filenames',
         help="Filename, qmin, qmax, yoffset, yscale, Qoffset, function type."
         "Function Types are: %s" %
         json.dumps(ReciprocalSpaceChoices))
-
     parser.add_argument(
         "--stem-name",
         type=str,
         dest="stem_name",
         default="merged",
         help="Stem name for output files")
-
+    parser.add_argument(
+        "--Rmax",
+        type=float,
+        default=50.0,
+        help="Maximum value in angstroms for real-space functions")
     parser.add_argument(
         "--real-space-function",
         type=str,
         default="g(r)",
         dest="real_space_function",
         help="Real-space function typej. Choices are: %s" %
         json.dumps(RealSpaceChoices))
-
-    parser.add_argument(
-        "--Rmax",
-        type=float,
-        default=50.0,
-        help="Maximum value in angstroms for real-space functions")
-
-    parser.add_argument(
-        "--Rpoints",
-        type=int,
-        default=5000,
-        help="Number of points in R for real-space functions")
-
-    parser.add_argument(
-        "--Rdelta",
-        type=float,
-        default=None,
-        help="Bin width to use in R for real-space functions")
-
-    parser.add_argument(
-        "--fourier-filter-cutoff",
-        type=float,
-        default=None,
-        dest="fourier_filter_cutoff",
-        help="Bin width to use in R for real-space functions")
-
-    parser.add_argument(
-        "--lorch-flag",
-        action="store_true",
-        default=False,
-        dest="lorch_flag",
-        help="Apply Lorch function")
-
+    parser.add_argument("--Rpoints", type=int, default=5000,
+                        help="Number of points in R for real-space functions")
+    parser.add_argument("--Rdelta", type=float, default=None,
+                        help="Bin width to use in R for real-space functions")
+    parser.add_argument("--fourier-filter-cutoff", type=float,
+                        default=None, dest="fourier_filter_cutoff",
+                        help="Bin width to use in R for real-space functions")
+    parser.add_argument("--lorch-flag", action="store_true",
+                        default=False, dest="lorch_flag",
+                        help="Apply Lorch function")
     parser.add_argument(
         "--bcoh_sqrd",
         type=float,
         default=1.0,
         dest="bcoh_sqrd",
         help="The (sum c*bbar)^2 term needed for F(Q) and G(r) for RMC output")
-
     parser.add_argument(
         "--btot_sqrd",
         type=float,
         default=1.0,
         dest="btot_sqrd",
         help="The (sum c*b^2) term needed for DCS(Q) input")
-
-    parser.add_argument(
-        "--merging",
-        nargs=2,
-        type=float,
-        default=[0.0, 1.0],
-        help="Offset and Scale to apply to the merged S(Q)")
-
-    parser.add_argument(
-        "--low-q-correction",
-        action='store_true',
-        help="Apply low-Q correction during FT")
-
-    return parser
+    parser.add_argument("--plot", action="store_true", default=False,
+                        help="Plots using matplotlib along the way")
+    parser.add_argument("--merging", nargs=2, type=float, default=[0.0, 1.0],
+                        help="Offset and Scale to apply to the merged S(Q)")
+    parser.add_argument("--low-q-correction", action='store_true',
+                        help="Apply low-Q correction during FT")
+    return parser.parse_args()
 
 
 def parse_cli_args(args):
-    """
-    Parse the CLI arguments and return a key-word dictionary with options to
-    pass to StoG class
-
-    :param args: Namespace returned from parsing the CLI arguments
-    :type args: argparse.Namespace
-    :return: Dictionary with options to pass to StoG class
-    :rtype: dict
-    """
-    if not isinstance(args, argparse.Namespace):
-        msg = "parse_cli_args takes a argparse.Namespace, "
-        msg += "yet was given argument of type: {}"
-        raise TypeError(msg.format(type(args)))
-
     # Get each file's info and story in dictionary
     files_info = list()
     for f in args.filenames:
         file_info = dict()
         file_info["Filename"] = f[0]
         file_info["Qmin"] = float(f[1])
         file_info["Qmax"] = float(f[2])
@@ -142,14 +86,15 @@
         "Files": files_info,
         "NumberDensity": args.density,
         "Rmax": args.Rmax,
         "Rpoints": args.Rpoints,
         "FourierFilter": {
             "Cutoff": args.fourier_filter_cutoff},
         "LorchFlag": args.lorch_flag,
+        "PlotFlag": args.plot,
         "Outputs": {
             "StemName": args.stem_name},
         "Merging": {
             "Y": {
                 "Offset": args.merging[0],
                 "Scale": args.merging[1]}},
         "<b_coh>^2": args.bcoh_sqrd,
```

### Comparing `pystog-0.4.0/pystog/stog.py` & `pystog-1.0.0/pystog/stog.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,46 +4,47 @@
 =============
 
 This module defines the StoG class
 that tries to replicate the previous
 stog program behavior in an organized fashion
 with the ability to re-construct the workflow.
 """
-from __future__ import absolute_import, division, print_function
 
-import sys
-import os
-from h5py import File
 import json
 import numpy as np
+import pandas as pd
 
 from pystog.utils import create_domain, RealSpaceChoices, ReciprocalSpaceChoices
 from pystog.converter import Converter
 from pystog.transformer import Transformer
 from pystog.fourier_filter import FourierFilter
 
-
-class NoInputFilesException(Exception):
-    """Exception when no files are given to process"""
+# Required for non-display environment (i.e. Travis-CI)
+import os
+import matplotlib as mpl
+if os.environ.get('DISPLAY', '') == '':
+    print('no display found. Using non-interactive Agg backend')
+    mpl.use('Agg')
+import matplotlib.pyplot as plt  # noqa: E402
 
 
 class StoG(object):
-    """
-    The StoG class is used to put together
+    """The StoG class is used to put together
     the Converter, Transformer, and FourierFilter
     class functionalities to reproduce the original
     **stog** Fortran program behavior. This class is meant to
     put together the functionality of the classes
     into higher-level calls to construct workflows
     for merging and processing multiple recprical space
     functions into a final output real space function.
 
     This pythonized-version of the original Fortran **stog**
-    uses numpy for data storage, organization, and
-    manipulation "under the hood".
+    uses pandas and numpy for data storage, organization, and
+    manipulation and matplotlib for diagonostic visualization
+    "under the hood".
 
     :examples:
 
     >>> import json
     >>> from pystog import StoG
     >>> with open("../data/examples/argon_pystog.json", 'r') as f:
     >>>     kwargs = json.load(f)
@@ -69,24 +70,28 @@
         self.__update_dr()
         self.__density = 1.0
         self.__bcoh_sqrd = 1.0
         self.__btot_sqrd = 1.0
         self.__low_q_correction = False
         self.__lorch_flag = False
         self.__fourier_filter_cutoff = None
+        self.__plot_flag = True
+        self.__plotting_kwargs = {'figsize': (16, 8),
+                                  'style': '-',
+                                  'ms': 1,
+                                  'lw': 1,
+                                  }
         self.__merged_opts = {"Y": {"Offset": 0.0, "Scale": 1.0}}
         self.__stem_name = "out"
 
-        # Storage arrays for total scattering functions
-        self.__reciprocal_individuals = np.empty([3, 0])
-        self.__sq_individuals = np.empty([3, 0])
-        self.__q_master = {}
-        self.__sq_master = {}
-        self.__r_master = {}
-        self.__gr_master = {}
+        # DataFrames for total scattering functions
+        self.__df_individuals = pd.DataFrame()
+        self.__df_sq_individuals = pd.DataFrame()
+        self.__df_sq_master = pd.DataFrame()
+        self.__df_gr_master = pd.DataFrame()
 
         # Attributes that do not (currently) change
         self.__sq_title = "S(Q) Merged"
         self.__qsq_minus_one_title = "Q[S(Q)-1] Merged"
         self._ft_title = "FT term"
         self.__sq_ft_title = "S(Q) FT"
         self.__fq_title = "F(Q) Merged"
@@ -120,16 +125,15 @@
         #: Must of type :class:`pystog.fourier_filter.FourierFilter`
         self.filter = FourierFilter()
 
         # Use key-word arguments to set attributes
         self.__kwargs2attr(kwargs)
 
     def __kwargs2attr(self, kwargs):
-        """
-        Takes the key-word arguments supplied to the
+        """Takes the key-word arguments supplied to the
         initialization of the class and maps them to
         attirbutes in the class. Commonly get the **kwargs**
         from the JSON input file.
         """
         if "Files" in kwargs:
             self.files = kwargs["Files"]
         if "RealSpaceFunction" in kwargs:
@@ -140,78 +144,73 @@
             self.rmax = float(kwargs["Rmax"])
         if "Rdelta" in kwargs:
             self.rdelta = kwargs["Rdelta"]
         elif "Rpoints" in kwargs:
             self.rdelta = self.rmax / kwargs["Rpoints"]
         if "NumberDensity" in kwargs:
             self.density = kwargs["NumberDensity"]
-        if "OmittedXrangeCorrection" in kwargs:
-            self.low_q_correction = kwargs["OmittedXrangeCorrection"]
+        if 'OmittedXrangeCorrection' in kwargs:
+            self.low_q_correction = kwargs['OmittedXrangeCorrection']
         if "LorchFlag" in kwargs:
             self.lorch_flag = kwargs["LorchFlag"]
         if "FourierFilter" in kwargs:
             if "Cutoff" in kwargs["FourierFilter"]:
                 self.fourier_filter_cutoff = kwargs["FourierFilter"]["Cutoff"]
+        if "PlotFlag" in kwargs:
+            self.plot_flag = kwargs["PlotFlag"]
         if "<b_coh>^2" in kwargs:
             self.bcoh_sqrd = kwargs["<b_coh>^2"]
         if "<b_tot^2>" in kwargs:
             self.btot_sqrd = kwargs["<b_tot^2>"]
         if "Merging" in kwargs:
             self.merged_opts = kwargs["Merging"]
-            if "Transform" in kwargs["Merging"]:
-                transform_opts = kwargs["Merging"]["Transform"]
+            if "Transform" in kwargs['Merging']:
+                transform_opts = kwargs['Merging']["Transform"]
                 if "Qmin" in transform_opts:
                     self.qmin = transform_opts["Qmin"]
                 if "Qmax" in transform_opts:
                     self.qmax = transform_opts["Qmax"]
         if "Outputs" in kwargs:
             if "StemName" in kwargs["Outputs"]:
                 self.stem_name = kwargs["Outputs"]["StemName"]
-        if "NexusFile" in kwargs:
-            self.nexus_file = kwargs["NexusFile"]
-        if "WorkspaceName" in kwargs:
-            self.workspace_name = kwargs["WorkspaceName"]
 
     # General attributes
     @property
     def xmin(self):
-        """
-        The minimum X value of all datasets to
+        """The minimum X value of all datasets to
         use for Fourier transforms (from recirocal space -> real space)
 
         :getter: Returns the current set value
         :setter: Set the xmin value for the Fourier transforms
         :type: float
         """
         return self.__xmin
 
     @xmin.setter
     def xmin(self, value):
         self.__xmin = value
 
     @property
     def xmax(self):
-        """
-        The maximum X value of all datasets to
+        """The maximum X value of all datasets to
         use for Fourier transforms (from recirocal space -> real space)
 
         :getter: Returns the current set value
         :setter: Set the xmax value for the Fourier transforms
         :type: float
         """
         return self.__xmax
 
     @xmax.setter
     def xmax(self, value):
         self.__xmax = value
 
     @property
     def qmin(self):
-        """
-        The :math:`Q_{min}` value to use for the Fourier
+        """The :math:`Q_{min}` value to use for the Fourier
         transforms (from recirocal space -> real space). This
         overrides **xmin** attribute if **xmin** < **qmin**.
 
         :getter: Returns the current set value
         :setter: Set the :math:`Q_{min}` value for the Fourier transforms
         :type: float
         """
@@ -219,16 +218,15 @@
 
     @qmin.setter
     def qmin(self, value):
         self.__qmin = value
 
     @property
     def qmax(self):
-        """
-        The :math:`Q_{max}` value to use for the Fourier
+        """The :math:`Q_{max}` value to use for the Fourier
         transforms (from recirocal space -> real space). This
         overrides **xmax** attribute if **qmax** < **xmax**.
 
         :getter: Returns the current set value
         :setter: Set the qmax value for the Fourier transforms
         :type: float
         """
@@ -236,64 +234,59 @@
 
     @qmax.setter
     def qmax(self, value):
         self.__qmax = value
 
     @property
     def files(self):
-        """
-        The files that contain the reciprocal space data
+        """The files that contain the reciprocal space data
         to merge together.
 
         :getter: Current list of files to merge
         :setter: Set the list of files to merg
         :type: list
         """
         return self.__files
 
     @files.setter
     def files(self, file_list):
         self.__files = file_list
 
     def append_file(self, new_file):
-        """
-        Appends a file to the file list
+        """Appends a file to the file list
 
         :param new_file: New file name to append
         :type new_file: str
         :return: File list with appended new_file
         :rtype: list
         """
         self.files = self.files + [new_file]
         return self.files
 
     def extend_file_list(self, new_files):
-        """
-        Extend the file list with a list of new files
+        """Extend the file list with a list of new files
 
         :param new_files: List of new files
         :type new_file: list
         :return: File list extended by new_files
         :rtype: list
         """
         self.files.extend(new_files)
         return self.files
 
     def __update_dr(self):
-        """
-        Uses **rdelta** and **rmax** attributes (:math:`\\Delta r` and
+        """Uses **rdelta** and **rmax** attributes (:math:`\\Delta r` and
         :math:`R_{max}`, respectively) to construct **dr** attribute
         (:math:`r`-space vector) via its setter
         """
         self.dr = create_domain(self.rmin, self.rmax, self.rdelta)
 
     @property
     def rdelta(self):
-        """
-        The :math:`\\Delta r` for the :math:`r`-space vector
+        """The :math:`\\Delta r` for the :math:`r`-space vector
 
         :getter: Return :math:`\\Delta r` value
         :setter: Set the :math:`\\Delta r` value
                  and update :math:`r`-space vector
                  via the **dr** attribute
         :type: value
         """
@@ -302,16 +295,15 @@
     @rdelta.setter
     def rdelta(self, value):
         self.__rdelta = value
         self.__update_dr()
 
     @property
     def rmin(self):
-        """
-        The :math:`R_{min}` valuefor the :math:`r`-space vector
+        """The :math:`R_{min}` valuefor the :math:`r`-space vector
 
         :getter: Return :math:`R_{min}` value
         :setter: Set the :math:`R_{min}` value and update :math:`r`-space vector
                  via the **dr** attribute
         :type: value
         """
         return self.__rmin
@@ -319,16 +311,15 @@
     @rmin.setter
     def rmin(self, value):
         self.__rmin = value
         self.__update_dr()
 
     @property
     def rmax(self):
-        """
-        The :math:`R_{max}` valuefor the :math:`r`-space vector
+        """The :math:`R_{max}` valuefor the :math:`r`-space vector
 
         :getter: Return :math:`R_{max}` value
         :setter: Set the :math:`R_{max}` value and update :math:`r`-space vector
                  via the **dr** attribute
         :type: value
         """
         return self.__rmax
@@ -336,47 +327,44 @@
     @rmax.setter
     def rmax(self, value):
         self.__rmax = value
         self.__update_dr()
 
     @property
     def dr(self):
-        """
-        The real space function X axis data, :math:`r`-space vector
+        """The real space function X axis data, :math:`r`-space vector
 
         :getter: Return the :math:`r` vector
         :setter: Set the :math:`r` vector
         :type: numpy.array
         """
         return self.__dr
 
     @dr.setter
     def dr(self, r):
         self.__dr = r
 
     @property
     def density(self):
-        """
-        The number density used (atoms/:math:`\\AA^{3}`) used for the
+        """The number density used (atoms/:math:`\\AA^{3}`) used for the
         :math:`\\rho_{0}` term in the equations
 
         :getter: Return the density value
         :setter: Set the density value
         :type: float
         """
         return self.__density
 
     @density.setter
     def density(self, value):
         self.__density = value
 
     @property
     def bcoh_sqrd(self):
-        """
-        The average coherent scattering length, squared:
+        """The average coherent scattering length, squared:
         :math:`\\langle b_{coh} \\rangle^2` =
         :math:`( \\sum_{i} c_{i} b_{coh,i} ) ( \\sum_{i} c_{i} b^*_{coh,i} )`
         where the subscript :math:`i` implies for atom type :math:`i`,
         :math:`c_{i}` is the concentration of :math:`i`,
         :math:`b_{coh,i}` is the coherent scattering length of :math:`i`,
         and :math:`b^*_{coh,i}`
         is the complex coherent scattering length of :math:`i`
@@ -400,16 +388,15 @@
 
     @bcoh_sqrd.setter
     def bcoh_sqrd(self, value):
         self.__bcoh_sqrd = value
 
     @property
     def btot_sqrd(self):
-        """
-        The average coherent scattering length, squared:
+        """The average coherent scattering length, squared:
         :math:`\\langle b_{tot}^2 \\rangle`
         = :math:`\\sum_{i} c_{i} b_{tot,i}^2`
         = :math:`\\frac{1}{4 \\pi} \\sum_i c_{i} \\sigma_{tot,i}`
         where the subscript :math:`i` implies for atom type :math:`i`,
         :math:`c_{i}` is the concentration of :math:`i` and
         :math:`\\sigma_{tot,i}` is the total cross-section of :math:`i`
 
@@ -433,32 +420,30 @@
 
     @btot_sqrd.setter
     def btot_sqrd(self, value):
         self.__btot_sqrd = value
 
     @property
     def stem_name(self):
-        """
-        A stem name to prefix for all output files. Replicates
+        """A stem name to prefix for all output files. Replicates
         the **stog** Fortran program behavior.
 
         :getter: Return the currently set stem name
         :setter: Set the stem name for output files
         :type: str
         """
         return self.__stem_name
 
     @stem_name.setter
     def stem_name(self, name):
         self.__stem_name = name
 
     @property
     def low_q_correction(self):
-        """
-        This sets the option to perform a low-:math:`Q` correction
+        """This sets the option to perform a low-:math:`Q` correction
         for the omitted :math:`Q` range.
 
         See :class:`pystog.transformer.Transformer` **_low_x_correction**
         method for more information.
 
         :getter: Return bool of applying the low-:math:`Q` correction
         :setter: Set whether the correction is applied or not
@@ -471,16 +456,15 @@
         if isinstance(value, bool):
             self.__low_q_correction = value
         else:
             raise TypeError("Expected a bool, True or False")
 
     @property
     def lorch_flag(self):
-        """
-        This sets the option to perform the Lorch dampening correction
+        """This sets the option to perform the Lorch dampening correction
         for the :math:`Q` range. Generally, will help reduce Fourier "ripples",
         or AKA "Gibbs phenomenon", due to discontinuity at :math:`Q_{max}`
         if the reciprocal space function is not at the
         :math:`Q -> \\infty` limit.
         Yet, will also broaden real space function peaks, possibly dubiously.
 
         See :class:`pystog.transformer.Transformer` **fourier_transform** and
@@ -497,16 +481,15 @@
         if isinstance(value, bool):
             self.__lorch_flag = value
         else:
             raise TypeError("Expected a bool, True or False")
 
     @property
     def fourier_filter_cutoff(self):
-        """
-        This sets the cutoff in :math:`r`-space for the Fourier
+        """This sets the cutoff in :math:`r`-space for the Fourier
         filter. The minimum is automatically 0.0. Thus, from
         0.0 to **fourier_filter_cutoff** is reverse transfomed,
         subtracted in reciprocal space, and then the difference
         is back-transformed.
 
         See :class:`pystog.fourier_filter.FourierFilter` for more information.
 
@@ -518,187 +501,163 @@
 
     @fourier_filter_cutoff.setter
     def fourier_filter_cutoff(self, value):
         self.__fourier_filter_cutoff = value
 
     @property
     def merged_opts(self):
-        """
-        This sets the options to perform after merging the
+        """This sets the options to perform after merging the
         reciprocal space functions together, such as an
         overall offset and scale.
 
         :getter: Return the options currently set
         :setter: Set the options for the merged pattern
         :type: dict
         """
         return self.__merged_opts
 
     @merged_opts.setter
     def merged_opts(self, options):
         self.__merged_opts = options
 
-    # Storage array attributes
+    # DataFrame attributes
 
     @property
-    def reciprocal_individuals(self):
-        """
-        The storage array for the input reciprocal space functions
+    def df_individuals(self):
+        """The DataFrame for the input reciprocal space functions
         loaded from **files** and with the loading processing
         from **add_dataset** class method.
 
-        :getter: Returns the current individual, input reciprocal space
-                 functions numpy array.
-                 The dimenions is :math:`3 x N*M` where N is the number
-                 of patterns stored and M is the length of the patterns.
-        :setter: Sets the numpy array
-        :type: numpy.ndarray
+        :getter: Returns the current individual, input
+                 reciprocal space functions DataFrame
+        :setter: Sets the DataFrame
+        :type: pandas.DataFrame
         """
-        return self.__reciprocal_individuals
+        return self.__df_individuals
 
-    @reciprocal_individuals.setter
-    def reciprocal_individuals(self, individuals):
-        self.__reciprocal_individuals = individuals
+    @df_individuals.setter
+    def df_individuals(self, df):
+        self.__df_individuals = df
 
     @property
-    def sq_individuals(self):
-        """
-        The storage array for the :math:`S(Q)` generated from each input
-        reciprocal space dataset in **reciprocal_individuals** array.
+    def df_sq_individuals(self):
+        """The DataFrame for the :math:`S(Q)` generated from each input
+        reciprocal space dataset in **df_individuals** class DataFrame.
 
-        :getter: Returns the current individual :math:`S(Q)` reciprocal space
-                 functions numpy array.
-                 The dimenions is :math:`3 x N*M` where N is the number
-                 of patterns stored and M is the length of the patterns.
-        :setter: Sets the numpy array
-        :type: numpy.ndarray
+        :getter: Returns the current individual :math:`S(Q)`
+                 reciprocal space functions DataFrame
+        :setter: Sets the DataFrame
+        :type: pandas.DataFrame
         """
-        return self.__sq_individuals
+        return self.__df_sq_individuals
 
-    @sq_individuals.setter
-    def sq_individuals(self, individuals):
-        self.__sq_individuals = individuals
+    @df_sq_individuals.setter
+    def df_sq_individuals(self, df):
+        self.__df_sq_individuals = df
 
     @property
-    def sq_master(self):
-        """
-        The "master" dictionary for the :math:`S(Q)` reciprocal
+    def df_sq_master(self):
+        """The "master" DataFrame for the :math:`S(Q)` reciprocal
         space functions that are generated for each processing step.
-
-        :getter: Returns the current "master" :math:`S(Q)` reciprocal space
-                 functions dictionary generated up to the current step in
-                 the workflow.
-        :setter: Sets the "master" :math:`S(Q)` function dictionary
-        :type: dict[str:numpy.ndarray]
         """
-        return self.__sq_master
+        return self.__df_sq_master
 
-    @sq_master.setter
-    def sq_master(self, sq):
-        self.__sq_master = sq
+    @df_sq_master.setter
+    def df_sq_master(self, df):
+        self.__df_sq_master = df
 
     @property
-    def gr_master(self):
-        """
-        The "master" dictionary for the real space functions
+    def df_gr_master(self):
+        """The "master" DataFrame for the real space functions
         that are generated for each processing step.
 
-        :getter: Returns the current "master" real space
-                 functions dictionary generated up to the current step in
-                 the workflow.
-        :setter: Sets the "master" real space function dictionary
-        :type: dict[str:numpy.ndarray]
+        :getter: Returns the current "master" real space function DataFrame
+        :setter: Sets the "master" real space function DataFrame
+        :type: pandas.DataFrame
         """
-        return self.__gr_master
+        return self.__df_gr_master
+
+    @df_gr_master.setter
+    def df_gr_master(self, df):
+        self.__df_gr_master = df
 
-    @gr_master.setter
-    def gr_master(self, gr):
-        self.__gr_master = gr
+    # Visualization attributes
 
     @property
-    def q_master(self):
-        """
-        The "master" dictionary for the domain :math:Q` of the reciprocal
-        space functions that are generated for each processing step.
+    def plot_flag(self):
+        """This sets the option for matplotlib to display
+        diagnostic plots or not.
 
-        :getter: Returns the current "master" :math:`Q` reciprocal space
-                 functions dictionary generated up to the current step in
-                 the workflow.
-        :setter: Sets the "master" :math:`Q` dictionary
-        :type: dict[str:numpy.ndarray]
+        :getter: Return bool of flag
+        :setter: Set whether the diagnostics are displayed or not
+        :type: bool
         """
-        return self.__q_master
+        return self.__plot_flag
 
-    @q_master.setter
-    def q_master(self, q):
-        self.__q_master = q
+    @plot_flag.setter
+    def plot_flag(self, value):
+        if isinstance(value, bool):
+            self.__plot_flag = value
+        else:
+            raise TypeError("Expected a bool, True or False")
 
     @property
-    def r_master(self):
+    def plotting_kwargs(self):
+        """The plot settings for visualization via matplotlib
+
+        :getter: Returns the current arguments
+        :setter: Sets the plotting kwargs
+        :type: dict
         """
-        The "master" dictionary for the domain :math:r` of the real
-        space functions that are generated for each processing step.
+        return self.__plotting_kwargs
 
-        :getter: Returns the current "master" :math:`r` real space
-                 functions dictionary generated up to the current step in
-                 the workflow.
-        :setter: Sets the "master" :math:`r` dictionary
-        :type: dict[str:numpy.ndarray]
-        """
-        return self.__r_master
-
-    @r_master.setter
-    def r_master(self, r):
-        self.__r_master = r
+    @plotting_kwargs.setter
+    def plotting_kwargs(self, kwargs):
+        self.__plotting_kwargs = kwargs
 
     @property
     def real_space_function(self):
-        """
-        The real space function to use throughoutt the processing
+        """The real space function to use throughoutt the processing
 
         :getter: Returns the currently select real space function
         :setter: Set the selected real space function and
                  updates other title attributes that rely on this
                  in their name.
         :type: str
         """
         return self.__real_space_function
 
     @real_space_function.setter
     def real_space_function(self, real_space_function):
         if real_space_function not in RealSpaceChoices:
-            raise ValueError(
-                "real_space_function must be of %s"
-                % ",".join(RealSpaceChoices.keys())
-            )
+            raise ValueError("real_space_function must be of %s" %
+                             ','.join(RealSpaceChoices.keys()))
         self.__real_space_function = real_space_function
         self.__gr_ft_title = "%s FT" % real_space_function
         self.__gr_lorch_title = "%s FT Lorched" % real_space_function
         self.__gr_title = "%s Merged" % real_space_function
 
     @property
     def sq_title(self):
-        """
-        The title of the :math:`S(Q)` function directly after merging
+        """The title of the :math:`S(Q)` function directly after merging
         the reciprocal space functions without any further corrections.
 
         :getter: Returns the current title for this function
         :setter: Sets the title for this function
         :type: str
         """
         return self.__sq_title
 
     @sq_title.setter
     def sq_title(self, title):
         self.__sq_title = title
 
     @property
     def qsq_minus_one_title(self):
-        """
-        The title of the :math:`Q[S(Q)-1]` function
+        """The title of the :math:`Q[S(Q)-1]` function
         directly after merging the reciprocal space
         functions without any further corrections.
 
         :getter: Returns the current title for this function
         :setter: Sets the title for this function
         :type: str
         """
@@ -706,376 +665,329 @@
 
     @qsq_minus_one_title.setter
     def qsq_minus_one_title(self, title):
         self.__qsq_minus_one_title = title
 
     @property
     def sq_ft_title(self):
-        """
-        The title of the :math:`S(Q)` function after
+        """The title of the :math:`S(Q)` function after
         merging and a fourier filter correction.
 
         :getter: Returns the current title for this function
         :setter: Sets the title for this function
         :type: str
         """
         return self.__sq_ft_title
 
     @sq_ft_title.setter
     def sq_ft_title(self, title):
         self.__sq_ft_title = title
 
     @property
     def fq_title(self):
-        """
-        The title of the :math:`F(Q)` function after
+        """The title of the :math:`F(Q)` function after
         merging and a fourier filter correction.
 
         :getter: Returns the current title for this function
         :setter: Sets the title for this function
         :type: str
         """
         return self.__fq_title
 
     @fq_title.setter
     def fq_title(self, title):
         self.__fq_title = title
 
     @property
     def gr_title(self):
-        """
-        The title of the real space function directly after merging
+        """The title of the real space function directly after merging
         the reciprocal space functions without any further corrections.
 
         :getter: Returns the current title for this function
         :setter: Sets the title for this function
         :type: str
         """
         return self.__gr_title
 
     @gr_title.setter
     def gr_title(self, title):
         self.__gr_title = title
 
     @property
     def gr_ft_title(self):
-        """
-        The title for the real space function after both
+        """The title for the real space function after both
         merging and a fourier filter correction
 
         :getter: Returns the current title for this function
         :setter: Sets the title for this function
         :type: str
         """
         return self.__gr_ft_title
 
     @gr_ft_title.setter
     def gr_ft_title(self, title):
         self.__gr_ft_title = title
 
     @property
     def gr_lorch_title(self):
-        """
-        The title for the real space function with the lorch correction
+        """The title for the real space function with the lorch correction
 
         :getter: Returns the current title for this function
         :setter: Sets the title for this function
         :type: str
         """
         return self.__gr_lorch_title
 
     @gr_lorch_title.setter
     def gr_lorch_title(self, title):
         self.__gr_lorch_title = title
 
     @property
     def GKofR_title(self):
-        """
-        The title of the :math:`G_{Keen Version}(r)` with
+        """The title of the :math:`G_{Keen Version}(r)` with
         all corrections applied.
 
         :getter: Returns the current title for this function
         :setter: Sets the title for this function
         :type: str
         """
         return self.__GKofR_title
 
     @GKofR_title.setter
     def GKofR_title(self, title):
         self.__GKofR_title = title
 
-    # -------------------------------------#
-    # Reading and Merging Spectrum
-
-    def extract(self, hdf_file, path, index=None):
-        data = File(hdf_file, "r")
-        # base = path.split("/")[1]
-        # print(data[base+"/title"].value)
-        if index is not None:
-            return data[path][index]
-        return data[path][()]
-
-    def extract_path_from_title(
-        self, hdf_file, title, title_path="title", wksp_path="workspace"
-    ):
-        data = File(hdf_file, "r")
-        choices = list()
-        for name, group in data.items():
-            index = os.path.join(name, title_path)
-            if data[index][(0)].decode("UTF-8") == title:
-                xpath = os.path.join("/", name, wksp_path, "axis1")
-                ypath = os.path.join("/", name, wksp_path, "values")
-                return xpath, ypath
-            else:
-                choices.append(data[index][()])
-
-        print("ERROR: Did not find a workspace with title: %s" % title)
-        print("       These are the workspaces titles found in this file")
-        for c in sorted(choices):
-            print("      %s" % c)
-        sys.exit("Stopping...")
-
-    def extract_xy(self, hdf_file, xpath, ypath, **kwargs):
-        x = self.extract(hdf_file, xpath)
-        y = self.extract(hdf_file, ypath, **kwargs)
-        y = np.insert(y, 0, y[0])  # hack for histogram xaxis
-        return x, y
-
-    def save_xy(self, filename, xdata, ydata):
-        # assert(len(xdata) == len(ydata))
-        with open(filename, "w") as f:
-            f.write("%d\n\n" % len(xdata))
-            for x, y in zip(xdata, ydata):
-                f.write("%f %f\n" % (x, y))
-
-    def read_nexus_file_by_bank(self, nexus_file, bank, title, **kwargs):
-        """
-        Reads an individual file bank by bank and uses the **extract_xy**
-        to handle extraction and **extract_path_from_title** to obtain
-        coord paths
-        """
-
-        xpath, ypath = self.extract_path_from_title(nexus_file, title)
-        output_file = "{}_bank{}.dat".format(title, bank)
-
-        output_file = self.stem_name + output_file
-
-        x, y = self.extract_xy(nexus_file, xpath, ypath, index=bank)
-        self.save_xy(output_file, x, y)
-
-    def read_all_nexus_file_banks(self):
-        # Check that we have files to operate on
-        if not self.files:
-            raise NoInputFilesException("No input files given in arguments")
-        if not self.nexus_file:
-            raise NoInputFilesException("No nexus file given in arguments")
-        if not self.workspace_name:
-            raise NoInputFilesException("No workspace name given in arguments")
-
-        # Read in all the data files
-        for i, file_info in enumerate(self.files):
-            self.read_nexus_file_by_bank(
-                self.nexus_file,
-                int(file_info["BankNumber"]),
-                self.workspace_name,
-            )
+# -------------------------------------#
+# Reading and Merging Spectrum
 
     def read_all_data(self, **kwargs):
-        """
-        Reads all the data from the **files** attribute
+        """Reads all the data from the **files** attribute
         Uses the **read_dataset** method on each file.
 
-        Will append all datasets to the numpy storage array,
-        **reciprocal_individuals**, and also convert to :math:`S(Q)` and add to
-        the **sq_individuals** numpy storage array in **add_dataset** method
+        Will append all datasets as DataFrames to the
+        **df_inviduals** attribute DataFrame
+        and also convert to :math:`S(Q)` and add to the **df_sq_individuals**
+        attribute DataFrame in **add_dataset** method
         via **read_dataset** method.
         """
-        # Check that we have files to operate on
-        if not self.files:
-            raise NoInputFilesException("No input files given in arguments")
+        assert self.files is not None
+        assert len(self.files) != 0
 
-        # Read in all the data files
         for i, file_info in enumerate(self.files):
+            file_info['index'] = i
             self.read_dataset(file_info, **kwargs)
 
     def read_dataset(
-        self, info, xcol=0, ycol=1, dycol=2, sep=r"\s+", skiprows=2, **kwargs
-    ):
-        """
-        Reads an individual file and uses the **add_dataset**
+            self,
+            info,
+            xcol=0,
+            ycol=1,
+            sep=r"\s+",
+            skiprows=2,
+            **kwargs):
+        """Reads an individual file and uses the **add_dataset**
         method to apply all dataset manipulations, such as
         scales, offsets, cropping, etc.
 
+        Will append the DataFrame to the **df_inviduals** attribute DataFrame
+        and also convert to :math:`S(Q)` and add to the **df_sq_individuals**
+        attribute DataFrame in **add_dataset** method.
+
         :param info: Dict with information for dataset
                      (filename, manipulations, etc.)
         :type info: dict
-        :param xcol: Column in data file for X-axis
+        :param xcol: The column in the data file that contains the X-axis
         :type xcol: int
-        :param ycol: Column in data file for Y-axis
+        :param ycol: The column in the data file that contains the Y-axis
         :type ycol: int
-        :param dycol: Column in data file for Y uncertainty
-        :type dycol: int
-        :param sep: Separator for the file used by numpy.loadtxt
+        :param sep: Separator for the file used by pandas.read_csv
         :type sep: raw string
-        :param skiprows: Number of rows to skip. Passed to numpy.loadtxt
+        :param skiprows: Number of rows to skip. Passed to pandas.read_csv
         :type skiprows: int
         """
-        _data = np.loadtxt(
-            info["Filename"], skiprows=skiprows, comments="#", unpack=True
-        )
-        if _data.shape[0] <= xcol or _data.shape[0] <= ycol:
-            raise RuntimeError("Data format incompatible with input parameters")
-        if _data.shape[0] <= dycol:
-            array_seq = (_data[xcol], _data[ycol], np.zeros_like(_data[ycol]))
-            data = np.stack(array_seq)
-        else:
-            data = np.stack((_data[xcol], _data[ycol], _data[dycol]))
-        info["data"] = data
-        self.add_dataset(info, **kwargs)
+        # TODO: Create a proper parser class so we can be
+        # more accepting of file formats.
+        data = pd.read_csv(info['Filename'],
+                           sep=sep,
+                           usecols=[xcol, ycol],
+                           names=['x', 'y'],
+                           skiprows=skiprows,
+                           engine='python',
+                           **kwargs)
+        info['data'] = data
+        self.add_dataset(info, index=info['index'], **kwargs)
 
     def add_dataset(
-        self, info, yscale=1.0, yoffset=0.0, xoffset=0.0, ydecimals=16, **kwargs
-    ):
-        """
-        Takes the info with the dataset and manipulations,
+            self,
+            info,
+            index=0,
+            yscale=1.,
+            yoffset=0.,
+            xoffset=0.,
+            ydecimals=16,
+            **kwargs):
+        """Takes the info with the dataset and manipulations,
         such as scales, offsets, cropping, etc., and creates
-        an invidual numpy array for the pattern.
+        an invidual DataFrame.
+
+        Will append the DataFrame to the **df_inviduals** attribute DataFrame
+        and also convert to :math:`S(Q)` and add to the **df_sq_individuals**
+        attribute DataFrame.
 
         :param info: Dict with information for dataset
                      (filename, manipulations, etc.)
         :type info: dict
+        :param index: Index of the added reciprocal space function dataset
+        :type index: int
         :param yscale: Scale factor for the Y data
                        (i.e. :math:`S(Q)`, :math:`F(Q)`, etc.)
         :type yscale: float
         :param yoffset: Offset factor for the Y data
                         (i.e. :math:`S(Q)`, :math:`F(Q)`, etc.)
         :type yoffset: float
         :param xoffset: Offset factor for the X data (i.e. :math:`Q`)
         :type yoffset: float
         """
         # Extract data
-        x = np.around(np.array(info["data"][0]), decimals=self.__xdecimals)
-        y = np.around(np.array(info["data"][1]), decimals=self.__ydecimals)
-        if len(info["data"]) == 3:
-            dy = np.around(np.array(info["data"][2]), decimals=self.__ydecimals)
-        else:
-            dy = np.zeros_like(y)
+        x = np.around(np.array(info['data']['x']), decimals=self.__xdecimals)
+        y = np.around(np.array(info['data']['y']), decimals=self.__ydecimals)
 
         # Cropping
         xmin = min(x)
         xmax = max(x)
-        if "Qmin" in info:
-            xmin = info["Qmin"]
-        if "Qmax" in info:
-            xmax = info["Qmax"]
-        x, y, dy = self.transformer.apply_cropping(x, y, xmin, xmax, dy=dy)
+        if 'Qmin' in info:
+            xmin = info['Qmin']
+        if 'Qmax' in info:
+            xmax = info['Qmax']
+        x, y, _ = self.transformer.apply_cropping(x, y, xmin, xmax)
 
         # Offset and scale
         adjusting = False
-        if "Y" in info:
+        if 'Y' in info:
             adjusting = True
-            if "Scale" in info["Y"]:
-                yscale = info["Y"]["Scale"]
-            if "Offset" in info["Y"]:
-                yoffset = info["Y"]["Offset"]
+            if 'Scale' in info['Y']:
+                yscale = info['Y']['Scale']
+            if 'Offset' in info['Y']:
+                yoffset = info['Y']['Offset']
 
-        if "X" in info:
+        if 'X' in info:
             adjusting = True
-            if "Offset" in info["X"]:
-                xoffset = info["X"]["Offset"]
+            if 'Offset' in info['X']:
+                xoffset = info['X']['Offset']
 
         if adjusting:
-            x, y, dy = self.apply_scales_and_offset(
-                x, y, dy=dy, yscale=yscale, yoffset=yoffset, xoffset=xoffset
-            )
+            x, y = self._apply_scales_and_offset(
+                x, y, yscale, yoffset, xoffset)
 
         # Save overal x-axis min and max
         self.xmin = min(self.xmin, xmin)
         self.xmax = max(self.xmax, xmax)
 
         # Use Qmin and Qmax to crop datasets
         if self.qmin is not None:
             if self.xmin < self.qmin:
-                x, y, dy = self.transformer.apply_cropping(
-                    x, y, self.qmin, self.xmax, dy=dy
-                )
+                x, y, _ = self.transformer.apply_cropping(
+                    x, y, self.qmin, self.xmax)
         if self.qmax is not None:
             if self.xmax > self.qmax:
-                x, y, dy = self.transformer.apply_cropping(
-                    x, y, self.xmin, self.qmax, dy=dy
-                )
+                x, y, _ = self.transformer.apply_cropping(
+                    x, y, self.xmin, self.qmax)
 
         # Default to S(Q) if function type not defined
         if "ReciprocalFunction" not in info:
             info["ReciprocalFunction"] = "S(Q)"
 
         if info["ReciprocalFunction"] not in ReciprocalSpaceChoices:
             error = "ReciprocalFunction was equal to {given}.\n"
             error += "ReciprocalFunction must be one of the folloing {options}"
             error = error.format(
                 given=info["ReciprocalFunction"],
-                options=json.dumps(ReciprocalSpaceChoices),
-            )
+                options=json.dumps(ReciprocalSpaceChoices))
             raise ValueError(error)
 
-        # Save reciprocal space function to the "invididuals" array
-        array_seq = (self.reciprocal_individuals, np.stack((x, y, dy)))
-        self.reciprocal_individuals = np.concatenate(array_seq, axis=1)
+        # Save reciprocal space function to the "invididuals" DataFrame
+        df = pd.DataFrame(
+            y, columns=[
+                '%s_%d' %
+                (info['ReciprocalFunction'], index)], index=x)
+        self.df_individuals = pd.concat([self.df_individuals, df], axis=1)
 
-        # Convert to S(Q) and save to the individual S(Q) array
+        # Convert to S(Q) and save to the individual S(Q) DataFrame
         if info["ReciprocalFunction"] == "Q[S(Q)-1]":
-            y, dy = self.converter.F_to_S(x, y, dfq=dy)
+            y, dy = self.converter.F_to_S(x, y)
         elif info["ReciprocalFunction"] == "FK(Q)":
             y, dy = self.converter.FK_to_S(
-                x, y, dfq_keen=dy, **{"<b_coh>^2": self.bcoh_sqrd}
-            )
+                x, y, **{'<b_coh>^2': self.bcoh_sqrd})
         elif info["ReciprocalFunction"] == "DCS(Q)":
-            y, dy = self.converter.DCS_to_S(
-                x,
-                y,
-                ddcs=dy,
-                **{"<b_coh>^2": self.bcoh_sqrd, "<b_tot^2>": self.btot_sqrd}
-            )
-        array_seq = (self.sq_individuals, np.stack((x, y, dy)))
-        self.sq_individuals = np.concatenate(array_seq, axis=1)
-
-    @staticmethod
-    def apply_scales_and_offset(
-        x, y, dy=None, yscale=1.0, yoffset=0.0, xoffset=0.0
-    ):
-        """
-        Applies scales to the Y-axis and offsets to both X and Y axes.
+            y, dy = self.converter.DCS_to_S(x, y,
+                                            **{'<b_coh>^2': self.bcoh_sqrd,
+                                               '<b_tot^2>': self.btot_sqrd})
+
+        df = pd.DataFrame(y, columns=['S(Q)_%d' % index], index=x)
+        self.df_sq_individuals = pd.concat(
+            [self.df_sq_individuals, df], axis=1)
+
+    def _apply_scales_and_offset(
+            self,
+            x,
+            y,
+            yscale=1.0,
+            yoffset=0.0,
+            xoffset=0.0):
+        """Applies scales to the Y-axis and offsets to both X and Y axes.
 
         :param x: X-axis data
         :type x: numpy.array or list
         :param y: Y-axis data
         :type y: numpy.array or list
         :param yscale: Y-axis scale factor
         :type yscale: float
         :param yoffset: Y-axis offset factor
         :type yoffset: float
         :param xoffset: X-axis offset factor
         :type xoffset: float
         :return: X and Y vectors after scales and offsets applied
         :rtype: numpy.array pair
         """
-        y = y * yscale
-        y = y + yoffset
-        x = x + xoffset
-        if dy is None:
-            dy = np.zeros_like(y)
-        dy = dy * yscale
-        return x, y, dy
+        y = self._scale(y, yscale)
+        y = self._offset(y, yoffset)
+        x = self._offset(x, xoffset)
+        return x, y
 
-    def merge_data(self):
+    def _offset(self, data, offset):
+        """Applies offset to data
+
+        :param data: Input data
+        :type data: numpy.array or list
+        :param offset: Offset to apply to data
+        :type offset: float
+        :return: Data with offset applied
+        :rtype: numpy.array
+        """
+        data = data + offset
+        return data
+
+    def _scale(self, data, scale):
+        """Applies scale to data
+
+        :param data: Input data
+        :type data: numpy.array or list
+        :param offset: Scale to apply to data
+        :type offset: float
+        :return: Data with scale applied
+        :rtype: numpy.array
         """
-        Merges the reciprocal space data stored in the
-        **reciprocal_individuals** numpy array into a single, merged
+        data = scale * data
+        return data
+
+    def merge_data(self):
+        """Merges the reciprocal space data stored in the
+        **df_individuals** class DataFrame into a single, merged
         recirocal space function. Stores the S(Q) result in
-        **sq_master** dictionary using **sq_title** (default: "S(Q) Merged").
+        **df_sq_master** class DataFrame.
 
         Also, converts this
         merged :math:`S(Q)` into :math:`Q[S(Q)-1]` via the
         **Converter** class and applies any modification
         specified in **merged_opts** dict attribute, specified
         by the **'Q[S(Q)-1]'** key of the dict. If there is modification,
         this modified :math:`Q[S(Q)-1]` will be converted to
@@ -1083,291 +995,238 @@
 
         Example dict of **merged_opts** for scaling of
         :math:`S(Q)` by 2 and then offsetting :math:`Q[S(Q)-1]` by 5:
 
         .. highlight:: python
         .. code-block:: python
 
-                {
-                    "Merging": {
-                        "Y": {
-                            "Offset": 0.0,
-                            "Scale": 2.0
-                        },
-                        "Q[S(Q)-1]": {
-                            "Y": "Offset": 5.0,
-                            "Scale": 1.0
+                {"Merging": { "Y": { "Offset": 0.0,
+                                 "Scale": 2.0 },
+                          "Q[S(Q)-1]": { "Y": "Offset": 5.0,
+                                    "Scale": 1.0 }
                         }
-                    }
-                }
         ...
         """
-        data_merged = []
-        _n_total = 0
-        _n_sum = 0
-        _n_err = 0
-        _previous_x = None
-
-        # At this point we have a concatenated array of data
-        # We need to sort according to Q first
-        # TODO: this is ugly but works for now.
-        _x = self.sq_individuals[0]
-        _y = self.sq_individuals[1]
-        _dy = self.sq_individuals[2]
-        zipped = zip(_x, _y, _dy)
-        ordered = sorted(zipped, key=lambda a: a[0])
-        _x, _y, _dy = zip(*ordered)
-        self.sq_individuals = np.stack(
-            (np.asarray(_x), np.asarray(_y), np.asarray(_dy))
-        )
-
-        # Go through the data and compute the average of points
-        # with the same Q.
-        for item in self.sq_individuals.T:
-            if item[0] == _previous_x:
-                _n_total += 1.0
-                _n_sum += item[1]
-                _n_err += item[2] ** 2
-            else:
-                if _n_total > 0:
-                    data_merged.append(
-                        [
-                            _previous_x,
-                            _n_sum / _n_total,
-                            np.sqrt(_n_err) / _n_total,
-                        ]
-                    )
-                _n_total = 1.0
-                _n_sum = item[1]
-                _n_err = item[2] ** 2
-            _previous_x = item[0]
-        if _n_total > 0:
-            data_merged.append(
-                [_previous_x, _n_sum / _n_total, np.sqrt(_n_err) / _n_total]
-            )
-
-        data_merged = np.asarray(data_merged).T
-
-        q = data_merged[0]
-        sq = data_merged[1]
-        dsq = data_merged[2]
-
-        q, sq, dsq = self.apply_scales_and_offset(
-            q,
-            sq,
-            yscale=self.merged_opts["Y"]["Scale"],
-            yoffset=self.merged_opts["Y"]["Offset"],
-            xoffset=0.0,
-            dy=dsq,
-        )
-        self.q_master[self.sq_title] = q
-        self.sq_master[self.sq_title] = sq
+        # TODO: Refator to have "S(Q)" as key for S(Q) modifications
+
+        # Sum over single S(Q) columns into a merged S(Q)
+        single_sofqs = self.df_sq_individuals.iloc[:, :]
+        self.df_sq_master[self.sq_title] = single_sofqs.mean(axis=1)
+
+        q = self.df_sq_master[self.sq_title].index.values
+        sq = self.df_sq_master[self.sq_title].values
+
+        q, sq = self._apply_scales_and_offset(q, sq,
+                                              self.merged_opts['Y']['Scale'],
+                                              self.merged_opts['Y']['Offset'],
+                                              0.0)
+        self.df_sq_master[self.sq_title] = sq
 
         # Also, create merged Q[S(Q)-1] with modifications, if specified
-        fofq, dfofq = self.converter.S_to_F(q, sq, dsq=dsq)
+        fofq, dfofq = self.converter.S_to_F(q, sq)
         if "Q[S(Q)-1]" in self.merged_opts:
             fofq_opts = self.merged_opts["Q[S(Q)-1]"]
             if "Y" in fofq_opts:
                 if "Scale" in fofq_opts["Y"]:
                     fofq *= fofq_opts["Y"]["Scale"]
                 if "Offset" in fofq_opts["Y"]:
                     fofq += fofq_opts["Y"]["Offset"]
-        self.q_master[self.qsq_minus_one_title] = q
-        self.sq_master[self.qsq_minus_one_title] = fofq
+        self.df_sq_master[self.qsq_minus_one_title] = fofq
 
         # Convert this Q[S(Q)-1] back to S(Q) and overwrite the 1st one
-        sq, dsq = self.converter.F_to_S(q, fofq, dfq=dfofq)
+        sq, dsq = self.converter.F_to_S(q, fofq)
         sq[np.isnan(sq)] = 0
-        self.sq_master[self.sq_title] = sq
+        self.df_sq_master[self.sq_title] = sq
 
     # -------------------------------------#
     # Transform Utilities
 
     def transform_merged(self):
-        """
-        Performs the Fourier transform on the merged **sq_master**
-        pattern to generate the desired real space function
+        """Performs the Fourier transform on the merged **df_sq_master**
+        DataFrame to generate the desired real space function
         with this correction. The results for real space are:
-        the domain is saved to the **r_master** dictionary and
-        the range is saved to the **gr_master** dictionary,
-        with both using the **gr_title** for the key of the dictionaries.
+        saved back to the **gr_master** DataFrame
         """
         # Create r-space vector if needed
         if self.dr is None or len(self.dr) == 0:
             self.__update_dr()
 
         # Get Q and S(Q)
-        q = self.q_master[self.sq_title]
-        sq = self.sq_master[self.sq_title]
+        q = self.df_sq_master[self.sq_title].index.values
+        sq = self.df_sq_master[self.sq_title].values
 
         # Perform the Fourier transform to selected real space function
-        transform_kwargs = {
-            "lorch": False,
-            "rho": self.density,
-            "<b_coh>^2": self.bcoh_sqrd,
-        }
+        transform_kwargs = {'lorch': False,
+                            'rho': self.density,
+                            '<b_coh>^2': self.bcoh_sqrd
+                            }
         if self.real_space_function == "g(r)":
             r, gofr, dgofr = self.transformer.S_to_g(
-                q, sq, self.dr, **transform_kwargs
-            )
+                q, sq, self.dr, **transform_kwargs)
         elif self.real_space_function == "G(r)":
             r, gofr, dgofr = self.transformer.S_to_G(
-                q, sq, self.dr, **transform_kwargs
-            )
+                q, sq, self.dr, **transform_kwargs)
         elif self.real_space_function == "GK(r)":
             r, gofr, dgofr = self.transformer.S_to_GK(
-                q, sq, self.dr, **transform_kwargs
-            )
+                q, sq, self.dr, **transform_kwargs)
 
-        self.gr_master[self.gr_title] = gofr
-        self.r_master[self.gr_title] = r
+        self.df_gr_master[self.gr_title] = gofr
+        self.df_gr_master = self.df_gr_master.set_index(r)
 
     def fourier_filter(self):
-        """
-        Performs the Fourier filter on the **sq_master**
-        pattern to generate the desired real space function
+        """Performs the Fourier filter on the **df_sq_master**
+        DataFrame to generate the desired real space function
         with this correction. The results from both reciprocal space and
         real space are:
 
-        1. Saved back to the respective "master" dictionaries
+        1. Saved back to the respective "master" DataFrames
         2. Saved to files via the **stem_name**
-        3. Returned from function
+        3. (optional) Plotted for diagnostics
+        4. Returned from function
 
         :return: Returns a tuple with :math:`r`,
                  the selected real space function,
                  :math:`Q`,
                  and :math:`S(Q)` functions
         :rtype: tuple of numpy.array
         """
-        kwargs = {
-            "lorch": False,
-            "rho": self.density,
-            "<b_coh>^2": self.bcoh_sqrd,
-            "OmittedXrangeCorrection": self.low_q_correction,
-        }
+        kwargs = {'lorch': False,
+                  'rho': self.density,
+                  '<b_coh>^2': self.bcoh_sqrd,
+                  'OmittedXrangeCorrection': self.low_q_correction
+                  }
         cutoff = self.fourier_filter_cutoff
 
         # Get reciprocal and real space data
-        if self.gr_title not in self.gr_master:
+        if self.gr_title not in self.df_gr_master.columns:
             msg = (
                 "WARNING: Fourier filtered before initial transform. "
-                "Peforming now..."
-            )
+                "Peforming now...")
             print(msg)
             self.transform_merged()
 
-        r = self.r_master[self.gr_title]
-        gr = self.gr_master[self.gr_title]
-        q = self.q_master[self.sq_title]
-        sq = self.sq_master[self.sq_title]
+        r = self.df_gr_master[self.gr_title].index.values
+        gr = self.df_gr_master[self.gr_title].values
+        q = self.df_sq_master[self.sq_title].index.values
+        sq = self.df_sq_master[self.sq_title].values
 
         # Fourier filter g(r)
         # NOTE: Real space function setter will catch ValueError so
         # so no need for `else` to catch error
         if self.real_space_function == "g(r)":
             q_ft, sq_ft, q, sq, r, gr, _, _, _ = self.filter.g_using_S(
-                r, gr, q, sq, cutoff, **kwargs
-            )
+                r, gr, q, sq, cutoff, **kwargs)
         elif self.real_space_function == "G(r)":
             q_ft, sq_ft, q, sq, r, gr, _, _, _ = self.filter.G_using_S(
-                r, gr, q, sq, cutoff, **kwargs
-            )
+                r, gr, q, sq, cutoff, **kwargs)
         elif self.real_space_function == "GK(r)":
             q_ft, sq_ft, q, sq, r, gr, _, _, _ = self.filter.GK_using_S(
-                r, gr, q, sq, cutoff, **kwargs
-            )
+                r, gr, q, sq, cutoff, **kwargs)
 
-        # Round to avoid mismatch index in domain and NaN
+        # Round to avoid mismatch index in DataFrame and NaN for column values
         q = np.around(q, decimals=self.__xdecimals)
         sq = np.around(sq, decimals=self.__ydecimals)
         q_ft = np.around(q_ft, decimals=self.__xdecimals)
         sq_ft = np.around(sq_ft, decimals=self.__ydecimals)
 
         # Add output to master dataframes and write files
-        self.q_master[self._ft_title] = q_ft
-        self.sq_master[self._ft_title] = sq_ft
+        self.df_sq_master = self.add_to_dataframe(
+            q_ft, sq_ft, self.df_sq_master, self._ft_title)
         self.write_out_ft()
 
-        self.q_master[self.sq_ft_title] = q
-        self.sq_master[self.sq_ft_title] = sq
+        self.df_sq_master = self.add_to_dataframe(
+            q, sq, self.df_sq_master, self.sq_ft_title)
         self.write_out_ft_sq()
 
-        self.r_master[self.gr_ft_title] = r
-        self.gr_master[self.gr_ft_title] = gr
+        self.df_gr_master = self.add_to_dataframe(
+            r, gr, self.df_gr_master, self.gr_ft_title)
         self.write_out_ft_gr()
 
+        # Plot results
+        if self.plot_flag:
+            exclude_list = [self.qsq_minus_one_title, self.sq_ft_title]
+            self.plot_sq(
+                ylabel="FourierFilter(Q)",
+                title="Fourier Transform of the low-r region below cutoff",
+                exclude_list=exclude_list)
+            exclude_list = [self.qsq_minus_one_title]
+            self.plot_sq(
+                title="Fourier Filtered S(Q)",
+                exclude_list=exclude_list)
+            self.plot_gr(
+                title="Fourier Filtered %s" %
+                self.real_space_function)
+
         return q, sq, r, gr
 
     def apply_lorch(self, q, sq, r):
-        """
-        Performs the Fourier transform using the Lorch
+        """Performs the Fourier transform using the Lorch
         dampening correction on the merged :math:`S(Q)` from
-        the **sq_master** dictionary to generate the
+        the **df_sq_master** DataFrame to generate the
         desired real space function with
         this correction. The results from both reciprocal space and
         real space are:
 
-        1. Saved back to the respective "master" dictionaries
+        1. Saved back to the respective "master" DataFrames
         2. Saved to files via the **stem_name**
-        3. Returned from function
+        3. (optional) Plotted for diagnostics
+        4. Returned from function
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param sq: :math:`S(Q)` vector
         :type sq: numpy.array or list
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :return: Returns a tuple with :math:`r` and selected real space function
         :rtype: tuple of numpy.array
         """
         if self.real_space_function == "g(r)":
             r, gr_lorch, _ = self.transformer.S_to_g(
-                q, sq, r, **{"lorch": True, "rho": self.density}
-            )
+                q, sq, r, **{'lorch': True, 'rho': self.density})
         elif self.real_space_function == "G(r)":
             r, gr_lorch, _ = self.transformer.S_to_G(
-                q, sq, r, **{"lorch": True}
-            )
+                q, sq, r, **{'lorch': True})
         elif self.real_space_function == "GK(r)":
             r, gr_lorch, _ = self.transformer.S_to_GK(
-                q,
-                sq,
-                r,
+                q, sq, r,
                 **{
-                    "lorch": True,
-                    "rho": self.density,
-                    "<b_coh>^2": self.bcoh_sqrd,
-                }
-            )
+                    'lorch': True,
+                    'rho': self.density,
+                    '<b_coh>^2': self.bcoh_sqrd
+                })
 
-        self.gr_master[self.gr_lorch_title] = gr_lorch
-        self.r_master[self.gr_lorch_title] = r
+        self.df_gr_master = self.add_to_dataframe(
+            r, gr_lorch, self.df_gr_master, self.gr_lorch_title)
         self.write_out_lorched_gr()
 
+        if self.plot_flag:
+            self.plot_gr(
+                title="Lorched %s" %
+                self.real_space_function)
+
         return r, gr_lorch
 
     def _get_lowR_mean_square(self):
-        """
-        Retuns the low-R mean square value for the real space function stored
-        in the "master" real space function, **gr_master**.
+        """Retuns the low-R mean square value for the real space function stored
+        in the "master" real space function class DataFrame, **df_gr_master**.
         Used as a cost function for optimiziation of the :math:`Q_{max}` value
         by an iterative adjustment. Calls **_lowR_mean_square* method.
         **Currently not used in PyStoG workflow since was done manually.**
 
         :return: The calculated low-R mean-square value
         :rtype: float
         """
         # TODO: Automate the :math:`Q_{max}` adjustment in an iterative loop
         # using a minimizer.
-        gr = self.gr_master[self.gr_title]
+        gr = self.df_gr_master[self.gr_title].values
         return self._lowR_mean_square(self.dr, gr)
 
     def _lowR_mean_square(self, r, gr, limit=1.01):
-        """
-        Calculates the low-R mean square value from a given real space function.
+        """Calculates the low-R mean square value from a given real space function.
         Used as a cost function for optimiziation of the :math:`Q_{max}` value
         by an iterative adjustment.
         **Currently not used in PyStoG workflow since was done manually.**
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: real space function vector
@@ -1382,171 +1241,321 @@
         # using a minimizer.
         gr = gr[r <= limit]
         gr_sq = np.multiply(gr, gr)
         average = sum(gr_sq)
         return np.sqrt(average)
 
     def _add_keen_fq(self, q, sq):
-        """
-        Adds the Keen version of :math:`F(Q)` to the
-        "master" recprical space storage array, **sq_master**, and
+        """Adds the Keen version of :math:`F(Q)` to the
+        "master" recprical space DataFrame, **df_sq_master**, and
         writes it out to file using the **stem_name**.
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param sq: :math:`S(Q)` vector
         :type sq: numpy.array or list
         """
-        kwargs = {"rho": self.density, "<b_coh>^2": self.bcoh_sqrd}
+        kwargs = {'rho': self.density, "<b_coh>^2": self.bcoh_sqrd}
         fq, dfq = self.converter.S_to_FK(q, sq, **kwargs)
-        self.sq_master[self.fq_title] = fq
-        self.q_master[self.fq_title] = q
+        self.df_sq_master = self.add_to_dataframe(
+            q, fq, self.df_sq_master, self.fq_title)
         self.write_out_rmc_fq()
 
     def _add_keen_gr(self, r, gr):
-        """
-        Adds the Keen version of :math:`G(r)` to the
-        "master" real space storage array, **gr_master**, and
+        """Adds the Keen version of :math:`G(r)` to the
+        "master" real space DataFrame, **df_gr_master**, and
         writes it out to file using the **stem_name**.
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: real space function vector
         :type gr: numpy.array or list
         """
-        kwargs = {"rho": self.density, "<b_coh>^2": self.bcoh_sqrd}
+        kwargs = {'rho': self.density, "<b_coh>^2": self.bcoh_sqrd}
         if self.real_space_function == "g(r)":
             GKofR, dGKofR = self.converter.g_to_GK(r, gr, **kwargs)
         elif self.real_space_function == "G(r)":
             GKofR, dGKofR = self.converter.G_to_GK(r, gr, **kwargs)
         elif self.real_space_function == "GK(r)":
             GKofR = gr
 
-        self.gr_master[self.GKofR_title] = GKofR
-        self.r_master[self.GKofR_title] = r
+        self.df_gr_master = self.add_to_dataframe(
+            r, GKofR, self.df_gr_master, self.GKofR_title)
         self.write_out_rmc_gr()
 
     # -------------------------------------#
+    # Plot Utilities
+
+    def _plot_df(self, df, xlabel, ylabel, title, exclude_list):
+        """Utility function to help plot a DataFrame
+
+        :param df: DataFrame to plot
+        :type df: pandas.DataFrame
+        :param xlabel: X-axis label
+        :type xlabel: str
+        :param ylabel: Y-axis label
+        :type ylabel: str
+        :param title: Title of plot
+        :type title: str
+        :param exclude_list: List of titles of columns in
+                        DataFrame **df** to exclude from plot
+        :type exclude_list: list of str
+        """
+        if exclude_list:
+            columns_diff = df.columns.difference(exclude_list)
+            columns_diff_ids = df.columns.get_indexer(columns_diff)
+            df = df.iloc[:, columns_diff_ids]
+        df.plot(**self.plotting_kwargs)
+        plt.xlabel(xlabel)
+        plt.ylabel(ylabel)
+        plt.title(title)
+        plt.show()
+
+    def plot_sq(self, xlabel='Q', ylabel='S(Q)', title='', exclude_list=None):
+        """Helper function to plot the :math:`S(Q)` functions
+        in the "master" DataFrame, **df_sq_master**.
+
+        :param xlabel: X-axis label
+        :type xlabel: str
+        :param ylabel: Y-axis label
+        :type ylabel: str
+        :param title: Title of plot
+        :type title: str
+        :param exclude_list: List of titles of columns in
+                        DataFrame to exclude from plot
+        :type exclude_list: list of str
+        """
+        df_sq = self.df_sq_master
+        self._plot_df(df_sq, xlabel, ylabel, title, exclude_list)
+
+    def plot_merged_sq(self):
+        """Helper function to multiplot the individual
+        real space functions in the **df_individuals** DataFrame,
+        these functions as individual :math:`S(Q)`, the merged
+        :math:`S(Q)` from the individual functions, and
+        :math:`Q[S(Q)-1]`.
+        """
+
+        plot_kwargs = self.plotting_kwargs.copy()
+        plot_kwargs['style'] = 'o-'
+        plot_kwargs['lw'] = 0.5
+
+        fig, axes = plt.subplots(2, 2, sharex=True)
+        plt.xlabel("Q")
+
+        # Plot the inividual reciprocal functions
+        if self.df_individuals.empty:
+            self.df_sq_individuals.plot(ax=axes[0, 0], **plot_kwargs)
+        else:
+            self.df_individuals.plot(ax=axes[0, 0], **plot_kwargs)
+
+        # Plot the inividual S(Q) functions
+        self.df_sq_individuals.plot(ax=axes[0, 1], **plot_kwargs)
+        axes[0, 1].set_ylabel("S(Q)")
+        axes[0, 1].set_title("Individual S(Q)")
+
+        # Plot the merged S(Q)
+        df_sq = self.df_sq_master.loc[:, [self.sq_title]]
+        df_sq.plot(ax=axes[1, 0], **plot_kwargs)
+        axes[1, 0].set_title("Merged S(Q)")
+        axes[1, 0].set_ylabel("S(Q)")
+
+        # Plot the merged Q[S(Q)-1]
+        df_fq = self.df_sq_master.loc[:, [self.qsq_minus_one_title]]
+        df_fq.plot(ax=axes[1, 1], **plot_kwargs)
+        axes[1, 1].set_title("Merged Q[S(Q)-1]")
+        axes[1, 1].set_ylabel("Q[S(Q)-1]")
+
+        plt.show()
+
+    def plot_gr(self, xlabel='r', ylabel='G(r)', title='', exclude_list=None):
+        """Helper function to plot the real space functions
+        in the "master" DataFrame, **df_gr_master**.
+
+        :param xlabel: X-axis label
+        :type xlabel: str
+        :param ylabel: Y-axis label
+        :type ylabel: str
+        :param title: Title of plot
+        :type title: str
+        :param exclude_list: List of titles of columns in
+                        DataFrame to exclude from plot
+        :type exclude_list: list of str
+        """
+        df_gr = self.df_gr_master
+        self._plot_df(df_gr, xlabel, ylabel, title, exclude_list)
+
+    def plot_summary_sq(self):
+        """Helper function to multiplot the reciprocal space
+        functions during processing and the :math:`F(Q)` function.
+        """
+        if self.fq_title not in self.df_sq_master.columns:
+            q = self.df_sq_master[self.sq_title].index.values
+            sq = self.df_sq_master[self.sq_title].values
+            self._add_keen_fq(q, sq)
+
+        fig, (ax1, ax2) = plt.subplots(1, 2, sharey=True)
+        exclude_list = [self.fq_title]
+        df = self.df_sq_master
+        columns_diff = df.columns.difference(exclude_list)
+        columns_diff_ids = df.columns.get_indexer(columns_diff)
+        df_sq = self.df_sq_master.iloc[:, columns_diff_ids]
+        df_sq.plot(ax=ax1, **self.plotting_kwargs)
+        df_fq = self.df_sq_master.loc[:, [self.fq_title]]
+        df_fq.plot(ax=ax2, **self.plotting_kwargs)
+        plt.xlabel("Q")
+        ax1.set_ylabel("S(Q)")
+        ax1.set_title("StoG S(Q) functions")
+        ax2.set_ylabel("FK(Q)")
+        ax2.set_title("Keen's F(Q)")
+        plt.show()
+
+    def plot_summary_gr(self):
+        """Helper function to multiplot the real space
+        functions during processing
+        and the :math:`G_{Keen Version}(Q)` function.
+        """
+        if self.GKofR_title not in self.df_gr_master.columns:
+            r = self.df_gr_master[self.gr_title].index.values
+            gr = self.df_gr_master[self.gr_title].values
+            self._add_keen_gr(r, gr)
+        fig, (ax1, ax2) = plt.subplots(1, 2, sharey=True)
+        df = self.df_gr_master
+        columns_diff = df.columns.difference([self.GKofR_title])
+        columns_diff_ids = df.columns.get_indexer(columns_diff)
+        df_gr = df.iloc[:, columns_diff_ids]
+        df_gr.plot(ax=ax1, **self.plotting_kwargs)
+        df_gk = df.loc[:, [self.GKofR_title]]
+        df_gk.plot(ax=ax2, **self.plotting_kwargs)
+        plt.xlabel("r")
+        ax1.set_ylabel(self.real_space_function)
+        ax1.set_title("StoG %s functions" % self.real_space_function)
+        ax2.set_ylabel("GK(r)")
+        ax2.set_title("Keen's G(r)")
+        plt.show()
+
+    # -------------------------------------#
     # Output Utilities
-    def _write_out_to_file(self, x, y, filename, places=12):
-        """
-        Helper function for writing out X Y data
-        to the filename in the RMCProfile format.
 
-        :param x: X data to write out
-        :type x: list
-        :param y: Y data to write out
-        :type y: list
+    def add_to_dataframe(self, x, y, df, title):
+        """Takes X,Y dataset and adds it to the given Datframe **df**,
+        with the given **title**. Utility function for updating
+        the class DataFrames.
+
+        :param x: X-axis vector
+        :type x: numpy.array or list
+        :param y: Y-axis vector
+        :type y: numpy.array or list
+        :param df: DataFrame to append (**x**, **y**) pair to as a column
+        :type df: pandas.DataFrame
+        :param title: The title of the column in the DataFrame
+        :type title: str
+        :return: DataFrame with X,Y data appended with given title
+        :rtype: pandas.DataFrame
+        """
+        df_temp = pd.DataFrame(y, columns=[title], index=x)
+        if title in df.columns:
+            df[title] = df_temp[title]
+            return df
+        df = pd.concat([df, df_temp], axis=1)
+        return df
+
+    def _write_out_df(self, df, cols, filename):
+        """Helper function for writing out the DataFrame **df**
+        and the given columns, **cols**, to the filename in
+        the RMCProfile format.
+
+        :param df: DataFrame to write from to filename
+        :type df: pandas.DataFrame
+        :param cols: Column title list for columns to write out
+        :type cols: List of str
         :param filename: Filename to write to
         :type filename: str
         """
-        with open(filename, "w") as f:
-            f.write("%d \n" % len(x))
+        if df.empty:
+            raise ValueError("Empty dataframe. Cannot write out.")
+
+        with open(filename, 'w') as f:
+            f.write("%d \n" % df.shape[0])
             f.write("# Comment line\n")
-        with open(filename, "a") as f:
-            for i, j in zip(x, y):
-                fmt = "{:.{places}f} {:.{places}f}\n"
-                f.write(fmt.format(i, j, places=places))
+        with open(filename, 'a') as f:
+            df.to_csv(f, sep='\t', columns=cols, header=False)
 
     def write_out_merged_sq(self, filename=None):
-        """
-        Helper function for writing out the merged :math:`S(Q)`
+        """Helper function for writing out the merged :math:`S(Q)`
 
         :param filename: Filename to write to
         :type filename: str
         """
         if filename is None:
             filename = "%s.sq" % self.stem_name
-        x = self.q_master[self.sq_title]
-        y = self.sq_master[self.sq_title]
-        self._write_out_to_file(x, y, filename)
+        self._write_out_df(self.df_sq_master, [self.sq_title], filename)
 
     def write_out_merged_gr(self, filename=None):
-        """
-        Helper function for writing out the merged real space function
+        """Helper function for writing out the merged real space function
 
         :param filename: Filename to write to
         :type filename: str
         """
         if filename is None:
             filename = "%s.gr" % self.stem_name
-        x = self.r_master[self.gr_title]
-        y = self.gr_master[self.gr_title]
-        self._write_out_to_file(x, y, filename)
+        self._write_out_df(self.df_gr_master, [self.gr_title], filename)
 
     def write_out_ft(self, filename=None):
-        """
-        Helper function for writing out the Fourier filter correction.
+        """Helper function for writing out the Fourier filter correction.
 
         :param filename: Filename to write to
         :type filename: str
         """
         if filename is None:
             filename = "ft.dat"
-        x = self.q_master[self._ft_title]
-        y = self.sq_master[self._ft_title]
-        self._write_out_to_file(x, y, filename)
+        self._write_out_df(self.df_sq_master, [self._ft_title], filename)
 
     def write_out_ft_sq(self, filename=None):
-        """
-        Helper function for writing out the Fourier filtered :math:`S(Q)`
+        """Helper function for writing out the Fourier filtered :math:`S(Q)`
 
         :param filename: Filename to write to
         :type filename: str
         """
         if filename is None:
             filename = "%s_ft.sq" % self.stem_name
-        x = self.q_master[self.sq_ft_title]
-        y = self.sq_master[self.sq_ft_title]
-        self._write_out_to_file(x, y, filename)
+        self._write_out_df(self.df_sq_master, [self.sq_ft_title], filename)
 
     def write_out_ft_gr(self, filename=None):
-        """
-        Helper function for writing out the Fourier filtered real space function
+        """Helper function for writing out the Fourier filtered real space function
 
         :param filename: Filename to write to
         :type filename: str
         """
         if filename is None:
             filename = "%s_ft.gr" % self.stem_name
-        x = self.r_master[self.gr_ft_title]
-        y = self.gr_master[self.gr_ft_title]
-        self._write_out_to_file(x, y, filename)
+        self._write_out_df(self.df_gr_master, [self.gr_ft_title], filename)
 
     def write_out_lorched_gr(self, filename=None):
-        """
-        Helper function for writing out the Lorch dampened real space function
+        """Helper function for writing out the Lorch dampened real space function
 
         :param filename: Filename to write to
         :type filename: str
         """
         if filename is None:
             filename = "%s_ft_lorched.gr" % self.stem_name
-        x = self.r_master[self.gr_lorch_title]
-        y = self.gr_master[self.gr_lorch_title]
-        self._write_out_to_file(x, y, filename)
+        self._write_out_df(self.df_gr_master, [self.gr_lorch_title], filename)
 
     def write_out_rmc_fq(self, filename=None):
-        """
-        Helper function for writing out the output :math:`F(Q)`
+        """Helper function for writing out the output :math:`F(Q)`
 
         :param filename: Filename to write to
         :type filename: str
         """
         if filename is None:
             filename = "%s_rmc.fq" % self.stem_name
-        x = self.q_master[self.fq_title]
-        y = self.sq_master[self.fq_title]
-        self._write_out_to_file(x, y, filename)
+        self._write_out_df(self.df_sq_master, [self.fq_title], filename)
 
     def write_out_rmc_gr(self, filename=None):
-        """
-        Helper function for writing out the output :math:`G_{Keen Version}(Q)`
+        """Helper function for writing out the output :math:`G_{Keen Version}(Q)`
 
         :param filename: Filename to write to
         :type filename: str
         """
         if filename is None:
             filename = "%s_rmc.gr" % self.stem_name
-        x = self.r_master[self.GKofR_title]
-        y = self.gr_master[self.GKofR_title]
-        self._write_out_to_file(x, y, filename)
+        self._write_out_df(self.df_gr_master, [self.GKofR_title], filename)
```

### Comparing `pystog-0.4.0/pystog/transformer.py` & `pystog-1.0.0/pystog/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 Transformer
 =============
 
 This module defines the Transformer class
 that performs the Fourier transforms
 """
 
+from __future__ import (absolute_import, division, print_function)
 import numpy as np
 
 from pystog.converter import Converter
 
 # -------------------------------------------------------#
 # Transforms between Reciprocal and Real Space Functions
 
 
 class Transformer:
-    """
-    The Transformer class is used to Fourier transform
+    """The Transformer class is used to Fourier transform
     between the difference spaces. Either:
     a reciprocal space function -> real space function
     or a real space function -> reciprocal space function
 
     :examples:
 
     >>> import numpy
@@ -34,16 +34,15 @@
     >>> q, sq, dsq = transformer.G_to_S(r, gr, q)
     """
 
     def __init__(self):
         self.converter = Converter()
 
     def _low_x_correction(self, xin, yin, xout, yout, **kwargs):
-        """
-        Omitted low-x range correction performed in the
+        """Omitted low-x range correction performed in the
         space you have transformed to. Does so by assumming a
         linear extrapolation to zero.
         Original author: Jack Carpenter
 
         :param xin: domain vector for space to be transformed from
         :type xin: numpy.array or list
         :param yin: range vector for space to be transformed from
@@ -51,16 +50,15 @@
         :param xout: domain vector for space to be transformed to
         :type xout: numpy.array or list
         :param yin: range vector for space to be transformed to
         :type yin: numpy.array or list
         :return: range vector for space transformed to with correction applied
         :rtype: numpy.array
         """
-        """
-        TODO: Refactor correction to just
+        """TODO: Refactor correction to just
         1) peform linear extrapolation in space before transform
         2) transform with extrapolated function
         Compare that implementation to this one.
         Replace this if equal (within tolerance)
         """
 
         lorch_flag = kwargs.get('lorch', False)
@@ -99,16 +97,15 @@
             correction[i] = (2 / np.pi) * (factor - F2)
 
         yout += correction
 
         return yout
 
     def apply_cropping(self, x, y, xmin, xmax, dy=None):
-        """
-        Utility to crop x and y based on xmin and xmax along x.
+        """Utility to crop x and y based on xmin and xmax along x.
         Provides the capability to specify the (Qmin,Qmax)
         or (Rmin,Rmax) in the Fourier transform
 
         :param x: domain vector
         :type x: numpy.array or list
         :param y: range vector
         :type y: numpy.array or list
@@ -132,16 +129,15 @@
                           xin,
                           yin,
                           xout,
                           xmin=None,
                           xmax=None,
                           dyin=None,
                           **kwargs):
-        """
-        The Fourier transform function. The kwargs
+        """The Fourier transform function. The kwargs
         argument allows for different modifications:
         Lorch dampening, omitted low-x range correction,
 
         :param xin: domain vector for space to be transformed from
         :type xin: numpy.array or list
         :param yin: range vector for space to be transformed from
         :type yin: numpy.array or list
@@ -185,16 +181,15 @@
             self._low_x_correction(xin, yin, xout, yout, **kwargs)
 
         return xout, yout, eout
 
     # Reciprocal -> Real Space Transforms  #
 
     def F_to_G(self, q, fq, r, dfq=None, **kwargs):
-        """
-        Transforms from reciprocal space :math:`Q[S(Q)-1]`
+        """Transforms from reciprocal space :math:`Q[S(Q)-1]`
         to real space :math:`G_{PDFFIT}(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq: :math:`Q[S(Q)-1]` vector
         :type fq: numpy.array or list
         :param r: :math:`r`-space vector
@@ -207,16 +202,15 @@
         """
         r, gr, dgr = self.fourier_transform(q, fq, r, dyin=dfq, **kwargs)
         gr *= 2. / np.pi
         dgr *= 2. / np.pi
         return r, gr, dgr
 
     def F_to_GK(self, q, fq, r, dfq=None, **kwargs):
-        """
-        Transforms from reciprocal space :math:`Q[S(Q)-1]`
+        """Transforms from reciprocal space :math:`Q[S(Q)-1]`
         to real space :math:`G_{Keen Version}(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq: :math:`Q[S(Q)-1]` vector
         :type fq: numpy.array or list
         :param r: :math:`r`-space vector
@@ -228,16 +222,15 @@
         :rtype: numpy.array, numpy.array, numpy.array
         """
         r, gr, dgr = self.F_to_G(q, fq, r, dfq, **kwargs)
         gr, dgr = self.converter.G_to_GK(r, gr, dgr, **kwargs)
         return r, gr, dgr
 
     def F_to_g(self, q, fq, r, dfq=None, **kwargs):
-        """
-        Transforms from reciprocal space :math:`Q[S(Q)-1]`
+        """Transforms from reciprocal space :math:`Q[S(Q)-1]`
         to real space :math:`g(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq: :math:`Q[S(Q)-1]` vector
         :type fq: numpy.array or list
         :param r: :math:`r`-space vector
@@ -250,16 +243,15 @@
         """
         r, gr, dgr = self.F_to_G(q, fq, r, dfq, **kwargs)
         gr, dgr = self.converter.G_to_g(r, gr, dgr, **kwargs)
         return r, gr, dgr
 
     # S(Q)
     def S_to_G(self, q, sq, r, dsq=None, **kwargs):
-        """
-        Transforms from reciprocal space :math:`S(Q)`
+        """Transforms from reciprocal space :math:`S(Q)`
         to real space :math:`G_{PDFFIT}(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param sq: :math:`S(Q)` vector
         :type sq: numpy.array or list
         :param r: :math:`r`-space vector
@@ -270,16 +262,15 @@
         :return: :math:`r`, :math:`G_{PDFFIT}(r)`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         fq, dfq = self.converter.S_to_F(q, sq, dsq)
         return self.F_to_G(q, fq, r, dfq, **kwargs)
 
     def S_to_GK(self, q, sq, r, dsq=None, **kwargs):
-        """
-        Transforms from reciprocal space :math:`S(Q)`
+        """Transforms from reciprocal space :math:`S(Q)`
         to real space :math:`G_{Keen Version}(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param sq: :math:`S(Q)` vector
         :type sq: numpy.array or list
         :param r: :math:`r`-space vector
@@ -290,16 +281,15 @@
         :return: :math:`r`, :math:`G_{Keen Version}(r)`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         fq, dfq = self.converter.S_to_F(q, sq, dsq)
         return self.F_to_GK(q, fq, r, dfq, **kwargs)
 
     def S_to_g(self, q, sq, r, dsq=None, **kwargs):
-        """
-        Transforms from reciprocal space :math:`S(Q)`
+        """Transforms from reciprocal space :math:`S(Q)`
         to real space :math:`g(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param sq: :math:`S(Q)` vector
         :type sq: numpy.array or list
         :param r: :math:`r`-space vector
@@ -311,16 +301,15 @@
         :rtype: numpy.array, numpy.array, numpy.array
         """
         fq, dfq = self.converter.S_to_F(q, sq, dsq)
         return self.F_to_g(q, fq, r, dfq, **kwargs)
 
     # Keen's F(Q)
     def FK_to_G(self, q, fq_keen, r, dfq_keen=None, **kwargs):
-        """
-        Transforms from reciprocal space :math:`F(Q)`
+        """Transforms from reciprocal space :math:`F(Q)`
         to real space :math:`G_{PDFFIT}(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq_keen: :math:`F(Q)` vector
         :type fq_keen: numpy.array or list
         :param r: :math:`r`-space vector
@@ -331,16 +320,15 @@
         :return: :math:`r`, :math:`G_{PDFFIT}(r)`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         fq, dfq = self.converter.FK_to_F(q, fq_keen, dfq_keen, **kwargs)
         return self.F_to_G(q, fq, r, dfq, **kwargs)
 
     def FK_to_GK(self, q, fq_keen, r, dfq_keen=None, **kwargs):
-        """
-        Transforms from reciprocal space :math:`F(Q)`
+        """Transforms from reciprocal space :math:`F(Q)`
         to real space :math:`G_{Keen Version}(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq_keen: :math:`F(Q)` vector
         :type fq_keen: numpy.array or list
         :param r: :math:`r`-space vector
@@ -351,16 +339,15 @@
         :return: :math:`r`, :math:`G_{Keen Version}(r)`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         fq, dfq = self.converter.FK_to_F(q, fq_keen, dfq_keen, **kwargs)
         return self.F_to_GK(q, fq, r, dfq, **kwargs)
 
     def FK_to_g(self, q, fq_keen, r, dfq_keen=None, **kwargs):
-        """
-        Transforms from reciprocal space :math:`F(Q)`
+        """Transforms from reciprocal space :math:`F(Q)`
         to real space :math:`g(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param fq_keen: :math:`F(Q)` vector
         :type fq_keen: numpy.array or list
         :param r: :math:`r`-space vector
@@ -372,16 +359,15 @@
         :rtype: numpy.array, numpy.array, numpy.array
         """
         fq, dfq = self.converter.FK_to_F(q, fq_keen, dfq_keen, **kwargs)
         return self.F_to_g(q, fq, r, dfq, **kwargs)
 
     # Differential cross-section = d_simga / d_Omega
     def DCS_to_G(self, q, dcs, r, ddcs=None, **kwargs):
-        """
-        Transforms from reciprocal space
+        """Transforms from reciprocal space
         :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
         to real space :math:`G_{PDFFIT}(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param dcs: :math:`\\frac{d \\sigma}{d \\Omega}(Q)` vector
         :type dcs: numpy.array or list
@@ -393,16 +379,15 @@
         :return: :math:`r`, :math:`G_{PDFFIT}(r)`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         fq, dfq = self.converter.DCS_to_F(q, dcs, ddcs, **kwargs)
         return self.F_to_G(q, fq, r, dfq, **kwargs)
 
     def DCS_to_GK(self, q, dcs, r, ddcs=None, **kwargs):
-        """
-        Transforms from reciprocal space
+        """Transforms from reciprocal space
         :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
         to real space :math:`G_{Keen Version}(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param dcs: :math:`\\frac{d \\sigma}{d \\Omega}(Q)` vector
         :type dcs: numpy.array or list
@@ -414,16 +399,15 @@
         :return: :math:`r`, :math:`G_{Keen Version}(r)`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         fq, dfq = self.converter.DCS_to_F(q, dcs, ddcs, **kwargs)
         return self.F_to_GK(q, fq, r, dfq, **kwargs)
 
     def DCS_to_g(self, q, dcs, r, ddcs=None, **kwargs):
-        """
-        Transforms from reciprocal space
+        """Transforms from reciprocal space
         :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
         to real space :math:`g(r)`
 
         :param q: :math:`Q`-space vector
         :type q: numpy.array or list
         :param dcs: :math:`\\frac{d \\sigma}{d \\Omega}(Q)` vector
         :type dcs: numpy.array or list
@@ -438,16 +422,15 @@
         fq, dfq = self.converter.DCS_to_F(q, dcs, ddcs, **kwargs)
         return self.F_to_g(q, fq, r, dfq, **kwargs)
 
     # Real -> Reciprocal Space Transforms  #
 
     # G(R) = PDF
     def G_to_F(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`G_{PDFFIT}(r)`
+        """Transforms from real space :math:`G_{PDFFIT}(r)`
         to reciprocal space :math:`Q[S(Q)-1]`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{PDFFIT}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -457,16 +440,15 @@
 
         :return: :math:`Q`, :math:`Q[S(Q)-1]`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         return self.fourier_transform(r, gr, q, dyin=dgr, **kwargs)
 
     def G_to_S(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`G_{PDFFIT}(r)`
+        """Transforms from real space :math:`G_{PDFFIT}(r)`
         to reciprocal space :math:`S(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{PDFFIT}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -478,16 +460,15 @@
         :rtype: numpy.array, numpy.array, numpy.array
         """
         q, fq, dfq = self.G_to_F(r, gr, q, dgr=dgr, **kwargs)
         sq, dsq = self.converter.F_to_S(q, fq, dfq=dfq)
         return q, sq, dsq
 
     def G_to_FK(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`G_{PDFFIT}(r)`
+        """Transforms from real space :math:`G_{PDFFIT}(r)`
         to reciprocal space :math:`F(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{PDFFIT}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -499,16 +480,15 @@
         :rtype: numpy.array, numpy.array, numpy.array
         """
         q, fq, dfq = self.G_to_F(r, gr, q, dgr=dgr, **kwargs)
         fq, dfq = self.converter.F_to_FK(q, fq, dfq=dfq, **kwargs)
         return q, fq, dfq
 
     def G_to_DCS(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`G_{PDFFIT}(r)`
+        """Transforms from real space :math:`G_{PDFFIT}(r)`
         to reciprocal space
         :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{PDFFIT}(r)` vector
         :type gr: numpy.array or list
@@ -523,16 +503,15 @@
         """
         q, fq, dfq = self.G_to_F(r, gr, q, dgr=dgr, **kwargs)
         dcs, ddcs = self.converter.F_to_DCS(q, fq, dfq=dfq, **kwargs)
         return q, dcs, ddcs
 
     # Keen's G(r)
     def GK_to_F(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`G_{Keen Version}(r)`
+        """Transforms from real space :math:`G_{Keen Version}(r)`
         to reciprocal space :math:`Q[S(Q)-1]`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{Keen Version}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -543,16 +522,15 @@
         :return: :math:`Q`, :math:`Q[S(Q)-1]`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         _gr, _dgr = self.converter.GK_to_G(r, gr, dgr=dgr, **kwargs)
         return self.G_to_F(r, _gr, q, dgr=_dgr, **kwargs)
 
     def GK_to_S(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`G_{Keen Version}(r)`
+        """Transforms from real space :math:`G_{Keen Version}(r)`
         to reciprocal space :math:`S(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{Keen Version}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -563,16 +541,15 @@
         :return: :math:`Q`, :math:`S(Q)`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         _gr, _dgr = self.converter.GK_to_G(r, gr, dgr=dgr, **kwargs)
         return self.G_to_S(r, _gr, q, dgr=_dgr, **kwargs)
 
     def GK_to_FK(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`G_{Keen Version}(r)`
+        """Transforms from real space :math:`G_{Keen Version}(r)`
         to reciprocal space :math:`F(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{Keen Version}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -583,16 +560,15 @@
         :return: :math:`Q`, :math:`F(Q)`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         _gr, _dgr = self.converter.GK_to_G(r, gr, dgr=dgr, **kwargs)
         return self.G_to_FK(r, _gr, q, dgr=_dgr, **kwargs)
 
     def GK_to_DCS(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`G_{Keen Version}(r)`
+        """Transforms from real space :math:`G_{Keen Version}(r)`
         to reciprocal space :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`G_{Keen Version}(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -605,16 +581,15 @@
         :rtype: numpy.array, numpy.array, numpy.array
         """
         _gr, _dgr = self.converter.GK_to_G(r, gr, dgr=dgr, **kwargs)
         return self.G_to_DCS(r, _gr, q, dgr=_dgr, **kwargs)
 
     # g(r)
     def g_to_F(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`g(r)`
+        """Transforms from real space :math:`g(r)`
         to reciprocal space :math:`Q[S(Q)-1]`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`g(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -625,16 +600,15 @@
         :return: :math:`Q`, :math:`Q[S(Q)-1]`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         _gr, _dgr = self.converter.g_to_G(r, gr, dgr=dgr, **kwargs)
         return self.G_to_F(r, _gr, q, dgr=_dgr, **kwargs)
 
     def g_to_S(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`g(r)`
+        """Transforms from real space :math:`g(r)`
         to reciprocal space :math:`S(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`g(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -645,16 +619,15 @@
         :return: :math:`Q`, :math:`S(Q)`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         _gr, _dgr = self.converter.g_to_G(r, gr, dgr=dgr, **kwargs)
         return self.G_to_S(r, _gr, q, dgr=_dgr, **kwargs)
 
     def g_to_FK(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`g(r)`
+        """Transforms from real space :math:`g(r)`
         to reciprocal space :math:`F(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`g(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
@@ -665,16 +638,15 @@
         :return: :math:`Q`, :math:`F(Q)`, and uncertainties
         :rtype: numpy.array, numpy.array, numpy.array
         """
         _gr, _dgr = self.converter.g_to_G(r, gr, dgr=dgr, **kwargs)
         return self.G_to_FK(r, _gr, q, dgr=_dgr, **kwargs)
 
     def g_to_DCS(self, r, gr, q, dgr=None, **kwargs):
-        """
-        Transforms from real space :math:`g(r)`
+        """Transforms from real space :math:`g(r)`
         to reciprocal space :math:`\\frac{d \\sigma}{d \\Omega}(Q)`
 
         :param r: :math:`r`-space vector
         :type r: numpy.array or list
         :param gr: :math:`g(r)` vector
         :type gr: numpy.array or list
         :param q: :math:`Q`-space vector
```

### Comparing `pystog-0.4.0/pystog/utils.py` & `pystog-1.0.0/pystog/utils.py`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/pystog.egg-info/PKG-INFO` & `pystog-1.0.0/pystog.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: pystog
-Version: 0.4.0
+Version: 1.0.0
 Summary: Manipulate total scattering functions
 Home-page: https://github.com/neutrons/pystog
 Author: Marshall McDonnell (marshallmcdonnell),Mathieu Doucet (mdoucet),Ross Whitfield (rosswhitfield),Pete Peterson (peterfpeterson),Yuanpeng Zhang (Kvieta1990)
 Author-email: mcdonnellmt@ornl.gov
 License: GPL License (version 3)
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
```

### Comparing `pystog-0.4.0/pystog.egg-info/SOURCES.txt` & `pystog-1.0.0/pystog.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-LICENSE
 MANIFEST.in
 README.md
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 pystog/__init__.py
 pystog/_version.py
 pystog/cli.py
 pystog/converter.py
 pystog/fourier_filter.py
 pystog/io.py
-pystog/pre_proc.py
 pystog/stog.py
 pystog/transformer.py
 pystog/utils.py
 pystog.egg-info/PKG-INFO
 pystog.egg-info/SOURCES.txt
 pystog.egg-info/dependency_links.txt
 pystog.egg-info/entry_points.txt
 pystog.egg-info/requires.txt
 pystog.egg-info/top_level.txt
 tests/__init__.py
 tests/create_test_files.py
 tests/materials.py
-tests/test_cli.py
+tests/runner.py
 tests/test_converter.py
 tests/test_fourier_filter.py
-tests/test_io.py
 tests/test_stog.py
 tests/test_transformer.py
 tests/utils.py
 tests/test_data/__init__.py
 tests/test_data/argon.gr
 tests/test_data/argon.real_space.dat
 tests/test_data/argon.reciprocal_space.dat
```

### Comparing `pystog-0.4.0/setup.py` & `pystog-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,10 +60,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
             "pystog_cli = pystog.cli:pystog_cli",
+            "transformer_cli = pystog.cli:transformer_cli"
         ]
     }
 )
```

### Comparing `pystog-0.4.0/tests/create_test_files.py` & `pystog-1.0.0/tests/create_test_files.py`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/tests/materials.py` & `pystog-1.0.0/tests/materials.py`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/tests/test_converter.py` & `pystog-1.0.0/tests/test_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -276,45 +276,27 @@
         assert_allclose(
             sq[self.first:self.last],
             self.sq_target,
             rtol=self.rtol,
             atol=self.atol)
         assert_allclose(dsq, np.ones_like(self.q) / self.q)
 
-    def F_to_S_with_no_dfq(self):
-        sq, dsq = self.converter.F_to_S(self.q, self.fq, **self.kwargs)
-        assert_allclose(
-            sq[self.first:self.last],
-            self.sq_target,
-            rtol=self.rtol,
-            atol=self.atol)
-        assert_allclose(dsq, np.zeros_like(dsq))
-
     def F_to_FK(self):
-        fq_keen, dfq_keen = self.converter.F_to_FK(
-            self.q, self.fq, np.ones_like(self.q), **self.kwargs)
+        fq_keen, dfq_keen = self.converter.F_to_FK(self.q, self.fq,
+                                                   np.ones_like(self.q),
+                                                   **self.kwargs)
         assert_allclose(
             fq_keen[self.first:self.last],
             self.fq_keen_target,
             rtol=self.rtol,
             atol=self.atol)
         assert_allclose(
             dfq_keen,
             np.ones_like(self.q) * self.kwargs['<b_coh>^2'] / self.q)
 
-    def F_to_FK_with_no_dfq(self):
-        fq_keen, dfq_keen = self.converter.F_to_FK(
-            self.q, self.fq, **self.kwargs)
-        assert_allclose(
-            fq_keen[self.first:self.last],
-            self.fq_keen_target,
-            rtol=self.rtol,
-            atol=self.atol)
-        assert_allclose(dfq_keen, np.zeros_like(dfq_keen))
-
     def F_to_DCS(self):
         dcs, ddcs = self.converter.F_to_DCS(self.q, self.fq,
                                             np.ones_like(self.q),
                                             **self.kwargs)
         assert_allclose(
             dcs[self.first:self.last],
             self.dcs_target,
@@ -409,23 +391,17 @@
 
     def test_S_to_DCS(self):
         self.S_to_DCS()
 
     def test_F_to_S(self):
         self.F_to_S()
 
-    def test_F_to_S_with_no_dfq(self):
-        self.F_to_S_with_no_dfq()
-
     def test_F_to_FK(self):
         self.F_to_FK()
 
-    def test_F_to_FK_with_no_dfq(self):
-        self.F_to_FK_with_no_dfq()
-
     def test_F_to_DCS(self):
         self.F_to_DCS()
 
     def test_FK_to_S(self):
         self.FK_to_S()
 
     def test_FK_to_F(self):
@@ -458,23 +434,17 @@
 
     def test_S_to_DCS(self):
         self.S_to_DCS()
 
     def test_F_to_S(self):
         self.F_to_S()
 
-    def test_F_to_S_with_no_dfq(self):
-        self.F_to_S_with_no_dfq()
-
     def test_F_to_FK(self):
         self.F_to_FK()
 
-    def test_F_to_FK_with_no_dfq(self):
-        self.F_to_FK_with_no_dfq()
-
     def test_F_to_DCS(self):
         self.F_to_DCS()
 
     def test_FK_to_S(self):
         self.FK_to_S()
 
     def test_FK_to_F(self):
```

### Comparing `pystog-0.4.0/tests/test_data/argon.gr` & `pystog-1.0.0/tests/test_data/argon.gr`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/tests/test_data/argon.real_space.dat` & `pystog-1.0.0/tests/test_data/argon.real_space.dat`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/tests/test_data/argon.reciprocal_space.dat` & `pystog-1.0.0/tests/test_data/argon.reciprocal_space.dat`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/tests/test_data/nickel.gr` & `pystog-1.0.0/tests/test_data/nickel.gr`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/tests/test_data/nickel.real_space.dat` & `pystog-1.0.0/tests/test_data/nickel.real_space.dat`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/tests/test_data/nickel.reciprocal_space.dat` & `pystog-1.0.0/tests/test_data/nickel.reciprocal_space.dat`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/tests/test_fourier_filter.py` & `pystog-1.0.0/tests/test_fourier_filter.py`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/tests/test_stog.py` & `pystog-1.0.0/tests/test_stog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 import numpy as np
+import pandas as pd
+from numpy.testing import assert_allclose
+
 import os
+import sys
+from tests.utils import \
+    get_data_path, load_data, get_index_of_function
+from tests.materials import Argon
+from pystog.utils import \
+    RealSpaceHeaders, ReciprocalSpaceHeaders
+from pystog.stog import StoG
+
 import tempfile
 import unittest
+if sys.version_info >= (3, 3):
+    from unittest.mock import patch
+else:
+    from mock import patch
 
-from tests.utils import get_data_path, get_index_of_function, load_data
-from tests.materials import Argon
-from pystog.utils import RealSpaceHeaders, ReciprocalSpaceHeaders
-from pystog.stog import NoInputFilesException, StoG
+
+# Real Space Function
 
 
 class TestStogBase(unittest.TestCase):
     rtol = 1.0
     atol = 1.0
 
     def initialize_material(self):
@@ -19,28 +32,25 @@
 
         # setup the tolerance
         self.first = self.material.reciprocal_space_first
         self.last = self.material.reciprocal_space_last
 
         data = load_data(self.material.reciprocal_space_filename)
         self.q = data[:, get_index_of_function("Q", ReciprocalSpaceHeaders)]
-        self.sq = data[:, get_index_of_function("S(Q)", ReciprocalSpaceHeaders)]
-        self.fq = data[
-            :, get_index_of_function("Q[S(Q)-1]", ReciprocalSpaceHeaders)
-        ]
-        self.fq_keen = data[
-            :, get_index_of_function("FK(Q)", ReciprocalSpaceHeaders)
-        ]
-        self.dcs = data[
-            :, get_index_of_function("DCS(Q)", ReciprocalSpaceHeaders)
-        ]
+        self.sq = data[:, get_index_of_function(
+            "S(Q)", ReciprocalSpaceHeaders)]
+        self.fq = data[:, get_index_of_function(
+            "Q[S(Q)-1]", ReciprocalSpaceHeaders)]
+        self.fq_keen = data[:, get_index_of_function(
+            "FK(Q)", ReciprocalSpaceHeaders)]
+        self.dcs = data[:, get_index_of_function(
+            "DCS(Q)", ReciprocalSpaceHeaders)]
 
         # targets for 1st peaks
         self.sq_target = self.material.sq_target
-        self.dsq_target = 3.087955
         self.fq_target = self.material.fq_target
         self.fq_keen_target = self.material.fq_keen_target
         self.dcs_target = self.material.dcs_target
 
         # setup the first, last indices
         self.real_space_first = self.material.real_space_first
         self.real_space_last = self.material.real_space_last
@@ -68,45 +78,54 @@
         self.material = Argon()
         self.initialize_material()
 
         self.real_xtarget = 3.525
         self.reciprocal_xtarget = 1.94
         self.fourier_filter_cutoff = 1.5
 
-        filename = get_data_path(self.material.reciprocal_space_filename)
+        filename = self.material.reciprocal_space_filename
         self.kwargs_for_files = {
-            "Files": [
+            'Files': [
                 {
-                    "Filename": filename,
-                    "ReciprocalFunction": "S(Q)",
-                    "Qmin": 0.02,
-                    "Qmax": 15.0,
-                    "Y": {"Offset": 0.0, "Scale": 1.0},
-                    "X": {"Offset": 0.0},
+                    'Filename': get_data_path(filename),
+                    'ReciprocalFunction': 'S(Q)',
+                    'Qmin': 0.02,
+                    'Qmax': 15.0,
+                    'Y': {
+                        'Offset': 0.0,
+                        'Scale': 1.0
+                    },
+                    'X': {
+                        'Offset': 0.0
+                    }
                 },
                 {
-                    "Filename": filename,
-                    "ReciprocalFunction": "S(Q)",
-                    "Qmin": 1.90,
-                    "Qmax": 35.2,
-                    "Y": {"Offset": 0.0, "Scale": 1.0},
-                    "X": {"Offset": 0.0},
-                },
+                    'Filename':
+                        get_data_path(self.material.reciprocal_space_filename),
+                    'ReciprocalFunction': 'S(Q)',
+                    'Qmin': 1.90,
+                    'Qmax': 35.2,
+                    'Y': {
+                        'Offset': 0.0,
+                        'Scale': 1.0},
+                    'X': {
+                        'Offset': 0.0}
+                }
             ]
         }
 
         self.kwargs_for_stog_input = {
-            "NumberDensity": self.material.kwargs["rho"],
-            "<b_coh>^2": self.material.kwargs["<b_coh>^2"],
-            "<b_tot^2>": self.material.kwargs["<b_tot^2>"],
-            "FourierFilter": {"Cutoff": self.fourier_filter_cutoff},
-            "OmittedXrangeCorrection": False,
-            "Rdelta": self.r[1] - self.r[0],
-            "Rmin": min(self.r),
-            "Rmax": max(self.r),
+            'NumberDensity': self.material.kwargs['rho'],
+            '<b_coh>^2': self.material.kwargs['<b_coh>^2'],
+            '<b_tot^2>': self.material.kwargs['<b_tot^2>'],
+            'FourierFilter': {'Cutoff': self.fourier_filter_cutoff},
+            'OmittedXrangeCorrection': False,
+            'Rdelta': self.r[1] - self.r[0],
+            'Rmin': min(self.r),
+            'Rmax': max(self.r)
         }
 
     def tearDown(self):
         unittest.TestCase.tearDown(self)
 
 
 class TestStogInit(TestStogBase):
@@ -134,89 +153,101 @@
         self.assertEqual(stog.rdelta, 0.01)
         self.assertEqual(stog.density, 1.0)
         self.assertEqual(stog.bcoh_sqrd, 1.0)
         self.assertEqual(stog.btot_sqrd, 1.0)
         self.assertEqual(stog.low_q_correction, False)
         self.assertEqual(stog.lorch_flag, False)
         self.assertEqual(stog.fourier_filter_cutoff, None)
-        self.assertEqual(stog.merged_opts, {"Y": {"Offset": 0.0, "Scale": 1.0}})
+        self.assertEqual(stog.plot_flag, True)
+        self.assertEqual(stog.plotting_kwargs, {'figsize': (16, 8),
+                                                'style': '-',
+                                                'ms': 1,
+                                                'lw': 1,
+                                                }
+                         )
+        self.assertEqual(
+            stog.merged_opts, {
+                "Y": {
+                    "Offset": 0.0, "Scale": 1.0}})
         self.assertEqual(stog.stem_name, "out")
-        self.assertEqual(stog.reciprocal_individuals.size, 0)
-        self.assertEqual(stog.q_master, {})
-        self.assertEqual(stog.sq_master, {})
-        self.assertEqual(stog.sq_individuals.size, 0)
-        self.assertEqual(stog.r_master, {})
-        self.assertEqual(stog.gr_master, {})
+        self.assertTrue(stog.df_individuals.empty)
+        self.assertTrue(stog.df_sq_master.empty)
+        self.assertTrue(stog.df_sq_individuals.empty)
+        self.assertTrue(stog.df_gr_master.empty)
 
     def test_stog_init_kwargs_files(self):
-        stog = StoG(**{"Files": ["file1.txt", "file2.txt"]})
-        self.assertEqual(stog.files, ["file1.txt", "file2.txt"])
+        stog = StoG(**{'Files': ['file1.txt', 'file2.txt']})
+        self.assertEqual(stog.files, ['file1.txt', 'file2.txt'])
 
     def test_stog_init_kwargs_real_space_function(self):
-        stog = StoG(**{"RealSpaceFunction": "G(r)"})
-        self.assertEqual(stog.real_space_function, "G(r)")
+        stog = StoG(**{'RealSpaceFunction': 'G(r)'})
+        self.assertEqual(stog.real_space_function, 'G(r)')
 
     def test_stog_init_kwargs_rmin(self):
-        stog = StoG(**{"Rmin": 2.0})
+        stog = StoG(**{'Rmin': 2.0})
         self.assertEqual(stog.rmin, 2.0)
 
     def test_stog_init_kwargs_rmax(self):
-        stog = StoG(**{"Rmax": 25.0})
+        stog = StoG(**{'Rmax': 25.0})
         self.assertEqual(stog.rmax, 25.0)
 
     def test_stog_init_kwargs_rdelta(self):
-        stog = StoG(**{"Rdelta": 0.5})
+        stog = StoG(**{'Rdelta': 0.5})
         self.assertEqual(stog.rdelta, 0.5)
 
     def test_stog_init_kwargs_rpoints(self):
-        stog = StoG(**{"Rpoints": 250})
+        stog = StoG(**{'Rpoints': 250})
         self.assertEqual(stog.rdelta, 0.2)
 
     def test_stog_init_kwargs_density(self):
-        stog = StoG(**{"NumberDensity": 2.0})
+        stog = StoG(**{'NumberDensity': 2.0})
         self.assertEqual(stog.density, 2.0)
 
     def test_stog_init_kwargs_low_q_correction(self):
-        stog = StoG(**{"OmittedXrangeCorrection": True})
+        stog = StoG(**{'OmittedXrangeCorrection': True})
         self.assertEqual(stog.low_q_correction, True)
 
     def test_stog_init_kwargs_lorch_flag(self):
-        stog = StoG(**{"LorchFlag": True})
+        stog = StoG(**{'LorchFlag': True})
         self.assertEqual(stog.lorch_flag, True)
 
     def test_stog_init_kwargs_fourier_filter_cutoff(self):
-        stog = StoG(**{"FourierFilter": {"Cutoff": 1.0}})
+        stog = StoG(**{'FourierFilter': {'Cutoff': 1.0}})
         self.assertEqual(stog.fourier_filter_cutoff, 1.0)
 
+    def test_stog_init_kwargs_plot_flag(self):
+        stog = StoG(**{'PlotFlag': False})
+        self.assertEqual(stog.plot_flag, False)
+
     def test_stog_init_kwargs_bcoh_sqrd(self):
-        stog = StoG(**{"<b_coh>^2": 0.5})
+        stog = StoG(**{'<b_coh>^2': 0.5})
         self.assertEqual(stog.bcoh_sqrd, 0.5)
 
     def test_stog_init_kwargs_btot_sqrd(self):
-        stog = StoG(**{"<b_tot^2>": 0.75})
+        stog = StoG(**{'<b_tot^2>': 0.75})
         self.assertEqual(stog.btot_sqrd, 0.75)
 
     def test_stog_init_kwargs_qmin_only(self):
-        stog = StoG(**{"Merging": {"Transform": {"Qmin": 0.5}}})
+        stog = StoG(**{'Merging': {'Transform': {'Qmin': 0.5}}})
         self.assertEqual(stog.qmin, 0.5)
         self.assertEqual(stog.qmax, None)
 
     def test_stog_init_kwargs_qmax_only(self):
-        stog = StoG(**{"Merging": {"Transform": {"Qmax": 30.0}}})
+        stog = StoG(**{'Merging': {'Transform': {'Qmax': 30.0}}})
         self.assertEqual(stog.qmin, None)
         self.assertEqual(stog.qmax, 30.0)
 
     def test_stog_init_kwargs_qmin_and_qmax(self):
-        stog = StoG(**{"Merging": {"Transform": {"Qmin": 0.5, "Qmax": 30.0}}})
+        stog = StoG(**{'Merging': {'Transform': {'Qmin': 0.5, 'Qmax': 30.0}}})
         self.assertEqual(stog.qmin, 0.5)
         self.assertEqual(stog.qmax, 30.0)
 
     def test_stog_init_kwargs_output_stem_name(self):
-        stog = StoG(**{"Outputs": {"StemName": "myName"}})
-        self.assertEqual(stog.stem_name, "myName")
+        stog = StoG(**{'Outputs': {'StemName': 'myName'}})
+        self.assertEqual(stog.stem_name, 'myName')
 
 
 class TestStogAttributes(TestStogBase):
     def setUp(self):
         super(TestStogAttributes, self).setUp()
 
     def test_stog_xmin_setter(self):
@@ -296,1019 +327,915 @@
         stog.real_space_function = "GK(r)"
         self.assertEqual(stog.real_space_function, "GK(r)")
         self.assertEqual(stog.gr_title, "GK(r) Merged")
         self.assertEqual(stog.real_space_function, "GK(r)")
         self.assertEqual(stog.gr_ft_title, "GK(r) FT")
         self.assertEqual(stog.gr_lorch_title, "GK(r) FT Lorched")
 
+    def test_stog_plotting_kwargs_setter(self):
+        stog = StoG()
+        new_kwargs = {
+            'figsize': (4, 4),
+            'style': 'o',
+            'ms': 2,
+            'lw': 2,
+        }
+        stog.plotting_kwargs = new_kwargs
+        self.assertEqual(stog.plotting_kwargs, new_kwargs)
+
     def test_stog_low_q_correction_exception(self):
         stog = StoG()
         with self.assertRaises(TypeError):
             stog.low_q_correction = 1.0
 
     def test_stog_lorch_flag_exception(self):
         stog = StoG()
         with self.assertRaises(TypeError):
             stog.lorch_flag = 1.0
 
+    def test_stog_plot_flag_exception(self):
+        stog = StoG()
+        with self.assertRaises(TypeError):
+            stog.plot_flag = 1.0
+
     def test_stog_real_space_function_exception(self):
         stog = StoG()
         with self.assertRaises(ValueError):
             stog.real_space_function = "Dog"
 
 
-class TestStogStorageArrays(TestStogBase):
+class TestStogDataFrameAttributes(TestStogBase):
     def setUp(self):
-        super(TestStogStorageArrays, self).setUp()
-        self.target = np.random.randn(3, 10)
+        super(TestStogDataFrameAttributes, self).setUp()
+        self.df_target = pd.DataFrame(np.random.randn(10, 2),
+                                      index=np.arange(10),
+                                      columns=list('XY'))
 
-    def test_stog_reciprocal_individuals_setter(self):
+    def test_stog_df_individuals_setter(self):
         stog = StoG()
-        stog.reciprocal_individuals = self.target
-        np.testing.assert_allclose(stog.reciprocal_individuals, self.target)
+        stog.df_individuals = self.df_target
+        self.assertTrue(stog.df_individuals.equals(self.df_target))
 
-    def test_stog_sq_individuals_setter(self):
+    def test_stog_df_sq_individuals_setter(self):
         stog = StoG()
-        stog.sq_individuals = self.target
-        np.testing.assert_allclose(stog.sq_individuals, self.target)
+        stog.df_sq_individuals = self.df_target
+        self.assertTrue(stog.df_sq_individuals.equals(self.df_target))
 
-    def test_stog_q_master_setter(self):
+    def test_stog_df_sq_master_setter(self):
         stog = StoG()
-        stog.q_master = self.target
-        np.testing.assert_allclose(stog.q_master, self.target)
+        stog.df_sq_master = self.df_target
+        self.assertTrue(stog.df_sq_master.equals(self.df_target))
 
-    def test_stog_sq_master_setter(self):
+    def test_stog_df_gr_master_setter(self):
         stog = StoG()
-        stog.sq_master = self.target
-        np.testing.assert_allclose(stog.sq_master, self.target)
-
-    def test_stog_r_master_setter(self):
-        stog = StoG()
-        stog.r_master = self.target
-        np.testing.assert_allclose(stog.r_master, self.target)
-
-    def test_stog_gr_master_setter(self):
-        stog = StoG()
-        stog.gr_master = self.target
-        np.testing.assert_allclose(stog.gr_master, self.target)
+        stog.df_gr_master = self.df_target
+        self.assertTrue(stog.df_gr_master.equals(self.df_target))
 
 
 class TestStogGeneralMethods(TestStogBase):
     def setUp(self):
         super(TestStogGeneralMethods, self).setUp()
 
     def test_stog_append_file(self):
-        stog = StoG(**{"Files": ["file1.txt", "file2.txt"]})
-        stog.append_file("file3.txt")
-        self.assertEqual(stog.files, ["file1.txt", "file2.txt", "file3.txt"])
+        stog = StoG(**{'Files': ['file1.txt', 'file2.txt']})
+        stog.append_file('file3.txt')
+        self.assertEqual(stog.files, ['file1.txt', 'file2.txt', 'file3.txt'])
 
     def test_stog_extend_file_list(self):
-        stog = StoG(**{"Files": ["file1.txt", "file2.txt"]})
-        stog.extend_file_list(["file3.txt", "file4.txt"])
+        stog = StoG(**{'Files': ['file1.txt', 'file2.txt']})
+        stog.extend_file_list(['file3.txt', 'file4.txt'])
         self.assertEqual(
-            stog.files, ["file1.txt", "file2.txt", "file3.txt", "file4.txt"]
-        )
+            stog.files, [
+                'file1.txt', 'file2.txt', 'file3.txt', 'file4.txt'])
 
 
 class TestStogDatasetSpecificMethods(TestStogBase):
     def setUp(self):
         super(TestStogDatasetSpecificMethods, self).setUp()
 
-    def test_stog_apply_scales_and_offset(self):
-        q, sq, dq = StoG.apply_scales_and_offset(self.q, self.sq)
-        np.testing.assert_allclose(q, self.q)
-        np.testing.assert_allclose(sq, self.sq)
-        np.testing.assert_allclose(dq, np.zeros_like(sq))
-
-    def test_stog_apply_scales_and_offset_with_dy(self):
-        q, sq, dq = StoG.apply_scales_and_offset(self.q, self.sq, dy=self.sq)
-        np.testing.assert_allclose(q, self.q)
-        np.testing.assert_allclose(sq, self.sq)
-        np.testing.assert_allclose(dq, self.sq)
-
-    def test_stog_apply_scales_and_offset_with_yscale(self):
-        q, sq, dq = StoG.apply_scales_and_offset(
-            self.q, self.sq, dy=self.sq, yscale=2.0
-        )
-        np.testing.assert_allclose(q, self.q)
-        np.testing.assert_allclose(sq, self.sq * 2.0)
-        np.testing.assert_allclose(dq, self.sq * 2.0)
-
-    def test_stog_apply_scales_and_offset_with_yoffset(self):
-        q, sq, dq = StoG.apply_scales_and_offset(
-            self.q, self.sq, dy=self.sq, yoffset=2.0
-        )
-        np.testing.assert_allclose(q, self.q)
-        np.testing.assert_allclose(sq, self.sq + 2.0)
-        np.testing.assert_allclose(dq, self.sq)
-
-    def test_stog_apply_scales_and_offset_with_xoffset(self):
-        q, sq, dq = StoG.apply_scales_and_offset(
-            self.q, self.sq, dy=self.sq, xoffset=2.0
-        )
-        np.testing.assert_allclose(q, self.q + 2.0)
-        np.testing.assert_allclose(sq, self.sq)
-        np.testing.assert_allclose(dq, self.sq)
-
     def test_stog_add_dataset(self):
         # Number of decimal places for precision
         places = 5
 
         # Initialize with material info for Argon
-        stog = StoG(
-            **{
-                "<b_coh>^2": self.kwargs["<b_coh>^2"],
-                "<b_tot^2>": self.kwargs["<b_tot^2>"],
-            }
-        )
+        stog = StoG(**{'<b_coh>^2': self.kwargs['<b_coh>^2'],
+                       '<b_tot^2>': self.kwargs['<b_tot^2>']})
 
         # Add the S(Q) data set and check values against targets
-        info = {"data": [self.q, self.sq], "ReciprocalFunction": "S(Q)"}
-        stog.add_dataset(info)
+        index = 0
+        info = {
+            'data': pd.DataFrame({'x': self.q, 'y': self.sq}),
+            'ReciprocalFunction': 'S(Q)'}
+        stog.add_dataset(info, index=index)
         self.assertEqual(
-            stog.reciprocal_individuals[0][self.first], self.reciprocal_xtarget
-        )
+            stog.df_individuals.iloc[self.first].name, self.reciprocal_xtarget)
+        self.assertAlmostEqual(
+            stog.df_individuals.iloc[self.first]['S(Q)_%d' % index],
+            self.sq_target[0],
+            places=places)
         self.assertAlmostEqual(
-            stog.reciprocal_individuals[1][self.first],
+            stog.df_sq_individuals.iloc[self.first]['S(Q)_%d' % index],
             self.sq_target[0],
-            places=places,
-        )
-        self.assertEqual(stog.reciprocal_individuals[2][self.first], 0.0)
-        self.assertAlmostEqual(
-            stog.sq_individuals[1][self.first], self.sq_target[0], places=places
-        )
-        self.assertEqual(stog.sq_individuals[2][self.first], 0.0)
+            places=places)
 
         # Add the Q[S(Q)-1] data set and check values for it and S(Q) against
         # targets
-        stride = stog.reciprocal_individuals.shape[1]
-        info = {"data": [self.q, self.fq], "ReciprocalFunction": "Q[S(Q)-1]"}
-        stog.add_dataset(info)
-
+        index = 1
+        info = {
+            'data': pd.DataFrame({'x': self.q, 'y': self.fq}),
+            'ReciprocalFunction': 'Q[S(Q)-1]'
+        }
+        stog.add_dataset(info, index=index)
         self.assertAlmostEqual(
-            stog.reciprocal_individuals[1][self.first + stride],
+            stog.df_individuals.iloc[self.first]['Q[S(Q)-1]_%d' % index],
             self.fq_target[0],
-            places=places,
-        )
-        self.assertEqual(
-            stog.reciprocal_individuals[2][self.first + stride], 0.0
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.sq_individuals[1][self.first], self.sq_target[0], places=places
-        )
-        self.assertEqual(stog.sq_individuals[2][self.first], 0.0)
+            stog.df_sq_individuals.iloc[self.first]['S(Q)_%d' % index],
+            self.sq_target[0],
+            places=places)
 
         # Add the FK(Q) data set and check values for it and S(Q) against
         # targets
-        stride = stog.reciprocal_individuals.shape[1]
-        info = {"data": [self.q, self.fq_keen], "ReciprocalFunction": "FK(Q)"}
-        stog.add_dataset(info)
+        index = 2
+        info = {
+            'data': pd.DataFrame({'x': self.q, 'y': self.fq_keen}),
+            'ReciprocalFunction': 'FK(Q)'}
+        stog.add_dataset(info, index=index)
         self.assertAlmostEqual(
-            stog.reciprocal_individuals[1][self.first + stride],
+            stog.df_individuals.iloc[self.first]['FK(Q)_%d' % index],
             self.fq_keen_target[0],
-            places=places,
-        )
-        self.assertEqual(
-            stog.reciprocal_individuals[2][self.first + stride], 0.0
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.sq_individuals[1][self.first], self.sq_target[0], places=places
-        )
-        self.assertEqual(stog.sq_individuals[2][self.first], 0.0)
+            stog.df_sq_individuals.iloc[self.first]['S(Q)_%d' % index],
+            self.sq_target[0],
+            places=places)
 
         # Add the DCS(Q) data set and check values for it and S(Q) against
         # targets
-        stride = stog.reciprocal_individuals.shape[1]
-        info = {"data": [self.q, self.dcs], "ReciprocalFunction": "DCS(Q)"}
-        stog.add_dataset(info)
+        index = 3
+        info = {
+            'data': pd.DataFrame({'x': self.q, 'y': self.dcs}),
+            'ReciprocalFunction': 'DCS(Q)'}
+        stog.add_dataset(info, index=index)
         self.assertAlmostEqual(
-            stog.reciprocal_individuals[1][self.first + stride],
+            stog.df_individuals.iloc[self.first]['DCS(Q)_%d' % index],
             self.dcs_target[0],
-            places=places,
-        )
-        self.assertEqual(
-            stog.reciprocal_individuals[2][self.first + stride], 0.0
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.sq_individuals[1][self.first], self.sq_target[0], places=places
-        )
-        self.assertEqual(stog.sq_individuals[2][self.first], 0.0)
+            stog.df_sq_individuals.iloc[self.first]['S(Q)_%d' % index],
+            self.sq_target[0],
+            places=places)
 
     def test_stog_add_dataset_yscale(self):
         # Scale S(Q) and make sure it does not equal original target values
         stog = StoG()
+        index = 0
         info = {
-            "data": [self.q, self.sq],
-            "ReciprocalFunction": "S(Q)",
-            "Y": {"Scale": 2.0},
-        }
-        stog.add_dataset(info)
+            'data': pd.DataFrame({'x': self.q, 'y': self.sq}),
+            'ReciprocalFunction': 'S(Q)',
+            'Y': {'Scale': 2.0}}
+        stog.add_dataset(info, index=index)
         self.assertNotEqual(
-            stog.reciprocal_individuals[1][self.first], self.sq_target[0]
-        )
-        self.assertEqual(stog.reciprocal_individuals[2][self.first], 0.0)
+            stog.df_individuals.iloc[self.first]['S(Q)_%d' % index],
+            self.sq_target[0])
         self.assertNotEqual(
-            stog.sq_individuals[1][self.first], self.sq_target[0]
-        )
-        self.assertEqual(stog.sq_individuals[2][self.first], 0.0)
+            stog.df_sq_individuals.iloc[self.first]['S(Q)_%d' % index],
+            self.sq_target[0])
 
     def test_stog_add_dataset_yoffset(self):
         # Offset S(Q) and make sure it does not equal original target values
         stog = StoG()
+        index = 0
         info = {
-            "data": [self.q, self.sq],
-            "ReciprocalFunction": "S(Q)",
-            "Y": {"Offset": 2.0},
-        }
-        stog.add_dataset(info)
-        self.assertNotEqual(
-            stog.reciprocal_individuals[1][self.first], self.sq_target[0]
-        )
-        self.assertEqual(stog.reciprocal_individuals[2][self.first], 0.0)
-        self.assertNotEqual(
-            stog.sq_individuals[1][self.first], self.sq_target[0]
-        )
-        self.assertEqual(stog.sq_individuals[2][self.first], 0.0)
-
-    def test_stog_add_dataset_yscale_with_dy(self):
-        # Scale S(Q) and make sure it does not equal original target values
-        stog = StoG()
-        info = {
-            "data": [self.q, self.sq, self.sq],
-            "ReciprocalFunction": "S(Q)",
-            "Y": {"Scale": 2.0},
-        }
-        stog.add_dataset(info)
-
-        self.assertNotEqual(
-            stog.reciprocal_individuals[1][self.first], self.sq_target[0]
-        )
-
-        dsq_target = info["Y"]["Scale"] * 2.59173
-        self.assertEqual(stog.reciprocal_individuals[2][self.first], dsq_target)
-
-        self.assertNotEqual(
-            stog.sq_individuals[1][self.first], self.sq_target[0]
-        )
-
-        self.assertEqual(stog.sq_individuals[2][self.first], dsq_target)
-
-    def test_stog_add_dataset_yoffset_with_dy(self):
-        # Offset S(Q) and make sure it does not equal original target values
-        stog = StoG()
-        info = {
-            "data": [self.q, self.sq, self.sq],
-            "ReciprocalFunction": "S(Q)",
-            "Y": {"Offset": 2.0},
-        }
-        stog.add_dataset(info)
-
+            'data': pd.DataFrame({'x': self.q, 'y': self.sq}),
+            'ReciprocalFunction': 'S(Q)',
+            'Y': {'Offset': 2.0}}
+        stog.add_dataset(info, index=index)
         self.assertNotEqual(
-            stog.reciprocal_individuals[1][self.first], self.sq_target[0]
-        )
-
-        dsq_target = 2.59173
-        self.assertEqual(stog.reciprocal_individuals[2][self.first], dsq_target)
-
+            stog.df_individuals.iloc[self.first]['S(Q)_%d' % index],
+            self.sq_target[0])
         self.assertNotEqual(
-            stog.sq_individuals[1][self.first], self.sq_target[0]
-        )
-
-        self.assertEqual(stog.sq_individuals[2][self.first], dsq_target)
+            stog.df_sq_individuals.iloc[self.first]['S(Q)_%d' % index],
+            self.sq_target[0])
 
     def test_stog_add_dataset_xoffset(self):
         # Offset Q from 1.96 -> 2.14
         stog = StoG()
+        index = 0
         info = {
-            "data": [self.q, self.sq],
-            "ReciprocalFunction": "S(Q)",
-            "X": {"Offset": 0.2},
-        }
-        stog.add_dataset(info)
-        self.assertEqual(stog.reciprocal_individuals[0][self.first], 2.14)
+            'data': pd.DataFrame({'x': self.q, 'y': self.sq}),
+            'ReciprocalFunction': 'S(Q)',
+            'X': {'Offset': 0.2}}
+        stog.add_dataset(info, index=index)
+        self.assertEqual(stog.df_individuals.iloc[self.first].name, 2.14)
 
     def test_stog_add_dataset_qmin_qmax_crop(self):
         # Check qmin and qmax apply cropping
         stog = StoG()
-        info = {"data": [self.q, self.sq], "ReciprocalFunction": "S(Q)"}
+        index = 0
+        info = {'data': pd.DataFrame({'x': self.q, 'y': self.sq}),
+                'ReciprocalFunction': 'S(Q)'}
         stog.qmin = 1.5
         stog.qmax = 12.0
-        stog.add_dataset(info)
-        self.assertEqual(stog.reciprocal_individuals[0][0], stog.qmin)
-        self.assertEqual(stog.reciprocal_individuals[0][-1], stog.qmax)
+        stog.add_dataset(info, index=index)
+        self.assertEqual(stog.df_individuals.iloc[0].name, stog.qmin)
+        self.assertEqual(stog.df_individuals.iloc[-1].name, stog.qmax)
 
     def test_stog_add_dataset_default_reciprocal_space_function(self):
-        # Checks the default reciprocal space function is S(Q)
-        places = 5
+        # Checks the default reciprocal space function is S(Q) and the index is
+        # set
         stog = StoG()
-        info = {"data": [self.q, self.sq]}
-        stog.add_dataset(info)
+        index = 300
+        info = {'data': pd.DataFrame({'x': self.q, 'y': self.sq})}
+        stog.add_dataset(info, index=index)
         self.assertEqual(
-            stog.reciprocal_individuals[0][self.first], self.reciprocal_xtarget
-        )
-        self.assertEqual(stog.reciprocal_individuals[2][self.first], 0.0)
-        self.assertAlmostEqual(
-            stog.reciprocal_individuals[1][self.first],
-            self.sq_target[0],
-            places=places,
-        )
-        self.assertEqual(stog.sq_individuals[2][self.first], 0.0)
+            list(
+                stog.df_individuals.columns.values), [
+                'S(Q)_%d' %
+                index])
 
     def test_stog_add_dataset_wrong_reciprocal_space_function_exception(self):
         # Check qmin and qmax apply cropping
         stog = StoG()
-        info = {"data": [self.q, self.sq], "ReciprocalFunction": "ABCDEFG(Q)"}
+        index = 0
+        info = {'data': pd.DataFrame({'x': self.q, 'y': self.sq}),
+                'ReciprocalFunction': 'ABCDEFG(Q)'}
         with self.assertRaises(ValueError):
-            stog.add_dataset(info)
-
-    def test_stog_read_nexus_file_by_bank(self):
-        stog = StoG()
-        bank = 1
-        nexus_file = "./tests/test_data/nexus/pystog_test.nxs"
-
-        stog.read_nexus_file_by_bank(nexus_file, bank, "pystog_test")
-
-        self.compareResults(
-            "./outpystog_test_bank1.dat",
-            "./tests/test_data/nexus/pystog_test_bank1.dat",
-        )
-
-    def compareResults(self, current, expected, cleanup=True):
-        output = np.loadtxt(current, unpack=True, skiprows=2)
-        expected_output = np.loadtxt(expected, unpack=True, skiprows=2)
-
-        np.allclose(output, expected_output)
-        if cleanup and os.path.exists(current):
-            os.remove(current)
-
-    def test_stog_read_all_nexus_file_by_json(self):
-        self.nexus_kwargs = {
-            "NexusFile": "./tests/test_data/nexus/pystog_test.nxs",
-            "WorkspaceName": "pystog_test",
-            "Files": [
-                {"BankNumber": "2"},
-                {"BankNumber": "3"},
-                {"BankNumber": "4"},
-                {"BankNumber": "5"},
-            ],
-            "Outputs": {"StemName": "stem_"},
-        }
-        stog = StoG(**self.nexus_kwargs)
-        stog.read_all_nexus_file_banks()
-        for i in (2, 3, 4, 5):
-            self.compareResults(
-                "./stem_pystog_test_bank{}.dat".format(i),
-                "./tests/test_data/nexus/pystog_test_bank{}.dat".format(i),
-            )
+            stog.add_dataset(info, index=index)
 
     def test_stog_read_dataset(self):
         # Number of decimal places for precision
         places = 5
 
         # Load S(Q) for Argon from test data
-        stog = StoG(
-            **{
-                "<b_coh>^2": self.kwargs["<b_coh>^2"],
-                "<b_tot^2>": self.kwargs["<b_tot^2>"],
-            }
-        )
+        stog = StoG(**{'<b_coh>^2': self.kwargs['<b_coh>^2'],
+                       '<b_tot^2>': self.kwargs['<b_tot^2>']})
         info = {
-            "Filename": get_data_path(self.material.reciprocal_space_filename),
-            "ReciprocalFunction": "S(Q)",
-            "Qmin": 0.02,
-            "Qmax": 35.2,
-            "Y": {"Offset": 0.0, "Scale": 1.0},
-            "X": {"Offset": 0.0},
-        }
+            'Filename': get_data_path(
+                self.material.reciprocal_space_filename),
+            'ReciprocalFunction': 'S(Q)',
+            'Qmin': 0.02,
+            'Qmax': 35.2,
+            'Y': {
+                'Offset': 0.0,
+                'Scale': 1.0},
+            'X': {
+                'Offset': 0.0}}
 
-        info["index"] = 0
+        info['index'] = 0
         stog.read_dataset(info)
 
         # Check S(Q) data against targets
         self.assertEqual(
-            stog.reciprocal_individuals[0][self.first], self.reciprocal_xtarget
-        )
+            stog.df_individuals.iloc[self.first].name, self.reciprocal_xtarget)
         self.assertAlmostEqual(
-            stog.reciprocal_individuals[1][self.first],
+            stog.df_individuals.iloc[self.first]['S(Q)_%d' % info['index']],
             self.sq_target[0],
-            places=places,
-        )
-        self.assertEqual(
-            stog.reciprocal_individuals[2][self.first], self.dsq_target
-        )
-        self.assertAlmostEqual(
-            stog.sq_individuals[1][self.first], self.sq_target[0], places=places
-        )
-        self.assertEqual(stog.sq_individuals[2][self.first], self.dsq_target)
-
-    def test_stog_read_dataset_xcol_data_format_exception(self):
-        stog = StoG()
-        filename = get_data_path(self.material.reciprocal_space_filename)
-        with self.assertRaises(RuntimeError):
-            stog.read_dataset({"Filename": filename}, xcol=99)
-
-    def test_stog_read_dataset_ycol_data_format_exception(self):
-        stog = StoG()
-        filename = get_data_path(self.material.reciprocal_space_filename)
-        with self.assertRaises(RuntimeError):
-            stog.read_dataset({"Filename": filename}, ycol=99)
-
-    def test_stog_read_dataset_dycol_too_large(self):
-        # Number of decimal places for precision
-        places = 5
-
-        # Load S(Q) for Argon from test data
-        stog = StoG(
-            **{
-                "<b_coh>^2": self.kwargs["<b_coh>^2"],
-                "<b_tot^2>": self.kwargs["<b_tot^2>"],
-            }
-        )
-        info = {
-            "Filename": get_data_path(self.material.reciprocal_space_filename),
-            "ReciprocalFunction": "S(Q)",
-            "Qmin": 0.02,
-            "Qmax": 35.2,
-            "Y": {"Offset": 0.0, "Scale": 1.0},
-            "X": {"Offset": 0.0},
-        }
-
-        info["index"] = 0
-        stog.read_dataset(info, dycol=99)
-
-        # Check S(Q) data against targets
-        self.assertEqual(
-            stog.reciprocal_individuals[0][self.first], self.reciprocal_xtarget
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.reciprocal_individuals[1][self.first],
+            stog.df_sq_individuals.iloc[self.first]['S(Q)_%d' % info['index']],
             self.sq_target[0],
-            places=places,
-        )
-        self.assertEqual(stog.reciprocal_individuals[2][self.first], 0.0)
-        self.assertAlmostEqual(
-            stog.sq_individuals[1][self.first], self.sq_target[0], places=places
-        )
+            places=places)
 
     def test_stog_read_all_data_assertion(self):
         stog = StoG()
-        with self.assertRaises(NoInputFilesException):
+        with self.assertRaises(AssertionError):
             stog.read_all_data()
 
         stog.files = list()
-        with self.assertRaises(NoInputFilesException):
+        with self.assertRaises(AssertionError):
             stog.read_all_data()
 
     def test_stog_read_all_data_for_files_length(self):
         # Load S(Q) for Argon from test data
         stog = StoG()
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.read_all_data()
 
         # Check S(Q) data against targets
-        self.assertEqual(len(stog.files), len(self.kwargs_for_files["Files"]))
+        self.assertEqual(
+            len(stog.files),
+            len(self.kwargs_for_files['Files']))
 
     def test_stog_read_all_data(self):
         # Number of decimal places for precision
         places = 5
 
         # Load S(Q) for Argon from test data
         stog = StoG()
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.read_all_data()
 
         # Check S(Q) data against targets
         self.assertEqual(
-            stog.reciprocal_individuals[0][self.first], self.reciprocal_xtarget
-        )
+            stog.df_individuals.iloc[self.first].name, self.reciprocal_xtarget)
         for index in range(len(stog.files)):
             self.assertAlmostEqual(
-                stog.reciprocal_individuals[1][self.first],
+                stog.df_individuals.iloc[self.first]['S(Q)_%d' % index],
                 self.sq_target[0],
-                places=places,
-            )
+                places=places)
             self.assertAlmostEqual(
-                stog.sq_individuals[1][self.first],
+                stog.df_sq_individuals.iloc[self.first]['S(Q)_%d' % index],
                 self.sq_target[0],
-                places=places,
-            )
+                places=places)
 
     def test_stog_merge_data(self):
         # Number of decimal places for precision
         places = 5
 
         # Load S(Q) for Argon from test data
         stog = StoG()
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.read_all_data()
         stog.merge_data()
 
         # Check S(Q) data against targets
         self.assertEqual(
-            stog.q_master[stog.sq_title][self.first], self.reciprocal_xtarget
-        )
+            stog.df_sq_master.iloc[self.first].name, self.reciprocal_xtarget)
         self.assertAlmostEqual(
-            stog.sq_master[stog.sq_title][self.first],
+            stog.df_sq_master.iloc[self.first][stog.sq_title],
             self.sq_target[0],
-            places=places,
-        )
+            places=places)
 
     def test_stog_merge_data_qsq_opts_scale(self):
         # Number of decimal places for precision
         places = 5
 
         # Load S(Q) for Argon from test data
         stog = StoG()
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.read_all_data()
-        qsq_opts = {"Y": {"Scale": 2.0}}
+        qsq_opts = {'Y': {'Scale': 2.0}}
 
         # Test Q[S(Q)-1] scale
-        stog.merged_opts["Q[S(Q)-1]"] = qsq_opts
+        stog.merged_opts['Q[S(Q)-1]'] = qsq_opts
         stog.merge_data()
         self.assertAlmostEqual(
-            stog.sq_master[stog.qsq_minus_one_title][self.first],
-            qsq_opts["Y"]["Scale"] * self.fq_target[0],
-            places=places,
-        )
+            stog.df_sq_master.iloc[self.first][stog.qsq_minus_one_title],
+            qsq_opts['Y']['Scale'] * self.fq_target[0],
+            places=places)
 
     def test_stog_merge_data_qsq_opts_offset(self):
         # Number of decimal places for precision
         places = 5
 
         # Load S(Q) for Argon from test data
         stog = StoG()
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.read_all_data()
-        qsq_opts = {"Y": {"Offset": 1.0}}
+        qsq_opts = {'Y': {'Offset': 1.0}}
 
         # Test Q[S(Q)-1] scale
-        stog.merged_opts["Q[S(Q)-1]"] = qsq_opts
+        stog.merged_opts['Q[S(Q)-1]'] = qsq_opts
         stog.merge_data()
         self.assertAlmostEqual(
-            stog.sq_master[stog.qsq_minus_one_title][self.first],
-            qsq_opts["Y"]["Offset"] + self.fq_target[0],
-            places=places,
-        )
+            stog.df_sq_master.iloc[self.first][stog.qsq_minus_one_title],
+            qsq_opts['Y']['Offset'] + self.fq_target[0],
+            places=places)
 
 
 class TestStogTransformSpecificMethods(TestStogDatasetSpecificMethods):
     def setUp(self):
         super(TestStogTransformSpecificMethods, self).setUp()
         self.lowR_target = 0.4720653
 
     def test_stog_transform_merged_default(self):
         # Number of decimal places for precision
         places = 2
 
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
 
         # Check g(r) data against targets
         self.assertAlmostEqual(
-            stog.r_master[stog.gr_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first].name,
             self.real_xtarget,
-            places=places,
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_title],
             self.gofr_target[0],
-            places=places,
-        )
+            places=places)
 
         # Test if no dr defined
         stog.dr = None
         stog.transform_merged()
 
         # Check g(r) data against targets
         self.assertAlmostEqual(
-            stog.r_master[stog.gr_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first].name,
             self.real_xtarget,
-            places=places,
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_title],
             self.gofr_target[0],
-            places=places,
-        )
+            places=places)
 
     def test_stog_transform_merged_GofR(self):
         # Number of decimal places for precision
         places = 2
 
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.real_space_function = "G(r)"
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
 
         # Check G(r) data against targets
         self.assertAlmostEqual(
-            stog.r_master[stog.gr_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first].name,
             self.real_xtarget,
-            places=places,
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_title],
             self.GofR_target[0],
-            places=places,
-        )
+            places=places)
 
     def test_stog_transform_merged_GKofR(self):
         # Number of decimal places for precision
         places = 2
 
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.real_space_function = "GK(r)"
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
 
         # Check GK(r) data against targets
         self.assertAlmostEqual(
-            stog.r_master[stog.gr_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first].name,
             self.real_xtarget,
-            places=places,
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_title],
             self.GKofR_target[0],
-            places=places,
-        )
+            places=places)
 
     def test_stog_transform_merged_for_nan_after_filter(self):
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.real_space_function = "GK(r)"
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
 
-        self.assertFalse(np.isnan(stog.sq_master[stog.sq_title]).any())
-        self.assertFalse(np.isnan(stog.gr_master[stog.gr_title]).any())
+        self.assertFalse(
+            np.isnan(stog.df_sq_master[stog.sq_title].values).any())
+        self.assertFalse(
+            np.isnan(stog.df_gr_master[stog.gr_title].values).any())
 
     def test_stog_fourier_filter(self):
         # Number of decimal places for precision
         places = 1
 
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = False
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
         stog.fourier_filter()
 
         # Check g(r) data against targets
         self.assertAlmostEqual(
-            stog.r_master[stog.gr_ft_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first].name,
             self.real_xtarget,
-            places=places,
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_ft_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_ft_title],
             self.gofr_ff_target[0],
-            places=places,
-        )
+            places=places)
 
     def test_stog_fourier_filter_before_transform_merged_call(self):
         # Number of decimal places for precision
         places = 1
 
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = False
         stog.read_all_data()
         stog.merge_data()
         stog.fourier_filter()
 
         # Check g(r) data against targets
         self.assertAlmostEqual(
-            stog.r_master[stog.gr_ft_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first].name,
             self.real_xtarget,
-            places=places,
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_ft_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_ft_title],
             self.gofr_ff_target[0],
-            places=places,
-        )
+            places=places)
 
     def test_stog_fourier_filter_GofR(self):
         # Number of decimal places for precision
         places = 1
 
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = False
         stog.real_space_function = "G(r)"
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
         stog.fourier_filter()
 
         # Check g(r) data against targets
         self.assertAlmostEqual(
-            stog.r_master[stog.gr_ft_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first].name,
             self.real_xtarget,
-            places=places,
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_ft_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_ft_title],
             self.GofR_ff_target[0],
-            places=places,
-        )
+            places=places)
 
     def test_stog_fourier_filter_GKofR(self):
         # Number of decimal places for precision
         places = 1
 
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = False
         stog.real_space_function = "GK(r)"
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
         stog.fourier_filter()
 
         # Check g(r) data against targets
         self.assertAlmostEqual(
-            stog.r_master[stog.gr_ft_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first].name,
             self.real_xtarget,
-            places=places,
-        )
+            places=places)
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_ft_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_ft_title],
             self.GKofR_ff_target[0],
-            places=places,
-        )
+            places=places)
+
+    @patch("matplotlib.pyplot.show")
+    def test_stog_fourier_filter_with_plot_flag(self, mock_show):
+        # Load S(Q) for Argon from test data
+        stog = StoG(**self.kwargs_for_stog_input)
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = True
+        stog.read_all_data()
+        stog.merge_data()
+        stog.transform_merged()
+        stog.fourier_filter()
+        mock_show.assert_called_with()
 
     def test_stog_fourier_filter_for_nan_after_filter(self):
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = False
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
         stog.fourier_filter()
 
-        self.assertFalse(np.isnan(stog.gr_master[stog.gr_title]).any())
-        self.assertFalse(np.isnan(stog.sq_master[stog.sq_title]).any())
-        self.assertFalse(np.isnan(stog.sq_master[stog._ft_title]).any())
-        self.assertFalse(np.isnan(stog.sq_master[stog.sq_ft_title]).any())
+        self.assertFalse(
+            np.isnan(stog.df_gr_master[stog.gr_title].values).any())
+        self.assertFalse(
+            np.isnan(stog.df_sq_master[stog.sq_title].values).any())
+        self.assertFalse(
+            np.isnan(stog.df_sq_master[stog._ft_title].values).any())
+        self.assertFalse(
+            np.isnan(stog.df_sq_master[stog.sq_ft_title].values).any())
 
     def test_stog_apply_lorch_default(self):
         # Number of decimal places for precision
         places = 5
 
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = False
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
         q, sq, r, gr = stog.fourier_filter()
         stog.apply_lorch(q, sq, r)
 
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_lorch_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_lorch_title],
             self.gofr_lorch_target[0],
-            places=places,
-        )
+            places=places)
 
     def test_stog_apply_lorch_GofR(self):
         # Number of decimal places for precision
         places = 5
 
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = False
         stog.real_space_function = "G(r)"
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
         q, sq, r, gr = stog.fourier_filter()
         stog.apply_lorch(q, sq, r)
 
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_lorch_title][self.real_space_first],
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_lorch_title],
             self.GofR_lorch_target[0],
-            places=places,
-        )
+            places=places)
 
     def test_stog_apply_lorch_GKofR(self):
         # Number of decimal places for precision
         places = 5
 
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = False
         stog.real_space_function = "GK(r)"
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
         q, sq, r, gr = stog.fourier_filter()
         stog.apply_lorch(q, sq, r)
 
         self.assertAlmostEqual(
-            stog.gr_master[stog.gr_lorch_title][self.real_space_first],
-            self.GKofR_lorch_target[0],
-            places=places,
-        )
+            stog.df_gr_master.iloc[self.real_space_first][stog.gr_lorch_title],
+            self.GKofR_lorch_target[0], places=places)
+
+    @patch("matplotlib.pyplot.show")
+    def test_stog_apply_lorch_with_plot_flag(self, mock_show):
+        # Load S(Q) for Argon from test data
+        stog = StoG(**self.kwargs_for_stog_input)
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = True
+        stog.read_all_data()
+        stog.merge_data()
+        stog.transform_merged()
+        q, sq, r, gr = stog.fourier_filter()
+        stog.apply_lorch(q, sq, r)
+        mock_show.assert_called_with()
 
     def test_stog_lowR_mean_square(self):
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = False
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
-        gr = stog.gr_master[stog.gr_title]
+        gr = stog.df_gr_master[stog.gr_title].values
         cost = stog._lowR_mean_square(stog.dr, gr)
         self.assertAlmostEqual(cost, self.lowR_target, places=7)
 
     def test_stog_get_lowR_mean_square(self):
         # Load S(Q) for Argon from test data
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
+        stog.plot_flag = False
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
         q, sq, r, gr = stog.fourier_filter()
         cost = stog._get_lowR_mean_square()
         self.assertAlmostEqual(cost, self.lowR_target, places=7)
 
 
-class TestStogBookkeepingMethods(TestStogDatasetSpecificMethods):
+class TestStogPlottingDataFrameMethods(TestStogDatasetSpecificMethods):
     def setUp(self):
-        super(TestStogBookkeepingMethods, self).setUp()
+        super(TestStogPlottingDataFrameMethods, self).setUp()
         stog = StoG(**self.kwargs_for_stog_input)
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
 
         self.stog = stog
 
     def test_stog_add_keen_fq(self):
         stog = self.stog
-        q = stog.sq_master[stog.sq_title]
-        sq = stog.sq_master[stog.sq_title]
+        q = stog.df_sq_master[stog.sq_title].index.values
+        sq = stog.df_sq_master[stog.sq_title].values
         stog._add_keen_fq(q, sq)
-        self.assertTrue(stog.fq_title in stog.sq_master)
+        self.assertTrue(stog.fq_title in stog.df_sq_master.columns)
 
     def test_stog_add_keen_gr_default(self):
         stog = self.stog
-        r = stog.gr_master[stog.gr_title]
-        gr = stog.gr_master[stog.gr_title]
+        r = stog.df_gr_master[stog.gr_title].index.values
+        gr = stog.df_gr_master[stog.gr_title].values
         stog._add_keen_gr(r, gr)
-        self.assertTrue(stog.GKofR_title in stog.gr_master)
+        self.assertTrue(stog.GKofR_title in stog.df_gr_master.columns)
 
     def test_stog_add_keen_gr_GofR(self):
         stog = StoG(**self.kwargs_for_stog_input)
         stog.real_space_function = "G(r)"
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
-        r = stog.gr_master[stog.gr_title]
-        gr = stog.gr_master[stog.gr_title]
+        r = stog.df_gr_master[stog.gr_title].index.values
+        gr = stog.df_gr_master[stog.gr_title].values
         stog._add_keen_gr(r, gr)
-        self.assertTrue(stog.GKofR_title in stog.gr_master)
+        self.assertTrue(stog.GKofR_title in stog.df_gr_master.columns)
 
     def test_stog_add_keen_gr_GKofR(self):
         stog = StoG(**self.kwargs_for_stog_input)
         stog.real_space_function = "GK(r)"
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
-        r = stog.gr_master[stog.gr_title]
-        gr = stog.gr_master[stog.gr_title]
+        r = stog.df_gr_master[stog.gr_title].index.values
+        gr = stog.df_gr_master[stog.gr_title].values
         stog._add_keen_gr(r, gr)
-        self.assertTrue(stog.GKofR_title in stog.gr_master)
+        self.assertTrue(stog.GKofR_title in stog.df_gr_master.columns)
+
+    @patch("matplotlib.pyplot.show")
+    def test_stog_plot_df(self, mock_show):
+        df = pd.DataFrame(np.random.randn(10, 2),
+                          index=np.arange(10),
+                          columns=list('XY'))
+        stog = StoG()
+        stog._plot_df(df, 'x', 'y', 'title', None)
+        mock_show.assert_called_with()
+
+    @patch("matplotlib.pyplot.show")
+    def test_stog_plot_sq(self, mock_show):
+        self.stog.plot_sq()
+        mock_show.assert_called_with()
+
+    @patch("matplotlib.pyplot.show")
+    def test_stog_plot_merged_sq(self, mock_show):
+        self.stog.plot_merged_sq()
+        mock_show.assert_called_with()
+
+        self.stog.df_individuals = pd.DataFrame()
+        self.stog.plot_merged_sq()
+        mock_show.assert_called_with()
+
+    @patch("matplotlib.pyplot.show")
+    def test_stog_plot_gr(self, mock_show):
+        self.stog.plot_gr()
+        mock_show.assert_called_with()
+
+    @patch("matplotlib.pyplot.show")
+    def test_stog_plot_summary_sq(self, mock_show):
+        self.stog.plot_summary_sq()
+        mock_show.assert_called_with()
+
+    @patch("matplotlib.pyplot.show")
+    def test_stog_plot_summary_gr(self, mock_show):
+        self.stog.plot_summary_gr()
+        mock_show.assert_called_with()
 
 
-class TestStogOutputMethods(TestStogDatasetSpecificMethods):
+class TestStogOutputDataFrameMethods(TestStogDatasetSpecificMethods):
     def setUp(self):
-        super(TestStogOutputMethods, self).setUp()
+        super(TestStogOutputDataFrameMethods, self).setUp()
         stog = StoG(**self.kwargs_for_stog_input)
+        stog.plot_flag = False
         stog.stem_name = "dog"
-        stog.files = self.kwargs_for_files["Files"]
+        stog.files = self.kwargs_for_files['Files']
         stog.read_all_data()
         stog.merge_data()
         stog.transform_merged()
 
         self.stog = stog
 
     # Decorator to provide the data to run each write_out_<type> test
-    def data_provider(self, x, y, filename):
+    def data_provider(self, stog, df, title, filename):
         def write_out_decorator(write_out_func):
             def wrap_function(*args):
                 # Using stem name
                 write_out_func()
+                x = df[title].index.values
+                y = df[title].values
 
-                data = {}
-                data["x"], data["y"] = np.genfromtxt(
-                    filename, skip_header=2, unpack=True
-                )
-
-                np.testing.assert_allclose(data["x"], x)
-                np.testing.assert_allclose(
-                    data["y"] - y,
-                    np.zeros(len(y)),
+                outfile_path = filename
+                data = pd.read_csv(outfile_path,
+                                   sep=r"\s+",
+                                   usecols=[0, 1],
+                                   names=['x', 'y'],
+                                   skiprows=2,
+                                   engine='python')
+
+                assert_allclose(data['x'], x)
+                assert_allclose(
+                    data['y'] - y,
+                    np.zeros(
+                        len(y)),
                     rtol=2.0,
                     atol=2.0,
-                    equal_nan=True,
-                )
+                    equal_nan=True)
 
-                os.remove(filename)
+                os.remove(outfile_path)
 
                 # Using set filename
-                tmp_filename = tempfile.mkstemp()[1]
+                outfile_path = tempfile.mkstemp()[1]
 
-                write_out_func(filename=tmp_filename)
-
-                data["x"], data["y"] = np.genfromtxt(
-                    tmp_filename, skip_header=2, unpack=True
-                )
-
-                np.testing.assert_allclose(data["x"], x)
-                np.testing.assert_allclose(data["y"], y)
-                os.remove(tmp_filename)
+                write_out_func(filename=outfile_path)
+                x = df[title].index.values
+                y = df[title].values
+
+                data = pd.read_csv(outfile_path,
+                                   sep=r"\s+",
+                                   usecols=[0, 1],
+                                   names=['x', 'y'],
+                                   skiprows=2,
+                                   engine='python')
+
+                assert_allclose(data['x'], x)
+                assert_allclose(data['y'], y)
+                os.remove(outfile_path)
 
             return wrap_function
-
         return write_out_decorator
 
     # Tests
+    def test_stog_add_to_dataframe(self):
+        x = np.random.randn(10)
+        y1 = np.random.randn(10)
+        y2 = np.random.randn(10)
+        df_target = pd.DataFrame(np.column_stack(
+            [y1, y2]), columns=['y1', 'y2'], index=x)
+        df = pd.DataFrame(np.column_stack([y1]), columns=['y1'], index=x)
+        df = self.stog.add_to_dataframe(x, y2, df, 'y2')
+        self.assertTrue(df.equals(df_target))
+
+        y3 = np.random.randn(10)
+        df = self.stog.add_to_dataframe(x, y3, df, 'y2')
+        self.assertFalse(df.equals(df_target))
+
     def test_stog_write_df(self):
         outfile_path = tempfile.mkstemp()[1]
-        x = self.stog.q_master[self.stog.sq_title]
-        y = self.stog.sq_master[self.stog.sq_title]
-        self.stog._write_out_to_file(x, y, outfile_path)
-        data = {}
-        data["x"], data["y"] = np.genfromtxt(
-            outfile_path, skip_header=2, unpack=True
-        )
+        self.stog._write_out_df(self.stog.df_sq_master,
+                                [self.stog.sq_title], outfile_path)
+        data = pd.read_csv(outfile_path,
+                           sep=r"\s+",
+                           usecols=[0, 1],
+                           names=['x', 'y'],
+                           skiprows=2,
+                           engine='python')
 
-        q = self.stog.q_master[self.stog.sq_title]
-        sq = self.stog.sq_master[self.stog.sq_title]
+        q = self.stog.df_sq_master[self.stog.sq_title].index.values
+        sq = self.stog.df_sq_master[self.stog.sq_title].values
 
-        np.testing.assert_allclose(data["x"], q)
-        np.testing.assert_allclose(data["y"], sq)
+        assert_allclose(data['x'], q)
+        assert_allclose(data['y'], sq)
         os.remove(outfile_path)
 
+        with self.assertRaises(ValueError):
+            self.stog._write_out_df(pd.DataFrame(), 'title', outfile_path)
+
     def test_write_out_merged_sq(self):
         # Have to decorate after the setUp() is called for the self.* args to
         # work
         @self.data_provider(
-            self.stog.q_master[self.stog.sq_title],
-            self.stog.sq_master[self.stog.sq_title],
-            "dog.sq",
-        )
+            self.stog,
+            self.stog.df_sq_master,
+            self.stog.sq_title,
+            "dog.sq")
         def decorated_write_out_merged(*args, **kwargs):
             self.stog.write_out_merged_sq(*args, **kwargs)
-
         decorated_write_out_merged()
 
     def test_write_out_merged_gr(self):
         # Have to decorate after the setUp() is called for the self.* args to
         # work
         @self.data_provider(
-            self.stog.r_master[self.stog.gr_title],
-            self.stog.gr_master[self.stog.gr_title],
-            "dog.gr",
-        )
+            self.stog,
+            self.stog.df_gr_master,
+            self.stog.gr_title,
+            "dog.gr")
         def decorated_write_out_merged(*args, **kwargs):
             self.stog.write_out_merged_gr(*args, **kwargs)
-
         decorated_write_out_merged()
 
     def test_write_out_ft_sq(self):
         self.stog.fourier_filter()
         # Have to decorate after the setUp() is called for the self.* args to
         # work
 
         @self.data_provider(
-            self.stog.q_master[self.stog.sq_ft_title],
-            self.stog.sq_master[self.stog.sq_ft_title],
-            "dog_ft.sq",
-        )
+            self.stog,
+            self.stog.df_sq_master,
+            self.stog.sq_ft_title,
+            'dog_ft.sq')
         def decorated_write_out_merged(*args, **kwargs):
             self.stog.write_out_ft_sq(*args, **kwargs)
-
         decorated_write_out_merged()
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     unittest.main()  # pragma: no cover
```

### Comparing `pystog-0.4.0/tests/test_transformer.py` & `pystog-1.0.0/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `pystog-0.4.0/tests/utils.py` & `pystog-1.0.0/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import print_function
 import os
 import numpy as np
 
 from pystog.utils import RealSpaceHeaders, ReciprocalSpaceHeaders
 from pystog.converter import Converter
 from pystog.transformer import Transformer
```

### Comparing `pystog-0.4.0/versioneer.py` & `pystog-1.0.0/versioneer.py`

 * *Files identical despite different names*

