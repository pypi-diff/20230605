# Comparing `tmp/gemseo-mma-1.0.0.tar.gz` & `tmp/gemseo-mma-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemseo-mma-1.0.0.tar", last modified: Thu Feb  9 10:57:15 2023, max compression
+gzip compressed data, was "gemseo-mma-2.0.0.tar", last modified: Mon Jun  5 13:03:12 2023, max compression
```

## Comparing `gemseo-mma-1.0.0.tar` & `gemseo-mma-2.0.0.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.035034 gemseo-mma-1.0.0/
--rw-r--r--   0 ad        (1000) ad        (1000)      450 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/.gitattributes
--rw-r--r--   0 ad        (1000) ad        (1000)      189 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/.gitignore
--rw-r--r--   0 ad        (1000) ad        (1000)       87 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/.gitlab-ci.yml
--rw-r--r--   0 ad        (1000) ad        (1000)     2969 2023-02-09 06:43:44.000000 gemseo-mma-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 ad        (1000) ad        (1000)     9105 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/.pylintrc
--rw-r--r--   0 ad        (1000) ad        (1000)      960 2023-02-09 06:38:26.000000 gemseo-mma-1.0.0/CHANGELOG.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     1837 2023-02-09 06:37:23.000000 gemseo-mma-1.0.0/CREDITS.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     7652 2022-03-24 13:18:51.000000 gemseo-mma-1.0.0/LICENSE.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.030034 gemseo-mma-1.0.0/LICENSES/
--rw-r--r--   0 ad        (1000) ad        (1000)    35149 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/LICENSES/GPLv3.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     7652 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/LICENSES/LGPLv3.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.031034 gemseo-mma-1.0.0/LICENSES/headers/
--rw-r--r--   0 ad        (1000) ad        (1000)      729 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/LICENSES/headers/BSD-0-Clause.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      334 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/LICENSES/headers/CC-BY-SA-4.0.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      710 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/LICENSES/headers/LGPL-3.0.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     4665 2023-02-09 10:57:15.035034 gemseo-mma-1.0.0/PKG-INFO
--rw-r--r--   0 ad        (1000) ad        (1000)     3507 2023-02-09 06:50:05.000000 gemseo-mma-1.0.0/README.rst
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.031034 gemseo-mma-1.0.0/examples/
--rw-r--r--   0 ad        (1000) ad        (1000)   161103 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/examples/analytic_example.ipynb
--rw-r--r--   0 ad        (1000) ad        (1000)      611 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/pyproject.toml
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.033034 gemseo-mma-1.0.0/requirements/
--rw-r--r--   0 ad        (1000) ad        (1000)       79 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/requirements/check.in
--rw-r--r--   0 ad        (1000) ad        (1000)      597 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/requirements/check.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       12 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/requirements/dist.in
--rw-r--r--   0 ad        (1000) ad        (1000)     1459 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/requirements/dist.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2116 2023-02-09 10:57:01.000000 gemseo-mma-1.0.0/requirements/test-python3.10.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2279 2023-02-09 10:57:01.000000 gemseo-mma-1.0.0/requirements/test-python3.7.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2114 2023-02-09 10:57:01.000000 gemseo-mma-1.0.0/requirements/test-python3.8.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2114 2023-02-09 10:57:01.000000 gemseo-mma-1.0.0/requirements/test-python3.9.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     1698 2023-02-09 10:57:15.036034 gemseo-mma-1.0.0/setup.cfg
--rw-r--r--   0 ad        (1000) ad        (1000)      839 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/setup.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.027034 gemseo-mma-1.0.0/src/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.033034 gemseo-mma-1.0.0/src/gemseo_mma/
--rw-r--r--   0 ad        (1000) ad        (1000)      830 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/src/gemseo_mma/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.034034 gemseo-mma-1.0.0/src/gemseo_mma/opt/
--rw-r--r--   0 ad        (1000) ad        (1000)      818 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/src/gemseo_mma/opt/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.035034 gemseo-mma-1.0.0/src/gemseo_mma/opt/core/
--rw-r--r--   0 ad        (1000) ad        (1000)      856 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/src/gemseo_mma/opt/core/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)    21269 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/src/gemseo_mma/opt/core/mma.py
--rw-r--r--   0 ad        (1000) ad        (1000)    12046 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/src/gemseo_mma/opt/core/mma_optimizer.py
--rw-r--r--   0 ad        (1000) ad        (1000)     7923 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/src/gemseo_mma/opt/lib_mma.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.035034 gemseo-mma-1.0.0/src/gemseo_mma/opt/options/
--rw-r--r--   0 ad        (1000) ad        (1000)     2103 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/src/gemseo_mma/opt/options/MMA_options.json
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.034034 gemseo-mma-1.0.0/src/gemseo_mma.egg-info/
--rw-r--r--   0 ad        (1000) ad        (1000)     4665 2023-02-09 10:57:14.000000 gemseo-mma-1.0.0/src/gemseo_mma.egg-info/PKG-INFO
--rw-r--r--   0 ad        (1000) ad        (1000)     1052 2023-02-09 10:57:15.000000 gemseo-mma-1.0.0/src/gemseo_mma.egg-info/SOURCES.txt
--rw-r--r--   0 ad        (1000) ad        (1000)        1 2023-02-09 10:57:14.000000 gemseo-mma-1.0.0/src/gemseo_mma.egg-info/dependency_links.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       41 2023-02-09 10:57:14.000000 gemseo-mma-1.0.0/src/gemseo_mma.egg-info/entry_points.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       73 2023-02-09 10:57:14.000000 gemseo-mma-1.0.0/src/gemseo_mma.egg-info/requires.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       11 2023-02-09 10:57:14.000000 gemseo-mma-1.0.0/src/gemseo_mma.egg-info/top_level.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 10:57:15.035034 gemseo-mma-1.0.0/tests/
--rw-r--r--   0 ad        (1000) ad        (1000)     5635 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/tests/test_mma_optimization.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3250 2023-02-09 06:17:25.000000 gemseo-mma-1.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.561532 gemseo-mma-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     9105 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/CREDITS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.555532 gemseo-mma-2.0.0/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/LICENSES/GPLv3.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/LICENSES/LGPLv3.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.556532 gemseo-mma-2.0.0/LICENSES/headers/
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/LICENSES/headers/BSD-0-Clause.txt
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/LICENSES/headers/CC-BY-SA-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/LICENSES/headers/LGPL-3.0.txt
+-rw-r--r--   0 root         (0) root         (0)     4707 2023-06-05 13:03:12.561532 gemseo-mma-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3599 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.556532 gemseo-mma-2.0.0/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     5963 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/examples/analytic_example.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.557532 gemseo-mma-2.0.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/requirements/check.in
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/requirements/check.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/requirements/dist.in
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/requirements/dist.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2166 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/requirements/test-python3.10.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/requirements/test-python3.8.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/requirements/test-python3.9.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1695 2023-06-05 13:03:12.561532 gemseo-mma-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.551532 gemseo-mma-2.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.558532 gemseo-mma-2.0.0/src/gemseo_mma/
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/src/gemseo_mma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.559532 gemseo-mma-2.0.0/src/gemseo_mma/opt/
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/src/gemseo_mma/opt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.560532 gemseo-mma-2.0.0/src/gemseo_mma/opt/core/
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/src/gemseo_mma/opt/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21270 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/src/gemseo_mma/opt/core/mma.py
+-rw-rw-rw-   0 root         (0) root         (0)    12787 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/src/gemseo_mma/opt/core/mma_optimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7565 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/src/gemseo_mma/opt/lib_mma.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.560532 gemseo-mma-2.0.0/src/gemseo_mma/opt/options/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/src/gemseo_mma/opt/options/MMA_options.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.559532 gemseo-mma-2.0.0/src/gemseo_mma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4707 2023-06-05 13:03:12.000000 gemseo-mma-2.0.0/src/gemseo_mma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-05 13:03:12.000000 gemseo-mma-2.0.0/src/gemseo_mma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 13:03:12.000000 gemseo-mma-2.0.0/src/gemseo_mma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-05 13:03:12.000000 gemseo-mma-2.0.0/src/gemseo_mma.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 13:03:12.000000 gemseo-mma-2.0.0/src/gemseo_mma.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-05 13:03:12.000000 gemseo-mma-2.0.0/src/gemseo_mma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 13:03:12.561532 gemseo-mma-2.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6346 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/tests/test_mma_optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     3266 2023-06-05 13:02:54.000000 gemseo-mma-2.0.0/tox.ini
```

### Comparing `gemseo-mma-1.0.0/.pre-commit-config.yaml` & `gemseo-mma-2.0.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   rev: v1.10.0
   hooks:
     - id: rst-backticks
     - id: rst-directive-colons
     - id: rst-inline-touching-normal
 
 - repo: https://github.com/PyCQA/autoflake
-  rev: v2.0.0
+  rev: v2.1.1
   hooks:
     - id: autoflake
       args: [
         --in-place,
         --remove-all-unused-imports,
       ]
 
@@ -36,74 +36,83 @@
   hooks:
     - id: reorder-python-imports
       name: reorder python imports in src
       files: ^src
       args: [
         --application-directories,
         src,
-        --py37-plus,
+        --py38-plus,
         --add-import,
         "from __future__ import annotations",
-        --replace-import,
-        "typing=gemseo.utils.python_compatibility:Final"
       ]
     - id: reorder-python-imports
       name: reorder python imports out of src
       exclude: ^src
       args: [
-        --py37-plus,
+        --py38-plus,
         --add-import,
         "from __future__ import annotations",
-        --replace-import,
-        "typing=gemseo.utils.python_compatibility:Final"
       ]
 
 - repo: https://github.com/myint/docformatter
-  rev: v1.5.1
+  rev: v1.6.5
   hooks:
     - id: docformatter
       args: [
         --in-place,
         --wrap-summaries,
-        "89",
+        "88",
         --wrap-descriptions,
-        "89",
+        "88",
       ]
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.4.0
   hooks:
     - id: pyupgrade
-      args: [--py37-plus]
+      args: [--py38-plus]
 
 - repo: https://github.com/psf/black
-  rev: 22.12.0
+  rev: 23.3.0
   hooks:
     - id: black
 
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
     - id: flake8
       additional_dependencies:
-        - flake8-annotations==2.9.1
-        - flake8-bugbear==22.12.6
-        - flake8-docstrings==1.6.0
+        - flake8-annotations==3.0.1
+        - flake8-bugbear==23.5.9
+        - flake8-docstrings==1.7.0
         - flake8-logging-format==0.9.0
         - flake8-print==5.0.0
         - pep8-naming==0.13.3
 
 - repo: https://github.com/commitizen-tools/commitizen
-  rev: v2.39.1
+  rev: 3.2.2
   hooks:
     - id: commitizen
       stages: [commit-msg]
 
+- repo: https://github.com/kynan/nbstripout
+  rev: 0.6.1
+  hooks:
+    - id: nbstripout
+
+- repo: https://github.com/nbQA-dev/nbQA
+  rev: 1.7.0
+  hooks:
+    - id: nbqa-black
+    - id: nbqa-pyupgrade
+      args: [ "--py38-plus" ]
+    - id: nbqa-autopep8
+
 - repo: https://github.com/Lucas-C/pre-commit-hooks
-  rev: v1.3.1
+  rev: v1.5.1
   hooks:
     - id: insert-license
       name: insert LGPL license
       exclude: ^doc_src
       files: \.py$
       args:
         - --license-filepath
```

### Comparing `gemseo-mma-1.0.0/.pylintrc` & `gemseo-mma-2.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `gemseo-mma-1.0.0/CHANGELOG.rst` & `gemseo-mma-2.0.0/CHANGELOG.rst`

 * *Files 19% similar despite different names*

```diff
@@ -21,11 +21,28 @@
 All notable changes of this project will be documented here.
 
 The format is based on
 `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_
 and this project adheres to
 `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
+
+Version 2.0.0 (June 2023)
+*************************
+
+Update to GEMSEO 5.
+
+Fixed
+-----
+- A bug on the option settings was solved.
+
+Changed
+-------
+- The ``ctol_abs`` option was removed, this was anyway not used.
+- The attributes and option names were changed to be more explicit.
+- The solver attributes are made private.
+
+
 Version 1.0.0 (February 2023)
 *****************************
 
 First release.
```

### Comparing `gemseo-mma-1.0.0/CREDITS.rst` & `gemseo-mma-2.0.0/CREDITS.rst`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     Python Software License
 
 Internal Dependencies
 ---------------------
 
 GEMSEO-mma source code includes software with compatible licenses that are listed below.
 
+`MMA <https://github.com/arjendeetman/GCMMA-MMA-Python>`_
+    GPL-3.0 License
+
 External application
 --------------------
 
 Some external applications are used by GEMSEO-mma,
 but not linked with the application,
 for documentation generation,
 training or example purposes.
@@ -61,14 +64,11 @@
 
 `setuptools <https://setuptools.readthedocs.io/>`_
     MIT
 
 `setuptools_scm <https://github.com/pypa/setuptools_scm/>`_
     MIT
 
-`MMA <https://github.com/arjendeetman/GCMMA-MMA-Python>`_
-    GPL-3.0 License
-
 Resources
 ---------
 
 Some icons and fonts are used by GEMSEO-mma or its documentation.
```

### Comparing `gemseo-mma-1.0.0/LICENSE.txt` & `gemseo-mma-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemseo-mma-1.0.0/LICENSES/GPLv3.txt` & `gemseo-mma-2.0.0/LICENSES/GPLv3.txt`

 * *Files identical despite different names*

### Comparing `gemseo-mma-1.0.0/LICENSES/LGPLv3.txt` & `gemseo-mma-2.0.0/LICENSES/LGPLv3.txt`

 * *Files identical despite different names*

### Comparing `gemseo-mma-1.0.0/LICENSES/headers/BSD-0-Clause.txt` & `gemseo-mma-2.0.0/LICENSES/headers/BSD-0-Clause.txt`

 * *Files identical despite different names*

### Comparing `gemseo-mma-1.0.0/LICENSES/headers/LGPL-3.0.txt` & `gemseo-mma-2.0.0/LICENSES/headers/LGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gemseo-mma-1.0.0/PKG-INFO` & `gemseo-mma-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-mma
-Version: 1.0.0
+Version: 2.0.0
 Summary: A gemseo wrapper of Python version of Method of Moving Asymptothes in the implementation of Arjen Deetman.
 Home-page: https://gitlab.com/gemseo
 Author: Simone Coniglio
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-mma
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-mma/-/issues
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
@@ -81,19 +80,19 @@
 
 * max_optimization_step: Also known as ``move`` parameter control the maximum distance of the next iteration design point from the current one. Reducing this parameter avoid divergence for highly non-linear problems.
 
 * min_asymptote_distance: The minimum distance of the asymptotes from the current design variable value.
 
 * max_asymptote_distance: The maximum distance of the asymptotes from the current design variable value.
 
-* asyinit: The initial asymptote distance from the current design variable value.
+* initial_asymptotes_distance: The initial asymptote distance from the current design variable value.
 
-* asyincr The incremental factor of asymptote distance from the current design variable value for successful iterations.
+* asymptotes_distance_amplification_coefficient The incremental factor of asymptote distance from the current design variable value for successful iterations.
 
-* asydecr: The decremental factor of asymptote distance from the current design variable value for successful iterations.
+* asymptotes_distance_reduction_coefficient: The decremental factor of asymptote distance from the current design variable value for successful iterations.
 
 * conv_tol: If provided control all other convergence tolerances.
 
 The shortest is the distance of the asymptotes, the highest is the convexity of the local approximation.
 It's another mechanism to control the optimization step.
 You can find an example in examples/analytic_example.ipynb.
```

### Comparing `gemseo-mma-1.0.0/README.rst` & `gemseo-mma-2.0.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -54,19 +54,19 @@
 
 * max_optimization_step: Also known as ``move`` parameter control the maximum distance of the next iteration design point from the current one. Reducing this parameter avoid divergence for highly non-linear problems.
 
 * min_asymptote_distance: The minimum distance of the asymptotes from the current design variable value.
 
 * max_asymptote_distance: The maximum distance of the asymptotes from the current design variable value.
 
-* asyinit: The initial asymptote distance from the current design variable value.
+* initial_asymptotes_distance: The initial asymptote distance from the current design variable value.
 
-* asyincr The incremental factor of asymptote distance from the current design variable value for successful iterations.
+* asymptotes_distance_amplification_coefficient The incremental factor of asymptote distance from the current design variable value for successful iterations.
 
-* asydecr: The decremental factor of asymptote distance from the current design variable value for successful iterations.
+* asymptotes_distance_reduction_coefficient: The decremental factor of asymptote distance from the current design variable value for successful iterations.
 
 * conv_tol: If provided control all other convergence tolerances.
 
 The shortest is the distance of the asymptotes, the highest is the convexity of the local approximation.
 It's another mechanism to control the optimization step.
 You can find an example in examples/analytic_example.ipynb.
```

### Comparing `gemseo-mma-1.0.0/pyproject.toml` & `gemseo-mma-2.0.0/pyproject.toml`

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

### Comparing `gemseo-mma-1.0.0/requirements/dist.txt` & `gemseo-mma-2.0.0/requirements/dist.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --resolver=backtracking requirements/dist.in
+#    pip-compile requirements/dist.in
 #
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-build==0.9.0
+build==0.10.0
     # via -r requirements/dist.in
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
-commonmark==0.9.1
-    # via rich
-cryptography==38.0.4
+cryptography==40.0.2
     # via secretstorage
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 idna==3.4
     # via requests
-importlib-metadata==5.2.0
+importlib-metadata==6.6.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 keyring==23.13.1
     # via twine
-more-itertools==9.0.0
+markdown-it-py==2.2.0
+    # via rich
+mdurl==0.1.2
+    # via markdown-it-py
+more-itertools==9.1.0
     # via jaraco-classes
-packaging==22.0
+packaging==23.1
     # via build
-pep517==0.13.0
-    # via build
-pkginfo==1.9.2
+pkginfo==1.9.6
     # via twine
 pycparser==2.21
     # via cffi
-pygments==2.13.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
+pyproject-hooks==1.0.0
+    # via build
 readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.6.0
+rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 tomli==2.0.1
     # via
     #   build
-    #   pep517
+    #   pyproject-hooks
 twine==4.0.2
     # via -r requirements/dist.in
-urllib3==1.26.13
+urllib3==2.0.2
     # via
     #   requests
     #   twine
 webencodings==0.5.1
     # via bleach
-zipp==3.11.0
+zipp==3.15.0
     # via importlib-metadata
```

### Comparing `gemseo-mma-1.0.0/requirements/test-python3.10.txt` & `gemseo-mma-2.0.0/requirements/test-python3.8.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,116 +1,120 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.8.txt
 #
-attrs==22.2.0
-    # via pytest
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
-covdefaults==2.2.2
+covdefaults==2.3.0
     # via gemseo-mma (setup.py)
-coverage[toml]==7.1.0
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 docstring-inheritance==1.0.0
     # via gemseo
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
-gemseo==4.3.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-mma (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.7.0
+h5py==3.8.0
     # via gemseo
 idna==3.4
     # via requests
+importlib-resources==5.12.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.6.2
+matplotlib==3.7.1
     # via gemseo
-networkx==2.8.8
+networkx==3.1
     # via gemseo
-numpy==1.23.4
+numpy==1.24.3
     # via
     #   contourpy
     #   gemseo
     #   gemseo-mma (setup.py)
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
-pandas==1.5.1
+pandas==2.0.0
     # via gemseo
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.2.1
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-mma (setup.py)
     #   pytest-cov
     #   pytest-xdist
 pytest-cov==4.0.0
     # via gemseo-mma (setup.py)
-pytest-xdist==3.2.0
+pytest-xdist==3.3.0
     # via gemseo-mma (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.2
+requests==2.30.0
     # via gemseo
-scipy==1.9.1
+scipy==1.10.1
     # via
     #   gemseo
     #   gemseo-mma (setup.py)
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via gemseo
-urllib3==1.26.14
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-mma-1.0.0/requirements/test-python3.7.txt` & `gemseo-mma-2.0.0/requirements/test-python3.10.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,125 +1,116 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.7.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
 #
-attrs==22.2.0
-    # via pytest
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
-covdefaults==2.2.2
+contourpy==1.0.7
+    # via matplotlib
+covdefaults==2.3.0
     # via gemseo-mma (setup.py)
-coverage[toml]==7.1.0
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 docstring-inheritance==1.0.0
     # via gemseo
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
-gemseo==4.3.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-mma (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.7.0
+h5py==3.8.0
     # via gemseo
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
-    # via
-    #   gemseo
-    #   pluggy
-    #   pytest
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.5.3
+matplotlib==3.7.1
     # via gemseo
-networkx==2.6.3
+networkx==3.1
     # via gemseo
-numpy==1.21.6
+numpy==1.24.3
     # via
+    #   contourpy
     #   gemseo
     #   gemseo-mma (setup.py)
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
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.2.1
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-mma (setup.py)
     #   pytest-cov
     #   pytest-xdist
 pytest-cov==4.0.0
     # via gemseo-mma (setup.py)
-pytest-xdist==3.2.0
+pytest-xdist==3.3.0
     # via gemseo-mma (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.2
+requests==2.30.0
     # via gemseo
-scipy==1.7.3
+scipy==1.10.1
     # via
     #   gemseo
     #   gemseo-mma (setup.py)
-singledispatchmethod==1.0
-    # via gemseo
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.4.0
-    # via
-    #   gemseo
-    #   importlib-metadata
-    #   kiwisolver
-urllib3==1.26.14
+typing-extensions==4.5.0
+    # via gemseo
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
-zipp==3.12.1
-    # via importlib-metadata
```

### Comparing `gemseo-mma-1.0.0/requirements/test-python3.8.txt` & `gemseo-mma-2.0.0/requirements/test-python3.9.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,116 +1,120 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.8.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.9.txt
 #
-attrs==22.2.0
-    # via pytest
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
-covdefaults==2.2.2
+covdefaults==2.3.0
     # via gemseo-mma (setup.py)
-coverage[toml]==7.1.0
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 docstring-inheritance==1.0.0
     # via gemseo
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
-gemseo==4.3.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-mma (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.7.0
+h5py==3.8.0
     # via gemseo
 idna==3.4
     # via requests
+importlib-resources==5.12.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.6.2
+matplotlib==3.7.1
     # via gemseo
-networkx==2.8.8
+networkx==3.1
     # via gemseo
-numpy==1.23.4
+numpy==1.24.3
     # via
     #   contourpy
     #   gemseo
     #   gemseo-mma (setup.py)
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
-pandas==1.5.1
+pandas==2.0.0
     # via gemseo
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.2.1
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-mma (setup.py)
     #   pytest-cov
     #   pytest-xdist
 pytest-cov==4.0.0
     # via gemseo-mma (setup.py)
-pytest-xdist==3.2.0
+pytest-xdist==3.3.0
     # via gemseo-mma (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.2
+requests==2.30.0
     # via gemseo
-scipy==1.9.1
+scipy==1.10.1
     # via
     #   gemseo
     #   gemseo-mma (setup.py)
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via gemseo
-urllib3==1.26.14
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-mma-1.0.0/setup.cfg` & `gemseo-mma-2.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -17,27 +17,26 @@
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
-	gemseo >=4
+	gemseo >=5
 	numpy
 	scipy
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
@@ -65,17 +64,19 @@
 ignore = 
 	E501
 	D105
 	E203
 	W503
 	ANN101
 	ANN102
+	ANN401
 select = ANN,B,C,D,E,F,G,N,T,W,B950
 max-line-length = 88
 docstring-convention = google
 per-file-ignores = 
-	tests/*.py:D100,ANN
+	tests/*.py: D100,D104,ANN
+	doc_src/*.py: D,T201
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gemseo-mma-1.0.0/setup.py` & `gemseo-mma-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `gemseo-mma-1.0.0/src/gemseo_mma/__init__.py` & `gemseo-mma-2.0.0/src/gemseo_mma/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mma-1.0.0/src/gemseo_mma/opt/__init__.py` & `gemseo-mma-2.0.0/src/gemseo_mma/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mma-1.0.0/src/gemseo_mma/opt/core/__init__.py` & `gemseo-mma-2.0.0/src/gemseo_mma/opt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mma-1.0.0/src/gemseo_mma/opt/core/mma.py` & `gemseo-mma-2.0.0/src/gemseo_mma/opt/core/mma.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """GCMMA-MMA-Python. This file is part of GCMMA-MMA-Python.
 
-GCMMA-MMA-Python is licensed
-under the terms of GNU General Public License as published by the Free Software
-Foundation. For more information and the LICENSE file, see `https://github.com/
+GCMMA-MMA-Python is licensed under the terms of GNU General Public License as published
+by the Free Software Foundation. For more information and the LICENSE file, see `
+https://github.com/
 arjendeetman/GCMMA-MMA-Python <https://github.com/arjendeetman/GCMMA-MMA-Python>`_
 . The original work is written by
 Krister Svanberg in MATLAB. This is the python version of the code written Arjen
 Deetman. version 09-11-2019.
 
 MMA optimizer.
```

### Comparing `gemseo-mma-1.0.0/src/gemseo_mma/opt/core/mma_optimizer.py` & `gemseo-mma-2.0.0/src/gemseo_mma/opt/core/mma_optimizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 
 
 class MMAOptimizer:
     """Method of Moving Asymptotes optimizer class.
 
     This class run an optimization algorithm to solve Non-linear Optimization problems
     with constraints. The objective function and the constraints and their gradients are
-    needed for the optimization algorithm. The original implementation the next iteration
-    candidate is computed using mmasub function adapted from
-    `https://github.com/arjendeetman/GCMMA-MMA-Python
+    needed for the optimization algorithm. The original implementation the next
+    iteration candidate is computed using mmasub function adapted from `
+    https://github.com/arjendeetman/GCMMA-MMA-Python
     <https://github.com/arjendeetman/GCMMA-MMA-Python>`_ . The external and internal move
     limit can be tuned to control minimum and maximum local approximation convexity. The
     max_optimization_step parameter can be used to control the optimization step. To
     avoid solver divergence in the case of highly non-linear problems one should use
     smaller values of the max_optimization_step, max_asymptote_distance and
     min_asymptote_distance.
     """
@@ -54,108 +54,114 @@
     __DEFAULT_MAXITER = 1000
     __DEFAULT_KKT_TOL = 1e-2
     __EMPTY_STRING = ""
     __DEFAULT_ASYINIT = 0.5
     __DEFAULT_ASYINCR = 1.2
     __DEFAULT_ASYDECR = 0.7
 
-    max_optimization_step: float
+    __max_optimization_step: float
     """The maximum optimization step."""
-    min_asymptote_distance: float
+    __min_asymptote_distance: float
     """The minimum distance of the asymptotes from the current design variable value."""
-    max_asymptote_distance: float
+    __max_asymptote_distance: float
     """The maximum distance of the asymptotes from the current design variable value."""
-    ftol_abs: float
+    __ftol_abs: float
     """The absolute tolerance on the objective function."""
-    ftol_rel: float
+    __ftol_rel: float
     """The relative tolerance on the objective function."""
-    xtol_rel: float
+    __xtol_rel: float
     """The relative tolerance on the design parameters."""
-    xtol_abs: float
+    __xtol_abs: float
     """The absolute tolerance on the design parameters."""
-    tol: float
+    __tol: float
     """KKT residual norm tolerance."""
-    max_iter: int
+    __max_iter: int
     """The maximum number of iterations."""
-    normalize_design_space: bool
+    __normalize_design_space: bool
     """Whether to normalize the design space."""
-    message: str
+    __message: str
     """The message of the optimization problem."""
-    problem: OptimizationProblem
+    __problem: OptimizationProblem
     """The GEMSEO OptimizationProblem to be solved."""
-    asyinit: float
+    __initial_asymptotes_distance: float
     """The initial asymptotes distance from the current design variable value."""
-    asyincr: float
-    """The incremental factor for successful iterations."""
-    asydecr: float
+    __asymptotes_distance_amplification_coefficient: float
+    """The amplification factor for successful iterations."""
+    __asymptotes_distance_reduction_coefficient: float
     """The decremental factor for unsuccessful iterations."""
 
     def __init__(self, problem: OptimizationProblem) -> None:
         """Constructor."""
-        self.problem = problem
-        self.message = self.__EMPTY_STRING
-        self.normalize_design_space = self.__DEFAULT_NORMALIZE_DESIGN_SPACE
-        self.max_iter = self.__DEFAULT_MAXITER
-        self.tol = self.__DEFAULT_KKT_TOL
-        self.xtol_abs = self.__DEFAULT_TOLERANCE
-        self.xtol_rel = self.__DEFAULT_TOLERANCE
-        self.ftol_rel = self.__DEFAULT_TOLERANCE
-        self.ftol_abs = self.__DEFAULT_TOLERANCE
-        self.ineq_tolerance = self.__DEFAULT_TOLERANCE
-        self.max_asymptote_distance = self.__DEFAULT_MAX_DISTANCE
-        self.min_asymptote_distance = self.__DEFAULT_MIN_DISTANCE
-        self.max_optimization_step = self.__DEFAULT_MAX_OPTIM_STEP
-        self.asyinit = self.__DEFAULT_ASYINIT
-        self.asyincr = self.__DEFAULT_ASYINCR
-        self.asydecr = self.__DEFAULT_ASYDECR
+        self.__problem = problem
+        self.__message = self.__EMPTY_STRING
+        self.__normalize_design_space = self.__DEFAULT_NORMALIZE_DESIGN_SPACE
+        self.__max_iter = self.__DEFAULT_MAXITER
+        self.__tol = self.__DEFAULT_KKT_TOL
+        self.__xtol_abs = self.__DEFAULT_TOLERANCE
+        self.__xtol_rel = self.__DEFAULT_TOLERANCE
+        self.__ftol_rel = self.__DEFAULT_TOLERANCE
+        self.__ftol_abs = self.__DEFAULT_TOLERANCE
+        self.__ineq_tolerance = self.__DEFAULT_TOLERANCE
+        self.__max_asymptote_distance = self.__DEFAULT_MAX_DISTANCE
+        self.__min_asymptote_distance = self.__DEFAULT_MIN_DISTANCE
+        self.__max_optimization_step = self.__DEFAULT_MAX_OPTIM_STEP
+        self.__initial_asymptotes_distance = self.__DEFAULT_ASYINIT
+        self.__asymptotes_distance_amplification_coefficient = self.__DEFAULT_ASYINCR
+        self.__asymptotes_distance_reduction_coefficient = self.__DEFAULT_ASYDECR
 
     def optimize(self, **options: bool | int | float) -> tuple[str, int]:
         """Optimize the problem.
 
         Args:
             **options: The optimization problem options.
 
         Returns:
             The optimization solver message and final status.
         """
-        self.normalize_design_space = options.get(
+        self.__normalize_design_space = options.get(
             "normalize_design_space", self.__DEFAULT_NORMALIZE_DESIGN_SPACE
         )
-        self.max_iter = options.get("max_iter", self.__DEFAULT_MAXITER)
-        self.tol = options.get("tol", self.__DEFAULT_TOLERANCE)
-        self.xtol_abs = options.get("xtol_abs", self.__DEFAULT_TOLERANCE)
-        self.xtol_rel = options.get("xtol_rel", self.__DEFAULT_TOLERANCE)
-        self.ftol_rel = options.get("ftol_rel", self.__DEFAULT_TOLERANCE)
-        self.ftol_abs = options.get("ftol_abs", self.__DEFAULT_TOLERANCE)
-        self.max_asymptote_distance = options.get(
+        self.__max_iter = options.get("max_iter", self.__DEFAULT_MAXITER)
+        self.__tol = options.get("tol", self.__DEFAULT_TOLERANCE)
+        self.__xtol_abs = options.get("xtol_abs", self.__DEFAULT_TOLERANCE)
+        self.__xtol_rel = options.get("xtol_rel", self.__DEFAULT_TOLERANCE)
+        self.__ftol_rel = options.get("ftol_rel", self.__DEFAULT_TOLERANCE)
+        self.__ftol_abs = options.get("ftol_abs", self.__DEFAULT_TOLERANCE)
+        self.__max_asymptote_distance = options.get(
             "max_asymptote_distance", self.__DEFAULT_MAX_DISTANCE
         )
-        self.min_asymptote_distance = options.get(
+        self.__min_asymptote_distance = options.get(
             "min_asymptote_distance", self.__DEFAULT_MIN_DISTANCE
         )
-        self.max_optimization_step = options.get(
+        self.__max_optimization_step = options.get(
             "max_optimization_step", self.__DEFAULT_MAX_OPTIM_STEP
         )
-        self.max_optimization_step = options.get("asyinit", self.__DEFAULT_ASYINIT)
-        self.max_optimization_step = options.get("asyincr", self.__DEFAULT_ASYINCR)
-        self.max_optimization_step = options.get("asydecr", self.__DEFAULT_ASYDECR)
+        self.__initial_asymptotes_distance = options.get(
+            "initial_asymptotes_distance", self.__DEFAULT_ASYINIT
+        )
+        self.__asymptotes_distance_amplification_coefficient = options.get(
+            "asymptotes_distance_amplification_coefficient", self.__DEFAULT_ASYINCR
+        )
+        self.__asymptotes_distance_reduction_coefficient = options.get(
+            "asymptotes_distance_reduction_coefficient", self.__DEFAULT_ASYDECR
+        )
 
         # initialize database
-        if not self.normalize_design_space:
-            x0 = self.problem.design_space.get_current_value()
+        if not self.__normalize_design_space:
+            x0 = self.__problem.design_space.get_current_value()
         else:
-            x0 = self.problem.design_space.normalize_vect(
-                self.problem.design_space.get_current_value()
+            x0 = self.__problem.design_space.normalize_vect(
+                self.__problem.design_space.get_current_value()
             )
 
         # launch optim
         xopt = self.iterate(x0)[0]
-        self.problem.design_space.set_current_value(xopt)
+        self.__problem.design_space.set_current_value(xopt)
 
-        return self.message, 0
+        return self.__message, 0
 
     def iterate(self, x0: ndarray) -> tuple[ndarray, ndarray]:
         """Iterate until convergence from the starting guess.
 
         Args:
             x0: The starting guess design point.
 
@@ -163,28 +169,32 @@
             The optimum design point and objective value.
         """
         n = len(x0)
         eeen = np.ones((n, 1))
         xval = np.reshape(x0, eeen.shape)
         xold1 = xval.copy()
         xold2 = xval.copy()
-        if not self.normalize_design_space:
-            xmin = np.reshape(self.problem.design_space.get_lower_bounds(), eeen.shape)
-            xmax = np.reshape(self.problem.design_space.get_upper_bounds(), eeen.shape)
+        if not self.__normalize_design_space:
+            xmin = np.reshape(
+                self.__problem.design_space.get_lower_bounds(), eeen.shape
+            )
+            xmax = np.reshape(
+                self.__problem.design_space.get_upper_bounds(), eeen.shape
+            )
         else:
             xmin = 0 * eeen
             xmax = eeen
         low = xmin.copy()
         upp = xmax.copy()
 
         a0 = 1
 
         outeriter = 0
-        maxoutit = self.max_iter
-        kkttol = self.tol
+        maxoutit = self.__max_iter
+        kkttol = self.__tol
         (
             f0val,
             df0dx,
             fval,
             dfdx,
         ) = self.__get_objective_and_constraints_with_gradients(xval.flatten())
         m = len(fval)
@@ -201,19 +211,22 @@
         change_f = 10
         change_x = 10
         change_relative_f = 10
         change_relative_x = 10
         outit = 0
         while (
             (kktnorm > kkttol)
-            and (change_x > self.xtol_abs)
-            and (change_relative_x > self.xtol_rel)
-            and (change_relative_f > self.ftol_rel)
-            and (change_f > self.ftol_abs)
-            or (any(fval > self.problem.ineq_tolerance) and change_fc > self.ftol_abs)
+            and (change_x > self.__xtol_abs)
+            and (change_relative_x > self.__xtol_rel)
+            and (change_relative_f > self.__ftol_rel)
+            and (change_f > self.__ftol_abs)
+            or (
+                any(fval > self.__problem.ineq_tolerance)
+                and change_fc > self.__ftol_abs
+            )
         ) and (outit < maxoutit):
             outit += 1
             outeriter += 1
 
             (
                 xmma,
                 ymma,
@@ -241,20 +254,20 @@
                 dfdx,
                 low,
                 upp,
                 a0,
                 a,
                 c,
                 d,
-                self.max_optimization_step,
-                self.max_asymptote_distance,
-                self.min_asymptote_distance,
-                self.asyinit,
-                self.asyincr,
-                self.asydecr,
+                self.__max_optimization_step,
+                self.__max_asymptote_distance,
+                self.__min_asymptote_distance,
+                self.__initial_asymptotes_distance,
+                self.__asymptotes_distance_amplification_coefficient,
+                self.__asymptotes_distance_reduction_coefficient,
             )
             (
                 f0valnew,
                 df0dxnew,
                 fvalnew,
                 dfdxnew,
             ) = self.__get_objective_and_constraints_with_gradients(xmma.flatten())
@@ -290,43 +303,43 @@
                 dfdx,
                 a0,
                 a,
                 c,
                 d,
             )
 
-        if self.normalize_design_space:
-            xopt = self.problem.design_space.unnormalize_vect(xval.flatten())
+        if self.__normalize_design_space:
+            xopt = self.__problem.design_space.unnormalize_vect(xval.flatten())
         else:
             xopt = xval.flatten()
 
         LOGGER.info("END OF MMA ALGORITHM")
         if kktnorm <= kkttol:
-            self.message = "KKT norm criteria met"
+            self.__message = "KKT norm criteria met"
         else:
-            self.message = "change criteria met"
+            self.__message = "change criteria met"
         return xopt, f0val
 
     def __get_objective_and_constraints_with_gradients(
         self, xval: ndarray
     ) -> tuple[ndarray, ndarray, ndarray, ndarray]:
         """Compute the objective and constraints with their gradients.
 
         Args:
             xval: The current design value.
 
         Returns:
             The objective and constraint value in the provided design point and their
                 gradients.
         """
-        f0val = self.problem.objective(xval)
-        df0dx = self.problem.objective.jac(xval)
+        f0val = self.__problem.objective(xval)
+        df0dx = self.__problem.objective.jac(xval)
         df0dx = np.reshape(df0dx, (df0dx.size, 1))
         constraint_list = []
         constraint_jac_list = []
-        for constraint in self.problem.constraints:
+        for constraint in self.__problem.constraints:
             constraint_list.append(constraint(xval).flatten())
             constraint_jac_list.append(atleast_2d(constraint.jac(xval)))
         fval = np.concatenate(constraint_list)
         fval = np.reshape(fval, (fval.size, 1))
         dfdx = np.concatenate(constraint_jac_list, axis=0)
         return f0val, df0dx, fval, dfdx
```

### Comparing `gemseo-mma-1.0.0/src/gemseo_mma/opt/lib_mma.py` & `gemseo-mma-2.0.0/src/gemseo_mma/opt/lib_mma.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """MMA optimizer library."""
 from __future__ import annotations
 
 from typing import Any
 
-from gemseo.algos.opt.opt_lib import OptimizationAlgorithmDescription
-from gemseo.algos.opt.opt_lib import OptimizationLibrary
+from gemseo.algos.opt.optimization_library import OptimizationAlgorithmDescription
+from gemseo.algos.opt.optimization_library import OptimizationLibrary
 from gemseo.algos.opt_result import OptimizationResult
 
 from gemseo_mma.opt.core.mma_optimizer import MMAOptimizer
 
 
 class MMASvanberg(OptimizationLibrary):
     """Svanberg Method of Moving Asymptotes optimization library."""
@@ -46,61 +46,52 @@
         }
 
     def _get_options(
         self,
         max_iter: int = 1000,
         ftol_abs: float = 1e-14,
         xtol_abs: float = 1e-14,
-        max_time: float = 0.0,
         ftol_rel: float = 1e-8,
         xtol_rel: float = 1e-8,
-        ctol_abs: float | None = None,
-        stopval: float | None = None,
         eq_tolerance: float = 1e-2,
-        ineq_tolerance: float = 1e-4,
         tol: float = 1e-2,
-        conv_tol: float = None,
+        conv_tol: float | None = None,
         max_optimization_step: float = 0.1,
         max_asymptote_distance: float = 10.0,
         min_asymptote_distance: float = 0.01,
-        asyinit: float = 0.5,
-        asyincr: float = 1.2,
-        asydecr: float = 0.7,
-        normalize_design_space: bool = False,
+        initial_asymptotes_distance: float = 0.5,
+        asymptotes_distance_amplification_coefficient: float = 1.2,
+        asymptotes_distance_reduction_coefficient: float = 0.7,
+        **kwargs: Any,
     ) -> dict[str, Any]:
         r"""Sets the options.
 
         Args:
             ftol_abs: The absolute tolerance on the objective function.
             xtol_abs: The absolute tolerance on the design parameters.
-            max_time: The maximum runtime in seconds. The value 0 means no runtime
-                limit.
             max_iter: The maximum number of iterations.
             ftol_rel: The relative tolerance on the objective function.
             xtol_rel: The relative tolerance on the design parameters.
-            ctol_abs: The absolute tolerance on the constraints.
-            stopval: The objective value at which the optimization will stop.
-                Stop minimizing when an objective value :math:`\leq` stopval is
-                found, or stop maximizing when a value :math:`\geq` stopval
-                is found. If None, this termination condition will not be active.
             normalize_design_space: If True, normalize the design variables between 0
                 and 1.
             eq_tolerance: The tolerance on the equality constraints.
-            ineq_tolerance: The tolerance on the inequality constraints.
             tol: tolerance of convergence used in MMA to be compared with kkt residual.
             conv_tol: If provided control all other convergence tolerances.
             max_optimization_step: The maximum optimization step.
             max_asymptote_distance: The maximum distance of the asymptotes from the
                 current design variable value.
             min_asymptote_distance: The minimum distance of the asymptotes from the
                 current design variable value.
-            asyinit: The initial asymptotes distance from the current design variable
-                value.
-            asyincr: The incremental factor for successful iterations.
-            asydecr: The decremental factor for unsuccessful iterations.
+            initial_asymptotes_distance: The initial asymptotes distance from the
+                current design variable value.
+            asymptotes_distance_amplification_coefficient: The amplification factor
+                for successful iterations.
+            asymptotes_distance_reduction_coefficient: The decremental factor for
+                unsuccessful iterations.
+            **kwargs: The other options.
 
         Returns:
             The converted options.
 
         Raises:
             ValueError: If an option is invalid.
         """
@@ -108,37 +99,30 @@
             ftol_rel = conv_tol
             ftol_abs = conv_tol
             xtol_rel = conv_tol
             xtol_abs = conv_tol
         else:
             conv_tol = min(ftol_rel, ftol_abs, xtol_rel, xtol_abs)
 
-        if ctol_abs is None:
-            ctol_abs = conv_tol
-
         return self._process_options(
             max_iter=max_iter,
             tol=tol,
-            normalize_design_space=normalize_design_space,
             conv_tol=conv_tol,
             max_optimization_step=max_optimization_step,
             max_asymptote_distance=max_asymptote_distance,
             min_asymptote_distance=min_asymptote_distance,
-            asyinit=asyinit,
-            asyincr=asyincr,
-            asydecr=asydecr,
+            initial_asymptotes_distance=initial_asymptotes_distance,
+            asymptotes_distance_amplification_coefficient=asymptotes_distance_amplification_coefficient,
+            asymptotes_distance_reduction_coefficient=asymptotes_distance_reduction_coefficient,
             ftol_rel=ftol_rel,
             ftol_abs=ftol_abs,
             xtol_rel=xtol_rel,
             xtol_abs=xtol_abs,
-            max_time=max_time,
-            stopval=stopval,
             eq_tolerance=eq_tolerance,
-            ineq_tolerance=ineq_tolerance,
-            ctol_abs=ctol_abs,
+            **kwargs,
         )
 
     def _run(self, **options: float | int | str) -> OptimizationResult:
         """Runs the algorithm, to be overloaded by subclasses.
 
         Args:
             **options: The options dict for the algorithm,
@@ -170,35 +154,41 @@
         if len(problem.database) == 0:
             return OptimizationResult(
                 optimizer_name=self.algo_name,
                 message=message,
                 status=status,
                 n_obj_call=0,
             )
-        x_0 = problem.database.get_x_by_iter(0)
+        x_0 = problem.database.get_x_vect(1)
         # get last point as optimum
-        x_opt = problem.database.get_x_by_iter(-1)
-        is_feas, _violation = problem.get_violation_criteria(x_opt)
-        f_opt = problem.database.get_f_of_x(fname=problem.objective.name, x_vect=x_opt)
+        x_opt = problem.database.get_x_vect(-1)
+        is_feas, _ = problem.get_violation_criteria(x_opt)
+        f_opt = problem.database.get_function_value(
+            function_name=problem.objective.name, x_vect_or_iteration=x_opt
+        )
         c_opt = {
-            cont.name: problem.database.get_f_of_x(fname=cont.name, x_vect=x_opt)
+            cont.name: problem.database.get_function_value(
+                function_name=cont.name, x_vect_or_iteration=x_opt
+            )
             for cont in problem.constraints
         }
         c_opt_grad = {
-            cont.name: problem.database.get_func_grad_history(funcname=cont.name)[-1]
+            cont.name: problem.database.get_gradient_history(function_name=cont.name)[
+                -1
+            ]
             for cont in problem.constraints
         }
         # f_opt, x_opt, is_feas, c_opt, c_opt_grad = problem.get_optimum()
         if f_opt is not None and not problem.minimize_objective:
             f_opt = -f_opt
         return OptimizationResult(
             x_0=x_0,
             x_opt=x_opt,
             f_opt=f_opt,
             optimizer_name=self.algo_name,
             message=message,
             status=status,
             n_obj_call=problem.objective.n_calls,
             is_feasible=is_feas,
-            constraints_values=c_opt,
+            constraint_values=c_opt,
             constraints_grad=c_opt_grad,
         )
```

### Comparing `gemseo-mma-1.0.0/src/gemseo_mma.egg-info/PKG-INFO` & `gemseo-mma-2.0.0/src/gemseo_mma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-mma
-Version: 1.0.0
+Version: 2.0.0
 Summary: A gemseo wrapper of Python version of Method of Moving Asymptothes in the implementation of Arjen Deetman.
 Home-page: https://gitlab.com/gemseo
 Author: Simone Coniglio
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-mma
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-mma/-/issues
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
@@ -81,19 +80,19 @@
 
 * max_optimization_step: Also known as ``move`` parameter control the maximum distance of the next iteration design point from the current one. Reducing this parameter avoid divergence for highly non-linear problems.
 
 * min_asymptote_distance: The minimum distance of the asymptotes from the current design variable value.
 
 * max_asymptote_distance: The maximum distance of the asymptotes from the current design variable value.
 
-* asyinit: The initial asymptote distance from the current design variable value.
+* initial_asymptotes_distance: The initial asymptote distance from the current design variable value.
 
-* asyincr The incremental factor of asymptote distance from the current design variable value for successful iterations.
+* asymptotes_distance_amplification_coefficient The incremental factor of asymptote distance from the current design variable value for successful iterations.
 
-* asydecr: The decremental factor of asymptote distance from the current design variable value for successful iterations.
+* asymptotes_distance_reduction_coefficient: The decremental factor of asymptote distance from the current design variable value for successful iterations.
 
 * conv_tol: If provided control all other convergence tolerances.
 
 The shortest is the distance of the asymptotes, the highest is the convexity of the local approximation.
 It's another mechanism to control the optimization step.
 You can find an example in examples/analytic_example.ipynb.
```

### Comparing `gemseo-mma-1.0.0/src/gemseo_mma.egg-info/SOURCES.txt` & `gemseo-mma-2.0.0/src/gemseo_mma.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 LICENSES/headers/LGPL-3.0.txt
 examples/analytic_example.ipynb
 requirements/check.in
 requirements/check.txt
 requirements/dist.in
 requirements/dist.txt
 requirements/test-python3.10.txt
-requirements/test-python3.7.txt
 requirements/test-python3.8.txt
 requirements/test-python3.9.txt
 src/gemseo_mma/__init__.py
 src/gemseo_mma.egg-info/PKG-INFO
 src/gemseo_mma.egg-info/SOURCES.txt
 src/gemseo_mma.egg-info/dependency_links.txt
 src/gemseo_mma.egg-info/entry_points.txt
```

### Comparing `gemseo-mma-1.0.0/tests/test_mma_optimization.py` & `gemseo-mma-2.0.0/tests/test_mma_optimization.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 
 import pytest
+from gemseo import create_discipline
+from gemseo import create_scenario
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.opt_result import OptimizationResult
-from gemseo.api import create_discipline
-from gemseo.api import create_scenario
 from gemseo_mma.opt.core.mma_optimizer import MMAOptimizer
 from gemseo_mma.opt.lib_mma import MMASvanberg
 from numpy import array
 from numpy import ones
 
 
 @pytest.fixture(params=[0.0, 0.25, 0.1, 1.0])
@@ -134,49 +134,70 @@
     [
         {
             "max_iter": 50,
             "algo_options": {"tol": 1e-4, "normalize_design_space": True},
         },
         {
             "max_iter": 30,
-            "algo_options": {"conv_tol": 1e-16, "tol": 1e-16},
+            "algo_options": {
+                "tol": 1e-16,
+                "conv_tol": 1e-16,
+            },
         },
         {
             "max_iter": 50,
             "algo_options": {
                 "xtol_rel": 1e-7,
                 "xtol_abs": 1e-7,
                 "ftol_rel": 1e-7,
                 "ftol_abs": 1e-7,
-                "ctol_abs": 1e-7,
                 "tol": 1e-16,
             },
         },
+        {
+            "max_iter": 50,
+            "algo_options": {
+                "xtol_rel": 1e-7,
+                "xtol_abs": 1e-7,
+                "ftol_rel": 1e-7,
+                "ftol_abs": 1e-7,
+                "initial_asymptotes_distance": 0.1,
+                "asymptotes_distance_amplification_coefficient": 1.3,
+                "asymptotes_distance_reduction_coefficient": 0.6,
+            },
+        },
     ],
 )
 parametrized_algo_ineq = pytest.mark.parametrize("algo_ineq", ["MMA"])
 
 
 @parametrized_options
 @parametrized_algo_ineq
 def test_execution_with_scenario(analytical_test_2d_ineq, options, algo_ineq):
     """Test for optimization scenario execution using MMA solver."""
     opt = options.copy()
     opt["algo"] = algo_ineq
     analytical_test_2d_ineq.execute(opt)
     problem = analytical_test_2d_ineq.formulation.opt_problem
-    assert pytest.approx(problem.solution.x_opt, 1e-4) == array([0.5, 0.5])
+    assert pytest.approx(problem.solution.x_opt, abs=1e-2) == array([0.5, 0.5])
 
 
-def test_direct_execution(analytical_test_2d_ineq):
+@parametrized_options
+def test_direct_execution(analytical_test_2d_ineq, options):
     """Test for optimization problem execution using MMA solver."""
     problem = analytical_test_2d_ineq.formulation.opt_problem
     optimizer = MMAOptimizer(problem)
-    optimizer.optimize()
-    assert pytest.approx(problem.design_space.get_current_value(), 1e-4) == array(
+    optimizer.optimize(**options["algo_options"])
+    for key in options["algo_options"].keys():
+        if not "conv_tol" == key:
+            assert (
+                getattr(optimizer, "_MMAOptimizer__" + key)
+                == options["algo_options"][key]
+            )
+    assert pytest.approx(problem.design_space.get_current_value(), abs=1e-2) == array(
         [0.5, 0.5]
     )
 
 
 def test_get_optimum_from_database(analytical_test_2d_ineq):
     """Test for get_optimum_from_database call before opt problem resolution."""
     lib = MMASvanberg()
```

### Comparing `gemseo-mma-1.0.0/tox.ini` & `gemseo-mma-2.0.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     pytest {env:__COVERAGE_POSARGS:} {posargs}
 
 [testenv:check]
 description = run code formatting and checking
 basepython = python3.9
 deps = -r requirements/check.txt
 skip_install = true
-whitelist_externals =
-    pre-commit
+whitelist_externals = pre-commit
 commands =
     pre-commit install
     pre-commit run --all-files
 
 [testenv:doc]
 description = build documentation
 basepython = python3.9
@@ -66,36 +65,38 @@
 whitelist_externals = rm
 commands =
     rm -rf dist build
     python -m build
     twine check dist/*
     python setup.py check --metadata
 
-[testenv:pypi-py{37,38,39,310}]
+[testenv:pypi-py{38,39,310}]
 description = test the pypi distribution
 deps = gemseo-mma[test]
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
-whitelist_externals = pip-compile
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

