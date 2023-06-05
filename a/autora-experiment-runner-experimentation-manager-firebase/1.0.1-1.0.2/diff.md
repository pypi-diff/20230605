# Comparing `tmp/autora-experiment-runner-experimentation-manager-firebase-1.0.1.tar.gz` & `tmp/autora-experiment-runner-experimentation-manager-firebase-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experiment-runner-experimentation-manager-firebase-1.0.1.tar", last modified: Mon Jun  5 15:00:15 2023, max compression
+gzip compressed data, was "autora-experiment-runner-experimentation-manager-firebase-1.0.2.tar", last modified: Mon Jun  5 15:20:13 2023, max compression
```

## Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1.tar` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.170091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 15:00:15.170091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/SweetPea.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:00:15.170091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/experiment_runner/experimentation_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/experiment_runner/experimentation_manager/firebase/
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 15:00:15.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-05 15:00:15.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:00:15.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 15:00:15.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 15:00:15.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:15.166091 autora-experiment-runner-experimentation-manager-firebase-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 15:00:05.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.1/tests/test_experimentation_manager_firebase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.961672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 15:20:13.961672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/SweetPea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:20:13.961672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/experiment_runner/experimentation_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/experiment_runner/experimentation_manager/firebase/
+-rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 15:20:13.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-05 15:20:13.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:20:13.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 15:20:13.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 15:20:13.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.961672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/tests/test_experimentation_manager_firebase.py
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/.github/workflows/python-publish.yml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/.gitignore` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/.pre-commit-config.yaml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/PKG-INFO` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-experimentation-manager-firebase
-Version: 1.0.1
+Version: 1.0.2
 Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observations between AutoRA and an experiment on Firebase.
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-experimentation-manager-firebase
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/README.md` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/docs/SweetPea.ipynb` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/SweetPea.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/mkdocs/base.yml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/pyproject.toml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,29 +344,27 @@
     meta_data = doc_ref_meta.get().to_dict()
 
     finished = True
     available = False
     for key, value in meta_data.items():
         # return available if there are conditions that haven't been started
         if value["start_time"] is None:
-            firebase_admin.delete_app(app)
             available = True
         else:
             if not value["finished"]:
                 unix_time_seconds = int(time.time())
                 time_from_started = unix_time_seconds - value["start_time"]
                 # check weather the started condition has timed out, if so, reset start_time and
                 # set available True
                 if time_from_started > time_out:
-                    firebase_admin.delete_app(app)
                     doc_ref_meta.update({key: {"start_time": None, "finished": False}})
                     available = True
                 else:
                     finished = False
-    firebase_admin.delete_app()
+    firebase_admin.delete_app(app)
     if available:
         return 'available'
     if finished:
         # if all start_times are set and have data, condition is finished
         return "finished"
     # if all start_times are set, but there is no data for all of them, pause the condition
     return "unavailable"
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-experimentation-manager-firebase
-Version: 1.0.1
+Version: 1.0.2
 Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observations between AutoRA and an experiment on Firebase.
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-experimentation-manager-firebase
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.1/tests/README.md` & `autora-experiment-runner-experimentation-manager-firebase-1.0.2/tests/README.md`

 * *Files identical despite different names*

