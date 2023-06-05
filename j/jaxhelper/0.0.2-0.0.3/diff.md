# Comparing `tmp/jaxhelper-0.0.2.tar.gz` & `tmp/jaxhelper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxhelper-0.0.2.tar", last modified: Mon Jun  5 13:30:50 2023, max compression
+gzip compressed data, was "jaxhelper-0.0.3.tar", last modified: Mon Jun  5 13:32:38 2023, max compression
```

## Comparing `jaxhelper-0.0.2.tar` & `jaxhelper-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:30:50.210023 jaxhelper-0.0.2/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:30:50.210023 jaxhelper-0.0.2/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      701 2023-06-04 20:54:48.000000 jaxhelper-0.0.2/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:30:50.210023 jaxhelper-0.0.2/jaxhelper/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     5049 2023-06-05 13:30:40.000000 jaxhelper-0.0.2/jaxhelper/__init__.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:30:50.210023 jaxhelper-0.0.2/jaxhelper.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:30:50.000000 jaxhelper-0.0.2/jaxhelper.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      172 2023-06-05 13:30:50.000000 jaxhelper-0.0.2/jaxhelper.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-05 13:30:50.000000 jaxhelper-0.0.2/jaxhelper.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       10 2023-06-05 13:30:50.000000 jaxhelper-0.0.2/jaxhelper.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-05 13:30:50.210023 jaxhelper-0.0.2/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1090 2023-06-05 13:29:59.000000 jaxhelper-0.0.2/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:32:38.574878 jaxhelper-0.0.3/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:32:38.574878 jaxhelper-0.0.3/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      701 2023-06-04 20:54:48.000000 jaxhelper-0.0.3/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:32:38.574878 jaxhelper-0.0.3/jaxhelper/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     5060 2023-06-05 13:32:21.000000 jaxhelper-0.0.3/jaxhelper/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-05 13:32:38.574878 jaxhelper-0.0.3/jaxhelper.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1478 2023-06-05 13:32:38.000000 jaxhelper-0.0.3/jaxhelper.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      172 2023-06-05 13:32:38.000000 jaxhelper-0.0.3/jaxhelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-05 13:32:38.000000 jaxhelper-0.0.3/jaxhelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       10 2023-06-05 13:32:38.000000 jaxhelper-0.0.3/jaxhelper.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-05 13:32:38.574878 jaxhelper-0.0.3/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1090 2023-06-05 13:32:27.000000 jaxhelper-0.0.3/setup.py
```

### Comparing `jaxhelper-0.0.2/PKG-INFO` & `jaxhelper-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxhelper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Basic tools and helpers for Jax
 Home-page: https://github.com/clashluke/jaxhelper
 Author: Lucas Nestler
 Author-email: github.jaxhelper@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jaxhelper-0.0.2/README.md` & `jaxhelper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jaxhelper-0.0.2/jaxhelper/__init__.py` & `jaxhelper-0.0.3/jaxhelper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         return next(iter(kwargs.values()))
     return None
 
 
 def if_flag(flag: str, baseline=identity):
     def _outer(fn):
         def _fn(*args, **kwargs):
-            if not _GLOBAL_FLAGS[flag]:
+            if not _GLOBAL_FLAGS.get(flag, False):
                 return baseline(*args, **kwargs)
             return fn(*args, **kwargs)
 
         return _fn
 
     return _outer
```

### Comparing `jaxhelper-0.0.2/jaxhelper.egg-info/PKG-INFO` & `jaxhelper-0.0.3/jaxhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxhelper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Basic tools and helpers for Jax
 Home-page: https://github.com/clashluke/jaxhelper
 Author: Lucas Nestler
 Author-email: github.jaxhelper@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jaxhelper-0.0.2/setup.py` & `jaxhelper-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Lucas Nestler",
     author_email="github.jaxhelper@nestler.sh",
     name='jaxhelper',
     license='BSD',
     description='Basic tools and helpers for Jax',
-    version='0.0.2',
+    version='0.0.3',
     long_description=README,
     url='https://github.com/clashluke/jaxhelper',
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     long_description_content_type="text/markdown",
     install_requires=[],
     classifiers=[
```

