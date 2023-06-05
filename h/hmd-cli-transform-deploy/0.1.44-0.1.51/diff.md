# Comparing `tmp/hmd_cli_transform_deploy-0.1.44-py3-none-any.whl.zip` & `tmp/hmd_cli_transform_deploy-0.1.51-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6526 bytes, number of entries: 7
--rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-03 15:03 hmd_cli_transform_deploy/__init__.py
--rw-rw-rw-  2.0 unx     6538 b- defN 23-Mar-03 15:03 hmd_cli_transform_deploy/controller.py
--rw-rw-rw-  2.0 unx     9365 b- defN 23-Mar-03 15:03 hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
--rw-rw-rw-  2.0 unx     2803 b- defN 23-Mar-03 15:03 hmd_cli_transform_deploy-0.1.44.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Mar-03 15:03 hmd_cli_transform_deploy-0.1.44.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       25 b- defN 23-Mar-03 15:03 hmd_cli_transform_deploy-0.1.44.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      664 b- defN 23-Mar-03 15:03 hmd_cli_transform_deploy-0.1.44.dist-info/RECORD
-7 files, 19487 bytes uncompressed, 5320 bytes compressed:  72.7%
+Zip file size: 6571 bytes, number of entries: 7
+-rw-rw-rw-  2.0 unx        0 b- defN 23-May-18 17:11 hmd_cli_transform_deploy/__init__.py
+-rw-rw-rw-  2.0 unx     6538 b- defN 23-May-18 17:11 hmd_cli_transform_deploy/controller.py
+-rw-rw-rw-  2.0 unx     9551 b- defN 23-May-18 17:11 hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
+-rw-rw-rw-  2.0 unx     2804 b- defN 23-May-18 17:12 hmd_cli_transform_deploy-0.1.51.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-May-18 17:12 hmd_cli_transform_deploy-0.1.51.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       25 b- defN 23-May-18 17:12 hmd_cli_transform_deploy-0.1.51.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      664 b- defN 23-May-18 17:12 hmd_cli_transform_deploy-0.1.51.dist-info/RECORD
+7 files, 19674 bytes uncompressed, 5365 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hmd_cli_transform_deploy/controller.py
 Comment: 
 
 Filename: hmd_cli_transform_deploy/hmd_cli_transform_deploy.py
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.44.dist-info/METADATA
+Filename: hmd_cli_transform_deploy-0.1.51.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.44.dist-info/WHEEL
+Filename: hmd_cli_transform_deploy-0.1.51.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.44.dist-info/top_level.txt
+Filename: hmd_cli_transform_deploy-0.1.51.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_transform_deploy-0.1.44.dist-info/RECORD
+Filename: hmd_cli_transform_deploy-0.1.51.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_transform_deploy/hmd_cli_transform_deploy.py

```diff
@@ -11,14 +11,15 @@
 from hmd_lib_auth.hmd_lib_auth import okta_service_account_token_by_service
 from hmd_lib_librarian_client.artifact_tools import content_item_path_from_parts
 from hmd_cli_tools.okta_tools import get_auth_token
 from hmd_lib_naming.hmd_lib_naming import HmdNamingClient, Service
 from InquirerPy import prompt
 import shutil
 import jwt
+from pathlib import Path
 
 # Grab hostname for locally running NeuronSphere
 # This should only be set when running Robot Integration tests.
 LOCALHOST = os.environ.get("HMD_NEURONSPHERE_LOCALHOST", "localhost")
 
 LOCAL_URL = f"http://{LOCALHOST}/hmd_ms_transform/"
 
@@ -46,15 +47,18 @@
 
     transform_client = HmdLibTransform(base_url=base_url, auth_token=auth_token)
 
     return transform_client
 
 
 def build():
-    shutil.copytree("src", "build/src", dirs_exist_okay=True)
+    if os.path.exists("build/src"):
+        # empty a dirty build directory
+        shutil.rmtree("build/src")
+    shutil.copytree("src", "build/src")
 
 
 def publish():
     pass
 
 
 def deploy(
@@ -222,23 +226,25 @@
 
             result = prompt(questions)
             if result.get("run_params") is None:
                 return
             run_params = json.loads(result.get("run_params"))
             transform_run[tf] = run_params
             run_params = None
+        else:
+            transform_run[tf] = run_params
 
     if transform_names is None:
         transform_names = transform_run.keys()
 
     retry = []
     scheduled = []
     retried = []
     for name in transform_names:
-        print(f"Running: {name}, {json.dumps(run_params)}")
+        print(f"Running: {name}, {json.dumps(transform_run[name])}")
         inst = transform_client.run_provider_transform(name, transform_run[name])
         if inst["status"] == "scheduling_failed":
             print(f"{name} failed to schedule.")
             retry.append(name)
         else:
             scheduled.append(
                 {"name": inst["instance_name"], "identifier": inst["identifier"]}
```

## Comparing `hmd_cli_transform_deploy-0.1.44.dist-info/METADATA` & `hmd_cli_transform_deploy-0.1.51.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-transform-deploy
-Version: 0.1.44
+Version: 0.1.51
 Summary: Command for deploying transforms
 Home-page: UNKNOWN
 Author: Kate Walls
 Author-email: kate.walls@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: acachecontrol (==0.3.5)
@@ -27,22 +27,22 @@
 Requires-Dist: decorator (==5.1.1)
 Requires-Dist: ecdsa (==0.17.0)
 Requires-Dist: frozenlist (==1.3.0)
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: greenlet (==1.1.2)
 Requires-Dist: gremlinpython (==3.5.2)
 Requires-Dist: hmd-cli-app (~=1.1.595)
-Requires-Dist: hmd-cli-tools (~=1.1.227)
-Requires-Dist: hmd-entity-storage (~=0.1.216)
-Requires-Dist: hmd-graphql-client (~=0.1.98)
+Requires-Dist: hmd-cli-tools (~=1.1.228)
+Requires-Dist: hmd-entity-storage (~=0.1.224)
+Requires-Dist: hmd-graphql-client (~=0.1.105)
 Requires-Dist: hmd-lang-naming (~=0.1.12)
-Requires-Dist: hmd-lib-auth (~=0.1.67)
-Requires-Dist: hmd-lib-librarian-client (~=0.1.50)
-Requires-Dist: hmd-lib-naming (~=0.2.28)
-Requires-Dist: hmd-lib-transform (~=0.1.49)
+Requires-Dist: hmd-lib-auth (~=0.1.75)
+Requires-Dist: hmd-lib-librarian-client (~=0.1.53)
+Requires-Dist: hmd-lib-naming (~=0.2.32)
+Requires-Dist: hmd-lib-transform (~=0.1.51)
 Requires-Dist: hmd-meta-types (~=0.2.87)
 Requires-Dist: hmd-schema-loader (~=0.2.35)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: isodate (==0.6.1)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jmespath (==0.10.0)
```

