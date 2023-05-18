# Comparing `tmp/indiek-core-0.1.4.tar.gz` & `tmp/indiek-core-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-core/dist/.tmp-dyo32cgb/indiek-core-0.1.4.tar", last modified: Thu May 18 00:48:14 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-core/dist/.tmp-ks8ar6w_/indiek-core-0.1.5.tar", last modified: Thu May 18 22:21:27 2023, max compression
```

## Comparing `indiek-core-0.1.4.tar` & `indiek-core-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:48:14.639869 indiek-core-0.1.4/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-15 20:23:22.000000 indiek-core-0.1.4/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1165 2023-05-18 00:48:14.639869 indiek-core-0.1.4/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      714 2023-05-09 22:12:17.000000 indiek-core-0.1.4/README.rst
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:48:14.619868 indiek-core-0.1.4/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:48:14.639869 indiek-core-0.1.4/indiek/core/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-05-07 17:29:44.000000 indiek-core-0.1.4/indiek/core/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3588 2023-05-13 11:39:09.000000 indiek-core-0.1.4/indiek/core/items.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3488 2023-05-08 22:13:30.000000 indiek-core-0.1.4/indiek/core/search.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:48:14.639869 indiek-core-0.1.4/indiek_core.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1165 2023-05-18 00:48:14.000000 indiek-core-0.1.4/indiek_core.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      319 2023-05-18 00:48:14.000000 indiek-core-0.1.4/indiek_core.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-18 00:48:14.000000 indiek-core-0.1.4/indiek_core.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       58 2023-05-18 00:48:14.000000 indiek-core-0.1.4/indiek_core.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-18 00:48:14.000000 indiek-core-0.1.4/indiek_core.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-18 00:48:14.639869 indiek-core-0.1.4/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      924 2023-05-18 00:01:49.000000 indiek-core-0.1.4/setup.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:48:14.639869 indiek-core-0.1.4/tests/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1528 2023-05-10 02:20:52.000000 indiek-core-0.1.4/tests/test_items.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3031 2023-05-08 22:21:51.000000 indiek-core-0.1.4/tests/test_search.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:21:27.384824 indiek-core-0.1.5/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-15 20:23:22.000000 indiek-core-0.1.5/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1320 2023-05-18 22:21:27.384824 indiek-core-0.1.5/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      869 2023-05-18 22:17:14.000000 indiek-core-0.1.5/README.rst
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:21:27.360824 indiek-core-0.1.5/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:21:27.384824 indiek-core-0.1.5/indiek/core/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-05-07 17:29:44.000000 indiek-core-0.1.5/indiek/core/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3777 2023-05-18 01:07:27.000000 indiek-core-0.1.5/indiek/core/items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3682 2023-05-18 01:27:39.000000 indiek-core-0.1.5/indiek/core/search.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:21:27.384824 indiek-core-0.1.5/indiek_core.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1320 2023-05-18 22:21:27.000000 indiek-core-0.1.5/indiek_core.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      319 2023-05-18 22:21:27.000000 indiek-core-0.1.5/indiek_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-18 22:21:27.000000 indiek-core-0.1.5/indiek_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       65 2023-05-18 22:21:27.000000 indiek-core-0.1.5/indiek_core.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-18 22:21:27.000000 indiek-core-0.1.5/indiek_core.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-18 22:21:27.384824 indiek-core-0.1.5/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      934 2023-05-18 22:12:08.000000 indiek-core-0.1.5/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:21:27.384824 indiek-core-0.1.5/tests/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1498 2023-05-18 01:07:32.000000 indiek-core-0.1.5/tests/test_items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3003 2023-05-18 01:21:54.000000 indiek-core-0.1.5/tests/test_search.py
```

### Comparing `indiek-core-0.1.4/LICENSE` & `indiek-core-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-core-0.1.4/PKG-INFO` & `indiek-core-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: indiek-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: core logic for indiek
 Home-page: https://pypi.org/project/indiek-core/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek.core
 Project-URL: Documentation, https://indiekcore.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
 
 Library that stores the core logic for the IndieK software suite.
 
+This library is not meant to be used directly. Rather, it should be
+used by GUIs or web apps that wish to comply with the IndieK API.
+
 ============
 Installation
 ============
 
 To install from PyPI: ``pip install indiek-core``
 
 To develop, use the [dev] dependency specification, e.g.:
@@ -36,12 +39,14 @@
     
     item1 = Definition(name='def1', content='example def 1')
     item1_id = item1.save()
 
     reloaded = Definition.load(item1_id)
     assert item1 == reloaded
 
+    item1.delete()
+
 =====
 Tests
 =====
 To run the full test suite, type the following from the top level of this repo:
 ``pytest``
```

### Comparing `indiek-core-0.1.4/README.rst` & `indiek-core-0.1.5/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 Library that stores the core logic for the IndieK software suite.
 
+This library is not meant to be used directly. Rather, it should be
+used by GUIs or web apps that wish to comply with the IndieK API.
+
 ============
 Installation
 ============
 
 To install from PyPI: ``pip install indiek-core``
 
 To develop, use the [dev] dependency specification, e.g.:
@@ -22,12 +25,14 @@
     
     item1 = Definition(name='def1', content='example def 1')
     item1_id = item1.save()
 
     reloaded = Definition.load(item1_id)
     assert item1 == reloaded
 
+    item1.delete()
+
 =====
 Tests
 =====
 To run the full test suite, type the following from the top level of this repo:
 ``pytest``
```

### Comparing `indiek-core-0.1.4/indiek/core/items.py` & `indiek-core-0.1.5/indiek/core/items.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,20 +88,19 @@
         return cls(**db_item.to_dict())
     
     def to_dict(self):
         """Export core Item content to dict."""
         return {a: getattr(self, a) for a in self._attr_defs}
     
 
+# TODO: automate class creation below
 class Definition(Item):
     BACKEND_CLS = default_driver.Definition
-    pass
-
-
 class Theorem(Item):
     BACKEND_CLS = default_driver.Theorem
-    pass
-
-
 class Proof(Item):
     BACKEND_CLS = default_driver.Proof
-    pass
+class Note(Item):
+    BACKEND_CLS = default_driver.Note
+class Question(Item):
+    BACKEND_CLS = default_driver.Question
+CORE_ITEM_TYPES = [Definition, Theorem, Proof, Note, Question]
```

### Comparing `indiek-core-0.1.4/indiek/core/search.py` & `indiek-core-0.1.5/indiek/core/search.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Search logic for the core IndieK API."""
 import re
 from typing import List, Union, Sequence, Dict
-from indiek.core.items import Item, Definition, Theorem, Proof
+from indiek.core.items import Item, Definition, Theorem, Proof, Note, Question
+from indiek.core.items import CORE_ITEM_TYPES as ITEM_TYPES
 from indiek.mockdb.items import (Item as DBItem,
                                  Definition as DBDefinition,
                                  Theorem as DBTheorem,
-                                 Proof as DBProof)
+                                 Proof as DBProof,
+                                 Note as DBNote,
+                                 Question as DBQuestion)
 
 
-BackendItem = Union[DBItem, DBDefinition, DBTheorem, DBProof]
-ITEM_TYPES = Definition, Theorem, Proof
+BackendItem = Union[DBItem, DBDefinition, DBTheorem, DBProof, DBNote, DBQuestion]
 
 
 def build_search_query(string: str) -> re.Pattern:
     base_str = '('
     base_str += '|'.join(string.split())
     base_str += ')'
     return re.compile(base_str, flags=re.IGNORECASE)
@@ -42,15 +44,15 @@
     Returns:
         List[Item]: list of core items
     """
     db_cls = core_cls.BACKEND_CLS
     return [core_cls.from_db(dbi) for dbi in db_cls.list_all()]
 
 
-def list_all_items(item_types: Sequence[Item] = (Definition, Theorem, Proof)) -> Dict[Item, List[Item]]:
+def list_all_items(item_types: Sequence[Item] = (Definition, Theorem, Proof, Note, Question)) -> Dict[Item, List[Item]]:
     """Fetch all items with optional type filter.
 
     Args:
         item_types (Sequence[Item], optional): list-like of core item types to use for segmented
             search. For example, if item_types is [Proof, Theorem], then backend will be queried only for these
             two types (more precisely for their corresponding types in backend typing). Defaults to (Definition,
             Theorem, Proof) in which case all types are queried. Note that another way to query all items without filtering 
@@ -62,15 +64,15 @@
             the default keys (Definition, Theorem, Proof).
     """
     if len(item_types) == 0:
         item_types = ITEM_TYPES
     return {item_type: fetch_and_cast(item_type) for item_type in item_types}
 
 
-def filter_str(search_str: str, item_types: Sequence[Item] = (Definition, Theorem, Proof)) -> Dict[Item, List[Item]]:
+def filter_str(search_str: str, item_types: Sequence[Item] = (Definition, Theorem, Proof, Note, Question)) -> Dict[Item, List[Item]]:
     """Search items from specified type which match search string.
 
     Backend items of type compatible with item_types are searched, retrieved and cast to Core type.
     The search_str is split on white spaces and regex are built and 'and-ed'. The resulting regex is
     applied on item name and content.
     
     Args:
```

### Comparing `indiek-core-0.1.4/indiek_core.egg-info/PKG-INFO` & `indiek-core-0.1.5/indiek_core.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: indiek-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: core logic for indiek
 Home-page: https://pypi.org/project/indiek-core/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek.core
 Project-URL: Documentation, https://indiekcore.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
 
 Library that stores the core logic for the IndieK software suite.
 
+This library is not meant to be used directly. Rather, it should be
+used by GUIs or web apps that wish to comply with the IndieK API.
+
 ============
 Installation
 ============
 
 To install from PyPI: ``pip install indiek-core``
 
 To develop, use the [dev] dependency specification, e.g.:
@@ -36,12 +39,14 @@
     
     item1 = Definition(name='def1', content='example def 1')
     item1_id = item1.save()
 
     reloaded = Definition.load(item1_id)
     assert item1 == reloaded
 
+    item1.delete()
+
 =====
 Tests
 =====
 To run the full test suite, type the following from the top level of this repo:
 ``pytest``
```

### Comparing `indiek-core-0.1.4/setup.py` & `indiek-core-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, 'README.rst'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='indiek-core',
     python_requires='>=3.8',
-    version='0.1.4',
+    version='0.1.5',
     url='https://pypi.org/project/indiek-core/',
     description='core logic for indiek',
     long_description=long_description,
     author='Adrian Ernesto Radillo',
     author_email='adrian.radillo@gmail.com',
     license='GNU Affero General Public License v3.0',
     packages=['indiek.core'],
-    install_requires=['indiek-mockdb>=0.1.4'],
+    install_requires=['indiek-mockdb >= 0.1.6, <0.2.0'],
     extras_require={
         'dev': [
             'pytest',
             'pytest-pep8',
             'pytest-cov'
         ]
     },
```

### Comparing `indiek-core-0.1.4/tests/test_items.py` & `indiek-core-0.1.5/tests/test_items.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
-from indiek.core.items import Item, Definition, Theorem, Proof
+from indiek.core.items import Item, Definition, Theorem, Proof, CORE_ITEM_TYPES
 from indiek.mockdb.items import Definition as DBDefinition
 from indiek import mockdb
 
-CORE_ITEM_TYPES = [Definition, Theorem, Proof]
 
 class TestItemAttr(unittest.TestCase):
     def test_instantiation(self):
         item = Item()
         expected_attr = [
             'name',
             'content',
```

### Comparing `indiek-core-0.1.4/tests/test_search.py` & `indiek-core-0.1.5/tests/test_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import unittest
 import re
-from indiek.core.items import  Proof, Theorem, Definition
+from indiek.core.items import  Proof, Theorem, Definition, CORE_ITEM_TYPES
 from indiek.core.search import list_all_items, search_and_cast, build_search_query, filter_str
 
 
-CORE_ITEM_TYPES = [Proof, Theorem, Definition]
-
-
 class TestSearch(unittest.TestCase):
     def setUp(self) -> None:
         """Make sure DB has at least 1 Item of each type."""
         self.ids = {cls: cls(name=str(cls)).save() for cls in CORE_ITEM_TYPES}
 
-    def test_list_all_items(self):
+    def test_list_all_items_1(self):
         # all written items have 'class' in their name
         class_in_name = filter_str("class")
             
         for written_cls in self.ids.keys():
             loaded_item = written_cls.load(self.ids[written_cls])
             self.assertIn(loaded_item, class_in_name[written_cls])
         
@@ -26,15 +23,15 @@
         # check type-specific results contain expected ids from setUp
         for core_type, core_items in thm_prf.items():
             if core_type in {Theorem, Proof}:
                 self.assertTrue(core_items)
             elif core_type == Definition:
                 self.assertFalse(core_items)
 
-    def test_list_all_items(self):
+    def test_list_all_items_2(self):
         # at least written items from setUp should be present
         all_items = []
         for ilist in list_all_items().values():
             all_items += ilist
             
         all_item_ids = [i._ikid for i in all_items]
         for written in self.ids.values():
```

