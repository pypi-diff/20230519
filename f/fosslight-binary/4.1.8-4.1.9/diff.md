# Comparing `tmp/fosslight_binary-4.1.8.tar.gz` & `tmp/fosslight_binary-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fosslight_binary-4.1.8.tar", last modified: Wed Sep  7 09:04:55 2022, max compression
+gzip compressed data, was "dist/fosslight_binary-4.1.9.tar", last modified: Thu Sep  8 01:53:16 2022, max compression
```

## Comparing `fosslight_binary-4.1.8.tar` & `fosslight_binary-4.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       59 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1305 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      134 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       92 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1889 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/src/fosslight_binary/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/src/fosslight_binary/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4119 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/src/fosslight_binary/_binary.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5585 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/src/fosslight_binary/_binary_dao.py
--rw-r--r--   0 runner    (1001) docker     (116)     1178 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/src/fosslight_binary/_help.py
--rw-r--r--   0 runner    (1001) docker     (116)     7720 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/src/fosslight_binary/_jar_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    10268 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/src/fosslight_binary/binary_analysis.py
--rw-r--r--   0 runner    (1001) docker     (116)     1828 2022-09-07 09:04:44.000000 fosslight_binary-4.1.8/src/fosslight_binary/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/src/fosslight_binary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/src/fosslight_binary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      568 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/src/fosslight_binary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/src/fosslight_binary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      150 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/src/fosslight_binary.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      266 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/src/fosslight_binary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-09-07 09:04:55.000000 fosslight_binary-4.1.8/src/fosslight_binary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1305 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      134 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       92 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1889 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/src/fosslight_binary/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/src/fosslight_binary/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4119 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/src/fosslight_binary/_binary.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5585 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/src/fosslight_binary/_binary_dao.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1178 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/src/fosslight_binary/_help.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7720 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/src/fosslight_binary/_jar_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    10268 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/src/fosslight_binary/binary_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1801 2022-09-08 01:53:06.000000 fosslight_binary-4.1.9/src/fosslight_binary/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/src/fosslight_binary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2174 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/src/fosslight_binary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      568 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/src/fosslight_binary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/src/fosslight_binary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      150 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/src/fosslight_binary.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      266 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/src/fosslight_binary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2022-09-08 01:53:16.000000 fosslight_binary-4.1.9/src/fosslight_binary.egg-info/top_level.txt
```

### Comparing `fosslight_binary-4.1.8/LICENSE` & `fosslight_binary-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_binary-4.1.8/PKG-INFO` & `fosslight_binary-4.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_binary
-Version: 4.1.8
+Version: 4.1.9
 Summary: FOSSLight Binary Scanner
 Home-page: https://github.com/fosslight/fosslight_binary_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_binary_scanner
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

### Comparing `fosslight_binary-4.1.8/README.md` & `fosslight_binary-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_binary-4.1.8/setup.py` & `fosslight_binary-4.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('requirements.txt', 'r', 'utf-8') as f:
     install_requires = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_binary',
-        version='4.1.8',
+        version='4.1.9',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Binary Scanner',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_binary-4.1.8/src/fosslight_binary/_binary.py` & `fosslight_binary-4.1.9/src/fosslight_binary/_binary.py`

 * *Files identical despite different names*

### Comparing `fosslight_binary-4.1.8/src/fosslight_binary/_binary_dao.py` & `fosslight_binary-4.1.9/src/fosslight_binary/_binary_dao.py`

 * *Files identical despite different names*

### Comparing `fosslight_binary-4.1.8/src/fosslight_binary/_help.py` & `fosslight_binary-4.1.9/src/fosslight_binary/_help.py`

 * *Files identical despite different names*

### Comparing `fosslight_binary-4.1.8/src/fosslight_binary/_jar_analysis.py` & `fosslight_binary-4.1.9/src/fosslight_binary/_jar_analysis.py`

 * *Files identical despite different names*

### Comparing `fosslight_binary-4.1.8/src/fosslight_binary/binary_analysis.py` & `fosslight_binary-4.1.9/src/fosslight_binary/binary_analysis.py`

 * *Files identical despite different names*

### Comparing `fosslight_binary-4.1.8/src/fosslight_binary/cli.py` & `fosslight_binary-4.1.9/src/fosslight_binary/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
     if args.version:    # -v option
         print_package_version(_PKG_NAME, "FOSSLight Binary Scanner Version:")
         sys.exit(0)
 
     if args.path:   # -p option
         path_to_find_bin = args.path
-        if not path_to_find_bin:
-            path_to_find_bin = os.getcwd()
+    else:
+        path_to_find_bin = os.getcwd()
 
     if args.output:  # -o option
         output_dir = args.output
 
     if args.dburl:  # -d option
         db_url = args.dburl
```

### Comparing `fosslight_binary-4.1.8/src/fosslight_binary.egg-info/PKG-INFO` & `fosslight_binary-4.1.9/src/fosslight_binary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-binary
-Version: 4.1.8
+Version: 4.1.9
 Summary: FOSSLight Binary Scanner
 Home-page: https://github.com/fosslight/fosslight_binary_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_binary_scanner
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

### Comparing `fosslight_binary-4.1.8/src/fosslight_binary.egg-info/SOURCES.txt` & `fosslight_binary-4.1.9/src/fosslight_binary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

