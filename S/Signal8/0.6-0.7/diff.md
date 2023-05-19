# Comparing `tmp/Signal8-0.6.tar.gz` & `tmp/Signal8-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-0.6.tar", last modified: Fri May 19 05:05:00 2023, max compression
+gzip compressed data, was "Signal8-0.7.tar", last modified: Fri May 19 05:14:13 2023, max compression
```

## Comparing `Signal8-0.6.tar` & `Signal8-0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 05:05:00.815012 Signal8-0.6/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-0.6/LICENSE
--rw-rw-rw-   0        0        0     4371 2023-05-19 05:05:00.812011 Signal8-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3881 2023-05-17 21:23:57.000000 Signal8-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 05:05:00.761011 Signal8-0.6/Signal8/
--rw-rw-rw-   0        0        0     6682 2023-05-19 04:56:46.000000 Signal8-0.6/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-05-19 05:04:09.000000 Signal8-0.6/Signal8/__init__.py
--rw-rw-rw-   0        0        0      117 2023-05-19 04:35:05.000000 Signal8-0.6/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:05:00.807012 Signal8-0.6/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-0.6/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     7891 2023-05-17 20:35:42.000000 Signal8-0.6/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2459 2023-05-17 19:04:54.000000 Signal8-0.6/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-0.6/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12660 2023-05-19 04:57:08.000000 Signal8-0.6/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:05:00.773011 Signal8-0.6/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4371 2023-05-19 05:05:00.000000 Signal8-0.6/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-19 05:05:00.000000 Signal8-0.6/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 05:05:00.000000 Signal8-0.6/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 05:05:00.000000 Signal8-0.6/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 05:05:00.815012 Signal8-0.6/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-05-19 05:04:49.000000 Signal8-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:14:13.571059 Signal8-0.7/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-0.7/LICENSE
+-rw-rw-rw-   0        0        0     4371 2023-05-19 05:14:13.569055 Signal8-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3881 2023-05-17 21:23:57.000000 Signal8-0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 05:14:13.505056 Signal8-0.7/Signal8/
+-rw-rw-rw-   0        0        0     6682 2023-05-19 05:13:45.000000 Signal8-0.7/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-05-19 05:04:09.000000 Signal8-0.7/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      136 2023-05-19 05:13:31.000000 Signal8-0.7/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:14:13.564059 Signal8-0.7/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-0.7/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     7891 2023-05-17 20:35:42.000000 Signal8-0.7/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2459 2023-05-17 19:04:54.000000 Signal8-0.7/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-0.7/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12585 2023-05-19 05:11:53.000000 Signal8-0.7/Signal8/utils/simple_env.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:14:13.540056 Signal8-0.7/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4371 2023-05-19 05:14:13.000000 Signal8-0.7/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-19 05:14:13.000000 Signal8-0.7/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 05:14:13.000000 Signal8-0.7/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 05:14:13.000000 Signal8-0.7/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 05:14:13.575056 Signal8-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-05-19 05:13:57.000000 Signal8-0.7/setup.py
```

### Comparing `Signal8-0.6/LICENSE` & `Signal8-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-0.6/PKG-INFO` & `Signal8-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 0.6
+Version: 0.7
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-0.6/README.md` & `Signal8-0.7/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-0.6/Signal8/Signal8.py` & `Signal8-0.7/Signal8/Signal8.py`

 * *Files identical despite different names*

### Comparing `Signal8-0.6/Signal8/utils/core.py` & `Signal8-0.7/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-0.6/Signal8/utils/problems.py` & `Signal8-0.7/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-0.6/Signal8/utils/simple_env.py` & `Signal8-0.7/Signal8/utils/simple_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,15 @@
         self.render_mode = render_mode
         pygame.init()
         self.viewer = None
         self.width = 700
         self.height = 700
         self.screen = pygame.Surface([self.width, self.height])
         self.max_size = 1
-        self.game_font = pygame.freetype.Font(
-            os.path.join(os.path.dirname(__file__), "secrcode.ttf"), 24
-        )
+        self.game_font = pygame.freetype.Font(None, 20)
 
         # Set up the drawing window
 
         self.renderOn = False
         self.seed()
 
         self.max_cycles = max_cycles
```

### Comparing `Signal8-0.6/Signal8.egg-info/PKG-INFO` & `Signal8-0.7/Signal8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 0.6
+Version: 0.7
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

