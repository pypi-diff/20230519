# Comparing `tmp/xuanpolicy-0.1.0.tar.gz` & `tmp/xuanpolicy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xuanpolicy-0.1.0.tar", last modified: Fri May 19 14:19:44 2023, max compression
+gzip compressed data, was "dist/xuanpolicy-0.1.1.tar", last modified: Fri May 19 15:11:33 2023, max compression
```

## Comparing `xuanpolicy-0.1.0.tar` & `xuanpolicy-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 14:19:44.000000 xuanpolicy-0.1.0/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-05-19 14:11:29.000000 xuanpolicy-0.1.0/LICENSE.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      741 2023-05-19 14:19:44.000000 xuanpolicy-0.1.0/PKG-INFO
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    14146 2023-05-19 09:59:23.000000 xuanpolicy-0.1.0/README.md
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       79 2023-05-19 14:19:44.000000 xuanpolicy-0.1.0/setup.cfg
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1200 2023-05-19 14:01:33.000000 xuanpolicy-0.1.0/setup.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 14:19:44.000000 xuanpolicy-0.1.0/xuanpolicy/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       40 2023-05-19 09:59:23.000000 xuanpolicy-0.1.0/xuanpolicy/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      780 2023-05-19 09:59:23.000000 xuanpolicy-0.1.0/xuanpolicy/main.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 14:19:44.000000 xuanpolicy-0.1.0/xuanpolicy.egg-info/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      741 2023-05-19 14:19:44.000000 xuanpolicy-0.1.0/xuanpolicy.egg-info/PKG-INFO
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      218 2023-05-19 14:19:44.000000 xuanpolicy-0.1.0/xuanpolicy.egg-info/SOURCES.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        1 2023-05-19 14:19:44.000000 xuanpolicy-0.1.0/xuanpolicy.egg-info/dependency_links.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       11 2023-05-19 14:19:44.000000 xuanpolicy-0.1.0/xuanpolicy.egg-info/top_level.txt
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 15:11:33.000000 xuanpolicy-0.1.1/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-05-19 14:11:29.000000 xuanpolicy-0.1.1/LICENSE.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      741 2023-05-19 15:11:33.000000 xuanpolicy-0.1.1/PKG-INFO
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    14146 2023-05-19 09:59:23.000000 xuanpolicy-0.1.1/README.md
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       79 2023-05-19 15:11:33.000000 xuanpolicy-0.1.1/setup.cfg
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1200 2023-05-19 15:11:20.000000 xuanpolicy-0.1.1/setup.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 15:11:33.000000 xuanpolicy-0.1.1/xuanpolicy/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       42 2023-05-19 15:09:59.000000 xuanpolicy-0.1.1/xuanpolicy/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      780 2023-05-19 09:59:23.000000 xuanpolicy-0.1.1/xuanpolicy/main.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2023-05-19 15:11:33.000000 xuanpolicy-0.1.1/xuanpolicy.egg-info/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      741 2023-05-19 15:11:33.000000 xuanpolicy-0.1.1/xuanpolicy.egg-info/PKG-INFO
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      218 2023-05-19 15:11:33.000000 xuanpolicy-0.1.1/xuanpolicy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        1 2023-05-19 15:11:33.000000 xuanpolicy-0.1.1/xuanpolicy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       11 2023-05-19 15:11:33.000000 xuanpolicy-0.1.1/xuanpolicy.egg-info/top_level.txt
```

### Comparing `xuanpolicy-0.1.0/LICENSE.txt` & `xuanpolicy-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.0/PKG-INFO` & `xuanpolicy-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xuanpolicy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Deep reinforcement learning library.
 Home-page: 
 Download-URL: 
 Author: Wenzhang Liu, Wenzhe Cai, Kun Jiang, etc.
 Author-email: 
 License: MIT
 Keywords: deep reinforcement learning,software library,platform
```

### Comparing `xuanpolicy-0.1.0/README.md` & `xuanpolicy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.0/setup.py` & `xuanpolicy-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name='xuanpolicy',
     packages=find_packages(include=['xuanpolicy']),
-    version='0.1.0',
+    version='0.1.1',
     description='Deep reinforcement learning library.',
     author='Wenzhang Liu, Wenzhe Cai, Kun Jiang, etc.',
     author_email='',
     license='MIT',
     url='',
     download_url='',
     keywords=['deep reinforcement learning', 'software library', 'platform'],
```

### Comparing `xuanpolicy-0.1.0/xuanpolicy/main.py` & `xuanpolicy-0.1.1/xuanpolicy/main.py`

 * *Files identical despite different names*

### Comparing `xuanpolicy-0.1.0/xuanpolicy.egg-info/PKG-INFO` & `xuanpolicy-0.1.1/xuanpolicy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xuanpolicy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Deep reinforcement learning library.
 Home-page: 
 Download-URL: 
 Author: Wenzhang Liu, Wenzhe Cai, Kun Jiang, etc.
 Author-email: 
 License: MIT
 Keywords: deep reinforcement learning,software library,platform
```

