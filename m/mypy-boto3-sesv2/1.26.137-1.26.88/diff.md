# Comparing `tmp/mypy-boto3-sesv2-1.26.137.tar.gz` & `tmp/mypy-boto3-sesv2-1.26.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sesv2-1.26.137.tar", last modified: Fri May 19 19:32:21 2023, max compression
+gzip compressed data, was "mypy-boto3-sesv2-1.26.88.tar", last modified: Thu Mar  9 20:38:43 2023, max compression
```

## Comparing `mypy-boto3-sesv2-1.26.137.tar` & `mypy-boto3-sesv2-1.26.88.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:32:21.676119 mypy-boto3-sesv2-1.26.137/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 19:32:05.000000 mypy-boto3-sesv2-1.26.137/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-05-19 19:32:21.676119 mypy-boto3-sesv2-1.26.137/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19506 2023-05-19 19:32:05.000000 mypy-boto3-sesv2-1.26.137/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:32:21.672119 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-19 19:32:05.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-19 19:32:05.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-19 19:32:05.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56738 2023-05-19 19:32:06.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56645 2023-05-19 19:32:06.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-19 19:32:07.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-05-19 19:32:07.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:32:05.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69150 2023-05-19 19:32:09.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69080 2023-05-19 19:32:08.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-19 19:32:05.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:32:21.676119 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-05-19 19:32:21.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-19 19:32:21.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:32:21.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:32:21.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 19:32:21.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 19:32:21.000000 mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 19:32:21.676119 mypy-boto3-sesv2-1.26.137/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-19 19:32:05.000000 mypy-boto3-sesv2-1.26.137/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:43.962381 mypy-boto3-sesv2-1.26.88/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20945 2023-03-09 20:38:43.958381 mypy-boto3-sesv2-1.26.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19466 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:43.958381 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56176 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56084 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68871 2023-03-09 20:38:28.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68801 2023-03-09 20:38:27.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:43.958381 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20945 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-09 20:38:43.000000 mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 20:38:43.962381 mypy-boto3-sesv2-1.26.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-09 20:38:24.000000 mypy-boto3-sesv2-1.26.88/setup.py
```

### Comparing `mypy-boto3-sesv2-1.26.137/LICENSE` & `mypy-boto3-sesv2-1.26.88/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-sesv2-1.26.137/PKG-INFO` & `mypy-boto3-sesv2-1.26.88/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.26.137
-Summary: Type annotations for boto3.SESV2 1.26.137 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.88
+Summary: Type annotations for boto3.SESV2 1.26.88 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sesv2"></a>
 
 # mypy-boto3-sesv2
 
 [![PyPI - mypy-boto3-sesv2](https://img.shields.io/pypi/v/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sesv2?color=blue)](https://pypistats.org/packages/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.26.137](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -434,15 +434,14 @@
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
-    PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
@@ -546,42 +545,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-sesv2-1.26.137/README.md` & `mypy-boto3-sesv2-1.26.88/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sesv2"></a>
 
 # mypy-boto3-sesv2
 
 [![PyPI - mypy-boto3-sesv2](https://img.shields.io/pypi/v/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sesv2?color=blue)](https://pypistats.org/packages/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.26.137](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -402,15 +402,14 @@
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
-    PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
@@ -514,42 +513,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/__main__.py` & `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SESV2 1.26.137\nVersion:         1.26.137\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SESV2 1.26.88\nVersion:         1.26.88\nBuilder version:"
+        " 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.137")
+    print("1.26.88")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/client.py` & `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -902,24 +902,14 @@
         """
         Move a dedicated IP address to an existing dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_in_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_in_pool)
         """
 
-    def put_dedicated_ip_pool_scaling_attributes(
-        self, *, PoolName: str, ScalingMode: ScalingModeType
-    ) -> Dict[str, Any]:
-        """
-        Used to convert a dedicated IP pool to a different scaling mode.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_pool_scaling_attributes)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_pool_scaling_attributes)
-        """
-
     def put_dedicated_ip_warmup_attributes(
         self, *, Ip: str, WarmupPercentage: int
     ) -> Dict[str, Any]:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/sesv2-2019-09-27/PutDedicatedIpWarmupAttributes).
```

### Comparing `mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/client.pyi` & `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -829,23 +829,14 @@
     def put_dedicated_ip_in_pool(self, *, Ip: str, DestinationPoolName: str) -> Dict[str, Any]:
         """
         Move a dedicated IP address to an existing dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_in_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_in_pool)
         """
-    def put_dedicated_ip_pool_scaling_attributes(
-        self, *, PoolName: str, ScalingMode: ScalingModeType
-    ) -> Dict[str, Any]:
-        """
-        Used to convert a dedicated IP pool to a different scaling mode.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_pool_scaling_attributes)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_pool_scaling_attributes)
-        """
     def put_dedicated_ip_warmup_attributes(
         self, *, Ip: str, WarmupPercentage: int
     ) -> Dict[str, Any]:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/sesv2-2019-09-27/PutDedicatedIpWarmupAttributes).
```

### Comparing `mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/literals.py` & `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BehaviorOnMxFailureType",
     "BulkEmailStatusType",
     "ContactLanguageType",
     "ContactListImportActionType",
     "DataFormatType",
     "DeliverabilityDashboardAccountStatusType",
@@ -56,15 +55,14 @@
     "WarmupStatusType",
     "SESV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 BehaviorOnMxFailureType = Literal["REJECT_MESSAGE", "USE_DEFAULT_VALUE"]
 BulkEmailStatusType = Literal[
     "ACCOUNT_DAILY_QUOTA_EXCEEDED",
     "ACCOUNT_SENDING_PAUSED",
     "ACCOUNT_SUSPENDED",
     "ACCOUNT_THROTTLED",
     "CONFIGURATION_SET_NOT_FOUND",
@@ -296,15 +294,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -340,15 +337,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -367,15 +363,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -462,15 +457,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/literals.pyi` & `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "BehaviorOnMxFailureType",
     "BulkEmailStatusType",
     "ContactLanguageType",
     "ContactListImportActionType",
     "DataFormatType",
     "DeliverabilityDashboardAccountStatusType",
@@ -55,14 +56,15 @@
     "WarmupStatusType",
     "SESV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 BehaviorOnMxFailureType = Literal["REJECT_MESSAGE", "USE_DEFAULT_VALUE"]
 BulkEmailStatusType = Literal[
     "ACCOUNT_DAILY_QUOTA_EXCEEDED",
     "ACCOUNT_SENDING_PAUSED",
     "ACCOUNT_SUSPENDED",
     "ACCOUNT_THROTTLED",
     "CONFIGURATION_SET_NOT_FOUND",
@@ -294,15 +296,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -338,15 +339,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -365,15 +365,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -460,15 +459,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/type_defs.py` & `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,14 @@
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
     "PutConfigurationSetSendingOptionsRequestRequestTypeDef",
     "PutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
-    "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "PutSuppressedDestinationRequestRequestTypeDef",
     "ReplacementTemplateTypeDef",
@@ -1354,22 +1353,14 @@
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
 
-PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef = TypedDict(
-    "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
-    {
-        "PoolName": str,
-        "ScalingMode": ScalingModeType,
-    },
-)
-
 PutDedicatedIpWarmupAttributesRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     {
         "Ip": str,
         "WarmupPercentage": int,
     },
 )
```

### Comparing `mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2/type_defs.pyi` & `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,14 @@
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
     "PutConfigurationSetSendingOptionsRequestRequestTypeDef",
     "PutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
-    "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "PutSuppressedDestinationRequestRequestTypeDef",
     "ReplacementTemplateTypeDef",
@@ -1329,22 +1328,14 @@
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
 
-PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef = TypedDict(
-    "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
-    {
-        "PoolName": str,
-        "ScalingMode": ScalingModeType,
-    },
-)
-
 PutDedicatedIpWarmupAttributesRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     {
         "Ip": str,
         "WarmupPercentage": int,
     },
 )
```

### Comparing `mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2.egg-info/PKG-INFO` & `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.26.137
-Summary: Type annotations for boto3.SESV2 1.26.137 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.88
+Summary: Type annotations for boto3.SESV2 1.26.88 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sesv2"></a>
 
 # mypy-boto3-sesv2
 
 [![PyPI - mypy-boto3-sesv2](https://img.shields.io/pypi/v/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sesv2?color=blue)](https://pypistats.org/packages/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.26.137](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -434,15 +434,14 @@
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
-    PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
@@ -546,42 +545,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-sesv2-1.26.137/mypy_boto3_sesv2.egg-info/SOURCES.txt` & `mypy-boto3-sesv2-1.26.88/mypy_boto3_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.26.137/setup.py` & `mypy-boto3-sesv2-1.26.88/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-sesv2.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-sesv2",
-    version="1.26.137",
+    version="1.26.88",
     packages=["mypy_boto3_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SESV2 1.26.137 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SESV2 1.26.88 service generated with mypy-boto3-builder 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

