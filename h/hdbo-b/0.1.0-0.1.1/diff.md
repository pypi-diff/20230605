# Comparing `tmp/hdbo_b-0.1.0.tar.gz` & `tmp/hdbo_b-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdbo_b-0.1.0.tar", max compression
+gzip compressed data, was "hdbo_b-0.1.1.tar", max compression
```

## Comparing `hdbo_b-0.1.0.tar` & `hdbo_b-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4286 2023-05-31 17:16:09.882042 hdbo_b-0.1.0/HDBOBenchmark/AdditiveFunction.py
--rw-r--r--   0        0        0      150 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/__init__.py
--rw-r--r--   0        0        0      469 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Ackley.py
--rw-r--r--   0        0        0      463 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Branin.py
--rw-r--r--   0        0        0      458 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Bukin.py
--rw-r--r--   0        0        0      471 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Dropwave.py
--rw-r--r--   0        0        0      479 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Eggholder.py
--rw-r--r--   0        0        0     5177 2023-06-03 11:04:17.327082 hdbo_b-0.1.0/HDBOBenchmark/base/FunctionBase.py
--rw-r--r--   0        0        0      490 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Griewank.py
--rw-r--r--   0        0        0      480 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Hartmann6d.py
--rw-r--r--   0        0        0      487 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Holdertable.py
--rw-r--r--   0        0        0      486 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Noise.py
--rw-r--r--   0        0        0      780 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Productsines.py
--rw-r--r--   0        0        0      495 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Rastrigin.py
--rw-r--r--   0        0        0      607 2023-05-31 17:11:02.835231 hdbo_b-0.1.0/HDBOBenchmark/base/Rosenbrock.py
--rw-r--r--   0        0        0      855 2023-05-31 17:11:02.839231 hdbo_b-0.1.0/HDBOBenchmark/base/Shubert.py
--rw-r--r--   0        0        0      763 2023-05-31 17:11:02.839231 hdbo_b-0.1.0/HDBOBenchmark/base/Sphere.py
--rw-r--r--   0        0        0     1085 2023-05-31 17:11:02.839231 hdbo_b-0.1.0/HDBOBenchmark/base/Trid.py
--rw-r--r--   0        0        0      467 2023-05-31 17:11:02.839231 hdbo_b-0.1.0/HDBOBenchmark/base/Zero.py
--rw-r--r--   0        0        0     1003 2023-05-31 17:11:02.839231 hdbo_b-0.1.0/HDBOBenchmark/base/__init__.py
--rw-r--r--   0        0        0     8489 2023-05-31 17:11:02.839231 hdbo_b-0.1.0/HDBOBenchmark/testFuncs.py
--rw-r--r--   0        0        0     1063 2023-06-03 16:36:06.564695 hdbo_b-0.1.0/LICENSE
--rw-r--r--   0        0        0     2552 2023-06-03 16:21:12.435764 hdbo_b-0.1.0/README.md
--rw-r--r--   0        0        0      753 2023-06-03 16:26:08.815317 hdbo_b-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 hdbo_b-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4286 2023-05-31 17:16:09.882042 hdbo_b-0.1.1/HDBOBenchmark/AdditiveFunction.py
+-rw-r--r--   0        0        0      150 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/__init__.py
+-rw-r--r--   0        0        0      469 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Ackley.py
+-rw-r--r--   0        0        0      463 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Branin.py
+-rw-r--r--   0        0        0      458 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Bukin.py
+-rw-r--r--   0        0        0      471 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Dropwave.py
+-rw-r--r--   0        0        0      479 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Eggholder.py
+-rw-r--r--   0        0        0     5177 2023-06-03 11:04:17.327082 hdbo_b-0.1.1/HDBOBenchmark/base/FunctionBase.py
+-rw-r--r--   0        0        0      490 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Griewank.py
+-rw-r--r--   0        0        0      480 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Hartmann6d.py
+-rw-r--r--   0        0        0      487 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Holdertable.py
+-rw-r--r--   0        0        0      486 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Noise.py
+-rw-r--r--   0        0        0      780 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Productsines.py
+-rw-r--r--   0        0        0      495 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Rastrigin.py
+-rw-r--r--   0        0        0      607 2023-05-31 17:11:02.835231 hdbo_b-0.1.1/HDBOBenchmark/base/Rosenbrock.py
+-rw-r--r--   0        0        0      855 2023-05-31 17:11:02.839231 hdbo_b-0.1.1/HDBOBenchmark/base/Shubert.py
+-rw-r--r--   0        0        0      763 2023-05-31 17:11:02.839231 hdbo_b-0.1.1/HDBOBenchmark/base/Sphere.py
+-rw-r--r--   0        0        0     1085 2023-05-31 17:11:02.839231 hdbo_b-0.1.1/HDBOBenchmark/base/Trid.py
+-rw-r--r--   0        0        0      467 2023-05-31 17:11:02.839231 hdbo_b-0.1.1/HDBOBenchmark/base/Zero.py
+-rw-r--r--   0        0        0     1003 2023-05-31 17:11:02.839231 hdbo_b-0.1.1/HDBOBenchmark/base/__init__.py
+-rw-r--r--   0        0        0     8489 2023-05-31 17:11:02.839231 hdbo_b-0.1.1/HDBOBenchmark/testFuncs.py
+-rw-r--r--   0        0        0     1063 2023-06-03 16:36:06.564695 hdbo_b-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4833 2023-06-05 18:32:11.976669 hdbo_b-0.1.1/README.md
+-rw-r--r--   0        0        0      753 2023-06-05 18:32:11.976669 hdbo_b-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5812 1970-01-01 00:00:00.000000 hdbo_b-0.1.1/PKG-INFO
```

### Comparing `hdbo_b-0.1.0/HDBOBenchmark/AdditiveFunction.py` & `hdbo_b-0.1.1/HDBOBenchmark/AdditiveFunction.py`

 * *Files identical despite different names*

### Comparing `hdbo_b-0.1.0/HDBOBenchmark/base/FunctionBase.py` & `hdbo_b-0.1.1/HDBOBenchmark/base/FunctionBase.py`

 * *Files identical despite different names*

### Comparing `hdbo_b-0.1.0/HDBOBenchmark/base/Productsines.py` & `hdbo_b-0.1.1/HDBOBenchmark/base/Productsines.py`

 * *Files identical despite different names*

### Comparing `hdbo_b-0.1.0/HDBOBenchmark/base/Rosenbrock.py` & `hdbo_b-0.1.1/HDBOBenchmark/base/Rosenbrock.py`

 * *Files identical despite different names*

### Comparing `hdbo_b-0.1.0/HDBOBenchmark/base/Shubert.py` & `hdbo_b-0.1.1/HDBOBenchmark/base/Shubert.py`

 * *Files identical despite different names*

### Comparing `hdbo_b-0.1.0/HDBOBenchmark/base/Sphere.py` & `hdbo_b-0.1.1/HDBOBenchmark/base/Sphere.py`

 * *Files identical despite different names*

### Comparing `hdbo_b-0.1.0/HDBOBenchmark/base/Trid.py` & `hdbo_b-0.1.1/HDBOBenchmark/base/Trid.py`

 * *Files identical despite different names*

### Comparing `hdbo_b-0.1.0/HDBOBenchmark/base/__init__.py` & `hdbo_b-0.1.1/HDBOBenchmark/base/__init__.py`

 * *Files identical despite different names*

### Comparing `hdbo_b-0.1.0/HDBOBenchmark/testFuncs.py` & `hdbo_b-0.1.1/HDBOBenchmark/testFuncs.py`

 * *Files identical despite different names*

### Comparing `hdbo_b-0.1.0/LICENSE` & `hdbo_b-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdbo_b-0.1.0/pyproject.toml` & `hdbo_b-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hdbo-b"
-version = "0.1.0"
+version = "0.1.1"
 description = "High-Dimentional Bayesian Benchmark (HDBO-B)"
 license = "MIT"
 authors = ["yiyuiii <yiyuiii@foxmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/yiyuiii/hdbo-b"
 repository = "https://github.com/yiyuiii/hdbo-b"
 documentation = "https://github.com/yiyuiii/hdbo-b#readme"
```

