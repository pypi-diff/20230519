# Comparing `tmp/alibabacloud_dop20221130_py2-1.0.0.tar.gz` & `tmp/alibabacloud_dop20221130_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dop20221130_py2-1.0.0.tar", last modified: Fri May 19 06:17:30 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dop20221130_py2-1.0.1.tar", last modified: Fri May 19 06:25:38 2023, max compression
```

## Comparing `alibabacloud_dop20221130_py2-1.0.0.tar` & `alibabacloud_dop20221130_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5155 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130/client.py
--rw-r--r--   0 root         (0) root         (0)    14526 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2023-05-19 06:17:30.000000 alibabacloud_dop20221130_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130/client.py
+-rw-r--r--   0 root         (0) root         (0)    14526 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-05-19 06:25:38.000000 alibabacloud_dop20221130_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_dop20221130_py2-1.0.0/LICENSE` & `alibabacloud_dop20221130_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dop20221130_py2-1.0.0/PKG-INFO` & `alibabacloud_dop20221130_py2-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dop20221130_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud dop (20221130) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dop20221130_py2-1.0.0/README-CN.md` & `alibabacloud_dop20221130_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dop20221130_py2-1.0.0/README.md` & `alibabacloud_dop20221130_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130/client.py` & `alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130/models.py` & `alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dop20221130_py2-1.0.0/alibabacloud_dop20221130_py2.egg-info/PKG-INFO` & `alibabacloud_dop20221130_py2-1.0.1/alibabacloud_dop20221130_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dop20221130-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud dop (20221130) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dop20221130_py2-1.0.0/setup.py` & `alibabacloud_dop20221130_py2-1.0.1/setup.py`

 * *Files identical despite different names*

