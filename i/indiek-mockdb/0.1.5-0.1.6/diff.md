# Comparing `tmp/indiek-mockdb-0.1.5.tar.gz` & `tmp/indiek-mockdb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-mockdb/dist/.tmp-02h09s8j/indiek-mockdb-0.1.5.tar", last modified: Thu May 18 00:44:55 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-mockdb/dist/.tmp-esq38ov4/indiek-mockdb-0.1.6.tar", last modified: Thu May 18 22:20:11 2023, max compression
```

## Comparing `indiek-mockdb-0.1.5.tar` & `indiek-mockdb-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:44:55.780690 indiek-mockdb-0.1.5/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-16 01:06:17.000000 indiek-mockdb-0.1.5/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-18 00:44:55.780690 indiek-mockdb-0.1.5/PKG-INFO
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:44:55.760689 indiek-mockdb-0.1.5/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:44:55.776690 indiek-mockdb-0.1.5/indiek/mockdb/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-04-16 01:07:43.000000 indiek-mockdb-0.1.5/indiek/mockdb/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     5620 2023-05-11 10:29:28.000000 indiek-mockdb-0.1.5/indiek/mockdb/items.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      512 2023-05-17 23:56:30.000000 indiek-mockdb-0.1.5/indiek/mockdb/persistence.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:44:55.780690 indiek-mockdb-0.1.5/indiek_mockdb.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-18 00:44:55.000000 indiek-mockdb-0.1.5/indiek_mockdb.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      308 2023-05-18 00:44:55.000000 indiek-mockdb-0.1.5/indiek_mockdb.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-18 00:44:55.000000 indiek-mockdb-0.1.5/indiek_mockdb.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       37 2023-05-18 00:44:55.000000 indiek-mockdb-0.1.5/indiek_mockdb.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-18 00:44:55.000000 indiek-mockdb-0.1.5/indiek_mockdb.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-18 00:44:55.780690 indiek-mockdb-0.1.5/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      656 2023-05-17 23:59:52.000000 indiek-mockdb-0.1.5/setup.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:44:55.780690 indiek-mockdb-0.1.5/tests/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3766 2023-05-10 09:58:53.000000 indiek-mockdb-0.1.5/tests/test_items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:20:11.972694 indiek-mockdb-0.1.6/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-16 01:06:17.000000 indiek-mockdb-0.1.6/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      509 2023-05-18 22:20:11.972694 indiek-mockdb-0.1.6/PKG-INFO
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:20:11.956694 indiek-mockdb-0.1.6/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:20:11.972694 indiek-mockdb-0.1.6/indiek/mockdb/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-04-16 01:07:43.000000 indiek-mockdb-0.1.6/indiek/mockdb/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     5885 2023-05-18 01:04:18.000000 indiek-mockdb-0.1.6/indiek/mockdb/items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      512 2023-05-17 23:56:30.000000 indiek-mockdb-0.1.6/indiek/mockdb/persistence.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:20:11.972694 indiek-mockdb-0.1.6/indiek_mockdb.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      509 2023-05-18 22:20:11.000000 indiek-mockdb-0.1.6/indiek_mockdb.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      308 2023-05-18 22:20:11.000000 indiek-mockdb-0.1.6/indiek_mockdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-18 22:20:11.000000 indiek-mockdb-0.1.6/indiek_mockdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       48 2023-05-18 22:20:11.000000 indiek-mockdb-0.1.6/indiek_mockdb.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-18 22:20:11.000000 indiek-mockdb-0.1.6/indiek_mockdb.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-18 22:20:11.972694 indiek-mockdb-0.1.6/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      759 2023-05-18 22:19:33.000000 indiek-mockdb-0.1.6/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:20:11.972694 indiek-mockdb-0.1.6/tests/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3732 2023-05-18 01:02:49.000000 indiek-mockdb-0.1.6/tests/test_items.py
```

### Comparing `indiek-mockdb-0.1.5/LICENSE` & `indiek-mockdb-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-mockdb-0.1.5/indiek/mockdb/items.py` & `indiek-mockdb-0.1.6/indiek/mockdb/items.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 import re
 from typing import Sequence, Optional, List, Any
 from frozendict import frozendict
 
 
+
 class MixedTypeOverrideError(Exception):
     """
     An item is trying to be saved with an ID 
     pertaining to an existing item of a different type.
     """
     pass
 
@@ -31,14 +32,16 @@
         _ikid (int): ID of item in mockdb. This is not part of indiek-core API.
     """
 
     _item_dict = frozendict(
         Definition = {},  # keys MUST match class names from module
         Theorem = {},
         Proof = {},
+        Note = {},
+        Question = {}
     )
     """
     All items are stored in this class variable. It is a nested dict. First level of 
     keys are classes, and values are dicts. Second level of keys are item unique IDs 
     (_ikid) and values are dicts containing item data."""
 
     _attr_defs = ['name', 'content', '_ikid']
@@ -168,15 +171,23 @@
         Returns:
             List[Item]: stored items.
         """
         class_items = cls._item_dict[cls.__name__]
         return [cls(**item_dict) for item_dict in class_items.values()]
 
 
-class Definition(Item):
-    pass
-
-class Theorem(Item):
-    pass
-
-class Proof(Item):
-    pass
+# TODO: automate class create below (__new__?)
+# Note impact of classes below on Item._item_dict
+class Definition(Item): pass
+class Theorem(Item): pass
+class Proof(Item): pass
+class Note(Item): pass
+class Question(Item): pass
+
+
+ITEM_CLASSES = [
+    Definition, 
+    Theorem, 
+    Proof,
+    Note,
+    Question,
+    ]
```

### Comparing `indiek-mockdb-0.1.5/indiek/mockdb/persistence.py` & `indiek-mockdb-0.1.6/indiek/mockdb/persistence.py`

 * *Files identical despite different names*

### Comparing `indiek-mockdb-0.1.5/tests/test_items.py` & `indiek-mockdb-0.1.6/tests/test_items.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import unittest
-from indiek.mockdb.items import Definition, Theorem, Proof, MixedTypeOverrideError
+from indiek.mockdb.items import Definition, Theorem, Proof, ITEM_CLASSES, MixedTypeOverrideError
 import re
 
 
-ITEM_CHILDREN = [Definition, Theorem, Proof]
-
-
 class TestItemAPI(unittest.TestCase):
     def test_instantiation(self):
         """Test that mockdb Item has the attr specified by indiek-core API."""
 
         item = Theorem()
         expected_attr = [
             'name',
@@ -95,15 +92,15 @@
         stored = Proof.list_all()
         self.assertIn(item3, stored)
 
     def test_str_filter(self):
         bambi = re.compile('bambi')
         nany = re.compile('nany')
         bamb = re.compile('bamb')
-        for cls in ITEM_CHILDREN:
+        for cls in ITEM_CLASSES:
             # write two items with specific str
             name_str = cls.__name__ + ' bambi'
             content_str = cls.__name__ + ' nany'
             cls(name=name_str, content=content_str).save()
 
             name_str = cls.__name__ + ' bamboo'
             content_str = cls.__name__ + ' granny'
```

