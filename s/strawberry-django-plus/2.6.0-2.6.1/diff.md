# Comparing `tmp/strawberry_django_plus-2.6.0.tar.gz` & `tmp/strawberry_django_plus-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.6.0.tar", max compression
+gzip compressed data, was "strawberry_django_plus-2.6.1.tar", max compression
```

## Comparing `strawberry_django_plus-2.6.0.tar` & `strawberry_django_plus-2.6.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1094 2023-06-01 15:39:56.763017 strawberry_django_plus-2.6.0/LICENSE
--rw-r--r--   0        0        0     3299 2023-06-01 15:39:56.763017 strawberry_django_plus-2.6.0/README.md
--rw-r--r--   0        0        0     4309 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     3001 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5562 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5751 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    26052 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3069 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1657 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6304 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0      896 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/middlewares/user_warmup.py
--rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    25062 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14825 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    26108 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1372 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27526 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    47560 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2337 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    18702 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10297 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13069 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-06-01 15:39:56.767017 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13142 2023-06-01 15:39:56.771016 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-06-01 15:39:56.771016 strawberry_django_plus-2.6.0/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-06-05 15:02:15.404553 strawberry_django_plus-2.6.1/LICENSE
+-rw-r--r--   0        0        0     3299 2023-06-05 15:02:15.404553 strawberry_django_plus-2.6.1/README.md
+-rw-r--r--   0        0        0     4309 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3001 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5562 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5751 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    26052 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3069 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1657 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1389 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0     6304 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0      896 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/middlewares/user_warmup.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    25062 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14825 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26108 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1372 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    27526 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0    47691 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1107 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0     1445 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
+-rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2357 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    18702 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0    10297 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13069 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    13142 2023-06-05 15:02:15.416553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-06-05 15:02:15.416553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.6.1/PKG-INFO
```

### Comparing `strawberry_django_plus-2.6.0/LICENSE` & `strawberry_django_plus-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/README.md` & `strawberry_django_plus-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/pyproject.toml` & `strawberry_django_plus-2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.6.0"
+version = "2.6.1"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
```

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/__init__.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/__init__.py`

 * *Files identical despite different names*

```diff
@@ -12,15 +12,15 @@
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
-__version__ = "2.6.0"  # x-release-please-version
+__version__ = "2.6.1"  # x-release-please-version
 
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
```

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/directives.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/field.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/filters.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/middlewares/debug_toolbar.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/middlewares/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/middlewares/user_warmup.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/middlewares/user_warmup.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/ordering.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/permissions.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/relay.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/relay.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from strawberry.lazy_type import LazyType
 from strawberry.permission import BasePermission
 from strawberry.schema.types.scalar import DEFAULT_SCALAR_REGISTRY
 from strawberry.type import StrawberryContainer, StrawberryList, StrawberryOptional
 from strawberry.types import Info
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.types.types import TypeDefinition
+from strawberry.union import StrawberryUnion
 from strawberry.utils.await_maybe import AwaitableOrValue
 from strawberry.utils.str_converters import to_camel_case
 from typing_extensions import Annotated
 
 from .settings import config
 from .utils import aio
 
@@ -994,21 +995,14 @@
     def get_result(
         self,
         source: Any,
         info: Info,
         args: List[Any],
         kwargs: Dict[str, Any],
     ) -> AwaitableOrValue[Any]:
-        type_def = info.return_type._type_definition  # type: ignore
-        assert isinstance(type_def, TypeDefinition)
-
-        field_type = type_def.type_var_map[NodeType]
-        if isinstance(field_type, LazyType):
-            field_type = field_type.resolve_type()
-
         if self.base_resolver is not None:
             # If base_resolver is not self.conn_resolver, then it is defined to something
             assert self.base_resolver
 
             resolver_args = self.resolver_args
             resolver_kwargs = {
                 # Consider both args not in default args and the ones specified by the resolver,
@@ -1032,15 +1026,26 @@
         *,
         nodes: AwaitableOrValue[Optional[Union[Iterable[Node], Connection[Node]]]] = None,
     ):
         # The base_resolver might have resolved to a Connection directly
         if isinstance(nodes, Connection):
             return nodes
 
-        return_type = cast(Connection[Node], info.return_type)
+        return_type = info.return_type
+        if isinstance(return_type, StrawberryUnion):
+            candidates = [
+                rt
+                for rt in return_type.types
+                if isinstance(rt, type) and issubclass(rt, Connection)
+            ]
+            if len(candidates) > 1:
+                raise TypeError("Multiple connection types found in union")
+
+            return_type = candidates[0]
+
         type_def = return_type._type_definition  # type: ignore
         assert isinstance(type_def, TypeDefinition)
 
         field_type = type_def.type_var_map[NodeType]
         if isinstance(field_type, LazyType):
             field_type = field_type.resolve_type()
```

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/settings.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html` & `strawberry_django_plus-2.6.1/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/test/client.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/test/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def request(
         self,
         body: Dict[str, object],
         headers: Optional[Dict[str, object]] = None,
         files: Optional[Dict[str, object]] = None,
     ):
-        kwargs: Dict[str, object] = {"data": body}
+        kwargs: Dict[str, object] = {"data": body, "headers": headers}
         if files:
             kwargs["format"] = "multipart"
         else:
             kwargs["content_type"] = "application/json"
 
         return self.client.post(self.path, **kwargs)
```

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/type.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/type.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/types.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.0/PKG-INFO` & `strawberry_django_plus-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.6.0
+Version: 2.6.1
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

