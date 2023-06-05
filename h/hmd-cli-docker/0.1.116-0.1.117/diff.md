# Comparing `tmp/hmd_cli_docker-0.1.116-py3-none-any.whl.zip` & `tmp/hmd_cli_docker-0.1.117-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9165 bytes, number of entries: 9
--rw-rw-rw-  2.0 unx        1 b- defN 23-Mar-09 15:45 hmd_cli_docker/__init__.py
--rw-rw-rw-  2.0 unx     1035 b- defN 23-Mar-09 15:45 hmd_cli_docker/config.py
--rw-rw-rw-  2.0 unx     7625 b- defN 23-Mar-09 15:45 hmd_cli_docker/controller.py
--rw-rw-rw-  2.0 unx    12730 b- defN 23-Mar-09 15:45 hmd_cli_docker/hmd_cli_docker.py
--rw-rw-rw-  2.0 unx     4415 b- defN 23-Mar-09 15:45 hmd_cli_docker/utils.py
--rw-rw-rw-  2.0 unx     1950 b- defN 23-Mar-09 15:46 hmd_cli_docker-0.1.116.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Mar-09 15:46 hmd_cli_docker-0.1.116.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       15 b- defN 23-Mar-09 15:46 hmd_cli_docker-0.1.116.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      750 b- defN 23-Mar-09 15:46 hmd_cli_docker-0.1.116.dist-info/RECORD
-9 files, 28613 bytes uncompressed, 7865 bytes compressed:  72.5%
+Zip file size: 9216 bytes, number of entries: 9
+-rw-rw-rw-  2.0 unx        1 b- defN 23-Apr-03 16:44 hmd_cli_docker/__init__.py
+-rw-rw-rw-  2.0 unx     1138 b- defN 23-Apr-03 16:44 hmd_cli_docker/config.py
+-rw-rw-rw-  2.0 unx     7625 b- defN 23-Apr-03 16:44 hmd_cli_docker/controller.py
+-rw-rw-rw-  2.0 unx    12939 b- defN 23-Apr-03 16:44 hmd_cli_docker/hmd_cli_docker.py
+-rw-rw-rw-  2.0 unx     4415 b- defN 23-Apr-03 16:44 hmd_cli_docker/utils.py
+-rw-rw-rw-  2.0 unx     1950 b- defN 23-Apr-03 16:44 hmd_cli_docker-0.1.117.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-03 16:44 hmd_cli_docker-0.1.117.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       15 b- defN 23-Apr-03 16:44 hmd_cli_docker-0.1.117.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      750 b- defN 23-Apr-03 16:44 hmd_cli_docker-0.1.117.dist-info/RECORD
+9 files, 28925 bytes uncompressed, 7916 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: hmd_cli_docker/hmd_cli_docker.py
 Comment: 
 
 Filename: hmd_cli_docker/utils.py
 Comment: 
 
-Filename: hmd_cli_docker-0.1.116.dist-info/METADATA
+Filename: hmd_cli_docker-0.1.117.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_docker-0.1.116.dist-info/WHEEL
+Filename: hmd_cli_docker-0.1.117.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_docker-0.1.116.dist-info/top_level.txt
+Filename: hmd_cli_docker-0.1.117.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_docker-0.1.116.dist-info/RECORD
+Filename: hmd_cli_docker-0.1.117.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_docker/config.py

```diff
@@ -1,12 +1,16 @@
 from pathlib import Path
 from hmd_lib_containers.config.build_config import ImageBuildConfig, ImageBuildSecret
 from hmd_cli_tools.hmd_cli_tools import read_manifest
 
 
+def get_default_npm_secret(npmrc_name: str):
+    return ImageBuildSecret(id="npmrc", src=npmrc_name)
+
+
 def get_default_pip_secret(pip_conf_name: str):
     return ImageBuildSecret(id="pipconfig", src=pip_conf_name)
 
 
 class HmdDockerDefaultBuildConfig(ImageBuildConfig):
     context_dir = Path(
         "./src/docker"
```

## hmd_cli_docker/hmd_cli_docker.py

```diff
@@ -27,15 +27,19 @@
     login_docker,
     get_docker_client,
     get_docker_registry,
     build_docker_tag,
     create_ecr_repository,
     pull_docker_image,
 )
-from .config import HmdDockerDefaultBuildConfig, get_default_pip_secret
+from .config import (
+    HmdDockerDefaultBuildConfig,
+    get_default_pip_secret,
+    get_default_npm_secret,
+)
 
 TARGET_PLATFORMS = {
     "x86_64": "linux/amd64",
     "arm64": "linux/arm64",
 }
 
 
@@ -88,14 +92,15 @@
     install_local = build_config.install_local
 
     docker_dir = build_config.context_dir
 
     with build_dir(name):
 
         pip_conf_name = Path.home() / ".config" / "pip" / "pip.conf"
+        npmrc_name = Path.home() / ".npmrc"
 
         if os.name == "nt":
             pip_conf_name = Path.home() / "pip" / "pip.ini"
 
         pip_conf_name = os.environ.get("PIP_CONFIG_FILE", pip_conf_name)
 
         if not pip_conf_name.exists():
@@ -176,14 +181,17 @@
 
         if not is_windows:
             build_config.secrets = [
                 *build_config.secrets,
                 get_default_pip_secret(str(pip_conf_name)),
             ]
 
+            if os.path.exists(npmrc_name):
+                build_config.secrets.append(get_default_npm_secret(npmrc_name))
+
         if os.environ.get("HMD_DOCKER_NETWORK") is not None:
             build_config.network = os.environ.get("HMD_DOCKER_NETWORK")
 
         build_image(tag, version, build_config)
 
     build_metadata_path = Path("./build/meta-data/")
```

## Comparing `hmd_cli_docker-0.1.116.dist-info/METADATA` & `hmd_cli_docker-0.1.117.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-docker
-Version: 0.1.116
+Version: 0.1.117
 Summary: Implementation for docker cli command
 Home-page: UNKNOWN
 Author: Jim Majure
 Author-email: jim.majure@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: attrs (==21.4.0)
@@ -16,16 +16,16 @@
 Requires-Dist: certifi (==2022.12.7)
 Requires-Dist: charset-normalizer (==2.0.12)
 Requires-Dist: click (==8.0.4)
 Requires-Dist: colorlog (==6.6.0)
 Requires-Dist: docker (==5.0.3)
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: hmd-cli-app (~=1.1.595)
-Requires-Dist: hmd-cli-tools (~=1.1.227)
-Requires-Dist: hmd-lang-deployment (~=0.1.73)
+Requires-Dist: hmd-cli-tools (~=1.1.228)
+Requires-Dist: hmd-lang-deployment (~=0.1.75)
 Requires-Dist: hmd-lib-containers (~=0.1.19)
 Requires-Dist: hmd-meta-types (~=0.2.87)
 Requires-Dist: hmd-schema-loader (~=0.2.35)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jmespath (==0.10.0)
```

