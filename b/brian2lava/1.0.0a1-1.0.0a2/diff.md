# Comparing `tmp/Brian2Lava-1.0.0a1.tar.gz` & `tmp/brian2lava-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Brian2Lava-1.0.0a1.tar", last modified: Mon Mar 27 00:06:56 2023, max compression
+gzip compressed data, was "brian2lava-1.0.0a2.tar", last modified: Fri May 19 13:30:48 2023, max compression
```

## Comparing `Brian2Lava-1.0.0a1.tar` & `brian2lava-1.0.0a2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-27 00:06:56.506214 Brian2Lava-1.0.0a1/
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-27 00:06:56.502214 Brian2Lava-1.0.0a1/Brian2Lava.egg-info/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2495 2023-03-27 00:06:56.000000 Brian2Lava-1.0.0a1/Brian2Lava.egg-info/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1692 2023-03-27 00:06:56.000000 Brian2Lava-1.0.0a1/Brian2Lava.egg-info/SOURCES.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-03-27 00:06:56.000000 Brian2Lava-1.0.0a1/Brian2Lava.egg-info/dependency_links.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      115 2023-03-27 00:06:56.000000 Brian2Lava-1.0.0a1/Brian2Lava.egg-info/requires.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       11 2023-03-27 00:06:56.000000 Brian2Lava-1.0.0a1/Brian2Lava.egg-info/top_level.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       80 2023-03-26 23:21:40.000000 Brian2Lava-1.0.0a1/MANIFEST.in
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2495 2023-03-27 00:06:56.506214 Brian2Lava-1.0.0a1/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1692 2023-03-26 08:53:24.000000 Brian2Lava-1.0.0a1/README.md
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-27 00:06:56.502214 Brian2Lava-1.0.0a1/brian2lava/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       47 2023-03-26 23:03:39.000000 Brian2Lava-1.0.0a1/brian2lava/__init__.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-27 00:06:56.502214 Brian2Lava-1.0.0a1/brian2lava/codegen/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     5722 2023-03-26 23:36:06.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/codeobject.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    24541 2023-03-26 08:26:50.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/lava_generator.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     3479 2023-03-26 23:38:15.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templater.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-27 00:06:56.506214 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1270 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/activation_processing.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      743 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/common_group.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      436 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/group_get_indices.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      633 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/group_variable_get.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      553 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/group_variable_get_conditional.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      550 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/group_variable_set.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1677 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/group_variable_set_conditional.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      537 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/ratemonitor.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      521 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/reset.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     7522 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/spatialstateupdate.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1179 2023-03-26 07:47:47.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/spikegenerator.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/spikemonitor.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)        1 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/statemonitor.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      419 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/stateupdate.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1183 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/summed_variable.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1452 2023-03-26 07:47:47.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/synapses.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1713 2023-03-26 21:28:29.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/synapses_create_array.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     9781 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/synapses_create_generator.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      524 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/synapses_push_spikes.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1672 2023-03-26 07:47:47.000000 Brian2Lava-1.0.0a1/brian2lava/codegen/templates/threshold.py_
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-27 00:06:56.506214 Brian2Lava-1.0.0a1/brian2lava/device/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6582 2023-03-26 23:26:05.000000 Brian2Lava-1.0.0a1/brian2lava/device/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2288 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/device/activate.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    12069 2023-03-26 07:47:47.000000 Brian2Lava-1.0.0a1/brian2lava/device/arrays.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    24793 2023-03-26 23:39:12.000000 Brian2Lava-1.0.0a1/brian2lava/device/build.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6838 2023-03-26 08:03:28.000000 Brian2Lava-1.0.0a1/brian2lava/device/codeobject.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    20208 2023-03-26 12:55:53.000000 Brian2Lava-1.0.0a1/brian2lava/device/run.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8638 2023-03-26 23:40:12.000000 Brian2Lava-1.0.0a1/brian2lava/device/synapses.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6891 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/device/variables.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1617 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/device/writer.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-27 00:06:56.506214 Brian2Lava-1.0.0a1/brian2lava/templates/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      935 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/templates/process.py.j2
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1405 2023-03-26 07:47:47.000000 Brian2Lava-1.0.0a1/brian2lava/templates/process_model.py.j2
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-27 00:06:56.506214 Brian2Lava-1.0.0a1/brian2lava/writer/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1369 2023-03-14 08:59:44.000000 Brian2Lava-1.0.0a1/brian2lava/writer/py.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-03-27 00:06:56.506214 Brian2Lava-1.0.0a1/setup.cfg
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1017 2023-03-27 00:06:49.000000 Brian2Lava-1.0.0a1/setup.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       80 2023-03-26 23:21:40.000000 brian2lava-1.0.0a2/MANIFEST.in
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2178 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1423 2023-05-19 13:30:09.000000 brian2lava-1.0.0a2/README.md
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.818439 brian2lava-1.0.0a2/brian2lava/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       47 2023-05-15 08:19:12.000000 brian2lava-1.0.0a2/brian2lava/__init__.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.818439 brian2lava-1.0.0a2/brian2lava/codegen/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     5722 2023-03-26 23:36:06.000000 brian2lava-1.0.0a2/brian2lava/codegen/codeobject.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    35555 2023-05-19 09:41:04.000000 brian2lava-1.0.0a2/brian2lava/codegen/lava_generator.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3479 2023-03-26 23:38:15.000000 brian2lava-1.0.0a2/brian2lava/codegen/templater.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.822439 brian2lava-1.0.0a2/brian2lava/codegen/templates/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1058 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/activation_processing.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      731 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/common_group.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      436 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/group_get_indices.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      633 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_get.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      553 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_get_conditional.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      512 2023-04-15 20:02:40.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_set.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1760 2023-04-15 20:02:40.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_set_conditional.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      537 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/ratemonitor.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      521 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/reset.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     7522 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/spatialstateupdate.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1179 2023-03-26 07:47:47.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/spikegenerator.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/spikemonitor.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)        1 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/statemonitor.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      419 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/stateupdate.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1305 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/summed_variable.py_
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1213 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1713 2023-03-26 21:28:29.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_create_array.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)    11153 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_create_generator.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      524 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_push_spikes.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1860 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_transmit.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1672 2023-03-26 07:47:47.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/threshold.py_
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/brian2lava/device/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     6977 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/device/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3090 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/device/activate.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    16121 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/device/arrays.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    23642 2023-05-19 09:41:04.000000 brian2lava-1.0.0a2/brian2lava/device/build.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3332 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/device/codeobject.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    25580 2023-05-19 09:41:04.000000 brian2lava-1.0.0a2/brian2lava/device/run.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    10616 2023-05-19 09:41:04.000000 brian2lava-1.0.0a2/brian2lava/device/synapses.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7050 2023-04-15 20:02:40.000000 brian2lava-1.0.0a2/brian2lava/device/variables.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1618 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/device/writer.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/brian2lava/templates/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      929 2023-04-15 20:02:40.000000 brian2lava-1.0.0a2/brian2lava/templates/process.py.j2
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1338 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/templates/process_model.py.j2
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/brian2lava/writer/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1369 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/writer/py.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.818439 brian2lava-1.0.0a2/brian2lava.egg-info/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2178 2023-05-19 13:30:48.000000 brian2lava-1.0.0a2/brian2lava.egg-info/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1743 2023-05-19 13:30:48.000000 brian2lava-1.0.0a2/brian2lava.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-05-19 13:30:48.000000 brian2lava-1.0.0a2/brian2lava.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      107 2023-05-19 13:30:48.000000 brian2lava-1.0.0a2/brian2lava.egg-info/requires.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       11 2023-05-19 13:30:48.000000 brian2lava-1.0.0a2/brian2lava.egg-info/top_level.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/setup.cfg
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1009 2023-05-19 13:28:48.000000 brian2lava-1.0.0a2/setup.py
```

### Comparing `Brian2Lava-1.0.0a1/Brian2Lava.egg-info/PKG-INFO` & `brian2lava-1.0.0a2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Brian2Lava
-Version: 1.0.0a1
+Name: brian2lava
+Version: 1.0.0a2
 Summary: An open source Brian2 interface for the neuromorphic computing framework Lava
 Home-page: https://gitlab.com/tetzlab/brian2lava
 Author: Carlo Michaelis, Francesco Negri, Winfried Oed, Jannik Luboeinski, Andrew Lehr, Tristan Stöber
 Author-email: carlo.michaelis@gmail.com
 License: MIT
 Description: # Brian2Lava
         
@@ -15,20 +15,14 @@
         
         * [Website](https://brian2lava.gitlab.io/)
         * [Documentation](https://brian2lava.gitlab.io/docs)
         ## Installation
         
         Brian2Lava currently supports Lava with `CPU` backend. We’re working on `Loihi` support. Please feel free to test Brian2Lava and report issues.
         
-        `Brian2Lava` requires that `Lava` is installed. Since `Lava` is currently not available on `pypi.org`, you need to install it from the the `Lava` GitHub repository via:
-        
-        ```
-        pip install https://github.com/lava-nc/lava/releases/download/v0.6.0/lava_nc-0.6.0.tar.gz
-        ```
-        
         The installation of `Brian2Lava` is provided via the the Python Package Index (`pip`):
         
         ```
         pip install brian2lava
         ```
         
         Note: perhaps also `conda` will be supported later.
```

### Comparing `Brian2Lava-1.0.0a1/Brian2Lava.egg-info/SOURCES.txt` & `brian2lava-1.0.0a2/brian2lava.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 MANIFEST.in
 README.md
 setup.py
-Brian2Lava.egg-info/PKG-INFO
-Brian2Lava.egg-info/SOURCES.txt
-Brian2Lava.egg-info/dependency_links.txt
-Brian2Lava.egg-info/requires.txt
-Brian2Lava.egg-info/top_level.txt
 brian2lava/__init__.py
+brian2lava.egg-info/PKG-INFO
+brian2lava.egg-info/SOURCES.txt
+brian2lava.egg-info/dependency_links.txt
+brian2lava.egg-info/requires.txt
+brian2lava.egg-info/top_level.txt
 brian2lava/codegen/codeobject.py
 brian2lava/codegen/lava_generator.py
 brian2lava/codegen/templater.py
 brian2lava/codegen/templates/activation_processing.py_
 brian2lava/codegen/templates/common_group.py_
 brian2lava/codegen/templates/group_get_indices.py_
 brian2lava/codegen/templates/group_variable_get.py_
@@ -25,14 +25,15 @@
 brian2lava/codegen/templates/statemonitor.py_
 brian2lava/codegen/templates/stateupdate.py_
 brian2lava/codegen/templates/summed_variable.py_
 brian2lava/codegen/templates/synapses.py_
 brian2lava/codegen/templates/synapses_create_array.py_
 brian2lava/codegen/templates/synapses_create_generator.py_
 brian2lava/codegen/templates/synapses_push_spikes.py_
+brian2lava/codegen/templates/synapses_transmit.py_
 brian2lava/codegen/templates/threshold.py_
 brian2lava/device/__init__.py
 brian2lava/device/activate.py
 brian2lava/device/arrays.py
 brian2lava/device/build.py
 brian2lava/device/codeobject.py
 brian2lava/device/run.py
```

### Comparing `Brian2Lava-1.0.0a1/PKG-INFO` & `brian2lava-1.0.0a2/brian2lava.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Brian2Lava
-Version: 1.0.0a1
+Name: brian2lava
+Version: 1.0.0a2
 Summary: An open source Brian2 interface for the neuromorphic computing framework Lava
 Home-page: https://gitlab.com/tetzlab/brian2lava
 Author: Carlo Michaelis, Francesco Negri, Winfried Oed, Jannik Luboeinski, Andrew Lehr, Tristan Stöber
 Author-email: carlo.michaelis@gmail.com
 License: MIT
 Description: # Brian2Lava
         
@@ -15,20 +15,14 @@
         
         * [Website](https://brian2lava.gitlab.io/)
         * [Documentation](https://brian2lava.gitlab.io/docs)
         ## Installation
         
         Brian2Lava currently supports Lava with `CPU` backend. We’re working on `Loihi` support. Please feel free to test Brian2Lava and report issues.
         
-        `Brian2Lava` requires that `Lava` is installed. Since `Lava` is currently not available on `pypi.org`, you need to install it from the the `Lava` GitHub repository via:
-        
-        ```
-        pip install https://github.com/lava-nc/lava/releases/download/v0.6.0/lava_nc-0.6.0.tar.gz
-        ```
-        
         The installation of `Brian2Lava` is provided via the the Python Package Index (`pip`):
         
         ```
         pip install brian2lava
         ```
         
         Note: perhaps also `conda` will be supported later.
```

### Comparing `Brian2Lava-1.0.0a1/README.md` & `brian2lava-1.0.0a2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,20 +7,14 @@
 
 * [Website](https://brian2lava.gitlab.io/)
 * [Documentation](https://brian2lava.gitlab.io/docs)
 ## Installation
 
 Brian2Lava currently supports Lava with `CPU` backend. We’re working on `Loihi` support. Please feel free to test Brian2Lava and report issues.
 
-`Brian2Lava` requires that `Lava` is installed. Since `Lava` is currently not available on `pypi.org`, you need to install it from the the `Lava` GitHub repository via:
-
-```
-pip install https://github.com/lava-nc/lava/releases/download/v0.6.0/lava_nc-0.6.0.tar.gz
-```
-
 The installation of `Brian2Lava` is provided via the the Python Package Index (`pip`):
 
 ```
 pip install brian2lava
 ```
 
 Note: perhaps also `conda` will be supported later.
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/codeobject.py` & `brian2lava-1.0.0a2/brian2lava/codegen/codeobject.py`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/lava_generator.py` & `brian2lava-1.0.0a2/brian2lava/codegen/lava_generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from brian2.parsing.rendering import NumpyNodeRenderer
 from brian2.core.functions import DEFAULT_FUNCTIONS, timestep
 from brian2.core.variables import Constant, ArrayVariable
 from brian2.utils.stringtools import get_identifiers, word_substitute, indent
 from brian2.utils.logger import get_logger
 from brian2.core.functions import Function
 from brian2.groups.neurongroup import NeuronGroup
+from brian2.units.unitsafefunctions import exprel
 
 from brian2.codegen.generators.base import CodeGenerator
 
 
 # TODO remove, only for development
 from pprint import pprint
 
@@ -44,15 +45,15 @@
     # Define some class variables
     class_name = 'lava'
     _use_ufunc_at_vectorisation = True  # allow this to be off for testing only
 
 
     def translate_expression(self, expr):
         """
-        TODO
+        Translate an abstract code expression to the right of an operator to Python code.
         """
 
         expr = word_substitute(expr, self.func_name_replacements)
         translated_expr = NumpyNodeRenderer(auto_vectorise=self.auto_vectorise).render_expr(expr, self.variables).strip()
         return translated_expr
 
 
@@ -229,15 +230,15 @@
                     lines.append(indent(f'if {conditional_write_vars[statement.var]}:'))
                     lines.append(indent(line, 2))
                 else:
                     lines.append(indent(line))
             lines.extend(indent(code) for code in
                          self.write_arrays(statements, read, write,
                                            variables, variable_indices))
-        
+            
         return lines
 
 
     @staticmethod
     def get_array_name(var, access_data=True, template_name=None):
         """
         Returns a variable name used in the template
@@ -409,14 +410,22 @@
             Jinja variables containing compiled *scalar* code.
         vector_code : `dict`
             Jinja variables containing compiled *vector* code.
         kwds : `dict`
             Jinja variables containing additional custom variables (so called 'keywords').
         """
 
+        # If we're dealing with synapses, we buffer the translation and manage their two functions separately
+        if self.template_name == 'synapses':
+            # Get the statements which are only related to synapses (the neuronal part of transmission is handled by another template)
+            scalar_statements,vector_statements = self.manage_neuron_activations(scalar_statements,vector_statements)
+
+            # Use these statements to manage synaptic transmission
+            self.manage_synaptic_behavior(scalar_statements,vector_statements)
+            
         scalar_code = {}
         vector_code = {}
         for name, block in scalar_statements.items():
             scalar_code[name] = self.translate_one_statement_sequence(
                 block, scalar=True
             )
         for name, block in vector_statements.items():
@@ -441,139 +450,317 @@
             Indicates if the statements shall be scalar or vectorized.
 
         Returns
         -------
         lines : `str[]`
             List of compiled code lines.
         """
+        # For synapses learning, we want to add a # EMPTY_CODE_BLOCK indicator when
+        # the vector learning statements are empty. This means that the codeobject will not be compiled.
+        if self.template_name == 'synapses' and len(statements) == 0 and not scalar:
+            return ['# EMPTY_CODE_BLOCK']
 
         variables = self.variables
         variable_indices = self.variable_indices
+
         read, write, indices, conditional_write_vars = self.arrays_helper(statements)
         lines = []
         all_unique = not self.has_repeated_indices(statements)
-        self.check_for_learning_statements(statements)
         if scalar or all_unique:
             # Simple translation
             lines.extend(self.read_arrays(read, write, indices, variables, variable_indices))
             created_vars = {stmt.var for stmt in statements if stmt.op == ':='}
             for stmt in statements:
                 line = self.translate_statement(stmt)
                 line = self.conditional_write(line, stmt, variables, conditional_write_vars, created_vars)
                 lines.append(line)
             lines.extend(self.write_arrays(statements, read, write, variables, variable_indices))
         else:
             # More complex translation to deal with repeated indices
             lines.extend(self.vectorise_code(statements, variables, variable_indices))
+        
+        # TODO: There might be a better way to add this..
+        # We treat the case of int() calls in a special way since importing
+        # the numpy.int32 function as int() would overwrite the Python int type
+        tmp = []
+        for line in lines:
+            if 'int(' in line:
+                line = line.replace('int(', '_numpy.int32(')
+            tmp.append(line)
+        lines = tmp
 
         return lines
 
 
-    def check_for_learning_statements(self, statements):
+    def manage_neuron_activations(self, scalar_statements, vector_statements):
         """
-        A method to look for learning statements and implement learning rules in the way of lava
+        Manages the transmission of synaptic variables to neurons and creates a code object to handle
+        the effect of synaptic transmission on neurons.
+        NOTE: This method strongly relies on the device, but also on the variables stored in the generator
+        so we have to choose whether this method should be used by the LavaGenerator or by the device itself..
 
         Parameters
         ----------
-        statements
-            Statements containing the corresponding variable, operation, expression and comment.
+        statements: list(Statement) 
+            A list of the statements search through for statemtents related to synaptic transmission
+
+        Returns:
+        --------
+        synapse_statements: list(Statement)
+            A list of the statements which are purely internal to synapses, i.e. statements related to 
+            learning rules. These statements are then processed by the usual pipeline.
+        """
+
+        from brian2 import get_device
+        device = get_device()
+        # The pathway will have been stored by the device at this point (see device.codeobject())
+        pathway = device._pathway
+
+        # Collect scalar and vector statements related to synapses
+        synapse_scalar_statements = {name:[] for name in scalar_statements}
+        synapse_vector_statements = {name:[] for name in vector_statements}
+
+        # Collect scalar and vector statements related to neurons
+        neuron_scalar_statements = {name:[] for name in scalar_statements}
+        neuron_vector_statements = {name:[] for name in vector_statements}
+
+        # Also copy the needed variables (having some extra ones is not a problem)
+        neuron_statement_variables = self.variables
+        neuron_created_vars = []
+        # For the next part we don't need to distinguish between statement types
+        all_statements = list(itertools.chain.from_iterable(scalar_statements.values())) + list(itertools.chain.from_iterable(vector_statements.values()))
+        # Check stmt.var is a created var. If it is, check if there is another stmt in which the var belongs to a neuron
+        # and the stmt.expr identifiers (you get them from get_identifiers(stmt.expr)) contain the created stmt.var. If so append the original var to neuron_created_vars
+        created_vars = {stmt.var for stmt in all_statements if stmt.op == ':='}
+        for stmt in all_statements:
+            if stmt.var in created_vars:
+                for other_stmt in all_statements:
+                    if other_stmt.var not in created_vars and isinstance(self.variables[other_stmt.var].owner,NeuronGroup):
+                        identifiers = get_identifiers(other_stmt.expr)
+                        if stmt.var in identifiers:
+                            neuron_created_vars.append(stmt.var)
+                            break
+
+        # We have to deal with both scalar and vector statements (even though in most cases scalar statements are empty)
+        for name, block in scalar_statements.items():
+            # This potentially is useless, but keep it for now.
+            created_vars = {stmt.var for stmt in block if stmt.op == ':='}
+            for stmt in block:
+                if stmt.var in created_vars:
+                    if stmt.var in neuron_created_vars:
+                        # Make the operator a simple '=' since the := operator is not recognized by the 
+                        # brian parser.
+                        stmt.op = '='
+                        neuron_scalar_statements[name].append(stmt)
+                    continue
+                var = self.variables[stmt.var]
+                if isinstance(var.owner,NeuronGroup):
+                    neuron_scalar_statements[name].append(stmt)
+                    continue
+                synapse_scalar_statements[name].append(stmt)
+            
+        
+        for name, block in vector_statements.items():
+            # Collecting all of the created vars.
+            created_vars = {stmt.var for stmt in block if stmt.op == ':='}
+            for stmt in block:
+                # Again the created vars are added to the statements if they are used by the neuron statements
+                if stmt.var in created_vars:
+                    if stmt.var in neuron_created_vars:
+                        stmt.op = '='
+                        neuron_vector_statements[name].append(stmt)
+                    continue
+                var = self.variables[stmt.var]
+                if isinstance(var.owner,NeuronGroup):
+                    neuron_vector_statements[name].append(stmt)
+                    continue
+                synapse_vector_statements[name].append(stmt)
+        
+
+        # Store the requirements for the synaptic connections in Lava
+        device.determine_lava_ports(pathway,neuron_statement_variables)
+        
+        # Create the 'activation_processing' codeobject handling synaptic effects on neurons
+        all_neuron_statements = [statement for block in neuron_scalar_statements.values() for statement in block]
+        all_neuron_statements += [statement for block in neuron_vector_statements.values() for statement in block]
+        
+        code_str = '\n'.join([stmt.var+stmt.op+str(stmt.expr) for stmt in all_neuron_statements])
+        abstract_code = {None: code_str}
+
+        codeobj_name = pathway.target.name +'_'+ self.owner.name + '_' + pathway.prepost + '_' + 'activation_processing'
+        # TODO: Check whether this kwd is actually required or not, for now I'll stay on the safe side
+        kwds = {'pathway': pathway}
+        # TODO: Figure out if it's better to use this function or 'create_runner_object()'
+        device.code_object(
+            owner= pathway.target,
+            name = codeobj_name,
+            abstract_code = abstract_code,
+            variables = neuron_statement_variables,
+            template_name = 'activation_processing',
+            variable_indices = self.variable_indices,
+            template_kwds=kwds,
+            override_conditional_write=self.override_conditional_write
+        )
+
+        return synapse_scalar_statements,synapse_vector_statements
+
+
+    def manage_synaptic_behavior(self, scalar_statements, vector_statements):
+        """
+        This method manages the two main code objects related to synaptic behavior: synapses_transmit and synapses.
+
+        Parameters
+        ----------
+        synapses_transmit:
+            handles the signal transmission of the selected variables along the pathway (pre->post or post->pre).
+            This code object is created by the device.
+        synapses:
+            handles the learning rules and the synaptic plasticity.
+            The code object is created by the LavaGenerator by following the usual pipeline.
+            Here we only check if the learning rules defined by the user are valid.
         """
 
-        # For release this is just going to throw an error, as learning is not implemented yet
-        for stmt in statements:
-            if self.template_name == 'activation_processing' and not isinstance(self.variables[stmt.var].owner,NeuronGroup):
-                msg = f""" In the current release learning is not supported yet: the 'on_pre' and 'on_post' conditions
-                can only be used to update variables belonging to NeuronGroups. (e.g. on_pre = 'v+=w' or similar).
-                The following expression is not allowed: {stmt}
+        vars_from_expr = []
+        # TODO: This here is not good, we'll have to figure out a proper way to do this
+        from brian2 import Clock, get_device
+        device = get_device()
+        accepted_owners = [type(None),Clock, type(self.owner)]
+        # Group all the statements in one variable
+        all_statements = scalar_statements.copy()
+        all_statements.update(vector_statements.copy())
+
+        # Go through all the statements and check if the variables are local to the synapses object
+        for statements in all_statements.values():
+            created_vars = {stmt.var for stmt in statements if stmt.op == ':='}
+            for stmt in statements:
+                # Again skip created_vars since they're an exception
+                if stmt.var in created_vars:
+                    continue
+                if hasattr(self.variables[stmt.var],'owner') and not self.variables[stmt.var].owner == self.owner:
+                    raise ValueError(f"The variable in this learning statement does not belong to synapses: {stmt}") 
+                vars_to_append = [self.variables[id] for id in get_identifiers(stmt.expr) if not id in created_vars and hasattr(self.variables[id],'owner')]
+                vars_from_expr = itertools.chain(vars_from_expr,vars_to_append)
+
+        for var in vars_from_expr:
+            cond = any([isinstance(var.owner, obj) for obj in accepted_owners])
+            if  not cond:
+                msg = f"""Learning rules requiring variables which are not strictly local to synapses is currently not supported.
+                Define all variables required for learning inside the Synapses object or as constants. The var {var.name} belongs to {var.owner}
+                and not to {self.owner}
                 """
-                raise NotImplementedError(msg)
+                raise ValueError(msg)
+
+        # Generate the codeobject needed for synaptic transmission. It doesn't need any code as the functionality is included in the template.
+        prepost = 'pre' if 'pre' in self.name else 'post'
+        codeobj_name = f'{self.owner.name}_{prepost}_synapses_transmit'
+        device.code_object(
+            owner= self.owner,
+            name = codeobj_name,
+            abstract_code = {None: ''},
+            variables = self.variables,
+            template_name = 'synapses_transmit',
+            variable_indices = self.variable_indices,
+            template_kwds={'pathway': device._pathway},
+            override_conditional_write=self.override_conditional_write
+        )
 
 
     def determine_keywords(self):
         """
         Adds custom variables to the Jinja templates
         """
 
         from brian2 import get_device
         device = get_device()
+        # Keywords dictionary, by default it only contains the name of the method.
+        kwds = {'name': self.name}
 
         # Add constants to template keywords
         # TODO Francesco: I'm wondering if this is the correct way to add the 'USES_VARIABLES' from templates
         # check: https://github.com/brian-team/brian2/blob/3cf65d4c5c8fa1512cf0a6deb515a8cdc81ae9e5/brian2/codegen/templates.py (186-217)
         # It seems that the templates themselves should take care of this. Further investigation is needed.
         constants = []
-        for var in self.variables.values():
+        for varname,var in self.variables.items():
             if isinstance(var, Constant):
-                constants.append(f'{var.name} = {var.get_value()}')
-            elif isinstance(var, ArrayVariable) and var.constant:
-                constants.append(f'{var.name} = {device.get_array_name(var)}[0]')
-        read_syn_vars = []
-        syn_output_vars = []
-        syn_output_ports = []
+                constants.append(f'{varname} = {var.get_value()}')
+            elif isinstance(var, ArrayVariable) and var.constant and var.owner == self.owner:
+                # TODO This has to be handled differently. For the moment we just avoid adding these to the template constants.
+                if self.template_name == 'synapses_create_generator' and (varname == '_synaptic_pre' or varname == '_synaptic_post'):
+                    continue 
+                constants.append(f'{varname} = {self.get_array_name(var,template_name=self.template_name)}[0]')
+            kwds['constants'] = constants
+
+        if 'synapses' in self.owner.name:
+            # This is only needed for the templates related to pathways
+            if self.template_name == 'synapses' or self.template_name == 'synapses_transmit':
+                # TODO: there might be a better way to access this value
+                prepost = 'pre' if 'pre' in self.name else 'post'
+                kwds['prepost'] = prepost
+                kwds['spiking_synapses'] = self.get_array_name(self.owner.variables[f"lava_spiking_synapses_{prepost}"])
 
         # Read the required synaptic variables which are to be sent to neurons
         # and send them out through the correct port.
-        if self.template_name == 'synapses':            
+        if self.template_name == 'synapses_transmit':  
+            read_syn_vars = []
+            syn_output_vars = []
+            syn_output_ports = []          
             ports = device.lava_ports
             for port in ports.values():
                 if not port['pathway'].synapses == self.owner or not port['varname'] in list(self.variables.keys()) or port['pathway'].prepost not in self.name:
                     continue
                 varname = port['varname']
                 lava_name = device.get_array_name(self.owner.variables[varname])
                 # Not sure about this
                 _idx = self.variable_indices[varname]
                 read_syn_vars.append(f'{varname} = {lava_name}[{_idx}]')
                 syn_output_vars.append(varname)
                 syn_output_ports.append(port['portname'])
+            kwds['read_syn_vars'] = read_syn_vars
+            kwds['syn_output_vars'] = syn_output_vars
+            kwds['syn_output_ports'] = syn_output_ports
+            kwds['zip'] = zip
 
         # Receive the input from the synapses
-        read_port_input = []
-        neur_input_vars = []
         if self.template_name == 'activation_processing':
-            from brian2 import get_device
-            device = get_device()
+            read_port_input = []
+            neur_input_vars = []
             ports = device.lava_ports
             for port in ports.values():
-                if not port['receiver'] == self.owner.name or not port['varname'] in list(self.variables.keys()):
+                if not port['pathway'] == device._pathway or not port['varname'] in list(self.variables.keys()):
                     continue
                 varname = port['varname'] + '_received'
                 portname = port['portname']
                 # Not sure about this
                 read_port_input.append(f'{varname} = self.{portname}_in.recv()')
                 neur_input_vars.append(varname)
+            kwds['neur_input_vars'] = neur_input_vars
+            kwds['read_port_input'] = read_port_input
 
         # Determine if scipy is available
         try:
             import scipy
             scipy_available = True
         except ImportError:
             scipy_available = False
+        kwds['_scipy_available'] = scipy_available
 
         # Collect template keywords and return
-        return {
-            '_scipy_available': scipy_available,
-            'constants': constants,
-            'read_port_input': read_port_input,
-            'neur_input_vars': neur_input_vars,
-            'syn_output_vars': syn_output_vars,
-            'syn_output_ports': syn_output_ports,
-            'read_syn_vars': read_syn_vars,
-            'zip': zip
-        }
+        return kwds
 
 
 # Functions that exist under the same name in numpy
 for func_name, func in [
     ('sin', np.sin), ('cos', np.cos), ('tan', np.tan), ('sinh', np.sinh),
     ('cosh', np.cosh), ('tanh', np.tanh), ('exp', np.exp), ('log', np.log),
     ('log10', np.log10), ('sqrt', np.sqrt), ('arcsin', np.arcsin),
     ('arccos', np.arccos), ('arctan', np.arctan), ('abs', np.abs), ('sign', np.sign)
 ]:
     DEFAULT_FUNCTIONS[func_name].implementations.add_implementation(LavaCodeGenerator, code=func)
 
+
 # Functions that are implemented in a somewhat special way
 def randn_func(vectorisation_idx):
     try:
         N = len(vectorisation_idx)
         return np.random.randn(N)
     except TypeError:
         # scalar value
@@ -593,25 +780,27 @@
     try:
         N = len(vectorisation_idx)
         return np.random.poisson(lam, size=N)
     except TypeError:
         # scalar value
         return np.random.poisson(lam)
 
-
+# NOTE: At the moment we are not really using these in any way and are instead importing the related functions
+# in the process and processmodel scripts. Maybe there is a way to automatically generate imports from these..
 DEFAULT_FUNCTIONS['randn'].implementations.add_implementation(LavaCodeGenerator, code=randn_func)
 DEFAULT_FUNCTIONS['rand'].implementations.add_implementation(LavaCodeGenerator, code=rand_func)
 DEFAULT_FUNCTIONS['poisson'].implementations.add_implementation(LavaCodeGenerator, code=poisson_func)
 clip_func = lambda array, a_min, a_max: np.clip(array, a_min, a_max)
 DEFAULT_FUNCTIONS['clip'].implementations.add_implementation(LavaCodeGenerator, code=clip_func)
 int_func = lambda value: np.int32(value)
 DEFAULT_FUNCTIONS['int'].implementations.add_implementation(LavaCodeGenerator, code=int_func)
 ceil_func = lambda value: np.int32(np.ceil(value))
 DEFAULT_FUNCTIONS['ceil'].implementations.add_implementation(LavaCodeGenerator, code=ceil_func)
 floor_func = lambda value: np.int32(np.floor(value))
 DEFAULT_FUNCTIONS['floor'].implementations.add_implementation(LavaCodeGenerator, code=floor_func)
+DEFAULT_FUNCTIONS['exprel'].implementations.add_implementation(LavaCodeGenerator,code = exprel)
 
 # We need to explicitly add an implementation for the timestep function,
 # otherwise Brian would *add* units during simulation, thinking that the
 # timestep function would not work correctly otherwise. This would slow the
 # function down significantly.
 DEFAULT_FUNCTIONS['timestep'].implementations.add_implementation(LavaCodeGenerator, code=timestep)
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templater.py` & `brian2lava-1.0.0a2/brian2lava/codegen/templater.py`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/activation_processing.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/activation_processing.py_`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 {# USES_VARIABLES {N} #}
 {% extends 'common_group.py_' %}
 
 {% block maincode %}
+
+    # constants
+    {% for c in constants %}
+    {{ c }}
+    {% endfor%}
+
     # Collect all the incoming variables from the synapses
     # We could have multiple inputs depending on the synaptic model:
     # e.g. if we have v += w + g*I and both w and g are synaptic variables, but I is a neuronal variable.
     # This allows for more generalizable models. 
     # TODO: handle the case in which no neuronal variable is on the right of the equation (i.e. just send the result of the operation).
     {% for var in read_port_input %}
     {{var}}
     {% endfor %}
 
-    # We assume there is always one InPort in the NeuronGroup 
-    # TODO: The next line takes care of the case in which an 'int' or 'bool' port is at index zero of neur_input_vars
-    # np.nan gets translated to this number, so we convert it back. Probably in future implementations we can avoid this.
-    _activation_indices = np.where({{neur_input_vars[0]}} == -9223372036854775808,_numpy.nan,{{neur_input_vars[0]}})[0]
-    _activation_indices = np.where(~_numpy.isnan({{neur_input_vars[0]}}))[0]
+    # We assume there is always one InPort in the NeuronGroup
+    # To check which indices to use we check for our "nan equivalent": {{nan}}
+    _activation_indices = np.where({{neur_input_vars[0]}}!= {{nan}})[0]
 
     # scalar code
     _vectorisation_idx = 1
     {{scalar_code|autoindent}}
 
     # vector code
     _idx = _activation_indices
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/common_group.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/common_group.py_`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 {% macro before_run() %}
 def {{name}}_before_run(self):
     import numpy as _numpy
     from brian2.codegen.runtime.numpy_rt.numpy_rt import LazyArange
     {% block before_code %}
     # EMPTY_CODE_BLOCK  -- overwrite in child template
     {% endblock %}
-    {% endmacro %}
+{% endmacro %}
 
 {% macro run() %}
 def {{name}}_run(self):
     import numpy as _numpy
     from brian2.codegen.runtime.numpy_rt.numpy_rt import LazyArange
     {% block maincode %}
     {% endblock %}
-    {% endmacro %}
+{% endmacro %}
 
 {% macro after_run() %}
 def {{name}}_after_run(self):
     import numpy as _numpy
     from brian2.codegen.runtime.numpy_rt.numpy_rt import LazyArange
     {% block after_code %}
     # EMPTY_CODE_BLOCK  -- overwrite in child template
     {% endblock %}
-    {% endmacro %}
+{% endmacro %}
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/group_variable_get.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_get.py_`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/group_variable_get_conditional.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_get_conditional.py_`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/group_variable_set.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_set.py_`

 * *Files 15% similar despite different names*

```diff
@@ -18,11 +18,9 @@
 
     # Vector code
     _idx = {{_group_idx}}
     _target_idx = slice(None)
     _vectorisation_idx = _idx
     {{vector_code|autoindent}}
 
-    # Return
-    {{return_statement}}
 
     {% endblock %}
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/group_variable_set_conditional.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_set_conditional.py_`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
     {# USES_VARIABLES { N } #}
     {# ALLOWS_SCALAR_WRITE #}
     {% extends 'common_group.py_' %}
 
     {% block maincode %}
+    # Constants
+    {% for c in constants %}
+    {{ c }}
+    {% endfor%}
     numpy_False = _numpy.bool_(False)
     numpy_True = _numpy.bool_(True)
 
     # Phase 1: we compute the indices where the conditional setting is to
     # be applied, and to do this we want to vectorise over all the values,
     # but we don't want to do the iterate all protocol, so we explicitly
     # set the idx to be slice(None)
     # scalar code
     _vectorisation_idx = 1
     {{scalar_code['condition']|autoindent}}
 
     # vector code
     _idx = slice(None)
-    _vectorisation_idx = LazyArange({{constant_or_scalar('N', variables['N'])}})
+    # Assume that N was defined in constants before
+    _vectorisation_idx = LazyArange(N)
     {{vector_code['condition']|autoindent}}
 
     # Phase 2: having computed _cond, the boolean array of points where
     # the setting is to be applied, we want to vectorise over idx being
     # only these values.
 
     {# Note that we don't write to scalar variables conditionally. The scalar code
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/ratemonitor.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/ratemonitor.py_`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/reset.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/reset.py_`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/spatialstateupdate.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/spatialstateupdate.py_`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/spikegenerator.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/spikegenerator.py_`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/synapses_create_array.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_create_array.py_`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/synapses_create_generator.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_create_generator.py_`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-{#
-USES_VARIABLES { _synaptic_pre, _synaptic_post, N,
-                 N_pre, N_post, _source_offset, _target_offset }
-#}
-{# WRITES_TO_READ_ONLY_VARIABLES { _synaptic_pre, _synaptic_post, N}
-#}
-{# ITERATE_ALL { _idx } #}
-{% extends 'common_group.py_' %}
-
-{% block maincode %}
-# Only need to do the initial import once, and trying is not expensive
-# only catching exceptions is expensive (which we just do the first time)
-try:
-    _done_initial_import
-except:
-    _done_initial_import = True
+    {#
+    USES_VARIABLES { _synaptic_pre, _synaptic_post, N,
+                    N_pre, N_post, _source_offset, _target_offset }
+    #}
+    {# WRITES_TO_READ_ONLY_VARIABLES { _synaptic_pre, _synaptic_post, N}
+    #}
+    {# ITERATE_ALL { _idx } #}
+    {% extends 'common_group.py_' %}
+
+    {% block maincode %}
+    # Only need to do the initial import once, and trying is not expensive
+    # only catching exceptions is expensive (which we just do the first time)
     import sys as _sys
     from numpy.random import rand as _np_rand
-    if _sys.version_info[0]==2:
-        range = xrange
-
     from numpy.random import binomial as _binomial
     import bisect as _bisect
     def _sample_without_replacement(low, high, step, p=None, size=None):
         if p == 0:
             return _numpy.array([], dtype=_numpy.int32)
         if p == 1:
             return _numpy.arange(low, high, step)
@@ -39,15 +32,15 @@
             raise IndexError(f"Requested sample size {size} is negative.")
             {% endif %}
         elif size is not None and size > n:
             {% if skip_if_invalid %}
             size = n
             {% else %}
             raise IndexError(f"Requested sample size {size} is bigger than the "
-                             f"population size {n}.")
+                            f"population size {n}.")
             {% endif %}
         if n == size:
             return _numpy.arange(low, high, step)
         if p is None:
             if step == 1:
                 _choice = _numpy.random.choice(n,  size=size, replace=False) + low
             else:
@@ -83,129 +76,146 @@
                 start = samples[-1]+1 # this is the starting point for the next round
                 if start >= n:
                     break
             if len(all_samples) > 1:
                 samples = _numpy.hstack(all_samples)
             samples = samples[:_bisect.bisect_left(samples, n)] # only keep the ones in the range we want
         return samples*step+low
-
-# number of synapses in the beginning
-_old_num_synapses = {{N}}
-# number of synapses during the creation process
-_cur_num_synapses = _old_num_synapses
-
-# scalar code
-_vectorisation_idx = 1
-{{scalar_code['setup_iterator']|autoindent}}
-{{scalar_code['generator_expr']|autoindent}}
-{{scalar_code['create_cond']|autoindent}}
-{{scalar_code['update']|autoindent}}
-
-{# For a connect call j='k+i for k in range(0, N_post, 2) if k+i < N_post'
-"j" is called the "result index" (and "_post_idx" the "result index array", etc.)
-"i" is called the "outer index" (and "_pre_idx" the "outer index array", etc.)
-"k" is called the inner variable #}
-
-for _{{outer_index}} in range({{outer_index_size}}):
-    _raw{{outer_index_array}} = _{{outer_index}} + {{outer_index_offset}}
-    {% if not result_index_condition %}
-    {{vector_code['create_cond']|autoindent}}
-    if not _cond:
-        continue
-    {% endif %}
-    {{vector_code['setup_iterator']|autoindent}}
-    {% if iterator_func=='range' %}
-    {{inner_variable}} = _numpy.arange(_iter_low, _iter_high, _iter_step)
-    {% elif iterator_func=='sample' %}
-    {% if iterator_kwds['sample_size'] == 'fixed' %}
-    {{inner_variable}} = _sample_without_replacement(_iter_low, _iter_high, _iter_step, None, size=_iter_size)
-    {% else %}
-    {{inner_variable}} = _sample_without_replacement(_iter_low, _iter_high, _iter_step, _iter_p)
-    {% endif %}
-    {% endif %}
-
-    _vectorisation_idx = {{inner_variable}}
-    {{vector_code['generator_expr']|autoindent}}
-    _vectorisation_idx = _{{result_index}}
-    _raw{{result_index_array}} = _{{result_index}} + {{result_index_offset}}
-    {% if result_index_condition %}
-    {% if result_index_used %}
-    {# The condition could index outside of array range #}
-    {% if skip_if_invalid %}
-    if _numpy.isscalar(_{{result_index}}):
-        if _{{result_index}}<0 or _{{result_index}}>={{result_index_size}}:
+    # Constants
+    {% for c in constants %}
+    {{ c }}
+    {% endfor%}
+    # number of synapses in the beginning
+    {% set N_init = get_array_name(owner.variables["N"], template_name = 'synapses_create_generator')%}
+    _old_num_synapses = int({{N_init}})
+    # number of synapses during the creation process
+    _cur_num_synapses = _old_num_synapses
+
+    # scalar code
+    _vectorisation_idx = 1
+    {{scalar_code['setup_iterator']|autoindent}}
+    {{scalar_code['generator_expr']|autoindent}}
+    {{scalar_code['create_cond']|autoindent}}
+    {{scalar_code['update']|autoindent}}
+
+    {# For a connect call j='k+i for k in range(0, N_post, 2) if k+i < N_post'
+    "j" is called the "result index" (and "_post_idx" the "result index array", etc.)
+    "i" is called the "outer index" (and "_pre_idx" the "outer index array", etc.)
+    "k" is called the inner variable #}
+
+    for _{{outer_index}} in range({{outer_index_size}}):
+        _raw{{outer_index_array}} = _{{outer_index}} + {{outer_index_offset}}
+        {% if not result_index_condition %}
+        {{vector_code['create_cond']|autoindent}}
+        if not _cond:
             continue
-    else:
-        _in_range = _numpy.logical_and(_{{result_index}}>=0, _{{result_index}}<{{result_index_size}})
-        _{{result_index}} = _{{result_index}}[_in_range]
-    {% else %}
-    if _numpy.isscalar(_{{result_index}}):
-        _min_val = _max_val = _{{result_index}}
-    elif _{{result_index}}.shape == (0, ):
-        continue
-    else:
-        _min_val = _numpy.min(_{{result_index}})
-        _max_val = _numpy.max(_{{result_index}})
-    if _min_val < 0:
-        # Stick to % formatting, since curly braces are used by Jinja2 already
-        raise IndexError("index {{result_index}}=%d outside allowed range from 0 to %d, and the condition refers to a post-synaptic variable" % (_min_val, {{result_index_size}}-1))
-    elif _max_val >= {{result_index_size}}:
-        raise IndexError("index {{result_index}}=%d outside allowed range from 0 to %d, and the condition refers to a post-synaptic variable" % (_max_val, {{result_index_size}}-1))
-    {% endif %}
-    {% endif %}
-    {{vector_code['create_cond']|autoindent}}
-    {% endif %}
-    {% if if_expression!='True' and result_index_condition %}
-    _{{result_index}}, _cond = _numpy.broadcast_arrays(_{{result_index}}, _cond)
-    _{{result_index}} = _{{result_index}}[_cond]
-    {% else %}
-    _{{result_index}}, {{inner_variable}} = _numpy.broadcast_arrays(_{{result_index}}, {{inner_variable}})
-    {% endif %}
-
-    {% if skip_if_invalid %}
-    if _numpy.isscalar(_{{result_index}}):
-        if _{{result_index}}<0 or _{{result_index}}>={{result_index_size}}:
+        {% endif %}
+        {{vector_code['setup_iterator']|autoindent}}
+        {% if iterator_func=='range' %}
+        {{inner_variable}} = _numpy.arange(_iter_low, _iter_high, _iter_step)
+        {% elif iterator_func=='sample' %}
+        {% if iterator_kwds['sample_size'] == 'fixed' %}
+        {{inner_variable}} = _sample_without_replacement(_iter_low, _iter_high, _iter_step, None, size=_iter_size)
+        {% else %}
+        {{inner_variable}} = _sample_without_replacement(_iter_low, _iter_high, _iter_step, _iter_p)
+        {% endif %}
+        {% endif %}
+
+        _vectorisation_idx = {{inner_variable}}
+        {{vector_code['generator_expr']|autoindent}}
+        _vectorisation_idx = _{{result_index}}
+        _raw{{result_index_array}} = _{{result_index}} + {{result_index_offset}}
+        {% if result_index_condition %}
+        {% if result_index_used %}
+        {# The condition could index outside of array range #}
+        {% if skip_if_invalid %}
+        if _numpy.isscalar(_{{result_index}}):
+            if _{{result_index}}<0 or _{{result_index}}>={{result_index_size}}:
+                continue
+        else:
+            _in_range = _numpy.logical_and(_{{result_index}}>=0, _{{result_index}}<{{result_index_size}})
+            _{{result_index}} = _{{result_index}}[_in_range]
+        {% else %}
+        if _numpy.isscalar(_{{result_index}}):
+            _min_val = _max_val = _{{result_index}}
+        elif _{{result_index}}.shape == (0, ):
             continue
-    else:
-        _in_range = _numpy.logical_and(_{{result_index}}>=0, _{{result_index}}<{{result_index_size}})
-        _{{result_index}} = _{{result_index}}[_in_range]
-    {% elif not result_index_used %}
-    {# Otherwise, we already checked before #}
-    if _numpy.isscalar(_{{result_index}}):
-        _min_val = _max_val = _{{result_index}}
-    elif _{{result_index}}.shape == (0, ):
-        continue
-    else:
-        _min_val = _numpy.min(_{{result_index}})
-        _max_val = _numpy.max(_{{result_index}})
-    if _min_val < 0:
-        raise IndexError("index _{{result_index}}=%d outside allowed range from 0 to %d" % (_min_val, {{result_index_size}}-1))
-    elif _max_val >= {{result_index_size}}:
-        raise IndexError("index _{{result_index}}=%d outside allowed range from 0 to %d" % (_max_val, {{result_index_size}}-1))
-    {% endif %}
-
-    _vectorisation_idx = _{{result_index}}
-    _raw{{result_index_array}} = _{{result_index}} + {{result_index_offset}}
-    {{vector_code['update']|autoindent}}
-
-    if not _numpy.isscalar(_n):
-        # The "n" expression involved the target variable
-        {{result_index_array}} = {{result_index_array}}.repeat(_n[_j])
-    elif _n != 1:
-        # We have a target-independent number
-        {{result_index_array}} = {{result_index_array}}.repeat(_n)
-    _numnew = len({{result_index_array}})
-
-    _new_num_synapses = _cur_num_synapses + _numnew
-    {{_dynamic__synaptic_pre}}.resize(_new_num_synapses)
-    {{_dynamic__synaptic_post}}.resize(_new_num_synapses)
-    {{_dynamic__synaptic_pre}}[_cur_num_synapses:] = _pre_idx
-    {{_dynamic__synaptic_post}}[_cur_num_synapses:] = _post_idx
-    _cur_num_synapses += _numnew
-
-# Resize all dependent dynamic arrays (synaptic weights, delays, etc.) and set
-# the total number of synapses
-_owner._resize(_cur_num_synapses)
-
-# And update N_incoming, N_outgoing and synapse_number
-_owner._update_synapse_numbers(_old_num_synapses)
-{% endblock %}
+        else:
+            _min_val = _numpy.min(_{{result_index}})
+            _max_val = _numpy.max(_{{result_index}})
+        if _min_val < 0:
+            # Stick to % formatting, since curly braces are used by Jinja2 already
+            raise IndexError("index {{result_index}}=%d outside allowed range from 0 to %d, and the condition refers to a post-synaptic variable" % (_min_val, {{result_index_size}}-1))
+        elif _max_val >= {{result_index_size}}:
+            raise IndexError("index {{result_index}}=%d outside allowed range from 0 to %d, and the condition refers to a post-synaptic variable" % (_max_val, {{result_index_size}}-1))
+        {% endif %}
+        {% endif %}
+        {{vector_code['create_cond']|autoindent}}
+        {% endif %}
+        {% if if_expression!='True' and result_index_condition %}
+        _{{result_index}}, _cond = _numpy.broadcast_arrays(_{{result_index}}, _cond)
+        _{{result_index}} = _{{result_index}}[_cond]
+        {% else %}
+        _{{result_index}}, {{inner_variable}} = _numpy.broadcast_arrays(_{{result_index}}, {{inner_variable}})
+        {% endif %}
+
+        {% if skip_if_invalid %}
+        if _numpy.isscalar(_{{result_index}}):
+            if _{{result_index}}<0 or _{{result_index}}>={{result_index_size}}:
+                continue
+        else:
+            _in_range = _numpy.logical_and(_{{result_index}}>=0, _{{result_index}}<{{result_index_size}})
+            _{{result_index}} = _{{result_index}}[_in_range]
+        {% elif not result_index_used %}
+        {# Otherwise, we already checked before #}
+        if _numpy.isscalar(_{{result_index}}):
+            _min_val = _max_val = _{{result_index}}
+        elif _{{result_index}}.shape == (0, ):
+            continue
+        else:
+            _min_val = _numpy.min(_{{result_index}})
+            _max_val = _numpy.max(_{{result_index}})
+        if _min_val < 0:
+            raise IndexError("index _{{result_index}}=%d outside allowed range from 0 to %d" % (_min_val, {{result_index_size}}-1))
+        elif _max_val >= {{result_index_size}}:
+            raise IndexError("index _{{result_index}}=%d outside allowed range from 0 to %d" % (_max_val, {{result_index_size}}-1))
+        {% endif %}
+
+        _vectorisation_idx = _{{result_index}}
+        _raw{{result_index_array}} = _{{result_index}} + {{result_index_offset}}
+        {{vector_code['update']|autoindent}}
+
+        if not _numpy.isscalar(_n):
+            # The "n" expression involved the target variable
+            {{result_index_array}} = {{result_index_array}}.repeat(_n[_j])
+        elif _n != 1:
+            # We have a target-independent number
+            {{result_index_array}} = {{result_index_array}}.repeat(_n)
+        _numnew = len({{result_index_array}})
+
+        _new_num_synapses = _cur_num_synapses + _numnew
+        {{_dynamic__synaptic_pre_init}} = _numpy.resize({{_dynamic__synaptic_pre_init}},_new_num_synapses)
+        {{_dynamic__synaptic_post_init}} = _numpy.resize({{_dynamic__synaptic_post_init}},_new_num_synapses)
+        {{_dynamic__synaptic_pre_init}}[_cur_num_synapses:] = _pre_idx
+        {{_dynamic__synaptic_post_init}}[_cur_num_synapses:] = _post_idx
+        _cur_num_synapses += _numnew
+
+    # Resize all dependent dynamic arrays (synaptic weights, delays, etc.) and set
+    # the total number of synapses
+
+    # Resize all dependent dynamic arrays (synaptic weights, delays, etc.) and set
+    # the total number of synapses
+    # TODO: when we implement a separate synapses process we could just use owner._resize() as shown below
+    {% for var in owner._registered_variables %}
+    {# We have to set the varnames manually instead of using filters because we need a special naming for this template #}
+    {% set varname = get_array_name(var,access_data = False, template_name = 'synapses_create_generator') %}
+    {{varname}} = _numpy.resize({{varname}}, _cur_num_synapses)
+    {% endfor %}
+
+    {{N_init}} = _numpy.array([_cur_num_synapses],dtype = 'int32')
+    # TODO to be deleted unless we implement the resize method.
+    #_owner._resize(_cur_num_synapses)
+
+    # And update N_incoming, N_outgoing and synapse_number
+    #_owner._update_synapse_numbers(_old_num_synapses)
+
+    {% endblock %}
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/synapses_push_spikes.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_push_spikes.py_`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/codegen/templates/threshold.py_` & `brian2lava-1.0.0a2/brian2lava/codegen/templates/threshold.py_`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/brian2lava/device/__init__.py` & `brian2lava-1.0.0a2/brian2lava/device/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,21 @@
 
         # Store root directory of this package
         self.package_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
         # The project dir is fixed in the Lava device
         # This is important, since a reinit otherweise don't know which directory to clean
         self.project_dir = 'lava_workspace'
+        os.makedirs('lava_workspace', exist_ok=True)
+        # Clear the contents of the workspace if it already existed.
+        for filename in os.listdir(self.project_dir):
+            file_path = os.path.join(self.project_dir, filename)
+
+            if os.path.isfile(file_path):
+                os.remove(file_path)
 
         # FIXME Defines the network schedule, if None, the user can choose the schedule
         self.network_schedule = None
         # NOTE Brian2Loihi used: ['start', 'synapses', 'groups', 'thresholds',  'resets', 'end']
 
         # Random number buffer
         self.randn_buffer_index = np.zeros(1, dtype=np.int32)
@@ -71,51 +78,49 @@
         # Store the ports required to connect processes
         self.lava_ports = {}
 
         # Brian template functions that belong to the process,
         # instead of the process model, e.g. 'group_variable_set'
         self.init_template_functions = [
             'group_variable_set',
+            'group_variable_set_conditional',
             'synapses_create_generator',
             'synapses_create_array'
         ]
         
         # Variables that represent our current feature support
-        from brian2 import SpikeGeneratorGroup, NeuronGroup, Synapses
+        from brian2 import SpikeGeneratorGroup, NeuronGroup, Synapses, PoissonGroup
         self.supported_processes = [
             NeuronGroup,
             Synapses,
-            SpikeGeneratorGroup
+            SpikeGeneratorGroup,
+            PoissonGroup
         ]
-        from brian2 import PoissonInput,PopulationRateMonitor,SpatialNeuron, PoissonGroup
+        from brian2 import PoissonInput,PopulationRateMonitor,SpatialNeuron
+        from brian2.synapses.synapses import SummedVariableUpdater
         self.unsupported_processes = [
             PoissonInput,
             PopulationRateMonitor,
             SpatialNeuron,
-            PoissonGroup
+            SummedVariableUpdater
         ]
 
         self.available_hardware = ["CPU"]
 
         # Stores names of indices that are used to initialize variables
         # e.g. _group_idx_1_v, _group_idx_2_ge, etc.
         self.set_variable_index_names = []
 
-        # Last method name for setting variables
-        self.last_set_variable_method_name = ''
-
-        # Maps process *method name* (for initializing variables) with
-        # *variable name* (variable to initialize)
-        self.init_variables = {}
-
         # Store Lava monitors
         # NOTE Some variables shall be probed only once by Lava, but are required
         #      for different Brian monitors, e.g. time
         self.lava_variables_to_monitor = []
         self.lava_monitors = {}
+        # Add monitors for additional variables (only for SpikeMonitors)
+        self.additional_monitors = {}
         #self.brian_monitors = {}
 
         self.monitor_types = {'state': 0, 'spike': 1}  # SimpleNamespace(**{ 'state': 0, 'spike': 1 })
         
         # Init a variable to store the Lava process
         self.process = None
 
@@ -152,41 +157,47 @@
     # Writer for writing rendered templates
     from .writer import (
         prepare_directory, write_templates
     )
 
     # Define code objects
     from .codeobject import (
-        code_object,
-        determine_lava_ports
+        code_object
     )
 
     # Run the network
     from .run import (
-        network_run, run, set_brian_monitor_values, init_lava_monitors, connect_lava_ports,select_root_processes
+        network_run, 
+        run_processes,
+        set_brian_monitor_values,
+        init_lava_monitors, 
+        connect_lava_ports,
+        select_root_processes,
+        update_brian_class_attributes
     )
 
     # Handle storage
     from .arrays import (
         add_array, get_value, get_array_name, init_with_zeros,
-        init_with_arange, fill_with_array, get_var_by_lava_name,
+        init_with_arange, fill_with_array,
         get_lava_var_name, resize
     )
 
     # Handle setter and getter for variables
     from .variables import (
         variableview_set_with_index_array,
         variableview_set_with_expression,
         variableview_set_with_expression_conditional
     )
 
     # Handle synapses
     from .synapses import (
         synapses_connect,
         spike_queue,
-        add_lava_synapses_generator
+        determine_lava_ports,
+        _add_spiking_synapses_vars
     )
 
 
 # Add lava device to all_devices and make it with this available to Brian2
 lava_device = LavaDevice()
 all_devices['lava'] = lava_device
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/device/activate.py` & `brian2lava-1.0.0a2/brian2lava/device/activate.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,14 @@
     Activates Brian2Lava device.
 
     The method adds the `LavaCodeObject` as code generation target
     """
     # Log that activate method was called
     self.logger.debug("Activating Lava device.")
 
-    # Use Lava code object
-    codegen_targets.add(LavaCodeObject)
-
     # Set codegen targets to 'lava'
     prefs.codegen.target = 'lava'
     prefs.codegen.string_expression_target = 'lava'
 
     # Log used device and code object
     self.logger.debug(f'Using code object class: {self.code_object_class().__name__} with Device: {self}')
 
@@ -51,29 +48,51 @@
     """
     Reinitializes the device, which is necessary if multiple `run()` calls
     are performed within a single script.
 
     *   Initialize device and call parent's `reinit`
     *   Reset `did_run` flag 
     *   Set network schedule and 'build_on_run' flag to previously chosen values
-    *   Clean workspace directory
     """
+    # TODO: fix!
+    self.logger.warn("""
+    Currently the device.reinit() method is causing some bugs so it is not recommended to use it.
+    If you want to run multiple simulations within a single notebook, we recommend to restart the kernel
+    for each new simulation run.
+    """)
     # Store network schedule and 'build_on_run' flag
     tmp_network_schedule = self.network_schedule
     tmp_build_on_run = self.build_on_run
+    build_options = self.build_options
+
+
+    # To make sure that we lose track of previously defined variables, we delete the
+    # class attributes.
+    for key in list(self.__dict__.keys()):
+        delattr(self, key)
+    
+    # Delete all the previously defined brian objects
+    if hasattr(self, 'lava_objects'):
+        for obj in self.lava_objects.values():
+            del obj
+    
+    # Delete the previously defined lava monitors
+    if hasattr(self, 'lava_monitors'):
+        for m in self.lava_monitors.values():
+            if m['lava_monitor'] is not None:
+                del m['lava_monitor']
 
     # Initialize the device
     self.__init__()
 
-    # Call reinit from super device
-    self.super.reinit()  # necessary?
-
     # Resets the 'did_run' flag
     self.did_run = False
 
     # Set network schedule and 'build_on_run' flag to previously chosen values
     self.network_schedule = tmp_network_schedule
     self.build_on_run = tmp_build_on_run
 
+    self.activate(build_on_run = self.build_on_run, **build_options)
+
     # Clean workspace: Get absolute workspace directory and remove recursively
-    abs_project_dir = os.path.abspath(os.path.join(os.getcwd(), self.project_dir))
-    shutil.rmtree(abs_project_dir)
+    #abs_project_dir = os.path.abspath(os.path.join(self.package_root, '..', self.project_dir))
+    #shutil.rmtree(abs_project_dir)
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/device/arrays.py` & `brian2lava-1.0.0a2/brian2lava/device/arrays.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,40 +27,45 @@
     """
 
     # Log that a value was requested from arrays
     self.logger.diagnostic(f'get_value {var.name}')
 
     return self.arrays[var]
 
-
-def get_var_by_lava_name(self, lava_var_name):
+def get_dtype_name(var):
     """
-    Get an array variable from array by lava variable name
+    Get the data type of a variable and return its name as a string - serves to avoid expressions like 'np.bool' that are deprecated since NumPy 1.24.
+    In the case of a NumPy data type, returns the name with the prefix 'np.'.
 
     Parameters
     ----------
-    lava_var_name : `string`
-        The name of the lava variable
+    var : `any`
+        The variable to consider (can also be a data type object itself)
 
     Returns
     -------
-    `ArrayVariable`
-        An array variable
+    `string`
+        Name of the dtype
     """
 
-    # Iterate over all arrays
-    for var, values in self.arrays.items():
-        # Check if variable is not DynamicArrayVariable, since we don't want to get monitor variables
-        is_no_monitor = not isinstance(var, DynamicArrayVariable)
-        # Check if name of variable matches given name
-        is_name_match = self.get_lava_var_name(var) == lava_var_name
-
-        # If both conditions match, break loop and return variable
-        if is_no_monitor and is_name_match:
-            return var
+    # If 'var' is an array
+    if np.ndim(var) > 0:
+        dtype = var.dtype
+    # If 'var' is a scalar variable
+    else:
+        dtype = np.dtype(type(var))
+
+    # Check if Python or NumPy data type is used
+    if dtype in [bool, int, float, complex, str, np.int32, np.int64, np.float32, np.float64]:
+        ret = dtype.name.replace('32', '').replace('64', '')
+    else:
+        ret = "np." + dtype.name
+
+    #print(f'get_dtype_name({var}) = {ret}')
+    return ret
 
 
 def get_lava_var_name(self, var):
     """
     Get a lava variable name based on an array variable.
 
     Parameters
@@ -82,14 +87,16 @@
         source_name = 'defaultclock' if var.name == 't' else var.owner.source.name
         #source_name = var.owner.name
         return f'_{source_name}_{var.name}'
     elif isinstance(var.owner, SpikeMonitor):
         lava_var_name = ''
         if var.name == 't': lava_var_name = '_defaultclock_t'
         if var.name == 'i': lava_var_name = var.owner.source.name +'_s_out'
+        # Manage the case of additional variables in the SpikeMonitor
+        else: lava_var_name = f'_{var.owner.source.name}_{var.name}'
         return lava_var_name
     else:
         return f'_{var.owner.name}_{var.name}'
 
 
 def get_array_name(self, var, access_data=True, prefix='self.'):
     """
@@ -109,21 +116,22 @@
     Returns
     -------
     `string`
         The corresponding variable name as it is used in Brian
 
     Notes
     -----
-    TODO This can possibly be hamrmonized with `get_lava_var_name`.
+    TODO This can possibly be harmonized with `get_lava_var_name`.
     """
     
     # The name of the array is part of the owner attribute
     # The owner is a `Nameable`, e.g. `NeuronGroup` or `Synapses`
     # If no owner name is available, 'temporary' is assigned
     owner_name = getattr(var.owner, 'name', 'temporary')
+    
 
     # Redefine prefix to empty string if it was set to 'None'
     if prefix is None:
         prefix = ''
     
     return f'{prefix}_{owner_name}_{var.name}'
 
@@ -186,56 +194,107 @@
     # Add array to device arrays
     self.arrays[var] = arr
 
     if isinstance(var.owner, (SpikeMonitor, StateMonitor)):
         # NOTE Currently only dynamic array variables of a monitor (like v, t, etc.) are added
         #      Constant values like N or __indices are currently ignored
         if isinstance(var, DynamicArrayVariable):
+            if isinstance(var.owner.record,bool):
+                # we only add a monitor if the record flag is not set to False, which means that the
+                # monitor is not used for recording.
+                if var.owner.record == False:
+                    if isinstance(var.owner,SpikeMonitor):
+                        self.logger.warn("Currently, setting 'record=False' in the SpikeMonitor is not supported. It will be in future releases")
+                    else:
+                        return   
+            else:
+                # Check if the user is trying to record specific indices
+                if len(var.owner.record) != len(var.owner.source) and var.name != 't':
+                    self.logger.warn("""[EFFICIENCY]: Setting recording indices is currently not supported by Lava. 
+                    The monitor will record all indices, which will then be filtered by brian2lava at a 
+                    later stage (so that the output will be compatible with what expected from Brian). 
+                    For this reason, the current implementation will be significantly slower than the 
+                    Brian implementation for larger simulations.""")
 
             # Get monitor type name from owner ('state' or 'spike')
             monitor_type_name = get_monitor_type_name(var.owner)
 
+            # We don't need a monitor for spike timings since this measurement is 
+            # handled differently.
+            if var.name == 't' and monitor_type_name == 'spike':
+                return
+
             # Define monitor name and lava variable name
-            monitor_name = f'_{monitor_type_name}_{var.owner.name}_{var.name}'
+            monitor_name = f'_{monitor_type_name}_{var.owner.name}'
+            # Spike monitors don't need variable names, this is to allow monitoring additional variables.
+            monitor_name += f'_{var.name}' if isinstance(var.owner, StateMonitor) else ''
             lava_var_name = self.get_lava_var_name(var)
 
+            # Set up the additional monitors if they were not yet defined.
+            if not monitor_name in self.additional_monitors:
+                self.additional_monitors[monitor_name] = []
+
             # Collect lava variable names that shall be monitored by lava
             # NOTE Only add variable name if it's not already in the list
             #      Variable names can occure in multiple monitors, e.g. time
             if lava_var_name not in self.lava_variables_to_monitor:
                 self.lava_variables_to_monitor.append(lava_var_name)
-            # Define monitor
+
+            # Special case: If the monitor already exists then we are dealing with an additional variable for SpikeMonitor
+            if monitor_type_name == 'spike' and var.name != 'i':
+                monitor_dict = {
+                        'name' : monitor_name + f"_add_{var.name}", # The name of this monitor, mainly for debugging
+                        'source': var.owner.source.name,
+                        'var': var,  # Brian variable
+                        'indices': var.owner.record,  # The indices of the variable to record
+                        'lava_var_name': lava_var_name,  # The variable name used in Lava
+                        'lava_monitor': None,  # The Lava monitor, instance is added later during 'run'
+                        'process_name': None # The name of the process that is monitored, will be set in 'run'
+                    }
+                # Add this monitor to the additional monitors
+                self.additional_monitors[monitor_name].append(monitor_dict)
+                try:
+                    # Add the additional monitors to the existing monitor
+                    self.lava_monitors[monitor_name]['additional_var_monitors'] = self.additional_monitors[monitor_name]
+                except KeyError:
+                    # This happens if the monitor was not added yet, so the additional monitors will be added 
+                    # when the monitor is defined through the 'i' variable.
+                    self.logger.debug(f"Monitor {monitor_name} not added yet, will add the additional var monitor for {lava_var_name} later.")
+                return
+
+            # This is the general purpose case. We are dealing with a new monitor.
             self.lava_monitors[monitor_name] = {
                 'name' : monitor_name, # The name of this monitor, mainly for debugging
                 'source': var.owner.source.name,
                 'var': var,  # Brian variable
+                'indices': var.owner.record,  # The indices of the variable to record
                 'lava_var_name': lava_var_name,  # The variable name used in Lava
                 'type': self.monitor_types[monitor_type_name],  # The monitor type ('state' or 'spike')
-                'lava_monitor': None  # The Lava monitor, instance is added later during 'run'
+                'additional_var_monitors': self.additional_monitors[monitor_name],  # Additional variables to monitor, e.g. 'v' for SpikeMonitor
+                'lava_monitor': None,  # The Lava monitor, instance is added later during 'run'
+                'process_name': None # The name of the process that is monitored, will be set in 'run'
             }
     else:
+        
+        dtype_name = get_dtype_name(arr)
+        type_name = dtype_name
         # Add the definition of a numpy array as string for lava
-        var_definition = f'np.empty({var.size}, dtype=np.{arr.dtype.name})'
-
-        # TODO this can be done better probably
-        dtype = arr.dtype.name        
-        value_type = dtype.replace('32', '')
-        value_type = value_type.replace('64', '')
+        var_definition = f'np.empty({var.size}, dtype={type_name})'
 
         # TODO is the key unique?
         # See also: https://github.com/brian-team/brian2/pull/304
         name = f'_{var.owner.name}_{var.name}'
         self.lava_variables[name] = {
             'name': var.name,
             'owner': var.owner.name,
             'definition': var_definition,
             'size': var.size,
             'shape': np.shape(arr),
-            'type': value_type,
-            'dtype': arr.dtype.name
+            'type': type_name,
+            'dtype': dtype_name
         }
 
         # NOTE information from this dict can also be obtained from self.lava_variables
         #      directly, but it's a bit complicated, for now we can leave it as a kind of cache
         self.lava_variable_names[var.name] = name
 
 
@@ -251,15 +310,15 @@
         The data type to use for the array
     """
 
     # Redefine variable definition for Lava variables
     name = f'_{var.owner.name}_{var.name}'
     if name in self.lava_variables.keys():
         lv = self.lava_variables[name]
-        lv['definition'] = f'np.zeros({lv["size"]}, dtype=np.{lv["dtype"]})'
+        lv['definition'] = f'np.zeros({lv["size"]}, dtype={lv["dtype"]})'
     
     # Log that an empty array was initialized
     self.logger.diagnostic(f'init_with_zeros {var.name}')
     
     self.arrays[var][:] = 0
 
 
@@ -278,15 +337,15 @@
         The data type to use for the array
     """
 
     # Redefine variable definition for Lava variables
     name = f'_{var.owner.name}_{var.name}'
     if name in self.lava_variables.keys():
         lv = self.lava_variables[name]
-        lv['definition'] = f'np.arange({start}, {lv["size"]+start}, dtype=np.{lv["dtype"]})'
+        lv['definition'] = f'np.arange({start}, {lv["size"]+start}, dtype={lv["dtype"]})'
     
     # Log that an array was created based on numpy arange
     self.logger.diagnostic(f'init_with_arange, arange from {start} to {var.get_len()+start}')
     
     self.arrays[var][:] = np.arange(start, stop=var.get_len()+start, dtype=dtype)
 
 
@@ -309,43 +368,44 @@
         lv = self.lava_variables[name]
 
         # Check if 'arr' is given as scalar
         is_scalar = not bool(len(np.shape(arr)))
         
         # If 'arr' is scalar and size is 1, add a simple array
         if is_scalar and lv['size'] == 1:
-            lv['definition'] = f'np.array([{arr}], dtype=np.{lv["dtype"]})'
+            lv['definition'] = f'np.array([{arr}], dtype={lv["dtype"]})'
         # If 'arr' is scalar and size > 1, add an array that repeats the value accordingly
         elif is_scalar and lv['size'] > 1:
-            lv['definition'] = f'np.array(np.repeat({arr}, {lv["size"]}), dtype=np.{lv["dtype"]})'
+            lv['definition'] = f'np.array(np.repeat({arr}, {lv["size"]}), dtype={lv["dtype"]})'
         # If 'arr' is actually an array, it's just transformed to a string definition
         else:
             arr_str = np.array2string(np.array(arr), separator=', ')
-            lv['definition'] = f'np.array({arr_str}, dtype=np.{lv["dtype"]})'
+            lv['definition'] = f'np.array({arr_str}, dtype={lv["dtype"]})'
 
     # Log that an array was filled with given values
     self.logger.diagnostic(f'fill_with_array, add {arr} to {var.name}')
     
     # Set array value
     self.arrays[var][:] = arr
 
 def resize(self, var, new_size):
     """
     Method called most times a DynamicArray variable is created. Updates the size of a DynamicArray.
     """
     # First resize it in our array-cache
-    self.arrays[var].resize(new_size)
+    # We use this form due to an error when trying to resize an array which is referenced by another array.
+    self.arrays[var] = np.resize(self.arrays[var], new_size)
 
     # Change the size of the variable in our variable dictionary
     # We also make sure to update the default definition in case the variable
     # is not initialized with a 'fill_with' method afterwards (in most cases it is).
     # This is probably redundant but ensures no bugs come up later on.
     name = f'_{var.owner.name}_{var.name}'
     if name in self.lava_variables.keys():
         lv = self.lava_variables[name]
         lv["size"] = new_size
         if 'np.empty' in lv["definition"]:
-            lv["definition"] = f'np.empty({lv["size"]}, dtype=np.{lv["dtype"]})'
+            lv["definition"] = f'np.empty({lv["size"]}, dtype={lv["dtype"]})'
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/device/build.py` & `brian2lava-1.0.0a2/brian2lava/device/build.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # from brian2.core.variables import Constant, ArrayVariable, AuxiliaryVariable
 from brian2.groups.neurongroup import NeuronGroup, StateUpdater, Resetter, Thresholder, SubexpressionUpdater
 from brian2.input.poissongroup import PoissonGroup
 from brian2.input.spikegeneratorgroup import SpikeGeneratorGroup
 from brian2.monitors.spikemonitor import SpikeMonitor
 from brian2.monitors.ratemonitor import PopulationRateMonitor
 from brian2.monitors.statemonitor import StateMonitor
-from brian2.synapses.synapses import Synapses
+from brian2.synapses.synapses import Synapses, SpikeSource
 # from brian2.units import second
 
 from pprint import pprint
 
 
 def build(
     self,
@@ -82,31 +82,31 @@
     # Get dt in seconds without unit
     dt_ = self.defaultclock.dt_
     # Add 'dt' to 'lava_variables' to make it available to Lava
     self.lava_variables['_defaultclock_dt']['definition'] = f'np.array([{dt_}])'
 
     if hardware == 'CPU':
         # Render Lava templates
-        for obj in self.lava_objects:
+        for obj in self.lava_objects.values():
             process_rendered, process_model_rendered = self.render_templates(obj)
             self.logger.diagnostic(
                 f"Compiling templates:\nProcess:\n{process_rendered}\nProcess Model:\n{process_model_rendered}"
             )
             # Write to file
             self.write_templates(process_rendered, process_model_rendered,obj.name)
 
         # Run Lava process
-        self.run()
+        self.run_processes()
     else:
         raise NotImplementedError(f'Hardware {hardware} is not implemented (yet), the list of available hardware: {self.available_hardware}')
 
 
 def render_templates(self, obj):
     """
-    Renders Jinja templates based on Brian network objects that are used in the lava taplates.
+    Renders Jinja templates based on Brian network objects that are used in the Lava templates.
     We call them `lava objects`.
 
     Parameters
     ----------
     obj : lava_object
         Lava related network object
     
@@ -131,15 +131,15 @@
     for item in process_model_methods:
         s += f'{item}\n'
     self.logger.diagnostic(s)
 
     # Get a list of ordered function calls to be implemented in
     # the 'run' and '__init__' function
     # TODO rename to 'process' and 'process_model' functions
-    lava_init_function_calls, lava_multi_init, lava_run_function_calls = self.get_lava_function_calls(obj)
+    lava_init_function_calls, lava_run_function_calls, learning_function_calls = self.get_lava_function_calls(obj)
 
     # Get the port definitions for process and process model
     proc_ports, proc_model_ports = self.get_lava_ports_definitions(obj)
     
     # Get formatted variables for lava process
     proc_variables_init, proc_variables_lava = self.get_lava_proc_variables(obj, lava_init_function_calls)
     
@@ -166,25 +166,26 @@
     env = self.get_jinja_environment()
 
     # Load and render 'process'
     process_template = env.get_template('process.py.j2')
     process_rendered = process_template.render(
         variables_init=proc_variables_init,
         variables_lava=proc_variables_lava,
-        multi_init_calls = lava_multi_init,
+        init_calls = lava_init_function_calls,
         init_methods=process_methods,
         required_imports=collect_required_imports(process_methods),
         name = obj.name
     )
     
     # Load and render 'process model'
     process_model_template = env.get_template('process_model.py.j2')
     process_model_rendered = process_model_template.render(
         methods=process_model_methods,
         run_functions=lava_run_function_calls,
+        lrn_functions = learning_function_calls,
         variables=lava_proc_model_variables,
         required_imports=collect_required_imports(process_model_methods),
         name = obj.name
     )
     
     return process_rendered, process_model_rendered
 
@@ -274,18 +275,19 @@
     # Define potential imports
     potential_imports = {
         'random': 'from random import random',
         'timestep': 'from brian2.core.functions import timestep',
         'LazyArange': 'from brian2.codegen.runtime.numpy_rt.numpy_rt import LazyArange',
         'ceil': 'from brian2.codegen.generators.numpy_generator import ceil_func as ceil',
         'floor': 'from brian2.codegen.generators.numpy_generator import floor_func as floor',
-        'int': 'from brian2.codegen.generators.numpy_generator import int_func as int',
-        'rand': 'from brian2.codegen.generators.numpy_generator import randn_func as rand',
+        #'int': 'from numpy import int32 as int', # This is being dealt with by the generator.
+        'rand': 'from brian2.codegen.generators.numpy_generator import rand_func as rand',
         'randn': 'from brian2.codegen.generators.numpy_generator import randn_func as randn',
         'poisson': 'from brian2.codegen.generators.numpy_generator import poisson_func as poisson',
+        'exprel': 'from brian2.units.unitsafefunctions import exprel',
         'logical_not': 'from numpy import logical_not',
         'sign': 'from numpy import sign',
         'abs': 'from numpy import abs',
         'sqrt': 'from numpy import sqrt',
         'exp': 'from numpy import exp',
         'log': 'from numpy import log',
         'log10': 'from numpy import log10',
@@ -294,15 +296,15 @@
         'tan': 'from numpy import tan',
         'sinh': 'from numpy import sinh',
         'cosh': 'from numpy import cosh',
         'tanh': 'from numpy import tanh',
         'arcsin': 'from numpy import arcsin',
         'arccos': 'from numpy import arccos',
         'arctan': 'from numpy import arctan',
-        
+        'clip': 'from numpy import clip'   
     }
     
     # Create empty array to collect required imports
     required_imports = []
     # Check if relevant function is in abstract code and if yes, add import
     for func, imp in potential_imports.items():
         for line in abstract_code:
@@ -329,15 +331,15 @@
     proc_model_ports : `string[]`
         A list of code lines that define process model ports
     """
 
     proc_ports = []
     proc_model_ports = []
     # Use the information contained in the objects to format the input and output ports
-    if isinstance(obj, NeuronGroup) or isinstance(obj,SpikeGeneratorGroup):
+    if isinstance(obj, SpikeSource):
         # Add the spikes_out ports, NOTE that the name has to be compatible with the name used
         # in the SpikeMonitor.
         spike_port = obj.name + '_s_out'
         proc_ports.append(f"self.{spike_port} = OutPort(shape= ({obj.N},))")
         proc_model_ports.append(f"{spike_port}: PyOutPort = LavaPyType(PyOutPort.VEC_DENSE, bool, precision=1)")
         for var in self.lava_ports.values():
             if not obj.name == var['receiver']:
@@ -364,17 +366,19 @@
                 proc_ports.append(f"self.{portname}_out = OutPort(shape = {shape_var}.shape)")
                 port_type = 'float' if not 'idx' in portname else 'int,precision = 1'
                 proc_model_ports.append(f"{portname}_out: PyOutPort = LavaPyType(PyOutPort.VEC_DENSE, {port_type})")
 
     # If there are aliases of the same variable, make sure to initialize them only once
     proc_ports = list(set(proc_ports))
     # Add a return just to make the code slightly cleaner
-    proc_ports[-1] += '\n'
+    if len(proc_ports):
+        proc_ports[-1] += '\n'
     proc_model_ports = list(set(proc_model_ports))
-    proc_model_ports[-1] += '\n'
+    if len(proc_model_ports):
+        proc_model_ports[-1] += '\n'
 
     return proc_ports, proc_model_ports
 
 
 def get_lava_proc_variables(self, obj, lava_init_function_calls):
     """
     Takes variable name/value pairs and generates a list of variables
@@ -483,88 +487,70 @@
     Returns
     -------
     init_calls : `string[]`
         A list of code that describes methods for the `process`
     run_calls : `string[]`
         A list of code that describes methods for the `process model`
     """
-    init_calls_lists = {}
-    init_calls = {}
     run_calls = []
-    multi_var_init_calls = []
+    init_calls = []
+    lrn_calls = []
 
     # Collect code objects for process
     code_objects = [c_o for c_o in list(self.code_objects.values()) if c_o.owner.name == obj.name]
 
     # Iterate over all code blocks and code objects
     # NOTE: The after_run code blocks are not really used at any point yet. 
     # FIXME: I take them out for now, because their behavior should be implemented differently!
     for block in ['_before_run()', '_run()']:
         for code_obj in code_objects:
             # If the codeobject is not empty, assign function names to related lists
             if code_obj.compiled_code[block[1:-2]] is not None:
                 function_name = f'self.{code_obj.name}{block}'
-                # Currently added synapses_create_array to the init functions because I believe we should only call it once.
-                #if 'group_variable_set_conditional' in code_obj.name or block == '_before_run()' or 'synapses_create_array' in code_obj.name: 
-                # # TODO: Here we might have to make sure that the 'group_...' gets added to index 0
-                #    init_calls.append(function_name)
                 # These functions are added to the lava process and initialize variables
                 if code_obj.template_name in self.init_template_functions:
-                    # Get variable that will be initialized in process
-                    var_name = self.init_variables[code_obj.name]
-                    # TODO: this can for sure be done more cleanly, but for now it suffices, check synapses.py to see why this works
-                    if isinstance(var_name,str):
-                        # If variable was not already added to list, just add it    
-                        if var_name not in init_calls_lists:
-                            init_calls_lists[var_name] = [function_name]
-                        # If variable was already added to list, append it to the existing item
-                        else:
-                            init_calls_lists[var_name].append(function_name)
-                    else:
-                        multi_var_init_calls.append(function_name)
+                    init_calls.append(function_name)
+                elif code_obj.template_name == 'synapses':
+                    lrn_calls.append(function_name)
                 # These functions handle the simulation and are part of the lava process model
                 else:
                     run_calls.append(function_name)
     run_calls = schedule_sort(run_calls, obj)
 
-    # Postprocess init calls
-    for key, values in init_calls_lists.items():
-        # If we have only one init function for the variable, just take it
-        if len(values) == 1:
-            init_calls[key] = values[0]
-        # If we have two or more init functions for the variable,
-        # we need to construct a lambda function that calls all init functions
-        else:
-            # Starting string definition for lambda function that calls all functions
-            st = '(lambda: ['
-            suffix = '])()[-1]'
-            # Iteratively add all function calls as string
-            for i, v in enumerate(values):
-                st += f'{v}'
-                if (i+1) < len(values):
-                    st += ', '
-            # Add suffix and add to init calls
-            st += suffix
-            init_calls[key] = st
+    # # Postprocess init calls
+    # for key, values in init_calls_lists.items():
+    #     # If we have only one init function for the variable, just take it
+    #     if len(values) == 1:
+    #         init_calls[key] = values[0]
+    #     # If we have two or more init functions for the variable,
+    #     # we need to construct a lambda function that calls all init functions
+    #     else:
+    #         # Starting string definition for lambda function that calls all functions
+    #         st = '(lambda: ['
+    #         suffix = '])()[-1]'
+    #         # Iteratively add all function calls as string
+    #         for i, v in enumerate(values):
+    #             st += f'{v}'
+    #             if (i+1) < len(values):
+    #                 st += ', '
+    #         # Add suffix and add to init calls
+    #         st += suffix
+    #         init_calls[key] = st
 
     # If in any of our code objects there's a time variable (probably always)
     # Add a line to update at each time step
-    time_update_set = False
-    timestep_update_set = False
-    for code_obj in code_objects:
-        code_obj_varnames = code_obj.variables.keys()
-        if 't' in code_obj_varnames and not time_update_set:
-            # TODO: this has to be made more generalizable to multiple clocks
-            run_calls.append('self._defaultclock_t += self._defaultclock_dt')
-            time_update_set = True
-        if 't_in_timesteps' in code_obj_varnames and not timestep_update_set:
-            run_calls.append('self._defaultclock_timestep += 1')
-            timestep_update_set = True
+    obj_varnames = obj.variables.keys()
+    if 't' in obj_varnames:
+        # TODO: this has to be made more generalizable to multiple clocks
+        run_calls.append('self._defaultclock_t += self._defaultclock_dt')
+    if 't_in_timesteps':
+        run_calls.append('self._defaultclock_timestep += 1')
+    
 
-    return init_calls, multi_var_init_calls, run_calls
+    return init_calls, run_calls, lrn_calls
 
 
 def schedule_sort(func_list, obj):
     """
     TODO
 
     Parameters
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/device/run.py` & `brian2lava-1.0.0a2/brian2lava/device/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 from brian2.synapses.synapses import Synapses
 from brian2.units import second
 
 from lava.magma.core.run_configs import Loihi1SimCfg
 from lava.magma.core.run_conditions import RunSteps
 from lava.proc.monitor.process import Monitor
 
-from pprint import pprint
-
-
 def network_run(
         self,
         net,
         duration,
         report=None,
         report_period=10 * second,
         namespace=None,
@@ -86,14 +83,15 @@
     # Set current time to end time (FIXME why? and whyt is the difference between self.t and self.t_?)
     # NOTE by carlo: self.t is with unit, self.t_ is without unit
     net.t_ = float(t_end)
 
     # Gets the number of neurons for the neuron group
     # FIXME this currenty assumes only *one* NeuronGroup
     #       If multiple neuron groups are present, this needs to be changed
+    # NOTE Francesco: Is this needed for anything?
     for obj in net.objects:
         if isinstance(obj, NeuronGroup):
             self.N = obj._N
     
     # FIXME Taken from CPPStandaloneDevice, but unclear what it means
     # In the CPP device it is noted that this is a hack
     # https://github.com/brian-team/brian2/blob/master/brian2/devices/cpp_standalone/device.py#L1404
@@ -101,24 +99,26 @@
         if clock.name == 'clock':
             clock._name = '_clock'
     
     # Collect code objects from network objects
     # Right now these lines don't really do anything since we're never referencing the 
     # variable code_objects again in this method
     code_objects = []
-    self.lava_objects = []
+    self.lava_objects = {}
     for obj in net.sorted_objects:
         # FIXME: Is this required? What does obj.active actually do?
         if obj.active:
             # These are (currently) the only BrianObjects that generate their own process
             # NOTE: This must be changed when implementing other Brian classes
             if any([isinstance(obj,supp_obj) for supp_obj in self.supported_processes]):
-                self.lava_objects.append(obj)
+                self.lava_objects[obj.name] = obj
             for codeobj in obj._code_objects:
+                # NOTE: For code cleanup, this is never actually used anywhere. Interesting that they save the objects as tuples of (clock,object)
                 code_objects.append((obj.clock, codeobj))
+    
 
     # FIXME This may require an update, similar to how CPPStandalone handles the report
     # https://github.com/brian-team/brian2/blob/master/brian2/devices/cpp_standalone/device.py#L1465
     #if report is not None:
     #    report_period = float(report_period)
     #    next_report_time = start_time + report_period
     #    if report == 'text' or report == 'stdout':
@@ -141,14 +141,15 @@
     # that seems to generate some basic code lines ...
 
     #for a in self.arrays:
     #    if (a.name == 't') and isinstance(a.owner, Clock):
     #        print(a.get_value())
     
     # Call network after_run method
+    # NOTE: Is this supposed to be here? Why not after calling the build function? 
     net.after_run()
     
     # Call build method
     if self.build_on_run:
         if self.did_run:  # FIXME necessary?
             raise RuntimeError("The network has already been built and run "
                                "before. Use set_device with "
@@ -172,19 +173,29 @@
     device = get_device()
     # Raise an error if the user is trying to implement unsupported objects
     objects = []
     for obj in net.sorted_objects:
         if any([isinstance(obj,unsupp_obj) for unsupp_obj in device.unsupported_processes]):
             obj_type = type(obj).__name__
             objects.append(obj_type)
+        for contained_obj in obj.contained_objects:
+            if any([isinstance(contained_obj,unsupp_obj) for unsupp_obj in device.unsupported_processes]):
+                obj_type = type(contained_obj).__name__
+                objects.append(obj_type)
+        if isinstance(obj, Synapses):
+            for pathway in obj._pathways:
+                if len(pathway.delay.variable.get_value()):
+                    objects.append("Delay in Synapses")
+                    break
+            
         
     if len(objects):
         objects_repr = '\n\t\t'.join(objects)
         msg = f"""
-        The following objects are not supported by brian2lava, yet:
+        The following objects or functionalities are not supported by brian2lava, yet:
                 {objects_repr}
         You can expect them in future releases. You can also ask for features 
         on the official brian2lava repo on GitLab:
         https://gitlab.com/brian2lava/brian2lava/-/tree/main
         """
         raise NotImplementedError(msg)
         
@@ -211,21 +222,19 @@
     compiled_processes = {}
     for name in names:
         exec(open(f'{directory}/{name}_process.py').read(), globals())
         exec(open(f'{directory}/{name}_process_model.py').read(), globals())
     
         exec(f"compiled_processes['{name}'] = {name}_P(name = '{name}')")
     
-    # Get instance of the process
-    # NOTE Linting assumes that 'Process' is not defined it does not
-    #      understand that it comes from the exec above
-    return compiled_processes  # noqa: F821
+    # Get instance of the processes
+    return compiled_processes 
 
 
-def run(self):
+def run_processes(self):
     """
     Executes the Lava simulation.
 
     We first compile the templates, initialize Lava and add configured monitors.
     Finally, the compiled Lava code is executed and monitor data is extracted.
     """
     
@@ -233,46 +242,59 @@
     # NOTE import seems not to work at the moment, exec works
     #import sys
     #sys.path.append(self.project_dir)
     #from process_model import ProcessModel
     #from process import Process
     
     # Compile templates
-    processes = compile_templates(self.project_dir, [obj.name for obj in self.lava_objects])
+    processes = compile_templates(self.project_dir, [obj for obj in self.lava_objects])
 
     
     # NOTE adding one step is necessary such that spikes are evaluated
     #      correctly by Lava and match Brian results
     num_steps = int(self.duration/self.defaultclock.dt) + 1
 
     # First initialize the monitors
     for process in processes.values():
         self.init_lava_monitors(process, num_steps)
-    
+
     # Connect the ports of connected processes
     self.connect_lava_ports(processes)
     root_processes = self.select_root_processes(processes)
     # Log that the run method was called
-    self.logger.diagnostic(f'Run Lava simulation for {self.duration} ({num_steps} steps)')
-    print(f'Run Lava simulation for {self.duration} ({num_steps} steps)')
+    self.logger.diagnostic(f'Running Lava simulation for {self.duration} ({num_steps} steps)')
+    print(f'Running Lava simulation for {self.duration} ({num_steps} steps)')
     
     # Run the simulation
     for process in root_processes:
         self.logger.debug(f"Running process: {process.name}")
         # Prepare simulation
         run_cfg = Loihi1SimCfg()
         process.run(condition=RunSteps(num_steps=num_steps), run_cfg=run_cfg)
 
+    self.logger.debug("Successfully run simulation")
+
     # After running the simulation, copy the monitored values from all the processes to brian
     for process in processes.values():
         # Set monitor values
         self.set_brian_monitor_values(process)
-    
+
+    self.logger.debug("Successfully retrieved monitor values")
+
+    # Update the class attributes of BrianObjects, so that the user can get their values normally.
+    self.update_brian_class_attributes(processes)
+
+    # Stop processes to terminate execution
+    for process in root_processes:
+        process.stop()
+
     # Indicate that the network simulation did run
     self.did_run = True
+    for process in processes.values():
+        del process
 
 
 def connect_lava_ports(self, processes):
     """
     Connect the ports of the connected processes.
 
     Parameters
@@ -383,144 +405,224 @@
 
     return root_nodes
 
 
 def init_lava_monitors(self, process, num_steps):
     """
     Initializes monitors, defined by the user in Brian.
+    In case a monitor has additional variables to be monitored, the function this method wraps 
+    is called recursively.
 
     Parameters
     ----------
     process : `Process`
         Lava process that is provided with a monitor
     num_steps : `int`
         Number of steps for which the monitor shall be active
 
     Notes
     -----
     Each probed Lava variable can be assigned to multiple monitors defined in Brian.
     E.g. time can be necessary for a state and a spike monitor, while time is only probed once from Lava.
     """
-    # TODO: This might not be the best way to do this, but it ensures that no extra monitors are created
-    # and that they are associated with the correct 'sources' only. Probably we could find a more efficient way to do this.
-    for m in self.lava_monitors.values():
-        # Only look at the right monitors
-        if not process.name == m['source']:
-            continue
 
+    def init_lava_monitor(m,num_steps):
+        """
+        We define this extra method because it can be called recursively for additional variables
+        """
         # If you find a process which should be monitored, look at which variable should be monitored
         lava_var_name = m['lava_var_name']
 
         # If the given process does not have the required variable, raise an error
         # This should never happen, but just for debugging I'll leave it for now
         if not hasattr(process,lava_var_name):
-            raise ValueError(f"Something went wrong: the process {process} does not have the variable {lava_var_name} required from the monitor")
+            raise ValueError(f"Something went wrong: the process {process.name} does not have the variable {lava_var_name} required from the monitor")
         
         
         # NOTE Lava allows only one monitor per variable, so we only create one if one was not already created
         try:
             # Init Lava monitor and define probe for variable
             monitor = Monitor()
             monitor.probe(getattr(process, lava_var_name), num_steps)
+            # Allow probing of additional variables for spike monitors
+            for additional_monitor in m['additional_var_monitors']:
+                init_lava_monitor(additional_monitor, num_steps)
+
         # If the monitor already exists, lava throws an AssertionError
         except AssertionError:
             # If that's the case, we look for the monitor in the previously defined monitors
             for k in self.lava_monitors.values():
                 if not k['lava_monitor'] is None and k['source'] == m['source'] and m['lava_var_name'] == k['lava_var_name']:
                     monitor = k['lava_monitor']
+                    break
+            if monitor == None: raise AssertionError(f"Something went wrong: the monitor for {m['source']} and {m['lava_var_name']} was not found")
+
         m['lava_monitor'] = monitor
+        # Note that for the spike monitor additional variables this is not set,
+        # which means that it will be skipped in the set_brian_monitor_values function
         m['process_name'] = getattr(process, 'name')
 
+    # TODO: This might not be the best way to do this, but it ensures that no extra monitors are created
+    # and that they are associated with the correct 'sources' only. Probably we could find a more efficient way to do this.
+    for m in self.lava_monitors.values():
+        # Only look at the right monitors
+        if not process.name == m['source']:
+            continue
+        init_lava_monitor(m, num_steps)
+
 
 def set_brian_monitor_values(self, process):
     """
     Transform Lava monitors to Brian monitor format.
 
     Parameters
     ----------
     process : `Process`
         Lava process that is provided with a monitor
     """
 
     # Iterate over Lava monitors
     for k, m in self.lava_monitors.items():
+
         # Only do this if the monitor refers to this process
         if not getattr(process,"name") == m['process_name']:
             continue
+
         # Get monitor variable
         var = m['var']
 
         # Define empty data variable
         # NOTE Lava monitors do not probe the inital values while Brian does
         #      We need to manually prepend the initial values to the monitored data
         init_data = None  # Contains initial values
         data = None  # Contains all other values
 
         # In case of a spike monitor, we need a more specific handling to get the time/spike indices
         if m['type'] == self.monitor_types['spike']:
-
-            if var.name == 't':
-                # Find monitor that contains 'i' variable
-                spike_monitor_name = f'_spike_{var.owner.name}_i'
-                spike_monitor = self.lava_monitors[spike_monitor_name]
-                # Get raw data from Lava monitor
-                raw = get_monitor_values(spike_monitor)
-                # Transform data to get actual spike times
-                data = (np.nonzero(raw)[0] * self.defaultclock.dt) - self.defaultclock.dt
-
+            if var.name == 'i':
                 # Get initial values from process
                 init_raw = getattr(process, f'_{getattr(process,"name")}__spikespace').init
-                # Transform data to get actual spike times
-                init_data = np.nonzero(init_raw)[0] * self.defaultclock.dt
+                i_init_data = np.nonzero(init_raw)[0]
+                t_init_data = np.nonzero(init_raw)[0]*self.defaultclock.dt
 
-            if var.name == 'i':
-                # Get raw data from Lava monitor
+                # Get the data from the monitor, for both i and t the data is the same
                 raw = get_monitor_values(m)
-                # Make sure that we always have two dimensions
-                if np.ndim(raw) == 1:
-                    raw = [raw]
-                # Transform data to get indices
-                data = np.nonzero(raw)[1]
+                t_data = (np.nonzero(raw)[1] * self.defaultclock.dt)
 
-                # Get initial values from process
-                init_raw = getattr(process, f'_{getattr(process,"name")}__spikespace').init
-                # Transform initial data to get indices
-                init_data = np.nonzero(init_raw)[0]
+                # Format it correctly
+                t_data = np.concatenate((t_init_data, t_data))
+                i_data = np.concatenate((i_init_data,np.nonzero(raw)[0]))
+                count = np.bincount(i_data,minlength = m['var'].owner.source.N)
+                
+                # Store the monitor data into the device arrays
+                self.arrays[var] = i_data
+                self.arrays[var.owner.variables["t"]] = t_data
+                self.arrays[var.owner.variables['count']] = count
+                for additional_monitor in m['additional_var_monitors']:
+                    # New variable to update in the arrays
+                    add_var = additional_monitor['var']
+                    data = get_monitor_values(additional_monitor)[:,:-2]
+                    # Get initial values from process
+                    init_data = getattr(process, additional_monitor['lava_var_name']).init
+                    init_data = init_data.reshape(init_data.shape[0], 1)
+                    # Select only the correct time points for the spiking neurons
+                    data = np.concatenate((init_data, data), axis=1)[i_data,np.nonzero(raw)[1]]
+                    self.arrays[add_var] = data
 
         # In case of a state monitor, just take the raw data from Lava
         if m['type'] == self.monitor_types['state']:
-            # NOTE remove additional simulation steps from monitor to match Brian simulation
-            data = get_monitor_values(m)[:-2]
 
+            # NOTE remove additional simulation steps from monitor to match Brian simulation
+            data = get_monitor_values(m)[:,:-2]
+            
             # Get initial values from process
             init_data = getattr(process, m['lava_var_name']).init
 
-        # Get dimension of data array
-        dim = np.ndim(data)
-
-        # Append init values and store data in related array variable
-        if dim == 1:
-            self.arrays[var] = np.append(init_data, data)
-
-        if dim == 2:
-            self.arrays[var] = np.append([init_data], data, axis=0)
+            if len(init_data) > 0:
+                init_data = init_data.reshape(init_data.shape[0], 1)
+                data = np.concatenate((init_data, data), axis=1)
+        
+            # Just formatting to make sure that we always have two dimensions
+            # as used in brian for state monitor values (only for variables other than time)
+            if var.name == 't':
+                self.arrays[var] = np.squeeze(data)
+                continue
 
+            # Manage other variables
+            if np.ndim(data) == 1:
+                data = np.array([data])
+
+            # If record is set to some specific indices, we only store the data at those indices
+            # Note that this is very inefficient, but in Lava it's impossible to select indices
+            # to record from a monitor. This is only to keep the results consistent with Brian.
+            if isinstance(m['indices'],np.ndarray):
+                # This case happens for variables that were not defined before calling the run() method
+                if m['indices'].shape == (0,):
+                    m['indices'] = np.arange(len(data))
+                data = data[m['indices']]
+
+            # In brian, by design, the __getattr__ from StateMonitors will transpose the data before returning it (but not for the time variable)
+            # So here we transpose one additional time to account for this.
+            # Found it: see https://github.com/brian-team/brian2/blob/master/brian2/monitors/statemonitor.py#L378
+            # It seems that this is done by design.. https://brian.discourse.group/t/how-to-get-all-data-from-all-monitors/302/4
+            self.arrays[var] = np.transpose(data)
 
 def get_monitor_values(monitor):
     """
     Get data from a Lava monitor.
 
     Parameters
     ----------
     monitor
         A monitor as defined in the device
     """
+
     # Define variables
     lava_monitor = monitor['lava_monitor']
     lava_var_name = monitor['lava_var_name']
     process_name = monitor['process_name']
+    
+
     # Return lava monitor values
-    # TODO we need to find out how Lava processes are numbered, 'Process_0'
-    #      is probably not generalizing for more than one process
-    # NOTE: SHOULD BE FIXED NOW!
     data = lava_monitor.get_data()[process_name][lava_var_name]
-    return np.squeeze(np.array(data))
+    data = np.transpose(np.array(data))
+
+    return data
+
+
+def update_brian_class_attributes(self,processes):
+    """
+    Update class attributes of Brian objects.
+    This allows the user to access attributes of Brian objects as they would in normal Brian.
+    We do this by going through the processes and finding their corresponding Brian objects.
+    Then we update the 'array' variable of the device with the new values so that when get_value gets called
+    the correct values are displayed.
+    Args:
+        processes: List of Lava processes
+    """
+    self.logger.debug("Updating Brian class attributes..")
+    # Iterate over processes
+    for p in processes.values():
+        obj = self.lava_objects[p.name]
+        for varname,var in obj.variables.items():
+            p_varname = self.get_array_name(var,prefix = None)
+
+            if hasattr(p,p_varname):
+                # NOTE: These next 2 lines are useful for fixing the reinit() issue.
+                # if "synaptic_pre" in p_varname or "synaptic_post" in p_varname:
+                #     print(p_varname, getattr(p,p_varname).get())
+
+                # This should almost never happen but sometimes some simulation 
+                # settings can produce arrays with length 0. We ignore these.
+                if getattr(p,p_varname).shape == (0,):
+                    self.logger.debug(f"Array {p_varname} has length 0, ignoring..")
+                    continue
+
+                dtype = var.dtype
+                self.arrays[var] = np.array(getattr(p,p_varname).get(), dtype=dtype)
+                    
+
+        if isinstance(obj, Synapses):
+            # Update the variables counting the number of synapses
+            # TODO: Verify that this is not needed during the simulation
+            # as right now we only update these variables AFTER running a simulation..
+            obj._update_synapse_numbers(0)
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/device/synapses.py` & `brian2lava-1.0.0a2/brian2lava/device/synapses.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from brian2.utils.logger import get_logger
 from brian2.utils.stringtools import get_identifiers, word_substitute
 from brian2.utils.arrays import calc_repeats
 from brian2.core.spikesource import SpikeSource
 from brian2.synapses.parse_synaptic_generator_syntax import parse_synapse_generator
 from brian2.parsing.bast import brian_ast
 from brian2.parsing.rendering import NodeRenderer
+from brian2 import Synapses, Function
 MAX_SYNAPSES = 2147483647
 
 
 def spike_queue(self, source_start, source_end):
     """
     TODO
 
@@ -109,15 +110,16 @@
         A namespace that will be used in addition to the group-specific
         namespaces (if defined). If not specified, the locals
         and globals around the run function will be used.
     level : int, optional
         How deep to go up the stack frame to look for the locals/global
         (see ``namespace`` argument).
     """
-
+    # First, add the spiking synapses variable to the lava_variables
+    self._add_spiking_synapses_vars(synapses)
     # Check types
     synapses._verify_connect_argument_types(condition, i, j, n, p)
 
     synapses._connect_called = True
 
     # Get namespace information
     if namespace is None:
@@ -132,61 +134,106 @@
             if i is not None or j is not None:
                 raise ValueError("Cannot combine condition with i or j "
                                     "arguments")
             if condition is False or condition == 'False':
                 # Nothing to do
                 return
             j = synapses._condition_to_generator_expression(condition, p, namespace)
-            print("Using synapses generator")
+            self.logger.debug("Using synapses from generator")
             synapses._add_synapses_generator(j, n, skip_if_invalid=skip_if_invalid,
                                             namespace=namespace, level=level + 2,
                                             over_presynaptic=True)
         # 2: connection indices
         elif (i is not None and j is not None) and not (isinstance(i, str) or isinstance(j, str)):
             if skip_if_invalid:
                 raise ValueError("Can only use skip_if_invalid with string "
                                     "syntax")
             i, j, n = synapses._verify_connect_array_arguments(i, j, n)
+            self.logger.debug("Using synapses from arrays")
             synapses._add_synapses_from_arrays(i, j, n, p, namespace=namespace)
         # 3: Generator expression over post-synaptic cells (i='...')
         elif isinstance(i, str):
             i = synapses._finalize_generator_expression(i, j, p, 'i', 'j')
+            self.logger.debug("Using synapses from generator")
             synapses._add_synapses_generator(i, n, skip_if_invalid=skip_if_invalid,
                                             namespace=namespace, level=level + 2,
                                             over_presynaptic=False)
         # 4: Generator expression over pre-synaptic cells (i='...')
         elif isinstance(j, str):
             j = synapses._finalize_generator_expression(j, i, p, 'j', 'i')
+            self.logger.debug("Using synapses from generator")
             synapses._add_synapses_generator(j, n, skip_if_invalid=skip_if_invalid,
                                             namespace=namespace, level=level + 2,
                                             over_presynaptic=True)
         else:
             raise ValueError("Must specify at least one of condition, i or "
                                 "j arguments")
     except IndexError as e:
         raise IndexError("Tried to create synapse indices outside valid "
                             "range. Original error message: " + str(e))
-    # Do some refactoring of the synapses code to adapt it to Lava API:
-    # FIXME: Probably this will be useless, but I'll wait before deleting it since it does no harm here for now.
-    self.add_lava_synapses_generator(synapses)
 
 
-def add_lava_synapses_generator(self, synapses):
+def _add_spiking_synapses_vars(self,synapses):
+    """
+    Adds a variable to the lava_variables which will store the spiking synapses from the last
+    timestep. The vector is then used to update the synaptic variables in the run_lrn function if
+    the synapses are plastic.
     """
-    A helper function to correctly tell lava which synaptic variables will be
-    initialized through this generator codeobject.
+    
+    for pathway in synapses._pathways:
+        prepost = pathway.prepost
+        name = f"lava_spiking_synapses_{prepost}"
+        size = 1
+
+        # This needs to be a dynamic array as its shape will change during the simulation
+        synapses.variables.add_dynamic_array(name,size,dtype = "int")
+
+        # Register this variable so that it will be correctly resized during the initialization.
+        synapses.register_variable(synapses.variables[name])
+
+
+def determine_lava_ports(self, pathway, variables):
+    """
+    Extracts the synaptic variables to be sent to the neurongroups and determine the Lava ports required for that.
 
     Parameters
     ----------
-    synapses : `Synapses`
-        An instance of the `Synapses` class
-
-    Notes
-    -----
-    At the moment I'm using a trick, which just adds a random int, used in build() to determine that this codeobject
-    initializes multiple variables. In the future this should be changed: either expanded if the variables themselves
-    are needed, or replaced by something more elegant.
-    """
-    # Extract the generator codeobj from the device's code_objects
-    # TODO: This is not clean and should be handled in a different way.
-    generator_codeobj = [self.code_objects[name] for name in self.code_objects if ('synapses_create' in name and self.code_objects[name].owner == synapses)][-1]
-    self.init_variables[generator_codeobj.name] = 123
+    pathway
+        Synaptic pathways.
+    variables
+        The variables contained in the code used by the pathway.
+    """
+    # Support for subgroups will come in the future
+    if 'subgroup' in pathway.source.name or 'subgroup' in pathway.target.name:
+        msg = f"""
+        Encountered a Subgroup object in the connection from {pathway.source.name} to {pathway.target.name}.
+        Subgroups are not supported yet. Subgroups are defined by indexing a NeuronGroup (e.g. P = NG[0:10]).
+        If you are using this method to connect synapses we suggest using alternative methods such as
+        the expression S.connect('i<10',p = p), which has been tested.
+        """
+        raise NotImplementedError(msg)
+    synaptic_vars = []
+    # TODO: this is probably not needed in case the update only requires synaptic variables,
+    # then you wouldn't need to send them to the neuronGroup. But for now let's just make
+    # the easiest scenario
+    for varname,var in variables.items():
+        if isinstance(var, Function) or not isinstance(var.owner, Synapses):
+            continue
+        synaptic_vars.append(varname)
+
+    # Var names are kept in their original form, but the ports are separated depending on the pathway
+    for varname in synaptic_vars:
+        portname = pathway.synapses.name +'_'+ pathway.prepost +'_'+ varname
+        self.lava_ports[portname] = {
+            'varname': varname, # Required by code generation
+            'portname': portname,
+            'pathway': pathway,
+            'sender' : pathway.source.name,
+            'receiver': pathway.target.name
+        }
+
+    ports = '\n\t'.join([port  for port in self.lava_ports])
+    msg = f"""Saved ports for synaptic transmission from synapses {pathway.synapses.name} to {pathway.target.name}:
+    Ports required:
+    {ports}
+    """
+    self.logger.diagnostic(msg)
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/device/variables.py` & `brian2lava-1.0.0a2/brian2lava/device/variables.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,22 +39,39 @@
     run_namespace : dict-like, optional
         An additional namespace that is used for variable lookup (if not
         defined, the implicit namespace of local variables is used).
     check_units : bool, optional
         Whether to check the units of the expression.
     """
 
-    # Try to cast code to value
-    value = None
-    try:
-        value = int(code)
-    except:
-        raise NotImplementedError('Defining variables as expressions is currently not supported. For more information: https://gitlab.com/tetzlab/brian2lava/-/issues/19')
-    # Update array variable
-    self.fill_with_array(variableview.variable, value)
+    variable = variableview.variable
+    if variable.scalar and cond != "True":
+        raise IndexError(
+            f"Cannot conditionally set the scalar variable '{variableview.name}'."
+        )
+    abstract_code_cond = f"_cond = {cond}"
+    abstract_code = f"{variableview.name} = {code}"
+    variables = Variables(None)
+    variables.add_auxiliary_variable("_cond", dtype=bool)
+    from brian2.codegen.codeobject import create_runner_codeobj
+
+    # TODO: Have an additional argument to avoid going through the index
+    # array for situations where iterate_all could be used
+
+    create_runner_codeobj(
+        variableview.group,
+        {"condition": abstract_code_cond, "statement": abstract_code},
+        "group_variable_set_conditional",
+        additional_variables=variables,
+        check_units=check_units,
+        run_namespace=run_namespace,
+        codeobj_class=self.code_object_class(
+            fallback_pref="codegen.string_expression_target"
+        ),
+    )
 
 
 def variableview_set_with_expression(self, variableview, item, code, run_namespace, check_units=True):
     """
     Sets a variable using a string expression. Is called by `VariableView.set_item` for statements such as
     ``S.var[:, :] = 'exp(-abs(i-j)/space_constant)*nS'``.
 
@@ -131,30 +148,23 @@
     # Add group idx variable
     # This function is part of the Variables class, but also calles get_array_name at some point
     variables.add_array(idx_name, size=len(indices), dtype=np.int32, values=indices)
 
     # Add the new group idx name to an array (needed for the counter)
     self.set_variable_index_names.append(variables._variables[idx_name])
 
-    # Store method name and lava variable name in init variables
-    # and set the current method name as last-used name (needed for the code object to identify the method name)
-    method_name = f'{variableview.group_name}_group_variable_set_{counter}_{variableview.name}'
-    lava_variable_name = self.get_array_name(variableview.variable, prefix='')
-    self.init_variables[method_name] = lava_variable_name
-    self.last_set_variable_method_name = method_name
-
     # Needs to be added to namespace, since group still requires the original name '_group_idx'
     # The specific reason for that is unknown ;)
     run_namespace['_group_idx'] = variables._variables[idx_name]
 
     # TODO: Have an additional argument to avoid going through the index
     # array for situations where iterate_all could be used
     from brian2.codegen.codeobject import create_runner_codeobj
 
-    codeobj = create_runner_codeobj(
+    create_runner_codeobj(
         variableview.group,
         abstract_code,
         "group_variable_set",
         additional_variables=variables,
         check_units=check_units,
         run_namespace=run_namespace,
         codeobj_class=self.code_object_class(
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/device/writer.py` & `brian2lava-1.0.0a2/brian2lava/device/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,7 +48,8 @@
     self.logger.diagnostic(f'{name}_process.py stored in working directory.')
     
     # Write 'process model' to working directory
     writer.write(f'{name}_process_model.py', process_model_rendered)
     
     # Log that process_model.py was stored
     self.logger.diagnostic(f'{name}_process_model.py stored in working directory.')
+
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/templates/process.py.j2` & `brian2lava-1.0.0a2/brian2lava/templates/process.py.j2`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         
         # Initialize variables using numpy expressions
         {% for va in variables_init %}
         {{ va }}
         {% endfor %}
 
         # Call the methods required for variable initialization
-        {% for c in multi_init_calls %}
+        {% for c in init_calls %}
         {{c}}
         {% endfor %}
 
         # Initialize variables using lava expressions
         {% for va in variables_lava %}
         {{ va }}
         {% endfor %}
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/templates/process_model.py.j2` & `brian2lava-1.0.0a2/brian2lava/templates/process_model.py.j2`

 * *Files 12% similar despite different names*

```diff
@@ -23,32 +23,35 @@
     {% endfor %}
 
     def __init__(self, proc_params: ty.Optional["ProcessParameters"] = None):
         super().__init__(proc_params=proc_params)
 
         self.has_init_run = False
 
-    #def run_init(self):
-    #    # Calling required init functions
-    #    {% for fc in init_functions %}
-    #    {{ fc }}
-    #    {% endfor %}
-    #    self.has_init_run = True
 
     def run_spk(self):
 
-        # Run init method before the first step is executed
-        #if not self.has_init_run:
-        #    self.run_init()
-
         # Calling the methods that are executed in every time step
         {% for rf in run_functions %}
         {{ rf }}
         {% endfor %}
 
+    {% if  'synapses' in name  and lrn_functions|length >= 1 %}
+
+    def lrn_guard(self) -> bool:
+        return True
+
+    def run_lrn(self):
+        {%for lf in lrn_functions %}
+        {{ lf }}
+        {% endfor %}
+
+    {% endif %}
+    
+
 
     
     {% for m in methods %}
     {{ m }}
     {% endfor%}
```

### Comparing `Brian2Lava-1.0.0a1/brian2lava/writer/py.py` & `brian2lava-1.0.0a2/brian2lava/writer/py.py`

 * *Files identical despite different names*

### Comparing `Brian2Lava-1.0.0a1/setup.py` & `brian2lava-1.0.0a2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
-	name='Brian2Lava',
-	version='1.0.0a1',  # consider adding '__version__' to 'brian2lava.__init__.py', but requires unified management of versions
+	name='brian2lava',
+	version='1.0.0a2',  # consider adding '__version__' to 'brian2lava.__init__.py', but requires unified management of versions
 	author='Carlo Michaelis, Francesco Negri, Winfried Oed, Jannik Luboeinski, Andrew Lehr, Tristan Stöber',
 	author_email='carlo.michaelis@gmail.com',
 	packages=['brian2lava', 'brian2lava.device', 'brian2lava.codegen', 'brian2lava.writer'],
 	python_requires='>3.8',
 	url='https://gitlab.com/tetzlab/brian2lava',
 	license='MIT',
 	description='An open source Brian2 interface for the neuromorphic computing framework Lava',
@@ -16,16 +16,16 @@
 		"brian2lava/codegen/templates": ["*.py_"],
 		"brian2lava/templates": ["*.py.j2"]
 	},
     include_package_data=True,
 	install_requires=[
 		"brian2>=2.5.1",
 		"jinja2>=2.7",
-		"numpy==1.23.5",
+		"numpy",
 		"pytest",
 		"scipy",
 		"markupsafe==2.0.1",
-		"lava-nc>=0.6.0",
+		"lava-nc>=0.7.0",
 		"matplotlib",
 		"regex>=2022.10.31"
 	],
 )
```

