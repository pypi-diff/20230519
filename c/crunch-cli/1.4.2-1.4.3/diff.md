# Comparing `tmp/crunch-cli-1.4.2.tar.gz` & `tmp/crunch-cli-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.4.2.tar", last modified: Thu May 18 13:26:17 2023, max compression
+gzip compressed data, was "crunch-cli-1.4.3.tar", last modified: Fri May 19 13:53:42 2023, max compression
```

## Comparing `crunch-cli-1.4.2.tar` & `crunch-cli-1.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:26:17.686307 crunch-cli-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-18 13:26:17.686307 crunch-cli-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:26:17.686307 crunch-cli-1.4.2/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:26:17.686307 crunch-cli-1.4.2/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:26:17.686307 crunch-cli-1.4.2/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:26:17.686307 crunch-cli-1.4.2/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-18 13:26:17.000000 crunch-cli-1.4.2/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-18 13:26:17.000000 crunch-cli-1.4.2/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:26:17.000000 crunch-cli-1.4.2/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 13:26:17.000000 crunch-cli-1.4.2/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:26:17.000000 crunch-cli-1.4.2/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-18 13:26:17.000000 crunch-cli-1.4.2/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 13:26:17.000000 crunch-cli-1.4.2/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 13:26:17.686307 crunch-cli-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-18 13:26:08.000000 crunch-cli-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 13:53:42.000000 crunch-cli-1.4.3/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:53:42.661653 crunch-cli-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-19 13:53:37.000000 crunch-cli-1.4.3/setup.py
```

### Comparing `crunch-cli-1.4.2/crunch/command/convert.py` & `crunch-cli-1.4.3/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/command/download.py` & `crunch-cli-1.4.3/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/command/push.py` & `crunch-cli-1.4.3/crunch/command/push.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import tarfile
 import tempfile
+import shutil
 
 import gitignorefile
 
 from .. import constants, utils
 
 
 def _list_files(
@@ -54,64 +55,65 @@
 
 
 def push(
     session: utils.CustomSession,
     message: str,
     main_file_path: str,
     model_directory_path: str,
+    export_path: str = None
 ):
     project_name = utils.read_project_name()
     push_token = utils.read_token()
 
     fds = []
 
     try:
         with tempfile.NamedTemporaryFile(prefix="submission-", suffix=".tar", dir=constants.DOT_CRUNCHDAO_DIRECTORY) as tmp:
             with tarfile.open(fileobj=tmp, mode="w") as tar:
                 for file in _list_code_files(model_directory_path):
                     print(f"compress {file}")
                     tar.add(file)
 
-            model_files = []
+            fd = open(tmp.name, "rb")
+            fds.append(fd)
+
+            files = [
+                ("codeFile", ('code.tar', fd, "application/x-tar"))
+            ]
 
             for path, name in _list_model_files(model_directory_path):
                 print(f"model {name}")
 
                 fd = open(path, "rb")
                 fds.append(fd)
 
-                model_files.append((name, fd))
-
-            tmp_fd = open(tmp.name, "rb")
-            fds.append(tmp_fd)
+                files.append(("modelFiles", (name, fd)))
 
-            files = [
-                ("codeFile", ('code.tar', tmp_fd, "application/x-tar"))
-            ]
+            if export_path:
+                print(f"export {export_path}")
+                shutil.copyfile(tmp.name, export_path)
+            else:
+                print(f"export project/{project_name}")
+                submission = session.post(
+                    f"/v1/projects/{project_name}/submissions",
+                    data={
+                        "message": message,
+                        "mainFilePath": main_file_path,
+                        "modelDirectoryPath": model_directory_path,
+                        "pushToken": push_token,
+                        "notebook": False
+                    },
+                    files=tuple(files)
+                ).json()
 
-            for model_file in model_files:
-                files.append(("modelFiles", model_file))
-
-            submission = session.post(
-                f"/v1/projects/{project_name}/submissions",
-                data={
-                    "message": message,
-                    "mainFilePath": main_file_path,
-                    "modelDirectoryPath": model_directory_path,
-                    "pushToken": push_token,
-                    "notebook": False
-                },
-                files=tuple(files)
-            ).json()
+                return submission
     finally:
         for fd in fds:
             fd.close()
 
-    return submission
-
 
 def push_summary(submission, session: utils.CustomSession):
     print("\n---")
     print(f"submission #{submission['number']} succesfully uploaded!")
 
     url = session.format_web_url(f"/project/submissions/{submission['number']}")
     print(f"Find it on your dashboard: {url}")
```

### Comparing `crunch-cli-1.4.2/crunch/command/setup.py` & `crunch-cli-1.4.3/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/command/test.py` & `crunch-cli-1.4.3/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/constants.py` & `crunch-cli-1.4.3/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/demo-project/.gitignore` & `crunch-cli-1.4.3/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/demo-project/main.py` & `crunch-cli-1.4.3/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/ensure.py` & `crunch-cli-1.4.3/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/inline.py` & `crunch-cli-1.4.3/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/library.py` & `crunch-cli-1.4.3/crunch/library.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/main.py` & `crunch-cli-1.4.3/crunch/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,18 +79,20 @@
     print(f" - To see all of the available commands of the CrunchDAO CLI, run: crunch --help")
 
 
 @cli.command(help="Send the new submission of your code.")
 @click.option("-m", "--message", prompt=True, default="", help="Specify the change of your code. (like a commit message)")
 @click.option("--main-file", "main_file_path", default="main.py", show_default=True, help="Entrypoint of your code.")
 @click.option("--model-directory", "model_directory_path", default="resources", show_default=True, help="Directory where your model is stored.")
+@click.option("--export", "export_path", show_default=True, type=str, help="Copy the `.tar` to the specified file")
 def push(
     message: str,
     main_file_path: str,
     model_directory_path: str,
+    export_path: str,
 ):
     utils.change_root()
 
     converted = False
     if not os.path.exists(main_file_path):
         print(f"missing {main_file_path}")
 
@@ -109,17 +111,19 @@
 
     try:
         submission = command.push(
             session,
             message=message,
             main_file_path=main_file_path,
             model_directory_path=model_directory_path,
+            export_path=export_path,
         )
 
-        command.push_summary(submission, session)
+        if submission:
+            command.push_summary(submission, session)
     finally:
         if converted:
             os.unlink(main_file_path)
 
 
 @cli.command(help="Test your code locally.")
 @click.option("--main-file", "main_file_path", default="main.py", show_default=True, help="Entrypoint of your code.")
```

### Comparing `crunch-cli-1.4.2/crunch/tester.py` & `crunch-cli-1.4.3/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch/utils.py` & `crunch-cli-1.4.3/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.4.3/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.2/setup.py` & `crunch-cli-1.4.3/setup.py`

 * *Files identical despite different names*

