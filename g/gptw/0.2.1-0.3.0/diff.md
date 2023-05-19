# Comparing `tmp/gptw-0.2.1.tar.gz` & `tmp/gptw-0.3.0.tar.gz`

## Comparing `gptw-0.2.1.tar` & `gptw-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.2.1/gptw/__init__.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 gptw-0.2.1/gptw/gptw.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 gptw-0.2.1/gptw/prompts.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.2.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.2.1/LICENSE
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 gptw-0.2.1/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 gptw-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 gptw-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.3.0/gptw/__init__.py
+-rw-r--r--   0        0        0     5504 2020-02-02 00:00:00.000000 gptw-0.3.0/gptw/gptw.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 gptw-0.3.0/gptw/prompts.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 gptw-0.3.0/README.md
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 gptw-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 gptw-0.3.0/PKG-INFO
```

### Comparing `gptw-0.2.1/gptw/gptw.py` & `gptw-0.3.0/gptw/gptw.py`

 * *Files 7% similar despite different names*

```diff
@@ -133,14 +133,34 @@
     for chunk in client.send_message(bot_name, text, with_chat_break=True):
         pass
     # delete the 3 latest messages, including the chat break
     client.purge_conversation(bot_name, count=3)
     return chunk["text"]
 
 
+def ask_gpt_web(token, proxy, model, text):
+    os.environ["CHATGPT_BASE_URL"] = proxy
+    logging.debug("proxy:" + os.environ["CHATGPT_BASE_URL"])
+
+    from revChatGPT.V1 import Chatbot
+
+    chatbot = Chatbot(
+        config={
+            "access_token": token,
+            "paid": True,
+            "model": model,
+            "collect_analytics": False,
+        }
+    )
+    response = ""
+    for data in chatbot.ask(text):
+        response = data["message"]
+    return response
+
+
 def list_commands(prompts):
     print(f'{"cmd":<{3}} | {"meaning":<{30}} | {"example"}')
     for pmt in prompts:
         print(
             f"{pmt: <{3}} | {prompts[pmt]['_comment']:<{30}} | {prompts[pmt]['example']}"
         )
 
@@ -176,14 +196,22 @@
         exit(0)
 
     logging.debug(f"cmd:{args.cmd},text:{text}")
 
     msg = f'{prompts[args.cmd]["prompt"]}\n\n{text}'
 
     if get_config("provider") == "openai":
+        logging.debug("use openai")
         model = get_config("openai-model")
         token = get_config("openai-token")
         print(ask_gpt(token, model, msg))
     if get_config("provider") == "poe":
+        logging.debug("use poe")
         token = get_config("poe-token")
         bot_name = get_config("poe-bot-name")
         print(ask_poe(token, bot_name, msg))
+    if get_config("provider") == "gpt-web":
+        logging.debug("use gpt-web")
+        token = get_config("gpt-web-token")
+        proxy = get_config("gpt-web-proxy")
+        model = get_config("gpt-web-model")
+        print(ask_gpt_web(token, proxy, model, msg))
```

### Comparing `gptw-0.2.1/gptw/prompts.json` & `gptw-0.3.0/gptw/prompts.json`

 * *Files identical despite different names*

### Comparing `gptw-0.2.1/.gitignore` & `gptw-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gptw-0.2.1/LICENSE` & `gptw-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gptw-0.2.1/README.md` & `gptw-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -114,14 +114,23 @@
 ww --config poe-token={YOUR_TOKEN}
 ```
 
 Bot names:
 
 {'capybara': 'Sage', 'beaver': 'GPT-4', 'a2_2': 'Claude+', 'a2': 'Claude', 'chinchilla': 'ChatGPT', 'nutria': 'Dragonfly'}
 
+### ChatGPT website
+
+```shell
+ww -c provider=gpt-web
+ww -c gpt-web-model=gpt-4
+ww -c gpt-web-token=  # https://chat.openai.com/api/auth/session copy the access_token session
+ww -c gpt-web-proxy=  # https://github.com/acheong08/ChatGPT-Proxy-V4
+```
+
 ## Uninstall
 
 ```shell
 pip uninstall gptw
 ```
 
 ## Development
```

### Comparing `gptw-0.2.1/pyproject.toml` & `gptw-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 readme.content-type = "text/markdown"
 keywords = ["ChatGPT", "Command Line", "English Translation","English Polishing"]
 license = "Apache-2.0"
 requires-python = ">=3.7.1"
 dependencies = [
   "argparse>=1.4.0",
   "openai>=0.27.0",
-  "poe-api>=0.3.1"
+  "poe-api>=0.3.1",
+  "revChatGPT>=5.0.3"
 ]
 optional-dependencies.testing = [
   "coverage==5.5",
   "pytest==7.1.3",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `gptw-0.2.1/PKG-INFO` & `gptw-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptw
-Version: 0.2.1
+Version: 0.3.0
 Summary: The ChatGPT command-line wrapper simplifies the execution of predetermined tasks through ChatGPT.
 Author: Xin Yang
 Author-email: xinydev@gmail.com
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: ChatGPT,Command Line,English Polishing,English Translation
 Classifier: Development Status :: 3 - Alpha
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7.1
 Requires-Dist: argparse>=1.4.0
 Requires-Dist: openai>=0.27.0
 Requires-Dist: poe-api>=0.3.1
+Requires-Dist: revchatgpt>=5.0.3
 Provides-Extra: testing
 Requires-Dist: coverage==5.5; extra == 'testing'
 Requires-Dist: pytest==7.1.3; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # GPT Simplify Your Daily Workflow (gptW)
 
@@ -143,14 +144,23 @@
 ww --config poe-token={YOUR_TOKEN}
 ```
 
 Bot names:
 
 {'capybara': 'Sage', 'beaver': 'GPT-4', 'a2_2': 'Claude+', 'a2': 'Claude', 'chinchilla': 'ChatGPT', 'nutria': 'Dragonfly'}
 
+### ChatGPT website
+
+```shell
+ww -c provider=gpt-web
+ww -c gpt-web-model=gpt-4
+ww -c gpt-web-token=  # https://chat.openai.com/api/auth/session copy the access_token session
+ww -c gpt-web-proxy=  # https://github.com/acheong08/ChatGPT-Proxy-V4
+```
+
 ## Uninstall
 
 ```shell
 pip uninstall gptw
 ```
 
 ## Development
```

