# Comparing `tmp/dataverse_api-0.2.3.tar.gz` & `tmp/dataverse_api-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_api-0.2.3.tar", max compression
+gzip compressed data, was "dataverse_api-0.2.4.tar", max compression
```

## Comparing `dataverse_api-0.2.3.tar` & `dataverse_api-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.2.3/dataverse_api/__init__.py
--rw-r--r--   0        0        0    24522 2023-06-02 12:47:02.784360 dataverse_api-0.2.3/dataverse_api/dataverse.py
--rw-r--r--   0        0        0     9719 2023-06-02 12:46:37.380533 dataverse_api-0.2.3/dataverse_api/utils.py
--rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.2.3/LICENSE
--rw-r--r--   0        0        0      801 2023-06-02 12:48:47.990615 dataverse_api-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3977 2023-05-30 13:41:54.655391 dataverse_api-0.2.3/README.md
--rw-r--r--   0        0        0     4528 1970-01-01 00:00:00.000000 dataverse_api-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.2.4/dataverse_api/__init__.py
+-rw-r--r--   0        0        0    23285 2023-06-05 13:02:03.152856 dataverse_api-0.2.4/dataverse_api/dataverse.py
+-rw-r--r--   0        0        0     9974 2023-06-05 13:02:03.153857 dataverse_api-0.2.4/dataverse_api/utils.py
+-rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.2.4/LICENSE
+-rw-r--r--   0        0        0      801 2023-06-05 13:01:53.823479 dataverse_api-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3977 2023-05-30 13:41:54.655391 dataverse_api-0.2.4/README.md
+-rw-r--r--   0        0        0     4528 1970-01-01 00:00:00.000000 dataverse_api-0.2.4/PKG-INFO
```

### Comparing `dataverse_api-0.2.3/dataverse_api/dataverse.py` & `dataverse_api-0.2.4/dataverse_api/dataverse.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pandas as pd
 import requests
 from msal_requests_auth.auth import ClientCredentialAuth, DeviceCodeAuth
 
 from dataverse_api.utils import (
     DataverseBatchCommand,
     DataverseError,
-    DataverseTableSchema,
     batch_command,
     batch_id_generator,
     chunk_data,
     convert_data,
     expand_headers,
     extract_batch_response_data,
     extract_key,
@@ -24,26 +23,14 @@
     parse_entity_metadata,
 )
 
 log = logging.getLogger()
 logging.basicConfig(level=logging.INFO)
 
 
-ENTITY_SET_PARAMS = ["EntitySetName", "PrimaryIdAttribute"]
-ENTITY_KEY_PARAMS = ["KeyAttributes"]
-ENTITY_ATTR_PARAMS = [
-    "LogicalName",
-    "SchemaName",
-    "AttributeType",
-    "IsValidForCreate",
-    "IsValidForUpdate",
-    "IsValidODataAttribute",
-]
-
-
 class DataverseClient:
     """
     Base class used to establish authorization and certain default
     parameters for connecting to Dataverse environment, along with
     base methods for interacting with the Web API.
 
     Args:
@@ -66,17 +53,15 @@
             "Accept": "application/json",
             "OData-MaxVersion": "4.0",
             "OData-Version": "4.0",
             "Content-Type": "application/json",
         }
 
     def entity(
-        self,
-        logical_name: Optional[str] = None,
-        entity_set_name: Optional[str] = None,
+        self, logical_name: str, validate: Optional[bool] = False
     ) -> DataverseEntity:
         """
         Returns an Entity class capable of interacting with the given Dataverse Entity.
 
         Args:
           - entity_logical_name: The logical name of the Dataverse Entity. Use to
             enable query-based validation against the API to check column names etc.
@@ -84,31 +69,20 @@
           - entity_set_name: The "API queryable" name of the Dataverse Entity. Use
             to bypass query-based validation, if your script arguments are already
             validated. This saves some API calls during initialization.
 
         Returns:
           - `DataverseEntity` readily instantiated.
         """
-        if (entity_set_name is not None) and (logical_name is not None):
-            log.warning("Using entity set name. Entity will not be validated.")
-            logical_name = None
-
-        name = entity_set_name or logical_name
-
-        if name is None:
-            raise DataverseError("Please provide valid input.")
-
-        if name not in self._entity_cache:
-            self._entity_cache[name] = DataverseEntity(
-                client=self,
-                logical_name=logical_name,
-                entity_set_name=entity_set_name,
+        if logical_name not in self._entity_cache:
+            self._entity_cache[logical_name] = DataverseEntity(
+                client=self, logical_name=logical_name, validate=validate
             )
 
-        return self._entity_cache[name]
+        return self._entity_cache[logical_name]
 
     def get(
         self, url: str, additional_headers: Optional[dict] = None, **kwargs
     ) -> requests.Response:
         """
         GET is used to retrieve data from Dataverse.
 
@@ -322,56 +296,38 @@
 
     >>> table = client.entity(entity_set_name="tablename")  # No validation
     """
 
     def __init__(
         self,
         client: DataverseClient,
-        logical_name: Optional[str] = None,
-        entity_set_name: Optional[str] = None,
+        logical_name: str,
+        validate: Optional[bool] = False,
     ):
         self._client = client
-        self._entity_set_name = entity_set_name
-
-        if logical_name is not None:
-            self._validate = True
-            metadata = self._get_entity_metadata(
-                logical_name=logical_name,
-                entity_params=ENTITY_SET_PARAMS,
-                attr_params=ENTITY_ATTR_PARAMS,
-                key_params=ENTITY_KEY_PARAMS,
-            )
-            self.schema = parse_entity_metadata(metadata)
-
-        elif entity_set_name is not None:
-            self._validate = False
-            self.schema = DataverseTableSchema(name=entity_set_name)
+        self._validate = validate
+        metadata = self._get_entity_metadata(logical_name=logical_name)
+        self.schema = parse_entity_metadata(metadata)
 
-    def _get_entity_metadata(
-        self,
-        logical_name: str,
-        entity_params: list[str],
-        attr_params: list[str],
-        key_params: list[str],
-    ) -> list[dict]:
+    def _get_entity_metadata(self, logical_name: str) -> list[dict]:
         """
         Required for initialization using logical name of Dataverse Entity.
 
         Returns:
           - `DataverseEntitySet` containing attrs `entity_set_name` and `key`
         """
         url = f"EntityDefinitions(LogicalName='{logical_name}')"
-        data = [
-            DataverseBatchCommand(f"{url}?$select={','.join(entity_params)}", "GET"),
-            DataverseBatchCommand(
-                f"{url}/Attributes?$select={','.join(attr_params)}", "GET"
-            ),
-            DataverseBatchCommand(f"{url}/Keys?$select={','.join(key_params)}", "GET"),
-        ]
-
+        data = [DataverseBatchCommand(url, "GET")]
+        if self._validate:
+            data.extend(
+                [
+                    DataverseBatchCommand(url + "/Attributes", "GET"),
+                    DataverseBatchCommand(url + "/Keys", "GET"),
+                ]
+            )
         response = self._client.batch_operation(data)
         return extract_batch_response_data(response.text)
 
     def update_single_value(
         self, data: dict[str, Any], key_columns: Optional[set[str]] = None
     ) -> None:
         """
@@ -381,15 +337,15 @@
           - data: Data that forms the basis for update into Dataverse.
           - key_columns: If validation is not enabled, provide primary column or
             columns that form an alternate key
 
         >>> data={"col1":"abc", "col2":"dac", "col3":69}
         >>> table.update_single_value(data, key_columns={"col1","col2"})
         """
-        key_columns = key_columns or self._validate_payload(data, mode="update")
+        key_columns = key_columns or self._validate_payload([data], mode="update")
 
         if key_columns is None and not self._validate:
             raise DataverseError("Key column(s) must be specified.")
 
         data, row_key = extract_key(data=data, key_columns=key_columns)
 
         if len(data) > 1:
@@ -436,18 +392,20 @@
 
         >>> data=[{"col1":"foo", "col2":2}, {"col1":"bar", "col3":5}]
         >>> table.upsert_single_column(data, key_columns="col1", liberal=True)
         """
         data = convert_data(data)
         key_columns = key_columns or self._validate_payload(data, mode="update")
 
+        liberal: bool = kwargs.get("liberal", False)
+
         if key_columns is None and not self._validate:
             raise DataverseError("Key column(s) must be specified.")
 
-        if not all(len(row) == 1 for row in data):
+        if not all(len(row) == 1 for row in data) and not liberal:
             raise DataverseError(
                 "Only one data column can be passed. Use `upsert` instead."
             )
 
         if kwargs.get("liberal", False) is False:
             key = list(data[0].keys())[0]
             for row in data[1:]:
```

### Comparing `dataverse_api-0.2.3/dataverse_api/utils.py` & `dataverse_api-0.2.4/dataverse_api/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     """
     Parses entity metadata from list of dicts.
 
     Args:
       - A list containing batch GET operation responses from Dataverse.
       - The list must contain three
     """
+    columns, altkeys = None, None  # Optional, will not be assigned if no validation
     for item in metadata:
         data = json.loads(item)
         if "$entity" in item:
             name, key = parse_meta_entity(data)
         elif "/Attributes" in item:
             columns = parse_meta_columns(data)
         elif "/Keys" in item:
@@ -265,34 +266,41 @@
 
 def batch_id_generator() -> str:
     """Simply creates a unique string."""
     return str(uuid4())
 
 
 def batch_command(batch_id: str, api_url: str, row: DataverseBatchCommand) -> str:
-    if row.mode == "GET":
-        row_command = f"""\
-        --{batch_id}
-        Content-Type: application/http
-        Content-Transfer-Encoding: binary
+    """
+    Translates a batch command to the actual request string payload.
 
-        {row.mode} {api_url}{row.uri} HTTP/1.1
+    Args:
+      - batch_id: Unique-ish string that delinates the batch
+      - api_url: The Dataverse Resource API endpoint
+      - row: The associated batch command data
+    """
 
-        """
-    else:
-        row_command = f"""\
-        --{batch_id}
-        Content-Type: application/http
-        Content-Transfer-Encoding: binary
+    uri = api_url + row.uri
+    data = row.data
 
-        {row.mode} {api_url}{row.uri} HTTP/1.1
-        Content-Type: application/json{'; type=entry' if row.mode=="POST" else""}
+    if row.mode == "PUT":
+        col, value = list(row.data.items())[0]
+        uri += f"/{col}"
+        data = {"value": value}
 
-        {json.dumps(row.data)}
-        """
+    row_command = f"""\
+    --{batch_id}
+    Content-Type: application/http
+    Content-Transfer-Encoding: binary
+
+    {row.mode} {uri} HTTP/1.1
+    Content-Type: application/json{'; type=entry' if row.mode=="POST" else""}
+
+    {json.dumps(data)}
+    """
     return dedent(row_command)
 
 
 def find_invalid_columns(
     key_columns: set[str],
     data_columns: set[str],
     schema_columns: dict[str, DataverseColumn],
```

### Comparing `dataverse_api-0.2.3/LICENSE` & `dataverse_api-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.2.3/pyproject.toml` & `dataverse_api-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataverse-api"
-version = "0.2.3"
+version = "0.2.4"
 description = "Abstraction layer for interacting with Microsoft Dataverse in Python. Supports batch operations!"
 authors = ["Marcus Risanger <69350948+MarcusRisanger@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 msal = "^1.22.0"
```

### Comparing `dataverse_api-0.2.3/README.md` & `dataverse_api-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.2.3/PKG-INFO` & `dataverse_api-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-api
-Version: 0.2.3
+Version: 0.2.4
 Summary: Abstraction layer for interacting with Microsoft Dataverse in Python. Supports batch operations!
 Author: Marcus Risanger
 Author-email: 69350948+MarcusRisanger@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

