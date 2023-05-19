# Comparing `tmp/gmpg-0.1.4.tar.gz` & `tmp/gmpg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmpg-0.1.4.tar", max compression
+gzip compressed data, was "gmpg-0.1.5.tar", max compression
```

## Comparing `gmpg-0.1.4.tar` & `gmpg-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      407 2023-01-27 00:43:43.216118 gmpg-0.1.4/gmpg/__init__.py
--rw-r--r--   0        0        0    10896 2023-01-27 00:43:43.216118 gmpg-0.1.4/gmpg/__main__.py
--rw-r--r--   0        0        0        0 2023-01-27 00:43:43.208118 gmpg-0.1.4/gmpg/_pkg/__init__.py
--rw-r--r--   0        0        0     2356 2023-01-27 00:43:43.204118 gmpg-0.1.4/gmpg/_pkg/install.py
--rw-r--r--   0        0        0     4554 2023-01-27 00:43:43.204118 gmpg-0.1.4/gmpg/_pkg/licensing/__init__.py
--rw-r--r--   0        0        0     1876 2023-01-27 00:43:43.204118 gmpg-0.1.4/gmpg/_pkg/licensing/licenses.json
--rw-r--r--   0        0        0     5185 2023-01-27 00:43:43.208118 gmpg-0.1.4/gmpg/_pkg/listing.py
--rwxr-xr-x   0        0        0       80 2023-01-27 00:43:43.208118 gmpg-0.1.4/gmpg/_pkg/runinenv
--rw-r--r--   0        0        0      497 2023-01-27 00:43:43.212118 gmpg-0.1.4/gmpg/_pkg/system.py
--rw-r--r--   0        0        0    12067 2023-05-18 22:43:58.957203 gmpg-0.1.4/gmpg/analysis.py
--rw-r--r--   0        0        0    11980 2023-01-28 00:07:01.355399 gmpg-0.1.4/gmpg/git.py
--rw-r--r--   0        0        0     6329 2023-01-27 00:43:43.216118 gmpg-0.1.4/gmpg/ide.py
--rw-r--r--   0        0        0     7161 2023-05-18 23:42:42.179473 gmpg-0.1.4/gmpg/pkg.py
--rw-r--r--   0        0        0     1011 2023-05-18 23:43:13.715967 gmpg-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 gmpg-0.1.4/setup.py
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 gmpg-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      407 2023-01-27 00:43:43.216118 gmpg-0.1.5/gmpg/__init__.py
+-rw-r--r--   0        0        0    10896 2023-01-27 00:43:43.216118 gmpg-0.1.5/gmpg/__main__.py
+-rw-r--r--   0        0        0        0 2023-01-27 00:43:43.208118 gmpg-0.1.5/gmpg/_pkg/__init__.py
+-rw-r--r--   0        0        0     2356 2023-01-27 00:43:43.204118 gmpg-0.1.5/gmpg/_pkg/install.py
+-rw-r--r--   0        0        0     4554 2023-01-27 00:43:43.204118 gmpg-0.1.5/gmpg/_pkg/licensing/__init__.py
+-rw-r--r--   0        0        0     1876 2023-01-27 00:43:43.204118 gmpg-0.1.5/gmpg/_pkg/licensing/licenses.json
+-rw-r--r--   0        0        0     5185 2023-01-27 00:43:43.208118 gmpg-0.1.5/gmpg/_pkg/listing.py
+-rwxr-xr-x   0        0        0       80 2023-01-27 00:43:43.208118 gmpg-0.1.5/gmpg/_pkg/runinenv
+-rw-r--r--   0        0        0      497 2023-01-27 00:43:43.212118 gmpg-0.1.5/gmpg/_pkg/system.py
+-rw-r--r--   0        0        0    12067 2023-05-18 22:43:58.957203 gmpg-0.1.5/gmpg/analysis.py
+-rw-r--r--   0        0        0    12028 2023-05-19 19:50:12.909776 gmpg-0.1.5/gmpg/git.py
+-rw-r--r--   0        0        0     6329 2023-01-27 00:43:43.216118 gmpg-0.1.5/gmpg/ide.py
+-rw-r--r--   0        0        0     7161 2023-05-18 23:42:42.179473 gmpg-0.1.5/gmpg/pkg.py
+-rw-r--r--   0        0        0     1011 2023-05-19 19:51:59.503814 gmpg-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 gmpg-0.1.5/setup.py
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 gmpg-0.1.5/PKG-INFO
```

### Comparing `gmpg-0.1.4/gmpg/__main__.py` & `gmpg-0.1.5/gmpg/__main__.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.4/gmpg/_pkg/install.py` & `gmpg-0.1.5/gmpg/_pkg/install.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.4/gmpg/_pkg/licensing/__init__.py` & `gmpg-0.1.5/gmpg/_pkg/licensing/__init__.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.4/gmpg/_pkg/licensing/licenses.json` & `gmpg-0.1.5/gmpg/_pkg/licensing/licenses.json`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.4/gmpg/_pkg/listing.py` & `gmpg-0.1.5/gmpg/_pkg/listing.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.4/gmpg/analysis.py` & `gmpg-0.1.5/gmpg/analysis.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.4/gmpg/git.py` & `gmpg-0.1.5/gmpg/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 ) -> Repository:
     """Return a Repository for given location."""
     location = Path(location)
     if gpg_home:
         gpg_home = Path(gpg_home)
     # if not Path(location).exists():
     if init:
-        args = ["git", "init", "-b", "main", str(location)]
+        # args = ["git", "init", "-b", "main", str(location)]
+        args = ["git", "init", str(location)]
         if bare:
             args.append("--bare")
         subprocess.check_call(args)
     # else:
     #     raise FileNotFoundError("repository does not exist "
     #                             "at {}".format(str(location)))
     return Repository(location, gpg_home=gpg_home)
```

### Comparing `gmpg-0.1.4/gmpg/ide.py` & `gmpg-0.1.5/gmpg/ide.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.4/gmpg/pkg.py` & `gmpg-0.1.5/gmpg/pkg.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.4/pyproject.toml` & `gmpg-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmpg"
-version = "0.1.4"
+version = "0.1.5"
 description = "tools for metamodern software development"
 keywords = ["Git", "Poetry"]
 homepage = "https://ragt.ag/code/projects/gmpg"
 repository = "https://ragt.ag/code/projects/gmpg.git"
 documentation = "https://ragt.ag/code/projects/gmpg/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
```

### Comparing `gmpg-0.1.4/setup.py` & `gmpg-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'txtint>=0.0.0']
 
 entry_points = \
 {'console_scripts': ['gmpg = gmpg.__main__:main']}
 
 setup_kwargs = {
     'name': 'gmpg',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'tools for metamodern software development',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/gmpg',
```

### Comparing `gmpg-0.1.4/PKG-INFO` & `gmpg-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmpg
-Version: 0.1.4
+Version: 0.1.5
 Summary: tools for metamodern software development
 Home-page: https://ragt.ag/code/projects/gmpg
 License: BSD-2-Clause
 Keywords: Git,Poetry
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.8,<3.11
```

