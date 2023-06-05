# Comparing `tmp/lmo-0.5.1.tar.gz` & `tmp/lmo-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.5.1.tar", max compression
+gzip compressed data, was "lmo-0.5.2.tar", max compression
```

## Comparing `lmo-0.5.1.tar` & `lmo-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.5.1/LICENSE
--rw-r--r--   0        0        0      792 2023-05-30 00:24:12.512261 lmo-0.5.1/README.md
--rw-r--r--   0        0        0      738 2023-05-31 01:27:05.830069 lmo-0.5.1/lmo/__init__.py
--rw-r--r--   0        0        0    22917 2023-05-31 01:55:50.420399 lmo-0.5.1/lmo/_lm.py
--rw-r--r--   0        0        0    11824 2023-05-30 21:35:52.549810 lmo-0.5.1/lmo/_lm_co.py
--rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.5.1/lmo/_meta.py
--rw-r--r--   0        0        0     4810 2023-05-31 01:21:35.070718 lmo-0.5.1/lmo/_pwm.py
--rw-r--r--   0        0        0     1615 2023-05-30 21:36:14.694306 lmo-0.5.1/lmo/_utils.py
--rw-r--r--   0        0        0     4467 2023-05-30 20:47:52.462490 lmo-0.5.1/lmo/linalg.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.5.1/lmo/py.typed
--rw-r--r--   0        0        0     3387 2023-05-30 21:31:38.836128 lmo-0.5.1/lmo/stats.py
--rw-r--r--   0        0        0     1609 2023-05-29 19:12:59.718239 lmo-0.5.1/lmo/typing.py
--rw-r--r--   0        0        0     1981 2023-05-31 01:58:05.887410 lmo-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 lmo-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.5.2/LICENSE
+-rw-r--r--   0        0        0      792 2023-05-30 00:24:12.512261 lmo-0.5.2/README.md
+-rw-r--r--   0        0        0      737 2023-06-04 10:26:56.859497 lmo-0.5.2/lmo/__init__.py
+-rw-r--r--   0        0        0    22851 2023-06-05 01:00:55.316572 lmo-0.5.2/lmo/_lm.py
+-rw-r--r--   0        0        0    11816 2023-06-04 14:08:29.938996 lmo-0.5.2/lmo/_lm_co.py
+-rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.5.2/lmo/_meta.py
+-rw-r--r--   0        0        0     4802 2023-06-04 14:08:29.950996 lmo-0.5.2/lmo/_pwm.py
+-rw-r--r--   0        0        0     1615 2023-06-03 20:03:40.058997 lmo-0.5.2/lmo/_utils.py
+-rw-r--r--   0        0        0     2240 2023-06-05 14:45:24.686312 lmo-0.5.2/lmo/diagnostic.py
+-rw-r--r--   0        0        0     4467 2023-05-30 20:47:52.462490 lmo-0.5.2/lmo/linalg.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.5.2/lmo/py.typed
+-rw-r--r--   0        0        0     5394 2023-06-05 14:17:18.849483 lmo-0.5.2/lmo/stats.py
+-rw-r--r--   0        0        0     1609 2023-05-29 19:12:59.718239 lmo-0.5.2/lmo/typing.py
+-rw-r--r--   0        0        0     2057 2023-06-05 14:48:17.622089 lmo-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 lmo-0.5.2/PKG-INFO
```

### Comparing `lmo-0.5.1/LICENSE` & `lmo-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.5.1/README.md` & `lmo-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `lmo-0.5.1/lmo/__init__.py` & `lmo-0.5.2/lmo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     l_variation,
     l_skew,
     l_kurtosis,
 )
 from ._lm_co import (
     l_comoment,
     l_coratio,
-
     l_coloc,
     l_coscale,
     l_corr,
     l_coskew,
     l_cokurtosis,
 )
```

### Comparing `lmo-0.5.1/lmo/_lm.py` & `lmo-0.5.2/lmo/_lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import numpy as np
 import numpy.typing as npt
 
 from ._pwm import b_moment_cov, b_weights
 from ._utils import clean_order, ensure_axis_at
 from .linalg import hosking_jacobi, sandwich, sh_legendre
-from .stats import order_stats
+from .stats import ordered
 from .typing import AnyInt, IntVector, SortKind
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
 # Low-level methods
 
@@ -301,15 +301,15 @@
         - [E. Elamir & A. Seheult (2003) - Trimmed L-moments](
             https://doi.org/10.1016/S0167-9473(02)00250-5)
         - [J.R.M. Hosking (2007) - Some theory and practical uses of trimmed
             L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
 
     """
     # weight-adjusted $x_{i:n}$
-    x_k = order_stats(
+    x_k = ordered(
         a,
         axis=axis,
         dtype=dtype,
         fweights=fweights,
         aweights=aweights,
         sort=sort,
     )
@@ -552,19 +552,19 @@
 
     Alias for [`lmo.l_moment(a, 1, *, **)`][lmo.l_moment].
 
     Examples:
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).standard_cauchy(99)
         >>> x.mean()
-        -7.564850346291148
+        -7.56485034...
         >>> lmo.l_loc(x)
-        -7.56485034629115
+        -7.56485034...
         >>> lmo.l_loc(x, trim=(1, 1))
-        -0.1592418019341137
+        -0.15924180...
 
     Notes:
         If `trim = (0, 0)` (default), the L-location is equivalent to the
         [arithmetic mean](https://wikipedia.org/wiki/Arithmetic_mean).
 
     See Also:
         - [`lmo.l_moment`][lmo.l_moment]
@@ -588,19 +588,19 @@
 
     Alias for [`lmo.l_moment(a, 2, *, **)`][lmo.l_moment].
 
     Examples:
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).standard_cauchy(99)
         >>> x.std()
-        72.8771524453277
+        72.87715244...
         >>> lmo.l_scale(x)
-        9.501123995203486
+        9.501123995...
         >>> lmo.l_scale(x, trim=(1, 1))
-        0.6589932797072331
+        0.658993279...
 
     Notes:
         If `trim = (0, 0)` (default), the L-scale is equivalent to half the
         [Gini mean difference (GMD)](
         https://wikipedia.org/wiki/Gini_mean_difference).
 
     See Also:
@@ -632,19 +632,19 @@
 
     Alias for [`lmo.l_ratio(a, 2, 1, *, **)`][lmo.l_ratio].
 
     Examples:
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).pareto(4.2, 99)
         >>> x.std() / x.mean()
-        1.321611129357151
+        1.32161112...
         >>> lmo.l_variation(x)
-        0.5907363914181409
+        0.59073639...
         >>> lmo.l_variation(x, trim=(0, 1))
-        0.5539504469144685
+        0.55395044...
 
     Notes:
         If `trim = (0, 0)` (default), this is equivalent to the
         [Gini coefficient](https://wikipedia.org/wiki/Arithmetic_mean),
         and lies within the interval $(0, 1)$.
 
     See Also:
@@ -680,17 +680,17 @@
 
     Alias for [`lmo.l_ratio(a, 3, 2, *, **)`][lmo.l_ratio].
 
     Examples:
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).standard_exponential(99)
         >>> lmo.l_skew(x)
-        0.38524343888616047
+        0.38524343...
         >>> lmo.l_skew(x, trim=(0, 1))
-        0.2711613932338941
+        0.27116139...
 
     See Also:
         - [`lmo.l_ratio`][lmo.l_ratio]
         - [`scipy.stats.skew`][scipy.stats.skew]
 
     """
     return l_ratio(a, 3, 2, trim, axis, dtype, **kwargs)
@@ -718,17 +718,17 @@
 
     Alias for [`lmo.l_ratio(a, 4, 2, *, **)`][lmo.l_ratio].
 
     Examples:
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).standard_t(2, 99)
         >>> lmo.l_kurtosis(x)
-        0.28912787109746096
+        0.28912787...
         >>> lmo.l_kurtosis(x, trim=(1, 1))
-        0.19928182131774994
+        0.19928182...
 
     Notes:
         The L-kurtosis $\\tau_4$ lies within the interval
         $[-\\frac{1}{4}, 1)$, and by the L-skewness $\\tau_3$ as
         $5 \\tau_3^2 - 1 \\le 4 \\tau_4$.
 
     See Also:
```

### Comparing `lmo-0.5.1/lmo/_lm_co.py` & `lmo-0.5.2/lmo/_lm_co.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Any, TypeVar, cast
 
 import numpy as np
 from numpy import typing as npt
 
 from ._utils import clean_order
 from ._lm import l_weights
-from .stats import order_stats
+from .stats import ordered
 from .typing import AnyInt, IntVector, SortKind
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
 def l_comoment(
     a: npt.ArrayLike,
@@ -153,15 +153,15 @@
     # the zeroth L-comoment is the delta function, so the L-comoment
     # matrix is the identity matrix
     L_ij[0] = np.eye(m, dtype=dtype)
 
     kwargs = {'axis': -1, 'dtype': dtype, 'sort': sort}
     for j in range(m):
         # concomitants of x[i] w.r.t. x[j] for all i
-        x_k_ij = order_stats(x, x[j], **kwargs)
+        x_k_ij = ordered(x, x[j], **kwargs)
 
         L_ij[1:, :, j] = np.inner(P_r, x_k_ij)
 
     return L_ij.take(_r, 0)  # pyright: ignore [reportUnknownMemberType]
 
 
 def l_coratio(
```

### Comparing `lmo-0.5.1/lmo/_pwm.py` & `lmo-0.5.2/lmo/_pwm.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 __all__ = 'b_weights', 'b_moment_cov'
 
 from typing import Any, TypeVar, cast
 
 import numpy as np
 import numpy.typing as npt
 
-from .stats import order_stats
+from .stats import ordered
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
 def b_weights(
     r: int,
     n: int,
@@ -83,15 +83,15 @@
         - https://wikipedia.org/wiki/Covariance_matrix
 
     References:
         - [E. Elmamir & A. Seheult (2004) - Exact variance structure of sample
             L-moments](https://doi.org/10.1016/S0378-3758(03)00213-1)
 
     """
-    x = order_stats(a, axis=axis, dtype=dtype, **kwargs)
+    x = ordered(a, axis=axis, dtype=dtype, **kwargs)
 
     # ensure the samples are "in front" (along axis=0)
     if axis and x.ndim > 1:
         x = np.moveaxis(x, axis, 0)
 
     n = len(x)
     P_k = b_weights(ks, n, dtype=dtype)
```

### Comparing `lmo-0.5.1/lmo/_utils.py` & `lmo-0.5.2/lmo/_utils.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.1/lmo/linalg.py` & `lmo-0.5.2/lmo/linalg.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.1/lmo/typing.py` & `lmo-0.5.2/lmo/typing.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.1/pyproject.toml` & `lmo-0.5.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["poetry-core", "oldest-supported-numpy"]
 build-backend = "poetry.core.masonry.api"
 
+
 [tool.poetry]
 name = "lmo"
-version = "0.5.1"
+version = "0.5.2"
 description = "L-Moments for robust statistics."
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://jorenham.github.io/lmo/"
 repository = "https://github.com/jorenham/lmo/"
 classifiers = [
@@ -26,39 +27,45 @@
 [tool.poetry.urls]
 Documentation = "https://jorenham.github.io/lmo/"
 "Bug Tracker" = "https://github.com/jorenham/lmo/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.21"
+scipy = { version = "^1.8", python = "<3.12" }
+
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 hypothesis = {extras = ["numpy"], version = "^6.75"}
 pyright = "^1.1"
 ruff = ">=0.0.263,<1.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-material = ">=9.1.9"
-mkdocstrings = {extras = ["python"], version = ">=0.21.2,<1.0"}
 mkdocs-include-markdown-plugin = { version = ">=4.0.4", python = "<3.12" }
+mkdocstrings = {extras = ["python"], version = ">=0.21.2,<1.0"}
 
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = [
     "-ra",
     "-W error",
     "--showlocals",
     "--strict-markers",
     "--strict-config",
     "--doctest-modules",
 ]
-doctest_optionflags = ["NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
+doctest_optionflags = [
+    "NORMALIZE_WHITESPACE",
+    "IGNORE_EXCEPTION_DETAIL",
+    "ELLIPSIS",
+]
 
 
 [tool.pyright]
 include = ["lmo"]
 exclude = [
     "**/__pycache__",
     "**/.pytest_cache",
```

### Comparing `lmo-0.5.1/PKG-INFO` & `lmo-0.5.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmo
-Version: 0.5.1
+Version: 0.5.2
 Summary: L-Moments for robust statistics.
 Home-page: https://jorenham.github.io/lmo/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: numpy (>=1.21,<2.0)
+Requires-Dist: scipy (>=1.8,<2.0) ; python_version < "3.12"
 Project-URL: Bug Tracker, https://github.com/jorenham/lmo/issues
 Project-URL: Documentation, https://jorenham.github.io/lmo/
 Project-URL: Repository, https://github.com/jorenham/lmo/
 Description-Content-Type: text/markdown
 
 <!--head-start-->
```

