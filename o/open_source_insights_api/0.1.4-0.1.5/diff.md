# Comparing `tmp/open_source_insights_api-0.1.4.tar.gz` & `tmp/open_source_insights_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_source_insights_api-0.1.4.tar", last modified: Fri May 19 15:32:31 2023, max compression
+gzip compressed data, was "open_source_insights_api-0.1.5.tar", last modified: Fri May 19 17:45:42 2023, max compression
```

## Comparing `open_source_insights_api-0.1.4.tar` & `open_source_insights_api-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1477 2023-05-19 14:38:48.904802 open_source_insights_api-0.1.4/LICENSE
--rwxr-xr-x   0        0        0      241 2023-05-19 15:32:25.091936 open_source_insights_api-0.1.4/open_source_insights_api/__init__.py
--rwxr-xr-x   0        0        0     7882 2023-05-19 15:07:52.296446 open_source_insights_api-0.1.4/open_source_insights_api/main.py
--rwxr-xr-x   0        0        0      414 2023-05-19 15:00:27.324032 open_source_insights_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 open_source_insights_api-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1477 2023-05-19 14:38:48.904802 open_source_insights_api-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0       90 2023-05-19 17:23:05.161293 open_source_insights_api-0.1.5/open_source_insights_api/__init__.py
+-rwxr-xr-x   0        0        0     7882 2023-05-19 15:07:52.296446 open_source_insights_api-0.1.5/open_source_insights_api/os_insights.py
+-rwxr-xr-x   0        0        0      414 2023-05-19 15:00:27.324032 open_source_insights_api-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 open_source_insights_api-0.1.5/PKG-INFO
```

### Comparing `open_source_insights_api-0.1.4/LICENSE` & `open_source_insights_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `open_source_insights_api-0.1.4/open_source_insights_api/main.py` & `open_source_insights_api-0.1.5/open_source_insights_api/os_insights.py`

 * *Files identical despite different names*

