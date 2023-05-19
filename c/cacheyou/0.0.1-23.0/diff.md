# Comparing `tmp/cacheyou-0.0.1.tar.gz` & `tmp/cacheyou-23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacheyou-0.0.1.tar", last modified: Thu May 18 08:11:51 2023, max compression
+gzip compressed data, was "cacheyou-23.0.tar", last modified: Fri May 19 03:37:08 2023, max compression
```

## Comparing `cacheyou-0.0.1.tar` & `cacheyou-23.0.tar`

### file list

```diff
@@ -1,34 +1,44 @@
--rw-r--r--   0        0        0      558 2023-05-04 10:23:41.851113 cacheyou-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      681 2023-05-18 08:10:40.955982 cacheyou-0.0.1/README.md
--rw-r--r--   0        0        0      465 2023-05-04 10:23:41.851391 cacheyou-0.0.1/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1326 2023-05-04 10:23:41.851487 cacheyou-0.0.1/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5021 2023-05-04 10:23:41.851605 cacheyou-0.0.1/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1535 2023-05-04 10:23:41.851688 cacheyou-0.0.1/cachecontrol/cache.py
--rw-r--r--   0        0        0      242 2023-05-04 10:23:41.851805 cacheyou-0.0.1/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     4949 2023-05-04 10:23:41.851917 cacheyou-0.0.1/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1021 2023-05-04 10:23:41.851996 cacheyou-0.0.1/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0      730 2023-05-04 10:23:41.852079 cacheyou-0.0.1/cachecontrol/compat.py
--rw-r--r--   0        0        0    16684 2023-05-04 10:23:41.852229 cacheyou-0.0.1/cachecontrol/controller.py
--rw-r--r--   0        0        0     3946 2023-05-04 10:23:41.852332 cacheyou-0.0.1/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4154 2023-05-04 10:23:41.852427 cacheyou-0.0.1/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7082 2023-05-18 08:10:40.956153 cacheyou-0.0.1/cachecontrol/serialize.py
--rw-r--r--   0        0        0      774 2023-05-04 10:23:41.852623 cacheyou-0.0.1/cachecontrol/wrapper.py
--rw-r--r--   0        0        0     1172 2023-05-18 08:11:51.470991 cacheyou-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       30 2023-05-04 10:23:41.854035 cacheyou-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     4786 2023-05-18 08:10:40.956553 cacheyou-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1142 2023-05-04 10:23:41.854213 cacheyou-0.0.1/tests/issue_263.py
--rw-r--r--   0        0        0     1671 2023-05-04 10:23:41.854303 cacheyou-0.0.1/tests/test_adapter.py
--rw-r--r--   0        0        0    10891 2023-05-18 08:10:40.956893 cacheyou-0.0.1/tests/test_cache_control.py
--rw-r--r--   0        0        0     1522 2023-05-04 10:23:41.854503 cacheyou-0.0.1/tests/test_chunked_response.py
--rw-r--r--   0        0        0     5144 2023-05-18 08:10:40.957131 cacheyou-0.0.1/tests/test_etag.py
--rw-r--r--   0        0        0     6585 2023-05-18 08:10:40.957311 cacheyou-0.0.1/tests/test_expires_heuristics.py
--rw-r--r--   0        0        0     1805 2023-05-04 10:23:41.854784 cacheyou-0.0.1/tests/test_max_age.py
--rw-r--r--   0        0        0     1600 2023-05-18 08:10:40.957462 cacheyou-0.0.1/tests/test_redirects.py
--rw-r--r--   0        0        0      959 2023-05-04 10:23:41.854937 cacheyou-0.0.1/tests/test_regressions.py
--rw-r--r--   0        0        0     5554 2023-05-18 08:10:40.957730 cacheyou-0.0.1/tests/test_serialization.py
--rw-r--r--   0        0        0      242 2023-05-04 10:23:41.855132 cacheyou-0.0.1/tests/test_server_http_version.py
--rw-r--r--   0        0        0     5643 2023-05-04 10:23:41.855245 cacheyou-0.0.1/tests/test_storage_filecache.py
--rw-r--r--   0        0        0      589 2023-05-18 08:10:40.957927 cacheyou-0.0.1/tests/test_storage_redis.py
--rw-r--r--   0        0        0     2964 2023-05-18 08:10:40.958152 cacheyou-0.0.1/tests/test_vary.py
--rw-r--r--   0        0        0      800 2023-05-04 10:23:41.855507 cacheyou-0.0.1/tests/utils.py
--rw-r--r--   0        0        0     1703 1970-01-01 00:00:00.000000 cacheyou-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      575 2023-05-19 03:36:49.481905 cacheyou-23.0/LICENSE.txt
+-rw-r--r--   0        0        0      830 2023-05-19 03:36:49.481905 cacheyou-23.0/README.md
+-rw-r--r--   0        0        0      516 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/__init__.py
+-rw-r--r--   0        0        0     1330 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/_cmd.py
+-rw-r--r--   0        0        0     4963 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/adapter.py
+-rw-r--r--   0        0        0     1543 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/cache.py
+-rw-r--r--   0        0        0      288 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/caches/__init__.py
+-rw-r--r--   0        0        0     4857 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/caches/file_cache.py
+-rw-r--r--   0        0        0     1145 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/caches/redis_cache.py
+-rw-r--r--   0        0        0    16692 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/controller.py
+-rw-r--r--   0        0        0     3955 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/filewrapper.py
+-rw-r--r--   0        0        0     4282 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/heuristics.py
+-rw-r--r--   0        0        0     6453 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/serialize.py
+-rw-r--r--   0        0        0      806 2023-05-19 03:36:49.481905 cacheyou-23.0/cacheyou/wrapper.py
+-rw-r--r--   0        0        0     5673 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/Makefile
+-rw-r--r--   0        0        0     8068 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/conf.py
+-rw-r--r--   0        0        0     5478 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/custom_heuristics.rst
+-rw-r--r--   0        0        0     5209 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/etags.rst
+-rw-r--r--   0        0        0     2289 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/index.rst
+-rw-r--r--   0        0        0     4040 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/release_notes.rst
+-rw-r--r--   0        0        0      643 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/requirements.txt
+-rw-r--r--   0        0        0     4297 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/storage.rst
+-rw-r--r--   0        0        0     2372 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/tips.rst
+-rw-r--r--   0        0        0     1792 2023-05-19 03:36:49.481905 cacheyou-23.0/docs/usage.rst
+-rw-r--r--   0        0        0     2501 2023-05-19 03:37:08.830092 cacheyou-23.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/__init__.py
+-rw-r--r--   0        0        0     4750 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/conftest.py
+-rw-r--r--   0        0        0     1098 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/issue_263.py
+-rw-r--r--   0        0        0     1682 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/test_adapter.py
+-rw-r--r--   0        0        0    10845 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/test_cache_control.py
+-rw-r--r--   0        0        0     1470 2023-05-19 03:36:49.481905 cacheyou-23.0/tests/test_chunked_response.py
+-rw-r--r--   0        0        0     5110 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_etag.py
+-rw-r--r--   0        0        0     6679 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_expires_heuristics.py
+-rw-r--r--   0        0        0     1769 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_max_age.py
+-rw-r--r--   0        0        0     1597 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_redirects.py
+-rw-r--r--   0        0        0      955 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_regressions.py
+-rw-r--r--   0        0        0     5380 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_serialization.py
+-rw-r--r--   0        0        0      259 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_server_http_version.py
+-rw-r--r--   0        0        0     5633 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_storage_filecache.py
+-rw-r--r--   0        0        0      789 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_storage_redis.py
+-rw-r--r--   0        0        0     2957 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/test_vary.py
+-rw-r--r--   0        0        0      792 2023-05-19 03:36:49.485906 cacheyou-23.0/tests/utils.py
+-rw-r--r--   0        0        0      484 2023-05-19 03:36:49.485906 cacheyou-23.0/tox.ini
+-rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 cacheyou-23.0/PKG-INFO
```

### Comparing `cacheyou-0.0.1/LICENSE.txt` & `cacheyou-23.0/LICENSE.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2012-2021  Eric Larson
+Copyright 2012-2021  Eric Larson, 2023 Frost Ming
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cacheyou-0.0.1/cachecontrol/_cmd.py` & `cacheyou-23.0/cacheyou/_cmd.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import logging
+from argparse import ArgumentParser
 
 import requests
 
-from cachecontrol.adapter import CacheControlAdapter
-from cachecontrol.cache import DictCache
-from cachecontrol.controller import logger
-
-from argparse import ArgumentParser
+from cacheyou.adapter import CacheControlAdapter
+from cacheyou.cache import DictCache
+from cacheyou.controller import logger
 
 
 def setup_logging():
     logger.setLevel(logging.DEBUG)
     handler = logging.StreamHandler()
     logger.addHandler(handler)
```

### Comparing `cacheyou-0.0.1/cachecontrol/adapter.py` & `cacheyou-23.0/cacheyou/adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import types
 import functools
+import types
 import zlib
 
 from requests.adapters import HTTPAdapter
 
-from .controller import CacheController, PERMANENT_REDIRECT_STATUSES
-from .cache import DictCache
-from .filewrapper import CallbackFileWrapper
+from cacheyou.cache import DictCache
+from cacheyou.controller import PERMANENT_REDIRECT_STATUSES, CacheController
+from cacheyou.filewrapper import CallbackFileWrapper
 
 
 class CacheControlAdapter(HTTPAdapter):
     invalidating_methods = {"PUT", "PATCH", "DELETE"}
 
     def __init__(
         self,
         cache=None,
         cache_etags=True,
         controller_class=None,
         serializer=None,
         heuristic=None,
         cacheable_methods=None,
         *args,
-        **kw
+        **kw,
     ):
-        super(CacheControlAdapter, self).__init__(*args, **kw)
+        super().__init__(*args, **kw)
         self.cache = DictCache() if cache is None else cache
         self.heuristic = heuristic
         self.cacheable_methods = cacheable_methods or ("GET",)
 
         controller_factory = controller_class or CacheController
         self.controller = controller_factory(
             self.cache, cache_etags=cache_etags, serializer=serializer
@@ -50,15 +50,15 @@
                 cached_response = None
             if cached_response:
                 return self.build_response(request, cached_response, from_cache=True)
 
             # check for etags and add headers if appropriate
             request.headers.update(self.controller.conditional_headers(request))
 
-        resp = super(CacheControlAdapter, self).send(request, **kw)
+        resp = super().send(request, **kw)
 
         return resp
 
     def build_response(
         self, request, response, from_cache=False, cacheable_methods=None
     ):
         """
@@ -116,22 +116,22 @@
                         if self.chunk_left == 0:
                             self._fp._close()
 
                     response._update_chunk_length = types.MethodType(
                         _update_chunk_length, response
                     )
 
-        resp = super(CacheControlAdapter, self).build_response(request, response)
+        resp = super().build_response(request, response)
 
         # See if we should invalidate the cache.
         if request.method in self.invalidating_methods and resp.ok:
             cache_url = self.controller.cache_url(request.url)
             self.cache.delete(cache_url)
 
         # Give the request a from_cache attr to let people use it
         resp.from_cache = from_cache
 
         return resp
 
     def close(self):
         self.cache.close()
-        super(CacheControlAdapter, self).close()
+        super().close()
```

### Comparing `cacheyou-0.0.1/cachecontrol/cache.py` & `cacheyou-23.0/cacheyou/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
 The cache object API for implementing caches. The default is a thread
 safe in-memory dictionary.
 """
 from threading import Lock
 
 
-class BaseCache(object):
-
+class BaseCache:
     def get(self, key):
         raise NotImplementedError()
 
     def set(self, key, value, expires=None):
         raise NotImplementedError()
 
     def delete(self, key):
         raise NotImplementedError()
 
     def close(self):
         pass
 
 
 class DictCache(BaseCache):
-
     def __init__(self, init_dict=None):
         self.lock = Lock()
         self.data = init_dict or {}
 
     def get(self, key):
         return self.data.get(key, None)
 
@@ -51,14 +49,15 @@
     That is, the expected interaction pattern is::
 
         cache.set(key, serialized_metadata)
         cache.set_body(key)
 
     Similarly, the body should be loaded separately via ``get_body()``.
     """
+
     def set_body(self, key, body):
         raise NotImplementedError()
 
     def get_body(self, key):
         """
         Return the body as file-like object.
         """
```

### Comparing `cacheyou-0.0.1/cachecontrol/caches/file_cache.py` & `cacheyou-23.0/cacheyou/caches/file_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import hashlib
 import os
 from textwrap import dedent
 
-from ..cache import BaseCache, SeparateBodyBaseCache
-from ..controller import CacheController
-
-try:
-    FileNotFoundError
-except NameError:
-    # py2.X
-    FileNotFoundError = (IOError, OSError)
+from cacheyou.cache import BaseCache, SeparateBodyBaseCache
+from cacheyou.controller import CacheController
 
 
 def _secure_open_write(filename, fmode):
     # We only want to write to this file, so open it in write only mode
     flags = os.O_WRONLY
 
     # os.O_CREAT | os.O_EXCL will fail if the file already exists, so we only
@@ -35,15 +29,15 @@
     if hasattr(os, "O_BINARY"):
         flags |= os.O_BINARY
 
     # Before we open our file, we want to delete any existing file that is
     # there
     try:
         os.remove(filename)
-    except (IOError, OSError):
+    except OSError:
         # The file must not exist already, so we can just skip ahead to opening
         pass
 
     # Open our file, the use of os.O_CREAT | os.O_EXCL will ensure that if a
     # race condition happens between the os.remove and this line, that an
     # error will be raised. Because we utilize a lockfile this should only
     # happen if someone is attempting to attack us.
@@ -64,18 +58,18 @@
         self,
         directory,
         forever=False,
         filemode=0o0600,
         dirmode=0o0700,
         lock_class=None,
     ):
-
         try:
             if lock_class is None:
                 from filelock import FileLock
+
                 lock_class = FileLock
         except ImportError:
             notice = dedent(
                 """
             NOTE: In order to use the FileCache you must have
             filelock installed. You can install it via pip:
               pip install filelock
@@ -116,15 +110,15 @@
     def _write(self, path, data: bytes):
         """
         Safely write the data to the given path.
         """
         # Make sure the directory exists
         try:
             os.makedirs(os.path.dirname(path), self.dirmode)
-        except (IOError, OSError):
+        except OSError:
             pass
 
         with self.lock_class(path + ".lock"):
             # Write our actual file
             with _secure_open_write(path, self.filemode) as fh:
                 fh.write(data)
```

### Comparing `cacheyou-0.0.1/cachecontrol/caches/redis_cache.py` & `cacheyou-23.0/cacheyou/caches/redis_cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
-from __future__ import division
 
-from datetime import datetime
-from cachecontrol.cache import BaseCache
+from datetime import datetime, timezone
 
+from cacheyou.cache import BaseCache
 
-class RedisCache(BaseCache):
 
+class RedisCache(BaseCache):
     def __init__(self, conn):
         self.conn = conn
 
     def get(self, key):
         return self.conn.get(key)
 
     def set(self, key, value, expires=None):
         if not expires:
             self.conn.set(key, value)
         elif isinstance(expires, datetime):
-            expires = expires - datetime.utcnow()
+            now_utc = datetime.now(timezone.utc)
+            if expires.tzinfo is None:
+                now_utc = now_utc.replace(tzinfo=None)
+            expires = expires - now_utc
             self.conn.setex(key, int(expires.total_seconds()), value)
         else:
             self.conn.setex(key, expires, value)
 
     def delete(self, key):
         self.conn.delete(key)
```

### Comparing `cacheyou-0.0.1/cachecontrol/controller.py` & `cacheyou-23.0/cacheyou/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
 The httplib2 algorithms ported for use with requests.
 """
+import calendar
 import logging
 import re
-import calendar
 import time
 from email.utils import parsedate_tz
 
 from requests.structures import CaseInsensitiveDict
 
-from .cache import DictCache, SeparateBodyBaseCache
-from .serialize import Serializer
-
+from cacheyou.cache import DictCache, SeparateBodyBaseCache
+from cacheyou.serialize import Serializer
 
 logger = logging.getLogger(__name__)
 
 URI = re.compile(r"^(([^:/?#]+):)?(//([^/?#]*))?([^?#]*)(\?([^#]*))?(#(.*))?")
 
 PERMANENT_REDIRECT_STATUSES = (301, 308)
 
@@ -29,15 +28,15 @@
 
     (scheme, authority, path, query, fragment) = parse_uri(uri)
     """
     groups = URI.match(uri).groups()
     return (groups[1], groups[3], groups[4], groups[6], groups[8])
 
 
-class CacheController(object):
+class CacheController:
     """An interface to see if request should cached or not."""
 
     def __init__(
         self, cache=None, cache_etags=True, serializer=None, status_codes=None
     ):
         self.cache = DictCache() if cache is None else cache
         self.cache_etags = cache_etags
@@ -354,15 +353,15 @@
             if response_headers.get("expires"):
                 expires = parsedate_tz(response_headers["expires"])
                 if expires is not None:
                     expires_time = calendar.timegm(expires) - date
 
             expires_time = max(expires_time, 14 * 86400)
 
-            logger.debug("etag object cached for {0} seconds".format(expires_time))
+            logger.debug(f"etag object cached for {expires_time} seconds")
             logger.debug("Caching due to etag")
             self._cache_set(cache_url, request, response, body, expires_time)
 
         # Add to the cache any permanent redirects. We do this before looking
         # that the Date headers.
         elif int(response.status) in PERMANENT_REDIRECT_STATUSES:
             logger.debug("Caching permanent redirect")
@@ -392,15 +391,15 @@
                     expires = parsedate_tz(response_headers["expires"])
                     if expires is not None:
                         expires_time = calendar.timegm(expires) - date
                     else:
                         expires_time = None
 
                     logger.debug(
-                        "Caching b/c of expires header. expires in {0} seconds".format(
+                        "Caching b/c of expires header. expires in {} seconds".format(
                             expires_time
                         )
                     )
                     self._cache_set(
                         cache_url,
                         request,
                         response,
@@ -428,19 +427,19 @@
         # The server isn't supposed to send headers that would make
         # the cached body invalid. But... just in case, we'll be sure
         # to strip out ones we know that might be problmatic due to
         # typical assumptions.
         excluded_headers = ["content-length"]
 
         cached_response.headers.update(
-            dict(
-                (k, v)
+            {
+                k: v
                 for k, v in response.headers.items()
                 if k.lower() not in excluded_headers
-            )
+            }
         )
 
         # we want a 200 b/c we have content via the cache
         cached_response.status = 200
 
         # update our cache
         self._cache_set(cache_url, request, cached_response)
```

### Comparing `cacheyou-0.0.1/cachecontrol/filewrapper.py` & `cacheyou-23.0/cacheyou/filewrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
-from tempfile import NamedTemporaryFile
 import mmap
+from tempfile import NamedTemporaryFile
 
 
-class CallbackFileWrapper(object):
+class CallbackFileWrapper:
     """
     Small wrapper around a fp object which will tee everything read into a
     buffer, and when that file is closed it will execute a callback with the
     contents of that buffer.
 
     All attributes are proxied to the underlying file object.
```

### Comparing `cacheyou-0.0.1/cachecontrol/heuristics.py` & `cacheyou-23.0/cacheyou/heuristics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import calendar
 import time
-
+from datetime import datetime, timedelta, timezone
 from email.utils import formatdate, parsedate, parsedate_tz
 
-from datetime import datetime, timedelta
-
 TIME_FMT = "%a, %d %b %Y %H:%M:%S GMT"
 
 
 def expire_after(delta, date=None):
-    date = date or datetime.utcnow()
+    date = date or datetime.now(timezone.utc)
     return date + delta
 
 
 def datetime_to_header(dt):
     return formatdate(calendar.timegm(dt.timetuple()))
 
 
-class BaseHeuristic(object):
-
+class BaseHeuristic:
     def warning(self, response):
         """
         Return a valid 1xx warning header value describing the cache
         adjustments.
 
         The response is provided too allow warnings like 113
         http://tools.ietf.org/html/rfc7234#section-5.5.4 where we need
@@ -62,15 +59,15 @@
     """
 
     def update_headers(self, response):
         headers = {}
 
         if "expires" not in response.headers:
             date = parsedate(response.headers["date"])
-            expires = expire_after(timedelta(days=1), date=datetime(*date[:6]))
+            expires = expire_after(timedelta(days=1), date=datetime(*date[:6], tzinfo=timezone.utc))
             headers["expires"] = datetime_to_header(expires)
             headers["cache-control"] = "public"
         return headers
 
 
 class ExpiresAfter(BaseHeuristic):
     """
@@ -97,16 +94,27 @@
     to calculate a reasonable value.
 
     Firefox also does something like this per
     https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching_FAQ
     http://lxr.mozilla.org/mozilla-release/source/netwerk/protocol/http/nsHttpResponseHead.cpp#397
     Unlike mozilla we limit this to 24-hr.
     """
+
     cacheable_by_default_statuses = {
-        200, 203, 204, 206, 300, 301, 404, 405, 410, 414, 501
+        200,
+        203,
+        204,
+        206,
+        300,
+        301,
+        404,
+        405,
+        410,
+        414,
+        501,
     }
 
     def update_headers(self, resp):
         headers = resp.headers
 
         if "expires" in headers:
             return {}
```

### Comparing `cacheyou-0.0.1/cachecontrol/serialize.py` & `cacheyou-23.0/cacheyou/serialize.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,75 +1,66 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import base64
 import io
 import json
+import pickle
 import zlib
 
 import msgpack
 from requests.structures import CaseInsensitiveDict
-
-from .compat import HTTPResponse, pickle, text_type
+from urllib3 import HTTPResponse
 
 
 def _b64_decode_bytes(b):
     return base64.b64decode(b.encode("ascii"))
 
 
 def _b64_decode_str(s):
     return _b64_decode_bytes(s).decode("utf8")
 
 
 _default_body_read = object()
 
 
-class Serializer(object):
+class Serializer:
     def dumps(self, request, response, body=None):
         response_headers = CaseInsensitiveDict(response.headers)
 
         if body is None:
             # When a body isn't passed in, we'll read the response. We
             # also update the response with a new file handler to be
             # sure it acts as though it was never read.
             body = response.read(decode_content=False)
             response._fp = io.BytesIO(body)
             response.length_remaining = len(body)
 
-        # NOTE: This is all a bit weird, but it's really important that on
-        #       Python 2.x these objects are unicode and not str, even when
-        #       they contain only ascii. The problem here is that msgpack
-        #       understands the difference between unicode and bytes and we
-        #       have it set to differentiate between them, however Python 2
-        #       doesn't know the difference. Forcing these to unicode will be
-        #       enough to have msgpack know the difference.
         data = {
-            u"response": {
-                u"body": body,  # Empty bytestring if body is stored separately
-                u"headers": dict(
-                    (text_type(k), text_type(v)) for k, v in response.headers.items()
-                ),
-                u"status": response.status,
-                u"version": response.version,
-                u"reason": text_type(response.reason),
-                u"decode_content": response.decode_content,
+            "response": {
+                "body": body,  # Empty bytestring if body is stored separately
+                "headers": {str(k): str(v) for k, v in response.headers.items()},
+                "status": response.status,
+                "version": response.version,
+                "reason": str(response.reason),
+                "decode_content": response.decode_content,
             }
         }
 
         # Construct our vary headers
-        data[u"vary"] = {}
-        if u"vary" in response_headers:
-            varied_headers = response_headers[u"vary"].split(",")
+        data["vary"] = {}
+        if "vary" in response_headers:
+            varied_headers = response_headers["vary"].split(",")
             for header in varied_headers:
-                header = text_type(header).strip()
+                header = str(header).strip()
                 header_value = request.headers.get(header, None)
                 if header_value is not None:
-                    header_value = text_type(header_value)
-                data[u"vary"][header] = header_value
+                    header_value = str(header_value)
+                data["vary"][header] = header_value
 
         return b",".join([b"cc=4", msgpack.dumps(data, use_bin_type=True)])
 
     def loads(self, request, data, body_file=None):
         # Short circuit if we've been given an empty set of data
         if not data:
             return
@@ -88,15 +79,15 @@
             ver = b"cc=0"
 
         # Get the version number out of the cc=N
         ver = ver.split(b"=", 1)[-1].decode("ascii")
 
         # Dispatch to the actual load method for the given version
         try:
-            return getattr(self, "_loads_v{}".format(ver))(request, data, body_file)
+            return getattr(self, f"_loads_v{ver}")(request, data, body_file)
 
         except AttributeError:
             # This is a version we don't have a loads function for, so we'll
             # just treat it as a miss and return None
             return
 
     def prepare_response(self, request, cached, body_file=None):
@@ -159,23 +150,22 @@
         try:
             cached = json.loads(zlib.decompress(data).decode("utf8"))
         except (ValueError, zlib.error):
             return
 
         # We need to decode the items that we've base64 encoded
         cached["response"]["body"] = _b64_decode_bytes(cached["response"]["body"])
-        cached["response"]["headers"] = dict(
-            (_b64_decode_str(k), _b64_decode_str(v))
-            for k, v in cached["response"]["headers"].items()
-        )
+        cached["response"]["headers"] = {
+            _b64_decode_str(k): _b64_decode_str(v) for k, v in cached["response"]["headers"].items()
+        }
         cached["response"]["reason"] = _b64_decode_str(cached["response"]["reason"])
-        cached["vary"] = dict(
-            (_b64_decode_str(k), _b64_decode_str(v) if v is not None else v)
+        cached["vary"] = {
+            _b64_decode_str(k): _b64_decode_str(v) if v is not None else v
             for k, v in cached["vary"].items()
-        )
+        }
 
         return self.prepare_response(request, cached, body_file)
 
     def _loads_v3(self, request, data, body_file):
         # Due to Python 2 encoding issues, it's impossible to know for sure
         # exactly how to load v3 entries, thus we'll treat these as a miss so
         # that they get rewritten out as v4 entries.
```

### Comparing `cacheyou-0.0.1/tests/conftest.py` & `cacheyou-23.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
-from pprint import pformat
-
 import os
 import socket
-
-import pytest
+from pprint import pformat
 
 import cherrypy
+import pytest
 
 
-class SimpleApp(object):
-
+class SimpleApp:
     def __init__(self):
         self.etag_count = 0
         self.update_etag_string()
 
     def dispatch(self, env):
         path = env["PATH_INFO"][1:].split("/")
         segment = path.pop(0)
@@ -49,15 +46,15 @@
             ("Vary", "Accept-Encoding, Accept"),
         ]
         start_response("200 OK", headers)
         return [response]
 
     def update_etag_string(self):
         self.etag_count += 1
-        self.etag_string = '"ETAG-{}"'.format(self.etag_count)
+        self.etag_string = f'"ETAG-{self.etag_count}"'
 
     def update_etag(self, env, start_response):
         self.update_etag_string()
         headers = [("Cache-Control", "max-age=5000"), ("Content-Type", "text/plain")]
         start_response("200 OK", headers)
         return [pformat(env).encode("utf8")]
 
@@ -82,38 +79,38 @@
         headers = [("Cache-Control", "no-cache")]
         start_response("200 OK", headers)
         return [pformat(env).encode("utf8")]
 
     def permanent_redirect(self, env, start_response):
         headers = [("Location", "/permalink")]
         start_response("301 Moved Permanently", headers)
-        return ["See: /permalink".encode("utf-8")]
+        return [b"See: /permalink"]
 
     def permalink(self, env, start_response):
         start_response("200 OK", [("Content-Type", "text/plain")])
-        return ["The permanent resource".encode("utf-8")]
+        return [b"The permanent resource"]
 
     def multiple_choices(self, env, start_response):
         headers = [("Link", "/permalink")]
         start_response("300 Multiple Choices", headers)
-        return ["See: /permalink".encode("utf-8")]
+        return [b"See: /permalink"]
 
     def stream(self, env, start_response):
         headers = [("Content-Type", "text/plain"), ("Cache-Control", "max-age=5000")]
         start_response("200 OK", headers)
 
         for i in range(10):
             yield pformat(i).encode("utf8")
 
     def fixed_length(self, env, start_response):
         body = b"0123456789"
         headers = [
             ("Content-Type", "text/plain"),
             ("Cache-Control", "max-age=5000"),
-            ("Content-Length", str(len(body)))
+            ("Content-Length", str(len(body))),
         ]
         start_response("200 OK", headers)
         return [body]
 
     def __call__(self, env, start_response):
         func = self.dispatch(env)
 
@@ -157,9 +154,9 @@
 
     cherrypy.server.start()
 
 
 def pytest_unconfigure(config):
     try:
         cherrypy.server.stop()
-    except:
+    except Exception:
         pass
```

### Comparing `cacheyou-0.0.1/tests/issue_263.py` & `cacheyou-23.0/tests/issue_263.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 #!/usr/bin/env python3
+import logging
 import sys
 
-import cachecontrol
 import requests
-from cachecontrol.cache import DictCache
-from cachecontrol.heuristics import BaseHeuristic
 
-import logging
+import cacheyou
+from cacheyou.cache import DictCache
+from cacheyou.heuristics import BaseHeuristic
 
 clogger = logging.getLogger("cachecontrol")
 clogger.addHandler(logging.StreamHandler())
 clogger.setLevel(logging.DEBUG)
 
 
-from pprint import pprint
-
-
 class NoAgeHeuristic(BaseHeuristic):
     def update_headers(self, response):
         if "cache-control" in response.headers:
             del response.headers["cache-control"]
 
 
-cache_adapter = cachecontrol.CacheControlAdapter(
+cache_adapter = cacheyou.CacheControlAdapter(
     DictCache(), cache_etags=True, heuristic=NoAgeHeuristic()
 )
 
 
 session = requests.Session()
 session.mount("https://", cache_adapter)
```

### Comparing `cacheyou-0.0.1/tests/test_adapter.py` & `cacheyou-23.0/tests/test_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import mock
-import pytest
+from unittest.mock import Mock
 
+import pytest
 from requests import Session
-from cachecontrol.adapter import CacheControlAdapter
-from cachecontrol.cache import DictCache
-from cachecontrol.wrapper import CacheControl
+
+from cacheyou.adapter import CacheControlAdapter
+from cacheyou.cache import DictCache
+from cacheyou.wrapper import CacheControl
 
 
 def use_wrapper():
     print("Using helper")
     sess = CacheControl(Session())
     return sess
 
@@ -30,16 +31,15 @@
     sess.get(url)
     yield sess
 
     # closing session object
     sess.close()
 
 
-class TestSessionActions(object):
-
+class TestSessionActions:
     def test_get_caches(self, url, sess):
         r2 = sess.get(url)
         assert r2.from_cache is True
 
     def test_get_with_no_cache_does_not_cache(self, url, sess):
         r2 = sess.get(url, headers={"Cache-Control": "no-cache"})
         assert not r2.from_cache
@@ -56,13 +56,13 @@
 
     def test_delete_invalidates_cache(self, url, sess):
         r2 = sess.delete(url)
         sess.get(url)
         assert not r2.from_cache
 
     def test_close(self):
-        cache = mock.Mock(spec=DictCache)
+        cache = Mock(spec=DictCache)
         sess = Session()
         sess.mount("http://", CacheControlAdapter(cache))
 
         sess.close()
         assert cache.close.called
```

### Comparing `cacheyou-0.0.1/tests/test_cache_control.py` & `cacheyou-23.0/tests/test_cache_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Unit tests that verify our caching methods work correctly.
 """
 import time
 from tempfile import mkdtemp
+from unittest.mock import ANY, Mock
 
 import pytest
-from mock import ANY, Mock
 
-from cachecontrol import CacheController
-from cachecontrol.cache import DictCache
-from cachecontrol.caches import SeparateBodyFileCache
+from cacheyou import CacheController
+from cacheyou.cache import DictCache
+from cacheyou.caches import SeparateBodyFileCache
 
 from .utils import DummyRequest, DummyResponse, NullSerializer
 
 TIME_FMT = "%a, %d %b %Y %H:%M:%S GMT"
 
 
-class TestCacheControllerResponse(object):
+class TestCacheControllerResponse:
     url = "http://url.com/"
 
     def req(self, headers=None):
         headers = headers or {}
         return Mock(full_url=self.url, url=self.url, headers=headers)  # < 1.x support
 
     def resp(self, headers=None):
         headers = headers or {}
-        return Mock(
-            status=200, headers=headers, request=self.req(), read=lambda **k: b"testing"
-        )
+        return Mock(status=200, headers=headers, request=self.req(), read=lambda **k: b"testing")
 
     @pytest.fixture()
     def cc(self):
         # Cache controller fixture
         return CacheController(Mock(), serializer=Mock())
 
     def test_no_cache_non_20x_response(self, cc):
@@ -217,28 +215,26 @@
         for r in [result, result2]:
             assert r.headers["ETag"] == etag
             assert r.headers["x-value"] == "b"
             assert r.headers["Content-Length"] == "100"
             assert r.read() == b"my body"
 
 
-class TestCacheControlRequest(object):
+class TestCacheControlRequest:
     url = "http://foo.com/bar"
 
     def setup_method(self):
         self.c = CacheController(DictCache(), serializer=NullSerializer())
 
     def req(self, headers):
         mock_request = Mock(url=self.url, headers=headers)
         return self.c.cached_request(mock_request)
 
     def test_cache_request_no_headers(self):
-        cached_resp = Mock(
-            headers={"ETag": "jfd9094r808", "Content-Length": 100}, status=200
-        )
+        cached_resp = Mock(headers={"ETag": "jfd9094r808", "Content-Length": 100}, status=200)
         self.c.cache = DictCache({self.url: cached_resp})
         resp = self.req({})
         assert not resp
 
     def test_cache_request_no_cache(self):
         resp = self.req({"cache-control": "no-cache"})
         assert not resp
```

### Comparing `cacheyou-0.0.1/tests/test_chunked_response.py` & `cacheyou-23.0/tests/test_chunked_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 """
 Test for supporting streamed responses (Transfer-Encoding: chunked)
 """
-from __future__ import print_function, unicode_literals
 
 import pytest
 import requests
 
-from cachecontrol import CacheControl
+from cacheyou import CacheControl
 
 
 @pytest.fixture()
 def sess():
     sess = CacheControl(requests.Session())
     yield sess
 
     # closing session object
     sess.close()
 
 
-class TestChunkedResponses(object):
-
+class TestChunkedResponses:
     def test_cache_chunked_response(self, url, sess):
         """
         Verify that an otherwise cacheable response is cached when the
         response is chunked.
         """
         url = url + "stream"
         r = sess.get(url)
```

### Comparing `cacheyou-0.0.1/tests/test_etag.py` & `cacheyou-23.0/tests/test_etag.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
+from unittest.mock import Mock, patch
+from urllib.parse import urljoin
+
 import pytest
 import requests
-from mock import Mock, patch
 
-from cachecontrol import CacheControl
-from cachecontrol.cache import DictCache
-from cachecontrol.compat import urljoin
+from cacheyou import CacheControl
+from cacheyou.cache import DictCache
 
 from .utils import NullSerializer
 
 
-class TestETag(object):
+class TestETag:
     """Test our equal priority caching with ETags
 
     Equal Priority Caching is a term I've defined to describe when
     ETags are cached orthgonally from Time Based Caching.
     """
 
     @pytest.fixture()
     def sess(self, url):
         self.etag_url = urljoin(url, "/etag")
         self.update_etag_url = urljoin(url, "/update_etag")
         self.cache = DictCache()
-        sess = CacheControl(
-            requests.Session(), cache=self.cache, serializer=NullSerializer()
-        )
+        sess = CacheControl(requests.Session(), cache=self.cache, serializer=NullSerializer())
         yield sess
 
         # closing session object
         sess.close()
 
     def test_etags_get_example(self, sess, server):
         """RFC 2616 14.26
@@ -76,15 +75,15 @@
         assert resp != r
         assert not resp.from_cache
 
         # Make sure we updated our cache with the new etag'd response.
         assert self.cache.get(self.etag_url) == resp.raw
 
 
-class TestDisabledETags(object):
+class TestDisabledETags:
     """Test our use of ETags when the response is stale and the
     response has an ETag.
     """
 
     @pytest.fixture()
     def sess(self, server, url):
         self.etag_url = urljoin(url, "/etag")
@@ -113,15 +112,15 @@
 
         r = sess.get(self.etag_url)
         assert r.from_cache
         assert "if-none-match" in r.request.headers
         assert r.status_code == 200
 
 
-class TestReleaseConnection(object):
+class TestReleaseConnection:
     """
     On 304s we still make a request using our connection pool, yet
     we do not call the parent adapter, which releases the connection
     back to the pool. This test ensures that when the parent `get`
     method is not called we consume the response (which should be
     empty according to the HTTP spec) and release the connection.
     """
```

### Comparing `cacheyou-0.0.1/tests/test_expires_heuristics.py` & `cacheyou-23.0/tests/test_expires_heuristics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import calendar
 import time
-from datetime import datetime
+from datetime import datetime, timezone
 from email.utils import formatdate, parsedate
 from pprint import pprint
+from unittest.mock import Mock
 
-from mock import Mock
 from requests import Session, get
 
-from cachecontrol import CacheControl
-from cachecontrol.heuristics import (
+from cacheyou import CacheControl
+from cacheyou.heuristics import (
     TIME_FMT,
     BaseHeuristic,
     ExpiresAfter,
     LastModified,
     OneDayCache,
 )
 
 from .utils import DummyResponse
 
 
-class TestHeuristicWithoutWarning(object):
+class TestHeuristicWithoutWarning:
     def setup_method(self):
         class NoopHeuristic(BaseHeuristic):
             warning = Mock()
 
             def update_headers(self, resp):
                 return {}
 
@@ -37,15 +37,15 @@
     def test_no_header_change_means_no_warning_header(self, url):
         the_url = url + "optional_cacheable_request"
         self.sess.get(the_url)
 
         assert not self.heuristic.warning.called
 
 
-class TestHeuristicWith3xxResponse(object):
+class TestHeuristicWith3xxResponse:
     def setup_method(self):
         class DummyHeuristic(BaseHeuristic):
             def update_headers(self, resp):
                 return {"x-dummy-header": "foobar"}
 
         self.sess = CacheControl(Session(), heuristic=DummyHeuristic())
 
@@ -56,22 +56,22 @@
 
     def test_heuristic_applies_to_304(self, url):
         the_url = url + "conditional_get"
         resp = self.sess.get(the_url)
         assert "x-dummy-header" in resp.headers
 
 
-class TestUseExpiresHeuristic(object):
+class TestUseExpiresHeuristic:
     def test_expires_heuristic_arg(self):
         sess = Session()
         cached_sess = CacheControl(sess, heuristic=Mock())
         assert cached_sess
 
 
-class TestOneDayCache(object):
+class TestOneDayCache:
     def setup_method(self):
         self.sess = Session()
         self.cached_sess = CacheControl(self.sess, heuristic=OneDayCache())
 
     def test_cache_for_one_day(self, url):
         the_url = url + "optional_cacheable_request"
         r = self.sess.get(the_url)
@@ -82,15 +82,15 @@
         pprint(dict(r.headers))
 
         r = self.sess.get(the_url)
         pprint(dict(r.headers))
         assert r.from_cache
 
 
-class TestExpiresAfter(object):
+class TestExpiresAfter:
     def setup_method(self):
         self.sess = Session()
         self.cache_sess = CacheControl(self.sess, heuristic=ExpiresAfter(days=1))
 
     def test_expires_after_one_day(self, url):
         the_url = url + "no_cache"
         resp = get(the_url)
@@ -102,15 +102,15 @@
         assert "warning" in r.headers
         assert r.headers["cache-control"] == "public"
 
         r = self.sess.get(the_url)
         assert r.from_cache
 
 
-class TestLastModified(object):
+class TestLastModified:
     def setup_method(self):
         self.sess = Session()
         self.cached_sess = CacheControl(self.sess, heuristic=LastModified())
 
     def test_last_modified(self, url):
         the_url = url + "optional_cacheable_request"
         r = self.sess.get(the_url)
@@ -125,15 +125,15 @@
         assert r.from_cache
 
 
 def datetime_to_header(dt):
     return formatdate(calendar.timegm(dt.timetuple()))
 
 
-class TestModifiedUnitTests(object):
+class TestModifiedUnitTests:
     def last_modified(self, period):
         return time.strftime(TIME_FMT, time.gmtime(self.time_now - period))
 
     def setup_method(self):
         self.heuristic = LastModified()
         self.time_now = time.time()
         day_in_seconds = 86400
@@ -153,15 +153,16 @@
         resp = DummyResponse(200, {"Expires": self.day_ahead})
         assert self.heuristic.update_headers(resp) == {}
 
     def test_last_modified_is_used(self):
         resp = DummyResponse(200, {"Date": self.now, "Last-Modified": self.week_ago})
         modified = self.heuristic.update_headers(resp)
         assert ["expires"] == list(modified.keys())
-        assert datetime(*parsedate(modified["expires"])[:6]) > datetime.now()
+        expected = datetime(*parsedate(modified["expires"])[:6], tzinfo=timezone.utc)
+        assert expected > datetime.now(timezone.utc)
 
     def test_last_modified_is_not_used_when_cache_control_present(self):
         resp = DummyResponse(
             200,
             {
                 "Date": self.now,
                 "Last-Modified": self.week_ago,
@@ -181,15 +182,16 @@
                 "Date": self.now,
                 "Last-Modified": self.week_ago,
                 "Cache-Control": "public",
             },
         )
         modified = self.heuristic.update_headers(resp)
         assert ["expires"] == list(modified.keys())
-        assert datetime(*parsedate(modified["expires"])[:6]) > datetime.now()
+        expected = datetime(*parsedate(modified["expires"])[:6], tzinfo=timezone.utc)
+        assert expected > datetime.now(timezone.utc)
 
     def test_warning_not_added_when_response_more_recent_than_24_hours(self):
         resp = DummyResponse(200, {"Date": self.now, "Last-Modified": self.week_ago})
         assert self.heuristic.warning(resp) is None
 
     def test_warning_is_not_added_when_heuristic_was_not_used(self):
         resp = DummyResponse(200, {"Date": self.now, "Expires": self.day_ahead})
```

### Comparing `cacheyou-0.0.1/tests/test_max_age.py` & `cacheyou-23.0/tests/test_max_age.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
-from __future__ import print_function
-import pytest
 
+import pytest
 from requests import Session
-from cachecontrol.adapter import CacheControlAdapter
-from cachecontrol.cache import DictCache
-from .utils import NullSerializer
 
+from cacheyou.adapter import CacheControlAdapter
+from cacheyou.cache import DictCache
+
+from .utils import NullSerializer
 
-class TestMaxAge(object):
 
+class TestMaxAge:
     @pytest.fixture()
     def sess(self, url):
         self.url = url
         self.cache = DictCache()
         sess = Session()
         sess.mount(
             "http://", CacheControlAdapter(self.cache, serializer=NullSerializer())
```

### Comparing `cacheyou-0.0.1/tests/test_redirects.py` & `cacheyou-23.0/tests/test_redirects.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Test for supporting redirect caches as needed.
 """
 import requests
 
-from cachecontrol import CacheControl
+from cacheyou import CacheControl
 
 
-class TestPermanentRedirects(object):
+class TestPermanentRedirects:
     def setup_method(self):
         self.sess = CacheControl(requests.Session())
 
     def test_redirect_response_is_cached(self, url):
         self.sess.get(url + "permanent_redirect", allow_redirects=False)
 
         resp = self.sess.get(url + "permanent_redirect", allow_redirects=False)
@@ -27,15 +27,15 @@
             url + "permanent_redirect",
             headers={"cache-control": "no-cache"},
             allow_redirects=False,
         )
         assert not resp.from_cache
 
 
-class TestMultipleChoicesRedirects(object):
+class TestMultipleChoicesRedirects:
     def setup_method(self):
         self.sess = CacheControl(requests.Session())
 
     def test_multiple_choices_is_cacheable(self, url):
         self.sess.get(url + "multiple_choices_redirect", allow_redirects=False)
 
         resp = self.sess.get(url + "multiple_choices_redirect", allow_redirects=False)
```

### Comparing `cacheyou-0.0.1/tests/test_regressions.py` & `cacheyou-23.0/tests/test_regressions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import sys
-import pytest
-
 
-from cachecontrol import CacheControl
-from cachecontrol.caches import FileCache
-from cachecontrol.filewrapper import CallbackFileWrapper
+import pytest
 from requests import Session
 
+from cacheyou import CacheControl
+from cacheyou.caches import FileCache
+from cacheyou.filewrapper import CallbackFileWrapper
 
-class Test39(object):
 
+class Test39:
     @pytest.mark.skipif(
         sys.version.startswith("2"), reason="Only run this for python 3.x"
     )
     def test_file_cache_recognizes_consumed_file_handle(self, url):
         s = CacheControl(Session(), FileCache("web_cache"))
         the_url = url + "cache_60"
         s.get(the_url)
```

### Comparing `cacheyou-0.0.1/tests/test_serialization.py` & `cacheyou-23.0/tests/test_serialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
+import pickle
+from unittest.mock import Mock
+
 import msgpack
 import requests
 
-from mock import Mock
-
-from cachecontrol.compat import pickle
-from cachecontrol.serialize import Serializer
+from cacheyou.serialize import Serializer
 
 
-class TestSerializer(object):
+class TestSerializer:
     def setup_method(self):
         self.serializer = Serializer()
         self.response_data = {
-            u"response": {
+            "response": {
                 # Encode the body as bytes b/c it will eventually be
                 # converted back into a BytesIO object.
-                u"body": "Hello World".encode("utf-8"),
-                u"headers": {
-                    u"Content-Type": u"text/plain",
-                    u"Expires": u"87654",
-                    u"Cache-Control": u"public",
+                "body": b"Hello World",
+                "headers": {
+                    "Content-Type": "text/plain",
+                    "Expires": "87654",
+                    "Cache-Control": "public",
                 },
-                u"status": 200,
-                u"version": 11,
-                u"reason": u"",
-                u"decode_content": True,
+                "status": 200,
+                "version": 11,
+                "reason": "",
+                "decode_content": True,
             }
         }
 
     def test_load_by_version_v0(self):
         data = b"cc=0,somedata"
         req = Mock()
         resp = self.serializer.loads(req, data)
         assert resp is None
 
     def test_read_version_v1(self):
         req = Mock()
         resp = self.serializer._loads_v1(req, pickle.dumps(self.response_data))
         # We have to decode our urllib3 data back into a unicode string.
-        assert resp.data == "Hello World".encode("utf-8")
+        assert resp.data == b"Hello World"
 
     def test_read_version_v2(self):
         req = Mock()
         compressed_base64_json = b'x\x9c\x1d\x8fK\x0f\x820\x10\x84\xff\xcb\x9e9h\xe3A\x9ax\xf0\x11K8hPi\xb8\x99>6\n!\xd4\xd0\x02!\x84\xff\xee\xc2qg\xbe\x9d\x9d\x9d\xa0E\xffs\x8dG\xe0\x13hgG\xe0\xf0\x14\xd2k\xb1\xffH\x16\x8fZd\x07\x88\xc0\xa2q\x16\xdf\xc65\x01\x9b\x00<\xb4\x1dF\xf0Ee\xb1\xf5\xcbj\xc6\xe2\xce\n\xd9\xd9\xf36\xc7\xe2TS\x0c\x8d;{\x8e\x07-\xae?\xfd9,1\x19\xbbVJ\xe4a\xa5\x93\xb4\xd7G\x929\x98D\x96Z\xd4\x15\x11\x8f\xe2;\xa8"\xad\xcd\xb0:\xf7\x8ba\xb7\x17U\x98#j\xaa\xbckH$\xcc\x07\x15::\xcc6\x9b\x08z\xeaP\xae\x0e[\xb8^\xb5\xf4\xc54\xcf\x7f\xef\xc0E\xe6'
         resp = self.serializer._loads_v2(req, compressed_base64_json)
         # We have to decode our urllib3 data back into a unicode string.
-        assert resp.data == "Hello World".encode("utf-8")
+        assert resp.data == b"Hello World"
 
     def test_load_by_version_v3(self):
         data = b"cc=3,somedata"
         req = Mock()
         resp = self.serializer.loads(req, data)
         assert resp is None
 
     def test_read_version_v4(self):
         req = Mock()
         resp = self.serializer._loads_v4(req, msgpack.dumps(self.response_data))
         # We have to decode our urllib3 data back into a unicode string.
-        assert resp.data == "Hello World".encode("utf-8")
+        assert resp.data == b"Hello World"
 
     def test_read_v1_serialized_with_py2_TypeError(self):
         # This tests how the code handles in reading data that was pickled
         # with an old version of cachecontrol running under Python 2
         req = Mock()
         py2_pickled_data = b"".join(
             [
@@ -76,15 +76,15 @@
                 b"sS'Cache-Control'\np15\nS'public'\np16\n",
                 b"sS'Expires'\np17\nS'87654'\np18\nsss.",
             ]
         )
         resp = self.serializer._loads_v1(req, py2_pickled_data)
         # We have to decode our urllib3 data back into a unicode
         # string.
-        assert resp.data == "Hello World".encode("utf-8")
+        assert resp.data == b"Hello World"
 
     def test_read_v2_corrupted_cache(self):
         # This should prevent a regression of bug #134
         req = Mock()
         assert self.serializer._loads_v2(req, b"") is None
 
     def test_read_latest_version_streamable(self, url):
@@ -98,45 +98,39 @@
         assert resp.read()
 
     def test_read_latest_version(self, url):
         original_resp = requests.get(url)
         data = original_resp.content
         req = original_resp.request
 
-        resp = self.serializer.loads(
-            req, self.serializer.dumps(req, original_resp.raw, data)
-        )
+        resp = self.serializer.loads(req, self.serializer.dumps(req, original_resp.raw, data))
 
         assert resp.read() == data
 
     def test_no_vary_header(self, url):
         original_resp = requests.get(url)
         data = original_resp.content
         req = original_resp.request
 
         # We make sure our response has a Vary header and that the
         # request doesn't have the header.
         original_resp.raw.headers["vary"] = "Foo"
 
-        assert self.serializer.loads(
-            req, self.serializer.dumps(req, original_resp.raw, data)
-        )
+        assert self.serializer.loads(req, self.serializer.dumps(req, original_resp.raw, data))
 
     def test_no_body_creates_response_file_handle_on_dumps(self, url):
         original_resp = requests.get(url, stream=True)
         data = None
         req = original_resp.request
 
-        assert self.serializer.loads(
-            req, self.serializer.dumps(req, original_resp.raw, data)
-        )
+        assert self.serializer.loads(req, self.serializer.dumps(req, original_resp.raw, data))
 
         # By passing in data=None it will force a read of the file
         # handle. Reading it again proves we're resetting the internal
         # file handle with a buffer.
         assert original_resp.raw.read()
 
     def test_no_incomplete_read_on_dumps(self, url):
         resp = requests.get(url + "fixed_length", stream=True)
         self.serializer.dumps(resp.request, resp.raw)
-        
+
         assert resp.content == b"0123456789"
```

### Comparing `cacheyou-0.0.1/tests/test_storage_filecache.py` & `cacheyou-23.0/tests/test_storage_filecache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Unit tests that verify FileCache storage works correctly.
 """
 import os
 import string
-
 from random import randint, sample
 
 import pytest
 import requests
-from cachecontrol import CacheControl
-from cachecontrol.caches import FileCache, SeparateBodyFileCache
 from filelock import FileLock
 
+from cacheyou import CacheControl
+from cacheyou.caches import FileCache, SeparateBodyFileCache
+
 
 def randomdata():
     """Plain random http data generator:"""
     key = "".join(sample(string.ascii_lowercase, randint(2, 4)))
     val = "".join(sample(string.ascii_lowercase + string.digits, randint(2, 10)))
-    return "&{}={}".format(key, val)
-
+    return f"&{key}={val}"
 
-class FileCacheTestsMixin(object):
 
+class FileCacheTestsMixin:
     FileCacheClass = None  # Either FileCache or SeparateBodyFileCache
 
     @pytest.fixture()
     def sess(self, url, tmpdir):
         self.url = url
         self.cache = self.FileCacheClass(str(tmpdir))
         sess = CacheControl(requests.Session(), cache=self.cache)
```

### Comparing `cacheyou-0.0.1/tests/test_storage_redis.py` & `cacheyou-23.0/tests/test_storage_redis.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
-from datetime import datetime
+from datetime import datetime, timezone
+from unittest.mock import Mock
 
-from mock import Mock
+from cacheyou.caches import RedisCache
 
-from cachecontrol.caches import RedisCache
 
-
-class TestRedisCache(object):
+class TestRedisCache:
     def setup_method(self):
         self.conn = Mock()
         self.cache = RedisCache(self.conn)
 
     def test_set_expiration_datetime(self):
         self.cache.set("foo", "bar", expires=datetime(2014, 2, 2))
         assert self.conn.setex.called
 
+    def test_set_expiration_datetime_aware(self):
+        self.cache.set("foo", "bar", expires=datetime(2014, 2, 2, tzinfo=timezone.utc))
+        assert self.conn.setex.called
+
     def test_set_expiration_int(self):
         self.cache.set("foo", "bar", expires=600)
         assert self.conn.setex.called
```

### Comparing `cacheyou-0.0.1/tests/test_vary.py` & `cacheyou-23.0/tests/test_vary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# SPDX-FileCopyrightText: 2015 Eric Larson
+# SPDX-FileCopyrightText: 2015 Eric Larson, 2023 Frost Ming
 #
 # SPDX-License-Identifier: Apache-2.0
 
+from pprint import pprint
+from urllib.parse import urljoin
+
 import pytest
 import requests
 
-from cachecontrol import CacheControl
-from cachecontrol.cache import DictCache
-from cachecontrol.compat import urljoin
-
-from pprint import pprint
-
+from cacheyou import CacheControl
+from cacheyou.cache import DictCache
 
-class TestVary(object):
 
+class TestVary:
     @pytest.fixture()
     def sess(self, url):
         self.url = urljoin(url, "/vary_accept")
         self.cache = DictCache()
         sess = CacheControl(requests.Session(), cache=self.cache)
         return sess
```

### Comparing `cacheyou-0.0.1/tests/utils.py` & `cacheyou-23.0/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Shared utility classes.
 """
 
 from requests.structures import CaseInsensitiveDict
 
 
-class NullSerializer(object):
+class NullSerializer:
 
     def dumps(self, request, response, body=None):
         return response
 
     def loads(self, request, data, body_file=None):
         if data and getattr(data, "chunked", False):
             data.chunked = False
```

### Comparing `cacheyou-0.0.1/PKG-INFO` & `cacheyou-23.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacheyou
-Version: 0.0.1
+Version: 23.0
 Summary: httplib2 caching for requests
 Keywords: requests http caching web
 Author-Email: Frost Ming <me@frostming.com>, Eric Larson <eric@ionrock.org>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -24,16 +24,17 @@
 Provides-Extra: redis
 Description-Content-Type: text/markdown
 
 
 # CacheYou
 
 [![Latest Version](https://img.shields.io/pypi/v/cacheyou.svg)](https://pypi.python.org/pypi/cacheyou)
+[![CI](https://github.com/frostming/cacheyou/actions/workflows/tests.yml/badge.svg)](https://github.com/frostming/cacheyou/actions/workflows/tests.yml)
 
-CachYou is a fork of [CacheControl] which is a port of the caching algorithms in httplib2 for use with
+CacheYou is a fork of [CacheControl] which is a port of the caching algorithms in httplib2 for use with
 requests session object.
 
 [CacheControl]: https://github.com/ionrock/cachecontrol
 
 ## Quickstart
 
 ```python
@@ -47,8 +48,8 @@
 ```
 
 If the URL contains any caching based headers, it will cache the
 result in a simple dictionary.
 
 For more info, check out the [docs]
 
-[docs]: http://cachecontrol.readthedocs.org/en/latest/
+[docs]: http://cacheyou.readthedocs.org/en/latest/
```

