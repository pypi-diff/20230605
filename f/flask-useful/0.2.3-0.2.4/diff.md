# Comparing `tmp/flask-useful-0.2.3.tar.gz` & `tmp/flask-useful-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-useful-0.2.3.tar", last modified: Sun May 21 14:25:21 2023, max compression
+gzip compressed data, was "flask-useful-0.2.4.tar", last modified: Mon Jun  5 19:07:46 2023, max compression
```

## Comparing `flask-useful-0.2.3.tar` & `flask-useful-0.2.4.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.333459 flask-useful-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.329459 flask-useful-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.329459 flask-useful-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-21 14:25:09.000000 flask-useful-0.2.3/.github/workflows/publish-stable.yml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-21 14:25:09.000000 flask-useful-0.2.3/.github/workflows/publish-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-21 14:25:09.000000 flask-useful-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-21 14:25:09.000000 flask-useful-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-21 14:25:21.333459 flask-useful-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 14:25:09.000000 flask-useful-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.329459 flask-useful-0.2.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-21 14:25:09.000000 flask-useful-0.2.3/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.329459 flask-useful-0.2.3/examples/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-21 14:25:09.000000 flask-useful-0.2.3/examples/blueprints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.329459 flask-useful-0.2.3/examples/blueprints/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:25:09.000000 flask-useful-0.2.3/examples/blueprints/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.329459 flask-useful-0.2.3/examples/blueprints/routes/api/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-21 14:25:09.000000 flask-useful-0.2.3/examples/blueprints/routes/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.329459 flask-useful-0.2.3/examples/blueprints/routes/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-21 14:25:09.000000 flask-useful-0.2.3/examples/blueprints/routes/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-21 14:25:09.000000 flask-useful-0.2.3/examples/blueprints/routes/api/v1/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.329459 flask-useful-0.2.3/examples/blueprints/routes/api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-21 14:25:09.000000 flask-useful-0.2.3/examples/blueprints/routes/api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-21 14:25:09.000000 flask-useful-0.2.3/examples/blueprints/routes/api/v2/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-21 14:25:09.000000 flask-useful-0.2.3/examples/blueprints/routes/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-21 14:25:09.000000 flask-useful-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 14:25:21.333459 flask-useful-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.329459 flask-useful-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.329459 flask-useful-0.2.3/src/flask_useful/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/flask_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/sqla.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.333459 flask-useful-0.2.3/src/flask_useful/wtforms/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/wtforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/wtforms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/wtforms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/wtforms/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-21 14:25:09.000000 flask-useful-0.2.3/src/flask_useful/wtforms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:25:21.333459 flask-useful-0.2.3/src/flask_useful.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-21 14:25:21.000000 flask-useful-0.2.3/src/flask_useful.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-21 14:25:21.000000 flask-useful-0.2.3/src/flask_useful.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:25:21.000000 flask-useful-0.2.3/src/flask_useful.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-21 14:25:21.000000 flask-useful-0.2.3/src/flask_useful.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 14:25:21.000000 flask-useful-0.2.3/src/flask_useful.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.413021 flask-useful-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.405021 flask-useful-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-05 19:07:30.000000 flask-useful-0.2.4/.github/workflows/publish-stable.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-05 19:07:30.000000 flask-useful-0.2.4/.github/workflows/publish-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 19:07:30.000000 flask-useful-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-05 19:07:30.000000 flask-useful-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-05 19:07:46.413021 flask-useful-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-05 19:07:30.000000 flask-useful-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/blueprints/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/blueprints/routes/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/blueprints/routes/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/api/v1/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/examples/blueprints/routes/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/api/v2/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 19:07:30.000000 flask-useful-0.2.4/examples/blueprints/routes/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-05 19:07:30.000000 flask-useful-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 19:07:46.413021 flask-useful-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.405021 flask-useful-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.409021 flask-useful-0.2.4/src/flask_useful/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/flask_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.413021 flask-useful-0.2.4/src/flask_useful/sqla/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/sqla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/sqla/ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/sqla/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/sqla/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.413021 flask-useful-0.2.4/src/flask_useful/wtforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/wtforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/wtforms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/wtforms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/wtforms/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-05 19:07:30.000000 flask-useful-0.2.4/src/flask_useful/wtforms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:07:46.413021 flask-useful-0.2.4/src/flask_useful.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-05 19:07:46.000000 flask-useful-0.2.4/src/flask_useful.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-05 19:07:46.000000 flask-useful-0.2.4/src/flask_useful.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:07:46.000000 flask-useful-0.2.4/src/flask_useful.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 19:07:46.000000 flask-useful-0.2.4/src/flask_useful.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 19:07:46.000000 flask-useful-0.2.4/src/flask_useful.egg-info/top_level.txt
```

### Comparing `flask-useful-0.2.3/.github/workflows/publish-stable.yml` & `flask-useful-0.2.4/.github/workflows/publish-stable.yml`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/.github/workflows/publish-test.yml` & `flask-useful-0.2.4/.github/workflows/publish-test.yml`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/LICENSE` & `flask-useful-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/pyproject.toml` & `flask-useful-0.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -40,7 +40,8 @@
 local_scheme = "no-local-version"
 fallback_version = "0.0.0"
 
 [tool.mypy]
 files = ["src/flask_useful"]
 python_version = "3.7"
 strict = true
+disallow_subclassing_any = false
```

### Comparing `flask-useful-0.2.3/src/flask_useful/app.py` & `flask-useful-0.2.4/src/flask_useful/app.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/src/flask_useful/decorators.py` & `flask-useful-0.2.4/src/flask_useful/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/src/flask_useful/flask_access.py` & `flask-useful-0.2.4/src/flask_useful/flask_access.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/src/flask_useful/mail.py` & `flask-useful-0.2.4/src/flask_useful/mail.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/src/flask_useful/sqla.py` & `flask-useful-0.2.4/src/flask_useful/sqla/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 from __future__ import annotations
 import typing as t
 import re
 
-from flask import current_app
 import sqlalchemy as sa
-from sqlalchemy.orm import Session
-from werkzeug.local import LocalProxy
+
+from .session import sqla_session
+
+if t.TYPE_CHECKING:
+    from sqlalchemy import Column
+    from sqlalchemy.orm import Session
 
 
 IdentityArgument = t.Union[t.Any, t.Tuple[t.Any, ...], t.Dict[str, t.Any]]
 
 
 __all__ = (
     'generate_slug',
-    'get_sqla_session',
+    'get_primary_columns',
     'normalize_pk',
-    'sqla_session',
-)
-
-
-sqla_session = t.cast(
-    Session,
-    LocalProxy(lambda: get_sqla_session()),
 )
 
 
 def generate_slug(
     slug_field: t.Any,
     slug: str,
     session: t.Optional[Session] = None,
@@ -35,58 +31,52 @@
 
     Arguments:
         slug_field: Model attribute containing slug.
         slug (str): The desired slug value.
         session (Session): SQLAlchemy session.
     """
     if session is None:
-        session = get_sqla_session()
+        session = sqla_session
 
     pattern = r'^%s(?:-([0-9]+))?$' % slug
 
     stmt = (
         sa.select(slug_field)
-            .where(slug_field.regexp_match(pattern))
-            .order_by(slug_field.desc())
-            .limit(1)
+          .where(slug_field.regexp_match(pattern))
+          .order_by(slug_field.desc())
+          .limit(1)
     )
     found = session.scalar(stmt)
 
     if not found:
         return slug
 
     match = re.match(pattern, found)
 
     if match is None:
         raise AssertionError('The query found one result for the regular expression.')
 
     return '{}-{}'.format(slug, int(match.group(1)) + 1)
 
 
-def get_sqla_session() -> Session:
-    """Returns the current session instance from application context."""
-    ext = current_app.extensions.get('sqlalchemy')
-
-    if ext is None:
-        raise RuntimeError(
-            'An extension named sqlalchemy was not found '
-            'in the list of registered extensions for the current application.'
-        )
-
-    return t.cast(Session, ext.db.session)
+def get_primary_columns(
+    model_class: t.Type[t.Any],
+) -> t.Tuple[Column[t.Any], ...]:
+    """Returns the primary key columns."""
+    return tuple(
+        c for c in sa.inspect(model_class).columns if c.primary_key
+    )
 
 
 def normalize_pk(
     value: IdentityArgument,
     model_class: t.Type[t.Any],
 ) -> t.Dict[str, t.Any]:
     """Returns the primary key with a cast as a dictionary."""
-    columns = tuple(
-        c for c in sa.inspect(model_class).columns if c.primary_key
-    )
+    columns = get_primary_columns(model_class)
 
     if not isinstance(value, tuple):
         if isinstance(value, dict):
             value = tuple(value[c.name] for c in columns)
         else:
             value = (value,)
```

### Comparing `flask-useful-0.2.3/src/flask_useful/utils.py` & `flask-useful-0.2.4/src/flask_useful/utils.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/src/flask_useful/views.py` & `flask-useful-0.2.4/src/flask_useful/views.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/src/flask_useful/wtforms/fields.py` & `flask-useful-0.2.4/src/flask_useful/wtforms/fields.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/src/flask_useful/wtforms/filters.py` & `flask-useful-0.2.4/src/flask_useful/wtforms/filters.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/src/flask_useful/wtforms/validators.py` & `flask-useful-0.2.4/src/flask_useful/wtforms/validators.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/src/flask_useful/wtforms/widgets.py` & `flask-useful-0.2.4/src/flask_useful/wtforms/widgets.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.3/src/flask_useful.egg-info/SOURCES.txt` & `flask-useful-0.2.4/src/flask_useful.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,24 +11,28 @@
 examples/blueprints/routes/api/__init__.py
 examples/blueprints/routes/api/v1/__init__.py
 examples/blueprints/routes/api/v1/users.py
 examples/blueprints/routes/api/v2/__init__.py
 examples/blueprints/routes/api/v2/users.py
 src/flask_useful/__init__.py
 src/flask_useful/app.py
+src/flask_useful/blueprints.py
 src/flask_useful/decorators.py
 src/flask_useful/flask_access.py
 src/flask_useful/mail.py
 src/flask_useful/py.typed
-src/flask_useful/sqla.py
 src/flask_useful/utils.py
 src/flask_useful/views.py
 src/flask_useful.egg-info/PKG-INFO
 src/flask_useful.egg-info/SOURCES.txt
 src/flask_useful.egg-info/dependency_links.txt
 src/flask_useful.egg-info/requires.txt
 src/flask_useful.egg-info/top_level.txt
+src/flask_useful/sqla/__init__.py
+src/flask_useful/sqla/ma.py
+src/flask_useful/sqla/session.py
+src/flask_useful/sqla/utils.py
 src/flask_useful/wtforms/__init__.py
 src/flask_useful/wtforms/fields.py
 src/flask_useful/wtforms/filters.py
 src/flask_useful/wtforms/validators.py
 src/flask_useful/wtforms/widgets.py
```

