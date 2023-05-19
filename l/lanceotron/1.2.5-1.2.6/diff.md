# Comparing `tmp/lanceotron-1.2.5.tar.gz` & `tmp/lanceotron-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanceotron-1.2.5.tar", last modified: Fri May 12 08:31:51 2023, max compression
+gzip compressed data, was "lanceotron-1.2.6.tar", last modified: Fri May 19 08:12:52 2023, max compression
```

## Comparing `lanceotron-1.2.5.tar` & `lanceotron-1.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lancehentges   (501) staff       (20)        0 2023-05-12 08:31:51.664939 lanceotron-1.2.5/
--rw-r--r--   0 lancehentges   (501) staff       (20)    35149 2023-05-10 14:56:30.000000 lanceotron-1.2.5/LICENSE
--rw-r--r--   0 lancehentges   (501) staff       (20)      210 2023-05-10 14:56:30.000000 lanceotron-1.2.5/MANIFEST.in
--rw-r--r--   0 lancehentges   (501) staff       (20)     4614 2023-05-12 08:31:51.664576 lanceotron-1.2.5/PKG-INFO
--rw-r--r--   0 lancehentges   (501) staff       (20)     4137 2023-05-10 14:56:30.000000 lanceotron-1.2.5/README.md
-drwxr-xr-x   0 lancehentges   (501) staff       (20)        0 2023-05-12 08:31:51.656212 lanceotron-1.2.5/lanceotron/
--rw-r--r--   0 lancehentges   (501) staff       (20)      147 2023-05-10 15:43:51.000000 lanceotron-1.2.5/lanceotron/__init__.py
--rw-r--r--   0 lancehentges   (501) staff       (20)     3757 2023-05-10 14:56:30.000000 lanceotron-1.2.5/lanceotron/cli.py
--rw-r--r--   0 lancehentges   (501) staff       (20)    32391 2023-05-11 08:03:27.000000 lanceotron-1.2.5/lanceotron/lanceotron.py
--rw-r--r--   0 lancehentges   (501) staff       (20)    16066 2023-05-11 08:03:27.000000 lanceotron-1.2.5/lanceotron/modules.py
-drwxr-xr-x   0 lancehentges   (501) staff       (20)        0 2023-05-12 08:31:51.660839 lanceotron-1.2.5/lanceotron/static/
--rw-r--r--   0 lancehentges   (501) staff       (20)       38 2023-05-10 14:56:30.000000 lanceotron-1.2.5/lanceotron/static/__init__.py
--rw-r--r--   0 lancehentges   (501) staff       (20)    48467 2023-05-10 14:56:30.000000 lanceotron-1.2.5/lanceotron/static/standard_scaler_deep_v5_03.p
--rw-r--r--   0 lancehentges   (501) staff       (20)      742 2023-05-10 14:56:30.000000 lanceotron-1.2.5/lanceotron/static/standard_scaler_wide_v5_03.p
--rw-r--r--   0 lancehentges   (501) staff       (20)  1727328 2023-05-10 14:56:30.000000 lanceotron-1.2.5/lanceotron/static/wide_and_deep_fully_trained_v5_03.h5
--rw-r--r--   0 lancehentges   (501) staff       (20)     4799 2023-05-10 14:56:30.000000 lanceotron-1.2.5/lanceotron/utils.py
-drwxr-xr-x   0 lancehentges   (501) staff       (20)        0 2023-05-12 08:31:51.659057 lanceotron-1.2.5/lanceotron.egg-info/
--rw-r--r--   0 lancehentges   (501) staff       (20)     4614 2023-05-12 08:31:51.000000 lanceotron-1.2.5/lanceotron.egg-info/PKG-INFO
--rw-r--r--   0 lancehentges   (501) staff       (20)      549 2023-05-12 08:31:51.000000 lanceotron-1.2.5/lanceotron.egg-info/SOURCES.txt
--rw-r--r--   0 lancehentges   (501) staff       (20)        1 2023-05-12 08:31:51.000000 lanceotron-1.2.5/lanceotron.egg-info/dependency_links.txt
--rw-r--r--   0 lancehentges   (501) staff       (20)       50 2023-05-12 08:31:51.000000 lanceotron-1.2.5/lanceotron.egg-info/entry_points.txt
--rw-r--r--   0 lancehentges   (501) staff       (20)       67 2023-05-12 08:31:51.000000 lanceotron-1.2.5/lanceotron.egg-info/requires.txt
--rw-r--r--   0 lancehentges   (501) staff       (20)       11 2023-05-12 08:31:51.000000 lanceotron-1.2.5/lanceotron.egg-info/top_level.txt
--rw-r--r--   0 lancehentges   (501) staff       (20)       38 2023-05-12 08:31:51.665038 lanceotron-1.2.5/setup.cfg
--rw-r--r--   0 lancehentges   (501) staff       (20)     1025 2023-05-12 08:29:45.000000 lanceotron-1.2.5/setup.py
-drwxr-xr-x   0 lancehentges   (501) staff       (20)        0 2023-05-12 08:31:51.663864 lanceotron-1.2.5/test/
--rw-r--r--   0 lancehentges   (501) staff       (20)     3357 2023-05-10 14:56:30.000000 lanceotron-1.2.5/test/test_main.py
+drwxr-xr-x   0 lancehentges   (501) staff       (20)        0 2023-05-19 08:12:52.685346 lanceotron-1.2.6/
+-rw-r--r--   0 lancehentges   (501) staff       (20)    35149 2023-05-10 14:56:30.000000 lanceotron-1.2.6/LICENSE
+-rw-r--r--   0 lancehentges   (501) staff       (20)      210 2023-05-10 14:56:30.000000 lanceotron-1.2.6/MANIFEST.in
+-rw-r--r--   0 lancehentges   (501) staff       (20)     4614 2023-05-19 08:12:52.685072 lanceotron-1.2.6/PKG-INFO
+-rw-r--r--   0 lancehentges   (501) staff       (20)     4137 2023-05-10 14:56:30.000000 lanceotron-1.2.6/README.md
+drwxr-xr-x   0 lancehentges   (501) staff       (20)        0 2023-05-19 08:12:52.673707 lanceotron-1.2.6/lanceotron/
+-rw-r--r--   0 lancehentges   (501) staff       (20)      147 2023-05-10 15:43:51.000000 lanceotron-1.2.6/lanceotron/__init__.py
+-rw-r--r--   0 lancehentges   (501) staff       (20)     3757 2023-05-10 14:56:30.000000 lanceotron-1.2.6/lanceotron/cli.py
+-rw-r--r--   0 lancehentges   (501) staff       (20)    32391 2023-05-11 08:03:27.000000 lanceotron-1.2.6/lanceotron/lanceotron.py
+-rw-r--r--   0 lancehentges   (501) staff       (20)    16024 2023-05-19 08:06:19.000000 lanceotron-1.2.6/lanceotron/modules.py
+drwxr-xr-x   0 lancehentges   (501) staff       (20)        0 2023-05-19 08:12:52.679027 lanceotron-1.2.6/lanceotron/static/
+-rw-r--r--   0 lancehentges   (501) staff       (20)       38 2023-05-10 14:56:30.000000 lanceotron-1.2.6/lanceotron/static/__init__.py
+-rw-r--r--   0 lancehentges   (501) staff       (20)    48467 2023-05-10 14:56:30.000000 lanceotron-1.2.6/lanceotron/static/standard_scaler_deep_v5_03.p
+-rw-r--r--   0 lancehentges   (501) staff       (20)      742 2023-05-10 14:56:30.000000 lanceotron-1.2.6/lanceotron/static/standard_scaler_wide_v5_03.p
+-rw-r--r--   0 lancehentges   (501) staff       (20)  1727328 2023-05-10 14:56:30.000000 lanceotron-1.2.6/lanceotron/static/wide_and_deep_fully_trained_v5_03.h5
+-rw-r--r--   0 lancehentges   (501) staff       (20)     4799 2023-05-10 14:56:30.000000 lanceotron-1.2.6/lanceotron/utils.py
+drwxr-xr-x   0 lancehentges   (501) staff       (20)        0 2023-05-19 08:12:52.676262 lanceotron-1.2.6/lanceotron.egg-info/
+-rw-r--r--   0 lancehentges   (501) staff       (20)     4614 2023-05-19 08:12:52.000000 lanceotron-1.2.6/lanceotron.egg-info/PKG-INFO
+-rw-r--r--   0 lancehentges   (501) staff       (20)      549 2023-05-19 08:12:52.000000 lanceotron-1.2.6/lanceotron.egg-info/SOURCES.txt
+-rw-r--r--   0 lancehentges   (501) staff       (20)        1 2023-05-19 08:12:52.000000 lanceotron-1.2.6/lanceotron.egg-info/dependency_links.txt
+-rw-r--r--   0 lancehentges   (501) staff       (20)       50 2023-05-19 08:12:52.000000 lanceotron-1.2.6/lanceotron.egg-info/entry_points.txt
+-rw-r--r--   0 lancehentges   (501) staff       (20)       67 2023-05-19 08:12:52.000000 lanceotron-1.2.6/lanceotron.egg-info/requires.txt
+-rw-r--r--   0 lancehentges   (501) staff       (20)       11 2023-05-19 08:12:52.000000 lanceotron-1.2.6/lanceotron.egg-info/top_level.txt
+-rw-r--r--   0 lancehentges   (501) staff       (20)       38 2023-05-19 08:12:52.685418 lanceotron-1.2.6/setup.cfg
+-rw-r--r--   0 lancehentges   (501) staff       (20)     1025 2023-05-19 08:09:46.000000 lanceotron-1.2.6/setup.py
+drwxr-xr-x   0 lancehentges   (501) staff       (20)        0 2023-05-19 08:12:52.684720 lanceotron-1.2.6/test/
+-rw-r--r--   0 lancehentges   (501) staff       (20)     3357 2023-05-10 14:56:30.000000 lanceotron-1.2.6/test/test_main.py
```

### Comparing `lanceotron-1.2.5/LICENSE` & `lanceotron-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lanceotron-1.2.5/PKG-INFO` & `lanceotron-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanceotron
-Version: 1.2.5
+Version: 1.2.6
 Summary: Command-line interface to the lanceotron deep learning peak caller
 Author: Chris Cole, Lance Hentges, Simone G. Riva
 Author-email: simo.riva15@gmail.com
 Project-URL: Bug Tracker, https://github.com/LHentges/lanceotron/issues
 Project-URL: Source, https://github.com/LHentges/lanceotron
 Keywords: deep learning,peak calling,keras
 Requires-Python: >=3.7
```

### Comparing `lanceotron-1.2.5/README.md` & `lanceotron-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `lanceotron-1.2.5/lanceotron/cli.py` & `lanceotron-1.2.6/lanceotron/cli.py`

 * *Files identical despite different names*

### Comparing `lanceotron-1.2.5/lanceotron/lanceotron.py` & `lanceotron-1.2.6/lanceotron/lanceotron.py`

 * *Files identical despite different names*

### Comparing `lanceotron-1.2.5/lanceotron/modules.py` & `lanceotron-1.2.6/lanceotron/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                 out_list = [
                     chrom,
                     coord_pair[0],
                     coord_pair[1],
                     model_classifications[0][i][0],
                     model_classifications[1][i][0],
                     model_classifications[2][i][0],
-                    max_array[i]+coord_pair[0],
+                    max_array[i],
                     region_counter+i
                 ]
                 X_wide_list = X_wide_array[i][:-1].tolist()
                 X_wide_list = [100.0 if x > 10 else x for x in X_wide_list]
                 out_list += X_wide_list
                 chrom_file_out.append(out_list)
             bed_file_out += chrom_file_out
@@ -269,15 +269,15 @@
                     chrom,
                     coord_pair[0],
                     coord_pair[1],
                     model_classifications[0][i][0],
                     model_classifications[1][i][0],
                     model_classifications[2][i][0],
                     pvalue_input,
-                    max_array[i]+coord_pair[0],
+                    max_array[i],
                     i+region_counter
                 ]
                 X_wide_list = X_wide_array[i][:-1].tolist()
                 X_wide_list = [100.0 if x > 10 else x for x in X_wide_list]
                 out_list += X_wide_list
                 chrom_file_out.append(out_list)
             pyBigWig_input.close()
@@ -369,15 +369,15 @@
                 out_list = [
                     chrom,
                     coord_pair[0],
                     coord_pair[1],
                     model_classifications[0][i][0],
                     model_classifications[1][i][0],
                     model_classifications[2][i][0],
-                    max_array[i]+coord_pair[0],
+                    max_array[i],
                     region_counter + i,
                 ]
                 X_wide_list = X_wide_array[i][:-1].tolist()
                 X_wide_list = [100.0 if x > 10 else x for x in X_wide_list]
                 out_list += X_wide_list
                 chrom_file_out.append(out_list)
             bed_file_out += chrom_file_out
```

### Comparing `lanceotron-1.2.5/lanceotron/static/standard_scaler_deep_v5_03.p` & `lanceotron-1.2.6/lanceotron/static/standard_scaler_deep_v5_03.p`

 * *Files identical despite different names*

### Comparing `lanceotron-1.2.5/lanceotron/static/standard_scaler_wide_v5_03.p` & `lanceotron-1.2.6/lanceotron/static/standard_scaler_wide_v5_03.p`

 * *Files identical despite different names*

### Comparing `lanceotron-1.2.5/lanceotron/static/wide_and_deep_fully_trained_v5_03.h5` & `lanceotron-1.2.6/lanceotron/static/wide_and_deep_fully_trained_v5_03.h5`

 * *Files identical despite different names*

### Comparing `lanceotron-1.2.5/lanceotron/utils.py` & `lanceotron-1.2.6/lanceotron/utils.py`

 * *Files identical despite different names*

### Comparing `lanceotron-1.2.5/lanceotron.egg-info/PKG-INFO` & `lanceotron-1.2.6/lanceotron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanceotron
-Version: 1.2.5
+Version: 1.2.6
 Summary: Command-line interface to the lanceotron deep learning peak caller
 Author: Chris Cole, Lance Hentges, Simone G. Riva
 Author-email: simo.riva15@gmail.com
 Project-URL: Bug Tracker, https://github.com/LHentges/lanceotron/issues
 Project-URL: Source, https://github.com/LHentges/lanceotron
 Keywords: deep learning,peak calling,keras
 Requires-Python: >=3.7
```

### Comparing `lanceotron-1.2.5/lanceotron.egg-info/SOURCES.txt` & `lanceotron-1.2.6/lanceotron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lanceotron-1.2.5/setup.py` & `lanceotron-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
    name='lanceotron',
-   version='1.2.5',
+   version='1.2.6',
    python_requires='>=3.7', 
    description='Command-line interface to the lanceotron deep learning peak caller',
    long_description=long_description,
    long_description_content_type="text/markdown",
    project_urls={
        "Bug Tracker": "https://github.com/LHentges/lanceotron/issues",
        "Source": "https://github.com/LHentges/lanceotron"},
```

### Comparing `lanceotron-1.2.5/test/test_main.py` & `lanceotron-1.2.6/test/test_main.py`

 * *Files identical despite different names*

