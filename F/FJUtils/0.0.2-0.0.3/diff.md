# Comparing `tmp/FJUtils-0.0.2.tar.gz` & `tmp/FJUtils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FJUtils-0.0.2.tar", last modified: Wed May 31 09:17:35 2023, max compression
+gzip compressed data, was "FJUtils-0.0.3.tar", last modified: Mon Jun  5 08:36:48 2023, max compression
```

## Comparing `FJUtils-0.0.2.tar` & `FJUtils-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-31 09:17:35.322928 FJUtils-0.0.2/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-31 09:17:35.322928 FJUtils-0.0.2/FJUtils.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2684 2023-05-31 09:17:35.000000 FJUtils-0.0.2/FJUtils.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      291 2023-05-31 09:17:35.000000 FJUtils-0.0.2/FJUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-05-31 09:17:35.000000 FJUtils-0.0.2/FJUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      122 2023-05-31 09:17:35.000000 FJUtils-0.0.2/FJUtils.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-05-31 09:17:35.000000 FJUtils-0.0.2/FJUtils.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-05-31 06:53:13.000000 FJUtils-0.0.2/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2684 2023-05-31 09:17:35.322928 FJUtils-0.0.2/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1925 2023-05-31 08:45:55.000000 FJUtils-0.0.2/README.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-31 09:17:35.322928 FJUtils-0.0.2/fjutils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      708 2023-05-31 08:45:55.000000 FJUtils-0.0.2/fjutils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8231 2023-05-31 08:45:55.000000 FJUtils-0.0.2/fjutils/checkpointing.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9903 2023-05-31 08:28:39.000000 FJUtils-0.0.2/fjutils/easylm.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-05-31 08:45:55.000000 FJUtils-0.0.2/fjutils/load.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2257 2023-05-31 08:45:55.000000 FJUtils-0.0.2/fjutils/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-05-31 08:31:14.000000 FJUtils-0.0.2/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-05-31 09:17:35.322928 FJUtils-0.0.2/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1215 2023-05-31 09:17:00.000000 FJUtils-0.0.2/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-05 08:36:48.474817 FJUtils-0.0.3/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-05 08:36:48.470817 FJUtils-0.0.3/FJUtils.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-06-05 08:36:48.000000 FJUtils-0.0.3/FJUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      313 2023-06-05 08:36:48.000000 FJUtils-0.0.3/FJUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-06-05 08:36:48.000000 FJUtils-0.0.3/FJUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      121 2023-06-05 08:36:48.000000 FJUtils-0.0.3/FJUtils.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-06-05 08:36:48.000000 FJUtils-0.0.3/FJUtils.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-05-31 06:53:13.000000 FJUtils-0.0.3/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-06-05 08:36:48.470817 FJUtils-0.0.3/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-05 08:34:56.000000 FJUtils-0.0.3/README.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-05 08:36:48.470817 FJUtils-0.0.3/fjutils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      708 2023-05-31 08:45:55.000000 FJUtils-0.0.3/fjutils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8245 2023-05-31 15:57:33.000000 FJUtils-0.0.3/fjutils/checkpointing.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9903 2023-05-31 08:28:39.000000 FJUtils-0.0.3/fjutils/easylm.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-05-31 08:45:55.000000 FJUtils-0.0.3/fjutils/load.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6882 2023-06-05 08:30:43.000000 FJUtils-0.0.3/fjutils/optimizers.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3757 2023-06-05 08:19:58.000000 FJUtils-0.0.3/fjutils/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-05-31 08:31:14.000000 FJUtils-0.0.3/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-05 08:36:48.474817 FJUtils-0.0.3/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1214 2023-06-05 08:36:45.000000 FJUtils-0.0.3/setup.py
```

### Comparing `FJUtils-0.0.2/LICENSE` & `FJUtils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.2/fjutils/__init__.py` & `FJUtils-0.0.3/fjutils/__init__.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.2/fjutils/checkpointing.py` & `FJUtils-0.0.3/fjutils/checkpointing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+
+import optax
 from ml_collections import ConfigDict
 import mlxu
 import jax
 import flax
 from flax.serialization import (
     from_bytes, to_bytes, to_state_dict, from_state_dict
 )
```

### Comparing `FJUtils-0.0.2/fjutils/easylm.py` & `FJUtils-0.0.3/fjutils/easylm.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.2/fjutils/load.py` & `FJUtils-0.0.3/fjutils/load.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.2/pyproject.toml` & `FJUtils-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.2/setup.py` & `FJUtils-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FJUtils",
-    version='0.0.2',
+    version='0.0.3',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
-        'jax~=0.4.10',
+        'jax~=0.4.7',
         'transformers~=4.29.2',
         'typing~=3.7.4.3',
         'numpy~=1.24.3',
         'flax~=0.6.4',
         'msgpack~=1.0.5',
         'setuptools~=59.6.0',
         'mlxu~=0.1.11'
```

