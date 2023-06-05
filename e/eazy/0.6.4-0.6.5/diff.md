# Comparing `tmp/eazy-0.6.4.tar.gz` & `tmp/eazy-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eazy-0.6.4.tar", last modified: Sat Mar 11 11:14:59 2023, max compression
+gzip compressed data, was "eazy-0.6.5.tar", last modified: Mon Jun  5 15:28:37 2023, max compression
```

## Comparing `eazy-0.6.4.tar` & `eazy-0.6.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.402124 eazy-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.378123 eazy-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.386124 eazy-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-11 11:14:47.000000 eazy-0.6.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-03-11 11:14:47.000000 eazy-0.6.4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-11 11:14:47.000000 eazy-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:47.000000 eazy-0.6.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-11 11:14:47.000000 eazy-0.6.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-11 11:14:47.000000 eazy-0.6.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-11 11:14:47.000000 eazy-0.6.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-11 11:14:47.000000 eazy-0.6.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-11 11:14:47.000000 eazy-0.6.4/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-11 11:14:59.402124 eazy-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-11 11:14:47.000000 eazy-0.6.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.386124 eazy-0.6.4/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-11 11:14:47.000000 eazy-0.6.4/binder/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.386124 eazy-0.6.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.382123 eazy-0.6.4/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.386124 eazy-0.6.4/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.386124 eazy-0.6.4/docs/eazy/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/eazy/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    36073 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/eazy/filters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/eazy/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/eazy/photoz.rst
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/eazy/templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/eazy/zout_columns.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.394123 eazy-0.6.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)  2836689 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/examples/HDFN-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   330296 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/examples/Riverside-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1966244 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/examples/compare_sps_algorithm.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   590683 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/examples/dash_viewer.png
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-11 11:14:47.000000 eazy-0.6.4/docs/rtd-pip-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.398124 eazy-0.6.4/eazy/
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.398124 eazy-0.6.4/eazy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/data/DLAcoeff.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/data/LAFcoeff.txt
--rw-r--r--   0 runner    (1001) docker     (123)   273600 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/data/alpha_lyr_stis_008.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/data/emlines_info.dat
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/data/spectra_kc13_12_tweak.params
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/data/zphot.param.default
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/igm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/param.py
--rw-r--r--   0 runner    (1001) docker     (123)   226825 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/photoz.py
--rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/sps.py
--rw-r--r--   0 runner    (1001) docker     (123)    49872 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.402124 eazy-0.6.4/eazy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/tests/test_igm.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/tests/test_param.py
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/tests/test_photoz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38961 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-11 11:14:59.000000 eazy-0.6.4/eazy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46541 2023-03-11 11:14:47.000000 eazy-0.6.4/eazy/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.398124 eazy-0.6.4/eazy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-11 11:14:59.000000 eazy-0.6.4/eazy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-11 11:14:59.000000 eazy-0.6.4/eazy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 11:14:59.000000 eazy-0.6.4/eazy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-11 11:14:59.000000 eazy-0.6.4/eazy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-11 11:14:59.000000 eazy-0.6.4/eazy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-11 11:14:47.000000 eazy-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-11 11:14:47.000000 eazy-0.6.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:14:59.402124 eazy-0.6.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-11 11:14:47.000000 eazy-0.6.4/scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-03-11 11:14:47.000000 eazy-0.6.4/scripts/nmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-11 11:14:47.000000 eazy-0.6.4/scripts/photoz.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-03-11 11:14:47.000000 eazy-0.6.4/scripts/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-03-11 11:14:47.000000 eazy-0.6.4/scripts/sps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-11 11:14:59.402124 eazy-0.6.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 11:14:47.000000 eazy-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.052916 eazy-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.032915 eazy-0.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.036915 eazy-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-05 15:28:22.000000 eazy-0.6.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-05 15:28:22.000000 eazy-0.6.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-05 15:28:22.000000 eazy-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:22.000000 eazy-0.6.5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-05 15:28:22.000000 eazy-0.6.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 15:28:22.000000 eazy-0.6.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-05 15:28:22.000000 eazy-0.6.5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 15:28:22.000000 eazy-0.6.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 15:28:22.000000 eazy-0.6.5/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-05 15:28:37.052916 eazy-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-05 15:28:22.000000 eazy-0.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.036915 eazy-0.6.5/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-05 15:28:22.000000 eazy-0.6.5/binder/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.036915 eazy-0.6.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.032915 eazy-0.6.5/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.036915 eazy-0.6.5/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.040915 eazy-0.6.5/docs/eazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36073 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/photoz.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/eazy/zout_columns.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.044916 eazy-0.6.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)  2836689 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/examples/HDFN-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   330296 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/examples/Riverside-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1966244 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/examples/compare_sps_algorithm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   590683 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/examples/dash_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-05 15:28:22.000000 eazy-0.6.5/docs/rtd-pip-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.048916 eazy-0.6.5/eazy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.052916 eazy-0.6.5/eazy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/DLAcoeff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/LAFcoeff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   273600 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/alpha_lyr_stis_008.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/emlines_info.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/spectra_kc13_12_tweak.params
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/data/zphot.param.default
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/igm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)   226826 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/photoz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/sps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50015 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.052916 eazy-0.6.5/eazy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_igm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_photoz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38961 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 15:28:36.000000 eazy-0.6.5/eazy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46541 2023-06-05 15:28:22.000000 eazy-0.6.5/eazy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.048916 eazy-0.6.5/eazy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-05 15:28:36.000000 eazy-0.6.5/eazy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-05 15:28:37.000000 eazy-0.6.5/eazy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:28:36.000000 eazy-0.6.5/eazy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-05 15:28:36.000000 eazy-0.6.5/eazy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 15:28:36.000000 eazy-0.6.5/eazy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-05 15:28:22.000000 eazy-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-05 15:28:22.000000 eazy-0.6.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:28:37.052916 eazy-0.6.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 15:28:22.000000 eazy-0.6.5/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-06-05 15:28:22.000000 eazy-0.6.5/scripts/nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-05 15:28:22.000000 eazy-0.6.5/scripts/photoz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-05 15:28:22.000000 eazy-0.6.5/scripts/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-06-05 15:28:22.000000 eazy-0.6.5/scripts/sps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-05 15:28:37.052916 eazy-0.6.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-06-05 15:28:22.000000 eazy-0.6.5/setup.py
```

### Comparing `eazy-0.6.4/.github/workflows/publish-to-pypi.yml` & `eazy-0.6.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/.github/workflows/python-package.yml` & `eazy-0.6.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/.gitignore` & `eazy-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/.readthedocs.yml` & `eazy-0.6.5/.readthedocs.yml`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     python: "3.10"
     
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   configuration: docs/conf.py
 
 # Optionally build your docs in additional formats such as PDF and ePub
-formats: all
+formats:
+    - htmlzip
 
 python:
   install:
     - method: pip
       path: .
       extra_requirements:
         - docs
```

### Comparing `eazy-0.6.4/CITATION.cff` & `eazy-0.6.5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/LICENSE.txt` & `eazy-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/PKG-INFO` & `eazy-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eazy
-Version: 0.6.4
+Version: 0.6.5
 Summary: Pythonic photo-zs
 Home-page: https://github.com/gbrammer/eazy-py
 Author: G. Brammer
 Author-email: gbrammer@gmail.com
 License: MIT
 Project-URL: Documentation, https://eazy-py.readthedocs.io/
 Project-URL: Source, https://github.com/gbrammer/eazy-py
```

### Comparing `eazy-0.6.4/README.rst` & `eazy-0.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/Makefile` & `eazy-0.6.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/conf.py` & `eazy-0.6.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/eazy/filters.rst` & `eazy-0.6.5/docs/eazy/filters.rst`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/eazy/install.rst` & `eazy-0.6.5/docs/eazy/install.rst`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/eazy/templates.rst` & `eazy-0.6.5/docs/eazy/templates.rst`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/eazy/zout_columns.rst` & `eazy-0.6.5/docs/eazy/zout_columns.rst`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/examples/HDFN-demo.ipynb` & `eazy-0.6.5/docs/examples/HDFN-demo.ipynb`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/examples/Riverside-demo.ipynb` & `eazy-0.6.5/docs/examples/Riverside-demo.ipynb`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/examples/compare_sps_algorithm.ipynb` & `eazy-0.6.5/docs/examples/compare_sps_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/examples/dash_viewer.png` & `eazy-0.6.5/docs/examples/dash_viewer.png`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/index.rst` & `eazy-0.6.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/docs/make.bat` & `eazy-0.6.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/__init__.py` & `eazy-0.6.5/eazy/__init__.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/data/DLAcoeff.txt` & `eazy-0.6.5/eazy/data/DLAcoeff.txt`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/data/LAFcoeff.txt` & `eazy-0.6.5/eazy/data/LAFcoeff.txt`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/data/alpha_lyr_stis_008.fits` & `eazy-0.6.5/eazy/data/alpha_lyr_stis_008.fits`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/data/emlines_info.dat` & `eazy-0.6.5/eazy/data/emlines_info.dat`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/data/zphot.param.default` & `eazy-0.6.5/eazy/data/zphot.param.default`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/filters.py` & `eazy-0.6.5/eazy/filters.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/hdf5.py` & `eazy-0.6.5/eazy/hdf5.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/igm.py` & `eazy-0.6.5/eazy/igm.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/param.py` & `eazy-0.6.5/eazy/param.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/photoz.py` & `eazy-0.6.5/eazy/photoz.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,15 +619,15 @@
             else:
                 print('Read CATALOG_FILE:', self.param['CATALOG_FILE'])
              
         if hasattr(self.param['CATALOG_FILE'], 'colnames'):
             self.cat = self.param['CATALOG_FILE']
         elif 'fits' in self.param['CATALOG_FILE'].lower():
             self.cat = Table.read(self.param['CATALOG_FILE'], format='fits')
-        elif self.param['CATALOG_FILE'].lower().endswith('csv'):
+        elif self.param['CATALOG_FILE'].lower().endswith('.csv'):
             self.cat = Table.read(self.param['CATALOG_FILE'], format='csv')        
         else:
             self.cat = Table.read(self.param['CATALOG_FILE'], 
                                   format=self.param['CATALOG_FORMAT'])
         
         if verbose:
             print(f'   >>> NOBJ = {len(self.cat)}')
```

### Comparing `eazy-0.6.4/eazy/sps.py` & `eazy-0.6.5/eazy/sps.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/templates.py` & `eazy-0.6.5/eazy/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1394,15 +1394,19 @@
         tstars += load_sonora_stars()
         
     return tstars
 
 
 def load_sonora_stars():
     """
-    Load Sonora brown dwarf models
+    Load Sonora brown dwarf models: Marley et al. (2018, 
+    https://zenodo.org/record/1309035)
+    
+    Get the templates from https://github.com/gbrammer/eazy-py/pull/33
+    
     """
     import glob
     
     paths = ['/tmp', './templates/', './']
     found = False
     
     for path in paths:
```

### Comparing `eazy-0.6.4/eazy/tests/test_filters.py` & `eazy-0.6.5/eazy/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/tests/test_igm.py` & `eazy-0.6.5/eazy/tests/test_igm.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/tests/test_param.py` & `eazy-0.6.5/eazy/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/tests/test_photoz.py` & `eazy-0.6.5/eazy/tests/test_photoz.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/tests/test_templates.py` & `eazy-0.6.5/eazy/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/tests/test_utils.py` & `eazy-0.6.5/eazy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/utils.py` & `eazy-0.6.5/eazy/utils.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy/visualization.py` & `eazy-0.6.5/eazy/visualization.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/eazy.egg-info/PKG-INFO` & `eazy-0.6.5/eazy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eazy
-Version: 0.6.4
+Version: 0.6.5
 Summary: Pythonic photo-zs
 Home-page: https://github.com/gbrammer/eazy-py
 Author: G. Brammer
 Author-email: gbrammer@gmail.com
 License: MIT
 Project-URL: Documentation, https://eazy-py.readthedocs.io/
 Project-URL: Source, https://github.com/gbrammer/eazy-py
```

### Comparing `eazy-0.6.4/eazy.egg-info/SOURCES.txt` & `eazy-0.6.5/eazy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/requirements.txt` & `eazy-0.6.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/scripts/nmf.py` & `eazy-0.6.5/scripts/nmf.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/scripts/photoz.py` & `eazy-0.6.5/scripts/photoz.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/scripts/run.py` & `eazy-0.6.5/scripts/run.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/scripts/sps.py` & `eazy-0.6.5/scripts/sps.py`

 * *Files identical despite different names*

### Comparing `eazy-0.6.4/setup.cfg` & `eazy-0.6.5/setup.cfg`

 * *Files identical despite different names*

