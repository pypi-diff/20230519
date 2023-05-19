# Comparing `tmp/fyers_token_manager_v2-0.1.1.tar.gz` & `tmp/fyers_token_manager_v2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_token_manager_v2-0.1.1.tar", last modified: Fri May 19 05:02:51 2023, max compression
+gzip compressed data, was "fyers_token_manager_v2-0.1.2.tar", last modified: Fri May 19 05:05:21 2023, max compression
```

## Comparing `fyers_token_manager_v2-0.1.1.tar` & `fyers_token_manager_v2-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 05:02:51.827835 fyers_token_manager_v2-0.1.1/
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.1.1/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-19 05:02:51.827835 fyers_token_manager_v2-0.1.1/PKG-INFO
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 05:26:39.000000 fyers_token_manager_v2-0.1.1/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 05:02:51.827835 fyers_token_manager_v2-0.1.1/fyers_token_manager_v2/
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)     4777 2023-05-19 05:02:34.000000 fyers_token_manager_v2-0.1.1/fyers_token_manager_v2/__init__.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 05:02:51.827835 fyers_token_manager_v2-0.1.1/fyers_token_manager_v2.egg-info/
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-19 05:02:51.000000 fyers_token_manager_v2-0.1.1/fyers_token_manager_v2.egg-info/PKG-INFO
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-19 05:02:51.000000 fyers_token_manager_v2-0.1.1/fyers_token_manager_v2.egg-info/SOURCES.txt
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-19 05:02:51.000000 fyers_token_manager_v2-0.1.1/fyers_token_manager_v2.egg-info/dependency_links.txt
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-19 05:02:51.000000 fyers_token_manager_v2-0.1.1/fyers_token_manager_v2.egg-info/requires.txt
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-19 05:02:51.000000 fyers_token_manager_v2-0.1.1/fyers_token_manager_v2.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-19 05:02:51.827835 fyers_token_manager_v2-0.1.1/setup.cfg
--rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-19 05:02:40.000000 fyers_token_manager_v2-0.1.1/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 05:05:21.773408 fyers_token_manager_v2-0.1.2/
+-rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.1.2/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-19 05:05:21.773408 fyers_token_manager_v2-0.1.2/PKG-INFO
+-rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 05:26:39.000000 fyers_token_manager_v2-0.1.2/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 05:05:21.769408 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2/
+-rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)     4840 2023-05-19 05:03:48.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2/__init__.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-19 05:05:21.773408 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/
+-rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-19 05:05:21.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/PKG-INFO
+-rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-19 05:05:21.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-19 05:05:21.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-19 05:05:21.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/requires.txt
+-rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-19 05:05:21.000000 fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-19 05:05:21.773408 fyers_token_manager_v2-0.1.2/setup.cfg
+-rwxrwxrwx   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-19 05:04:36.000000 fyers_token_manager_v2-0.1.2/setup.py
```

### Comparing `fyers_token_manager_v2-0.1.1/PKG-INFO` & `fyers_token_manager_v2-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_token_manager_v2
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers_token_manager_v2-0.1.1/README.md` & `fyers_token_manager_v2-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fyers_token_manager_v2-0.1.1/fyers_token_manager_v2/__init__.py` & `fyers_token_manager_v2-0.1.2/fyers_token_manager_v2/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,16 +27,19 @@
 
         self.__set_access_token_file_name()
         self.__initialize()
 
     def __set_access_token_file_name(self):
         home_directory = os.path.expanduser("~")
 
-        self.__data_path = pathlib.Path(f"{home_directory}/data/{self.username}")
-        self.__logs_path = pathlib.Path(f"{home_directory}/logs")
+        self.__data_path = pathlib.Path(
+            f"{home_directory}/fyers_token_manager/data/{self.username}"
+        )
+
+        self.__logs_path = pathlib.Path(f"{home_directory}/fyers_token_manager/logs")
 
         if not self.__data_path.exists():
             self.__data_path.mkdir(parents=True, exist_ok=True)
 
         if not self.__logs_path.exists():
             self.__logs_path.mkdir()
```

### Comparing `fyers_token_manager_v2-0.1.1/fyers_token_manager_v2.egg-info/PKG-INFO` & `fyers_token_manager_v2-0.1.2/fyers_token_manager_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager-v2
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers_token_manager_v2-0.1.1/setup.py` & `fyers_token_manager_v2-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers_token_manager_v2",
-    version="0.1.1",
+    version="0.1.2",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers_token_manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

