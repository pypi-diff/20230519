# Comparing `tmp/atlas-framework-0.1.3.tar.gz` & `tmp/atlas-framework-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-framework-0.1.3.tar", last modified: Tue May 16 19:18:10 2023, max compression
+gzip compressed data, was "atlas-framework-0.1.5.tar", last modified: Fri May 19 20:15:42 2023, max compression
```

## Comparing `atlas-framework-0.1.3.tar` & `atlas-framework-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.583477 atlas-framework-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/src/atlas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/src/atlas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/src/atlas/app/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/src/atlas/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/src/atlas/app/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/src/atlas/app/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/src/atlas/context/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/src/atlas/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/src/atlas_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-16 19:18:10.000000 atlas-framework-0.1.3/src/atlas_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-16 19:18:10.000000 atlas-framework-0.1.3/src/atlas_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:18:10.000000 atlas-framework-0.1.3/src/atlas_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 19:18:10.000000 atlas-framework-0.1.3/src/atlas_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 19:18:10.000000 atlas-framework-0.1.3/src/atlas_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.251253 atlas-framework-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-19 20:15:42.251253 atlas-framework-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:15:42.251253 atlas-framework-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.247253 atlas-framework-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.247253 atlas-framework-0.1.5/src/atlas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/src/atlas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.247253 atlas-framework-0.1.5/src/atlas/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/src/atlas/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/src/atlas/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/src/atlas/app/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.247253 atlas-framework-0.1.5/src/atlas/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/src/atlas/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.251253 atlas-framework-0.1.5/src/atlas_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-19 20:15:42.000000 atlas-framework-0.1.5/src/atlas_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-19 20:15:42.000000 atlas-framework-0.1.5/src/atlas_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:15:42.000000 atlas-framework-0.1.5/src/atlas_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-19 20:15:42.000000 atlas-framework-0.1.5/src/atlas_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 20:15:42.000000 atlas-framework-0.1.5/src/atlas_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.251253 atlas-framework-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/tests/test_context.py
```

### Comparing `atlas-framework-0.1.3/LICENSE` & `atlas-framework-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atlas-framework-0.1.3/pyproject.toml` & `atlas-framework-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
+requires = ["setuptools>=62.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [project]
 name = "atlas-framework"
-version = "0.1.3"
+version = "0.1.5"
 authors = [
   { name="Grant Viklund", email="renderbox@gmail.com" },
 ]
 description = "Class-based famework for quickly creating robust Python apps."
 readme = "README.md"
-requires-python = ">=3.8,<3.12"
+requires-python = ">=3.7,<3.12"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -39,14 +39,17 @@
 ]
 test = [
     "coverage",
     "pytest"
 ]
 docs = [
     "coverage",
+    "mkdocs",
+    "mkdocs-material",
+    "mkdocstrings[python]",
 ]
 pyside2 = [
     "PySide2",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/renderbox/atlas-framework"
```

### Comparing `atlas-framework-0.1.3/src/atlas/app/base.py` & `atlas-framework-0.1.5/src/atlas/app/base.py`

 * *Files identical despite different names*

### Comparing `atlas-framework-0.1.3/src/atlas/app/gui.py` & `atlas-framework-0.1.5/src/atlas/app/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,30 +69,38 @@
             )
 
             # Load the UI file
             uifile = QFile(gui_path)
             uifile.open(QFile.ReadOnly)
             loader = QUiLoader()
 
-            # Attach the loaded results to the window variable
-            self.window = loader.load(uifile)
+            try:
+                # Attach the loaded results to the window variable
+                self.window = loader.load(uifile)
+            except RuntimeError as e:
+                print(
+                    "Could not load the file: {}\nOne is needed to use a PySide2 GUI based app.".format(
+                        gui_path
+                    )
+                )
+                print(e)
 
             uifile.close()
 
-        self.connect_signals_and_slots()
-
-        self.window.show()
-        sys.exit(self.app.exec_())
-
     def connect_signals_and_slots(self):
         """Step that will connect signals and slots from the UI file to code"""
         pass
 
     def run_gui(self, ctx):
         """
         Evaluated when in GUI mode.  By default just loads the GUI.
         Can be overridden to do other things when loading a GUI.
 
         Args:
             ctx (Context): Context to execute the tool with
         """
         self.load_gui()
+
+        self.connect_signals_and_slots()
+
+        self.window.show()
+        sys.exit(self.app.exec_())
```

### Comparing `atlas-framework-0.1.3/src/atlas/context/__init__.py` & `atlas-framework-0.1.5/src/atlas/context/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas-framework-0.1.3/tests/test_context.py` & `atlas-framework-0.1.5/tests/test_context.py`

 * *Files identical despite different names*

