# Comparing `tmp/relative-addons-system-2.5.3.tar.gz` & `tmp/relative-addons-system-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative-addons-system-2.5.3.tar", last modified: Fri May 19 16:20:16 2023, max compression
+gzip compressed data, was "relative-addons-system-2.5.4.tar", last modified: Fri May 19 16:35:53 2023, max compression
```

## Comparing `relative-addons-system-2.5.3.tar` & `relative-addons-system-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:20:16.925054 relative-addons-system-2.5.3/
--rw-rw-rw-   0        0        0     1064 2022-10-11 13:46:50.000000 relative-addons-system-2.5.3/LICENSE
--rw-rw-rw-   0        0        0     5788 2023-05-19 16:20:16.923054 relative-addons-system-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     3851 2023-05-02 08:59:29.000000 relative-addons-system-2.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 16:20:16.613209 relative-addons-system-2.5.3/RelativeAddonsSystem/
--rw-rw-rw-   0        0        0      309 2023-05-19 16:18:55.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:20:16.638166 relative-addons-system-2.5.3/RelativeAddonsSystem/addon/
--rw-rw-rw-   0        0        0     5113 2023-05-19 16:17:52.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/addon/__init__.py
--rw-rw-rw-   0        0        0     1632 2023-05-02 08:26:45.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/addon/metadata.py
--rw-rw-rw-   0        0        0     1999 2023-05-17 18:40:17.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/libraries.py
--rw-rw-rw-   0        0        0    10612 2023-05-02 08:38:57.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/system.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:20:16.821629 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/
--rw-rw-rw-   0        0        0      215 2023-04-16 16:56:05.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/__init__.py
--rw-rw-rw-   0        0        0     2466 2023-05-02 08:33:45.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/cache.py
--rw-rw-rw-   0        0        0      382 2022-10-25 18:37:38.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/recursive_reload_module.py
--rw-rw-rw-   0        0        0     1629 2023-05-02 08:40:18.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/storage.py
--rw-rw-rw-   0        0        0     1442 2022-05-31 14:24:28.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/version_checker.py
--rw-rw-rw-   0        0        0      397 2023-05-02 08:06:08.000000 relative-addons-system-2.5.3/RelativeAddonsSystem/utils/version_transform.py
--rw-rw-rw-   0        0        0      764 2023-05-19 16:18:55.000000 relative-addons-system-2.5.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-19 16:20:16.921054 relative-addons-system-2.5.3/relative_addons_system.egg-info/
--rw-rw-rw-   0        0        0     5788 2023-05-19 16:20:16.000000 relative-addons-system-2.5.3/relative_addons_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-19 16:20:16.000000 relative-addons-system-2.5.3/relative_addons_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:20:16.000000 relative-addons-system-2.5.3/relative_addons_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-19 16:20:16.000000 relative-addons-system-2.5.3/relative_addons_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-19 16:20:16.000000 relative-addons-system-2.5.3/relative_addons_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 16:20:16.925054 relative-addons-system-2.5.3/setup.cfg
--rw-rw-rw-   0        0        0      902 2022-11-08 14:20:04.000000 relative-addons-system-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:35:53.528545 relative-addons-system-2.5.4/
+-rw-rw-rw-   0        0        0     1064 2022-10-11 13:46:50.000000 relative-addons-system-2.5.4/LICENSE
+-rw-rw-rw-   0        0        0     5788 2023-05-19 16:35:53.526542 relative-addons-system-2.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3851 2023-05-02 08:59:29.000000 relative-addons-system-2.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 16:35:53.463543 relative-addons-system-2.5.4/RelativeAddonsSystem/
+-rw-rw-rw-   0        0        0      309 2023-05-19 16:30:37.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:35:53.472546 relative-addons-system-2.5.4/RelativeAddonsSystem/addon/
+-rw-rw-rw-   0        0        0     5328 2023-05-19 16:29:43.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/addon/__init__.py
+-rw-rw-rw-   0        0        0     1632 2023-05-02 08:26:45.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/addon/metadata.py
+-rw-rw-rw-   0        0        0     1999 2023-05-17 18:40:17.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/libraries.py
+-rw-rw-rw-   0        0        0    10612 2023-05-02 08:38:57.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/system.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:35:53.505546 relative-addons-system-2.5.4/RelativeAddonsSystem/utils/
+-rw-rw-rw-   0        0        0      215 2023-04-16 16:56:05.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/utils/__init__.py
+-rw-rw-rw-   0        0        0     2466 2023-05-02 08:33:45.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/utils/cache.py
+-rw-rw-rw-   0        0        0      382 2022-10-25 18:37:38.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/utils/recursive_reload_module.py
+-rw-rw-rw-   0        0        0     1629 2023-05-02 08:40:18.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/utils/storage.py
+-rw-rw-rw-   0        0        0     1442 2022-05-31 14:24:28.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/utils/version_checker.py
+-rw-rw-rw-   0        0        0      397 2023-05-02 08:06:08.000000 relative-addons-system-2.5.4/RelativeAddonsSystem/utils/version_transform.py
+-rw-rw-rw-   0        0        0      764 2023-05-19 16:34:54.000000 relative-addons-system-2.5.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-19 16:35:53.524541 relative-addons-system-2.5.4/relative_addons_system.egg-info/
+-rw-rw-rw-   0        0        0     5788 2023-05-19 16:35:53.000000 relative-addons-system-2.5.4/relative_addons_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-19 16:35:53.000000 relative-addons-system-2.5.4/relative_addons_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:35:53.000000 relative-addons-system-2.5.4/relative_addons_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-19 16:35:53.000000 relative-addons-system-2.5.4/relative_addons_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-19 16:35:53.000000 relative-addons-system-2.5.4/relative_addons_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 16:35:53.528545 relative-addons-system-2.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      902 2022-11-08 14:20:04.000000 relative-addons-system-2.5.4/setup.py
```

### Comparing `relative-addons-system-2.5.3/LICENSE` & `relative-addons-system-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.3/PKG-INFO` & `relative-addons-system-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relative-addons-system
-Version: 2.5.3
+Version: 2.5.4
 Summary: Easier way to manage your project addons
 Home-page: 
 Author: YoungTitanium
 Author-email: "kuyugama(youngtitanium)" <mail.kuyugama@gmail.com>
 License: Copyright 2022 kuyugama(youngtitanium)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `relative-addons-system-2.5.3/README.md` & `relative-addons-system-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.3/RelativeAddonsSystem/addon/__init__.py` & `relative-addons-system-2.5.4/RelativeAddonsSystem/addon/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,26 +12,32 @@
 class MetadataError(BaseException):
     pass
 
 
 class Addon:
     def __init__(self, path: Path, meta_path: Path = None, module=None):
 
+        if isinstance(path, str):
+            path = Path(path)
+
+        elif not isinstance(path, Path):
+            raise ValueError("Unsupported type for addon path - {type}".format(type=type(path)))
+
         if meta_path is None:
             meta_path = path / "addon.json"
 
         if not isinstance(meta_path, Path):
             raise MetadataError(
                 "Cannot recognize metadata of addon at {path}".format(
                     path=path.absolute()
                 )
             )
 
         self._meta = AddonMeta(meta_path)
-        self.path = path
+        self.path = path.absolute()
         self._module = module
         self._storage = None
 
         self._module_path = self.path.relative_to(Path().absolute())
         self._config_path = self.path / (self.meta.name + "-storage.json")
 
     @property
```

### Comparing `relative-addons-system-2.5.3/RelativeAddonsSystem/addon/metadata.py` & `relative-addons-system-2.5.4/RelativeAddonsSystem/addon/metadata.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.3/RelativeAddonsSystem/libraries.py` & `relative-addons-system-2.5.4/RelativeAddonsSystem/libraries.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.3/RelativeAddonsSystem/system.py` & `relative-addons-system-2.5.4/RelativeAddonsSystem/system.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.3/RelativeAddonsSystem/utils/cache.py` & `relative-addons-system-2.5.4/RelativeAddonsSystem/utils/cache.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.3/RelativeAddonsSystem/utils/storage.py` & `relative-addons-system-2.5.4/RelativeAddonsSystem/utils/storage.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.3/RelativeAddonsSystem/utils/version_checker.py` & `relative-addons-system-2.5.4/RelativeAddonsSystem/utils/version_checker.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.3/pyproject.toml` & `relative-addons-system-2.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative-addons-system"
-version = "2.5.3"
+version = "2.5.4"
 description = "Easier way to manage your project addons"
 authors = [{ name = "kuyugama(youngtitanium)", email = "mail.kuyugama@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `relative-addons-system-2.5.3/relative_addons_system.egg-info/PKG-INFO` & `relative-addons-system-2.5.4/relative_addons_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relative-addons-system
-Version: 2.5.3
+Version: 2.5.4
 Summary: Easier way to manage your project addons
 Home-page: 
 Author: YoungTitanium
 Author-email: "kuyugama(youngtitanium)" <mail.kuyugama@gmail.com>
 License: Copyright 2022 kuyugama(youngtitanium)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `relative-addons-system-2.5.3/relative_addons_system.egg-info/SOURCES.txt` & `relative-addons-system-2.5.4/relative_addons_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.5.3/setup.py` & `relative-addons-system-2.5.4/setup.py`

 * *Files identical despite different names*

