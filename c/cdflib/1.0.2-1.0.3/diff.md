# Comparing `tmp/cdflib-1.0.2.tar.gz` & `tmp/cdflib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdflib-1.0.2.tar", last modified: Fri Jun  2 12:39:11 2023, max compression
+gzip compressed data, was "cdflib-1.0.3.tar", last modified: Mon Jun  5 11:09:46 2023, max compression
```

## Comparing `cdflib-1.0.2.tar` & `cdflib-1.0.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.040321 cdflib-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.032322 cdflib-1.0.2/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-02 12:38:50.000000 cdflib-1.0.2/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-02 12:38:50.000000 cdflib-1.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-02 12:38:50.000000 cdflib-1.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.028322 cdflib-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.032322 cdflib-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-02 12:38:50.000000 cdflib-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-02 12:38:50.000000 cdflib-1.0.2/.github/workflows/pypi-build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-02 12:38:50.000000 cdflib-1.0.2/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-02 12:38:50.000000 cdflib-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-02 12:38:50.000000 cdflib-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-02 12:38:50.000000 cdflib-1.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-02 12:38:50.000000 cdflib-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 12:38:50.000000 cdflib-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-02 12:39:11.040321 cdflib-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-02 12:38:50.000000 cdflib-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.032322 cdflib-1.0.2/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 12:38:50.000000 cdflib-1.0.2/archive/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-02 12:38:50.000000 cdflib-1.0.2/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.032322 cdflib-1.0.2/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 12:38:50.000000 cdflib-1.0.2/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-02 12:38:50.000000 cdflib-1.0.2/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.036321 cdflib-1.0.2/cdflib/
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/CDFLeapSeconds.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 12:39:10.000000 cdflib-1.0.2/cdflib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    84619 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/cdfread.py
--rw-r--r--   0 runner    (1001) docker     (123)   104337 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/cdfwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    65531 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/epochs_astropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.036321 cdflib-1.0.2/cdflib/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37917 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/xarray/cdf_to_xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    32046 2023-06-02 12:38:50.000000 cdflib-1.0.2/cdflib/xarray/xarray_to_cdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.036321 cdflib-1.0.2/cdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-02 12:39:10.000000 cdflib-1.0.2/cdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-02 12:39:11.000000 cdflib-1.0.2/cdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:39:10.000000 cdflib-1.0.2/cdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-02 12:39:10.000000 cdflib-1.0.2/cdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 12:39:10.000000 cdflib-1.0.2/cdflib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.036321 cdflib-1.0.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.040321 cdflib-1.0.2/doc/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/modules/cdfepoch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/modules/cdfread.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/modules/cdfwrite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/modules/dataclasses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/modules/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-02 12:38:50.000000 cdflib-1.0.2/doc/modules/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 12:38:50.000000 cdflib-1.0.2/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-02 12:38:50.000000 cdflib-1.0.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-02 12:38:50.000000 cdflib-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-02 12:39:11.040321 cdflib-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.040321 cdflib-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-02 12:38:50.000000 cdflib-1.0.2/tests/test_astropy_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-02 12:38:50.000000 cdflib-1.0.2/tests/test_cdfread.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-02 12:38:50.000000 cdflib-1.0.2/tests/test_cdfread_rle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-06-02 12:38:50.000000 cdflib-1.0.2/tests/test_cdfwrite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-06-02 12:38:50.000000 cdflib-1.0.2/tests/test_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-06-02 12:38:50.000000 cdflib-1.0.2/tests/test_xarray_reader_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:39:11.040321 cdflib-1.0.2/tests/testfiles/
--rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-06-02 12:38:50.000000 cdflib-1.0.2/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
--rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-06-02 12:38:50.000000 cdflib-1.0.2/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-02 12:38:50.000000 cdflib-1.0.2/tests/testfiles/testing_file_location.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-02 12:38:50.000000 cdflib-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.155523 cdflib-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-05 11:09:32.000000 cdflib-1.0.3/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 11:09:32.000000 cdflib-1.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.147523 cdflib-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-05 11:09:32.000000 cdflib-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-05 11:09:32.000000 cdflib-1.0.3/.github/workflows/pypi-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-05 11:09:32.000000 cdflib-1.0.3/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 11:09:32.000000 cdflib-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-05 11:09:32.000000 cdflib-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-05 11:09:32.000000 cdflib-1.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-05 11:09:32.000000 cdflib-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 11:09:32.000000 cdflib-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-05 11:09:46.155523 cdflib-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-05 11:09:32.000000 cdflib-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-05 11:09:32.000000 cdflib-1.0.3/archive/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-05 11:09:32.000000 cdflib-1.0.3/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:32.000000 cdflib-1.0.3/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-05 11:09:32.000000 cdflib-1.0.3/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/cdflib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/CDFLeapSeconds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84457 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104337 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/cdfwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65531 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/epochs_astropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/cdflib/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37917 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/xarray/cdf_to_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32046 2023-06-05 11:09:32.000000 cdflib-1.0.3/cdflib/xarray/xarray_to_cdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.151523 cdflib-1.0.3/cdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 11:09:46.000000 cdflib-1.0.3/cdflib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 11:09:32.000000 cdflib-1.0.3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.155523 cdflib-1.0.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.155523 cdflib-1.0.3/doc/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/cdfepoch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/cdfread.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/cdfwrite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/dataclasses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-05 11:09:32.000000 cdflib-1.0.3/doc/modules/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-05 11:09:32.000000 cdflib-1.0.3/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-05 11:09:32.000000 cdflib-1.0.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-05 11:09:32.000000 cdflib-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-05 11:09:46.155523 cdflib-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.155523 cdflib-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_astropy_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_cdfread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_cdfread_rle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16228 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_cdfwrite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9647 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/test_xarray_reader_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:09:46.155523 cdflib-1.0.3/tests/testfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)   125566 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)    70003 2023-06-05 11:09:32.000000 cdflib-1.0.3/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-05 11:09:32.000000 cdflib-1.0.3/tox.ini
```

### Comparing `cdflib-1.0.2/.circleci/config.yml` & `cdflib-1.0.3/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/.github/workflows/ci.yml` & `cdflib-1.0.3/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
         python-version: ['3.8', '3.9', '3.10', '3.11']
     steps:
     - uses: actions/checkout@v3
 
-    - uses: actions/setup-python@v3
+    - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install package and test requirements
       run: |
-        pip install .[tests]
+        pip install -e .[tests]
         pip check
 
     - name: Run tests
       run: pytest --cov=cdflib
 
     - name: Upload code coverage
-      uses: codecov/codecov-action@v2
+      uses: codecov/codecov-action@v3
```

### Comparing `cdflib-1.0.2/.github/workflows/pypi-build.yaml` & `cdflib-1.0.3/.github/workflows/pypi-build.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/.pre-commit-config.yaml` & `cdflib-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/.readthedocs.yml` & `cdflib-1.0.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/LICENSE` & `cdflib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/PKG-INFO` & `cdflib-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.0.2/README.md` & `cdflib-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/asv.conf.json` & `cdflib-1.0.3/asv.conf.json`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/benchmarks/benchmarks.py` & `cdflib-1.0.3/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/cdflib/CDFLeapSeconds.txt` & `cdflib-1.0.3/cdflib/CDFLeapSeconds.txt`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/cdflib/cdfread.py` & `cdflib-1.0.3/cdflib/cdfread.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,22 +513,22 @@
                 entries.append(entryData)
 
             return_dict[adr_info.name] = entries
             byte_loc = adr_info.next_adr_loc
 
         return return_dict
 
-    def varattsget(self, variable: Optional[str] = None) -> Dict[str, Union[None, str, np.ndarray]]:
+    def varattsget(self, variable: Union[str, int]) -> Dict[str, Union[None, str, np.ndarray]]:
         """
         Gets all variable attributes.
 
         Unlike attget, which returns a single attribute entry value,
         this function returns all of the variable attribute entries,
         in a dictionary (in the form of 'attribute': value pair) for
-        a variable. If there is no entry found, None is returned.
+        a variable.
         """
         if isinstance(variable, int) and self._num_zvariable > 0 and self._num_rvariable > 0:
             raise ValueError("This CDF has both r and z variables. Use variable name")
         if isinstance(variable, str):
             position = self._first_zvariable
             num_variables = self._num_zvariable
             for zVar in [True, False]:
@@ -547,16 +547,14 @@
                 zVar = True
             else:
                 num_variable = self._num_rvariable
                 zVar = False
             if variable < 0 or variable >= num_variable:
                 raise ValueError(f"No variable by this number: {variable}")
             return self._read_varatts(variable, zVar)
-        else:
-            raise ValueError("Please set variable keyword equal to " "the name or number of an variable")
 
     def _uncompress_rle(self, data: bytes) -> bytearray:
         result = bytearray()
         index = 0
         while index < len(data):
             value = data[index]
             if value == 0:
@@ -1303,17 +1301,18 @@
                 else:
                     dim_varys.append(True)
             for x in range(0, len(dim_varys)):
                 dim_sizes.append(self._rvariables_dim_sizes[x])
             num_dims = len(dim_sizes)
             coff = 124 + toadd + 4 * self._rvariables_num_dims
         # Only set if pad value is in the flags
+        pad: Union[None, str, np.ndarray] = None
         if pad_bool:
             byte_stream = vdr[coff:]
-            pad: Union[str, np.ndarray]
+
             try:
                 pad = self._read_data(byte_stream, data_type, 1, num_elements)
             except Exception:
                 if data_type == 51 or data_type == 52:
                     pad = " " * num_elements
 
         if section_type == 8:
```

### Comparing `cdflib-1.0.2/cdflib/cdfwrite.py` & `cdflib-1.0.3/cdflib/cdfwrite.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/cdflib/dataclasses.py` & `cdflib-1.0.3/cdflib/dataclasses.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/cdflib/epochs.py` & `cdflib-1.0.3/cdflib/epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/cdflib/epochs_astropy.py` & `cdflib-1.0.3/cdflib/epochs_astropy.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/cdflib/s3.py` & `cdflib-1.0.3/cdflib/s3.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/cdflib/xarray/cdf_to_xarray.py` & `cdflib-1.0.3/cdflib/xarray/cdf_to_xarray.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/cdflib/xarray/xarray_to_cdf.py` & `cdflib-1.0.3/cdflib/xarray/xarray_to_cdf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/cdflib.egg-info/PKG-INFO` & `cdflib-1.0.3/cdflib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdflib
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python CDF reader toolkit
 Home-page: https://github.com/MAVENSDC/cdflib
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: CDF,maven,lasp,PDS,GSFC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `cdflib-1.0.2/cdflib.egg-info/SOURCES.txt` & `cdflib-1.0.3/cdflib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-.coveragerc
 .flake8
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 MANIFEST.in
 README.md
 asv.conf.json
+codecov.yml
 meta.yaml
 mypy.ini
 pyproject.toml
 setup.cfg
 tox.ini
 .circleci/config.yml
 .github/workflows/ci.yml
@@ -51,10 +51,10 @@
 doc/modules/xarray.rst
 tests/test_astropy_epochs.py
 tests/test_cdfread.py
 tests/test_cdfread_rle.py
 tests/test_cdfwrite.py
 tests/test_epochs.py
 tests/test_xarray_reader_writer.py
+tests/testfiles/de2_ion2s_rpa_19830213_v01.cdf
 tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf
-tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
-tests/testfiles/testing_file_location.txt
+tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
```

### Comparing `cdflib-1.0.2/doc/Makefile` & `cdflib-1.0.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/doc/changelog.rst` & `cdflib-1.0.3/doc/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+1.0.3
+=====
+- The ``variable`` parameter to `cdflib.cdfread.CDF.varattsget` is no longer optional.
+  Not specifying it raised an error anyway in previous versions of cdflib.
+- Fixed an error loading CDF files without a pad value set.
+
 1.0.2
 =====
 To make the ``xarray`` functionality easier to discover and import, a new
 ``cdflib.xarray`` namespace has been added. This means the recommended
 way to import the xarray functionality is now
 ``from cdflib.xarray import cdf_to_xarray, xarray_to_cdf``
```

### Comparing `cdflib-1.0.2/doc/conf.py` & `cdflib-1.0.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/doc/index.rst` & `cdflib-1.0.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/doc/make.bat` & `cdflib-1.0.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/doc/modules/cdfepoch.rst` & `cdflib-1.0.3/doc/modules/cdfepoch.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/doc/modules/cdfread.rst` & `cdflib-1.0.3/doc/modules/cdfread.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/doc/modules/cdfwrite.rst` & `cdflib-1.0.3/doc/modules/cdfwrite.rst`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/meta.yaml` & `cdflib-1.0.3/meta.yaml`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/mypy.ini` & `cdflib-1.0.3/mypy.ini`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/setup.cfg` & `cdflib-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/tests/test_astropy_epochs.py` & `cdflib-1.0.3/tests/test_astropy_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/tests/test_cdfwrite.py` & `cdflib-1.0.3/tests/test_cdfwrite.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/tests/test_epochs.py` & `cdflib-1.0.3/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/tests/test_xarray_reader_writer.py` & `cdflib-1.0.3/tests/test_xarray_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf` & `cdflib-1.0.3/tests/testfiles/fa_esa_l2_eeb_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `cdflib-1.0.2/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf` & `cdflib-1.0.3/tests/testfiles/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf`

 * *Files identical despite different names*

