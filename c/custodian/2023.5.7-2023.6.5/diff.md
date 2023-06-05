# Comparing `tmp/custodian-2023.5.7.tar.gz` & `tmp/custodian-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodian-2023.5.7.tar", last modified: Sun May  7 20:41:37 2023, max compression
+gzip compressed data, was "custodian-2023.6.5.tar", last modified: Mon Jun  5 15:24:27 2023, max compression
```

## Comparing `custodian-2023.5.7.tar` & `custodian-2023.6.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.788636 custodian-2023.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-07 20:37:45.000000 custodian-2023.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-07 20:37:45.000000 custodian-2023.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-07 20:41:37.788636 custodian-2023.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-07 20:37:45.000000 custodian-2023.5.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.780636 custodian-2023.5.7/custodian/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/ansible/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/ansible/interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/converge_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/converge_kpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/cstdn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/run_nwchem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12410 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/run_vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/cp2k/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    36593 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/feff/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/lobster/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/lobster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/lobster/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/lobster/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/nwchem/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/nwchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/nwchem/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/nwchem/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/qchem/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.788636 custodian-2023.5.7/custodian/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/tests/test_custodian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.788636 custodian-2023.5.7/custodian/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76156 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    38518 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-07 20:37:45.000000 custodian-2023.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 20:37:45.000000 custodian-2023.5.7/requirements-ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-07 20:37:45.000000 custodian-2023.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-07 20:41:37.788636 custodian-2023.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-07 20:37:45.000000 custodian-2023.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-05 15:20:36.000000 custodian-2023.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 15:20:36.000000 custodian-2023.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-05 15:24:27.789778 custodian-2023.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-05 15:20:36.000000 custodian-2023.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/ansible/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/ansible/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/converge_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/converge_kpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/cstdn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/run_nwchem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12410 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/run_vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian/cp2k/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36611 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian/feff/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/feff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/feff/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/feff/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/feff/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/custodian/lobster/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/lobster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/lobster/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/lobster/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/custodian/nwchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/nwchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/nwchem/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/nwchem/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/custodian/qchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/qchem/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/qchem/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/qchem/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/custodian/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/tests/test_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/custodian/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76553 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/vasp/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/vasp/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39455 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/vasp/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/vasp/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-05 15:20:36.000000 custodian-2023.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 15:20:36.000000 custodian-2023.6.5/requirements-ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:20:36.000000 custodian-2023.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 15:24:27.789778 custodian-2023.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-05 15:20:36.000000 custodian-2023.6.5/setup.py
```

### Comparing `custodian-2023.5.7/LICENSE` & `custodian-2023.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/PKG-INFO` & `custodian-2023.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodian
-Version: 2023.5.7
+Version: 2023.6.5
 Summary: A simple JIT job management framework in Python.
 Home-page: https://github.com/materialsproject/custodian
 Author: Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau
 Author-email: ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 License: MIT
 Keywords: jit,just-in-time,job,management,vasp
```

### Comparing `custodian-2023.5.7/README.rst` & `custodian-2023.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/ansible/actions.py` & `custodian-2023.6.5/custodian/ansible/actions.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/ansible/interpreter.py` & `custodian-2023.6.5/custodian/ansible/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/cli/converge_geometry.py` & `custodian-2023.6.5/custodian/cli/converge_geometry.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/cli/converge_kpoints.py` & `custodian-2023.6.5/custodian/cli/converge_kpoints.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/cli/cstdn.py` & `custodian-2023.6.5/custodian/cli/cstdn.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/cli/run_nwchem.py` & `custodian-2023.6.5/custodian/cli/run_nwchem.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/cli/run_vasp.py` & `custodian-2023.6.5/custodian/cli/run_vasp.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/cp2k/handlers.py` & `custodian-2023.6.5/custodian/cp2k/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/cp2k/interpreter.py` & `custodian-2023.6.5/custodian/cp2k/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/cp2k/jobs.py` & `custodian-2023.6.5/custodian/cp2k/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/cp2k/utils.py` & `custodian-2023.6.5/custodian/cp2k/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/cp2k/validators.py` & `custodian-2023.6.5/custodian/cp2k/validators.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/custodian.py` & `custodian-2023.6.5/custodian/custodian.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,15 @@
         monitor_freq=30,
         skip_over_errors=False,
         scratch_dir=None,
         gzipped_output=False,
         checkpoint=False,
         terminate_func=None,
         terminate_on_nonzero_returncode=True,
+        **kwargs,
     ):
         """
         Initializes a Custodian from a list of jobs and error handlers.
 
         Args:
             handlers ([ErrorHandler]): Error handlers. In order of priority of
                 fixing.
```

### Comparing `custodian-2023.5.7/custodian/feff/handlers.py` & `custodian-2023.6.5/custodian/feff/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/feff/interpreter.py` & `custodian-2023.6.5/custodian/feff/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/feff/jobs.py` & `custodian-2023.6.5/custodian/feff/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/lobster/handlers.py` & `custodian-2023.6.5/custodian/lobster/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/lobster/jobs.py` & `custodian-2023.6.5/custodian/lobster/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/nwchem/handlers.py` & `custodian-2023.6.5/custodian/nwchem/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/nwchem/jobs.py` & `custodian-2023.6.5/custodian/nwchem/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/qchem/handlers.py` & `custodian-2023.6.5/custodian/qchem/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/qchem/jobs.py` & `custodian-2023.6.5/custodian/qchem/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/qchem/utils.py` & `custodian-2023.6.5/custodian/qchem/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/tests/test_custodian.py` & `custodian-2023.6.5/custodian/tests/test_custodian.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/utils.py` & `custodian-2023.6.5/custodian/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/vasp/handlers.py` & `custodian-2023.6.5/custodian/vasp/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,23 +98,25 @@
         "posmap": ["POSMAP"],
         "point_group": ["group operation missing"],
         "symprec_noise": ["determination of the symmetry of your systems shows a strong"],
         "dfpt_ncore": ["PEAD routines do not work for NCORE", "remove the tag NPAR from the INCAR file"],
         "bravais": ["Inconsistent Bravais lattice"],
         "nbands_not_sufficient": ["number of bands is not sufficient"],
         "hnform": ["HNFORM: k-point generating"],
-        "coef": ["while reading plane"],
+        "coef": ["while reading plane", "while reading WAVECAR"],
         "set_core_wf": ["internal error in SET_CORE_WF"],
+        "read_error": ["Error reading item", "Error code was IERR= 5"],
     }
 
     def __init__(
         self,
         output_filename="vasp.out",
         errors_subset_to_catch=None,
         vtst_fixes=False,
+        **kwargs,
     ):
         """
         Initializes the handler with the output file to check.
 
         Args:
             output_filename (str): This is the file where the stdout for vasp
                 is being redirected. The error messages that are checked are
@@ -600,14 +602,19 @@
         if "set_core_wf" in self.errors:
             # Unfixable error where the solution is to update the POTCARs
             warnings.warn(
                 "We suggest using a new version of the POTCAR files to resolve the SET_CORE_WF error.", UserWarning
             )
             return {"errors": ["set_core_wf"], "actions": None}
 
+        if "read_error" in self.errors:
+            # Unfixable error --- the user made a mistake in the INCAR
+            warnings.warn("Looks like you made a typo in the INCAR. Please double-check it.", UserWarning)
+            return {"errors": ["read_error"], "actions": None}
+
         if "hnform" in self.errors:
             # The only solution is to change your k-point grid or disable symmetry
             # For internal calculation compatibility's sake, we do the latter
             if vi["INCAR"].get("ISYM", 2) > 0:
                 actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
 
         VaspModder(vi=vi).apply_actions(actions)
```

### Comparing `custodian-2023.5.7/custodian/vasp/interpreter.py` & `custodian-2023.6.5/custodian/vasp/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian/vasp/jobs.py` & `custodian-2023.6.5/custodian/vasp/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 This module implements basic kinds of jobs for VASP runs.
 """
 
 import logging
 import math
 import os
 import shutil
-import signal
 import subprocess
 from shutil import which
 
 import numpy as np
+import psutil
 from monty.serialization import dumpfn, loadfn
 from monty.shutil import decompress_dir
 from pymatgen.core.structure import Structure
 from pymatgen.io.vasp.inputs import Incar, Kpoints, Poscar, VaspInput
 from pymatgen.io.vasp.outputs import Outcar, Vasprun
 
 from custodian.custodian import SENTRY_DSN, Job
@@ -147,15 +147,14 @@
         self.suffix = suffix
         self.settings_override = settings_override
         self.auto_npar = auto_npar
         self.auto_gamma = auto_gamma
         self.gamma_vasp_cmd = gamma_vasp_cmd
         self.copy_magmom = copy_magmom
         self.auto_continue = auto_continue
-        self.sbprcss = None
 
         if SENTRY_DSN:
             # if using Sentry logging, add specific VASP executable to scope
             from sentry_sdk import configure_scope
 
             with configure_scope() as scope:
                 try:
@@ -250,18 +249,15 @@
                     if self.gamma_vasp_cmd is not None and which(self.gamma_vasp_cmd[-1]):
                         cmd = self.gamma_vasp_cmd
                     elif which(cmd[-1] + ".gamma"):
                         cmd[-1] += ".gamma"
         logger.info(f"Running {' '.join(cmd)}")
         with open(self.output_file, "w") as f_std, open(self.stderr_file, "w", buffering=1) as f_err:
             # use line buffering for stderr
-            self.sbprcss = subprocess.Popen(
-                cmd, stdout=f_std, stderr=f_err, start_new_session=True
-            )  # pylint: disable=R1732
-            return self.sbprcss
+            return subprocess.Popen(cmd, stdout=f_std, stderr=f_err, start_new_session=True)  # pylint: disable=R1732
 
     def postprocess(self):
         """
         Postprocessing includes renaming and gzipping where necessary.
         Also copies the magmom to the incar if necessary
         """
         for f in VASP_OUTPUT_FILES + [self.output_file]:
@@ -666,20 +662,42 @@
             f.write(f"# {lattice_direction} energy\n")
             for k in sorted(energies.keys()):
                 f.write(f"{k} {energies[k]}\n")
 
     def terminate(self):
         """
         Kill all vasp processes associated with the current job.
-        """
-        logger.info(f"Custodian terminating all VASP processes within process group {self.sbprcss.pid}")
-        try:
-            os.killpg(os.getpgid(self.sbprcss.pid), signal.SIGTERM)
-        except Exception:
-            pass
+        This is done by looping over all processes and selecting the ones
+        that contain "vasp" as well as access files (CHGCAR in particular)
+        in the custodian working directory.
+        There is also a safety that kills all vasp processes if non of the
+        processes can be killed (This is bad if more than one vasp runs are
+        simultaneously executed on the same node). However, this should never
+        happen.
+        """
+        workdir = os.getcwd()
+        logger.info(f"kill vasp processes in work dir {workdir}")
+        is_killed = False
+        for proc in psutil.process_iter():
+            try:
+                if "vasp" in proc.name().lower():
+                    for file in proc.open_files():
+                        if workdir + "/CHGCAR" == file.path and psutil.pid_exists(proc.pid):
+                            proc.kill()
+                            is_killed = True
+            except (psutil.NoSuchProcess, psutil.AccessDenied):
+                continue
+        if not is_killed:
+            logger.warning(f"killing vasp processes in work dir {workdir} failed. Resorting to 'killall'.")
+            cmds = self.vasp_cmd
+            if self.gamma_vasp_cmd:
+                cmds += self.gamma_vasp_cmd
+                for k in cmds:
+                    if "vasp" in k:
+                        subprocess.run(["killall", f"{k}"])
 
 
 class VaspNEBJob(VaspJob):
     """
     A NEB vasp job, especially for CI-NEB running at PBS clusters.
     The class is added for the purpose of handling a different folder
     arrangement in NEB calculation.
@@ -762,15 +780,14 @@
         self.half_kpts = half_kpts
         self.auto_gamma = auto_gamma
         self.gamma_vasp_cmd = gamma_vasp_cmd
         self.auto_continue = auto_continue
         self.settings_override = settings_override
         self.neb_dirs = []  # 00, 01, etc.
         self.neb_sub = []  # 01, 02, etc.
-        self.sbprcss = None
 
         for path in os.listdir("."):
             if os.path.isdir(path) and path.isdigit():
                 self.neb_dirs.append(path)
         self.neb_dirs = sorted(self.neb_dirs)
         self.neb_sub = self.neb_dirs[1:-1]
 
@@ -850,18 +867,15 @@
                 if self.gamma_vasp_cmd is not None and which(self.gamma_vasp_cmd[-1]):
                     cmd = self.gamma_vasp_cmd
                 elif which(cmd[-1] + ".gamma"):
                     cmd[-1] += ".gamma"
         logger.info(f"Running {' '.join(cmd)}")
         with open(self.output_file, "w") as f_std, open(self.stderr_file, "w", buffering=1) as f_err:
             # Use line buffering for stderr
-            self.sbprcss = subprocess.Popen(
-                cmd, stdout=f_std, stderr=f_err, start_new_session=True
-            )  # pylint: disable=R1732
-            return self.sbprcss
+            return subprocess.Popen(cmd, stdout=f_std, stderr=f_err, start_new_session=True)  # pylint: disable=R1732
 
     def postprocess(self):
         """
         Postprocessing includes renaming and gzipping where necessary.
         """
         # Add suffix to all sub_dir/{items}
         for path in self.neb_dirs:
```

### Comparing `custodian-2023.5.7/custodian/vasp/validators.py` & `custodian-2023.6.5/custodian/vasp/validators.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/custodian.egg-info/PKG-INFO` & `custodian-2023.6.5/custodian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodian
-Version: 2023.5.7
+Version: 2023.6.5
 Summary: A simple JIT job management framework in Python.
 Home-page: https://github.com/materialsproject/custodian
 Author: Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau
 Author-email: ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 License: MIT
 Keywords: jit,just-in-time,job,management,vasp
```

### Comparing `custodian-2023.5.7/custodian.egg-info/SOURCES.txt` & `custodian-2023.6.5/custodian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/setup.cfg` & `custodian-2023.6.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.7/setup.py` & `custodian-2023.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_desc = f.read()
     ind = long_desc.find("\n")
     long_desc = long_desc[ind + 1 :]
 
 setup(
     name="custodian",
     packages=find_packages(),
-    version="2023.5.7",
+    version="2023.6.5",
     install_requires=["monty>=2.0.6", "ruamel.yaml>=0.15.6", "sentry-sdk>=0.8.0"],
     extras_require={"vasp, nwchem, qchem": ["pymatgen>=2019.8.23"]},
     package_data={},
     author="Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau",
     author_email="ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     url="https://github.com/materialsproject/custodian",
```

