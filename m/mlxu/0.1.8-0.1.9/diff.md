# Comparing `tmp/mlxu-0.1.8.tar.gz` & `tmp/mlxu-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlxu-0.1.8.tar", last modified: Sun Feb 26 00:29:42 2023, max compression
+gzip compressed data, was "mlxu-0.1.9.tar", last modified: Wed Mar  1 23:20:41 2023, max compression
```

## Comparing `mlxu-0.1.8.tar` & `mlxu-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 young     (1000) young     (1000)        0 2023-02-26 00:29:42.817916 mlxu-0.1.8/
--rw-rw-r--   0 young     (1000) young     (1000)     1067 2023-01-29 05:21:10.000000 mlxu-0.1.8/LICENSE
--rw-rw-r--   0 young     (1000) young     (1000)      411 2023-02-26 00:29:42.817916 mlxu-0.1.8/PKG-INFO
--rw-rw-r--   0 young     (1000) young     (1000)     4444 2023-02-23 00:36:40.000000 mlxu-0.1.8/README.md
-drwxrwxr-x   0 young     (1000) young     (1000)        0 2023-02-26 00:29:42.817916 mlxu-0.1.8/mlxu/
--rw-rw-r--   0 young     (1000) young     (1000)      465 2023-02-26 00:27:30.000000 mlxu-0.1.8/mlxu/__init__.py
--rw-rw-r--   0 young     (1000) young     (1000)     3047 2023-02-23 00:31:40.000000 mlxu-0.1.8/mlxu/config.py
--rw-rw-r--   0 young     (1000) young     (1000)     4350 2023-02-14 02:22:26.000000 mlxu-0.1.8/mlxu/jax_utils.py
--rw-rw-r--   0 young     (1000) young     (1000)     4102 2023-02-14 02:26:00.000000 mlxu-0.1.8/mlxu/logging.py
--rw-rw-r--   0 young     (1000) young     (1000)     1235 2023-02-26 00:27:55.000000 mlxu-0.1.8/mlxu/utils.py
-drwxrwxr-x   0 young     (1000) young     (1000)        0 2023-02-26 00:29:42.817916 mlxu-0.1.8/mlxu.egg-info/
--rw-rw-r--   0 young     (1000) young     (1000)      411 2023-02-26 00:29:42.000000 mlxu-0.1.8/mlxu.egg-info/PKG-INFO
--rw-rw-r--   0 young     (1000) young     (1000)      245 2023-02-26 00:29:42.000000 mlxu-0.1.8/mlxu.egg-info/SOURCES.txt
--rw-rw-r--   0 young     (1000) young     (1000)        1 2023-02-26 00:29:42.000000 mlxu-0.1.8/mlxu.egg-info/dependency_links.txt
--rw-rw-r--   0 young     (1000) young     (1000)       75 2023-02-26 00:29:42.000000 mlxu-0.1.8/mlxu.egg-info/requires.txt
--rw-rw-r--   0 young     (1000) young     (1000)        5 2023-02-26 00:29:42.000000 mlxu-0.1.8/mlxu.egg-info/top_level.txt
--rw-rw-r--   0 young     (1000) young     (1000)       38 2023-02-26 00:29:42.817916 mlxu-0.1.8/setup.cfg
--rw-rw-r--   0 young     (1000) young     (1000)      766 2023-02-26 00:26:13.000000 mlxu-0.1.8/setup.py
+drwxrwxr-x   0 young     (1000) young     (1000)        0 2023-03-01 23:20:41.365430 mlxu-0.1.9/
+-rw-rw-r--   0 young     (1000) young     (1000)     1067 2023-01-29 05:21:10.000000 mlxu-0.1.9/LICENSE
+-rw-rw-r--   0 young     (1000) young     (1000)      411 2023-03-01 23:20:41.365430 mlxu-0.1.9/PKG-INFO
+-rw-rw-r--   0 young     (1000) young     (1000)     4444 2023-02-23 00:36:40.000000 mlxu-0.1.9/README.md
+drwxrwxr-x   0 young     (1000) young     (1000)        0 2023-03-01 23:20:41.365430 mlxu-0.1.9/mlxu/
+-rw-rw-r--   0 young     (1000) young     (1000)      465 2023-02-26 00:27:30.000000 mlxu-0.1.9/mlxu/__init__.py
+-rw-rw-r--   0 young     (1000) young     (1000)     3047 2023-02-23 00:31:40.000000 mlxu-0.1.9/mlxu/config.py
+-rw-rw-r--   0 young     (1000) young     (1000)     4350 2023-02-14 02:22:26.000000 mlxu-0.1.9/mlxu/jax_utils.py
+-rw-rw-r--   0 young     (1000) young     (1000)     4102 2023-02-14 02:26:00.000000 mlxu-0.1.9/mlxu/logging.py
+-rw-rw-r--   0 young     (1000) young     (1000)     1262 2023-03-01 23:19:19.000000 mlxu-0.1.9/mlxu/utils.py
+drwxrwxr-x   0 young     (1000) young     (1000)        0 2023-03-01 23:20:41.365430 mlxu-0.1.9/mlxu.egg-info/
+-rw-rw-r--   0 young     (1000) young     (1000)      411 2023-03-01 23:20:41.000000 mlxu-0.1.9/mlxu.egg-info/PKG-INFO
+-rw-rw-r--   0 young     (1000) young     (1000)      245 2023-03-01 23:20:41.000000 mlxu-0.1.9/mlxu.egg-info/SOURCES.txt
+-rw-rw-r--   0 young     (1000) young     (1000)        1 2023-03-01 23:20:41.000000 mlxu-0.1.9/mlxu.egg-info/dependency_links.txt
+-rw-rw-r--   0 young     (1000) young     (1000)       75 2023-03-01 23:20:41.000000 mlxu-0.1.9/mlxu.egg-info/requires.txt
+-rw-rw-r--   0 young     (1000) young     (1000)        5 2023-03-01 23:20:41.000000 mlxu-0.1.9/mlxu.egg-info/top_level.txt
+-rw-rw-r--   0 young     (1000) young     (1000)       38 2023-03-01 23:20:41.365430 mlxu-0.1.9/setup.cfg
+-rw-rw-r--   0 young     (1000) young     (1000)      766 2023-03-01 23:19:30.000000 mlxu-0.1.9/setup.py
```

### Comparing `mlxu-0.1.8/LICENSE` & `mlxu-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mlxu-0.1.8/README.md` & `mlxu-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mlxu-0.1.8/mlxu/config.py` & `mlxu-0.1.9/mlxu/config.py`

 * *Files identical despite different names*

### Comparing `mlxu-0.1.8/mlxu/jax_utils.py` & `mlxu-0.1.9/mlxu/jax_utils.py`

 * *Files identical despite different names*

### Comparing `mlxu-0.1.8/mlxu/logging.py` & `mlxu-0.1.9/mlxu/logging.py`

 * *Files identical despite different names*

### Comparing `mlxu-0.1.8/mlxu/utils.py` & `mlxu-0.1.9/mlxu/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,18 @@
     def __exit__(self, exc_type, exc_value, exc_tb):
         self._time = time.time() - self._start_time
 
     def __call__(self):
         return self._time
 
 
-def open_file(path, mode='rb'):
+def open_file(path, mode='rb', cache_type='readahead'):
     if path.startswith("gs://"):
         logging.getLogger("fsspec").setLevel(logging.WARNING)
-        return gcsfs.GCSFileSystem().open(path, mode, cache_type='block')
+        return gcsfs.GCSFileSystem().open(path, mode, cache_type=cache_type)
     else:
         return open(path, mode)
 
 
 def save_pickle(obj, path):
     with open_file(path, 'wb') as fout:
         pickle.dump(obj, fout)
```

### Comparing `mlxu-0.1.8/setup.py` & `mlxu-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mlxu',
-    version='0.1.8',
+    version='0.1.9',
     license='MIT',
     description='Machine learning experiment utils.',
     url='https://github.com/young-geng/mlxu',
     packages=find_packages(include=['mlxu']),
     python_requires=">=3.7",
     install_requires=[
         'absl-py',
```

