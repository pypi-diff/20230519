# Comparing `tmp/pydictable-1.0.2.tar.gz` & `tmp/pydictable-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydictable-1.0.2.tar", last modified: Tue May  2 10:06:55 2023, max compression
+gzip compressed data, was "pydictable-1.1.0.tar", last modified: Fri May 19 09:57:25 2023, max compression
```

## Comparing `pydictable-1.0.2.tar` & `pydictable-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:06:55.421827 pydictable-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-02 10:06:42.000000 pydictable-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-02 10:06:55.421827 pydictable-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-02 10:06:42.000000 pydictable-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:06:55.421827 pydictable-1.0.2/pydictable/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    26708 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:06:55.421827 pydictable-1.0.2/pydictable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-02 10:06:55.000000 pydictable-1.0.2/pydictable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-02 10:06:55.000000 pydictable-1.0.2/pydictable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:06:55.000000 pydictable-1.0.2/pydictable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 10:06:55.000000 pydictable-1.0.2/pydictable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:06:55.421827 pydictable-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-02 10:06:42.000000 pydictable-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:57:25.231090 pydictable-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-19 09:57:15.000000 pydictable-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-19 09:57:25.227090 pydictable-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-19 09:57:15.000000 pydictable-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:57:25.227090 pydictable-1.1.0/pydictable/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28020 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-19 09:57:15.000000 pydictable-1.1.0/pydictable/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:57:25.227090 pydictable-1.1.0/pydictable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-19 09:57:25.000000 pydictable-1.1.0/pydictable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-19 09:57:25.000000 pydictable-1.1.0/pydictable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:57:25.000000 pydictable-1.1.0/pydictable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 09:57:25.000000 pydictable-1.1.0/pydictable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:57:25.231090 pydictable-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-19 09:57:15.000000 pydictable-1.1.0/setup.py
```

### Comparing `pydictable-1.0.2/LICENSE` & `pydictable-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydictable-1.0.2/README.md` & `pydictable-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pydictable-1.0.2/pydictable/core.py` & `pydictable-1.1.0/pydictable/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 from enum import Enum
 from typing import Dict, get_type_hints, Union, Type, Any
 
 from pydictable.field import StrField, IntField, FloatField, BoolField, ListField, UnionField, NoneField, \
     ObjectField, DataValidationError, EnumField, DatetimeField, DictField, AnyField
 from pydictable.type import _BaseDictAble, Field
 
+
+class InvalidSchema(Exception):
+    pass
+
+
 TYPE_TO_FIELD = {
     str: StrField,
     int: IntField,
     float: FloatField,
     bool: BoolField,
     dict: DictField,
     type(None): NoneField,
@@ -29,14 +34,15 @@
             if k in fields:
                 self.__setattr__(k, v)
         if kwargs.get('dict'):
             self.__validate_dict(kwargs['dict'])
             self.__apply_dict(kwargs['dict'])
         if len(args) > 0:
             raise ReferenceError('Use kwargs to init DictAble')
+        self.__set_defaults()
         self.__validate()
 
     @classmethod
     def __get_field_type_by_type_hint(cls, type_hint) -> Type[Field]:
         if type_hint in TYPE_TO_FIELD:
             return TYPE_TO_FIELD[type_hint]
 
@@ -109,15 +115,15 @@
 
     def __clear_default_field_values(self):
         for attr, field in self.__class__.__get_fields().items():
             self.__setattr__(attr, None)
 
     def __apply_dict(self, d: dict):
         for attr, field in self.__class__.__get_fields().items():
-            value = d.get(self.__get_field_key(attr), field.default)
+            value = d.get(self.__get_field_key(attr))
             if not field.required and value is None:
                 continue
             self.__setattr__(attr, field.from_dict(value))
 
     def __validate_dict(self, raw_values: dict):
         for attr, field in self.__get_fields().items():
             value = raw_values.get(self.__get_field_key(attr), field.default)
@@ -141,14 +147,26 @@
                 field.validate(attr, value)
             except DataValidationError as e:
                 raise DataValidationError(f'{attr}.{e.path}', e.err)
             except AssertionError:
                 raise DataValidationError(attr,
                                           'Post check failed. Invalid value "{}" for field "{}"'.format(value, attr))
 
+    def __set_defaults(self):
+        for attr, field in self.__get_fields().items():
+            if field.required and field.default is not None:
+                raise InvalidSchema(f'Both required and default passed for field {attr}')
+            value = self.__getattribute__(attr)
+            if value is None:
+                if field.default:
+                    self.__setattr__(attr, field.default)
+                elif field.default_factory:
+                    func, args, kwargs = field.default_factory
+                    self.__setattr__(attr, func(*args, **kwargs))
+
     def to_dict(self) -> dict:
         d = {}
         for attr, field in self.__class__.__get_fields().items():
             raw_value = self.__getattribute__(attr)
             if not field.required and raw_value is None:
                 d[self.__get_field_key(attr)] = None
                 continue
```

### Comparing `pydictable-1.0.2/pydictable/field.py` & `pydictable-1.1.0/pydictable/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC
 from datetime import datetime
 from enum import EnumMeta, Enum
-from typing import Type, List, Any
+from typing import Type, List, Any, Callable
 
-from pydictable.type import Field, _BaseDictAble
+from pydictable.type import Field, _BaseDictAble, DefaultFactoryType
 
 
 class DataValidationError(Exception):
     def __init__(self, path: str, err):
         super(DataValidationError, self).__init__(path, err)
         self.path = path
         self.err = err
@@ -293,17 +293,18 @@
 class DictField(Field):
     def __init__(
             self,
             key_type: Field = AnyField(),
             value_type: Field = AnyField(),
             required: bool = False,
             key: str = None,
-            default: Any = None
+            default: Any = None,
+            default_factory: DefaultFactoryType = None
     ):
-        super(DictField, self).__init__(required=required, key=key, default=default)
+        super(DictField, self).__init__(required=required, key=key, default=default, default_factory=default_factory)
         self.key_type = key_type
         self.value_type = value_type
 
     def from_dict(self, value):
         return {self.key_type.from_dict(k): self.value_type.from_dict(v) for k, v in value.items()}
 
     def to_dict(self, value):
```

### Comparing `pydictable-1.0.2/pydictable/test_core.py` & `pydictable-1.1.0/pydictable/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from datetime import datetime
 from enum import Enum
+from time import sleep
 from typing import List, Dict, Optional, Tuple, Union, Any
 from unittest import TestCase
 
 from pydictable.core import DictAble
 from pydictable.field import IntField, StrField, ListField, ObjectField, DatetimeField, CustomField, MultiTypeField, \
     EnumField, DictField, DictValueField, UnionField, DataValidationError
 
@@ -646,15 +647,15 @@
         input_dict = {'name': 'Pramod'}
         user = User(dict=input_dict)
         self.assertEqual(user.name, 'Pramod')
         self.assertEqual(user.time_stamp, 1673442076263)
 
         class Email(DictAble):
             to: str = StrField(required=True)
-            subject: str = StrField(required=True, default="General inquiry")
+            subject: str = StrField(default="General inquiry")
             body: str = StrField(required=True)
 
         input_dict = {'to': 'testing@gmail.com', 'body': "Hello"}
         email = Email(dict=input_dict)
         self.assertEqual(email.to, 'testing@gmail.com')
         self.assertEqual(email.subject, 'General inquiry')
         self.assertEqual(email.body, 'Hello')
@@ -756,7 +757,46 @@
 
         class Profile(DictAble):
             address: Address = ObjectField(Address)
 
         profile = Profile(dict={'address': {'location': 'Bengaluru'}})
         self.assertEqual(profile.address.references, None)
         self.assertEqual(profile.to_dict(), {'address': {'references': None, 'location': 'Bengaluru'}})
+
+    def test_dynamic_default(self):
+        now = datetime.now()
+
+        class DOB(DictAble):
+            date: datetime = DatetimeField(default=now)
+
+        self.assertEqual(DOB().date, now)
+        _now = datetime(2023, 5, 19)
+        self.assertEqual(DOB(date=_now).date, _now)
+
+        self.assertEqual(DOB(dict={}).date, now)
+        self.assertEqual(DOB(dict={'date': None}).date, now)
+
+        millis = 1684462306000
+        self.assertEqual(DOB(dict={'date': millis}).date, datetime.fromtimestamp(millis/1000))
+
+        class DOB(DictAble):
+            date: datetime = DatetimeField(default_factory=(datetime.now, (), {}))
+            date_2: datetime = DatetimeField(default=datetime.now())
+
+        self.assertLessEqual((DOB().date - datetime.now()).total_seconds(), 1e2)
+
+        dob1 = DOB()
+        sleep(1)
+        dob2 = DOB()
+
+        self.assertEqual(dob1.date_2, dob2.date_2)
+        self.assertLessEqual((dob2.date - dob1.date).total_seconds(), 1 + 1e2)
+
+        def math(a: int, b: int):
+            return a * b
+
+        class Number(DictAble):
+            num: int = IntField(default_factory=(math, (8,), {'b': 5}))
+
+        self.assertEqual(Number().num, 40)
+        self.assertEqual(Number(dict={'num': None}).num, 40)
+        self.assertEqual(Number(dict={'num': 5}).num, 5)
```

### Comparing `pydictable-1.0.2/pydictable/test_field.py` & `pydictable-1.1.0/pydictable/test_field.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.0.2/setup.py` & `pydictable-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pydictable',
-    version='1.0.2',
+    version='1.1.0',
     author='Pramod Kumar',
     author_email='pramodkumar.damam73@gmail.com',
     description='Make your classes from/to dict',
     url='https://github.com/pskd73/pydictable.git',
     packages=['pydictable'],
     include_package_data=True,
     long_description='A tool to create data modals from dict and convert it to dict. '
```

