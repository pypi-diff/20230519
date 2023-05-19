# Comparing `tmp/new-component-0.4.0.tar.gz` & `tmp/new-component-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new-component-0.4.0.tar", last modified: Fri May 19 21:18:43 2023, max compression
+gzip compressed data, was "new-component-0.4.2.tar", last modified: Fri May 19 21:35:18 2023, max compression
```

## Comparing `new-component-0.4.0.tar` & `new-component-0.4.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-05-19 21:18:20.306099 new-component-0.4.0/LICENSE
--rw-r--r--   0        0        0     4705 2023-05-19 21:18:20.306099 new-component-0.4.0/README.md
--rw-r--r--   0        0        0     1595 2023-05-19 21:18:20.306099 new-component-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6187 2023-05-19 21:18:20.306099 new-component-0.4.0/tests/test_new_component.py
--rw-r--r--   0        0        0      491 2023-05-19 21:18:20.306099 new-component-0.4.0/tests/test_version.py
--rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 new-component-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-19 21:34:56.459287 new-component-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4798 2023-05-19 21:34:56.459287 new-component-0.4.2/README.md
+-rw-r--r--   0        0        0     1660 2023-05-19 21:34:56.463287 new-component-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6187 2023-05-19 21:34:56.463287 new-component-0.4.2/tests/test_new_component.py
+-rw-r--r--   0        0        0      491 2023-05-19 21:34:56.463287 new-component-0.4.2/tests/test_version.py
+-rw-r--r--   0        0        0     5053 1970-01-01 00:00:00.000000 new-component-0.4.2/PKG-INFO
```

### Comparing `new-component-0.4.0/LICENSE` & `new-component-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `new-component-0.4.0/README.md` & `new-component-0.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # new-component
 
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 Ian Cleary ([iancleary](https://iancleary.me))
 
 ## Description
```

### Comparing `new-component-0.4.0/pyproject.toml` & `new-component-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "new-component"
-version = "0.4.0"
+version = "0.4.2"
 description = "Quickly create opinionated Styled Components for React Projects"
 authors = [
     { name = "Ian Cleary", email = "github@iancleary.me" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dependencies = [
@@ -14,14 +14,17 @@
     "rich==13.3.5",
     "Jinja2==3.1.2",
 ]
 
 [project.license]
 text = "MIT"
 
+[project.scripts]
+new-component = "new_component.__main__:main"
+
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest==7.2.0",
     "black==22.10.0",
     "mypy==0.990",
     "ruff==0.0.225",
     "pytest-pretty==1.2.0",
```

### Comparing `new-component-0.4.0/tests/test_new_component.py` & `new-component-0.4.2/tests/test_new_component.py`

 * *Files identical despite different names*

### Comparing `new-component-0.4.0/PKG-INFO` & `new-component-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: new-component
-Version: 0.4.0
+Version: 0.4.2
 Summary: Quickly create opinionated Styled Components for React Projects
 License: MIT
 Author-email: Ian Cleary <github@iancleary.me>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # new-component
 
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 Ian Cleary ([iancleary](https://iancleary.me))
 
 ## Description
```

