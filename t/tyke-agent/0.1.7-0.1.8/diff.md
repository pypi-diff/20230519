# Comparing `tmp/tyke-agent-0.1.7.tar.gz` & `tmp/tyke-agent-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyke-agent-0.1.7.tar", last modified: Tue May 16 04:36:37 2023, max compression
+gzip compressed data, was "tyke-agent-0.1.8.tar", last modified: Fri May 19 03:46:45 2023, max compression
```

## Comparing `tyke-agent-0.1.7.tar` & `tyke-agent-0.1.8.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.714450 tyke-agent-0.1.7/
--rw-rw-r--   0 bhaskar    (501) staff       (20)    11348 2023-05-11 10:33:50.000000 tyke-agent-0.1.7/LICENSE
--rw-r--r--   0 bhaskar    (501) staff       (20)     2975 2023-05-16 04:36:37.714275 tyke-agent-0.1.7/PKG-INFO
--rw-rw-r--   0 bhaskar    (501) staff       (20)     2501 2023-05-16 04:33:41.000000 tyke-agent-0.1.7/README.md
--rw-rw-r--   0 bhaskar    (501) staff       (20)      106 2022-08-25 14:02:53.000000 tyke-agent-0.1.7/pyproject.toml
--rw-r--r--   0 bhaskar    (501) staff       (20)       38 2023-05-16 04:36:37.714488 tyke-agent-0.1.7/setup.cfg
--rw-rw-r--   0 bhaskar    (501) staff       (20)     3251 2023-05-11 14:13:14.000000 tyke-agent-0.1.7/setup.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.696226 tyke-agent-0.1.7/src/
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.698463 tyke-agent-0.1.7/src/tyke/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      354 2022-10-22 15:56:27.000000 tyke-agent-0.1.7/src/tyke/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.699494 tyke-agent-0.1.7/src/tyke/agent/
--rw-rw-r--   0 bhaskar    (501) staff       (20)    13249 2023-05-16 03:46:27.000000 tyke-agent-0.1.7/src/tyke/agent/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.700209 tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/
--rw-rw-r--   0 bhaskar    (501) staff       (20)        0 2022-08-25 14:02:53.000000 tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)      625 2022-10-22 16:49:39.000000 tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/sitecustomize.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     2125 2022-10-22 15:55:10.000000 tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/tyke_instrument.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.701517 tyke-agent-0.1.7/src/tyke/agent/config/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     7552 2022-10-25 03:02:38.000000 tyke-agent-0.1.7/src/tyke/agent/config/__init__.py
--rw-r--r--   0 bhaskar    (501) staff       (20)     4658 2022-11-30 14:36:51.000000 tyke-agent-0.1.7/src/tyke/agent/config/config_pb2.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)      847 2022-08-25 14:02:53.000000 tyke-agent-0.1.7/src/tyke/agent/config/default.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     5838 2022-10-22 15:56:27.000000 tyke-agent-0.1.7/src/tyke/agent/config/environment.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)      913 2022-10-25 03:02:41.000000 tyke-agent-0.1.7/src/tyke/agent/config/file.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)      462 2022-10-25 02:36:21.000000 tyke-agent-0.1.7/src/tyke/agent/constants.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     1240 2022-10-22 15:56:27.000000 tyke-agent-0.1.7/src/tyke/agent/custom_logger.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.701903 tyke-agent-0.1.7/src/tyke/agent/filter/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      951 2022-08-25 14:02:53.000000 tyke-agent-0.1.7/src/tyke/agent/filter/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     1353 2022-10-22 15:56:27.000000 tyke-agent-0.1.7/src/tyke/agent/filter/registry.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.702065 tyke-agent-0.1.7/src/tyke/agent/init/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     8927 2022-10-22 15:56:25.000000 tyke-agent-0.1.7/src/tyke/agent/init/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.702826 tyke-agent-0.1.7/src/tyke/agent/instrumentation/
--rw-rw-r--   0 bhaskar    (501) staff       (20)    13041 2022-12-09 09:41:41.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.703131 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aiohttp/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     7670 2022-10-25 02:36:48.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aiohttp/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.704006 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aiopg/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      457 2023-05-11 12:39:26.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aiopg/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.704374 tyke-agent-0.1.7/src/tyke/agent/instrumentation/asyncpg/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      589 2023-05-11 12:00:36.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/asyncpg/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.704675 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aws_lambda/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     9227 2022-10-22 16:49:39.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aws_lambda/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.704985 tyke-agent-0.1.7/src/tyke/agent/instrumentation/boto/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      488 2022-10-22 16:49:39.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/boto/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.705325 tyke-agent-0.1.7/src/tyke/agent/instrumentation/botocore/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      511 2022-10-22 16:49:39.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/botocore/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.705542 tyke-agent-0.1.7/src/tyke/agent/instrumentation/celery/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      441 2023-05-11 12:39:40.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/celery/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.705858 tyke-agent-0.1.7/src/tyke/agent/instrumentation/confluent_kafka/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      513 2023-05-11 12:40:05.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/confluent_kafka/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.706874 tyke-agent-0.1.7/src/tyke/agent/instrumentation/django/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     3201 2022-10-31 06:05:42.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/django/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     3455 2022-10-26 19:28:45.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/django/django_auto_instrumentation_compat.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.707178 tyke-agent-0.1.7/src/tyke/agent/instrumentation/elasticsearch/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      508 2023-05-11 12:40:23.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/elasticsearch/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.707997 tyke-agent-0.1.7/src/tyke/agent/instrumentation/fast_api/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     8052 2022-10-25 02:36:53.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/fast_api/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     2816 2022-10-22 15:56:26.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/fast_api/fast_api_auto_instrumentation_compat.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.708286 tyke-agent-0.1.7/src/tyke/agent/instrumentation/flask/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     7903 2022-10-25 02:37:00.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/flask/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.708518 tyke-agent-0.1.7/src/tyke/agent/instrumentation/grpc/
--rw-rw-r--   0 bhaskar    (501) staff       (20)    11626 2022-10-25 02:37:01.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/grpc/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.708701 tyke-agent-0.1.7/src/tyke/agent/instrumentation/httpx/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      448 2023-05-11 12:38:34.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/httpx/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     7625 2023-05-16 03:44:42.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/instrumentation_definitions.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.709012 tyke-agent-0.1.7/src/tyke/agent/instrumentation/kafka_python/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      456 2023-05-11 12:40:49.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/kafka_python/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.709275 tyke-agent-0.1.7/src/tyke/agent/instrumentation/method/
--rw-r--r--   0 bhaskar    (501) staff       (20)     1635 2023-05-11 16:45:11.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/method/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.709528 tyke-agent-0.1.7/src/tyke/agent/instrumentation/mysql/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      436 2023-05-11 12:38:55.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/mysql/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.709806 tyke-agent-0.1.7/src/tyke/agent/instrumentation/postgresql/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      565 2023-05-11 12:41:38.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/postgresql/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.710090 tyke-agent-0.1.7/src/tyke/agent/instrumentation/postgresql_binary/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      726 2023-05-15 18:31:15.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/postgresql_binary/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.710345 tyke-agent-0.1.7/src/tyke/agent/instrumentation/pymongo/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      448 2023-05-11 12:41:17.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/pymongo/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.710640 tyke-agent-0.1.7/src/tyke/agent/instrumentation/pymysql/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      447 2023-05-11 12:38:46.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/pymysql/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.710881 tyke-agent-0.1.7/src/tyke/agent/instrumentation/redis/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      435 2023-05-11 12:38:39.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/redis/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.711191 tyke-agent-0.1.7/src/tyke/agent/instrumentation/remoulade/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      459 2023-05-11 12:45:19.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/remoulade/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.711508 tyke-agent-0.1.7/src/tyke/agent/instrumentation/requests/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     3238 2023-01-05 13:32:00.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/requests/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.711780 tyke-agent-0.1.7/src/tyke/agent/instrumentation/sklearn/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      447 2023-05-11 12:46:52.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/sklearn/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.712087 tyke-agent-0.1.7/src/tyke/agent/instrumentation/sqlalchemy/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      465 2023-05-11 12:48:09.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/sqlalchemy/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.712386 tyke-agent-0.1.7/src/tyke/agent/instrumentation/urllib/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      441 2023-05-11 14:12:39.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/urllib/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.713013 tyke-agent-0.1.7/src/tyke/agent/instrumentation/urllib3/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      447 2023-05-11 14:11:23.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/urllib3/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)      502 2022-10-25 04:51:53.000000 tyke-agent-0.1.7/src/tyke/env_var_settings.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)       92 2023-05-11 15:06:08.000000 tyke-agent-0.1.7/src/tyke/version.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.714082 tyke-agent-0.1.7/src/tyke_agent.egg-info/
--rw-r--r--   0 bhaskar    (501) staff       (20)     2975 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/PKG-INFO
--rw-r--r--   0 bhaskar    (501) staff       (20)     2563 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/SOURCES.txt
--rw-r--r--   0 bhaskar    (501) staff       (20)        1 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/dependency_links.txt
--rw-r--r--   0 bhaskar    (501) staff       (20)       87 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/entry_points.txt
--rw-r--r--   0 bhaskar    (501) staff       (20)     1589 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/requires.txt
--rw-r--r--   0 bhaskar    (501) staff       (20)        5 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/top_level.txt
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.998734 tyke-agent-0.1.8/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)    11348 2023-05-11 10:33:50.000000 tyke-agent-0.1.8/LICENSE
+-rw-r--r--   0 bhaskar    (501) staff       (20)     3238 2023-05-19 03:46:45.998553 tyke-agent-0.1.8/PKG-INFO
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     2764 2023-05-18 04:12:47.000000 tyke-agent-0.1.8/README.md
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      106 2022-08-25 14:02:53.000000 tyke-agent-0.1.8/pyproject.toml
+-rw-r--r--   0 bhaskar    (501) staff       (20)       38 2023-05-19 03:46:45.998773 tyke-agent-0.1.8/setup.cfg
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     3251 2023-05-11 14:13:14.000000 tyke-agent-0.1.8/setup.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.989259 tyke-agent-0.1.8/src/
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.990290 tyke-agent-0.1.8/src/tyke/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      354 2022-10-22 15:56:27.000000 tyke-agent-0.1.8/src/tyke/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.990676 tyke-agent-0.1.8/src/tyke/agent/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)    13249 2023-05-16 03:46:27.000000 tyke-agent-0.1.8/src/tyke/agent/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.991039 tyke-agent-0.1.8/src/tyke/agent/autoinstrumentation/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)        0 2022-08-25 14:02:53.000000 tyke-agent-0.1.8/src/tyke/agent/autoinstrumentation/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      625 2022-10-22 16:49:39.000000 tyke-agent-0.1.8/src/tyke/agent/autoinstrumentation/sitecustomize.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     2125 2022-10-22 15:55:10.000000 tyke-agent-0.1.8/src/tyke/agent/autoinstrumentation/tyke_instrument.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.991722 tyke-agent-0.1.8/src/tyke/agent/config/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     7552 2022-10-25 03:02:38.000000 tyke-agent-0.1.8/src/tyke/agent/config/__init__.py
+-rw-r--r--   0 bhaskar    (501) staff       (20)     4658 2022-11-30 14:36:51.000000 tyke-agent-0.1.8/src/tyke/agent/config/config_pb2.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      847 2022-08-25 14:02:53.000000 tyke-agent-0.1.8/src/tyke/agent/config/default.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     5838 2022-10-22 15:56:27.000000 tyke-agent-0.1.8/src/tyke/agent/config/environment.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      913 2022-10-25 03:02:41.000000 tyke-agent-0.1.8/src/tyke/agent/config/file.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      462 2022-10-25 02:36:21.000000 tyke-agent-0.1.8/src/tyke/agent/constants.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     1240 2022-10-22 15:56:27.000000 tyke-agent-0.1.8/src/tyke/agent/custom_logger.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.991990 tyke-agent-0.1.8/src/tyke/agent/filter/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      951 2022-08-25 14:02:53.000000 tyke-agent-0.1.8/src/tyke/agent/filter/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     1353 2022-10-22 15:56:27.000000 tyke-agent-0.1.8/src/tyke/agent/filter/registry.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.992123 tyke-agent-0.1.8/src/tyke/agent/init/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     8927 2022-10-22 15:56:25.000000 tyke-agent-0.1.8/src/tyke/agent/init/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.992406 tyke-agent-0.1.8/src/tyke/agent/instrumentation/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)    13106 2023-05-18 05:03:21.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.992552 tyke-agent-0.1.8/src/tyke/agent/instrumentation/aiohttp/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     7670 2022-10-25 02:36:48.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/aiohttp/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.992683 tyke-agent-0.1.8/src/tyke/agent/instrumentation/aiopg/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      457 2023-05-11 12:39:26.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/aiopg/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.992818 tyke-agent-0.1.8/src/tyke/agent/instrumentation/asyncpg/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      589 2023-05-11 12:00:36.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/asyncpg/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.992965 tyke-agent-0.1.8/src/tyke/agent/instrumentation/aws_lambda/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     9227 2022-10-22 16:49:39.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/aws_lambda/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.993092 tyke-agent-0.1.8/src/tyke/agent/instrumentation/boto/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      488 2022-10-22 16:49:39.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/boto/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.993216 tyke-agent-0.1.8/src/tyke/agent/instrumentation/botocore/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      511 2022-10-22 16:49:39.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/botocore/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.993684 tyke-agent-0.1.8/src/tyke/agent/instrumentation/celery/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      441 2023-05-11 12:39:40.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/celery/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.993957 tyke-agent-0.1.8/src/tyke/agent/instrumentation/confluent_kafka/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      513 2023-05-11 12:40:05.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/confluent_kafka/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.994312 tyke-agent-0.1.8/src/tyke/agent/instrumentation/django/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     3201 2023-05-19 03:46:09.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/django/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     3455 2022-10-26 19:28:45.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/django/django_auto_instrumentation_compat.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.994462 tyke-agent-0.1.8/src/tyke/agent/instrumentation/elasticsearch/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      508 2023-05-11 12:40:23.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/elasticsearch/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.994779 tyke-agent-0.1.8/src/tyke/agent/instrumentation/fast_api/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     8052 2022-10-25 02:36:53.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/fast_api/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     2816 2022-10-22 15:56:26.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/fast_api/fast_api_auto_instrumentation_compat.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.994931 tyke-agent-0.1.8/src/tyke/agent/instrumentation/flask/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     7903 2022-10-25 02:37:00.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/flask/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.995057 tyke-agent-0.1.8/src/tyke/agent/instrumentation/grpc/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)    11626 2022-10-25 02:37:01.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/grpc/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.995180 tyke-agent-0.1.8/src/tyke/agent/instrumentation/httpx/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      448 2023-05-11 12:38:34.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/httpx/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     7625 2023-05-16 03:44:42.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/instrumentation_definitions.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.995292 tyke-agent-0.1.8/src/tyke/agent/instrumentation/kafka_python/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      456 2023-05-11 12:40:49.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/kafka_python/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.995424 tyke-agent-0.1.8/src/tyke/agent/instrumentation/method/
+-rw-r--r--   0 bhaskar    (501) staff       (20)     1635 2023-05-11 16:45:11.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/method/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.995556 tyke-agent-0.1.8/src/tyke/agent/instrumentation/mysql/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      436 2023-05-11 12:38:55.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/mysql/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.995688 tyke-agent-0.1.8/src/tyke/agent/instrumentation/postgresql/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      565 2023-05-11 12:41:38.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/postgresql/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.995841 tyke-agent-0.1.8/src/tyke/agent/instrumentation/postgresql_binary/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      726 2023-05-15 18:31:15.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/postgresql_binary/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.995990 tyke-agent-0.1.8/src/tyke/agent/instrumentation/pymongo/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     1090 2023-05-19 03:04:52.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/pymongo/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.996126 tyke-agent-0.1.8/src/tyke/agent/instrumentation/pymysql/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      447 2023-05-11 12:38:46.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/pymysql/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.996263 tyke-agent-0.1.8/src/tyke/agent/instrumentation/redis/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      435 2023-05-11 12:38:39.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/redis/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.996400 tyke-agent-0.1.8/src/tyke/agent/instrumentation/remoulade/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      459 2023-05-11 12:45:19.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/remoulade/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.996536 tyke-agent-0.1.8/src/tyke/agent/instrumentation/requests/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     3238 2023-01-05 13:32:00.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/requests/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.996679 tyke-agent-0.1.8/src/tyke/agent/instrumentation/sklearn/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      447 2023-05-11 12:46:52.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/sklearn/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.996830 tyke-agent-0.1.8/src/tyke/agent/instrumentation/sqlalchemy/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      465 2023-05-11 12:48:09.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/sqlalchemy/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.996978 tyke-agent-0.1.8/src/tyke/agent/instrumentation/urllib/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      441 2023-05-11 14:12:39.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/urllib/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.997124 tyke-agent-0.1.8/src/tyke/agent/instrumentation/urllib3/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      447 2023-05-11 14:11:23.000000 tyke-agent-0.1.8/src/tyke/agent/instrumentation/urllib3/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      502 2022-10-25 04:51:53.000000 tyke-agent-0.1.8/src/tyke/env_var_settings.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)       92 2023-05-18 05:04:46.000000 tyke-agent-0.1.8/src/tyke/version.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-19 03:46:45.998233 tyke-agent-0.1.8/src/tyke_agent.egg-info/
+-rw-r--r--   0 bhaskar    (501) staff       (20)     3238 2023-05-19 03:46:45.000000 tyke-agent-0.1.8/src/tyke_agent.egg-info/PKG-INFO
+-rw-r--r--   0 bhaskar    (501) staff       (20)     2563 2023-05-19 03:46:45.000000 tyke-agent-0.1.8/src/tyke_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 bhaskar    (501) staff       (20)        1 2023-05-19 03:46:45.000000 tyke-agent-0.1.8/src/tyke_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 bhaskar    (501) staff       (20)       87 2023-05-19 03:46:45.000000 tyke-agent-0.1.8/src/tyke_agent.egg-info/entry_points.txt
+-rw-r--r--   0 bhaskar    (501) staff       (20)     1589 2023-05-19 03:46:45.000000 tyke-agent-0.1.8/src/tyke_agent.egg-info/requires.txt
+-rw-r--r--   0 bhaskar    (501) staff       (20)        5 2023-05-19 03:46:45.000000 tyke-agent-0.1.8/src/tyke_agent.egg-info/top_level.txt
```

### Comparing `tyke-agent-0.1.7/LICENSE` & `tyke-agent-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/PKG-INFO` & `tyke-agent-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyke-agent
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tyke Python Agent
 Home-page: https://tyke.ai
 Author: TykeVision
 Author-email: tech@tyke.ai
 Project-URL: Bug Tracker, https://github.com/tykevision/python-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,22 +24,25 @@
 - capture SQL queries
 - tracing context propagation
 
 Tyke python agent supports Python 3.6+
 
 | Library | Description | Supported Library Versions|
 |------|-------------| ---------------|
-| [flask](https://flask.palletsprojects.com/en/1.1.x/api)|A micro web framework written in Python.| 1.\*, 2.\*|
-| [django](https://docs.djangoproject.com/)|Python web framework | 1.10+|
-| [grpc](https://grpc.github.io/grpc/python/)|Python GRPC library.| 1.27+|
+| [flask](https://flask.palletsprojects.com/en/1.1.x/api)|A micro web framework written in Python.| 1.\*, 2.\* |
+| [django](https://docs.djangoproject.com/)|Python web framework | 1.10+ |
+| [fastapi](https://docs.djangoproject.com/)|Python web framework |  ~= 0.58 |
+| [grpc](https://grpc.github.io/grpc/python/)|Python GRPC library.| 1.27+ |
 | [mysql-connector](https://dev.mysql.com/doc/connector-python/en/)| Python MySQL database client library.| 8.\*|
+| [pymyql](https://pymysql.readthedocs.io/en/latest/)| Python MySQL database PyMysql library.| 2+|
 | [psycopg2/psycopg2-binary/postgresql](https://www.psycopg.org/docs/)|Python Postgresql database client library. | 2.7.3.1+ |
 | [requests](https://docs.python-requests.org/en/master/)|Python HTTP client library.| 2.\*|
 | [aiohttp](https://docs.aiohttp.org/en/stable/)|Python async HTTP client library.| 3.\*|
 | [pymongo](https://pymongo.readthedocs.io/en/stable/)|Python mongodb pymongo library.| >= 3.1+, < 5.0|
+| [redis](https://redis.readthedocs.io/en/latest/)|Python Redis library.| 3.0.0+|
 
 ## Getting started
 
 ## Instrumentation
 
 Instrumentation requires editing your code to initialize an agent, and registering any applicable modules to be instrumented.
```

### Comparing `tyke-agent-0.1.7/README.md` & `tyke-agent-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,25 @@
 - capture SQL queries
 - tracing context propagation
 
 Tyke python agent supports Python 3.6+
 
 | Library | Description | Supported Library Versions|
 |------|-------------| ---------------|
-| [flask](https://flask.palletsprojects.com/en/1.1.x/api)|A micro web framework written in Python.| 1.\*, 2.\*|
-| [django](https://docs.djangoproject.com/)|Python web framework | 1.10+|
-| [grpc](https://grpc.github.io/grpc/python/)|Python GRPC library.| 1.27+|
+| [flask](https://flask.palletsprojects.com/en/1.1.x/api)|A micro web framework written in Python.| 1.\*, 2.\* |
+| [django](https://docs.djangoproject.com/)|Python web framework | 1.10+ |
+| [fastapi](https://docs.djangoproject.com/)|Python web framework |  ~= 0.58 |
+| [grpc](https://grpc.github.io/grpc/python/)|Python GRPC library.| 1.27+ |
 | [mysql-connector](https://dev.mysql.com/doc/connector-python/en/)| Python MySQL database client library.| 8.\*|
+| [pymyql](https://pymysql.readthedocs.io/en/latest/)| Python MySQL database PyMysql library.| 2+|
 | [psycopg2/psycopg2-binary/postgresql](https://www.psycopg.org/docs/)|Python Postgresql database client library. | 2.7.3.1+ |
 | [requests](https://docs.python-requests.org/en/master/)|Python HTTP client library.| 2.\*|
 | [aiohttp](https://docs.aiohttp.org/en/stable/)|Python async HTTP client library.| 3.\*|
 | [pymongo](https://pymongo.readthedocs.io/en/stable/)|Python mongodb pymongo library.| >= 3.1+, < 5.0|
+| [redis](https://redis.readthedocs.io/en/latest/)|Python Redis library.| 3.0.0+|
 
 ## Getting started
 
 ## Instrumentation
 
 Instrumentation requires editing your code to initialize an agent, and registering any applicable modules to be instrumented.
```

### Comparing `tyke-agent-0.1.7/setup.py` & `tyke-agent-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/sitecustomize.py` & `tyke-agent-0.1.8/src/tyke/agent/autoinstrumentation/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/tyke_instrument.py` & `tyke-agent-0.1.8/src/tyke/agent/autoinstrumentation/tyke_instrument.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/config/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/config/config_pb2.py` & `tyke-agent-0.1.8/src/tyke/agent/config/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/config/default.py` & `tyke-agent-0.1.8/src/tyke/agent/config/default.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/config/environment.py` & `tyke-agent-0.1.8/src/tyke/agent/config/environment.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/config/file.py` & `tyke-agent-0.1.8/src/tyke/agent/config/file.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/custom_logger.py` & `tyke-agent-0.1.8/src/tyke/agent/custom_logger.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/filter/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/filter/registry.py` & `tyke-agent-0.1.8/src/tyke/agent/filter/registry.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/init/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/init/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,17 +95,18 @@
 
     # Bhaskar modified
     def eligible_based_on_content_type(self, headers: dict):
         """find content-type in headers"""
         content_type = headers.get("content-type")
         if type(content_type) is tuple:
             content_type = content_type[1]
-        return (
-            content_type if content_type in self._ALLOWED_CONTENT_TYPES else None
-        )  # plyint:disable=R1710
+        # return (
+        #     content_type if content_type in self._ALLOWED_CONTENT_TYPES else None
+        # )  # plyint:disable=R1710
+        return content_type in self._ALLOWED_CONTENT_TYPES
     
     # Bhaskar Added
     def get_content_encoding(self, headers: dict):
         """find content-type in headers"""
         try:
             content_encoding = headers.get("content-encoding")
             if type(content_encoding) is tuple:
```

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/aiohttp/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/asyncpg/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/asyncpg/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/aws_lambda/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/confluent_kafka/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/confluent_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/django/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/django/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/django/django_auto_instrumentation_compat.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/django/django_auto_instrumentation_compat.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/fast_api/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/fast_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/fast_api/fast_api_auto_instrumentation_compat.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/fast_api/fast_api_auto_instrumentation_compat.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/flask/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/grpc/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/instrumentation_definitions.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/instrumentation_definitions.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/method/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/method/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/postgresql/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/postgresql_binary/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/postgresql_binary/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke/agent/instrumentation/requests/__init__.py` & `tyke-agent-0.1.8/src/tyke/agent/instrumentation/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke_agent.egg-info/PKG-INFO` & `tyke-agent-0.1.8/src/tyke_agent.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyke-agent
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tyke Python Agent
 Home-page: https://tyke.ai
 Author: TykeVision
 Author-email: tech@tyke.ai
 Project-URL: Bug Tracker, https://github.com/tykevision/python-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,22 +24,25 @@
 - capture SQL queries
 - tracing context propagation
 
 Tyke python agent supports Python 3.6+
 
 | Library | Description | Supported Library Versions|
 |------|-------------| ---------------|
-| [flask](https://flask.palletsprojects.com/en/1.1.x/api)|A micro web framework written in Python.| 1.\*, 2.\*|
-| [django](https://docs.djangoproject.com/)|Python web framework | 1.10+|
-| [grpc](https://grpc.github.io/grpc/python/)|Python GRPC library.| 1.27+|
+| [flask](https://flask.palletsprojects.com/en/1.1.x/api)|A micro web framework written in Python.| 1.\*, 2.\* |
+| [django](https://docs.djangoproject.com/)|Python web framework | 1.10+ |
+| [fastapi](https://docs.djangoproject.com/)|Python web framework |  ~= 0.58 |
+| [grpc](https://grpc.github.io/grpc/python/)|Python GRPC library.| 1.27+ |
 | [mysql-connector](https://dev.mysql.com/doc/connector-python/en/)| Python MySQL database client library.| 8.\*|
+| [pymyql](https://pymysql.readthedocs.io/en/latest/)| Python MySQL database PyMysql library.| 2+|
 | [psycopg2/psycopg2-binary/postgresql](https://www.psycopg.org/docs/)|Python Postgresql database client library. | 2.7.3.1+ |
 | [requests](https://docs.python-requests.org/en/master/)|Python HTTP client library.| 2.\*|
 | [aiohttp](https://docs.aiohttp.org/en/stable/)|Python async HTTP client library.| 3.\*|
 | [pymongo](https://pymongo.readthedocs.io/en/stable/)|Python mongodb pymongo library.| >= 3.1+, < 5.0|
+| [redis](https://redis.readthedocs.io/en/latest/)|Python Redis library.| 3.0.0+|
 
 ## Getting started
 
 ## Instrumentation
 
 Instrumentation requires editing your code to initialize an agent, and registering any applicable modules to be instrumented.
```

### Comparing `tyke-agent-0.1.7/src/tyke_agent.egg-info/SOURCES.txt` & `tyke-agent-0.1.8/src/tyke_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.7/src/tyke_agent.egg-info/requires.txt` & `tyke-agent-0.1.8/src/tyke_agent.egg-info/requires.txt`

 * *Files identical despite different names*

