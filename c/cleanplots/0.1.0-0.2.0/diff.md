# Comparing `tmp/cleanplots-0.1.0.tar.gz` & `tmp/cleanplots-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cleanplots-0.1.0.tar", last modified: Thu Apr 14 15:41:26 2022, max compression
+gzip compressed data, was "cleanplots-0.2.0.tar", last modified: Fri May 19 19:53:59 2023, max compression
```

## Comparing `cleanplots-0.1.0.tar` & `cleanplots-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwx------   0 henrypinkard   (501) staff       (20)        0 2022-04-14 15:41:26.000000 cleanplots-0.1.0/
--rwx------   0 henrypinkard   (501) staff       (20)      611 2022-04-14 15:41:26.000000 cleanplots-0.1.0/PKG-INFO
--rwx------   0 henrypinkard   (501) staff       (20)        0 2022-04-14 15:36:28.000000 cleanplots-0.1.0/README.md
-drwx------   0 henrypinkard   (501) staff       (20)        0 2022-04-14 15:41:26.000000 cleanplots-0.1.0/cleanplots/
--rwx------   0 henrypinkard   (501) staff       (20)       56 2022-04-14 15:40:29.000000 cleanplots-0.1.0/cleanplots/__init__.py
--rwx------   0 henrypinkard   (501) staff       (20)       72 2022-04-14 15:35:42.000000 cleanplots-0.1.0/cleanplots/_version.py
--rwx------   0 henrypinkard   (501) staff       (20)     5317 2022-03-25 02:49:12.000000 cleanplots-0.1.0/cleanplots/cleanplots.py
-drwx------   0 henrypinkard   (501) staff       (20)        0 2022-04-14 15:41:26.000000 cleanplots-0.1.0/cleanplots.egg-info/
--rwx------   0 henrypinkard   (501) staff       (20)      611 2022-04-14 15:41:26.000000 cleanplots-0.1.0/cleanplots.egg-info/PKG-INFO
--rwx------   0 henrypinkard   (501) staff       (20)      258 2022-04-14 15:41:26.000000 cleanplots-0.1.0/cleanplots.egg-info/SOURCES.txt
--rwx------   0 henrypinkard   (501) staff       (20)        1 2022-04-14 15:41:26.000000 cleanplots-0.1.0/cleanplots.egg-info/dependency_links.txt
--rwx------   0 henrypinkard   (501) staff       (20)       25 2022-04-14 15:41:26.000000 cleanplots-0.1.0/cleanplots.egg-info/requires.txt
--rwx------   0 henrypinkard   (501) staff       (20)       11 2022-04-14 15:41:26.000000 cleanplots-0.1.0/cleanplots.egg-info/top_level.txt
--rwx------   0 henrypinkard   (501) staff       (20)       38 2022-04-14 15:41:26.000000 cleanplots-0.1.0/setup.cfg
--rwx------   0 henrypinkard   (501) staff       (20)     1091 2022-04-14 15:40:12.000000 cleanplots-0.1.0/setup.py
+drwxrwxr-x   0 hpinkard_waller  (1015) hpinkard_waller  (1015)        0 2023-05-19 19:53:59.956944 cleanplots-0.2.0/
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)     1521 2022-10-26 01:33:44.000000 cleanplots-0.2.0/LICENSE
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)      577 2023-05-19 19:53:59.956944 cleanplots-0.2.0/PKG-INFO
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)        0 2022-10-26 01:33:44.000000 cleanplots-0.2.0/README.md
+drwxrwxr-x   0 hpinkard_waller  (1015) hpinkard_waller  (1015)        0 2023-05-19 19:53:59.956944 cleanplots-0.2.0/cleanplots/
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)       56 2022-10-26 01:33:44.000000 cleanplots-0.2.0/cleanplots/__init__.py
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)       72 2023-05-19 19:53:35.000000 cleanplots-0.2.0/cleanplots/_version.py
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)    10861 2023-05-09 16:16:46.000000 cleanplots-0.2.0/cleanplots/cleanplots.py
+drwxrwxr-x   0 hpinkard_waller  (1015) hpinkard_waller  (1015)        0 2023-05-19 19:53:59.956944 cleanplots-0.2.0/cleanplots.egg-info/
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)      577 2023-05-19 19:53:59.000000 cleanplots-0.2.0/cleanplots.egg-info/PKG-INFO
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)      266 2023-05-19 19:53:59.000000 cleanplots-0.2.0/cleanplots.egg-info/SOURCES.txt
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)        1 2023-05-19 19:53:59.000000 cleanplots-0.2.0/cleanplots.egg-info/dependency_links.txt
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)       25 2023-05-19 19:53:59.000000 cleanplots-0.2.0/cleanplots.egg-info/requires.txt
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)       11 2023-05-19 19:53:59.000000 cleanplots-0.2.0/cleanplots.egg-info/top_level.txt
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)       38 2023-05-19 19:53:59.956944 cleanplots-0.2.0/setup.cfg
+-rw-rw-r--   0 hpinkard_waller  (1015) hpinkard_waller  (1015)     1091 2022-10-26 01:33:44.000000 cleanplots-0.2.0/setup.py
```

### Comparing `cleanplots-0.1.0/setup.py` & `cleanplots-0.2.0/setup.py`

 * *Files identical despite different names*

