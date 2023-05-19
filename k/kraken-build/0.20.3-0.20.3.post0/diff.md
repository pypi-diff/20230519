# Comparing `tmp/kraken_build-0.20.3.tar.gz` & `tmp/kraken_build-0.20.3.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_build-0.20.3.tar", max compression
+gzip compressed data, was "kraken_build-0.20.3.post0.tar", max compression
```

## Comparing `kraken_build-0.20.3.tar` & `kraken_build-0.20.3.post0.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      998 2023-05-19 08:28:35.412431 kraken_build-0.20.3/LICENSE
--rw-r--r--   0        0        0      677 2023-05-19 08:29:54.004757 kraken_build-0.20.3/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-19 08:29:38.904686 kraken_build-0.20.3/src/kraken/build/__init__.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 kraken_build-0.20.3/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-05-19 08:28:35.412431 kraken_build-0.20.3.post0/LICENSE
+-rw-r--r--   0        0        0      178 2023-05-19 08:28:35.412431 kraken_build-0.20.3.post0/README.md
+-rw-r--r--   0        0        0      704 2023-05-19 08:30:54.025024 kraken_build-0.20.3.post0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-19 08:29:38.904686 kraken_build-0.20.3.post0/src/kraken/build/__init__.py
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 kraken_build-0.20.3.post0/PKG-INFO
```

### Comparing `kraken_build-0.20.3/LICENSE` & `kraken_build-0.20.3.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_build-0.20.3/pyproject.toml` & `kraken_build-0.20.3.post0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-build"
-version = "0.20.3"
+version = "0.20.3.post0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
+readme = "README.md"
 packages = [{ include = "kraken/build", from = "src" }]
 classifiers = []
 keywords = []
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kraken-build/kraken-build/issues"
 Documentation = "https://kraken-build.github.io/kraken-build/"
```

