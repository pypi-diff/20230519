# Comparing `tmp/shinherpro-1.4.5.tar.gz` & `tmp/shinherpro-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.4.5.tar", last modified: Fri May 19 07:58:02 2023, max compression
+gzip compressed data, was "shinherpro-1.4.6.tar", last modified: Fri May 19 08:02:28 2023, max compression
```

## Comparing `shinherpro-1.4.5.tar` & `shinherpro-1.4.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 07:58:02.980306 shinherpro-1.4.5/
--rw-rw-rw-   0        0        0      148 2023-05-19 07:58:02.980306 shinherpro-1.4.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-19 07:58:02.965345 shinherpro-1.4.5/TYAI/
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.4.5/TYAI/__init__.py
--rw-rw-rw-   0        0        0    10046 2023-05-19 03:01:32.000000 shinherpro-1.4.5/TYAI/tyaigradesystepro142.py
--rw-rw-rw-   0        0        0       42 2023-05-19 07:58:02.980306 shinherpro-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0      399 2023-05-19 07:57:57.000000 shinherpro-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:58:02.978310 shinherpro-1.4.5/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      148 2023-05-19 07:58:02.000000 shinherpro-1.4.5/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-19 07:58:02.000000 shinherpro-1.4.5/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 07:58:02.000000 shinherpro-1.4.5/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-19 07:58:02.000000 shinherpro-1.4.5/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-19 07:58:02.000000 shinherpro-1.4.5/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 08:02:28.069383 shinherpro-1.4.6/
+-rw-rw-rw-   0        0        0      148 2023-05-19 08:02:28.069383 shinherpro-1.4.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-19 08:02:28.057443 shinherpro-1.4.6/TYAI/
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.4.6/TYAI/__init__.py
+-rw-rw-rw-   0        0        0     9855 2023-05-19 08:02:02.000000 shinherpro-1.4.6/TYAI/tyaigradesystepro142.py
+-rw-rw-rw-   0        0        0       42 2023-05-19 08:02:28.069383 shinherpro-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      399 2023-05-19 08:02:23.000000 shinherpro-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:02:28.067402 shinherpro-1.4.6/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      148 2023-05-19 08:02:27.000000 shinherpro-1.4.6/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-19 08:02:28.000000 shinherpro-1.4.6/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 08:02:27.000000 shinherpro-1.4.6/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-19 08:02:27.000000 shinherpro-1.4.6/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-19 08:02:27.000000 shinherpro-1.4.6/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.4.5/TYAI/tyaigradesystepro142.py` & `shinherpro-1.4.6/TYAI/tyaigradesystepro142.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,28 +257,14 @@
 
 
 
 
 
 
 
-model = modle_setup("C:\\Users\\User\\Downloads\\vfc_AiModel_4.1_VGG16_black.h5")
-
-driver = chrome_driver_setup()
-
-print(getGrades("013333","B123742969",driver,model))
-
-
-
-
-
-
-
-
-
```

