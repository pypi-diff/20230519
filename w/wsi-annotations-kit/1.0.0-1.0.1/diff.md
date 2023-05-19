# Comparing `tmp/wsi-annotations-kit-1.0.0.tar.gz` & `tmp/wsi-annotations-kit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wsi-annotations-kit-1.0.0.tar", last modified: Wed May 17 21:53:13 2023, max compression
+gzip compressed data, was "dist\wsi-annotations-kit-1.0.1.tar", last modified: Fri May 19 18:51:46 2023, max compression
```

## Comparing `wsi-annotations-kit-1.0.0.tar` & `wsi-annotations-kit-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 21:53:13.000000 wsi-annotations-kit-1.0.0/
--rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      621 2023-05-17 21:53:13.000000 wsi-annotations-kit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      136 2023-05-17 17:57:10.000000 wsi-annotations-kit-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 21:53:13.000000 wsi-annotations-kit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      701 2023-05-17 21:53:09.000000 wsi-annotations-kit-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:53:13.000000 wsi-annotations-kit-1.0.0/wsi_annotations_kit.egg-info/
--rw-rw-rw-   0        0        0      621 2023-05-17 21:53:12.000000 wsi-annotations-kit-1.0.0/wsi_annotations_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-05-17 21:53:13.000000 wsi-annotations-kit-1.0.0/wsi_annotations_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 21:53:12.000000 wsi-annotations-kit-1.0.0/wsi_annotations_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 21:53:12.000000 wsi-annotations-kit-1.0.0/wsi_annotations_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 18:51:46.000000 wsi-annotations-kit-1.0.1/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      621 2023-05-19 18:51:46.000000 wsi-annotations-kit-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2023-05-17 17:57:10.000000 wsi-annotations-kit-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 18:51:46.000000 wsi-annotations-kit-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      701 2023-05-19 18:44:03.000000 wsi-annotations-kit-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:51:46.000000 wsi-annotations-kit-1.0.1/wsi_annotations_kit.egg-info/
+-rw-rw-rw-   0        0        0      621 2023-05-19 18:51:46.000000 wsi-annotations-kit-1.0.1/wsi_annotations_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-05-19 18:51:46.000000 wsi-annotations-kit-1.0.1/wsi_annotations_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 18:51:46.000000 wsi-annotations-kit-1.0.1/wsi_annotations_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 18:51:46.000000 wsi-annotations-kit-1.0.1/wsi_annotations_kit.egg-info/top_level.txt
```

### Comparing `wsi-annotations-kit-1.0.0/LICENSE` & `wsi-annotations-kit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wsi-annotations-kit-1.0.0/PKG-INFO` & `wsi-annotations-kit-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsi-annotations-kit-1.0.0/setup.py` & `wsi-annotations-kit-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wsi-annotations-kit",
-    version="1.0.0",
+    version="1.0.1",
     author="Sam Border",
     author_email="sam.border2256@gmail.com",
     description="Utility functions for generating, saving, and converting annotation files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spborder/wsi_annotations_kit",
     packages=setuptools.find_packages(),
```

### Comparing `wsi-annotations-kit-1.0.0/wsi_annotations_kit.egg-info/PKG-INFO` & `wsi-annotations-kit-1.0.1/wsi_annotations_kit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

