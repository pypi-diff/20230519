# Comparing `tmp/WinTraceroute-1.3.2.tar.gz` & `tmp/WinTraceroute-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinTraceroute-1.3.2.tar", last modified: Thu May 11 22:12:23 2023, max compression
+gzip compressed data, was "WinTraceroute-1.3.3.tar", last modified: Fri May 19 15:34:21 2023, max compression
```

## Comparing `WinTraceroute-1.3.2.tar` & `WinTraceroute-1.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:12:23.789938 WinTraceroute-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-11 22:11:50.000000 WinTraceroute-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-05-11 22:12:23.789938 WinTraceroute-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-11 22:11:50.000000 WinTraceroute-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:12:23.789938 WinTraceroute-1.3.2/WinTraceroute.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-05-11 22:12:23.000000 WinTraceroute-1.3.2/WinTraceroute.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-11 22:12:23.000000 WinTraceroute-1.3.2/WinTraceroute.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 22:12:23.000000 WinTraceroute-1.3.2/WinTraceroute.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 22:12:23.000000 WinTraceroute-1.3.2/WinTraceroute.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 22:12:23.000000 WinTraceroute-1.3.2/WinTraceroute.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 22:12:23.000000 WinTraceroute-1.3.2/WinTraceroute.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-11 22:11:50.000000 WinTraceroute-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 22:12:23.789938 WinTraceroute-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:12:23.789938 WinTraceroute-1.3.2/traceroute/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 22:11:50.000000 WinTraceroute-1.3.2/traceroute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-11 22:11:50.000000 WinTraceroute-1.3.2/traceroute/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100486 2023-05-11 22:11:50.000000 WinTraceroute-1.3.2/traceroute/lorem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-11 22:11:50.000000 WinTraceroute-1.3.2/traceroute/traceroute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:21.246363 WinTraceroute-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-19 15:33:40.000000 WinTraceroute-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-05-19 15:34:21.246363 WinTraceroute-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-19 15:33:40.000000 WinTraceroute-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:21.246363 WinTraceroute-1.3.3/WinTraceroute.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-05-19 15:34:21.000000 WinTraceroute-1.3.3/WinTraceroute.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-19 15:34:21.000000 WinTraceroute-1.3.3/WinTraceroute.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:34:21.000000 WinTraceroute-1.3.3/WinTraceroute.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 15:34:21.000000 WinTraceroute-1.3.3/WinTraceroute.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 15:34:21.000000 WinTraceroute-1.3.3/WinTraceroute.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 15:34:21.000000 WinTraceroute-1.3.3/WinTraceroute.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-19 15:33:40.000000 WinTraceroute-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:34:21.246363 WinTraceroute-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:21.246363 WinTraceroute-1.3.3/traceroute/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:33:40.000000 WinTraceroute-1.3.3/traceroute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-19 15:33:40.000000 WinTraceroute-1.3.3/traceroute/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100486 2023-05-19 15:33:40.000000 WinTraceroute-1.3.3/traceroute/lorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-05-19 15:33:40.000000 WinTraceroute-1.3.3/traceroute/traceroute.py
```

### Comparing `WinTraceroute-1.3.2/LICENSE` & `WinTraceroute-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.2/PKG-INFO` & `WinTraceroute-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinTraceroute
-Version: 1.3.2
+Version: 1.3.3
 Summary: A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `WinTraceroute-1.3.2/README.md` & `WinTraceroute-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.2/WinTraceroute.egg-info/PKG-INFO` & `WinTraceroute-1.3.3/WinTraceroute.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinTraceroute
-Version: 1.3.2
+Version: 1.3.3
 Summary: A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `WinTraceroute-1.3.2/pyproject.toml` & `WinTraceroute-1.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "bumpver", "scapy==2.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WinTraceroute"
-version = "1.3.2"
+version = "1.3.3"
 description = "A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy."
 authors = [{ name = "Nico Rittinghaus", email = "nico@ritti.ng" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta"
@@ -24,15 +24,15 @@
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "pyinstaller==5.10.1"]
 
 [project.urls]
 Homepage = "https://github.com/NiRit100/WinTraceroute"
 
 [tool.bumpver]
-current_version = "1.3.2"
+current_version = "1.3.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 # (BETA) tells setuptools you will be using a readme file for the long description field for your pypi profile.
```

### Comparing `WinTraceroute-1.3.2/traceroute/__main__.py` & `WinTraceroute-1.3.3/traceroute/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         print()
         print()
         print("NOTE: This software runs best under Python 3.9 and later.")
         print("      It is currently running on Python " + \
             str(py_version_info.major) + "." + str(py_version_info.minor) + ".")
         print("      The program can still be executed, but it might show some" \
             "\n      strange behaviour.")
-        input("  Press any key to continue.")
+        input("  Press ENTER to continue.")
         print("--- CONTINUING")
         print()
 
     try:
         # this once was a match statement, but not any more 
         # since the language downgrade
         if args.module == 'UDP':
```

### Comparing `WinTraceroute-1.3.2/traceroute/lorem.py` & `WinTraceroute-1.3.3/traceroute/lorem.py`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.2/traceroute/traceroute.py` & `WinTraceroute-1.3.3/traceroute/traceroute.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,17 +154,18 @@
 
 def is_dest_reached(responses:list, dest):
     for rt in responses:
         if rt == None:
             continue
         else:
             rt_icmp = rt[ICMP]
-            if rt_icmp.type == 3 or rt.src == dest:
-                return True  # Dest unreachable, port unavailable
-    return False
+            if rt_icmp.type != 3 and rt_icmp.code != 3: 
+                # NOT Dest unreachable, port unavailable
+                return False  
+    return True
 
 def summarize_termination(host, times, ttl, dest_reached):
     print(file=_WINTRACEROUTE_PRINT_FILE)
     if dest_reached:
         print("Destination '" + host + "' reached " + \
             " in RTT " + summarize_times(times, as_string=True) + " ms " + \
             " via " + str(ttl) + " hops.", \
```

