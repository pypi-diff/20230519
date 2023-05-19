# Comparing `tmp/minari-0.3.0.tar.gz` & `tmp/minari-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minari-0.3.0.tar", last modified: Wed May 17 14:59:57 2023, max compression
+gzip compressed data, was "minari-0.3.0b0.tar", last modified: Wed May 17 14:20:16 2023, max compression
```

## Comparing `minari-0.3.0.tar` & `minari-0.3.0b0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:59:57.741129 minari-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-05-17 14:59:45.000000 minari-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-17 14:59:57.741129 minari-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-17 14:59:45.000000 minari-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:59:57.737129 minari-0.3.0/minari/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-17 14:59:45.000000 minari-0.3.0/minari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-17 14:59:45.000000 minari-0.3.0/minari/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:59:57.737129 minari-0.3.0/minari/data_collector/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-17 14:59:45.000000 minari-0.3.0/minari/data_collector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:59:57.737129 minari-0.3.0/minari/data_collector/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-17 14:59:45.000000 minari-0.3.0/minari/data_collector/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-17 14:59:45.000000 minari-0.3.0/minari/data_collector/callbacks/episode_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-17 14:59:45.000000 minari-0.3.0/minari/data_collector/callbacks/step_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-05-17 14:59:45.000000 minari-0.3.0/minari/data_collector/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:59:57.737129 minari-0.3.0/minari/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:59:45.000000 minari-0.3.0/minari/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-17 14:59:45.000000 minari-0.3.0/minari/dataset/minari_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-17 14:59:45.000000 minari-0.3.0/minari/dataset/minari_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:59:57.741129 minari-0.3.0/minari/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 14:59:45.000000 minari-0.3.0/minari/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-17 14:59:45.000000 minari-0.3.0/minari/storage/datasets_root_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-05-17 14:59:45.000000 minari-0.3.0/minari/storage/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-17 14:59:45.000000 minari-0.3.0/minari/storage/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-17 14:59:45.000000 minari-0.3.0/minari/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:59:57.737129 minari-0.3.0/minari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-17 14:59:57.000000 minari-0.3.0/minari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-17 14:59:57.000000 minari-0.3.0/minari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:59:57.000000 minari-0.3.0/minari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-17 14:59:57.000000 minari-0.3.0/minari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-17 14:59:57.000000 minari-0.3.0/minari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 14:59:57.000000 minari-0.3.0/minari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-17 14:59:45.000000 minari-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:59:57.741129 minari-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-17 14:59:45.000000 minari-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:59:57.741129 minari-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-05-17 14:59:45.000000 minari-0.3.0/tests/test_dataset_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 14:59:45.000000 minari-0.3.0/tests/test_dataset_download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.510837 minari-0.3.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-05-17 14:20:00.000000 minari-0.3.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-17 14:20:16.510837 minari-0.3.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-17 14:20:00.000000 minari-0.3.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.502837 minari-0.3.0b0/minari/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/minari/data_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/data_collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/minari/data_collector/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/data_collector/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/data_collector/callbacks/episode_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/data_collector/callbacks/step_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/data_collector/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/minari/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/dataset/minari_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/dataset/minari_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/minari/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/storage/datasets_root_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/storage/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/storage/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-17 14:20:00.000000 minari-0.3.0b0/minari/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/minari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 14:20:16.000000 minari-0.3.0b0/minari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-17 14:20:00.000000 minari-0.3.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:20:16.510837 minari-0.3.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-17 14:20:00.000000 minari-0.3.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.506837 minari-0.3.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-05-17 14:20:00.000000 minari-0.3.0b0/tests/test_dataset_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 14:20:00.000000 minari-0.3.0b0/tests/test_dataset_download.py
```

### Comparing `minari-0.3.0/LICENSE` & `minari-0.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/PKG-INFO` & `minari-0.3.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minari
-Version: 0.3.0
+Version: 0.3.0b0
 Summary: A standard format for offline reinforcement learning datasets, with popular reference datasets and related utilities.
 Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
 Project-URL: Homepage, https://farama.org
 Project-URL: Repository, https://github.com/Farama-Foundation/Minari
 Project-URL: Documentation, https://minari.farama.org/
 Project-URL: Bug Report, https://github.com/Farama-Foundation/Minari/issues
```

### Comparing `minari-0.3.0/README.md` & `minari-0.3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/minari/__init__.py` & `minari-0.3.0b0/minari/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     "load_dataset",
     "combine_datasets",
     "create_dataset_from_buffers",
     "create_dataset_from_collector_env",
     "split_dataset",
 ]
 
-__version__ = "0.3.0"
+__version__ = "0.3.0b"
```

### Comparing `minari-0.3.0/minari/cli.py` & `minari-0.3.0b0/minari/cli.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/minari/data_collector/callbacks/episode_metadata.py` & `minari-0.3.0b0/minari/data_collector/callbacks/episode_metadata.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/minari/data_collector/callbacks/step_data.py` & `minari-0.3.0b0/minari/data_collector/callbacks/step_data.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/minari/data_collector/data_collector.py` & `minari-0.3.0b0/minari/data_collector/data_collector.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/minari/dataset/minari_dataset.py` & `minari-0.3.0b0/minari/dataset/minari_dataset.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/minari/dataset/minari_storage.py` & `minari-0.3.0b0/minari/dataset/minari_storage.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/minari/storage/hosting.py` & `minari-0.3.0b0/minari/storage/hosting.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/minari/storage/local.py` & `minari-0.3.0b0/minari/storage/local.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/minari/utils.py` & `minari-0.3.0b0/minari/utils.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/minari.egg-info/PKG-INFO` & `minari-0.3.0b0/minari.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minari
-Version: 0.3.0
+Version: 0.3.0b0
 Summary: A standard format for offline reinforcement learning datasets, with popular reference datasets and related utilities.
 Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
 Project-URL: Homepage, https://farama.org
 Project-URL: Repository, https://github.com/Farama-Foundation/Minari
 Project-URL: Documentation, https://minari.farama.org/
 Project-URL: Bug Report, https://github.com/Farama-Foundation/Minari/issues
```

### Comparing `minari-0.3.0/minari.egg-info/SOURCES.txt` & `minari-0.3.0b0/minari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/pyproject.toml` & `minari-0.3.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/setup.py` & `minari-0.3.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/tests/test_dataset_creation.py` & `minari-0.3.0b0/tests/test_dataset_creation.py`

 * *Files identical despite different names*

### Comparing `minari-0.3.0/tests/test_dataset_download.py` & `minari-0.3.0b0/tests/test_dataset_download.py`

 * *Files identical despite different names*

