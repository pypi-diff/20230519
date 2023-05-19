# Comparing `tmp/cacheyou-23.0.tar.gz` & `tmp/cacheyou-23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacheyou-23.0.tar", last modified: Fri May 19 03:37:08 2023, max compression
+gzip compressed data, was "cacheyou-23.1.tar", last modified: Fri May 19 10:41:10 2023, max compression
```

## Comparing `cacheyou-23.0.tar` & `cacheyou-23.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0      575 2023-05-19 03:36:49.481905 cacheyou-23.0/LICENSE.txt
--rw-r--r--   0        0        0      830 2023-05-19 03:36:49.481905 cacheyou-23.0/README.md
--rw-r--r--   0        0        0      516 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/__init__.py
--rw-r--r--   0        0        0     1330 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/_cmd.py
--rw-r--r--   0        0        0     4963 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/adapter.py
--rw-r--r--   0        0        0     1543 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/cache.py
--rw-r--r--   0        0        0      288 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/caches/__init__.py
--rw-r--r--   0        0        0     4857 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/caches/file_cache.py
--rw-r--r--   0        0        0     1145 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/caches/redis_cache.py
--rw-r--r--   0        0        0    16692 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/controller.py
--rw-r--r--   0        0        0     3955 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/filewrapper.py
--rw-r--r--   0        0        0     4282 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/heuristics.py
--rw-r--r--   0        0        0     6453 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/serialize.py
--rw-r--r--   0        0        0      806 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/wrapper.py
--rw-r--r--   0        0        0     5673 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/Makefile
--rw-r--r--   0        0        0     8068 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/conf.py
--rw-r--r--   0        0        0     5478 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/custom_heuristics.rst
--rw-r--r--   0        0        0     5209 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/etags.rst
--rw-r--r--   0        0        0     2289 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/index.rst
--rw-r--r--   0        0        0     4040 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/release_notes.rst
--rw-r--r--   0        0        0      643 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/requirements.txt
--rw-r--r--   0        0        0     4297 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/storage.rst
--rw-r--r--   0        0        0     2372 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/tips.rst
--rw-r--r--   0        0        0     1792 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/usage.rst
--rw-r--r--   0        0        0     2501 2023-05-19 03:37:08.830092 cacheyou-23.0/pyproject.toml
--rw-r--r--   0        0        0       30 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/__init__.py
--rw-r--r--   0        0        0     4750 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/conftest.py
--rw-r--r--   0        0        0     1098 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/issue_263.py
--rw-r--r--   0        0        0     1682 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/test_adapter.py
--rw-r--r--   0        0        0    10845 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/test_cache_control.py
--rw-r--r--   0        0        0     1470 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/test_chunked_response.py
--rw-r--r--   0        0        0     5110 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_etag.py
--rw-r--r--   0        0        0     6679 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_expires_heuristics.py
--rw-r--r--   0        0        0     1769 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_max_age.py
--rw-r--r--   0        0        0     1597 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_redirects.py
--rw-r--r--   0        0        0      955 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_regressions.py
--rw-r--r--   0        0        0     5380 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_serialization.py
--rw-r--r--   0        0        0      259 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_server_http_version.py
--rw-r--r--   0        0        0     5633 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_storage_filecache.py
--rw-r--r--   0        0        0      789 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_storage_redis.py
--rw-r--r--   0        0        0     2957 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_vary.py
--rw-r--r--   0        0        0      792 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/utils.py
--rw-r--r--   0        0        0      484 2023-05-19 03:36:49.485906 cacheyou-23.0/tox.ini
--rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 cacheyou-23.0/PKG-INFO
+-rw-r--r--   0        0        0      575 2023-05-19 10:40:54.836398 cacheyou-23.1/LICENSE.txt
+-rw-r--r--   0        0        0      830 2023-05-19 10:40:54.836398 cacheyou-23.1/README.md
+-rw-r--r--   0        0        0      516 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/_cmd.py
+-rw-r--r--   0        0        0     5832 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/adapter.py
+-rw-r--r--   0        0        0     1895 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/cache.py
+-rw-r--r--   0        0        0      288 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/caches/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/caches/file_cache.py
+-rw-r--r--   0        0        0     1709 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/caches/redis_cache.py
+-rw-r--r--   0        0        0    17699 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/controller.py
+-rw-r--r--   0        0        0     4208 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/filewrapper.py
+-rw-r--r--   0        0        0     4808 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/heuristics.py
+-rw-r--r--   0        0        0        0 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/py.typed
+-rw-r--r--   0        0        0     7348 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/serialize.py
+-rw-r--r--   0        0        0     1284 2023-05-19 10:40:54.836398 cacheyou-23.1/cacheyou/wrapper.py
+-rw-r--r--   0        0        0     5673 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/Makefile
+-rw-r--r--   0        0        0     8119 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/conf.py
+-rw-r--r--   0        0        0     5478 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/custom_heuristics.rst
+-rw-r--r--   0        0        0     5209 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/etags.rst
+-rw-r--r--   0        0        0     2289 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/index.rst
+-rw-r--r--   0        0        0     4085 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/release_notes.rst
+-rw-r--r--   0        0        0      643 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/requirements.txt
+-rw-r--r--   0        0        0     4297 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/storage.rst
+-rw-r--r--   0        0        0     2372 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/tips.rst
+-rw-r--r--   0        0        0     1792 2023-05-19 10:40:54.836398 cacheyou-23.1/docs/usage.rst
+-rw-r--r--   0        0        0     2626 2023-05-19 10:41:10.088362 cacheyou-23.1/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/__init__.py
+-rw-r--r--   0        0        0     4750 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/conftest.py
+-rw-r--r--   0        0        0     1114 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/issue_263.py
+-rw-r--r--   0        0        0     1682 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_adapter.py
+-rw-r--r--   0        0        0    10845 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_cache_control.py
+-rw-r--r--   0        0        0     1470 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_chunked_response.py
+-rw-r--r--   0        0        0     5110 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_etag.py
+-rw-r--r--   0        0        0     6679 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_expires_heuristics.py
+-rw-r--r--   0        0        0     1747 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_max_age.py
+-rw-r--r--   0        0        0     1597 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_redirects.py
+-rw-r--r--   0        0        0      941 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_regressions.py
+-rw-r--r--   0        0        0     5484 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_serialization.py
+-rw-r--r--   0        0        0      259 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_server_http_version.py
+-rw-r--r--   0        0        0     5689 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_storage_filecache.py
+-rw-r--r--   0        0        0      789 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_storage_redis.py
+-rw-r--r--   0        0        0     2957 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/test_vary.py
+-rw-r--r--   0        0        0      792 2023-05-19 10:40:54.840398 cacheyou-23.1/tests/utils.py
+-rw-r--r--   0        0        0      484 2023-05-19 10:40:54.840398 cacheyou-23.1/tox.ini
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 cacheyou-23.1/PKG-INFO
```

### Comparing `cacheyou-23.0/LICENSE.txt` & `cacheyou-23.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/README.md` & `cacheyou-23.1/README.md`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/cacheyou/__init__.py` & `cacheyou-23.1/cacheyou/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 """
 import logging
 
 from cacheyou.adapter import CacheControlAdapter
 from cacheyou.controller import CacheController
 from cacheyou.wrapper import CacheControl
 
-__version__ = "23.0"
+__version__ = "23.1"
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __all__ = ("CacheControl", "CacheControlAdapter", "CacheController")
```

### Comparing `cacheyou-23.0/cacheyou/_cmd.py` & `cacheyou-23.1/cacheyou/_cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 # SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import logging
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 
 import requests
 
 from cacheyou.adapter import CacheControlAdapter
 from cacheyou.cache import DictCache
 from cacheyou.controller import logger
 
 
-def setup_logging():
+def setup_logging() -> None:
     logger.setLevel(logging.DEBUG)
     handler = logging.StreamHandler()
     logger.addHandler(handler)
 
 
-def get_session():
-    adapter = CacheControlAdapter(
-        DictCache(), cache_etags=True, serializer=None, heuristic=None
-    )
+def get_session() -> requests.Session:
+    adapter = CacheControlAdapter(DictCache(), cache_etags=True, serializer=None, heuristic=None)
     sess = requests.Session()
     sess.mount("http://", adapter)
     sess.mount("https://", adapter)
 
-    sess.cache_controller = adapter.controller
+    sess.cache_controller = adapter.controller  # type:ignore[attr-defined]
     return sess
 
 
-def get_args():
+def get_args() -> Namespace:
     parser = ArgumentParser()
     parser.add_argument("url", help="The URL to try and cache")
     return parser.parse_args()
 
 
-def main(args=None):
+def main() -> None:
     args = get_args()
     sess = get_session()
 
     # Make a request to get a response
     resp = sess.get(args.url)
 
     # Turn on logging
     setup_logging()
 
     # try setting the cache
-    sess.cache_controller.cache_response(resp.request, resp.raw)
+    sess.cache_controller.cache_response(resp.request, resp.raw)  # type: ignore[attr-defined]
 
     # Now try to get it
-    if sess.cache_controller.cached_request(resp.request):
+    if sess.cache_controller.cached_request(resp.request):  # type: ignore[attr-defined]
         print("Cached!")
     else:
         print("Not cached :(")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cacheyou-23.0/cacheyou/adapter.py` & `cacheyou-23.1/cacheyou/adapter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,62 @@
 # SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
 import functools
 import types
+import typing as t
 import zlib
 
 from requests.adapters import HTTPAdapter
 
 from cacheyou.cache import DictCache
 from cacheyou.controller import PERMANENT_REDIRECT_STATUSES, CacheController
 from cacheyou.filewrapper import CallbackFileWrapper
 
+if t.TYPE_CHECKING:
+    import requests
+    from urllib3.response import HTTPResponse
+
+    from cacheyou.cache import BaseCache
+    from cacheyou.heuristics import BaseHeuristic
+    from cacheyou.serialize import Serializer
+
 
 class CacheControlAdapter(HTTPAdapter):
     invalidating_methods = {"PUT", "PATCH", "DELETE"}
 
     def __init__(
         self,
-        cache=None,
-        cache_etags=True,
-        controller_class=None,
-        serializer=None,
-        heuristic=None,
-        cacheable_methods=None,
-        *args,
-        **kw,
+        cache: BaseCache | None = None,
+        cache_etags: bool = True,
+        controller_class: type[CacheController] | None = None,
+        serializer: Serializer | None = None,
+        heuristic: BaseHeuristic | None = None,
+        cacheable_methods: t.Collection[str] | None = None,
+        *args: t.Any,
+        **kw: t.Any,
     ):
         super().__init__(*args, **kw)
         self.cache = DictCache() if cache is None else cache
         self.heuristic = heuristic
         self.cacheable_methods = cacheable_methods or ("GET",)
 
         controller_factory = controller_class or CacheController
         self.controller = controller_factory(
             self.cache, cache_etags=cache_etags, serializer=serializer
         )
 
-    def send(self, request, cacheable_methods=None, **kw):
+    def send(  # type: ignore[override]
+        self,
+        request: requests.PreparedRequest,
+        cacheable_methods: t.Collection[str] | None = None,
+        **kw: t.Any,
+    ) -> requests.Response:
         """
         Send a request. Use the request information to see if it
         exists in the cache and cache the response if we need to and can.
         """
         cacheable = cacheable_methods or self.cacheable_methods
         if request.method in cacheable:
             try:
@@ -55,16 +70,20 @@
             request.headers.update(self.controller.conditional_headers(request))
 
         resp = super().send(request, **kw)
 
         return resp
 
     def build_response(
-        self, request, response, from_cache=False, cacheable_methods=None
-    ):
+        self,
+        request: requests.PreparedRequest,
+        response: HTTPResponse,
+        from_cache: bool = False,
+        cacheable_methods: t.Collection[str] | None = None,
+    ) -> requests.Response:
         """
         Build a response by making a request or using the cache.
 
         This will end up calling send and returning a potentially
         cached response
         """
         cacheable = cacheable_methods or self.cacheable_methods
@@ -76,17 +95,15 @@
 
             # apply any expiration heuristics
             if response.status == 304:
                 # We must have sent an ETag request. This could mean
                 # that we've been expired already or that we simply
                 # have an etag. In either case, we want to try and
                 # update the cache if that is the case.
-                cached_response = self.controller.update_cached_response(
-                    request, response
-                )
+                cached_response = self.controller.update_cached_response(request, response)
 
                 if cached_response is not response:
                     from_cache = True
 
                 # We are done with the server response, read a
                 # possible response body (compliant servers will
                 # not return one, but we cannot be 100% sure) and
@@ -98,40 +115,40 @@
 
             # We always cache the 301 responses
             elif int(response.status) in PERMANENT_REDIRECT_STATUSES:
                 self.controller.cache_response(request, response)
             else:
                 # Wrap the response file with a wrapper that will cache the
                 #   response when the stream has been consumed.
-                response._fp = CallbackFileWrapper(
-                    response._fp,
-                    functools.partial(
-                        self.controller.cache_response, request, response
-                    ),
+                response._fp = CallbackFileWrapper(  # type: ignore[assignment, attr-defined]
+                    response._fp,  # type: ignore[attr-defined]
+                    functools.partial(self.controller.cache_response, request, response),
                 )
                 if response.chunked:
-                    super_update_chunk_length = response._update_chunk_length
+                    super_update_chunk_length = (
+                        response._update_chunk_length  # type: ignore[attr-defined]
+                    )
 
                     def _update_chunk_length(self):
                         super_update_chunk_length()
                         if self.chunk_left == 0:
                             self._fp._close()
 
-                    response._update_chunk_length = types.MethodType(
+                    response._update_chunk_length = types.MethodType(  # type: ignore[attr-defined]
                         _update_chunk_length, response
                     )
 
-        resp = super().build_response(request, response)
+        resp: requests.Response = super().build_response(request, response)
 
         # See if we should invalidate the cache.
         if request.method in self.invalidating_methods and resp.ok:
-            cache_url = self.controller.cache_url(request.url)
+            cache_url = self.controller.cache_url(t.cast(str, request.url))
             self.cache.delete(cache_url)
 
         # Give the request a from_cache attr to let people use it
-        resp.from_cache = from_cache
+        resp.from_cache = from_cache  # type: ignore[attr-defined]
 
         return resp
 
-    def close(self):
+    def close(self) -> None:
         self.cache.close()
         super().close()
```

### Comparing `cacheyou-23.0/cacheyou/cache.py` & `cacheyou-23.1/cacheyou/cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,44 +2,50 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
 The cache object API for implementing caches. The default is a thread
 safe in-memory dictionary.
 """
+from __future__ import annotations
+
+import typing as t
 from threading import Lock
 
+if t.TYPE_CHECKING:
+    from datetime import datetime
+
 
 class BaseCache:
-    def get(self, key):
+    def get(self, key: str) -> bytes | None:
         raise NotImplementedError()
 
-    def set(self, key, value, expires=None):
+    def set(self, key: str, value: bytes, expires: int | datetime | None = None) -> None:
         raise NotImplementedError()
 
-    def delete(self, key):
+    def delete(self, key: str) -> None:
         raise NotImplementedError()
 
-    def close(self):
+    def close(self) -> None:
         pass
 
 
 class DictCache(BaseCache):
-    def __init__(self, init_dict=None):
+    def __init__(self, init_dict: dict[str, bytes] | None = None) -> None:
         self.lock = Lock()
         self.data = init_dict or {}
 
-    def get(self, key):
-        return self.data.get(key, None)
+    def get(self, key: str) -> bytes | None:
+        return self.data.get(key)
 
-    def set(self, key, value, expires=None):
+    def set(self, key: str, value: bytes, expires: int | datetime | None = None) -> None:
         with self.lock:
             self.data.update({key: value})
 
-    def delete(self, key):
+    def delete(self, key: str) -> None:
         with self.lock:
             if key in self.data:
                 self.data.pop(key)
 
 
 class SeparateBodyBaseCache(BaseCache):
     """
@@ -50,15 +56,15 @@
 
         cache.set(key, serialized_metadata)
         cache.set_body(key)
 
     Similarly, the body should be loaded separately via ``get_body()``.
     """
 
-    def set_body(self, key, body):
+    def set_body(self, key: str, body: bytes) -> None:
         raise NotImplementedError()
 
-    def get_body(self, key):
+    def get_body(self, key: str) -> t.IO[bytes] | None:
         """
         Return the body as file-like object.
         """
         raise NotImplementedError()
```

### Comparing `cacheyou-23.0/cacheyou/controller.py` & `cacheyou-23.1/cacheyou/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,69 @@
 # SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
 The httplib2 algorithms ported for use with requests.
 """
+from __future__ import annotations
+
 import calendar
 import logging
 import re
 import time
+import typing as t
 from email.utils import parsedate_tz
 
 from requests.structures import CaseInsensitiveDict
 
 from cacheyou.cache import DictCache, SeparateBodyBaseCache
 from cacheyou.serialize import Serializer
 
+if t.TYPE_CHECKING:
+    from datetime import datetime
+
+    from requests import PreparedRequest
+    from urllib3.response import HTTPResponse
+
+    from cacheyou.cache import BaseCache
+
 logger = logging.getLogger(__name__)
 
 URI = re.compile(r"^(([^:/?#]+):)?(//([^/?#]*))?([^?#]*)(\?([^#]*))?(#(.*))?")
 
 PERMANENT_REDIRECT_STATUSES = (301, 308)
 
 
-def parse_uri(uri):
+def parse_uri(uri: str) -> tuple[str, str, str, str, str]:
     """Parses a URI using the regex given in Appendix B of RFC 3986.
 
     (scheme, authority, path, query, fragment) = parse_uri(uri)
     """
-    groups = URI.match(uri).groups()
+    groups = URI.match(uri).groups()  # type: ignore[union-attr]
     return (groups[1], groups[3], groups[4], groups[6], groups[8])
 
 
 class CacheController:
     """An interface to see if request should cached or not."""
 
     def __init__(
-        self, cache=None, cache_etags=True, serializer=None, status_codes=None
+        self,
+        cache: BaseCache | None = None,
+        cache_etags: bool = True,
+        serializer: Serializer | None = None,
+        status_codes: t.Collection[int] | None = None,
     ):
         self.cache = DictCache() if cache is None else cache
         self.cache_etags = cache_etags
         self.serializer = serializer or Serializer()
         self.cacheable_status_codes = status_codes or (200, 203, 300, 301, 308)
 
     @classmethod
-    def _urlnorm(cls, uri):
+    def _urlnorm(cls, uri: str) -> str:
         """Normalize the URL to create a safe key for the cache"""
         (scheme, authority, path, query, fragment) = parse_uri(uri)
         if not scheme or not authority:
             raise Exception("Only absolute URIs are allowed. uri = %s" % uri)
 
         scheme = scheme.lower()
         authority = authority.lower()
@@ -60,18 +75,18 @@
         # computing the digest. See Section 6.2.2 of Std 66.
         request_uri = query and "?".join([path, query]) or path
         defrag_uri = scheme + "://" + authority + request_uri
 
         return defrag_uri
 
     @classmethod
-    def cache_url(cls, uri):
+    def cache_url(cls, uri: str) -> str:
         return cls._urlnorm(uri)
 
-    def parse_cache_control(self, headers):
+    def parse_cache_control(self, headers: t.Mapping[str, str]) -> dict[str, t.Any]:
         known_directives = {
             # https://tools.ietf.org/html/rfc7234#section-5.2
             "max-age": (int, True),
             "max-stale": (int, False),
             "min-fresh": (int, True),
             "no-cache": (None, False),
             "no-store": (None, False),
@@ -82,15 +97,15 @@
             "private": (None, False),
             "proxy-revalidate": (None, False),
             "s-maxage": (int, True),
         }
 
         cc_headers = headers.get("cache-control", headers.get("Cache-Control", ""))
 
-        retval = {}
+        retval: dict[str, t.Any] = {}
 
         for cc_directive in cc_headers.split(","):
             if not cc_directive.strip():
                 continue
 
             parts = cc_directive.split("=", 1)
             directive = parts[0].strip()
@@ -117,19 +132,20 @@
                         "Invalid value for cache-control directive " "%s, must be %s",
                         directive,
                         typ.__name__,
                     )
 
         return retval
 
-    def _load_from_cache(self, request):
+    def _load_from_cache(self, request: PreparedRequest) -> HTTPResponse | None:
         """
         Load a cached response, or return None if it's not available.
         """
         cache_url = request.url
+        assert cache_url is not None
         cache_data = self.cache.get(cache_url)
         if cache_data is None:
             logger.debug("No cache entry available")
             return None
 
         if isinstance(self.cache, SeparateBodyBaseCache):
             body_file = self.cache.get_body(cache_url)
@@ -137,20 +153,20 @@
             body_file = None
 
         result = self.serializer.loads(request, cache_data, body_file)
         if result is None:
             logger.warning("Cache entry deserialization failed, entry ignored")
         return result
 
-    def cached_request(self, request):
+    def cached_request(self, request: PreparedRequest) -> HTTPResponse | t.Literal[False]:
         """
         Return a cached response if it exists in the cache, otherwise
         return False.
         """
-        cache_url = self.cache_url(request.url)
+        cache_url = self.cache_url(t.cast(str, request.url))
         logger.debug('Looking up "%s" in the cache', cache_url)
         cc = self.parse_cache_control(request.headers)
 
         # Bail out if the request insists on fresh data
         if "no-cache" in cc:
             logger.debug('Request header has "no-cache", cache bypassed')
             return False
@@ -188,15 +204,15 @@
                 # and should be deleted.
                 logger.debug("Purging cached response: no date or etag")
                 self.cache.delete(cache_url)
             logger.debug("Ignoring cached response: no date")
             return False
 
         now = time.time()
-        date = calendar.timegm(parsedate_tz(headers["date"]))
+        date = calendar.timegm(parsedate_tz(headers["date"]))  # type: ignore[arg-type]
         current_age = max(0, now - date)
         logger.debug("Current age based on date: %i", current_age)
 
         # TODO: There is an assumption that the result will be a
         #       urllib3 response object. This may not be best since we
         #       could probably avoid instantiating or constructing the
         #       response until we know we need it.
@@ -210,25 +226,23 @@
             freshness_lifetime = resp_cc["max-age"]
             logger.debug("Freshness lifetime from max-age: %i", freshness_lifetime)
 
         # If there isn't a max-age, check for an expires header
         elif "expires" in headers:
             expires = parsedate_tz(headers["expires"])
             if expires is not None:
-                expire_time = calendar.timegm(expires) - date
+                expire_time = calendar.timegm(expires) - date  # type: ignore[arg-type]
                 freshness_lifetime = max(0, expire_time)
                 logger.debug("Freshness lifetime from expires: %i", freshness_lifetime)
 
         # Determine if we are setting freshness limit in the
         # request. Note, this overrides what was in the response.
         if "max-age" in cc:
             freshness_lifetime = cc["max-age"]
-            logger.debug(
-                "Freshness lifetime from request max-age: %i", freshness_lifetime
-            )
+            logger.debug("Freshness lifetime from request max-age: %i", freshness_lifetime)
 
         if "min-fresh" in cc:
             min_fresh = cc["min-fresh"]
             # adjust our current age by our min fresh
             current_age += min_fresh
             logger.debug("Adjusted current age from min-fresh: %i", current_age)
 
@@ -242,30 +256,37 @@
         if "etag" not in headers:
             logger.debug('The cached response is "stale" with no etag, purging')
             self.cache.delete(cache_url)
 
         # return the original handler
         return False
 
-    def conditional_headers(self, request):
+    def conditional_headers(self, request: PreparedRequest) -> dict[str, str]:
         resp = self._load_from_cache(request)
         new_headers = {}
 
         if resp:
             headers = CaseInsensitiveDict(resp.headers)
 
             if "etag" in headers:
                 new_headers["If-None-Match"] = headers["ETag"]
 
             if "last-modified" in headers:
                 new_headers["If-Modified-Since"] = headers["Last-Modified"]
 
         return new_headers
 
-    def _cache_set(self, cache_url, request, response, body=None, expires_time=None):
+    def _cache_set(
+        self,
+        cache_url: str,
+        request: PreparedRequest,
+        response: HTTPResponse,
+        body: bytes | None = None,
+        expires_time: int | datetime | None = None,
+    ) -> None:
         """
         Store the data in the cache.
         """
         if isinstance(self.cache, SeparateBodyBaseCache):
             # We pass in the body separately; just put a placeholder empty
             # string in the metadata.
             self.cache.set(
@@ -280,33 +301,37 @@
         else:
             self.cache.set(
                 cache_url,
                 self.serializer.dumps(request, response, body),
                 expires=expires_time,
             )
 
-    def cache_response(self, request, response, body=None, status_codes=None):
+    def cache_response(
+        self,
+        request: PreparedRequest,
+        response: HTTPResponse,
+        body: bytes | None = None,
+        status_codes: t.Collection[int] | None = None,
+    ) -> None:
         """
         Algorithm for caching requests.
 
         This assumes a requests Response object.
         """
         # From httplib2: Don't cache 206's since we aren't going to
         #                handle byte range requests
         cacheable_status_codes = status_codes or self.cacheable_status_codes
         if response.status not in cacheable_status_codes:
-            logger.debug(
-                "Status code %s not in %s", response.status, cacheable_status_codes
-            )
+            logger.debug("Status code %s not in %s", response.status, cacheable_status_codes)
             return
 
         response_headers = CaseInsensitiveDict(response.headers)
 
         if "date" in response_headers:
-            date = calendar.timegm(parsedate_tz(response_headers["date"]))
+            date = calendar.timegm(parsedate_tz(response_headers["date"]))  # type: ignore[arg-type]
         else:
             date = 0
 
         # If we've been given a body, our response has a Content-Length, that
         # Content-Length is valid then we can check to see if the body we've
         # been given matches the expected size, and if it doesn't we'll just
         # skip trying to cache it.
@@ -317,15 +342,15 @@
             and int(response_headers["content-length"]) != len(body)
         ):
             return
 
         cc_req = self.parse_cache_control(request.headers)
         cc = self.parse_cache_control(response_headers)
 
-        cache_url = self.cache_url(request.url)
+        cache_url = self.cache_url(t.cast(str, request.url))
         logger.debug('Updating cache with response from "%s"', cache_url)
 
         # Delete it from the cache if we happen to have it stored there
         no_store = False
         if "no-store" in cc:
             no_store = True
             logger.debug('Response header has "no-store"')
@@ -349,15 +374,15 @@
 
         # If we've been given an etag, then keep the response
         if self.cache_etags and "etag" in response_headers:
             expires_time = 0
             if response_headers.get("expires"):
                 expires = parsedate_tz(response_headers["expires"])
                 if expires is not None:
-                    expires_time = calendar.timegm(expires) - date
+                    expires_time = calendar.timegm(expires) - date  # type: ignore[arg-type]
 
             expires_time = max(expires_time, 14 * 86400)
 
             logger.debug(f"etag object cached for {expires_time} seconds")
             logger.debug("Caching due to etag")
             self._cache_set(cache_url, request, response, body, expires_time)
 
@@ -367,15 +392,15 @@
             logger.debug("Caching permanent redirect")
             self._cache_set(cache_url, request, response, b"")
 
         # Add to the cache if the response headers demand it. If there
         # is no date header then we can't do anything about expiring
         # the cache.
         elif "date" in response_headers:
-            date = calendar.timegm(parsedate_tz(response_headers["date"]))
+            date = calendar.timegm(parsedate_tz(response_headers["date"]))  # type: ignore[arg-type]
             # cache when there is a max-age > 0
             if "max-age" in cc and cc["max-age"] > 0:
                 logger.debug("Caching b/c date exists and max-age > 0")
                 expires_time = cc["max-age"]
                 self._cache_set(
                     cache_url,
                     request,
@@ -386,39 +411,39 @@
 
             # If the request can expire, it means we should cache it
             # in the meantime.
             elif "expires" in response_headers:
                 if response_headers["expires"]:
                     expires = parsedate_tz(response_headers["expires"])
                     if expires is not None:
-                        expires_time = calendar.timegm(expires) - date
+                        expires_time = calendar.timegm(expires) - date  # type: ignore[arg-type]
                     else:
                         expires_time = None
 
                     logger.debug(
-                        "Caching b/c of expires header. expires in {} seconds".format(
-                            expires_time
-                        )
+                        "Caching b/c of expires header. expires in %s seconds", expires_time
                     )
                     self._cache_set(
                         cache_url,
                         request,
                         response,
                         body,
                         expires_time,
                     )
 
-    def update_cached_response(self, request, response):
+    def update_cached_response(
+        self, request: PreparedRequest, response: HTTPResponse
+    ) -> HTTPResponse:
         """On a 304 we will get a new set of headers that we want to
         update our cached value with, assuming we have one.
 
         This should only ever be called when we've sent an ETag and
         gotten a 304 as the response.
         """
-        cache_url = self.cache_url(request.url)
+        cache_url = self.cache_url(t.cast(str, request.url))
         cached_response = self._load_from_cache(request)
 
         if not cached_response:
             # we didn't have a cached response
             return response
 
         # Lets update our headers with the headers from the new request:
@@ -427,19 +452,15 @@
         # The server isn't supposed to send headers that would make
         # the cached body invalid. But... just in case, we'll be sure
         # to strip out ones we know that might be problmatic due to
         # typical assumptions.
         excluded_headers = ["content-length"]
 
         cached_response.headers.update(
-            {
-                k: v
-                for k, v in response.headers.items()
-                if k.lower() not in excluded_headers
-            }
+            {k: v for k, v in response.headers.items() if k.lower() not in excluded_headers}
         )
 
         # we want a 200 b/c we have content via the cache
         cached_response.status = 200
 
         # update our cache
         self._cache_set(cache_url, request, cached_response)
```

### Comparing `cacheyou-23.0/cacheyou/filewrapper.py` & `cacheyou-23.1/cacheyou/filewrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
 import mmap
+import typing as t
 from tempfile import NamedTemporaryFile
 
+if t.TYPE_CHECKING:
+    from http.client import HTTPResponse as HttplibResponse
+
 
 class CallbackFileWrapper:
     """
     Small wrapper around a fp object which will tee everything read into a
     buffer, and when that file is closed it will execute a callback with the
     contents of that buffer.
 
@@ -21,32 +26,32 @@
     as the temporary files directory is disk-based (sometimes it's a
     memory-backed-``tmpfs`` on Linux), data will be unloaded to disk if memory
     pressure is high.  For small files the disk usually won't be used at all,
     it'll all be in the filesystem memory cache, so there should be no
     performance impact.
     """
 
-    def __init__(self, fp, callback):
+    def __init__(self, fp: HttplibResponse, callback: t.Callable[[bytes], None] | None) -> None:
         self.__buf = NamedTemporaryFile("rb+", delete=True)
         self.__fp = fp
         self.__callback = callback
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> t.Any:
         # The vaguaries of garbage collection means that self.__fp is
         # not always set.  By using __getattribute__ and the private
         # name[0] allows looking up the attribute value and raising an
         # AttributeError when it doesn't exist. This stop thigns from
         # infinitely recursing calls to getattr in the case where
         # self.__fp hasn't been set.
         #
         # [0] https://docs.python.org/2/reference/expressions.html#atom-identifiers
         fp = self.__getattribute__("_CallbackFileWrapper__fp")
         return getattr(fp, name)
 
-    def __is_fp_closed(self):
+    def __is_fp_closed(self) -> bool:
         try:
             return self.__fp.fp is None
 
         except AttributeError:
             pass
 
         try:
@@ -55,54 +60,52 @@
         except AttributeError:
             pass
 
         # We just don't cache it then.
         # TODO: Add some logging here...
         return False
 
-    def _close(self):
+    def _close(self) -> None:
         if self.__callback:
             if self.__buf.tell() == 0:
                 # Empty file:
                 result = b""
             else:
                 # Return the data without actually loading it into memory,
                 # relying on Python's buffer API and mmap(). mmap() just gives
                 # a view directly into the filesystem's memory cache, so it
                 # doesn't result in duplicate memory use.
                 self.__buf.seek(0, 0)
-                result = memoryview(
-                    mmap.mmap(self.__buf.fileno(), 0, access=mmap.ACCESS_READ)
-                )
+                result = memoryview(mmap.mmap(self.__buf.fileno(), 0, access=mmap.ACCESS_READ))
             self.__callback(result)
 
         # We assign this to None here, because otherwise we can get into
         # really tricky problems where the CPython interpreter dead locks
         # because the callback is holding a reference to something which
         # has a __del__ method. Setting this to None breaks the cycle
         # and allows the garbage collector to do it's thing normally.
         self.__callback = None
 
         # Closing the temporary file releases memory and frees disk space.
         # Important when caching big files.
         self.__buf.close()
 
-    def read(self, amt=None):
+    def read(self, amt: int | None = None) -> bytes:
         data = self.__fp.read(amt)
         if data:
             # We may be dealing with b'', a sign that things are over:
             # it's passed e.g. after we've already closed self.__buf.
             self.__buf.write(data)
         if self.__is_fp_closed():
             self._close()
 
         return data
 
-    def _safe_read(self, amt):
-        data = self.__fp._safe_read(amt)
+    def _safe_read(self, amt: int) -> bytes:
+        data = self.__fp._safe_read(amt)  # type: ignore[attr-defined]
         if amt == 2 and data == b"\r\n":
             # urllib executes this read to toss the CRLF at the end
             # of the chunk.
             return data
 
         self.__buf.write(data)
         if self.__is_fp_closed():
```

### Comparing `cacheyou-23.0/cacheyou/heuristics.py` & `cacheyou-23.1/cacheyou/heuristics.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 # SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
+from __future__ import annotations
+
 import calendar
 import time
+import typing as t
 from datetime import datetime, timedelta, timezone
 from email.utils import formatdate, parsedate, parsedate_tz
 
+if t.TYPE_CHECKING:
+    from urllib3.response import HTTPResponse
 TIME_FMT = "%a, %d %b %Y %H:%M:%S GMT"
 
 
-def expire_after(delta, date=None):
+def expire_after(delta: timedelta, date: datetime | None = None) -> datetime:
     date = date or datetime.now(timezone.utc)
     return date + delta
 
 
-def datetime_to_header(dt):
+def datetime_to_header(dt: datetime) -> str:
     return formatdate(calendar.timegm(dt.timetuple()))
 
 
 class BaseHeuristic:
-    def warning(self, response):
+    def warning(self, response: HTTPResponse) -> str | None:
         """
         Return a valid 1xx warning header value describing the cache
         adjustments.
 
         The response is provided too allow warnings like 113
         http://tools.ietf.org/html/rfc7234#section-5.5.4 where we need
         to explicitly say response is over 24 hours old.
         """
         return '110 - "Response is Stale"'
 
-    def update_headers(self, response):
+    def update_headers(self, response: HTTPResponse) -> dict[str, str]:
         """Update the response headers with any new headers.
 
         NOTE: This SHOULD always include some Warning header to
               signify that the response was cached by the client, not
               by way of the provided headers.
         """
         return {}
 
-    def apply(self, response):
+    def apply(self, response: HTTPResponse) -> HTTPResponse:
         updated_headers = self.update_headers(response)
 
         if updated_headers:
             response.headers.update(updated_headers)
             warning_header_value = self.warning(response)
             if warning_header_value is not None:
                 response.headers.update({"Warning": warning_header_value})
@@ -54,40 +59,42 @@
 
 class OneDayCache(BaseHeuristic):
     """
     Cache the response by providing an expires 1 day in the
     future.
     """
 
-    def update_headers(self, response):
+    def update_headers(self, response: HTTPResponse) -> dict[str, str]:
         headers = {}
 
         if "expires" not in response.headers:
             date = parsedate(response.headers["date"])
-            expires = expire_after(timedelta(days=1), date=datetime(*date[:6], tzinfo=timezone.utc))
+            expires = expire_after(
+                timedelta(days=1),
+                date=datetime(*date[:6], tzinfo=timezone.utc),  # type: ignore[misc]
+            )
             headers["expires"] = datetime_to_header(expires)
             headers["cache-control"] = "public"
         return headers
 
 
 class ExpiresAfter(BaseHeuristic):
     """
     Cache **all** requests for a defined time period.
     """
 
-    def __init__(self, **kw):
+    def __init__(self, **kw: float) -> None:
         self.delta = timedelta(**kw)
 
-    def update_headers(self, response):
+    def update_headers(self, response: HTTPResponse) -> dict[str, str]:
         expires = expire_after(self.delta)
         return {"expires": datetime_to_header(expires), "cache-control": "public"}
 
-    def warning(self, response):
-        tmpl = "110 - Automatically cached for %s. Response might be stale"
-        return tmpl % self.delta
+    def warning(self, response: HTTPResponse) -> str | None:
+        return f"110 - Automatically cached for {self.delta}. Response might be stale"
 
 
 class LastModified(BaseHeuristic):
     """
     If there is no Expires header already, fall back on Last-Modified
     using the heuristic from
     http://tools.ietf.org/html/rfc7234#section-4.2.2
@@ -109,39 +116,39 @@
         404,
         405,
         410,
         414,
         501,
     }
 
-    def update_headers(self, resp):
-        headers = resp.headers
+    def update_headers(self, response: HTTPResponse) -> dict[str, str]:
+        headers = response.headers
 
         if "expires" in headers:
             return {}
 
         if "cache-control" in headers and headers["cache-control"] != "public":
             return {}
 
-        if resp.status not in self.cacheable_by_default_statuses:
+        if response.status not in self.cacheable_by_default_statuses:
             return {}
 
         if "date" not in headers or "last-modified" not in headers:
             return {}
 
-        date = calendar.timegm(parsedate_tz(headers["date"]))
+        date = calendar.timegm(parsedate_tz(headers["date"]))  # type: ignore[arg-type]
         last_modified = parsedate(headers["last-modified"])
         if date is None or last_modified is None:
             return {}
 
         now = time.time()
         current_age = max(0, now - date)
         delta = date - calendar.timegm(last_modified)
         freshness_lifetime = max(0, min(delta / 10, 24 * 3600))
         if freshness_lifetime <= current_age:
             return {}
 
         expires = date + freshness_lifetime
         return {"expires": time.strftime(TIME_FMT, time.gmtime(expires))}
 
-    def warning(self, resp):
+    def warning(self, response: HTTPResponse) -> str | None:
         return None
```

### Comparing `cacheyou-23.0/cacheyou/serialize.py` & `cacheyou-23.1/cacheyou/serialize.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 # SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
+from __future__ import annotations
+
 import base64
 import io
 import json
 import pickle
+import typing as t
 import zlib
 
 import msgpack
 from requests.structures import CaseInsensitiveDict
 from urllib3 import HTTPResponse
 
+if t.TYPE_CHECKING:
+    from requests import PreparedRequest
+
 
-def _b64_decode_bytes(b):
+def _b64_decode_bytes(b: str) -> bytes:
     return base64.b64decode(b.encode("ascii"))
 
 
-def _b64_decode_str(s):
+def _b64_decode_str(s: str) -> str:
     return _b64_decode_bytes(s).decode("utf8")
 
 
 _default_body_read = object()
 
 
 class Serializer:
-    def dumps(self, request, response, body=None):
+    def dumps(
+        self, request: PreparedRequest, response: HTTPResponse, body: bytes | None = None
+    ) -> bytes:
         response_headers = CaseInsensitiveDict(response.headers)
 
         if body is None:
             # When a body isn't passed in, we'll read the response. We
             # also update the response with a new file handler to be
             # sure it acts as though it was never read.
             body = response.read(decode_content=False)
-            response._fp = io.BytesIO(body)
+            response._fp = io.BytesIO(body)  # type: ignore[attr-defined]
             response.length_remaining = len(body)
 
         data = {
             "response": {
                 "body": body,  # Empty bytestring if body is stored separately
                 "headers": {str(k): str(v) for k, v in response.headers.items()},
                 "status": response.status,
@@ -56,18 +64,20 @@
                 header_value = request.headers.get(header, None)
                 if header_value is not None:
                     header_value = str(header_value)
                 data["vary"][header] = header_value
 
         return b",".join([b"cc=4", msgpack.dumps(data, use_bin_type=True)])
 
-    def loads(self, request, data, body_file=None):
+    def loads(
+        self, request: PreparedRequest, data: bytes, body_file: t.IO[bytes] | None = None
+    ) -> HTTPResponse | None:
         # Short circuit if we've been given an empty set of data
         if not data:
-            return
+            return None
 
         # Determine what version of the serializer the data was serialized
         # with
         try:
             ver, data = data.split(b",", 1)
         except ValueError:
             ver = b"cc=0"
@@ -75,106 +85,118 @@
         # Make sure that our "ver" is actually a version and isn't a false
         # positive from a , being in the data stream.
         if ver[:3] != b"cc=":
             data = ver + data
             ver = b"cc=0"
 
         # Get the version number out of the cc=N
-        ver = ver.split(b"=", 1)[-1].decode("ascii")
+        ver_str = ver.split(b"=", 1)[-1].decode("ascii")
 
         # Dispatch to the actual load method for the given version
         try:
-            return getattr(self, f"_loads_v{ver}")(request, data, body_file)
+            return getattr(self, f"_loads_v{ver_str}")(request, data, body_file)
 
         except AttributeError:
             # This is a version we don't have a loads function for, so we'll
             # just treat it as a miss and return None
-            return
+            return None
 
-    def prepare_response(self, request, cached, body_file=None):
+    def prepare_response(
+        self, request: PreparedRequest, cached: dict, body_file: t.IO[bytes] | None = None
+    ) -> HTTPResponse | None:
         """Verify our vary headers match and construct a real urllib3
         HTTPResponse object.
         """
         # Special case the '*' Vary value as it means we cannot actually
         # determine if the cached response is suitable for this request.
         # This case is also handled in the controller code when creating
         # a cache entry, but is left here for backwards compatibility.
         if "*" in cached.get("vary", {}):
-            return
+            return None
 
         # Ensure that the Vary headers for the cached response match our
         # request
         for header, value in cached.get("vary", {}).items():
             if request.headers.get(header, None) != value:
-                return
+                return None
 
         body_raw = cached["response"].pop("body")
 
-        headers = CaseInsensitiveDict(data=cached["response"]["headers"])
+        headers: t.MutableMapping[str, str] = CaseInsensitiveDict(
+            data=cached["response"]["headers"]
+        )
         if headers.get("transfer-encoding", "") == "chunked":
             headers.pop("transfer-encoding")
 
         cached["response"]["headers"] = headers
 
         try:
             if body_file is None:
-                body = io.BytesIO(body_raw)
-            else:
-                body = body_file
+                body_file = io.BytesIO(body_raw)
         except TypeError:
             # This can happen if cachecontrol serialized to v1 format (pickle)
             # using Python 2. A Python 2 str(byte string) will be unpickled as
             # a Python 3 str (unicode string), which will cause the above to
             # fail with:
             #
             #     TypeError: 'str' does not support the buffer interface
-            body = io.BytesIO(body_raw.encode("utf8"))
+            body_file = io.BytesIO(body_raw.encode("utf8"))
 
-        return HTTPResponse(body=body, preload_content=False, **cached["response"])
+        return HTTPResponse(body=body_file, preload_content=False, **cached["response"])
 
-    def _loads_v0(self, request, data, body_file=None):
+    def _loads_v0(
+        self, request: PreparedRequest, data: bytes, body_file: t.IO[bytes] | None = None
+    ) -> HTTPResponse | None:
         # The original legacy cache data. This doesn't contain enough
         # information to construct everything we need, so we'll treat this as
         # a miss.
-        return
+        return None
 
-    def _loads_v1(self, request, data, body_file=None):
+    def _loads_v1(
+        self, request: PreparedRequest, data: bytes, body_file: t.IO[bytes] | None = None
+    ) -> HTTPResponse | None:
         try:
             cached = pickle.loads(data)
         except ValueError:
-            return
+            return None
 
         return self.prepare_response(request, cached, body_file)
 
-    def _loads_v2(self, request, data, body_file=None):
+    def _loads_v2(
+        self, request: PreparedRequest, data: bytes, body_file: t.IO[bytes] | None = None
+    ) -> HTTPResponse | None:
         assert body_file is None
         try:
             cached = json.loads(zlib.decompress(data).decode("utf8"))
         except (ValueError, zlib.error):
-            return
+            return None
 
         # We need to decode the items that we've base64 encoded
         cached["response"]["body"] = _b64_decode_bytes(cached["response"]["body"])
         cached["response"]["headers"] = {
             _b64_decode_str(k): _b64_decode_str(v) for k, v in cached["response"]["headers"].items()
         }
         cached["response"]["reason"] = _b64_decode_str(cached["response"]["reason"])
         cached["vary"] = {
             _b64_decode_str(k): _b64_decode_str(v) if v is not None else v
             for k, v in cached["vary"].items()
         }
 
         return self.prepare_response(request, cached, body_file)
 
-    def _loads_v3(self, request, data, body_file):
+    def _loads_v3(
+        self, request: PreparedRequest, data: bytes, body_file: t.IO[bytes] | None = None
+    ) -> HTTPResponse | None:
         # Due to Python 2 encoding issues, it's impossible to know for sure
         # exactly how to load v3 entries, thus we'll treat these as a miss so
         # that they get rewritten out as v4 entries.
-        return
+        return None
 
-    def _loads_v4(self, request, data, body_file=None):
+    def _loads_v4(
+        self, request: PreparedRequest, data: bytes, body_file: t.IO[bytes] | None = None
+    ) -> HTTPResponse | None:
         try:
             cached = msgpack.loads(data, raw=False)
         except ValueError:
-            return
+            return None
 
         return self.prepare_response(request, cached, body_file)
```

### Comparing `cacheyou-23.0/docs/Makefile` & `cacheyou-23.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/docs/conf.py` & `cacheyou-23.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
+from __future__ import annotations
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = ["sphinx.ext.autodoc", "sphinx.ext.todo", "sphinx.ext.viewcode"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
@@ -47,15 +48,15 @@
 copyright = "2013, Eric Larson, 2023 Frost Ming"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = "23.0"
+release = "23.1"
 # The short X.Y version.
 version = release
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
@@ -168,15 +169,15 @@
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "CacheYoudoc"
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
-latex_elements = {
+latex_elements: dict[str, str] = {
     # The paper size ('letterpaper' or 'a4paper').
     # 'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
     # 'pointsize': '10pt',
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
 }
```

### Comparing `cacheyou-23.0/docs/custom_heuristics.rst` & `cacheyou-23.1/docs/custom_heuristics.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/docs/etags.rst` & `cacheyou-23.1/docs/etags.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/docs/index.rst` & `cacheyou-23.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/docs/release_notes.rst` & `cacheyou-23.1/docs/release_notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,21 @@
 
   SPDX-License-Identifier: Apache-2.0
 
 ===============
  Release Notes
 ===============
 
+23.1
+====
+
+* Add type hints to the code base.
+
 23.0
-======
+====
 
 The first release of ``CacheYou``.
 
 * Replace the usages of deprecated ``datetime.utcnow()``.
 * Fix the compatibility with ``urllib3`` 2.0.
 * Drop the support for Python prior to 3.7.
 * Switch to PDM as the project manager.
```

### Comparing `cacheyou-23.0/docs/requirements.txt` & `cacheyou-23.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/docs/storage.rst` & `cacheyou-23.1/docs/storage.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/docs/tips.rst` & `cacheyou-23.1/docs/tips.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/docs/usage.rst` & `cacheyou-23.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/pyproject.toml` & `cacheyou-23.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "CacheYou"
-version = "23.0"
+version = "23.1"
 description = "httplib2 caching for requests"
 keywords = [
     "requests",
     "http",
     "caching",
     "web",
 ]
@@ -28,26 +28,28 @@
 requires-python = ">=3.7"
 dependencies = [
     "msgpack>=0.5.2",
     "requests",
 ]
 
 [project.urls]
-Homepage = "https://github.com/ionrock/cachecontrol"
+Homepage = "https://github.com/frostming/cacheyou"
+Documentation = "https://cacheyou.readthedocs.io"
+"Release Notes" = "https://cacheyou.readthedocs.io/en/latest/release_notes.html"
 
 [project.optional-dependencies]
 filecache = [
     "filelock>=3.8.0",
 ]
 redis = [
     "redis>=2.10.5",
 ]
 
 [project.scripts]
-doesitcache = "cachecontrol._cmd:main"
+doesitcache = "cacheyou._cmd:main"
 
 [tool.pdm]
 plugins = [
     "pdm-autoexport",
 ]
 
 [tool.pdm.build]
@@ -121,15 +123,15 @@
 
 [tool.ruff.isort]
 known-first-party = [
     "cacheyou",
 ]
 
 [tool.bumpver]
-current_version = "23.0"
+current_version = "23.1"
 version_pattern = "YY.INC0[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `cacheyou-23.0/tests/conftest.py` & `cacheyou-23.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/tests/issue_263.py` & `cacheyou-23.1/tests/issue_263.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     return
 
     print(f"{resp.status_code} {resp.request.method}")
     for k, v in response.headers.items():
         print(f"{k}: {v}")
 
 
-for i in range(2):
-    response = session.get(
-        "https://api.github.com/repos/sigmavirus24/github3.py/pulls/1033"
-    )
+for _ in range(2):
+    response = session.get("https://api.github.com/repos/sigmavirus24/github3.py/pulls/1033")
     log_resp(response)
     print(f"Content length: {len(response.content)}")
-    print(response.from_cache)
+    print(response.from_cache)  # type: ignore[attr-defined]
     if len(response.content) == 0:
         sys.exit(1)
```

### Comparing `cacheyou-23.0/tests/test_adapter.py` & `cacheyou-23.1/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/tests/test_cache_control.py` & `cacheyou-23.1/tests/test_cache_control.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/tests/test_chunked_response.py` & `cacheyou-23.1/tests/test_chunked_response.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/tests/test_etag.py` & `cacheyou-23.1/tests/test_etag.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/tests/test_expires_heuristics.py` & `cacheyou-23.1/tests/test_expires_heuristics.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/tests/test_max_age.py` & `cacheyou-23.1/tests/test_max_age.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 
 class TestMaxAge:
     @pytest.fixture()
     def sess(self, url):
         self.url = url
         self.cache = DictCache()
         sess = Session()
-        sess.mount(
-            "http://", CacheControlAdapter(self.cache, serializer=NullSerializer())
-        )
+        sess.mount("http://", CacheControlAdapter(self.cache, serializer=NullSerializer()))
         return sess
 
     def test_client_max_age_0(self, sess):
         """
         Making sure when the client uses max-age=0 we don't get a
         cached copy even though we're still fresh.
         """
```

### Comparing `cacheyou-23.0/tests/test_redirects.py` & `cacheyou-23.1/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/tests/test_regressions.py` & `cacheyou-23.1/tests/test_regressions.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
 from cacheyou import CacheControl
 from cacheyou.caches import FileCache
 from cacheyou.filewrapper import CallbackFileWrapper
 
 
 class Test39:
-    @pytest.mark.skipif(
-        sys.version.startswith("2"), reason="Only run this for python 3.x"
-    )
+    @pytest.mark.skipif(sys.version.startswith("2"), reason="Only run this for python 3.x")
     def test_file_cache_recognizes_consumed_file_handle(self, url):
         s = CacheControl(Session(), FileCache("web_cache"))
         the_url = url + "cache_60"
         s.get(the_url)
         r = s.get(the_url)
         assert r.from_cache
         s.close()
```

### Comparing `cacheyou-23.0/tests/test_serialization.py` & `cacheyou-23.1/tests/test_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,22 @@
         req = Mock()
         resp = self.serializer._loads_v1(req, pickle.dumps(self.response_data))
         # We have to decode our urllib3 data back into a unicode string.
         assert resp.data == b"Hello World"
 
     def test_read_version_v2(self):
         req = Mock()
-        compressed_base64_json = b'x\x9c\x1d\x8fK\x0f\x820\x10\x84\xff\xcb\x9e9h\xe3A\x9ax\xf0\x11K8hPi\xb8\x99>6\n!\xd4\xd0\x02!\x84\xff\xee\xc2qg\xbe\x9d\x9d\x9d\xa0E\xffs\x8dG\xe0\x13hgG\xe0\xf0\x14\xd2k\xb1\xffH\x16\x8fZd\x07\x88\xc0\xa2q\x16\xdf\xc65\x01\x9b\x00<\xb4\x1dF\xf0Ee\xb1\xf5\xcbj\xc6\xe2\xce\n\xd9\xd9\xf36\xc7\xe2TS\x0c\x8d;{\x8e\x07-\xae?\xfd9,1\x19\xbbVJ\xe4a\xa5\x93\xb4\xd7G\x929\x98D\x96Z\xd4\x15\x11\x8f\xe2;\xa8"\xad\xcd\xb0:\xf7\x8ba\xb7\x17U\x98#j\xaa\xbckH$\xcc\x07\x15::\xcc6\x9b\x08z\xeaP\xae\x0e[\xb8^\xb5\xf4\xc54\xcf\x7f\xef\xc0E\xe6'
+        compressed_base64_json = (
+            b"x\x9c\x1d\x8fK\x0f\x820\x10\x84\xff\xcb\x9e9h\xe3A\x9ax\xf0\x11K8hPi"
+            b"\xb8\x99>6\n!\xd4\xd0\x02!\x84\xff\xee\xc2qg\xbe\x9d\x9d\x9d\xa0E\xffs\x8dG\xe0\x13hgG"
+            b"\xe0\xf0\x14\xd2k\xb1\xffH\x16\x8fZd\x07\x88\xc0\xa2q\x16\xdf\xc65\x01\x9b\x00<\xb4\x1dF"
+            b"\xf0Ee\xb1\xf5\xcbj\xc6\xe2\xce\n\xd9\xd9\xf36\xc7\xe2TS\x0c\x8d;{\x8e\x07-\xae?\xfd9,1"
+            b'\x19\xbbVJ\xe4a\xa5\x93\xb4\xd7G\x929\x98D\x96Z\xd4\x15\x11\x8f\xe2;\xa8"\xad\xcd\xb0:'
+            b"\xf7\x8ba\xb7\x17U\x98#j\xaa\xbckH$\xcc\x07\x15::\xcc6\x9b\x08z\xeaP\xae\x0e[\xb8^\xb5\xf4\xc54\xcf\x7f\xef\xc0E\xe6"
+        )
         resp = self.serializer._loads_v2(req, compressed_base64_json)
         # We have to decode our urllib3 data back into a unicode string.
         assert resp.data == b"Hello World"
 
     def test_load_by_version_v3(self):
         data = b"cc=3,somedata"
         req = Mock()
```

### Comparing `cacheyou-23.0/tests/test_storage_filecache.py` & `cacheyou-23.1/tests/test_storage_filecache.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 
 class TestFileCache(FileCacheTestsMixin):
     """
     Tests for ``FileCache``.
     """
 
-    FileCacheClass = FileCache
+    FileCacheClass = FileCache  # type: ignore[assignment]
 
     def test_body_stored_inline(self, sess):
         """The body is stored together with the metadata."""
         url = self.url + "cache_60"
         response = sess.get(url)
         body = response.content
         response2 = sess.get(url)
@@ -141,15 +141,15 @@
 
 
 class TestSeparateBodyFileCache(FileCacheTestsMixin):
     """
     Tests for ``SeparateBodyFileCache``
     """
 
-    FileCacheClass = SeparateBodyFileCache
+    FileCacheClass = SeparateBodyFileCache  # type: ignore[assignment]
 
     def test_body_actually_stored_separately(self, sess):
         """
         Body is stored and can be retrieved from the SeparateBodyFileCache, with assurances
         it's actually being loaded from separate file than metadata.
         """
         url = self.url + "cache_60"
```

### Comparing `cacheyou-23.0/tests/test_storage_redis.py` & `cacheyou-23.1/tests/test_storage_redis.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/tests/test_vary.py` & `cacheyou-23.1/tests/test_vary.py`

 * *Files identical despite different names*

### Comparing `cacheyou-23.0/tests/utils.py` & `cacheyou-23.1/tests/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 Shared utility classes.
 """
 
 from requests.structures import CaseInsensitiveDict
 
 
 class NullSerializer:
-
     def dumps(self, request, response, body=None):
         return response
 
     def loads(self, request, data, body_file=None):
         if data and getattr(data, "chunked", False):
             data.chunked = False
         return data
 
 
 class DummyResponse:
     """Match a ``urllib3.response.HTTPResponse``."""
+
     version = "1.1"
     reason = b"Because"
     strict = 0
     decode_content = False
 
     def __init__(self, status, headers):
         self.status = status
```

### Comparing `cacheyou-23.0/PKG-INFO` & `cacheyou-23.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: cacheyou
-Version: 23.0
+Version: 23.1
 Summary: httplib2 caching for requests
 Keywords: requests http caching web
 Author-Email: Frost Ming <me@frostming.com>, Eric Larson <eric@ionrock.org>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Homepage, https://github.com/ionrock/cachecontrol
+Project-URL: Homepage, https://github.com/frostming/cacheyou
+Project-URL: Documentation, https://cacheyou.readthedocs.io
+Project-URL: Release notes, https://cacheyou.readthedocs.io/en/latest/release_notes.html
 Requires-Python: >=3.7
 Requires-Dist: msgpack>=0.5.2
 Requires-Dist: requests
 Requires-Dist: filelock>=3.8.0; extra == "filecache"
 Requires-Dist: redis>=2.10.5; extra == "redis"
 Provides-Extra: filecache
 Provides-Extra: redis
```

