# Comparing `tmp/map_apply-0.1.3.tar.gz` & `tmp/map_apply-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "map_apply-0.1.3.tar", max compression
+gzip compressed data, was "map_apply-0.1.5.tar", max compression
```

## Comparing `map_apply-0.1.3.tar` & `map_apply-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       74 2023-05-16 12:45:26.000000 map_apply-0.1.3/map_apply/__init__.py
--rw-r--r--   0        0        0     1177 2023-05-19 12:37:36.000000 map_apply-0.1.3/map_apply/cli.py
--rw-r--r--   0        0        0       13 2023-05-19 12:37:36.000000 map_apply-0.1.3/map_apply/consts.py
--rw-r--r--   0        0        0      464 2023-05-19 12:26:46.000000 map_apply-0.1.3/map_apply/file_handler.py
--rw-r--r--   0        0        0     2704 2023-05-19 12:38:16.000000 map_apply-0.1.3/map_apply/main.py
--rw-r--r--   0        0        0        0 2023-05-16 11:04:18.000000 map_apply-0.1.3/map_apply/scripts/__init__.py
--rw-r--r--   0        0        0      338 2023-05-16 12:04:50.000000 map_apply-0.1.3/map_apply/scripts/map_apply.py
--rw-r--r--   0        0        0      524 2023-05-19 12:39:50.000000 map_apply-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      796 2023-05-19 12:41:49.717206 map_apply-0.1.3/setup.py
--rw-r--r--   0        0        0      446 2023-05-19 12:41:49.717206 map_apply-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-05-16 12:45:26.000000 map_apply-0.1.5/map_apply/__init__.py
+-rw-r--r--   0        0        0     1177 2023-05-19 12:37:36.000000 map_apply-0.1.5/map_apply/cli.py
+-rw-r--r--   0        0        0       13 2023-05-19 12:37:36.000000 map_apply-0.1.5/map_apply/consts.py
+-rw-r--r--   0        0        0      464 2023-05-19 12:26:46.000000 map_apply-0.1.5/map_apply/file_handler.py
+-rw-r--r--   0        0        0     2652 2023-05-19 12:56:38.000000 map_apply-0.1.5/map_apply/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:04:18.000000 map_apply-0.1.5/map_apply/scripts/__init__.py
+-rw-r--r--   0        0        0      375 2023-05-19 13:10:40.000000 map_apply-0.1.5/map_apply/scripts/map_apply.py
+-rw-r--r--   0        0        0      524 2023-05-19 13:11:54.000000 map_apply-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      796 2023-05-19 13:12:11.845655 map_apply-0.1.5/setup.py
+-rw-r--r--   0        0        0      446 2023-05-19 13:12:11.845655 map_apply-0.1.5/PKG-INFO
```

### Comparing `map_apply-0.1.3/map_apply/cli.py` & `map_apply-0.1.5/map_apply/cli.py`

 * *Files identical despite different names*

### Comparing `map_apply-0.1.3/map_apply/main.py` & `map_apply-0.1.5/map_apply/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 #
 #     else:
 #         raise
 #
 #
 
 
-def apply_map(source_file, new_file, mapping, separator, out_file):
+def apply_map(source_file, new_file, mapping, separator):
 
     # ROADMAP
     # Sort the source data file
     # improve the replacement search algorithm
 
     for line_number, line in enumerate(source_file):
 
@@ -88,11 +88,10 @@
 
     # creating a new file
     with open(f'{out_file}', mode='w+', encoding='utf-8') as nf:  # nf - new file
         with open_file_if_exists(input_file) as inf:  # inf - input_file
             apply_map(source_file=inf,
                       new_file=nf,
                       mapping=sorted_map,
-                      separator=separator,
-                      out_file=out_file)
+                      separator=separator)
 
     return True
```

### Comparing `map_apply-0.1.3/pyproject.toml` & `map_apply-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "map_apply"
-version = "0.1.3"
+version = "0.1.5"
 description = "Copies the input file and substitute one keyfield with another using 'map' file"
 authors = ["Smirnov Sergey"]
 license = "MIT"
 packages = [{include="map_apply"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `map_apply-0.1.3/setup.py` & `map_apply-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['argparse>=1.4.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['map_apply = map_apply.scripts.map_apply:main']}
 
 setup_kwargs = {
     'name': 'map-apply',
-    'version': '0.1.3',
+    'version': '0.1.5',
     'description': "Copies the input file and substitute one keyfield with another using 'map' file",
     'long_description': None,
     'author': 'Smirnov Sergey',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

