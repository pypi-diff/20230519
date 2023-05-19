# Comparing `tmp/lps22hh-0.1.1.tar.gz` & `tmp/lps22hh-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lps22hh-0.1.1.tar", last modified: Fri May 19 12:23:34 2023, max compression
+gzip compressed data, was "lps22hh-0.2.0.tar", last modified: Fri May 19 12:35:15 2023, max compression
```

## Comparing `lps22hh-0.1.1.tar` & `lps22hh-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-19 12:23:34.571636 lps22hh-0.1.1/
--rw-r--r--   0 chris      (501) staff       (20)     1072 2023-05-19 06:32:49.000000 lps22hh-0.1.1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     2616 2023-05-19 12:23:34.571127 lps22hh-0.1.1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     1912 2023-05-19 11:42:57.000000 lps22hh-0.1.1/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-19 12:23:34.567064 lps22hh-0.1.1/lps22hh/
--rw-r--r--   0 chris      (501) staff       (20)       28 2023-05-19 12:21:00.000000 lps22hh-0.1.1/lps22hh/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    11086 2023-05-19 09:48:57.000000 lps22hh-0.1.1/lps22hh/lps22hh.py
--rw-r--r--   0 chris      (501) staff       (20)     2081 2023-05-19 09:44:38.000000 lps22hh-0.1.1/lps22hh/register.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-19 12:23:34.570140 lps22hh-0.1.1/lps22hh.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     2616 2023-05-19 12:23:33.000000 lps22hh-0.1.1/lps22hh.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      209 2023-05-19 12:23:34.000000 lps22hh-0.1.1/lps22hh.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-19 12:23:33.000000 lps22hh-0.1.1/lps22hh.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)        8 2023-05-19 12:23:34.000000 lps22hh-0.1.1/lps22hh.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-19 12:23:34.571826 lps22hh-0.1.1/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)      980 2023-05-19 12:23:26.000000 lps22hh-0.1.1/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-19 12:35:15.795024 lps22hh-0.2.0/
+-rw-r--r--   0 chris      (501) staff       (20)     1072 2023-05-19 06:32:49.000000 lps22hh-0.2.0/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)     2616 2023-05-19 12:35:15.794580 lps22hh-0.2.0/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     1912 2023-05-19 11:42:57.000000 lps22hh-0.2.0/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-19 12:35:15.790173 lps22hh-0.2.0/lps22hh/
+-rw-r--r--   0 chris      (501) staff       (20)       28 2023-05-19 12:21:00.000000 lps22hh-0.2.0/lps22hh/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    11086 2023-05-19 09:48:57.000000 lps22hh-0.2.0/lps22hh/lps22hh.py
+-rw-r--r--   0 chris      (501) staff       (20)     2081 2023-05-19 09:44:38.000000 lps22hh-0.2.0/lps22hh/register.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-19 12:35:15.793546 lps22hh-0.2.0/lps22hh.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     2616 2023-05-19 12:35:14.000000 lps22hh-0.2.0/lps22hh.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      209 2023-05-19 12:35:15.000000 lps22hh-0.2.0/lps22hh.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-19 12:35:15.000000 lps22hh-0.2.0/lps22hh.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)        8 2023-05-19 12:35:15.000000 lps22hh-0.2.0/lps22hh.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-19 12:35:15.795411 lps22hh-0.2.0/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)      980 2023-05-19 12:34:40.000000 lps22hh-0.2.0/setup.py
```

### Comparing `lps22hh-0.1.1/LICENSE` & `lps22hh-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lps22hh-0.1.1/PKG-INFO` & `lps22hh-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lps22hh
-Version: 0.1.1
+Version: 0.2.0
 Summary: Raspberry Pi Pico Micropyhton library to interact with the ST LPS22HH Barometric pressure sensor
 Home-page: https://github.com/cbraissant/lps22hh_pico_driver
 Author: Chris Braissant
 Author-email: chrisbraissant@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

### Comparing `lps22hh-0.1.1/README.md` & `lps22hh-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lps22hh-0.1.1/lps22hh/lps22hh.py` & `lps22hh-0.2.0/lps22hh/lps22hh.py`

 * *Files identical despite different names*

### Comparing `lps22hh-0.1.1/lps22hh/register.py` & `lps22hh-0.2.0/lps22hh/register.py`

 * *Files identical despite different names*

### Comparing `lps22hh-0.1.1/lps22hh.egg-info/PKG-INFO` & `lps22hh-0.2.0/lps22hh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lps22hh
-Version: 0.1.1
+Version: 0.2.0
 Summary: Raspberry Pi Pico Micropyhton library to interact with the ST LPS22HH Barometric pressure sensor
 Home-page: https://github.com/cbraissant/lps22hh_pico_driver
 Author: Chris Braissant
 Author-email: chrisbraissant@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

### Comparing `lps22hh-0.1.1/setup.py` & `lps22hh-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.11',
     'Topic :: Software Development :: Embedded Systems',
 ]
 
 setup(
     name = 'lps22hh',
-    version = '0.1.1',
+    version = '0.2.0',
     author = 'Chris Braissant',
     author_email = 'chrisbraissant@gmail.com',
     description = 'Raspberry Pi Pico Micropyhton library to interact with the ST LPS22HH Barometric pressure sensor',
     license = 'MIT',
     url='https://github.com/cbraissant/lps22hh_pico_driver',
     install_requires = [],
     classifiers=classifiers,
```

