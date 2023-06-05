# Comparing `tmp/jekyll_to_hugo-0.0.8.tar.gz` & `tmp/jekyll_to_hugo-0.0.9.tar.gz`

## Comparing `jekyll_to_hugo-0.0.8.tar` & `jekyll_to_hugo-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/Makefile
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/config.yaml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/main.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/requirements-dev.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/requirements-test.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/requirements.txt
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/tox.ini
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/jekyll-to-hugo.iml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/__init__.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/config.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/utils.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/converter/__init__.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/converter/converter.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/converter/regex_heuristics.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/converter/tags_heuristics.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/converter/wordpress_markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/io/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/io/reader.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/io/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/tests/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/tests/utils.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/tests/utils_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/tests/converter/__init__.py
--rw-r--r--   0        0        0     6583 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/app/tests/converter/wordpress_markdown_test.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docker/Dockerfile
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docker/Tox.Dockerfile
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/Makefile
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/conf.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/make.bat
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/requirements.txt
--rw-r--r--   0        0        0   112873 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/docs/_static/nuculabs_logo.png
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/LICENSE
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/readme.md
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/Makefile
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/config.yaml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/requirements-dev.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/requirements-test.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/tox.ini
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/.idea/jekyll-to-hugo.iml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/__init__.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/config.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/main.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/utils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/converter/__init__.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/converter/converter.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/converter/regex_heuristics.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/converter/tags_heuristics.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/converter/wordpress_markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/io/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/io/reader.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/io/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/tests/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/tests/utils.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/tests/utils_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/tests/converter/__init__.py
+-rw-r--r--   0        0        0     6583 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/app/tests/converter/wordpress_markdown_test.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/docker/Dockerfile
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/docker/Tox.Dockerfile
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/docs/conf.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/docs/make.bat
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0   112873 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/docs/_static/nuculabs_logo.png
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/readme.md
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.9/PKG-INFO
```

### Comparing `jekyll_to_hugo-0.0.8/config.yaml` & `jekyll_to_hugo-0.0.9/config.yaml`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/main.py` & `jekyll_to_hugo-0.0.9/app/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 
 from app.config import Configurator, ensure_config_exists
 from app.converter import Converter
 
 
 def main():
+    """
+    Main function of the program.
+    """
     # Configurator
     ensure_config_exists()
     configurator = Configurator()
 
     # Logging configuration
     logging.basicConfig(
         format="%(asctime)s %(process)d %(levelname)s %(message)s",
```

### Comparing `jekyll_to_hugo-0.0.8/tox.ini` & `jekyll_to_hugo-0.0.9/tox.ini`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/app/config.py` & `jekyll_to_hugo-0.0.9/app/config.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/app/utils.py` & `jekyll_to_hugo-0.0.9/app/utils.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/app/converter/converter.py` & `jekyll_to_hugo-0.0.9/app/converter/converter.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/app/converter/regex_heuristics.py` & `jekyll_to_hugo-0.0.9/app/converter/regex_heuristics.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/app/converter/wordpress_markdown.py` & `jekyll_to_hugo-0.0.9/app/converter/wordpress_markdown.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/app/io/reader.py` & `jekyll_to_hugo-0.0.9/app/io/reader.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/app/io/writer.py` & `jekyll_to_hugo-0.0.9/app/io/writer.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/app/tests/utils.py` & `jekyll_to_hugo-0.0.9/app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/app/tests/utils_test.py` & `jekyll_to_hugo-0.0.9/app/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/app/tests/converter/wordpress_markdown_test.py` & `jekyll_to_hugo-0.0.9/app/tests/converter/wordpress_markdown_test.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/docs/Makefile` & `jekyll_to_hugo-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/docs/conf.py` & `jekyll_to_hugo-0.0.9/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 project = "Jekyll To Hugo"
 copyright = "2023-Present, Denis Nutiu and contributors"
 author = "Denis Nutiu and contributors"
-release = "0.0.7"
+release = "0.0.9"
 html_logo = "_static/nuculabs_logo.png"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["autoapi.extension", "myst_parser"]
```

### Comparing `jekyll_to_hugo-0.0.8/docs/make.bat` & `jekyll_to_hugo-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/docs/_static/nuculabs_logo.png` & `jekyll_to_hugo-0.0.9/docs/_static/nuculabs_logo.png`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/.gitignore` & `jekyll_to_hugo-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/LICENSE` & `jekyll_to_hugo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/pyproject.toml` & `jekyll_to_hugo-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jekyll-to-hugo"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Denis Nutiu", email="nuculabs@outlook.com" },
 ]
 description = "Python library for converting jekyll md files to Hugo."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -24,15 +24,15 @@
   "beautifulsoup4>=4.12, <5",
   "PyYAML",
   "soupsieve>=2.4, <3",
   "pydantic>=1.10, <2",
 ]
 
 [project.scripts]
-jekyll-to-hugo = "main:main"
+jekyll-to-hugo = "app.main:main"
 
 [project.optional-dependencies]
 dev = ["black", "isort", "autoflake", "pytest"]
 docs = [
   "sphinx",
   "myst_parser",
   "sphinx-autoapi>=2.1.0, <3",
```

### Comparing `jekyll_to_hugo-0.0.8/readme.md` & `jekyll_to_hugo-0.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.8/PKG-INFO` & `jekyll_to_hugo-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jekyll-to-hugo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python library for converting jekyll md files to Hugo.
 Project-URL: Homepage, https://github.com/dnutiu/jekyll-to-hugo
 Project-URL: Bug Tracker, https://github.com/dnutiu/jekyll-to-hugo/issues
 Author-email: Denis Nutiu <nuculabs@outlook.com>
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

