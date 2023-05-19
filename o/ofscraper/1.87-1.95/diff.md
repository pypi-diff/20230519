# Comparing `tmp/ofscraper-1.87.tar.gz` & `tmp/ofscraper-1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.87.tar", max compression
+gzip compressed data, was "ofscraper-1.95.tar", max compression
```

## Comparing `ofscraper-1.87.tar` & `ofscraper-1.95.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.87/LICENSE
--rw-r--r--   0        0        0     6024 2023-04-30 01:57:35.320013 ofscraper-1.87/README.md
--rw-r--r--   0        0        0     1235 2023-04-30 15:56:33.941101 ofscraper-1.87/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.87/src/__init__.py
--rw-r--r--   0        0        0      733 2023-04-30 15:56:33.941101 ofscraper-1.87/src/__version__.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.87/src/api/__init__.py
--rw-r--r--   0        0        0     2195 2023-04-29 21:06:53.651540 ofscraper-1.87/src/api/highlights.py
--rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.87/src/api/init.py
--rw-r--r--   0        0        0     1841 2023-04-29 21:06:53.652540 ofscraper-1.87/src/api/me.py
--rw-r--r--   0        0        0     3598 2023-04-29 21:06:53.652540 ofscraper-1.87/src/api/messages.py
--rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.87/src/api/paid.py
--rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.87/src/api/posts.py
--rw-r--r--   0        0        0     3273 2023-04-29 21:06:53.652540 ofscraper-1.87/src/api/profile.py
--rw-r--r--   0        0        0     2058 2023-04-29 21:06:53.652540 ofscraper-1.87/src/api/subscriptions.py
--rw-r--r--   0        0        0     5474 2023-04-29 21:06:53.652540 ofscraper-1.87/src/api/timeline.py
--rw-r--r--   0        0        0     4793 2023-04-29 21:06:53.652540 ofscraper-1.87/src/constants.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.87/src/db/__init__.py
--rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.87/src/db/operations.py
--rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.87/src/db/queries.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.87/src/interaction/__init__.py
--rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.87/src/interaction/like.py
--rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.87/src/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.87/src/prompts/prompt_strings.py
--rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.87/src/prompts/prompts.py
--rwxr-xr-x   0        0        0    19166 2023-04-30 01:56:48.978541 ofscraper-1.87/src/scraper.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.87/src/utils/__init__.py
--rw-r--r--   0        0        0     2864 2023-04-29 21:06:53.652540 ofscraper-1.87/src/utils/args.py
--rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.87/src/utils/auth.py
--rw-r--r--   0        0        0     8945 2023-04-29 21:06:53.652540 ofscraper-1.87/src/utils/config.py
--rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.87/src/utils/dates.py
--rw-r--r--   0        0        0    11230 2023-04-30 02:09:39.647464 ofscraper-1.87/src/utils/download.py
--rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.87/src/utils/encoding.py
--rw-r--r--   0        0        0     2938 2023-04-29 01:50:36.061807 ofscraper-1.87/src/utils/exit.py
--rw-r--r--   0        0        0     1142 2023-04-30 01:53:48.669716 ofscraper-1.87/src/utils/logger.py
--rw-r--r--   0        0        0     3004 2023-04-29 21:06:53.652540 ofscraper-1.87/src/utils/paths.py
--rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.87/src/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.87/src/utils/separate.py
--rw-r--r--   0        0        0     7233 1970-01-01 00:00:00.000000 ofscraper-1.87/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-19 18:02:23.727934 ofscraper-1.95/LICENSE
+-rw-r--r--   0        0        0     5177 2023-05-19 18:02:23.727934 ofscraper-1.95/README.md
+-rw-r--r--   0        0        0      607 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     1986 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2243 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/me.py
+-rw-r--r--   0        0        0     4359 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     1884 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     9170 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     2841 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1867 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     6457 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     4999 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     3611 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     5477 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    20976 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/prompts/prompts.py
+-rwxr-xr-x   0        0        0    22508 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/scraper.py
+-rw-r--r--   0        0        0        1 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3655 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8994 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0    10859 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      993 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    17597 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2938 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     4540 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     5369 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3008 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-05-19 18:02:24.687933 ofscraper-1.95/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     1505 2023-05-19 18:02:58.707954 ofscraper-1.95/pyproject.toml
+-rw-r--r--   0        0        0     6556 1970-01-01 00:00:00.000000 ofscraper-1.95/PKG-INFO
```

### Comparing `ofscraper-1.87/LICENSE` & `ofscraper-1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.87/README.md` & `ofscraper-1.95/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,37 +9,15 @@
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
         This is a theoritical program only and is for educational purposes. If you choose to use it then it may or may not work. You solely accept full responsability and indemnify the creator, hostors, contributors and all other involved persons from any any all responsability.
     </li>
 
- ## 1.8x Changes:
- - sync keys names across config(old keys will still work)
-  * change username to model_username in metadata
-  * change site_name to sitename in metadata
- - remove --purchased args
- - add purchase and pinned as post types
- - add letter-count argument
-   * This is for counting letters and not words for
-   textlength
- - added testing 
-    * to install run poetry install --with test 
-    * run with poetry run pytest
- - print path for each file
- - responsetype mapping in config
-    * This is for example keeping all messages or paid post in same folder, but also allow long time users to keep their current structure
- - added a Post class to serve as a 'single source of truth' for all responsetypes
- - removed unused functions like download_paid that are no longer needed
- - prompts and config functions have been revamped
- - shutdown handler
- - removed .tempmedia
- - added extension to responsetype profile downloads
- - fixed bugs caused by duplicate uploads on pages
- - additional bugs and fixes
+
 
   ## Description:
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
 
@@ -125,26 +103,35 @@
  
  # commandline
  While the menu is easy to use, and convient. You may want more automation.
  
  The best way to do this is through the commandline system. This will allow you to skip the menu, and for example scrape a provided list of accounts
  
   https://github.com/datawhores/ofscraper/wiki/command-line-args
+
+# Docker Support
+https://github.com/datawhores/ofscraper/pkgs/container/ofscraper
  
  # Customazation
     
 https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
 https://github.com/datawhores/ofscraper/wiki/Config-Options
 
   
 # Issues
 Open a issue in this repo, or you can mention your issue in the discord
 
 https://discord.gg/wN7uxEVHRK
     
+# Feature Requests
+
+https://ofscraper.clearflask.com/feedback
+    
+Or the discord
+    
     
 ## Common
 ### Status Down
       
 This typically means that your auth information is not correct, or onlyfans signed you out.
 ### 404 Issue
```

### Comparing `ofscraper-1.87/src/__init__.py` & `ofscraper-1.95/ofscraper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,10 +4,10 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
-from .__version__ import __title__, __description__, __url__, __version__
+from .__version__ import __title__, __description__, __url__
 from .__version__ import __author__, __author_email__, __license__
 from .__version__ import __copyright__
```

### Comparing `ofscraper-1.87/src/api/highlights.py` & `ofscraper-1.95/ofscraper/api/highlights.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,37 +6,41 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
 from itertools import chain
-
+import logging
 import httpx
 from tenacity import retry,stop_after_attempt,wait_random
+import ofscraper.constants as constants
+import ofscraper.utils.auth as auth
+log=logging.getLogger(__package__)
 
 
-from ..constants import NUM_TRIES,highlightsWithStoriesEP, highlightsWithAStoryEP, storyEP
-from ..utils import auth
 
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def scrape_highlights(headers, user_id) -> list:
     with httpx.Client(http2=True, headers=headers) as c:
-        url_stories = highlightsWithStoriesEP.format(user_id)
-        url_story = highlightsWithAStoryEP.format(user_id)
+        url_stories = constants.highlightsWithStoriesEP.format(user_id)
+        url_story = constants.highlightsWithAStoryEP.format(user_id)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url_stories, headers))
         r_multiple = c.get(url_stories, timeout=None)
 
         c.headers.update(auth.create_sign(url_story, headers))
         r_one = c.get(url_story, timeout=None)
 
+        # highlights_, stories
         if not r_multiple.is_error and not r_one.is_error:
+            log.debug(f"[bold]Highlight Post Count without Dupes[/bold] {len(r_multiple.json())} found")
+            log.debug(f"[bold]Story Post Count without Dupes[/bold] {len(r_one.json())} found")
             return get_highlightList(r_multiple.json()),r_one.json()
 
         r_multiple.raise_for_status()
         r_one.raise_for_status()
 
 def get_highlightList(data):
     for ele in list(filter(lambda x:isinstance(x,list),data.values())):
@@ -49,22 +53,9 @@
 
 
 
 
 
 
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-async def scrape_story(headers, story_id: int) -> list:
-    async with httpx.AsyncClient(http2=True, headers=headers) as c:
-        url = storyEP.format(story_id)
-
-        auth.add_cookies(c)
-        c.headers.update(auth.create_sign(url, headers))
-
-        r = await c.get(url, timeout=None)
-        if not r.is_error:
-            return r.json()['stories']
-        r.raise_for_status()
-
```

### Comparing `ofscraper-1.87/src/api/init.py` & `ofscraper-1.95/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.87/src/api/me.py` & `ofscraper-1.95/ofscraper/api/me.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,47 +4,56 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
+import logging
 import httpx
 from rich.console import Console
-console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
-from ..constants import meEP,subscribeCountEP,NUM_TRIES
-from ..utils import auth, encoding
+import ofscraper.constants as constants
+import ofscraper.utils.auth as auth
+import ofscraper.utils.encoding as encoding
+from ofscraper.utils.logger import updateSenstiveDict
+log=logging.getLogger(__package__)
+console=Console()
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=2, max=6),reraise=True,after=lambda retry_state:print(f"Attempting to login attempt:{retry_state.attempt_number}/5")) 
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=2, max=6),reraise=True,after=lambda retry_state:print(f"Attempting to login attempt:{retry_state.attempt_number}/5")) 
 def scrape_user(headers):
     with httpx.Client(http2=True, headers=headers) as c:
-        url = meEP
+        url = constants.meEP
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
         r = c.get(url, timeout=None)
         if not r.is_error:
+            updateSenstiveDict(r.json()["id"],"userid")
+            updateSenstiveDict(r.json()["username"],"username")
+            updateSenstiveDict(r.json()["name"],"name")
             return r.json()
         r.raise_for_status()
 
 
 def parse_user(profile):
     name = encoding.encode_utf_16(profile['name'])
     username = profile['username']
+
     return (name, username)
 
 
 def print_user(name, username):
-    console.print(f'Welcome, {name} | {username}')
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
+    if log.level<=constants.SUPPRESS_LOG_LEVEL:
+        console.print(f'Welcome, {name} | {username}')
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def parse_subscriber_count(headers):
     with httpx.Client(http2=True, headers=headers) as c:
-        url = subscribeCountEP
+        url = constants.subscribeCountEP
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
         r = c.get(url, timeout=None)
         if not r.is_error:
             data=r.json()
             return data["subscriptions"]["all"]
         r.raise_for_status()
```

### Comparing `ofscraper-1.87/src/api/posts.py` & `ofscraper-1.95/ofscraper/api/posts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from ..utils.config import read_config
 import re
-from ..constants import TEXTLENGTH_DEFAULT
-import src.utils.args as args_
-config = read_config()['config']
+import logging
+import httpx
+from ..constants import LICENCE_URL
+import ofscraper.utils.args as args_
+import ofscraper.utils.auth as auth
+from mpegdash.parser import MPEGDASHParser
+import ofscraper.utils.config as config
 
+log=logging.getLogger(__package__)
 
 class Post():
     def __init__(self, post, model_id, username, responsetype=None):
         self._post = post
         self._model_id = model_id
         self._username = username
         self._responsetype_ = responsetype or post.get("responseType")
@@ -52,27 +56,26 @@
     @property
     def responsetype_(self):
         return self._responsetype_
 
     @property
     def responsetype(self):
         if self.archived:
-            if config.get("responsetype", {}).get("archived") == "":
+            if config.get_archived_responsetype(config.read_config()) == "":
                 return "achived"
-            elif config.get("responsetype", {}).get("archived") == None:
-                return "achived"
-            elif config.get("responsetype", {}).get("archived") != "":
-                return config.get("responsetype", {}).get("archived")
+            return config.get_archived_responsetype(config.read_config())
+
         else:
-            if config.get("responsetype", {}).get(self._responsetype_) == "":
+            response=config.read_config().get("responsetype", {}).get(self._responsetype_) 
+            if  response == "":
                 return self._responsetype_
-            elif config.get("responsetype", {}).get(self._responsetype_) == None:
+            elif  response == None:
                 return self._responsetype_
-            elif config.get("responsetype", {}).get(self._responsetype_) != "":
-                return config.get("responsetype", {}).get(self._responsetype_)
+            elif  response != "":
+                return  response
 
     @property
     def id(self):
         return self._post["id"]
 
     @property
     def date(self):
@@ -191,26 +194,57 @@
     def postid(self):
         return self._post.id
 
     @property
     def text(self):
         return self._post.text
 
+    
+    @property
+    def mpd(self):
+        if self.url:
+            return None
+        return self._media.get("files",{}).get("drm",{}).get("manifest",{}).get("dash")
+    @property
+    def policy(self):
+        if self.url:
+            return None
+        return self._media.get("files",{}).get("drm",{}).get("signature",{}).get("dash",{}).get("CloudFront-Policy")
+    
+    @property
+    def keypair(self):
+        if self.url:
+            return None
+        return self._media.get("files",{}).get("drm",{}).get("signature",{}).get("dash",{}).get("CloudFront-Key-Pair-Id")
+    
+    @property
+    def signature(self):
+        if self.url:
+            return None
+        return self._media.get("files",{}).get("drm",{}).get("signature",{}).get("dash",{}).get("CloudFront-Signature")
+    
+
+    @property
+    def mpdout(self):
+        if not self.mpd:
+            return None
+
+
 
     @property
     def text_(self):
         text = self.text
         # this is for removing emojis
         # text=re.sub("[^\x00-\x7F]","",text)
         # this is for removing html tags
         text = re.sub("<[^>]*>", "", text)
         # this for remove random special invalid special characters
         text = re.sub('[\n<>:"/\|?*]+', '', text)
         text = re.sub(" +", " ", text)
-        length = int(config.get("textlength") or TEXTLENGTH_DEFAULT)
+        length = int(config.get_textlength(config.read_config()))
         if args_.getargs().letter_count:
             if length==0 and self._addcount():
                 return f"{text}_{self.count}"
             elif length==0 and not self._addcount():
                 return text
             elif length!=0 and not self._addcount():
                 return "".join(list(text))[:length]
@@ -244,17 +278,15 @@
 
     @property
     def count(self):
         return self._count+1
 
     @property
     def filename(self):
-        if not self.url:
-            return
-        return self.url.split('.')[-2].split('/')[-1].strip("/,.;!_-@#$%^&*()+\\ ")
+        return  re.sub("\.mpd$","",(self.url or self.mpd).split('.')[-2].split('/')[-1].strip("/,.;!_-@#$%^&*()+\\ "))
 
     @property
     def preview(self):
         if self.post.preview:
             return 1
         else:
             return 0
@@ -262,13 +294,32 @@
     @property
     def linked(self):
         return None
 
     @property
     def media(self):
         return self._media
+    @property
+    def parse_mpd(self): 
+        if not self.mpd:
+            return
+        headers = auth.make_headers(auth.read_auth())
+        params={"Policy":self.policy,"Key-Pair-Id":self.keypair,"Signature":self.signature}
+        with httpx.Client(http2=True, headers=headers,params=params) as c:
+            auth.add_cookies(c)
+            c.headers.update(auth.create_sign(self.mpd, headers))
+            r = c.get(self.mpd, timeout=None)
+            if r.status_code!=200:
+                return None
+            return MPEGDASHParser.parse(r.content.decode())
+    @property
+    def license(self):
+        responsetype=self.post.post["responseType"]
+        if responsetype in ["timeline","archived","pinned"]:
+            responsetype="post"
+        return LICENCE_URL.format(self.id,responsetype,self.postid)
 
     # for use in dynamic names
     def _addcount(self):
         if len(self._post.allmedia) > 1 or self.responsetype_ in ["stories", "highlights"]:
             return True
-        return False
+        return False
```

### Comparing `ofscraper-1.87/src/api/profile.py` & `ofscraper-1.95/ofscraper/api/profile.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,25 @@
         _____                                               
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
-
-from datetime import datetime
-from itertools import zip_longest
-
+import logging
 import httpx
 from rich.console import Console
-console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
 from ..constants import profileEP,NUM_TRIES
-from ..utils import auth, dates, encoding
+from ..utils import auth, encoding
 from xxhash import xxh32
 
+log=logging.getLogger(__package__)
+console=Console()
+
 @retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def scrape_profile(headers, username) -> dict:
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
@@ -62,15 +61,15 @@
 
 
 
 def print_profile_info(info):
     header_fmt = 'Name: {} | Username: {} | ID: {} | Joined: {}\n'
     info_fmt = '- {} posts\n -- {} photos\n -- {} videos\n -- {} audios\n- {} archived posts'
     final_fmt = header_fmt + info_fmt
-    console.print(final_fmt.format(*info))
+    log.info(final_fmt.format(*info))
 
 
 @retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def get_id(headers, username):
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
 
@@ -78,18 +77,9 @@
         c.headers.update(auth.create_sign(url, headers))
 
         r = c.get(url, timeout=None)
         if not r.is_error:
             return r.json()['id']
         r.raise_for_status()
 
-def print_paid_info(paid_content,username):
-    console.print(
-f"""
-Username: {username}
-- paid content {len(paid_content)}
- -- photos {len(list(filter(lambda x:x.get("mediatype")=="photo" or x.get("mediatype")=="gif",paid_content)))}
- -- videos {len(list(filter(lambda x:x.get("mediatype")=="video",paid_content)))}
- -- audios {len(list(filter(lambda x:x.get("mediatype")=="audio" ,paid_content)))}
-"""
-)
+
```

### Comparing `ofscraper-1.87/src/api/subscriptions.py` & `ofscraper-1.95/ofscraper/api/subscriptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
 from itertools import chain
-
+import logging
 import httpx
 from rich.console import Console
 console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
 from ..constants import subscriptionsEP,NUM_TRIES
 from ..utils import auth, dates
+log=logging.getLogger(__package__)
 
 
 async def get_subscriptions(headers, subscribe_count):
     offsets = range(0, subscribe_count, 10)
     tasks = [scrape_subscriptions(headers, offset) for offset in offsets]
     subscriptions = await asyncio.gather(*tasks)
     return list(chain.from_iterable(subscriptions))
@@ -41,12 +42,7 @@
 
 def parse_subscriptions(subscriptions: list) -> list:
     data = [{"name":profile['username'],"id":profile['id'],"date":dates.convert_date_to_mdyhms(
         profile['subscribedByExpireDate']),"active":not profile['subscribedIsExpiredNow'],"data":profile} for profile in subscriptions]
     return data
 
 
-def print_subscriptions(subscriptions: list):
-    fmt = '{:>4} {:^25} {:>15} {:^35}'
-    console.print(fmt.format('NUM', 'USERNAME', 'ID', 'EXPIRES ON'))
-    for c, t in enumerate(subscriptions, 1):
-        console.print(fmt.format(c, *t))
```

### Comparing `ofscraper-1.87/src/constants.py` & `ofscraper-1.95/ofscraper/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 purchased_contentEP = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}&user_id={}"
 
 mainPromptChoices = {
     'Download content from a user': 0,
     'Like all of a user\'s posts': 1,
     'Unlike all of a user\'s posts': 2,
-    'Edit auth.json`file': 3,
+    'Edit auth.json file': 3,
     'Edit config.json file': 4,
     'Edit Profile': 5,
 
 }
 usernameOrListChoices = {
     'Select from accounts on profile': 0,
     'Enter a username': 1,
@@ -83,22 +83,29 @@
 
 DIR_FORMAT_DEFAULT="{model_username}/{responsetype}/{mediatype}/"
 FILE_FORMAT_DEFAULT="{filename}.{ext}"
 METADATA_DEFAULT="{configpath}/{profile}/.data/{model_username}_{model_id}"
 FILE_SIZE_DEFAULT=0
 TEXTLENGTH_DEFAULT=0
 FILTER_DEFAULT=["Images","Audios","Videos"]
-SAVE_LOCATION_DEFAULT=str(pathlib.Path.home()/'Data/ofscraper')
+SAVE_PATH_DEFAULT=str(pathlib.Path.home()/'Data/ofscraper')
 DATE_DEFAULT="MM-DD-YYYY"
 PROFILE_DEFAULT="main_profile"
 PREMIUM_DEFAULT="Premium"
+MP4DECRYPT_DEFAULT=""
+FFMPEG_DEFAULT =""
+DISCORD_DEFAULT =""
+SUPPRESS_LOG_LEVEL=21
 RESPONSE_TYPE_DEFAULT= {
             "message":"messages",
             "timeline":"posts",
             "archived":"archived",
-            "paid":"paid",
+            "paid":"messages",
             "stories":"stories",
-            "highlights":"highlights",
+            "highlights":"stories",
             "profile":"profile",
             "pinned":"posts"
         }
-NUM_TRIES=5
+NUM_TRIES=5
+RESPONSE_EXPIRY=5000000
+LICENCE_URL="https://onlyfans.com/api2/v2/users/media/{}/drm/{}/{}?type=widevine"
+logname="ofscraper"
```

### Comparing `ofscraper-1.87/src/db/queries.py` & `ofscraper-1.95/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.87/src/interaction/like.py` & `ofscraper-1.95/ofscraper/interaction/like.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,40 +6,51 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import random
 import time
+import logging
 from typing import Union
 import asyncio
 import httpx
 from rich.console import Console
 console=Console()
 from halo import Halo
 from ..api import timeline
 from ..constants import favoriteEP, postURL
 from ..utils import auth
 
+log=logging.getLogger(__package__)
 
-def get_posts(headers, model_id,username):
-    with Halo(text='Getting posts...'):
+
+
+
+def get_posts(headers, model_id):
+    with Halo(text='Getting all timeline posts...'):
         pinned_posts = timeline.scrape_pinned_posts(headers, model_id)
-        timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id,username))
+        timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
         archived_posts = timeline.scrape_archived_posts(headers, model_id)
-
+    log.debug(f"[bold]Number of Post Found[/bold] {len(pinned_posts) + len(timeline_posts) + len(archived_posts)}")
     return pinned_posts + timeline_posts + archived_posts
 
 
 def filter_for_unfavorited(posts: list) -> list:
-    return list(filter(lambda x:x.get("isFavorite")==False,posts))
+    output=list(filter(lambda x:x.get("isFavorite")==False,posts))
+    log.debug(f"[bold]Number of unliked post[/bold {len(output)}")
+    return output
+
+
 
 
 def filter_for_favorited(posts: list) -> list:
-    return list(filter(lambda x:x.get("isFavorite")==True,posts))
+    output=list(filter(lambda x:x.get("isFavorite")==True,posts))
+    log.debug(f"[bold]Number of liked post[/bold {len(output)}")
+    return output
 
 
 
 def get_post_ids(posts: list) -> list:
     valid_post=list(filter(lambda x:x.get("isOpened")==True,posts))
     return list(map(lambda x:x.get("id"),valid_post))
    
@@ -66,14 +77,15 @@
                 retries = 0
                 while retries <= 1:
                     time.sleep(random.uniform(0.8, 0.9))
                     retries += 1
                     try:
                         r = c.post(url)
                         if not r.is_error or r.status_code == 400:
+                            log.debug(f"ID: {i} Performed {'like' if like_action==True else 'unlike'} action")
                             break
                         else:
                             _handle_err(r, postURL.format(i, username))
                     except httpx.TransportError as e:
                         _handle_err(e, postURL.format(i, username))
       
 
@@ -87,8 +99,8 @@
             if 'error' in json and 'message' in json['error']:
                 message = json['error']['message']
             status = f'STATUS CODE {param.status_code}: '
         else:
             message = str(param)
     except:
         pass
-    console.print(f'{status}{message}, post at {url}')
+    log.warning(f'{status}{message}, post at {url}')
```

### Comparing `ofscraper-1.87/src/prompts/prompt_functions.py` & `ofscraper-1.95/ofscraper/prompts/prompt_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 from prompt_toolkit.validation import Validator
 import re
 import string
-from pathvalidate import ValidationError, validate_filepath,validate_filename
+from pathvalidate import  validate_filepath,validate_filename
 import platform
 import pathlib
 import arrow
+import textwrap
+import ofscraper.utils.paths as paths
 def emptyListValidator():
     def callable(x):
         return len(x)>0
     return Validator.from_callable(
     callable,
     "You must select at least one"
     )
@@ -64,21 +66,17 @@
             return True
         except:
             return False
       
     
     return Validator.from_callable(
                 callable,
-f"""
-Possible Errors
-1. Placeholder syntax must be {{placeholder}}
-2. Invalid placeholder valid placeholders are {["date","responsetype","mediatype","value","model_id","first_letter","sitename","model_username"]}
-3. Must be a valid path when placeholders are replaced
-"""
-                
+textwrap.dedent(f"""
+Improper syntax or invalid placeholder
+""").strip()                
                 ,
                 move_cursor_to_end=True,
             )
 
 def fileformatvalidator():
     def callable(x):
         try:
@@ -97,21 +95,17 @@
             return True
         except:
             return False
       
     
     return Validator.from_callable(
                 callable,
-f"""
-Possible Errors
-1. Placeholder syntax must be {{placeholder}}
-2. Invalid placeholder valid placeholders are {["date","responsetype","mediatype","model_id",
-                                   "first_letter","sitename","model_username","post_id","filename","value","text","ext"]}
-3. Must be a filename when placeholders are replaced
-"""
+textwrap.dedent(f"""
+Improper syntax or invalid placeholder
+""").strip()
                 
                 ,
                 move_cursor_to_end=True,
             )
 
 def dateplaceholdervalidator():
     def callable(x):
@@ -120,22 +114,47 @@
                 return False
             return True
         except:
             return False
     return Validator.from_callable(
                 callable,
                 """
-                Date Format is invalid
-                See:https://arrow.readthedocs.io/en/latest/guide.html#supported-tokens
+    Date Format is invalid -> https://arrow.readthedocs.io/en/latest/guide.html#supported-tokens
                 """
                 ,True
     )
 
 
+def mp4decryptvalidator():
+    def callable(x):
+       return paths.mp4decryptchecker(x)
+            
+    return Validator.from_callable(
+                callable,
+textwrap.dedent(f"""
+Filepath is invalid or not detected as mp4decrypt
+""").strip()
+                
+                ,
+                move_cursor_to_end=True,
+            )
 
+def ffmpegvalidator():
+    def callable(x):
+       return paths.ffmpegchecker(x)
+            
+    return Validator.from_callable(
+                callable,
+textwrap.dedent(f"""
+Filepath is invalid or not detected as ffmpeg
+""").strip()
+                
+                ,
+                move_cursor_to_end=True,
+            )
 
 def metadatavalidator():
     def callable(x):
         try:
             placeholders=list(filter(lambda x:x!=None,[v[1] for v in string.Formatter().parse(x)]))
             validplaceholders=set(["sitename","first_letter","model_username","model_id","configpath","profile"])
             if len(list(filter(lambda x:x not in validplaceholders,placeholders)))>0:
@@ -149,17 +168,26 @@
             return True
         except:
             return False
       
     
     return Validator.from_callable(
                 callable,
-f"""
-Possible Errors
-1. Placeholder syntax must be {{placeholder}}
-2. Invalid placeholder valid placeholders are {["sitename","first_letter","model_username","model_id","configpath","profile"]}
-3. Must be a valid path when placeholders are replaced
-"""
+textwrap.dedent(f"""
+Improper syntax or invalid placeholder
+""").strip()
                 
                 ,
                 move_cursor_to_end=True,
-            )
+            )
+def DiscordValidator():
+    def callable(x):
+         if len(x)==0:
+            return True
+         return re.search("https://discord.com/api/webhooks/[0-9]*/[0-9a-z]*",x)!=None
+    return Validator.from_callable(
+    callable,
+textwrap.dedent(    
+"""
+must be discord webhook -> example: https://discord.com/api/webhooks/{numeric}/{alphanumeric}
+    """
+    ).strip())
```

### Comparing `ofscraper-1.87/src/prompts/prompts.py` & `ofscraper-1.95/ofscraper/prompts/prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,48 +3,44 @@
         _____                                               
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
-
-import re
-import json
 import sys
 from rich.console import Console
 import pathlib
-console=Console()
 from InquirerPy.resolver import prompt
 from InquirerPy.separator import Separator
 from InquirerPy.base import Choice
 from InquirerPy.validator import EmptyInputValidator,PathValidator
+import ofscraper.constants as constants
+import ofscraper.prompts.prompt_strings as prompt_strings
+import ofscraper.prompts.prompt_functions as prompt_functions
+import ofscraper.utils.config as config
 
-from ..constants import mainPromptChoices, profilesPromptChoices,FILTER_DEFAULT
-from .prompt_strings import CHECKLISTINSTRUCTIONS,FUZZY_INSTRUCTION
-from .prompt_functions import cleanTextInput,emptyListValidator,jsonValidator,jsonloader,namevalitator,dirformatvalidator \
-,dateplaceholdervalidator,fileformatvalidator,metadatavalidator
-import src.utils.config as config
+console=Console()
 def main_prompt() -> int:
-    main_prompt_choices = [*mainPromptChoices]
+    main_prompt_choices = [*constants.mainPromptChoices]
     main_prompt_choices.insert(3, Separator())
 
     name = 'action'
 
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': 'What would you like to do?',
             'choices': [*main_prompt_choices],
         }
     ]
 
     answer = prompt(questions)
-    return mainPromptChoices[answer[name]]
+    return constants.mainPromptChoices[answer[name]]
 
 
 
 
 
 
 
@@ -56,25 +52,25 @@
 
     questions = [
         {
             'type': 'checkbox',
             'qmark': '[?]',
             'name': name,
             'message': 'Which area(s) would you like to scrape? (Press ENTER to continue)',
-             "validate":emptyListValidator(),
+             "validate":prompt_functions.emptyListValidator(),
             'choices': [
                 Choice('Timeline'),
                 Choice('Pinned'),
                 Choice('Archived'),
                 Choice('Highlights'),
                 Choice('Stories'),
                 Choice('Messages'),
                 Choice("Purchased")
             ]
-            ,"instruction":CHECKLISTINSTRUCTIONS,
+            ,"instruction":prompt_strings.CHECKLISTINSTRUCTIONS,
 
         }
     ]
     answers = prompt(questions)
     return answers[name]
 
 
@@ -163,48 +159,48 @@
             'choices':["Enter Each Field Manually","Paste From Cookie Helper"],
             "default":"Enter Each Field Manually"
 
         }
     ]  
       
     return prompt(questions)[0]
-def user_agent_prompt(pcurrent):
+def user_agent_prompt(current):
     questions = [
         {
             'type': 'input',
             'message':'Enter User_Agent from browser',
             'default':current,
             'validate':EmptyInputValidator(),
-            'filter':lambda x:cleanTextInput(x)
+            'filter':lambda x:prompt_functions.cleanTextInput(x)
         }
     ]
     return  prompt(questions)[0]
 
 def xbc_prompt():
     questions = [
         {
             'type': 'input',
             'message':'Enter x-bc request header',
             'instruction':f"\nGo to browser network tools to view\nFor more instructions visit https://github.com/datawhores/ofscraper\n\n"
             ,'validate':EmptyInputValidator(),
-            'filter':lambda x:cleanTextInput(x)
+            'filter':lambda x:prompt_functions.cleanTextInput(x)
         }
     ]
     return  prompt(questions)[0]
 
 
 
 
 def auth_full_paste():
     questions = [
         {
             'type': 'input',
             'message':'Paste Text from Extension',
-            "validate": jsonValidator(),
-            "filter":jsonloader,
+            "validate": prompt_functions.jsonValidator(),
+            "filter":prompt_functions.jsonloader,
              "instruction":\
 """
 Cookie Helper Repo:https://github.com/M-rcus/OnlyFans-Cookie-Helper
 """
              
 
         }
@@ -215,20 +211,20 @@
     name = 'profile'
 
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': 'Select one of the following:',
-            'choices': [*profilesPromptChoices]
+            'choices': [*constants.profilesPromptChoices]
         }
     ]
 
     answer = prompt(questions)
-    return profilesPromptChoices[answer[name]]
+    return constants.profilesPromptChoices[answer[name]]
 
 
 def edit_profiles_prompt(profiles) -> str:
     name = 'edit'
 
     profile_names = [profile.stem for profile in profiles]
 
@@ -269,15 +265,15 @@
             'type': 'input',
             'name': name,
             'message': 
 """
 What would you like to name your new profile?
 only letters, numbers, and underscores are allowed
 """,
-            'validator':namevalitator()
+            'validator':prompt_functions.namevalitator()
 
         }
     ]
 
     answer = prompt(questions)
     return answer[name]
 
@@ -287,15 +283,15 @@
 
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': 'Select Profile',
             'choices':profiles
-            ,"validate":emptyListValidator()
+            ,"validate":prompt_functions.emptyListValidator()
         }
     ]
     answer = prompt(questions)
     profile = answer[name]
     return profile
 
 
@@ -303,24 +299,24 @@
 
     questions = [
         {
             'type': 'input',
             'name': 'main_profile',
             'message': 'What would you like your main profile to be?',
             'default': config.get_main_profile(config_),
-            "validate":lambda x:emptyListValidator() and  isinstance(x[0],str)
+            "validate":lambda x:prompt_functions.emptyListValidator() and  isinstance(x[0],str)
         },
         {
             'type': 'filepath',
             'name': 'save_location',
             'message':"save_location: ",
             'long_instruction': 'Where would you like to set as the root save downloaded directory?',
             'default':config.get_save_location(config_),
-            "filter":lambda x:cleanTextInput(x)
-            
+            "filter":lambda x:prompt_functions.cleanTextInput(x),
+            "validate": lambda x:pathlib.Path(x).is_dir() and PathValidator()
         },
         {
             'type': 'number',
             'name': 'file_size_limit',
             'message':"file_size_limit: ",
             'long_instruction':
 """
@@ -334,22 +330,22 @@
         },
            {
             'type': 'input',
             'name': 'dir_format',
             'message':"dir_format: ",
             'long_instruction': 'What format do you want for download directories',
             'default': config.get_dirformat(config_),
-             "validate":dirformatvalidator()
+             "validate":prompt_functions.dirformatvalidator()
         },
               {
             'type': 'input',
             'name': 'file_format',
             'message': 'What format do you want for downloaded files',
             'default':config.get_fileformat(config_),
-             "validate":fileformatvalidator()
+             "validate":prompt_functions.fileformatvalidator()
         },
                      {
             'type': 'number',
             'name': 'textlength',
             'message':"textlength: ",
             'long_instruction': 'Enter the max length to extract for post text, 0 means unlimited\n',
             'default': config.get_textlength(config_),
@@ -358,126 +354,160 @@
         },
          {
             'type': 'input',
             'name': 'date',
             'message': 'date: ',
             "long_instruction":"Enter Date format",
             'default': config.get_date(config_),
-             "validate":dateplaceholdervalidator()
+             "validate":prompt_functions.dateplaceholdervalidator()
         },
         {
             'type': 'input',
             'name': 'metadata',
             "message":"metadata: ",
             'long_instruction': 'Where should metadata files be saved',
             'default':config.get_metadata(config_),
-             "validate":metadatavalidator()
+             "validate":prompt_functions.metadatavalidator()
         },
         {
             'type': 'checkbox',
             'name': 'filter',
             "message":"filter: ",
-            'choices':list(map(lambda x:Choice(name=x,value=x, enabled=x.capitalize() in set(config.get_filter(config_))),FILTER_DEFAULT)),
-             "validate":emptyListValidator()
+            'choices':list(map(lambda x:Choice(name=x,value=x, enabled=x.capitalize() in set(config.get_filter(config_))),constants.FILTER_DEFAULT)),
+             "validate":prompt_functions.emptyListValidator()
+        },
+
+        {
+            'type': 'filepath',
+            'name': 'mp4decrypt',
+            "message":"mp4decrypt path: ",
+             "validate":PathValidator() and  EmptyInputValidator() and prompt_functions.mp4decryptvalidator(),
+            "default":config.get_mp4decrypt(config_),
+            "long_instruction":             """
+Certain content requires decryption to process please provide the full path to mp4decrypt
+Linux version [mp4decrypt] and windows version [mp4decrypt.exe] are provided in the repo         
+"""
+        },
+        {
+                        'type': 'filepath',
+            'name': 'ffmpeg',
+            "message":"ffmpeg path: ",
+             "validate":PathValidator() and  EmptyInputValidator() and prompt_functions.ffmpegvalidator(),
+             "long_instruction": 
+             """
+Certain content requires decryption to process please provide the full path to ffmpeg
+Linux version [ffmpeg] and windows version [ffmpeg.exe] are provided in the repo         
+""",
+"default":config.get_ffmpeg(config_)
+        
+        },
+
+        {
+            'type': 'input',
+            'name': 'discord',
+            "message":"discord webhook: ",
+             "validate":prompt_functions.DiscordValidator(),
+             "default":config.get_discord(config_)
         },
   
     ]
 
     questions2 = [
         {
             'type': 'input',
             'name': 'timeline',
             'long_instruction': 
             """
 set responsetype for timeline posts
 Empty string is consider to be 'posts'
             """,
             'default': config.get_timeline_responsetype(config_),
-            'message':"input: "
+            'message':"timeline responsetype mapping: "
         },
              {
             'type': 'input',
             'name': 'archived',
             'long_instruction': 
             """
 set responsetype for archived posts
 Empty string is consider to be 'archived'
             """,
             'default': config.get_archived_responsetype(config_),
-            'message':"input: "
+            'message':"archived responsetype mapping: "
         },
 
     {
             'type': 'input',
             'name': 'pinned',
             'long_instruction': 
             """
 set responsetype for pinned posts
-Empty string is consider to be 'archived'
+Empty string is consider to be 'pinned'
             """,
-            'default': config.get_archived_responsetype(config_),
-            'message':"input: "
+            'default': config.get_pinned_responsetype(config_),
+            'message':"pinned responsetype mapping: "
         },
                      {
             'type': 'input',
             'name': 'message',
             'long_instruction': 
             """
 set responsetype for message posts
 Empty string is consider to be 'message'
             """,
             'default': config.get_messages_responsetype(config_),
-            'message':"input: "
+            'message':"message responstype mapping: "
         },
                         {
             'type': 'input',
             'name': 'paid',
             'long_instruction': 
             """
 set responsetype for paid posts
 Empty string is consider to be 'paid'
             """,
             'default': config.get_paid_responsetype(config_),
-            'message':"input: "
+            'message':"paid responsetype mapping: "
         },
                              {
     'type': 'input',
             'name': 'stories',
             'long_instruction': 
             """
 set responsetype for stories
 Empty string is consider to be 'stories'
             """,
             'default': config.get_stories_responsetype(config_),
-            'message':"input: "
+            'message':"stories responsetype mapping: "
         },
                                     {
     'type': 'input',
             'name': 'highlights',
             'long_instruction': 
             """
 set responsetype for highlights
 Empty string is consider to be 'highlights'
             """,
             'default': config.get_highlights_responsetype(config_),
-            'message':"input: "
+            'message':"highlight responsetype mapping: "
         },
                                           {
     'type': 'input',
             'name': 'profile',
             'long_instruction': 
             """
 set responsetype for profile
 Empty string is consider to be 'profile'
             """,
             'default': config.get_profile_responsetype(config_),
-            'message':"input: "
+            'message':"profile responsetype mapping: "
         }
      ]
     answers = prompt(questions)
+    console.print("Set mapping for {responsetype} placeholder\n\n")
     answers["responsetype"]=prompt(questions2)
     return answers
 def reset_username_prompt() -> bool:
     name = 'reset username'
     questions = [
         {
             'type': 'list',
@@ -485,14 +515,56 @@
             'message': "Do you want to reset username option",
             'choices':["Yes","No"]
         }
     ]
 
     answer = prompt(questions)
     return answer[name]
+def mp4_prompt(config_):
+    questions = [
+         {
+            'type': 'filepath',
+            'name': 'mp4decrypt',
+            "message":"mp4decrypt path: ",
+             "validate":PathValidator() and  EmptyInputValidator() and prompt_functions.mp4decryptvalidator(),
+             "long_instruction": 
+             """
+Certain content requires decryption to process please provide the full path to mp4decrypt
+Linux version [mp4decrypt] and windows version [mp4decrypt.exe] are provided in the repo
+
+https://www.bento4.com/documentation/mp4decrypt/
+""",
+"default":config.get_mp4decrypt(config_)
+        },
+    ]
+
+    answer = prompt(questions)
+    return answer["mp4decrypt"]
+
+def ffmpeg_prompt(config_):
+    questions = [
+         {
+            'type': 'filepath',
+            'name': 'ffmpeg',
+            "message":"ffmpeg path: ",
+             "validate":PathValidator() and  EmptyInputValidator() and prompt_functions.ffmpegvalidator(),
+             "long_instruction": 
+             """
+Certain content requires decryption to process please provide the full path to ffmpeg
+Linux version [ffmpeg] and windows version [ffmpeg.exe] are provided in the repo 
+
+https://ffmpeg.org/download.html
+""",
+"default":config.get_ffmpeg(config_)
+        },
+    ]
+
+    answer = prompt(questions)
+    return answer["ffmpeg"] 
+
 def continue_prompt() -> bool:
     name = 'reset username'
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': "Do you want to continue with script",
@@ -508,16 +580,16 @@
       "keybindings":{
                              "toggle": [{"key": "s-right"},{"key": ["pagedown","right"]},{"key": ["home","right"]}],
 
                               
                          }
                          
      ,"multiselect":True
-      ,"validate":emptyListValidator(),
-      "instruction":FUZZY_INSTRUCTION,
+      ,"validate":prompt_functions.emptyListValidator(),
+      "instruction":prompt_strings.FUZZY_INSTRUCTION,
       "choices":list(map(lambda x:Choice(x,name=f"{x['name']} {x['date'] } {x['active']}")   ,sorted(models,key=lambda x:x['name']))),"transformer":lambda result:",".join(map(lambda x:x.split(" ")[0],result))
        ,"prompt":'Filter: ',
        "marker":"\u25c9 ",
        "marker_pl":"\u25cb "
 
       },
```

### Comparing `ofscraper-1.87/src/scraper.py` & `ofscraper-1.95/ofscraper/scraper.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,68 +9,91 @@
 """
 
 import asyncio
 import os
 import sys
 import platform
 import time
+import traceback
 import schedule
-from contextlib import contextmanager
 import threading
 import queue
+import logging
+import textwrap
+from contextlib import contextmanager
+import timeit
 from itertools import chain
 import re
 from rich.console import Console
-import traceback
-
-from .prompts import prompts
-console=Console()
-from .constants import donateEP
-from .api import init, highlights, me, messages, profile, subscriptions, paid, timeline
-from .db import operations
-from .interaction import like
-from .utils import auth, config, download, profiles
 import webbrowser
 from halo import Halo
-from .utils.config import read_config
-import src.api.posts as posts_
-import src.utils.args as args_
-import src.utils.paths as paths
-import src.utils.exit as exit
+import arrow
+import ofscraper.prompts.prompts as prompts
+import ofscraper.api.messages as messages
+import ofscraper.db.operations as operations
+import ofscraper.api.posts as posts_
+import ofscraper.utils.args as args_
+import ofscraper.utils.paths as paths
+import ofscraper.utils.exit as exit
+import ofscraper.api.paid as paid
+import ofscraper.api.highlights as highlights
+import ofscraper.api.timeline as timeline
+import ofscraper.api.profile as profile
+import ofscraper.utils.config as config
+import ofscraper.api.subscriptions as subscriptions
+import ofscraper.api.me as me
+import ofscraper.utils.auth as auth
+import ofscraper.utils.profiles as profiles
+import ofscraper.api.init as init
+import ofscraper.utils.download as download
+import ofscraper.interaction.like as like
+import ofscraper.utils.logger as logger
+import ofscraper.utils.args as args_
+import ofscraper.constants as constants
+
 
 
+console=Console()
+log=logger.init_logger(logging.getLogger(__package__))
+args=args_.getargs()
+log.debug(args)
+f = open(os.devnull, 'w')
 
-@Halo(text='Getting messages...')
+@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f ,text='Getting messages...')
 def process_messages(headers, model_id,username):
-    messages_ =asyncio.run(messages.get_messages(headers,  model_id,username)) 
-    operations.save_messages_response(messages_,model_id,username)
+    messages_ =asyncio.run(messages.get_messages(headers,  model_id)) 
     messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
+    log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),messages_))}")
+    log.debug("Removing locked messages media")
     for message in messages_:
      operations.write_messages_table(message)
     output=[]
     [ output.extend(message.media) for message in messages_]
     return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
-@Halo(text='Getting Paid Content...')
-def process_paid_post(headers, model_id,username):
+@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting Paid Content...')
+def process_paid_post(model_id,username):
     paid_content=paid.scrape_paid(username)
     paid_content=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="paid"),paid_content))
+    log.debug(f"[bold]Paid Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),paid_content))}")
+    log.debug("Removing locked paid media")
     for post in paid_content:
         operations.write_post_table(post,model_id,username)
     output=[]
     [output.extend(post.media) for post in paid_content]
     return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
          
 
-@Halo(text='Getting highlights and stories...')
+@Halo(stream=sys.stdout  if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting highlights and stories...\n')
 def process_highlights(headers, model_id,username):
     highlights_, stories = highlights.scrape_highlights(headers, model_id)
     highlights_, stories=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="highlights"),highlights_)),\
     list(map(lambda x:posts_.Post(x,model_id,username,responsetype="stories"),stories))
+    log.debug(f"[bold]Combined Story and Highlight Media count[/bold] {sum(map(lambda x:len(x.allmedia), highlights_))+sum(map(lambda x:len(x.allmedia), stories))}")
     for post in highlights_:
         operations.write_stories_table(post,model_id,username)
     for post in stories:
         operations.write_stories_table(post,model_id,username)   
     output=[]
     output2=[]
     [ output.extend(highlight.media) for highlight in highlights_]
@@ -80,64 +103,70 @@
      
 
 
 
 
 
 
-@Halo(text='Getting timeline media...')
+@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting timeline media...')
 def process_timeline_posts(headers, model_id,username):
-    timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id,username))
-    operations.save_timeline_response(timeline_posts,model_id,username)
+    timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
     timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
+    log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),timeline_posts))}")
+    log.debug("Removing locked timeline media")
     for post in timeline_posts:
         operations.write_post_table(post,model_id,username)
     output=[]
     [output.extend(post.media) for post in  timeline_posts ]
     return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
-@Halo(text='Getting archived media...')
+@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting archived media...')
 def process_archived_posts(headers, model_id,username):
     archived_posts = timeline.get_archive_post(headers, model_id)
-    operations.save_archive_response(archived_posts,model_id,username)
     archived_posts =list(map(lambda x:posts_.Post(x,model_id,username),archived_posts ))
+    log.debug(f"[bold]Archived Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),archived_posts))}")
+    log.debug("Removing locked archived media")
+
     for post in archived_posts:
         operations.write_post_table(post,model_id,username)
     output=[]
     [ output.extend(post.media) for post in archived_posts ]
     return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 
 
 
-@Halo(text='Getting pinned media...')
+@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting pinned media...')
 def process_pinned_posts(headers, model_id,username):
     pinned_posts = timeline.get_pinned_post(headers, model_id,username)
-    operations.save_pinned_response(pinned_posts,model_id,username)
     pinned_posts =list(map(lambda x:posts_.Post(x,model_id,username,"pinned"),pinned_posts ))
+    log.debug(f"[bold]Pinned Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),pinned_posts))}")
+    log.debug("Removing locked pinned media")
     for post in  pinned_posts:
         operations.write_post_table(post,model_id,username)
     output=[]
     [ output.extend(post.media) for post in pinned_posts ]
     return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 def process_profile(headers, username) -> list:
     user_profile = profile.scrape_profile(headers, username)
     urls, info = profile.parse_profile(user_profile)
-    profile.print_profile_info(info)
+    profile.print_profile_info(info)       
     output=[]
     for ele in enumerate(urls):
         count=ele[0]
         data=ele[1]
         output.append(posts_.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
+    avatars=list(filter(lambda x:x.filename=='avatar',output))
+    if len(avatars)>0:
+        log.info(f"Avatar : {avatars[0].url}")
     return output
 
 
 
-
 def process_areas(headers, ele, model_id) -> list:
     args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.areas_prompt())
 ))
     timeline_posts_dicts  = []
     pinned_post_dict=[]
     archived_posts_dicts  = []
     highlights_dicts  = []
@@ -155,58 +184,62 @@
     if ('Timeline' in args.posts or 'All' in args.posts) and ele["active"]:
             timeline_posts_dicts = process_timeline_posts(headers, model_id,username)
     if ('Archived' in args.posts or 'All' in args.posts) and ele["active"]:
             archived_posts_dicts = process_archived_posts(headers, model_id,username)
     if 'Messages' in args.posts or 'All' in args.posts:
             messages_dicts = process_messages(headers, model_id,username)
     if "Purchased" in args.posts or "All" in args.posts:
-            purchased_dict=process_paid_post(headers, model_id,username)
+            purchased_dict=process_paid_post(model_id,username)
     if ('Highlights'  in args.posts or 'Stories'  in args.posts or 'All' in args.posts)   and ele["active"]:
             highlights_tuple = process_highlights(headers, model_id,username)  
             if 'Highlights'  in args.posts:
                 highlights_dicts=highlights_tuple[0]
             if 'Stories'  in args.posts:
                 stories_dicts=highlights_tuple[1]   
             if 'All' in args.posts:
                 highlights_dicts=highlights_tuple[0]
                 stories_dicts=highlights_tuple[1]               
     return posts_filter(list(chain(*[profile_dicts  , timeline_posts_dicts ,pinned_post_dict,purchased_dict,
             archived_posts_dicts , highlights_dicts , messages_dicts,stories_dicts]))
 
 )
 
-def posts_filter(posts):
-    filtersettings=config.read_config()["config"].get('filter')
+def posts_filter(media):
+    filtersettings=config.get_filter(config.read_config())
     output=[]
     ids=set()
-    for post in posts:
-        if not post.id or post.id not in ids:
-            output.append(post)
-            ids.add(post.id)
+    log.info("Removing duplicate media")
+    log.debug(f"[bold]Combined Media Count with dupes[/bold]  {len(media)}")
+    for item in media:
+        if not item.id or item.id not in ids:
+            output.append(item)
+            ids.add(item.id)
+    log.debug(f"[bold]Combined Media Count without dupes[/bold] {len(output)}")
+    output=list(sorted(output,key=lambda x:x.date,reverse=True))
     if isinstance(filtersettings,str):
         filtersettings=filtersettings.split(",")
     if isinstance(filtersettings,list):
         filtersettings=list(map(lambda x:x.lower().replace(" ",""),filtersettings))
         filtersettings=list(filter(lambda x:x!="",filtersettings))
         if len(filtersettings)==0:
-            return posts
-        console.print(f"filtering post to {filtersettings}")
-        return list(filter(lambda x:x.mediatype.lower() in filtersettings,output))
+            return media
+        log.info(f"filtering Media to {','.join(filtersettings)}")
+        output= list(filter(lambda x:x.mediatype.lower() in filtersettings,output))
     else:
-        console.print("The settings you picked for the filter are not valid\nNot Filtering")
-        return output
-        
+        log.info("The settings you picked for the filter are not valid\nNot Filtering")
+        log.debug(f"[bold]Combined Media Count Filtered:[/bold] {len(output)}")
+    return output
 
+        
 
-def do_database_migration():
-    operations.user_db_migration()
 
 
 def get_usernames(parsed_subscriptions: list) -> list:
     usernames = [sub[0] for sub in parsed_subscriptions]
+    log.debug(f"[bold]Usernames on account:[/bold] {usernames}")
     return usernames
 
 
 def get_model(parsed_subscriptions: list) -> tuple:
     """
     Prints user's subscriptions to console and accepts input from user corresponding 
     to the model(s) whose content they would like to scrape.
@@ -216,15 +249,15 @@
   
 def get_model_inputsplit(commaString):
     def hyphenRange(hyphenString):
         x = [int(x) for x in hyphenString.split('-')]
         return range(x[0], x[-1]+1)
     return chain(*[hyphenRange(r) for r in list(filter(lambda x:x.isdigit(),re.split(',| ',commaString)))])
 
-@Halo(text='Getting your subscriptions (this may take awhile)...')
+@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting your subscriptions (this may take awhile)...') 
 def get_models(headers, subscribe_count) -> list:
     """
     Get user's subscriptions in form of a list.
     """
     list_subscriptions = asyncio.run(
         subscriptions.get_subscriptions(headers, subscribe_count))
     parsed_subscriptions = subscriptions.parse_subscriptions(
@@ -242,40 +275,34 @@
 def setfilter():
     if prompts.decide_filters_prompts()=="Yes":
         global args
         args=prompts.modify_filters_prompt(args)
         args_.changeargs(args)
 
 def process_prompts():
-    changeusernames=True
+    
     while  True:
-        args.posts=None
+        args.posts=[]
         result_main_prompt = prompts.main_prompt()
-        if changeusernames and result_main_prompt in [0,1,2]:
-            setfilter()
-            getselected_usernames()
+     
         #download
         if result_main_prompt == 0:
             check_auth()
+            check_config()
             process_post()     
 
         # like a user's posts
         elif result_main_prompt == 1:
             check_auth()
             process_like()
         # Unlike a user's posts
         elif result_main_prompt == 2:
             check_auth()
             process_unlike()
-
-        # elif result_main_prompt == 3:
-        #     # Migrate from old database
-        #     do_database_migration()
         
-
         elif result_main_prompt == 3:
             # Edit `auth.json` file
             auth.edit_auth()
         
         elif result_main_prompt == 4:
             # Edit `config.json` file
             config.edit_config()
@@ -310,156 +337,164 @@
             elif result_profiles_prompt == 3:
                 # Delete a profile
                 profiles.delete_profile()
 
             elif result_profiles_prompt == 4:
                 # View profiles
                 profiles.print_profiles()
-        console.print("Done With Run")
         if prompts.continue_prompt()=="No":
             break
-        global selectedusers
-        if selectedusers:
-            changeusernames=False
-            console.print(f"Currently Selected Users\n{list(map(lambda x:x['name'],selectedusers))}")
-            if prompts.reset_username_prompt()=="Yes":
-                selectedusers=None
-                changeusernames=True
+  
         
 
 
 def process_post():
-    profiles.print_current_profile()
-    headers = auth.make_headers(auth.read_auth())
-    init.print_sign_status(headers)
-    userdata=getselected_usernames()
-    for ele in userdata:
-        print(f"Getting Selected post type(s) for {ele['name']}\nSubscription Active: {ele['active']}")
-        try:
-            model_id = profile.get_id(headers, ele["name"])
-            create_tables(model_id,ele['name'])
-            operations.write_profile_table(model_id,ele['name'])
-            combined_urls=process_areas(headers, ele, model_id)
-            asyncio.run(download.process_dicts(
-            ele["name"],
-            model_id,
-            combined_urls,
-            forced=args.dupe,
-            ))
-        except Exception as e:
-            console.print("run failed with exception: ", e)
-    
-    
+    with scrape_context_manager():
+        profiles.print_current_profile()
+        headers = auth.make_headers(auth.read_auth())
+        init.print_sign_status(headers)
+        userdata=getselected_usernames()
+        for ele in userdata:
+            if args.posts:
+                log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
+            try:
+                model_id = profile.get_id(headers, ele["name"])
+                create_tables(model_id,ele['name'])
+                operations.write_profile_table(model_id,ele['name'])
+                combined_urls=process_areas(headers, ele, model_id)
+                asyncio.run(download.process_dicts(
+                ele["name"],
+                model_id,
+                combined_urls,
+                forced=args.dupe,
+                ))
+            except Exception as e:
+                log.traceback(f"failed with exception: {e}")
+                log.traceback(traceback.format_exc())
+        
+        
 
 def process_like():
-    profiles.print_current_profile()
-    headers = auth.make_headers(auth.read_auth())
-    userdata=getselected_usernames()
-    for ele in list(filter(lambda x: x["active"],userdata)):
-            model_id = profile.get_id(headers, ele["name"])
-            posts = like.get_posts(headers, model_id,ele["name"])
-            unfavorited_posts = like.filter_for_unfavorited(posts)
-            post_ids = like.get_post_ids(unfavorited_posts)
-            like.like(headers, model_id, ele["name"], post_ids)
+    with scrape_context_manager():
+        profiles.print_current_profile()
+        headers = auth.make_headers(auth.read_auth())
+        userdata=getselected_usernames()
+        for ele in list(filter(lambda x: x["active"],userdata)):
+                model_id = profile.get_id(headers, ele["name"])
+                posts = like.get_posts(headers, model_id)
+                unfavorited_posts = like.filter_for_unfavorited(posts)
+                post_ids = like.get_post_ids(unfavorited_posts)
+                like.like(headers, model_id, ele["name"], post_ids)
 
 def process_unlike():
-    profiles.print_current_profile()
-    headers = auth.make_headers(auth.read_auth())
-    init.print_sign_status(headers)
-    userdata=getselected_usernames()
-    for ele in list(filter(lambda x: x["active"],userdata)):
-            model_id = profile.get_id(headers, ele["name"])
-            posts = like.get_posts(headers, model_id,ele['name'])
-            favorited_posts = like.filter_for_favorited(posts)
-            post_ids = like.get_post_ids(favorited_posts)
-            like.unlike(headers, model_id, ele["name"], post_ids)
-
-@contextmanager
-def asuppress_stdout():
-    with open(os.devnull, "w") as devnull:
-        old_stdout = sys.stdout
-        old_stderr=sys.stderr
-        sys.stdout = devnull
-        sys.stderr = devnull
-        try:  
-            yield
-        finally:
-            sys.stdout = old_stdout
-            sys.stderr = old_stderr
-
-def set_schedule(*params):
-    [schedule.every(args.daemon).minutes.do(jobqueue.put,param) for param in params]
+    with scrape_context_manager(): 
+        profiles.print_current_profile()
+        headers = auth.make_headers(auth.read_auth())
+        init.print_sign_status(headers)
+        userdata=getselected_usernames()
+        for ele in list(filter(lambda x: x["active"],userdata)):
+                model_id = profile.get_id(headers, ele["name"])
+                posts = like.get_posts(headers, model_id)
+                favorited_posts = like.filter_for_favorited(posts)
+                post_ids = like.get_post_ids(favorited_posts)
+                like.unlike(headers, model_id, ele["name"], post_ids)
+#Adds a function to the job queue
+def set_schedule(*functs):
+    [schedule.every(args.daemon).minutes.do(jobqueue.put,funct) for funct in functs]
     while True:
         schedule.run_pending()
         time.sleep(30)
 
 
+
 ## run script once or on schedule based on args
-def run(*params):
+def run(*functs):
     # get usernames prior to potentially supressing output
     check_auth()
     getselected_usernames()
-    console.print(f"starting script daemon: {args.daemon!=None} silent-mode: {args.silent}")    
-    if args.silent:
-        with suppress_stdout():
-            run_helper(*params)
-    else:
-        run_helper(*params)
-    console.print("script finished")
+   
+    if args.output=="PROMPT":
+        log.info(f"[bold]silent-mode on[/bold]")    
+    if args.daemon:
+        log.info(f"[bold]daemon mode on[/bold]")   
+    run_helper(*functs)
+
 
-def run_helper(*params):
-    [param() for param in params]    
+def run_helper(*functs):
+    # run each function once
+    [funct() for funct in functs]    
     if args.daemon:
         global jobqueue
         jobqueue=queue.Queue()
-        worker_thread = threading.Thread(target=set_schedule,args=[*params])
+        worker_thread = threading.Thread(target=set_schedule,args=[*functs])
         worker_thread.start()
+        # Check if jobqueue has function
         while True:
             job_func = jobqueue.get()
             job_func()
             jobqueue.task_done()
+            log.debug(schedule.jobs)
                 
 def check_auth():
     status=None
     while status!="UP":
         headers = auth.make_headers(auth.read_auth())
         status=init.getstatus(headers)
         if status=="DOWN":
+            log.error("Auth Failed")
             auth.make_auth(auth=auth.read_auth())
             continue
         break
         
 
-    
+def check_config():
+    while not  paths.mp4decryptchecker(config.get_mp4decrypt(config.read_config())):
+        console.print("You need to select path for mp4decrypt\n\n")
+        log.debug(f"[bold]current mp4decrypt path[/bold] {config.get_mp4decrypt(config.read_config())}")
+        config.update_mp4decrypt()
+    while not  paths.ffmpegchecker(config.get_ffmpeg(config.read_config())):
+        console.print("You need to select path for ffmpeg\n\n")
+        log.debug(f"[bold]current ffmpeg path[/bold] {config.get_ffmpeg(config.read_config())}")
+        config.update_ffmpeg()
+    log.debug(f"[bold]final mp4decrypt path[/bold] {config.get_mp4decrypt(config.read_config())}")
+    log.debug(f"[bold]final ffmpeg path[/bold] {config.get_ffmpeg(config.read_config())}")
+
+
 
        
 
 def getselected_usernames():
     #username list will be retrived once per run
     global selectedusers
     if selectedusers:
-        return selectedusers
-
-    
-    headers = auth.make_headers(auth.read_auth())
-    subscribe_count = process_me(headers)
-    parsed_subscriptions = get_models(headers, subscribe_count)
-    filter_subscriptions=filteruserHelper(parsed_subscriptions )
-    if args.username and "ALL" in args.username:
-        selectedusers=filter_subscriptions
-    
-
-    elif args.username:
-        userSelect=set(args.username)
-        selectedusers=list(filter(lambda x:x["name"] in userSelect,filter_subscriptions))
-    #manually select usernames
+        if len(args.posts)>0:
+            return selectedusers
+        elif prompts.reset_username_prompt()=="No":
+           return selectedusers
+        else:
+            setfilter()
     else:
-        selectedusers= get_model(filter_subscriptions)
-    #remove dupes
-    return selectedusers
+        if len(args.posts)==0:
+            setfilter()
+        headers = auth.make_headers(auth.read_auth())
+        subscribe_count = process_me(headers)
+        parsed_subscriptions = get_models(headers, subscribe_count)
+        filter_subscriptions=filteruserHelper(parsed_subscriptions )
+        if args.username and "ALL" in args.username:
+            selectedusers=filter_subscriptions
+        
+
+        elif args.username:
+            userSelect=set(args.username)
+            selectedusers=list(filter(lambda x:x["name"] in userSelect,filter_subscriptions))
+        #manually select usernames
+        else:
+            selectedusers= get_model(filter_subscriptions)
+        #remove dupes
+        return selectedusers
 def filteruserHelper(usernames):
     #paid/free
     filterusername=usernames
     if args.account_type=="paid":
         filterusername=list(filter(lambda x:x["data"]["subscribePrice"]>0,filterusername))
     if args.account_type=="free":
         filterusername=list(filter(lambda x:x["data"]["subscribePrice"]==0,filterusername))
@@ -479,65 +514,79 @@
     operations.create_message_table(model_id,username)
     operations.create_media_table(model_id,username)
     operations.create_products_table(model_id,username)
     operations.create_others_table(model_id,username)
     operations.create_profile_table(model_id,username)
     operations.create_stories_table(model_id,username)
 
+
+
 @contextmanager
-def suppress_stdout():
-    with open(os.devnull, "w") as devnull:
-        old_stdout = sys.stdout
-        old_stderr=sys.stderr
-        sys.stdout = devnull
-        sys.stderr = devnull
-        try:  
-            yield
-        finally:
-            sys.stdout = old_stdout
-            sys.stderr = old_stderr
+def scrape_context_manager():
+        
+        # Before yield as the enter method
 
-args=args_.getargs()
+        start = timeit.default_timer()
+        log.error(
+f"""
+==============================                            
+[bold]starting script[/bold]
+==============================
+"""
+    
+
+    )
+        yield
+        end=timeit.default_timer()
+        log.error(f"""
+===========================
+[bold]Script Finished[/bold]
+Run Time:  [bold]{str(arrow.get(end)-arrow.get(start)).split(".")[0]}[/bold]
+===========================
+""")
+        None   
 def main():
+    
+# Python program for creating a
+# context manager using @contextmanager
+# decorator
+ 
     with exit.DelayedKeyboardInterrupt(paths.cleanup,False):
         try:
+ 
             scrapper()
+
+            
+
         except Exception as E:
-            None
-            # console.print(E)
-            # console.print(traceback.format_exc(), style="white")
+            log.traceback(E)
+            log.traceback(traceback.format_exc())
         quit()
 def scrapper():
     if platform.system == 'Windows':
         os.system('color')
     # try:
     #     webbrowser.open(donateEP)
     # except:
     #     pass
     global selectedusers
     selectedusers=None
-
-
-    
-    if len(list(filter(lambda x:x!=None and x!=False,[args.action,args.posts])))==0:
+    functs=[]
+    if len(args.posts)==0 and not args.action:
         if args.daemon:
-            console.print("You need to pass at least one scraping method\n--action\n--posts\n--purchase\nAre all valid options. Skipping and going to menu")
+                    log.warning("You need to pass at least one scraping method\n--action\n--posts\n--purchase\nAre all valid options. Skipping and going to menu")
         process_prompts()
-        sys.exit(0)
-    
-
-
-
-    if args.posts: 
-        check_auth()
-        run(process_post)        
-    if args.action=="like":
-        check_auth()
-        run(process_like)
-    if args.action=="unlike":
-        check_auth()    
-        run(process_unlike)  
+        return
+    check_auth()
+    check_config()
+    if len(args.posts)>0: 
+        functs.append(process_post)      
+    elif args.action=="like":
+        functs.append(process_like)
+    elif args.action=="unlike":
+        functs.append(process_unlike)
+    run(*functs)  
+  
+       
 
-if __name__ == '__main__':
-    main()
```

### Comparing `ofscraper-1.87/src/utils/args.py` & `ofscraper-1.95/ofscraper/utils/args.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 import argparse
-from src.__version__ import  __version__
+import logging
 import sys
+import pkg_resources
+from ofscraper.__version__ import __version__ 
+
+args=None
+log=logging.getLogger(__package__)
 def getargs(input=None):
     global args
     if args and input==None:
         return args
-    if input==None:
+    if "pytest" in sys.modules and input==None:
+        input=[]
+    elif input==None:
         input=sys.argv[1:]
 
     parser = argparse.ArgumentParser()
 
     parser = argparse.ArgumentParser(add_help=False)   
     general=parser.add_argument_group("General",description="General Args")  
-    general.add_argument('-v', '--version', action='version', version='%(prog)s ' + __version__)
+    general.add_argument('-v', '--version', action='version', version=__version__ )
     general.add_argument('-h', '--help', action='help')
 
                                     
     general.add_argument(
         '-u', '--username', help="select which username to process (name,name2)\nSet to ALL for all users",type=lambda x: list(filter( lambda y:y!="",x.split(",")))
     )
     general.add_argument(
         '-d', '--daemon', help='run script in the background\nSet value to minimum minutes between script runs\nOverdue runs will run as soon as previous run finishes', type=int,default=None
     )
+
+    general.add_argument(
+        '-l', '--log', help = 'set log file level', type=str.upper,default="OFF",choices=["OFF","LOW","NORMAL","DEBUG"]
+    ),
     general.add_argument(
-        '-s', '--silent', help = 'mute output', action = 'store_true',default=False
+        '-dc', '--discord', help = 'set discord log level', type=str.upper,default="OFF",choices=["OFF","LOW","NORMAL","DEBUG"]
     )
+
     general.add_argument(
-        '-l', '--log', help = 'set log level', type=str.upper,default=None,choices=["OFF","INFO","DEBUG"]
+        '-p', '--output', help = 'set output log level', type=str.upper,default="NORMAL",choices=["PROMPT","LOW","NORMAL","DEBUG"]
     )
     post=parser.add_argument_group("Post",description="What type of post to scrape")                                      
 
     post.add_argument("-e","--dupe",action="store_true",default=False,help="Bypass the dupe check and redownload all files")
     post.add_argument(
-        '-o', '--posts', help = 'Download content from a models wall',default=None,required=False,type = str.lower,choices=["highlights","all","archived","messages","timeline","pinned","stories","purchased",],action='append'
+        '-o', '--posts', help = 'Download content from a model',default=[],required=False,type = posttype_helper,action='extend'
     )
     post.add_argument("-c","--letter-count",action="store_true",default=False,help="intrepret config 'textlength' as max length by letter")
     post.add_argument("-a","--action",default=None,help="perform like or unlike action on each post",choices=["like","unlike"])
      #Filters for accounts
     filters=parser.add_argument_group("filters",description="Filters out usernames based on selected parameters")
     
     filters.add_argument(
@@ -44,16 +56,26 @@
     )
     filters.add_argument(
         '-r', '--renewal', help = 'Filter by whether renewal is on or off for account',default=None,required=False,type = str.lower,choices=["active","disabled"]
     )
     filters.add_argument(
         '-ss', '--sub-status', help = 'Filter by whether or not your subscription has expired or not',default=None,required=False,type = str.lower,choices=["active","expired"]
     )
-    
+
     args=parser.parse_args(input)
+    #deduplicate posts
+    args.posts=list(set(args.posts or []))
     return args
-args=None
+
+
+    
+def posttype_helper(x):
+    choices=set(["highlights","all","archived","messages","timeline","pinned","stories","purchased"])
+    if isinstance(x,str):
+        x=x.split(',')
+    if len(list(filter(lambda y:y not in choices,x)))>0:
+        raise argparse.ArgumentTypeError("error: argument -o/--posts: invalid choice: 'timeline,messages,purchased' (choose from 'highlights', 'all', 'archived', 'messages', 'timeline', 'pinned', 'stories', 'purchased')")
+    return x
+
 def changeargs(newargs):
     global args
     args=newargs
-    
-
```

### Comparing `ofscraper-1.87/src/utils/auth.py` & `ofscraper-1.95/ofscraper/utils/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 import hashlib
 import json
 import pathlib
 import time
 from urllib.parse import urlparse
 import requests
 from rich.console import Console
-console=Console()
 import httpx
 import browser_cookie3
 from .profiles import get_current_profile
-from ..prompts.prompts import auth_prompt, ask_make_auth_prompt,browser_prompt,\
-user_agent_prompt,xbc_prompt,auth_full_paste,manual_auth_prompt
+from ..prompts.prompts import *
 from ..constants import configPath, authFile, DC_EP, requestAuth
 
+console=Console()
+
 
 
 def read_auth():
     make_request_auth()
 
     profile = get_current_profile()
 
@@ -176,15 +176,20 @@
 
     auth_uid = 'auth_uid_{}'.format(auth['auth']['auth_id'])
 
     client.cookies.set('sess', auth['auth']['sess'], domain=domain)
     client.cookies.set('auth_id', auth['auth']['auth_id'], domain=domain)
     if auth['auth']['auth_uid_']:
         client.cookies.set(auth_uid, auth['auth']['auth_uid_'], domain=domain)
-
+def get_cookies():
+    profile = get_current_profile()
+    p = pathlib.Path.home() / configPath / profile
+    with open(p / authFile, 'r') as f:
+        auth = json.load(f)
+    return  f"auth_id={auth['auth']['auth_id']};sess={auth['auth']['sess']};"
 
 def create_sign(link, headers):
     """
     credit: DC and hippothon
     """
     content = read_request_auth()
```

### Comparing `ofscraper-1.87/src/utils/dates.py` & `ofscraper-1.95/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.87/src/utils/encoding.py` & `ofscraper-1.95/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.87/src/utils/exit.py` & `ofscraper-1.95/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.87/src/utils/profiles.py` & `ofscraper-1.95/ofscraper/utils/profiles.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,44 +8,44 @@
                  \/     \/           \/            \/         
 """
 
 import pathlib
 import shutil
 from rich.console import Console
 from rich import print
+import ofscraper.utils.config as config_
+import ofscraper.prompts.prompts as prompts
+import ofscraper.constants as constants
+
 console=Console()
-from .config import read_config, update_config
-from ..prompts.prompts import get_profile_prompt,change_default_profile
-from ..constants import configPath, configFile, mainProfile
-configPath = '.config/ofscraper'
 
 
 def get_profile_path():
-    config_path = pathlib.Path.home() / configPath
+    config_path = pathlib.Path.home() / constants.configPath
     return config_path
 
 
 def get_profiles() -> list:
     config_path = get_profile_path()
     dir_contents = config_path.glob('*')
     profiles = [item for item in dir_contents if item.is_dir()]
     return profiles
 
 def change_profile():
     console.print('Current profiles:')
-    profile = get_profile_prompt(print_profiles())
+    profile = prompts.get_profile_prompt(print_profiles())
 
-    update_config(mainProfile, profile)
+    config_.update_config(constants.mainProfile, profile)
 
     print(f'[green]Successfully changed profile to[/green] {profile}')
 
 
 def delete_profile():
     console.print('Current profiles:')
-    profile = get_profile_prompt(print_profiles())
+    profile = prompts.get_profile_prompt(print_profiles())
 
     if profile == get_current_profile():
         raise OSError(
             'You cannot delete a profile that you\'re currently using')
 
     p = get_profile_path() / profile
     shutil.rmtree(p)
@@ -54,29 +54,29 @@
 
 
 def create_profile(path, dir_name: str):
     dir_path = path / dir_name
 
     if not dir_path.is_dir():
         dir_path.mkdir(parents=True, exist_ok=False)
-    if change_default_profile()=="Yes":
-        update_config(mainProfile, dir_name)
+    if prompts.change_default_profile()=="Yes":
+        config_.update_config(constants.mainProfile, dir_name)
     console.print('[green]Successfully created[/green] {dir_name}'.format(dir_name=dir_name))
     
 
 def edit_profile_name(old_profile_name: str, new_profile_name: str):
     profiles = get_profiles()
 
     for profile in profiles:
         if profile.stem == old_profile_name:
             profile.replace(profile.parent / new_profile_name)
             shutil.rmtree(profile,ignore_errors=True)
            
     if old_profile_name == get_current_profile():
-        update_config(mainProfile, new_profile_name)
+        config_.update_config(constants.mainProfile, new_profile_name)
 
     print(
         f"[green]Successfully changed[green] '{old_profile_name}' to '{new_profile_name}'")
 
 
 def print_profiles() -> list:
     profile_names = [profile.stem for profile in get_profiles()]
@@ -85,16 +85,16 @@
     for name in profile_names:
         console.print(profile_fmt.format(name))
 
     return profile_names
 
 
 def get_current_profile():
-    config = read_config()
-    return config['config'][mainProfile]
+    config = config_.read_config()
+    return config[constants.mainProfile]
 
 
 def print_current_profile():
     get_profiles()
 
     current_profile = get_current_profile()
     print('Using profile: [cyan]{}[/cyan]'.format(current_profile))
```

### Comparing `ofscraper-1.87/src/utils/separate.py` & `ofscraper-1.95/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.87/PKG-INFO` & `ofscraper-1.95/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.87
+Version: 1.95
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: browser-cookie3 (>=0.17.1,<0.18.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: diskcache (>=5.6.1,<6.0.0)
+Requires-Dist: dunamai (>=1.17.0,<2.0.0)
+Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: httpx[http2] (>=0.23.3,<0.24.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
+Requires-Dist: mpegdash (>=0.3.1,<0.4.0)
 Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
@@ -40,37 +44,15 @@
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
         This is a theoritical program only and is for educational purposes. If you choose to use it then it may or may not work. You solely accept full responsability and indemnify the creator, hostors, contributors and all other involved persons from any any all responsability.
     </li>
 
- ## 1.8x Changes:
- - sync keys names across config(old keys will still work)
-  * change username to model_username in metadata
-  * change site_name to sitename in metadata
- - remove --purchased args
- - add purchase and pinned as post types
- - add letter-count argument
-   * This is for counting letters and not words for
-   textlength
- - added testing 
-    * to install run poetry install --with test 
-    * run with poetry run pytest
- - print path for each file
- - responsetype mapping in config
-    * This is for example keeping all messages or paid post in same folder, but also allow long time users to keep their current structure
- - added a Post class to serve as a 'single source of truth' for all responsetypes
- - removed unused functions like download_paid that are no longer needed
- - prompts and config functions have been revamped
- - shutdown handler
- - removed .tempmedia
- - added extension to responsetype profile downloads
- - fixed bugs caused by duplicate uploads on pages
- - additional bugs and fixes
+
 
   ## Description:
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
 
@@ -156,26 +138,35 @@
  
  # commandline
  While the menu is easy to use, and convient. You may want more automation.
  
  The best way to do this is through the commandline system. This will allow you to skip the menu, and for example scrape a provided list of accounts
  
   https://github.com/datawhores/ofscraper/wiki/command-line-args
+
+# Docker Support
+https://github.com/datawhores/ofscraper/pkgs/container/ofscraper
  
  # Customazation
     
 https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
 https://github.com/datawhores/ofscraper/wiki/Config-Options
 
   
 # Issues
 Open a issue in this repo, or you can mention your issue in the discord
 
 https://discord.gg/wN7uxEVHRK
     
+# Feature Requests
+
+https://ofscraper.clearflask.com/feedback
+    
+Or the discord
+    
     
 ## Common
 ### Status Down
       
 This typically means that your auth information is not correct, or onlyfans signed you out.
 ### 404 Issue
```

