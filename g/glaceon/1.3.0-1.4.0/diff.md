# Comparing `tmp/glaceon-1.3.0.tar.gz` & `tmp/glaceon-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glaceon-1.3.0.tar", last modified: Mon May 15 08:59:41 2023, max compression
+gzip compressed data, was "glaceon-1.4.0.tar", last modified: Fri May 19 08:04:51 2023, max compression
```

## Comparing `glaceon-1.3.0.tar` & `glaceon-1.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 08:59:41.384020 glaceon-1.3.0/
-drwxrwxrwx   0        0        0        0 2023-05-15 08:59:41.378017 glaceon-1.3.0/GLACEON/
--rw-rw-rw-   0        0        0     2423 2023-05-15 08:21:53.000000 glaceon-1.3.0/GLACEON/__init__.py
--rw-rw-rw-   0        0        0     2855 2023-05-15 08:59:41.384020 glaceon-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1624 2023-05-15 08:46:25.000000 glaceon-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 08:59:41.383355 glaceon-1.3.0/glaceon.egg-info/
--rw-rw-rw-   0        0        0     2855 2023-05-15 08:59:41.000000 glaceon-1.3.0/glaceon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-05-15 08:59:41.000000 glaceon-1.3.0/glaceon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 08:59:41.000000 glaceon-1.3.0/glaceon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-15 08:59:41.000000 glaceon-1.3.0/glaceon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 08:59:41.385021 glaceon-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1551 2023-05-15 08:58:51.000000 glaceon-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:04:51.625355 glaceon-1.4.0/
+drwxrwxrwx   0        0        0        0 2023-05-19 08:04:51.620377 glaceon-1.4.0/GLACEON/
+-rw-rw-rw-   0        0        0     2896 2023-05-19 08:04:14.000000 glaceon-1.4.0/GLACEON/__init__.py
+-rw-rw-rw-   0        0        0     2855 2023-05-19 08:04:51.625355 glaceon-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1624 2023-05-15 08:46:25.000000 glaceon-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 08:04:51.624357 glaceon-1.4.0/glaceon.egg-info/
+-rw-rw-rw-   0        0        0     2855 2023-05-19 08:04:51.000000 glaceon-1.4.0/glaceon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-05-19 08:04:51.000000 glaceon-1.4.0/glaceon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 08:04:51.000000 glaceon-1.4.0/glaceon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 08:04:51.000000 glaceon-1.4.0/glaceon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 08:04:51.625355 glaceon-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1551 2023-05-19 08:04:32.000000 glaceon-1.4.0/setup.py
```

### Comparing `glaceon-1.3.0/GLACEON/__init__.py` & `glaceon-1.4.0/GLACEON/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 import time
 
 
-class cli:
+class cli
 
     def __init__(self, speed=None, debug=None):
         self.speed = speed
         self.last_timestamp = time.time()
         self.debug = debug
         self.initialized = speed is not None and debug is not None
 
@@ -25,15 +25,14 @@
             r += r_step
             g += g_step
             b += b_step
             faded_text += f"\033[38;2;{int(r)};{int(g)};{int(b)}m{letter}\033[0m"
         return faded_text
 
     def print(self, tag, message):
-
         timestamp = self.getTimestamp()
         inittag = self.fade("ERROR", (255, 0, 0), (128, 0, 0))
 
         if not self.initialized:
             if not self.debug:
                 print(f"{timestamp} [{inittag}] Not initialized!")
                 input()
@@ -58,13 +57,34 @@
             if not self.debug:
                 return
             tag_text = self.fade(tag_text, (0, 0, 255), (0, 191, 255))
         else:
             print(f"{timestamp} [{inittag}] Invalid Tag: {tag}")
             input()
             exit()
-        current_time = datetime.now().strftime("%H:%M:%S")
 
+        current_time = datetime.now().strftime("%H:%M:%S")
         time_elapsed = time.time() - self.last_timestamp
         self.last_timestamp += max(1 / self.speed - time_elapsed, 0)
 
-        print(f"{timestamp} [{tag_text}] {message_text}")
+        print(f"{timestamp} [{tag_text}] {message_text}")
+
+
+class FlaskGlaceon:
+
+    def __init__(self, glaceon_instance):
+        self.g = glaceon_instance
+
+    def info(self, message):
+        self.g.print("INFO", message)
+
+    def warning(self, message):
+        self.g.print("WARNING", message)
+
+    def error(self, message):
+        self.g.print("ERROR", message)
+
+    def success(self, message):
+        self.g.print("SUCCESS", message)
+
+    def debug(self, message):
+        self.g.print("DEBUG", message)
```

### Comparing `glaceon-1.3.0/PKG-INFO` & `glaceon-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glaceon
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Simple And Clean Logging Library That Can Be Used For Any Type Of Application.
 Home-page: https://pypi.python.org/pypi/glaceon
 Author: Zappy
 Author-email: monkey@monk.com
 License: MIT
 Project-URL: Homepage, https://github.com/BornPaster/Glaceon
 Project-URL: Suggestions, https://github.com/BornPaster/Glaceon/issues
```

### Comparing `glaceon-1.3.0/README.md` & `glaceon-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `glaceon-1.3.0/glaceon.egg-info/PKG-INFO` & `glaceon-1.4.0/glaceon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glaceon
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Simple And Clean Logging Library That Can Be Used For Any Type Of Application.
 Home-page: https://pypi.python.org/pypi/glaceon
 Author: Zappy
 Author-email: monkey@monk.com
 License: MIT
 Project-URL: Homepage, https://github.com/BornPaster/Glaceon
 Project-URL: Suggestions, https://github.com/BornPaster/Glaceon/issues
```

### Comparing `glaceon-1.3.0/setup.py` & `glaceon-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
     
 setup(name="glaceon",
-      version="1.3.0",
+      version="1.4.0",
       description="A Simple And Clean Logging Library That Can Be Used For Any Type Of Application.",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
       author="Zappy",
       url="https://pypi.python.org/pypi/glaceon",
       author_email="monkey@monk.com",
```

