# Comparing `tmp/alia-0.2.3.tar.gz` & `tmp/alia-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alia-0.2.3.tar", last modified: Thu May 18 15:43:06 2023, max compression
+gzip compressed data, was "alia-0.2.4.tar", last modified: Fri May 19 20:19:37 2023, max compression
```

## Comparing `alia-0.2.3.tar` & `alia-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-05-18 15:43:06.825529 alia-0.2.3/
--rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.3/LICENSE
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-05-18 15:43:06.825232 alia-0.2.3/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      529 2023-04-20 21:02:49.000000 alia-0.2.3/README.md
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-05-18 15:43:06.823183 alia-0.2.3/alia/
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.3/alia/__init__.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.3/alia/colors.py
--rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.3/alia/df_tools.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    28691 2023-05-18 15:41:40.000000 alia-0.2.3/alia/tools.py
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-05-18 15:43:06.824853 alia-0.2.3/alia.egg-info/
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-05-18 15:43:06.000000 alia-0.2.3/alia.egg-info/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-05-18 15:43:06.000000 alia-0.2.3/alia.egg-info/SOURCES.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-05-18 15:43:06.000000 alia-0.2.3/alia.egg-info/dependency_links.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       94 2023-05-18 15:43:06.000000 alia-0.2.3/alia.egg-info/requires.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-05-18 15:43:06.000000 alia-0.2.3/alia.egg-info/top_level.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-05-18 15:43:06.825616 alia-0.2.3/setup.cfg
--rw-r--r--   0 aliavictor   (502) staff       (20)      926 2023-05-18 15:41:46.000000 alia-0.2.3/setup.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-05-19 20:19:37.927221 alia-0.2.4/
+-rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.4/LICENSE
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-05-19 20:19:37.926918 alia-0.2.4/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      529 2023-04-20 21:02:49.000000 alia-0.2.4/README.md
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-05-19 20:19:37.924497 alia-0.2.4/alia/
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.4/alia/__init__.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.4/alia/colors.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.4/alia/df_tools.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    29221 2023-05-19 20:19:05.000000 alia-0.2.4/alia/tools.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-05-19 20:19:37.926537 alia-0.2.4/alia.egg-info/
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-05-19 20:19:37.000000 alia-0.2.4/alia.egg-info/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-05-19 20:19:37.000000 alia-0.2.4/alia.egg-info/SOURCES.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-05-19 20:19:37.000000 alia-0.2.4/alia.egg-info/dependency_links.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       94 2023-05-19 20:19:37.000000 alia-0.2.4/alia.egg-info/requires.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-05-19 20:19:37.000000 alia-0.2.4/alia.egg-info/top_level.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-05-19 20:19:37.927300 alia-0.2.4/setup.cfg
+-rw-r--r--   0 aliavictor   (502) staff       (20)      926 2023-05-19 20:19:30.000000 alia-0.2.4/setup.py
```

### Comparing `alia-0.2.3/LICENSE` & `alia-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alia-0.2.3/PKG-INFO` & `alia-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.2.3/README.md` & `alia-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `alia-0.2.3/alia/colors.py` & `alia-0.2.4/alia/colors.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.3/alia/df_tools.py` & `alia-0.2.4/alia/df_tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.3/alia/tools.py` & `alia-0.2.4/alia/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -679,15 +679,15 @@
         else:
             return bool(len(obj) == 0 or obj[list(obj.columns)[0]].values[0] == "")
     elif isinstance(obj, list):
         return bool(obj == [])
     elif isinstance(obj, str):
         return bool(obj == "")
     elif isinstance(obj, dict):
-        return bool(len(keys(obj)) == 0)
+        return bool(len(obj.keys()) == 0)
 
 
 def numdict(input_list):
     """Creates a dictionary from a list where the keys are an item's index and the values are the list's items.
 
     Args:
         input_list (list): List of items
@@ -885,25 +885,37 @@
             isinstance(dict_obj[key], str) and nullstr(dict_obj[key])
         ):
             return val
 
     return dict_obj.get(key, val)
 
 
-def filelist(dirpath, raise_err=False):
+def filelist(dirpath, ext=None, prefix=None, raise_err=False):
     """Lists the filenames in the passed directory.
 
     Args:
         dirpath (str): Directory path to reference
+        ext (str): Extension of the files to target
+        prefix (str): Target files that start with this prefix
         raise_err (bool): If False FileNotFoundErrors will fail silently
 
     Returns:
         A list containing all the filenames in the given directory."""
+    if ext and "." not in ext:
+        ext = f".{ext.strip()}"
+
     try:
-        return [i for i in os.listdir(dirpath) if i[0].isalnum()]
+        if ext and prefix:
+            return [i for i in os.listdir(dirpath) if i.startswith(prefix) and i.endswith(ext)]
+        elif ext:
+            return [i for i in os.listdir(dirpath) if i.endswith(ext)]
+        elif prefix:
+            return [i for i in os.listdir(dirpath) if i.startswith(prefix)]
+        else:
+            return [i for i in os.listdir(dirpath) if i[0].isalnum()]
     except FileNotFoundError:
         if raise_err:
             raise FileNotFoundError
         else:
             red("<b>Can't locate directory</b>")
             return None
```

### Comparing `alia-0.2.3/alia.egg-info/PKG-INFO` & `alia-0.2.4/alia.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

