# Comparing `tmp/napari-annotate-0.0.1.tar.gz` & `tmp/napari-annotate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-annotate-0.0.1.tar", last modified: Thu Nov  3 14:24:55 2022, max compression
+gzip compressed data, was "napari-annotate-0.0.2.tar", last modified: Mon Jun  5 09:17:10 2023, max compression
```

## Comparing `napari-annotate-0.0.1.tar` & `napari-annotate-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 14:24:55.765589 napari-annotate-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 14:24:55.761589 napari-annotate-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 14:24:55.765589 napari-annotate-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 14:24:55.765589 napari-annotate-0.0.1/.napari/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-11-03 14:24:55.765589 napari-annotate-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/manifest.in
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-11-03 14:24:55.765589 napari-annotate-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 14:24:55.761589 napari-annotate-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 14:24:55.765589 napari-annotate-0.0.1/src/napari_annotate/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/src/napari_annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6886 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/src/napari_annotate/_annotate.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/src/napari_annotate/_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-03 14:24:55.000000 napari-annotate-0.0.1/src/napari_annotate/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-11-03 14:24:37.000000 napari-annotate-0.0.1/src/napari_annotate/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 14:24:55.765589 napari-annotate-0.0.1/src/napari_annotate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-11-03 14:24:55.000000 napari-annotate-0.0.1/src/napari_annotate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-11-03 14:24:55.000000 napari-annotate-0.0.1/src/napari_annotate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 14:24:55.000000 napari-annotate-0.0.1/src/napari_annotate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-03 14:24:55.000000 napari-annotate-0.0.1/src/napari_annotate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-03 14:24:55.000000 napari-annotate-0.0.1/src/napari_annotate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-03 14:24:55.000000 napari-annotate-0.0.1/src/napari_annotate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:17:10.823597 napari-annotate-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:17:10.819597 napari-annotate-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:17:10.823597 napari-annotate-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:17:10.823597 napari-annotate-0.0.2/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-05 09:17:10.823597 napari-annotate-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/manifest.in
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-05 09:17:10.823597 napari-annotate-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:17:10.819597 napari-annotate-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:17:10.823597 napari-annotate-0.0.2/src/napari_annotate/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/src/napari_annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24951 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/src/napari_annotate/_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 09:17:10.000000 napari-annotate-0.0.2/src/napari_annotate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-05 09:16:57.000000 napari-annotate-0.0.2/src/napari_annotate/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:17:10.823597 napari-annotate-0.0.2/src/napari_annotate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-05 09:17:10.000000 napari-annotate-0.0.2/src/napari_annotate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-05 09:17:10.000000 napari-annotate-0.0.2/src/napari_annotate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:17:10.000000 napari-annotate-0.0.2/src/napari_annotate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-05 09:17:10.000000 napari-annotate-0.0.2/src/napari_annotate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 09:17:10.000000 napari-annotate-0.0.2/src/napari_annotate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 09:17:10.000000 napari-annotate-0.0.2/src/napari_annotate.egg-info/top_level.txt
```

### Comparing `napari-annotate-0.0.1/.github/workflows/deploy.yml` & `napari-annotate-0.0.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-annotate-0.0.1/.gitignore` & `napari-annotate-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-annotate-0.0.1/LICENSE.txt` & `napari-annotate-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `napari-annotate-0.0.1/setup.cfg` & `napari-annotate-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-annotate
-version = 0.0.1
+version = 0.0.2
 author = Jules Scholler
 author_email = jules.scholler@wysscenter.ch
 url = https://github.com/WyssCenter
 license = MPL-2.0
 description = Annotate large 2D slides
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `napari-annotate-0.0.1/src/napari_annotate.egg-info/SOURCES.txt` & `napari-annotate-0.0.2/src/napari_annotate.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/deploy.yml
 .napari/DESCRIPTION.md
 src/napari_annotate/__init__.py
 src/napari_annotate/_annotate.py
-src/napari_annotate/_reader.py
 src/napari_annotate/_version.py
 src/napari_annotate/napari.yaml
 src/napari_annotate.egg-info/PKG-INFO
 src/napari_annotate.egg-info/SOURCES.txt
 src/napari_annotate.egg-info/dependency_links.txt
 src/napari_annotate.egg-info/entry_points.txt
 src/napari_annotate.egg-info/requires.txt
```

