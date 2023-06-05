# Comparing `tmp/sqlalchemy-vertica-python-0.5.9.tar.gz` & `tmp/sqlalchemy-vertica-python-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlalchemy-vertica-python-0.5.9.tar", last modified: Tue Jun  9 15:29:57 2020, max compression
+gzip compressed data, was "sqlalchemy-vertica-python-0.6.3.tar", last modified: Mon Jun  5 20:29:03 2023, max compression
```

## Comparing `sqlalchemy-vertica-python-0.5.9.tar` & `sqlalchemy-vertica-python-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3867 2020-06-09 15:29:52.000000 sqlalchemy-vertica-python-0.5.9/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/sqla_vertica_python/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13435 2020-06-09 15:29:52.000000 sqlalchemy-vertica-python-0.5.9/sqla_vertica_python/vertica_python.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-06-09 15:29:52.000000 sqlalchemy-vertica-python-0.5.9/sqla_vertica_python/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/sqlalchemy_vertica_python.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/sqlalchemy_vertica_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/sqlalchemy_vertica_python.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      395 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/sqlalchemy_vertica_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      110 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/sqlalchemy_vertica_python.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/sqlalchemy_vertica_python.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2304 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/sqlalchemy_vertica_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1204 2020-06-09 15:29:52.000000 sqlalchemy-vertica-python-0.5.9/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      260 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2304 2020-06-09 15:29:57.000000 sqlalchemy-vertica-python-0.5.9/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:29:03.903907 sqlalchemy-vertica-python-0.6.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-06-05 20:28:59.000000 sqlalchemy-vertica-python-0.6.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2304 2023-06-05 20:29:03.907907 sqlalchemy-vertica-python-0.6.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1204 2023-06-05 20:28:59.000000 sqlalchemy-vertica-python-0.6.3/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-06-05 20:29:03.907907 sqlalchemy-vertica-python-0.6.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3867 2023-06-05 20:28:59.000000 sqlalchemy-vertica-python-0.6.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:29:03.903907 sqlalchemy-vertica-python-0.6.3/sqla_vertica_python/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:28:59.000000 sqlalchemy-vertica-python-0.6.3/sqla_vertica_python/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13636 2023-06-05 20:28:59.000000 sqlalchemy-vertica-python-0.6.3/sqla_vertica_python/vertica_python.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 20:29:03.903907 sqlalchemy-vertica-python-0.6.3/sqlalchemy_vertica_python.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2304 2023-06-05 20:29:03.000000 sqlalchemy-vertica-python-0.6.3/sqlalchemy_vertica_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2023-06-05 20:29:03.000000 sqlalchemy-vertica-python-0.6.3/sqlalchemy_vertica_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-05 20:29:03.000000 sqlalchemy-vertica-python-0.6.3/sqlalchemy_vertica_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      110 2023-06-05 20:29:03.000000 sqlalchemy-vertica-python-0.6.3/sqlalchemy_vertica_python.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-06-05 20:29:03.000000 sqlalchemy-vertica-python-0.6.3/sqlalchemy_vertica_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-06-05 20:29:03.000000 sqlalchemy-vertica-python-0.6.3/sqlalchemy_vertica_python.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sqlalchemy-vertica-python-0.5.9/setup.py` & `sqlalchemy-vertica-python-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.cmd import Command
 from setuptools import setup
 from setuptools.command.install import install
 import os.path
 import sys
 
 
-__version__ = '0.5.9'
+__version__ = '0.6.3'
 
 
 # From https://circleci.com/blog/continuously-deploying-python-packages-to-pypi-with-circleci/
 class VerifyVersionCommand(install):
     """Custom command to verify that the git tag matches our version"""
     description = 'verify that the git tag matches our version'
```

### Comparing `sqlalchemy-vertica-python-0.5.9/sqla_vertica_python/vertica_python.py` & `sqlalchemy-vertica-python-0.6.3/sqla_vertica_python/vertica_python.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from sqlalchemy import text
 from sqlalchemy import types as sqltypes
 from sqlalchemy.dialects.postgresql.base import PGDialect
 from sqlalchemy.dialects.postgresql import INTERVAL
 from sqlalchemy.engine import reflection
 from sqlalchemy.schema import CreateColumn
 from sqlalchemy.ext.compiler import compiles
 
@@ -38,14 +39,15 @@
         'BOOLEAN': sqltypes.BOOLEAN,
 
         'CHAR': sqltypes.CHAR,
         'VARCHAR': sqltypes.VARCHAR,
         'LONG VARCHAR': sqltypes.VARCHAR,
         'VARCHAR2': sqltypes.VARCHAR,
         'TEXT': sqltypes.VARCHAR,
+        'UUID': sqltypes.VARCHAR,
 
         'DATE': sqltypes.DATE(),
         'DATETIME': sqltypes.DATETIME(),
         'SMALLDATETIME': sqltypes.DATETIME(),
         'TIME': sqltypes.TIME(),
         'TIMETZ': sqltypes.TIME(timezone=True),
         'TIME WITH TIMEZONE': sqltypes.TIME(timezone=True),
@@ -83,139 +85,141 @@
         return (
             isinstance(e, self.dbapi.Error) and
             connection is not None and
             connection.closed()
         )
 
     @classmethod
-    def dbapi(cls):
+    def import_dbapi(cls):
         vp_module = __import__('vertica_python')
 
         # sqlalchemy expects to find the base Error class here,
         # so we need to alias it
         vp_module.Error = vp_module.errors.Error
 
         return vp_module
+    
+    dbapi = import_dbapi
 
 
     def create_connect_args(self, url):
         opts = url.translate_connect_args(username='user')
         opts.update(url.query)
         return [[], opts]
 
 
     def has_schema(self, connection, schema):
         query = ("SELECT EXISTS (SELECT schema_name FROM v_catalog.schemata "
                  "WHERE schema_name='%s')") % (schema)
-        rs = connection.execute(query)
+        rs = connection.execute(text(query))
         return bool(rs.scalar())
 
 
     def has_table(self, connection, table_name, schema=None):
         if schema is None:
             schema = self._get_default_schema_name(connection)
         query = ("SELECT EXISTS ("
                  "SELECT table_name FROM v_catalog.all_tables "
                  "WHERE schema_name='%s' AND "
                  "table_name='%s'"
                  ")") % (schema, table_name)
-        rs = connection.execute(query)
+        rs = connection.execute(text(query))
         return bool(rs.scalar())
 
 
     def has_sequence(self, connection, sequence_name, schema=None):
         if schema is None:
             schema = self._get_default_schema_name(connection)
         query = ("SELECT EXISTS ("
                  "SELECT sequence_name FROM v_catalog.sequences "
                  "WHERE sequence_schema='%s' AND "
                  "sequence_name='%s'"
                  ")") % (schema, sequence_name)
-        rs = connection.execute(query)
+        rs = connection.execute(text(query))
         return bool(rs.scalar())
 
 
     def has_type(self, connection, type_name, schema=None):
         query = ("SELECT EXISTS ("
                  "SELECT type_name FROM v_catalog.types "
                  "WHERE type_name='%s'"
                  ")") % (type_name)
-        rs = connection.execute(query)
+        rs = connection.execute(text(query))
         return bool(rs.scalar())
 
 
     def _get_server_version_info(self, connection):
-        v = connection.scalar("select version()")
+        v = connection.scalar(text("select version()"))
         m = re.match(
             '.*Vertica Analytic Database '
             'v(\d+)\.(\d+)\.(\d)+.*',
             v)
         if not m:
             raise AssertionError(
                 "Could not determine version from string '%s'" % v)
         return tuple([int(x) for x in m.group(1, 2, 3) if x is not None])
 
 
     def _get_default_schema_name(self, connection):
-        return connection.scalar("select current_schema()")
+        return connection.scalar(text("select current_schema()"))
 
 
     @reflection.cache
     def get_schema_names(self, connection, **kw):
         query = "SELECT schema_name FROM v_catalog.schemata ORDER BY schema_name"
-        rs = connection.execute(query)
+        rs = connection.execute(text(query))
         return [row[0] for row in rs if not row[0].startswith('v_')]
 
 
     @reflection.cache
     def get_table_comment(self, connection, table_name, schema=None, **kw):
         schema_conditional = (
             "" if schema is None else "AND object_schema = '{schema}'".format(schema=schema))
         query = """
         SELECT comment FROM v_catalog.comments WHERE object_type = 'TABLE'
         AND object_name = '{table_name}'
         {schema_conditional}
         """.format(table_name=table_name, schema_conditional=schema_conditional)
-        rs = connection.execute(query)
+        rs = connection.execute(text(query))
         return {"text": rs.scalar()}
 
 
     @reflection.cache
     def get_table_names(self, connection, schema=None, **kw):
         s = ["SELECT table_name FROM v_catalog.tables"]
         if schema is not None:
             s.append("WHERE table_schema = '%s'" % (schema,))
         s.append("ORDER BY table_schema, table_name")
 
-        rs = connection.execute(' '.join(s))
+        rs = connection.execute(text(' '.join(s)))
         return [row[0] for row in rs]
 
 
     @reflection.cache
     def get_view_names(self, connection, schema=None, **kw):
         s = ["SELECT table_name FROM v_catalog.views"]
         if schema is not None:
             s.append("WHERE table_schema = '%s'" % (schema,))
         s.append("ORDER BY table_schema, table_name")
 
-        rs = connection.execute(' '.join(s))
+        rs = connection.execute(text(' '.join(s)))
         return [row[0] for row in rs]
 
     @reflection.cache
     def get_columns(self, connection, table_name, schema=None, **kw):
         schema_conditional = (
             "" if schema is None else "AND table_schema = '{schema}'".format(schema=schema))
 
         pk_column_select = """
         SELECT column_name FROM v_catalog.primary_keys
         WHERE table_name = '{table_name}'
         AND constraint_type = 'p'
         {schema_conditional}
         """.format(table_name=table_name, schema_conditional=schema_conditional)
-        primary_key_columns = tuple(row[0] for row in connection.execute(pk_column_select))
+        primary_key_columns = tuple(row[0] for row in connection.execute(text(pk_column_select)))
         column_select = """
         SELECT
           column_name,
           data_type,
           column_default,
           is_nullable,
           is_identity,
@@ -233,32 +237,32 @@
           ordinal_position
         FROM v_catalog.view_columns
         where table_name = '{table_name}'
         {schema_conditional}
         ORDER BY ordinal_position ASC
         """.format(table_name=table_name, schema_conditional=schema_conditional)
         colobjs = []
-        column_select_results = list(connection.execute(column_select))
-        for row in list(connection.execute(column_select)):
-            sequence_info = connection.execute("""
+        column_select_results = list(connection.execute(text(column_select)))
+        for row in list(connection.execute(text(column_select))):
+            sequence_info = connection.execute(text("""
                 SELECT
                 sequence_name as name,
                 minimum as start,
                 increment_by as increment
                 FROM v_catalog.sequences
                 WHERE identity_table_name = '{table_name}'
                 {schema_conditional}
                 """.format(
                     table_name=table_name,
                     schema_conditional=(
                         "" if schema is None
                         else "AND sequence_schema = '{schema}'".format(schema=schema)
                     )
                 )
-            ).first() if row.is_identity else None
+            )).first() if row.is_identity else None
 
             colobj = self._get_column_info(
                 row.column_name,
                 row.data_type,
                 row.is_nullable,
                 row.column_default,
                 row.is_identity,
@@ -309,15 +313,15 @@
 
         query = "SELECT constraint_id, constraint_name, column_name FROM v_catalog.constraint_columns \n\
                  WHERE table_name = '" + table_name + "'"
         if schema is not None:
              query += " AND table_schema = '" + schema + "'"
         query += " AND constraint_type = 'u'"
 
-        rs = connection.execute(query)
+        rs = connection.execute(text(query))
 
         unique_names = {row[1] for row in rs}
 
         result_dict = {unique: [] for unique in unique_names}
         for row in rs:
             result_dict[row[1]].append(row[2])
 
@@ -353,15 +357,15 @@
         """.format(table_name=table_name, schema_clause=(
             "" if schema is None else "AND i.table_schema ='{schema}'".format(schema=schema)))
 
         return [
             {
                 'name': name,
                 'sqltext': src[1:-1]
-            } for name, src in connection.execute(query).fetchall()
+            } for name, src in connection.execute(text(query)).fetchall()
         ]
 
     # constraints are enforced on selects, but returning nothing for these
     # methods allows table introspection to work
 
     @reflection.cache
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
@@ -369,15 +373,15 @@
                  WHERE constraint_type = 'p' AND table_name = '" + table_name + "'"
 
         if schema is not None:
             query += " AND table_schema = '" + schema + "' \n"
 
         cols = set()
         name = None
-        for row in connection.execute(query):
+        for row in connection.execute(text(query)):
              name = row[1] if name is None else name
              cols.add(row[2])
 
         return {"constrained_columns": list(cols), "name": name}
 
 
     def get_foreign_keys(self, connection, table_name, schema, **kw):
```

### Comparing `sqlalchemy-vertica-python-0.5.9/sqlalchemy_vertica_python.egg-info/PKG-INFO` & `sqlalchemy-vertica-python-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.2
 Name: sqlalchemy-vertica-python
-Version: 0.5.9
+Version: 0.6.3
 Summary: Vertica dialect for sqlalchemy using vertica_python
 Home-page: https://github.com/bluelabsio/sqlalchemy-vertica-python
 Author: James Casbon, Luke Emery-Fertitta
 Maintainer: Vince Broz
 Maintainer-email: opensource@bluelabs.com
 License: MIT
-Download-URL: https://github.com/bluelabsio/sqlalchemy-vertica-python/tarball/0.5.9
+Download-URL: https://github.com/bluelabsio/sqlalchemy-vertica-python/tarball/0.6.3
 Description: sqlalchemy-vertica-python
         =========================
         
         Vertica dialect for sqlalchemy. Forked from the `Vertica ODBC dialect <https://pypi.python.org/pypi/vertica-sqlalchemy>`_, written by `James Casbon <https://github.com/jamescasbon>`_.
         
         This module implements a Vertica dialect for SQLAlchemy using the pure-Python DB-API driver `vertica-python <https://github.com/vertica/vertica-python>`_, as adapted by `Luke Emery-Fertitta <https://github.com/lemeryfertitta>`_.
```

### Comparing `sqlalchemy-vertica-python-0.5.9/README.rst` & `sqlalchemy-vertica-python-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy-vertica-python-0.5.9/PKG-INFO` & `sqlalchemy-vertica-python-0.6.3/sqlalchemy_vertica_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.2
 Name: sqlalchemy-vertica-python
-Version: 0.5.9
+Version: 0.6.3
 Summary: Vertica dialect for sqlalchemy using vertica_python
 Home-page: https://github.com/bluelabsio/sqlalchemy-vertica-python
 Author: James Casbon, Luke Emery-Fertitta
 Maintainer: Vince Broz
 Maintainer-email: opensource@bluelabs.com
 License: MIT
-Download-URL: https://github.com/bluelabsio/sqlalchemy-vertica-python/tarball/0.5.9
+Download-URL: https://github.com/bluelabsio/sqlalchemy-vertica-python/tarball/0.6.3
 Description: sqlalchemy-vertica-python
         =========================
         
         Vertica dialect for sqlalchemy. Forked from the `Vertica ODBC dialect <https://pypi.python.org/pypi/vertica-sqlalchemy>`_, written by `James Casbon <https://github.com/jamescasbon>`_.
         
         This module implements a Vertica dialect for SQLAlchemy using the pure-Python DB-API driver `vertica-python <https://github.com/vertica/vertica-python>`_, as adapted by `Luke Emery-Fertitta <https://github.com/lemeryfertitta>`_.
```

