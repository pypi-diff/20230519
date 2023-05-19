# Comparing `tmp/fastkafka-0.6.0rc0.tar.gz` & `tmp/fastkafka-0.6.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkafka-0.6.0rc0.tar", last modified: Fri May 12 13:45:18 2023, max compression
+gzip compressed data, was "fastkafka-0.6.1rc0.tar", last modified: Fri May 19 12:58:29 2023, max compression
```

## Comparing `fastkafka-0.6.0rc0.tar` & `fastkafka-0.6.1rc0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/
--rw-r--r--   0 davor     (1000) davor     (1000)    11864 2023-05-12 12:45:54.000000 fastkafka-0.6.0rc0/CONTRIBUTING.md
--rw-r--r--   0 davor     (1000) davor     (1000)    11357 2023-01-25 09:24:15.000000 fastkafka-0.6.0rc0/LICENSE
--rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-01-25 09:24:15.000000 fastkafka-0.6.0rc0/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    29859 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/PKG-INFO
--rw-r--r--   0 davor     (1000) davor     (1000)    28431 2023-04-21 14:13:44.000000 fastkafka-0.6.0rc0/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.190037 fastkafka-0.6.0rc0/fastkafka/
--rw-r--r--   0 davor     (1000) davor     (1000)      525 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.190037 fastkafka-0.6.0rc0/fastkafka/_application/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_application/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    31006 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_application/app.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     7688 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_application/tester.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     1631 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_cli.py
--rw-r--r--   0 davor     (1000) davor     (1000)     3879 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_cli_docs.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      852 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_cli_testing.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/fastkafka/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     3705 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_components/_subprocess.py
--rw-r--r--   0 davor     (1000) davor     (1000)    10188 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_components/aiokafka_consumer_loop.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    16654 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_components/asyncapi.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     2940 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_components/benchmarking.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     4706 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/docs_dependencies.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/fastkafka/_components/encoder/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/encoder/__init__.py
--rw-r--r--   0 davor     (1000) davor     (1000)    13910 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_components/encoder/avro.py
--rw-r--r--   0 davor     (1000) davor     (1000)     1640 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_components/encoder/json.py
--rw-r--r--   0 davor     (1000) davor     (1000)     2952 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/helpers.py
--rw-r--r--   0 davor     (1000) davor     (1000)     4446 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/logger.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    12567 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/meta.py
--rw-r--r--   0 davor     (1000) davor     (1000)     5930 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_components/producer_decorator.py
--rw-r--r--   0 davor     (1000) davor     (1000)     8081 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_components/task_streaming.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     5090 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/test_dependencies.py
--rw-r--r--   0 davor     (1000) davor     (1000)    17520 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_docusaurus_helper.py
--rw-r--r--   0 davor     (1000) davor     (1000)    50547 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    80310 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_modidx.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     6095 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_server.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/fastkafka/_testing/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_testing/__init__.py
--rw-r--r--   0 davor     (1000) davor     (1000)    19995 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_testing/apache_kafka_broker.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    20456 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_testing/in_memory_broker.py
--rw-r--r--   0 davor     (1000) davor     (1000)    12364 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_testing/local_redpanda_broker.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     4671 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_testing/test_utils.py
--rw-r--r--   0 davor     (1000) davor     (1000)      598 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/encoder.py
--rw-r--r--   0 davor     (1000) davor     (1000)      858 2023-05-12 13:44:35.000000 fastkafka-0.6.0rc0/fastkafka/testing.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.190037 fastkafka-0.6.0rc0/fastkafka.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    29859 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     1387 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      146 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-01-25 09:30:21.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      611 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       10 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/top_level.txt
--rw-r--r--   0 davor     (1000) davor     (1000)     1231 2023-05-12 12:45:54.000000 fastkafka-0.6.0rc0/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/setup.cfg
--rw-rw-r--   0 davor     (1000) davor     (1000)     3682 2023-05-12 13:44:07.000000 fastkafka-0.6.0rc0/setup.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11864 2023-05-19 12:02:29.000000 fastkafka-0.6.1rc0/CONTRIBUTING.md
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-03-14 07:16:19.000000 fastkafka-0.6.1rc0/LICENSE
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-03-14 07:16:19.000000 fastkafka-0.6.1rc0/MANIFEST.in
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    29859 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28431 2023-04-20 13:45:13.000000 fastkafka-0.6.1rc0/README.md
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.874296 fastkafka-0.6.1rc0/fastkafka/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/__init__.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.874296 fastkafka-0.6.1rc0/fastkafka/_application/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_application/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    31006 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_application/app.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7746 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_application/tester.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1631 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_cli.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3879 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_cli_docs.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      852 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_cli_testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/fastkafka/_components/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3705 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_components/_subprocess.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    10188 2023-05-19 12:53:39.000000 fastkafka-0.6.1rc0/fastkafka/_components/aiokafka_consumer_loop.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    16654 2023-05-19 12:53:39.000000 fastkafka-0.6.1rc0/fastkafka/_components/asyncapi.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2940 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_components/benchmarking.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4706 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/docs_dependencies.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/fastkafka/_components/encoder/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/encoder/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13910 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_components/encoder/avro.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1640 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_components/encoder/json.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2952 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4446 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/logger.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12567 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/meta.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5930 2023-05-19 12:53:39.000000 fastkafka-0.6.1rc0/fastkafka/_components/producer_decorator.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     8081 2023-05-19 12:53:39.000000 fastkafka-0.6.1rc0/fastkafka/_components/task_streaming.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5090 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/test_dependencies.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    17520 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_docusaurus_helper.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    50547 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    80310 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_modidx.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6095 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_server.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/fastkafka/_testing/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_testing/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    19995 2023-05-19 12:53:38.000000 fastkafka-0.6.1rc0/fastkafka/_testing/apache_kafka_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    20456 2023-05-19 12:53:38.000000 fastkafka-0.6.1rc0/fastkafka/_testing/in_memory_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12364 2023-05-19 12:53:38.000000 fastkafka-0.6.1rc0/fastkafka/_testing/local_redpanda_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4671 2023-05-19 12:53:39.000000 fastkafka-0.6.1rc0/fastkafka/_testing/test_utils.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/encoder.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-05-19 12:53:38.000000 fastkafka-0.6.1rc0/fastkafka/testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.874296 fastkafka-0.6.1rc0/fastkafka.egg-info/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    29859 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1387 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/entry_points.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-03-14 07:23:45.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/not-zip-safe
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      611 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/requires.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/top_level.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-05-19 12:53:24.000000 fastkafka-0.6.1rc0/settings.ini
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/setup.cfg
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3682 2023-05-19 12:02:29.000000 fastkafka-0.6.1rc0/setup.py
```

### Comparing `fastkafka-0.6.0rc0/CONTRIBUTING.md` & `fastkafka-0.6.1rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/LICENSE` & `fastkafka-0.6.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/PKG-INFO` & `fastkafka-0.6.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.6.0rc0
+Version: 0.6.1rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
```

### Comparing `fastkafka-0.6.0rc0/README.md` & `fastkafka-0.6.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/__init__.py` & `fastkafka-0.6.1rc0/fastkafka/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.0rc0"
+__version__ = "0.6.1rc0"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/010_Application_export.ipynb.
 
 # %% auto 0
 __all__ = ['dummy']
 
 # %% ../nbs/010_Application_export.ipynb 1
 from ._application.app import FastKafka
```

### Comparing `fastkafka-0.6.0rc0/fastkafka/_application/app.py` & `fastkafka-0.6.1rc0/fastkafka/_application/app.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_application/tester.py` & `fastkafka-0.6.1rc0/fastkafka/_application/tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     async def skeleton_func(msg: BaseModel) -> None:
         pass
 
     mirror_func = skeleton_func
     sig = inspect.signature(skeleton_func)
 
     # adjust name
-    mirror_func.__name__ = "on_" + topic
+    mirror_func.__name__ = "on_" + topic.replace(".", "_")
 
     # adjust arg and return val
     sig = sig.replace(
         parameters=[
             inspect.Parameter(
                 name="msg",
                 annotation=msg_type,
@@ -185,27 +185,27 @@
     async def skeleton_func(msg: BaseModel) -> BaseModel:
         return msg
 
     mirror_func = skeleton_func
     sig = inspect.signature(skeleton_func)
 
     # adjust name
-    mirror_func.__name__ = "to_" + topic
+    mirror_func.__name__ = "to_" + topic.replace(".", "_")
 
     # adjust arg and return val
     sig = sig.replace(parameters=[msg_type], return_annotation=msg_type.annotation)
 
     mirror_func.__signature__ = sig  # type: ignore
     return mirror_func
 
 # %% ../../nbs/016_Tester.ipynb 18
 @patch
 def create_mirrors(self: Tester) -> None:
     for app in self.apps:
         for topic, (consumer_f, _, _, _) in app._consumers_store.items():
             mirror_f = mirror_consumer(topic, consumer_f)
-            mirror_f = self.produces()(mirror_f)  # type: ignore
+            mirror_f = self.produces(topic=topic)(mirror_f)  # type: ignore
             setattr(self, mirror_f.__name__, mirror_f)
         for topic, (producer_f, _, _) in app._producers_store.items():
             mirror_f = mirror_producer(topic, producer_f)
-            mirror_f = self.consumes()(mirror_f)  # type: ignore
+            mirror_f = self.consumes(topic=topic)(mirror_f)  # type: ignore
             setattr(self, mirror_f.__name__, mirror_f)
```

### Comparing `fastkafka-0.6.0rc0/fastkafka/_cli.py` & `fastkafka-0.6.1rc0/fastkafka/_cli.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_cli_docs.py` & `fastkafka-0.6.1rc0/fastkafka/_cli_docs.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_cli_testing.py` & `fastkafka-0.6.1rc0/fastkafka/_cli_testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/_subprocess.py` & `fastkafka-0.6.1rc0/fastkafka/_components/_subprocess.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/aiokafka_consumer_loop.py` & `fastkafka-0.6.1rc0/fastkafka/_components/aiokafka_consumer_loop.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/asyncapi.py` & `fastkafka-0.6.1rc0/fastkafka/_components/asyncapi.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/benchmarking.py` & `fastkafka-0.6.1rc0/fastkafka/_components/benchmarking.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/docs_dependencies.py` & `fastkafka-0.6.1rc0/fastkafka/_components/docs_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/encoder/avro.py` & `fastkafka-0.6.1rc0/fastkafka/_components/encoder/avro.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/encoder/json.py` & `fastkafka-0.6.1rc0/fastkafka/_components/encoder/json.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/helpers.py` & `fastkafka-0.6.1rc0/fastkafka/_components/helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/logger.py` & `fastkafka-0.6.1rc0/fastkafka/_components/logger.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/meta.py` & `fastkafka-0.6.1rc0/fastkafka/_components/meta.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/producer_decorator.py` & `fastkafka-0.6.1rc0/fastkafka/_components/producer_decorator.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/task_streaming.py` & `fastkafka-0.6.1rc0/fastkafka/_components/task_streaming.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_components/test_dependencies.py` & `fastkafka-0.6.1rc0/fastkafka/_components/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_docusaurus_helper.py` & `fastkafka-0.6.1rc0/fastkafka/_docusaurus_helper.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_helpers.py` & `fastkafka-0.6.1rc0/fastkafka/_helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_modidx.py` & `fastkafka-0.6.1rc0/fastkafka/_modidx.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_server.py` & `fastkafka-0.6.1rc0/fastkafka/_server.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_testing/apache_kafka_broker.py` & `fastkafka-0.6.1rc0/fastkafka/_testing/apache_kafka_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_testing/in_memory_broker.py` & `fastkafka-0.6.1rc0/fastkafka/_testing/in_memory_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_testing/local_redpanda_broker.py` & `fastkafka-0.6.1rc0/fastkafka/_testing/local_redpanda_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/_testing/test_utils.py` & `fastkafka-0.6.1rc0/fastkafka/_testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/encoder.py` & `fastkafka-0.6.1rc0/fastkafka/encoder.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka/testing.py` & `fastkafka-0.6.1rc0/fastkafka/testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka.egg-info/PKG-INFO` & `fastkafka-0.6.1rc0/fastkafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.6.0rc0
+Version: 0.6.1rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
```

### Comparing `fastkafka-0.6.0rc0/fastkafka.egg-info/SOURCES.txt` & `fastkafka-0.6.1rc0/fastkafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/fastkafka.egg-info/requires.txt` & `fastkafka-0.6.1rc0/fastkafka.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.0rc0/settings.ini` & `fastkafka-0.6.1rc0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastkafka
 lib_name = %(repo)s
-version = 0.6.0rc0
+version = 0.6.1rc0
 min_python = 3.8
 license = apache2
 
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastkafka
```

### Comparing `fastkafka-0.6.0rc0/setup.py` & `fastkafka-0.6.1rc0/setup.py`

 * *Files identical despite different names*

