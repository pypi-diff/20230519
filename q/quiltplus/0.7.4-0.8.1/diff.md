# Comparing `tmp/quiltplus-0.7.4.tar.gz` & `tmp/quiltplus-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltplus-0.7.4.tar", max compression
+gzip compressed data, was "quiltplus-0.8.1.tar", max compression
```

## Comparing `quiltplus-0.7.4.tar` & `quiltplus-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.7.4/LICENSE.md
--rw-r--r--   0        0        0     1183 2023-03-02 00:44:34.769534 quiltplus-0.7.4/README.md
--rw-r--r--   0        0        0      814 2023-04-06 00:37:02.810343 quiltplus-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      697 2023-03-01 19:37:11.442576 quiltplus-0.7.4/quiltplus/__init__.py
--rw-r--r--   0        0        0     3258 2023-03-01 19:37:11.442886 quiltplus-0.7.4/quiltplus/cache.py
--rw-r--r--   0        0        0       36 2023-03-01 19:37:11.443193 quiltplus-0.7.4/quiltplus/cli/__init__.py
--rw-r--r--   0        0        0      612 2023-03-01 19:37:11.443370 quiltplus-0.7.4/quiltplus/cli/catalog.py
--rw-r--r--   0        0        0      237 2023-03-01 19:37:11.443620 quiltplus-0.7.4/quiltplus/cli/context.py
--rw-r--r--   0        0        0      927 2023-03-01 19:37:11.443833 quiltplus-0.7.4/quiltplus/cli/depend.py
--rw-r--r--   0        0        0     1168 2023-03-01 19:37:11.444170 quiltplus-0.7.4/quiltplus/cli/group.py
--rw-r--r--   0        0        0      665 2023-03-01 19:37:11.444406 quiltplus-0.7.4/quiltplus/cli/pkg.py
--rwxr-xr-x   0        0        0      127 2023-02-27 04:37:56.107220 quiltplus-0.7.4/quiltplus/cli/qp.py
--rw-r--r--   0        0        0     1009 2023-03-01 19:37:11.444736 quiltplus-0.7.4/quiltplus/cli/stage.py
--rw-r--r--   0        0        0     5712 2023-03-01 19:37:11.445107 quiltplus-0.7.4/quiltplus/config.py
--rw-r--r--   0        0        0     3178 2023-04-06 00:33:15.758389 quiltplus-0.7.4/quiltplus/id.py
--rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.7.4/quiltplus/ignore.py
--rw-r--r--   0        0        0     4830 2023-04-06 00:35:26.424277 quiltplus-0.7.4/quiltplus/package.py
--rw-r--r--   0        0        0     1668 2023-03-01 19:37:11.447225 quiltplus-0.7.4/quiltplus/parse.py
--rw-r--r--   0        0        0     1375 2023-03-01 19:37:11.447556 quiltplus-0.7.4/quiltplus/unparse.py
--rw-r--r--   0        0        0     1953 1970-01-01 00:00:00.000000 quiltplus-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.8.1/LICENSE.md
+-rw-r--r--   0        0        0     1183 2023-03-02 00:44:34.769534 quiltplus-0.8.1/README.md
+-rw-r--r--   0        0        0      842 2023-05-19 20:33:53.562381 quiltplus-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      821 2023-05-19 20:32:18.927042 quiltplus-0.8.1/quiltplus/__init__.py
+-rw-r--r--   0        0        0     3258 2023-03-01 19:37:11.442886 quiltplus-0.8.1/quiltplus/cache.py
+-rw-r--r--   0        0        0       36 2023-03-01 19:37:11.443193 quiltplus-0.8.1/quiltplus/cli/__init__.py
+-rw-r--r--   0        0        0      612 2023-03-01 19:37:11.443370 quiltplus-0.8.1/quiltplus/cli/catalog.py
+-rw-r--r--   0        0        0      237 2023-03-01 19:37:11.443620 quiltplus-0.8.1/quiltplus/cli/context.py
+-rw-r--r--   0        0        0      927 2023-03-01 19:37:11.443833 quiltplus-0.8.1/quiltplus/cli/depend.py
+-rw-r--r--   0        0        0     1168 2023-03-01 19:37:11.444170 quiltplus-0.8.1/quiltplus/cli/group.py
+-rw-r--r--   0        0        0      665 2023-03-01 19:37:11.444406 quiltplus-0.8.1/quiltplus/cli/pkg.py
+-rwxr-xr-x   0        0        0      127 2023-02-27 04:37:56.107220 quiltplus-0.8.1/quiltplus/cli/qp.py
+-rw-r--r--   0        0        0     1009 2023-03-01 19:37:11.444736 quiltplus-0.8.1/quiltplus/cli/stage.py
+-rw-r--r--   0        0        0     5712 2023-03-01 19:37:11.445107 quiltplus-0.8.1/quiltplus/config.py
+-rw-r--r--   0        0        0     3227 2023-05-19 18:59:56.847388 quiltplus-0.8.1/quiltplus/id.py
+-rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.8.1/quiltplus/ignore.py
+-rw-r--r--   0        0        0     5025 2023-05-19 18:59:56.848083 quiltplus-0.8.1/quiltplus/package.py
+-rw-r--r--   0        0        0     1867 2023-05-19 18:59:56.848713 quiltplus-0.8.1/quiltplus/parse.py
+-rw-r--r--   0        0        0      696 2023-05-19 18:59:56.848983 quiltplus-0.8.1/quiltplus/registry.py
+-rw-r--r--   0        0        0      524 2023-05-19 20:33:14.589232 quiltplus-0.8.1/quiltplus/resource.py
+-rw-r--r--   0        0        0      467 2023-05-19 18:59:56.849553 quiltplus-0.8.1/quiltplus/types.py
+-rw-r--r--   0        0        0     1375 2023-05-19 17:22:44.235928 quiltplus-0.8.1/quiltplus/unparse.py
+-rw-r--r--   0        0        0      779 2023-05-19 18:59:56.850051 quiltplus-0.8.1/quiltplus/versions.py
+-rw-r--r--   0        0        0     2052 1970-01-01 00:00:00.000000 quiltplus-0.8.1/PKG-INFO
```

### Comparing `quiltplus-0.7.4/LICENSE.md` & `quiltplus-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/README.md` & `quiltplus-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/pyproject.toml` & `quiltplus-0.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "quiltplus"
-version = "0.7.4"
+version = "0.8.1"
 description = "Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["yaml", "api", "resource", "quilt"]
 packages = [
    { include = "quiltplus" }
 ]
 
 [tool.poetry.scripts]
 qp = "quiltplus.cli.qp:cli"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 quilt3 = "^5.1.0"
 trio = "^0.22.0"
 isort = "^5.12.0"
 asyncclick = "^8.1.3.4"
 pytest-cov = "^4.0.0"
 # anyio = "^3.6.1"
 # anyio = {git = "https://github.com/agronholm/anyio.git"}
 anyio = "^3.6.2"
+typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 pytest-trio = "^0.8.0"
 pytest-watcher = "^0.2.6"
 
 [build-system]
```

### Comparing `quiltplus-0.7.4/quiltplus/cache.py` & `quiltplus-0.8.1/quiltplus/cache.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/quiltplus/cli/catalog.py` & `quiltplus-0.8.1/quiltplus/cli/catalog.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/quiltplus/cli/depend.py` & `quiltplus-0.8.1/quiltplus/cli/depend.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/quiltplus/cli/group.py` & `quiltplus-0.8.1/quiltplus/cli/group.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/quiltplus/cli/pkg.py` & `quiltplus-0.8.1/quiltplus/cli/pkg.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/quiltplus/cli/stage.py` & `quiltplus-0.8.1/quiltplus/cli/stage.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/quiltplus/config.py` & `quiltplus-0.8.1/quiltplus/config.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/quiltplus/id.py` & `quiltplus-0.8.1/quiltplus/id.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Create Immutable Identifier from a Quilt+ URI
 import logging
 from pathlib import Path
 from socket import gethostname
 from tempfile import TemporaryDirectory
 
-from .parse import K_BKT, K_CAT, K_HSH, K_PKG, K_STR, K_STR_DEFAULT, PREFIX, TYPES, QuiltParse
+from .parse import (
+    K_BKT,
+    K_CAT,
+    K_HSH,
+    K_PKG,
+    K_PTH,
+    K_STR,
+    K_STR_DEFAULT,
+    PREFIX,
+    QuiltParse,
+)
 from .unparse import QuiltUnparse
 
 
 class QuiltID(QuiltParse):
     DEFAULT_CATALOG = "open.quiltdata.com"
     LOCAL_HOST = gethostname()
     LOCAL_SCHEME = "local"
@@ -80,14 +90,19 @@
     def source_uri(self):
         return self._source_uri
 
     def quilt_uri(self):
         uri_string = QuiltUnparse(self.attrs).unparse()
         return uri_string
 
+    def path_uri(self, path: str):
+        attrs = {**self.attrs, K_PTH: path}
+        uri_string = QuiltUnparse(attrs).unparse()
+        return uri_string
+
     def catalog_uri(self):
         catalog = self.get(K_CAT, QuiltID.DEFAULT_CATALOG)
         uri_string = f"https://{catalog}/b/{self.get(K_BKT)}"
         if self.has_package:
             uri_string += f"/packages/{self.get(K_PKG)}"
         return uri_string
 
@@ -95,17 +110,13 @@
         return {
             index: self.index,
             title: self.get(K_PKG),
             subtitle: self.source_uri(),
         }
 
     def type(self):
-        for index, key in enumerate(TYPES):
-            next_key = TYPES[index + 1]
-            if next_key not in self.attrs:
-                return key
-        return False
+        return self._type
 
     def __del__(self):
         if self._cleanup:
             print(f"{__class__.__name__}.__del__[{self._tempDir}]")
             self._tempDir.cleanup()
```

### Comparing `quiltplus-0.7.4/quiltplus/ignore.py` & `quiltplus-0.8.1/quiltplus/ignore.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/quiltplus/package.py` & `quiltplus-0.8.1/quiltplus/package.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Resource-oriented version of a Quilt Package
-# (must already exist, at least for now)
 
 import logging
 import os
 import platform
 import shutil
 import subprocess
 
 from quilt3 import Package
+from typing_extensions import Self
 
 from .config import QuiltConfig
-from .id import K_PKG, QuiltID
+from .id import QuiltID
 
 
 class QuiltPackage:
     METHOD_NAMES = "get list diff patch put post".split(" ")
 
     @staticmethod
     def FromURI(url_string: str):
@@ -39,14 +39,17 @@
         self.registry = id.registry()
         self._local_path = root / id.sub_path() if root else id.local_path()
         self.config = QuiltConfig.ForRoot(self._local_path)
 
     def __repr__(self):
         return f"QuiltPackage[{self.id}]@{self.local_path()})"
 
+    def __eq__(self, other: Self):
+        return self.registry == other.registry
+
     def __str__(self):
         return self.__repr__()
 
     def local_path(self, *paths: str):
         p = self._local_path
         for path in paths:
             p = p / path
@@ -92,21 +95,24 @@
     async def local(self):
         q = Package().set_dir(".", path=self.dest())
         return q
 
     async def remote(self):
         return await self.browse()
 
-    async def list(self, changed_only=False):
+    async def child(self, changed_only=False):
         if changed_only:
             diffs = await self.diff()
             return [x for sub in diffs.values() for x in sub]
         q = await self.remote()
         return list(q.keys())
 
+    async def list(self, changed_only=False):
+        return [self.id.path_uri(k) for k in await self.child(changed_only)]
+
     async def diff(self):
         logging.debug(f"\ndiff.local_files\n{self.local_files()}")
         q_remote = await self.remote()
         logging.debug(f"diff.remote_keys {q_remote.keys()}")
         q_local = await self.local()
         logging.debug(f"diff.local_keys {q_local.keys()}")
         diffs = q_remote.diff(q_local)
```

### Comparing `quiltplus-0.7.4/quiltplus/parse.py` & `quiltplus-0.8.1/quiltplus/parse.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 K_HSH = "top_hash"
 K_BKT = "bucket"
 K_PKG = "package"
 K_PTH = "path"
 K_PRP = "property"
 K_QRY = "query"
 K_TAG = "tag"
+K_VER = "versions"
 K_CAT = "catalog"
 
 K_PKG_FULL = "__package__"
 K_STR_DEFAULT = "s3"
-TYPES = [K_STR, K_BKT, K_PKG, K_CAT, K_PTH, K_PRP, K_QRY, None]
 FRAG_KEYS = [K_PKG_FULL, K_PTH, K_PRP, K_CAT]
 
 
 class QuiltParse:
     def __init__(self, uri_string):
         self.uri = urlparse(uri_string)
         self.attrs = self.parse_fragments(self.uri.fragment)
@@ -39,22 +39,30 @@
         return scalars
 
     def parse_id(self, host):
         if PREFIX not in self.uri.scheme:
             raise ValueError(f"Error: invalid URI scheme {self.uri.scheme}: {self.uri}")
         self.attrs[K_STR] = self.uri.scheme.replace(PREFIX, "")
         self.attrs[K_BKT] = host
+        self._type = K_BKT
         self.has_package = self.parse_package()
+        if K_PRP in self.attrs:
+            self._type = K_PRP
+        elif K_PTH in self.attrs:
+            self._type = K_PTH
 
     def parse_package(self):
         if K_PKG not in self.attrs:
             return False
         pkg = self.attrs[K_PKG]
+        self._type = K_VER
         if "@" in pkg:
+            self._type = K_PKG
             s = pkg.split("@")
             self.attrs[K_HSH] = s[1]
             self.attrs[K_PKG] = s[0]
         if ":" in pkg:
+            self._type = K_PKG
             s = pkg.split(":")
             self.attrs[K_TAG] = s[1]
             self.attrs[K_PKG] = s[0]
         return True
```

### Comparing `quiltplus-0.7.4/quiltplus/unparse.py` & `quiltplus-0.8.1/quiltplus/unparse.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.7.4/PKG-INFO` & `quiltplus-0.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: quiltplus
-Version: 0.7.4
+Version: 0.8.1
 Summary: Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform
 License: MIT
 Keywords: yaml,api,resource,quilt
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.6.2,<4.0.0)
 Requires-Dist: asyncclick (>=8.1.3.4,<9.0.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: quilt3 (>=5.1.0,<6.0.0)
 Requires-Dist: trio (>=0.22.0,<0.23.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # quiltplus
 
 Resource-oriented API for Quilt's decentralized social knowledge platform
 
 ## Command-Line QuickStart
```

