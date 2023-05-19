# Comparing `tmp/pyspeaker-5.0.tar.gz` & `tmp/pyspeaker-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspeaker-5.0.tar", last modified: Thu May 18 16:53:57 2023, max compression
+gzip compressed data, was "pyspeaker-6.0.tar", last modified: Fri May 19 06:16:58 2023, max compression
```

## Comparing `pyspeaker-5.0.tar` & `pyspeaker-6.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 16:53:57.208852 pyspeaker-5.0/
--rw-rw-rw-   0        0        0     1091 2023-02-23 09:47:52.000000 pyspeaker-5.0/LICENSE.txt
--rw-rw-rw-   0        0        0      212 2023-05-18 16:53:57.207847 pyspeaker-5.0/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 pyspeaker-5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 16:53:57.177195 pyspeaker-5.0/app/
--rw-rw-rw-   0        0        0      776 2023-04-17 09:09:58.000000 pyspeaker-5.0/app/Audio.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:53:57.202453 pyspeaker-5.0/app/pyspeaker.egg-info/
--rw-rw-rw-   0        0        0      212 2023-05-18 16:53:57.000000 pyspeaker-5.0/app/pyspeaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-18 16:53:57.000000 pyspeaker-5.0/app/pyspeaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 16:53:57.000000 pyspeaker-5.0/app/pyspeaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-18 16:53:57.000000 pyspeaker-5.0/app/pyspeaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 16:53:57.000000 pyspeaker-5.0/app/pyspeaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 16:53:57.209899 pyspeaker-5.0/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-05-18 16:53:27.000000 pyspeaker-5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:16:58.120160 pyspeaker-6.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-23 09:47:52.000000 pyspeaker-6.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      212 2023-05-19 06:16:58.118160 pyspeaker-6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 pyspeaker-6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 06:16:58.086646 pyspeaker-6.0/app/
+-rw-rw-rw-   0        0        0      776 2023-04-17 09:09:58.000000 pyspeaker-6.0/app/Audio.py
+-rw-rw-rw-   0        0        0       55 2023-05-19 06:06:32.000000 pyspeaker-6.0/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:16:58.116160 pyspeaker-6.0/app/pyspeaker.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-05-19 06:16:58.000000 pyspeaker-6.0/app/pyspeaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-19 06:16:58.000000 pyspeaker-6.0/app/pyspeaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 06:16:58.000000 pyspeaker-6.0/app/pyspeaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-19 06:16:58.000000 pyspeaker-6.0/app/pyspeaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-19 06:16:58.000000 pyspeaker-6.0/app/pyspeaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 06:16:58.120160 pyspeaker-6.0/setup.cfg
+-rw-rw-rw-   0        0        0      770 2023-05-19 06:16:33.000000 pyspeaker-6.0/setup.py
```

### Comparing `pyspeaker-5.0/LICENSE.txt` & `pyspeaker-6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyspeaker-5.0/app/Audio.py` & `pyspeaker-6.0/app/Audio.py`

 * *Files identical despite different names*

