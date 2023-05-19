# Comparing `tmp/configzen-0.1.16.tar.gz` & `tmp/configzen-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.16.tar", max compression
+gzip compressed data, was "configzen-0.1.17.tar", max compression
```

## Comparing `configzen-0.1.16.tar` & `configzen-0.1.17.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.16/configzen/__init__.py
--rw-r--r--   0        0        0    51639 2023-05-18 21:36:55.343016 configzen-0.1.16/configzen/config.py
--rw-r--r--   0        0        0     1288 2023-05-18 19:52:49.639880 configzen-0.1.16/configzen/errors.py
--rw-r--r--   0        0        0    19327 2023-05-18 19:53:22.621820 configzen-0.1.16/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.16/configzen/py.typed
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.16/LICENSE
--rw-r--r--   0        0        0     1216 2023-05-18 21:37:54.029301 configzen-0.1.16/pyproject.toml
--rw-r--r--   0        0        0     7152 2023-05-18 21:39:04.668338 configzen-0.1.16/README.md
--rw-r--r--   0        0        0     7843 1970-01-01 00:00:00.000000 configzen-0.1.16/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.17/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.17/configzen/__main__.py
+-rw-r--r--   0        0        0    52320 2023-05-19 16:17:32.119988 configzen-0.1.17/configzen/config.py
+-rw-r--r--   0        0        0     2220 2023-05-19 16:22:05.204560 configzen-0.1.17/configzen/errors.py
+-rw-r--r--   0        0        0    19090 2023-05-19 16:21:38.232918 configzen-0.1.17/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.17/configzen/py.typed
+-rw-r--r--   0        0        0      643 2023-05-19 16:22:05.221561 configzen-0.1.17/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.17/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-19 16:24:31.531220 configzen-0.1.17/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 16:08:27.014931 configzen-0.1.17/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.17/PKG-INFO
```

### Comparing `configzen-0.1.16/configzen/config.py` & `configzen-0.1.17/configzen/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,36 +55,54 @@
     # 5432
 """
 
 from __future__ import annotations
 
 import abc
 import collections.abc
-import contextlib
 import copy
 import dataclasses
 import functools
 import io
 import os
 import pathlib
 import urllib.parse
 import urllib.request
 from collections.abc import Callable, Generator
-from typing import (TYPE_CHECKING, Any, ClassVar, Generic, Literal, NamedTuple, TypeVar,
-                    Union, cast, no_type_check)
+from typing import (
+    Any,
+    ClassVar,
+    Generic,
+    Literal,
+    cast,
+    no_type_check
+)
 
 import anyconfig
 import pydantic
 from anyconfig.utils import filter_options, is_dict_like, is_list_like
 from pydantic.json import ENCODERS_BY_TYPE
 from pydantic.main import ModelMetaclass
 
-from configzen.errors import (ConfigItemAccessError, ProcessorLookupError,
-                              UnknownParserError)
+from configzen.errors import (
+    ConfigItemAccessError,
+    InternalConfigError,
+    ProcessorLookupError,
+    UnknownParserError,
+    format_syntax_error,
+)
 from configzen.processor import SUBST_METADATA, DirectiveContext, Processor
+from configzen.typedefs import (
+    T,
+    ConfigModelT,
+    SupportsRoute,
+    ConfigIO,
+    AsyncConfigIO,
+    RawResourceT,
+)
 
 try:
     import aiofiles
 
     AIOFILES_AVAILABLE = True
 except ImportError:
     aiofiles = None  # type: ignore[assignment]
@@ -107,23 +125,14 @@
 )
 
 _URL_SCHEMES: set[str] = set(
     urllib.parse.uses_relative + urllib.parse.uses_netloc + urllib.parse.uses_params,
 ) - {""}
 CONTEXT: str = "__configzen_context__"
 
-T = TypeVar("T")
-
-ContextT = TypeVar("ContextT", bound="AnyContext")
-ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
-SupportsRoute = Union[str, list[str], "Route"]
-
-OpenedT = contextlib.AbstractContextManager
-RawResourceT = Union[OpenedT, str, os.PathLike, pathlib.Path]
-
 
 def _get_defaults_from_model_class(
     model: type[pydantic.BaseSettings],
 ) -> dict[str, Any]:
     defaults = {}
     for field in model.__fields__.values():
         default = field.default
@@ -133,16 +142,16 @@
             defaults[field.name] = default
     return defaults
 
 
 def _vars(obj: Any) -> dict[str, Any]:
     obj_dict = obj
     if not isinstance(obj, dict):
-        obj_dict = vars(obj)
-    return obj_dict
+        obj_dict = obj.__dict__
+    return cast(dict[str, Any], obj_dict)
 
 
 def _is_namedtuple(
     obj: Any,
 ) -> bool:
     return (
         isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields")
@@ -267,16 +276,16 @@
     if cls is None:
         return functools.partial(generic_validator, func)
 
     generic_validate.register(cls, func)
     return cls
 
 
-@convert.register
-def convert_list(obj: list) -> list:
+@convert.register(list)
+def convert_list(obj: list[Any]) -> list[Any]:
     """
     Convert a list to safely-serializable form.
 
     Parameters
     ----------
     obj
         The list to convert.
@@ -284,16 +293,16 @@
     Returns
     -------
     The converted list.
     """
     return [convert(item) for item in obj]
 
 
-@convert.register
-def convert_mapping(obj: collections.abc.Mapping) -> dict[str, Any]:
+@convert.register(collections.abc.Mapping)
+def convert_mapping(obj: collections.abc.Mapping[Any, Any]) -> dict[Any, Any]:
     """
     Convert a mapping to safely-serializable form.
 
     Parameters
     ----------
     obj
         The mapping to convert.
@@ -302,15 +311,15 @@
     -------
     The converted mapping.
     """
     return {k: convert(v) for k, v in obj.items()}
 
 
 @functools.singledispatch
-def convert_namedtuple(obj: tuple) -> Any:
+def convert_namedtuple(obj: tuple[Any, ...]) -> Any:
     """
     Convert a namedtuple to safely-serializable form.
 
     Parameters
     ----------
     obj
         The namedtuple to convert.
@@ -346,15 +355,15 @@
                 )
                 raise ValueError(msg)
             target[actual_key] = value
 
     return load_options, dump_options
 
 
-class ConfigLoader:
+class ConfigLoader(Generic[ConfigModelT]):
     """
     A configuration resource loader.
 
     This class is used to represent a configuration resource, which
     can be a file, a URL, or a file-like object. It is used internally
     by `ConfigModel` and `AsyncConfigModel` to load and save
     configuration files.
@@ -391,37 +400,44 @@
         The URL schemes that are allowed to be used.
 
     Raises
     ------
     ValueError
     """
 
-    _resource: OpenedT | str | os.PathLike | pathlib.Path
-    processor_class: type[Processor]
+    _resource: ConfigIO | str | os.PathLike[str] | pathlib.Path
+    processor_class: type[Processor[ConfigModelT]]
     ac_parser: str | None
     create_if_missing: bool
     allowed_url_schemes: set[str]
     use_pydantic_json: bool = True
     load_options: dict[str, Any]
     dump_options: dict[str, Any]
 
     _DEFAULT_RESOURCE_KWARGS: ClassVar[dict[str, Any]] = {"encoding": "UTF-8"}
     _DEFAULT_ALLOWED_URL_SCHEMES: ClassVar[set[str]] = {"file", "http", "https"}
-    _OPEN_KWARGS: ClassVar[frozenset] = frozenset((
-        "mode", "buffering", "encoding", "errors", "newline"
-    ))
-    _URLOPEN_KWARGS: ClassVar[frozenset] = frozenset((
-        "data", "timeout", "cafile", "capath", "cadefault", "context",
-    ))
+    _OPEN_KWARGS: ClassVar[frozenset[str]] = frozenset(
+        ("mode", "buffering", "encoding", "errors", "newline")
+    )
+    _URLOPEN_KWARGS: ClassVar[frozenset[str]] = frozenset(
+        (
+            "data",
+            "timeout",
+            "cafile",
+            "capath",
+            "cadefault",
+            "context",
+        )
+    )
 
     def __init__(
         self,
         resource: RawResourceT,
         ac_parser: str | None = None,
-        processor_class: type[Processor] | None = None,
+        processor_class: type[Processor[ConfigModelT]] | None = None,
         *,
         create_if_missing: bool = False,
         **kwargs: Any,
     ) -> None:
         """Parameters
         ----------
         resource
@@ -437,28 +453,26 @@
             Whether to use Pydantic's JSON encoder/decoder instead of the default
             anyconfig one.
         **kwargs
             Additional keyword arguments to pass to
             `anyconfig.loads()` and `anyconfig.dumps()`.
         """
         if processor_class is None:
-            processor_class = Processor
+            processor_class = Processor[ConfigModelT]
 
         self.processor_class = processor_class
         self.ac_parser = ac_parser
         self.resource = resource
         self.create_if_missing = create_if_missing
         self.use_pydantic_json = kwargs.pop("use_pydantic_json", True)
         self.default_kwargs = kwargs.pop(
-            "default_kwargs",
-            self._DEFAULT_RESOURCE_KWARGS.copy()
+            "default_kwargs", self._DEFAULT_RESOURCE_KWARGS.copy()
         )
         self.allowed_url_schemes = kwargs.pop(
-            "allowed_url_schemes",
-            self._DEFAULT_ALLOWED_URL_SCHEMES.copy()
+            "allowed_url_schemes", self._DEFAULT_ALLOWED_URL_SCHEMES.copy()
         )
         self.load_options, self.dump_options = _split_ac_options(kwargs)
 
     @property
     def resource(self) -> RawResourceT:
         """
         The resource of the configuration.
@@ -545,28 +559,40 @@
 
         Parameters
         ----------
         blob
             The configuration to load.
         ac_parser
             The name of the anyconfig parser to use for loading the configuration.
+        preprocess
         **kwargs
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration dictionary.
         """
         if ac_parser is None:
             ac_parser = self.ac_parser
         kwargs = self.load_options | kwargs
-        loaded = anyconfig.loads(blob, ac_parser=ac_parser, **kwargs)
+        loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
+            blob,
+            ac_parser=ac_parser,
+            **kwargs
+        )
+        if not isinstance(loaded, collections.abc.Mapping):
+            msg = (
+                f"Expected a mapping as a result of loading {self.resource}, "
+                f"got {type(loaded).__name__}."
+            )
+            raise TypeError(msg)
+        loaded = dict(loaded)
         if preprocess:
             loaded = self.processor_class(self, loaded).preprocess()
-        return loaded
+        return cast(dict[str, Any], loaded)
 
     def dump_config(
         self,
         config: ConfigModelT,
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> str:
@@ -624,15 +650,15 @@
     def is_url(self) -> bool:
         """Whether the resource is a URL."""
         return (
             isinstance(self.resource, str)
             and urllib.parse.urlparse(self.resource).scheme in _URL_SCHEMES
         )
 
-    def open_resource(self, **kwds: Any) -> OpenedT:
+    def open_resource(self, **kwds: Any) -> ConfigIO:
         """
         Open the configuration file.
 
         Parameters
         ----------
         **kwds
             Keyword arguments to pass to the opening routine.
@@ -643,30 +669,32 @@
         -------
         The opened resource.
         """
         if self.resource is None:
             return io.StringIO()
         if self.is_url:
             url = urllib.parse.urlparse(cast(str, self.resource))
-
             if url.scheme not in self.allowed_url_schemes:
                 msg = (
                     f"URL scheme {url.scheme!r} is not allowed, "
                     f"must be one of {self.allowed_url_schemes!r}"
                 )
                 raise ValueError(msg)
             kwds = filter_options(self._URLOPEN_KWARGS, kwds)
             request = urllib.request.Request(url.geturl())
-            return urllib.request.urlopen(request, **kwds)  # noqa: S310
+            return cast(
+                ConfigIO,
+                urllib.request.urlopen(request, **kwds)  # noqa: S310
+            )
         if isinstance(self.resource, (str, os.PathLike, pathlib.Path)):
             kwds = filter_options(self._OPEN_KWARGS, kwds)
-            return pathlib.Path(self.resource).open(**kwds)
+            return cast(ConfigIO, pathlib.Path(self.resource).open(**kwds))
         return self.resource
 
-    def processor_open_resource(self, **kwargs: Any) -> OpenedT:
+    def processor_open_resource(self, **kwargs: Any) -> ConfigIO:
         """
         Called by the processor to open a configuration resource with reading intention.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the opening routine.
@@ -676,15 +704,15 @@
         Returns
         -------
         The opened resource.
         """
         kwargs = self._get_default_kwargs("read", kwargs)
         return self.open_resource(**kwargs)
 
-    def open_resource_async(self, **kwds: Any) -> Any:
+    def open_resource_async(self, **kwds: Any) -> AsyncConfigIO:
         """
         Open the configuration file asynchronously.
 
         Parameters
         ----------
         **kwds
             Keyword arguments to pass to the opening routine.
@@ -710,23 +738,24 @@
     def _get_default_kwargs(
         self,
         method: Literal["read", "write"],
         kwargs: dict[str, Any] | None = None,
     ) -> dict[str, Any]:
         if not kwargs:
             kwargs = self.default_kwargs
+        new_kwargs = cast(dict[str, Any], kwargs).copy()
         if not self.is_url:
             if method == "read":
-                kwargs.setdefault("mode", "r")
+                new_kwargs.setdefault("mode", "r")
             elif method == "write":
-                kwargs.setdefault("mode", "w")
+                new_kwargs.setdefault("mode", "w")
             else:
                 msg = f"invalid resource access method: {method!r}"
                 raise ValueError(msg)
-        return kwargs
+        return new_kwargs
 
     def read(
         self,
         *,
         config_class: type[ConfigModelT],
         create_kwargs: dict[str, Any] | None = None,
         **kwargs: Any,
@@ -754,17 +783,19 @@
                 blob = fp.read()
         except FileNotFoundError:
             blob = None
             if self.create_if_missing:
                 defaults = _get_defaults_from_model_class(config_class)
                 blob = self.dump_data(defaults)
                 self.write(blob, **(create_kwargs or {}))
-        return self.load_into(config_class, blob, **self.load_options)
+            else:
+                raise
+        return self.load_into(config_class, cast(str, blob), **self.load_options)
 
-    def write(self, blob: str | collections.abc.ByteString, **kwargs: Any) -> int:
+    def write(self, blob: str, **kwargs: Any) -> int:
         """
         Write the configuration file.
 
         Parameters
         ----------
         blob
             The string/bytes to write into the resource.
@@ -812,15 +843,15 @@
                 defaults = _get_defaults_from_model_class(config_class)
                 blob = self.dump_data(defaults)
                 await self.write_async(blob, **(create_kwargs or {}))
         return self.load_into(config_class, blob, **self.load_options)
 
     async def write_async(
         self,
-        blob: str | collections.abc.ByteString,
+        blob: str,
         **kwargs: Any,
     ) -> int:
         """
         Write the configuration file asynchronously.
 
         Parameters
         ----------
@@ -834,15 +865,19 @@
         The number of bytes written.
         """
         kwargs = self._get_default_kwargs("write", kwargs=kwargs)
         async with self.open_resource_async(**kwargs) as fp:
             return await fp.write(blob)
 
     @classmethod
-    def from_directive_context(cls, ctx: DirectiveContext, /) -> ConfigLoader:
+    def from_directive_context(
+        cls,
+        ctx: DirectiveContext,
+        /
+    ) -> ConfigLoader[ConfigModelT]:
         """
         Create a configuration loader from a preprocessor directive context.
 
         Parameters
         ----------
         ctx
 
@@ -868,69 +903,77 @@
 
 class Route:
     _TOK_DOT = "."
     _TOK_DOTLIST_ESCAPE_LEFT = "["
     _TOK_DOTLIST_ESCAPE_RIGHT = "]"
 
     def __init__(self, route: SupportsRoute) -> None:
-        self.list_route = self._parse(route)
+        self.list_route = self.parse(route)
 
     @classmethod
-    def _parse(cls, route: SupportsRoute) -> list[str]:
+    def parse(cls, route: SupportsRoute) -> list[str]:
         if isinstance(route, Route):
             return route.list_route
         if isinstance(route, list):
             return route
         if isinstance(route, str):
             return cls._decompose(route)
         raise TypeError(f"invalid route type {type(route)!r}")
 
     @classmethod
     def _decompose(cls, route: str) -> list[str]:
         route = route.removesuffix(cls._TOK_DOT) + cls._TOK_DOT[0]
         argument = ""
         escape_ctx = False
-        prev_ch = None
+        prev_char = None
         list_route = []
-        for ch in route:
-            if ch in cls._TOK_DOT:
+        for char_no, char in enumerate(route, start=1):
+            if char in cls._TOK_DOT:
                 if escape_ctx:
-                    argument += ch
+                    argument += char
                 else:
                     list_route.append(argument)
                     argument = ""
-            elif ch in cls._TOK_DOTLIST_ESCAPE_LEFT:
-                if prev_ch and prev_ch in cls._TOK_DOTLIST_ESCAPE_RIGHT:
-                    raise ValueError(
+            elif char in cls._TOK_DOTLIST_ESCAPE_LEFT:
+                if prev_char and prev_char in cls._TOK_DOTLIST_ESCAPE_RIGHT:
+                    raise InternalConfigError(
                         "invalid escape sequence "
-                        f"(expected {cls._TOK_DOT[0]} between escape sequences)"
+                        f"(expected {cls._TOK_DOT[0]} between escape sequences)",
+                        extra=char_no,
                     )
                 if escape_ctx:
-                    raise ValueError("invalid escape sequence")
+                    msg = "invalid escape sequence"
+                    raise InternalConfigError(msg, extra=char_no)
                 escape_ctx = True
-            elif ch in cls._TOK_DOTLIST_ESCAPE_RIGHT:
+            elif char in cls._TOK_DOTLIST_ESCAPE_RIGHT:
                 if not escape_ctx:
-                    raise ValueError("invalid escape sequence")
+                    msg = "invalid escape sequence"
+                    raise InternalConfigError(msg, extra=char_no)
                 escape_ctx = False
                 list_route.append(argument)
                 argument = ""
             else:
-                argument += ch
-            prev_ch = ch
+                argument += char
+            prev_char = char
         return list_route
 
+    @classmethod
+    def decompose(cls, route: str) -> list[str]:
+        with format_syntax_error(route):
+            return cls._decompose(route)
+
     def __iter__(self) -> Generator[str, None, None]:
         yield from self.list_route
 
 
 def select_scope(
-    mapping: dict[str, Any],
+    mapping: Any,
     route: SupportsRoute,
     scope_converter: Callable[[Any], dict[str, Any]] = _vars,
-    loader: ConfigLoader | None = None,
+    loader: ConfigLoader[ConfigModelT] | None = None,
 ) -> Any:
     """
     Get an item at a route.
 
     Parameters
     ----------
     mapping
@@ -952,163 +995,137 @@
             route_here.append(part)
             scope = scope_converter(scope)[part]
     except KeyError:
         raise ProcessorLookupError(loader, route_here) from None
     return scope
 
 
-if TYPE_CHECKING:
+@dataclasses.dataclass(frozen=True)
+class ConfigAt(Generic[ConfigModelT]):
+    """
+    A configuration item at a specific location.
 
-    class ConfigAt(NamedTuple, Generic[ConfigModelT]):
-        owner: ConfigModelT
-        mapping: dict[str, Any] | None
-        route: SupportsRoute
+    Attributes
+    ----------
+    owner
+        The configuration model instance.
+    mapping
+        The mapping to use.
+    route
+        The route to the item.
+    """
 
-        def get(self) -> Any:
-            ...
+    owner: ConfigModelT
+    mapping: dict[str, Any] | None
+    route: SupportsRoute
 
-        def update(self, _value: Any) -> dict[str, Any]:
-            ...
+    def get(self) -> Any:
+        """
+        Get the value of the item.
 
-        async def save_async(self) -> int:
-            ...
+        Returns
+        -------
+        The value of the item.
+        """
+        try:
+            scope = select_scope(self.mapping or self.owner, self.route)
+        except KeyError as err:
+            route_here = err.args[1]
+            raise ConfigItemAccessError(self.owner, route_here) from None
+        return scope
 
-        def save(self) -> int:
-            ...
+    def update(self, value: Any) -> Any:
+        """
+        Update the value of the item with regard to this item mapping.
 
-        async def reload_async(self) -> Any:
-            ...
+        Parameters
+        ----------
+        value
+            The new value.
 
-        def reload(self) -> Any:
-            ...
+        Returns
+        -------
+        The updated mapping.
+        """
+        route = list(Route(self.route))
+        mapping = self.mapping or self.owner
+        key = route.pop()
+        submapping = _vars(mapping)
+        route_here = []
+        try:
+            for part in route:
+                route_here.append(part)
+                submapping = _vars(submapping[part])
+            submapping[key] = value
+        except KeyError:
+            raise ConfigItemAccessError(self.owner, route_here) from None
+        return mapping
+
+    async def save_async(self, **kwargs: Any) -> int:
+        """
+        Save the configuration asynchronously.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the saving function.
 
-else:
+        Returns
+        -------
+        The number of bytes written.
+        """
+        return await save_async(self, **kwargs)
 
-    class ConfigAt(NamedTuple):
+    def save(self, **kwargs: Any) -> int:
         """
-        A configuration item at a specific location.
+        Save the configuration.
 
-        Attributes
+        Parameters
         ----------
-        owner
-            The configuration model instance.
-        mapping
-            The mapping to use.
-        route
-            The route to the item.
+        **kwargs
+            Keyword arguments to pass to the saving function.
+
+        Returns
+        -------
+        The number of bytes written.
         """
+        return save(self, **kwargs)
 
-        owner: ConfigModelT
-        mapping: dict[str, Any] | None
-        route: SupportsRoute
-
-        def get(self) -> Any:
-            """
-            Get the value of the item.
-
-            Returns
-            -------
-            The value of the item.
-            """
-            try:
-                scope = select_scope(self.mapping or self.owner, self.route)
-            except KeyError as err:
-                route_here = err.args[1]
-                raise ConfigItemAccessError(self.owner, route_here) from None
-            return scope
-
-        def update(self, value: Any) -> collections.abc.MutableMapping:
-            """
-            Update the value of the item with regard to this item mapping.
-
-            Parameters
-            ----------
-            value
-                The new value.
-
-            Returns
-            -------
-            The updated mapping.
-            """
-            route = list(Route(self.route))
-            mapping = self.mapping or self.owner
-            key = route.pop()
-            submapping = _vars(mapping)
-            route_here = []
-            try:
-                for part in route:
-                    route_here.append(part)
-                    submapping = _vars(submapping[part])
-                submapping[key] = value
-            except KeyError:
-                raise ConfigItemAccessError(self.owner, route_here) from None
-            return mapping
-
-        async def save_async(self, **kwargs: Any) -> int:
-            """
-            Save the configuration asynchronously.
+    async def reload_async(self, **kwargs: Any) -> Any:
+        """
+        Reload the configuration asynchronously.
 
-            Parameters
-            ----------
-            **kwargs
-                Keyword arguments to pass to the saving function.
+        Parameters
+        ----------
+        kwargs
+            Keyword arguments to pass to the reloading function.
 
-            Returns
-            -------
-            The number of bytes written.
-            """
-            return await save_async(self, **kwargs)
-
-        def save(self, **kwargs: Any) -> int:
-            """
-            Save the configuration.
+        Returns
+        -------
+        The reloaded configuration or its belonging item.
+        """
+        return await reload_async(self, **kwargs)
 
-            Parameters
-            ----------
-            **kwargs
-                Keyword arguments to pass to the saving function.
+    def reload(self, **kwargs: Any) -> Any:
+        """
+        Reload the configuration.
+
+        Parameters
+        ----------
+        kwargs
+            Keyword arguments to pass to the reloading function.
 
-            Returns
-            -------
-            The number of bytes written.
-            """
-            return save(self, **kwargs)
-
-        async def reload_async(self, **kwargs: Any) -> Any:
-            """
-            Reload the configuration asynchronously.
-
-            Parameters
-            ----------
-            kwargs
-                Keyword arguments to pass to the reloading function.
-
-            Returns
-            -------
-            The reloaded configuration or its belonging item.
-            """
-            return await reload_async(self, **kwargs)
-
-        def reload(self, **kwargs: Any) -> Any:
-            """
-            Reload the configuration.
-
-            Parameters
-            ----------
-            kwargs
-                Keyword arguments to pass to the reloading function.
-
-            Returns
-            -------
-            The reloaded configuration or its belonging item.
-            """
-            return reload(self, **kwargs)
+        Returns
+        -------
+        The reloaded configuration or its belonging item.
+        """
+        return reload(self, **kwargs)
 
 
-def save(section: ConfigModelT | ConfigAt, **kwargs: Any) -> int:
+def save(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> int:
     """
     Save the configuration.
 
     Parameters
     ----------
     section
         The configuration model instance or the configuration item.
@@ -1130,15 +1147,18 @@
     context = get_context(config)
     blob = context.loader.dump_config(config.copy(update=data))
     result = config.write(blob, **kwargs)
     context.initial_state = data
     return result
 
 
-async def save_async(section: ConfigModelT | ConfigAt, **kwargs: Any) -> int:
+async def save_async(
+    section: ConfigModelT | ConfigAt[ConfigModelT],
+    **kwargs: Any
+) -> int:
     """
     Save the configuration asynchronously.
 
     Parameters
     ----------
     section
         The configuration model instance or the configuration item.
@@ -1160,15 +1180,15 @@
     context = get_context(config)
     blob = context.loader.dump_config(config.copy(update=data))
     result = await config.write_async(blob, **kwargs)
     context.initial_state = data
     return result
 
 
-def reload(section: ConfigModelT | ConfigAt, **kwargs: Any) -> Any:
+def reload(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> Any:
     """
     Reload the configuration.
 
     Parameters
     ----------
     section
         The configuration model instance or the configuration item.
@@ -1185,19 +1205,22 @@
 
     config = section.owner
     context = get_context(config)
     data = config.__dict__
     newest = context.loader.read(config_class=type(config), **kwargs)
     section_data = ConfigAt(newest, newest.__dict__, section.route).get()
     new_mapping = ConfigAt(config, data, section.route).update(section_data)
-    config.__dict__ |= new_mapping
+    config.__dict__.update(new_mapping)
     return section_data
 
 
-async def reload_async(section: ConfigModelT | ConfigAt, **kwargs: Any) -> Any:
+async def reload_async(
+    section: ConfigModelT | ConfigAt[ConfigModelT],
+    **kwargs: Any
+) -> Any:
     """
     Reload the configuration asynchronously.
 
     Parameters
     ----------
     section
         The configuration model instance or the configuration item.
@@ -1214,15 +1237,15 @@
 
     config = section.owner
     context = get_context(config)
     data = config.__dict__
     newest = await context.loader.read_async(config_class=type(config), **kwargs)
     section_data = ConfigAt(newest, newest.__dict__, section.route).get()
     new_mapping = ConfigAt(config, data, section.route).update(section_data)
-    config.__dict__ |= new_mapping
+    config.__dict__.update(new_mapping)
     return new_mapping
 
 
 class AnyContext(abc.ABC, Generic[ConfigModelT]):
     """
     The base class for configuration context.
     Contexts are used to
@@ -1235,15 +1258,14 @@
     ----------
     initial_state
         The initial configuration state.
 
     """
 
     initial_state: dict[str, Any]
-    _initial_state: dict[str, Any]
 
     @abc.abstractmethod
     def trace_route(self) -> collections.abc.Generator[str, None, None]:
         """Trace the route to where the configuration subcontext points to."""
 
     @staticmethod
     def get(config: ConfigModelT) -> AnyContext[ConfigModelT]:
@@ -1255,15 +1277,15 @@
         config
             The configuration model instance.
 
         Returns
         -------
         The context of the configuration model.
         """
-        return object.__getattribute__(config, CONTEXT)
+        return cast(AnyContext[ConfigModelT], object.__getattribute__(config, CONTEXT))
 
     def bind_to(self, config: ConfigModelT) -> None:
         """
         Bind the context to the configuration model.
 
         Parameters
         ----------
@@ -1291,67 +1313,68 @@
         -------
         The new subcontext.
         """
         return Subcontext(self, part)
 
     @property
     @abc.abstractmethod
-    def loader(self) -> ConfigLoader:
+    def loader(self) -> ConfigLoader[ConfigModelT]:
         """The configuration resource loader."""
 
     @property
     @abc.abstractmethod
     def owner(self) -> ConfigModelT | None:
         """
         The top-level configuration model instance,
         holding all adjacent contexts.
         """
 
     @property
     @abc.abstractmethod
-    def section(self) -> ConfigModelT | ConfigAt[ConfigModelT]:
+    def at(self) -> ConfigModelT | ConfigAt[ConfigModelT] | None:
         """
         The configuration model instance or the configuration item
         this context points to.
         """
 
 
-class Context(AnyContext, Generic[ConfigModelT]):
+class Context(AnyContext[ConfigModelT], Generic[ConfigModelT]):
     """
     The context of a configuration model.
 
     Parameters
     ----------
     loader
         The configuration resource.
     owner
         The top-level configuration model instance,
         holding all belonging subcontexts.
     """
+    _initial_state: dict[str, Any]
 
     def __init__(
         self,
-        loader: ConfigLoader,
+        loader: ConfigLoader[ConfigModelT],
         owner: ConfigModelT | None = None,
     ) -> None:
         self._loader = loader
         self._owner = None
         self._initial_state = {}
 
         self.owner = owner
 
     def trace_route(self) -> collections.abc.Generator[str, None, None]:
         yield from ()
 
     @property
-    def loader(self) -> ConfigLoader:
+    def loader(self) -> ConfigLoader[ConfigModelT]:
         return self._loader
 
     @property
-    def section(self) -> ConfigModelT | None:
+    def at(self) -> ConfigModelT | None:
         return self.owner
 
     @property
     def owner(self) -> ConfigModelT | None:
         return self._owner
 
     @owner.setter
@@ -1366,15 +1389,15 @@
         return copy.deepcopy(self._initial_state)
 
     @initial_state.setter
     def initial_state(self, initial_state: dict[str, Any]) -> None:
         self._initial_state = copy.deepcopy(initial_state)
 
 
-class Subcontext(AnyContext, Generic[ConfigModelT]):
+class Subcontext(AnyContext[ConfigModelT], Generic[ConfigModelT]):
     """
     The subcontext of a configuration model.
 
     Parameters
     ----------
     parent
         The parent context.
@@ -1383,25 +1406,25 @@
     """
 
     def __init__(self, parent: AnyContext[ConfigModelT], part: str) -> None:
         self._parent = parent
         self._part = part
 
     @property
-    def loader(self) -> ConfigLoader:
+    def loader(self) -> ConfigLoader[ConfigModelT]:
         return self._parent.loader
 
     def trace_route(self) -> collections.abc.Generator[str, None, None]:
         yield from self._parent.trace_route()
         yield self._part
 
     @property
-    def section(self) -> ConfigAt[ConfigModelT]:
+    def at(self) -> ConfigAt[ConfigModelT]:
         if self.owner is None:
-            msg = "Cannot get section for unbound context"
+            msg = "Cannot get section pointed to by an unbound context"
             raise ValueError(msg)
         return ConfigAt(self.owner, None, list(self.trace_route()))
 
     @property
     def owner(self) -> ConfigModelT | None:
         return self._parent.owner
 
@@ -1456,15 +1479,19 @@
     try:
         context = get_context(config)
     except RuntimeError:
         context = None
     return context
 
 
-def _json_encoder(model_encoder: Callable, value: Any, **kwargs: Any) -> Any:
+def _json_encoder(
+    model_encoder: Callable[..., Any],
+    value: Any,
+    **kwargs: Any
+) -> Any:
     initial_state_type = type(value)
     converted_value = convert(value)
     if isinstance(converted_value, initial_state_type):
         return model_encoder(value, **kwargs)
     return converted_value
 
 
@@ -1481,15 +1508,15 @@
         if kwargs.pop("root", None):
             return type.__new__(cls, name, bases, namespace, **kwargs)
         new_class = super().__new__(cls, name, bases, namespace, **kwargs)
         new_class.__json_encoder__ = functools.partial(
             _json_encoder,
             new_class.__json_encoder__,
         )
-        return new_class
+        return cast(type, new_class)
 
 
 class ConfigModel(
     pydantic.BaseSettings,
     metaclass=CMBMetaclass,
     root=True,
 ):
@@ -1524,22 +1551,23 @@
             yield from state.items()
         else:
             yield from super()._iter(**kwargs)
 
     @classmethod
     def _resolve_loader(
         cls,
-        resource: ConfigLoader | RawResourceT | None = None,
+        resource: ConfigLoader[ConfigModelT] | RawResourceT | None = None,
         *,
         create_if_missing: bool | None = None,
-    ) -> ConfigLoader:
+    ) -> ConfigLoader[ConfigModelT]:
         if resource is None:
             resource = getattr(cls.__config__, "resource", None)
         if resource is None:
             raise ValueError("No resource specified")
+        loader: ConfigLoader[ConfigModelT]
         if isinstance(resource, (str, bytes)):
             loader = ConfigLoader(resource)
         elif isinstance(resource, ConfigLoader):
             loader = resource
         else:
             raise TypeError(f"Invalid resource type: {type(resource).__name__}")
         if create_if_missing is not None:
@@ -1579,15 +1607,15 @@
         Rollback the configuration to its initial state.
 
         Returns
         -------
         None
         """
         context = get_context(self)
-        self.__dict__ |= context.initial_state
+        self.__dict__.update(context.initial_state)
 
     def _ensure_settings_with_context(
         self, name: str, value: ConfigModelT
     ) -> ConfigModelT:
         context = get_context_or_none(self)
         if (
             context
@@ -1603,15 +1631,15 @@
         if isinstance(value, ConfigModel):
             return self._ensure_settings_with_context(attr, value)
         return value
 
     @classmethod
     def load(
         cls: type[ConfigModelT],
-        resource: ConfigLoader | RawResourceT | None = None,
+        resource: ConfigLoader[ConfigModelT] | RawResourceT | None = None,
         create_if_missing: bool | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration file.
         To reload the configuration, use the `reload()` method.
 
@@ -1652,17 +1680,17 @@
         context = get_context(self)
         if context.owner is self:
             new_config = context.loader.read(config_class=type(self), **kwargs)
             context.bind_to(new_config)
             context.initial_state = new_config.__dict__
             new_config.rollback()
             return new_config
-        return reload(context.section)
+        return cast(ConfigModelT, reload(cast(ConfigAt[ConfigModelT], context.at)))
 
-    def save(self, **kwargs: Any) -> int:
+    def save(self: ConfigModelT, **kwargs: Any) -> int:
         """
         Save the configuration to the configuration file.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the write method.
@@ -1673,17 +1701,17 @@
         """
         context = get_context(self)
         if context.owner is self:
             blob = context.loader.dump_config(self)
             result = self.write(blob, **kwargs)
             context.initial_state = self.__dict__
             return result
-        return save(context.section)
+        return save(cast(ConfigAt[ConfigModelT], context.at))
 
-    def write(self, blob: str | collections.abc.ByteString, **kwargs: Any) -> int:
+    def write(self, blob: str, **kwargs: Any) -> int:
         """
         Overwrite the configuration file with the given string or bytes.
 
         Parameters
         ----------
         blob
             The blob to write to the configuration file.
@@ -1692,33 +1720,33 @@
 
         Returns
         -------
         The number of bytes written.
         """
         context = get_context(self)
         if context.loader.is_url:
-            msg = "Saving to URLs is not yet supported"
+            msg = "Writing to URLs is not yet supported"
             raise NotImplementedError(msg)
         return context.loader.write(blob, **kwargs)
 
     @classmethod
     async def load_async(
         cls: type[ConfigModelT],
-        resource: ConfigLoader | RawResourceT | None,
+        resource: ConfigLoader[ConfigModelT] | RawResourceT | None,
         *,
         create_if_missing: bool = False,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration file asynchronously.
         To reload the configuration, use the `reload()` method.
 
         Parameters
         ----------
-        loader
+        resource
             The configuration resource.
         create_if_missing
             Whether to create the configuration file if it does not exist.
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
@@ -1747,17 +1775,20 @@
         context = get_context(self)
         if context.owner is self:
             new_async_config = await context.loader.read_async(**kwargs)
             context.bind_to(new_async_config)
             context.initial_state = new_async_config.__dict__
             self.rollback()
             return new_async_config
-        return await reload_async(context.section)
+        return cast(
+            ConfigModelT,
+            await reload_async(cast(ConfigAt[ConfigModelT], context.at))
+        )
 
-    async def save_async(self, **kwargs: Any) -> int:
+    async def save_async(self: ConfigModelT, **kwargs: Any) -> int:
         """
         Save the configuration to the configuration file asynchronously.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the write method.
@@ -1768,18 +1799,18 @@
         """
         context = get_context(self)
         if context.owner is self:
             blob = context.loader.dump_config(self)
             result = await self.write_async(blob, **kwargs)
             context.initial_state = self.__dict__
             return result
-        return await save_async(context.section)
+        return await save_async(cast(ConfigAt[ConfigModelT], context.at))
 
     async def write_async(
-        self, blob: str | collections.abc.ByteString, **kwargs: Any
+        self, blob: str, **kwargs: Any
     ) -> int:
         """
         Overwrite the configuration file asynchronously with the given string or bytes.
 
         Parameters
         ----------
         blob
@@ -1808,8 +1839,11 @@
         The configuration resource to read from/write to.
 
         If a string, it will be interpreted as a path to a file.
 
     And all other attributes from `pydantic.BaseSettings.Config`.
     """
 
-    resource: ConfigLoader | RawResourceT | None = None
+    resource: ConfigLoader[ConfigModel] | RawResourceT | None = None
+    validate_assignment: bool = True
+
+    Extra = pydantic.Extra
```

### Comparing `configzen-0.1.16/configzen/errors.py` & `configzen-0.1.17/configzen/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,56 @@
 """This module contains all the custom errors raised by _configzen_."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+import contextlib
+from collections.abc import Generator
+from typing import TYPE_CHECKING, Any
 
 import anyconfig
 
 if TYPE_CHECKING:
-    from configzen.config import ConfigLoader, ConfigModelT
+    from configzen.config import ConfigLoader
+    from configzen.typedefs import ConfigModelT
 
 
 class ConfigError(Exception):
     """An error occurred while loading a configuration."""
 
 
 class IncorrectConfigError(ConfigError):
     """An error occurred while loading a configuration."""
 
 
+class InternalConfigError(ConfigError):
+    """Error to raise before reraising as an underlying error."""
+
+    def __init__(self, msg: str, extra: Any = None) -> None:
+        super().__init__(msg)
+        self.extra = extra
+
+
+class ArgumentSyntaxError(ConfigError):
+    """An error occurred while parsing arguments."""
+
+
+@contextlib.contextmanager
+def format_syntax_error(source: str) -> Generator[None, None, None]:
+    """Raise a SyntaxError with a message and a source."""
+    try:
+        yield
+    except InternalConfigError as exc:
+        char_no = exc.extra
+        charlist = ["~"] * len(source)
+        charlist[char_no] = "^"
+        indicator = "".join(charlist)
+        msg = "\n".join(map(str, (exc, repr(source), indicator)))
+        raise ArgumentSyntaxError(msg) from None
+
+
 class UnknownParserError(ConfigError, anyconfig.UnknownFileTypeError):
     """Engine was attempted to be used but is not registered."""
 
 
 class ConfigItemAccessError(ConfigError, LookupError):
     """An error occurred while accessing configuration part."""
 
@@ -32,10 +61,14 @@
             f"could not get {type(config).__name__}.{route}",
         )
 
 
 class ProcessorLookupError(ConfigError, LookupError):
     """An error occurred while looking up a processor."""
 
-    def __init__(self, resource: ConfigLoader | None, route: list[str]) -> None:
+    def __init__(
+        self,
+        resource: ConfigLoader[ConfigModelT] | None,
+        route: list[str]
+    ) -> None:
         resource_name = resource.resource if resource else "the provided resource"
         super().__init__(f"{route} not found in {resource_name}")
```

### Comparing `configzen-0.1.16/configzen/processor.py` & `configzen-0.1.17/configzen/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from __future__ import annotations
 
 import dataclasses
 import enum
 from collections.abc import Callable
-from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar
+from typing import TYPE_CHECKING, Any, ClassVar, TypedDict, TypeVar, Generic
 
 from anyconfig.utils import is_dict_like, is_list_like
 
+from configzen.errors import InternalConfigError, format_syntax_error
+from configzen.typedefs import ConfigModelT
+
 if TYPE_CHECKING:
     from configzen.config import AnyContext, ConfigLoader
 
-
 __all__ = (
     "DirectiveContext",
     "directive",
     "Processor",
 )
 
 
 DirectiveT = TypeVar("DirectiveT")
-ProcessorT = TypeVar("ProcessorT", bound="Processor")
 
 SUBST_METADATA: str = "__configzen_substitute__"
 EXECUTES_DIRECTIVES: str = "__configzen_executes_directives__"
 
 
-DirectiveHandlerT = Callable[[ProcessorT, "DirectiveContext"], None]
-
-
 def directive(
     name: str | enum.Enum,
-) -> Callable[[DirectiveHandlerT], DirectiveHandlerT]:
+) -> Callable[..., Any]:
     """
     Decorator for creating processor directives.
 
     Parameters
     ----------
     name
         The name of the directive.
@@ -42,25 +40,25 @@
     Returns
     -------
     The decorated function.
     """
     if isinstance(name, enum.Enum):
         name = name.value.casefold()
 
-    def decorator(func: DirectiveHandlerT) -> DirectiveHandlerT:
+    def decorator(func: Any) -> Any:
         if not hasattr(func, EXECUTES_DIRECTIVES):
             setattr(func, EXECUTES_DIRECTIVES, set())
         getattr(func, EXECUTES_DIRECTIVES).add(name)
         return func
 
     return decorator
 
 
 @dataclasses.dataclass
-class DirectiveContext(Generic[DirectiveT]):
+class DirectiveContext:
     """
     Context for processor directives.
 
     Attributes
     ----------
     directive
         The directive.
@@ -73,15 +71,15 @@
     snippet
         The config snippet where this directive was invoked.
     container
         The dictionary that contains the :attr:`dict`.
 
     """
 
-    directive: DirectiveT
+    directive: str
     key: str
     prefix: str
     arguments: list[str]
     snippet: dict[str, Any]
     container: dict[str, Any]
 
     def has_duplicates(self, *, require_same_arguments: bool = True) -> bool:
@@ -98,199 +96,186 @@
                 if require_same_arguments and arguments != self.arguments:
                     continue
                 return True
         return False
 
 
 class Tokens(str, enum.Enum):
-    LPAREN = "("
-    RPAREN = ")"
-    COMMA = ",;"
-    STRING = "\"'"
-    ESCAPE = "\\"
+    LPAREN: str = "("
+    RPAREN: str = ")"
+    COMMA: str = ",;"
+    STRING: str = "\"'"
+    ESCAPE: str = "\\"
 
 
 class ArgumentSyntaxError(ValueError):
     """
     Raised when there is a syntax error in an argument.
     """
 
 
 def _parse_argument_string_impl(
     raw_argument_string: str,
     tokens: type[Tokens] = Tokens,
 ) -> list[str]:
-    prev_ch = None
-
+    prev_char = None
     string_ctx = None
     escape_ctx = False
     arguments: list[str] = []
     argument = ""
     emit = arguments.append
     explicit_strings_ctx = True
 
     tok_escape = tokens.ESCAPE
     tok_string = tokens.STRING
     tok_comma = tokens.COMMA
 
-    for no, ch in enumerate(raw_argument_string, start=1):
+    for char_no, char in enumerate(raw_argument_string, start=1):
         if escape_ctx:
             escape_ctx = False
-            argument += ch
-        elif ch in tok_escape:
+            argument += char
+        elif char in tok_escape:
             escape_ctx = True
-        elif ch in tok_string:
+        elif char in tok_string:
             if string_ctx and not explicit_strings_ctx:
-                raise ArgumentSyntaxError(
-                    f"Implicit string closed with explicit string character {ch}",
-                    (no, ch),
-                )
+                msg = f"Implicit string closed with explicit string character {char}"
+                raise InternalConfigError(msg, extra=char_no)
             explicit_strings_ctx = True
             if string_ctx is None:
                 # we enter a string
-                string_ctx = ch
-            elif string_ctx == ch:
+                string_ctx = char
+            elif string_ctx == char:
                 # we exit a string
                 string_ctx = None
             else:
                 # we are in a string
-                argument += ch
-        elif ch in tok_comma:
+                argument += char
+        elif char in tok_comma:
             if string_ctx:
                 if not explicit_strings_ctx:
                     string_ctx = None
                     explicit_strings_ctx = True
                     emit(argument)
                     argument = ""
             else:
-                if prev_ch in {*tok_comma, None}:
-                    raise ArgumentSyntaxError("Empty argument", (no, ch))
+                if prev_char in {*tok_comma, None}:
+                    msg = "Empty argument"
+                    raise InternalConfigError(msg, extra=char_no)
                 emit(argument)
                 argument = ""
                 explicit_strings_ctx = False
-        elif not string_ctx and not ch.isspace():
-            if prev_ch in {*tok_comma, None}:
-                string_ctx = ch
-                argument += ch
+        elif not string_ctx and not char.isspace():
+            if prev_char in {*tok_comma, None}:
+                string_ctx = char
+                argument += char
                 explicit_strings_ctx = False
             if explicit_strings_ctx:
-                raise ArgumentSyntaxError(
-                    "Unexpected character after explicit string", (no, ch)
-                )
+                msg = "Unexpected character after explicit string"
+                raise InternalConfigError(msg, extra=char_no)
         else:
-            argument += ch
-        prev_ch = ch
+            argument += char
+        prev_char = char
     return arguments
 
 
 def _parse_argument_string(
     raw_argument_string: str,
     tokens: type[Tokens] = Tokens,
 ) -> list[str]:
     """Half for jokes, half for serious use"""
 
-    no = 0
     tok_comma = tokens.COMMA
 
     if any(raw_argument_string.endswith(tok) for tok in tok_comma):
         raw_argument_string = raw_argument_string[:-1]
     raw_argument_string += tok_comma[0]
 
-    # Parse arguments with respect to strings
-    try:
-        arguments = _parse_argument_string_impl(raw_argument_string, tokens)
-    except ArgumentSyntaxError as e:
-        msg, (no, ch) = e.args
-        charlist = ["~"] * (len(raw_argument_string) + 1)
-        displayed_argument_string = (
-            raw_argument_string[:-1]
-            if no == len(raw_argument_string) + 1
-            else raw_argument_string
-        ).join((tokens.LPAREN[0], tokens.RPAREN[0]))
-        charlist[no] = "^"
-        indicator = "".join(charlist)
-        raise ArgumentSyntaxError(
-            "\n" + displayed_argument_string + "\n" + indicator + "\n" + msg
-        ) from None
-
-    return arguments
+    with format_syntax_error(raw_argument_string):
+        return _parse_argument_string_impl(raw_argument_string, tokens)
 
 
 def parse_directive_call(
     prefix: str,
     directive_name: str,
     tokens: type[Tokens] = Tokens,
 ) -> tuple[str, list[str]]:
     arguments = []
     if directive_name.startswith(prefix):
-        directive_name = directive_name[len(prefix):].casefold()
+        directive_name = directive_name[len(prefix) :].casefold()
 
         if directive_name.endswith(tokens.RPAREN):
             try:
                 lpar = directive_name.index(tokens.LPAREN)
             except ValueError:
                 raise ValueError(f"invalid directive call: {directive_name}") from None
             (directive_name, raw_argument_string) = (
                 directive_name[:lpar],
-                directive_name[lpar + 1: -1],
+                directive_name[lpar + 1 : -1],
             )
             arguments = _parse_argument_string(raw_argument_string, tokens)
 
         if not directive_name.isidentifier():
             raise ValueError(f"Invalid directive name: {directive_name}")
 
     return directive_name, arguments
 
 
-class SubstitutionMetadata(TypedDict):
-    """
-    Metadata for a substitution directive: either EXPAND or EXTEND call.
+if TYPE_CHECKING:
+    class SubstitutionMetadata(TypedDict, Generic[ConfigModelT]):
+        route: str | None
+        context: AnyContext[ConfigModelT]
+        preprocess: bool
 
-    Attributes
-    ----------
-    route
-        The route to import from.
-    context
-        The context attached to the import.
-    """
+else:
+    class SubstitutionMetadata(TypedDict):
+        """
+        Metadata for a substitution directive: either EXPAND or EXTEND call.
+
+        Attributes
+        ----------
+        route
+            The route to import from.
+        context
+            The context attached to the import.
+        """
 
-    route: str | None
-    context: AnyContext
-    preprocess: bool
+        route: str | None
+        context: AnyContext[ConfigModelT]
+        preprocess: bool
 
 
-class BaseProcessor:
+class BaseProcessor(Generic[ConfigModelT]):
     """
     Processor that executes directives.
 
     Attributes
     ----------
     dict_config
         The dictionary config to parse and update.
     directive_prefix
         The prefix for directives.
     """
 
-    _directive_handlers: dict[str, DirectiveHandlerT] = None  # type: ignore[assignment]
+    _directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
     directive_prefix: ClassVar[str]
     extension_prefix: ClassVar[str]
 
     def __init__(
         self,
-        resource: ConfigLoader,
+        resource: ConfigLoader[ConfigModelT],
         dict_config: dict[str, Any],
     ) -> None:
         self.loader = resource
         self.dict_config = dict_config
 
     @classmethod
     def export(
         cls,
         state: dict[str, Any],
-        metadata: SubstitutionMetadata,
+        metadata: SubstitutionMetadata[ConfigModelT],
     ) -> None:
         pass
 
     def preprocess(self) -> dict[str, Any]:
         """
         Parse the dictionary config and return the parsed config,
         ready for instantiating the model.
@@ -359,21 +344,25 @@
             cls._directive_handlers = cls._directive_handlers.copy()
         for _name, func in cls.__dict__.items():
             if hasattr(func, EXECUTES_DIRECTIVES):
                 for directive_name in getattr(func, EXECUTES_DIRECTIVES):
                     cls._directive_handlers[directive_name] = func
 
     @classmethod
-    def register_directive(cls, name: str, func: DirectiveHandlerT) -> None:
+    def register_directive(cls, name: str, func: Any) -> None:
         if cls._directive_handlers is None:
             cls._directive_handlers = {}
         cls._directive_handlers[name] = func
 
     @classmethod
-    def directive(cls, directive_name: str, arguments: list[str] | None = None) -> str:
+    def directive(
+        cls,
+        directive_name: str,
+        arguments: list[str] | None = None
+    ) -> str:
         """
         Create a directive call.
 
         Parameters
         ----------
         directive_name
             The name of the directive.
@@ -392,31 +381,31 @@
                 argument = argument.replace("\\", "\\\\")
                 return f'"{argument}"'
             return argument
 
         if isinstance(directive_name, enum.Enum):
             directive_name = directive_name.value
 
-        return (
-            cls.directive_prefix
-            + directive_name
-            + (",".join(map(_fmt_argument, arguments)).join("()") if arguments else "")
+        fmt_arguments = (
+            ",".join(map(_fmt_argument, arguments)).join("()")
+            if arguments else ""
         )
+        return cls.directive_prefix + directive_name + fmt_arguments
 
 
 class Directives(str, enum.Enum):
     EXPAND = "expand"
     EXTEND = "extend"
     INCLUDE = "include"
     COPY = "copy"
     PROCESSOR = "processor"
     DEFINE = "define"
 
 
-class Processor(BaseProcessor):
+class Processor(BaseProcessor[ConfigModelT]):
     directive_prefix = "^"
     extension_prefix = "+"
 
     @directive(Directives.EXPAND)
     def expand(self, ctx: DirectiveContext) -> None:
         """
         Expand a configuration with another configuration.
@@ -541,19 +530,15 @@
           foo: 3
           bar: 2
         ```
         """
         return self._substitute(ctx, preprocess=False, preserve=False)
 
     def _substitute(
-        self,
-        ctx: DirectiveContext,
-        *,
-        preprocess: bool,
-        preserve: bool
+        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
     ) -> None:
         from configzen.config import CONTEXT, Context, select_scope
 
         loader_class = type(self.loader)
         if len(ctx.arguments) > 1:
             msg = f"{ctx.directive!r} directive can select only one section"
             raise ValueError(msg)
@@ -579,32 +564,30 @@
                     f"from {loader.resource} that does not exist"
                 ) from None
             if not is_dict_like(substituted):
                 raise ValueError(
                     f"imported item {substitution_route!r} "
                     f"from {loader.resource} is not a dictionary"
                 )
-        context: Context = Context(loader)
+        context: Context[ConfigModelT] = Context(loader)
         ctx.container = substituted | ctx.container
 
         if preserve:
             ctx.container |= {
                 CONTEXT: context,
                 SUBST_METADATA: SubstitutionMetadata(
-                    route=substitution_route,
-                    context=context,
-                    preprocess=preprocess
+                    route=substitution_route, context=context, preprocess=preprocess
                 ),
             }
 
     @classmethod
     def export(
         cls,
         state: dict[str, Any],
-        metadata: SubstitutionMetadata,
+        metadata: SubstitutionMetadata[ConfigModelT],
     ) -> None:
         """
         Exports model state preserving substition directive calls in the model state.
 
         Parameters
         ----------
         metadata
@@ -612,19 +595,21 @@
         """
         from configzen.config import convert, select_scope
 
         overrides = {}
 
         context = metadata["context"]
         route = metadata["route"]
-        preprocess = metadata["preprocess"]
         loader = context.loader
+        preprocess = metadata["preprocess"]
 
         with loader.processor_open_resource() as reader:
-            loaded = loader.load_into_dict(reader.read(), preprocess=preprocess)
+            # Here, we intentionally always preprocess the loaded configuration.
+            loaded = loader.load_into_dict(reader.read(), preprocess=True)
+
             if route:
                 loaded = select_scope(loaded, route, loader=loader)
 
         substituted_values = loaded.copy()
 
         missing = object()
```

### Comparing `configzen-0.1.16/LICENSE` & `configzen-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.16/README.md` & `configzen-0.1.17/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 overriding desired sections as needed:
 
 ```yaml
 # production.yaml
 ^extend: base.json
 
 +app:
-    debug: false
+  debug: false
 ```
 
 Using `+` in front of a key will update the section already defined at that key,
 instead of replacing it.
 
 Notice how configuration file formats don't matter in _configzen_: you can 
 extend JSON configurations in YAML, but that might be as well any other format
```

### Comparing `configzen-0.1.16/PKG-INFO` & `configzen-0.1.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.16
+Version: 0.1.17
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -166,15 +166,15 @@
 overriding desired sections as needed:
 
 ```yaml
 # production.yaml
 ^extend: base.json
 
 +app:
-    debug: false
+  debug: false
 ```
 
 Using `+` in front of a key will update the section already defined at that key,
 instead of replacing it.
 
 Notice how configuration file formats don't matter in _configzen_: you can 
 extend JSON configurations in YAML, but that might be as well any other format
```

