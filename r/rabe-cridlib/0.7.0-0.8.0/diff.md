# Comparing `tmp/rabe_cridlib-0.7.0.tar.gz` & `tmp/rabe_cridlib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabe_cridlib-0.7.0.tar", max compression
+gzip compressed data, was "rabe_cridlib-0.8.0.tar", max compression
```

## Comparing `rabe_cridlib-0.7.0.tar` & `rabe_cridlib-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34520 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/LICENSE
--rw-r--r--   0        0        0     2844 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/README.md
--rw-r--r--   0        0        0      343 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/get.py
--rw-r--r--   0        0        0     4586 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/lib.py
--rw-r--r--   0        0        0      221 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/parse.py
--rw-r--r--   0        0        0        0 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/py.typed
--rw-r--r--   0        0        0      192 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/strategy/__init__.py
--rw-r--r--   0        0        0     1305 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/strategy/future.py
--rw-r--r--   0        0        0      624 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/strategy/now.py
--rw-r--r--   0        0        0      772 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/strategy/past.py
--rw-r--r--   0        0        0     1051 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/util.py
--rw-r--r--   0        0        0     1544 2023-04-29 08:12:02.445325 rabe_cridlib-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 rabe_cridlib-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2844 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/README.md
+-rw-r--r--   0        0        0      343 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/__init__.py
+-rw-r--r--   0        0        0     1419 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/get.py
+-rw-r--r--   0        0        0     4586 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/lib.py
+-rw-r--r--   0        0        0      221 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/parse.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/py.typed
+-rw-r--r--   0        0        0      192 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/strategy/__init__.py
+-rw-r--r--   0        0        0     1305 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/strategy/future.py
+-rw-r--r--   0        0        0      624 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/strategy/now.py
+-rw-r--r--   0        0        0      772 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/strategy/past.py
+-rw-r--r--   0        0        0     1051 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/util.py
+-rw-r--r--   0        0        0     1544 2023-05-19 00:58:41.595635 rabe_cridlib-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 rabe_cridlib-0.8.0/PKG-INFO
```

### Comparing `rabe_cridlib-0.7.0/LICENSE` & `rabe_cridlib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.7.0/README.md` & `rabe_cridlib-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.7.0/cridlib/get.py` & `rabe_cridlib-0.8.0/cridlib/get.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.7.0/cridlib/lib.py` & `rabe_cridlib-0.8.0/cridlib/lib.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.7.0/cridlib/strategy/future.py` & `rabe_cridlib-0.8.0/cridlib/strategy/future.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.7.0/cridlib/strategy/now.py` & `rabe_cridlib-0.8.0/cridlib/strategy/now.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.7.0/cridlib/strategy/past.py` & `rabe_cridlib-0.8.0/cridlib/strategy/past.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.7.0/cridlib/util.py` & `rabe_cridlib-0.8.0/cridlib/util.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.7.0/pyproject.toml` & `rabe_cridlib-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rabe-cridlib"
-version = "v0.7.0" # 0.0.0 placeholder is replaced on release
+version = "v0.8.0" # 0.0.0 placeholder is replaced on release
 description = "Generate CRIDs for RaBe"
 repository = "https://github.com/radiorabe/python-rabe-cridlib"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `rabe_cridlib-0.7.0/PKG-INFO` & `rabe_cridlib-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabe-cridlib
-Version: 0.7.0
+Version: 0.8.0
 Summary: Generate CRIDs for RaBe
 Home-page: https://github.com/radiorabe/python-rabe-cridlib
 License: AGPL-3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

