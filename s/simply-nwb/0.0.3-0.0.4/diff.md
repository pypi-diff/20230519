# Comparing `tmp/simply_nwb-0.0.3.tar.gz` & `tmp/simply_nwb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.0.3.tar", last modified: Fri May 12 16:34:26 2023, max compression
+gzip compressed data, was "simply_nwb-0.0.4.tar", last modified: Fri May 19 19:32:26 2023, max compression
```

## Comparing `simply_nwb-0.0.3.tar` & `simply_nwb-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.801905 simply_nwb-0.0.3/
--rw-rw-rw-   0        0        0      494 2023-05-12 16:34:26.800908 simply_nwb-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-10 16:56:33.000000 simply_nwb-0.0.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-12 16:34:26.801905 simply_nwb-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-05-12 16:26:57.000000 simply_nwb-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.788162 simply_nwb-0.0.3/simply_nwb/
--rw-rw-rw-   0        0        0       35 2023-05-10 18:53:16.000000 simply_nwb-0.0.3/simply_nwb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.794921 simply_nwb-0.0.3/simply_nwb/acquisition/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:12:45.000000 simply_nwb-0.0.3/simply_nwb/acquisition/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.798910 simply_nwb-0.0.3/simply_nwb/acquisition/tools/
--rw-rw-rw-   0        0        0       50 2023-05-10 20:47:41.000000 simply_nwb-0.0.3/simply_nwb/acquisition/tools/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-05-10 17:46:16.000000 simply_nwb-0.0.3/simply_nwb/acquisition/tools/blackrock.py
--rw-rw-rw-   0        0        0     3831 2023-05-11 16:28:17.000000 simply_nwb-0.0.3/simply_nwb/acquisition/tools/p_erg.py
--rw-rw-rw-   0        0        0      436 2023-05-12 15:44:54.000000 simply_nwb-0.0.3/simply_nwb/nwb_inspect_script.py
--rw-rw-rw-   0        0        0    11191 2023-05-12 15:49:58.000000 simply_nwb-0.0.3/simply_nwb/simple_nwb.py
--rw-rw-rw-   0        0        0     3774 2023-05-12 15:53:16.000000 simply_nwb-0.0.3/simply_nwb/testing.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.799914 simply_nwb-0.0.3/simply_nwb/transforms/
--rw-rw-rw-   0        0        0        0 2023-05-10 16:49:20.000000 simply_nwb-0.0.3/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     2026 2023-05-12 15:44:54.000000 simply_nwb-0.0.3/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.793923 simply_nwb-0.0.3/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      494 2023-05-12 16:34:26.000000 simply_nwb-0.0.3/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-05-12 16:34:26.000000 simply_nwb-0.0.3/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 16:34:26.000000 simply_nwb-0.0.3/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-12 16:34:26.000000 simply_nwb-0.0.3/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-12 16:34:26.000000 simply_nwb-0.0.3/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.230713 simply_nwb-0.0.4/
+-rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-05-19 19:32:26.230713 simply_nwb-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:32:26.230713 simply_nwb-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-05-19 19:32:25.000000 simply_nwb-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.217682 simply_nwb-0.0.4/simply_nwb/
+-rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.221680 simply_nwb-0.0.4/simply_nwb/acquisition/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/acquisition/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.229205 simply_nwb-0.0.4/simply_nwb/acquisition/tools/
+-rw-rw-rw-   0        0        0      181 2023-05-19 17:18:00.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/blackrock.py
+-rw-rw-rw-   0        0        0      563 2023-05-19 17:18:00.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/csv.py
+-rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/labjack.py
+-rw-rw-rw-   0        0        0     3990 2023-05-19 17:18:00.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/mp4.py
+-rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/p_erg.py
+-rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/plaintext.py
+-rw-rw-rw-   0        0        0     3382 2023-05-19 17:18:00.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/tif.py
+-rw-rw-rw-   0        0        0      462 2023-05-19 17:18:00.000000 simply_nwb-0.0.4/simply_nwb/acquisition/tools/yaml.py
+-rw-rw-rw-   0        0        0      436 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/nwb_inspect_script.py
+-rw-rw-rw-   0        0        0    15731 2023-05-19 17:44:29.000000 simply_nwb-0.0.4/simply_nwb/simple_nwb.py
+-rw-rw-rw-   0        0        0     6651 2023-05-19 17:48:58.000000 simply_nwb-0.0.4/simply_nwb/testing.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.229205 simply_nwb-0.0.4/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.4/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     3498 2023-05-19 17:39:54.000000 simply_nwb-0.0.4/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:32:26.220691 simply_nwb-0.0.4/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-05-19 19:32:26.000000 simply_nwb-0.0.4/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-05-19 19:32:26.000000 simply_nwb-0.0.4/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:32:26.000000 simply_nwb-0.0.4/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-05-19 19:32:26.000000 simply_nwb-0.0.4/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-19 19:32:26.000000 simply_nwb-0.0.4/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.0.3/setup.py` & `simply_nwb-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
 
 
 with open('./README.rst') as f:
     long_description = f.read()
 
 
 setup(
     name='simply_nwb',
-    packages=['simply_nwb', 'simply_nwb.acquisition', 'simply_nwb.acquisition.tools', 'simply_nwb.transforms'],
+    packages=find_packages(),
     version=VERSION,
     description='Common NWB use cases and simplified interface for common usage',
     author='Spencer Hanson',
     long_description=long_description,
     install_requires=parse_requirements('requirements.txt'),
     keywords=['neuroscience', 'nwb', 'tools', 'science'],
     classifiers=[
```

### Comparing `simply_nwb-0.0.3/simply_nwb/acquisition/tools/blackrock.py` & `simply_nwb-0.0.4/simply_nwb/acquisition/tools/blackrock.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.3/simply_nwb/acquisition/tools/p_erg.py` & `simply_nwb-0.0.4/simply_nwb/acquisition/tools/p_erg.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import pandas as pd
 from io import StringIO
 
 from simply_nwb.util import warn_on_name_format
 
 
 def _format_column_name(column_name):
-    """
-    Internal helper function to help rename columns
-    e.g. 'Data Pnt(ms):' -> 'data_pnt_ms'
+    # Internal helper function to help rename columns
+    # e.g. 'Data Pnt(ms):' -> 'data_pnt_ms'
+    #
+    # :param column_name: input column name
+    # :return: str of reformatted column name
 
-    :param column_name: input column name
-    :return: str of reformatted column name
-    """
     replacements = [
         # Turn ')' into a '_'
         # e.g. 'Data Pnt(ms):' -> 'Data Pnt_ms):'
         ("(", "_"),
         (":", ""),
         (" ", "_"),
         (")", ""),
@@ -26,14 +25,15 @@
         column_name = column_name.replace(from_val, to_val)
 
     column_name = column_name.lower()  # To lowercase
     return column_name
 
 
 def _parse_perg_metadata(filename):
+    # Helper func
     divider_count = 0
     line_datas = []
 
     with open(filename, "r") as f:
         data = f.readlines()
         for line in data:
             if divider_count == 0:
@@ -45,35 +45,33 @@
                 else:
                     line_datas.append(line)
         line_datas.insert(0, "value")  # Insert dummy first entry
         return pd.read_csv(StringIO("\n".join(line_datas))).T  # Transpose since data is formatted sideways
 
 
 def _reformat_column_names(panda_data):
-    """
-    Helper function to rename the columns in a pandas dataframe
-    :param panda_data: pd dataframe
-    :return: pd dataframe with different column names, formatted nicer
-    """
+    # Helper function to rename the columns in a pandas dataframe
+    # :param panda_data: pd dataframe
+    # :return: pd dataframe with different column names, formatted nicer
+
     rename_mapping = []
     for col_name in panda_data.columns:
         rename_mapping.append([col_name, _format_column_name(col_name)])
 
     for old_name, new_name in rename_mapping:
         panda_data[new_name] = panda_data[old_name]
         panda_data.pop(old_name)
     return panda_data
 
 
 def _parse_perg_data(filename):
-    """
-    Helper func to parse out only the data, a separate func will parse out metadata
-    :param filename: filename of the pERG file
-    :return: pandas dataframe
-    """
+    # Helper func to parse out only the data, a separate func will parse out metadata
+    # :param filename: filename of the pERG file
+    # :return: pandas dataframe
+
     last_header_idx = -1
     with open(filename, "r") as f:
         data = f.readlines()
         for idx, line in enumerate(data):
             if line.startswith("-------"):
                 last_header_idx = idx
         if last_header_idx == -1:
@@ -81,15 +79,15 @@
 
         data = data[last_header_idx + 1:]
         data = list(filter(lambda x: x.strip("\n") != '', data))
 
         return pd.read_csv(StringIO("\n".join(data)))
 
 
-def parse_perg_to_table(filename=None, reformat_column_names=True):
+def perg_parse_to_table(filename=None, reformat_column_names=True):
     """
     Parse the output of a pERG reading into a dict
 
     :param filename: filename of the pERG data to parse
     :param reformat_column_names: reformat the column names, e.g 'Data Pnt(ms):' -> 'data_pnt_ms'
     :return: dict of data
     """
```

