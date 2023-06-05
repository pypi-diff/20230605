# Comparing `tmp/qiskit-iqm-8.2.tar.gz` & `tmp/qiskit-iqm-8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-iqm-8.2.tar", last modified: Fri Jun  2 08:10:11 2023, max compression
+gzip compressed data, was "qiskit-iqm-8.3.tar", last modified: Mon Jun  5 07:52:48 2023, max compression
```

## Comparing `qiskit-iqm-8.2.tar` & `qiskit-iqm-8.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.762906 qiskit-iqm-8.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-02 08:10:11.762906 qiskit-iqm-8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/examples/bell_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:10:11.762906 qiskit-iqm-8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.754906 qiskit-iqm-8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/src/qiskit_iqm/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/src/qiskit_iqm/qiskit_to_iqm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-02 08:10:11.000000 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-02 08:10:11.000000 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:10:11.000000 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-02 08:10:11.000000 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 08:10:11.000000 qiskit-iqm-8.2/src/qiskit_iqm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:11.758906 qiskit-iqm-8.2/tests/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/fake_backends/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/fake_backends/test_fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/fake_backends/test_iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/test_iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/test_iqm_facade_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/test_iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/test_iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tests/test_qiskit_to_iqm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-02 08:09:15.000000 qiskit-iqm-8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.821072 qiskit-iqm-8.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.813072 qiskit-iqm-8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.813072 qiskit-iqm-8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-05 07:52:48.821072 qiskit-iqm-8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/examples/bell_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:52:48.821072 qiskit-iqm-8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.813072 qiskit-iqm-8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/src/qiskit_iqm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/qiskit_to_iqm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-05 07:52:48.000000 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-05 07:52:48.000000 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:52:48.000000 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-05 07:52:48.000000 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 07:52:48.000000 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.821072 qiskit-iqm-8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.821072 qiskit-iqm-8.3/tests/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/fake_backends/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/fake_backends/test_fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/fake_backends/test_iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/test_iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/test_iqm_facade_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/test_iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/test_iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/test_qiskit_to_iqm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tox.ini
```

### Comparing `qiskit-iqm-8.2/.github/workflows/ci.yml` & `qiskit-iqm-8.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/.github/workflows/publish.yml` & `qiskit-iqm-8.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/.github/workflows/tag_and_release.yml` & `qiskit-iqm-8.3/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/CHANGELOG.rst` & `qiskit-iqm-8.3/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+Version 8.3
+============
+
+* Bugfixes for ``heralding`` run with zero shots returned. `#65 <https://github.com/iqm-finland/qiskit-on-iqm/pull/65>`_
+* Allow specifying ``calibration_set_id`` both as string and as ``UUID``. `#65 <https://github.com/iqm-finland/qiskit-on-iqm/pull/65>`_
+
 Version 8.2
 ============
 
 * Add ``heralding`` option to ``IQMBackend``. `#63 <https://github.com/iqm-finland/qiskit-on-iqm/pull/63>`_
 * Upgrade to ``IQMClient`` version 12.5. `#63 <https://github.com/iqm-finland/qiskit-on-iqm/pull/63>`_
 
 Version 8.1
```

### Comparing `qiskit-iqm-8.2/CONTRIBUTING.rst` & `qiskit-iqm-8.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/LICENSE` & `qiskit-iqm-8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/PKG-INFO` & `qiskit-iqm-8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 8.2
+Version: 8.3
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qiskit-iqm-8.2/README.rst` & `qiskit-iqm-8.3/README.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/docs/Makefile` & `qiskit-iqm-8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/docs/_static/images/favicon.ico` & `qiskit-iqm-8.3/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/docs/_static/images/logo.png` & `qiskit-iqm-8.3/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/docs/_templates/autosummary-class-template.rst` & `qiskit-iqm-8.3/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/docs/_templates/autosummary-module-template.rst` & `qiskit-iqm-8.3/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/docs/_templates/page.html` & `qiskit-iqm-8.3/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/docs/_templates/versioning.html` & `qiskit-iqm-8.3/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/docs/conf.py` & `qiskit-iqm-8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/docs/index.rst` & `qiskit-iqm-8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/docs/user_guide.rst` & `qiskit-iqm-8.3/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/examples/bell_measure.py` & `qiskit-iqm-8.3/examples/bell_measure.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/pyproject.toml` & `qiskit-iqm-8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/src/qiskit_iqm/__init__.py` & `qiskit-iqm-8.3/src/qiskit_iqm/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/__init__.py` & `qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/fake_adonis.py` & `qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/src/qiskit_iqm/fake_backends/iqm_fake_backend.py` & `qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/iqm_fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/src/qiskit_iqm/iqm_backend.py` & `qiskit-iqm-8.3/src/qiskit_iqm/iqm_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/src/qiskit_iqm/iqm_job.py` & `qiskit-iqm-8.3/src/qiskit_iqm/iqm_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 from __future__ import annotations
 
 from collections import Counter
 from datetime import date
 from typing import Optional, Union
 import uuid
+import warnings
 
 from iqm_client import CircuitMeasurementResults, HeraldingMode, IQMClient, RunRequest, RunResult, Status
 import numpy as np
 from qiskit.providers import JobStatus, JobV1
 from qiskit.result import Counts, Result
 
 from qiskit_iqm.qiskit_to_iqm import MeasurementKey
@@ -63,19 +64,26 @@
     def _format_measurement_results(
         measurement_results: CircuitMeasurementResults, requested_shots: int, expect_exact_shots: bool = True
     ) -> list[str]:
         formatted_results: dict[int, np.ndarray] = {}
         for k, v in measurement_results.items():
             mk = MeasurementKey.from_string(k)
             res = np.array(v, dtype=int)
-            # in Qiskit each measurement is a separate single-qubit instruction. qiskit-iqm assigns unique measurement
-            # key to each such instruction, so only one column is expected per measurement key.
-            if res.shape[1] != 1:
-                raise ValueError(f'Measurement result {mk} has the wrong shape {res.shape}, expected (*, 1)')
-            res = res[:, 0]
+            if len(v) == 0 and not expect_exact_shots:
+                warnings.warn(
+                    'Received measurement results containing zero shots. '
+                    'In case you are using non-default heralding mode, this could be because of bad calibration.'
+                )
+                res = np.array([])
+            else:
+                # in Qiskit each measurement is a separate single-qubit instruction. qiskit-iqm assigns unique
+                # measurement key to each such instruction, so only one column is expected per measurement key.
+                if res.shape[1] != 1:
+                    raise ValueError(f'Measurement result {mk} has the wrong shape {res.shape}, expected (*, 1)')
+                res = res[:, 0]
 
             shots = len(res)
             if expect_exact_shots and shots != requested_shots:
                 raise ValueError(f'Expected {requested_shots} shots but got {shots} for measurement result {mk}')
 
             # group the measurements into cregs, fill in zeros for unused bits
             creg = formatted_results.setdefault(mk.creg_idx, np.zeros((shots, mk.creg_len), dtype=int))
```

### Comparing `qiskit-iqm-8.2/src/qiskit_iqm/iqm_provider.py` & `qiskit-iqm-8.3/src/qiskit_iqm/iqm_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,26 +60,28 @@
         circuits = [run_input] if isinstance(run_input, QuantumCircuit) else run_input
 
         if len(circuits) == 0:
             raise ValueError('Empty list of circuits submitted for execution.')
 
         shots = options.get('shots', self.options.shots)
         calibration_set_id = options.get('calibration_set_id', self.options.calibration_set_id)
+        if calibration_set_id is not None and not isinstance(calibration_set_id, UUID):
+            calibration_set_id = UUID(calibration_set_id)
         circuit_duration_check = options.get('circuit_duration_check', self.options.circuit_duration_check)
         heralding_mode = options.get('heralding_mode', self.options.heralding_mode)
 
         circuits_serialized: list[Circuit] = [self.serialize_circuit(circuit) for circuit in circuits]
         used_indices: set[int] = reduce(
             lambda qubits, circuit: qubits.union(set(int(q) for q in circuit.all_qubits())), circuits_serialized, set()
         )
         qubit_mapping = {str(idx): qb for idx, qb in self._idx_to_qb.items() if idx in used_indices}
         job_id = self.client.submit_circuits(
             circuits_serialized,
             qubit_mapping=qubit_mapping,
-            calibration_set_id=UUID(calibration_set_id) if calibration_set_id else None,
+            calibration_set_id=calibration_set_id if calibration_set_id else None,
             shots=shots,
             circuit_duration_check=circuit_duration_check,
             heralding_mode=heralding_mode,
         )
         job = IQMJob(self, str(job_id), shots=shots)
         job.circuit_metadata = [c.metadata for c in circuits]
         return job
```

### Comparing `qiskit-iqm-8.2/src/qiskit_iqm/qiskit_to_iqm.py` & `qiskit-iqm-8.3/src/qiskit_iqm/qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/src/qiskit_iqm.egg-info/PKG-INFO` & `qiskit-iqm-8.3/src/qiskit_iqm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 8.2
+Version: 8.3
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qiskit-iqm-8.2/src/qiskit_iqm.egg-info/SOURCES.txt` & `qiskit-iqm-8.3/src/qiskit_iqm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/tag-from-pipeline.sh` & `qiskit-iqm-8.3/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/tests/conftest.py` & `qiskit-iqm-8.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/tests/fake_backends/conftest.py` & `qiskit-iqm-8.3/tests/fake_backends/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/tests/fake_backends/test_fake_adonis.py` & `qiskit-iqm-8.3/tests/fake_backends/test_fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/tests/fake_backends/test_iqm_fake_backend.py` & `qiskit-iqm-8.3/tests/fake_backends/test_iqm_fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/tests/test_iqm_backend.py` & `qiskit-iqm-8.3/tests/test_iqm_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/tests/test_iqm_facade_backend.py` & `qiskit-iqm-8.3/tests/test_iqm_facade_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/tests/test_iqm_job.py` & `qiskit-iqm-8.3/tests/test_iqm_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Testing IQMJob.
 """
 import uuid
 
-from iqm_client import Instruction, IQMClient, RunResult, RunStatus, SingleQubitMapping, Status
+from iqm_client import HeraldingMode, Instruction, IQMClient, RunResult, RunStatus, SingleQubitMapping, Status
 import mockito
 from mockito import mock, when
 import pytest
 from qiskit import QuantumCircuit
 from qiskit.providers import JobStatus
 from qiskit.result import Counts
 from qiskit.result import Result as QiskitResult
@@ -33,16 +33,16 @@
     client = mock(IQMClient)
     when(client).get_quantum_architecture().thenReturn(adonis_architecture)
     backend = IQMBackend(client)
     return IQMJob(backend, str(uuid.uuid4()))
 
 
 @pytest.fixture()
-def iqm_result_single_register():
-    return {'c_2_0_0': [[0], [1], [0], [1]], 'c_2_0_1': [[1], [1], [1], [0]]}
+def iqm_result_no_shots():
+    return {'c_2_0_0': [], 'c_2_0_1': []}
 
 
 @pytest.fixture()
 def iqm_result_two_registers():
     return {'c_2_0_0': [[1], [0], [1], [0]], 'c_2_0_1': [[1], [1], [0], [1]], 'd_4_1_2': [[1], [1], [1], [1]]}
 
 
@@ -121,14 +121,31 @@
     # and call to status() does not call any functions from client.
     result = job.result()
     assert isinstance(result, QiskitResult)
     assert job.status() == JobStatus.DONE
     mockito.verify(job._client, times=1).wait_for_results(uuid.UUID(job.job_id()))
 
 
+def test_result_no_shots(job, iqm_result_no_shots, iqm_metadata):
+    iqm_metadata['request']['heralding_mode'] = HeraldingMode.ZEROS
+    client_result = RunResult(
+        status=Status.READY,
+        measurements=[iqm_result_no_shots],
+        metadata=iqm_metadata,
+    )
+    when(job._client).wait_for_results(uuid.UUID(job.job_id())).thenReturn(client_result)
+
+    with pytest.warns(UserWarning, match='Received measurement results containing zero shots.'):
+        result = job.result()
+
+    assert isinstance(result, QiskitResult)
+    assert result.get_memory() == []
+    assert result.get_counts() == Counts({})
+
+
 def test_result_multiple_circuits(job, iqm_result_two_registers):
     instruction_meta = [{'name': 'measurement', 'qubits': ['0'], 'args': {'key': 'm1'}}]
     iqm_metadata_multiple_circuits = {
         'calibration_set_id': '9d75904b-0c93-461f-b1dc-bd200cfad1f1',
         'request': {
             'shots': 4,
             'circuits': [
```

### Comparing `qiskit-iqm-8.2/tests/test_iqm_provider.py` & `qiskit-iqm-8.3/tests/test_iqm_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,20 +267,24 @@
     backend.client.submit_circuits = lambda *args, **kwargs: some_id
     job = backend.run([circuit_1, circuit_2], shots=10)
     assert isinstance(job, IQMJob)
     assert job.job_id() == str(some_id)
     assert job.circuit_metadata == [circuit_1.metadata, circuit_2.metadata]
 
 
-def test_run_with_custom_calibration_set_id(backend, circuit, submit_circuits_default_kwargs, job_id):
+@pytest.mark.parametrize(
+    'calibration_set_id', ['67e77465-d90e-4839-986e-9270f952b743', uuid.UUID('67e77465-d90e-4839-986e-9270f952b743')]
+)
+def test_run_with_custom_calibration_set_id(
+    backend, circuit, submit_circuits_default_kwargs, job_id, calibration_set_id
+):
     circuit.measure(0, 0)
     circuit_ser = backend.serialize_circuit(circuit)
-    calibration_set_id = '67e77465-d90e-4839-986e-9270f952b743'
     kwargs = submit_circuits_default_kwargs | {
-        'calibration_set_id': uuid.UUID(calibration_set_id),
+        'calibration_set_id': uuid.UUID('67e77465-d90e-4839-986e-9270f952b743'),
         'qubit_mapping': {'0': 'QB1'},
     }
     when(backend.client).submit_circuits([circuit_ser], **kwargs).thenReturn(job_id)
 
     backend.run([circuit], calibration_set_id=calibration_set_id)
```

### Comparing `qiskit-iqm-8.2/tests/test_qiskit_to_iqm.py` & `qiskit-iqm-8.3/tests/test_qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.2/tox.ini` & `qiskit-iqm-8.3/tox.ini`

 * *Files identical despite different names*

