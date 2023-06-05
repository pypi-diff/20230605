# Comparing `tmp/invenio-workflows-tugraz-0.2.1.tar.gz` & `tmp/invenio-workflows-tugraz-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-workflows-tugraz-0.2.1.tar", last modified: Fri Jun  2 13:35:39 2023, max compression
+gzip compressed data, was "invenio-workflows-tugraz-0.2.2.tar", last modified: Mon Jun  5 08:59:21 2023, max compression
```

## Comparing `invenio-workflows-tugraz-0.2.1.tar` & `invenio-workflows-tugraz-0.2.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:39.535561 invenio-workflows-tugraz-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:39.527561 invenio-workflows-tugraz-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:39.531561 invenio-workflows-tugraz-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-02 13:35:39.535561 invenio-workflows-tugraz-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:39.531561 invenio-workflows-tugraz-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:39.531561 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:39.531561 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/data/
--rw-r--r--   0 runner    (1001) docker     (123)   939307 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/data/iso6393.json
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:39.535561 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/openaccess/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/openaccess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/openaccess/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/openaccess/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/openaccess/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/openaccess/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:39.535561 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/theses.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:39.531561 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-02 13:35:39.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-02 13:35:39.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:35:39.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-02 13:35:39.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:35:39.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 13:35:39.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 13:35:39.000000 invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-02 13:35:39.535561 invenio-workflows-tugraz-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:35:39.535561 invenio-workflows-tugraz-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-02 13:35:33.000000 invenio-workflows-tugraz-0.2.1/tests/test_invenio_workflows_tugraz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:59:20.996500 invenio-workflows-tugraz-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:59:20.988499 invenio-workflows-tugraz-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:59:20.992499 invenio-workflows-tugraz-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-05 08:59:20.996500 invenio-workflows-tugraz-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:59:20.992499 invenio-workflows-tugraz-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:59:20.992499 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:59:20.996500 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   939307 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/data/iso6393.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:59:20.996500 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/openaccess/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/openaccess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/openaccess/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/openaccess/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/openaccess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/openaccess/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:59:20.996500 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/theses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:59:20.992499 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-05 08:59:20.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-05 08:59:20.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 08:59:20.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 08:59:20.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 08:59:20.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-05 08:59:20.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 08:59:20.000000 invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-05 08:59:20.996500 invenio-workflows-tugraz-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:59:20.996500 invenio-workflows-tugraz-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-05 08:59:14.000000 invenio-workflows-tugraz-0.2.2/tests/test_invenio_workflows_tugraz.py
```

### Comparing `invenio-workflows-tugraz-0.2.1/.editorconfig` & `invenio-workflows-tugraz-0.2.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/.github/workflows/tests.yml` & `invenio-workflows-tugraz-0.2.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/CHANGES.rst` & `invenio-workflows-tugraz-0.2.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.2.2 (release 2023-06-05)
+
+- fix: wrong method used to get the record
+
+
 Version v0.2.1 (release 2023-06-02)
 
 - theses: not only drafts should be updated
 - fix: theses update_func api used wrong
 
 
 Version v0.2.0 (release 2023-05-26)
```

### Comparing `invenio-workflows-tugraz-0.2.1/CONTRIBUTING.rst` & `invenio-workflows-tugraz-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/LICENSE` & `invenio-workflows-tugraz-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/MANIFEST.in` & `invenio-workflows-tugraz-0.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/PKG-INFO` & `invenio-workflows-tugraz-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-workflows-tugraz
-Version: 0.2.1
+Version: 0.2.2
 Summary: "Package serves as a place for the workflows of the repository of the TU Graz."
 Home-page: https://github.com/tu-graz-library/invenio-workflows-tugraz
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio workflows TUGraz
 Platform: any
@@ -26,14 +26,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.2.2 (release 2023-06-05)
+
+- fix: wrong method used to get the record
+
+
 Version v0.2.1 (release 2023-06-02)
 
 - theses: not only drafts should be updated
 - fix: theses update_func api used wrong
 
 
 Version v0.2.0 (release 2023-05-26)
```

### Comparing `invenio-workflows-tugraz-0.2.1/babel.ini` & `invenio-workflows-tugraz-0.2.2/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/docs/Makefile` & `invenio-workflows-tugraz-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/docs/conf.py` & `invenio-workflows-tugraz-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/docs/index.rst` & `invenio-workflows-tugraz-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/docs/make.bat` & `invenio-workflows-tugraz-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/config.py` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/config.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/data/iso6393.json` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/data/iso6393.json`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/ext.py` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/openaccess/convert.py` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/openaccess/convert.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/openaccess/utils.py` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/openaccess/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/openaccess/workflow.py` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/openaccess/workflow.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/__init__.py` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/convert.py` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/convert.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/decorators.py` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/theses.py` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/theses.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     CampusOnlineConfigs,
     CampusOnlineID,
     ThesesFilter,
     ThesesState,
 )
 from invenio_campusonline.utils import get_embargo_range
 from invenio_config_tugraz import get_identity_from_user_by_email
-from invenio_pidstore.errors import PIDDoesNotExistError
 from invenio_records_marc21 import (
     DuplicateRecordError,
     Marc21Metadata,
     Marc21RecordService,
     check_about_duplicate,
     create_record,
     current_records_marc21,
@@ -180,22 +179,16 @@
     records_service: Marc21RecordService,
     alma_service: AlmaSRUService,
     marc_id: str,
     cms_id: str,
     identity: Identity,
 ) -> None:
     """Update the record by metadata from alma."""
-    try:
-        data = records_service.read(id_=marc_id, identity=identity).data
-    except PIDDoesNotExistError:
-        try:
-            data = records_service.read_draft(id_=marc_id, identity=identity).data
-        except PIDDoesNotExistError as esc:
-            msg = f"pid: {marc_id} not found"
-            raise RuntimeError(msg) from esc
+    record_list = records_service.search_versions(id_=marc_id, identity=identity)
+    data = list(record_list.hits)[0]
 
     marc21_etree = alma_service.get_record(cms_id, search_key="local_field_995")
     marc21_record = Marc21Metadata(metadata=marc21_etree[0])
 
     is_restricted = marc21_record.exists_field(
         category="971",
         ind1="7",
```

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz/theses/views.py` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz/theses/views.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz.egg-info/PKG-INFO` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-workflows-tugraz
-Version: 0.2.1
+Version: 0.2.2
 Summary: "Package serves as a place for the workflows of the repository of the TU Graz."
 Home-page: https://github.com/tu-graz-library/invenio-workflows-tugraz
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio workflows TUGraz
 Platform: any
@@ -26,14 +26,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.2.2 (release 2023-06-05)
+
+- fix: wrong method used to get the record
+
+
 Version v0.2.1 (release 2023-06-02)
 
 - theses: not only drafts should be updated
 - fix: theses update_func api used wrong
 
 
 Version v0.2.0 (release 2023-05-26)
```

### Comparing `invenio-workflows-tugraz-0.2.1/invenio_workflows_tugraz.egg-info/SOURCES.txt` & `invenio-workflows-tugraz-0.2.2/invenio_workflows_tugraz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/setup.cfg` & `invenio-workflows-tugraz-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/tests/conftest.py` & `invenio-workflows-tugraz-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.2.1/tests/test_invenio_workflows_tugraz.py` & `invenio-workflows-tugraz-0.2.2/tests/test_invenio_workflows_tugraz.py`

 * *Files identical despite different names*

