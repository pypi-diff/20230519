# Comparing `tmp/sysnet-pyutils-1.0.1.tar.gz` & `tmp/sysnet-pyutils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysnet-pyutils-1.0.1.tar", last modified: Thu Apr  6 10:53:22 2023, max compression
+gzip compressed data, was "sysnet-pyutils-1.0.2.tar", last modified: Fri May 19 13:26:14 2023, max compression
```

## Comparing `sysnet-pyutils-1.0.1.tar` & `sysnet-pyutils-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 10:53:22.880650 sysnet-pyutils-1.0.1/
--rw-rw-rw-   0        0        0    35184 2023-03-27 14:59:40.000000 sysnet-pyutils-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     5807 2023-04-06 10:53:22.879649 sysnet-pyutils-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5185 2023-04-06 10:22:58.000000 sysnet-pyutils-1.0.1/README.md
--rw-rw-rw-   0        0        0      862 2023-04-06 10:52:47.000000 sysnet-pyutils-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       47 2023-03-27 16:22:12.000000 sysnet-pyutils-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 10:53:22.880650 sysnet-pyutils-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-06 10:53:22.869652 sysnet-pyutils-1.0.1/sysnet_pyutils/
--rw-rw-rw-   0        0        0        0 2023-03-27 15:02:04.000000 sysnet-pyutils-1.0.1/sysnet_pyutils/__init__.py
--rw-rw-rw-   0        0        0     2622 2023-04-06 08:45:17.000000 sysnet-pyutils-1.0.1/sysnet_pyutils/barcode.py
--rw-rw-rw-   0        0        0     2763 2023-04-06 10:52:47.000000 sysnet-pyutils-1.0.1/sysnet_pyutils/ident.py
--rw-rw-rw-   0        0        0     8620 2023-04-06 10:52:47.000000 sysnet-pyutils-1.0.1/sysnet_pyutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:53:22.878651 sysnet-pyutils-1.0.1/sysnet_pyutils.egg-info/
--rw-rw-rw-   0        0        0     5807 2023-04-06 10:53:22.000000 sysnet-pyutils-1.0.1/sysnet_pyutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-06 10:53:22.000000 sysnet-pyutils-1.0.1/sysnet_pyutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 10:53:22.000000 sysnet-pyutils-1.0.1/sysnet_pyutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-06 10:53:22.000000 sysnet-pyutils-1.0.1/sysnet_pyutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-06 10:53:22.000000 sysnet-pyutils-1.0.1/sysnet_pyutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 13:26:14.504728 sysnet-pyutils-1.0.2/
+-rw-rw-rw-   0        0        0    35184 2023-03-27 14:59:40.000000 sysnet-pyutils-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     9052 2023-05-19 13:26:14.503729 sysnet-pyutils-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8430 2023-05-19 13:25:22.000000 sysnet-pyutils-1.0.2/README.md
+-rw-rw-rw-   0        0        0      862 2023-05-19 13:25:22.000000 sysnet-pyutils-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2023-03-27 16:22:12.000000 sysnet-pyutils-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 13:26:14.504728 sysnet-pyutils-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 13:26:14.493862 sysnet-pyutils-1.0.2/sysnet_pyutils/
+-rw-rw-rw-   0        0        0        0 2023-03-27 15:02:04.000000 sysnet-pyutils-1.0.2/sysnet_pyutils/__init__.py
+-rw-rw-rw-   0        0        0     2622 2023-04-06 08:45:17.000000 sysnet-pyutils-1.0.2/sysnet_pyutils/barcode.py
+-rw-rw-rw-   0        0        0     2763 2023-04-06 10:52:47.000000 sysnet-pyutils-1.0.2/sysnet_pyutils/ident.py
+-rw-rw-rw-   0        0        0    14941 2023-05-19 13:25:22.000000 sysnet-pyutils-1.0.2/sysnet_pyutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:26:14.502729 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/
+-rw-rw-rw-   0        0        0     9052 2023-05-19 13:26:14.000000 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-19 13:26:14.000000 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 13:26:14.000000 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-19 13:26:14.000000 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-19 13:26:14.000000 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/top_level.txt
```

### Comparing `sysnet-pyutils-1.0.1/LICENSE` & `sysnet-pyutils-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sysnet-pyutils-1.0.1/pyproject.toml` & `sysnet-pyutils-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysnet-pyutils"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Data Developer", email="info@sysnet.cz" },
 ]
 description = "Python Utilities"
 readme = "README.md"
 license = { file="LICENSE.md" }
 requires-python = ">=3.9"
```

### Comparing `sysnet-pyutils-1.0.1/sysnet_pyutils/barcode.py` & `sysnet-pyutils-1.0.2/sysnet_pyutils/barcode.py`

 * *Files identical despite different names*

### Comparing `sysnet-pyutils-1.0.1/sysnet_pyutils/ident.py` & `sysnet-pyutils-1.0.2/sysnet_pyutils/ident.py`

 * *Files identical despite different names*

