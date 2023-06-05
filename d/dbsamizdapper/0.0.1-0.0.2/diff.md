# Comparing `tmp/dbsamizdapper-0.0.1.tar.gz` & `tmp/dbsamizdapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbsamizdapper-0.0.1.tar", max compression
+gzip compressed data, was "dbsamizdapper-0.0.2.tar", max compression
```

## Comparing `dbsamizdapper-0.0.1.tar` & `dbsamizdapper-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    32474 2023-05-30 02:58:12.099436 dbsamizdapper-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1151 2023-06-01 15:28:01.814706 dbsamizdapper-0.0.1/README.md
--rw-r--r--   0        0        0      338 2023-06-01 14:07:19.946281 dbsamizdapper-0.0.1/dbsamizdat/__init__.py
--rw-r--r--   0        0        0     1699 2023-06-01 10:50:44.871032 dbsamizdapper-0.0.1/dbsamizdat/api.py
--rw-r--r--   0        0        0     5128 2023-06-01 14:08:36.096856 dbsamizdapper-0.0.1/dbsamizdat/apps.py
--rw-r--r--   0        0        0     1721 2023-05-30 07:09:40.993026 dbsamizdapper-0.0.1/dbsamizdat/django_api.py
--rw-r--r--   0        0        0     2806 2023-06-01 08:44:33.114063 dbsamizdapper-0.0.1/dbsamizdat/exceptions.py
--rw-r--r--   0        0        0     2444 2023-06-01 14:08:36.084855 dbsamizdapper-0.0.1/dbsamizdat/graphvizdot.py
--rw-r--r--   0        0        0     6132 2023-06-01 14:08:34.308706 dbsamizdapper-0.0.1/dbsamizdat/libdb.py
--rw-r--r--   0        0        0     4566 2023-06-01 14:08:36.108857 dbsamizdapper-0.0.1/dbsamizdat/libgraph.py
--rw-r--r--   0        0        0     1658 2023-06-01 14:08:36.084855 dbsamizdapper-0.0.1/dbsamizdat/loader.py
--rw-r--r--   0        0        0      793 2023-06-01 14:08:34.252701 dbsamizdapper-0.0.1/dbsamizdat/management/commands/dbsamizdat.py
--rw-r--r--   0        0        0      110 2023-05-30 02:58:12.103435 dbsamizdapper-0.0.1/dbsamizdat/models.py
--rwxr-xr-x   0        0        0    15212 2023-06-01 15:06:10.617709 dbsamizdapper-0.0.1/dbsamizdat/runner.py
--rw-r--r--   0        0        0    11734 2023-06-01 14:08:36.080855 dbsamizdapper-0.0.1/dbsamizdat/samizdat.py
--rw-r--r--   0        0        0     5354 2023-06-01 14:08:34.324707 dbsamizdapper-0.0.1/dbsamizdat/samtypes.py
--rw-r--r--   0        0        0     2134 2023-06-01 08:57:46.104347 dbsamizdapper-0.0.1/dbsamizdat/util.py
--rw-r--r--   0        0        0     1141 2023-06-01 15:31:31.833331 dbsamizdapper-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 dbsamizdapper-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    32474 2023-05-30 02:58:12.099436 dbsamizdapper-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1444 2023-06-03 04:25:18.510688 dbsamizdapper-0.0.2/README.md
+-rw-r--r--   0        0        0      338 2023-06-01 14:07:19.946281 dbsamizdapper-0.0.2/dbsamizdat/__init__.py
+-rw-r--r--   0        0        0     1699 2023-06-01 10:50:44.871032 dbsamizdapper-0.0.2/dbsamizdat/api.py
+-rw-r--r--   0        0        0     5149 2023-06-04 23:42:59.233051 dbsamizdapper-0.0.2/dbsamizdat/apps.py
+-rw-r--r--   0        0        0     1721 2023-05-30 07:09:40.993026 dbsamizdapper-0.0.2/dbsamizdat/django_api.py
+-rw-r--r--   0        0        0     2806 2023-06-01 08:44:33.114063 dbsamizdapper-0.0.2/dbsamizdat/exceptions.py
+-rw-r--r--   0        0        0     2444 2023-06-01 14:08:36.084855 dbsamizdapper-0.0.2/dbsamizdat/graphvizdot.py
+-rw-r--r--   0        0        0     6132 2023-06-04 05:47:56.922760 dbsamizdapper-0.0.2/dbsamizdat/libdb.py
+-rw-r--r--   0        0        0     5145 2023-06-05 02:49:04.922968 dbsamizdapper-0.0.2/dbsamizdat/libgraph.py
+-rw-r--r--   0        0        0     1967 2023-06-05 02:37:16.301863 dbsamizdapper-0.0.2/dbsamizdat/loader.py
+-rw-r--r--   0        0        0      793 2023-06-01 14:08:34.252701 dbsamizdapper-0.0.2/dbsamizdat/management/commands/dbsamizdat.py
+-rw-r--r--   0        0        0      110 2023-05-30 02:58:12.103435 dbsamizdapper-0.0.2/dbsamizdat/models.py
+-rwxr-xr-x   0        0        0    15632 2023-06-05 06:28:11.969618 dbsamizdapper-0.0.2/dbsamizdat/runner.py
+-rw-r--r--   0        0        0    11175 2023-06-05 06:28:11.969618 dbsamizdapper-0.0.2/dbsamizdat/samizdat.py
+-rw-r--r--   0        0        0     7253 2023-06-05 06:28:11.969618 dbsamizdapper-0.0.2/dbsamizdat/samtypes.py
+-rw-r--r--   0        0        0      600 2023-06-05 02:38:39.907725 dbsamizdapper-0.0.2/dbsamizdat/util.py
+-rw-r--r--   0        0        0     1141 2023-06-05 07:24:03.420014 dbsamizdapper-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 dbsamizdapper-0.0.2/PKG-INFO
```

### Comparing `dbsamizdapper-0.0.1/LICENSE.txt` & `dbsamizdapper-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.1/README.md` & `dbsamizdapper-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -17,10 +17,25 @@
  - Opinionated code formatting
    - black + isort
    - replaced `lambda`s
  - some simple `pytest` functions
 
 and probably many more undocumented changes
 
+
+## Running Tests
+
+Spin up a docker container
+
+`docker run -p 5435:5432 -e POSTGRES_HOST_AUTH_METHOD=trust postgres:latest`
+
+The db url for this container would be:
+
+"postgresql:///postgres@localhost:5435/postgres"
+
+Make this the environment variable `DB_URL`, or add it to the `.env` file
+
 ## Original README
 
 Check out the original readme for rationale and how-to documentation
+
+
```

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/api.py` & `dbsamizdapper-0.0.2/dbsamizdat/api.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/apps.py` & `dbsamizdapper-0.0.2/dbsamizdat/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,20 @@
     RenameField,
     RenameModel,
     RunPython,
     RunSQL,
 )
 from django.db.models.signals import post_migrate, pre_migrate
 
+from dbsamizdat.samtypes import FQTuple
+
 from .libdb import dbstate_equals_definedstate
 from .libgraph import depsort_with_sidekicks, sanity_check, subtree_depends, unmanaged_refs
 from .loader import get_samizdats
 from .runner import ArgType, cmd_nuke, cmd_sync, get_cursor, txstyle
-from .util import fqify_node
 
 DBCONN = "default"  # Only migrations on the default DB connections are supported. For now.
 SMART_MIGRATIONS = getattr(settings, "DBSAMIZDAT_SMART_MIGRATIONS", False)  # Don't use with custom Operations!
 style = color_style()
 
 
 def get_cmd_args(**kwargs):
@@ -96,28 +97,28 @@
                     RenameField,
                     AlterField,
                     DeleteModel,
                     RenameModel,
                     AlterModelTable,
                 ),
             ):
-                tables_affected.add(fqify_node(model_meta.db_table))
+                tables_affected.add(FQTuple.fqify(model_meta.db_table))
     return (False, tables_affected)
 
 
 def premigrate_handler(sender, **kwargs):
     if not (kwargs.get("plan")) or (kwargs["using"] != DBCONN):
         return
 
     if not SMART_MIGRATIONS:
         # Make no effort to determine whether we can be selective in which state we'll remove.
         nuke(**kwargs)
         return
 
-    samizdats = depsort_with_sidekicks(sanity_check(get_samizdats()))
+    samizdats = list(depsort_with_sidekicks(sanity_check(get_samizdats())))
     db_compare = dbstate_equals_definedstate(get_django_cursor(), samizdats)
     if not db_compare.issame:
         # There's unsynced samizdat state, and we can't tell if
         # a) new state depends on the post-migrate state or the pre-migrate state
         # b) old state will get in the way of the migrations
         # (or both.) Therefor, we can't sync, but neither can we leave any stuff lying around.
         # Thus we'll have to nuke DB state.
```

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/django_api.py` & `dbsamizdapper-0.0.2/dbsamizdat/django_api.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/exceptions.py` & `dbsamizdapper-0.0.2/dbsamizdat/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/graphvizdot.py` & `dbsamizdapper-0.0.2/dbsamizdat/graphvizdot.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/libdb.py` & `dbsamizdapper-0.0.2/dbsamizdat/libdb.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/loader.py` & `dbsamizdapper-0.0.2/dbsamizdat/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import inspect
+from abc import ABC
 from importlib import import_module
 from importlib.util import find_spec
 from logging import getLogger
 from typing import Iterable
 
-from dbsamizdat.samizdat import Samizdat, SamizdatFunction, SamizdatMaterializedView, SamizdatTrigger, SamizdatView
+from dbsamizdat.samizdat import (
+    Samizdat,
+    SamizdatFunction,
+    SamizdatMaterializedView,
+    SamizdatTrigger,
+    SamizdatView,
+    SamizdatWithSidekicks,
+)
 from dbsamizdat.samtypes import ProtoSamizdat
 
 excludelist = {
     Samizdat,
+    SamizdatWithSidekicks,
     SamizdatFunction,
     SamizdatView,
     SamizdatMaterializedView,
     SamizdatTrigger,
+    ABC,
 }
 
 logger = getLogger(__name__)
 
 AUTOLOAD_MODULENAME = "dbsamizdat_defs"
 
 
@@ -25,15 +35,22 @@
     Returns all subclasses of "Samizdat"
     where they are not considered abstract
     """
 
     def all_subclasses(cls):
         return set(cls.__subclasses__()).union([s for c in cls.__subclasses__() for s in all_subclasses(c)])
 
-    return all_subclasses(Samizdat).difference(excludelist)
+    # Exclude double imports
+    heads = set()
+    unique = set()
+    for klass in all_subclasses(Samizdat).difference(excludelist):
+        if klass.head_id() not in heads:
+            unique.add(klass)
+            heads.add(klass.head_id())
+    return unique
 
 
 def samizdats_in_module(mod):
     """
     Returns the samizdat instances in a given module
     """
     for _, thing in inspect.getmembers(mod):
```

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/management/commands/dbsamizdat.py` & `dbsamizdapper-0.0.2/dbsamizdat/management/commands/dbsamizdat.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/runner.py` & `dbsamizdapper-0.0.2/dbsamizdat/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 from dbsamizdat.samizdat import Samizdat, SamizdatMaterializedView
 
 from .exceptions import DatabaseError, FunctionSignatureError, SamizdatException
 from .graphvizdot import dot
 from .libdb import dbinfo_to_class, dbstate_equals_definedstate, get_dbstate
 from .libgraph import depsort_with_sidekicks, node_dump, sanity_check, subtree_depends
-from .loader import get_samizdats, autodiscover_samizdats
-from .samtypes import Cursor, ProtoSamizdat, entitypes
-from .util import fqify_node, nodenamefmt, sqlfmt
+from .loader import autodiscover_samizdats, get_samizdats
+from .samtypes import Cursor, FQTuple, ProtoSamizdat, entitypes
+from .util import nodenamefmt, sqlfmt
 
 if typing.TYPE_CHECKING:
     from argparse import ArgumentParser
 
 dotenv.load_dotenv()
 
 
@@ -49,35 +49,47 @@
     dburl: str | None = os.environ.get("DBURL")
 
 
 def vprint(args: ArgType, *pargs, **pkwargs):
     if args.log_rather_than_print:
         logger.info(" ".join(map(str, pargs)))
     elif args.verbosity:
-        print(*pargs, **PRINTKWARGS, **pkwargs)
+        print(*pargs, **PRINTKWARGS, **pkwargs)  # type: ignore
 
 
 def timer() -> Generator[float, None, None]:
     """
     Generator to show time elapsed since the last iteration
     """
     last = monotonic()
     while True:
         cur = monotonic()
         yield (cur - last)
         last = cur
 
 
-def get_sds(in_django: bool = False):
-    if in_django:
-        sds = list(autodiscover_samizdats())
+def get_sds(in_django: bool = False, samizdats: Iterable[Samizdat] | None = None):
+    """
+    Samizdats may be defined by:
+     - A list
+     - "Autodiscovery"
+     - A Django module search
+    """
+    if samizdats:
+        sds = set(samizdats)
+    elif in_django:
+        sds = set(autodiscover_samizdats())
     else:
-        sds = get_samizdats()
+        sds = set(get_samizdats())
+
     sanity_check(sds)
-    return depsort_with_sidekicks(sds)
+    sorted_sds = list(depsort_with_sidekicks(sds))
+    sanity_check(sorted_sds)
+    return sorted_sds
+
 
 @contextmanager
 def get_cursor(args: ArgType) -> Generator[Cursor, None, None]:
     """
     Returns a psycopg or Django cursor
     """
 
@@ -126,15 +138,15 @@
 
 def cmd_refresh(args: ArgType):
     with get_cursor(args) as cursor:
         samizdats = get_sds(args.in_django)
         matviews: list[SamizdatMaterializedView] = [sd for sd in samizdats if sd.entity_type == entitypes.MATVIEW]
 
         if args.belownodes:
-            rootnodes = {fqify_node(rootnode) for rootnode in args.belownodes}
+            rootnodes = {FQTuple.fqify(rootnode) for rootnode in args.belownodes}
             allnodes = node_dump(samizdats)
             if rootnodes - allnodes:
                 raise ValueError(
                     """Unknown rootnodes:\n\t- %s"""
                     % "\n\t- ".join([nodenamefmt(rootnode) for rootnode in rootnodes - allnodes])
                 )
             subtree_bundle = subtree_depends(samizdats, rootnodes)
@@ -145,22 +157,25 @@
         def refreshes():
             for sd in matviews:
                 yield "refresh", sd, sd.refresh(concurrent_allowed=True)
 
         executor(refreshes(), args, cursor, max_namelen=max_namelen, timing=True)
 
 
-def cmd_sync(args: ArgType):
-    samizdats = get_sds(args.in_django)
+def cmd_sync(args: ArgType, samizdatsIn: list[Samizdat] | None = None):
+    samizdats = tuple(get_sds(False, samizdatsIn)) or tuple(get_sds(args.in_django))
 
     with get_cursor(args) as cursor:
         db_compare = dbstate_equals_definedstate(cursor, samizdats)
         if db_compare.issame:
             vprint(args, "No differences, nothing to do.")
             return
+
+        # Get the longest name from what's in the
+        # database and defined state
         max_namelen = max(len(str(ds)) for ds in db_compare.excess_dbstate | db_compare.excess_definedstate)
         if db_compare.excess_dbstate:
 
             def drops():
                 for sd in db_compare.excess_dbstate:
                     yield "drop", sd, sd.drop(if_exists=True)
                     # we don't know the deptree; so they may have vanished
@@ -280,18 +295,15 @@
                 end="",
             )
             vprint(args, f"\n\n{sqlfmt(sql)}\n\n")
 
     action_cnt = 0
     for ix, progress in enumerate(yielder):
         action_cnt += 1
-        try:
-            progressprint(ix, *progress)
-        except:
-            raise
+        progressprint(ix, *progress)
         action_totake, sd, sql = progress
         try:
             try:
                 cursor.execute("BEGIN;")  # harmless if already in a tx but raises a warning
                 cursor.execute(f"SAVEPOINT action_{action_totake};")
                 cursor.execute(sql)
             except Exception as ouch:
```

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/samizdat.py` & `dbsamizdapper-0.0.2/dbsamizdat/samizdat.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import typing
 from collections import Counter
 from hashlib import md5
 from json import dumps as jsondumps
 from string import Template
 from time import time as now
 
-from dbsamizdat.samtypes import FQTuple, HasFQ, HasRefreshTriggers, Mogrifier, ProtoSamizdat, entitypes
+from dbsamizdat.samtypes import FQTuple, HasRefreshTriggers, HasSidekicks, Mogrifier, ProtoSamizdat, entitypes
 
-from .util import db_object_identity, fqify_node, nodenamefmt
+from .util import nodenamefmt
 
 _DBINFO_VERSION = 1  # Version number for signature format. For future use
 
 TRIGGER_DEPCOUNTER_PADDED_WIDTH = 5
 
 
 class Samizdat(ProtoSamizdat):
@@ -22,61 +22,44 @@
     """
 
     entity_type: entitypes = entitypes.VIEW
     # This is populated when restoring the class info from the database
     implanted_hash: str | None = None
 
     @classmethod
-    def get_name(cls) -> str:
-        return cls.__name__
+    def db_object_identity(cls):
+        return cls.fq().db_object_identity()
 
     @classmethod
     def fq(cls):
         return FQTuple(schema=cls.schema, object_name=cls.get_name())
 
     def __str__(self):
         funcargs = getattr(self, "function_arguments_signature", None)
         node = (self.schema, self.get_name(), funcargs) if funcargs else (self.schema, self.get_name())
         return nodenamefmt(node)
 
     @classmethod
-    def db_object_identity(cls) -> str:
-        return db_object_identity(cls)
-
-    @classmethod
     def definition_hash(cls):
         """
         Return the "implanted" hash if preset or generate
         a new descriptive hash of this instance
         """
         if cls.implanted_hash:
             return cls.implanted_hash
 
         return md5("|".join([cls.sql_template, cls.db_object_identity()]).encode("utf-8")).hexdigest()
 
     @classmethod
-    def fqify(cls, ref: HasFQ):
-        if isinstance(ref, str):
-            return FQTuple(cls.schema or "public", ref)
-        elif hasattr(ref, "fq"):
-            # On most Samizdat classes, the `fq` classproperty is
-            # ("public", "name")
-            return ref.fq()
-        elif isinstance(ref, tuple):
-            # A dependency can also be specified as a 2tuple of schema, thing_name
-            return FQTuple(*ref)
-        raise TypeError
-
-    @classmethod
     def fqdeps_on(cls):
-        return {cls.fqify(dep) for dep in cls.deps_on}
+        return {FQTuple.fqify(dep) for dep in cls.deps_on}
 
     @classmethod
     def fqdeps_on_unmanaged(cls):
-        return {cls.fqify(dep) for dep in cls.deps_on_unmanaged}
+        return {FQTuple.fqify(dep) for dep in cls.deps_on_unmanaged}
 
     @classmethod
     def dbinfo(cls):
         """
         Returns descriptor (json) for this object, to be stored in the database
         """
         return jsondumps(
@@ -119,42 +102,33 @@
     def drop(cls, if_exists=False):
         """
         SQL to drop object. Cascade because we have no idea about the dependency tree.
         """
         return f"""DROP {cls.entity_type.value} {"IF EXISTS" if if_exists else ""} {cls.db_object_identity()} CASCADE;"""  # noqa: E501
 
     @classmethod
-    def and_sidekicks(cls):
-        """
-        On some classes, this will yield autogenerated sidekick classes
-        """
-        yield cls
-        yield from ()
-
-    @classmethod
     def head_id(cls):
         return hash((cls.schema, cls.get_name(), cls.entity_type.name, cls.definition_hash()))
 
 
 class SamizdatView(Samizdat):
     entity_type = entitypes.VIEW
 
 
 class SamizdatFunction(Samizdat):
     entity_type = entitypes.FUNCTION
     function_arguments_signature = ""
     autorefresher = False
+    function_name: str | None = None
     # this field serves to identify this node as autogenerated
     # through a materialized view with populated `refresh_triggers` attribute
 
     @classmethod
     def get_name(cls) -> str:
-        if fn_name := getattr(cls, "function_name", None):
-            return fn_name
-        return cls.__name__
+        return getattr(cls, "function_name") or cls.__name__
 
     @classmethod
     def fq(cls):
         return FQTuple(
             schema=cls.schema,
             object_name=cls.get_name(),
             args=cls.function_arguments_signature,
@@ -216,63 +190,71 @@
         (indirectly it is, through a table.)
         Yet trigger names do not need to be unique in a schema.
         Yet we need a unique identifier for them, within the dbsamizdat collection.
         So we use the table the trigger is attached to as a component
         in the fully qualified name.
         """
 
-        return FQTuple(schema=db_object_identity(cls.on_table), object_name=cls.get_name())
+        return FQTuple(schema=FQTuple.fqify(cls.on_table).db_object_identity(), object_name=cls.get_name())
 
     def __str__(self):
         return nodenamefmt(self.fq())
 
     @classmethod
     def fqdeps_on_unmanaged(cls):
-        return {fqify_node(n) for n in cls.deps_on_unmanaged | {cls.on_table}}
+        return {FQTuple.fqify(n) for n in cls.deps_on_unmanaged | {cls.on_table}}
 
     @classmethod
     def create(cls):
-        target_table = db_object_identity(cls.on_table)
+        target_table = FQTuple.fqify(cls.on_table).db_object_identity()
         subst = dict(
             preamble=f"""CREATE {cls.entity_type.value} "{cls.get_name()}" {cls.condition} ON {target_table}""",
             samizdatname=cls.get_name(),
         )
         return Template(cls.sql_template).safe_substitute(subst)
 
     @classmethod
     def drop(cls, if_exists=False):
-        ident = db_object_identity(cls.on_table)
+        ident = FQTuple.fqify(cls.on_table).db_object_identity()
         return (
             f"""DROP {cls.entity_type.value} {"IF EXISTS" if if_exists else ""} {cls.get_name()} ON {ident} CASCADE;"""
         )
 
     @classmethod
     def sign(cls, cursor: Mogrifier):
         comment = cursor.mogrify(
-            f"""COMMENT ON {cls.entity_type.value} "{cls.get_name()}" ON {db_object_identity(cls.on_table)} IS %s;""",
+            f"""COMMENT ON {cls.entity_type.value} "{cls.get_name()}" ON {FQTuple.fqify(cls.on_table).db_object_identity()} IS %s;""",
             (cls.dbinfo(),),
         )
         if isinstance(comment, bytes):
             return comment.decode()
         return comment
 
     @classmethod
     def head_id(cls):
         return hash(
             (
-                fqify_node(cls.on_table)[0],
+                FQTuple.fqify(cls.on_table).schema,
                 cls.get_name(),
                 cls.entity_type.name,
-                fqify_node(cls.on_table)[1],
+                FQTuple.fqify(cls.on_table).object_name,
                 cls.definition_hash(),
             )
         )
 
 
-class SamizdatMaterializedView(Samizdat, HasRefreshTriggers):
+class SamizdatWithSidekicks(Samizdat, HasSidekicks, HasRefreshTriggers):
+    """
+    This class is here for mypy detection of sidekicks function
+    """
+
+    pass
+
+
+class SamizdatMaterializedView(SamizdatWithSidekicks):
     entity_type = entitypes.MATVIEW
     refresh_concurrently = False
     refresh_triggers = set()
     AUTOREFRESHER_COUNTER = "autorefresher"
 
     @classmethod
     def refresh(cls, concurrent_allowed=True):
@@ -289,15 +271,15 @@
         """
         if cls.refresh_triggers:
             yield type(
                 f"{cls.get_name()}_refresh",
                 (SamizdatFunction,),
                 dict(
                     schema=cls.schema,
-                    deps_on={cls.fq()},
+                    deps_on={cls},
                     autorefresher=True,
                     sql_template="""
                         ${preamble}
                         RETURNS trigger AS $THEBODY$
                         BEGIN
                         %s
                         RETURN NULL;
@@ -316,15 +298,15 @@
         dep_order = counter[cls.AUTOREFRESHER_COUNTER]
         if dep_order > 10**TRIGGER_DEPCOUNTER_PADDED_WIDTH - 1:
             raise ValueError(
                 f"Trigger creation order {dep_order} requires a autonumbering padding width increase (TRIGGER_DEPCOUNTER_PADDED_WIDTH)."
             )
         triggerfn = next(cls.gen_refresh_triggerfunction(), None)
         if triggerfn:
-            for ix, triggertable in enumerate(sorted(cls.fqrefresh_triggers())):
+            for ix, triggertable in enumerate(cls.fqrefresh_triggers()):
                 class_name = f"t%.{TRIGGER_DEPCOUNTER_PADDED_WIDTH}d_%d_autorefresh" % (
                     dep_order,
                     ix,
                 )
                 yield type(
                     class_name,
                     (SamizdatTrigger,),
@@ -338,20 +320,19 @@
                                 FOR EACH STATEMENT EXECUTE PROCEDURE %s;
                             """
                         % triggerfn.creation_identity(),
                     ),
                 )
 
     @classmethod
-    def and_sidekicks(cls):
+    def sidekicks(cls):
         """
         Yields "functions" and "triggers"
         to help manage this Materialized View
         """
-        yield cls
         if not cls.refresh_triggers:
             return
 
         counter = Counter()
         counter.update({cls.AUTOREFRESHER_COUNTER: 1})
         yield from cls.gen_refresh_triggerfunction()
         yield from cls.gen_refresh_tabletriggers(counter=counter)
```

### Comparing `dbsamizdapper-0.0.1/dbsamizdat/samtypes.py` & `dbsamizdapper-0.0.2/dbsamizdat/samtypes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from abc import abstractmethod
+from __future__ import annotations
+
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Iterable, NamedTuple, Protocol
+from typing import Any, Iterable, Type
 
 from dbsamizdat.exceptions import UnsuitableNameError
 
 PG_IDENTIFIER_MAXLEN = 63
 PG_IDENTIFIER_VERBOTEN = set('"')
 # Actually allowed, but we'd have to escape it everywhere.
 # See https://www.postgresql.org/docs/current/sql-syntax-lexical.html#SQL-SYNTAX-IDENTIFIERS
@@ -16,103 +19,188 @@
 # be raised if this is exceeded.
 # The size here is chosen to retain short-ish trigger names without running into problems
 # all too soon.
 
 
 class entitypes(Enum):
     UNDEFINED = "UNDEFINED"
+    TABLE = "TABLE"
     VIEW = "VIEW"
     MATVIEW = "MATERIALIZED VIEW"
     FUNCTION = "FUNCTION"
     TRIGGER = "TRIGGER"
 
 
-class FQTuple(NamedTuple):
-    schema: str
-    object_name: str
-    args: str | None = None
-
-
-class HasFQ(Protocol):
+class HasFQ(ABC):
     """
     Ability to "fully qualify" oneself as a postgres instance
     """
 
     @classmethod
+    @abstractmethod
     def fq(cls) -> FQTuple:
         ...
 
 
+@dataclass(frozen=True)
+class FQTuple:
+    """
+    This dataclass converts different formats of fully qualified names
+    to a consistent class format for `DB object identification`
+    """
+
+    schema: str | None = "public"
+    object_name: str | None = None
+    args: str | None = None
+
+    def __lt__(self, other: FQTuple):
+        return self.db_object_identity() > other.db_object_identity()
+
+    def db_object_identity(self):
+        if self.args is not None:
+            return f'"{self.schema}"."{self.object_name}"({self.args})'
+        return f'"{self.schema}"."{self.object_name}"'
+
+    @classmethod
+    def fqify(cls, arg: FQIffable):
+        """
+        This is a constructor method
+        """
+        if isinstance(arg, FQTuple):
+            return arg
+
+        elif isinstance(arg, str):
+            return cls(schema="public", object_name=arg)
+
+        elif isinstance(arg, tuple):
+            """
+            Convert a 2tuple of schema, thing_name
+            """
+            if len(arg) == 1:
+                return cls(schema=arg[1])
+
+            if len(arg) == 2:
+                return cls(schema=arg[0], object_name=arg[1])
+
+            if len(arg) == 3:
+                return cls(schema=arg[0], object_name=arg[1], args=arg[2])
+
+        elif hasattr(arg, "fq"):
+            """
+            Convert a Samizdat like instance
+            """
+            return arg.fq()
+
+        else:
+            raise TypeError
+
+
 objectname = str
 schemaname = str
 sql_query = str
-# Already a "FQ"; or, something which can give its own FQ
 
 
-class HasFQify(Protocol):
+class SqlGeneration(ABC):
+    """
+    A class which can "sign" itself, "create", and "drop"
+    """
+
     @classmethod
-    def fqify(cls, ref: HasFQ) -> FQTuple:
+    @abstractmethod
+    def sign(cls, cursor: "Mogrifier") -> sql_query:
+        """
+        Generate COMMENT ON sql storing a signature
+        We need the cursor to let psycopg (2) properly escape our json-as-text-string.
+        """
         ...
 
+    @classmethod
+    @abstractmethod
+    def create(cls) -> sql_query:
+        """
+        SQL to create this DB object
+        """
+        ...
 
-class HasRefreshTriggers(HasFQ, HasFQify):
+    @classmethod
+    @abstractmethod
+    def drop(cls, if_exists: bool) -> sql_query:
+        """
+        SQL to drop object. Cascade because we have no idea about the dependency tree.
+        """
+        ...
+
+
+class HasRefreshTriggers(HasFQ):
     """
     Optional extras for refreshing a view on table changes
+    This automatically adds triggers for when a table refreshes to another MatView
     """
 
     refresh_triggers: set["FQIffable"] = set()
 
     @classmethod
     def fqrefresh_triggers(cls):
-        return {cls.fqify(trigger) for trigger in cls.refresh_triggers}
+        return {FQTuple.fqify(trigger) for trigger in cls.refresh_triggers}
 
 
-class ProtoSamizdat(HasFQ, HasFQify):
-    deps_on: set["FQIffable"] = set()
-    deps_on_unmanaged: set["FQIffable"] = set()
-    schema: schemaname | None = "public"
-    sql_template: sql_query = """
-        -- There should be a class-dependent body for ${samizdatname} here.
-        -- See README.md.
-        """
-    entity_type: entitypes
+class HasGetName(ABC):
+    """
+    This object can return a "Name" for itself and
+    will validate that this name is likely to be "nice" for
+    postgres to use
+    """
 
-    @classmethod
-    @abstractmethod
-    def get_name(cls) -> str:
-        return cls.__name__
+    object_name: str | None = None
 
     @classmethod
-    @abstractmethod
-    def db_object_identity(cls) -> str:
-        ...
+    def get_name(cls) -> str:
+        return cls.object_name or cls.__name__
 
     @classmethod
-    @abstractmethod
     def validate_name(cls):
         """
         Check whether name is a valid PostgreSQL identifier. Note that we'll quote
         the identifier everywhere ("quoted identifier" per
         https://www.postgresql.org/docs/current/sql-syntax-lexical.html#SQL-SYNTAX-IDENTIFIERS)
         """
         name = cls.get_name()
         for char in name:
             if ord(char) > 0x7F:
                 raise UnsuitableNameError("Name contains non-ASCII characters", samizdat=cls)
         # Technically we could UESCAPE these,
         # and make the length calculation much more complicated.
         if len(name) > PG_IDENTIFIER_MAXLEN:
             raise UnsuitableNameError("Name is too long", samizdat=cls)
-        if set(name) & PG_IDENTIFIER_VERBOTEN:
-            badchars = {set(name) & PG_IDENTIFIER_VERBOTEN}
+        if badchars := set(name) & PG_IDENTIFIER_VERBOTEN:
             raise UnsuitableNameError(
                 f"""Name contains unwelcome characters ({badchars})""",
                 samizdat=cls,
             )
 
+
+class ProtoSamizdat(HasFQ, HasGetName, SqlGeneration):
+    """
+    A Samizdat class has abilities to create SQL and
+    describe itself using a fully qualified name
+    """
+
+    deps_on: set[FQIffable] = set()
+    deps_on_unmanaged: set[FQIffable] = set()
+    schema: schemaname | None = "public"
+    sql_template: sql_query = """
+        -- There should be a class-dependent body for ${samizdatname} here.
+        -- See README.md.
+        """
+    entity_type: entitypes
+
+    @classmethod
+    def db_object_identity(cls) -> str:
+        return cls.fq().db_object_identity()
+
     @classmethod
     @abstractmethod
     def definition_hash(cls):
         """
         Return the "implanted" hash if preset or generate
         a new descriptive hash of this instance
         """
@@ -134,57 +222,38 @@
         """
         Returns descriptor (json) for this object, to be stored in the database
         """
         ...
 
     @classmethod
     @abstractmethod
-    def sign(cls, cursor: "Mogrifier") -> sql_query:
-        """
-        Generate COMMENT ON sql storing a signature
-        We need the cursor to let psycopg (2) properly escape our json-as-text-string.
-        """
+    def head_id(cls) -> str:
         ...
 
-    @classmethod
-    @abstractmethod
-    def create(cls) -> sql_query:
-        """
-        SQL to create this DB object
-        """
-        ...
 
-    @classmethod
-    @abstractmethod
-    def drop(cls, if_exists: bool) -> sql_query:
-        """
-        SQL to drop object. Cascade because we have no idea about the dependency tree.
-        """
-        ...
+FQIffable = FQTuple | HasFQ | str | ProtoSamizdat | Type[ProtoSamizdat] | tuple[str, ...]
 
-    @classmethod
-    @abstractmethod
-    def and_sidekicks(cls) -> Iterable["ProtoSamizdat"]:
-        """
-        On some classes, this will yield autogenerated sidekick classes
-        """
-        ...
+
+class HasSidekicks(ABC):
+    """
+    Some Samizdat classes have additional
+    triggers or functions
+    One example is Materialized Views with `refresh_triggers`
+    """
 
     @classmethod
     @abstractmethod
-    def head_id(cls) -> str:
+    def sidekicks(cls) -> Iterable["ProtoSamizdat"]:
         ...
 
 
-FQIffable = FQTuple | HasFQ | str | ProtoSamizdat | tuple[str, ...]
-
-
-class Mogrifier(Protocol):
+class Mogrifier(ABC):
     """
     A class which can "mogrify" a SQL string
+    This helps to differentiate between psycopg & pscyopg2 'Cursur
     """
 
     @abstractmethod
     def mogrify(self, *args, **kwargs) -> str | bytes:
         ...
 
     @property
```

### Comparing `dbsamizdapper-0.0.1/pyproject.toml` & `dbsamizdapper-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbsamizdapper"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Josh Brooks <josh@catalpa.io>",]
 readme = "README.md"
 
 packages = [
     { include = "dbsamizdat" },
 ]
```

### Comparing `dbsamizdapper-0.0.1/PKG-INFO` & `dbsamizdapper-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbsamizdapper
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,11 +30,26 @@
  - Opinionated code formatting
    - black + isort
    - replaced `lambda`s
  - some simple `pytest` functions
 
 and probably many more undocumented changes
 
+
+## Running Tests
+
+Spin up a docker container
+
+`docker run -p 5435:5432 -e POSTGRES_HOST_AUTH_METHOD=trust postgres:latest`
+
+The db url for this container would be:
+
+"postgresql:///postgres@localhost:5435/postgres"
+
+Make this the environment variable `DB_URL`, or add it to the `.env` file
+
 ## Original README
 
 Check out the original readme for rationale and how-to documentation
 
+
+
```

