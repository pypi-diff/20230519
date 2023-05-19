# Comparing `tmp/fastconfig-0.1.1.tar.gz` & `tmp/fastconfig-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastconfig-0.1.1.tar", max compression
+gzip compressed data, was "fastconfig-0.2.0.tar", max compression
```

## Comparing `fastconfig-0.1.1.tar` & `fastconfig-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-05-13 08:01:32.474026 fastconfig-0.1.1/LICENSE
--rw-r--r--   0        0        0     2328 2023-05-17 13:30:36.745522 fastconfig-0.1.1/README.md
--rw-r--r--   0        0        0     3041 2023-05-15 03:49:27.742503 fastconfig-0.1.1/fastconfig/__init__.py
--rw-r--r--   0        0        0     2918 2023-05-17 13:30:36.745719 fastconfig-0.1.1/fastconfig/config.py
--rw-r--r--   0        0        0      262 2023-05-17 13:30:36.745869 fastconfig-0.1.1/fastconfig/exception.py
--rw-r--r--   0        0        0     1403 2023-05-17 13:30:36.746033 fastconfig-0.1.1/fastconfig/internals/loader.py
--rw-r--r--   0        0        0     3096 2023-05-17 13:30:36.746365 fastconfig-0.1.1/fastconfig/internals/type_checker.py
--rw-r--r--   0        0        0     2010 2023-05-17 13:30:36.746509 fastconfig-0.1.1/fastconfig/internals/validator.py
--rw-r--r--   0        0        0      734 2023-05-17 13:35:15.658758 fastconfig-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 fastconfig-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-13 08:01:32.474026 fastconfig-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2221 2023-05-19 12:16:39.579264 fastconfig-0.2.0/README.md
+-rw-r--r--   0        0        0     3165 2023-05-19 12:34:25.653939 fastconfig-0.2.0/fastconfig/__init__.py
+-rw-r--r--   0        0        0     6542 2023-05-19 06:42:52.517790 fastconfig-0.2.0/fastconfig/config.py
+-rw-r--r--   0        0        0      589 2023-05-19 06:42:52.518014 fastconfig-0.2.0/fastconfig/exception.py
+-rw-r--r--   0        0        0     1079 2023-05-19 06:42:52.518240 fastconfig-0.2.0/fastconfig/internals/loader.py
+-rw-r--r--   0        0        0     3138 2023-05-19 06:42:52.518473 fastconfig-0.2.0/fastconfig/internals/type_checker.py
+-rw-r--r--   0        0        0     1807 2023-05-19 06:42:52.518695 fastconfig-0.2.0/fastconfig/internals/validator.py
+-rw-r--r--   0        0        0      860 2023-05-19 12:34:25.654226 fastconfig-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 fastconfig-0.2.0/PKG-INFO
```

### Comparing `fastconfig-0.1.1/LICENSE` & `fastconfig-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastconfig-0.1.1/README.md` & `fastconfig-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,102 @@
+Metadata-Version: 2.1
+Name: fastconfig
+Version: 0.2.0
+Summary: A lightweight way to find the project root and load config
+Home-page: https://github.com/kyoto7250
+License: MIT
+Author: kyoto7250
+Author-email: kyoto7250@aol.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: toml (>=0.10.0,<0.11.0)
+Project-URL: Repository, https://github.com/kyoto7250/fastconfig
+Description-Content-Type: text/markdown
+
 # fastconfig
 A lightweight way to find the project root and load config in python3.
 current support is [`3.9`, `3.10`, `3.11`].
 
-
-## Abstract
-
 This library provides two functionalities:
 
-
 * A function to search for files while traversing up to the project root.
     - `fastconfig.find_project_root`
     - `fastconfig.is_project_root`
     - `fastconfig.search`
 * A function to directly build a class from a configuration file.
     - `fastconfig.config.FastConfig`
-    - `fastconfig.config.ConfigBuilder`
+      * `build`
+      * `to_dict`
 
 
 ## Install
 
 ```bash
 pip install fastconfig
 ```
 
 ## Usage
 
-### toml
-
-```toml
-setting_path = "setting_path"
-[section]
-numeric = 24
-```
-
-
+- `example.json`
 ```json
 {
     "setting_path": "setting_path",
     "section": {
         "numeric": 42
     }
 }
 ```
 
+- `other.toml`
+```toml
+setting_path = "setting_path"
+[section]
+numeric = 24
+```
+
 ```python
+# main.py
 import fastconfig
-from fastconfig.config import FastConfig, ConfigBuilder, Metadata
+from fastconfig.config import FastConfig, fc_field
 from fastconfig.exception import FastConfigError
 from dataclasses import field, dataclass
 
 
 @dataclass
 class Config(FastConfig):
-    result: int = field(
-        default=-1, metadata=Metadata({"section": ["section", "numeric"]})
-    )
+    result: int = fc_field(key="section.numeric", default=-1)
     # If metadata does not exist, it is searched by variable name
-    setting_path: str = field(default="default")
+    setting_path: str = fc_field(default="default")
     # Type checking is done based on the type of dataclass. Type checking is recursive.
-    dic: dict[str, int] = field(
-        default_factory=dict, metadata=Metadata({"section": "section"})
-    )
+    dic: dict[str, int] = fc_field(key="section", default_factory=dict)
 
 
 if path := fastconfig.search("example.json"):
     try:
         # build instance
-        config = ConfigBuilder.build(path, Config)
+        config = Config.build(path)
         assert config == Config(
             result=42, setting_path="setting_path", dic={"numeric": 42}
         )
     except FastConfigError:
         raise RuntimeError
 else:
     config = Config()
 
 if other_path := fastconfig.search("other.toml"):
     # can update config
-    config = ConfigBuilder.build(other_path, config)
+    config = Config.build(other_path, config)
     assert config == Config(result=24, setting_path="setting_path", dic={"numeric": 24})
 ```
 
 ## Motivation
 
 In many projects, it is common to write configuration files, read them in code, and build Config classes. I created this library to enable these functions to be implemented by simply defining a class and specifying a file name (such as pyproject.toml).
 
 ## Contribution
 If you have suggestions for features or improvements to the code, please feel free to create an issue first.
+
```

### Comparing `fastconfig-0.1.1/fastconfig/__init__.py` & `fastconfig-0.2.0/fastconfig/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+"""This package provides the methods to search files."""
 import os
 from pathlib import Path
 from typing import List, Optional, Union
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 PROJECT_ROOTS: List[str] = [".hg", ".git"]
 DEPTH: int = 10
 
 
 def is_project_root(path: Union[str, Path]) -> bool:
     """
     Check the given path is the project root directory or not.
+
     This method determines the project root by whether the version control tool directory exists.
 
     Args:
-        path (Union[str, Path]): The path to check whether it is the project root or not
+        path (Union[str, Path]):
+            The path to check whether it is the project root or not
 
     Returns:
         bool: The result of the project root or not
     """
     if isinstance(path, str):
         path = Path(path)
 
@@ -28,18 +31,19 @@
         if path.joinpath(candidate).is_dir():
             return True
     return False
 
 
 def find_project_root(path: Optional[Union[str, Path]] = None) -> Optional[Path]:
     """
-    Return if the project root is found, or None if not
+    Return if the project root is found, or None if not.
 
     Args:
-        path (Optional[Union[str, Path]]): A path string or Path object to start searching, If nothing is passed, start in the current directory
+        path (Optional[Union[str, Path]]):
+            A path string or Path object to start searching, If nothing is passed, start in the current directory
 
     Returns:
         Optional[Path]: the project root path, or None if the project root is not found
     """
     if path is None:
         path = os.getcwd()
     cnt: int = 0
@@ -62,20 +66,25 @@
 
 def search(
     target: Union[str, Path],
     path: Optional[Union[str, Path]] = None,
     end_up_the_project_root: bool = True,
 ) -> Optional[Path]:
     """
-    Recursively searches for files with the name of the target and returns the result
+    Recursively searches for files with the name of the target and returns the result.
 
     Args:
-        target (Union[str, Path]): Search target filename, and directory names are ignored
-        path (Optional[Union[str, Path]]): A path string or Path object to start searching, If nothing is passed, start in the current directory
-        end_up_the_project_root (bool): Whether or not to search the directory where the version control tool exists
+        target (Union[str, Path]):
+            Search target filename, and directory names are ignored.
+
+        path (Optional[Union[str, Path]]):
+            A path string or Path object to start searching, If nothing is passed, start in the current directory.
+
+        end_up_the_project_root (bool):
+            Whether or not to search the directory where the version control tool exists
 
     Returns:
         Optional[Path]: a path of the target file, or None if the target file is not found
     """
     if isinstance(target, str):
         target = Path(target)
```

### Comparing `fastconfig-0.1.1/fastconfig/internals/loader.py` & `fastconfig-0.2.0/fastconfig/internals/loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,17 @@
+"""this module provides `_FileLoader`."""
 import json
-import sys
 from typing import Any
 
-from fastconfig.exception import InvalidConfigError
+import toml
 
-if sys.version_info >= (3, 11):
-    import tomllib
-else:
-    import toml as tomllib
+from fastconfig.exception import InvalidConfigError
 
 
-class FileLoader:
+class _FileLoader:
     def __call__(self, path: str) -> dict[str, Any]:
         if path.endswith(".json"):
             return self.load_json(path)
         elif path.endswith(".toml"):
             return self.load_toml(path)
         raise InvalidConfigError("FastConfig only supports json and toml formats now")
 
@@ -25,20 +22,13 @@
             if not isinstance(config, dict):
                 config = {"content": config}
             return config
         except json.decoder.JSONDecodeError as e:
             raise InvalidConfigError(str(e))
 
     def load_toml(self, path: str) -> dict[str, Any]:
-        if sys.version_info >= (3, 11):
-            try:
-                with open(path, "rb") as f:
-                    config = tomllib.load(f)
-            except tomllib.TOMLDecodeError as e:
-                raise InvalidConfigError(str(e))
-        else:
-            try:
-                with open(path, "r") as f:
-                    config = tomllib.load(f)
-            except tomllib.decoder.TomlDecodeError as e:
-                raise InvalidConfigError(str(e))
+        try:
+            with open(path, "r") as f:
+                config = toml.load(f)
+        except toml.decoder.TomlDecodeError as e:
+            raise InvalidConfigError(str(e))
         return config
```

### Comparing `fastconfig-0.1.1/fastconfig/internals/type_checker.py` & `fastconfig-0.2.0/fastconfig/internals/type_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+"""this module provides _TypeChecker."""
 import datetime
 from types import GenericAlias
 from typing import Any, Type, Union, _SpecialForm, get_args, get_origin
 
 from fastconfig.exception import UnexpectedValueError
 
 DATE_TYPES = [datetime.datetime, datetime.date, datetime.time]
 
 
-class TypeChecker:
+class _TypeChecker:
     def __call__(
         self, key: str, value: Any, typeinfo: Union[type, GenericAlias, _SpecialForm]
     ) -> Any:
         self.value = value
         if not self.check(key, value, typeinfo):
             raise UnexpectedValueError(
                 f"{key}: {value} is not valid type. must be of type {typeinfo}"
```

### Comparing `fastconfig-0.1.1/fastconfig/internals/validator.py` & `fastconfig-0.2.0/fastconfig/internals/validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,51 @@
+"""this module provides Validator."""
 from dataclasses import MISSING, Field
-from typing import Any, Optional, Union
+from typing import Any, List, Optional, Union
 
-from fastconfig.exception import MissingRequiredElementError, UnexpectedValueError
-from fastconfig.internals.type_checker import TypeChecker
+from fastconfig.exception import MissingRequiredElementError
+from fastconfig.internals.type_checker import _TypeChecker
 
 
-def extract(setting: dict[str, Any], section: Union[str, list[str]]) -> Optional[Any]:
+def _extract(setting: dict[str, Any], section: Union[str, List[str]]) -> Optional[Any]:
     if isinstance(section, str) and section in setting:
         return setting[section]
-    elif isinstance(section, list):
+    elif isinstance(section, List):
         for element in section:
             if not (isinstance(setting, dict) and element in setting):
                 return None
             setting = setting[element]
         return setting
     return None
 
 
 class DEFAULT_VALUE:
-    """
-    This class is the dummy object for meaning `use default value`
-    """
+    """This class is the dummy object for meaning `use default value`."""
 
     pass
 
 
-class Validator:
+class _Validator:
     def __init__(self, setting: dict[str, Any]) -> None:
         self.setting: dict[str, Any] = setting
-        self.checker: TypeChecker = TypeChecker()
+        self.checker: _TypeChecker = _TypeChecker()
 
     def __call__(self, key: str, f: Field, build: bool = True) -> Any:
         metadata: dict[str, Any] = dict(f.metadata) if hasattr(f, "metadata") else {}
-        section: str = metadata["section"] if "section" in metadata else key
-        value: Any = extract(self.setting, section)
+        separator = metadata["separator"] if "separator" in metadata else "."
+        setting_key: Union[str, List[str]] = (
+            metadata["key"].split(separator) if "key" in metadata else key
+        )
+        value: Any = _extract(self.setting, setting_key)
 
         if value is None:
             if (
                 isinstance(f.default, type(MISSING))
                 and isinstance(f.default_factory, type(MISSING))
                 and build
             ):
                 # TODO: check default_factry
                 raise MissingRequiredElementError(f"key: {key} is not found")
             return DEFAULT_VALUE()
 
         value = self.checker(key, value, f.type)
-        if "choice" in metadata and value not in metadata["choice"]:
-            raise UnexpectedValueError(
-                f"{key}: {value} is not valid. must be selected in {metadata['choice']}"
-            )
-
-        if "validate" in metadata and metadata["validate"](value):
-            # TODO: think error message
-            raise UnexpectedValueError
         return value
```

### Comparing `fastconfig-0.1.1/pyproject.toml` & `fastconfig-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastconfig"
-version = "0.1.1"
+version = "0.2.0"
 description = "A lightweight way to find the project root and load config"
 authors = ["kyoto7250 <kyoto7250@aol.com>"]
 homepage = "https://github.com/kyoto7250"
 repository = "https://github.com/kyoto7250/fastconfig"
 license = "MIT"
 readme = "README.md"
 
@@ -15,14 +15,17 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 ruff = "^0.0.267"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
+pydocstyle = "^6.3.0"
+mkdocstrings-python = "^1.0.0"
+mkdocs-material = "^9.1.13"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 88
@@ -32,7 +35,10 @@
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 pythonpath = [
   "."
 ]
+
+[tool.pydocstyle]
+match= "(?!test_).*\\.py"
```

### Comparing `fastconfig-0.1.1/PKG-INFO` & `fastconfig-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,82 @@
-Metadata-Version: 2.1
-Name: fastconfig
-Version: 0.1.1
-Summary: A lightweight way to find the project root and load config
-Home-page: https://github.com/kyoto7250
-License: MIT
-Author: kyoto7250
-Author-email: kyoto7250@aol.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: toml (>=0.10.0,<0.11.0)
-Project-URL: Repository, https://github.com/kyoto7250/fastconfig
-Description-Content-Type: text/markdown
-
 # fastconfig
 A lightweight way to find the project root and load config in python3.
 current support is [`3.9`, `3.10`, `3.11`].
 
-
-## Abstract
-
 This library provides two functionalities:
 
-
 * A function to search for files while traversing up to the project root.
     - `fastconfig.find_project_root`
     - `fastconfig.is_project_root`
     - `fastconfig.search`
 * A function to directly build a class from a configuration file.
     - `fastconfig.config.FastConfig`
-    - `fastconfig.config.ConfigBuilder`
+      * `build`
+      * `to_dict`
 
 
 ## Install
 
 ```bash
 pip install fastconfig
 ```
 
 ## Usage
 
-### toml
-
-```toml
-setting_path = "setting_path"
-[section]
-numeric = 24
-```
-
-
+- `example.json`
 ```json
 {
     "setting_path": "setting_path",
     "section": {
         "numeric": 42
     }
 }
 ```
 
+- `other.toml`
+```toml
+setting_path = "setting_path"
+[section]
+numeric = 24
+```
+
 ```python
+# main.py
 import fastconfig
-from fastconfig.config import FastConfig, ConfigBuilder, Metadata
+from fastconfig.config import FastConfig, fc_field
 from fastconfig.exception import FastConfigError
 from dataclasses import field, dataclass
 
 
 @dataclass
 class Config(FastConfig):
-    result: int = field(
-        default=-1, metadata=Metadata({"section": ["section", "numeric"]})
-    )
+    result: int = fc_field(key="section.numeric", default=-1)
     # If metadata does not exist, it is searched by variable name
-    setting_path: str = field(default="default")
+    setting_path: str = fc_field(default="default")
     # Type checking is done based on the type of dataclass. Type checking is recursive.
-    dic: dict[str, int] = field(
-        default_factory=dict, metadata=Metadata({"section": "section"})
-    )
+    dic: dict[str, int] = fc_field(key="section", default_factory=dict)
 
 
 if path := fastconfig.search("example.json"):
     try:
         # build instance
-        config = ConfigBuilder.build(path, Config)
+        config = Config.build(path)
         assert config == Config(
             result=42, setting_path="setting_path", dic={"numeric": 42}
         )
     except FastConfigError:
         raise RuntimeError
 else:
     config = Config()
 
 if other_path := fastconfig.search("other.toml"):
     # can update config
-    config = ConfigBuilder.build(other_path, config)
+    config = Config.build(other_path, config)
     assert config == Config(result=24, setting_path="setting_path", dic={"numeric": 24})
 ```
 
 ## Motivation
 
 In many projects, it is common to write configuration files, read them in code, and build Config classes. I created this library to enable these functions to be implemented by simply defining a class and specifying a file name (such as pyproject.toml).
 
 ## Contribution
 If you have suggestions for features or improvements to the code, please feel free to create an issue first.
-
```

