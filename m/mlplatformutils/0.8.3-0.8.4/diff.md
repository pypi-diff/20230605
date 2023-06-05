# Comparing `tmp/mlplatformutils-0.8.3.tar.gz` & `tmp/mlplatformutils-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.8.3.tar", last modified: Mon Jun  5 05:44:42 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.8.4.tar", last modified: Mon Jun  5 06:21:57 2023, max compression
```

## Comparing `mlplatformutils-0.8.3.tar` & `mlplatformutils-0.8.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 05:44:42.167901 mlplatformutils-0.8.3/
--rw-rw-rw-   0        0        0     3052 2023-06-05 05:44:42.168902 mlplatformutils-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.3/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-05 05:44:42.173434 mlplatformutils-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-06-05 05:40:44.000000 mlplatformutils-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 05:44:41.865402 mlplatformutils-0.8.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 05:44:41.909639 mlplatformutils-0.8.3/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.3/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 05:44:42.163903 mlplatformutils-0.8.3/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7218 2023-06-05 05:40:12.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-05 05:40:38.000000 mlplatformutils-0.8.3/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-05 05:44:41.973620 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3052 2023-06-05 05:44:41.000000 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-05 05:44:41.000000 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 05:44:41.000000 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-05 05:44:41.000000 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 05:44:41.000000 mlplatformutils-0.8.3/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 06:21:57.054082 mlplatformutils-0.8.4/
+-rw-rw-rw-   0        0        0     3055 2023-06-05 06:21:57.055073 mlplatformutils-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.4/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-05 06:21:57.062077 mlplatformutils-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-05 06:21:51.000000 mlplatformutils-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:21:56.797362 mlplatformutils-0.8.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 06:21:56.834596 mlplatformutils-0.8.4/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.4/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:21:57.049074 mlplatformutils-0.8.4/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3611 2023-06-05 06:21:00.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7274 2023-06-05 06:20:40.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-05 06:21:34.000000 mlplatformutils-0.8.4/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:21:56.939141 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3055 2023-06-05 06:21:56.000000 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-05 06:21:56.000000 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 06:21:56.000000 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-05 06:21:56.000000 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 06:21:56.000000 mlplatformutils-0.8.4/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.8.3/PKG-INFO` & `mlplatformutils-0.8.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.3
+Version: 0.8.4
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
@@ -58,15 +58,15 @@
 
  ***python -m twine upload dist/* *** <br />
 
 ## Description
 
 <br />
 
-**app_insights_logger** - Constains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights <br />
+**app_insights_logger** - Contains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights <br />
 
 <br />
 
 **lineagegraph** - Contains **LineageGraph** Class with functions to manage Graph on Azure Cosmos DB enabled with Gremlin <br />
 
 **platformutils** - Contains platform utility functions to check, install depedencies, check Azure ML Compute 
 
@@ -90,13 +90,13 @@
 * read_from_parquet_as_pandas
 
 ### Examples
 
 <br />
 
 **from mlplatformutils.core.platformutils import is_package_installed** <br />
-print(is_package_installed("pandas")) <br />
+**print(is_package_installed("pandas"))** <br />
 **from mlplatformutils.core.app_insights_logger import telemetrylogger** <br />
 **from mlplatformutils.core.lineagegraph import LineageGraph** <br />
 **from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2** <br />
 **import mlplatformutils.core.platformutils as mlpu** <br />
 mlpu.__version__ <br />
```

### Comparing `mlplatformutils-0.8.3/setup.py` & `mlplatformutils-0.8.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.8.3',
+    version='0.8.4',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.8.3/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.8.4/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.3/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.8.4/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.3/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.8.4/src/mlplatformutils/core/pandasutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         client_id=SOURCE_READ_SPN_VALUE,\
         client_secret=SOURCE_READ_SPNKEY_VALUE,\
         tenant_id=tenant_id
     )
     pandas_df = DeltaTable(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH, file_system=fs).to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
-    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns")
+    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("delta"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     return pandas_df
 
 def read_from_parquet_as_pandas(SOURCE_STORAGE_ACCOUNT_VALUE,\
                                 SOURCE_READ_SPN_VALUE,\
@@ -60,13 +60,13 @@
     client_secret=SOURCE_READ_SPNKEY_VALUE)
     
     handler=pyarrowfs_adlgen2.AccountHandler.from_account_name(SOURCE_STORAGE_ACCOUNT_VALUE,credential=credential)
     fs = pyarrow.fs.PyFileSystem(handler)
     pandas_df = pd.read_parquet(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs)
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
-    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns")
+    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
 
     return pandas_df
```

### Comparing `mlplatformutils-0.8.3/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.8.4/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.3/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.8.4/src/mlplatformutils/core/sparkutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     spark.conf.set("fs.azure.account.oauth.provider.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net",  "org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider")
     spark.conf.set("fs.azure.account.oauth2.client.id."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_READ_SPN_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.secret."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_READ_SPNKEY_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.endpoint."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "https://login.microsoftonline.com/"+AZURE_TENANT_ID+"/oauth2/token")
 
     df = spark.read.format(file_format).load(file_path)
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
-    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns")
+    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(file_path),\
                                              "FileFormat_"+sourcePostfix:str(file_format),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(df.columns)+"]"})
     
     return df
 
 def write_to_adls_gen2(SOURCE_STORAGE_ACCOUNT_VALUE,\
@@ -54,15 +54,15 @@
     spark.conf.set("fs.azure.account.auth.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "OAuth")
     spark.conf.set("fs.azure.account.oauth.provider.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net",  "org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider")
     spark.conf.set("fs.azure.account.oauth2.client.id."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_WRITE_SPN_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.secret."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_WRITE_SPNKEY_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.endpoint."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "https://login.microsoftonline.com/"+AZURE_TENANT_ID+"/oauth2/token")
     
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
-    targetPostfix=get_max_properties_starting_with(documentId,"DataWriteColumns")
+    targetPostfix=get_max_properties_starting_with(documentId,"DataWriteColumns",LineageLogger)
     LineageLogger.update_vertex(documentId, {"DataWriteTarget_"+targetPostfix: str(file_path),\
                                         "FileFormat_"+targetPostfix:file_format,\
                                         "DataWriteColumns_"+targetPostfix:"["+",".join(df.columns)+"]"})
     if repartition is None:
         df.write.format(file_format).mode('overwrite').save(file_path)
     else:
         df.repartition(repartition).write.format(file_format).mode('overwrite').save(file_path)
@@ -78,15 +78,15 @@
                 option("kustoQuery", kustoOptions["kustoTable"]). \
                 option("kustoAadAppId", kustoOptions["kustoAADClientID"]). \
                 option("kustoAadAppSecret", kustoOptions["kustoClientAADClientPassword"]). \
                 option("kustoAadAuthorityID", kustoOptions["kustoAADAuthorityID"]). \
                 load()
     
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
-    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns")
+    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
     LineageLogger.update_vertex(documentId, {"KustoDataReadCluster_"+sourcePostfix: str(kustoOptions["kustoCluster"]),\
                                         "KustoDataReadDatabase_"+sourcePostfix: str(kustoOptions["kustoDatabase"]),\
                                         "KustoDataReadQuery_"+sourcePostfix: str(kustoOptions["kustoTable"]),\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(kustoDf.columns)+"]"})                
     return kustoDf
 
 def read_from_azsql(SQL_SERVER_INSTANCE,access_token,Query,RUN_ID,PIPELINE_STEP_NAME,LineageLogger):
@@ -98,12 +98,12 @@
         .option("query", Query) \
         .option("accessToken", access_token) \
         .option("encrypt", "true") \
         .option("hostNameInCertificate", "*.database.windows.net") \
         .load()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
-    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns")
+    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
     LineageLogger.update_vertex(documentId, {"SqlDataReadServer_"+sourcePostfix: str(SQL_SERVER_INSTANCE),\
                                         "SqlDataReadQuery_"+sourcePostfix: str(Query),\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(df.columns)+"]"})  
     return df
```

### Comparing `mlplatformutils-0.8.3/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.8.4/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.3
+Version: 0.8.4
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
@@ -58,15 +58,15 @@
 
  ***python -m twine upload dist/* *** <br />
 
 ## Description
 
 <br />
 
-**app_insights_logger** - Constains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights <br />
+**app_insights_logger** - Contains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights <br />
 
 <br />
 
 **lineagegraph** - Contains **LineageGraph** Class with functions to manage Graph on Azure Cosmos DB enabled with Gremlin <br />
 
 **platformutils** - Contains platform utility functions to check, install depedencies, check Azure ML Compute 
 
@@ -90,13 +90,13 @@
 * read_from_parquet_as_pandas
 
 ### Examples
 
 <br />
 
 **from mlplatformutils.core.platformutils import is_package_installed** <br />
-print(is_package_installed("pandas")) <br />
+**print(is_package_installed("pandas"))** <br />
 **from mlplatformutils.core.app_insights_logger import telemetrylogger** <br />
 **from mlplatformutils.core.lineagegraph import LineageGraph** <br />
 **from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2** <br />
 **import mlplatformutils.core.platformutils as mlpu** <br />
 mlpu.__version__ <br />
```

### Comparing `mlplatformutils-0.8.3/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.8.4/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

