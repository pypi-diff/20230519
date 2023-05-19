# Comparing `tmp/fickling-0.0.4.tar.gz` & `tmp/fickling-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fickling-0.0.4.tar", last modified: Wed Sep  7 16:00:49 2022, max compression
+gzip compressed data, was "fickling-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fickling-0.0.4.tar` & `fickling-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 16:00:49.520901 fickling-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-09-07 16:00:39.000000 fickling-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-09-07 16:00:49.520901 fickling-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2861 2022-09-07 16:00:39.000000 fickling-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 16:00:49.520901 fickling-0.0.4/fickling/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-09-07 16:00:39.000000 fickling-0.0.4/fickling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-07 16:00:39.000000 fickling-0.0.4/fickling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-09-07 16:00:39.000000 fickling-0.0.4/fickling/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     4820 2022-09-07 16:00:39.000000 fickling-0.0.4/fickling/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    31844 2022-09-07 16:00:39.000000 fickling-0.0.4/fickling/pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-09-07 16:00:39.000000 fickling-0.0.4/fickling/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 16:00:49.520901 fickling-0.0.4/fickling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-09-07 16:00:49.000000 fickling-0.0.4/fickling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-09-07 16:00:49.000000 fickling-0.0.4/fickling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-07 16:00:49.000000 fickling-0.0.4/fickling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-07 16:00:49.000000 fickling-0.0.4/fickling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-07 16:00:49.000000 fickling-0.0.4/fickling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-07 16:00:49.000000 fickling-0.0.4/fickling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-07 16:00:49.520901 fickling-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-09-07 16:00:39.000000 fickling-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 16:00:49.520901 fickling-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-09-07 16:00:39.000000 fickling-0.0.4/test/test_crashes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-09-07 16:00:39.000000 fickling-0.0.4/test/test_pickle.py
+-rw-r--r--   0        0        0     7652 2023-05-19 16:32:54.507444 fickling-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2885 2023-05-19 16:32:54.507444 fickling-0.0.5/README.md
+-rw-r--r--   0        0        0       22 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/__main__.py
+-rw-r--r--   0        0        0     5019 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/analysis.py
+-rw-r--r--   0        0        0     6152 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/cli.py
+-rw-r--r--   0        0        0    45956 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/pickle.py
+-rw-r--r--   0        0        0     2577 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/tracing.py
+-rw-r--r--   0        0        0     1884 2023-05-19 16:32:54.507444 fickling-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 fickling-0.0.5/PKG-INFO
```

### Comparing `fickling-0.0.4/LICENSE` & `fickling-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fickling-0.0.4/README.md` & `fickling-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # Fickling
 
 Fickling is a decompiler, static analyzer, and bytecode rewriter for Python
 [pickle](https://docs.python.org/3/library/pickle.html) object serializations.
 
-Pickled Python objects are in fact bytecode that is interpreted by a stack-based virtual machine
-built into Python called the "Pickle Machine". Fickling can take pickled data streams and decompile them into
-human-readable Python code that, when executed, will deserialize to the original serialized object.
-
-The authors do not prescribe any meaning to the “F” in Fickling; it could stand for “fickle,” … or something else.
-Divining its meaning is a personal journey in discretion and is left as an exercise to the reader.
+Pickled Python objects are in fact bytecode that is interpreted by a stack-based
+virtual machine built into Python called the "Pickle Machine". Fickling can take
+pickled data streams and decompile them into human-readable Python code that,
+when executed, will deserialize to the original serialized object.
+
+The authors do not prescribe any meaning to the “F” in Fickling; it could stand
+for “fickle,” … or something else. Divining its meaning is a personal journey
+in discretion and is left as an exercise to the reader.
 
 Learn more about it in our [blog post](https://blog.trailofbits.com/2021/03/15/never-a-dill-moment-exploiting-machine-learning-pickle-files/)
 and [DEF CON 2021 talk](https://www.youtube.com/watch?v=bZ0m_H_dEJI).
 
 ## Installation
 
 Fickling has been tested on Python 3.6 through Python 3.9 and has very few dependencies.
 It can be installed through pip:
+
+```bash
+python -m pip install fickling
 ```
-pip3 install fickling
-```
+
 This installs both the library and the command line utility.
 
 ## Usage
 
 Fickling can be run programmatically:
+
 ```python
 >>> import ast
 >>> import pickle
 >>> from fickling.pickle import Pickled
 >>> print(ast.dump(Pickled.load(pickle.dumps([1, 2, 3, 4])).ast, indent=4))
 Module(
     body=[
@@ -41,33 +46,38 @@
                     Constant(value=2),
                     Constant(value=3),
                     Constant(value=4)],
                 ctx=Load()))])
 ```
 
 Fickling can also be run as a command line utility:
-```bash
+
+```console
 $ fickling pickled.data
 result = [1, 2, 3, 4]
 ```
 
-This is of course a simple example. However, Python pickle bytecode can run arbitrary Python commands (such as 
-`exec` or `os.system`) so it is a security risk to unpickle untrusted data. You can test for common patterns of
+This is of course a simple example. However, Python pickle bytecode can run
+arbitrary Python commands (such as `exec` or `os.system`) so it is a security
+risk to unpickle untrusted data. You can test for common patterns of
 malicious pickle files with the `--check-safety` option:
-```bash
+
+```console
 $ fickling --check-safety pickled.data
 Warning: Fickling failed to detect any overtly unsafe code, but the pickle file may still be unsafe.
 Do not unpickle this file if it is from an untrusted source!
 ```
 
-You can also safely trace the execution of the Pickle virtual machine without exercising any malicious code with the
-`--trace` option.
+You can also safely trace the execution of the Pickle virtual machine without
+exercising any malicious code with the `--trace` option.
 
-Finally, you can inject arbitrary Python code that will be run on unpickling into an existing pickle file with the
-`--inject` option.
+Finally, you can inject arbitrary Python code that will be run on unpickling
+into an existing pickle file with the `--inject` option.
 
 ## License
 
 This utility was developed by [Trail of Bits](https://www.trailofbits.com/).
 It is licensed under the [GNU Lesser General Public License v3.0](LICENSE).
-[Contact us](mailto:opensource@trailofbits.com) if you're looking for an exception to the terms.
+[Contact us](mailto:opensource@trailofbits.com) if you're looking for an
+exception to the terms.
+
 © 2021, Trail of Bits.
```

### Comparing `fickling-0.0.4/fickling/cli.py` & `fickling-0.0.5/fickling/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,172 @@
-from argparse import ArgumentParser
 import sys
-from typing import List, Optional, Tuple
+from argparse import ArgumentParser
+from typing import List, Optional
 
 if sys.version_info >= (3, 9):
     from ast import unparse
 else:
     from astunparse import unparse
 
-from . import pickle, tracing, version
+from . import __version__, pickle, tracing
 from .analysis import check_safety
 
 
 def main(argv: Optional[List[str]] = None) -> int:
     if argv is None:
         argv = sys.argv
 
-    parser = ArgumentParser(description="fickle is a static analyzer and interpreter for Python pickle data")
-    parser.add_argument("PICKLE_FILE", type=str, nargs="?", default="-", help="path to the pickle file to either "
-                                                                              "analyze or create (default is '-' for "
-                                                                              "STDIN/STDOUT)")
+    parser = ArgumentParser(
+        description="fickle is a static analyzer and interpreter for Python pickle data"
+    )
+    parser.add_argument(
+        "PICKLE_FILE",
+        type=str,
+        nargs="?",
+        default="-",
+        help="path to the pickle file to either "
+        "analyze or create (default is '-' for "
+        "STDIN/STDOUT)",
+    )
     options = parser.add_mutually_exclusive_group()
-    options.add_argument("--inject", "-i", type=str, default=None, help="inject the specified Python code to be run at "
-                                                                        "the end of depickling, and output the "
-                                                                        "resulting pickle data")
+    options.add_argument(
+        "--inject",
+        "-i",
+        type=str,
+        default=None,
+        help="inject the specified Python code to be run at the end of depickling, "
+        "and output the resulting pickle data",
+    )
+    parser.add_argument(
+        "--inject-target",
+        type=int,
+        default=0,
+        help="some machine learning frameworks stack multiple pickles into the same model file; "
+        "this option specifies the index of the pickle file in which to inject the code from the "
+        "`--inject` command (default is 0)",
+    )
     options.add_argument("--create", "-c", type=str, default=None)
-    parser.add_argument("--run-last", "-l", action="store_true", help="used with --inject to have the injected code "
-                                                                      "run after the existing pickling code in "
-                                                                      "PICKLE_FILE (default is for the injected code "
-                                                                      "to be run before the existing code)")
-    parser.add_argument("--replace-result", "-r", action="store_true",
-                        help="used with --inject to replace the unpickling result of the code in PICKLE_FILE with the "
-                             "return value of the injected code. Either way, the preexisting pickling code is still "
-                             "executed.")
-    options.add_argument("--check-safety", "-s", action="store_true",
-                         help="test if the given pickle file is known to be unsafe. If so, exit with non-zero status. "
-                              "This test is not guaranteed correct; the pickle file may still be unsafe even if this "
-                              "check exits with code zero.")
-    parser.add_argument("--trace", "-t", action="store_true",
-                        help="print a runtime trace while interpreting the input pickle file")
+    parser.add_argument(
+        "--run-last",
+        "-l",
+        action="store_true",
+        help="used with --inject to have the injected code "
+        "run after the existing pickling code in "
+        "PICKLE_FILE (default is for the injected code "
+        "to be run before the existing code)",
+    )
+    parser.add_argument(
+        "--replace-result",
+        "-r",
+        action="store_true",
+        help=(
+            "used with --inject to replace the unpickling result of the code in PICKLE_FILE "
+            "with the return value of the injected code. Either way, the preexisting pickling "
+            "code is still executed."
+        ),
+    )
+    options.add_argument(
+        "--check-safety",
+        "-s",
+        action="store_true",
+        help=(
+            "test if the given pickle file is known to be unsafe. If so, exit with non-zero "
+            "status. This test is not guaranteed correct; the pickle file may still be unsafe "
+            "even if this check exits with code zero."
+        ),
+    )
+    parser.add_argument(
+        "--trace",
+        "-t",
+        action="store_true",
+        help="print a runtime trace while interpreting the input pickle file",
+    )
     parser.add_argument("--version", "-v", action="store_true", help="print the version and exit")
 
     args = parser.parse_args(argv[1:])
 
     if args.version:
         if sys.stdout.isatty():
-            print(f"fickling version {version()}")
+            print(f"fickling version {__version__}")
         else:
-            print(version())
+            print(__version__)
         return 0
 
     if args.create is None:
         if args.PICKLE_FILE == "-":
             if hasattr(sys.stdin, "buffer") and sys.stdin.buffer is not None:
                 file = sys.stdin.buffer
             else:
                 file = sys.stdin
         else:
             file = open(args.PICKLE_FILE, "rb")
         try:
-            pickled = pickle.Pickled.load(file)
+            stacked_pickled = pickle.StackedPickle.load(file)
+        except pickle.PickleDecodeError as e:
+            sys.stderr.write(f"Error: {str(e)}\n")
+            return 1
         finally:
             file.close()
 
         if args.inject is not None:
+            if args.inject_target >= len(stacked_pickled):
+                sys.stderr.write(
+                    f"Error: --inject-target {args.inject_target} is too high; there are only "
+                    f"{len(stacked_pickled)} stacked pickle files in the input\n"
+                )
+                return 1
+            if hasattr(sys.stdout, "buffer") and sys.stdout.buffer is not None:
+                buffer = sys.stdout.buffer
+            else:
+                buffer = sys.stdout
+            for pickled in stacked_pickled[: args.inject_target]:
+                pickled.dump(buffer)
+            pickled = stacked_pickled[args.inject_target]
             if not isinstance(pickled[-1], pickle.Stop):
-                sys.stderr.write("Error: The last opcode of the input file was expected to be STOP, but was in fact "
-                                 f"{pickled[-1].info.name}")
+                sys.stderr.write(
+                    "Warning: The last opcode of the input file was expected to be STOP, but was "
+                    f"in fact {pickled[-1].info.name}"
+                )
             pickled.insert_python_eval(
                 args.inject,
                 run_first=not args.run_last,
-                use_output_as_unpickle_result=args.replace_result
+                use_output_as_unpickle_result=args.replace_result,
             )
-            if hasattr(sys.stdout, "buffer") and sys.stdout.buffer is not None:
-                pickled.dump(sys.stdout.buffer)
-            else:
-                pickled.dump(sys.stdout)
+            pickled.dump(buffer)
+            for pickled in stacked_pickled[args.inject_target + 1 :]:
+                pickled.dump(buffer)
         elif args.check_safety:
-            return [1, 0][check_safety(pickled)]
-        elif args.trace:
-            trace = tracing.Trace(pickle.Interpreter(pickled))
-            print(unparse(trace.run()))
+            was_safe = True
+            for pickled in stacked_pickled:
+                if not check_safety(pickled):
+                    was_safe = False
+            return [1, 0][was_safe]
         else:
-            print(unparse(pickled.ast))
+            var_id = 0
+            for i, pickled in enumerate(stacked_pickled):
+                interpreter = pickle.Interpreter(
+                    pickled, first_variable_id=var_id, result_variable=f"result{i}"
+                )
+                if args.trace:
+                    trace = tracing.Trace(interpreter)
+                    print(unparse(trace.run()))
+                else:
+                    print(unparse(interpreter.to_ast()))
+                var_id = interpreter.next_variable_id
     else:
-        pickled = pickle.Pickled([
-            pickle.Global.create("__builtin__", "eval"),
-            pickle.Mark(),
-            pickle.Unicode(args.create.encode("utf-8")),
-            pickle.Tuple(),
-            pickle.Reduce(),
-            pickle.Stop()
-        ])
+        pickled = pickle.Pickled(
+            [
+                pickle.Global.create("__builtin__", "eval"),
+                pickle.Mark(),
+                pickle.Unicode(args.create.encode("utf-8")),
+                pickle.Tuple(),
+                pickle.Reduce(),
+                pickle.Stop(),
+            ]
+        )
         if args.PICKLE_FILE == "-":
             file = sys.stdout
             if hasattr(file, "buffer") and file.buffer is not None:
                 file = file.buffer
         else:
             file = open(args.PICKLE_FILE, "wb")
         try:
```

### Comparing `fickling-0.0.4/fickling/pickle.py` & `fickling-0.0.5/fickling/pickle.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 import ast
 import distutils.sysconfig as sysconfig
-from abc import abstractmethod
+import struct
+import sys
+from abc import ABC, abstractmethod
 from collections.abc import MutableSequence, Sequence
+from enum import Enum
+from io import BytesIO
 from pathlib import Path
-from pickletools import genops, opcodes, OpcodeInfo
+from pickletools import OpcodeInfo, genops, opcodes
 from typing import (
     Any,
     BinaryIO,
     ByteString,
     Dict,
     FrozenSet,
     Generic,
     Iterable,
     Iterator,
     List,
     Optional,
-    overload,
     Set,
     Type,
     TypeVar,
     Union,
+    overload,
+)
+from typing import (
+    Tuple as TupleType,
 )
-
-import sys
 
 T = TypeVar("T")
 
 if sys.version_info < (3, 9):
     # abstract collections were not subscriptable until Python 3.9
     OpcodeSequence = MutableSequence
     GenericSequence = Sequence
 
     def make_constant(*args, **kwargs) -> ast.Constant:
-        # prior to Python 3.9, the ast.Constant class did not have a `kind` member, but the `astunparse` module
-        # expects that!
+        # prior to Python 3.9, the ast.Constant class did not have a `kind` member, but the
+        # `astunparse` module expects that!
         ret = ast.Constant(*args, **kwargs)
         if not hasattr(ret, "kind"):
             setattr(ret, "kind", None)
         return ret
 
-
 else:
     OpcodeSequence = MutableSequence["Opcode"]
     GenericSequence = Sequence[T]
     make_constant = ast.Constant
 
 BUILTIN_MODULE_NAMES: FrozenSet[str] = frozenset(sys.builtin_module_names)
 
@@ -76,17 +80,15 @@
         position: Optional[int] = None,
         data: Optional[bytes] = None,
         *,
         info: Optional[OpcodeInfo] = None,
     ):
         if self.__class__ is Opcode:
             if info is None:
-                raise TypeError(
-                    "The Opcode class must be constructed with the `info` argument"
-                )
+                raise TypeError("The Opcode class must be constructed with the `info` argument")
         elif info is not None and info != self.info:
             raise ValueError(
                 f"Invalid info type for {self.__class__.__name__}; expected {self.info!r} but got "
                 f"{info!r}"
             )
         self.arg: Any = argument
         self.pos: Optional[int] = position
@@ -103,50 +105,56 @@
             return self._data
 
     @data.setter
     def data(self, value: bytes):
         self._data = value
 
     def encode(self) -> bytes:
+        return self.encode_opcode() + self.encode_body()
+
+    def encode_opcode(self) -> bytes:
+        return self.info.code.encode("latin-1")
+
+    def encode_body(self) -> bytes:
         if self.info.arg is None or self.info.arg.n == 0:
-            return self.info.code.encode("latin-1")
+            return b""
         raise NotImplementedError(
-            f"encode() is not yet implemented for opcode {self.__class__.__name__}"
+            f"encode_body() is not yet implemented for opcode {self.__class__.__name__}"
         )
 
     def __new__(cls, *args, **kwargs):
         if cls is Opcode:
             if "info" not in kwargs:
-                raise ValueError(
-                    f"You must provide an `info` argument to construct {cls.__name__}"
-                )
+                raise ValueError(f"You must provide an `info` argument to construct {cls.__name__}")
             else:
                 info = kwargs["info"]
             if info.name in OPCODES_BY_NAME:
                 del kwargs["info"]
                 return OPCODES_BY_NAME[info.name](*args, **kwargs)
             else:
                 raise NotImplementedError(f"TODO: Add support for Opcode {info.name}")
         return super().__new__(cls)
 
     def run(self, interpreter: "Interpreter"):
-        raise NotImplementedError(
-            f"TODO: Add support for Pickle opcode {self.info.name}"
-        )
+        raise NotImplementedError(f"TODO: Add support for Pickle opcode {self.info.name}")
 
     def __init_subclass__(cls, **kwargs):
-        if cls.__name__ not in ("NoOp", "StackSliceOpcode", "ConstantOpcode"):
+        if cls.__name__ not in (
+            "NoOp",
+            "StackSliceOpcode",
+            "ConstantOpcode",
+            "DynamicLength",
+            "ConstantInt",
+        ):
             if not hasattr(cls, "name") or cls.name is None:
                 raise TypeError("Opcode subclasses must define a name")
             elif cls.name in OPCODES_BY_NAME:
                 raise TypeError(f"An Opcode named {cls.name} is already defined")
             elif cls.name not in OPCODE_INFO_BY_NAME:
-                raise TypeError(
-                    f"An Opcode named {cls.name} is not defined in `pickletools`"
-                )
+                raise TypeError(f"An Opcode named {cls.name} is not defined in `pickletools`")
             OPCODES_BY_NAME[cls.name] = cls
             setattr(cls, "info", OPCODE_INFO_BY_NAME[cls.name])
             # find the associated `pickletools` OpcodeInfo:
         return super().__init_subclass__(**kwargs)
 
     def __repr__(self):
         if self.pos is None:
@@ -156,14 +164,70 @@
         if self.has_data():
             d = f", data={self.data!r}"
         else:
             d = ""
         return f"{self.__class__.__name__}(info={self.info!r}, argument={self.arg!r}{d}{p})"
 
 
+class Endianness(Enum):
+    Little = "<"
+    Big = ">"
+
+
+class DynamicLength(Opcode, ABC):
+    length_signed: bool = False
+    length_bytes: int = 4
+    length_endianness: Endianness = Endianness.Little
+    struct_types = {1: "b", 2: "h", 4: "i", 8: "q"}
+    min_value: int
+    max_value: int
+
+    def __init_subclass__(cls, **kwargs):
+        ret = super().__init_subclass__(**kwargs)
+        length_bits = cls.length_bytes * 8
+        if cls.length_signed:
+            cls.min_value = 1 << (length_bits - 1)
+            cls.max_value = cls.min_value ^ (2**length_bits - 1)
+        else:
+            cls.min_value = 0
+            cls.max_value = 2**length_bits - 1
+        return ret
+
+    @classmethod
+    def encode_length(cls, length: int) -> bytes:
+        if cls.length_bytes not in cls.struct_types:
+            raise TypeError(
+                f"{cls.__name__}.struct_types does not include a value for "
+                f"{cls.__name__}.length_bytes = {cls.length_bytes}"
+            )
+        if length < cls.min_value or length > cls.max_value:
+            raise ValueError(
+                f"Invalid length {length}: {cls.__name__} can only represent lengths in the range "
+                f"[{cls.min_value}, {cls.max_value}]"
+            )
+        st = cls.struct_types[cls.length_bytes]
+        if not cls.length_signed:
+            st = st.upper()
+        return struct.pack(f"{cls.length_endianness.value}{st}", length)
+
+    def encode(self) -> bytes:
+        body = self.encode_body()
+        return self.encode_opcode() + self.encode_length(len(body)) + body
+
+    @classmethod
+    def validate(cls, obj):
+        length = len(cls(obj).encode_body())
+        if length < cls.min_value or length > cls.max_value:
+            raise ValueError(
+                f"Invalid object {obj!r}: {cls.__name__} can only represent objects with lengths "
+                f"in the range [{cls.min_value}, {cls.max_value}]"
+            )
+        return obj
+
+
 class NoOp(Opcode):
     def run(self, interpreter: "Interpreter"):
         pass
 
 
 def raw_unicode_escape(byte_string: bytes) -> str:
     s = []
@@ -180,33 +244,119 @@
         else:
             s.append(f"\\u{b:04x}")
     s.append("\n")
     return "".join(s)
 
 
 class ConstantOpcode(Opcode):
+    ConstantOpcodePriorities: Dict[Type["ConstantOpcode"], int] = {}
+    priority: int
+
     def run(self, interpreter: "Interpreter"):
         interpreter.stack.append(make_constant(self.arg))
 
+    def __init_subclass__(cls, **kwargs):
+        ret = super().__init_subclass__(**kwargs)
+        if not cls.__name__ == "ConstantInt":
+            if cls.validate.__code__ == ConstantOpcode.validate.__code__:
+                raise TypeError(f"{cls.__name__} must implement the validate method")
+            elif (
+                not hasattr(cls, "priority")
+                or not isinstance(cls.priority, int)
+                or cls.priority is None
+            ):
+                raise TypeError(
+                    f"{cls.__name__} must define an integer priority used for auto-instantiation "
+                    "from ConstantOpcode.new(...)"
+                )
+            ConstantOpcode.ConstantOpcodePriorities[cls] = cls.priority
+        return ret
+
+    @classmethod
+    def validate(cls, obj):
+        """
+        Validates whether obj can be used to instantiate a new instance of this class using new(...)
+
+        Returning the value of the object to be saved to the constant
+        Or throwing a ValueError if obj cannot be used to instantiate this type of constant
+        """
+        raise NotImplementedError()
+
+    @classmethod
+    def new(cls: Type[T], obj) -> T:
+        for subclass, _ in sorted(
+            ConstantOpcode.ConstantOpcodePriorities.items(), key=lambda kv: kv[1]
+        ):
+            if not issubclass(subclass, cls):
+                continue
+            try:
+                return subclass(subclass.validate(obj))
+            except ValueError:
+                pass
+        raise ValueError(
+            "There is no subclass of ConstantOpcode that handles objects of type "
+            f"{type(obj)!r} for {obj!r}"
+        )
+
+
+class ConstantInt(ConstantOpcode, ABC):
+    signed: bool = False
+    num_bytes: int = 4
+    endianness: Endianness = Endianness.Little
+    struct_types = {1: "b", 2: "h", 4: "i", 8: "q"}
+    min_value: int
+    max_value: int
+
+    def __init_subclass__(cls, **kwargs):
+        ret = super().__init_subclass__(**kwargs)
+        length_bits = cls.num_bytes * 8
+        if cls.signed:
+            cls.min_value = 1 << (length_bits - 1)
+            cls.max_value = cls.min_value ^ (2**length_bits - 1)
+        else:
+            cls.min_value = 0
+            cls.max_value = 2**length_bits - 1
+        return ret
+
+    def encode_body(self) -> bytes:
+        st = self.struct_types[self.num_bytes]
+        if not self.signed:
+            st = st.upper()
+        return struct.pack(f"{self.endianness.value}{st}")
+
+    @classmethod
+    def validate(cls, obj):
+        if not isinstance(obj, int):
+            raise ValueError(f"{cls.__name__} can only be instantiated from integers, not {obj!r}")
+        elif cls.num_bytes not in cls.struct_types:
+            raise TypeError(
+                f"{cls.__name__}.struct_types does not include a value for "
+                f"{cls.__name__}.length_bytes = {cls.num_bytes}"
+            )
+        elif obj < cls.min_value or obj > cls.max_value:
+            raise ValueError(
+                f"Invalid value {obj!r}: {cls.__name__} can only represent lengths in the range "
+                f"[{cls.min_value}, {cls.max_value}]"
+            )
+        return obj
+
 
 class StackSliceOpcode(Opcode):
     def run(self, interpreter: "Interpreter", stack_slice: List[ast.expr]):
         raise NotImplementedError(f"{self.__class__.__name__} must implement run()")
 
     def __init_subclass__(cls, **kwargs):
         ret = super().__init_subclass__(**kwargs)
         orig_run = cls.run
 
         def run_wrapper(self, interpreter: "Interpreter"):
             args = []
             while True:
                 if not interpreter.stack:
-                    raise ValueError(
-                        "Exhausted the stack while searching for a MarkObject!"
-                    )
+                    raise ValueError("Exhausted the stack while searching for a MarkObject!")
                 obj = interpreter.stack.pop()
                 if isinstance(obj, MarkObject):
                     break
                 else:
                     args.append(obj)
             args = list(reversed(args))
             return orig_run(self, interpreter, args)
@@ -224,26 +374,34 @@
         self.likely_safe_imports: Set[str] = set()
 
     def _process_import(self, node: Union[ast.Import, ast.ImportFrom]):
         self.imports.append(node)
         if isinstance(node, ast.ImportFrom) and is_std_module(node.module):
             self.likely_safe_imports |= {name.name for name in node.names}
 
-    def visit_Import(self, node: ast.Import):
+    def visit_Import(self, node: ast.Import):  # noqa: N802
         self._process_import(node)
 
-    def visit_ImportFrom(self, node: ast.ImportFrom):
+    def visit_ImportFrom(self, node: ast.ImportFrom):  # noqa: N802
         self._process_import(node)
 
-    def visit_Call(self, node: ast.Call):
+    def visit_Call(self, node: ast.Call):  # noqa: N802
         self.calls.append(node)
         if not isinstance(node.func, ast.Attribute) or node.func.attr != "__setstate__":
             self.non_setstate_calls.append(node)
 
 
+class PickleDecodeError(ValueError):
+    pass
+
+
+class EmptyPickleError(PickleDecodeError):
+    pass
+
+
 class Pickled(OpcodeSequence):
     def __init__(self, opcodes: Iterable[Opcode]):
         self._opcodes: List[Opcode] = list(opcodes)
         self._ast: Optional[ast.Module] = None
         self._properties: Optional[ASTProperties] = None
 
     def __len__(self) -> int:
@@ -256,95 +414,87 @@
         return self._opcodes[index]
 
     def insert(self, index: int, opcode: Opcode):
         self._opcodes.insert(index, opcode)
         self._ast = None
         self._properties = None
 
-    def insert_python_exec(
+    def insert_python(
         self,
-        exec_cmd: str,
+        *args,
+        module: str = "builtins",
+        attr: str = "eval",
         run_first: bool = True,
         use_output_as_unpickle_result: bool = False,
     ):
         if not isinstance(self[-1], Stop):
             raise ValueError("Expected the last opcode to be STOP")
-        """
-        Similar to what Evan did down below, this imports the builtin exec function
-        Exec works on statements, while eval works on expressions
-        """
-        self.insert(0, Global.create("__builtin__", "exec"))
-        self.insert(1, Mark())
-        # This might be a multiline exec, so lets just insert the payload one by one.
-        self.insert(2, Unicode(exec_cmd.encode("utf-8")))
-        self.insert(3, Tuple())
+        # we need to add the call to GLOBAL before the preexisting code, because the following code
+        # can sometimes mess up module lookup (somehow? I, Evan, don't fully understand why yet).
+        # So we set up the "import" of `__builtin__.eval` first, then set up the stack for a call
+        # to it, and then either immediately call the `eval` with a `Reduce` opcode (the default)
+        # or optionally insert the `Reduce` at the end (and hope that the existing code cleans up
+        # its stack so it remains how we left it!
+        # TODO: Add code to emulate the code afterward and confirm that the stack is sane!
+        i = 0
+        while isinstance(self[i], (Proto, Frame)):
+            i += 1
+        self.insert(i, Global.create(module, attr))
+        i += 1
+        self.insert(i, Mark())
+        i += 1
+        for arg in args:
+            self.insert(i, ConstantOpcode.new(arg))
+            i += 1
+        self.insert(i, Tuple())
+        i += 1
         if run_first:
-            self.insert(4, Reduce())
+            self.insert(i, Reduce())
             if use_output_as_unpickle_result:
                 self.insert(-1, Pop())
-        if not run_first:
+        else:
             if use_output_as_unpickle_result:
+                # the top of the stack should be the original unpickled value, but we can throw
+                # that away because we are replacing it with the result of calling eval:
                 self.insert(-1, Pop())
+                # now the top of the stack should be our original Global, Mark, Unicode,
+                # Tuple setup, ready for Reduce:
                 self.insert(-1, Reduce())
             else:
+                # we need to preserve the "real" output of the preexisting unpickling, which should
+                # be at the top of the stack, directly above our Tuple, Unicode, Mark, and Global
+                # stack items we added above.
+                # So, we have to save the original result to the memo. First, interpret the existing
+                # code to see which memo location it would be saved to:
                 interpreter = Interpreter(self)
                 interpreter.run()
                 memo_id = len(interpreter.memory)
                 self.insert(-1, Memoize())
                 self.insert(-1, Pop())
                 self.insert(-1, Reduce())
+                self.insert(-1, Pop())
                 self.insert(-1, Get.create(memo_id))
 
-        pass
+    insert_python_eval = insert_python
 
-    def insert_python_eval(
+    def insert_python_exec(
         self,
-        eval_cmd: str,
+        *args,
         run_first: bool = True,
         use_output_as_unpickle_result: bool = False,
     ):
-        if not isinstance(self[-1], Stop):
-            raise ValueError("Expected the last opcode to be STOP")
-        # we need to add the call to GLOBAL before the preexisting code, because the following code can sometimes
-        # mess up module look (somehow? I, Evan, don't fully understand why yet).
-        # So we set up the "import" of `__builtin__.eval` first, then set up the stack for a call to it,
-        # and then either immediately call the `eval` with a `Reduce` opcode (the default)
-        # or optionally insert the `Reduce` at the end (and hope that the existing code cleans up its stack so it
-        # remains how we left it! TODO: Add code to emulate the code afterward and confirm that the stack is sane!
-        self.insert(0, Global.create("__builtin__", "eval"))
-        self.insert(1, Mark())
-        self.insert(2, Unicode(eval_cmd.encode("utf-8")))
-        self.insert(3, Tuple())
-        if run_first:
-            self.insert(4, Reduce())
-            if use_output_as_unpickle_result:
-                self.insert(-1, Pop())
-        if not run_first:
-            if use_output_as_unpickle_result:
-                # the top of the stack should be the original unpickled value, but we can throw that away because
-                # we are replacing it with the result of calling eval:
-                self.insert(-1, Pop())
-                # now the top of the stack should be our original Global, Mark, Unicode, Tuple setup, ready for Reduce:
-                self.insert(-1, Reduce())
-            else:
-                # we need to preserve the "real" output of the preexisting unpickling, which should be at the top
-                # of the stack, directly above our Tuple, Unicode, Mark, and Global stack items we added above.
-                # So, we have to save the original result to the memo. First, interpret the existing code to see which
-                # memo location it would be saved to:
-                interpreter = Interpreter(self)
-                interpreter.run()
-                memo_id = len(interpreter.memory)
-                self.insert(-1, Memoize())
-                self.insert(-1, Pop())
-                self.insert(-1, Reduce())
-                self.insert(-1, Get.create(memo_id))
+        return self.insert_python(
+            *args,
+            module="builtins",
+            attr="exec",
+            run_first=run_first,
+            use_output_as_unpickle_result=use_output_as_unpickle_result,
+        )
 
-    def __setitem__(
-        self, index: Union[int, slice], item: Union[Opcode, Iterable[Opcode]]
-    ):
+    def __setitem__(self, index: Union[int, slice], item: Union[Opcode, Iterable[Opcode]]):
         self._opcodes[index] = item
         self._ast = None
         self._properties = None
 
     def __delitem__(self, index: int):
         del self._opcodes[index]
         self._ast = None
@@ -361,38 +511,75 @@
             file.write(opcode.data)
 
     @property
     def opcodes(self) -> Iterator[Opcode]:
         return iter(self)
 
     @staticmethod
+    def make_stream(data: Union[ByteString, BinaryIO]) -> BinaryIO:
+        if isinstance(data, (bytes, bytearray, ByteString)):
+            data = BytesIO(data)
+        elif (not hasattr(data, "seekable") or not data.seekable()) and hasattr(data, "read"):
+            data = BytesIO(data.read())
+        return data
+
+    @staticmethod
     def load(pickled: Union[ByteString, BinaryIO]) -> "Pickled":
-        if not isinstance(pickled, (bytes, bytearray)) and hasattr(pickled, "read"):
-            pickled = pickled.read()
+        pickled = Pickled.make_stream(pickled)
+        first_pos = pickled.tell()
         opcodes: List[Opcode] = []
-        for info, arg, pos in genops(pickled):
-            if info.arg is None or info.arg.n == 0:
-                if pos is not None:
-                    data = pickled[pos : pos + 1]
-                else:
-                    data = info.code
-            elif info.arg.n > 0 and pos is not None:
-                data = pickled[pos : pos + 1 + info.arg.n]
+
+        try:
+            for info, arg, pos in genops(pickled):
+                pos_before = pickled.tell()
+                try:
+                    if (
+                        pos is not None
+                        and opcodes
+                        and opcodes[-1].pos is not None
+                        and not opcodes[-1].has_data()
+                        and opcodes[-1].pos < pos
+                    ):
+                        pickled.seek(opcodes[-1].pos)
+                        opcodes[-1].data = pickled.read(pos - opcodes[-1].pos)
+                    if pos is not None:
+                        pickled.seek(pos)
+                    if info.arg is None or info.arg.n == 0:
+                        if pos is not None:
+                            data = None
+                        else:
+                            data = info.code.encode("utf-8")
+                    elif info.arg.n > 0 and pos is not None:
+                        data = pickled.read(len(info.code) + info.arg.n)
+                        if len(data) != len(info.code) + info.arg.n:
+                            raise PickleDecodeError(
+                                f"Error decoding opcode {info.name} at offset {pos}: "
+                                f"Expected {len(info.code) + info.arg.n} bytes of data but only "
+                                f"read {len(data)}"
+                            )
+                    else:
+                        data = None
+                    opcodes.append(Opcode(info=info, argument=arg, data=data, position=pos))
+                finally:
+                    # Need to reset the position within the file so as not to confuse genops
+                    pickled.seek(pos_before)
+        except ValueError as e:
+            if opcodes:
+                raise PickleDecodeError(e)
             else:
-                data = None
-            if (
-                pos is not None
-                and opcodes
-                and opcodes[-1].pos is not None
-                and not opcodes[-1].has_data()
-            ):
-                opcodes[-1].data = pickled[opcodes[-1].pos : pos]
-            opcodes.append(Opcode(info=info, argument=arg, data=data, position=pos))
-        if opcodes and not opcodes[-1].has_data() and opcodes[-1].pos is not None:
-            opcodes[-1].data = pickled[opcodes[-1].pos :]
+                raise EmptyPickleError()
+        if opcodes:
+            if opcodes[-1].pos is not None:
+                if opcodes[-1].has_data():
+                    last_pos = opcodes[-1].pos + len(opcodes[-1].data)
+                else:
+                    last_pos = opcodes[-1].pos + len(opcodes[-1].info.code)
+                pickled.seek(last_pos)
+        else:
+            pickled.seek(first_pos)
         return Pickled(opcodes)
 
     @property
     def properties(self) -> ASTProperties:
         if self._properties is None:
             self._properties = ASTProperties()
             self._properties.visit(self.ast)
@@ -406,25 +593,35 @@
     @property
     def has_call(self) -> bool:
         """Checks whether unpickling would cause a function call"""
         return bool(self.properties.calls)
 
     @property
     def has_non_setstate_call(self) -> bool:
-        """Checks whether unpickling would cause a call to a function other than object.__setstate__"""
+        """Checks whether unpickling would cause a call to a function other than
+        object.__setstate__"""
         return bool(self.properties.non_setstate_calls)
 
     @property
     def is_likely_safe(self) -> bool:
         # `self.has_call` is probably safe as long as `not self.has_import`
         return not self.has_import and not self.has_non_setstate_call
 
     def unsafe_imports(self) -> Iterator[Union[ast.Import, ast.ImportFrom]]:
         for node in self.properties.imports:
-            if node.module in ("__builtin__", "os", "subprocess", "sys", "builtins", "socket"):
+            if node.module in (
+                "__builtin__",
+                "__builtins__",
+                "builtins",
+                "os",
+                "subprocess",
+                "sys",
+                "builtins",
+                "socket",
+            ):
                 yield node
             elif "eval" in (n.name for n in node.names):
                 yield node
 
     def non_standard_imports(self) -> Iterator[Union[ast.Import, ast.ImportFrom]]:
         for node in self.properties.imports:
             if not is_std_module(node.module):
@@ -459,17 +656,15 @@
         return len(self._stack)
 
     def pop(self):
         if not self._stack:
             if self.opcode is None:
                 raise IndexError("Stack is empty")
             else:
-                raise IndexError(
-                    f"Opcode {self.opcode!s} attempted to pop from an empty stack"
-                )
+                raise IndexError(f"Opcode {self.opcode!s} attempted to pop from an empty stack")
         else:
             return self._stack.pop()
 
     def push(self, obj: T):
         self._stack.append(obj)
 
     append = push
@@ -484,21 +679,18 @@
 class ModuleBody:
     def __init__(self, interpreter: "Interpreter"):
         self._list: List[ast.stmt] = []
         self.interpreter: Interpreter = interpreter
 
     def append(self, stmt: ast.stmt):
         lineno = len(self._list) + 1
-        if (
-            hasattr(stmt, "lineno")
-            and stmt.lineno is not None
-            and stmt.lineno != lineno
-        ):
+        if hasattr(stmt, "lineno") and stmt.lineno is not None and stmt.lineno != lineno:
             raise ValueError(
-                f"Statement {stmt} was expected to have line number {lineno} but instead has {stmt.lineno}"
+                f"Statement {stmt} was expected to have line number {lineno} but instead has "
+                f"{stmt.lineno}"
             )
         setattr(stmt, "lineno", lineno)
         self._list.append(stmt)
 
     def extend(self, stmts: Iterable[ast.stmt]):
         for stmt in stmts:
             self.append(stmt)
@@ -510,28 +702,70 @@
         return len(self._list)
 
     def __getitem__(self, index: Union[int, slice]) -> ast.stmt:
         return self._list[index]
 
 
 class Interpreter:
-    def __init__(self, pickled: Pickled):
+    def __init__(
+        self, pickled: Pickled, first_variable_id: int = 0, result_variable: str = "result"
+    ):
         self.pickled: Pickled = pickled
         self.memory: Dict[int, ast.expr] = {}
         self.stack: Stack[Union[ast.expr, MarkObject]] = Stack()
         self.module_body: ModuleBody = ModuleBody(self)
+        self.result_variable: str = result_variable
         self._module: Optional[ast.Module] = None
-        self._var_counter: int = 0
+        self._var_counter: int = first_variable_id
         self._opcodes: Iterator[Opcode] = iter(pickled)
 
+    @property
+    def next_variable_id(self) -> int:
+        return self._var_counter
+
     def to_ast(self) -> ast.Module:
         if self._module is None:
             self.run()
         return self._module
 
+    def unused_assignments(self) -> Dict[str, ast.Assign]:
+        if self._module is None:
+            self.run()
+        used: Set[str] = set()
+        defined: Set[str] = set()
+        assignments: Dict[str, ast.Assign] = {}
+        for statement in self.module_body:
+            # skip the last statement because it is always used
+            if isinstance(statement, ast.Assign):
+                if (
+                    len(statement.targets) == 1
+                    and isinstance(statement.targets[0], ast.Name)
+                    and statement.targets[0].id == "result"
+                ):
+                    # this is the return value of the program
+                    break
+                for target in statement.targets:
+                    if isinstance(target, ast.Name):
+                        defined.add(target.id)
+                        if target.id in assignments:
+                            # this should never happen, since Fickling constructs the AST
+                            sys.stderr.write(
+                                f"Warning: Duplicate declaration of variable {target.id}\n"
+                            )
+                        assignments[target.id] = statement
+                statement = statement.value
+            if statement is not None:
+                for node in ast.walk(statement):
+                    if isinstance(node, ast.Name):
+                        used.add(node.id)
+        return {varname: assignments[varname] for varname in defined - used}
+
+    def unused_variables(self) -> FrozenSet[str]:
+        return self.unused_assignments().keys()  # type: ignore
+
     def stop(self):
         self._opcodes = iter(())
 
     def run(self):
         while True:
             try:
                 self.step()
@@ -569,14 +803,31 @@
     def __str__(self):
         return ast.dump(self.to_ast())
 
 
 class Proto(NoOp):
     name = "PROTO"
 
+    @staticmethod
+    def create(version: int) -> "Proto":
+        return Proto(version)
+
+    def encode_body(self) -> bytes:
+        return bytes([self.version])
+
+    @property
+    def version(self) -> int:
+        if self.arg is None:
+            return 0
+        elif isinstance(self.arg, int):
+            return self.arg
+        else:
+            # Endianness shouldn't really matter here because there is only one byte for the version
+            return int.from_bytes(self.arg, "big", signed=False)
+
 
 class Global(Opcode):
     name = "GLOBAL"
 
     @staticmethod
     def create(module: str, attr: str) -> "Global":
         return Global(f"{module} {attr}")
@@ -588,54 +839,50 @@
     @property
     def attr(self) -> str:
         _, attribute, *_ = self.arg.split(" ")
         return attribute
 
     def run(self, interpreter: Interpreter):
         module, attr = self.module, self.attr
-        if module == "__builtin__":
+        if module in ("__builtin__", "__builtins__", "builtins"):
             # no need to emit an import for builtins!
             pass
         else:
             if sys.version_info < (3, 9):
                 # workaround for a bug in astunparse
                 alias = ast.alias(attr, asname=None)
             else:
                 alias = ast.alias(attr)
-            interpreter.module_body.append(
-                ast.ImportFrom(module=module, names=[alias], level=0)
-            )
+            interpreter.module_body.append(ast.ImportFrom(module=module, names=[alias], level=0))
         interpreter.stack.append(ast.Name(attr, ast.Load()))
 
     def encode(self) -> bytes:
-        return f"c{self.module}\n{self.attr}\n".encode("utf-8")
+        return f"c{self.module}\n{self.attr}\n".encode()
 
 
 class StackGlobal(NoOp):
     name = "STACK_GLOBAL"
 
     def run(self, interpreter: Interpreter):
         attr = interpreter.stack.pop()
         module = interpreter.stack.pop()
         if isinstance(module, ast.Constant):
             module = module.value
         if isinstance(attr, ast.Constant):
             attr = attr.value
-        if module == "__builtin__":
+        if module in ("__builtin__", "__builtins__", "builtins"):
             # no need to emit an import for builtins!
             pass
         else:
             if sys.version_info < (3, 9):
                 # workaround for a bug in astunparse
                 alias = ast.alias(attr, asname=None)
             else:
                 alias = ast.alias(attr)
-            interpreter.module_body.append(
-                ast.ImportFrom(module=module, names=[alias], level=0)
-            )
+            interpreter.module_body.append(ast.ImportFrom(module=module, names=[alias], level=0))
         interpreter.stack.append(ast.Name(attr, ast.Load()))
 
 
 class Put(Opcode):
     name = "PUT"
 
     def run(self, interpreter: Interpreter):
@@ -683,27 +930,50 @@
     def run(self, interpreter: Interpreter):
         top = interpreter.stack.pop()
         mid = interpreter.stack.pop()
         bot = interpreter.stack.pop()
         interpreter.stack.append(ast.Tuple((bot, mid, top), ast.Load()))
 
 
+class AddItems(Opcode):
+    name = "ADDITEMS"
+
+    def run(self, interpreter: Interpreter):
+        to_add = []
+        while interpreter.stack:
+            obj = interpreter.stack.pop()
+            if isinstance(obj, MarkObject):
+                break
+            to_add.append(obj)
+        else:
+            raise ValueError("Exhausted the stack while searching for a MarkObject!")
+        if not interpreter.stack:
+            raise ValueError("Stack was empty; expected a pyset")
+        pyset = interpreter.stack.pop()
+        if not isinstance(pyset, ast.Set):
+            raise ValueError(
+                f"{pyset!r} was expected to be a set-like object with an `add` function"
+            )
+        pyset.elts.extend(reversed(to_add))
+
+
 class Reduce(Opcode):
     name = "REDUCE"
 
     def run(self, interpreter: Interpreter):
         args = interpreter.stack.pop()
         func = interpreter.stack.pop()
         if isinstance(args, ast.Tuple):
             call = ast.Call(func, list(args.elts), [])
         else:
             call = ast.Call(func, [ast.Starred(args)], [])
         # Any call to reduce can have global side effects, since it runs arbitrary Python code.
-        # However, if we just save it to the stack, then it might not make it to the final AST unless the stack
-        # value is actually used. So save the result to a temp variable, and then put that on the stack:
+        # However, if we just save it to the stack, then it might not make it to the final AST
+        # unless the stack value is actually used. So save the result to a temp variable, and then
+        # put that on the stack:
         var_name = interpreter.new_variable(call)
         interpreter.stack.append(ast.Name(var_name, ast.Load()))
 
 
 class Mark(Opcode):
     name = "MARK"
 
@@ -714,41 +984,70 @@
 class Pop(Opcode):
     name = "POP"
 
     def run(self, interpreter: Interpreter):
         interpreter.stack.pop()
 
 
-class Unicode(ConstantOpcode):
-    name = "UNICODE"
+class ShortBinUnicode(DynamicLength, ConstantOpcode):
+    name = "SHORT_BINUNICODE"
+    priority = 5000
+    length_bytes = 1
 
-    def encode(self) -> bytes:
-        return self.info.code.encode("latin-1") + raw_unicode_escape(self.arg).encode(
-            "utf-8"
-        )
+    @classmethod
+    def validate(cls, obj: str) -> bytes:
+        if not isinstance(obj, str):
+            raise ValueError(f"obj must be of type str, not {obj!r}")
+        return super().validate(obj.encode("utf-8"))
+
+    def encode_body(self) -> bytes:
+        text = self.arg
+        if isinstance(text, str):
+            text = text.encode("utf-8")
+        return text
 
 
-class BinUnicode(ConstantOpcode):
+class BinUnicode(ShortBinUnicode):
     name = "BINUNICODE"
+    priority = ShortBinUnicode.priority + 1
+    length_bytes = 4
 
 
-class ShortBinUnicode(BinUnicode):
-    name = "SHORT_BINUNICODE"
+class BinUnicode8(BinUnicode):
+    name = "BINUNICODE8"
+    priority = BinUnicode.priority + 1
+    length_bytes = 8
 
-    def encode(self) -> bytes:
-        text = self.arg
-        if isinstance(text, str):
-            text = text.encode("utf-8")
-        if len(text) > 0xFF:
-            raise ValueError(f"{self.arg!r} is too long for a {self.name}")
-        return self.info.code.encode("latin-1") + bytes([len(text)]) + text
+
+class Unicode(ConstantOpcode):
+    name = "UNICODE"
+    priority = BinUnicode8.priority + 1
+
+    @classmethod
+    def validate(cls, obj: str) -> bytes:
+        if not isinstance(obj, str):
+            raise ValueError(f"{cls.__name__}.new expects a str object, not {obj!r}")
+        return obj.encode("utf-8")
+
+    def encode_body(self) -> bytes:
+        return raw_unicode_escape(self.arg).encode("utf-8")
 
 
 class String(ConstantOpcode):
     name = "STRING"
+    priority = Unicode.priority + 1
+
+    def encode_body(self) -> bytes:
+        return repr(self.arg).encode("utf-8")
+
+    @classmethod
+    def validate(cls, obj):
+        if not isinstance(obj, str):
+            raise ValueError(f"String must be instantiated from a str, not {obj!r}")
+        return obj
 
 
 class NewObj(Opcode):
     name = "NEWOBJ"
 
     def run(self, interpreter: Interpreter):
         args = interpreter.stack.pop()
@@ -853,37 +1152,35 @@
     @property
     def memo_id(self) -> int:
         return int(self.arg)
 
     def run(self, interpreter: Interpreter):
         interpreter.stack.append(interpreter.memory[self.memo_id])
 
-    def encode(self) -> bytes:
-        return self.info.code.encode("latin-1") + f"{self.memo_id}\n".encode("utf-8")
+    def encode_body(self) -> bytes:
+        return f"{self.memo_id}\n".encode()
 
     @staticmethod
     def create(memo_id: int) -> "Get":
-        return Get(f"{memo_id}\n".encode("utf-8"))
+        return Get(f"{memo_id}\n".encode())
 
 
 class SetItems(StackSliceOpcode):
     name = "SETITEMS"
 
     def run(self, interpreter: Interpreter, stack_slice: List[ast.expr]):
         pydict = interpreter.stack.pop()
         update_dict_keys = []
         update_dict_values = []
         for key, value in zip(stack_slice[::2], stack_slice[1::2]):
             update_dict_keys.append(key)
             update_dict_values.append(value)
         if isinstance(pydict, ast.Dict) and not pydict.keys:
             # the dict is empty, so add a new one
-            interpreter.stack.append(
-                ast.Dict(keys=update_dict_keys, values=update_dict_values)
-            )
+            interpreter.stack.append(ast.Dict(keys=update_dict_keys, values=update_dict_values))
         else:
             dict_name = interpreter.new_variable(pydict)
             update_dict = ast.Dict(keys=update_dict_keys, values=update_dict_values)
             interpreter.module_body.append(
                 ast.Expr(
                     ast.Call(
                         ast.Attribute(ast.Name(dict_name, ast.Load()), "update"),
@@ -915,32 +1212,39 @@
             interpreter.stack.append(ast.Name(dict_name, ast.Load()))
 
 
 class Stop(Opcode):
     name = "STOP"
 
     def run(self, interpreter: Interpreter):
-        interpreter.new_variable(interpreter.stack.pop(), name="result")
+        interpreter.new_variable(interpreter.stack.pop(), name=interpreter.result_variable)
         interpreter.stop()
 
 
 class Frame(NoOp):
     name = "FRAME"
 
 
-class BinInt(ConstantOpcode):
-    name = "BININT"
-
-
-class BinInt1(BinInt):
+class BinInt1(ConstantInt):
     name = "BININT1"
+    priority = 100
+    num_bytes = 1
 
 
 class BinInt2(BinInt1):
     name = "BININT2"
+    priority = BinInt1.priority + 1
+    num_bytes = 2
+
+
+class BinInt(ConstantInt):
+    name = "BININT"
+    priority = BinInt2.priority + 1
+    num_bytes = 4
+    signed = True
 
 
 class EmptySet(Opcode):
     name = "EMPTY_SET"
 
     def run(self, interpreter: Interpreter):
         interpreter.stack.append(ast.Set([]))
@@ -972,54 +1276,95 @@
 
     def run(self, interpreter: Interpreter):
         value = interpreter.stack.pop()
         list_obj = interpreter.stack[-1]
         if isinstance(list_obj, ast.List):
             list_obj.elts.append(value)
         else:
-            raise ValueError(
-                f"Expected a list on the stack, but instead found {list_obj!r}"
-            )
+            raise ValueError(f"Expected a list on the stack, but instead found {list_obj!r}")
 
 
 class Appends(StackSliceOpcode):
     name = "APPENDS"
 
     def run(self, interpreter: Interpreter, stack_slice: List[ast.expr]):
         list_obj = interpreter.stack[-1]
         if isinstance(list_obj, ast.List):
             list_obj.elts.extend(stack_slice)
         else:
-            raise ValueError(
-                f"Expected a list on the stack, but instead found {list_obj!r}"
-            )
+            raise ValueError(f"Expected a list on the stack, but instead found {list_obj!r}")
 
 
 class BinFloat(ConstantOpcode):
     name = "BINFLOAT"
+    priority = BinInt1.priority * 2
+
+    @classmethod
+    def validate(cls, obj):
+        if not isinstance(obj, float):
+            raise ValueError(f"{cls.__name__} expects a float, but received {obj!r}")
+        return obj
 
 
-class BinBytes(ConstantOpcode):
+class ShortBinBytes(DynamicLength, ConstantOpcode):
+    name = "SHORT_BINBYTES"
+    priority = Unicode.priority + 1
+    length_bytes = 1
+
+    @classmethod
+    def validate(cls, obj):
+        if not isinstance(obj, bytes):
+            raise ValueError(
+                f"{cls.__name__} must be instantiated with an object of type bytes, not {obj!r}"
+            )
+        return super().validate(obj)
+
+
+class BinBytes(ShortBinBytes):
     name = "BINBYTES"
+    priority = ShortBinBytes.priority + 1
+    length_bytes = 4
 
 
-class ShortBinBytes(BinBytes):
-    name = "SHORT_BINBYTES"
+class BinBytes8(BinBytes):
+    name = "BINBYTES8"
+    priority = BinBytes.priority + 1
+    length_bytes = 8
+
+
+class Long1(ConstantInt):
+    name = "LONG1"
+    num_bytes = 1
+    signed = True
+    priority = BinInt.priority + 1
+
+
+class Long4(ConstantInt):
+    name = "LONG4"
+    num_bytes = 4
+    signed = True
+    priority = Long1.priority + 1
 
 
 class Int(ConstantOpcode):
     name = "INT"
+    priority = Long4.priority + 1
 
+    def encode_body(self) -> bytes:
+        return f"{int(self.arg)}\n".encode()
 
-class Long(ConstantOpcode):
-    name = "LONG"
+    @classmethod
+    def validate(cls, obj):
+        _ = int(obj)
+        return obj
 
 
-class Long1(Long):
-    name = "LONG1"
+class Long(Int):
+    name = "LONG"
+    priority = Int.priority + 1
 
 
 class Dict(Opcode):
     name = "DICT"
 
     def run(self, interpreter: Interpreter):
         i = 0
@@ -1040,7 +1385,87 @@
 
         if len(keys) != len(values):
             raise ValueError(
                 f"Number of keys ({len(keys)}) and values ({len(values)}) for DICT do not match"
             )
 
         interpreter.stack.append(ast.Dict(keys=keys, values=values))
+
+
+if sys.version_info < (3, 9):
+    # abstract collections were not subscriptable until Python 3.9
+    PickledSequence = Sequence
+else:
+    PickledSequence = Sequence[Pickled]
+
+
+class StackedPickle(PickledSequence):
+    def __init__(self, pickled: Iterable[Pickled]):
+        self.pickled: TupleType[Pickled, ...] = tuple(pickled)
+
+    def __getitem__(self, index: int) -> Pickled:
+        return self.pickled[index]
+
+    def __len__(self) -> int:
+        return len(self.pickled)
+
+    @staticmethod
+    def load(pickled: Union[ByteString, BinaryIO]) -> "StackedPickle":
+        pickled = Pickled.make_stream(pickled)
+        pickles: List[Pickled] = []
+        while True:
+            try:
+                p = Pickled.load(pickled)
+                if len(p) == 0:
+                    break
+                pickles.append(p)
+            except EmptyPickleError:
+                break
+        if not pickles:
+            raise EmptyPickleError("No pickle files detected")
+        return StackedPickle(pickles)
+
+
+class List(Opcode):
+    name = "LIST"
+
+    def run(self, interpreter: Interpreter):
+        objs = []
+        while interpreter.stack:
+            obj = interpreter.stack.pop()
+            if isinstance(obj, MarkObject):
+                break
+            objs.append(obj)
+        else:
+            raise ValueError("Exhausted the stack while searching for a MarkObject!")
+
+        interpreter.stack.append(ast.List(elts=objs[::-1], ctx=ast.Load()))
+
+
+class FrozenSet(Opcode):
+    name = "FROZENSET"
+
+    def run(self, interpreter: Interpreter):
+        objs = []
+        while interpreter.stack:
+            obj = interpreter.stack.pop()
+            if isinstance(obj, MarkObject):
+                break
+            objs.append(obj)
+        else:
+            raise ValueError("Exhausted the stack while searching for a MarkObject!")
+
+        interpreter.stack.append(ast.Constant(ast.Set(elts=objs[::-1])))
+
+
+class Dup(Opcode):
+    name = "DUP"
+
+    def run(self, interpreter: Interpreter):
+        stack_len = len(interpreter.stack)
+        if stack_len == 0:
+            raise IndexError(
+                f"Opcode {self.opcode!s} \
+                attempted to duplicate the topmost entry on the stack, but it is empty"
+            )
+        obj = interpreter.stack[stack_len - 1]
+        interpreter.stack.append(obj)
```

### Comparing `fickling-0.0.4/fickling/tracing.py` & `fickling-0.0.5/fickling/tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,18 @@
             value = unparse(pushed_value).strip()
         print(f"\tPushed {value}")
 
     def on_memoize(self, index: int, value: ast.expr):
         print(f"\tMemoized {index} -> {unparse(value).strip()}")
 
     def on_update_memo(self, index: int, old_value: ast.expr, new_value: ast.expr):
-        print(f"\tMemo index {index} changed from {unparse(old_value).strip()} to {unparse(new_value).strip()}")
+        print(
+            f"\tMemo index {index} changed from {unparse(old_value).strip()} to "
+            f"{unparse(new_value).strip()}"
+        )
 
     def on_statement(self, statement: ast.stmt):
         print(f"\t{unparse(statement).strip()}")
 
     def on_opcode(self, opcode: Opcode):
         print(opcode.name)
```

