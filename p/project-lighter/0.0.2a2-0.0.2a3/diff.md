# Comparing `tmp/project_lighter-0.0.2a2.tar.gz` & `tmp/project_lighter-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_lighter-0.0.2a2.tar", max compression
+gzip compressed data, was "project_lighter-0.0.2a3.tar", max compression
```

## Comparing `project_lighter-0.0.2a2.tar` & `project_lighter-0.0.2a3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1080 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/LICENSE
--rw-r--r--   0        0        0      485 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/README.md
--rw-r--r--   0        0        0       67 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/__init__.py
--rw-r--r--   0        0        0      125 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/__init__.py
--rw-r--r--   0        0        0    14196 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/logger.py
--rw-r--r--   0        0        0     6508 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/writer/__init__.py
--rw-r--r--   0        0        0     7593 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/writer/base.py
--rw-r--r--   0        0        0     2662 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/writer/file.py
--rw-r--r--   0        0        0     2427 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/writer/table.py
--rw-r--r--   0        0        0    19790 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/system.py
--rw-r--r--   0        0        0       36 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/__init__.py
--rw-r--r--   0        0        0      627 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/cli.py
--rw-r--r--   0        0        0     2566 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/collate.py
--rw-r--r--   0        0        0     1547 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/dynamic_imports.py
--rw-r--r--   0        0        0     3431 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/freezer.py
--rw-r--r--   0        0        0     2278 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/misc.py
--rw-r--r--   0        0        0     5881 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/model.py
--rw-r--r--   0        0        0     2483 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/runner.py
--rw-r--r--   0        0        0       24 2023-05-24 14:43:03.884755 project_lighter-0.0.2a2/lighter/version.py
--rw-r--r--   0        0        0     4399 2023-05-24 14:43:03.832755 project_lighter-0.0.2a2/pyproject.toml
--rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 project_lighter-0.0.2a2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/LICENSE
+-rw-r--r--   0        0        0     2164 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/README.md
+-rw-r--r--   0        0        0       67 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/__init__.py
+-rw-r--r--   0        0        0      125 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/callbacks/__init__.py
+-rw-r--r--   0        0        0    14196 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/callbacks/logger.py
+-rw-r--r--   0        0        0     6508 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/callbacks/writer/__init__.py
+-rw-r--r--   0        0        0     7593 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/callbacks/writer/base.py
+-rw-r--r--   0        0        0     2662 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/callbacks/writer/file.py
+-rw-r--r--   0        0        0     2427 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/callbacks/writer/table.py
+-rw-r--r--   0        0        0    19790 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/system.py
+-rw-r--r--   0        0        0       36 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/utils/__init__.py
+-rw-r--r--   0        0        0      627 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/utils/cli.py
+-rw-r--r--   0        0        0     2566 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/utils/collate.py
+-rw-r--r--   0        0        0     1547 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/utils/dynamic_imports.py
+-rw-r--r--   0        0        0     3431 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/utils/freezer.py
+-rw-r--r--   0        0        0     2278 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/utils/misc.py
+-rw-r--r--   0        0        0     5881 2023-06-05 20:40:38.040021 project_lighter-0.0.2a3/lighter/utils/model.py
+-rw-r--r--   0        0        0     2483 2023-06-05 20:40:38.044021 project_lighter-0.0.2a3/lighter/utils/runner.py
+-rw-r--r--   0        0        0       24 2023-06-05 20:41:00.388203 project_lighter-0.0.2a3/lighter/version.py
+-rw-r--r--   0        0        0     4399 2023-06-05 20:41:00.336202 project_lighter-0.0.2a3/pyproject.toml
+-rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 project_lighter-0.0.2a3/PKG-INFO
```

### Comparing `project_lighter-0.0.2a2/LICENSE` & `project_lighter-0.0.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/callbacks/logger.py` & `project_lighter-0.0.2a3/lighter/callbacks/logger.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/callbacks/utils.py` & `project_lighter-0.0.2a3/lighter/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/callbacks/writer/base.py` & `project_lighter-0.0.2a3/lighter/callbacks/writer/base.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/callbacks/writer/file.py` & `project_lighter-0.0.2a3/lighter/callbacks/writer/file.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/callbacks/writer/table.py` & `project_lighter-0.0.2a3/lighter/callbacks/writer/table.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/system.py` & `project_lighter-0.0.2a3/lighter/system.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/utils/cli.py` & `project_lighter-0.0.2a3/lighter/utils/cli.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/utils/collate.py` & `project_lighter-0.0.2a3/lighter/utils/collate.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/utils/dynamic_imports.py` & `project_lighter-0.0.2a3/lighter/utils/dynamic_imports.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/utils/freezer.py` & `project_lighter-0.0.2a3/lighter/utils/freezer.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/utils/misc.py` & `project_lighter-0.0.2a3/lighter/utils/misc.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/utils/model.py` & `project_lighter-0.0.2a3/lighter/utils/model.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/lighter/utils/runner.py` & `project_lighter-0.0.2a3/lighter/utils/runner.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a2/pyproject.toml` & `project_lighter-0.0.2a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 lighter = "lighter.utils.cli:interface"
 
 [tool.poetry]
 name = "project-lighter"
-version = "0.0.2a2"
+version = "0.0.2a3"
 description = "YAML-based automated rapid prototyping framework for deep learning experiments"
 readme = "README.md"
 authors = ["Ibrahim Hadzic <ibrahimhadzic45@gmail.com>" ,
             "Suraj Pai <b.pai@maastrichtuniversity.nl>", 
             "Keno Bressem <kbressem@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/lighter/lighter"
```

