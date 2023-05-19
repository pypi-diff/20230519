# Comparing `tmp/fyers_token_manager_v2-0.0.8.tar.gz` & `tmp/fyers_token_manager_v2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_token_manager_v2-0.0.8.tar", last modified: Sat May 13 04:04:11 2023, max compression
+gzip compressed data, was "fyers_token_manager_v2-0.0.9.tar", last modified: Fri May 19 04:25:28 2023, max compression
```

## Comparing `fyers_token_manager_v2-0.0.8.tar` & `fyers_token_manager_v2-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-13 04:04:11.724230 fyers_token_manager_v2-0.0.8/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.8/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-13 04:04:11.724230 fyers_token_manager_v2-0.0.8/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 05:26:39.000000 fyers_token_manager_v2-0.0.8/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-13 04:04:11.724230 fyers_token_manager_v2-0.0.8/fyers_token_manager_v2/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4806 2023-05-12 00:50:04.000000 fyers_token_manager_v2-0.0.8/fyers_token_manager_v2/__init__.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-13 04:04:11.724230 fyers_token_manager_v2-0.0.8/fyers_token_manager_v2.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-13 04:04:11.000000 fyers_token_manager_v2-0.0.8/fyers_token_manager_v2.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-13 04:04:11.000000 fyers_token_manager_v2-0.0.8/fyers_token_manager_v2.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-13 04:04:11.000000 fyers_token_manager_v2-0.0.8/fyers_token_manager_v2.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-13 04:04:11.000000 fyers_token_manager_v2-0.0.8/fyers_token_manager_v2.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-13 04:04:11.000000 fyers_token_manager_v2-0.0.8/fyers_token_manager_v2.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-13 04:04:11.724230 fyers_token_manager_v2-0.0.8/setup.cfg
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-12 00:58:49.000000 fyers_token_manager_v2-0.0.8/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 04:25:28.516276 fyers_token_manager_v2-0.0.9/
+-rwxr-xr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.9/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-19 04:25:28.516276 fyers_token_manager_v2-0.0.9/PKG-INFO
+-rwxr-xr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 05:26:39.000000 fyers_token_manager_v2-0.0.9/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 04:25:28.516276 fyers_token_manager_v2-0.0.9/fyers_token_manager_v2/
+-rwxr-xr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)     4806 2023-05-12 00:50:04.000000 fyers_token_manager_v2-0.0.9/fyers_token_manager_v2/__init__.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 04:25:28.516276 fyers_token_manager_v2-0.0.9/fyers_token_manager_v2.egg-info/
+-rwxr-xr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-19 04:25:28.000000 fyers_token_manager_v2-0.0.9/fyers_token_manager_v2.egg-info/PKG-INFO
+-rwxr-xr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-19 04:25:28.000000 fyers_token_manager_v2-0.0.9/fyers_token_manager_v2.egg-info/SOURCES.txt
+-rwxr-xr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-19 04:25:28.000000 fyers_token_manager_v2-0.0.9/fyers_token_manager_v2.egg-info/dependency_links.txt
+-rwxr-xr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-19 04:25:28.000000 fyers_token_manager_v2-0.0.9/fyers_token_manager_v2.egg-info/requires.txt
+-rwxr-xr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-19 04:25:28.000000 fyers_token_manager_v2-0.0.9/fyers_token_manager_v2.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-19 04:25:28.516276 fyers_token_manager_v2-0.0.9/setup.cfg
+-rwxr-xr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-19 04:22:29.000000 fyers_token_manager_v2-0.0.9/setup.py
```

### Comparing `fyers_token_manager_v2-0.0.8/PKG-INFO` & `fyers_token_manager_v2-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_token_manager_v2
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers_token_manager_v2-0.0.8/README.md` & `fyers_token_manager_v2-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fyers_token_manager_v2-0.0.8/fyers_token_manager_v2/__init__.py` & `fyers_token_manager_v2-0.0.9/fyers_token_manager_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fyers_token_manager_v2-0.0.8/fyers_token_manager_v2.egg-info/PKG-INFO` & `fyers_token_manager_v2-0.0.9/fyers_token_manager_v2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager-v2
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers_token_manager_v2-0.0.8/setup.py` & `fyers_token_manager_v2-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers_token_manager_v2",
-    version="0.0.8",
+    version="0.0.9",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers_token_manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

