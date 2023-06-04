# Comparing `tmp/omnata_plugin_runtime-0.1.3.tar.gz` & `tmp/omnata_plugin_runtime-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_plugin_runtime-0.1.3.tar", max compression
+gzip compressed data, was "omnata_plugin_runtime-0.1.4.tar", max compression
```

## Comparing `omnata_plugin_runtime-0.1.3.tar` & `omnata_plugin_runtime-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    26526 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/LICENSE
--rw-r--r--   0        0        0      296 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/README.md
--rw-r--r--   0        0        0      826 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1213 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/__init__.py
--rw-r--r--   0        0        0     3277 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/api.py
--rw-r--r--   0        0        0    29524 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/configuration.py
--rw-r--r--   0        0        0    12646 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/forms.py
--rw-r--r--   0        0        0     3547 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/logging.py
--rw-r--r--   0        0        0    64614 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/omnata_plugin.py
--rw-r--r--   0        0        0    18222 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/plugin_entrypoints.py
--rw-r--r--   0        0        0    10078 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/rate_limiting.py
--rw-r--r--   0        0        0     2611 2023-06-02 02:26:50.914610 omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/record_transformer.py
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/LICENSE
+-rw-r--r--   0        0        0      296 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/README.md
+-rw-r--r--   0        0        0      826 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1213 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/__init__.py
+-rw-r--r--   0        0        0     3277 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/api.py
+-rw-r--r--   0        0        0    29524 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/configuration.py
+-rw-r--r--   0        0        0    12646 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/forms.py
+-rw-r--r--   0        0        0     3975 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/logging.py
+-rw-r--r--   0        0        0    64614 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/omnata_plugin.py
+-rw-r--r--   0        0        0    18397 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/plugin_entrypoints.py
+-rw-r--r--   0        0        0    10078 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/rate_limiting.py
+-rw-r--r--   0        0        0     2611 2023-06-04 23:47:26.739094 omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/record_transformer.py
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.1.4/PKG-INFO
```

### Comparing `omnata_plugin_runtime-0.1.3/LICENSE` & `omnata_plugin_runtime-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.3/pyproject.toml` & `omnata_plugin_runtime-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnata-plugin-runtime"
-version = "0.1.3"
+version = "0.1.4"
 description = "A development kit to assist with building, testing and publishing Omnata Plugins"
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{include = "omnata_plugin_runtime", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/__init__.py` & `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/api.py` & `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/api.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/configuration.py` & `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/configuration.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/forms.py` & `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/forms.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/logging.py` & `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/logging.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 import threading
 import datetime
 import logging
 import logging.handlers
 from typing import List
 import pandas
 from snowflake.snowpark import Session
+from pydantic import ValidationError
+
+class CustomLogger(logging.Logger):
+    """
+    Custom logger that can handle pydantic validation errors.
+    Without this, you get "Object of type ErrorWrapper is not JSON serializable"
+    when logging the exception.
+    """
+    def error(self, msg, *args, **kwargs):
+        if isinstance(msg, ValidationError):
+            msg = msg.errors()
+        super().error(msg, *args, **kwargs)
 
 class OmnataPluginLogHandler(logging.handlers.BufferingHandler):
     """
     A logging handler to ship logs back into Omnata Snowflake tables. It uses a combination
     of time and capacity to flush the buffer.
     Additional information about the current sync and run is included, so that logs can be filtered easily.
     """
```

### Comparing `omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/omnata_plugin.py` & `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/omnata_plugin.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/plugin_entrypoints.py` & `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/plugin_entrypoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 
 import json
 import sys
 import os
 import importlib
 import datetime
-from logging import getLogger
+import logging
 from typing import Dict, List, Union, Optional
 from omnata_plugin_runtime.forms import ConnectionMethod
 from omnata_plugin_runtime.logging import OmnataPluginLogHandler
 from omnata_plugin_runtime.rate_limiting import ApiLimits
 from pydantic import BaseModel, parse_obj_as # pylint: disable=no-name-in-module
 from pydantic.json import pydantic_encoder as pydantic_json_encoder # pylint:disable=no-name-in-module
 from snowflake.snowpark import Session
 from omnata_plugin_runtime.omnata_plugin import OmnataPlugin, HttpRateLimiting, OutboundSyncRequest, InboundSyncRequest
 from omnata_plugin_runtime.configuration import OutboundSyncConfigurationParameters,SyncDirection,InboundSyncConfigurationParameters, OutboundSyncStrategy, StoredConfigurationValue,SyncConfigurationParameters,InboundSyncStreamsConfiguration, StreamConfiguration, StoredStreamConfiguration, SyncConfigurationParameters, StoredMappingValue
 from omnata_plugin_runtime.rate_limiting import ApiLimits, RetryLaterException, RateLimitState, RequestRateLimit
 from omnata_plugin_runtime.api import ApplyPayload
-logger = getLogger(__name__)
+from omnata_plugin_runtime.logging import CustomLogger
+# set the logger class to our custom logger so that pydantic errors are handled correctly
+logging.setLoggerClass(CustomLogger)
+logger = logging.getLogger(__name__)
 # this is the new API for secrets access (https://docs.snowflake.com/en/LIMITEDACCESS/secret-api-reference)
 import _snowflake # pylint: disable=import-error
 IMPORT_DIRECTORY_NAME = "snowflake_import_directory"
 
 class PluginEntrypoint():
     """
     This class gives each plugin's stored procs an initial point of contact.
```

### Comparing `omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/rate_limiting.py` & `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.3/src/omnata_plugin_runtime/record_transformer.py` & `omnata_plugin_runtime-0.1.4/src/omnata_plugin_runtime/record_transformer.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.1.3/PKG-INFO` & `omnata_plugin_runtime-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnata-plugin-runtime
-Version: 0.1.3
+Version: 0.1.4
 Summary: A development kit to assist with building, testing and publishing Omnata Plugins
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

