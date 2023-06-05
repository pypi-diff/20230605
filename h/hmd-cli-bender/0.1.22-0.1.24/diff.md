# Comparing `tmp/hmd_cli_bender-0.1.22-py3-none-any.whl.zip` & `tmp/hmd_cli_bender-0.1.24-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5703 bytes, number of entries: 7
--rw-rw-rw-  2.0 unx        0 b- defN 23-Jun-05 13:34 hmd_cli_bender/__init__.py
--rw-rw-rw-  2.0 unx     3035 b- defN 23-Jun-05 13:34 hmd_cli_bender/controller.py
--rw-rw-rw-  2.0 unx    10229 b- defN 23-Jun-05 13:34 hmd_cli_bender/hmd_cli_bender.py
--rw-rw-rw-  2.0 unx     1409 b- defN 23-Jun-05 13:34 hmd_cli_bender-0.1.22.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Jun-05 13:34 hmd_cli_bender-0.1.22.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       15 b- defN 23-Jun-05 13:34 hmd_cli_bender-0.1.22.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      585 b- defN 23-Jun-05 13:34 hmd_cli_bender-0.1.22.dist-info/RECORD
-7 files, 15365 bytes uncompressed, 4657 bytes compressed:  69.7%
+Zip file size: 5731 bytes, number of entries: 7
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Jun-05 14:09 hmd_cli_bender/__init__.py
+-rw-rw-rw-  2.0 unx     3035 b- defN 23-Jun-05 14:09 hmd_cli_bender/controller.py
+-rw-rw-rw-  2.0 unx    10363 b- defN 23-Jun-05 14:09 hmd_cli_bender/hmd_cli_bender.py
+-rw-rw-rw-  2.0 unx     1409 b- defN 23-Jun-05 14:09 hmd_cli_bender-0.1.24.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Jun-05 14:09 hmd_cli_bender-0.1.24.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       15 b- defN 23-Jun-05 14:09 hmd_cli_bender-0.1.24.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      585 b- defN 23-Jun-05 14:09 hmd_cli_bender-0.1.24.dist-info/RECORD
+7 files, 15499 bytes uncompressed, 4685 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hmd_cli_bender/controller.py
 Comment: 
 
 Filename: hmd_cli_bender/hmd_cli_bender.py
 Comment: 
 
-Filename: hmd_cli_bender-0.1.22.dist-info/METADATA
+Filename: hmd_cli_bender-0.1.24.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_bender-0.1.22.dist-info/WHEEL
+Filename: hmd_cli_bender-0.1.24.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_bender-0.1.22.dist-info/top_level.txt
+Filename: hmd_cli_bender-0.1.24.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_bender-0.1.22.dist-info/RECORD
+Filename: hmd_cli_bender-0.1.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_bender/hmd_cli_bender.py

```diff
@@ -50,15 +50,14 @@
 
     compose = {
         "version": "3.2",
         "services": {
             "bender_transform": {
                 "image": image_name,
                 "container_name": f"bender-inst_{instance_name}",
-                "networks": ["neuronsphere"],
                 "environment": {
                     "TRANSFORM_INSTANCE_CONTEXT": json.dumps(
                         transform_instance_context
                     ),
                     "HMD_ENVIRONMENT": environment,
                     "HMD_REGION": region,
                     "HMD_ACCOUNT": account,
@@ -107,44 +106,48 @@
     r = subprocess.run("docker network inspect neuronsphere_default".split(" "))
 
     if r.returncode == 0:
         compose["networks"]["neuronsphere"] = {
             "name": "neuronsphere_default",
             "external": True,
         }
+        compose["services"]["bender_transform"]["networks"] = ["neuronsphere"]
 
     local_mnt = get_local_package_mount(
         repo_name=os.path.basename(os.path.abspath(repo_path))
     )
 
     if local_mnt is not None:
         compose["services"]["bender_transform"]["volumes"].append(local_mnt)
 
     if auth_token is not None:
         compose["services"]["bender_transform"]["environment"][
             "HMD_AUTH_TOKEN"
         ] = auth_token
 
-    aws_profile = os.environ.get("AWS_PROFILE")
-    if hmd_home and aws_profile:
-        session = boto3.Session(profile_name=aws_profile)
-        creds = session.get_credentials()
-
-        if creds.access_key:
-            compose["services"]["bender_transform"]["environment"][
-                "AWS_ACCESS_KEY_ID"
-            ] = creds.access_key
-        if creds.secret_key:
-            compose["services"]["bender_transform"]["environment"][
-                "AWS_SECRET_ACCESS_KEY"
-            ] = creds.secret_key
-        if creds.token:
-            compose["services"]["bender_transform"]["environment"][
-                "AWS_SESSION_TOKEN"
-            ] = creds.token
+    try:
+        aws_profile = os.environ.get("AWS_PROFILE")
+        if hmd_home and aws_profile:
+            session = boto3.Session(profile_name=aws_profile)
+            creds = session.get_credentials()
+
+            if creds.access_key:
+                compose["services"]["bender_transform"]["environment"][
+                    "AWS_ACCESS_KEY_ID"
+                ] = creds.access_key
+            if creds.secret_key:
+                compose["services"]["bender_transform"]["environment"][
+                    "AWS_SECRET_ACCESS_KEY"
+                ] = creds.secret_key
+            if creds.token:
+                compose["services"]["bender_transform"]["environment"][
+                    "AWS_SESSION_TOKEN"
+                ] = creds.token
+    except:
+        pass
 
     secrets = {"secrets": {}}
 
     if docker_secret:
         secrets["secrets"].update({"docker_repo": {"file": docker_secret}})
         compose["services"]["bender_transform"]["secrets"].append("docker_repo")
         compose["services"]["bender_transform"]["environment"].update(
```

## Comparing `hmd_cli_bender-0.1.22.dist-info/METADATA` & `hmd_cli_bender-0.1.24.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-bender
-Version: 0.1.22
+Version: 0.1.24
 Summary: CLI for bender transform
 Home-page: UNKNOWN
 Author: Kate Walls
 Author-email: kate.walls@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: aws-secretsmanager-caching (==1.1.1.5)
```

