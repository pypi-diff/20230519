# Comparing `tmp/psychicapi-0.3.tar.gz` & `tmp/psychicapi-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psychicapi-0.3.tar", last modified: Fri May 19 03:36:36 2023, max compression
+gzip compressed data, was "psychicapi-0.4.tar", last modified: Fri May 19 17:44:40 2023, max compression
```

## Comparing `psychicapi-0.3.tar` & `psychicapi-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 03:36:36.000000 psychicapi-0.3/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      272 2023-05-19 03:36:36.000000 psychicapi-0.3/PKG-INFO
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       41 2023-05-18 20:09:12.000000 psychicapi-0.3/psychicapi/__init__.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     1753 2023-05-18 23:32:28.000000 psychicapi-0.3/psychicapi/psychic.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      154 2023-05-17 05:32:44.000000 psychicapi-0.3/README.md
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      327 2023-05-19 03:36:27.000000 psychicapi-0.3/setup.py
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      272 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/requires.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-05-19 03:36:36.000000 psychicapi-0.3/setup.cfg
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 17:44:40.633012 psychicapi-0.4/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     1759 2023-05-19 17:44:40.628633 psychicapi-0.4/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     1520 2023-05-19 17:42:55.000000 psychicapi-0.4/README.md
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 17:44:40.599245 psychicapi-0.4/psychicapi/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       41 2023-05-18 20:09:12.000000 psychicapi-0.4/psychicapi/__init__.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     1753 2023-05-18 23:32:28.000000 psychicapi-0.4/psychicapi/psychic.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 17:44:40.607410 psychicapi-0.4/psychicapi.egg-info/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     1759 2023-05-19 17:44:40.000000 psychicapi-0.4/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-05-19 17:44:40.000000 psychicapi-0.4/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-05-19 17:44:40.000000 psychicapi-0.4/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-05-19 17:44:40.000000 psychicapi-0.4/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-05-19 17:44:40.000000 psychicapi-0.4/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-05-19 17:44:40.633266 psychicapi-0.4/setup.cfg
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      638 2023-05-19 17:43:25.000000 psychicapi-0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `psychicapi-0.3/psychicapi/psychic.py` & `psychicapi-0.4/psychicapi/psychic.py`

 * *Files identical despite different names*

