# Comparing `tmp/un_yaml-0.2.0.tar.gz` & `tmp/un_yaml-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "un_yaml-0.2.0.tar", max compression
+gzip compressed data, was "un_yaml-0.3.0.tar", max compression
```

## Comparing `un_yaml-0.2.0.tar` & `un_yaml-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-31 12:54:36.386488 un_yaml-0.2.0/LICENSE
--rw-r--r--   0        0        0      100 2023-05-31 12:54:36.387406 un_yaml-0.2.0/README.md
--rw-r--r--   0        0        0      751 2023-06-02 07:14:32.759061 un_yaml-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      441 2023-06-02 07:14:32.763817 un_yaml-0.2.0/un_yaml/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 07:14:32.763900 un_yaml-0.2.0/un_yaml/py.typed
--rw-r--r--   0        0        0     4071 2023-06-02 07:14:32.764583 un_yaml-0.2.0/un_yaml/un_cli.py
--rw-r--r--   0        0        0     1769 2023-06-02 07:14:32.765229 un_yaml-0.2.0/un_yaml/un_conf.py
--rw-r--r--   0        0        0     2180 2023-06-02 07:14:32.765632 un_yaml-0.2.0/un_yaml/un_uri.py
--rw-r--r--   0        0        0     2232 2023-06-02 07:14:32.766373 un_yaml-0.2.0/un_yaml/un_yaml.py
--rw-r--r--   0        0        0      190 2023-06-02 07:14:32.766902 un_yaml-0.2.0/un_yaml/wrapper.py
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 un_yaml-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 12:54:36.386488 un_yaml-0.3.0/LICENSE
+-rw-r--r--   0        0        0      100 2023-05-31 12:54:36.387406 un_yaml-0.3.0/README.md
+-rw-r--r--   0        0        0      751 2023-06-05 13:59:26.405560 un_yaml-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      441 2023-06-02 07:14:32.763817 un_yaml-0.3.0/un_yaml/__init__.py
+-rw-r--r--   0        0        0      695 2023-06-05 13:59:26.408347 un_yaml-0.3.0/un_yaml/cli.yaml
+-rw-r--r--   0        0        0        0 2023-06-02 07:14:32.763900 un_yaml-0.3.0/un_yaml/py.typed
+-rw-r--r--   0        0        0     4070 2023-06-05 13:59:26.409191 un_yaml-0.3.0/un_yaml/un_cli.py
+-rw-r--r--   0        0        0     1058 2023-06-05 13:59:26.409985 un_yaml-0.3.0/un_yaml/un_conf.py
+-rw-r--r--   0        0        0     2180 2023-06-02 07:14:32.765632 un_yaml-0.3.0/un_yaml/un_uri.py
+-rw-r--r--   0        0        0     3048 2023-06-05 13:59:26.410872 un_yaml-0.3.0/un_yaml/un_yaml.py
+-rw-r--r--   0        0        0      190 2023-06-02 07:14:32.766902 un_yaml-0.3.0/un_yaml/wrapper.py
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 un_yaml-0.3.0/PKG-INFO
```

### Comparing `un_yaml-0.2.0/LICENSE` & `un_yaml-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `un_yaml-0.2.0/pyproject.toml` & `un_yaml-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "un_yaml"
-version = "0.2.0"
+version = "0.3.0"
 description = "Universal YAML: replace repetitive code with your own Domain-Specific un-Language (DSuL)"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 anyio = "^3.7.0"
```

### Comparing `un_yaml-0.2.0/un_yaml/un_cli.py` & `un_yaml-0.3.0/un_yaml/un_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 import logging
 from argparse import ArgumentParser, Namespace
 from collections.abc import Sequence
-from importlib.metadata import version
 from pathlib import Path  # NOQA F401
 from sys import stdout
 from typing import Any
 
-__version__: str = version("un_yaml")
 
 from .un_conf import UnConf
 from .un_uri import UnUri
-from .un_yaml import UnYaml
+from .un_yaml import UnYaml, __version__
 
 # Harcode most parameters for now
 # TODO: infer them from the YAML file
 
 
 class UnCli(UnYaml):
     """Use UnYaml to create a CLI from a YAML file."""
 
     CLI_YAML = "cli.yaml"
     CMD = "commands"
     ARG_KEYS = (
         "dest,metavar,type,default,required,choices,action,nargs,const,help".split(",")
     )
+    K_VER = "version"
 
     @staticmethod
     def ARG_KWS(arg: dict):
         kwargs = {k: v for k, v in arg.items() if k in UnCli.ARG_KEYS}
         kwargs["type"] = eval(kwargs["type"]) if "type" in kwargs else str
         return kwargs
 
-    def __init__(self, file=CLI_YAML, dir=".") -> None:
-        yaml_data = UnYaml.LoadYaml(file, "tests")
+    def __init__(self, pkg: str, file=CLI_YAML, dir=".") -> None:
+        yaml_data = UnYaml.LoadYaml(file, pkg)
         super().__init__(yaml_data)
         if UnCli.CMD not in self.data:
             raise ValueError(f"'{UnCli.CMD}' not in file '{file}':\n{self.data}")
         self.cmds = self.get(UnCli.CMD)
         self.doc = self.get_handler("doc")()
-        self.path = Path(dir) / UnConf.DEFAULT
+        self.path = Path(dir) / UnCli.DEFAULT
         self.conf = UnConf(self.path, doc=type(self.doc).__name__)
 
     def parse_version(self, parser: ArgumentParser) -> None:
         doc_name = self.info("doc")
-        __version__ = version(doc_name)
         parser.add_argument(
             "-v",
-            "--version",
+            f"--{UnCli.K_VER}",
             action="store_const",
             const=f"{doc_name} {__version__}",
             help="Show version and exit.",
         )
 
     def make_parser(self) -> ArgumentParser:
         parser = ArgumentParser(self.get("doc"))
@@ -64,15 +62,15 @@
                     subparser.add_argument(arg["name"], **UnCli.ARG_KWS(arg))
         return parser
 
     async def run(self, argv: Sequence[str] | None, out=stdout):
         args: Any = self.parse(argv)
         if not args:
             return False
-        if hasattr(args, "version") and args.version:
+        if hasattr(args, UnCli.K_VER) and args.version:
             print(args.version, file=out)
             return False
         return await self.execute(args, out)
 
     def parse(self, argv: Sequence[str] | None) -> Namespace | None:
         parser = self.make_parser()
         args = parser.parse_args(argv)
@@ -83,17 +81,19 @@
 
     def get_resource(self, uri: UnUri) -> Any:
         handler = self.get_handler(uri.tool())
         logging.debug(f"handler: {handler}")
         return handler(uri.attrs)
 
     def log_resource(self, argv: dict):
-        uri = argv[UnUri.ARG_URI]
+        args = argv.copy()
+        args.pop(UnCli.K_VER, None)
+        uri = args.pop(UnUri.ARG_URI)
         tool = uri.tool()
-        opts = {str(uri): argv}
+        opts = {str(uri): args}
         logging.debug(f"tool[{tool}] {opts}")
         self.conf.put(tool, opts)
         self.conf.save()
 
     def resource(self, argv: dict) -> dict:
         """Hardcode resource transformation to key named URI, for now"""
         if UnUri.ARG_URI in argv:
```

### Comparing `un_yaml-0.2.0/un_yaml/un_uri.py` & `un_yaml-0.3.0/un_yaml/un_uri.py`

 * *Files identical despite different names*

### Comparing `un_yaml-0.2.0/un_yaml/un_yaml.py` & `un_yaml-0.3.0/un_yaml/un_yaml.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,58 @@
 from importlib import import_module, resources
+from importlib.metadata import version
 from typing import Any, Callable
+from pathlib import Path
 
 from yaml import safe_load
 
+__version__: str = version("un_yaml")
 
 class UnYaml:
     KEY = "_yaml"
     SEP = "/"
     PREFIX = "#/"
     REF = "$ref"
     REF_ERROR = f"Value for Key {REF} does not start with {PREFIX}"
+    DEFAULT = "data.yaml"
+    DEFAULT_INFO = {
+        "_version": __version__,
+        "app": "data-yaml",
+        "app_version": "0.0.1",
+        "doc": __name__,
+        "doc_version": "0.0.1",
+    }
 
-    @staticmethod
-    def LoadYaml(filename: str, pkg: str, sub: str = "") -> dict:
+    @classmethod
+    def LoadYaml(cls, filename: str, pkg: str, sub: str = "") -> dict:
         yaml_dir = resources.files(pkg)
         if len(sub) > 0:
             yaml_dir = yaml_dir / sub
         yaml_file = yaml_dir / filename
         yaml_string = yaml_file.read_text()
         yaml_data = safe_load(yaml_string)
         return yaml_data
 
+    @classmethod
+    def NewYaml(cls, info={}) -> dict:
+        opts = UnYaml.DEFAULT_INFO | {"doc": cls.__name__} | info
+        yaml_data = {UnYaml.KEY: opts}
+        return yaml_data
+
+    @classmethod
+    def ReadYaml(cls, path: Path, defaults={}) -> dict:
+        if not path.exists():
+            return cls.NewYaml(defaults)
+        yaml_string = path.read_text()
+        yaml_data = safe_load(yaml_string)
+
+        if not yaml_data:
+            return cls.NewYaml(defaults)
+        return yaml_data
+
     def __init__(self, yaml_data: dict) -> None:
         self.data = yaml_data
         assert self.data, "UnYaml: no data"
         self._info = self.data[UnYaml.KEY]
 
     def info(self, key: str) -> Any:
         return self._info.get(key)
```

### Comparing `un_yaml-0.2.0/PKG-INFO` & `un_yaml-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: un-yaml
-Version: 0.2.0
+Version: 0.3.0
 Summary: Universal YAML: replace repetitive code with your own Domain-Specific un-Language (DSuL)
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

