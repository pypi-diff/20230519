# Comparing `tmp/hyperfast_python_template-0.4.9.tar.gz` & `tmp/hyperfast_python_template-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.4.9.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.5.0.tar", max compression
```

## Comparing `hyperfast_python_template-0.4.9.tar` & `hyperfast_python_template-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-05 01:02:42.633668 hyperfast_python_template-0.4.9/LICENSE
--rw-r--r--   0        0        0     2573 2023-05-05 01:02:42.633668 hyperfast_python_template-0.4.9/README.md
--rw-r--r--   0        0        0     2991 2023-05-05 01:02:59.541535 hyperfast_python_template-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      323 2023-05-05 01:02:42.637668 hyperfast_python_template-0.4.9/src/hyperfastpy/__cli__.py
--rw-r--r--   0        0        0      135 2023-05-05 01:02:42.637668 hyperfast_python_template-0.4.9/src/hyperfastpy/__init__.py
--rw-r--r--   0        0        0       22 2023-05-05 01:02:59.493535 hyperfast_python_template-0.4.9/src/hyperfastpy/_version.py
--rw-r--r--   0        0        0      272 2023-05-05 01:02:59.493535 hyperfast_python_template-0.4.9/src/hyperfastpy/conf/about/__init__.yaml
--rw-r--r--   0        0        0      243 2023-05-05 01:02:42.637668 hyperfast_python_template-0.4.9/src/hyperfastpy/project.toml
--rw-r--r--   0        0        0        0 2023-05-05 01:02:42.637668 hyperfast_python_template-0.4.9/src/hyperfastpy/py.typed
--rw-r--r--   0        0        0      242 2023-05-05 01:02:42.637668 hyperfast_python_template-0.4.9/src/hyperfastpy/pyproject.toml
--rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 hyperfast_python_template-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5490 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/README.md
+-rw-r--r--   0        0        0     2991 2023-05-19 20:33:39.062720 hyperfast_python_template-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/src/hyperfastpy/__cli__.py
+-rw-r--r--   0        0        0      135 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/src/hyperfastpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-19 20:33:39.002717 hyperfast_python_template-0.5.0/src/hyperfastpy/_version.py
+-rw-r--r--   0        0        0      272 2023-05-19 20:33:39.002717 hyperfast_python_template-0.5.0/src/hyperfastpy/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      243 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/src/hyperfastpy/project.toml
+-rw-r--r--   0        0        0        0 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/src/hyperfastpy/py.typed
+-rw-r--r--   0        0        0      242 2023-05-19 20:33:18.865937 hyperfast_python_template-0.5.0/src/hyperfastpy/pyproject.toml
+-rw-r--r--   0        0        0     6156 1970-01-01 00:00:00.000000 hyperfast_python_template-0.5.0/PKG-INFO
```

### Comparing `hyperfast_python_template-0.4.9/LICENSE` & `hyperfast_python_template-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.4.9/pyproject.toml` & `hyperfast_python_template-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.4.9"
+version = "0.5.0"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyperfast-python-template"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
@@ -15,15 +15,15 @@
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-python-semantic-release = "^7.33.1"
+python-semantic-release = "^7.33.4"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
```

