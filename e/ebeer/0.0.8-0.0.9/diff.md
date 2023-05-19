# Comparing `tmp/ebeer-0.0.8.tar.gz` & `tmp/ebeer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.8.tar", last modified: Fri May 19 18:12:15 2023, max compression
+gzip compressed data, was "ebeer-0.0.9.tar", last modified: Fri May 19 18:26:10 2023, max compression
```

## Comparing `ebeer-0.0.8.tar` & `ebeer-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:15.924611 ebeer-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 18:12:15.924611 ebeer-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 18:11:08.000000 ebeer-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 18:11:08.000000 ebeer-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:12:15.924611 ebeer-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:15.924611 ebeer-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 18:11:08.000000 ebeer-0.0.8/src/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 18:11:08.000000 ebeer-0.0.8/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:15.924611 ebeer-0.0.8/src/ebeer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 18:11:08.000000 ebeer-0.0.8/src/ebeer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-19 18:11:08.000000 ebeer-0.0.8/src/ebeer/beer_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-19 18:11:08.000000 ebeer-0.0.8/src/ebeer/label_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:15.924611 ebeer-0.0.8/src/ebeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 18:12:15.000000 ebeer-0.0.8/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-19 18:12:15.000000 ebeer-0.0.8/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:12:15.000000 ebeer-0.0.8/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 18:12:15.000000 ebeer-0.0.8/src/ebeer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:15.924611 ebeer-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 18:11:08.000000 ebeer-0.0.8/tests/test_classify.py
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

### Comparing `ebeer-0.0.8/src/ebeer/beer_classifier.py` & `ebeer-0.0.9/src/ebeer/beer_classifier.py`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.8/src/ebeer/label_index.py` & `ebeer-0.0.9/src/ebeer/label_index.py`

 * *Files identical despite different names*

