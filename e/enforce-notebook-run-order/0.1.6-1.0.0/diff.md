# Comparing `tmp/enforce_notebook_run_order-0.1.6.tar.gz` & `tmp/enforce_notebook_run_order-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enforce_notebook_run_order-0.1.6.tar", max compression
+gzip compressed data, was "enforce_notebook_run_order-1.0.0.tar", max compression
```

## Comparing `enforce_notebook_run_order-0.1.6.tar` & `enforce_notebook_run_order-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2995 2023-06-02 20:22:30.852474 enforce_notebook_run_order-0.1.6/README.md
--rw-r--r--   0        0        0      821 2023-06-02 20:22:30.856474 enforce_notebook_run_order-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5033 2023-06-02 20:22:30.856474 enforce_notebook_run_order-0.1.6/src/enforce_notebook_run_order.py
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 enforce_notebook_run_order-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2925 2023-06-05 16:13:13.701301 enforce_notebook_run_order-1.0.0/README.md
+-rw-r--r--   0        0        0      821 2023-06-05 16:13:13.701301 enforce_notebook_run_order-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4422 2023-06-05 16:13:13.701301 enforce_notebook_run_order-1.0.0/src/enforce_notebook_run_order.py
+-rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.0.0/PKG-INFO
```

### Comparing `enforce_notebook_run_order-0.1.6/README.md` & `enforce_notebook_run_order-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,44 +36,42 @@
 `enforce-notebook-run-order` can be installed via pip:
 
 ``` {.sourceCode .bash}
 pip install enforce-notebook-run-order
 ```
 
 It can also be set up as a [pre-commit hook](https://pre-commit.com/).
-See the [Pre-commit hook](#pre-commit-hook) section for more details.
+See the [pre-commit hook](#pre-commit-hook) section for more details.
 
 Usage
 -----
 
 `enforce-notebook-run-order` can be used as a standalone script, or as a
 [pre-commit hook](https://pre-commit.com/).
 
 ### Standalone
 
 To use `enforce-notebook-run-order` as a standalone script, simply run
-it with the path to the notebook you want to check:
+it with the path to the notebook(s) you want to check:
 
 ``` {.sourceCode .bash}
-enforce-notebook-run-order my_notebook.ipynb
+enforce-notebook-run-order my_notebook.ipynb my_other_notebook.ipynb
 ```
 
 Or point it to a directory to check all notebooks in that directory:
 
 ``` {.sourceCode .bash}
 enforce-notebook-run-order my_notebooks/
 ```
 
-### Pre-commit hook
+### pre-commit hook
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
 ``` {.sourceCode .yaml}
-- repo: https://github.com/christopher-hacker/enforce-notebook-run-order
-    rev: 0.1.5
+repos:
+-   repo: https://github.com/christopher-hacker/enforce_notebook_run_order
+    rev: 1.0.0
     hooks:
-    - id: enforce-notebook-run-order
-        name: enforce-notebook-run-order
-        entry: enforce-notebook-run-order
-        types: [jupyter]
+    -   id: enforce-notebook-run-order
 ```
```

#### html2text {}

```diff
@@ -6,20 +6,19 @@
 can lead to notebooks being committed to the repository in a state where they
 don\'t run from top to bottom, and other collaborators may receive different
 results when running the notebook from top to bottom. `enforce-notebook-run-
 order` enforces the run order of a notebook by raising an exception if any
 cells are run out of order. Installation ------------ `enforce-notebook-run-
 order` can be installed via pip: ``` {.sourceCode .bash} pip install enforce-
 notebook-run-order ``` It can also be set up as a [pre-commit hook](https://
-pre-commit.com/). See the [Pre-commit hook](#pre-commit-hook) section for more
+pre-commit.com/). See the [pre-commit hook](#pre-commit-hook) section for more
 details. Usage ----- `enforce-notebook-run-order` can be used as a standalone
 script, or as a [pre-commit hook](https://pre-commit.com/). ### Standalone To
 use `enforce-notebook-run-order` as a standalone script, simply run it with the
-path to the notebook you want to check: ``` {.sourceCode .bash} enforce-
-notebook-run-order my_notebook.ipynb ``` Or point it to a directory to check
-all notebooks in that directory: ``` {.sourceCode .bash} enforce-notebook-run-
-order my_notebooks/ ``` ### Pre-commit hook To use `enforce_notebook_run_order`
-as a pre-commit hook, add the following to your `.pre-commit-config.yaml`: ```
-{.sourceCode .yaml} - repo: https://github.com/christopher-hacker/enforce-
-notebook-run-order rev: 0.1.5 hooks: - id: enforce-notebook-run-order name:
-enforce-notebook-run-order entry: enforce-notebook-run-order types: [jupyter]
-```
+path to the notebook(s) you want to check: ``` {.sourceCode .bash} enforce-
+notebook-run-order my_notebook.ipynb my_other_notebook.ipynb ``` Or point it to
+a directory to check all notebooks in that directory: ``` {.sourceCode .bash}
+enforce-notebook-run-order my_notebooks/ ``` ### pre-commit hook To use
+`enforce_notebook_run_order` as a pre-commit hook, add the following to your
+`.pre-commit-config.yaml`: ``` {.sourceCode .yaml} repos: - repo: https://
+github.com/christopher-hacker/enforce_notebook_run_order rev: 1.0.0 hooks: -
+id: enforce-notebook-run-order ```
```

### Comparing `enforce_notebook_run_order-0.1.6/pyproject.toml` & `enforce_notebook_run_order-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enforce-notebook-run-order"
-version = "0.1.6"
+version = "1.0.0"
 description = ""
 authors = ["Chris Hacker <49451910+christopher-hacker@users.noreply.github.com>"]
 license = "MIT"
 urls = { homepage = "https://github.com/christopher-hacker/enforce-notebook-run-order" }
 readme = "README.md"
 packages = [
     { include = "*", from = "src" },
```

### Comparing `enforce_notebook_run_order-0.1.6/src/enforce_notebook_run_order.py` & `enforce_notebook_run_order-1.0.0/src/enforce_notebook_run_order.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """forces notebooks to run cells sequentially and fails if cells were run out of order"""
 
 import json
 import os
 import pathlib
+from typing import List
 import click
 
 
 class NotebookCodeCellNotRunError(Exception):
     """raised when a notebook code cell was not run"""
 
 
@@ -14,14 +15,33 @@
     """raised when a notebook is run out of order"""
 
 
 class InvalidNotebookRunError(Exception):
     """raised when any problems were identified with a notebook's run order"""
 
 
+def notebook_is_in_virtualenv(notebook_path: pathlib.Path) -> bool:
+    """
+    Checks whether a notebook is in the current repo or is in the virtual environment's
+    site-packages directory.
+
+    Some dependencies may contain Jupyter notebooks in their site-packages directory for
+    testing or documentation purposes. These notebooks should not be checked for run order.
+
+    Args:
+        notebook_path (pathlib.Path): Path to the notebook file.
+
+    Returns:
+        bool: True if the notebook is in the virtual environment's site-packages directory.
+    """
+    # if the notebook_path contains "site-packages", it is in the virtual environment
+    # and should not be checked
+    return "site-packages" in str(notebook_path)
+
+
 def check_notebook_run_order(notebook_data: dict) -> None:
     """
     Checks that the notebook cells were run sequentially and fails if not.
 
     Args:
         notebook_data (dict): Notebook data in dictionary format.
 
@@ -44,90 +64,59 @@
                     f"The cell that caused this error is #{current_cell_number} "
                     f"and the previous cell was #{previous_cell_number}. \n\n"
                     f"Cell contents: \n\n> {cell}"
                 )
             previous_cell_number = current_cell_number
 
 
-def notebook_is_in_virtualenv(notebook_path: pathlib.Path) -> bool:
-    """
-    Checks whether a notebook is in the current repo or is in the virtual environment's
-    site-packages directory.
+def check_single_notebook(path: str):
+    """Check a single notebook."""
+    notebook_path = pathlib.Path(path)
+    with open(notebook_path, "r", encoding="UTF-8") as notebook_file:
+        notebook_data = json.load(notebook_file)
+    try:
+        check_notebook_run_order(notebook_data)
+    except (NotebookCodeCellNotRunError, NotebookRunOrderError) as error:
+        raise InvalidNotebookRunError(
+            f"Notebook {notebook_path} was not run in order.\n\n"
+            # append the error message from the check_notebook_run_order function
+            f"{error}\n\n"
+        ) from error
 
-    Some dependencies may contain Jupyter notebooks in their site-packages directory for
-    testing or documentation purposes. These notebooks should not be checked for run order.
-
-    Args:
-        notebook_path (pathlib.Path): Path to the notebook file.
 
-    Returns:
-        bool: True if the notebook is in the virtual environment's site-packages directory.
-    """
-    # if the notebook_path contains "site-packages", it is in the virtual environment
-    # and should not be checked
-    return "site-packages" in str(notebook_path)
+def process_path(path: str):
+    """Processes a single path. Raises an exception if the path is invalid."""
+    if os.path.isdir(path):
+        # Get all .ipynb files in the directory and its subdirectories
+        for dirpath, _, filenames in os.walk(path):
+            for filename in filenames:
+                notebok_path = pathlib.Path(dirpath) / filename
+                if filename.endswith(".ipynb") and not notebook_is_in_virtualenv(
+                    notebok_path
+                ):
+                    check_single_notebook(os.path.join(dirpath, filename))
+    elif path.endswith(".ipynb"):
+        check_single_notebook(path)
+    else:
+        raise ValueError(
+            f"Cannot check file {path}. "
+            "Must be a path to a notebook file with the .ipynb extension, or a directory."
+        )
 
 
-def check_all_repo_notebooks(notebook_dir=".") -> None:
+@click.command()
+@click.argument("paths", nargs=-1, type=click.Path(exists=True), required=False)
+def cli(paths: List[str] = None):
     """
-    Recursively searches for all Jupyter notebooks in the specified directory
-    and checks their run order.
-
-    Args:
-        notebook_dir (str, optional): Directory to recursively search for notebooks.
-            Defaults to ".".
-
-    Raises:
-        InvalidNotebookRunError: If a notebook was run out of order.
+    Checks the run order of notebooks in the specified paths,
+    or the entire repo if no paths are specified
     """
-    for root, _, files in os.walk(notebook_dir):
-        for file in files:
-            if file.endswith(".ipynb"):
-                if notebook_is_in_virtualenv(pathlib.Path(root) / file):
-                    continue
-                notebook_path = pathlib.Path(root) / file
-                print(notebook_path)
-                with open(notebook_path, "r", encoding="UTF-8") as notebook_file:
-                    notebook_data = json.load(notebook_file)
-                try:
-                    check_notebook_run_order(notebook_data)
-                except (NotebookCodeCellNotRunError, NotebookRunOrderError) as error:
-                    raise InvalidNotebookRunError(
-                        f"Notebook {notebook_path} was not run in order.\n\n"
-                        # append the error message from the check_notebook_run_order function
-                        f"{error}\n\n"
-                    ) from error
-
-
-@click.command()
-@click.option(
-    "--path",
-    "-p",
-    default=".",
-    help="Path to a directory containing notebooks, or a single notebook. "
-    "If not specified, will search the entire repo",
-)
-def cli(path="."):
-    """Checks the run order of notebooks in the specified directory"""
-    if os.path.isdir(path):
-        check_all_repo_notebooks(path)
+    if paths:
+        for path in paths:
+            process_path(path)
     else:
-        if not path.endswith(".ipynb"):
-            raise ValueError(
-                f"Invalid value passed to --path: {path}. "
-                "Must be a path to a notebook file with the .ipynb extension, or a directory."
-            )
-        notebook_path = pathlib.Path(path)
-        with open(notebook_path, "r", encoding="UTF-8") as notebook_file:
-            notebook_data = json.load(notebook_file)
-        try:
-            check_notebook_run_order(notebook_data)
-        except (NotebookCodeCellNotRunError, NotebookRunOrderError) as error:
-            raise InvalidNotebookRunError(
-                f"Notebook {notebook_path} was not run in order.\n\n"
-                # append the error message from the check_notebook_run_order function
-                f"{error}\n\n"
-            ) from error
+        # If no paths are provided, check the current directory
+        process_path(".")
 
 
 if __name__ == "__main__":  # pragma: no cover
     cli()
```

### Comparing `enforce_notebook_run_order-0.1.6/PKG-INFO` & `enforce_notebook_run_order-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enforce-notebook-run-order
-Version: 0.1.6
+Version: 1.0.0
 Summary: 
 License: MIT
 Author: Chris Hacker
 Author-email: 49451910+christopher-hacker@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -55,45 +55,43 @@
 `enforce-notebook-run-order` can be installed via pip:
 
 ``` {.sourceCode .bash}
 pip install enforce-notebook-run-order
 ```
 
 It can also be set up as a [pre-commit hook](https://pre-commit.com/).
-See the [Pre-commit hook](#pre-commit-hook) section for more details.
+See the [pre-commit hook](#pre-commit-hook) section for more details.
 
 Usage
 -----
 
 `enforce-notebook-run-order` can be used as a standalone script, or as a
 [pre-commit hook](https://pre-commit.com/).
 
 ### Standalone
 
 To use `enforce-notebook-run-order` as a standalone script, simply run
-it with the path to the notebook you want to check:
+it with the path to the notebook(s) you want to check:
 
 ``` {.sourceCode .bash}
-enforce-notebook-run-order my_notebook.ipynb
+enforce-notebook-run-order my_notebook.ipynb my_other_notebook.ipynb
 ```
 
 Or point it to a directory to check all notebooks in that directory:
 
 ``` {.sourceCode .bash}
 enforce-notebook-run-order my_notebooks/
 ```
 
-### Pre-commit hook
+### pre-commit hook
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
 ``` {.sourceCode .yaml}
-- repo: https://github.com/christopher-hacker/enforce-notebook-run-order
-    rev: 0.1.5
+repos:
+-   repo: https://github.com/christopher-hacker/enforce_notebook_run_order
+    rev: 1.0.0
     hooks:
-    - id: enforce-notebook-run-order
-        name: enforce-notebook-run-order
-        entry: enforce-notebook-run-order
-        types: [jupyter]
+    -   id: enforce-notebook-run-order
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.0.0 Summary:
 License: MIT Author: Chris Hacker Author-email: 49451910+christopher-
 hacker@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.1.3,<9.0.0) Requires-Dist: jupyter (>=1.0.0,<2.0.0) Project-URL: homepage,
@@ -16,20 +16,19 @@
 can lead to notebooks being committed to the repository in a state where they
 don\'t run from top to bottom, and other collaborators may receive different
 results when running the notebook from top to bottom. `enforce-notebook-run-
 order` enforces the run order of a notebook by raising an exception if any
 cells are run out of order. Installation ------------ `enforce-notebook-run-
 order` can be installed via pip: ``` {.sourceCode .bash} pip install enforce-
 notebook-run-order ``` It can also be set up as a [pre-commit hook](https://
-pre-commit.com/). See the [Pre-commit hook](#pre-commit-hook) section for more
+pre-commit.com/). See the [pre-commit hook](#pre-commit-hook) section for more
 details. Usage ----- `enforce-notebook-run-order` can be used as a standalone
 script, or as a [pre-commit hook](https://pre-commit.com/). ### Standalone To
 use `enforce-notebook-run-order` as a standalone script, simply run it with the
-path to the notebook you want to check: ``` {.sourceCode .bash} enforce-
-notebook-run-order my_notebook.ipynb ``` Or point it to a directory to check
-all notebooks in that directory: ``` {.sourceCode .bash} enforce-notebook-run-
-order my_notebooks/ ``` ### Pre-commit hook To use `enforce_notebook_run_order`
-as a pre-commit hook, add the following to your `.pre-commit-config.yaml`: ```
-{.sourceCode .yaml} - repo: https://github.com/christopher-hacker/enforce-
-notebook-run-order rev: 0.1.5 hooks: - id: enforce-notebook-run-order name:
-enforce-notebook-run-order entry: enforce-notebook-run-order types: [jupyter]
-```
+path to the notebook(s) you want to check: ``` {.sourceCode .bash} enforce-
+notebook-run-order my_notebook.ipynb my_other_notebook.ipynb ``` Or point it to
+a directory to check all notebooks in that directory: ``` {.sourceCode .bash}
+enforce-notebook-run-order my_notebooks/ ``` ### pre-commit hook To use
+`enforce_notebook_run_order` as a pre-commit hook, add the following to your
+`.pre-commit-config.yaml`: ``` {.sourceCode .yaml} repos: - repo: https://
+github.com/christopher-hacker/enforce_notebook_run_order rev: 1.0.0 hooks: -
+id: enforce-notebook-run-order ```
```

