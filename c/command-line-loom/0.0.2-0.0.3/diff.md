# Comparing `tmp/command_line_loom-0.0.2.tar.gz` & `tmp/command_line_loom-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "command_line_loom-0.0.2.tar", max compression
+gzip compressed data, was "command_line_loom-0.0.3.tar", max compression
```

## Comparing `command_line_loom-0.0.2.tar` & `command_line_loom-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-05-18 18:19:49.972930 command_line_loom-0.0.2/LICENSE
--rw-r--r--   0        0        0     4466 2023-05-18 18:24:52.435855 command_line_loom-0.0.2/README.md
--rw-r--r--   0        0        0        7 2023-05-19 13:37:16.686088 command_line_loom-0.0.2/cll/__init__.py
--rw-r--r--   0        0        0     1555 2023-05-19 13:37:16.690088 command_line_loom-0.0.2/cll/__main__.py
--rw-r--r--   0        0        0     7561 2023-05-19 15:48:20.964766 command_line_loom-0.0.2/cll/app.py
--rw-r--r--   0        0        0     7157 2023-05-19 17:37:55.543457 command_line_loom-0.0.2/cll/config.py
--rw-r--r--   0        0        0      217 2023-05-19 13:37:16.690088 command_line_loom-0.0.2/cll/data_structs/__init__.py
--rw-r--r--   0        0        0    11532 2023-05-19 18:53:41.708355 command_line_loom-0.0.2/cll/data_structs/data_structs.py
--rw-r--r--   0        0        0     9731 2023-05-19 18:50:43.718154 command_line_loom-0.0.2/cll/data_structs/loom_index.py
--rw-r--r--   0        0        0     2493 2023-05-19 17:01:41.546225 command_line_loom-0.0.2/cll/data_structs/node.py
--rw-r--r--   0        0        0     1025 2023-05-19 13:37:16.690088 command_line_loom-0.0.2/cll/io.py
--rw-r--r--   0        0        0     2292 2023-05-19 13:37:16.690088 command_line_loom-0.0.2/cll/store.py
--rw-r--r--   0        0        0     7988 2023-05-19 19:17:40.037687 command_line_loom-0.0.2/cll/templater.py
--rw-r--r--   0        0        0    13494 2023-05-19 20:15:12.816294 command_line_loom-0.0.2/cll/tree.py
--rw-r--r--   0        0        0     1052 2023-05-19 20:16:46.779561 command_line_loom-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 command_line_loom-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-18 18:19:49.972930 command_line_loom-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4466 2023-05-18 18:24:52.435855 command_line_loom-0.0.3/README.md
+-rw-r--r--   0        0        0        7 2023-05-19 13:37:16.686088 command_line_loom-0.0.3/cll/__init__.py
+-rw-r--r--   0        0        0     1555 2023-05-19 13:37:16.690088 command_line_loom-0.0.3/cll/__main__.py
+-rw-r--r--   0        0        0     7645 2023-05-19 20:37:53.421731 command_line_loom-0.0.3/cll/app.py
+-rw-r--r--   0        0        0     7096 2023-05-19 20:33:17.487868 command_line_loom-0.0.3/cll/config.py
+-rw-r--r--   0        0        0      217 2023-05-19 13:37:16.690088 command_line_loom-0.0.3/cll/data_structs/__init__.py
+-rw-r--r--   0        0        0    11532 2023-05-19 18:53:41.708355 command_line_loom-0.0.3/cll/data_structs/data_structs.py
+-rw-r--r--   0        0        0     9817 2023-05-19 20:24:08.516125 command_line_loom-0.0.3/cll/data_structs/loom_index.py
+-rw-r--r--   0        0        0     2493 2023-05-19 17:01:41.546225 command_line_loom-0.0.3/cll/data_structs/node.py
+-rw-r--r--   0        0        0     1025 2023-05-19 13:37:16.690088 command_line_loom-0.0.3/cll/io.py
+-rw-r--r--   0        0        0     2292 2023-05-19 13:37:16.690088 command_line_loom-0.0.3/cll/store.py
+-rw-r--r--   0        0        0     7963 2023-05-19 20:35:18.534930 command_line_loom-0.0.3/cll/templater.py
+-rw-r--r--   0        0        0    12804 2023-05-19 20:48:25.868085 command_line_loom-0.0.3/cll/tree.py
+-rw-r--r--   0        0        0     1052 2023-05-19 20:49:52.943636 command_line_loom-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 command_line_loom-0.0.3/PKG-INFO
```

### Comparing `command_line_loom-0.0.2/LICENSE` & `command_line_loom-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.2/README.md` & `command_line_loom-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.2/cll/__main__.py` & `command_line_loom-0.0.3/cll/__main__.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.2/cll/app.py` & `command_line_loom-0.0.3/cll/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,28 +190,29 @@
     print(ctx.obj.tree.params)
 
 
 @cli.command()
 @cli.command(name="s", hidden=True)
 def save(ctx: Context):
     "(s) Save the current config to the config file."
-    ctx.obj.config._dict["engine_params"] = ctx.obj.tree.params
-    Config.save_openai_config(ctx.obj.config._dict)
+    ctx.obj.openai_config["engine_params"] = ctx.obj.tree.params
+    Config.save_openai_config(ctx.obj.openai_config)
     print("Saved config.")
 
 
 @cli.command()
 @cli.command(name="u", hidden=True)
 def update(
     ctx: Context,
     name: Annotated[Optional[str], Argument()] = None,
     value: Annotated[Optional[str], Argument()] = None,
     kv: Annotated[Optional[str], Argument()] = None,
 ):
-    "(u) Update a config value, or set of values. (kv in the form of 'name1=value1,name2=value2')"
+    "(u) Update a config value, or set of values. (kv in the form of 'name1=value1,name2=value2'). "
+    "You can also just type 'name value' without 'u' to update a single value."
     if kv:
         updates = kv.split(",")
         for kv in updates:
             name, value = kv.split("=")
             Config._update(name, value, ctx.obj.tree.params)
         return
     Config._update(name, value, ctx.obj.tree.params)
```

### Comparing `command_line_loom-0.0.2/cll/config.py` & `command_line_loom-0.0.3/cll/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,16 @@
         "file": True,
         "chat_path": "~/.config/cll/chats",
         "chat_name": "default",
         "echo_prompt": False,
         "append": False,
         "backup_path": "/tmp/cll/",
         "templater": {
-            "in_postfix": "\n",
-            "out_postfix": "\n",
-            "in_prefix": "Human: ",
-            "out_prefix": "GPT:",
+            "in_prefix": "\nHuman: ",
+            "out_prefix": "\nGPT:",
             "template": True,
             "template_path": "~/.config/cll/templates",
             "template_file": "assist.j2",
         },
     }
     OPENAI_DEFAULT_PARAMS = {
         "frequency_penalty": 0,
```

### Comparing `command_line_loom-0.0.2/cll/data_structs/data_structs.py` & `command_line_loom-0.0.3/cll/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.2/cll/data_structs/loom_index.py` & `command_line_loom-0.0.3/cll/data_structs/loom_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,16 @@
                 node = self.index_struct.get_node(identifier)
             nodes.append(node)
         for node in nodes:
             self.extend(node)
 
     def delete(self, identifiers: List[Union[int, str]]) -> None:
         """Delete a list of nodes in the index."""
+        if not isinstance(identifiers, list):
+            identifiers = [identifiers]
         nodes = []
         for identifier in identifiers:
             if identifier in self.tags.keys():
                 node = self.index_struct.all_nodes[self.tags[identifier]]
             else:
                 node = self.index_struct.get_node(identifier)
             nodes.append(node)
```

### Comparing `command_line_loom-0.0.2/cll/data_structs/node.py` & `command_line_loom-0.0.3/cll/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.2/cll/io.py` & `command_line_loom-0.0.3/cll/io.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.2/cll/store.py` & `command_line_loom-0.0.3/cll/store.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.2/cll/templater.py` & `command_line_loom-0.0.3/cll/templater.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,16 @@
 
 
 @cli.command()
 @cli.command(name="s", hidden=True)
 def save(ctx: Context):
     "(s) Save the current config to the config file."
     config = ctx.obj.templater.config
-    config["templater"] = ctx.obj.templater.template_config
-    Config.save_config(ctx.obj.templater.config)
+    config._dict["templater"] = ctx.obj.templater.template_config
+    config.save()
 
 
 @cli.command()
 @cli.command(name="u", hidden=True)
 def update(
     ctx: Context,
     name: Annotated[Optional[str], Argument()] = None,
```

### Comparing `command_line_loom-0.0.2/cll/tree.py` & `command_line_loom-0.0.3/cll/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -245,15 +245,18 @@
 @cli.command(name="s", hidden=True)
 def send(
     ctx: Context,
     msg: Annotated[Optional[List[str]], Argument()],
 ):
     """(s) Adds a new message to the chain and sends it all."""
     _append(ctx, msg)
+    _send(ctx)
 
+
+def _send(ctx):
     prompt = ctx.obj.tree.prompt
     prompt = ctx.obj.templater.prompt(prompt)
 
     params = deepcopy(ctx.obj.tree.params)
     params["prompt"] = prompt
     responses, choice = ctx.obj.simple_gen(ctx.obj.config, params)
     if len(responses) == 1:
@@ -275,36 +278,15 @@
     path_with_current(ctx)
 
 
 @cli.command()
 @cli.command(name="pu", hidden=True)
 def push(ctx: Context):
     """(pu) sends the tree with no new message."""
-
-    prompt = ctx.obj.tree.prompt
-    prompt = ctx.obj.templater.prompt(prompt)
-
-    params = deepcopy(ctx.obj.tree.params)
-    params["prompt"] = prompt
-    responses, choice = ctx.obj.simple_gen(ctx.obj.config, params)
-    if len(responses) == 1:
-        response = ctx.obj.templater.out(responses[0])
-        ctx.obj.tree.extend(response)
-    else:
-        for response in responses.values():
-            response = ctx.obj.templater.out(response)
-            ctx.obj.tree.insert(response)
-
-    if choice is not None:
-        index = len(responses) - choice
-        node_indexes = list(ctx.obj.tree.index.index_struct.all_nodes.keys())
-        ctx.obj.tree.index.checkout(node_indexes[-index])
-    ctx.obj.tree.save()
-
-    path_with_current(ctx)
+    _send(ctx)
 
 
 @cli.command()
 @cli.command(name="n", hidden=True)
 def new(ctx: Context):
     """n[ew] starts a new chain (a new root)"""
     ctx.obj.tree.index.clear_checkout()
@@ -374,25 +356,23 @@
 @cli.command(name="prompt", hidden=True)
 def edit_prompt(ctx: Context, index: Annotated[Optional[str], Argument()] = None):
     """(prompt) Export the full prompt to an editor for saving."""
     input = str(ctx.obj.tree.prompt)
     click.edit(input)
 
 
-@cli.command()
-@cli.command(name="del", hidden=True)
-def delete(ctx: Context, indexes: Annotated[Optional[str], Argument()] = None):
-    "(del) delete some nodes (space separated) (last one by default)"
-    if not indexes:
-        indexes = [ctx.obj.tree.index.path[-1].index]
-    else:
-        indexes = indexes.split(" ")
-
-    for index in indexes:
-        ctx.obj.tree.index.delete(int(index))
+# @cli.command()
+# @cli.command(name="del", hidden=True)
+# def delete(ctx: Context, indexes: Annotated[Optional[str], Argument()] = None):
+#     "(del) delete some nodes (space separated) (last one by default)"
+#     if not indexes:
+#         indexes = [ctx.obj.tree.index.path[-1].index]
+#     else:
+#         indexes = indexes.split(" ")
+#     ctx.obj.tree.index.delete(indexes)
 
 
 @cli.command()
 @cli.command(name="cp", hidden=True)
 def cherry_pick(ctx: Context, indexes: str):
     "(cp) Copy nodes onto the current branch (can be indexes or tags, space separated)"
     indexes = [int(index) if index.isdigit() else index for index in indexes.split(" ")]
@@ -422,14 +402,16 @@
             return
         ctx.obj.tree.extend(output)
     elif choice in ["cp", "cherry pick"]:
         ctx.obj.tree.index.cherry_pick(ids)
     elif choice in ["d", "delete"]:
         ctx.obj.tree.index.delete(ids)
 
+    path_with_current(ctx)
+
 
 # @staticmethod
 # def context(_, command_params, tree):
 #     if command_params and command_params[0] == "help":
 #         click.echo(
 #             "modify the context. context can be added to nodes but are not part of the main path\n"
 #             "\t\t\tsubcommands are clear, list, remove or add"
```

### Comparing `command_line_loom-0.0.2/pyproject.toml` & `command_line_loom-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "command-line-loom"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["fergus <fergusfettes@gmail.com>"]
 homepage = "https://github.com/fergusfettes/command-line-loom"
 readme = "README.md"
 packages = [{include = "cll"}]
 
 [tool.poetry.dependencies]
```

### Comparing `command_line_loom-0.0.2/PKG-INFO` & `command_line_loom-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: command-line-loom
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Home-page: https://github.com/fergusfettes/command-line-loom
 Author: fergus
 Author-email: fergusfettes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

