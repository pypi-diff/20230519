# Comparing `tmp/owenpdf-3.0.tar.gz` & `tmp/owenpdf-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owenpdf-3.0.tar", last modified: Fri May 19 07:38:06 2023, max compression
+gzip compressed data, was "owenpdf-3.1.tar", last modified: Fri May 19 07:44:06 2023, max compression
```

## Comparing `owenpdf-3.0.tar` & `owenpdf-3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 owenzheng   (501) staff       (20)        0 2023-05-19 07:38:06.705567 owenpdf-3.0/
--rw-r--r--   0 owenzheng   (501) staff       (20)    35148 2023-05-19 03:27:35.000000 owenpdf-3.0/LICENSE
--rw-r--r--   0 owenzheng   (501) staff       (20)      109 2023-05-19 07:38:06.705434 owenpdf-3.0/PKG-INFO
--rw-r--r--   0 owenzheng   (501) staff       (20)       37 2023-05-19 03:21:37.000000 owenpdf-3.0/README.md
-drwxr-xr-x   0 owenzheng   (501) staff       (20)        0 2023-05-19 07:38:06.704897 owenpdf-3.0/owenpdf/
--rw-r--r--   0 owenzheng   (501) staff       (20)        0 2023-05-19 03:16:32.000000 owenpdf-3.0/owenpdf/__init__.py
--rw-r--r--   0 owenzheng   (501) staff       (20)       35 2023-05-19 03:17:02.000000 owenpdf-3.0/owenpdf/pdf2text.py
--rw-r--r--   0 owenzheng   (501) staff       (20)        0 2023-05-19 03:17:33.000000 owenpdf-3.0/owenpdf/pdfimage.py
-drwxr-xr-x   0 owenzheng   (501) staff       (20)        0 2023-05-19 07:38:06.705303 owenpdf-3.0/owenpdf.egg-info/
--rw-r--r--   0 owenzheng   (501) staff       (20)      109 2023-05-19 07:38:06.000000 owenpdf-3.0/owenpdf.egg-info/PKG-INFO
--rw-r--r--   0 owenzheng   (501) staff       (20)      210 2023-05-19 07:38:06.000000 owenpdf-3.0/owenpdf.egg-info/SOURCES.txt
--rw-r--r--   0 owenzheng   (501) staff       (20)        1 2023-05-19 07:38:06.000000 owenpdf-3.0/owenpdf.egg-info/dependency_links.txt
--rw-r--r--   0 owenzheng   (501) staff       (20)        8 2023-05-19 07:38:06.000000 owenpdf-3.0/owenpdf.egg-info/top_level.txt
--rw-r--r--   0 owenzheng   (501) staff       (20)       38 2023-05-19 07:38:06.705600 owenpdf-3.0/setup.cfg
--rw-r--r--   0 owenzheng   (501) staff       (20)      217 2023-05-19 07:37:44.000000 owenpdf-3.0/setup.py
+drwxr-xr-x   0 owenzheng   (501) staff       (20)        0 2023-05-19 07:44:06.672931 owenpdf-3.1/
+-rw-r--r--   0 owenzheng   (501) staff       (20)    35148 2023-05-19 03:27:35.000000 owenpdf-3.1/LICENSE
+-rw-r--r--   0 owenzheng   (501) staff       (20)      109 2023-05-19 07:44:06.672765 owenpdf-3.1/PKG-INFO
+-rw-r--r--   0 owenzheng   (501) staff       (20)       37 2023-05-19 03:21:37.000000 owenpdf-3.1/README.md
+drwxr-xr-x   0 owenzheng   (501) staff       (20)        0 2023-05-19 07:44:06.671964 owenpdf-3.1/owenpdf/
+-rw-r--r--   0 owenzheng   (501) staff       (20)        0 2023-05-19 03:16:32.000000 owenpdf-3.1/owenpdf/__init__.py
+-rw-r--r--   0 owenzheng   (501) staff       (20)        0 2023-05-19 03:17:33.000000 owenpdf-3.1/owenpdf/pdf2image.py
+-rw-r--r--   0 owenzheng   (501) staff       (20)       36 2023-05-19 07:42:18.000000 owenpdf-3.1/owenpdf/pdf2text.py
+drwxr-xr-x   0 owenzheng   (501) staff       (20)        0 2023-05-19 07:44:06.672591 owenpdf-3.1/owenpdf.egg-info/
+-rw-r--r--   0 owenzheng   (501) staff       (20)      109 2023-05-19 07:44:06.000000 owenpdf-3.1/owenpdf.egg-info/PKG-INFO
+-rw-r--r--   0 owenzheng   (501) staff       (20)      211 2023-05-19 07:44:06.000000 owenpdf-3.1/owenpdf.egg-info/SOURCES.txt
+-rw-r--r--   0 owenzheng   (501) staff       (20)        1 2023-05-19 07:44:06.000000 owenpdf-3.1/owenpdf.egg-info/dependency_links.txt
+-rw-r--r--   0 owenzheng   (501) staff       (20)        8 2023-05-19 07:44:06.000000 owenpdf-3.1/owenpdf.egg-info/top_level.txt
+-rw-r--r--   0 owenzheng   (501) staff       (20)       38 2023-05-19 07:44:06.672968 owenpdf-3.1/setup.cfg
+-rw-r--r--   0 owenzheng   (501) staff       (20)      217 2023-05-19 07:43:30.000000 owenpdf-3.1/setup.py
```

### Comparing `owenpdf-3.0/LICENSE` & `owenpdf-3.1/LICENSE`

 * *Files identical despite different names*

