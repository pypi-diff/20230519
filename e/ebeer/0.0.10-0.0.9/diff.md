# Comparing `tmp/ebeer-0.0.10.tar.gz` & `tmp/ebeer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.10.tar", last modified: Fri May 19 18:49:13 2023, max compression
+gzip compressed data, was "ebeer-0.0.9.tar", last modified: Fri May 19 18:26:10 2023, max compression
```

## Comparing `ebeer-0.0.10.tar` & `ebeer-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:49:13.181093 ebeer-0.0.10/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-19 18:49:13.181093 ebeer-0.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 18:48:05.000000 ebeer-0.0.10/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-19 18:48:05.000000 ebeer-0.0.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:49:13.181093 ebeer-0.0.10/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:49:13.181093 ebeer-0.0.10/src/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 18:48:05.000000 ebeer-0.0.10/src/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 18:48:05.000000 ebeer-0.0.10/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:49:13.181093 ebeer-0.0.10/src/ebeer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 18:48:05.000000 ebeer-0.0.10/src/ebeer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-19 18:48:05.000000 ebeer-0.0.10/src/ebeer/beer_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-19 18:48:05.000000 ebeer-0.0.10/src/ebeer/label_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:49:13.181093 ebeer-0.0.10/src/ebeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-19 18:49:13.000000 ebeer-0.0.10/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-19 18:49:13.000000 ebeer-0.0.10/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:49:13.000000 ebeer-0.0.10/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 18:49:13.000000 ebeer-0.0.10/src/ebeer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 18:48:05.000000 ebeer-0.0.10/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:49:13.181093 ebeer-0.0.10/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 18:48:05.000000 ebeer-0.0.10/tests/test_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:10.477319 ebeer-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 18:26:10.477319 ebeer-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 18:25:05.000000 ebeer-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 18:25:05.000000 ebeer-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:26:10.477319 ebeer-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:10.477319 ebeer-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:10.477319 ebeer-0.0.9/src/ebeer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/ebeer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/ebeer/beer_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/ebeer/label_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:10.477319 ebeer-0.0.9/src/ebeer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 18:26:10.000000 ebeer-0.0.9/src/ebeer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-19 18:26:10.000000 ebeer-0.0.9/src/ebeer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:26:10.000000 ebeer-0.0.9/src/ebeer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 18:26:10.000000 ebeer-0.0.9/src/ebeer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-19 18:25:05.000000 ebeer-0.0.9/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:10.477319 ebeer-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 18:25:05.000000 ebeer-0.0.9/tests/test_classify.py
```

### Comparing `ebeer-0.0.10/src/ebeer/beer_classifier.py` & `ebeer-0.0.9/src/ebeer/beer_classifier.py`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.10/src/ebeer/label_index.py` & `ebeer-0.0.9/src/ebeer/label_index.py`

 * *Files identical despite different names*

