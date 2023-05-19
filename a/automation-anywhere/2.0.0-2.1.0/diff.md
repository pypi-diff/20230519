# Comparing `tmp/automation_anywhere-2.0.0.tar.gz` & `tmp/automation_anywhere-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_anywhere-2.0.0.tar", last modified: Fri May  5 19:03:06 2023, max compression
+gzip compressed data, was "automation_anywhere-2.1.0.tar", last modified: Fri May 19 19:11:37 2023, max compression
```

## Comparing `automation_anywhere-2.0.0.tar` & `automation_anywhere-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:03:06.632693 automation_anywhere-2.0.0/
--rw-rw-rw-   0        0        0     1088 2023-05-03 18:24:17.000000 automation_anywhere-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     2386 2023-05-05 19:03:06.629692 automation_anywhere-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1794 2023-05-05 18:54:19.000000 automation_anywhere-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 19:03:06.434035 automation_anywhere-2.0.0/automation_anywhere/
--rw-rw-rw-   0        0        0       57 2023-05-03 18:24:17.000000 automation_anywhere-2.0.0/automation_anywhere/__init__.py
--rw-rw-rw-   0        0        0     4171 2023-05-05 18:15:54.000000 automation_anywhere-2.0.0/automation_anywhere/base.py
--rw-rw-rw-   0        0        0      190 2023-05-05 16:43:55.000000 automation_anywhere-2.0.0/automation_anywhere/errors.py
--rw-rw-rw-   0        0        0     7724 2023-05-05 18:30:08.000000 automation_anywhere-2.0.0/automation_anywhere/executor.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:03:06.620635 automation_anywhere-2.0.0/automation_anywhere.egg-info/
--rw-rw-rw-   0        0        0     2386 2023-05-05 19:03:06.000000 automation_anywhere-2.0.0/automation_anywhere.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-05-05 19:03:06.000000 automation_anywhere-2.0.0/automation_anywhere.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:03:06.000000 automation_anywhere-2.0.0/automation_anywhere.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-05 19:03:06.000000 automation_anywhere-2.0.0/automation_anywhere.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      661 2023-05-05 19:02:29.000000 automation_anywhere-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 19:03:06.633691 automation_anywhere-2.0.0/setup.cfg
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:11:37.676112 automation_anywhere-2.1.0/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.0/LICENSE
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-19 19:11:37.676112 automation_anywhere-2.1.0/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3431 2023-05-19 18:02:53.000000 automation_anywhere-2.1.0/README.md
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:11:37.676112 automation_anywhere-2.1.0/automation_anywhere/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.0/automation_anywhere/__init__.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4068 2023-05-11 13:45:41.000000 automation_anywhere-2.1.0/automation_anywhere/base.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.0/automation_anywhere/errors.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)    10108 2023-05-19 18:00:11.000000 automation_anywhere-2.1.0/automation_anywhere/executor.py
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:11:37.676112 automation_anywhere-2.1.0/automation_anywhere.egg-info/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-19 19:11:37.000000 automation_anywhere-2.1.0/automation_anywhere.egg-info/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-05-19 19:11:37.000000 automation_anywhere-2.1.0/automation_anywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-05-19 19:11:37.000000 automation_anywhere-2.1.0/automation_anywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-05-19 19:11:37.000000 automation_anywhere-2.1.0/automation_anywhere.egg-info/top_level.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-05-19 19:10:11.000000 automation_anywhere-2.1.0/pyproject.toml
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-05-19 19:11:37.676112 automation_anywhere-2.1.0/setup.cfg
```

### Comparing `automation_anywhere-2.0.0/LICENSE` & `automation_anywhere-2.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 minterciso
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2018 minterciso
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `automation_anywhere-2.0.0/pyproject.toml` & `automation_anywhere-2.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name="automation_anywhere"
-version="2.0.0"
-authors=[{name="Mateus Interciso", email="minterciso@gmail.com"}]
-description="A Python Package to deploy tasks on Automation Anywhere 360"
-readme="README.md"
-requires-python=">=3.9"
-classifiers = [
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/minterciso/pyAutomationAnywhere"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name="automation_anywhere"
+version="2.1.0"
+authors=[{name="Mateus Interciso", email="minterciso@gmail.com"}]
+description="A Python Package to deploy tasks on Automation Anywhere 360"
+readme="README.md"
+requires-python=">=3.9"
+classifiers = [
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/minterciso/pyAutomationAnywhere"
 "Bug Tracker" = "https://github.com/minterciso/pyAutomationAnywhere/issues"
```

