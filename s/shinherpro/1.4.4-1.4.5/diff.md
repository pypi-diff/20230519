# Comparing `tmp/shinherpro-1.4.4.tar.gz` & `tmp/shinherpro-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.4.4.tar", last modified: Fri May 19 07:51:12 2023, max compression
+gzip compressed data, was "shinherpro-1.4.5.tar", last modified: Fri May 19 07:58:02 2023, max compression
```

## Comparing `shinherpro-1.4.4.tar` & `shinherpro-1.4.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 07:51:12.098936 shinherpro-1.4.4/
--rw-rw-rw-   0        0        0      148 2023-05-19 07:51:12.098936 shinherpro-1.4.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-19 07:51:12.079015 shinherpro-1.4.4/TYAI/
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.4.4/TYAI/__init__.py
--rw-rw-rw-   0        0        0    10046 2023-05-19 03:01:32.000000 shinherpro-1.4.4/TYAI/tyaigradesystepro142.py
--rw-rw-rw-   0        0        0       42 2023-05-19 07:51:12.099934 shinherpro-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      399 2023-05-19 07:48:41.000000 shinherpro-1.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:51:12.097966 shinherpro-1.4.4/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      148 2023-05-19 07:51:12.000000 shinherpro-1.4.4/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-19 07:51:12.000000 shinherpro-1.4.4/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 07:51:12.000000 shinherpro-1.4.4/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-19 07:51:12.000000 shinherpro-1.4.4/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-19 07:51:12.000000 shinherpro-1.4.4/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 07:58:02.980306 shinherpro-1.4.5/
+-rw-rw-rw-   0        0        0      148 2023-05-19 07:58:02.980306 shinherpro-1.4.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-19 07:58:02.965345 shinherpro-1.4.5/TYAI/
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.4.5/TYAI/__init__.py
+-rw-rw-rw-   0        0        0    10046 2023-05-19 03:01:32.000000 shinherpro-1.4.5/TYAI/tyaigradesystepro142.py
+-rw-rw-rw-   0        0        0       42 2023-05-19 07:58:02.980306 shinherpro-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      399 2023-05-19 07:57:57.000000 shinherpro-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:58:02.978310 shinherpro-1.4.5/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      148 2023-05-19 07:58:02.000000 shinherpro-1.4.5/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-19 07:58:02.000000 shinherpro-1.4.5/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 07:58:02.000000 shinherpro-1.4.5/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-19 07:58:02.000000 shinherpro-1.4.5/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-19 07:58:02.000000 shinherpro-1.4.5/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.4.4/TYAI/tyaigradesystepro142.py` & `shinherpro-1.4.5/TYAI/tyaigradesystepro142.py`

 * *Files identical despite different names*

