# Comparing `tmp/asv_runner-0.0.2.tar.gz` & `tmp/asv_runner-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asv_runner-0.0.2.tar", last modified: Mon Jun  5 03:22:45 2023, max compression
+gzip compressed data, was "asv_runner-0.0.3.tar", last modified: Mon Jun  5 03:29:58 2023, max compression
```

## Comparing `asv_runner-0.0.2.tar` & `asv_runner-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      286 2023-06-05 03:22:39.016460 asv_runner-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/__init__.py
--rw-r--r--   0        0        0     2759 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/aux.py
--rw-r--r--   0        0        0      585 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/benchmarks/__init__.py
--rw-r--r--   0        0        0    10646 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/benchmarks/_base.py
--rw-r--r--   0        0        0      183 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/benchmarks/_exceptions.py
--rw-r--r--   0        0        0     3404 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/benchmarks/_maxrss.py
--rw-r--r--   0        0        0      817 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/benchmarks/mem.py
--rw-r--r--   0        0        0      587 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/benchmarks/peakmem.py
--rw-r--r--   0        0        0     5400 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/benchmarks/time.py
--rw-r--r--   0        0        0     1759 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/benchmarks/timeraw.py
--rw-r--r--   0        0        0      581 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/benchmarks/track.py
--rw-r--r--   0        0        0      317 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/check.py
--rw-r--r--   0        0        0    11444 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/console.py
--rw-r--r--   0        0        0     5865 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/discovery.py
--rw-r--r--   0        0        0     1117 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/run.py
--rw-r--r--   0        0        0     5209 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/server.py
--rw-r--r--   0        0        0      473 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/setup_cache.py
--rw-r--r--   0        0        0     9589 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/statistics.py
--rw-r--r--   0        0        0     1941 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/timing.py
--rw-r--r--   0        0        0     3467 2023-06-05 03:22:39.016460 asv_runner-0.0.2/asv_runner/util.py
--rw-r--r--   0        0        0      838 2023-06-05 03:22:45.464434 asv_runner-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 asv_runner-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      286 2023-06-05 03:29:51.801955 asv_runner-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/__init__.py
+-rw-r--r--   0        0        0     2759 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/aux.py
+-rw-r--r--   0        0        0      585 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/__init__.py
+-rw-r--r--   0        0        0    10646 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/_base.py
+-rw-r--r--   0        0        0      183 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/_exceptions.py
+-rw-r--r--   0        0        0     3404 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/_maxrss.py
+-rw-r--r--   0        0        0      817 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/mem.py
+-rw-r--r--   0        0        0      587 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/peakmem.py
+-rw-r--r--   0        0        0     5400 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/time.py
+-rw-r--r--   0        0        0     1759 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/benchmarks/timeraw.py
+-rw-r--r--   0        0        0      581 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/benchmarks/track.py
+-rw-r--r--   0        0        0      317 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/check.py
+-rw-r--r--   0        0        0    11444 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/console.py
+-rw-r--r--   0        0        0     5865 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/discovery.py
+-rw-r--r--   0        0        0     1117 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/run.py
+-rw-r--r--   0        0        0     5209 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/server.py
+-rw-r--r--   0        0        0      473 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/setup_cache.py
+-rw-r--r--   0        0        0     9809 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/statistics.py
+-rw-r--r--   0        0        0     1941 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/timing.py
+-rw-r--r--   0        0        0     3467 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/util.py
+-rw-r--r--   0        0        0      838 2023-06-05 03:29:58.218110 asv_runner-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 asv_runner-0.0.3/PKG-INFO
```

### Comparing `asv_runner-0.0.2/asv_runner/aux.py` & `asv_runner-0.0.3/asv_runner/aux.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/benchmarks/__init__.py` & `asv_runner-0.0.3/asv_runner/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/benchmarks/_base.py` & `asv_runner-0.0.3/asv_runner/benchmarks/_base.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/benchmarks/_maxrss.py` & `asv_runner-0.0.3/asv_runner/benchmarks/_maxrss.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/benchmarks/mem.py` & `asv_runner-0.0.3/asv_runner/benchmarks/mem.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/benchmarks/peakmem.py` & `asv_runner-0.0.3/asv_runner/benchmarks/peakmem.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/benchmarks/time.py` & `asv_runner-0.0.3/asv_runner/benchmarks/time.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/benchmarks/timeraw.py` & `asv_runner-0.0.3/asv_runner/benchmarks/timeraw.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/benchmarks/track.py` & `asv_runner-0.0.3/asv_runner/benchmarks/track.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/console.py` & `asv_runner-0.0.3/asv_runner/console.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/discovery.py` & `asv_runner-0.0.3/asv_runner/discovery.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/run.py` & `asv_runner-0.0.3/asv_runner/run.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/server.py` & `asv_runner-0.0.3/asv_runner/server.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/statistics.py` & `asv_runner-0.0.3/asv_runner/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 import math
 
 
+def get_err(result, stats):
+    """
+    Return an 'error measure' suitable for informing the user
+    about the spread of the measurement results.
+    """
+    a, b = stats["q_25"], stats["q_75"]
+    return (b - a) / 2
+
+
 def binom_pmf(n, k, p):
     """Binomial pmf = (n choose k) p**k (1 - p)**(n - k)"""
     if not (0 <= k <= n):
         return 0
     if p == 0:
         return 1.0 * (k == 0)
     elif p == 1.0:
```

### Comparing `asv_runner-0.0.2/asv_runner/timing.py` & `asv_runner-0.0.3/asv_runner/timing.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/asv_runner/util.py` & `asv_runner-0.0.3/asv_runner/util.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.2/pyproject.toml` & `asv_runner-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 description = "Core Python benchmark code for ASV"
 authors = [
     { name = "Rohit Goswami", email = "rog32@hi.is" },
 ]
 maintainers = [
     { name = "Rohit Goswami", email = "rog32@hi.is" },
 ]
-version = "0.0.2"
+version = "0.0.3"
 dependencies = []
 requires-python = ">=3.7"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `asv_runner-0.0.2/PKG-INFO` & `asv_runner-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asv-runner
-Version: 0.0.2
+Version: 0.0.3
 Summary: Core Python benchmark code for ASV
 Author-Email: Rohit Goswami <rog32@hi.is>
 Maintainer-Email: Rohit Goswami <rog32@hi.is>
 License: MIT
 Requires-Python: >=3.7
 Provides-Extra: lint
 Requires-Dist: ruff>=0.0.265; extra == "lint"
```

