# Comparing `tmp/mapperr-0.0.5.tar.gz` & `tmp/mapperr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapperr-0.0.5.tar", last modified: Tue Feb  8 20:33:10 2022, max compression
+gzip compressed data, was "mapperr-0.1.0.tar", last modified: Fri May 19 20:26:47 2023, max compression
```

## Comparing `mapperr-0.0.5.tar` & `mapperr-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-02-08 20:33:10.846269 mapperr-0.0.5/
--rw-rw-rw-   0        0        0     1097 2022-02-07 19:43:31.000000 mapperr-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2702 2022-02-08 20:33:10.845270 mapperr-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2280 2022-02-07 19:43:31.000000 mapperr-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2022-02-08 20:33:10.776941 mapperr-0.0.5/mapperr/
--rw-rw-rw-   0        0        0      773 2022-02-07 19:43:31.000000 mapperr-0.0.5/mapperr/__init__.py
--rw-rw-rw-   0        0        0     2431 2022-02-07 19:43:31.000000 mapperr-0.0.5/mapperr/mapr.py
-drwxrwxrwx   0        0        0        0 2022-02-08 20:33:10.837263 mapperr-0.0.5/mapperr.egg-info/
--rw-rw-rw-   0        0        0     2702 2022-02-08 20:33:10.000000 mapperr-0.0.5/mapperr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2022-02-08 20:33:10.000000 mapperr-0.0.5/mapperr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-08 20:33:10.000000 mapperr-0.0.5/mapperr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-02-08 20:33:10.000000 mapperr-0.0.5/mapperr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-02-08 20:33:10.848268 mapperr-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      721 2022-02-07 19:53:51.000000 mapperr-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-08 20:33:10.842269 mapperr-0.0.5/test/
--rw-rw-rw-   0        0        0     1855 2022-02-07 19:43:31.000000 mapperr-0.0.5/test/test_mapperr.py
--rw-rw-rw-   0        0        0      727 2022-02-07 19:43:31.000000 mapperr-0.0.5/test/test_mapperr2.py
--rw-rw-rw-   0        0        0      498 2022-02-07 19:43:31.000000 mapperr-0.0.5/test/test_mapperr3.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-19 20:26:47.987399 mapperr-0.1.0/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.1.0/LICENSE
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2684 2023-05-19 20:26:47.987256 mapperr-0.1.0/PKG-INFO
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     2314 2023-05-19 20:22:50.000000 mapperr-0.1.0/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-19 20:26:47.985823 mapperr-0.1.0/mapperr/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      959 2023-05-15 14:38:18.000000 mapperr-0.1.0/mapperr/__init__.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     2346 2023-05-15 14:38:18.000000 mapperr-0.1.0/mapperr/mapr.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-19 20:26:47.986522 mapperr-0.1.0/mapperr.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2684 2023-05-19 20:26:47.000000 mapperr-0.1.0/mapperr.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      268 2023-05-19 20:26:47.000000 mapperr-0.1.0/mapperr.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-05-19 20:26:47.000000 mapperr-0.1.0/mapperr.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-05-19 20:26:47.000000 mapperr-0.1.0/mapperr.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-05-19 20:26:47.987449 mapperr-0.1.0/setup.cfg
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-05-19 20:23:41.000000 mapperr-0.1.0/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-19 20:26:47.987028 mapperr-0.1.0/test/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     1741 2023-05-15 14:38:02.000000 mapperr-0.1.0/test/test_nested_objects.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.1.0/test/test_op_required.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-05-15 14:38:02.000000 mapperr-0.1.0/test/test_unmatched_types.py
```

### Comparing `mapperr-0.0.5/PKG-INFO` & `mapperr-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,102 @@
-Metadata-Version: 2.1
-Name: mapperr
-Version: 0.0.5
-Summary: mapperr for mapping across dict and object, recursively
-Home-page: https://github.com/mujdecisy/mapperr
-Author: mujdecisy
-Author-email: mujdecisy@gmail.com
-License: UNKNOWN
-Keywords: python,mapper,recursive mapping
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **mapperr - mapping across dictionary and class object, recursively**
-
-If you are using python for implementing protocols, cache management, nosql or sql database manupilation with  the object oriented concepts in your code, mapperr can handle your object in your way, easily.
-
-## Installation
-`via pip`
-```shell
-pip3 install mapperr
-```
-`via direct setup`
-```shell
-pip3 install setuptools
-python3 setup.py sdist bdist_wheel
-pip3 install dist/mapperr-0.0.1-py3-none-any.whl
-```
-
-## Usage
-Your classes' attributes are needed to be annotated with their types like `int`, `str`, `Book`, `List[Book]`. Parameterized constructors are not suitable, you can use it with plain objects which has most trash work.
-
-**`to_obj( dict_data: dict, destination_class: Type ) -> object`**
-
-**`to_dict( obj: object ) -> dict`**
-
-
-```python
-from typing import List
-from pprint import pprint
-from mapperr import to_dict, to_obj
-
-class Book:
-    _id: int
-    title: str
-
-class BookShelf:
-    code: str
-    books: List[Book]
-
-class Library:
-    name: str
-    book_shelfs: List[BookShelf]
-
-
-def retrieve_library_from_the_source() -> dict:
-    return {
-        "name" : "Hogwarts Library",
-        "book_shelfs" : [
-            {
-                "code" : "A1",
-                "books" : [
-                    {
-                    "_id" : 0,
-                    "title" : "Defence Against the Dark Arts"
-                    },
-                    {
-                    "_id" : 1,
-                    "title" : "Potions"
-                    },
-                ]
-            },
-            {
-                "code" : "A2",
-                "books" : [
-                    {
-                    "_id" : 3,
-                    "title" : "Charms"
-                    },
-                    {
-                    "_id" : 4,
-                    "title" : "Herbology"
-                    },
-                ]
-            }
-        ]
-    }
-
-def send_library_to_the_source(data: dict):
-    pprint(data)
-
-
-lib: Library = to_obj(retrieve_library_from_the_source(), Library)
-
-new_book = Book()
-new_book._id = 5
-new_book.title = "Alchemy"
-
-lib.book_shelfs[0].books.append(new_book)
-
-send_library_to_the_source( to_dict(lib) )
-```
-
+Metadata-Version: 2.1
+Name: mapperr
+Version: 0.1.0
+Summary: mapperr for mapping across dict and object, recursively
+Home-page: https://github.com/mujdecisy/mapperr
+Author: mujdecisy
+Author-email: mujdecisy@gmail.com
+Keywords: python,mapper,recursive mapping
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **mapperr - mapping across dictionary and class object, recursively**
+
+If you are using python for implementing protocols, cache management, nosql or sql database manupilation with  the object oriented concepts in your code, mapperr can handle your object in your way, easily.
+
+## Installation
+`via pip`
+```shell
+pip3 install mapperr
+```
+`via direct setup`
+```shell
+pip3 install setuptools
+python3 setup.py sdist bdist_wheel
+pip3 install dist/mapperr-0.0.1-py3-none-any.whl
+```
+
+## Usage
+Your classes' attributes are needed to be annotated with their types like `int`, `str`, `Book`, `List[Book]`. Parameterized constructors are not suitable, you can use it with plain objects which has most trash work. You can also fill your required options with param `op_required` as string list.
+
+**`to_obj( dict_data: dict, destination_class: Type ) -> object`**
+
+**`to_dict( obj: object ) -> dict`**
+
+
+```python
+from typing import List
+from pprint import pprint
+from mapperr import to_dict, to_obj
+
+class Book:
+    _id: int
+    title: str
+    op_required: list = ['_id', 'title']
+
+class BookShelf:
+    code: str
+    books: List[Book]
+
+class Library:
+    name: str
+    book_shelfs: List[BookShelf]
+
+
+def retrieve_library_from_the_source() -> dict:
+    return {
+        "name" : "Hogwarts Library",
+        "book_shelfs" : [
+            {
+                "code" : "A1",
+                "books" : [
+                    {
+                    "_id" : 0,
+                    "title" : "Defence Against the Dark Arts"
+                    },
+                    {
+                    "_id" : 1,
+                    "title" : "Potions"
+                    },
+                ]
+            },
+            {
+                "code" : "A2",
+                "books" : [
+                    {
+                    "_id" : 3,
+                    "title" : "Charms"
+                    },
+                    {
+                    "_id" : 4,
+                    "title" : "Herbology"
+                    },
+                ]
+            }
+        ]
+    }
+
+def send_library_to_the_source(data: dict):
+    pprint(data)
+
+
+lib: Library = to_obj(retrieve_library_from_the_source(), Library)
+
+new_book = Book()
+new_book._id = 5
+new_book.title = "Alchemy"
+
+lib.book_shelfs[0].books.append(new_book)
+
+send_library_to_the_source( to_dict(lib) )
+```
```

### Comparing `mapperr-0.0.5/README.md` & `mapperr-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,90 @@
-# **mapperr - mapping across dictionary and class object, recursively**
-
-If you are using python for implementing protocols, cache management, nosql or sql database manupilation with  the object oriented concepts in your code, mapperr can handle your object in your way, easily.
-
-## Installation
-`via pip`
-```shell
-pip3 install mapperr
-```
-`via direct setup`
-```shell
-pip3 install setuptools
-python3 setup.py sdist bdist_wheel
-pip3 install dist/mapperr-0.0.1-py3-none-any.whl
-```
-
-## Usage
-Your classes' attributes are needed to be annotated with their types like `int`, `str`, `Book`, `List[Book]`. Parameterized constructors are not suitable, you can use it with plain objects which has most trash work.
-
-**`to_obj( dict_data: dict, destination_class: Type ) -> object`**
-
-**`to_dict( obj: object ) -> dict`**
-
-
-```python
-from typing import List
-from pprint import pprint
-from mapperr import to_dict, to_obj
-
-class Book:
-    _id: int
-    title: str
-
-class BookShelf:
-    code: str
-    books: List[Book]
-
-class Library:
-    name: str
-    book_shelfs: List[BookShelf]
-
-
-def retrieve_library_from_the_source() -> dict:
-    return {
-        "name" : "Hogwarts Library",
-        "book_shelfs" : [
-            {
-                "code" : "A1",
-                "books" : [
-                    {
-                    "_id" : 0,
-                    "title" : "Defence Against the Dark Arts"
-                    },
-                    {
-                    "_id" : 1,
-                    "title" : "Potions"
-                    },
-                ]
-            },
-            {
-                "code" : "A2",
-                "books" : [
-                    {
-                    "_id" : 3,
-                    "title" : "Charms"
-                    },
-                    {
-                    "_id" : 4,
-                    "title" : "Herbology"
-                    },
-                ]
-            }
-        ]
-    }
-
-def send_library_to_the_source(data: dict):
-    pprint(data)
-
-
-lib: Library = to_obj(retrieve_library_from_the_source(), Library)
-
-new_book = Book()
-new_book._id = 5
-new_book.title = "Alchemy"
-
-lib.book_shelfs[0].books.append(new_book)
-
-send_library_to_the_source( to_dict(lib) )
+# **mapperr - mapping across dictionary and class object, recursively**
+
+If you are using python for implementing protocols, cache management, nosql or sql database manupilation with  the object oriented concepts in your code, mapperr can handle your object in your way, easily.
+
+## Installation
+`via pip`
+```shell
+pip3 install mapperr
+```
+`via direct setup`
+```shell
+pip3 install setuptools
+python3 setup.py sdist bdist_wheel
+pip3 install dist/mapperr-0.0.1-py3-none-any.whl
+```
+
+## Usage
+Your classes' attributes are needed to be annotated with their types like `int`, `str`, `Book`, `List[Book]`. Parameterized constructors are not suitable, you can use it with plain objects which has most trash work. You can also fill your required options with param `op_required` as string list.
+
+**`to_obj( dict_data: dict, destination_class: Type ) -> object`**
+
+**`to_dict( obj: object ) -> dict`**
+
+
+```python
+from typing import List
+from pprint import pprint
+from mapperr import to_dict, to_obj
+
+class Book:
+    _id: int
+    title: str
+    op_required: list = ['_id', 'title']
+
+class BookShelf:
+    code: str
+    books: List[Book]
+
+class Library:
+    name: str
+    book_shelfs: List[BookShelf]
+
+
+def retrieve_library_from_the_source() -> dict:
+    return {
+        "name" : "Hogwarts Library",
+        "book_shelfs" : [
+            {
+                "code" : "A1",
+                "books" : [
+                    {
+                    "_id" : 0,
+                    "title" : "Defence Against the Dark Arts"
+                    },
+                    {
+                    "_id" : 1,
+                    "title" : "Potions"
+                    },
+                ]
+            },
+            {
+                "code" : "A2",
+                "books" : [
+                    {
+                    "_id" : 3,
+                    "title" : "Charms"
+                    },
+                    {
+                    "_id" : 4,
+                    "title" : "Herbology"
+                    },
+                ]
+            }
+        ]
+    }
+
+def send_library_to_the_source(data: dict):
+    pprint(data)
+
+
+lib: Library = to_obj(retrieve_library_from_the_source(), Library)
+
+new_book = Book()
+new_book._id = 5
+new_book.title = "Alchemy"
+
+lib.book_shelfs[0].books.append(new_book)
+
+send_library_to_the_source( to_dict(lib) )
 ```
```

### Comparing `mapperr-0.0.5/mapperr/__init__.py` & `mapperr-0.1.0/mapperr/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from mapperr.mapr import _maprit
-
-def to_obj( src: dict, root_class: type) -> object:
-    des: object = root_class()
-    required_variables = getattr(des, 'required', [])
-    
-    res = _maprit(src, des, root_class)
-    
-    res.__setattr__('required', required_variables)
-    __check_required(res)
-    return res
-
-def to_dict( src: object ) -> dict:
-    des = {}
-    return _maprit(src, des, src.__class__)
-
-def obj_to_obj( src: object, dest_class: type ) -> object:
-    d = to_dict(src)
-    return to_obj(d, dest_class)
-
-def __check_required(o: object) -> bool:
-    required_variables: list = getattr(o, 'required', [])
-    for e in required_variables:
-        if o.__getattribute__(e) == None:
+from mapperr.mapr import _maprit
+
+def to_obj( src: dict, root_class: type) -> object:
+    des: object = root_class()
+    required_variables = getattr(des, 'op_required', [])
+
+    res = _maprit(src, des, root_class)
+
+    res.__setattr__('op_required', required_variables)
+    __check_required(res, root_class)
+    return res
+
+def to_dict( src: object ) -> dict:
+    des = {}
+    return _maprit(src, des, src.__class__)
+
+def obj_to_obj( src: object, dest_class: type ) -> object:
+    d = to_dict(src)
+    return to_obj(d, dest_class)
+
+def __check_required(o: object, root_class: type) -> bool:
+    required_variables: list = getattr(o, 'op_required', [])
+    annot_keys = root_class.__annotations__.keys()
+    for e in required_variables:
+        if e not in annot_keys:
+            raise TypeError(f'{e} can not be required due to not being attribute of the class')
+        if o.__getattribute__(e) == None:
             raise AttributeError(f'{e} is required')
```

### Comparing `mapperr-0.0.5/mapperr/mapr.py` & `mapperr-0.1.0/mapperr/mapr.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import importlib
-import warnings
-
-def _maprit(src, des, root_class):
-    rwkey = "d2o" if isinstance(src, dict) else "o2d"
-    rdr = __rw[rwkey]["r"]
-    wtr = __rw[rwkey]["w"]
-    rcv = __rw[rwkey]["rcv"]
-
-    annots = root_class.__dict__["__annotations__"]
-
-    for k,t in annots.items():
-        v = rdr(src, k)
-        tstr = str(t)
-
-        if v != None and not __is_matching_types(t, type(v)):
-            warnings.warn(f"{k} not in type [{t}], it is [{type(v)}], it is replaced as None")
-            wtr(des, k, None)
-            continue
-
-        if (__is_defined_list(tstr) and __get_list_inner_type(tstr) in __prm.values()) or (v == None or t in __prm.keys()):
-            wtr(des, k, v)
-            continue
-
-        if __is_defined_list(tstr):
-            els = []
-            itcls = __simport(__get_list_inner_type(tstr))
-            for e in v:
-                els.append( rcv(e, itcls) )
-            wtr(des, k, els)
-            continue
-
-        itcls = __simport(__clean_type_str(tstr))
-        wtr(des, k, rcv(v, itcls))
-    return des
-
-def __is_defined_list(type_str: str) -> bool:
-    return type_str.startswith("typing.List")
-
-def __get_list_inner_type(type_str: str) -> str:
-    return type_str.replace("typing.List[","").replace("]","")
-
-def __clean_type_str(type_str: str) -> str:
-    return type_str.replace("<class '", "").replace("'>", "")
-
-def __is_matching_types(t1, t2) -> bool:
-    t1 = __type_check(t1)
-    t2 = __type_check(t2)
-    if t1 == t2:
-        return True
-    return False
-
-def __type_check(t: type) -> type:
-    if __is_defined_list(str(t)):
-        return list
-    if __clean_type_str(str(t)) not in __prm.values():
-        return dict
-    return t
-
-__rw = {
-    "d2o" : {
-        "r" : lambda e, k: e.get(k),
-        "w" : lambda e, k, v: e.__setattr__(k, v),
-        "rcv" : lambda s, c: _maprit(s, c(), c)
-    },
-    "o2d" : {
-        "r" : lambda e, k: e.__getattribute__(k),
-        "w" : lambda e, k, v: e.update({k:v}),
-        "rcv" : lambda s, c: _maprit(s, {}, s.__class__)
-    }
-}
-
-__prm = {
-    str: "str",
-    int: "int",
-    float: "float",
-    dict: "dict",
-    list: "list"
-}
-
-def __simport(module_and_class: str):
-    cstr = module_and_class.split(".")[-1]
-    mstr = module_and_class.replace(f".{cstr}", "")
-    m = importlib.import_module(mstr)
-    c = getattr(m, cstr)
+import importlib
+import warnings
+
+def _maprit(src, des, root_class):
+    rwkey = "d2o" if isinstance(src, dict) else "o2d"
+    rdr = __rw[rwkey]["r"]
+    wtr = __rw[rwkey]["w"]
+    rcv = __rw[rwkey]["rcv"]
+
+    annots = root_class.__dict__["__annotations__"]
+
+    for k,t in annots.items():
+        v = rdr(src, k)
+        tstr = str(t)
+
+        if v != None and not __is_matching_types(t, type(v)):
+            warnings.warn(f"{k} not in type [{t}], it is [{type(v)}], it is replaced as None")
+            wtr(des, k, None)
+            continue
+
+        if (__is_defined_list(tstr) and __get_list_inner_type(tstr) in __prm.values()) or (v == None or t in __prm.keys()):
+            wtr(des, k, v)
+            continue
+
+        if __is_defined_list(tstr):
+            els = []
+            itcls = __simport(__get_list_inner_type(tstr))
+            for e in v:
+                els.append( rcv(e, itcls) )
+            wtr(des, k, els)
+            continue
+
+        itcls = __simport(__clean_type_str(tstr))
+        wtr(des, k, rcv(v, itcls))
+    return des
+
+def __is_defined_list(type_str: str) -> bool:
+    return type_str.startswith("typing.List")
+
+def __get_list_inner_type(type_str: str) -> str:
+    return type_str.replace("typing.List[","").replace("]","")
+
+def __clean_type_str(type_str: str) -> str:
+    return type_str.replace("<class '", "").replace("'>", "")
+
+def __is_matching_types(t1, t2) -> bool:
+    t1 = __type_check(t1)
+    t2 = __type_check(t2)
+    if t1 == t2:
+        return True
+    return False
+
+def __type_check(t: type) -> type:
+    if __is_defined_list(str(t)):
+        return list
+    if __clean_type_str(str(t)) not in __prm.values():
+        return dict
+    return t
+
+__rw = {
+    "d2o" : {
+        "r" : lambda e, k: e.get(k),
+        "w" : lambda e, k, v: e.__setattr__(k, v),
+        "rcv" : lambda s, c: _maprit(s, c(), c)
+    },
+    "o2d" : {
+        "r" : lambda e, k: e.__getattribute__(k),
+        "w" : lambda e, k, v: e.update({k:v}),
+        "rcv" : lambda s, c: _maprit(s, {}, s.__class__)
+    }
+}
+
+__prm = {
+    str: "str",
+    int: "int",
+    float: "float",
+    dict: "dict",
+    list: "list"
+}
+
+def __simport(module_and_class: str):
+    cstr = module_and_class.split(".")[-1]
+    mstr = module_and_class.replace(f".{cstr}", "")
+    m = importlib.import_module(mstr)
+    c = getattr(m, cstr)
     return c
```

### Comparing `mapperr-0.0.5/mapperr.egg-info/PKG-INFO` & `mapperr-0.1.0/mapperr.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,102 @@
-Metadata-Version: 2.1
-Name: mapperr
-Version: 0.0.5
-Summary: mapperr for mapping across dict and object, recursively
-Home-page: https://github.com/mujdecisy/mapperr
-Author: mujdecisy
-Author-email: mujdecisy@gmail.com
-License: UNKNOWN
-Keywords: python,mapper,recursive mapping
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **mapperr - mapping across dictionary and class object, recursively**
-
-If you are using python for implementing protocols, cache management, nosql or sql database manupilation with  the object oriented concepts in your code, mapperr can handle your object in your way, easily.
-
-## Installation
-`via pip`
-```shell
-pip3 install mapperr
-```
-`via direct setup`
-```shell
-pip3 install setuptools
-python3 setup.py sdist bdist_wheel
-pip3 install dist/mapperr-0.0.1-py3-none-any.whl
-```
-
-## Usage
-Your classes' attributes are needed to be annotated with their types like `int`, `str`, `Book`, `List[Book]`. Parameterized constructors are not suitable, you can use it with plain objects which has most trash work.
-
-**`to_obj( dict_data: dict, destination_class: Type ) -> object`**
-
-**`to_dict( obj: object ) -> dict`**
-
-
-```python
-from typing import List
-from pprint import pprint
-from mapperr import to_dict, to_obj
-
-class Book:
-    _id: int
-    title: str
-
-class BookShelf:
-    code: str
-    books: List[Book]
-
-class Library:
-    name: str
-    book_shelfs: List[BookShelf]
-
-
-def retrieve_library_from_the_source() -> dict:
-    return {
-        "name" : "Hogwarts Library",
-        "book_shelfs" : [
-            {
-                "code" : "A1",
-                "books" : [
-                    {
-                    "_id" : 0,
-                    "title" : "Defence Against the Dark Arts"
-                    },
-                    {
-                    "_id" : 1,
-                    "title" : "Potions"
-                    },
-                ]
-            },
-            {
-                "code" : "A2",
-                "books" : [
-                    {
-                    "_id" : 3,
-                    "title" : "Charms"
-                    },
-                    {
-                    "_id" : 4,
-                    "title" : "Herbology"
-                    },
-                ]
-            }
-        ]
-    }
-
-def send_library_to_the_source(data: dict):
-    pprint(data)
-
-
-lib: Library = to_obj(retrieve_library_from_the_source(), Library)
-
-new_book = Book()
-new_book._id = 5
-new_book.title = "Alchemy"
-
-lib.book_shelfs[0].books.append(new_book)
-
-send_library_to_the_source( to_dict(lib) )
-```
-
+Metadata-Version: 2.1
+Name: mapperr
+Version: 0.1.0
+Summary: mapperr for mapping across dict and object, recursively
+Home-page: https://github.com/mujdecisy/mapperr
+Author: mujdecisy
+Author-email: mujdecisy@gmail.com
+Keywords: python,mapper,recursive mapping
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **mapperr - mapping across dictionary and class object, recursively**
+
+If you are using python for implementing protocols, cache management, nosql or sql database manupilation with  the object oriented concepts in your code, mapperr can handle your object in your way, easily.
+
+## Installation
+`via pip`
+```shell
+pip3 install mapperr
+```
+`via direct setup`
+```shell
+pip3 install setuptools
+python3 setup.py sdist bdist_wheel
+pip3 install dist/mapperr-0.0.1-py3-none-any.whl
+```
+
+## Usage
+Your classes' attributes are needed to be annotated with their types like `int`, `str`, `Book`, `List[Book]`. Parameterized constructors are not suitable, you can use it with plain objects which has most trash work. You can also fill your required options with param `op_required` as string list.
+
+**`to_obj( dict_data: dict, destination_class: Type ) -> object`**
+
+**`to_dict( obj: object ) -> dict`**
+
+
+```python
+from typing import List
+from pprint import pprint
+from mapperr import to_dict, to_obj
+
+class Book:
+    _id: int
+    title: str
+    op_required: list = ['_id', 'title']
+
+class BookShelf:
+    code: str
+    books: List[Book]
+
+class Library:
+    name: str
+    book_shelfs: List[BookShelf]
+
+
+def retrieve_library_from_the_source() -> dict:
+    return {
+        "name" : "Hogwarts Library",
+        "book_shelfs" : [
+            {
+                "code" : "A1",
+                "books" : [
+                    {
+                    "_id" : 0,
+                    "title" : "Defence Against the Dark Arts"
+                    },
+                    {
+                    "_id" : 1,
+                    "title" : "Potions"
+                    },
+                ]
+            },
+            {
+                "code" : "A2",
+                "books" : [
+                    {
+                    "_id" : 3,
+                    "title" : "Charms"
+                    },
+                    {
+                    "_id" : 4,
+                    "title" : "Herbology"
+                    },
+                ]
+            }
+        ]
+    }
+
+def send_library_to_the_source(data: dict):
+    pprint(data)
+
+
+lib: Library = to_obj(retrieve_library_from_the_source(), Library)
+
+new_book = Book()
+new_book._id = 5
+new_book.title = "Alchemy"
+
+lib.book_shelfs[0].books.append(new_book)
+
+send_library_to_the_source( to_dict(lib) )
+```
```

### Comparing `mapperr-0.0.5/test/test_mapperr.py` & `mapperr-0.1.0/test/test_nested_objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,61 @@
-from unittest import TestCase
-from typing import List
-from mapperr import to_dict, to_obj
-
-class A:
-    a1: str
-    a2: int
-
-class B:
-    b1: str
-    b2: int
-    b3: A
-
-class C:
-    c1: str
-    c2: int
-    c3: List[B]
-    c4: List[int]
-    c5: dict
-    c6: list
-    c7: float
-
-    def test(self):
-        print("hi")
-
-
-class TestMapperr(TestCase):
-    def setUp(self) -> None:
-        self.a = A()
-        self.a.a1, self.a.a2 = "text", 1
-        self.ad = {"a1": "text", "a2": 1}
-        
-        self.a2 = A()
-        self.a2.a1, self.a2.a2 = "text2", 1
-
-        self.b = B()
-        self.b.b1, self.b.b2, self.b.b3 = "text", 1, self.a
-        self.bd = {'b1': 'text', 'b2': 1, 'b3': {'a1': 'text', 'a2': 1}}
-        
-        self.b2 = B()
-        self.b2.b1, self.b2.b2, self.b2.b3 = "text2", 1, self.a2
-
-        self.c = C()
-        self.c.c1, self.c.c2, self.c.c3, self.c.c4, self.c.c5, self.c.c6 = "text", 1, [self.b, self.b2], [1,2], {"msg": "hello"}, ["x", "y", "z"]
-        self.c.c7 = 3.14
-        self.cd = {'c1': 'text', 'c2': 1, 'c3': [{'b1': 'text', 'b2': 1, 'b3': {'a1': 'text', 'a2': 1}}, {'b1': 'text2', 'b2': 1, 'b3': {'a1': 'text2', 'a2': 1}}], 'c4': [1, 2], 'c5': {'msg': 'hello'}, 'c6': ['x', 'y', 'z'], 'c7' : 3.14}
-
-    def test_todict_level1(self):
-        self.assertEqual(to_dict(self.a), self.ad)
-
-    def test_todict_level2(self):
-        self.assertEqual(to_dict(self.b), self.bd)
-
-    def test_todict_level3(self):
-        self.assertEqual(to_dict(self.c), self.cd)
-
-    def test_toobj_level1(self):
-        self.assertEqual(to_dict( to_obj(self.ad, A) ), self.ad)
-
-    def test_toobj_level2(self):
-        self.assertEqual(to_dict( to_obj(self.bd, B) ), self.bd)
-
-    def test_toobj_level3(self):
+from unittest import TestCase
+from typing import List
+from mapperr import to_dict, to_obj
+
+class A:
+    a1: str
+    a2: int
+
+class B:
+    b1: str
+    b2: int
+    b3: A
+
+class C:
+    c1: str
+    c2: int
+    c3: List[B]
+    c4: List[int]
+    c5: dict
+    c6: list
+    c7: float
+
+
+class TestNestedObjects(TestCase):
+    def setUp(self) -> None:
+        self.a = A()
+        self.a.a1, self.a.a2 = "text", 1
+        self.ad = {"a1": "text", "a2": 1}
+
+        self.a2 = A()
+        self.a2.a1, self.a2.a2 = "text2", 1
+
+        self.b = B()
+        self.b.b1, self.b.b2, self.b.b3 = "text", 1, self.a
+        self.bd = {'b1': 'text', 'b2': 1, 'b3': {'a1': 'text', 'a2': 1}}
+
+        self.b2 = B()
+        self.b2.b1, self.b2.b2, self.b2.b3 = "text2", 1, self.a2
+
+        self.c = C()
+        self.c.c1, self.c.c2, self.c.c3, self.c.c4, self.c.c5, self.c.c6 = "text", 1, [self.b, self.b2], [1,2], {"msg": "hello"}, ["x", "y", "z"]
+        self.c.c7 = 3.14
+        self.cd = {'c1': 'text', 'c2': 1, 'c3': [{'b1': 'text', 'b2': 1, 'b3': {'a1': 'text', 'a2': 1}}, {'b1': 'text2', 'b2': 1, 'b3': {'a1': 'text2', 'a2': 1}}], 'c4': [1, 2], 'c5': {'msg': 'hello'}, 'c6': ['x', 'y', 'z'], 'c7' : 3.14}
+
+    def test_todict_level1(self):
+        self.assertEqual(to_dict(self.a), self.ad)
+
+    def test_todict_level2(self):
+        self.assertEqual(to_dict(self.b), self.bd)
+
+    def test_todict_level3(self):
+        self.assertEqual(to_dict(self.c), self.cd)
+
+    def test_toobj_level1(self):
+        self.assertEqual(to_dict( to_obj(self.ad, A) ), self.ad)
+
+    def test_toobj_level2(self):
+        self.assertEqual(to_dict( to_obj(self.bd, B) ), self.bd)
+
+    def test_toobj_level3(self):
         self.assertEqual(to_dict( to_obj(self.cd, C) ), self.cd)
```

### Comparing `mapperr-0.0.5/test/test_mapperr2.py` & `mapperr-0.1.0/test/test_unmatched_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from unittest import TestCase
-from mapperr import to_dict, to_obj
-import warnings
-
-class A:
-    a1: float
-    a2: str
-
-class TestMapperr2(TestCase):
-    def setUp(self) -> None:
-        self.a = A()
-        self.a.a1, self.a.a2 = "text", 1
-        self.ad = {"a1": "text", "a2": 1}
-
-    def test_todict_level1(self):
-        with warnings.catch_warnings(record=True) as w:
-            warnings.simplefilter("always")
-            to_dict(self.a)
-            self.assertEqual(len(w), 2)
-            
-
-    def test_toobj_level1(self):
-        with warnings.catch_warnings(record=True) as w:
-            warnings.simplefilter("always")
-            to_obj(self.ad, A)
+from unittest import TestCase
+from mapperr import to_dict, to_obj
+import warnings
+
+class A:
+    a1: float
+    a2: str
+
+class TestUnmatchedTypes(TestCase):
+    def setUp(self) -> None:
+        self.a = A()
+        self.a.a1, self.a.a2 = "text", 1
+        self.ad = {"a1": "text", "a2": 1}
+
+    def test__to_dict__throwsWarning_whenTypesAreNotMatching(self):
+        with warnings.catch_warnings(record=True) as w:
+            warnings.simplefilter("always")
+            to_dict(self.a)
+            self.assertEqual(len(w), 2)
+
+    def test__to_obj__throwsWarning_whenTypesAreNotMatching(self):
+        with warnings.catch_warnings(record=True) as w:
+            warnings.simplefilter("always")
+            to_obj(self.ad, A)
             self.assertEqual(len(w), 2)
```

