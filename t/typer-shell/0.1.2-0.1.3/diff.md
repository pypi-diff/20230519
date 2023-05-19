# Comparing `tmp/typer_shell-0.1.2.tar.gz` & `tmp/typer_shell-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_shell-0.1.2.tar", max compression
+gzip compressed data, was "typer_shell-0.1.3.tar", max compression
```

## Comparing `typer_shell-0.1.2.tar` & `typer_shell-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1653 2023-05-19 12:57:58.395975 typer_shell-0.1.2/README.md
--rw-r--r--   0        0        0      536 2023-05-19 13:22:54.192091 typer_shell-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       74 2023-05-19 12:45:11.119837 typer_shell-0.1.2/typer_shell/__init__.py
--rw-r--r--   0        0        0     6488 2023-05-19 13:22:01.260153 typer_shell-0.1.2/typer_shell/typer_shell.py
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 typer_shell-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1653 2023-05-19 12:57:58.395975 typer_shell-0.1.3/README.md
+-rw-r--r--   0        0        0      536 2023-05-19 13:39:07.529997 typer_shell-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-05-19 12:45:11.119837 typer_shell-0.1.3/typer_shell/__init__.py
+-rw-r--r--   0        0        0     6512 2023-05-19 13:38:31.227495 typer_shell-0.1.3/typer_shell/typer_shell.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 typer_shell-0.1.3/PKG-INFO
```

### Comparing `typer_shell-0.1.2/README.md` & `typer_shell-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `typer_shell-0.1.2/pyproject.toml` & `typer_shell-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-shell"
-version = "0.1.2"
+version = "0.1.3"
 description = "A shell for typer apps with autocompletion and history"
 authors = ["fergus <fergusfettes@gmail.com>"]
 readme = "README.md"
 packages = [{include = "typer_shell"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
```

### Comparing `typer_shell-0.1.2/typer_shell/typer_shell.py` & `typer_shell-0.1.3/typer_shell/typer_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     app = Typer()
 
     app.command(hidden=True)(help)
     app.command(hidden=True)(shell)
 
     if params and not params_path:
         params_path = Path(tempfile.NamedTemporaryFile().name)
-    params_path = Path(params_path)
+    if params_path:
+        params_path = Path(params_path)
 
     @app.callback(invoke_without_command=True)
     def main(ctx: Context):
         _obj(ctx, params, params_path, obj)
         if ctx.invoked_subcommand is None:
             shell = make_click_shell(ctx, prompt=prompt, intro=intro)
             shell.default = _default
```

### Comparing `typer_shell-0.1.2/PKG-INFO` & `typer_shell-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-shell
-Version: 0.1.2
+Version: 0.1.3
 Summary: A shell for typer apps with autocompletion and history
 Author: fergus
 Author-email: fergusfettes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

