# Comparing `tmp/Phanatic-2.2.0.tar.gz` & `tmp/Phanatic-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Phanatic-2.2.0.tar", last modified: Thu May 18 09:57:31 2023, max compression
+gzip compressed data, was "Phanatic-2.2.1.tar", last modified: Fri May 19 09:52:31 2023, max compression
```

## Comparing `Phanatic-2.2.0.tar` & `Phanatic-2.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-18 09:57:31.259535 Phanatic-2.2.0/
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)    34523 2023-05-18 09:50:13.000000 Phanatic-2.2.0/LICENSE.md
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      723 2023-05-18 09:57:31.259535 Phanatic-2.2.0/PKG-INFO
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-18 09:57:31.259535 Phanatic-2.2.0/Phanatic/
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-18 09:53:44.000000 Phanatic-2.2.0/Phanatic/__init__.py
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     4116 2023-05-18 09:55:54.000000 Phanatic-2.2.0/Phanatic/main.py
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-18 09:57:31.259535 Phanatic-2.2.0/Phanatic.egg-info/
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      723 2023-05-18 09:57:31.000000 Phanatic-2.2.0/Phanatic.egg-info/PKG-INFO
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      220 2023-05-18 09:57:31.000000 Phanatic-2.2.0/Phanatic.egg-info/SOURCES.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        1 2023-05-18 09:57:31.000000 Phanatic-2.2.0/Phanatic.egg-info/dependency_links.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       51 2023-05-18 09:57:31.000000 Phanatic-2.2.0/Phanatic.egg-info/entry_points.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        9 2023-05-18 09:57:31.000000 Phanatic-2.2.0/Phanatic.egg-info/top_level.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       38 2023-05-18 09:57:31.259535 Phanatic-2.2.0/setup.cfg
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     1002 2023-05-18 09:57:03.000000 Phanatic-2.2.0/setup.py
+drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-19 09:52:31.785738 Phanatic-2.2.1/
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)    34523 2023-05-19 09:37:09.000000 Phanatic-2.2.1/LICENSE.md
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      723 2023-05-19 09:52:31.785738 Phanatic-2.2.1/PKG-INFO
+drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-19 09:52:31.785738 Phanatic-2.2.1/Phanatic/
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-19 09:37:09.000000 Phanatic-2.2.1/Phanatic/__init__.py
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     4116 2023-05-19 09:51:56.000000 Phanatic-2.2.1/Phanatic/main.py
+drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-19 09:52:31.785738 Phanatic-2.2.1/Phanatic.egg-info/
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      723 2023-05-19 09:52:31.000000 Phanatic-2.2.1/Phanatic.egg-info/PKG-INFO
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      220 2023-05-19 09:52:31.000000 Phanatic-2.2.1/Phanatic.egg-info/SOURCES.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        1 2023-05-19 09:52:31.000000 Phanatic-2.2.1/Phanatic.egg-info/dependency_links.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       51 2023-05-19 09:52:31.000000 Phanatic-2.2.1/Phanatic.egg-info/entry_points.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        9 2023-05-19 09:52:31.000000 Phanatic-2.2.1/Phanatic.egg-info/top_level.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       38 2023-05-19 09:52:31.785738 Phanatic-2.2.1/setup.cfg
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     1002 2023-05-19 09:51:06.000000 Phanatic-2.2.1/setup.py
```

### Comparing `Phanatic-2.2.0/LICENSE.md` & `Phanatic-2.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Phanatic-2.2.0/PKG-INFO` & `Phanatic-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Phanatic
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python package to run de novo bacteriophage assembly container.
 Home-page: https://github.com/JoshuaIszatt/Phanatic
 Author: Joshua Iszatt
 Author-email: joshiszatt@gmail.com
 License: AGPL-3.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `Phanatic-2.2.0/Phanatic/main.py` & `Phanatic-2.2.1/Phanatic/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 f"{file_path} is not a valid file path")
         if not os.access(file_path, os.R_OK):
             raise argparse.ArgumentTypeError(
                 f"{file_path} is not a readable file")
         return file_path
 
     # Parsing arguments
-    image = 'iszatt/phanatic:2.2.0'
+    image = 'iszatt/phanatic:2.2.1'
     parser = argparse.ArgumentParser(description=f"Easy short read assembly. Joshua J Iszatt: https://github.com/JoshuaIszatt")
 
     # Input/output options
     parser.add_argument('-i', '--input', type=valid_dir, help='Input reads files')
     parser.add_argument('-o', '--output', type=valid_dir, help='Direct output to this location')
     parser.add_argument('-r', '--reads', type=str, choices=['PE_illumina_150'], default='PE_illumina_150', help='Pipeline options')
     parser.add_argument('-c', '--config', type=valid_file, help='Use config file to customise assembly')
```

### Comparing `Phanatic-2.2.0/Phanatic.egg-info/PKG-INFO` & `Phanatic-2.2.1/Phanatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Phanatic
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python package to run de novo bacteriophage assembly container.
 Home-page: https://github.com/JoshuaIszatt/Phanatic
 Author: Joshua Iszatt
 Author-email: joshiszatt@gmail.com
 License: AGPL-3.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `Phanatic-2.2.0/setup.py` & `Phanatic-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="Phanatic",
-    version="2.2.0",
+    version="2.2.1",
     description="Python package to run de novo bacteriophage assembly container.",
     url="https://github.com/JoshuaIszatt/Phanatic",
     author="Joshua Iszatt",
     author_email="joshiszatt@gmail.com",
     license="AGPL-3.0",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
```

