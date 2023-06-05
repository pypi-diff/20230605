# Comparing `tmp/enforce_notebook_run_order-1.0.0.tar.gz` & `tmp/enforce_notebook_run_order-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enforce_notebook_run_order-1.0.0.tar", max compression
+gzip compressed data, was "enforce_notebook_run_order-1.1.0.tar", max compression
```

## Comparing `enforce_notebook_run_order-1.0.0.tar` & `enforce_notebook_run_order-1.1.0.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     2925 2023-06-05 16:13:13.701301 enforce_notebook_run_order-1.0.0/README.md
--rw-r--r--   0        0        0      821 2023-06-05 16:13:13.701301 enforce_notebook_run_order-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4422 2023-06-05 16:13:13.701301 enforce_notebook_run_order-1.0.0/src/enforce_notebook_run_order.py
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3160 2023-06-05 19:36:42.036154 enforce_notebook_run_order-1.1.0/README.md
+-rw-r--r--   0        0        0      865 2023-06-05 19:36:42.036154 enforce_notebook_run_order-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5578 2023-06-05 19:36:42.036154 enforce_notebook_run_order-1.1.0/src/enforce_notebook_run_order.py
+-rw-r--r--   0        0        0     3445 2023-06-05 19:36:42.036154 enforce_notebook_run_order-1.1.0/src/temp_notebook.py
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 enforce_notebook_run_order-1.1.0/PKG-INFO
```

### Comparing `enforce_notebook_run_order-1.0.0/README.md` & `enforce_notebook_run_order-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -50,23 +50,29 @@
 
 ### Standalone
 
 To use `enforce-notebook-run-order` as a standalone script, simply run
 it with the path to the notebook(s) you want to check:
 
 ``` {.sourceCode .bash}
-enforce-notebook-run-order my_notebook.ipynb my_other_notebook.ipynb
+nbcheck my_notebook.ipynb my_other_notebook.ipynb
 ```
 
 Or point it to a directory to check all notebooks in that directory:
 
 ``` {.sourceCode .bash}
-enforce-notebook-run-order my_notebooks/
+nbcheck my_notebooks/
 ```
 
+You can also use the full `enforce-notebook-run-order` command, but the
+`nbcheck` command is provided as a convenience.
+
+For information on the command line interface, please refer to the [CLI
+documentation](module_enforce_notebook_run_order.html#command-line-interface).
+
 ### pre-commit hook
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
 ``` {.sourceCode .yaml}
 repos:
```

#### html2text {}

```diff
@@ -10,15 +10,18 @@
 cells are run out of order. Installation ------------ `enforce-notebook-run-
 order` can be installed via pip: ``` {.sourceCode .bash} pip install enforce-
 notebook-run-order ``` It can also be set up as a [pre-commit hook](https://
 pre-commit.com/). See the [pre-commit hook](#pre-commit-hook) section for more
 details. Usage ----- `enforce-notebook-run-order` can be used as a standalone
 script, or as a [pre-commit hook](https://pre-commit.com/). ### Standalone To
 use `enforce-notebook-run-order` as a standalone script, simply run it with the
-path to the notebook(s) you want to check: ``` {.sourceCode .bash} enforce-
-notebook-run-order my_notebook.ipynb my_other_notebook.ipynb ``` Or point it to
-a directory to check all notebooks in that directory: ``` {.sourceCode .bash}
-enforce-notebook-run-order my_notebooks/ ``` ### pre-commit hook To use
-`enforce_notebook_run_order` as a pre-commit hook, add the following to your
-`.pre-commit-config.yaml`: ``` {.sourceCode .yaml} repos: - repo: https://
-github.com/christopher-hacker/enforce_notebook_run_order rev: 1.0.0 hooks: -
-id: enforce-notebook-run-order ```
+path to the notebook(s) you want to check: ``` {.sourceCode .bash} nbcheck
+my_notebook.ipynb my_other_notebook.ipynb ``` Or point it to a directory to
+check all notebooks in that directory: ``` {.sourceCode .bash} nbcheck
+my_notebooks/ ``` You can also use the full `enforce-notebook-run-order`
+command, but the `nbcheck` command is provided as a convenience. For
+information on the command line interface, please refer to the [CLI
+documentation](module_enforce_notebook_run_order.html#command-line-interface).
+### pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook,
+add the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml}
+repos: - repo: https://github.com/christopher-hacker/enforce_notebook_run_order
+rev: 1.0.0 hooks: - id: enforce-notebook-run-order ```
```

### Comparing `enforce_notebook_run_order-1.0.0/pyproject.toml` & `enforce_notebook_run_order-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enforce-notebook-run-order"
-version = "1.0.0"
+version = "1.1.0"
 description = ""
 authors = ["Chris Hacker <49451910+christopher-hacker@users.noreply.github.com>"]
 license = "MIT"
 urls = { homepage = "https://github.com/christopher-hacker/enforce-notebook-run-order" }
 readme = "README.md"
 packages = [
     { include = "*", from = "src" },
@@ -27,8 +27,9 @@
 pre-commit = "^3.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-enforce-notebook-run-order = "enforce_notebook_run_order:cli"
+enforce-notebook-run-order = "enforce_notebook_run_order:cli"
+nbcheck = "enforce_notebook_run_order:cli"
```

### Comparing `enforce_notebook_run_order-1.0.0/src/enforce_notebook_run_order.py` & `enforce_notebook_run_order-1.1.0/src/enforce_notebook_run_order.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """forces notebooks to run cells sequentially and fails if cells were run out of order"""
 
 import json
 import os
 import pathlib
 from typing import List
+import warnings
 import click
+import temp_notebook
 
 
 class NotebookCodeCellNotRunError(Exception):
     """raised when a notebook code cell was not run"""
 
 
 class NotebookRunOrderError(Exception):
@@ -64,59 +66,85 @@
                     f"The cell that caused this error is #{current_cell_number} "
                     f"and the previous cell was #{previous_cell_number}. \n\n"
                     f"Cell contents: \n\n> {cell}"
                 )
             previous_cell_number = current_cell_number
 
 
-def check_single_notebook(path: str):
+def check_single_notebook(notebook_path: str, no_run: bool = False):
     """Check a single notebook."""
-    notebook_path = pathlib.Path(path)
+    notebook_path = pathlib.Path(notebook_path)
     with open(notebook_path, "r", encoding="UTF-8") as notebook_file:
         notebook_data = json.load(notebook_file)
     try:
         check_notebook_run_order(notebook_data)
-    except (NotebookCodeCellNotRunError, NotebookRunOrderError) as error:
+        if not no_run:
+            with temp_notebook.TempNotebook(notebook_data) as temp_nb:
+                temp_nb.check_notebook()
+    except (
+        NotebookCodeCellNotRunError,
+        NotebookRunOrderError,
+        temp_notebook.InvalidNotebookJsonError,
+        temp_notebook.CellOutputMismatchError,
+    ) as error:
         raise InvalidNotebookRunError(
-            f"Notebook {notebook_path} was not run in order.\n\n"
-            # append the error message from the check_notebook_run_order function
-            f"{error}\n\n"
+            f"Notebook {notebook_path} was not run in order.\n\n{error}\n\n"
         ) from error
+    print(f"Notebook {notebook_path} was run correctly.")
 
 
-def process_path(path: str):
+def process_path(path: str, no_run: bool = False):
     """Processes a single path. Raises an exception if the path is invalid."""
     if os.path.isdir(path):
         # Get all .ipynb files in the directory and its subdirectories
         for dirpath, _, filenames in os.walk(path):
             for filename in filenames:
                 notebok_path = pathlib.Path(dirpath) / filename
                 if filename.endswith(".ipynb") and not notebook_is_in_virtualenv(
                     notebok_path
                 ):
-                    check_single_notebook(os.path.join(dirpath, filename))
+                    check_single_notebook(
+                        os.path.join(dirpath, filename),
+                        no_run=no_run,
+                    )
     elif path.endswith(".ipynb"):
         check_single_notebook(path)
     else:
         raise ValueError(
             f"Cannot check file {path}. "
             "Must be a path to a notebook file with the .ipynb extension, or a directory."
         )
 
 
 @click.command()
 @click.argument("paths", nargs=-1, type=click.Path(exists=True), required=False)
-def cli(paths: List[str] = None):
+@click.option(
+    "--no-run",
+    is_flag=True,
+    help="Do not run the notebooks, only check the run order. "
+    "This may miss some errors, but is useful for extremely long running notebooks. "
+    "If you use this option, you should consider moving the long-running code to a "
+    "separate task that runs separately from the notebook.",
+)
+def cli(paths: List[str] = None, no_run: bool = False):
     """
     Checks the run order of notebooks in the specified paths,
     or the entire repo if no paths are specified
     """
+    if no_run:
+        warnings.warn(
+            "The --no-run option will not catch all problems with notebooks. "
+            "It is possible that the checks will pass, but the notebook was still run "
+            "out of order. It is highly recommended to move any long-running code to a separate "
+            "task that runs separately from the notebook."
+        )
+
     if paths:
         for path in paths:
-            process_path(path)
+            process_path(path, no_run)
     else:
         # If no paths are provided, check the current directory
-        process_path(".")
+        process_path(".", no_run)
 
 
 if __name__ == "__main__":  # pragma: no cover
     cli()
```

### Comparing `enforce_notebook_run_order-1.0.0/PKG-INFO` & `enforce_notebook_run_order-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enforce-notebook-run-order
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 License: MIT
 Author: Chris Hacker
 Author-email: 49451910+christopher-hacker@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -69,23 +69,29 @@
 
 ### Standalone
 
 To use `enforce-notebook-run-order` as a standalone script, simply run
 it with the path to the notebook(s) you want to check:
 
 ``` {.sourceCode .bash}
-enforce-notebook-run-order my_notebook.ipynb my_other_notebook.ipynb
+nbcheck my_notebook.ipynb my_other_notebook.ipynb
 ```
 
 Or point it to a directory to check all notebooks in that directory:
 
 ``` {.sourceCode .bash}
-enforce-notebook-run-order my_notebooks/
+nbcheck my_notebooks/
 ```
 
+You can also use the full `enforce-notebook-run-order` command, but the
+`nbcheck` command is provided as a convenience.
+
+For information on the command line interface, please refer to the [CLI
+documentation](module_enforce_notebook_run_order.html#command-line-interface).
+
 ### pre-commit hook
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
 ``` {.sourceCode .yaml}
 repos:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 1.1.0 Summary:
 License: MIT Author: Chris Hacker Author-email: 49451910+christopher-
 hacker@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.1.3,<9.0.0) Requires-Dist: jupyter (>=1.0.0,<2.0.0) Project-URL: homepage,
@@ -20,15 +20,18 @@
 cells are run out of order. Installation ------------ `enforce-notebook-run-
 order` can be installed via pip: ``` {.sourceCode .bash} pip install enforce-
 notebook-run-order ``` It can also be set up as a [pre-commit hook](https://
 pre-commit.com/). See the [pre-commit hook](#pre-commit-hook) section for more
 details. Usage ----- `enforce-notebook-run-order` can be used as a standalone
 script, or as a [pre-commit hook](https://pre-commit.com/). ### Standalone To
 use `enforce-notebook-run-order` as a standalone script, simply run it with the
-path to the notebook(s) you want to check: ``` {.sourceCode .bash} enforce-
-notebook-run-order my_notebook.ipynb my_other_notebook.ipynb ``` Or point it to
-a directory to check all notebooks in that directory: ``` {.sourceCode .bash}
-enforce-notebook-run-order my_notebooks/ ``` ### pre-commit hook To use
-`enforce_notebook_run_order` as a pre-commit hook, add the following to your
-`.pre-commit-config.yaml`: ``` {.sourceCode .yaml} repos: - repo: https://
-github.com/christopher-hacker/enforce_notebook_run_order rev: 1.0.0 hooks: -
-id: enforce-notebook-run-order ```
+path to the notebook(s) you want to check: ``` {.sourceCode .bash} nbcheck
+my_notebook.ipynb my_other_notebook.ipynb ``` Or point it to a directory to
+check all notebooks in that directory: ``` {.sourceCode .bash} nbcheck
+my_notebooks/ ``` You can also use the full `enforce-notebook-run-order`
+command, but the `nbcheck` command is provided as a convenience. For
+information on the command line interface, please refer to the [CLI
+documentation](module_enforce_notebook_run_order.html#command-line-interface).
+### pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook,
+add the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml}
+repos: - repo: https://github.com/christopher-hacker/enforce_notebook_run_order
+rev: 1.0.0 hooks: - id: enforce-notebook-run-order ```
```

