# Comparing `tmp/adafruit-circuitpython-bme680-3.4.9.tar.gz` & `tmp/adafruit-circuitpython-bme680-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bme680-3.4.9.tar", last modified: Mon Aug 22 18:37:04 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-bme680-3.5.0.tar", last modified: Mon Jun  5 20:57:14 2023, max compression
```

## Comparing `adafruit-circuitpython-bme680-3.4.9.tar` & `adafruit-circuitpython-bme680-3.5.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.270232 adafruit-circuitpython-bme680-3.4.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    20289 2022-08-22 18:36:56.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_bme680.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-08-22 18:37:04.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-08-22 18:37:04.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:37:04.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-22 18:37:04.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-22 18:37:04.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5189 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-22 18:36:56.000000 adafruit-circuitpython-bme680-3.4.9/examples/bme680_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-08-22 18:36:56.000000 adafruit-circuitpython-bme680-3.4.9/examples/bme680_spi.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-08-22 18:36:56.000000 adafruit-circuitpython-bme680-3.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.368552 adafruit-circuitpython-bme680-3.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.376552 adafruit-circuitpython-bme680-3.5.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.376552 adafruit-circuitpython-bme680-3.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.380552 adafruit-circuitpython-bme680-3.5.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    29359 2023-06-05 20:57:06.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_bme680.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.380552 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-05 20:57:14.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-05 20:57:14.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:57:14.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 20:57:14.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 20:57:14.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/contributors.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-05 20:57:06.000000 adafruit-circuitpython-bme680-3.5.0/examples/bme680_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-05 20:57:06.000000 adafruit-circuitpython-bme680-3.5.0/examples/bme680_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-05 20:57:06.000000 adafruit-circuitpython-bme680-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/setup.cfg
```

### Comparing `adafruit-circuitpython-bme680-3.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bme680-3.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.9/.gitignore` & `adafruit-circuitpython-bme680-3.5.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-bme680-3.4.9/.pre-commit-config.yaml` & `adafruit-circuitpython-bme680-3.5.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-bme680-3.4.9/.pylintrc` & `adafruit-circuitpython-bme680-3.5.0/.pylintrc`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-bme680-3.4.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bme680-3.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.9/LICENSE` & `adafruit-circuitpython-bme680-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bme680-3.5.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.9/LICENSES/MIT.txt` & `adafruit-circuitpython-bme680-3.5.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bme680-3.5.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.9/PKG-INFO` & `adafruit-circuitpython-bme680-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bme680
-Version: 3.4.9
+Version: 3.5.0
 Summary: CircuitPython driver for BME680 sensor over I2C
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BME680
 Keywords: adafruit,blinka,circuitpython,micropython,bme680,hardware,temperature,pressure,humidity,gas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bme680/badge/?version=latest
```

### Comparing `adafruit-circuitpython-bme680-3.4.9/README.rst` & `adafruit-circuitpython-bme680-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.9/adafruit_bme680.py` & `adafruit-circuitpython-bme680-3.5.0/adafruit_bme680.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # SPDX-FileCopyrightText: 2017 ladyada for Adafruit Industries
 #
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: MIT AND BSD-3-Clause
 
 # We have a lot of attributes for this complex sensor.
 # pylint: disable=too-many-instance-attributes
+# pylint: disable=no_self_use
+# pylint: disable=consider-using-f-string
 
 """
 `adafruit_bme680`
 ================================================================================
 
 CircuitPython library for BME680 temperature, pressure and humidity sensor.
 
 
 * Author(s): Limor Fried
 
+
+original Adafruit_BME680 with addition of set_gas_heater().  Other new members are private.
+
+
 Implementation Notes
 --------------------
 
 **Hardware:**
 
 * `Adafruit BME680 Temp, Humidity, Pressure and Gas Sensor <https://www.adafruit.com/product/3660>`_
 
@@ -29,30 +35,60 @@
 """
 
 import struct
 import time
 import math
 from micropython import const
 
+
+def delay_microseconds(nusec):
+    """HELP must be same as dev->delay_us"""
+    time.sleep(nusec / 1000000.0)
+
+
 try:
     # Used only for type annotations.
 
     import typing  # pylint: disable=unused-import
 
     from circuitpython_typing import ReadableBuffer
     from busio import I2C, SPI
     from digitalio import DigitalInOut
 
 except ImportError:
     pass
 
-__version__ = "3.4.9"
+__version__ = "3.5.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BME680.git"
 
 
+# garberw added begin  ===========================
+#    I2C ADDRESS/BITS/SETTINGS NEW
+#    -----------------------------------------------------------------------
+_BME68X_ENABLE_HEATER = const(0x00)
+_BME68X_DISABLE_HEATER = const(0x01)
+_BME68X_DISABLE_GAS_MEAS = const(0x00)
+_BME68X_ENABLE_GAS_MEAS_L = const(0x01)
+_BME68X_ENABLE_GAS_MEAS_H = const(0x02)
+_BME68X_SLEEP_MODE = const(0)
+_BME68X_FORCED_MODE = const(1)
+_BME68X_VARIANT_GAS_LOW = const(0x00)
+_BME68X_VARIANT_GAS_HIGH = const(0x01)
+_BME68X_HCTRL_MSK = const(0x08)
+_BME68X_HCTRL_POS = const(3)
+_BME68X_NBCONV_MSK = const(0x0F)
+_BME68X_RUN_GAS_MSK = const(0x30)
+_BME68X_RUN_GAS_POS = const(4)
+_BME68X_MODE_MSK = const(0x03)
+_BME68X_PERIOD_POLL = const(10000)
+_BME68X_REG_CTRL_GAS_0 = const(0x70)
+_BME68X_REG_CTRL_GAS_1 = const(0x71)
+
+
+# garberw added end  ===========================
 #    I2C ADDRESS/BITS/SETTINGS
 #    -----------------------------------------------------------------------
 _BME680_CHIPID = const(0x61)
 
 _BME680_REG_CHIPID = const(0xD0)
 _BME68X_REG_VARIANT = const(0xF0)
 _BME680_BME680_COEFF_ADDR1 = const(0x89)
@@ -112,14 +148,51 @@
     1000000.0,
     500000.0,
     250000.0,
     125000.0,
 )
 
 
+# garberw added begin  ===========================
+INT32 = int
+INT16 = int
+INT8 = int
+UINT32 = int
+UINT16 = int
+UINT8 = int
+
+
+def bme_set_bits(reg_data, bitname_msk, bitname_pos, data):
+    """
+    Macro to set bits
+    data2 = data << bitname_pos
+    set masked bits from data2 in reg_data
+    """
+    return (reg_data & ~bitname_msk) | ((data << bitname_pos) & bitname_msk)
+
+
+def bme_set_bits_pos_0(reg_data, bitname_msk, data):
+    """
+    Macro to set bits starting from position 0
+    set masked bits from data in reg_data
+    """
+    return (reg_data & ~bitname_msk) | (data & bitname_msk)
+
+
+class GasHeaterException(Exception):
+    """
+    Error during set_gas_heater()
+    """
+
+    def __init__(self, msg="GasHeaterException default"):
+        self.msg = msg
+        super().__init__(msg)
+
+
+# garberw added end ===========================
 def _read24(arr: ReadableBuffer) -> float:
     """Parse an unsigned 24-bit value as a floating point and return it."""
     ret = 0.0
     # print([hex(i) for i in arr])
     for b in arr:
         ret *= 256.0
         ret += float(b & 0xFF)
@@ -167,14 +240,20 @@
         self._adc_gas = None
         self._gas_range = None
         self._t_fine = None
 
         self._last_reading = 0
         self._min_refresh_time = 1 / refresh_rate
 
+        # garberw added begin ===========================
+        self._amb_temp = 25  # Copy required parameters from reference bme68x_dev struct
+        self.set_gas_heater(320, 150)  # heater 320 deg C for 150 msec
+
+        # garberw added end ===========================
+
     @property
     def pressure_oversample(self) -> int:
         """The oversampling for pressure sensor"""
         return _BME680_SAMPLERATES[self._pressure_oversample]
 
     @pressure_oversample.setter
     def pressure_oversample(self, sample_rate: int) -> None:
@@ -399,14 +478,188 @@
 
     def _read(self, register: int, length: int) -> bytearray:
         raise NotImplementedError()
 
     def _write(self, register: int, values: bytearray) -> None:
         raise NotImplementedError()
 
+    # garberw added begin ===========================
+    def set_gas_heater(self, heater_temp: UINT16, heater_time: UINT16) -> bool:
+        """
+        *  @brief  Enable and configure gas reading + heater
+        *  @param  heater_temp
+        *          Desired temperature in degrees Centigrade
+        *  @param  heater_time
+        *          Time to keep heater on in milliseconds
+        *  @return True on success, False on failure
+        """
+        if (heater_temp == 0) or (heater_time == 0):
+            return False
+        # enable = BME68X_ENABLE
+        try:
+            self._set_heatr_conf(heater_temp, heater_time)
+        except GasHeaterException:
+            return False
+        return True
+
+    def _set_heatr_conf(self, heater_temp: UINT16, heater_time: UINT16) -> None:
+        # restrict to BME68X_FORCED_MODE
+        op_mode: UINT8 = _BME68X_FORCED_MODE
+        # restrict to enable = True
+        enable: bool = True
+        nb_conv: UINT8 = 0
+        hctrl: UINT8 = _BME68X_ENABLE_HEATER
+        run_gas: UINT8 = 0
+        ctrl_gas_data_0: UINT8 = 0
+        ctrl_gas_data_1: UINT8 = 0
+        ctrl_gas_addr_0: UINT8 = _BME68X_REG_CTRL_GAS_0
+        ctrl_gas_addr_1: UINT8 = _BME68X_REG_CTRL_GAS_1
+        try:
+            self._set_op_mode(_BME68X_SLEEP_MODE)
+            self._set_conf(heater_temp, heater_time, op_mode)
+            ctrl_gas_data_0 = self._read_byte(ctrl_gas_addr_0)
+            ctrl_gas_data_1 = self._read_byte(ctrl_gas_addr_1)
+            if enable:
+                hctrl = _BME68X_ENABLE_HEATER
+                if self._chip_variant == _BME68X_VARIANT_GAS_HIGH:
+                    run_gas = _BME68X_ENABLE_GAS_MEAS_H
+                else:
+                    run_gas = _BME68X_ENABLE_GAS_MEAS_L
+            else:
+                hctrl = _BME68X_DISABLE_HEATER
+                run_gas = _BME68X_DISABLE_GAS_MEAS
+
+            ctrl_gas_data_0 = bme_set_bits(
+                ctrl_gas_data_0, _BME68X_HCTRL_MSK, _BME68X_HCTRL_POS, hctrl
+            )
+            ctrl_gas_data_1 = bme_set_bits_pos_0(
+                ctrl_gas_data_1, _BME68X_NBCONV_MSK, nb_conv
+            )
+            ctrl_gas_data_1 = bme_set_bits(
+                ctrl_gas_data_1, _BME68X_RUN_GAS_MSK, _BME68X_RUN_GAS_POS, run_gas
+            )
+            self._write(ctrl_gas_addr_0, [ctrl_gas_data_0])
+            self._write(ctrl_gas_addr_1, [ctrl_gas_data_1])
+            # HELP check this
+            self._set_op_mode(_BME68X_FORCED_MODE)
+        except GasHeaterException as exc:
+            self._set_op_mode(_BME68X_FORCED_MODE)
+            raise exc
+
+    def _set_op_mode(self, op_mode: UINT8) -> None:
+        """
+        * @brief This API is used to set the operation mode of the sensor
+        """
+        tmp_pow_mode: UINT8 = 0
+        pow_mode: UINT8 = _BME68X_FORCED_MODE
+        reg_addr: UINT8 = _BME680_REG_CTRL_MEAS
+        # Call until in sleep
+        try:
+            # was a do {} while() loop
+            while pow_mode != _BME68X_SLEEP_MODE:
+                tmp_pow_mode = self._read_byte(_BME680_REG_CTRL_MEAS)
+                # Put to sleep before changing mode
+                pow_mode = tmp_pow_mode & _BME68X_MODE_MSK
+                if pow_mode != _BME68X_SLEEP_MODE:
+                    tmp_pow_mode &= ~_BME68X_MODE_MSK  # Set to sleep
+                    self._write(reg_addr, [tmp_pow_mode])
+                    # dev->delay_us(_BME68X_PERIOD_POLL, dev->intf_ptr)  # HELP
+                    delay_microseconds(_BME68X_PERIOD_POLL)
+            # Already in sleep
+            if op_mode != _BME68X_SLEEP_MODE:
+                tmp_pow_mode = (tmp_pow_mode & ~_BME68X_MODE_MSK) | (
+                    op_mode & _BME68X_MODE_MSK
+                )
+                self._write(reg_addr, [tmp_pow_mode])
+        except GasHeaterException as exc:
+            raise exc
+
+    def _set_conf(
+        self, heater_temp: UINT16, heater_time: UINT16, op_mode: UINT8
+    ) -> None:
+        """
+        This internal API is used to set heater configurations
+        """
+        try:
+            if op_mode != _BME68X_FORCED_MODE:
+                raise GasHeaterException("_set_conf not forced mode")
+            rh_reg_addr: UINT8 = _BME680_BME680_RES_HEAT_0
+            rh_reg_data: UINT8 = self._calc_res_heat(heater_temp)
+            gw_reg_addr: UINT8 = _BME680_BME680_GAS_WAIT_0
+            gw_reg_data: UINT8 = self._calc_gas_wait(heater_time)
+            self._write(rh_reg_addr, [rh_reg_data])
+            self._write(gw_reg_addr, [gw_reg_data])
+        except GasHeaterException as exc:
+            raise exc
+
+    def _calc_res_heat(self, temp: UINT16) -> UINT8:
+        """
+        This internal API is used to calculate the heater resistance value using float
+        """
+        gh1: INT8 = self._gas_calibration[0]
+        gh2: INT16 = self._gas_calibration[1]
+        gh3: INT8 = self._gas_calibration[2]
+        htr: UINT8 = self._heat_range
+        htv: INT8 = self._heat_val
+        amb: UINT8 = self._amb_temp
+
+        temp = min(temp, 400)  # Cap temperature
+
+        var1: INT32 = ((INT32(amb) * gh3) / 1000) * 256
+        var2: INT32 = (gh1 + 784) * (
+            ((((gh2 + 154009) * temp * 5) / 100) + 3276800) / 10
+        )
+        var3: INT32 = var1 + (var2 / 2)
+        var4: INT32 = var3 / (htr + 4)
+        var5: INT32 = (131 * htv) + 65536
+        heatr_res_x100: INT32 = INT32(((var4 / var5) - 250) * 34)
+        heatr_res: UINT8 = UINT8((heatr_res_x100 + 50) / 100)
+
+        return heatr_res
+
+    def _calc_res_heat(self, temp: UINT16) -> UINT8:
+        """
+        This internal API is used to calculate the heater resistance value
+        """
+        gh1: float = float(self._gas_calibration[0])
+        gh2: float = float(self._gas_calibration[1])
+        gh3: float = float(self._gas_calibration[2])
+        htr: float = float(self._heat_range)
+        htv: float = float(self._heat_val)
+        amb: float = float(self._amb_temp)
+
+        temp = min(temp, 400)  # Cap temperature
+
+        var1: float = (gh1 / (16.0)) + 49.0
+        var2: float = ((gh2 / (32768.0)) * (0.0005)) + 0.00235
+        var3: float = gh3 / (1024.0)
+        var4: float = var1 * (1.0 + (var2 * float(temp)))
+        var5: float = var4 + (var3 * amb)
+        res_heat: UINT8 = UINT8(
+            3.4 * ((var5 * (4 / (4 + htr)) * (1 / (1 + (htv * 0.002)))) - 25)
+        )
+        return res_heat
+
+    def _calc_gas_wait(self, dur: UINT16) -> UINT8:
+        """
+        This internal API is used to calculate the gas wait
+        """
+        factor: UINT8 = 0
+        durval: UINT8 = 0xFF  # Max duration
+
+        if dur < 0xFC0:
+            return durval
+        while dur > 0x3F:
+            dur = dur / 4
+            factor += 1
+        durval = UINT8(dur + (factor * 64))
+        return durval
+
+    # garberw added end ===========================
+
 
 class Adafruit_BME680_I2C(Adafruit_BME680):
     """Driver for I2C connected BME680.
 
     :param ~busio.I2C i2c: The I2C bus the BME680 is connected to.
     :param int address: I2C device address. Defaults to :const:`0x77`
     :param bool debug: Print debug statements when `True`. Defaults to `False`
```

### Comparing `adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/PKG-INFO` & `adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bme680
-Version: 3.4.9
+Version: 3.5.0
 Summary: CircuitPython driver for BME680 sensor over I2C
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BME680
 Keywords: adafruit,blinka,circuitpython,micropython,bme680,hardware,temperature,pressure,humidity,gas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bme680/badge/?version=latest
```

### Comparing `adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/SOURCES.txt` & `adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_bme680.py
+contributors.md
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
+LICENSES/BSD-3-Clause.txt
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_bme680.egg-info/PKG-INFO
 adafruit_circuitpython_bme680.egg-info/SOURCES.txt
 adafruit_circuitpython_bme680.egg-info/dependency_links.txt
 adafruit_circuitpython_bme680.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-bme680-3.4.9/docs/_static/favicon.ico` & `adafruit-circuitpython-bme680-3.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.9/docs/conf.py` & `adafruit-circuitpython-bme680-3.5.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
 ]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "BusDevice": (
@@ -35,15 +37,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit BME680 Library"
-copyright = "2017 ladyada"
+creation_year = "2017"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " ladyada"
 author = "ladyada"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-bme680-3.4.9/docs/index.rst` & `adafruit-circuitpython-bme680-3.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.9/examples/bme680_simpletest.py` & `adafruit-circuitpython-bme680-3.5.0/examples/bme680_simpletest.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import time
 import board
 import adafruit_bme680
 
 # Create sensor object, communicating over the board's default I2C bus
 i2c = board.I2C()  # uses board.SCL and board.SDA
+# i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
 bme680 = adafruit_bme680.Adafruit_BME680_I2C(i2c, debug=False)
 
 # change this to match the location's pressure (hPa) at sea level
 bme680.sea_level_pressure = 1013.25
 
 # You will usually have to add an offset to account for the temperature of
 # the sensor. This is usually around 5 degrees but varies by use. Use a
```

### Comparing `adafruit-circuitpython-bme680-3.4.9/examples/bme680_spi.py` & `adafruit-circuitpython-bme680-3.5.0/examples/bme680_spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.9/pyproject.toml` & `adafruit-circuitpython-bme680-3.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bme680"
 description = "CircuitPython driver for BME680 sensor over I2C"
-version = "3.4.9"
+version = "3.5.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BME680"}
 keywords = [
     "adafruit",
@@ -35,14 +35,15 @@
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Embedded Systems",
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
-dynamic = ["dependencies"]
+dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
 py-modules = ["adafruit_bme680"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
+optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

