# Comparing `tmp/ocdsextensionregistry-0.2.1.tar.gz` & `tmp/ocdsextensionregistry-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdsextensionregistry-0.2.1.tar", last modified: Wed May 24 20:51:21 2023, max compression
+gzip compressed data, was "ocdsextensionregistry-0.2.2.tar", last modified: Mon Jun  5 20:53:07 2023, max compression
```

## Comparing `ocdsextensionregistry-0.2.1.tar` & `ocdsextensionregistry-0.2.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.334182 ocdsextensionregistry-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.334182 ocdsextensionregistry-0.2.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/codelist_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/extension_registry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/extension_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/profile_builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/translation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.338183 ocdsextensionregistry-0.2.1/ocdsextensionregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/codelist_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.338183 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.338183 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.338183 ocdsextensionregistry-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/commands/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/commands/test_generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/commands/test_generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/commands/test_none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/fixtures/location-v1.1.4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/tests/fixtures/ocds_coveredBy_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/fixtures/ocds_coveredBy_extension/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_codelist_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.309322 ocdsextensionregistry-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.309322 ocdsextensionregistry-0.2.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/codelist_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/extension_registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/extension_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/profile_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.313322 ocdsextensionregistry-0.2.2/ocdsextensionregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/codelist_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.313322 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.313322 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/commands/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/commands/test_generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/commands/test_generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/commands/test_none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/fixtures/location-v1.1.4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/tests/fixtures/ocds_coveredBy_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/fixtures/ocds_coveredBy_extension/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_codelist_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tox.ini
```

### Comparing `ocdsextensionregistry-0.2.1/LICENSE` & `ocdsextensionregistry-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/PKG-INFO` & `ocdsextensionregistry-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.2.1
+Version: 0.2.2
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.2.1/README.rst` & `ocdsextensionregistry-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/docs/Makefile` & `ocdsextensionregistry-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/docs/changelog.rst` & `ocdsextensionregistry-0.2.2/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.2.2 (2023-06-05)
+------------------
+
+-  fix: :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_full_name` and :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_name` return the correct name for GitLab URLs.
+-  fix: Clarify error message for ``AttributeError`` on :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_full_name`, :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_name`, and :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_user`.
+
 0.2.1 (2023-05-24)
 ------------------
 
 -  feat: Add a ``--no-frozen`` option to all commands.
 -  Drop Python 3.7 support.
 
 0.2.0 (2022-10-29)
```

### Comparing `ocdsextensionregistry-0.2.1/docs/cli.rst` & `ocdsextensionregistry-0.2.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/docs/conf.py` & `ocdsextensionregistry-0.2.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Extension Registry Python Package"
 copyright = "2018, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.2.1"
+version = "0.2.2"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdsextensionregistry-0.2.1/docs/index.rst` & `ocdsextensionregistry-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/docs/translation.rst` & `ocdsextensionregistry-0.2.2/docs/translation.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/__init__.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/__main__.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/api.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/codelist.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/codelist_code.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/base.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/base.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/download.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/generate_data_file.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/generate_pot_files.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/exceptions.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension_registry.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension_version.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -256,21 +256,30 @@
         modification, e.g. https://github.com/open-contracting-extensions/ocds_bid_extension.git
 
         Experimental
         """
         return self._repository_property('url')
 
     def _repository_full_name(self, parsed, config):
-        return re.match(config['full_name:pattern'], parsed.path).group(1)
+        match = re.search(config['full_name:pattern'], parsed.path)
+        if match:
+            return match.group(1)
+        raise AttributeError(f"{parsed.path} !~ {config['full_name:pattern']}")
 
     def _repository_name(self, parsed, config):
-        return re.match(config['name:pattern'], parsed.path).group(1)
+        match = re.search(config['name:pattern'], parsed.path)
+        if match:
+            return match.group(1)
+        raise AttributeError(f"{parsed.path} !~ {config['name:pattern']}")
 
     def _repository_user(self, parsed, config):
-        return re.match(config['user:pattern'], parsed.path).group(1)
+        match = re.search(config['user:pattern'], parsed.path)
+        if match:
+            return match.group(1)
+        raise AttributeError(f"{parsed.path} !~ {config['user:pattern']}")
 
     def _repository_user_page(self, parsed, config):
         return config['html_page:prefix'] + self._repository_user(parsed, config)
 
     def _repository_html_page(self, parsed, config):
         return config['html_page:prefix'] + self._repository_full_name(parsed, config)
 
@@ -313,14 +322,14 @@
                 'html_page:prefix': 'https://bitbucket.org/',
                 'url:prefix': 'https://bitbucket.org/',
                 'url:suffix': '.git',  # assumes Git not Mercurial, which can't be disambiguated using the base URL
             }
         if netloc == 'gitlab.com':
             # A base URL may look like: https://gitlab.com/gitlab-org/gitter/env/raw/master/
             return {
-                'full_name:pattern': r'\A/(.+)/raw/',
-                'name:pattern': r'/([^/]+)/raw/',
+                'full_name:pattern': r'\A/(.+)/-/raw/',
+                'name:pattern': r'/([^/]+)/-/raw/',
                 'user:pattern': r'\A/([^/]+)',
                 'html_page:prefix': 'https://gitlab.com/',
                 'url:prefix': 'https://gitlab.com/',
                 'url:suffix': '.git',
             }
```

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/profile_builder.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry/util.py` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry/util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/PKG-INFO` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.2.1
+Version: 0.2.2
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/SOURCES.txt` & `ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/setup.cfg` & `ocdsextensionregistry-0.2.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ocdsextensionregistry
-version = 0.2.1
+version = 0.2.2
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = Eases access to information from the extension registry of the Open Contracting Data Standard
 url = https://github.com/open-contracting/extension_registry.py
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `ocdsextensionregistry-0.2.1/tests/commands/test_download.py` & `ocdsextensionregistry-0.2.2/tests/commands/test_download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/commands/test_generate_data_file.py` & `ocdsextensionregistry-0.2.2/tests/commands/test_generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/commands/test_generate_pot_files.py` & `ocdsextensionregistry-0.2.2/tests/commands/test_generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/fixtures/location-v1.1.4.json` & `ocdsextensionregistry-0.2.2/tests/fixtures/location-v1.1.4.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/fixtures/ocds_coveredBy_extension/release-schema.json` & `ocdsextensionregistry-0.2.2/tests/fixtures/ocds_coveredBy_extension/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/test_api.py` & `ocdsextensionregistry-0.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/test_codelist.py` & `ocdsextensionregistry-0.2.2/tests/test_codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/test_codelist_code.py` & `ocdsextensionregistry-0.2.2/tests/test_codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/test_extension.py` & `ocdsextensionregistry-0.2.2/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/test_extension_registry.py` & `ocdsextensionregistry-0.2.2/tests/test_extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/test_extension_version.py` & `ocdsextensionregistry-0.2.2/tests/test_extension_version.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/test_profile_builder.py` & `ocdsextensionregistry-0.2.2/tests/test_profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tests/test_util.py` & `ocdsextensionregistry-0.2.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.1/tox.ini` & `ocdsextensionregistry-0.2.2/tox.ini`

 * *Files identical despite different names*

