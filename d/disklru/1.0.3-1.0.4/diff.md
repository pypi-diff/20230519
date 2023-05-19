# Comparing `tmp/disklru-1.0.3.tar.gz` & `tmp/disklru-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disklru-1.0.3.tar", last modified: Fri May 19 01:13:05 2023, max compression
+gzip compressed data, was "disklru-1.0.4.tar", last modified: Fri May 19 01:25:38 2023, max compression
```

## Comparing `disklru-1.0.3.tar` & `disklru-1.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.483499 disklru-1.0.3/
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.476371 disklru-1.0.3/.github/
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.480984 disklru-1.0.3/.github/workflows/
--rw-r--r--   0 niteris    (501) staff       (20)      855 2023-05-18 22:37:02.000000 disklru-1.0.3/.github/workflows/lint.yml
--rw-r--r--   0 niteris    (501) staff       (20)      801 2023-05-18 22:37:02.000000 disklru-1.0.3/.github/workflows/push_macos.yml
--rw-r--r--   0 niteris    (501) staff       (20)      803 2023-05-18 22:37:02.000000 disklru-1.0.3/.github/workflows/push_ubuntu.yml
--rw-r--r--   0 niteris    (501) staff       (20)      800 2023-05-18 22:37:02.000000 disklru-1.0.3/.github/workflows/push_win.yml
--rw-r--r--   0 niteris    (501) staff       (20)     1914 2023-05-18 22:37:02.000000 disklru-1.0.3/.gitignore
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.481643 disklru-1.0.3/.vscode/
--rw-r--r--   0 niteris    (501) staff       (20)     1354 2023-05-18 22:37:02.000000 disklru-1.0.3/.vscode/launch.json
--rw-r--r--   0 niteris    (501) staff       (20)      819 2023-05-18 22:37:02.000000 disklru-1.0.3/.vscode/settings.json
--rw-r--r--   0 niteris    (501) staff       (20)     1109 2023-05-18 22:37:02.000000 disklru-1.0.3/.vscode/tasks.json
--rw-r--r--   0 niteris    (501) staff       (20)     1064 2023-05-18 22:37:02.000000 disklru-1.0.3/LICENSE
--rw-r--r--   0 niteris    (501) staff       (20)      102 2023-05-18 22:37:02.000000 disklru-1.0.3/MANIFEST.in
--rw-r--r--   0 niteris    (501) staff       (20)     1496 2023-05-19 01:13:05.483291 disklru-1.0.3/PKG-INFO
--rw-r--r--   0 niteris    (501) staff       (20)      862 2023-05-18 22:37:02.000000 disklru-1.0.3/README.md
--rwxr-xr-x   0 niteris    (501) staff       (20)      400 2023-05-19 00:59:49.000000 disklru-1.0.3/activate.sh
--rwxr-xr-x   0 niteris    (501) staff       (20)      435 2023-05-18 22:37:02.000000 disklru-1.0.3/lint.sh
--rw-r--r--   0 niteris    (501) staff       (20)     2138 2023-05-18 22:37:02.000000 disklru-1.0.3/make_venv.py
--rw-r--r--   0 niteris    (501) staff       (20)      712 2023-05-19 01:12:28.000000 disklru-1.0.3/pyproject.toml
--rw-r--r--   0 niteris    (501) staff       (20)       47 2023-05-19 01:11:14.000000 disklru-1.0.3/requirements.testing.txt
--rw-r--r--   0 niteris    (501) staff       (20)       38 2023-05-19 01:13:05.483552 disklru-1.0.3/setup.cfg
--rw-r--r--   0 niteris    (501) staff       (20)     1090 2023-05-18 22:37:02.000000 disklru-1.0.3/setup.py
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.476770 disklru-1.0.3/src/
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.482015 disklru-1.0.3/src/disklru/
--rw-r--r--   0 niteris    (501) staff       (20)       92 2023-05-19 01:11:14.000000 disklru-1.0.3/src/disklru/__init__.py
--rw-r--r--   0 niteris    (501) staff       (20)     3641 2023-05-19 01:11:14.000000 disklru-1.0.3/src/disklru/disklru.py
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.482734 disklru-1.0.3/src/disklru.egg-info/
--rw-r--r--   0 niteris    (501) staff       (20)     1496 2023-05-19 01:13:05.000000 disklru-1.0.3/src/disklru.egg-info/PKG-INFO
--rw-r--r--   0 niteris    (501) staff       (20)      543 2023-05-19 01:13:05.000000 disklru-1.0.3/src/disklru.egg-info/SOURCES.txt
--rw-r--r--   0 niteris    (501) staff       (20)        1 2023-05-19 01:13:05.000000 disklru-1.0.3/src/disklru.egg-info/dependency_links.txt
--rw-r--r--   0 niteris    (501) staff       (20)        8 2023-05-19 01:13:05.000000 disklru-1.0.3/src/disklru.egg-info/top_level.txt
-drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.482906 disklru-1.0.3/tests/
--rw-r--r--   0 niteris    (501) staff       (20)     3163 2023-05-19 01:11:27.000000 disklru-1.0.3/tests/test_disklru.py
--rw-r--r--   0 niteris    (501) staff       (20)      498 2023-05-19 01:11:14.000000 disklru-1.0.3/tox.ini
--rwxr-xr-x   0 niteris    (501) staff       (20)      291 2023-05-18 22:37:02.000000 disklru-1.0.3/upload_package.sh
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:25:38.494877 disklru-1.0.4/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:25:38.486332 disklru-1.0.4/.github/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:25:38.491574 disklru-1.0.4/.github/workflows/
+-rw-r--r--   0 niteris    (501) staff       (20)      855 2023-05-18 22:37:02.000000 disklru-1.0.4/.github/workflows/lint.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      801 2023-05-18 22:37:02.000000 disklru-1.0.4/.github/workflows/push_macos.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      803 2023-05-18 22:37:02.000000 disklru-1.0.4/.github/workflows/push_ubuntu.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      800 2023-05-18 22:37:02.000000 disklru-1.0.4/.github/workflows/push_win.yml
+-rw-r--r--   0 niteris    (501) staff       (20)     1914 2023-05-18 22:37:02.000000 disklru-1.0.4/.gitignore
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:25:38.492247 disklru-1.0.4/.vscode/
+-rw-r--r--   0 niteris    (501) staff       (20)     1354 2023-05-18 22:37:02.000000 disklru-1.0.4/.vscode/launch.json
+-rw-r--r--   0 niteris    (501) staff       (20)      819 2023-05-18 22:37:02.000000 disklru-1.0.4/.vscode/settings.json
+-rw-r--r--   0 niteris    (501) staff       (20)     1109 2023-05-18 22:37:02.000000 disklru-1.0.4/.vscode/tasks.json
+-rw-r--r--   0 niteris    (501) staff       (20)     1064 2023-05-18 22:37:02.000000 disklru-1.0.4/LICENSE
+-rw-r--r--   0 niteris    (501) staff       (20)      102 2023-05-18 22:37:02.000000 disklru-1.0.4/MANIFEST.in
+-rw-r--r--   0 niteris    (501) staff       (20)     1496 2023-05-19 01:25:38.494587 disklru-1.0.4/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)      862 2023-05-18 22:37:02.000000 disklru-1.0.4/README.md
+-rwxr-xr-x   0 niteris    (501) staff       (20)      400 2023-05-19 00:59:49.000000 disklru-1.0.4/activate.sh
+-rwxr-xr-x   0 niteris    (501) staff       (20)      435 2023-05-18 22:37:02.000000 disklru-1.0.4/lint.sh
+-rw-r--r--   0 niteris    (501) staff       (20)     2138 2023-05-18 22:37:02.000000 disklru-1.0.4/make_venv.py
+-rw-r--r--   0 niteris    (501) staff       (20)      712 2023-05-19 01:24:45.000000 disklru-1.0.4/pyproject.toml
+-rw-r--r--   0 niteris    (501) staff       (20)       47 2023-05-19 01:11:14.000000 disklru-1.0.4/requirements.testing.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       38 2023-05-19 01:25:38.494939 disklru-1.0.4/setup.cfg
+-rw-r--r--   0 niteris    (501) staff       (20)     1090 2023-05-18 22:37:02.000000 disklru-1.0.4/setup.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:25:38.486701 disklru-1.0.4/src/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:25:38.492830 disklru-1.0.4/src/disklru/
+-rw-r--r--   0 niteris    (501) staff       (20)       92 2023-05-19 01:11:14.000000 disklru-1.0.4/src/disklru/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)     3764 2023-05-19 01:24:38.000000 disklru-1.0.4/src/disklru/disklru.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:25:38.493834 disklru-1.0.4/src/disklru.egg-info/
+-rw-r--r--   0 niteris    (501) staff       (20)     1496 2023-05-19 01:25:38.000000 disklru-1.0.4/src/disklru.egg-info/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)      543 2023-05-19 01:25:38.000000 disklru-1.0.4/src/disklru.egg-info/SOURCES.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        1 2023-05-19 01:25:38.000000 disklru-1.0.4/src/disklru.egg-info/dependency_links.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        8 2023-05-19 01:25:38.000000 disklru-1.0.4/src/disklru.egg-info/top_level.txt
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:25:38.494039 disklru-1.0.4/tests/
+-rw-r--r--   0 niteris    (501) staff       (20)     3163 2023-05-19 01:11:27.000000 disklru-1.0.4/tests/test_disklru.py
+-rw-r--r--   0 niteris    (501) staff       (20)      498 2023-05-19 01:11:14.000000 disklru-1.0.4/tox.ini
+-rwxr-xr-x   0 niteris    (501) staff       (20)      291 2023-05-18 22:37:02.000000 disklru-1.0.4/upload_package.sh
```

### Comparing `disklru-1.0.3/.github/workflows/lint.yml` & `disklru-1.0.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/.github/workflows/push_macos.yml` & `disklru-1.0.4/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/.github/workflows/push_ubuntu.yml` & `disklru-1.0.4/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/.github/workflows/push_win.yml` & `disklru-1.0.4/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/.gitignore` & `disklru-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/.vscode/launch.json` & `disklru-1.0.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/.vscode/settings.json` & `disklru-1.0.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/.vscode/tasks.json` & `disklru-1.0.4/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/LICENSE` & `disklru-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/PKG-INFO` & `disklru-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disklru
-Version: 1.0.3
+Version: 1.0.4
 Summary: Creates a python disk LRU / cache - great for apps that want to save data
 Home-page: https://github.com/zackees/disklru
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `disklru-1.0.3/README.md` & `disklru-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/make_venv.py` & `disklru-1.0.4/make_venv.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/pyproject.toml` & `disklru-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 keywords = ["template-python-cmd"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
 ]
 # Change this with the version number bump.
 # Also make the change in zcmds/version.py
-version = "1.0.3"
+version = "1.0.4"
 
 [tool.ruff]
 line-length = 200
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
```

### Comparing `disklru-1.0.3/setup.py` & `disklru-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/src/disklru/disklru.py` & `disklru-1.0.4/src/disklru/disklru.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 Disk-based LRU cache using SQLite.
 """
 
 import json
 import os
 import sqlite3
+import sys
 from datetime import datetime
 from typing import Any
 
 # pylint: disable=line-too-long
 
 
 class DiskLRUCache:
     """Disk-based LRU cache using SQLite."""
 
     def __init__(self, db_path: str, max_size: str) -> None:
         """Initializes the cache."""
         os.makedirs(os.path.dirname(db_path), exist_ok=True)
+        if not os.path.exists(db_path) and sys.platform != "win32":
+            os.system(f'touch "{db_path}"')
         self.conn = sqlite3.connect(db_path)
         self.closed = False
         self.cursor = self.conn.cursor()
         self.cursor.execute(
             """
             CREATE TABLE IF NOT EXISTS cache (
                 key TEXT PRIMARY KEY,
```

### Comparing `disklru-1.0.3/src/disklru.egg-info/PKG-INFO` & `disklru-1.0.4/src/disklru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disklru
-Version: 1.0.3
+Version: 1.0.4
 Summary: Creates a python disk LRU / cache - great for apps that want to save data
 Home-page: https://github.com/zackees/disklru
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `disklru-1.0.3/src/disklru.egg-info/SOURCES.txt` & `disklru-1.0.4/src/disklru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disklru-1.0.3/tests/test_disklru.py` & `disklru-1.0.4/tests/test_disklru.py`

 * *Files identical despite different names*

