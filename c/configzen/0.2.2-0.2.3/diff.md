# Comparing `tmp/configzen-0.2.2.tar.gz` & `tmp/configzen-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.2.2.tar", max compression
+gzip compressed data, was "configzen-0.2.3.tar", max compression
```

## Comparing `configzen-0.2.2.tar` & `configzen-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.2/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.2/configzen/__main__.py
--rw-r--r--   0        0        0    60641 2023-05-31 04:04:21.671560 configzen-0.2.2/configzen/config.py
--rw-r--r--   0        0        0     2460 2023-05-31 03:37:38.318229 configzen-0.2.2/configzen/errors.py
--rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.2.2/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.2/configzen/py.typed
--rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.2.2/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.2/LICENSE
--rw-r--r--   0        0        0     1154 2023-05-31 04:06:30.940657 configzen-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.2/README.md
--rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.3/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.3/configzen/__main__.py
+-rw-r--r--   0        0        0    67072 2023-06-05 06:56:38.878732 configzen-0.2.3/configzen/config.py
+-rw-r--r--   0        0        0     2460 2023-06-05 06:53:12.902541 configzen-0.2.3/configzen/errors.py
+-rw-r--r--   0        0        0    30567 2023-06-05 06:53:19.290433 configzen-0.2.3/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.3/configzen/py.typed
+-rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.3/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1154 2023-06-05 06:58:57.556277 configzen-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.3/README.md
+-rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.3/PKG-INFO
```

### Comparing `configzen-0.2.2/configzen/__main__.py` & `configzen-0.2.3/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.2/configzen/config.py` & `configzen-0.2.3/configzen/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,29 +83,30 @@
 import pydantic
 from anyconfig.utils import filter_options, is_dict_like, is_list_like
 from pydantic.fields import (  # type: ignore[attr-defined]
     ModelField,
     make_generic_validator,
 )
 from pydantic.json import ENCODERS_BY_TYPE
-from pydantic.main import ModelMetaclass, BaseModel
+from pydantic.main import BaseModel, ModelMetaclass
 from pydantic.utils import ROOT_KEY
 
 from configzen.errors import (
     ConfigAccessError,
     InternalConfigError,
     ResourceLookupError,
     UnspecifiedParserError,
     pretty_syntax_error,
 )
 from configzen.processor import EXPORT, DirectiveContext, Processor
 from configzen.typedefs import (
     AsyncConfigIO,
     ConfigIO,
     ConfigModelT,
+    IncludeExcludeT,
     NormalizedResourceT,
     RawResourceT,
     SupportsRoute,
     T,
 )
 
 try:
@@ -125,15 +126,17 @@
     "reload",
     "reload_async",
     "pre_serialize",
     "with_pre_serialize",
     "post_deserialize",
     "with_post_deserialize",
     "export",
+    "export_async",
     "with_exporter",
+    "with_async_exporter",
 )
 
 _URL_SCHEMES: set[str] = set(
     urllib.parse.uses_relative + urllib.parse.uses_netloc + urllib.parse.uses_params
 ) - {""}
 CONTEXT: str = "__context__"
 TOKEN: str = "__context_token__"
@@ -198,16 +201,16 @@
     if dataclasses.is_dataclass(obj):
         return pre_serialize(dataclasses.asdict(obj))
     if _is_namedtuple(obj):
         return _ps_namedtuple(obj)
     return obj
 
 
-for obj_type, encoder in ENCODERS_BY_TYPE.items():
-    pre_serialize.register(obj_type, encoder)
+for obj_type, obj_encoder in ENCODERS_BY_TYPE.items():
+    pre_serialize.register(obj_type, obj_encoder)
 
 
 def with_pre_serialize(
     func: collections.abc.Callable[[T], Any], cls: type[T] | None = None
 ) -> type[T] | Any:
     """
     Register a pre-serialization converter function for a type.
@@ -314,14 +317,30 @@
     obj
     """
     if isinstance(obj, ConfigModel) and not _exporting.get():
         return obj.export(**kwargs)
     return cast(dict[str, Any], obj.dict(**kwargs))
 
 
+@functools.singledispatch
+async def export_async(obj: Any, **kwargs: Any) -> dict[str, Any]:
+    """
+    Export a ConfigModel to a safely-serializable format.
+    Register a custom exporter for a type using the `with_exporter` decorator,
+    which can help to exclude particular values from the export if needed.
+
+    Parameters
+    ----------
+    obj
+    """
+    if isinstance(obj, ConfigModel) and not _exporting.get():
+        return await obj.export_async(**kwargs)
+    return cast(dict[str, Any], await obj.dict_async(**kwargs))
+
+
 def with_exporter(
     func: collections.abc.Callable[[ConfigModelT], dict[str, Any]],
     cls: type[ConfigModelT] | None = None,
 ) -> type[ConfigModelT] | Any:
     """
     Register a custom exporter for a type.
 
@@ -332,14 +351,43 @@
     cls
         The type to register the exporter for.
     """
     if cls is None:
         return functools.partial(with_exporter, func)
 
     export.register(cls, func)
+    if export_async.dispatch(cls) is export_async:
+
+        async def default_async_func(obj: Any) -> Any:
+            return func(obj)
+
+        export_async.register(cls, default_async_func)
+    return cls
+
+
+def with_async_exporter(
+    func: collections.abc.Callable[
+        [ConfigModelT], collections.abc.Coroutine[Any, Any, dict[str, Any]]
+    ],
+    cls: type[ConfigModelT] | None = None,
+) -> type[ConfigModelT] | Any:
+    """
+    Register a custom exporter for a type.
+
+    Parameters
+    ----------
+    func
+        The exporter function.
+    cls
+        The type to register the exporter for.
+    """
+    if cls is None:
+        return functools.partial(with_exporter, func)
+
+    export_async.register(cls, func)
     return cls
 
 
 @pre_serialize.register(list)
 def _ps_list(obj: list[Any]) -> list[Any]:
     """
     Convert a list to safely-serializable form.
@@ -631,14 +679,34 @@
         The loaded configuration.
         """
         dict_config = self.load_into_dict(blob, ac_parser=ac_parser, **kwargs)
         if dict_config is None:
             dict_config = {}
         return config_class.parse_obj(dict_config)
 
+    def _preload_into_dict(
+        self,
+        blob: str,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> dict[str, Any]:
+        if ac_parser is None:
+            ac_parser = self.ac_parser
+        kwargs = self.load_options | kwargs
+        loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
+            blob, ac_parser=ac_parser, **kwargs
+        )
+        if not isinstance(loaded, collections.abc.Mapping):
+            msg = (
+                f"Expected a mapping as a result of loading {self.resource}, "
+                f"got {type(loaded).__name__}."
+            )
+            raise TypeError(msg)
+        return dict(loaded)
+
     def load_into_dict(
         self,
         blob: str,
         ac_parser: str | None = None,
         *,
         preprocess: bool = True,
         **kwargs: Any,
@@ -658,30 +726,48 @@
         **kwargs
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration dictionary.
         """
-        if ac_parser is None:
-            ac_parser = self.ac_parser
-        kwargs = self.load_options | kwargs
-        loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
-            blob, ac_parser=ac_parser, **kwargs
-        )
-        if not isinstance(loaded, collections.abc.Mapping):
-            msg = (
-                f"Expected a mapping as a result of loading {self.resource}, "
-                f"got {type(loaded).__name__}."
-            )
-            raise TypeError(msg)
-        loaded = dict(loaded)
+        loaded = self._preload_into_dict(blob, ac_parser, **kwargs)
         if preprocess:
             loaded = self.processor_class(self, loaded).preprocess()
-        return cast(dict[str, Any], loaded)
+        return loaded
+
+    async def load_into_dict_async(
+        self,
+        blob: str,
+        ac_parser: str | None = None,
+        *,
+        preprocess: bool = True,
+        **kwargs: Any,
+    ) -> dict[str, Any]:
+        """
+        Load the configuration into a dictionary asynchronously.
+
+        Parameters
+        ----------
+        blob
+            The configuration to load.
+        ac_parser
+            The name of the anyconfig parser to use for loading the configuration.
+        preprocess
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration dictionary.
+        """
+        loaded = self._preload_into_dict(blob, ac_parser, **kwargs)
+        if preprocess:
+            loaded = await self.processor_class(self, loaded).preprocess_async()
+        return loaded
 
     def dump_config(
         self,
         config: ConfigModelT,
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> str:
@@ -704,14 +790,43 @@
         if ac_parser is None:
             ac_parser = self.ac_parser
         if ac_parser == "json" and self.use_pydantic_json:
             kwargs = filter_options(self.JSON_KWARGS, self.dump_options | kwargs)
             return config.json(**kwargs)
         return self.dump_data(export(config), ac_parser=ac_parser, **kwargs)
 
+    async def dump_config_async(
+        self,
+        config: ConfigModelT,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> str:
+        """
+        Dump the configuration to a string.
+
+        Parameters
+        ----------
+        config
+            The configuration to dump.
+        ac_parser
+            The name of the anyconfig parser to use for saving the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.dumps()`.
+
+        Returns
+        -------
+        The dumped configuration.
+        """
+        if ac_parser is None:
+            ac_parser = self.ac_parser
+        if ac_parser == "json" and self.use_pydantic_json:
+            kwargs = filter_options(self.JSON_KWARGS, self.dump_options | kwargs)
+            return await config.json_async(**kwargs)
+        return self.dump_data(await export_async(config), ac_parser=ac_parser, **kwargs)
+
     def dump_data(
         self,
         data: dict[str, Any],
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> str:
         """
@@ -778,17 +893,45 @@
                     # Moreover, we want to allow the file to be opened
                     # from a file descriptor, not supported by Path().
                     open(self.resource, **kwds),  # noqa: PTH123, SIM115
                 )
             return cast(ConfigIO, pathlib.Path(self.resource).open(**kwds))
         return cast(ConfigIO, self.resource)
 
+    def open_resource_async(self, **kwds: Any) -> AsyncConfigIO:
+        """
+        Open the configuration file asynchronously.
+
+        Parameters
+        ----------
+        **kwds
+            Keyword arguments to pass to the opening routine.
+
+        Returns
+        -------
+        The opened resource.
+        """
+        if self.is_url:
+            msg = "asynchronous URL opening is not supported"
+            raise NotImplementedError(msg)
+        if not AIOFILES_AVAILABLE:
+            msg = (
+                "aiofiles is not available, cannot open file "
+                "asynchronously (install with `pip install aiofiles`)"
+            )
+            raise RuntimeError(msg)
+        if isinstance(self.resource, (int, pathlib.Path)):
+            kwds = filter_options(self.OPEN_KWARGS, kwds)
+            return aiofiles.open(self.resource, **kwds)
+        raise RuntimeError("cannot open resource asynchronously")
+
     def processor_open_resource(self, **kwargs: Any) -> ConfigIO:
         """
-        Called by the processor to open a configuration resource with reading intention.
+        Called by the processor to open a configuration resource
+        with the reading intention.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the opening routine.
             For URLs, these are passed to ``urllib.request.urlopen()``.
             For local files, these are passed to ``builtins.open()``.
@@ -796,40 +939,32 @@
         Returns
         -------
         The opened resource.
         """
         kwargs = self._get_default_kwargs("read", kwargs)
         return self.open_resource(**kwargs)
 
-    def open_resource_async(self, **kwds: Any) -> AsyncConfigIO:
+    def processor_open_resource_async(self, **kwargs: Any) -> AsyncConfigIO:
         """
-        Open the configuration file asynchronously.
+        Called by the processor to open a configuration resource asynchronously
+        with the reading intention.
 
         Parameters
         ----------
-        **kwds
+        **kwargs
             Keyword arguments to pass to the opening routine.
+            For URLs, these are passed to ``urllib.request.urlopen()``.
+            For local files, these are passed to ``builtins.open()``.
 
         Returns
         -------
         The opened resource.
         """
-        if self.is_url:
-            msg = "asynchronous URL opening is not supported"
-            raise NotImplementedError(msg)
-        if not AIOFILES_AVAILABLE:
-            msg = (
-                "aiofiles is not available, cannot open file "
-                "asynchronously (install with `pip install aiofiles`)"
-            )
-            raise RuntimeError(msg)
-        if isinstance(self.resource, (int, pathlib.Path)):
-            kwds = filter_options(self.OPEN_KWARGS, kwds)
-            return aiofiles.open(self.resource, **kwds)
-        raise RuntimeError("cannot open resource asynchronously")
+        kwargs = self._get_default_kwargs("read", kwargs)
+        return self.open_resource_async(**kwargs)
 
     def _get_default_kwargs(
         self,
         method: Literal["read", "write"],
         kwargs: dict[str, Any] | None = None,
     ) -> dict[str, Any]:
         if not kwargs:
@@ -1703,30 +1838,99 @@
         The exported configuration model.
         """
         tok = _exporting.set(True)  # noqa: FBT003
         ctx = contextvars.copy_context()
         _exporting.reset(tok)
         return ctx.run(self.dict, **kwargs)
 
-    @no_type_check
-    def _iter(
+    async def export_async(self, **kwargs: Any) -> dict[str, Any]:
+        """
+        Export the configuration model.
+
+        Returns
+        -------
+        The exported configuration model.
+        """
+        tok = _exporting.set(True)  # noqa: FBT003
+        ctx = contextvars.copy_context()
+        _exporting.reset(tok)
+        return await ctx.run(self.dict_async, **kwargs)
+
+    async def dict_async(self, **kwargs: Any) -> dict[str, Any]:
+        """
+        Get the dictionary representation of the configuration model.
+
+        Returns
+        -------
+        The dictionary representation of the configuration model.
+        """
+        return dict(await self._iter_async(to_dict=True, **kwargs))
+
+    async def json_async(  # noqa: PLR0913
+        self,
+        include: IncludeExcludeT = None,
+        exclude: IncludeExcludeT = None,
+        *,
+        by_alias: bool = False,
+        exclude_unset: bool = False,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        encoder: collections.abc.Callable[[Any], Any] | None = None,
+        models_as_dict: bool = True,
+        **dumps_kwargs: Any,
+    ) -> str:
+        encoder = cast(
+            collections.abc.Callable[[Any], Any], encoder or self.__json_encoder__
+        )
+        data = dict(
+            await self._iter_async(
+                to_dict=models_as_dict,
+                by_alias=by_alias,
+                include=include,
+                exclude=exclude,
+                exclude_unset=exclude_unset,
+                exclude_defaults=exclude_defaults,
+                exclude_none=exclude_none,
+            )
+        )
+        if self.__custom_root_type__:
+            data = data[ROOT_KEY]
+        return self.__config__.json_dumps(data, default=encoder, **dumps_kwargs)
+
+    def _iter(  # type: ignore[override]
         self, **kwargs: Any
     ) -> collections.abc.Iterator[tuple[str, Any]]:
         if kwargs.get("to_dict", False) and _exporting.get():
             state = {}
             for key, value in super()._iter(**kwargs):
                 state[key] = value
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
                 context.manager.processor_class.export(state, metadata=metadata)
             yield from state.items()
         else:
             yield from super()._iter(**kwargs)
 
+    async def _iter_async(
+        self, **kwargs: Any
+    ) -> collections.abc.Iterator[tuple[str, Any]]:
+        if kwargs.get("to_dict", False) and _exporting.get():
+            state = {}
+            for key, value in super()._iter(**kwargs):
+                state[key] = value
+            metadata = getattr(self, EXPORT, None)
+            if metadata:
+                context = get_context(self)
+                await context.manager.processor_class.export_async(
+                    state, metadata=metadata
+                )
+            return ((key, value) for key, value in state.items())
+        return super()._iter(**kwargs)
+
     @classmethod
     @no_type_check
     def _get_value(cls, value: Any, *, to_dict: bool, **kwds: Any) -> Any:
         if _exporting.get():
             exporter = export.dispatch(type(value))
             if (
                 isinstance(value, BaseModel) or exporter != export.dispatch(object)
@@ -1963,15 +2167,15 @@
         -------
         self
         """
         manager = cls._resolve_manager(resource, create_if_missing=create_if_missing)
         context = Context(manager)  # type: Context[ConfigModelT]
         current_context.set(context)
         local = contextvars.copy_context()
-        config = manager.read(config_class=cls, **kwargs)
+        config = await manager.read_async(config_class=cls, **kwargs)
         setattr(config, LOCAL, local)
         context.owner = config
         return config
 
     async def reload_async(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
         """
         Reload the configuration file asynchronously.
@@ -2021,15 +2225,15 @@
         context = get_context(self)
         if context.owner is self:
             if write_kwargs is None:
                 write_kwargs = {}
             tok = _exporting.set(True)  # noqa: FBT003
             ctx = contextvars.copy_context()
             _exporting.reset(tok)
-            blob = ctx.run(context.manager.dump_config, self, **kwargs)
+            blob = await ctx.run(context.manager.dump_config_async, self, **kwargs)
             result = await self.write_async(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
         return await save_async(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
             **kwargs,
```

### Comparing `configzen-0.2.2/configzen/errors.py` & `configzen-0.2.3/configzen/errors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module contains all the custom errors raised by _configzen_."""
 
 from __future__ import annotations
 
-import contextlib
 import collections.abc
+import contextlib
 from typing import TYPE_CHECKING, Any
 
 import anyconfig
 
 if TYPE_CHECKING:
     from configzen.config import ConfigManager
     from configzen.typedefs import ConfigModelT
```

### Comparing `configzen-0.2.2/configzen/processor.py` & `configzen-0.2.3/configzen/processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
+import asyncio
 import copy
 import dataclasses
 import enum
 import pathlib
 from collections.abc import Callable
 from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
 
 from anyconfig.utils import is_dict_like, is_list_like
 
 from configzen.errors import (
     ConfigPreprocessingError,
     InternalConfigError,
     pretty_syntax_error,
 )
-from configzen.typedefs import ConfigModelT
+from configzen.typedefs import ConfigModelT, SupportsRoute
 
 if TYPE_CHECKING:
     from configzen.config import BaseContext, ConfigManager
 
 __all__ = (
     "DirectiveContext",
     "directive",
@@ -26,38 +27,47 @@
 )
 
 
 DirectiveT = TypeVar("DirectiveT")
 
 EXPORT: str = "__configzen_export__"
 EXECUTES_DIRECTIVES: str = "__configzen_executes_directives__"
+EXECUTES_DIRECTIVES_ASYNC: str = "__configzen_executes_directives_async__"
 
 
 def directive(
     name: str | enum.Enum,
+    *,
+    asynchronous: bool | None = None,
 ) -> Callable[..., Any]:
     """
     Decorator for creating processor directives.
 
     Parameters
     ----------
     name
         The name of the directive.
+    asynchronous
+        Whether the decorated directive function is asynchronous.
 
     Returns
     -------
     The decorated function.
     """
     if isinstance(name, enum.Enum):
         name = name.value.casefold()
 
     def decorator(func: Any) -> Any:
-        if not hasattr(func, EXECUTES_DIRECTIVES):
-            setattr(func, EXECUTES_DIRECTIVES, set())
-        getattr(func, EXECUTES_DIRECTIVES).add(name)
+        nonlocal asynchronous
+        if asynchronous is None:
+            asynchronous = asyncio.iscoroutinefunction(func)
+        attr = EXECUTES_DIRECTIVES_ASYNC if asynchronous else EXECUTES_DIRECTIVES
+        if not hasattr(func, attr):
+            setattr(func, attr, set())
+        getattr(func, attr).add(name)
         return func
 
     return decorator
 
 
 @dataclasses.dataclass
 class DirectiveContext:
@@ -115,15 +125,15 @@
 
 class ArgumentSyntaxError(ValueError):
     """
     Raised when there is a syntax error in an argument.
     """
 
 
-def _parse_argument_string_impl(
+def _parse_argument_string_impl(  # noqa: C901, PLR0912, PLR0915
     raw_argument_string: str,
     tokens: type[Tokens] = Tokens,
 ) -> list[str]:
     prev_char = None
     string_ctx = None
     escape_ctx = False
     arguments: list[str] = []
@@ -267,23 +277,24 @@
     dict_config
         The dictionary config to parse and update.
     directive_prefix
         The prefix for directives.
     """
 
     _directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
+    _async_directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
     directive_prefix: ClassVar[str]
     extension_prefix: ClassVar[str]
 
     def __init__(
         self,
-        resource: ConfigManager[ConfigModelT],
+        manager: ConfigManager[ConfigModelT],
         dict_config: dict[str, Any],
     ) -> None:
-        self.manager = resource
+        self.manager = manager
         self.dict_config = dict_config
 
     @classmethod
     def export(
         cls,
         state: Any,
         *,
@@ -310,21 +321,71 @@
             else:
                 cls.export(list(state.values()), metadata=None)
         elif is_list_like(state):
             for item in state:
                 cls.export(item, metadata=None)
 
     @classmethod
+    async def export_async(
+        cls,
+        state: Any,
+        *,
+        metadata: ExportMetadata[ConfigModelT] | None = None,
+    ) -> None:
+        """
+        Export the state asynchronously.
+
+        Parameters
+        ----------
+        state
+            The state to export.
+        metadata
+            The metadata of the substitution.
+        """
+        if is_dict_like(state):
+            if metadata is None:
+                from configzen.config import CONTEXT
+
+                state.pop(CONTEXT, None)
+                metadata = state.pop(EXPORT, None)
+            if metadata:
+                await cls._export_async(state, metadata)
+            else:
+                await cls.export_async(list(state.values()), metadata=None)
+        elif is_list_like(state):
+            for item in state:
+                await cls.export_async(item, metadata=None)
+
+    @classmethod
     def _export(
         cls,
         state: Any,
         metadata: ExportMetadata[ConfigModelT],
     ) -> None:
         raise NotImplementedError
 
+    @classmethod
+    async def _export_async(
+        cls,
+        state: Any,
+        metadata: ExportMetadata[ConfigModelT],
+    ) -> None:
+        raise NotImplementedError
+
+    async def preprocess_async(self) -> dict[str, Any]:
+        """
+        Parse the dictionary config and return the parsed config,
+        ready for instantiating the model.
+
+        Returns
+        -------
+        The parsed config.
+        """
+        return cast(dict[str, Any], await self._preprocess_async(self.dict_config))
+
     def preprocess(self) -> dict[str, Any]:
         """
         Parse the dictionary config and return the parsed config,
         ready for instantiating the model.
 
         Returns
         -------
@@ -372,32 +433,91 @@
                 self._call_directive(context)
                 new_container = self._preprocess(context.container)
                 result |= new_container
             else:
                 result[key] = self._preprocess(value)
         return result
 
+    async def _preprocess_async(self, container: Any) -> Any:
+        if not is_dict_like(container):
+            if is_list_like(container):
+                return [await self._preprocess_async(v) for v in container]
+            return container
+
+        result: dict[str, Any] = {}
+
+        for key, value in sorted(
+            cast(dict[str, Any], container).items(),
+            key=lambda item: item[0] == self.directive_prefix,
+        ):
+            if key.startswith(self.extension_prefix):
+                actual_key = key.lstrip(self.extension_prefix)
+                overridden = result.get(actual_key, {})
+                if not is_dict_like(overridden):
+                    raise ConfigPreprocessingError(
+                        f"{self.extension_prefix} can be used only for overriding "
+                        f"dictionary sections but item at {actual_key!r} "
+                        f"is not a dictionary"
+                    )
+                replacement = overridden | value
+                result[actual_key] = await self._preprocess_async(replacement)
+            elif key.startswith(self.directive_prefix):
+                directive_name, arguments = parse_directive_call(
+                    self.directive_prefix, key
+                )
+                context_container = container.copy()
+                del context_container[key]
+                context = DirectiveContext(
+                    directive=directive_name,
+                    key=key,
+                    prefix=self.directive_prefix,
+                    arguments=arguments,
+                    snippet=value,
+                    container=context_container,
+                )
+                await self._call_directive_async(context)
+                new_container = await self._preprocess_async(context.container)
+                result |= new_container
+            else:
+                result[key] = await self._preprocess_async(value)
+        return result
+
     def _call_directive(self, context: DirectiveContext) -> None:
         handler = self._directive_handlers.get(context.directive)
         if handler is None:
             raise ConfigPreprocessingError(
                 f"unknown preprocessing directive: {context.directive!r}"
             )
         handler(self, context)
 
+    async def _call_directive_async(self, context: DirectiveContext) -> None:
+        handler = self._async_directive_handlers.get(context.directive)
+        if handler is None:
+            raise ConfigPreprocessingError(
+                f"unknown preprocessing directive: {context.directive!r}"
+            )
+        await handler(self, context)
+
     def __init_subclass__(cls, **kwargs: Any) -> None:
         super().__init_subclass__(**kwargs)
         if cls._directive_handlers is None:
             cls._directive_handlers = {}
         else:
             cls._directive_handlers = cls._directive_handlers.copy()
+        if cls._async_directive_handlers is None:
+            cls._async_directive_handlers = {}
+        else:
+            cls._async_directive_handlers = cls._async_directive_handlers.copy()
         for _name, func in cls.__dict__.items():
             if hasattr(func, EXECUTES_DIRECTIVES):
                 for directive_name in getattr(func, EXECUTES_DIRECTIVES):
                     cls._directive_handlers[directive_name] = func
+            elif hasattr(func, EXECUTES_DIRECTIVES_ASYNC):
+                for directive_name in getattr(func, EXECUTES_DIRECTIVES_ASYNC):
+                    cls._async_directive_handlers[directive_name] = func
 
     @classmethod
     def register_directive(cls, name: str, func: Any) -> None:
         if cls._directive_handlers is None:
             cls._directive_handlers = {}
         cls._directive_handlers[name] = func
 
@@ -447,15 +567,15 @@
     directive_prefix = "^"
     extension_prefix = "+"
     route_separator: ClassVar[str] = ":"
 
     @directive(Directives.EXTEND)
     def extend(self, ctx: DirectiveContext) -> None:
         """
-        extend a configuration with another configuration.
+        Extend a configuration with another configuration.
         Recursively preprocess the referenced configuration.
         Preserve information about the referenced configuration.
 
         Visual example
         --------------
 
         With `base.yaml` containing:
@@ -477,15 +597,15 @@
 
         ```yaml
         ^extend: base.yaml
         +section:
           foo: 3
         ```
         """
-        return self._substitute(ctx, preprocess=True, preserve=True)
+        self._substitute(ctx, preprocess=True, preserve=True)
 
     @directive(Directives.INCLUDE)
     def include(self, ctx: DirectiveContext) -> None:
         """
         Include a configuration in another configuration.
         Recursively preprocess the referenced configuration.
         Do not preserve information about the referenced configuration.
@@ -521,15 +641,15 @@
         ```yaml
         ^extend: biz.yaml
         +section:
           bar: 2
           foo: 3
         ```
         """
-        return self._substitute(ctx, preprocess=True, preserve=False)
+        self._substitute(ctx, preprocess=True, preserve=False)
 
     @directive(Directives.COPY)
     def copy(self, ctx: DirectiveContext) -> None:
         """
         Copy a configuration and paste into another configuration.
         This is just a literal copy-paste.
         Do not preprocess the referenced configuration.
@@ -557,35 +677,59 @@
 
         ```yaml
         section:
           foo: 3
           bar: 2
         ```
         """
-        return self._substitute(ctx, preprocess=False, preserve=False)
+        self._substitute(ctx, preprocess=False, preserve=False)
 
-    def _substitute(
-        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
-    ) -> None:
-        from configzen.config import CONTEXT, Context, at
+    @directive(Directives.EXTEND)
+    async def extend_async(self, ctx: DirectiveContext) -> None:
+        """
+        Extend a configuration with another configuration asynchronously.
+        For more information see `extend`.
+        """
+        await self._substitute_async(ctx, preprocess=True, preserve=True)
 
+    @directive(Directives.EXTEND)
+    async def include_async(self, ctx: DirectiveContext) -> None:
+        """
+        Include a configuration in another configuration asynchronously.
+        For more information see `include`.
+        """
+        await self._substitute_async(ctx, preprocess=True, preserve=False)
+
+    @directive(Directives.COPY)
+    async def copy_async(self, ctx: DirectiveContext) -> None:
+        """
+        Copy a configuration and paste into another configuration asynchronously.
+        For more information see `copy`.
+        """
+        await self._substitute_async(ctx, preprocess=False, preserve=False)
+
+    def _get_substitution_info(
+        self, ctx: DirectiveContext, *, preserve: bool
+    ) -> tuple[
+        ConfigManager[ConfigModelT], ConfigManager[ConfigModelT], SupportsRoute | None
+    ]:
         manager_class = type(self.manager)
 
         if len(ctx.arguments):
             msg = f"{ctx.directive!r} directive takes no () arguments"
             raise ConfigPreprocessingError(msg)
 
         if preserve and ctx.has_duplicates(require_same_arguments=False):
             msg = (
                 f"using more than one {ctx.directive!r} directive "
                 "in the same section is not allowed"
             )
             raise ConfigPreprocessingError(msg)
 
-        manager, substitution_route = manager_class.from_directive_context(
+        manager, route = manager_class.from_directive_context(
             ctx, route_separator=self.route_separator
         )
 
         if manager.resource == self.manager.resource:
             raise ConfigPreprocessingError(
                 f"{manager.resource} tried to {ctx.directive!r} on itself"
             )
@@ -594,33 +738,78 @@
         if manager.relative:
             parent = cast(pathlib.Path, self.manager.resource).parent
             child = cast(pathlib.Path, manager.resource)
 
             actual_manager = copy.copy(manager)
             actual_manager.resource = parent / child
 
-        with actual_manager.processor_open_resource() as reader:
-            substituted = manager.load_into_dict(reader.read(), preprocess=preprocess)
+        return actual_manager, manager, route
+
+    def _substitute(
+        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
+    ) -> None:
+        actual_mgr, mgr, route = self._get_substitution_info(ctx, preserve=preserve)
+
+        with actual_mgr.processor_open_resource() as reader:
+            source = mgr.load_into_dict(reader.read(), preprocess=preprocess)
+
+        self._substitute_impl(
+            ctx,
+            route,
+            source=source,
+            manager=mgr,
+            preprocess=preprocess,
+            preserve=preserve,
+        )
+
+    async def _substitute_async(
+        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
+    ) -> None:
+        actual_mgr, mgr, route = self._get_substitution_info(ctx, preserve=preserve)
+
+        async with actual_mgr.processor_open_resource_async() as reader:
+            source = mgr.load_into_dict(await reader.read(), preprocess=preprocess)
+
+        self._substitute_impl(
+            ctx,
+            route,
+            source=source,
+            manager=mgr,
+            preprocess=preprocess,
+            preserve=preserve,
+        )
 
-        if substitution_route:
-            substituted = at(substituted, substitution_route, manager=manager)
-            if not is_dict_like(substituted):
+    @staticmethod
+    def _substitute_impl(  # noqa: PLR0913
+        ctx: DirectiveContext,
+        route: SupportsRoute | None,
+        *,
+        source: dict[str, Any],
+        manager: ConfigManager[ConfigModelT],
+        preprocess: bool,
+        preserve: bool,
+    ) -> None:
+        from configzen.config import CONTEXT, Context, at
+
+        if route:
+            source = at(source, route, manager=manager)
+            if not is_dict_like(source):
                 raise ConfigPreprocessingError(
-                    f"imported item {substitution_route!r} "
+                    f"imported item {route!r} "
                     f"from {manager.resource} is not a dictionary"
                 )
 
         context: Context[ConfigModelT] = Context(manager)
-        ctx.container = substituted | ctx.container
+        ctx.container = source | ctx.container
 
         if preserve:
             ctx.container |= {
                 CONTEXT: context,
                 EXPORT: ExportMetadata(
-                    route=str(substitution_route),
+                    route=str(route),
                     context=context,
                     preprocess=preprocess,
                     key_order=list(ctx.container),
                 ),
             }
 
     @classmethod
@@ -684,22 +873,116 @@
             elif counterpart_value != value:
                 overrides[key] = counterpart_value
                 del substituted_values[key]
 
         for value in state.values():
             cls.export(value, metadata=None)
 
-        # TODO: Optimize. We iterate over the same about 3-4 times.
+        cls._export_finalize(
+            context=context,
+            state=state,
+            overrides=overrides,
+            values=substituted_values,
+            route=route,
+            key_order=key_order,
+        )
+
+    @classmethod
+    async def _export_async(
+        cls,
+        state: dict[str, Any],
+        metadata: ExportMetadata[ConfigModelT],
+    ) -> None:
+        """
+        Exports model state preserving substition directive calls in the model state.
+
+        Parameters
+        ----------
+        metadata
+        state
+        """
+        from configzen.config import CONTEXT, at, pre_serialize
+
+        overrides = {}
+
+        route = metadata["route"]
+        context = metadata["context"]
+        key_order = metadata["key_order"]
+        manager = context.manager
+
+        async with manager.processor_open_resource_async() as reader:
+            # Here we intentionally always preprocess the loaded configuration.
+            loaded = await manager.load_into_dict_async(await reader.read())
+
+            if route:
+                loaded = at(loaded, route, manager=manager)
+
+        substituted_values = loaded.copy()
+
+        missing = object()
+
+        for key, value in loaded.items():
+            counterpart_value = state.pop(key, missing)
+            if counterpart_value is missing:
+                continue
+            counterpart_value = pre_serialize(counterpart_value)
+
+            if is_dict_like(value):
+                if EXPORT in value:
+                    value.pop(CONTEXT, None)
+                    await cls.export_async(value, metadata=value.pop(EXPORT))
+                overrides_for_key = {
+                    sub_key: comp
+                    for sub_key, comp in counterpart_value.items()
+                    if (
+                        (orig := value.get(sub_key, missing)) is missing or orig != comp
+                    )
+                }
+                if overrides_for_key:
+                    export_key = manager.processor_class.extension_prefix + key
+                    overrides[export_key] = overrides_for_key
+
+            elif is_list_like(value):
+                await cls.export_async(value, metadata=None)
+
+            elif counterpart_value != value:
+                overrides[key] = counterpart_value
+                del substituted_values[key]
+
+        for value in state.values():
+            await cls.export_async(value, metadata=None)
+
+        cls._export_finalize(
+            context=context,
+            state=state,
+            overrides=overrides,
+            values=substituted_values,
+            route=route,
+            key_order=key_order,
+        )
+
+    @classmethod
+    def _export_finalize(  # noqa: PLR0913
+        cls,
+        context: BaseContext[ConfigModelT],
+        *,
+        state: dict[str, Any],
+        overrides: dict[str, Any],
+        values: dict[str, Any],
+        route: str | None,
+        key_order: list[str],
+    ) -> None:
+        # TODO: Optimize. We iterate over the same too many times.
 
         state |= overrides
         extras: dict[str, Any] = {
             key: state.pop(key) for key in set(state) if key not in key_order
         }
 
-        if substituted_values:
+        if values:
             substitution_directive = cls.directive(Directives.EXTEND)
             resource = str(context.manager.resource)
             if route:
                 resource = cls.route_separator.join((resource, route))
             # Put the substitution directive at the beginning of the state in-place.
             state |= {substitution_directive: resource} | {
                 key: state.pop(key) for key in set(state)
```

### Comparing `configzen-0.2.2/configzen/typedefs.py` & `configzen-0.2.3/configzen/typedefs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import collections.abc
 import contextlib
 import os
 import pathlib
 import sys
-from typing import TYPE_CHECKING, TextIO, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Optional, TextIO, TypeVar, Union
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 if TYPE_CHECKING:
@@ -20,7 +21,13 @@
 ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
 SupportsRoute: TypeAlias = Union[str, list[str], "Route"]
 
 ConfigIO: TypeAlias = contextlib.AbstractContextManager[TextIO]
 AsyncConfigIO: TypeAlias = "AiofilesContextManager[None, None, AsyncTextIOWrapper]"
 RawResourceT: TypeAlias = Union[ConfigIO, str, int, os.PathLike, pathlib.Path]
 NormalizedResourceT: TypeAlias = Union[ConfigIO, str, int, pathlib.Path]
+IncludeExcludeT: TypeAlias = Optional[
+    Union[
+        collections.abc.Set[Union[int, str]],
+        collections.abc.Mapping[Union[int, str], Any],
+    ]
+]
```

### Comparing `configzen-0.2.2/LICENSE` & `configzen-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.2.2/pyproject.toml` & `configzen-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.2.2"
+version = "0.2.3"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.2.2/README.md` & `configzen-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.2.2/PKG-INFO` & `configzen-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.2.2
+Version: 0.2.3
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

