# Comparing `tmp/pikendus_backend-0.2.4.tar.gz` & `tmp/pikendus_backend-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikendus_backend-0.2.4.tar", last modified: Thu May 11 14:33:38 2023, max compression
+gzip compressed data, was "pikendus_backend-0.2.5.tar", last modified: Thu May 11 16:56:30 2023, max compression
```

## Comparing `pikendus_backend-0.2.4.tar` & `pikendus_backend-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-11 14:33:11.185458 pikendus_backend-0.2.4/LICENSE
--rw-r--r--   0        0        0      728 2023-05-11 14:33:11.185458 pikendus_backend-0.2.4/README.md
--rw-r--r--   0        0        0     3105 2023-05-11 14:33:11.185458 pikendus_backend-0.2.4/pikendus_backend/PikendusWheelBuilder.py
--rw-r--r--   0        0        0     1702 2023-05-11 14:33:11.185458 pikendus_backend-0.2.4/pikendus_backend/__init__.py
--rw-r--r--   0        0        0      823 2023-05-11 14:33:11.185458 pikendus_backend-0.2.4/pikendus_backend/main.py
--rwxr-xr-x   0        0        0     3459 2023-05-11 14:33:11.186458 pikendus_backend-0.2.4/pikendus_backend/scripts/calc_dep_f90.py
--rw-r--r--   0        0        0     4229 2023-05-11 14:33:11.186458 pikendus_backend-0.2.4/pikendus_backend/scripts/compile.py
--rwxr-xr-x   0        0        0     1728 2023-05-11 14:33:11.186458 pikendus_backend-0.2.4/pikendus_backend/scripts/gene_py_src.py
--rwxr-xr-x   0        0        0     2117 2023-05-11 14:33:11.186458 pikendus_backend-0.2.4/pikendus_backend/scripts/ligne_debug.py
--rw-r--r--   0        0        0    13199 2023-05-11 14:33:11.186458 pikendus_backend-0.2.4/pikendus_backend/structure.py
--rw-r--r--   0        0        0     2879 2023-05-11 14:33:38.565645 pikendus_backend-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 pikendus_backend-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/LICENSE
+-rw-r--r--   0        0        0      728 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/README.md
+-rw-r--r--   0        0        0     3082 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/PikendusWheelBuilder.py
+-rw-r--r--   0        0        0     1702 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/__init__.py
+-rw-r--r--   0        0        0     1371 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/__main__.py
+-rw-r--r--   0        0        0     4228 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/compile.py
+-rwxr-xr-x   0        0        0     1728 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/gene_py_src.py
+-rwxr-xr-x   0        0        0     2114 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/ligne_debug.py
+-rw-r--r--   0        0        0      823 2023-05-11 16:56:00.072697 pikendus_backend-0.2.5/pikendus_backend/main.py
+-rw-r--r--   0        0        0    13981 2023-05-11 16:56:00.073698 pikendus_backend-0.2.5/pikendus_backend/structure.py
+-rw-r--r--   0        0        0     3699 2023-05-11 16:56:30.750970 pikendus_backend-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 pikendus_backend-0.2.5/PKG-INFO
```

### Comparing `pikendus_backend-0.2.4/LICENSE` & `pikendus_backend-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.4/README.md` & `pikendus_backend-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.4/pikendus_backend/PikendusWheelBuilder.py` & `pikendus_backend-0.2.5/pikendus_backend/PikendusWheelBuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,24 @@
 from typing import IO, Iterable, Tuple
 from importlib.metadata import version as get_version
 
 from pdm.backend.hooks import Context
 from pdm.backend.wheel import WheelBuilder
 
 from .structure import generateTypeHeaders, generateFunctionHeaders
-from .scripts.compile import compile
-from .scripts.gene_py_src import generate_wrappers
+from .compile import compile
+from .gene_py_src import generate_wrappers
+
+
+WHEEL_FILE_FORMAT = """\
+Wheel-Version: 1.0
+Generator: pikendus-backend ({version})
+Root-Is-Purelib: {is_purelib}
+Tag: {tag}
+"""
 
 
 class PikendusWheelBuilder(WheelBuilder):
     """Wheel builder
 
     Args:
         context: the build context
@@ -63,21 +71,14 @@
             out_file=context.build_dir / module_name / "pikendus.py",
         )
         yield file_pth.relative_to(context.build_dir).as_posix(), file_pth
 
         yield from self._get_metadata_files(context)
 
     def _write_wheel_file(self, fp: IO[str], is_purelib: bool) -> None:
-        WHEEL_FILE_FORMAT = """\
-Wheel-Version: 1.0
-Generator: pikendus-backend ({version})
-Root-Is-Purelib: {is_purelib}
-Tag: {tag}
-"""
-
         try:
             version = get_version("pikendus-backend")
         except ModuleNotFoundError:
             version = "0.0.0+local"
 
         fp.write(
             WHEEL_FILE_FORMAT.format(
```

### Comparing `pikendus_backend-0.2.4/pikendus_backend/__init__.py` & `pikendus_backend-0.2.5/pikendus_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.4/pikendus_backend/main.py` & `pikendus_backend-0.2.5/pikendus_backend/main.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.4/pikendus_backend/scripts/compile.py` & `pikendus_backend-0.2.5/pikendus_backend/compile.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy
 import numpy.f2py
 
 from .ligne_debug import ligne_debug
 
 
 def compile(pdm_build_dir: Path, src_dir: Path) -> Path:
-    from .. import logger
+    from . import logger
 
     build_dir = Path(".pikendus").absolute()
     if build_dir.exists() and not build_dir.is_dir():
         raise AssertionError(f"{build_dir} is not a directory")
     build_dir.mkdir(parents=True, exist_ok=True)
 
     with open("pyproject.toml", "r") as f:
```

### Comparing `pikendus_backend-0.2.4/pikendus_backend/scripts/gene_py_src.py` & `pikendus_backend-0.2.5/pikendus_backend/gene_py_src.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.4/pikendus_backend/scripts/ligne_debug.py` & `pikendus_backend-0.2.5/pikendus_backend/ligne_debug.py`

 * *Files 13% similar despite different names*

```diff
@@ -54,14 +54,14 @@
             self.line = f.readline()
             new_line = self.line
             self.num_line += 1
 
 
 def ligne_debug(src: Path, dst: Path, debug: bool = False):
     """Transformation des [DEBUG]Message en
-    [DEBUG]<nl>@<nf> : Message, où <nl> est le numéro de ligne et <nf> le nom du fichier.
+    [DEBUG]<nl>@<nf>Message, où <nl> est le numéro de ligne et <nf> le nom du fichier.
     Créé une copie dans le nême dossier que l'original (extension .old)
 
     """
     app = LigneDebugApp(src, dst)
 
     app.traite(debug)
```

### Comparing `pikendus_backend-0.2.4/pikendus_backend/structure.py` & `pikendus_backend-0.2.5/pikendus_backend/structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             description = field.get("description", "")
 
             ds.addField(name, typ, int(niter), unit, description)
 
         return ds
 
 
-def generateTypeHeaders(root: Path, out_file: Path) -> List[Path]:
+def generateTypeHeaders(root: Path, out_file: Path, markdown: bool = False) -> List[Path]:
     created_files = []
 
     out_dir = out_file.parent
     out_dir.mkdir(exist_ok=True, parents=True)
 
     G = nx.DiGraph()
     with open(root, "r") as f:
@@ -175,50 +175,83 @@
             G.add_edge(dep.typ, ds.name)
 
     list_ds = list(topological_sort(G))
 
     # Generation header C
     fn = out_file.stem
     macro_name = "_%s_H_" % fn.upper()
-    res = [f"// {out_file}.h", "", "#include <stdint.h>", "", ""]
+    if markdown:
+        res = ["```c"]
+    else:
+        res = []
+    res.extend([f"// {out_file}.h", "", "#include <stdint.h>", "", ""])
     res.append("#ifndef %s" % macro_name)
     res.append("#define %s" % macro_name)
     res.append("")
     for ds in list_ds:
         res.append(G.nodes[ds]["ds"].toCHeader())
         res.append("")
     res.append("#endif")
     res.append("")
 
-    with open(f"{out_file}.h", "w") as f:
+    if markdown:
+        res.append("```")
+
+    h_file = f"{out_file}.h"
+    if markdown:
+        h_file += ".md"
+
+    with open(h_file, "w") as f:
         f.write("\n".join(res))
-        created_files.append(Path(f"{out_file}.h"))
+        created_files.append(Path(h_file))
 
     # Generation header Fortran
-    res = [f"! {out_file}.finc"]
+    if markdown:
+        res = ["```fortran"]
+    else:
+        res = []
+    res.append(f"! {out_file}.finc")
     res.append("")
     for ds in list_ds:
         res.append(G.nodes[ds]["ds"].toFHeader())
         res.append("")
 
-    with open(f"{out_file}.finc", "w") as f:
+    if markdown:
+        res.append("```")
+
+    finc_file = f"{out_file}.finc"
+    if markdown:
+        finc_file += ".md"
+
+    with open(finc_file, "w") as f:
         f.write("\n".join(res))
-        created_files.append(Path(f"{out_file}.finc"))
+        created_files.append(Path(finc_file))
 
     # Generation header Python
-    res = [f"# {out_file}.py"]
+    if markdown:
+        res = ["```python"]
+    else:
+        res = []
+    res.append(f"# {out_file}.py")
     res.append("")
     res.extend(["import ctypes", "", ""])
     for ds in list_ds:
         res.append(G.nodes[ds]["ds"].toPyHeader())
         res.append("")
 
-    with open(f"{out_file}.py", "w") as f:
+    if markdown:
+        res.append("```")
+
+    py_file = f"{out_file}.py"
+    if markdown:
+        py_file += ".md"
+
+    with open(py_file, "w") as f:
         f.write("\n".join(res))
-        created_files.append(Path(f"{out_file}.py"))
+        created_files.append(Path(py_file))
 
     return created_files
 
 
 def descToPython(build_dir: Path, dat: dict, pkg_name: str, type_files: List[Path]) -> str:
     code = ["import ctypes"]
     code.append("from ctypes import byref, addressof")
@@ -397,22 +430,33 @@
         code.append("")
         code.append("")
 
     return "\n".join(code)
 
 
 def generateFunctionHeaders(
-    build_dir: Path, root: Path, type_files: List[Path], pkg_name: str, out_file: Path
+    build_dir: Path,
+    root: Path,
+    type_files: List[Path],
+    pkg_name: str,
+    out_file: Path,
+    markdown: bool = False,
 ) -> Path:
     with open(root, "r") as f:
         data = yaml.load(f, Loader=yaml.SafeLoader)
 
     code = descToPython(build_dir, data["functions"], pkg_name, type_files)
+    if markdown:
+        out_file = out_file.parent / (out_file.name + ".md")
     with open(out_file, "w") as f:
+        if markdown:
+            f.write("```python\n")
         f.write(code)
+        if markdown:
+            f.write("\n```")
 
     return out_file.absolute()
 
 
 if __name__ == "__main__":
     type_files = generateTypeHeaders(
         Path("tests/ma_librairie/data_struct/description.yaml"),
```

### Comparing `pikendus_backend-0.2.4/PKG-INFO` & `pikendus_backend-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikendus-backend
-Version: 0.2.4
+Version: 0.2.5
 Summary: A PEP517 compliant build backend, able to compile C and fortran source files
 Author-Email: Yann de Thé <yann@johncloud.fr>
 License: MIT License
         
         Copyright (c) 2023 Yann de Thé
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,14 +33,15 @@
 Requires-Dist: setuptools-scm>=7.1
 Requires-Dist: pdm-backend>=2.0.6
 Requires-Dist: wheel>=0.40.0
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: toml>=0.10.2
 Requires-Dist: networkx>=3.1
 Requires-Dist: PyYAML>=6.0
+Requires-Dist: typer>=0.9.0
 Description-Content-Type: text/markdown
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://dev.to/frostming/a-review-pipenv-vs-poetry-vs-pdm-39b4)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![Python](https://img.shields.io/badge/python-3.8-green)
 ![Doc](htmldoc/doc_badge.svg)
 ![Coverage](htmldoc/cov_badge.svg)
```

