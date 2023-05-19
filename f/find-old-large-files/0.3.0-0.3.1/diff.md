# Comparing `tmp/find_old_large_files-0.3.0.tar.gz` & `tmp/find_old_large_files-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find_old_large_files-0.3.0.tar", last modified: Fri May 19 20:50:40 2023, max compression
+gzip compressed data, was "find_old_large_files-0.3.1.tar", last modified: Fri May 19 21:03:26 2023, max compression
```

## Comparing `find_old_large_files-0.3.0.tar` & `find_old_large_files-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:40.549920 find_old_large_files-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 20:50:19.000000 find_old_large_files-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 20:50:40.549920 find_old_large_files-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 20:50:19.000000 find_old_large_files-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:40.549920 find_old_large_files-0.3.0/find_old_large_files/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 20:50:19.000000 find_old_large_files-0.3.0/find_old_large_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-19 20:50:19.000000 find_old_large_files-0.3.0/find_old_large_files/find_old_large_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:40.549920 find_old_large_files-0.3.0/find_old_large_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:50:40.549920 find_old_large_files-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 20:50:19.000000 find_old_large_files-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:03:26.171678 find_old_large_files-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 21:03:05.000000 find_old_large_files-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:03:26.171678 find_old_large_files-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 21:03:05.000000 find_old_large_files-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:03:26.171678 find_old_large_files-0.3.1/find_old_large_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 21:03:05.000000 find_old_large_files-0.3.1/find_old_large_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-19 21:03:05.000000 find_old_large_files-0.3.1/find_old_large_files/find_old_large_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:03:26.171678 find_old_large_files-0.3.1/find_old_large_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:03:26.000000 find_old_large_files-0.3.1/find_old_large_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 21:03:26.000000 find_old_large_files-0.3.1/find_old_large_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:03:26.000000 find_old_large_files-0.3.1/find_old_large_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 21:03:26.000000 find_old_large_files-0.3.1/find_old_large_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 21:03:26.000000 find_old_large_files-0.3.1/find_old_large_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 21:03:26.000000 find_old_large_files-0.3.1/find_old_large_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:03:26.171678 find_old_large_files-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 21:03:05.000000 find_old_large_files-0.3.1/setup.py
```

### Comparing `find_old_large_files-0.3.0/LICENSE` & `find_old_large_files-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.3.0/PKG-INFO` & `find_old_large_files-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find_old_large_files
-Version: 0.3.0
+Version: 0.3.1
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.3.0/README.md` & `find_old_large_files-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.3.0/find_old_large_files/find_old_large_files.py` & `find_old_large_files-0.3.1/find_old_large_files/find_old_large_files.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import time
 import argparse
 import logging
 import concurrent.futures
 from pathlib import Path
-from tqdm import tqdm
+from tqdm import tqdm, trange
+from time import sleep
+import itertools
 
 class FileScanner:
     def __init__(self, dir_path, size_limit, days_limit, excluded_extensions, trash_dir):
         self.dir_path = Path(dir_path)
         self.size_limit = size_limit
         self.days_limit = days_limit
         self.excluded_extensions = set(excluded_extensions)
@@ -20,35 +22,32 @@
                             format='%(asctime)s - %(levelname)s - %(message)s')
         logging.info('Initialized FileScanner with dir_path: %s, size_limit: %s, days_limit: %s, excluded_extensions: %s, trash_dir: %s',
                      dir_path, size_limit, days_limit, excluded_extensions, trash_dir)
 
     @staticmethod
     def file_age_in_days(file_path):
         return (time.time() - file_path.stat().st_mtime) / (60*60*24)
-
-    def count_files(self):
-        return sum(1 for _ in self.scan_files())
-
+    
     def scan_files(self):
         for entry in self.dir_path.rglob('*'):
             if entry.is_file():
                 yield entry
 
-    def process_file(self, file_path, file_handler, pbar):
+    def process_file(self, file_path, pbar):
         try:
             if (file_path.stat().st_size > self.size_limit and
                 self.file_age_in_days(file_path) > self.days_limit and
                 file_path.suffix not in self.excluded_extensions):
                 self.files_to_move.append(file_path)
                 logging.info('Added file to move: %s', file_path)
-                if file_handler is not None:
-                    file_handler(file_path)
+                return file_path
         except FileNotFoundError:
             logging.error('File not found: %s', file_path)
-        pbar.update()
+        finally:
+            pbar.update()
 
     def total_size_in_gb(self):
         total_size = sum(file_path.stat().st_size for file_path in self.files_to_move)
         return total_size / (1024 * 1024 * 1024)  # Convert bytes to gigabytes
 
     def move_files_to_trash(self):
         self.trash_dir.mkdir(parents=True, exist_ok=True)
@@ -58,41 +57,43 @@
                     file_path.rename(self.trash_dir / file_path.name)
                     logging.info('Moved file to trash: %s', file_path)
                 except OSError as e:
                     logging.error('Error moving file: %s', e)
                 pbar.update()
         logging.info('Completed moving files to trash')
 
-    def print_file(self, file_path):
-        size_in_mb = file_path.stat().st_size / (1024 * 1024)
-        if size_in_mb < 1024:
-            print(f"Old, large file: {file_path} Size: {size_in_mb:.2f} MB")
-            logging.info('Old, large file: %s Size: %.2f MB', file_path, size_in_mb)
-        else:
-            size_in_gb = size_in_mb / 1024
-            print(f"Old, large file: {file_path} Size: {size_in_gb:.2f} GB")
-            logging.info('Old, large file: %s Size: %.2f GB', file_path, size_in_gb)
-
 def main():
     home = str(Path.home())
 
     parser = argparse.ArgumentParser(description="Find and remove large, old files.")
     parser.add_argument("--size", type=int, default=100, help="File size limit in MB")
     parser.add_argument("--days", type=int, default=365, help="File age limit in days")
     parser.add_argument("--dir", type=str, default=home, help="Directory to scan")
     parser.add_argument("--exclude", type=str, nargs='*', default=['.docx', '.xlsx'], help="File extensions to exclude")
     parser.add_argument("--trash", type=str, default=os.path.join(home, 'trash'), help="Directory to move files to")
 
     args = parser.parse_args()
     size_limit = args.size * 1024 * 1024  # Convert size from MB to bytes
 
     scanner = FileScanner(args.dir, size_limit, args.days, args.exclude, args.trash)
-    with tqdm(total=scanner.count_files(), desc='Scanning files', ncols=70) as pbar:
+    
+    spinner = itertools.cycle(['-', '/', '|', '\\'])
+    
+    print("Starting the file scanning process... ", end='')
+    for _ in range(10):  # arbitrary delay for the loading animation
+        print(next(spinner), end='\r')
+        sleep(0.1)
+
+    with tqdm(total=sum(1 for _ in scanner.scan_files()), desc='Scanning files', ncols=70) as pbar:
         with concurrent.futures.ThreadPoolExecutor() as executor:
-            futures = [executor.submit(scanner.process_file, file_path, scanner.print_file, pbar) for file_path in scanner.scan_files()]
-            concurrent.futures.wait(futures)
+            futures = [executor.submit(scanner.process_file, file_path, pbar) for file_path in scanner.scan_files()]
+            for future in concurrent.futures.as_completed(futures):
+                file = future.result()
+                if file:
+                    print(f"Old, large file: {file} Size: {file.stat().st_size / (1024 * 1024):.2f} MB")
+
     print("Total size to be moved to trash: {:.2f} GB".format(scanner.total_size_in_gb()))
-    input("Press enter to move these files to trash...")
-    scanner.move_files_to_trash()
+    if input("Press enter to move these files to trash...") == '':
+        scanner.move_files_to_trash()
 
 if __name__ == "__main__":
     main()
```

### Comparing `find_old_large_files-0.3.0/find_old_large_files.egg-info/PKG-INFO` & `find_old_large_files-0.3.1/find_old_large_files.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find-old-large-files
-Version: 0.3.0
+Version: 0.3.1
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.3.0/setup.py` & `find_old_large_files-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="find_old_large_files",
-    version="0.3.0",  # Increment the version here
+    version="0.3.1",  # Increment the version here
     packages=find_packages(),
     install_requires=["tqdm"],
     entry_points={
         'console_scripts': [
             'find_old_large_files=find_old_large_files:run',
         ],
     },
```

