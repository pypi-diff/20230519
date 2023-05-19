# Comparing `tmp/twitter-api-client-0.7.9.tar.gz` & `tmp/twitter-api-client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.7.9.tar", last modified: Thu May  4 22:30:42 2023, max compression
+gzip compressed data, was "twitter-api-client-0.8.0.tar", last modified: Fri May 19 04:24:48 2023, max compression
```

## Comparing `twitter-api-client-0.7.9.tar` & `twitter-api-client-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-04 22:30:42.583988 twitter-api-client-0.7.9/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6951 2023-05-04 22:30:42.583988 twitter-api-client-0.7.9/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-05-04 22:30:42.583988 twitter-api-client-0.7.9/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     8245 2023-05-04 22:26:29.000000 twitter-api-client-0.7.9/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-04 22:30:42.583988 twitter-api-client-0.7.9/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    11745 2023-05-04 22:19:22.000000 twitter-api-client-0.7.9/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     4524 2023-05-03 18:01:10.000000 twitter-api-client-0.7.9/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-30 17:24:38.000000 twitter-api-client-0.7.9/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-04 22:30:42.583988 twitter-api-client-0.7.9/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6951 2023-05-04 22:30:42.000000 twitter-api-client-0.7.9/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-05-04 22:30:42.000000 twitter-api-client-0.7.9/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-05-04 22:30:42.000000 twitter-api-client-0.7.9/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-05-04 22:30:42.000000 twitter-api-client-0.7.9/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-05-04 22:30:42.000000 twitter-api-client-0.7.9/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 04:24:48.953359 twitter-api-client-0.8.0/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6982 2023-05-19 04:24:48.953359 twitter-api-client-0.8.0/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-05-19 04:24:48.953359 twitter-api-client-0.8.0/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     8284 2023-05-19 04:15:40.000000 twitter-api-client-0.8.0/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 04:24:48.953359 twitter-api-client-0.8.0/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    11745 2023-05-04 22:19:22.000000 twitter-api-client-0.8.0/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4660 2023-05-19 04:06:49.000000 twitter-api-client-0.8.0/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-30 17:24:38.000000 twitter-api-client-0.8.0/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-19 04:24:48.953359 twitter-api-client-0.8.0/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6982 2023-05-19 04:24:48.000000 twitter-api-client-0.8.0/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-05-19 04:24:48.000000 twitter-api-client-0.8.0/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-05-19 04:24:48.000000 twitter-api-client-0.8.0/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-05-19 04:24:48.000000 twitter-api-client-0.8.0/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-05-19 04:24:48.000000 twitter-api-client-0.8.0/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.7.9/LICENSE` & `twitter-api-client-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.9/PKG-INFO` & `twitter-api-client-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.9
+Version: 0.8.0
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -227,20 +227,22 @@
 
 latest_results = search.run(
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'ios android',
     limit=100,
     latest=True,  # get latest tweets only
+    retries=3,
 )
 
 general_results = search.run(
     '(#dogs OR #cats) min_retweets:500',
     'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'skateboarding baseball guitar',
     'cheese bread butter',
     'ios android',
     limit=100,
+    retries=11,
 )
 ```
```

### Comparing `twitter-api-client-0.7.9/setup.py` & `twitter-api-client-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.7.9",
+    version="0.8.0",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     Implementation of Twitter's v1, v2, and GraphQL APIs
     
     Includes tools to **scrape**, **automate**, and **search**.
 
@@ -233,25 +233,27 @@
     
     latest_results = search.run(
         'brasil portugal -argentina',
         'paperswithcode -tensorflow -tf',
         'ios android',
         limit=100,
         latest=True,  # get latest tweets only
+        retries=3,
     )
     
     general_results = search.run(
         '(#dogs OR #cats) min_retweets:500',
         'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
         'brasil portugal -argentina',
         'paperswithcode -tensorflow -tf',
         'skateboarding baseball guitar',
         'cheese bread butter',
         'ios android',
         limit=100,
+        retries=11,
     )
     ```
     '''),
     long_description_content_type='text/markdown',
     author="Trevor Hobenshield",
     author_email="trevorhobenshield@gmail.com",
     url="https://github.com/trevorhobenshield/twitter-api-client",
```

### Comparing `twitter-api-client-0.7.9/twitter/account.py` & `twitter-api-client-0.8.0/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.9/twitter/constants.py` & `twitter-api-client-0.8.0/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.9/twitter/login.py` & `twitter-api-client-0.8.0/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.9/twitter/scraper.py` & `twitter-api-client-0.8.0/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.9/twitter/search.py` & `twitter-api-client-0.8.0/twitter/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,46 +49,49 @@
     async def process(self, queries: tuple, config: dict, out: Path, **kwargs) -> list:
         async with AsyncClient(headers=get_headers(self.session)) as s:
             return await asyncio.gather(*(self.paginate(q, s, config, out, **kwargs) for q in queries))
 
     async def paginate(self, query: str, session: AsyncClient, config: dict, out: Path, **kwargs) -> list[
         dict]:
         config['q'] = query
-        r, data, next_cursor = await self.backoff(lambda: self.get(session, config), query)
+        r, data, next_cursor = await self.backoff(lambda: self.get(session, config), query, **kwargs)
         all_data = [data]
         c = colors.pop() if colors else ''
         ids = set()
         while next_cursor:
             ids |= set(data['globalObjects']['tweets'])
             if len(ids) >= kwargs.get('limit', math.inf):
                 logger.debug(f'[{GREEN}success{RESET}] returned {len(ids)} search results for {c}{query}{reset}')
                 return all_data
             logger.debug(f'{c}{query}{reset}')
             config['cursor'] = next_cursor
 
-            r, data, next_cursor = await self.backoff(lambda: self.get(session, config), query)
+            r, data, next_cursor = await self.backoff(lambda: self.get(session, config), query, **kwargs)
+            if r is None:
+                return all_data
             data['query'] = query
             (out / f'raw/{time.time_ns()}.json').write_text(
                 orjson.dumps(data, option=orjson.OPT_INDENT_2).decode(),
                 encoding='utf-8'
             )
             all_data.append(data)
         return all_data
 
-    async def backoff(self, fn, info, retries=12):
+    async def backoff(self, fn, info, **kwargs):
+        retries = kwargs.get('retries', 3)
         for i in range(retries + 1):
             try:
                 r, data, next_cursor = await fn()
                 if not data.get('globalObjects', {}).get('tweets'):
                     raise Exception
                 return r, data, next_cursor
             except Exception as e:
                 if i == retries:
                     logger.debug(f'Max retries exceeded\n{e}')
-                    return
+                    return None, None, None
                 t = 2 ** i + random.random()
                 logger.debug(f'No data for: \u001b[1m{info}\u001b[0m | retrying in {f"{t:.2f}"} seconds\t\t{e}')
                 time.sleep(t)
 
     async def get(self, session: AsyncClient, params: dict) -> tuple:
         url = set_qs(self.api, params, update=True, safe='()')
         r = await session.get(url)
```

### Comparing `twitter-api-client-0.7.9/twitter/util.py` & `twitter-api-client-0.8.0/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.9/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.8.0/twitter_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.9
+Version: 0.8.0
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -227,20 +227,22 @@
 
 latest_results = search.run(
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'ios android',
     limit=100,
     latest=True,  # get latest tweets only
+    retries=3,
 )
 
 general_results = search.run(
     '(#dogs OR #cats) min_retweets:500',
     'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'skateboarding baseball guitar',
     'cheese bread butter',
     'ios android',
     limit=100,
+    retries=11,
 )
 ```
```

