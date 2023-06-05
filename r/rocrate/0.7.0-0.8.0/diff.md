# Comparing `tmp/rocrate-0.7.0.tar.gz` & `tmp/rocrate-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocrate-0.7.0.tar", last modified: Mon May 30 15:13:51 2022, max compression
+gzip compressed data, was "rocrate-0.8.0.tar", last modified: Mon Jun  5 13:30:49 2023, max compression
```

## Comparing `rocrate-0.7.0.tar` & `rocrate-0.8.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 15:13:51.305936 rocrate-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-05-30 15:13:31.000000 rocrate-0.7.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-05-30 15:13:31.000000 rocrate-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-30 15:13:31.000000 rocrate-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13682 2022-05-30 15:13:51.305936 rocrate-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12401 2022-05-30 15:13:31.000000 rocrate-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-30 15:13:31.000000 rocrate-0.7.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 15:13:51.297936 rocrate-0.7.0/rocrate/
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5071 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 15:13:51.301936 rocrate-0.7.0/rocrate/data/
--rw-r--r--   0 runner    (1001) docker     (121)   164469 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/data/ro-crate.jsonld
--rw-r--r--   0 runner    (1001) docker     (121)  1478612 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/data/schema.jsonld
--rw-r--r--   0 runner    (1001) docker     (121)     4717 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 15:13:51.301936 rocrate-0.7.0/rocrate/model/
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/computationalworkflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     5256 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/computerlanguage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/contextentity.py
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/creativework.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/data_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2547 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5040 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/file_or_dir.py
--rw-r--r--   0 runner    (1001) docker     (121)     4124 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/person.py
--rw-r--r--   0 runner    (1001) docker     (121)     3166 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/preview.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/root_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/softwareapplication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/testdefinition.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/testinstance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/testservice.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/model/testsuite.py
--rw-r--r--   0 runner    (1001) docker     (121)    20137 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/rocrate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 15:13:51.301936 rocrate-0.7.0/rocrate/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     7173 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/templates/preview_template.html.j2
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2022-05-30 15:13:31.000000 rocrate-0.7.0/rocrate/vocabs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 15:13:51.297936 rocrate-0.7.0/rocrate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13682 2022-05-30 15:13:51.000000 rocrate-0.7.0/rocrate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-05-30 15:13:51.000000 rocrate-0.7.0/rocrate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 15:13:51.000000 rocrate-0.7.0/rocrate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-30 15:13:51.000000 rocrate-0.7.0/rocrate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-30 15:13:51.000000 rocrate-0.7.0/rocrate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-30 15:13:51.000000 rocrate-0.7.0/rocrate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-05-30 15:13:51.305936 rocrate-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3887 2022-05-30 15:13:31.000000 rocrate-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 15:13:51.305936 rocrate-0.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3678 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    11301 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6872 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    16293 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    15984 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/test_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/test_readwrite.py
--rw-r--r--   0 runner    (1001) docker     (121)    10962 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/test_test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4947 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/test_workflow_ro_crate.py
--rw-r--r--   0 runner    (1001) docker     (121)    13071 2022-05-30 15:13:31.000000 rocrate-0.7.0/test/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:30:49.752848 rocrate-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-05 13:30:25.000000 rocrate-0.8.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-05 13:30:25.000000 rocrate-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 13:30:25.000000 rocrate-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-06-05 13:30:49.752848 rocrate-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-06-05 13:30:25.000000 rocrate-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 13:30:25.000000 rocrate-0.8.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:30:49.748848 rocrate-0.8.0/rocrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:30:49.748848 rocrate-0.8.0/rocrate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   164469 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/data/ro-crate.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)  1478612 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/data/schema.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:30:49.752848 rocrate-0.8.0/rocrate/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/computationalworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/computerlanguage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/contextentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/creativework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/data_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/file_or_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/root_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/softwareapplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/testdefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/testinstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/testservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/model/testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/rocrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:30:49.752848 rocrate-0.8.0/rocrate/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/templates/preview_template.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-05 13:30:25.000000 rocrate-0.8.0/rocrate/vocabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:30:49.748848 rocrate-0.8.0/rocrate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-06-05 13:30:49.000000 rocrate-0.8.0/rocrate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-05 13:30:49.000000 rocrate-0.8.0/rocrate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:30:49.000000 rocrate-0.8.0/rocrate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-05 13:30:49.000000 rocrate-0.8.0/rocrate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 13:30:49.000000 rocrate-0.8.0/rocrate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 13:30:49.000000 rocrate-0.8.0/rocrate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-05 13:30:49.752848 rocrate-0.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3919 2023-06-05 13:30:25.000000 rocrate-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:30:49.752848 rocrate-0.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/test_jsonld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16900 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/test_readwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/test_test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/test_workflow_ro_crate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15237 2023-06-05 13:30:25.000000 rocrate-0.8.0/test/test_write.py
```

### Comparing `rocrate-0.7.0/CITATION.cff` & `rocrate-0.8.0/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     orcid: https://orcid.org/0000-0002-6190-122X
   - family-names: Gaignard
     given-names: Alban
     orcid: https://orcid.org/0000-0002-3597-8557
   - family-names: Huber
     given-names: Sebastiaan
     orcid: https://orcid.org/0000-0001-5845-8880
+  - family-names: Kinoshita
+    given-names: Bruno
+    orcid: https://orcid.org/0000-0001-8250-4074
   - family-names: Leo
     given-names: Simone
     orcid: https://orcid.org/0000-0001-8271-5429
   - family-names: Pireddu
     given-names: Luca
     orcid: https://orcid.org/0000-0002-4663-5613
   - family-names: Rodríguez-Navas
@@ -28,10 +31,10 @@
   - family-names: Sirvent
     given-names: Raül
     orcid: https://orcid.org/0000-0003-0606-2512
   - family-names: Soiland-Reyes
     given-names: Stian
     orcid: https://orcid.org/0000-0001-9842-9718
 title: "ro-crate-py"
-version: 0.7.0
+version: 0.8.0
 doi: 10.5281/zenodo.3956493
-date-released: 2022-05-30
+date-released: 2023-06-05
```

### Comparing `rocrate-0.7.0/LICENSE` & `rocrate-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rocrate-0.7.0/PKG-INFO` & `rocrate-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: rocrate
-Version: 0.7.0
+Version: 0.8.0
 Summary: RO-Crate metadata generator/parser
 Home-page: https://github.com/ResearchObject/ro-crate-py/
-Author: Paul De Geest, Bert Droesbeke, Ignacio Eguinoa, Alban Gaignard, Sebastiaan Huber, Simone Leo, Luca Pireddu, Laura Rodríguez-Navas, Raül Sirvent, Stian Soiland-Reyes
+Download-URL: https://github.com/researchobject/ro-crate-py/archive/0.8.0.tar.gz
+Author: Paul De Geest, Bert Droesbeke, Ignacio Eguinoa, Alban Gaignard, Sebastiaan Huber, Bruno Kinoshita, Simone Leo, Luca Pireddu, Laura Rodríguez-Navas, Raül Sirvent, Stian Soiland-Reyes
 Author-email: stain@apache.org
 License: Apache-2.0
-Download-URL: https://github.com/researchobject/ro-crate-py/archive/0.7.0.tar.gz
 Keywords: researchobject ro-crate ro metadata jsonld
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -71,15 +70,15 @@
 })
 diagram = crate.add_file("exp/diagram.svg", dest_path="images/figure.svg", properties={
     "name": "bar chart",
     "encodingFormat": "image/svg+xml"
 })
 ```
 
-We've started by adding the data entitites. Now we need contextual entities to represent Alice and Bob:
+We've started by adding the data entities. Now we need contextual entities to represent Alice and Bob:
 
 ```python
 from rocrate.model.person import Person
 
 alice_id = "https://orcid.org/0000-0000-0000-0000"
 bob_id = "https://orcid.org/0000-0000-0000-0001"
 alice = crate.add(Person(crate, alice_id, properties={
@@ -116,14 +115,17 @@
 
 You can also add whole directories. A directory in RO-Crate is represented by the `Dataset` entity:
 
 ```python
 logs = crate.add_dataset("exp/logs")
 ```
 
+Note that the above adds all files and directories contained in `"exp/logs"` recursively to the crate, but only the top-level `"exp/logs"` dataset itself is listed in the metadata file (there is no requirement to represent every file and folder in the JSON-LD). To also add files and directory recursively to the metadata, use `add_tree` (but note that it only works on local directory trees).
+
+
 #### Appending elements to property values
 
 What ro-crate-py entities actually store is their JSON representation:
 
 ```python
 paper.properties()
 ```
@@ -196,14 +198,68 @@
 
 Note that entities can have multiple types, e.g.:
 
 ```python
     "@type" = ["File", "SoftwareSourceCode"]
 ```
 
+#### Modifying the crate from JSON-LD dictionaries
+
+The `add_jsonld` method allows to add a contextual entity directly from a
+JSON-LD dictionary containing at least the `@id` and `@type` keys:
+
+```python
+crate.add_jsonld({
+    "@id": "https://orcid.org/0000-0000-0000-0000",
+    "@type": "Person",
+    "name": "Alice Doe"
+})
+```
+
+Existing entities can be updated from JSON-LD dictionaries via `update_jsonld`:
+
+```python
+crate.update_jsonld({
+    "@id": "https://orcid.org/0000-0000-0000-0000",
+    "name": "Alice K. Doe"
+})
+```
+
+There is also an `add_or_update_jsonld` method that adds the entity if it's
+not already in the crate and updates it if it already exists (note that, when
+updating, the `@type` key is ignored). This allows to "patch" an RO-Crate from
+a JSON-LD file. For instance, suppose you have the following `patch.json` file:
+
+```json
+{
+    "@graph": [
+        {
+            "@id": "./",
+            "author": {"@id": "https://orcid.org/0000-0000-0000-0001"}
+        },
+        {
+            "@id": "https://orcid.org/0000-0000-0000-0001",
+            "@type": "Person",
+            "name": "Bob Doe"
+        }
+    ]
+}
+```
+
+Then the following sets Bob as the author of the crate according to the above
+file:
+
+```python
+crate = ROCrate("temp-crate")
+with open("patch.json") as f:
+    json_data = json.load(f)
+for d in json_data.get("@graph", []):
+    crate.add_or_update_jsonld(d)
+```
+
 ### Consuming an RO-Crate
 
 An existing RO-Crate package can be loaded from a directory or zip file:
 
 ```python
 crate = ROCrate('exp_crate')  # or ROCrate('exp_crate.zip')
 for e in crate.get_entities():
@@ -303,15 +359,15 @@
 ### Example
 
 ```bash
 # From the ro-crate-py repository root
 cd test/test-data/ro-crate-galaxy-sortchangecase
 ```
 
-This directory is already an ro-crate. Delete the metadata file to get a plain directory tree:
+This directory is already an RO-Crate. Delete the metadata file to get a plain directory tree:
 
 ```bash
 rm ro-crate-metadata.json
 ```
 
 Now the directory tree contains several files and directories, including a Galaxy workflow and a Planemo test file, but it's not an RO-Crate since there is no metadata file. Initialize the crate:
 
@@ -330,40 +386,37 @@
 
 To register the workflow as a `ComputationalWorkflow`:
 
 ```bash
 rocrate add workflow -l galaxy sort-and-change-case.ga
 ```
 
-Now the workflow has a type of `["File", "SoftwareSourceCode", "ComputationalWorkflow"]` and points to a `ComputerLanguage` entity that represents the Galaxy workflow language. Also, the workflow is listed as the crate's `mainEntity` (see https://about.workflowhub.eu/Workflow-RO-Crate).
+Now the workflow has a type of `["File", "SoftwareSourceCode", "ComputationalWorkflow"]` and points to a `ComputerLanguage` entity that represents the Galaxy workflow language. Also, the workflow is listed as the crate's `mainEntity` (see the [Workflow RO-Crate profile](https://w3id.org/workflowhub/workflow-ro-crate/1.0)).
 
-To add [workflow testing metadata](https://github.com/crs4/life_monitor/wiki/Workflow-Testing-RO-Crate) to the crate:
+To add [workflow testing metadata](https://crs4.github.io/life_monitor/workflow_testing_ro_crate) to the crate:
 
 ```bash
 rocrate add test-suite -i test1
 rocrate add test-instance test1 http://example.com -r jobs -i test1_1
 rocrate add test-definition test1 test/test1/sort-and-change-case-test.yml -e planemo -v '>=0.70'
 ```
 
-
 ## License
 
- * Copyright 2019-2022 The University of Manchester, UK
- * Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
- * Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
- * Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
- * Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+ * Copyright 2019-2023 The University of Manchester, UK
+ * Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+ * Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+ * Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+ * Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 
 Licensed under the 
 Apache License, version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>, 
 see the file `LICENSE.txt` for details.
 
 ## Cite as
 
 [![DOI](https://zenodo.org/badge/216605684.svg)](https://zenodo.org/badge/latestdoi/216605684)
 
 The above DOI corresponds to the latest versioned release as [published to Zenodo](https://zenodo.org/record/3956493), where you will find all earlier releases. 
 To cite `ro-crate-py` independent of version, use <https://doi.org/10.5281/zenodo.3956493>, which will always redirect to the latest release.
 
 You may also be interested in the paper [Packaging research artefacts with RO-Crate](https://doi.org/10.3233/DS-210053).
-
-
```

### Comparing `rocrate-0.7.0/README.md` & `rocrate-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 })
 diagram = crate.add_file("exp/diagram.svg", dest_path="images/figure.svg", properties={
     "name": "bar chart",
     "encodingFormat": "image/svg+xml"
 })
 ```
 
-We've started by adding the data entitites. Now we need contextual entities to represent Alice and Bob:
+We've started by adding the data entities. Now we need contextual entities to represent Alice and Bob:
 
 ```python
 from rocrate.model.person import Person
 
 alice_id = "https://orcid.org/0000-0000-0000-0000"
 bob_id = "https://orcid.org/0000-0000-0000-0001"
 alice = crate.add(Person(crate, alice_id, properties={
@@ -87,14 +87,17 @@
 
 You can also add whole directories. A directory in RO-Crate is represented by the `Dataset` entity:
 
 ```python
 logs = crate.add_dataset("exp/logs")
 ```
 
+Note that the above adds all files and directories contained in `"exp/logs"` recursively to the crate, but only the top-level `"exp/logs"` dataset itself is listed in the metadata file (there is no requirement to represent every file and folder in the JSON-LD). To also add files and directory recursively to the metadata, use `add_tree` (but note that it only works on local directory trees).
+
+
 #### Appending elements to property values
 
 What ro-crate-py entities actually store is their JSON representation:
 
 ```python
 paper.properties()
 ```
@@ -167,14 +170,68 @@
 
 Note that entities can have multiple types, e.g.:
 
 ```python
     "@type" = ["File", "SoftwareSourceCode"]
 ```
 
+#### Modifying the crate from JSON-LD dictionaries
+
+The `add_jsonld` method allows to add a contextual entity directly from a
+JSON-LD dictionary containing at least the `@id` and `@type` keys:
+
+```python
+crate.add_jsonld({
+    "@id": "https://orcid.org/0000-0000-0000-0000",
+    "@type": "Person",
+    "name": "Alice Doe"
+})
+```
+
+Existing entities can be updated from JSON-LD dictionaries via `update_jsonld`:
+
+```python
+crate.update_jsonld({
+    "@id": "https://orcid.org/0000-0000-0000-0000",
+    "name": "Alice K. Doe"
+})
+```
+
+There is also an `add_or_update_jsonld` method that adds the entity if it's
+not already in the crate and updates it if it already exists (note that, when
+updating, the `@type` key is ignored). This allows to "patch" an RO-Crate from
+a JSON-LD file. For instance, suppose you have the following `patch.json` file:
+
+```json
+{
+    "@graph": [
+        {
+            "@id": "./",
+            "author": {"@id": "https://orcid.org/0000-0000-0000-0001"}
+        },
+        {
+            "@id": "https://orcid.org/0000-0000-0000-0001",
+            "@type": "Person",
+            "name": "Bob Doe"
+        }
+    ]
+}
+```
+
+Then the following sets Bob as the author of the crate according to the above
+file:
+
+```python
+crate = ROCrate("temp-crate")
+with open("patch.json") as f:
+    json_data = json.load(f)
+for d in json_data.get("@graph", []):
+    crate.add_or_update_jsonld(d)
+```
+
 ### Consuming an RO-Crate
 
 An existing RO-Crate package can be loaded from a directory or zip file:
 
 ```python
 crate = ROCrate('exp_crate')  # or ROCrate('exp_crate.zip')
 for e in crate.get_entities():
@@ -274,15 +331,15 @@
 ### Example
 
 ```bash
 # From the ro-crate-py repository root
 cd test/test-data/ro-crate-galaxy-sortchangecase
 ```
 
-This directory is already an ro-crate. Delete the metadata file to get a plain directory tree:
+This directory is already an RO-Crate. Delete the metadata file to get a plain directory tree:
 
 ```bash
 rm ro-crate-metadata.json
 ```
 
 Now the directory tree contains several files and directories, including a Galaxy workflow and a Planemo test file, but it's not an RO-Crate since there is no metadata file. Initialize the crate:
 
@@ -301,32 +358,31 @@
 
 To register the workflow as a `ComputationalWorkflow`:
 
 ```bash
 rocrate add workflow -l galaxy sort-and-change-case.ga
 ```
 
-Now the workflow has a type of `["File", "SoftwareSourceCode", "ComputationalWorkflow"]` and points to a `ComputerLanguage` entity that represents the Galaxy workflow language. Also, the workflow is listed as the crate's `mainEntity` (see https://about.workflowhub.eu/Workflow-RO-Crate).
+Now the workflow has a type of `["File", "SoftwareSourceCode", "ComputationalWorkflow"]` and points to a `ComputerLanguage` entity that represents the Galaxy workflow language. Also, the workflow is listed as the crate's `mainEntity` (see the [Workflow RO-Crate profile](https://w3id.org/workflowhub/workflow-ro-crate/1.0)).
 
-To add [workflow testing metadata](https://github.com/crs4/life_monitor/wiki/Workflow-Testing-RO-Crate) to the crate:
+To add [workflow testing metadata](https://crs4.github.io/life_monitor/workflow_testing_ro_crate) to the crate:
 
 ```bash
 rocrate add test-suite -i test1
 rocrate add test-instance test1 http://example.com -r jobs -i test1_1
 rocrate add test-definition test1 test/test1/sort-and-change-case-test.yml -e planemo -v '>=0.70'
 ```
 
-
 ## License
 
- * Copyright 2019-2022 The University of Manchester, UK
- * Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
- * Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
- * Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
- * Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+ * Copyright 2019-2023 The University of Manchester, UK
+ * Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+ * Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+ * Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+ * Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 
 Licensed under the 
 Apache License, version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>, 
 see the file `LICENSE.txt` for details.
 
 ## Cite as
```

### Comparing `rocrate-0.7.0/rocrate/__init__.py` & `rocrate-0.8.0/rocrate/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -29,25 +29,27 @@
 
 __author__ = ", ".join((
     'Paul De Geest',
     'Bert Droesbeke',
     'Ignacio Eguinoa',
     'Alban Gaignard',
     'Sebastiaan Huber',
+    'Bruno Kinoshita',
     'Simone Leo',
     'Luca Pireddu',
     'Laura Rodríguez-Navas',
     'Raül Sirvent',
     'Stian Soiland-Reyes'
 ))
 __copyright__ = """\
-Copyright 2019-2022 The University of Manchester, UK
-Copyright 2022 Vlaams Instituut voor Biotechnologie (VIB), DE
-Copyright 2022 Barcelona Supercomputing Center (BSC), ES
-Copyright 2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+Copyright 2019-2023 The University of Manchester, UK
+Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 """
 __license__ = ("Apache License, version 2.0 "
                "<https://www.apache.org/licenses/LICENSE-2.0>")
 
 # for arcp scheme registration with urllib.parse
 import arcp  # noqa
```

### Comparing `rocrate-0.7.0/rocrate/cli.py` & `rocrate-0.8.0/rocrate/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,18 +28,14 @@
 
 
 LANG_CHOICES = list(LANG_MAP)
 SERVICE_CHOICES = list(SERVICE_MAP)
 ENGINE_CHOICES = list(APP_MAP)
 
 
-class State:
-    pass
-
-
 class CSVParamType(click.ParamType):
     name = "csv"
 
     def convert(self, value, param, ctx):
         if isinstance(value, (list, tuple, set, frozenset)):
             return value
         try:
```

### Comparing `rocrate-0.7.0/rocrate/data/ro-crate.jsonld` & `rocrate-0.8.0/rocrate/data/ro-crate.jsonld`

 * *Files identical despite different names*

### Comparing `rocrate-0.7.0/rocrate/data/schema.jsonld` & `rocrate-0.8.0/rocrate/data/schema.jsonld`

 * *Files identical despite different names*

### Comparing `rocrate-0.7.0/rocrate/metadata.py` & `rocrate-0.8.0/rocrate/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/__init__.py` & `rocrate-0.8.0/rocrate/model/data_entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+#!/usr/bin/env python
+
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Model of RO-Crate metadata.
 
-This module intends to cover each of the data entities and contextual entities
-in rocrate_ represented as different Python classes.
+from .entity import Entity
+
+
+class DataEntity(Entity):
 
-.. _rocrate: https://w3id.org/ro/crate/
-"""
+    def write(self, base_path):
+        pass
```

### Comparing `rocrate-0.7.0/rocrate/model/computationalworkflow.py` & `rocrate-0.8.0/rocrate/model/computationalworkflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/computerlanguage.py` & `rocrate-0.8.0/rocrate/model/computerlanguage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -65,117 +65,136 @@
         return self.get("version")
 
     @version.setter
     def version(self, version):
         self["version"] = version
 
 
-# For workflow ro-crates. Note that
-# https://about.workflowhub.eu/Workflow-RO-Crate/ does not specify versions.
+# See https://w3id.org/workflowhub/workflow-ro-crate/1.0
+# (note that it does not specify "version")
 
-CWL_DEFAULT_VERSION = "1.2"
-# https://github.com/galaxyproject/gxformat2 has some info on gxformat2 versions
-# version can probably be simply ignored for "native" *.ga workflows
-GALAXY_DEFAULT_VERSION = "21.09"
-KNIME_DEFAULT_VERSION = "4.5.0"
-NEXTFLOW_DEFAULT_VERSION = "21.10"
-SNAKEMAKE_DEFAULT_VERSION = "6.13"
-COMPSS_DEFAULT_VERSION = "2.10"
 
-
-def cwl(crate, version=CWL_DEFAULT_VERSION):
+def cwl(crate, version=None):
     id_ = "https://w3id.org/workflowhub/workflow-ro-crate#cwl"
-    return ComputerLanguage(crate, identifier=id_, properties={
+    identifier = "https://w3id.org/cwl/"
+    if version:
+        identifier = f"{identifier}v{version}/"
+    properties = {
         "name": "Common Workflow Language",
         "alternateName": "CWL",
         "identifier": {
-            "@id": f"https://w3id.org/cwl/{version}/"
+            "@id": identifier
         },
         "url": {
             "@id": "https://www.commonwl.org/"
         },
-        "version": version
-    })
+    }
+    if version:
+        properties["version"] = version
+    return ComputerLanguage(crate, identifier=id_, properties=properties)
 
 
-def galaxy(crate, version=GALAXY_DEFAULT_VERSION):
+def galaxy(crate, version=None):
     id_ = "https://w3id.org/workflowhub/workflow-ro-crate#galaxy"
-    return ComputerLanguage(crate, identifier=id_, properties={
+    properties = {
         "name": "Galaxy",
         "identifier": {
             "@id": "https://galaxyproject.org/"
         },
         "url": {
             "@id": "https://galaxyproject.org/"
-        },
-        "version": version
-    })
+        }
+    }
+    if version:
+        properties["version"] = version
+    return ComputerLanguage(crate, identifier=id_, properties=properties)
 
 
-def knime(crate, version=KNIME_DEFAULT_VERSION):
+def knime(crate, version=None):
     id_ = "https://w3id.org/workflowhub/workflow-ro-crate#knime"
-    return ComputerLanguage(crate, identifier=id_, properties={
+    properties = {
         "name": "KNIME",
         "identifier": {
             "@id": "https://www.knime.com/"
         },
         "url": {
             "@id": "https://www.knime.com/"
-        },
-        "version": version
-    })
+        }
+    }
+    if version:
+        properties["version"] = version
+    return ComputerLanguage(crate, identifier=id_, properties=properties)
 
 
-def nextflow(crate, version=NEXTFLOW_DEFAULT_VERSION):
+def nextflow(crate, version=None):
     id_ = "https://w3id.org/workflowhub/workflow-ro-crate#nextflow"
-    return ComputerLanguage(crate, identifier=id_, properties={
+    properties = {
         "name": "Nextflow",
         "identifier": {
             "@id": "https://www.nextflow.io/"
         },
         "url": {
             "@id": "https://www.nextflow.io/"
-        },
-        "version": version
-    })
+        }
+    }
+    if version:
+        properties["version"] = version
+    return ComputerLanguage(crate, identifier=id_, properties=properties)
 
 
-def snakemake(crate, version=SNAKEMAKE_DEFAULT_VERSION):
+def snakemake(crate, version=None):
     id_ = "https://w3id.org/workflowhub/workflow-ro-crate#snakemake"
-    return ComputerLanguage(crate, identifier=id_, properties={
+    properties = {
         "name": "Snakemake",
         "identifier": {
             "@id": "https://doi.org/10.1093/bioinformatics/bts480"
         },
         "url": {
             "@id": "https://snakemake.readthedocs.io"
-        },
-        "version": version
-    })
+        }
+    }
+    if version:
+        properties["version"] = version
+    return ComputerLanguage(crate, identifier=id_, properties=properties)
 
 
-def compss(crate, version=COMPSS_DEFAULT_VERSION):
-    return ComputerLanguage(crate, identifier="#compss", properties={
+def compss(crate, version=None):
+    properties = {
         "name": "COMPSs Programming Model",
         "alternateName": "COMPSs",
         "url": "http://compss.bsc.es/",
-        "citation": "https://doi.org/10.1007/s10723-013-9272-5",
-        "version": version
-    })
+        "citation": "https://doi.org/10.1007/s10723-013-9272-5"
+    }
+    if version:
+        properties["version"] = version
+    return ComputerLanguage(crate, identifier="#compss", properties=properties)
+
+
+def autosubmit(crate, version=None):
+    properties = {
+        "name": "Autosubmit",
+        "alternateName": "AS",
+        "url": "https://autosubmit.readthedocs.io/",
+        "citation": "https://doi.org/10.1109/HPCSim.2016.7568429"
+    }
+    if version:
+        properties["version"] = version
+    return ComputerLanguage(crate, identifier="#autosubmit", properties=properties)
 
 
 LANG_MAP = {
     "cwl": cwl,
     "galaxy": galaxy,
     "knime": knime,
     "nextflow": nextflow,
     "snakemake": snakemake,
     "compss": compss,
+    "autosubmit": autosubmit,
 }
 
 
 def get_lang(crate, name, version=None):
     try:
         func = LANG_MAP[name.lower()]
     except KeyError:
         raise ValueError(f"Unknown language: {name}")
-    return func(crate, version=version) if version else func(crate)
+    return func(crate, version=version)
```

### Comparing `rocrate-0.7.0/rocrate/model/contextentity.py` & `rocrate-0.8.0/rocrate/model/contextentity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/creativework.py` & `rocrate-0.8.0/rocrate/model/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-#!/usr/bin/env python
-
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .entity import Entity
+"""
+Model of RO-Crate metadata.
 
+This module intends to cover each of the data entities and contextual entities
+in rocrate_ represented as different Python classes.
 
-class CreativeWork(Entity):
-    pass
+.. _rocrate: https://w3id.org/ro/crate/
+"""
```

### Comparing `rocrate-0.7.0/rocrate/model/data_entity.py` & `rocrate-0.8.0/rocrate/model/creativework.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 from .entity import Entity
 
 
-class DataEntity(Entity):
-
-    def write(self, base_path):
-        pass
+class CreativeWork(Entity):
+    pass
```

### Comparing `rocrate-0.7.0/rocrate/model/dataset.py` & `rocrate-0.8.0/rocrate/model/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import errno
+import os
 import shutil
 from pathlib import Path
 from urllib.request import urlopen
 
 from .file_or_dir import FileOrDir
 from ..utils import is_url, iso_now
 
@@ -44,17 +46,24 @@
         if is_url(str(self.source)):
             if self.validate_url and not self.fetch_remote:
                 with urlopen(self.source) as _:
                     self._jsonld['sdDatePublished'] = iso_now()
             if self.fetch_remote:
                 self.__get_parts(out_path)
         else:
-            out_path.mkdir(parents=True, exist_ok=True)
-            if not self.crate.source and self.source and Path(self.source).exists():
-                self.crate._copy_unlisted(self.source, out_path)
+            if self.source is None:
+                out_path.mkdir(parents=True, exist_ok=True)
+            else:
+                if not Path(self.source).exists():
+                    raise FileNotFoundError(
+                        errno.ENOENT, os.strerror(errno.ENOENT), str(self.source)
+                    )
+                out_path.mkdir(parents=True, exist_ok=True)
+                if not self.crate.source:
+                    self.crate._copy_unlisted(self.source, out_path)
 
     def __get_parts(self, out_path):
         out_path.mkdir(parents=True, exist_ok=True)
         base = self.source.rstrip("/")
         for entry in self._jsonld.get("hasPart", []):
             try:
                 part = entry["@id"]
```

### Comparing `rocrate-0.7.0/rocrate/model/entity.py` & `rocrate-0.8.0/rocrate/model/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,29 +28,29 @@
 class Entity(MutableMapping):
 
     def __init__(self, crate, identifier=None, properties=None):
         self.crate = crate
         if identifier:
             self.id = self.format_id(identifier)
         else:
-            self.id = "#%s" % uuid.uuid4()
+            self.id = f"#{uuid.uuid4()}"
         if properties:
             empty = self._empty()
             empty.update(properties)
             self._jsonld = empty
         else:
             self._jsonld = self._empty()
 
     # Format the given ID with rules appropriate for this type.
     # For example, Dataset (directory) data entities SHOULD end with /
     def format_id(self, identifier):
         return str(identifier)
 
     def __repr__(self):
-        return "<%s %s>" % (self.id, self.type)
+        return f"<{self.id} {self.type}>"
 
     def properties(self):
         return self._jsonld
 
     def as_jsonld(self):
         return self._jsonld
```

### Comparing `rocrate-0.7.0/rocrate/model/file.py` & `rocrate-0.8.0/rocrate/model/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 from pathlib import Path
 import shutil
 import urllib.request
+import warnings
 from http.client import HTTPResponse
 from io import BytesIO, StringIO
 
 from .file_or_dir import FileOrDir
 from ..utils import is_url, iso_now
 
 
@@ -55,11 +55,14 @@
                                 'encodingFormat': response.getheader('Content-Type')
                             })
                         if not self.fetch_remote:
                             self._jsonld['sdDatePublished'] = iso_now()
                     if self.fetch_remote:
                         out_file_path.parent.mkdir(parents=True, exist_ok=True)
                         urllib.request.urlretrieve(response.url, out_file_path)
-        elif os.path.isfile(self.source):
+        elif self.source is None:
+            # Allows to record a File entity whose @id does not exist, see #73
+            warnings.warn(f"No source for {self.id}")
+        else:
             out_file_path.parent.mkdir(parents=True, exist_ok=True)
             if not out_file_path.exists() or not out_file_path.samefile(self.source):
                 shutil.copy(self.source, out_file_path)
```

### Comparing `rocrate-0.7.0/rocrate/model/file_or_dir.py` & `rocrate-0.8.0/rocrate/model/file_or_dir.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/metadata.py` & `rocrate-0.8.0/rocrate/model/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/person.py` & `rocrate-0.8.0/rocrate/model/person.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/preview.py` & `rocrate-0.8.0/rocrate/model/preview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/root_dataset.py` & `rocrate-0.8.0/rocrate/model/root_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/softwareapplication.py` & `rocrate-0.8.0/rocrate/model/softwareapplication.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -50,15 +50,14 @@
 
     @version.setter
     def version(self, version):
         self["version"] = version
 
 
 PLANEMO_ID = "https://w3id.org/ro/terms/test#PlanemoEngine"
-PLANEMO_DEFAULT_VERSION = "0.74"
 
 
 def planemo(crate):
     return SoftwareApplication(crate, identifier=PLANEMO_ID, properties={
         "name": "Planemo",
         "url": {
             "@id": "https://github.com/galaxyproject/planemo"
```

### Comparing `rocrate-0.7.0/rocrate/model/testdefinition.py` & `rocrate-0.8.0/rocrate/model/testdefinition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/testinstance.py` & `rocrate-0.8.0/rocrate/model/testinstance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/testservice.py` & `rocrate-0.8.0/rocrate/model/testservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/model/testsuite.py` & `rocrate-0.8.0/rocrate/model/testsuite.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/rocrate.py` & `rocrate-0.8.0/rocrate/rocrate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,14 +16,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import errno
 import uuid
 import zipfile
 import atexit
+import os
 import shutil
 import tempfile
 
 from collections import OrderedDict
 from pathlib import Path
 from urllib.parse import urljoin
 
@@ -37,15 +38,15 @@
 from .model.metadata import WORKFLOW_PROFILE, Metadata, LegacyMetadata, TESTING_EXTRA_TERMS, metadata_class
 from .model.preview import Preview
 from .model.testdefinition import TestDefinition
 from .model.computationalworkflow import ComputationalWorkflow, WorkflowDescription, galaxy_to_abstract_cwl
 from .model.computerlanguage import ComputerLanguage, get_lang
 from .model.testinstance import TestInstance
 from .model.testservice import TestService, get_service
-from .model.softwareapplication import SoftwareApplication, get_app, PLANEMO_DEFAULT_VERSION
+from .model.softwareapplication import SoftwareApplication, get_app
 from .model.testsuite import TestSuite
 
 from .utils import is_url, subclasses, get_norm_value, walk
 from .metadata import read_metadata, find_root_entity_id
 
 
 def pick_type(json_entity, type_map, fallback=None):
@@ -319,14 +320,29 @@
             fetch_remote=fetch_remote,
             validate_url=validate_url,
             properties=properties
         ))
 
     add_directory = add_dataset
 
+    def add_tree(self, source, dest_path=None, properties=None):
+        if not source:
+            raise ValueError("source must refer to an existing local directory")
+        top = self.add_dataset(source, dest_path=dest_path)
+        dest_path = Path(top.id).as_posix()
+        for e in os.scandir(source):
+            dest = dest_path / Path(e.path).relative_to(source)
+            if e.is_file():
+                file_ = self.add_file(source=e.path, dest_path=dest)
+                top.append_to("hasPart", file_)
+            if e.is_dir():
+                dir_ = self.add_tree(e.path, dest_path=dest)
+                top.append_to("hasPart", dir_)
+        return top
+
     def add(self, *entities):
         """\
         Add one or more entities to this RO-Crate.
 
         If an entity with the same (canonical) id is already present in the
         crate, it will be replaced (as in Python dictionaries).
 
@@ -434,16 +450,15 @@
         workflow = self.add(cls(
             self, source=source, dest_path=dest_path, fetch_remote=fetch_remote,
             validate_url=validate_url, properties=properties
         ))
         if isinstance(lang, ComputerLanguage):
             assert lang.crate is self
         else:
-            kwargs = {"version": lang_version} if lang_version else {}
-            lang = get_lang(self, lang, **kwargs)
+            lang = get_lang(self, lang, version=lang_version)
             self.add(lang)
         lang_str = lang.id.rsplit("#", 1)[1]
         workflow.lang = lang
         if main:
             self.mainEntity = workflow
             profiles = set(_.rstrip("/") for _ in get_norm_value(self.metadata, "conformsTo"))
             profiles.add(WORKFLOW_PROFILE)
@@ -490,33 +505,101 @@
         self.metadata.extra_terms.update(TESTING_EXTRA_TERMS)
         return instance
 
     def add_test_definition(
             self, suite, source=None, dest_path=None, fetch_remote=False, validate_url=False, properties=None,
             engine="planemo", engine_version=None
     ):
-        if engine_version is None:
-            # FIXME: this should be engine-specific
-            engine_version = PLANEMO_DEFAULT_VERSION
         suite = self.__validate_suite(suite)
         definition = self.add(
             TestDefinition(self, source=source, dest_path=dest_path, fetch_remote=fetch_remote,
                            validate_url=validate_url, properties=properties)
         )
         if isinstance(engine, SoftwareApplication):
             assert engine.crate is self
         else:
             engine = get_app(self, engine)
             self.add(engine)
         definition.engine = engine
-        definition.engineVersion = engine_version
+        if engine_version is not None:
+            definition.engineVersion = engine_version
         suite.definition = definition
         self.metadata.extra_terms.update(TESTING_EXTRA_TERMS)
         return definition
 
+    def add_jsonld(self, jsonld):
+        """Add a JSON-LD dictionary as a contextual entity to the RO-Crate.
+
+        The `@id` and `@type` keys must be present in the JSON-LD dictionary.
+
+        Args:
+            jsonld: A JSON-LD dictionary containing at least `@id` and `@type`.
+        Return:
+            The entity added to the RO-Crate.
+        Raises:
+            ValueError: if the jsonld object is empty or None or if the
+                entity already exists (found via @id).
+        """
+        required_keys = {"@id", "@type"}
+        if not jsonld or not required_keys.issubset(jsonld):
+            raise ValueError("you must provide a non-empty JSON-LD dictionary with @id and @type set")
+        entity_id = jsonld.pop("@id")
+        if self.get(entity_id):
+            raise ValueError(f"entity {entity_id} already exists in the RO-Crate")
+        return self.add(ContextEntity(
+            self,
+            entity_id,
+            properties=jsonld
+        ))
+
+    def update_jsonld(self, jsonld):
+        """Update an entity in the RO-Crate from a JSON-LD dictionary.
+
+        An `@id` must be present in the JSON-LD dictionary. Any other keys
+        in the JSON-LD dictionary that start with `@` will be removed.
+
+        Args:
+            jsonld: A JSON-LD dictionary.
+        Return:
+            The updated entity.
+        Raises:
+            ValueError: if the jsonld object is empty or None, if @id was not
+              provided, or if the entity was not found.
+        """
+        if not jsonld or "@id" not in jsonld:
+            raise ValueError("you must provide a non-empty JSON-LD dictionary")
+        entity_id = jsonld.pop("@id")
+        entity: Entity = self.get(entity_id)
+        if not entity:
+            raise ValueError(f"entity {entity_id} does not exist in the RO-Crate")
+        jsonld = {k: v for k, v in jsonld.items() if not k.startswith('@')}
+        entity._jsonld.update(jsonld)
+        return entity
+
+    def add_or_update_jsonld(self, jsonld):
+        """Add or update an entity from a JSON-LD dictionary.
+
+        An `@id` must be present in the JSON-LD dictionary.
+
+        Args:
+            jsonld: A JSON-LD dictionary.
+        Return:
+            The added or updated entity.
+        Raises:
+            ValueError: if the jsonld object is empty or None or if @id was not
+              provided.
+        """
+        if not jsonld or "@id" not in jsonld:
+            raise ValueError("you must provide a non-empty JSON-LD dictionary")
+        entity_id = jsonld.get("@id")
+        entity: Entity = self.get(entity_id)
+        if not entity:
+            return self.add_jsonld(jsonld)
+        return self.update_jsonld(jsonld)
+
     def __validate_suite(self, suite):
         if isinstance(suite, TestSuite):
             assert suite.crate is self
         else:
             suite = self.dereference(suite)
             if suite is None:
                 raise ValueError("suite not found")
```

### Comparing `rocrate-0.7.0/rocrate/templates/preview_template.html.j2` & `rocrate-0.8.0/rocrate/templates/preview_template.html.j2`

 * *Files identical despite different names*

### Comparing `rocrate-0.7.0/rocrate/utils.py` & `rocrate-0.8.0/rocrate/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate/vocabs.py` & `rocrate-0.8.0/rocrate/vocabs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/rocrate.egg-info/PKG-INFO` & `rocrate-0.8.0/rocrate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: rocrate
-Version: 0.7.0
+Version: 0.8.0
 Summary: RO-Crate metadata generator/parser
 Home-page: https://github.com/ResearchObject/ro-crate-py/
-Author: Paul De Geest, Bert Droesbeke, Ignacio Eguinoa, Alban Gaignard, Sebastiaan Huber, Simone Leo, Luca Pireddu, Laura Rodríguez-Navas, Raül Sirvent, Stian Soiland-Reyes
+Download-URL: https://github.com/researchobject/ro-crate-py/archive/0.8.0.tar.gz
+Author: Paul De Geest, Bert Droesbeke, Ignacio Eguinoa, Alban Gaignard, Sebastiaan Huber, Bruno Kinoshita, Simone Leo, Luca Pireddu, Laura Rodríguez-Navas, Raül Sirvent, Stian Soiland-Reyes
 Author-email: stain@apache.org
 License: Apache-2.0
-Download-URL: https://github.com/researchobject/ro-crate-py/archive/0.7.0.tar.gz
 Keywords: researchobject ro-crate ro metadata jsonld
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -71,15 +70,15 @@
 })
 diagram = crate.add_file("exp/diagram.svg", dest_path="images/figure.svg", properties={
     "name": "bar chart",
     "encodingFormat": "image/svg+xml"
 })
 ```
 
-We've started by adding the data entitites. Now we need contextual entities to represent Alice and Bob:
+We've started by adding the data entities. Now we need contextual entities to represent Alice and Bob:
 
 ```python
 from rocrate.model.person import Person
 
 alice_id = "https://orcid.org/0000-0000-0000-0000"
 bob_id = "https://orcid.org/0000-0000-0000-0001"
 alice = crate.add(Person(crate, alice_id, properties={
@@ -116,14 +115,17 @@
 
 You can also add whole directories. A directory in RO-Crate is represented by the `Dataset` entity:
 
 ```python
 logs = crate.add_dataset("exp/logs")
 ```
 
+Note that the above adds all files and directories contained in `"exp/logs"` recursively to the crate, but only the top-level `"exp/logs"` dataset itself is listed in the metadata file (there is no requirement to represent every file and folder in the JSON-LD). To also add files and directory recursively to the metadata, use `add_tree` (but note that it only works on local directory trees).
+
+
 #### Appending elements to property values
 
 What ro-crate-py entities actually store is their JSON representation:
 
 ```python
 paper.properties()
 ```
@@ -196,14 +198,68 @@
 
 Note that entities can have multiple types, e.g.:
 
 ```python
     "@type" = ["File", "SoftwareSourceCode"]
 ```
 
+#### Modifying the crate from JSON-LD dictionaries
+
+The `add_jsonld` method allows to add a contextual entity directly from a
+JSON-LD dictionary containing at least the `@id` and `@type` keys:
+
+```python
+crate.add_jsonld({
+    "@id": "https://orcid.org/0000-0000-0000-0000",
+    "@type": "Person",
+    "name": "Alice Doe"
+})
+```
+
+Existing entities can be updated from JSON-LD dictionaries via `update_jsonld`:
+
+```python
+crate.update_jsonld({
+    "@id": "https://orcid.org/0000-0000-0000-0000",
+    "name": "Alice K. Doe"
+})
+```
+
+There is also an `add_or_update_jsonld` method that adds the entity if it's
+not already in the crate and updates it if it already exists (note that, when
+updating, the `@type` key is ignored). This allows to "patch" an RO-Crate from
+a JSON-LD file. For instance, suppose you have the following `patch.json` file:
+
+```json
+{
+    "@graph": [
+        {
+            "@id": "./",
+            "author": {"@id": "https://orcid.org/0000-0000-0000-0001"}
+        },
+        {
+            "@id": "https://orcid.org/0000-0000-0000-0001",
+            "@type": "Person",
+            "name": "Bob Doe"
+        }
+    ]
+}
+```
+
+Then the following sets Bob as the author of the crate according to the above
+file:
+
+```python
+crate = ROCrate("temp-crate")
+with open("patch.json") as f:
+    json_data = json.load(f)
+for d in json_data.get("@graph", []):
+    crate.add_or_update_jsonld(d)
+```
+
 ### Consuming an RO-Crate
 
 An existing RO-Crate package can be loaded from a directory or zip file:
 
 ```python
 crate = ROCrate('exp_crate')  # or ROCrate('exp_crate.zip')
 for e in crate.get_entities():
@@ -303,15 +359,15 @@
 ### Example
 
 ```bash
 # From the ro-crate-py repository root
 cd test/test-data/ro-crate-galaxy-sortchangecase
 ```
 
-This directory is already an ro-crate. Delete the metadata file to get a plain directory tree:
+This directory is already an RO-Crate. Delete the metadata file to get a plain directory tree:
 
 ```bash
 rm ro-crate-metadata.json
 ```
 
 Now the directory tree contains several files and directories, including a Galaxy workflow and a Planemo test file, but it's not an RO-Crate since there is no metadata file. Initialize the crate:
 
@@ -330,40 +386,37 @@
 
 To register the workflow as a `ComputationalWorkflow`:
 
 ```bash
 rocrate add workflow -l galaxy sort-and-change-case.ga
 ```
 
-Now the workflow has a type of `["File", "SoftwareSourceCode", "ComputationalWorkflow"]` and points to a `ComputerLanguage` entity that represents the Galaxy workflow language. Also, the workflow is listed as the crate's `mainEntity` (see https://about.workflowhub.eu/Workflow-RO-Crate).
+Now the workflow has a type of `["File", "SoftwareSourceCode", "ComputationalWorkflow"]` and points to a `ComputerLanguage` entity that represents the Galaxy workflow language. Also, the workflow is listed as the crate's `mainEntity` (see the [Workflow RO-Crate profile](https://w3id.org/workflowhub/workflow-ro-crate/1.0)).
 
-To add [workflow testing metadata](https://github.com/crs4/life_monitor/wiki/Workflow-Testing-RO-Crate) to the crate:
+To add [workflow testing metadata](https://crs4.github.io/life_monitor/workflow_testing_ro_crate) to the crate:
 
 ```bash
 rocrate add test-suite -i test1
 rocrate add test-instance test1 http://example.com -r jobs -i test1_1
 rocrate add test-definition test1 test/test1/sort-and-change-case-test.yml -e planemo -v '>=0.70'
 ```
 
-
 ## License
 
- * Copyright 2019-2022 The University of Manchester, UK
- * Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
- * Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
- * Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
- * Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+ * Copyright 2019-2023 The University of Manchester, UK
+ * Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+ * Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+ * Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+ * Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 
 Licensed under the 
 Apache License, version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>, 
 see the file `LICENSE.txt` for details.
 
 ## Cite as
 
 [![DOI](https://zenodo.org/badge/216605684.svg)](https://zenodo.org/badge/latestdoi/216605684)
 
 The above DOI corresponds to the latest versioned release as [published to Zenodo](https://zenodo.org/record/3956493), where you will find all earlier releases. 
 To cite `ro-crate-py` independent of version, use <https://doi.org/10.5281/zenodo.3956493>, which will always redirect to the latest release.
 
 You may also be interested in the paper [Packaging research artefacts with RO-Crate](https://doi.org/10.3233/DS-210053).
-
-
```

### Comparing `rocrate-0.7.0/rocrate.egg-info/SOURCES.txt` & `rocrate-0.8.0/rocrate.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 rocrate/model/testinstance.py
 rocrate/model/testservice.py
 rocrate/model/testsuite.py
 rocrate/templates/preview_template.html.j2
 test/__init__.py
 test/conftest.py
 test/test_cli.py
+test/test_jsonld.py
 test/test_metadata.py
 test/test_model.py
 test/test_read.py
 test/test_readwrite.py
 test/test_test_metadata.py
 test/test_utils.py
 test/test_workflow_ro_crate.py
```

### Comparing `rocrate-0.7.0/setup.py` & `rocrate-0.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -57,14 +57,15 @@
     long_description=long_description,
     author=", ".join((
         'Paul De Geest',
         'Bert Droesbeke',
         'Ignacio Eguinoa',
         'Alban Gaignard',
         'Sebastiaan Huber',
+        'Bruno Kinoshita',
         'Simone Leo',
         'Luca Pireddu',
         'Laura Rodríguez-Navas',
         'Raül Sirvent',
         'Stian Soiland-Reyes'
     )),
     python_requires='>=3.7',
```

### Comparing `rocrate-0.7.0/test/conftest.py` & `rocrate-0.8.0/test/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/test/test_cli.py` & `rocrate-0.8.0/test/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -125,15 +125,15 @@
     assert result.exit_code == 0
     crate = ROCrate(crate_dir)
     for p in "LICENSE", "sort-and-change-case.ga":
         assert isinstance(crate.dereference(p), File)
     for p in exclude.split(",") + ["test/"]:
         assert not crate.dereference(p)
     for e in crate.data_entities:
-        assert not(e.id.startswith("test"))
+        assert not e.id.startswith("test")
 
 
 @pytest.mark.parametrize("cwd", [False, True])
 def test_cli_add_workflow(test_data_dir, helpers, monkeypatch, cwd):
     # init
     crate_dir = test_data_dir / "ro-crate-galaxy-sortchangecase"
     runner = CliRunner()
```

### Comparing `rocrate-0.7.0/test/test_metadata.py` & `rocrate-0.8.0/test/test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/test/test_model.py` & `rocrate-0.8.0/test/test_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 import json
+import os
 import tempfile
+import timeit
 import uuid
 from pathlib import Path
 
 import pytest
 from rocrate.rocrate import ROCrate
 from rocrate.model.data_entity import DataEntity
 from rocrate.model.file import File
@@ -90,14 +92,29 @@
     dataset = crate.add(Dataset(crate, test_data_dir / 'test_add_dir'))
     data_entity = crate.add(DataEntity(crate, '#mysterious'))
     assert set(crate.data_entities) == {file_, dataset, data_entity}
     part_ids = set(_["@id"] for _ in crate.root_dataset._jsonld["hasPart"])
     assert set(_.id for _ in (file_, dataset, data_entity)) <= part_ids
 
 
+@pytest.mark.skipif(os.name != "posix", reason="CI sometimes fails on macOS")
+def test_data_entities_perf():
+    """\
+    Test that adding a data entity happens in constant time.
+
+    See https://github.com/ResearchObject/ro-crate-py/pull/127 (this is a
+    regression test). The time required for 500 iterations should be ~0.01s if
+    entities are added in constant time, ~1s if they are added in linear time.
+    """
+    crate = ROCrate()
+    assert timeit.Timer(
+        "crate.add_file(uuid.uuid4().hex)", "import uuid", globals=locals()
+    ).timeit(500) < 0.1
+
+
 def test_remote_data_entities():
     crate = ROCrate()
     file_uri = "https://www.rfc-editor.org/rfc/rfc3986.txt"
     dataset_uri = "https://ftp.mozilla.org/pub/misc/errorpages/"
     file_ = crate.add(File(crate, file_uri))
     dataset = crate.add(Dataset(crate, dataset_uri))
     assert file_.id == file_uri
```

### Comparing `rocrate-0.7.0/test/test_read.py` & `rocrate-0.8.0/test/test_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -228,19 +228,19 @@
 def test_exclude(test_data_dir, tmpdir, helpers):
     def check(out=False):
         for p in "LICENSE", "sort-and-change-case.ga":
             assert isinstance(crate.dereference(p), File)
         for p in exclude + ["test/"]:
             assert not crate.dereference(p)
             if out:
-                assert not(crate.source / p).exists()
+                assert not (crate.source / p).exists()
         for e in crate.data_entities:
-            assert not(e.id.startswith("test"))
+            assert not e.id.startswith("test")
         if out:
-            assert not(crate.source / "test").exists()
+            assert not (crate.source / "test").exists()
     crate_dir = test_data_dir / "ro-crate-galaxy-sortchangecase"
     (crate_dir / helpers.METADATA_FILE_NAME).unlink()
     exclude = ["test", "README.md"]
     crate = ROCrate(crate_dir, init=True, exclude=exclude)
     check()
     out_path = tmpdir / 'ro_crate_out'
     crate.write(out_path)
@@ -316,32 +316,66 @@
     shutil.rmtree(crate_dir / name)
     crate = ROCrate(crate_dir)
 
     examples_dataset = crate.dereference(name)
     assert examples_dataset.id == f'{name}/'
 
     out_path = tmpdir / 'crate_read_out'
+    with pytest.raises(OSError):
+        crate.write(out_path)
+
+    # Two options to get a writable crate
+
+    # 1. Set the source to None (will create an empty dir)
+    examples_dataset.source = None
+    crate.write(out_path)
+    assert (out_path / name).is_dir()
+
+    shutil.rmtree(out_path)
+
+    # 2. Provide an existing source
+    source = tmpdir / "source"
+    source.mkdir()
+    examples_dataset.source = source
     crate.write(out_path)
-    assert not (out_path / 'README.txt').exists()
+    assert (out_path / name).is_dir()
 
 
+@pytest.mark.filterwarnings("ignore")
 def test_missing_file(test_data_dir, tmpdir):
     crate_dir = test_data_dir / 'read_crate'
     name = 'test_file_galaxy.txt'
     test_path = crate_dir / name
     test_path.unlink()
     crate = ROCrate(crate_dir)
 
     test_file = crate.dereference(name)
     assert test_file.id == name
 
     out_path = tmpdir / 'crate_read_out'
+    with pytest.raises(OSError):
+        crate.write(out_path)
+
+    # Two options to get a writable crate
+
+    # 1. Set the source to None (file will still be missing in the copy)
+    test_file.source = None
     crate.write(out_path)
     assert not (out_path / name).exists()
 
+    shutil.rmtree(out_path)
+
+    # 2. Provide an existing source
+    source = tmpdir / "source.txt"
+    text = "foo\nbar\n"
+    source.write_text(text)
+    test_file.source = source
+    crate.write(out_path)
+    assert (out_path / name).read_text() == text
+
 
 def test_generic_data_entity(tmpdir):
     rc_id = "#collection"
     metadata = {
         "@context": [
             "https://w3id.org/ro/crate/1.1/context",
             {"@vocab": "http://schema.org/"},
```

### Comparing `rocrate-0.7.0/test/test_readwrite.py` & `rocrate-0.8.0/test/test_readwrite.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/test/test_test_metadata.py` & `rocrate-0.8.0/test/test_test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -239,14 +239,16 @@
         kwargs["engine"] = engine
     if engine_version:
         kwargs["engine_version"] = engine_version
     d = crate.add_test_definition(suite, **kwargs)
     assert crate.dereference(PLANEMO) is d.engine
     if engine_version:
         assert d.engineVersion == engine_version
+    else:
+        assert "engineVersion" not in d
 
 
 def test_test_suites_prop(test_data_dir):
     top_dir = test_data_dir / "ro-crate-galaxy-sortchangecase"
     wf_path = top_dir / "sort-and-change-case.ga"
     crate = ROCrate()
     wf = crate.add(ComputationalWorkflow(crate, wf_path, wf_path.name))
```

### Comparing `rocrate-0.7.0/test/test_utils.py` & `rocrate-0.8.0/test/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rocrate-0.7.0/test/test_workflow_ro_crate.py` & `rocrate-0.8.0/test/test_workflow_ro_crate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import pytest
+
 from rocrate.rocrate import ROCrate, make_workflow_rocrate
-from rocrate.model.computerlanguage import CWL_DEFAULT_VERSION, GALAXY_DEFAULT_VERSION
 
 WF_CRATE = "https://w3id.org/workflowhub/workflow-ro-crate"
 
 
 def test_galaxy_wf_crate(test_data_dir, tmpdir, helpers):
     wf_id = 'test_galaxy_wf.ga'
     wf_path = test_data_dir / wf_id
@@ -29,15 +30,15 @@
     assert isinstance(wf_crate, ROCrate)
 
     wf = wf_crate.dereference(wf_id)
     assert wf._default_type == "ComputationalWorkflow"
     assert wf_crate.mainEntity is wf
     lang = wf_crate.dereference(f"{WF_CRATE}#galaxy")
     assert hasattr(lang, "name")
-    assert lang.version == GALAXY_DEFAULT_VERSION
+    assert "version" not in lang
     assert wf.get("programmingLanguage") is lang
     assert wf.get("subjectOf") is not None
     assert helpers.WORKFLOW_DESC_TYPES.issubset(wf["subjectOf"].type)
 
     out_path = tmpdir / 'ro_crate_out'
     out_path.mkdir()
     wf_crate.write(out_path)
@@ -64,15 +65,15 @@
     wf_crate = make_workflow_rocrate(wf_path, wf_type='CWL')
     assert isinstance(wf_crate, ROCrate)
 
     wf = wf_crate.dereference(wf_id)
     assert wf_crate.mainEntity is wf
     lang = wf_crate.dereference(f"{WF_CRATE}#cwl")
     assert hasattr(lang, "name")
-    assert lang.version == CWL_DEFAULT_VERSION
+    assert "version" not in lang
     assert wf.get("programmingLanguage") is lang
     assert "subjectOf" not in wf
 
     out_path = tmpdir / 'ro_crate_out'
     out_path.mkdir()
     wf_crate.write(out_path)
     json_entities = helpers.read_json_entities(out_path)
@@ -95,15 +96,15 @@
     )
     assert isinstance(wf_crate, ROCrate)
 
     wf = wf_crate.dereference(wf_id)
     assert wf_crate.mainEntity is wf
     lang = wf_crate.dereference(f"{WF_CRATE}#galaxy")
     assert hasattr(lang, "name")
-    assert lang.version == GALAXY_DEFAULT_VERSION
+    assert "version" not in lang
     assert wf.get("programmingLanguage") is lang
     assert wf.get("subjectOf") is not None
     assert helpers.WORKFLOW_DESC_TYPES.issubset(wf["subjectOf"].type)
     assert wf_crate.dereference(extra_file1.name) is not None
     assert wf_crate.dereference(extra_file2.name) is not None
 
     out_path = tmpdir / 'ro_crate_out'
@@ -120,7 +121,23 @@
         assert f1.read() == f2.read()
     assert file1.exists()
     with open(extra_file1) as f1, open(file1) as f2:
         assert f1.read() == f2.read()
     assert file2.exists()
     with open(extra_file2) as f1, open(file2) as f2:
         assert f1.read() == f2.read()
+
+
+@pytest.mark.parametrize("lang_version", [None, "1.2"])
+def test_cwl_lang_version(test_data_dir, lang_version):
+    wf_id = 'sample_cwl_wf.cwl'
+    wf_path = test_data_dir / wf_id
+    crate = ROCrate()
+    workflow = crate.add_workflow(wf_path, wf_id, lang_version=lang_version)
+    lang = workflow["programmingLanguage"]
+    lang_id = lang["identifier"]
+    if lang_version is None:
+        assert lang_id == "https://w3id.org/cwl/"
+        assert "version" not in lang
+    else:
+        assert lang_id == "https://w3id.org/cwl/v1.2/"
+        assert lang["version"] == "1.2"
```

### Comparing `rocrate-0.7.0/test/test_write.py` & `rocrate-0.8.0/test/test_write.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019-2022 The University of Manchester, UK
-# Copyright 2020-2022 Vlaams Instituut voor Biotechnologie (VIB), BE
-# Copyright 2020-2022 Barcelona Supercomputing Center (BSC), ES
-# Copyright 2020-2022 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
-# Copyright 2022 École Polytechnique Fédérale de Lausanne, CH
+# Copyright 2019-2023 The University of Manchester, UK
+# Copyright 2020-2023 Vlaams Instituut voor Biotechnologie (VIB), BE
+# Copyright 2020-2023 Barcelona Supercomputing Center (BSC), ES
+# Copyright 2020-2023 Center for Advanced Studies, Research and Development in Sardinia (CRS4), IT
+# Copyright 2022-2023 École Polytechnique Fédérale de Lausanne, CH
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -297,31 +297,44 @@
     try:
         crate.write(out_path)
     except PermissionError:
         pass
     # no error on Windows, or on Linux as root, so we don't use pytest.raises
 
 
-@pytest.mark.parametrize("fetch_remote,validate_url", [(False, False), (False, True), (True, False), (True, True)])
-def test_missing_source(test_data_dir, tmpdir, fetch_remote, validate_url):
+@pytest.mark.filterwarnings("ignore")
+@pytest.mark.parametrize("what", ["file", "dataset"])
+def test_missing_source(test_data_dir, tmpdir, what):
     path = test_data_dir / uuid.uuid4().hex
-    args = {"fetch_remote": fetch_remote, "validate_url": validate_url}
-
-    crate = ROCrate()
-    file_ = crate.add_file(path, **args)
-    assert file_ is crate.dereference(path.name)
-    out_path = tmpdir / 'ro_crate_out_1'
-    crate.write(out_path)
-    assert not (out_path / path.name).exists()
 
     crate = ROCrate()
-    file_ = crate.add_file(path, path.name, **args)
-    assert file_ is crate.dereference(path.name)
-    out_path = tmpdir / 'ro_crate_out_2'
-    assert not (out_path / path.name).exists()
+    entity = getattr(crate, f"add_{what}")(path)
+    assert entity is crate.dereference(path.name)
+    crate_dir = tmpdir / 'ro_crate_out_1'
+    with pytest.raises(OSError):
+        crate.write(crate_dir)
+
+    crate = ROCrate()
+    entity = getattr(crate, f"add_{what}")(path, path.name)
+    assert entity is crate.dereference(path.name)
+    crate_dir = tmpdir / 'ro_crate_out_2'
+    with pytest.raises(OSError):
+        crate.write(crate_dir)
+
+    crate = ROCrate()
+    entity = getattr(crate, f"add_{what}")(None, path.name)
+    assert entity is crate.dereference(path.name)
+    crate_dir = tmpdir / 'ro_crate_out_3'
+    crate.write(crate_dir)
+    out_path = crate_dir / path.name
+    if what == "file":
+        assert not out_path.exists()
+    else:
+        assert out_path.is_dir()
+        assert not any(out_path.iterdir())
 
 
 @pytest.mark.parametrize("fetch_remote,validate_url", [(False, False), (False, True), (True, False), (True, True)])
 def test_stringio_no_dest(test_data_dir, fetch_remote, validate_url):
     crate = ROCrate()
     with pytest.raises(ValueError):
         crate.add_file(io.StringIO("foo"))
@@ -332,20 +345,23 @@
     crate = ROCrate()
     with pytest.raises(ValueError):
         crate.add_file()
 
 
 def test_dataset(test_data_dir, tmpdir):
     crate = ROCrate()
-    path = test_data_dir / "a" / "b"
-    d1 = crate.add_dataset(path)
+    path_a_b = test_data_dir / "a" / "b"
+    path_c = test_data_dir / "c"
+    for p in path_a_b, path_c:
+        p.mkdir(parents=True)
+    d1 = crate.add_dataset(path_a_b)
     assert crate.dereference("b") is d1
-    d2 = crate.add_dataset(path, "a/b")
+    d2 = crate.add_dataset(path_a_b, "a/b")
     assert crate.dereference("a/b") is d2
-    d_from_str = crate.add_dataset(str(test_data_dir / "c"))
+    d_from_str = crate.add_dataset(str(path_c))
     assert crate.dereference("c") is d_from_str
 
     out_path = tmpdir / 'ro_crate_out'
     out_path.mkdir()
     crate.write(out_path)
 
     assert (out_path / "b").is_dir()
@@ -373,7 +389,46 @@
     zip_path = crate_dir / zip_name  # within the crate dir
     crate.write_zip(zip_path)
     out_path = tmpdir / 'ro_crate_out'
     with zipfile.ZipFile(zip_path, "r") as zf:
         zf.extractall(out_path)
 
     assert not (out_path / zip_name).exists()
+
+
+def test_add_tree(test_data_dir, tmpdir):
+    source = test_data_dir / "read_extra"
+    (source / "ro-crate-metadata.json").unlink()
+    crate = ROCrate()
+    crate.add_tree(source)
+    out_path = tmpdir / 'ro_crate_out'
+    crate.write(out_path)
+
+    assert (out_path / "read_extra").is_dir()
+    assert (out_path / "read_extra" / "listed").is_dir()
+    assert (out_path / "read_extra" / "listed" / "listed.txt").is_file()
+    assert (out_path / "read_extra" / "listed" / "not_listed.txt").is_file()
+    assert (out_path / "read_extra" / "not_listed").is_dir()
+    assert (out_path / "read_extra" / "not_listed" / "not_listed.txt").is_file()
+    assert (out_path / "read_extra" / "listed.txt").is_file()
+    assert (out_path / "read_extra" / "not_listed.txt").is_file()
+
+    crate = ROCrate(out_path)
+    top = crate.get("read_extra")
+    assert top.type == "Dataset"
+    listed = crate.get("read_extra/listed")
+    assert listed.type == "Dataset"
+    not_listed = crate.get("read_extra/not_listed")
+    assert not_listed.type == "Dataset"
+    listed_txt = crate.get("read_extra/listed.txt")
+    assert listed_txt.type == "File"
+    not_listed_txt = crate.get("read_extra/not_listed.txt")
+    assert not_listed_txt.type == "File"
+    assert set(top["hasPart"]) == {listed, not_listed, listed_txt, not_listed_txt}
+    listed_listed_txt = crate.get("read_extra/listed/listed.txt")
+    listed_not_listed_txt = crate.get("read_extra/listed/not_listed.txt")
+    assert set(listed["hasPart"]) == {listed_listed_txt, listed_not_listed_txt}
+    not_listed_not_listed_txt = crate.get("read_extra/not_listed/not_listed.txt")
+    assert set(not_listed["hasPart"]) == {not_listed_not_listed_txt}
+
+    with pytest.raises(ValueError):
+        crate.add_tree(None, dest_path="foobar")
```

