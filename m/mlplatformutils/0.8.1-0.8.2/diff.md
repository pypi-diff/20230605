# Comparing `tmp/mlplatformutils-0.8.1.tar.gz` & `tmp/mlplatformutils-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.8.1.tar", last modified: Mon Jun  5 01:15:38 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.8.2.tar", last modified: Mon Jun  5 01:20:55 2023, max compression
```

## Comparing `mlplatformutils-0.8.1.tar` & `mlplatformutils-0.8.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 01:15:38.141885 mlplatformutils-0.8.1/
--rw-rw-rw-   0        0        0     2938 2023-06-05 01:15:38.142886 mlplatformutils-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.1/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-05 01:15:38.156886 mlplatformutils-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-06-05 01:15:25.000000 mlplatformutils-0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:15:38.012061 mlplatformutils-0.8.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 01:15:38.032568 mlplatformutils-0.8.1/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.1/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:15:38.137886 mlplatformutils-0.8.1/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-05 01:04:22.000000 mlplatformutils-0.8.1/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:15:38.094344 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     2938 2023-06-05 01:15:37.000000 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-05 01:15:37.000000 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 01:15:37.000000 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-05 01:15:37.000000 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 01:15:37.000000 mlplatformutils-0.8.1/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 01:20:55.669278 mlplatformutils-0.8.2/
+-rw-rw-rw-   0        0        0     2999 2023-06-05 01:20:55.670275 mlplatformutils-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.2/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-05 01:20:55.675280 mlplatformutils-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-05 01:20:45.000000 mlplatformutils-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:20:55.566216 mlplatformutils-0.8.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 01:20:55.584267 mlplatformutils-0.8.2/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.2/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:20:55.666284 mlplatformutils-0.8.2/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-05 01:20:36.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:20:55.622270 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     2999 2023-06-05 01:20:55.000000 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-05 01:20:55.000000 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 01:20:55.000000 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-05 01:20:55.000000 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 01:20:55.000000 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.8.1/PKG-INFO` & `mlplatformutils-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.1
+Version: 0.8.2
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
@@ -82,14 +82,17 @@
 
 **pandasutils** - Contains functions to read data from Azure Data Lake Gen2 (from Delta Format or Parquet Format) into Pandas Dataframe without Spark while ensuring integrated Lineage Graph Logging.
 
 * read_from_delta_as_pandas
 * read_from_parquet_as_pandas
 
 ### Examples
-from mlplatformutils.core.platformutils import is_package_installed
-print(is_package_installed("pandas"))
-from mlplatformutils.core.app_insights_logger import telemetrylogger
-from mlplatformutils.core.lineagegraph import LineageGraph
-from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2
-import mlplatformutils.core.platformutils as mlpu
-mlpu.__version__
+
+<br />
+
+from mlplatformutils.core.platformutils import is_package_installed <br />
+print(is_package_installed("pandas")) <br />
+from mlplatformutils.core.app_insights_logger import telemetrylogger <br />
+from mlplatformutils.core.lineagegraph import LineageGraph <br />
+from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2 <br />
+import mlplatformutils.core.platformutils as mlpu <br />
+mlpu.__version__ <br />
```

### Comparing `mlplatformutils-0.8.1/setup.py` & `mlplatformutils-0.8.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.8.1',
+    version='0.8.2',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.8.1/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.8.2/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.1/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.8.2/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.1/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.8.2/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.1/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.8.2/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.1/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.8.2/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.1/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.8.2/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.1
+Version: 0.8.2
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
@@ -82,14 +82,17 @@
 
 **pandasutils** - Contains functions to read data from Azure Data Lake Gen2 (from Delta Format or Parquet Format) into Pandas Dataframe without Spark while ensuring integrated Lineage Graph Logging.
 
 * read_from_delta_as_pandas
 * read_from_parquet_as_pandas
 
 ### Examples
-from mlplatformutils.core.platformutils import is_package_installed
-print(is_package_installed("pandas"))
-from mlplatformutils.core.app_insights_logger import telemetrylogger
-from mlplatformutils.core.lineagegraph import LineageGraph
-from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2
-import mlplatformutils.core.platformutils as mlpu
-mlpu.__version__
+
+<br />
+
+from mlplatformutils.core.platformutils import is_package_installed <br />
+print(is_package_installed("pandas")) <br />
+from mlplatformutils.core.app_insights_logger import telemetrylogger <br />
+from mlplatformutils.core.lineagegraph import LineageGraph <br />
+from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2 <br />
+import mlplatformutils.core.platformutils as mlpu <br />
+mlpu.__version__ <br />
```

### Comparing `mlplatformutils-0.8.1/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.8.2/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

