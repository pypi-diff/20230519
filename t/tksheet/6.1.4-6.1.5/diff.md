# Comparing `tmp/tksheet-6.1.4.tar.gz` & `tmp/tksheet-6.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.1.4.tar", last modified: Tue May 16 17:02:20 2023, max compression
+gzip compressed data, was "tksheet-6.1.5.tar", last modified: Fri May 19 16:16:43 2023, max compression
```

## Comparing `tksheet-6.1.4.tar` & `tksheet-6.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 17:02:20.306486 tksheet-6.1.4/
--rw-rw-rw-   0        0        0     1101 2023-05-16 06:43:15.000000 tksheet-6.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3657 2023-05-16 17:02:20.306486 tksheet-6.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3007 2023-05-16 06:43:15.000000 tksheet-6.1.4/README.md
--rw-rw-rw-   0        0        0       86 2023-05-16 17:02:20.307488 tksheet-6.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-05-16 09:10:25.000000 tksheet-6.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:02:20.297918 tksheet-6.1.4/tksheet/
--rw-rw-rw-   0        0        0     1901 2023-05-16 09:13:29.000000 tksheet-6.1.4/tksheet/__init__.py
--rw-rw-rw-   0        0        0   162453 2023-05-16 10:59:08.000000 tksheet-6.1.4/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   111539 2023-05-16 12:22:43.000000 tksheet-6.1.4/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8846 2023-05-16 09:05:56.000000 tksheet-6.1.4/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   328259 2023-05-16 13:09:52.000000 tksheet-6.1.4/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12695 2023-05-16 09:06:02.000000 tksheet-6.1.4/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   108469 2023-05-16 09:07:24.000000 tksheet-6.1.4/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5746 2023-05-16 09:06:07.000000 tksheet-6.1.4/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    59987 2023-05-16 06:43:15.000000 tksheet-6.1.4/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:02:20.306486 tksheet-6.1.4/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3657 2023-05-16 17:02:20.000000 tksheet-6.1.4/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-05-16 17:02:20.000000 tksheet-6.1.4/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 17:02:20.000000 tksheet-6.1.4/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 17:02:20.000000 tksheet-6.1.4/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 16:16:43.617146 tksheet-6.1.5/
+-rw-rw-rw-   0        0        0     1101 2023-05-19 10:58:20.000000 tksheet-6.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3657 2023-05-19 16:16:43.617146 tksheet-6.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-05-19 10:58:20.000000 tksheet-6.1.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-19 16:16:43.617146 tksheet-6.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-05-19 10:59:33.000000 tksheet-6.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:16:43.601509 tksheet-6.1.5/tksheet/
+-rw-rw-rw-   0        0        0     1901 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   163926 2023-05-19 15:49:40.000000 tksheet-6.1.5/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   111539 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0     8846 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   328259 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12695 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   108469 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5746 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    59987 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:16:43.617146 tksheet-6.1.5/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3657 2023-05-19 16:16:43.000000 tksheet-6.1.5/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-05-19 16:16:43.000000 tksheet-6.1.5/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:16:43.000000 tksheet-6.1.5/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 16:16:43.000000 tksheet-6.1.5/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.1.4/LICENSE.txt` & `tksheet-6.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.4/PKG-INFO` & `tksheet-6.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.4
+Version: 6.1.5
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.4.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.5.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.1.4/README.md` & `tksheet-6.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.4/setup.py` & `tksheet-6.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.1.4',
+  version = '6.1.5',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.4.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.5.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.1.4/tksheet/__init__.py` & `tksheet-6.1.5/tksheet/__init__.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.4/tksheet/_tksheet.py` & `tksheet-6.1.5/tksheet/_tksheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,224 +506,328 @@
             if label in self.MT.extra_header_rc_menu_funcs:
                 del self.MT.extra_header_rc_menu_funcs[label]
             if label in self.MT.extra_empty_space_rc_menu_funcs:
                 del self.MT.extra_empty_space_rc_menu_funcs[label]
         self.MT.create_rc_menus()
 
     def extra_bindings(self, bindings, func=None):
-        if func is not None and isinstance(bindings, str) and bindings.lower() in emitted_events:
-            self.bind_event(bindings, func)
-
-        if isinstance(bindings, str) and bindings.lower() in (
-            "all",
-            "bind_all",
-            "unbind_all",
-        ):
-            self.MT.extra_begin_ctrl_c_func = func
-            self.MT.extra_begin_ctrl_x_func = func
-            self.MT.extra_begin_ctrl_v_func = func
-            self.MT.extra_begin_ctrl_z_func = func
-            self.MT.extra_begin_delete_key_func = func
-            self.RI.ri_extra_begin_drag_drop_func = func
-            self.CH.ch_extra_begin_drag_drop_func = func
-            self.MT.extra_begin_del_rows_rc_func = func
-            self.MT.extra_begin_del_cols_rc_func = func
-            self.MT.extra_begin_insert_cols_rc_func = func
-            self.MT.extra_begin_insert_rows_rc_func = func
-            self.MT.extra_begin_edit_cell_func = func
-            self.CH.extra_begin_edit_cell_func = func
-            self.RI.extra_begin_edit_cell_func = func
-            self.CH.column_width_resize_func = func
-            self.RI.row_height_resize_func = func
-
-        if isinstance(bindings, str) and bindings.lower() in (
-            "all",
-            "bind_all",
-            "unbind_all",
-            "all_select_events",
-            "select",
-            "selectevents",
-            "select_events",
-        ):
-            self.MT.selection_binding_func = func
-            self.MT.select_all_binding_func = func
-            self.RI.selection_binding_func = func
-            self.CH.selection_binding_func = func
-            self.MT.drag_selection_binding_func = func
-            self.RI.drag_selection_binding_func = func
-            self.CH.drag_selection_binding_func = func
-            self.MT.shift_selection_binding_func = func
-            self.RI.shift_selection_binding_func = func
-            self.CH.shift_selection_binding_func = func
-            self.MT.ctrl_selection_binding_func = func
-            self.RI.ctrl_selection_binding_func = func
-            self.CH.ctrl_selection_binding_func = func
-            self.MT.deselection_binding_func = func
-
-        if isinstance(bindings, str) and bindings.lower() in (
-            "all",
-            "bind_all",
-            "unbind_all",
-            "all_modified_events",
-            "sheetmodified",
-            "sheet_modified" "modified_events",
-            "modified",
-        ):
-            self.MT.extra_end_ctrl_c_func = func
-            self.MT.extra_end_ctrl_x_func = func
-            self.MT.extra_end_ctrl_v_func = func
-            self.MT.extra_end_ctrl_z_func = func
-            self.MT.extra_end_delete_key_func = func
-            self.RI.ri_extra_end_drag_drop_func = func
-            self.CH.ch_extra_end_drag_drop_func = func
-            self.MT.extra_end_del_rows_rc_func = func
-            self.MT.extra_end_del_cols_rc_func = func
-            self.MT.extra_end_insert_cols_rc_func = func
-            self.MT.extra_end_insert_rows_rc_func = func
-            self.MT.extra_end_edit_cell_func = func
-            self.CH.extra_end_edit_cell_func = func
-            self.RI.extra_end_edit_cell_func = func
-
-        else:
-            if isinstance(bindings[0], str) and not isinstance(bindings, str):
-                iterable = [bindings]
-            elif isinstance(bindings, str):
-                iterable = [(bindings, func)]
-            else:
-                iterable = bindings
-            for binding, func in iterable:
-                binding == binding.lower()
-                if binding in ("begin_copy", "begin_ctrl_c"):
-                    self.MT.extra_begin_ctrl_c_func = func
-                if binding in ("ctrl_c", "end_copy", "end_ctrl_c"):
-                    self.MT.extra_end_ctrl_c_func = func
-
-                if binding in ("begin_cut", "begin_ctrl_x"):
-                    self.MT.extra_begin_ctrl_x_func = func
-                if binding in ("ctrl_x", "end_cut", "end_ctrl_x"):
-                    self.MT.extra_end_ctrl_x_func = func
-
-                if binding in ("begin_paste", "begin_ctrl_v"):
-                    self.MT.extra_begin_ctrl_v_func = func
-                if binding in ("ctrl_v", "end_paste", "end_ctrl_v"):
-                    self.MT.extra_end_ctrl_v_func = func
-
-                if binding in ("begin_undo", "begin_ctrl_z"):
-                    self.MT.extra_begin_ctrl_z_func = func
-                if binding in ("ctrl_z", "end_undo", "end_ctrl_z"):
-                    self.MT.extra_end_ctrl_z_func = func
-
-                if binding in ("begin_delete_key", "begin_delete"):
-                    self.MT.extra_begin_delete_key_func = func
-                if binding in ("delete_key", "end_delete", "end_delete_key"):
-                    self.MT.extra_end_delete_key_func = func
-
-                if binding == "begin_edit_cell":
-                    self.MT.extra_begin_edit_cell_func = func
-                if binding == "end_edit_cell" or binding == "edit_cell":
-                    self.MT.extra_end_edit_cell_func = func
-
-                if binding == "begin_edit_header":
-                    self.CH.extra_begin_edit_cell_func = func
-                if binding == "end_edit_header" or binding == "edit_header":
-                    self.CH.extra_end_edit_cell_func = func
-
-                if binding == "begin_edit_index":
-                    self.RI.extra_begin_edit_cell_func = func
-                if binding == "end_edit_index" or binding == "edit_index":
-                    self.RI.extra_end_edit_cell_func = func
-
-                if binding == "begin_row_index_drag_drop":
-                    self.RI.ri_extra_begin_drag_drop_func = func
-                if binding in ("row_index_drag_drop", "end_row_index_drag_drop"):
-                    self.RI.ri_extra_end_drag_drop_func = func
-
-                if binding == "begin_column_header_drag_drop":
-                    self.CH.ch_extra_begin_drag_drop_func = func
-                if binding in (
-                    "column_header_drag_drop",
-                    "end_column_header_drag_drop",
-                ):
-                    self.CH.ch_extra_end_drag_drop_func = func
-
-                if binding in ("begin_rc_delete_row", "begin_delete_rows"):
-                    self.MT.extra_begin_del_rows_rc_func = func
-                if binding in ("rc_delete_row", "end_rc_delete_row", "end_delete_rows"):
-                    self.MT.extra_end_del_rows_rc_func = func
-
-                if binding in ("begin_rc_delete_column", "begin_delete_columns"):
-                    self.MT.extra_begin_del_cols_rc_func = func
-                if binding in (
-                    "rc_delete_column",
-                    "end_rc_delete_column",
-                    "end_delete_columns",
-                ):
-                    self.MT.extra_end_del_cols_rc_func = func
-
-                if binding in (
-                    "begin_rc_insert_column",
-                    "begin_insert_column",
-                    "begin_insert_columns",
-                ):
-                    self.MT.extra_begin_insert_cols_rc_func = func
-                if binding in (
-                    "rc_insert_column",
-                    "end_rc_insert_column",
-                    "end_insert_column",
-                    "end_insert_columns",
-                ):
-                    self.MT.extra_end_insert_cols_rc_func = func
-
-                if binding in (
-                    "begin_rc_insert_row",
-                    "begin_insert_row",
-                    "begin_insert_rows",
-                ):
-                    self.MT.extra_begin_insert_rows_rc_func = func
-                if binding in (
-                    "rc_insert_row",
-                    "end_rc_insert_row",
-                    "end_insert_row",
-                    "end_insert_rows",
-                ):
-                    self.MT.extra_end_insert_rows_rc_func = func
-
-                if binding == "column_width_resize":
-                    self.CH.column_width_resize_func = func
-                if binding == "row_height_resize":
-                    self.RI.row_height_resize_func = func
-
-                if binding == "cell_select":
-                    self.MT.selection_binding_func = func
-                if binding in ("select_all", "ctrl_a"):
-                    self.MT.select_all_binding_func = func
-                if binding == "row_select":
-                    self.RI.selection_binding_func = func
-                if binding in ("col_select", "column_select"):
-                    self.CH.selection_binding_func = func
-                if binding == "drag_select_cells":
-                    self.MT.drag_selection_binding_func = func
-                if binding == "drag_select_rows":
-                    self.RI.drag_selection_binding_func = func
-                if binding == "drag_select_columns":
-                    self.CH.drag_selection_binding_func = func
-                if binding == "shift_cell_select":
-                    self.MT.shift_selection_binding_func = func
-                if binding == "shift_row_select":
-                    self.RI.shift_selection_binding_func = func
-                if binding == "shift_column_select":
-                    self.CH.shift_selection_binding_func = func
-                if binding == "ctrl_cell_select":
-                    self.MT.ctrl_selection_binding_func = func
-                if binding == "ctrl_row_select":
-                    self.RI.ctrl_selection_binding_func = func
-                if binding == "ctrl_column_select":
-                    self.CH.ctrl_selection_binding_func = func
-                if binding == "deselect":
-                    self.MT.deselection_binding_func = func
+        # bindings is str, func arg is None or Callable
+        if isinstance(bindings, str):
+            iterable = [(bindings, func)]
+        # bindings is list or tuple of strings, func arg is None or Callable
+        elif is_iterable(bindings) and isinstance(bindings[0], str):
+            iterable = [(b, func) for b in bindings]
+        # bindings is a list or tuple of two tuples or lists
+        # in this case the func arg is ignored
+        # e.g. [(binding, function), (binding, function), ...]
+        elif is_iterable(bindings):
+            iterable = bindings
+
+        for b, f in iterable:
+            b = b.lower()
+
+            if func is not None and b in emitted_events:
+                self.bind_event(b, f)
+
+            if b in (
+                "all",
+                "bind_all",
+                "unbind_all",
+            ):
+                self.MT.extra_begin_ctrl_c_func = f
+                self.MT.extra_begin_ctrl_x_func = f
+                self.MT.extra_begin_ctrl_v_func = f
+                self.MT.extra_begin_ctrl_z_func = f
+                self.MT.extra_begin_delete_key_func = f
+                self.RI.ri_extra_begin_drag_drop_func = f
+                self.CH.ch_extra_begin_drag_drop_func = f
+                self.MT.extra_begin_del_rows_rc_func = f
+                self.MT.extra_begin_del_cols_rc_func = f
+                self.MT.extra_begin_insert_cols_rc_func = f
+                self.MT.extra_begin_insert_rows_rc_func = f
+                self.MT.extra_begin_edit_cell_func = f
+                self.CH.extra_begin_edit_cell_func = f
+                self.RI.extra_begin_edit_cell_func = f
+                self.CH.column_width_resize_func = f
+                self.RI.row_height_resize_func = f
+
+            if b in (
+                "all",
+                "bind_all",
+                "unbind_all",
+                "all_select_events",
+                "select",
+                "selectevents",
+                "select_events",
+            ):
+                self.MT.selection_binding_func = f
+                self.MT.select_all_binding_func = f
+                self.RI.selection_binding_func = f
+                self.CH.selection_binding_func = f
+                self.MT.drag_selection_binding_func = f
+                self.RI.drag_selection_binding_func = f
+                self.CH.drag_selection_binding_func = f
+                self.MT.shift_selection_binding_func = f
+                self.RI.shift_selection_binding_func = f
+                self.CH.shift_selection_binding_func = f
+                self.MT.ctrl_selection_binding_func = f
+                self.RI.ctrl_selection_binding_func = f
+                self.CH.ctrl_selection_binding_func = f
+                self.MT.deselection_binding_func = f
+
+            if b in (
+                "all",
+                "bind_all",
+                "unbind_all",
+                "all_modified_events",
+                "sheetmodified",
+                "sheet_modified" "modified_events",
+                "modified",
+            ):
+                self.MT.extra_end_ctrl_c_func = f
+                self.MT.extra_end_ctrl_x_func = f
+                self.MT.extra_end_ctrl_v_func = f
+                self.MT.extra_end_ctrl_z_func = f
+                self.MT.extra_end_delete_key_func = f
+                self.RI.ri_extra_end_drag_drop_func = f
+                self.CH.ch_extra_end_drag_drop_func = f
+                self.MT.extra_end_del_rows_rc_func = f
+                self.MT.extra_end_del_cols_rc_func = f
+                self.MT.extra_end_insert_cols_rc_func = f
+                self.MT.extra_end_insert_rows_rc_func = f
+                self.MT.extra_end_edit_cell_func = f
+                self.CH.extra_end_edit_cell_func = f
+                self.RI.extra_end_edit_cell_func = f
+
+            if b in (
+                "begin_copy",
+                "begin_ctrl_c",
+            ):
+                self.MT.extra_begin_ctrl_c_func = f
+            if b in (
+                "ctrl_c",
+                "end_copy",
+                "end_ctrl_c",
+                "copy",
+            ):
+                self.MT.extra_end_ctrl_c_func = f
+
+            if b in (
+                "begin_cut",
+                "begin_ctrl_x",
+            ):
+                self.MT.extra_begin_ctrl_x_func = f
+            if b in (
+                "ctrl_x",
+                "end_cut",
+                "end_ctrl_x",
+                "cut",
+            ):
+                self.MT.extra_end_ctrl_x_func = f
+
+            if b in (
+                "begin_paste",
+                "begin_ctrl_v",
+            ):
+                self.MT.extra_begin_ctrl_v_func = f
+            if b in (
+                "ctrl_v",
+                "end_paste",
+                "end_ctrl_v",
+                "paste",
+            ):
+                self.MT.extra_end_ctrl_v_func = f
+
+            if b in (
+                "begin_undo",
+                "begin_ctrl_z",
+            ):
+                self.MT.extra_begin_ctrl_z_func = f
+            if b in (
+                "ctrl_z",
+                "end_undo",
+                "end_ctrl_z",
+                "undo",
+            ):
+                self.MT.extra_end_ctrl_z_func = f
+
+            if b in (
+                "begin_delete_key",
+                "begin_delete",
+            ):
+                self.MT.extra_begin_delete_key_func = f
+            if b in (
+                "delete_key",
+                "end_delete",
+                "end_delete_key",
+                "delete",
+            ):
+                self.MT.extra_end_delete_key_func = f
+
+            if b in (
+                "begin_edit_cell",
+                "begin_edit_table",
+            ):
+                self.MT.extra_begin_edit_cell_func = f
+            if b in (
+                "end_edit_cell",
+                "edit_cell",
+                "edit_table",
+            ):
+                self.MT.extra_end_edit_cell_func = f
+
+            if b == "begin_edit_header":
+                self.CH.extra_begin_edit_cell_func = f
+            if b in (
+                "end_edit_header",
+                "edit_header",
+            ):
+                self.CH.extra_end_edit_cell_func = f
+
+            if b == "begin_edit_index":
+                self.RI.extra_begin_edit_cell_func = f
+            if b in (
+                "end_edit_index",
+                "edit_index",
+            ):
+                self.RI.extra_end_edit_cell_func = f
+
+            if b in (
+                "begin_row_index_drag_drop",
+                "begin_move_rows",
+            ):
+                self.RI.ri_extra_begin_drag_drop_func = f
+            if b in (
+                "row_index_drag_drop",
+                "move_rows",
+                "end_move_rows",
+                "end_row_index_drag_drop",
+            ):
+                self.RI.ri_extra_end_drag_drop_func = f
+
+            if b in (
+                "begin_column_header_drag_drop",
+                "begin_move_columns",
+            ):
+                self.CH.ch_extra_begin_drag_drop_func = f
+            if b in (
+                "column_header_drag_drop",
+                "move_columns",
+                "end_move_columns",
+                "end_column_header_drag_drop",
+            ):
+                self.CH.ch_extra_end_drag_drop_func = f
+
+            if b in (
+                "begin_rc_delete_row",
+                "begin_delete_rows",
+            ):
+                self.MT.extra_begin_del_rows_rc_func = f
+            if b in (
+                "rc_delete_row",
+                "end_rc_delete_row",
+                "end_delete_rows",
+                "delete_rows",
+            ):
+                self.MT.extra_end_del_rows_rc_func = f
+
+            if b in (
+                "begin_rc_delete_column",
+                "begin_delete_columns",
+            ):
+                self.MT.extra_begin_del_cols_rc_func = f
+            if b in (
+                "rc_delete_column",
+                "end_rc_delete_column",
+                "end_delete_columns",
+                "delete_columns",
+            ):
+                self.MT.extra_end_del_cols_rc_func = f
+
+            if b in (
+                "begin_rc_insert_column",
+                "begin_insert_column",
+                "begin_insert_columns",
+                "begin_add_column",
+                "begin_rc_add_column",
+                "begin_add_columns",
+            ):
+                self.MT.extra_begin_insert_cols_rc_func = f
+            if b in (
+                "rc_insert_column",
+                "end_rc_insert_column",
+                "end_insert_column",
+                "end_insert_columns",
+                "rc_add_column",
+                "end_rc_add_column",
+                "end_add_column",
+                "end_add_columns",
+            ):
+                self.MT.extra_end_insert_cols_rc_func = f
+
+            if b in (
+                "begin_rc_insert_row",
+                "begin_insert_row",
+                "begin_insert_rows",
+                "begin_rc_add_row",
+                "begin_add_row",
+                "begin_add_rows",
+            ):
+                self.MT.extra_begin_insert_rows_rc_func = f
+            if b in (
+                "rc_insert_row",
+                "end_rc_insert_row",
+                "end_insert_row",
+                "end_insert_rows",
+                "rc_add_row",
+                "end_rc_add_row",
+                "end_add_row",
+                "end_add_rows",
+            ):
+                self.MT.extra_end_insert_rows_rc_func = f
+
+            if b == "column_width_resize":
+                self.CH.column_width_resize_func = f
+            if b == "row_height_resize":
+                self.RI.row_height_resize_func = f
+
+            if b == "cell_select":
+                self.MT.selection_binding_func = f
+            if b in (
+                "select_all",
+                "ctrl_a",
+            ):
+                self.MT.select_all_binding_func = f
+            if b == "row_select":
+                self.RI.selection_binding_func = f
+            if b in (
+                "col_select",
+                "column_select",
+            ):
+                self.CH.selection_binding_func = f
+            if b == "drag_select_cells":
+                self.MT.drag_selection_binding_func = f
+            if b == "drag_select_rows":
+                self.RI.drag_selection_binding_func = f
+            if b == "drag_select_columns":
+                self.CH.drag_selection_binding_func = f
+            if b == "shift_cell_select":
+                self.MT.shift_selection_binding_func = f
+            if b == "shift_row_select":
+                self.RI.shift_selection_binding_func = f
+            if b == "shift_column_select":
+                self.CH.shift_selection_binding_func = f
+            if b == "ctrl_cell_select":
+                self.MT.ctrl_selection_binding_func = f
+            if b == "ctrl_row_select":
+                self.RI.ctrl_selection_binding_func = f
+            if b == "ctrl_column_select":
+                self.CH.ctrl_selection_binding_func = f
+            if b == "deselect":
+                self.MT.deselection_binding_func = f
 
     def emit_event(self, event, data={}):
         self.event_generate(event, data=data)
 
     def bind_event(self, sequence: str, func: Callable, add: Union[str, None] = None) -> None:
         widget = self
```

### Comparing `tksheet-6.1.4/tksheet/_tksheet_column_headers.py` & `tksheet-6.1.5/tksheet/_tksheet_column_headers.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.4/tksheet/_tksheet_formatters.py` & `tksheet-6.1.5/tksheet/_tksheet_formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.4/tksheet/_tksheet_main_table.py` & `tksheet-6.1.5/tksheet/_tksheet_main_table.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.4/tksheet/_tksheet_other_classes.py` & `tksheet-6.1.5/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.4/tksheet/_tksheet_row_index.py` & `tksheet-6.1.5/tksheet/_tksheet_row_index.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.4/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.1.5/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.4/tksheet/_tksheet_vars.py` & `tksheet-6.1.5/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.4/tksheet.egg-info/PKG-INFO` & `tksheet-6.1.5/tksheet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.4
+Version: 6.1.5
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.4.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.5.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

