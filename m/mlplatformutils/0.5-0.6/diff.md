# Comparing `tmp/mlplatformutils-0.5.tar.gz` & `tmp/mlplatformutils-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.5.tar", last modified: Sun Jun  4 21:21:08 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.6.tar", last modified: Sun Jun  4 22:01:24 2023, max compression
```

## Comparing `mlplatformutils-0.5.tar` & `mlplatformutils-0.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 21:21:08.186158 mlplatformutils-0.5/
--rw-rw-rw-   0        0        0     3046 2023-06-04 21:21:08.187156 mlplatformutils-0.5/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-06-04 02:08:17.000000 mlplatformutils-0.5/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-04 21:21:08.192152 mlplatformutils-0.5/setup.cfg
--rw-rw-rw-   0        0        0      640 2023-06-04 21:21:04.000000 mlplatformutils-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 21:21:08.084007 mlplatformutils-0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 21:21:08.105603 mlplatformutils-0.5/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.5/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 21:21:08.182153 mlplatformutils-0.5/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.5/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.5/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.5/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.5/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.5/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.5/src/mlplatformutils/core/sparkutils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 21:21:08.150152 mlplatformutils-0.5/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3046 2023-06-04 21:21:07.000000 mlplatformutils-0.5/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-06-04 21:21:07.000000 mlplatformutils-0.5/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 21:21:07.000000 mlplatformutils-0.5/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-04 21:21:07.000000 mlplatformutils-0.5/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-04 21:21:07.000000 mlplatformutils-0.5/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 22:01:24.385226 mlplatformutils-0.6/
+-rw-rw-rw-   0        0        0     3625 2023-06-04 22:01:24.386211 mlplatformutils-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-04 02:08:17.000000 mlplatformutils-0.6/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-04 22:01:24.390744 mlplatformutils-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      536 2023-06-04 22:00:52.000000 mlplatformutils-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 22:01:24.153628 mlplatformutils-0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 22:01:24.191636 mlplatformutils-0.6/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.6/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 22:01:24.381209 mlplatformutils-0.6/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.6/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.6/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.6/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.6/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.6/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.6/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       19 2023-06-04 22:00:56.000000 mlplatformutils-0.6/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-04 22:01:24.272642 mlplatformutils-0.6/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3625 2023-06-04 22:01:23.000000 mlplatformutils-0.6/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-04 22:01:24.000000 mlplatformutils-0.6/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 22:01:23.000000 mlplatformutils-0.6/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-04 22:01:23.000000 mlplatformutils-0.6/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-04 22:01:23.000000 mlplatformutils-0.6/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.5/PKG-INFO` & `mlplatformutils-0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.5
+Version: 0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Description: # mlplatformutils
         
@@ -39,20 +39,25 @@
         |   |-- |-- lineagegraph.py<br />
         |   |-- |-- app_insights_logger.py<br />
         <br />
         
         ## Instructions
         
         <br />
-         install twine - twine is a utility package that is used for publishing Python packages on PyPI
-         python -m pip install twine 
-         Build Package - create the source distribution of the package
-         python setup.py sdist 
-         Upload Package to PyPI
-         python -m twine upload dist/*
+         install twine - twine is a utility package that is used for publishing Python packages on PyPI <br />
+         
+         **python -m pip install twine** <br />
+         
+         Build Package - create the source distribution of the package <br />
+         
+         **python setup.py sdist** <br />
+         
+         Upload Package to PyPI <br />
+        
+         ***python -m twine upload dist/* *** <br />
         
         ## Description
         
         <br />
         
         **app_insights_logger** - Constains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights
         **lineagegraph** - Contains **LineageGraph** Class with functions to manage Graph on Azure Cosmos DB enabled with Gremlin
@@ -74,10 +79,18 @@
         * read_from_azsql
         
         **pandasutils** - Contains functions to read data from Azure Data Lake Gen2 (from Delta Format or Parquet Format) into Pandas Dataframe without Spark while ensuring integrated Lineage Graph Logging.
         
         * read_from_delta_as_pandas
         * read_from_parquet_as_pandas
         
+        ### Examples
+        from mlplatformutils.core.platformutils import is_package_installed
+        print(is_package_installed("pandas"))
+        from mlplatformutils.core.app_insights_logger import telemetrylogger
+        from mlplatformutils.core.lineagegraph import LineageGraph
+        from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2
+        import mlplatformutils.core.platformutils as mlpu
+        mlpu.__version__
 Keywords: mlplatformutils
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.5/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.6/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.5/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.6/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.5/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.6/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.5/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.6/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.5/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.6/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.5/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.6/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.5
+Version: 0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Description: # mlplatformutils
         
@@ -39,20 +39,25 @@
         |   |-- |-- lineagegraph.py<br />
         |   |-- |-- app_insights_logger.py<br />
         <br />
         
         ## Instructions
         
         <br />
-         install twine - twine is a utility package that is used for publishing Python packages on PyPI
-         python -m pip install twine 
-         Build Package - create the source distribution of the package
-         python setup.py sdist 
-         Upload Package to PyPI
-         python -m twine upload dist/*
+         install twine - twine is a utility package that is used for publishing Python packages on PyPI <br />
+         
+         **python -m pip install twine** <br />
+         
+         Build Package - create the source distribution of the package <br />
+         
+         **python setup.py sdist** <br />
+         
+         Upload Package to PyPI <br />
+        
+         ***python -m twine upload dist/* *** <br />
         
         ## Description
         
         <br />
         
         **app_insights_logger** - Constains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights
         **lineagegraph** - Contains **LineageGraph** Class with functions to manage Graph on Azure Cosmos DB enabled with Gremlin
@@ -74,10 +79,18 @@
         * read_from_azsql
         
         **pandasutils** - Contains functions to read data from Azure Data Lake Gen2 (from Delta Format or Parquet Format) into Pandas Dataframe without Spark while ensuring integrated Lineage Graph Logging.
         
         * read_from_delta_as_pandas
         * read_from_parquet_as_pandas
         
+        ### Examples
+        from mlplatformutils.core.platformutils import is_package_installed
+        print(is_package_installed("pandas"))
+        from mlplatformutils.core.app_insights_logger import telemetrylogger
+        from mlplatformutils.core.lineagegraph import LineageGraph
+        from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2
+        import mlplatformutils.core.platformutils as mlpu
+        mlpu.__version__
 Keywords: mlplatformutils
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.5/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.6/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 src/mlplatformutils.egg-info/requires.txt
 src/mlplatformutils.egg-info/top_level.txt
 src/mlplatformutils/core/__init__.py
 src/mlplatformutils/core/app_insights_logger.py
 src/mlplatformutils/core/lineagegraph.py
 src/mlplatformutils/core/pandasutils.py
 src/mlplatformutils/core/platformutils.py
-src/mlplatformutils/core/sparkutils.py
+src/mlplatformutils/core/sparkutils.py
+src/mlplatformutils/core/version.py
```

