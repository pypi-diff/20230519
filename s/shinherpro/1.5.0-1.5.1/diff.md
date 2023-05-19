# Comparing `tmp/shinherpro-1.5.0.tar.gz` & `tmp/shinherpro-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.5.0.tar", last modified: Fri May 19 09:07:12 2023, max compression
+gzip compressed data, was "shinherpro-1.5.1.tar", last modified: Fri May 19 14:18:30 2023, max compression
```

## Comparing `shinherpro-1.5.0.tar` & `shinherpro-1.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 09:07:12.481903 shinherpro-1.5.0/
--rw-rw-rw-   0        0        0      163 2023-05-19 09:07:12.480904 shinherpro-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-19 09:06:20.000000 shinherpro-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 09:07:12.481903 shinherpro-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      274 2023-05-19 09:02:43.000000 shinherpro-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:07:12.478911 shinherpro-1.5.0/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      163 2023-05-19 09:07:12.000000 shinherpro-1.5.0/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-19 09:07:12.000000 shinherpro-1.5.0/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 09:07:12.000000 shinherpro-1.5.0/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-19 09:07:12.000000 shinherpro-1.5.0/shinherpro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 09:07:12.480904 shinherpro-1.5.0/tyaishinher/
--rw-rw-rw-   0        0        0        0 2023-05-19 09:05:03.000000 shinherpro-1.5.0/tyaishinher/__init__.py
--rw-rw-rw-   0        0        0     9843 2023-05-19 08:57:07.000000 shinherpro-1.5.0/tyaishinher/tyaigradesystepro142.py
+drwxrwxrwx   0        0        0        0 2023-05-19 14:18:30.643865 shinherpro-1.5.1/
+-rw-rw-rw-   0        0        0      143 2023-05-19 14:18:30.643369 shinherpro-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-19 14:18:30.643865 shinherpro-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      400 2023-05-19 14:18:01.000000 shinherpro-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 14:18:30.621541 shinherpro-1.5.1/shinherpro/
+-rw-rw-rw-   0        0        0    10046 2023-05-19 03:01:32.000000 shinherpro-1.5.1/shinherpro/TYAI142.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.5.1/shinherpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 14:18:30.641385 shinherpro-1.5.1/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      143 2023-05-19 14:18:30.000000 shinherpro-1.5.1/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-19 14:18:30.000000 shinherpro-1.5.1/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 14:18:30.000000 shinherpro-1.5.1/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-19 14:18:30.000000 shinherpro-1.5.1/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-19 14:18:30.000000 shinherpro-1.5.1/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.5.0/tyaishinher/tyaigradesystepro142.py` & `shinherpro-1.5.1/shinherpro/TYAI142.py`

 * *Files 3% similar despite different names*

```diff
@@ -257,14 +257,34 @@
 
 
 
 
 
 
 
+model = modle_setup("C:\\Users\\User\\Downloads\\vfc_AiModel_4.1_VGG16_black.h5")
+
+driver = chrome_driver_setup()
+
+print(getGrades("013333","B123742969",driver,model))
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

