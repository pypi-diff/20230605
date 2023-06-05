# Comparing `tmp/gemseo-petsc-2.0.0.tar.gz` & `tmp/gemseo-petsc-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemseo-petsc-2.0.0.tar", last modified: Thu Jul 28 09:35:20 2022, max compression
+gzip compressed data, was "gemseo-petsc-3.0.0.tar", last modified: Mon Jun  5 09:50:12 2023, max compression
```

## Comparing `gemseo-petsc-2.0.0.tar` & `gemseo-petsc-3.0.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.561760 gemseo-petsc-2.0.0/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      476 2021-10-11 07:26:02.000000 gemseo-petsc-2.0.0/.gitattributes
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      191 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/.gitignore
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.551760 gemseo-petsc-2.0.0/.gitlab/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.553760 gemseo-petsc-2.0.0/.gitlab/issue_templates/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1126 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/.gitlab/issue_templates/Bug.md
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1029 2021-10-07 07:54:27.000000 gemseo-petsc-2.0.0/.gitlab/issue_templates/Documentation.md
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1033 2021-10-07 07:54:27.000000 gemseo-petsc-2.0.0/.gitlab/issue_templates/Feature Proposal.md
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      771 2021-10-07 07:54:27.000000 gemseo-petsc-2.0.0/.gitlab/issue_templates/Refactoring.md
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2788 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/.gitlab-ci.yml
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2491 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     9105 2021-10-08 08:56:20.000000 gemseo-petsc-2.0.0/.pylintrc
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1048 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/CHANGELOG.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1781 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/CREDITS.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     7652 2021-10-11 07:26:02.000000 gemseo-petsc-2.0.0/LICENSE.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.551760 gemseo-petsc-2.0.0/LICENSES/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.554760 gemseo-petsc-2.0.0/LICENSES/headers/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      729 2021-10-11 07:26:02.000000 gemseo-petsc-2.0.0/LICENSES/headers/BSD-0-Clause.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      334 2021-10-11 07:26:02.000000 gemseo-petsc-2.0.0/LICENSES/headers/CC-BY-SA-4.0.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      710 2021-10-11 07:26:02.000000 gemseo-petsc-2.0.0/LICENSES/headers/LGPL-3.0.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       55 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/MANIFEST.in
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3614 2022-07-28 09:35:20.561760 gemseo-petsc-2.0.0/PKG-INFO
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2532 2021-10-11 07:26:02.000000 gemseo-petsc-2.0.0/README.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      611 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/pyproject.toml
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.555760 gemseo-petsc-2.0.0/requirements/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       79 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/requirements/check.in
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      629 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/requirements/check.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       99 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/requirements/conda.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       12 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/requirements/dist.in
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1373 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/requirements/dist.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1538 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/requirements/doc.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2161 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/requirements/test-python3.10.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2417 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/requirements/test-python3.7.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2159 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/requirements/test-python3.8.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2159 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/requirements/test-python3.9.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1674 2022-07-28 09:35:20.562760 gemseo-petsc-2.0.0/setup.cfg
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      839 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/setup.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.551760 gemseo-petsc-2.0.0/src/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.555760 gemseo-petsc-2.0.0/src/gemseo_petsc/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      826 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/src/gemseo_petsc/__init__.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.556760 gemseo-petsc-2.0.0/src/gemseo_petsc/linear_solvers/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      823 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/src/gemseo_petsc/linear_solvers/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     9465 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/src/gemseo_petsc/linear_solvers/ksp_lib.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.556760 gemseo-petsc-2.0.0/src/gemseo_petsc/linear_solvers/options/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1965 2021-10-08 08:56:20.000000 gemseo-petsc-2.0.0/src/gemseo_petsc/linear_solvers/options/PETSC_KSP_options.json
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.556760 gemseo-petsc-2.0.0/src/gemseo_petsc.egg-info/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3614 2022-07-28 09:35:20.000000 gemseo-petsc-2.0.0/src/gemseo_petsc.egg-info/PKG-INFO
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1268 2022-07-28 09:35:20.000000 gemseo-petsc-2.0.0/src/gemseo_petsc.egg-info/SOURCES.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        1 2022-07-28 09:35:20.000000 gemseo-petsc-2.0.0/src/gemseo_petsc.egg-info/dependency_links.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       45 2022-07-28 09:35:20.000000 gemseo-petsc-2.0.0/src/gemseo_petsc.egg-info/entry_points.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       77 2022-07-28 09:35:20.000000 gemseo-petsc-2.0.0/src/gemseo_petsc.egg-info/requires.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       13 2022-07-28 09:35:20.000000 gemseo-petsc-2.0.0/src/gemseo_petsc.egg-info/top_level.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.556760 gemseo-petsc-2.0.0/tests/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      838 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/tests/__init__.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.556760 gemseo-petsc-2.0.0/tests/linear_solvers/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      836 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/tests/linear_solvers/__init__.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:35:20.560760 gemseo-petsc-2.0.0/tests/linear_solvers/data/
--rwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)  1712591 2021-10-08 13:21:31.000000 gemseo-petsc-2.0.0/tests/linear_solvers/data/a_mat.npz
--rwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   502906 2021-10-08 13:21:31.000000 gemseo-petsc-2.0.0/tests/linear_solvers/data/b_vec.pkl
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     8289 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/tests/linear_solvers/test_ksp.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3721 2022-07-28 09:34:19.000000 gemseo-petsc-2.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.658784 gemseo-petsc-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.648701 gemseo-petsc-3.0.0/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.653284 gemseo-petsc-3.0.0/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/.gitlab/issue_templates/Bug.md
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/.gitlab/issue_templates/Documentation.md
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/.gitlab/issue_templates/Feature Proposal.md
+-rw-rw-rw-   0 root         (0) root         (0)      771 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/.gitlab/issue_templates/Refactoring.md
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     9105 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/CREDITS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.649618 gemseo-petsc-3.0.0/LICENSES/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.653284 gemseo-petsc-3.0.0/LICENSES/headers/
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/LICENSES/headers/BSD-0-Clause.txt
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/LICENSES/headers/CC-BY-SA-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/LICENSES/headers/LGPL-3.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4103 2023-06-05 09:50:12.658784 gemseo-petsc-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3071 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.655118 gemseo-petsc-3.0.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/requirements/check.in
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/requirements/check.txt
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/requirements/conda.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/requirements/dist.in
+-rw-rw-rw-   0 root         (0) root         (0)     1493 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/requirements/dist.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/requirements/doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/requirements/test-python3.10.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/requirements/test-python3.8.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/requirements/test-python3.9.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-06-05 09:50:12.660618 gemseo-petsc-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.649618 gemseo-petsc-3.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.655118 gemseo-petsc-3.0.0/src/gemseo_petsc/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/src/gemseo_petsc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.656034 gemseo-petsc-3.0.0/src/gemseo_petsc/linear_solvers/
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/src/gemseo_petsc/linear_solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9481 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/src/gemseo_petsc/linear_solvers/ksp_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.656034 gemseo-petsc-3.0.0/src/gemseo_petsc/linear_solvers/options/
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/src/gemseo_petsc/linear_solvers/options/PETSC_KSP_options.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.656034 gemseo-petsc-3.0.0/src/gemseo_petsc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4103 2023-06-05 09:50:12.000000 gemseo-petsc-3.0.0/src/gemseo_petsc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-06-05 09:50:12.000000 gemseo-petsc-3.0.0/src/gemseo_petsc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 09:50:12.000000 gemseo-petsc-3.0.0/src/gemseo_petsc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-05 09:50:12.000000 gemseo-petsc-3.0.0/src/gemseo_petsc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-05 09:50:12.000000 gemseo-petsc-3.0.0/src/gemseo_petsc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 09:50:12.000000 gemseo-petsc-3.0.0/src/gemseo_petsc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.656034 gemseo-petsc-3.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      838 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.656951 gemseo-petsc-3.0.0/tests/linear_solvers/
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/tests/linear_solvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.657868 gemseo-petsc-3.0.0/tests/linear_solvers/data/
+-rwxrwxrwx   0 root         (0) root         (0)  1712591 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/tests/linear_solvers/data/a_mat.npz
+-rwxrwxrwx   0 root         (0) root         (0)   502906 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/tests/linear_solvers/data/b_vec.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     8234 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/tests/linear_solvers/test_ksp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:50:12.658784 gemseo-petsc-3.0.0/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/tools/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     3906 2023-06-05 09:49:31.000000 gemseo-petsc-3.0.0/tox.ini
```

### Comparing `gemseo-petsc-2.0.0/.gitlab/issue_templates/Bug.md` & `gemseo-petsc-3.0.0/.gitlab/issue_templates/Bug.md`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/.gitlab/issue_templates/Documentation.md` & `gemseo-petsc-3.0.0/.gitlab/issue_templates/Documentation.md`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/.gitlab/issue_templates/Feature Proposal.md` & `gemseo-petsc-3.0.0/.gitlab/issue_templates/Feature Proposal.md`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/.gitlab/issue_templates/Refactoring.md` & `gemseo-petsc-3.0.0/.gitlab/issue_templates/Refactoring.md`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/.pylintrc` & `gemseo-petsc-3.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/CHANGELOG.rst` & `gemseo-petsc-3.0.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,25 @@
 
 The format is based on
 `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_
 and this project adheres to
 `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
 
+Version 3.0.0 (June 2023)
+*************************
+
+Update to GEMSEO 5.0.0.
+
+Changed
+-------
+
+Renamed ``ksp_lib.py`` to ``ksp_library.py``.
+
+
 Version 2.0.0 (November 2021)
 *****************************
 
 Update to GEMSEO 4.0.0.
 
 
 Version 1.0.0 (November 2021)
```

### Comparing `gemseo-petsc-2.0.0/CREDITS.rst` & `gemseo-petsc-3.0.0/CREDITS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -68,7 +68,12 @@
     MIT
 
 `setuptools <https://setuptools.readthedocs.io/>`_
     MIT
 
 `setuptools_scm <https://github.com/pypa/setuptools_scm/>`_
     MIT
+
+Resources
+---------
+
+Some icons and fonts are used by GEMSEO-pdfo or its documentation.
```

### Comparing `gemseo-petsc-2.0.0/LICENSE.txt` & `gemseo-petsc-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/LICENSES/headers/BSD-0-Clause.txt` & `gemseo-petsc-3.0.0/LICENSES/headers/BSD-0-Clause.txt`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/LICENSES/headers/LGPL-3.0.txt` & `gemseo-petsc-3.0.0/LICENSES/headers/LGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/PKG-INFO` & `gemseo-petsc-3.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-petsc
-Version: 2.0.0
+Version: 3.0.0
 Summary: PETSc GEMSEO interface
 Home-page: https://gitlab.com/gemseo
 Author: François Gallard
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-petsc
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-petsc/-/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
@@ -86,20 +85,34 @@
 it is possible to build **PETSc** and **petsc4py** under a Windows environment,
 and hence to have the **gemseo-petsc** plugin working.
 A description of the procedure to build these dependencies can be found `here <https://openmdao.readthedocs.io/en/1.7.3/getting-started/mpi_windows.html>`_
 
 Bugs/Questions
 --------------
 
-Bugs can be reported in the PETSc GEMSEO interface issue `tracker <http://forge-mdo.irt-aese.local/dev/gems/gemseo_petsc/-/issues>`_.
+Please use the gitlab issue tracker at
+https://gitlab.com/gemseo/dev/gemseo-petsc/-/issues
+to submit bugs or questions.
 
 License
 -------
 
-The gemseo-petsc plugin is licensed under the `GNU Lesser General Public License v3 <https://www.gnu.org/licenses/lgpl-3.0.en.html.>`_
+The GEMSEO-PETSc source code is distributed under the GNU LGPL v3.0 license.
+A copy of it can be found in the LICENSE.txt file.
+The GNU LGPL v3.0 license is an exception to the GNU GPL v3.0 license.
+A copy of the GNU GPL v3.0 license can be found in the LICENSES folder.
+
+The GEMSEO-PETSc examples are distributed under the BSD 0-Clause, a permissive
+license that allows to copy paste the code of examples without preserving the
+copyright mentions.
+
+The GEMSEO-PETSc documentation is distributed under the CC BY-SA 4.0 license.
+
+The GEMSEO-PETSc product depends on other software which have various licenses.
+The list of dependencies with their licenses is given in the CREDITS.rst file.
 
 Contributors
 ------------
 
 - François Gallard
 - Jean-Christophe Giret
 - Antoine Dechaume
```

### Comparing `gemseo-petsc-2.0.0/README.rst` & `gemseo-petsc-3.0.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -59,20 +59,34 @@
 it is possible to build **PETSc** and **petsc4py** under a Windows environment,
 and hence to have the **gemseo-petsc** plugin working.
 A description of the procedure to build these dependencies can be found `here <https://openmdao.readthedocs.io/en/1.7.3/getting-started/mpi_windows.html>`_
 
 Bugs/Questions
 --------------
 
-Bugs can be reported in the PETSc GEMSEO interface issue `tracker <http://forge-mdo.irt-aese.local/dev/gems/gemseo_petsc/-/issues>`_.
+Please use the gitlab issue tracker at
+https://gitlab.com/gemseo/dev/gemseo-petsc/-/issues
+to submit bugs or questions.
 
 License
 -------
 
-The gemseo-petsc plugin is licensed under the `GNU Lesser General Public License v3 <https://www.gnu.org/licenses/lgpl-3.0.en.html.>`_
+The GEMSEO-PETSc source code is distributed under the GNU LGPL v3.0 license.
+A copy of it can be found in the LICENSE.txt file.
+The GNU LGPL v3.0 license is an exception to the GNU GPL v3.0 license.
+A copy of the GNU GPL v3.0 license can be found in the LICENSES folder.
+
+The GEMSEO-PETSc examples are distributed under the BSD 0-Clause, a permissive
+license that allows to copy paste the code of examples without preserving the
+copyright mentions.
+
+The GEMSEO-PETSc documentation is distributed under the CC BY-SA 4.0 license.
+
+The GEMSEO-PETSc product depends on other software which have various licenses.
+The list of dependencies with their licenses is given in the CREDITS.rst file.
 
 Contributors
 ------------
 
 - François Gallard
 - Jean-Christophe Giret
 - Antoine Dechaume
```

### Comparing `gemseo-petsc-2.0.0/pyproject.toml` & `gemseo-petsc-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # logging settings identical to the defaults of gemseo.api.configure_logger()
 log_file_level = "INFO"
 log_file_date_format = "%H:%M:%S"
 log_file_format = "%(levelname)8s - %(asctime)s: %(message)s"
 # filterwarnings = ignore::pytest.PytestExperimentalApiWarning
 
 [tool.black]
-target-version = ['py37']
+target-version = ['py38']
```

### Comparing `gemseo-petsc-2.0.0/requirements/check.txt` & `gemseo-petsc-3.0.0/requirements/check.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
 #    pip-compile requirements/check.in
 #
 cfgv==3.3.1
     # via pre-commit
-distlib==0.3.5
+distlib==0.3.6
     # via virtualenv
-filelock==3.7.1
+filelock==3.12.0
     # via virtualenv
-identify==2.5.2
+identify==2.5.24
     # via pre-commit
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
-platformdirs==2.5.2
+platformdirs==3.5.1
     # via virtualenv
-pre-commit==2.20.0
+pre-commit==3.3.2
     # via -r requirements/check.in
 pyyaml==6.0
     # via pre-commit
-six==1.16.0
-    # via virtualenv
-toml==0.10.2
-    # via pre-commit
-virtualenv==20.15.1
+virtualenv==20.23.0
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `gemseo-petsc-2.0.0/requirements/dist.txt` & `gemseo-petsc-3.0.0/requirements/dist.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
 #    pip-compile requirements/dist.in
 #
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-build==0.8.0
+build==0.10.0
     # via -r requirements/dist.in
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
-charset-normalizer==2.1.0
+charset-normalizer==3.1.0
     # via requests
-commonmark==0.9.1
-    # via rich
-cryptography==37.0.4
+cryptography==40.0.2
     # via secretstorage
-docutils==0.19
+docutils==0.20.1
     # via readme-renderer
-idna==3.3
+idna==3.4
     # via requests
-importlib-metadata==4.12.0
+importlib-metadata==6.6.0
     # via
     #   keyring
     #   twine
+jaraco-classes==3.2.3
+    # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-keyring==23.7.0
+keyring==23.13.1
     # via twine
-packaging==21.3
-    # via build
-pep517==0.12.0
+markdown-it-py==2.2.0
+    # via rich
+mdurl==0.1.2
+    # via markdown-it-py
+more-itertools==9.1.0
+    # via jaraco-classes
+packaging==23.1
     # via build
-pkginfo==1.8.3
+pkginfo==1.9.6
     # via twine
 pycparser==2.21
     # via cffi
-pygments==2.12.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
-pyparsing==3.0.9
-    # via packaging
-readme-renderer==35.0
+pyproject-hooks==1.0.0
+    # via build
+readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.9.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.5.1
+rich==13.3.5
     # via twine
-secretstorage==3.3.2
+secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 tomli==2.0.1
     # via
     #   build
-    #   pep517
-twine==4.0.1
+    #   pyproject-hooks
+twine==4.0.2
     # via -r requirements/dist.in
-urllib3==1.26.10
+urllib3==2.0.2
     # via
     #   requests
     #   twine
 webencodings==0.5.1
     # via bleach
-zipp==3.8.1
+zipp==3.15.0
     # via importlib-metadata
```

### Comparing `gemseo-petsc-2.0.0/requirements/doc.txt` & `gemseo-petsc-3.0.0/requirements/doc.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via matplotlib
 docstring-inheritance==1.0.0
     # via gemseo
 fastjsonschema==2.16.1
     # via gemseo
 fonttools==4.34.4
     # via matplotlib
-gemseo==4.0.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-petsc (setup.py)
 genson==1.2.2
     # via gemseo
 h5py==3.6.0
     # via gemseo
 idna==3.3
     # via requests
```

### Comparing `gemseo-petsc-2.0.0/requirements/test-python3.10.txt` & `gemseo-petsc-3.0.0/requirements/test-python3.10.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,119 +1,119 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
 #
-attrs==21.4.0
-    # via pytest
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.0
+charset-normalizer==3.1.0
     # via requests
-covdefaults==2.2.0
+contourpy==1.0.7
+    # via matplotlib
+covdefaults==2.3.0
     # via gemseo-petsc (setup.py)
-coverage[toml]==6.4.2
+coverage[toml]==7.2.6
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 docstring-inheritance==1.0.0
     # via gemseo
+exceptiongroup==1.1.1
+    # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.1
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.34.4
+fonttools==4.39.4
     # via matplotlib
-gemseo==4.0.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-petsc (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.6.0
+h5py==3.8.0
     # via gemseo
-idna==3.3
+idna==3.4
     # via requests
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-matplotlib==3.5.2
+matplotlib==3.7.1
     # via gemseo
-    # via petsc
-networkx==2.8.5
+networkx==3.1
     # via gemseo
-numpy==1.22.4
+numpy==1.24.3
     # via
+    #   contourpy
     #   gemseo
+    #   gemseo-petsc (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
     #   petsc4py
     #   pyxdsm
     #   scipy
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.4.3
+pandas==2.0.0
     # via gemseo
     # via petsc4py
     # via gemseo-petsc (setup.py)
-pillow==9.2.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
-py==1.11.0
-    # via
-    #   pytest
-    #   pytest-forked
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.1.2
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-petsc (setup.py)
     #   pytest-cov
-    #   pytest-forked
     #   pytest-xdist
-pytest-cov==3.0.0
+pytest-cov==4.1.0
     # via gemseo-petsc (setup.py)
-pytest-forked==1.4.0
-    # via pytest-xdist
-pytest-xdist==2.5.0
+pytest-xdist==3.3.1
     # via gemseo-petsc (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.1
+pytz==2023.3
     # via pandas
-pyxdsm==2.2.1
+pyxdsm==2.2.2
     # via gemseo
-requests==2.28.1
-    # via gemseo
-scipy==1.7.3
+requests==2.31.0
     # via gemseo
+scipy==1.10.1
+    # via
+    #   gemseo
+    #   gemseo-petsc (setup.py)
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.0
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.3.0
+typing-extensions==4.6.2
     # via gemseo
-urllib3==1.26.11
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.0.0
+xxhash==3.2.0
     # via gemseo
```

### Comparing `gemseo-petsc-2.0.0/requirements/test-python3.7.txt` & `gemseo-petsc-3.0.0/requirements/test-python3.9.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,123 @@
 #
-# This file is autogenerated by pip-compile with python 3.7
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.7.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.9.txt
 #
-attrs==21.4.0
-    # via pytest
-cached-property==1.5.2
-    # via h5py
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.0
+charset-normalizer==3.1.0
     # via requests
-covdefaults==2.2.0
+contourpy==1.0.7
+    # via matplotlib
+covdefaults==2.3.0
     # via gemseo-petsc (setup.py)
-coverage[toml]==6.4.2
+coverage[toml]==7.2.6
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 docstring-inheritance==1.0.0
     # via gemseo
+exceptiongroup==1.1.1
+    # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.1
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.34.4
+fonttools==4.39.4
     # via matplotlib
-gemseo==4.0.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-petsc (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.6.0
+h5py==3.8.0
     # via gemseo
-idna==3.3
+idna==3.4
     # via requests
-importlib-metadata==4.12.0
-    # via
-    #   gemseo
-    #   pluggy
-    #   pytest
-iniconfig==1.1.1
+importlib-resources==5.12.0
+    # via matplotlib
+iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-matplotlib==3.5.2
+matplotlib==3.7.1
     # via gemseo
-    # via petsc
-networkx==2.6.3
+networkx==3.1
     # via gemseo
-numpy==1.21.6
+numpy==1.24.3
     # via
+    #   contourpy
     #   gemseo
+    #   gemseo-petsc (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
     #   petsc4py
     #   pyxdsm
     #   scipy
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.3.5
+pandas==2.0.0
     # via gemseo
     # via petsc4py
     # via gemseo-petsc (setup.py)
-pillow==9.2.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
-py==1.11.0
-    # via
-    #   pytest
-    #   pytest-forked
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.1.2
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-petsc (setup.py)
     #   pytest-cov
-    #   pytest-forked
     #   pytest-xdist
-pytest-cov==3.0.0
+pytest-cov==4.1.0
     # via gemseo-petsc (setup.py)
-pytest-forked==1.4.0
-    # via pytest-xdist
-pytest-xdist==2.5.0
+pytest-xdist==3.3.1
     # via gemseo-petsc (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.1
+pytz==2023.3
     # via pandas
-pyxdsm==2.2.1
-    # via gemseo
-requests==2.28.1
+pyxdsm==2.2.2
     # via gemseo
-scipy==1.7.3
-    # via gemseo
-singledispatchmethod==1.0
+requests==2.31.0
     # via gemseo
+scipy==1.10.1
+    # via
+    #   gemseo
+    #   gemseo-petsc (setup.py)
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.0
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.3.0
-    # via
-    #   gemseo
-    #   importlib-metadata
-    #   kiwisolver
-urllib3==1.26.11
+typing-extensions==4.6.2
+    # via gemseo
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.0.0
+xxhash==3.2.0
     # via gemseo
-zipp==3.8.1
-    # via importlib-metadata
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-petsc-2.0.0/requirements/test-python3.8.txt` & `gemseo-petsc-3.0.0/requirements/test-python3.8.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,119 +1,123 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/test-python3.8.txt
 #
-attrs==21.4.0
-    # via pytest
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.0
+charset-normalizer==3.1.0
     # via requests
-covdefaults==2.2.0
+contourpy==1.0.7
+    # via matplotlib
+covdefaults==2.3.0
     # via gemseo-petsc (setup.py)
-coverage[toml]==6.4.2
+coverage[toml]==7.2.6
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 docstring-inheritance==1.0.0
     # via gemseo
+exceptiongroup==1.1.1
+    # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.1
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.34.4
+fonttools==4.39.4
     # via matplotlib
-gemseo==4.0.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-petsc (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.6.0
+h5py==3.8.0
     # via gemseo
-idna==3.3
+idna==3.4
     # via requests
-iniconfig==1.1.1
+importlib-resources==5.12.0
+    # via matplotlib
+iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-matplotlib==3.5.2
+matplotlib==3.7.1
     # via gemseo
-    # via petsc
-networkx==2.8.5
+networkx==3.1
     # via gemseo
-numpy==1.22.4
+numpy==1.24.3
     # via
+    #   contourpy
     #   gemseo
+    #   gemseo-petsc (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
     #   petsc4py
     #   pyxdsm
     #   scipy
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.4.3
+pandas==2.0.0
     # via gemseo
     # via petsc4py
     # via gemseo-petsc (setup.py)
-pillow==9.2.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
-py==1.11.0
-    # via
-    #   pytest
-    #   pytest-forked
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.1.2
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-petsc (setup.py)
     #   pytest-cov
-    #   pytest-forked
     #   pytest-xdist
-pytest-cov==3.0.0
+pytest-cov==4.1.0
     # via gemseo-petsc (setup.py)
-pytest-forked==1.4.0
-    # via pytest-xdist
-pytest-xdist==2.5.0
+pytest-xdist==3.3.1
     # via gemseo-petsc (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.1
+pytz==2023.3
     # via pandas
-pyxdsm==2.2.1
+pyxdsm==2.2.2
     # via gemseo
-requests==2.28.1
-    # via gemseo
-scipy==1.7.3
+requests==2.31.0
     # via gemseo
+scipy==1.10.1
+    # via
+    #   gemseo
+    #   gemseo-petsc (setup.py)
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.0
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.3.0
+typing-extensions==4.6.2
     # via gemseo
-urllib3==1.26.11
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.0.0
+xxhash==3.2.0
     # via gemseo
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-petsc-2.0.0/setup.cfg` & `gemseo-petsc-3.0.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -17,66 +17,67 @@
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = true
-python_requires = >=3.7, <3.11
+python_requires = >=3.8, <3.11
 install_requires = 
-	gemseo >=4.0.0
+	gemseo >=5
+	numpy
 	petsc4py >=3
+	scipy
 
 [options.packages.find]
 where = src
 
-[options.package_data]
-gemseo_petsc = 
-	linear_solvers/options/*.json
-
 [options.extras_require]
 test = 
 	covdefaults
 	pytest
 	pytest-cov
 	pytest-xdist
 
+[bdist_wheel]
+universal = true
+
 [options.entry_points]
 gemseo_plugins = 
 	gemseo-petsc = gemseo_petsc
 
-[bdist_wheel]
-universal = true
-
 [coverage:run]
 plugins = covdefaults
 source = gemseo_petsc
 
 [coverage:report]
 fail_under = 1
 
 [flake8]
 ignore = 
 	E501
 	D105
 	E203
 	W503
-select = B,C,D,E,F,G,N,T,W,B950
+	ANN101
+	ANN102
+	ANN401
+select = ANN,B,C,D,E,F,G,N,T,W,B950
 max-line-length = 88
 docstring-convention = google
 per-file-ignores = 
-	tests/*.py:D
+	tests/*.py: D100,D104,ANN
+	doc_src/*.py: D,T201
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gemseo-petsc-2.0.0/setup.py` & `gemseo-petsc-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/src/gemseo_petsc/__init__.py` & `gemseo-petsc-3.0.0/src/gemseo_petsc/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/src/gemseo_petsc/linear_solvers/__init__.py` & `gemseo-petsc-3.0.0/src/gemseo_petsc/linear_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/src/gemseo_petsc/linear_solvers/ksp_lib.py` & `gemseo-petsc-3.0.0/src/gemseo_petsc/linear_solvers/ksp_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from __future__ import annotations
 
 import logging
 import sys
 from typing import Any
 
 import petsc4py
-from gemseo.algos.linear_solvers.linear_solver_lib import LinearSolverDescription
-from gemseo.algos.linear_solvers.linear_solver_lib import LinearSolverLib
+from gemseo.algos.linear_solvers.linear_solver_library import LinearSolverDescription
+from gemseo.algos.linear_solvers.linear_solver_library import LinearSolverLibrary
 from numpy import arange
 from numpy import array
 from numpy import ndarray
 from scipy.sparse import csr_matrix
 from scipy.sparse import find
 from scipy.sparse.base import issparse
 
@@ -37,15 +37,15 @@
 # command args in the options database.
 petsc4py.init(sys.argv)
 from petsc4py import PETSc  # noqa: E402
 
 LOGGER = logging.getLogger(__name__)
 
 
-class PetscKSPAlgos(LinearSolverLib):
+class PetscKSPAlgos(LinearSolverLibrary):
     """Interface to PETSC KSP.
 
     For further information, please read
     https://petsc4py.readthedocs.io/en/stable/manual/ksp/
 
     https://petsc.org/release/docs/manualpages/KSP/KSP.html#KSP
     """
```

### Comparing `gemseo-petsc-2.0.0/src/gemseo_petsc/linear_solvers/options/PETSC_KSP_options.json` & `gemseo-petsc-3.0.0/src/gemseo_petsc/linear_solvers/options/PETSC_KSP_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/src/gemseo_petsc.egg-info/PKG-INFO` & `gemseo-petsc-3.0.0/src/gemseo_petsc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-petsc
-Version: 2.0.0
+Version: 3.0.0
 Summary: PETSc GEMSEO interface
 Home-page: https://gitlab.com/gemseo
 Author: François Gallard
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-petsc
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-petsc/-/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
@@ -86,20 +85,34 @@
 it is possible to build **PETSc** and **petsc4py** under a Windows environment,
 and hence to have the **gemseo-petsc** plugin working.
 A description of the procedure to build these dependencies can be found `here <https://openmdao.readthedocs.io/en/1.7.3/getting-started/mpi_windows.html>`_
 
 Bugs/Questions
 --------------
 
-Bugs can be reported in the PETSc GEMSEO interface issue `tracker <http://forge-mdo.irt-aese.local/dev/gems/gemseo_petsc/-/issues>`_.
+Please use the gitlab issue tracker at
+https://gitlab.com/gemseo/dev/gemseo-petsc/-/issues
+to submit bugs or questions.
 
 License
 -------
 
-The gemseo-petsc plugin is licensed under the `GNU Lesser General Public License v3 <https://www.gnu.org/licenses/lgpl-3.0.en.html.>`_
+The GEMSEO-PETSc source code is distributed under the GNU LGPL v3.0 license.
+A copy of it can be found in the LICENSE.txt file.
+The GNU LGPL v3.0 license is an exception to the GNU GPL v3.0 license.
+A copy of the GNU GPL v3.0 license can be found in the LICENSES folder.
+
+The GEMSEO-PETSc examples are distributed under the BSD 0-Clause, a permissive
+license that allows to copy paste the code of examples without preserving the
+copyright mentions.
+
+The GEMSEO-PETSc documentation is distributed under the CC BY-SA 4.0 license.
+
+The GEMSEO-PETSc product depends on other software which have various licenses.
+The list of dependencies with their licenses is given in the CREDITS.rst file.
 
 Contributors
 ------------
 
 - François Gallard
 - Jean-Christophe Giret
 - Antoine Dechaume
```

### Comparing `gemseo-petsc-2.0.0/src/gemseo_petsc.egg-info/SOURCES.txt` & `gemseo-petsc-3.0.0/src/gemseo_petsc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 requirements/check.in
 requirements/check.txt
 requirements/conda.txt
 requirements/dist.in
 requirements/dist.txt
 requirements/doc.txt
 requirements/test-python3.10.txt
-requirements/test-python3.7.txt
 requirements/test-python3.8.txt
 requirements/test-python3.9.txt
 src/gemseo_petsc/__init__.py
 src/gemseo_petsc.egg-info/PKG-INFO
 src/gemseo_petsc.egg-info/SOURCES.txt
 src/gemseo_petsc.egg-info/dependency_links.txt
 src/gemseo_petsc.egg-info/entry_points.txt
 src/gemseo_petsc.egg-info/requires.txt
 src/gemseo_petsc.egg-info/top_level.txt
 src/gemseo_petsc/linear_solvers/__init__.py
-src/gemseo_petsc/linear_solvers/ksp_lib.py
+src/gemseo_petsc/linear_solvers/ksp_library.py
 src/gemseo_petsc/linear_solvers/options/PETSC_KSP_options.json
 tests/__init__.py
 tests/linear_solvers/__init__.py
 tests/linear_solvers/test_ksp.py
 tests/linear_solvers/data/a_mat.npz
-tests/linear_solvers/data/b_vec.pkl
+tests/linear_solvers/data/b_vec.pkl
+tools/Dockerfile
```

### Comparing `gemseo-petsc-2.0.0/tests/__init__.py` & `gemseo-petsc-3.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/tests/linear_solvers/__init__.py` & `gemseo-petsc-3.0.0/tests/linear_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/tests/linear_solvers/data/a_mat.npz` & `gemseo-petsc-3.0.0/tests/linear_solvers/data/a_mat.npz`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/tests/linear_solvers/data/b_vec.pkl` & `gemseo-petsc-3.0.0/tests/linear_solvers/data/b_vec.pkl`

 * *Files identical despite different names*

### Comparing `gemseo-petsc-2.0.0/tests/linear_solvers/test_ksp.py` & `gemseo-petsc-3.0.0/tests/linear_solvers/test_ksp.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,33 +20,32 @@
 from __future__ import annotations
 
 import pickle
 from itertools import product
 from os.path import dirname
 from os.path import join
 from typing import Any
-from typing import List
 from typing import Mapping
 
 import pytest
+from gemseo import create_discipline
+from gemseo import create_mda
 from gemseo.algos.linear_solvers.linear_problem import LinearProblem
 from gemseo.algos.linear_solvers.linear_solvers_factory import LinearSolversFactory
-from gemseo.api import create_discipline
-from gemseo.api import create_mda
 from gemseo.core.discipline import MDODiscipline
-from gemseo_petsc.linear_solvers.ksp_lib import _convert_ndarray_to_mat_or_vec
+from gemseo_petsc.linear_solvers.ksp_library import _convert_ndarray_to_mat_or_vec
 from numpy import eye
 from numpy import random
 from petsc4py import PETSc
 from scipy.sparse import coo_matrix
 from scipy.sparse import load_npz
 
 
 def test_algo_list():
-    """Tests the algo list detection at lib creation."""
+    """Tests the algo list detection at library creation."""
     factory = LinearSolversFactory()
     assert factory.is_available("PetscKSPAlgos")
     assert factory.is_available("PETSC_KSP")
 
 
 def test_basic():
     """Test the resolution of a random linear problem."""
@@ -63,16 +62,16 @@
     assert problem.compute_residuals(True) < 1e-10
 
 
 def test_basic_using_hook():
     """Test the resolution of a random linear problem."""
 
     def func(
-        ksp,  # type: PETSc.KSP
-        options,  # type: Mapping[str, Any]
+        ksp: PETSc.KSP,
+        options: Mapping[str, Any],
     ):
         """Set the options of the KSP with options."""
         ksp.setType("cg")
 
     random.seed(1)
     n = 3
     problem = LinearProblem(eye(n), random.rand(n))
@@ -184,15 +183,15 @@
         preconditioner_type="ilu",
         monitor_residuals=False,
     )
     assert problem.compute_residuals(True) < 1e-3
 
 
 @pytest.fixture()
-def sobieski_disciplines():  # type: (...) -> List[MDODiscipline]
+def sobieski_disciplines() -> list[MDODiscipline]:
     """Return the Sobieski disciplines.
 
     Returns:
          The Sobieski disciplines.
     """
     disciplines = create_discipline(
         [
```

### Comparing `gemseo-petsc-2.0.0/tox.ini` & `gemseo-petsc-3.0.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -26,28 +26,29 @@
     # matplotlib cannot access a registry key and falls back to the WINDIR var
     # https://matplotlib.org/stable/api/font_manager_api.html#matplotlib.font_manager.win32FontDirectory.
     WINDIR = {env:WINDIR:C:\Windows}
     # Use a non GUI rendering backend for matplotlib.
     MPLBACKEND = AGG
     # Define pytest options for using coverage.
     coverage: __COVERAGE_POSARGS=--cov --cov-config=setup.cfg --cov-report=xml --cov-report=html
+    # Do not use ssh or rsh for initiating the MPI processes since it may not be available in docker.
+    OMPI_MCA_plm_rsh_agent =
 passenv =
     # See dev docs.
     GEMSEO_KEEP_IMAGE_COMPARISONS
 commands =
     pytest {env:__COVERAGE_POSARGS:} {posargs}
 
 [testenv:check]
 description = run code formatting and checking
 basepython = python3.9
 deps = -r requirements/check.txt
 conda_spec =
 skip_install = true
-whitelist_externals =
-    git
+whitelist_externals = pre-commit
 commands =
     pre-commit install
     pre-commit run --all-files
 
 [testenv:doc]
 description = build documentation
 basepython = python3.9
@@ -72,42 +73,45 @@
 whitelist_externals = rm
 commands =
     rm -rf dist build
     python -m build
     twine check dist/*
     python setup.py check --metadata
 
-[testenv:pypi-py{37,38,39,310}]
+[testenv:pypi-py{38,39,310}]
 description = test the pypi distribution
 deps = gemseo-petsc[test]
 skip_install = true
 
 [testenv:update-deps-{doc,dist,check}]
 description = update the non test envs dependencies
 basepython = python3.9
 extras =
     doc: {[testenv:doc]extras}
 setenv =
 passenv =
 deps = pip-tools
 conda_spec =
 skip_install = true
+whitelist_externals =
+    pip-compile
+    check: pre-commit
 commands =
     doc: pip-compile --upgrade --upgrade-package {[deps]gemseo} --extra doc -o requirements/doc.txt
     dist: pip-compile --upgrade requirements/dist.in
     check: pip-compile --upgrade requirements/check.in
     check: pre-commit autoupdate
 
-[testenv:update-deps-test-py{37,38,39,310}]
+[testenv:update-deps-test-py{38,39,310}]
 description = update the test envs dependencies
 extras = {[testenv]extras}
 setenv =
 passenv =
 conda_spec =
 deps = pip-tools
 whitelist_externals = sed
 skip_install = true
 commands =
     pip-compile --upgrade --upgrade-package {[deps]gemseo} --extra test -o requirements/test-{basepython}.txt
-    sed -i  '/mpi4py==/d' requirements/test-{basepython}.txt
-    sed -i  '/petsc4py==/d' requirements/test-{basepython}.txt
-    sed -i  '/petsc==/d' requirements/test-{basepython}.txt
+    sed -i '/mpi4py==/d' requirements/test-{basepython}.txt
+    sed -i '/petsc4py==/d' requirements/test-{basepython}.txt
+    sed -i '/petsc==/d' requirements/test-{basepython}.txt
```

