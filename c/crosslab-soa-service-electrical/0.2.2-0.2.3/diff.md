# Comparing `tmp/crosslab_soa_service_electrical-0.2.2.tar.gz` & `tmp/crosslab_soa_service_electrical-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_electrical-0.2.2.tar", last modified: Wed Apr 19 18:30:49 2023, max compression
+gzip compressed data, was "crosslab_soa_service_electrical-0.2.3.tar", last modified: Fri May 19 08:17:37 2023, max compression
```

## Comparing `crosslab_soa_service_electrical-0.2.2.tar` & `crosslab_soa_service_electrical-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.366616 crosslab_soa_service_electrical-0.2.2/
--rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-04-19 18:30:49.366616 crosslab_soa_service_electrical-0.2.2/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.2/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      585 2023-04-19 18:30:49.366616 crosslab_soa_service_electrical-0.2.2/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.2/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/
--rw-r--r--   0 dev       (1000) docker-host   (967)      256 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     5204 2023-04-19 13:37:16.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/electrical_connection_service.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      745 2023-02-10 10:19:30.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/py.typed
--rw-r--r--   0 dev       (1000) docker-host   (967)      614 2023-04-12 09:26:55.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interface.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interfaces/
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     2876 2023-04-19 13:37:16.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-04-19 18:30:49.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      770 2023-04-19 18:30:49.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:30:49.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-04-19 18:30:49.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:30:49.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)     4076 2023-04-19 13:37:16.000000 crosslab_soa_service_electrical-0.2.2/tests/test_gpio.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      810 2023-04-19 13:37:16.000000 crosslab_soa_service_electrical-0.2.2/tests/test_standard.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.823256 crosslab_soa_service_electrical-0.2.3/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-05-19 08:17:37.823256 crosslab_soa_service_electrical-0.2.3/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.3/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      585 2023-05-19 08:17:37.823256 crosslab_soa_service_electrical-0.2.3/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.3/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.813256 crosslab_soa_service_electrical-0.2.3/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.813256 crosslab_soa_service_electrical-0.2.3/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.813256 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.816589 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      256 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     5204 2023-04-26 09:19:14.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/electrical_connection_service.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      745 2023-02-10 10:19:30.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/py.typed
+-rw-r--r--   0 dev       (1000) docker-host   (967)      614 2023-04-12 09:26:55.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interface.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.819923 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interfaces/
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     2876 2023-04-26 09:19:14.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.819923 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-05-19 08:17:37.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      770 2023-05-19 08:17:37.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-19 08:17:37.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-19 08:17:37.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-19 08:17:37.000000 crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:17:37.823256 crosslab_soa_service_electrical-0.2.3/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)     4076 2023-04-26 09:19:14.000000 crosslab_soa_service_electrical-0.2.3/tests/test_gpio.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      810 2023-04-26 09:19:14.000000 crosslab_soa_service_electrical-0.2.3/tests/test_standard.py
```

### Comparing `crosslab_soa_service_electrical-0.2.2/setup.cfg` & `crosslab_soa_service_electrical-0.2.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_electrical
-version = 0.2.2
+version = 0.2.3
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Electrical Service
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/electrical_connection_service.py` & `crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/electrical_connection_service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/messages.py` & `crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/messages.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interface.py` & `crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interface.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py` & `crosslab_soa_service_electrical-0.2.3/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt` & `crosslab_soa_service_electrical-0.2.3/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.2/tests/test_gpio.py` & `crosslab_soa_service_electrical-0.2.3/tests/test_gpio.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.2/tests/test_standard.py` & `crosslab_soa_service_electrical-0.2.3/tests/test_standard.py`

 * *Files identical despite different names*

