# Comparing `tmp/shinherpro-1.4.7.tar.gz` & `tmp/shinherpro-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.4.7.tar", last modified: Fri May 19 08:12:21 2023, max compression
+gzip compressed data, was "shinherpro-1.4.9.tar", last modified: Fri May 19 08:57:39 2023, max compression
```

## Comparing `shinherpro-1.4.7.tar` & `shinherpro-1.4.9.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 08:12:21.044435 shinherpro-1.4.7/
--rw-rw-rw-   0        0        0      148 2023-05-19 08:12:21.043341 shinherpro-1.4.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-19 08:12:21.031582 shinherpro-1.4.7/TYAI/
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.4.7/TYAI/__init__.py
--rw-rw-rw-   0        0        0     9855 2023-05-19 08:02:02.000000 shinherpro-1.4.7/TYAI/tyaigradesystepro142.py
--rw-rw-rw-   0        0        0       42 2023-05-19 08:12:21.044435 shinherpro-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0      399 2023-05-19 08:12:17.000000 shinherpro-1.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:12:21.042342 shinherpro-1.4.7/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      148 2023-05-19 08:12:20.000000 shinherpro-1.4.7/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-19 08:12:20.000000 shinherpro-1.4.7/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 08:12:20.000000 shinherpro-1.4.7/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-19 08:12:20.000000 shinherpro-1.4.7/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-19 08:12:20.000000 shinherpro-1.4.7/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 08:57:39.422295 shinherpro-1.4.9/
+-rw-rw-rw-   0        0        0      163 2023-05-19 08:57:39.421295 shinherpro-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-19 08:57:39.422295 shinherpro-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      267 2023-05-19 08:57:14.000000 shinherpro-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:57:39.414312 shinherpro-1.4.9/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      163 2023-05-19 08:57:39.000000 shinherpro-1.4.9/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-19 08:57:39.000000 shinherpro-1.4.9/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 08:57:39.000000 shinherpro-1.4.9/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-19 08:57:39.000000 shinherpro-1.4.9/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 08:57:39.420325 shinherpro-1.4.9/tyai/
+-rw-rw-rw-   0        0        0     9843 2023-05-19 08:57:07.000000 shinherpro-1.4.9/tyai/tyaigradesystepro142.py
```

### Comparing `shinherpro-1.4.7/TYAI/tyaigradesystepro142.py` & `shinherpro-1.4.9/tyai/tyaigradesystepro142.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,13 +265,7 @@
 
 
 
 
 
 
 
-
-
-
-
-
-
```

