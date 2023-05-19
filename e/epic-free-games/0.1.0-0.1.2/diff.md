# Comparing `tmp/epic_free_games-0.1.0.tar.gz` & `tmp/epic_free_games-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epic_free_games-0.1.0.tar", max compression
+gzip compressed data, was "epic_free_games-0.1.2.tar", max compression
```

## Comparing `epic_free_games-0.1.0.tar` & `epic_free_games-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       44 2023-05-19 03:47:03.477629 epic_free_games-0.1.0/README.md
--rw-r--r--   0        0        0       58 2023-05-19 03:47:03.477629 epic_free_games-0.1.0/epic_free_games/__init__.py
--rw-r--r--   0        0        0     2242 2023-05-19 03:47:03.477629 epic_free_games-0.1.0/epic_free_games/epic_games.py
--rw-r--r--   0        0        0      546 2023-05-19 03:47:03.481629 epic_free_games-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 epic_free_games-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      784 2023-05-19 15:16:40.669869 epic_free_games-0.1.2/README.md
+-rw-r--r--   0        0        0       65 2023-05-19 15:16:40.669869 epic_free_games-0.1.2/epic_free_games/__init__.py
+-rw-r--r--   0        0        0     2242 2023-05-19 15:16:40.669869 epic_free_games-0.1.2/epic_free_games/epic_games.py
+-rw-r--r--   0        0        0      546 2023-05-19 15:16:40.669869 epic_free_games-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 epic_free_games-0.1.2/PKG-INFO
```

### Comparing `epic_free_games-0.1.0/epic_free_games/epic_games.py` & `epic_free_games-0.1.2/epic_free_games/epic_games.py`

 * *Files identical despite different names*

### Comparing `epic_free_games-0.1.0/pyproject.toml` & `epic_free_games-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epic-free-games"
-version = "0.1.0"
+version = "0.1.2"
 description = "A wrapper for Epic Games Store free games"
 authors = ["Hudson Brendon <contato.hudsonbrendon@gmail.com>"]
 readme = "README.md"
 packages = [{include = "epic_free_games"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

