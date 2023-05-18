# Comparing `tmp/veilcord-0.0.0.1.tar.gz` & `tmp/veilcord-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.0.1.tar", last modified: Wed May 17 01:49:52 2023, max compression
+gzip compressed data, was "veilcord-0.0.0.2.tar", last modified: Thu May 18 23:24:59 2023, max compression
```

## Comparing `veilcord-0.0.0.1.tar` & `veilcord-0.0.0.2.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 01:49:52.561590 veilcord-0.0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1922 2023-05-17 01:49:52.560593 veilcord-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      744 2023-05-17 01:49:03.000000 veilcord-0.0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 01:49:52.561590 veilcord-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1600 2023-05-17 01:49:20.000000 veilcord-0.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 01:49:52.542128 veilcord-0.0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 01:48:15.000000 veilcord-0.0.0.1/tests/testing.py
-drwxrwxrwx   0        0        0        0 2023-05-17 01:49:52.544122 veilcord-0.0.0.1/veilcord/
--rw-rw-rw-   0        0        0        0 2023-05-17 01:46:59.000000 veilcord-0.0.0.1/veilcord/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-17 01:46:52.000000 veilcord-0.0.0.1/veilcord/main.py
-drwxrwxrwx   0        0        0        0 2023-05-17 01:49:52.559594 veilcord-0.0.0.1/veilcord.egg-info/
--rw-rw-rw-   0        0        0     1922 2023-05-17 01:49:52.000000 veilcord-0.0.0.1/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-05-17 01:49:52.000000 veilcord-0.0.0.1/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 01:49:52.000000 veilcord-0.0.0.1/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-17 01:49:52.000000 veilcord-0.0.0.1/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-17 01:49:52.000000 veilcord-0.0.0.1/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 23:24:59.228887 veilcord-0.0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1926 2023-05-18 23:24:59.227890 veilcord-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-05-17 01:51:11.000000 veilcord-0.0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 23:24:59.228887 veilcord-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-05-18 23:23:33.000000 veilcord-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 23:24:59.216918 veilcord-0.0.0.2/veilcord/
+-rw-rw-rw-   0        0        0     8801 2023-05-17 02:45:43.000000 veilcord-0.0.0.2/veilcord/__init__.py
+-rw-rw-rw-   0        0        0     7886 2023-05-18 22:17:53.000000 veilcord-0.0.0.2/veilcord/verification.py
+drwxrwxrwx   0        0        0        0 2023-05-18 23:24:59.226891 veilcord-0.0.0.2/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     1926 2023-05-18 23:24:59.000000 veilcord-0.0.0.2/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-18 23:24:59.000000 veilcord-0.0.0.2/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 23:24:59.000000 veilcord-0.0.0.2/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-18 23:24:59.000000 veilcord-0.0.0.2/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 23:24:59.000000 veilcord-0.0.0.2/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.0.1/LICENSE` & `veilcord-0.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.1/PKG-INFO` & `veilcord-0.0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
@@ -28,15 +28,15 @@
 License-File: LICENSE
 
 # VeilCord.
 <img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
 ```less
-                > Custom Console Going To Be Used For My Projects
+              > Custom Discord Tools Going To Be Used For My Projects
                     And Available To Anyone Else Who Wants To Use <
 ```
 
 ---
 
 ### Installation
 ```yaml
```

### Comparing `veilcord-0.0.0.1/README.md` & `veilcord-0.0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # VeilCord.
 <img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
 ```less
-                > Custom Console Going To Be Used For My Projects
+              > Custom Discord Tools Going To Be Used For My Projects
                     And Available To Anyone Else Who Wants To Use <
 ```
 
 ---
 
 ### Installation
 ```yaml
```

### Comparing `veilcord-0.0.0.1/setup.py` & `veilcord-0.0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.001"
+vers = "0.0.0.2"
     
 setup(name="veilcord",
       version=vers,
       description="VeilCord // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
@@ -35,11 +35,11 @@
         'Homepage': 'https://github.com/imvast/veilcord',
         'Suggestions': 'https://github.com/imvast/veilcord/issues',
       },
     
       python_requires="~=3.7",
 
       install_requires=[
-          "colorama>=0.4.6",
-          "requests>=2.30.0"
+          "terminut>=0.0.0.869",
+          "tls_client>=0.2.1"
       ]
 )
```

### Comparing `veilcord-0.0.0.1/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.0.2/veilcord.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
@@ -28,15 +28,15 @@
 License-File: LICENSE
 
 # VeilCord.
 <img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
 ```less
-                > Custom Console Going To Be Used For My Projects
+              > Custom Discord Tools Going To Be Used For My Projects
                     And Available To Anyone Else Who Wants To Use <
 ```
 
 ---
 
 ### Installation
 ```yaml
```

