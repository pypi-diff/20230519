# Comparing `tmp/pytest-lsp-0.2.1.tar.gz` & `tmp/pytest-lsp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-lsp-0.2.1.tar", last modified: Sat Jan 14 00:45:22 2023, max compression
+gzip compressed data, was "pytest-lsp-0.3.0.tar", last modified: Fri May 19 20:10:41 2023, max compression
```

## Comparing `pytest-lsp-0.2.1.tar` & `pytest-lsp-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 00:45:22.068549 pytest-lsp-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-01-14 00:45:22.068549 pytest-lsp-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 00:45:22.060548 pytest-lsp-0.2.1/pytest_lsp/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-14 00:44:49.000000 pytest-lsp-0.2.1/pytest_lsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/pytest_lsp/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/pytest_lsp/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 00:45:22.068549 pytest-lsp-0.2.1/pytest_lsp/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/pytest_lsp/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/pytest_lsp/clients/neovim_v0.6.1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/pytest_lsp/clients/visual_studio_code_v1.65.2.json
--rw-r--r--   0 runner    (1001) docker     (123)    38174 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/pytest_lsp/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/pytest_lsp/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/pytest_lsp/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 00:45:22.068549 pytest-lsp-0.2.1/pytest_lsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-01-14 00:45:22.000000 pytest-lsp-0.2.1/pytest_lsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-01-14 00:45:22.000000 pytest-lsp-0.2.1/pytest_lsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 00:45:22.000000 pytest-lsp-0.2.1/pytest_lsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-14 00:45:22.000000 pytest-lsp-0.2.1/pytest_lsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-14 00:45:22.000000 pytest-lsp-0.2.1/pytest_lsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-14 00:45:22.000000 pytest-lsp-0.2.1/pytest_lsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-01-14 00:45:22.068549 pytest-lsp-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-14 00:44:23.000000 pytest-lsp-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:10:41.471397 pytest-lsp-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-19 20:10:41.471397 pytest-lsp-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-19 20:10:30.000000 pytest-lsp-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:10:41.467397 pytest-lsp-0.3.0/pytest_lsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/pytest_lsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/pytest_lsp/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-19 20:10:30.000000 pytest-lsp-0.3.0/pytest_lsp/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:10:41.471397 pytest-lsp-0.3.0/pytest_lsp/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/pytest_lsp/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/pytest_lsp/clients/neovim_v0.6.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/pytest_lsp/clients/visual_studio_code_v1.65.2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    65916 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/pytest_lsp/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/pytest_lsp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/pytest_lsp/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/pytest_lsp/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:10:41.467397 pytest-lsp-0.3.0/pytest_lsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-19 20:10:41.000000 pytest-lsp-0.3.0/pytest_lsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-19 20:10:41.000000 pytest-lsp-0.3.0/pytest_lsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:10:41.000000 pytest-lsp-0.3.0/pytest_lsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 20:10:41.000000 pytest-lsp-0.3.0/pytest_lsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-19 20:10:41.000000 pytest-lsp-0.3.0/pytest_lsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 20:10:41.000000 pytest-lsp-0.3.0/pytest_lsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-19 20:10:41.471397 pytest-lsp-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:10:41.471397 pytest-lsp-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-19 20:10:01.000000 pytest-lsp-0.3.0/tests/test_plugin.py
```

### Comparing `pytest-lsp-0.2.1/LICENSE` & `pytest-lsp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-lsp-0.2.1/PKG-INFO` & `pytest-lsp-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,85 @@
 Metadata-Version: 2.1
 Name: pytest-lsp
-Version: 0.2.1
-Summary: Pytest plugin for end-to-end testing of language servers
-Home-page: https://alcarney.github.io/lsp-devtools
-Author: Alex Carney
-Author-email: alcarneyme@gmail.com
+Version: 0.3.0
+Summary: pytest plugin for end-to-end testing of language servers
+Author-email: Alex Carney <alcarneyme@gmail.com>
 License: MIT
-Project-URL: Bug Tracker, https://github.com/alcarney/lsp-devtools/issues
-Project-URL: Source Code, https://github.com/alcarney/lsp-devtools
-Platform: any
+Project-URL: Bug Tracker, https://github.com/swyddfa/lsp-devtools/issues
+Project-URL: Documentation, https://swyddfa.github.io/lsp-devtools/
+Project-URL: Source Code, https://github.com/swyddfa/lsp-devtools
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: typecheck
 License-File: LICENSE
 
 # pytest-lsp: End-to-end testing of language servers with pytest
 
-> This plugin is in **very** early development, it currently implements just enough to support the test suite of the [esbonio](https://github.com/swyddfa/esbonio) language server.
-
 `pytest-lsp` is a pytest plugin for writing end-to-end tests for language servers.
 
 It works by running the language server in a subprocess and communicating with it over stdio, just like a real language client.
 This also means `pytest-lsp` can be used to test language servers written in any language - not just Python.
 
 `pytest-lsp` relies on the [`pygls`](https://github.com/openlawlibrary/pygls) library for its language server protocol implementation.
 
 ```python
 import sys
-import pytest
+
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
+from lsprotocol.types import (
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import (
+    ClientServerConfig,
+    LanguageClient,
+    client_capabilities,
+)
 
 
 @pytest_lsp.fixture(
-    scope='session',
     config=ClientServerConfig(
         server_command=[sys.executable, "-m", "esbonio"],
-        root_uri="file:///path/to/test/project/root/"
     ),
 )
-async def client():
-    pass
-
-
-@pytest.mark.asyncio
-async def test_completion(client):
-    test_uri="file:///path/to/test/project/root/test_file.rst"
-    result = await client.completion_request(test_uri, line=5, character=23)
+async def client(lsp_client: LanguageClient):
+    # Setup
+    response = await lsp_client.initialize_session(
+        InitializeParams(
+            capabilities=client_capabilities("visual-studio-code"),
+            root_uri="file:///path/to/test/project/root/",
+        )
+    )
+
+    yield
+
+    # Teardown
+    await lsp_client.shutdown_session()
+
+
+async def test_completion(client: LanguageClient):
+    result = await client.text_document_completion_async(
+        params=CompletionParams(
+            position=Position(line=5, character=23),
+            text_document=TextDocumentIdentifier(
+                uri="file:///path/to/test/project/root/test_file.rst"
+            ),
+        )
+    )
 
     assert len(result.items) > 0
 ```
```

### Comparing `pytest-lsp-0.2.1/README.md` & `pytest-lsp-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,58 @@
 # pytest-lsp: End-to-end testing of language servers with pytest
 
-> This plugin is in **very** early development, it currently implements just enough to support the test suite of the [esbonio](https://github.com/swyddfa/esbonio) language server.
-
 `pytest-lsp` is a pytest plugin for writing end-to-end tests for language servers.
 
 It works by running the language server in a subprocess and communicating with it over stdio, just like a real language client.
 This also means `pytest-lsp` can be used to test language servers written in any language - not just Python.
 
 `pytest-lsp` relies on the [`pygls`](https://github.com/openlawlibrary/pygls) library for its language server protocol implementation.
 
 ```python
 import sys
-import pytest
+
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
+from lsprotocol.types import (
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import (
+    ClientServerConfig,
+    LanguageClient,
+    client_capabilities,
+)
 
 
 @pytest_lsp.fixture(
-    scope='session',
     config=ClientServerConfig(
         server_command=[sys.executable, "-m", "esbonio"],
-        root_uri="file:///path/to/test/project/root/"
     ),
 )
-async def client():
-    pass
-
-
-@pytest.mark.asyncio
-async def test_completion(client):
-    test_uri="file:///path/to/test/project/root/test_file.rst"
-    result = await client.completion_request(test_uri, line=5, character=23)
+async def client(lsp_client: LanguageClient):
+    # Setup
+    response = await lsp_client.initialize_session(
+        InitializeParams(
+            capabilities=client_capabilities("visual-studio-code"),
+            root_uri="file:///path/to/test/project/root/",
+        )
+    )
+
+    yield
+
+    # Teardown
+    await lsp_client.shutdown_session()
+
+
+async def test_completion(client: LanguageClient):
+    result = await client.text_document_completion_async(
+        params=CompletionParams(
+            position=Position(line=5, character=23),
+            text_document=TextDocumentIdentifier(
+                uri="file:///path/to/test/project/root/test_file.rst"
+            ),
+        )
+    )
 
     assert len(result.items) > 0
 ```
```

### Comparing `pytest-lsp-0.2.1/pytest_lsp/clients/neovim_v0.6.1.json` & `pytest-lsp-0.3.0/pytest_lsp/clients/neovim_v0.6.1.json`

 * *Files identical despite different names*

### Comparing `pytest-lsp-0.2.1/pytest_lsp/clients/visual_studio_code_v1.65.2.json` & `pytest-lsp-0.3.0/pytest_lsp/clients/visual_studio_code_v1.65.2.json`

 * *Files identical despite different names*

### Comparing `pytest-lsp-0.2.1/pytest_lsp.egg-info/PKG-INFO` & `pytest-lsp-0.3.0/pytest_lsp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,85 @@
 Metadata-Version: 2.1
 Name: pytest-lsp
-Version: 0.2.1
-Summary: Pytest plugin for end-to-end testing of language servers
-Home-page: https://alcarney.github.io/lsp-devtools
-Author: Alex Carney
-Author-email: alcarneyme@gmail.com
+Version: 0.3.0
+Summary: pytest plugin for end-to-end testing of language servers
+Author-email: Alex Carney <alcarneyme@gmail.com>
 License: MIT
-Project-URL: Bug Tracker, https://github.com/alcarney/lsp-devtools/issues
-Project-URL: Source Code, https://github.com/alcarney/lsp-devtools
-Platform: any
+Project-URL: Bug Tracker, https://github.com/swyddfa/lsp-devtools/issues
+Project-URL: Documentation, https://swyddfa.github.io/lsp-devtools/
+Project-URL: Source Code, https://github.com/swyddfa/lsp-devtools
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: typecheck
 License-File: LICENSE
 
 # pytest-lsp: End-to-end testing of language servers with pytest
 
-> This plugin is in **very** early development, it currently implements just enough to support the test suite of the [esbonio](https://github.com/swyddfa/esbonio) language server.
-
 `pytest-lsp` is a pytest plugin for writing end-to-end tests for language servers.
 
 It works by running the language server in a subprocess and communicating with it over stdio, just like a real language client.
 This also means `pytest-lsp` can be used to test language servers written in any language - not just Python.
 
 `pytest-lsp` relies on the [`pygls`](https://github.com/openlawlibrary/pygls) library for its language server protocol implementation.
 
 ```python
 import sys
-import pytest
+
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
+from lsprotocol.types import (
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import (
+    ClientServerConfig,
+    LanguageClient,
+    client_capabilities,
+)
 
 
 @pytest_lsp.fixture(
-    scope='session',
     config=ClientServerConfig(
         server_command=[sys.executable, "-m", "esbonio"],
-        root_uri="file:///path/to/test/project/root/"
     ),
 )
-async def client():
-    pass
-
-
-@pytest.mark.asyncio
-async def test_completion(client):
-    test_uri="file:///path/to/test/project/root/test_file.rst"
-    result = await client.completion_request(test_uri, line=5, character=23)
+async def client(lsp_client: LanguageClient):
+    # Setup
+    response = await lsp_client.initialize_session(
+        InitializeParams(
+            capabilities=client_capabilities("visual-studio-code"),
+            root_uri="file:///path/to/test/project/root/",
+        )
+    )
+
+    yield
+
+    # Teardown
+    await lsp_client.shutdown_session()
+
+
+async def test_completion(client: LanguageClient):
+    result = await client.text_document_completion_async(
+        params=CompletionParams(
+            position=Position(line=5, character=23),
+            text_document=TextDocumentIdentifier(
+                uri="file:///path/to/test/project/root/test_file.rst"
+            ),
+        )
+    )
 
     assert len(result.items) > 0
 ```
```

### Comparing `pytest-lsp-0.2.1/pytest_lsp.egg-info/SOURCES.txt` & `pytest-lsp-0.3.0/pytest_lsp.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 pytest_lsp/__init__.py
-pytest_lsp/check.py
+pytest_lsp/checks.py
 pytest_lsp/client.py
 pytest_lsp/gen.py
 pytest_lsp/plugin.py
+pytest_lsp/protocol.py
 pytest_lsp/py.typed
 pytest_lsp.egg-info/PKG-INFO
 pytest_lsp.egg-info/SOURCES.txt
 pytest_lsp.egg-info/dependency_links.txt
 pytest_lsp.egg-info/entry_points.txt
 pytest_lsp.egg-info/requires.txt
 pytest_lsp.egg-info/top_level.txt
 pytest_lsp/clients/__init__.py
 pytest_lsp/clients/neovim_v0.6.1.json
-pytest_lsp/clients/visual_studio_code_v1.65.2.json
+pytest_lsp/clients/visual_studio_code_v1.65.2.json
+tests/test_client.py
+tests/test_examples.py
+tests/test_plugin.py
```

