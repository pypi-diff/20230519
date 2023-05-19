# Comparing `tmp/pylint_actions-0.3.1.tar.gz` & `tmp/pylint_actions-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_actions-0.3.1.tar", max compression
+gzip compressed data, was "pylint_actions-0.4.0.tar", max compression
```

## Comparing `pylint_actions-0.3.1.tar` & `pylint_actions-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-04-04 17:00:14.635940 pylint_actions-0.3.1/LICENSE
--rw-r--r--   0        0        0      870 2023-04-04 17:00:14.635940 pylint_actions-0.3.1/README.md
--rw-r--r--   0        0        0     1170 2023-04-04 17:00:14.635940 pylint_actions-0.3.1/pylint_actions/__init__.py
--rw-r--r--   0        0        0     1275 2023-04-04 17:00:14.635940 pylint_actions-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2133 1970-01-01 00:00:00.000000 pylint_actions-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-19 16:26:09.231260 pylint_actions-0.4.0/LICENSE
+-rw-r--r--   0        0        0      870 2023-05-19 16:26:09.235260 pylint_actions-0.4.0/README.md
+-rw-r--r--   0        0        0     1170 2023-05-19 16:26:09.235260 pylint_actions-0.4.0/pylint_actions/__init__.py
+-rw-r--r--   0        0        0     1283 2023-05-19 16:26:09.235260 pylint_actions-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2137 1970-01-01 00:00:00.000000 pylint_actions-0.4.0/PKG-INFO
```

### Comparing `pylint_actions-0.3.1/LICENSE` & `pylint_actions-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint_actions-0.3.1/README.md` & `pylint_actions-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pylint_actions-0.3.1/pylint_actions/__init__.py` & `pylint_actions-0.4.0/pylint_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint_actions-0.3.1/pyproject.toml` & `pylint_actions-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylint-actions"
-version = "0.3.1"
+version = "0.4.0"
 description = "Pylint plugin for GitHub Actions"
 license = "MIT"
 homepage = "https://github.com/skhomuti/pylint-actions"
 repository = "https://github.com/skhomuti/pylint-actions"
 keywords = ["pylint", "github", "actions", "linter", "static code analysis", "python"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
 authors = ["skhomuti <skhomuti@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "pylint_actions"},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.7.2,<4.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pylint_actions-0.3.1/PKG-INFO` & `pylint_actions-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pylint-actions
-Version: 0.3.1
+Version: 0.4.0
 Summary: Pylint plugin for GitHub Actions
 Home-page: https://github.com/skhomuti/pylint-actions
 License: MIT
 Keywords: pylint,github,actions,linter,static code analysis,python
 Author: skhomuti
 Author-email: skhomuti@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.7.2,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Project-URL: Repository, https://github.com/skhomuti/pylint-actions
 Description-Content-Type: text/markdown
```

