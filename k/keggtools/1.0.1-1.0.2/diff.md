# Comparing `tmp/keggtools-1.0.1.tar.gz` & `tmp/keggtools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keggtools-1.0.1.tar", last modified: Mon Oct  3 19:02:24 2022, max compression
+gzip compressed data, was "keggtools-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `keggtools-1.0.1.tar` & `keggtools-1.0.2.tar`

### file list

```diff
@@ -1,53 +1,21 @@
--rw-r--r--   0        0        0     1155 2022-10-03 18:10:20.169325 keggtools-1.0.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2289 2022-10-03 18:25:58.687610 keggtools-1.0.1/.github/workflows/package.yml
--rw-r--r--   0        0        0     2069 2022-10-03 18:32:22.809225 keggtools-1.0.1/.gitignore
--rw-r--r--   0        0        0     1645 2022-10-03 18:24:35.312126 keggtools-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1029 2022-10-03 18:56:01.596374 keggtools-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0     1344 2022-08-15 17:25:03.794817 keggtools-1.0.1/INSTALL.md
--rw-r--r--   0        0        0     1071 2021-01-20 18:48:18.741520 keggtools-1.0.1/LICENSE
--rw-r--r--   0        0        0     3844 2022-10-03 18:39:44.758472 keggtools-1.0.1/Makefile
--rw-r--r--   0        0        0     2402 2022-10-03 18:35:08.228196 keggtools-1.0.1/README.md
--rwxr-xr-x   0        0        0      920 2022-10-03 18:59:52.434932 keggtools-1.0.1/keggtools/__init__.py
--rw-r--r--   0        0        0      143 2021-10-10 17:12:25.507941 keggtools-1.0.1/keggtools/__pycache__/__init__.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0      746 2022-09-16 16:52:16.662464 keggtools-1.0.1/keggtools/__pycache__/__init__.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0        0        0     1162 2022-10-03 18:59:52.942929 keggtools-1.0.1/keggtools/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      629 2022-08-26 10:59:58.452887 keggtools-1.0.1/keggtools/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7215 2021-10-10 17:12:25.564010 keggtools-1.0.1/keggtools/__pycache__/analysis.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     8304 2022-09-16 16:52:16.662464 keggtools-1.0.1/keggtools/__pycache__/analysis.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0        0        0     8203 2022-10-03 18:19:25.146036 keggtools-1.0.1/keggtools/__pycache__/analysis.cpython-36.pyc
--rw-r--r--   0        0        0     8232 2022-08-26 10:59:58.452887 keggtools-1.0.1/keggtools/__pycache__/analysis.cpython-38.pyc
--rw-r--r--   0        0        0     1903 2021-10-10 17:12:26.328915 keggtools-1.0.1/keggtools/__pycache__/const.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1978 2022-09-16 16:52:16.862426 keggtools-1.0.1/keggtools/__pycache__/const.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0        0        0    10846 2022-10-03 18:54:55.640786 keggtools-1.0.1/keggtools/__pycache__/const.cpython-36.pyc
--rw-r--r--   0        0        0     1923 2022-08-26 10:59:58.664882 keggtools-1.0.1/keggtools/__pycache__/const.cpython-38.pyc
--rw-r--r--   0        0        0     8389 2021-10-10 18:05:17.316280 keggtools-1.0.1/keggtools/__pycache__/models.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    27246 2022-09-16 16:52:16.862426 keggtools-1.0.1/keggtools/__pycache__/models.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0        0        0    23816 2022-10-03 18:19:25.338035 keggtools-1.0.1/keggtools/__pycache__/models.cpython-36.pyc
--rw-r--r--   0        0        0    23813 2022-08-26 10:59:58.660882 keggtools-1.0.1/keggtools/__pycache__/models.cpython-38.pyc
--rw-r--r--   0        0        0    11349 2021-10-10 18:05:17.320280 keggtools-1.0.1/keggtools/__pycache__/render.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     9939 2022-09-16 16:52:16.866425 keggtools-1.0.1/keggtools/__pycache__/render.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0        0        0     9854 2022-10-03 18:19:25.342035 keggtools-1.0.1/keggtools/__pycache__/render.cpython-36.pyc
--rw-r--r--   0        0        0     9763 2022-08-26 10:59:58.664882 keggtools-1.0.1/keggtools/__pycache__/render.cpython-38.pyc
--rw-r--r--   0        0        0     5020 2021-10-10 18:05:17.264279 keggtools-1.0.1/keggtools/__pycache__/resolver.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     7695 2022-09-17 12:02:07.970817 keggtools-1.0.1/keggtools/__pycache__/resolver.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0        0        0     7541 2022-10-03 18:19:25.362035 keggtools-1.0.1/keggtools/__pycache__/resolver.cpython-36.pyc
--rw-r--r--   0        0        0     5480 2022-08-26 11:00:08.192639 keggtools-1.0.1/keggtools/__pycache__/resolver.cpython-38.pyc
--rw-r--r--   0        0        0     7557 2021-10-10 18:05:17.312280 keggtools-1.0.1/keggtools/__pycache__/storage.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4471 2022-09-16 16:52:16.890421 keggtools-1.0.1/keggtools/__pycache__/storage.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0        0        0     4368 2022-10-03 18:19:25.362035 keggtools-1.0.1/keggtools/__pycache__/storage.cpython-36.pyc
--rw-r--r--   0        0        0     4303 2022-08-26 11:00:08.192639 keggtools-1.0.1/keggtools/__pycache__/storage.cpython-38.pyc
--rw-r--r--   0        0        0     6885 2021-10-10 18:05:17.268279 keggtools-1.0.1/keggtools/__pycache__/utils.cpython-36-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     8362 2022-09-16 16:52:16.862426 keggtools-1.0.1/keggtools/__pycache__/utils.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0        0        0     8255 2022-10-03 18:19:25.338035 keggtools-1.0.1/keggtools/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0        0        0     8237 2022-08-26 10:59:58.664882 keggtools-1.0.1/keggtools/__pycache__/utils.cpython-38.pyc
--rwxr-xr-x   0        0        0    10695 2022-10-03 18:19:24.070043 keggtools-1.0.1/keggtools/analysis.py
--rwxr-xr-x   0        0        0    12079 2022-10-03 18:54:54.980790 keggtools-1.0.1/keggtools/const.py
--rwxr-xr-x   0        0        0    31426 2022-10-03 18:19:24.230042 keggtools-1.0.1/keggtools/models.py
--rwxr-xr-x   0        0        0    22448 2022-10-03 18:19:24.126042 keggtools-1.0.1/keggtools/render.py
--rwxr-xr-x   0        0        0     9152 2022-10-03 18:19:24.050043 keggtools-1.0.1/keggtools/resolver.py
--rwxr-xr-x   0        0        0     4513 2022-10-03 18:19:24.030043 keggtools-1.0.1/keggtools/storage.py
--rwxr-xr-x   0        0        0     8280 2022-10-03 18:19:24.066043 keggtools-1.0.1/keggtools/utils.py
--rw-r--r--   0        0        0     2231 2022-10-03 19:01:20.162384 keggtools-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1505 2022-10-03 19:02:14.782043 keggtools-1.0.1/requirements.txt
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 keggtools-1.0.1/setup.py
--rw-r--r--   0        0        0     3708 1970-01-01 00:00:00.000000 keggtools-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       29 2022-10-22 21:28:18.825522 keggtools-1.0.2/.flake8
+-rw-r--r--   0        0        0     1182 2023-06-05 19:41:37.076895 keggtools-1.0.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2249 2023-06-05 19:41:40.180738 keggtools-1.0.2/.github/workflows/package.yml
+-rw-r--r--   0        0        0     2069 2022-10-03 18:32:22.809225 keggtools-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1622 2022-10-22 21:31:53.888830 keggtools-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1040 2022-11-05 20:00:51.869075 keggtools-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2021-01-20 18:48:18.741520 keggtools-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3984 2022-11-05 23:34:27.236022 keggtools-1.0.2/Makefile
+-rw-r--r--   0        0        0     2396 2023-06-05 19:38:38.141898 keggtools-1.0.2/README.md
+-rwxr-xr-x   0        0        0      920 2023-06-05 19:39:22.563664 keggtools-1.0.2/keggtools/__init__.py
+-rwxr-xr-x   0        0        0    10687 2023-06-05 19:38:38.145897 keggtools-1.0.2/keggtools/analysis.py
+-rwxr-xr-x   0        0        0    12079 2022-10-03 18:54:54.980790 keggtools-1.0.2/keggtools/const.py
+-rwxr-xr-x   0        0        0    31420 2023-06-05 19:38:38.145897 keggtools-1.0.2/keggtools/models.py
+-rwxr-xr-x   0        0        0    22422 2023-06-05 19:38:38.149897 keggtools-1.0.2/keggtools/render.py
+-rwxr-xr-x   0        0        0     9148 2023-06-05 19:38:38.149897 keggtools-1.0.2/keggtools/resolver.py
+-rwxr-xr-x   0        0        0     4513 2022-10-03 18:19:24.030043 keggtools-1.0.2/keggtools/storage.py
+-rwxr-xr-x   0        0        0     8280 2022-10-03 18:19:24.066043 keggtools-1.0.2/keggtools/utils.py
+-rw-r--r--   0        0        0     2159 2023-06-05 19:38:38.149897 keggtools-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2493 2023-06-05 19:38:38.149897 keggtools-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 keggtools-1.0.2/setup.py
+-rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 keggtools-1.0.2/PKG-INFO
```

### Comparing `keggtools-1.0.1/.github/workflows/docs.yml` & `keggtools-1.0.2/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 
 name: Deploy docs
 
 on:
     workflow_dispatch:
     release:
+        types: [published]
         branches:
             - main
 
 
 # Jobs
 jobs:
 
     docs:
         # Run on ubuntu latest
         runs-on: ubuntu-latest
 
 
         steps:
-        -   uses: actions/checkout@v2
+        -   uses: actions/checkout@v3
 
-        -   name: Set up Python 3.6
-            uses: actions/setup-python@v2
+        -   name: Set up Python 3.8
+            uses: actions/setup-python@v4
             with:
-                python-version: "3.6"
+                python-version: "3.8"
 
 
         # Test and build the docs for keggtools
         -   name: test and build docs
             run: |
                 pip install flit Sphinx furo
                 flit install --deps=production
```

### Comparing `keggtools-1.0.1/.github/workflows/package.yml` & `keggtools-1.0.2/.github/workflows/package.yml`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,21 @@
     build:
         # Run on ubuntu latest
         runs-on: ubuntu-latest
 
         # Matrix testing
         strategy:
             matrix:
-                # Check for all python versions >=3.6
-                # python-version: [3.6, 3.7, 3.8, 3.9]
-                python-version: ["3.6"]
+                # Check for all python versions >=3.8
+                python-version: ["3.8", "3.9", "3.10"]
 
         steps:
-        -   uses: actions/checkout@v2
+        -   uses: actions/checkout@v3
         -   name: Set up Python ${{ matrix.python-version }}
-            uses: actions/setup-python@v2
+            uses: actions/setup-python@v4
             with:
                 python-version: ${{ matrix.python-version }}
 
         # Install dependencies from freeze
         -   name: Install dependencies
             run: |
                 sudo apt-get install -y graphviz
```

### Comparing `keggtools-1.0.1/.gitignore` & `keggtools-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `keggtools-1.0.1/.pre-commit-config.yaml` & `keggtools-1.0.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -40,30 +40,31 @@
 
 -   repo: https://github.com/PyCQA/flake8
     rev: "5.0.4"
     hooks:
     -   id: flake8
         name: Run linting with flake8
         files: (.*).py
-        args: [--max-line-length=120]
+        args: [--config=./.flake8]
 
 
 # -   repo: https://github.com/pre-commit/mirrors-mypy
 #     rev: v0.971
 #     hooks:
 #     -   id: mypy
-#         name: Static code analysis of backend
+#         name: Static code analysis
 #         files: ^(keggtools|test|docs)/(.*).py
 #         additional_dependencies: ["types-requests"]
 
+
 # add pytest hook
 -   repo: local
     hooks:
     -   id: pytest
-        name: Run unittest on worker
+        name: Run unittest
         stages: [commit]
         language: system
         entry: pytest
         types: [python]
         pass_filenames: false
         always_run: true
```

### Comparing `keggtools-1.0.1/.vscode/settings.json` & `keggtools-1.0.2/.vscode/settings.json`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {
     "git.ignoreLimitWarning": true,
-    "settings": {
-        "files.exclude": {
-            "**/.DS_Store": true,
-            "**/venv": true,
-            "**/.mypy_cache": true,
-            "**/.pytest_cache": true,
-        }
+    "files.exclude": {
+        "**/.DS_Store": true,
+        "**/venv": true,
+        "**/.mypy_cache": true,
+        "**/.pytest_cache": true,
+        "**/.coverage": true,
+        "**/coverage": true,
     },
     "python.defaultInterpreterPath": "./venv/bin/python",
     "editor.formatOnSave": true,
     "python.formatting.provider": "black",
     "python.formatting.blackPath": "./venv/bin/black",
     "python.linting.flake8Enabled": true,
     "python.linting.flake8Path": "./venv/bin/flake8",
```

### Comparing `keggtools-1.0.1/LICENSE` & `keggtools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keggtools-1.0.1/README.md` & `keggtools-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # keggtools
 Library for KEGG pathway enrichment analysis.
 
 Documentation: [https://keggtools.org/](https://keggtools.org/)
+
 PyPi: [https://pypi.org/project/keggtools/](https://pypi.org/project/keggtools/)
 
 
 ## Installation
 
-`keggtools` only supports `python` version greater than or equal `3.6`.
+`keggtools` only supports `python` version greater than or equal `3.8`.
 
 Dependencies
 
 * `graphviz`
 
 `python` dependencies
 
 * `requests`
 * `pydot`
-* `scipy>=1.5.4`
+* `scipy`
 
 
 Installation `keggtools` package using `pip`:
 
 ```bash
 python3 -m pip install keggtools
 ```
```

### Comparing `keggtools-1.0.1/keggtools/__init__.py` & `keggtools-1.0.2/keggtools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Init keggtools module """
 
 
-__version__: str = "1.0.1"
+__version__: str = "1.0.2"
 
 from .analysis import EnrichmentResult, Enrichment  # noqa: F401
 from .const import (  # noqa: F401
     IMMUNE_SYSTEM_PATHWAYS,
     GLOBAL_AND_OVERVIEW_MAPS,
     CARBOHYDRATE_METABOLISM,
     ENERGY_METABOLISM,
```

### Comparing `keggtools-1.0.1/keggtools/analysis.py` & `keggtools-1.0.2/keggtools/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         org: str,
         pathway_id: str,
         pathway_name: str,
         found_genes: list,
         pathway_genes: list,
         pathway_title: Optional[str] = None,
     ) -> None:
-
         """
         Init Result of KEGG pathway enrichment analysis.
 
         :param str org: 3 letter code of organism used by KEGG database.
         :param str pathway_id: Identifier of KEGG pathway.
         :param str pathway_name: Name of KEGG pathway.
         :param list found_genes: List of found genes.
@@ -187,15 +186,14 @@
         # pylint: disable=too-many-locals
 
         all_found_genes: int = 0
         absolute_pathway_genes: int = 0
         study_n: int = len(gene_list)
 
         for pathway in self.all_pathways:
-
             genes_found: List[str] = []
             all_pathways_genes = pathway.get_genes()
             absolute_pathway_genes += len(all_pathways_genes)
 
             # Check for intersection between gene list and genes in pathway
             for gene_id in all_pathways_genes:
                 if gene_id in gene_list:
@@ -213,18 +211,16 @@
                 pathway_genes=all_pathways_genes,
             )
             self.result.append(pathway_result)
 
         # Perform Fisher exact test
         # http://docs.scipy.org/doc/scipy-0.17.0/reference/generated/scipy.stats.fisher_exact.html
         for analysis in self.result:
-
             # Skip p value calculation if no genes are found
             if analysis.study_count > 0:
-
                 a_var: int = analysis.study_count
                 b_var: int = study_n - analysis.study_count
                 c_var: int = analysis.pathway_genes_count - analysis.study_count
                 d_var: int = (
                     absolute_pathway_genes - analysis.pathway_genes_count - b_var
                 )
```

### Comparing `keggtools-1.0.1/keggtools/const.py` & `keggtools-1.0.2/keggtools/const.py`

 * *Files identical despite different names*

### Comparing `keggtools-1.0.1/keggtools/models.py` & `keggtools-1.0.2/keggtools/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -617,15 +617,14 @@
             id=get_attribute(element=item, key="id"),
             name=get_attribute(element=item, key="name"),
         )
 
         # Parse child alt elements
         for child in item:
             if child.tag == "alt":
-
                 # TODO warn if overwrite
                 # TODO: or raise exception (only 1 alt should be presnet)
                 # if parsed_product.alt is not None:
                 #     warn(message="'Alt'")
 
                 parsed_product.alt = Alt.parse(item=child)
 
@@ -704,15 +703,14 @@
             id=get_attribute(element=item, key="id"),
             name=get_attribute(element=item, key="name"),
         )
 
         # Parse child alt elements
         for child in item:
             if child.tag == "alt":
-
                 # TODO warn if overwrite
                 # TODO: or raise exception (only 1 alt should be presnet)
                 # if parsed_substrate.alt is not None:
                 #     warn(message="'Alt'")
 
                 parsed_substrate.alt = Alt.parse(item=child)
 
@@ -1029,15 +1027,14 @@
 
         result: List[str] = []
 
         # Iterate of entries and get all gene type
         # Keep list of genes unique
         for entry in self.entries:
             if entry.type == "gene":
-
                 # Get name of entry (KEGG identifier)
                 # if " " in entry.name:
                 #     # Check if name contains a space, which indicates list of multiple identifier
                 #     splitted_entries: List[str] = entry.name.split(" ")
                 #     for single_entry in splitted_entries:
                 #         if single_entry not in result:
                 #             result.append(single_entry)
```

### Comparing `keggtools-1.0.1/keggtools/render.py` & `keggtools-1.0.2/keggtools/render.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,21 +84,19 @@
             "cellspacing": "0",
             "cellpadding": "4",
         },
     )
 
     # TODO: implement multiple cols for longer lists (square format)
     for index, (key, value) in enumerate(items.items()):
-
         element_row: Element = SubElement(element_table, "tr", attrib={})
 
         element_col: Element = SubElement(element_row, "td")
 
         if truncate is not None and index >= truncate:
-
             element_col.text = f"{len(items.items()) - truncate} more genes..."
             break
 
         element_col.attrib = {"bgcolor": value}
 
         # Set key as inner text of table cell
         element_col.text = key
@@ -305,24 +303,22 @@
         #     resolved_gene_names = self.resolve_missing_gene_names(truncate_gene_list=truncate_gene_list)
 
         # add all nodes and edges
         related_entries = [int(p.entry1) for p in self.pathway.relations]
         related_entries.extend([int(p.entry2) for p in self.pathway.relations])
 
         for entry in self.pathway.entries:
-
             # Use entry id as default label
             # TODO: use different default label as fallback
             entry_label: str = entry.id
 
             # only render genes with at least 1 relation
             if int(entry.id) in related_entries:
                 # case select for types gene, comp, group, ...
                 if entry.type == "gene":
-
                     # Get entry name by graphics element name attribute
                     if entry.graphics is not None and entry.graphics.name is not None:
                         entry_label = entry.graphics.name.split(", ")[0]
 
                     # Check if entry name contains multiple gene entries
                     # TODO: request the names of the entry names with .../find/gene1+gene2 ->
                     # parse list and use names as labels
@@ -358,15 +354,14 @@
                                 style="filled",
                                 color="#000000",
                                 fillcolor="#ffffff",
                             )
                         )
 
                     else:
-
                         # Single node
                         self.graph.add_node(
                             Node(
                                 name=entry.id,
                                 label=entry_label,
                                 shape="rectangle",
                                 style="filled",
@@ -374,30 +369,27 @@
                                 fillcolor=self.get_gene_color(
                                     gene_id=entry.get_gene_id()[0]
                                 ),
                             )
                         )
 
                 elif entry.type == "group":
-
                     component_label: List[Tuple[str, str]] = []
 
                     # Iterate of components of group entry
                     for comp in entry.components:
-
                         component_entry: Optional[Entry] = self.pathway.get_entry_by_id(
                             comp.id
                         )
 
                         if (
                             component_entry is not None
                             and component_entry.graphics is not None
                             and component_entry.graphics.name is not None
                         ):
-
                             # Append tuple of gene id and color to labels
                             component_label.append(
                                 (
                                     component_entry.graphics.name.split(", ")[0],
                                     self.get_gene_color(
                                         component_entry.get_gene_id()[0]
                                     ),
@@ -421,15 +413,14 @@
                             style="filled",
                             color="#000000",
                             fillcolor="#ffffff",
                         )
                     )
 
                 elif entry.type == "compound":
-
                     # TODO: resolver compound with resolver
 
                     if entry.graphics is not None and entry.graphics.name is not None:
                         entry_label = entry.graphics.name.split(", ")[0]
 
                     # Add compound node to graph
                     self.graph.add_node(
@@ -440,15 +431,14 @@
                             style="filled",
                             color="#000000",
                             fillcolor="#ffffff",
                         )
                     )
 
                 elif entry.type == "reaction":
-
                     # TODO: implement reaction rendering
 
                     pass
 
                 # TODO: add pathway map to dot graph
                 # elif entry.type == "map":
 
@@ -462,15 +452,14 @@
                 #         shape="rectangle",
                 #         style="rounded,filled",
                 #         color="#000000",
                 #         fillcolor="#ffffff",
                 #     ))
 
         for rel in self.pathway.relations:
-
             # Create edge instance from relation enties
             relation_edge: Edge = Edge(
                 src=rel.entry1,
                 dst=rel.entry2,
             )
 
             # default line style
@@ -497,18 +486,16 @@
             # Iterate over relation subtypes and check if moleuclar event is present
             edge_label: Optional[str] = None
 
             # Default arrowhead
             arrowhead: str = "none"
 
             for subtype in rel.subtypes:
-
                 # Check if subtype is molecular event to set label of edge
                 if subtype.name in molecular_event_dict:
-
                     # Check if label is none (no subtype found in prior iter steps)
                     if edge_label is None:
                         edge_label = molecular_event_dict[subtype.name]
                     else:
                         # TODO: is this event even possible ?
                         # TODO: handle but call warning
                         # A molecular event was already found. Append label to existing label
```

### Comparing `keggtools-1.0.1/keggtools/resolver.py` & `keggtools-1.0.2/keggtools/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,20 +142,18 @@
         :return: Returns content of file as string.
         :rtype: str
         """
 
         file_data: Optional[str] = None
 
         if self.storage.exist(filename=filename):
-
             # return pathway list dump
             file_data = self.storage.load(filename=filename)
 
         else:
-
             # Data not found in cache. Request from REST api
 
             file_data = _request(url=url, **kwargs)
 
             # Save in storage
             self.storage.save(filename=filename, data=file_data)
```

### Comparing `keggtools-1.0.1/keggtools/storage.py` & `keggtools-1.0.2/keggtools/storage.py`

 * *Files identical despite different names*

### Comparing `keggtools-1.0.1/keggtools/utils.py` & `keggtools-1.0.2/keggtools/utils.py`

 * *Files identical despite different names*

### Comparing `keggtools-1.0.1/pyproject.toml` & `keggtools-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,40 +5,39 @@
 build-backend = "flit_core.buildapi"
 
 
 # Project details
 [project]
 name = "keggtools"
 description = "Enrichment analysis and visualisation toolkit for KEGG pathways"
-requires-python = '>=3.6'
+requires-python = '>=3.8'
 license = {file = "LICENSE"}
 
 authors = [
     {name="harryhaller001", email = "harryhaller001@gmail.com"}
 ]
 
 maintainers = [
     {name="harryhaller001", email = "harryhaller001@gmail.com"}
 ]
 
 readme = {file = "README.md", content-type="text/markdown"}
 
 classifiers=[
     "Development Status :: 3 - Alpha",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "pydot >= 1.4.2",
-    "requests >= 2.27.1",
-    "scipy >= 1.5.4",
+    "pydot",
+    "requests",
+    "scipy",
 ]
 
 dynamic = ["version"]
 
 
 # Project urls
 [project.urls]
@@ -64,15 +63,15 @@
     "furo",
 ]
 
 
 # Mypy config
 # https://mypy.readthedocs.io/en/stable/config_file.html#using-a-pyproject-toml-file
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 warn_return_any = true
 warn_unused_configs = true
 
 
 # Ignore libs which are not PEP 561 compliant
 [[tool.mypy.overrides]]
 module = [
```

### Comparing `keggtools-1.0.1/setup.py` & `keggtools-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 packages = \
 ['keggtools']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pydot >= 1.4.2', 'requests >= 2.27.1', 'scipy >= 1.5.4']
+['pydot', 'requests', 'scipy']
 
 extras_require = \
 {'doc': ['Sphinx', 'furo'],
  'test': ['flake8',
           'black',
           'pytest',
           'coverage',
           'mypy',
           'types-requests',
           'responses',
           'pandas']}
 
 setup(name='keggtools',
-      version='1.0.1',
+      version='1.0.2',
       description='Enrichment analysis and visualisation toolkit for KEGG pathways',
       author=None,
       author_email='harryhaller001 <harryhaller001@gmail.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
       extras_require=extras_require,
-      python_requires='>=3.6',
+      python_requires='>=3.8',
      )
```

### Comparing `keggtools-1.0.1/PKG-INFO` & `keggtools-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: keggtools
-Version: 1.0.1
+Version: 1.0.2
 Summary: Enrichment analysis and visualisation toolkit for KEGG pathways
 Author-email: harryhaller001 <harryhaller001@gmail.com>
 Maintainer-email: harryhaller001 <harryhaller001@gmail.com>
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Dist: pydot >= 1.4.2
-Requires-Dist: requests >= 2.27.1
-Requires-Dist: scipy >= 1.5.4
+Requires-Dist: pydot
+Requires-Dist: requests
+Requires-Dist: scipy
 Requires-Dist: Sphinx ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: coverage ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
@@ -31,30 +30,31 @@
 Provides-Extra: doc
 Provides-Extra: test
 
 # keggtools
 Library for KEGG pathway enrichment analysis.
 
 Documentation: [https://keggtools.org/](https://keggtools.org/)
+
 PyPi: [https://pypi.org/project/keggtools/](https://pypi.org/project/keggtools/)
 
 
 ## Installation
 
-`keggtools` only supports `python` version greater than or equal `3.6`.
+`keggtools` only supports `python` version greater than or equal `3.8`.
 
 Dependencies
 
 * `graphviz`
 
 `python` dependencies
 
 * `requests`
 * `pydot`
-* `scipy>=1.5.4`
+* `scipy`
 
 
 Installation `keggtools` package using `pip`:
 
 ```bash
 python3 -m pip install keggtools
 ```
```

