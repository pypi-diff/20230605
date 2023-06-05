# Comparing `tmp/pyauxlib-0.0.0.tar.gz` & `tmp/pyauxlib-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyauxlib-0.0.0.tar", last modified: Thu Jun  1 03:11:49 2023, max compression
+gzip compressed data, was "pyauxlib-0.0.1.tar", last modified: Mon Jun  5 01:35:10 2023, max compression
```

## Comparing `pyauxlib-0.0.0.tar` & `pyauxlib-0.0.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.815620 pyauxlib-0.0.0/
--rw-rw-rw-   0        0        0      761 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0     2070 2023-06-01 02:11:47.000000 pyauxlib-0.0.0/.cookiecutterrc
--rw-rw-rw-   0        0        0      192 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/.coveragerc
--rw-rw-rw-   0        0        0      373 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.492821 pyauxlib-0.0.0/.github/
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.616620 pyauxlib-0.0.0/.github/workflows/
--rw-rw-rw-   0        0        0     2012 2023-06-01 02:11:47.000000 pyauxlib-0.0.0/.github/workflows/github-actions.yml
--rw-rw-rw-   0        0        0      714 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      241 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/.readthedocs.yml
--rw-rw-rw-   0        0        0       79 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0       94 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     2403 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1538 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      449 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1818 2023-06-01 03:11:49.813621 pyauxlib-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2253 2023-06-01 02:11:47.000000 pyauxlib-0.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.625627 pyauxlib-0.0.0/ci/
--rw-rw-rw-   0        0        0     2950 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/ci/bootstrap.py
--rw-rw-rw-   0        0        0       78 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/ci/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.495824 pyauxlib-0.0.0/ci/templates/
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.496762 pyauxlib-0.0.0/ci/templates/.github/
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.629620 pyauxlib-0.0.0/ci/templates/.github/workflows/
--rw-rw-rw-   0        0        0     2195 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/ci/templates/.github/workflows/github-actions.yml
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.676621 pyauxlib-0.0.0/docs/
--rw-rw-rw-   0        0        0       29 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/authors.rst
--rw-rw-rw-   0        0        0       31 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/changelog.rst
--rw-rw-rw-   0        0        0     1193 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/contributing.rst
--rw-rw-rw-   0        0        0      265 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/index.rst
--rw-rw-rw-   0        0        0       95 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/installation.rst
--rw-rw-rw-   0        0        0       28 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/readme.rst
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.684620 pyauxlib-0.0.0/docs/reference/
--rw-rw-rw-   0        0        0       67 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/reference/index.rst
--rw-rw-rw-   0        0        0      111 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/reference/pyauxlib.rst
--rw-rw-rw-   0        0        0       31 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/requirements.txt
--rw-rw-rw-   0        0        0      120 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/spelling_wordlist.txt
--rw-rw-rw-   0        0        0       75 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/docs/usage.rst
--rw-rw-rw-   0        0        0     1209 2023-06-01 03:03:31.000000 pyauxlib-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      801 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/pytest.ini
--rw-rw-rw-   0        0        0       42 2023-06-01 03:11:49.816621 pyauxlib-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2097 2023-06-01 03:04:45.000000 pyauxlib-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.500752 pyauxlib-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.688620 pyauxlib-0.0.0/src/pyauxlib/
--rw-rw-rw-   0        0        0      153 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.724622 pyauxlib-0.0.0/src/pyauxlib/callables/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/callables/__init__.py
--rw-rw-rw-   0        0        0     3128 2023-06-01 03:06:01.000000 pyauxlib-0.0.0/src/pyauxlib/callables/callables.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.733620 pyauxlib-0.0.0/src/pyauxlib/decorators/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/decorators/__init__.py
--rw-rw-rw-   0        0        0      349 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/decorators/timing.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.757630 pyauxlib-0.0.0/src/pyauxlib/experimental/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/experimental/__init__.py
--rw-rw-rw-   0        0        0     4595 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/experimental/decorator.py
--rw-rw-rw-   0        0        0     1035 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/experimental/get_caller_path.py
--rw-rw-rw-   0        0        0      694 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/experimental/kwargs.py
--rw-rw-rw-   0        0        0     1333 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/experimental/lists.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.775623 pyauxlib-0.0.0/src/pyauxlib/io/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/io/__init__.py
--rw-rw-rw-   0        0        0     5310 2023-06-01 03:06:01.000000 pyauxlib-0.0.0/src/pyauxlib/io/filesfolders.py
--rw-rw-rw-   0        0        0      443 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/io/utils.py
--rw-rw-rw-   0        0        0     1854 2023-06-01 02:11:46.000000 pyauxlib-0.0.0/src/pyauxlib/io/yamlio.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.802620 pyauxlib-0.0.0/src/pyauxlib/utils/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:11:47.000000 pyauxlib-0.0.0/src/pyauxlib/utils/__init__.py
--rw-rw-rw-   0        0        0     1111 2023-06-01 02:11:47.000000 pyauxlib-0.0.0/src/pyauxlib/utils/deprecations.py
--rw-rw-rw-   0        0        0     1464 2023-06-01 02:11:47.000000 pyauxlib-0.0.0/src/pyauxlib/utils/dictionaries.py
--rw-rw-rw-   0        0        0     2559 2023-06-01 02:11:47.000000 pyauxlib-0.0.0/src/pyauxlib/utils/encoding.py
--rw-rw-rw-   0        0        0     3897 2023-06-01 02:11:47.000000 pyauxlib-0.0.0/src/pyauxlib/utils/logger.py
--rw-rw-rw-   0        0        0     5422 2023-06-01 02:11:47.000000 pyauxlib-0.0.0/src/pyauxlib/utils/timer.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.717634 pyauxlib-0.0.0/src/pyauxlib.egg-info/
--rw-rw-rw-   0        0        0     1818 2023-06-01 03:11:49.000000 pyauxlib-0.0.0/src/pyauxlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1476 2023-06-01 03:11:49.000000 pyauxlib-0.0.0/src/pyauxlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 03:11:49.000000 pyauxlib-0.0.0/src/pyauxlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-01 03:11:33.000000 pyauxlib-0.0.0/src/pyauxlib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-06-01 03:11:49.000000 pyauxlib-0.0.0/src/pyauxlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 03:11:49.000000 pyauxlib-0.0.0/src/pyauxlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 03:11:49.809626 pyauxlib-0.0.0/tests/
--rw-rw-rw-   0        0        0      598 2023-06-01 02:11:47.000000 pyauxlib-0.0.0/tests/test_pyauxlib.py
--rw-rw-rw-   0        0        0     1404 2023-06-01 03:01:15.000000 pyauxlib-0.0.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.503582 pyauxlib-0.0.1/
+-rw-rw-rw-   0        0        0      761 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/.bumpversion.cfg
+-rw-rw-rw-   0        0        0     2007 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/.cookiecutterrc
+-rw-rw-rw-   0        0        0      192 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/.coveragerc
+-rw-rw-rw-   0        0        0      373 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.235581 pyauxlib-0.0.1/.github/
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.326579 pyauxlib-0.0.1/.github/workflows/
+-rw-rw-rw-   0        0        0     2012 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/.github/workflows/github-actions.yml
+-rw-rw-rw-   0        0        0      714 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      241 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/.readthedocs.yml
+-rw-rw-rw-   0        0        0       79 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0       94 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     2403 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1538 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0      449 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1818 2023-06-05 01:35:10.500581 pyauxlib-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2253 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.336584 pyauxlib-0.0.1/ci/
+-rw-rw-rw-   0        0        0     2950 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/ci/bootstrap.py
+-rw-rw-rw-   0        0        0       78 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/ci/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.239581 pyauxlib-0.0.1/ci/templates/
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.239581 pyauxlib-0.0.1/ci/templates/.github/
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.341581 pyauxlib-0.0.1/ci/templates/.github/workflows/
+-rw-rw-rw-   0        0        0     2195 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/ci/templates/.github/workflows/github-actions.yml
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.380580 pyauxlib-0.0.1/docs/
+-rw-rw-rw-   0        0        0       29 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/authors.rst
+-rw-rw-rw-   0        0        0       31 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1193 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0      265 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/index.rst
+-rw-rw-rw-   0        0        0       95 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/installation.rst
+-rw-rw-rw-   0        0        0       28 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/readme.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.388582 pyauxlib-0.0.1/docs/reference/
+-rw-rw-rw-   0        0        0       67 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/reference/index.rst
+-rw-rw-rw-   0        0        0      111 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/reference/pyauxlib.rst
+-rw-rw-rw-   0        0        0       31 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/requirements.txt
+-rw-rw-rw-   0        0        0      120 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/spelling_wordlist.txt
+-rw-rw-rw-   0        0        0       75 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/usage.rst
+-rw-rw-rw-   0        0        0     1262 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      801 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/pytest.ini
+-rw-rw-rw-   0        0        0       42 2023-06-05 01:35:10.503582 pyauxlib-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2161 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.244581 pyauxlib-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.392580 pyauxlib-0.0.1/src/pyauxlib/
+-rw-rw-rw-   0        0        0      153 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/src/pyauxlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.422582 pyauxlib-0.0.1/src/pyauxlib/callables/
+-rw-rw-rw-   0        0        0        0 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/callables/__init__.py
+-rw-rw-rw-   0        0        0     3128 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/callables/callables.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.428580 pyauxlib-0.0.1/src/pyauxlib/decorators/
+-rw-rw-rw-   0        0        0        0 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/decorators/__init__.py
+-rw-rw-rw-   0        0        0      349 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/decorators/timing.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.448581 pyauxlib-0.0.1/src/pyauxlib/experimental/
+-rw-rw-rw-   0        0        0        0 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/experimental/__init__.py
+-rw-rw-rw-   0        0        0     4595 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/experimental/decorator.py
+-rw-rw-rw-   0        0        0     1035 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/experimental/get_caller_path.py
+-rw-rw-rw-   0        0        0      694 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/experimental/kwargs.py
+-rw-rw-rw-   0        0        0     1333 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/experimental/lists.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.465580 pyauxlib-0.0.1/src/pyauxlib/io/
+-rw-rw-rw-   0        0        0        0 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/io/__init__.py
+-rw-rw-rw-   0        0        0     5364 2023-06-02 09:44:05.000000 pyauxlib-0.0.1/src/pyauxlib/io/filesfolders.py
+-rw-rw-rw-   0        0        0      443 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/io/utils.py
+-rw-rw-rw-   0        0        0     1854 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/io/yamlio.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.491580 pyauxlib-0.0.1/src/pyauxlib/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/__init__.py
+-rw-rw-rw-   0        0        0     1111 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/deprecations.py
+-rw-rw-rw-   0        0        0     1464 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/dictionaries.py
+-rw-rw-rw-   0        0        0     2559 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/encoding.py
+-rw-rw-rw-   0        0        0     3897 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/logger.py
+-rw-rw-rw-   0        0        0     5422 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/timer.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.415581 pyauxlib-0.0.1/src/pyauxlib.egg-info/
+-rw-rw-rw-   0        0        0     1818 2023-06-05 01:35:09.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1476 2023-06-05 01:35:10.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 01:35:09.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-05 01:34:54.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2023-06-05 01:35:09.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 01:35:09.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.496580 pyauxlib-0.0.1/tests/
+-rw-rw-rw-   0        0        0      598 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/tests/test_pyauxlib.py
+-rw-rw-rw-   0        0        0     1476 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/tox.ini
```

### Comparing `pyauxlib-0.0.0/.bumpversion.cfg` & `pyauxlib-0.0.1/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.0
+current_version = 0.0.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `pyauxlib-0.0.0/.github/workflows/github-actions.yml` & `pyauxlib-0.0.1/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/.pre-commit-config.yaml` & `pyauxlib-0.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/CONTRIBUTING.rst` & `pyauxlib-0.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/LICENSE` & `pyauxlib-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/PKG-INFO` & `pyauxlib-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauxlib
-Version: 0.0.0
+Version: 0.0.1
 Summary: Auxiliary library for python.
 Home-page: https://github.com/psolsfer/pyauxlib
 Author: Pablo Solís Fernández
 Author-email: pablosolisfernandez@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyauxlib.readthedocs.io/
 Project-URL: Changelog, https://pyauxlib.readthedocs.io/en/latest/changelog.html
```

### Comparing `pyauxlib-0.0.0/README.rst` & `pyauxlib-0.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/pyauxlib
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pyauxlib.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/pyauxlib
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/psolsfer/pyauxlib/v0.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/psolsfer/pyauxlib/v0.0.1.svg
     :alt: Commits since latest release
-    :target: https://github.com/psolsfer/pyauxlib/compare/v0.0.0...main
+    :target: https://github.com/psolsfer/pyauxlib/compare/v0.0.1...main
 
 
 
 .. end-badges
 
 Auxiliary library for python.
```

### Comparing `pyauxlib-0.0.0/ci/bootstrap.py` & `pyauxlib-0.0.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/ci/templates/.github/workflows/github-actions.yml` & `pyauxlib-0.0.1/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/docs/conf.py` & `pyauxlib-0.0.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "PyAuxLib"
 year = "2023"
 author = "Pablo Solís Fernández"
 copyright = f"{year}, {author}"
-version = release = "0.0.0"
+version = release = "0.0.1"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/psolsfer/pyauxlib/issues/%s", "#"),
     "pr": ("https://github.com/psolsfer/pyauxlib/pull/%s", "PR #"),
 }
```

### Comparing `pyauxlib-0.0.0/pyproject.toml` & `pyauxlib-0.0.1/pyproject.toml`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-[build-system]
-requires = [
-    "setuptools>=30.3.0",
-    "wheel",
-]
-
-[tool.ruff.per-file-ignores]
-"ci/*" = ["S"]
-
-[tool.ruff]
-extend-exclude = ["static", "ci/templates"]
-ignore = [
-    "RUF001", # ruff-specific rules ambiguous-unicode-character-string
-    "S101", # flake8-bandit assert
-    "S308", # flake8-bandit suspicious-mark-safe-usage
-    "E501", # pycodestyle line-too-long
-]
-line-length = 140
-select = [
-    "B", # flake8-bugbear
-    "C4", # flake8-comprehensions
-    "DTZ", # flake8-datetimez
-    "E", # pycodestyle errors
-    "EXE", # flake8-executable
-    "F", # pyflakes
-    "I", # isort
-    "INT", # flake8-gettext
-    "PIE", # flake8-pie
-    "PLC", # pylint convention
-    "PLE", # pylint errors
-    "PT", # flake8-pytest-style
-    "PTH", # flake8-use-pathlib
-    "Q", # flake8-quotes
-    "RSE", # flake8-raise
-    "RUF", # ruff-specific rules
-    "S", # flake8-bandit
-    "UP", # pyupgrade
-    "W", # pycodestyle warnings
-]
-src = ["src", "tests"]
-target-version = "py310"
-
-[tool.ruff.flake8-pytest-style]
-fixture-parentheses = false
-mark-parentheses = false
-
-[tool.ruff.isort]
-forced-separate = ["conftest"]
-force-single-line = true
-
-[tool.black]
-line-length = 140
-target-version = ["py310"]
+[build-system]
+requires = [
+    "setuptools>=30.3.0",
+    "wheel",
+]
+
+[tool.ruff.per-file-ignores]
+"ci/*" = ["S"]
+
+[tool.ruff]
+extend-exclude = ["static", "ci/templates"]
+ignore = [
+    "RUF001", # ruff-specific rules ambiguous-unicode-character-string
+    "S101", # flake8-bandit assert
+    "S308", # flake8-bandit suspicious-mark-safe-usage
+    "E501", # pycodestyle line-too-long
+]
+line-length = 140
+select = [
+    "B", # flake8-bugbear
+    "C4", # flake8-comprehensions
+    "DTZ", # flake8-datetimez
+    "E", # pycodestyle errors
+    "EXE", # flake8-executable
+    "F", # pyflakes
+    "I", # isort
+    "INT", # flake8-gettext
+    "PIE", # flake8-pie
+    "PLC", # pylint convention
+    "PLE", # pylint errors
+    "PT", # flake8-pytest-style
+    "PTH", # flake8-use-pathlib
+    "Q", # flake8-quotes
+    "RSE", # flake8-raise
+    "RUF", # ruff-specific rules
+    "S", # flake8-bandit
+    "UP", # pyupgrade
+    "W", # pycodestyle warnings
+]
+src = ["src", "tests"]
+target-version = "py310"
+
+[tool.ruff.flake8-pytest-style]
+fixture-parentheses = false
+mark-parentheses = false
+
+[tool.ruff.isort]
+forced-separate = ["conftest"]
+force-single-line = true
+
+[tool.black]
+line-length = 140
+target-version = ["py310"]
```

### Comparing `pyauxlib-0.0.0/pytest.ini` & `pyauxlib-0.0.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/setup.py` & `pyauxlib-0.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-#!/usr/bin/env python
-import re
-from pathlib import Path
-
-from setuptools import find_packages
-from setuptools import setup
-
-
-def read(*names, **kwargs):
-    with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
-        return fh.read()
-
-
-requirements = ["deprecated", "wrapt"]
-test_requirements = [
-    "pytest>=3",
-]
-
-setup(
-    name="pyauxlib",
-    version="0.0.0",
-    license="BSD-3-Clause",
-    description="Auxiliary library for python.",
-    long_description="{}\n{}".format(
-        re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
-        re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
-    ),
-    author="Pablo Solís Fernández",
-    author_email="pablosolisfernandez@gmail.com",
-    url="https://github.com/psolsfer/pyauxlib",
-    packages=find_packages("src"),
-    package_dir={"": "src"},
-    py_modules=[path.stem for path in Path("src").glob("*.py")],
-    include_package_data=True,
-    zip_safe=False,
-    classifiers=[
-        # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "Development Status :: 2 - Pre-Alpha",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Topic :: Utilities",
-    ],
-    project_urls={
-        "Documentation": "https://pyauxlib.readthedocs.io/",
-        "Changelog": "https://pyauxlib.readthedocs.io/en/latest/changelog.html",
-        "Issue Tracker": "https://github.com/psolsfer/pyauxlib/issues",
-    },
-    keywords=[
-        # eg: "keyword1", "keyword2", "keyword3",
-    ],
-    python_requires=">=3.10",
-    install_requires=requirements,
-    extras_require={
-        # eg:
-        #   "rst": ["docutils>=0.11"],
-        #   ":python_version=="2.6"": ["argparse"],
-    },
-    tests_require=test_requirements,
-)
+#!/usr/bin/env python
+import re
+from pathlib import Path
+
+from setuptools import find_packages
+from setuptools import setup
+
+
+def read(*names, **kwargs):
+    with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
+        return fh.read()
+
+
+requirements = ["deprecated", "wrapt"]
+test_requirements = [
+    "pytest>=3",
+]
+
+setup(
+    name="pyauxlib",
+    version="0.0.1",
+    license="BSD-3-Clause",
+    description="Auxiliary library for python.",
+    long_description="{}\n{}".format(
+        re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
+        re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
+    ),
+    author="Pablo Solís Fernández",
+    author_email="pablosolisfernandez@gmail.com",
+    url="https://github.com/psolsfer/pyauxlib",
+    packages=find_packages("src"),
+    package_dir={"": "src"},
+    py_modules=[path.stem for path in Path("src").glob("*.py")],
+    include_package_data=True,
+    zip_safe=False,
+    classifiers=[
+        # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Utilities",
+    ],
+    project_urls={
+        "Documentation": "https://pyauxlib.readthedocs.io/",
+        "Changelog": "https://pyauxlib.readthedocs.io/en/latest/changelog.html",
+        "Issue Tracker": "https://github.com/psolsfer/pyauxlib/issues",
+    },
+    keywords=[
+        # eg: "keyword1", "keyword2", "keyword3",
+    ],
+    python_requires=">=3.10",
+    install_requires=requirements,
+    extras_require={
+        # eg:
+        #   "rst": ["docutils>=0.11"],
+        #   ":python_version=="2.6"": ["argparse"],
+    },
+    tests_require=test_requirements,
+)
```

### Comparing `pyauxlib-0.0.0/src/pyauxlib/callables/callables.py` & `pyauxlib-0.0.1/src/pyauxlib/callables/callables.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib/experimental/decorator.py` & `pyauxlib-0.0.1/src/pyauxlib/experimental/decorator.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib/experimental/get_caller_path.py` & `pyauxlib-0.0.1/src/pyauxlib/experimental/get_caller_path.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib/experimental/kwargs.py` & `pyauxlib-0.0.1/src/pyauxlib/experimental/kwargs.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib/experimental/lists.py` & `pyauxlib-0.0.1/src/pyauxlib/experimental/lists.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib/io/filesfolders.py` & `pyauxlib-0.0.1/src/pyauxlib/io/filesfolders.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,28 +99,29 @@
                 folder=entry,
                 subfolders=True,
                 file_extensions=file_extensions,
                 parent_path=parent_path,
             )
 
 
-def create_folder(path: Path):
+def create_folder(path: Path, includes_file=False):
     """Creates the folder passed in the path (if it doesn't exist).
     Useful to be sure that a folder exists before saving a file.
 
     Parameters
     ----------
     path : Path
         Path object for the folder (can also include the file)
+    includes_file : bool, optional
+        The path includes a file at the end, by default False.
     """
 
     # NOTE: see also os.makedirs
 
-    # Removes the filename if included in the original path
-    path = path if not path.suffix else path.parents[0]
+    path = path.parent if includes_file else path
 
     try:
         path.mkdir(parents=True)
     except FileExistsError:
         # Defeats race condition when another thread created the path
         pass
```

### Comparing `pyauxlib-0.0.0/src/pyauxlib/io/yamlio.py` & `pyauxlib-0.0.1/src/pyauxlib/io/yamlio.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib/utils/deprecations.py` & `pyauxlib-0.0.1/src/pyauxlib/utils/deprecations.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib/utils/dictionaries.py` & `pyauxlib-0.0.1/src/pyauxlib/utils/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib/utils/encoding.py` & `pyauxlib-0.0.1/src/pyauxlib/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib/utils/logger.py` & `pyauxlib-0.0.1/src/pyauxlib/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib/utils/timer.py` & `pyauxlib-0.0.1/src/pyauxlib/utils/timer.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/src/pyauxlib.egg-info/PKG-INFO` & `pyauxlib-0.0.1/src/pyauxlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauxlib
-Version: 0.0.0
+Version: 0.0.1
 Summary: Auxiliary library for python.
 Home-page: https://github.com/psolsfer/pyauxlib
 Author: Pablo Solís Fernández
 Author-email: pablosolisfernandez@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyauxlib.readthedocs.io/
 Project-URL: Changelog, https://pyauxlib.readthedocs.io/en/latest/changelog.html
```

### Comparing `pyauxlib-0.0.0/src/pyauxlib.egg-info/SOURCES.txt` & `pyauxlib-0.0.1/src/pyauxlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/tests/test_pyauxlib.py` & `pyauxlib-0.0.1/tests/test_pyauxlib.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.0/tox.ini` & `pyauxlib-0.0.1/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,93 @@
 00000000: 5b74 6573 7465 6e76 3a62 6f6f 7473 7472  [testenv:bootstr
-00000010: 6170 5d0a 6465 7073 203d 0a20 2020 206a  ap].deps =.    j
-00000020: 696e 6a61 320a 2020 2020 746f 780a 736b  inja2.    tox.sk
-00000030: 6970 5f69 6e73 7461 6c6c 203d 2074 7275  ip_install = tru
-00000040: 650a 636f 6d6d 616e 6473 203d 0a20 2020  e.commands =.   
-00000050: 2070 7974 686f 6e20 6369 2f62 6f6f 7473   python ci/boots
-00000060: 7472 6170 2e70 7920 2d2d 6e6f 2d65 6e76  trap.py --no-env
-00000070: 0a70 6173 7365 6e76 203d 0a20 2020 202a  .passenv =.    *
-00000080: 0a0a 3b20 6120 6765 6e65 7261 7469 7665  ..; a generative
-00000090: 2074 6f78 2063 6f6e 6669 6775 7261 7469   tox configurati
-000000a0: 6f6e 2c20 7365 653a 2068 7474 7073 3a2f  on, see: https:/
-000000b0: 2f74 6f78 2e77 696b 692f 656e 2f6c 6174  /tox.wiki/en/lat
-000000c0: 6573 742f 7573 6572 5f67 7569 6465 2e68  est/user_guide.h
-000000d0: 746d 6c23 6765 6e65 7261 7469 7665 2d65  tml#generative-e
-000000e0: 6e76 6972 6f6e 6d65 6e74 730a 5b74 6f78  nvironments.[tox
-000000f0: 5d0a 656e 766c 6973 7420 3d0a 2020 2020  ].envlist =.    
-00000100: 636c 6561 6e2c 0a20 2020 2063 6865 636b  clean,.    check
-00000110: 2c0a 2020 2020 646f 6373 2c0a 2020 2020  ,.    docs,.    
-00000120: 7b70 7933 3130 2c70 7933 3131 7d2c 0a20  {py310,py311},. 
-00000130: 2020 2072 6570 6f72 740a 6967 6e6f 7265     report.ignore
-00000140: 5f62 6173 6570 7974 686f 6e5f 636f 6e66  _basepython_conf
-00000150: 6c69 6374 203d 2074 7275 650a 0a5b 7465  lict = true..[te
-00000160: 7374 656e 765d 0a62 6173 6570 7974 686f  stenv].basepytho
-00000170: 6e20 3d0a 2020 2020 7079 3331 303a 207b  n =.    py310: {
-00000180: 656e 763a 544f 5850 5954 484f 4e3a 7079  env:TOXPYTHON:py
-00000190: 7468 6f6e 332e 3130 7d0a 2020 2020 7079  thon3.10}.    py
-000001a0: 3331 313a 207b 656e 763a 544f 5850 5954  311: {env:TOXPYT
-000001b0: 484f 4e3a 7079 7468 6f6e 332e 3131 7d0a  HON:python3.11}.
-000001c0: 2020 2020 7b62 6f6f 7473 7472 6170 2c63      {bootstrap,c
-000001d0: 6c65 616e 2c63 6865 636b 2c72 6570 6f72  lean,check,repor
-000001e0: 742c 646f 6373 7d3a 207b 656e 763a 544f  t,docs}: {env:TO
-000001f0: 5850 5954 484f 4e3a 7079 7468 6f6e 337d  XPYTHON:python3}
-00000200: 0a73 6574 656e 7620 3d0a 2020 2020 5059  .setenv =.    PY
-00000210: 5448 4f4e 5041 5448 3d7b 746f 7869 6e69  THONPATH={toxini
-00000220: 6469 727d 2f74 6573 7473 0a20 2020 2050  dir}/tests.    P
-00000230: 5954 484f 4e55 4e42 5546 4645 5245 443d  YTHONUNBUFFERED=
-00000240: 7965 730a 7061 7373 656e 7620 3d0a 2020  yes.passenv =.  
-00000250: 2020 2a0a 7573 6564 6576 656c 6f70 203d    *.usedevelop =
-00000260: 2066 616c 7365 0a64 6570 7320 3d0a 2020   false.deps =.  
-00000270: 2020 7079 7465 7374 0a20 2020 2070 7974    pytest.    pyt
-00000280: 6573 742d 636f 760a 636f 6d6d 616e 6473  est-cov.commands
-00000290: 203d 0a20 2020 207b 706f 7361 7267 733a   =.    {posargs:
-000002a0: 7079 7465 7374 202d 2d63 6f76 202d 2d63  pytest --cov --c
-000002b0: 6f76 2d72 6570 6f72 743d 7465 726d 2d6d  ov-report=term-m
-000002c0: 6973 7369 6e67 202d 2d63 6f76 2d72 6570  issing --cov-rep
-000002d0: 6f72 743d 786d 6c20 2d76 7620 7465 7374  ort=xml -vv test
-000002e0: 737d 0a0a 5b74 6573 7465 6e76 3a63 6865  s}..[testenv:che
-000002f0: 636b 5d0a 6465 7073 203d 0a20 2020 2064  ck].deps =.    d
-00000300: 6f63 7574 696c 730a 2020 2020 6368 6563  ocutils.    chec
-00000310: 6b2d 6d61 6e69 6665 7374 0a20 2020 2070  k-manifest.    p
-00000320: 7265 2d63 6f6d 6d69 740a 2020 2020 7265  re-commit.    re
-00000330: 6164 6d65 2d72 656e 6465 7265 720a 2020  adme-renderer.  
-00000340: 2020 7079 676d 656e 7473 0a20 2020 2069    pygments.    i
-00000350: 736f 7274 0a73 6b69 705f 696e 7374 616c  sort.skip_instal
-00000360: 6c20 3d20 7472 7565 0a63 6f6d 6d61 6e64  l = true.command
-00000370: 7320 3d0a 2020 2020 7079 7468 6f6e 2073  s =.    python s
-00000380: 6574 7570 2e70 7920 6368 6563 6b20 2d2d  etup.py check --
-00000390: 7374 7269 6374 202d 2d6d 6574 6164 6174  strict --metadat
-000003a0: 6120 2d2d 7265 7374 7275 6374 7572 6564  a --restructured
-000003b0: 7465 7874 0a20 2020 2063 6865 636b 2d6d  text.    check-m
-000003c0: 616e 6966 6573 7420 2e0a 2020 2020 7072  anifest ..    pr
-000003d0: 652d 636f 6d6d 6974 2072 756e 202d 2d61  e-commit run --a
-000003e0: 6c6c 2d66 696c 6573 202d 2d73 686f 772d  ll-files --show-
-000003f0: 6469 6666 2d6f 6e2d 6661 696c 7572 650a  diff-on-failure.
-00000400: 0a5b 7465 7374 656e 763a 646f 6373 5d0a  .[testenv:docs].
-00000410: 7573 6564 6576 656c 6f70 203d 2074 7275  usedevelop = tru
-00000420: 650a 6465 7073 203d 0a20 2020 202d 727b  e.deps =.    -r{
-00000430: 746f 7869 6e69 6469 727d 2f64 6f63 732f  toxinidir}/docs/
-00000440: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
-00000450: 0a63 6f6d 6d61 6e64 7320 3d0a 2020 2020  .commands =.    
-00000460: 7370 6869 6e78 2d62 7569 6c64 207b 706f  sphinx-build {po
-00000470: 7361 7267 733a 2d45 7d20 2d62 2068 746d  sargs:-E} -b htm
-00000480: 6c20 646f 6373 2064 6973 742f 646f 6373  l docs dist/docs
-00000490: 0a20 2020 2073 7068 696e 782d 6275 696c  .    sphinx-buil
-000004a0: 6420 2d62 206c 696e 6b63 6865 636b 2064  d -b linkcheck d
-000004b0: 6f63 7320 6469 7374 2f64 6f63 730a 0a5b  ocs dist/docs..[
-000004c0: 7465 7374 656e 763a 7265 706f 7274 5d0a  testenv:report].
-000004d0: 6465 7073 203d 0a20 2020 2063 6f76 6572  deps =.    cover
-000004e0: 6167 650a 736b 6970 5f69 6e73 7461 6c6c  age.skip_install
-000004f0: 203d 2074 7275 650a 636f 6d6d 616e 6473   = true.commands
-00000500: 203d 0a20 2020 2063 6f76 6572 6167 6520   =.    coverage 
-00000510: 7265 706f 7274 0a20 2020 2063 6f76 6572  report.    cover
-00000520: 6167 6520 6874 6d6c 0a0a 5b74 6573 7465  age html..[teste
-00000530: 6e76 3a63 6c65 616e 5d0a 636f 6d6d 616e  nv:clean].comman
-00000540: 6473 203d 2063 6f76 6572 6167 6520 6572  ds = coverage er
-00000550: 6173 650a 736b 6970 5f69 6e73 7461 6c6c  ase.skip_install
-00000560: 203d 2074 7275 650a 6465 7073 203d 0a20   = true.deps =. 
-00000570: 2020 2063 6f76 6572 6167 650a               coverage.
+00000010: 6170 5d0d 0a64 6570 7320 3d0d 0a20 2020  ap]..deps =..   
+00000020: 206a 696e 6a61 320d 0a20 2020 2074 6f78   jinja2..    tox
+00000030: 0d0a 736b 6970 5f69 6e73 7461 6c6c 203d  ..skip_install =
+00000040: 2074 7275 650d 0a63 6f6d 6d61 6e64 7320   true..commands 
+00000050: 3d0d 0a20 2020 2070 7974 686f 6e20 6369  =..    python ci
+00000060: 2f62 6f6f 7473 7472 6170 2e70 7920 2d2d  /bootstrap.py --
+00000070: 6e6f 2d65 6e76 0d0a 7061 7373 656e 7620  no-env..passenv 
+00000080: 3d0d 0a20 2020 202a 0d0a 0d0a 3b20 6120  =..    *....; a 
+00000090: 6765 6e65 7261 7469 7665 2074 6f78 2063  generative tox c
+000000a0: 6f6e 6669 6775 7261 7469 6f6e 2c20 7365  onfiguration, se
+000000b0: 653a 2068 7474 7073 3a2f 2f74 6f78 2e77  e: https://tox.w
+000000c0: 696b 692f 656e 2f6c 6174 6573 742f 7573  iki/en/latest/us
+000000d0: 6572 5f67 7569 6465 2e68 746d 6c23 6765  er_guide.html#ge
+000000e0: 6e65 7261 7469 7665 2d65 6e76 6972 6f6e  nerative-environ
+000000f0: 6d65 6e74 730d 0a5b 746f 785d 0d0a 656e  ments..[tox]..en
+00000100: 766c 6973 7420 3d0d 0a20 2020 2063 6c65  vlist =..    cle
+00000110: 616e 2c0d 0a20 2020 2063 6865 636b 2c0d  an,..    check,.
+00000120: 0a20 2020 2064 6f63 732c 0d0a 2020 2020  .    docs,..    
+00000130: 7b70 7933 3130 2c70 7933 3131 7d2c 0d0a  {py310,py311},..
+00000140: 2020 2020 7265 706f 7274 0d0a 6967 6e6f      report..igno
+00000150: 7265 5f62 6173 6570 7974 686f 6e5f 636f  re_basepython_co
+00000160: 6e66 6c69 6374 203d 2074 7275 650d 0a0d  nflict = true...
+00000170: 0a5b 7465 7374 656e 765d 0d0a 6261 7365  .[testenv]..base
+00000180: 7079 7468 6f6e 203d 0d0a 2020 2020 7079  python =..    py
+00000190: 3331 303a 207b 656e 763a 544f 5850 5954  310: {env:TOXPYT
+000001a0: 484f 4e3a 7079 7468 6f6e 332e 3130 7d0d  HON:python3.10}.
+000001b0: 0a20 2020 2070 7933 3131 3a20 7b65 6e76  .    py311: {env
+000001c0: 3a54 4f58 5059 5448 4f4e 3a70 7974 686f  :TOXPYTHON:pytho
+000001d0: 6e33 2e31 317d 0d0a 2020 2020 7b62 6f6f  n3.11}..    {boo
+000001e0: 7473 7472 6170 2c63 6c65 616e 2c63 6865  tstrap,clean,che
+000001f0: 636b 2c72 6570 6f72 742c 646f 6373 7d3a  ck,report,docs}:
+00000200: 207b 656e 763a 544f 5850 5954 484f 4e3a   {env:TOXPYTHON:
+00000210: 7079 7468 6f6e 337d 0d0a 7365 7465 6e76  python3}..setenv
+00000220: 203d 0d0a 2020 2020 5059 5448 4f4e 5041   =..    PYTHONPA
+00000230: 5448 3d7b 746f 7869 6e69 6469 727d 2f74  TH={toxinidir}/t
+00000240: 6573 7473 0d0a 2020 2020 5059 5448 4f4e  ests..    PYTHON
+00000250: 554e 4255 4646 4552 4544 3d79 6573 0d0a  UNBUFFERED=yes..
+00000260: 7061 7373 656e 7620 3d0d 0a20 2020 202a  passenv =..    *
+00000270: 0d0a 7573 6564 6576 656c 6f70 203d 2066  ..usedevelop = f
+00000280: 616c 7365 0d0a 6465 7073 203d 0d0a 2020  alse..deps =..  
+00000290: 2020 7079 7465 7374 0d0a 2020 2020 7079    pytest..    py
+000002a0: 7465 7374 2d63 6f76 0d0a 636f 6d6d 616e  test-cov..comman
+000002b0: 6473 203d 0d0a 2020 2020 7b70 6f73 6172  ds =..    {posar
+000002c0: 6773 3a70 7974 6573 7420 2d2d 636f 7620  gs:pytest --cov 
+000002d0: 2d2d 636f 762d 7265 706f 7274 3d74 6572  --cov-report=ter
+000002e0: 6d2d 6d69 7373 696e 6720 2d2d 636f 762d  m-missing --cov-
+000002f0: 7265 706f 7274 3d78 6d6c 202d 7676 2074  report=xml -vv t
+00000300: 6573 7473 7d0d 0a0d 0a5b 7465 7374 656e  ests}....[testen
+00000310: 763a 6368 6563 6b5d 0d0a 6465 7073 203d  v:check]..deps =
+00000320: 0d0a 2020 2020 646f 6375 7469 6c73 0d0a  ..    docutils..
+00000330: 2020 2020 6368 6563 6b2d 6d61 6e69 6665      check-manife
+00000340: 7374 0d0a 2020 2020 7072 652d 636f 6d6d  st..    pre-comm
+00000350: 6974 0d0a 2020 2020 7265 6164 6d65 2d72  it..    readme-r
+00000360: 656e 6465 7265 720d 0a20 2020 2070 7967  enderer..    pyg
+00000370: 6d65 6e74 730d 0a20 2020 2069 736f 7274  ments..    isort
+00000380: 0d0a 736b 6970 5f69 6e73 7461 6c6c 203d  ..skip_install =
+00000390: 2074 7275 650d 0a63 6f6d 6d61 6e64 7320   true..commands 
+000003a0: 3d0d 0a20 2020 2070 7974 686f 6e20 7365  =..    python se
+000003b0: 7475 702e 7079 2063 6865 636b 202d 2d73  tup.py check --s
+000003c0: 7472 6963 7420 2d2d 6d65 7461 6461 7461  trict --metadata
+000003d0: 202d 2d72 6573 7472 7563 7475 7265 6474   --restructuredt
+000003e0: 6578 740d 0a20 2020 2063 6865 636b 2d6d  ext..    check-m
+000003f0: 616e 6966 6573 7420 2e0d 0a20 2020 2070  anifest ...    p
+00000400: 7265 2d63 6f6d 6d69 7420 7275 6e20 2d2d  re-commit run --
+00000410: 616c 6c2d 6669 6c65 7320 2d2d 7368 6f77  all-files --show
+00000420: 2d64 6966 662d 6f6e 2d66 6169 6c75 7265  -diff-on-failure
+00000430: 0d0a 0d0a 5b74 6573 7465 6e76 3a64 6f63  ....[testenv:doc
+00000440: 735d 0d0a 7573 6564 6576 656c 6f70 203d  s]..usedevelop =
+00000450: 2074 7275 650d 0a64 6570 7320 3d0d 0a20   true..deps =.. 
+00000460: 2020 202d 727b 746f 7869 6e69 6469 727d     -r{toxinidir}
+00000470: 2f64 6f63 732f 7265 7175 6972 656d 656e  /docs/requiremen
+00000480: 7473 2e74 7874 0d0a 636f 6d6d 616e 6473  ts.txt..commands
+00000490: 203d 0d0a 2020 2020 7370 6869 6e78 2d62   =..    sphinx-b
+000004a0: 7569 6c64 207b 706f 7361 7267 733a 2d45  uild {posargs:-E
+000004b0: 7d20 2d62 2068 746d 6c20 646f 6373 2064  } -b html docs d
+000004c0: 6973 742f 646f 6373 0d0a 2020 2020 7370  ist/docs..    sp
+000004d0: 6869 6e78 2d62 7569 6c64 202d 6220 6c69  hinx-build -b li
+000004e0: 6e6b 6368 6563 6b20 646f 6373 2064 6973  nkcheck docs dis
+000004f0: 742f 646f 6373 0d0a 0d0a 5b74 6573 7465  t/docs....[teste
+00000500: 6e76 3a72 6570 6f72 745d 0d0a 6465 7073  nv:report]..deps
+00000510: 203d 0d0a 2020 2020 636f 7665 7261 6765   =..    coverage
+00000520: 0d0a 736b 6970 5f69 6e73 7461 6c6c 203d  ..skip_install =
+00000530: 2074 7275 650d 0a63 6f6d 6d61 6e64 7320   true..commands 
+00000540: 3d0d 0a20 2020 2063 6f76 6572 6167 6520  =..    coverage 
+00000550: 7265 706f 7274 0d0a 2020 2020 636f 7665  report..    cove
+00000560: 7261 6765 2068 746d 6c0d 0a0d 0a5b 7465  rage html....[te
+00000570: 7374 656e 763a 636c 6561 6e5d 0d0a 636f  stenv:clean]..co
+00000580: 6d6d 616e 6473 203d 2063 6f76 6572 6167  mmands = coverag
+00000590: 6520 6572 6173 650d 0a73 6b69 705f 696e  e erase..skip_in
+000005a0: 7374 616c 6c20 3d20 7472 7565 0d0a 6465  stall = true..de
+000005b0: 7073 203d 0d0a 2020 2020 636f 7665 7261  ps =..    covera
+000005c0: 6765 0d0a                                ge..
```

