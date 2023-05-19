# Comparing `tmp/unitlab-1.8.3.tar.gz` & `tmp/unitlab-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-1.8.3.tar", last modified: Thu May 18 07:14:54 2023, max compression
+gzip compressed data, was "unitlab-1.8.4.tar", last modified: Fri May 19 07:14:11 2023, max compression
```

## Comparing `unitlab-1.8.3.tar` & `unitlab-1.8.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-18 07:14:54.870458 unitlab-1.8.3/
--rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.3/LICENSE.md
--rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.3/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-18 07:14:54.870458 unitlab-1.8.3/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      812 2023-05-16 06:53:44.000000 unitlab-1.8.3/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2023-05-18 07:14:54.870458 unitlab-1.8.3/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1114 2023-05-18 07:13:54.000000 unitlab-1.8.3/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-18 07:14:54.866459 unitlab-1.8.3/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-18 07:14:54.866459 unitlab-1.8.3/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)       63 2023-05-17 08:58:29.000000 unitlab-1.8.3/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)    11120 2023-05-17 13:54:30.000000 unitlab-1.8.3/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)      746 2023-05-17 08:50:07.000000 unitlab-1.8.3/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     4572 2023-05-17 13:51:47.000000 unitlab-1.8.3/src/unitlab/pretty.py
--rw-rw-r--   0 me        (1000) me        (1000)     2311 2023-05-17 13:50:32.000000 unitlab-1.8.3/src/unitlab/run.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-18 07:14:54.870458 unitlab-1.8.3/src/unitlab.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-18 07:14:54.000000 unitlab-1.8.3/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      376 2023-05-18 07:14:54.000000 unitlab-1.8.3/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-05-18 07:14:54.000000 unitlab-1.8.3/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       44 2023-05-18 07:14:54.000000 unitlab-1.8.3/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       61 2023-05-18 07:14:54.000000 unitlab-1.8.3/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-05-18 07:14:54.000000 unitlab-1.8.3/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-19 07:14:11.219713 unitlab-1.8.4/
+-rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.4/LICENSE.md
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.4/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-19 07:14:11.219713 unitlab-1.8.4/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      812 2023-05-16 06:53:44.000000 unitlab-1.8.4/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2023-05-19 07:14:11.219713 unitlab-1.8.4/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1131 2023-05-19 07:12:49.000000 unitlab-1.8.4/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-19 07:14:11.215713 unitlab-1.8.4/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-19 07:14:11.215713 unitlab-1.8.4/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)       63 2023-05-17 08:58:29.000000 unitlab-1.8.4/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)    11120 2023-05-17 13:54:30.000000 unitlab-1.8.4/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)      746 2023-05-17 08:50:07.000000 unitlab-1.8.4/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     4572 2023-05-17 13:51:47.000000 unitlab-1.8.4/src/unitlab/pretty.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2311 2023-05-17 13:50:32.000000 unitlab-1.8.4/src/unitlab/run.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-19 07:14:11.219713 unitlab-1.8.4/src/unitlab.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      376 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       44 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       67 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-1.8.3/LICENSE.md` & `unitlab-1.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.3/PKG-INFO` & `unitlab-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.8.3
+Version: 1.8.4
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `unitlab-1.8.3/README.md` & `unitlab-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.3/setup.py` & `unitlab-1.8.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="1.8.3",
+    version="1.8.4",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
@@ -21,18 +21,19 @@
         "Programming Language :: Python :: 3.11",
     ],
     package_dir={"": "src"},
     url="https://github.com/teamunitlab/unitlab-sdk",
     keywords="unitlab-sdk",
     install_requires=[
         "aiohttp",
-        "requests",
-        "prettytable",
-        "tqdm",
         "numpy",
         "opencv-python",
         "Pillow",
+        "prettytable",
+        "requests",
+        "tqdm",
+        "typer",
     ],
     entry_points={
         "console_scripts": ["unitlab=unitlab.run:app"],
     },
 )
```

### Comparing `unitlab-1.8.3/src/unitlab/client.py` & `unitlab-1.8.4/src/unitlab/client.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.3/src/unitlab/exceptions.py` & `unitlab-1.8.4/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.3/src/unitlab/pretty.py` & `unitlab-1.8.4/src/unitlab/pretty.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.3/src/unitlab/run.py` & `unitlab-1.8.4/src/unitlab/run.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.3/src/unitlab.egg-info/PKG-INFO` & `unitlab-1.8.4/src/unitlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.8.3
+Version: 1.8.4
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

