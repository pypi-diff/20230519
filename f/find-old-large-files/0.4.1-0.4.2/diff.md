# Comparing `tmp/find_old_large_files-0.4.1.tar.gz` & `tmp/find_old_large_files-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find_old_large_files-0.4.1.tar", last modified: Fri May 19 21:29:21 2023, max compression
+gzip compressed data, was "find_old_large_files-0.4.2.tar", last modified: Fri May 19 21:37:03 2023, max compression
```

## Comparing `find_old_large_files-0.4.1.tar` & `find_old_large_files-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:21.054741 find_old_large_files-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 21:29:03.000000 find_old_large_files-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:29:21.054741 find_old_large_files-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 21:29:03.000000 find_old_large_files-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:21.054741 find_old_large_files-0.4.1/find_old_large_files/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 21:29:03.000000 find_old_large_files-0.4.1/find_old_large_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-19 21:29:03.000000 find_old_large_files-0.4.1/find_old_large_files/find_old_large_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:21.054741 find_old_large_files-0.4.1/find_old_large_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:29:21.000000 find_old_large_files-0.4.1/find_old_large_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 21:29:21.000000 find_old_large_files-0.4.1/find_old_large_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:29:21.000000 find_old_large_files-0.4.1/find_old_large_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 21:29:21.000000 find_old_large_files-0.4.1/find_old_large_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 21:29:21.000000 find_old_large_files-0.4.1/find_old_large_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 21:29:21.000000 find_old_large_files-0.4.1/find_old_large_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:29:21.054741 find_old_large_files-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 21:29:03.000000 find_old_large_files-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:37:03.719135 find_old_large_files-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 21:36:46.000000 find_old_large_files-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:37:03.719135 find_old_large_files-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 21:36:46.000000 find_old_large_files-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:37:03.719135 find_old_large_files-0.4.2/find_old_large_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 21:36:46.000000 find_old_large_files-0.4.2/find_old_large_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-19 21:36:46.000000 find_old_large_files-0.4.2/find_old_large_files/find_old_large_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:37:03.719135 find_old_large_files-0.4.2/find_old_large_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 21:37:03.000000 find_old_large_files-0.4.2/find_old_large_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 21:37:03.000000 find_old_large_files-0.4.2/find_old_large_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:37:03.000000 find_old_large_files-0.4.2/find_old_large_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 21:37:03.000000 find_old_large_files-0.4.2/find_old_large_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 21:37:03.000000 find_old_large_files-0.4.2/find_old_large_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 21:37:03.000000 find_old_large_files-0.4.2/find_old_large_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:37:03.719135 find_old_large_files-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 21:36:46.000000 find_old_large_files-0.4.2/setup.py
```

### Comparing `find_old_large_files-0.4.1/LICENSE` & `find_old_large_files-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.4.1/PKG-INFO` & `find_old_large_files-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find_old_large_files
-Version: 0.4.1
+Version: 0.4.2
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.4.1/README.md` & `find_old_large_files-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.4.1/find_old_large_files/find_old_large_files.py` & `find_old_large_files-0.4.2/find_old_large_files/find_old_large_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,94 @@
 import os
 import time
 import argparse
 import logging
-from pathlib import Path
 import concurrent.futures
+from pathlib import Path
 from tqdm import tqdm
 
 class FileScanner:
     def __init__(self, dir_path, size_limit, days_limit, excluded_extensions, trash_dir):
         self.dir_path = dir_path
         self.size_limit = size_limit
         self.days_limit = days_limit
-        self.excluded_extensions = set(excluded_extensions)  # Changed from list to set
+        self.excluded_extensions = set(excluded_extensions)  # Convert to set for performance
         self.trash_dir = trash_dir
-        self.files_to_move = []
+        self.files_to_move = []  # Store the files to be moved
 
+        # Set up logging
         logging.basicConfig(filename=os.path.join(self.trash_dir, 'file_scanner.log'), 
                             level=logging.INFO,
                             format='%(asctime)s - %(levelname)s - %(message)s')
         logging.info('Initialized FileScanner with dir_path: %s, size_limit: %s, days_limit: %s, excluded_extensions: %s, trash_dir: %s',
                      dir_path, size_limit, days_limit, excluded_extensions, trash_dir)
 
     @staticmethod
     def file_age_in_days(file_path):
         return (time.time() - os.path.getmtime(file_path)) / (60*60*24)
 
-    def count_files(self):
-        for _, _, filenames in os.scandir(self.dir_path):
-            yield len(filenames)
+    def gen_files(self, path=None):
+        if path is None:
+            path = self.dir_path
+
+        for entry in os.scandir(path):
+            if entry.is_dir(follow_symlinks=False):
+                yield from self.gen_files(entry.path)
+            else:
+                yield entry
 
     def scan_files(self, file_handler=None):
         print("Starting the file scanning process... This may take a while, please hang tight.")
-        num_files = sum(self.count_files())
-        with tqdm(total=num_files, desc='Scanning files', ncols=70) as pbar:
+        with tqdm(total=sum(1 for _ in self.gen_files()), desc='Scanning files', ncols=70) as pbar:
             with concurrent.futures.ThreadPoolExecutor() as executor:
-                futures = []
-                for entry in os.scandir(self.dir_path):
-                    if entry.is_file():
-                        futures.append(executor.submit(self.process_file, entry.path, file_handler, pbar))
-                concurrent.futures.wait(futures)
+                futures = [executor.submit(self.process_file, entry.path, file_handler, pbar) for entry in self.gen_files()]
+            concurrent.futures.wait(futures)
 
     def process_file(self, file_path, file_handler, pbar):
         try:
             if (os.path.getsize(file_path) > self.size_limit and
                 self.file_age_in_days(file_path) > self.days_limit and
-                Path(file_path).suffix not in self.excluded_extensions):
-                self.files_to_move.append(file_path)
+                not Path(file_path).suffix in self.excluded_extensions):
+                self.files_to_move.append(file_path)  # Add to files to be moved
                 logging.info('Added file to move: %s', file_path)
                 if file_handler is not None:
                     file_handler(file_path)
         except FileNotFoundError:
             logging.error('File not found: %s', file_path)
         pbar.update()
 
     def total_size_in_gb(self):
         total_size = sum(os.path.getsize(file_path) for file_path in self.files_to_move)
-        return total_size / (1024 * 1024 * 1024)
+        return total_size / (1024 * 1024 * 1024)  # Convert bytes to gigabytes
 
     def move_files_to_trash(self):
         os.makedirs(self.trash_dir, exist_ok=True)
         with tqdm(total=len(self.files_to_move), desc='Moving files', ncols=70) as pbar:
             for file_path in self.files_to_move:
                 try:
                     os.rename(file_path, os.path.join(self.trash_dir, os.path.basename(file_path)))
                     logging.info('Moved file to trash: %s', file_path)
-                except OSError as e:  # Specific Exception Handling
+                except OSError as e:  # Catch specifically the OSError
                     logging.error('Error moving file: %s', e)
                 pbar.update()
-        logging.info('Completed moving files to trash')
-
-    def print_file(self, file_path):
-        size_in_mb = os.path.getsize(file_path) / (1024 * 1024)
-        if size_in_mb < 1024:
-            print(f"Old, large file: {file_path} Size: {size_in_mb:.2f} MB")
-            logging.info('Old, large file: %s Size: %.2f MB', file_path, size_in_mb)
-        else:
-            size_in_gb = size_in_mb / 1024
-            print(f"Old, large file: {file_path} Size: {size_in_gb:.2f} GB")
-            logging.info('Old, large file: %s Size: %.2f GB', file_path, size_in_gb)
+        logging.info('Finished moving files')
 
 def main():
-    home = str(Path.home())
-
-    parser = argparse.ArgumentParser(description="Find and remove large, old files.")
-    parser.add_argument("--size", type=int, default=100, help="File size limit in MB")
-    parser.add_argument("--days", type=int, default=365, help="File age limit in days")
-    parser.add_argument("--dir", type=str, default=home, help="Directory to scan")
-    parser.add_argument("--exclude", type=str, nargs='*', default=['.docx', '.xlsx'], help="File extensions to exclude")
-    parser.add_argument("--trash", type=str, default=os.path.join(home, 'trash'), help="Directory to move files to")
-
+    parser = argparse.ArgumentParser(description='Find old and large files that are hogging disk space')
+    parser.add_argument('dir_path', type=str, help='Directory to scan')
+    parser.add_argument('--size_limit', type=int, default=1e9, help='File size limit in bytes')
+    parser.add_argument('--days_limit', type=int, default=180, help='File age limit in days')
+    parser.add_argument('--excluded_extensions', nargs='*', default=['.mp4', '.jpg'], help='File extensions to exclude')
+    parser.add_argument('--trash_dir', type=str, default='/tmp/trash', help='Directory to move files to')
     args = parser.parse_args()
-    size_limit = args.size * 1024 * 1024  # Convert size from MB to bytes
 
-    scanner = FileScanner(args.dir, size_limit, args.days, args.exclude, args.trash)
+    scanner = FileScanner(args.dir_path, args.size_limit, args.days_limit, args.excluded_extensions, args.trash_dir)
+
     scanner.scan_files(scanner.print_file)
-    # ...
-    print("Total size to be moved to trash: {:.2f} GB".format(scanner.total_size_in_gb()))
-    user_input = input("Do you want to move these files to trash? (Y/N): ")
-    if user_input.lower() == 'y':
+    print(f"Total size to be moved to trash: {scanner.total_size_in_gb():.2f} GB")
+
+    choice = input("Do you want to move these files to trash? (yes/no): ")
+    if choice.lower() == 'yes':
         scanner.move_files_to_trash()
-    else:
-        print("Files were not moved to trash.")
-# ...
 
 if __name__ == "__main__":
     main()
```

### Comparing `find_old_large_files-0.4.1/find_old_large_files.egg-info/PKG-INFO` & `find_old_large_files-0.4.2/find_old_large_files.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find-old-large-files
-Version: 0.4.1
+Version: 0.4.2
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.4.1/setup.py` & `find_old_large_files-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="find_old_large_files",
-    version="0.4.1",  # Increment the version here
+    version="0.4.2",  # Increment the version here
     packages=find_packages(),
     install_requires=["tqdm"],
     entry_points={
         'console_scripts': [
             'find_old_large_files=find_old_large_files:run',
         ],
     },
```

