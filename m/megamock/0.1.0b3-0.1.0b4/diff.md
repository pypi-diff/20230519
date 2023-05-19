# Comparing `tmp/megamock-0.1.0b3.tar.gz` & `tmp/megamock-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megamock-0.1.0b3.tar", max compression
+gzip compressed data, was "megamock-0.1.0b4.tar", max compression
```

## Comparing `megamock-0.1.0b3.tar` & `megamock-0.1.0b4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 08:50:11.430853 megamock-0.1.0b3/LICENSE
--rwxr-xr-x   0        0        0    10248 2023-05-10 08:50:11.431855 megamock-0.1.0b3/README.md
--rwxr-xr-x   0        0        0      282 2023-05-10 08:50:11.445853 megamock-0.1.0b3/megamock/__init__.py
--rwxr-xr-x   0        0        0     5689 2023-05-10 08:50:11.445853 megamock-0.1.0b3/megamock/import_machinery.py
--rwxr-xr-x   0        0        0     3881 2023-05-10 08:50:11.446853 megamock-0.1.0b3/megamock/import_references.py
--rwxr-xr-x   0        0        0    32748 2023-05-10 10:26:15.062755 megamock-0.1.0b3/megamock/megamocks.py
--rwxr-xr-x   0        0        0    14787 2023-05-10 08:50:11.448853 megamock-0.1.0b3/megamock/megapatches.py
--rwxr-xr-x   0        0        0     3672 2023-05-10 08:50:11.448853 megamock-0.1.0b3/megamock/megas.py
--rwxr-xr-x   0        0        0     3066 2023-05-10 08:50:11.449852 megamock-0.1.0b3/megamock/name_words.py
--rwxr-xr-x   0        0        0        0 2023-05-10 08:50:11.449852 megamock-0.1.0b3/megamock/plugins/__init__.py
--rwxr-xr-x   0        0        0      949 2023-05-10 08:50:11.450861 megamock-0.1.0b3/megamock/plugins/pytest.py
--rwxr-xr-x   0        0        0      303 2023-05-10 08:50:11.450861 megamock-0.1.0b3/megamock/type_util.py
--rwxr-xr-x   0        0        0     1199 2023-05-10 10:24:17.344905 megamock-0.1.0b3/pyproject.toml
--rw-r--r--   0        0        0    11236 1970-01-01 00:00:00.000000 megamock-0.1.0b3/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 08:50:11.430853 megamock-0.1.0b4/LICENSE
+-rwxr-xr-x   0        0        0    10248 2023-05-10 08:50:11.431855 megamock-0.1.0b4/README.md
+-rwxr-xr-x   0        0        0      282 2023-05-10 08:50:11.445853 megamock-0.1.0b4/megamock/__init__.py
+-rwxr-xr-x   0        0        0     5689 2023-05-10 08:50:11.445853 megamock-0.1.0b4/megamock/import_machinery.py
+-rwxr-xr-x   0        0        0     4341 2023-05-19 01:34:42.492745 megamock-0.1.0b4/megamock/import_references.py
+-rw-r--r--   0        0        0    32414 2023-05-14 00:51:44.177376 megamock-0.1.0b4/megamock/megamocks.py
+-rwxr-xr-x   0        0        0    14787 2023-05-10 08:50:11.448853 megamock-0.1.0b4/megamock/megapatches.py
+-rwxr-xr-x   0        0        0     3672 2023-05-10 08:50:11.448853 megamock-0.1.0b4/megamock/megas.py
+-rwxr-xr-x   0        0        0     3066 2023-05-10 08:50:11.449852 megamock-0.1.0b4/megamock/name_words.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 08:50:11.449852 megamock-0.1.0b4/megamock/plugins/__init__.py
+-rwxr-xr-x   0        0        0      949 2023-05-10 08:50:11.450861 megamock-0.1.0b4/megamock/plugins/pytest.py
+-rwxr-xr-x   0        0        0      303 2023-05-10 08:50:11.450861 megamock-0.1.0b4/megamock/type_util.py
+-rw-r--r--   0        0        0     1199 2023-05-19 01:20:24.141022 megamock-0.1.0b4/pyproject.toml
+-rw-r--r--   0        0        0    11236 1970-01-01 00:00:00.000000 megamock-0.1.0b4/PKG-INFO
```

### Comparing `megamock-0.1.0b3/LICENSE` & `megamock-0.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b3/README.md` & `megamock-0.1.0b4/README.md`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b3/megamock/import_machinery.py` & `megamock-0.1.0b4/megamock/import_machinery.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b3/megamock/import_references.py` & `megamock-0.1.0b4/megamock/import_references.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,27 @@
     @staticmethod
     def add_reference(
         module: ModuleType,
         calling_module: ModuleType,
         original_name: str,
         named_as: str,
     ) -> None:
+        # do not bother with bad modules. Example: conftest from pytest
+        if not calling_module.__package__:
+            # this can happen if using megamock + pytest hot reloader
+            return
+        References._add_reference(module, calling_module, original_name, named_as)
+
+    @staticmethod
+    def _add_reference(
+        module: ModuleType,
+        calling_module: ModuleType,
+        original_name: str,
+        named_as: str,
+    ) -> None:
         module_path = module.__name__
         References.references[calling_module.__name__][named_as] = ModAndName(
             module_path,
             original_name,
         )
         base_original_name = original_name.split(".")[0]
         References.reverse_references[module_path][base_original_name].add(
```

### Comparing `megamock-0.1.0b3/megamock/megamocks.py` & `megamock-0.1.0b4/megamock/megamocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 import re
 import time
 import traceback
 from abc import ABCMeta
 from collections import defaultdict
 from dataclasses import dataclass, field
 from inspect import isawaitable, isclass, iscoroutinefunction
-from typing import Any, Callable, Generic, Literal, TypeVar, cast, overload
+from typing import (
+    Any,
+    Callable,
+    Generic,
+    Literal,
+    TypeVar,
+    cast,
+    get_type_hints,
+    overload,
+)
 from unittest import mock
 from unittest.mock import create_autospec
 
 from megamock import name_words
 from megamock.type_util import MISSING, MISSING_TYPE
 
 T = TypeVar("T")
@@ -394,32 +403,21 @@
                     raise
         else:
             self.__dict__[key] = value
 
     def _set_attr_annotations_check(self, key: str, value: Any) -> None:
         # do not check type if assigning a mock object
         # note that MegaMock is a subclass of NonCallableMagicMock
-        if not isinstance(
-            value, mock.NonCallableMock | mock.NonCallableMagicMock
-        ):
-            allowed_values = self.megamock.spec.__annotations__[key]
+        if not isinstance(value, mock.NonCallableMock | mock.NonCallableMagicMock):
+            allowed_values = get_type_hints(self.megamock.spec)[key]
 
             def raise_type_error() -> None:
-                raise TypeError(
-                    f"{value!r} is not an instance of {allowed_values}"
-                )
+                raise TypeError(f"{value!r} is not an instance of {allowed_values}")
 
-            # handle:
-            # "from __future__ import annotations" converting type to str
-            if isinstance(allowed_values, str):
-                if str(value.__class__.__name__) not in [
-                    x.strip() for x in allowed_values.split("|")
-                ]:
-                    raise_type_error()
-            elif not isinstance(value, allowed_values):
+            if not isinstance(value, allowed_values):
                 raise_type_error()
 
     def _get_spec_from_parents(
         self, _parent_stack: list[_MegaMockMixin] | None = None
     ) -> Any:
         """
         The built-in generate autospec function creates a few issues because
```

### Comparing `megamock-0.1.0b3/megamock/megapatches.py` & `megamock-0.1.0b4/megamock/megapatches.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b3/megamock/megas.py` & `megamock-0.1.0b4/megamock/megas.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b3/megamock/name_words.py` & `megamock-0.1.0b4/megamock/name_words.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b3/megamock/plugins/pytest.py` & `megamock-0.1.0b4/megamock/plugins/pytest.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b3/pyproject.toml` & `megamock-0.1.0b4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "megamock"
-version = "0.1.0-beta.3"
+version = "0.1.0-beta.4"
 description = "Mega mocking capabilities - stop using dot-notated paths!"
 authors = ["James Hutchison <jamesghutchison@proton.me>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/JamesHutchison/megamock"
 repository = "https://github.com/JamesHutchison/megamock"
 keywords = ["mock", "test"]
```

### Comparing `megamock-0.1.0b3/PKG-INFO` & `megamock-0.1.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megamock
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: Mega mocking capabilities - stop using dot-notated paths!
 Home-page: https://github.com/JamesHutchison/megamock
 License: MIT
 Keywords: mock,test
 Author: James Hutchison
 Author-email: jamesghutchison@proton.me
 Requires-Python: >=3.10,<4.0
```

