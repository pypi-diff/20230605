# Comparing `tmp/comet_llm-0.0.2.tar.gz` & `tmp/comet_llm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_llm-0.0.2.tar", last modified: Wed May 31 13:58:31 2023, max compression
+gzip compressed data, was "comet_llm-0.0.3.tar", last modified: Mon Jun  5 13:34:45 2023, max compression
```

## Comparing `comet_llm-0.0.2.tar` & `comet_llm-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:31.439604 comet_llm-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-31 13:58:31.439604 comet_llm-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 13:58:21.000000 comet_llm-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:58:31.439604 comet_llm-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-31 13:58:21.000000 comet_llm-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:31.435604 comet_llm-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:31.439604 comet_llm-0.0.2/src/comet_llm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:31.439604 comet_llm-0.0.2/src/comet_llm/experiment_api/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/experiment_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/experiment_api/comet_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/experiment_api/experiment_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/experiment_api/request_exception_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/experiment_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-31 13:58:21.000000 comet_llm-0.0.2/src/comet_llm/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:31.439604 comet_llm-0.0.2/src/comet_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 13:58:31.000000 comet_llm-0.0.2/src/comet_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:34:45.729216 comet_llm-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 13:34:45.729216 comet_llm-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 13:34:35.000000 comet_llm-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:34:45.729216 comet_llm-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-05 13:34:35.000000 comet_llm-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:34:45.721215 comet_llm-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:34:45.725216 comet_llm-0.0.3/src/comet_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:34:45.729216 comet_llm-0.0.3/src/comet_llm/experiment_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/experiment_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/experiment_api/comet_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/experiment_api/experiment_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/experiment_api/request_exception_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/experiment_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-05 13:34:35.000000 comet_llm-0.0.3/src/comet_llm/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:34:45.729216 comet_llm-0.0.3/src/comet_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 13:34:45.000000 comet_llm-0.0.3/src/comet_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 13:34:45.000000 comet_llm-0.0.3/src/comet_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:34:45.000000 comet_llm-0.0.3/src/comet_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:34:45.000000 comet_llm-0.0.3/src/comet_llm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 13:34:45.000000 comet_llm-0.0.3/src/comet_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 13:34:45.000000 comet_llm-0.0.3/src/comet_llm.egg-info/top_level.txt
```

### Comparing `comet_llm-0.0.2/PKG-INFO` & `comet_llm-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_llm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Comet logger for LLM
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_llm-0.0.2/setup.py` & `comet_llm-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,11 +50,11 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="comet_llm",
     name="comet_llm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.ml",
-    version="0.0.2",
+    version="0.0.3",
     zip_safe=False,
     license="Proprietary",
 )
```

### Comparing `comet_llm-0.0.2/src/comet_llm/__init__.py` & `comet_llm-0.0.3/src/comet_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.2/src/comet_llm/api.py` & `comet_llm-0.0.3/src/comet_llm/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,36 +10,33 @@
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 import io
 import json
-from typing import Any, Dict, Optional, Union
+from typing import Dict, Optional, Union
 
-import flatten_dict
-
-from . import convert, experiment_api, experiment_info
+from . import convert, experiment_api, experiment_info, preprocess
 
 ASSET_FORMAT_VERSION = 3
 
 
 def log_prompt(
     prompt: str,
     output: str,
     workspace: Optional[str] = None,
     project: Optional[str] = None,
     api_key: Optional[str] = None,
     prompt_template: Optional[str] = None,
     prompt_template_variables: Optional[
         Dict[str, Union[str, bool, float, None]]
     ] = None,
-    metadata: Optional[Dict[str, str]] = None,
-    start_timestamp: Optional[float] = None,
-    end_timestamp: Optional[float] = None,
+    metadata: Optional[Dict[str, Union[str, bool, float, None]]] = None,
+    timestamp: Optional[float] = None,
     duration: Optional[float] = None,
 ) -> None:
     """
     Logs a single prompt and output to Comet platform.
 
     Args:
         prompt: str (required) input prompt to LLM.
@@ -48,16 +45,15 @@
         project: str (optional) project name to create in comet workspace.
         api_key: str (optional) comet API key.
         prompt_template: str (optional) user-defined template used for creating a prompt.
         prompt_template_variables: Dict[str, str] (optional) dictionary with data used
             in prompt_template to build a prompt.
         metadata: Dict[str, Union[str, bool, float, None]] (optional) user-defined
             dictionary with additional metadata to the call.
-        start_timestamp: float (optional) start timestamp of prompt call
-        end_timestamp: float (optional) end timestamp of prompt call
+        timestamp: float (optional) timestamp of prompt call in seconds
         duration: float (optional) duration of prompt call
 
     Example:
 
     ```python
     log_prompt(
         prompt="Answer the question and if the question can't be answered, say \"I don't know\"\n\n---\n\nQuestion: What is your name?\nAnswer:",
@@ -83,14 +79,16 @@
     Returns: None.
     """
     LOG_PROMPT_API_KEY_NOT_FOUND_MESSAGE = """
     CometLLM requires an API key. Please provide it as the
     api_key argument to log_prompt or as an environment
     variable named COMET_API_KEY
     """
+    timestamp = preprocess.timestamp(timestamp)
+
     info = experiment_info.get(
         api_key,
         workspace,
         project,
         api_key_not_found_message=LOG_PROMPT_API_KEY_NOT_FOUND_MESSAGE,
     )
     experiment_api_ = experiment_api.ExperimentAPI(
@@ -99,40 +97,41 @@
 
     call_data = convert.call_data_to_dict(
         prompt=prompt,
         outputs=output,
         metadata=metadata,
         prompt_template=prompt_template,
         prompt_template_variables=prompt_template_variables,
-        start_timestamp=start_timestamp,
-        end_timestamp=end_timestamp,
+        start_timestamp=timestamp,
+        end_timestamp=timestamp,
         duration=duration,
     )
 
     asset_data = {
         "version": ASSET_FORMAT_VERSION,
         "chain_nodes": [call_data],
         "chain_inputs": {
             "final_prompt": prompt,
             "prompt_template": prompt_template,
             "prompt_template_variables": prompt_template_variables,
         },
         "chain_outputs": {"output": output},
         "category": "single_prompt",
-        "metadata": {},
-        "start_timestamp": start_timestamp,
-        "end_timestamp": end_timestamp,
+        "metadata": "the-metadata",
+        "start_timestamp": timestamp,
+        "end_timestamp": timestamp,
         "chain_duration": duration,
     }
 
     experiment_api_.log_asset_with_io(
         name="comet_llm_data.json",
         file=io.StringIO(json.dumps(asset_data)),
         asset_type="llm_data",
     )
 
-    parameters = convert.chain_metadata_to_flat_dict(
-        metadata, start_timestamp, end_timestamp, duration
-    )
+    if duration is not None:
+        experiment_api_.log_metric("chain_duration", duration)
+
+    parameters = convert.chain_metadata_to_flat_parameters(metadata)
 
     for name, value in parameters.items():
         experiment_api_.log_parameter(name, value)
```

### Comparing `comet_llm-0.0.2/src/comet_llm/config.py` & `comet_llm-0.0.3/src/comet_llm/config.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.2/src/comet_llm/convert.py` & `comet_llm-0.0.3/src/comet_llm/convert.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,30 +43,19 @@
         "start_timestamp": start_timestamp,
         "end_timestamp": end_timestamp,
         "parent_ids": [],
         "metadata": metadata,
     }
 
 
-def chain_metadata_to_flat_dict(
-    metadata: Optional[Dict[str, Any]],
-    start_timestamp: Optional[float],
-    end_timestamp: Optional[float],
-    duration: Optional[float],
+def chain_metadata_to_flat_parameters(
+    metadata: Optional[Dict[str, Any]]
 ) -> Dict[str, Any]:
-
-    timestamp_parameters = {
-        "start_timestamp": start_timestamp,
-        "end_timestamp": end_timestamp,
-        "chain_duration": duration,
-    }
     metadata_parameters = (
         flatten_dict.flatten(metadata, reducer="dot") if metadata is not None else {}
     )
 
     result = {
-        key: value
-        for key, value in {**timestamp_parameters, **metadata_parameters}.items()
-        if value is not None
+        key: value for key, value in metadata_parameters.items() if value is not None
     }
 
     return result
```

### Comparing `comet_llm-0.0.2/src/comet_llm/exceptions.py` & `comet_llm-0.0.3/src/comet_llm/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.2/src/comet_llm/experiment_api/__init__.py` & `comet_llm-0.0.3/src/comet_llm/experiment_api/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.2/src/comet_llm/experiment_api/comet_api_client.py` & `comet_llm-0.0.3/src/comet_llm/experiment_api/comet_api_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -52,14 +52,27 @@
             json={
                 "experimentKey": experiment_key,
                 "parameterName": name,
                 "parameterValue": value,
             },
         )
 
+    def log_experiment_metric(
+        self, experiment_key: str, name: str, value: JSONEncodable
+    ) -> ResponseContent:
+        return self._request(
+            "POST",
+            "/api/rest/v2/write/experiment/metric",
+            json={
+                "experimentKey": experiment_key,
+                "metricName": name,
+                "metricValue": value,
+            },
+        )
+
     def log_experiment_asset_with_io(
         self,
         experiment_key: str,
         name: str,
         file: IO,
         asset_type: str,
         extension: Optional[str] = None,
```

### Comparing `comet_llm-0.0.2/src/comet_llm/experiment_api/experiment_api.py` & `comet_llm-0.0.3/src/comet_llm/experiment_api/experiment_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,7 +38,10 @@
             self._experiment_key, name=name, file=file, asset_type=asset_type
         )
 
     def log_parameter(self, name: str, value: Any) -> None:
         self._client.log_experiment_parameter(
             self._experiment_key, name=name, value=value
         )
+
+    def log_metric(self, name: str, value: Any) -> None:
+        self._client.log_experiment_metric(self._experiment_key, name=name, value=value)
```

### Comparing `comet_llm-0.0.2/src/comet_llm/experiment_api/request_exception_wrapper.py` & `comet_llm-0.0.3/src/comet_llm/experiment_api/request_exception_wrapper.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.2/src/comet_llm/experiment_info.py` & `comet_llm-0.0.3/src/comet_llm/experiment_info.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.2/src/comet_llm/types.py` & `comet_llm-0.0.3/src/comet_llm/types.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.2/src/comet_llm.egg-info/PKG-INFO` & `comet_llm-0.0.3/src/comet_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet-llm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Comet logger for LLM
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_llm-0.0.2/src/comet_llm.egg-info/SOURCES.txt` & `comet_llm-0.0.3/src/comet_llm.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 README.md
 setup.py
 src/comet_llm/__init__.py
 src/comet_llm/api.py
 src/comet_llm/config.py
 src/comet_llm/convert.py
+src/comet_llm/datetimes.py
 src/comet_llm/exceptions.py
 src/comet_llm/experiment_info.py
+src/comet_llm/preprocess.py
 src/comet_llm/types.py
 src/comet_llm.egg-info/PKG-INFO
 src/comet_llm.egg-info/SOURCES.txt
 src/comet_llm.egg-info/dependency_links.txt
 src/comet_llm.egg-info/not-zip-safe
 src/comet_llm.egg-info/requires.txt
 src/comet_llm.egg-info/top_level.txt
```

