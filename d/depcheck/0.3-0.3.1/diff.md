# Comparing `tmp/depcheck-0.3.tar.gz` & `tmp/depcheck-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depcheck-0.3.tar", max compression
+gzip compressed data, was "depcheck-0.3.1.tar", max compression
```

## Comparing `depcheck-0.3.tar` & `depcheck-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-06-02 16:01:31.743776 depcheck-0.3/LICENSE.md
--rw-r--r--   0        0        0     1804 2023-06-02 16:01:31.743776 depcheck-0.3/README.md
--rw-r--r--   0        0        0     1279 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/__init__.py
--rw-r--r--   0        0        0     2110 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/depchecker.py
--rw-r--r--   0        0        0     5513 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/models.py
--rw-r--r--   0        0        0     1305 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/readers.py
--rw-r--r--   0        0        0      139 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/util.py
--rw-r--r--   0        0        0      417 2023-06-02 16:01:31.743776 depcheck-0.3/depcheck/util_test.py
--rw-r--r--   0        0        0      963 2023-06-02 16:01:31.743776 depcheck-0.3/pyproject.toml
--rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 depcheck-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-05 16:06:44.171563 depcheck-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     1711 2023-06-05 16:06:44.171563 depcheck-0.3.1/README.md
+-rw-r--r--   0        0        0     1279 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/__init__.py
+-rw-r--r--   0        0        0     2110 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/depchecker.py
+-rw-r--r--   0        0        0     5522 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/models.py
+-rw-r--r--   0        0        0     1305 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/readers.py
+-rw-r--r--   0        0        0      139 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/util.py
+-rw-r--r--   0        0        0      417 2023-06-05 16:06:44.171563 depcheck-0.3.1/depcheck/util_test.py
+-rw-r--r--   0        0        0      965 2023-06-05 16:06:44.179564 depcheck-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 depcheck-0.3.1/PKG-INFO
```

### Comparing `depcheck-0.3/LICENSE.md` & `depcheck-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `depcheck-0.3/depcheck/__init__.py` & `depcheck-0.3.1/depcheck/__init__.py`

 * *Files identical despite different names*

### Comparing `depcheck-0.3/depcheck/depchecker.py` & `depcheck-0.3.1/depcheck/depchecker.py`

 * *Files identical despite different names*

### Comparing `depcheck-0.3/depcheck/models.py` & `depcheck-0.3.1/depcheck/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                     subpackages.add(detected_package)
 
         pkg_to_layers = self.__ruleset.packages_to_layers
 
         subp_copy = copy(subpackages)
         for idx, sp in enumerate(subp_copy):
             for pkg, pkg_layer in pkg_to_layers.items():
-                if pkg in sp and pkg_layer != layer and sp in subpackages:
+                if sp.startswith(pkg) and pkg_layer != layer and sp in subpackages:
                     # Remove the subpackages that belong in different layers
                     # eg: if we have layer 1="a" and layer 2="a.b", then "a.b.c" does not belong in layer 1
                     subpackages.remove(sp)
 
         return list(subpackages)
 
     def __package_dependencies(self, packages: set[str]) -> set[str]:
```

### Comparing `depcheck-0.3/depcheck/readers.py` & `depcheck-0.3.1/depcheck/readers.py`

 * *Files identical despite different names*

### Comparing `depcheck-0.3/pyproject.toml` & `depcheck-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "depcheck"
-version = "0.3"
+version = "0.3.1"
 authors = ["FlixMobility Tech <open-source@flixbus.com>"]
 description = "Python code quality package that helps in defining and restricting how components of your code may interact"
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/flix-tech/depcheck"
 repository = "https://github.com/flix-tech/depcheck"
 documentation = "https://github.com/flix-tech/depcheck"
```

### Comparing `depcheck-0.3/PKG-INFO` & `depcheck-0.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depcheck
-Version: 0.3
+Version: 0.3.1
 Summary: Python code quality package that helps in defining and restricting how components of your code may interact
 Home-page: https://github.com/flix-tech/depcheck
 License: MIT
 Keywords: dependencies,hexagonal,architecture,jdepend,deptrac
 Author: FlixMobility Tech
 Author-email: open-source@flixbus.com
 Requires-Python: >=3.9,<4.0
@@ -17,54 +17,53 @@
 Requires-Dist: pydeps (>=1.12.0,<2.0.0)
 Project-URL: Documentation, https://github.com/flix-tech/depcheck
 Project-URL: Repository, https://github.com/flix-tech/depcheck
 Description-Content-Type: text/markdown
 
 ![Depcheck: Dependency Checker](https://images2.imgbox.com/da/85/J5OEzbAH_o.jpg)
 
-Depcheck is a command line code-quality tool which supports adopting a 
-layered architecture by making it possible to specify dependency constraints
-between packages of your own Python application. 
+Depcheck is a command line code-quality tool which supports adopting a layered architecture
+by making it possible to specify dependency constraints between packages of your own Python application.
 The tool aims to achieve the same goals as [Deptrac][deptrac] in PHP and [JDepend][jdepend] in Java
 
 ## Install
-Install from [Pypi][pypi-link] via `pip install depcheck`
+- Via [`poetry`][poetry] (recommended): Install with `poetry add depcheck`
+- Via `pip`: Install from [Pypi][pypi-link] via `pip install depcheck`
 
 ## Usage
-Let's say you have a project with the directory structure below:
-```text
-example
-    root
-        foo
-        bar
-        main.py
-        __init__.py
-    README.md
-    .gitignore
-    .depcheck.yml
+To run via CLI you run:
+```shell
+depcheck <root_dir> -f <config_file>
+
+# Or, with poetry
+poetry run depcheck <root_dir> -f <config_file>
+```
+
+The `example` directory demonstrates how the tool works.
+
+```shell
+cd example
+
+poetry run depcheck example -f .depcheck.ok.yml  # This should be correct
+poetry run depcheck example -f .depcheck.errors.yml  # This should give errors
 ```
-Note: Package directories should contain **\_\_init\_\_.py** to be recognized as a package.
-- Navigate to the `example` then run `depcheck` for your project:
-    ```shell
-    poetry run depcheck example -f .depcheck.ok.yml  # This should be correct
-    poetry run depcheck example -f .depcheck.errors.yml  # This should give errors
-    ```
-- As you can see in the directory structure above, we have `.depcheck.yml` 
-  configuration file in the project directory. If you would like to change 
-  the path of the configuration file, use `-f` or `--file` argument:
-    ```shell
-    depcheck root -f /path/to/your/custom/depcheck.yml
-    ```
+
+To understand how to configure the tool, look inside the YML files. The `-f` argument is optional.
+Implicitly, the tool will look for `.depcheck.yml`.
+
+**NOTE:** Package directories should contain `__init__.py` to be recognized as a package!
+
 
 ## Contributing
 All contributions are welcomed! See our [CONTRIBUTING.md][contribution] document.
 
 
 <!-- Links -->
 [hexagonal-architecture]: https://en.wikipedia.org/wiki/Hexagonal_architecture_(software)
 [upgrade-python-version]: ./docs/upgrade-python-version.md
 [update-project-dependencies]: ./docs/upgrade-python-version.md
 [pypi-link]: https://pypi.org/project/depcheck/
 [contribution]: ./CONTRIBUTING.md
 [deptrac]: https://github.com/qossmic/deptrac
 [jdepend]: https://github.com/clarkware/jdepend
+[poetry]: https://python-poetry.org/
```

