# Comparing `tmp/mock_data_generator-0.1.0.tar.gz` & `tmp/mock_data_generator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-0.1.0.tar", max compression
+gzip compressed data, was "mock_data_generator-1.0.1.tar", max compression
```

## Comparing `mock_data_generator-0.1.0.tar` & `mock_data_generator-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-0.1.0/LICENSE
--rw-r--r--   0        0        0     1917 2023-06-05 04:47:23.541208 mock_data_generator-0.1.0/mock_data_generator/driver.py
--rw-r--r--   0        0        0      855 2023-06-05 06:13:59.110635 mock_data_generator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 mock_data_generator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1913 2023-06-05 06:20:40.916685 mock_data_generator-1.0.1/README.md
+-rw-r--r--   0        0        0     1917 2023-06-05 04:47:23.541208 mock_data_generator-1.0.1/mock_data_generator/driver.py
+-rw-r--r--   0        0        0      876 2023-06-05 06:59:01.159267 mock_data_generator-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 mock_data_generator-1.0.1/PKG-INFO
```

### Comparing `mock_data_generator-0.1.0/LICENSE` & `mock_data_generator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-0.1.0/mock_data_generator/driver.py` & `mock_data_generator-1.0.1/mock_data_generator/driver.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-0.1.0/pyproject.toml` & `mock_data_generator-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "0.1.0"
+version = "1.0.1"
 description = "Generate mock data using json schema supplied."
 authors = ["Rahul Auti <rahulsmtauti@gmail.com>"]
 license = "MIT"
+readme = "README.md"
 
 [tool.poetry.scripts]
 generate = "mock_data_generator.driver:run"
 
 [tool.poetry.dependencies]
 python = "~3.11.3"
 faker = "^18.9.0"
@@ -28,13 +29,13 @@
 ]
 
 [build-system]
 requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

