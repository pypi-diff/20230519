# Comparing `tmp/upconan-1.0.1.tar.gz` & `tmp/upconan-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upconan-1.0.1.tar", last modified: Fri May 19 13:18:15 2023, max compression
+gzip compressed data, was "upconan-1.0.2.tar", last modified: Fri May 19 13:20:55 2023, max compression
```

## Comparing `upconan-1.0.1.tar` & `upconan-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:15.265373 upconan-1.0.1/
--rw-rw-rw-   0        0        0     1062 2023-05-19 13:12:37.000000 upconan-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      452 2023-05-19 13:18:15.264371 upconan-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-05-19 13:13:20.000000 upconan-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 13:18:15.265373 upconan-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      813 2023-05-19 13:17:52.000000 upconan-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:15.264371 upconan-1.0.1/upconan.egg-info/
--rw-rw-rw-   0        0        0      452 2023-05-19 13:18:15.000000 upconan-1.0.1/upconan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-19 13:18:15.000000 upconan-1.0.1/upconan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 13:18:15.000000 upconan-1.0.1/upconan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-19 13:18:15.000000 upconan-1.0.1/upconan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-19 13:18:15.000000 upconan-1.0.1/upconan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-19 13:18:15.000000 upconan-1.0.1/upconan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 13:18:15.000000 upconan-1.0.1/upconan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 13:20:54.999582 upconan-1.0.2/
+-rw-rw-rw-   0        0        0     1062 2023-05-19 13:12:37.000000 upconan-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      452 2023-05-19 13:20:54.999582 upconan-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-05-19 13:13:20.000000 upconan-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 13:20:54.999582 upconan-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      813 2023-05-19 13:20:40.000000 upconan-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:20:54.987583 upconan-1.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:21:11.000000 upconan-1.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0     4604 2023-05-19 13:08:26.000000 upconan-1.0.2/src/upconan.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:20:54.998583 upconan-1.0.2/upconan.egg-info/
+-rw-rw-rw-   0        0        0      452 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/top_level.txt
```

### Comparing `upconan-1.0.1/LICENSE` & `upconan-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upconan-1.0.1/setup.py` & `upconan-1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='upconan',
-    version="1.0.1",
+    version="1.0.2",
     description="一个更新conanfile的便捷工具",
     long_description="""从剪贴板复制conan包信息，更新当前路径下的conanfile.py或conanfile.txt文件中对应的conan包版本""",
     keywords='python conan',
     author='leytou',
     author_email='hi_litao@163.com',
     url='https://github.com/leytou/upconan',
     license='MIT',
```

