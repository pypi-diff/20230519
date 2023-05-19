# Comparing `tmp/butler-connect-0.5.5.tar.gz` & `tmp/butler-connect-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.5.5.tar", last modified: Fri May 19 08:45:51 2023, max compression
+gzip compressed data, was "butler-connect-0.5.6.tar", last modified: Fri May 19 09:42:53 2023, max compression
```

## Comparing `butler-connect-0.5.5.tar` & `butler-connect-0.5.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 08:45:51.169453 butler-connect-0.5.5/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.5.5/LICENSE
--rw-rw-rw-   0        0        0     2228 2023-05-19 08:45:51.168457 butler-connect-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-05-19 08:45:21.000000 butler-connect-0.5.5/README.md
--rw-rw-rw-   0        0        0      738 2023-05-19 08:45:27.000000 butler-connect-0.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 08:45:51.170453 butler-connect-0.5.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 08:45:51.122675 butler-connect-0.5.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 08:45:51.132770 butler-connect-0.5.5/src/butlerConnect/
--rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.5.5/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    18399 2023-05-19 08:44:35.000000 butler-connect-0.5.5/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:45:51.135774 butler-connect-0.5.5/src/butlerDescription/
--rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.5.5/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.5.5/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.5.5/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.5.5/src/butlerDescription/group.py
--rw-rw-rw-   0        0        0     1656 2023-05-12 19:37:09.000000 butler-connect-0.5.5/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:45:51.165927 butler-connect-0.5.5/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     2228 2023-05-19 08:45:51.000000 butler-connect-0.5.5/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-05-19 08:45:51.000000 butler-connect-0.5.5/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 08:45:51.000000 butler-connect-0.5.5/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-05-19 08:45:51.000000 butler-connect-0.5.5/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-05-19 08:45:51.000000 butler-connect-0.5.5/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 09:42:53.661723 butler-connect-0.5.6/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.5.6/LICENSE
+-rw-rw-rw-   0        0        0     2321 2023-05-19 09:42:53.660719 butler-connect-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-05-19 09:41:31.000000 butler-connect-0.5.6/README.md
+-rw-rw-rw-   0        0        0      738 2023-05-19 09:42:37.000000 butler-connect-0.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 09:42:53.661723 butler-connect-0.5.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 09:42:53.629057 butler-connect-0.5.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 09:42:53.632056 butler-connect-0.5.6/src/butlerConnect/
+-rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.5.6/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    18399 2023-05-19 08:44:35.000000 butler-connect-0.5.6/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:42:53.635060 butler-connect-0.5.6/src/butlerDescription/
+-rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.5.6/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.5.6/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.5.6/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.5.6/src/butlerDescription/group.py
+-rw-rw-rw-   0        0        0     1656 2023-05-12 19:37:09.000000 butler-connect-0.5.6/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:42:53.658700 butler-connect-0.5.6/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     2321 2023-05-19 09:42:53.000000 butler-connect-0.5.6/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-05-19 09:42:53.000000 butler-connect-0.5.6/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 09:42:53.000000 butler-connect-0.5.6/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-05-19 09:42:53.000000 butler-connect-0.5.6/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-05-19 09:42:53.000000 butler-connect-0.5.6/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.5.5/LICENSE` & `butler-connect-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.5.5/PKG-INFO` & `butler-connect-0.5.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.5.5
+Version: 0.5.6
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,7 +46,9 @@
 - handling error
 ### 0.5.0
 - adding group-types
 ### 0.5.2
 - adding signalOptionType and groupOptionType with forwardingMQTT
 ### 0.5.5
 - Solving problems on publishing data without connecting dest
+### 0.5.5
+- Solving Problems with createConsumer with same topic an different routing_keys
```

### Comparing `butler-connect-0.5.5/src/butlerConnect/pikaButler.py` & `butler-connect-0.5.6/src/butlerConnect/pikaButler.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.5.5/src/butlerDescription/control.py` & `butler-connect-0.5.6/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.5.5/src/butlerDescription/signal.py` & `butler-connect-0.5.6/src/butlerDescription/signal.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.5.5/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.5.6/src/butler_connect.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.5.5
+Version: 0.5.6
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,7 +46,9 @@
 - handling error
 ### 0.5.0
 - adding group-types
 ### 0.5.2
 - adding signalOptionType and groupOptionType with forwardingMQTT
 ### 0.5.5
 - Solving problems on publishing data without connecting dest
+### 0.5.5
+- Solving Problems with createConsumer with same topic an different routing_keys
```

