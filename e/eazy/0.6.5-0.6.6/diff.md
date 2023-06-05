# Comparing `tmp/eazy-0.6.5.tar.gz` & `tmp/eazy-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eazy-0.6.5.tar", last modified: Mon Jun  5 15:28:37 2023, max compression
+gzip compressed data, was "eazy-0.6.6.tar", last modified: Mon Jun  5 15:58:08 2023, max compression
```

## Comparing `eazy-0.6.5.tar` & `eazy-0.6.6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.052916 eazy-0.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.032915 eazy-0.6.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.036915 eazy-0.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-05 15:28:22.000000 eazy-0.6.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-05 15:28:22.000000 eazy-0.6.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-05 15:28:22.000000 eazy-0.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:22.000000 eazy-0.6.5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-05 15:28:22.000000 eazy-0.6.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 15:28:22.000000 eazy-0.6.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-05 15:28:22.000000 eazy-0.6.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 15:28:22.000000 eazy-0.6.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 15:28:22.000000 eazy-0.6.5/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-05 15:28:37.052916 eazy-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-05 15:28:22.000000 eazy-0.6.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.036915 eazy-0.6.5/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-05 15:28:22.000000 eazy-0.6.5/binder/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.036915 eazy-0.6.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.032915 eazy-0.6.5/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.036915 eazy-0.6.5/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.040915 eazy-0.6.5/docs/eazy/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    36073 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/filters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/photoz.rst
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/zout_columns.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.044916 eazy-0.6.5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)  2836689 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/examples/HDFN-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   330296 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/examples/Riverside-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1966244 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/examples/compare_sps_algorithm.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   590683 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/examples/dash_viewer.png
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/rtd-pip-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.048916 eazy-0.6.5/eazy/
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.052916 eazy-0.6.5/eazy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/DLAcoeff.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/LAFcoeff.txt
--rw-r--r--   0 runner    (1001) docker     (123)   273600 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/alpha_lyr_stis_008.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/emlines_info.dat
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/spectra_kc13_12_tweak.params
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/zphot.param.default
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/igm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/param.py
--rw-r--r--   0 runner    (1001) docker     (123)   226826 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/photoz.py
--rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/sps.py
--rw-r--r--   0 runner    (1001) docker     (123)    50015 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.052916 eazy-0.6.5/eazy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_igm.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_param.py
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_photoz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38961 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 15:28:36.000000 eazy-0.6.5/eazy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46541 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.048916 eazy-0.6.5/eazy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-05 15:28:36.000000 eazy-0.6.5/eazy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-05 15:28:37.000000 eazy-0.6.5/eazy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:28:36.000000 eazy-0.6.5/eazy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-05 15:28:36.000000 eazy-0.6.5/eazy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 15:28:36.000000 eazy-0.6.5/eazy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-05 15:28:22.000000 eazy-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-05 15:28:22.000000 eazy-0.6.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.052916 eazy-0.6.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 15:28:22.000000 eazy-0.6.5/scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-06-05 15:28:22.000000 eazy-0.6.5/scripts/nmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-05 15:28:22.000000 eazy-0.6.5/scripts/photoz.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-05 15:28:22.000000 eazy-0.6.5/scripts/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-06-05 15:28:22.000000 eazy-0.6.5/scripts/sps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-05 15:28:37.052916 eazy-0.6.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-06-05 15:28:22.000000 eazy-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.726415 eazy-0.6.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.710414 eazy-0.6.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.710414 eazy-0.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-05 15:58:00.000000 eazy-0.6.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-05 15:58:00.000000 eazy-0.6.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-05 15:58:00.000000 eazy-0.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:00.000000 eazy-0.6.6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-05 15:58:00.000000 eazy-0.6.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 15:58:00.000000 eazy-0.6.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-05 15:58:00.000000 eazy-0.6.6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 15:58:00.000000 eazy-0.6.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 15:58:00.000000 eazy-0.6.6/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-05 15:58:08.726415 eazy-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-05 15:58:00.000000 eazy-0.6.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.714414 eazy-0.6.6/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-05 15:58:00.000000 eazy-0.6.6/binder/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.714414 eazy-0.6.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.710414 eazy-0.6.6/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.714414 eazy-0.6.6/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.714414 eazy-0.6.6/docs/eazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/eazy/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36073 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/eazy/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/eazy/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/eazy/photoz.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/eazy/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/eazy/zout_columns.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.718414 eazy-0.6.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)  2836689 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/examples/HDFN-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   330296 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/examples/Riverside-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1966244 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/examples/compare_sps_algorithm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   590683 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/examples/dash_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-05 15:58:00.000000 eazy-0.6.6/docs/rtd-pip-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.722414 eazy-0.6.6/eazy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.726415 eazy-0.6.6/eazy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/data/DLAcoeff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/data/LAFcoeff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   273600 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/data/alpha_lyr_stis_008.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/data/emlines_info.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/data/spectra_kc13_12_tweak.params
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/data/zphot.param.default
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/igm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)   226826 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/photoz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/sps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50015 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.726415 eazy-0.6.6/eazy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/tests/test_igm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/tests/test_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/tests/test_photoz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38961 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 15:58:08.000000 eazy-0.6.6/eazy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46637 2023-06-05 15:58:00.000000 eazy-0.6.6/eazy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.722414 eazy-0.6.6/eazy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-05 15:58:08.000000 eazy-0.6.6/eazy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-05 15:58:08.000000 eazy-0.6.6/eazy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:58:08.000000 eazy-0.6.6/eazy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-05 15:58:08.000000 eazy-0.6.6/eazy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 15:58:08.000000 eazy-0.6.6/eazy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-05 15:58:00.000000 eazy-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-05 15:58:00.000000 eazy-0.6.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:58:08.726415 eazy-0.6.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 15:58:00.000000 eazy-0.6.6/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-06-05 15:58:00.000000 eazy-0.6.6/scripts/nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-05 15:58:00.000000 eazy-0.6.6/scripts/photoz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-05 15:58:00.000000 eazy-0.6.6/scripts/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-06-05 15:58:00.000000 eazy-0.6.6/scripts/sps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-05 15:58:08.726415 eazy-0.6.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-06-05 15:58:00.000000 eazy-0.6.6/setup.py
```

### Comparing `eazy-0.6.5/.github/workflows/publish-to-pypi.yml` & `eazy-0.6.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/.github/workflows/python-package.yml` & `eazy-0.6.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/.gitignore` & `eazy-0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/.readthedocs.yml` & `eazy-0.6.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/CITATION.cff` & `eazy-0.6.6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/LICENSE.txt` & `eazy-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/PKG-INFO` & `eazy-0.6.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eazy
-Version: 0.6.5
+Version: 0.6.6
 Summary: Pythonic photo-zs
 Home-page: https://github.com/gbrammer/eazy-py
 Author: G. Brammer
 Author-email: gbrammer@gmail.com
 License: MIT
 Project-URL: Documentation, https://eazy-py.readthedocs.io/
 Project-URL: Source, https://github.com/gbrammer/eazy-py
@@ -43,24 +43,20 @@
 Installation instructions
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code:: bash
 
     pip install eazy
 
-    # Forked dependencies that don't come with pip
-    pip install git+https://github.com/gbrammer/dust_attenuation.git
-    pip install git+https://github.com/gbrammer/dust_extinction.git
-
 Demo
 ~~~~
 
 .. image:: https://colab.research.google.com/assets/colab-badge.svg
  :target: https://colab.research.google.com/github/gbrammer/eazy-py/blob/master/docs/examples/HDFN-demo.ipynb
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/gbrammer/eazy-py/HEAD?filepath=docs%2Fexamples%2FHDFN-demo.ipynb
 
 
 Citation
-~~~~~~~~~~~~~
-Please cite both this reposiotry and `Brammer et al. (2008) <https://ui.adsabs.harvard.edu/abs/2008ApJ...686.1503B/abstract>`_. A BiBTeX for this repository can be generated via the *Cite this repository* link in the upper left corner of the `GitHub page <https://github.com/gbrammer/eazy-py>`_.
+~~~~~~~~
+Please cite both this repository and `Brammer et al. (2008) <https://ui.adsabs.harvard.edu/abs/2008ApJ...686.1503B/abstract>`_. A BiBTeX for this repository can be generated via the *Cite this repository* link in the upper left corner of the `GitHub page <https://github.com/gbrammer/eazy-py>`_.
```

### Comparing `eazy-0.6.5/README.rst` & `eazy-0.6.6/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -23,24 +23,20 @@
 Installation instructions
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code:: bash
 
     pip install eazy
 
-    # Forked dependencies that don't come with pip
-    pip install git+https://github.com/gbrammer/dust_attenuation.git
-    pip install git+https://github.com/gbrammer/dust_extinction.git
-
 Demo
 ~~~~
 
 .. image:: https://colab.research.google.com/assets/colab-badge.svg
  :target: https://colab.research.google.com/github/gbrammer/eazy-py/blob/master/docs/examples/HDFN-demo.ipynb
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/gbrammer/eazy-py/HEAD?filepath=docs%2Fexamples%2FHDFN-demo.ipynb
 
 
 Citation
-~~~~~~~~~~~~~
-Please cite both this reposiotry and `Brammer et al. (2008) <https://ui.adsabs.harvard.edu/abs/2008ApJ...686.1503B/abstract>`_. A BiBTeX for this repository can be generated via the *Cite this repository* link in the upper left corner of the `GitHub page <https://github.com/gbrammer/eazy-py>`_.
+~~~~~~~~
+Please cite both this repository and `Brammer et al. (2008) <https://ui.adsabs.harvard.edu/abs/2008ApJ...686.1503B/abstract>`_. A BiBTeX for this repository can be generated via the *Cite this repository* link in the upper left corner of the `GitHub page <https://github.com/gbrammer/eazy-py>`_.
```

### Comparing `eazy-0.6.5/docs/Makefile` & `eazy-0.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/docs/conf.py` & `eazy-0.6.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/docs/eazy/filters.rst` & `eazy-0.6.6/docs/eazy/filters.rst`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/docs/eazy/install.rst` & `eazy-0.6.6/docs/eazy/install.rst`

 * *Files 17% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Install with `pip`
 ==================
 .. code:: bash
 
     pip install eazy
-    
-    # Forked dependencies that don't come with pip
-    pip install git+https://github.com/gbrammer/dust_attenuation.git
-    pip install git+https://github.com/gbrammer/dust_extinction.git
 
 Install from the repository
 ===========================
 .. code:: bash
     
     ### [OPTIONAL!] create a fresh conda environment
     conda create -n eazy39 python=3.9
@@ -33,8 +29,8 @@
     pip install .[test] -r requirements.txt
     pytest
     
     
 Binder Demo
 ~~~~~~~~~~~
 .. image:: https://mybinder.org/badge_logo.svg
- :target: https://mybinder.org/v2/gh/gbrammer/eazy-py/HEAD?filepath=docs%2Fexamples%2FHDFN-demo.ipynb
+ :target: https://mybinder.org/v2/gh/gbrammer/eazy-py/HEAD?filepath=docs%2Fexamples%2FHDFN-demo.ipynb
```

### Comparing `eazy-0.6.5/docs/eazy/templates.rst` & `eazy-0.6.6/docs/eazy/templates.rst`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/docs/eazy/zout_columns.rst` & `eazy-0.6.6/docs/eazy/zout_columns.rst`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/docs/examples/HDFN-demo.ipynb` & `eazy-0.6.6/docs/examples/HDFN-demo.ipynb`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/docs/examples/Riverside-demo.ipynb` & `eazy-0.6.6/docs/examples/Riverside-demo.ipynb`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/docs/examples/compare_sps_algorithm.ipynb` & `eazy-0.6.6/docs/examples/compare_sps_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/docs/examples/dash_viewer.png` & `eazy-0.6.6/docs/examples/dash_viewer.png`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/docs/index.rst` & `eazy-0.6.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/docs/make.bat` & `eazy-0.6.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/__init__.py` & `eazy-0.6.6/eazy/__init__.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/data/DLAcoeff.txt` & `eazy-0.6.6/eazy/data/DLAcoeff.txt`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/data/LAFcoeff.txt` & `eazy-0.6.6/eazy/data/LAFcoeff.txt`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/data/alpha_lyr_stis_008.fits` & `eazy-0.6.6/eazy/data/alpha_lyr_stis_008.fits`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/data/emlines_info.dat` & `eazy-0.6.6/eazy/data/emlines_info.dat`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/data/zphot.param.default` & `eazy-0.6.6/eazy/data/zphot.param.default`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/filters.py` & `eazy-0.6.6/eazy/filters.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/hdf5.py` & `eazy-0.6.6/eazy/hdf5.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/igm.py` & `eazy-0.6.6/eazy/igm.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/param.py` & `eazy-0.6.6/eazy/param.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/photoz.py` & `eazy-0.6.6/eazy/photoz.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/sps.py` & `eazy-0.6.6/eazy/sps.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/templates.py` & `eazy-0.6.6/eazy/templates.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/tests/test_filters.py` & `eazy-0.6.6/eazy/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/tests/test_igm.py` & `eazy-0.6.6/eazy/tests/test_igm.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/tests/test_param.py` & `eazy-0.6.6/eazy/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/tests/test_photoz.py` & `eazy-0.6.6/eazy/tests/test_photoz.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/tests/test_templates.py` & `eazy-0.6.6/eazy/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/tests/test_utils.py` & `eazy-0.6.6/eazy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/utils.py` & `eazy-0.6.6/eazy/utils.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/eazy/visualization.py` & `eazy-0.6.6/eazy/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         
         with urllib.request.urlopen(furl) as url:
             olap = json.loads(url.read().decode())
         
         return olap
     
     
-    def make_dash_app(self, template='plotly_white', server_mode='external', port=8050, app=None, app_type='jupyter', plot_height=680, external_stylesheets=['https://codepen.io/chriddyp/pen/bWLwgP.css'], infer_proxy=False, slider_width=140, cutout_hdu=None, cutout_rgb=None, cutout_size=10, api_filters=None, api_size=2, PLOT_TYPES=['zphot-zspec', 'Mag-redshift', 'Mass-redshift', 'UVJ', 'RA/Dec', 'UV-redshift', 'chi2-redshift'], get_content=False):
+    def make_dash_app(self, template='plotly_white', server_mode='external', port=8050, app=None, app_type='jupyter', plot_height=680, external_stylesheets=['https://codepen.io/chriddyp/pen/bWLwgP.css'], infer_proxy=False, slider_width=140, cutout_hdu=None, cutout_rgb=None, cutout_size=10, api_filters=None, api_size=2, api_args='', PLOT_TYPES=['zphot-zspec', 'Mag-redshift', 'Mass-redshift', 'UVJ', 'RA/Dec', 'UV-redshift', 'chi2-redshift'], get_content=False):
         """
         Create a Plotly/Dash app for interactive exploration
         
         Parameters
         ----------
         template : str
             `plotly` style `template <https://plotly.com/python/templates/#specifying-themes-in-graph-object-figures>`_.
@@ -253,14 +253,15 @@
         for _t in self.extra_plots:
             PLOT_TYPES.append(_t)
             
         COLOR_TYPES = ['z_phot', 'z_spec', 'mass', 'sSFR', 'chi2']
         self.COLOR_TYPES = COLOR_TYPES
         self.PLOT_TYPES = PLOT_TYPES
         self.cutout_data = None
+        self.cutout_wcs = None
         self.api_filters = api_filters
         
         #_title = f"{self.photoz.param['MAIN_OUTPUT_FILE']}"
         #_subhead = f"Nobj={self.photoz.NOBJ}  Nfilt={self.photoz.NFILT}"
         _title = [html.Strong(self.photoz.param['MAIN_OUTPUT_FILE']), 
                   ' / N', html.Sub('obj'), f'={self.photoz.NOBJ}', 
                   ' / N', html.Sub('filt'), f'={self.photoz.NFILT}', 
@@ -274,15 +275,15 @@
                                    'height':'14pt', 
                                    'margin-top':'-20px'})
         
         # bool_options = {'has_zspec': 'z_spec > 0', 
         #                 'use': 'Use == 1'}
         
         if cutout_hdu is not None:
-            cutout_wcs = pywcs.WCS(cutout_hdu.header, relax=True)
+            self.cutout_wcs = pywcs.WCS(cutout_hdu.header, relax=True)
             if cutout_rgb is None:
                 self.cutout_data = cutout_hdu.data
             else:
                 self.cutout_data = np.flipud(plt.imread(cutout_rgb))
                 
             print('xxx', self.cutout_data.shape)
             
@@ -292,14 +293,15 @@
                                  ], style={'right':'70px', 
                                            'width':'120px',
                                            'height':'120px',
                                         'border':'1px solid rgb(200,200,200)',
                                            'top':'10px', 
                                            'position':'absolute'})
             cutout_target = 'figure'
+            
         elif api_filters is not None:
             
             cutout_div = html.Div([
                              dcc.Graph(id='cutout-figure', 
                                        style={})
                                  ], style={'right':'70px', 
                                            'width':'120px',
@@ -891,15 +893,16 @@
             import json 
             import PIL.Image
             
             ix = np.where(self.df['id'] == id_i)[0][0]
             ri, di = self.df['ra'][ix], self.df['dec'][ix]
             
             turl = f'https://grizli-cutout.herokuapp.com/thumb?'
-            turl += f'ra={ri}&dec={di}&size={api_size}&filters={api_filters}'   
+            turl += f'ra={ri}&dec={di}&size={api_size}'
+            turl += f'{api_args}&filters={api_filters}'   
             #print(turl)
             # with open('/tmp/thumb.log','a') as fp:
             #     fp.write(turl+'\n')
                 
             req = urllib.request.urlopen(turl)
                                                         
             thumb = np.array(PIL.Image.open(req))
```

### Comparing `eazy-0.6.5/eazy.egg-info/PKG-INFO` & `eazy-0.6.6/eazy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eazy
-Version: 0.6.5
+Version: 0.6.6
 Summary: Pythonic photo-zs
 Home-page: https://github.com/gbrammer/eazy-py
 Author: G. Brammer
 Author-email: gbrammer@gmail.com
 License: MIT
 Project-URL: Documentation, https://eazy-py.readthedocs.io/
 Project-URL: Source, https://github.com/gbrammer/eazy-py
@@ -43,24 +43,20 @@
 Installation instructions
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code:: bash
 
     pip install eazy
 
-    # Forked dependencies that don't come with pip
-    pip install git+https://github.com/gbrammer/dust_attenuation.git
-    pip install git+https://github.com/gbrammer/dust_extinction.git
-
 Demo
 ~~~~
 
 .. image:: https://colab.research.google.com/assets/colab-badge.svg
  :target: https://colab.research.google.com/github/gbrammer/eazy-py/blob/master/docs/examples/HDFN-demo.ipynb
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/gbrammer/eazy-py/HEAD?filepath=docs%2Fexamples%2FHDFN-demo.ipynb
 
 
 Citation
-~~~~~~~~~~~~~
-Please cite both this reposiotry and `Brammer et al. (2008) <https://ui.adsabs.harvard.edu/abs/2008ApJ...686.1503B/abstract>`_. A BiBTeX for this repository can be generated via the *Cite this repository* link in the upper left corner of the `GitHub page <https://github.com/gbrammer/eazy-py>`_.
+~~~~~~~~
+Please cite both this repository and `Brammer et al. (2008) <https://ui.adsabs.harvard.edu/abs/2008ApJ...686.1503B/abstract>`_. A BiBTeX for this repository can be generated via the *Cite this repository* link in the upper left corner of the `GitHub page <https://github.com/gbrammer/eazy-py>`_.
```

### Comparing `eazy-0.6.5/eazy.egg-info/SOURCES.txt` & `eazy-0.6.6/eazy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/requirements.txt` & `eazy-0.6.6/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 # scipy >= 1.5.0
 # matplotlib >= 3.2
 # astropy >= 4.0
 # peakutils >= 1.0.3
 # tqdm
 # h5py
 
-# dustmaps needs healpy in environment.yml since 
+# dustmaps needs healpy in environment.yml since
 # often can't compile on Mac with pip
 # ... removing requirement so that can distribute just with requirements.txt
 # dustmaps
 
-# My clones of the dust modules
-git+https://github.com/gbrammer/dust_extinction.git
-git+https://github.com/gbrammer/dust_attenuation.git
+# git+https://github.com/gbrammer/dust_extinction.git
+# git+https://github.com/gbrammer/dust_attenuation.git
 
 # Needed for template smoothing, doesn't bring whole fsps distro
 astro-sedpy>=0.3
 # astro-prospector
```

### Comparing `eazy-0.6.5/scripts/nmf.py` & `eazy-0.6.6/scripts/nmf.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/scripts/photoz.py` & `eazy-0.6.6/scripts/photoz.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/scripts/run.py` & `eazy-0.6.6/scripts/run.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/scripts/sps.py` & `eazy-0.6.6/scripts/sps.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.5/setup.cfg` & `eazy-0.6.6/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,26 @@
 	scipy
 	matplotlib
 	astropy
 	peakutils
 	tqdm
 	h5py
 	astro-sedpy>=0.3
+	dust_attenuation @ git+https://github.com/karllark/dust_attenuation#egg=dust_attenuation
+	dust_extinction @ git+https://github.com/gbrammer/dust_extinction.git#egg=dust_extinction
 packages = find:
 include_package_data = True
 
 [options.extras_require]
 test = 
 	pytest>=5.1
 	flake8
 docs = 
 	sphinx
 	sphinx-astropy
-	dust_attenuation @ git+https://github.com/gbrammer/dust_attenuation.git
-	dust_extinction @ git+https://github.com/gbrammer/dust_extinction.git
 
 [options.package_data]
 eazy.data = 
 	*.txt
 	alpha_lyr_stis_008.fits
 	emlines_info.dat
 	zphot.param.default
```

