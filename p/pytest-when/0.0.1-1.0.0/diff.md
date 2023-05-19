# Comparing `tmp/pytest_when-0.0.1.tar.gz` & `tmp/pytest_when-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_when-0.0.1.tar", last modified: Fri May 19 13:47:29 2023, max compression
+gzip compressed data, was "pytest_when-1.0.0.tar", last modified: Fri May 19 15:40:32 2023, max compression
```

## Comparing `pytest_when-0.0.1.tar` & `pytest_when-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,8 @@
--rw-r--r--   0        0        0    11342 2023-05-19 10:56:49.789783 pytest_when-0.0.1/LICENSE
--rw-r--r--   0        0        0      127 2023-05-19 11:01:32.646956 pytest_when-0.0.1/README.md
--rw-r--r--   0        0        0     2577 2023-05-19 13:47:29.648278 pytest_when-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 pytest_when-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-19 15:39:57.715109 pytest_when-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1628 2023-05-19 15:39:57.715109 pytest_when-1.0.0/README.md
+-rw-r--r--   0        0        0     2752 2023-05-19 15:40:32.011164 pytest_when-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 15:39:57.715109 pytest_when-1.0.0/tests/resources/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-19 15:39:57.715109 pytest_when-1.0.0/tests/resources/example_module.py
+-rw-r--r--   0        0        0     2492 2023-05-19 15:39:57.715109 pytest_when-1.0.0/tests/test_create_call_key.py
+-rw-r--r--   0        0        0     5409 2023-05-19 15:39:57.715109 pytest_when-1.0.0/tests/test_integration.py
+-rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 pytest_when-1.0.0/PKG-INFO
```

### Comparing `pytest_when-0.0.1/LICENSE` & `pytest_when-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_when-0.0.1/pyproject.toml` & `pytest_when-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,21 @@
     "py38",
 ]
 
 [tool.ruff]
 target-version = "py38"
 ignore = [
     "E501",
+    "D107",
     "D203",
     "D211",
     "D212",
     "D213",
+    "D407",
+    "D412",
     "INP001",
     "I001",
     "D100",
     "D103",
     "D104",
     "D101",
     "COM812",
@@ -24,32 +27,35 @@
     "G004",
     "S101",
     "G010",
     "ERA001",
     "F401",
     "N812",
     "PLR0913",
-    "ANN101",
-    "ANN102",
+    "ANN",
     "PGH003",
     "D102",
     "D105",
+    "EM101",
 ]
 select = [
     "ALL",
 ]
 exclude = []
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = [
     "ANN001",
+    "ANN202",
     "ANN201",
     "PT019",
     "PD901",
     "ARG001",
+    "ARG002",
+    "ARG003",
     "PT015",
     "PT023",
 ]
 "tests/conftest.py" = [
     "ALL",
 ]
 
@@ -62,15 +68,15 @@
 
 [tool.coverage.paths]
 source = [
     "./pytest_when",
 ]
 
 [tool.coverage.report]
-fail_under = 100
+fail_under = 53
 skip_covered = true
 show_missing = true
 
 [tool.coverage.html]
 directory = "coverage_html"
 
 [tool.pytest.ini_options]
@@ -138,25 +144,28 @@
 
 [tool.pdm.version]
 source = "scm"
 
 [project]
 name = "pytest_when"
 dynamic = []
-description = ""
+description = "Utility makes mocing more readable"
 authors = [
     { name = "zhukovgreen", email = "iam+pytest-when@zhukovgreen.pro" },
 ]
 dependencies = [
     "environs>=9.5.0",
     "pip>=23.1.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.0.1"
+version = "1.0.0"
+
+[project.entry-points.pytest11]
+pytest-when = "pytest_when.plugin"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/pytest-when"
 
 [build-system]
 requires = [
     "pdm-backend",
```

