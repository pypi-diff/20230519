# Comparing `tmp/veilcord-0.0.0.2.tar.gz` & `tmp/veilcord-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.0.2.tar", last modified: Thu May 18 23:24:59 2023, max compression
+gzip compressed data, was "veilcord-0.0.0.3.tar", last modified: Fri May 19 00:07:38 2023, max compression
```

## Comparing `veilcord-0.0.0.2.tar` & `veilcord-0.0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 23:24:59.228887 veilcord-0.0.0.2/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1926 2023-05-18 23:24:59.227890 veilcord-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-05-17 01:51:11.000000 veilcord-0.0.0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 23:24:59.228887 veilcord-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-05-18 23:23:33.000000 veilcord-0.0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 23:24:59.216918 veilcord-0.0.0.2/veilcord/
--rw-rw-rw-   0        0        0     8801 2023-05-17 02:45:43.000000 veilcord-0.0.0.2/veilcord/__init__.py
--rw-rw-rw-   0        0        0     7886 2023-05-18 22:17:53.000000 veilcord-0.0.0.2/veilcord/verification.py
-drwxrwxrwx   0        0        0        0 2023-05-18 23:24:59.226891 veilcord-0.0.0.2/veilcord.egg-info/
--rw-rw-rw-   0        0        0     1926 2023-05-18 23:24:59.000000 veilcord-0.0.0.2/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-18 23:24:59.000000 veilcord-0.0.0.2/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 23:24:59.000000 veilcord-0.0.0.2/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-18 23:24:59.000000 veilcord-0.0.0.2/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 23:24:59.000000 veilcord-0.0.0.2/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 00:07:38.548392 veilcord-0.0.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1926 2023-05-19 00:07:38.547393 veilcord-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-05-17 01:51:11.000000 veilcord-0.0.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 00:07:38.548392 veilcord-0.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-05-19 00:03:30.000000 veilcord-0.0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 00:07:38.540409 veilcord-0.0.0.3/veilcord/
+-rw-rw-rw-   0        0        0    13740 2023-05-19 00:06:20.000000 veilcord-0.0.0.3/veilcord/__init__.py
+-rw-rw-rw-   0        0        0     7885 2023-05-18 23:58:49.000000 veilcord-0.0.0.3/veilcord/verification.py
+drwxrwxrwx   0        0        0        0 2023-05-19 00:07:38.546396 veilcord-0.0.0.3/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     1926 2023-05-19 00:07:38.000000 veilcord-0.0.0.3/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-19 00:07:38.000000 veilcord-0.0.0.3/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 00:07:38.000000 veilcord-0.0.0.3/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-19 00:07:38.000000 veilcord-0.0.0.3/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 00:07:38.000000 veilcord-0.0.0.3/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.0.2/LICENSE` & `veilcord-0.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.2/PKG-INFO` & `veilcord-0.0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
```

### Comparing `veilcord-0.0.0.2/README.md` & `veilcord-0.0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.2/setup.py` & `veilcord-0.0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.2"
+vers = "0.0.0.3"
     
 setup(name="veilcord",
       version=vers,
       description="VeilCord // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `veilcord-0.0.0.2/veilcord/verification.py` & `veilcord-0.0.0.3/veilcord/verification.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     sessionThread = None
     sessionOn = True
     
     
 class Verification:
     def __init__(
         self, 
-        session: Optional[Session] = HTTPClient().session, 
+        session: Optional[Session] = HTTPClient().session,
         device_type: Literal["browser", "mobile"] = "browser", 
         user_agent: Optional[str] = None
     ) -> None:
         self.session = session
         self.user_agent_browser = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"
         self.user_agent_mobile = "Discord-Android/170014;RNA"
         self.device_type_browser = "Windows"
```

### Comparing `veilcord-0.0.0.2/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.0.3/veilcord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
```

