# Comparing `tmp/cellworld-tracking-0.0.5.tar.gz` & `tmp/cellworld-tracking-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld-tracking-0.0.5.tar", last modified: Fri Dec 31 19:07:36 2021, max compression
+gzip compressed data, was "cellworld-tracking-0.0.6.tar", last modified: Mon Jan 10 00:42:47 2022, max compression
```

## Comparing `cellworld-tracking-0.0.5.tar` & `cellworld-tracking-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2021-12-31 19:07:36.617159 cellworld-tracking-0.0.5/
--rwxrwxrwx   0 german    (1000) german    (1000)      213 2021-12-31 19:07:36.609157 cellworld-tracking-0.0.5/PKG-INFO
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2021-12-31 19:07:36.093054 cellworld-tracking-0.0.5/cellworld_tracking/
--rwxrwxrwx   0 german    (1000) german    (1000)       60 2021-12-31 19:07:34.000000 cellworld-tracking-0.0.5/cellworld_tracking/__init__.py
--rwxrwxrwx   0 german    (1000) german    (1000)     5487 2021-12-31 19:07:34.000000 cellworld-tracking-0.0.5/cellworld_tracking/agent_tracking.py
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2021-12-31 19:07:36.529471 cellworld-tracking-0.0.5/cellworld_tracking.egg-info/
--rwxrwxrwx   0 german    (1000) german    (1000)      213 2021-12-31 19:07:35.000000 cellworld-tracking-0.0.5/cellworld_tracking.egg-info/PKG-INFO
--rwxrwxrwx   0 german    (1000) german    (1000)      326 2021-12-31 19:07:35.000000 cellworld-tracking-0.0.5/cellworld_tracking.egg-info/SOURCES.txt
--rwxrwxrwx   0 german    (1000) german    (1000)        1 2021-12-31 19:07:35.000000 cellworld-tracking-0.0.5/cellworld_tracking.egg-info/dependency_links.txt
--rwxrwxrwx   0 german    (1000) german    (1000)        1 2021-12-31 19:07:35.000000 cellworld-tracking-0.0.5/cellworld_tracking.egg-info/not-zip-safe
--rwxrwxrwx   0 german    (1000) german    (1000)       32 2021-12-31 19:07:35.000000 cellworld-tracking-0.0.5/cellworld_tracking.egg-info/requires.txt
--rwxrwxrwx   0 german    (1000) german    (1000)       19 2021-12-31 19:07:35.000000 cellworld-tracking-0.0.5/cellworld_tracking.egg-info/top_level.txt
--rwxrwxrwx   0 german    (1000) german    (1000)       38 2021-12-31 19:07:36.620157 cellworld-tracking-0.0.5/setup.cfg
--rwxrwxrwx   0 german    (1000) german    (1000)      264 2021-12-31 19:07:34.000000 cellworld-tracking-0.0.5/setup.py
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-10 00:42:45.983778 cellworld-tracking-0.0.6/
+-rwxrwxrwx   0 german    (1000) german    (1000)      213 2022-01-10 00:42:45.981778 cellworld-tracking-0.0.6/PKG-INFO
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-10 00:42:45.909210 cellworld-tracking-0.0.6/cellworld_tracking/
+-rwxrwxrwx   0 german    (1000) german    (1000)       60 2022-01-10 00:42:45.000000 cellworld-tracking-0.0.6/cellworld_tracking/__init__.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     5491 2022-01-10 00:42:45.000000 cellworld-tracking-0.0.6/cellworld_tracking/agent_tracking.py
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-10 00:42:45.969763 cellworld-tracking-0.0.6/cellworld_tracking.egg-info/
+-rwxrwxrwx   0 german    (1000) german    (1000)      213 2022-01-10 00:42:45.000000 cellworld-tracking-0.0.6/cellworld_tracking.egg-info/PKG-INFO
+-rwxrwxrwx   0 german    (1000) german    (1000)      326 2022-01-10 00:42:45.000000 cellworld-tracking-0.0.6/cellworld_tracking.egg-info/SOURCES.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-01-10 00:42:45.000000 cellworld-tracking-0.0.6/cellworld_tracking.egg-info/dependency_links.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-01-10 00:42:45.000000 cellworld-tracking-0.0.6/cellworld_tracking.egg-info/not-zip-safe
+-rwxrwxrwx   0 german    (1000) german    (1000)       32 2022-01-10 00:42:45.000000 cellworld-tracking-0.0.6/cellworld_tracking.egg-info/requires.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)       19 2022-01-10 00:42:45.000000 cellworld-tracking-0.0.6/cellworld_tracking.egg-info/top_level.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)       38 2022-01-10 00:42:45.983778 cellworld-tracking-0.0.6/setup.cfg
+-rwxrwxrwx   0 german    (1000) german    (1000)      264 2022-01-10 00:42:45.000000 cellworld-tracking-0.0.6/setup.py
```

### Comparing `cellworld-tracking-0.0.5/cellworld_tracking/agent_tracking.py` & `cellworld-tracking-0.0.6/cellworld_tracking/agent_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,20 +58,20 @@
     def __run__(self, cmd:str, parameters="", new_connection=True, leave_open=False):
         try:
             if new_connection:
                 self.client = Client()
                 self.client.connect(self.ip, self.port)
             self.client.connection.send(Message(cmd, parameters))
             t = Timer(5)
-            while not self.client.messages.contains(cmd + "_result") and t:
+            while not self.client.messages.contains(cmd + "_response") and t:
                 pass
             if not leave_open:
                 self.client.disconnect()
                 self.client = None
-            if self.client.messages.get_message(cmd + "_result").body == "ok":
+            if self.client.messages.get_message(cmd + "_response").body == "ok":
                 return True
             else:
                 return False
         except:
             return False
 
     def register_consumer(self, call_back=None):
```

