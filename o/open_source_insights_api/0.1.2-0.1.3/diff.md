# Comparing `tmp/open_source_insights_api-0.1.2.tar.gz` & `tmp/open_source_insights_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_source_insights_api-0.1.2.tar", last modified: Fri May 19 15:22:50 2023, max compression
+gzip compressed data, was "open_source_insights_api-0.1.3.tar", last modified: Fri May 19 15:30:14 2023, max compression
```

## Comparing `open_source_insights_api-0.1.2.tar` & `open_source_insights_api-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1477 2023-05-19 14:38:48.904802 open_source_insights_api-0.1.2/LICENSE
--rwxr-xr-x   0        0        0       90 2023-05-19 15:22:30.733721 open_source_insights_api-0.1.2/open_source_insights_api/__init__.py
--rwxr-xr-x   0        0        0     7882 2023-05-19 15:07:52.296446 open_source_insights_api-0.1.2/open_source_insights_api/open_source_insights_api.py
--rwxr-xr-x   0        0        0      414 2023-05-19 15:00:27.324032 open_source_insights_api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 open_source_insights_api-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1477 2023-05-19 14:38:48.904802 open_source_insights_api-0.1.3/LICENSE
+-rwxr-xr-x   0        0        0      261 2023-05-19 15:30:08.218347 open_source_insights_api-0.1.3/open_source_insights_api/__init__.py
+-rwxr-xr-x   0        0        0     7882 2023-05-19 15:07:52.296446 open_source_insights_api-0.1.3/open_source_insights_api/open_source_insights_api.py
+-rwxr-xr-x   0        0        0      414 2023-05-19 15:00:27.324032 open_source_insights_api-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 open_source_insights_api-0.1.3/PKG-INFO
```

### Comparing `open_source_insights_api-0.1.2/LICENSE` & `open_source_insights_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_source_insights_api-0.1.2/open_source_insights_api/open_source_insights_api.py` & `open_source_insights_api-0.1.3/open_source_insights_api/open_source_insights_api.py`

 * *Files identical despite different names*

