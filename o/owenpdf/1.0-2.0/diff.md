# Comparing `tmp/owenpdf-1.0.tar.gz` & `tmp/owenpdf-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owenpdf-1.0.tar", last modified: Fri May 19 03:33:15 2023, max compression
+gzip compressed data, was "owenpdf-2.0.tar", last modified: Fri May 19 07:32:24 2023, max compression
```

## Comparing `owenpdf-1.0.tar` & `owenpdf-2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 owenzheng   (501) staff       (20)        0 2023-05-19 03:33:15.913008 owenpdf-1.0/
--rw-r--r--   0 owenzheng   (501) staff       (20)    35148 2023-05-19 03:27:35.000000 owenpdf-1.0/LICENSE
--rw-r--r--   0 owenzheng   (501) staff       (20)      109 2023-05-19 03:33:15.912874 owenpdf-1.0/PKG-INFO
--rw-r--r--   0 owenzheng   (501) staff       (20)       37 2023-05-19 03:21:37.000000 owenpdf-1.0/README.md
-drwxr-xr-x   0 owenzheng   (501) staff       (20)        0 2023-05-19 03:33:15.912733 owenpdf-1.0/owenpdf.egg-info/
--rw-r--r--   0 owenzheng   (501) staff       (20)      109 2023-05-19 03:33:15.000000 owenpdf-1.0/owenpdf.egg-info/PKG-INFO
--rw-r--r--   0 owenzheng   (501) staff       (20)      150 2023-05-19 03:33:15.000000 owenpdf-1.0/owenpdf.egg-info/SOURCES.txt
--rw-r--r--   0 owenzheng   (501) staff       (20)        1 2023-05-19 03:33:15.000000 owenpdf-1.0/owenpdf.egg-info/dependency_links.txt
--rw-r--r--   0 owenzheng   (501) staff       (20)        1 2023-05-19 03:33:15.000000 owenpdf-1.0/owenpdf.egg-info/top_level.txt
--rw-r--r--   0 owenzheng   (501) staff       (20)       38 2023-05-19 03:33:15.913048 owenpdf-1.0/setup.cfg
--rw-r--r--   0 owenzheng   (501) staff       (20)      218 2023-05-19 03:31:58.000000 owenpdf-1.0/setup.py
+drwxr-xr-x   0 owenzheng   (501) staff       (20)        0 2023-05-19 07:32:24.166295 owenpdf-2.0/
+-rw-r--r--   0 owenzheng   (501) staff       (20)    35148 2023-05-19 03:27:35.000000 owenpdf-2.0/LICENSE
+-rw-r--r--   0 owenzheng   (501) staff       (20)      109 2023-05-19 07:32:24.166173 owenpdf-2.0/PKG-INFO
+-rw-r--r--   0 owenzheng   (501) staff       (20)       37 2023-05-19 03:21:37.000000 owenpdf-2.0/README.md
+drwxr-xr-x   0 owenzheng   (501) staff       (20)        0 2023-05-19 07:32:24.166041 owenpdf-2.0/owenpdf.egg-info/
+-rw-r--r--   0 owenzheng   (501) staff       (20)      109 2023-05-19 07:32:24.000000 owenpdf-2.0/owenpdf.egg-info/PKG-INFO
+-rw-r--r--   0 owenzheng   (501) staff       (20)      150 2023-05-19 07:32:24.000000 owenpdf-2.0/owenpdf.egg-info/SOURCES.txt
+-rw-r--r--   0 owenzheng   (501) staff       (20)        1 2023-05-19 07:32:24.000000 owenpdf-2.0/owenpdf.egg-info/dependency_links.txt
+-rw-r--r--   0 owenzheng   (501) staff       (20)        1 2023-05-19 07:32:24.000000 owenpdf-2.0/owenpdf.egg-info/top_level.txt
+-rw-r--r--   0 owenzheng   (501) staff       (20)       38 2023-05-19 07:32:24.166330 owenpdf-2.0/setup.cfg
+-rw-r--r--   0 owenzheng   (501) staff       (20)      218 2023-05-19 07:32:07.000000 owenpdf-2.0/setup.py
```

### Comparing `owenpdf-1.0/LICENSE` & `owenpdf-2.0/LICENSE`

 * *Files identical despite different names*

