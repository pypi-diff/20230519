# Comparing `tmp/find_old_large_files-0.2.5.tar.gz` & `tmp/find_old_large_files-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find_old_large_files-0.2.5.tar", last modified: Fri May 19 16:12:40 2023, max compression
+gzip compressed data, was "find_old_large_files-0.3.0.tar", last modified: Fri May 19 20:50:40 2023, max compression
```

## Comparing `find_old_large_files-0.2.5.tar` & `find_old_large_files-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:40.877810 find_old_large_files-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 16:12:21.000000 find_old_large_files-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 16:12:40.877810 find_old_large_files-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 16:12:21.000000 find_old_large_files-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:40.873810 find_old_large_files-0.2.5/find_old_large_files/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 16:12:21.000000 find_old_large_files-0.2.5/find_old_large_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-19 16:12:21.000000 find_old_large_files-0.2.5/find_old_large_files/find_old_large_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:40.877810 find_old_large_files-0.2.5/find_old_large_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:12:40.877810 find_old_large_files-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 16:12:21.000000 find_old_large_files-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:40.549920 find_old_large_files-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 20:50:19.000000 find_old_large_files-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 20:50:40.549920 find_old_large_files-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 20:50:19.000000 find_old_large_files-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:40.549920 find_old_large_files-0.3.0/find_old_large_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 20:50:19.000000 find_old_large_files-0.3.0/find_old_large_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-19 20:50:19.000000 find_old_large_files-0.3.0/find_old_large_files/find_old_large_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:40.549920 find_old_large_files-0.3.0/find_old_large_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 20:50:40.000000 find_old_large_files-0.3.0/find_old_large_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:50:40.549920 find_old_large_files-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 20:50:19.000000 find_old_large_files-0.3.0/setup.py
```

### Comparing `find_old_large_files-0.2.5/LICENSE` & `find_old_large_files-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.2.5/PKG-INFO` & `find_old_large_files-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find_old_large_files
-Version: 0.2.5
+Version: 0.3.0
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.2.5/README.md` & `find_old_large_files-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.2.5/find_old_large_files/find_old_large_files.py` & `find_old_large_files-0.3.0/find_old_large_files/find_old_large_files.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,81 +4,70 @@
 import logging
 import concurrent.futures
 from pathlib import Path
 from tqdm import tqdm
 
 class FileScanner:
     def __init__(self, dir_path, size_limit, days_limit, excluded_extensions, trash_dir):
-        self.dir_path = dir_path
+        self.dir_path = Path(dir_path)
         self.size_limit = size_limit
         self.days_limit = days_limit
-        self.excluded_extensions = excluded_extensions
-        self.trash_dir = trash_dir
-        self.files_to_move = []  # Store the files to be moved
-
-        # Set up logging
-        logging.basicConfig(filename=os.path.join(self.trash_dir, 'file_scanner.log'), 
-                            level=logging.INFO,
+        self.excluded_extensions = set(excluded_extensions)
+        self.trash_dir = Path(trash_dir)
+        self.files_to_move = []
+
+        logging.basicConfig(filename=str(self.trash_dir / 'file_scanner.log'), 
+                            level=os.environ.get('LOGGING_LEVEL', logging.INFO),
                             format='%(asctime)s - %(levelname)s - %(message)s')
         logging.info('Initialized FileScanner with dir_path: %s, size_limit: %s, days_limit: %s, excluded_extensions: %s, trash_dir: %s',
                      dir_path, size_limit, days_limit, excluded_extensions, trash_dir)
 
     @staticmethod
     def file_age_in_days(file_path):
-        return (time.time() - os.path.getmtime(file_path)) / (60*60*24)
+        return (time.time() - file_path.stat().st_mtime) / (60*60*24)
 
     def count_files(self):
-        count = 0
-        for _, _, filenames in os.walk(self.dir_path):
-            count += len(filenames)
-        logging.info('Total files in dir_path: %s', count)
-        return count
-
-    def scan_files(self, file_handler=None):
-        num_files = self.count_files()
-        with tqdm(total=num_files, desc='Scanning files', ncols=70) as pbar:
-            with concurrent.futures.ThreadPoolExecutor() as executor:
-                futures = []
-                for foldername, subfolders, filenames in os.walk(self.dir_path):
-                    for filename in filenames:
-                        file_path = os.path.join(foldername, filename)
-                        futures.append(executor.submit(self.process_file, file_path, file_handler, pbar))
-                concurrent.futures.wait(futures)
+        return sum(1 for _ in self.scan_files())
+
+    def scan_files(self):
+        for entry in self.dir_path.rglob('*'):
+            if entry.is_file():
+                yield entry
 
     def process_file(self, file_path, file_handler, pbar):
         try:
-            if (os.path.getsize(file_path) > self.size_limit and
+            if (file_path.stat().st_size > self.size_limit and
                 self.file_age_in_days(file_path) > self.days_limit and
-                not Path(file_path).suffix in self.excluded_extensions):
-                self.files_to_move.append(file_path)  # Add to files to be moved
+                file_path.suffix not in self.excluded_extensions):
+                self.files_to_move.append(file_path)
                 logging.info('Added file to move: %s', file_path)
                 if file_handler is not None:
                     file_handler(file_path)
         except FileNotFoundError:
             logging.error('File not found: %s', file_path)
         pbar.update()
 
     def total_size_in_gb(self):
-        total_size = sum(os.path.getsize(file_path) for file_path in self.files_to_move)
+        total_size = sum(file_path.stat().st_size for file_path in self.files_to_move)
         return total_size / (1024 * 1024 * 1024)  # Convert bytes to gigabytes
 
     def move_files_to_trash(self):
-        os.makedirs(self.trash_dir, exist_ok=True)
+        self.trash_dir.mkdir(parents=True, exist_ok=True)
         with tqdm(total=len(self.files_to_move), desc='Moving files', ncols=70) as pbar:
             for file_path in self.files_to_move:
                 try:
-                    os.rename(file_path, os.path.join(self.trash_dir, os.path.basename(file_path)))
+                    file_path.rename(self.trash_dir / file_path.name)
                     logging.info('Moved file to trash: %s', file_path)
-                except Exception as e:
+                except OSError as e:
                     logging.error('Error moving file: %s', e)
                 pbar.update()
         logging.info('Completed moving files to trash')
 
     def print_file(self, file_path):
-        size_in_mb = os.path.getsize(file_path) / (1024 * 1024)
+        size_in_mb = file_path.stat().st_size / (1024 * 1024)
         if size_in_mb < 1024:
             print(f"Old, large file: {file_path} Size: {size_in_mb:.2f} MB")
             logging.info('Old, large file: %s Size: %.2f MB', file_path, size_in_mb)
         else:
             size_in_gb = size_in_mb / 1024
             print(f"Old, large file: {file_path} Size: {size_in_gb:.2f} GB")
             logging.info('Old, large file: %s Size: %.2f GB', file_path, size_in_gb)
@@ -93,15 +82,17 @@
     parser.add_argument("--exclude", type=str, nargs='*', default=['.docx', '.xlsx'], help="File extensions to exclude")
     parser.add_argument("--trash", type=str, default=os.path.join(home, 'trash'), help="Directory to move files to")
 
     args = parser.parse_args()
     size_limit = args.size * 1024 * 1024  # Convert size from MB to bytes
 
     scanner = FileScanner(args.dir, size_limit, args.days, args.exclude, args.trash)
-    scanner.scan_files(scanner.print_file)
+    with tqdm(total=scanner.count_files(), desc='Scanning files', ncols=70) as pbar:
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            futures = [executor.submit(scanner.process_file, file_path, scanner.print_file, pbar) for file_path in scanner.scan_files()]
+            concurrent.futures.wait(futures)
     print("Total size to be moved to trash: {:.2f} GB".format(scanner.total_size_in_gb()))
     input("Press enter to move these files to trash...")
-    scanner.move_files_to_trash()  # Move files to trash
-
+    scanner.move_files_to_trash()
 
 if __name__ == "__main__":
     main()
```

### Comparing `find_old_large_files-0.2.5/find_old_large_files.egg-info/PKG-INFO` & `find_old_large_files-0.3.0/find_old_large_files.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find-old-large-files
-Version: 0.2.5
+Version: 0.3.0
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.2.5/setup.py` & `find_old_large_files-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="find_old_large_files",
-    version="0.2.5",  # Increment the version here
+    version="0.3.0",  # Increment the version here
     packages=find_packages(),
     install_requires=["tqdm"],
     entry_points={
         'console_scripts': [
             'find_old_large_files=find_old_large_files:run',
         ],
     },
```

