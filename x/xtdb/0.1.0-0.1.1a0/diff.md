# Comparing `tmp/xtdb-0.1.0.tar.gz` & `tmp/xtdb-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtdb-0.1.0.tar", max compression
+gzip compressed data, was "xtdb-0.1.1a0.tar", max compression
```

## Comparing `xtdb-0.1.0.tar` & `xtdb-0.1.1a0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    13827 2023-05-10 11:34:24.361633 xtdb-0.1.0/LICENSE
--rw-r--r--   0        0        0     2708 2023-05-19 15:35:12.005966 xtdb-0.1.0/README.md
--rw-r--r--   0        0        0     1581 2023-05-19 15:58:30.585759 xtdb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 11:34:24.361633 xtdb-0.1.0/xtdb/__init__.py
--rw-r--r--   0        0        0      240 2023-05-19 13:44:52.308746 xtdb-0.1.0/xtdb/__main__.py
--rw-r--r--   0        0        0      165 2023-05-17 09:07:20.271074 xtdb-0.1.0/xtdb/exceptions.py
--rw-r--r--   0        0        0     1857 2023-05-19 14:48:05.011172 xtdb-0.1.0/xtdb/orm.py
--rw-r--r--   0        0        0     5620 2023-05-19 13:19:02.480756 xtdb-0.1.0/xtdb/query.py
--rw-r--r--   0        0        0     7140 2023-05-19 15:05:45.979690 xtdb-0.1.0/xtdb/session.py
--rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 xtdb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13827 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/LICENSE
+-rw-r--r--   0        0        0     2708 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/README.md
+-rw-r--r--   0        0        0     1582 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/__init__.py
+-rw-r--r--   0        0        0      240 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/__main__.py
+-rw-r--r--   0        0        0      165 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/exceptions.py
+-rw-r--r--   0        0        0     1857 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/orm.py
+-rw-r--r--   0        0        0     5620 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/query.py
+-rw-r--r--   0        0        0     7140 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/session.py
+-rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 xtdb-0.1.1a0/PKG-INFO
```

### Comparing `xtdb-0.1.0/LICENSE` & `xtdb-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `xtdb-0.1.0/README.md` & `xtdb-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `xtdb-0.1.0/pyproject.toml` & `xtdb-0.1.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtdb"
-version = "0.1.0"
+version = "0.1.1a"
 packages = [{ include = "xtdb" }]
 include  = ["xtdb/**"]
 exclude = [
     "**/.idea",
     "**/.git*",
     "**/.*ignore",
     "**/.flake8",
```

### Comparing `xtdb-0.1.0/xtdb/orm.py` & `xtdb-0.1.1a0/xtdb/orm.py`

 * *Files identical despite different names*

### Comparing `xtdb-0.1.0/xtdb/query.py` & `xtdb-0.1.1a0/xtdb/query.py`

 * *Files identical despite different names*

### Comparing `xtdb-0.1.0/xtdb/session.py` & `xtdb-0.1.1a0/xtdb/session.py`

 * *Files identical despite different names*

### Comparing `xtdb-0.1.0/PKG-INFO` & `xtdb-0.1.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtdb
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: A Python connector and ORM for XTDB.
 Home-page: https://github.com/Donnype/xtdb-py
 Author: Donny Peeters
 Author-email: donny.peeters@hotmail.com
 Maintainer: Donny Peeters
 Maintainer-email: donny.peeters@hotmail.com
 Requires-Python: >=3.8,<4.0
```

