# Comparing `tmp/swagger-plugin-for-sphinx-3.0.0.tar.gz` & `tmp/swagger-plugin-for-sphinx-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swagger-plugin-for-sphinx-3.0.0.tar", last modified: Mon Mar  6 14:47:57 2023, max compression
+gzip compressed data, was "swagger-plugin-for-sphinx-3.1.0.tar", last modified: Mon Jun  5 14:00:52 2023, max compression
```

## Comparing `swagger-plugin-for-sphinx-3.0.0.tar` & `swagger-plugin-for-sphinx-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:47:57.565290 swagger-plugin-for-sphinx-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-06 14:47:30.000000 swagger-plugin-for-sphinx-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-03-06 14:47:57.565290 swagger-plugin-for-sphinx-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-03-06 14:47:30.000000 swagger-plugin-for-sphinx-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-06 14:47:30.000000 swagger-plugin-for-sphinx-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 14:47:57.565290 swagger-plugin-for-sphinx-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:47:57.565290 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-06 14:47:30.000000 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-06 14:47:30.000000 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:47:30.000000 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-06 14:47:30.000000 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx/swagger.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:47:57.565290 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-03-06 14:47:57.000000 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-06 14:47:57.000000 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:47:57.000000 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-06 14:47:57.000000 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-06 14:47:57.000000 swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:47:57.565290 swagger-plugin-for-sphinx-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-03-06 14:47:30.000000 swagger-plugin-for-sphinx-3.0.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/swagger.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-05 14:00:52.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-05 14:00:52.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:00:52.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 14:00:52.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 14:00:52.000000 swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:00:52.236040 swagger-plugin-for-sphinx-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-05 14:00:26.000000 swagger-plugin-for-sphinx-3.1.0/tests/test_plugin.py
```

### Comparing `swagger-plugin-for-sphinx-3.0.0/LICENSE` & `swagger-plugin-for-sphinx-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swagger-plugin-for-sphinx-3.0.0/PKG-INFO` & `swagger-plugin-for-sphinx-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagger-plugin-for-sphinx
-Version: 3.0.0
+Version: 3.1.0
 Summary: Sphinx plugin which renders a OpenAPI specification with Swagger
 Author-email: Kai Mueller <kai.mueller01@sap.com>
 License: Apache-2.0
 Project-URL: Issue Tracker, https://github.com/SAP/swagger-plugin-for-sphinx/issues
 Project-URL: Changelog, https://github.com/SAP/swagger-plugin-for-sphinx/blob/main/CHANGELOG.md
 Keywords: sphinx,swagger,plugin,openapi
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,17 +29,17 @@
 License-File: LICENSE
 
 [![REUSE status](https://api.reuse.software/badge/github.com/SAP/swagger-plugin-for-sphinx)](https://api.reuse.software/info/github.com/SAP/swagger-plugin-for-sphinx)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # Swagger Plugin for Sphinx
 
-This is handy plugin to bring [Swagger](https://swagger.io/) and [Sphinx](https://www.sphinx-doc.org/en/master/) together.
+This is a handy plugin to bring [Swagger](https://swagger.io/) and [Sphinx](https://www.sphinx-doc.org/en/master/) together.
 
-It is able to generate one or multiple swagger HTML pages with a custom configuration which host an OpenAPI specification.
+It can generate one or multiple swagger HTML pages with a custom configuration that hosts an OpenAPI specification.
 
 ## Install
 
 Just run `pip install swagger-plugin-for-sphinx`
 
 
 ## Usage
@@ -52,53 +52,53 @@
 Then add the main configuration for swagger:
 ```python
 swagger_present_uri = ""
 swagger_bundle_uri = ""
 swagger_css_uri = ""
 ```
 These correspond to the modules explained [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/installation.md).
-By default the latest release is used from [here](https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest).
+By default, the latest release is used from [here](https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest).
 
-As a last step, define the swagger configuration as followed:
+As a last step, define the swagger configuration as follows:
 ```python
 swagger = [
     {
         "name": "Service API",
         "page": "openapi",
         "options": {
             "url": "openapi.yaml",
         },
     }
 ]
 ```
-Each item of the list will generate a new swagger HTML page.
+Each item on the list will generate a new swagger HTML page.
 The `name` is the HTML page name and `page` defines the file name without an extension. This needs to be included in the TOC.
 The `options` are then used for the `SwaggerUIBundle` as defined [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/configuration.md).
 Please don't specify the `dom_id` since it's hardcoded in the HTML page.
 
-In the sphinx build, a HTML page is created and put into the `_static` directory of the build.
+In the sphinx build, an HTML page is created and put into the `_static` directory of the build.
 
-If the specification is provided as a file, don't forget to copy it (e.g. by putting it into the `html_static_path`).
+If the specification is provided as a file, don't forget to copy it (e.g., by putting it into the `html_static_path`).
 
-To silence the warning `toctree contains reference to nonexisting document`,, just put a dummy file with the same name as `page` into the source folder.
+To silence the warning `toctree contains reference to nonexisting document`, just put a dummy file with the same name as `page` into the source folder.
 
 ## Build and Publish
 
 This project uses `setuptools` as the dependency management and build tool.
 To publish a new release, follow these steps:
 * Update the version in the `pyproject.toml`
 * Add an entry in the changelog
 * Push a new tag like `vX.X.X` to trigger the release
 
 ## Support, Feedback, Contributing
 
-This project is open to feature requests/suggestions, bug reports etc. via [GitHub issues](https://github.com/SAP/<your-project>/issues). Contribution and feedback are encouraged and always welcome. For more information about how to contribute, the project structure, as well as additional contribution information, see our [Contribution Guidelines](CONTRIBUTING.md).
+This project is open to feature requests/suggestions, bug reports etc., via [GitHub issues](https://github.com/SAP/<your-project>/issues). Contribution and feedback are encouraged and always welcome. For more information about how to contribute, the project structure, as well as additional contribution information, see our [Contribution Guidelines](CONTRIBUTING.md).
 
 ## Code of Conduct
 
 We as members, contributors, and leaders pledge to make participation in our community a harassment-free experience for everyone. By participating in this project, you agree to abide by its [Code of Conduct](CODE_OF_CONDUCT.md) at all times.
 
 ## Licensing
 
-Copyright 2022 SAP SE or an SAP affiliate company and swagger-plugin-for-sphinx contributors.
+Copyright 2023 SAP SE or an SAP affiliate company and swagger-plugin-for-sphinx contributors.
 Please see our [LICENSE](LICENSE) for copyright and license information.
 Detailed information including third-party components and their licensing/copyright information is available [via the REUSE tool](https://api.reuse.software/info/github.com/SAP/<your-project>).
```

### Comparing `swagger-plugin-for-sphinx-3.0.0/README.md` & `swagger-plugin-for-sphinx-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [![REUSE status](https://api.reuse.software/badge/github.com/SAP/swagger-plugin-for-sphinx)](https://api.reuse.software/info/github.com/SAP/swagger-plugin-for-sphinx)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # Swagger Plugin for Sphinx
 
-This is handy plugin to bring [Swagger](https://swagger.io/) and [Sphinx](https://www.sphinx-doc.org/en/master/) together.
+This is a handy plugin to bring [Swagger](https://swagger.io/) and [Sphinx](https://www.sphinx-doc.org/en/master/) together.
 
-It is able to generate one or multiple swagger HTML pages with a custom configuration which host an OpenAPI specification.
+It can generate one or multiple swagger HTML pages with a custom configuration that hosts an OpenAPI specification.
 
 ## Install
 
 Just run `pip install swagger-plugin-for-sphinx`
 
 
 ## Usage
@@ -22,53 +22,53 @@
 Then add the main configuration for swagger:
 ```python
 swagger_present_uri = ""
 swagger_bundle_uri = ""
 swagger_css_uri = ""
 ```
 These correspond to the modules explained [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/installation.md).
-By default the latest release is used from [here](https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest).
+By default, the latest release is used from [here](https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest).
 
-As a last step, define the swagger configuration as followed:
+As a last step, define the swagger configuration as follows:
 ```python
 swagger = [
     {
         "name": "Service API",
         "page": "openapi",
         "options": {
             "url": "openapi.yaml",
         },
     }
 ]
 ```
-Each item of the list will generate a new swagger HTML page.
+Each item on the list will generate a new swagger HTML page.
 The `name` is the HTML page name and `page` defines the file name without an extension. This needs to be included in the TOC.
 The `options` are then used for the `SwaggerUIBundle` as defined [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/configuration.md).
 Please don't specify the `dom_id` since it's hardcoded in the HTML page.
 
-In the sphinx build, a HTML page is created and put into the `_static` directory of the build.
+In the sphinx build, an HTML page is created and put into the `_static` directory of the build.
 
-If the specification is provided as a file, don't forget to copy it (e.g. by putting it into the `html_static_path`).
+If the specification is provided as a file, don't forget to copy it (e.g., by putting it into the `html_static_path`).
 
-To silence the warning `toctree contains reference to nonexisting document`,, just put a dummy file with the same name as `page` into the source folder.
+To silence the warning `toctree contains reference to nonexisting document`, just put a dummy file with the same name as `page` into the source folder.
 
 ## Build and Publish
 
 This project uses `setuptools` as the dependency management and build tool.
 To publish a new release, follow these steps:
 * Update the version in the `pyproject.toml`
 * Add an entry in the changelog
 * Push a new tag like `vX.X.X` to trigger the release
 
 ## Support, Feedback, Contributing
 
-This project is open to feature requests/suggestions, bug reports etc. via [GitHub issues](https://github.com/SAP/<your-project>/issues). Contribution and feedback are encouraged and always welcome. For more information about how to contribute, the project structure, as well as additional contribution information, see our [Contribution Guidelines](CONTRIBUTING.md).
+This project is open to feature requests/suggestions, bug reports etc., via [GitHub issues](https://github.com/SAP/<your-project>/issues). Contribution and feedback are encouraged and always welcome. For more information about how to contribute, the project structure, as well as additional contribution information, see our [Contribution Guidelines](CONTRIBUTING.md).
 
 ## Code of Conduct
 
 We as members, contributors, and leaders pledge to make participation in our community a harassment-free experience for everyone. By participating in this project, you agree to abide by its [Code of Conduct](CODE_OF_CONDUCT.md) at all times.
 
 ## Licensing
 
-Copyright 2022 SAP SE or an SAP affiliate company and swagger-plugin-for-sphinx contributors.
+Copyright 2023 SAP SE or an SAP affiliate company and swagger-plugin-for-sphinx contributors.
 Please see our [LICENSE](LICENSE) for copyright and license information.
 Detailed information including third-party components and their licensing/copyright information is available [via the REUSE tool](https://api.reuse.software/info/github.com/SAP/<your-project>).
```

### Comparing `swagger-plugin-for-sphinx-3.0.0/pyproject.toml` & `swagger-plugin-for-sphinx-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "swagger-plugin-for-sphinx"
-version = "3.0.0"
+version = "3.1.0"
 description = "Sphinx plugin which renders a OpenAPI specification with Swagger"
 authors = [{ name = "Kai Mueller", email = "kai.mueller01@sap.com"}]
 readme = "README.md"
 keywords = ["sphinx", "swagger", "plugin", "openapi"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
@@ -25,38 +25,38 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
     "Typing :: Typed"
 ]
 requires-python = ">=3.8,<4"
 dependencies = [
-    "sphinx~=6.0",
+    "sphinx>=6.0,<8",
     "jinja2~=3.0",
 ]
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Issue Tracker" = "https://github.com/SAP/swagger-plugin-for-sphinx/issues"
 "Changelog" = "https://github.com/SAP/swagger-plugin-for-sphinx/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 dev = [
-    "pre-commit==3.1.0",
-    "pylint==2.16.2",
-    "pytest==7.2.1",
+    "pre-commit==3.3.2",
+    "pylint==2.17.4",
+    "pytest==7.3.1",
     "pytest-mock==3.10.0",
     "coverage==7.2.0",
     "diff-cover==7.5.0",
-    "pytest-cov==4.0.0",
-    "black==23.1.0",
+    "pytest-cov==4.1.0",
+    "black==23.3.0",
     "isort==5.12.0",
     "flake8==6.0.0",
-    "mypy==1.0.1",
+    "mypy==1.3.0",
 ]
 
 [tool.setuptools.packages.find]
 include = ["swagger_plugin_for_sphinx"]
 
 [tool.setuptools.package-data]
 swagger_plugin_for_sphinx = ["py.typed", "*.j2"]
```

### Comparing `swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx/_plugin.py` & `swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/_plugin.py`

 * *Files identical despite different names*

### Comparing `swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx/swagger.j2` & `swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx/swagger.j2`

 * *Files identical despite different names*

### Comparing `swagger-plugin-for-sphinx-3.0.0/swagger_plugin_for_sphinx.egg-info/PKG-INFO` & `swagger-plugin-for-sphinx-3.1.0/swagger_plugin_for_sphinx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagger-plugin-for-sphinx
-Version: 3.0.0
+Version: 3.1.0
 Summary: Sphinx plugin which renders a OpenAPI specification with Swagger
 Author-email: Kai Mueller <kai.mueller01@sap.com>
 License: Apache-2.0
 Project-URL: Issue Tracker, https://github.com/SAP/swagger-plugin-for-sphinx/issues
 Project-URL: Changelog, https://github.com/SAP/swagger-plugin-for-sphinx/blob/main/CHANGELOG.md
 Keywords: sphinx,swagger,plugin,openapi
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,17 +29,17 @@
 License-File: LICENSE
 
 [![REUSE status](https://api.reuse.software/badge/github.com/SAP/swagger-plugin-for-sphinx)](https://api.reuse.software/info/github.com/SAP/swagger-plugin-for-sphinx)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # Swagger Plugin for Sphinx
 
-This is handy plugin to bring [Swagger](https://swagger.io/) and [Sphinx](https://www.sphinx-doc.org/en/master/) together.
+This is a handy plugin to bring [Swagger](https://swagger.io/) and [Sphinx](https://www.sphinx-doc.org/en/master/) together.
 
-It is able to generate one or multiple swagger HTML pages with a custom configuration which host an OpenAPI specification.
+It can generate one or multiple swagger HTML pages with a custom configuration that hosts an OpenAPI specification.
 
 ## Install
 
 Just run `pip install swagger-plugin-for-sphinx`
 
 
 ## Usage
@@ -52,53 +52,53 @@
 Then add the main configuration for swagger:
 ```python
 swagger_present_uri = ""
 swagger_bundle_uri = ""
 swagger_css_uri = ""
 ```
 These correspond to the modules explained [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/installation.md).
-By default the latest release is used from [here](https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest).
+By default, the latest release is used from [here](https://cdn.jsdelivr.net/npm/swagger-ui-dist@latest).
 
-As a last step, define the swagger configuration as followed:
+As a last step, define the swagger configuration as follows:
 ```python
 swagger = [
     {
         "name": "Service API",
         "page": "openapi",
         "options": {
             "url": "openapi.yaml",
         },
     }
 ]
 ```
-Each item of the list will generate a new swagger HTML page.
+Each item on the list will generate a new swagger HTML page.
 The `name` is the HTML page name and `page` defines the file name without an extension. This needs to be included in the TOC.
 The `options` are then used for the `SwaggerUIBundle` as defined [here](https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/configuration.md).
 Please don't specify the `dom_id` since it's hardcoded in the HTML page.
 
-In the sphinx build, a HTML page is created and put into the `_static` directory of the build.
+In the sphinx build, an HTML page is created and put into the `_static` directory of the build.
 
-If the specification is provided as a file, don't forget to copy it (e.g. by putting it into the `html_static_path`).
+If the specification is provided as a file, don't forget to copy it (e.g., by putting it into the `html_static_path`).
 
-To silence the warning `toctree contains reference to nonexisting document`,, just put a dummy file with the same name as `page` into the source folder.
+To silence the warning `toctree contains reference to nonexisting document`, just put a dummy file with the same name as `page` into the source folder.
 
 ## Build and Publish
 
 This project uses `setuptools` as the dependency management and build tool.
 To publish a new release, follow these steps:
 * Update the version in the `pyproject.toml`
 * Add an entry in the changelog
 * Push a new tag like `vX.X.X` to trigger the release
 
 ## Support, Feedback, Contributing
 
-This project is open to feature requests/suggestions, bug reports etc. via [GitHub issues](https://github.com/SAP/<your-project>/issues). Contribution and feedback are encouraged and always welcome. For more information about how to contribute, the project structure, as well as additional contribution information, see our [Contribution Guidelines](CONTRIBUTING.md).
+This project is open to feature requests/suggestions, bug reports etc., via [GitHub issues](https://github.com/SAP/<your-project>/issues). Contribution and feedback are encouraged and always welcome. For more information about how to contribute, the project structure, as well as additional contribution information, see our [Contribution Guidelines](CONTRIBUTING.md).
 
 ## Code of Conduct
 
 We as members, contributors, and leaders pledge to make participation in our community a harassment-free experience for everyone. By participating in this project, you agree to abide by its [Code of Conduct](CODE_OF_CONDUCT.md) at all times.
 
 ## Licensing
 
-Copyright 2022 SAP SE or an SAP affiliate company and swagger-plugin-for-sphinx contributors.
+Copyright 2023 SAP SE or an SAP affiliate company and swagger-plugin-for-sphinx contributors.
 Please see our [LICENSE](LICENSE) for copyright and license information.
 Detailed information including third-party components and their licensing/copyright information is available [via the REUSE tool](https://api.reuse.software/info/github.com/SAP/<your-project>).
```

### Comparing `swagger-plugin-for-sphinx-3.0.0/tests/test_plugin.py` & `swagger-plugin-for-sphinx-3.1.0/tests/test_plugin.py`

 * *Files identical despite different names*

