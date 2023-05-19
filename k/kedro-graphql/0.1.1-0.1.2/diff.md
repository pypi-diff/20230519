# Comparing `tmp/kedro-graphql-0.1.1.tar.gz` & `tmp/kedro-graphql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-graphql-0.1.1.tar", last modified: Fri May 19 13:35:19 2023, max compression
+gzip compressed data, was "kedro-graphql-0.1.2.tar", last modified: Fri May 19 13:48:00 2023, max compression
```

## Comparing `kedro-graphql-0.1.1.tar` & `kedro-graphql-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.674605 kedro-graphql-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-19 13:35:19.674605 kedro-graphql-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 13:35:19.674605 kedro-graphql-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.666605 kedro-graphql-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.670605 kedro-graphql-0.1.1/src/kedro_graphql/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.670605 kedro-graphql-0.1.1/src/kedro_graphql/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/backends/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/celeryapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/celeryconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.670605 kedro-graphql-0.1.1/src/kedro_graphql/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/example/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/pipeline_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.670605 kedro-graphql-0.1.1/src/kedro_graphql/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.670605 kedro-graphql-0.1.1/src/kedro_graphql/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/pipelines/example00/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/pipelines/example00/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.674605 kedro-graphql-0.1.1/src/kedro_graphql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/kedro_graphql/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.670605 kedro-graphql-0.1.1/src/kedro_graphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-19 13:35:19.000000 kedro-graphql-0.1.1/src/kedro_graphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-19 13:35:19.000000 kedro-graphql-0.1.1/src/kedro_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:35:19.000000 kedro-graphql-0.1.1/src/kedro_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 13:35:19.000000 kedro-graphql-0.1.1/src/kedro_graphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.674605 kedro-graphql-0.1.1/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.674605 kedro-graphql-0.1.1/src/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/tests/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:19.674605 kedro-graphql-0.1.1/src/tests/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/tests/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/tests/pipelines/example00/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/tests/test_schema_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/tests/test_schema_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-19 13:35:02.000000 kedro-graphql-0.1.1/src/tests/test_schema_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.434670 kedro-graphql-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-19 13:48:00.434670 kedro-graphql-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 13:48:00.434670 kedro-graphql-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.422670 kedro-graphql-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.426669 kedro-graphql-0.1.2/src/kedro_graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.430669 kedro-graphql-0.1.2/src/kedro_graphql/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/backends/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/celeryapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/celeryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.430669 kedro-graphql-0.1.2/src/kedro_graphql/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/example/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/pipeline_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.430669 kedro-graphql-0.1.2/src/kedro_graphql/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.430669 kedro-graphql-0.1.2/src/kedro_graphql/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/pipelines/example00/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/pipelines/example00/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.430669 kedro-graphql-0.1.2/src/kedro_graphql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/kedro_graphql/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.426669 kedro-graphql-0.1.2/src/kedro_graphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-19 13:48:00.000000 kedro-graphql-0.1.2/src/kedro_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-19 13:48:00.000000 kedro-graphql-0.1.2/src/kedro_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:48:00.000000 kedro-graphql-0.1.2/src/kedro_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 13:48:00.000000 kedro-graphql-0.1.2/src/kedro_graphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 13:48:00.000000 kedro-graphql-0.1.2/src/kedro_graphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.430669 kedro-graphql-0.1.2/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.434670 kedro-graphql-0.1.2/src/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/tests/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:48:00.434670 kedro-graphql-0.1.2/src/tests/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/tests/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/tests/pipelines/example00/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/tests/test_schema_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/tests/test_schema_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-19 13:47:46.000000 kedro-graphql-0.1.2/src/tests/test_schema_subscription.py
```

### Comparing `kedro-graphql-0.1.1/LICENSE.txt` & `kedro-graphql-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/PKG-INFO` & `kedro-graphql-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kedro-graphql-0.1.1/README.md` & `kedro-graphql-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/pyproject.toml` & `kedro-graphql-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,24 @@
     "data science",
     "data engineering",
 ]
 license = {text = "Apache Software License (Apache 2.0)"}
 classifiers = [
     "Programming Language :: Python :: 3.10",
 ]
-dynamic = ["version", "readme"]
+dynamic = ["version", "readme", "dependencies"]
 
 [project.urls]
 Homepage = "https://github.com/opensean/kedro-graphql"
 Source = "https://github.com/opensean/kedro-graphql"
 
 [tool.setuptools.dynamic]
 readme = {file = "README.md", content-type = "text/markdown"}
 version = {attr = "kedro_graphql.__version__"}
+dependencies = {file = "src/requirements.txt"}
 
 [tool.kedro]
 package_name = "kedro_graphql"
 project_name = "kedro-graphql"
 kedro_init_version = "0.18.4"
 
 [tool.isort]
```

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/__main__.py` & `kedro-graphql-0.1.2/src/kedro_graphql/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/asgi.py` & `kedro-graphql-0.1.2/src/kedro_graphql/asgi.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/backends/base.py` & `kedro-graphql-0.1.2/src/kedro_graphql/backends/base.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/backends/mongodb.py` & `kedro-graphql-0.1.2/src/kedro_graphql/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/commands.py` & `kedro-graphql-0.1.2/src/kedro_graphql/commands.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/config.py` & `kedro-graphql-0.1.2/src/kedro_graphql/config.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/decorators.py` & `kedro-graphql-0.1.2/src/kedro_graphql/decorators.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/events.py` & `kedro-graphql-0.1.2/src/kedro_graphql/events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/example/app.py` & `kedro-graphql-0.1.2/src/kedro_graphql/example/app.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/models.py` & `kedro-graphql-0.1.2/src/kedro_graphql/models.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/plugins/plugins.py` & `kedro-graphql-0.1.2/src/kedro_graphql/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/schema.py` & `kedro-graphql-0.1.2/src/kedro_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/settings.py` & `kedro-graphql-0.1.2/src/kedro_graphql/settings.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql/tasks.py` & `kedro-graphql-0.1.2/src/kedro_graphql/tasks.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql.egg-info/PKG-INFO` & `kedro-graphql-0.1.2/src/kedro_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kedro-graphql-0.1.1/src/kedro_graphql.egg-info/SOURCES.txt` & `kedro-graphql-0.1.2/src/kedro_graphql.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
+src/requirements.txt
 src/setup.py
 src/kedro_graphql/__init__.py
 src/kedro_graphql/__main__.py
 src/kedro_graphql/asgi.py
 src/kedro_graphql/celeryapp.py
 src/kedro_graphql/celeryconfig.py
 src/kedro_graphql/commands.py
@@ -16,14 +17,15 @@
 src/kedro_graphql/pipeline_registry.py
 src/kedro_graphql/schema.py
 src/kedro_graphql/settings.py
 src/kedro_graphql/tasks.py
 src/kedro_graphql.egg-info/PKG-INFO
 src/kedro_graphql.egg-info/SOURCES.txt
 src/kedro_graphql.egg-info/dependency_links.txt
+src/kedro_graphql.egg-info/requires.txt
 src/kedro_graphql.egg-info/top_level.txt
 src/kedro_graphql/backends/__init__.py
 src/kedro_graphql/backends/base.py
 src/kedro_graphql/backends/mongodb.py
 src/kedro_graphql/example/__init__.py
 src/kedro_graphql/example/app.py
 src/kedro_graphql/pipelines/__init__.py
```

### Comparing `kedro-graphql-0.1.1/src/setup.py` & `kedro-graphql-0.1.2/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/tests/conftest.py` & `kedro-graphql-0.1.2/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/tests/test_events.py` & `kedro-graphql-0.1.2/src/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/tests/test_run.py` & `kedro-graphql-0.1.2/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/tests/test_schema_mutation.py` & `kedro-graphql-0.1.2/src/tests/test_schema_mutation.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/tests/test_schema_query.py` & `kedro-graphql-0.1.2/src/tests/test_schema_query.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.1/src/tests/test_schema_subscription.py` & `kedro-graphql-0.1.2/src/tests/test_schema_subscription.py`

 * *Files identical despite different names*

