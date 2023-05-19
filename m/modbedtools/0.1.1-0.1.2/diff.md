# Comparing `tmp/modbedtools-0.1.1.tar.gz` & `tmp/modbedtools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modbedtools-0.1.1.tar", last modified: Fri May 19 14:39:30 2023, max compression
+gzip compressed data, was "modbedtools-0.1.2.tar", last modified: Fri May 19 14:52:13 2023, max compression
```

## Comparing `modbedtools-0.1.1.tar` & `modbedtools-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:39:30.805696 modbedtools-0.1.1/
--rw-r--r--   0 dli        (501) staff       (20)     1067 2023-01-18 19:28:55.000000 modbedtools-0.1.1/LICENSE
--rw-r--r--   0 dli        (501) staff       (20)     8089 2023-05-19 14:39:30.805079 modbedtools-0.1.1/PKG-INFO
--rw-r--r--   0 dli        (501) staff       (20)     7644 2023-05-19 14:36:16.000000 modbedtools-0.1.1/README.md
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:39:30.799752 modbedtools-0.1.1/modbed/
--rw-r--r--   0 dli        (501) staff       (20)        0 2023-01-18 19:31:33.000000 modbedtools-0.1.1/modbed/__init__.py
--rw-r--r--   0 dli        (501) staff       (20)     6620 2023-05-15 19:56:33.000000 modbedtools-0.1.1/modbed/modbed.py
--rw-r--r--   0 dli        (501) staff       (20)       22 2023-05-15 15:53:10.000000 modbedtools-0.1.1/modbed/version.py
--rwxr-xr-x   0 dli        (501) staff       (20)     3224 2023-05-13 03:59:08.000000 modbedtools-0.1.1/modbedtools
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:39:30.803876 modbedtools-0.1.1/modbedtools.egg-info/
--rw-r--r--   0 dli        (501) staff       (20)     8089 2023-05-19 14:39:30.000000 modbedtools-0.1.1/modbedtools.egg-info/PKG-INFO
--rw-r--r--   0 dli        (501) staff       (20)      266 2023-05-19 14:39:30.000000 modbedtools-0.1.1/modbedtools.egg-info/SOURCES.txt
--rw-r--r--   0 dli        (501) staff       (20)        1 2023-05-19 14:39:30.000000 modbedtools-0.1.1/modbedtools.egg-info/dependency_links.txt
--rw-r--r--   0 dli        (501) staff       (20)        6 2023-05-19 14:39:30.000000 modbedtools-0.1.1/modbedtools.egg-info/requires.txt
--rw-r--r--   0 dli        (501) staff       (20)        7 2023-05-19 14:39:30.000000 modbedtools-0.1.1/modbedtools.egg-info/top_level.txt
--rw-r--r--   0 dli        (501) staff       (20)       38 2023-05-19 14:39:30.805897 modbedtools-0.1.1/setup.cfg
--rw-r--r--   0 dli        (501) staff       (20)      771 2023-01-18 19:33:05.000000 modbedtools-0.1.1/setup.py
+drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:52:13.017742 modbedtools-0.1.2/
+-rw-r--r--   0 dli        (501) staff       (20)     1067 2023-01-18 19:28:55.000000 modbedtools-0.1.2/LICENSE
+-rw-r--r--   0 dli        (501) staff       (20)     8089 2023-05-19 14:52:13.017347 modbedtools-0.1.2/PKG-INFO
+-rw-r--r--   0 dli        (501) staff       (20)     7644 2023-05-19 14:36:16.000000 modbedtools-0.1.2/README.md
+drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:52:13.014656 modbedtools-0.1.2/modbed/
+-rw-r--r--   0 dli        (501) staff       (20)        0 2023-01-18 19:31:33.000000 modbedtools-0.1.2/modbed/__init__.py
+-rw-r--r--   0 dli        (501) staff       (20)     6620 2023-05-15 19:56:33.000000 modbedtools-0.1.2/modbed/modbed.py
+-rw-r--r--   0 dli        (501) staff       (20)       22 2023-05-19 14:52:01.000000 modbedtools-0.1.2/modbed/version.py
+-rwxr-xr-x   0 dli        (501) staff       (20)     3224 2023-05-13 03:59:08.000000 modbedtools-0.1.2/modbedtools
+drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:52:13.016860 modbedtools-0.1.2/modbedtools.egg-info/
+-rw-r--r--   0 dli        (501) staff       (20)     8089 2023-05-19 14:52:12.000000 modbedtools-0.1.2/modbedtools.egg-info/PKG-INFO
+-rw-r--r--   0 dli        (501) staff       (20)      266 2023-05-19 14:52:12.000000 modbedtools-0.1.2/modbedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 dli        (501) staff       (20)        1 2023-05-19 14:52:12.000000 modbedtools-0.1.2/modbedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 dli        (501) staff       (20)        6 2023-05-19 14:52:12.000000 modbedtools-0.1.2/modbedtools.egg-info/requires.txt
+-rw-r--r--   0 dli        (501) staff       (20)        7 2023-05-19 14:52:12.000000 modbedtools-0.1.2/modbedtools.egg-info/top_level.txt
+-rw-r--r--   0 dli        (501) staff       (20)       38 2023-05-19 14:52:13.017843 modbedtools-0.1.2/setup.cfg
+-rw-r--r--   0 dli        (501) staff       (20)      771 2023-01-18 19:33:05.000000 modbedtools-0.1.2/setup.py
```

### Comparing `modbedtools-0.1.1/LICENSE` & `modbedtools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modbedtools-0.1.1/PKG-INFO` & `modbedtools-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modbedtools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate modbed track files for visualization on WashU Epigenome Browser
 Home-page: https://github.com/lidaof/modbedtools
 Author: Daofeng Li
 Author-email: lidaof@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `modbedtools-0.1.1/README.md` & `modbedtools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `modbedtools-0.1.1/modbed/modbed.py` & `modbedtools-0.1.2/modbed/modbed.py`

 * *Files identical despite different names*

### Comparing `modbedtools-0.1.1/modbedtools` & `modbedtools-0.1.2/modbedtools`

 * *Files identical despite different names*

### Comparing `modbedtools-0.1.1/modbedtools.egg-info/PKG-INFO` & `modbedtools-0.1.2/modbedtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modbedtools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate modbed track files for visualization on WashU Epigenome Browser
 Home-page: https://github.com/lidaof/modbedtools
 Author: Daofeng Li
 Author-email: lidaof@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `modbedtools-0.1.1/setup.py` & `modbedtools-0.1.2/setup.py`

 * *Files identical despite different names*

