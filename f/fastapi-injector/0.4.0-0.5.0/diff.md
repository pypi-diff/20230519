# Comparing `tmp/fastapi_injector-0.4.0.tar.gz` & `tmp/fastapi_injector-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_injector-0.4.0.tar", max compression
+gzip compressed data, was "fastapi_injector-0.5.0.tar", max compression
```

## Comparing `fastapi_injector-0.4.0.tar` & `fastapi_injector-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1326 2021-11-29 20:05:35.155753 fastapi_injector-0.4.0/LICENSE
--rw-r--r--   0        0        0     5737 2023-01-06 08:17:28.967047 fastapi_injector-0.4.0/README.md
--rw-r--r--   0        0        0      621 2023-01-06 08:10:56.889683 fastapi_injector-0.4.0/fastapi_injector/__init__.py
--rw-r--r--   0        0        0      618 2022-06-17 17:58:35.653761 fastapi_injector-0.4.0/fastapi_injector/attach.py
--rw-r--r--   0        0        0      217 2022-06-17 17:58:35.653761 fastapi_injector-0.4.0/fastapi_injector/exceptions.py
--rw-r--r--   0        0        0      971 2023-01-06 08:10:56.889683 fastapi_injector-0.4.0/fastapi_injector/injected.py
--rw-r--r--   0        0        0        0 2022-06-06 16:52:41.573382 fastapi_injector-0.4.0/fastapi_injector/py.typed
--rw-r--r--   0        0        0     2936 2022-06-17 17:58:35.653761 fastapi_injector-0.4.0/fastapi_injector/request_scope.py
--rw-r--r--   0        0        0      689 2023-01-06 08:18:36.184433 fastapi_injector-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6639 1970-01-01 00:00:00.000000 fastapi_injector-0.4.0/setup.py
--rw-r--r--   0        0        0     6540 1970-01-01 00:00:00.000000 fastapi_injector-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1326 2021-11-29 20:05:35.155753 fastapi_injector-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6332 2023-05-19 18:58:07.855882 fastapi_injector-0.5.0/README.md
+-rw-r--r--   0        0        0      673 2023-05-19 18:47:49.138684 fastapi_injector-0.5.0/fastapi_injector/__init__.py
+-rw-r--r--   0        0        0      618 2022-06-17 17:58:35.653761 fastapi_injector-0.5.0/fastapi_injector/attach.py
+-rw-r--r--   0        0        0      217 2022-06-17 17:58:35.653761 fastapi_injector-0.5.0/fastapi_injector/exceptions.py
+-rw-r--r--   0        0        0      971 2023-02-01 19:17:45.406262 fastapi_injector-0.5.0/fastapi_injector/injected.py
+-rw-r--r--   0        0        0        0 2022-06-06 16:52:41.573382 fastapi_injector-0.5.0/fastapi_injector/py.typed
+-rw-r--r--   0        0        0     3440 2023-05-19 18:47:49.138684 fastapi_injector-0.5.0/fastapi_injector/request_scope.py
+-rw-r--r--   0        0        0      894 2023-05-19 18:49:42.232117 fastapi_injector-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7288 1970-01-01 00:00:00.000000 fastapi_injector-0.5.0/PKG-INFO
```

### Comparing `fastapi_injector-0.4.0/LICENSE` & `fastapi_injector-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_injector-0.4.0/README.md` & `fastapi_injector-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -132,14 +132,27 @@
     foo: Interface = Injected(Interface),
     bar: Interface = Injected(Interface),
 ):
     # the following assert will pass because both are the same instance.
     assert foo is bar
 ```
 
+Outside of FastAPI routes, you can use `RequestScopeFactory.create_scope`, which returns a context manager that substitutes `InjectorMiddleware`.
+This is useful in celery tasks, cron jobs, CLI commands and other parts of your application outside of the request-response cycle.
+
+```python
+class MessageHandler:
+    def __init__(self, request_scope_factory: Inject[RequestScopeFactory]) -> None:
+        self.request_scope_factory = request_scope_factory
+
+    async def handle(self, message: Any) -> None:
+        with self.request_scope_factory.create_scope():
+            # process message
+```
+
 ### SyncInjected
 The dependency constructed by `Injected` is asynchronous. This causes it to run on the main thread. Should your usecase require a synchronous dependency, there's also an alternative - `SyncInjected`. Synchronous dependencies created by `SyncInjected` will be run on a separate thread from the threadpool. See the [FastAPI docs on this behaviour](https://fastapi.tiangolo.com/async/#dependencies).
 
 ## Testing with fastapi-injector
 
 To use your app in tests with overridden dependencies, modify the injector before each test:
```

### Comparing `fastapi_injector-0.4.0/fastapi_injector/__init__.py` & `fastapi_injector-0.5.0/fastapi_injector/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 
 from fastapi_injector.attach import attach_injector, get_injector_instance
 from fastapi_injector.exceptions import InjectorNotAttached
 from fastapi_injector.injected import Injected, SyncInjected
 from fastapi_injector.request_scope import (
     InjectorMiddleware,
     RequestScope,
+    RequestScopeFactory,
     request_scope,
 )
 
 __all__ = [
     "attach_injector",
     "get_injector_instance",
     "Injected",
     "SyncInjected",
     "InjectorNotAttached",
     "request_scope",
     "RequestScope",
+    "RequestScopeFactory",
     "InjectorMiddleware",
 ]
```

### Comparing `fastapi_injector-0.4.0/fastapi_injector/attach.py` & `fastapi_injector-0.5.0/fastapi_injector/attach.py`

 * *Files identical despite different names*

### Comparing `fastapi_injector-0.4.0/fastapi_injector/injected.py` & `fastapi_injector-0.5.0/fastapi_injector/injected.py`

 * *Files identical despite different names*

### Comparing `fastapi_injector-0.4.0/fastapi_injector/request_scope.py` & `fastapi_injector-0.5.0/fastapi_injector/request_scope.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 import uuid
+from contextlib import contextmanager
 from contextvars import ContextVar
 from typing import Any, Dict, Type
 
-from injector import Injector, InstanceProvider, Provider, Scope, ScopeDecorator, T
+from injector import (
+    Inject,
+    Injector,
+    InstanceProvider,
+    Provider,
+    Scope,
+    ScopeDecorator,
+    T,
+)
 from starlette.types import Receive, Send
 
 from fastapi_injector.exceptions import RequestScopeError
 
 _request_id_ctx: ContextVar[uuid.UUID] = ContextVar("request_id")
 
 
@@ -62,29 +71,44 @@
         """Clear the cache for a given request key."""
         del self.cache[key]
 
 
 request_scope = ScopeDecorator(RequestScope)
 
 
+class RequestScopeFactory:
+    """
+    Allows to create request scopes.
+    """
+
+    def __init__(self, request_scope_instance: Inject[RequestScope]) -> None:
+        self.request_scope_instance = request_scope_instance
+
+    @contextmanager
+    def create_scope(self):
+        """Creates a new request scope within dependencies are cached."""
+        rid = uuid.uuid4()
+        rid_ctx = _request_id_ctx.set(rid)
+        self.request_scope_instance.add_key(rid)
+        try:
+            yield
+        finally:
+            self.request_scope_instance.clear_key(rid)
+            _request_id_ctx.reset(rid_ctx)
+
+
 class InjectorMiddleware:
     """
     Middleware that enables request-scoped injection through ContextVar-based cache.
     """
 
     def __init__(self, app, injector: Injector) -> None:
         self.app = app
-        self.request_scope_instance = injector.get(RequestScope)
+        self.request_scope_factory = injector.get(RequestScopeFactory)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """
         Add an identifier to the request
         that can be used retrieve scoped dependencies.
         """
-        rid = uuid.uuid4()
-        rid_ctx = _request_id_ctx.set(rid)
-        self.request_scope_instance.add_key(rid)
-        try:
+        with self.request_scope_factory.create_scope():
             await self.app(scope, receive, send)
-        finally:
-            self.request_scope_instance.clear_key(rid)
-            _request_id_ctx.reset(rid_ctx)
```

### Comparing `fastapi_injector-0.4.0/setup.py` & `fastapi_injector-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,231 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fastapi-injector
+Version: 0.5.0
+Summary: python-injector integration for FastAPI
+Home-page: https://github.com/matyasrichter/fastapi-injector
+License: BSD
+Author: Matyas Richter
+Author-email: matyas@mrichter.cz
+Requires-Python: >=3.8,<3.12
+Classifier: Environment :: Web Environment
+Classifier: Framework :: FastAPI
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
+Requires-Dist: fastapi (>=0.70.0)
+Requires-Dist: injector (>=0.19.0)
+Project-URL: Repository, https://github.com/matyasrichter/fastapi-injector
+Description-Content-Type: text/markdown
+
+# FastAPI Injector
+
+![Workflow status](https://github.com/matyasrichter/fastapi-injector/actions/workflows/build.yml/badge.svg?branch=main)
+[![Coverage status](https://coveralls.io/repos/github/matyasrichter/fastapi-injector/badge.svg)](https://coveralls.io/github/matyasrichter/fastapi-injector?branch=main)
+
+Integrates [injector](https://github.com/alecthomas/injector) with [FastAPI](https://github.com/tiangolo/fastapi).
+
+Github: https://github.com/matyasrichter/fastapi-injector  
+PyPI: https://pypi.org/project/fastapi-injector/
+
+## Installation
+
+```shell
+pip install fastapi-injector
+```
+
+## Usage
+
+When creating your FastAPI app, attach the injector to it:
+
+```python
+# app.py
+from fastapi import FastAPI
+from injector import Injector
+from fastapi_injector import attach_injector
+
+
+def create_app(injector: Injector) -> FastAPI:
+    app = FastAPI()
+    app.include_router(...)
+    ...
+    attach_injector(app, injector)
+    return app
+```
+
+Then, use `Injected` in your routes. Under the hood, `Injected` is `Depends`, so you can use it anywhere `Depends` can be used. In the following example, `InterfaceType` is
+something you've bound an implementation to in your injector instance.
+
+```python
+from fastapi import APIRouter
+from fastapi_injector import Injected
+
+router = APIRouter()
+
+
+@router.get("/")
+async def get_root(integer: int = Injected(InterfaceType)):
+    return integer
+```
+
+A more complete example could look like this (your FastAPI code only depends on `InterfaceType`,
+its implementation only depends on a domain layer port etc.):
+
+```python
+# ------------------------
+# interface.py
+import abc
+from abc import abstractmethod
+
+
+class SomeInterface(abc.ABC):
+    @abstractmethod
+    async def create_some_entity(self) -> None:
+        """Creates and saves an entity."""
+
+
+# ------------------------
+# service.py
+import abc
+from .interface import SomeInterface
+
+
+class SomeSavePort(abc.ABC):
+    @abc.abstractmethod
+    async def save_something(self, something: Entity) -> None:
+        """Saves an entity."""
+
+
+class SomeService(SomeInterface):
+    def __init__(self, save_port: Inject[SomeSavePort]):
+        self.save_port = save_port
+
+    async def create_some_entity(self) -> None:
+        entity = Entity(attr1=1, attr2=2)
+        await self.save_port.save_something(entity)
+
+
+# ------------------------
+# repository.py
+from .service import SomeSavePort
+
+
+class SomeRepository(SomeSavePort):
+    async def save_something(self, something: Entity) -> None:
+# code that saves the entity to the DB
+```
+
+## Request scope
+A common requirement is to have a dependency resolved to the same instance multiple times in the same request,
+but to create new instances for other requests. An example usecase for this behaviour 
+is managing per-request DB connections.
+
+This library provides a `RequestScope` that fulfills this requirement.
+Under the hood, it uses [Context Variables](https://docs.python.org/3/library/contextvars.html)
+introduced in Python 3.7, generates a UUID4 for each request, and caches dependencies in a dictionary
+with this uuid as the key.
+
+```python
+from injector import Injector
+from fastapi import FastAPI
+from fastapi_injector import InjectorMiddleware, request_scope, attach_injector
+
+from foo.bar import Interface, Implementation
+
+inj = Injector()
+# Use request_scope when binding the dependency
+inj.binder.bind(Interface, to=Implementation, scope=request_scope)
+
+app = FastAPI()
+# Add the injector middleware to the app instance
+app.add_middleware(InjectorMiddleware, injector=inj)
+attach_injector(app, inj)
+```
+
+Your dependencies will then be cached within a request's resolution tree.
+Caching works both for top-level and nested dependencies
+(e.g. when you inject a DB connection to multiple repository classes).
+
+```python
+@app.get("/")
+def get_root(
+    foo: Interface = Injected(Interface),
+    bar: Interface = Injected(Interface),
+):
+    # the following assert will pass because both are the same instance.
+    assert foo is bar
+```
+
+Outside of FastAPI routes, you can use `RequestScopeFactory.create_scope`, which returns a context manager that substitutes `InjectorMiddleware`.
+This is useful in celery tasks, cron jobs, CLI commands and other parts of your application outside of the request-response cycle.
+
+```python
+class MessageHandler:
+    def __init__(self, request_scope_factory: Inject[RequestScopeFactory]) -> None:
+        self.request_scope_factory = request_scope_factory
+
+    async def handle(self, message: Any) -> None:
+        with self.request_scope_factory.create_scope():
+            # process message
+```
+
+### SyncInjected
+The dependency constructed by `Injected` is asynchronous. This causes it to run on the main thread. Should your usecase require a synchronous dependency, there's also an alternative - `SyncInjected`. Synchronous dependencies created by `SyncInjected` will be run on a separate thread from the threadpool. See the [FastAPI docs on this behaviour](https://fastapi.tiangolo.com/async/#dependencies).
+
+## Testing with fastapi-injector
+
+To use your app in tests with overridden dependencies, modify the injector before each test:
+
+```python
+# ------------------------
+# app entrypoint
+import pytest
+from injector import Injector
+
+app = create_app(inj)
+
+if __name__ == "__main__":
+    uvicorn.run("app", ...)
+
+
+# ------------------------
+# composition root
+def create_injector() -> Injector:
+    inj = Injector()
+    # note that this still gets executed,
+    # so if you need to get rid of a DB connection, for example,
+    # you would need to use a callable provider.
+    inj.binder.bind(int, 1)
+    return inj
+
+
+# ------------------------
+# tests
+from fastapi import FastAPI
+from fastapi.testclient import TestClient
+from path.to.app.factory import create_app
+
+
+@pytest.fixture
+def app() -> FastAPI:
+    inj = Injector()
+    inj.binder.bind(int, 2)
+    return create_app(inj)
+
+
+def some_test(app: FastAPI):
+    # use test client with the new app
+    client = TestClient(app)
+```
+
+## Contributing
+All contributions are welcome. Please raise an issue and/or open a pull request if you'd like to help to make `fastapi-injector` better.
+- Use [poetry](https://python-poetry.org/docs/) to install dependencies
+- Use [pre-commit](https://pre-commit.com/) to run linters and formatters before committing and pushing
+- Write tests for your code
 
-packages = \
-['fastapi_injector']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['fastapi>=0.70.0', 'injector>=0.19.0']
-
-setup_kwargs = {
-    'name': 'fastapi-injector',
-    'version': '0.4.0',
-    'description': 'python-injector integration for FastAPI',
-    'long_description': '# FastAPI Injector\n\n![Workflow status](https://github.com/matyasrichter/fastapi-injector/actions/workflows/build.yml/badge.svg?branch=main)\n[![Coverage status](https://coveralls.io/repos/github/matyasrichter/fastapi-injector/badge.svg)](https://coveralls.io/github/matyasrichter/fastapi-injector?branch=main)\n\nIntegrates [injector](https://github.com/alecthomas/injector) with [FastAPI](https://github.com/tiangolo/fastapi).\n\nGithub: https://github.com/matyasrichter/fastapi-injector  \nPyPI: https://pypi.org/project/fastapi-injector/\n\n## Installation\n\n```shell\npip install fastapi-injector\n```\n\n## Usage\n\nWhen creating your FastAPI app, attach the injector to it:\n\n```python\n# app.py\nfrom fastapi import FastAPI\nfrom injector import Injector\nfrom fastapi_injector import attach_injector\n\n\ndef create_app(injector: Injector) -> FastAPI:\n    app = FastAPI()\n    app.include_router(...)\n    ...\n    attach_injector(app, injector)\n    return app\n```\n\nThen, use `Injected` in your routes. Under the hood, `Injected` is `Depends`, so you can use it anywhere `Depends` can be used. In the following example, `InterfaceType` is\nsomething you\'ve bound an implementation to in your injector instance.\n\n```python\nfrom fastapi import APIRouter\nfrom fastapi_injector import Injected\n\nrouter = APIRouter()\n\n\n@router.get("/")\nasync def get_root(integer: int = Injected(InterfaceType)):\n    return integer\n```\n\nA more complete example could look like this (your FastAPI code only depends on `InterfaceType`,\nits implementation only depends on a domain layer port etc.):\n\n```python\n# ------------------------\n# interface.py\nimport abc\nfrom abc import abstractmethod\n\n\nclass SomeInterface(abc.ABC):\n    @abstractmethod\n    async def create_some_entity(self) -> None:\n        """Creates and saves an entity."""\n\n\n# ------------------------\n# service.py\nimport abc\nfrom .interface import SomeInterface\n\n\nclass SomeSavePort(abc.ABC):\n    @abc.abstractmethod\n    async def save_something(self, something: Entity) -> None:\n        """Saves an entity."""\n\n\nclass SomeService(SomeInterface):\n    def __init__(self, save_port: Inject[SomeSavePort]):\n        self.save_port = save_port\n\n    async def create_some_entity(self) -> None:\n        entity = Entity(attr1=1, attr2=2)\n        await self.save_port.save_something(entity)\n\n\n# ------------------------\n# repository.py\nfrom .service import SomeSavePort\n\n\nclass SomeRepository(SomeSavePort):\n    async def save_something(self, something: Entity) -> None:\n# code that saves the entity to the DB\n```\n\n## Request scope\nA common requirement is to have a dependency resolved to the same instance multiple times in the same request,\nbut to create new instances for other requests. An example usecase for this behaviour \nis managing per-request DB connections.\n\nThis library provides a `RequestScope` that fulfills this requirement.\nUnder the hood, it uses [Context Variables](https://docs.python.org/3/library/contextvars.html)\nintroduced in Python 3.7, generates a UUID4 for each request, and caches dependencies in a dictionary\nwith this uuid as the key.\n\n```python\nfrom injector import Injector\nfrom fastapi import FastAPI\nfrom fastapi_injector import InjectorMiddleware, request_scope, attach_injector\n\nfrom foo.bar import Interface, Implementation\n\ninj = Injector()\n# Use request_scope when binding the dependency\ninj.binder.bind(Interface, to=Implementation, scope=request_scope)\n\napp = FastAPI()\n# Add the injector middleware to the app instance\napp.add_middleware(InjectorMiddleware, injector=inj)\nattach_injector(app, inj)\n```\n\nYour dependencies will then be cached within a request\'s resolution tree.\nCaching works both for top-level and nested dependencies\n(e.g. when you inject a DB connection to multiple repository classes).\n\n```python\n@app.get("/")\ndef get_root(\n    foo: Interface = Injected(Interface),\n    bar: Interface = Injected(Interface),\n):\n    # the following assert will pass because both are the same instance.\n    assert foo is bar\n```\n\n### SyncInjected\nThe dependency constructed by `Injected` is asynchronous. This causes it to run on the main thread. Should your usecase require a synchronous dependency, there\'s also an alternative - `SyncInjected`. Synchronous dependencies created by `SyncInjected` will be run on a separate thread from the threadpool. See the [FastAPI docs on this behaviour](https://fastapi.tiangolo.com/async/#dependencies).\n\n## Testing with fastapi-injector\n\nTo use your app in tests with overridden dependencies, modify the injector before each test:\n\n```python\n# ------------------------\n# app entrypoint\nimport pytest\nfrom injector import Injector\n\napp = create_app(inj)\n\nif __name__ == "__main__":\n    uvicorn.run("app", ...)\n\n\n# ------------------------\n# composition root\ndef create_injector() -> Injector:\n    inj = Injector()\n    # note that this still gets executed,\n    # so if you need to get rid of a DB connection, for example,\n    # you would need to use a callable provider.\n    inj.binder.bind(int, 1)\n    return inj\n\n\n# ------------------------\n# tests\nfrom fastapi import FastAPI\nfrom fastapi.testclient import TestClient\nfrom path.to.app.factory import create_app\n\n\n@pytest.fixture\ndef app() -> FastAPI:\n    inj = Injector()\n    inj.binder.bind(int, 2)\n    return create_app(inj)\n\n\ndef some_test(app: FastAPI):\n    # use test client with the new app\n    client = TestClient(app)\n```\n\n## Contributing\nAll contributions are welcome. Please raise an issue and/or open a pull request if you\'d like to help to make `fastapi-injector` better.\n- Use [poetry](https://python-poetry.org/docs/) to install dependencies\n- Use [pre-commit](https://pre-commit.com/) to run linters and formatters before committing and pushing\n- Write tests for your code\n',
-    'author': 'Matyas Richter',
-    'author_email': 'matyas@mrichter.cz',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/matyasrichter/fastapi-injector',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

