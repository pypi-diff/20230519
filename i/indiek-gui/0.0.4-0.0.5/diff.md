# Comparing `tmp/indiek-gui-0.0.4.tar.gz` & `tmp/indiek-gui-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-gui/dist/.tmp-2dm50h__/indiek-gui-0.0.4.tar", last modified: Thu May 18 00:42:24 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-gui/dist/.tmp-d5fl3g_9/indiek-gui-0.0.5.tar", last modified: Thu May 18 22:24:34 2023, max compression
```

## Comparing `indiek-gui-0.0.4.tar` & `indiek-gui-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:42:24.230288 indiek-gui-0.0.4/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-05-05 01:24:51.000000 indiek-gui-0.0.4/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-18 00:42:24.230288 indiek-gui-0.0.4/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      555 2023-05-06 19:18:51.000000 indiek-gui-0.0.4/README.rst
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:42:24.206288 indiek-gui-0.0.4/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:42:24.230288 indiek-gui-0.0.4/indiek/gui/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       34 2023-05-09 22:32:51.000000 indiek-gui-0.0.4/indiek/gui/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    22894 2023-05-18 00:36:44.000000 indiek-gui-0.0.4/indiek/gui/app.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     2745 2023-05-13 12:07:45.000000 indiek-gui-0.0.4/indiek/gui/items.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3932 2023-05-14 16:42:30.000000 indiek-gui-0.0.4/indiek/gui/styles.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:42:24.230288 indiek-gui-0.0.4/indiek_gui.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      325 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       47 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/entry_points.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       56 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-18 00:42:24.000000 indiek-gui-0.0.4/indiek_gui.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      147 2023-05-18 00:42:24.230288 indiek-gui-0.0.4/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      920 2023-05-09 22:33:03.000000 indiek-gui-0.0.4/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:24:34.233131 indiek-gui-0.0.5/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-05-05 01:24:51.000000 indiek-gui-0.0.5/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1228 2023-05-18 22:24:34.233131 indiek-gui-0.0.5/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      780 2023-05-18 22:14:41.000000 indiek-gui-0.0.5/README.rst
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:24:34.229131 indiek-gui-0.0.5/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:24:34.233131 indiek-gui-0.0.5/indiek/gui/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       34 2023-05-09 22:32:51.000000 indiek-gui-0.0.5/indiek/gui/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    23176 2023-05-18 01:13:15.000000 indiek-gui-0.0.5/indiek/gui/app.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     2957 2023-05-18 01:10:23.000000 indiek-gui-0.0.5/indiek/gui/items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3932 2023-05-14 16:42:30.000000 indiek-gui-0.0.5/indiek/gui/styles.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 22:24:34.233131 indiek-gui-0.0.5/indiek_gui.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1228 2023-05-18 22:24:34.000000 indiek-gui-0.0.5/indiek_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      325 2023-05-18 22:24:34.000000 indiek-gui-0.0.5/indiek_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-18 22:24:34.000000 indiek-gui-0.0.5/indiek_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       47 2023-05-18 22:24:34.000000 indiek-gui-0.0.5/indiek_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       63 2023-05-18 22:24:34.000000 indiek-gui-0.0.5/indiek_gui.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-18 22:24:34.000000 indiek-gui-0.0.5/indiek_gui.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      147 2023-05-18 22:24:34.233131 indiek-gui-0.0.5/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      928 2023-05-18 22:12:53.000000 indiek-gui-0.0.5/setup.py
```

### Comparing `indiek-gui-0.0.4/LICENSE` & `indiek-gui-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-gui-0.0.4/PKG-INFO` & `indiek-gui-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiek-gui
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tkinter GUI for IndieK
 Home-page: https://pypi.org/project/indiek-gui/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek-gui
 Project-URL: Documentation, https://indiekgui.readthedocs.io/en/latest/
@@ -31,12 +31,17 @@
 ==========
 Call ``indiek-gui`` from your terminal to launch the GUI.
 
 ..  code-block:: bash
 
     indiek-gui
 
+This GUI enables you to create definitions, theorems and proofs,
+and store them on an mock Database. It offers you the possibility
+to persist the mock database to your file system as a JSON file, 
+and to reload it later on.
+
 =====
 Tests
 =====
 To run the full test suite, type the following from the top level of this repo:
 ``pytest``
```

### Comparing `indiek-gui-0.0.4/indiek/gui/app.py` & `indiek-gui-0.0.5/indiek/gui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,41 +9,45 @@
 from typing import Optional, Mapping, Tuple, Iterator
 from tkinter import *
 from tkinter import filedialog
 from tkinter import ttk
 from functools import partial
 from indiek.mockdb.persistence import persist, load_from_file
 from indiek.core.search import list_all_items, filter_str
-from indiek.gui.items import core_to_gui_item, Item as GUIItem, Definition, Theorem, Proof
+from indiek.gui.items import core_to_gui_item, Item as GUIItem, Definition, Theorem, Proof, Note, Question
 from indiek.gui.styles import IndiekTheme, DEFAULT_FONT
 from indiek.core.items import (Definition as CoreDefinition, 
                                Theorem as CoreTheorem, 
-                               Proof as CoreProof)
+                               Proof as CoreProof,
+                               Note as CoreNote, 
+                               Question as CoreQuestion)
 from . import __version__
 
 
 PairOfInt = Tuple[int, int]
 
 
 DEFAULT_PERSISTENCE_DIR = '/home/adrian_admin/prog/indiek/indiek-gui/.data/'
 """Path where DB gets persisted and loaded from."""
 
 
-ITEM_TYPES = [Definition, Theorem, Proof]
+ITEM_TYPES = [Definition, Theorem, Proof, Note, Question]
 """List of item types."""
 
 
-FILTER_NAMES = ['Definitions', 'Theorems', 'Proofs']
+FILTER_NAMES = ['Definitions', 'Theorems', 'Proofs', 'Notes', 'Questions']
 """Strings used in filter radio buttons for each Item type."""
 
 
 NAME_TO_ITEM_TYPE = {
     'Definitions': CoreDefinition, 
     'Theorems': CoreTheorem, 
-    'Proofs': CoreProof
+    'Proofs': CoreProof,
+    'Notes': CoreNote, 
+    'Questions': CoreQuestion,
 }
 assert set(NAME_TO_ITEM_TYPE.keys()) == set(FILTER_NAMES)
 
 
 CANVAS_OPTIONS = {
     'search_results': dict(
         background='blue',
@@ -638,24 +642,25 @@
                 content_var=StringVar(value=self._default_str),
                 name=self._default_str, 
                 content=self._default_str
                 )
 
     def persist_box(self):
         filename = filedialog.asksaveasfilename(initialdir=DEFAULT_PERSISTENCE_DIR)
-        persist(filename)
+        if filename:
+            persist(filename)
 
     def load_box(self):
         filename = filedialog.askopenfilename(initialdir=DEFAULT_PERSISTENCE_DIR)
-        load_from_file(filename)
-        neutral_item = self._initialize_view_var()
-        self.populate_view_pane(neutral_item)
-        self.clear_all_search()
-        self.collect_search()
-
+        if filename:
+            load_from_file(filename)
+            neutral_item = self._initialize_view_var()
+            self.populate_view_pane(neutral_item)
+            self.clear_all_search()
+            self.collect_search()
 
     def create_main_menu(self):
         win = self.root
         menubar = Menu(win)
         menu_file = Menu(menubar)
         menu_file.add_command(label='Persist Session', command=self.persist_box)
         menu_file.add_command(label='Load Session', command=self.load_box)
```

### Comparing `indiek-gui-0.0.4/indiek/gui/items.py` & `indiek-gui-0.0.5/indiek/gui/items.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from tkinter import StringVar
 from indiek.core.items import (Item as CoreItem,
                                Definition as CoreDefinition,
                                Proof as CoreProof,
-                               Theorem as CoreTheorem)
+                               Theorem as CoreTheorem,
+                               Note as CoreNote,
+                               Question as CoreQuestion)
 
 
 class Item(CoreItem):
     """
     Indiek GUI Item.
 
     This subclasses the core Item class and adds some GUI-specific functionality.
@@ -56,30 +58,26 @@
         return super().save()
 
     def delete(self):
         super().delete()
         for n in self._str_var_names:
             self.update_str_var(n, '', set_core_attr=True)
 
-class Definition(Item, CoreDefinition):
-    pass
-
-
-class Proof(Item, CoreProof):
-    pass
-
-
-class Theorem(Item, CoreTheorem):
-    pass
-
+class Definition(Item, CoreDefinition): pass
+class Proof(Item, CoreProof): pass
+class Theorem(Item, CoreTheorem): pass
+class Note(Item, CoreNote): pass
+class Question(Item, CoreQuestion): pass
 
 CORE_TO_GUI_TYPES = {
     CoreDefinition: Definition,
     CoreProof: Proof,
-    CoreTheorem: Theorem
+    CoreTheorem: Theorem,
+    CoreNote: Note,
+    CoreQuestion: Question,
 }
 
 
 def core_to_gui_item(core_item: CoreItem, name_var: StringVar, content_var: StringVar) -> Item:
     kwargs = dict(name_var=name_var, content_var=content_var)
     kwargs.update({a: getattr(core_item, a) for a in core_item._attr_defs})
     return CORE_TO_GUI_TYPES[core_item.__class__](**kwargs)
```

### Comparing `indiek-gui-0.0.4/indiek/gui/styles.py` & `indiek-gui-0.0.5/indiek/gui/styles.py`

 * *Files identical despite different names*

### Comparing `indiek-gui-0.0.4/indiek_gui.egg-info/PKG-INFO` & `indiek-gui-0.0.5/indiek_gui.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiek-gui
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tkinter GUI for IndieK
 Home-page: https://pypi.org/project/indiek-gui/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek-gui
 Project-URL: Documentation, https://indiekgui.readthedocs.io/en/latest/
@@ -31,12 +31,17 @@
 ==========
 Call ``indiek-gui`` from your terminal to launch the GUI.
 
 ..  code-block:: bash
 
     indiek-gui
 
+This GUI enables you to create definitions, theorems and proofs,
+and store them on an mock Database. It offers you the possibility
+to persist the mock database to your file system as a JSON file, 
+and to reload it later on.
+
 =====
 Tests
 =====
 To run the full test suite, type the following from the top level of this repo:
 ``pytest``
```

### Comparing `indiek-gui-0.0.4/setup.py` & `indiek-gui-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, 'README.rst'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='indiek-gui',
     python_requires='>=3.8',
-    version='0.0.4',
+    version='0.0.5',
     url='https://pypi.org/project/indiek-gui/',
     description='Tkinter GUI for IndieK',
     long_description=long_description,
     author='Adrian Ernesto Radillo',
     author_email='adrian.radillo@gmail.com',
     license='GNU Affero General Public License v3.0',
     packages=['indiek.gui'],
-    install_requires=['indiek-core == 0.1.4'],
+    install_requires=['indiek-core >= 0.1.5, <0.2.0'],
     extras_require={
         'dev': [
             'pytest',
             'pytest-pep8',
             'pytest-cov'
         ]
     },
```

