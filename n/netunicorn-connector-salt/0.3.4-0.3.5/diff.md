# Comparing `tmp/netunicorn-connector-salt-0.3.4.tar.gz` & `tmp/netunicorn-connector-salt-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-salt-0.3.4.tar", last modified: Wed May 10 04:48:47 2023, max compression
+gzip compressed data, was "netunicorn-connector-salt-0.3.5.tar", last modified: Mon Jun  5 20:24:20 2023, max compression
```

## Comparing `netunicorn-connector-salt-0.3.4.tar` & `netunicorn-connector-salt-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.340055 netunicorn-connector-salt-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-10 04:48:28.000000 netunicorn-connector-salt-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-10 04:48:47.340055 netunicorn-connector-salt-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-10 04:48:28.000000 netunicorn-connector-salt-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-10 04:48:28.000000 netunicorn-connector-salt-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 04:48:47.340055 netunicorn-connector-salt-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.336055 netunicorn-connector-salt-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.336055 netunicorn-connector-salt-0.3.4/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.336055 netunicorn-connector-salt-0.3.4/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.336055 netunicorn-connector-salt-0.3.4/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.340055 netunicorn-connector-salt-0.3.4/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:28.000000 netunicorn-connector-salt-0.3.4/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22393 2023-05-10 04:48:28.000000 netunicorn-connector-salt-0.3.4/src/netunicorn/director/infrastructure/connectors/salt_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.340055 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-10 04:48:47.000000 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-10 04:48:47.000000 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:48:47.000000 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 04:48:47.000000 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:48:47.000000 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.027721 netunicorn-connector-salt-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 20:24:03.000000 netunicorn-connector-salt-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-05 20:24:20.027721 netunicorn-connector-salt-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-05 20:24:03.000000 netunicorn-connector-salt-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-05 20:24:03.000000 netunicorn-connector-salt-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:24:20.027721 netunicorn-connector-salt-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.015721 netunicorn-connector-salt-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.015721 netunicorn-connector-salt-0.3.5/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.015721 netunicorn-connector-salt-0.3.5/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.015721 netunicorn-connector-salt-0.3.5/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.015721 netunicorn-connector-salt-0.3.5/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:03.000000 netunicorn-connector-salt-0.3.5/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22508 2023-06-05 20:24:03.000000 netunicorn-connector-salt-0.3.5/src/netunicorn/director/infrastructure/connectors/salt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:24:20.027721 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-05 20:24:20.000000 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 20:24:20.000000 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:24:20.000000 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 20:24:20.000000 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 20:24:20.000000 netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-salt-0.3.4/LICENSE` & `netunicorn-connector-salt-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.4/PKG-INFO` & `netunicorn-connector-salt-0.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.4
+Version: 0.3.5
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-salt-0.3.4/README.md` & `netunicorn-connector-salt-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.4/pyproject.toml` & `netunicorn-connector-salt-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-connector-salt"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "SaltStack connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-connector-salt-0.3.4/src/netunicorn/director/infrastructure/connectors/salt_connector.py` & `netunicorn-connector-salt-0.3.5/src/netunicorn/director/infrastructure/connectors/salt_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,38 +26,40 @@
         config_file: str | None,
         netunicorn_gateway: str,
         logger: Optional[logging.Logger] = None,
     ):
         self.connector_name = connector_name
         self.config_file = config_file
         self.netunicorn_gateway = netunicorn_gateway
+        if not logger:
+            logging.basicConfig(level=logging.DEBUG)
+            logger = logging.getLogger(__name__)
+        self.logger = logger
 
         self.config = {}
         if config_file:
             with open(config_file, "r") as f:
                 self.config = yaml.safe_load(f)
 
         self.PUBLIC_GRAINS: list[str] = self.config.get(
             "netunicorn.connector.salt.public_grains", ["location", "osarch", "kernel", "netunicorn-environments"]
         )
+        self.logger.debug(f"Grains: {self.PUBLIC_GRAINS}")
 
         self.endpoint = self.config.get(
             "netunicorn.connector.salt.endpoint"
         ).removesuffix("/")
+        self.logger.debug(f"Endpoint: {self.endpoint}")
+
         self.runpoint = self.endpoint + "/run"
         self.username = self.config.get("netunicorn.connector.salt.username")
         self.password = self.config.get("netunicorn.connector.salt.password")
         self.eauth = self.config.get("netunicorn.connector.salt.eauth")
         self.session = None
 
-        if not logger:
-            logging.basicConfig(level=logging.DEBUG)
-            logger = logging.getLogger(__name__)
-        self.logger = logger
-
     async def initialize(self) -> None:
         self.session = aiohttp.ClientSession(headers={"Accept": "application/json"})
         return
 
     async def health(self) -> Tuple[bool, str]:
         return True, "OK"
```

### Comparing `netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/PKG-INFO` & `netunicorn-connector-salt-0.3.5/src/netunicorn_connector_salt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.4
+Version: 0.3.5
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

