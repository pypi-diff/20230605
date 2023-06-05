# Comparing `tmp/tab2neo-1.3.0.0.tar.gz` & `tmp/tab2neo-1.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tab2neo-1.3.0.0.tar", last modified: Fri Jun  2 14:24:53 2023, max compression
+gzip compressed data, was "tab2neo-1.3.0.1.tar", last modified: Mon Jun  5 08:02:59 2023, max compression
```

## Comparing `tab2neo-1.3.0.0.tar` & `tab2neo-1.3.0.1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:24:53.046901 tab2neo-1.3.0.0/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    11357 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/LICENSE
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    18778 2023-06-02 14:24:53.042901 tab2neo-1.3.0.0/PKG-INFO
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     5418 2023-06-02 13:00:16.000000 tab2neo-1.3.0.0/README.md
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:24:52.926901 tab2neo-1.3.0.0/data_loaders/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      241 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/data_loaders/__init__.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     3401 2023-02-21 08:21:40.000000 tab2neo-1.3.0.0/data_loaders/azure_data_loader.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    18843 2023-04-26 08:28:43.000000 tab2neo-1.3.0.0/data_loaders/file_data_loader.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     1492 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/data_loaders/hive_data_loader.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     1157 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/data_loaders/sql_server_data_loader.py
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:24:52.930901 tab2neo-1.3.0.0/data_providers/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       54 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/data_providers/__init__.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    10972 2023-06-02 13:00:16.000000 tab2neo-1.3.0.0/data_providers/data_provider.py
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:24:52.978901 tab2neo-1.3.0.0/derivation_method/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      229 2023-06-02 13:00:16.000000 tab2neo-1.3.0.0/derivation_method/__init__.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)   103924 2023-06-02 14:16:57.000000 tab2neo-1.3.0.0/derivation_method/action.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    68853 2023-06-02 13:00:16.000000 tab2neo-1.3.0.0/derivation_method/derivation_method.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     3784 2023-06-02 13:00:16.000000 tab2neo-1.3.0.0/derivation_method/method.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     3223 2023-06-02 13:00:16.000000 tab2neo-1.3.0.0/derivation_method/predict_links.cql
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     1043 2023-06-02 13:00:16.000000 tab2neo-1.3.0.0/derivation_method/predict_output_classes.cql
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    48787 2023-06-02 14:16:57.000000 tab2neo-1.3.0.0/derivation_method/super_method.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    10250 2023-06-02 13:00:17.000000 tab2neo-1.3.0.0/derivation_method/utils.py
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:24:52.994901 tab2neo-1.3.0.0/logger/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)        0 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/logger/__init__.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     1217 2023-02-21 08:21:40.000000 tab2neo-1.3.0.0/logger/logger.py
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:24:53.002901 tab2neo-1.3.0.0/model_appliers/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       53 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/model_appliers/__init__.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    29312 2023-06-02 13:00:17.000000 tab2neo-1.3.0.0/model_appliers/model_applier.py
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:24:53.010901 tab2neo-1.3.0.0/model_managers/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       53 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/model_managers/__init__.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    55794 2023-06-02 13:00:17.000000 tab2neo-1.3.0.0/model_managers/model_manager.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      103 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/pyproject.toml
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:24:53.022901 tab2neo-1.3.0.0/query_builders/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       53 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/query_builders/__init__.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    40776 2023-04-26 08:28:43.000000 tab2neo-1.3.0.0/query_builders/query_builder.py
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      544 2023-01-18 16:31:33.000000 tab2neo-1.3.0.0/requirements.txt
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       38 2023-06-02 14:24:53.046901 tab2neo-1.3.0.0/setup.cfg
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)     2337 2023-06-02 13:00:17.000000 tab2neo-1.3.0.0/setup.py
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:24:53.034901 tab2neo-1.3.0.0/tab2neo.egg-info/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    18778 2023-06-02 14:24:52.000000 tab2neo-1.3.0.0/tab2neo.egg-info/PKG-INFO
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      950 2023-06-02 14:24:52.000000 tab2neo-1.3.0.0/tab2neo.egg-info/SOURCES.txt
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)        1 2023-06-02 14:24:52.000000 tab2neo-1.3.0.0/tab2neo.egg-info/dependency_links.txt
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)      544 2023-06-02 14:24:52.000000 tab2neo-1.3.0.0/tab2neo.egg-info/requires.txt
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)       98 2023-06-02 14:24:52.000000 tab2neo-1.3.0.0/tab2neo.egg-info/top_level.txt
-drwxrwxr-x   0 wm698947  (1006) wm698947  (1006)        0 2023-06-02 14:24:53.038901 tab2neo-1.3.0.0/tests/
--rw-rw-r--   0 wm698947  (1006) wm698947  (1006)    11269 2023-06-02 13:00:17.000000 tab2neo-1.3.0.0/tests/test_comparison_utilities.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 08:02:59.487385 tab2neo-1.3.0.1/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11357 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/LICENSE
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11844 2023-06-05 08:02:59.487385 tab2neo-1.3.0.1/PKG-INFO
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     5418 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/README.md
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 08:02:59.471385 tab2neo-1.3.0.1/data_loaders/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      241 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/data_loaders/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3401 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/data_loaders/azure_data_loader.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    18843 2023-04-27 08:50:20.000000 tab2neo-1.3.0.1/data_loaders/file_data_loader.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1492 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/data_loaders/hive_data_loader.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1157 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/data_loaders/sql_server_data_loader.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 08:02:59.471385 tab2neo-1.3.0.1/data_providers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       54 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/data_providers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10972 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/data_providers/data_provider.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 08:02:59.479385 tab2neo-1.3.0.1/derivation_method/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      229 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/derivation_method/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)   103938 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/derivation_method/action.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    68853 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/derivation_method/derivation_method.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3784 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/derivation_method/method.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3223 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/derivation_method/predict_links.cql
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1043 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/derivation_method/predict_output_classes.cql
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    48787 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/derivation_method/super_method.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10250 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/derivation_method/utils.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 08:02:59.479385 tab2neo-1.3.0.1/logger/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        0 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/logger/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1217 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/logger/logger.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 08:02:59.479385 tab2neo-1.3.0.1/model_appliers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/model_appliers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    29312 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/model_appliers/model_applier.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 08:02:59.483385 tab2neo-1.3.0.1/model_managers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/model_managers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    55794 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/model_managers/model_manager.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      103 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/pyproject.toml
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 08:02:59.483385 tab2neo-1.3.0.1/query_builders/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-04-21 05:47:21.000000 tab2neo-1.3.0.1/query_builders/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    40776 2023-04-27 08:50:20.000000 tab2neo-1.3.0.1/query_builders/query_builder.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       38 2023-06-05 08:02:59.487385 tab2neo-1.3.0.1/setup.cfg
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2318 2023-06-05 08:01:25.000000 tab2neo-1.3.0.1/setup.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 08:02:59.487385 tab2neo-1.3.0.1/tab2neo.egg-info/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11844 2023-06-05 08:02:59.000000 tab2neo-1.3.0.1/tab2neo.egg-info/PKG-INFO
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      933 2023-06-05 08:02:59.000000 tab2neo-1.3.0.1/tab2neo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        1 2023-06-05 08:02:59.000000 tab2neo-1.3.0.1/tab2neo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      544 2023-06-05 08:02:59.000000 tab2neo-1.3.0.1/tab2neo.egg-info/requires.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       98 2023-06-05 08:02:59.000000 tab2neo-1.3.0.1/tab2neo.egg-info/top_level.txt
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 08:02:59.487385 tab2neo-1.3.0.1/tests/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11269 2023-06-05 07:59:59.000000 tab2neo-1.3.0.1/tests/test_comparison_utilities.py
```

### Comparing `tab2neo-1.3.0.0/LICENSE` & `tab2neo-1.3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/README.md` & `tab2neo-1.3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/data_loaders/azure_data_loader.py` & `tab2neo-1.3.0.1/data_loaders/azure_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/data_loaders/file_data_loader.py` & `tab2neo-1.3.0.1/data_loaders/file_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/data_loaders/hive_data_loader.py` & `tab2neo-1.3.0.1/data_loaders/hive_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/data_loaders/sql_server_data_loader.py` & `tab2neo-1.3.0.1/data_loaders/sql_server_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/data_providers/data_provider.py` & `tab2neo-1.3.0.1/data_providers/data_provider.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/derivation_method/action.py` & `tab2neo-1.3.0.1/derivation_method/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1152,40 +1152,40 @@
         logger.info(f"{len(self.df)} records in modified data")
         logger.debug(f"DataFrame: \n{self.df.to_string(max_rows=10)}")
 
         # make a request to the cldgitapi for commit id
 
         # only do this if the repo exists
         if self.meta.get("github_repo") is not None:
-            token = Fernet(os.environ.get('CLDGITAPI_ENCRYPTION_KEY')).encrypt(os.getenv('GIT_TOKEN').encode())
+            token = Fernet(os.environ.get('CLDGITAPI_ENCRYPTION_KEY')).encrypt(github_token.encode())
             headers = {'Content-Type': 'application/json', 'Accept': 'application/json'}
             gitapi_url = os.getenv('CLD_GIT_API_HOST')
             endpoint = 'get_commit'
 
             if self.meta.get('lang', '').lower() in ['py', 'python']:
                 extension = 'py'
             elif self.meta.get('lang', '').lower() == 'r':
                 extension = 'R'
             else:
                 raise KeyError(f"Expected property 'lang' to be 'python', 'Python', 'py', 'r' or 'R'. It was {self.meta.get('lang', '')}")
 
-            file_path = f'{self.meta.get("repo_scripts_path")}/{self.meta.get("package")}'
+            file_path = f'{self.meta.get("repo_scripts_path")}/{self.meta.get("package")}.{extension}'
 
             json_ = { 'repo': self.meta.get("github_repo"), 'branch': github_branch, 'base_url': github_base_url, 'file_path': file_path}
 
             # print to input logs
             logger.info(f'calling gitapi at {gitapi_url} to request latest commit_id for file {file_path} in repo {self.meta.get("github_repo")}')
 
             # api call 
             commit_resp = requests.get(url=f'{gitapi_url}/{endpoint}/', params={'token': token}, headers=headers, json=json_)
             response_content = commit_resp.json()
             try:
                 assert commit_resp.status_code == 200, f'Status code {commit_resp.status_code}'
             except AssertionError as err:
-                logger.error(resp.get('detail'))
+                logger.error(response_content.get('detail'))
                 raise err
             else:
                 commit_id = response_content.get('commit_id')
 
             # print output to logs and check response code
             logger.info(f"Retrieved commit_id: {commit_id}")
```

### Comparing `tab2neo-1.3.0.0/derivation_method/derivation_method.py` & `tab2neo-1.3.0.1/derivation_method/derivation_method.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/derivation_method/method.py` & `tab2neo-1.3.0.1/derivation_method/method.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/derivation_method/predict_links.cql` & `tab2neo-1.3.0.1/derivation_method/predict_links.cql`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/derivation_method/predict_output_classes.cql` & `tab2neo-1.3.0.1/derivation_method/predict_output_classes.cql`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/derivation_method/super_method.py` & `tab2neo-1.3.0.1/derivation_method/super_method.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/derivation_method/utils.py` & `tab2neo-1.3.0.1/derivation_method/utils.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/logger/logger.py` & `tab2neo-1.3.0.1/logger/logger.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/model_appliers/model_applier.py` & `tab2neo-1.3.0.1/model_appliers/model_applier.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/model_managers/model_manager.py` & `tab2neo-1.3.0.1/model_managers/model_manager.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/query_builders/query_builder.py` & `tab2neo-1.3.0.1/query_builders/query_builder.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/requirements.txt` & `tab2neo-1.3.0.1/tab2neo.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.0/setup.py` & `tab2neo-1.3.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import setuptools
 import os
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
 def read_text(file_name: str):
     return open(os.path.join(file_name)).read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 required = []
@@ -26,18 +23,18 @@
             print('Dependency to a git repository should have the format:')
             print('git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name')
     else:
         required.append(line)
 
 setuptools.setup(
     name="tab2neo",                         # This is the name of the package
-    version="1.3.0.0",                      # Release.Major Feature.Minor Feature.Bug Fix
+    version="1.3.0.1",                      # Release.Major Feature.Minor Feature.Bug Fix
     author="Alexey Kuznetsov",              # Full name of the author
     description="Clinical Linked Data: High-level Python classes to load, model and reshape tabular data imported into Neo4j database",
-    long_description=long_description,      # Long description read from the the readme file
+    long_description="https://github.com/GSK-Biostatistics/tab2neo/blob/main/README.md",      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(include=[
         "logger",
         "analysis_metadata",
         "derivation_method",
         "data_loaders",
         "data_providers",
```

### Comparing `tab2neo-1.3.0.0/tab2neo.egg-info/SOURCES.txt` & `tab2neo-1.3.0.1/tab2neo.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-requirements.txt
 setup.py
 data_loaders/__init__.py
 data_loaders/azure_data_loader.py
 data_loaders/file_data_loader.py
 data_loaders/hive_data_loader.py
 data_loaders/sql_server_data_loader.py
 data_providers/__init__.py
```

### Comparing `tab2neo-1.3.0.0/tests/test_comparison_utilities.py` & `tab2neo-1.3.0.1/tests/test_comparison_utilities.py`

 * *Files identical despite different names*

