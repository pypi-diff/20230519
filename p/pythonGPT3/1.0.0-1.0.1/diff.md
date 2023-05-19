# Comparing `tmp/pythonGPT3-1.0.0.tar.gz` & `tmp/pythonGPT3-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonGPT3-1.0.0.tar", last modified: Fri May 19 17:40:43 2023, max compression
+gzip compressed data, was "pythonGPT3-1.0.1.tar", last modified: Fri May 19 20:08:29 2023, max compression
```

## Comparing `pythonGPT3-1.0.0.tar` & `pythonGPT3-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 sheded    (1000) sheded    (1000)        0 2023-05-19 17:40:42.993130 pythonGPT3-1.0.0/
--rw-rw-r--   0 sheded    (1000) sheded    (1000)     1069 2023-05-19 16:56:33.000000 pythonGPT3-1.0.0/LICENSE.txt
--rw-rw-r--   0 sheded    (1000) sheded    (1000)        0 2023-05-19 14:20:03.000000 pythonGPT3-1.0.0/MANIFEST.in
--rw-rw-r--   0 sheded    (1000) sheded    (1000)     2806 2023-05-19 17:40:42.993130 pythonGPT3-1.0.0/PKG-INFO
--rw-rw-r--   0 sheded    (1000) sheded    (1000)     1053 2023-05-19 15:07:12.000000 pythonGPT3-1.0.0/README.md
--rw-rw-r--   0 sheded    (1000) sheded    (1000)      105 2023-05-19 17:21:22.000000 pythonGPT3-1.0.0/pyproject.toml
--rw-rw-r--   0 sheded    (1000) sheded    (1000)      806 2023-05-19 17:40:42.993130 pythonGPT3-1.0.0/setup.cfg
-drwxrwxr-x   0 sheded    (1000) sheded    (1000)        0 2023-05-19 17:40:42.989130 pythonGPT3-1.0.0/src/
-drwxrwxr-x   0 sheded    (1000) sheded    (1000)        0 2023-05-19 17:40:42.993130 pythonGPT3-1.0.0/src/pythonGPT/
--rw-rw-r--   0 sheded    (1000) sheded    (1000)        0 2023-05-19 14:13:22.000000 pythonGPT3-1.0.0/src/pythonGPT/__init__.py
--rw-rw-r--   0 sheded    (1000) sheded    (1000)     1846 2023-05-19 15:04:30.000000 pythonGPT3-1.0.0/src/pythonGPT/pythonGPT.py
-drwxrwxr-x   0 sheded    (1000) sheded    (1000)        0 2023-05-19 17:40:42.993130 pythonGPT3-1.0.0/src/pythonGPT3.egg-info/
--rw-rw-r--   0 sheded    (1000) sheded    (1000)     2806 2023-05-19 17:40:42.000000 pythonGPT3-1.0.0/src/pythonGPT3.egg-info/PKG-INFO
--rw-rw-r--   0 sheded    (1000) sheded    (1000)      263 2023-05-19 17:40:42.000000 pythonGPT3-1.0.0/src/pythonGPT3.egg-info/SOURCES.txt
--rw-rw-r--   0 sheded    (1000) sheded    (1000)        1 2023-05-19 17:40:42.000000 pythonGPT3-1.0.0/src/pythonGPT3.egg-info/dependency_links.txt
--rw-rw-r--   0 sheded    (1000) sheded    (1000)       10 2023-05-19 17:40:42.000000 pythonGPT3-1.0.0/src/pythonGPT3.egg-info/top_level.txt
+drwxrwxr-x   0 sheded    (1000) sheded    (1000)        0 2023-05-19 20:08:29.732485 pythonGPT3-1.0.1/
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)     1069 2023-05-19 16:56:33.000000 pythonGPT3-1.0.1/LICENSE.txt
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)        0 2023-05-19 14:20:03.000000 pythonGPT3-1.0.1/MANIFEST.in
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)     3096 2023-05-19 20:08:29.732485 pythonGPT3-1.0.1/PKG-INFO
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)     1343 2023-05-19 18:15:02.000000 pythonGPT3-1.0.1/README.md
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)      105 2023-05-19 17:21:22.000000 pythonGPT3-1.0.1/pyproject.toml
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)      806 2023-05-19 20:08:29.736485 pythonGPT3-1.0.1/setup.cfg
+drwxrwxr-x   0 sheded    (1000) sheded    (1000)        0 2023-05-19 20:08:29.724485 pythonGPT3-1.0.1/src/
+drwxrwxr-x   0 sheded    (1000) sheded    (1000)        0 2023-05-19 20:08:29.728485 pythonGPT3-1.0.1/src/pythonGPT/
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)        0 2023-05-19 14:13:22.000000 pythonGPT3-1.0.1/src/pythonGPT/__init__.py
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)     1765 2023-05-19 20:04:17.000000 pythonGPT3-1.0.1/src/pythonGPT/pythonGPT.py
+drwxrwxr-x   0 sheded    (1000) sheded    (1000)        0 2023-05-19 20:08:29.732485 pythonGPT3-1.0.1/src/pythonGPT3.egg-info/
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)     3096 2023-05-19 20:08:29.000000 pythonGPT3-1.0.1/src/pythonGPT3.egg-info/PKG-INFO
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)      263 2023-05-19 20:08:29.000000 pythonGPT3-1.0.1/src/pythonGPT3.egg-info/SOURCES.txt
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)        1 2023-05-19 20:08:29.000000 pythonGPT3-1.0.1/src/pythonGPT3.egg-info/dependency_links.txt
+-rw-rw-r--   0 sheded    (1000) sheded    (1000)       10 2023-05-19 20:08:29.000000 pythonGPT3-1.0.1/src/pythonGPT3.egg-info/top_level.txt
```

### Comparing `pythonGPT3-1.0.0/LICENSE.txt` & `pythonGPT3-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythonGPT3-1.0.0/PKG-INFO` & `pythonGPT3-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonGPT3
-Version: 1.0.0
+Version: 1.0.1
 Summary: "The ChatGPT Requests module is a Python package that provides a convenient interface for making requests to the ChatGPT language model."
 Home-page: https://gitlab.com/codasteroid/basicpkg
 Author: Ahmed Sheded
 Author-email: sheded222@gmail.com
 Project-URL: Bug Tracker, https://github.com/AhmedSheded/pythonGPT/issues
 Project-URL: repository, https://gitlab.com/AhmedSheded/pythonGPT
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,23 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pythonGPT
 
-ChatGPT Requests Module
+pythonGPT Requests Module
 
-The ChatGPT Requests module is a Python package that provides a convenient interface for making requests to the ChatGPT language model. It abstracts away the complexity of interacting with the model's API, allowing developers to easily integrate ChatGPT into their applications.
+The pythonGPT Requests module is a Python package that provides a convenient interface for making requests to the ChatGPT language model. It abstracts away the complexity of interacting with the model's API, allowing developers to easily integrate ChatGPT into their applications.
+
+You can ask one question by request function, or you can send a file of questions separated by a question mark to requests function, and you will get a text file with the answers.
+
+
+you can have your APi key from this link after signing in
+https://platform.openai.com/account/api-keys
 
 Key Features:
 - Simple API: The module provides a high-level API that simplifies the process of sending messages and receiving responses from the ChatGPT model.
 - Stateful Conversations: It supports stateful conversations, enabling users to have multi-turn interactions by maintaining context across messages.
 - Error Handling: The module includes robust error handling to gracefully handle API errors and timeouts, ensuring a reliable integration.
 
 Usage Example:
```

### Comparing `pythonGPT3-1.0.0/README.md` & `pythonGPT3-1.0.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # pythonGPT
 
-ChatGPT Requests Module
+pythonGPT Requests Module
 
-The ChatGPT Requests module is a Python package that provides a convenient interface for making requests to the ChatGPT language model. It abstracts away the complexity of interacting with the model's API, allowing developers to easily integrate ChatGPT into their applications.
+The pythonGPT Requests module is a Python package that provides a convenient interface for making requests to the ChatGPT language model. It abstracts away the complexity of interacting with the model's API, allowing developers to easily integrate ChatGPT into their applications.
+
+You can ask one question by request function, or you can send a file of questions separated by a question mark to requests function, and you will get a text file with the answers.
+
+
+you can have your APi key from this link after signing in
+https://platform.openai.com/account/api-keys
 
 Key Features:
 - Simple API: The module provides a high-level API that simplifies the process of sending messages and receiving responses from the ChatGPT model.
 - Stateful Conversations: It supports stateful conversations, enabling users to have multi-turn interactions by maintaining context across messages.
 - Error Handling: The module includes robust error handling to gracefully handle API errors and timeouts, ensuring a reliable integration.
 
 Usage Example:
```

### Comparing `pythonGPT3-1.0.0/setup.cfg` & `pythonGPT3-1.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pythonGPT3
-version = 1.0.0
+version = 1.0.1
 author = Ahmed Sheded
 author_email = sheded222@gmail.com
 description = "The ChatGPT Requests module is a Python package that provides a convenient interface for making requests to the ChatGPT language model."
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://gitlab.com/codasteroid/basicpkg
 project_urls =
```

### Comparing `pythonGPT3-1.0.0/src/pythonGPT/pythonGPT.py` & `pythonGPT3-1.0.1/src/pythonGPT/pythonGPT.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import requests
 import time
-import json
 
 
 class PythonGPT:
     def __init__(self, api_key):
         self.api_key = api_key
         self.api_url = 'https://api.openai.com/v1/chat/completions'
         self.headers = {
@@ -20,16 +19,15 @@
             "temperature": 0.7,
 
         }
         try:
             response = requests.post(self.api_url, headers=self.headers, json=data)
             response.raise_for_status()
             response_json = response.json()
-            conversation_id = response.json()['id']
-            return conversation_id, response_json['choices'][0]['message']['content'].strip()
+            return response_json['choices'][0]['message']['content'].strip()
         except requests.exceptions.RequestException as err:
             print('An error occurred:', err)
             return None
 
     def requests(self, file_path):
         with open(file_path, 'r') as f:
             content = f.readlines()
```

### Comparing `pythonGPT3-1.0.0/src/pythonGPT3.egg-info/PKG-INFO` & `pythonGPT3-1.0.1/src/pythonGPT3.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonGPT3
-Version: 1.0.0
+Version: 1.0.1
 Summary: "The ChatGPT Requests module is a Python package that provides a convenient interface for making requests to the ChatGPT language model."
 Home-page: https://gitlab.com/codasteroid/basicpkg
 Author: Ahmed Sheded
 Author-email: sheded222@gmail.com
 Project-URL: Bug Tracker, https://github.com/AhmedSheded/pythonGPT/issues
 Project-URL: repository, https://gitlab.com/AhmedSheded/pythonGPT
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,23 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pythonGPT
 
-ChatGPT Requests Module
+pythonGPT Requests Module
 
-The ChatGPT Requests module is a Python package that provides a convenient interface for making requests to the ChatGPT language model. It abstracts away the complexity of interacting with the model's API, allowing developers to easily integrate ChatGPT into their applications.
+The pythonGPT Requests module is a Python package that provides a convenient interface for making requests to the ChatGPT language model. It abstracts away the complexity of interacting with the model's API, allowing developers to easily integrate ChatGPT into their applications.
+
+You can ask one question by request function, or you can send a file of questions separated by a question mark to requests function, and you will get a text file with the answers.
+
+
+you can have your APi key from this link after signing in
+https://platform.openai.com/account/api-keys
 
 Key Features:
 - Simple API: The module provides a high-level API that simplifies the process of sending messages and receiving responses from the ChatGPT model.
 - Stateful Conversations: It supports stateful conversations, enabling users to have multi-turn interactions by maintaining context across messages.
 - Error Handling: The module includes robust error handling to gracefully handle API errors and timeouts, ensuring a reliable integration.
 
 Usage Example:
```

