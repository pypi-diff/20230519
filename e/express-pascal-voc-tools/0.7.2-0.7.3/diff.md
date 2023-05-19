# Comparing `tmp/express-pascal-voc-tools-0.7.2.tar.gz` & `tmp/express-pascal-voc-tools-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express-pascal-voc-tools-0.7.2.tar", last modified: Mon May 15 16:37:50 2023, max compression
+gzip compressed data, was "express-pascal-voc-tools-0.7.3.tar", last modified: Fri May 19 09:09:50 2023, max compression
```

## Comparing `express-pascal-voc-tools-0.7.2.tar` & `express-pascal-voc-tools-0.7.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 16:37:50.837181 express-pascal-voc-tools-0.7.2/
--rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.7.2/LICENSE
--rw-rw-rw-   0        0        0     4900 2023-05-15 16:37:50.827940 express-pascal-voc-tools-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     4416 2023-05-11 13:01:05.000000 express-pascal-voc-tools-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 16:37:50.727942 express-pascal-voc-tools-0.7.2/express_pascal_voc_tools.egg-info/
--rw-rw-rw-   0        0        0     4900 2023-05-15 16:37:49.000000 express-pascal-voc-tools-0.7.2/express_pascal_voc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-15 16:37:50.000000 express-pascal-voc-tools-0.7.2/express_pascal_voc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 16:37:49.000000 express-pascal-voc-tools-0.7.2/express_pascal_voc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-15 16:37:49.000000 express-pascal-voc-tools-0.7.2/express_pascal_voc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 16:37:49.000000 express-pascal-voc-tools-0.7.2/express_pascal_voc_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 16:37:50.837181 express-pascal-voc-tools-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-05-15 16:37:29.000000 express-pascal-voc-tools-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:37:50.796774 express-pascal-voc-tools-0.7.2/voc_tools/
--rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.7.2/voc_tools/__init__.py
--rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.7.2/voc_tools/constants.py
--rw-rw-rw-   0        0        0     5146 2023-05-15 16:30:16.000000 express-pascal-voc-tools-0.7.2/voc_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:37:50.814531 express-pascal-voc-tools-0.7.2/voc_tools/unittest/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.7.2/voc_tools/unittest/__init__.py
--rw-rw-rw-   0        0        0     3745 2023-05-12 04:43:55.000000 express-pascal-voc-tools-0.7.2/voc_tools/unittest/reader_test.py
--rw-rw-rw-   0        0        0     8974 2023-05-15 16:30:16.000000 express-pascal-voc-tools-0.7.2/voc_tools/utils.py
--rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.7.2/voc_tools/visulizer.py
--rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.7.2/voc_tools/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:09:50.233495 express-pascal-voc-tools-0.7.3/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0     5588 2023-05-19 09:09:50.224937 express-pascal-voc-tools-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5104 2023-05-19 09:08:53.000000 express-pascal-voc-tools-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 09:09:50.104398 express-pascal-voc-tools-0.7.3/express_pascal_voc_tools.egg-info/
+-rw-rw-rw-   0        0        0     5588 2023-05-19 09:09:48.000000 express-pascal-voc-tools-0.7.3/express_pascal_voc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-19 09:09:49.000000 express-pascal-voc-tools-0.7.3/express_pascal_voc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 09:09:48.000000 express-pascal-voc-tools-0.7.3/express_pascal_voc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-19 09:09:48.000000 express-pascal-voc-tools-0.7.3/express_pascal_voc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 09:09:48.000000 express-pascal-voc-tools-0.7.3/express_pascal_voc_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 09:09:50.233495 express-pascal-voc-tools-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-05-19 09:09:11.000000 express-pascal-voc-tools-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:09:50.185542 express-pascal-voc-tools-0.7.3/voc_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.7.3/voc_tools/__init__.py
+-rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.7.3/voc_tools/constants.py
+-rw-rw-rw-   0        0        0     5146 2023-05-15 16:30:16.000000 express-pascal-voc-tools-0.7.3/voc_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:09:50.209142 express-pascal-voc-tools-0.7.3/voc_tools/unittest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.7.3/voc_tools/unittest/__init__.py
+-rw-rw-rw-   0        0        0     3745 2023-05-12 04:43:55.000000 express-pascal-voc-tools-0.7.3/voc_tools/unittest/reader_test.py
+-rw-rw-rw-   0        0        0     8974 2023-05-15 16:30:16.000000 express-pascal-voc-tools-0.7.3/voc_tools/utils.py
+-rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.7.3/voc_tools/visulizer.py
+-rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.7.3/voc_tools/writer.py
```

### Comparing `express-pascal-voc-tools-0.7.2/LICENSE` & `express-pascal-voc-tools-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.7.2/PKG-INFO` & `express-pascal-voc-tools-0.7.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: express-pascal-voc-tools
-Version: 0.7.2
-Summary: A tool for creating, reading and visualizing Pascal VOC annotations
-Author: Soumen Sardar
-Author-email: soumensardarintmain@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Express Pascal Voc Tools
 
 A tool for creating, reading and visualizing Pascal VOC annotations.
 **Report Bugs** [here](https://github.com/Redcof/pascal_voc_tools/issues)
 
 # Getting Started
 
@@ -171,15 +158,34 @@
 
 jpeg = from_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
 jpeg.see()
 # OR
 see_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
 ```
 
+### Load not PascalVOC dataset
+
+```python
+import pathlib
+from voc_tools.constants import VOC_IMAGES
+from voc_tools.reader import list_dir
+from voc_tools.utils import Dataset, VOCDataset
+
+dataset = pathlib.Path(r"path/to/dataset")
+# set global flags
+Dataset.IMAGE_DIR = "images"  # Say, instead of 'JPEGImages', the images are stored in 'images' directory
+# reading filepaths
+file_paths = list(list_dir(str(dataset / "train"), dir_flag=VOC_IMAGES, fullpath=True))
+file_paths.extend(list(list_dir(str(dataset / "test"), dir_flag=VOC_IMAGES, fullpath=True)))
+
+# if you have captions stored in 'captions' directory
+voc_data = VOCDataset(dataset, caption_support=True)
+```
+
 # Collaborate
 
 GitHub: [https://github.com/Redcof/pascal_voc_tools.git](https://github.com/Redcof/pascal_voc_tools.git)
 
 **Build and Publish**
 
 1. `python setup.py sdist bdist_wheel`
-1. `python -m twine upload dist/*`
+1. `python -m twine upload dist/*`
```

### Comparing `express-pascal-voc-tools-0.7.2/express_pascal_voc_tools.egg-info/PKG-INFO` & `express-pascal-voc-tools-0.7.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.7.2
+Version: 0.7.3
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -171,14 +171,33 @@
 
 jpeg = from_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
 jpeg.see()
 # OR
 see_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
 ```
 
+### Load not PascalVOC dataset
+
+```python
+import pathlib
+from voc_tools.constants import VOC_IMAGES
+from voc_tools.reader import list_dir
+from voc_tools.utils import Dataset, VOCDataset
+
+dataset = pathlib.Path(r"path/to/dataset")
+# set global flags
+Dataset.IMAGE_DIR = "images"  # Say, instead of 'JPEGImages', the images are stored in 'images' directory
+# reading filepaths
+file_paths = list(list_dir(str(dataset / "train"), dir_flag=VOC_IMAGES, fullpath=True))
+file_paths.extend(list(list_dir(str(dataset / "test"), dir_flag=VOC_IMAGES, fullpath=True)))
+
+# if you have captions stored in 'captions' directory
+voc_data = VOCDataset(dataset, caption_support=True)
+```
+
 # Collaborate
 
 GitHub: [https://github.com/Redcof/pascal_voc_tools.git](https://github.com/Redcof/pascal_voc_tools.git)
 
 **Build and Publish**
 
 1. `python setup.py sdist bdist_wheel`
```

### Comparing `express-pascal-voc-tools-0.7.2/setup.py` & `express-pascal-voc-tools-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=['lxml', 'numpy', 'opencv-python'],
     version_config=True,
-    version="0.7.2"
+    version="0.7.3"
     # setup_requires=["setuptools-git-versioning"]
 )
```

### Comparing `express-pascal-voc-tools-0.7.2/voc_tools/reader.py` & `express-pascal-voc-tools-0.7.3/voc_tools/reader.py`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.7.2/voc_tools/unittest/reader_test.py` & `express-pascal-voc-tools-0.7.3/voc_tools/unittest/reader_test.py`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.7.2/voc_tools/utils.py` & `express-pascal-voc-tools-0.7.3/voc_tools/utils.py`

 * *Files identical despite different names*

