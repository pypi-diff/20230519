# Comparing `tmp/py_datastruct-0.3.0.tar.gz` & `tmp/py_datastruct-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_datastruct-0.3.0.tar", max compression
+gzip compressed data, was "py_datastruct-0.4.0.tar", max compression
```

## Comparing `py_datastruct-0.3.0.tar` & `py_datastruct-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1076 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/LICENSE
--rw-r--r--   0        0        0     9323 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/README.md
--rw-r--r--   0        0        0      676 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/__init__.py
--rw-r--r--   0        0        0     3154 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/context.py
--rw-r--r--   0        0        0     1038 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/fields/__init__.py
--rw-r--r--   0        0        0     1476 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/fields/_utils.py
--rw-r--r--   0        0        0     6105 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/fields/helper.py
--rw-r--r--   0        0        0     2337 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/fields/special.py
--rw-r--r--   0        0        0      894 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/fields/standard.py
--rw-r--r--   0        0        0     1900 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/fields/wrapper.py
--rw-r--r--   0        0        0    15547 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/main.py
--rw-r--r--   0        0        0     2400 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/types.py
--rw-r--r--   0        0        0      141 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/utils/__init__.py
--rw-r--r--   0        0        0      517 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/utils/config.py
--rw-r--r--   0        0        0      233 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/utils/const.py
--rw-r--r--   0        0        0     2793 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/utils/context.py
--rw-r--r--   0        0        0     8251 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/utils/fields.py
--rw-r--r--   0        0        0     1466 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/utils/fmt.py
--rw-r--r--   0        0        0     1307 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/utils/misc.py
--rw-r--r--   0        0        0      839 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/datastruct/utils/public.py
--rw-r--r--   0        0        0      490 2023-03-25 21:54:02.917952 py_datastruct-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9960 1970-01-01 00:00:00.000000 py_datastruct-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/LICENSE
+-rw-r--r--   0        0        0     9323 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/README.md
+-rw-r--r--   0        0        0      676 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/datastruct/__init__.py
+-rw-r--r--   0        0        0     3154 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/datastruct/context.py
+-rw-r--r--   0        0        0     1090 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/datastruct/fields/__init__.py
+-rw-r--r--   0        0        0     1476 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/datastruct/fields/_utils.py
+-rw-r--r--   0        0        0     7455 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/datastruct/fields/helper.py
+-rw-r--r--   0        0        0     2337 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/datastruct/fields/special.py
+-rw-r--r--   0        0        0      894 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/datastruct/fields/standard.py
+-rw-r--r--   0        0        0     1900 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/datastruct/fields/wrapper.py
+-rw-r--r--   0        0        0    17567 2023-05-19 09:09:06.167323 py_datastruct-0.4.0/datastruct/main.py
+-rw-r--r--   0        0        0     2400 2023-05-19 09:09:06.171323 py_datastruct-0.4.0/datastruct/types.py
+-rw-r--r--   0        0        0      141 2023-05-19 09:09:06.171323 py_datastruct-0.4.0/datastruct/utils/__init__.py
+-rw-r--r--   0        0        0      517 2023-05-19 09:09:06.171323 py_datastruct-0.4.0/datastruct/utils/config.py
+-rw-r--r--   0        0        0      233 2023-05-19 09:09:06.171323 py_datastruct-0.4.0/datastruct/utils/const.py
+-rw-r--r--   0        0        0     2793 2023-05-19 09:09:06.171323 py_datastruct-0.4.0/datastruct/utils/context.py
+-rw-r--r--   0        0        0     8195 2023-05-19 09:09:06.171323 py_datastruct-0.4.0/datastruct/utils/fields.py
+-rw-r--r--   0        0        0     1466 2023-05-19 09:09:06.171323 py_datastruct-0.4.0/datastruct/utils/fmt.py
+-rw-r--r--   0        0        0     1307 2023-05-19 09:09:06.171323 py_datastruct-0.4.0/datastruct/utils/misc.py
+-rw-r--r--   0        0        0      839 2023-05-19 09:09:06.171323 py_datastruct-0.4.0/datastruct/utils/public.py
+-rw-r--r--   0        0        0      490 2023-05-19 09:09:06.171323 py_datastruct-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9960 1970-01-01 00:00:00.000000 py_datastruct-0.4.0/PKG-INFO
```

### Comparing `py_datastruct-0.3.0/LICENSE` & `py_datastruct-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/README.md` & `py_datastruct-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/__init__.py` & `py_datastruct-0.4.0/datastruct/__init__.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/context.py` & `py_datastruct-0.4.0/datastruct/context.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/fields/__init__.py` & `py_datastruct-0.4.0/datastruct/fields/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 #  Copyright (c) Kuba Szczodrzyński 2023-1-7.
 
 from .helper import (
     bitfield,
     buffer_end,
     buffer_start,
+    bytestr,
     checksum_end,
     checksum_field,
     checksum_start,
     const,
     const_into,
     eval_into,
     hook_end,
     packing,
     probe,
-    string,
     tell,
     tell_into,
+    text,
     unpacking,
     validate,
     varlist,
+    vartext,
     virtual,
 )
 from .special import action, align, alignto, hook, padding, seek, skip
 from .standard import built, field, subfield
 from .wrapper import adapter, cond, repeat, switch
 
 __all__ = [
@@ -30,14 +32,15 @@
     "adapter",
     "align",
     "alignto",
     "bitfield",
     "buffer_end",
     "buffer_start",
     "built",
+    "bytestr",
     "checksum_end",
     "checksum_field",
     "checksum_start",
     "cond",
     "const",
     "const_into",
     "eval_into",
@@ -46,17 +49,18 @@
     "hook_end",
     "packing",
     "padding",
     "probe",
     "repeat",
     "seek",
     "skip",
-    "string",
     "subfield",
     "switch",
     "tell",
     "tell_into",
+    "text",
     "unpacking",
     "validate",
     "varlist",
+    "vartext",
     "virtual",
 ]
```

### Comparing `py_datastruct-0.3.0/datastruct/fields/_utils.py` & `py_datastruct-0.4.0/datastruct/fields/_utils.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/fields/helper.py` & `py_datastruct-0.4.0/datastruct/fields/helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -71,36 +71,81 @@
     def wrap(base: Field):
         base.default = const_value
         return adapter(Const())(base)
 
     return wrap
 
 
-def string(length: Value[int], *, default: str = ..., padding: bytes = None):
-    class String(Adapter):
+def bytestr(length: Value[int], *, default: bytes = ..., padding: bytes = None):
+    class ByteStr(Adapter):
         def encode(self, value: bytes, ctx: Context) -> bytes:
             return value.ljust(
                 evaluate(ctx, length), padding or ctx.P.config.padding_pattern
             )
 
         def decode(self, value: bytes, ctx: Context) -> bytes:
             return value.rstrip(padding or ctx.P.config.padding_pattern)
 
-    return adapter(String())(field(length, default=default))
+    return adapter(ByteStr())(field(length, default=default))
 
 
-def varlist(when: Eval[bool]):
-    return repeat(
-        when=lambda ctx: (
-            (ctx.G.packing and ctx.P.i < len(ctx.P.self))
-            or (ctx.G.unpacking and when(ctx))
+def text(
+    length: Value[int],
+    *,
+    default: str = ...,
+    encoding: str = "utf-8",
+    padding: bytes = None,
+    variable: bool = False,
+):
+    class Text(Adapter):
+        def encode(self, value: str, ctx: Context) -> bytes:
+            if variable:
+                return value.encode(encoding)
+            return value.encode(encoding).ljust(
+                evaluate(ctx, length),
+                padding or ctx.P.config.padding_pattern,
+            )
+
+        def decode(self, value: bytes, ctx: Context) -> str:
+            return value.rstrip(
+                padding or ctx.P.config.padding_pattern,
+            ).decode(encoding)
+
+    return adapter(Text())(
+        field(
+            lambda ctx: len(ctx.P.self)
+            if variable and ctx.G.packing
+            else evaluate(ctx, length),
+            default=default,
         )
     )
 
 
+def vartext(length: Value[int], **kwargs):
+    return text(length, variable=True, **kwargs)
+
+
+def varlist(count: Value[int] = None, *, when: Eval[bool] = None):
+    if count is not None:
+        return repeat(
+            when=lambda ctx: (
+                (ctx.G.packing and ctx.P.i < len(ctx.P.self))
+                or (ctx.G.unpacking and ctx.P.i < evaluate(ctx, count))
+            )
+        )
+    if when is not None:
+        return repeat(
+            when=lambda ctx: (
+                (ctx.G.packing and ctx.P.i < len(ctx.P.self))
+                or (ctx.G.unpacking and when(ctx))
+            )
+        )
+    raise TypeError("Either count or when has to be specified")
+
+
 def probe():
     def _probe(ctx: Context):
         print(f"Probe: {ctx}")
 
     return action(_probe)
```

### Comparing `py_datastruct-0.3.0/datastruct/fields/special.py` & `py_datastruct-0.4.0/datastruct/fields/special.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/fields/standard.py` & `py_datastruct-0.4.0/datastruct/fields/standard.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/fields/wrapper.py` & `py_datastruct-0.4.0/datastruct/fields/wrapper.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/main.py` & `py_datastruct-0.4.0/datastruct/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,27 +23,50 @@
     field_decode,
     field_do_seek,
     field_encode,
     field_get_base,
     field_get_default,
     field_get_meta,
     field_get_padding,
+    field_get_type,
     field_switch_base,
     field_validate,
 )
 from .utils.fmt import fmt_evaluate
 from .utils.misc import SizingIO
 
 
 @dataclass
 class DataStruct:
     def __post_init__(self) -> None:
         for field, meta, value in self.fields():
             field_validate(field, meta)
 
+            if value != Ellipsis:
+                # try to map simple default values
+                field_type, _ = field_get_type(field)
+                if field_type is not None:
+                    value = field_decode(value, field_type)
+                    if not isinstance(value, field_type):
+                        if meta.adapter:
+                            # try to adapt default values
+                            try:
+                                value = meta.adapter.decode(value, None)
+                            except Exception:
+                                raise ValueError(
+                                    f"Couldn't build the default value of {field.name} - the adapter "
+                                    "might be requiring the context. Pass 'default' value "
+                                    "resulting *after* applying the adapter"
+                                )
+                        else:
+                            raise TypeError(
+                                f"Wrong field type - expected {field_type}, found default {type(value)}"
+                            )
+                    self.__setattr__(field.name, value)
+
             # accept special fields and those already having a value
             if value != Ellipsis or not meta.public:
                 continue
 
             default = field_get_default(field, meta, DataStruct)
             if default is not None:
                 # print("Got default for", field.name, default)
@@ -175,15 +198,22 @@
             while count is None or i < count:
                 ctx.P.self = value
                 ctx.P.i = i
                 if evaluate(ctx, meta.when) is False:
                     break
 
                 if not base_meta.builder:
-                    item = next(items_iter)
+                    try:
+                        item = next(items_iter)
+                    except StopIteration:
+                        raise ValueError(
+                            "No more items to pack! "
+                            "Check the return value of 'when' and 'last'. "
+                            "Perhaps the list is missing the last element?"
+                        )
                 else:
                     item = Ellipsis
                 item = self._write_field(ctx, base_field, base_meta, item)
                 if isinstance(items, list):
                     # don't reassign built fields to tuples
                     # only update in lists (which will update self+ctx too)
                     if len(items) <= i:
@@ -199,14 +229,17 @@
                     break
                 i += 1
             ctx.P.pop("i", None)
             return items
 
         if meta.ftype == FieldType.COND:
             if evaluate(ctx, meta.condition) is False:
+                if meta.if_not is not Ellipsis:
+                    value = evaluate(ctx, meta.if_not)
+                    return value
                 return Ellipsis
             return self._write_field(ctx, *field_get_base(meta), value)
 
         if meta.ftype == FieldType.SWITCH:
             field = field_switch_base(self.config(), ctx, meta)
             meta = field_get_meta(field)
             if value is Ellipsis:
@@ -307,14 +340,15 @@
             meta = field_get_meta(field)
             return cls._read_field(ctx, field, meta)
 
     def pack(
         self,
         io: Optional[IO[bytes]] = None,
         parent: Union[Context, "DataStruct", None] = None,
+        fname: str = None,
         **kwargs,
     ) -> Optional[bytes]:
         sizing = isinstance(io, SizingIO)
         if isinstance(parent, Context) and not sizing:
             glob = parent.G
         else:
             if io is None:
@@ -329,19 +363,25 @@
 
         fields = self.fields()
         ctx = build_context(glob, parent, self.config(), **kwargs)
         ctx.self = self
         field_name = type(self).__name__
         try:
             for field, meta, _ in fields:
+                if fname is not None and field.name != fname:
+                    continue
+                fname = None
                 field_name = f"{type(self).__name__}.{field.name}"
                 # print(f"Packing {meta.ftype.name} '{field_name}'")
                 value = self._write_field(ctx, field, meta, ctx[field.name])
                 if value is not Ellipsis and meta.public:
                     setattr(self, field.name, value)
+            if fname is not None:
+                # after packing, the field must have been found
+                raise ValueError(f"No such field: {fname}")
         except EXCEPTIONS as e:
             if ctx.G.sizing:
                 suffix = f"; while sizing '{field_name}'"
             else:
                 suffix = f"; while packing '{field_name}'"
             e.args = (e.args[0] + suffix,)
             raise e
@@ -387,19 +427,20 @@
         except EXCEPTIONS as e:
             suffix = f"; while unpacking '{field_name}'"
             e.args = (e.args[0] + suffix,)
             raise e
 
     def sizeof(
         self,
+        fname: str = None,
         parent: Union[Context, "DataStruct", None] = None,
         **kwargs,
     ) -> int:
         io = SizingIO()
-        self.pack(io=io, parent=parent, **kwargs)
+        self.pack(io=io, parent=parent, fname=fname, **kwargs)
         return io.size
 
     def fields(self) -> List[Tuple[Field, FieldMeta, Any]]:
         return [
             (
                 field,
                 field_get_meta(field),
```

### Comparing `py_datastruct-0.3.0/datastruct/types.py` & `py_datastruct-0.4.0/datastruct/types.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/utils/config.py` & `py_datastruct-0.4.0/datastruct/utils/config.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/utils/context.py` & `py_datastruct-0.4.0/datastruct/utils/context.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/utils/fields.py` & `py_datastruct-0.4.0/datastruct/utils/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,35 +10,33 @@
 from .const import ARRAYS
 from .context import evaluate
 from .fmt import fmt_check
 from .misc import pad_up, repstr
 
 
 def field_encode(v: Any) -> Any:
-    if isinstance(v, str):
-        return v.encode()
     if isinstance(v, int):
         return v
     if isinstance(v, Enum):
         return v.value
     return v
 
 
 def field_decode(v: Any, cls: type) -> Any:
-    if issubclass(cls, str):
-        return v.decode()
     if issubclass(cls, Enum):
         return cls(v)
     return v
 
 
 def field_get_type(field: Field) -> Tuple[type, Optional[type]]:
     field_type = field.type
     if field_type is Ellipsis:
         return field_type, None
+    if field_type is Any:
+        return None, None
     if hasattr(field_type, "__origin__"):
         field_type = field.type.__origin__
     if not isinstance(field_type, type):
         return field_type, None
     if issubclass(field_type, ARRAYS) and hasattr(field.type, "__args__"):
         return field_type, field.type.__args__[0]
     return field_type, None
```

### Comparing `py_datastruct-0.3.0/datastruct/utils/fmt.py` & `py_datastruct-0.4.0/datastruct/utils/fmt.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/utils/misc.py` & `py_datastruct-0.4.0/datastruct/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/datastruct/utils/public.py` & `py_datastruct-0.4.0/datastruct/utils/public.py`

 * *Files identical despite different names*

### Comparing `py_datastruct-0.3.0/PKG-INFO` & `py_datastruct-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datastruct
-Version: 0.3.0
+Version: 0.4.0
 Summary: Combination of struct and dataclasses for easy parsing of binary formats
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

