# Comparing `tmp/discord-rich-presence-1.0.0.post1.tar.gz` & `tmp/discord-rich-presence-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-rich-presence-1.0.0.post1.tar", last modified: Tue Jun 14 06:32:24 2022, max compression
+gzip compressed data, was "discord-rich-presence-1.0.1.tar", last modified: Fri May 19 03:21:48 2023, max compression
```

## Comparing `discord-rich-presence-1.0.0.post1.tar` & `discord-rich-presence-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2022-06-14 06:32:24.451724 discord-rich-presence-1.0.0.post1/
--rw-r--r--   0 maxwe      (501) staff       (20)     1064 2022-06-14 05:49:12.000000 discord-rich-presence-1.0.0.post1/LICENSE
--rw-r--r--   0 maxwe      (501) staff       (20)     2803 2022-06-14 06:32:24.451370 discord-rich-presence-1.0.0.post1/PKG-INFO
--rw-r--r--   0 maxwe      (501) staff       (20)     2111 2022-06-14 05:47:37.000000 discord-rich-presence-1.0.0.post1/README.md
-drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2022-06-14 06:32:24.445717 discord-rich-presence-1.0.0.post1/discord_rich_presence.egg-info/
--rw-r--r--   0 maxwe      (501) staff       (20)     2803 2022-06-14 06:32:23.000000 discord-rich-presence-1.0.0.post1/discord_rich_presence.egg-info/PKG-INFO
--rw-r--r--   0 maxwe      (501) staff       (20)      250 2022-06-14 06:32:24.000000 discord-rich-presence-1.0.0.post1/discord_rich_presence.egg-info/SOURCES.txt
--rw-r--r--   0 maxwe      (501) staff       (20)        1 2022-06-14 06:32:23.000000 discord-rich-presence-1.0.0.post1/discord_rich_presence.egg-info/dependency_links.txt
--rw-r--r--   0 maxwe      (501) staff       (20)       10 2022-06-14 06:32:24.000000 discord-rich-presence-1.0.0.post1/discord_rich_presence.egg-info/top_level.txt
-drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2022-06-14 06:32:24.447025 discord-rich-presence-1.0.0.post1/discordrp/
--rw-r--r--   0 maxwe      (501) staff       (20)      266 2022-06-14 06:27:52.000000 discord-rich-presence-1.0.0.post1/discordrp/__init__.py
--rw-r--r--   0 maxwe      (501) staff       (20)     4858 2022-06-14 05:08:12.000000 discord-rich-presence-1.0.0.post1/discordrp/presence.py
--rw-r--r--   0 maxwe      (501) staff       (20)       38 2022-06-14 06:32:24.451845 discord-rich-presence-1.0.0.post1/setup.cfg
--rw-r--r--   0 maxwe      (501) staff       (20)      932 2022-06-14 06:13:05.000000 discord-rich-presence-1.0.0.post1/setup.py
+drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-05-19 03:21:48.344714 discord-rich-presence-1.0.1/
+-rw-r--r--   0 maxwe      (501) staff       (20)     1064 2022-06-14 05:49:12.000000 discord-rich-presence-1.0.1/LICENSE
+-rw-r--r--   0 maxwe      (501) staff       (20)     2797 2023-05-19 03:21:48.344064 discord-rich-presence-1.0.1/PKG-INFO
+-rw-r--r--   0 maxwe      (501) staff       (20)     2111 2022-06-14 05:47:37.000000 discord-rich-presence-1.0.1/README.md
+drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-05-19 03:21:48.338109 discord-rich-presence-1.0.1/discord_rich_presence.egg-info/
+-rw-r--r--   0 maxwe      (501) staff       (20)     2797 2023-05-19 03:21:48.000000 discord-rich-presence-1.0.1/discord_rich_presence.egg-info/PKG-INFO
+-rw-r--r--   0 maxwe      (501) staff       (20)      250 2023-05-19 03:21:48.000000 discord-rich-presence-1.0.1/discord_rich_presence.egg-info/SOURCES.txt
+-rw-r--r--   0 maxwe      (501) staff       (20)        1 2023-05-19 03:21:48.000000 discord-rich-presence-1.0.1/discord_rich_presence.egg-info/dependency_links.txt
+-rw-r--r--   0 maxwe      (501) staff       (20)       10 2023-05-19 03:21:48.000000 discord-rich-presence-1.0.1/discord_rich_presence.egg-info/top_level.txt
+drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-05-19 03:21:48.341306 discord-rich-presence-1.0.1/discordrp/
+-rw-r--r--   0 maxwe      (501) staff       (20)      260 2023-05-19 03:14:54.000000 discord-rich-presence-1.0.1/discordrp/__init__.py
+-rw-r--r--   0 maxwe      (501) staff       (20)     4884 2023-05-19 03:14:00.000000 discord-rich-presence-1.0.1/discordrp/presence.py
+-rw-r--r--   0 maxwe      (501) staff       (20)       38 2023-05-19 03:21:48.344970 discord-rich-presence-1.0.1/setup.cfg
+-rw-r--r--   0 maxwe      (501) staff       (20)      932 2022-06-14 06:13:05.000000 discord-rich-presence-1.0.1/setup.py
```

### Comparing `discord-rich-presence-1.0.0.post1/LICENSE` & `discord-rich-presence-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-rich-presence-1.0.0.post1/PKG-INFO` & `discord-rich-presence-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-rich-presence
-Version: 1.0.0.post1
+Version: 1.0.1
 Summary: A lightweight and safe module for creating custom rich presences on Discord.
 Home-page: https://github.com/TenType/discord-rich-presence
 Author: TenType
 License: MIT
 Keywords: discord,presence,rich presence,activity,rpc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discord-rich-presence-1.0.0.post1/README.md` & `discord-rich-presence-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `discord-rich-presence-1.0.0.post1/discord_rich_presence.egg-info/PKG-INFO` & `discord-rich-presence-1.0.1/discord_rich_presence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-rich-presence
-Version: 1.0.0.post1
+Version: 1.0.1
 Summary: A lightweight and safe module for creating custom rich presences on Discord.
 Home-page: https://github.com/TenType/discord-rich-presence
 Author: TenType
 License: MIT
 Keywords: discord,presence,rich presence,activity,rpc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discord-rich-presence-1.0.0.post1/discordrp/presence.py` & `discord-rich-presence-1.0.1/discordrp/presence.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
 
 class Presence:
     """
     The main class used to connect to Discord for its rich presence API.
     """
 
-    def __init__(self, client_id: int):
+    def __init__(self, client_id: str):
         self.client_id = client_id
         self._platform = sys.platform
         self._socket = None
 
         # Connect to Discord IPC
         self._connect()
 
@@ -118,17 +118,17 @@
             # Windows pipe
             return R'\\?\pipe\\' + SOCKET_NAME
 
         # Unix pipe
         for env in ('XDG_RUNTIME_DIR', 'TMPDIR', 'TMP', 'TEMP'):
             path = os.environ.get(env)
             if path is not None:
-                return path + SOCKET_NAME
+                return os.path.join(path, SOCKET_NAME)
 
-        return '/tmp/' + SOCKET_NAME
+        return os.path.join('/tmp/', SOCKET_NAME)
 
     def _try_socket(self, pipe: str, i: int):
         if self._platform == WINDOWS:
             self._socket = open(pipe.format(i), 'wb')
         else:
             self._socket = socket.socket(socket.AF_UNIX)
             self._socket.connect(pipe.format(i))
```

### Comparing `discord-rich-presence-1.0.0.post1/setup.py` & `discord-rich-presence-1.0.1/setup.py`

 * *Files identical despite different names*

