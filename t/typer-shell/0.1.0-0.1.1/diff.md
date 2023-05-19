# Comparing `tmp/typer_shell-0.1.0.tar.gz` & `tmp/typer_shell-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_shell-0.1.0.tar", max compression
+gzip compressed data, was "typer_shell-0.1.1.tar", max compression
```

## Comparing `typer_shell-0.1.0.tar` & `typer_shell-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      642 2023-05-19 12:50:05.543477 typer_shell-0.1.0/README.md
--rw-r--r--   0        0        0      528 2023-05-19 12:36:28.064572 typer_shell-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       74 2023-05-19 12:45:11.119837 typer_shell-0.1.0/typer_shell/__init__.py
--rw-r--r--   0        0        0     6444 2023-05-19 12:42:26.595094 typer_shell-0.1.0/typer_shell/typer_shell.py
--rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 typer_shell-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1653 2023-05-19 12:57:58.395975 typer_shell-0.1.1/README.md
+-rw-r--r--   0        0        0      536 2023-05-19 13:01:11.376406 typer_shell-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-05-19 12:45:11.119837 typer_shell-0.1.1/typer_shell/__init__.py
+-rw-r--r--   0        0        0     6444 2023-05-19 12:42:26.595094 typer_shell-0.1.1/typer_shell/typer_shell.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 typer_shell-0.1.1/PKG-INFO
```

### Comparing `typer_shell-0.1.0/pyproject.toml` & `typer_shell-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "typer-shell"
-version = "0.1.0"
+version = "0.1.1"
 description = "A shell for typer apps with autocompletion and history"
 authors = ["fergus <fergusfettes@gmail.com>"]
 readme = "README.md"
 packages = [{include = "typer_shell"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.8.1,<3.12"
 typer = "^0.9.0"
 click = "^8.1.3"
 rich = "^13.3.5"
 click-shell = "^2.1"
 iterfzf = "^0.5.0.20.0"
 pyyaml = "^6.0"
```

### Comparing `typer_shell-0.1.0/typer_shell/typer_shell.py` & `typer_shell-0.1.1/typer_shell/typer_shell.py`

 * *Files identical despite different names*

