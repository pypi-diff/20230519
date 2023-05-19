# Comparing `tmp/cukcuk-0.5.1.tar.gz` & `tmp/cukcuk-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cukcuk-0.5.1.tar", last modified: Fri May 19 02:00:39 2023, max compression
+gzip compressed data, was "cukcuk-0.5.2.tar", last modified: Fri May 19 02:02:56 2023, max compression
```

## Comparing `cukcuk-0.5.1.tar` & `cukcuk-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:00:39.956358 cukcuk-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-19 02:00:39.956358 cukcuk-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 02:00:29.000000 cukcuk-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:00:39.956358 cukcuk-0.5.1/cukcuk/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-19 02:00:29.000000 cukcuk-0.5.1/cukcuk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-19 02:00:29.000000 cukcuk-0.5.1/cukcuk/async_login_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-19 02:00:29.000000 cukcuk-0.5.1/cukcuk/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-19 02:00:29.000000 cukcuk-0.5.1/cukcuk/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-05-19 02:00:29.000000 cukcuk-0.5.1/cukcuk/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-05-19 02:00:29.000000 cukcuk-0.5.1/cukcuk/login_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-19 02:00:29.000000 cukcuk-0.5.1/cukcuk/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:00:39.956358 cukcuk-0.5.1/cukcuk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-19 02:00:39.000000 cukcuk-0.5.1/cukcuk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-19 02:00:39.000000 cukcuk-0.5.1/cukcuk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:00:39.000000 cukcuk-0.5.1/cukcuk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 02:00:39.000000 cukcuk-0.5.1/cukcuk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 02:00:39.000000 cukcuk-0.5.1/cukcuk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-19 02:00:29.000000 cukcuk-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-19 02:00:39.956358 cukcuk-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:02:56.398866 cukcuk-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-19 02:02:56.398866 cukcuk-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 02:02:46.000000 cukcuk-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:02:56.394866 cukcuk-0.5.2/cukcuk/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-19 02:02:46.000000 cukcuk-0.5.2/cukcuk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-19 02:02:46.000000 cukcuk-0.5.2/cukcuk/async_login_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-19 02:02:46.000000 cukcuk-0.5.2/cukcuk/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-19 02:02:46.000000 cukcuk-0.5.2/cukcuk/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-05-19 02:02:46.000000 cukcuk-0.5.2/cukcuk/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-05-19 02:02:46.000000 cukcuk-0.5.2/cukcuk/login_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-19 02:02:46.000000 cukcuk-0.5.2/cukcuk/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:02:56.394866 cukcuk-0.5.2/cukcuk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-19 02:02:56.000000 cukcuk-0.5.2/cukcuk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-19 02:02:56.000000 cukcuk-0.5.2/cukcuk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:02:56.000000 cukcuk-0.5.2/cukcuk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 02:02:56.000000 cukcuk-0.5.2/cukcuk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 02:02:56.000000 cukcuk-0.5.2/cukcuk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-19 02:02:46.000000 cukcuk-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-19 02:02:56.398866 cukcuk-0.5.2/setup.cfg
```

### Comparing `cukcuk-0.5.1/cukcuk/async_login_session.py` & `cukcuk-0.5.2/cukcuk/async_login_session.py`

 * *Files identical despite different names*

### Comparing `cukcuk-0.5.1/cukcuk/branch.py` & `cukcuk-0.5.2/cukcuk/branch.py`

 * *Files identical despite different names*

### Comparing `cukcuk-0.5.1/cukcuk/common.py` & `cukcuk-0.5.2/cukcuk/common.py`

 * *Files identical despite different names*

### Comparing `cukcuk-0.5.1/cukcuk/invoice.py` & `cukcuk-0.5.2/cukcuk/invoice.py`

 * *Files identical despite different names*

### Comparing `cukcuk-0.5.1/cukcuk/login_session.py` & `cukcuk-0.5.2/cukcuk/login_session.py`

 * *Files identical despite different names*

### Comparing `cukcuk-0.5.1/cukcuk/storage.py` & `cukcuk-0.5.2/cukcuk/storage.py`

 * *Files identical despite different names*

