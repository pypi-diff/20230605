# Comparing `tmp/autora-experiment-runner-experimentation-manager-firebase-1.0.0a4.tar.gz` & `tmp/autora-experiment-runner-experimentation-manager-firebase-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experiment-runner-experimentation-manager-firebase-1.0.0a4.tar", last modified: Sat May 27 19:37:48 2023, max compression
+gzip compressed data, was "autora-experiment-runner-experimentation-manager-firebase-1.0.1.tar", last modified: Mon Jun  5 15:00:15 2023, max compression
```

## Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4.tar` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.689347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/SweetPea.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/experiment_runner/experimentation_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/experiment_runner/experimentation_manager/firebase/
--rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-27 19:37:48.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-27 19:37:48.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 19:37:48.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-27 19:37:48.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 19:37:48.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/tests/test_experimentation_manager_firebase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.170091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 15:00:15.170091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/SweetPea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:00:15.170091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/experiment_runner/experimentation_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/experiment_runner/experimentation_manager/firebase/
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 15:00:15.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-05 15:00:15.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:00:15.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 15:00:15.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 15:00:15.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/tests/test_experimentation_manager_firebase.py
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.github/workflows/python-publish.yml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.gitignore` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.pre-commit-config.yaml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/PKG-INFO` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-experimentation-manager-firebase
-Version: 1.0.0a4
-Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observation between AutoRA and an experiment on Firebase.
+Version: 1.0.1
+Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observations between AutoRA and an experiment on Firebase.
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-experimentation-manager-firebase
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/README.md` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/SweetPea.ipynb` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/SweetPea.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/mkdocs/base.yml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/pyproject.toml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 # UPDATE THIS BEFORE PUBLISHING
 name = "autora-experiment-runner-experimentation-manager-firebase"
-description = "AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observation between AutoRA and an experiment on Firebase."
+description = "AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observations between AutoRA and an experiment on Firebase."
 authors = [{ name = "Younes Strittmatter", email = "younes_strittmatter@brown.edu" }]
 dynamic = ["version"]
 
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.8,<4"
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import time
 from typing import Any
 import numpy as np
 import warnings
 
 import firebase_admin
 from firebase_admin import credentials, firestore
+import json
 
-
-def _sequence_to_db_object(iterable):
+def _sequence_to_db_object(iterable, save=False):
     """
     Helper function to convert an array into a dictionary for a database
     Args:
         iterable: an iterable
 
     Returns:
         a dict with keys 0, 1, 2..
@@ -36,15 +36,15 @@
     for t in iterable:
         is_int64 = is_int64 or isinstance(t, np.int64)
         is_float64 = is_float64 or isinstance(t, np.float64)
     if is_int64:
         warnings.warn('Converting np.int64 to int to store in Firestore, may loose precision')
     if is_float64:
         warnings.warn('Converting np.float64 to float to store in Firestore, may loose precision')
-    return {i: int(t) if isinstance(t, np.integer) else float(t) if isinstance(t, np.floating) else t for i, t in enumerate(iterable)}
+    return {i: int(t) if isinstance(t, np.integer) else float(t) if isinstance(t, np.floating) else t if isinstance(t, dict) else json.dumps(t) for i, t in enumerate(iterable)}
 
 
 def _get_collection(
         collection_name: str,
         firebase_credentials: dict
 ):
     """
@@ -56,18 +56,20 @@
 
     Returns:
         the firebase collection
     """
     # get the firebase collection (name of the study most probably)
     if not firebase_admin._apps:
         cred = credentials.Certificate(firebase_credentials)
-        firebase_admin.initialize_app(cred)
+        app = firebase_admin.initialize_app(cred)
+    else:
+        app = firebase_admin.get_app()
     db = firestore.client()
 
-    return db.collection(f"{collection_name}")
+    return app, db.collection(f"{collection_name}")
 
 
 def _set_meta(
         seq_col: Any,
         condition_dict: dict,
         doc_meta: str = 'autora_meta',
         is_append: bool = False
@@ -108,17 +110,18 @@
     Args:
         collection_name: the name of the study as given in firebase
         condition: the condition to run
         firebase_credentials: dict with the credentials for firebase
         doc_meta: document to store metadata
         is_append: if true, append the conditions instead of resetting them
     """
-    seq_col = _get_collection(collection_name, firebase_credentials)
+    app, seq_col = _get_collection(collection_name, firebase_credentials)
     condition_dict = _sequence_to_db_object(condition)
     _set_meta(seq_col, condition_dict, doc_meta, is_append)
+    firebase_admin.delete_app(app)
 
 
 def __reset_col(
         parent_col,
         doc,
         col
 ):
@@ -221,17 +224,18 @@
         firebase_credentials: dict with the credentials for firebase
         doc_out: document to store out data
         doc_in: document to store in data
         col_observation: collection to store the observations
         col_condition: collection to store the conditions
         is_append: if true, append the conditions and observations instead of resetting them
     """
-    seq_col = _get_collection(collection_name, firebase_credentials)
+    app, seq_col = _get_collection(collection_name, firebase_credentials)
     condition_dict = _sequence_to_db_object(condition)
     _set_up_experiment_db(seq_col, condition_dict, doc_out, doc_in, col_observation, col_condition, is_append)
+    firebase_admin.delete_app(app)
 
 
 def send_conditions(
         collection_name: str,
         conditions: Any,
         firebase_credentials: dict,
         doc_meta: str = "autora_meta",
@@ -257,22 +261,24 @@
         is_append: if true, append the conditions, observations and meta-data instead of resetting them
     """
 
     # get the conditions with their indexes
     condition_dict = _sequence_to_db_object(conditions)
 
     # get the firebase collection
-    seq_col = _get_collection(collection_name, firebase_credentials)
+    app, seq_col = _get_collection(collection_name, firebase_credentials)
 
     # set the meta data
     _set_meta(seq_col, condition_dict, doc_meta, is_append)
 
     # setup db for conditions and observations
     _set_up_experiment_db(seq_col, condition_dict, doc_out, doc_in, col_observation, col_condition, is_append)
 
+    firebase_admin.delete_app(app)
+
 
 def get_observations(collection_name: str,
                      firebase_credentials: dict,
                      doc_out: str = "autora_out",
                      col_observation: str = "observations", ) -> Any:
     """
     get observations from firestore database
@@ -286,25 +292,28 @@
 
     Returns:
         observations
     """
 
     if not firebase_admin._apps:
         cred = credentials.Certificate(firebase_credentials)
-        firebase_admin.initialize_app(cred)
+        app = firebase_admin.initialize_app(cred)
+    else:
+        app = firebase_admin.get_app()
     db = firestore.client()
     seq_col = db.collection(f"{collection_name}")
 
     doc_ref_out = seq_col.document(doc_out)
 
     col_ref = doc_ref_out.collection(col_observation)
     docs = col_ref.stream()
     observations = {}
     for doc in docs:
         observations.update(doc.reference.get().to_dict())
+    firebase_admin.delete_app(app)
     return observations
 
 
 def check_firebase_status(
         collection_name: str, firebase_credentials: dict, time_out: int
 ) -> str:
     """
@@ -321,35 +330,43 @@
             (1) available -> no action needed, recruitment should be started (if paused)
             (2) finished -> collection of observations is finished
             (3) unavailable -> all conditions are running, recruitment should be paused
     """
 
     if not firebase_admin._apps:
         cred = credentials.Certificate(firebase_credentials)
-        firebase_admin.initialize_app(cred)
+        app = firebase_admin.initialize_app(cred)
+    else:
+        app = firebase_admin.get_app()
     db = firestore.client()
     seq_col = db.collection(f"{collection_name}")
 
     doc_ref_meta = seq_col.document("autora_meta")
     meta_data = doc_ref_meta.get().to_dict()
 
     finished = True
+    available = False
     for key, value in meta_data.items():
         # return available if there are conditions that haven't been started
         if value["start_time"] is None:
-            return "available"
+            firebase_admin.delete_app(app)
+            available = True
         else:
             if not value["finished"]:
                 unix_time_seconds = int(time.time())
                 time_from_started = unix_time_seconds - value["start_time"]
                 # check weather the started condition has timed out, if so, reset start_time and
-                # return available
+                # set available True
                 if time_from_started > time_out:
+                    firebase_admin.delete_app(app)
                     doc_ref_meta.update({key: {"start_time": None, "finished": False}})
-                    return "available"
+                    available = True
                 else:
                     finished = False
+    firebase_admin.delete_app()
+    if available:
+        return 'available'
     if finished:
         # if all start_times are set and have data, condition is finished
         return "finished"
     # if all start_times are set, but there is no data for all of them, pause the condition
     return "unavailable"
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-experimentation-manager-firebase
-Version: 1.0.0a4
-Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observation between AutoRA and an experiment on Firebase.
+Version: 1.0.1
+Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observations between AutoRA and an experiment on Firebase.
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-experimentation-manager-firebase
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/tests/README.md` & `autora-experiment-runner-experimentation-manager-firebase-1.0.1/tests/README.md`

 * *Files identical despite different names*

