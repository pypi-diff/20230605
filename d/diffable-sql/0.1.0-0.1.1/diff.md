# Comparing `tmp/diffable_sql-0.1.0.tar.gz` & `tmp/diffable_sql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffable_sql-0.1.0.tar", max compression
+gzip compressed data, was "diffable_sql-0.1.1.tar", max compression
```

## Comparing `diffable_sql-0.1.0.tar` & `diffable_sql-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1581 2023-06-05 12:38:54.595935 diffable_sql-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-03 23:15:48.955317 diffable_sql-0.1.0/diffable_sql/__init__.py
--rw-r--r--   0        0        0       76 2023-06-05 12:09:18.014828 diffable_sql-0.1.0/diffable_sql/__main__.py
--rw-r--r--   0        0        0     2368 2023-06-05 12:37:53.072327 diffable_sql-0.1.0/diffable_sql/cli.py
--rw-r--r--   0        0        0      652 2023-06-05 12:38:23.449479 diffable_sql-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2041 1970-01-01 00:00:00.000000 diffable_sql-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1581 2023-06-05 12:38:54.595935 diffable_sql-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 23:15:48.955317 diffable_sql-0.1.1/diffable_sql/__init__.py
+-rw-r--r--   0        0        0       76 2023-06-05 12:09:18.014828 diffable_sql-0.1.1/diffable_sql/__main__.py
+-rw-r--r--   0        0        0     2368 2023-06-05 12:37:53.072327 diffable_sql-0.1.1/diffable_sql/cli.py
+-rw-r--r--   0        0        0      761 2023-06-05 13:14:52.135504 diffable_sql-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 diffable_sql-0.1.1/PKG-INFO
```

### Comparing `diffable_sql-0.1.0/README.md` & `diffable_sql-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `diffable_sql-0.1.0/diffable_sql/cli.py` & `diffable_sql-0.1.1/diffable_sql/cli.py`

 * *Files identical despite different names*

### Comparing `diffable_sql-0.1.0/pyproject.toml` & `diffable_sql-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [tool.poetry]
 name = "diffable-sql"
-version = "0.1.0"
+version = "0.1.1"
 description = "Output normalised diffable database schemas"
 authors = ["Tom Forbes <tom@tomforb.es>"]
 readme = "README.md"
 packages = [{include = "diffable_sql"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 SQLAlchemy = "^2.0.15"
 click = "^8.1.3"
+psycopg2-binary = { version = "^2.9", optional = true }
 
 [tool.poetry.scripts]
 diffable-sql = "diffable_sql.cli:cli"
 
+[tool.poetry.extras]
+postgres = ["psycopg2-binary"]
+
 [tool.poetry.group.dev.dependencies]
 sqlalchemy = {extras = ["postgresql"], version = "^2.0.15"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `diffable_sql-0.1.0/PKG-INFO` & `diffable_sql-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: diffable-sql
-Version: 0.1.0
+Version: 0.1.1
 Summary: Output normalised diffable database schemas
 Author: Tom Forbes
 Author-email: tom@tomforb.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: postgres
 Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: psycopg2-binary (>=2.9,<3.0) ; extra == "postgres"
 Description-Content-Type: text/markdown
 
 # Diffable SQL
 
 This is a small tool that outputs SQL from a number of databases in a sorted, diff-friendly order.
 
 ## Install
```

