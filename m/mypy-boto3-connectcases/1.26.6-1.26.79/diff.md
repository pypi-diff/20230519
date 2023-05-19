# Comparing `tmp/mypy-boto3-connectcases-1.26.6.tar.gz` & `tmp/mypy-boto3-connectcases-1.26.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcases-1.26.6.tar", last modified: Wed Nov  9 20:50:02 2022, max compression
+gzip compressed data, was "mypy-boto3-connectcases-1.26.79.tar", last modified: Fri Feb 24 21:22:49 2023, max compression
```

## Comparing `mypy-boto3-connectcases-1.26.6.tar` & `mypy-boto3-connectcases-1.26.79.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 20:50:02.819553 mypy-boto3-connectcases-1.26.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16181 2022-11-09 20:50:02.819553 mypy-boto3-connectcases-1.26.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14726 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 20:50:02.819553 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21690 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    21652 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7783 2022-11-09 20:48:58.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7781 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3392 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    29282 2022-11-09 20:48:58.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    29238 2022-11-09 20:48:58.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-09 20:48:57.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 20:50:02.819553 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16181 2022-11-09 20:50:02.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-09 20:50:02.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 20:50:02.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 20:50:02.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-09 20:50:02.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-09 20:50:02.000000 mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 20:50:02.819553 mypy-boto3-connectcases-1.26.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-11-09 20:48:56.000000 mypy-boto3-connectcases-1.26.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.729198 mypy-boto3-connectcases-1.26.79/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-02-24 21:22:49.729198 mypy-boto3-connectcases-1.26.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.729198 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-02-24 21:22:07.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29452 2023-02-24 21:22:07.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29408 2023-02-24 21:22:07.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.729198 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 21:22:49.000000 mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 21:22:49.729198 mypy-boto3-connectcases-1.26.79/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-02-24 21:22:06.000000 mypy-boto3-connectcases-1.26.79/setup.py
```

### Comparing `mypy-boto3-connectcases-1.26.6/LICENSE` & `mypy-boto3-connectcases-1.26.79/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.6/PKG-INFO` & `mypy-boto3-connectcases-1.26.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.26.6
-Summary: Type annotations for boto3.ConnectCases 1.26.6 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.79
+Summary: Type annotations for boto3.ConnectCases 1.26.79 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.26.6](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,14 +345,15 @@
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateFieldRequestRequestTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
+    DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.26.6/README.md` & `mypy-boto3-connectcases-1.26.79/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.26.6](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,14 +313,15 @@
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateFieldRequestRequestTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
+    DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/__init__.py` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/__init__.pyi` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/__main__.py` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCases 1.26.6\nVersion:         1.26.6\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.ConnectCases 1.26.79\nVersion:         1.26.79\nBuilder"
+        " version: 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.6")
+    print("1.26.79")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/client.py` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,22 @@
         """
         Creates a template in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_template)
         """
 
+    def delete_domain(self, *, domainId: str) -> Dict[str, Any]:
+        """
+        Deletes a domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_domain)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_domain)
+        """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
```

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/client.pyi` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,21 @@
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_template)
         """
+    def delete_domain(self, *, domainId: str) -> Dict[str, Any]:
+        """
+        Deletes a domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_domain)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_domain)
+        """
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
```

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/literals.py` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CommentBodyTextTypeType",
     "DomainStatusType",
     "FieldNamespaceType",
     "FieldTypeType",
     "OrderType",
     "RelatedItemTypeType",
@@ -32,15 +31,14 @@
     "ConnectCasesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CommentBodyTextTypeType = Literal["Text/Plain"]
 DomainStatusType = Literal["Active", "CreationFailed", "CreationInProgress"]
 FieldNamespaceType = Literal["Custom", "System"]
 FieldTypeType = Literal["Boolean", "DateTime", "Number", "SingleSelect", "Text"]
 OrderType = Literal["Asc", "Desc"]
 RelatedItemTypeType = Literal["Comment", "Contact"]
 SearchCasesPaginatorName = Literal["search_cases"]
@@ -67,14 +65,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -84,27 +83,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -133,14 +136,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -188,14 +192,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -206,30 +211,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -261,28 +269,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -310,51 +322,58 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -377,8 +396,16 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["search_cases", "search_related_items"]
-RegionName = Literal["us-east-1", "us-west-2"]
+RegionName = Literal[
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-west-2",
+    "us-east-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/literals.pyi` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "CommentBodyTextTypeType",
     "DomainStatusType",
     "FieldNamespaceType",
     "FieldTypeType",
     "OrderType",
     "RelatedItemTypeType",
@@ -31,14 +32,15 @@
     "ConnectCasesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 CommentBodyTextTypeType = Literal["Text/Plain"]
 DomainStatusType = Literal["Active", "CreationFailed", "CreationInProgress"]
 FieldNamespaceType = Literal["Custom", "System"]
 FieldTypeType = Literal["Boolean", "DateTime", "Number", "SingleSelect", "Text"]
 OrderType = Literal["Asc", "Desc"]
 RelatedItemTypeType = Literal["Comment", "Contact"]
 SearchCasesPaginatorName = Literal["search_cases"]
@@ -65,14 +67,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -82,27 +85,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -131,14 +138,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -186,14 +194,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -204,30 +213,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -259,28 +271,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -308,51 +324,58 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -375,8 +398,16 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["search_cases", "search_related_items"]
-RegionName = Literal["us-east-1", "us-west-2"]
+RegionName = Literal[
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-west-2",
+    "us-east-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/paginator.py` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/paginator.pyi` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/type_defs.py` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateFieldRequestRequestTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
+    "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
@@ -291,14 +292,21 @@
 RequiredFieldTypeDef = TypedDict(
     "RequiredFieldTypeDef",
     {
         "fieldId": str,
     },
 )
 
+DeleteDomainRequestRequestTypeDef = TypedDict(
+    "DeleteDomainRequestRequestTypeDef",
+    {
+        "domainId": str,
+    },
+)
+
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
```

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases/type_defs.pyi` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateFieldRequestRequestTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
+    "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
@@ -284,14 +285,21 @@
 RequiredFieldTypeDef = TypedDict(
     "RequiredFieldTypeDef",
     {
         "fieldId": str,
     },
 )
 
+DeleteDomainRequestRequestTypeDef = TypedDict(
+    "DeleteDomainRequestRequestTypeDef",
+    {
+        "domainId": str,
+    },
+)
+
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
```

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases.egg-info/PKG-INFO` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.26.6
-Summary: Type annotations for boto3.ConnectCases 1.26.6 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.79
+Summary: Type annotations for boto3.ConnectCases 1.26.79 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.26.6](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,14 +345,15 @@
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateFieldRequestRequestTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
+    DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.26.6/mypy_boto3_connectcases.egg-info/SOURCES.txt` & `mypy-boto3-connectcases-1.26.79/mypy_boto3_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.26.6/setup.py` & `mypy-boto3-connectcases-1.26.79/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-connectcases",
-    version="1.26.6",
+    version="1.26.79",
     packages=["mypy_boto3_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectCases 1.26.6 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.ConnectCases 1.26.79 service generated with mypy-boto3-builder"
+        " 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 connectcases type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_connectcases": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_connectcases": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

