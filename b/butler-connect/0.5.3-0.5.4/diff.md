# Comparing `tmp/butler-connect-0.5.3.tar.gz` & `tmp/butler-connect-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.5.3.tar", last modified: Thu May 18 09:03:43 2023, max compression
+gzip compressed data, was "butler-connect-0.5.4.tar", last modified: Thu May 18 09:14:11 2023, max compression
```

## Comparing `butler-connect-0.5.3.tar` & `butler-connect-0.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 09:03:43.215277 butler-connect-0.5.3/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.5.3/LICENSE
--rw-rw-rw-   0        0        0     2154 2023-05-18 09:03:43.214276 butler-connect-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-05-12 19:39:44.000000 butler-connect-0.5.3/README.md
--rw-rw-rw-   0        0        0      738 2023-05-18 09:03:20.000000 butler-connect-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 09:03:43.215277 butler-connect-0.5.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 09:03:43.186297 butler-connect-0.5.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 09:03:43.189274 butler-connect-0.5.3/src/butlerConnect/
--rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.5.3/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    17963 2023-04-25 15:59:19.000000 butler-connect-0.5.3/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:03:43.192274 butler-connect-0.5.3/src/butlerDescription/
--rw-rw-rw-   0        0        0      207 2023-05-18 09:02:00.000000 butler-connect-0.5.3/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.5.3/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.5.3/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.5.3/src/butlerDescription/group.py
--rw-rw-rw-   0        0        0     1656 2023-05-12 19:37:09.000000 butler-connect-0.5.3/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:03:43.212293 butler-connect-0.5.3/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     2154 2023-05-18 09:03:43.000000 butler-connect-0.5.3/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-05-18 09:03:43.000000 butler-connect-0.5.3/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 09:03:43.000000 butler-connect-0.5.3/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-05-18 09:03:43.000000 butler-connect-0.5.3/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-05-18 09:03:43.000000 butler-connect-0.5.3/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 09:14:11.121684 butler-connect-0.5.4/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0     2154 2023-05-18 09:14:11.116677 butler-connect-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-05-12 19:39:44.000000 butler-connect-0.5.4/README.md
+-rw-rw-rw-   0        0        0      738 2023-05-18 09:13:55.000000 butler-connect-0.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 09:14:11.122679 butler-connect-0.5.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 09:14:11.090817 butler-connect-0.5.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 09:14:11.093813 butler-connect-0.5.4/src/butlerConnect/
+-rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.5.4/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    17963 2023-04-25 15:59:19.000000 butler-connect-0.5.4/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:14:11.101153 butler-connect-0.5.4/src/butlerDescription/
+-rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.5.4/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.5.4/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.5.4/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.5.4/src/butlerDescription/group.py
+-rw-rw-rw-   0        0        0     1656 2023-05-12 19:37:09.000000 butler-connect-0.5.4/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:14:11.114683 butler-connect-0.5.4/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     2154 2023-05-18 09:14:11.000000 butler-connect-0.5.4/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-05-18 09:14:11.000000 butler-connect-0.5.4/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 09:14:11.000000 butler-connect-0.5.4/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-05-18 09:14:11.000000 butler-connect-0.5.4/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-05-18 09:14:11.000000 butler-connect-0.5.4/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.5.3/LICENSE` & `butler-connect-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.5.3/PKG-INFO` & `butler-connect-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.5.3
+Version: 0.5.4
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `butler-connect-0.5.3/pyproject.toml` & `butler-connect-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.5.3"
+version = "0.5.4"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.5.3/src/butlerConnect/pikaButler.py` & `butler-connect-0.5.4/src/butlerConnect/pikaButler.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.5.3/src/butlerDescription/control.py` & `butler-connect-0.5.4/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.5.3/src/butlerDescription/signal.py` & `butler-connect-0.5.4/src/butlerDescription/signal.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.5.3/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.5.4/src/butler_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.5.3
+Version: 0.5.4
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

