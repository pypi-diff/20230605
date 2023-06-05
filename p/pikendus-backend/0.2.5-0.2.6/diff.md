# Comparing `tmp/pikendus_backend-0.2.5.tar.gz` & `tmp/pikendus_backend-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikendus_backend-0.2.5.tar", last modified: Thu May 11 16:56:30 2023, max compression
+gzip compressed data, was "pikendus_backend-0.2.6.tar", last modified: Mon Jun  5 15:32:50 2023, max compression
```

## Comparing `pikendus_backend-0.2.5.tar` & `pikendus_backend-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/LICENSE
--rw-r--r--   0        0        0      728 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/README.md
--rw-r--r--   0        0        0     3082 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/PikendusWheelBuilder.py
--rw-r--r--   0        0        0     1702 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/__init__.py
--rw-r--r--   0        0        0     1371 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/__main__.py
--rw-r--r--   0        0        0     4228 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/compile.py
--rwxr-xr-x   0        0        0     1728 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/gene_py_src.py
--rwxr-xr-x   0        0        0     2114 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/ligne_debug.py
--rw-r--r--   0        0        0      823 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/main.py
--rw-r--r--   0        0        0    13981 2023-05-11 16:56:00.073698 pikendus_backend-0.2.5/pikendus_backend/structure.py
--rw-r--r--   0        0        0     3699 2023-05-11 16:56:30.750970 pikendus_backend-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 pikendus_backend-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-05 15:32:30.479823 pikendus_backend-0.2.6/LICENSE
+-rw-r--r--   0        0        0      850 2023-06-05 15:32:30.479823 pikendus_backend-0.2.6/README.md
+-rw-r--r--   0        0        0     3279 2023-06-05 15:32:30.479823 pikendus_backend-0.2.6/pikendus_backend/PikendusWheelBuilder.py
+-rw-r--r--   0        0        0     1521 2023-06-05 15:32:30.479823 pikendus_backend-0.2.6/pikendus_backend/__init__.py
+-rw-r--r--   0        0        0     1371 2023-06-05 15:32:30.479823 pikendus_backend-0.2.6/pikendus_backend/__main__.py
+-rw-r--r--   0        0        0     4441 2023-06-05 15:32:30.479823 pikendus_backend-0.2.6/pikendus_backend/compile.py
+-rwxr-xr-x   0        0        0     1595 2023-06-05 15:32:30.479823 pikendus_backend-0.2.6/pikendus_backend/gene_py_src.py
+-rwxr-xr-x   0        0        0     2359 2023-06-05 15:32:30.479823 pikendus_backend-0.2.6/pikendus_backend/ligne_debug.py
+-rw-r--r--   0        0        0      823 2023-06-05 15:32:30.479823 pikendus_backend-0.2.6/pikendus_backend/main.py
+-rw-r--r--   0        0        0    14417 2023-06-05 15:32:30.479823 pikendus_backend-0.2.6/pikendus_backend/structure.py
+-rw-r--r--   0        0        0     3699 2023-06-05 15:32:50.050527 pikendus_backend-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 pikendus_backend-0.2.6/PKG-INFO
```

### Comparing `pikendus_backend-0.2.5/LICENSE` & `pikendus_backend-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.5/pikendus_backend/PikendusWheelBuilder.py` & `pikendus_backend-0.2.6/pikendus_backend/PikendusWheelBuilder.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,17 +44,22 @@
 
         module_name = (
             context.config.data["project"]["name"].replace("-", "_").replace(" ", "_").lower()
         )
 
         tool_config = context.config.data.get("tool", dict())
         pikendus_config = tool_config.get("pikendus", dict())
-        structure_description = pikendus_config.get(
-            "structure_description", "data_struct/description.yaml"
-        )
+        structure_description = pikendus_config.get("structure_description", None)
+        if structure_description is None:
+            raise ValueError(
+                "Keyword 'structure_description' not found "
+                "in pyproject.toml's [tool.pikendus] section"
+            )
+
+        # if structure_description
         type_files = generateTypeHeaders(
             root=Path(structure_description),
             out_file=context.build_dir / module_name / "pikendus_types",
         )
         for file in type_files:
             yield file.relative_to(context.build_dir).as_posix(), file
```

### Comparing `pikendus_backend-0.2.5/pikendus_backend/__init__.py` & `pikendus_backend-0.2.6/pikendus_backend/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,8 @@
 # -*- coding: utf-8 -*-
-"""
-
-# Testing
-
-## Run the tests
-
-To run tests, just run:
-
-    pdm run pytest
-
-## Test reports
-
-[See test report](../tests/report.html)
-
-[See coverage](../coverage/index.html)
-
-"""
 import os
 import logging
 
 from rich.logging import RichHandler
 from setuptools_scm import get_version  # type: ignore
```

### Comparing `pikendus_backend-0.2.5/pikendus_backend/__main__.py` & `pikendus_backend-0.2.6/pikendus_backend/__main__.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.5/pikendus_backend/compile.py` & `pikendus_backend-0.2.6/pikendus_backend/compile.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,24 @@
 import numpy
 import numpy.f2py
 
 from .ligne_debug import ligne_debug
 
 
 def compile(pdm_build_dir: Path, src_dir: Path) -> Path:
+    """Generate the shared library
+
+    Args:
+        pdm_build_dir: build dir used by the pdm backend
+        src_dir: library's source directory
+
+    Returns:
+        Path to the created shared library
+
+    """
     from . import logger
 
     build_dir = Path(".pikendus").absolute()
     if build_dir.exists() and not build_dir.is_dir():
         raise AssertionError(f"{build_dir} is not a directory")
     build_dir.mkdir(parents=True, exist_ok=True)
```

### Comparing `pikendus_backend-0.2.5/pikendus_backend/gene_py_src.py` & `pikendus_backend-0.2.6/pikendus_backend/gene_py_src.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 import subprocess
-from typing import List
-
-
-def liste_fic(root: Path, pattern: str = "**/*", ext: List[str] = ["*"]) -> List[Path]:
-    list_fic = []
-    found = root.rglob(f"{pattern}.*")
-    list_fic.extend((f for f in found if f.is_file() and f.suffix in ext or "*" in ext))
-
-    return list_fic
 
 
 def generate_wrappers(
     config: dict,
     src_dir: Path,
     pdm_build_dir: Path,
 ):
-    "Génération des wrappers python"
+    """Génération des wrappers python
+
+    Args:
+        config: Configuration data
+        src_dir: library's source directory
+        pdm_build_dir: build dir used by the pdm backend
+
+    """
     src_dir = src_dir.expanduser().resolve()
     pdm_build_dir = pdm_build_dir.expanduser().resolve()
 
     module_name = config["project"]["name"].replace("-", "_").replace(" ", "_").lower()
     nom = f"_{module_name}"
 
     sig_fic = None
     for sig_fic in src_dir.rglob("*.pyf"):
         pass
     if sig_fic is None:
         raise AssertionError("pyf file not found")
 
     dst_dir = pdm_build_dir / module_name
 
-    l_src_found = liste_fic(root=src_dir, ext=[".f"])
+    l_src_found = list(src_dir.rglob("*.f"))
     l_src = list()
     for pth in l_src_found:
         s = str(pth)
         # Suppression de la liste des sources générés par
         # une précédente compilation
         if (
             "fortranobject" not in s
```

### Comparing `pikendus_backend-0.2.5/pikendus_backend/ligne_debug.py` & `pikendus_backend-0.2.6/pikendus_backend/ligne_debug.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,33 @@
 
 import codecs
 from os.path import basename
 from pathlib import Path
 
 
 class LigneDebugApp(object):
-    def __init__(self, src, dst):
+    """Class to handle [DEBUG], [INFO], [WARNING] and [ERROR] messages in fortran sources
+
+    Args:
+        src: Path to a fortran source to analyse
+        dst: Path to the file where the modified source should be written
+
+    """
+
+    def __init__(self, src: Path, dst: Path):
         self.src = src
         self.dst = dst
 
-    def traite(self, deb):
-        f = codecs.open(self.src, "r", "latin-1")
-        g = codecs.open(self.dst, "w", "latin-1")
+    def process(self, debug):
+        f = codecs.open(self.src, "r", "utf-8")
+        g = codecs.open(self.dst, "w", "utf-8")
 
         nf = basename(self.src)
 
-        balises = ["[DEBUG", "[ERREUR", "[ATTENTION", "[INFO"]
+        balises = ["[DEBUG", "[ERROR", "[WARNING", "[INFO"]
 
         self.num_line = 1
         self.line = f.readline()
         new_line = self.line
         while self.line != "":
             # Ajout des infos de num de ligne / nom de fichier
             for b in balises:
@@ -40,15 +48,15 @@
                             new_line[: i + lb]
                             + ("]<%.5i@%s>" % (self.num_line, nf))
                             + new_line[j + 1 :]
                         )
 
             # Suppression de "d" en début de ligne
             if len(new_line) > 0 and new_line[0] == "d":
-                if deb:
+                if debug:
                     new_line = " " + new_line[1:]
                 else:
                     new_line = ""
 
             g.write(new_line)
 
             self.line = f.readline()
@@ -60,8 +68,8 @@
     """Transformation des [DEBUG]Message en
     [DEBUG]<nl>@<nf>Message, où <nl> est le numéro de ligne et <nf> le nom du fichier.
     Créé une copie dans le nême dossier que l'original (extension .old)
 
     """
     app = LigneDebugApp(src, dst)
 
-    app.traite(debug)
+    app.process(debug)
```

### Comparing `pikendus_backend-0.2.5/pikendus_backend/main.py` & `pikendus_backend-0.2.6/pikendus_backend/main.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.5/pikendus_backend/structure.py` & `pikendus_backend-0.2.6/pikendus_backend/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import List
-import yaml
 
+import yaml
 import networkx as nx
 from networkx.algorithms.dag import topological_sort
 
 
 _itf_types_map = {
     "u1": "int",
     "u2": "int",
@@ -56,15 +56,26 @@
     "s8": "integer*8",
     "f4": "real*4",
     "f8": "real*8",
 }
 
 
 class Field(object):
-    def __init__(self, name: str, typ: str, niter: int, unit: str, description: str):
+    """Describe one field of a data structure
+
+    Args:
+        name: Name of the field
+        typ: Type of the field
+        niter: Number of element if the field is an array
+        unit: Unit of the field
+        description: Description of the field
+
+    """
+
+    def __init__(self, name: str, typ: str, niter: int = 1, unit: str = "", description: str = ""):
         self.name = name
         self.typ = typ
         self.niter = niter
         self.unit = unit
         self.descrption = description
 
     def isBasicType(self) -> bool:
@@ -101,14 +112,21 @@
         if self.niter == 1:
             return '        ("%s", %s),' % (self.name, ctyp)
         else:
             return '        ("%s", %s*%i),' % (self.name, ctyp, self.niter)
 
 
 class DataStructure(object):
+    """Description of a whole data structure
+
+    Args:
+        name: Name of the structure
+
+    """
+
     def __init__(self, name: str):
         self.name = name
         self.fields = []
         self.deps = []
 
     def addField(self, name: str, typ: str, niter: int, unit: str, description: str) -> Field:
         field = Field(name, typ, int(niter), unit, description)
@@ -162,14 +180,17 @@
     out_dir = out_file.parent
     out_dir.mkdir(exist_ok=True, parents=True)
 
     G = nx.DiGraph()
     with open(root, "r") as f:
         data = yaml.load(f, Loader=yaml.SafeLoader)
 
+    if not hasattr(data, "types"):
+        return []
+
     for ds_name in data["types"].keys():
         type_desc = data["types"][ds_name]
         ds = DataStructure.fromDict(ds_name, type_desc)
 
         G.add_node(ds.name, ds=ds)
         for dep in ds.deps:
             G.add_edge(dep.typ, ds.name)
```

### Comparing `pikendus_backend-0.2.5/pyproject.toml` & `pikendus_backend-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "numpy>=1.24.3",
     "toml>=0.10.2",
     "networkx>=3.1",
     "PyYAML>=6.0",
     "typer>=0.9.0",
 ]
 requires-python = ">3.8"
-version = "0.2.5"
+version = "0.2.6"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.com/ydethe/pikendus-backend/issues"
 Homepage = "https://gitlab.com/ydethe/pikendus-backend"
```

### Comparing `pikendus_backend-0.2.5/PKG-INFO` & `pikendus_backend-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikendus-backend
-Version: 0.2.5
+Version: 0.2.6
 Summary: A PEP517 compliant build backend, able to compile C and fortran source files
 Author-Email: Yann de Thé <yann@johncloud.fr>
 License: MIT License
         
         Copyright (c) 2023 Yann de Thé
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,17 +38,17 @@
 Requires-Dist: networkx>=3.1
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: typer>=0.9.0
 Description-Content-Type: text/markdown
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://dev.to/frostming/a-review-pipenv-vs-poetry-vs-pdm-39b4)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![Python](https://img.shields.io/badge/python-3.8-green)
-![Doc](htmldoc/doc_badge.svg)
-![Coverage](htmldoc/cov_badge.svg)
+[![Python](https://img.shields.io/badge/python-3.8-green)]()
+[![Doc](https://ydethe.gitlab.io/pikendus-backend/doc_badge.svg)](https://ydethe.gitlab.io/pikendus-backend/)
+[![Coverage](https://ydethe.gitlab.io/pikendus-backend/cov_badge.svg)]()
 
 # Quick look
 
 pikendus backend is a PEP517 compliant build backend, able to compile C and fortran source files
 pikendus is an estonian word that means 'extension'
 
 # Build the doc
```

