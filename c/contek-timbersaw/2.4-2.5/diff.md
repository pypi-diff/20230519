# Comparing `tmp/contek-timbersaw-2.4.tar.gz` & `tmp/contek-timbersaw-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contek-timbersaw-2.4.tar", last modified: Sat Oct  8 08:48:45 2022, max compression
+gzip compressed data, was "contek-timbersaw-2.5.tar", last modified: Thu May 18 10:11:05 2023, max compression
```

## Comparing `contek-timbersaw-2.4.tar` & `contek-timbersaw-2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-10-08 08:48:45.028944 contek-timbersaw-2.4/
--rw-rw-rw-   0        0        0     1082 2022-03-24 03:32:36.000000 contek-timbersaw-2.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2154 2022-10-08 08:48:45.027944 contek-timbersaw-2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1650 2022-05-30 04:03:41.000000 contek-timbersaw-2.4/README.md
-drwxrwxrwx   0        0        0        0 2022-10-08 08:48:45.018935 contek-timbersaw-2.4/contek_timbersaw/
--rw-rw-rw-   0        0        0     2397 2022-03-24 05:27:47.000000 contek-timbersaw-2.4/contek_timbersaw/__init__.py
--rw-rw-rw-   0        0        0     1916 2022-10-08 08:47:49.000000 contek-timbersaw-2.4/contek_timbersaw/async_compressor.py
--rw-rw-rw-   0        0        0     1195 2022-10-08 08:47:49.000000 contek-timbersaw-2.4/contek_timbersaw/deleter.py
--rw-rw-rw-   0        0        0     2517 2022-10-08 08:47:49.000000 contek-timbersaw-2.4/contek_timbersaw/timed_rolling_file_handler.py
-drwxrwxrwx   0        0        0        0 2022-10-08 08:48:45.026943 contek-timbersaw-2.4/contek_timbersaw.egg-info/
--rw-rw-rw-   0        0        0     2154 2022-10-08 08:48:44.000000 contek-timbersaw-2.4/contek_timbersaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2022-10-08 08:48:44.000000 contek-timbersaw-2.4/contek_timbersaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-08 08:48:44.000000 contek-timbersaw-2.4/contek_timbersaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-10-08 08:48:44.000000 contek-timbersaw-2.4/contek_timbersaw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-10-08 08:48:44.000000 contek-timbersaw-2.4/contek_timbersaw.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2022-10-08 08:48:45.029946 contek-timbersaw-2.4/setup.cfg
--rw-rw-rw-   0        0        0      795 2022-10-08 08:47:58.000000 contek-timbersaw-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:11:05.601452 contek-timbersaw-2.5/
+-rw-rw-rw-   0        0        0     1082 2022-03-24 03:32:36.000000 contek-timbersaw-2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2154 2023-05-18 10:11:05.600452 contek-timbersaw-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1650 2022-05-30 04:03:41.000000 contek-timbersaw-2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 10:11:05.593399 contek-timbersaw-2.5/contek_timbersaw/
+-rw-rw-rw-   0        0        0     2340 2023-05-18 10:09:19.000000 contek-timbersaw-2.5/contek_timbersaw/__init__.py
+-rw-rw-rw-   0        0        0     1916 2022-10-08 08:47:49.000000 contek-timbersaw-2.5/contek_timbersaw/async_compressor.py
+-rw-rw-rw-   0        0        0     1195 2022-10-08 08:47:49.000000 contek-timbersaw-2.5/contek_timbersaw/deleter.py
+-rw-rw-rw-   0        0        0     2517 2022-10-08 08:47:49.000000 contek-timbersaw-2.5/contek_timbersaw/timed_rolling_file_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:11:05.599450 contek-timbersaw-2.5/contek_timbersaw.egg-info/
+-rw-rw-rw-   0        0        0     2154 2023-05-18 10:11:05.000000 contek-timbersaw-2.5/contek_timbersaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-05-18 10:11:05.000000 contek-timbersaw-2.5/contek_timbersaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 10:11:05.000000 contek-timbersaw-2.5/contek_timbersaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-18 10:11:05.000000 contek-timbersaw-2.5/contek_timbersaw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 10:11:05.000000 contek-timbersaw-2.5/contek_timbersaw.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-18 10:11:05.601452 contek-timbersaw-2.5/setup.cfg
+-rw-rw-rw-   0        0        0      795 2023-05-18 10:09:31.000000 contek-timbersaw-2.5/setup.py
```

### Comparing `contek-timbersaw-2.4/LICENSE.txt` & `contek-timbersaw-2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contek-timbersaw-2.4/PKG-INFO` & `contek-timbersaw-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contek-timbersaw
-Version: 2.4
+Version: 2.5
 Summary: Timbersaw for automatic logging configuration
 Home-page: https://github.com/contek-io/contek-timbersaw
 Author: contek_bjy
 Author-email: bjy@contek.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `contek-timbersaw-2.4/README.md` & `contek-timbersaw-2.5/README.md`

 * *Files identical despite different names*

### Comparing `contek-timbersaw-2.4/contek_timbersaw/__init__.py` & `contek-timbersaw-2.5/contek_timbersaw/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,53 +14,46 @@
     log_date_format = os.getenv(
         'log_date_format',
         '%Y-%m-%dT%H:%M:%S',
     )
     log_root = os.getenv('log_root', os.path.join(os.getcwd(), 'logs'))
     log_rolling = os.getenv('log_rolling', 'MIDNIGHT')
     log_utc = bool(os.getenv('log_utc', False))
-    log_info_retention_days = int(os.getenv('log_info_retention_days', '14'))
+    log_info_retention_days = int(os.getenv('log_info_retention_days', '7'))
+    log_warn_retention_days = int(os.getenv('log_warn_retention_days', '14'))
     log_error_retention_days = int(os.getenv('log_error_retention_days', '28'))
 
     logger = logging.getLogger()
     formatter = logging.Formatter(fmt=log_format, datefmt=log_date_format)
     if log_utc:
         formatter.converter = time.gmtime
     stream_handler = logging.StreamHandler()
     stream_handler.setFormatter(formatter)
     stream_handler.setStream(sys.stdout)
-
     logger.addHandler(stream_handler)
     logger.setLevel(logging.INFO)
     logger.propagate = True
 
-    info_dir = os.path.join(log_root, 'info')
-    os.makedirs(info_dir, exist_ok=True)
-    info_file_handler = TimedRollingFileHandler(
-        info_dir,
-        compression_format='gz',
-        retention=log_info_retention_days * 24 * 60 * 60,
-        when=log_rolling,
-        utc=log_utc,
-    )
-    info_file_handler.setFormatter(formatter)
-    info_file_handler.setLevel(logging.INFO)
-    logger.addHandler(info_file_handler)
-
-    error_dir = os.path.join(log_root, 'error')
-    os.makedirs(error_dir, exist_ok=True)
-    error_file_handler = TimedRollingFileHandler(
-        error_dir,
-        retention=log_error_retention_days * 24 * 60 * 60,
-        when=log_rolling,
-        utc=log_utc,
-    )
-    error_file_handler.setFormatter(formatter)
-    error_file_handler.setLevel(logging.ERROR)
-    logger.addHandler(error_file_handler)
+    def add_file_handler(level, retention_days, compression_format=None):
+        file_dir = os.path.join(log_root, level)
+        os.makedirs(file_dir, exist_ok=True)
+        handler = TimedRollingFileHandler(
+            file_dir,
+            compression_format=compression_format,
+            retention=retention_days * 24 * 60 * 60,
+            when=log_rolling,
+            utc=log_utc,
+        )
+        handler.setFormatter(formatter)
+        handler.setLevel(logging.getLevelNamesMapping()[level])
+        logger.addHandler(handler)
+
+    add_file_handler('INFO', log_info_retention_days, 'gz')
+    add_file_handler('WARN', log_warn_retention_days)
+    add_file_handler('ERROR', log_error_retention_days)
 
     def handle_exception(exc_type, exc_value, exc_traceback) -> None:
         if issubclass(exc_type, KeyboardInterrupt):
             sys.__excepthook__(exc_type, exc_value, exc_traceback)
             return
 
         logger.exception(
```

### Comparing `contek-timbersaw-2.4/contek_timbersaw/async_compressor.py` & `contek-timbersaw-2.5/contek_timbersaw/async_compressor.py`

 * *Files identical despite different names*

### Comparing `contek-timbersaw-2.4/contek_timbersaw/deleter.py` & `contek-timbersaw-2.5/contek_timbersaw/deleter.py`

 * *Files identical despite different names*

### Comparing `contek-timbersaw-2.4/contek_timbersaw/timed_rolling_file_handler.py` & `contek-timbersaw-2.5/contek_timbersaw/timed_rolling_file_handler.py`

 * *Files identical despite different names*

### Comparing `contek-timbersaw-2.4/contek_timbersaw.egg-info/PKG-INFO` & `contek-timbersaw-2.5/contek_timbersaw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contek-timbersaw
-Version: 2.4
+Version: 2.5
 Summary: Timbersaw for automatic logging configuration
 Home-page: https://github.com/contek-io/contek-timbersaw
 Author: contek_bjy
 Author-email: bjy@contek.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `contek-timbersaw-2.4/setup.py` & `contek-timbersaw-2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='contek-timbersaw',
-    version='2.4',
+    version='2.5',
     description='Timbersaw for automatic logging configuration',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

