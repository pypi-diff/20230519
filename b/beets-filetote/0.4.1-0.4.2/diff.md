# Comparing `tmp/beets_filetote-0.4.1.tar.gz` & `tmp/beets_filetote-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beets_filetote-0.4.1.tar", max compression
+gzip compressed data, was "beets_filetote-0.4.2.tar", max compression
```

## Comparing `beets_filetote-0.4.1.tar` & `beets_filetote-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1143 2023-05-15 22:44:37.210357 beets_filetote-0.4.1/LICENSE
--rw-r--r--   0        0        0    13893 2023-05-15 22:44:37.210357 beets_filetote-0.4.1/README.md
--rw-r--r--   0        0        0      144 2023-05-15 22:44:37.210357 beets_filetote-0.4.1/beetsplug/__init__.py
--rw-r--r--   0        0        0    24313 2023-05-15 22:44:37.210357 beets_filetote-0.4.1/beetsplug/filetote.py
--rw-r--r--   0        0        0     2571 2023-05-15 22:44:37.210357 beets_filetote-0.4.1/beetsplug/filetote_dataclasses.py
--rw-r--r--   0        0        0     2205 2023-05-15 22:44:37.210357 beets_filetote-0.4.1/beetsplug/mapping_model.py
--rw-r--r--   0        0        0     2010 2023-05-15 22:44:37.210357 beets_filetote-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    15515 1970-01-01 00:00:00.000000 beets_filetote-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1143 2023-05-19 20:49:37.517447 beets_filetote-0.4.2/LICENSE
+-rw-r--r--   0        0        0    13886 2023-05-19 20:49:37.517447 beets_filetote-0.4.2/README.md
+-rw-r--r--   0        0        0      144 2023-05-19 20:49:37.517447 beets_filetote-0.4.2/beetsplug/__init__.py
+-rw-r--r--   0        0        0    24368 2023-05-19 20:49:37.521447 beets_filetote-0.4.2/beetsplug/filetote.py
+-rw-r--r--   0        0        0     2571 2023-05-19 20:49:37.521447 beets_filetote-0.4.2/beetsplug/filetote_dataclasses.py
+-rw-r--r--   0        0        0     2205 2023-05-19 20:49:37.521447 beets_filetote-0.4.2/beetsplug/mapping_model.py
+-rw-r--r--   0        0        0     2010 2023-05-19 20:49:37.521447 beets_filetote-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    15508 1970-01-01 00:00:00.000000 beets_filetote-0.4.2/PKG-INFO
```

### Comparing `beets_filetote-0.4.1/LICENSE` & `beets_filetote-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beets_filetote-0.4.1/README.md` & `beets_filetote-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![MIT license][license image]][license link]
 [![CI][ci image]][ci link]
 [![GitHub release][github image]][github link]
 [![PyPI][pypi_version]][pypi_link]
 [![PyPI - Python Version][pypi_python_versions]][pypi_link]
 
 A plugin that moves non-music extra files, attachments, and artifacts during
-the import process for [beets](http://beets.radbox.org/), a music library
+the import process for [beets](https://beets.io/), a music library
 manager (and much more!).
 
 ## Installing
 
 ### Stable
 
 The stable version of the plugin is available from PyPI and can be installed
```

### Comparing `beets_filetote-0.4.1/beetsplug/filetote.py` & `beets_filetote-0.4.2/beetsplug/filetote.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,16 @@
                     selected_path_format = path_format
             elif (
                 pattern_category
                 and not query.startswith(
                     (filename_prefix, paired_ext_prefix, ext_prefix)
                 )
                 and self.remove_prefix(query, pattern_prefix) == pattern_category
-            ):  # This should pull the corresponding pattern def,
+            ):
+                # This should pull the corresponding pattern def,
                 # Prioritize `filename:` and `paired_ext:` query selectory over
                 # `pattern:`
                 if selected_path_query not in [filename_prefix, paired_ext_prefix]:
                     selected_path_query = pattern_prefix
                     selected_path_format = path_format
             elif query.startswith(ext_prefix) and artifact_ext == (
                 "." + self.remove_prefix(query, ext_prefix).lstrip(".")
@@ -283,16 +284,16 @@
 
         mapping_meta = {
             "albumpath": util.displayable_path(album_path),
             "medianame_old": medianame_old,
             "medianame_new": medianame_new,
         }
 
-        # Include all normal Item fields
-        mapping_meta.update(beets_item)
+        # Include all normal Item fields, using the formatted values
+        mapping_meta.update(beets_item.formatted())
 
         return FiletoteMappingModel(**mapping_meta)
 
     def _collect_paired_artifacts(
         self, beets_item: "Item", source: str, destination: bytes
     ) -> None:
         """
```

### Comparing `beets_filetote-0.4.1/beetsplug/filetote_dataclasses.py` & `beets_filetote-0.4.2/beetsplug/filetote_dataclasses.py`

 * *Files identical despite different names*

### Comparing `beets_filetote-0.4.1/beetsplug/mapping_model.py` & `beets_filetote-0.4.2/beetsplug/mapping_model.py`

 * *Files identical despite different names*

### Comparing `beets_filetote-0.4.1/pyproject.toml` & `beets_filetote-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beets-filetote"
-version = "0.4.1"
+version = "0.4.2"
 description = "A beets plugin to copy/moves non-music extra files, attachments, and artifacts during the import process."
 authors = ["Gavin Tronset <gtronset@gmail.com>"]
 keywords = ["beets", "files", "artifacts", "extra"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "beetsplug"}]
 repository = "https://github.com/gtronset/beets-filetote"
```

### Comparing `beets_filetote-0.4.1/PKG-INFO` & `beets_filetote-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-filetote
-Version: 0.4.1
+Version: 0.4.2
 Summary: A beets plugin to copy/moves non-music extra files, attachments, and artifacts during the import process.
 Home-page: https://github.com/gtronset/beets-filetote
 License: MIT
 Keywords: beets,files,artifacts,extra
 Author: Gavin Tronset
 Author-email: gtronset@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -36,15 +36,15 @@
 [![MIT license][license image]][license link]
 [![CI][ci image]][ci link]
 [![GitHub release][github image]][github link]
 [![PyPI][pypi_version]][pypi_link]
 [![PyPI - Python Version][pypi_python_versions]][pypi_link]
 
 A plugin that moves non-music extra files, attachments, and artifacts during
-the import process for [beets](http://beets.radbox.org/), a music library
+the import process for [beets](https://beets.io/), a music library
 manager (and much more!).
 
 ## Installing
 
 ### Stable
 
 The stable version of the plugin is available from PyPI and can be installed
```

