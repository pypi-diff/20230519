# Comparing `tmp/lgtm-lint-1.0.1.tar.gz` & `tmp/lgtm-lint-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lgtm-lint-1.0.1.tar", last modified: Wed May 17 02:12:53 2023, max compression
+gzip compressed data, was "lgtm-lint-1.0.2.tar", last modified: Fri May 19 17:06:45 2023, max compression
```

## Comparing `lgtm-lint-1.0.1.tar` & `lgtm-lint-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:12:53.407793 lgtm-lint-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-17 02:12:40.000000 lgtm-lint-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-17 02:12:53.403793 lgtm-lint-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-17 02:12:40.000000 lgtm-lint-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-17 02:12:40.000000 lgtm-lint-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 02:12:53.407793 lgtm-lint-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:12:53.399793 lgtm-lint-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:12:53.403793 lgtm-lint-1.0.1/src/lgtm_lint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 02:12:40.000000 lgtm-lint-1.0.1/src/lgtm_lint/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2834 2023-05-17 02:12:40.000000 lgtm-lint-1.0.1/src/lgtm_lint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:12:53.403793 lgtm-lint-1.0.1/src/lgtm_lint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-17 02:12:53.000000 lgtm-lint-1.0.1/src/lgtm_lint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-17 02:12:53.000000 lgtm-lint-1.0.1/src/lgtm_lint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 02:12:53.000000 lgtm-lint-1.0.1/src/lgtm_lint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 02:12:53.000000 lgtm-lint-1.0.1/src/lgtm_lint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 02:12:53.000000 lgtm-lint-1.0.1/src/lgtm_lint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:45.734916 lgtm-lint-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-19 17:06:34.000000 lgtm-lint-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-19 17:06:45.734916 lgtm-lint-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-19 17:06:34.000000 lgtm-lint-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-19 17:06:34.000000 lgtm-lint-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 17:06:45.734916 lgtm-lint-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:45.734916 lgtm-lint-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:45.734916 lgtm-lint-1.0.2/src/lgtm_lint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:34.000000 lgtm-lint-1.0.2/src/lgtm_lint/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2864 2023-05-19 17:06:34.000000 lgtm-lint-1.0.2/src/lgtm_lint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:45.734916 lgtm-lint-1.0.2/src/lgtm_lint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-19 17:06:45.000000 lgtm-lint-1.0.2/src/lgtm_lint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-19 17:06:45.000000 lgtm-lint-1.0.2/src/lgtm_lint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:06:45.000000 lgtm-lint-1.0.2/src/lgtm_lint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 17:06:45.000000 lgtm-lint-1.0.2/src/lgtm_lint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 17:06:45.000000 lgtm-lint-1.0.2/src/lgtm_lint.egg-info/top_level.txt
```

### Comparing `lgtm-lint-1.0.1/LICENSE` & `lgtm-lint-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lgtm-lint-1.0.1/PKG-INFO` & `lgtm-lint-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lgtm-lint
-Version: 1.0.1
+Version: 1.0.2
 Summary: A fully featured 'Looks good to me!' linter.
 Author-email: Paul Maxwell <maxwellpaulm@gmail.com>, Zach Spar <zachspar@gmail.com>
 Project-URL: Homepage, https://github.com/maxwellpaulm/lgtm-lint
 Project-URL: Bug Tracker, https://github.com/maxwellpaulm/lgtm-lint/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
@@ -14,24 +14,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/lgtm-lint.svg)](https://badge.fury.io/py/lgtm-lint)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lgtm-lint?style=plastic)
+ [![License: Unlicense](https://img.shields.io/badge/license-Unlicense-blue.svg)](http://unlicense.org/)
+
 # LGTM Linter
 Looks good to me! This is a satirical "linter" that doesn't actually assert or check anything. Linters have become so picky and opinionated that we thought it might be refreshing to have one that is happy with your code just the way it is!
 
-## Local Python Install
-You can install this package locally by running the following from project root:
+
+## Python Install
+You can install this package via PyPI with the following command:
 ```bash
-pip install -e .
+pip install lgtm-lint
 ```
 This will automatically add `lgtm-lint` to your path.
 
+
 ## Legacy Install
 Just run the following:
 ```bash
 ./legacy_install.sh
 ```
 This will install the script in your user bin. Also, Python3 is required to run the linter.
```

### Comparing `lgtm-lint-1.0.1/pyproject.toml` & `lgtm-lint-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lgtm-lint"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Paul Maxwell", email="maxwellpaulm@gmail.com" },
   { name="Zach Spar", email="zachspar@gmail.com" },
 ]
 description = "A fully featured 'Looks good to me!' linter."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `lgtm-lint-1.0.1/src/lgtm_lint/__main__.py` & `lgtm-lint-1.0.2/src/lgtm_lint/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,89 +1,93 @@
 #!/usr/bin/env python3
 
-import sys
-import time
 import glob
-import os
 import math
+import os
+import sys
+import time
 
 
 def progress_bar(
-        iteration: int, 
-        total: int, 
-        prefix: str = '', 
-        suffix: str = '', 
-        decimals: int = 1, 
-        length: int = 100, 
-        fill: str = '█', 
-        print_end: str = "\r"
-    ):
+    iteration: int,
+    total: int,
+    prefix: str = "",
+    suffix: str = "",
+    decimals: int = 1,
+    length: int = 100,
+    fill: str = "█",
+    print_end: str = "\r",
+):
     """
     Call in a loop to create terminal progress bar
     @params:
         iteration   - Required  : current iteration (Int)
         total       - Required  : total iterations (Int)
         prefix      - Optional  : prefix string (Str)
         suffix      - Optional  : suffix string (Str)
         decimals    - Optional  : positive number of decimals in percent complete (Int)
         length      - Optional  : character length of bar (Int)
         fill        - Optional  : bar fill character (Str)
         print_end   - Optional  : end character (e.g. "\r", "\r\n") (Str)
     """
     percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
     filled_length = int(length * iteration // total)
-    bar = fill * filled_length + '-' * (length - filled_length)
-    print(f'\r{prefix} |{bar}| {percent}% {suffix}', end = print_end)
-    if iteration == total: 
+    bar = fill * filled_length + "-" * (length - filled_length)
+    print(f"\r{prefix} |{bar}| {percent}% {suffix}", end=print_end)
+    if iteration == total:
         print()
 
 
 def main():
     """Main function and entry point."""
     # check python version
     if sys.version_info < (3, 7):
         print("Python 3.7 or later is required.")
         sys.exit(1)
 
-
     if len(sys.argv) < 2:
         print("Please provide a path to lint. Usage: lgtm_lint <path>")
         sys.exit(1)
         # run linting
 
     lint_paths = sys.argv[1:]
-    print(f'Expanding linting paths: {lint_paths}')
+    print(f"Expanding linting paths: {lint_paths}")
     lint_files = []
     for lint_path in lint_paths:
         lint_files.extend([f for f in glob.glob(lint_path, recursive=True) if os.path.isfile(f)])
 
     if len(lint_files) == 0:
-        print('No files found to lint.')
+        print("No files found to lint.")
         sys.exit(1)
 
-    print(f'Found {len(lint_files)} files to lint.')
-    print('Linting files...')
+    print(f"Found {len(lint_files)} files to lint.")
+    print("Linting files...")
 
     # Initial call to print 0% progress
     items = list(range(0, 57))
     items_len = len(items)
-    step_size = math.ceil(items_len/len(lint_files))
+    step_size = math.ceil(items_len / len(lint_files))
     max_char_len = max([len(f) for f in lint_files])
     done_msg = f"Done!{' ' * max_char_len}"
 
-    progress_bar(iteration=0, total=items_len, prefix='Progress:', suffix='Complete', length=50)
+    progress_bar(iteration=0, total=items_len, prefix="Progress:", suffix="Complete", length=50)
     for i, item in enumerate(items):
         time.sleep(0.1)
-        file = lint_files[min(math.floor(i/step_size), len(lint_files) - 1)]
+        file = lint_files[min(math.floor(i / step_size), len(lint_files) - 1)]
         message = f"Linting {file}{' ' * (max_char_len - len(file))}"
-        progress_bar(iteration=i + 1, total=items_len, prefix='Progress:', suffix=message if i != (items_len-1) else done_msg, length=50)
+        progress_bar(
+            iteration=i + 1,
+            total=items_len,
+            prefix="Progress:",
+            suffix=message if i != (items_len - 1) else done_msg,
+            length=50,
+        )
 
-    print('Summary:')
+    print("Summary:")
     for file in lint_files:
-        print(f'\t{file}\t\U00002705')
+        print(f"\t\U00002705\t{file}")
 
-    print('\nLooks good to me! \U0001F44D')
+    print("\nLooks good to me! \U0001F44D")
 
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `lgtm-lint-1.0.1/src/lgtm_lint.egg-info/PKG-INFO` & `lgtm-lint-1.0.2/src/lgtm_lint.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lgtm-lint
-Version: 1.0.1
+Version: 1.0.2
 Summary: A fully featured 'Looks good to me!' linter.
 Author-email: Paul Maxwell <maxwellpaulm@gmail.com>, Zach Spar <zachspar@gmail.com>
 Project-URL: Homepage, https://github.com/maxwellpaulm/lgtm-lint
 Project-URL: Bug Tracker, https://github.com/maxwellpaulm/lgtm-lint/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
@@ -14,24 +14,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/lgtm-lint.svg)](https://badge.fury.io/py/lgtm-lint)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lgtm-lint?style=plastic)
+ [![License: Unlicense](https://img.shields.io/badge/license-Unlicense-blue.svg)](http://unlicense.org/)
+
 # LGTM Linter
 Looks good to me! This is a satirical "linter" that doesn't actually assert or check anything. Linters have become so picky and opinionated that we thought it might be refreshing to have one that is happy with your code just the way it is!
 
-## Local Python Install
-You can install this package locally by running the following from project root:
+
+## Python Install
+You can install this package via PyPI with the following command:
 ```bash
-pip install -e .
+pip install lgtm-lint
 ```
 This will automatically add `lgtm-lint` to your path.
 
+
 ## Legacy Install
 Just run the following:
 ```bash
 ./legacy_install.sh
 ```
 This will install the script in your user bin. Also, Python3 is required to run the linter.
```

