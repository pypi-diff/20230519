# Comparing `tmp/ofscraper-1.86.tar.gz` & `tmp/ofscraper-1.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.86.tar", max compression
+gzip compressed data, was "ofscraper-1.87.tar", max compression
```

## Comparing `ofscraper-1.86.tar` & `ofscraper-1.87.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.86/LICENSE
--rw-r--r--   0        0        0     5800 2023-04-29 01:50:36.060807 ofscraper-1.86/README.md
--rw-r--r--   0        0        0     1235 2023-04-29 22:25:20.860303 ofscraper-1.86/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.86/src/__init__.py
--rw-r--r--   0        0        0      733 2023-04-29 22:25:20.860303 ofscraper-1.86/src/__version__.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.86/src/api/__init__.py
--rw-r--r--   0        0        0     2195 2023-04-29 21:06:53.651540 ofscraper-1.86/src/api/highlights.py
--rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.86/src/api/init.py
--rw-r--r--   0        0        0     1841 2023-04-29 21:06:53.652540 ofscraper-1.86/src/api/me.py
--rw-r--r--   0        0        0     3598 2023-04-29 21:06:53.652540 ofscraper-1.86/src/api/messages.py
--rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.86/src/api/paid.py
--rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.86/src/api/posts.py
--rw-r--r--   0        0        0     3273 2023-04-29 21:06:53.652540 ofscraper-1.86/src/api/profile.py
--rw-r--r--   0        0        0     2058 2023-04-29 21:06:53.652540 ofscraper-1.86/src/api/subscriptions.py
--rw-r--r--   0        0        0     5474 2023-04-29 21:06:53.652540 ofscraper-1.86/src/api/timeline.py
--rw-r--r--   0        0        0     4793 2023-04-29 21:06:53.652540 ofscraper-1.86/src/constants.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.86/src/db/__init__.py
--rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.86/src/db/operations.py
--rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.86/src/db/queries.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.86/src/interaction/__init__.py
--rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.86/src/interaction/like.py
--rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.86/src/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.86/src/prompts/prompt_strings.py
--rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.86/src/prompts/prompts.py
--rwxr-xr-x   0        0        0    19182 2023-04-29 22:26:06.685815 ofscraper-1.86/src/scraper.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.86/src/utils/__init__.py
--rw-r--r--   0        0        0     2864 2023-04-29 21:06:53.652540 ofscraper-1.86/src/utils/args.py
--rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.86/src/utils/auth.py
--rw-r--r--   0        0        0     8945 2023-04-29 21:06:53.652540 ofscraper-1.86/src/utils/config.py
--rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.86/src/utils/dates.py
--rw-r--r--   0        0        0    11237 2023-04-29 21:54:25.606047 ofscraper-1.86/src/utils/download.py
--rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.86/src/utils/encoding.py
--rw-r--r--   0        0        0     2938 2023-04-29 01:50:36.061807 ofscraper-1.86/src/utils/exit.py
--rw-r--r--   0        0        0     1027 2023-04-29 22:23:00.769846 ofscraper-1.86/src/utils/logger.py
--rw-r--r--   0        0        0     3004 2023-04-29 21:06:53.652540 ofscraper-1.86/src/utils/paths.py
--rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.86/src/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.86/src/utils/separate.py
--rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 ofscraper-1.86/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.87/LICENSE
+-rw-r--r--   0        0        0     6024 2023-04-30 01:57:35.320013 ofscraper-1.87/README.md
+-rw-r--r--   0        0        0     1235 2023-04-30 15:56:33.941101 ofscraper-1.87/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.87/src/__init__.py
+-rw-r--r--   0        0        0      733 2023-04-30 15:56:33.941101 ofscraper-1.87/src/__version__.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.87/src/api/__init__.py
+-rw-r--r--   0        0        0     2195 2023-04-29 21:06:53.651540 ofscraper-1.87/src/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.87/src/api/init.py
+-rw-r--r--   0        0        0     1841 2023-04-29 21:06:53.652540 ofscraper-1.87/src/api/me.py
+-rw-r--r--   0        0        0     3598 2023-04-29 21:06:53.652540 ofscraper-1.87/src/api/messages.py
+-rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.87/src/api/paid.py
+-rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.87/src/api/posts.py
+-rw-r--r--   0        0        0     3273 2023-04-29 21:06:53.652540 ofscraper-1.87/src/api/profile.py
+-rw-r--r--   0        0        0     2058 2023-04-29 21:06:53.652540 ofscraper-1.87/src/api/subscriptions.py
+-rw-r--r--   0        0        0     5474 2023-04-29 21:06:53.652540 ofscraper-1.87/src/api/timeline.py
+-rw-r--r--   0        0        0     4793 2023-04-29 21:06:53.652540 ofscraper-1.87/src/constants.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.87/src/db/__init__.py
+-rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.87/src/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.87/src/db/queries.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.87/src/interaction/__init__.py
+-rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.87/src/interaction/like.py
+-rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.87/src/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.87/src/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.87/src/prompts/prompts.py
+-rwxr-xr-x   0        0        0    19166 2023-04-30 01:56:48.978541 ofscraper-1.87/src/scraper.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.87/src/utils/__init__.py
+-rw-r--r--   0        0        0     2864 2023-04-29 21:06:53.652540 ofscraper-1.87/src/utils/args.py
+-rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.87/src/utils/auth.py
+-rw-r--r--   0        0        0     8945 2023-04-29 21:06:53.652540 ofscraper-1.87/src/utils/config.py
+-rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.87/src/utils/dates.py
+-rw-r--r--   0        0        0    11230 2023-04-30 02:09:39.647464 ofscraper-1.87/src/utils/download.py
+-rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.87/src/utils/encoding.py
+-rw-r--r--   0        0        0     2938 2023-04-29 01:50:36.061807 ofscraper-1.87/src/utils/exit.py
+-rw-r--r--   0        0        0     1142 2023-04-30 01:53:48.669716 ofscraper-1.87/src/utils/logger.py
+-rw-r--r--   0        0        0     3004 2023-04-29 21:06:53.652540 ofscraper-1.87/src/utils/paths.py
+-rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.87/src/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.87/src/utils/separate.py
+-rw-r--r--   0        0        0     7233 1970-01-01 00:00:00.000000 ofscraper-1.87/PKG-INFO
```

### Comparing `ofscraper-1.86/LICENSE` & `ofscraper-1.87/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/README.md` & `ofscraper-1.87/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,32 +47,47 @@
 
 ## Installation
 
 ### Recommended python3.9 or python3.10
 
 
 # Windows: 
+## stable
 ```
 pip install ofscraper
 ```
 or 
-
+## development
 ```
 pip install git+https://github.com/datawhores/ofscraper.git 
 ```
+or 
+## specific version
+```
+pip install ofscraper==x
+```
+where x is the vesion you want to install
+
 
 #  macOS/Linux
 ```
 pip3 install ofscraper
 ```
 or
 ```
 pip3 install git+https://github.com/datawhores/ofscraper.git 
 ```
 
+or 
+## specific version
+```
+pip install ofscraper==x
+```
+where x is the vesion you want to install
+
 ## Authentication
 
 You'll need to retrive your auth information 
     
 https://github.com/datawhores/ofscraper/wiki/Auth
```

### Comparing `ofscraper-1.86/pyproject.toml` & `ofscraper-1.87/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.86"
+version = "1.87"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
```

### Comparing `ofscraper-1.86/src/__init__.py` & `ofscraper-1.87/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/__version__.py` & `ofscraper-1.87/src/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/       
 """
 
 __title__ = 'ofscraper'
-__version__ = '1.86'
+__version__ = '1.87'
 __author__ = 'datawhores'
 __author_email__ = 'datawhores@riseup.net'
 __description__ = 'A command-line program to quickly download,like or unlike posts, and more'
 __url__ = 'https://github.com/datawhores/ofscraper'
 __license__ = 'GNU General Public License v3 or later (GPLv3+)'
 __copyright__ = 'Copyright 2023'
```

### Comparing `ofscraper-1.86/src/api/highlights.py` & `ofscraper-1.87/src/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/api/init.py` & `ofscraper-1.87/src/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/api/me.py` & `ofscraper-1.87/src/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/api/messages.py` & `ofscraper-1.87/src/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/api/paid.py` & `ofscraper-1.87/src/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/api/posts.py` & `ofscraper-1.87/src/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/api/profile.py` & `ofscraper-1.87/src/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/api/subscriptions.py` & `ofscraper-1.87/src/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/api/timeline.py` & `ofscraper-1.87/src/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/constants.py` & `ofscraper-1.87/src/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/db/operations.py` & `ofscraper-1.87/src/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/db/queries.py` & `ofscraper-1.87/src/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/interaction/like.py` & `ofscraper-1.87/src/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/prompts/prompt_functions.py` & `ofscraper-1.87/src/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/prompts/prompts.py` & `ofscraper-1.87/src/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/scraper.py` & `ofscraper-1.87/src/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     urls, info = profile.parse_profile(user_profile)
     profile.print_profile_info(info)
     output=[]
     for ele in enumerate(urls):
         count=ele[0]
         data=ele[1]
         output.append(posts_.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
-    reexcludedBittern8turn output
+    return output
 
 
 
 
 def process_areas(headers, ele, model_id) -> list:
     args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.areas_prompt())
 ))
```

### Comparing `ofscraper-1.86/src/utils/args.py` & `ofscraper-1.87/src/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/utils/auth.py` & `ofscraper-1.87/src/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/utils/config.py` & `ofscraper-1.87/src/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/utils/dates.py` & `ofscraper-1.87/src/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/utils/download.py` & `ofscraper-1.87/src/utils/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,20 +35,19 @@
 from .separate import separate_by_id
 from ..db import operations
 from .paths import set_directory,getmediadir
 from ..utils import auth
 from ..constants import NUM_TRIES,FILE_FORMAT_DEFAULT,DATE_DEFAULT,TEXTLENGTH_DEFAULT,FILE_SIZE_DEFAULT
 from ..utils.profiles import get_current_profile
 from .dates import convert_local_time
-import logging
 attempt = contextvars.ContextVar("attempt")
 
 config = read_config()['config']
 import src.utils.logger as logger
-log=logger.log
+log=logger.getlogger()
 
 
 async def process_dicts(username, model_id, medialist,forced=False):
     if medialist:
         if not forced:
             media_ids = set(operations.get_media_ids(model_id,username))
             medialist = separate_by_id(medialist, media_ids)
```

### Comparing `ofscraper-1.86/src/utils/encoding.py` & `ofscraper-1.87/src/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/utils/exit.py` & `ofscraper-1.87/src/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/utils/logger.py` & `ofscraper-1.87/src/utils/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,20 @@
         s=re.sub("&Signature=[^&]+", "&Signature={hidden}", s)
         s=re.sub("&Key-Pair-Id=[^&]+", "&Key-Pair-Id={hidden}", s)
         return s
 
     def format(self, record):
         original = logging.Formatter.format(self, record)  # call parent method
         return self._filter(original)
-log=logging.getLogger("ofscraper")
-log.setLevel(args_.getargs().log or 100)
-fh=logging.FileHandler(paths.getlogpath(),mode="a")
-fh.setLevel(args_.getargs().log or 100)
-formatter = SensitiveFormatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s',"%Y-%m-%d %H:%M:%S")
-fh.setFormatter(formatter)
-log.addHandler(fh)
+log=None
+def getlogger():
+    global log
+    if log:
+        return log
+    log=logging.getLogger("ofscraper")
+    log.setLevel(args_.getargs().log or 100)
+    fh=logging.FileHandler(paths.getlogpath(),mode="a")
+    fh.setLevel(args_.getargs().log or 100)
+    formatter = SensitiveFormatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s',"%Y-%m-%d %H:%M:%S")
+    fh.setFormatter(formatter)
+    log.addHandler(fh)
+    return log
```

### Comparing `ofscraper-1.86/src/utils/paths.py` & `ofscraper-1.87/src/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/utils/profiles.py` & `ofscraper-1.87/src/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/src/utils/separate.py` & `ofscraper-1.87/src/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.86/PKG-INFO` & `ofscraper-1.87/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.86
+Version: 1.87
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -78,32 +78,47 @@
 
 ## Installation
 
 ### Recommended python3.9 or python3.10
 
 
 # Windows: 
+## stable
 ```
 pip install ofscraper
 ```
 or 
-
+## development
 ```
 pip install git+https://github.com/datawhores/ofscraper.git 
 ```
+or 
+## specific version
+```
+pip install ofscraper==x
+```
+where x is the vesion you want to install
+
 
 #  macOS/Linux
 ```
 pip3 install ofscraper
 ```
 or
 ```
 pip3 install git+https://github.com/datawhores/ofscraper.git 
 ```
 
+or 
+## specific version
+```
+pip install ofscraper==x
+```
+where x is the vesion you want to install
+
 ## Authentication
 
 You'll need to retrive your auth information 
     
 https://github.com/datawhores/ofscraper/wiki/Auth
```

