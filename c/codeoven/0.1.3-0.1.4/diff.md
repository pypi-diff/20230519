# Comparing `tmp/codeoven-0.1.3.tar.gz` & `tmp/codeoven-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeoven-0.1.3.tar", last modified: Sun Apr  2 08:09:27 2023, max compression
+gzip compressed data, was "codeoven-0.1.4.tar", last modified: Fri May 19 00:35:24 2023, max compression
```

## Comparing `codeoven-0.1.3.tar` & `codeoven-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-02 08:09:27.855890 codeoven-0.1.3/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 codeoven-0.1.3/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       67 2023-04-02 08:09:16.000000 codeoven-0.1.3/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)     6114 2023-04-02 08:09:27.855943 codeoven-0.1.3/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)     5147 2023-04-02 07:29:56.000000 codeoven-0.1.3/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 codeoven-0.1.3/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)     1068 2023-04-02 08:09:27.856222 codeoven-0.1.3/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 codeoven-0.1.3/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-02 08:09:27.852922 codeoven-0.1.3/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-02 08:09:27.855016 codeoven-0.1.3/src/codeoven/
--rw-r--r--   0 shuntaro   (501) staff       (20)       26 2023-04-02 07:38:59.000000 codeoven-0.1.3/src/codeoven/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)    18120 2022-08-24 10:59:06.000000 codeoven-0.1.3/src/codeoven/codeoven.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     1612 2022-08-26 16:10:57.000000 codeoven-0.1.3/src/codeoven/oven_utils.c
--rw-r--r--   0 shuntaro   (501) staff       (20)      194 2022-06-02 00:59:28.000000 codeoven-0.1.3/src/codeoven/oven_utils.h
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-04-02 08:09:27.855778 codeoven-0.1.3/src/codeoven.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     6114 2023-04-02 08:09:27.000000 codeoven-0.1.3/src/codeoven.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      348 2023-04-02 08:09:27.000000 codeoven-0.1.3/src/codeoven.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-04-02 08:09:27.000000 codeoven-0.1.3/src/codeoven.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       23 2023-04-02 08:09:27.000000 codeoven-0.1.3/src/codeoven.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        9 2023-04-02 08:09:27.000000 codeoven-0.1.3/src/codeoven.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-05-19 00:35:24.713052 codeoven-0.1.4/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 codeoven-0.1.4/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       67 2023-04-02 08:09:16.000000 codeoven-0.1.4/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)     6114 2023-05-19 00:35:24.713140 codeoven-0.1.4/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)     5147 2023-04-02 07:29:56.000000 codeoven-0.1.4/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 codeoven-0.1.4/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1068 2023-05-19 00:35:24.713507 codeoven-0.1.4/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 codeoven-0.1.4/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-05-19 00:35:24.709272 codeoven-0.1.4/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-05-19 00:35:24.711990 codeoven-0.1.4/src/codeoven/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       26 2023-04-02 07:38:59.000000 codeoven-0.1.4/src/codeoven/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)    18193 2023-05-19 00:34:03.000000 codeoven-0.1.4/src/codeoven/codeoven.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1612 2022-08-26 16:10:57.000000 codeoven-0.1.4/src/codeoven/oven_utils.c
+-rw-r--r--   0 shuntaro   (501) staff       (20)      194 2022-06-02 00:59:28.000000 codeoven-0.1.4/src/codeoven/oven_utils.h
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-05-19 00:35:24.712930 codeoven-0.1.4/src/codeoven.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     6114 2023-05-19 00:35:24.000000 codeoven-0.1.4/src/codeoven.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      348 2023-05-19 00:35:24.000000 codeoven-0.1.4/src/codeoven.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-05-19 00:35:24.000000 codeoven-0.1.4/src/codeoven.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       23 2023-05-19 00:35:24.000000 codeoven-0.1.4/src/codeoven.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        9 2023-05-19 00:35:24.000000 codeoven-0.1.4/src/codeoven.egg-info/top_level.txt
```

### Comparing `codeoven-0.1.3/LICENSE.txt` & `codeoven-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codeoven-0.1.3/PKG-INFO` & `codeoven-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeoven
-Version: 0.1.3
+Version: 0.1.4
 Summary: Effortlessly integrates C code with Python.
 Home-page: https://github.com/chocolate-icecream/codeoven
 Author: chocolate-icecream
 Project-URL: Bug Tracker, https://github.com/chocolate-icecream/codeoven/issues
 Keywords: Igor
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `codeoven-0.1.3/README.md` & `codeoven-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `codeoven-0.1.3/setup.cfg` & `codeoven-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = codeoven
-version = 0.1.3
+version = 0.1.4
 author = chocolate-icecream
 description = Effortlessly integrates C code with Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chocolate-icecream/codeoven
 project_urls = 
 	Bug Tracker = https://github.com/chocolate-icecream/codeoven/issues
```

### Comparing `codeoven-0.1.3/src/codeoven/codeoven.py` & `codeoven-0.1.4/src/codeoven/codeoven.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
                 output_codes.append(code.compose(parameters))
             if isinstance(code, (Array1D)):
                 output_codes.append(code.compose(parameters))
         return output_codes
 
     def flag_finder(self, code:str):
         if "<gsl" in code:
-                self.flag_dict["gsl"] = "-lgsl"
+                self.flag_dict["gsl"] = "-I /opt/homebrew/opt/gsl/include -L /opt/homebrew/opt/gsl/lib -lgsl -lgslcblas"
 
 class ProcessRunner:
     def __init__(self):
         self.result_dict = {}
 
     def run(self, exec_name):
         result = subprocess.run([exec_name], encoding="UTF-8", stdout=subprocess.PIPE)
```

### Comparing `codeoven-0.1.3/src/codeoven/oven_utils.c` & `codeoven-0.1.4/src/codeoven/oven_utils.c`

 * *Files identical despite different names*

### Comparing `codeoven-0.1.3/src/codeoven.egg-info/PKG-INFO` & `codeoven-0.1.4/src/codeoven.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeoven
-Version: 0.1.3
+Version: 0.1.4
 Summary: Effortlessly integrates C code with Python.
 Home-page: https://github.com/chocolate-icecream/codeoven
 Author: chocolate-icecream
 Project-URL: Bug Tracker, https://github.com/chocolate-icecream/codeoven/issues
 Keywords: Igor
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

