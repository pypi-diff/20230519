# Comparing `tmp/textagon-0.1.0.tar.gz` & `tmp/textagon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textagon-0.1.0.tar", last modified: Fri May 19 16:07:50 2023, max compression
+gzip compressed data, was "textagon-0.1.1.tar", last modified: Fri May 19 17:14:33 2023, max compression
```

## Comparing `textagon-0.1.0.tar` & `textagon-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:07:50.950454 textagon-0.1.0/
--rw-rw-rw-   0        0        0      181 2023-05-19 16:07:50.950454 textagon-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-19 16:07:50.950454 textagon-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-05-19 16:06:58.000000 textagon-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:07:50.940451 textagon-0.1.0/textagon/
--rw-rw-rw-   0        0        0       31 2023-05-19 15:57:41.000000 textagon-0.1.0/textagon/__init__.py
--rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.0/textagon/install-dependencies.py
--rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.0/textagon/process-text.py
--rw-rw-rw-   0        0        0       44 2023-05-19 15:57:07.000000 textagon-0.1.0/textagon/textagon.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:07:50.950454 textagon-0.1.0/textagon.egg-info/
--rw-rw-rw-   0        0        0      181 2023-05-19 16:07:50.000000 textagon-0.1.0/textagon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-19 16:07:50.000000 textagon-0.1.0/textagon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:07:50.000000 textagon-0.1.0/textagon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 16:07:50.000000 textagon-0.1.0/textagon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 17:14:33.039585 textagon-0.1.1/
+-rw-rw-rw-   0        0        0      181 2023-05-19 17:14:33.038575 textagon-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-19 17:14:33.039585 textagon-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-05-19 17:14:28.000000 textagon-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:14:33.025820 textagon-0.1.1/textagon/
+-rw-rw-rw-   0        0        0       70 2023-05-19 17:12:16.000000 textagon-0.1.1/textagon/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.1/textagon/install-dependencies.py
+-rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.1/textagon/process-text.py
+-rw-rw-rw-   0        0        0     3428 2023-05-19 17:12:02.000000 textagon-0.1.1/textagon/textagon.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:14:33.038575 textagon-0.1.1/textagon.egg-info/
+-rw-rw-rw-   0        0        0      181 2023-05-19 17:14:32.000000 textagon-0.1.1/textagon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-19 17:14:32.000000 textagon-0.1.1/textagon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 17:14:32.000000 textagon-0.1.1/textagon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-05-19 17:14:32.000000 textagon-0.1.1/textagon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 17:14:32.000000 textagon-0.1.1/textagon.egg-info/top_level.txt
```

### Comparing `textagon-0.1.0/textagon/process-text.py` & `textagon-0.1.1/textagon/process-text.py`

 * *Files identical despite different names*

