# Comparing `tmp/jaxhelper-0.0.1.tar.gz` & `tmp/jaxhelper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxhelper-0.0.1.tar", last modified: Sun Jun  4 20:54:18 2023, max compression
+gzip compressed data, was "jaxhelper-0.0.2.tar", last modified: Mon Jun  5 13:30:50 2023, max compression
```

## Comparing `jaxhelper-0.0.1.tar` & `jaxhelper-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-04 20:54:18.974466 jaxhelper-0.0.1/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1492 2023-06-04 20:54:18.974466 jaxhelper-0.0.1/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      715 2023-06-04 20:53:19.000000 jaxhelper-0.0.1/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-04 20:54:18.974466 jaxhelper-0.0.1/jaxhelper/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     4913 2023-06-04 20:53:13.000000 jaxhelper-0.0.1/jaxhelper/__init__.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-04 20:54:18.974466 jaxhelper-0.0.1/jaxhelper.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1492 2023-06-04 20:54:18.000000 jaxhelper-0.0.1/jaxhelper.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      172 2023-06-04 20:54:18.000000 jaxhelper-0.0.1/jaxhelper.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-04 20:54:18.000000 jaxhelper-0.0.1/jaxhelper.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       10 2023-06-04 20:54:18.000000 jaxhelper-0.0.1/jaxhelper.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-04 20:54:18.974466 jaxhelper-0.0.1/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1090 2023-06-04 20:54:05.000000 jaxhelper-0.0.1/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:30:50.210023 jaxhelper-0.0.2/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:30:50.210023 jaxhelper-0.0.2/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      701 2023-06-04 20:54:48.000000 jaxhelper-0.0.2/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:30:50.210023 jaxhelper-0.0.2/jaxhelper/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     5049 2023-06-05 13:30:40.000000 jaxhelper-0.0.2/jaxhelper/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:30:50.210023 jaxhelper-0.0.2/jaxhelper.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:30:50.000000 jaxhelper-0.0.2/jaxhelper.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      172 2023-06-05 13:30:50.000000 jaxhelper-0.0.2/jaxhelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-05 13:30:50.000000 jaxhelper-0.0.2/jaxhelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       10 2023-06-05 13:30:50.000000 jaxhelper-0.0.2/jaxhelper.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-05 13:30:50.210023 jaxhelper-0.0.2/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1090 2023-06-05 13:29:59.000000 jaxhelper-0.0.2/setup.py
```

### Comparing `jaxhelper-0.0.1/PKG-INFO` & `jaxhelper-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxhelper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Basic tools and helpers for Jax
 Home-page: https://github.com/clashluke/jaxhelper
 Author: Lucas Nestler
 Author-email: github.jaxhelper@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # JaxHelper
 
-/home/lucas/PycharmProjects/jaxtools/setup.py
+Basic tools and helpers for Jax
 
 ## Getting Started
 
 ### Installation
 
 ```BASH
 python3 -m pip install jaxhelper
```

### Comparing `jaxhelper-0.0.1/README.md` & `jaxhelper-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # JaxHelper
 
-/home/lucas/PycharmProjects/jaxtools/setup.py
+Basic tools and helpers for Jax
 
 ## Getting Started
 
 ### Installation
 
 ```BASH
 python3 -m pip install jaxhelper
```

### Comparing `jaxhelper-0.0.1/jaxhelper/__init__.py` & `jaxhelper-0.0.2/jaxhelper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import typing
 from typing import Callable, Tuple
 
 import jax
 from jax import lax, numpy as jnp
 
 _GLOBAL_FLAGS = {}
 
@@ -77,15 +78,17 @@
 
 def tree_dtype(tree):
     x, _structure = jax.tree_util.tree_flatten(tree)
     return x[0].dtype
 
 
 @map_fn
-def index(x, index):
+def index(x, index: typing.Optional[int] = None):
+    if index is None:
+        return map_fn(lambda k: k[x])  # x is index, we simply curried
     return x[index]
 
 
 @map_fn
 def nan_default(x, default):
     return jnp.where(jnp.isfinite(x), x, default)  # True, False | x in (NaN, Inf, -Inf)
```

### Comparing `jaxhelper-0.0.1/jaxhelper.egg-info/PKG-INFO` & `jaxhelper-0.0.2/jaxhelper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxhelper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Basic tools and helpers for Jax
 Home-page: https://github.com/clashluke/jaxhelper
 Author: Lucas Nestler
 Author-email: github.jaxhelper@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # JaxHelper
 
-/home/lucas/PycharmProjects/jaxtools/setup.py
+Basic tools and helpers for Jax
 
 ## Getting Started
 
 ### Installation
 
 ```BASH
 python3 -m pip install jaxhelper
```

### Comparing `jaxhelper-0.0.1/setup.py` & `jaxhelper-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Lucas Nestler",
     author_email="github.jaxhelper@nestler.sh",
     name='jaxhelper',
     license='BSD',
     description='Basic tools and helpers for Jax',
-    version='0.0.1',
+    version='0.0.2',
     long_description=README,
     url='https://github.com/clashluke/jaxhelper',
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     long_description_content_type="text/markdown",
     install_requires=[],
     classifiers=[
```

