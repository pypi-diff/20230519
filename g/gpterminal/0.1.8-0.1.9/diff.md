# Comparing `tmp/gpterminal-0.1.8.tar.gz` & `tmp/gpterminal-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpterminal-0.1.8.tar", last modified: Fri May 19 03:37:08 2023, max compression
+gzip compressed data, was "gpterminal-0.1.9.tar", last modified: Fri May 19 05:21:01 2023, max compression
```

## Comparing `gpterminal-0.1.8.tar` & `gpterminal-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-19 03:37:08.721678 gpterminal-0.1.8/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3187 2023-05-19 03:37:08.721118 gpterminal-0.1.8/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2433 2023-05-16 11:36:53.000000 gpterminal-0.1.8/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-19 03:37:08.716244 gpterminal-0.1.8/cli/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.8/cli/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.8/cli/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.8/cli/cli.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.8/cli/code_execution.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2525 2023-05-19 02:30:59.000000 gpterminal-0.1.8/cli/command_print.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4961 2023-05-19 03:36:56.000000 gpterminal-0.1.8/cli/gs.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.8/cli/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-19 03:37:08.719923 gpterminal-0.1.8/gpterminal.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3187 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)      332 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       65 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       59 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-19 03:37:08.721846 gpterminal-0.1.8/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1310 2023-05-19 03:37:04.000000 gpterminal-0.1.8/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-19 05:21:01.827911 gpterminal-0.1.9/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3187 2023-05-19 05:21:01.827575 gpterminal-0.1.9/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2433 2023-05-16 11:36:53.000000 gpterminal-0.1.9/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-19 05:21:01.823424 gpterminal-0.1.9/cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.9/cli/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.9/cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.9/cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.9/cli/code_execution.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2647 2023-05-19 04:49:20.000000 gpterminal-0.1.9/cli/command_print.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5329 2023-05-19 04:47:20.000000 gpterminal-0.1.9/cli/gs.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.9/cli/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-19 05:21:01.826951 gpterminal-0.1.9/gpterminal.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3187 2023-05-19 05:21:01.000000 gpterminal-0.1.9/gpterminal.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      332 2023-05-19 05:21:01.000000 gpterminal-0.1.9/gpterminal.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-19 05:21:01.000000 gpterminal-0.1.9/gpterminal.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       65 2023-05-19 05:21:01.000000 gpterminal-0.1.9/gpterminal.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       59 2023-05-19 05:21:01.000000 gpterminal-0.1.9/gpterminal.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-19 05:21:01.000000 gpterminal-0.1.9/gpterminal.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-19 05:21:01.828042 gpterminal-0.1.9/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1310 2023-05-19 05:20:58.000000 gpterminal-0.1.9/setup.py
```

### Comparing `gpterminal-0.1.8/PKG-INFO` & `gpterminal-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterminal
-Version: 0.1.8
+Version: 0.1.9
 Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
 Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gpterminal-0.1.8/README.md` & `gpterminal-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.8/cli/ChatGPT.py` & `gpterminal-0.1.9/cli/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.8/cli/cli.py` & `gpterminal-0.1.9/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.8/cli/code_execution.py` & `gpterminal-0.1.9/cli/code_execution.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.8/cli/command_print.py` & `gpterminal-0.1.9/cli/command_print.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 
 def show_cursor():
     sys.stdout.write("\033[?25h")
     sys.stdout.flush()
 
 def select_command(commands):
     selected_index = 0
+    # 给最后一个命令加上重新输入
+    commands.append({"description": "重新输入", "cmd": "重新输入"})
 
     def display_commands(commands, selected_index):
         os.system("cls" if os.name == "nt" else "clear")
         hide_cursor()
         aligned = Align.left("\n".join([
             f"[{'>' if i == selected_index else ' '}][dim]{cmd['description']}[/dim]\n  [bold green]{cmd['cmd']}[/bold green]"
             for i, cmd in enumerate(commands)
```

### Comparing `gpterminal-0.1.8/cli/gs.py` & `gpterminal-0.1.9/cli/gs.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 from rich.markdown import Markdown
 from .code_execution import *
 from .cli import get_api_key
 from .command_print import *
 from rich import print
 from rich.text import Text
 import random
-
+import readline
+# 配置 readline
+readline.parse_and_bind("set enable-meta-key on")
+readline.parse_and_bind("set input-meta on")
+readline.parse_and_bind("set output-meta on")
+readline.parse_and_bind("set convert-meta off")
 sys.stdin.reconfigure(encoding='utf-8')
 
 
 def print_colorful(content):
     text = Text()
     colors = ["red", "green", "yellow", "blue", "magenta", "cyan", "white"]
     for char in content:
@@ -54,15 +59,15 @@
     base_url, api_key = get_api_key()
     openai.api_key = api_key
     openai.api_base = base_url + 'v1'
     system_prompt="""   
         1.  用户的系统是: {sys.platform}
         2.  如果用户的输入是命令,帮用户查看命令是否正确，不正确给出正确的命令,最终按照规定输出
             如果用户的输入是自然语言,则帮用户生成命令行，最终按规定输出
-        3.  你的输出可以提供多条相关命令供用户选择，最少4条,如果没有四条，另外几条可以是类似的命令
+        3.  你的输出可以提供多条相关命令供用户选择，最少2条,最多4条,如果没有2条，另外几条可以是类似的命令
         3.  IMPORTANT: 你的输出必须是以下格式, 不准有多余的描述
         <CMD>
         [
             {
                 "description": "命令说明",
                 "cmd": "命令行"
             },
@@ -125,14 +130,17 @@
                 print_colorful(content)
         print()
         print("=" * 80)
         commands = json.loads(tmp.strip())
         print(commands)
         if len(commands) > 0:
             selected_index = select_command(commands)
+            # 如果是最后一个，那就是重新输入
+            if selected_index == len(commands) - 1:
+                continue
             print(f"\n您选择了: {commands[selected_index]['cmd']}")
             # 咨询用户是否执行命令
             if ask_user_execute():
                 # 执行命令
                 execute_command(commands[selected_index]['cmd'])
                 break
             else:
```

### Comparing `gpterminal-0.1.8/cli/utils.py` & `gpterminal-0.1.9/cli/utils.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.8/gpterminal.egg-info/PKG-INFO` & `gpterminal-0.1.9/gpterminal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterminal
-Version: 0.1.8
+Version: 0.1.9
 Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
 Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gpterminal-0.1.8/setup.py` & `gpterminal-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gpterminal",
-    version="0.1.8",
+    version="0.1.9",
     author="Your Name",
     author_email="your.email@example.com",
     description="A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yourusername/gpterminal",
     packages=find_packages(),
```

