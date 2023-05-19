# Comparing `tmp/recon_cli-0.0.2.tar.gz` & `tmp/recon_cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recon_cli-0.0.2.tar", last modified: Wed May 17 02:19:21 2023, max compression
+gzip compressed data, was "recon_cli-0.0.3.tar", last modified: Fri May 19 03:28:00 2023, max compression
```

## Comparing `recon_cli-0.0.2.tar` & `recon_cli-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       51 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.flake8
--rw-r--r--   0        0        0      231 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      655 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      625 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.github/workflows/tox.yml
--rw-r--r--   0        0        0      948 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.gitignore
--rw-r--r--   0        0        0      563 2023-05-17 02:19:21.000000 recon_cli-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1069 2023-05-17 02:19:21.000000 recon_cli-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1225 2023-05-17 02:19:21.000000 recon_cli-0.0.2/README.md
--rw-r--r--   0        0        0      911 2023-05-17 02:19:21.000000 recon_cli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       99 2023-05-17 02:19:21.000000 recon_cli-0.0.2/recon/__init__.py
--rw-r--r--   0        0        0     9837 2023-05-17 02:19:21.000000 recon_cli-0.0.2/recon/main.py
--rw-r--r--   0        0        0      364 2023-05-17 02:19:21.000000 recon_cli-0.0.2/recon/utils.py
--rw-r--r--   0        0        0     1058 2023-05-17 02:19:21.000000 recon_cli-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-17 02:19:21.000000 recon_cli-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3113 2023-05-17 02:19:21.000000 recon_cli-0.0.2/tests/test_main.py
--rw-r--r--   0        0        0      385 2023-05-17 02:19:21.000000 recon_cli-0.0.2/tox.ini
--rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 recon_cli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.flake8
+-rw-r--r--   0        0        0      231 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      655 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      625 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.github/workflows/tox.yml
+-rw-r--r--   0        0        0      948 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.gitignore
+-rw-r--r--   0        0        0      563 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1069 2023-05-19 03:28:00.000000 recon_cli-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1225 2023-05-19 03:28:00.000000 recon_cli-0.0.3/README.md
+-rw-r--r--   0        0        0      938 2023-05-19 03:28:00.000000 recon_cli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-05-19 03:28:00.000000 recon_cli-0.0.3/recon/__init__.py
+-rw-r--r--   0        0        0     4306 2023-05-19 03:28:00.000000 recon_cli-0.0.3/recon/__main__.py
+-rw-r--r--   0        0        0     9837 2023-05-19 03:28:00.000000 recon_cli-0.0.3/recon/reconcile.py
+-rw-r--r--   0        0        0      364 2023-05-19 03:28:00.000000 recon_cli-0.0.3/recon/utils.py
+-rw-r--r--   0        0        0     1058 2023-05-19 03:28:00.000000 recon_cli-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-19 03:28:00.000000 recon_cli-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     3113 2023-05-19 03:28:00.000000 recon_cli-0.0.3/tests/test_main.py
+-rw-r--r--   0        0        0      385 2023-05-19 03:28:00.000000 recon_cli-0.0.3/tox.ini
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 recon_cli-0.0.3/PKG-INFO
```

### Comparing `recon_cli-0.0.2/.github/workflows/publish.yml` & `recon_cli-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.2/.github/workflows/tox.yml` & `recon_cli-0.0.3/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.2/.gitignore` & `recon_cli-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.2/.pre-commit-config.yaml` & `recon_cli-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.2/LICENSE.txt` & `recon_cli-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.2/README.md` & `recon_cli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.2/pyproject.toml` & `recon_cli-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "recon-cli"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Mynhardt Burger", email="mynhardt+recon@gmail.com" },
 ]
 description = "Simple reconciliation of two lists based on a common field"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -13,15 +13,16 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Financial and Insurance Industry",
     "Natural Language :: English"]
 
 dependencies = [
     "pandas == 2.0.1",
     "pandas[performance] == 2.0.1",
-    "pandas[excel] == 2.0.1"
+    "pandas[excel] == 2.0.1",
+    "typer[all] == 0.9.0"
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest >=2.7.3",
     "pytest-cov",
 ]
```

### Comparing `recon_cli-0.0.2/recon/main.py` & `recon_cli-0.0.3/recon/reconcile.py`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.2/requirements.txt` & `recon_cli-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.2/tests/test_main.py` & `recon_cli-0.0.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.2/PKG-INFO` & `recon_cli-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: recon-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple reconciliation of two lists based on a common field
 Author-email: Mynhardt Burger <mynhardt+recon@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Natural Language :: English
 Requires-Dist: pandas == 2.0.1
 Requires-Dist: pandas[performance] == 2.0.1
 Requires-Dist: pandas[excel] == 2.0.1
+Requires-Dist: typer[all] == 0.9.0
 Requires-Dist: pytest >=2.7.3 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Project-URL: Homepage, https://github.com/mynhardtburger/recon-cli
 Provides-Extra: test
 
 # recon-cli: Simple command line tool to reconcile lists
```

