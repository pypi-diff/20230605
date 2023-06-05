# Comparing `tmp/factor_pricing_model_risk_model-2023.3.0.tar.gz` & `tmp/factor_pricing_model_risk_model-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factor_pricing_model_risk_model-2023.3.0.tar", max compression
+gzip compressed data, was "factor_pricing_model_risk_model-2023.4.0.tar", max compression
```

## Comparing `factor_pricing_model_risk_model-2023.3.0.tar` & `factor_pricing_model_risk_model-2023.4.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0     1078 2023-03-10 22:08:54.853682 factor_pricing_model_risk_model-2023.3.0/LICENSE
--rw-r--r--   0        0        0     6693 2023-03-10 22:08:54.853682 factor_pricing_model_risk_model-2023.3.0/README.md
--rw-r--r--   0        0        0     2617 2023-03-10 22:08:58.997753 factor_pricing_model_risk_model-2023.3.0/pyproject.toml
--rw-r--r--   0        0        0       25 2023-03-10 22:08:58.969752 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/__init__.py
--rw-r--r--   0        0        0      253 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/accuracy/__init__.py
--rw-r--r--   0        0        0     3060 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/accuracy/bias.py
--rw-r--r--   0        0        0     5199 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/accuracy/value_at_risk.py
--rw-r--r--   0        0        0      113 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/config.py
--rw-r--r--   0        0        0       46 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/engine/__init__.py
--rw-r--r--   0        0        0      183 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/engine/numpy.py
--rw-r--r--   0        0        0     8898 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/factor_risk_model.py
--rw-r--r--   0        0        0     7149 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/pipeline/__init__.py
--rw-r--r--   0        0        0      621 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/pipeline/portfolio.py
--rw-r--r--   0        0        0      796 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/pipeline/returns.py
--rw-r--r--   0        0        0        0 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/py.typed
--rw-r--r--   0        0        0       59 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/regressor/__init__.py
--rw-r--r--   0        0        0     1138 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/regressor/ewls.py
--rw-r--r--   0        0        0     1806 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/regressor/wls.py
--rw-r--r--   0        0        0     2835 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/risk_model.py
--rw-r--r--   0        0        0     2698 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/rolling_factor_risk_model.py
--rw-r--r--   0        0        0     4496 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/rolling_risk_model.py
--rw-r--r--   0        0        0       36 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/statistical/__init__.py
--rw-r--r--   0        0        0     4761 2023-03-10 22:08:54.857682 factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/statistical/pca.py
--rw-r--r--   0        0        0     8376 1970-01-01 00:00:00.000000 factor_pricing_model_risk_model-2023.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-05 21:42:22.109424 factor_pricing_model_risk_model-2023.4.0/LICENSE
+-rw-r--r--   0        0        0     6687 2023-06-05 21:42:22.109424 factor_pricing_model_risk_model-2023.4.0/README.md
+-rw-r--r--   0        0        0     2617 2023-06-05 21:42:27.569488 factor_pricing_model_risk_model-2023.4.0/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-05 21:42:27.525487 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/__init__.py
+-rw-r--r--   0        0        0      253 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/accuracy/__init__.py
+-rw-r--r--   0        0        0     3060 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/accuracy/bias.py
+-rw-r--r--   0        0        0     5199 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/accuracy/value_at_risk.py
+-rw-r--r--   0        0        0      113 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/config.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/dataset/__init__.py
+-rw-r--r--   0        0        0     3255 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/dataset/crypto.py
+-rw-r--r--   0        0        0       46 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/engine/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/engine/numpy.py
+-rw-r--r--   0        0        0    11187 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/factor_risk_model.py
+-rw-r--r--   0        0        0     7438 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/__init__.py
+-rw-r--r--   0        0        0      621 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/portfolio.py
+-rw-r--r--   0        0        0      796 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/returns.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/py.typed
+-rw-r--r--   0        0        0       59 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/regressor/__init__.py
+-rw-r--r--   0        0        0     1138 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/regressor/ewls.py
+-rw-r--r--   0        0        0     2514 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/regressor/wls.py
+-rw-r--r--   0        0        0     2835 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/risk_model.py
+-rw-r--r--   0        0        0     5537 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/rolling_factor_risk_model.py
+-rw-r--r--   0        0        0     5025 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/rolling_risk_model.py
+-rw-r--r--   0        0        0       59 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/statistical/__init__.py
+-rw-r--r--   0        0        0     3932 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/statistical/apca.py
+-rw-r--r--   0        0        0     4728 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/statistical/pca.py
+-rw-r--r--   0        0        0     8370 1970-01-01 00:00:00.000000 factor_pricing_model_risk_model-2023.4.0/PKG-INFO
```

### Comparing `factor_pricing_model_risk_model-2023.3.0/LICENSE` & `factor_pricing_model_risk_model-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.3.0/README.md` & `factor_pricing_model_risk_model-2023.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -139,18 +139,18 @@
 )
 ```
 
 ## Roadmap
 
 The following major features will be enhanced
 
-- Factor exposures computation from factor returns (Q1 2023)
-- Shrinking covariance (Q1 2023)
-- Exponential decay weighted least squares regression (Q1-Q2 2023)
-- Multiple types of running engine, e.g. Tensorflow (Q1-Q2 2023)
-- Multi-asset class factor model (Q2 2023)
-- Fundamental type risk model (Q3 2023)
+- Factor exposures computation from factor returns (Q2 2023)
+- Shrinking covariance (Q2 2023)
+- Exponential decay weighted least squares regression (Q3 2023)
+- Multiple types of running engine, e.g. Tensorflow (Q3 2023)
+- Multi-asset class factor model (Q3 2023)
+- Fundamental type risk model (Q4 2023)
 
 ## Contribution
 
 All levels of contributions are welcomed. Please refer to the [contributing](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/contributing.html)
 section for development and release guidelines.
```

#### html2text {}

```diff
@@ -42,14 +42,14 @@
 risk model regarding an equally weighted portfolio (of which its weights are
 denoted as `weights`), pass the instrument observed returns (denoted as
 `returns`), and either a rolling risk model (to compute the volatility
 forecast) or a time series of volatility forecasts. ``` from
 fpm_risk_model.accuracy import compute_bias_statistics compute_bias_statistics
 ( X=returns, weights=weights, window=window ... ) ``` ## Roadmap The following
 major features will be enhanced - Factor exposures computation from factor
-returns (Q1 2023) - Shrinking covariance (Q1 2023) - Exponential decay weighted
-least squares regression (Q1-Q2 2023) - Multiple types of running engine, e.g.
-Tensorflow (Q1-Q2 2023) - Multi-asset class factor model (Q2 2023) -
-Fundamental type risk model (Q3 2023) ## Contribution All levels of
-contributions are welcomed. Please refer to the [contributing](https://factor-
-pricing-model-risk-model.readthedocs.io/en/latest/contributing.html) section
-for development and release guidelines.
+returns (Q2 2023) - Shrinking covariance (Q2 2023) - Exponential decay weighted
+least squares regression (Q3 2023) - Multiple types of running engine, e.g.
+Tensorflow (Q3 2023) - Multi-asset class factor model (Q3 2023) - Fundamental
+type risk model (Q4 2023) ## Contribution All levels of contributions are
+welcomed. Please refer to the [contributing](https://factor-pricing-model-risk-
+model.readthedocs.io/en/latest/contributing.html) section for development and
+release guidelines.
```

### Comparing `factor_pricing_model_risk_model-2023.3.0/pyproject.toml` & `factor_pricing_model_risk_model-2023.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "factor-pricing-model-risk-model"
-version = "2023.3.0"
+version = "2023.4.0"
 description = "Package to build risk models for factor pricing model"
 authors = ["Factor Pricing Model <factor.pricing.model@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/factorpricingmodel/factor-pricing-model-risk-model"
 documentation = "https://factor-pricing-model-risk-model.readthedocs.io"
 classifiers = [
```

### Comparing `factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/accuracy/bias.py` & `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/accuracy/bias.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/accuracy/value_at_risk.py` & `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/accuracy/value_at_risk.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/factor_risk_model.py` & `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/factor_risk_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+from os.path import join
 from typing import Optional
 
 from numpy import any, diag_indices_from, nan, ndarray
 from pandas import DataFrame, Series
 
 from .regressor import WLS
 from .risk_model import RiskModel
@@ -199,16 +201,17 @@
         if isinstance(y, DataFrame):
             y_input = y.values
 
         # Set the default regressor
         regressor = regressor or WLS()
 
         # Transform the factor exposures from the y input
-        factor_exposures = regressor.fit(X=X, y=y_input)
-        residual_returns = y_input - X @ factor_exposures
+        regressor_result = regressor.fit(X=X, y=y_input)
+        factor_exposures = regressor_result.beta
+        residual_returns = regressor_result.alpha
 
         if isinstance(self.factor_returns, DataFrame):
             factor_exposures = DataFrame(
                 factor_exposures,
                 index=self.factor_exposures.index,
                 columns=y.columns,
             )
@@ -284,7 +287,73 @@
             if isinstance(self._factor_exposures, DataFrame):
                 instruments = instruments[valid_instruments]
 
         if isinstance(self._factor_exposures, DataFrame):
             cov = DataFrame(cov, index=instruments, columns=instruments)
 
         return cov
+
+    def write_directory(self, path: str, format="parquet", **kwargs):
+        """
+        Write the factor risk model to directory.
+
+        Parameters
+        ----------
+        path: str
+          Destination path.
+
+        format: str
+            Supported formats. Default is "parquet". Options
+            are "csv", "parquet" and "hdf".
+
+        **kwargs: dict
+            Optional keyword arguments for the write operation.
+        """
+        method_name = f"to_{format}"
+        getattr(self._factor_exposures, method_name)(
+            join(path, f"factor_exposures.{format}"), **kwargs
+        )
+        getattr(self._factor_returns, method_name)(
+            join(path, f"factor_returns.{format}"), **kwargs
+        )
+        getattr(self._residual_returns, method_name)(
+            join(path, f"residual_returns.{format}"), **kwargs
+        )
+        with open(join(path, "metadata.json"), mode="w+") as fp:
+            json.dump(self.asdict(), fp)
+
+    @classmethod
+    def read_directory(cls, path: str, format: str = "parquet", **kwargs):
+        """
+        Read model from specified directory.
+
+        Parameters
+        ----------
+        path: str
+            Directory to read model from.
+
+        format: str
+            Supported formats. Default is "parquet". Options
+            are "csv", "parquet" and "hdf".
+
+        **kwargs: dict
+            Optional keyword arguments for the write operation.
+        """
+        method_name = f"read_{format}"
+        import pandas
+
+        method = getattr(pandas, method_name)
+        factor_exposures = method(join(path, f"factor_exposures.{format}"), **kwargs)
+        factor_exposures.index.name = None
+        factor_returns = method(join(path, f"factor_returns.{format}"), **kwargs)
+        factor_returns.index.name = None
+        residual_returns = method(join(path, f"residual_returns.{format}"), **kwargs)
+        residual_returns.index.name = None
+        with open(join(path, "metadata.json")) as fp:
+            metadata = json.load(fp)
+
+        return cls(
+            factor_exposures=factor_exposures,
+            factor_returns=factor_returns,
+            residual_returns=residual_returns,
+            **metadata,
+        )
```

### Comparing `factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/pipeline/__init__.py` & `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,18 @@
       A fitted factor risk model.
     """
     model = model.lower().replace("-", "_")
     if model == "pca":
         from ..statistical.pca import PCA
 
         model = PCA(**kwargs)
+    elif model == "apca":
+        from ..statistical.apca import APCA
+
+        model = APCA(**kwargs)
     else:
         raise ValueError(f"Model name {model} is not supported")
 
     return model.fit(X=data)
 
 
 def generate_rolling_factor_risk_model(
@@ -53,18 +57,27 @@
     **kwargs,
 ) -> RollingFactorRiskModel:
     model = model.lower().replace("-", "_")
     if model == "pca":
         from ..statistical.pca import PCA
 
         model = PCA(**model_parameters)
+    elif model == "apca":
+        from ..statistical.apca import APCA
+
+        model = APCA(**model_parameters)
     else:
         raise ValueError(f"Model name {model} is not supported")
     rolling_model = RollingFactorRiskModel(model=model, **kwargs)
-    return rolling_model.fit(X=data, weights=weights)
+
+    params = {}
+    if weights is not None:
+        params["weights"] = weights
+
+    return rolling_model.fit(X=data, **params)
 
 
 def dump_factor_risk_model(
     risk_model: FactorRiskModel,
     metadata_file: str,
     format: str,
     parameters: Optional[Dict] = None,
```

### Comparing `factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/pipeline/portfolio.py` & `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/portfolio.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/pipeline/returns.py` & `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/returns.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/regressor/ewls.py` & `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/regressor/ewls.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/risk_model.py` & `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/risk_model.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/rolling_risk_model.py` & `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/rolling_risk_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 from typing import Dict, Iterable, Optional, Tuple
 
-from pandas import DataFrame
+from pandas import DataFrame, Timestamp
 
 from .config import Config
 from .risk_model import RiskModel
 
 
 class RollingRiskModelConfig(Config):
     """
@@ -72,15 +72,18 @@
         """
         return self._config
 
     def get(self, name, **kwargs) -> RiskModel:
         """
         Return a factor risk model from the given name / key.
         """
-        return self._values.get(name, **kwargs)
+        try:
+            name = Timestamp(name)
+        finally:
+            return self._values.get(name, **kwargs)
 
     def keys(self) -> Iterable[datetime]:
         """
         Return a list of keys.
         """
         return self._values.keys()
 
@@ -92,24 +95,32 @@
 
     def items(self) -> Iterable[Tuple[datetime, RiskModel]]:
         """
         Return a list of tuples with keys and values.
         """
         return self._values.items()
 
-    def fit(self, X: DataFrame, weights: Optional[DataFrame] = None) -> object:
+    def fit(
+        self,
+        X: DataFrame,
+        validity: Optional[DataFrame] = None,
+        weights: Optional[DataFrame] = None,
+    ) -> object:
         """
         Fit the model.
 
         Parameters
         ----------
         X: DataFrame
             The instrument returns of which its index and columns
             are the date / time and return values.
 
+        validity: DataFrame
+            The instrument validity on the date.
+
         weights: DataFrame
             The weights of the instruments, same dimension as the
             instrument returns.
 
         Returns
         -------
         object
@@ -141,16 +152,25 @@
                     weights_input = None
                 elif isinstance(weights, DataFrame):
                     weights_input = weights.loc[index_name]
                 else:
                     raise TypeError(
                         f"Invalid type of weights {weights.__class__.__name__}"
                     )
+
+                if validity is not None:
+                    validity_input = validity.loc[index_name]
+                    X_input = X_input.loc[:, validity_input]
+
+                params = {}
+                if weights_input is not None:
+                    params["weights"] = weights_input
+
                 values[index_name] = self._model.fit(
-                    X=X_input, weights=weights_input
+                    X=X_input.fillna(0.0), **params
                 ).copy()
         except Exception as exc:
             raise RuntimeError(
                 f"Failed to fit at the index {index} due to error: {exc}"
             )
 
         self._values = values
```

### Comparing `factor_pricing_model_risk_model-2023.3.0/src/fpm_risk_model/statistical/pca.py` & `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/statistical/pca.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     demean : Optional[bool]
         Indicate whether to demean before fitting. Default is True.
     speedup: Optional[bool]
         Indicate whether to speed up the computation as much as possible.
         Default is True.
     """
 
-    n_components: int
+    n_components: Union[int, float, str]
     demean: Optional[bool] = True
     speedup: Optional[bool] = True
 
 
 class PCA(FactorRiskModel):
     """
     PCA statistics model.
@@ -113,33 +113,31 @@
         # Exposure matrix (n, N)
         B = eg.multiply(
             U_m,
             eg.array(self._model.singular_values_ * eg.sqrt(T))[:, eg.newaxis],
         )
         # Factor matrix (T, n)
         wls = WLS()
-        F = wls.fit(X=B.T, y=X_fit.T, weights=weights_fit).T
-        # Residual returns (N, T)
-        residual_returns = X_fit - F @ B
+        wls_result = wls.fit(X=B.T, y=X_fit.T, weights=weights_fit)
+        F = wls_result.beta.T
+        residual_returns = wls_result.alpha.T
 
         # Fill back the instruments which don't have any returns
         # with 0.0 exposures and residual returns
         if self._config.speedup:
-            B_reindex = eg.zeros((self._config.n_components, N))
+            B_reindex = eg.zeros((B.shape[0], N))
             residual_returns_reindex = eg.zeros(X.shape)
             B_reindex[:, X_reindex] = B[:, :]
             residual_returns_reindex[:, X_reindex] = residual_returns[:, :]
             B = B_reindex
             residual_returns = residual_returns_reindex
 
         # Convert back to dataframe if necessary
         if isinstance(X, DataFrame):
-            factor_index = [
-                f"factor_{index + 1}" for index in range(self._config.n_components)
-            ]
+            factor_index = [f"factor_{index + 1}" for index in range(B.shape[0])]
             B = DataFrame(B, index=factor_index, columns=X.columns)
             F = DataFrame(F, index=X.index, columns=factor_index)
             residual_returns = DataFrame(
                 residual_returns, index=X.index, columns=X.columns
             )
 
         # Return itself out
```

### Comparing `factor_pricing_model_risk_model-2023.3.0/PKG-INFO` & `factor_pricing_model_risk_model-2023.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factor-pricing-model-risk-model
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Package to build risk models for factor pricing model
 Home-page: https://github.com/factorpricingmodel/factor-pricing-model-risk-model
 License: MIT
 Author: Factor Pricing Model
 Author-email: factor.pricing.model@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -173,19 +173,19 @@
 )
 ```
 
 ## Roadmap
 
 The following major features will be enhanced
 
-- Factor exposures computation from factor returns (Q1 2023)
-- Shrinking covariance (Q1 2023)
-- Exponential decay weighted least squares regression (Q1-Q2 2023)
-- Multiple types of running engine, e.g. Tensorflow (Q1-Q2 2023)
-- Multi-asset class factor model (Q2 2023)
-- Fundamental type risk model (Q3 2023)
+- Factor exposures computation from factor returns (Q2 2023)
+- Shrinking covariance (Q2 2023)
+- Exponential decay weighted least squares regression (Q3 2023)
+- Multiple types of running engine, e.g. Tensorflow (Q3 2023)
+- Multi-asset class factor model (Q3 2023)
+- Fundamental type risk model (Q4 2023)
 
 ## Contribution
 
 All levels of contributions are welcomed. Please refer to the [contributing](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/contributing.html)
 section for development and release guidelines.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: factor-pricing-model-risk-model Version: 2023.3.0
+Metadata-Version: 2.1 Name: factor-pricing-model-risk-model Version: 2023.4.0
 Summary: Package to build risk models for factor pricing model Home-page:
 https://github.com/factorpricingmodel/factor-pricing-model-risk-model License:
 MIT Author: Factor Pricing Model Author-email: factor.pricing.model@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
@@ -64,14 +64,14 @@
 risk model regarding an equally weighted portfolio (of which its weights are
 denoted as `weights`), pass the instrument observed returns (denoted as
 `returns`), and either a rolling risk model (to compute the volatility
 forecast) or a time series of volatility forecasts. ``` from
 fpm_risk_model.accuracy import compute_bias_statistics compute_bias_statistics
 ( X=returns, weights=weights, window=window ... ) ``` ## Roadmap The following
 major features will be enhanced - Factor exposures computation from factor
-returns (Q1 2023) - Shrinking covariance (Q1 2023) - Exponential decay weighted
-least squares regression (Q1-Q2 2023) - Multiple types of running engine, e.g.
-Tensorflow (Q1-Q2 2023) - Multi-asset class factor model (Q2 2023) -
-Fundamental type risk model (Q3 2023) ## Contribution All levels of
-contributions are welcomed. Please refer to the [contributing](https://factor-
-pricing-model-risk-model.readthedocs.io/en/latest/contributing.html) section
-for development and release guidelines.
+returns (Q2 2023) - Shrinking covariance (Q2 2023) - Exponential decay weighted
+least squares regression (Q3 2023) - Multiple types of running engine, e.g.
+Tensorflow (Q3 2023) - Multi-asset class factor model (Q3 2023) - Fundamental
+type risk model (Q4 2023) ## Contribution All levels of contributions are
+welcomed. Please refer to the [contributing](https://factor-pricing-model-risk-
+model.readthedocs.io/en/latest/contributing.html) section for development and
+release guidelines.
```

