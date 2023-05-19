# Comparing `tmp/pencode-0.1.0.1.tar.gz` & `tmp/pencode-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pencode-0.1.0.1.tar", last modified: Fri May 19 16:21:53 2023, max compression
+gzip compressed data, was "pencode-0.1.0.2.tar", last modified: Fri May 19 16:27:48 2023, max compression
```

## Comparing `pencode-0.1.0.1.tar` & `pencode-0.1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:21:53.213703 pencode-0.1.0.1/
--rw-rw-rw-   0        0        0      148 2023-05-19 16:21:53.211697 pencode-0.1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-19 16:21:53.206693 pencode-0.1.0.1/pencode.egg-info/
--rw-rw-rw-   0        0        0      148 2023-05-19 16:21:52.000000 pencode-0.1.0.1/pencode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      132 2023-05-19 16:21:53.000000 pencode-0.1.0.1/pencode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:21:52.000000 pencode-0.1.0.1/pencode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:21:53.000000 pencode-0.1.0.1/pencode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 16:21:53.214702 pencode-0.1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      215 2023-05-19 16:21:33.000000 pencode-0.1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:27:48.365661 pencode-0.1.0.2/
+-rw-rw-rw-   0        0        0      148 2023-05-19 16:27:48.362720 pencode-0.1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-19 16:27:48.339660 pencode-0.1.0.2/pencode.egg-info/
+-rw-rw-rw-   0        0        0      148 2023-05-19 16:27:48.000000 pencode-0.1.0.2/pencode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      132 2023-05-19 16:27:48.000000 pencode-0.1.0.2/pencode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:27:48.000000 pencode-0.1.0.2/pencode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:27:48.000000 pencode-0.1.0.2/pencode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 16:27:48.366658 pencode-0.1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      215 2023-05-19 16:27:32.000000 pencode-0.1.0.2/setup.py
```

