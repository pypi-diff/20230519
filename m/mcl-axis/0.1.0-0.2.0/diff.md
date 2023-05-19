# Comparing `tmp/mcl-axis-0.1.0.tar.gz` & `tmp/mcl-axis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcl-axis-0.1.0.tar", last modified: Thu May 18 07:15:07 2023, max compression
+gzip compressed data, was "mcl-axis-0.2.0.tar", last modified: Fri May 19 12:53:50 2023, max compression
```

## Comparing `mcl-axis-0.1.0.tar` & `mcl-axis-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 07:15:07.363801 mcl-axis-0.1.0/
--rw-rw-rw-   0        0        0     1080 2023-05-17 13:43:07.000000 mcl-axis-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      461 2023-05-18 07:15:07.361756 mcl-axis-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-05-17 13:45:22.000000 mcl-axis-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 07:15:07.336273 mcl-axis-0.1.0/mcl/
--rw-rw-rw-   0        0        0       27 2023-05-18 07:13:27.000000 mcl-axis-0.1.0/mcl/__init__.py
--rw-rw-rw-   0        0        0       69 2023-05-18 07:13:28.000000 mcl-axis-0.1.0/mcl/__main__.py
--rw-rw-rw-   0        0        0     2391 2023-05-18 06:39:31.000000 mcl-axis-0.1.0/mcl/core.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:15:07.359239 mcl-axis-0.1.0/mcl_axis.egg-info/
--rw-rw-rw-   0        0        0      461 2023-05-18 07:15:07.000000 mcl-axis-0.1.0/mcl_axis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-18 07:15:07.000000 mcl-axis-0.1.0/mcl_axis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 07:15:07.000000 mcl-axis-0.1.0/mcl_axis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-18 07:15:07.000000 mcl-axis-0.1.0/mcl_axis.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2023-05-18 07:15:07.000000 mcl-axis-0.1.0/mcl_axis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-18 07:15:07.000000 mcl-axis-0.1.0/mcl_axis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 07:15:07.364764 mcl-axis-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-05-18 07:14:45.000000 mcl-axis-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:53:50.579971 mcl-axis-0.2.0/
+-rw-rw-rw-   0        0        0     1080 2023-05-17 13:43:07.000000 mcl-axis-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      461 2023-05-19 12:53:50.572273 mcl-axis-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-05-18 12:17:58.000000 mcl-axis-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 12:53:50.548834 mcl-axis-0.2.0/mcl/
+-rw-rw-rw-   0        0        0       27 2023-05-18 07:13:27.000000 mcl-axis-0.2.0/mcl/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-05-18 07:13:28.000000 mcl-axis-0.2.0/mcl/__main__.py
+-rw-rw-rw-   0        0        0     2518 2023-05-19 09:13:24.000000 mcl-axis-0.2.0/mcl/core.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:53:50.572273 mcl-axis-0.2.0/mcl_axis.egg-info/
+-rw-rw-rw-   0        0        0      461 2023-05-19 12:53:50.000000 mcl-axis-0.2.0/mcl_axis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-19 12:53:50.000000 mcl-axis-0.2.0/mcl_axis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 12:53:50.000000 mcl-axis-0.2.0/mcl_axis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-19 12:53:50.000000 mcl-axis-0.2.0/mcl_axis.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2023-05-19 12:53:50.000000 mcl-axis-0.2.0/mcl_axis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-19 12:53:50.000000 mcl-axis-0.2.0/mcl_axis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 12:53:50.579971 mcl-axis-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-05-19 12:52:46.000000 mcl-axis-0.2.0/setup.py
```

### Comparing `mcl-axis-0.1.0/LICENSE` & `mcl-axis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcl-axis-0.1.0/mcl/core.py` & `mcl-axis-0.2.0/mcl/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import click
 import libcst as cst
 import tabulate
 from libcst._nodes.statement import ImportFrom
 
 
 class Visitor(cst.CSTVisitor):
-    def __init__(self, files: list[str]) -> None:
+    def __init__(self, user_defined_modules: set[str]) -> None:
         super().__init__()
-        self.files = files
+        self.user_defined_modules = user_defined_modules
         self.count = {}
 
     def recursive_value(self, node) -> str:
         if isinstance(node, str):
             return node
         return self.recursive_value(node.value)
 
@@ -22,26 +22,27 @@
         if package not in self.count:
             self.count[package] = 0
 
         self.count[package] += 1
 
     def visit_Import(self, node: cst.CSTNode):
         for alias in node.names:
-            if alias.name.value in self.files:
+            package = self.recursive_value(alias.name.value)
+            if package in self.user_defined_modules:
                 continue
 
-            package = self.recursive_value(alias.name.value)
             self.gain_count(package)
 
     def visit_ImportFrom(self, node: ImportFrom) -> bool | None:
         if not hasattr(node.module, "value"):
             return
-        if node.module.value in self.files:
-            return
         package = self.recursive_value(node.module.value)
+
+        if package in self.user_defined_modules:
+            return
         self.gain_count(package)
 
 
 def is_ignored_folder(path, ignored_folders):
     return any(folder in path.parts for folder in ignored_folders)
 
 
@@ -60,23 +61,26 @@
     current_directory = Path()
     ignored_folders = get_ignored_folders()
     files = [
         file
         for file in current_directory.rglob("*.py")
         if not is_ignored_folder(file, ignored_folders)
     ]
-    package_modules = [
-        file.parent for file in files if file.name in ("__main__.py", "__init__.py")
-    ]
+    user_defined_modules = {
+        str(file.parent.stem)
+        for file in files
+        if file.name in ("__main__.py", "__init__.py")
+    }
+    user_defined_modules.update({file.stem for file in files})
     counter = Counter()
     for file in files:
         try:
             node = cst.parse_module(file.read_text())
         except UnicodeDecodeError:
             continue
-        visitor = Visitor([file.stem for file in files] + package_modules)
+        visitor = Visitor(user_defined_modules)
         node.visit(visitor)
         counter.update(visitor.count)
 
     items = [(key, value) for key, value in counter.items()]
     items.sort(key=lambda x: x[1], reverse=True)
     print(tabulate.tabulate(items, ("packages", "count")))
```

### Comparing `mcl-axis-0.1.0/setup.py` & `mcl-axis-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # py -m build
 # twine upload dist/*
-VERSION = "0.1.0"
+VERSION = "0.2.0"
 DESCRIPTION = "A tool to find the most common libraries used"
 LONG_DESCRIPTION = """
 A tool to find the most commonly imported
 python libraries in a target directory 
 """
 
 # Setup
```

