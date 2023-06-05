# Comparing `tmp/amukhsimov-jupyter-templates-bigdata-0.0.8.tar.gz` & `tmp/amukhsimov-jupyter-templates-bigdata-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amukhsimov-jupyter-templates-bigdata-0.0.8.tar", last modified: Tue May 23 13:40:54 2023, max compression
+gzip compressed data, was "amukhsimov-jupyter-templates-bigdata-0.0.9.tar", last modified: Mon Jun  5 10:15:18 2023, max compression
```

## Comparing `amukhsimov-jupyter-templates-bigdata-0.0.8.tar` & `amukhsimov-jupyter-templates-bigdata-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:40:54.033609 amukhsimov-jupyter-templates-bigdata-0.0.8/
--rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 13:40:54.033424 amukhsimov-jupyter-templates-bigdata-0.0.8/PKG-INFO
--rw-r--r--   0 amukhsimov   (502) staff       (20)     1998 2023-05-23 10:23:41.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/README.md
--rw-r--r--   0 amukhsimov   (502) staff       (20)       38 2023-05-23 13:40:54.033662 amukhsimov-jupyter-templates-bigdata-0.0.8/setup.cfg
--rw-r--r--   0 amukhsimov   (502) staff       (20)      944 2023-05-23 13:40:45.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/setup.py
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:40:54.031531 amukhsimov-jupyter-templates-bigdata-0.0.8/src/
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:40:54.032449 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/
--rw-r--r--   0 amukhsimov   (502) staff       (20)       79 2023-05-23 13:05:45.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/__init__.py
--rw-r--r--   0 amukhsimov   (502) staff       (20)     9788 2023-05-23 13:40:30.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/connectors.py
--rw-r--r--   0 amukhsimov   (502) staff       (20)      808 2023-05-23 08:22:13.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/crypto.py
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:40:54.033222 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/
--rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 13:40:53.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
--rw-r--r--   0 amukhsimov   (502) staff       (20)      496 2023-05-23 13:40:53.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)        1 2023-05-23 13:40:53.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       54 2023-05-23 13:40:53.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       37 2023-05-23 13:40:53.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-06-05 10:15:18.920508 amukhsimov-jupyter-templates-bigdata-0.0.9/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-06-05 10:15:18.920305 amukhsimov-jupyter-templates-bigdata-0.0.9/PKG-INFO
+-rw-r--r--   0 amukhsimov   (502) staff       (20)     2064 2023-06-05 10:15:14.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/README.md
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       38 2023-06-05 10:15:18.920558 amukhsimov-jupyter-templates-bigdata-0.0.9/setup.cfg
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      944 2023-06-05 10:14:26.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/setup.py
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-06-05 10:15:18.918455 amukhsimov-jupyter-templates-bigdata-0.0.9/src/
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-06-05 10:15:18.919232 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       79 2023-05-23 13:05:45.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata/__init__.py
+-rw-r--r--   0 amukhsimov   (502) staff       (20)    10001 2023-05-25 09:37:57.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata/connectors.py
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      808 2023-05-23 08:22:13.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata/crypto.py
+-rw-r--r--   0 amukhsimov   (502) staff       (20)        0 2023-05-25 09:34:58.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata/functions.py
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-06-05 10:15:18.920080 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata.egg-info/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-06-05 10:15:18.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      550 2023-06-05 10:15:18.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)        1 2023-06-05 10:15:18.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       54 2023-06-05 10:15:18.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       37 2023-06-05 10:15:18.000000 amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.8/README.md` & `amukhsimov-jupyter-templates-bigdata-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,18 @@
  - `REMOTE_SPARK_DRIVER_MEMORY=16g`
  - `REMOTE_SPARK_DRIVE_MAX_RESULTS_SIZE=16g`
  - `REMOTE_SPARK_MASTER=spark://<address>:<port>`
  - `REMOTE_SPARK_HADOOP_FS_DEFAULT_FS=hdfs://<address>:<port>`
  - `REMOTE_SPARK_SQL_WAREHOUSE_DIR=hdfs://<address>:<port>/path/to/warehouse`
 
 
+ - `HADOOPNAMENODE_HOST=spark47`
+ - `HADOOPNAMENODE_PORT=9000`
+
+
  - `IABS_PROD_IP=<encrypted text>`
  - `IABS_PROD_PORT=<encrypted text>`
  - `IABS_PROD_SID=<encrypted text>`
  - `IABS_PROD_USERNAME=<encrypted text>`
  - `IABS_PROD_PASSWORD=<encrypted text>`
 
 
@@ -51,9 +55,9 @@
 
  - `MICROSERVICES_PREPROD_IP=<encrypted text>`
  - `MICROSERVICES_PREPROD_PORT=<encrypted text>`
  - `MICROSERVICES_PREPROD_USERNAME=<encrypted text>`
  - `MICROSERVICES_PREPROD_PASSWORD=<encrypted text>`
 
 ### BUILDING PACKAGE
- - `python setup.py sdist bdist_wheel`
+ - `python3 setup.py sdist bdist_wheel`
  - `python3 -m twine upload --repository pypi dist/*`
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.8/setup.py` & `amukhsimov-jupyter-templates-bigdata-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'amukhsimov-jupyter-templates-bigdata'
 LONG_DESCRIPTION = 'No description'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="amukhsimov-jupyter-templates-bigdata",
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/connectors.py` & `amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata/connectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 REMOTE_SPARK_DRIVER_MEMORY = os.getenv("REMOTE_SPARK_DRIVER_MEMORY", "32g")
 REMOTE_SPARK_DRIVE_MAX_RESULTS_SIZE = os.getenv("REMOTE_SPARK_DRIVE_MAX_RESULTS_SIZE", "32g")
 REMOTE_SPARK_MASTER = os.getenv("REMOTE_SPARK_MASTER", None)
 # REMOTE_SPARK_DRIVER_EXTRA_CLASS_PATH = os.getenv("REMOTE_SPARK_DRIVER_EXTRA_CLASS_PATH", None)
 REMOTE_SPARK_HADOOP_FS_DEFAULT_FS = os.getenv("REMOTE_SPARK_HADOOP_FS_DEFAULT_FS", None)
 REMOTE_SPARK_SQL_WAREHOUSE_DIR = os.getenv("REMOTE_SPARK_SQL_WAREHOUSE_DIR", None)
 
+HADOOPNAMENODE_HOST = os.getenv("HADOOPNAMENODE_HOST", None)
+HADOOPNAMENODE_PORT = os.getenv("HADOOPNAMENODE_PORT", None)
+
 IABS_PROD_IP = os.getenv("IABS_PROD_IP", None)
 IABS_PROD_PORT = os.getenv("IABS_PROD_PORT", None)
 IABS_PROD_SID = os.getenv("IABS_PROD_SID", None)
 IABS_PROD_USERNAME = os.getenv("IABS_PROD_USERNAME", None)
 IABS_PROD_PASSWORD = os.getenv("IABS_PROD_PASSWORD", None)
 
 IABS_PREPROD_IP = os.getenv("IABS_PREPROD_IP", None)
@@ -91,14 +94,17 @@
             if REMOTE_SPARK_HADOOP_FS_DEFAULT_FS is not None:
                 spark = spark.config("spark.hadoop.fs.defaultFS", REMOTE_SPARK_HADOOP_FS_DEFAULT_FS)
             if REMOTE_SPARK_SQL_WAREHOUSE_DIR is not None:
                 spark = spark.config("spark.sql.warehouse.dir", REMOTE_SPARK_SQL_WAREHOUSE_DIR)
 
             return spark.appName(app_name).getOrCreate()
 
+    def get_namenode_addr(self):
+        return HADOOPNAMENODE_HOST, HADOOPNAMENODE_PORT
+
     def _get_iabs_creds(self, env, master_password):
         if env == "prod":
             ip = decode_text(IABS_PROD_IP, master_password)
             port = decode_text(IABS_PROD_PORT, master_password)
             sid = decode_text(IABS_PROD_SID, master_password)
             username = decode_text(IABS_PROD_USERNAME, master_password)
             password = decode_text(IABS_PROD_PASSWORD, master_password)
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/crypto.py` & `amukhsimov-jupyter-templates-bigdata-0.0.9/src/amukhsimov_jupyter_templates_bigdata/crypto.py`

 * *Files identical despite different names*

