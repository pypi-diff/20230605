# Comparing `tmp/hmd_cli_bender-0.1.19-py3-none-any.whl.zip` & `tmp/hmd_cli_bender-0.1.22-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5264 bytes, number of entries: 7
--rw-rw-rw-  2.0 unx        0 b- defN 23-Apr-12 13:27 hmd_cli_bender/__init__.py
--rw-rw-rw-  2.0 unx     3035 b- defN 23-Apr-12 13:27 hmd_cli_bender/controller.py
--rw-rw-rw-  2.0 unx     8792 b- defN 23-Apr-12 13:27 hmd_cli_bender/hmd_cli_bender.py
--rw-rw-rw-  2.0 unx     1409 b- defN 23-Apr-12 13:27 hmd_cli_bender-0.1.19.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-12 13:27 hmd_cli_bender-0.1.19.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       15 b- defN 23-Apr-12 13:27 hmd_cli_bender-0.1.19.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      584 b- defN 23-Apr-12 13:27 hmd_cli_bender-0.1.19.dist-info/RECORD
-7 files, 13927 bytes uncompressed, 4218 bytes compressed:  69.7%
+Zip file size: 5703 bytes, number of entries: 7
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Jun-05 13:34 hmd_cli_bender/__init__.py
+-rw-rw-rw-  2.0 unx     3035 b- defN 23-Jun-05 13:34 hmd_cli_bender/controller.py
+-rw-rw-rw-  2.0 unx    10229 b- defN 23-Jun-05 13:34 hmd_cli_bender/hmd_cli_bender.py
+-rw-rw-rw-  2.0 unx     1409 b- defN 23-Jun-05 13:34 hmd_cli_bender-0.1.22.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Jun-05 13:34 hmd_cli_bender-0.1.22.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       15 b- defN 23-Jun-05 13:34 hmd_cli_bender-0.1.22.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      585 b- defN 23-Jun-05 13:34 hmd_cli_bender-0.1.22.dist-info/RECORD
+7 files, 15365 bytes uncompressed, 4657 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hmd_cli_bender/controller.py
 Comment: 
 
 Filename: hmd_cli_bender/hmd_cli_bender.py
 Comment: 
 
-Filename: hmd_cli_bender-0.1.19.dist-info/METADATA
+Filename: hmd_cli_bender-0.1.22.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_bender-0.1.19.dist-info/WHEEL
+Filename: hmd_cli_bender-0.1.22.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_bender-0.1.19.dist-info/top_level.txt
+Filename: hmd_cli_bender-0.1.22.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_bender-0.1.19.dist-info/RECORD
+Filename: hmd_cli_bender-0.1.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_bender/hmd_cli_bender.py

```diff
@@ -1,23 +1,39 @@
 # Implement the lifecycle commands here
 import os
 import json
 from pathlib import Path
+from pkgutil import get_loader
+import subprocess
 from cement.utils.shell import exec_cmd2
 from hmd_cli_tools.hmd_cli_tools import get_env_var
 from hmd_cli_tools.okta_tools import get_auth_token
 from typing import Dict
 from tempfile import TemporaryDirectory
 import urllib
 import yaml
 import traceback
+import boto3
 
 hmd_home = os.environ.get("HMD_HOME")
 
 
+def get_local_package_mount(repo_name: str):
+    pkg_path = get_loader(repo_name.replace("-", "_"))
+
+    if pkg_path is None:
+        return None
+
+    return {
+        "type": "bind",
+        "source": str(Path.resolve(Path(pkg_path.get_filename()).parent)),
+        "target": f"/usr/local/lib/python3.9/site-packages/{repo_name.replace('-', '_')}",
+    }
+
+
 def get_compose(
     image_name: str,
     instance_name: str,
     transform_instance_context: Dict,
     environment: str,
     region: str,
     customer_code: str,
@@ -80,35 +96,55 @@
                         "target": "/root/pip_cache/",
                     },
                 ],
                 "secrets": [],
                 "extra_hosts": ["host.docker.internal:host-gateway"],
             }
         },
-        "networks": {
-            "neuronsphere": {"name": "neuronsphere_default", "external": True}
-        },
+        "networks": {},
     }
 
+    # Check if local NeuronSphere is running and connect to the Docker network
+    r = subprocess.run("docker network inspect neuronsphere_default".split(" "))
+
+    if r.returncode == 0:
+        compose["networks"]["neuronsphere"] = {
+            "name": "neuronsphere_default",
+            "external": True,
+        }
+
+    local_mnt = get_local_package_mount(
+        repo_name=os.path.basename(os.path.abspath(repo_path))
+    )
+
+    if local_mnt is not None:
+        compose["services"]["bender_transform"]["volumes"].append(local_mnt)
+
     if auth_token is not None:
         compose["services"]["bender_transform"]["environment"][
             "HMD_AUTH_TOKEN"
         ] = auth_token
 
-    if hmd_home:
-        compose["services"]["bender_transform"]["volumes"].append(
-            {
-                "type": "bind",
-                "source": f"{os.path.expanduser('~')}/.aws",
-                "target": "/root/.aws/",
-            }
-        )
-        compose["services"]["bender_transform"]["environment"][
-            "AWS_PROFILE"
-        ] = os.environ.get("AWS_PROFILE")
+    aws_profile = os.environ.get("AWS_PROFILE")
+    if hmd_home and aws_profile:
+        session = boto3.Session(profile_name=aws_profile)
+        creds = session.get_credentials()
+
+        if creds.access_key:
+            compose["services"]["bender_transform"]["environment"][
+                "AWS_ACCESS_KEY_ID"
+            ] = creds.access_key
+        if creds.secret_key:
+            compose["services"]["bender_transform"]["environment"][
+                "AWS_SECRET_ACCESS_KEY"
+            ] = creds.secret_key
+        if creds.token:
+            compose["services"]["bender_transform"]["environment"][
+                "AWS_SESSION_TOKEN"
+            ] = creds.token
 
     secrets = {"secrets": {}}
 
     if docker_secret:
         secrets["secrets"].update({"docker_repo": {"file": docker_secret}})
         compose["services"]["bender_transform"]["secrets"].append("docker_repo")
         compose["services"]["bender_transform"]["environment"].update(
@@ -151,21 +187,28 @@
         region = get_env_var("HMD_REGION")
         cust_code = get_env_var("HMD_CUSTOMER_CODE")
         account = os.environ.get("HMD_ACCOUNT", "")
 
     repo_path = os.getcwd()
 
     transform_instance_context = {
-        "instance_name": instance_name,
+        "instance_name": instance_name.replace("-", "_"),
         "repo_name": name,
         "version": version,
         "deployment_id": deployment_id,
     }
 
     extra_context = {}
+
+    if context_file is None:
+        context_file = Path(repo_path) / "test" / "local_context.json"
+
+    if not os.path.exists(context_file):
+        context_file = Path(repo_path) / "meta-data" / "config_local.json"
+
     if context_file is not None and os.path.exists(context_file):
         with open(context_file, "r") as ctx:
             extra_context = json.load(ctx)
 
     transform_instance_context = {**transform_instance_context, **extra_context}
 
     pip_username = os.environ.get("PIP_USERNAME")
```

## Comparing `hmd_cli_bender-0.1.19.dist-info/METADATA` & `hmd_cli_bender-0.1.22.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-bender
-Version: 0.1.19
+Version: 0.1.22
 Summary: CLI for bender transform
 Home-page: UNKNOWN
 Author: Kate Walls
 Author-email: kate.walls@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: aws-secretsmanager-caching (==1.1.1.5)
```

