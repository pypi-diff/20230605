# Comparing `tmp/check-type-hints-0.0.3.tar.gz` & `tmp/check-type-hints-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check-type-hints-0.0.3.tar", last modified: Tue May 30 10:01:01 2023, max compression
+gzip compressed data, was "check-type-hints-0.0.4.tar", last modified: Mon Jun  5 10:37:26 2023, max compression
```

## Comparing `check-type-hints-0.0.3.tar` & `check-type-hints-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 10:01:01.197996 check-type-hints-0.0.3/
--rw-rw-rw-   0        0        0      122 2023-05-30 10:01:01.197996 check-type-hints-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 09:57:01.000000 check-type-hints-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 10:01:01.187878 check-type-hints-0.0.3/check_type_hints/
--rw-rw-rw-   0        0        0        0 2023-05-30 09:57:29.000000 check-type-hints-0.0.3/check_type_hints/__init__.py
--rw-rw-rw-   0        0        0     2950 2023-05-30 09:57:01.000000 check-type-hints-0.0.3/check_type_hints/main.py
-drwxrwxrwx   0        0        0        0 2023-05-30 10:01:01.195967 check-type-hints-0.0.3/check_type_hints.egg-info/
--rw-rw-rw-   0        0        0      122 2023-05-30 10:01:01.000000 check-type-hints-0.0.3/check_type_hints.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-05-30 10:01:01.000000 check-type-hints-0.0.3/check_type_hints.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 10:01:01.000000 check-type-hints-0.0.3/check_type_hints.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-30 10:01:01.000000 check-type-hints-0.0.3/check_type_hints.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 10:01:01.000000 check-type-hints-0.0.3/check_type_hints.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-30 10:01:01.000000 check-type-hints-0.0.3/check_type_hints.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 10:01:01.197996 check-type-hints-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-05-30 10:00:42.000000 check-type-hints-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:37:26.405667 check-type-hints-0.0.4/
+-rw-rw-rw-   0        0        0     2011 2023-06-05 10:37:26.405035 check-type-hints-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1488 2023-06-05 10:32:59.000000 check-type-hints-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 10:37:26.394051 check-type-hints-0.0.4/check_type_hints/
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:57:29.000000 check-type-hints-0.0.4/check_type_hints/__init__.py
+-rw-rw-rw-   0        0        0     3977 2023-06-05 09:42:13.000000 check-type-hints-0.0.4/check_type_hints/main.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:37:26.403127 check-type-hints-0.0.4/check_type_hints.egg-info/
+-rw-rw-rw-   0        0        0     2011 2023-06-05 10:37:26.000000 check-type-hints-0.0.4/check_type_hints.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-05 10:37:26.000000 check-type-hints-0.0.4/check_type_hints.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 10:37:26.000000 check-type-hints-0.0.4/check_type_hints.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-06-05 10:37:26.000000 check-type-hints-0.0.4/check_type_hints.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 10:37:26.000000 check-type-hints-0.0.4/check_type_hints.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-05 10:37:26.000000 check-type-hints-0.0.4/check_type_hints.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 10:37:26.406190 check-type-hints-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      548 2023-06-05 10:34:41.000000 check-type-hints-0.0.4/setup.py
```

### Comparing `check-type-hints-0.0.3/check_type_hints/main.py` & `check-type-hints-0.0.4/check_type_hints/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,17 +15,18 @@
         text=True,
     )
     changed_files = result.stdout.strip().split("\n")
     return [file for file in changed_files if file.endswith(".py")]
 
 
 class TypeHintChecker(ast.NodeVisitor):
-    def __init__(self, file: str):
+    def __init__(self, file: str, file_method: set = None):
         self.errors = []
         self.file = file
+        self.file_method = file_method if file_method else {}
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
         self.check_type_hints(node, "Function")
 
     def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> None:
         self.check_type_hints(node, "Async Function")
 
@@ -34,43 +35,72 @@
             if isinstance(item, (ast.FunctionDef, ast.AsyncFunctionDef)):
                 self.check_type_hints(item, "Method")
         self.generic_visit(node)
 
     def check_type_hints(
         self, node: Union[ast.FunctionDef, ast.AsyncFunctionDef], func_type: str
     ) -> None:
+        if self.file_method and node.name in self.file_method:
+            return
         if node.name != "__init__" and node.returns is None:
             self.errors.append(
                 f"Warning: {self.file} {func_type} '{node.name}' is missing return type hint"
             )
         for arg in node.args.args:
             if arg.arg in ["self", "cls"]:
                 continue
             if arg.annotation is None:
                 self.errors.append(
                     f"Warning: {self.file}{func_type} '{node.name}' is missing type hint for argument '{arg.arg}'"
                 )
 
 
-def check_file_for_type_hints(file: str) -> List[str]:
+def check_file_for_type_hints(file: str, filter_method: set = None) -> List[str]:
     with open(file, "r", encoding="utf-8") as source:
         tree = ast.parse(source.read())
 
-    checker = TypeHintChecker(file)
+    checker = TypeHintChecker(file, filter_method)
     checker.visit(tree)
 
     return checker.errors
 
 
+def filter_directory(file: str, filter_set: set) -> bool:
+    folds = file.split("/")
+    return folds[1] in filter_set if len(folds) > 1 else False
+
+
 @app.command()
-def check(ignore: Annotated[bool, typer.Option(
-    help="In the pre-commit, select whether to ignore the error and proceed with the commit.")] = False) -> None:
+def check(
+    ignore: Annotated[
+        bool,
+        typer.Option(
+            help="In the pre-commit, select whether to ignore the error and proceed with the commit."
+        ),
+    ] = False,
+    filter: Annotated[
+        List[str],
+        typer.Option(
+            help="You can enable filter to filter the folders that do not participate in the check. such as tests, pytests"
+        ),
+    ] = None,
+    method: Annotated[
+        List[str],
+        typer.Option(
+            help="You can choose to filter certain special methods, such as get, post, put, delete, patch."
+        ),
+    ] = None,
+) -> None:
     errors = []
+    filter = set(filter) if filter else None
+    method = set(method) if method else None
     for file in get_files_to_commit():
-        if file_errors := check_file_for_type_hints(file):
+        if filter and filter_directory(file, set(filter)):
+            continue
+        if file_errors := check_file_for_type_hints(file, method):
             errors.extend([f"{file}: {error}" for error in file_errors])
     if errors:
         print("Type hint errors found:")
         for error in errors:
             print(error)
     else:
         print("No type hint errors found")
```

