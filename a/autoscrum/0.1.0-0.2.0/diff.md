# Comparing `tmp/autoscrum-0.1.0.tar.gz` & `tmp/autoscrum-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoscrum-0.1.0.tar", last modified: Mon May 29 21:29:54 2023, max compression
+gzip compressed data, was "autoscrum-0.2.0.tar", last modified: Mon Jun  5 17:37:26 2023, max compression
```

## Comparing `autoscrum-0.1.0.tar` & `autoscrum-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,24 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-29 21:29:54.510896 autoscrum-0.1.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)      429 2023-05-29 21:29:54.506896 autoscrum-0.1.0/PKG-INFO
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-29 21:29:54.506896 autoscrum-0.1.0/autoscrum/
--rw-rw-r--   0 martin    (1000) martin    (1000)       78 2023-05-29 21:28:26.000000 autoscrum-0.1.0/autoscrum/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-29 21:29:54.506896 autoscrum-0.1.0/autoscrum.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)      429 2023-05-29 21:29:54.000000 autoscrum-0.1.0/autoscrum.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      236 2023-05-29 21:29:54.000000 autoscrum-0.1.0/autoscrum.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-29 21:29:54.000000 autoscrum-0.1.0/autoscrum.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-05-29 21:29:54.000000 autoscrum-0.1.0/autoscrum.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       63 2023-05-29 21:29:54.000000 autoscrum-0.1.0/autoscrum.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-05-29 21:29:54.000000 autoscrum-0.1.0/autoscrum.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     1114 2023-05-29 21:29:04.000000 autoscrum-0.1.0/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-29 21:29:54.510896 autoscrum-0.1.0/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-05 17:37:26.637970 autoscrum-0.2.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    35149 2023-06-05 14:55:21.000000 autoscrum-0.2.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)    43986 2023-06-05 17:37:26.637970 autoscrum-0.2.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2969 2023-06-05 15:41:55.000000 autoscrum-0.2.0/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-05 17:37:26.637970 autoscrum-0.2.0/autoscrum/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      113 2023-06-05 15:22:08.000000 autoscrum-0.2.0/autoscrum/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5205 2023-06-05 15:16:22.000000 autoscrum-0.2.0/autoscrum/__main__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5577 2023-06-05 15:15:15.000000 autoscrum-0.2.0/autoscrum/autoscrum.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1777 2023-06-01 20:12:54.000000 autoscrum-0.2.0/autoscrum/controller.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-05 17:37:26.637970 autoscrum-0.2.0/autoscrum/data/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2274 2023-06-05 14:59:10.000000 autoscrum-0.2.0/autoscrum/data/featurizer.hbs
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1032 2023-06-05 15:00:21.000000 autoscrum-0.2.0/autoscrum/data/taskalizer.hbs
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-05 17:37:26.637970 autoscrum-0.2.0/autoscrum.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    43986 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      416 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       80 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1153 2023-06-05 17:37:10.000000 autoscrum-0.2.0/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-06-05 17:37:26.637970 autoscrum-0.2.0/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)      417 2023-06-05 14:52:02.000000 autoscrum-0.2.0/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-05 17:37:26.637970 autoscrum-0.2.0/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      195 2023-06-05 15:24:14.000000 autoscrum-0.2.0/tests/test_autoscrum.py
```

### Comparing `autoscrum-0.1.0/pyproject.toml` & `autoscrum-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autoscrum"
-version = "0.1.0"
+version = "0.2.0"
 description = "AutoScrum"
 readme = "README.md"
 authors = [{ name = "Martin Schröder", email = "info@swedishembedded.com" }]
 license = { file = "LICENSE" }
 classifiers = [
-	"License :: OSI Approved :: Apache Software License",
+	"License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
 ]
 keywords = []
 dependencies = [
-	"pypdf",
-	"xformers",
+	"guidance",
+	"pathlib",
+	"datetime",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
 	"black",
+	"build",
 	"bumpversion",
 	"isort",
 	"pip-tools",
 	"pytest"
 ]
 
 [project.urls]
 Homepage = "https://github.com/autoscrum/autoscrum"
 
 [project.scripts]
 autoscrum = "autoscrum.__main__:main"
 
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

