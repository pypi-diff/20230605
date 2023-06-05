# Comparing `tmp/datomize-2.1.7.tar.gz` & `tmp/datomize-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datomize-2.1.7.tar", last modified: Thu Jan 12 14:37:48 2023, max compression
+gzip compressed data, was "dist/datomize-2.3.7.tar", last modified: Mon Jun  5 08:54:13 2023, max compression
```

## Comparing `datomize-2.1.7.tar` & `datomize-2.3.7.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-01-12 14:37:48.000000 datomize-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-01-12 14:34:37.000000 datomize-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-01-12 14:37:47.000000 datomize-2.1.7/datomize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-12 14:37:48.000000 datomize-2.1.7/datomize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 14:37:47.000000 datomize-2.1.7/datomize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-12 14:37:47.000000 datomize-2.1.7/datomize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-12 14:37:47.000000 datomize-2.1.7/datomize.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/datoenhancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/datogenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/datomapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/datomizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/datotrainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/datotuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/helpers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/helpers/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/authentication/authentication_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/helpers/autodiscovery/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/autodiscovery/autodiscovery_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/helpers/business_unit_project/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/business_unit_project/business_unit_project_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/common_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/helpers/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/datasource/datasource_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/helpers/generator/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/generator/generator_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/helpers/train/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/train/datatuner_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/train/enhance_ml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/train/train_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/helpers/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/wrapper/evaluation_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/helpers/wrapper/schema_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-01-12 14:37:36.000000 datomize-2.1.7/datomizer/protos/autodiscoveryservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-01-12 14:37:36.000000 datomize-2.1.7/datomizer/protos/datakubeservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-01-12 14:37:36.000000 datomize-2.1.7/datomizer/protos/datasourceconfigservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-01-12 14:37:36.000000 datomize-2.1.7/datomizer/protos/datatunerservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-01-12 14:37:36.000000 datomize-2.1.7/datomizer/protos/enhancemlresults_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-01-12 14:37:36.000000 datomize-2.1.7/datomizer/protos/infrastructuresettings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-01-12 14:37:36.000000 datomize-2.1.7/datomizer/protos/synthschemavalidationresult_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:37:48.000000 datomize-2.1.7/datomizer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/utils/enhance_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/utils/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/utils/step_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-12 14:34:37.000000 datomize-2.1.7/datomizer/utils/thresholds.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 14:37:48.000000 datomize-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-01-12 14:37:46.000000 datomize-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-05 08:54:13.000000 datomize-2.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-05 08:52:02.000000 datomize-2.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 08:54:13.000000 datomize-2.3.7/datomize.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datoenhancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datogenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datomapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datomizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datotrainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/datotuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/authentication/authentication_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/autodiscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/autodiscovery/autodiscovery_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/business_unit_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/business_unit_project/business_unit_project_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/common_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/datasource/datasource_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/generator/generator_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/train/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/train/datatuner_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/train/enhance_ml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/train/train_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/helpers/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/wrapper/evaluation_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/helpers/wrapper/schema_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/autodiscoveryservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/constantsservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/datakubeservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/datasourceconfigservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20073 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/datatunerservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/enhancemlresults_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/fieldsettingsservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/infrastructuresettings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12101 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/privacyevaluationservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21243 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/protos/synthschemavalidationresult_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:54:13.000000 datomize-2.3.7/datomizer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/enhance_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/step_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 08:52:02.000000 datomize-2.3.7/datomizer/utils/thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 08:54:13.000000 datomize-2.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-05 08:54:13.000000 datomize-2.3.7/setup.py
```

### Comparing `datomize-2.1.7/PKG-INFO` & `datomize-2.3.7/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,104 +1,121 @@
-Metadata-Version: 2.1
-Name: datomize
-Version: 2.1.7
-Summary: Datomize python client
-Home-page: https://datomize.github.io/datomizeSDK
-Author: Datomize Ltd.
-Author-email: support@datomize.com
-License: Apache Software License (https://www.apache.org/licenses/LICENSE-2.0)
-Project-URL: Documentation, https://datomize.github.io/datomizeSDK
-Description: Welcome to Datomize Python SDK
-        ==============================
-        
-        Datomize is a Data-Driven Solution to machine learning. Datomize augments source data with synthetic data of exceptional quality, and can be used to generate synthetic replicas, optimize training data with balanced and richer data, and address the data bias challenge.
-        
-        # Getting Started
-        
-        ## Getting your application user & password
-        
-        In order to use the Datomize Python SDK client, you first need to register the Datomize solution. Once registering Datomize, you will be provided with ``username`` and ``password``, which get passed to ``datomize.Datomizer()`` when starting your application.
-        
-        Please register the Datomize solution on Datomize [Registration](https://app.datomize.com/#/dcs-on-boarding-page).
-        
-        ## Installation
-        
-        ```shell
-        pip install datomize
-        ```
-        
-        ## Important links
-        
-        - [Documentation](https://datomize.github.io/datomizeSDK)
-        
-        ### Usage Example
-        
-        ```python
-        # Import relevant packages
-        from datomizer import Datomizer, DatoMapper, DatoTrainer, DatoGenerator, DatoEnhancer
-        from sklearn.datasets import load_iris
-        import pandas as pd
-        
-        # load input data:
-        data = load_iris(return_X_y=False, as_frame=True)
-        df = pd.concat([data.data, data.target], axis=1)
-        
-        # Create a Datomizer with your credentials:
-        datomizer = Datomizer(username=username, password=password)
-        
-        # Create a DatoMapper and analyze the data structure:
-        mapper = DatoMapper(datomizer)
-        mapper.discover(df_map={"df1": df})
-        
-        # Create a DatoTrainer and train the generative model:
-        trainer = DatoTrainer(mapper)
-        trainer.train()
-        
-        # Create a DatoGenerator and generate a syntheyic replica:
-        generator = DatoGenerator(trainer)
-        generator.generate(output_ratio=5)  # 5 times the original number of records will be created
-        synth_data = pd.read_csv(generator.get_generated_data_csv())
-        
-        # Create a DatoEnhancer for a spedific prediction task and generate a balanced and augmented data to enhance your training data:
-        enhancer = DatoEnhancer(mapper)
-        enhancer.generate(target_column="target")
-        train_enhanced = pd.read_csv(enhancer.get_generated_data_csv())
-        ```
-        
-        ### Async Usage Example
-        
-        ```python
-        from datomizer import Datomizer, DatoMapper, DatoTrainer, DatoGenerator
-        
-        datomizer = Datomizer(username=username, password=password)
-        
-        mapper = DatoMapper(datomizer)
-        mapper.discover(df_map={"df1": df}, title="Some Title", wait=False)
-        ...
-        do something...
-        mapper.wait()
-        
-        trainer = DatoTrainer(mapper)
-        trainer.train(wait=False)
-        ...
-        do something...
-        trainer.wait()
-        
-        generator = DatoGenerator(trainer)
-        generator.generate(wait=False)
-        ...
-        do something...
-        generator.wait()
-        
-        dato_df = pd.read_csv(generator.get_generated_data_csv())
-        ```
-        
-Keywords: machine learning
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Welcome to Datomize Python SDK
+==============================
+
+Datomize is a Data-Driven Solution to machine learning. Datomize augments source data with synthetic data of exceptional quality, and can be used to generate synthetic replicas, optimize training data with balanced and richer data, and address the data bias challenge.
+
+# Getting Started
+
+## Getting your application user & password
+
+In order to use the Datomize Python SDK client, you first need to register the Datomize solution. Once registering Datomize, you will be provided with ``username`` and ``password``, which get passed to ``datomize.Datomizer()`` when starting your application.
+
+Please register the Datomize solution on Datomize [Registration](https://app.datomize.com/#/dcs-on-boarding-page).
+
+## Installation
+
+```shell
+pip install datomize
+```
+
+## Important links
+
+- [Documentation](https://datomize.github.io/datomizeSDK)
+
+### Usage Example
+
+```python
+# Import relevant packages
+from datomizer import Datomizer, DatoMapper, DatoTrainer, DatoGenerator, DatoEnhancer
+from sklearn.datasets import load_iris
+import pandas as pd
+
+# load input data:
+data = load_iris(return_X_y=False, as_frame=True)
+df = pd.concat([data.data, data.target], axis=1)
+
+# Create a Datomizer with your credentials:
+datomizer = Datomizer(username=username, password=password)
+
+# Create a DatoMapper and analyze the data structure:
+mapper = DatoMapper(datomizer)
+mapper.discover(df_map={"df1": df})
+
+# Create a DatoTrainer and train the generative model:
+trainer = DatoTrainer(mapper)
+trainer.train()
+
+# Create a DatoGenerator and generate a syntheyic replica:
+generator = DatoGenerator(trainer)
+generator.generate(output_ratio=5)  # 5 times the original number of records will be created
+synth_data = pd.read_csv(generator.get_generated_data_csv())
+
+# Create a DatoEnhancer for a spedific prediction task and generate a balanced and augmented data to enhance your training data:
+enhancer = DatoEnhancer(mapper)
+enhancer.generate(target_column="target")
+train_enhanced = pd.read_csv(enhancer.get_generated_data_csv())
+```
+
+### Async Usage Example
+
+```python
+from datomizer import Datomizer, DatoMapper, DatoTrainer, DatoGenerator
+
+datomizer = Datomizer(username=username, password=password)
+
+mapper = DatoMapper(datomizer)
+mapper.discover(df_map={"df1": df}, title="Some Title", wait=False)
+...
+do something...
+mapper.wait()
+
+trainer = DatoTrainer(mapper)
+trainer.train(wait=False)
+...
+do something...
+trainer.wait()
+
+generator = DatoGenerator(trainer)
+generator.generate(wait=False)
+...
+do something...
+generator.wait()
+
+dato_df = pd.read_csv(generator.get_generated_data_csv())
+```
+
+### Misc examples
+
+```python
+# Import relevant packages
+from datomizer import Datomizer, DatoMapper, DatoTrainer, DatoGenerator, DatoEnhancer
+from datomizer.helpers.wrapper.schema_wrapper import SchemaWrapper
+import pandas as pd
+from sqlalchemy import create_engine
+# load input data:
+db_connection_str = 'mysql+pymysql://guest:relational@relational.fit.cvut.cz/financial'
+db_connection = create_engine(db_connection_str)
+account = pd.read_sql('SELECT * FROM account', con=db_connection)
+loan = pd.read_sql('SELECT * FROM loan', con=db_connection)
+
+# Create a Datomizer with your credentials:
+datomizer = Datomizer(username=username, password=password)
+
+# Create a DatoMapper and analyze the data structure:
+mapper = DatoMapper(datomizer)
+mapper.discover(df_map={"account": account, "loan": loan})
+
+schema: SchemaWrapper = mapper.get_schema()
+schema.add_relation_one2many(table_one="account", column_one="account_id",
+                             table_many="loan", column_many="account_id")
+mapper.schema = schema
+mapper.set_schema()
+# Create a DatoTrainer and train the generative model:
+trainer = DatoTrainer(mapper)
+trainer.train()
+
+# Create a DatoGenerator and generate a syntheyic replica:
+generator = DatoGenerator(trainer)
+generator.generate(output_ratio=1)  # 5 times the original number of records will be created
+synth_account = pd.read_csv(generator.get_generated_data_csv("account"))
+synth_loan = pd.read_csv(generator.get_generated_data_csv("loan"))
+```
```

### Comparing `datomize-2.1.7/datomize.egg-info/SOURCES.txt` & `datomize-2.3.7/datomize.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -20,21 +20,25 @@
 datomizer/helpers/generator/generator_helper.py
 datomizer/helpers/train/datatuner_helper.py
 datomizer/helpers/train/enhance_ml_helper.py
 datomizer/helpers/train/train_helper.py
 datomizer/helpers/wrapper/evaluation_wrapper.py
 datomizer/helpers/wrapper/schema_wrapper.py
 datomizer/protos/autodiscoveryservice_pb2.py
+datomizer/protos/constantsservice_pb2.py
 datomizer/protos/datakubeservice_pb2.py
 datomizer/protos/datasourceconfigservice_pb2.py
 datomizer/protos/datatunerservice_pb2.py
 datomizer/protos/enhancemlresults_pb2.py
+datomizer/protos/fieldsettingsservice_pb2.py
 datomizer/protos/infrastructuresettings_pb2.py
+datomizer/protos/privacyevaluationservice_pb2.py
 datomizer/protos/synthschemavalidationresult_pb2.py
 datomizer/utils/constants.py
 datomizer/utils/enhance_ml.py
 datomizer/utils/exceptions.py
 datomizer/utils/general.py
+datomizer/utils/interfaces.py
 datomizer/utils/messages.py
 datomizer/utils/schema.py
 datomizer/utils/step_types.py
 datomizer/utils/thresholds.py
```

### Comparing `datomize-2.1.7/datomizer/datoenhancer.py` & `datomize-2.3.7/datomizer/datoenhancer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import io
 
 from datomizer import DatoMapper
 from datomizer.helpers import common_helper
 from datomizer.helpers.train import enhance_ml_helper, train_helper
+from datomizer.helpers.train.enhance_ml_helper import DEFAULT_ALGORITHMS, DEFAULT_METRIC
 from datomizer.utils.general import ID, MODELS, ERROR
-from datomizer.utils.messages import MISSING_TARGET_TABLE
+from datomizer.utils.interfaces import DatoGenInterface
+from datomizer.utils.messages import MISSING_TARGET_COLUMN
 from datomizer.utils.step_types import ML_TRAIN_AND_GENERATE
-from datomizer.utils.enhance_ml import Metrics, Algorithms
+from datomizer.utils.enhance_ml import Metrics, Algorithms, map_enum_list
 from datomizer.utils.enhance_ml import assert_column_valid_for_eml
-from datomizer.protos.autodiscoveryservice_pb2 import TableDTO, ColumnDTO
 
 
-class DatoEnhancer(object):
+class DatoEnhancer(DatoGenInterface):
     dato_mapper: DatoMapper
     train_id = 0
     models = []
     metric_list = []
     algorithm_list = []
-    target_table: TableDTO
-    target_column: ColumnDTO
+    target_table: str
+    target_column: str
 
     def __init__(self, dato_mapper: DatoMapper):
         """Create DatoEnhancer object for enhancing the mapped input data for a specific prediction target.
         Args:
             dato_mapper: the DatoMapper object for the input data."""
         dato_mapper.next_step_validation()
         self.dato_mapper = dato_mapper
@@ -32,20 +33,27 @@
     def restore(cls, dato_mapper: DatoMapper, train_id):
         dato_enhancer = cls(dato_mapper)
         dato_enhancer.train_id = train_id
         dato_enhancer.wait()
         return dato_enhancer
 
     def generate(self, target_table: str = "", target_column: str = "",
-                 metric_list: [Metrics] = [], algorithm_list: [Algorithms] = [], wait=True) -> None:
-        self.validate_and_set_params(target_table, target_column, metric_list, algorithm_list)
+                 optimize_metric: Metrics = DEFAULT_METRIC, algorithm_list: [Algorithms] = [], wait=True) -> None:
+        """Trains DatoEnhancer object for enhancing the mapped input data for a specific prediction target.
+        Args:
+            target_table: target table name.
+            target_column: target column name.
+            optimize_metric: Metric which you want model to optimize by.
+            algorithm_list: Algorithms list which you want to use.
+            wait: use wait=False for asynchronous programming; True by default (awaits for the results)."""
+        self.validate_and_set_params(target_table, target_column, optimize_metric, algorithm_list)
 
         self.train_id = enhance_ml_helper.enhance_ml_generate(self.dato_mapper,
-                                                              target_table=self.target_table.name,
-                                                              target_column=self.target_column.name,
+                                                              target_table=self.target_table,
+                                                              target_column=self.target_column,
                                                               metric_list=self.metric_list,
                                                               algorithm_list=self.algorithm_list)
         if wait:
             self.wait()
 
     def wait(self) -> None:
         """Wait until the train method returns."""
@@ -57,30 +65,41 @@
                                                   step_type=ML_TRAIN_AND_GENERATE,
                                                   train_id=self.train_id)
         if status == ERROR:
             raise Exception("Trainer Failed")
         train = train_helper.get_train_iteration(self.dato_mapper, self.train_id)
         self.models = train[MODELS]
 
-    def validate_and_set_params(self, target_table, target_column, metric_list, algorithm_list):
-        assert target_column, MISSING_TARGET_TABLE
-        self.target_table = self.dato_mapper.schema.table(target_table)
-        self.target_column = self.dato_mapper.schema.column(target_table, target_column)
-        assert_column_valid_for_eml(self.target_column)
-        self.metric_list = metric_list
-        self.algorithm_list = algorithm_list
+    def validate_and_set_params(self, target_table, target_column, optimize_metric, algorithm_list):
+        assert target_column, MISSING_TARGET_COLUMN
+        self.target_table = self.dato_mapper.schema.table(target_table).name
+
+        column = self.dato_mapper.schema.column(target_table, target_column)
+        assert_column_valid_for_eml(column)
+        self.target_column = column.name
+
+        if not optimize_metric:
+            optimize_metric = DEFAULT_METRIC
+        self.metric_list = map_enum_list([optimize_metric])
+
+        if not algorithm_list:
+            algorithm_list = DEFAULT_ALGORITHMS
+        self.algorithm_list = map_enum_list(algorithm_list)
+
+    def list_tables(self):
+        return self.dato_mapper.schema.tables_name()
 
-    def get_generated_data(self, is_full: bool = False) -> None:
+    def get_generated_data(self) -> None:
         self.restore_validation()
 
         print(common_helper.get_generated_zip(datomizer=self.dato_mapper.datomizer,
                                               business_unit_id=self.dato_mapper.business_unit_id,
                                               project_id=self.dato_mapper.project_id,
                                               flow_id=self.dato_mapper.flow_id,
-                                              model_id=self.get_model_id(is_full),
+                                              model_id=self.get_model_id(),
                                               train_id=self.train_id))
 
     def get_generated_data_csv(self, table_name: str = None) -> io.StringIO:
         """Get the generated data in a csv format.
                 Args:
                     table_name: the name of the generated data
                 Returns:
```

### Comparing `datomize-2.1.7/datomizer/datogenerator.py` & `datomize-2.3.7/datomizer/datogenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import io
 
 from datomizer import DatoTrainer
 from datomizer.helpers.common_helper import get_flow, wait_for_step_type, get_generated_zip, get_generated_csv
 from datomizer.helpers.generator.generator_helper import generate, assert_output_ratio
 from datomizer.helpers.datasource.datasource_helper import create_target_private_datasource
 from datomizer.utils.general import TARGET_DATASOURCE_ID, ERROR
+from datomizer.utils.interfaces import DatoGenInterface
 from datomizer.utils.step_types import GENERATE
 
 
-class DatoGenerator(object):
+class DatoGenerator(DatoGenInterface):
     dato_trainer: DatoTrainer
     synth_id = 0
     datasource_id = 0
 
     def __init__(self, dato_trainer: DatoTrainer):
         """Create DatoGenerator object for generating data using the trained generative model.
         Args:
@@ -63,14 +64,17 @@
                                     flow_id=self.synth_id,
                                     is_synth=True,
                                     step_type=GENERATE)
         if status == ERROR:
             raise Exception("Synth Failed")
         self.datasource_id = self.get_flow()[TARGET_DATASOURCE_ID]
 
+    def list_tables(self):
+        return self.dato_trainer.dato_mapper.schema.tables_name()
+
     def get_generated_data(self) -> None:
         self.restore_validation()
         print(get_generated_zip(datomizer=self.dato_trainer.dato_mapper.datomizer,
                                 business_unit_id=self.dato_trainer.dato_mapper.business_unit_id,
                                 project_id=self.dato_trainer.dato_mapper.project_id,
                                 flow_id=self.synth_id))
```

### Comparing `datomize-2.1.7/datomizer/datomapper.py` & `datomize-2.3.7/datomizer/datomapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from datomizer import Datomizer
 from datomizer.helpers.datasource.datasource_helper import create_origin_private_datasource_from_path, save_df_to_csv, validate_data_size_limits
 from datomizer.helpers.common_helper import get_flow, wait_for_step_type
 from datomizer.helpers.business_unit_project.business_unit_project_helper import get_default_business_unit_project
 from datomizer.helpers.autodiscovery.autodiscovery_helper import discover, get_schema_discovery, put_schema_discovery
 from datomizer.helpers.wrapper.schema_wrapper import SchemaWrapper
 from datomizer.utils.general import ORIGIN_DATASOURCE_ID, ERROR
+from datomizer.utils.interfaces import DatoCommonInterface
 from datomizer.utils.step_types import COLUMN_DISCOVERY
 
 
-class DatoMapper(object):
+class DatoMapper(DatoCommonInterface):
     datomizer: Datomizer
     business_unit_id = 0
     project_id = 0
     datasource_id = 0
     flow_id = 0
     schema: SchemaWrapper = None
 
@@ -93,14 +94,17 @@
             Datomize mapping dictionary"""
         self.restore_validation()
         self.schema = SchemaWrapper(put_schema_discovery(self.datomizer,
                                                          self.business_unit_id, self.project_id, self.flow_id,
                                                          self.schema.schema))
         return self.schema
 
+    def list_tables(self):
+        return self.schema.tables_name()
+
     def base_validation(self):
         assert (self.business_unit_id > 0 and self.project_id > 0), "missing base properties"
 
     def set_datasource_validation(self):
         self.base_validation()
         assert self.datasource_id == 0, "datasource id cannot be mutated"
```

### Comparing `datomize-2.1.7/datomizer/datomizer.py` & `datomize-2.3.7/datomizer/datomizer.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/datomizer/datotrainer.py` & `datomize-2.3.7/datomizer/datotrainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import io
 
 from datomizer import DatoMapper
 from datomizer.helpers.common_helper import wait_for_step_type, get_generated_zip, get_generated_csv
 from datomizer.helpers.train.train_helper import train, get_train_iteration, get_evaluation
 from datomizer.helpers.wrapper.evaluation_wrapper import EvaluationWrapper
 from datomizer.utils.general import ID, MODELS, ERROR
+from datomizer.utils.interfaces import DatoGenInterface
 from datomizer.utils.step_types import TRAIN_AND_GENERATE
 
 
-class DatoTrainer(object):
+class DatoTrainer(DatoGenInterface):
     dato_mapper: DatoMapper
     train_id = 0
     model_id = 0
 
     def __init__(self, dato_mapper: DatoMapper):
         """Create DatoTrainer object for training a generative model for the mapped input data.
         Args:
@@ -49,14 +50,17 @@
                                     flow_id=self.dato_mapper.flow_id,
                                     step_type=TRAIN_AND_GENERATE,
                                     train_id=self.train_id)
         if status == ERROR:
             raise Exception("Trainer Failed")
         self.model_id = get_train_iteration(self.dato_mapper, self.train_id)[MODELS][0][ID]
 
+    def list_tables(self):
+        return self.dato_mapper.schema.tables_name()
+
     def get_generated_data(self) -> None:
         self.next_step_validation()
         print(get_generated_zip(datomizer=self.dato_mapper.datomizer,
                                 business_unit_id=self.dato_mapper.business_unit_id,
                                 project_id=self.dato_mapper.project_id,
                                 flow_id=self.dato_mapper.flow_id,
                                 train_id=self.train_id,
```

### Comparing `datomize-2.1.7/datomizer/datotuner.py` & `datomize-2.3.7/datomizer/datotuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import io
 
 from datomizer import DatoMapper
 from datomizer.helpers.common_helper import wait_for_step_type, get_generated_zip, get_generated_csv
 from datomizer.helpers.train import datatuner_helper, train_helper
 from datomizer.utils.general import ID, MODELS, ERROR
+from datomizer.utils.interfaces import DatoGenInterface
 from datomizer.utils.step_types import DT_TRAIN_AND_GENERATE
 from datomizer.protos.datatunerservice_pb2 import DataTunerDTO
 
 
-class DatoTuner(object):
+class DatoTuner(DatoGenInterface):
     dato_mapper: DatoMapper
     train_id = 0
     model_id = 0
 
     def __init__(self, dato_mapper: DatoMapper):
         """Create DatoTuner object for training a tuned model for the mapped input data.
         Args:
@@ -48,14 +49,17 @@
                                     flow_id=self.dato_mapper.flow_id,
                                     step_type=DT_TRAIN_AND_GENERATE,
                                     train_id=self.train_id)
         if status == ERROR:
             raise Exception("Trainer Failed")
         self.model_id = train_helper.get_train_iteration(self.dato_mapper, self.train_id)[MODELS][0][ID]
 
+    def list_tables(self):
+        return self.dato_mapper.schema.tables_name()
+
     def get_generated_data(self) -> None:
         self.next_step_validation()
         print(get_generated_zip(datomizer=self.dato_mapper.datomizer,
                                 business_unit_id=self.dato_mapper.business_unit_id,
                                 project_id=self.dato_mapper.project_id,
                                 flow_id=self.dato_mapper.flow_id,
                                 train_id=self.train_id,
```

### Comparing `datomize-2.1.7/datomizer/helpers/authentication/authentication_helper.py` & `datomize-2.3.7/datomizer/helpers/authentication/authentication_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/datomizer/helpers/autodiscovery/autodiscovery_helper.py` & `datomize-2.3.7/datomizer/helpers/autodiscovery/autodiscovery_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/datomizer/helpers/business_unit_project/business_unit_project_helper.py` & `datomize-2.3.7/datomizer/helpers/business_unit_project/business_unit_project_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/datomizer/helpers/common_helper.py` & `datomize-2.3.7/datomizer/helpers/common_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/datomizer/helpers/datasource/datasource_helper.py` & `datomize-2.3.7/datomizer/helpers/datasource/datasource_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/datomizer/helpers/generator/generator_helper.py` & `datomize-2.3.7/datomizer/helpers/generator/generator_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/datomizer/helpers/train/datatuner_helper.py` & `datomize-2.3.7/datomizer/helpers/train/datatuner_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/datomizer/helpers/train/enhance_ml_helper.py` & `datomize-2.3.7/datomizer/helpers/train/enhance_ml_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,27 +7,19 @@
 
 DEFAULT_ALGORITHMS = [Algorithms.RANDOM_FOREST,
                       Algorithms.GBM,
                       Algorithms.KNN,
                       Algorithms.LR,
                       Algorithms.LGBM,
                       Algorithms.XGBOOST]
-DEFAULT_METRICS = [Metrics.F1,
-                   Metrics.PR_AUC]
+DEFAULT_METRIC = Metrics.F1
 
 
 def create_enhance_ml_request(target_table, target_column,
                               metric_list=[], algorithm_list=[]) -> dict:
-    if not metric_list:
-        metric_list = DEFAULT_METRICS
-    if not algorithm_list:
-        algorithm_list = DEFAULT_ALGORITHMS
-
-    metric_list = map_enum_list(metric_list)
-    algorithm_list = map_enum_list(algorithm_list)
 
     return {"tableName": target_table, "targetColumn": target_column,
             "metricList": metric_list, "algorithmList": algorithm_list}
 
 
 def enhance_ml_generate(dato_mapper: DatoMapper, target_table, target_column, metric_list=[], algorithm_list=[]) -> int:
     dato_mapper.wait()
```

### Comparing `datomize-2.1.7/datomizer/helpers/train/train_helper.py` & `datomize-2.3.7/datomizer/helpers/train/train_helper.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/datomizer/protos/autodiscoveryservice_pb2.py` & `datomize-2.3.7/datomizer/protos/datatunerservice_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,274 +1,311 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: autodiscoveryservice.proto
+# source: datatunerservice.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x61utodiscoveryservice.proto\x12\x08\x64\x61takube\"\x95\x02\n\x12SchemaDiscoveryDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\"\n\x06tables\x18\x02 \x03(\x0b\x32\x12.datakube.TableDTO\x12-\n\x0c\x64\x65pendencies\x18\x03 \x03(\x0b\x32\x17.datakube.DependencyDTO\x12\x16\n\x0enumberOfTables\x18\x04 \x01(\x05\x12\x17\n\x0fnumberOfRecords\x18\x05 \x01(\x03\x12\x17\n\x0fnumberOfColumns\x18\x06 \x01(\x05\x12\x10\n\x08\x64\x61taSize\x18\x07 \x01(\x02\x12\x1c\n\x14numberOfDependencies\x18\x08 \x01(\x05\x12\x13\n\x0bisValidated\x18\t \x01(\x08\x12\x0f\n\x07version\x18\x63 \x01(\t\"\xc0\x04\n\x08TableDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x04\x12$\n\x07\x63olumns\x18\x03 \x03(\x0b\x32\x13.datakube.ColumnDTO\x12\x0f\n\x07isFixed\x18\x05 \x01(\x08\x12\x31\n\nsequential\x18\x06 \x01(\x0b\x32\x1d.datakube.TableDTO.Sequential\x12!\n\nprimaryKey\x18\x07 \x01(\x0b\x32\r.datakube.Key\x12\"\n\x0b\x66oreignKeys\x18\x08 \x03(\x0b\x32\r.datakube.Key\x12(\n\nCandidates\x18\n \x01(\x0b\x32\x14.datakube.Candidates\x12.\n\rmappingConfig\x18\x0b \x01(\x0b\x32\x17.datakube.MappingConfig\x12\x10\n\x08\x45ntities\x18\x0c \x03(\r\x12\x10\n\x08\x64\x61taSize\x18\r \x01(\x02\x1a\xa9\x01\n\nSequential\x12\x35\n\x0cisSequential\x18\x01 \x01(\x0e\x32\x1f.datakube.TableDTO.IsSequential\x12+\n\x0esequenceSource\x18\x02 \x01(\x0e\x32\x13.datakube.KeySource\x12\x0f\n\x07groupBy\x18\x03 \x03(\t\x12\x0e\n\x06sortBy\x18\x04 \x03(\t\x12\x16\n\x0esequenceLength\x18\x05 \x01(\x02\"=\n\x0cIsSequential\x12\x06\n\x02NO\x10\x00\x12\x07\n\x03YES\x10\x01\x12\r\n\tSUSPECTED\x10\x02\x12\r\n\tNOT_VALID\x10\x03\"\x8f\x01\n\nCandidates\x12*\n\nprimaryKey\x18\x01 \x03(\x0b\x32\x16.datakube.CandidateKey\x12+\n\x0b\x66oreignKeys\x18\x02 \x03(\x0b\x32\x16.datakube.CandidateKey\x12(\n\x0c\x65rrorSummery\x18\x62 \x03(\x0b\x32\x12.datakube.ErrorDTO\"E\n\rMappingConfig\x12\x1c\n\x14shouldMaskIdentifier\x18\x01 \x01(\x08\x12\x16\n\x0eshouldMaskText\x18\x02 \x01(\x08\"E\n\x0c\x43\x61ndidateKey\x12\x12\n\ncolumnName\x18\x01 \x03(\t\x12!\n\x05state\x18\x02 \x01(\x0b\x32\x12.datakube.StateDTO\"M\n\x03Key\x12\r\n\x05keyId\x18\x01 \x01(\r\x12\x12\n\ncolumnName\x18\x02 \x03(\t\x12#\n\x06source\x18\x03 \x01(\x0e\x32\x13.datakube.KeySource\"\xb8\x04\n\tColumnDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07rawType\x18\x02 \x01(\t\x12\x13\n\x0buniqueCount\x18\x04 \x01(\x04\x12\x14\n\x0cnotNullCount\x18\x05 \x01(\x04\x12\x11\n\tminDigits\x18\x06 \x01(\x04\x12\x11\n\tmaxDigits\x18\x07 \x01(\x04\x12\x17\n\x0fisRunningNumber\x18\x08 \x01(\x08\x12\x10\n\x08minValue\x18\t \x01(\t\x12\x10\n\x08maxValue\x18\n \x01(\t\x12\x0f\n\x07isFixed\x18\x0b \x01(\x08\x12\x16\n\x0e\x61vailableRoles\x18\x0c \x03(\t\x12\x0c\n\x04role\x18\r \x01(\t\x12\x0f\n\x07\x66ormats\x18\x0e \x03(\t\x12\x14\n\x0cinferredType\x18\x0f \x01(\t\x12+\n\nstatistics\x18\x10 \x01(\x0b\x32\x17.datakube.StatisticsDTO\x12!\n\x05state\x18\x11 \x01(\x0b\x32\x12.datakube.StateDTO\x12\x13\n\x0bisSupported\x18\x12 \x01(\x08\x12\r\n\x05train\x18\x13 \x01(\x08\x12\x16\n\x0e\x61vailableTypes\x18\x14 \x03(\t\x12\x15\n\rfloatPercison\x18\x15 \x01(\x04\x12\x10\n\x08\x45ntityID\x18\x16 \x01(\r\x12/\n\x0c\x63ustomParams\x18\x17 \x01(\x0b\x32\x19.datakube.CustomParamsDTO\x12\x10\n\x08isIgnore\x18\x18 \x01(\x08\x12(\n\x0c\x65rrorSummery\x18\x62 \x03(\x0b\x32\x12.datakube.ErrorDTO\"[\n\x08StateDTO\x12\x1f\n\x06status\x18\x01 \x01(\x0e\x32\x0f.datakube.State\x12.\n\rchangedFields\x18\x02 \x03(\x0e\x32\x17.datakube.MutableFields\"\xd6\x01\n\rDependencyDTO\x12#\n\x04left\x18\x01 \x01(\x0b\x32\x15.datakube.TableRefDTO\x12$\n\x05right\x18\x02 \x01(\x0b\x32\x15.datakube.TableRefDTO\x12-\n\x10\x64\x65pendencySource\x18\x03 \x01(\x0e\x32\x13.datakube.KeySource\x12!\n\x05state\x18\x04 \x01(\x0b\x32\x12.datakube.StateDTO\x12(\n\x0c\x65rrorSummery\x18\x62 \x03(\x0b\x32\x12.datakube.ErrorDTO\"\x95\x03\n\x0bTableRefDTO\x12\x11\n\ttableName\x18\x01 \x01(\t\x12\r\n\x05keyId\x18\x02 \x01(\r\x12.\n\x07keyType\x18\x03 \x01(\x0e\x32\x1d.datakube.TableRefDTO.KeyType\x12>\n\x0f\x63\x61rdinalityType\x18\x04 \x01(\x0e\x32%.datakube.TableRefDTO.CardinalityType\x12@\n\x10relationshipType\x18\x05 \x01(\x0e\x32&.datakube.TableRefDTO.RelationshipType\"3\n\x07KeyType\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02PK\x10\x01\x12\x06\n\x02\x46K\x10\x02\x12\x0e\n\nComposedPK\x10\x03\"4\n\x0f\x43\x61rdinalityType\x12\x07\n\x03One\x10\x00\x12\x08\n\x04Many\x10\x01\x12\x0e\n\nUnassigned\x10\x03\"G\n\x10RelationshipType\x12\t\n\x05\x45qual\x10\x00\x12\x0b\n\x07Overlap\x10\x01\x12\x0c\n\x08\x43ontains\x10\x02\x12\r\n\tContained\x10\x03\"G\n\x08\x45rrorDTO\x12(\n\nerrorState\x18\x01 \x01(\x0e\x32\x14.datakube.ErrorState\x12\x11\n\terrorInfo\x18\x02 \x01(\t\"\x9d\x01\n\rStatisticsDTO\x12\x17\n\x0ftypeConsistency\x18\x01 \x01(\x02\x12\x14\n\x0c\x61verageValue\x18\x02 \x01(\x02\x12\x19\n\x11standardDeviation\x18\x03 \x01(\x02\x12\x0f\n\x07\x65ntropy\x18\x04 \x01(\x02\x12\x31\n\rtypeRoleScore\x18\x05 \x03(\x0b\x32\x1a.datakube.TypeRoleScoreDTO\"d\n\x10TypeRoleScoreDTO\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x17\n\x0ftypeConsistency\x18\x02 \x01(\x02\x12)\n\troleScore\x18\x03 \x03(\x0b\x32\x16.datakube.RoleScoreDTO\"+\n\x0cRoleScoreDTO\x12\x0c\n\x04role\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x02\"#\n\x0f\x43ustomParamsDTO\x12\x10\n\x08isFreeze\x18\x01 \x01(\x08\"I\n\x12SchemaHistogramDTO\x12\x33\n\x0etableHistogram\x18\x01 \x03(\x0b\x32\x1b.datakube.TableHistogramDTO\"^\n\x11TableHistogramDTO\x12\x11\n\ttableName\x18\x01 \x01(\t\x12\x36\n\x10\x63olumnsHistogram\x18\x02 \x03(\x0b\x32\x1c.datakube.ColumnHistogramDTO\"r\n\x12\x43olumnHistogramDTO\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12,\n\x07\x65ntries\x18\x02 \x03(\x0b\x32\x1b.datakube.HistogramEntryDTO\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04role\x18\x04 \x01(\t\"A\n\x11HistogramEntryDTO\x12\r\n\x05value\x18\x01 \x01(\t\x12\x0e\n\x06isNull\x18\x02 \x01(\x08\x12\r\n\x05\x63ount\x18\x03 \x01(\x05*M\n\tKeySource\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08METADATA\x10\x01\x12\x0e\n\nDISCOVERED\x10\x02\x12\n\n\x06MANUAL\x10\x03\x12\x0c\n\x08INTERNAL\x10\x04*N\n\x05State\x12\t\n\x05VALID\x10\x00\x12\r\n\tNOT_VALID\x10\x01\x12\x11\n\rUSER_MODIFIED\x10\x02\x12\x18\n\x14MODIFICATION_FAILURE\x10\x03*r\n\rMutableFields\x12\x19\n\x15\x43HANGED_COLUMN_FORMAT\x10\x00\x12\x17\n\x13\x43HANGED_COLUMN_TYPE\x10\x01\x12\x17\n\x13\x43HANGED_COLUMN_ROLE\x10\x02\x12\x14\n\x10\x41\x44\x44\x45\x44_DEPENDENCY\x10\x03*\x88\x01\n\nErrorState\x12\x11\n\rGENERAL_ERROR\x10\x00\x12\x14\n\x10\x43ONNECTION_ERROR\x10\x01\x12\x10\n\x0cMEMORY_ERROR\x10\x02\x12\x1a\n\x16\x41UTHENTICATION_FAILURE\x10\x03\x12\x11\n\rPARSING_ERROR\x10\x04\x12\x10\n\x0cUNKNOWN_TYPE\x10\x05\x42k\nMcom.datomize.datomizer.backend.components.management.dto.autodiscoveryserviceB\x1a\x41utoDiscoveryServiceProtosb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x64\x61tatunerservice.proto\x12\tdatatuner\"7\n\x0c\x44\x61taTunerDTO\x12\'\n\x08ruleSets\x18\x01 \x03(\x0b\x32\x15.datatuner.RuleSetDTO\"B\n\nRuleSetDTO\x12\x11\n\ttableName\x18\x01 \x01(\t\x12!\n\x05rules\x18\x02 \x03(\x0b\x32\x12.datatuner.RuleDTO\"\x80\x01\n\x07RuleDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x13\n\x0boutputRatio\x18\x02 \x01(\x01\x12\x14\n\x0coutputAmount\x18\x03 \x01(\x05\x12%\n\x07\x63lauses\x18\x04 \x03(\x0b\x32\x14.datatuner.ClauseDTO\x12\x17\n\x0fgeneratedAmount\x18\x05 \x01(\x05\"\xe7\x01\n\tClauseDTO\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12<\n\x11\x63\x61tegoricalClause\x18\x14 \x01(\x0b\x32\x1f.datatuner.CategoricalClauseDTOH\x00\x12\x30\n\x0brangeClause\x18\x15 \x01(\x0b\x32\x19.datatuner.RangeClauseDTOH\x00\x12H\n\x17numericNormalDistClause\x18\x16 \x01(\x0b\x32%.datatuner.NumericNormalDistClauseDTOH\x00\x42\x0c\n\nClauseType\"-\n\x14\x43\x61tegoricalClauseDTO\x12\x15\n\rcategoryValue\x18\x01 \x01(\t\"4\n\x0eRangeClauseDTO\x12\x10\n\x08minValue\x18\x01 \x01(\t\x12\x10\n\x08maxValue\x18\x02 \x01(\t\"e\n\x1aNumericNormalDistClauseDTO\x12\x11\n\tmeanValue\x18\x01 \x01(\t\x12\x10\n\x08stdValue\x18\x02 \x01(\t\x12\x10\n\x08minValue\x18\x03 \x01(\t\x12\x10\n\x08maxValue\x18\x04 \x01(\t\"E\n\x11\x44TResultSchemaDTO\x12\x30\n\x0bresultTable\x18\x01 \x03(\x0b\x32\x1b.datatuner.DTResultTableDTO\"\x99\x01\n\x10\x44TResultTableDTO\x12\x11\n\ttableName\x18\x01 \x01(\t\x12)\n\x05rules\x18\x02 \x03(\x0b\x32\x1a.datatuner.DTResultRuleDTO\x12\r\n\x05score\x18\x03 \x01(\x01\x12\x38\n\x0crealMetaData\x18\x04 \x01(\x0b\x32\".datatuner.EffectedColHistMetaData\"\xd1\x03\n\x0f\x44TResultRuleDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x37\n\x0esynthHistogram\x18\x02 \x03(\x0b\x32\x1f.datatuner.DTResultHistogramDTO\x12;\n\x12originalHistograms\x18\x03 \x03(\x0b\x32\x1f.datatuner.DTResultHistogramDTO\x12\r\n\x05score\x18\x04 \x01(\x01\x12\x14\n\x0coutputAmount\x18\x06 \x01(\x05\x12\x44\n\x12numEffectedColHist\x18\x07 \x01(\x0b\x32(.datatuner.DTEffectedColumnsHistogramDTO\x12\x41\n\x0f\x65\x66\x66\x65\x63tedColHist\x18\x08 \x01(\x0b\x32(.datatuner.DTEffectedColumnsHistogramDTO\x12%\n\x07\x63lauses\x18\t \x03(\x0b\x32\x14.datatuner.ClauseDTO\x12<\n\x12ifColumnHypothesis\x18\n \x03(\x0b\x32 .datatuner.IfColumnHypothesisDTO\x12\x13\n\x0bwhatColumns\x18\x0b \x03(\t\x12\x14\n\x0cgivenColumns\x18\x0c \x03(\t\"\x80\x01\n\x14\x44TResultHistogramDTO\x12\x32\n\thistogram\x18\x01 \x03(\x0b\x32\x1f.datatuner.DTColumnHistogramDTO\x12\r\n\x05score\x18\x02 \x01(\x01\x12%\n\x07\x63lauses\x18\x03 \x03(\x0b\x32\x14.datatuner.ClauseDTO\"e\n\x14\x44TColumnHistogramDTO\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12\x13\n\x0bxTickLabels\x18\x02 \x03(\t\x12\r\n\x05yData\x18\x03 \x03(\x01\x12\x15\n\risCategorical\x18\x04 \x01(\x08\"y\n\x1d\x44TEffectedColumnsHistogramDTO\x12\x10\n\x08xColName\x18\x01 \x03(\t\x12\r\n\x05yData\x18\x02 \x03(\x01\x12\x37\n\x0bsynMetaData\x18\x07 \x01(\x0b\x32\".datatuner.EffectedColHistMetaData\"\x87\x01\n\x17\x45\x66\x66\x65\x63tedColHistMetaData\x12\x13\n\x0b\x63olumnNames\x18\x01 \x03(\t\x12\x0c\n\x04mean\x18\x02 \x03(\x01\x12\x0b\n\x03std\x18\x03 \x03(\x01\x12\x0b\n\x03min\x18\x04 \x03(\x01\x12\x0b\n\x03max\x18\x05 \x03(\x01\x12\n\n\x02q1\x18\x06 \x03(\x01\x12\n\n\x02q2\x18\x07 \x03(\x01\x12\n\n\x02q3\x18\x08 \x03(\x01\"D\n\x0eWhatIfTunerDTO\x12\x32\n\rhypothesisSet\x18\x01 \x03(\x0b\x32\x1b.datatuner.HypothesisSetDTO\"\x80\x01\n\x10HypothesisSetDTO\x12\x11\n\ttableName\x18\x01 \x01(\t\x12\x14\n\x0cgivenColumns\x18\x02 \x03(\t\x12\x13\n\x0bwhatColumns\x18\x03 \x03(\t\x12.\n\nhypothesis\x18\x04 \x03(\x0b\x32\x1a.datatuner.IfHypothesisDTO\"t\n\x0fIfHypothesisDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12<\n\x12ifColumnHypothesis\x18\x02 \x03(\x0b\x32 .datatuner.IfColumnHypothesisDTO\x12\x17\n\x0fgeneratedAmount\x18\x03 \x01(\x05\"\x93\x03\n\x15IfColumnHypothesisDTO\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12J\n\x18\x63\x61tegoricalMapHypothesis\x18\x14 \x01(\x0b\x32&.datatuner.CategoricalHypothesisMapDTOH\x00\x12N\n\x1a\x63\x61tegoricalConstHypothesis\x18\x15 \x01(\x0b\x32(.datatuner.CategoricalHypothesisConstDTOH\x00\x12>\n\x11numericHypothesis\x18\x16 \x01(\x0b\x32!.datatuner.NumericalHypothesisDTOH\x00\x12\x36\n\x0e\x64\x61teHypothesis\x18\x17 \x01(\x0b\x32\x1c.datatuner.DateHypothesisDTOH\x00\x12@\n\x13\x64\x61teConstHypothesis\x18\x18 \x01(\x0b\x32!.datatuner.DateConstHypothesisDTOH\x00\x42\x10\n\x0eHypothesisType\".\n\x1d\x43\x61tegoricalHypothesisConstDTO\x12\r\n\x05value\x18\x01 \x01(\t\"M\n\x1b\x43\x61tegoricalHypothesisMapDTO\x12.\n\x0b\x63\x61tegoryMap\x18\x01 \x03(\x0b\x32\x19.datatuner.CategoryMapDTO\"I\n\x0e\x43\x61tegoryMapDTO\x12\x1d\n\x15originalCategoryValue\x18\x01 \x01(\t\x12\x18\n\x10newCategoryValue\x18\x02 \x01(\t\"}\n\x16NumericalHypothesisDTO\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x30\n\tnumericOp\x18\x02 \x01(\x0e\x32\x1d.datatuner.NumericalOperation\x12\x10\n\x08minValue\x18\x03 \x01(\x01\x12\x10\n\x08maxValue\x18\x04 \x01(\x01\";\n\x11\x44\x61teHypothesisDTO\x12&\n\x07\x64\x61teMap\x18\x01 \x03(\x0b\x32\x15.datatuner.DateMapDTO\"B\n\nDateMapDTO\x12\r\n\x05value\x18\x01 \x01(\x01\x12%\n\x08\x64\x61teUnit\x18\x02 \x01(\x0e\x32\x13.datatuner.DateUnit\"\'\n\x16\x44\x61teConstHypothesisDTO\x12\r\n\x05value\x18\x01 \x01(\t\"[\n\x17TunerGroupsHistogramDTO\x12\x0c\n\x04\x63ols\x18\x01 \x03(\t\x12\x32\n\x07\x65ntries\x18\x02 \x03(\x0b\x32!.datatuner.TunerHistogramEntryDTO\"Q\n\x16TunerHistogramEntryDTO\x12\x0e\n\x06values\x18\x01 \x03(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\x12\x18\n\x10\x63ount_percentage\x18\x03 \x01(\x01*D\n\x12NumericalOperation\x12\x0c\n\x08\x41\x44\x44ITION\x10\x00\x12\x12\n\x0eMULTIPLICATION\x10\x01\x12\x0c\n\x08\x43ONSTANT\x10\x02*9\n\x08\x44\x61teUnit\x12\x08\n\x04\x44\x41YS\x10\x00\x12\t\n\x05HOURS\x10\x01\x12\x0b\n\x07MINUTES\x10\x02\x12\x0b\n\x07SECONDS\x10\x03\x42\x63\nIcom.datomize.datomizer.backend.components.management.dto.datatunerserviceB\x16\x44\x61taTunerServiceProtosb\x06proto3')
 
-_KEYSOURCE = DESCRIPTOR.enum_types_by_name['KeySource']
-KeySource = enum_type_wrapper.EnumTypeWrapper(_KEYSOURCE)
-_STATE = DESCRIPTOR.enum_types_by_name['State']
-State = enum_type_wrapper.EnumTypeWrapper(_STATE)
-_MUTABLEFIELDS = DESCRIPTOR.enum_types_by_name['MutableFields']
-MutableFields = enum_type_wrapper.EnumTypeWrapper(_MUTABLEFIELDS)
-_ERRORSTATE = DESCRIPTOR.enum_types_by_name['ErrorState']
-ErrorState = enum_type_wrapper.EnumTypeWrapper(_ERRORSTATE)
-NONE = 0
-METADATA = 1
-DISCOVERED = 2
-MANUAL = 3
-INTERNAL = 4
-VALID = 0
-NOT_VALID = 1
-USER_MODIFIED = 2
-MODIFICATION_FAILURE = 3
-CHANGED_COLUMN_FORMAT = 0
-CHANGED_COLUMN_TYPE = 1
-CHANGED_COLUMN_ROLE = 2
-ADDED_DEPENDENCY = 3
-GENERAL_ERROR = 0
-CONNECTION_ERROR = 1
-MEMORY_ERROR = 2
-AUTHENTICATION_FAILURE = 3
-PARSING_ERROR = 4
-UNKNOWN_TYPE = 5
-
-
-_SCHEMADISCOVERYDTO = DESCRIPTOR.message_types_by_name['SchemaDiscoveryDTO']
-_TABLEDTO = DESCRIPTOR.message_types_by_name['TableDTO']
-_TABLEDTO_SEQUENTIAL = _TABLEDTO.nested_types_by_name['Sequential']
-_CANDIDATES = DESCRIPTOR.message_types_by_name['Candidates']
-_MAPPINGCONFIG = DESCRIPTOR.message_types_by_name['MappingConfig']
-_CANDIDATEKEY = DESCRIPTOR.message_types_by_name['CandidateKey']
-_KEY = DESCRIPTOR.message_types_by_name['Key']
-_COLUMNDTO = DESCRIPTOR.message_types_by_name['ColumnDTO']
-_STATEDTO = DESCRIPTOR.message_types_by_name['StateDTO']
-_DEPENDENCYDTO = DESCRIPTOR.message_types_by_name['DependencyDTO']
-_TABLEREFDTO = DESCRIPTOR.message_types_by_name['TableRefDTO']
-_ERRORDTO = DESCRIPTOR.message_types_by_name['ErrorDTO']
-_STATISTICSDTO = DESCRIPTOR.message_types_by_name['StatisticsDTO']
-_TYPEROLESCOREDTO = DESCRIPTOR.message_types_by_name['TypeRoleScoreDTO']
-_ROLESCOREDTO = DESCRIPTOR.message_types_by_name['RoleScoreDTO']
-_CUSTOMPARAMSDTO = DESCRIPTOR.message_types_by_name['CustomParamsDTO']
-_SCHEMAHISTOGRAMDTO = DESCRIPTOR.message_types_by_name['SchemaHistogramDTO']
-_TABLEHISTOGRAMDTO = DESCRIPTOR.message_types_by_name['TableHistogramDTO']
-_COLUMNHISTOGRAMDTO = DESCRIPTOR.message_types_by_name['ColumnHistogramDTO']
-_HISTOGRAMENTRYDTO = DESCRIPTOR.message_types_by_name['HistogramEntryDTO']
-_TABLEDTO_ISSEQUENTIAL = _TABLEDTO.enum_types_by_name['IsSequential']
-_TABLEREFDTO_KEYTYPE = _TABLEREFDTO.enum_types_by_name['KeyType']
-_TABLEREFDTO_CARDINALITYTYPE = _TABLEREFDTO.enum_types_by_name['CardinalityType']
-_TABLEREFDTO_RELATIONSHIPTYPE = _TABLEREFDTO.enum_types_by_name['RelationshipType']
-SchemaDiscoveryDTO = _reflection.GeneratedProtocolMessageType('SchemaDiscoveryDTO', (_message.Message,), {
-  'DESCRIPTOR' : _SCHEMADISCOVERYDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.SchemaDiscoveryDTO)
-  })
-_sym_db.RegisterMessage(SchemaDiscoveryDTO)
-
-TableDTO = _reflection.GeneratedProtocolMessageType('TableDTO', (_message.Message,), {
-
-  'Sequential' : _reflection.GeneratedProtocolMessageType('Sequential', (_message.Message,), {
-    'DESCRIPTOR' : _TABLEDTO_SEQUENTIAL,
-    '__module__' : 'autodiscoveryservice_pb2'
-    # @@protoc_insertion_point(class_scope:datakube.TableDTO.Sequential)
-    })
-  ,
-  'DESCRIPTOR' : _TABLEDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.TableDTO)
-  })
-_sym_db.RegisterMessage(TableDTO)
-_sym_db.RegisterMessage(TableDTO.Sequential)
-
-Candidates = _reflection.GeneratedProtocolMessageType('Candidates', (_message.Message,), {
-  'DESCRIPTOR' : _CANDIDATES,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.Candidates)
-  })
-_sym_db.RegisterMessage(Candidates)
-
-MappingConfig = _reflection.GeneratedProtocolMessageType('MappingConfig', (_message.Message,), {
-  'DESCRIPTOR' : _MAPPINGCONFIG,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.MappingConfig)
-  })
-_sym_db.RegisterMessage(MappingConfig)
-
-CandidateKey = _reflection.GeneratedProtocolMessageType('CandidateKey', (_message.Message,), {
-  'DESCRIPTOR' : _CANDIDATEKEY,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.CandidateKey)
-  })
-_sym_db.RegisterMessage(CandidateKey)
-
-Key = _reflection.GeneratedProtocolMessageType('Key', (_message.Message,), {
-  'DESCRIPTOR' : _KEY,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.Key)
-  })
-_sym_db.RegisterMessage(Key)
-
-ColumnDTO = _reflection.GeneratedProtocolMessageType('ColumnDTO', (_message.Message,), {
-  'DESCRIPTOR' : _COLUMNDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.ColumnDTO)
-  })
-_sym_db.RegisterMessage(ColumnDTO)
-
-StateDTO = _reflection.GeneratedProtocolMessageType('StateDTO', (_message.Message,), {
-  'DESCRIPTOR' : _STATEDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.StateDTO)
-  })
-_sym_db.RegisterMessage(StateDTO)
-
-DependencyDTO = _reflection.GeneratedProtocolMessageType('DependencyDTO', (_message.Message,), {
-  'DESCRIPTOR' : _DEPENDENCYDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.DependencyDTO)
-  })
-_sym_db.RegisterMessage(DependencyDTO)
-
-TableRefDTO = _reflection.GeneratedProtocolMessageType('TableRefDTO', (_message.Message,), {
-  'DESCRIPTOR' : _TABLEREFDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.TableRefDTO)
-  })
-_sym_db.RegisterMessage(TableRefDTO)
-
-ErrorDTO = _reflection.GeneratedProtocolMessageType('ErrorDTO', (_message.Message,), {
-  'DESCRIPTOR' : _ERRORDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.ErrorDTO)
-  })
-_sym_db.RegisterMessage(ErrorDTO)
-
-StatisticsDTO = _reflection.GeneratedProtocolMessageType('StatisticsDTO', (_message.Message,), {
-  'DESCRIPTOR' : _STATISTICSDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.StatisticsDTO)
-  })
-_sym_db.RegisterMessage(StatisticsDTO)
-
-TypeRoleScoreDTO = _reflection.GeneratedProtocolMessageType('TypeRoleScoreDTO', (_message.Message,), {
-  'DESCRIPTOR' : _TYPEROLESCOREDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.TypeRoleScoreDTO)
-  })
-_sym_db.RegisterMessage(TypeRoleScoreDTO)
-
-RoleScoreDTO = _reflection.GeneratedProtocolMessageType('RoleScoreDTO', (_message.Message,), {
-  'DESCRIPTOR' : _ROLESCOREDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.RoleScoreDTO)
-  })
-_sym_db.RegisterMessage(RoleScoreDTO)
-
-CustomParamsDTO = _reflection.GeneratedProtocolMessageType('CustomParamsDTO', (_message.Message,), {
-  'DESCRIPTOR' : _CUSTOMPARAMSDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.CustomParamsDTO)
-  })
-_sym_db.RegisterMessage(CustomParamsDTO)
-
-SchemaHistogramDTO = _reflection.GeneratedProtocolMessageType('SchemaHistogramDTO', (_message.Message,), {
-  'DESCRIPTOR' : _SCHEMAHISTOGRAMDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.SchemaHistogramDTO)
-  })
-_sym_db.RegisterMessage(SchemaHistogramDTO)
-
-TableHistogramDTO = _reflection.GeneratedProtocolMessageType('TableHistogramDTO', (_message.Message,), {
-  'DESCRIPTOR' : _TABLEHISTOGRAMDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.TableHistogramDTO)
-  })
-_sym_db.RegisterMessage(TableHistogramDTO)
-
-ColumnHistogramDTO = _reflection.GeneratedProtocolMessageType('ColumnHistogramDTO', (_message.Message,), {
-  'DESCRIPTOR' : _COLUMNHISTOGRAMDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.ColumnHistogramDTO)
-  })
-_sym_db.RegisterMessage(ColumnHistogramDTO)
-
-HistogramEntryDTO = _reflection.GeneratedProtocolMessageType('HistogramEntryDTO', (_message.Message,), {
-  'DESCRIPTOR' : _HISTOGRAMENTRYDTO,
-  '__module__' : 'autodiscoveryservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.HistogramEntryDTO)
+_NUMERICALOPERATION = DESCRIPTOR.enum_types_by_name['NumericalOperation']
+NumericalOperation = enum_type_wrapper.EnumTypeWrapper(_NUMERICALOPERATION)
+_DATEUNIT = DESCRIPTOR.enum_types_by_name['DateUnit']
+DateUnit = enum_type_wrapper.EnumTypeWrapper(_DATEUNIT)
+ADDITION = 0
+MULTIPLICATION = 1
+CONSTANT = 2
+DAYS = 0
+HOURS = 1
+MINUTES = 2
+SECONDS = 3
+
+
+_DATATUNERDTO = DESCRIPTOR.message_types_by_name['DataTunerDTO']
+_RULESETDTO = DESCRIPTOR.message_types_by_name['RuleSetDTO']
+_RULEDTO = DESCRIPTOR.message_types_by_name['RuleDTO']
+_CLAUSEDTO = DESCRIPTOR.message_types_by_name['ClauseDTO']
+_CATEGORICALCLAUSEDTO = DESCRIPTOR.message_types_by_name['CategoricalClauseDTO']
+_RANGECLAUSEDTO = DESCRIPTOR.message_types_by_name['RangeClauseDTO']
+_NUMERICNORMALDISTCLAUSEDTO = DESCRIPTOR.message_types_by_name['NumericNormalDistClauseDTO']
+_DTRESULTSCHEMADTO = DESCRIPTOR.message_types_by_name['DTResultSchemaDTO']
+_DTRESULTTABLEDTO = DESCRIPTOR.message_types_by_name['DTResultTableDTO']
+_DTRESULTRULEDTO = DESCRIPTOR.message_types_by_name['DTResultRuleDTO']
+_DTRESULTHISTOGRAMDTO = DESCRIPTOR.message_types_by_name['DTResultHistogramDTO']
+_DTCOLUMNHISTOGRAMDTO = DESCRIPTOR.message_types_by_name['DTColumnHistogramDTO']
+_DTEFFECTEDCOLUMNSHISTOGRAMDTO = DESCRIPTOR.message_types_by_name['DTEffectedColumnsHistogramDTO']
+_EFFECTEDCOLHISTMETADATA = DESCRIPTOR.message_types_by_name['EffectedColHistMetaData']
+_WHATIFTUNERDTO = DESCRIPTOR.message_types_by_name['WhatIfTunerDTO']
+_HYPOTHESISSETDTO = DESCRIPTOR.message_types_by_name['HypothesisSetDTO']
+_IFHYPOTHESISDTO = DESCRIPTOR.message_types_by_name['IfHypothesisDTO']
+_IFCOLUMNHYPOTHESISDTO = DESCRIPTOR.message_types_by_name['IfColumnHypothesisDTO']
+_CATEGORICALHYPOTHESISCONSTDTO = DESCRIPTOR.message_types_by_name['CategoricalHypothesisConstDTO']
+_CATEGORICALHYPOTHESISMAPDTO = DESCRIPTOR.message_types_by_name['CategoricalHypothesisMapDTO']
+_CATEGORYMAPDTO = DESCRIPTOR.message_types_by_name['CategoryMapDTO']
+_NUMERICALHYPOTHESISDTO = DESCRIPTOR.message_types_by_name['NumericalHypothesisDTO']
+_DATEHYPOTHESISDTO = DESCRIPTOR.message_types_by_name['DateHypothesisDTO']
+_DATEMAPDTO = DESCRIPTOR.message_types_by_name['DateMapDTO']
+_DATECONSTHYPOTHESISDTO = DESCRIPTOR.message_types_by_name['DateConstHypothesisDTO']
+_TUNERGROUPSHISTOGRAMDTO = DESCRIPTOR.message_types_by_name['TunerGroupsHistogramDTO']
+_TUNERHISTOGRAMENTRYDTO = DESCRIPTOR.message_types_by_name['TunerHistogramEntryDTO']
+DataTunerDTO = _reflection.GeneratedProtocolMessageType('DataTunerDTO', (_message.Message,), {
+  'DESCRIPTOR' : _DATATUNERDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.DataTunerDTO)
+  })
+_sym_db.RegisterMessage(DataTunerDTO)
+
+RuleSetDTO = _reflection.GeneratedProtocolMessageType('RuleSetDTO', (_message.Message,), {
+  'DESCRIPTOR' : _RULESETDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.RuleSetDTO)
+  })
+_sym_db.RegisterMessage(RuleSetDTO)
+
+RuleDTO = _reflection.GeneratedProtocolMessageType('RuleDTO', (_message.Message,), {
+  'DESCRIPTOR' : _RULEDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.RuleDTO)
+  })
+_sym_db.RegisterMessage(RuleDTO)
+
+ClauseDTO = _reflection.GeneratedProtocolMessageType('ClauseDTO', (_message.Message,), {
+  'DESCRIPTOR' : _CLAUSEDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.ClauseDTO)
+  })
+_sym_db.RegisterMessage(ClauseDTO)
+
+CategoricalClauseDTO = _reflection.GeneratedProtocolMessageType('CategoricalClauseDTO', (_message.Message,), {
+  'DESCRIPTOR' : _CATEGORICALCLAUSEDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.CategoricalClauseDTO)
+  })
+_sym_db.RegisterMessage(CategoricalClauseDTO)
+
+RangeClauseDTO = _reflection.GeneratedProtocolMessageType('RangeClauseDTO', (_message.Message,), {
+  'DESCRIPTOR' : _RANGECLAUSEDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.RangeClauseDTO)
+  })
+_sym_db.RegisterMessage(RangeClauseDTO)
+
+NumericNormalDistClauseDTO = _reflection.GeneratedProtocolMessageType('NumericNormalDistClauseDTO', (_message.Message,), {
+  'DESCRIPTOR' : _NUMERICNORMALDISTCLAUSEDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.NumericNormalDistClauseDTO)
+  })
+_sym_db.RegisterMessage(NumericNormalDistClauseDTO)
+
+DTResultSchemaDTO = _reflection.GeneratedProtocolMessageType('DTResultSchemaDTO', (_message.Message,), {
+  'DESCRIPTOR' : _DTRESULTSCHEMADTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.DTResultSchemaDTO)
+  })
+_sym_db.RegisterMessage(DTResultSchemaDTO)
+
+DTResultTableDTO = _reflection.GeneratedProtocolMessageType('DTResultTableDTO', (_message.Message,), {
+  'DESCRIPTOR' : _DTRESULTTABLEDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.DTResultTableDTO)
+  })
+_sym_db.RegisterMessage(DTResultTableDTO)
+
+DTResultRuleDTO = _reflection.GeneratedProtocolMessageType('DTResultRuleDTO', (_message.Message,), {
+  'DESCRIPTOR' : _DTRESULTRULEDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.DTResultRuleDTO)
+  })
+_sym_db.RegisterMessage(DTResultRuleDTO)
+
+DTResultHistogramDTO = _reflection.GeneratedProtocolMessageType('DTResultHistogramDTO', (_message.Message,), {
+  'DESCRIPTOR' : _DTRESULTHISTOGRAMDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.DTResultHistogramDTO)
+  })
+_sym_db.RegisterMessage(DTResultHistogramDTO)
+
+DTColumnHistogramDTO = _reflection.GeneratedProtocolMessageType('DTColumnHistogramDTO', (_message.Message,), {
+  'DESCRIPTOR' : _DTCOLUMNHISTOGRAMDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.DTColumnHistogramDTO)
+  })
+_sym_db.RegisterMessage(DTColumnHistogramDTO)
+
+DTEffectedColumnsHistogramDTO = _reflection.GeneratedProtocolMessageType('DTEffectedColumnsHistogramDTO', (_message.Message,), {
+  'DESCRIPTOR' : _DTEFFECTEDCOLUMNSHISTOGRAMDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.DTEffectedColumnsHistogramDTO)
+  })
+_sym_db.RegisterMessage(DTEffectedColumnsHistogramDTO)
+
+EffectedColHistMetaData = _reflection.GeneratedProtocolMessageType('EffectedColHistMetaData', (_message.Message,), {
+  'DESCRIPTOR' : _EFFECTEDCOLHISTMETADATA,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.EffectedColHistMetaData)
+  })
+_sym_db.RegisterMessage(EffectedColHistMetaData)
+
+WhatIfTunerDTO = _reflection.GeneratedProtocolMessageType('WhatIfTunerDTO', (_message.Message,), {
+  'DESCRIPTOR' : _WHATIFTUNERDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.WhatIfTunerDTO)
+  })
+_sym_db.RegisterMessage(WhatIfTunerDTO)
+
+HypothesisSetDTO = _reflection.GeneratedProtocolMessageType('HypothesisSetDTO', (_message.Message,), {
+  'DESCRIPTOR' : _HYPOTHESISSETDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.HypothesisSetDTO)
+  })
+_sym_db.RegisterMessage(HypothesisSetDTO)
+
+IfHypothesisDTO = _reflection.GeneratedProtocolMessageType('IfHypothesisDTO', (_message.Message,), {
+  'DESCRIPTOR' : _IFHYPOTHESISDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.IfHypothesisDTO)
+  })
+_sym_db.RegisterMessage(IfHypothesisDTO)
+
+IfColumnHypothesisDTO = _reflection.GeneratedProtocolMessageType('IfColumnHypothesisDTO', (_message.Message,), {
+  'DESCRIPTOR' : _IFCOLUMNHYPOTHESISDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.IfColumnHypothesisDTO)
+  })
+_sym_db.RegisterMessage(IfColumnHypothesisDTO)
+
+CategoricalHypothesisConstDTO = _reflection.GeneratedProtocolMessageType('CategoricalHypothesisConstDTO', (_message.Message,), {
+  'DESCRIPTOR' : _CATEGORICALHYPOTHESISCONSTDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.CategoricalHypothesisConstDTO)
+  })
+_sym_db.RegisterMessage(CategoricalHypothesisConstDTO)
+
+CategoricalHypothesisMapDTO = _reflection.GeneratedProtocolMessageType('CategoricalHypothesisMapDTO', (_message.Message,), {
+  'DESCRIPTOR' : _CATEGORICALHYPOTHESISMAPDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.CategoricalHypothesisMapDTO)
+  })
+_sym_db.RegisterMessage(CategoricalHypothesisMapDTO)
+
+CategoryMapDTO = _reflection.GeneratedProtocolMessageType('CategoryMapDTO', (_message.Message,), {
+  'DESCRIPTOR' : _CATEGORYMAPDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.CategoryMapDTO)
+  })
+_sym_db.RegisterMessage(CategoryMapDTO)
+
+NumericalHypothesisDTO = _reflection.GeneratedProtocolMessageType('NumericalHypothesisDTO', (_message.Message,), {
+  'DESCRIPTOR' : _NUMERICALHYPOTHESISDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.NumericalHypothesisDTO)
+  })
+_sym_db.RegisterMessage(NumericalHypothesisDTO)
+
+DateHypothesisDTO = _reflection.GeneratedProtocolMessageType('DateHypothesisDTO', (_message.Message,), {
+  'DESCRIPTOR' : _DATEHYPOTHESISDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.DateHypothesisDTO)
+  })
+_sym_db.RegisterMessage(DateHypothesisDTO)
+
+DateMapDTO = _reflection.GeneratedProtocolMessageType('DateMapDTO', (_message.Message,), {
+  'DESCRIPTOR' : _DATEMAPDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.DateMapDTO)
+  })
+_sym_db.RegisterMessage(DateMapDTO)
+
+DateConstHypothesisDTO = _reflection.GeneratedProtocolMessageType('DateConstHypothesisDTO', (_message.Message,), {
+  'DESCRIPTOR' : _DATECONSTHYPOTHESISDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.DateConstHypothesisDTO)
+  })
+_sym_db.RegisterMessage(DateConstHypothesisDTO)
+
+TunerGroupsHistogramDTO = _reflection.GeneratedProtocolMessageType('TunerGroupsHistogramDTO', (_message.Message,), {
+  'DESCRIPTOR' : _TUNERGROUPSHISTOGRAMDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.TunerGroupsHistogramDTO)
+  })
+_sym_db.RegisterMessage(TunerGroupsHistogramDTO)
+
+TunerHistogramEntryDTO = _reflection.GeneratedProtocolMessageType('TunerHistogramEntryDTO', (_message.Message,), {
+  'DESCRIPTOR' : _TUNERHISTOGRAMENTRYDTO,
+  '__module__' : 'datatunerservice_pb2'
+  # @@protoc_insertion_point(class_scope:datatuner.TunerHistogramEntryDTO)
   })
-_sym_db.RegisterMessage(HistogramEntryDTO)
+_sym_db.RegisterMessage(TunerHistogramEntryDTO)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\nMcom.datomize.datomizer.backend.components.management.dto.autodiscoveryserviceB\032AutoDiscoveryServiceProtos'
-  _KEYSOURCE._serialized_start=3326
-  _KEYSOURCE._serialized_end=3403
-  _STATE._serialized_start=3405
-  _STATE._serialized_end=3483
-  _MUTABLEFIELDS._serialized_start=3485
-  _MUTABLEFIELDS._serialized_end=3599
-  _ERRORSTATE._serialized_start=3602
-  _ERRORSTATE._serialized_end=3738
-  _SCHEMADISCOVERYDTO._serialized_start=41
-  _SCHEMADISCOVERYDTO._serialized_end=318
-  _TABLEDTO._serialized_start=321
-  _TABLEDTO._serialized_end=897
-  _TABLEDTO_SEQUENTIAL._serialized_start=665
-  _TABLEDTO_SEQUENTIAL._serialized_end=834
-  _TABLEDTO_ISSEQUENTIAL._serialized_start=836
-  _TABLEDTO_ISSEQUENTIAL._serialized_end=897
-  _CANDIDATES._serialized_start=900
-  _CANDIDATES._serialized_end=1043
-  _MAPPINGCONFIG._serialized_start=1045
-  _MAPPINGCONFIG._serialized_end=1114
-  _CANDIDATEKEY._serialized_start=1116
-  _CANDIDATEKEY._serialized_end=1185
-  _KEY._serialized_start=1187
-  _KEY._serialized_end=1264
-  _COLUMNDTO._serialized_start=1267
-  _COLUMNDTO._serialized_end=1835
-  _STATEDTO._serialized_start=1837
-  _STATEDTO._serialized_end=1928
-  _DEPENDENCYDTO._serialized_start=1931
-  _DEPENDENCYDTO._serialized_end=2145
-  _TABLEREFDTO._serialized_start=2148
-  _TABLEREFDTO._serialized_end=2553
-  _TABLEREFDTO_KEYTYPE._serialized_start=2375
-  _TABLEREFDTO_KEYTYPE._serialized_end=2426
-  _TABLEREFDTO_CARDINALITYTYPE._serialized_start=2428
-  _TABLEREFDTO_CARDINALITYTYPE._serialized_end=2480
-  _TABLEREFDTO_RELATIONSHIPTYPE._serialized_start=2482
-  _TABLEREFDTO_RELATIONSHIPTYPE._serialized_end=2553
-  _ERRORDTO._serialized_start=2555
-  _ERRORDTO._serialized_end=2626
-  _STATISTICSDTO._serialized_start=2629
-  _STATISTICSDTO._serialized_end=2786
-  _TYPEROLESCOREDTO._serialized_start=2788
-  _TYPEROLESCOREDTO._serialized_end=2888
-  _ROLESCOREDTO._serialized_start=2890
-  _ROLESCOREDTO._serialized_end=2933
-  _CUSTOMPARAMSDTO._serialized_start=2935
-  _CUSTOMPARAMSDTO._serialized_end=2970
-  _SCHEMAHISTOGRAMDTO._serialized_start=2972
-  _SCHEMAHISTOGRAMDTO._serialized_end=3045
-  _TABLEHISTOGRAMDTO._serialized_start=3047
-  _TABLEHISTOGRAMDTO._serialized_end=3141
-  _COLUMNHISTOGRAMDTO._serialized_start=3143
-  _COLUMNHISTOGRAMDTO._serialized_end=3257
-  _HISTOGRAMENTRYDTO._serialized_start=3259
-  _HISTOGRAMENTRYDTO._serialized_end=3324
+  DESCRIPTOR._serialized_options = b'\nIcom.datomize.datomizer.backend.components.management.dto.datatunerserviceB\026DataTunerServiceProtos'
+  _NUMERICALOPERATION._serialized_start=3321
+  _NUMERICALOPERATION._serialized_end=3389
+  _DATEUNIT._serialized_start=3391
+  _DATEUNIT._serialized_end=3448
+  _DATATUNERDTO._serialized_start=37
+  _DATATUNERDTO._serialized_end=92
+  _RULESETDTO._serialized_start=94
+  _RULESETDTO._serialized_end=160
+  _RULEDTO._serialized_start=163
+  _RULEDTO._serialized_end=291
+  _CLAUSEDTO._serialized_start=294
+  _CLAUSEDTO._serialized_end=525
+  _CATEGORICALCLAUSEDTO._serialized_start=527
+  _CATEGORICALCLAUSEDTO._serialized_end=572
+  _RANGECLAUSEDTO._serialized_start=574
+  _RANGECLAUSEDTO._serialized_end=626
+  _NUMERICNORMALDISTCLAUSEDTO._serialized_start=628
+  _NUMERICNORMALDISTCLAUSEDTO._serialized_end=729
+  _DTRESULTSCHEMADTO._serialized_start=731
+  _DTRESULTSCHEMADTO._serialized_end=800
+  _DTRESULTTABLEDTO._serialized_start=803
+  _DTRESULTTABLEDTO._serialized_end=956
+  _DTRESULTRULEDTO._serialized_start=959
+  _DTRESULTRULEDTO._serialized_end=1424
+  _DTRESULTHISTOGRAMDTO._serialized_start=1427
+  _DTRESULTHISTOGRAMDTO._serialized_end=1555
+  _DTCOLUMNHISTOGRAMDTO._serialized_start=1557
+  _DTCOLUMNHISTOGRAMDTO._serialized_end=1658
+  _DTEFFECTEDCOLUMNSHISTOGRAMDTO._serialized_start=1660
+  _DTEFFECTEDCOLUMNSHISTOGRAMDTO._serialized_end=1781
+  _EFFECTEDCOLHISTMETADATA._serialized_start=1784
+  _EFFECTEDCOLHISTMETADATA._serialized_end=1919
+  _WHATIFTUNERDTO._serialized_start=1921
+  _WHATIFTUNERDTO._serialized_end=1989
+  _HYPOTHESISSETDTO._serialized_start=1992
+  _HYPOTHESISSETDTO._serialized_end=2120
+  _IFHYPOTHESISDTO._serialized_start=2122
+  _IFHYPOTHESISDTO._serialized_end=2238
+  _IFCOLUMNHYPOTHESISDTO._serialized_start=2241
+  _IFCOLUMNHYPOTHESISDTO._serialized_end=2644
+  _CATEGORICALHYPOTHESISCONSTDTO._serialized_start=2646
+  _CATEGORICALHYPOTHESISCONSTDTO._serialized_end=2692
+  _CATEGORICALHYPOTHESISMAPDTO._serialized_start=2694
+  _CATEGORICALHYPOTHESISMAPDTO._serialized_end=2771
+  _CATEGORYMAPDTO._serialized_start=2773
+  _CATEGORYMAPDTO._serialized_end=2846
+  _NUMERICALHYPOTHESISDTO._serialized_start=2848
+  _NUMERICALHYPOTHESISDTO._serialized_end=2973
+  _DATEHYPOTHESISDTO._serialized_start=2975
+  _DATEHYPOTHESISDTO._serialized_end=3034
+  _DATEMAPDTO._serialized_start=3036
+  _DATEMAPDTO._serialized_end=3102
+  _DATECONSTHYPOTHESISDTO._serialized_start=3104
+  _DATECONSTHYPOTHESISDTO._serialized_end=3143
+  _TUNERGROUPSHISTOGRAMDTO._serialized_start=3145
+  _TUNERGROUPSHISTOGRAMDTO._serialized_end=3236
+  _TUNERHISTOGRAMENTRYDTO._serialized_start=3238
+  _TUNERHISTOGRAMENTRYDTO._serialized_end=3319
 # @@protoc_insertion_point(module_scope)
```

### Comparing `datomize-2.1.7/datomizer/protos/datakubeservice_pb2.py` & `datomize-2.3.7/datomizer/protos/datakubeservice_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x64\x61takubeservice.proto\x12\x08\x64\x61takube\"\xf9\x01\n\x0f\x44\x61taKubeMessage\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\r\n\x05jobId\x18\x02 \x01(\t\x12\x1a\n\x12securityIdentifier\x18\x03 \x01(\t\x12\x38\n\nobjectType\x18\x04 \x01(\x0e\x32$.datakube.DataKubeMessage.ObjectType\x12\x10\n\x08userName\x18\x05 \x01(\t\x12\x0e\n\x06\x66lowId\x18\x06 \x01(\t\"M\n\nObjectType\x12\x18\n\x14\x41\x44\x44_METADATA_MESSAGE\x10\x00\x12\x0e\n\nFINISH_JOB\x10\x01\x12\x15\n\x11SUBTASK_COMPLETED\x10\x02\"\x84\x01\n\x12\x41\x64\x64MetadataMessage\x12=\n\tmap_field\x18\x01 \x03(\x0b\x32*.datakube.AddMetadataMessage.MapFieldEntry\x1a/\n\rMapFieldEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xee\x01\n\tFinishJob\x12\x11\n\texception\x18\x01 \x01(\t\x12<\n\x0f\x65xceptionReason\x18\x02 \x01(\x0e\x32#.datakube.FinishJob.ExceptionReason\x12*\n\x06status\x18\x03 \x01(\x0e\x32\x1a.datakube.FinishJob.Status\"!\n\x06Status\x12\x0b\n\x07SUCCESS\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\"A\n\x0f\x45xceptionReason\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07GENERAL\x10\x01\x12\x17\n\x13\x43OMMUNICATION_ERROR\x10\x02\"\xab\x01\n\x1a\x41\x64\x64itionalConfigurationDto\x12T\n\x10\x63onfigurationMap\x18\x01 \x03(\x0b\x32:.datakube.AdditionalConfigurationDto.ConfigurationMapEntry\x1a\x37\n\x15\x43onfigurationMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01*\xcc\x02\n\x0c\x44\x61taKubeStep\x12\x17\n\x13VALIDATE_CONNECTION\x10\x00\x12\x14\n\x10\x43OLUMN_DISCOVERY\x10\x01\x12\x13\n\x0fTABLE_DISCOVERY\x10\x02\x12\x1a\n\x16\x44\x45PENDENCIES_DISCOVERY\x10\x03\x12\x0f\n\x0bSAMPLE_DATA\x10\x04\x12\t\n\x05TRAIN\x10\x05\x12\x0c\n\x08GENERATE\x10\x06\x12\x0c\n\x08\x45VALUATE\x10\x07\x12\x19\n\x15ML_SPLIT_AND_EVALUATE\x10\x08\x12\x19\n\x15ML_TRAIN_AND_GENERATE\x10\t\x12\x16\n\x12TRAIN_AND_GENERATE\x10\n\x12\x0b\n\x07WARM_UP\x10\x0b\x12\x0c\n\x08\x44T_TRAIN\x10\x0c\x12\x0f\n\x0b\x44T_GENERATE\x10\r\x12\x0f\n\x0b\x44T_EVALUATE\x10\x0e\x12\x19\n\x15\x44T_TRAIN_AND_GENERATE\x10\x0f\x42\x61\nHcom.datomize.datomizer.backend.components.management.dto.datakubeserviceB\x15\x44\x61taKubeServiceProtosb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x64\x61takubeservice.proto\x12\x08\x64\x61takube\"\xf9\x01\n\x0f\x44\x61taKubeMessage\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\r\n\x05jobId\x18\x02 \x01(\t\x12\x1a\n\x12securityIdentifier\x18\x03 \x01(\t\x12\x38\n\nobjectType\x18\x04 \x01(\x0e\x32$.datakube.DataKubeMessage.ObjectType\x12\x10\n\x08userName\x18\x05 \x01(\t\x12\x0e\n\x06\x66lowId\x18\x06 \x01(\t\"M\n\nObjectType\x12\x18\n\x14\x41\x44\x44_METADATA_MESSAGE\x10\x00\x12\x0e\n\nFINISH_JOB\x10\x01\x12\x15\n\x11SUBTASK_COMPLETED\x10\x02\"\x84\x01\n\x12\x41\x64\x64MetadataMessage\x12=\n\tmap_field\x18\x01 \x03(\x0b\x32*.datakube.AddMetadataMessage.MapFieldEntry\x1a/\n\rMapFieldEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xee\x01\n\tFinishJob\x12\x11\n\texception\x18\x01 \x01(\t\x12<\n\x0f\x65xceptionReason\x18\x02 \x01(\x0e\x32#.datakube.FinishJob.ExceptionReason\x12*\n\x06status\x18\x03 \x01(\x0e\x32\x1a.datakube.FinishJob.Status\"!\n\x06Status\x12\x0b\n\x07SUCCESS\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\"A\n\x0f\x45xceptionReason\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07GENERAL\x10\x01\x12\x17\n\x13\x43OMMUNICATION_ERROR\x10\x02\"\xab\x01\n\x1a\x41\x64\x64itionalConfigurationDto\x12T\n\x10\x63onfigurationMap\x18\x01 \x03(\x0b\x32:.datakube.AdditionalConfigurationDto.ConfigurationMapEntry\x1a\x37\n\x15\x43onfigurationMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01*\x97\x03\n\x0c\x44\x61taKubeStep\x12\x17\n\x13VALIDATE_CONNECTION\x10\x00\x12\x14\n\x10\x43OLUMN_DISCOVERY\x10\x01\x12\x13\n\x0fTABLE_DISCOVERY\x10\x02\x12\x1a\n\x16\x44\x45PENDENCIES_DISCOVERY\x10\x03\x12\x0f\n\x0bSAMPLE_DATA\x10\x04\x12\t\n\x05TRAIN\x10\x05\x12\x0c\n\x08GENERATE\x10\x06\x12\x0c\n\x08\x45VALUATE\x10\x07\x12\x19\n\x15ML_SPLIT_AND_EVALUATE\x10\x08\x12\x19\n\x15ML_TRAIN_AND_GENERATE\x10\t\x12\x16\n\x12TRAIN_AND_GENERATE\x10\n\x12\x0b\n\x07WARM_UP\x10\x0b\x12\x0c\n\x08\x44T_TRAIN\x10\x0c\x12\x0f\n\x0b\x44T_GENERATE\x10\r\x12\x0f\n\x0b\x44T_EVALUATE\x10\x0e\x12\x19\n\x15\x44T_TRAIN_AND_GENERATE\x10\x0f\x12\x0c\n\x08WI_TRAIN\x10\x10\x12\x0f\n\x0bWI_GENERATE\x10\x11\x12\x0f\n\x0bWI_EVALUATE\x10\x12\x12\x19\n\x15WI_TRAIN_AND_GENERATE\x10\x13\x42\x61\nHcom.datomize.datomizer.backend.components.management.dto.datakubeserviceB\x15\x44\x61taKubeServiceProtosb\x06proto3')
 
 _DATAKUBESTEP = DESCRIPTOR.enum_types_by_name['DataKubeStep']
 DataKubeStep = enum_type_wrapper.EnumTypeWrapper(_DATAKUBESTEP)
 VALIDATE_CONNECTION = 0
 COLUMN_DISCOVERY = 1
 TABLE_DISCOVERY = 2
 DEPENDENCIES_DISCOVERY = 3
@@ -31,14 +31,18 @@
 ML_TRAIN_AND_GENERATE = 9
 TRAIN_AND_GENERATE = 10
 WARM_UP = 11
 DT_TRAIN = 12
 DT_GENERATE = 13
 DT_EVALUATE = 14
 DT_TRAIN_AND_GENERATE = 15
+WI_TRAIN = 16
+WI_GENERATE = 17
+WI_EVALUATE = 18
+WI_TRAIN_AND_GENERATE = 19
 
 
 _DATAKUBEMESSAGE = DESCRIPTOR.message_types_by_name['DataKubeMessage']
 _ADDMETADATAMESSAGE = DESCRIPTOR.message_types_by_name['AddMetadataMessage']
 _ADDMETADATAMESSAGE_MAPFIELDENTRY = _ADDMETADATAMESSAGE.nested_types_by_name['MapFieldEntry']
 _FINISHJOB = DESCRIPTOR.message_types_by_name['FinishJob']
 _ADDITIONALCONFIGURATIONDTO = DESCRIPTOR.message_types_by_name['AdditionalConfigurationDto']
@@ -95,15 +99,15 @@
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\nHcom.datomize.datomizer.backend.components.management.dto.datakubeserviceB\025DataKubeServiceProtos'
   _ADDMETADATAMESSAGE_MAPFIELDENTRY._options = None
   _ADDMETADATAMESSAGE_MAPFIELDENTRY._serialized_options = b'8\001'
   _ADDITIONALCONFIGURATIONDTO_CONFIGURATIONMAPENTRY._options = None
   _ADDITIONALCONFIGURATIONDTO_CONFIGURATIONMAPENTRY._serialized_options = b'8\001'
   _DATAKUBESTEP._serialized_start=838
-  _DATAKUBESTEP._serialized_end=1170
+  _DATAKUBESTEP._serialized_end=1245
   _DATAKUBEMESSAGE._serialized_start=36
   _DATAKUBEMESSAGE._serialized_end=285
   _DATAKUBEMESSAGE_OBJECTTYPE._serialized_start=208
   _DATAKUBEMESSAGE_OBJECTTYPE._serialized_end=285
   _ADDMETADATAMESSAGE._serialized_start=288
   _ADDMETADATAMESSAGE._serialized_end=420
   _ADDMETADATAMESSAGE_MAPFIELDENTRY._serialized_start=373
```

### Comparing `datomize-2.1.7/datomizer/protos/datasourceconfigservice_pb2.py` & `datomize-2.3.7/datomizer/protos/datasourceconfigservice_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x64\x61tasourceconfigservice.proto\x12\x08\x64\x61takube\"\xae\x02\n\x13\x44\x61tasourceConfigDTO\x12?\n\x13\x62\x61sicAuthentication\x18\x01 \x01(\x0b\x32 .datakube.BasicAuthenticationDTOH\x00\x12/\n\x08\x64\x61tabase\x18\x0b \x01(\x0b\x32\x1b.datakube.DatabaseConfigDTOH\x01\x12\'\n\x04hdfs\x18\x0c \x01(\x0b\x32\x17.datakube.HDFSConfigDTOH\x01\x12#\n\x02s3\x18\r \x01(\x0b\x32\x15.datakube.S3ConfigDTOH\x01\x12\x36\n\x0c\x63ustomConfig\x18\x14 \x01(\x0b\x32 .datakube.CustomConfigurationDTOB\x10\n\x0e\x61uthenticationB\r\n\x0b\x64\x61ta_source\"\xae\x01\n\x16\x43ustomConfigurationDTO\x12.\n\tdelimiter\x18\x01 \x01(\x0b\x32\x1b.datakube.NullableStringDTO\x12.\n\tnoneValue\x18\x02 \x01(\x0b\x32\x1b.datakube.NullableStringDTO\x12\x34\n\x0f\x65scapeCharacter\x18\x03 \x01(\x0b\x32\x1b.datakube.NullableStringDTO\"2\n\x11NullableStringDTO\x12\x0e\n\x06isNull\x18\x01 \x01(\x08\x12\r\n\x05value\x18\x02 \x01(\t\"<\n\x16\x42\x61sicAuthenticationDTO\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"v\n\x11\x44\x61tabaseConfigDTO\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\t\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\x12\x0e\n\x06schema\x18\x04 \x01(\t\x12$\n\x04type\x18\x05 \x01(\x0e\x32\x16.datakube.DatabaseType\"\x95\x01\n\rHDFSConfigDTO\x12%\n\x06\x66ormat\x18\x01 \x01(\x0e\x32\x15.datakube.FilesFormat\x12\x11\n\troot_path\x18\x02 \x01(\t\x12\x14\n\x0c\x65ndpoint_url\x18\x03 \x01(\t\x12\x34\n\x0f\x66ormat_settings\x18\x04 \x01(\x0b\x32\x1b.datakube.FormatSettingsDTO\"\xa8\x01\n\x0bS3ConfigDTO\x12%\n\x06\x66ormat\x18\x01 \x01(\x0e\x32\x15.datakube.FilesFormat\x12\x11\n\troot_path\x18\x02 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x03 \x01(\t\x12\x14\n\x0c\x65ndpoint_url\x18\x04 \x01(\t\x12\x34\n\x0f\x66ormat_settings\x18\x05 \x01(\x0b\x32\x1b.datakube.FormatSettingsDTO\"R\n\x11\x46ormatSettingsDTO\x12\x33\n\x0c\x63sv_settings\x18\x01 \x01(\x0b\x32\x1b.datakube.ParserCSVSettingsH\x00\x42\x08\n\x06parser\"&\n\x11ParserCSVSettings\x12\x11\n\tdelimiter\x18\x01 \x01(\t\"\x8d\x01\n\x19\x44\x61taKubeJobDataSourcesDTO\x12\x37\n\x12origin_data_source\x18\x01 \x01(\x0b\x32\x1b.datakube.DatabaseConfigDTO\x12\x37\n\x12target_data_source\x18\x02 \x01(\x0b\x32\x1b.datakube.DatabaseConfigDTO*#\n\x0b\x46ilesFormat\x12\x0b\n\x07PARQUET\x10\x00\x12\x07\n\x03\x43SV\x10\x01*1\n\x0c\x44\x61tabaseType\x12\x0c\n\x08POSTGRES\x10\x00\x12\n\n\x06ORACLE\x10\x01\x12\x07\n\x03\x44\x42\x32\x10\x02\x42q\nPcom.datomize.datomizer.backend.components.management.dto.datasourceconfigserviceB\x1d\x44\x61tasourceConfigServiceProtosb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x64\x61tasourceconfigservice.proto\x12\x10\x64\x61tasourceconfig\"\xd6\x02\n\x13\x44\x61tasourceConfigDTO\x12G\n\x13\x62\x61sicAuthentication\x18\x01 \x01(\x0b\x32(.datasourceconfig.BasicAuthenticationDTOH\x00\x12\x37\n\x08\x64\x61tabase\x18\x0b \x01(\x0b\x32#.datasourceconfig.DatabaseConfigDTOH\x01\x12/\n\x04hdfs\x18\x0c \x01(\x0b\x32\x1f.datasourceconfig.HDFSConfigDTOH\x01\x12+\n\x02s3\x18\r \x01(\x0b\x32\x1d.datasourceconfig.S3ConfigDTOH\x01\x12>\n\x0c\x63ustomConfig\x18\x14 \x01(\x0b\x32(.datasourceconfig.CustomConfigurationDTOB\x10\n\x0e\x61uthenticationB\r\n\x0b\x64\x61ta_source\"\xfd\x01\n\x16\x43ustomConfigurationDTO\x12\x36\n\tdelimiter\x18\x01 \x01(\x0b\x32#.datasourceconfig.NullableStringDTO\x12\x36\n\tnoneValue\x18\x02 \x01(\x0b\x32#.datasourceconfig.NullableStringDTO\x12<\n\x0f\x65scapeCharacter\x18\x03 \x01(\x0b\x32#.datasourceconfig.NullableStringDTO\x12\x35\n\x08\x65ncoding\x18\x04 \x01(\x0b\x32#.datasourceconfig.NullableStringDTO\"2\n\x11NullableStringDTO\x12\x0e\n\x06isNull\x18\x01 \x01(\x08\x12\r\n\x05value\x18\x02 \x01(\t\"<\n\x16\x42\x61sicAuthenticationDTO\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"~\n\x11\x44\x61tabaseConfigDTO\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\t\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\x12\x0e\n\x06schema\x18\x04 \x01(\t\x12,\n\x04type\x18\x05 \x01(\x0e\x32\x1e.datasourceconfig.DatabaseType\"\xa5\x01\n\rHDFSConfigDTO\x12-\n\x06\x66ormat\x18\x01 \x01(\x0e\x32\x1d.datasourceconfig.FilesFormat\x12\x11\n\troot_path\x18\x02 \x01(\t\x12\x14\n\x0c\x65ndpoint_url\x18\x03 \x01(\t\x12<\n\x0f\x66ormat_settings\x18\x04 \x01(\x0b\x32#.datasourceconfig.FormatSettingsDTO\"\xb8\x01\n\x0bS3ConfigDTO\x12-\n\x06\x66ormat\x18\x01 \x01(\x0e\x32\x1d.datasourceconfig.FilesFormat\x12\x11\n\troot_path\x18\x02 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x03 \x01(\t\x12\x14\n\x0c\x65ndpoint_url\x18\x04 \x01(\t\x12<\n\x0f\x66ormat_settings\x18\x05 \x01(\x0b\x32#.datasourceconfig.FormatSettingsDTO\"Z\n\x11\x46ormatSettingsDTO\x12;\n\x0c\x63sv_settings\x18\x01 \x01(\x0b\x32#.datasourceconfig.ParserCSVSettingsH\x00\x42\x08\n\x06parser\"&\n\x11ParserCSVSettings\x12\x11\n\tdelimiter\x18\x01 \x01(\t\"\x9d\x01\n\x19\x44\x61taKubeJobDataSourcesDTO\x12?\n\x12origin_data_source\x18\x01 \x01(\x0b\x32#.datasourceconfig.DatabaseConfigDTO\x12?\n\x12target_data_source\x18\x02 \x01(\x0b\x32#.datasourceconfig.DatabaseConfigDTO*#\n\x0b\x46ilesFormat\x12\x0b\n\x07PARQUET\x10\x00\x12\x07\n\x03\x43SV\x10\x01*1\n\x0c\x44\x61tabaseType\x12\x0c\n\x08POSTGRES\x10\x00\x12\n\n\x06ORACLE\x10\x01\x12\x07\n\x03\x44\x42\x32\x10\x02\x42q\nPcom.datomize.datomizer.backend.components.management.dto.datasourceconfigserviceB\x1d\x44\x61tasourceConfigServiceProtosb\x06proto3')
 
 _FILESFORMAT = DESCRIPTOR.enum_types_by_name['FilesFormat']
 FilesFormat = enum_type_wrapper.EnumTypeWrapper(_FILESFORMAT)
 _DATABASETYPE = DESCRIPTOR.enum_types_by_name['DatabaseType']
 DatabaseType = enum_type_wrapper.EnumTypeWrapper(_DATABASETYPE)
 PARQUET = 0
 CSV = 1
@@ -37,103 +37,103 @@
 _S3CONFIGDTO = DESCRIPTOR.message_types_by_name['S3ConfigDTO']
 _FORMATSETTINGSDTO = DESCRIPTOR.message_types_by_name['FormatSettingsDTO']
 _PARSERCSVSETTINGS = DESCRIPTOR.message_types_by_name['ParserCSVSettings']
 _DATAKUBEJOBDATASOURCESDTO = DESCRIPTOR.message_types_by_name['DataKubeJobDataSourcesDTO']
 DatasourceConfigDTO = _reflection.GeneratedProtocolMessageType('DatasourceConfigDTO', (_message.Message,), {
   'DESCRIPTOR' : _DATASOURCECONFIGDTO,
   '__module__' : 'datasourceconfigservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.DatasourceConfigDTO)
+  # @@protoc_insertion_point(class_scope:datasourceconfig.DatasourceConfigDTO)
   })
 _sym_db.RegisterMessage(DatasourceConfigDTO)
 
 CustomConfigurationDTO = _reflection.GeneratedProtocolMessageType('CustomConfigurationDTO', (_message.Message,), {
   'DESCRIPTOR' : _CUSTOMCONFIGURATIONDTO,
   '__module__' : 'datasourceconfigservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.CustomConfigurationDTO)
+  # @@protoc_insertion_point(class_scope:datasourceconfig.CustomConfigurationDTO)
   })
 _sym_db.RegisterMessage(CustomConfigurationDTO)
 
 NullableStringDTO = _reflection.GeneratedProtocolMessageType('NullableStringDTO', (_message.Message,), {
   'DESCRIPTOR' : _NULLABLESTRINGDTO,
   '__module__' : 'datasourceconfigservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.NullableStringDTO)
+  # @@protoc_insertion_point(class_scope:datasourceconfig.NullableStringDTO)
   })
 _sym_db.RegisterMessage(NullableStringDTO)
 
 BasicAuthenticationDTO = _reflection.GeneratedProtocolMessageType('BasicAuthenticationDTO', (_message.Message,), {
   'DESCRIPTOR' : _BASICAUTHENTICATIONDTO,
   '__module__' : 'datasourceconfigservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.BasicAuthenticationDTO)
+  # @@protoc_insertion_point(class_scope:datasourceconfig.BasicAuthenticationDTO)
   })
 _sym_db.RegisterMessage(BasicAuthenticationDTO)
 
 DatabaseConfigDTO = _reflection.GeneratedProtocolMessageType('DatabaseConfigDTO', (_message.Message,), {
   'DESCRIPTOR' : _DATABASECONFIGDTO,
   '__module__' : 'datasourceconfigservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.DatabaseConfigDTO)
+  # @@protoc_insertion_point(class_scope:datasourceconfig.DatabaseConfigDTO)
   })
 _sym_db.RegisterMessage(DatabaseConfigDTO)
 
 HDFSConfigDTO = _reflection.GeneratedProtocolMessageType('HDFSConfigDTO', (_message.Message,), {
   'DESCRIPTOR' : _HDFSCONFIGDTO,
   '__module__' : 'datasourceconfigservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.HDFSConfigDTO)
+  # @@protoc_insertion_point(class_scope:datasourceconfig.HDFSConfigDTO)
   })
 _sym_db.RegisterMessage(HDFSConfigDTO)
 
 S3ConfigDTO = _reflection.GeneratedProtocolMessageType('S3ConfigDTO', (_message.Message,), {
   'DESCRIPTOR' : _S3CONFIGDTO,
   '__module__' : 'datasourceconfigservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.S3ConfigDTO)
+  # @@protoc_insertion_point(class_scope:datasourceconfig.S3ConfigDTO)
   })
 _sym_db.RegisterMessage(S3ConfigDTO)
 
 FormatSettingsDTO = _reflection.GeneratedProtocolMessageType('FormatSettingsDTO', (_message.Message,), {
   'DESCRIPTOR' : _FORMATSETTINGSDTO,
   '__module__' : 'datasourceconfigservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.FormatSettingsDTO)
+  # @@protoc_insertion_point(class_scope:datasourceconfig.FormatSettingsDTO)
   })
 _sym_db.RegisterMessage(FormatSettingsDTO)
 
 ParserCSVSettings = _reflection.GeneratedProtocolMessageType('ParserCSVSettings', (_message.Message,), {
   'DESCRIPTOR' : _PARSERCSVSETTINGS,
   '__module__' : 'datasourceconfigservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.ParserCSVSettings)
+  # @@protoc_insertion_point(class_scope:datasourceconfig.ParserCSVSettings)
   })
 _sym_db.RegisterMessage(ParserCSVSettings)
 
 DataKubeJobDataSourcesDTO = _reflection.GeneratedProtocolMessageType('DataKubeJobDataSourcesDTO', (_message.Message,), {
   'DESCRIPTOR' : _DATAKUBEJOBDATASOURCESDTO,
   '__module__' : 'datasourceconfigservice_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.DataKubeJobDataSourcesDTO)
+  # @@protoc_insertion_point(class_scope:datasourceconfig.DataKubeJobDataSourcesDTO)
   })
 _sym_db.RegisterMessage(DataKubeJobDataSourcesDTO)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\nPcom.datomize.datomizer.backend.components.management.dto.datasourceconfigserviceB\035DatasourceConfigServiceProtos'
-  _FILESFORMAT._serialized_start=1350
-  _FILESFORMAT._serialized_end=1385
-  _DATABASETYPE._serialized_start=1387
-  _DATABASETYPE._serialized_end=1436
-  _DATASOURCECONFIGDTO._serialized_start=44
-  _DATASOURCECONFIGDTO._serialized_end=346
-  _CUSTOMCONFIGURATIONDTO._serialized_start=349
-  _CUSTOMCONFIGURATIONDTO._serialized_end=523
-  _NULLABLESTRINGDTO._serialized_start=525
-  _NULLABLESTRINGDTO._serialized_end=575
-  _BASICAUTHENTICATIONDTO._serialized_start=577
-  _BASICAUTHENTICATIONDTO._serialized_end=637
-  _DATABASECONFIGDTO._serialized_start=639
-  _DATABASECONFIGDTO._serialized_end=757
-  _HDFSCONFIGDTO._serialized_start=760
-  _HDFSCONFIGDTO._serialized_end=909
-  _S3CONFIGDTO._serialized_start=912
-  _S3CONFIGDTO._serialized_end=1080
-  _FORMATSETTINGSDTO._serialized_start=1082
-  _FORMATSETTINGSDTO._serialized_end=1164
-  _PARSERCSVSETTINGS._serialized_start=1166
-  _PARSERCSVSETTINGS._serialized_end=1204
-  _DATAKUBEJOBDATASOURCESDTO._serialized_start=1207
-  _DATAKUBEJOBDATASOURCESDTO._serialized_end=1348
+  _FILESFORMAT._serialized_start=1541
+  _FILESFORMAT._serialized_end=1576
+  _DATABASETYPE._serialized_start=1578
+  _DATABASETYPE._serialized_end=1627
+  _DATASOURCECONFIGDTO._serialized_start=52
+  _DATASOURCECONFIGDTO._serialized_end=394
+  _CUSTOMCONFIGURATIONDTO._serialized_start=397
+  _CUSTOMCONFIGURATIONDTO._serialized_end=650
+  _NULLABLESTRINGDTO._serialized_start=652
+  _NULLABLESTRINGDTO._serialized_end=702
+  _BASICAUTHENTICATIONDTO._serialized_start=704
+  _BASICAUTHENTICATIONDTO._serialized_end=764
+  _DATABASECONFIGDTO._serialized_start=766
+  _DATABASECONFIGDTO._serialized_end=892
+  _HDFSCONFIGDTO._serialized_start=895
+  _HDFSCONFIGDTO._serialized_end=1060
+  _S3CONFIGDTO._serialized_start=1063
+  _S3CONFIGDTO._serialized_end=1247
+  _FORMATSETTINGSDTO._serialized_start=1249
+  _FORMATSETTINGSDTO._serialized_end=1339
+  _PARSERCSVSETTINGS._serialized_start=1341
+  _PARSERCSVSETTINGS._serialized_end=1379
+  _DATAKUBEJOBDATASOURCESDTO._serialized_start=1382
+  _DATAKUBEJOBDATASOURCESDTO._serialized_end=1539
 # @@protoc_insertion_point(module_scope)
```

### Comparing `datomize-2.1.7/datomizer/protos/infrastructuresettings_pb2.py` & `datomize-2.3.7/datomizer/protos/infrastructuresettings_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,59 +10,59 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cinfrastructuresettings.proto\x12\x08\x64\x61takube\"\xda\x01\n\x1fSparkConnectionConfigurationDto\x12\x0b\n\x03url\x18\x01 \x01(\t\x12i\n\x18\x63onfigurationVariableMap\x18\x02 \x03(\x0b\x32G.datakube.SparkConnectionConfigurationDto.ConfigurationVariableMapEntry\x1a?\n\x1d\x43onfigurationVariableMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\\\n\x19S3StorageConfigurationDto\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"W\n\x15KafkaConfigurationDto\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\tBp\nPcom.datomize.datomizer.backend.components.management.dto.infrastructure.settingsB\x1cInfrastructureSettingsProtosb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cinfrastructuresettings.proto\x12\x0einfrastructure\"\xe0\x01\n\x1fSparkConnectionConfigurationDto\x12\x0b\n\x03url\x18\x01 \x01(\t\x12o\n\x18\x63onfigurationVariableMap\x18\x02 \x03(\x0b\x32M.infrastructure.SparkConnectionConfigurationDto.ConfigurationVariableMapEntry\x1a?\n\x1d\x43onfigurationVariableMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\\\n\x19S3StorageConfigurationDto\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"W\n\x15KafkaConfigurationDto\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\r\n\x05topic\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\tBp\nPcom.datomize.datomizer.backend.components.management.dto.infrastructure.settingsB\x1cInfrastructureSettingsProtosb\x06proto3')
 
 
 
 _SPARKCONNECTIONCONFIGURATIONDTO = DESCRIPTOR.message_types_by_name['SparkConnectionConfigurationDto']
 _SPARKCONNECTIONCONFIGURATIONDTO_CONFIGURATIONVARIABLEMAPENTRY = _SPARKCONNECTIONCONFIGURATIONDTO.nested_types_by_name['ConfigurationVariableMapEntry']
 _S3STORAGECONFIGURATIONDTO = DESCRIPTOR.message_types_by_name['S3StorageConfigurationDto']
 _KAFKACONFIGURATIONDTO = DESCRIPTOR.message_types_by_name['KafkaConfigurationDto']
 SparkConnectionConfigurationDto = _reflection.GeneratedProtocolMessageType('SparkConnectionConfigurationDto', (_message.Message,), {
 
   'ConfigurationVariableMapEntry' : _reflection.GeneratedProtocolMessageType('ConfigurationVariableMapEntry', (_message.Message,), {
     'DESCRIPTOR' : _SPARKCONNECTIONCONFIGURATIONDTO_CONFIGURATIONVARIABLEMAPENTRY,
     '__module__' : 'infrastructuresettings_pb2'
-    # @@protoc_insertion_point(class_scope:datakube.SparkConnectionConfigurationDto.ConfigurationVariableMapEntry)
+    # @@protoc_insertion_point(class_scope:infrastructure.SparkConnectionConfigurationDto.ConfigurationVariableMapEntry)
     })
   ,
   'DESCRIPTOR' : _SPARKCONNECTIONCONFIGURATIONDTO,
   '__module__' : 'infrastructuresettings_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.SparkConnectionConfigurationDto)
+  # @@protoc_insertion_point(class_scope:infrastructure.SparkConnectionConfigurationDto)
   })
 _sym_db.RegisterMessage(SparkConnectionConfigurationDto)
 _sym_db.RegisterMessage(SparkConnectionConfigurationDto.ConfigurationVariableMapEntry)
 
 S3StorageConfigurationDto = _reflection.GeneratedProtocolMessageType('S3StorageConfigurationDto', (_message.Message,), {
   'DESCRIPTOR' : _S3STORAGECONFIGURATIONDTO,
   '__module__' : 'infrastructuresettings_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.S3StorageConfigurationDto)
+  # @@protoc_insertion_point(class_scope:infrastructure.S3StorageConfigurationDto)
   })
 _sym_db.RegisterMessage(S3StorageConfigurationDto)
 
 KafkaConfigurationDto = _reflection.GeneratedProtocolMessageType('KafkaConfigurationDto', (_message.Message,), {
   'DESCRIPTOR' : _KAFKACONFIGURATIONDTO,
   '__module__' : 'infrastructuresettings_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.KafkaConfigurationDto)
+  # @@protoc_insertion_point(class_scope:infrastructure.KafkaConfigurationDto)
   })
 _sym_db.RegisterMessage(KafkaConfigurationDto)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\nPcom.datomize.datomizer.backend.components.management.dto.infrastructure.settingsB\034InfrastructureSettingsProtos'
   _SPARKCONNECTIONCONFIGURATIONDTO_CONFIGURATIONVARIABLEMAPENTRY._options = None
   _SPARKCONNECTIONCONFIGURATIONDTO_CONFIGURATIONVARIABLEMAPENTRY._serialized_options = b'8\001'
-  _SPARKCONNECTIONCONFIGURATIONDTO._serialized_start=43
-  _SPARKCONNECTIONCONFIGURATIONDTO._serialized_end=261
-  _SPARKCONNECTIONCONFIGURATIONDTO_CONFIGURATIONVARIABLEMAPENTRY._serialized_start=198
-  _SPARKCONNECTIONCONFIGURATIONDTO_CONFIGURATIONVARIABLEMAPENTRY._serialized_end=261
-  _S3STORAGECONFIGURATIONDTO._serialized_start=263
-  _S3STORAGECONFIGURATIONDTO._serialized_end=355
-  _KAFKACONFIGURATIONDTO._serialized_start=357
-  _KAFKACONFIGURATIONDTO._serialized_end=444
+  _SPARKCONNECTIONCONFIGURATIONDTO._serialized_start=49
+  _SPARKCONNECTIONCONFIGURATIONDTO._serialized_end=273
+  _SPARKCONNECTIONCONFIGURATIONDTO_CONFIGURATIONVARIABLEMAPENTRY._serialized_start=210
+  _SPARKCONNECTIONCONFIGURATIONDTO_CONFIGURATIONVARIABLEMAPENTRY._serialized_end=273
+  _S3STORAGECONFIGURATIONDTO._serialized_start=275
+  _S3STORAGECONFIGURATIONDTO._serialized_end=367
+  _KAFKACONFIGURATIONDTO._serialized_start=369
+  _KAFKACONFIGURATIONDTO._serialized_end=456
 # @@protoc_insertion_point(module_scope)
```

### Comparing `datomize-2.1.7/datomizer/protos/synthschemavalidationresult_pb2.py` & `datomize-2.3.7/datomizer/protos/synthschemavalidationresult_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,28 +11,32 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!synthschemavalidationresult.proto\x12\x08\x64\x61takube\"7\n\nSummaryDTO\x12\x0c\n\x04high\x18\x01 \x01(\x03\x12\x0e\n\x06medium\x18\x02 \x01(\x03\x12\x0b\n\x03low\x18\x03 \x01(\x03\"\xd3\x03\n\x1eSynthSchemaValidationResultDTO\x12\x12\n\ntotalScore\x18\x01 \x01(\x01\x12\x13\n\x0btablesTotal\x18\x02 \x01(\x01\x12\x17\n\x0f\x64\x65pendencyTotal\x18\x03 \x01(\x01\x12\x32\n\x06tables\x18\x04 \x03(\x0b\x32\".datakube.TableValidationResultDTO\x12=\n\x0c\x64\x65pendencies\x18\x05 \x03(\x0b\x32\'.datakube.DependencyValidationResultDTO\x12V\n\x0fmeasuresSummary\x18\x06 \x03(\x0b\x32=.datakube.SynthSchemaValidationResultDTO.MeasuresSummaryEntry\x12\x32\n\x14tablesQualitySummary\x18\x07 \x01(\x0b\x32\x14.datakube.SummaryDTO\x12\x38\n\x1a\x64\x65pendenciesQualitySummary\x18\x08 \x01(\x0b\x32\x14.datakube.SummaryDTO\x1a\x36\n\x14MeasuresSummaryEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"\xbf\x05\n\x18TableValidationResultDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x0c\x64istribution\x18\x02 \x01(\x0b\x32\x19.datakube.DoubleVectorDTO\x12.\n\x0b\x63orrelation\x18\x03 \x01(\x0b\x32\x19.datakube.DoubleMatrixDTO\x12/\n\tdetection\x18\x04 \x03(\x0b\x32\x1c.datakube.DetectionResultDTO\x12+\n\x07utility\x18\x05 \x03(\x0b\x32\x1a.datakube.UtilityResultDTO\x12-\n\x08\x63overage\x18\x06 \x03(\x0b\x32\x1b.datakube.CoverageResultDTO\x12V\n\x12measureTotalScores\x18\x07 \x03(\x0b\x32:.datakube.TableValidationResultDTO.MeasureTotalScoresEntry\x12\x12\n\ntotalScore\x18\x08 \x01(\x01\x12\x30\n\x12\x63orrelationSummary\x18\t \x01(\x0b\x32\x14.datakube.SummaryDTO\x12\x39\n\x14\x63olumnsDistributions\x18\x0b \x03(\x0b\x32\x1b.datakube.ColumnDistHistDTO\x12\x33\n\x0b\x63overageNew\x18\x0c \x01(\x0b\x32\x1e.datakube.CoverageResultNewDTO\x12*\n\ttextScore\x18\r \x01(\x0b\x32\x17.datakube.TextResultDTO\x12\x32\n\rsequenceScore\x18\x0e \x03(\x0b\x32\x1b.datakube.SequenceResultDTO\x1a\x39\n\x17MeasureTotalScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"\xc8\x03\n\x1d\x44\x65pendencyValidationResultDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x0b\x63orrelation\x18\x02 \x01(\x0b\x32\x19.datakube.DoubleMatrixDTO\x12/\n\tdetection\x18\x03 \x03(\x0b\x32\x1c.datakube.DetectionResultDTO\x12+\n\x07utility\x18\x04 \x03(\x0b\x32\x1a.datakube.UtilityResultDTO\x12-\n\x08\x63overage\x18\x05 \x03(\x0b\x32\x1b.datakube.CoverageResultDTO\x12[\n\x12measureTotalScores\x18\x06 \x03(\x0b\x32?.datakube.DependencyValidationResultDTO.MeasureTotalScoresEntry\x12\x12\n\ntotalScore\x18\x07 \x01(\x01\x12\x30\n\x12\x63orrelationSummary\x18\x08 \x01(\x0b\x32\x14.datakube.SummaryDTO\x1a\x39\n\x17MeasureTotalScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"\x9d\x01\n\x12\x44\x65tectionResultDTO\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12%\n\x04type\x18\x02 \x01(\x0e\x32\x17.datakube.AlgorithmType\x12(\n\nmetricType\x18\x03 \x01(\x0e\x32\x14.datakube.MetricType\x12\r\n\x05score\x18\x04 \x01(\x01\x12\x10\n\x08RawScore\x18\x05 \x01(\x01\"y\n\x11\x43overageResultDTO\x12%\n\x04type\x18\x01 \x01(\x0e\x32\x17.datakube.AlgorithmType\x12,\n\x07results\x18\x02 \x03(\x0b\x32\x1b.datakube.MLScoreResultsDTO\x12\x0f\n\x07\x43olName\x18\x03 \x01(\t\"N\n\x14\x43overageResultNewDTO\x12\x19\n\x11originCardinality\x18\x01 \x03(\x01\x12\x0c\n\x04\x63ols\x18\x02 \x03(\t\x12\r\n\x05score\x18\x03 \x03(\x01\"x\n\x10UtilityResultDTO\x12%\n\x04type\x18\x01 \x01(\x0e\x32\x17.datakube.AlgorithmType\x12,\n\x07results\x18\x02 \x03(\x0b\x32\x1b.datakube.MLScoreResultsDTO\x12\x0f\n\x07\x43olName\x18\x03 \x01(\t\"\xb9\x01\n\x11MLScoreResultsDTO\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12(\n\nmetricType\x18\x02 \x01(\x0e\x32\x14.datakube.MetricType\x12\x13\n\x0boriginScore\x18\x03 \x01(\x01\x12\x13\n\x0btargetScore\x18\x04 \x01(\x01\x12\x11\n\tdiffScore\x18\x05 \x01(\x01\x12\x0f\n\x07success\x18\x06 \x01(\x08\x12\x15\n\rfailureReason\x18\x07 \x01(\t\"?\n\x0f\x44oubleMatrixDTO\x12\x0c\n\x04rows\x18\x01 \x03(\t\x12\x0c\n\x04\x63ols\x18\x02 \x03(\t\x12\x10\n\x04\x64\x61ta\x18\x03 \x03(\x01\x42\x02\x10\x01\"1\n\x0f\x44oubleVectorDTO\x12\x0c\n\x04\x63ols\x18\x01 \x03(\t\x12\x10\n\x04\x64\x61ta\x18\x02 \x03(\x01\x42\x02\x10\x01\"-\n\x07HistDTO\x12\x13\n\x0bxTickLabels\x18\x01 \x03(\t\x12\r\n\x05yData\x18\x02 \x03(\x01\"\x8c\x01\n\x11\x43olumnDistHistDTO\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12%\n\noriginHist\x18\x02 \x01(\x0b\x32\x11.datakube.HistDTO\x12%\n\ntargetHist\x18\x03 \x01(\x0b\x32\x11.datakube.HistDTO\x12\x15\n\risCategorical\x18\x04 \x01(\x08\"R\n\rTextResultDTO\x12\r\n\x05score\x18\x01 \x01(\x01\x12\x32\n\x0b\x63olumnScore\x18\x02 \x03(\x0b\x32\x1d.datakube.TextColumnResultDTO\"g\n\x13TextColumnResultDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rbi_gram_score\x18\x02 \x01(\x01\x12\x16\n\x0etri_gram_score\x18\x03 \x01(\x01\x12\x13\n\x0btotal_score\x18\x04 \x01(\x01\"\xdb\x01\n\x11SequenceResultDTO\x12\x1f\n\x04type\x18\x01 \x01(\x0e\x32\x11.datakube.SeqType\x12\x12\n\noriginSize\x18\x02 \x01(\x03\x12\x12\n\ntargetSize\x18\x03 \x01(\x03\x12\x15\n\ralgorithmName\x18\x04 \x01(\t\x12(\n\nmetricType\x18\x05 \x01(\x0e\x32\x14.datakube.MetricType\x12\x13\n\x0boriginScore\x18\x06 \x01(\x01\x12\x13\n\x0btargetScore\x18\x07 \x01(\x01\x12\x12\n\nsimilarity\x18\x08 \x01(\x01*.\n\rAlgorithmType\x12\x0e\n\nCLASSIFIER\x10\x00\x12\r\n\tREGRESSOR\x10\x01*0\n\nMetricType\x12\x07\n\x03\x41UC\x10\x00\x12\x06\n\x02\x46\x31\x10\x01\x12\x08\n\x04RMSE\x10\x02\x12\x07\n\x03MSE\x10\x03*-\n\x07SeqType\x12\n\n\x06SINGLE\x10\x00\x12\n\n\x06\x44OUBLE\x10\x01\x12\n\n\x06SERIES\x10\x02\x42{\nUcom.datomize.datomizer.backend.components.management.dto.synthschemavalidationserviceB\"SynthSchemaValidationServiceProtosb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!synthschemavalidationresult.proto\x12\x15synthschemavalidation\"7\n\nSummaryDTO\x12\x0c\n\x04high\x18\x01 \x01(\x03\x12\x0e\n\x06medium\x18\x02 \x01(\x03\x12\x0b\n\x03low\x18\x03 \x01(\x03\"\xab\x04\n\x1eSynthSchemaValidationResultDTO\x12\x12\n\ntotalScore\x18\x01 \x01(\x01\x12\x13\n\x0btablesTotal\x18\x02 \x01(\x01\x12\x17\n\x0f\x64\x65pendencyTotal\x18\x03 \x01(\x01\x12?\n\x06tables\x18\x04 \x03(\x0b\x32/.synthschemavalidation.TableValidationResultDTO\x12J\n\x0c\x64\x65pendencies\x18\x05 \x03(\x0b\x32\x34.synthschemavalidation.DependencyValidationResultDTO\x12\x63\n\x0fmeasuresSummary\x18\x06 \x03(\x0b\x32J.synthschemavalidation.SynthSchemaValidationResultDTO.MeasuresSummaryEntry\x12?\n\x14tablesQualitySummary\x18\x07 \x01(\x0b\x32!.synthschemavalidation.SummaryDTO\x12\x45\n\x1a\x64\x65pendenciesQualitySummary\x18\x08 \x01(\x0b\x32!.synthschemavalidation.SummaryDTO\x12\x15\n\routputRecords\x18\t \x01(\x03\x1a\x36\n\x14MeasuresSummaryEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"\xaa\x07\n\x18TableValidationResultDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12<\n\x0c\x64istribution\x18\x02 \x01(\x0b\x32&.synthschemavalidation.DoubleVectorDTO\x12;\n\x0b\x63orrelation\x18\x03 \x01(\x0b\x32&.synthschemavalidation.DoubleMatrixDTO\x12<\n\tdetection\x18\x04 \x03(\x0b\x32).synthschemavalidation.DetectionResultDTO\x12\x38\n\x07utility\x18\x05 \x03(\x0b\x32\'.synthschemavalidation.UtilityResultDTO\x12:\n\x08\x63overage\x18\x06 \x03(\x0b\x32(.synthschemavalidation.CoverageResultDTO\x12\x63\n\x12measureTotalScores\x18\x07 \x03(\x0b\x32G.synthschemavalidation.TableValidationResultDTO.MeasureTotalScoresEntry\x12\x12\n\ntotalScore\x18\x08 \x01(\x01\x12=\n\x12\x63orrelationSummary\x18\t \x01(\x0b\x32!.synthschemavalidation.SummaryDTO\x12\x46\n\x14\x63olumnsDistributions\x18\x0b \x03(\x0b\x32(.synthschemavalidation.ColumnDistHistDTO\x12@\n\x0b\x63overageNew\x18\x0c \x01(\x0b\x32+.synthschemavalidation.CoverageResultNewDTO\x12\x37\n\ttextScore\x18\r \x01(\x0b\x32$.synthschemavalidation.TextResultDTO\x12?\n\rsequenceScore\x18\x0e \x03(\x0b\x32(.synthschemavalidation.SequenceResultDTO\x12\x15\n\routputRecords\x18\x0f \x01(\x03\x12\x43\n\x1b\x64\x65tectionFeatureImportances\x18\x10 \x01(\x0b\x32\x1e.synthschemavalidation.HistDTO\x1a\x39\n\x17MeasureTotalScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"\x96\x04\n\x1d\x44\x65pendencyValidationResultDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12;\n\x0b\x63orrelation\x18\x02 \x01(\x0b\x32&.synthschemavalidation.DoubleMatrixDTO\x12<\n\tdetection\x18\x03 \x03(\x0b\x32).synthschemavalidation.DetectionResultDTO\x12\x38\n\x07utility\x18\x04 \x03(\x0b\x32\'.synthschemavalidation.UtilityResultDTO\x12:\n\x08\x63overage\x18\x05 \x03(\x0b\x32(.synthschemavalidation.CoverageResultDTO\x12h\n\x12measureTotalScores\x18\x06 \x03(\x0b\x32L.synthschemavalidation.DependencyValidationResultDTO.MeasureTotalScoresEntry\x12\x12\n\ntotalScore\x18\x07 \x01(\x01\x12=\n\x12\x63orrelationSummary\x18\x08 \x01(\x0b\x32!.synthschemavalidation.SummaryDTO\x1a\x39\n\x17MeasureTotalScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"\xb7\x01\n\x12\x44\x65tectionResultDTO\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x32\n\x04type\x18\x02 \x01(\x0e\x32$.synthschemavalidation.AlgorithmType\x12\x35\n\nmetricType\x18\x03 \x01(\x0e\x32!.synthschemavalidation.MetricType\x12\r\n\x05score\x18\x04 \x01(\x01\x12\x10\n\x08RawScore\x18\x05 \x01(\x01\"\x93\x01\n\x11\x43overageResultDTO\x12\x32\n\x04type\x18\x01 \x01(\x0e\x32$.synthschemavalidation.AlgorithmType\x12\x39\n\x07results\x18\x02 \x03(\x0b\x32(.synthschemavalidation.MLScoreResultsDTO\x12\x0f\n\x07\x43olName\x18\x03 \x01(\t\"N\n\x14\x43overageResultNewDTO\x12\x19\n\x11originCardinality\x18\x01 \x03(\x01\x12\x0c\n\x04\x63ols\x18\x02 \x03(\t\x12\r\n\x05score\x18\x03 \x03(\x01\"\x92\x01\n\x10UtilityResultDTO\x12\x32\n\x04type\x18\x01 \x01(\x0e\x32$.synthschemavalidation.AlgorithmType\x12\x39\n\x07results\x18\x02 \x03(\x0b\x32(.synthschemavalidation.MLScoreResultsDTO\x12\x0f\n\x07\x43olName\x18\x03 \x01(\t\"\xc6\x01\n\x11MLScoreResultsDTO\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x35\n\nmetricType\x18\x02 \x01(\x0e\x32!.synthschemavalidation.MetricType\x12\x13\n\x0boriginScore\x18\x03 \x01(\x01\x12\x13\n\x0btargetScore\x18\x04 \x01(\x01\x12\x11\n\tdiffScore\x18\x05 \x01(\x01\x12\x0f\n\x07success\x18\x06 \x01(\x08\x12\x15\n\rfailureReason\x18\x07 \x01(\t\"?\n\x0f\x44oubleMatrixDTO\x12\x0c\n\x04rows\x18\x01 \x03(\t\x12\x0c\n\x04\x63ols\x18\x02 \x03(\t\x12\x10\n\x04\x64\x61ta\x18\x03 \x03(\x01\x42\x02\x10\x01\"1\n\x0f\x44oubleVectorDTO\x12\x0c\n\x04\x63ols\x18\x01 \x03(\t\x12\x10\n\x04\x64\x61ta\x18\x02 \x03(\x01\x42\x02\x10\x01\"-\n\x07HistDTO\x12\x13\n\x0bxTickLabels\x18\x01 \x03(\t\x12\r\n\x05yData\x18\x02 \x03(\x01\"\xa6\x01\n\x11\x43olumnDistHistDTO\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12\x32\n\noriginHist\x18\x02 \x01(\x0b\x32\x1e.synthschemavalidation.HistDTO\x12\x32\n\ntargetHist\x18\x03 \x01(\x0b\x32\x1e.synthschemavalidation.HistDTO\x12\x15\n\risCategorical\x18\x04 \x01(\x08\"\x93\x01\n\rTextResultDTO\x12\r\n\x05score\x18\x01 \x01(\x01\x12?\n\x0b\x63olumnScore\x18\x02 \x03(\x0b\x32*.synthschemavalidation.TextColumnResultDTO\x12\x32\n\x05types\x18\x03 \x03(\x0b\x32#.synthschemavalidation.TextScoreDTO\"\xcd\x01\n\x13TextColumnResultDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rbi_gram_score\x18\x02 \x01(\x01\x12\x16\n\x0etri_gram_score\x18\x03 \x01(\x01\x12\x13\n\x0btotal_score\x18\x04 \x01(\x01\x12-\n\x04type\x18\x05 \x01(\x0e\x32\x1f.synthschemavalidation.TextType\x12\x35\n\x07metrics\x18\x06 \x03(\x0b\x32$.synthschemavalidation.TextMetricDTO\"L\n\x0cTextScoreDTO\x12-\n\x04type\x18\x01 \x01(\x0e\x32\x1f.synthschemavalidation.TextType\x12\r\n\x05score\x18\x02 \x01(\x01\"\xa6\x01\n\rTextMetricDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x46\n\tsubScores\x18\x02 \x03(\x0b\x32\x33.synthschemavalidation.TextMetricDTO.SubScoresEntry\x12\r\n\x05score\x18\x03 \x01(\x01\x1a\x30\n\x0eSubScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"\xf5\x01\n\x11SequenceResultDTO\x12,\n\x04type\x18\x01 \x01(\x0e\x32\x1e.synthschemavalidation.SeqType\x12\x12\n\noriginSize\x18\x02 \x01(\x03\x12\x12\n\ntargetSize\x18\x03 \x01(\x03\x12\x15\n\ralgorithmName\x18\x04 \x01(\t\x12\x35\n\nmetricType\x18\x05 \x01(\x0e\x32!.synthschemavalidation.MetricType\x12\x13\n\x0boriginScore\x18\x06 \x01(\x01\x12\x13\n\x0btargetScore\x18\x07 \x01(\x01\x12\x12\n\nsimilarity\x18\x08 \x01(\x01*.\n\rAlgorithmType\x12\x0e\n\nCLASSIFIER\x10\x00\x12\r\n\tREGRESSOR\x10\x01*0\n\nMetricType\x12\x07\n\x03\x41UC\x10\x00\x12\x06\n\x02\x46\x31\x10\x01\x12\x08\n\x04RMSE\x10\x02\x12\x07\n\x03MSE\x10\x03*\x1d\n\x08TextType\x12\x08\n\x04\x43HAR\x10\x00\x12\x07\n\x03\x45NG\x10\x01*-\n\x07SeqType\x12\n\n\x06SINGLE\x10\x00\x12\n\n\x06\x44OUBLE\x10\x01\x12\n\n\x06SERIES\x10\x02\x42{\nUcom.datomize.datomizer.backend.components.management.dto.synthschemavalidationserviceB\"SynthSchemaValidationServiceProtosb\x06proto3')
 
 _ALGORITHMTYPE = DESCRIPTOR.enum_types_by_name['AlgorithmType']
 AlgorithmType = enum_type_wrapper.EnumTypeWrapper(_ALGORITHMTYPE)
 _METRICTYPE = DESCRIPTOR.enum_types_by_name['MetricType']
 MetricType = enum_type_wrapper.EnumTypeWrapper(_METRICTYPE)
+_TEXTTYPE = DESCRIPTOR.enum_types_by_name['TextType']
+TextType = enum_type_wrapper.EnumTypeWrapper(_TEXTTYPE)
 _SEQTYPE = DESCRIPTOR.enum_types_by_name['SeqType']
 SeqType = enum_type_wrapper.EnumTypeWrapper(_SEQTYPE)
 CLASSIFIER = 0
 REGRESSOR = 1
 AUC = 0
 F1 = 1
 RMSE = 2
 MSE = 3
+CHAR = 0
+ENG = 1
 SINGLE = 0
 DOUBLE = 1
 SERIES = 2
 
 
 _SUMMARYDTO = DESCRIPTOR.message_types_by_name['SummaryDTO']
 _SYNTHSCHEMAVALIDATIONRESULTDTO = DESCRIPTOR.message_types_by_name['SynthSchemaValidationResultDTO']
@@ -48,148 +52,173 @@
 _MLSCORERESULTSDTO = DESCRIPTOR.message_types_by_name['MLScoreResultsDTO']
 _DOUBLEMATRIXDTO = DESCRIPTOR.message_types_by_name['DoubleMatrixDTO']
 _DOUBLEVECTORDTO = DESCRIPTOR.message_types_by_name['DoubleVectorDTO']
 _HISTDTO = DESCRIPTOR.message_types_by_name['HistDTO']
 _COLUMNDISTHISTDTO = DESCRIPTOR.message_types_by_name['ColumnDistHistDTO']
 _TEXTRESULTDTO = DESCRIPTOR.message_types_by_name['TextResultDTO']
 _TEXTCOLUMNRESULTDTO = DESCRIPTOR.message_types_by_name['TextColumnResultDTO']
+_TEXTSCOREDTO = DESCRIPTOR.message_types_by_name['TextScoreDTO']
+_TEXTMETRICDTO = DESCRIPTOR.message_types_by_name['TextMetricDTO']
+_TEXTMETRICDTO_SUBSCORESENTRY = _TEXTMETRICDTO.nested_types_by_name['SubScoresEntry']
 _SEQUENCERESULTDTO = DESCRIPTOR.message_types_by_name['SequenceResultDTO']
 SummaryDTO = _reflection.GeneratedProtocolMessageType('SummaryDTO', (_message.Message,), {
   'DESCRIPTOR' : _SUMMARYDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.SummaryDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.SummaryDTO)
   })
 _sym_db.RegisterMessage(SummaryDTO)
 
 SynthSchemaValidationResultDTO = _reflection.GeneratedProtocolMessageType('SynthSchemaValidationResultDTO', (_message.Message,), {
 
   'MeasuresSummaryEntry' : _reflection.GeneratedProtocolMessageType('MeasuresSummaryEntry', (_message.Message,), {
     'DESCRIPTOR' : _SYNTHSCHEMAVALIDATIONRESULTDTO_MEASURESSUMMARYENTRY,
     '__module__' : 'synthschemavalidationresult_pb2'
-    # @@protoc_insertion_point(class_scope:datakube.SynthSchemaValidationResultDTO.MeasuresSummaryEntry)
+    # @@protoc_insertion_point(class_scope:synthschemavalidation.SynthSchemaValidationResultDTO.MeasuresSummaryEntry)
     })
   ,
   'DESCRIPTOR' : _SYNTHSCHEMAVALIDATIONRESULTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.SynthSchemaValidationResultDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.SynthSchemaValidationResultDTO)
   })
 _sym_db.RegisterMessage(SynthSchemaValidationResultDTO)
 _sym_db.RegisterMessage(SynthSchemaValidationResultDTO.MeasuresSummaryEntry)
 
 TableValidationResultDTO = _reflection.GeneratedProtocolMessageType('TableValidationResultDTO', (_message.Message,), {
 
   'MeasureTotalScoresEntry' : _reflection.GeneratedProtocolMessageType('MeasureTotalScoresEntry', (_message.Message,), {
     'DESCRIPTOR' : _TABLEVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY,
     '__module__' : 'synthschemavalidationresult_pb2'
-    # @@protoc_insertion_point(class_scope:datakube.TableValidationResultDTO.MeasureTotalScoresEntry)
+    # @@protoc_insertion_point(class_scope:synthschemavalidation.TableValidationResultDTO.MeasureTotalScoresEntry)
     })
   ,
   'DESCRIPTOR' : _TABLEVALIDATIONRESULTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.TableValidationResultDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.TableValidationResultDTO)
   })
 _sym_db.RegisterMessage(TableValidationResultDTO)
 _sym_db.RegisterMessage(TableValidationResultDTO.MeasureTotalScoresEntry)
 
 DependencyValidationResultDTO = _reflection.GeneratedProtocolMessageType('DependencyValidationResultDTO', (_message.Message,), {
 
   'MeasureTotalScoresEntry' : _reflection.GeneratedProtocolMessageType('MeasureTotalScoresEntry', (_message.Message,), {
     'DESCRIPTOR' : _DEPENDENCYVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY,
     '__module__' : 'synthschemavalidationresult_pb2'
-    # @@protoc_insertion_point(class_scope:datakube.DependencyValidationResultDTO.MeasureTotalScoresEntry)
+    # @@protoc_insertion_point(class_scope:synthschemavalidation.DependencyValidationResultDTO.MeasureTotalScoresEntry)
     })
   ,
   'DESCRIPTOR' : _DEPENDENCYVALIDATIONRESULTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.DependencyValidationResultDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.DependencyValidationResultDTO)
   })
 _sym_db.RegisterMessage(DependencyValidationResultDTO)
 _sym_db.RegisterMessage(DependencyValidationResultDTO.MeasureTotalScoresEntry)
 
 DetectionResultDTO = _reflection.GeneratedProtocolMessageType('DetectionResultDTO', (_message.Message,), {
   'DESCRIPTOR' : _DETECTIONRESULTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.DetectionResultDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.DetectionResultDTO)
   })
 _sym_db.RegisterMessage(DetectionResultDTO)
 
 CoverageResultDTO = _reflection.GeneratedProtocolMessageType('CoverageResultDTO', (_message.Message,), {
   'DESCRIPTOR' : _COVERAGERESULTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.CoverageResultDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.CoverageResultDTO)
   })
 _sym_db.RegisterMessage(CoverageResultDTO)
 
 CoverageResultNewDTO = _reflection.GeneratedProtocolMessageType('CoverageResultNewDTO', (_message.Message,), {
   'DESCRIPTOR' : _COVERAGERESULTNEWDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.CoverageResultNewDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.CoverageResultNewDTO)
   })
 _sym_db.RegisterMessage(CoverageResultNewDTO)
 
 UtilityResultDTO = _reflection.GeneratedProtocolMessageType('UtilityResultDTO', (_message.Message,), {
   'DESCRIPTOR' : _UTILITYRESULTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.UtilityResultDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.UtilityResultDTO)
   })
 _sym_db.RegisterMessage(UtilityResultDTO)
 
 MLScoreResultsDTO = _reflection.GeneratedProtocolMessageType('MLScoreResultsDTO', (_message.Message,), {
   'DESCRIPTOR' : _MLSCORERESULTSDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.MLScoreResultsDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.MLScoreResultsDTO)
   })
 _sym_db.RegisterMessage(MLScoreResultsDTO)
 
 DoubleMatrixDTO = _reflection.GeneratedProtocolMessageType('DoubleMatrixDTO', (_message.Message,), {
   'DESCRIPTOR' : _DOUBLEMATRIXDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.DoubleMatrixDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.DoubleMatrixDTO)
   })
 _sym_db.RegisterMessage(DoubleMatrixDTO)
 
 DoubleVectorDTO = _reflection.GeneratedProtocolMessageType('DoubleVectorDTO', (_message.Message,), {
   'DESCRIPTOR' : _DOUBLEVECTORDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.DoubleVectorDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.DoubleVectorDTO)
   })
 _sym_db.RegisterMessage(DoubleVectorDTO)
 
 HistDTO = _reflection.GeneratedProtocolMessageType('HistDTO', (_message.Message,), {
   'DESCRIPTOR' : _HISTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.HistDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.HistDTO)
   })
 _sym_db.RegisterMessage(HistDTO)
 
 ColumnDistHistDTO = _reflection.GeneratedProtocolMessageType('ColumnDistHistDTO', (_message.Message,), {
   'DESCRIPTOR' : _COLUMNDISTHISTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.ColumnDistHistDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.ColumnDistHistDTO)
   })
 _sym_db.RegisterMessage(ColumnDistHistDTO)
 
 TextResultDTO = _reflection.GeneratedProtocolMessageType('TextResultDTO', (_message.Message,), {
   'DESCRIPTOR' : _TEXTRESULTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.TextResultDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.TextResultDTO)
   })
 _sym_db.RegisterMessage(TextResultDTO)
 
 TextColumnResultDTO = _reflection.GeneratedProtocolMessageType('TextColumnResultDTO', (_message.Message,), {
   'DESCRIPTOR' : _TEXTCOLUMNRESULTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.TextColumnResultDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.TextColumnResultDTO)
   })
 _sym_db.RegisterMessage(TextColumnResultDTO)
 
+TextScoreDTO = _reflection.GeneratedProtocolMessageType('TextScoreDTO', (_message.Message,), {
+  'DESCRIPTOR' : _TEXTSCOREDTO,
+  '__module__' : 'synthschemavalidationresult_pb2'
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.TextScoreDTO)
+  })
+_sym_db.RegisterMessage(TextScoreDTO)
+
+TextMetricDTO = _reflection.GeneratedProtocolMessageType('TextMetricDTO', (_message.Message,), {
+
+  'SubScoresEntry' : _reflection.GeneratedProtocolMessageType('SubScoresEntry', (_message.Message,), {
+    'DESCRIPTOR' : _TEXTMETRICDTO_SUBSCORESENTRY,
+    '__module__' : 'synthschemavalidationresult_pb2'
+    # @@protoc_insertion_point(class_scope:synthschemavalidation.TextMetricDTO.SubScoresEntry)
+    })
+  ,
+  'DESCRIPTOR' : _TEXTMETRICDTO,
+  '__module__' : 'synthschemavalidationresult_pb2'
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.TextMetricDTO)
+  })
+_sym_db.RegisterMessage(TextMetricDTO)
+_sym_db.RegisterMessage(TextMetricDTO.SubScoresEntry)
+
 SequenceResultDTO = _reflection.GeneratedProtocolMessageType('SequenceResultDTO', (_message.Message,), {
   'DESCRIPTOR' : _SEQUENCERESULTDTO,
   '__module__' : 'synthschemavalidationresult_pb2'
-  # @@protoc_insertion_point(class_scope:datakube.SequenceResultDTO)
+  # @@protoc_insertion_point(class_scope:synthschemavalidation.SequenceResultDTO)
   })
 _sym_db.RegisterMessage(SequenceResultDTO)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\nUcom.datomize.datomizer.backend.components.management.dto.synthschemavalidationserviceB\"SynthSchemaValidationServiceProtos'
@@ -199,52 +228,62 @@
   _TABLEVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._serialized_options = b'8\001'
   _DEPENDENCYVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._options = None
   _DEPENDENCYVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._serialized_options = b'8\001'
   _DOUBLEMATRIXDTO.fields_by_name['data']._options = None
   _DOUBLEMATRIXDTO.fields_by_name['data']._serialized_options = b'\020\001'
   _DOUBLEVECTORDTO.fields_by_name['data']._options = None
   _DOUBLEVECTORDTO.fields_by_name['data']._serialized_options = b'\020\001'
-  _ALGORITHMTYPE._serialized_start=3129
-  _ALGORITHMTYPE._serialized_end=3175
-  _METRICTYPE._serialized_start=3177
-  _METRICTYPE._serialized_end=3225
-  _SEQTYPE._serialized_start=3227
-  _SEQTYPE._serialized_end=3272
-  _SUMMARYDTO._serialized_start=47
-  _SUMMARYDTO._serialized_end=102
-  _SYNTHSCHEMAVALIDATIONRESULTDTO._serialized_start=105
-  _SYNTHSCHEMAVALIDATIONRESULTDTO._serialized_end=572
-  _SYNTHSCHEMAVALIDATIONRESULTDTO_MEASURESSUMMARYENTRY._serialized_start=518
-  _SYNTHSCHEMAVALIDATIONRESULTDTO_MEASURESSUMMARYENTRY._serialized_end=572
-  _TABLEVALIDATIONRESULTDTO._serialized_start=575
-  _TABLEVALIDATIONRESULTDTO._serialized_end=1278
-  _TABLEVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._serialized_start=1221
-  _TABLEVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._serialized_end=1278
-  _DEPENDENCYVALIDATIONRESULTDTO._serialized_start=1281
-  _DEPENDENCYVALIDATIONRESULTDTO._serialized_end=1737
-  _DEPENDENCYVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._serialized_start=1221
-  _DEPENDENCYVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._serialized_end=1278
-  _DETECTIONRESULTDTO._serialized_start=1740
-  _DETECTIONRESULTDTO._serialized_end=1897
-  _COVERAGERESULTDTO._serialized_start=1899
-  _COVERAGERESULTDTO._serialized_end=2020
-  _COVERAGERESULTNEWDTO._serialized_start=2022
-  _COVERAGERESULTNEWDTO._serialized_end=2100
-  _UTILITYRESULTDTO._serialized_start=2102
-  _UTILITYRESULTDTO._serialized_end=2222
-  _MLSCORERESULTSDTO._serialized_start=2225
-  _MLSCORERESULTSDTO._serialized_end=2410
-  _DOUBLEMATRIXDTO._serialized_start=2412
-  _DOUBLEMATRIXDTO._serialized_end=2475
-  _DOUBLEVECTORDTO._serialized_start=2477
-  _DOUBLEVECTORDTO._serialized_end=2526
-  _HISTDTO._serialized_start=2528
-  _HISTDTO._serialized_end=2573
-  _COLUMNDISTHISTDTO._serialized_start=2576
-  _COLUMNDISTHISTDTO._serialized_end=2716
-  _TEXTRESULTDTO._serialized_start=2718
-  _TEXTRESULTDTO._serialized_end=2800
-  _TEXTCOLUMNRESULTDTO._serialized_start=2802
-  _TEXTCOLUMNRESULTDTO._serialized_end=2905
-  _SEQUENCERESULTDTO._serialized_start=2908
-  _SEQUENCERESULTDTO._serialized_end=3127
+  _TEXTMETRICDTO_SUBSCORESENTRY._options = None
+  _TEXTMETRICDTO_SUBSCORESENTRY._serialized_options = b'8\001'
+  _ALGORITHMTYPE._serialized_start=4104
+  _ALGORITHMTYPE._serialized_end=4150
+  _METRICTYPE._serialized_start=4152
+  _METRICTYPE._serialized_end=4200
+  _TEXTTYPE._serialized_start=4202
+  _TEXTTYPE._serialized_end=4231
+  _SEQTYPE._serialized_start=4233
+  _SEQTYPE._serialized_end=4278
+  _SUMMARYDTO._serialized_start=60
+  _SUMMARYDTO._serialized_end=115
+  _SYNTHSCHEMAVALIDATIONRESULTDTO._serialized_start=118
+  _SYNTHSCHEMAVALIDATIONRESULTDTO._serialized_end=673
+  _SYNTHSCHEMAVALIDATIONRESULTDTO_MEASURESSUMMARYENTRY._serialized_start=619
+  _SYNTHSCHEMAVALIDATIONRESULTDTO_MEASURESSUMMARYENTRY._serialized_end=673
+  _TABLEVALIDATIONRESULTDTO._serialized_start=676
+  _TABLEVALIDATIONRESULTDTO._serialized_end=1614
+  _TABLEVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._serialized_start=1557
+  _TABLEVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._serialized_end=1614
+  _DEPENDENCYVALIDATIONRESULTDTO._serialized_start=1617
+  _DEPENDENCYVALIDATIONRESULTDTO._serialized_end=2151
+  _DEPENDENCYVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._serialized_start=1557
+  _DEPENDENCYVALIDATIONRESULTDTO_MEASURETOTALSCORESENTRY._serialized_end=1614
+  _DETECTIONRESULTDTO._serialized_start=2154
+  _DETECTIONRESULTDTO._serialized_end=2337
+  _COVERAGERESULTDTO._serialized_start=2340
+  _COVERAGERESULTDTO._serialized_end=2487
+  _COVERAGERESULTNEWDTO._serialized_start=2489
+  _COVERAGERESULTNEWDTO._serialized_end=2567
+  _UTILITYRESULTDTO._serialized_start=2570
+  _UTILITYRESULTDTO._serialized_end=2716
+  _MLSCORERESULTSDTO._serialized_start=2719
+  _MLSCORERESULTSDTO._serialized_end=2917
+  _DOUBLEMATRIXDTO._serialized_start=2919
+  _DOUBLEMATRIXDTO._serialized_end=2982
+  _DOUBLEVECTORDTO._serialized_start=2984
+  _DOUBLEVECTORDTO._serialized_end=3033
+  _HISTDTO._serialized_start=3035
+  _HISTDTO._serialized_end=3080
+  _COLUMNDISTHISTDTO._serialized_start=3083
+  _COLUMNDISTHISTDTO._serialized_end=3249
+  _TEXTRESULTDTO._serialized_start=3252
+  _TEXTRESULTDTO._serialized_end=3399
+  _TEXTCOLUMNRESULTDTO._serialized_start=3402
+  _TEXTCOLUMNRESULTDTO._serialized_end=3607
+  _TEXTSCOREDTO._serialized_start=3609
+  _TEXTSCOREDTO._serialized_end=3685
+  _TEXTMETRICDTO._serialized_start=3688
+  _TEXTMETRICDTO._serialized_end=3854
+  _TEXTMETRICDTO_SUBSCORESENTRY._serialized_start=3806
+  _TEXTMETRICDTO_SUBSCORESENTRY._serialized_end=3854
+  _SEQUENCERESULTDTO._serialized_start=3857
+  _SEQUENCERESULTDTO._serialized_end=4102
 # @@protoc_insertion_point(module_scope)
```

### Comparing `datomize-2.1.7/datomizer/utils/constants.py` & `datomize-2.3.7/datomizer/utils/constants.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/datomizer/utils/enhance_ml.py` & `datomize-2.3.7/datomizer/utils/enhance_ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,10 +37,10 @@
     PR_AUC = "PR_AUC"
 
 
 def map_enum_list(enum_list: []):
     return [obj.value for obj in enum_list]
 
 
-def assert_column_valid_for_eml(column: ColumnDTO) -> bool:
+def assert_column_valid_for_eml(column: ColumnDTO):
     assert column.role == Roles.LABEL.value, EML_TARGET_INVALID_ROLE
     assert 2 <= column.uniqueCount <= 10, EML_TARGET_INVALID_UNIQUE_COUNT
```

### Comparing `datomize-2.1.7/datomizer/utils/general.py` & `datomize-2.3.7/datomizer/utils/general.py`

 * *Files identical despite different names*

### Comparing `datomize-2.1.7/setup.py` & `datomize-2.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="datomize",
-    version="2.1.7",
+    version="2.3.7",
     license='Apache Software License (https://www.apache.org/licenses/LICENSE-2.0)',
     description="Datomize python client",
     packages=find_namespace_packages(),
     install_requires=[
         'requests', 'protobuf==3.19.4'
     ],
     url="https://datomize.github.io/datomizeSDK",
```

