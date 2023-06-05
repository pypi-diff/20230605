# Comparing `tmp/checkmk_dev_tools-0.1.5.tar.gz` & `tmp/checkmk_dev_tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkmk_dev_tools-0.1.5.tar", max compression
+gzip compressed data, was "checkmk_dev_tools-0.1.6.tar", max compression
```

## Comparing `checkmk_dev_tools-0.1.5.tar` & `checkmk_dev_tools-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1056 2023-05-31 14:32:38.730307 checkmk_dev_tools-0.1.5/README.rst
--rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.5/cmk_dev/__init__.py
--rwxr-xr-x   0        0        0    12759 2023-05-31 14:32:31.574262 checkmk_dev_tools-0.1.5/cmk_dev/ci_artifacts.py
--rwxr-xr-x   0        0        0     2184 2023-05-10 11:28:30.476996 checkmk_dev_tools-0.1.5/cmk_dev/cli.py
--rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.5/cmk_dev/listen_std.py
--rw-r--r--   0        0        0     1919 2023-05-31 14:33:16.562542 checkmk_dev_tools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-31 14:32:38.730307 checkmk_dev_tools-0.1.6/README.rst
+-rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.6/cmk_dev/__init__.py
+-rwxr-xr-x   0        0        0    13820 2023-06-05 07:24:31.924090 checkmk_dev_tools-0.1.6/cmk_dev/ci_artifacts.py
+-rwxr-xr-x   0        0        0     2184 2023-05-10 11:28:30.476996 checkmk_dev_tools-0.1.6/cmk_dev/cli.py
+-rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.6/cmk_dev/listen_std.py
+-rw-r--r--   0        0        0     1919 2023-06-05 09:34:19.663050 checkmk_dev_tools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.6/PKG-INFO
```

### Comparing `checkmk_dev_tools-0.1.5/README.rst` & `checkmk_dev_tools-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.5/cmk_dev/ci_artifacts.py` & `checkmk_dev_tools-0.1.6/cmk_dev/ci_artifacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 from argparse import Namespace as Args
 from collections.abc import Mapping
 from configparser import ConfigParser
 from contextlib import contextmanager, suppress
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-
+from collections.abc import Sequence, Mapping
 import yaml
 from jenkins import Jenkins, JenkinsException
 
 # pylint: disable=too-many-instance-attributes
 
+GenMap = None | bool | str | float | int | Sequence['GenMap'], Mapping[str, 'GenMap']
+
 
 def parse_args() -> Args:
     """Cool git like multi command argument parser"""
     parser = ArgumentParser("Provide CI artifacts locally")
     parser.add_argument(
         "--log-level",
         "-l",
@@ -34,32 +36,33 @@
         default="INFO",
     )
 
     parser.set_defaults(func=lambda *_: parser.print_usage())
     subparsers = parser.add_subparsers(help="available commands", metavar="CMD")
 
     parser_info = subparsers.add_parser("info")
-    parser_info.set_defaults(func=fn_info)
+    parser_info.set_defaults(func=_fn_info)
     parser_info.add_argument("job", type=lambda a: a.strip(" /"))
 
     parser_fetch = subparsers.add_parser("fetch")
-    parser_fetch.set_defaults(func=fn_fetch)
+    parser_fetch.set_defaults(func=_fn_fetch)
     parser_fetch.add_argument("job", type=str)
     parser_fetch.add_argument(
         "-c",
         "--credentials",
         type=split_params,
         help=(
             "provide 'url', 'username' and 'password' "
             "or 'username_env', 'url_env' and 'password_env' respectively."
             " If no credentials are provided, the JJB config at "
             " ~/.config/jenkins_jobs/jenkins_jobs.ini is being used."
         ),
     )
     parser_fetch.add_argument("-p", "--params", type=split_params, action="append")
+    parser_fetch.add_argument("-d", "--dir-dependencies", type=str, action="append")
     parser_fetch.add_argument(
         "-t",
         "--time-constraints",
         type=str,
         default="today",
     )
     parser_fetch.add_argument(
@@ -68,52 +71,60 @@
         default="out",
         type=Path,
     )
 
     return parser.parse_args()
 
 
-def split_params(string: str) -> dict[str, str]:
+def split_params(string: str) -> GenMap:
     """Splits a 'string packed map' like 'foo=23,bar=42 into a dict"""
     return {k: v for p in string.split(",") for k, v in (p.split("="),)}
 
 
 def logger():
     """Convenience function retrieves 'our' logger"""
     return logging.getLogger("ci-artifacts")
 
 
 @dataclass
 class Build:
     """Models a Jenkins job build"""
 
+    url: str
     number: int
     timestamp: datetime
     result: str
     building: str
-    artifacts: list[str]
-    parameters: str
     in_progress: bool
+    parameters: str
+    path_hashes: Mapping[str, str]
+    artifacts: list[str]
 
-    def __init__(self, raw_build_info):
-        def params_from(build_info):
+    def __init__(self, raw_build_info: GenMap):
+        def params_from(build_info: GenMap, action_name: str, item_name: str):
             """Return job parameters of provided @build_info as dict"""
             for action in build_info["actions"]:
-                if action.get("_class") == "hudson.model.ParametersAction":
-                    return {p["name"]: p["value"] for p in action["parameters"]}
+                if (action.get("_class") or "").rsplit(".", 1)[-1] == action_name:
+                    if action_name == "ParametersAction":
+                        return {p["name"]: p["value"] for p in action[item_name]}
+                    elif action_name == "CustomBuildPropertiesAction":
+                        return action[item_name]
             return {}
 
+        self.url = raw_build_info["url"]
         self.number = raw_build_info["number"]
         self.timestamp = datetime.fromtimestamp(raw_build_info["timestamp"] // 1000)
         self.result = raw_build_info["result"]
         self.building = raw_build_info["building"]
-        self.artifacts = [a["relativePath"] for a in raw_build_info["artifacts"]]
-        self.parameters = params_from(raw_build_info)
-        self.url = raw_build_info["url"]
         self.in_progress = raw_build_info["inProgress"]
+        self.parameters = params_from(raw_build_info, "ParametersAction", "parameters")
+        self.path_hashes = params_from(raw_build_info, "CustomBuildPropertiesAction", "properties")
+        self.artifacts = [a["relativePath"] for a in raw_build_info["artifacts"]]
+        # SCM could be retrieved via 'hudson.plugins.git.util.BuildData'
+
 
 
 @dataclass
 class Job:
     """Models a Jenkins job"""
 
     name: str
@@ -171,47 +182,29 @@
     whoami = client.get_whoami()
     if not whoami["id"] == username:
         logger().warning("client.get_whoami() does not match jenkins_config['user']")
 
     yield client
 
 
-def fn_info(args: Args) -> None:
+def _fn_info(args: Args) -> None:
     """Entry point for information about job artifacts"""
     with jenkins_client(**extract_credentials(args.credentials)) as client:
         class_name = (job_info := client.get_job_info(args.job))["_class"]
         if class_name == "com.cloudbees.hudson.plugins.folder.Folder":
             # print(yaml.dump(job_info))
             print(Folder(job_info))
         elif class_name == "org.jenkinsci.plugins.workflow.job.WorkflowJob":
             build_infos = [client.get_build_info(args.job, b["number"]) for b in job_info["builds"]]
             print(Job(job_info, build_infos))
         else:
             print(f"Don't know class type {class_name}", file=sys.stderr)
             raise SystemExit(-1)
 
 
-def meets_constraints(build, params, time_constraints):
-    """Checks if a set of requirements are met for a given build"""
-    if build.parameters != params:
-        logger().debug("don't match: %s != %s", build.parameters, params)
-        return False
-
-    if time_constraints == "today":
-        if build.timestamp.date() != datetime.now().date():
-            logger().debug(
-                "time constraints not met: %s != %s", build.timestamp.date(), datetime.now().date()
-            )
-            return False
-    else:
-        raise RuntimeError(f"Don't understand {time_constraints}")
-
-    return True
-
-
 def md5from(filepath: Path) -> str | None:
     """Returns an MD5 sum from contents of file provided"""
     with suppress(FileNotFoundError):
         with open(filepath, "rb") as input_file:
             file_hash = hashlib.md5()
             while chunk := input_file.read(1 << 16):
                 file_hash.update(chunk)
@@ -256,14 +249,37 @@
             logger().debug("Download: %s", fp_filename)
             reply.raise_for_status()
             with open(artifact_filename, "wb") as out_file:
                 for chunk in reply.iter_content(chunk_size=1 << 16):
                     out_file.write(chunk)
 
 
+def meets_constraints(build: Build, params: Mapping[str, str], time_constraints: str) -> bool:
+    """Checks if a set of requirements are met for a given build"""
+    # TODO: find solution for unprovided parameters and default/empty values
+    mismatching_parameters = [
+        (key, build.parameters.get(key, ''), params.get(key, ''))
+        for key in set(build.parameters | params) - {"DISABLE_CACHE"}
+        if build.parameters.get(key, '') != params.get(key, '')
+    ]
+    if mismatching_parameters:
+        logger().debug("build nr=%d doesn't match: %s != %s", build.number, build.parameters, params)
+
+    if time_constraints == "today":
+        if build.timestamp.date() != datetime.now().date():
+            logger().debug(
+                "time constraints not met: %s != %s", build.timestamp.date(), datetime.now().date()
+            )
+            return False
+    else:
+        raise RuntimeError(f"Don't understand {time_constraints}")
+
+    return True
+
+
 def find_matching_build(job: Job, params: Mapping[str, str | int], time_constraints: str) -> Build:
     """Goes through a job's build items and returns the first one to match certain criteria or None
     if none is found"""
     for build_id, build in job.builds.items():
         if meets_constraints(build, params, time_constraints):
             print(
                 f"Found matching build: {build_id}"
@@ -283,15 +299,15 @@
         print(yaml.dump(queue_item))
         if executable := queue_item.get("executable"):
             print(yaml.dump(executable))
             return Build(client.get_build_info(job_full_path, executable["number"]))
         time.sleep(1)
 
 
-def fn_fetch(args: Args) -> None:
+def _fn_fetch(args: Args) -> None:
     """Entry point for fetching artifacts"""
     params = {k: v for p in (args.params or []) for k, v in p.items()}
     logger().debug("Parsed params: %s", params)
     fetch_job_artifacts(args.job, params, args.time_constraints, args.credentials, args.out_dir)
 
 
 def fetch_job_artifacts(job_full_path, params, time_constraints, credentials, out_dir) -> None:
```

### Comparing `checkmk_dev_tools-0.1.5/cmk_dev/cli.py` & `checkmk_dev_tools-0.1.6/cmk_dev/cli.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.5/cmk_dev/listen_std.py` & `checkmk_dev_tools-0.1.6/cmk_dev/listen_std.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.5/pyproject.toml` & `checkmk_dev_tools-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkmk-dev-tools"
-version = "0.1.5"
+version = "0.1.6"
 description = "Checkmk DevOps tools"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/tribe29/checkmk"
 readme = "README.rst"
 packages = [
   {include = "cmk_dev/**/*.py"}
 ]
```

### Comparing `checkmk_dev_tools-0.1.5/PKG-INFO` & `checkmk_dev_tools-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkmk-dev-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Checkmk DevOps tools
 Home-page: https://github.com/tribe29/checkmk
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

