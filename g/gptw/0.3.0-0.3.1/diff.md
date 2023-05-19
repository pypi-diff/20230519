# Comparing `tmp/gptw-0.3.0.tar.gz` & `tmp/gptw-0.3.1.tar.gz`

## Comparing `gptw-0.3.0.tar` & `gptw-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.3.0/gptw/__init__.py
--rw-r--r--   0        0        0     5504 2020-02-02 00:00:00.000000 gptw-0.3.0/gptw/gptw.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 gptw-0.3.0/gptw/prompts.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.3.0/LICENSE
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 gptw-0.3.0/README.md
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 gptw-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 gptw-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.3.1/gptw/__init__.py
+-rw-r--r--   0        0        0     5504 2020-02-02 00:00:00.000000 gptw-0.3.1/gptw/gptw.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 gptw-0.3.1/gptw/prompts.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 gptw-0.3.1/README.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 gptw-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 gptw-0.3.1/PKG-INFO
```

### Comparing `gptw-0.3.0/gptw/gptw.py` & `gptw-0.3.1/gptw/gptw.py`

 * *Files identical despite different names*

### Comparing `gptw-0.3.0/gptw/prompts.json` & `gptw-0.3.1/gptw/prompts.json`

 * *Files identical despite different names*

### Comparing `gptw-0.3.0/.gitignore` & `gptw-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gptw-0.3.0/LICENSE` & `gptw-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gptw-0.3.0/README.md` & `gptw-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gptw-0.3.0/pyproject.toml` & `gptw-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Natural Language :: English",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 [project.scripts]
 gptw="gptw.gptw:main"
```

### Comparing `gptw-0.3.0/PKG-INFO` & `gptw-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: gptw
-Version: 0.3.0
+Version: 0.3.1
 Summary: The ChatGPT command-line wrapper simplifies the execution of predetermined tasks through ChatGPT.
 Author: Xin Yang
 Author-email: xinydev@gmail.com
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: ChatGPT,Command Line,English Polishing,English Translation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7.1
 Requires-Dist: argparse>=1.4.0
 Requires-Dist: openai>=0.27.0
 Requires-Dist: poe-api>=0.3.1
```

