# Comparing `tmp/cryton_cli-2022.2.1.tar.gz` & `tmp/cryton_cli-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryton_cli-2022.2.1.tar", max compression
+gzip compressed data, was "cryton_cli-2023.1.0.tar", max compression
```

## Comparing `cryton_cli-2022.2.1.tar` & `cryton_cli-2023.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1075 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/LICENSE
--rw-r--r--   0        0        0     9215 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/README.md
--rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/etc/__init__.py
--rw-r--r--   0        0        0      573 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/etc/config.py
--rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/__init__.py
--rwxr-xr-x   0        0        0     2468 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/cli.py
--rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/commands/__init__.py
--rw-r--r--   0        0        0      341 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/commands/dynamic_runs.py
--rw-r--r--   0        0        0     5034 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/commands/execution_variable.py
--rw-r--r--   0        0        0     1647 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/commands/log.py
--rw-r--r--   0        0        0    14687 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/commands/plan.py
--rw-r--r--   0        0        0     5040 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/commands/plan_template.py
--rw-r--r--   0        0        0    13020 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/commands/run.py
--rw-r--r--   0        0        0    13483 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/commands/stage.py
--rw-r--r--   0        0        0    13255 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/commands/step.py
--rw-r--r--   0        0        0     4840 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/commands/worker.py
--rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/util/__init__.py
--rw-r--r--   0        0        0     6553 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/util/api.py
--rw-r--r--   0        0        0       82 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/util/constants.py
--rw-r--r--   0        0        0    11462 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/cryton_cli/lib/util/util.py
--rw-r--r--   0        0        0     1150 2023-02-08 20:29:51.389499 cryton_cli-2022.2.1/pyproject.toml
--rw-r--r--   0        0        0    10591 1970-01-01 00:00:00.000000 cryton_cli-2022.2.1/setup.py
--rw-r--r--   0        0        0    10411 1970-01-01 00:00:00.000000 cryton_cli-2022.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/LICENSE
+-rw-r--r--   0        0        0     1629 2023-03-09 11:37:14.195759 cryton_cli-2023.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/etc/__init__.py
+-rw-r--r--   0        0        0      601 2023-03-03 18:48:26.810411 cryton_cli-2023.1.0/cryton_cli/etc/config.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/__init__.py
+-rwxr-xr-x   0        0        0     2468 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/cli.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/__init__.py
+-rw-r--r--   0        0        0      341 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/dynamic_runs.py
+-rw-r--r--   0        0        0     5034 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/execution_variable.py
+-rw-r--r--   0        0        0     1647 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/log.py
+-rw-r--r--   0        0        0    14687 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/plan.py
+-rw-r--r--   0        0        0     5040 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/plan_template.py
+-rw-r--r--   0        0        0    13020 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/run.py
+-rw-r--r--   0        0        0    13483 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/stage.py
+-rw-r--r--   0        0        0    13255 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/step.py
+-rw-r--r--   0        0        0     4840 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/worker.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/util/__init__.py
+-rw-r--r--   0        0        0     6553 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/util/api.py
+-rw-r--r--   0        0        0       82 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/util/constants.py
+-rw-r--r--   0        0        0    11462 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/util/util.py
+-rw-r--r--   0        0        0     1170 2023-03-09 11:37:14.195759 cryton_cli-2023.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 cryton_cli-2023.1.0/setup.py
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 cryton_cli-2023.1.0/PKG-INFO
```

### Comparing `cryton_cli-2022.2.1/LICENSE` & `cryton_cli-2023.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/cli.py` & `cryton_cli-2023.1.0/cryton_cli/lib/cli.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/commands/execution_variable.py` & `cryton_cli-2023.1.0/cryton_cli/lib/commands/execution_variable.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/commands/log.py` & `cryton_cli-2023.1.0/cryton_cli/lib/commands/log.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/commands/plan.py` & `cryton_cli-2023.1.0/cryton_cli/lib/commands/plan.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/commands/plan_template.py` & `cryton_cli-2023.1.0/cryton_cli/lib/commands/plan_template.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/commands/run.py` & `cryton_cli-2023.1.0/cryton_cli/lib/commands/run.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/commands/stage.py` & `cryton_cli-2023.1.0/cryton_cli/lib/commands/stage.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/commands/step.py` & `cryton_cli-2023.1.0/cryton_cli/lib/commands/step.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/commands/worker.py` & `cryton_cli-2023.1.0/cryton_cli/lib/commands/worker.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/util/api.py` & `cryton_cli-2023.1.0/cryton_cli/lib/util/api.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/cryton_cli/lib/util/util.py` & `cryton_cli-2023.1.0/cryton_cli/lib/util/util.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2022.2.1/pyproject.toml` & `cryton_cli-2023.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cryton-cli"
-version = "2022.2.1"
+version = "2023.1.0"
 description = "Command line interface for Cryton Core"
 authors = [
     "Ivo Nutár <nutar@ics.muni.cz>",
     "Milan Boháček <bohacek@ics.muni.cz>",
     "Jiří Rája <raja@ics.muni.cz>",
     "Andrej Tomči <tomci@ics.muni.cz>"
 ]
@@ -18,30 +18,31 @@
 documentation = "https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/"
 keywords = [
     "cryton", "cli", "client"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-PyYAML = "~6.0"
-Jinja2 = "~3.0.3"
-pyfiglet = "~0.8.post1"
-termcolor = "~1.1.0"
-requests = "~2.27.0"
-click = "~8.1.2"
-tzlocal = "~4.1"
-pytz = "~2021.3"
-python-dotenv = "~0.20.0"
+python = ">=3.8,<3.12"
+PyYAML = "^6.0"
+Jinja2 = "^3.0.3"
+pyfiglet = "^0.8.post1"
+termcolor = "^2.2.0"
+requests = "^2.27.0"
+click = "^8.1.2"
+tzlocal = "^4.1"
+pytz = "^2022.7"
+python-dotenv = "^1.0.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "~6.2.5"
-pytest-cov = "~3.0.0"
-pytest-mock = "~3.6.1"
-requests-mock = "~1.9.3"
+[tool.poetry.group.dev.dependencies]
+pytest = "^6.2.5"
+pytest-cov = "^3.0.0"
+pytest-mock = "^3.6.1"
+requests-mock = "^1.9.3"
+tox = "^4.4.4"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 cryton-cli = 'cryton_cli.lib.cli:cli'
```

