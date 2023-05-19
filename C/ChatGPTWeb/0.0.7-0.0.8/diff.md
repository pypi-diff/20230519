# Comparing `tmp/ChatGPTWeb-0.0.7.tar.gz` & `tmp/ChatGPTWeb-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatGPTWeb-0.0.7.tar", last modified: Thu Apr 13 13:57:48 2023, max compression
+gzip compressed data, was "ChatGPTWeb-0.0.8.tar", last modified: Fri May 19 06:22:32 2023, max compression
```

## Comparing `ChatGPTWeb-0.0.7.tar` & `ChatGPTWeb-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:57:48.296762 ChatGPTWeb-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-04-13 13:57:48.291762 ChatGPTWeb-0.0.7/ChatGPTWeb/
--rw-rw-rw-   0        0        0    19656 2023-04-13 13:57:22.000000 ChatGPTWeb-0.0.7/ChatGPTWeb/ChatGPTWeb.py
--rw-rw-rw-   0        0        0       56 2023-04-08 08:59:30.000000 ChatGPTWeb-0.0.7/ChatGPTWeb/__init__.py
--rw-rw-rw-   0        0        0     1958 2023-04-13 13:41:31.000000 ChatGPTWeb-0.0.7/ChatGPTWeb/__main__.py
--rw-rw-rw-   0        0        0     6288 2023-04-13 13:35:36.000000 ChatGPTWeb-0.0.7/ChatGPTWeb/config.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:57:48.294762 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/
--rw-rw-rw-   0        0        0     3516 2023-04-13 13:57:48.000000 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-04-13 13:57:48.000000 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:57:48.000000 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-13 13:57:48.000000 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-13 13:57:48.000000 ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-04-07 06:03:43.000000 ChatGPTWeb-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3516 2023-04-13 13:57:48.295763 ChatGPTWeb-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3161 2023-04-13 13:42:59.000000 ChatGPTWeb-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 13:57:48.296762 ChatGPTWeb-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-04-13 13:57:32.000000 ChatGPTWeb-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:22:32.237189 ChatGPTWeb-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-05-19 06:22:32.232193 ChatGPTWeb-0.0.8/ChatGPTWeb/
+-rw-rw-rw-   0        0        0    23949 2023-05-19 06:02:57.000000 ChatGPTWeb-0.0.8/ChatGPTWeb/ChatGPTWeb.py
+-rw-rw-rw-   0        0        0       56 2023-04-08 08:59:30.000000 ChatGPTWeb-0.0.8/ChatGPTWeb/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-05-19 06:20:46.000000 ChatGPTWeb-0.0.8/ChatGPTWeb/__main__.py
+-rw-rw-rw-   0        0        0     6418 2023-05-19 06:18:09.000000 ChatGPTWeb-0.0.8/ChatGPTWeb/config.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:22:32.235190 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/
+-rw-rw-rw-   0        0        0     3516 2023-05-19 06:22:32.000000 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-19 06:22:32.000000 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 06:22:32.000000 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-19 06:22:32.000000 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-19 06:22:32.000000 ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-04-07 06:03:43.000000 ChatGPTWeb-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3516 2023-05-19 06:22:32.236191 ChatGPTWeb-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3161 2023-04-13 13:42:59.000000 ChatGPTWeb-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 06:22:32.237189 ChatGPTWeb-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      660 2023-05-19 06:21:44.000000 ChatGPTWeb-0.0.8/setup.py
```

### Comparing `ChatGPTWeb-0.0.7/ChatGPTWeb/__main__.py` & `ChatGPTWeb-0.0.8/ChatGPTWeb/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from ChatGPTWeb.ChatGPTWeb import chatgpt
-from ChatGPTWeb.config import MsgData,Personality
-import asyncio
-import aioconsole
-
-# from ChatGPTWeb import chatgpt
-# from config import MsgData,Personality
+# from ChatGPTWeb.ChatGPTWeb import chatgpt
+# from ChatGPTWeb.config import MsgData,Personality
 # import asyncio
 # import aioconsole
 
-session_token=["sessiton_token_one",
-               "sessiton_token_two",
+from ChatGPTWeb import chatgpt
+from config import MsgData,Personality
+import asyncio
+import aioconsole
+
+session_token=[
+    "eyJhbGciOiJkaXIiLCJlbmMiOiJBMjU2R0NNIn0..",
+    "eyJhbGciOiJkaXIiLCJlbmMiOiJBMjU2R0NNIn0.."
 ]
 
 personality_definition = Personality(
     [
         {
             "name":"one",
             'value':'one value'
```

### Comparing `ChatGPTWeb-0.0.7/ChatGPTWeb/config.py` & `ChatGPTWeb-0.0.8/ChatGPTWeb/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import uuid
 import json
 import logging
 from typing import TypedDict,Optional,Literal,List,Dict
 
 url_session = "https://chat.openai.com/api/auth/session"
 url_chatgpt = "https://chat.openai.com:443/backend-api/conversation"
+url_check = "https://chat.openai.com/api/auth/session"
 
 formator = logging.Formatter(fmt = "%(asctime)s %(filename)s %(levelname)s %(message)s",datefmt="%Y/%m/%d %X")
 
 
 class Personality:
     def __init__(self, init_list: List[Dict[str, str]]):
         self.init_list = []
@@ -20,16 +21,16 @@
        
     
     def show_name(self):
         name = [f"{index+1}. {x.get('name')}" for index,x in enumerate(self.init_list)]
         return '\n'.join(name)
     
     
-    def get_value_by_name(self, name: str):
-        return next((x.get("value") for x in self.init_list if x.get("name") == name), None)
+    def get_value_by_name(self, name: str) -> str:
+        return next((x.get("value") for x in self.init_list if x.get("name") == name), "")
     
     def add_dict_to_list(self, new_dict: dict):
         self.init_list.append(new_dict)
         
     def save_data(self):
         tmp = '\n'.join([json.dumps(x) for x in self.init_list])
         try:
@@ -100,19 +101,23 @@
         self.msg_recv = msg_recv
         self.conversation_id = conversation_id
         self.p_msg_id = p_msg_id
         self.next_msg_id = next_msg_id
         self.post_data = post_data
         
 class Payload():
+
+
+
     @staticmethod
     def new_payload(prompt: str) -> str:
         return json.dumps({
             "action":
             "next",
+            "history_and_training_disabled":False,
             "messages": [{
                 "id": str(uuid.uuid4()),
                 "author": {
                     "role": "user"
                 },
                 "content": {
                     "content_type": "text",
@@ -127,14 +132,15 @@
             -480
         })
     @staticmethod
     def old_payload(prompt: str,conversation_id: str,p_msg_id: str) -> str:
         return json.dumps({
             "action":
             "next",
+            "history_and_training_disabled":False,
             "messages": [{
                 "id": str(uuid.uuid4()),
                 "author": {
                     "role": "user"
                 },
                 "content": {
                     "content_type": "text",
@@ -150,29 +156,29 @@
             "timezone_offset_min":
             -480
         })
     @staticmethod
     def headers(token: str,data: str):
         return {
             "Host": "chat.openai.com",
-            "User-Agent":
-            "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/109.0",
             "Accept": "text/event-stream",
-            "Accept-Language": "en-US,en;q=0.5",
-            "Accept-Encoding": "gzip, deflate, br",
+            "Accept-Language": "zh-CN,zh;q=0.9",
+            "Accept-Encoding": "gzip, deflate",
             "Content-Type": "application/json",
             "Content-Length": str(len(str(data))),
-            "Referer": "https://chat.openai.com/chat",
+            "Referer": "https://chat.openai.com/",
             "Authorization": f"Bearer {token}",
             "Origin": "https://chat.openai.com",
             "Connection": "keep-alive",
+            "sec-ch-ua-mobile": "?0",
+            #"sec-ch-ua-platform": "\"Windows\"", 
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
-            "Sec-Fetch-Site": "same-origin",
-            "TE": "trailers"
+            "Sec-Fetch-Site": "same-origin"
+            #"TE": "trailers"
         }
         
     @staticmethod        
     def system_new_payload(prompt: str) -> str:
         return json.dumps({
             "action":
             "next",
```

### Comparing `ChatGPTWeb-0.0.7/ChatGPTWeb.egg-info/PKG-INFO` & `ChatGPTWeb-0.0.8/ChatGPTWeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTWeb
-Version: 0.0.7
+Version: 0.0.8
 Summary: a ChatGPT API,no web ui
 Home-page: https://github.com/nek0us/ChatGPT
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `ChatGPTWeb-0.0.7/LICENSE` & `ChatGPTWeb-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.7/PKG-INFO` & `ChatGPTWeb-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTWeb
-Version: 0.0.7
+Version: 0.0.8
 Summary: a ChatGPT API,no web ui
 Home-page: https://github.com/nek0us/ChatGPT
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `ChatGPTWeb-0.0.7/README.md` & `ChatGPTWeb-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.7/setup.py` & `ChatGPTWeb-0.0.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from setuptools import setup, find_packages 
 
 with open("README.md", "r",encoding="utf8") as readme_file:
     readme = readme_file.read()
 
-requirements = ["playwright","aioconsole"] # 这里填依赖包信息
+requirements = ["playwright","aioconsole"] 
 
 setup(
     name="ChatGPTWeb",
-    version="0.0.7",
+    version="0.0.8",
     author="nek0us",
     author_email="nekouss@gmail.com",
     description="a ChatGPT API,no web ui",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/nek0us/ChatGPT",
     packages=find_packages(),
-    # Single module也可以：
-    # py_modules=['timedd']
     install_requires=requirements,
     classifiers=[
 	"Programming Language :: Python :: 3.9",
 	"License :: OSI Approved :: MIT License",
     ],
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

