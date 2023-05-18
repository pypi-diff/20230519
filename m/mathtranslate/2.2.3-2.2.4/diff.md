# Comparing `tmp/mathtranslate-2.2.3.tar.gz` & `tmp/mathtranslate-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.2.3.tar", last modified: Thu May 18 00:31:59 2023, max compression
+gzip compressed data, was "mathtranslate-2.2.4.tar", last modified: Thu May 18 23:14:54 2023, max compression
```

## Comparing `mathtranslate-2.2.3.tar` & `mathtranslate-2.2.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:31:59.125939 mathtranslate-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-18 00:31:59.125939 mathtranslate-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:31:59.117939 mathtranslate-2.2.3/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:31:59.121939 mathtranslate-2.2.3/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:31:59.121939 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:31:59.121939 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:31:59.121939 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:31:59.121939 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:31:59.121939 mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:31:59.125939 mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:31:59.121939 mathtranslate-2.2.3/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-18 00:31:59.000000 mathtranslate-2.2.3/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-18 00:31:59.000000 mathtranslate-2.2.3/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 00:31:59.000000 mathtranslate-2.2.3/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 00:31:59.000000 mathtranslate-2.2.3/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 00:31:59.000000 mathtranslate-2.2.3/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 00:31:59.000000 mathtranslate-2.2.3/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 00:31:59.125939 mathtranslate-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-18 00:31:34.000000 mathtranslate-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.202137 mathtranslate-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:54.198137 mathtranslate-2.2.4/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 23:14:54.000000 mathtranslate-2.2.4/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:14:54.202137 mathtranslate-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-18 23:14:30.000000 mathtranslate-2.2.4/setup.py
```

### Comparing `mathtranslate-2.2.3/LICENSE` & `mathtranslate-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/PKG-INFO` & `mathtranslate-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.2.3
+Version: 2.2.4
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
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.3 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.4 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.2.3/README.md` & `mathtranslate-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/config.py` & `mathtranslate-2.2.4/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/encoding.py` & `mathtranslate-2.2.4/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/process_file.py` & `mathtranslate-2.2.4/mathtranslate/process_file.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/process_latex.py` & `mathtranslate-2.2.4/mathtranslate/process_latex.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
 pattern_env = get_pattern_env(r'.*?')  # \begin{xxx} \end{xxx}, group 1: name, group 2: option, group 3: content
 pattern_command_full = get_pattern_command_full(match_command_name)   # \xxx[xxx]{xxx} and \xxx{xxx}, group 1: name, group 2: option, group 4: content
 pattern_command_simple = rf'\\({match_command_name})'  # \xxx, group 1: name
 pattern_brace = get_pattern_brace(0)  # {xxx}, group 1: content
 pattern_newcommand = rf'\\(?:newcommand|def){spaces}(?:\{{\\([a-zA-Z]+)\}}|\\([a-zA-Z]+)){spaces}(?:\[(\d)\])?{spaces}({get_pattern_brace(4)})'  # \newcommand{name}[n_arguments]{content}, group 1/2: name, group 3: n_arguments, group 5: content
 
-pattern_set1 = rf'\\set[a-zA-Z]*{spaces}\\[a-zA-Z]+{spaces}\{{.*\}}'
-pattern_set2 = rf'\\set[a-zA-Z]*{spaces}\{{\\[a-zA-Z]+\}}{spaces}\{{.*\}}'
+pattern_set1 = rf'\\set[a-zA-Z]*{spaces}\\[a-zA-Z]+{spaces}\{{.*?\}}'
+pattern_set2 = rf'\\set[a-zA-Z]*{spaces}\{{\\[a-zA-Z]+\}}{spaces}\{{.*?\}}'
 pattern_theorem = r"\\newtheorem[ \t]*\{(.+?)\}"  # \newtheorem{xxx}, group 1: name
 pattern_accent = r"\\([`'\"^~=.])(?:\{([a-zA-Z])\}|([a-zA-Z]))"  # match special characters with accents, group 1: accent, group 2/3: normal character
 match_code_accent = rf'{math_code}([A-Z]{{2}})([a-zA-Z])'  # group 1: accent name, group 2: normal character, e.g. \"o or \"{o}
 list_special = ['\\', '%', '&', '#', '$', '{', '}', ' ']  # all special characters in form of \x
 
 special_character_forward = {
     '\\': 'BS',
```

### Comparing `mathtranslate-2.2.3/mathtranslate/process_text.py` & `mathtranslate-2.2.4/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencent.py` & `mathtranslate-2.2.4/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-2.2.4/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/translate.py` & `mathtranslate-2.2.4/mathtranslate/translate.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/translate_arxiv.py` & `mathtranslate-2.2.4/mathtranslate/translate_arxiv.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/translate_tex.py` & `mathtranslate-2.2.4/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/upload_overleaf.py` & `mathtranslate-2.2.4/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate/utils.py` & `mathtranslate-2.2.4/mathtranslate/utils.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.2.4/mathtranslate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.2.3
+Version: 2.2.4
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
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.3 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.4 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.2.3/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-2.2.4/mathtranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.3/setup.py` & `mathtranslate-2.2.4/setup.py`

 * *Files identical despite different names*

