# Comparing `tmp/worktoy-0.28.8.tar.gz` & `tmp/worktoy-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worktoy-0.28.8.tar", last modified: Sun May 14 11:32:39 2023, max compression
+gzip compressed data, was "worktoy-0.30.0.tar", last modified: Thu May 18 22:43:08 2023, max compression
```

## Comparing `worktoy-0.28.8.tar` & `worktoy-0.30.0.tar`

### file list

```diff
@@ -1,34 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.090558 worktoy-0.28.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-14 11:32:30.000000 worktoy-0.28.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 11:32:39.090558 worktoy-0.28.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-14 11:32:30.000000 worktoy-0.28.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-14 11:32:30.000000 worktoy-0.28.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-14 11:32:39.090558 worktoy-0.28.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.086558 worktoy-0.28.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.086558 worktoy-0.28.8/src/worktoy/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_anywayuwantit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_callmemaybe.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_maybe.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_maybeType.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_maybeTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_searchKeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_stringlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.090558 worktoy-0.28.8/src/worktoy/mockdata/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/mockdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/mockdata/_intfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/mockdata/_strfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.090558 worktoy-0.28.8/src/worktoy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 11:32:39.000000 worktoy-0.28.8/src/worktoy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-14 11:32:39.000000 worktoy-0.28.8/src/worktoy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:32:39.000000 worktoy-0.28.8/src/worktoy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 11:32:39.000000 worktoy-0.28.8/src/worktoy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.090558 worktoy-0.28.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__callmemaybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__intfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__maybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__maybeType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__maybeTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__searchKeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__strfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__stringlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.642198 worktoy-0.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-18 22:42:59.000000 worktoy-0.30.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-18 22:43:08.642198 worktoy-0.30.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-18 22:42:59.000000 worktoy-0.30.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-18 22:42:59.000000 worktoy-0.30.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-18 22:43:08.642198 worktoy-0.30.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.634198 worktoy-0.30.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.638198 worktoy-0.30.0/src/worktoy/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_anywayuwantit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_hereismynumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_maybeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_maybeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_monospace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_overload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_overloadlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_parameterlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_parsify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_parsifyerrors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_searchKeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_searchterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_stringlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_textbetween.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_typenames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_workdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_workdictmeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_workmeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.638198 worktoy-0.30.0/src/worktoy/mockdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/mockdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/mockdata/_intfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/mockdata/_strfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.642198 worktoy-0.30.0/src/worktoy/sharperexceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/sharperexceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/sharperexceptions/_argumenterror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/sharperexceptions/_parsingerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/sharperexceptions/_readonlyerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/sharperexceptions/_testexception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.638198 worktoy-0.30.0/src/worktoy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-18 22:43:08.000000 worktoy-0.30.0/src/worktoy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-18 22:43:08.000000 worktoy-0.30.0/src/worktoy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:43:08.000000 worktoy-0.30.0/src/worktoy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 22:43:08.000000 worktoy-0.30.0/src/worktoy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.642198 worktoy-0.30.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__ArgumentError.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__intfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__maybeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__maybeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__readonlyerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__searchKeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__searchterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__strfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__stringlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__textbetween.py
```

### Comparing `worktoy-0.28.8/LICENSE` & `worktoy-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/PKG-INFO` & `worktoy-0.30.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worktoy
-Version: 0.28.8
+Version: 0.30.0
 Summary: Collection of Utilities
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
 Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `worktoy-0.28.8/README.md` & `worktoy-0.30.0/README.md`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/pyproject.toml` & `worktoy-0.30.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools>=63.2']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "worktoy"
-version = "0.28.8"
+version = "0.30.0"
 authors = [
     { name = "Asger Jon Vistisen", email = "asgerjon2@gmail.com" },
 ]
 description = "Collection of Utilities"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `worktoy-0.28.8/setup.cfg` & `worktoy-0.30.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [METADATA]
 name = WorkToy
-version = 0.28.8
+version = 0.30.0
 author = Asger Jon Vistisen
 author_email = asgerjon2@gmail.com
 description = A Collection of Utilities
 long_description = file:README.md,LICENSE
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `worktoy-0.28.8/src/worktoy/_anywayuwantit.py` & `worktoy-0.30.0/src/worktoy/_anywayuwantit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """AnywayUWantIt provides a simplified abstract metaclass"""
 #  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
+#  Copyright (c) 2023 Asger Jon Vistisen 
 from __future__ import annotations
 
 from _py_abc import ABCMeta
 from abc import ABCMeta as ABCMetaLOL
 from typing import Any
 
 _modules = [ABCMetaLOL]
```

### Comparing `worktoy-0.28.8/src/worktoy/_callmemaybe.py` & `worktoy-0.30.0/src/worktoy/_callmemaybe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 """This abstract metaclass registers any callable object as an instance."""
 #  MIT License
 #  Copyright (c) 2023 Asger Jon Vistisen
 from __future__ import annotations
 
-from typing import Any, NoReturn
+from typing import Any, NoReturn, Callable, Never
+from warnings import warn
 
-from worktoy import AnywayUWantIt, searchKeys, maybeType, maybe
+from worktoy import AnywayUWantIt, searchKeys, maybeType, maybe, monoSpace
 
 
 class CallMeMaybe(metaclass=AnywayUWantIt):
   """This abstract metaclass registers any callable object as an instance."""
 
   _explicits = []
   _callables = []
   _unCallables = []
+  _unCallableFunctions = []
 
   @staticmethod
   def recognizeInstance(instance: Any = None) -> bool:
     """Recognizing anything callable as an instance"""
+    for callableType in CallMeMaybe._callables:
+      if isinstance(instance, callableType):
+        return True
+    for unCallableType in CallMeMaybe._unCallables:
+      if isinstance(instance, unCallableType):
+        return False
+    if instance in CallMeMaybe._unCallableFunctions:
+      return False
+    # if isinstance(instance, Callable)
+    if isinstance(instance, Callable):
+      return True
     callableFlag = getattr(instance, '__isCallable__', None)
     if callableFlag is not None:
       if not callableFlag:
         return False
+      return True
     if isinstance(instance, (int, float, str, complex)):
       return False
     if isinstance(instance, (tuple, dict, list, set)):
       return False
-    for callableType in CallMeMaybe._callables:
-      if isinstance(instance, callableType):
-        return True
-    for callableType in CallMeMaybe._unCallables:
-      if isinstance(instance, callableType):
-        return False
     if instance is None:
       return False
     classId = getattr(instance, '__class__', None)
     instanceName = getattr(instance, '__name__', None)
     if instanceName is None:
-      e = """Unable to recognize instance name"""
-      raise ValueError(e)
+      return True
     if classId is None:
       e = """Unable to recognize class of instance"""
       raise ValueError(e)
     className = getattr(classId, '__name__', None)
     if className is None:
       e = """Unable to recognize name of instance class"""
       raise ValueError(e)
@@ -62,31 +69,60 @@
     cls._unCallables.append(other)
 
   @classmethod
   def registerCallable(cls, other: type) -> NoReturn:
     """Registers other type as being explicitly callable"""
     cls._callables.append(other)
 
+  @classmethod
+  def registerUnCallableFunction(cls, other: Callable) -> NoReturn:
+    """Registers other function as unCallable"""
+    cls._unCallableFunctions.append(other)
+
+  @classmethod
+  def registerCallableFunction(cls, *_) -> Never:
+    """LOL"""
+    msg = """Do not use this method 'registerCallableFunction' as any 
+    function this method would accept is already callable. In a future 
+    update this will raise an error."""
+    warn(PendingDeprecationWarning(warn(msg)))
+
   def __init__(self, *args, **kwargs) -> None:
     callableKwarg = searchKeys('callable', 'callMeMaybe') @ bool >> kwargs
     callableArg = maybeType(str, *args)
     if callableArg is not None:
       if callableArg == 'callable':
         callableArg = True
       elif callableArg in ['Not-callable', 'not callable']:
         callableArg = False
     callableDefault = True
     self._callableFlag = maybe(callableKwarg, callableArg, callableDefault)
 
-  def __call__(self, func: Any) -> Any:
+  def __call__(self, other: Callable | type) -> Any:
     """Use as a function decorator. By default, the decorated function are
     regarded as callable. Change this by setting keyword argument
     'callable' to False so that a decorated function will not be regarded
     as a callable. """
-    if isinstance(func, type):
-      if maybe(self._callableFlag, True):
-        CallMeMaybe.registerCallable(func)
-        return func
-      CallMeMaybe.registerUnCallable(func)
-      return func
-    setattr(func, '__isCallable__', maybe(self._callableFlag, True))
-    return func
+    isCallable = isinstance(other, Callable)
+    isType = isinstance(other, type)
+    if isType:
+      return maybe(self._handleType(other), other)
+    if isCallable:
+      return maybe(self._handleCallable(other), other)
+    msg = """CallMeMaybe should decorate classes or functions, not %s"""
+    raise TypeError(monoSpace(msg % type(other)))
+
+  def _handleCallable(self, func: Callable) -> NoReturn:
+    """Handles the callables."""
+    if self._callableFlag is not None:
+      if self._callableFlag:
+        return self.registerCallableFunction(func)
+      return self.registerUnCallableFunction(func)
+    return self.registerUnCallableFunction(func)
+
+  def _handleType(self, type_: type) -> NoReturn:
+    """Handles types"""
+    if self._callableFlag is not None:
+      if self._callableFlag:
+        return self.registerCallable(type_)
+      return self.registerUnCallable(type_)
+    return self.registerUnCallable(type_)
```

### Comparing `worktoy-0.28.8/src/worktoy/_maybeTypes.py` & `worktoy-0.30.0/src/worktoy/_maybeTypes.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/src/worktoy/_searchKeys.py` & `worktoy-0.30.0/src/worktoy/_searchKeys.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/src/worktoy/_stringlist.py` & `worktoy-0.30.0/src/worktoy/_stringlist.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/src/worktoy/mockdata/_intfactory.py` & `worktoy-0.30.0/src/worktoy/mockdata/_intfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/src/worktoy/mockdata/_strfactory.py` & `worktoy-0.30.0/src/worktoy/mockdata/_strfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/src/worktoy.egg-info/PKG-INFO` & `worktoy-0.30.0/src/worktoy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worktoy
-Version: 0.28.8
+Version: 0.30.0
 Summary: Collection of Utilities
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
 Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `worktoy-0.28.8/tests/test__callmemaybe.py` & `worktoy-0.30.0/tests/test__callmemaybe.py`

 * *Files 20% similar despite different names*

```diff
@@ -74,28 +74,46 @@
   """Class implementing __call__, but explicitly set to not being
   recognized by CallMeMaybe"""
 
   def __call__(self, *args, **kwargs) -> NoReturn:
     """f... da police!"""
     return 'f... da police!'
 
+  def __str__(self, *args, **kwargs) -> str:
+    """I know I'm callable, but I'm supposed to not be recognized as
+    callable!"""
+    return """I know I'm callable, but I'm supposed to not be recognized as
+    callable!"""
+
 
 class TestCallMeMaybe(TestCase):
   """Testing CallMeMaybe
   #  MIT License
   #  Copyright (c) 2023 Asger Jon Vistisen"""
 
   def setUp(self) -> NoReturn:
     """Sets up the tests"""
     self.callMeMaybe = CallMeMaybe()
     self.callable = HereIsMyNumber()
     self.notCallable = ThisIsCrazy()
     self.inCognitoClassInstance = InCognitoClass()
     self.inCognitoFunction = inCognitoFunction
 
+  def testTypeError(self) -> NoReturn:
+    """Testing error raised when calling something other than a type,
+    class or callable."""
+    with self.assertRaises(TypeError):
+      CallMeMaybe()(777)
+
+    with self.assertRaises(TypeError):
+      CallMeMaybe()(.777)
+
+    with self.assertRaises(TypeError):
+      CallMeMaybe()(1j)
+
   def testCallables(self) -> NoReturn:
     """Testing the type name of print"""
     callables = [print, func, sin, self.callable, ]
     for item in callables:
       self.assertTrue(self.callMeMaybe.recognizeInstance(item))
 
   def testUnCallables(self) -> NoReturn:
```

### Comparing `worktoy-0.28.8/tests/test__intfactory.py` & `worktoy-0.30.0/tests/test__intfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/tests/test__maybe.py` & `worktoy-0.30.0/tests/test__maybe.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/tests/test__maybeType.py` & `worktoy-0.30.0/tests/test__maybeType.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/tests/test__maybeTypes.py` & `worktoy-0.30.0/tests/test__maybeTypes.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/tests/test__searchKeys.py` & `worktoy-0.30.0/tests/test__searchKeys.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/tests/test__strfactory.py` & `worktoy-0.30.0/tests/test__strfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.8/tests/test__stringlist.py` & `worktoy-0.30.0/tests/test__stringlist.py`

 * *Files identical despite different names*

