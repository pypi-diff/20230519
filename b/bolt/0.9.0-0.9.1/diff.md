# Comparing `tmp/bolt-0.9.0.tar.gz` & `tmp/bolt-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolt-0.9.0.tar", max compression
+gzip compressed data, was "bolt-0.9.1.tar", max compression
```

## Comparing `bolt-0.9.0.tar` & `bolt-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2022-06-24 17:20:51.764021 bolt-0.9.0/LICENSE
--rw-r--r--   0        0        0     2255 2022-06-24 17:20:51.764021 bolt-0.9.0/README.md
--rw-r--r--   0        0        0      180 2022-06-24 17:21:54.152411 bolt-0.9.0/bolt/__init__.py
--rw-r--r--   0        0        0     5704 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/ast.py
--rw-r--r--   0        0        0    32290 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/codegen.py
--rw-r--r--   0        0        0        0 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/contrib/__init__.py
--rw-r--r--   0        0        0      847 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/contrib/debug_codegen.py
--rw-r--r--   0        0        0     2067 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/contrib/lazy.py
--rw-r--r--   0        0        0     5507 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/contrib/sandbox.py
--rw-r--r--   0        0        0     7125 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/helpers.py
--rw-r--r--   0        0        0     2186 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/loop_info.py
--rw-r--r--   0        0        0    55040 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/parse.py
--rw-r--r--   0        0        0      149 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/plugin.py
--rw-r--r--   0        0        0        0 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/py.typed
--rw-r--r--   0        0        0        0 2022-06-24 17:20:51.764021 bolt-0.9.0/bolt/resources/__init__.py
--rw-r--r--   0        0        0     6103 2022-06-24 17:20:51.768022 bolt-0.9.0/bolt/resources/commands.json
--rw-r--r--   0        0        0    13975 2022-06-24 17:20:51.768022 bolt-0.9.0/bolt/runtime.py
--rw-r--r--   0        0        0     1673 2022-06-24 17:20:51.768022 bolt-0.9.0/bolt/utils.py
--rw-r--r--   0        0        0     1270 2022-06-24 17:21:54.172412 bolt-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3022 2022-06-24 17:21:56.955466 bolt-0.9.0/setup.py
--rw-r--r--   0        0        0     3041 2022-06-24 17:21:56.956411 bolt-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-02 16:09:25.441057 bolt-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2255 2022-07-02 16:09:25.441057 bolt-0.9.1/README.md
+-rw-r--r--   0        0        0      180 2022-07-02 16:09:53.553239 bolt-0.9.1/bolt/__init__.py
+-rw-r--r--   0        0        0     5704 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/ast.py
+-rw-r--r--   0        0        0    32290 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/codegen.py
+-rw-r--r--   0        0        0        0 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/contrib/__init__.py
+-rw-r--r--   0        0        0      847 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/contrib/debug_codegen.py
+-rw-r--r--   0        0        0     2067 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/contrib/lazy.py
+-rw-r--r--   0        0        0     5507 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/contrib/sandbox.py
+-rw-r--r--   0        0        0     7445 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/helpers.py
+-rw-r--r--   0        0        0     2186 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/loop_info.py
+-rw-r--r--   0        0        0    55040 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/parse.py
+-rw-r--r--   0        0        0      149 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/plugin.py
+-rw-r--r--   0        0        0        0 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/py.typed
+-rw-r--r--   0        0        0        0 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/resources/__init__.py
+-rw-r--r--   0        0        0     6103 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/resources/commands.json
+-rw-r--r--   0        0        0    13975 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/runtime.py
+-rw-r--r--   0        0        0     1673 2022-07-02 16:09:25.441057 bolt-0.9.1/bolt/utils.py
+-rw-r--r--   0        0        0     1270 2022-07-02 16:09:53.577239 bolt-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3022 2022-07-02 16:09:56.637488 bolt-0.9.1/setup.py
+-rw-r--r--   0        0        0     3041 2022-07-02 16:09:56.638573 bolt-0.9.1/PKG-INFO
```

### Comparing `bolt-0.9.0/LICENSE` & `bolt-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/README.md` & `bolt-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/bolt/ast.py` & `bolt-0.9.1/bolt/ast.py`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/bolt/codegen.py` & `bolt-0.9.1/bolt/codegen.py`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/bolt/contrib/debug_codegen.py` & `bolt-0.9.1/bolt/contrib/debug_codegen.py`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/bolt/contrib/lazy.py` & `bolt-0.9.1/bolt/contrib/lazy.py`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/bolt/contrib/sandbox.py` & `bolt-0.9.1/bolt/contrib/sandbox.py`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/bolt/helpers.py` & `bolt-0.9.1/bolt/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -182,54 +182,62 @@
 
 def converter(f: Callable[[Any], AstNode]) -> Callable[[Any, AstNode], AstNode]:
     internal(f)
 
     @internal
     @wraps(f)
     def wrapper(obj: Any, node: AstNode) -> AstNode:
+        if isinstance(obj, AstNode):
+            return set_location(obj, node)
         return set_location(f(obj), node)
 
     return wrapper
 
 
 @dataclass
 class JsonObjectConverter:
     """Converter for json objects."""
 
     json_converter: Callable[[Any, AstNode], AstNode]
 
     @internal
     def __call__(self, obj: Any, node: AstNode) -> AstNode:
+        if isinstance(obj, AstNode):
+            return set_location(obj, node)
         if isinstance(node := self.json_converter(obj, node), AstJsonObject):
             return node
         raise ValueError(f"Invalid json object of type {type(obj)!r}.")
 
 
 @dataclass
 class NbtCompoundConverter:
     """Converter for nbt compounds."""
 
     nbt_converter: Callable[[Any, AstNode], AstNode]
 
     @internal
     def __call__(self, obj: Any, node: AstNode) -> AstNode:
+        if isinstance(obj, AstNode):
+            return set_location(obj, node)
         if isinstance(node := self.nbt_converter(obj, node), AstNbtCompound):
             return node
         raise ValueError(f"Invalid nbt compound of type {type(obj)!r}.")
 
 
 @dataclass
 class EntityConverter:
     """Converter for entities."""
 
     uuid_converter: Callable[[Any, AstNode], AstNode]
     player_name_converter: Callable[[Any, AstNode], AstNode]
 
     @internal
     def __call__(self, obj: Any, node: AstNode) -> AstNode:
+        if isinstance(obj, AstNode):
+            return set_location(obj, node)
         if isinstance(obj, str):
             if obj.count("-") == 4:
                 return self.uuid_converter(obj, node)
             return self.player_name_converter(obj, node)
         if isinstance(obj, UUID):
             return self.uuid_converter(obj, node)
         raise ValueError(f"Invalid entity value of type {type(obj)!r}.")
```

### Comparing `bolt-0.9.0/bolt/loop_info.py` & `bolt-0.9.1/bolt/loop_info.py`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/bolt/parse.py` & `bolt-0.9.1/bolt/parse.py`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/bolt/resources/commands.json` & `bolt-0.9.1/bolt/resources/commands.json`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/bolt/runtime.py` & `bolt-0.9.1/bolt/runtime.py`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/bolt/utils.py` & `bolt-0.9.1/bolt/utils.py`

 * *Files identical despite different names*

### Comparing `bolt-0.9.0/pyproject.toml` & `bolt-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bolt"
-version = "0.9.0"
+version = "0.9.1"
 description = "Supercharge Minecraft commands with Python"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/mcbeet/bolt"
 repository = "https://github.com/mcbeet/bolt"
 documentation = "https://github.com/mcbeet/bolt"
```

### Comparing `bolt-0.9.0/setup.py` & `bolt-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['beet>=0.68.2', 'mecha>=0.54.3']
 
 setup_kwargs = {
     'name': 'bolt',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Supercharge Minecraft commands with Python',
     'long_description': '# Bolt\n\n[![GitHub Actions](https://github.com/mcbeet/bolt/workflows/CI/badge.svg)](https://github.com/mcbeet/bolt/actions)\n[![PyPI](https://img.shields.io/pypi/v/bolt.svg)](https://pypi.org/project/bolt/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bolt.svg)](https://pypi.org/project/bolt/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![Discord](https://img.shields.io/discord/900530660677156924?color=7289DA&label=discord&logo=discord&logoColor=fff)](https://discord.gg/98MdSGMm8j)\n\n> Supercharge Minecraft commands with Python.\n\n```python\ninfinite_invisibility = {\n    Id: 14,\n    Duration: 999999,\n    Amplifier: 1,\n    ShowParticles: false,\n}\n\ndef summon_chicken_army(n):\n    for i in range(n):\n        summon chicken ~i ~ ~ {\n            Tags: [f"quack{i}"],\n            IsChickenJockey: true,\n            Passengers: [{\n                id: zombie,\n                IsBaby: true,\n                ActiveEffects: [infinite_invisibility]\n            }]\n        }\n\nsay Go forth, my minions!\nsummon_chicken_army(16)\n```\n\n## Installation\n\nThe package can be installed with `pip`.\n\n```bash\n$ pip install bolt\n```\n\n## Contributing\n\nContributions are welcome. Make sure to first open an issue discussing the problem or the new feature before creating a pull request. The project uses [`poetry`](https://python-poetry.org/).\n\n```bash\n$ poetry install\n```\n\nYou can run the tests with `poetry run pytest`.\n\n```bash\n$ poetry run pytest\n```\n\nThe project must type-check with [`pyright`](https://github.com/microsoft/pyright). If you\'re using VSCode the [`pylance`](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension should report diagnostics automatically. You can also install the type-checker locally with `npm install` and run it from the command-line.\n\n```bash\n$ npm run watch\n$ npm run check\n```\n\nThe code follows the [`black`](https://github.com/psf/black) code style. Import statements are sorted with [`isort`](https://pycqa.github.io/isort/).\n\n```bash\n$ poetry run isort bolt tests\n$ poetry run black bolt tests\n$ poetry run black --check bolt tests\n```\n\n---\n\nLicense - [MIT](https://github.com/mcbeet/bolt/blob/main/LICENSE)\n',
     'author': 'Valentin Berlier',
     'author_email': 'berlier.v@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mcbeet/bolt',
```

### Comparing `bolt-0.9.0/PKG-INFO` & `bolt-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Supercharge Minecraft commands with Python
 Home-page: https://github.com/mcbeet/bolt
 License: MIT
 Keywords: beet,minecraft,minecraft-commands,scripting-language,mcfunction
 Author: Valentin Berlier
 Author-email: berlier.v@gmail.com
 Requires-Python: >=3.8,<4.0
```

