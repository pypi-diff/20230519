# Comparing `tmp/disklru-1.0.2.tar.gz` & `tmp/disklru-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disklru-1.0.2.tar", last modified: Thu May 11 01:43:07 2023, max compression
+gzip compressed data, was "disklru-1.0.3.tar", last modified: Fri May 19 01:13:05 2023, max compression
```

## Comparing `disklru-1.0.2.tar` & `disklru-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.781341 disklru-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.698341 disklru-1.0.2/.github/
-drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.750340 disklru-1.0.2/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-05-10 22:45:22.000000 disklru-1.0.2/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      801 2023-05-10 22:45:22.000000 disklru-1.0.2/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      803 2023-05-10 22:45:22.000000 disklru-1.0.2/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      800 2023-05-10 22:45:22.000000 disklru-1.0.2/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     1914 2023-05-10 22:45:22.000000 disklru-1.0.2/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.754344 disklru-1.0.2/.vscode/
--rw-rw-rw-   0        0        0     1354 2023-05-10 22:45:22.000000 disklru-1.0.2/.vscode/launch.json
--rw-rw-rw-   0        0        0      819 2023-05-10 22:45:22.000000 disklru-1.0.2/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2023-05-10 22:45:22.000000 disklru-1.0.2/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2023-05-10 22:45:22.000000 disklru-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      102 2023-05-10 22:45:22.000000 disklru-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1542 2023-05-11 01:43:07.780341 disklru-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      862 2023-05-10 22:59:34.000000 disklru-1.0.2/README.md
--rw-rw-rw-   0        0        0      415 2023-05-10 22:46:08.000000 disklru-1.0.2/activate.sh
--rw-rw-rw-   0        0        0      435 2023-05-10 22:45:22.000000 disklru-1.0.2/lint.sh
--rw-rw-rw-   0        0        0     2138 2023-05-10 22:45:22.000000 disklru-1.0.2/make_venv.py
--rw-rw-rw-   0        0        0      712 2023-05-11 01:42:54.000000 disklru-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       47 2023-05-10 22:45:22.000000 disklru-1.0.2/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 01:43:07.781341 disklru-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1090 2023-05-10 22:45:22.000000 disklru-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.700342 disklru-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.757341 disklru-1.0.2/src/disklru/
--rw-rw-rw-   0        0        0       92 2023-05-10 22:45:22.000000 disklru-1.0.2/src/disklru/__init__.py
--rw-rw-rw-   0        0        0     3641 2023-05-11 01:42:19.000000 disklru-1.0.2/src/disklru/disklru.py
-drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.778342 disklru-1.0.2/src/disklru.egg-info/
--rw-rw-rw-   0        0        0     1542 2023-05-11 01:43:07.000000 disklru-1.0.2/src/disklru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-05-11 01:43:07.000000 disklru-1.0.2/src/disklru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 01:43:07.000000 disklru-1.0.2/src/disklru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-11 01:43:07.000000 disklru-1.0.2/src/disklru.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.779340 disklru-1.0.2/tests/
--rw-rw-rw-   0        0        0     2943 2023-05-11 01:41:53.000000 disklru-1.0.2/tests/test_disklru.py
--rw-rw-rw-   0        0        0      498 2023-05-10 22:45:22.000000 disklru-1.0.2/tox.ini
--rw-rw-rw-   0        0        0      291 2023-05-10 22:45:22.000000 disklru-1.0.2/upload_package.sh
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.483499 disklru-1.0.3/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.476371 disklru-1.0.3/.github/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.480984 disklru-1.0.3/.github/workflows/
+-rw-r--r--   0 niteris    (501) staff       (20)      855 2023-05-18 22:37:02.000000 disklru-1.0.3/.github/workflows/lint.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      801 2023-05-18 22:37:02.000000 disklru-1.0.3/.github/workflows/push_macos.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      803 2023-05-18 22:37:02.000000 disklru-1.0.3/.github/workflows/push_ubuntu.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      800 2023-05-18 22:37:02.000000 disklru-1.0.3/.github/workflows/push_win.yml
+-rw-r--r--   0 niteris    (501) staff       (20)     1914 2023-05-18 22:37:02.000000 disklru-1.0.3/.gitignore
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.481643 disklru-1.0.3/.vscode/
+-rw-r--r--   0 niteris    (501) staff       (20)     1354 2023-05-18 22:37:02.000000 disklru-1.0.3/.vscode/launch.json
+-rw-r--r--   0 niteris    (501) staff       (20)      819 2023-05-18 22:37:02.000000 disklru-1.0.3/.vscode/settings.json
+-rw-r--r--   0 niteris    (501) staff       (20)     1109 2023-05-18 22:37:02.000000 disklru-1.0.3/.vscode/tasks.json
+-rw-r--r--   0 niteris    (501) staff       (20)     1064 2023-05-18 22:37:02.000000 disklru-1.0.3/LICENSE
+-rw-r--r--   0 niteris    (501) staff       (20)      102 2023-05-18 22:37:02.000000 disklru-1.0.3/MANIFEST.in
+-rw-r--r--   0 niteris    (501) staff       (20)     1496 2023-05-19 01:13:05.483291 disklru-1.0.3/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)      862 2023-05-18 22:37:02.000000 disklru-1.0.3/README.md
+-rwxr-xr-x   0 niteris    (501) staff       (20)      400 2023-05-19 00:59:49.000000 disklru-1.0.3/activate.sh
+-rwxr-xr-x   0 niteris    (501) staff       (20)      435 2023-05-18 22:37:02.000000 disklru-1.0.3/lint.sh
+-rw-r--r--   0 niteris    (501) staff       (20)     2138 2023-05-18 22:37:02.000000 disklru-1.0.3/make_venv.py
+-rw-r--r--   0 niteris    (501) staff       (20)      712 2023-05-19 01:12:28.000000 disklru-1.0.3/pyproject.toml
+-rw-r--r--   0 niteris    (501) staff       (20)       47 2023-05-19 01:11:14.000000 disklru-1.0.3/requirements.testing.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       38 2023-05-19 01:13:05.483552 disklru-1.0.3/setup.cfg
+-rw-r--r--   0 niteris    (501) staff       (20)     1090 2023-05-18 22:37:02.000000 disklru-1.0.3/setup.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.476770 disklru-1.0.3/src/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.482015 disklru-1.0.3/src/disklru/
+-rw-r--r--   0 niteris    (501) staff       (20)       92 2023-05-19 01:11:14.000000 disklru-1.0.3/src/disklru/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)     3641 2023-05-19 01:11:14.000000 disklru-1.0.3/src/disklru/disklru.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.482734 disklru-1.0.3/src/disklru.egg-info/
+-rw-r--r--   0 niteris    (501) staff       (20)     1496 2023-05-19 01:13:05.000000 disklru-1.0.3/src/disklru.egg-info/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)      543 2023-05-19 01:13:05.000000 disklru-1.0.3/src/disklru.egg-info/SOURCES.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        1 2023-05-19 01:13:05.000000 disklru-1.0.3/src/disklru.egg-info/dependency_links.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        8 2023-05-19 01:13:05.000000 disklru-1.0.3/src/disklru.egg-info/top_level.txt
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-19 01:13:05.482906 disklru-1.0.3/tests/
+-rw-r--r--   0 niteris    (501) staff       (20)     3163 2023-05-19 01:11:27.000000 disklru-1.0.3/tests/test_disklru.py
+-rw-r--r--   0 niteris    (501) staff       (20)      498 2023-05-19 01:11:14.000000 disklru-1.0.3/tox.ini
+-rwxr-xr-x   0 niteris    (501) staff       (20)      291 2023-05-18 22:37:02.000000 disklru-1.0.3/upload_package.sh
```

### Comparing `disklru-1.0.2/.github/workflows/lint.yml` & `disklru-1.0.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/.github/workflows/push_macos.yml` & `disklru-1.0.3/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/.github/workflows/push_ubuntu.yml` & `disklru-1.0.3/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/.github/workflows/push_win.yml` & `disklru-1.0.3/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/.gitignore` & `disklru-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/.vscode/launch.json` & `disklru-1.0.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/.vscode/settings.json` & `disklru-1.0.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/.vscode/tasks.json` & `disklru-1.0.3/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/LICENSE` & `disklru-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/PKG-INFO` & `disklru-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1
-Name: disklru
-Version: 1.0.2
-Summary: Creates a python disk LRU / cache - great for apps that want to save data
-Home-page: https://github.com/zackees/disklru
-Maintainer: Zachary Vorhies
-License: BSD 3-Clause License
-Keywords: template-python-cmd
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# disklru
-
-Creates a disk based lru that you can use in your apps.
-
-Useful for caches.
-
-Zero dependency package.
-
-[![Linting](https://github.com/zackees/disklru/actions/workflows/lint.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/lint.yml)
-
-[![MacOS_Tests](https://github.com/zackees/disklru/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_macos.yml)
-[![Ubuntu_Tests](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml)
-[![Win_Tests](https://github.com/zackees/disklru/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_win.yml)
-
-
-# Usage
-
-```python
-LRU_CACHE_FILE = "cache.db"
-MAX_FILES = 4
-cache = DiskLRUCache(LRU_CACHE_FILE, MAX_FILES)
-cache.put("key", "value")
-assert cache.get("key1") == "val"
-cache.clear()
-```
-
-# Windows
-
-This environment requires you to use `git-bash`.
-
-# Linting
-
-Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
+Metadata-Version: 2.1
+Name: disklru
+Version: 1.0.3
+Summary: Creates a python disk LRU / cache - great for apps that want to save data
+Home-page: https://github.com/zackees/disklru
+Maintainer: Zachary Vorhies
+License: BSD 3-Clause License
+Keywords: template-python-cmd
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# disklru
+
+Creates a disk based lru that you can use in your apps.
+
+Useful for caches.
+
+Zero dependency package.
+
+[![Linting](https://github.com/zackees/disklru/actions/workflows/lint.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/lint.yml)
+
+[![MacOS_Tests](https://github.com/zackees/disklru/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_macos.yml)
+[![Ubuntu_Tests](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml)
+[![Win_Tests](https://github.com/zackees/disklru/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_win.yml)
+
+
+# Usage
+
+```python
+LRU_CACHE_FILE = "cache.db"
+MAX_FILES = 4
+cache = DiskLRUCache(LRU_CACHE_FILE, MAX_FILES)
+cache.put("key", "value")
+assert cache.get("key1") == "val"
+cache.clear()
+```
+
+# Windows
+
+This environment requires you to use `git-bash`.
+
+# Linting
+
+Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
```

### Comparing `disklru-1.0.2/README.md` & `disklru-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/make_venv.py` & `disklru-1.0.3/make_venv.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/pyproject.toml` & `disklru-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 keywords = ["template-python-cmd"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
 ]
 # Change this with the version number bump.
 # Also make the change in zcmds/version.py
-version = "1.0.2"
+version = "1.0.3"
 
 [tool.ruff]
 line-length = 200
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
```

### Comparing `disklru-1.0.2/setup.py` & `disklru-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/src/disklru/disklru.py` & `disklru-1.0.3/src/disklru/disklru.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/src/disklru.egg-info/PKG-INFO` & `disklru-1.0.3/src/disklru.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1
-Name: disklru
-Version: 1.0.2
-Summary: Creates a python disk LRU / cache - great for apps that want to save data
-Home-page: https://github.com/zackees/disklru
-Maintainer: Zachary Vorhies
-License: BSD 3-Clause License
-Keywords: template-python-cmd
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# disklru
-
-Creates a disk based lru that you can use in your apps.
-
-Useful for caches.
-
-Zero dependency package.
-
-[![Linting](https://github.com/zackees/disklru/actions/workflows/lint.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/lint.yml)
-
-[![MacOS_Tests](https://github.com/zackees/disklru/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_macos.yml)
-[![Ubuntu_Tests](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml)
-[![Win_Tests](https://github.com/zackees/disklru/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_win.yml)
-
-
-# Usage
-
-```python
-LRU_CACHE_FILE = "cache.db"
-MAX_FILES = 4
-cache = DiskLRUCache(LRU_CACHE_FILE, MAX_FILES)
-cache.put("key", "value")
-assert cache.get("key1") == "val"
-cache.clear()
-```
-
-# Windows
-
-This environment requires you to use `git-bash`.
-
-# Linting
-
-Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
+Metadata-Version: 2.1
+Name: disklru
+Version: 1.0.3
+Summary: Creates a python disk LRU / cache - great for apps that want to save data
+Home-page: https://github.com/zackees/disklru
+Maintainer: Zachary Vorhies
+License: BSD 3-Clause License
+Keywords: template-python-cmd
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# disklru
+
+Creates a disk based lru that you can use in your apps.
+
+Useful for caches.
+
+Zero dependency package.
+
+[![Linting](https://github.com/zackees/disklru/actions/workflows/lint.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/lint.yml)
+
+[![MacOS_Tests](https://github.com/zackees/disklru/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_macos.yml)
+[![Ubuntu_Tests](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml)
+[![Win_Tests](https://github.com/zackees/disklru/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_win.yml)
+
+
+# Usage
+
+```python
+LRU_CACHE_FILE = "cache.db"
+MAX_FILES = 4
+cache = DiskLRUCache(LRU_CACHE_FILE, MAX_FILES)
+cache.put("key", "value")
+assert cache.get("key1") == "val"
+cache.clear()
+```
+
+# Windows
+
+This environment requires you to use `git-bash`.
+
+# Linting
+
+Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
```

### Comparing `disklru-1.0.2/src/disklru.egg-info/SOURCES.txt` & `disklru-1.0.3/src/disklru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disklru-1.0.2/tests/test_disklru.py` & `disklru-1.0.3/tests/test_disklru.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 
 
 class DskLRUTester(unittest.TestCase):
     """Main tester class."""
 
     def setUp(self):
         self.cache = DiskLRUCache(LRU_CACHE_FILE, 4)
-
-    def tearDown(self):
         # Clean up the database file after running each test
         self.cache.clear()
 
+    def tearDown(self):
+        if not self.cache.closed:
+            self.cache.close()
+
     def test_set_and_get(self):
         """Tests setting and getting a value."""
         self.cache.put("key", "value")
         self.assertEqual(self.cache.get("key"), "value")
 
     def test_clear(self):
         """Tests clearing the cache."""
@@ -80,10 +82,15 @@
         self.assertIsNotNone(self.cache.get("key5"))
 
     def test_json(self) -> None:
         """Tests that the cache can store and retrieve JSON objects."""
         self.cache.put_json("key", {"foo": "bar"})
         self.assertEqual(self.cache.get_json("key"), {"foo": "bar"})
 
+    def test_close(self) -> None:
+        """Tests that the cache can be closed."""
+        self.cache.close()
+        self.assertTrue(self.cache.closed)
+
 
 if __name__ == "__main__":
     unittest.main()
```

