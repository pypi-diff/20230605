# Comparing `tmp/lp_ap_tools-0.1.4-py3-none-any.whl.zip` & `tmp/lp_ap_tools-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4438 bytes, number of entries: 8
+Zip file size: 4951 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       15 b- defN 23-May-29 02:44 lp_ap_tools/__init__.py
--rw-r--r--  2.0 unx     8130 b- defN 23-May-31 02:54 lp_ap_tools/lp_ap_tools.py
+-rw-r--r--  2.0 unx    10366 b- defN 23-Jun-05 02:37 lp_ap_tools/lp_ap_tools.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-29 02:51 tests/__init__.py
 -rw-r--r--  2.0 unx      104 b- defN 23-May-29 03:34 tests/lp_ap_tools_test.py
--rw-r--r--  2.0 unx      856 b- defN 23-May-31 02:55 lp_ap_tools-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 02:55 lp_ap_tools-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-May-31 02:55 lp_ap_tools-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      626 b- defN 23-May-31 02:55 lp_ap_tools-0.1.4.dist-info/RECORD
-8 files, 9841 bytes uncompressed, 3338 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx      856 b- defN 23-Jun-05 02:39 lp_ap_tools-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 02:39 lp_ap_tools-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 02:39 lp_ap_tools-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      627 b- defN 23-Jun-05 02:39 lp_ap_tools-0.1.5.dist-info/RECORD
+8 files, 12078 bytes uncompressed, 3851 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/lp_ap_tools_test.py
 Comment: 
 
-Filename: lp_ap_tools-0.1.4.dist-info/METADATA
+Filename: lp_ap_tools-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: lp_ap_tools-0.1.4.dist-info/WHEEL
+Filename: lp_ap_tools-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: lp_ap_tools-0.1.4.dist-info/top_level.txt
+Filename: lp_ap_tools-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: lp_ap_tools-0.1.4.dist-info/RECORD
+Filename: lp_ap_tools-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lp_ap_tools/lp_ap_tools.py

```diff
@@ -1,28 +1,30 @@
 import functools
 import time
 import os
 import globus_sdk 
-from flask import request #TODO update library with flask library
-from datetime import datetime
-from rocrate.rocrate import ROCrate, SoftwareApplication
-from rocrate.model.person import Person
-from pydantic import Field, BaseModel, create_model # include pydantic in new tooling
+from globus_sdk import TransferClient, TransferData, LocalGlobusConnectPersonal
 from globus_action_provider_tools.data_types import ActionProviderDescription, ActionRequest, ActionStatus
 from globus_action_provider_tools.flask import ActionProviderBlueprint
 from globus_action_provider_tools import AuthState
 
+from flask import request 
+from datetime import datetime
+from rocrate.rocrate import ROCrate, SoftwareApplication
+from rocrate.model.person import Person
+from pydantic import Field, BaseModel, create_model
+
+
 # possible schema for container description in ROcrate
 # https://openschemas.github.io/specifications/ContainerRecipe/
 
 # LP fields to be included within AP input_schema
 # TODO: Build schema, and provide flexibility in chosen fields. 
 LP_FIELDS = {
-   'context_description': (str, Field(..., title="Some required input", description="A useful description")),
-   'researcher_comment': (str, Field(..., title="Some required input", description="A useful description")),
+   'management_ep_id': (str, Field(..., title="Some required input", description="A useful description")),
 }
 
 # returns a new model with the union of the original class 
 # and the LP fields
 def add_lp_params(origin_class: BaseModel):
    original_fields = {name: (field.outer_type_, field.field_info) for name, field in origin_class.__fields__.items()}
    return create_model(type(origin_class).__name__, **{**original_fields, **LP_FIELDS})
@@ -70,16 +72,15 @@
                      crate: ROCrate):
    pass
 
 def create_user(ap_auth: AuthState,
                   ap_status: ActionStatus,
                   crate: ROCrate):
    # Athenticates with globus to get information such as the creator's identity
-   ac = globus_sdk.AuthClient(authorizer=globus_sdk.AccessTokenAuthorizer(ap_auth.bearer_token))
-
+   ac = ap_auth.auth_client
    # Get creator's identity and add to RO-Crate
    creator_id = ap_status.creator_id.replace("urn:globus:auth:identity:", "")
    creator_identity = ac.get_identities(ids=creator_id)
    user = crate.add(Person(
       crate=crate,
       identifier=creator_identity['identities'][0]['id'],
       properties={
@@ -98,17 +99,23 @@
                   ap_status: ActionStatus,
                   raw_request: request):
    # Add action to RO-Crate
    action = crate.add(SoftwareApplication(
       crate=crate,
       identifier=ap_status.action_id,
       properties={
-         "name": ap_apbt.name,
+         "title": ap_apbt.name,
+         "subtitle": ap_description.subtitle,
          "description": ap_description.description,
-         "url": raw_request[0].url
+         "url": raw_request[0].url,
+         "API_version": ap_description.api_version,
+         "globus_auth_scope": ap_description.globus_auth_scope,
+         "keywords": ap_description.keywords,
+         "visible_to": ap_description.visible_to,
+         "creator_id": ap_status.creator_id,
       }
    ))
    # associate action with creator
    return action
 
 def create_input(crate: ROCrate,
                  dir_struct: dict):
@@ -117,81 +124,118 @@
    in "exp/logs" recursively to the crate, but only the top-level 
    "exp/logs" dataset itself is listed in the metadata file (there 
    is no requirement to represent every file and folder in the 
    JSON-LD). To also add files and directory recursively to the 
    metadata, use add_tree (but note that it only works on local 
    directory trees)."""
 
-   input_files = crate.add_dataset(dir_struct['input'])
+   input_files = crate.add_tree(dir_struct['input'])
    return input_files
 
 def create_output(crate: ROCrate,
                   dir_struct: dict):
 
    """Note that the above adds all files and directories contained 
    in "exp/logs" recursively to the crate, but only the top-level 
    "exp/logs" dataset itself is listed in the metadata file (there 
    is no requirement to represent every file and folder in the 
    JSON-LD). To also add files and directory recursively to the 
    metadata, use add_tree (but note that it only works on local 
    directory trees)."""
 
-   output_files = crate.add_dataset(dir_struct['output'])
+   output_files = crate.add_tree(dir_struct['output'])
    return output_files
 
+def transfer_crate(ap_auth: AuthState,
+                   crate_path: str,
+                   management_ep_id: str,
+                   ap_status: ActionStatus,
+                   ap_apbt: ActionProviderBlueprint):
+   
+   # Get local running globus connect personal endpoint
+   local_gcp = LocalGlobusConnectPersonal()
+   # Get dependent token for globus transfer API
+   dependent_tokens = ap_auth.auth_client.oauth2_get_dependent_tokens(ap_auth.bearer_token)
+   transfer_token = dependent_tokens.by_resource_server['transfer.api.globus.org']['access_token']
+   # Transfer crate to management endpoint
+   transfer_client = TransferClient(authorizer=globus_sdk.AccessTokenAuthorizer(transfer_token))
+   data = TransferData(transfer_client,
+                       source_endpoint=local_gcp.endpoint_id,
+                       destination_endpoint=management_ep_id,
+                       label=f"{ap_apbt.name}_AP crate transfer: crate_{ap_status.action_id}")
+   data.add_item(crate_path, f"CRATE_DIR/crate_{ap_status.action_id}", recursive=True)
+   transfer_result = transfer_client.submit_transfer(data)
+   print(f"Transfering crate for job {ap_status.action_id}. Transfer Job ID: {transfer_result['task_id']}")
+
 # -----------------------------------------------
 # ------------ Primary decorator  ---------------
 # -----------------------------------------------
 
-def LP_artefact(dir_struct: dict,
-                description: str = "description",
-                creator: str = "creator"):
+def LP_artefact(dir_struct: dict):
     def middle(run_computation):
       @functools.wraps(run_computation)
       def create_ROcrate(ap_description: ActionProviderDescription, 
                          ap_request: ActionRequest, 
                          ap_status: ActionStatus,
                          ap_auth: AuthState,
                          ap_apbt: ActionProviderBlueprint,
                          raw_request: request):
+         
+         # --------------------------------------------------------
+         # ---------------- Preprocessing Crate -------------------
+         # --------------------------------------------------------
 
          # Create RO-Crate
          crate_name = f"crate_{ap_status.action_id}"
          crate = ROCrate()
          crate.name = crate_name
          crate.description = f"LP artefact for action {ap_status.action_id}"
          crate.datePublished = datetime.now().isoformat()
-         # debug_ap_objects(ap_description, ap_request, ap_status, ap_auth, ap_apbt)
-
-         # use athentication token to integrate with globus metadata
+         # pass ap_auth to retrieve creator's identity from globus
          user = create_user(ap_auth=ap_auth, 
                         ap_status=ap_status, 
                         crate=crate)
          action = create_action(crate=crate,
                        ap_apbt=ap_apbt,
                        ap_description=ap_description,
                        ap_status=ap_status,
                        raw_request=raw_request)
          # Add relationship between user and action
          action["executed"] = user
          # Add staged input files to RO-Crate
          input = create_input(crate=crate, dir_struct=dir_struct)
          # Add relationship between action and input
-         action["input"] = input
+         action["input_dir"] = input
+
+         # --------------------------------------------------------
+         # ----------------- Run computation ----------------------
+         # --------------------------------------------------------
 
          # Execute the container, and record various metadata
+         # TODO: Provide a method for extracting/generating metadata 
+         # from inside the container
          print(f"----- Computation for action {ap_status.action_id} starting -----")
          start_time = time.time()
          computation = run_computation(ap_description, ap_request, ap_status, ap_auth, ap_apbt, raw_request)
          total_time = time.time() - start_time
          print(f"----- Computation for action {ap_status.action_id} ending. Total time taken: {total_time} -----")
 
+         # --------------------------------------------------------
+         # ---------------- Postprocessing Crate ------------------
+         # --------------------------------------------------------
+
          # Add output files to RO-Crate
          output = create_output(crate=crate, dir_struct=dir_struct)
          # Add relationship between action and output
-         action["output"] = output
+         action["output_dir"] = output
 
          # Write RO-Crate to disk
          crate.write_crate(os.path.join(dir_struct["crates"], f"crate_{ap_status.action_id}"))
+         # Transfer crate to management endpoint
+         transfer_crate(ap_auth=ap_auth,
+                        crate_path=os.path.join(dir_struct["crates"], crate_name), 
+                        management_ep_id=ap_request.body["management_ep_id"],
+                        ap_status=ap_status,
+                        ap_apbt=ap_apbt)
          return computation
       return create_ROcrate
     return middle
```

## Comparing `lp_ap_tools-0.1.4.dist-info/METADATA` & `lp_ap_tools-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lp-ap-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python decorator for creating ActionProvider RO-crates within a Globus flow
 Home-page: https://github.com/GusEllerm/lp_tools.git
 Author: Augustus Ellerm
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

