# Comparing `tmp/datatrail_cli-0.2.0.tar.gz` & `tmp/datatrail_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.2.0.tar", max compression
+gzip compressed data, was "datatrail_cli-0.3.0.tar", max compression
```

## Comparing `datatrail_cli-0.2.0.tar` & `datatrail_cli-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1080 2023-05-26 20:56:06.198466 datatrail_cli-0.2.0/LICENSE
--rw-r--r--   0        0        0     3558 2023-05-26 20:56:06.198466 datatrail_cli-0.2.0/README.md
--rw-r--r--   0        0        0      214 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/__init__.py
--rw-r--r--   0        0        0      893 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/cli.py
--rw-r--r--   0        0        0     3714 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/config.py
--rw-r--r--   0        0        0     1062 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/config.yaml
--rw-r--r--   0        0        0     3442 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/ls.py
--rw-r--r--   0        0        0     4415 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/ps.py
--rw-r--r--   0        0        0     3978 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/pull.py
--rw-r--r--   0        0        0     8795 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/src/functions.py
--rw-r--r--   0        0        0     8262 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/utilities/cadcclient.py
--rw-r--r--   0        0        0     1493 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/utilities/utilities.py
--rw-r--r--   0        0        0     1048 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 datatrail_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-05 15:36:00.935159 datatrail_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3558 2023-06-05 15:36:00.935159 datatrail_cli-0.3.0/README.md
+-rw-r--r--   0        0        0      214 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/__init__.py
+-rw-r--r--   0        0        0     3862 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/clear.py
+-rw-r--r--   0        0        0      929 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/cli.py
+-rw-r--r--   0        0        0     3714 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/config.yaml
+-rw-r--r--   0        0        0     3442 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/ls.py
+-rw-r--r--   0        0        0     4415 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/ps.py
+-rw-r--r--   0        0        0     4066 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/pull.py
+-rw-r--r--   0        0        0    12027 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/src/functions.py
+-rw-r--r--   0        0        0     9241 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     1493 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1048 2023-06-05 15:36:00.943159 datatrail_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 datatrail_cli-0.3.0/PKG-INFO
```

### Comparing `datatrail_cli-0.2.0/LICENSE` & `datatrail_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.2.0/README.md` & `datatrail_cli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.2.0/dtcli/cli.py` & `datatrail_cli-0.3.0/dtcli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Datatrail Command Line Interface."""
 
 import click
 from click_aliasing import ClickAliasedGroup
 from pkg_resources import get_distribution
 from rich import console, pretty
 
-from dtcli import config, ls, ps, pull
+from dtcli import clear, config, ls, ps, pull
 
 pretty.install()
 terminal = console.Console()
 
 
 # Main CLI
 @click.group(cls=ClickAliasedGroup)
@@ -34,11 +34,12 @@
         style="green",
     )
 
 
 cli.add_command(ls.list, aliases=["ls"])
 cli.add_command(ps.ps)
 cli.add_command(pull.pull)
+cli.add_command(clear.clear)
 cli.add_command(config.config)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `datatrail_cli-0.2.0/dtcli/config.py` & `datatrail_cli-0.3.0/dtcli/config.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.2.0/dtcli/config.yaml` & `datatrail_cli-0.3.0/dtcli/config.yaml`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.2.0/dtcli/ls.py` & `datatrail_cli-0.3.0/dtcli/ls.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.2.0/dtcli/ps.py` & `datatrail_cli-0.3.0/dtcli/ps.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.2.0/dtcli/pull.py` & `datatrail_cli-0.3.0/dtcli/pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,9 +120,15 @@
     else:
         is_download = Confirm.ask(
             f"Download {len(files['missing'])} files?",
         )
 
     # Download missing files.
     if is_download:
-        get_files(files["missing"], site=site, directory=directory, cores=cores)
+        get_files(
+            files["missing"],
+            site=site,
+            directory=directory,
+            cores=cores,
+            verbose=verbose,
+        )
     return None
```

### Comparing `datatrail_cli-0.2.0/dtcli/src/functions.py` & `datatrail_cli-0.3.0/dtcli/src/functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Functions for CLI."""
 
 import logging
 import os
+import shutil
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 
 from dtcli.config import procure
 from dtcli.utilities import cadcclient, utilities
@@ -220,26 +221,34 @@
 
 
 def get_files(
     files: List[str],
     site: str,
     directory: str,
     cores: int,
+    verbose: int,
 ) -> None:
     """Download all files from a dataset which only contains files.
 
     Args:
         files (List[str]): Paths of files to download.
         site (str): Local machine.
         directory (str): Path to download files to. Default depends on site.
         cores (int): Number of processors to initiate download on.
+        verbose (int): Verbosity level.
 
     Returns:
         None
     """
+    # Set logging level.
+    logger.setLevel("WARNING")
+    if verbose == 1:
+        logger.setLevel("INFO")
+    elif verbose > 1:
+        logger.setLevel("DEBUG")
     # Load configuration.
     config = procure()
     mounts = config["root_mounts"]
     # download missing files.
     if len(files) > 0:
         print(f"{len(files)} files missing.")
         print(f"Downloading {len(files)} missing files.")
@@ -247,9 +256,106 @@
         if not directory:
             directory = mounts[site]
         destinations = [directory + "/" + f for f in files]
         # make directory structure if it does not exist.
         folders = {os.path.dirname(path) for path in destinations}
         for folder in folders:
             os.makedirs(folder, exist_ok=True)
-        cadcclient.pget(source=files, destination=destinations, processors=cores)
+        cadcclient.pget(
+            source=files, destination=destinations, processors=cores, verbose=verbose
+        )
     return None
+
+
+def clear_dataset_path(path: str, verbose: int, quiet: bool) -> bool:
+    """Delete a path provided.
+
+    Args:
+        path (str): Path to delete.
+        verbose (int): Verbosity level.
+        quiet (bool): Quiet mode.
+
+    Returns:
+        bool: True if path was deleted.
+    """
+    logger.setLevel("WARNING")
+    if verbose == 1:
+        logger.setLevel("INFO")
+    elif verbose > 1:
+        logger.setLevel("DEBUG")
+    elif quiet:
+        logger.setLevel("ERROR")
+
+    # Check if path exists.
+    logger.debug(f"Checking if path {path} exists.")
+    exists = os.path.exists(path)
+
+    # Delete files.
+    if exists:
+        shutil.rmtree(path)
+        logger.info("Path successfully removed.")
+        return True
+    else:
+        logger.info(f"Path {path} not found.")
+        return False
+
+
+def find_dataset_common_path(
+    scope: str, dataset: str, site: str, verbose: int, quiet: bool
+) -> Optional[str]:
+    """Find common path for a dataset.
+
+    Args:
+        scope (str): Scope of dataset.
+        dataset (str): Name of dataset.
+        site (str): Local machine.
+        verbose (int): Verbosity level.
+        quiet (bool): Quiet mode.
+
+    Returns:
+        Optional[str]: Common path for dataset.
+    """
+    logger.setLevel("WARNING")
+    if verbose == 1:
+        logger.setLevel("INFO")
+    elif verbose > 1:
+        logger.setLevel("DEBUG")
+    elif quiet:
+        logger.setLevel("ERROR")
+    # Load configuration.
+    logger.debug("Loading configuration.")
+    try:
+        config = procure()
+        server = config["server"]
+        logger.debug(f"Server: {server}")
+        logger.debug("Configuration loaded successfully.")
+    except Exception:
+        logger.error(
+            "No configuration file found. Create one with `datatrail config init`."
+        )
+        logger.error("No config. Create one with `datatrail config init`.")
+        return None
+    # Query Datatrail Central Server.
+    logger.info(f"Querying Datatrail for {dataset} {scope}.")
+    payload = {"name": dataset, "scope": scope}
+    url = server + "/query/dataset/find"
+    logger.debug(f"URL: {url}")
+    try:
+        r = requests.post(url, json=payload)
+        dataset_locations = utilities.decode_response(r)  # type: ignore
+    except ConnectionError:
+        return "The Datatrail Central Server at CHIME at is not reachable!!!"
+    # Build data paths.
+    if dataset_locations["file_replica_locations"].get("minoc"):  # type: ignore
+        file_uris = dataset_locations["file_replica_locations"]["minoc"]  # type: ignore
+        file_paths = [f.replace("cadc:CHIMEFRB/", "") for f in file_uris]
+
+        common_path = os.path.commonprefix(file_paths).replace("//", "/")
+        if common_path[-1] != "/":
+            common_path = "/".join(common_path.split("/")[:-1])
+
+    else:
+        logger.info(f"Dataset {dataset} {scope} not found on Minoc.")
+        logger.info("Cannot clear dataset.")
+        return None
+
+    return common_path
```

### Comparing `datatrail_cli-0.2.0/dtcli/utilities/cadcclient.py` & `datatrail_cli-0.3.0/dtcli/utilities/cadcclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,70 +73,97 @@
 
 
 def get(
     source: List[str],
     destination: List[str],
     certfile: Optional[str] = None,
     namespace: str = "cadc:CHIMEFRB",
+    verbose: int = 0,
 ):
     """Retrieve a file, stored on the CANFAR file server, and copy it locally.
 
     Args:
         source (List[str]): List of source files to retrieve.
         destination (List[str]): List of destination files to copy to.
         certfile (Optional[str], optional): Certificate. Defaults to None.
         namespace (str): Minoc Namespace. Defaults to "cadc:CHIMEFRB".
+        verbose (int): Verbosity level. Defaults to 0.
     """
+    # Set logging level.
+    logger.setLevel("WARNING")
+    if verbose == 1:
+        logger.setLevel("INFO")
+    elif verbose > 1:
+        logger.setLevel("DEBUG")
+
+    logger.info("Connecting to CADC...")
     _, storage, _ = _connect(certfile=certfile)
+    not_found: List[str] = []
     try:
+        logger.debug("Checking source and destination length match.")
+        logger.debug(f"Source length: {len(source)}")
+        logger.debug(f"Destination length: {len(destination)}")
         assert len(source) == len(destination), (
             "The number of source files must match the number of destination files."
             f"Got {len(source)} source files and {len(destination)} destination files."
         )
         for index, filename in enumerate(source):
-            filename = namespace + "/" + filename
-            storage.cadcget(filename, destination[index])  # type: ignore
-            logger.debug(f"{filename} ➜ {destination[index]} ✔")
-    except cadcutils.exceptions.NotFoundException as error:  # type: ignore
-        logger.error(f"CADC Exception: {error}")
-        raise error
+            try:
+                filename = namespace + "/" + filename
+                storage.cadcget(filename, destination[index])  # type: ignore
+                logger.debug(f"{filename} ➜ {destination[index]} ✔")
+            except cadcutils.exceptions.NotFoundException as error:  # type: ignore
+                logger.error(f"CADC Exception: {filename}")
+                not_found.append(str(error))
     except cadcutils.exceptions.HttpException as error:  # type: ignore
         logger.error(f"CADC Exception: {error}")
         raise error
     except Exception as error:
         logger.error(f"Error: {error}")
         raise error
+    if len(not_found) > 0:
+        logger.error(f"Number of files not found: {len(not_found)}")
+        logger.error(f"Not found: {not_found}")
     logger.info(f"Process {os.getpid()} finished.")
 
 
 def pget(
     source: List[str],
     destination: List[str],
     certfile: Optional[str] = None,
     namespace: str = "cadc:CHIMEFRB",
     processors: int = os.cpu_count() or 1,
+    verbose: int = 0,
 ):
     """Parallelly retrieve files, stored on the CANFAR file server, and copy it locally.
 
     Args:
         source (List[str]): List of source files to retrieve.
         destination (List[str]): List of destination files to copy to.
         certfile (Optional[str], optional): Certificate. Defaults to None.
         namespace (_type_, optional): Minoc Namespace. Defaults to "cadc:CHIMEFRB".
         processors (int, optional): Number of processes to use.
             Defaults to os.cpu_count() or 1.
+        verbose (int, optional): Verbosity level. Defaults to 0.
     """
+    # Set logging level.
+    logger.setLevel("WARNING")
+    if verbose == 1:
+        logger.setLevel("INFO")
+    elif verbose > 1:
+        logger.setLevel("DEBUG")
+
     sources: List[List[Any]] = split(source, processors)
     destinations: List[List[Any]] = split(destination, processors)
     logger.info(f"Starting {processors} processes.")
     processes: List[DillProcess] = []
     for process in range(processors):
         mp = DillProcess(
             target=get,
-            args=(sources[process], destinations[process], certfile, namespace),
+            args=(sources[process], destinations[process], certfile, namespace, verbose),
         )
         processes.append(mp)
     for proc in processes:
         proc.start()
     for proc in processes:
         proc.join()
```

### Comparing `datatrail_cli-0.2.0/dtcli/utilities/utilities.py` & `datatrail_cli-0.3.0/dtcli/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.2.0/pyproject.toml` & `datatrail_cli-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datatrail-cli"
-version = "0.2.0"
+version = "0.3.0"
 description = "CHIME/FRB Datatrail CLI"
 authors = ["CHIME FRB Project Office"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dtcli" }]
 
 [tool.poetry.dependencies]
```

### Comparing `datatrail_cli-0.2.0/PKG-INFO` & `datatrail_cli-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrail-cli
-Version: 0.2.0
+Version: 0.3.0
 Summary: CHIME/FRB Datatrail CLI
 License: MIT
 Author: CHIME FRB Project Office
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datatrail-cli Version: 0.2.0 Summary: CHIME/FRB
+Metadata-Version: 2.1 Name: datatrail-cli Version: 0.3.0 Summary: CHIME/FRB
 Datatrail CLI License: MIT Author: CHIME FRB Project Office Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: cadcdata (>=2.4,<3.0) Requires-Dist: cadctap
 (>=0.9.11,<0.10.0) Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0) Requires-Dist:
```

