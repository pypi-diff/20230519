# Comparing `tmp/acrclient-0.3.0.tar.gz` & `tmp/acrclient-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrclient-0.3.0.tar", max compression
+gzip compressed data, was "acrclient-0.4.0.tar", max compression
```

## Comparing `acrclient-0.3.0.tar` & `acrclient-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2287 2023-04-29 23:12:33.634727 acrclient-0.3.0/README.md
--rw-r--r--   0        0        0      307 2023-04-29 23:12:33.634727 acrclient-0.3.0/acrclient/__init__.py
--rw-r--r--   0        0        0     4983 2023-04-29 23:12:33.634727 acrclient-0.3.0/acrclient/client.py
--rw-r--r--   0        0        0      664 2023-04-29 23:12:33.634727 acrclient-0.3.0/acrclient/models.py
--rw-r--r--   0        0        0        0 2023-04-29 23:12:33.634727 acrclient-0.3.0/acrclient/py.typed
--rw-r--r--   0        0        0     1672 2023-04-29 23:13:06.026890 acrclient-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 acrclient-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2287 2023-05-19 10:37:11.721984 acrclient-0.4.0/README.md
+-rw-r--r--   0        0        0      307 2023-05-19 10:37:11.721984 acrclient-0.4.0/acrclient/__init__.py
+-rw-r--r--   0        0        0     4983 2023-05-19 10:37:11.721984 acrclient-0.4.0/acrclient/client.py
+-rw-r--r--   0        0        0      664 2023-05-19 10:37:11.721984 acrclient-0.4.0/acrclient/models.py
+-rw-r--r--   0        0        0        0 2023-05-19 10:37:11.721984 acrclient-0.4.0/acrclient/py.typed
+-rw-r--r--   0        0        0     1672 2023-05-19 10:37:37.377805 acrclient-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 acrclient-0.4.0/PKG-INFO
```

### Comparing `acrclient-0.3.0/README.md` & `acrclient-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `acrclient-0.3.0/acrclient/client.py` & `acrclient-0.4.0/acrclient/client.py`

 * *Files identical despite different names*

### Comparing `acrclient-0.3.0/acrclient/models.py` & `acrclient-0.4.0/acrclient/models.py`

 * *Files identical despite different names*

### Comparing `acrclient-0.3.0/pyproject.toml` & `acrclient-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "acrclient"
-version = "v0.3.0"
+version = "v0.4.0"
 description = "API wrapper for the v2 ACRCloud API"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-v3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `acrclient-0.3.0/PKG-INFO` & `acrclient-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrclient
-Version: 0.3.0
+Version: 0.4.0
 Summary: API wrapper for the v2 ACRCloud API
 License: AGPL-v3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

