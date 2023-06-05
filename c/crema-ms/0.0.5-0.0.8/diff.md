# Comparing `tmp/crema-ms-0.0.5.tar.gz` & `tmp/crema-ms-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crema-ms-0.0.5.tar", last modified: Fri Jun 11 18:12:46 2021, max compression
+gzip compressed data, was "crema-ms-0.0.8.tar", last modified: Mon Jun  5 15:57:03 2023, max compression
```

## Comparing `crema-ms-0.0.5.tar` & `crema-ms-0.0.8.tar`

### file list

```diff
@@ -1,73 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.622231 crema-ms-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.602230 crema-ms-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.606230 crema-ms-0.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      672 2021-06-11 18:12:31.000000 crema-ms-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.606230 crema-ms-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2021-06-11 18:12:31.000000 crema-ms-0.0.5/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (121)      853 2021-06-11 18:12:31.000000 crema-ms-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2021-06-11 18:12:31.000000 crema-ms-0.0.5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2281 2021-06-11 18:12:31.000000 crema-ms-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-06-11 18:12:31.000000 crema-ms-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-06-11 18:12:31.000000 crema-ms-0.0.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-11 18:12:31.000000 crema-ms-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2597 2021-06-11 18:12:46.622231 crema-ms-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2021-06-11 18:12:31.000000 crema-ms-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.606230 crema-ms-0.0.5/crema/
--rw-r--r--   0 runner    (1001) docker     (121)      729 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12000 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/confidence.py
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/crema.py
--rw-r--r--   0 runner    (1001) docker     (121)     7375 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3320 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/params.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.606230 crema-ms-0.0.5/crema/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5705 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/parsers/crux.py
--rw-r--r--   0 runner    (1001) docker     (121)     2885 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/parsers/mztab.py
--rw-r--r--   0 runner    (1001) docker     (121)     3832 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/parsers/txt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/qvalues.py
--rw-r--r--   0 runner    (1001) docker     (121)      538 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.606230 crema-ms-0.0.5/crema/writers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2941 2021-06-11 18:12:31.000000 crema-ms-0.0.5/crema/writers/txt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.610230 crema-ms-0.0.5/crema_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2597 2021-06-11 18:12:46.000000 crema-ms-0.0.5/crema_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2021-06-11 18:12:46.000000 crema-ms-0.0.5/crema_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-11 18:12:46.000000 crema-ms-0.0.5/crema_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-06-11 18:12:46.000000 crema-ms-0.0.5/crema_ms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-06-11 18:12:46.000000 crema-ms-0.0.5/crema_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-11 18:12:46.000000 crema-ms-0.0.5/crema_ms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.614230 crema-ms-0.0.5/data/
--rw-r--r--   0 runner    (1001) docker     (121)  1268941 2021-06-11 18:12:31.000000 crema-ms-0.0.5/data/MSV000085729.mzTab
--rw-r--r--   0 runner    (1001) docker     (121)  3536154 2021-06-11 18:12:31.000000 crema-ms-0.0.5/data/example_psms_decoy.txt
--rw-r--r--   0 runner    (1001) docker     (121)  3364063 2021-06-11 18:12:31.000000 crema-ms-0.0.5/data/example_psms_target.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.618230 crema-ms-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      634 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.618230 crema-ms-0.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)   105501 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/_static/crema_logo_caramel_light.png
--rw-r--r--   0 runner    (1001) docker     (121)     3028 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.618230 crema-ms-0.0.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/api/confidence.rst
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/api/dataset.rst
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/api/functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1572 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      928 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3199 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     6492 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2021-06-11 18:12:31.000000 crema-ms-0.0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      585 2021-06-11 18:12:31.000000 crema-ms-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2021-06-11 18:12:46.622231 crema-ms-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-06-11 18:12:31.000000 crema-ms-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.618230 crema-ms-0.0.5/static/
--rw-r--r--   0 runner    (1001) docker     (121)   762279 2021-06-11 18:12:31.000000 crema-ms-0.0.5/static/crema_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.622231 crema-ms-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:31.000000 crema-ms-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6385 2021-06-11 18:12:31.000000 crema-ms-0.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.622231 crema-ms-0.0.5/tests/system_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:31.000000 crema-ms-0.0.5/tests/system_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2021-06-11 18:12:31.000000 crema-ms-0.0.5/tests/system_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2021-06-11 18:12:31.000000 crema-ms-0.0.5/tests/system_tests/test_crux_tdc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:46.622231 crema-ms-0.0.5/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-11 18:12:31.000000 crema-ms-0.0.5/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2021-06-11 18:12:31.000000 crema-ms-0.0.5/tests/unit_tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-06-11 18:12:31.000000 crema-ms-0.0.5/tests/unit_tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2333 2021-06-11 18:12:31.000000 crema-ms-0.0.5/tests/unit_tests/test_qvalues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.145516 crema-ms-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.113516 crema-ms-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.117516 crema-ms-0.0.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-05 15:56:44.000000 crema-ms-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.117516 crema-ms-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-05 15:56:44.000000 crema-ms-0.0.8/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-05 15:56:44.000000 crema-ms-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-05 15:56:44.000000 crema-ms-0.0.8/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-05 15:56:44.000000 crema-ms-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-05 15:56:44.000000 crema-ms-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 15:56:44.000000 crema-ms-0.0.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-06-05 15:56:44.000000 crema-ms-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-05 15:57:03.145516 crema-ms-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-05 15:56:44.000000 crema-ms-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.121516 crema-ms-0.0.8/crema/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25994 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/confidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/crema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.121516 crema-ms-0.0.8/crema/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/parsers/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/parsers/msamanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/parsers/msfragger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/parsers/msgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/parsers/mztab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/parsers/pepxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/parsers/tide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/parsers/txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/qvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.125516 crema-ms-0.0.8/crema/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-05 15:56:44.000000 crema-ms-0.0.8/crema/writers/txt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.125516 crema-ms-0.0.8/crema_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-05 15:57:03.000000 crema-ms-0.0.8/crema_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-05 15:57:03.000000 crema-ms-0.0.8/crema_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:57:03.000000 crema-ms-0.0.8/crema_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 15:57:03.000000 crema-ms-0.0.8/crema_ms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-05 15:57:03.000000 crema-ms-0.0.8/crema_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 15:57:03.000000 crema-ms-0.0.8/crema_ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.133516 crema-ms-0.0.8/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1268941 2023-06-05 15:56:44.000000 crema-ms-0.0.8/data/MSV000085729.mzTab
+-rw-r--r--   0 runner    (1001) docker     (123)  3536154 2023-06-05 15:56:44.000000 crema-ms-0.0.8/data/example_psms_decoy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  3364063 2023-06-05 15:56:44.000000 crema-ms-0.0.8/data/example_psms_target.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    97312 2023-06-05 15:56:44.000000 crema-ms-0.0.8/data/msfragger.pepxml
+-rw-r--r--   0 runner    (1001) docker     (123)  5511838 2023-06-05 15:56:44.000000 crema-ms-0.0.8/data/tide-search.pep.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.141516 crema-ms-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.141516 crema-ms-0.0.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   105501 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/_static/crema_logo_caramel_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.141516 crema-ms-0.0.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/api/confidence.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/api/dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/api/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-05 15:56:44.000000 crema-ms-0.0.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-05 15:56:44.000000 crema-ms-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-05 15:57:03.145516 crema-ms-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 15:56:44.000000 crema-ms-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.141516 crema-ms-0.0.8/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   762279 2023-06-05 15:56:44.000000 crema-ms-0.0.8/static/crema_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.145516 crema-ms-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:56:44.000000 crema-ms-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-05 15:56:44.000000 crema-ms-0.0.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.145516 crema-ms-0.0.8/tests/system_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:56:44.000000 crema-ms-0.0.8/tests/system_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-05 15:56:44.000000 crema-ms-0.0.8/tests/system_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-05 15:56:44.000000 crema-ms-0.0.8/tests/system_tests/test_crux_tdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:57:03.145516 crema-ms-0.0.8/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:56:44.000000 crema-ms-0.0.8/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-05 15:56:44.000000 crema-ms-0.0.8/tests/unit_tests/test_confidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-05 15:56:44.000000 crema-ms-0.0.8/tests/unit_tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-05 15:56:44.000000 crema-ms-0.0.8/tests/unit_tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-05 15:56:44.000000 crema-ms-0.0.8/tests/unit_tests/test_qvalues.py
```

### Comparing `crema-ms-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md` & `crema-ms-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/.github/workflows/publish.yml` & `crema-ms-0.0.8/.github/workflows/publish.yml`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
 
 name: PyPI
 
 on:
   release:
     types: [created]
+  workflow_dispatch:
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v2
```

### Comparing `crema-ms-0.0.5/.github/workflows/tests.yml` & `crema-ms-0.0.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/.gitignore` & `crema-ms-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/LICENSE` & `crema-ms-0.0.8/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+Copyright 2023 Battelle Memorial Institute, University of Washington,
+University of Sydney.
+
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `crema-ms-0.0.5/crema/crema.py` & `crema-ms-0.0.8/crema/crema.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 This is the command line interface for crema
 """
 import os
 import sys
 import time
 import logging
 
-from .parsers.crux import read_crux
+from .parsers.tide import read_tide
+from .parsers.msamanda import read_msamanda
+from .parsers.msfragger import read_msfragger
+from .parsers.msgf import read_msgf
+from .parsers.comet import read_comet
 from .parsers.mztab import read_mztab
+from .parsers.pepxml import read_pepxml
 from .params import Params
 
 
 def main():
     """The CLI entry point"""
     start_time = time.time()
 
@@ -33,29 +38,43 @@
         format="[%(levelname)s] %(message)s",
     )
 
     # Write logs to stderr as well
     logging.getLogger().addHandler(logging.StreamHandler())
 
     logging.info("crema")
-    logging.info("Written by Donavan See and William E Fondrie in the ")
+    logging.info(
+        "Written by Andy Lin, Donavan See and William E Fondrie in the "
+    )
     logging.info(
         "Department of Genome Sciences at the University of Washington."
     )
     logging.info("Command issued:")
     logging.info("%s", " ".join(sys.argv))
     logging.info("")
     logging.info("Starting Analysis")
     logging.info("=================")
 
     # Create dataset object
-    try:
-        psms = read_crux(args.psm_files)
-    except:  # TODO: Add specific exceptions
-        psms = read_mztab(args.psm_files)
+    readers = [
+        read_tide,
+        read_msgf,
+        read_msamanda,
+        read_comet,
+        read_msfragger,
+        read_pepxml,
+        read_mztab,
+    ]
+
+    for read_fn in readers:
+        try:
+            psms = read_fn(args.psm_files)
+            break
+        except:
+            raise ValueError("Unrecognized file type.")
 
     conf = psms.assign_confidence(
         score_column=args.score,
         eval_fdr=args.eval_fdr,
         method=args.method,
     )
```

### Comparing `crema-ms-0.0.5/crema/dataset.py` & `crema-ms-0.0.8/crema/dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """The :py:class:`PsmDataset` class is used to define a collection of
 peptide-spectrum matches.
 """
 import logging
 
 from .confidence import TdcConfidence
+from .confidence import MixmaxConfidence
 from .qvalues import tdc
 from .utils import listify
 
 LOGGER = logging.getLogger(__name__)
 
 
 class PsmDataset:
@@ -26,14 +27,19 @@
     score_columns : str or tuple of str, optional
         One or more columns that indicate scores by which crema can rank PSMs.
     peptide_column : str
         The column that defines a unique peptide. Modifications should be
         indicated either in square brackets :code:`[]` or parentheses
         :code:`()`. The exact modification format within these entities does
         not matter, so long as it is consistent.
+    protein_columns : str
+        The column that defines a unique protein.
+    protein_delim : str
+        The string delimiter that is needed to separate multiple proteins found
+        in the protein column.
     peptide_pairing: dict
         A map of target and decoy peptide sequence pairings to be used for TDC.
         This should be in the form {key=target_sequence:value=decoy_sequence}
         where decoy sequences are shuffled versions of target sequences.
     copy_data : bool, optional
         If true, a deep copy of the data is created. This uses more memory, but
         is safer because it prevents accidental modification of the underlying
@@ -43,45 +49,50 @@
     Attributes
     ----------
     data : pandas.DataFrame
     spectrum_columns : list of str
     score_columns : list of str
     target_column : str
     peptide_column : str
+    protein_column : str
+    protein_delim : str
     methods : dict
     peptide_pairing : dict
     """
 
-    methods = {
-        "tdc": TdcConfidence,
-    }
+    methods = {"tdc": TdcConfidence, "mixmax": MixmaxConfidence}
 
     def __init__(
         self,
         psms,
         target_column,
         spectrum_columns,
         score_columns,
         peptide_column,
+        protein_column,
+        protein_delim,
         peptide_pairing=None,
         copy_data=True,
     ):
         """Initialize a PsmDataset object."""
         self.score_columns = listify(score_columns)
         self._spectrum_columns = listify(spectrum_columns)
         self._target_column = target_column
         self._peptide_column = peptide_column
+        self._protein_column = protein_column
+        self._protein_delim = protein_delim
         self._peptide_pairing = peptide_pairing
 
         fields = sum(
             [
                 self._spectrum_columns,
                 self.score_columns,
                 [self._target_column],
                 [self._peptide_column],
+                [self._protein_column],
             ],
             [],
         )
         self._data = psms.copy(deep=copy_data).loc[:, fields]
         self._data[target_column] = self._data[target_column].astype(bool)
         self._num_targets = self.targets.sum()
         self._num_decoys = (~self.targets).sum()
@@ -112,14 +123,24 @@
 
     @property
     def peptides(self):
         """The peptides as a :py:class:`pandas.Series`."""
         return self[self._peptide_column]
 
     @property
+    def proteins(self):
+        """The proteins as a :py:class:`pandas.Series`."""
+        return self[self._protein_column]
+
+    @property
+    def protein_delim(self):
+        """The delimiter to split protein IDs as a string."""
+        return self[self._protein_delim]
+
+    @property
     def scores(self):
         """The scores for each PSM as a :py:class:`pandas.DataFrame`."""
         return self[self.score_columns]
 
     @property
     def targets(self):
         """An array indicating whether each PSM is a target"""
@@ -136,14 +157,17 @@
 
     def assign_confidence(
         self,
         score_column=None,
         desc=None,
         eval_fdr=0.01,
         method="tdc",
+        pep_fdr_type="psm-peptide",
+        prot_fdr_type="best",
+        threshold=0.01,
     ):
         """Assign confidence estimates to this collection of peptide-spectrum matches.
 
         Parameters
         ----------
         score_column : str, optional
             The score by which to rank the PSMs for confidence estimation. If
@@ -156,28 +180,41 @@
             rate threshold (`eval_fdr`). If `score_column` is :code:`None`,
             this parameter is ignored.
         eval_fdr : float, optional
             The false discovery rate threshold used to evaluate the best
             `score_column` and `desc` to choose. This should range from 0 to 1.
         method : {"tdc"}, optional
             The method for crema to use when calculating the confidence estimates.
+        pep_fdr_type : {"psm-only","peptide-only",psm-peptide"}, optional
+            The method for crema to use when calculating peptide level confidence
+            estimates. Default is "psm-peptide".
+        prot_fdr_type : {"best", "combine"}, optional
+            The method for crema to use when calculating protein level confidence
+            estimates. Default is "best".
+        threshold : float or "q-value", optional
+            The FDR threshold for accepting discoveries. Default is 0.01. If
+            "q-value" is chosen, then "accept" column is replaced with
+            "crema q-value".
 
         Returns
         -------
         Confidence object
             The confidence estimates for this PsmDataset.
         """
         if score_column is None:
             score_column, _, desc = self.find_best_score(eval_fdr)
 
         conf = self.methods[method](
             psms=self,
             score_column=score_column,
             desc=desc,
             eval_fdr=eval_fdr,
+            pep_fdr_type=pep_fdr_type,
+            prot_fdr_type=prot_fdr_type,
+            threshold=threshold,
         )
 
         return conf
 
     def find_best_score(self, eval_fdr=0.01):
         """Find the best score for this collection of PSMs
 
@@ -211,7 +248,35 @@
                 best_score = feat_idx
                 best_desc = desc
 
         if best_score is None:
             raise RuntimeError("No PSMs were found below the 'eval_fdr'.")
 
         return best_score, best_passing, best_desc
+
+    def set_protein_column(self, new_protein_column):
+        """Replaces current protein column with input protein column
+
+        Parameters
+        ----------
+        new_protein_column : pandas.Series
+
+        Returns
+        -------
+
+        """
+        self._data[self._protein_column] = new_protein_column
+        return
+
+    def set_peptide_column(self, new_peptide_column):
+        """Replaces current peptide column with input peptide column
+
+        Parameters
+        ----------
+        new_peptide_column : pandas.Series
+
+        Returns
+        -------
+
+        """
+        self._data[self._peptide_column] = new_peptide_column
+        return
```

### Comparing `crema-ms-0.0.5/crema/params.py` & `crema-ms-0.0.8/crema/params.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 def _configure_parser():
     """Creates and configures all the arguments for the parser"""
 
     desc = (
         f"crema version {__version__}\n\n"
-        "Written by Donavan See (seed99@cs.washington.edu) and \n"
+        "Written by Andy Lin, Donavan See (seed99@cs.washington.edu), and \n"
         "William E Fondrie (wfondrie@uw.edu) in the \n"
         "Department of Genome Sciences at the University of Washington\n\n"
         "Official code website: https://github.com/Noble-Lab/crema\n\n"
         "More documentation and examples: https://crema-ms.readthedocs.io/"
     )
 
     parser = argparse.ArgumentParser(
@@ -49,15 +49,15 @@
 
     parser.add_argument(
         "psm_files",
         type=str,
         nargs="+",
         help=(
             "One or more collection of peptide-spectrum matches (PSMs) in the "
-            "mzTab or Crux tab-delimited formats."
+            "mzTab or Tide tab-delimited formats."
         ),
     )
 
     parser.add_argument(
         "-s",
         "--score",
         type=str,
@@ -103,14 +103,32 @@
         "-m",
         "--method",
         type=str,
         default="tdc",
         choices=["tdc"],
         help="The confidence estimation method to use.",
     )
+
+    parser.add_argument(
+        "-p",
+        "--pep_fdr_type",
+        type=str,
+        default="psm-only",
+        choices=["psm-only", "peptide-only", "psm-peptide"],
+        help="The peptide-level FDR estimation method to use.",
+    )
+
+    parser.add_argument(
+        "-r",
+        "--prot_fdr_type",
+        type=str,
+        default="best",
+        choices=["best", "combine"],
+        help="The protein-level FDR estimation method to use.",
+    )
     return parser
 
 
 def _process_line(line, width, indent):
     """Process a line in the CLI help"""
     line = textwrap.fill(
         line,
```

### Comparing `crema-ms-0.0.5/crema/parsers/crux.py` & `crema-ms-0.0.8/crema/parsers/tide.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,135 @@
-"""A parser for the crux tab-delimited format"""
+"""A parser for the Tide tab-delimited format"""
 import re
 import logging
 
 import pandas as pd
 
 from .txt import read_txt
 from .. import utils
 
 LOGGER = logging.getLogger(__name__)
 
 
-def read_crux(txt_files, peptide_tdc=False, copy_data=True):
-    """Read peptide-spectrum matches (PSMs) from Crux tab-delimited files.
+def read_tide(
+    txt_files, pairing_file_name=None, decoy_prefix="decoy_", copy_data=True
+):
+    """Read peptide-spectrum matches (PSMs) from Tide tab-delimited files.
 
     Parameters
     ----------
     txt_files : str, pandas.DataFrame or tuple of str
-        One or more collection of PSMs in the Crux tab-delimited format.
-    peptide_tdc : bool, optional
-        Perform an additional step of target-decoy competition at the
-        peptide-level. Peptides are mapped to the decoys that generated them
-        and only the higher scoring of a pair are retained. This additional
-        step yields additional statistical power to detect peptides.
+        One or more collection of PSMs in the Tide tab-delimited format.
+    pairing_file_name : str, optional
+        A tab-delimited file that explicity pairs target and decoy peptide
+        sequences. Requires one column labled 'target' that contains target
+        sequences and a second colun labeled 'decoy' that contains decoy
+        sequences. This file can be generated by setting --peptide-list=T
+        in tide-index.
+    decoy_prefix : str, optional
+        The prefix used to indicate a decoy protein in the protein column.
+        Default value is 'decoy_'.
     copy_data : bool, optional
         If true, a deep copy of the data is created. This uses more memory, but
         is safer because it prevents accidental modification of the underlying
         data. This argument only has an effect when `txt_files` is a
         :py:class:`pandas.DataFrame`
 
     Returns
     -------
     PsmDataset
         A :py:class:`~crema.dataset.PsmDataset` object containing the parsed
         PSMs.
     """
     target = "target/decoy"
     peptide = "sequence"
-    spectrum = ["scan", "spectrum precursor m/z"]
+    spectrum = ["file", "scan"]
     pairing = "original target sequence"
+    protein = "protein id"
+    protein_delim = ","
 
-    # Possible score columns output by Crux.
+    # Possible score columns output by Tide.
     scores = {
         "sp score",
         "delta_cn",
         "delta_lcn",
         "xcorr score",
         "exact p-value",
         "refactored xcorr",
         "res-ev p-value",
         "combined p-value",
+        "tailor score",
     }
+    scores_all = scores
 
-    # Keep only crux scores that exist in all of the files.
+    # Keep only Tide scores that exist in all of the files.
     if isinstance(txt_files, pd.DataFrame):
         scores = scores.intersection(set(txt_files.columns))
     else:
         txt_files = utils.listify(txt_files)
         for txt_file in txt_files:
             with open(txt_file) as txt_ref:
                 cols = txt_ref.readline().rstrip().split("\t")
                 scores = scores.intersection(set(cols))
 
     if not scores:
         raise ValueError(
-            "Could not find any of the Crux score columns in all of the files."
-            f"The columns crema looks for are {', '.join(list(scores))}"
+            "Could not find any of the Tide score columns in all of the files."
+            f" The columns Crema looks for are {', '.join(list(scores_all))}"
         )
 
     scores = list(scores)
 
     # Read in the files:
-    fields = spectrum + [peptide] + [target] + scores + [pairing]
+    fields = [*spectrum, peptide, target, *scores, pairing, protein]
     if isinstance(txt_files, pd.DataFrame):
         data = txt_files.copy(deep=copy_data).loc[:, fields]
     else:
-        data = pd.concat([_parse_psms(f, fields) for f in txt_files])
+        data = pd.concat(
+            [utils.parse_psms_txt(f, fields, False) for f in txt_files]
+        )
 
     psms = read_txt(
         data,
         target_column=target,
         spectrum_columns=spectrum,
         score_columns=scores,
         peptide_column=peptide,
+        protein_column=protein,
+        protein_delim=protein_delim,
         sep="\t",
         copy_data=False,
     )
-    if peptide_tdc:
-        psms._peptide_pairing = _create_pairing(data)
-
-    return psms
 
+    # always pair target and decoys for Tide
+    if pairing_file_name == None:  # implicit pairing
+        psms._peptide_pairing = _create_pairing(data)
+    else:  # explicit pairing
+        psms._peptide_pairing = utils.create_pairing_from_file(
+            pairing_file_name
+        )
 
-def _parse_psms(txt_file, cols, log=True):
-    """Parse a single Crux tab-delimited file
-
-    Parameters
-    ----------
-    txt_file : str
-        The crux tab-delimited file to read.
-    cols : list of str
-        The columns to parse.
+    # Remove the start position of peptide in protein if present
+    # This looks like "protName(XX)"
+    # Remove decoy prefix from protein ID
+    protein_column = psms.proteins
+    new_protein_column = protein_column.str.replace(
+        "\\([^()]*\\)", "", regex=True
+    )
+    new_protein_column = new_protein_column.str.replace(
+        decoy_prefix, "", regex=True
+    )
+    psms.set_protein_column(new_protein_column)
 
-    Returns
-    -------
-    pandas.DataFrame
-        A :py:class:`pandas.DataFrame` containing the parsed PSMs
-    """
-    if log:
-        LOGGER.info("Reading PSMs from %s...", txt_file)
-    return pd.read_csv(txt_file, sep="\t", usecols=lambda c: c in cols)
+    return psms
 
 
 def _create_pairing(pairing_data):
-    """Parse a single Crux tab-delimited file
+    """Parse a single Tide dataframe to implicity pair target and
+    decoy sequences.
 
     Parameters
     ----------
     pairing_data : pandas.DataFrame
         A collection of PSMs with the necessary columns to create a
         target/decoy peptide pairing. Required columns are "peptide mass",
         "sequence", "target/decoy", "original target sequence"
@@ -162,16 +175,16 @@
     targets = pairing_data.loc[~is_decoy, :].copy()
     decoys = pairing_data.loc[is_decoy, :].copy()
 
     # Strip the target sequence modifications:
     targets[seq] = targets["sequence"].str.replace(r"\[.*?\]", "", regex=True)
 
     # Add an 'ord' column to disambiguate multiple matches per peptide:
-    targets["ord"] = targets.groupby([seq, "mods"]).rank("first")
-    decoys["ord"] = decoys.groupby([seq, "mods"]).rank("first")
+    targets["ord"] = targets.groupby([seq, "mods"])["sequence"].rank("first")
+    decoys["ord"] = decoys.groupby([seq, "mods"])["sequence"].rank("first")
 
     # Inner join the DataFrames to induce a pairing.
     # Targets with a missing decoy will be dropped.
     # Decoys with a missing target will be dropped.
     merged = pd.merge(
         targets,
         decoys,
```

### Comparing `crema-ms-0.0.5/crema/parsers/mztab.py` & `crema-ms-0.0.8/crema/parsers/mztab.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,27 +30,29 @@
     psms = pd.concat([_parse_psms(f) for f in mztab_files])
 
     # Initialize column names from mzTab standard specifications
     spectrum_col = ["spectra_ref"]
     score_col = [c for c in psms.columns if "search_engine_score" in c]
     target_col = "opt_global_cv_MS:1002217_decoy_peptide"
     sequence_col = "sequence"
+    protein_col = "accession"  # TODO check if correct
+    delim_col = ";"  # TODO check if correct
     mod_col = "modifications"
 
     # Check that all column headers are valid, otherwise, throw error
     if len(set(spectrum_col) & set(psms.columns)) < len(spectrum_col):
         raise KeyError(
             "The mzTab file does not contain the columns that define a "
             f"spectrum. These are: {', '.join(spectrum_col)}."
         )
 
     if sequence_col not in psms.columns or mod_col not in psms.columns:
         raise KeyError(
-            "The mzTab file does not the columns to specify peptide sequence "
-            "and modifications."
+            "The mzTab file does not contain the columns to specify "
+            "peptide sequence and modifications."
         )
 
     if target_col not in psms.columns:
         raise KeyError(
             "The mzTab file does not contain the column that specifies "
             f"whether a PSM is a target or decoy, {target_col}"
         )
@@ -62,23 +64,25 @@
         )
 
     # Create the necesssary columns
     psms["peptide"] = psms[sequence_col] + "[" + psms[mod_col] + "]"
     psms["target"] = ~psms[target_col].astype(bool)
 
     # Keep only the relevant columns
-    columns = spectrum_col + score_col + ["peptide", "target"]
+    columns = spectrum_col + score_col + ["peptide", "target"] + [protein_col]
     psms = psms.loc[:, columns]
 
     return PsmDataset(
         psms=psms,
         target_column="target",
         spectrum_columns=spectrum_col,
         score_columns=score_col,
         peptide_column="peptide",
+        protein_column=protein_col,
+        protein_delim=delim_col,
         copy_data=False,
     )
 
 
 def _parse_psms(mztab_file):
     """Parse a single mzTab file using Pyteomics
```

### Comparing `crema-ms-0.0.5/crema/parsers/txt.py` & `crema-ms-0.0.8/crema/parsers/txt.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,34 +10,40 @@
 
 def read_txt(
     txt_files,
     target_column,
     spectrum_columns,
     score_columns,
     peptide_column,
+    protein_column,
+    protein_delim,
     sep="\t",
     copy_data=True,
 ):
     """Read peptide-spectrum matches (PSMs) from delimited text files.
 
     Parameters
     ----------
     txt_files : str, panda.DataFrame, or tuple of str
         One or more collection of PSMs in a tabular text format.
     target_column : str
         The column that indicates whether a PSM is a target or a decoy.
     spectrum_columns : str or tuple of str
         One or more columns that together define a unique mass spectrum.
-    score_columns : str or tuple of str, optional
+    score_columns : str or tuple of str
         One or more columns that indicate scores by which crema can rank PSMs.
     peptide_column : str
         The column that defines a unique peptide. Modifications should be
         indicated either in square brackets :code:`[]` or parentheses
         :code:`()`. The exact modification format within these entities does
         not matter, so long as it is consistent.
+    protein_column : str
+        The column that defines a unique protein.
+    protein_delim : str
+        The delimiter to separate protein IDs.
     sep : str, optional
         The delimiter to use.
     copy_data : bool, optional
         If true, a deep copy of the data is created. This uses more memory, but
         is safer because it prevents accidental modification of the underlying
         data. This argument only has an effect when `pin_files` is a
         :py:class:`pandas.DataFrame`
@@ -45,15 +51,15 @@
     Returns
     -------
     PsmDataset
         A :py:class:`~crema.dataset.PsmDataset` object containing the parsed
         PSMs.
     """
     # Store column names in a list to be used by read_csv function
-    fields = [target_column, peptide_column]
+    fields = [target_column, peptide_column, protein_column]
 
     # Verify some arguments are lists:
     spectrum_columns = listify(spectrum_columns)
     score_columns = listify(score_columns)
     fields += spectrum_columns + score_columns
 
     # Parse the data
@@ -67,25 +73,27 @@
     data[target_column] = _convert_target_col(data[target_column])
     return PsmDataset(
         psms=data,
         target_column=target_column,
         spectrum_columns=spectrum_columns,
         score_columns=score_columns,
         peptide_column=peptide_column,
+        protein_column=protein_column,
+        protein_delim=protein_delim,
         copy_data=False,
     )
 
 
 def _parse_psms(txt_file, sep, cols):
     """Parse a single delimited txt file.
 
     Parameters
     ----------
     txt_file : str
-        The crux tab-delimited file to read.
+        The Crux tab-delimited file to read.
     sep : str
         The delimiter to use.
     cols : list of str
         The columns to parse.
 
     Returns
     -------
```

### Comparing `crema-ms-0.0.5/crema/writers/txt.py` & `crema-ms-0.0.8/crema/writers/txt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Writer to save results in a tab-delmited format"""
 from pathlib import Path
 from collections import defaultdict
 
 import pandas as pd
 
 
-def to_txt(conf, output_dir=None, file_root=None, sep="\t", decoys=False):
+def to_txt(
+    conf, output_dir=None, file_root=None, sep="\t", decoys=False, precision=6
+):
     """Save confidence estimates to delimited text files.
 
     Write the confidence estimates for each of the available levels
     (i.e. PSMs, peptides, proteins) to separate flat text files using the
     specified delimiter. If more than one collection of confidence estimates
     is provided, they will be combined, yielding a single file for each level
     specified by either dataset.
@@ -26,14 +28,16 @@
         always be "crema.{level}.txt" where "{level}" indicates the level at
         which confidence estimation was performed (i.e. PSMs, peptides,
         proteins).
     sep : str, optional
         The delimiter to use.
     decoys : bool, optional
         Save decoys confidence estimates as well?
+    precision : int, optional
+        Precision for float values.
 
     Returns
     -------
     list of str
         The paths to the saved files.
 
     """
@@ -55,15 +59,17 @@
     for res in conf:
         for level, qval_list in _get_level_data(res, decoys).items():
             results[level] += qval_list
 
     out_files = []
     for level, qval_list in results.items():
         out_file = str(file_base) + f".{level}.txt"
-        pd.concat(qval_list).to_csv(out_file, sep=sep, index=False)
+        pd.concat(qval_list).to_csv(
+            out_file, sep=sep, index=False, float_format=f"%.{precision}f"
+        )
         out_files.append(out_file)
 
     return out_files
 
 
 def _get_level_data(conf, decoys):
     """Return the dataframes for each level.
```

### Comparing `crema-ms-0.0.5/crema_ms.egg-info/SOURCES.txt` & `crema-ms-0.0.8/crema_ms.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -14,28 +14,35 @@
 crema/confidence.py
 crema/crema.py
 crema/dataset.py
 crema/params.py
 crema/qvalues.py
 crema/utils.py
 crema/parsers/__init__.py
-crema/parsers/crux.py
+crema/parsers/comet.py
+crema/parsers/msamanda.py
+crema/parsers/msfragger.py
+crema/parsers/msgf.py
 crema/parsers/mztab.py
+crema/parsers/pepxml.py
+crema/parsers/tide.py
 crema/parsers/txt.py
 crema/writers/__init__.py
 crema/writers/txt.py
 crema_ms.egg-info/PKG-INFO
 crema_ms.egg-info/SOURCES.txt
 crema_ms.egg-info/dependency_links.txt
 crema_ms.egg-info/entry_points.txt
 crema_ms.egg-info/requires.txt
 crema_ms.egg-info/top_level.txt
 data/MSV000085729.mzTab
 data/example_psms_decoy.txt
 data/example_psms_target.txt
+data/msfragger.pepxml
+data/tide-search.pep.xml
 docs/CHANGELOG.md
 docs/Makefile
 docs/cli.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/_static/crema_logo_caramel_light.png
@@ -47,10 +54,11 @@
 static/crema_logo.svg
 tests/__init__.py
 tests/conftest.py
 tests/system_tests/__init__.py
 tests/system_tests/test_cli.py
 tests/system_tests/test_crux_tdc.py
 tests/unit_tests/__init__.py
+tests/unit_tests/test_confidence.py
 tests/unit_tests/test_dataset.py
 tests/unit_tests/test_parsers.py
 tests/unit_tests/test_qvalues.py
```

### Comparing `crema-ms-0.0.5/data/MSV000085729.mzTab` & `crema-ms-0.0.8/data/MSV000085729.mzTab`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/data/example_psms_decoy.txt` & `crema-ms-0.0.8/data/example_psms_decoy.txt`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/data/example_psms_target.txt` & `crema-ms-0.0.8/data/example_psms_target.txt`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/docs/Makefile` & `crema-ms-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/docs/_static/crema_logo_caramel_light.png` & `crema-ms-0.0.8/docs/_static/crema_logo_caramel_light.png`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/docs/_static/custom.css` & `crema-ms-0.0.8/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/docs/api/index.rst` & `crema-ms-0.0.8/docs/api/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Python API
 ==========
 The Python API enables maximum flexibility using crema.
 
-Read PSMs easily using the :py:func:`~crema.read_crux()` or
-:py:func:`~crema.read_mztab()` functions for files in the Crux
+Read PSMs easily using the :py:func:`~crema.read_tide()` or
+:py:func:`~crema.read_mztab()` functions for files in the Tide
 tab-delimited format or mzTab format, respectively. Alternatively,
 more generic tab delimited files can be read using the :py:func:`~crema.read_txt()`.
 
 Once read, a collection of PSMs is stored in a :py:class:`~crema.dataset.PsmDataset` object.
 Calling the :py:func:`~crema.assign_confidence()` function will calculate confidence estimates
 for the respective psm data using the specified confidence estimate method.
 
@@ -39,15 +39,19 @@
     assign_confidence
 
 Parsers
 *****************
 .. autosummary::
     :nosignatures:
 
-    read_crux
+    read_tide
+    read_msamanda
+    read_msfragger
+    read_msgf
+    read_pepxml
     read_mztab
     read_txt
 
 Writers
 *****************
 .. autosummary::
     :nosignatures:
@@ -59,15 +63,15 @@
 .. currentmodule:: crema.dataset
 .. autosummary::
     :nosignatures:
 
     PsmDataset
 
 Confidence
----------
+----------
 .. currentmodule:: crema.confidence
 .. autosummary::
     :nosignatures:
 
     Confidence
```

### Comparing `crema-ms-0.0.5/docs/cli.rst` & `crema-ms-0.0.8/docs/cli.rst`

 * *Files 8% similar despite different names*

```diff
@@ -10,13 +10,17 @@
 ---------
 There will be three output files:
 
 #. A txt file named "crema.psms.txt" containing an additional column (crema q-value) of psm level confidence estimate results appended to the spectrum, peptide, and score columns from the input file.
 
 #. A txt file named "crema.peptides.txt" containing an additional column (crema q-value) of peptide level confidence estimate results appended to the spectrum, peptide, and score columns from the input file.
 
-#. A txt file named "crema.log.txt" containing the logging information from using crema.
+#. A txt file named "crema.proteins.txt" containing an additional column (crema
+q-value) of protein level confidence estimate results appended to the protein id
+and score columns from the input file.
+
+#. A txt file named "crema.log.txt" containing the logging information from using crema. Note that this file is only created when running Crema through via the command line.
 
 Note that the program writes to the current working directory by default:
 
 * The name of the output directory can be specified using the ---output_dir argument.
-* A prefix can be added to the output file names be using the ---file_root argument.
+* A prefix can be added to the output file names be using the ---file_root argument.
```

### Comparing `crema-ms-0.0.5/docs/conf.py` & `crema-ms-0.0.8/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 except ModuleNotFoundError:
     subprocess.run(["pip", "install", "numpydoc"], check=True)
 
 
 # -- Project information -----------------------------------------------------
 project = "crema"
 copyright = "2020, Donavan See"
-author = "William E. Fondrie, Donavan See, William S. Noble"
+author = "Andy Lin, William E. Fondrie, Donavan See, William S. Noble"
 version = str(crema.__version__)
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
@@ -43,15 +43,14 @@
     "sphinx.ext.coverage",
     "sphinx.ext.viewcode",
     "numpydoc",
     "sphinx_rtd_theme",
     "sphinx.ext.intersphinx",
     "sphinxarg.ext",
     "nbsphinx",
-    "myst_parser",
 ]
 
 nbsphinx_execute = "never"
 
 autosummary_generate = True
 autodoc_default_options = {
     "members": True,
```

### Comparing `crema-ms-0.0.5/docs/index.rst` & `crema-ms-0.0.8/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 package manager.
 
 crema also depends on several Python packages:
 
 - `numba <http://numba.pydata.org/>`_
 - `numpy <https://numpy.org/>`_
 - `pandas <https://pandas.pydata.org/>`_
+- `lxml <https://lxml.de/>`_
 - `pyteomics <https://pyteomics.readthedocs.io/en/latest/>`_
 
 
 
 
 We recommend using `pip` to install crema. Missing dependencies will also
 be installed automatically:
@@ -69,51 +70,54 @@
    $ pip3 install crema-ms
 
 Basic Usage
 -----------
 Use **crema** from the Command Line
 ###################################
 
-If your input files are in the mzTab or Crux tab-delimited formats, then simple crema analyses can be performed
+If your input files are in a file format that is supported, such mzTab or
+Tide tab-delimited, then simple crema analyses can be performed
 straight from the command line!
 
 Suppose your mzTab file is located at the directory "data/psms.mztab". Simply run the following command:
 
 .. code-block:: bash
 
    $ crema data/psms.mztab
 
-Suppose your Crux files are located at the directory "data/target_psms.txt" and "data/decoy_psms.txt".
+Suppose your Tide files are located at the directory "data/target_psms.txt" and "data/decoy_psms.txt".
 Simply run the following command:
 
 .. code-block:: bash
 
    $ crema data/target_psms.txt data/decoy_psms.txt
 
 That's it. The software will then run the target-decoy competition FDR estimation method using information from these columns
 to calculate confidence estimates for the given data.
 
-Your results will be saved in your working directory as .txt files named "crema.psms.txt" and "crema.peptides.txt".
+Your results will be saved in your working directory as .txt files named
+"crema.psms.txt", "crema.peptides.txt", and "crema.proteins.txt".
 These files will contain an additional column ("crema q-value") that is appended to several columns
 (specifically those that identify the psm, peptide sequence, and score) parsed from the input file.
 
 For a full list of parameters, see the :doc:`Command Line Interface <cli>`.
 
-Use **crema** as a Python package
+Use **crema** as a Python Package
 ###################################
 
 Here is a simple demonstration of how to use crema as an API:
 
 .. code-block:: Python
 
     >>> import crema
     >>> input_files = ["data/target_psms.txt", "decoy_psms/decoys.txt"]
-    >>> psms = crema.read_crux(input_files)
-    >>> results =  psms.assign_confidence(score_column="combined p-value", desc=True, eval_fdr=0.01, method="tdc")
-    >>> results.to_txt(ouput_dir="example_output_dir", file_root="test", sep="\t", decoys=False)
+    >>> pairing_file = "pairing_file.txt"
+    >>> psms = crema.read_tide(input_files, pairing_file_name=pairing_file)
+    >>> results =  psms.assign_confidence(score_column="combined p-value", pep_fdr_type="psm-peptide")
+    >>> results.to_txt(output_dir="example_output_dir", file_root="test", sep="\t", decoys=False)
 
 Let's break this down and see what's really happening.
 
 First, start up the Python interpreter:
 
 .. code-block:: bash
 
@@ -121,43 +125,67 @@
 
 Next, import crema as a package:
 
 .. code-block:: Python
 
    >>> import crema
 
-Call the :doc:`read_crux() <api/functions>` method and pass in the desired input files. Note that
-the files "data/target_psms.txt" and "data/decoy_psms.txt" are already in the required Crux file
-format. The :doc:`read_crux() <api/functions>` method will return a :doc:`dataset <api/dataset>` object
+Call the :doc:`read_tide() <api/functions>` method and pass in the desired input
+files. The files "data/target_psms.txt" and "data/decoy_psms.txt" contais PSMs
+and are in the required Tide file format. In addition, the pairing_file is an
+optional argument that explicitly pairs target and decoy peptides.
+The :doc:`read_tide() <api/functions>` method will return a :doc:`dataset <api/dataset>` object
 that we will save as "psms" in this example:
 
 .. code-block:: Python
 
    >>> input_files = ["data/target_psms.txt", "decoy_psms/decoys.txt"]
-   >>> psms = crema.read_crux(input_files)
+   >>> pairing_file = "pairing_file.txt"
+   >>> psms = crema.read_tide(input_files. pairing_file_name=pairing_file)
+
+Note that you can replace :doc:`read_tide() <api/functions>` with other methods
+such as :doc:`read_txt() <api/functions>` and :doc:`read_msgf()
+<api/functions>`.
 
 Execute the desired FDR estimation method by calling the :doc:`assign_confidence <api/functions>` method on
 the dataset object that we created above.
 This operation will return a :doc:`confidence <api/confidence>` object that we will save as "results":
 
 .. code-block:: Python
 
-   >>> results =  psms.assign_confidence(score_column="combined p-value", desc=True, eval_fdr=0.01, method="tdc")
+   >>> results =  psms.assign_confidence(score_column="combined p-value", pep_fdr_type="psm-peptide")
 
 Note: The parameters passed here are optional and are only specified here for
-demonstration. Further details can be found in the documentation for the :doc:`dataset <api/dataset>` class.
+demonstration. Further details can be found in the documentation for the
+:doc:`dataset <api/dataset>` class.
+
+Note: The pep_fdr_type argument denotes the method used to estimate peptide-level
+FDR. There are 3 options: psm-only, peptide-only, and psm-peptide. A pairing
+file is required to run the peptide-only and psm-peptide. Also, note that
+peptide-only requires a separate target and decoy database search. If
+peptide-only is used in conjunction with a concatenated target-decoy search, then
+it becomes equivalent to the psm-peptide.
 
 Confidence objects contain a :doc:`to_txt() <api/confidence>` method that allows you to write your results to a txt file.
 Your results will be saved in your working directory (unless otherwise specified)
-as .txt files named "crema.psms.txt" and "crema.peptides.txt".
+as .txt files named "crema.psms.txt", "crema.peptides.txt", and
+"crema.proteins.txt".
 These files will contain an additional column ("crema q-value") that is appended to several columns
 (specifically those that identify the psm, peptide sequence, and score) parsed from the input file.
 
 .. code-block:: Python
 
-   >>> results.to_txt(ouput_dir="example_output_dir", file_root=None, sep="\t", decoys=False)
+   >>> results.to_txt(output_dir="example_output_dir", file_root=None, sep="\t", decoys=False)
 
 Note: The parameters passed here are optional and are only specified here for
 demonstration. Further details can be found in the documentation for the :doc:`confidence <api/confidence>` class.
 
 That's all there is to it! You have successfully used crema as an API to
-calculate confidence estimates for your data.
+calculate confidence estimates for your data.
+
+Supported Database Search Engines
+###################################
+
+crema currently supports output generated from Tide, MSGF+, MSAmanda, Comet, MSFragger.
+
+In addition, crema supports input files, from any search engine, that are in the
+follow file formats: mzTab, pepXML, and generic delmited text files.
```

### Comparing `crema-ms-0.0.5/docs/make.bat` & `crema-ms-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/pyproject.toml` & `crema-ms-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/setup.cfg` & `crema-ms-0.0.8/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = crema-ms
-author = William E. Fondrie
-author_email = fondriew@gmail.com
+author = Andy Lin
+author_email = linandy@uw.edu
 description = Confidence estimation for proteomics experiments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/noble-lab/crema
 project_urls = 
 	Documentation = https://crema-ms.readthedocs.io
 	Bug Tracker = https://github.com/noble-lab/crema/issues
@@ -17,17 +17,18 @@
 	Topic :: Scientific/Engineering :: Bio-Informatics
 
 [options]
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy>=1.18.1
-	pandas>=1.0.3
+	pandas>=1.3.0
 	numba>=0.48.0
 	pyteomics>=4.4.2
+	lxml>=4.6.3
 
 [options.extras_require]
 docs = 
 	numpydoc>=1.0.0
 	sphinx-argparse>=0.2.5
 	sphinx-rtd-theme>=0.5.0
 	nbsphinx>=0.7.1
```

### Comparing `crema-ms-0.0.5/static/crema_logo.svg` & `crema-ms-0.0.8/static/crema_logo.svg`

 * *Files identical despite different names*

### Comparing `crema-ms-0.0.5/tests/system_tests/test_cli.py` & `crema-ms-0.0.8/tests/system_tests/test_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 """These tests verify that the crema CLI works as expected."""
 from pathlib import Path
 import subprocess
 
 
-def test_cli_basic(basic_crux_txt, tmp_path):
+def test_cli_basic(basic_tide_txt, tmp_path):
     """Test that the basic cli works."""
-    cmd = ["crema", "--output_dir", tmp_path, "-e", "0.5", basic_crux_txt]
+    cmd = ["crema", "--output_dir", tmp_path, "-e", "0.5", basic_tide_txt]
     subprocess.run(cmd, check=True)
     assert Path(tmp_path, "crema.psms.txt").exists()
+    assert Path(tmp_path, "crema.peptides.txt").exists()
+    assert Path(tmp_path, "crema.proteins.txt").exists()
     assert Path(tmp_path, "crema.log.txt").exists()
 
 
-def test_cli_custom_root(basic_crux_txt, tmp_path):
+def test_cli_custom_root(basic_tide_txt, tmp_path):
     """Test that the cli works with custom file root."""
     cmd = ["crema", "-o", tmp_path, "-f", "myFileRoot", "-e", "0.5"]
-    cmd.append(basic_crux_txt)
+    cmd.append(basic_tide_txt)
     subprocess.run(cmd, check=True)
     assert Path(tmp_path, "myFileRoot.crema.psms.txt").exists()
+    assert Path(tmp_path, "myFileRoot.crema.peptides.txt").exists()
+    assert Path(tmp_path, "myFileRoot.crema.proteins.txt").exists()
     assert Path(tmp_path, "myFileRoot.crema.log.txt").exists()
 
 
-def test_real(real_crux_txt, tmp_path):
+def test_real(real_tide_txt, tmp_path):
     """Test that crema works on real Crux results"""
-    cmd = ["crema", "--output_dir", tmp_path] + list(real_crux_txt)
+    cmd = ["crema", "--output_dir", tmp_path] + list(real_tide_txt)
     subprocess.run(cmd, check=True)
     assert Path(tmp_path, "crema.psms.txt").exists()
+    assert Path(tmp_path, "crema.peptides.txt").exists()
+    assert Path(tmp_path, "crema.proteins.txt").exists()
     assert Path(tmp_path, "crema.log.txt").exists()
```

### Comparing `crema-ms-0.0.5/tests/unit_tests/test_dataset.py` & `crema-ms-0.0.8/tests/unit_tests/test_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,63 +5,74 @@
 import numpy as np
 import pandas as pd
 
 from crema import PsmDataset
 
 
 @pytest.fixture
-def simple_df(basic_crux_df):
+def simple_df(basic_tide_df):
     """A simple dataframe of PSMs"""
-    df = basic_crux_df
+    df = basic_tide_df
     df["target"] = df["target/decoy"].replace({"target": True, "decoy": False})
     return df.drop(columns="target/decoy")
 
 
 def test_create_object(simple_df):
     """Ensures that a PsmDataset object can be initialized properly."""
     psms = PsmDataset(
         psms=simple_df,
         target_column="target",
-        spectrum_columns=["scan", "spectrum precursor m/z"],
+        spectrum_columns=["file", "scan"],
         score_columns=["combined p-value", "x"],
         peptide_column="sequence",
+        protein_column="protein id",
+        protein_delim=",",
     )
     assert isinstance(psms, PsmDataset)
 
 
 def test_properties(simple_df):
     """Check the public properties of the PsmDataset object."""
     psms = PsmDataset(
         psms=simple_df,
         target_column="target",
-        spectrum_columns=["scan", "spectrum precursor m/z"],
+        spectrum_columns=["file", "scan"],
         score_columns=["combined p-value", "x"],
         peptide_column="sequence",
+        protein_column="protein id",
+        protein_delim=",",
     )
 
-    pd.testing.assert_frame_equal(psms.data, simple_df, check_like=True)
-    assert list(psms.spectra.columns) == ["scan", "spectrum precursor m/z"]
+    # TODO remove after Will code review
+    # This is not true anymore because columns are used as input that
+    # are not found in output (namely "original target sequence).
+    # pd.testing.assert_frame_equal(psms.data, simple_df, check_like=True)
+    assert list(psms.spectra.columns) == ["file", "scan"]
     assert psms.score_columns == ["combined p-value", "x"]
     assert psms.peptides.name == "sequence"
+    assert psms.proteins.name == "protein id"
+    assert psms._protein_delim == ","
     pd.testing.assert_frame_equal(
         psms.scores, simple_df.loc[:, ["combined p-value", "x"]]
     )
     np.testing.assert_array_equal(
         psms.targets, simple_df.loc[:, "target"].values
     )
 
 
 def test_getitem(simple_df):
     """Test the __getitem__ method"""
     psms = PsmDataset(
         psms=simple_df,
         target_column="target",
-        spectrum_columns=["scan", "spectrum precursor m/z"],
+        spectrum_columns=["file", "scan"],
         score_columns=["combined p-value", "x"],
         peptide_column="sequence",
+        protein_column="protein id",
+        protein_delim=",",
     )
 
     pd.testing.assert_series_equal(psms["scan"], simple_df["scan"])
     pd.testing.assert_series_equal(
         psms["combined p-value"],
         simple_df["combined p-value"],
     )
@@ -71,13 +82,15 @@
     """Test the find_best_score() method"""
     psms = PsmDataset(
         psms=simple_df,
         target_column="target",
         spectrum_columns=["scan", "spectrum precursor m/z"],
         score_columns=["combined p-value", "x"],
         peptide_column="sequence",
+        protein_column="protein id",
+        protein_delim=",",
     )
 
     score, npass, desc = psms.find_best_score(eval_fdr=0.4)
     assert score == "x"
     assert npass == 4
     assert desc
```

