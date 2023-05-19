# Comparing `tmp/xmodel-0.5.0.tar.gz` & `tmp/xmodel-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmodel-0.5.0.tar", max compression
+gzip compressed data, was "xmodel-0.6.0.tar", max compression
```

## Comparing `xmodel-0.5.0.tar` & `xmodel-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1211 2023-05-05 17:50:12.783048 xmodel-0.5.0/LICENSE
--rw-r--r--   0        0        0     1046 2023-05-05 17:50:12.783048 xmodel-0.5.0/README.md
--rw-r--r--   0        0        0     2072 2023-05-05 17:50:12.783048 xmodel-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    20732 2023-05-05 17:50:12.783048 xmodel-0.5.0/xmodel/__init__.py
--rw-r--r--   0        0        0       18 2023-05-05 17:50:12.783048 xmodel-0.5.0/xmodel/_private/__init__.py
--rw-r--r--   0        0        0       33 2023-05-05 17:50:12.783048 xmodel-0.5.0/xmodel/_private/api/__init__.py
--rw-r--r--   0        0        0     7007 2023-05-05 17:50:12.783048 xmodel-0.5.0/xmodel/_private/api/state.py
--rw-r--r--   0        0        0      828 2023-05-05 17:50:12.783048 xmodel-0.5.0/xmodel/_private/api/utils.py
--rw-r--r--   0        0        0      191 2023-05-05 17:50:12.783048 xmodel-0.5.0/xmodel/base/__init__.py
--rw-r--r--   0        0        0    48954 2023-05-05 17:50:12.783048 xmodel-0.5.0/xmodel/base/api.py
--rw-r--r--   0        0        0    35396 2023-05-05 17:50:12.783048 xmodel-0.5.0/xmodel/base/fields.py
--rw-r--r--   0        0        0    32659 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/base/model.py
--rw-r--r--   0        0        0    21759 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/base/structure.py
--rw-r--r--   0        0        0        1 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/common/__init__.py
--rw-r--r--   0        0        0    13348 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/common/children.py
--rw-r--r--   0        0        0     1943 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/common/lazy.py
--rw-r--r--   0        0        0      963 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/common/types.py
--rw-r--r--   0        0        0     1635 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/common/unwrap.py
--rw-r--r--   0        0        0     2555 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/common/utils.py
--rw-r--r--   0        0        0     7716 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/converters.py
--rw-r--r--   0        0        0       89 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/errors.py
--rw-r--r--   0        0        0      801 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/json.py
--rw-r--r--   0        0        0      273 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/remote/__init__.py
--rw-r--r--   0        0        0    30590 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/remote/api.py
--rw-r--r--   0        0        0     7789 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/remote/client.py
--rw-r--r--   0        0        0      301 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/remote/errors.py
--rw-r--r--   0        0        0     2242 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/remote/model.py
--rw-r--r--   0        0        0     3112 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/remote/options.py
--rw-r--r--   0        0        0    12775 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/remote/response_state.py
--rw-r--r--   0        0        0     6709 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/remote/structure.py
--rw-r--r--   0        0        0     7935 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/remote/weak_cache_pool.py
--rw-r--r--   0        0        0      240 2023-05-05 17:50:12.787047 xmodel-0.5.0/xmodel/util.py
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 xmodel-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-05-19 17:34:52.770700 xmodel-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1046 2023-05-19 17:34:52.770700 xmodel-0.6.0/README.md
+-rw-r--r--   0        0        0     2072 2023-05-19 17:34:52.774700 xmodel-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    20732 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/__init__.py
+-rw-r--r--   0        0        0       18 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/_private/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/_private/api/__init__.py
+-rw-r--r--   0        0        0     7007 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/_private/api/state.py
+-rw-r--r--   0        0        0      828 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/_private/api/utils.py
+-rw-r--r--   0        0        0      191 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/base/__init__.py
+-rw-r--r--   0        0        0    48954 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/base/api.py
+-rw-r--r--   0        0        0    35396 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/base/fields.py
+-rw-r--r--   0        0        0    32969 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/base/model.py
+-rw-r--r--   0        0        0    21759 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/base/structure.py
+-rw-r--r--   0        0        0        1 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/common/__init__.py
+-rw-r--r--   0        0        0    13348 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/common/children.py
+-rw-r--r--   0        0        0     1943 2023-05-19 17:34:52.774700 xmodel-0.6.0/xmodel/common/lazy.py
+-rw-r--r--   0        0        0      963 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/common/types.py
+-rw-r--r--   0        0        0     1635 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/common/unwrap.py
+-rw-r--r--   0        0        0     2555 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/common/utils.py
+-rw-r--r--   0        0        0     7716 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/converters.py
+-rw-r--r--   0        0        0       89 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/errors.py
+-rw-r--r--   0        0        0      801 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/json.py
+-rw-r--r--   0        0        0      273 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/remote/__init__.py
+-rw-r--r--   0        0        0    30590 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/remote/api.py
+-rw-r--r--   0        0        0     7789 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/remote/client.py
+-rw-r--r--   0        0        0      301 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/remote/errors.py
+-rw-r--r--   0        0        0     2242 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/remote/model.py
+-rw-r--r--   0        0        0     3112 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/remote/options.py
+-rw-r--r--   0        0        0    12775 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/remote/response_state.py
+-rw-r--r--   0        0        0     6709 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/remote/structure.py
+-rw-r--r--   0        0        0     7935 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/remote/weak_cache_pool.py
+-rw-r--r--   0        0        0      240 2023-05-19 17:34:52.778700 xmodel-0.6.0/xmodel/util.py
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 xmodel-0.6.0/PKG-INFO
```

### Comparing `xmodel-0.5.0/LICENSE` & `xmodel-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/README.md` & `xmodel-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/pyproject.toml` & `xmodel-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xmodel"
-version = "0.5.0"
+version = "0.6.0"
 description = "Models for working with JSON, ie: JsonModel"
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xmodel"}]
 readme = "README.md"
 repository = "https://github.com/xyngular/py-xmodel"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `xmodel-0.5.0/xmodel/__init__.py` & `xmodel-0.6.0/xmodel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,8 +496,8 @@
     'BaseStructure',
     'Field',
     'Converter',
     'XModelError',
     'JsonModel'
 ]
 
-__version__ = '0.5.0'
+__version__ = '0.6.0'
```

### Comparing `xmodel-0.5.0/xmodel/_private/api/state.py` & `xmodel-0.6.0/xmodel/_private/api/state.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/_private/api/utils.py` & `xmodel-0.6.0/xmodel/_private/api/utils.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/base/api.py` & `xmodel-0.6.0/xmodel/base/api.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/base/fields.py` & `xmodel-0.6.0/xmodel/base/fields.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/base/model.py` & `xmodel-0.6.0/xmodel/base/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import sys
 import typing
 
 from xmodel.common.lazy import LazyClassAttr  # noqa - orm private module
 from logging import getLogger
 from typing import get_type_hints, TYPE_CHECKING, TypeVar, Generic, Type, Optional, Any, Mapping, \
     Callable
@@ -353,23 +354,29 @@
 
         cls_api_type = type(type(self).api)
         api = cls_api_type(model=self)
         setattr(self, "api", api)  # Avoids IDE from using this as type-hint for `self.api`.
 
         first_arg = args[0] if args_len > 0 else None
 
-        if isinstance(first_arg, BaseModel):
+        if isinstance(first_arg, str):
+            # We assume `str` is a json-string, parse json and import.
+            json_objs = json.loads(first_arg)
+            api.update_from_json(json_objs)
+        elif isinstance(first_arg, BaseModel):
             # todo: Probably make this recursive, in that we copy sub-base-models as well???
             api.copy_from_model(first_arg)
         elif isinstance(first_arg, Mapping):
             api.update_from_json(first_arg)
         elif first_arg is not None:
             raise XModelError(
                 f"When a first argument to BaseModel.__init__ is provided, it needs to be a "
-                f"mapping/dict with the json values in it OR a BaseModel instance to copy from; "
+                f"mapping/dict with the json values in it "
+                f"OR a BaseModel instance to copy from "
+                f"OR a str with a json dict/obj to parse inside of string; "
                 f"I was given a type ({type(first_arg)}) with value ({first_arg}) instead."
             )
 
         for k, v in initial_values.items():
             if not self.api.structure.get_field(k):
                 raise XModelError(
                     f"While constructing {self}, init method got a value for an "
```

### Comparing `xmodel-0.5.0/xmodel/base/structure.py` & `xmodel-0.6.0/xmodel/base/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/common/children.py` & `xmodel-0.6.0/xmodel/common/children.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/common/lazy.py` & `xmodel-0.6.0/xmodel/common/lazy.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/common/types.py` & `xmodel-0.6.0/xmodel/common/types.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/common/unwrap.py` & `xmodel-0.6.0/xmodel/common/unwrap.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/common/utils.py` & `xmodel-0.6.0/xmodel/common/utils.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/converters.py` & `xmodel-0.6.0/xmodel/converters.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/json.py` & `xmodel-0.6.0/xmodel/json.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/remote/api.py` & `xmodel-0.6.0/xmodel/remote/api.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/remote/client.py` & `xmodel-0.6.0/xmodel/remote/client.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/remote/model.py` & `xmodel-0.6.0/xmodel/remote/model.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/remote/options.py` & `xmodel-0.6.0/xmodel/remote/options.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/remote/response_state.py` & `xmodel-0.6.0/xmodel/remote/response_state.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/remote/structure.py` & `xmodel-0.6.0/xmodel/remote/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/xmodel/remote/weak_cache_pool.py` & `xmodel-0.6.0/xmodel/remote/weak_cache_pool.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.5.0/PKG-INFO` & `xmodel-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmodel
-Version: 0.5.0
+Version: 0.6.0
 Summary: Models for working with JSON, ie: JsonModel
 Home-page: https://github.com/xyngular/py-xmodel
 Author: Josh Orr
 Author-email: josh@orr.blue
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3
```

