# Comparing `tmp/rabbitmq-broker-0.1.2.tar.gz` & `tmp/rabbitmq-broker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitmq-broker-0.1.2.tar", last modified: Fri May 19 11:42:43 2023, max compression
+gzip compressed data, was "rabbitmq-broker-1.0.0.tar", last modified: Fri May 19 12:52:32 2023, max compression
```

## Comparing `rabbitmq-broker-0.1.2.tar` & `rabbitmq-broker-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 11:42:43.132286 rabbitmq-broker-0.1.2/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-0.1.2/HISTORY.rst
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1074 2023-05-18 13:33:44.000000 rabbitmq-broker-0.1.2/LICENSE
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      158 2023-05-18 13:33:44.000000 rabbitmq-broker-0.1.2/MANIFEST.in
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     2116 2023-05-19 11:42:43.136286 rabbitmq-broker-0.1.2/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1731 2023-05-18 14:21:48.000000 rabbitmq-broker-0.1.2/README.md
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2023-05-18 13:42:42.000000 rabbitmq-broker-0.1.2/README.rst
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      599 2023-05-19 11:42:30.000000 rabbitmq-broker-0.1.2/pyproject.toml
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 11:42:43.124286 rabbitmq-broker-0.1.2/rabbitmq_broker.egg-info/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     2116 2023-05-19 11:42:43.000000 rabbitmq-broker-0.1.2/rabbitmq_broker.egg-info/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      566 2023-05-19 11:42:43.000000 rabbitmq-broker-0.1.2/rabbitmq_broker.egg-info/SOURCES.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2023-05-19 11:42:43.000000 rabbitmq-broker-0.1.2/rabbitmq_broker.egg-info/dependency_links.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       70 2023-05-19 11:42:43.000000 rabbitmq-broker-0.1.2/rabbitmq_broker.egg-info/requires.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       11 2023-05-19 11:42:43.000000 rabbitmq-broker-0.1.2/rabbitmq_broker.egg-info/top_level.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      228 2023-05-19 10:05:15.000000 rabbitmq-broker-0.1.2/requirements.txt
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 11:42:43.128286 rabbitmq-broker-0.1.2/rmq_broker/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       22 2023-05-19 11:42:36.000000 rabbitmq-broker-0.1.2/rmq_broker/__init__.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 11:42:43.128286 rabbitmq-broker-0.1.2/rmq_broker/async_chains/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:36:17.000000 rabbitmq-broker-0.1.2/rmq_broker/async_chains/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     7340 2023-05-18 13:36:17.000000 rabbitmq-broker-0.1.2/rmq_broker/async_chains/base.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 11:42:43.128286 rabbitmq-broker-0.1.2/rmq_broker/chains/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-0.1.2/rmq_broker/chains/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     7304 2023-05-18 13:36:17.000000 rabbitmq-broker-0.1.2/rmq_broker/chains/base.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 11:42:43.132286 rabbitmq-broker-0.1.2/rmq_broker/queues/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-0.1.2/rmq_broker/queues/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1107 2023-05-18 14:09:24.000000 rabbitmq-broker-0.1.2/rmq_broker/queues/base.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1765 2023-05-18 13:36:17.000000 rabbitmq-broker-0.1.2/rmq_broker/queues/rabbitmq.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      620 2023-05-18 13:36:17.000000 rabbitmq-broker-0.1.2/rmq_broker/schemas.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      512 2023-05-18 13:36:17.000000 rabbitmq-broker-0.1.2/rmq_broker/settings.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      928 2023-05-19 11:42:43.136286 rabbitmq-broker-0.1.2/setup.cfg
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.327794 rabbitmq-broker-1.0.0/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.0/HISTORY.rst
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1074 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.0/LICENSE
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      158 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.0/MANIFEST.in
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     4277 2023-05-19 12:52:32.327794 rabbitmq-broker-1.0.0/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     3893 2023-05-19 12:52:16.000000 rabbitmq-broker-1.0.0/README.md
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2023-05-18 13:42:42.000000 rabbitmq-broker-1.0.0/README.rst
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      599 2023-05-19 12:06:12.000000 rabbitmq-broker-1.0.0/pyproject.toml
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.319795 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     4277 2023-05-19 12:52:32.000000 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      566 2023-05-19 12:52:32.000000 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2023-05-19 12:52:32.000000 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       70 2023-05-19 12:52:32.000000 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/requires.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       11 2023-05-19 12:52:32.000000 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/top_level.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      228 2023-05-19 12:06:03.000000 rabbitmq-broker-1.0.0/requirements.txt
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.323794 rabbitmq-broker-1.0.0/rmq_broker/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       22 2023-05-19 12:06:01.000000 rabbitmq-broker-1.0.0/rmq_broker/__init__.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.323794 rabbitmq-broker-1.0.0/rmq_broker/async_chains/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/async_chains/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     7340 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/async_chains/base.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.323794 rabbitmq-broker-1.0.0/rmq_broker/chains/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.0/rmq_broker/chains/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     7304 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/chains/base.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.327794 rabbitmq-broker-1.0.0/rmq_broker/queues/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.0/rmq_broker/queues/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1107 2023-05-18 14:09:24.000000 rabbitmq-broker-1.0.0/rmq_broker/queues/base.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1765 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/queues/rabbitmq.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      620 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/schemas.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      512 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/settings.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      928 2023-05-19 12:52:32.327794 rabbitmq-broker-1.0.0/setup.cfg
```

### Comparing `rabbitmq-broker-0.1.2/LICENSE` & `rabbitmq-broker-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-0.1.2/pyproject.toml` & `rabbitmq-broker-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rabbitmq-broker"
-version = "0.1.2"
+version = "1.0.0"
 authors = [
   { name="Nikita Sysoev", email="njt55cs@gmail.com" },
 ]
 description = "RPC брокер сообщений"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `rabbitmq-broker-0.1.2/rabbitmq_broker.egg-info/SOURCES.txt` & `rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-0.1.2/rmq_broker/async_chains/base.py` & `rabbitmq-broker-1.0.0/rmq_broker/async_chains/base.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-0.1.2/rmq_broker/chains/base.py` & `rabbitmq-broker-1.0.0/rmq_broker/chains/base.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-0.1.2/rmq_broker/queues/base.py` & `rabbitmq-broker-1.0.0/rmq_broker/queues/base.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-0.1.2/rmq_broker/queues/rabbitmq.py` & `rabbitmq-broker-1.0.0/rmq_broker/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-0.1.2/rmq_broker/schemas.py` & `rabbitmq-broker-1.0.0/rmq_broker/schemas.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-0.1.2/rmq_broker/settings.py` & `rabbitmq-broker-1.0.0/rmq_broker/settings.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-0.1.2/setup.cfg` & `rabbitmq-broker-1.0.0/setup.cfg`

 * *Files identical despite different names*

