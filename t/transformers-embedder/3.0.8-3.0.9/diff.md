# Comparing `tmp/transformers_embedder-3.0.8.tar.gz` & `tmp/transformers_embedder-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_embedder-3.0.8.tar", last modified: Thu Nov  3 11:43:19 2022, max compression
+gzip compressed data, was "transformers_embedder-3.0.9.tar", last modified: Fri May 19 07:49:54 2023, max compression
```

## Comparing `transformers_embedder-3.0.8.tar` & `transformers_embedder-3.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 11:43:19.353803 transformers_embedder-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13104 2022-11-03 11:43:19.357802 transformers_embedder-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12477 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-03 11:43:19.357802 transformers_embedder-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 11:43:19.353803 transformers_embedder-3.0.8/transformers_embedder/
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/transformers_embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20983 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/transformers_embedder/embedder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 11:43:19.353803 transformers_embedder-3.0.8/transformers_embedder/modules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/transformers_embedder/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/transformers_embedder/modules/encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3866 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/transformers_embedder/modules/scalar_mix.py
--rw-r--r--   0 runner    (1001) docker     (121)    27468 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/transformers_embedder/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-11-03 11:42:53.000000 transformers_embedder-3.0.8/transformers_embedder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 11:43:19.353803 transformers_embedder-3.0.8/transformers_embedder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13104 2022-11-03 11:43:19.000000 transformers_embedder-3.0.8/transformers_embedder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-11-03 11:43:19.000000 transformers_embedder-3.0.8/transformers_embedder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 11:43:19.000000 transformers_embedder-3.0.8/transformers_embedder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-03 11:43:19.000000 transformers_embedder-3.0.8/transformers_embedder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-03 11:43:19.000000 transformers_embedder-3.0.8/transformers_embedder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:54.975232 transformers_embedder-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-05-19 07:49:54.975232 transformers_embedder-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 07:49:54.975232 transformers_embedder-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:54.971232 transformers_embedder-3.0.9/transformers_embedder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/transformers_embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/transformers_embedder/embedder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:54.975232 transformers_embedder-3.0.9/transformers_embedder/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/transformers_embedder/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/transformers_embedder/modules/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/transformers_embedder/modules/scalar_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27468 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/transformers_embedder/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-19 07:49:38.000000 transformers_embedder-3.0.9/transformers_embedder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:54.975232 transformers_embedder-3.0.9/transformers_embedder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-05-19 07:49:54.000000 transformers_embedder-3.0.9/transformers_embedder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-19 07:49:54.000000 transformers_embedder-3.0.9/transformers_embedder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:49:54.000000 transformers_embedder-3.0.9/transformers_embedder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-19 07:49:54.000000 transformers_embedder-3.0.9/transformers_embedder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 07:49:54.000000 transformers_embedder-3.0.9/transformers_embedder.egg-info/top_level.txt
```

### Comparing `transformers_embedder-3.0.8/PKG-INFO` & `transformers_embedder-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers_embedder
-Version: 3.0.8
+Version: 3.0.9
 Summary: Word level transformer based embeddings
 Home-page: https://github.com/Riccorl/transformers-embedder
 Author: Riccardo Orlando
 Author-email: orlandoricc@gmail.com
 License: Apache
 Keywords: NLP deep learning transformer pytorch BERT google subtoken wordpieces embeddings
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 
 <div align="center">
 
 # Transformers Embedder
 
 [![Open in Visual Studio Code](https://img.shields.io/badge/preview%20in-vscode.dev-blue)](https://github.dev/Riccorl/transformers-embedder)
 [![PyTorch](https://img.shields.io/badge/PyTorch-orange?logo=pytorch)](https://pytorch.org/)
-[![Transformers](https://img.shields.io/badge/4.24-🤗%20Transformers-6670ff)](https://huggingface.co/transformers/)
+[![Transformers](https://img.shields.io/badge/4.28-🤗%20Transformers-6670ff)](https://huggingface.co/transformers/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
 
 [![Upload to PyPi](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-pypi.yml/badge.svg)](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-pypi.yml)
 [![Upload to PyPi](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-conda.yml/badge.svg)](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-conda.yml)
 [![PyPi Version](https://img.shields.io/github/v/release/Riccorl/transformers-embedder)](https://github.com/Riccorl/transformers-embedder/releases)
 [![Anaconda-Server Badge](https://anaconda.org/riccorl/transformers-embedder/badges/version.svg)](https://anaconda.org/riccorl/transformers-embedder)
 [![DeepSource](https://deepsource.io/gh/Riccorl/transformers-embedder.svg/?label=active+issues)](https://deepsource.io/gh/Riccorl/transformers-embedder/?ref=repository-badge)
```

### Comparing `transformers_embedder-3.0.8/README.md` & `transformers_embedder-3.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align="center">
 
 # Transformers Embedder
 
 [![Open in Visual Studio Code](https://img.shields.io/badge/preview%20in-vscode.dev-blue)](https://github.dev/Riccorl/transformers-embedder)
 [![PyTorch](https://img.shields.io/badge/PyTorch-orange?logo=pytorch)](https://pytorch.org/)
-[![Transformers](https://img.shields.io/badge/4.24-🤗%20Transformers-6670ff)](https://huggingface.co/transformers/)
+[![Transformers](https://img.shields.io/badge/4.28-🤗%20Transformers-6670ff)](https://huggingface.co/transformers/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
 
 [![Upload to PyPi](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-pypi.yml/badge.svg)](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-pypi.yml)
 [![Upload to PyPi](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-conda.yml/badge.svg)](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-conda.yml)
 [![PyPi Version](https://img.shields.io/github/v/release/Riccorl/transformers-embedder)](https://github.com/Riccorl/transformers-embedder/releases)
 [![Anaconda-Server Badge](https://anaconda.org/riccorl/transformers-embedder/badges/version.svg)](https://anaconda.org/riccorl/transformers-embedder)
 [![DeepSource](https://deepsource.io/gh/Riccorl/transformers-embedder.svg/?label=active+issues)](https://deepsource.io/gh/Riccorl/transformers-embedder/?ref=repository-badge)
```

### Comparing `transformers_embedder-3.0.8/setup.py` & `transformers_embedder-3.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 extras = {}
-extras["torch"] = ["torch>=1.5,<1.14"]
+extras["torch"] = ["torch>=1.5,<2.1"]
 extras["all"] = extras["torch"]
 extras["docs"] = ["mkdocs-material"]
 
-install_requires = ["transformers>=4.14,<4.25"]
+install_requires = ["transformers>=4.14,<4.29"]
 
 setuptools.setup(
     name="transformers_embedder",
-    version="3.0.8",
+    version="3.0.9",
     author="Riccardo Orlando",
     author_email="orlandoricc@gmail.com",
     description="Word level transformer based embeddings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Riccorl/transformers-embedder",
     keywords="NLP deep learning transformer pytorch BERT google subtoken wordpieces embeddings",
```

### Comparing `transformers_embedder-3.0.8/transformers_embedder/__init__.py` & `transformers_embedder-3.0.9/transformers_embedder/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers_embedder-3.0.8/transformers_embedder/embedder.py` & `transformers_embedder-3.0.9/transformers_embedder/embedder.py`

 * *Files identical despite different names*

### Comparing `transformers_embedder-3.0.8/transformers_embedder/modules/encoder.py` & `transformers_embedder-3.0.9/transformers_embedder/modules/encoder.py`

 * *Files identical despite different names*

### Comparing `transformers_embedder-3.0.8/transformers_embedder/modules/scalar_mix.py` & `transformers_embedder-3.0.9/transformers_embedder/modules/scalar_mix.py`

 * *Files identical despite different names*

### Comparing `transformers_embedder-3.0.8/transformers_embedder/tokenizer.py` & `transformers_embedder-3.0.9/transformers_embedder/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transformers_embedder-3.0.8/transformers_embedder.egg-info/PKG-INFO` & `transformers_embedder-3.0.9/transformers_embedder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-embedder
-Version: 3.0.8
+Version: 3.0.9
 Summary: Word level transformer based embeddings
 Home-page: https://github.com/Riccorl/transformers-embedder
 Author: Riccardo Orlando
 Author-email: orlandoricc@gmail.com
 License: Apache
 Keywords: NLP deep learning transformer pytorch BERT google subtoken wordpieces embeddings
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 
 <div align="center">
 
 # Transformers Embedder
 
 [![Open in Visual Studio Code](https://img.shields.io/badge/preview%20in-vscode.dev-blue)](https://github.dev/Riccorl/transformers-embedder)
 [![PyTorch](https://img.shields.io/badge/PyTorch-orange?logo=pytorch)](https://pytorch.org/)
-[![Transformers](https://img.shields.io/badge/4.24-🤗%20Transformers-6670ff)](https://huggingface.co/transformers/)
+[![Transformers](https://img.shields.io/badge/4.28-🤗%20Transformers-6670ff)](https://huggingface.co/transformers/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
 
 [![Upload to PyPi](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-pypi.yml/badge.svg)](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-pypi.yml)
 [![Upload to PyPi](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-conda.yml/badge.svg)](https://github.com/Riccorl/transformers-embedder/actions/workflows/python-publish-conda.yml)
 [![PyPi Version](https://img.shields.io/github/v/release/Riccorl/transformers-embedder)](https://github.com/Riccorl/transformers-embedder/releases)
 [![Anaconda-Server Badge](https://anaconda.org/riccorl/transformers-embedder/badges/version.svg)](https://anaconda.org/riccorl/transformers-embedder)
 [![DeepSource](https://deepsource.io/gh/Riccorl/transformers-embedder.svg/?label=active+issues)](https://deepsource.io/gh/Riccorl/transformers-embedder/?ref=repository-badge)
```

### Comparing `transformers_embedder-3.0.8/transformers_embedder.egg-info/SOURCES.txt` & `transformers_embedder-3.0.9/transformers_embedder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

