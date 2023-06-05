# Comparing `tmp/hcai-nova-server-0.1.7.tar.gz` & `tmp/hcai-nova-server-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-0.1.7.tar", last modified: Fri Jun  2 12:26:41 2023, max compression
+gzip compressed data, was "hcai-nova-server-0.1.8.tar", last modified: Mon Jun  5 06:53:30 2023, max compression
```

## Comparing `hcai-nova-server-0.1.7.tar` & `hcai-nova-server-0.1.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.265701 hcai-nova-server-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9863 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 12:26:41.265701 hcai-nova-server-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:53:30.318303 hcai-nova-server-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-05 06:53:30.318303 hcai-nova-server-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:53:30.314303 hcai-nova-server-0.1.8/hcai_nova_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-05 06:53:30.000000 hcai-nova-server-0.1.8/hcai_nova_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-06-05 06:53:30.000000 hcai-nova-server-0.1.8/hcai_nova_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 06:53:30.000000 hcai-nova-server-0.1.8/hcai_nova_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-05 06:53:30.000000 hcai-nova-server-0.1.8/hcai_nova_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-05 06:53:30.000000 hcai-nova-server-0.1.8/hcai_nova_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-05 06:53:30.000000 hcai-nova-server-0.1.8/hcai_nova_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:53:30.314303 hcai-nova-server-0.1.8/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:53:30.318303 hcai-nova-server-0.1.8/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9818 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7072 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:53:30.318303 hcai-nova-server-0.1.8/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 06:53:30.318303 hcai-nova-server-0.1.8/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-05 06:53:30.318303 hcai-nova-server-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-05 06:53:16.000000 hcai-nova-server-0.1.8/setup.py
```

### Comparing `hcai-nova-server-0.1.7/PKG-INFO` & `hcai-nova-server-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server
-Version: 0.1.7
+Version: 0.1.8
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-0.1.7/hcai_nova_server.egg-info/PKG-INFO` & `hcai-nova-server-0.1.8/hcai_nova_server.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server
-Version: 0.1.7
+Version: 0.1.8
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-0.1.7/hcai_nova_server.egg-info/SOURCES.txt` & `hcai-nova-server-0.1.8/hcai_nova_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/route/cancel.py` & `hcai-nova-server-0.1.8/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/route/explain.py` & `hcai-nova-server-0.1.8/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/route/extract.py` & `hcai-nova-server-0.1.8/nova_server/route/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,54 +5,54 @@
     dataset_utils,
     thread_utils,
     status_utils,
     log_utils,
     import_utils,
 )
 from nova_server.utils.key_utils import get_key_from_request_form
-from flask import current_app
 from nova_server.utils.thread_utils import THREADS
 from nova_server.utils.status_utils import update_progress
 from pathlib import Path, PureWindowsPath
 from nova_utils.db_utils.nova_types import DataTypes
 from nova_utils.ssi_utils.ssi_xml_utils import Chain, ChainLink
 from nova_utils.ssi_utils.ssi_stream_utils import Stream, Chunk, FileTypes, NPDataTypes
 from importlib.machinery import SourceFileLoader
 from hcai_datasets.hcai_nova_dynamic.hcai_nova_dynamic_iterable import (
     HcaiNovaDynamicIterable,
 )
 import ffmpegio
 import numpy as np
 from nova_server.utils import db_utils
-
-
+from flask import current_app
+import os
 extract = Blueprint("extract", __name__)
 
 
 @extract.route("/extract", methods=["POST"])
 def extract_thread():
     if request.method == "POST":
         request_form = request.form.to_dict()
         key = get_key_from_request_form(request_form)
-        thread = extract_data(request_form, current_app._get_current_object())
+        thread = extract_data(request_form)
         status_utils.add_new_job(key)
         data = {"success": "true"}
         thread.start()
         THREADS[key] = thread
         return jsonify(data)
 
 
 @thread_utils.ml_thread_wrapper
-def extract_data(request_form, app_context):
+def extract_data(request_form):
 
     # Initialize
+    cml_dir = os.environ["NOVA_CML_DIR"]
+    data_dir = os.environ["NOVA_DATA_DIR"]
+
     key = get_key_from_request_form(request_form)
     logger = log_utils.get_logger_for_thread(key)
-    cml_dir = app_context.config["CML_DIR"]
-    data_dir = app_context.config["DATA_DIR"]
 
     chain_file_path = Path(cml_dir).joinpath(
         PureWindowsPath(request_form["chainFilePath"])
     )
 
     log_conform_request = dict(request_form)
     log_conform_request["password"] = "---"
```

### Comparing `hcai-nova-server-0.1.7/nova_server/route/log.py` & `hcai-nova-server-0.1.8/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/route/predict.py` & `hcai-nova-server-0.1.8/nova_server/route/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This file contains the general logic for predicting annotations to the nova database"""
 import copy
+import os
 from pathlib import Path, PureWindowsPath
 from nova_server.utils import db_utils
 from flask import Blueprint, request, jsonify
 from nova_utils.ssi_utils.ssi_xml_utils import Trainer
 from importlib.machinery import SourceFileLoader
 from nova_server.utils.thread_utils import THREADS
 from nova_server.utils.status_utils import update_progress
@@ -15,51 +16,51 @@
     dataset_utils,
     import_utils,
 )
 from hcai_datasets.hcai_nova_dynamic.hcai_nova_dynamic_iterable import (
     HcaiNovaDynamicIterable,
 )
 from nova_utils.interfaces.server_module import Trainer as iTrainer
-from flask import current_app
 
 predict = Blueprint("predict", __name__)
 
 
 @predict.route("/predict", methods=["POST"])
 def predict_thread():
     if request.method == "POST":
         request_form = request.form.to_dict()
         key = get_key_from_request_form(request_form)
-        thread = predict_data(request_form, current_app._get_current_object())
+        thread = predict_data(request_form)
         status_utils.add_new_job(key)
         data = {"success": "true"}
         thread.start()
         THREADS[key] = thread
         return jsonify(data)
 
 
 @thread_utils.ml_thread_wrapper
-def predict_data(request_form, app_context):
+def predict_data(request_form):
     key = get_key_from_request_form(request_form)
     logger = log_utils.get_logger_for_thread(key)
-    cml_dir = app_context.config["CML_DIR"]
-    data_dir = app_context.config["DATA_DIR"]
+
+    cml_dir = os.environ["NOVA_CML_DIR"]
+    data_dir = os.environ["NOVA_DATA_DIR"]
 
     log_conform_request = dict(request_form)
     log_conform_request["password"] = "---"
 
     logger.info("Action 'Predict' started.")
     status_utils.update_status(key, status_utils.JobStatus.RUNNING)
     trainer_file_path = Path(cml_dir).joinpath(
         PureWindowsPath(request_form["trainerFilePath"])
     )
     trainer = Trainer()
 
     if not trainer_file_path.is_file():
-        logger.error("Trainer file not available!")
+        logger.error(f"Trainer file not available: {trainer_file_path}")
         status_utils.update_status(key, status_utils.JobStatus.ERROR)
         return None
     else:
         trainer.load_from_file(trainer_file_path)
         logger.info("Trainer successfully loaded.")
 
     if not trainer.model_script_path:
```

### Comparing `hcai-nova-server-0.1.7/nova_server/route/status.py` & `hcai-nova-server-0.1.8/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/route/train.py` & `hcai-nova-server-0.1.8/nova_server/route/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         log_conform_request = dict(request_form)
         log_conform_request['password'] = '---'
 
         logger.info("Action 'Train' started.")
         trainer = Trainer()
 
         if not trainer_file_path.is_file():
-            logger.error("Trainer file not available!")
+            logger.error(f"Trainer file not available: {trainer_file_path}")
             status_utils.update_status(key, status_utils.JobStatus.ERROR)
             return None
         else:
             trainer.load_from_file(trainer_file_path)
             logger.info("Trainer successfully loaded.")
```

### Comparing `hcai-nova-server-0.1.7/nova_server/utils/dataset_utils.py` & `hcai-nova-server-0.1.8/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/utils/db_utils.py` & `hcai-nova-server-0.1.8/nova_server/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/utils/explain_utils.py` & `hcai-nova-server-0.1.8/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/utils/import_utils.py` & `hcai-nova-server-0.1.8/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/utils/key_utils.py` & `hcai-nova-server-0.1.8/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/utils/log_utils.py` & `hcai-nova-server-0.1.8/nova_server/utils/log_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 import threading
-import pathlib
+from pathlib import Path
+import os
 from nova_server.utils import status_utils
-
+from flask import current_app
 
 LOGS = {}
 
 
 def get_logfile_name_for_thread(log_key):
     return log_key + "-job_" + threading.current_thread().name
 
 
 def get_log_path_for_thread(log_key):
     name = get_logfile_name_for_thread(log_key)
-    # TODO: add  dynamic log path from config
-    return pathlib.Path(__file__).parent.parent / "logs" / (name + ".log")
+    log_dir = os.environ["NOVA_CML_DIR"]
+    return Path(log_dir) / (name + ".log")
 
 
 def init_logger(logger, log_key):
     print("Init logger" + str(threading.current_thread().name))
     try:
         log_path = get_log_path_for_thread(log_key)
         status_utils.set_log_path(log_key, log_path)
```

### Comparing `hcai-nova-server-0.1.7/nova_server/utils/status_utils.py` & `hcai-nova-server-0.1.8/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/nova_server/utils/thread_utils.py` & `hcai-nova-server-0.1.8/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.7/setup.py` & `hcai-nova-server-0.1.8/setup.py`

 * *Files identical despite different names*

