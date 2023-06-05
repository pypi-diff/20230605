# Comparing `tmp/model_bakery-1.8.0.tar.gz` & `tmp/model_bakery-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_bakery-1.8.0.tar", last modified: Thu Oct 13 19:59:12 2022, max compression
+gzip compressed data, was "model_bakery-1.9.0.tar", last modified: Mon Oct 24 06:11:27 2022, max compression
```

## Comparing `model_bakery-1.8.0.tar` & `model_bakery-1.9.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.621872 model_bakery-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    13138 2022-10-13 19:59:03.000000 model_bakery-1.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-10-13 19:59:03.000000 model_bakery-1.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-13 19:59:03.000000 model_bakery-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-10-13 19:59:03.000000 model_bakery-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2022-10-13 19:59:12.621872 model_bakery-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-10-13 19:59:03.000000 model_bakery-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.617872 model_bakery-1.8.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.617872 model_bakery-1.8.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     9633 2022-10-13 19:59:03.000000 model_bakery-1.8.0/docs/source/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5016 2022-10-13 19:59:03.000000 model_bakery-1.8.0/docs/source/how_bakery_behaves.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-10-13 19:59:03.000000 model_bakery-1.8.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-10-13 19:59:03.000000 model_bakery-1.8.0/docs/source/migrating_from_mommy.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11084 2022-10-13 19:59:03.000000 model_bakery-1.8.0/docs/source/recipes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-10-13 19:59:03.000000 model_bakery-1.8.0/docs/source/test_runners.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.621872 model_bakery-1.8.0/model_bakery/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    25976 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/baker.py
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6681 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/generators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/gis.py
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/mock_file.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/mock_img.jpeg
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     9046 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/random_gen.py
--rw-r--r--   0 runner    (1001) docker     (121)     8294 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/recipe.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/timezone.py
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-10-13 19:59:03.000000 model_bakery-1.8.0/model_bakery/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.621872 model_bakery-1.8.0/model_bakery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2022-10-13 19:59:12.000000 model_bakery-1.8.0/model_bakery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-10-13 19:59:12.000000 model_bakery-1.8.0/model_bakery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 19:59:12.000000 model_bakery-1.8.0/model_bakery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-13 19:59:12.000000 model_bakery-1.8.0/model_bakery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-13 19:59:12.000000 model_bakery-1.8.0/model_bakery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-13 19:59:03.000000 model_bakery-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-13 19:59:03.000000 model_bakery-1.8.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-10-13 19:59:12.621872 model_bakery-1.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1622 2022-10-13 19:59:03.000000 model_bakery-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.621872 model_bakery-1.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.621872 model_bakery-1.8.0/tests/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/ambiguous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/ambiguous/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.621872 model_bakery-1.8.0/tests/ambiguous2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/ambiguous2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/ambiguous2/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.621872 model_bakery-1.8.0/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2938 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/generic/baker_recipes.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/generic/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/generic/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/generic/generators.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13907 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/generic/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.617872 model_bakery-1.8.0/tests/generic/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.621872 model_bakery-1.8.0/tests/generic/tests/sub_package/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/generic/tests/sub_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/generic/tests/sub_package/baker_recipes.py
--rw-r--r--   0 runner    (1001) docker     (121)    39832 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/test_baker.py
--rw-r--r--   0 runner    (1001) docker     (121)     3746 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/test_extending_bakery.py
--rw-r--r--   0 runner    (1001) docker     (121)    23402 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/test_filling_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    25948 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/test_recipes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6184 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.621872 model_bakery-1.8.0/tests/uninstalled/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tests/uninstalled/baker_recipes.py
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-10-13 19:59:03.000000 model_bakery-1.8.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:59:12.621872 model_bakery-1.8.0/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-10-13 19:59:03.000000 model_bakery-1.8.0/utils/from_mommy_to_bakery.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.514335 model_bakery-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    13544 2022-10-24 06:11:18.000000 model_bakery-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2022-10-24 06:11:18.000000 model_bakery-1.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2022-10-24 06:11:18.000000 model_bakery-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2022-10-24 06:11:18.000000 model_bakery-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3546 2022-10-24 06:11:27.514335 model_bakery-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2022-10-24 06:11:18.000000 model_bakery-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.510334 model_bakery-1.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.510334 model_bakery-1.9.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     9633 2022-10-24 06:11:18.000000 model_bakery-1.9.0/docs/source/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5016 2022-10-24 06:11:18.000000 model_bakery-1.9.0/docs/source/how_bakery_behaves.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2022-10-24 06:11:18.000000 model_bakery-1.9.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2022-10-24 06:11:18.000000 model_bakery-1.9.0/docs/source/migrating_from_mommy.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11084 2022-10-24 06:11:18.000000 model_bakery-1.9.0/docs/source/recipes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1529 2022-10-24 06:11:18.000000 model_bakery-1.9.0/docs/source/test_runners.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.514335 model_bakery-1.9.0/model_bakery/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27032 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/baker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      333 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/generators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/gis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/mock_file.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/mock_img.jpeg
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     9046 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/random_gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8294 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4514 2022-10-24 06:11:18.000000 model_bakery-1.9.0/model_bakery/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.514335 model_bakery-1.9.0/model_bakery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3546 2022-10-24 06:11:27.000000 model_bakery-1.9.0/model_bakery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1384 2022-10-24 06:11:27.000000 model_bakery-1.9.0/model_bakery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-10-24 06:11:27.000000 model_bakery-1.9.0/model_bakery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2022-10-24 06:11:27.000000 model_bakery-1.9.0/model_bakery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2022-10-24 06:11:27.000000 model_bakery-1.9.0/model_bakery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2022-10-24 06:11:18.000000 model_bakery-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2022-10-24 06:11:18.000000 model_bakery-1.9.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2022-10-24 06:11:27.514335 model_bakery-1.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1622 2022-10-24 06:11:18.000000 model_bakery-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.514335 model_bakery-1.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.514335 model_bakery-1.9.0/tests/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/ambiguous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/ambiguous/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.514335 model_bakery-1.9.0/tests/ambiguous2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/ambiguous2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/ambiguous2/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2695 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.514335 model_bakery-1.9.0/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2938 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/generic/baker_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/generic/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/generic/forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/generic/generators.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13907 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/generic/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.510334 model_bakery-1.9.0/tests/generic/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.514335 model_bakery-1.9.0/tests/generic/tests/sub_package/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/generic/tests/sub_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/generic/tests/sub_package/baker_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40665 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/test_baker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3746 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/test_extending_bakery.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23402 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/test_filling_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25948 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/test_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6575 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.514335 model_bakery-1.9.0/tests/uninstalled/
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tests/uninstalled/baker_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2022-10-24 06:11:18.000000 model_bakery-1.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-10-24 06:11:27.514335 model_bakery-1.9.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3211 2022-10-24 06:11:18.000000 model_bakery-1.9.0/utils/from_mommy_to_bakery.py
```

### Comparing `model_bakery-1.8.0/CHANGELOG.md` & `model_bakery-1.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 ### Added
 
 ### Changed
 
 ### Removed
 
+## [1.9.0](https://pypi.org/project/model-bakery/1.9.0/)
+- Fixed a bug with `seq` being passed a tz-aware start value [PR #353](https://github.com/model-bakers/model_bakery/pull/353)
+- Create m2m when using `_bulk_create=True` [PR #354](https://github.com/model-bakers/model_bakery/pull/354)
+- [dev] Use official postgis docker image in CI [PR #355](https://github.com/model-bakers/model_bakery/pull/355)
+
 ## [1.8.0](https://pypi.org/project/model-bakery/1.8.0/)
 
 ### Changed
 - Improve `Baker.get_fields()` to subtract lists instead of extra set cast [PR #352](https://github.com/model-bakers/model_bakery/pull/352)
 
 ## [1.7.1](https://pypi.org/project/model-bakery/1.7.1/)
```

### Comparing `model_bakery-1.8.0/CONTRIBUTING.md` & `model_bakery-1.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/LICENSE` & `model_bakery-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/PKG-INFO` & `model_bakery-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model_bakery
-Version: 1.8.0
+Version: 1.9.0
 Summary: Smart object creation facility for Django.
 Home-page: https://github.com/model-bakers/model_bakery
 Author: berin
 Author-email: bernardoxhc@gmail.com
 License: Apache 2.0
 Keywords: django testing factory python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `model_bakery-1.8.0/README.md` & `model_bakery-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/docs/source/basic_usage.rst` & `model_bakery-1.9.0/docs/source/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/docs/source/how_bakery_behaves.rst` & `model_bakery-1.9.0/docs/source/how_bakery_behaves.rst`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/docs/source/index.rst` & `model_bakery-1.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/docs/source/migrating_from_mommy.rst` & `model_bakery-1.9.0/docs/source/migrating_from_mommy.rst`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/docs/source/recipes.rst` & `model_bakery-1.9.0/docs/source/recipes.rst`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/docs/source/test_runners.rst` & `model_bakery-1.9.0/docs/source/test_runners.rst`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/model_bakery/baker.py` & `model_bakery-1.9.0/model_bakery/baker.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Optional,
     Type,
     Union,
     cast,
     overload,
 )
 
+from django import VERSION as DJANGO_VERSION
 from django.apps import apps
 from django.conf import settings
 from django.contrib import contenttypes
 from django.db.models import (
     AutoField,
     BooleanField,
     Field,
@@ -783,8 +784,31 @@
     if baker._using:
         # Try to use the desired DB and let Django fail if spanning
         # relationships without the proper router setup
         manager = baker.model._base_manager.using(baker._using)
     else:
         manager = baker.model._base_manager
 
-    return manager.bulk_create(entries)
+    existing_entries = list(manager.values_list("pk", flat=True))
+    created_entries = manager.bulk_create(entries)
+    # bulk_create in Django < 4.0 does not return ids of created objects.
+    #  drop this after 01 Apr 2024 (Django 3.2 LTS end of life)
+    if DJANGO_VERSION < (4, 0):
+        created_entries = manager.exclude(pk__in=existing_entries)
+
+    # set many-to-many relations from kwargs
+    for entry in created_entries:
+        for field in baker.model._meta.many_to_many:
+            if field.name in kwargs:
+                through_model = getattr(entry, field.name).through
+                through_model.objects.bulk_create(
+                    [
+                        through_model(
+                            **{
+                                field.remote_field.name: entry,
+                                field.related_model._meta.model_name: obj,
+                            }
+                        )
+                        for obj in kwargs[field.name]
+                    ]
+                )
+    return created_entries
```

### Comparing `model_bakery-1.8.0/model_bakery/generators.py` & `model_bakery-1.9.0/model_bakery/generators.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/model_bakery/gis.py` & `model_bakery-1.9.0/model_bakery/gis.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/model_bakery/mock_img.jpeg` & `model_bakery-1.9.0/model_bakery/mock_img.jpeg`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/model_bakery/random_gen.py` & `model_bakery-1.9.0/model_bakery/random_gen.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/model_bakery/recipe.py` & `model_bakery-1.9.0/model_bakery/recipe.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/model_bakery/utils.py` & `model_bakery-1.9.0/model_bakery/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,16 @@
             date = datetime.datetime.combine(value, datetime.datetime.now().time())
         elif type(value) is datetime.time:
             date = datetime.datetime.combine(datetime.date.today(), value)
         else:
             date = value
 
         # convert to epoch time
-        start = (date - datetime.datetime(1970, 1, 1)).total_seconds()
+        epoch_datetime = datetime.datetime(1970, 1, 1, tzinfo=date.tzinfo)
+        start = (date - epoch_datetime).total_seconds()
         increment_by = increment_by.total_seconds()
         for n in itertools.count(increment_by, increment_by):
             series_date = tz_aware(datetime.datetime.utcfromtimestamp(start + n))
             if type(value) is datetime.time:
                 yield series_date.time()
             elif type(value) is datetime.date:
                 yield series_date.date()
```

### Comparing `model_bakery-1.8.0/model_bakery.egg-info/PKG-INFO` & `model_bakery-1.9.0/model_bakery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-bakery
-Version: 1.8.0
+Version: 1.9.0
 Summary: Smart object creation facility for Django.
 Home-page: https://github.com/model-bakers/model_bakery
 Author: berin
 Author-email: bernardoxhc@gmail.com
 License: Apache 2.0
 Keywords: django testing factory python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `model_bakery-1.8.0/model_bakery.egg-info/SOURCES.txt` & `model_bakery-1.9.0/model_bakery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/setup.py` & `model_bakery-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/tests/conftest.py` & `model_bakery-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/tests/generic/baker_recipes.py` & `model_bakery-1.9.0/tests/generic/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/tests/generic/models.py` & `model_bakery-1.9.0/tests/generic/models.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/tests/test_baker.py` & `model_bakery-1.9.0/tests/test_baker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import itertools
 from decimal import Decimal
 from unittest.mock import patch
 
 import pytest
+from django import VERSION as DJANGO_VERSION
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.db.models import Manager
 from django.db.models.signals import m2m_changed
 from django.test import TestCase, override_settings
 
 from model_bakery import baker, random_gen
@@ -147,25 +148,26 @@
         assert models.Person.objects.count() == 5
 
         with self.assertNumQueries(5):
             people = baker.make(models.Person, _quantity=5, name="George Washington")
             assert all(p.name == "George Washington" for p in people)
 
     def test_make_quantity_respecting_bulk_create_parameter(self):
-        with self.assertNumQueries(1):
+        query_count = 2 if DJANGO_VERSION >= (4, 0) else 3
+        with self.assertNumQueries(query_count):
             baker.make(models.Person, _quantity=5, _bulk_create=True)
         assert models.Person.objects.count() == 5
 
-        with self.assertNumQueries(1):
+        with self.assertNumQueries(query_count):
             people = baker.make(
                 models.Person, name="George Washington", _quantity=5, _bulk_create=True
             )
             assert all(p.name == "George Washington" for p in people)
 
-        with self.assertNumQueries(1):
+        with self.assertNumQueries(query_count):
             baker.make(models.NonStandardManager, _quantity=3, _bulk_create=True)
             assert getattr(models.NonStandardManager, "objects", None) is None
             assert (
                 models.NonStandardManager._base_manager
                 == models.NonStandardManager.manager
             )
             assert (
@@ -358,49 +360,51 @@
 
     def test_create_multiple_one_to_one(self):
         baker.make(models.LonelyPerson, _quantity=5)
         assert models.LonelyPerson.objects.all().count() == 5
         assert models.Person.objects.all().count() == 5
 
     def test_bulk_create_multiple_one_to_one(self):
-        with self.assertNumQueries(6):
+        query_count = 7 if DJANGO_VERSION >= (4, 0) else 8
+        with self.assertNumQueries(query_count):
             baker.make(models.LonelyPerson, _quantity=5, _bulk_create=True)
 
         assert models.LonelyPerson.objects.all().count() == 5
         assert models.Person.objects.all().count() == 5
 
     def test_chaining_bulk_create_reduces_query_count(self):
-        qtd = 5
-        with self.assertNumQueries(3):
-            baker.make(models.Person, _quantity=qtd, _bulk_create=True)
+        query_count = 5 if DJANGO_VERSION >= (4, 0) else 7
+        with self.assertNumQueries(query_count):
+            baker.make(models.Person, _quantity=5, _bulk_create=True)
             person_iter = models.Person.objects.all().iterator()
             baker.make(
                 models.LonelyPerson,
                 only_friend=person_iter,
                 _quantity=5,
                 _bulk_create=True,
             )
             # 2 bulk create and 1 select on Person
 
         assert models.LonelyPerson.objects.all().count() == 5
         assert models.Person.objects.all().count() == 5
 
     def test_bulk_create_multiple_fk(self):
-        with self.assertNumQueries(6):
+        query_count = 7 if DJANGO_VERSION >= (4, 0) else 8
+        with self.assertNumQueries(query_count):
             baker.make(models.PaymentBill, _quantity=5, _bulk_create=True)
 
         assert models.PaymentBill.objects.all().count() == 5
         assert models.User.objects.all().count() == 5
 
     def test_create_many_to_many_if_flagged(self):
         store = baker.make(models.Store, make_m2m=True)
         assert store.employees.count() == 5
         assert store.customers.count() == 5
 
-    def test_regresstion_many_to_many_field_is_accepted_as_kwargs(self):
+    def test_regression_many_to_many_field_is_accepted_as_kwargs(self):
         employees = baker.make(models.Person, _quantity=3)
         customers = baker.make(models.Person, _quantity=3)
 
         store = baker.make(models.Store, employees=employees, customers=customers)
 
         assert store.employees.count() == 3
         assert store.customers.count() == 3
@@ -1028,7 +1032,20 @@
 
         movie = baker.make(
             models.MovieWithAnnotation,
             title="Old Boy",
             _from_manager="objects",
         )
         assert movie.title == movie.name
+
+
+class TestCreateM2MWhenBulkCreate(TestCase):
+    @pytest.mark.django_db
+    def test_create(self):
+        query_count = 13 if DJANGO_VERSION >= (4, 0) else 14
+        with self.assertNumQueries(query_count):
+            person = baker.make(models.Person)
+            baker.make(
+                models.Classroom, students=[person], _quantity=10, _bulk_create=True
+            )
+        c1, c2 = models.Classroom.objects.all()[:2]
+        assert list(c1.students.all()) == list(c2.students.all()) == [person]
```

### Comparing `model_bakery-1.8.0/tests/test_extending_bakery.py` & `model_bakery-1.9.0/tests/test_extending_bakery.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/tests/test_filling_fields.py` & `model_bakery-1.9.0/tests/test_filling_fields.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/tests/test_recipes.py` & `model_bakery-1.9.0/tests/test_recipes.py`

 * *Files identical despite different names*

### Comparing `model_bakery-1.8.0/tests/test_utils.py` & `model_bakery-1.9.0/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,28 +142,38 @@
         assert next(sequence) == datetime.time(18, 36, 58, 457698)
 
     @pytest.mark.parametrize("use_tz", [False, True])
     def test_datetime(self, settings, use_tz):
         settings.USE_TZ = use_tz
         tzinfo = datetime.timezone.utc if use_tz else None
 
+        # Starting with tz-unaware (naive) datetime
         sequence = seq(
             datetime.datetime(2021, 2, 11, 15, 39, 58, 457698),
             increment_by=datetime.timedelta(hours=3),
         )
         assert next(sequence) == datetime.datetime(
             2021, 2, 11, 18, 39, 58, 457698
         ).replace(tzinfo=tzinfo)
         assert next(sequence) == datetime.datetime(
             2021, 2, 11, 21, 39, 58, 457698
         ).replace(tzinfo=tzinfo)
         assert next(sequence) == datetime.datetime(
             2021, 2, 12, 00, 39, 58, 457698
         ).replace(tzinfo=tzinfo)
 
+        # Starting with tz-aware datetime
+        sequence = seq(
+            datetime.datetime(2021, 2, 11, 15, 39, 58, 457698, tzinfo=tzinfo),
+            increment_by=datetime.timedelta(hours=3),
+        )
+        assert next(sequence) == datetime.datetime(
+            2021, 2, 11, 18, 39, 58, 457698
+        ).replace(tzinfo=tzinfo)
+
     @pytest.mark.parametrize(
         "value",
         [
             datetime.datetime(2021, 2, 11, 15, 39, 58, 457698),
             datetime.date(2021, 2, 11),
             datetime.time(15, 39, 58, 457698),
         ],
```

### Comparing `model_bakery-1.8.0/tox.ini` & `model_bakery-1.9.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     3.11: py311
 
 [testenv]
 setenv =
     PYTHONPATH={toxinidir}
     postgresql: TEST_DB=postgis
     postgresql: PGUSER=postgres
+    postgresql: PGPASSWORD=postgres
     sqlite: TEST_DB=sqlite
     sqlite: USE_TZ=True
 deps =
     pillow
     pytest
     pytest-django
     django32: Django==3.2
```

### Comparing `model_bakery-1.8.0/utils/from_mommy_to_bakery.py` & `model_bakery-1.9.0/utils/from_mommy_to_bakery.py`

 * *Files identical despite different names*

