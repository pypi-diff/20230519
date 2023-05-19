# Comparing `tmp/relative-addons-system-2.5.2.tar.gz` & `tmp/relative-addons-system-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative-addons-system-2.5.2.tar", last modified: Wed May 17 18:59:02 2023, max compression
+gzip compressed data, was "relative-addons-system-2.5.3.tar", last modified: Fri May 19 16:20:16 2023, max compression
```

## Comparing `relative-addons-system-2.5.2.tar` & `relative-addons-system-2.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 18:59:02.703450 relative-addons-system-2.5.2/
--rw-rw-rw-   0        0        0     1064 2022-10-11 13:46:50.000000 relative-addons-system-2.5.2/LICENSE
--rw-rw-rw-   0        0        0     5788 2023-05-17 18:59:02.702448 relative-addons-system-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     3851 2023-05-02 08:59:29.000000 relative-addons-system-2.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 18:59:02.616158 relative-addons-system-2.5.2/RelativeAddonsSystem/
--rw-rw-rw-   0        0        0      309 2023-05-17 18:58:06.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 18:59:02.632159 relative-addons-system-2.5.2/RelativeAddonsSystem/addon/
--rw-rw-rw-   0        0        0     5413 2023-05-17 18:58:06.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/addon/__init__.py
--rw-rw-rw-   0        0        0     1632 2023-05-02 08:26:45.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/addon/metadata.py
--rw-rw-rw-   0        0        0     1999 2023-05-17 18:40:17.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/libraries.py
--rw-rw-rw-   0        0        0    10612 2023-05-02 08:38:57.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/system.py
-drwxrwxrwx   0        0        0        0 2023-05-17 18:59:02.686687 relative-addons-system-2.5.2/RelativeAddonsSystem/utils/
--rw-rw-rw-   0        0        0      215 2023-04-16 16:56:05.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/utils/__init__.py
--rw-rw-rw-   0        0        0     2466 2023-05-02 08:33:45.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/utils/cache.py
--rw-rw-rw-   0        0        0      382 2022-10-25 18:37:38.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/utils/recursive_reload_module.py
--rw-rw-rw-   0        0        0     1629 2023-05-02 08:40:18.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/utils/storage.py
--rw-rw-rw-   0        0        0     1442 2022-05-31 14:24:28.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/utils/version_checker.py
--rw-rw-rw-   0        0        0      397 2023-05-02 08:06:08.000000 relative-addons-system-2.5.2/RelativeAddonsSystem/utils/version_transform.py
--rw-rw-rw-   0        0        0      764 2023-05-17 18:58:06.000000 relative-addons-system-2.5.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-17 18:59:02.699454 relative-addons-system-2.5.2/relative_addons_system.egg-info/
--rw-rw-rw-   0        0        0     5788 2023-05-17 18:59:02.000000 relative-addons-system-2.5.2/relative_addons_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-17 18:59:02.000000 relative-addons-system-2.5.2/relative_addons_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 18:59:02.000000 relative-addons-system-2.5.2/relative_addons_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 18:59:02.000000 relative-addons-system-2.5.2/relative_addons_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-17 18:59:02.000000 relative-addons-system-2.5.2/relative_addons_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 18:59:02.703450 relative-addons-system-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0      902 2022-11-08 14:20:04.000000 relative-addons-system-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:20:16.925054 relative-addons-system-2.5.3/
+-rw-rw-rw-   0        0        0     1064 2022-10-11 13:46:50.000000 relative-addons-system-2.5.3/LICENSE
+-rw-rw-rw-   0        0        0     5788 2023-05-19 16:20:16.923054 relative-addons-system-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3851 2023-05-02 08:59:29.000000 relative-addons-system-2.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 16:20:16.613209 relative-addons-system-2.5.3/RelativeAddonsSystem/
+-rw-rw-rw-   0        0        0      309 2023-05-19 16:18:55.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:20:16.638166 relative-addons-system-2.5.3/RelativeAddonsSystem/addon/
+-rw-rw-rw-   0        0        0     5113 2023-05-19 16:17:52.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/addon/__init__.py
+-rw-rw-rw-   0        0        0     1632 2023-05-02 08:26:45.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/addon/metadata.py
+-rw-rw-rw-   0        0        0     1999 2023-05-17 18:40:17.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/libraries.py
+-rw-rw-rw-   0        0        0    10612 2023-05-02 08:38:57.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/system.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:20:16.821629 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/
+-rw-rw-rw-   0        0        0      215 2023-04-16 16:56:05.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/__init__.py
+-rw-rw-rw-   0        0        0     2466 2023-05-02 08:33:45.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/cache.py
+-rw-rw-rw-   0        0        0      382 2022-10-25 18:37:38.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/recursive_reload_module.py
+-rw-rw-rw-   0        0        0     1629 2023-05-02 08:40:18.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/storage.py
+-rw-rw-rw-   0        0        0     1442 2022-05-31 14:24:28.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/version_checker.py
+-rw-rw-rw-   0        0        0      397 2023-05-02 08:06:08.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/version_transform.py
+-rw-rw-rw-   0        0        0      764 2023-05-19 16:18:55.000000 relative-addons-system-2.5.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-19 16:20:16.921054 relative-addons-system-2.5.3/relative_addons_system.egg-info/
+-rw-rw-rw-   0        0        0     5788 2023-05-19 16:20:16.000000 relative-addons-system-2.5.3/relative_addons_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-19 16:20:16.000000 relative-addons-system-2.5.3/relative_addons_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:20:16.000000 relative-addons-system-2.5.3/relative_addons_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-19 16:20:16.000000 relative-addons-system-2.5.3/relative_addons_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-19 16:20:16.000000 relative-addons-system-2.5.3/relative_addons_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 16:20:16.925054 relative-addons-system-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      902 2022-11-08 14:20:04.000000 relative-addons-system-2.5.3/setup.py
```

### Comparing `relative-addons-system-2.5.2/LICENSE` & `relative-addons-system-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.2/PKG-INFO` & `relative-addons-system-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relative-addons-system
-Version: 2.5.2
+Version: 2.5.3
 Summary: Easier way to manage your project addons
 Home-page: 
 Author: YoungTitanium
 Author-email: "kuyugama(youngtitanium)" <mail.kuyugama@gmail.com>
 License: Copyright 2022 kuyugama(youngtitanium)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `relative-addons-system-2.5.2/README.md` & `relative-addons-system-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.2/RelativeAddonsSystem/addon/__init__.py` & `relative-addons-system-2.5.3/RelativeAddonsSystem/addon/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import importlib
-import json
 import shutil
 import warnings
 from pathlib import Path
 
 from .metadata import AddonMeta
 from RelativeAddonsSystem import libraries, utils
 
@@ -41,33 +40,28 @@
             if not self.path / "addon.json":
                 raise MetadataError(
                     "Cannot find metadata file of addon at {path}".format(
                         path=self.path.absolute()
                     )
                 )
 
-            with open(self.path / "addon.json") as info:
-                self._meta = AddonMeta(**json.load(info))
+            self._meta = AddonMeta(self.path / "addon.json")
 
         return self._meta
 
     def __str__(self):
         return f"Addon(name={repr(self.meta.get('name', 'None'))}, path={repr(self.path.absolute())})"
 
     def enable(self):
-        self.meta["status"] = "enabled"
-
-        with open(self.path / "addon.json", "w", encoding="utf8") as f:
-            json.dump(self.meta, f, ensure_ascii=False, indent=4)
+        self.meta.status = "enabled"
+        self.meta.save()
 
     def disable(self):
-        self.meta["status"] = "disabled"
-
-        with open(self.path / "addon.json", "w", encoding="utf8") as f:
-            json.dump(self.meta, f, ensure_ascii=False, indent=4)
+        self.meta.status = "disabled"
+        self.meta.save()
 
     def remove(self):
         """
         **Removes addon**
         """
         shutil.rmtree(self.path)
         del self
```

### Comparing `relative-addons-system-2.5.2/RelativeAddonsSystem/addon/metadata.py` & `relative-addons-system-2.5.3/RelativeAddonsSystem/addon/metadata.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.2/RelativeAddonsSystem/libraries.py` & `relative-addons-system-2.5.3/RelativeAddonsSystem/libraries.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.2/RelativeAddonsSystem/system.py` & `relative-addons-system-2.5.3/RelativeAddonsSystem/system.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.2/RelativeAddonsSystem/utils/cache.py` & `relative-addons-system-2.5.3/RelativeAddonsSystem/utils/cache.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.2/RelativeAddonsSystem/utils/storage.py` & `relative-addons-system-2.5.3/RelativeAddonsSystem/utils/storage.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.2/RelativeAddonsSystem/utils/version_checker.py` & `relative-addons-system-2.5.3/RelativeAddonsSystem/utils/version_checker.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.2/pyproject.toml` & `relative-addons-system-2.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative-addons-system"
-version = "2.5.2"
+version = "2.5.3"
 description = "Easier way to manage your project addons"
 authors = [{ name = "kuyugama(youngtitanium)", email = "mail.kuyugama@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `relative-addons-system-2.5.2/relative_addons_system.egg-info/PKG-INFO` & `relative-addons-system-2.5.3/relative_addons_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relative-addons-system
-Version: 2.5.2
+Version: 2.5.3
 Summary: Easier way to manage your project addons
 Home-page: 
 Author: YoungTitanium
 Author-email: "kuyugama(youngtitanium)" <mail.kuyugama@gmail.com>
 License: Copyright 2022 kuyugama(youngtitanium)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `relative-addons-system-2.5.2/relative_addons_system.egg-info/SOURCES.txt` & `relative-addons-system-2.5.3/relative_addons_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.2/setup.py` & `relative-addons-system-2.5.3/setup.py`

 * *Files identical despite different names*

