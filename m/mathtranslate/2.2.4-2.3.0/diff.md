# Comparing `tmp/mathtranslate-2.2.4.tar.gz` & `tmp/mathtranslate-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.2.4.tar", last modified: Thu May 18 23:14:54 2023, max compression
+gzip compressed data, was "mathtranslate-2.3.0.tar", last modified: Fri May 19 00:38:12 2023, max compression
```

## Comparing `mathtranslate-2.2.4.tar` & `mathtranslate-2.3.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.202137 mathtranslate-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:14:54.202137 mathtranslate-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.792152 mathtranslate-2.3.0/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/setup.py
```

### Comparing `mathtranslate-2.2.4/LICENSE` & `mathtranslate-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/PKG-INFO` & `mathtranslate-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.2.4
+Version: 2.3.0
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.4 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.0 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.2.4/README.md` & `mathtranslate-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/config.py` & `mathtranslate-2.3.0/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/encoding.py` & `mathtranslate-2.3.0/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/process_file.py` & `mathtranslate-2.3.0/mathtranslate/process_file.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/process_latex.py` & `mathtranslate-2.3.0/mathtranslate/process_latex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/process_text.py` & `mathtranslate-2.3.0/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencent.py` & `mathtranslate-2.3.0/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/translate.py` & `mathtranslate-2.3.0/mathtranslate/translate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python
+from . import __version__
 from . import process_latex
 from . import process_text
+from . import cache
 from .process_latex import environment_list, command_list, format_list
 from .process_text import char_limit
 from .encoding import get_file_encoding
 import time
 import re
 import tqdm
 
@@ -17,14 +19,15 @@
 default_end = r'''
 \end{document}
 '''
 
 
 class TextTranslator:
     def __init__(self, engine, language_to, language_from):
+        self.engine = engine
         if engine == 'google':
             import mtranslate as translator
         elif engine == 'tencent':
             from mathtranslate.tencent import Translator
             translator = Translator()
         else:
             assert False, "engine must be google or tencent"
@@ -169,14 +172,20 @@
         '''
         text, objs = process_latex.replace_latex_objects(latex)
         paragraphs_text = re.split(r'\n\n+', text)
         paragraphs_latex = [process_latex.recover_latex_objects(paragraph_text, objs)[0] for paragraph_text in paragraphs_text]
         return paragraphs_latex
 
     def translate_full_latex(self, latex_original, make_complete=True):
+        cache.remove_extra()
+        hash_key = cache.deterministic_hash((latex_original, __version__, self.translator.engine, self.translator.language_from, self.translator.language_to))
+        if cache.is_cached(hash_key):
+            print('Cache is found')
+        cache.create_cache(hash_key)
+
         self.nbad = 0
         self.ntotal = 0
 
         latex_original = process_latex.remove_tex_comments(latex_original)
         latex_original = process_latex.process_newcommands(latex_original)
 
         latex_original = process_latex.replace_accent(latex_original)
@@ -201,15 +210,19 @@
 
         latex_original_paragraphs = self.split_latex_to_paragraphs(latex_original)
         latex_translated_paragraphs = []
 
         self.num = 0
         for latex_original_paragraph in tqdm.tqdm(latex_original_paragraphs):
             try:
-                latex_translated_paragraph = self.translate_paragraph_latex(latex_original_paragraph)
+                hash_key_paragraph = cache.deterministic_hash(latex_original_paragraph)
+                latex_translated_paragraph = cache.load_paragraph(hash_key, hash_key_paragraph)
+                if latex_translated_paragraph is None:
+                    latex_translated_paragraph = self.translate_paragraph_latex(latex_original_paragraph)
+                    cache.write_paragraph(hash_key, hash_key_paragraph, latex_translated_paragraph)
                 latex_translated_paragraphs.append(latex_translated_paragraph)
             except BaseException as e:
                 print('Error found in Parapragh', self.num)
                 print('Content')
                 print(latex_original_paragraph)
                 raise e
             self.num += 1
```

### Comparing `mathtranslate-2.2.4/mathtranslate/translate_arxiv.py` & `mathtranslate-2.3.0/mathtranslate/translate_arxiv.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/translate_tex.py` & `mathtranslate-2.3.0/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/upload_overleaf.py` & `mathtranslate-2.3.0/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate/utils.py` & `mathtranslate-2.3.0/mathtranslate/utils.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.4/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.3.0/mathtranslate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.2.4
+Version: 2.3.0
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.4 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.0 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.2.4/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-2.3.0/mathtranslate.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 mathtranslate/__init__.py
+mathtranslate/cache.py
 mathtranslate/config.py
 mathtranslate/encoding.py
 mathtranslate/process_file.py
 mathtranslate/process_latex.py
 mathtranslate/process_text.py
 mathtranslate/tencent.py
 mathtranslate/translate.py
```

### Comparing `mathtranslate-2.2.4/setup.py` & `mathtranslate-2.3.0/setup.py`

 * *Files identical despite different names*

