# Comparing `tmp/distribution_algebra-0.1.8.tar.gz` & `tmp/distribution_algebra-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distribution_algebra-0.1.8.tar", max compression
+gzip compressed data, was "distribution_algebra-0.1.9.tar", max compression
```

## Comparing `distribution_algebra-0.1.8.tar` & `distribution_algebra-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-01-02 23:46:59.569582 distribution_algebra-0.1.8/LICENSE
--rw-r--r--   0        0        0     1669 2023-01-03 04:19:41.690347 distribution_algebra-0.1.8/README.md
--rw-r--r--   0        0        0      635 2023-01-08 22:30:16.894797 distribution_algebra-0.1.8/distribution_algebra/__init__.py
--rw-r--r--   0        0        0        0 2022-12-31 17:10:19.083478 distribution_algebra-0.1.8/distribution_algebra/__main__.py
--rw-r--r--   0        0        0     1711 2023-01-03 00:06:34.416869 distribution_algebra-0.1.8/distribution_algebra/beta.py
--rw-r--r--   0        0        0      283 2023-01-07 23:14:44.916776 distribution_algebra-0.1.8/distribution_algebra/config.py
--rw-r--r--   0        0        0     3866 2023-01-08 22:30:16.898797 distribution_algebra-0.1.8/distribution_algebra/distribution.py
--rw-r--r--   0        0        0      819 2023-01-05 00:18:36.813792 distribution_algebra-0.1.8/distribution_algebra/examples/algebra.py
--rw-r--r--   0        0        0     1776 2023-01-05 00:18:36.813792 distribution_algebra-0.1.8/distribution_algebra/examples/beta_slider.py
--rw-r--r--   0        0        0     3386 2023-01-03 00:06:34.428869 distribution_algebra-0.1.8/distribution_algebra/lognormal.py
--rw-r--r--   0        0        0     2106 2023-01-03 00:06:34.420869 distribution_algebra-0.1.8/distribution_algebra/normal.py
--rw-r--r--   0        0        0     3072 2023-01-08 22:30:16.894797 distribution_algebra-0.1.8/distribution_algebra/plotting.py
--rw-r--r--   0        0        0     1583 2023-01-08 22:30:16.902797 distribution_algebra-0.1.8/distribution_algebra/poisson.py
--rw-r--r--   0        0        0        0 2022-12-28 14:59:28.246863 distribution_algebra-0.1.8/distribution_algebra/py.typed
--rw-r--r--   0        0        0     2239 2023-01-08 22:31:45.204108 distribution_algebra-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       23 2022-12-29 14:46:34.357292 distribution_algebra-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     1970 2023-01-03 00:06:34.444870 distribution_algebra-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0     3304 2023-01-04 14:20:25.778752 distribution_algebra-0.1.8/tests/test_algebra.py
--rw-r--r--   0        0        0     1085 2023-01-03 00:06:34.456870 distribution_algebra-0.1.8/tests/test_lognormal.py
--rw-r--r--   0        0        0      694 2023-01-03 00:06:34.448870 distribution_algebra-0.1.8/tests/test_normal.py
--rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 distribution_algebra-0.1.8/setup.py
--rw-r--r--   0        0        0     3047 1970-01-01 00:00:00.000000 distribution_algebra-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-02 23:46:59.569582 distribution_algebra-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1669 2023-01-03 04:19:41.690347 distribution_algebra-0.1.9/README.md
+-rw-r--r--   0        0        0      635 2023-01-08 22:30:16.894797 distribution_algebra-0.1.9/distribution_algebra/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-31 17:10:19.083478 distribution_algebra-0.1.9/distribution_algebra/__main__.py
+-rw-r--r--   0        0        0     1711 2023-01-03 00:06:34.416869 distribution_algebra-0.1.9/distribution_algebra/beta.py
+-rw-r--r--   0        0        0     1712 2023-01-08 22:32:37.832850 distribution_algebra-0.1.9/distribution_algebra/beta4.py
+-rw-r--r--   0        0        0      283 2023-01-07 23:14:44.916776 distribution_algebra-0.1.9/distribution_algebra/config.py
+-rw-r--r--   0        0        0     3996 2023-01-08 23:05:42.818884 distribution_algebra-0.1.9/distribution_algebra/distribution.py
+-rw-r--r--   0        0        0      819 2023-01-05 00:18:36.813792 distribution_algebra-0.1.9/distribution_algebra/examples/algebra.py
+-rw-r--r--   0        0        0     1776 2023-01-05 00:18:36.813792 distribution_algebra-0.1.9/distribution_algebra/examples/beta_slider.py
+-rw-r--r--   0        0        0     3386 2023-01-03 00:06:34.428869 distribution_algebra-0.1.9/distribution_algebra/lognormal.py
+-rw-r--r--   0        0        0     2106 2023-01-03 00:06:34.420869 distribution_algebra-0.1.9/distribution_algebra/normal.py
+-rw-r--r--   0        0        0     3781 2023-01-08 23:36:01.278263 distribution_algebra-0.1.9/distribution_algebra/plotting.py
+-rw-r--r--   0        0        0     1583 2023-01-08 22:30:16.902797 distribution_algebra-0.1.9/distribution_algebra/poisson.py
+-rw-r--r--   0        0        0        0 2022-12-28 14:59:28.246863 distribution_algebra-0.1.9/distribution_algebra/py.typed
+-rw-r--r--   0        0        0     2260 2023-01-08 23:37:06.451636 distribution_algebra-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       23 2022-12-29 14:46:34.357292 distribution_algebra-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     1970 2023-01-03 00:06:34.444870 distribution_algebra-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     3304 2023-01-04 14:20:25.778752 distribution_algebra-0.1.9/tests/test_algebra.py
+-rw-r--r--   0        0        0     1085 2023-01-03 00:06:34.456870 distribution_algebra-0.1.9/tests/test_lognormal.py
+-rw-r--r--   0        0        0      694 2023-01-03 00:06:34.448870 distribution_algebra-0.1.9/tests/test_normal.py
+-rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 distribution_algebra-0.1.9/setup.py
+-rw-r--r--   0        0        0     3047 1970-01-01 00:00:00.000000 distribution_algebra-0.1.9/PKG-INFO
```

### Comparing `distribution_algebra-0.1.8/LICENSE` & `distribution_algebra-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/README.md` & `distribution_algebra-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/distribution_algebra/__init__.py` & `distribution_algebra-0.1.9/distribution_algebra/__init__.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/distribution_algebra/beta.py` & `distribution_algebra-0.1.9/distribution_algebra/beta.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/distribution_algebra/distribution.py` & `distribution_algebra-0.1.9/distribution_algebra/distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 # Note: Not using `pydantic_dataclass` because it does not support
 # NDArray validation.
 @dataclass(frozen=True, kw_only=True, eq=False)
 class VectorizedDistribution(Generic[T_in]):
     sample: NDArray[T_in]
+    is_continuous: bool = field(default=True, repr=False)
 
     @property
     def mean(self) -> np.float64:
         return self.sample.mean()
 
     @property
     def var(self) -> np.float64:
@@ -63,15 +64,16 @@
     @abstractmethod
     def support(self) -> tuple[float, float]: ...
 
     @abstractmethod
     def draw(self, size: int) -> NDArray[T_in]: ...
 
     def to_vectorized(self) -> VectorizedDistribution[T_in]:
-        return VectorizedDistribution(sample=self.draw(size=SAMPLE_SIZE))
+        return VectorizedDistribution(sample=self.draw(size=SAMPLE_SIZE),
+                                      is_continuous=self.is_continuous)
 
     @abstractmethod
     def pdf(self, linspace: NDArray[np.float64] | NDArray[np.int_]) -> NDArray[np.float64]: ...
 
     def __add__(self, other: Any) -> Any:
         match other:
             case UnivariateDistribution():
```

### Comparing `distribution_algebra-0.1.8/distribution_algebra/examples/algebra.py` & `distribution_algebra-0.1.9/distribution_algebra/examples/algebra.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/distribution_algebra/examples/beta_slider.py` & `distribution_algebra-0.1.9/distribution_algebra/examples/beta_slider.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/distribution_algebra/lognormal.py` & `distribution_algebra-0.1.9/distribution_algebra/lognormal.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/distribution_algebra/normal.py` & `distribution_algebra-0.1.9/distribution_algebra/normal.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/distribution_algebra/plotting.py` & `distribution_algebra-0.1.9/distribution_algebra/plotting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
+from collections import Counter as counter
 from functools import singledispatch
-from typing import Any
+from typing import Any, Counter
 
 import matplotlib.pyplot as plt
 import numpy as np
 from loguru import logger
 from matplotlib.lines import Line2D
 from matplotlib.patches import Polygon
 from numpy.typing import NDArray
@@ -43,50 +44,64 @@
 
 
 @plot.register(VectorizedDistribution)
 def plot_vectorized_distribution(
         vdist: VectorizedDistribution[T_in], ax = None, **kwargs: Any) \
         -> tuple[NDArray[np.float64], NDArray[np.float64], list[Polygon]]:
     ax = ax or plt.gca()
+
+    if not vdist.is_continuous:
+        sample_counter: counter[T_in] = counter(vdist.sample)
+        x: NDArray[np.float64] = np.array(list(sample_counter.keys()), dtype=np.float64)
+        heights: NDArray[np.float64] = np.array(
+            list(sample_counter.values()), dtype=np.float64) / len(vdist.sample)
+        return ax.bar(x, heights, alpha=0.25, align="center", width=0.2, **kwargs) # type: ignore
+
+
     number_of_bins: int = min(len(set(vdist.sample)), 100)
     return ax.hist(vdist.sample, bins=number_of_bins, alpha=0.25, density=True,
                    align="left", **kwargs)  # type: ignore
 
-@logger.catch
+
 def plot_all_distributions() -> None:
     plt.xkcd()
     axes: tuple[tuple[plt.Axes, ...], ...]
     _, axes = plt.subplots(2, 2)
 
     # Normal distributions.
     ax: plt.Axes = axes[0][0]
     a: Normal = Normal(mean=-5.0, var=9.0)
     b: Normal = Normal(mean=1.0, var=4.0)
     plot(a, ax=ax, label=f"{a}")
-    plot(b, ax=ax, label=f"{b}")
+    b_plot = plot(b, ax=ax, label=f"{b}")
+    b_plot[0].set_label("Prob. density func.")
     ax.legend()
 
     # Lognormal distributions.
     ax = axes[0][1]
     l1: Lognormal = Lognormal(mean=10, var=10.0)
-    plot(l1, ax=ax, label=f"{l1}")
+    l1_plot = plot(l1, ax=ax, label=f"{l1}")
+    l1_plot[0].set_label("Prob. density func.")
     ax.legend()
 
     # Beta distributions.
     ax = axes[1][0]
     b1: Beta = Beta(alpha=1, beta=1)
     b2: Beta = Beta(alpha=9, beta=3)
     plot(b1, ax=ax, label=f"{b1}")
-    plot(b2, ax=ax, label=f"{b2}")
+    b2_plot = plot(b2, ax=ax, label=f"{b2}")
+    b2_plot[0].set_label("Prob. density func.")
     ax.legend()
 
     # Poisson distributions.
     ax = axes[1][1]
+    ax.set_xticks(range(20))
     p1: Poisson = Poisson(lam=4)
-    plot(p1, ax=ax, label=f"{p1}")
+    p1_plot = plot(p1, ax=ax, label=f"{p1}")
+    p1_plot[0].set_label("Prob. mass func.")
     ax.legend()
 
     plt.suptitle("Plotting various univariate random distributions.")
     plt.show()
 
 
 if __name__ == '__main__':
```

### Comparing `distribution_algebra-0.1.8/distribution_algebra/poisson.py` & `distribution_algebra-0.1.9/distribution_algebra/poisson.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/pyproject.toml` & `distribution_algebra-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "distribution_algebra"
-version = "0.1.8"
+version = "0.1.9"
 description = "A python package that implements an easy-to-use interface for random variables, statistical distributions, and their algebra."
 readme="README.md"
 license = "GPL-3.0-or-later"
 authors = ["Vaibhav Karve <vkarve@protonmail.com>"]
 keywords = ["statistics", "typed", "python3", "distribution", "random", "algebra"]
 homepage = "https://vaibhavkarve.github.io/distribution-algebra/"
 repository = "https://github.com/vaibhavkarve/distribution-algebra"
@@ -43,14 +43,15 @@
 safety = "^2.3.5"
 py2puml = "^0.6.0"
 pytest-cov = "^4.0.0"
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.0.0"
 mkdocs-git-revision-date-localized-plugin = "^1.1.0"
 mkdocstrings = {version = ">=0.18", extras = ["python"]}
+pyright = ">1.1.286"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 python_version = "3.10"
```

### Comparing `distribution_algebra-0.1.8/tests/conftest.py` & `distribution_algebra-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/tests/test_algebra.py` & `distribution_algebra-0.1.9/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/tests/test_lognormal.py` & `distribution_algebra-0.1.9/tests/test_lognormal.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/tests/test_normal.py` & `distribution_algebra-0.1.9/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `distribution_algebra-0.1.8/setup.py` & `distribution_algebra-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'numpy>=1.24.0,<2.0.0',
  'pydantic>=1.10.4,<2.0.0',
  'scipy>=1.9.3,<2.0.0',
  'wheel>=0.38.1']
 
 setup_kwargs = {
     'name': 'distribution-algebra',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'A python package that implements an easy-to-use interface for random variables, statistical distributions, and their algebra.',
     'long_description': '# distribution-algebra\nA python package that implements an easy-to-use interface for random\nvariables, statistical distributions, and their algebra.\n\nThis Python package is brought to you by [Vaibhav Karve](https://vaibhavkarve.github.io).\n\n`distribution-algebra` recognizes Normal, Lognormal, Beta and Poisson\ndistributions. The package implements an interface to easily construct\nuser-defined Univariate distributions as well Vectorized distributions.\n\nAdditional features include:\n- A `plot` function for probability density/mass function plotting.\n- A `draw` function for drawing random samples of specified size from a given distribution.\n- Addition and multiplication operations defined directly on distributions:\n  - For example, the sum of two Normal (Poisson) distributions is Normal (Poisson).\n  - The product of two Lognormal distributions is Lognormal.\n  - The sum of two arbitrary univariate distributions is expressed as a Vectorized distribution.\n\n\n![Example plot](https://github.com/vaibhavkarve/distribution-algebra/raw/main/docs/example_plot_univariate.png)\n\n\nThis package is written in Python v3.10, and is publicly available\nunder the [GNU-GPL-v3.0\nlicense](https://github.com/vaibhavkarve/normal-form/blob/main/LICENSE).\n\n\n# Installation and usage\n\nTo get started on using this package,\n\n1.  Istall Python 3.10 or higher.\n2.  `python3.10 -m pip install distribution-algebra`\n3.  Use it in a python script (or interactive REPL)\n\n    ```python\n    from distribution_algebra import Beta, Lognormal, Normal, Poisson\n\n    x: Normal = Normal(mean=1.0, var=9.0)\n\ty: Normal = Normal(mean=1.0, var=16.0)\n\n\tassert x + y == Normal(mean=2.0, var=25.0)\n    ```\n',
     'author': 'Vaibhav Karve',
     'author_email': 'vkarve@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://vaibhavkarve.github.io/distribution-algebra/',
```

### Comparing `distribution_algebra-0.1.8/PKG-INFO` & `distribution_algebra-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distribution-algebra
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package that implements an easy-to-use interface for random variables, statistical distributions, and their algebra.
 Home-page: https://vaibhavkarve.github.io/distribution-algebra/
 License: GPL-3.0-or-later
 Keywords: statistics,typed,python3,distribution,random,algebra
 Author: Vaibhav Karve
 Author-email: vkarve@protonmail.com
 Requires-Python: >=3.10,<3.11
```

