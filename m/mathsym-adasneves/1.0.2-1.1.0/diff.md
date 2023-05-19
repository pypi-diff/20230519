# Comparing `tmp/mathsym_adasneves-1.0.2.tar.gz` & `tmp/mathsym_adasneves-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathsym_adasneves-1.0.2.tar", last modified: Fri May 19 00:14:09 2023, max compression
+gzip compressed data, was "mathsym_adasneves-1.1.0.tar", last modified: Fri May 19 00:32:28 2023, max compression
```

## Comparing `mathsym_adasneves-1.0.2.tar` & `mathsym_adasneves-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:14:09.799025 mathsym_adasneves-1.0.2/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-1.0.2/LICENSE
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1013 2023-05-19 00:14:09.795025 mathsym_adasneves-1.0.2/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      495 2023-05-14 18:40:24.000000 mathsym_adasneves-1.0.2/README.md
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      591 2023-05-19 00:09:20.000000 mathsym_adasneves-1.0.2/pyproject.toml
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-19 00:14:09.799025 mathsym_adasneves-1.0.2/setup.cfg
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:14:09.795025 mathsym_adasneves-1.0.2/src/
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:14:09.795025 mathsym_adasneves-1.0.2/src/mathsym_adasneves.egg-info/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1013 2023-05-19 00:14:09.000000 mathsym_adasneves-1.0.2/src/mathsym_adasneves.egg-info/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      437 2023-05-19 00:14:09.000000 mathsym_adasneves-1.0.2/src/mathsym_adasneves.egg-info/SOURCES.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-19 00:14:09.000000 mathsym_adasneves-1.0.2/src/mathsym_adasneves.egg-info/dependency_links.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-19 00:14:09.000000 mathsym_adasneves-1.0.2/src/mathsym_adasneves.egg-info/top_level.txt
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:14:09.795025 mathsym_adasneves-1.0.2/src/symMath_adasneves127/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:08:33.000000 mathsym_adasneves-1.0.2/src/symMath_adasneves127/__init__.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1089 2023-05-19 00:09:20.000000 mathsym_adasneves-1.0.2/src/symMath_adasneves127/equation.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-19 00:13:51.000000 mathsym_adasneves-1.0.2/src/symMath_adasneves127/token.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1762 2023-05-19 00:09:20.000000 mathsym_adasneves-1.0.2/src/symMath_adasneves127/token_maker.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     3438 2023-05-19 00:09:20.000000 mathsym_adasneves-1.0.2/src/symMath_adasneves127/tree_maker.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     2242 2023-05-19 00:09:20.000000 mathsym_adasneves-1.0.2/src/symMath_adasneves127/tree_node.py
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:32:28.255805 mathsym_adasneves-1.1.0/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-1.1.0/LICENSE
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1744 2023-05-19 00:32:28.255805 mathsym_adasneves-1.1.0/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1226 2023-05-19 00:28:33.000000 mathsym_adasneves-1.1.0/README.md
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      591 2023-05-19 00:32:11.000000 mathsym_adasneves-1.1.0/pyproject.toml
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-19 00:32:28.255805 mathsym_adasneves-1.1.0/setup.cfg
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:32:28.251804 mathsym_adasneves-1.1.0/src/
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:32:28.251804 mathsym_adasneves-1.1.0/src/mathsym_adasneves.egg-info/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1744 2023-05-19 00:32:28.000000 mathsym_adasneves-1.1.0/src/mathsym_adasneves.egg-info/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      437 2023-05-19 00:32:28.000000 mathsym_adasneves-1.1.0/src/mathsym_adasneves.egg-info/SOURCES.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-19 00:32:28.000000 mathsym_adasneves-1.1.0/src/mathsym_adasneves.egg-info/dependency_links.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-19 00:32:28.000000 mathsym_adasneves-1.1.0/src/mathsym_adasneves.egg-info/top_level.txt
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:32:28.251804 mathsym_adasneves-1.1.0/src/symMath_adasneves127/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:08:33.000000 mathsym_adasneves-1.1.0/src/symMath_adasneves127/__init__.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1089 2023-05-19 00:09:20.000000 mathsym_adasneves-1.1.0/src/symMath_adasneves127/equation.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-19 00:13:51.000000 mathsym_adasneves-1.1.0/src/symMath_adasneves127/token.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1762 2023-05-19 00:09:20.000000 mathsym_adasneves-1.1.0/src/symMath_adasneves127/token_maker.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     3438 2023-05-19 00:09:20.000000 mathsym_adasneves-1.1.0/src/symMath_adasneves127/tree_maker.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     2242 2023-05-19 00:09:20.000000 mathsym_adasneves-1.1.0/src/symMath_adasneves127/tree_node.py
```

### Comparing `mathsym_adasneves-1.0.2/LICENSE` & `mathsym_adasneves-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.0.2/pyproject.toml` & `mathsym_adasneves-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mathsym_adasneves"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
   { name="Alex Dasneves", email="adasneves@adasneves.info" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mathsym_adasneves-1.0.2/src/symMath_adasneves127/equation.py` & `mathsym_adasneves-1.1.0/src/symMath_adasneves127/equation.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.0.2/src/symMath_adasneves127/token_maker.py` & `mathsym_adasneves-1.1.0/src/symMath_adasneves127/token_maker.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.0.2/src/symMath_adasneves127/tree_maker.py` & `mathsym_adasneves-1.1.0/src/symMath_adasneves127/tree_maker.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.0.2/src/symMath_adasneves127/tree_node.py` & `mathsym_adasneves-1.1.0/src/symMath_adasneves127/tree_node.py`

 * *Files identical despite different names*

