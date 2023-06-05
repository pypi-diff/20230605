# Comparing `tmp/jekyll_to_hugo-0.0.7.tar.gz` & `tmp/jekyll_to_hugo-0.0.8.tar.gz`

## Comparing `jekyll_to_hugo-0.0.7.tar` & `jekyll_to_hugo-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,42 @@
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/Makefile
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/config.yaml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/main.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/requirements-dev.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/requirements-test.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/requirements.txt
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/tox.ini
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/.idea/jekyll-to-hugo.iml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/.idea/misc.xml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/__init__.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/config.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/utils.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/converter/__init__.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/converter/converter.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/converter/regex_heuristics.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/converter/tags_heuristics.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/converter/wordpress_markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/io/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/io/reader.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/io/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/tests/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/tests/utils.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/tests/utils_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/tests/converter/__init__.py
--rw-r--r--   0        0        0     6583 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/app/tests/converter/wordpress_markdown_test.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/docker/Dockerfile
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/docker/Tox.Dockerfile
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/LICENSE
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/readme.md
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/Makefile
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/config.yaml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/main.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/requirements-dev.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/requirements-test.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/tox.ini
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/jekyll-to-hugo.iml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/__init__.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/config.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/utils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/converter/__init__.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/converter/converter.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/converter/regex_heuristics.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/converter/tags_heuristics.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/converter/wordpress_markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/io/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/io/reader.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/io/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/tests/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/tests/utils.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/tests/utils_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/tests/converter/__init__.py
+-rw-r--r--   0        0        0     6583 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/tests/converter/wordpress_markdown_test.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docker/Dockerfile
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docker/Tox.Dockerfile
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/Makefile
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/conf.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/make.bat
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/requirements.txt
+-rw-r--r--   0        0        0   112873 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/_static/nuculabs_logo.png
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/readme.md
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/PKG-INFO
```

### Comparing `jekyll_to_hugo-0.0.7/config.yaml` & `jekyll_to_hugo-0.0.8/config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 logging_level: "INFO"
-source_path: "/Users/dnutiu/PycharmProjects/jekyll-to-hugo/my_test_data/_posts"
-output_path: "/Users/dnutiu/NucuLabsProjects/NucuLabsDevBlog/content/posts"
+source_path: "/home/denis/PycharmProjects/jekyll-to-hugo/my_test_data/_posts"
+output_path: "/home/denis/Projects/NucuLabsDev/content/posts"
 converter: "wordpress_markdown_converter"
 converter_options:
   enable_regex_heuristics: true
   author_rewrite: "Denis Nuțiu"
   links_rewrite:
     - source: "http://localhost/"
       target: "/"
```

### Comparing `jekyll_to_hugo-0.0.7/main.py` & `jekyll_to_hugo-0.0.8/main.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/tox.ini` & `jekyll_to_hugo-0.0.8/tox.ini`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/app/config.py` & `jekyll_to_hugo-0.0.8/app/config.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/app/utils.py` & `jekyll_to_hugo-0.0.8/app/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def guard_against_none_or_empty_str(value: str, name: str):
     """
     Guard against None or empty string.
 
     Parameters:
-    ----------
+    -----------
     value: str
         The value to check.
     name: str
         The name of the value.
     """
 
     if value is None or not isinstance(value, str) or value == "":
@@ -29,15 +29,15 @@
 
 
 def guard_against_none(value, name: str):
     """
     Guard against None.
 
     Parameters:
-    ----------
+    -----------
     value: str
         The value to check.
     name: str
         The name of the value.
     """
 
     if value is None:
```

### Comparing `jekyll_to_hugo-0.0.7/app/converter/converter.py` & `jekyll_to_hugo-0.0.8/app/converter/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,10 +54,10 @@
                 file_writer = FileWriter(output_path.joinpath(source_abs_path.name))
 
                 self.markdown_converter.convert_jekyll_to_hugo(
                     file_reader,
                     file_writer,
                 )
                 posts_converted_count += 1
-                self._logger.info(f"Converted {posts_converted_count} posts! 🚀")
+            self._logger.info(f"Converted {posts_converted_count} posts! 🚀")
         except StopIteration:
             self._logger.fatal(f"Source path {source_path} does not exist!")
```

### Comparing `jekyll_to_hugo-0.0.7/app/converter/regex_heuristics.py` & `jekyll_to_hugo-0.0.8/app/converter/regex_heuristics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+import dataclasses
 import re
-from collections import namedtuple
+from typing import Callable
 
 from app import utils
 
-RegexCallback = namedtuple("RegexCallback", ["callback", "name"])
+
+@dataclasses.dataclass
+class RegexCallback:
+    callback: Callable[[re.Match], str]
+    name: str
 
 
 class RegexHeuristics:
     """
     Regex heuristics class for applying modifying a line using regex lines.
     """
```

### Comparing `jekyll_to_hugo-0.0.7/app/converter/wordpress_markdown.py` & `jekyll_to_hugo-0.0.8/app/converter/wordpress_markdown.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/app/io/reader.py` & `jekyll_to_hugo-0.0.8/app/io/reader.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/app/io/writer.py` & `jekyll_to_hugo-0.0.8/app/io/writer.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/app/tests/utils.py` & `jekyll_to_hugo-0.0.8/app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/app/tests/utils_test.py` & `jekyll_to_hugo-0.0.8/app/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/app/tests/converter/wordpress_markdown_test.py` & `jekyll_to_hugo-0.0.8/app/tests/converter/wordpress_markdown_test.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/.gitignore` & `jekyll_to_hugo-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/LICENSE` & `jekyll_to_hugo-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/pyproject.toml` & `jekyll_to_hugo-0.0.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jekyll-to-hugo"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Denis Nutiu", email="nuculabs@outlook.com" },
 ]
 description = "Python library for converting jekyll md files to Hugo."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -27,12 +27,18 @@
   "pydantic>=1.10, <2",
 ]
 
 [project.scripts]
 jekyll-to-hugo = "main:main"
 
 [project.optional-dependencies]
-dev = ["black", "pdoc", "isort", "autoflake", "pytest"]
+dev = ["black", "isort", "autoflake", "pytest"]
+docs = [
+  "sphinx",
+  "myst_parser",
+  "sphinx-autoapi>=2.1.0, <3",
+  "furo==2023.5.20"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/dnutiu/jekyll-to-hugo"
 "Bug Tracker" = "https://github.com/dnutiu/jekyll-to-hugo/issues"
```

### Comparing `jekyll_to_hugo-0.0.7/readme.md` & `jekyll_to_hugo-0.0.8/readme.md`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.7/PKG-INFO` & `jekyll_to_hugo-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jekyll-to-hugo
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python library for converting jekyll md files to Hugo.
 Project-URL: Homepage, https://github.com/dnutiu/jekyll-to-hugo
 Project-URL: Bug Tracker, https://github.com/dnutiu/jekyll-to-hugo/issues
 Author-email: Denis Nutiu <nuculabs@outlook.com>
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -18,16 +18,20 @@
 Requires-Dist: pydantic<2,>=1.10
 Requires-Dist: pyyaml
 Requires-Dist: soupsieve<3,>=2.4
 Provides-Extra: dev
 Requires-Dist: autoflake; extra == 'dev'
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
-Requires-Dist: pdoc; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: furo==2023.5.20; extra == 'docs'
+Requires-Dist: myst-parser; extra == 'docs'
+Requires-Dist: sphinx; extra == 'docs'
+Requires-Dist: sphinx-autoapi<3,>=2.1.0; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # Jekyll to Hugo Converter
 
 Jekyll to Hugo Converter is a simple tool to convert Jekyll posts to Hugo posts.
 
 I've used this tool to convert [my blog](https://blog.nuculabs.dev) from WordPress to Jekyll and finally to Hugo.
```

