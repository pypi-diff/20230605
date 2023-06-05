# Comparing `tmp/django-fakery-4.1.0.tar.gz` & `tmp/django-fakery-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-fakery-4.1.0.tar", last modified: Mon Mar  6 18:02:02 2023, max compression
+gzip compressed data, was "dist/django-fakery-4.1.1.tar", last modified: Mon Jun  5 15:12:19 2023, max compression
```

## Comparing `django-fakery-4.1.0.tar` & `django-fakery-4.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-03-06 18:02:02.367709 django-fakery-4.1.0/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     1080 2019-10-15 17:28:35.000000 django-fakery-4.1.0/LICENSE
--rw-r--r--   0 flavio.curella   (502) staff       (20)       74 2019-10-15 17:28:35.000000 django-fakery-4.1.0/MANIFEST.in
--rw-r--r--   0 flavio.curella   (502) staff       (20)    13007 2023-03-06 18:02:02.367884 django-fakery-4.1.0/PKG-INFO
--rw-r--r--   0 flavio.curella   (502) staff       (20)    12245 2023-03-06 17:54:50.000000 django-fakery-4.1.0/README.rst
--rw-r--r--   0 flavio.curella   (502) staff       (20)        6 2023-03-06 18:01:52.000000 django-fakery-4.1.0/VERSION
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-03-06 18:02:02.364876 django-fakery-4.1.0/django_fakery/
--rw-r--r--   0 flavio.curella   (502) staff       (20)      307 2023-03-06 18:01:52.000000 django-fakery-4.1.0/django_fakery/__init__.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)     4698 2019-10-20 19:27:11.000000 django-fakery-4.1.0/django_fakery/blueprint.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)      560 2021-07-13 15:17:35.000000 django-fakery-4.1.0/django_fakery/compat.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)       43 2019-10-15 17:28:35.000000 django-fakery-4.1.0/django_fakery/exceptions.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)    18601 2023-03-06 17:21:34.000000 django-fakery-4.1.0/django_fakery/faker_factory.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)     4781 2023-03-06 17:21:23.000000 django-fakery-4.1.0/django_fakery/fakes.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)     6792 2023-03-06 17:21:23.000000 django-fakery-4.1.0/django_fakery/field_mappings.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)      250 2019-10-15 17:28:35.000000 django-fakery-4.1.0/django_fakery/lazy.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)      214 2023-03-06 17:51:49.000000 django-fakery-4.1.0/django_fakery/plugin.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2020-04-09 14:10:00.000000 django-fakery-4.1.0/django_fakery/py.typed
--rw-r--r--   0 flavio.curella   (502) staff       (20)       18 2019-10-15 17:28:35.000000 django-fakery-4.1.0/django_fakery/rels.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3013 2019-10-15 17:28:35.000000 django-fakery-4.1.0/django_fakery/shortcuts.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)      439 2021-07-12 17:14:21.000000 django-fakery-4.1.0/django_fakery/types.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)      957 2019-10-15 17:28:35.000000 django-fakery-4.1.0/django_fakery/utils.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)     2155 2023-03-06 17:21:23.000000 django-fakery-4.1.0/django_fakery/values.py
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-03-06 18:02:02.367407 django-fakery-4.1.0/django_fakery.egg-info/
--rw-r--r--   0 flavio.curella   (502) staff       (20)    13007 2023-03-06 18:02:01.000000 django-fakery-4.1.0/django_fakery.egg-info/PKG-INFO
--rw-r--r--   0 flavio.curella   (502) staff       (20)      660 2023-03-06 18:02:02.000000 django-fakery-4.1.0/django_fakery.egg-info/SOURCES.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2023-03-06 18:02:01.000000 django-fakery-4.1.0/django_fakery.egg-info/dependency_links.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       48 2023-03-06 18:02:01.000000 django-fakery-4.1.0/django_fakery.egg-info/entry_points.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       42 2023-03-06 18:02:02.000000 django-fakery-4.1.0/django_fakery.egg-info/requires.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       14 2023-03-06 18:02:02.000000 django-fakery-4.1.0/django_fakery.egg-info/top_level.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)      102 2023-03-06 18:02:02.368546 django-fakery-4.1.0/setup.cfg
--rw-r--r--   0 flavio.curella   (502) staff       (20)     1445 2023-03-06 17:49:37.000000 django-fakery-4.1.0/setup.py
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-06-05 15:12:19.000000 django-fakery-4.1.1/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     1080 2019-10-15 17:28:35.000000 django-fakery-4.1.1/LICENSE
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       74 2019-10-15 17:28:35.000000 django-fakery-4.1.1/MANIFEST.in
+-rw-r--r--   0 flavio.curella   (502) staff       (20)    16940 2023-06-05 15:12:19.000000 django-fakery-4.1.1/PKG-INFO
+-rw-r--r--   0 flavio.curella   (502) staff       (20)    12245 2023-03-06 17:54:50.000000 django-fakery-4.1.1/README.rst
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        6 2023-06-05 15:12:01.000000 django-fakery-4.1.1/VERSION
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-06-05 15:12:19.000000 django-fakery-4.1.1/django_fakery/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      307 2023-06-05 15:12:01.000000 django-fakery-4.1.1/django_fakery/__init__.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     4952 2023-06-05 15:11:52.000000 django-fakery-4.1.1/django_fakery/blueprint.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      560 2021-07-13 15:17:35.000000 django-fakery-4.1.1/django_fakery/compat.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       43 2019-10-15 17:28:35.000000 django-fakery-4.1.1/django_fakery/exceptions.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)    18700 2023-06-05 15:11:52.000000 django-fakery-4.1.1/django_fakery/faker_factory.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     4781 2023-03-06 17:21:23.000000 django-fakery-4.1.1/django_fakery/fakes.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     6784 2023-06-05 15:11:52.000000 django-fakery-4.1.1/django_fakery/field_mappings.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      213 2023-06-05 15:11:52.000000 django-fakery-4.1.1/django_fakery/lazy.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      214 2023-03-06 17:51:49.000000 django-fakery-4.1.1/django_fakery/plugin.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2020-04-09 14:10:00.000000 django-fakery-4.1.1/django_fakery/py.typed
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       18 2019-10-15 17:28:35.000000 django-fakery-4.1.1/django_fakery/rels.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     2954 2023-06-05 15:11:52.000000 django-fakery-4.1.1/django_fakery/shortcuts.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      439 2021-07-12 17:14:21.000000 django-fakery-4.1.1/django_fakery/types.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     1033 2023-06-05 15:11:52.000000 django-fakery-4.1.1/django_fakery/utils.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     2155 2023-03-06 17:21:23.000000 django-fakery-4.1.1/django_fakery/values.py
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-06-05 15:12:19.000000 django-fakery-4.1.1/django_fakery.egg-info/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)    16940 2023-06-05 15:12:19.000000 django-fakery-4.1.1/django_fakery.egg-info/PKG-INFO
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      660 2023-06-05 15:12:19.000000 django-fakery-4.1.1/django_fakery.egg-info/SOURCES.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2023-06-05 15:12:19.000000 django-fakery-4.1.1/django_fakery.egg-info/dependency_links.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       49 2023-06-05 15:12:19.000000 django-fakery-4.1.1/django_fakery.egg-info/entry_points.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       42 2023-06-05 15:12:19.000000 django-fakery-4.1.1/django_fakery.egg-info/requires.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       14 2023-06-05 15:12:19.000000 django-fakery-4.1.1/django_fakery.egg-info/top_level.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      102 2023-06-05 15:12:19.000000 django-fakery-4.1.1/setup.cfg
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     1445 2023-03-06 17:49:37.000000 django-fakery-4.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django-fakery-4.1.0/LICENSE` & `django-fakery-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-fakery-4.1.0/PKG-INFO` & `django-fakery-4.1.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: django-fakery
-Version: 4.1.0
-Summary: A model instances generator for Django
-Home-page: https://github.com/fcurella/django-fakery/
-Author: Flavio Curella
-Author-email: flavio.curella@gmail.com
-License: MIT
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-License-File: LICENSE
-
 Django-fakery
 =============
 
 .. image:: https://badge.fury.io/py/django-fakery.svg
     :target: https://badge.fury.io/py/django-fakery
 
 .. image:: https://travis-ci.org/fcurella/django-fakery.svg?branch=master
@@ -509,9 +487,7 @@
 
 .. _model_mommy: https://github.com/vandersonmota/model_mommy
 
 License
 -------
 
 This software is released under the MIT License.
-
-
```

### Comparing `django-fakery-4.1.0/django_fakery/blueprint.py` & `django-fakery-4.1.1/django_fakery/blueprint.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,42 +3,51 @@
 from typing import Optional as Opt
 from typing import overload
 
 from .types import Built, FieldMap, SaveHooks, Seed, T
 
 
 class Blueprint(Generic[T]):
-    def __init__(self, model, fields=None, pre_save=None, post_save=None, seed=None):
-        # type: (T, Opt[FieldMap], Opt[SaveHooks], Opt[SaveHooks], Opt[Seed]) -> None
+    def __init__(
+        self,
+        model: T,
+        fields: Opt[FieldMap] = None,
+        pre_save: Opt[SaveHooks] = None,
+        post_save: Opt[SaveHooks] = None,
+        seed: Opt[Seed] = None,
+    ):
         from .faker_factory import factory
 
         self.factory = factory
 
         self._model = model
         self._fields = fields or {}
         self.seed = seed
         self.pre_save = pre_save
         self.post_save = post_save
 
         self.pk = -1
 
-    def fields(self, **kwargs):
-        # type: (**Any) -> "Blueprint"
+    def fields(self, **kwargs) -> "Blueprint":
         return Blueprint(
             model=self._model,
             fields=dict(self._fields, **kwargs),
             pre_save=self.pre_save,
             post_save=self.post_save,
             seed=self.seed,
         )
 
     def make_one(
-        self, fields=None, pre_save=None, post_save=None, seed=None, iteration=None
-    ):
-        # type: (Opt[FieldMap], Opt[SaveHooks], Opt[SaveHooks], Opt[Seed], Opt[int]) -> T
+        self,
+        fields: Opt[FieldMap] = None,
+        pre_save: Opt[SaveHooks] = None,
+        post_save: Opt[SaveHooks] = None,
+        seed: Opt[Seed] = None,
+        iteration: Opt[int] = None,
+    ) -> T:
         _fields = self._fields.copy()
         if fields:
             _fields.update(fields)
         if seed is None:
             seed = self.seed
 
         if pre_save is None:
@@ -48,21 +57,33 @@
             post_save = self.post_save
 
         return self.factory.make_one(
             self._model, _fields, pre_save, post_save, seed, iteration
         )
 
     @overload
-    def make(self, fields, pre_save, post_save, seed, quantity):  # pragma: no cover
-        # type: (Opt[FieldMap], Opt[SaveHooks], Opt[SaveHooks], Opt[Seed], None) -> T
+    def make(
+        self,
+        fields: Opt[FieldMap],
+        pre_save: Opt[SaveHooks],
+        post_save: Opt[SaveHooks],
+        seed: Opt[Seed],
+        quantity: None,
+    ) -> T:  # pragma: no cover
         pass
 
     @overload
-    def make(self, fields, pre_save, post_save, seed, quantity):  # pragma: no cover
-        # type: (Opt[FieldMap], Opt[SaveHooks], Opt[SaveHooks], Opt[Seed], int) -> List[T]
+    def make(
+        self,
+        fields: Opt[FieldMap],
+        pre_save: Opt[SaveHooks],
+        post_save: Opt[SaveHooks],
+        seed: Opt[Seed],
+        quantity: int,
+    ) -> List[T]:  # pragma: no cover
         pass
 
     def make(
         self, fields=None, pre_save=None, post_save=None, seed=None, quantity=None
     ):
         _fields = self._fields.copy()
         if fields:
@@ -77,21 +98,33 @@
             post_save = self.post_save
 
         return self.factory.make(
             self._model, _fields, pre_save, post_save, seed, quantity
         )
 
     @overload
-    def build(self, fields, pre_save, seed, quantity, make_fks):  # pragma: no cover
-        # type: (Opt[FieldMap], Opt[SaveHooks], Opt[Seed], None, bool) -> Built
+    def build(
+        self,
+        fields: Opt[FieldMap],
+        pre_save: Opt[SaveHooks],
+        seed: Opt[Seed],
+        quantity: None,
+        make_fks: bool,
+    ) -> Built:  # pragma: no cover
         pass
 
     @overload
-    def build(self, fields, pre_save, seed, quantity, make_fks):  # pragma: no cover
-        # type: (Opt[FieldMap], Opt[SaveHooks], Opt[Seed], int, bool) -> List[Built]
+    def build(
+        self,
+        fields: Opt[FieldMap],
+        pre_save: Opt[SaveHooks],
+        seed: Opt[Seed],
+        quantity: int,
+        make_fks: bool,
+    ) -> List[Built]:  # pragma: no cover
         pass
 
     def build(
         self, fields=None, pre_save=None, seed=None, quantity=None, make_fks=False
     ):
         _fields = self._fields.copy()
         if fields:
@@ -103,21 +136,31 @@
             pre_save = self.pre_save
 
         return self.factory.build(
             self._model, _fields, pre_save, seed, quantity, make_fks
         )
 
     @overload
-    def m(self, pre_save, post_save, seed, quantity):  # pragma: no cover
-        # type: (Opt[SaveHooks], Opt[SaveHooks], Opt[Seed], None) -> Callable[..., T]
+    def m(
+        self,
+        pre_save: Opt[SaveHooks],
+        post_save: Opt[SaveHooks],
+        seed: Opt[Seed],
+        quantity: None,
+    ) -> Callable[..., T]:  # pragma: no cover
         pass
 
     @overload
-    def m(self, pre_save, post_save, seed, quantity):  # pragma: no cover
-        # type: (Opt[SaveHooks], Opt[SaveHooks], Opt[Seed], int) -> Callable[..., List[T]]
+    def m(
+        self,
+        pre_save: Opt[SaveHooks],
+        post_save: Opt[SaveHooks],
+        seed: Opt[Seed],
+        quantity: int,
+    ) -> Callable[..., List[T]]:  # pragma: no cover
         pass
 
     def m(self, pre_save=None, post_save=None, seed=None, quantity=None):
         make = partial(
             self.make,
             pre_save=pre_save,
             post_save=post_save,
@@ -127,21 +170,23 @@
 
         def fn(**kwargs):
             return make(fields=kwargs)
 
         return fn
 
     @overload
-    def b(self, pre_save, seed, quantity, make_fks):  # pragma: no cover
-        # type: (Opt[SaveHooks], Opt[Seed], None, bool) -> Callable[..., Built]
+    def b(
+        self, pre_save: Opt[SaveHooks], seed: Opt[Seed], quantity: None, make_fks: bool
+    ) -> Callable[..., Built]:  # pragma: no cover
         pass
 
     @overload
-    def b(self, pre_save, seed, quantity, make_fks):  # pragma: no cover
-        # type: (Opt[SaveHooks], Opt[Seed], int, bool) -> Callable[..., List[Built]]
+    def b(
+        self, pre_save: Opt[SaveHooks], seed: Opt[Seed], quantity: int, make_fks: bool
+    ) -> Callable[..., List[Built]]:  # pragma: no cover
         pass
 
     def b(self, pre_save=None, seed=None, quantity=None, make_fks=False):
         build = partial(
             self.build,
             pre_save=pre_save,
             seed=seed,
```

### Comparing `django-fakery-4.1.0/django_fakery/compat.py` & `django-fakery-4.1.1/django_fakery/compat.py`

 * *Files identical despite different names*

### Comparing `django-fakery-4.1.0/django_fakery/fakes.py` & `django-fakery-4.1.1/django_fakery/fakes.py`

 * *Files identical despite different names*

### Comparing `django-fakery-4.1.0/django_fakery/field_mappings.py` & `django-fakery-4.1.1/django_fakery/field_mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     "Store items in the order the keys were last added"
 
     def add(self, key, value):
         super().__setitem__(key, value)
         self.move_to_end(key, last=False)
 
 
-STRING_FIELDS = (
+STRING_FIELDS: Tuple[Any, ...] = (
     models.CharField,
     models.TextField,
-)  # type: Tuple[Any, ...]
+)
 
 if HAS_PSYCOPG2:
     from django.contrib.postgres import fields as pg_fields
 
     STRING_FIELDS += (pg_fields.CICharField, pg_fields.CITextField)
 """
 This module maps fields to functions generating values.
```

### Comparing `django-fakery-4.1.0/django_fakery/shortcuts.py` & `django-fakery-4.1.1/django_fakery/shortcuts.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 from django.utils import timezone
 
 from faker import Faker
 
 ParsableDate = Union[str, int, datetime, timedelta]
 
 
-def get_timezone():
-    # type: () -> Optional[tzinfo]
+def get_timezone() -> Optional[tzinfo]:
     return timezone.get_current_timezone() if settings.USE_TZ else None
 
 
-def future_datetime(end="+30d"):
-    # type: (ParsableDate) -> Callable[[int, Faker], datetime]
+def future_datetime(end: ParsableDate = "+30d") -> Callable[[int, Faker], datetime]:
     """
     Returns a ``datetime`` object in the future (that is, 1 second from now) up
     to the specified ``end``. ``end`` can be a string, another datetime, or a
     timedelta. If it's a string, it must start with `+`, followed by and integer
     and a unit, Eg: ``'+30d'``. Defaults to `'+30d'`
 
     Valid units are:
@@ -29,16 +27,15 @@
     * ``'hours'``, ``'hours'``
     * ``'minutes'``, ``'m'``
     * ``'seconds'``, ``'s'``
     """
     return lambda n, f: f.future_datetime(end_date=end, tzinfo=get_timezone())
 
 
-def future_date(end="+30d"):
-    # type: (ParsableDate) -> Callable[[int, Faker], date]
+def future_date(end: ParsableDate = "+30d") -> Callable[[int, Faker], date]:
     """
     Returns a ``date`` object in the future (that is, 1 day from now) up to
     the specified ``end``. ``end`` can be a string, another date, or a
     timedelta. If it's a string, it must start with `+`, followed by and integer
     and a unit, Eg: ``'+30d'``. Defaults to `'+30d'`
 
     Valid units are:
@@ -48,16 +45,15 @@
     * ``'hours'``, ``'hours'``
     * ``'minutes'``, ``'m'``
     * ``'seconds'``, ``'s'``
     """
     return lambda n, f: f.future_date(end_date=end, tzinfo=get_timezone())
 
 
-def past_datetime(start="-30d"):
-    # type: (ParsableDate) -> Callable[[int, Faker], datetime]
+def past_datetime(start: ParsableDate = "-30d") -> Callable[[int, Faker], datetime]:
     """
     Returns a ``datetime`` object in the past between 1 second ago and the
     specified ``start``. ``start`` can be a string, another datetime, or a
     timedelta. If it's a string, it must start with `-`, followed by and integer
     and a unit, Eg: ``'-30d'``. Defaults to `'-30d'`
 
     Valid units are:
@@ -67,16 +63,15 @@
     * ``'hours'``, ``'h'``
     * ``'minutes'``, ``'m'``
     * ``'seconds'``, ``'s'``
     """
     return lambda n, f: f.past_datetime(start_date=start, tzinfo=get_timezone())
 
 
-def past_date(start="-30d"):
-    # type: (ParsableDate) -> Callable[[int, Faker], date]
+def past_date(start: ParsableDate = "-30d") -> Callable[[int, Faker], date]:
     """
     Returns a ``date`` object in the past between 1 day ago and the
     specified ``start``. ``start`` can be a string, another date, or a
     timedelta. If it's a string, it must start with `-`, followed by and integer
     and a unit, Eg: ``'-30d'``. Defaults to `'-30d'`
 
     Valid units are:
```

### Comparing `django-fakery-4.1.0/django_fakery/utils.py` & `django-fakery-4.1.1/django_fakery/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,46 @@
-from typing import overload
+from typing import Any, List, Type, overload
 
 from django.apps import apps
 from django.db import models
 
 from six import string_types
 
 from .types import T
 
 
-def language_to_locale(language):
+def language_to_locale(language: str) -> str:
     """
     Converts django's `LANGUAGE_CODE` settings to a proper locale code.
     """
     tokens = language.split("-")
     if len(tokens) == 1:
         return tokens[0]
     return "%s_%s" % (tokens[0], tokens[1].upper())
 
 
 @overload
-def get_model(model):
-    # type: (str) -> models.Model
+def get_model(model: str) -> models.Model:
     pass
 
 
 @overload
-def get_model(model):
-    # type: (T) -> T
+def get_model(model: T) -> T:
     pass
 
 
 def get_model(model):
     if isinstance(model, string_types):
         model = apps.get_model(*model.split("."))
     return model
 
 
-def get_model_fields(model):
+def get_model_fields(model: Type[models.Model]) -> List[models.fields.Field]:
     fields = list(model._meta._forward_fields_map.items())
     for m2m in model._meta.many_to_many:
         fields.append((m2m.name, m2m))
     return fields
 
 
-def set_related(instance, attr, value):
+def set_related(instance: models.Model, attr: str, value: Any):
     field = getattr(instance, attr)
     field.set(value)
```

### Comparing `django-fakery-4.1.0/django_fakery/values.py` & `django-fakery-4.1.1/django_fakery/values.py`

 * *Files identical despite different names*

### Comparing `django-fakery-4.1.0/django_fakery.egg-info/SOURCES.txt` & `django-fakery-4.1.1/django_fakery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-fakery-4.1.0/setup.py` & `django-fakery-4.1.1/setup.py`

 * *Files identical despite different names*

