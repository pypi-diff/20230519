# Comparing `tmp/kedro-graphql-0.1.3.tar.gz` & `tmp/kedro-graphql-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-graphql-0.1.3.tar", last modified: Fri May 19 14:37:37 2023, max compression
+gzip compressed data, was "kedro-graphql-0.1.4.tar", last modified: Fri May 19 18:26:22 2023, max compression
```

## Comparing `kedro-graphql-0.1.3.tar` & `kedro-graphql-0.1.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.364412 kedro-graphql-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-19 14:37:37.364412 kedro-graphql-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 14:37:37.364412 kedro-graphql-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.352413 kedro-graphql-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.356413 kedro-graphql-0.1.3/src/kedro_graphql/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.360412 kedro-graphql-0.1.3/src/kedro_graphql/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/backends/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/celeryapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/celeryconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.360412 kedro-graphql-0.1.3/src/kedro_graphql/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/example/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/pipeline_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.360412 kedro-graphql-0.1.3/src/kedro_graphql/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.360412 kedro-graphql-0.1.3/src/kedro_graphql/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/pipelines/example00/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/pipelines/example00/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.360412 kedro-graphql-0.1.3/src/kedro_graphql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/kedro_graphql/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.360412 kedro-graphql-0.1.3/src/kedro_graphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-19 14:37:37.000000 kedro-graphql-0.1.3/src/kedro_graphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-19 14:37:37.000000 kedro-graphql-0.1.3/src/kedro_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:37:37.000000 kedro-graphql-0.1.3/src/kedro_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-19 14:37:37.000000 kedro-graphql-0.1.3/src/kedro_graphql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 14:37:37.000000 kedro-graphql-0.1.3/src/kedro_graphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 14:37:37.000000 kedro-graphql-0.1.3/src/kedro_graphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.364412 kedro-graphql-0.1.3/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.364412 kedro-graphql-0.1.3/src/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/tests/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:37.364412 kedro-graphql-0.1.3/src/tests/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/tests/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/tests/pipelines/example00/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/tests/test_schema_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/tests/test_schema_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-19 14:37:23.000000 kedro-graphql-0.1.3/src/tests/test_schema_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 18:26:22.752717 kedro-graphql-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.744717 kedro-graphql-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/backends/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/celeryapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/celeryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/example/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/pipeline_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/example00/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/example00/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/tests/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/pipelines/example00/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/test_schema_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/test_schema_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/test_schema_subscription.py
```

### Comparing `kedro-graphql-0.1.3/LICENSE.txt` & `kedro-graphql-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/PKG-INFO` & `kedro-graphql-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.1.3
+Version: 0.1.4
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kedro-graphql-0.1.3/README.md` & `kedro-graphql-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/pyproject.toml` & `kedro-graphql-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/__main__.py` & `kedro-graphql-0.1.4/src/kedro_graphql/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/asgi.py` & `kedro-graphql-0.1.4/src/kedro_graphql/asgi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from fastapi import FastAPI
 from strawberry.fastapi import GraphQLRouter
-from .config import config, backend, backend_kwargs
-from .schema import schema
-from celery.result import AsyncResult
-
-
+from .backends import init_backend
+from .schema import build_schema       
 class KedroGraphql(FastAPI):
     def __init__(self):
         super(KedroGraphql, self).__init__()
-        graphql_app = GraphQLRouter(schema)
-        self.config = config
-        self.backend = backend(**backend_kwargs)
+
+        self.backend = init_backend()
     
         @self.on_event("startup")
         def startup_backend():
             self.backend.startup()
     
         @self.on_event("shutdown")
         def shutdown_backend():
             self.backend.shutdown()
     
-    
+        graphql_app = GraphQLRouter(build_schema())
         self.include_router(graphql_app, prefix = "/graphql")
         self.add_websocket_route("/graphql", graphql_app)
+
```

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/backends/base.py` & `kedro-graphql-0.1.4/src/kedro_graphql/backends/base.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/backends/mongodb.py` & `kedro-graphql-0.1.4/src/kedro_graphql/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/commands.py` & `kedro-graphql-0.1.4/src/kedro_graphql/commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import click
 import uvicorn
-import os
-from .config import config
 from importlib import import_module
+from .config import config, discover_plugins
 
 @click.group(name="kedro-graphql")
 def commands():
     pass
 
 
 @commands.command()
 @click.pass_obj
 @click.option(
     "--app",
     "-a",
-    default=config["KEDRO_GRAPHQL_APP"],
+    default = config["KEDRO_GRAPHQL_APP"],
     help="Application import path"
 )
 @click.option(
     "--imports",
     "-i",
-    default=config["KEDRO_GRAPHQL_IMPORTS"],
+    default = config["KEDRO_GRAPHQL_IMPORTS"],
     help="Additional import paths"
 )
 @click.option(
     "--worker",
     "-w",
     is_flag=True,
     default=False,
@@ -33,16 +32,17 @@
 def gql(metadata, app, imports, worker):
     """Commands for working with kedro-graphql."""
     if worker:
         from .celeryapp import app
         worker = app.Worker()
         worker.start()
     else:
-        module, class_name = app.rsplit(".", 1)
+        config["KEDRO_GRAPHQL_IMPORTS"] = imports
+        config["KEDRO_GRAPHQL_APP"] = app
+
+        discover_plugins()
+                
+        module, class_name = config["KEDRO_GRAPHQL_APP"].rsplit(".", 1)
         module = import_module(module)
         class_inst = getattr(module, class_name)
-
-        imports = [i.strip() for i in imports.split(",") if len(i.strip()) > 0]
-        for i in imports:
-            import_module(i)
-        
+       
         uvicorn.run(class_inst(), port=5000, log_level="info")
```

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/config.py` & `kedro-graphql-0.1.4/src/kedro_graphql/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,37 +16,30 @@
 conf_parameters = context.config_loader["parameters"]
 
 ## define defaults
 config = {
     "MONGO_URI": "mongodb://root:example@localhost:27017/",
     "MONGO_DB_NAME": "pipelines",
     "KEDRO_GRAPHQL_IMPORTS": "kedro_graphql.plugins.plugins,",
-    "KEDRO_GRAPHQL_APP": "kedro_graphql.asgi.KedroGraphql"
+    "KEDRO_GRAPHQL_APP": "kedro_graphql.asgi.KedroGraphql",
+    "KEDRO_GRAPHQL_BACKEND": "kedro_graphql.backends.mongodb.MongoBackend"
     }
 
 load_config = {
     **dotenv_values(".env"),  # load 
     **os.environ,  # override loaded values with environment variables
 }
 
 ## override defaults
 config.update(load_config)
 
-## parse imports
-#config["KEDRO_GRAPHQL_IMPORTS"] = [i.strip() for i in config["KEDRO_GRAPHQL_IMPORTS"].split(",") if len(i.strip()) > 0]
-imports = [i.strip() for i in config["KEDRO_GRAPHQL_IMPORTS"].split(",") if len(i.strip()) > 0]
-
-## ".backends.mongodb.MongoBackend"
-backend_module, backend_class = "kedro_graphql.backends.mongodb.MongoBackend".rsplit(".", 1)
-backend_kwargs = {"uri": config.get("MONGO_URI"), "db": config.get("MONGO_DB_NAME")}
-backend_module = import_module(backend_module)
-backend = getattr(backend_module, backend_class)
 
 RESOLVER_PLUGINS = {}
 TYPE_PLUGINS = {"query":[],
                 "mutation":[],
                 "subscription":[]}
 
-## discover plugins e.g. decorated functions e.g @gql_resolver, @gql_query, etc...
-#for i in config["KEDRO_GRAPHQL_IMPORTS"]:
-for i in imports:
-    import_module(i)
+def discover_plugins():
+    ## discover plugins e.g. decorated functions e.g @gql_query, etc...
+    imports = [i.strip() for i in config["KEDRO_GRAPHQL_IMPORTS"].split(",") if len(i.strip()) > 0]
+    for i in imports:
+        import_module(i)
```

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/decorators.py` & `kedro-graphql-0.1.4/src/kedro_graphql/decorators.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/events.py` & `kedro-graphql-0.1.4/src/kedro_graphql/events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/example/app.py` & `kedro-graphql-0.1.4/src/kedro_graphql/example/app.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/models.py` & `kedro-graphql-0.1.4/src/kedro_graphql/models.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/plugins/plugins.py` & `kedro-graphql-0.1.4/src/kedro_graphql/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/schema.py` & `kedro-graphql-0.1.4/src/kedro_graphql/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .config import PIPELINES, RESOLVER_PLUGINS, TYPE_PLUGINS
+from .config import PIPELINES, TYPE_PLUGINS
 from .events import PipelineEventMonitor
 import strawberry
 from strawberry.tools import merge_types
 from strawberry.types import Info
 from typing import AsyncGenerator, List
 from .celeryapp import app as APP_CELERY
 from .tasks import run_pipeline
@@ -54,15 +54,15 @@
                 "inputs": serial["inputs"], 
                 "outputs": serial["outputs"], 
                 "parameters": serial["parameters"]}
         )
         
         ## PLACE HOLDER for future reolver plugins
         ## testing plugin_resolvers, 
-        RESOLVER_PLUGINS["text_in"].__input__("called text_in resolver")
+        #RESOLVER_PLUGINS["text_in"].__input__("called text_in resolver")
 
         print(f'Starting {p.name} pipeline with task_id: ' + str(p.task_id))
         p = info.context["request"].app.backend.create(p)
         print(p.id)
 
         return p
 
@@ -71,12 +71,14 @@
 class Subscription:
     @strawberry.subscription
     async def pipeline(self, id: str, info: Info) -> AsyncGenerator[PipelineEvent, None]:
         async for e in PipelineEventMonitor(app = APP_CELERY, task_id = info.context["request"].app.backend.load(id=id).task_id ).consume():
             e["id"] = id
             yield PipelineEvent(**e)
 
-ComboQuery = merge_types("Query", tuple([Query] + TYPE_PLUGINS["query"]))
-ComboMutation = merge_types("Mutation", tuple([Mutation] + TYPE_PLUGINS["mutation"]))
-ComboSubscription = merge_types("Subscription", tuple([Subscription] + TYPE_PLUGINS["subscription"]))
 
-schema = strawberry.Schema(query=ComboQuery, mutation=ComboMutation, subscription=ComboSubscription)
+def build_schema():
+    ComboQuery = merge_types("Query", tuple([Query] + TYPE_PLUGINS["query"]))
+    ComboMutation = merge_types("Mutation", tuple([Mutation] + TYPE_PLUGINS["mutation"]))
+    ComboSubscription = merge_types("Subscription", tuple([Subscription] + TYPE_PLUGINS["subscription"]))
+    
+    return strawberry.Schema(query=ComboQuery, mutation=ComboMutation, subscription=ComboSubscription)
```

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/settings.py` & `kedro-graphql-0.1.4/src/kedro_graphql/settings.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql/tasks.py` & `kedro-graphql-0.1.4/src/kedro_graphql/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from kedro.framework.project import pipelines
 from kedro.io import DataCatalog
 from kedro.runner import SequentialRunner
 from celery import shared_task, Task
-from celery.result import AsyncResult
-from .config import backend, backend_kwargs
-from .models import Pipeline
+from .backends import init_backend
 from fastapi.encoders import jsonable_encoder
 
 
 class KedroGraphqlTask(Task):
     _db = None
 
     @property
     def db(self):
         if self._db is None:
-            self._db = backend(**backend_kwargs)
+            self._db = init_backend()
         return self._db
 
     def before_start(self, task_id, args, kwargs):
         """Handler called before the task starts.
 
         .. versionadded:: 5.2
```

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql.egg-info/PKG-INFO` & `kedro-graphql-0.1.4/src/kedro_graphql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.1.3
+Version: 0.1.4
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kedro-graphql-0.1.3/src/kedro_graphql.egg-info/SOURCES.txt` & `kedro-graphql-0.1.4/src/kedro_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/setup.py` & `kedro-graphql-0.1.4/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/tests/conftest.py` & `kedro-graphql-0.1.4/src/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from pathlib import Path
 from kedro.framework.project import settings
 from kedro.config import ConfigLoader
 from kedro.framework.context import KedroContext
 from kedro.framework.hooks import _create_hook_manager
-from kedro_graphql.config import backend, backend_kwargs
+from kedro_graphql.backends import init_backend
 from kedro_graphql.tasks import run_pipeline
 from kedro_graphql.models import Pipeline, DataSet, Parameter
 from unittest.mock import patch
 
 
 
 @pytest.fixture(scope="session")
@@ -43,15 +43,15 @@
 
 @pytest.fixture(scope="session")
 def celery_worker_parameters():
     return {"without_heartbeat": False}
 
 @pytest.fixture
 def mock_backend():
-    return backend(**backend_kwargs)
+    return init_backend()
 
 @pytest.fixture
 def mock_info_context(mock_backend):
     class App():
         backend = mock_backend
 
     class Request():
```

### Comparing `kedro-graphql-0.1.3/src/tests/test_events.py` & `kedro-graphql-0.1.4/src/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/tests/test_run.py` & `kedro-graphql-0.1.4/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.3/src/tests/test_schema_mutation.py` & `kedro-graphql-0.1.4/src/tests/test_schema_mutation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 
 """
 
 
 import pytest
-from kedro_graphql.schema import schema
+from kedro_graphql.schema import build_schema
+
+schema = build_schema()
 
 @pytest.mark.usefixtures('celery_session_app')
 @pytest.mark.usefixtures('celery_session_worker')
 class TestSchemaMutations:
     @pytest.mark.asyncio
     async def test_pipeline(self, mock_info_context, mock_text_in, mock_text_out):
```

### Comparing `kedro-graphql-0.1.3/src/tests/test_schema_query.py` & `kedro-graphql-0.1.4/src/tests/test_schema_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 
 """
 
 
 import pytest
-from kedro_graphql.schema import schema
+from kedro_graphql.schema import build_schema
+
+schema = build_schema()
 
 @pytest.mark.usefixtures('celery_session_app')
 @pytest.mark.usefixtures('celery_session_worker')
 class TestSchemaQuery:
 
     @pytest.mark.asyncio
     async def test_pipeline(self, mock_info_context, mock_pipeline):
```

### Comparing `kedro-graphql-0.1.3/src/tests/test_schema_subscription.py` & `kedro-graphql-0.1.4/src/tests/test_schema_subscription.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 
 """
 import pytest
-from kedro_graphql.schema import schema
-from kedro_graphql.tasks import run_pipeline
+from kedro_graphql.schema import build_schema
 
+schema = build_schema()
 @pytest.mark.usefixtures('celery_session_app')
 @pytest.mark.usefixtures('celery_session_worker')
 class TestSchemaSubscriptions:
     @pytest.mark.asyncio
     async def test_pipeline(self, mock_info_context, mock_pipeline):
         """Requires Redis to run.
         """
```

