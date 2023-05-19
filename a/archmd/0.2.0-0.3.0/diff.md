# Comparing `tmp/archmd-0.2.0.tar.gz` & `tmp/archmd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archmd-0.2.0.tar", last modified: Wed May 26 10:33:17 2021, max compression
+gzip compressed data, was "archmd-0.3.0.tar", max compression
```

## Comparing `archmd-0.2.0.tar` & `archmd-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2021-05-26 10:31:53.469897 archmd-0.2.0/LICENSE
--rw-r--r--   0        0        0     4060 2021-05-26 10:32:20.423713 archmd-0.2.0/archmd/__init__.py
--rw-r--r--   0        0        0      477 2021-05-26 10:32:44.149953 archmd-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      738 2021-05-26 10:33:17.917196 archmd-0.2.0/setup.py
--rw-r--r--   0        0        0      340 2021-05-26 10:33:17.917323 archmd-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-19 09:44:25.697088 archmd-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5770 2023-05-19 10:45:42.494512 archmd-0.3.0/archmd/__init__.py
+-rw-r--r--   0        0        0      447 2023-05-19 10:45:10.292670 archmd-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 archmd-0.3.0/setup.py
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 archmd-0.3.0/PKG-INFO
```

### Comparing `archmd-0.2.0/LICENSE` & `archmd-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `archmd-0.2.0/setup.py` & `archmd-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['archmd']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['typer>=0.3.2,<0.4.0']
+['typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['archmd = archmd:app']}
 
 setup_kwargs = {
     'name': 'archmd',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'A simple command line utility to build an architecture.md file',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Joel Collins',
     'author_email': 'pypi@jtcollins.net',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

