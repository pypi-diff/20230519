# Comparing `tmp/ebeer-0.0.5.tar.gz` & `tmp/ebeer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.5.tar", last modified: Thu May 18 22:01:50 2023, max compression
+gzip compressed data, was "ebeer-0.0.6.tar", last modified: Fri May 19 00:37:42 2023, max compression
```

## Comparing `ebeer-0.0.5.tar` & `ebeer-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:01:50.282068 ebeer-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-18 22:01:50.282068 ebeer-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-18 22:00:33.000000 ebeer-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-18 22:00:33.000000 ebeer-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:01:50.282068 ebeer-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:01:50.282068 ebeer-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 22:00:33.000000 ebeer-0.0.5/src/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 22:00:33.000000 ebeer-0.0.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:01:50.282068 ebeer-0.0.5/src/ebeer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 22:00:33.000000 ebeer-0.0.5/src/ebeer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-18 22:00:33.000000 ebeer-0.0.5/src/ebeer/beer_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-18 22:00:33.000000 ebeer-0.0.5/src/ebeer/label_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:01:50.282068 ebeer-0.0.5/src/ebeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-18 22:01:50.000000 ebeer-0.0.5/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-18 22:01:50.000000 ebeer-0.0.5/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:01:50.000000 ebeer-0.0.5/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 22:01:50.000000 ebeer-0.0.5/src/ebeer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:01:50.282068 ebeer-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-18 22:00:33.000000 ebeer-0.0.5/tests/test_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:37:42.803117 ebeer-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 00:37:42.803117 ebeer-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 00:36:33.000000 ebeer-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 00:36:33.000000 ebeer-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:37:42.803117 ebeer-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:37:42.803117 ebeer-0.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 00:36:33.000000 ebeer-0.0.6/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 00:36:33.000000 ebeer-0.0.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:37:42.803117 ebeer-0.0.6/src/ebeer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 00:36:33.000000 ebeer-0.0.6/src/ebeer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-19 00:36:33.000000 ebeer-0.0.6/src/ebeer/beer_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-19 00:36:33.000000 ebeer-0.0.6/src/ebeer/label_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:37:42.803117 ebeer-0.0.6/src/ebeer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 00:37:42.000000 ebeer-0.0.6/src/ebeer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-19 00:37:42.000000 ebeer-0.0.6/src/ebeer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:37:42.000000 ebeer-0.0.6/src/ebeer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 00:37:42.000000 ebeer-0.0.6/src/ebeer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:37:42.803117 ebeer-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 00:36:33.000000 ebeer-0.0.6/tests/test_classify.py
```

### Comparing `ebeer-0.0.5/src/ebeer/beer_classifier.py` & `ebeer-0.0.6/src/ebeer/beer_classifier.py`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.5/src/ebeer/label_index.py` & `ebeer-0.0.6/src/ebeer/label_index.py`

 * *Files identical despite different names*

