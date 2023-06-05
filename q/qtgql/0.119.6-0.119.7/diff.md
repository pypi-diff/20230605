# Comparing `tmp/qtgql-0.119.6.tar.gz` & `tmp/qtgql-0.119.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.119.6.tar", max compression
+gzip compressed data, was "qtgql-0.119.7.tar", max compression
```

## Comparing `qtgql-0.119.6.tar` & `qtgql-0.119.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1064 2023-06-04 14:43:06.560257 qtgql-0.119.6/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-04 14:43:06.560257 qtgql-0.119.6/README.md
--rw-r--r--   0        0        0     4445 2023-06-04 14:43:25.564415 qtgql-0.119.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0        0 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/compiler/__init__.py
--rw-r--r--   0        0        0     1761 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/compiler/builtin_scalars.py
--rw-r--r--   0        0        0    13091 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/compiler/operation.py
--rw-r--r--   0        0        0     3733 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/compiler/template.py
--rw-r--r--   0        0        0     2159 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/config.py
--rw-r--r--   0        0        0      420 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/cppref.py
--rw-r--r--   0        0        0       41 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/exceptions.py
--rw-r--r--   0        0        0     3187 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/graphql_ref.py
--rw-r--r--   0        0        0    17783 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/introspection.py
--rw-r--r--   0        0        0    11078 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/objecttype.py
--rw-r--r--   0        0        0        0 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/runtime/__init__.py
--rw-r--r--   0        0        0     1571 2023-06-04 14:43:06.572257 qtgql-0.119.6/qtgqlcodegen/runtime/custom_scalars.py
--rw-r--r--   0        0        0      488 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0      536 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/templates/config.jinja.hpp
--rw-r--r--   0        0        0     5016 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/templates/macros.jinja.hpp
--rw-r--r--   0        0        0     4857 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     4077 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0     1028 2023-06-04 14:43:06.576257 qtgql-0.119.6/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-05 12:12:53.216019 qtgql-0.119.7/LICENSE
+-rw-r--r--   0        0        0     1805 2023-06-05 12:12:53.216019 qtgql-0.119.7/README.md
+-rw-r--r--   0        0        0     4445 2023-06-05 12:13:20.364525 qtgql-0.119.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/compiler/__init__.py
+-rw-r--r--   0        0        0     1782 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/compiler/builtin_scalars.py
+-rw-r--r--   0        0        0    13094 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/compiler/operation.py
+-rw-r--r--   0        0        0     3940 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/compiler/template.py
+-rw-r--r--   0        0        0     2167 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0     1246 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/cppref.py
+-rw-r--r--   0        0        0       41 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/exceptions.py
+-rw-r--r--   0        0        0     3187 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/graphql_ref.py
+-rw-r--r--   0        0        0    18043 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/introspection.py
+-rw-r--r--   0        0        0    12736 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/objecttype.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/runtime/__init__.py
+-rw-r--r--   0        0        0     1571 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/runtime/custom_scalars.py
+-rw-r--r--   0        0        0      488 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0      536 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/config.jinja.hpp
+-rw-r--r--   0        0        0     5016 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/macros.jinja.hpp
+-rw-r--r--   0        0        0     4917 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0      816 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/schema.jinja.cpp
+-rw-r--r--   0        0        0     4552 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0     1028 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.7/PKG-INFO
```

### Comparing `qtgql-0.119.6/LICENSE` & `qtgql-0.119.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.6/README.md` & `qtgql-0.119.7/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.6/pyproject.toml` & `qtgql-0.119.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.119.6"
+version = "0.119.7"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.119.6/qtgqlcodegen/cli.py` & `qtgql-0.119.7/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.6/qtgqlcodegen/compiler/builtin_scalars.py` & `qtgql-0.119.7/qtgqlcodegen/compiler/builtin_scalars.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,12 +64,13 @@
                 yield member
 
     def by_graphql_name(self, name: str) -> Optional[BuiltinScalar]:
         for scalar in self:
             if scalar.graphql_name == name:
                 return scalar
 
+    @cached_property
     def keys(self) -> list[str]:
         return [scalar.graphql_name for scalar in self]
 
 
 BuiltinScalars = _BuiltinScalars()
```

### Comparing `qtgql-0.119.6/qtgqlcodegen/compiler/operation.py` & `qtgql-0.119.7/qtgqlcodegen/compiler/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                 assert fragment
 
                 type_name = fragment.type_condition.name.value
                 concrete = operation.evaluator.get_objecttype_by_name(type_name)
                 assert concrete
                 if not has_typename_selection(fragment.selection_set):
                     inject_typename_selection(fragment.selection_set)
-                if not has_id_selection(fragment.selection_set) and concrete.has_id_field:
+                if not has_id_selection(fragment.selection_set) and concrete.implements_node:
                     inject_id_selection(fragment.selection_set)
 
                 for selection_node in fragment.selection_set.selections:
                     field_node = is_field_node(selection_node)
                     assert field_node
 
                     if not is_type_name_selection(field_node):
```

### Comparing `qtgql-0.119.6/qtgqlcodegen/compiler/template.py` & `qtgql-0.119.7/qtgqlcodegen/compiler/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     if ignore:
         return v
     return "{" + v + "}"
 
 
 template_env.filters["wrapcurly"] = wrap_curly_filter
 
-SCHEMA_TEMPLATE = template_env.get_template("schema.jinja.hpp")
+SCHEMA_HPP_TEMPLATE = template_env.get_template("schema.jinja.hpp")
+SCHEMA_CPP_TEMPLATE = template_env.get_template("schema.jinja.cpp")
 OPERATION_TEMPLATE = template_env.get_template("operation.jinja.hpp")
 CONFIG_TEMPLATE = template_env.get_template("config.jinja.hpp")
 CMAKE_TEMPLATE = template_env.get_template("CMakeLists.jinja.cmake")
 
 
 @define
 class SchemaTemplateContext:
@@ -77,16 +78,20 @@
         return self.operation.name.lower()
 
     @property
     def schema_ns(self) -> str:
         return self.config.env_name
 
 
-def schema_types_template(context: SchemaTemplateContext) -> str:
-    return SCHEMA_TEMPLATE.render(context=context)
+def schema_types_template_hpp(context: SchemaTemplateContext) -> str:
+    return SCHEMA_HPP_TEMPLATE.render(context=context)
+
+
+def schema_types_template_cpp(context: SchemaTemplateContext) -> str:
+    return SCHEMA_CPP_TEMPLATE.render(context=context)
 
 
 def operation_template(context: OperationTemplateContext) -> str:
     return OPERATION_TEMPLATE.render(context=context)
 
 
 @define(slots=False)
```

### Comparing `qtgql-0.119.6/qtgqlcodegen/config.py` & `qtgql-0.119.7/qtgqlcodegen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import cached_property
 from pathlib import Path
 from typing import Callable
 from typing import Type
 
 from attrs import define
 
-from qtgqlcodegen.compiler.template import schema_types_template
+from qtgqlcodegen.compiler.template import schema_types_template_hpp
 from qtgqlcodegen.compiler.template import SchemaTemplateContext
 from qtgqlcodegen.introspection import SchemaEvaluator
 from qtgqlcodegen.runtime.custom_scalars import CUSTOM_SCALARS
 from qtgqlcodegen.runtime.custom_scalars import CustomScalarMap
 
 
 @define(slots=False)
@@ -28,15 +28,15 @@
 
     Also the generated QML imports would fall under this namespace.
     """
     evaluator: Type[SchemaEvaluator] = SchemaEvaluator
     """evaluates the schema and generates types."""
     custom_scalars: CustomScalarMap = {}
     """mapping of custom scalars, respected by the schema evaluator."""
-    template_class: Callable[[SchemaTemplateContext], str] = schema_types_template
+    template_class: Callable[[SchemaTemplateContext], str] = schema_types_template_hpp
     """jinja template."""
     debug: bool = False
     """Templates would render some additional helpers for testing."""
 
     @cached_property
     def schema_path(self) -> Path:
         return self.graphql_dir / "schema.graphql"
```

### Comparing `qtgql-0.119.6/qtgqlcodegen/graphql_ref.py` & `qtgql-0.119.7/qtgqlcodegen/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.6/qtgqlcodegen/introspection.py` & `qtgql-0.119.7/qtgqlcodegen/introspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 from qtgqlcodegen.compiler.builtin_scalars import BuiltinScalars
 from qtgqlcodegen.compiler.operation import QtGqlOperationDefinition
 from qtgqlcodegen.compiler.template import cmake_template
 from qtgqlcodegen.compiler.template import CmakeTemplateContext
 from qtgqlcodegen.compiler.template import operation_template
 from qtgqlcodegen.compiler.template import OperationTemplateContext
-from qtgqlcodegen.compiler.template import schema_types_template
+from qtgqlcodegen.compiler.template import schema_types_template_cpp
+from qtgqlcodegen.compiler.template import schema_types_template_hpp
 from qtgqlcodegen.compiler.template import SchemaTemplateContext
 from qtgqlcodegen.exceptions import QtGqlException
 from qtgqlcodegen.graphql_ref import is_enum_definition
 from qtgqlcodegen.graphql_ref import is_input_definition
 from qtgqlcodegen.graphql_ref import is_interface_definition
 from qtgqlcodegen.graphql_ref import is_list_definition
 from qtgqlcodegen.graphql_ref import is_named_type_node
@@ -280,15 +281,15 @@
                     f"type {type_} does not not define an id field.\n"
                     f"fields: {type_.fields}",
                 )
         implements = [self._evaluate_interface_type(interface) for interface in type_.interfaces]
 
         ret = QtGqlObjectTypeDefinition(
             name=t_name,
-            implements=implements,
+            interfaces_raw=implements,
             docstring=type_.description,
             fields_dict={
                 name: self._evaluate_field(name, field) for name, field in type_.fields.items()
             },
         )
         self._objecttypes_def_map[ret.name] = ret
         for interface in type_.interfaces:
@@ -318,15 +319,15 @@
         interface: gql_def.GraphQLInterfaceType,
     ) -> QtGqlInterfaceDefinition:
         if ret := self._interfaces_map.get(interface.name, None):
             return ret
         implements = [self._evaluate_interface_type(base) for base in interface.interfaces]
         ret = QtGqlInterfaceDefinition(
             name=interface.name,
-            implements=implements,
+            interfaces_raw=implements,
             docstring=interface.description,
             fields_dict={
                 name: self._evaluate_field(name, field) for name, field in interface.fields.items()
             },
         )
         self._interfaces_map[ret.name] = ret
         return ret
@@ -377,25 +378,14 @@
         operation_miner = QtGqlVisitor(self)
         visitor.visit(operations, operation_miner)
         self._operations.update(operation_miner.operations)
 
     def generate(self) -> list[FileSpec]:
         self.parse_schema_concretes()
         self.parse_operations()
-        context = SchemaTemplateContext(
-            enums=list(self._enums_def_map.values()),
-            types=[
-                t
-                for name, t in self._objecttypes_def_map.items()
-                if name not in BuiltinScalars.keys() and name not in self.root_types_names
-            ],
-            interfaces=list(self._interfaces_map.values()),
-            input_objects=list(self._input_objects_def_map.values()),
-            config=self.config,
-        )
 
         operations: list[FileSpec] = []
         for op_name, op in self._operations.items():
             operations.append(
                 FileSpec(
                     content=operation_template(
                         OperationTemplateContext(
@@ -403,30 +393,46 @@
                             config=self.config,
                             debug=self.config.debug,
                         ),
                     ),
                     path=self.config.generated_dir / f"{op_name}.hpp",
                 ),
             )
-        schema = FileSpec(
-            content=schema_types_template(context),
+
+        context = SchemaTemplateContext(
+            enums=list(self._enums_def_map.values()),
+            types=[
+                t
+                for name, t in self._objecttypes_def_map.items()
+                if name not in BuiltinScalars.keys and name not in self.root_types_names
+            ],
+            interfaces=list(self._interfaces_map.values()),
+            input_objects=list(self._input_objects_def_map.values()),
+            config=self.config,
+        )
+        schema_hpp = FileSpec(
+            content=schema_types_template_hpp(context),
             path=self.config.generated_dir / "schema.hpp",
         )
+        schema_cpp = FileSpec(
+            content=schema_types_template_cpp(context),
+            path=self.config.generated_dir / "schema.cpp",
+        )
 
-        return [schema, *operations]
+        return [schema_hpp, schema_cpp, *operations]
 
     def dump(self):
         """:param file: Path to the directory the codegen would dump to."""
-        headers = self.generate()
+        sources = self.generate()
 
         args = ["clang-format"] + [
-            str(f.path) for f in headers if f.path.suffix in (".cpp", ".h", ".hpp")
+            str(f.path) for f in sources if f.path.suffix in (".cpp", ".h", ".hpp")
         ]
         cmake = FileSpec(
-            content=cmake_template(CmakeTemplateContext(config=self.config, sources=headers)),
+            content=cmake_template(CmakeTemplateContext(config=self.config, sources=sources)),
             path=self.config.generated_dir / "CMakeLists.txt",
         )
-        headers.append(cmake)
+        sources.append(cmake)
         args.append("-i")
-        for f in headers:
+        for f in sources:
             f.dump()
         subprocess.run(args)
```

### Comparing `qtgql-0.119.6/qtgqlcodegen/objecttype.py` & `qtgql-0.119.7/qtgqlcodegen/objecttype.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import attrs
 from attrs import define
 from typingref import TypeHinter
 from typingref import UNSET
 
 from qtgqlcodegen.compiler.builtin_scalars import BuiltinScalar
 from qtgqlcodegen.compiler.operation import QtGqlQueriedObjectType
+from qtgqlcodegen.cppref import QtGqlTypes
 from qtgqlcodegen.utils import AntiForwardRef
 
 if TYPE_CHECKING:
     from qtgqlcodegen.runtime.custom_scalars import CustomScalarDefinition
     from qtgqlcodegen.runtime.custom_scalars import CustomScalarMap
 
 
@@ -157,16 +158,16 @@
 
     @cached_property
     def can_select_id(self) -> Optional[QtGqlFieldDefinition]:
         object_type = self.type.is_object_type or self.type.is_interface
         if not object_type:
             if self.type.is_model:
                 object_type = self.type.is_model.is_object_type
-        if object_type:
-            return object_type.has_id_field
+        if object_type and object_type.implements_node:
+            return object_type.fields_dict["id"]
 
 
 @define(slots=False)
 class BaseGqlTypeDefinition:
     name: str
     fields_dict: dict[str, QtGqlFieldDefinition]
     docstring: Optional[str] = ""
@@ -174,28 +175,73 @@
     @property
     def fields(self) -> list[QtGqlFieldDefinition]:
         return list(self.fields_dict.values())
 
 
 @define(slots=False)
 class QtGqlObjectTypeDefinition(BaseGqlTypeDefinition):
-    implements: list[QtGqlInterfaceDefinition] = attrs.Factory(list)
+    interfaces_raw: list[QtGqlInterfaceDefinition] = attrs.Factory(list)
 
-    @cached_property
-    def has_id_field(self) -> Optional[QtGqlFieldDefinition]:
-        return self.fields_dict.get("id", None)
+    def implements(self, interface: QtGqlInterfaceDefinition) -> bool:
+        for m_interface in self.interfaces_raw:
+            if interface is m_interface or m_interface.implements(interface):
+                return True
+        return False
 
     @cached_property
-    def id_is_optional(self) -> Optional[QtGqlFieldDefinition]:
-        if id_f := self.has_id_field:
-            if id_f.type.is_optional():
-                return id_f
+    def bases(self) -> list[QtGqlInterfaceDefinition]:
+        """
+        returns only the top level interfaces that should be inherited.
+        if i.e
+        ```graphql
+        interface Node{
+        id: ID!
+        }
+
+        interface A implements Node{
+        otherField: String!
+        }
+
+        type Foo implements A{
+        ...
+        }
+        ```
+        Type `Foo` would extend only `A`
+
+        If there are no interfaces returns only ObjectTypeABCWithID or ObjectTypeABC.
+        """
+        not_unique_interfaces: list[QtGqlInterfaceDefinition] = []
+
+        if not self.interfaces_raw:
+            # these are not really interfaces though they are inherited if there are no interfaces.
+            if self.implements_node:
+                return [QtGqlTypes.ObjectTypeABCWithID]  # type: ignore
+
+            else:
+                return [QtGqlTypes.ObjectTypeABC]  # type: ignore
+
+        for interface in self.interfaces_raw:
+            for other in self.interfaces_raw:
+                if other is not interface:
+                    if interface.implements(other):
+                        not_unique_interfaces.append(other)
+
+        return [intfs for intfs in self.interfaces_raw if intfs not in not_unique_interfaces]
+
+    @cached_property
+    def implements_node(self) -> bool:
+        if isinstance(self, QtGqlInterfaceDefinition):
+            if self.name == "Node":
+                return True
+        return any(base.implements_node for base in self.bases)
 
     def __attrs_post_init__(self):
-        for base in self.implements:
+        # inject this object type to the interface.
+        # later the interface would use this list to know who he might resolve to.
+        for base in self.interfaces_raw:
             if not base.implementations.get(self.name):
                 base.implementations[self.name] = self
 
 
 @define(slots=False)
 class QtGqlInterfaceDefinition(QtGqlObjectTypeDefinition):
     implementations: dict[str, BaseGqlTypeDefinition] = attrs.field(factory=dict)
```

### Comparing `qtgql-0.119.6/qtgqlcodegen/runtime/custom_scalars.py` & `qtgql-0.119.7/qtgqlcodegen/runtime/custom_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.6/qtgqlcodegen/templates/config.jinja.hpp` & `qtgql-0.119.7/qtgqlcodegen/templates/config.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.6/qtgqlcodegen/templates/macros.jinja.hpp` & `qtgql-0.119.7/qtgqlcodegen/templates/macros.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.6/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.119.7/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -83,14 +83,16 @@
 return ret;
 };
 public:
 👉 context.operation.name 👈(): qtgql::gqlwstransport::OperationHandlerABC(qtgql::gqlwstransport::GqlWsTrnsMsgWithID(qtgql::gqlwstransport::OperationPayload(
         {%- for line in context.operation.query.splitlines() %}"👉 line 👈"{% endfor -%}
         ), OPERATION_ID)){};
 
+QTGQL_STATIC_MAKE_SHARED(👉 context.operation.name 👈)
+
 inline const QUuid &operation_id() const override{
 return OPERATION_ID;
 }
 
 
 void on_next(const QJsonObject &message) override{
     if (!m_data && message.contains("data")){
```

### Comparing `qtgql-0.119.6/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.119.7/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% import "macros.jinja.hpp" as macros -%}
 #pragma once
 #include <QObject>
 #include <QJsonObject>
+#include <QJsonArray>
 #include <memory>
 
 #include <qtgql/bases/bases.hpp>
 {% for dep in context.dependencies -%}
 👉 dep 👈
 {% endfor %}
 
@@ -35,42 +36,52 @@
     GraphQLEnum_MACRO(👉enum.name👈)
 };
 
 {% endfor %}
 };
 {% endif %}
 
+// ---------- Interfaces ----------
+{% for interface in context.interfaces -%}
+class 👉 interface.name 👈 {% for base in interface.bases %} {%if loop.first %}: {% endif %} public 👉 base.name 👈 {% if not loop.last %}, {% endif %}{% endfor %}{
+Q_OBJECT
+👉 macros.concrete_type_fields(interface) 👈
+
+static std::shared_ptr<👉 interface.name 👈> from_json(const QJsonObject& data,
+                                                const qtgql::bases::SelectionsConfig &config,
+                                                const qtgql::bases::OperationMetadata& metadata);
+
+};
+{% endfor %}
+
 // ---------- Object Types ----------
 {% for type in context.types %}
-{%- set base_class -%}{% if type.has_id_field %}ObjectTypeABCWithID{% else %}ObjectTypeABC{% endif %}{%- endset -%}
-class 👉 type.name 👈 : public qtgql::bases::👉 base_class 👈{
+{%- set base_class -%}{% if type. implements_node %}ObjectTypeABCWithID{% else %}ObjectTypeABC{% endif %}{%- endset -%}
+class 👉 type.name 👈 {% for base in type.bases %}{%if loop.first%}: {% endif %} public 👉 base.name 👈 {% if not loop.last %}, {% endif %}{% endfor %}{
 Q_OBJECT
 
 protected:
 👉 macros.concrete_type_fields(type) 👈
 public:
 static auto & INST_STORE() {
     static qtgql::bases::ObjectStore<👉 type.name 👈> _store;
     return _store;
 }
 inline static const QString TYPE_NAME = "👉 type.name 👈";
 static auto get_node(const QString & id){
     return INST_STORE().get_node(id);
 }
-explicit 👉 type.name 👈 (QObject* parent = nullptr)
-: qtgql::bases::👉 base_class 👈::👉 base_class 👈(parent) {};
-
 
 static std::shared_ptr<👉 type.name 👈> from_json(const QJsonObject& data,
                                  const qtgql::bases::SelectionsConfig &config,
                                  const qtgql::bases::OperationMetadata& metadata){
 if (data.isEmpty()){
     return {};
 }
-{% if type.has_id_field %}
+{% if type. implements_node %}
 if (config.selections.contains("id") && !data.value("id").isNull()) {
     auto cached_maybe = get_node(data.value("id").toString());
     if(cached_maybe.has_value()){
         auto node = cached_maybe.value();
         node->update(data, config);
         return node;
     }
@@ -78,26 +89,22 @@
 {% endif %}
 
 auto inst = std::make_shared<👉 type.name 👈>();
 {% for f in type.fields -%}
 {% set assign_to %} inst->👉 f.private_name 👈 {% endset %}
 👉macros.deserialize_field(f, assign_to)👈
 {% endfor %}
-{% if type.id_is_optional %}
-if (inst->id) {
-INST_STORE().add_node(inst, metadata.operation_id);
-}
-{% elif type.has_id_field and not type.id_is_optional %}
+{% if type. implements_node %}
 INST_STORE().add_node(inst, metadata.operation_id);
 {% endif %}
 return inst;
 };
 
 void loose(const qtgql::bases::OperationMetadata &metadata){
-    {% if type.has_id_field %}
+    {% if type. implements_node %}
     INST_STORE().loose(m_id, metadata.operation_id);
     {% else %}
     throw "not implemented";
     {% endif %}
 };
 void update(const QJsonObject &data,
             const qtgql::bases::SelectionsConfig &config){
```

### Comparing `qtgql-0.119.6/qtgqlcodegen/utils.py` & `qtgql-0.119.7/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.6/PKG-INFO` & `qtgql-0.119.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.119.6
+Version: 0.119.7
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

