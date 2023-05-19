# Comparing `tmp/textureminer-0.0.1.tar.gz` & `tmp/textureminer-0.0.2.tar.gz`

## Comparing `textureminer-0.0.1.tar` & `textureminer-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 textureminer-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 textureminer-0.0.1/src/textureminer/__init__.py
--rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 textureminer-0.0.1/src/textureminer/texture_miner.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 textureminer-0.0.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 textureminer-0.0.1/LICENSE
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 textureminer-0.0.1/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 textureminer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 textureminer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 textureminer-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 textureminer-0.0.2/src/textureminer/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 textureminer-0.0.2/src/textureminer/__main__.py
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 textureminer-0.0.2/src/textureminer/texture_miner.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 textureminer-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 textureminer-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 textureminer-0.0.2/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 textureminer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 textureminer-0.0.2/PKG-INFO
```

### Comparing `textureminer-0.0.1/src/textureminer/texture_miner.py` & `textureminer-0.0.2/src/textureminer/texture_miner.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,22 +193,30 @@
         string: path of the scaled textures
     """
 
     if do_merge:
         merge_dirs(path, path)
 
     for subdir, _, files in os.walk(path):
+        print_stylized(
+            "Textures are being filtered..." if do_merge else
+            f"{os.path.basename(subdir).capitalize()} textures are being filtered..."
+        )
+        f.filter(f'{os.path.abspath(subdir)}', ['.png'])
+
+        if scale_factor == 1:
+            continue
+
         if len(files) > 0:
             print_stylized(
                 f"{len(files)} textures are being resized..." if do_merge else
                 f"{len(files)} {os.path.basename(subdir)} textures are being resized..."
             )
 
         for fil in files:
-            f.filter(f'{os.path.abspath(subdir)}', ['.png'])
             image.scale(f"{os.path.abspath(subdir)}/{fil}", scale_factor,
                         scale_factor)
 
     return path
 
 
 def merge_dirs(input_dir: str, output_dir: str):
```

### Comparing `textureminer-0.0.1/.gitignore` & `textureminer-0.0.2/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -155,8 +155,9 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
-output/
+output/
+token.txt
```

### Comparing `textureminer-0.0.1/LICENSE` & `textureminer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textureminer-0.0.1/README.md` & `textureminer-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -33,29 +33,29 @@
 
 
 ### Installation
 
 Use pip to install `texture_miner`.
 
 ```sh
-python3 -m pip install --upgrade texture_miner # TODO: replace with actual package name
+python3 -m pip install --upgrade textureminer
 ```
 
 Install the required libraried as listed on [requirements.txt](./requirements.txt).
 
 ```shell
 python3 -m pip install -r requirements.txt
 ```
 
 ## Usage
 
 To download and scale textures for the most recent stable release do the following.
 
 ```python
-# TODO: add usage examples
+python3 -m textureminer
 ```
 
 
 At a high level, the script follows the following steps.
 1. Download the client `.jar` file for the specified version from Mojang's servers.
 2. Extract the textures from the `.jar` file.
 3. Filter the extracted files, only leaving item and block textures to the specified output directory (default: `~/Downloads/mc-textures`).
```

### Comparing `textureminer-0.0.1/pyproject.toml` & `textureminer-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "textureminer"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="4MBL" },
 ]
 description = "Script that allows you to extract and scale Minecraft's item and block textures."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.11"
```

### Comparing `textureminer-0.0.1/PKG-INFO` & `textureminer-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textureminer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Script that allows you to extract and scale Minecraft's item and block textures.
 Project-URL: Homepage, https://github.com/4MBL/texture-miner
 Project-URL: Bug Tracker, https://github.com/4MBL/texture-miner/issues
 Author: 4MBL
 License: MIT License
         
         Copyright (c) 2023 4MBL
@@ -68,29 +68,29 @@
 
 
 ### Installation
 
 Use pip to install `texture_miner`.
 
 ```sh
-python3 -m pip install --upgrade texture_miner # TODO: replace with actual package name
+python3 -m pip install --upgrade textureminer
 ```
 
 Install the required libraried as listed on [requirements.txt](./requirements.txt).
 
 ```shell
 python3 -m pip install -r requirements.txt
 ```
 
 ## Usage
 
 To download and scale textures for the most recent stable release do the following.
 
 ```python
-# TODO: add usage examples
+python3 -m textureminer
 ```
 
 
 At a high level, the script follows the following steps.
 1. Download the client `.jar` file for the specified version from Mojang's servers.
 2. Extract the textures from the `.jar` file.
 3. Filter the extracted files, only leaving item and block textures to the specified output directory (default: `~/Downloads/mc-textures`).
```

