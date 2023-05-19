# Comparing `tmp/ducktables-0.1.0.tar.gz` & `tmp/ducktables-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducktables-0.1.0.tar", last modified: Wed May 17 22:57:33 2023, max compression
+gzip compressed data, was "ducktables-0.1.1.tar", last modified: Fri May 19 19:37:24 2023, max compression
```

## Comparing `ducktables-0.1.0.tar` & `ducktables-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-17 22:57:33.821283 ducktables-0.1.0/
--rw-rw-r--   0 mark      (4000) mark      (4000)      210 2023-05-17 22:57:33.821283 ducktables-0.1.0/PKG-INFO
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-17 22:57:33.821283 ducktables-0.1.0/ducktables.egg-info/
--rw-rw-r--   0 mark      (4000) mark      (4000)      210 2023-05-17 22:57:33.000000 ducktables-0.1.0/ducktables.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (4000) mark      (4000)      177 2023-05-17 22:57:33.000000 ducktables-0.1.0/ducktables.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-05-17 22:57:33.000000 ducktables-0.1.0/ducktables.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)      231 2023-05-17 22:57:33.000000 ducktables-0.1.0/ducktables.egg-info/requires.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-05-17 22:57:33.000000 ducktables-0.1.0/ducktables.egg-info/top_level.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)       38 2023-05-17 22:57:33.821283 ducktables-0.1.0/setup.cfg
--rw-rw-r--   0 mark      (4000) mark      (4000)      252 2023-05-17 21:46:31.000000 ducktables-0.1.0/setup.py
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-19 19:37:24.321740 ducktables-0.1.1/
+-rw-rw-r--   0 mark      (4000) mark      (4000)      210 2023-05-19 19:37:24.321740 ducktables-0.1.1/PKG-INFO
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-19 19:37:24.321740 ducktables-0.1.1/ducktables.egg-info/
+-rw-rw-r--   0 mark      (4000) mark      (4000)      210 2023-05-19 19:37:24.000000 ducktables-0.1.1/ducktables.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (4000) mark      (4000)      177 2023-05-19 19:37:24.000000 ducktables-0.1.1/ducktables.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-05-19 19:37:24.000000 ducktables-0.1.1/ducktables.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)      267 2023-05-19 19:37:24.000000 ducktables-0.1.1/ducktables.egg-info/requires.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-05-19 19:37:24.000000 ducktables-0.1.1/ducktables.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)       38 2023-05-19 19:37:24.321740 ducktables-0.1.1/setup.cfg
+-rw-rw-r--   0 mark      (4000) mark      (4000)      252 2023-05-19 19:35:38.000000 ducktables-0.1.1/setup.py
```

