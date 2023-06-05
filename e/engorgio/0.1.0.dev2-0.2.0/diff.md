# Comparing `tmp/engorgio-0.1.0.dev2.tar.gz` & `tmp/engorgio-0.2.0.tar.gz`

## Comparing `engorgio-0.1.0.dev2.tar` & `engorgio-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/.pydantic-typer-copier-answers.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/CHANGELOG.md
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/.github/workflows/release.yml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/engorgio/__about__.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/engorgio/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/engorgio/decorator.py
--rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/engorgio/expand.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/examples/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/examples/person.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/examples/person_cli.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/tests/__init__.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/tests/models.py
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/tests/test_person.py
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/LICENSE.txt
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/README.md
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 engorgio-0.1.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 engorgio-0.2.0/.pydantic-typer-copier-answers.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 engorgio-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 engorgio-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 engorgio-0.2.0/docs/tutorial.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 engorgio-0.2.0/engorgio/__about__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 engorgio-0.2.0/engorgio/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 engorgio-0.2.0/engorgio/condense.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 engorgio-0.2.0/engorgio/decorator.py
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 engorgio-0.2.0/engorgio/expand.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 engorgio-0.2.0/examples/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 engorgio-0.2.0/examples/person.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 engorgio-0.2.0/examples/person_cli.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/models.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/test_expand.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/test_hero.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/test_no_model.py
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 engorgio-0.2.0/tests/test_person.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 engorgio-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 engorgio-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 engorgio-0.2.0/README.md
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 engorgio-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 engorgio-0.2.0/PKG-INFO
```

### Comparing `engorgio-0.1.0.dev2/engorgio/expand.py` & `engorgio-0.2.0/engorgio/expand.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,178 +5,231 @@
 
 SPDX-FileCopyrightText: 2023-present Waylon S. Walker <waylon@waylonwalker.com>
 
 SPDX-License-Identifier: MIT
 """
 
 import inspect
-from typing import Any, Callable, Dict, Optional
+import os
+from typing import Callable, Dict, Optional
 
-import pyflyby
+import black
 from pydantic.fields import ModelField
 
 
+def create_default(field: ModelField) -> str:
+    """Create the default value for pydantic ModelFields."""
+    if "=" not in repr(field) and not hasattr(field, "required"):
+        default = ""
+    if "=" not in repr(field) and hasattr(field, "required"):
+        default = ""
+    elif not hasattr(field, "required"):
+        default = f'="{field.default}"'
+    elif field.default is None and not getattr(field, "required", False):
+        default = "=None"
+    elif field.default is not None:
+        default = f'="{field.default}"'
+    else:
+        default = ""
+
+    return default
+
+
+def create_default_typer(
+    panel_name: str,
+    field: ModelField,
+    *,
+    prompt_always: bool = False,
+) -> str:
+    """Create the default value for pydantic ModelFields for typer functions."""
+    prompt = ""
+    if prompt_always:
+        prompt = ", prompt=True"
+    if "=" not in repr(field) and not hasattr(field, "required"):
+        default = ""
+    if "=" not in repr(field) and hasattr(field, "required"):
+        default = "=None"
+    elif not hasattr(field, "required"):
+        default = f'="{field.default}"'
+    elif field.default is None and not getattr(field, "required", False):
+        default = f' = typer.Option(None, help="{field.field_info.description or ""}", rich_help_panel="{panel_name}"{prompt})'
+    elif field.default is not None:
+        default = f' = typer.Option("{field.default}", help="{field.field_info.description or ""}", rich_help_panel="{panel_name}"{prompt})'
+    else:
+        default = f' = typer.Option(..., help="{field.field_info.description or ""}", rich_help_panel="{panel_name}", prompt=True)'
+    return default
+
+
 def make_annotation(
     name: str,
     field: ModelField,
-    names: Dict[str, str],
+    # parents: Dict[str, str],
+    model_separator: str = "__",
     *,
     typer: bool = False,
+    prompt_always: bool = False,
 ) -> str:
     """Create an annotation for pydantic ModelFields."""
-    panel_name = names.get(name)
-    next_name = panel_name
-    while next_name is not None:
-        next_name = names.get(next_name)
-        if next_name is not None:
-            panel_name = f"{next_name}.{panel_name}"
+    # might still need this when parents=False
+    # while next_name is not None:
+    #     if next_name is not None:
 
     annotation = (
         field.annotation.__name__
         if str(field.annotation).startswith("<")
         else str(field.annotation)
     )
-
-    if "=" not in repr(field) and not hasattr(field, "required"):
-        default = "=None"
-    elif not hasattr(field, "required"):
-        default = f'="{field.default}"'
-    elif field.default is None and not getattr(field, "required", False):
-        if typer:
-            default = f' = typer.Option(None, help="{field.field_info.description or ""}", rich_help_panel="{panel_name}")'
-        else:
-            default = "=None"
-    elif field.default is not None:
-        if typer:
-            default = f' = typer.Option("{field.default}", help="{field.field_info.description or ""}", rich_help_panel="{panel_name}")'
-        else:
-            default = f'="{field.default}"'
-    elif typer:
-        default = f' = typer.Option(..., help="{field.field_info.description or ""}", rich_help_panel="{panel_name}", prompt=True)'
-    else:
-        default = ""
+    annotation = f": {annotation}" if annotation != "_empty" else ""
     if typer:
-        return f"{name}: {annotation}{default}"
-    return f"{name}: {annotation}{default}"
+        default = create_default_typer(
+            panel_name="--".join(name.split(model_separator)[:-1]),
+            field=field,
+            prompt_always=prompt_always,
+        )
+    else:
+        default = create_default(
+            field=field,
+        )
+
+    return f"{name}{annotation}{default}"
 
 
-def make_signature(
+def init_more_args(
     func: Callable,
-    wrapper: Callable,
+    more_args: Dict,
+    model_separator: str = "__",
     *,
-    typer: bool = False,
-    more_args: Optional[Dict] = None,
-):
-    """Return a new function with that accepts model fields."""
-    if more_args is None:
-        more_args = {}
+    include_parent_model: bool = False,
+) -> Dict:
+    """Initialize the more_args dict."""
+    parents = {}
     sig = inspect.signature(func)
-    names = {}
     for name, param in sig.parameters.items():
         if hasattr(param.annotation, "__fields__"):
-            more_args = {**more_args, **param.annotation.__fields__}
+            if include_parent_model:
+                new_param = {
+                    f"{name}{model_separator}{k}": v
+                    for k, v in param.annotation.__fields__.items()
+                }
+            else:
+                new_param = param.annotation.__fields__
+            more_args = {**more_args, **new_param}
             for field in param.annotation.__fields__:
-                names[field] = param.annotation.__name__
+                parents[field] = param.annotation.__name__
         else:
             more_args[name] = param
+        return more_args, parents
+    return None
+
+
+def get_more_args(
+    func: Callable,
+    model_separator: str = "__",
+    *,
+    include_parent_model: bool = None,
+    more_args: Optional[Dict] = None,
+) -> Dict:
+    """Get the more_args dict."""
+    if more_args is None:
+        more_args = {}
+    more_args, parents = init_more_args(
+        func=func,
+        model_separator=model_separator,
+        include_parent_model=include_parent_model,
+        more_args=more_args,
+    )
 
     while any(
         hasattr(param.annotation, "__fields__") for name, param in more_args.items()
     ):
         keys_to_remove = []
         for name, param in more_args.items():
             if hasattr(param.annotation, "__fields__"):
                 # model parent lookup
-                names[param.annotation.__name__] = names[name]
 
                 if name not in param.annotation.__fields__.keys():
                     keys_to_remove.append(name)
-                more_args = {**more_args, **param.annotation.__fields__}
+
+                if include_parent_model:
+                    new_param = {
+                        f"{name}{model_separator}{k}": v
+                        for k, v in param.annotation.__fields__.items()
+                    }
+                else:
+                    new_param = param.annotation.__fields__
+
+                more_args = {**more_args, **new_param}
+
                 for field in param.annotation.__fields__:
-                    names[field] = param.annotation.__name__
+                    parents[field] = param.annotation.__name__
 
         for key in keys_to_remove:
             del more_args[key]
+    return more_args
 
-    wrapper.__doc__ = (
-        func.__doc__ or ""
-    ) + f"\nalso accepts {more_args.keys()} in place of person model"
-    raw_args = [
+
+def make_expanded_function(
+    func: Callable,
+    wrapper: Callable,
+    model_separator: str = "__",
+    *,
+    include_parent_model: bool = True,
+    typer: bool = False,
+):
+    """Return a new function with that accepts model fields."""
+    more_args = get_more_args(
+        func=func,
+        model_separator=model_separator,
+        include_parent_model=include_parent_model,
+    )
+
+    annotations = [
         make_annotation(
-            name,
-            field,
-            names=names,
+            name=name,
+            field=field,
+            model_separator=model_separator,
             typer=typer,
         )
         for name, field in more_args.items()
     ]
-    aargs = ", ".join([arg for arg in raw_args if "=" not in arg])
-    kwargs = ", ".join([arg for arg in raw_args if "=" in arg])
 
-    call_args = ",".join([f"{name}={name}" for name, field in more_args.items()])
+    # split raw_args into args and kwargs
+    aargs = ", ".join([arg for arg in annotations if "=" not in arg])
+    kwargs = ", ".join([arg for arg in annotations if "=" in arg])
+
+    # args to call the wrapper function with
+    call_args = ",".join([f"{name}={name}" for name in more_args])
 
-    def get_import(arg):
-        try:
-            if arg.type_.__module__ != "builtins":
-                return f"from {arg.type_.__module__} import {arg.type_.__name__}\n"
-        except AttributeError:
-            ...
-        return ""
+    # update the docscring
+    wrapper.__doc__ = (
+        func.__doc__ or ""
+    ) + f"\nalso accepts {more_args.keys()} in place of person model"
 
     new_func_str = f"""
+import typer
 def {func.__name__}({aargs}{', ' if aargs else ''}{kwargs}):
     '''{func.__doc__}'''
     return wrapper({call_args})
     """
+    new_func_str = black.format_str(src_contents=new_func_str, mode=black.FileMode())
+
+    pyflyby_log_level = os.getenv("PYFLYBY_LOG_LEVEL")
+    if pyflyby_log_level is None:
+        os.environ["PYFLYBY_LOG_LEVEL"] = "WARNING"
+
+    import pyflyby
+
     pyflyby.auto_import(new_func_str, locals())
+
     exec(new_func_str, locals(), globals())  # noqa: S102
     new_func = globals()[func.__name__]
 
     sig = inspect.signature(new_func)
     for param in sig.parameters.values():
         if hasattr(param.annotation, "__fields__"):
-            return make_signature(new_func, wrapper, typer=typer, more_args=more_args)
+            return make_expanded_function(
+                new_func,
+                wrapper,
+                typer=typer,
+                model_separator=model_separator,
+            )
     return new_func
-
-
-def expand_param(
-    param: inspect.Parameter,
-    kwargs: Dict[str, Any],
-    models: Optional[Dict[str, str]] = None,
-) -> Any:
-    """Further expands params with a Pydantic annotation, given a param.
-
-    Recursively creates an instance of any param.annotation that has __fields__
-    using the expanded kwargs.y:
-    using the expanded kwargs.
-    """
-    models = {}
-    for field_name, field in param.annotation.__fields__.items():
-        if hasattr(field.annotation, "__fields__"):
-            models[field_name] = expand_param(field, kwargs, models)
-    return param.annotation(**kwargs, **models)
-
-
-def expand_kwargs(func: Callable, kwargs: Dict[str, Any]) -> Dict[str, Any]:
-    """Expand kwargs with Pydantic annotations given a function.
-
-    Inspects the arguments of the func and expands any of the kwargs with a
-    Pydantic annotation, to add its fields to the kwargs.
-    """
-    sig = inspect.signature(func)
-    updated_kwargs = {}
-    for name, value in kwargs.items():
-        if name in sig.parameters:
-            updated_kwargs[name] = value
-
-    for name, param in sig.parameters.items():
-        # func wants this directly
-        # this should check isinstance, but it's not working
-        #
-        if name in kwargs and repr(param.annotation) == repr(kwargs[name]):
-            updated_kwargs[name] = kwargs[name]
-
-        # an instance was not passed in, create one with kwargs passed in
-        elif hasattr(param.annotation, "__fields__"):
-            updated_kwargs[name] = expand_param(param, kwargs)
-        # its something else so pass it
-    return updated_kwargs
```

### Comparing `engorgio-0.1.0.dev2/examples/person_cli.py` & `engorgio-0.2.0/examples/person_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 SPDX-FileCopyrightText: 2023-present Waylon S. Walker <waylon@waylonwalker.com>
 
 SPDX-License-Identifier: MIT
 """
 import typer
 
 from engorgio import engorgio
-from tests.models import Person
+from tests.models import Hero, Person
 
 app = typer.Typer(
     name="engorgio",
     help="a demo app",
 )
 
 
@@ -27,11 +27,21 @@
     """Get a person's information."""
     from rich import print
 
     print(thing)
     print(another)
 
     print(person)
+    return person
+
+
+@app.command()
+@engorgio(typer=True)
+def get_hero(hero: Hero) -> Hero:
+    """Get a hero"""
+    from rich import print
+
+    print(hero)
 
 
 if __name__ == "__main__":
-    typer.run(get_person)
+    app()
```

### Comparing `engorgio-0.1.0.dev2/tests/models.py` & `engorgio-0.2.0/tests/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 Classes:
 
 * `Alpha`: A class for representing an alpha value.
 * `Color`: A class for representing a color.
 * `Hair`: A class for representing hair.
 * `Person`: A class for representing a person.
 * `MyDate`: A class for representing a date.
+* `Hero`: A class for representing a hero.
+* `Pet`: A class for representing a pet.
+
+SPDX-FileCopyrightText: 2023-present Waylon S. Walker <waylon@waylonwalker.com>
+
+SPDX-License-Identifier: MIT
 
 """
 from dataclasses import dataclass
 import datetime
 from typing import Optional
 
 from polyfactory.factories import DataclassFactory
@@ -94,14 +100,23 @@
     )
     hair: Hair = Field(
         ...,
         description="The person's hair.",
     )
 
 
+class Pet(BaseModel):
+    name: str = Field(..., description="The pet's name.")
+
+
+class Hero(BaseModel):
+    name: str = Field(..., description="The hero's name.")
+    pet: Pet = Field(..., description="The hero's pet.")
+
+
 class AlphaFactory(ModelFactory[Alpha]):
 
     """A class for generating an alpha value."""
 
     __model__ = Alpha
 
 
@@ -122,14 +137,28 @@
 class PersonFactory(ModelFactory[Person]):
 
     """A class for generating a person."""
 
     __model__ = Person
 
 
+class HeroFactory(ModelFactory[Hero]):
+
+    """A class for generating a hero."""
+
+    __model__ = Hero
+
+
+class PetFactory(ModelFactory[Pet]):
+
+    """A class for generating a pet."""
+
+    __model__ = Pet
+
+
 class MyDate(BaseModel):
     date: datetime.datetime
 
 
 class MyDateFactory(ModelFactory[MyDate]):
     __model__ = MyDate
```

### Comparing `engorgio-0.1.0.dev2/tests/test_person.py` & `engorgio-0.2.0/tests/test_person.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,55 +6,79 @@
 """
 
 import inspect
 
 import pytest
 
 from engorgio import engorgio
+from tests import models
 
-from . import models
 
-# this one is broken
-# def test_no_pydantic() -> None:
-#     @engorgio()
-#     def get_person(alpha) -> None:
-#         """Mydocstring."""
+def test_no_pydantic() -> None:
+    @engorgio()
+    def get_person(alpha) -> None:
+        """Mydocstring."""
 
 
 def test_single_signature() -> None:
-    @engorgio()
+    @engorgio(include_parent_model=False)
     def get_person(alpha: models.Alpha) -> None:
         """Mydocstring."""
         return alpha
 
     sig = inspect.signature(get_person)
     params = sig.parameters
     assert "a" in params
 
     assert "alpha" not in params
     alpha = models.AlphaFactory().build()
     assert get_person(**alpha.dict()) == alpha
 
 
+def test_single_signature_with_parent() -> None:
+    @engorgio()
+    def get_person(alpha: models.Alpha) -> None:
+        """Mydocstring."""
+        return alpha
+
+    sig = inspect.signature(get_person)
+    params = sig.parameters
+    assert "alpha__a" in params
+
+    assert "alpha" not in params
+
+
 @pytest.mark.parametrize(
     "alpha",
     models.AlphaFactory().batch(size=5),
 )
 def test_single_instance(alpha: models.Alpha) -> None:
-    @engorgio()
+    @engorgio(include_parent_model=False)
     def get_person(alpha: models.Alpha) -> None:
         """Mydocstring."""
         return alpha
 
     assert get_person(**alpha.dict()) == alpha
-    # this should maybe work
 
 
-def test_one_nest_signature() -> None:
+@pytest.mark.parametrize(
+    "alpha",
+    models.AlphaFactory().batch(size=5),
+)
+def test_single_instance_with_parent(alpha: models.Alpha) -> None:
     @engorgio()
+    def get_person(alpha: models.Alpha) -> None:
+        """Mydocstring."""
+        return alpha
+
+    assert get_person(alpha__a=alpha.a) == alpha
+
+
+def test_one_nest_signature() -> None:
+    @engorgio(include_parent_model=False)
     def get_person(color: models.Color) -> None:
         """Mydocstring."""
         return color
 
     sig = inspect.signature(get_person)
     params = sig.parameters
     assert "r" in params
@@ -65,29 +89,56 @@
     assert "color" not in params
     assert "alpha" not in params
 
     color = models.ColorFactory().build()
     assert get_person(**color.dict(exclude={"alpha"}), **color.alpha.dict()) == color
 
 
+def test_one_nest_signature_with_parent() -> None:
+    @engorgio()
+    def get_person(color: models.Color) -> None:
+        """Mydocstring."""
+        return color
+
+    sig = inspect.signature(get_person)
+    params = sig.parameters
+    assert "color__r" in params
+    assert "color__g" in params
+    assert "color__b" in params
+    assert "color__alpha__a" in params
+    assert "a" not in params
+
+    assert "color" not in params
+    assert "alpha" not in params
+
+    # color = models.ColorFactory().build()
+    # assert (
+    #     get_person(
+    #         **color.dict(exclude={"alpha"}),
+    #         **{f"alpha__{k}": v for k, v in color.alpha.dict().items()},
+    #     ) ==
+    #     color
+    # )
+
+
 @pytest.mark.parametrize(
     "color",
     models.ColorFactory().batch(size=5),
 )
 def test_one_nest_instance(color: models.Color) -> None:
-    @engorgio()
+    @engorgio(include_parent_model=False)
     def get_person(color: models.Color) -> None:
         """Mydocstring."""
         return color
 
     assert get_person(**color.dict(exclude={"alpha"}), **color.alpha.dict()) == color
 
 
 def test_two_nest_signature() -> None:
-    @engorgio()
+    @engorgio(include_parent_model=False)
     def get_hair(hair: models.Hair) -> None:
         """Mydocstring."""
         return hair
 
     sig = inspect.signature(get_hair)
     params = sig.parameters
     assert "length" in params
@@ -112,15 +163,15 @@
 
 
 @pytest.mark.parametrize(
     "hair",
     models.HairFactory().batch(size=5),
 )
 def test_two_nest_instance(hair: models.Hair) -> None:
-    @engorgio()
+    @engorgio(include_parent_model=False)
     def get_hair(hair: models.Hair) -> None:
         """Mydocstring."""
         return hair
 
     assert (
         get_hair(
             **hair.dict(exclude={"color"}),
@@ -128,15 +179,15 @@
             **hair.color.alpha.dict(),
         ) ==
         hair
     )
 
 
 def test_three_nest_signature() -> None:
-    @engorgio()
+    @engorgio(include_parent_model=False)
     def get_person(person: models.Person) -> None:
         """Mydocstring."""
         return person
 
     sig = inspect.signature(get_person)
     params = sig.parameters
     assert "name" in params
@@ -169,15 +220,15 @@
 
 
 @pytest.mark.parametrize(
     "person",
     models.PersonFactory().batch(size=5),
 )
 def test_three_nest_instance(person: models.Person) -> None:
-    @engorgio()
+    @engorgio(include_parent_model=False)
     def get_person(person: models.Person) -> None:
         """Mydocstring."""
         return person
 
     assert (
         get_person(
             **person.dict(exclude={"hair"}),
@@ -186,15 +237,15 @@
             **person.hair.color.alpha.dict(),
         ) ==
         person
     )
 
 
 def test_mydate() -> None:
-    @engorgio()
+    @engorgio(include_parent_model=False)
     def get_mydate(date: models.MyDate) -> None:
         """Mydocstring."""
         return date
 
     sig = inspect.signature(get_mydate)
     params = sig.parameters
     assert "date" in params
@@ -204,15 +255,15 @@
 
 
 @pytest.mark.parametrize(
     "date",
     models.MyDateFactory().batch(size=5),
 )
 def test_mydate_instance(date: models.MyDate) -> None:
-    @engorgio()
+    @engorgio(include_parent_model=False)
     def get_mydate(date: models.MyDate) -> None:
         """Mydocstring."""
         return date
 
     assert get_mydate(**date.dict()) == date
```

### Comparing `engorgio-0.1.0.dev2/.gitignore` & `engorgio-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev2/LICENSE.txt` & `engorgio-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev2/README.md` & `engorgio-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # engorgio
 
+<img src="https://github.com/WaylonWalker/engorgio/assets/22648375/e2577efd-cb4b-417a-8139-ef2a7d75c8d9" width=100%>
+
+Expands function arguments into fields.
+
 https://user-images.githubusercontent.com/22648375/235036031-a9dc6589-e350-4a18-9114-6568cb362f74.mp4
 
+
 ## Installation
 
 pypi package to come if this works out, and I can decide
 what to call it. I think its possible to do this for other
 objects like dataclasses as well.
 
 ```console
```

### Comparing `engorgio-0.1.0.dev2/pyproject.toml` & `engorgio-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `engorgio-0.1.0.dev2/PKG-INFO` & `engorgio-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engorgio
-Version: 0.1.0.dev2
+Version: 0.2.0
 Summary: Expand pydantic function arguments by casting the engorgio decorator
 Project-URL: Documentation, https://github.com/waylonwalker/engorgio#readme
 Project-URL: Issues, https://github.com/waylonwalker/engorgio/issues
 Project-URL: Source, https://github.com/waylonwalker/engorgio
 Project-URL: Changelog, https://github.com/WaylonWalker/engorgio/blob/main/CHANGELOG.md
 Author-email: "Waylon S. Walker" <waylon@waylonwalker.com>
 License-Expression: MIT
@@ -24,16 +24,21 @@
 Requires-Dist: rich
 Requires-Dist: textual
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 # engorgio
 
+<img src="https://github.com/WaylonWalker/engorgio/assets/22648375/e2577efd-cb4b-417a-8139-ef2a7d75c8d9" width=100%>
+
+Expands function arguments into fields.
+
 https://user-images.githubusercontent.com/22648375/235036031-a9dc6589-e350-4a18-9114-6568cb362f74.mp4
 
+
 ## Installation
 
 pypi package to come if this works out, and I can decide
 what to call it. I think its possible to do this for other
 objects like dataclasses as well.
 
 ```console
```

