# Comparing `tmp/theopendictionary-0.3.0.tar.gz` & `tmp/theopendictionary-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theopendictionary-0.3.0.tar", max compression
+gzip compressed data, was "theopendictionary-0.4.0.tar", max compression
```

## Comparing `theopendictionary-0.3.0.tar` & `theopendictionary-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      422 2023-04-04 00:15:55.556211 theopendictionary-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       29 2023-04-04 00:15:55.556211 theopendictionary-0.3.0/theopendictionary/__init__.py
--rw-r--r--   0        0        0     1650 2023-04-04 00:15:55.556211 theopendictionary-0.3.0/theopendictionary/odict.py
--rw-r--r--   0        0        0     2405 2023-04-04 00:15:55.556211 theopendictionary-0.3.0/theopendictionary/test_odict.py
--rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 theopendictionary-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      422 2023-05-19 21:33:52.150491 theopendictionary-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-01-07 22:51:39.553380 theopendictionary-0.4.0/theopendictionary/__init__.py
+-rw-r--r--   0        0        0     1442 2023-04-04 07:15:34.237886 theopendictionary-0.4.0/theopendictionary/odict.py
+-rw-r--r--   0        0        0     2405 2023-04-04 07:15:21.644772 theopendictionary-0.4.0/theopendictionary/test_odict.py
+-rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 theopendictionary-0.4.0/PKG-INFO
```

### Comparing `theopendictionary-0.3.0/theopendictionary/odict.py` & `theopendictionary-0.4.0/theopendictionary/odict.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,14 @@
 from os import environ, remove
 from subprocess import run
 from tempfile import NamedTemporaryFile
 from typing import List
 
 
 def exec(*args: List[str]):
-    print(
-        " ".join(
-            [
-                "../bin/odict" if environ.get("RUNTIME_ENV") == "test" else "odict",
-                "--quiet",
-                *args,
-            ]
-        )
-    )
     out = run(
         [
             "../bin/odict" if environ.get("RUNTIME_ENV") == "test" else "odict",
             "--quiet",
             *args,
         ],
         capture_output=True,
```

### Comparing `theopendictionary-0.3.0/theopendictionary/test_odict.py` & `theopendictionary-0.4.0/theopendictionary/test_odict.py`

 * *Files identical despite different names*

