# Comparing `tmp/twitter-api-client-0.8.0.tar.gz` & `tmp/twitter-api-client-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.8.0.tar", last modified: Fri May 19 04:24:48 2023, max compression
+gzip compressed data, was "twitter-api-client-0.8.1.tar", last modified: Fri May 19 17:27:56 2023, max compression
```

## Comparing `twitter-api-client-0.8.0.tar` & `twitter-api-client-0.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 04:24:48.953359 twitter-api-client-0.8.0/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6982 2023-05-19 04:24:48.953359 twitter-api-client-0.8.0/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-05-19 04:24:48.953359 twitter-api-client-0.8.0/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     8284 2023-05-19 04:15:40.000000 twitter-api-client-0.8.0/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 04:24:48.953359 twitter-api-client-0.8.0/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    11745 2023-05-04 22:19:22.000000 twitter-api-client-0.8.0/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     4660 2023-05-19 04:06:49.000000 twitter-api-client-0.8.0/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 04:24:48.953359 twitter-api-client-0.8.0/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6982 2023-05-19 04:24:48.000000 twitter-api-client-0.8.0/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-05-19 04:24:48.000000 twitter-api-client-0.8.0/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-05-19 04:24:48.000000 twitter-api-client-0.8.0/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-05-19 04:24:48.000000 twitter-api-client-0.8.0/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-05-19 04:24:48.000000 twitter-api-client-0.8.0/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 17:27:56.711608 twitter-api-client-0.8.1/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-30 17:24:38.000000 twitter-api-client-0.8.1/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     7092 2023-05-19 17:27:56.711608 twitter-api-client-0.8.1/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-05-19 17:27:56.711608 twitter-api-client-0.8.1/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     8414 2023-05-19 17:26:23.000000 twitter-api-client-0.8.1/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 17:27:56.711608 twitter-api-client-0.8.1/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-30 17:24:38.000000 twitter-api-client-0.8.1/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21951 2023-05-19 16:55:22.000000 twitter-api-client-0.8.1/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-30 17:24:38.000000 twitter-api-client-0.8.1/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-30 17:24:38.000000 twitter-api-client-0.8.1/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    11972 2023-05-19 16:55:22.000000 twitter-api-client-0.8.1/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     5193 2023-05-19 17:15:54.000000 twitter-api-client-0.8.1/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-30 17:24:38.000000 twitter-api-client-0.8.1/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 17:27:56.711608 twitter-api-client-0.8.1/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     7092 2023-05-19 17:27:56.000000 twitter-api-client-0.8.1/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-05-19 17:27:56.000000 twitter-api-client-0.8.1/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-05-19 17:27:56.000000 twitter-api-client-0.8.1/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-05-19 17:27:56.000000 twitter-api-client-0.8.1/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-05-19 17:27:56.000000 twitter-api-client-0.8.1/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.8.0/LICENSE` & `twitter-api-client-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.0/PKG-INFO` & `twitter-api-client-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.0
+Version: 0.8.1
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -196,16 +196,18 @@
     444444,
 ])
 
 
 
 # trends
 scraper.trends()
+```
 
-
+#### Resume Pagination
+```python
 from twitter.scraper import Scraper
 from twitter.constants import Operation
 
 email, username, password = ...,...,...
 scraper = Scraper(email, username, password, debug=1, save=True)
 
 operation = Operation.Followers
@@ -219,15 +221,16 @@
 
 #### Search
 
 ```python   
 from twitter.search import Search
 
 email, username, password = ..., ..., ...
-search = Search(email, username, password)
+# default output directory is `data/raw` if save=True
+search = Search(email, username, password, debug=1, save=True)
 
 latest_results = search.run(
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'ios android',
     limit=100,
     latest=True,  # get latest tweets only
```

### Comparing `twitter-api-client-0.8.0/setup.py` & `twitter-api-client-0.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.8.0",
+    version="0.8.1",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     Implementation of Twitter's v1, v2, and GraphQL APIs
     
     Includes tools to **scrape**, **automate**, and **search**.
 
@@ -202,16 +202,18 @@
         444444,
     ])
     
 
     
     # trends
     scraper.trends()
-
-
+    ```
+    
+    #### Resume Pagination
+    ```python
     from twitter.scraper import Scraper
     from twitter.constants import Operation
     
     email, username, password = ...,...,...
     scraper = Scraper(email, username, password, debug=1, save=True)
     
     operation = Operation.Followers
@@ -225,15 +227,16 @@
     
     #### Search
     
     ```python   
     from twitter.search import Search
     
     email, username, password = ..., ..., ...
-    search = Search(email, username, password)
+    # default output directory is `data/raw` if save=True
+    search = Search(email, username, password, debug=1, save=True)
     
     latest_results = search.run(
         'brasil portugal -argentina',
         'paperswithcode -tensorflow -tf',
         'ios android',
         limit=100,
         latest=True,  # get latest tweets only
```

### Comparing `twitter-api-client-0.8.0/twitter/account.py` & `twitter-api-client-0.8.1/twitter/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,42 @@
 import logging.config
 import math
 import mimetypes
 import random
 import time
 from copy import deepcopy
 from datetime import datetime
+from logging import Logger
 from pathlib import Path
 from urllib.parse import urlencode
 from uuid import uuid1, getnode
 
 import orjson
 from httpx import Response
 from tqdm import tqdm
 
 from .constants import *
 from .login import login
 from .util import find_key, get_headers, fmt_status, get_cursor, save_data
 
-logging.config.dictConfig(log_config)
-logger = logging.getLogger(__name__)
-
 
 class Account:
 
-    def __init__(self, email: str, username: str, password: str, *, save=True, debug: int = 0):
+    def __init__(self, email: str, username: str, password: str, **kwargs):
         self.session = login(email, username, password)
         self.gql_url = 'https://twitter.com/i/api/graphql'
         self.v1_url = 'https://api.twitter.com/1.1'
-        self.save = save
-        self.debug = debug
+        self.save = kwargs.get('save', True)
+        self.debug = kwargs.get('debug', 0)
+        self.logger = self.init_logger(kwargs.get('log_config', False))
+
+    @staticmethod
+    def init_logger(cfg: dict) -> Logger:
+        logging.config.dictConfig(cfg or log_config)
+        return logging.getLogger(__name__)
 
     def gql(self, method: str, operation: tuple, variables: dict, features: dict = Operation.default_features) -> dict:
         qid, op = operation
         params = {
             'queryId': qid,
             'features': features,
             'variables': Operation.default_variables | variables
@@ -368,15 +372,15 @@
         twid = int(self.session.cookies.get('twid').split('=')[-1].strip('"'))
         headers = get_headers(self.session)
         r = self.session.post(
             url=f'{self.v1_url}/strato/column/User/{twid}/search/searchSafety',
             headers=headers,
             json=settings,
         )
-        logger.debug(r)
+        self.logger.debug(r)
         return r
 
     def update_settings(self, settings: dict) -> dict:
         return self.v1('account/settings.json', settings)
 
     def change_password(self, old: str, new: str) -> dict:
         params = {
@@ -443,15 +447,15 @@
             variables['cursor'] = cursor
             data = self.gql(method, operation, variables)
 
             cursor = get_cursor(data)
             ids |= set(find_key(data, 'rest_id'))
 
             if self.debug:
-                logger.debug(f'cursor: {cursor}\tunique results: {len(ids)}')
+                self.logger.debug(f'cursor: {cursor}\tunique results: {len(ids)}')
 
             if prev_len == len(ids):
                 dups += 1
 
             res.append(data)
         return res
 
@@ -492,58 +496,58 @@
             with open(file, 'rb') as f:
                 i = 0
                 while chunk := f.read(UPLOAD_CHUNK_SIZE):  # todo: arbitrary max size for now
                     data = {'command': 'APPEND', 'media_id': media_id, 'segment_index': i}
                     files = {'media': chunk}
                     r = self.session.post(url=url, headers=headers, data=data, files=files)
                     if r.status_code < 200 or r.status_code > 299:
-                        logger.debug(f'{r.status_code} {r.text}')
+                        self.logger.debug(f'{r.status_code} {r.text}')
                         raise Exception(f'[{RED}error{RESET}] upload failed')
                     i += 1
                     pbar.update(f.tell() - pbar.n)
 
         data = {'command': 'FINALIZE', 'media_id': media_id, 'allow_async': 'true'}
         if is_dm:
             data |= {'original_md5': hashlib.md5(file.read_bytes()).hexdigest()}
         r = self.session.post(url=url, headers=headers, data=data)
 
-        # logger.debug(f'processing, please wait...')
+        # self.logger.debug(f'processing, please wait...')
         processing_info = r.json().get('processing_info')
         while processing_info:
             state = processing_info['state']
             if error := processing_info.get("error"):
                 raise Exception(f'media upload failed: {error}')
             if state == MEDIA_UPLOAD_SUCCEED:
                 break
             if state == MEDIA_UPLOAD_FAIL:
                 raise Exception(f'[{RED}error{RESET}] media processing failed')
             check_after_secs = processing_info.get('check_after_secs', random.randint(1, 5))
             time.sleep(check_after_secs)
             params = {'command': 'STATUS', 'media_id': media_id}
             r = self.session.get(url=url, headers=headers, params=params)
             processing_info = r.json().get('processing_info')
-        # logger.debug('processing complete')
+        # self.logger.debug('processing complete')
         return media_id
 
     def _add_alt_text(self, media_id: int, text: str) -> Response:
         params = {"media_id": media_id, "alt_text": {"text": text}}
         url = f'{self.v1_url}/media/metadata/create.json'
         r = self.session.post(url, headers=get_headers(self.session), json=params)
         return r
 
     def log(self, response: Response):
         status = fmt_status(response.status_code)
         if 'json' in response.headers.get('content-type', ''):
             if response.json().get('errors'):
-                logger.debug(f'[{RED}twitter error{RESET}]')
-                logger.debug(f'{response.url}')
-                logger.debug(f'{response.text}')
+                self.logger.debug(f'[{RED}twitter error{RESET}]')
+                self.logger.debug(f'{response.url}')
+                self.logger.debug(f'{response.text}')
                 return
-        logger.debug(status)
+        self.logger.debug(status)
         if self.debug >= 1:
-            logger.debug(f'{response.url}')
+            self.logger.debug(f'{response.url}')
         if self.debug >= 2:
-            logger.debug(f'{response.text}')
+            self.logger.debug(f'{response.text}')
         if self.debug >= 3:
-            logger.debug(f'{response.headers}')
+            self.logger.debug(f'{response.headers}')
         if self.debug >= 4:
-            logger.debug(f'{response.cookies}')
+            self.logger.debug(f'{response.cookies}')
```

### Comparing `twitter-api-client-0.8.0/twitter/constants.py` & `twitter-api-client-0.8.1/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.0/twitter/login.py` & `twitter-api-client-0.8.1/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.0/twitter/scraper.py` & `twitter-api-client-0.8.1/twitter/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import asyncio
 import logging.config
 import math
 import platform
 import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from logging import Logger
 from pathlib import Path
-from typing import List
 from urllib.parse import urlsplit
 
 import httpx
 import orjson
 from httpx import AsyncClient, Response
 from tqdm import tqdm
 
 from .constants import *
 from .login import login
 from .util import find_key, save_data, get_cursor, get_headers, set_qs, fmt_status
 
-logging.config.dictConfig(log_config)
-logger = logging.getLogger(__name__)
-
 try:
     if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
         import nest_asyncio
 
         nest_asyncio.apply()
 except:
     ...
@@ -34,19 +31,25 @@
 
         uvloop.install()
     except ImportError as e:
         ...
 
 
 class Scraper:
-    def __init__(self, email: str, username: str, password: str, *, save=True, debug=False):
+    def __init__(self, email: str, username: str, password: str, **kwargs):
         self.session = login(email, username, password)
         self.api = 'https://twitter.com/i/api/graphql'
-        self.save = save
-        self.debug = debug
+        self.save = kwargs.get('save', True)
+        self.debug = kwargs.get('debug', 0)
+        self.logger = self.init_logger(kwargs.get('log_config', False))
+
+    @staticmethod
+    def init_logger(cfg: dict) -> Logger:
+        logging.config.dictConfig(cfg or log_config)
+        return logging.getLogger(__name__)
 
     def users(self, screen_names: list[str]) -> list:
         return self._run(screen_names, Operation.UserByScreenName)
 
     def tweets_by_id(self, tweet_ids: list[int]) -> list[dict]:
         return self._run(tweet_ids, Operation.TweetResultByRestId)
 
@@ -169,29 +172,30 @@
             r = await self._query(session, _id, operation, cursor=cursor)
             data = r.json()
 
             cursor = get_cursor(data)
             ids |= set(find_key(data, 'rest_id'))
 
             if self.debug:
-                logger.debug(f'cursor: {cursor}\tunique results: {len(ids)}')
+                self.logger.debug(f'cursor: {cursor}\tunique results: {len(ids)}')
 
             if prev_len == len(ids):
                 dups += 1
 
             res.append(data)
 
         if is_resuming:
             return res, cursor
         return res
 
     def resume_pagination(self, *args, **kwargs):
         async def _resume(session: AsyncClient, _id: int | str, operation: tuple, limit=math.inf, **kwargs) -> tuple:
             session = AsyncClient(headers=get_headers(session), cookies=self.session.cookies)
             return await self._paginate(session, _id, operation, limit, **kwargs)
+
         return asyncio.run(_resume(*args, **kwargs))
 
     async def _query(self, session: AsyncClient, _id: int | str | list, operation: tuple, **kwargs) -> Response:
         qid, op, k = operation
         params = {k: orjson.dumps(v).decode() for k, v in {
             'variables': {k: _id} | Operation.default_variables | kwargs,
             'features': Operation.default_features,
@@ -232,15 +236,15 @@
         ext = urlsplit(cdn_url).path.split('/')[-1]
         try:
             with httpx.stream('GET', cdn_url) as r:
                 with open(f'{path}/{name}_{ext}', 'wb') as f:
                     for chunk in r.iter_bytes(chunk_size=chunk_size):
                         f.write(chunk)
         except Exception as e:
-            logger.debug(f'[{RED}error{RESET}] failed to download media: {post_url} {e}')
+            self.logger.debug(f'[{RED}error{RESET}] failed to download media: {post_url} {e}')
 
     def trends(self) -> dict:
         """Get trends for all UTC offsets"""
 
         def get_trends(offset: str, url: str, headers: dict):
             headers['x-twitter-utcoffset'] = offset
             r = self.session.get(url, headers=headers)
@@ -266,30 +270,30 @@
         return trends
 
     def log(self, r: Response | Response, txt: str, data: dict):
         status = r.status_code
 
         def stat(r):
             if self.debug >= 1:
-                logger.debug(f'{r.url}')
+                self.logger.debug(f'{r.url}')
             if self.debug >= 2:
-                logger.debug(f'{txt}')
+                self.logger.debug(f'{txt}')
 
             limits = {k: v for k, v in r.headers.items() if 'x-rate-limit' in k}
             current_time = int(time.time())
             wait = int(r.headers.get('x-rate-limit-reset', current_time)) - current_time
-            logger.debug(
+            self.logger.debug(
                 f"remaining: {MAGENTA}{limits['x-rate-limit-remaining']}/{limits['x-rate-limit-limit']}{RESET} requests")
-            logger.debug(f'reset:     {MAGENTA}{(wait / 60):.2f}{RESET} minutes')
+            self.logger.debug(f'reset:     {MAGENTA}{(wait / 60):.2f}{RESET} minutes')
 
         try:
             if 'json' in r.headers.get('content-type', ''):
                 if data.get('errors'):
-                    logger.debug(f'[{RED}error{RESET}] {status} {data}')
+                    self.logger.debug(f'[{RED}error{RESET}] {status} {data}')
                 else:
-                    logger.debug(fmt_status(status))
+                    self.logger.debug(fmt_status(status))
                     stat(r)
             else:
-                logger.debug(fmt_status(status))
+                self.logger.debug(fmt_status(status))
                 stat(r)
         except Exception as e:
-            logger.debug(f'failed to log: {e}')
+            self.logger.debug(f'failed to log: {e}')
```

### Comparing `twitter-api-client-0.8.0/twitter/search.py` & `twitter-api-client-0.8.1/twitter/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import asyncio
 import logging.config
 import math
 import platform
 import random
 import time
+from logging import Logger
 from pathlib import Path
 
 import orjson
 from httpx import AsyncClient
 
 from .constants import *
 from .login import login
 from .util import set_qs, get_headers, find_key
 
 reset = '\u001b[0m'
 colors = [f'\u001b[{i}m' for i in range(30, 38)]
-logging.config.dictConfig(log_config)
-logger = logging.getLogger(__name__)
 
 try:
     if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
         import nest_asyncio
 
         nest_asyncio.apply()
 except:
@@ -32,76 +31,93 @@
 
         uvloop.install()
     except ImportError as e:
         ...
 
 
 class Search:
-    def __init__(self, email: str, username: str, password: str):
+    def __init__(self, email: str, username: str, password: str, **kwargs):
         self.session = login(email, username, password)
         self.api = 'https://api.twitter.com/2/search/adaptive.json?'
+        self.save = kwargs.get('save', True)
+        self.debug = kwargs.get('debug', 0)
+        self.logger = self.init_logger(kwargs.get('log_config', False))
+
+    @staticmethod
+    def init_logger(cfg: dict) -> Logger:
+        logging.config.dictConfig(cfg or log_config)
+        return logging.getLogger(__name__)
 
     def run(self, *args, out: str = 'data', **kwargs):
         out_path = self.make_output_dirs(out)
         if kwargs.get('latest', False):
             search_config['tweet_search_mode'] = 'live'
         return asyncio.run(self.process(args, search_config, out_path, **kwargs))
 
     async def process(self, queries: tuple, config: dict, out: Path, **kwargs) -> list:
         async with AsyncClient(headers=get_headers(self.session)) as s:
             return await asyncio.gather(*(self.paginate(q, s, config, out, **kwargs) for q in queries))
 
     async def paginate(self, query: str, session: AsyncClient, config: dict, out: Path, **kwargs) -> list[
         dict]:
         config['q'] = query
-        r, data, next_cursor = await self.backoff(lambda: self.get(session, config), query, **kwargs)
+        data, next_cursor = await self.backoff(lambda: self.get(session, config), query, **kwargs)
         all_data = [data]
         c = colors.pop() if colors else ''
         ids = set()
         while next_cursor:
             ids |= set(data['globalObjects']['tweets'])
             if len(ids) >= kwargs.get('limit', math.inf):
-                logger.debug(f'[{GREEN}success{RESET}] returned {len(ids)} search results for {c}{query}{reset}')
+                if self.debug:
+                    self.logger.debug(
+                        f'[{GREEN}success{RESET}] returned {len(ids)} search results for {c}{query}{reset}')
                 return all_data
-            logger.debug(f'{c}{query}{reset}')
+            if self.debug:
+                self.logger.debug(f'{c}{query}{reset}')
             config['cursor'] = next_cursor
 
-            r, data, next_cursor = await self.backoff(lambda: self.get(session, config), query, **kwargs)
-            if r is None:
+            data, next_cursor = await self.backoff(lambda: self.get(session, config), query, **kwargs)
+            if not data:
                 return all_data
+
             data['query'] = query
-            (out / f'raw/{time.time_ns()}.json').write_text(
-                orjson.dumps(data, option=orjson.OPT_INDENT_2).decode(),
-                encoding='utf-8'
-            )
+
+            if self.save:
+                (out / f'raw/{time.time_ns()}.json').write_text(
+                    orjson.dumps(data, option=orjson.OPT_INDENT_2).decode(),
+                    encoding='utf-8'
+                )
             all_data.append(data)
         return all_data
 
     async def backoff(self, fn, info, **kwargs):
         retries = kwargs.get('retries', 3)
         for i in range(retries + 1):
             try:
-                r, data, next_cursor = await fn()
+                data, next_cursor = await fn()
                 if not data.get('globalObjects', {}).get('tweets'):
                     raise Exception
-                return r, data, next_cursor
+                return data, next_cursor
             except Exception as e:
                 if i == retries:
-                    logger.debug(f'Max retries exceeded\n{e}')
-                    return None, None, None
+                    if self.debug:
+                        self.logger.debug(f'Max retries exceeded\n{e}')
+                    return None, None
                 t = 2 ** i + random.random()
-                logger.debug(f'No data for: \u001b[1m{info}\u001b[0m | retrying in {f"{t:.2f}"} seconds\t\t{e}')
+                if self.debug:
+                    self.logger.debug(
+                        f'No data for: \u001b[1m{info}\u001b[0m | retrying in {f"{t:.2f}"} seconds\t\t{e}')
                 time.sleep(t)
 
     async def get(self, session: AsyncClient, params: dict) -> tuple:
         url = set_qs(self.api, params, update=True, safe='()')
         r = await session.get(url)
         data = r.json()
         next_cursor = self.get_cursor(data)
-        return r, data, next_cursor
+        return data, next_cursor
 
     def get_cursor(self, res: dict):
         try:
             if live := find_key(res, 'value'):
                 if cursor := [x for x in live if 'scroll' in x]:
                     return cursor[0]
             for instr in res['timeline']['instructions']:
@@ -110,15 +126,16 @@
                     if cursor['cursorType'] == 'Bottom':
                         return cursor['value']
                     continue
                 for entry in instr['addEntries']['entries']:
                     if entry['entryId'] == 'cursor-bottom-0':
                         return entry['content']['operation']['cursor']['value']
         except Exception as e:
-            logger.debug(e)
+            if self.debug:
+                self.logger.debug(e)
 
     def make_output_dirs(self, path: str) -> Path:
-        p = Path(f'~/{path}').expanduser()
+        p = Path(f'{path}')
         (p / 'raw').mkdir(parents=True, exist_ok=True)
         (p / 'processed').mkdir(parents=True, exist_ok=True)
         (p / 'final').mkdir(parents=True, exist_ok=True)
         return p
```

### Comparing `twitter-api-client-0.8.0/twitter/util.py` & `twitter-api-client-0.8.1/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.0/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.8.1/twitter_api_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.0
+Version: 0.8.1
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -196,16 +196,18 @@
     444444,
 ])
 
 
 
 # trends
 scraper.trends()
+```
 
-
+#### Resume Pagination
+```python
 from twitter.scraper import Scraper
 from twitter.constants import Operation
 
 email, username, password = ...,...,...
 scraper = Scraper(email, username, password, debug=1, save=True)
 
 operation = Operation.Followers
@@ -219,15 +221,16 @@
 
 #### Search
 
 ```python   
 from twitter.search import Search
 
 email, username, password = ..., ..., ...
-search = Search(email, username, password)
+# default output directory is `data/raw` if save=True
+search = Search(email, username, password, debug=1, save=True)
 
 latest_results = search.run(
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'ios android',
     limit=100,
     latest=True,  # get latest tweets only
```

