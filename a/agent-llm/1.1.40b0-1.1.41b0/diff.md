# Comparing `tmp/agent-llm-1.1.40b0.tar.gz` & `tmp/agent-llm-1.1.41b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent-llm-1.1.40b0.tar", last modified: Thu May 18 21:34:10 2023, max compression
+gzip compressed data, was "agent-llm-1.1.41b0.tar", last modified: Fri May 19 16:31:57 2023, max compression
```

## Comparing `agent-llm-1.1.40b0.tar` & `agent-llm-1.1.41b0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:34:10.302741 agent-llm-1.1.40b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-05-18 21:34:10.302741 agent-llm-1.1.40b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:34:10.298741 agent-llm-1.1.40b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 21:34:10.302741 agent-llm-1.1.40b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:34:10.298741 agent-llm-1.1.40b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:34:10.298741 agent-llm-1.1.40b0/src/agent-llm/
--rw-r--r--   0 runner    (1001) docker     (123)    27238 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/AgentLLM.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/Commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:34:10.298741 agent-llm-1.1.40b0/src/agent-llm/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/Config/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:34:10.302741 agent-llm-1.1.40b0/src/agent-llm/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/smartchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/smartinstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)    22092 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 21:33:55.000000 agent-llm-1.1.40b0/src/agent-llm/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:34:10.302741 agent-llm-1.1.40b0/src/agent_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-05-18 21:34:10.000000 agent-llm-1.1.40b0/src/agent_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-18 21:34:10.000000 agent-llm-1.1.40b0/src/agent_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:34:10.000000 agent-llm-1.1.40b0/src/agent_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-18 21:34:10.000000 agent-llm-1.1.40b0/src/agent_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 21:34:10.000000 agent-llm-1.1.40b0/src/agent_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:31:57.606404 agent-llm-1.1.41b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-05-19 16:31:57.606404 agent-llm-1.1.41b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:31:57.598404 agent-llm-1.1.41b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:31:57.606404 agent-llm-1.1.41b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:31:57.598404 agent-llm-1.1.41b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:31:57.602404 agent-llm-1.1.41b0/src/agent-llm/
+-rw-r--r--   0 runner    (1001) docker     (123)    27238 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/AgentLLM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/Commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:31:57.602404 agent-llm-1.1.41b0/src/agent-llm/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/Config/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:31:57.602404 agent-llm-1.1.41b0/src/agent-llm/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/smartchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/smartinstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31803 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 16:31:46.000000 agent-llm-1.1.41b0/src/agent-llm/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:31:57.602404 agent-llm-1.1.41b0/src/agent_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-05-19 16:31:57.000000 agent-llm-1.1.41b0/src/agent_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-19 16:31:57.000000 agent-llm-1.1.41b0/src/agent_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:31:57.000000 agent-llm-1.1.41b0/src/agent_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-19 16:31:57.000000 agent-llm-1.1.41b0/src/agent_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 16:31:57.000000 agent-llm-1.1.41b0/src/agent_llm.egg-info/top_level.txt
```

### Comparing `agent-llm-1.1.40b0/LICENSE` & `agent-llm-1.1.41b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/PKG-INFO` & `agent-llm-1.1.41b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-llm
-Version: 1.1.40b0
+Version: 1.1.41b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agent-llm-1.1.40b0/docs/README.md` & `agent-llm-1.1.41b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/setup.py` & `agent-llm-1.1.41b0/setup.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/AgentLLM.py` & `agent-llm-1.1.41b0/src/agent-llm/AgentLLM.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/Commands.py` & `agent-llm-1.1.41b0/src/agent-llm/Commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,14 +48,27 @@
                             "name": command_name,
                             "args": command_args,
                             "enabled": False,
                         }
                     )
         return available_commands
 
+    def get_enabled_commands(self):
+        enabled_commands = []
+        for command in self.available_commands:
+            if command["enabled"]:
+                enabled_commands.append(command)
+        return enabled_commands
+
+    def get_command_args(self, command_name: str):
+        for command in self.available_commands:
+            if command["friendly_name"] == command_name:
+                return command["args"]
+        return None
+
     def load_commands(self):
         commands = []
         command_files = self.CFG.load_command_files()
         for command_file in command_files:
             module_name = os.path.splitext(os.path.basename(command_file))[0]
             module = importlib.import_module(f"commands.{module_name}")
             if issubclass(getattr(module, module_name), Commands):
```

### Comparing `agent-llm-1.1.40b0/src/agent-llm/Config/Agent.py` & `agent-llm-1.1.41b0/src/agent-llm/Config/Agent.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/Config/__init__.py` & `agent-llm-1.1.41b0/src/agent-llm/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/CustomPrompt.py` & `agent-llm-1.1.41b0/src/agent-llm/CustomPrompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,14 +29,23 @@
         # Get all files in prompts folder that end in .txt and replace .txt with empty string
         prompts = []
         for file in os.listdir("prompts"):
             if file.endswith(".txt"):
                 prompts.append(file.replace(".txt", ""))
         return prompts
 
+    def get_prompt_args(self, prompt_name):
+        prompt = self.get_prompt(prompt_name)
+        # Find anything in the file between { and } and add them to a list to return
+        prompt_vars = []
+        for word in prompt.split():
+            if word.startswith("{") and word.endswith("}"):
+                prompt_vars.append(word[1:-1])
+        return prompt_vars
+
     def delete_prompt(self, prompt_name):
         os.remove(os.path.join("prompts", f"{prompt_name}.txt"))
 
     def update_prompt(self, prompt_name, prompt):
         with open(os.path.join("prompts", f"{prompt_name}.txt"), "w") as f:
             f.write(prompt)
```

### Comparing `agent-llm-1.1.40b0/src/agent-llm/Embedding.py` & `agent-llm-1.1.41b0/src/agent-llm/Embedding.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/Memories.py` & `agent-llm-1.1.41b0/src/agent-llm/Memories.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/app.py` & `agent-llm-1.1.41b0/src/agent-llm/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import threading
 from typing import Optional, Dict, List, Any
 from provider import get_provider_options
 from Embedding import get_embedding_providers
 import os
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_directory, "src/agent-llm/version"), encoding="utf-8") as f:
+with open(os.path.join(this_directory, "version"), encoding="utf-8") as f:
     version = f.read().strip()
 
 CFG = Config()
 app = FastAPI(
     title="Agent-LLM",
     description="Agent-LLM is an Artificial Intelligence Automation platform for creating and managing AI agents. Visit the GitHub repo for more information or to report issues. https://github.com/Josh-XT/Agent-LLM/",
     version=version,
```

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/__init__.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/azure.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/bing.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/fastchat.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/gpt4all.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/gpt4free.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/gpugpt4all.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/huggingchat.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/kobold.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/llamacpp.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/oobabooga.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/openai.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/palm.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/provider/transformer.py` & `agent-llm-1.1.41b0/src/agent-llm/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/requirements.txt` & `agent-llm-1.1.41b0/src/agent-llm/requirements.txt`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/smartchat.py` & `agent-llm-1.1.41b0/src/agent-llm/smartchat.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/smartinstruct.py` & `agent-llm-1.1.41b0/src/agent-llm/smartinstruct.py`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent-llm/streamlit.py` & `agent-llm-1.1.41b0/src/agent-llm/streamlit.py`

 * *Files 22% similar despite different names*

```diff
@@ -531,14 +531,251 @@
                 st.success(f"Chain '{chain_name}' created.")
             elif chain_action == "Delete Chain":
                 Chain().delete_chain(chain_name)
                 st.success(f"Chain '{chain_name}' deleted.")
         else:
             st.error("Chain name is required.")
 
+    st.header("Manage Chain Steps")
+
+    chain_names = Chain().get_chains()
+    selected_chain_name = st.selectbox("Select Chain", [""] + chain_names)
+
+    if selected_chain_name:
+        chain = Chain().get_steps(selected_chain_name)
+
+        st.subheader(f"Selected Chain: {selected_chain_name}")
+
+        def modify_step(step):
+            step_number = step["step"]
+            agent_name = step["agent_name"]
+            prompt_type = step["prompt_type"]
+            prompt = step.get("prompt", "")
+
+            modify_step_number = st.number_input(
+                "Step Number",
+                min_value=1,
+                step=1,
+                value=step_number,
+                key=f"step_num_{step_number}",
+            )
+            modify_agent_name = st.selectbox(
+                "Select Agent",
+                options=[""] + [agent["name"] for agent in CFG.get_agents()],
+                index=(
+                    [agent["name"] for agent in CFG.get_agents()].index(agent_name) + 1
+                )
+                if agent_name in [agent["name"] for agent in CFG.get_agents()]
+                else 0,
+                key=f"agent_name_{step_number}",
+            )
+            modify_prompt_type = st.selectbox(
+                "Select Prompt Type",
+                options=["", "Command", "Prompt"],
+                index=["", "Command", "Prompt"].index(prompt_type),
+                key=f"prompt_type_{step_number}",
+            )
+
+            if modify_prompt_type == "Command":
+                available_commands = [
+                    cmd["friendly_name"]
+                    for cmd in Commands(agent_name).get_enabled_commands()
+                ]
+                command_name = st.selectbox(
+                    "Select Command",
+                    [""] + available_commands,
+                    key=f"command_name_{step_number}",
+                    index=available_commands.index(prompt.get("command_name", "")) + 1
+                    if "command_name" in prompt
+                    else 0,
+                )
+
+                if command_name:
+                    command_args = Commands(agent_name).get_command_args(command_name)
+                    formatted_command_args = ", ".join(
+                        [
+                            f"{arg}: {st.text_input(arg, value=prompt.get(arg, ''), key=f'{arg}_{step_number}')} "
+                            for arg in command_args
+                            if arg != "context"
+                        ]
+                    )
+                    modify_prompt = f"{command_name}({formatted_command_args})"
+            elif modify_prompt_type == "Prompt":
+                available_prompts = CustomPrompt().get_prompts()
+                modify_prompt_name = st.selectbox(
+                    "Select Custom Prompt",
+                    [""] + available_prompts,
+                    key=f"prompt_name_{step_number}",
+                    index=available_prompts.index(prompt.get("prompt_name", "")) + 1
+                    if "prompt_name" in prompt
+                    else 0,
+                )
+
+                if modify_prompt_name:
+                    prompt_args = CustomPrompt().get_prompt_args(modify_prompt_name)
+                    formatted_prompt_args = ", ".join(
+                        [
+                            f"{arg}: {st.text_input(arg, value=prompt.get(arg, ''), key=f'{arg}_{step_number}')} "
+                            for arg in prompt_args
+                            if arg != "context"
+                        ]
+                    )
+                    modify_prompt = f"{modify_prompt_name}({formatted_prompt_args})"
+            else:
+                modify_prompt = ""
+
+            if st.button("Modify Step", key=f"modify_{step_number}"):
+                Chain().update_step(
+                    selected_chain_name,
+                    step_number,
+                    modify_agent_name,
+                    modify_prompt_type,
+                    modify_prompt,
+                )
+                st.success(
+                    f"Step {step_number} updated in chain '{selected_chain_name}'."
+                )
+                return {
+                    "step": modify_step_number,
+                    "agent_name": modify_agent_name,
+                    "prompt_type": modify_prompt_type,
+                    "prompt": modify_prompt,
+                }
+            return step
+
+        st.write("Existing Steps:")
+        if chain:
+            for step in chain:
+                if step is not None:
+                    try:
+                        step = modify_step(step)
+                    except TypeError:
+                        st.error(
+                            "Error loading chain step. Please check the chain configuration."
+                        )
+
+        step_number = max([s["step"] for s in chain]) + 1 if chain else 1
+        agent_name = st.selectbox(
+            "Select Agent",
+            options=[""] + [agent["name"] for agent in CFG.get_agents()],
+            index=0,
+            key="add_step_agent_name",
+        )
+        prompt_type = st.selectbox(
+            "Select Prompt Type",
+            [""] + ["Command", "Prompt"],
+            key="add_step_prompt_type",
+        )
+
+        if prompt_type == "Command":
+            available_commands = [
+                cmd["friendly_name"]
+                for cmd in Commands(agent_name).get_enabled_commands()
+            ]
+            command_name = st.selectbox(
+                "Select Command", [""] + available_commands, key="add_step_command_name"
+            )
+
+            if command_name:
+                command_args = Commands(agent_name).get_command_args(command_name)
+                formatted_command_args = ", ".join(
+                    [
+                        f"{arg}: {st.text_input(arg, key=f'add_step_{arg}')} "
+                        for arg in command_args
+                        if arg != "context"
+                    ]
+                )
+                prompt = f"{command_name}({formatted_command_args})"
+        elif prompt_type == "Prompt":
+            available_prompts = CustomPrompt().get_prompts()
+            prompt_name = st.selectbox(
+                "Select Custom Prompt",
+                [""] + available_prompts,
+                key="add_step_prompt_name",
+            )
+
+            if prompt_name:
+                prompt_args = CustomPrompt().get_prompt_args(prompt_name)
+                formatted_prompt_args = ", ".join(
+                    [
+                        f"{arg}: {st.text_input(arg, key=f'add_step_{arg}')} "
+                        for arg in prompt_args
+                        if arg != "context"
+                    ]
+                )
+                prompt = f"{prompt_name}({formatted_prompt_args})"
+        else:
+            prompt = ""
+
+        step_action = st.selectbox(
+            "Action", ["Add Step", "Update Step", "Delete Step"], key="add_step_action"
+        )
+
+        if st.button("Perform Step Action", key="add_step_button"):
+            if (
+                selected_chain_name
+                and step_number
+                and agent_name
+                and prompt_type
+                and prompt
+            ):
+                if step_action == "Add Step":
+                    if prompt_type == "Command":
+                        prompt_data = {"command_name": command_name}
+                        for arg in command_args:
+                            if arg != "context":
+                                prompt_data[arg] = st.session_state[f"add_step_{arg}"]
+                    elif prompt_type == "Prompt":
+                        prompt_data = {"prompt_name": prompt_name}
+                        for arg in prompt_args:
+                            if arg != "context":
+                                prompt_data[arg] = st.session_state[f"add_step_{arg}"]
+
+                    Chain().add_chain_step(
+                        selected_chain_name,
+                        step_number,
+                        agent_name,
+                        prompt_type,
+                        prompt_data,
+                    )
+                    st.success(
+                        f"Step {step_number} added to chain '{selected_chain_name}'."
+                    )
+                elif step_action == "Update Step":
+                    if prompt_type == "Command":
+                        prompt_data = {"command_name": command_name}
+                        for arg in command_args:
+                            if arg != "context":
+                                prompt_data[arg] = st.session_state[f"add_step_{arg}"]
+                    elif prompt_type == "Prompt":
+                        prompt_data = {"prompt_name": prompt_name}
+                        for arg in prompt_args:
+                            if arg != "context":
+                                prompt_data[arg] = st.session_state[f"add_step_{arg}"]
+
+                    Chain().update_step(
+                        selected_chain_name,
+                        step_number,
+                        agent_name,
+                        prompt_type,
+                        prompt_data,
+                    )
+                    st.success(
+                        f"Step {step_number} updated in chain '{selected_chain_name}'."
+                    )
+                elif step_action == "Delete Step":
+                    Chain().delete_step(selected_chain_name, step_number)
+                    st.success(
+                        f"Step {step_number} deleted from chain '{selected_chain_name}'."
+                    )
+            else:
+                st.error("All fields are required.")
+    else:
+        st.warning("Please select a chain to manage steps.")
+
 elif main_selection == "Custom Prompts":
     st.header("Manage Custom Prompts")
 
     prompt_name = st.text_input("Prompt Name")
     prompt_content = st.text_area("Prompt Content")
     prompt_action = st.selectbox(
         "Action", ["Add Prompt", "Update Prompt", "Delete Prompt"]
```

### Comparing `agent-llm-1.1.40b0/src/agent_llm.egg-info/PKG-INFO` & `agent-llm-1.1.41b0/src/agent_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-llm
-Version: 1.1.40b0
+Version: 1.1.41b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agent-llm-1.1.40b0/src/agent_llm.egg-info/SOURCES.txt` & `agent-llm-1.1.41b0/src/agent_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agent-llm-1.1.40b0/src/agent_llm.egg-info/requires.txt` & `agent-llm-1.1.41b0/src/agent_llm.egg-info/requires.txt`

 * *Files identical despite different names*

