# Comparing `tmp/weasel-0.0.0.tar.gz` & `tmp/weasel-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weasel-0.0.0.tar", last modified: Tue Sep 27 10:38:14 2022, max compression
+gzip compressed data, was "weasel-0.1.0rc0.tar", last modified: Mon Jun  5 11:26:31 2023, max compression
```

## Comparing `weasel-0.0.0.tar` & `weasel-0.1.0rc0.tar`

### file list

```diff
@@ -1,14 +1,57 @@
-drwxrwxrwx   0        0        0        0 2022-09-27 10:38:14.697395 weasel-0.0.0/
--rw-rw-rw-   0        0        0     1149 2022-03-03 16:32:03.000000 weasel-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     1159 2022-09-27 10:38:14.697395 weasel-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       52 2022-09-27 10:22:14.000000 weasel-0.0.0/README.md
--rw-rw-rw-   0        0        0       84 2022-09-27 10:26:28.000000 weasel-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      987 2022-09-27 10:38:14.700399 weasel-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      154 2022-09-27 10:36:07.000000 weasel-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-27 10:38:14.690954 weasel-0.0.0/weasel/
--rw-rw-rw-   0        0        0        0 2022-09-27 10:24:03.000000 weasel-0.0.0/weasel/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-27 10:38:14.697395 weasel-0.0.0/weasel.egg-info/
--rw-rw-rw-   0        0        0     1159 2022-09-27 10:38:14.000000 weasel-0.0.0/weasel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2022-09-27 10:38:14.000000 weasel-0.0.0/weasel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-27 10:38:14.000000 weasel-0.0.0/weasel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-09-27 10:38:14.000000 weasel-0.0.0/weasel.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 11:26:31.404996 weasel-0.1.0rc0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)     3691 2023-06-05 11:26:31.404996 weasel-0.1.0rc0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2657 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      403 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1379 2023-06-05 11:26:31.404996 weasel-0.1.0rc0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 11:26:31.400995 weasel-0.1.0rc0/weasel/
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/about.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 11:26:31.400995 weasel-0.1.0rc0/weasel/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)      272 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8231 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/cli/assets.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4757 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/cli/clone.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5160 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/cli/document.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8460 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/cli/dvc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/cli/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2934 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/cli/pull.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2764 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/cli/push.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7967 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/cli/remote_storage.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14748 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/cli/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4627 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/schemas.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 11:26:31.404996 weasel-0.1.0rc0/weasel/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 11:26:31.404996 weasel-0.1.0rc0/weasel/tests/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/tests/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6698 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/tests/cli/test_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5928 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/tests/cli/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1908 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/tests/cli/test_document.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2058 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/tests/cli/test_remote.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/tests/test_schemas.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5222 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/tests/test_validation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      600 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 11:26:31.404996 weasel-0.1.0rc0/weasel/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5778 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      595 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2796 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/filesystem.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2232 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/frozen.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6419 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/git.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1380 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/hashing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/logging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      587 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/modules.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1294 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/remote.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3221 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/validation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2098 2023-06-05 11:26:20.000000 weasel-0.1.0rc0/weasel/util/versions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 11:26:31.400995 weasel-0.1.0rc0/weasel.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3691 2023-06-05 11:26:31.000000 weasel-0.1.0rc0/weasel.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1117 2023-06-05 11:26:31.000000 weasel-0.1.0rc0/weasel.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 11:26:31.000000 weasel-0.1.0rc0/weasel.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       44 2023-06-05 11:26:31.000000 weasel-0.1.0rc0/weasel.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      202 2023-06-05 11:26:31.000000 weasel-0.1.0rc0/weasel.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-06-05 11:26:31.000000 weasel-0.1.0rc0/weasel.egg-info/top_level.txt
```

### Comparing `weasel-0.0.0/LICENSE` & `weasel-0.1.0rc0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (C) 2016-2022 ExplosionAI GmbH, 2016 spaCy GmbH, 2015 Matthew Honnibal
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (C) 2022 ExplosionAI GmbH
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

