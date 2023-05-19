# Comparing `tmp/gpterminal-0.1.7.tar.gz` & `tmp/gpterminal-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpterminal-0.1.7.tar", last modified: Tue May 16 11:37:23 2023, max compression
+gzip compressed data, was "gpterminal-0.1.8.tar", last modified: Fri May 19 03:37:08 2023, max compression
```

## Comparing `gpterminal-0.1.7.tar` & `gpterminal-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 11:37:23.378929 gpterminal-0.1.7/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3187 2023-05-16 11:37:23.378371 gpterminal-0.1.7/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2433 2023-05-16 11:36:53.000000 gpterminal-0.1.7/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 11:37:23.373580 gpterminal-0.1.7/cli/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.7/cli/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.7/cli/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.7/cli/cli.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.7/cli/code_execution.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.7/cli/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 11:37:23.377322 gpterminal-0.1.7/gpterminal.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3187 2023-05-16 11:37:23.000000 gpterminal-0.1.7/gpterminal.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)      301 2023-05-16 11:37:23.000000 gpterminal-0.1.7/gpterminal.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-16 11:37:23.000000 gpterminal-0.1.7/gpterminal.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       42 2023-05-16 11:37:23.000000 gpterminal-0.1.7/gpterminal.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       59 2023-05-16 11:37:23.000000 gpterminal-0.1.7/gpterminal.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-16 11:37:23.000000 gpterminal-0.1.7/gpterminal.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-16 11:37:23.379133 gpterminal-0.1.7/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1276 2023-05-16 11:37:19.000000 gpterminal-0.1.7/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-19 03:37:08.721678 gpterminal-0.1.8/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3187 2023-05-19 03:37:08.721118 gpterminal-0.1.8/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2433 2023-05-16 11:36:53.000000 gpterminal-0.1.8/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-19 03:37:08.716244 gpterminal-0.1.8/cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.8/cli/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.8/cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.8/cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.8/cli/code_execution.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2525 2023-05-19 02:30:59.000000 gpterminal-0.1.8/cli/command_print.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4961 2023-05-19 03:36:56.000000 gpterminal-0.1.8/cli/gs.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.8/cli/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-19 03:37:08.719923 gpterminal-0.1.8/gpterminal.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3187 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      332 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       65 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       59 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-19 03:37:08.000000 gpterminal-0.1.8/gpterminal.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-19 03:37:08.721846 gpterminal-0.1.8/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1310 2023-05-19 03:37:04.000000 gpterminal-0.1.8/setup.py
```

### Comparing `gpterminal-0.1.7/PKG-INFO` & `gpterminal-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterminal
-Version: 0.1.7
+Version: 0.1.8
 Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
 Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gpterminal-0.1.7/README.md` & `gpterminal-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.7/cli/ChatGPT.py` & `gpterminal-0.1.8/cli/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.7/cli/cli.py` & `gpterminal-0.1.8/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.7/cli/code_execution.py` & `gpterminal-0.1.8/cli/code_execution.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.7/cli/utils.py` & `gpterminal-0.1.8/cli/utils.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.7/gpterminal.egg-info/PKG-INFO` & `gpterminal-0.1.8/gpterminal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterminal
-Version: 0.1.7
+Version: 0.1.8
 Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
 Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gpterminal-0.1.7/setup.py` & `gpterminal-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gpterminal",
-    version="0.1.7",
+    version="0.1.8",
     author="Your Name",
     author_email="your.email@example.com",
     description="A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yourusername/gpterminal",
     packages=find_packages(),
@@ -33,10 +33,11 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     python_requires=">=3.6",
     entry_points={
         "console_scripts": [
             "gt=cli.cli:gpterminal",
+            "gs=cli.gs:gpterminal"
         ],
     },
-)
+)
```

