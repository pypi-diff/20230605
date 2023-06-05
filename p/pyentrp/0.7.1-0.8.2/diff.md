# Comparing `tmp/pyentrp-0.7.1.tar.gz` & `tmp/pyentrp-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyentrp-0.7.1.tar", last modified: Thu Jun 24 22:38:26 2021, max compression
+gzip compressed data, was "pyentrp-0.8.2.tar", max compression
```

## Comparing `pyentrp-0.7.1.tar` & `pyentrp-0.8.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
-drwxr-xr-x   0 darya      (501) staff       (20)        0 2021-06-24 22:38:26.479604 pyentrp-0.7.1/
--rw-r--r--   0 darya      (501) staff       (20)     4482 2021-06-24 22:38:26.479747 pyentrp-0.7.1/PKG-INFO
-drwxr-xr-x   0 darya      (501) staff       (20)        0 2021-06-24 22:38:26.479528 pyentrp-0.7.1/pyentrp/
--rw-r--r--   0 darya      (501) staff       (20)        0 2021-06-24 22:04:12.039086 pyentrp-0.7.1/pyentrp/__init__.py
--rw-r--r--   0 darya      (501) staff       (20)    11693 2021-06-24 22:12:45.921959 pyentrp-0.7.1/pyentrp/entropy.py
--rw-r--r--   0 darya      (501) staff       (20)      293 2021-06-24 22:04:12.039608 pyentrp-0.7.1/setup.cfg
--rw-r--r--   0 darya      (501) staff       (20)     4325 2021-06-24 22:38:07.564006 pyentrp-0.7.1/setup.py
+-rw-r--r--   0        0        0    12117 2023-06-05 12:02:45.510463 pyentrp-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1744 2023-06-05 12:02:45.510463 pyentrp-0.8.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 12:02:45.514463 pyentrp-0.8.2/pyentrp/__init__.py
+-rw-r--r--   0        0        0    11701 2023-06-05 12:02:45.514463 pyentrp-0.8.2/pyentrp/entropy.py
+-rw-r--r--   0        0        0     1612 2023-06-05 12:02:45.514463 pyentrp-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 pyentrp-0.8.2/PKG-INFO
```

### Comparing `pyentrp-0.7.1/pyentrp/entropy.py` & `pyentrp-0.8.2/pyentrp/entropy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# -*- coding: utf-8 -*-
-
-from __future__ import unicode_literals
+from math import factorial
 
 import numpy as np
-from math import factorial
 
 
 def _embed(x, order=3, delay=1):
-    """Time-delay embedding.
+    """
+    Time-delay embedding.
 
     Parameters
     ----------
     x : 1d-array, shape (n_times)
         Time series
     order : int
         Embedding dimension (order)
@@ -22,67 +20,70 @@
     -------
     embedded : ndarray, shape (n_times - (order - 1) * delay, order)
         Embedded time-series.
     """
     N = len(x)
     Y = np.empty((order, N - (order - 1) * delay))
     for i in range(order):
-        Y[i] = x[i * delay:i * delay + Y.shape[1]]
+        Y[i] = x[i * delay : i * delay + Y.shape[1]]
     return Y.T
 
 
 def util_pattern_space(time_series, lag, dim):
-    """Create a set of sequences with given lag and dimension
+    """
+    Create a set of sequences with given lag and dimension
 
     Args:
        time_series: Vector or string of the sample data
        lag: Lag between beginning of sequences
        dim: Dimension (number of patterns)
 
     Returns:
         2D array of vectors
     """
     n = len(time_series)
 
     if lag * dim > n:
-        raise Exception('Result matrix exceeded size limit, try to change lag or dim.')
+        raise Exception("Result matrix exceeded size limit, try to change lag or dim.")
     elif lag < 1:
-        raise Exception('Lag should be greater or equal to 1.')
+        raise Exception("Lag should be greater or equal to 1.")
 
     pattern_space = np.empty((n - lag * (dim - 1), dim))
     for i in range(n - lag * (dim - 1)):
         for j in range(dim):
             pattern_space[i][j] = time_series[i + j * lag]
 
     return pattern_space
 
 
 def util_standardize_signal(time_series):
     return (time_series - np.mean(time_series)) / np.std(time_series)
 
 
 def util_granulate_time_series(time_series, scale):
-    """Extract coarse-grained time series
+    """
+    Extract coarse-grained time series
 
     Args:
         time_series: Time series
         scale: Scale factor
 
     Returns:
         Vector of coarse-grained time series with given scale factor
     """
     n = len(time_series)
     b = int(np.fix(n / scale))
-    temp = np.reshape(time_series[0:b * scale], (b, scale))
+    temp = np.reshape(time_series[0 : b * scale], (b, scale))
     cts = np.mean(temp, axis=1)
     return cts
 
 
 def shannon_entropy(time_series):
-    """Return the Shannon Entropy of the sample data.
+    """
+    Return the Shannon Entropy of the sample data.
 
     Args:
         time_series: Vector or string of the sample data
 
     Returns:
         The Shannon Entropy as float value
     """
@@ -91,30 +92,31 @@
     if not isinstance(time_series, str):
         time_series = list(time_series)
 
     # Create a frequency data
     data_set = list(set(time_series))
     freq_list = []
     for entry in data_set:
-        counter = 0.
+        counter = 0.0
         for i in time_series:
             if i == entry:
                 counter += 1
         freq_list.append(float(counter) / len(time_series))
 
     # Shannon entropy
     ent = 0.0
     for freq in freq_list:
         ent += freq * np.log2(freq)
     ent = -ent
     return ent
 
 
 def sample_entropy(time_series, sample_length, tolerance=None):
-    """Calculates the sample entropy of degree m of a time_series.
+    """
+    Calculates the sample entropy of degree m of a time_series.
 
     This method uses chebychev norm.
     It is quite fast for random data, but can be slower is there is
     structure in the input time series.
 
     Args:
         time_series: numpy array of time series
@@ -139,35 +141,37 @@
 
     time_series = np.array(time_series)
     if tolerance is None:
         tolerance = 0.1 * np.std(time_series)
 
     n = len(time_series)
 
-    # Ntemp is a vector that holds the number of matches. N[k] holds matches templates of length k
+    # Ntemp is a vector that holds the number of matches
+    # N[k] holds matches templates of length k
     Ntemp = np.zeros(M + 2)
     # Templates of length 0 matches by definition:
     Ntemp[0] = n * (n - 1) / 2
 
     for i in range(n - M - 1):
-        template = time_series[i:(i + M + 1)]  # We have 'M+1' elements in the template
-        rem_time_series = time_series[i + 1:]
+        template = time_series[i : (i + M + 1)]  # We have 'M+1' elements in the template
+        rem_time_series = time_series[i + 1 :]
 
         search_list = np.arange(len(rem_time_series) - M, dtype=np.int32)
         for length in range(1, len(template) + 1):
             hit_list = np.abs(rem_time_series[search_list] - template[length - 1]) < tolerance
             Ntemp[length] += np.sum(hit_list)
             search_list = search_list[hit_list] + 1
 
     sampen = -np.log(Ntemp[1:] / Ntemp[:-1])
     return sampen
 
 
 def multiscale_entropy(time_series, sample_length, tolerance=None, maxscale=None):
-    """Calculate the Multiscale Entropy of the given time series considering
+    """
+    Calculate the Multiscale Entropy of the given time series considering
     different time-scales of the time series.
 
     Args:
         time_series: Time series for analysis
         sample_length: Bandwidth or group of points
         tolerance: Tolerance (default = 0.1*std(time_series))
 
@@ -190,15 +194,16 @@
     for i in range(maxscale):
         temp = util_granulate_time_series(time_series, i + 1)
         mse[i] = sample_entropy(temp, sample_length, tolerance)[-1]
     return mse
 
 
 def permutation_entropy(time_series, order=3, delay=1, normalize=False):
-    """Permutation Entropy.
+    """
+    Permutation Entropy.
 
     Parameters
     ----------
     time_series : list or np.array
         Time series
     order : int
         Order of permutation entropy
@@ -245,54 +250,56 @@
         >>> # Return a value comprised between 0 and 1.
         >>> print(permutation_entropy(x, order=3, normalize=True))
             0.589
     """
     x = np.array(time_series)
     hashmult = np.power(order, np.arange(order))
     # Embed x and sort the order of permutations
-    sorted_idx = _embed(x, order=order, delay=delay).argsort(kind='quicksort')
+    sorted_idx = _embed(x, order=order, delay=delay).argsort(kind="quicksort")
     # Associate unique integer to each permutations
     hashval = (np.multiply(sorted_idx, hashmult)).sum(1)
     # Return the counts
     _, c = np.unique(hashval, return_counts=True)
     # Use np.true_divide for Python 2 compatibility
     p = np.true_divide(c, c.sum())
     pe = -np.multiply(p, np.log2(p)).sum()
     if normalize:
         pe /= np.log2(factorial(order))
     return pe
 
 
 def multiscale_permutation_entropy(time_series, m, delay, scale):
-    """Calculate the Multiscale Permutation Entropy
+    """
+    Calculate the Multiscale Permutation Entropy
 
     Args:
         time_series: Time series for analysis
         m: Order of permutation entropy
         delay: Time delay
         scale: Scale factor
 
     Returns:
         Vector containing Multiscale Permutation Entropy
 
     Reference:
         [1] Francesco Carlo Morabito et al. Multivariate Multi-Scale Permutation Entropy for
-            Complexity Analysis of Alzheimer’s Disease EEG. www.mdpi.com/1099-4300/14/7/1186
+            Complexity Analysis of Alzheimer`s Disease EEG. www.mdpi.com/1099-4300/14/7/1186
         [2] http://www.mathworks.com/matlabcentral/fileexchange/37288-multiscale-permutation-entropy-mpe/content/MPerm.m
     """
     mspe = []
     for i in range(scale):
         coarse_time_series = util_granulate_time_series(time_series, i + 1)
         pe = permutation_entropy(coarse_time_series, order=m, delay=delay)
         mspe.append(pe)
     return mspe
 
 
 def weighted_permutation_entropy(time_series, order=2, delay=1, normalize=False):
-    """Calculate the weighted permutation entropy. Weighted permutation
+    """
+    Calculate the weighted permutation entropy. Weighted permutation
     entropy captures the information in the amplitude of a signal where
     standard permutation entropy only measures the information in the
     ordinal pattern, "motif."
 
     Parameters
     ----------
     time_series : list or np.array
@@ -309,15 +316,15 @@
     -------
     wpe : float
         Weighted Permutation Entropy
 
     References
     ----------
     .. [1] Bilal Fadlallah, Badong Chen, Andreas Keil, and José Príncipe
-           Phys. Rev. E 87, 022911 – Published 20 February 2013
+           Phys. Rev. E 87, 022911 - Published 20 February 2013
 
     Notes
     -----
     Last updated (March 2021) by Samuel Dotson (samgdotson@gmail.com)
 
     Examples
     --------
@@ -334,35 +341,36 @@
         >>> # Return a value comprised between 0 and 1.
         >>> print(permutation_entropy(x, order=3, normalize=True))
             0.547
     """
     x = _embed(time_series, order=order, delay=delay)
 
     weights = np.var(x, axis=1)
-    sorted_idx = x.argsort(kind='quicksort', axis=1)
+    sorted_idx = x.argsort(kind="quicksort", axis=1)
     motifs, c = np.unique(sorted_idx, return_counts=True, axis=0)
     pw = np.zeros(len(motifs))
 
     # TODO hashmap
-    for i, j in zip(weights, sorted_idx):
+    for i, j in zip(weights, sorted_idx):  # noqa: B905
         idx = int(np.where((j == motifs).sum(1) == order)[0])
         pw[idx] += i
 
     pw /= weights.sum()
 
     b = np.log2(pw)
     wpe = -np.dot(pw, b)
     if normalize:
         wpe /= np.log2(factorial(order))
     return wpe
 
 
 # TODO add tests
 def composite_multiscale_entropy(time_series, sample_length, scale, tolerance=None):
-    """Calculate the Composite Multiscale Entropy of the given time series.
+    """
+    Calculate the Composite Multiscale Entropy of the given time series.
 
     Args:
         time_series: Time series for analysis
         sample_length: Number of sequential points of the time series
         scale: Scale factor
         tolerance: Tolerance (default = 0.1...0.2 * std(time_series))
```

