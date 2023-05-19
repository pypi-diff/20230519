# Comparing `tmp/guardshield-1.0.1.tar.gz` & `tmp/guardshield-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\guardshield-1.0.1.tar", last modified: Fri May 19 17:04:48 2023, max compression
+gzip compressed data, was "dist\guardshield-1.0.2.tar", last modified: Fri May 19 17:13:30 2023, max compression
```

## Comparing `guardshield-1.0.1.tar` & `guardshield-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 17:04:48.898958 guardshield-1.0.1/
--rw-rw-rw-   0        0        0      232 2023-05-19 17:04:48.897961 guardshield-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2323 2023-05-19 17:02:01.000000 guardshield-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 17:04:48.875050 guardshield-1.0.1/guardshield/
--rw-rw-rw-   0        0        0       87 2023-05-18 23:49:41.000000 guardshield-1.0.1/guardshield/__init__.py
--rw-rw-rw-   0        0        0    17408 2023-05-18 23:20:40.000000 guardshield-1.0.1/guardshield/lib.dll
--rw-rw-rw-   0        0        0     1857 2023-05-19 17:01:08.000000 guardshield-1.0.1/guardshield/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 17:04:48.896991 guardshield-1.0.1/guardshield.egg-info/
--rw-rw-rw-   0        0        0      232 2023-05-19 17:04:48.000000 guardshield-1.0.1/guardshield.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-05-19 17:04:48.000000 guardshield-1.0.1/guardshield.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 17:04:48.000000 guardshield-1.0.1/guardshield.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-19 17:04:48.000000 guardshield-1.0.1/guardshield.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-05-19 17:04:48.000000 guardshield-1.0.1/guardshield.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 17:04:48.898958 guardshield-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      476 2023-05-19 17:04:36.000000 guardshield-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:13:30.405916 guardshield-1.0.2/
+-rw-rw-rw-   0        0        0      232 2023-05-19 17:13:30.404919 guardshield-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2323 2023-05-19 17:02:01.000000 guardshield-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 17:13:30.378993 guardshield-1.0.2/guardshield/
+-rw-rw-rw-   0        0        0       87 2023-05-18 23:49:41.000000 guardshield-1.0.2/guardshield/__init__.py
+-rw-rw-rw-   0        0        0    17408 2023-05-18 23:20:40.000000 guardshield-1.0.2/guardshield/lib.dll
+-rw-rw-rw-   0        0        0     1818 2023-05-19 17:13:16.000000 guardshield-1.0.2/guardshield/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:13:30.403921 guardshield-1.0.2/guardshield.egg-info/
+-rw-rw-rw-   0        0        0      232 2023-05-19 17:13:30.000000 guardshield-1.0.2/guardshield.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-05-19 17:13:30.000000 guardshield-1.0.2/guardshield.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 17:13:30.000000 guardshield-1.0.2/guardshield.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-19 17:13:30.000000 guardshield-1.0.2/guardshield.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-05-19 17:13:30.000000 guardshield-1.0.2/guardshield.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 17:13:30.405916 guardshield-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      476 2023-05-19 17:12:35.000000 guardshield-1.0.2/setup.py
```

### Comparing `guardshield-1.0.1/README.md` & `guardshield-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `guardshield-1.0.1/guardshield/lib.dll` & `guardshield-1.0.2/guardshield/lib.dll`

 * *Files identical despite different names*

### Comparing `guardshield-1.0.1/guardshield/main.py` & `guardshield-1.0.2/guardshield/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os, ctypes, threading, time, sys
+import pkg_resources
 
 timeout = 0.1
 
 
 class AntiDebugger:
 
     def __init__(self, dll, settings):
@@ -42,17 +43,16 @@
             "anti_debugger" : anti_debugger,
             "kill_on_debug" : kill_on_debug,
             "custom_function_on_detection" : custom_function_on_detection
         }
 
     def load_dll(self) -> None:
 
-        path = getattr(sys, '_MEIPASS', os.path.dirname(os.path.abspath(__file__)))
-        dir = os.path.join(path, r'lib.dll')
-        self.dll = ctypes.WinDLL(dir)
+        path = pkg_resources.resource_filename(__name__, 'lib.dll')
+        self.dll = ctypes.WinDLL(path)
     
     def check_security(self) -> None:
 
         if self.settings['anti_debugger'] == True:
             AntiDebugger(
                 dll = self.dll,
                 settings = self.settings
```

