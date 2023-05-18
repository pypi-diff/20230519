# Comparing `tmp/libheader-1.0.0.tar.gz` & `tmp/libheader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libheader-1.0.0.tar", last modified: Thu May 18 23:06:36 2023, max compression
+gzip compressed data, was "libheader-1.0.1.tar", last modified: Thu May 18 23:24:14 2023, max compression
```

## Comparing `libheader-1.0.0.tar` & `libheader-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 23:06:36.936138 libheader-1.0.0/
--rw-rw-rw-   0        0        0      615 2023-05-18 23:06:36.936138 libheader-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 23:06:36.924137 libheader-1.0.0/libheader/
--rw-rw-rw-   0        0        0       26 2023-05-18 21:45:06.000000 libheader-1.0.0/libheader/__init__.py
--rw-rw-rw-   0        0        0      265 2023-05-18 23:02:34.000000 libheader-1.0.0/libheader/__main__.py
--rw-rw-rw-   0        0        0      861 2023-05-18 21:44:48.000000 libheader-1.0.0/libheader/gcclh.py
--rw-rw-rw-   0        0        0      913 2023-05-18 21:40:08.000000 libheader-1.0.0/libheader/lh.py
--rw-rw-rw-   0        0        0      556 2023-05-18 21:56:22.000000 libheader-1.0.0/libheader/makelh.py
-drwxrwxrwx   0        0        0        0 2023-05-18 23:06:36.934134 libheader-1.0.0/libheader.egg-info/
--rw-rw-rw-   0        0        0      615 2023-05-18 23:06:36.000000 libheader-1.0.0/libheader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-05-18 23:06:36.000000 libheader-1.0.0/libheader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 23:06:36.000000 libheader-1.0.0/libheader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-18 23:06:36.000000 libheader-1.0.0/libheader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 23:06:36.937134 libheader-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      808 2023-05-18 23:06:07.000000 libheader-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:24:14.718547 libheader-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-18 23:24:14.718547 libheader-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-18 23:24:02.000000 libheader-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:24:14.714547 libheader-1.0.1/libheader/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-18 23:24:02.000000 libheader-1.0.1/libheader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-18 23:24:02.000000 libheader-1.0.1/libheader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-18 23:24:02.000000 libheader-1.0.1/libheader/gcclh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-18 23:24:02.000000 libheader-1.0.1/libheader/lh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-18 23:24:02.000000 libheader-1.0.1/libheader/makelh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:24:14.714547 libheader-1.0.1/libheader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-18 23:24:14.000000 libheader-1.0.1/libheader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-18 23:24:14.000000 libheader-1.0.1/libheader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:24:14.000000 libheader-1.0.1/libheader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 23:24:14.000000 libheader-1.0.1/libheader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:24:14.718547 libheader-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-18 23:24:02.000000 libheader-1.0.1/setup.py
```

