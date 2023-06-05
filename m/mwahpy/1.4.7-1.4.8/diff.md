# Comparing `tmp/mwahpy-1.4.7.tar.gz` & `tmp/mwahpy-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwahpy-1.4.7.tar", last modified: Fri Mar 10 20:15:51 2023, max compression
+gzip compressed data, was "mwahpy-1.4.8.tar", last modified: Mon Jun  5 15:10:50 2023, max compression
```

## Comparing `mwahpy-1.4.7.tar` & `mwahpy-1.4.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-03-10 20:15:51.791995 mwahpy-1.4.7/
-drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-03-10 20:15:51.735996 mwahpy-1.4.7/.github/
-drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-03-10 20:15:51.735996 mwahpy-1.4.7/.github/workflows/
--rw-rw-r--   0 donlon    (1000) donlon    (1000)      983 2022-03-23 22:02:28.000000 mwahpy-1.4.7/.github/workflows/python-publish.yml
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1074 2022-03-23 22:02:28.000000 mwahpy-1.4.7/LICENSE.txt
--rw-rw-r--   0 donlon    (1000) donlon    (1000)       42 2022-03-23 22:02:28.000000 mwahpy-1.4.7/MANIFEST.in
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     4608 2023-03-10 20:15:51.791995 mwahpy-1.4.7/PKG-INFO
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     4138 2023-02-15 14:56:48.000000 mwahpy-1.4.7/README.md
-drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-03-10 20:15:51.735996 mwahpy-1.4.7/__pycache__/
--rw-rw-r--   0 donlon    (1000) donlon    (1000)      435 2022-03-23 22:02:28.000000 mwahpy-1.4.7/__pycache__/flags.cpython-35.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1212 2022-03-23 22:02:28.000000 mwahpy-1.4.7/__pycache__/mwahpy_global.cpython-35.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)      860 2022-03-23 22:02:28.000000 mwahpy-1.4.7/__pycache__/setup.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     7066 2023-03-10 18:30:56.000000 mwahpy-1.4.7/changelog.txt
-drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-03-10 20:15:51.767995 mwahpy-1.4.7/doc/
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     3861 2022-03-23 22:02:28.000000 mwahpy-1.4.7/doc/doc.aux
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1143 2022-03-23 22:02:28.000000 mwahpy-1.4.7/doc/doc.listing
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    53207 2022-03-23 22:02:28.000000 mwahpy-1.4.7/doc/doc.log
--rw-rw-r--   0 donlon    (1000) donlon    (1000)   339041 2022-03-23 22:02:28.000000 mwahpy-1.4.7/doc/doc.pdf
--rw-rw-r--   0 donlon    (1000) donlon    (1000)   547336 2022-03-23 22:02:28.000000 mwahpy-1.4.7/doc/doc.synctex.gz
--rw-rw-r--   0 donlon    (1000) donlon    (1000)   133831 2022-03-23 22:02:28.000000 mwahpy-1.4.7/doc/doc.tex
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     2903 2022-03-23 22:02:28.000000 mwahpy-1.4.7/doc/doc.toc
-drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-03-10 20:15:51.771995 mwahpy-1.4.7/mwahpy/
--rw-rw-r--   0 donlon    (1000) donlon    (1000)        0 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__init__.py
-drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-03-10 20:15:51.787995 mwahpy-1.4.7/mwahpy/__pycache__/
--rw-rw-r--   0 donlon    (1000) donlon    (1000)      136 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/__init__.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    18064 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/coords.cpython-35.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    14719 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/coords.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     7260 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/data.cpython-35.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    13230 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/data.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)      289 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/flags.cpython-35.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)      278 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/flags.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)      984 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/glob.cpython-35.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1010 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/mwahpy_glob.cpython-35.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1136 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/mwahpy_glob.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1626 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/mwahpy_global.cpython-35.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1957 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/nbody.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    10004 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/orbit_fitter.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     7282 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/orbit_fitter_gc.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     9509 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/orbit_fitting.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    11181 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/orbit_fitting_gc.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     9744 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/orbit_fitting_gc_new.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     2077 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/output_handler.cpython-35.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     4359 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/output_handler.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1980 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/plot.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1299 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/pot.cpython-35.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1274 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/pot.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    15131 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/__pycache__/timestep.cpython-36.pyc
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    30651 2023-03-10 20:11:28.000000 mwahpy-1.4.7/mwahpy/coords.py
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     2582 2022-03-24 18:02:11.000000 mwahpy-1.4.7/mwahpy/flags.py
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     2609 2022-03-30 20:30:05.000000 mwahpy-1.4.7/mwahpy/mwahpy_glob.py
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     3561 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/nbody.py
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    19303 2022-10-28 21:26:57.000000 mwahpy-1.4.7/mwahpy/orbit_fitter.py
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    13158 2022-10-20 15:02:53.000000 mwahpy-1.4.7/mwahpy/orbit_fitter_gc.py
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     8586 2022-09-24 19:01:34.000000 mwahpy-1.4.7/mwahpy/output_handler.py
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     8993 2023-03-10 16:05:04.000000 mwahpy-1.4.7/mwahpy/plot.py
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1698 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy/pot.py
--rw-rw-r--   0 donlon    (1000) donlon    (1000)    33989 2023-02-27 22:00:11.000000 mwahpy-1.4.7/mwahpy/timestep.py
-drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-03-10 20:15:51.771995 mwahpy-1.4.7/mwahpy.egg-info/
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     4608 2023-03-10 20:15:51.000000 mwahpy-1.4.7/mwahpy.egg-info/PKG-INFO
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     1818 2023-03-10 20:15:51.000000 mwahpy-1.4.7/mwahpy.egg-info/SOURCES.txt
--rw-rw-r--   0 donlon    (1000) donlon    (1000)        1 2023-03-10 20:15:51.000000 mwahpy-1.4.7/mwahpy.egg-info/dependency_links.txt
--rw-rw-r--   0 donlon    (1000) donlon    (1000)       37 2023-03-10 20:15:51.000000 mwahpy-1.4.7/mwahpy.egg-info/requires.txt
--rw-rw-r--   0 donlon    (1000) donlon    (1000)       20 2023-03-10 20:15:51.000000 mwahpy-1.4.7/mwahpy.egg-info/top_level.txt
-drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-03-10 20:15:51.787995 mwahpy-1.4.7/mwahpy_tests/
--rw-rw-r--   0 donlon    (1000) donlon    (1000)        0 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy_tests/__init__.py
-drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-03-10 20:15:51.791995 mwahpy-1.4.7/mwahpy_tests/nbody_test/
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     3245 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy_tests/nbody_test/1
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     3252 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy_tests/nbody_test/2
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     3252 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy_tests/nbody_test/3
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     7627 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy_tests/test.py
--rw-rw-r--   0 donlon    (1000) donlon    (1000)     3245 2022-03-23 22:02:28.000000 mwahpy-1.4.7/mwahpy_tests/test_bodies.out
--rw-rw-r--   0 donlon    (1000) donlon    (1000)       38 2023-03-10 20:15:51.791995 mwahpy-1.4.7/setup.cfg
--rw-rw-r--   0 donlon    (1000) donlon    (1000)      838 2023-03-10 20:13:28.000000 mwahpy-1.4.7/setup.py
+drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-06-05 15:10:50.115419 mwahpy-1.4.8/
+drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-06-05 15:10:50.011420 mwahpy-1.4.8/.github/
+drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-06-05 15:10:50.015420 mwahpy-1.4.8/.github/workflows/
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)      983 2022-03-23 22:02:28.000000 mwahpy-1.4.8/.github/workflows/python-publish.yml
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1074 2022-03-23 22:02:28.000000 mwahpy-1.4.8/LICENSE.txt
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)       42 2022-03-23 22:02:28.000000 mwahpy-1.4.8/MANIFEST.in
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     4608 2023-06-05 15:10:50.115419 mwahpy-1.4.8/PKG-INFO
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     4138 2023-02-15 14:56:48.000000 mwahpy-1.4.8/README.md
+drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-06-05 15:10:50.015420 mwahpy-1.4.8/__pycache__/
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)      435 2022-03-23 22:02:28.000000 mwahpy-1.4.8/__pycache__/flags.cpython-35.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1212 2022-03-23 22:02:28.000000 mwahpy-1.4.8/__pycache__/mwahpy_global.cpython-35.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)      860 2022-03-23 22:02:28.000000 mwahpy-1.4.8/__pycache__/setup.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     7457 2023-06-05 15:02:58.000000 mwahpy-1.4.8/changelog.txt
+drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-06-05 15:10:50.087419 mwahpy-1.4.8/doc/
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     3861 2022-03-23 22:02:28.000000 mwahpy-1.4.8/doc/doc.aux
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1143 2022-03-23 22:02:28.000000 mwahpy-1.4.8/doc/doc.listing
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    53207 2022-03-23 22:02:28.000000 mwahpy-1.4.8/doc/doc.log
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)   339041 2022-03-23 22:02:28.000000 mwahpy-1.4.8/doc/doc.pdf
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)   547336 2022-03-23 22:02:28.000000 mwahpy-1.4.8/doc/doc.synctex.gz
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)   133831 2022-03-23 22:02:28.000000 mwahpy-1.4.8/doc/doc.tex
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     2903 2022-03-23 22:02:28.000000 mwahpy-1.4.8/doc/doc.toc
+drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-06-05 15:10:50.095420 mwahpy-1.4.8/mwahpy/
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)        0 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__init__.py
+drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-06-05 15:10:50.111419 mwahpy-1.4.8/mwahpy/__pycache__/
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)      136 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    18064 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/coords.cpython-35.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    14719 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/coords.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     7260 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/data.cpython-35.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    13230 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/data.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)      289 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/flags.cpython-35.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)      278 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/flags.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)      984 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/glob.cpython-35.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1010 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/mwahpy_glob.cpython-35.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1136 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/mwahpy_glob.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1626 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/mwahpy_global.cpython-35.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1957 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/nbody.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    10004 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/orbit_fitter.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     7282 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/orbit_fitter_gc.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     9509 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/orbit_fitting.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    11181 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/orbit_fitting_gc.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     9744 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/orbit_fitting_gc_new.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     2077 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/output_handler.cpython-35.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     4359 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/output_handler.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1980 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/plot.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1299 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/pot.cpython-35.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1274 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/pot.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    15131 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/__pycache__/timestep.cpython-36.pyc
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    29430 2023-05-31 00:32:14.000000 mwahpy-1.4.8/mwahpy/coords.py
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     2582 2022-03-24 18:02:11.000000 mwahpy-1.4.8/mwahpy/flags.py
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     2609 2022-03-30 20:30:05.000000 mwahpy-1.4.8/mwahpy/mwahpy_glob.py
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     3561 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/nbody.py
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    19303 2022-10-28 21:26:57.000000 mwahpy-1.4.8/mwahpy/orbit_fitter.py
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    13158 2022-10-20 15:02:53.000000 mwahpy-1.4.8/mwahpy/orbit_fitter_gc.py
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     8586 2022-09-24 19:01:34.000000 mwahpy-1.4.8/mwahpy/output_handler.py
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     8993 2023-03-10 16:05:04.000000 mwahpy-1.4.8/mwahpy/plot.py
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1698 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy/pot.py
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)    33989 2023-05-23 17:47:22.000000 mwahpy-1.4.8/mwahpy/timestep.py
+drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-06-05 15:10:50.095420 mwahpy-1.4.8/mwahpy.egg-info/
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     4608 2023-06-05 15:10:49.000000 mwahpy-1.4.8/mwahpy.egg-info/PKG-INFO
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     1818 2023-06-05 15:10:49.000000 mwahpy-1.4.8/mwahpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)        1 2023-06-05 15:10:49.000000 mwahpy-1.4.8/mwahpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)       37 2023-06-05 15:10:49.000000 mwahpy-1.4.8/mwahpy.egg-info/requires.txt
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)       20 2023-06-05 15:10:49.000000 mwahpy-1.4.8/mwahpy.egg-info/top_level.txt
+drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-06-05 15:10:50.111419 mwahpy-1.4.8/mwahpy_tests/
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)        0 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy_tests/__init__.py
+drwxrwxr-x   0 donlon    (1000) donlon    (1000)        0 2023-06-05 15:10:50.111419 mwahpy-1.4.8/mwahpy_tests/nbody_test/
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     3245 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy_tests/nbody_test/1
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     3252 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy_tests/nbody_test/2
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     3252 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy_tests/nbody_test/3
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     7627 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy_tests/test.py
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)     3245 2022-03-23 22:02:28.000000 mwahpy-1.4.8/mwahpy_tests/test_bodies.out
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)       38 2023-06-05 15:10:50.115419 mwahpy-1.4.8/setup.cfg
+-rw-rw-r--   0 donlon    (1000) donlon    (1000)      838 2023-05-30 23:14:20.000000 mwahpy-1.4.8/setup.py
```

### Comparing `mwahpy-1.4.7/.github/workflows/python-publish.yml` & `mwahpy-1.4.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/LICENSE.txt` & `mwahpy-1.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/PKG-INFO` & `mwahpy-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwahpy
-Version: 1.4.7
+Version: 1.4.8
 Summary: A python package for easily parsing and processing data from MilkyWay@home
 Home-page: https://github.com/thomasdonlon/mwahpy
 Author: Tom Donlon
 Author-email: donlot@rpi.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mwahpy-1.4.7/README.md` & `mwahpy-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/__pycache__/mwahpy_global.cpython-35.pyc` & `mwahpy-1.4.8/__pycache__/mwahpy_global.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/__pycache__/setup.cpython-36.pyc` & `mwahpy-1.4.8/__pycache__/setup.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/changelog.txt` & `mwahpy-1.4.8/changelog.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-v1.4.7:
+v1.4.8:
+ - fixed bug in computing vgsr and vr for simulated data
+ - corrected rotation matrix and typo in coords.eq_to_OC_koposov2019()
+ - added inverse coords.OC_to_eq_koposov2019()
+ - added @fix_arrays decorator to coords that makes it a lot easier to implement flexible 
+   array & non-array inputs
+ - added some flexible array/non-array inputs to various coords functions
+
+v1.4.7: (MINOR PATCH)
  - made the goodness-of-fit in orbit_fitter an actual chi-squared
  - fixed type mismatch in coords.pole_rotation_inv
  - added timestep.get_bound_mass()
  - added timestep.check_for_incest()
  - edited github readme
  - split_at_id_wrap works again for new Nbody formatting, added a toggle for user-inputted 
    values for backwards compatability
```

### Comparing `mwahpy-1.4.7/doc/doc.aux` & `mwahpy-1.4.8/doc/doc.aux`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/doc/doc.listing` & `mwahpy-1.4.8/doc/doc.listing`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/doc/doc.log` & `mwahpy-1.4.8/doc/doc.log`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/doc/doc.pdf` & `mwahpy-1.4.8/doc/doc.pdf`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/doc/doc.synctex.gz` & `mwahpy-1.4.8/doc/doc.synctex.gz`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/doc/doc.tex` & `mwahpy-1.4.8/doc/doc.tex`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/doc/doc.toc` & `mwahpy-1.4.8/doc/doc.toc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/coords.cpython-35.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/coords.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/coords.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/coords.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/data.cpython-35.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/data.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/data.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/data.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/glob.cpython-35.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/glob.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/mwahpy_glob.cpython-35.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/mwahpy_glob.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/mwahpy_glob.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/mwahpy_glob.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/mwahpy_global.cpython-35.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/mwahpy_global.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/nbody.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/nbody.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/orbit_fitter.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/orbit_fitter.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/orbit_fitter_gc.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/orbit_fitter_gc.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/orbit_fitting.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/orbit_fitting.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/orbit_fitting_gc.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/orbit_fitting_gc.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/orbit_fitting_gc_new.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/orbit_fitting_gc_new.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/output_handler.cpython-35.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/output_handler.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/output_handler.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/output_handler.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/plot.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/plot.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/pot.cpython-35.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/pot.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/pot.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/pot.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/__pycache__/timestep.cpython-36.pyc` & `mwahpy-1.4.8/mwahpy/__pycache__/timestep.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/coords.py` & `mwahpy-1.4.8/mwahpy/coords.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,41 +6,59 @@
 
 #TODO: Make sure all transformations have inverse transformations
 #TODO: Make sure all transormations have unit tests
 #TODO: (low priority) Allow certain quantities (like galactocentric phi/theta) to be expressed/input in radians
 #TODO: (low priority) add left-handed versions to all galactic cartesian transformations
 
 #===============================================================================
+#TEMPLATE
+#===============================================================================
+#this generically allows functions to take in either arrays or single values
+# and turns everything into arrays behind the scenes
+
+def fix_arrays(func, *args, **kwargs):
+    def wrapper(*args, **kwargs):
+
+        use_array = True
+        if not(isinstance(args[0], np.ndarray)): #check whether the first input is an array (assume all inputs are symmetric)
+            use_array = False
+            args = tuple([np.array([args[i]]) for i in range(len(args))]) #if they aren't, convert the args to arrays
+
+        ret = func(*args) #catches the output from the function
+
+        if not use_array: #convert them back if necessary
+            if not(isinstance(ret, tuple)): #check whether we can actually iterate on the returned values (i.e. whether the func returns a single value or multiple)
+                ret = ret[0]
+            else:
+                ret = tuple([ret[i][0] for i in range(len(ret))])
+
+        return ret
+    return wrapper
+
+#===============================================================================
 #HELPER FUNCTIONS
 #===============================================================================
 #These functions aren't meant to be accessed by outside files or by end users,
 #and as such they are not well documented, named, or tested
 
+@fix_arrays
 def wrap_long(lon, rad=False):
 
     if rad:
         lon = lon * 180/np.pi
 
-    use_array = True
-    if not(isinstance(lon, np.ndarray)):
-        use_array = False
-        lon = np.array([lon])
-
     for i in range(len(lon)):
         if lon[i] < 0:
             lon[i] += 360
         elif lon[i] > 360:
             lon[i] -= 360
 
     if rad:
         lon = lon * np.pi/180
 
-    if not use_array:
-        lon = lon[0]
-
     return lon
 
 #rotate the given data around the provided axis
 #TODO: Allow array-like input
 def rot_around_arb_axis(x, y, z, ux, uy, uz, theta):
     #TODO: Allow radians or degrees
     #x, y, z: 3D cartesian coordinates of the data
@@ -65,41 +83,31 @@
     xyz = np.matmul(R, xyz)
     x = xyz[0]
     y = xyz[1]
     z = xyz[2]
 
     return x, y, z
 
+@fix_arrays
 def long_lat_to_unit_vec(l, b, left_handed=False, rad=False):
 
-    use_array = True
-    if not(isinstance(l, np.ndarray)):
-        use_array = False
-        l = np.array([l])
-        b = np.array([b])
-
     if not rad:
         l = l*np.pi/180
         b = b*np.pi/180
 
     if left_handed:
         #left-handed
         x = -1 * np.cos(l)*np.cos(b)
     else:
         #right-handed
         x = np.cos(l)*np.cos(b)
 
     y = np.sin(l)*np.cos(b)
     z = np.sin(b)
 
-    if not use_array:
-        x = x[0]
-        y = y[0]
-        z = z[0]
-
     return x, y, z
 
 def comp_wise_dot(M, v, normalize=False):
     #performs a component-wise dot product for matrix M of vectors, with vector v
     #if normalize == True, normalize v and each component of M
     tol = 1e-6
 
@@ -119,186 +127,127 @@
 
     return out
 
 #===============================================================================
 #FIRST ORDER COORDINATE/POSITION TRANSFORMATIONS
 #===============================================================================
 
+@fix_arrays
 def cart_to_gal(x, y, z, left_handed=False):
     #get l, b, r (helio) from galactocentric X, Y, Z coords
-    use_array = True
-    if not(isinstance(x, np.ndarray)):
-        use_array = False
-        x = np.array([x])
-        y = np.array([y])
-        z = np.array([z])
 
     if left_handed:
         r = ((x+solar_ps.x)**2 + y**2 + z**2)**0.5
         l = np.arctan2(y,-1*(x-8))*180/np.pi
     else:
         r = ((x-solar_ps.x)**2 + y**2 + z**2)**0.5
         l = np.arctan2(y,(x+8))*180/np.pi
     b = np.arcsin(z/r)*180/np.pi
 
-    if not use_array:
-        l = l[0]
-        b = b[0]
-        r = r[0]
-
     return l, b, r
 
 #-------------------------------------------------------------------------------
 
+@fix_arrays
 def gal_to_cart(l, b, r, left_handed=False, rad=False):
 
-    use_array = True
-    if not(isinstance(l, np.ndarray)):
-        use_array = False
-        l = np.array([l])
-        b = np.array([b])
-        r = np.array([r])
-
     if not rad:
         l = l*np.pi/180
         b = b*np.pi/180
 
     if left_handed:
         #left-handed
         x = -1*solar_ps.x - r*np.cos(l)*np.cos(b)
     else:
         #right-handed
         x = r*np.cos(l)*np.cos(b) + solar_ps.x
 
     y = r*np.sin(l)*np.cos(b)
     z = r*np.sin(b)
 
-    if not use_array:
-        x = x[0]
-        y = y[0]
-        z = z[0]
-
     return x, y, z
 
 #-------------------------------------------------------------------------------
 
 #input: x[kpc], y[kpc], z[kpc]
 #output: Cylindrical coordinates (R, [kpc], Z [kpc], Phi [deg])
 #phi = 0 when oriented along the positive x-axis
+@fix_arrays
 def cart_to_cyl(x, y, z):
 
-    use_array = True
-    if not(isinstance(x, np.ndarray)):
-        use_array = False
-        x = np.array([x])
-        y = np.array([y])
-
     R = (x**2 + y**2)**0.5
     phi = np.arctan2(y, x)*180/np.pi
 
-    if not use_array:
-        R = R[0]
-        phi = phi[0]
-
     return R, z, phi
 
 #-------------------------------------------------------------------------------
 
+@fix_arrays
 def cyl_to_cart(R, z, phi):
 
-    use_array = True
-    if not(isinstance(R, np.ndarray)):
-        use_array = False
-        R = np.array([R])
-        phi = np.array([phi])
-
     phi = phi*np.pi/180
 
     x = R*np.cos(phi)
     y = R*np.sin(phi)
 
-    if not use_array:
-        x = x[0]
-        y = y[0]
-
     return x, y, z
 
 #-------------------------------------------------------------------------------
 
+@fix_arrays
 def cart_to_sph(x, y, z):
 
-    use_array = True
-    if not(isinstance(x, np.ndarray)):
-        use_array = False
-        x = np.array([x])
-        y = np.array([y])
-        z = np.array([z])
-
     r = (x**2 + y**2 + z**2)**0.5
 
     phi = np.arctan2(y, x)*180/np.pi
     theta = np.arcsin(z/r)*180/np.pi
 
-    if not use_array:
-        phi = phi[0]
-        theta = theta[0]
-        r = r[0]
-
     return phi, theta, r
 
 #-------------------------------------------------------------------------------
 
+@fix_arrays
 def sph_to_cart(phi, theta, r):
 
-    use_array = True
-    if not(isinstance(phi, np.ndarray)):
-        use_array = False
-        phi = np.array([phi])
-        theta = np.array([theta])
-        r = np.array([r])
-
     phi = phi*np.pi/180
     theta = theta*np.pi/180
 
     x = r*np.cos(phi)*np.cos(theta)
     y = r*np.sin(phi)*np.cos(theta)
     z = r*np.sin(theta)
 
-    if not use_array:
-        x = x[0]
-        y = y[0]
-        z = z[0]
-
     return x, y, z
 
 #===============================================================================
 #SECOND ORDER COORDINATE/POSITION TRANSFORMATIONS
 #===============================================================================
 
+@fix_arrays
 def cyl_to_gal(R, z, phi):
     x, y, z = cyl_to_cart(R, z, phi)
     l, b, r = cart_to_gal(x, y, z)
     return l, b, r
 
 #-------------------------------------------------------------------------------
 
+@fix_arrays
 def gal_to_cyl(l, b, r):
     x, y, z = gal_to_cart(l, b, r)
     R, z, phi = cart_to_cyl(x, y, z)
     return R, z, phi
 
 #===============================================================================
 #VELOCITY TRANSFORMATIONS
 #===============================================================================
 
 # Input: distance [kpc], radial velocity [km/s], RA/DEC [degrees], and pmRA/pmDEC [mas/yr]
 # Returns: Galactic vx, vy, vz velocities [km/s]
 # NOTE: pmRA = d/dt(RA) * cos(DEC)
-# Arguments should be numpy arrays for most efficient usage
 # Adapted from code written by Alan Pearl
+@fix_arrays
 def get_uvw(ra, dec, dist, rv, pmra, pmde):
 
     # Conversion from Equatorial (J2000) Cartesian to Galactic Cartesian
     EQ2GC = np.array( [[-0.05487572, -0.87343729, -0.48383453],
                       [  0.49410871, -0.44482923,  0.7469821 ],
                       [ -0.86766654, -0.19807649,  0.45598456]], dtype=np.float32 )
 
@@ -320,14 +269,15 @@
     vel_Eq = np.array([ vx_Eq, vy_Eq, vz_Eq ])
     U, V, W = np.dot(EQ2GC, vel_Eq)
 
     return U, V, W
 
 #-------------------------------------------------------------------------------
 
+@fix_arrays
 def get_vxvyvz(ra, dec, dist, rv, pmra, pmde):
 
     U, V, W = get_uvw(ra, dec, dist, rv, pmra, pmde)
 
     # add Sun's velocity
     vx = U + solar_ps.vx
     vy = V + solar_ps.vy
@@ -335,27 +285,17 @@
 
     return vx, vy, vz
 
 #-------------------------------------------------------------------------------
 
 #TODO: Do the linear algebra to avoid a inv calculation, since that's huge time waste
 #solar reflex motion will be already removed if UVW are galactocentric
-#inputs must be arrays, even if just of length 1
+@fix_arrays
 def get_rvpm(ra, dec, dist, U, V, W):
 
-    use_array = True
-    if not(isinstance(ra, np.ndarray)):
-        use_array = False
-        ra = np.array([ra])
-        dec = np.array([dec])
-        dist = np.array([dist])
-        U = np.array([U])
-        V = np.array([V])
-        W = np.array([W])
-
     k = 4.74057
     rv = np.array([0.0]*len(ra))
     pmra = np.array([0.0]*len(ra))
     pmdec = np.array([0.0]*len(ra))
 
     i = 0
     while i < len(ra):
@@ -375,41 +315,53 @@
 
         rv[i] = rvpm[0][0]
         pmra[i] = rvpm[1][0]/dist[i]/k
         pmdec[i] = rvpm[2][0]/dist[i]/k
 
         i += 1
 
-    if not use_array:
-        rv = rv[0]
-        pmra = pmra[0]
-        pmdec = pmdec[0]
-
     return rv, pmra, pmdec
 
 #-------------------------------------------------------------------------------
 
-#inputs must be arrays, even if just of length 1
+@fix_arrays
 def remove_sol_mot_from_pm(ra, dec, dist, pmra, pmdec):
+
     vx = np.array([-solar_ps.vx] * len(ra))
     vy = np.array([-solar_ps.vy] * len(ra))
     vz = np.array([-solar_ps.vz] * len(ra))
 
     rv, mura, mudec = get_rvpm(ra, dec, dist, vx, vy, vz)
 
     #don't directly modify pmra and pmdec
     pmra_new = pmra - mura
     pmdec_new = pmdec - mudec
 
     return pmra_new, pmdec_new
 
 #-------------------------------------------------------------------------------
 
-#does not work for arrays!
-#TODO: make work with arrays
+@fix_arrays
+def add_sol_mot_to_pm(ra, dec, dist, pmra, pmdec):
+
+    vx = np.array([-solar_ps.vx] * len(ra))
+    vy = np.array([-solar_ps.vy] * len(ra))
+    vz = np.array([-solar_ps.vz] * len(ra))
+
+    rv, mura, mudec = get_rvpm(ra, dec, dist, vx, vy, vz)
+
+    #don't directly modify pmra and pmdec
+    pmra_new = pmra + mura
+    pmdec_new = pmdec + mudec
+
+    return pmra_new, pmdec_new
+
+#-------------------------------------------------------------------------------
+
+@fix_arrays
 def get_uvw_errors(dist, ra, dec, pmra, pmdec, err_pmra, err_pmdec, err_rv, err_dist):
     #distance in pc
     k = 4.74057
 
     ra_rad = ra * np.pi/180
     dec_rad = dec * np.pi/180
 
@@ -430,53 +382,35 @@
     err_u = (uvw_var[0][0])**0.5
     err_v = (uvw_var[1][0])**0.5
     err_w = (uvw_var[2][0])**0.5
 
     return err_u, err_v, err_w
 
 #remove solar reflex motion from line of sight velocity
+@fix_arrays
 def vlos_to_vgsr(l, b, vlos):
     #TODO: Allow ra, dec as inputs
 
-    use_array = True
-    if not(isinstance(l, np.ndarray)):
-        use_array = False
-        l = np.array([l])
-        b = np.array([b])
-        vlos = np.array([rv])
-
     l = l * np.pi/180
     b = b * np.pi/180
 
     vgsr = vlos + solar_ps.vx*np.cos(l)*np.cos(b) + solar_ps.vy*np.sin(l)*np.cos(b) + solar_ps.vz*np.sin(b)
 
-    if not use_array:
-        vgsr = vgsr[0]
-
     return vgsr
 
 #add solar reflex motion back into GSR line of sight velocity
+@fix_arrays
 def vgsr_to_vlos(l, b, vgsr):
     #TODO: Allow ra, dec as inputs
 
-    use_array = True
-    if not(isinstance(l, np.ndarray)):
-        use_array = False
-        l = np.array([l])
-        b = np.array([b])
-        vgsr = np.array([vgsr])
-
     l = l * np.pi/180
     b = b * np.pi/180
 
     vlos = vgsr - solar_ps.vx*np.cos(l)*np.cos(b) - solar_ps.vy*np.sin(l)*np.cos(b) - solar_ps.vz*np.sin(b)
 
-    if not use_array:
-        vlos = vlos[0]
-
     return vlos
 
 #=====================================
 #MISC TOOLS
 #=====================================
 
 #-------------------------------------------------------------------------------
@@ -566,14 +500,15 @@
 
     return x, y, z
 
 #-------------------------------------------------------------------------------
 
 #kind of a helper function for the gal_to_lambet and cart_to_lambet functions,
 #although it just finds longitude and latitude of any cartesian system
+@fix_arrays
 def cart_to_lonlat(x, y, z):
     Lam = np.arctan2(y, x)*180/np.pi #convert to degrees
 
     #correct Lam to be between 0 and 360 instead of -180 to 180
     i = 0
     while i < len(Lam):
         if Lam[i] < 0:
@@ -611,14 +546,15 @@
     x_prime, y_prime, z_prime = cart_to_plane(x,y,z, normal=normal, point=point)
     Lam, Bet = cart_to_lonlat(x_prime, y_prime, z_prime)
 
     return Lam, Bet
 
 #-------------------------------------------------------------------------------
 
+# I believe x, y, z can be arrays
 def cart_to_sgr(x,y,z):
 
     x_prime = x_prime - solar_ps.x
     xyz = np.array([x, y, z])
 
     #Euler rotation matrix from Solar frame into Sgr
     phi = 183.8 * np.pi/180
@@ -643,16 +579,15 @@
     Lam = np.arctan2(y, x)*180/np.pi
     Bet = np.arcsin(z/(x**2 + y**2 + z**2)**0.5)*180/np.pi
 
     return Lam, Bet
 
 #-------------------------------------------------------------------------------
 
-#gal2plane: np.array(floats), np.array(floats), np.array(floats), (float, float, float), (float, float, float) --> np.array(floats), np.array(floats)
-#takes in galactic coordinates for a star(s) and returns their Lamba, Beta coordinates with respect to the Sgr stream plane
+#takes in galactic coordinates for a star(s) and returns their Lambda, Beta coordinates with respect to the Sgr stream plane
 def gal_to_sgr(l, b):
     #l, b: Galactic coordinates (can be arrays)
 
     x = np.cos(l*np.pi/180)*np.cos(b*np.pi/180)
     y = np.sin(l*np.pi/180)*np.cos(b*np.pi/180)
     z = np.sin(b*np.pi/180)
     xyz = np.array([x, y, z])
@@ -680,20 +615,16 @@
     Lam = wrap_long(np.arctan2(y, x)*180/np.pi)
     Bet = np.arcsin(z/(x**2 + y**2 + z**2)**0.5)*180/np.pi
 
     return Lam, Bet
 
 #-------------------------------------------------------------------------------
 
-#gal2plane: np.array(floats), np.array(floats), np.array(floats), (float, float, float), (float, float, float) --> np.array(floats), np.array(floats)
-#takes in galactic coordinates for a star(s) and returns their Lamba, Beta coordinates with respect to a rotated plane with the normal vector provided
+#takes in Lambda, Beta coordinates for a star(s) and returns their Galactic coordinates with respect to the Sgr stream plane
 def sgr_to_gal(Lam, Bet):
-    #x, y, z: galactocentric x, y, z coordinates
-    #normal: 3-vector providing the orientation of the plane to rotate into
-    #point: 3-vector 'suggesting' the direction of the new x-axis
 
     x = np.cos(Lam*np.pi/180)*np.cos(Bet*np.pi/180)
     y = np.sin(Lam*np.pi/180)*np.cos(Bet*np.pi/180)
     z = np.sin(Bet*np.pi/180)
     xyz = np.array([x, y, z])
 
     #Euler rotation matrix from Solar frame into Sgr
@@ -823,124 +754,120 @@
 #===============================================================================
 #EXTRA UTILITIES
 #===============================================================================
 
 #euler angle rotation matrix
 #too long to format like I normally would
 #out here because it's used for the transform and inverse transform
+#is it bad to do this outside because it utilizes memory even without using the relevant functions? Probably. It can't be that bad though, right?
 phi = 128.79*np.pi/180
 theta = 54.39*np.pi/180
 psi = 90.70*np.pi/180
 
 newberg2010_ERM = np.array([[(np.cos(psi)*np.cos(phi))-(np.cos(theta)*np.sin(phi)*np.sin(psi)),
                              (np.cos(psi)*np.sin(phi))+(np.cos(theta)*np.cos(phi)*np.sin(psi)),
                              np.sin(psi)*np.sin(theta)],
                             [(-np.sin(psi)*np.cos(phi))-(np.cos(theta)*np.sin(phi)*np.cos(psi)),
                              (-np.sin(psi)*np.sin(phi))+(np.cos(theta)*np.cos(phi)*np.cos(psi)),
                              np.cos(psi)*np.sin(theta)],
                             [np.sin(theta)*np.sin(phi),
                              -np.sin(theta)*np.cos(phi),
                              np.cos(theta)]])
 
+k19_rotmat = np.array([[-0.44761231, -0.08785756, -0.88990128],
+                       [-0.84246097,  0.37511331,  0.38671632],
+                       [ 0.29983786,  0.92280606, -0.24192190]])
+
 #-------------------------------------------------------------------------------
 
 #coordinate transform from (l,b) to Orphan-Chenab Stream (Lambda,Beta) from Newberg et al. (2010)
 #adapted from code by Hiroka Warren
+@fix_arrays
 def gal_to_lambet_newberg2010(l, b):
 
-    use_array = True
-    if not(isinstance(l, np.ndarray)):
-        use_array = False
-        l = np.array([l])
-        b = np.array([b])
-
     l_rad = l*np.pi/180
     b_rad = b*np.pi/180
 
     M2 = np.array([np.cos(b_rad)*np.cos(l_rad),
                    np.cos(b_rad)*np.sin(l_rad),
                    np.sin(b_rad)])
 
     M3 = np.matmul(newberg2010_ERM,M2)
 
     lam = np.arctan2(M3[1], M3[0])*180/np.pi
     bet = np.arcsin(M3[2])*180/np.pi
 
-    if not use_array:
-        lam = lam[0]
-        bet = bet[0]
-
     return lam, bet
 
 #-------------------------------------------------------------------------------
 
 #(inverse) coordinate transform from Orphan-Chenab Stream (Lambda,Beta) to (l,b) from Newberg et al. (2010)
 #adapted from code by Hiroka Warren
+@fix_arrays
 def lambet_to_gal_newberg2010(lam, bet):
 
-    use_array = True
-    if not(isinstance(lam, np.ndarray)):
-        use_array = False
-        lam = np.array([lam])
-        bet = np.array([bet])
-
     inv_M1 = np.linalg.inv(newberg2010_ERM)
 
     lam_rad = lam*np.pi/180
     bet_rad = bet*np.pi/180
 
     M2 = np.array([np.cos(bet_rad)*np.cos(lam_rad),
                    np.cos(bet_rad)*np.sin(lam_rad),
                    np.sin(bet_rad)])
 
     M3 = np.matmul(inv_M1,M2)
 
     l = np.arctan2(M3[1],M3[0])*180/np.pi
     b = np.arcsin(M3[2])*180/np.pi
 
-    if not use_array:
-        l = l[0]
-        b = b[0]
-
     return l, b
 
 #-------------------------------------------------------------------------------
 
 #Conversion from (ra, dec) to (phi1, phi2) for Orphan-Chenab stream as per Koposov et al. (2019)
+@fix_arrays
 def eq_to_OC_koposov2019(ra, dec):
 
-    use_array = True
-    if not(isinstance(ra, np.ndarray)):
-        use_array = False
-        ra = np.array([ra])
-        dec = np.array([dec])
-
-    M1 = np.array([[ 0.455572, -0.165815, -0.874620],
-                   [-0.184451,  0.943594, -0.274968],
-                   [ 0.870880,  0.286592,  0.399290]])
-
     ra_rad = ra*np.pi/180
     dec_rad = dec*np.pi/180
 
     M2 = np.array([np.cos(ra_rad)*np.cos(dec_rad),
                    np.sin(ra_rad)*np.cos(dec_rad),
                    np.sin(dec_rad)])
 
-    M3 = np.matmul(M1,M2)
+    M3 = np.matmul(k19_rotmat,M2)
 
-    phi1 = np.arctan2(M3[1],M3[2])*180/np.pi
+    phi1 = np.arctan2(M3[0],M3[1])*180/np.pi
     phi2 = np.arcsin(M3[2])*180/np.pi
 
-    if not use_array:
-        phi1 = phi1[0]
-        phi2 = phi2[0]
-
     return phi1, phi2
 
 #-------------------------------------------------------------------------------
+
+#Inverse conversion from (phi1, phi2) to (ra, dec) for Orphan-Chenab stream as per Koposov et al. (2019)
+@fix_arrays
+def OC_to_eq_koposov2019(phi1, phi2):
+
+    M1 = np.linalg.inv(k19_rotmat)
+
+    phi1_rad = phi1*np.pi/180
+    phi2_rad = phi2*np.pi/180
+
+    M2 = np.array([np.cos(phi1_rad)*np.cos(phi2_rad),
+                   np.sin(phi1_rad)*np.cos(phi2_rad),
+                   np.sin(phi2_rad)])
+
+    M3 = np.matmul(M1,M2)
+
+    ra = np.arctan2(M3[0],M3[1])*180/np.pi
+    dec = np.arcsin(M3[2])*180/np.pi
+
+    return ra, dec
+
+#-------------------------------------------------------------------------------
 #hard-coded pole_rotation transformations
 
 oc_pole = (72, -14) #koposov et al. (2019) Orphan-Chenab stream transformation (ra, dec)
 oc_origin = (191.10487, 62.86084)
 
 def eq_to_OC(ra, dec, **kwargs):
     return pole_rotation(ra, dec, oc_pole, oc_origin, **kwargs)
```

### Comparing `mwahpy-1.4.7/mwahpy/flags.py` & `mwahpy-1.4.8/mwahpy/flags.py`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/mwahpy_glob.py` & `mwahpy-1.4.8/mwahpy/mwahpy_glob.py`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/nbody.py` & `mwahpy-1.4.8/mwahpy/nbody.py`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/orbit_fitter.py` & `mwahpy-1.4.8/mwahpy/orbit_fitter.py`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/orbit_fitter_gc.py` & `mwahpy-1.4.8/mwahpy/orbit_fitter_gc.py`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/output_handler.py` & `mwahpy-1.4.8/mwahpy/output_handler.py`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/plot.py` & `mwahpy-1.4.8/mwahpy/plot.py`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/pot.py` & `mwahpy-1.4.8/mwahpy/pot.py`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy/timestep.py` & `mwahpy-1.4.8/mwahpy/timestep.py`

 * *Files identical despite different names*

```diff
@@ -306,15 +306,15 @@
         self.lx = self.y * self.vz - self.z * self.vy
         self.ly = self.z * self.vx - self.x * self.vz
         self.lz = self.x * self.vy - self.y * self.vx
         self.lperp = (self.lx**2 + self.ly**2)**0.5
         self.ltot = (self.lx**2 + self.ly**2 + self.lz**2)**0.5
 
         #velocity information
-        self.vgsr = ((self.x+8)*self.vx + self.y*self.vy + self.x*self.vz)/self.dist
+        self.vgsr = ((self.x+8)*self.vx + self.y*self.vy + self.z*self.vz)/self.dist
         self.vlos = self.vgsr - 10.1*np.cos(self.b*np.pi/180)*np.cos(self.l*np.pi/180) - 224*np.cos(self.b*np.pi/180)*np.sin(self.l*np.pi/180) - 6.7*np.sin(self.b*np.pi/180)
         self.vrad = (self.x*self.vx + self.y*self.vy + self.z*self.vz)/self.r
         self.vrot = self.lz/(self.x**2 + self.y**2)**0.5 #should have a factor of cos(theta) I think? Need to define what I mean exactly by this quantity
                                                          #should also make a polar velocity if I'm going to do that
         self.vR = (self.x*self.vx + self.y*self.vy)/self.R
 
         #relative information
```

### Comparing `mwahpy-1.4.7/mwahpy.egg-info/PKG-INFO` & `mwahpy-1.4.8/mwahpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwahpy
-Version: 1.4.7
+Version: 1.4.8
 Summary: A python package for easily parsing and processing data from MilkyWay@home
 Home-page: https://github.com/thomasdonlon/mwahpy
 Author: Tom Donlon
 Author-email: donlot@rpi.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mwahpy-1.4.7/mwahpy.egg-info/SOURCES.txt` & `mwahpy-1.4.8/mwahpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy_tests/nbody_test/1` & `mwahpy-1.4.8/mwahpy_tests/nbody_test/1`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy_tests/nbody_test/2` & `mwahpy-1.4.8/mwahpy_tests/nbody_test/2`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy_tests/nbody_test/3` & `mwahpy-1.4.8/mwahpy_tests/nbody_test/3`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy_tests/test.py` & `mwahpy-1.4.8/mwahpy_tests/test.py`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/mwahpy_tests/test_bodies.out` & `mwahpy-1.4.8/mwahpy_tests/test_bodies.out`

 * *Files identical despite different names*

### Comparing `mwahpy-1.4.7/setup.py` & `mwahpy-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mwahpy",
-    version="1.4.7",
+    version="1.4.8",
     author="Tom Donlon",
     author_email="donlot@rpi.edu",
     description="A python package for easily parsing and processing data from MilkyWay@home",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thomasdonlon/mwahpy",
     packages=setuptools.find_packages(),
```

