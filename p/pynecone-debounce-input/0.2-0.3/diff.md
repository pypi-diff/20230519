# Comparing `tmp/pynecone-debounce-input-0.2.tar.gz` & `tmp/pynecone-debounce-input-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-debounce-input-0.2.tar", last modified: Mon Apr 24 18:31:26 2023, max compression
+gzip compressed data, was "pynecone-debounce-input-0.3.tar", last modified: Fri May 19 15:18:51 2023, max compression
```

## Comparing `pynecone-debounce-input-0.2.tar` & `pynecone-debounce-input-0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.433489 pynecone-debounce-input-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-24 18:31:26.433489 pynecone-debounce-input-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/example/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/example/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/example/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/pcconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:31:26.433489 pynecone-debounce-input-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.433489 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-24 18:31:26.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-24 18:31:26.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:31:26.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 18:31:26.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 18:31:26.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.433489 pynecone-debounce-input-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:18:51.495571 pynecone-debounce-input-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:18:51.483571 pynecone-debounce-input-0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:18:51.491571 pynecone-debounce-input-0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-19 15:18:51.495571 pynecone-debounce-input-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:18:51.491571 pynecone-debounce-input-0.3/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/example/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:18:51.491571 pynecone-debounce-input-0.3/example/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/example/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:18:51.491571 pynecone-debounce-input-0.3/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/example/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/example/pcconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:18:51.495571 pynecone-debounce-input-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:18:51.491571 pynecone-debounce-input-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:18:51.495571 pynecone-debounce-input-0.3/src/pynecone_debounce_input.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-19 15:18:51.000000 pynecone-debounce-input-0.3/src/pynecone_debounce_input.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-19 15:18:51.000000 pynecone-debounce-input-0.3/src/pynecone_debounce_input.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:18:51.000000 pynecone-debounce-input-0.3/src/pynecone_debounce_input.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 15:18:51.000000 pynecone-debounce-input-0.3/src/pynecone_debounce_input.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 15:18:51.000000 pynecone-debounce-input-0.3/src/pynecone_debounce_input.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/src/pynecone_debounce_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:18:51.495571 pynecone-debounce-input-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-19 15:18:10.000000 pynecone-debounce-input-0.3/tox.ini
```

### Comparing `pynecone-debounce-input-0.2/.github/workflows/publish.yml` & `pynecone-debounce-input-0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.2/.github/workflows/test.yml` & `pynecone-debounce-input-0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.2/LICENSE` & `pynecone-debounce-input-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.2/PKG-INFO` & `pynecone-debounce-input-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone-debounce-input
-Version: 0.2
+Version: 0.3
 Summary: Pynecone full-stack framework wrapper around react-debounce-input
 Author-email: Masen Furer <m_github@0x26.net>
 License: MIT License
         
         Copyright (c) 2023 Masen Furer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -132,14 +132,18 @@
 
 #### `force_notify_on_blur: bool = True`
 
 Same as `force_notify_by_enter`, but notification will be sent when focus leaves the input field.
 
 ## Changelog
 
+### v0.3 - 2023-05-19
+
+* Support pynecone >= 0.1.30 (`pynecone.var` changed to `pynecone.vars`)
+
 ### v0.2 - 2023-04-24
 
 * `import pynecone_debounce_input` automatically adds `react-debounce-input` to `Config.frontend_packages`
 * fix example in README, missing comma
 * improve test assertions when exporting example project
 
 ### v0.1 - 2023-04-21
```

### Comparing `pynecone-debounce-input-0.2/README.md` & `pynecone-debounce-input-0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,18 @@
 
 #### `force_notify_on_blur: bool = True`
 
 Same as `force_notify_by_enter`, but notification will be sent when focus leaves the input field.
 
 ## Changelog
 
+### v0.3 - 2023-05-19
+
+* Support pynecone >= 0.1.30 (`pynecone.var` changed to `pynecone.vars`)
+
 ### v0.2 - 2023-04-24
 
 * `import pynecone_debounce_input` automatically adds `react-debounce-input` to `Config.frontend_packages`
 * fix example in README, missing comma
 * improve test assertions when exporting example project
 
 ### v0.1 - 2023-04-21
```

### Comparing `pynecone-debounce-input-0.2/example/assets/favicon.ico` & `pynecone-debounce-input-0.3/example/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.2/example/example/example.py` & `pynecone-debounce-input-0.3/example/example/example.py`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.2/pyproject.toml` & `pynecone-debounce-input-0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     'Topic :: Software Development :: Libraries',
     'Topic :: Utilities',
     # 'Programming Language :: Javascript',
     'Programming Language :: Python',
 ]
 dynamic = ["version", "readme"]
 dependencies = [
-    'pynecone ~= 0.1.24',
+    'pynecone ~= 0.1.30',
 ]
 
 [project.urls]
 Homepage = "https://github.com/trivial-intelligence/pynecone-debounce-input"
 
 [tool.setuptools]
 platforms = ['unix', 'linux', 'osx', 'cygwin', 'win32']
```

### Comparing `pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/PKG-INFO` & `pynecone-debounce-input-0.3/src/pynecone_debounce_input.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone-debounce-input
-Version: 0.2
+Version: 0.3
 Summary: Pynecone full-stack framework wrapper around react-debounce-input
 Author-email: Masen Furer <m_github@0x26.net>
 License: MIT License
         
         Copyright (c) 2023 Masen Furer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -132,14 +132,18 @@
 
 #### `force_notify_on_blur: bool = True`
 
 Same as `force_notify_by_enter`, but notification will be sent when focus leaves the input field.
 
 ## Changelog
 
+### v0.3 - 2023-05-19
+
+* Support pynecone >= 0.1.30 (`pynecone.var` changed to `pynecone.vars`)
+
 ### v0.2 - 2023-04-24
 
 * `import pynecone_debounce_input` automatically adds `react-debounce-input` to `Config.frontend_packages`
 * fix example in README, missing comma
 * improve test assertions when exporting example project
 
 ### v0.1 - 2023-04-21
```

### Comparing `pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/SOURCES.txt` & `pynecone-debounce-input-0.3/src/pynecone_debounce_input.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.2/src/pynecone_debounce_input.py` & `pynecone-debounce-input-0.3/src/pynecone_debounce_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Any
 
 import pynecone as pc
 
 from pynecone.components.tags import Tag
-from pynecone.var import Var
+from pynecone.vars import Var
 
 
 class DebounceInput(pc.Component):
     library = "react-debounce-input"
     tag = "DebounceInput"
     min_length: Var[int] = 0
     debounce_timeout: Var[int] = 100
```

### Comparing `pynecone-debounce-input-0.2/tests/test_export.py` & `pynecone-debounce-input-0.3/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.2/tests/test_render.py` & `pynecone-debounce-input-0.3/tests/test_render.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 import pynecone as pc
-from pynecone.var import BaseVar
+from pynecone.vars import BaseVar
 
 from pynecone_debounce_input import debounce_input
 
 
 def test_render_no_child():
     with pytest.raises(RuntimeError):
         _ = debounce_input().render()
```

### Comparing `pynecone-debounce-input-0.2/tox.ini` & `pynecone-debounce-input-0.3/tox.ini`

 * *Files identical despite different names*

