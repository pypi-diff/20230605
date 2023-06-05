# Comparing `tmp/python_code_outline-0.1.2.tar.gz` & `tmp/python_code_outline-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_code_outline-0.1.2.tar", max compression
+gzip compressed data, was "python_code_outline-0.1.3.tar", max compression
```

## Comparing `python_code_outline-0.1.2.tar` & `python_code_outline-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 python_code_outline-0.1.2/LICENSE
--rw-r--r--   0        0        0     3373 2023-06-01 07:31:41.153014 python_code_outline-0.1.2/README.md
--rw-r--r--   0        0        0      540 2023-06-01 08:02:18.227987 python_code_outline-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      130 2023-06-01 08:01:36.675219 python_code_outline-0.1.2/python_code_outline/__init__.py
--rw-r--r--   0        0        0     5442 2023-06-01 08:00:46.613655 python_code_outline-0.1.2/python_code_outline/python_report_generator.py
--rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 python_code_outline-0.1.2/setup.py
--rw-r--r--   0        0        0     3727 1970-01-01 00:00:00.000000 python_code_outline-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 python_code_outline-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5714 2023-06-05 05:57:35.083931 python_code_outline-0.1.3/README.md
+-rw-r--r--   0        0        0      540 2023-06-05 06:35:50.296065 python_code_outline-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-06-05 06:35:45.789411 python_code_outline-0.1.3/python_code_outline/__init__.py
+-rw-r--r--   0        0        0     5494 2023-06-05 06:20:39.362103 python_code_outline-0.1.3/python_code_outline/python_report_generator.py
+-rw-r--r--   0        0        0     6336 1970-01-01 00:00:00.000000 python_code_outline-0.1.3/setup.py
+-rw-r--r--   0        0        0     6014 1970-01-01 00:00:00.000000 python_code_outline-0.1.3/PKG-INFO
```

### Comparing `python_code_outline-0.1.2/LICENSE` & `python_code_outline-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_code_outline-0.1.2/pyproject.toml` & `python_code_outline-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-code-outline"
-version = "0.1.2"
+version = "0.1.3"
 description = "Takes a folder path and outputs a text outline of the code, supports ignore files."
 authors = ["Sean Dearnaley <SeanDearnaley@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `python_code_outline-0.1.2/python_code_outline/python_report_generator.py` & `python_code_outline-0.1.3/python_code_outline/python_report_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,26 +75,29 @@
             output.extend(process_function_def(item))
         elif isinstance(item, ast.ClassDef):
             output.extend(process_class_def(item))
 
     return "\n".join(output)
 
 
+# ...
+
+
 def generate_report(
     root: Path, root_folder: Path, ignored_patterns: Optional[List[str]] = None
 ) -> str:
     """
     Generate a report of the code structure for all Python
     files in a given folder."""
 
     if ignored_patterns is None:
         ignored_patterns = []
 
     entries = list_entries(root)
-    report = []
+    report: List[str] = []  # add type hint for report list
 
     for entry in entries:
         if (
             entry.is_file()
             and not is_ignored(entry, ignored_patterns)
             and entry.suffix == ".py"
         ):
```

