# Comparing `tmp/mlplatformutils-0.8.2.tar.gz` & `tmp/mlplatformutils-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.8.2.tar", last modified: Mon Jun  5 01:20:55 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.8.3.tar", last modified: Mon Jun  5 05:44:42 2023, max compression
```

## Comparing `mlplatformutils-0.8.2.tar` & `mlplatformutils-0.8.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 01:20:55.669278 mlplatformutils-0.8.2/
--rw-rw-rw-   0        0        0     2999 2023-06-05 01:20:55.670275 mlplatformutils-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.2/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-05 01:20:55.675280 mlplatformutils-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-06-05 01:20:45.000000 mlplatformutils-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:20:55.566216 mlplatformutils-0.8.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 01:20:55.584267 mlplatformutils-0.8.2/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.2/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:20:55.666284 mlplatformutils-0.8.2/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-05 01:20:36.000000 mlplatformutils-0.8.2/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:20:55.622270 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     2999 2023-06-05 01:20:55.000000 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-05 01:20:55.000000 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 01:20:55.000000 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-05 01:20:55.000000 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 01:20:55.000000 mlplatformutils-0.8.2/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 05:44:42.167901 mlplatformutils-0.8.3/
+-rw-rw-rw-   0        0        0     3052 2023-06-05 05:44:42.168902 mlplatformutils-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.3/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-05 05:44:42.173434 mlplatformutils-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-05 05:40:44.000000 mlplatformutils-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:44:41.865402 mlplatformutils-0.8.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 05:44:41.909639 mlplatformutils-0.8.3/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.3/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:44:42.163903 mlplatformutils-0.8.3/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7218 2023-06-05 05:40:12.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-05 05:40:38.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:44:41.973620 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3052 2023-06-05 05:44:41.000000 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-05 05:44:41.000000 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 05:44:41.000000 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-05 05:44:41.000000 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 05:44:41.000000 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.8.2/PKG-INFO` & `mlplatformutils-0.8.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.2
+Version: 0.8.3
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
 # mlplatformutils
 
 <br />
- mlplatformutils for observability
+
+ **mlplatformutils for observability**
 
 ## Structure
 
 <br />
 .<br />
 |-- LICENSE.txt<br />
 |-- README.rst<br />
@@ -57,18 +58,21 @@
 
  ***python -m twine upload dist/* *** <br />
 
 ## Description
 
 <br />
 
-**app_insights_logger** - Constains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights
-**lineagegraph** - Contains **LineageGraph** Class with functions to manage Graph on Azure Cosmos DB enabled with Gremlin
+**app_insights_logger** - Constains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights <br />
+
+<br />
+
+**lineagegraph** - Contains **LineageGraph** Class with functions to manage Graph on Azure Cosmos DB enabled with Gremlin <br />
 
-**platformutils** - Contains platform utility functions to check, install depedencies, check Azure ML Compute
+**platformutils** - Contains platform utility functions to check, install depedencies, check Azure ML Compute 
 
 * is_package_installed
 * install_pip
 * get_environment
 * set_environment
 * assert_amlcompute
 * read_setup_ini
@@ -85,14 +89,14 @@
 * read_from_delta_as_pandas
 * read_from_parquet_as_pandas
 
 ### Examples
 
 <br />
 
-from mlplatformutils.core.platformutils import is_package_installed <br />
+**from mlplatformutils.core.platformutils import is_package_installed** <br />
 print(is_package_installed("pandas")) <br />
-from mlplatformutils.core.app_insights_logger import telemetrylogger <br />
-from mlplatformutils.core.lineagegraph import LineageGraph <br />
-from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2 <br />
-import mlplatformutils.core.platformutils as mlpu <br />
+**from mlplatformutils.core.app_insights_logger import telemetrylogger** <br />
+**from mlplatformutils.core.lineagegraph import LineageGraph** <br />
+**from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2** <br />
+**import mlplatformutils.core.platformutils as mlpu** <br />
 mlpu.__version__ <br />
```

### Comparing `mlplatformutils-0.8.2/setup.py` & `mlplatformutils-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.8.2',
+    version='0.8.3',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.8.2/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.8.3/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.2/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.8.3/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.2/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.8.3/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.2/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.8.3/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.2/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.8.3/src/mlplatformutils/core/sparkutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                         file_path,\
                         file_format,\
                         SOURCE_READ_SPN_VALUE,\
                         SOURCE_READ_SPNKEY_VALUE,\
                         RUN_ID,\
                         PIPELINE_STEP_NAME,\
                         LineageLogger):
-
+    from pyspark.sql.session import SparkSession
     spark = SparkSession.builder.appName("Read from ADLS Gen2").getOrCreate()
     spark.conf.set("fs.azure.account.auth.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "OAuth")
     spark.conf.set("fs.azure.account.oauth.provider.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net",  "org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider")
     spark.conf.set("fs.azure.account.oauth2.client.id."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_READ_SPN_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.secret."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_READ_SPNKEY_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.endpoint."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "https://login.microsoftonline.com/"+AZURE_TENANT_ID+"/oauth2/token")
 
@@ -45,15 +45,15 @@
                        repartition,\
                        df,\
                        SOURCE_WRITE_SPN_VALUE,\
                        SOURCE_WRITE_SPNKEY_VALUE,\
                        RUN_ID,\
                        PIPELINE_STEP_NAME,\
                        LineageLogger):
-                       
+    from pyspark.sql.session import SparkSession             
     spark = SparkSession.builder.appName("Read from ADLS Gen2").getOrCreate()
     spark.conf.set("fs.azure.account.auth.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "OAuth")
     spark.conf.set("fs.azure.account.oauth.provider.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net",  "org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider")
     spark.conf.set("fs.azure.account.oauth2.client.id."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_WRITE_SPN_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.secret."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_WRITE_SPNKEY_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.endpoint."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "https://login.microsoftonline.com/"+AZURE_TENANT_ID+"/oauth2/token")
     
@@ -65,14 +65,15 @@
     if repartition is None:
         df.write.format(file_format).mode('overwrite').save(file_path)
     else:
         df.repartition(repartition).write.format(file_format).mode('overwrite').save(file_path)
     return
 
 def read_from_kusto(kustoOptions,RUN_ID,PIPELINE_STEP_NAME,LineageLogger):
+    from pyspark.sql.session import SparkSession
     pyKusto = SparkSession.builder.appName("kustoPySpark").getOrCreate()
     kustoDf  = pyKusto.read. \
                 format("com.microsoft.kusto.spark.datasource"). \
                 option("kustoCluster", kustoOptions["kustoCluster"]). \
                 option("kustoDatabase", kustoOptions["kustoDatabase"]). \
                 option("kustoQuery", kustoOptions["kustoTable"]). \
                 option("kustoAadAppId", kustoOptions["kustoAADClientID"]). \
@@ -85,15 +86,15 @@
     LineageLogger.update_vertex(documentId, {"KustoDataReadCluster_"+sourcePostfix: str(kustoOptions["kustoCluster"]),\
                                         "KustoDataReadDatabase_"+sourcePostfix: str(kustoOptions["kustoDatabase"]),\
                                         "KustoDataReadQuery_"+sourcePostfix: str(kustoOptions["kustoTable"]),\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(kustoDf.columns)+"]"})                
     return kustoDf
 
 def read_from_azsql(SQL_SERVER_INSTANCE,access_token,Query,RUN_ID,PIPELINE_STEP_NAME,LineageLogger):
-
+    from pyspark.sql.session import SparkSession
     pySql = SparkSession.builder.appName("AzSQLPySpark").getOrCreate()
     df = pySql.read \
         .format("com.microsoft.sqlserver.jdbc.spark") \
         .option("url", SQL_SERVER_INSTANCE) \
         .option("query", Query) \
         .option("accessToken", access_token) \
         .option("encrypt", "true") \
```

### Comparing `mlplatformutils-0.8.2/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.8.3/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.2
+Version: 0.8.3
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
 # mlplatformutils
 
 <br />
- mlplatformutils for observability
+
+ **mlplatformutils for observability**
 
 ## Structure
 
 <br />
 .<br />
 |-- LICENSE.txt<br />
 |-- README.rst<br />
@@ -57,18 +58,21 @@
 
  ***python -m twine upload dist/* *** <br />
 
 ## Description
 
 <br />
 
-**app_insights_logger** - Constains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights
-**lineagegraph** - Contains **LineageGraph** Class with functions to manage Graph on Azure Cosmos DB enabled with Gremlin
+**app_insights_logger** - Constains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights <br />
+
+<br />
+
+**lineagegraph** - Contains **LineageGraph** Class with functions to manage Graph on Azure Cosmos DB enabled with Gremlin <br />
 
-**platformutils** - Contains platform utility functions to check, install depedencies, check Azure ML Compute
+**platformutils** - Contains platform utility functions to check, install depedencies, check Azure ML Compute 
 
 * is_package_installed
 * install_pip
 * get_environment
 * set_environment
 * assert_amlcompute
 * read_setup_ini
@@ -85,14 +89,14 @@
 * read_from_delta_as_pandas
 * read_from_parquet_as_pandas
 
 ### Examples
 
 <br />
 
-from mlplatformutils.core.platformutils import is_package_installed <br />
+**from mlplatformutils.core.platformutils import is_package_installed** <br />
 print(is_package_installed("pandas")) <br />
-from mlplatformutils.core.app_insights_logger import telemetrylogger <br />
-from mlplatformutils.core.lineagegraph import LineageGraph <br />
-from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2 <br />
-import mlplatformutils.core.platformutils as mlpu <br />
+**from mlplatformutils.core.app_insights_logger import telemetrylogger** <br />
+**from mlplatformutils.core.lineagegraph import LineageGraph** <br />
+**from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2** <br />
+**import mlplatformutils.core.platformutils as mlpu** <br />
 mlpu.__version__ <br />
```

### Comparing `mlplatformutils-0.8.2/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.8.3/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

