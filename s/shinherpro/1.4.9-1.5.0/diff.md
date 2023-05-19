# Comparing `tmp/shinherpro-1.4.9.tar.gz` & `tmp/shinherpro-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.4.9.tar", last modified: Fri May 19 08:57:39 2023, max compression
+gzip compressed data, was "shinherpro-1.5.0.tar", last modified: Fri May 19 09:07:12 2023, max compression
```

## Comparing `shinherpro-1.4.9.tar` & `shinherpro-1.5.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 08:57:39.422295 shinherpro-1.4.9/
--rw-rw-rw-   0        0        0      163 2023-05-19 08:57:39.421295 shinherpro-1.4.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-19 08:57:39.422295 shinherpro-1.4.9/setup.cfg
--rw-rw-rw-   0        0        0      267 2023-05-19 08:57:14.000000 shinherpro-1.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:57:39.414312 shinherpro-1.4.9/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      163 2023-05-19 08:57:39.000000 shinherpro-1.4.9/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-05-19 08:57:39.000000 shinherpro-1.4.9/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 08:57:39.000000 shinherpro-1.4.9/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-19 08:57:39.000000 shinherpro-1.4.9/shinherpro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 08:57:39.420325 shinherpro-1.4.9/tyai/
--rw-rw-rw-   0        0        0     9843 2023-05-19 08:57:07.000000 shinherpro-1.4.9/tyai/tyaigradesystepro142.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:07:12.481903 shinherpro-1.5.0/
+-rw-rw-rw-   0        0        0      163 2023-05-19 09:07:12.480904 shinherpro-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-19 09:06:20.000000 shinherpro-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 09:07:12.481903 shinherpro-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      274 2023-05-19 09:02:43.000000 shinherpro-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:07:12.478911 shinherpro-1.5.0/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      163 2023-05-19 09:07:12.000000 shinherpro-1.5.0/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-19 09:07:12.000000 shinherpro-1.5.0/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 09:07:12.000000 shinherpro-1.5.0/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-19 09:07:12.000000 shinherpro-1.5.0/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 09:07:12.480904 shinherpro-1.5.0/tyaishinher/
+-rw-rw-rw-   0        0        0        0 2023-05-19 09:05:03.000000 shinherpro-1.5.0/tyaishinher/__init__.py
+-rw-rw-rw-   0        0        0     9843 2023-05-19 08:57:07.000000 shinherpro-1.5.0/tyaishinher/tyaigradesystepro142.py
```

### Comparing `shinherpro-1.4.9/tyai/tyaigradesystepro142.py` & `shinherpro-1.5.0/tyaishinher/tyaigradesystepro142.py`

 * *Files identical despite different names*

