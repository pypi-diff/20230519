# Comparing `tmp/find_old_large_files-0.4.3.tar.gz` & `tmp/find_old_large_files-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find_old_large_files-0.4.3.tar", last modified: Fri May 19 21:47:06 2023, max compression
+gzip compressed data, was "find_old_large_files-0.4.4.tar", last modified: Fri May 19 21:51:22 2023, max compression
```

## Comparing `find_old_large_files-0.4.3.tar` & `find_old_large_files-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:47:06.733206 find_old_large_files-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 21:46:46.000000 find_old_large_files-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:47:06.733206 find_old_large_files-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 21:46:46.000000 find_old_large_files-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:47:06.733206 find_old_large_files-0.4.3/find_old_large_files/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 21:46:46.000000 find_old_large_files-0.4.3/find_old_large_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-19 21:46:46.000000 find_old_large_files-0.4.3/find_old_large_files/find_old_large_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:47:06.733206 find_old_large_files-0.4.3/find_old_large_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:47:06.000000 find_old_large_files-0.4.3/find_old_large_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 21:47:06.000000 find_old_large_files-0.4.3/find_old_large_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:47:06.000000 find_old_large_files-0.4.3/find_old_large_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 21:47:06.000000 find_old_large_files-0.4.3/find_old_large_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 21:47:06.000000 find_old_large_files-0.4.3/find_old_large_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 21:47:06.000000 find_old_large_files-0.4.3/find_old_large_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:47:06.733206 find_old_large_files-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 21:46:46.000000 find_old_large_files-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:51:22.039332 find_old_large_files-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 21:51:05.000000 find_old_large_files-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:51:22.039332 find_old_large_files-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 21:51:05.000000 find_old_large_files-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:51:22.039332 find_old_large_files-0.4.4/find_old_large_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 21:51:05.000000 find_old_large_files-0.4.4/find_old_large_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-19 21:51:05.000000 find_old_large_files-0.4.4/find_old_large_files/find_old_large_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:51:22.039332 find_old_large_files-0.4.4/find_old_large_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 21:51:22.000000 find_old_large_files-0.4.4/find_old_large_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:51:22.039332 find_old_large_files-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 21:51:05.000000 find_old_large_files-0.4.4/setup.py
```

### Comparing `find_old_large_files-0.4.3/LICENSE` & `find_old_large_files-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.4.3/PKG-INFO` & `find_old_large_files-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find_old_large_files
-Version: 0.4.3
+Version: 0.4.4
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.4.3/README.md` & `find_old_large_files-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.4.3/find_old_large_files/find_old_large_files.py` & `find_old_large_files-0.4.4/find_old_large_files/find_old_large_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,20 +70,23 @@
                     logging.info('Moved file to trash: %s', file_path)
                 except OSError as e:  # Catch specifically the OSError
                     logging.error('Error moving file: %s', e)
                 pbar.update()
         logging.info('Finished moving files')
 
 def main():
-    parser = argparse.ArgumentParser(description='Find old and large files')
-    parser.add_argument('dir_path', type=str, default='/Users/username/Documents', nargs='?', help='Directory to scan')
-    parser.add_argument('--size_limit', type=int, default=200, help='File size limit in bytes')
-    parser.add_argument('--days_limit', type=int, default=180, help='File age limit in days')
-    parser.add_argument('--excluded_extensions', nargs='*', default=['.pdf', '.docx'], help='File extensions to exclude')
-    parser.add_argument('--trash_dir', type=str, default='/Users/username/trash', help='Directory to move files to')
+    home = str(Path.home())
+
+    parser = argparse.ArgumentParser(description="Find and remove large, old files.")
+    parser.add_argument("--size", type=int, default=100, help="File size limit in MB")
+    parser.add_argument("--days", type=int, default=365, help="File age limit in days")
+    parser.add_argument("--dir", type=str, default=home, help="Directory to scan")
+    parser.add_argument("--exclude", type=str, nargs='*', default=['.docx', '.xlsx'], help="File extensions to exclude")
+    parser.add_argument("--trash", type=str, default=os.path.join(home, 'trash'), help="Directory to move files to")
+
     args = parser.parse_args()
 
     scanner = FileScanner(args.dir_path, args.size_limit, args.days_limit, args.excluded_extensions, args.trash_dir)
 
     scanner.scan_files()
     print(f"Total size to be moved to trash: {scanner.total_size_in_gb():.2f} GB")
```

### Comparing `find_old_large_files-0.4.3/find_old_large_files.egg-info/PKG-INFO` & `find_old_large_files-0.4.4/find_old_large_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find-old-large-files
-Version: 0.4.3
+Version: 0.4.4
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.4.3/setup.py` & `find_old_large_files-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="find_old_large_files",
-    version="0.4.3",  # Increment the version here
+    version="0.4.4",  # Increment the version here
     packages=find_packages(),
     install_requires=["tqdm"],
     entry_points={
         'console_scripts': [
             'find_old_large_files=find_old_large_files:run',
         ],
     },
```

