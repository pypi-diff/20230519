# Comparing `tmp/gameyamlspiderandgenerator-1.4.4.tar.gz` & `tmp/gameyamlspiderandgenerator-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.4.4.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.5.0.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.4.4.tar` & `gameyamlspiderandgenerator-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.4.4/LICENSE
--rwxr-xr-x   0        0        0     1321 2023-05-05 11:54:39.050733 gameyamlspiderandgenerator-1.4.4/README.md
--rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1751 2023-05-05 11:54:39.052734 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      235 2023-05-15 23:17:15.527274 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     3721 2023-05-15 23:18:06.030212 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0      560 2023-05-15 23:18:51.608508 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/validate.py
--rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2722 2023-05-16 00:58:45.661904 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7203 2023-05-14 14:53:55.250700 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7700 2023-05-05 14:39:08.992543 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1472 2023-05-05 14:39:08.993151 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1944 2023-05-05 11:54:39.057708 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2611 2023-05-05 11:54:39.066258 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      700 2023-05-16 00:57:34.403809 gameyamlspiderandgenerator-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.4.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.5.0/LICENSE
+-rwxr-xr-x   0        0        0     1321 2023-05-05 11:54:39.050733 gameyamlspiderandgenerator-1.5.0/README.md
+-rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1751 2023-05-05 11:54:39.052734 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      235 2023-05-19 14:05:11.849031 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0      901 2023-05-19 15:02:18.997930 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/openai.py
+-rwxr-xr-x   0        0        0     3879 2023-05-19 14:09:35.954441 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      559 2023-05-19 14:05:11.679558 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     3163 2023-05-19 15:02:38.731415 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7203 2023-05-14 14:53:55.250700 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7700 2023-05-05 14:39:08.992543 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1472 2023-05-05 14:39:08.993151 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1944 2023-05-05 11:54:39.057708 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2611 2023-05-05 11:54:39.066258 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      264 2023-05-19 13:17:24.010025 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/thread.py
+-rwxr-xr-x   0        0        0      719 2023-05-19 15:05:19.437639 gameyamlspiderandgenerator-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.5.0/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.4.4/LICENSE` & `gameyamlspiderandgenerator-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/README.md` & `gameyamlspiderandgenerator-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 from re import sub
 from urllib.parse import quote_plus
 
-from bs4 import BeautifulSoup
 from loguru import logger
 
 from ..hook import BaseHook
 from ..util.config import config
 from ..util.spider import get_json
+from ..util.thread import ThreadWithReturnValue
 
 
 # print(config, type(config))
 
-
 class Search(BaseHook):
-    REQUIRED = "get_name"
+    CHANGED = ["tags", "links"]
+
+    def __init__(self):
+        self.pure = None
+        self.encode = None
 
     @staticmethod
     def name_filter(string: str, pattern: str = r"[^A-z]", repl: str = ""):
         """
         
         Args:
             string: The string to be replaced
             pattern: Regular expression, replace non-English letters by default
             repl: The string to replace with
 
         Returns:
 
         """
         return sub(pattern, repl, string)
-
-    def __init__(self, name: str) -> None:
-        logger.info(f"Hook: init {name}")
-        self.pure = self.name_filter(name)
-        self.encode = quote_plus(self.name_filter(name, repl=" "))
-
     def search_play(self) -> tuple:
         data = get_json(
             "https://serpapi.com/search?engine=google_play&apikey="
             f'{config["api"]["google-play"]}&store=apps&q={self.encode}'
         )
         if "organic_results" in data and any(
                 [self.name_filter(i["title"]) == self.pure for i in data["organic_results"][0]["items"]]):
@@ -58,19 +55,23 @@
         return [], []
 
     def search_all(self) -> list:
         func_list = [
             self.__getattribute__(i)
             for i in (list(filter(lambda x: "__" not in x, self.__dir__())))
         ]
-        func_list = filter(
+        func_list = list(filter(
             lambda x: callable(x) and x.__name__.startswith("search") and x.__name__ != "search_all",
             func_list,
-        )
-        return [ii() for ii in func_list]
+        ))
+
+        fn_list = [ThreadWithReturnValue(target=i) for i in func_list]
+        for i in fn_list:
+            i.start()
+        return [ii.join() for ii in fn_list]
 
     def search_epic(self):
         from epicstore_api import EpicGamesStoreAPI
 
         api = EpicGamesStoreAPI().fetch_store_games(keywords="TUNIC", sort_dir="DESC")
         game_list = api['data']['Catalog']['searchStore']['elements']
         reg = r"[^A-z\d]"
@@ -87,14 +88,16 @@
         Args:
             data: yaml daya
 
         Returns:
             The processed dict data
 
         """
+        self.pure = self.name_filter(data['name'])
+        self.encode = quote_plus(self.name_filter(data['name'], repl=" "))
         temp = data.copy()
         try:
             result = self.search_all()
             publish = [i[0] for i in result] + temp["tags"]['publish']
             link = [i[1] for i in result] + temp["links"]
 
             def rm_empty(s: list):
```

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/validate.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ..util.spider import get_text
 from jsonschema import validate
 from yaml import safe_load
 from loguru import logger
 
 
 class Verify(BaseHook):
-    REQUIRED = None
+    CHANGED = None
 
     def setup(self, data: dict):
         try:
             validate(data, safe_load(get_text('https://raw.githubusercontent.com/FurryGamesIndex/games/master/schemas'
                                               '/game.schema.yaml')))
             logger.success("verification complete")
         except Exception as e:
```

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import abc
 import re
+import time
 from typing import List
 
+from loguru import logger
+
+from ..util.thread import ThreadWithReturnValue
+
 
 class BasePlugin(abc.ABC):
     """插件基类"""
 
     _VERIFY_PATTERN: re.Pattern
 
     @classmethod
@@ -26,19 +31,30 @@
         加载钩子
 
         Args:
             data: 钩子数据
         """
         from gameyamlspiderandgenerator.util.plugin_manager import pkg
         pkg.__init__()
-        for i in pkg.hook.values():
-            if i.REQUIRED is None:
-                data = i().setup(data)
-            else:
-                data = i(self.__getattribute__(i.REQUIRED)()).setup(data)
+
+        def get_fn_address():
+            fn: list = []
+            for i in pkg.hook.values():
+                    fn.append([i().setup, i.CHANGED])
+            return fn
+
+        fn = get_fn_address()
+        fn_list = [(ThreadWithReturnValue(target=i, args=(data,)), _) for i, _ in fn]
+        for i, _ in fn_list:
+            i.start()
+        result = [(ii.join(), changed) for ii, changed in fn_list]
+        for _data, changed in result:
+            if changed is not None:
+                for i in changed:
+                    data[i] = _data[i]
         return data
 
     @abc.abstractmethod
     def get_name(self) -> str:
         """
         获取游戏名称
```

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.4/pyproject.toml` & `gameyamlspiderandgenerator-1.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.4.4"
+version = "1.5.0"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -19,14 +19,15 @@
 requests = "^2.28.2"
 ruamel-base = "^1.0.0"
 loguru = "^0.6.0"
 pyyaml = "^6.0"
 pysocks = "^1.7.1"
 epicstore-api = "^0.1.6"
 jsonschema = "^4.17.3"
+openai = "^0.27.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `gameyamlspiderandgenerator-1.4.4/PKG-INFO` & `gameyamlspiderandgenerator-1.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.4.4
+Version: 1.5.0
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -12,14 +12,15 @@
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: epicstore-api (>=0.1.6,<0.2.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: ruamel-base (>=1.0.0,<2.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: ruamel.yaml.string (>=0.1.0,<0.2.0)
```

