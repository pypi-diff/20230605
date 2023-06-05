# Comparing `tmp/bibtex2cff-0.2.0.tar.gz` & `tmp/bibtex2cff-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibtex2cff-0.2.0.tar", max compression
+gzip compressed data, was "bibtex2cff-0.2.1.tar", max compression
```

## Comparing `bibtex2cff-0.2.0.tar` & `bibtex2cff-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1079 2023-05-28 13:15:37.013069 bibtex2cff-0.2.0/LICENSE
--rw-r--r--   0        0        0     1014 2023-05-28 13:15:37.013069 bibtex2cff-0.2.0/README.md
--rw-r--r--   0        0        0     2518 2023-05-28 13:15:37.013069 bibtex2cff-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-05-28 13:15:37.013069 bibtex2cff-0.2.0/src/bibtex2cff/__init__.py
--rw-r--r--   0        0        0     6342 2023-05-28 13:15:37.013069 bibtex2cff-0.2.0/src/bibtex2cff/cmd.py
--rw-r--r--   0        0        0     8753 2023-05-28 13:15:37.013069 bibtex2cff-0.2.0/src/bibtex2cff/convert_cff.py
--rw-r--r--   0        0        0    11256 2023-05-28 13:15:37.013069 bibtex2cff-0.2.0/src/bibtex2cff/definitions.py
--rw-r--r--   0        0        0     2045 1970-01-01 00:00:00.000000 bibtex2cff-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-05 18:30:33.967322 bibtex2cff-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1110 2023-06-05 18:30:33.967322 bibtex2cff-0.2.1/README.md
+-rw-r--r--   0        0        0     2508 2023-06-05 18:30:33.967322 bibtex2cff-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-05 18:30:33.967322 bibtex2cff-0.2.1/src/bibtex2cff/__init__.py
+-rw-r--r--   0        0        0     6344 2023-06-05 18:30:33.967322 bibtex2cff-0.2.1/src/bibtex2cff/cmd.py
+-rw-r--r--   0        0        0     9481 2023-06-05 18:30:33.967322 bibtex2cff-0.2.1/src/bibtex2cff/convert_cff.py
+-rw-r--r--   0        0        0    11256 2023-06-05 18:30:33.967322 bibtex2cff-0.2.1/src/bibtex2cff/definitions.py
+-rw-r--r--   0        0        0     2137 1970-01-01 00:00:00.000000 bibtex2cff-0.2.1/PKG-INFO
```

### Comparing `bibtex2cff-0.2.0/LICENSE` & `bibtex2cff-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bibtex2cff-0.2.0/README.md` & `bibtex2cff-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # BibTeX2CFF
 
 [![PyPI](https://img.shields.io/pypi/v/bibtex2cff?logo=pypi&logoColor=yellow)](https://pypi.org/project/bibtex2cff/)
+[![DOI](https://zenodo.org/badge/642463530.svg)](https://zenodo.org/badge/latestdoi/642463530)
+
 
 ## Description
 
 This is a simple CMD-tool to convert BibTeX files to CFF files. It is dedicated to the [Citation File Format](https://citation-file-format.github.io/), which is a YAML-based format for bibliographic metadata.
 
 The idea is faster to generate CFF files from BibTeX files, which can be used in other tools, such as [Zenodo](https://zenodo.org/).
```

### Comparing `bibtex2cff-0.2.0/pyproject.toml` & `bibtex2cff-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bibtex2cff"
-version = "0.2.0"
+version = "0.2.1"
 description = "Converting Bibtex to CITATION.cff fileformat"
 authors = ["Anselm Hahn <anselm.hahn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bibtex2cff", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -17,15 +17,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Markup :: LaTeX",
 ]
 keywords = ["bibtex", "cff", "citation", "citation-file-format"]
 
 
     [tool.poetry.dependencies]
-    python = "^3.8.1"
+    python = "^3.9"
     bibtexparser = "^1.4.0"
     pydantic = { extras = ["email"], version = "^1.10.7" }
     pyyaml = "^6.0"
 
 
     [tool.poetry.group.dev.dependencies]
     pytest = "^7.3.1"
@@ -57,15 +57,15 @@
 src_paths = ["poetry", "tests"]
 skip_glob = ["*/setup.py"]
 filter_files = true
 known_first_party = "poetry"
 
 [tool.black]
 line-length = 88
-target-version = ["py38", "py39", "py310", "py311"]
+target-version = ["py39", "py310", "py311"]
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
```

### Comparing `bibtex2cff-0.2.0/src/bibtex2cff/cmd.py` & `bibtex2cff-0.2.1/src/bibtex2cff/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Command line interface for bibtex2cff."""
 import argparse as ap
 
 from pathlib import Path
 
 from bibtex2cff import __version__
-from bibtex2cff.convert_cff import CFFDefintionUpdate
+from bibtex2cff.convert_cff import CFFDefinitionUpdate
 from bibtex2cff.convert_cff import save_cff_definition
 
 
 def cmd() -> ap.Namespace:
     """Parse command line arguments and return a Namespace object."""
     parser = ap.ArgumentParser(
         prog="bibtex2cff",
@@ -218,14 +218,14 @@
 
 
 def main() -> None:
     """Main function for bibtex2cff."""
     args = cmd()
 
     bibtex_path = args.bibfile
-    definition = CFFDefintionUpdate(
+    definition = CFFDefinitionUpdate(
         bibtex_path, **{k: v for k, v in vars(args).items() if v is not None}
     ).get_definition
     if args.outfile:
         save_cff_definition(definition, Path.cwd(), args.outfile)
     else:
         save_cff_definition(definition)
```

### Comparing `bibtex2cff-0.2.0/src/bibtex2cff/convert_cff.py` & `bibtex2cff-0.2.1/src/bibtex2cff/convert_cff.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,15 +217,15 @@
             "software": SoftwareDefinition,
             "datatset": DatasetDefinition,
             "misc": DatasetDefinition,
         }
         return definitions[_type](kwargs)()
 
 
-class CFFDefintionUpdate(DefinitionBridge):
+class CFFDefinitionUpdate(DefinitionBridge):
     """Class for updating CFF definitions."""
 
     def __init__(self, bibtex_path: str, **kwargs: Dict[str, Any]) -> None:
         """Initialize the class with default, BibTeX, and optional definitions.
 
         Args:
             bibtex_path (str): The path to the BibTeX file.
@@ -244,15 +244,37 @@
 
         Returns:
             Dict[str, Any]: A dictionary representation of the CFF entry.
         """
         definition = self.default().get_definition
         definition.update(self.bibtex(self.bibtex_path).get_definition)
         definition.update(self.optional(definition, **self.kwargs).get_definition)
-        return CFFDefinition(**definition).dict(exclude_none=True, by_alias=True)
+        return self.replace_hyphens_with_underscores(
+            CFFDefinition(**definition).dict(exclude_none=True, by_alias=True)
+        )
+
+    def replace_hyphens_with_underscores(self, data: Dict[str, Any]) -> Dict[str, Any]:
+        """Replace hyphens with underscores in a dictionary.
+
+        Args:
+
+            data (Dict[str, Any]): A dictionary.
+
+        Returns:
+            Dict[str, Any]: A dictionary with hyphens replaced with underscores.
+        """
+        if isinstance(data, dict):
+            return {
+                k.replace("_", "-"): self.replace_hyphens_with_underscores(v)
+                for k, v in data.items()
+            }
+        elif isinstance(data, list):
+            return [self.replace_hyphens_with_underscores(v) for v in data]
+        else:
+            return data
 
 
 def save_cff_definition(
     cff_definition: Dict[str, Any],
     directory: Optional[Path] = None,
     citation_cff: str = "CITATION.cff",
 ) -> None:
```

### Comparing `bibtex2cff-0.2.0/src/bibtex2cff/definitions.py` & `bibtex2cff-0.2.1/src/bibtex2cff/definitions.py`

 * *Files identical despite different names*

### Comparing `bibtex2cff-0.2.0/PKG-INFO` & `bibtex2cff-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bibtex2cff
-Version: 0.2.0
+Version: 0.2.1
 Summary: Converting Bibtex to CITATION.cff fileformat
 License: MIT
 Keywords: bibtex,cff,citation,citation-file-format
 Author: Anselm Hahn
 Author-email: anselm.hahn@gmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -23,14 +23,16 @@
 Requires-Dist: pydantic[email] (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 # BibTeX2CFF
 
 [![PyPI](https://img.shields.io/pypi/v/bibtex2cff?logo=pypi&logoColor=yellow)](https://pypi.org/project/bibtex2cff/)
+[![DOI](https://zenodo.org/badge/642463530.svg)](https://zenodo.org/badge/latestdoi/642463530)
+
 
 ## Description
 
 This is a simple CMD-tool to convert BibTeX files to CFF files. It is dedicated to the [Citation File Format](https://citation-file-format.github.io/), which is a YAML-based format for bibliographic metadata.
 
 The idea is faster to generate CFF files from BibTeX files, which can be used in other tools, such as [Zenodo](https://zenodo.org/).
```

