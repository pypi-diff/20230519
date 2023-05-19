# Comparing `tmp/genki-wave-0.5.1.tar.gz` & `tmp/genki-wave-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genki-wave-0.5.1.tar", last modified: Fri Apr 28 14:03:30 2023, max compression
+gzip compressed data, was "genki-wave-0.5.2.tar", last modified: Fri May 19 16:03:12 2023, max compression
```

## Comparing `genki-wave-0.5.1.tar` & `genki-wave-0.5.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-04-28 14:03:30.385147 genki-wave-0.5.1/
--rw-r--r--   0 egill      (501) staff       (20)     1079 2022-05-09 10:31:46.000000 genki-wave-0.5.1/LICENSE
--rw-r--r--   0 egill      (501) staff       (20)     4012 2023-04-28 14:03:30.384994 genki-wave-0.5.1/PKG-INFO
--rw-r--r--   0 egill      (501) staff       (20)     3408 2022-05-09 10:31:46.000000 genki-wave-0.5.1/README.md
-drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-04-28 14:03:30.382039 genki-wave-0.5.1/examples/
--rw-r--r--   0 egill      (501) staff       (20)        0 2022-05-09 10:31:46.000000 genki-wave-0.5.1/examples/__init__.py
--rw-r--r--   0 egill      (501) staff       (20)       82 2022-05-09 10:31:46.000000 genki-wave-0.5.1/examples/discover_wave.py
--rw-r--r--   0 egill      (501) staff       (20)     1838 2023-04-28 14:02:22.000000 genki-wave-0.5.1/examples/run_async.py
--rw-r--r--   0 egill      (501) staff       (20)     6221 2023-04-27 12:53:23.000000 genki-wave-0.5.1/examples/run_midi.py
--rw-r--r--   0 egill      (501) staff       (20)     2295 2023-04-27 12:53:23.000000 genki-wave-0.5.1/examples/run_threads.py
-drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-04-28 14:03:30.383193 genki-wave-0.5.1/genki_wave/
--rw-r--r--   0 egill      (501) staff       (20)        0 2022-05-09 10:31:46.000000 genki-wave-0.5.1/genki_wave/__init__.py
--rw-r--r--   0 egill      (501) staff       (20)     9335 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/asyncio_runner.py
--rw-r--r--   0 egill      (501) staff       (20)     3973 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/callbacks.py
--rw-r--r--   0 egill      (501) staff       (20)      100 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/constants.py
-drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-04-28 14:03:30.384824 genki-wave-0.5.1/genki_wave/data/
--rw-r--r--   0 egill      (501) staff       (20)      274 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/data/__init__.py
--rw-r--r--   0 egill      (501) staff       (20)     1412 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/data/enums.py
--rw-r--r--   0 egill      (501) staff       (20)    12462 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/data/organization.py
--rw-r--r--   0 egill      (501) staff       (20)     1909 2023-04-27 12:53:23.000000 genki-wave-0.5.1/genki_wave/data/points.py
--rw-r--r--   0 egill      (501) staff       (20)      621 2022-05-09 10:31:46.000000 genki-wave-0.5.1/genki_wave/data/structures.py
--rw-r--r--   0 egill      (501) staff       (20)     1904 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/data/writing.py
--rw-r--r--   0 egill      (501) staff       (20)      649 2023-04-27 12:53:23.000000 genki-wave-0.5.1/genki_wave/discover.py
--rw-r--r--   0 egill      (501) staff       (20)     6230 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/protocols.py
--rw-r--r--   0 egill      (501) staff       (20)     4328 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/threading_runner.py
--rw-r--r--   0 egill      (501) staff       (20)     1324 2023-04-27 12:53:23.000000 genki-wave-0.5.1/genki_wave/utils.py
-drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-04-28 14:03:30.383908 genki-wave-0.5.1/genki_wave.egg-info/
--rw-r--r--   0 egill      (501) staff       (20)     4012 2023-04-28 14:03:30.000000 genki-wave-0.5.1/genki_wave.egg-info/PKG-INFO
--rw-r--r--   0 egill      (501) staff       (20)      675 2023-04-28 14:03:30.000000 genki-wave-0.5.1/genki_wave.egg-info/SOURCES.txt
--rw-r--r--   0 egill      (501) staff       (20)        1 2023-04-28 14:03:30.000000 genki-wave-0.5.1/genki_wave.egg-info/dependency_links.txt
--rw-r--r--   0 egill      (501) staff       (20)       37 2023-04-28 14:03:30.000000 genki-wave-0.5.1/genki_wave.egg-info/requires.txt
--rw-r--r--   0 egill      (501) staff       (20)       20 2023-04-28 14:03:30.000000 genki-wave-0.5.1/genki_wave.egg-info/top_level.txt
--rw-r--r--   0 egill      (501) staff       (20)       38 2023-04-28 14:03:30.385207 genki-wave-0.5.1/setup.cfg
--rw-r--r--   0 egill      (501) staff       (20)      919 2023-04-28 14:03:02.000000 genki-wave-0.5.1/setup.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-05-19 16:03:12.385884 genki-wave-0.5.2/
+-rw-r--r--   0 egill      (501) staff       (20)     1079 2022-05-09 10:31:46.000000 genki-wave-0.5.2/LICENSE
+-rw-r--r--   0 egill      (501) staff       (20)     4012 2023-05-19 16:03:12.385698 genki-wave-0.5.2/PKG-INFO
+-rw-r--r--   0 egill      (501) staff       (20)     3408 2022-05-09 10:31:46.000000 genki-wave-0.5.2/README.md
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-05-19 16:03:12.381626 genki-wave-0.5.2/examples/
+-rw-r--r--   0 egill      (501) staff       (20)        0 2022-05-09 10:31:46.000000 genki-wave-0.5.2/examples/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)       82 2022-05-09 10:31:46.000000 genki-wave-0.5.2/examples/discover_wave.py
+-rw-r--r--   0 egill      (501) staff       (20)     1838 2023-04-28 14:02:22.000000 genki-wave-0.5.2/examples/run_async.py
+-rw-r--r--   0 egill      (501) staff       (20)     6221 2023-04-27 12:53:23.000000 genki-wave-0.5.2/examples/run_midi.py
+-rw-r--r--   0 egill      (501) staff       (20)     2295 2023-04-27 12:53:23.000000 genki-wave-0.5.2/examples/run_threads.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-05-19 16:03:12.383607 genki-wave-0.5.2/genki_wave/
+-rw-r--r--   0 egill      (501) staff       (20)        0 2022-05-09 10:31:46.000000 genki-wave-0.5.2/genki_wave/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)     9335 2023-04-28 14:02:22.000000 genki-wave-0.5.2/genki_wave/asyncio_runner.py
+-rw-r--r--   0 egill      (501) staff       (20)     3973 2023-04-28 14:02:22.000000 genki-wave-0.5.2/genki_wave/callbacks.py
+-rw-r--r--   0 egill      (501) staff       (20)      100 2023-04-28 14:02:22.000000 genki-wave-0.5.2/genki_wave/constants.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-05-19 16:03:12.385453 genki-wave-0.5.2/genki_wave/data/
+-rw-r--r--   0 egill      (501) staff       (20)      274 2023-04-28 14:02:22.000000 genki-wave-0.5.2/genki_wave/data/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)     1412 2023-04-28 14:02:22.000000 genki-wave-0.5.2/genki_wave/data/enums.py
+-rw-r--r--   0 egill      (501) staff       (20)    12462 2023-04-28 14:02:22.000000 genki-wave-0.5.2/genki_wave/data/organization.py
+-rw-r--r--   0 egill      (501) staff       (20)     1909 2023-04-27 12:53:23.000000 genki-wave-0.5.2/genki_wave/data/points.py
+-rw-r--r--   0 egill      (501) staff       (20)      621 2022-05-09 10:31:46.000000 genki-wave-0.5.2/genki_wave/data/structures.py
+-rw-r--r--   0 egill      (501) staff       (20)     1904 2023-04-28 14:02:22.000000 genki-wave-0.5.2/genki_wave/data/writing.py
+-rw-r--r--   0 egill      (501) staff       (20)      649 2023-04-27 12:53:23.000000 genki-wave-0.5.2/genki_wave/discover.py
+-rw-r--r--   0 egill      (501) staff       (20)     6230 2023-04-28 14:02:22.000000 genki-wave-0.5.2/genki_wave/protocols.py
+-rw-r--r--   0 egill      (501) staff       (20)     4328 2023-04-28 14:02:22.000000 genki-wave-0.5.2/genki_wave/threading_runner.py
+-rw-r--r--   0 egill      (501) staff       (20)     1324 2023-04-27 12:53:23.000000 genki-wave-0.5.2/genki_wave/utils.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-05-19 16:03:12.384402 genki-wave-0.5.2/genki_wave.egg-info/
+-rw-r--r--   0 egill      (501) staff       (20)     4012 2023-05-19 16:03:12.000000 genki-wave-0.5.2/genki_wave.egg-info/PKG-INFO
+-rw-r--r--   0 egill      (501) staff       (20)      675 2023-05-19 16:03:12.000000 genki-wave-0.5.2/genki_wave.egg-info/SOURCES.txt
+-rw-r--r--   0 egill      (501) staff       (20)        1 2023-05-19 16:03:12.000000 genki-wave-0.5.2/genki_wave.egg-info/dependency_links.txt
+-rw-r--r--   0 egill      (501) staff       (20)       37 2023-05-19 16:03:12.000000 genki-wave-0.5.2/genki_wave.egg-info/requires.txt
+-rw-r--r--   0 egill      (501) staff       (20)       20 2023-05-19 16:03:12.000000 genki-wave-0.5.2/genki_wave.egg-info/top_level.txt
+-rw-r--r--   0 egill      (501) staff       (20)       38 2023-05-19 16:03:12.385936 genki-wave-0.5.2/setup.cfg
+-rw-r--r--   0 egill      (501) staff       (20)      919 2023-05-19 16:03:03.000000 genki-wave-0.5.2/setup.py
```

### Comparing `genki-wave-0.5.1/LICENSE` & `genki-wave-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/PKG-INFO` & `genki-wave-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genki-wave
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python API for Wave by Genki
 Home-page: https://github.com/genkiinstruments/genki-wave
 Author: Robert Torfason
 Author-email: robert@genkiinstruments.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genki-wave-0.5.1/README.md` & `genki-wave-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/examples/run_async.py` & `genki-wave-0.5.2/examples/run_async.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/examples/run_midi.py` & `genki-wave-0.5.2/examples/run_midi.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/examples/run_threads.py` & `genki-wave-0.5.2/examples/run_threads.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/asyncio_runner.py` & `genki-wave-0.5.2/genki_wave/asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/callbacks.py` & `genki-wave-0.5.2/genki_wave/callbacks.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/data/enums.py` & `genki-wave-0.5.2/genki_wave/data/enums.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/data/organization.py` & `genki-wave-0.5.2/genki_wave/data/organization.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/data/points.py` & `genki-wave-0.5.2/genki_wave/data/points.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/data/structures.py` & `genki-wave-0.5.2/genki_wave/data/structures.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/data/writing.py` & `genki-wave-0.5.2/genki_wave/data/writing.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/discover.py` & `genki-wave-0.5.2/genki_wave/discover.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/protocols.py` & `genki-wave-0.5.2/genki_wave/protocols.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/threading_runner.py` & `genki-wave-0.5.2/genki_wave/threading_runner.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave/utils.py` & `genki-wave-0.5.2/genki_wave/utils.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/genki_wave.egg-info/PKG-INFO` & `genki-wave-0.5.2/genki_wave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genki-wave
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python API for Wave by Genki
 Home-page: https://github.com/genkiinstruments/genki-wave
 Author: Robert Torfason
 Author-email: robert@genkiinstruments.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genki-wave-0.5.1/genki_wave.egg-info/SOURCES.txt` & `genki-wave-0.5.2/genki_wave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genki-wave-0.5.1/setup.py` & `genki-wave-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md") as f:
     readme = f.read()
 
 requires = ["bleak", "cobs", "pyserial", "pyserial-asyncio"]
 
 setup(
     name="genki-wave",
-    version="0.5.1",
+    version="0.5.2",
     description="Python API for Wave by Genki",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Robert Torfason",
     author_email="robert@genkiinstruments.com",
     url="https://github.com/genkiinstruments/genki-wave",
     license="MIT",
```

