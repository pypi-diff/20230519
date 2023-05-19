# Comparing `tmp/shinherpro-1.4.6.tar.gz` & `tmp/shinherpro-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.4.6.tar", last modified: Fri May 19 08:02:28 2023, max compression
+gzip compressed data, was "shinherpro-1.4.7.tar", last modified: Fri May 19 08:12:21 2023, max compression
```

## Comparing `shinherpro-1.4.6.tar` & `shinherpro-1.4.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 08:02:28.069383 shinherpro-1.4.6/
--rw-rw-rw-   0        0        0      148 2023-05-19 08:02:28.069383 shinherpro-1.4.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-19 08:02:28.057443 shinherpro-1.4.6/TYAI/
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.4.6/TYAI/__init__.py
--rw-rw-rw-   0        0        0     9855 2023-05-19 08:02:02.000000 shinherpro-1.4.6/TYAI/tyaigradesystepro142.py
--rw-rw-rw-   0        0        0       42 2023-05-19 08:02:28.069383 shinherpro-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      399 2023-05-19 08:02:23.000000 shinherpro-1.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:02:28.067402 shinherpro-1.4.6/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      148 2023-05-19 08:02:27.000000 shinherpro-1.4.6/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-19 08:02:28.000000 shinherpro-1.4.6/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 08:02:27.000000 shinherpro-1.4.6/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-19 08:02:27.000000 shinherpro-1.4.6/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-19 08:02:27.000000 shinherpro-1.4.6/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 08:12:21.044435 shinherpro-1.4.7/
+-rw-rw-rw-   0        0        0      148 2023-05-19 08:12:21.043341 shinherpro-1.4.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-19 08:12:21.031582 shinherpro-1.4.7/TYAI/
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.4.7/TYAI/__init__.py
+-rw-rw-rw-   0        0        0     9855 2023-05-19 08:02:02.000000 shinherpro-1.4.7/TYAI/tyaigradesystepro142.py
+-rw-rw-rw-   0        0        0       42 2023-05-19 08:12:21.044435 shinherpro-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      399 2023-05-19 08:12:17.000000 shinherpro-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:12:21.042342 shinherpro-1.4.7/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      148 2023-05-19 08:12:20.000000 shinherpro-1.4.7/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-19 08:12:20.000000 shinherpro-1.4.7/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 08:12:20.000000 shinherpro-1.4.7/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-19 08:12:20.000000 shinherpro-1.4.7/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-19 08:12:20.000000 shinherpro-1.4.7/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.4.6/TYAI/tyaigradesystepro142.py` & `shinherpro-1.4.7/TYAI/tyaigradesystepro142.py`

 * *Files identical despite different names*

