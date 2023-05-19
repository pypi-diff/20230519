# Comparing `tmp/utilki-0.1.8.tar.gz` & `tmp/utilki-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.1.8.tar", max compression
+gzip compressed data, was "utilki-0.2.0.tar", max compression
```

## Comparing `utilki-0.1.8.tar` & `utilki-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.1.8/README.md
--rw-r--r--   0        0        0      532 2023-05-15 13:42:34.297532 utilki-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.1.8/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.1.8/utilki/cli.py
--rw-r--r--   0        0        0     4221 2023-05-15 13:41:42.781275 utilki-0.1.8/utilki/task_mixin.py
--rw-r--r--   0        0        0     1848 2023-05-15 13:43:22.702693 utilki-0.1.8/setup.py
--rw-r--r--   0        0        0     1510 2023-05-15 13:43:22.702842 utilki-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.2.0/README.md
+-rw-r--r--   0        0        0      532 2023-05-19 15:52:08.592820 utilki-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.2.0/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.2.0/utilki/cli.py
+-rw-r--r--   0        0        0     4286 2023-05-19 15:51:51.219136 utilki-0.2.0/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1848 2023-05-19 15:52:15.479213 utilki-0.2.0/setup.py
+-rw-r--r--   0        0        0     1510 2023-05-19 15:52:15.479472 utilki-0.2.0/PKG-INFO
```

### Comparing `utilki-0.1.8/README.md` & `utilki-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.1.8/pyproject.toml` & `utilki-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.1.8"
+version = "0.2.0"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 click = "^8.1.3"
```

### Comparing `utilki-0.1.8/utilki/cli.py` & `utilki-0.2.0/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.1.8/utilki/task_mixin.py` & `utilki-0.2.0/utilki/task_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 
 
 class TaskMixin:
     __dataclass_fields__: ClassVar[Dict[str, Any]]
     __fields__: ClassVar[Dict[str, Any]]
 
     @classmethod
+    def __init__(cls, **kwargs):
+        ...
+
+    @classmethod
     def create(cls):
         params: List[Tuple[str, Any]] = []
         if hasattr(cls, "__dataclass_fields__"):
             fields: Iterable[Field] = cls.__dataclass_fields__.values()
             for field in fields:
                 params.append((field.name, field.type))
         if hasattr(cls, "__fields__"):
@@ -76,15 +80,15 @@
         if list_str.endswith("]"):
             list_str = list_str[:-1]
         return tuple(map(type_, list_str.split(",")))
 
     @classmethod
     def parse(cls, name_, type_):
         value = cls.get_default(name_)
-        print(f"parsing '{name_}' with type {type_} and value {value}")
+        # print(f"parsing '{name_}' with type {type_} and value {value}")
         if isinstance(value, str):
             if type_ == List[int]:
                 return cls.parse_list(value, int)
             elif type_ == List[str]:
                 return cls.parse_list(value, str)
             elif type_ == List[float]:
                 return cls.parse_list(value, float)
```

### Comparing `utilki-0.1.8/setup.py` & `utilki-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utilki = utilki.cli:cli']}
 
 setup_kwargs = {
     'name': 'utilki',
-    'version': '0.1.8',
+    'version': '0.2.0',
     'description': 'A collection of useful utilities',
     'long_description': '# utilki\n\n[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)\n\nutils that are frequently used by me and might be useful for others\n\n## installation\n\n```bash\npip install utilki\n```\n\n## TaskMixin\n\nMixin class that adds `create()` classmethod to dataclass you define as your task params. Useful when you have a lot of container based tasks executed on remote clusters (e.g. Kubernetes, Hashicorp Nomad, etc.). It reads task params from environment variables, parses, and validates them. \n\n```python\nfrom utilki import TaskMixin\n\n@dataclass\nclass Task(TaskMixin):\n    ayy: float = 69.69\n    lmao: str = "420"\n\nos.environ["ayy"] = "42.42"\nos.environ["lmao"] = "69"\n\nt = Task.create()\nprint(f"ayy: {t.ayy}, type: {type(t.ayy)}")\n# ayy: 42.42, type: <class \'float\'>\nprint(f"lmao: {t.lmao}, type: {type(t.lmao)}")\n# lmao: 69, type: <class \'str\'>\n```\n\n## Cli\n\n### Venv\n\n```bash\n$ utilki venv 3.8.10\n$ Enter venv name: new_venv\n$ Created venv `new_venv` with Python version 3.8.10\n```',
     'author': 'Khaidar Bikmaev',
     'author_email': 'khaidar@bikmaev.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `utilki-0.1.8/PKG-INFO` & `utilki-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.1.8
+Version: 0.2.0
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

