# Comparing `tmp/toolstr-0.9.4.tar.gz` & `tmp/toolstr-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolstr-0.9.4.tar", last modified: Tue May  9 04:46:11 2023, max compression
+gzip compressed data, was "toolstr-0.9.5.tar", last modified: Fri May 19 02:50:18 2023, max compression
```

## Comparing `toolstr-0.9.4.tar` & `toolstr-0.9.5.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.4/.gitignore
--rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.4/LICENSE
--rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.4/README.md
--rw-r--r--   0        0        0      612 2023-05-09 04:42:34.474533 toolstr-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      245 2023-05-09 04:45:20.622523 toolstr-0.9.4/toolstr/__init__.py
--rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.4/toolstr/charts/README.md
--rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.4/toolstr/charts/__init__.py
--rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.4/toolstr/charts/braille_utils.py
--rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.4/toolstr/charts/char_dicts.py
--rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.4/toolstr/charts/grid_utils.py
--rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.4/toolstr/charts/line_utils.py
--rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.4/toolstr/charts/plot_utils.py
--rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.4/toolstr/charts/raster_utils.py
--rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.4/toolstr/charts/render_utils.py
--rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.4/toolstr/charts/sextant_utils.py
--rw-r--r--   0        0        0      186 2023-04-24 03:18:32.307974 toolstr-0.9.4/toolstr/formats/__init__.py
--rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.4/toolstr/formats/bullet_formats.py
--rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.4/toolstr/formats/column_formats.py
--rw-r--r--   0        0        0     7280 2023-03-27 19:55:46.509117 toolstr-0.9.4/toolstr/formats/datatype_formats.py
--rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.4/toolstr/formats/positional_formats.py
--rw-r--r--   0        0        0     2191 2022-12-09 18:24:40.526344 toolstr-0.9.4/toolstr/formats/rich_formats.py
--rw-r--r--   0        0        0     3167 2023-04-24 06:16:05.352543 toolstr-0.9.4/toolstr/formats/template_formats.py
--rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.4/toolstr/outlines/__init__.py
--rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.4/toolstr/outlines/outline_chars.py
--rw-r--r--   0        0        0     7359 2023-05-08 16:02:35.196513 toolstr-0.9.4/toolstr/outlines/outline_printing.py
--rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.4/toolstr/py.typed
--rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.4/toolstr/spec.py
--rw-r--r--   0        0        0       28 2022-12-12 20:09:48.083313 toolstr-0.9.4/toolstr/summaries/__init__.py
--rw-r--r--   0        0        0     6158 2023-04-05 16:58:38.202042 toolstr-0.9.4/toolstr/summaries/set_summary.py
--rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.4/toolstr/tables/__init__.py
--rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.4/toolstr/tables/multiline_tables.py
--rw-r--r--   0        0        0     2983 2023-04-24 06:16:44.834292 toolstr-0.9.4/toolstr/tables/table_adapters.py
--rw-r--r--   0        0        0    33607 2023-03-22 21:23:07.773603 toolstr-0.9.4/toolstr/tables/table_utils.py
--rw-r--r--   0        0        0     8722 1970-01-01 00:00:00.000000 toolstr-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.5/LICENSE
+-rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.5/README.md
+-rw-r--r--   0        0        0      612 2023-05-09 04:42:34.474533 toolstr-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-05-19 02:49:50.256020 toolstr-0.9.5/toolstr/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-19 00:35:26.933408 toolstr-0.9.5/toolstr/buffers/__init__.py
+-rw-r--r--   0        0        0      416 2023-05-19 00:38:07.842409 toolstr-0.9.5/toolstr/buffers/stdout_utils.py
+-rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.5/toolstr/charts/README.md
+-rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.5/toolstr/charts/__init__.py
+-rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.5/toolstr/charts/braille_utils.py
+-rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.5/toolstr/charts/char_dicts.py
+-rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.5/toolstr/charts/grid_utils.py
+-rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.5/toolstr/charts/line_utils.py
+-rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.5/toolstr/charts/plot_utils.py
+-rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.5/toolstr/charts/raster_utils.py
+-rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.5/toolstr/charts/render_utils.py
+-rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.5/toolstr/charts/sextant_utils.py
+-rw-r--r--   0        0        0      186 2023-04-24 03:18:32.307974 toolstr-0.9.5/toolstr/formats/__init__.py
+-rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.5/toolstr/formats/bullet_formats.py
+-rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.5/toolstr/formats/column_formats.py
+-rw-r--r--   0        0        0     7280 2023-03-27 19:55:46.509117 toolstr-0.9.5/toolstr/formats/datatype_formats.py
+-rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.5/toolstr/formats/positional_formats.py
+-rw-r--r--   0        0        0     2191 2022-12-09 18:24:40.526344 toolstr-0.9.5/toolstr/formats/rich_formats.py
+-rw-r--r--   0        0        0     3167 2023-04-24 06:16:05.352543 toolstr-0.9.5/toolstr/formats/template_formats.py
+-rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.5/toolstr/outlines/__init__.py
+-rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.5/toolstr/outlines/outline_chars.py
+-rw-r--r--   0        0        0     7359 2023-05-08 16:02:35.196513 toolstr-0.9.5/toolstr/outlines/outline_printing.py
+-rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.5/toolstr/py.typed
+-rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.5/toolstr/spec.py
+-rw-r--r--   0        0        0       28 2022-12-12 20:09:48.083313 toolstr-0.9.5/toolstr/summaries/__init__.py
+-rw-r--r--   0        0        0     6158 2023-04-05 16:58:38.202042 toolstr-0.9.5/toolstr/summaries/set_summary.py
+-rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.5/toolstr/tables/__init__.py
+-rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.5/toolstr/tables/multiline_tables.py
+-rw-r--r--   0        0        0     2983 2023-04-24 06:16:44.834292 toolstr-0.9.5/toolstr/tables/table_adapters.py
+-rw-r--r--   0        0        0    33565 2023-05-19 02:48:05.006316 toolstr-0.9.5/toolstr/tables/table_utils.py
+-rw-r--r--   0        0        0     8722 1970-01-01 00:00:00.000000 toolstr-0.9.5/PKG-INFO
```

### Comparing `toolstr-0.9.4/LICENSE` & `toolstr-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/README.md` & `toolstr-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/pyproject.toml` & `toolstr-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/charts/braille_utils.py` & `toolstr-0.9.5/toolstr/charts/braille_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/charts/char_dicts.py` & `toolstr-0.9.5/toolstr/charts/char_dicts.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/charts/grid_utils.py` & `toolstr-0.9.5/toolstr/charts/grid_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/charts/line_utils.py` & `toolstr-0.9.5/toolstr/charts/line_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/charts/plot_utils.py` & `toolstr-0.9.5/toolstr/charts/plot_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/charts/raster_utils.py` & `toolstr-0.9.5/toolstr/charts/raster_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/charts/render_utils.py` & `toolstr-0.9.5/toolstr/charts/render_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/charts/sextant_utils.py` & `toolstr-0.9.5/toolstr/charts/sextant_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/formats/bullet_formats.py` & `toolstr-0.9.5/toolstr/formats/bullet_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/formats/column_formats.py` & `toolstr-0.9.5/toolstr/formats/column_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/formats/datatype_formats.py` & `toolstr-0.9.5/toolstr/formats/datatype_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/formats/positional_formats.py` & `toolstr-0.9.5/toolstr/formats/positional_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/formats/rich_formats.py` & `toolstr-0.9.5/toolstr/formats/rich_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/formats/template_formats.py` & `toolstr-0.9.5/toolstr/formats/template_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/outlines/outline_chars.py` & `toolstr-0.9.5/toolstr/outlines/outline_chars.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/outlines/outline_printing.py` & `toolstr-0.9.5/toolstr/outlines/outline_printing.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/spec.py` & `toolstr-0.9.5/toolstr/spec.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/summaries/set_summary.py` & `toolstr-0.9.5/toolstr/summaries/set_summary.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/tables/multiline_tables.py` & `toolstr-0.9.5/toolstr/tables/multiline_tables.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/tables/table_adapters.py` & `toolstr-0.9.5/toolstr/tables/table_adapters.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.4/toolstr/tables/table_utils.py` & `toolstr-0.9.5/toolstr/tables/table_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1033,15 +1033,14 @@
         if console is None:
             import rich.console
 
             console = rich.console.Console(
                 file=file,
                 theme=rich.theme.Theme(inherit=False),
                 width=10000,
-                color_system='truecolor',
             )
         console.print(table_as_str)
 
     else:
         print(table_as_str)
```

### Comparing `toolstr-0.9.4/PKG-INFO` & `toolstr-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolstr
-Version: 0.9.4
+Version: 0.9.5
 Summary: toolstr is a suite of str processing tools, including formatting and drawing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: tooltime>=0.2.10
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: scikit-image>=0.19.2 ; extra == "full"
 Requires-Dist: rich>=12.1.0 ; extra == "full"
```

