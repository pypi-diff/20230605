# Comparing `tmp/bomf-0.5.2.tar.gz` & `tmp/bomf-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.5.2.tar", last modified: Mon Jun  5 13:29:08 2023, max compression
+gzip compressed data, was "bomf-0.5.3.tar", last modified: Mon Jun  5 13:29:40 2023, max compression
```

## Comparing `bomf-0.5.2.tar` & `bomf-0.5.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.937340 bomf-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.933340 bomf-0.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-05 13:28:59.000000 bomf-0.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.933340 bomf-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-05 13:28:59.000000 bomf-0.5.2/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-05 13:28:59.000000 bomf-0.5.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 13:28:59.000000 bomf-0.5.2/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-05 13:28:59.000000 bomf-0.5.2/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-05 13:28:59.000000 bomf-0.5.2/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-05 13:28:59.000000 bomf-0.5.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-05 13:28:59.000000 bomf-0.5.2/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-05 13:28:59.000000 bomf-0.5.2/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-05 13:28:59.000000 bomf-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-05 13:28:59.000000 bomf-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-05 13:28:59.000000 bomf-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-05 13:29:08.937340 bomf-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-05 13:28:59.000000 bomf-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-05 13:28:59.000000 bomf-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 13:28:59.000000 bomf-0.5.2/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 13:28:59.000000 bomf-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-05 13:29:08.941340 bomf-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-05 13:28:59.000000 bomf-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.929340 bomf-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.933340 bomf-0.5.2/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.933340 bomf-0.5.2/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.933340 bomf-0.5.2/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.933340 bomf-0.5.2/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.937340 bomf-0.5.2/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.937340 bomf-0.5.2/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.937340 bomf-0.5.2/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.937340 bomf-0.5.2/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-05 13:28:59.000000 bomf-0.5.2/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.933340 bomf-0.5.2/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-05 13:29:08.000000 bomf-0.5.2/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-05 13:29:08.000000 bomf-0.5.2/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:29:08.000000 bomf-0.5.2/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:29:08.000000 bomf-0.5.2/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 13:29:08.000000 bomf-0.5.2/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 13:29:08.000000 bomf-0.5.2/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-05 13:28:59.000000 bomf-0.5.2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:08.937340 bomf-0.5.2/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-05 13:28:59.000000 bomf-0.5.2/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 13:28:59.000000 bomf-0.5.2/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-05 13:28:59.000000 bomf-0.5.2/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-05 13:28:59.000000 bomf-0.5.2/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-05 13:28:59.000000 bomf-0.5.2/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-05 13:28:59.000000 bomf-0.5.2/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-05 13:28:59.000000 bomf-0.5.2/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-05 13:28:59.000000 bomf-0.5.2/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-06-05 13:28:59.000000 bomf-0.5.2/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.451995 bomf-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.447995 bomf-0.5.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-05 13:29:33.000000 bomf-0.5.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.447995 bomf-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-05 13:29:33.000000 bomf-0.5.3/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-05 13:29:33.000000 bomf-0.5.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 13:29:33.000000 bomf-0.5.3/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-05 13:29:33.000000 bomf-0.5.3/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-05 13:29:33.000000 bomf-0.5.3/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-05 13:29:33.000000 bomf-0.5.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-05 13:29:33.000000 bomf-0.5.3/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-05 13:29:33.000000 bomf-0.5.3/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-05 13:29:33.000000 bomf-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-05 13:29:33.000000 bomf-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-05 13:29:33.000000 bomf-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-05 13:29:40.451995 bomf-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-05 13:29:33.000000 bomf-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-05 13:29:33.000000 bomf-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 13:29:33.000000 bomf-0.5.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 13:29:33.000000 bomf-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-05 13:29:40.451995 bomf-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-05 13:29:33.000000 bomf-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.447995 bomf-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.447995 bomf-0.5.3/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.447995 bomf-0.5.3/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.447995 bomf-0.5.3/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.447995 bomf-0.5.3/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.447995 bomf-0.5.3/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.451995 bomf-0.5.3/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.451995 bomf-0.5.3/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.451995 bomf-0.5.3/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-05 13:29:33.000000 bomf-0.5.3/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.447995 bomf-0.5.3/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-05 13:29:40.000000 bomf-0.5.3/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-05 13:29:40.000000 bomf-0.5.3/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:29:40.000000 bomf-0.5.3/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:29:40.000000 bomf-0.5.3/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 13:29:40.000000 bomf-0.5.3/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 13:29:40.000000 bomf-0.5.3/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-05 13:29:33.000000 bomf-0.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:29:40.451995 bomf-0.5.3/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-05 13:29:33.000000 bomf-0.5.3/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 13:29:33.000000 bomf-0.5.3/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-05 13:29:33.000000 bomf-0.5.3/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-05 13:29:33.000000 bomf-0.5.3/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-05 13:29:33.000000 bomf-0.5.3/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-05 13:29:33.000000 bomf-0.5.3/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-05 13:29:33.000000 bomf-0.5.3/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-05 13:29:33.000000 bomf-0.5.3/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-06-05 13:29:33.000000 bomf-0.5.3/unittests/test_validation.py
```

### Comparing `bomf-0.5.2/.github/dependabot.yml` & `bomf-0.5.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/.github/workflows/black.yml` & `bomf-0.5.3/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/.github/workflows/codeql-analysis.yml` & `bomf-0.5.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/.github/workflows/coverage.yml` & `bomf-0.5.3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/.github/workflows/packaging_test.yml` & `bomf-0.5.3/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/.github/workflows/python-publish.yml` & `bomf-0.5.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/.github/workflows/pythonlint.yml` & `bomf-0.5.3/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/.github/workflows/unittests.yml` & `bomf-0.5.3/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/.gitignore` & `bomf-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/.pre-commit-config.yaml` & `bomf-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/LICENSE` & `bomf-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/PKG-INFO` & `bomf-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.2
+Version: 0.5.3
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.2/README.md` & `bomf-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/pyproject.toml` & `bomf-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/requirements.txt` & `bomf-0.5.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/setup.cfg` & `bomf-0.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/__init__.py` & `bomf-0.5.3/src/bomf/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,92 +56,93 @@
         """
         a mapper that transforms bo4e data sets to a structure that suits the target system
         """
         self.target_loader: EntityLoader[TargetDataModel] = target_loader
         """
         The target loader moves the target entities into the actual target system.
         """
+        self.logger = logging.getLogger(self.__class__.__name__)
+        """
+        Class logger
+        """
 
     async def _map_to_target_validate_and_load(self, bo4e_datasets: list[IntermediateDataSet]) -> list[LoadingSummary]:
         """
         This method encapsulates the steps:
         1. validation
         2. mapping intermediate models to target
         3. load to target system.
         They have been encapsulated because they're used by both the migrate and migrate_paginated methods.
         """
-        logger = logging.getLogger(self.__class__.__name__)
         if self.validation_manager is not None:
-            logger.info("Applying validation rules to %i bo4e data sets", len(bo4e_datasets))
+            self.logger.info("Applying validation rules to %i bo4e data sets", len(bo4e_datasets))
             validation_result = await self.validation_manager.validate(*bo4e_datasets)
-            logger.info(
+            self.logger.info(
                 "Creating target models from those %i datasets that passed the validation",
                 len(validation_result.succeeded_data_sets),
             )
             target_data_models = await self.bo4e_to_target_mapper.create_target_models(
                 validation_result.succeeded_data_sets
             )
         else:
-            logger.warning("No validation set; skipping validation")
-            logger.info("Creating target models from all %i datasets", len(bo4e_datasets))
+            self.logger.warning("No validation set; skipping validation")
+            self.logger.info("Creating target models from all %i datasets", len(bo4e_datasets))
             target_data_models = await self.bo4e_to_target_mapper.create_target_models(bo4e_datasets)
-        logger.info("Loading %i target models into target system", len(target_data_models))
+        self.logger.info("Loading %i target models into target system", len(target_data_models))
         loading_summaries = await self.target_loader.load_entities(target_data_models)
         success_count, failure_count = _get_success_failure_count(loading_summaries)
-        logger.info("Loaded %i entities successfully, %i failed", success_count, failure_count)
+        self.logger.info("Loaded %i entities successfully, %i failed", success_count, failure_count)
         return loading_summaries
 
     async def migrate(self) -> list[LoadingSummary]:
         """
         run the entire migration flow from source to target which includes:
         1. create bo4e data source using the source_data_set_to_bo4e_mapper
         2. checking that all the bo4e data sets obey the validation rules
         3. mapping from bo4e to the target data model
         4. loading the target data models into the target system.
         """
         # todo: here we should add some logging and statistics stuff
-        logger = logging.getLogger(self.__class__.__name__)
-        logger.info("Starting migration %s (w/o pagination)", self.__class__.__name__)
+        self.logger.info("Starting migration %s (w/o pagination)", self.__class__.__name__)
         bo4e_datasets = await self.source_data_to_bo4e_mapper.create_data_sets()
         loading_summaries = await self._map_to_target_validate_and_load(bo4e_datasets)
         return loading_summaries
 
     async def migrate_paginated(self, chunk_size: int) -> list[LoadingSummary]:
         """
         This is similar to migrate, but it loads the data in chunks of chunk_size.
         Therefore, the source_data_to_bo4e_mapper must support pagination.
         """
-        logger = logging.getLogger(self.__class__.__name__)
-        logger.info("Starting migration %s (with page size %i)", self.__class__.__name__, chunk_size)
+        self.logger.info("Starting migration %s (with page size %i)", self.__class__.__name__, chunk_size)
         offset = 0
         loading_summaries = []
         while True:
-            logger.info("Processing offset=%i, limit=%i", offset, chunk_size)
+            self.logger.info("Processing offset=%i, limit=%i", offset, chunk_size)
             try:
                 bo4e_datasets = await self.source_data_to_bo4e_mapper.create_data_sets(
                     limit=chunk_size, offset=offset
                 )  # this might raise an PaginationNotSupportedException
             except TypeError as type_error:
                 error_message = str(type_error)
                 if (
                     "got an unexpected keyword argument 'limit'" in error_message
                     or "got an unexpected keyword argument 'offset'" in error_message
                 ):
                     # this case should be prevented by the type checker already
                     raise PaginationNotSupportedException() from type_error
                 raise
-            logger.debug("Received %i datasets (limit was %i)", len(bo4e_datasets), chunk_size)
+            self.logger.debug("Received %i datasets (limit was %i)", len(bo4e_datasets), chunk_size)
             if len(bo4e_datasets) == 0:
-                logger.info("Received no more datasets; Stopping")
+                self.logger.info("Received no more datasets; Stopping")
                 break
             chunk_loading_summaries = await self._map_to_target_validate_and_load(bo4e_datasets)
             loading_summaries.extend(chunk_loading_summaries)
             await asyncio.sleep(1)  # give the system 1s some time to breathe
             offset += chunk_size
         success_count, failure_count = _get_success_failure_count(loading_summaries)
-        logger.info(
+        self.logger.info(
             "Finished paginated migration. In total we loaded %i entities out of which %i succeeded and %i failed",
             len(loading_summaries),
             success_count,
             failure_count,
         )
         return loading_summaries
```

### Comparing `bomf-0.5.2/src/bomf/filter/__init__.py` & `bomf-0.5.3/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.5.3/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/loader/entityloader.py` & `bomf-0.5.3/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/mapper/__init__.py` & `bomf-0.5.3/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/model/__init__.py` & `bomf-0.5.3/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/provider/__init__.py` & `bomf-0.5.3/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/validation/core/analysis.py` & `bomf-0.5.3/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/validation/core/errors.py` & `bomf-0.5.3/src/bomf/validation/core/errors.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/validation/core/execution.py` & `bomf-0.5.3/src/bomf/validation/core/execution.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/validation/core/types.py` & `bomf-0.5.3/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/validation/core/utils.py` & `bomf-0.5.3/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/validation/core/validator.py` & `bomf-0.5.3/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/validation/path_map.py` & `bomf-0.5.3/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/validation/query_map.py` & `bomf-0.5.3/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf/validation/utils.py` & `bomf-0.5.3/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/src/bomf.egg-info/PKG-INFO` & `bomf-0.5.3/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.2
+Version: 0.5.3
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.2/src/bomf.egg-info/SOURCES.txt` & `bomf-0.5.3/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/tox.ini` & `bomf-0.5.3/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/unittests/test_bo4e_data_set.py` & `bomf-0.5.3/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/unittests/test_entity_loader.py` & `bomf-0.5.3/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/unittests/test_filter.py` & `bomf-0.5.3/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/unittests/test_mapper.py` & `bomf-0.5.3/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/unittests/test_migration.py` & `bomf-0.5.3/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/unittests/test_source_data_provider.py` & `bomf-0.5.3/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.2/unittests/test_validation.py` & `bomf-0.5.3/unittests/test_validation.py`

 * *Files identical despite different names*

