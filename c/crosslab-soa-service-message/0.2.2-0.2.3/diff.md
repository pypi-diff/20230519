# Comparing `tmp/crosslab_soa_service_message-0.2.2.tar.gz` & `tmp/crosslab_soa_service_message-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_message-0.2.2.tar", last modified: Wed Apr 19 18:36:14 2023, max compression
+gzip compressed data, was "crosslab_soa_service_message-0.2.3.tar", last modified: Fri May 19 08:24:10 2023, max compression
```

## Comparing `crosslab_soa_service_message-0.2.2.tar` & `crosslab_soa_service_message-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/
--rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.2/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      580 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.2/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.395013 crosslab_soa_service_message-0.2.2/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.395013 crosslab_soa_service_message-0.2.2/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.395013 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/
--rw-r--r--   0 dev       (1000) docker-host   (967)      213 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     2607 2023-04-19 13:37:16.000000 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/message_service.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      232 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/py.typed
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-04-19 18:36:14.000000 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      523 2023-04-19 18:36:14.000000 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:36:14.000000 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-04-19 18:36:14.000000 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:36:14.000000 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)      916 2023-04-19 13:37:16.000000 crosslab_soa_service_message-0.2.2/tests/test_standard.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.148730 crosslab_soa_service_message-0.2.3/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-05-19 08:24:10.148730 crosslab_soa_service_message-0.2.3/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.3/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      580 2023-05-19 08:24:10.148730 crosslab_soa_service_message-0.2.3/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.3/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.145397 crosslab_soa_service_message-0.2.3/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.145397 crosslab_soa_service_message-0.2.3/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.145397 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.145397 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      213 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     2607 2023-04-26 09:19:14.000000 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/message_service.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      232 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/py.typed
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.145397 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-05-19 08:24:10.000000 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      523 2023-05-19 08:24:10.000000 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-19 08:24:10.000000 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-19 08:24:10.000000 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-19 08:24:10.000000 crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:24:10.148730 crosslab_soa_service_message-0.2.3/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      916 2023-04-26 09:19:14.000000 crosslab_soa_service_message-0.2.3/tests/test_standard.py
```

### Comparing `crosslab_soa_service_message-0.2.2/setup.cfg` & `crosslab_soa_service_message-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_message
-version = 0.2.2
+version = 0.2.3
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA message Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/message_service.py` & `crosslab_soa_service_message-0.2.3/src/crosslab/soa_services/message/message_service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/SOURCES.txt` & `crosslab_soa_service_message-0.2.3/src/crosslab_soa_service_message.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_message-0.2.2/tests/test_standard.py` & `crosslab_soa_service_message-0.2.3/tests/test_standard.py`

 * *Files identical despite different names*

