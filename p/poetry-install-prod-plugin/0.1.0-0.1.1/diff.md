# Comparing `tmp/poetry_install_prod_plugin-0.1.0.tar.gz` & `tmp/poetry_install_prod_plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_install_prod_plugin-0.1.0.tar", max compression
+gzip compressed data, was "poetry_install_prod_plugin-0.1.1.tar", max compression
```

## Comparing `poetry_install_prod_plugin-0.1.0.tar` & `poetry_install_prod_plugin-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1057 2023-05-19 19:14:17.794739 poetry_install_prod_plugin-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      470 2023-05-19 19:26:22.210716 poetry_install_prod_plugin-0.1.0/README.md
--rw-r--r--   0        0        0      619 2023-05-19 19:29:44.039946 poetry_install_prod_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 19:22:13.244173 poetry_install_prod_plugin-0.1.0/src/poetry_install_prod_plugin/__init__.py
--rw-r--r--   0        0        0     2975 2023-05-19 19:24:18.362452 poetry_install_prod_plugin-0.1.0/src/poetry_install_prod_plugin/plugin.py
--rw-r--r--   0        0        0        0 2023-05-19 19:23:26.041778 poetry_install_prod_plugin-0.1.0/src/poetry_install_prod_plugin/py.typed
--rw-r--r--   0        0        0     1046 1970-01-01 00:00:00.000000 poetry_install_prod_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-05-19 19:14:17.794739 poetry_install_prod_plugin-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      470 2023-05-19 19:26:22.210716 poetry_install_prod_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0      687 2023-05-19 19:40:02.927354 poetry_install_prod_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 19:22:13.244173 poetry_install_prod_plugin-0.1.1/src/poetry_install_prod_plugin/__init__.py
+-rw-r--r--   0        0        0     2975 2023-05-19 19:24:18.362452 poetry_install_prod_plugin-0.1.1/src/poetry_install_prod_plugin/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-19 19:23:26.041778 poetry_install_prod_plugin-0.1.1/src/poetry_install_prod_plugin/py.typed
+-rw-r--r--   0        0        0     1188 1970-01-01 00:00:00.000000 poetry_install_prod_plugin-0.1.1/PKG-INFO
```

### Comparing `poetry_install_prod_plugin-0.1.0/LICENSE.txt` & `poetry_install_prod_plugin-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `poetry_install_prod_plugin-0.1.0/pyproject.toml` & `poetry_install_prod_plugin-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "poetry-install-prod-plugin"
-version = "0.1.0"
+version = "0.1.1"
 description = "Adds a command which forces local (path) dependencies to be installed in non-editable mode, even when marked as editable."
 authors = ["Doeke <doekebuursma@gmail.com>"]
 license = "MIT"
+repository = "https://github.com/Doekeb/poetry-install-prod-plugin"
 readme = "README.md"
 packages = [{ include = "poetry_install_prod_plugin", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 poetry = "^1.5.0"
```

### Comparing `poetry_install_prod_plugin-0.1.0/src/poetry_install_prod_plugin/plugin.py` & `poetry_install_prod_plugin-0.1.1/src/poetry_install_prod_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_install_prod_plugin-0.1.0/PKG-INFO` & `poetry_install_prod_plugin-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: poetry-install-prod-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Adds a command which forces local (path) dependencies to be installed in non-editable mode, even when marked as editable.
+Home-page: https://github.com/Doekeb/poetry-install-prod-plugin
 License: MIT
 Author: Doeke
 Author-email: doekebuursma@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: poetry (>=1.5.0,<2.0.0)
+Project-URL: Repository, https://github.com/Doekeb/poetry-install-prod-plugin
 Description-Content-Type: text/markdown
 
 # Install Prod
 
 Adds a command `poetry install-prod` which forces local (path) dependencies to be installed in non-editable mode, even when marked as editable. This is particularly useful for monorepo architectures with many cross-dependencies. In a development environment it is desireable to install local (path) dependencies as symbolic links so they are editable, but in a production or CI/CD environment it is necessary to install all dependencies as non-editable.
```

