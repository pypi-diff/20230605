# Comparing `tmp/stablerandom-0.6.44.tar.gz` & `tmp/stablerandom-0.6.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stablerandom-0.6.44.tar", max compression
+gzip compressed data, was "stablerandom-0.6.45.tar", max compression
```

## Comparing `stablerandom-0.6.44.tar` & `stablerandom-0.6.45.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-05-19 22:47:15.852869 stablerandom-0.6.44/LICENSE.txt
--rw-r--r--   0        0        0     2040 2023-05-19 22:47:15.852869 stablerandom-0.6.44/README.md
--rw-r--r--   0        0        0      452 2023-05-19 22:47:31.529219 stablerandom-0.6.44/pyproject.toml
--rw-r--r--   0        0        0      145 2023-05-19 22:47:15.852869 stablerandom-0.6.44/stablerandom/__init__.py
--rw-r--r--   0        0        0     3633 2023-05-19 22:47:15.852869 stablerandom-0.6.44/stablerandom/stablerandom.py
--rw-r--r--   0        0        0     3060 2023-05-19 22:47:15.852869 stablerandom-0.6.44/stablerandom/stablerandom_test.py
--rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 stablerandom-0.6.44/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-05 21:24:13.483295 stablerandom-0.6.45/LICENSE.txt
+-rw-r--r--   0        0        0     2040 2023-06-05 21:24:13.483295 stablerandom-0.6.45/README.md
+-rw-r--r--   0        0        0      452 2023-06-05 21:24:32.799646 stablerandom-0.6.45/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-06-05 21:24:13.483295 stablerandom-0.6.45/stablerandom/__init__.py
+-rw-r--r--   0        0        0     4336 2023-06-05 21:24:13.483295 stablerandom-0.6.45/stablerandom/stablerandom.py
+-rw-r--r--   0        0        0     3148 2023-06-05 21:24:13.483295 stablerandom-0.6.45/stablerandom/stablerandom_test.py
+-rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 stablerandom-0.6.45/PKG-INFO
```

### Comparing `stablerandom-0.6.44/LICENSE.txt` & `stablerandom-0.6.45/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stablerandom-0.6.44/README.md` & `stablerandom-0.6.45/README.md`

 * *Files identical despite different names*

### Comparing `stablerandom-0.6.44/stablerandom/stablerandom.py` & `stablerandom-0.6.45/stablerandom/stablerandom.py`

 * *Files 24% similar despite different names*

```diff
@@ -74,18 +74,28 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         _randomLocalStack.pop()
 
 stablerandom = StableRandom()
 
 # random functions to wrap for stable,
 # from https://numpy.org/doc/stable/reference/random/legacy.html#functions-in-numpy-random
-
+_random_functions = (
+    'rand', 'randn', 'randint', 'random_integers', 'random_sample', 'choice', 'bytes',
+    'shuffle', 'permutation',
+    'beta', 'binomial', 'chisquare', 'dirichlet', 'exponential', 'f', 'gamma', 'geometric', 'gumbel',
+    'hypergeometric', 'laplace', 'logistic', 'lognormal', 'logseries', 'multinomial', 'multivariate_normal',
+    'negative_binomial', 'noncentral_chisquare', 'noncentral_f', 'normal', 'pareto', 'poisson', 'power',
+    'rayleigh', 'standard_cauchy', 'standard_exponential', 'standard_gamma', 'standard_normal',
+    'triangular', 'uniform', 'vonmises', 'wald', 'weibull', 'zipf',
+    'ranf', 'sample'
+)
 
 # List of all available numpy.random functions
-_random_functions = [x for x in dir(numpy.random) if not x.startswith('_')]
+#_omit_functions = ('mtrand')
+#_random_functions = [x for x in dir(numpy.random) if (not x.startswith('_') and not x in _omit_functions)]
 
 # Dictionary Mapping numpy.random functions to their equivalents available on the Generator
 _random_dictionary = {'randint': 'integers', 'random_integers': 'integers',
                       'sample': 'random', 'ranf': 'random', 'random_sample': 'random'}
 
 
 def _wrap_numpy_random(funcName):
```

### Comparing `stablerandom-0.6.44/stablerandom/stablerandom_test.py` & `stablerandom-0.6.45/stablerandom/stablerandom_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,7 +125,12 @@
 
     @stablerandom
     def not_wrapped_rand():
         return numpy.random.rand(1)
 
     assert not_wrapped_randn() != not_wrapped_randn()
     assert not_wrapped_rand() != not_wrapped_rand()
+
+
+def test_mtrand_rand():
+    # should quietly work
+    assert numpy.random.mtrand._rand
```

### Comparing `stablerandom-0.6.44/PKG-INFO` & `stablerandom-0.6.45/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stablerandom
-Version: 0.6.44
+Version: 0.6.45
 Summary: Create stable/repeatable numpy.random applications
 Author: John Heintz
 Author-email: john@gistlabs.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

