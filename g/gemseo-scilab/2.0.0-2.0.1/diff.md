# Comparing `tmp/gemseo-scilab-2.0.0.tar.gz` & `tmp/gemseo-scilab-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemseo-scilab-2.0.0.tar", last modified: Thu Jul 28 09:56:25 2022, max compression
+gzip compressed data, was "gemseo-scilab-2.0.1.tar", last modified: Mon Jun  5 12:32:29 2023, max compression
```

## Comparing `gemseo-scilab-2.0.0.tar` & `gemseo-scilab-2.0.1.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.798916 gemseo-scilab-2.0.0/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      450 2021-09-07 12:00:53.000000 gemseo-scilab-2.0.0/.gitattributes
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      192 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/.gitignore
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.792916 gemseo-scilab-2.0.0/.gitlab/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.795916 gemseo-scilab-2.0.0/.gitlab/issue_templates/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1126 2021-11-09 15:46:38.000000 gemseo-scilab-2.0.0/.gitlab/issue_templates/Bug.md
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1029 2021-11-09 15:46:38.000000 gemseo-scilab-2.0.0/.gitlab/issue_templates/Documentation.md
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1033 2021-11-09 15:46:38.000000 gemseo-scilab-2.0.0/.gitlab/issue_templates/Feature Proposal.md
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      771 2021-11-09 15:46:38.000000 gemseo-scilab-2.0.0/.gitlab/issue_templates/Refactoring.md
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2464 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/.gitlab-ci.yml
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2491 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     9105 2021-09-07 12:00:53.000000 gemseo-scilab-2.0.0/.pylintrc
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1043 2022-07-28 09:46:42.000000 gemseo-scilab-2.0.0/CHANGELOG.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1571 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/CREDITS.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     7652 2022-01-04 15:28:03.000000 gemseo-scilab-2.0.0/LICENSE.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.795916 gemseo-scilab-2.0.0/LICENSES/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    35149 2021-09-07 15:39:06.000000 gemseo-scilab-2.0.0/LICENSES/GPLv3.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.795916 gemseo-scilab-2.0.0/LICENSES/headers/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      729 2021-09-07 15:39:06.000000 gemseo-scilab-2.0.0/LICENSES/headers/BSD-0-Clause.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      334 2021-09-07 15:39:06.000000 gemseo-scilab-2.0.0/LICENSES/headers/CC-BY-SA-4.0.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      710 2021-09-07 15:39:06.000000 gemseo-scilab-2.0.0/LICENSES/headers/LGPL-3.0.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2575 2022-07-28 09:56:25.798916 gemseo-scilab-2.0.0/PKG-INFO
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1452 2021-09-23 08:54:22.000000 gemseo-scilab-2.0.0/README.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      611 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/pyproject.toml
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.796916 gemseo-scilab-2.0.0/requirements/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       79 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/requirements/check.in
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      629 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/requirements/check.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       12 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/requirements/dist.in
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1373 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/requirements/dist.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1460 2022-07-28 09:55:53.000000 gemseo-scilab-2.0.0/requirements/doc.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2132 2022-07-28 09:55:53.000000 gemseo-scilab-2.0.0/requirements/test-python3.10.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2388 2022-07-28 09:55:53.000000 gemseo-scilab-2.0.0/requirements/test-python3.7.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2130 2022-07-28 09:55:53.000000 gemseo-scilab-2.0.0/requirements/test-python3.8.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2130 2022-07-28 09:55:53.000000 gemseo-scilab-2.0.0/requirements/test-python3.9.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1618 2022-07-28 09:56:25.799916 gemseo-scilab-2.0.0/setup.cfg
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      839 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/setup.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.793916 gemseo-scilab-2.0.0/src/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.796916 gemseo-scilab-2.0.0/src/gemseo_scilab/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      802 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/src/gemseo_scilab/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     6000 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/src/gemseo_scilab/py_scilab.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     5361 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/src/gemseo_scilab/scilab_discipline.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.797916 gemseo-scilab-2.0.0/src/gemseo_scilab.egg-info/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2575 2022-07-28 09:56:25.000000 gemseo-scilab-2.0.0/src/gemseo_scilab.egg-info/PKG-INFO
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1301 2022-07-28 09:56:25.000000 gemseo-scilab-2.0.0/src/gemseo_scilab.egg-info/SOURCES.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        1 2022-07-28 09:56:25.000000 gemseo-scilab-2.0.0/src/gemseo_scilab.egg-info/dependency_links.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       47 2022-07-28 09:56:25.000000 gemseo-scilab-2.0.0/src/gemseo_scilab.egg-info/entry_points.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       82 2022-07-28 09:56:25.000000 gemseo-scilab-2.0.0/src/gemseo_scilab.egg-info/requires.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       14 2022-07-28 09:56:25.000000 gemseo-scilab-2.0.0/src/gemseo_scilab.egg-info/top_level.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.797916 gemseo-scilab-2.0.0/tests/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      801 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/tests/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1137 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/tests/conftest.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.793916 gemseo-scilab-2.0.0/tests/sci/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.797916 gemseo-scilab-2.0.0/tests/sci/dummy_func/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1539 2021-11-09 15:46:38.000000 gemseo-scilab-2.0.0/tests/sci/dummy_func/dummy_package.sci
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.798916 gemseo-scilab-2.0.0/tests/sci/no_args/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      780 2021-09-23 08:50:35.000000 gemseo-scilab-2.0.0/tests/sci/no_args/no_args.sci
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.798916 gemseo-scilab-2.0.0/tests/sci/no_func/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      340 2021-09-23 08:50:35.000000 gemseo-scilab-2.0.0/tests/sci/no_func/no_func_name.sci
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.798916 gemseo-scilab-2.0.0/tests/sci/no_output/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      370 2021-09-23 08:50:35.000000 gemseo-scilab-2.0.0/tests/sci/no_output/no_output.sci
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.798916 gemseo-scilab-2.0.0/tests/sci/str_rep/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      371 2021-09-23 08:50:35.000000 gemseo-scilab-2.0.0/tests/sci/str_rep/str_repr.sci
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3009 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/tests/test_py_scilab.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3984 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/tests/test_scilab_discipline.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:56:25.798916 gemseo-scilab-2.0.0/tools/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      482 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/tools/Dockerfile
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3194 2022-07-28 09:45:55.000000 gemseo-scilab-2.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.995842 gemseo-scilab-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.982842 gemseo-scilab-2.0.1/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.988842 gemseo-scilab-2.0.1/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/.gitlab/issue_templates/Bug.md
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/.gitlab/issue_templates/Documentation.md
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/.gitlab/issue_templates/Feature Proposal.md
+-rw-rw-rw-   0 root         (0) root         (0)      771 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/.gitlab/issue_templates/Refactoring.md
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     9105 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/CREDITS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.988842 gemseo-scilab-2.0.1/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/LICENSES/GPLv3.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.989842 gemseo-scilab-2.0.1/LICENSES/headers/
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/LICENSES/headers/BSD-0-Clause.txt
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/LICENSES/headers/CC-BY-SA-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/LICENSES/headers/LGPL-3.0.txt
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-06-05 12:32:29.995842 gemseo-scilab-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.990842 gemseo-scilab-2.0.1/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/requirements/check.in
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/requirements/check.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/requirements/dist.in
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/requirements/dist.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/requirements/doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2198 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/requirements/test-python3.10.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2288 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/requirements/test-python3.8.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2288 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/requirements/test-python3.9.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2023-06-05 12:32:29.996842 gemseo-scilab-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.983842 gemseo-scilab-2.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.991842 gemseo-scilab-2.0.1/src/gemseo_scilab/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/src/gemseo_scilab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/src/gemseo_scilab/py_scilab.py
+-rw-rw-rw-   0 root         (0) root         (0)     4703 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/src/gemseo_scilab/scilab_discipline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.992842 gemseo-scilab-2.0.1/src/gemseo_scilab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-06-05 12:32:29.000000 gemseo-scilab-2.0.1/src/gemseo_scilab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-06-05 12:32:29.000000 gemseo-scilab-2.0.1/src/gemseo_scilab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 12:32:29.000000 gemseo-scilab-2.0.1/src/gemseo_scilab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-05 12:32:29.000000 gemseo-scilab-2.0.1/src/gemseo_scilab.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-06-05 12:32:29.000000 gemseo-scilab-2.0.1/src/gemseo_scilab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-05 12:32:29.000000 gemseo-scilab-2.0.1/src/gemseo_scilab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.993842 gemseo-scilab-2.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.984841 gemseo-scilab-2.0.1/tests/sci/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.993842 gemseo-scilab-2.0.1/tests/sci/dummy_func/
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tests/sci/dummy_func/dummy_package.sci
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.994842 gemseo-scilab-2.0.1/tests/sci/no_args/
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tests/sci/no_args/no_args.sci
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.994842 gemseo-scilab-2.0.1/tests/sci/no_func/
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tests/sci/no_func/no_func_name.sci
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.994842 gemseo-scilab-2.0.1/tests/sci/no_output/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tests/sci/no_output/no_output.sci
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.994842 gemseo-scilab-2.0.1/tests/sci/str_rep/
+-rw-rw-rw-   0 root         (0) root         (0)      371 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tests/sci/str_rep/str_repr.sci
+-rw-rw-rw-   0 root         (0) root         (0)     3009 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tests/test_py_scilab.py
+-rw-rw-rw-   0 root         (0) root         (0)     3929 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tests/test_scilab_discipline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:32:29.995842 gemseo-scilab-2.0.1/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tools/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     3251 2023-06-05 12:32:12.000000 gemseo-scilab-2.0.1/tox.ini
```

### Comparing `gemseo-scilab-2.0.0/.gitlab/issue_templates/Bug.md` & `gemseo-scilab-2.0.1/.gitlab/issue_templates/Bug.md`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/.gitlab/issue_templates/Documentation.md` & `gemseo-scilab-2.0.1/.gitlab/issue_templates/Documentation.md`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/.gitlab/issue_templates/Feature Proposal.md` & `gemseo-scilab-2.0.1/.gitlab/issue_templates/Feature Proposal.md`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/.gitlab/issue_templates/Refactoring.md` & `gemseo-scilab-2.0.1/.gitlab/issue_templates/Refactoring.md`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/.pylintrc` & `gemseo-scilab-2.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/CHANGELOG.rst` & `gemseo-scilab-2.0.1/CHANGELOG.rst`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 
 The format is based on
 `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_
 and this project adheres to
 `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
 
+Version 2.0.1 (June 2023)
+*************************
+
+Update to GEMSEO 5.
+
+
 Version 2.0.0 (November 2021)
 *****************************
 
 Update to GEMSEO 4.0.0.
 
 
 Version 1.0.0 (November 2021)
```

### Comparing `gemseo-scilab-2.0.0/CREDITS.rst` & `gemseo-scilab-2.0.1/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/LICENSE.txt` & `gemseo-scilab-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/LICENSES/GPLv3.txt` & `gemseo-scilab-2.0.1/LICENSES/GPLv3.txt`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/LICENSES/headers/BSD-0-Clause.txt` & `gemseo-scilab-2.0.1/LICENSES/headers/BSD-0-Clause.txt`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/LICENSES/headers/LGPL-3.0.txt` & `gemseo-scilab-2.0.1/LICENSES/headers/LGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/PKG-INFO` & `gemseo-scilab-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-scilab
-Version: 2.0.0
+Version: 2.0.1
 Summary: GEMSEO plugin to create disciplines from scilab source code.
 Home-page: https://gitlab.com/gemseo
 Author: François Gallard
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-scilab
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-scilab/-/issues
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
```

### Comparing `gemseo-scilab-2.0.0/README.rst` & `gemseo-scilab-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/pyproject.toml` & `gemseo-scilab-2.0.1/pyproject.toml`

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

### Comparing `gemseo-scilab-2.0.0/requirements/check.txt` & `gemseo-scilab-2.0.1/requirements/check.txt`

 * *Files 17% similar despite different names*

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
+pre-commit==3.3.1
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

### Comparing `gemseo-scilab-2.0.0/requirements/dist.txt` & `gemseo-scilab-2.0.1/requirements/dist.txt`

 * *Files 13% similar despite different names*

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
+docutils==0.20
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
+requests==2.30.0
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

### Comparing `gemseo-scilab-2.0.0/requirements/doc.txt` & `gemseo-scilab-2.0.1/requirements/doc.txt`

 * *Files 6% similar despite different names*

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
     # via gemseo-scilab (setup.py)
 genson==1.2.2
     # via gemseo
 h5py==3.6.0
     # via gemseo
 idna==3.3
     # via requests
```

### Comparing `gemseo-scilab-2.0.0/requirements/test-python3.10.txt` & `gemseo-scilab-2.0.1/requirements/test-python3.9.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,117 +1,120 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.9.txt
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
     # via gemseo-scilab (setup.py)
-coverage[toml]==6.4.2
+coverage[toml]==7.2.5
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
     # via gemseo-scilab (setup.py)
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
-networkx==2.8.5
+networkx==3.1
     # via gemseo
-numpy==1.22.4
+numpy==1.23.5
     # via
+    #   contourpy
     #   gemseo
+    #   gemseo-scilab (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
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
     #   gemseo-scilab (setup.py)
     #   pytest-cov
-    #   pytest-forked
     #   pytest-xdist
-pytest-cov==3.0.0
+pytest-cov==4.0.0
     # via gemseo-scilab (setup.py)
-pytest-forked==1.4.0
-    # via pytest-xdist
-pytest-xdist==2.5.0
+pytest-xdist==3.3.0
     # via gemseo-scilab (setup.py)
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
+requests==2.30.0
     # via gemseo
 scilab2py==0.6.2
     # via gemseo-scilab (setup.py)
-scipy==1.7.3
+scipy==1.10.1
     # via gemseo
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
+typing-extensions==4.5.0
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

### Comparing `gemseo-scilab-2.0.0/requirements/test-python3.7.txt` & `gemseo-scilab-2.0.1/requirements/test-python3.10.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,131 +1,116 @@
 #
-# This file is autogenerated by pip-compile with python 3.7
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.7.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
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
     # via gemseo-scilab (setup.py)
-coverage[toml]==6.4.2
+coverage[toml]==7.2.5
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
     # via gemseo-scilab (setup.py)
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
-networkx==2.6.3
+networkx==3.1
     # via gemseo
-numpy==1.21.6
+numpy==1.23.5
     # via
+    #   contourpy
     #   gemseo
+    #   gemseo-scilab (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
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
     #   gemseo-scilab (setup.py)
     #   pytest-cov
-    #   pytest-forked
     #   pytest-xdist
-pytest-cov==3.0.0
+pytest-cov==4.0.0
     # via gemseo-scilab (setup.py)
-pytest-forked==1.4.0
-    # via pytest-xdist
-pytest-xdist==2.5.0
+pytest-xdist==3.3.0
     # via gemseo-scilab (setup.py)
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
+requests==2.30.0
     # via gemseo
 scilab2py==0.6.2
     # via gemseo-scilab (setup.py)
-scipy==1.7.3
-    # via gemseo
-singledispatchmethod==1.0
+scipy==1.10.1
     # via gemseo
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
+typing-extensions==4.5.0
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
```

### Comparing `gemseo-scilab-2.0.0/requirements/test-python3.8.txt` & `gemseo-scilab-2.0.1/requirements/test-python3.8.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,117 +1,120 @@
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
     # via gemseo-scilab (setup.py)
-coverage[toml]==6.4.2
+coverage[toml]==7.2.5
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
     # via gemseo-scilab (setup.py)
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
-networkx==2.8.5
+networkx==3.1
     # via gemseo
-numpy==1.22.4
+numpy==1.23.5
     # via
+    #   contourpy
     #   gemseo
+    #   gemseo-scilab (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
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
     #   gemseo-scilab (setup.py)
     #   pytest-cov
-    #   pytest-forked
     #   pytest-xdist
-pytest-cov==3.0.0
+pytest-cov==4.0.0
     # via gemseo-scilab (setup.py)
-pytest-forked==1.4.0
-    # via pytest-xdist
-pytest-xdist==2.5.0
+pytest-xdist==3.3.0
     # via gemseo-scilab (setup.py)
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
+requests==2.30.0
     # via gemseo
 scilab2py==0.6.2
     # via gemseo-scilab (setup.py)
-scipy==1.7.3
+scipy==1.10.1
     # via gemseo
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
+typing-extensions==4.5.0
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

### Comparing `gemseo-scilab-2.0.0/setup.cfg` & `gemseo-scilab-2.0.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -17,28 +17,28 @@
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
-	scilab2py >=0.6.0
+	gemseo >=5
+	numpy <1.24
+	scilab2py ==0.6.2
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test = 
 	covdefaults
@@ -62,15 +62,21 @@
 
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
+per-file-ignores = 
+	tests/*.py: D100,D104,ANN
+	doc_src/*.py: D,T201
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gemseo-scilab-2.0.0/setup.py` & `gemseo-scilab-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/src/gemseo_scilab/__init__.py` & `gemseo-scilab-2.0.1/src/gemseo_scilab/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/src/gemseo_scilab/py_scilab.py` & `gemseo-scilab-2.0.1/src/gemseo_scilab/py_scilab.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,35 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Scilab wrapper."""
 from __future__ import annotations
 
 import logging
 import re
-from glob import glob
 from pathlib import Path
+from typing import Any
+from typing import Callable
+from typing import Final
 from typing import Sequence
 
 from numpy import ndarray
 from scilab2py import scilab
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ScilabFunction:
     """A scilab function."""
 
+    _f_pointer: Callable | None
+    _fun_def: str
+    name: str
+    args: Sequence[str]
+    outs: Sequence[str]
+
     def __init__(
         self,
         fun_def: str,
         name: str,
         args: Sequence[str],
         outs: Sequence[str],
     ) -> None:
@@ -49,67 +57,68 @@
         self._fun_def = fun_def
         self.name = name
         self.args = args
         self.outs = outs
 
         self.__init_from_def()
 
-    def __call__(self, *args, **kwargs) -> dict[str, float | ndarray]:
-        """Call the scilab function."""
+    def __call__(  # noqa: D102
+        self, *args: Any, **kwargs: Any
+    ) -> dict[str, float | ndarray]:
         return self._f_pointer(*args, **kwargs)
 
     def __init_from_def(self) -> None:
         """Initialize the function from its definition."""
         exec(self._fun_def)
         self._f_pointer = locals()[self.name]
 
-    def __getstate__(self):
+    def __getstate__(self) -> dict[str, Any]:
         out_dict = self.__dict__.copy()
         del out_dict["_f_pointer"]
         return out_dict
 
-    def __setstate__(self, state):
+    def __setstate__(self, state: dict[str, Any]) -> None:
         self.__dict__.update(state)
         self._f_pointer = None
         self.__init_from_def()
 
 
 class ScilabPackage:
     """Interface to a scilab package.
 
     Scilab python interface scans the sci files in a directory and generates python
     functions from them.
     """
 
-    RE_OUTS = re.compile(r"\[([^$].*?)]")
-    RE_FUNC = re.compile(r"=([^$].*?)\(")
-    RE_ARGS = re.compile(r"\(([^$].*?)\)")
+    RE_OUTS: Final[re.Pattern] = re.compile(r"\[([^$].*?)]")
+    RE_FUNC: Final[re.Pattern] = re.compile(r"=([^$].*?)\(")
+    RE_ARGS: Final[re.Pattern] = re.compile(r"\(([^$].*?)\)")
 
-    def __init__(self, script_dir_path: str) -> None:
+    def __init__(self, script_dir_path: str | Path) -> None:
         """Constructor.
 
         Args:
-            script_dir_path : The path to the directory to scan for .sci files.
+            script_dir_path: The path to the directory to scan for .sci files.
 
         Raises:
             FileNotFoundError: If the `script_dir_path` does not exist.
         """
-        if not Path(script_dir_path).exists():
+        script_dir_path = Path(script_dir_path)
+        if not script_dir_path.is_dir():
             raise FileNotFoundError(
                 f"Script directory for Scilab sources: {script_dir_path}"
                 " does not exist."
             )
 
         # scilab.timeout = 10
-        LOGGER.info("Use scilab script directory: %s", script_dir_path)
+        LOGGER.info("Using the scilab script directory: %s", script_dir_path)
 
-        self.__script_dir_path = script_dir_path
         scilab.getd(str(script_dir_path))
         self.functions = {}
-        self.__scan_funcs()
+        self.__scan_funcs(script_dir_path)
 
     def __scan_onef(self, line: str) -> None:
         """Scan a function in a sci file to parse its arguments, outputs and name.
 
         Args:
             line: The line from the sci file to scan.
 
@@ -156,21 +165,21 @@
     outputs: {outs_form}
     '''
     {outs_form} = scilab.{fname}({args_form})
     return {outs_form}
 """
         self.functions[fname] = ScilabFunction(fun_def, fname, fargs, fouts)
 
-    def __scan_funcs(self) -> None:
+    def __scan_funcs(self, script_dir_path: Path) -> None:
         """Scan all functions in the directory.
 
         Raises:
             ValueError: If an interface cannot be generated for a function.
         """
-        for script_f in glob(str(Path(self.__script_dir_path) / "*.sci")):
+        for script_f in script_dir_path.glob("*.sci"):
             LOGGER.info("Found script file: %s", script_f)
 
             with open(script_f) as script:
                 for line in script.readlines():
                     if not line.strip().startswith("function"):
                         continue
```

### Comparing `gemseo-scilab-2.0.0/src/gemseo_scilab/scilab_discipline.py` & `gemseo-scilab-2.0.1/src/gemseo_scilab/scilab_discipline.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Scilab discipline."""
 from __future__ import annotations
 
 import logging
+from copy import copy
 from typing import Mapping
+from typing import MutableMapping
 
 from gemseo.core.data_processor import DataProcessor
 from gemseo.core.discipline import MDODiscipline
 from numpy import array
 from numpy import ndarray
 
 from gemseo_scilab.py_scilab import ScilabFunction
@@ -44,31 +46,32 @@
                 generate the discipline from.
             script_dir_path: The path to the directory to scan for `.sci` files.
 
         Raises:
             ValueError: If the function is not in any of the files of
                 the `script_dir_path`.
         """
-        super().__init__(
-            name=function_name,
-            auto_detect_grammar_files=False,
-            grammar_type=MDODiscipline.JSON_GRAMMAR_TYPE,
-        )
         self.__scilab_package = ScilabPackage(script_dir_path)
 
         if function_name not in self.__scilab_package.functions:
             raise ValueError(
                 f"The function named {function_name}"
                 f" is not in script_dir {script_dir_path}"
             )
 
         self._scilab_function = self.__scilab_package.functions[function_name]
 
-        self.input_grammar.update_from_data(self.__base_input_data)
-        self.output_grammar.update_from_data(self.__base_output_data)
+        super().__init__(
+            name=function_name,
+            auto_detect_grammar_files=False,
+            grammar_type=MDODiscipline.GrammarType.JSON,
+        )
+
+        self.input_grammar.update_from_names(self._scilab_function.args)
+        self.output_grammar.update_from_names(self._scilab_function.outs)
         self.data_processor = ScilabDataProcessor(self._scilab_function)
 
     def _run(self) -> None:
         """Run the discipline.
 
         Raises:
             BaseException: If the discipline execution fails.
@@ -85,61 +88,39 @@
 
         if len(out_names) == 1:
             self.store_local_data(**{out_names[0]: output_data})
         else:
             for out_n, out_v in zip(out_names, output_data):
                 self.store_local_data(**{out_n: out_v})
 
-    @property
-    def __base_input_data(self) -> dict[str, float | ndarray]:
-        """The data to initialize the inputs."""
-        def_data = [0.1]
-        return {k: def_data for k in self._scilab_function.args}
-
-    @property
-    def __base_output_data(self) -> dict[str, float | ndarray]:
-        """The data to initialize the outputs."""
-        def_data = [0.1]
-        return {k: def_data for k in self._scilab_function.outs}
-
-    def get_attributes_to_serialize(self) -> list[str]:
-        """Define the attributes to be serialized.
-
-        Returns:
-            The attributes names.
-        """
-        attrs = super().get_attributes_to_serialize()
-        attrs.append("_scilab_function")
-        return attrs
-
 
 class ScilabDataProcessor(DataProcessor):
     """A scilab function data processor."""
 
     def __init__(self, scilab_function: ScilabFunction) -> None:
         """Constructor.
 
         Args:
             scilab_function: The scilab function.
         """
         super().__init__()
         self._scilab_function = scilab_function
 
     def pre_process_data(
-        self, input_data: Mapping[str, ndarray]
-    ) -> dict[str, float | ndarray]:
+        self, input_data: MutableMapping[str, ndarray]
+    ) -> Mapping[str, ndarray]:
         """Convert the input from GEMSEO to scilab.
 
         Args:
             input_data: The input data.
 
         Returns:
             The data to be passed to scilab.
         """
-        processed_data = input_data.copy()
+        processed_data = copy(input_data)
         for data_name in self._scilab_function.args:
             processed_data[data_name] = processed_data[data_name]
         return processed_data
 
     def post_process_data(
         self, local_data: Mapping[str, float | ndarray]
     ) -> dict[str, ndarray]:
```

### Comparing `gemseo-scilab-2.0.0/src/gemseo_scilab.egg-info/PKG-INFO` & `gemseo-scilab-2.0.1/src/gemseo_scilab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-scilab
-Version: 2.0.0
+Version: 2.0.1
 Summary: GEMSEO plugin to create disciplines from scilab source code.
 Home-page: https://gitlab.com/gemseo
 Author: François Gallard
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-scilab
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-scilab/-/issues
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
```

### Comparing `gemseo-scilab-2.0.0/src/gemseo_scilab.egg-info/SOURCES.txt` & `gemseo-scilab-2.0.1/src/gemseo_scilab.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 LICENSES/headers/LGPL-3.0.txt
 requirements/check.in
 requirements/check.txt
 requirements/dist.in
 requirements/dist.txt
 requirements/doc.txt
 requirements/test-python3.10.txt
-requirements/test-python3.7.txt
 requirements/test-python3.8.txt
 requirements/test-python3.9.txt
 src/gemseo_scilab/__init__.py
 src/gemseo_scilab/py_scilab.py
 src/gemseo_scilab/scilab_discipline.py
 src/gemseo_scilab.egg-info/PKG-INFO
 src/gemseo_scilab.egg-info/SOURCES.txt
```

### Comparing `gemseo-scilab-2.0.0/tests/__init__.py` & `gemseo-scilab-2.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/tests/conftest.py` & `gemseo-scilab-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/tests/sci/dummy_func/dummy_package.sci` & `gemseo-scilab-2.0.1/tests/sci/dummy_func/dummy_package.sci`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/tests/sci/no_args/no_args.sci` & `gemseo-scilab-2.0.1/tests/sci/no_args/no_args.sci`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/tests/test_py_scilab.py` & `gemseo-scilab-2.0.1/tests/test_py_scilab.py`

 * *Files identical despite different names*

### Comparing `gemseo-scilab-2.0.0/tests/test_scilab_discipline.py` & `gemseo-scilab-2.0.1/tests/test_scilab_discipline.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Tests for the scilab discipline."""
 from __future__ import annotations
 
 import logging
 import pickle
 from pathlib import Path
-from typing import Dict
 from typing import Mapping
 
 import pytest
 from gemseo_scilab.py_scilab import ScilabPackage
 from gemseo_scilab.scilab_discipline import ScilabDiscipline
 from numpy import array
 from numpy import ndarray
@@ -31,17 +30,17 @@
 DIRNAME = Path(__file__).parent / "sci/dummy_func"
 
 
 DUMMY_FUNCS = ["dummy_func1", "dummy_func2", "dummy_func3", "dummy_func4"]
 
 
 def exec_disc(
-    fname,  # type: str
-    in_data,  # type: Mapping[str, ndarray]
-):  # type: (...) -> Dict[str, ndarray]
+    fname: str,
+    in_data: Mapping[str, ndarray],
+) -> dict[str, ndarray]:
     """Create and execute a scilab discipline.
 
     Args:
         fname: The name of the function.
         in_data: The input data.
 
     Returns:
@@ -92,15 +91,15 @@
     """Test the execution of a ScilabDiscipline in parallel.
 
     Args:
         tmp_wd: Fixture to move into a temporary work directory.
     """
     disc = ScilabDiscipline("dummy_func1", DIRNAME)
     outf = "outf.pck"
-    disc.serialize(outf)
+    disc.to_pickle(outf)
     inputs = {"b": array([1.0])}
     out_ref = disc.execute(inputs)
 
     disc_load = pickle.load(open(outf, "rb"))
     out = disc_load.execute(inputs)
     assert (out["a"] == out_ref["a"]).all()
```

### Comparing `gemseo-scilab-2.0.0/tox.ini` & `gemseo-scilab-2.0.1/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     pytest {env:__COVERAGE_POSARGS:} {posargs}
 
 [testenv:check]
 description = run code formatting and checking
 basepython = python3.9
 deps = -r requirements/check.txt
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
@@ -66,35 +65,38 @@
 whitelist_externals = rm
 commands =
     rm -rf dist build
     python -m build
     twine check dist/*
     python setup.py check --metadata
 
-[testenv:pypi-py{37,38,39,310}]
+[testenv:pypi-py{38,39,310}]
 description = test the pypi distribution
 deps = gemseo-scilab[test]
 skip_install = true
 
 [testenv:update-deps-{doc,dist,check}]
 description = update the non test envs dependencies
 basepython = python3.9
 extras =
     doc: {[testenv:doc]extras}
 setenv =
 passenv =
 deps = pip-tools
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
 deps = pip-tools
 skip_install = true
 commands =
```

