# Comparing `tmp/ream2-2.5.2.tar.gz` & `tmp/ream2-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ream2-2.5.2.tar", max compression
+gzip compressed data, was "ream2-2.6.0.tar", max compression
```

## Comparing `ream2-2.5.2.tar` & `ream2-2.6.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1064 2022-10-28 21:58:46.047247 ream2-2.5.2/LICENSE
--rw-r--r--   0        0        0     5267 2022-11-01 19:46:31.826604 ream2-2.5.2/README.md
--rw-r--r--   0        0        0      752 2023-04-03 05:40:13.167043 ream2-2.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-28 21:58:46.047770 ream2-2.5.2/ream/__init__.py
--rw-r--r--   0        0        0    13032 2023-02-03 20:33:43.995322 ream2-2.5.2/ream/actor_graph.py
--rw-r--r--   0        0        0     2173 2023-04-03 05:40:13.167289 ream2-2.5.2/ream/actor_state.py
--rw-r--r--   0        0        0     2040 2023-04-03 05:40:13.167458 ream2-2.5.2/ream/actor_version.py
--rw-r--r--   0        0        0        0 2022-10-28 21:58:46.048025 ream2-2.5.2/ream/actors/__init__.py
--rw-r--r--   0        0        0     3242 2023-04-03 05:40:13.167703 ream2-2.5.2/ream/actors/base.py
--rw-r--r--   0        0        0     1685 2022-10-28 21:58:46.048171 ream2-2.5.2/ream/actors/interface.py
--rw-r--r--   0        0        0    37487 2023-04-03 05:40:13.168051 ream2-2.5.2/ream/cache_helper.py
--rw-r--r--   0        0        0     3393 2023-04-19 22:09:20.839645 ream2-2.5.2/ream/cli_helper.py
--rw-r--r--   0        0        0    34149 2023-04-03 05:40:13.168657 ream2-2.5.2/ream/data_model_helper.py
--rw-r--r--   0        0        0    12489 2023-04-03 05:40:13.168961 ream2-2.5.2/ream/dataset_helper.py
--rw-r--r--   0        0        0     8875 2023-02-03 20:33:43.997558 ream2-2.5.2/ream/fs.py
--rw-r--r--   0        0        0     6636 2023-04-19 22:09:20.839850 ream2-2.5.2/ream/helper.py
--rw-r--r--   0        0        0     3607 2023-04-19 22:09:20.840085 ream2-2.5.2/ream/params_helper.py
--rw-r--r--   0        0        0     1090 2023-04-03 05:40:13.169487 ream2-2.5.2/ream/prelude.py
--rw-r--r--   0        0        0     2169 2023-04-03 05:40:13.169660 ream2-2.5.2/ream/workspace.py
--rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 ream2-2.5.2/setup.py
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-19 00:38:31.312440 ream2-2.6.0/LICENSE
+-rw-r--r--   0        0        0     5267 2023-05-19 00:38:31.312440 ream2-2.6.0/README.md
+-rw-r--r--   0        0        0      752 2023-05-19 00:38:31.316441 ream2-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/__init__.py
+-rw-r--r--   0        0        0    13032 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actor_graph.py
+-rw-r--r--   0        0        0     2197 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actor_state.py
+-rw-r--r--   0        0        0     2040 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actor_version.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actors/__init__.py
+-rw-r--r--   0        0        0     3815 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actors/base.py
+-rw-r--r--   0        0        0     1155 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actors/dsid.py
+-rw-r--r--   0        0        0      976 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actors/enum.py
+-rw-r--r--   0        0        0      363 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actors/interface.py
+-rw-r--r--   0        0        0    37569 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/cache_helper.py
+-rw-r--r--   0        0        0     3393 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/cli_helper.py
+-rw-r--r--   0        0        0    34210 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/data_model_helper.py
+-rw-r--r--   0        0        0    14434 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/dataset_helper.py
+-rw-r--r--   0        0        0     9669 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/fs.py
+-rw-r--r--   0        0        0     6636 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/helper.py
+-rw-r--r--   0        0        0     5684 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/params_helper.py
+-rw-r--r--   0        0        0     1090 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/prelude.py
+-rw-r--r--   0        0        0     2248 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/workspace.py
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.6.0/PKG-INFO
```

### Comparing `ream2-2.5.2/LICENSE` & `ream2-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ream2-2.5.2/README.md` & `ream2-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ream2-2.5.2/pyproject.toml` & `ream2-2.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ream2"
-version = "2.5.2"
+version = "2.6.0"
 description = "An actor architecture for research software"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/ream"
 repository = "https://github.com/binh-vu/ream"
 packages = [
```

### Comparing `ream2-2.5.2/ream/actor_graph.py` & `ream2-2.6.0/ream/actor_graph.py`

 * *Files identical despite different names*

### Comparing `ream2-2.5.2/ream/actor_state.py` & `ream2-2.6.0/ream/actor_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         dependencies: Optional[List[ActorState]] = None,
     ) -> ActorState:
         """Compute a unique cache id"""
         if version is None:
             assert hasattr(CLS, "VERSION"), f"Class {CLS} must have a VERSION attribute"
             version = getattr(CLS, "VERSION")
 
-        assert isinstance(
+        assert version is not None and isinstance(
             version, (int, str, ActorVersion)
         ), "Version must be a string, a number, or an ActorVersion"
 
         return ActorState(
             classpath=get_classpath(CLS),
             classversion=version,
             params=args,
```

### Comparing `ream2-2.5.2/ream/actor_version.py` & `ream2-2.6.0/ream/actor_version.py`

 * *Files identical despite different names*

### Comparing `ream2-2.5.2/ream/actors/base.py` & `ream2-2.6.0/ream/actors/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 from __future__ import annotations
 from dataclasses import is_dataclass
-import functools
 import os
-from pathlib import Path
 from typing import (
     Optional,
     List,
     Type,
     TypeVar,
     Generic,
 )
 from ream.actor_state import ActorState
 from ream.helper import resolve_type_arguments
 from ream.params_helper import EnumParams
 from ream.fs import FS
 from ream.workspace import ReamWorkspace
 from loguru import logger
-from ream.actors.interface import Actor, E
+from ream.actors.interface import Actor
 
 P = TypeVar("P")
 
 
-class BaseActor(Generic[E, P], Actor[E]):
+class BaseActor(Actor, Generic[P]):
+    """A based for parameterized actor that its output is always determisitic given: the input, actor's state, and actor's provenance.
+
+    The actor's provenance is an optional mechanism to provide additional guarantee to always have deterministic output if
+    the combination of input and actor's state is not sufficient. For example, training a model with a random seed and the store the model
+    for later use, the provenance can be the path to the model. Normally, we advise to avoid using provenance if possible.
+
+    The actor state is determined based on: its parameters and the dependant actors' states.
+    """
+
     def __init__(
         self,
         params: P,
         dep_actors: Optional[List[BaseActor]] = None,
     ):
         self._working_fs: Optional[FS] = None
         self.dep_actors: List[BaseActor] = dep_actors or []
@@ -77,17 +84,17 @@
             self._working_fs = FS(cache_dir)
         return self._working_fs
 
     @classmethod
     def get_param_cls(cls) -> Type[P]:
         """Get the parameter class of this actor"""
         args = resolve_type_arguments(BaseActor, cls)
-        assert len(args) == 2
-        assert is_dataclass(args[1])
-        return args[1]  # type: ignore
+        assert len(args) == 1
+        assert is_dataclass(args[0])
+        return args[0]  # type: ignore
 
     def get_verbose_level(self) -> int:
         """Get the verbose level of this actor from the environment variable"""
         return int(os.environ.get(self.__class__.__name__.upper() + "_VERBOSE", "0"))
 
     def _fmt_prov(self, *prov: str) -> str:
         """Format the provenances"""
```

### Comparing `ream2-2.5.2/ream/cache_helper.py` & `ream2-2.6.0/ream/cache_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -436,24 +436,25 @@
                 )
 
                 if not cache_file.exists():
                     output = func(self, *args, **kwargs)
                     with fs.acquire_write_lock(), cache_file.reserve_and_track() as fpath:
                         if log_serde_time:
                             with Timer().watch_and_report(
-                                f"serialize file {cache_file.relpath}",
+                                f"serialize file {cache_file._realdiskpath}",
                                 self.logger.debug,
                             ):
                                 ser(output, fpath)
                         else:
                             ser(output, fpath)
                 else:
                     if log_serde_time:
                         with Timer().watch_and_report(
-                            f"deserialize file {cache_file.relpath}", self.logger.debug
+                            f"deserialize file {cache_file._realdiskpath}",
+                            self.logger.debug,
                         ):
                             output = deser(cache_file.get())
                     else:
                         output = deser(cache_file.get())
                 return output
 
             if mem_persist is not None:
@@ -554,24 +555,25 @@
                 )
 
                 if not cache_file.exists():
                     output = func(self, *args, **kwargs)
                     with fs.acquire_write_lock(), cache_file.reserve_and_track() as fpath:
                         if log_serde_time:
                             with Timer().watch_and_report(
-                                f"serialize file {cache_file.relpath}",
+                                f"serialize file {cache_file._realdiskpath}",
                                 self.logger.debug,
                             ):
                                 ser(output, fpath, compression)
                         else:
                             ser(output, fpath, compression)
                 else:
                     if log_serde_time:
                         with Timer().watch_and_report(
-                            f"deserialize file {cache_file.relpath}", self.logger.debug
+                            f"deserialize file {cache_file._realdiskpath}",
+                            self.logger.debug,
                         ):
                             output = deser(cache_file.get(), compression)
                     else:
                         output = deser(cache_file.get(), compression)
                 return output
 
             if mem_persist is not None:
```

### Comparing `ream2-2.5.2/ream/cli_helper.py` & `ream2-2.6.0/ream/cli_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.5.2/ream/data_model_helper.py` & `ream2-2.6.0/ream/data_model_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import os
 
 import pickle
 import struct
 from dataclasses import dataclass, fields, is_dataclass
 from pathlib import Path, PosixPath, WindowsPath
 from typing import (
-    IO,
-    Annotated,
     BinaryIO,
     Callable,
     Generic,
     List,
     Literal,
     Optional,
     Sequence,
@@ -22,15 +20,15 @@
     Union,
     get_origin,
     get_type_hints,
 )
 from typing_extensions import Self
 from copy import deepcopy
 from nptyping import NDArray, Shape
-from nptyping.typing_ import Float64
+from nptyping.typing_ import Float64, Number
 import numpy as np
 import orjson
 import pyarrow as pa
 import pyarrow.parquet as pq
 from nptyping.ndarray import NDArrayMeta  # type: ignore
 from nptyping.shape_expression import get_dimensions  # type: ignore
 from ream.helper import has_dict_with_nonstr_keys
@@ -182,15 +180,18 @@
         metadata: NumpyDataModelMetadata = self._metadata  # type: ignore
         return len(getattr(self, metadata.array_props[0]))
 
     def shallow_clone(self) -> Self:
         return self.__class__(*(getattr(self, name) for name in self.__slots__))
 
     def replace(self, field: str, value: np.ndarray):
-        assert getattr(self, field).shape == value.shape
+        assert getattr(self, field).shape == value.shape, (
+            getattr(self, field).shape,
+            value.shape,
+        )
         newobj = self.shallow_clone()
         setattr(newobj, field, value)
         return newobj
 
     @classmethod
     def concatenate(
         cls,
@@ -876,17 +877,17 @@
 
         return index
 
 
 class SingleNumpyArray(NumpyDataModel):
     __slots__ = ["value"]
 
-    value: NDArray[Shape["*"], Float64]
+    value: NDArray[Shape["*"], Number]
 
-    def __init__(self, value: NDArray[Shape["*"], Float64]):
+    def __init__(self, value: NDArray[Shape["*"], Number]):
         self.value = value
 
 
 SingleNumpyArray.init()
 
 # dir = VirtualDir("/tmp", filetrack=FileTrack())
 # print(dir.name2file, dir.filetrack)
```

### Comparing `ream2-2.5.2/ream/dataset_helper.py` & `ream2-2.6.0/ream/dataset_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,34 +10,34 @@
     Tuple,
     List,
     Callable,
     TypeVar,
 )
 from loguru import logger
 from dataclasses import dataclass
-from ream.actors.interface import E
 from pathlib import Path
 from serde.helper import AVAILABLE_COMPRESSIONS, get_filepath
 import serde.pickle
 import serde.json
 
 RawSlice = TypedDict(
     "Slice", value=float, is_percentage=bool, absolute_value=Optional[int]
 )
+E = TypeVar("E")
 E2 = TypeVar("E2")
 
 
-class DatasetDict(dict[str, E]):
+class DatasetDict(Dict[str, E]):
     serde: tuple[Callable, Callable, Optional[str]] = (
         serde.pickle.ser,
         serde.pickle.deser,
         "pkl",
     )
 
-    def __init__(self, name: str, subsets: Dict[str, E], provenance: str = ""):
+    def __init__(self, name: str, subsets: dict[str, E], provenance: str = ""):
         super().__init__(subsets)
         self.name = name
         self.provenance = provenance
 
     def into_single_value(self) -> E:
         assert len(self) == 1
         return list(self.values())[0]
@@ -100,14 +100,67 @@
             else:
                 filepath = dir / (subset if subset != "" else "_empty")
                 ds[subset] = cls.serde[1](filepath, compression)
 
         return ds
 
 
+class DatasetList(List[E]):
+    serde: tuple[Callable, Callable, Optional[str]] = (
+        serde.pickle.ser,
+        serde.pickle.deser,
+        "pkl",
+    )
+
+    def __init__(self, name: str, items: list[E], provenance: str = ""):
+        super().__init__(items)
+        self.name = name
+        self.provenance = provenance
+
+    def map(self, fn: Callable[[E], E2]) -> DatasetList[E2]:
+        """Transform dataset from DatasetList[E] to DatasetList[E2]"""
+        return DatasetList(self.name, [fn(item) for item in self], self.provenance)
+
+    def save(self, dir: Path, compression: Optional[AVAILABLE_COMPRESSIONS] = None):
+        (dir / "metadata.json").write_bytes(
+            orjson.dumps(
+                {
+                    "name": self.name,
+                    "provenance": self.provenance,
+                }
+            )
+        )
+
+        fileext = self.serde[2]
+        if fileext is not None:
+            filename = f"data.{fileext}"
+            filepath = get_filepath(dir / filename, compression)
+            self.serde[0](list(self), filepath)
+        else:
+            filename = "data"
+            self.serde[0](list(self), dir / "data", compression)
+
+    @classmethod
+    def load(cls, dir: Path, compression: Optional[AVAILABLE_COMPRESSIONS] = None):
+        metadata = serde.json.deser(dir / "metadata.json")
+        name = metadata["name"]
+        provenance = metadata["provenance"]
+
+        fileext = cls.serde[2]
+        if fileext is not None:
+            filename = f"data.{fileext}"
+            filepath = get_filepath(dir / filename, compression)
+            lst = cls.serde[1](filepath)
+        else:
+            filepath = dir / "data"
+            lst = cls.serde[1](filepath, compression)
+
+        return cls(name, lst, provenance)
+
+
 @dataclass
 class AbsoluteRangeSelection:
     start: int
     end: int
 
     def __len__(self):
         return self.end - self.start
@@ -143,30 +196,30 @@
         raise Exception(
             "PercentageRangeSelection does not support select. Convert it to AbsoluteRangeSelection first using to_absolute"
         )
 
 
 @dataclass
 class IndexSelection:
-    index: List[int]
+    index: list[int]
 
     def __len__(self):
         return len(self.index)
 
     def __str__(self):
         return "[" + ",".join([str(i) for i in self.index]) + "]"
 
     def select(self, array: list[E]) -> list[E]:
         return [array[i] for i in self.index]
 
 
 @dataclass
 class DatasetQuery:
     dataset: str
-    subsets: Dict[
+    subsets: dict[
         str, AbsoluteRangeSelection | PercentageRangeSelection | IndexSelection
     ]
     shuffle: bool  # the shuffle is done before splitting
     seed: Optional[int]
 
     @staticmethod
     @functools.lru_cache(maxsize=1024)
@@ -244,20 +297,20 @@
                     else:
                         m = re.match(r"^(?P<sname>[a-zA-Z]+)$", subset)
                         assert (
                             m is not None
                         ), f"Invalid subset spec: `{subset}` in `{splitquery}` in `{query}`"
                         subsets[m.group("sname")] = PercentageRangeSelection(0, 100)
         else:
-            subsets: Dict[
+            subsets: dict[
                 str, AbsoluteRangeSelection | PercentageRangeSelection | IndexSelection
             ] = {"": PercentageRangeSelection(0, 100)}
         return DatasetQuery(dataset, subsets, shuffle, seed)
 
-    def select(self, array: List[E]) -> DatasetDict[List[E]]:
+    def select(self, array: list[E]) -> DatasetDict[list[E]]:
         n_exs = len(array)
 
         # gate check for percentage range selection that select all data
         subsets = {
             subset: selection.to_absolute(n_exs)
             if isinstance(selection, PercentageRangeSelection)
             else selection
@@ -303,14 +356,18 @@
             }
 
         return DatasetDict(
             self.dataset,
             output_subsets,
         )
 
+    def select_list(self, array: list[E]) -> DatasetList[E]:
+        assert len(self.subsets) == 1 and "" in self.subsets
+        return DatasetList(self.dataset, self.select(array)[""])
+
     def strip(self) -> DatasetQuery:
         """Remove the subset name from the query. Error when there are multiple subsets."""
         if len(self.subsets) > 1:
             raise ValueError(
                 f"Cannot strip subsets from query when there are multiple subsets: {self.subsets}"
             )
         return DatasetQuery(
@@ -326,15 +383,15 @@
             self.dataset, {subset: self.subsets[subset]}, self.shuffle, self.seed
         )
 
     def iter_subset(self) -> Iterator[Tuple[str, DatasetQuery]]:
         """Iterate over the subsets in the query."""
         return ((subset, self.subset(subset)) for subset in self.subsets)
 
-    def get_query(self, subsets: Optional[str | List[str]] = None) -> str:
+    def get_query(self, subsets: Optional[str | list[str]] = None) -> str:
         """Generate a query string for retrieving the subsets of the dataset."""
         if subsets is None:
             subsets = list(self.subsets.keys())
         elif isinstance(subsets, str):
             subsets = [subsets]
         else:
             assert all(subset in self.subsets for subset in subsets)
@@ -343,9 +400,9 @@
             [f"{subset}{str(self.subsets[subset])}" for subset in subsets]
         )
         if len(subsets) > 1 or "" not in subsets:
             filter = f":{filter}"
 
         return f"{self.dataset}{filter}{':shuffle' if self.shuffle else ''}{f':{self.seed}' if self.seed is not None else ''}"
 
-    def get_subset_disk_names(self) -> Dict[str, str]:
+    def get_subset_disk_names(self) -> dict[str, str]:
         return {name: "_empty" if name == "" else name for name in self.subsets.keys()}
```

### Comparing `ream2-2.5.2/ream/fs.py` & `ream2-2.6.0/ream/fs.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     def get(
         self,
         relpath: str,
         key: Optional[Union[dict, str, bytes]] = None,
         diskpath: Optional[str] = None,
         save_key: bool = False,
         subdir: bool = False,
+        subdir_incr: bool = False,
     ) -> FSPath:
         """Get a path associated with a virtual relpath with key.
 
         If the relpath is a directory (has extensions) and is already exists but with different key, it will create a new directory
         with the unique number suffix when `subdir` is False, otherwise, it will create a subdirectory
         named by the unique number.
         """
@@ -76,14 +77,15 @@
 
         return FSPath(
             relpath,
             diskpath=diskpath,
             ser_key=ser_key,
             save_key=save_key,
             subdir=subdir,
+            subdir_incr=subdir_incr,
             fs=self,
         )
 
     @contextmanager
     def acquire_write_lock(self):
         """Acquire a write lock on the current directory. You should use this before
         any attempt to write to the cache directory to prevent multiple processes
@@ -112,15 +114,16 @@
 
 @dataclass
 class FSPath:
     relpath: str
     diskpath: str
     ser_key: bytes
     save_key: bool
-    subdir: bool
+    subdir: bool  # whether to create a subdirectory for different keys
+    subdir_incr: bool  # whether to name the subdirectory with an incremental number or to use the last row number
     fs: FS
     _id: Optional[int] = None
     _status: Optional[ItemStatus] = None
     _realdiskpath: str = ""
 
     def status(self) -> ItemStatus:
         """"""
@@ -198,15 +201,27 @@
                 ]
                 if last_id is None:
                     last_id = 0
 
                 pdiskpath = Path(self.diskpath)
                 ext = "".join(pdiskpath.suffixes)
                 if self.subdir and ext == "":
-                    self._realdiskpath = str(pdiskpath / f"{last_id + 1:03d}")
+                    if self.subdir_incr:
+                        dirs = [
+                            int(d.name)
+                            for d in pdiskpath.iterdir()
+                            if d.is_dir() and d.name.isdigit()
+                        ]
+                        if len(dirs) == 0:
+                            subdirname = f"{0:03d}"
+                        else:
+                            subdirname = f"{max(dirs) + 1:03d}"
+                        self._realdiskpath = str(pdiskpath / subdirname)
+                    else:
+                        self._realdiskpath = str(pdiskpath / f"{last_id + 1:03d}")
                 else:
                     self._realdiskpath = str(
                         pdiskpath.parent
                         / (
                             pdiskpath.name[: len(pdiskpath.name) - len(ext)]
                             + f"_{last_id + 1:03d}"
                             + ext
```

### Comparing `ream2-2.5.2/ream/helper.py` & `ream2-2.6.0/ream/helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.5.2/ream/prelude.py` & `ream2-2.6.0/ream/prelude.py`

 * *Files identical despite different names*

### Comparing `ream2-2.5.2/ream/workspace.py` & `ream2-2.6.0/ream/workspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,20 @@
 
     def reserve_working_dir(self, state: ActorState) -> Path:
         classversion = slugify(str(state.classversion)).replace("-", "_")
         relpath = os.path.join(state.classpath, classversion)
         key = state.to_dict()
         diskpath = f"{state.get_classname()}/v{classversion}"
         path = self.fs.get(
-            relpath=relpath, key=key, diskpath=diskpath, save_key=True, subdir=True
+            relpath=relpath,
+            key=key,
+            diskpath=diskpath,
+            save_key=True,
+            subdir=True,
+            subdir_incr=True,
         )
 
         if path.exists():
             return self.ensure_consistent_version(state.classversion, path.get())
 
         # reserve the working directory for this actor, as we do not perform any
         # action that need to track, we need to mark it as success otherwise, the
```

### Comparing `ream2-2.5.2/setup.py` & `ream2-2.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,152 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ream2
+Version: 2.6.0
+Summary: An actor architecture for research software
+Home-page: https://github.com/binh-vu/ream
+License: MIT
+Author: Binh Vu
+Author-email: binh@toan2.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: filelock (>=3.8.0,<4.0.0)
+Requires-Dist: graph-wrapper (>=1.5.0,<2.0.0)
+Requires-Dist: hugedict (>=2.9.2,<3.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: nptyping (>=2.5.0,<3.0.0)
+Requires-Dist: orjson (>=3.8.2,<4.0.0)
+Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
+Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
+Requires-Dist: serde2 (>=1.6.0,<2.0.0)
+Requires-Dist: t2-yada (>=1.2.0,<2.0.0)
+Requires-Dist: timer4 (>=1.0.4,<2.0.0)
+Project-URL: Repository, https://github.com/binh-vu/ream
+Description-Content-Type: text/markdown
+
+# ream ![PyPI](https://img.shields.io/pypi/v/ream2) ![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
+
+A simple actor architecture for your research project. It helps addressing three problems so that you can focus on your main research:
+
+1. Configuring hyper-parameters of your method
+2. Speed-up the feedback cycles via easy & smart caching
+3. Running each step in your method independently.
+
+It's more powerful to combine with [`osin`](https://github.com/binh-vu/osin).
+
+## Introduction
+
+Let's say you are developing a method, an algorithm, or a pipeline to solve a problem. In many cases, it can be viewed as a computational graph. So why not structure your code as a computational graph, where each node is a component in your method or a step in your pipeline? It made your code more modular, and easy to release, cache, and evaluate.
+To see how we can apply this architecture, let's take a look at a record linkage project (linking entities in a table). A record linkage system typically has the following steps:
+
+1. Generate candidate entities in a table
+2. Rank the candidate entities and select the best matches.
+
+So naturally, we will have two actors for two steps: `CandidateGeneration` and `CandidateRanking`:
+
+```python
+import pandas as pd
+from typing import Literal
+from ream.prelude import BaseActor
+from dataclasses import dataclass
+
+@dataclass
+class CanGenParams:
+    # type of query that will be sent to ElasticSearch
+    query_type: Literal["exact-match", "fuzzy-match"]
+
+class CandidateGeneration(BaseActor[pd.DataFrame, CanGenParams]):
+    VERSION = 100
+
+    def run(self, table: pd.DataFrame):
+        # generate candidate entities of the given table
+        ...
+
+@dataclass
+class CanRankParams:
+    # ranking method to use
+    rank_method: Literal["pairwise", "columnwise"]
+
+class CandidateRanking(BaseActor[pd.DataFrame, CanRankParams]):
+    VERSION = 100
+
+    def __init__(self, params: CanRankParams, cangen_actor: CandidateGeneration):
+        super().__init__(params, [cangen_actor])
+
+    def run(self, table: pd.DataFrame):
+        # rank candidate entities of the given table
+        ...
+```
+
+The two actors make the code more modular and closer to releasable quality. To define the linking pipeline, we can use `ActorGraph`:
+
+```python
+from ream.prelude import ActorGraph, ActorNode, ActorEdge
+
+g = ActorGraph()
+cangen = g.add_node(ActorNode.new(CandidateGeneration))
+canrank = g.add_node(ActorNode.new(CandidateRanking))
+g.add_edge(BaseEdge(id=-1, source=cangen, target=canrank))
+```
+
+If we provide type hints for arguments of actors, as in the examples above, you can automatically construct the graph by given the actor classes.
+
+```python
+from ream.prelude import ActorGraph
+
+g = ActorGraph.auto([CandidateGeneration, CandidateRanking])
+```
+
+This seems boring and does not offer much, but then you can pick whatever actor and its function you want to call without manually initializing and parsing command line arguments. For example, we want to trigger the `evaluate` method on each actor. The parameters of the actors will be obtained automatically from the command line arguments, thanks to the [`yada`](https://github.com/binh-vu/yada) parser.
+
+```python
+if __name__ == "__main__":
+    g.run(actor_class="CandidateGeneration", actor_method="evaluate")
+```
+
+The `evaluate` method for each actor can be very useful. On the candidate generation actor, it can tell us the upper bound accuracy of our method so we know whether we need to improve the candidate generation or candidate ranking. If a dataset actor is introduced to the computational graph as demonstrated below, its evaluate method can tell us statistics about the dataset.
+
+```python
+from ream.prelude import NoParams, BaseActor, DatasetQuery
+
+class DatasetActor(BaseActor[str, NoParams]):
+    VERSION = 100
+
+    def run(self, query: str):
+        # use a query so we can dynamically select a subset of the dataset for quickly test
+        # for example: mnist[:10] -- select first 10 examples
+        dsquery = DatasetQuery.from_string(query)
+
+        # load the real dataset
+        examples = ...
+        return dsquery.select(examples)
+
+    def evaluate(self, query: str):
+        dsdict = self.run(query)
+        for split, examples in dsdict.items():
+            print(f"Dataset: {dsdict.name} - split {split} has {len(examples)} examples")
+```
+
+Let's talk about caching. Each actor when running will be uniquely identified by its name, version, and parameters (including the dependent actor parameters), and this is referred to as actor state which you can retrieve from `BaseActor.get_actor_state` function. From this, we can create a unique folder associated with that state that you can use to store your cache data (the folder can be retrieved from the function `BaseActor.get_working_fs`). Whenever the actor's dependency is updated, you will always get a new folder so no worry about managing the cache yourself! To set it up, in the file that defines the actor graph, init the ream workspace as follows:
+
+```python
+from ream.prelude import ReamWorkspace, ActorGraph
+
+ReamWorkspace.init("<folder>/<to>/<store>/<cache>")
+g = ActorGraph()
+...
+```
+
+## Installation
+
+```python
+pip install ream2  # not ream
+```
 
-packages = \
-['ream', 'ream.actors']
+## Examples
 
-package_data = \
-{'': ['*']}
+Will be added later.
 
-install_requires = \
-['filelock>=3.8.0,<4.0.0',
- 'graph-wrapper>=1.5.0,<2.0.0',
- 'hugedict>=2.9.2,<3.0.0',
- 'loguru>=0.6.0,<0.7.0',
- 'nptyping>=2.5.0,<3.0.0',
- 'orjson>=3.8.2,<4.0.0',
- 'pyarrow>=11.0.0,<12.0.0',
- 'python-slugify>=6.1.2,<7.0.0',
- 'serde2>=1.6.0,<2.0.0',
- 't2-yada>=1.2.0,<2.0.0',
- 'timer4>=1.0.4,<2.0.0']
-
-setup_kwargs = {
-    'name': 'ream2',
-    'version': '2.5.2',
-    'description': 'An actor architecture for research software',
-    'long_description': '# ream ![PyPI](https://img.shields.io/pypi/v/ream2) ![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)\n\nA simple actor architecture for your research project. It helps addressing three problems so that you can focus on your main research:\n\n1. Configuring hyper-parameters of your method\n2. Speed-up the feedback cycles via easy & smart caching\n3. Running each step in your method independently.\n\nIt\'s more powerful to combine with [`osin`](https://github.com/binh-vu/osin).\n\n## Introduction\n\nLet\'s say you are developing a method, an algorithm, or a pipeline to solve a problem. In many cases, it can be viewed as a computational graph. So why not structure your code as a computational graph, where each node is a component in your method or a step in your pipeline? It made your code more modular, and easy to release, cache, and evaluate.\nTo see how we can apply this architecture, let\'s take a look at a record linkage project (linking entities in a table). A record linkage system typically has the following steps:\n\n1. Generate candidate entities in a table\n2. Rank the candidate entities and select the best matches.\n\nSo naturally, we will have two actors for two steps: `CandidateGeneration` and `CandidateRanking`:\n\n```python\nimport pandas as pd\nfrom typing import Literal\nfrom ream.prelude import BaseActor\nfrom dataclasses import dataclass\n\n@dataclass\nclass CanGenParams:\n    # type of query that will be sent to ElasticSearch\n    query_type: Literal["exact-match", "fuzzy-match"]\n\nclass CandidateGeneration(BaseActor[pd.DataFrame, CanGenParams]):\n    VERSION = 100\n\n    def run(self, table: pd.DataFrame):\n        # generate candidate entities of the given table\n        ...\n\n@dataclass\nclass CanRankParams:\n    # ranking method to use\n    rank_method: Literal["pairwise", "columnwise"]\n\nclass CandidateRanking(BaseActor[pd.DataFrame, CanRankParams]):\n    VERSION = 100\n\n    def __init__(self, params: CanRankParams, cangen_actor: CandidateGeneration):\n        super().__init__(params, [cangen_actor])\n\n    def run(self, table: pd.DataFrame):\n        # rank candidate entities of the given table\n        ...\n```\n\nThe two actors make the code more modular and closer to releasable quality. To define the linking pipeline, we can use `ActorGraph`:\n\n```python\nfrom ream.prelude import ActorGraph, ActorNode, ActorEdge\n\ng = ActorGraph()\ncangen = g.add_node(ActorNode.new(CandidateGeneration))\ncanrank = g.add_node(ActorNode.new(CandidateRanking))\ng.add_edge(BaseEdge(id=-1, source=cangen, target=canrank))\n```\n\nIf we provide type hints for arguments of actors, as in the examples above, you can automatically construct the graph by given the actor classes.\n\n```python\nfrom ream.prelude import ActorGraph\n\ng = ActorGraph.auto([CandidateGeneration, CandidateRanking])\n```\n\nThis seems boring and does not offer much, but then you can pick whatever actor and its function you want to call without manually initializing and parsing command line arguments. For example, we want to trigger the `evaluate` method on each actor. The parameters of the actors will be obtained automatically from the command line arguments, thanks to the [`yada`](https://github.com/binh-vu/yada) parser.\n\n```python\nif __name__ == "__main__":\n    g.run(actor_class="CandidateGeneration", actor_method="evaluate")\n```\n\nThe `evaluate` method for each actor can be very useful. On the candidate generation actor, it can tell us the upper bound accuracy of our method so we know whether we need to improve the candidate generation or candidate ranking. If a dataset actor is introduced to the computational graph as demonstrated below, its evaluate method can tell us statistics about the dataset.\n\n```python\nfrom ream.prelude import NoParams, BaseActor, DatasetQuery\n\nclass DatasetActor(BaseActor[str, NoParams]):\n    VERSION = 100\n\n    def run(self, query: str):\n        # use a query so we can dynamically select a subset of the dataset for quickly test\n        # for example: mnist[:10] -- select first 10 examples\n        dsquery = DatasetQuery.from_string(query)\n\n        # load the real dataset\n        examples = ...\n        return dsquery.select(examples)\n\n    def evaluate(self, query: str):\n        dsdict = self.run(query)\n        for split, examples in dsdict.items():\n            print(f"Dataset: {dsdict.name} - split {split} has {len(examples)} examples")\n```\n\nLet\'s talk about caching. Each actor when running will be uniquely identified by its name, version, and parameters (including the dependent actor parameters), and this is referred to as actor state which you can retrieve from `BaseActor.get_actor_state` function. From this, we can create a unique folder associated with that state that you can use to store your cache data (the folder can be retrieved from the function `BaseActor.get_working_fs`). Whenever the actor\'s dependency is updated, you will always get a new folder so no worry about managing the cache yourself! To set it up, in the file that defines the actor graph, init the ream workspace as follows:\n\n```python\nfrom ream.prelude import ReamWorkspace, ActorGraph\n\nReamWorkspace.init("<folder>/<to>/<store>/<cache>")\ng = ActorGraph()\n...\n```\n\n## Installation\n\n```python\npip install ream2  # not ream\n```\n\n## Examples\n\nWill be added later.\n',
-    'author': 'Binh Vu',
-    'author_email': 'binh@toan2.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/binh-vu/ream',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

