# Comparing `tmp/chalice-1.9.0.tar.gz` & `tmp/chalice-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chalice-1.9.0.tar", last modified: Mon Jun 17 21:59:19 2019, max compression
+gzip compressed data, was "dist/chalice-1.9.1.tar", last modified: Tue Jul  9 20:10:55 2019, max compression
```

## Comparing `chalice-1.9.0.tar` & `chalice-1.9.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/
--rw-r--r--   0 root         (0) root         (0)    39586 2019-06-17 21:59:03.000000 chalice-1.9.0/README.rst
--rw-r--r--   0 root         (0) root         (0)       61 2019-06-17 21:59:19.000000 chalice-1.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6579 2019-06-17 21:59:03.000000 chalice-1.9.0/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    11357 2019-06-17 21:59:03.000000 chalice-1.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1439 2019-06-17 21:59:19.000000 chalice-1.9.0/setup.py
--rw-r--r--   0 root         (0) root         (0)    50422 2019-06-17 21:59:19.000000 chalice-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2019-06-17 21:59:03.000000 chalice-1.9.0/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      233 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       46 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    50422 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1988 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-06-17 21:59:16.000000 chalice-1.9.0/chalice.egg-info/not-zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice/
--rw-r--r--   0 root         (0) root         (0)    26840 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/local.py
--rw-r--r--   0 root         (0) root         (0)     4222 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/logs.py
--rw-r--r--   0 root         (0) root         (0)      287 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/policies-extra.json
--rw-r--r--   0 root         (0) root         (0)     5782 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/compat.py
--rw-r--r--   0 root         (0) root         (0)    41629 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/awsclient.py
--rw-r--r--   0 root         (0) root         (0)   282631 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/policies.json
--rw-r--r--   0 root         (0) root         (0)    26358 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/analyzer.py
--rw-r--r--   0 root         (0) root         (0)     9143 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/utils.py
--rw-r--r--   0 root         (0) root         (0)     6038 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/constants.py
--rw-r--r--   0 root         (0) root         (0)     7385 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/policy.py
--rw-r--r--   0 root         (0) root         (0)      472 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16519 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice/cli/
--rw-r--r--   0 root         (0) root         (0)    19363 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4475 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/cli/reloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice/cli/filewatch/
--rw-r--r--   0 root         (0) root         (0)     3429 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/cli/filewatch/stat.py
--rw-r--r--   0 root         (0) root         (0)     1285 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/cli/filewatch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1530 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/cli/filewatch/eventbased.py
--rw-r--r--   0 root         (0) root         (0)    11617 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/cli/factory.py
--rw-r--r--   0 root         (0) root         (0)    16566 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice/deploy/
--rw-r--r--   0 root         (0) root         (0)     6442 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/deploy/executor.py
--rw-r--r--   0 root         (0) root         (0)    10399 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/deploy/swagger.py
--rw-r--r--   0 root         (0) root         (0)     8036 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/deploy/validate.py
--rw-r--r--   0 root         (0) root         (0)     5903 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/deploy/models.py
--rw-r--r--   0 root         (0) root         (0)    39195 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/deploy/planner.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/deploy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37014 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/deploy/deployer.py
--rw-r--r--   0 root         (0) root         (0)    34759 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/deploy/packager.py
--rw-r--r--   0 root         (0) root         (0)     4162 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/invoke.py
--rw-r--r--   0 root         (0) root         (0)    20085 2019-06-17 21:59:03.000000 chalice-1.9.0/chalice/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    46531 2019-06-17 21:59:19.000000 chalice-1.9.0/chalice/app.py
--rw-r--r--   0 root         (0) root         (0)    22486 2019-06-17 21:59:19.000000 chalice-1.9.0/CHANGELOG.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)     3049 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/test_logs.py
--rw-r--r--   0 root         (0) root         (0)    62920 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/test_app.py
--rw-r--r--   0 root         (0) root         (0)    19056 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/test_package.py
--rw-r--r--   0 root         (0) root         (0)     2967 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     7715 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/test_pipeline.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/tests/unit/cli/
--rw-r--r--   0 root         (0) root         (0)      892 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/cli/test_cli.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/tests/unit/deploy/
--rw-r--r--   0 root         (0) root         (0)    10498 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/deploy/test_packager.py
--rw-r--r--   0 root         (0) root         (0)     9361 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/deploy/test_validate.py
--rw-r--r--   0 root         (0) root         (0)    52290 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/deploy/test_deployer.py
--rw-r--r--   0 root         (0) root         (0)    62112 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/deploy/test_planner.py
--rw-r--r--   0 root         (0) root         (0)    21373 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/deploy/test_swagger.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/deploy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1762 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/deploy/test_models.py
--rw-r--r--   0 root         (0) root         (0)    10289 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/deploy/test_executor.py
--rw-r--r--   0 root         (0) root         (0)     3121 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/conftest.py
--rw-r--r--   0 root         (0) root         (0)    20674 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/test_analyzer.py
--rw-r--r--   0 root         (0) root         (0)    20779 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/test_config.py
--rw-r--r--   0 root         (0) root         (0)     8180 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/test_invoke.py
--rw-r--r--   0 root         (0) root         (0)    38929 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/test_local.py
--rw-r--r--   0 root         (0) root         (0)     4901 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/unit/test_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/tests/functional/
--rw-r--r--   0 root         (0) root         (0)    43166 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/test_package.py
--rw-r--r--   0 root         (0) root         (0)     3771 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    12339 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/test_deployer.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-17 21:59:19.000000 chalice-1.9.0/tests/functional/cli/
--rw-r--r--   0 root         (0) root         (0)    19860 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/cli/test_cli.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9617 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/cli/test_factory.py
--rw-r--r--   0 root         (0) root         (0)     3775 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/cli/test_reloader.py
--rw-r--r--   0 root         (0) root         (0)      106 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/conftest.py
--rw-r--r--   0 root         (0) root         (0)     8658 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/test_local.py
--rw-r--r--   0 root         (0) root         (0)    77255 2019-06-17 21:59:03.000000 chalice-1.9.0/tests/functional/test_awsclient.py
--rw-r--r--   0 root         (0) root         (0)       64 2019-06-17 21:59:03.000000 chalice-1.9.0/NOTICE
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/
+-rw-r--r--   0 root         (0) root         (0)       64 2019-07-09 20:10:39.000000 chalice-1.9.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    39586 2019-07-09 20:10:39.000000 chalice-1.9.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)    11357 2019-07-09 20:10:39.000000 chalice-1.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6579 2019-07-09 20:10:39.000000 chalice-1.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)      192 2019-07-09 20:10:39.000000 chalice-1.9.1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       14 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1988 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-07-09 20:10:52.000000 chalice-1.9.1/chalice.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      233 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)    50422 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice/
+-rw-r--r--   0 root         (0) root         (0)      287 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/policies-extra.json
+-rw-r--r--   0 root         (0) root         (0)     9143 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/utils.py
+-rw-r--r--   0 root         (0) root         (0)   282631 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/policies.json
+-rw-r--r--   0 root         (0) root         (0)    16566 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/config.py
+-rw-r--r--   0 root         (0) root         (0)    20085 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/compat.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/policy.py
+-rw-r--r--   0 root         (0) root         (0)     4222 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/logs.py
+-rw-r--r--   0 root         (0) root         (0)     6038 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/constants.py
+-rw-r--r--   0 root         (0) root         (0)    26358 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/analyzer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice/cli/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice/cli/filewatch/
+-rw-r--r--   0 root         (0) root         (0)     3429 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/cli/filewatch/stat.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/cli/filewatch/eventbased.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/cli/filewatch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/cli/reloader.py
+-rw-r--r--   0 root         (0) root         (0)    11617 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/cli/factory.py
+-rw-r--r--   0 root         (0) root         (0)    19363 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/invoke.py
+-rw-r--r--   0 root         (0) root         (0)    16519 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/package.py
+-rw-r--r--   0 root         (0) root         (0)    46874 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice/app.py
+-rw-r--r--   0 root         (0) root         (0)      472 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/chalice/deploy/
+-rw-r--r--   0 root         (0) root         (0)    37014 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/deploy/deployer.py
+-rw-r--r--   0 root         (0) root         (0)    10399 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/deploy/swagger.py
+-rw-r--r--   0 root         (0) root         (0)    34759 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/deploy/packager.py
+-rw-r--r--   0 root         (0) root         (0)     8036 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/deploy/validate.py
+-rw-r--r--   0 root         (0) root         (0)     5903 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/deploy/models.py
+-rw-r--r--   0 root         (0) root         (0)    39195 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/deploy/planner.py
+-rw-r--r--   0 root         (0) root         (0)     6442 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/deploy/executor.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/deploy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26840 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/local.py
+-rw-r--r--   0 root         (0) root         (0)    41629 2019-07-09 20:10:39.000000 chalice-1.9.1/chalice/awsclient.py
+-rw-r--r--   0 root         (0) root         (0)    22585 2019-07-09 20:10:55.000000 chalice-1.9.1/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)       61 2019-07-09 20:10:55.000000 chalice-1.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1439 2019-07-09 20:10:55.000000 chalice-1.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)     3771 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8658 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/test_local.py
+-rw-r--r--   0 root         (0) root         (0)    12339 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/test_deployer.py
+-rw-r--r--   0 root         (0) root         (0)      106 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/tests/functional/cli/
+-rw-r--r--   0 root         (0) root         (0)     9617 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/cli/test_factory.py
+-rw-r--r--   0 root         (0) root         (0)    19860 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/cli/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     3775 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/cli/test_reloader.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43166 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/test_package.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77255 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/functional/test_awsclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)     2967 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    38929 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/test_local.py
+-rw-r--r--   0 root         (0) root         (0)    20779 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     3049 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/test_logs.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/tests/unit/cli/
+-rw-r--r--   0 root         (0) root         (0)      892 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/cli/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64430 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/test_app.py
+-rw-r--r--   0 root         (0) root         (0)    19056 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/test_package.py
+-rw-r--r--   0 root         (0) root         (0)     7715 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/test_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-09 20:10:55.000000 chalice-1.9.1/tests/unit/deploy/
+-rw-r--r--   0 root         (0) root         (0)    21373 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/deploy/test_swagger.py
+-rw-r--r--   0 root         (0) root         (0)    52290 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/deploy/test_deployer.py
+-rw-r--r--   0 root         (0) root         (0)    62112 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/deploy/test_planner.py
+-rw-r--r--   0 root         (0) root         (0)    10289 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/deploy/test_executor.py
+-rw-r--r--   0 root         (0) root         (0)     9361 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/deploy/test_validate.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/deploy/test_models.py
+-rw-r--r--   0 root         (0) root         (0)    10498 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/deploy/test_packager.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/deploy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/test_policy.py
+-rw-r--r--   0 root         (0) root         (0)     8180 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/test_invoke.py
+-rw-r--r--   0 root         (0) root         (0)    20674 2019-07-09 20:10:39.000000 chalice-1.9.1/tests/unit/test_analyzer.py
+-rw-r--r--   0 root         (0) root         (0)    50422 2019-07-09 20:10:55.000000 chalice-1.9.1/PKG-INFO
```

### Comparing `chalice-1.9.0/README.rst` & `chalice-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/CONTRIBUTING.rst` & `chalice-1.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/LICENSE` & `chalice-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/setup.py` & `chalice-1.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'jmespath>=0.9.3,<1.0.0',
     'wheel',
     'setuptools'
 ]
 
 setup(
     name='chalice',
-    version='1.9.0',
+    version='1.9.1',
     description="Microframework",
     long_description=README,
     author="James Saryerwinnie",
     author_email='js@jamesls.com',
     url='https://github.com/aws/chalice',
     packages=find_packages(exclude=['tests']),
     install_requires=install_requires,
```

### Comparing `chalice-1.9.0/PKG-INFO` & `chalice-1.9.1/chalice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalice
-Version: 1.9.0
+Version: 1.9.1
 Summary: Microframework
 Home-page: https://github.com/aws/chalice
 Author: James Saryerwinnie
 Author-email: js@jamesls.com
 License: Apache License 2.0
 Description: ========================================
         Python Serverless Microframework for AWS
```

### Comparing `chalice-1.9.0/chalice.egg-info/PKG-INFO` & `chalice-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalice
-Version: 1.9.0
+Version: 1.9.1
 Summary: Microframework
 Home-page: https://github.com/aws/chalice
 Author: James Saryerwinnie
 Author-email: js@jamesls.com
 License: Apache License 2.0
 Description: ========================================
         Python Serverless Microframework for AWS
```

### Comparing `chalice-1.9.0/chalice.egg-info/SOURCES.txt` & `chalice-1.9.1/chalice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/local.py` & `chalice-1.9.1/chalice/local.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/logs.py` & `chalice-1.9.1/chalice/logs.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/compat.py` & `chalice-1.9.1/chalice/compat.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/awsclient.py` & `chalice-1.9.1/chalice/awsclient.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/policies.json` & `chalice-1.9.1/chalice/policies.json`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/analyzer.py` & `chalice-1.9.1/chalice/analyzer.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/utils.py` & `chalice-1.9.1/chalice/utils.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/constants.py` & `chalice-1.9.1/chalice/constants.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/policy.py` & `chalice-1.9.1/chalice/policy.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/package.py` & `chalice-1.9.1/chalice/package.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/cli/__init__.py` & `chalice-1.9.1/chalice/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/cli/reloader.py` & `chalice-1.9.1/chalice/cli/reloader.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/cli/filewatch/stat.py` & `chalice-1.9.1/chalice/cli/filewatch/stat.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/cli/filewatch/__init__.py` & `chalice-1.9.1/chalice/cli/filewatch/__init__.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/cli/filewatch/eventbased.py` & `chalice-1.9.1/chalice/cli/filewatch/eventbased.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/cli/factory.py` & `chalice-1.9.1/chalice/cli/factory.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/config.py` & `chalice-1.9.1/chalice/config.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/deploy/executor.py` & `chalice-1.9.1/chalice/deploy/executor.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/deploy/swagger.py` & `chalice-1.9.1/chalice/deploy/swagger.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/deploy/validate.py` & `chalice-1.9.1/chalice/deploy/validate.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/deploy/models.py` & `chalice-1.9.1/chalice/deploy/models.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/deploy/planner.py` & `chalice-1.9.1/chalice/deploy/planner.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/deploy/deployer.py` & `chalice-1.9.1/chalice/deploy/deployer.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/deploy/packager.py` & `chalice-1.9.1/chalice/deploy/packager.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/invoke.py` & `chalice-1.9.1/chalice/invoke.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/pipeline.py` & `chalice-1.9.1/chalice/pipeline.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/chalice/app.py` & `chalice-1.9.1/chalice/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,34 +7,36 @@
 import json
 import traceback
 import decimal
 import base64
 from collections import defaultdict
 
 
-__version__ = '1.9.0'
+__version__ = '1.9.1'
 _PARAMS = re.compile(r'{\w+}')
 
 # Implementation note:  This file is intended to be a standalone file
 # that gets copied into the lambda deployment package.  It has no dependencies
 # on other parts of chalice so it can stay small and lightweight, with minimal
 # startup overhead.  This also means we need to handle py2/py3 compat issues
 # directly in this file instead of copying over compat.py
 try:
     from urllib.parse import unquote_plus
     from collections.abc import Mapping
+    from collections.abc import MutableMapping
 
     unquote_str = unquote_plus
 
     # In python 3 string and bytes are different so we explicitly check
     # for both.
     _ANY_STRING = (str, bytes)
 except ImportError:
     from urllib import unquote_plus
     from collections import Mapping
+    from collections import MutableMapping
 
     # This is borrowed from botocore/compat.py
     def unquote_str(value, encoding='utf-8'):
         # In python2, unquote() gives us a string back that has the urldecoded
         # bits, but not the unicode parts.  We need to decode this manually.
         # unquote has special logic in which if it receives a unicode object it
         # will decode it to latin1.  This is hard coded.  To avoid this, we'll
@@ -146,44 +148,55 @@
     MethodNotAllowedError,
     RequestTimeoutError,
     ConflictError,
     UnprocessableEntityError,
     TooManyRequestsError]
 
 
-class MultiDict(Mapping):
-    """A read only mapping of key to list of values.
+class MultiDict(MutableMapping):  # pylint: disable=too-many-ancestors
+    """A mapping of key to list of values.
 
     Accessing it in the usual way will return the last value in the list.
-    Calling getlist will return a list of values with the same key.
+    Calling getlist will return a list of all the values associated with
+    the same key.
     """
 
     def __init__(self, mapping):
         if mapping is None:
             mapping = {}
 
         self._dict = mapping
 
     def __getitem__(self, k):
-        values_list = self._dict[k]
-
         try:
-            return values_list[-1]
+            return self._dict[k][-1]
         except IndexError:
             raise KeyError(k)
 
+    def __setitem__(self, k, v):
+        self._dict[k] = [v]
+
+    def __delitem__(self, k):
+        del self._dict[k]
+
     def getlist(self, k):
-        return list(self._dict.get(k, []))
+        return list(self._dict[k])
 
     def __len__(self):
         return len(self._dict)
 
     def __iter__(self):
         return iter(self._dict)
 
+    def __repr__(self):
+        return 'MultiDict(%s)' % self._dict
+
+    def __str__(self):
+        return repr(self)
+
 
 class CaseInsensitiveMapping(Mapping):
     """Case insensitive and read-only mapping."""
 
     def __init__(self, mapping):
         mapping = mapping or {}
         self._dict = {k.lower(): v for k, v in mapping.items()}
```

### Comparing `chalice-1.9.0/CHANGELOG.rst` & `chalice-1.9.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 CHANGELOG
 =========
 
+1.9.1
+=====
+
+* Make MultiDict mutable
+  (`#1158 <https://github.com/aws/chalice/issues/1158>`__)
+
+
 1.9.0
 =====
 
 * Update PIP to support up to 19.1.x
   (`#1104 <https://github.com/aws/chalice/issues/1104>`__)
 * Fix handling of more complex Accept headers for binary
   content types
```

### Comparing `chalice-1.9.0/tests/unit/test_logs.py` & `chalice-1.9.1/tests/unit/test_logs.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/test_app.py` & `chalice-1.9.1/tests/unit/test_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1914,21 +1914,24 @@
 def test_multidict_raises_keyerror(input_dict):
     d = MultiDict(input_dict)
     with pytest.raises(KeyError):
         val = d['key']
         assert val is val
 
 
-@pytest.mark.parametrize('input_dict', [
-    {},
-    {'key': []}
-])
-def test_multidict_returns_emptylist(input_dict):
-    d = MultiDict(input_dict)
-    assert d.getlist('key') == []
+def test_multidict_pop_raises_del_error():
+    d = MultiDict({})
+    with pytest.raises(KeyError):
+        del d['key']
+
+
+def test_multidict_getlist_does_raise_keyerror():
+    d = MultiDict({})
+    with pytest.raises(KeyError):
+        d.getlist('key')
 
 
 @pytest.mark.parametrize('input_dict', [
     {'key': ['value']},
     {'key': ['']},
     {'key': ['value1', 'value2', 'value3']},
     {'key': ['value1', 'value2', None]}
@@ -1958,11 +1961,75 @@
 def test_multidict_list_wont_change_source(input_dict):
     d = MultiDict(input_dict)
     dict_copy = deepcopy(input_dict)
     d.getlist('key')[0] = 'othervalue'
     assert d.getlist('key') == dict_copy['key']
 
 
-def test_multidict_is_readonly():
-    d = MultiDict(None)
-    with pytest.raises(TypeError):
-        d['key'] = 'value'
+@pytest.mark.parametrize('input_dict,key,popped,leftover', [
+    (
+        {'key': ['value'], 'key2': [[]]},
+        'key',
+        'value',
+        {'key2': []},
+    ),
+    (
+        {'key': [''], 'key2': [[]]},
+        'key',
+        '',
+        {'key2': []},
+    ),
+    (
+        {'key': ['value1', 'value2', 'value3'],
+         'key2': [[]]},
+        'key',
+        'value3',
+        {'key2': []},
+    ),
+])
+def test_multidict_list_can_pop_value(input_dict, key, popped, leftover):
+    d = MultiDict(input_dict)
+    pop_result = d.pop(key)
+    assert popped == pop_result
+    assert leftover == {key: d[key] for key in d}
+
+
+def test_multidict_assignment():
+    d = MultiDict({})
+    d['key'] = 'value'
+    assert d['key'] == 'value'
+
+
+def test_multidict_get_reassigned_value():
+    d = MultiDict({})
+    d['key'] = 'value'
+    assert d['key'] == 'value'
+    assert d.get('key') == 'value'
+    assert d.getlist('key') == ['value']
+
+
+def test_multidict_get_list_wraps_key():
+    d = MultiDict({})
+    d['key'] = ['value']
+    assert d.getlist('key') == [['value']]
+
+
+def test_multidict_repr():
+    d = MultiDict({
+        'foo': ['bar', 'baz'],
+        'buz': ['qux'],
+    })
+    rep = repr(d)
+    assert rep.startswith('MultiDict({')
+    assert "'foo': ['bar', 'baz']" in rep
+    assert "'buz': ['qux']" in rep
+
+
+def test_multidict_str():
+    d = MultiDict({
+        'foo': ['bar', 'baz'],
+        'buz': ['qux'],
+    })
+    rep = str(d)
+    assert rep.startswith('MultiDict({')
+    assert "'foo': ['bar', 'baz']" in rep
+    assert "'buz': ['qux']" in rep
```

### Comparing `chalice-1.9.0/tests/unit/test_package.py` & `chalice-1.9.1/tests/unit/test_package.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/test_utils.py` & `chalice-1.9.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/test_pipeline.py` & `chalice-1.9.1/tests/unit/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/cli/test_cli.py` & `chalice-1.9.1/tests/unit/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/deploy/test_packager.py` & `chalice-1.9.1/tests/unit/deploy/test_packager.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/deploy/test_validate.py` & `chalice-1.9.1/tests/unit/deploy/test_validate.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/deploy/test_deployer.py` & `chalice-1.9.1/tests/unit/deploy/test_deployer.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/deploy/test_planner.py` & `chalice-1.9.1/tests/unit/deploy/test_planner.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/deploy/test_swagger.py` & `chalice-1.9.1/tests/unit/deploy/test_swagger.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/deploy/test_models.py` & `chalice-1.9.1/tests/unit/deploy/test_models.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/deploy/test_executor.py` & `chalice-1.9.1/tests/unit/deploy/test_executor.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/conftest.py` & `chalice-1.9.1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/test_analyzer.py` & `chalice-1.9.1/tests/unit/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/test_config.py` & `chalice-1.9.1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/test_invoke.py` & `chalice-1.9.1/tests/unit/test_invoke.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/test_local.py` & `chalice-1.9.1/tests/unit/test_local.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/unit/test_policy.py` & `chalice-1.9.1/tests/unit/test_policy.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/functional/test_package.py` & `chalice-1.9.1/tests/functional/test_package.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/functional/test_utils.py` & `chalice-1.9.1/tests/functional/test_utils.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/functional/test_deployer.py` & `chalice-1.9.1/tests/functional/test_deployer.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/functional/cli/test_cli.py` & `chalice-1.9.1/tests/functional/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/functional/cli/test_factory.py` & `chalice-1.9.1/tests/functional/cli/test_factory.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/functional/cli/test_reloader.py` & `chalice-1.9.1/tests/functional/cli/test_reloader.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/functional/test_local.py` & `chalice-1.9.1/tests/functional/test_local.py`

 * *Files identical despite different names*

### Comparing `chalice-1.9.0/tests/functional/test_awsclient.py` & `chalice-1.9.1/tests/functional/test_awsclient.py`

 * *Files identical despite different names*

