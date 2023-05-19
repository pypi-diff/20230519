# Comparing `tmp/arithmetic-dice-roller-0.3.0.tar.gz` & `tmp/arithmetic-dice-roller-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetic-dice-roller-0.3.0.tar", last modified: Fri May 19 08:31:05 2023, max compression
+gzip compressed data, was "arithmetic-dice-roller-0.3.1.tar", last modified: Fri May 19 08:48:25 2023, max compression
```

## Comparing `arithmetic-dice-roller-0.3.0.tar` & `arithmetic-dice-roller-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-05-19 08:31:05.150281 arithmetic-dice-roller-0.3.0/
--rw-r--r--   0 damax     (1000) damax     (1000)     4593 2023-05-19 08:31:05.150281 arithmetic-dice-roller-0.3.0/PKG-INFO
--rw-r--r--   0 damax     (1000) damax     (1000)     4054 2022-03-02 13:20:22.000000 arithmetic-dice-roller-0.3.0/README.md
-drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-05-19 08:31:05.150281 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/
--rw-r--r--   0 damax     (1000) damax     (1000)        0 2021-11-05 13:05:11.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/__init__.py
--rw-r--r--   0 damax     (1000) damax     (1000)     1956 2022-12-13 12:06:00.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/__main__.py
--rw-r--r--   0 damax     (1000) damax     (1000)    11783 2023-05-19 08:28:18.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/roller.py
-drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-05-19 08:31:05.150281 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/
--rw-r--r--   0 damax     (1000) damax     (1000)     4593 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/PKG-INFO
--rw-r--r--   0 damax     (1000) damax     (1000)      399 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/SOURCES.txt
--rw-r--r--   0 damax     (1000) damax     (1000)        1 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/dependency_links.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       80 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/entry_points.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       12 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/requires.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       23 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/top_level.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       38 2023-05-19 08:31:05.150281 arithmetic-dice-roller-0.3.0/setup.cfg
--rw-r--r--   0 damax     (1000) damax     (1000)     1712 2023-05-19 08:29:08.000000 arithmetic-dice-roller-0.3.0/setup.py
+drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-05-19 08:48:25.882228 arithmetic-dice-roller-0.3.1/
+-rw-r--r--   0 damax     (1000) damax     (1000)     4593 2023-05-19 08:48:25.882228 arithmetic-dice-roller-0.3.1/PKG-INFO
+-rw-r--r--   0 damax     (1000) damax     (1000)     4054 2023-05-19 08:47:31.000000 arithmetic-dice-roller-0.3.1/README.md
+drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-05-19 08:48:25.882228 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller/
+-rw-r--r--   0 damax     (1000) damax     (1000)        0 2021-11-05 13:05:11.000000 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller/__init__.py
+-rw-r--r--   0 damax     (1000) damax     (1000)     1956 2022-12-13 12:06:00.000000 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller/__main__.py
+-rw-r--r--   0 damax     (1000) damax     (1000)    11783 2023-05-19 08:28:18.000000 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller/roller.py
+drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-05-19 08:48:25.882228 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller.egg-info/
+-rw-r--r--   0 damax     (1000) damax     (1000)     4593 2023-05-19 08:48:25.000000 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller.egg-info/PKG-INFO
+-rw-r--r--   0 damax     (1000) damax     (1000)      399 2023-05-19 08:48:25.000000 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller.egg-info/SOURCES.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)        1 2023-05-19 08:48:25.000000 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller.egg-info/dependency_links.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       80 2023-05-19 08:48:25.000000 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller.egg-info/entry_points.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       12 2023-05-19 08:48:25.000000 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller.egg-info/requires.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       23 2023-05-19 08:48:25.000000 arithmetic-dice-roller-0.3.1/arithmetic_dice_roller.egg-info/top_level.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       38 2023-05-19 08:48:25.882228 arithmetic-dice-roller-0.3.1/setup.cfg
+-rw-r--r--   0 damax     (1000) damax     (1000)     1712 2023-05-19 08:47:51.000000 arithmetic-dice-roller-0.3.1/setup.py
```

### Comparing `arithmetic-dice-roller-0.3.0/PKG-INFO` & `arithmetic-dice-roller-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arithmetic-dice-roller
-Version: 0.3.0
+Version: 0.3.1
 Summary: A handy dice roller with extended notation and arithmetic expressions management.
 Home-page: https://github.com/massimopavoni/arithmetic-dice-roller
 Author: Massimo Pavoni
 Author-email: maspavoni@gmail.com
 Platform: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -12,15 +12,15 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # arithmetic-dice-roller
 [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/massimopavoni/arithmetic-dice-roller?include_prereleases)](https://github.com/massimopavoni/arithmetic-dice-roller/releases)
 [![PyPI Package](https://img.shields.io/pypi/v/arithmetic-dice-roller)](https://pypi.org/project/arithmetic-dice-roller/)
 [![GitHub License](https://img.shields.io/github/license/massimopavoni/arithmetic-dice-roller)](https://github.com/massimopavoni/arithmetic-dice-roller/blob/main/LICENSE)
-[![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3100/)
+[![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3110/)
 
 [![Discord](https://img.shields.io/discord/926217143194886234?label=Join%20Not%20Declared%20Developers)](https://discord.gg/ZA76nJ3RsU)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T8BD7A1)
 
 A handy dice roller with extended notation and arithmetic expressions' management.
```

### Comparing `arithmetic-dice-roller-0.3.0/README.md` & `arithmetic-dice-roller-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # arithmetic-dice-roller
 [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/massimopavoni/arithmetic-dice-roller?include_prereleases)](https://github.com/massimopavoni/arithmetic-dice-roller/releases)
 [![PyPI Package](https://img.shields.io/pypi/v/arithmetic-dice-roller)](https://pypi.org/project/arithmetic-dice-roller/)
 [![GitHub License](https://img.shields.io/github/license/massimopavoni/arithmetic-dice-roller)](https://github.com/massimopavoni/arithmetic-dice-roller/blob/main/LICENSE)
-[![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3100/)
+[![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3110/)
 
 [![Discord](https://img.shields.io/discord/926217143194886234?label=Join%20Not%20Declared%20Developers)](https://discord.gg/ZA76nJ3RsU)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T8BD7A1)
 
 A handy dice roller with extended notation and arithmetic expressions' management.
```

### Comparing `arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/__main__.py` & `arithmetic-dice-roller-0.3.1/arithmetic_dice_roller/__main__.py`

 * *Files identical despite different names*

### Comparing `arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/roller.py` & `arithmetic-dice-roller-0.3.1/arithmetic_dice_roller/roller.py`

 * *Files identical despite different names*

### Comparing `arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/PKG-INFO` & `arithmetic-dice-roller-0.3.1/arithmetic_dice_roller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arithmetic-dice-roller
-Version: 0.3.0
+Version: 0.3.1
 Summary: A handy dice roller with extended notation and arithmetic expressions management.
 Home-page: https://github.com/massimopavoni/arithmetic-dice-roller
 Author: Massimo Pavoni
 Author-email: maspavoni@gmail.com
 Platform: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -12,15 +12,15 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # arithmetic-dice-roller
 [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/massimopavoni/arithmetic-dice-roller?include_prereleases)](https://github.com/massimopavoni/arithmetic-dice-roller/releases)
 [![PyPI Package](https://img.shields.io/pypi/v/arithmetic-dice-roller)](https://pypi.org/project/arithmetic-dice-roller/)
 [![GitHub License](https://img.shields.io/github/license/massimopavoni/arithmetic-dice-roller)](https://github.com/massimopavoni/arithmetic-dice-roller/blob/main/LICENSE)
-[![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3100/)
+[![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3110/)
 
 [![Discord](https://img.shields.io/discord/926217143194886234?label=Join%20Not%20Declared%20Developers)](https://discord.gg/ZA76nJ3RsU)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T8BD7A1)
 
 A handy dice roller with extended notation and arithmetic expressions' management.
```

### Comparing `arithmetic-dice-roller-0.3.0/setup.py` & `arithmetic-dice-roller-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from setuptools import setup, find_packages
 
 README = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='arithmetic-dice-roller',
-    version='0.3.0',
+    version='0.3.1',
     description="A handy dice roller with extended notation and arithmetic expressions management.",
     long_description=README,
     long_description_content_type="text/markdown",
     author='Massimo Pavoni',
     author_email='maspavoni@gmail.com',
     url='https://github.com/massimopavoni/arithmetic-dice-roller',
     license_files='LICENSE',
```

