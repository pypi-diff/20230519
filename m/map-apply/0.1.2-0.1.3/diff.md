# Comparing `tmp/map_apply-0.1.2.tar.gz` & `tmp/map_apply-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "map_apply-0.1.2.tar", max compression
+gzip compressed data, was "map_apply-0.1.3.tar", max compression
```

## Comparing `map_apply-0.1.2.tar` & `map_apply-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       74 2023-05-16 12:45:26.000000 map_apply-0.1.2/map_apply/__init__.py
--rw-r--r--   0        0        0      981 2023-05-16 11:14:46.000000 map_apply-0.1.2/map_apply/cli.py
--rw-r--r--   0        0        0      344 2023-05-17 10:39:02.000000 map_apply-0.1.2/map_apply/file_handler.py
--rw-r--r--   0        0        0     2415 2023-05-17 17:14:18.000000 map_apply-0.1.2/map_apply/main.py
--rw-r--r--   0        0        0        0 2023-05-16 11:04:18.000000 map_apply-0.1.2/map_apply/scripts/__init__.py
--rw-r--r--   0        0        0      338 2023-05-16 12:04:50.000000 map_apply-0.1.2/map_apply/scripts/map_apply.py
--rw-r--r--   0        0        0      524 2023-05-17 17:15:56.000000 map_apply-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      796 2023-05-17 17:16:26.227795 map_apply-0.1.2/setup.py
--rw-r--r--   0        0        0      446 2023-05-17 17:16:26.227795 map_apply-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-05-16 12:45:26.000000 map_apply-0.1.3/map_apply/__init__.py
+-rw-r--r--   0        0        0     1177 2023-05-19 12:37:36.000000 map_apply-0.1.3/map_apply/cli.py
+-rw-r--r--   0        0        0       13 2023-05-19 12:37:36.000000 map_apply-0.1.3/map_apply/consts.py
+-rw-r--r--   0        0        0      464 2023-05-19 12:26:46.000000 map_apply-0.1.3/map_apply/file_handler.py
+-rw-r--r--   0        0        0     2704 2023-05-19 12:38:16.000000 map_apply-0.1.3/map_apply/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:04:18.000000 map_apply-0.1.3/map_apply/scripts/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-16 12:04:50.000000 map_apply-0.1.3/map_apply/scripts/map_apply.py
+-rw-r--r--   0        0        0      524 2023-05-19 12:39:50.000000 map_apply-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      796 2023-05-19 12:41:49.717206 map_apply-0.1.3/setup.py
+-rw-r--r--   0        0        0      446 2023-05-19 12:41:49.717206 map_apply-0.1.3/PKG-INFO
```

### Comparing `map_apply-0.1.2/map_apply/cli.py` & `map_apply-0.1.3/map_apply/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 
     parser.add_argument('-i', '--input', help='Input file to be handled')
     parser.add_argument('-m',
                         '--map',
                         help='File with 2 rows of values. '
                              'the first row values will be '
                              'substituted with the 2nd row')
+    parser.add_argument('-o',
+                        '--out',
+                        help='Output filename. Defaults with .out extension '
+                             'if not specified')
+
     parser.add_argument('-s', '--separator', help='Map file separator. '
                                                   'Tabulation is the default',
                         default='\t')
 
     args = parser.parse_args()
 
     return args
```

### Comparing `map_apply-0.1.2/map_apply/main.py` & `map_apply-0.1.3/map_apply/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Main module to perform mapping"""
 
-from map_apply.file_handler import open_file_if_exists
+from map_apply.file_handler import open_file_if_exists, get_file_format
 
 
 def clean_data(f, separator):
     """  splits, removes emptiness, new lines and BOM signature """
     lines = []
     for line_number, line in enumerate(f):
 
@@ -25,16 +25,25 @@
     # mapping - is a list of lists w/ 2 values
     # we need to find a line with the [0] that equals to search
     for number, line in enumerate(mapping):
         if line[0] == search:
             return line[1], number
     return None, None
 
+# def get_new_filename(source_filename):
+#
+#     if get_file_format(source_filename).upper() == CSV.upper():
+#
+#     else:
+#         raise
+#
+#
 
-def apply_map(source_file, new_file, mapping, separator):
+
+def apply_map(source_file, new_file, mapping, separator, out_file):
 
     # ROADMAP
     # Sort the source data file
     # improve the replacement search algorithm
 
     for line_number, line in enumerate(source_file):
 
@@ -61,25 +70,29 @@
             li[-1] = f'{li[-1][:-2]}\n'  # removes the last tabulation
 
             new_file.writelines(
                 li
             )
 
 
-def map_apply(input_file, map_file, separator):
+def map_apply(input_file, map_file, separator, out_file):
+
+    if not out_file:
+        out_file = f'{input_file}.out'
 
     # read the map and sort it
     with open_file_if_exists(map_file) as mf:  # fm - map_file
         sorted_map = sorted(
             clean_data(mf, separator),
             key=lambda x: x[0]
         )
 
     # creating a new file
-    with open(f'{input_file}.feed', mode='w+', encoding='utf-8') as nf:  # nf - new file
+    with open(f'{out_file}', mode='w+', encoding='utf-8') as nf:  # nf - new file
         with open_file_if_exists(input_file) as inf:  # inf - input_file
             apply_map(source_file=inf,
                       new_file=nf,
                       mapping=sorted_map,
-                      separator=separator)
+                      separator=separator,
+                      out_file=out_file)
 
     return True
```

### Comparing `map_apply-0.1.2/pyproject.toml` & `map_apply-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "map_apply"
-version = "0.1.2"
+version = "0.1.3"
 description = "Copies the input file and substitute one keyfield with another using 'map' file"
 authors = ["Smirnov Sergey"]
 license = "MIT"
 packages = [{include="map_apply"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `map_apply-0.1.2/setup.py` & `map_apply-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['argparse>=1.4.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['map_apply = map_apply.scripts.map_apply:main']}
 
 setup_kwargs = {
     'name': 'map-apply',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': "Copies the input file and substitute one keyfield with another using 'map' file",
     'long_description': None,
     'author': 'Smirnov Sergey',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

