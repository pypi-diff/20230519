# Comparing `tmp/llmspec-0.1.0.tar.gz` & `tmp/llmspec-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmspec-0.1.0.tar", last modified: Tue May 16 08:20:54 2023, max compression
+gzip compressed data, was "llmspec-0.2.0.tar", last modified: Fri May 19 04:35:47 2023, max compression
```

## Comparing `llmspec-0.1.0.tar` & `llmspec-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11098 2023-05-16 08:20:37.747546 llmspec-0.1.0/LICENSE
--rw-r--r--   0        0        0       33 2023-05-16 08:20:37.747546 llmspec-0.1.0/README.md
--rw-r--r--   0        0        0       98 2023-05-16 08:20:37.747546 llmspec-0.1.0/llmspec/__init__.py
--rw-r--r--   0        0        0     3519 2023-05-16 08:20:37.747546 llmspec-0.1.0/llmspec/llmspec.py
--rw-r--r--   0        0        0      699 2023-05-16 08:20:54.527629 llmspec-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-16 08:20:37.747546 llmspec-0.1.0/tests/dummy_test.py
--rw-r--r--   0        0        0      249 1970-01-01 00:00:00.000000 llmspec-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11098 2023-05-19 04:35:37.579458 llmspec-0.2.0/LICENSE
+-rw-r--r--   0        0        0       33 2023-05-19 04:35:37.579458 llmspec-0.2.0/README.md
+-rw-r--r--   0        0        0      461 2023-05-19 04:35:37.579458 llmspec-0.2.0/llmspec/__init__.py
+-rw-r--r--   0        0        0     8693 2023-05-19 04:35:37.579458 llmspec-0.2.0/llmspec/llmspec.py
+-rw-r--r--   0        0        0     1056 2023-05-19 04:35:47.575492 llmspec-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-19 04:35:37.579458 llmspec-0.2.0/tests/dummy_test.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.2.0/PKG-INFO
```

### Comparing `llmspec-0.1.0/LICENSE` & `llmspec-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmspec-0.1.0/pyproject.toml` & `llmspec-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 [project]
 name = "llmspec"
-version = "0.1.0"
+dynamic = []
 description = "LLM unified interface"
 authors = [
     { name = "TensorChord", email = "modelz@tensorchord.ai" },
 ]
-dependencies = []
-requires-python = ">=3.7"
+keywords = [
+    "machine learning",
+    "deep learning",
+    "large language model",
+]
+classifiers = [
+    "Intended Audience :: Developers",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+]
+dependencies = [
+    "msgspec>=0.15.0",
+]
+requires-python = ">=3.8"
 readme = "README.md"
+version = "0.2.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
+[tool.pdm.version]
+source = "scm"
+write_to = "llmspec/__version__.py"
+write_template = "__version__ = '{}'"
+
 [tool.pdm.dev-dependencies]
 lint = [
     "ruff>=0.0.267",
     "black>=23.3.0",
 ]
 test = [
     "pytest>=7.3.1",
```

