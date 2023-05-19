# Comparing `tmp/logol-0.0.4.tar.gz` & `tmp/logol-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logol-0.0.4.tar", last modified: Mon Dec 26 16:33:00 2022, max compression
+gzip compressed data, was "logol-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `logol-0.0.4.tar` & `logol-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3161 2022-02-11 11:53:48.259908 logol-0.0.4/.gitignore
--rw-r--r--   0        0        0     1105 2022-12-26 16:09:44.368041 logol-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2022-12-26 12:31:09.358622 logol-0.0.4/README.md
--rw-r--r--   0        0        0     3976 2022-12-26 16:30:05.630514 logol-0.0.4/logol.py
--rw-r--r--   0        0        0      542 2022-12-26 16:17:46.069923 logol-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      460 2022-12-26 14:34:21.869496 logol-0.0.4/test.py
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 logol-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3161 2022-02-11 11:53:48.259908 logol-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1105 2022-12-26 16:09:44.368041 logol-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-26 12:31:09.358622 logol-0.0.5/README.md
+-rw-r--r--   0        0        0     4374 2023-05-19 17:51:14.960008 logol-0.0.5/logol.py
+-rw-r--r--   0        0        0      417 2023-05-19 18:18:36.913952 logol-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-05-19 17:11:02.794317 logol-0.0.5/test.py
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 logol-0.0.5/PKG-INFO
```

### Comparing `logol-0.0.4/.gitignore` & `logol-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `logol-0.0.4/LICENSE` & `logol-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `logol-0.0.4/logol.py` & `logol-0.0.5/logol.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Pre-configured logs"""
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 import logging
 from logging.handlers import RotatingFileHandler
 from logging import Logger
 from typing import Dict, Optional
 from time import time_ns
 from pathlib import Path
@@ -13,16 +13,15 @@
 FORMAT_PRINTER = '%(asctime)s @%(threadName)s -> %(message)s'
 BASE_PATH = str(Path().home() / 'Logs')
 
 __loggers: Dict[str, Logger] = {}
 __printers: Dict[str, Logger] = {}
 
 
-def __default_logger(name, logpath, filesize_mb):
-    logger = logging.getLogger(name)
+def __configure_logger(logger, logpath, filesize_mb):
     logger.setLevel(logging.DEBUG)
 
     formatter = logging.Formatter(fmt=FORMAT_LOGGER, datefmt='%d/%b/%y %H:%M:%S')
     if logpath:
         if filesize_mb:
             logfile = RotatingFileHandler(logpath, mode='a', encoding='utf-8', maxBytes=filesize_mb*1024*1024)
         else:
@@ -61,37 +60,46 @@
     console.setFormatter(formatter)
 
     logger.addHandler(console)
 
     return logger
 
 def remove_handlers(logger):
-    for hdlr in logger.handlers:
-        logger.removeHandler(hdlr)
+    while len(logger.handlers) != 0:
+        logger.removeHandler(logger.handlers[0])
     
     return logger
 
-def get_logger(name, logpath=None, filesize_mb:Optional[int]=None):
+def get_logger(name, logpath=None, filesize_mb:Optional[int]=None, force:bool=False):
     """Get a Logger object from the logging module partly configured.
 
     Args:
         name (str): Name of log.
         logpath (str, optional): Path to log file. Defaults to None.
         filesize_mb (Optional[int], optional): Maximum size of log file. Defaults to None.
 
     Returns:
         Logger: A Logger object from the logging module.
     """
-    if name in __loggers:
+
+    if name not in __loggers:
+        logger = logging.getLogger(name)
+        logger = __configure_logger(logger, logpath, filesize_mb)
+        __loggers[name] = logger
+        return logger
+    elif force:
         logger = __loggers[name]
-        logger.warn(f'Trying to create a log with {logpath=} and {filesize_mb=} but a log with name {name} already exists.')
+        logger.warning(f'Reconfiguring the log called {name} to {logpath=}, {filesize_mb=}')
+        logger = remove_handlers(logger)
+        logger = __configure_logger(logger, logpath, filesize_mb)
         return logger
-    else:
-        logger = __default_logger(name, logpath, filesize_mb)
-        __loggers[name] = logger
+    else:   
+        logger = __loggers[name]
+        logger.warn(f'Trying to create a log with {logpath=} and {filesize_mb=}  but a log '
+                    f'with name {name} already exists. To force this operatin use force=True')
         return logger
 
 
 def get_print_debug(logpath, filesize_mb:int=5):
     """Get print and debug functions with logfile
 
     Args:
```

