# Comparing `tmp/loadbalancer_interface-1.1.2.tar.gz` & `tmp/loadbalancer_interface-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Nov 22 22:36:49 2022, from Unix
+gzip compressed data, was "loadbalancer_interface-1.2.0.tar", last modified: Fri May 19 20:58:09 2023, max compression
```

## Comparing `loadbalancer_interface-1.1.2.tar` & `loadbalancer_interface-1.2.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/
--rw-rw-r--   0 addyess   (1000) addyess   (1000)     4770 2022-11-22 22:34:44.000000 loadbalancer_interface-1.1.1/PKG-INFO
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     3719 2021-03-16 21:24:03.000000 loadbalancer_interface-1.1.1/README.md
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-consumer/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       81 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-consumer/config.yaml
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)      281 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-consumer/metadata.yaml
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       21 2021-03-11 23:06:50.000000 loadbalancer_interface-1.1.1/examples/lb-consumer/requirements.txt
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-consumer/src/
--rwxrwxr-x   0 johnsca   (1000) johnsca   (1000)     2120 2021-03-12 17:02:08.000000 loadbalancer_interface-1.1.1/examples/lb-consumer/src/charm.py
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-consumer-reactive/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       81 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-consumer-reactive/config.yaml
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       42 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-consumer-reactive/layer.yaml
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)      290 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-consumer-reactive/metadata.yaml
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-consumer-reactive/reactive/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     1690 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-consumer-reactive/reactive/charm.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       17 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-consumer-reactive/wheelhouse.txt
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-provider/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)      205 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-provider/metadata.yaml
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       21 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-provider/requirements.txt
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-provider/src/
--rwxrwxr-x   0 johnsca   (1000) johnsca   (1000)     1452 2021-04-05 18:46:16.000000 loadbalancer_interface-1.1.1/examples/lb-provider/src/charm.py
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-provider-reactive/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       42 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-provider-reactive/layer.yaml
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-provider-reactive/lib/
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-provider-reactive/lib/charms/
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-provider-reactive/lib/charms/layer/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       46 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-provider-reactive/lib/charms/layer/provides_reactive.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)      214 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-provider-reactive/metadata.yaml
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/examples/lb-provider-reactive/reactive/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)      979 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-provider-reactive/reactive/charm.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       17 2021-03-08 19:24:40.000000 loadbalancer_interface-1.1.1/examples/lb-provider-reactive/wheelhouse.txt
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/loadbalancer_interface/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       83 2021-03-01 23:18:06.000000 loadbalancer_interface-1.1.1/loadbalancer_interface/__init__.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     1727 2021-02-23 22:28:20.000000 loadbalancer_interface-1.1.1/loadbalancer_interface/base.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     4823 2021-03-09 20:14:36.000000 loadbalancer_interface-1.1.1/loadbalancer_interface/provides.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     2541 2021-03-16 21:24:03.000000 loadbalancer_interface-1.1.1/loadbalancer_interface/pytest_plugin.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     9544 2021-04-20 18:19:43.000000 loadbalancer_interface-1.1.1/loadbalancer_interface/requires.py
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/loadbalancer_interface/schemas/
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)      359 2021-02-10 16:58:09.000000 loadbalancer_interface-1.1.1/loadbalancer_interface/schemas/__init__.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     2305 2021-02-10 16:58:09.000000 loadbalancer_interface-1.1.1/loadbalancer_interface/schemas/base.py
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)     4315 2021-03-01 20:40:23.000000 loadbalancer_interface-1.1.1/loadbalancer_interface/schemas/v1.py
-drwxrwxr-x   0 johnsca   (1000) johnsca   (1000)        0 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/loadbalancer_interface.egg-info/
--rw-rw-r--   0 addyess   (1000) addyess   (1000)     4770 2022-11-22 22:35:49.000000 loadbalancer_interface-1.1.1/loadbalancer_interface.egg-info/PKG-INFO
--rw-rw-r--   0 addyess   (1000) addyess   (1000)     1305 2022-11-22 22:36:48.000000 loadbalancer_interface-1.1.1/loadbalancer_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)        1 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/loadbalancer_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)      244 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/loadbalancer_interface.egg-info/entry_points.txt
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       79 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/loadbalancer_interface.egg-info/requires.txt
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       23 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/loadbalancer_interface.egg-info/top_level.txt
--rw-rw-r--   0 johnsca   (1000) johnsca   (1000)       38 2021-04-20 18:20:21.000000 loadbalancer_interface-1.1.1/setup.cfg
--rw-rw-r--   0 addyess   (1000) addyess   (1000)     1994 2022-11-22 22:35:17.000000 loadbalancer_interface-1.1.1/setup.py
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.847901 loadbalancer_interface-1.2.0/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)    11357 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/LICENSE
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     4057 2023-05-19 20:58:09.847901 loadbalancer_interface-1.2.0/PKG-INFO
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     3719 2023-05-17 13:37:25.000000 loadbalancer_interface-1.2.0/README.md
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.839901 loadbalancer_interface-1.2.0/examples/
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.839901 loadbalancer_interface-1.2.0/examples/lb-consumer/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      186 2023-05-16 21:41:25.000000 loadbalancer_interface-1.2.0/examples/lb-consumer/charmcraft.yaml
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       81 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/examples/lb-consumer/config.yaml
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      281 2023-05-16 21:41:25.000000 loadbalancer_interface-1.2.0/examples/lb-consumer/metadata.yaml
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       21 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/examples/lb-consumer/requirements.txt
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.843901 loadbalancer_interface-1.2.0/examples/lb-consumer/src/
+-rwxrwxr-x   0 addyess   (1000) addyess   (1000)     2120 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/examples/lb-consumer/src/charm.py
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.843901 loadbalancer_interface-1.2.0/examples/lb-consumer-reactive/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       81 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/examples/lb-consumer-reactive/config.yaml
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       42 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/examples/lb-consumer-reactive/layer.yaml
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      290 2023-05-16 21:41:25.000000 loadbalancer_interface-1.2.0/examples/lb-consumer-reactive/metadata.yaml
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.843901 loadbalancer_interface-1.2.0/examples/lb-consumer-reactive/reactive/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     1690 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/examples/lb-consumer-reactive/reactive/charm.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       28 2023-05-16 21:41:25.000000 loadbalancer_interface-1.2.0/examples/lb-consumer-reactive/wheelhouse.txt
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.843901 loadbalancer_interface-1.2.0/examples/lb-provider/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      186 2023-05-16 21:41:25.000000 loadbalancer_interface-1.2.0/examples/lb-provider/charmcraft.yaml
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      205 2023-05-16 21:41:25.000000 loadbalancer_interface-1.2.0/examples/lb-provider/metadata.yaml
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       21 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/examples/lb-provider/requirements.txt
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.843901 loadbalancer_interface-1.2.0/examples/lb-provider/src/
+-rwxrwxr-x   0 addyess   (1000) addyess   (1000)     1452 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/examples/lb-provider/src/charm.py
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.843901 loadbalancer_interface-1.2.0/examples/lb-provider-reactive/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       42 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/examples/lb-provider-reactive/layer.yaml
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.839901 loadbalancer_interface-1.2.0/examples/lb-provider-reactive/lib/
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.839901 loadbalancer_interface-1.2.0/examples/lb-provider-reactive/lib/charms/
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.843901 loadbalancer_interface-1.2.0/examples/lb-provider-reactive/lib/charms/layer/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       46 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/examples/lb-provider-reactive/lib/charms/layer/provides_reactive.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      214 2023-05-16 21:41:25.000000 loadbalancer_interface-1.2.0/examples/lb-provider-reactive/metadata.yaml
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.843901 loadbalancer_interface-1.2.0/examples/lb-provider-reactive/reactive/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     1148 2023-05-19 20:57:09.000000 loadbalancer_interface-1.2.0/examples/lb-provider-reactive/reactive/charm.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       28 2023-05-16 21:41:25.000000 loadbalancer_interface-1.2.0/examples/lb-provider-reactive/wheelhouse.txt
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.847901 loadbalancer_interface-1.2.0/loadbalancer_interface/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       83 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/loadbalancer_interface/__init__.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     1727 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/loadbalancer_interface/base.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     5639 2023-05-19 20:57:09.000000 loadbalancer_interface-1.2.0/loadbalancer_interface/provides.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     2892 2023-05-16 21:41:25.000000 loadbalancer_interface-1.2.0/loadbalancer_interface/pytest_plugin.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     9544 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/loadbalancer_interface/requires.py
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.847901 loadbalancer_interface-1.2.0/loadbalancer_interface/schemas/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      359 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/loadbalancer_interface/schemas/__init__.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     2305 2023-03-03 16:55:44.000000 loadbalancer_interface-1.2.0/loadbalancer_interface/schemas/base.py
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     4345 2023-05-16 21:41:25.000000 loadbalancer_interface-1.2.0/loadbalancer_interface/schemas/v1.py
+drwxrwxr-x   0 addyess   (1000) addyess   (1000)        0 2023-05-19 20:58:09.847901 loadbalancer_interface-1.2.0/loadbalancer_interface.egg-info/
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     4057 2023-05-19 20:58:09.000000 loadbalancer_interface-1.2.0/loadbalancer_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     1386 2023-05-19 20:58:09.000000 loadbalancer_interface-1.2.0/loadbalancer_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)        1 2023-05-19 20:58:09.000000 loadbalancer_interface-1.2.0/loadbalancer_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)      243 2023-05-19 20:58:09.000000 loadbalancer_interface-1.2.0/loadbalancer_interface.egg-info/entry_points.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       79 2023-05-19 20:58:09.000000 loadbalancer_interface-1.2.0/loadbalancer_interface.egg-info/requires.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       23 2023-05-19 20:58:09.000000 loadbalancer_interface-1.2.0/loadbalancer_interface.egg-info/top_level.txt
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)       38 2023-05-19 20:58:09.847901 loadbalancer_interface-1.2.0/setup.cfg
+-rw-rw-r--   0 addyess   (1000) addyess   (1000)     1994 2023-05-19 20:57:09.000000 loadbalancer_interface-1.2.0/setup.py
```

### Comparing `loadbalancer_interface-1.1.1/PKG-INFO` & `loadbalancer_interface-1.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,99 @@
 Metadata-Version: 2.1
 Name: loadbalancer_interface
-Version: 1.1.2
+Version: 1.2.0
 Summary: 'loadbalancer' interface protocol API library
 Home-page: https://github.com/juju-solutions/loadbalancer-interface
 Author: Cory Johns
 Author-email: cory.johns@canonical.com
 License: Apache License 2.0
-Description: # `loadbalancer` Interface Protocol API Library
-        
-        This library provides an API for requesting and providing load balancers or
-        ingress endpoints from one charm to another. It can be used in either charms
-        written in the newer [Operator Framework][] or older charms still using the
-        [charms.reactive Framework][].
-        
-        
-        ## Installation / Setup
-        
-        Include this library as a dependency for your charm, either in
-        `requirements.txt` for Operator Framework charms, or `wheelhouse.txt` for
-        reactive charms:
-        
-        ```
-        loadbalancer_interface
-        ```
-        
-        ## Usage
-        
-        ### Requesting Load Balancers
-        
-        Requesting a load balancer from a provider is done via the `LBProvider` class.
-        The general pattern for using the class is:
-        
-          * Wait for the provider to become available
-          * Get a `Request` object via the `get_request(name)` method
-          * Set the appropriate fields on the request object
-          * Send the `Request` via the `send_request(request)` method
-          * Wait for the `Response` to be provided (or updated)
-          * Get the `Response` object via either the `get_response(name)` method or
-            via the `new_responses` property
-          * Confirm that the request was successful and use the provided LB's address
-          * Acknowledge the `Response` via `ack_response(response)`
-        
-        There are examples in the repo for how to do this in [an operator charm][requires-operator]
-        or in [a reactive charm][requires-reactive].
-        
-        
-        ### Providing Load Balancers
-        
-        Providing a load balancer to consumers is done via the `LBConsumers` class.  The
-        general pattern for using the class is:
-        
-          * Wait for new or updated requests to come in
-          * Iterate over each request object in the `new_requests` property
-          * Create a load balancer according to the request's fields
-          * Set the appropriate fields on the request's `response` object
-          * Send the request's response via the `send_response(request)` method
-        
-        There are examples in the repo for how to do this in [an operator charm][provides-operator]
-        or in [a reactive charm][provides-reactive].
-        
-        ## API Reference
-        
-        See the [API docs][] for detailed reference on the API.
-        
-        ## Test Charms
-        
-        To ease testing of charms using this interface, this library provides test charms
-        which can be used with the pytest-operator plugin based integration test to
-        serve as a basic counterpart to the charm providing or requiring this interface.
-        
-        The charms are accessed via an `lb_charms` fixture, which is session scoped.
-        The fixture provides an object with attributes for each of the [example
-        charms][] available in the repo. (The attribute names will be the charm names
-        with dashes replaced with underscores.) For example:
-        
-        ```python
-        async def test_build_and_deploy(ops_test, lb_charms):
-            my_charm = await ops_test.build_charm(".")
-            lb_provider = await ops_test.build_charm(lb_charms.lb_provider)
-            await ops_test.model.deploy(my_charm)
-            await ops_test.model.deploy(lb_provider)
-            await ops_test.model.add_relation("my-charm", "lb-provider")
-        ```
-        
-        
-        <!-- Links -->
-        
-        [Operator Framework]: https://github.com/canonical/operator/
-        [charms.reactive Framework]: https://charmsreactive.readthedocs.io/
-        [requires-operator]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/requires-operator/
-        [requires-reactive]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/requires-reactive/
-        [provides-operator]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/provides-operator/
-        [provides-reactive]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/provides-reactive/
-        [API docs]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/docs/api.md
-        [example charms]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# `loadbalancer` Interface Protocol API Library
+
+This library provides an API for requesting and providing load balancers or
+ingress endpoints from one charm to another. It can be used in either charms
+written in the newer [Operator Framework][] or older charms still using the
+[charms.reactive Framework][].
+
+
+## Installation / Setup
+
+Include this library as a dependency for your charm, either in
+`requirements.txt` for Operator Framework charms, or `wheelhouse.txt` for
+reactive charms:
+
+```
+loadbalancer_interface
+```
+
+## Usage
+
+### Requesting Load Balancers
+
+Requesting a load balancer from a provider is done via the `LBProvider` class.
+The general pattern for using the class is:
+
+  * Wait for the provider to become available
+  * Get a `Request` object via the `get_request(name)` method
+  * Set the appropriate fields on the request object
+  * Send the `Request` via the `send_request(request)` method
+  * Wait for the `Response` to be provided (or updated)
+  * Get the `Response` object via either the `get_response(name)` method or
+    via the `new_responses` property
+  * Confirm that the request was successful and use the provided LB's address
+  * Acknowledge the `Response` via `ack_response(response)`
+
+There are examples in the repo for how to do this in [an operator charm][requires-operator]
+or in [a reactive charm][requires-reactive].
+
+
+### Providing Load Balancers
+
+Providing a load balancer to consumers is done via the `LBConsumers` class.  The
+general pattern for using the class is:
+
+  * Wait for new or updated requests to come in
+  * Iterate over each request object in the `new_requests` property
+  * Create a load balancer according to the request's fields
+  * Set the appropriate fields on the request's `response` object
+  * Send the request's response via the `send_response(request)` method
+
+There are examples in the repo for how to do this in [an operator charm][provides-operator]
+or in [a reactive charm][provides-reactive].
+
+## API Reference
+
+See the [API docs][] for detailed reference on the API.
+
+## Test Charms
+
+To ease testing of charms using this interface, this library provides test charms
+which can be used with the pytest-operator plugin based integration test to
+serve as a basic counterpart to the charm providing or requiring this interface.
+
+The charms are accessed via an `lb_charms` fixture, which is session scoped.
+The fixture provides an object with attributes for each of the [example
+charms][] available in the repo. (The attribute names will be the charm names
+with dashes replaced with underscores.) For example:
+
+```python
+async def test_build_and_deploy(ops_test, lb_charms):
+    my_charm = await ops_test.build_charm(".")
+    lb_provider = await ops_test.build_charm(lb_charms.lb_provider)
+    await ops_test.model.deploy(my_charm)
+    await ops_test.model.deploy(lb_provider)
+    await ops_test.model.add_relation("my-charm", "lb-provider")
+```
+
+
+<!-- Links -->
+
+[Operator Framework]: https://github.com/canonical/operator/
+[charms.reactive Framework]: https://charmsreactive.readthedocs.io/
+[requires-operator]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/requires-operator/
+[requires-reactive]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/requires-reactive/
+[provides-operator]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/provides-operator/
+[provides-reactive]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/provides-reactive/
+[API docs]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/docs/api.md
+[example charms]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples
```

### Comparing `loadbalancer_interface-1.1.1/README.md` & `loadbalancer_interface-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `loadbalancer_interface-1.1.1/examples/lb-consumer/src/charm.py` & `loadbalancer_interface-1.2.0/examples/lb-consumer/src/charm.py`

 * *Files identical despite different names*

### Comparing `loadbalancer_interface-1.1.1/examples/lb-consumer-reactive/reactive/charm.py` & `loadbalancer_interface-1.2.0/examples/lb-consumer-reactive/reactive/charm.py`

 * *Files identical despite different names*

### Comparing `loadbalancer_interface-1.1.1/examples/lb-provider/src/charm.py` & `loadbalancer_interface-1.2.0/examples/lb-provider/src/charm.py`

 * *Files identical despite different names*

### Comparing `loadbalancer_interface-1.1.1/examples/lb-provider-reactive/reactive/charm.py` & `loadbalancer_interface-1.2.0/examples/lb-provider-reactive/reactive/charm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 #!/usr/bin/env python3
 
 from charms.reactive import when, when_not, set_flag, endpoint_from_name
 from charms import layer
 
 
+def allow_lb_consumers_to_read_requests():
+    lb_consumers = endpoint_from_name("lb-consumers")
+    lb_consumers.follower_perms(read=True)
+    return lb_consumers
+
+
 @when_not("charm.status.is-set")
 def set_status():
     layer.status.active("")
     set_flag("charm.status.is-set")
 
 
 @when("endpoint.lb-consumers.requests_changed")
 def get_lb():
     layer.status.maintenance("processing requests")
-    lb_consumers = endpoint_from_name("lb-consumers")
+    lb_consumers = allow_lb_consumers_to_read_requests()
     for request in lb_consumers.new_requests:
         response = request.response
         if not request.public:
             response.error = response.error_types.unsupported
             response.error_fields = {"public": "public only"}
         else:
             try:
```

### Comparing `loadbalancer_interface-1.1.1/loadbalancer_interface/base.py` & `loadbalancer_interface-1.2.0/loadbalancer_interface/base.py`

 * *Files identical despite different names*

### Comparing `loadbalancer_interface-1.1.1/loadbalancer_interface/pytest_plugin.py` & `loadbalancer_interface-1.2.0/loadbalancer_interface/pytest_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from contextlib import contextmanager
 from pathlib import Path
+import shutil
 
 import pytest
 
 
 try:
     from importlib.resources import path as resource_path
 except ImportError:
@@ -43,18 +44,24 @@
         self._lb_provider = None
         self._lb_consumer = None
         self._lb_provider_reactive = None
         self._lb_consumer_reactive = None
 
     def _render(self, charm_resource):
         with resource_path("loadbalancer_interface", "examples") as rp:
+            assert isinstance(self._lb_lib_url, Path)
+            if (rp / charm_resource / "charmcraft.yaml").exists():
+                shutil.copy2(self._lb_lib_url, rp / charm_resource)
+                lb_url = f"file:./{self._lb_lib_url.name}"
+            else:
+                lb_url = f"file://{self._lb_lib_url}#egg=loadbalancer_interface"
             return self._ops_test.render_charm(
                 rp / charm_resource,
                 include=["wheelhouse.txt", "requirements.txt"],
-                lb_lib_url=self._lb_lib_url,
+                lb_lib_url=lb_url,
             )
 
     @property
     def lb_provider(self):
         if self._lb_provider is None:
             self._lb_provider = self._render("lb-provider")
         return self._lb_provider
```

### Comparing `loadbalancer_interface-1.1.1/loadbalancer_interface/requires.py` & `loadbalancer_interface-1.2.0/loadbalancer_interface/requires.py`

 * *Files identical despite different names*

### Comparing `loadbalancer_interface-1.1.1/loadbalancer_interface/schemas/base.py` & `loadbalancer_interface-1.2.0/loadbalancer_interface/schemas/base.py`

 * *Files identical despite different names*

### Comparing `loadbalancer_interface-1.1.1/loadbalancer_interface/schemas/v1.py` & `loadbalancer_interface-1.2.0/loadbalancer_interface/schemas/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,16 @@
         if self._response is None:
             self._response = Response(self)
         return self._response
 
     @classmethod
     def loads(cls, request_sdata, response_sdata=None):
         self = cls()
-        self._update(json.loads(request_sdata))
+        if request_sdata:
+            self._update(json.loads(request_sdata))
         if response_sdata:
             self.response._update(json.loads(response_sdata))
         return self
 
     def add_health_check(self, **kwargs):
         """Create a HealthCheck and add it to the list."""
         health_check = HealthCheck()._update(kwargs)
```

### Comparing `loadbalancer_interface-1.1.1/loadbalancer_interface.egg-info/PKG-INFO` & `loadbalancer_interface-1.2.0/loadbalancer_interface.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,99 @@
 Metadata-Version: 2.1
 Name: loadbalancer-interface
-Version: 1.1.2
+Version: 1.2.0
 Summary: 'loadbalancer' interface protocol API library
 Home-page: https://github.com/juju-solutions/loadbalancer-interface
 Author: Cory Johns
 Author-email: cory.johns@canonical.com
 License: Apache License 2.0
-Description: # `loadbalancer` Interface Protocol API Library
-        
-        This library provides an API for requesting and providing load balancers or
-        ingress endpoints from one charm to another. It can be used in either charms
-        written in the newer [Operator Framework][] or older charms still using the
-        [charms.reactive Framework][].
-        
-        
-        ## Installation / Setup
-        
-        Include this library as a dependency for your charm, either in
-        `requirements.txt` for Operator Framework charms, or `wheelhouse.txt` for
-        reactive charms:
-        
-        ```
-        loadbalancer_interface
-        ```
-        
-        ## Usage
-        
-        ### Requesting Load Balancers
-        
-        Requesting a load balancer from a provider is done via the `LBProvider` class.
-        The general pattern for using the class is:
-        
-          * Wait for the provider to become available
-          * Get a `Request` object via the `get_request(name)` method
-          * Set the appropriate fields on the request object
-          * Send the `Request` via the `send_request(request)` method
-          * Wait for the `Response` to be provided (or updated)
-          * Get the `Response` object via either the `get_response(name)` method or
-            via the `new_responses` property
-          * Confirm that the request was successful and use the provided LB's address
-          * Acknowledge the `Response` via `ack_response(response)`
-        
-        There are examples in the repo for how to do this in [an operator charm][requires-operator]
-        or in [a reactive charm][requires-reactive].
-        
-        
-        ### Providing Load Balancers
-        
-        Providing a load balancer to consumers is done via the `LBConsumers` class.  The
-        general pattern for using the class is:
-        
-          * Wait for new or updated requests to come in
-          * Iterate over each request object in the `new_requests` property
-          * Create a load balancer according to the request's fields
-          * Set the appropriate fields on the request's `response` object
-          * Send the request's response via the `send_response(request)` method
-        
-        There are examples in the repo for how to do this in [an operator charm][provides-operator]
-        or in [a reactive charm][provides-reactive].
-        
-        ## API Reference
-        
-        See the [API docs][] for detailed reference on the API.
-        
-        ## Test Charms
-        
-        To ease testing of charms using this interface, this library provides test charms
-        which can be used with the pytest-operator plugin based integration test to
-        serve as a basic counterpart to the charm providing or requiring this interface.
-        
-        The charms are accessed via an `lb_charms` fixture, which is session scoped.
-        The fixture provides an object with attributes for each of the [example
-        charms][] available in the repo. (The attribute names will be the charm names
-        with dashes replaced with underscores.) For example:
-        
-        ```python
-        async def test_build_and_deploy(ops_test, lb_charms):
-            my_charm = await ops_test.build_charm(".")
-            lb_provider = await ops_test.build_charm(lb_charms.lb_provider)
-            await ops_test.model.deploy(my_charm)
-            await ops_test.model.deploy(lb_provider)
-            await ops_test.model.add_relation("my-charm", "lb-provider")
-        ```
-        
-        
-        <!-- Links -->
-        
-        [Operator Framework]: https://github.com/canonical/operator/
-        [charms.reactive Framework]: https://charmsreactive.readthedocs.io/
-        [requires-operator]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/requires-operator/
-        [requires-reactive]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/requires-reactive/
-        [provides-operator]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/provides-operator/
-        [provides-reactive]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/provides-reactive/
-        [API docs]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/docs/api.md
-        [example charms]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# `loadbalancer` Interface Protocol API Library
+
+This library provides an API for requesting and providing load balancers or
+ingress endpoints from one charm to another. It can be used in either charms
+written in the newer [Operator Framework][] or older charms still using the
+[charms.reactive Framework][].
+
+
+## Installation / Setup
+
+Include this library as a dependency for your charm, either in
+`requirements.txt` for Operator Framework charms, or `wheelhouse.txt` for
+reactive charms:
+
+```
+loadbalancer_interface
+```
+
+## Usage
+
+### Requesting Load Balancers
+
+Requesting a load balancer from a provider is done via the `LBProvider` class.
+The general pattern for using the class is:
+
+  * Wait for the provider to become available
+  * Get a `Request` object via the `get_request(name)` method
+  * Set the appropriate fields on the request object
+  * Send the `Request` via the `send_request(request)` method
+  * Wait for the `Response` to be provided (or updated)
+  * Get the `Response` object via either the `get_response(name)` method or
+    via the `new_responses` property
+  * Confirm that the request was successful and use the provided LB's address
+  * Acknowledge the `Response` via `ack_response(response)`
+
+There are examples in the repo for how to do this in [an operator charm][requires-operator]
+or in [a reactive charm][requires-reactive].
+
+
+### Providing Load Balancers
+
+Providing a load balancer to consumers is done via the `LBConsumers` class.  The
+general pattern for using the class is:
+
+  * Wait for new or updated requests to come in
+  * Iterate over each request object in the `new_requests` property
+  * Create a load balancer according to the request's fields
+  * Set the appropriate fields on the request's `response` object
+  * Send the request's response via the `send_response(request)` method
+
+There are examples in the repo for how to do this in [an operator charm][provides-operator]
+or in [a reactive charm][provides-reactive].
+
+## API Reference
+
+See the [API docs][] for detailed reference on the API.
+
+## Test Charms
+
+To ease testing of charms using this interface, this library provides test charms
+which can be used with the pytest-operator plugin based integration test to
+serve as a basic counterpart to the charm providing or requiring this interface.
+
+The charms are accessed via an `lb_charms` fixture, which is session scoped.
+The fixture provides an object with attributes for each of the [example
+charms][] available in the repo. (The attribute names will be the charm names
+with dashes replaced with underscores.) For example:
+
+```python
+async def test_build_and_deploy(ops_test, lb_charms):
+    my_charm = await ops_test.build_charm(".")
+    lb_provider = await ops_test.build_charm(lb_charms.lb_provider)
+    await ops_test.model.deploy(my_charm)
+    await ops_test.model.deploy(lb_provider)
+    await ops_test.model.add_relation("my-charm", "lb-provider")
+```
+
+
+<!-- Links -->
+
+[Operator Framework]: https://github.com/canonical/operator/
+[charms.reactive Framework]: https://charmsreactive.readthedocs.io/
+[requires-operator]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/requires-operator/
+[requires-reactive]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/requires-reactive/
+[provides-operator]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/provides-operator/
+[provides-reactive]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples/provides-reactive/
+[API docs]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/docs/api.md
+[example charms]: https://github.com/juju-solutions/loadbalancer-interface/blob/master/examples
```

### Comparing `loadbalancer_interface-1.1.1/loadbalancer_interface.egg-info/SOURCES.txt` & `loadbalancer_interface-1.2.0/loadbalancer_interface.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+LICENSE
 README.md
 setup.py
+examples/lb-consumer/charmcraft.yaml
 examples/lb-consumer/config.yaml
 examples/lb-consumer/metadata.yaml
 examples/lb-consumer/requirements.txt
 examples/lb-consumer-reactive/config.yaml
 examples/lb-consumer-reactive/layer.yaml
 examples/lb-consumer-reactive/metadata.yaml
 examples/lb-consumer-reactive/wheelhouse.txt
 examples/lb-consumer-reactive/reactive/charm.py
 examples/lb-consumer/src/charm.py
+examples/lb-provider/charmcraft.yaml
 examples/lb-provider/metadata.yaml
 examples/lb-provider/requirements.txt
 examples/lb-provider-reactive/layer.yaml
 examples/lb-provider-reactive/metadata.yaml
 examples/lb-provider-reactive/wheelhouse.txt
 examples/lb-provider-reactive/lib/charms/layer/provides_reactive.py
 examples/lb-provider-reactive/reactive/charm.py
@@ -26,8 +29,8 @@
 loadbalancer_interface.egg-info/SOURCES.txt
 loadbalancer_interface.egg-info/dependency_links.txt
 loadbalancer_interface.egg-info/entry_points.txt
 loadbalancer_interface.egg-info/requires.txt
 loadbalancer_interface.egg-info/top_level.txt
 loadbalancer_interface/schemas/__init__.py
 loadbalancer_interface/schemas/base.py
-loadbalancer_interface/schemas/v1.py
+loadbalancer_interface/schemas/v1.py
```

### Comparing `loadbalancer_interface-1.1.1/setup.py` & `loadbalancer_interface-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from shutil import rmtree
 
 
 SETUP = {
     "name": "loadbalancer_interface",
-    "version": "1.1.2",
+    "version": "1.2.0",
     "author": "Cory Johns",
     "author_email": "cory.johns@canonical.com",
     "url": "https://github.com/juju-solutions/loadbalancer-interface",
     "packages": [
         "loadbalancer_interface",
         "loadbalancer_interface.schemas",
         "loadbalancer_interface.examples",  # Synthetic package populated at build time
```

