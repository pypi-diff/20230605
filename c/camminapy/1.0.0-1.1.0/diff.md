# Comparing `tmp/camminapy-1.0.0.tar.gz` & `tmp/camminapy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-1.0.0.tar", max compression
+gzip compressed data, was "camminapy-1.1.0.tar", max compression
```

## Comparing `camminapy-1.0.0.tar` & `camminapy-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-1.0.0/LICENSE
--rw-r--r--   0        0        0      176 2023-05-26 07:23:10.043872 camminapy-1.0.0/README.rst
--rw-r--r--   0        0        0      202 2023-05-26 07:23:10.044811 camminapy-1.0.0/camminapy/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-1.0.0/camminapy/data/__init__.py
--rw-r--r--   0        0        0     6293 2023-05-26 07:23:10.045497 camminapy-1.0.0/camminapy/data/resample.py
--rw-r--r--   0        0        0      163 2023-05-25 11:46:26.866899 camminapy-1.0.0/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     1085 2023-05-25 11:44:40.466282 camminapy-1.0.0/camminapy/plot/altair_config.py
--rw-r--r--   0        0        0     6242 2023-05-26 07:23:10.045894 camminapy-1.0.0/camminapy/plot/altair_theme.py
--rw-r--r--   0        0        0     2633 2023-05-25 12:58:34.534445 camminapy-1.0.0/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-1.0.0/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-1.0.0/camminapy/utils/config.py
--rw-r--r--   0        0        0      734 2023-05-26 07:23:10.046191 camminapy-1.0.0/camminapy/utils/logger.py
--rw-r--r--   0        0        0     1083 2023-05-26 07:23:10.050272 camminapy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 camminapy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-1.1.0/LICENSE
+-rw-r--r--   0        0        0      361 2023-05-26 08:44:24.292769 camminapy-1.1.0/README.md
+-rw-r--r--   0        0        0      119 2023-05-26 08:04:14.503813 camminapy-1.1.0/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-1.1.0/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     6299 2023-05-26 08:55:46.589484 camminapy-1.1.0/camminapy/data/resample.py
+-rw-r--r--   0        0        0      163 2023-05-25 11:46:26.866899 camminapy-1.1.0/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     1085 2023-05-25 11:44:40.466282 camminapy-1.1.0/camminapy/plot/altair_config.py
+-rw-r--r--   0        0        0     6242 2023-05-26 07:23:10.045894 camminapy-1.1.0/camminapy/plot/altair_theme.py
+-rw-r--r--   0        0        0     2633 2023-05-25 12:58:34.534445 camminapy-1.1.0/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-1.1.0/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-1.1.0/camminapy/utils/config.py
+-rw-r--r--   0        0        0      734 2023-05-26 07:23:10.046191 camminapy-1.1.0/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1138 2023-06-05 10:50:31.036043 camminapy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 camminapy-1.1.0/PKG-INFO
```

### Comparing `camminapy-1.0.0/LICENSE` & `camminapy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-1.0.0/camminapy/data/resample.py` & `camminapy-1.1.0/camminapy/data/resample.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     pl.DataFrame
         A dataframe with the same columns as the input dataframe and where
         `interpolation_column` is spaced as `interpolation_step` and all other
         data is interpolated onto that timeline.
 
     Info
     -------
-    This is a wrapper that just calls resample_dataframe_polars for each group.
+    This is a wrapper that just calls `resample_dataframe_polars` for each group.
     """
     return pl.concat(
         [
             resample_dataframe_polars(
                 groupdf,
                 interpolation_column=interpolation_column,
                 interpolation_step=interpolation_step,
@@ -140,15 +140,15 @@
     pd.DataFrame
         A dataframe with the same columns as the input dataframe and where
         `interpolation_column` is spaced as `interpolation_step` and all other
         data is interpolated onto that timeline.
 
     Info
     -------
-    This is a wrapper that just calls resample_dataframe_polars.
+    This is a wrapper that just calls `resample_dataframe_polars`.
     """
     return resample_dataframe_polars(
         df=pl.DataFrame(df),
         interpolation_column=interpolation_column,
         interpolation_step=interpolation_step,
         to_log=to_log,
     ).to_pandas()
@@ -181,15 +181,15 @@
     pd.DataFrame
         A dataframe with the same columns as the input dataframe and where
         `interpolation_column` is spaced as `interpolation_step` and all other
         data is interpolated onto that timeline.
 
     Info
     -------
-    This is a wrapper that just calls resample_dataframe_grouped_polars.
+    This is a wrapper that just calls `resample_dataframe_grouped_polars`.
 
     """
     return resample_dataframe_grouped_polars(
         df=pl.DataFrame(df),
         interpolation_column=interpolation_column,
         interpolation_step=interpolation_step,
         group_column=group_column,
```

### Comparing `camminapy-1.0.0/camminapy/plot/altair_config.py` & `camminapy-1.1.0/camminapy/plot/altair_config.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.0.0/camminapy/plot/altair_theme.py` & `camminapy-1.1.0/camminapy/plot/altair_theme.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.0.0/camminapy/plot/footer.py` & `camminapy-1.1.0/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.0.0/camminapy/utils/config.py` & `camminapy-1.1.0/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.0.0/camminapy/utils/logger.py` & `camminapy-1.1.0/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.0.0/pyproject.toml` & `camminapy-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "camminapy"
-version = "1.0.0"
-description = "Personal helper functions and code snippets."
+version = "1.1.0"
+description = "My personal code collection."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
-readme = "README.rst"
+readme = "README.md"
 repository = "https://github.com/thomascamminady/camminapy"
-
+homepage = "https://thomascamminady.github.io/camminapy/camminapy.html"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 altair = "^5.0.0"
 gitpython = "^3.1.31"
-polars = "^0.17.15"
+polars = ">=0.17.15"
 pyarrow = "^12.0.0"
 rich = "^13.3.5"
 toolz = "^0.12.0"
 pdoc = "^13.1.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.1"
```

