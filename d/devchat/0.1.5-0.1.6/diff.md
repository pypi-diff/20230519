# Comparing `tmp/devchat-0.1.5.tar.gz` & `tmp/devchat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devchat-0.1.5.tar", last modified: Fri May 12 04:10:23 2023, max compression
+gzip compressed data, was "devchat-0.1.6.tar", last modified: Fri May 19 17:53:58 2023, max compression
```

## Comparing `devchat-0.1.5.tar` & `devchat-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-12 04:10:23.687226 devchat-0.1.5/
--rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.5/LICENSE
--rw-r--r--   0 basicthinker   (501) staff       (20)      227 2023-05-12 04:10:23.687061 devchat-0.1.5/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)       44 2023-05-05 13:17:54.000000 devchat-0.1.5/README.md
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-12 04:10:23.683537 devchat-0.1.5/devchat/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.5/devchat/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5666 2023-05-12 01:45:56.000000 devchat-0.1.5/devchat/_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     4552 2023-05-12 00:41:47.000000 devchat-0.1.5/devchat/assistant.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1464 2023-05-05 13:17:54.000000 devchat-0.1.5/devchat/chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)      614 2023-05-07 23:44:52.000000 devchat-0.1.5/devchat/message.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-12 04:10:23.685283 devchat-0.1.5/devchat/openai/
--rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.5/devchat/openai/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3402 2023-05-08 03:20:19.000000 devchat-0.1.5/devchat/openai/openai_chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.5/devchat/openai/openai_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     6017 2023-05-12 02:31:16.000000 devchat-0.1.5/devchat/openai/openai_prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     6447 2023-05-12 00:56:54.000000 devchat-0.1.5/devchat/prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3568 2023-05-08 03:39:48.000000 devchat-0.1.5/devchat/store.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     4981 2023-05-12 00:21:13.000000 devchat-0.1.5/devchat/utils.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-12 04:10:23.684398 devchat-0.1.5/devchat.egg-info/
--rw-r--r--   0 basicthinker   (501) staff       (20)      227 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/SOURCES.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/dependency_links.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/entry_points.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      116 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/requires.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/top_level.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.5/pyproject.toml
--rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-12 04:10:23.687268 devchat-0.1.5/setup.cfg
--rw-r--r--   0 basicthinker   (501) staff       (20)      547 2023-05-12 04:09:29.000000 devchat-0.1.5/setup.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-12 04:10:23.686789 devchat-0.1.5/tests/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.5/tests/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5996 2023-05-12 00:42:14.000000 devchat-0.1.5/tests/test_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.5/tests/test_openai_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5908 2023-05-12 00:53:18.000000 devchat-0.1.5/tests/test_openai_prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     2303 2023-05-05 15:34:17.000000 devchat-0.1.5/tests/test_store.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.5/tests/test_utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-19 17:53:58.898735 devchat-0.1.6/
+-rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.6/LICENSE
+-rw-r--r--   0 basicthinker   (501) staff       (20)      415 2023-05-19 17:53:58.898580 devchat-0.1.6/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3584 2023-05-19 17:28:29.000000 devchat-0.1.6/README.md
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-19 17:53:58.894792 devchat-0.1.6/devchat/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.6/devchat/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5660 2023-05-18 09:46:55.000000 devchat-0.1.6/devchat/_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4552 2023-05-12 00:41:47.000000 devchat-0.1.6/devchat/assistant.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1464 2023-05-05 13:17:54.000000 devchat-0.1.6/devchat/chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)      614 2023-05-07 23:44:52.000000 devchat-0.1.6/devchat/message.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-19 17:53:58.896829 devchat-0.1.6/devchat/openai/
+-rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.6/devchat/openai/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3399 2023-05-18 09:47:11.000000 devchat-0.1.6/devchat/openai/openai_chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.6/devchat/openai/openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6017 2023-05-18 05:09:41.000000 devchat-0.1.6/devchat/openai/openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6447 2023-05-12 00:56:54.000000 devchat-0.1.6/devchat/prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3704 2023-05-19 17:29:57.000000 devchat-0.1.6/devchat/store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4981 2023-05-12 00:21:13.000000 devchat-0.1.6/devchat/utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-19 17:53:58.895860 devchat-0.1.6/devchat.egg-info/
+-rw-r--r--   0 basicthinker   (501) staff       (20)      415 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/SOURCES.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/dependency_links.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/entry_points.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      116 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/requires.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/top_level.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.6/pyproject.toml
+-rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-19 17:53:58.898773 devchat-0.1.6/setup.cfg
+-rw-r--r--   0 basicthinker   (501) staff       (20)      770 2023-05-19 17:52:56.000000 devchat-0.1.6/setup.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-19 17:53:58.898284 devchat-0.1.6/tests/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.6/tests/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5996 2023-05-12 00:42:14.000000 devchat-0.1.6/tests/test_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.6/tests/test_openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5908 2023-05-12 00:53:18.000000 devchat-0.1.6/tests/test_openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     2303 2023-05-05 15:34:17.000000 devchat-0.1.6/tests/test_store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.6/tests/test_utils.py
```

### Comparing `devchat-0.1.5/LICENSE` & `devchat-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/devchat/_cli.py` & `devchat-0.1.6/devchat/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     if not os.path.exists(chat_dir):
         os.makedirs(chat_dir)
 
     default_config_data = {
         'model': 'gpt-3.5-turbo',
         'provider': 'OpenAI',
         'OpenAI': {
-            'temperature': 0.2
+            'temperature': 0
         }
     }
 
     try:
         with open(os.path.join(chat_dir, 'config.json'), 'r', encoding='utf-8') as file:
             config_data = json.load(file)
     except FileNotFoundError:
@@ -102,28 +102,28 @@
     If the file is not found, it uses the following default configuration:
     ```json
     {
         "model": "gpt-3.5-turbo",
         "tokens-per-prompt": 3000,
         "provider": "OpenAI",
         "OpenAI": {
-            "temperature": 0.2
+            "temperature": 0
         }
     }
     ```
 
     To customize the configuration, create `.chat/config.json` in your current Git root directory
     and modify the settings as needed. We recoommend the following settings:
     ```json
     {
         "model": "gpt-4",
         "tokens-per-prompt": 6000,
         "provider": "OpenAI",
         "OpenAI": {
-            "temperature": 0.2,
+            "temperature": 0,
             "stream": true
         }
     }
     ```
 
     Note: To use OpenAI's APIs, you must have an API key to run the CLI.
     Run the following command line with your API key:
```

### Comparing `devchat-0.1.5/devchat/assistant.py` & `devchat-0.1.6/devchat/assistant.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/devchat/chat.py` & `devchat-0.1.6/devchat/chat.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/devchat/message.py` & `devchat-0.1.6/devchat/message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/devchat/openai/openai_chat.py` & `devchat-0.1.6/devchat/openai/openai_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class OpenAIChatConfig(BaseModel):
     """
     Configuration object for the OpenAIChat class.
     """
     model: str
-    temperature: Optional[float] = Field(None, ge=0, le=2)
+    temperature: Optional[float] = Field(0, ge=0, le=2)
     top_p: Optional[float] = Field(None, ge=0, le=1)
     n: Optional[int] = Field(None, ge=1)
     stream: Optional[bool] = Field(None)
     stop: Optional[Union[str, List[str]]] = Field(None)
     max_tokens: Optional[int] = Field(None, ge=1)
     presence_penalty: Optional[float] = Field(None, ge=-2.0, le=2.0)
     frequency_penalty: Optional[float] = Field(None, ge=-2.0, le=2.0)
```

### Comparing `devchat-0.1.5/devchat/openai/openai_message.py` & `devchat-0.1.6/devchat/openai/openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/devchat/openai/openai_prompt.py` & `devchat-0.1.6/devchat/openai/openai_prompt.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/devchat/prompt.py` & `devchat-0.1.6/devchat/prompt.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/devchat/store.py` & `devchat-0.1.6/devchat/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,32 @@
         Args:
             path (str): The folder to store the files containing the store.
         """
         store_dir = os.path.expanduser(store_dir)
         if not os.path.isdir(store_dir):
             os.makedirs(store_dir)
         self._graph_path = os.path.join(store_dir, 'prompts.graphml')
-        self._db_path = os.path.join(store_dir, 'prompts.db')
+        self._db_path = os.path.join(store_dir, 'prompts')
 
         if os.path.isfile(self._graph_path):
             try:
                 self._graph = nx.read_graphml(self._graph_path)
             except ParseError as error:
                 raise ValueError(f"Invalid file format for graph: {self._graph_path}") from error
         else:
             self._graph = nx.DiGraph()
 
         self._db = shelve.open(self._db_path)
 
+    def __del__(self):
+        """
+        Close the shelve file when the Store object is destroyed.
+        """
+        self._db.close()
+
     @property
     def graph_path(self) -> str:
         """
         The path to the graph store file.
         """
         return self._graph_path
 
@@ -50,32 +56,32 @@
 
         Args:
             prompt (Prompt): The prompt to store.
         """
         if not prompt.hash:
             prompt.set_hash()
 
+        # Store the prompt object in the shelve database
+        self._db[prompt.hash] = prompt
+        self._db.sync()
+
         # Add the prompt to the graph
         self._graph.add_node(prompt.hash, timestamp=prompt.timestamp)
 
         # Add edges for parents and references
         if prompt.parent:
             if prompt.parent not in self._graph:
                 raise ValueError(f'Parent {prompt.parent} not found in the store.')
             self._graph.add_edge(prompt.hash, prompt.parent)
         for reference_hash in prompt.references:
             if reference_hash not in self._graph:
                 raise ValueError(f'Reference {reference_hash} not found in the store.')
             self._graph.add_edge(prompt.hash, reference_hash)
         nx.write_graphml(self._graph, self._graph_path)
 
-        # Store the prompt object in the shelve database
-        self._db[prompt.hash] = prompt
-        self._db.sync()
-
     def get_prompt(self, prompt_hash: str) -> Prompt:
         """
         Retrieve a prompt from the store.
 
         Args:
             prompt_hash (str): The hash of the prompt to retrieve.
         Returns:
```

### Comparing `devchat-0.1.5/devchat/utils.py` & `devchat-0.1.6/devchat/utils.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/devchat.egg-info/SOURCES.txt` & `devchat-0.1.6/devchat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/tests/test_cli.py` & `devchat-0.1.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/tests/test_openai_message.py` & `devchat-0.1.6/tests/test_openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/tests/test_openai_prompt.py` & `devchat-0.1.6/tests/test_openai_prompt.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/tests/test_store.py` & `devchat-0.1.6/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.5/tests/test_utils.py` & `devchat-0.1.6/tests/test_utils.py`

 * *Files identical despite different names*

