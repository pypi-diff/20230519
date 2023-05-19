# Comparing `tmp/noiftimer-2.1.0.tar.gz` & `tmp/noiftimer-2.2.0.tar.gz`

## Comparing `noiftimer-2.1.0.tar` & `noiftimer-2.2.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 noiftimer-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 noiftimer-2.1.0/docs/index.html
--rw-r--r--   0        0        0    34120 2020-02-02 00:00:00.000000 noiftimer-2.1.0/docs/noiftimer.html
--rw-r--r--   0        0        0    26805 2020-02-02 00:00:00.000000 noiftimer-2.1.0/docs/search.js
--rw-r--r--   0        0        0   151271 2020-02-02 00:00:00.000000 noiftimer-2.1.0/docs/noiftimer/noiftimer.html
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 noiftimer-2.1.0/src/noiftimer/__init__.py
--rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 noiftimer-2.1.0/src/noiftimer/noiftimer.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 noiftimer-2.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 noiftimer-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 noiftimer-2.1.0/README.md
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 noiftimer-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 noiftimer-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 noiftimer-2.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 noiftimer-2.2.0/docs/index.html
+-rw-r--r--   0        0        0    34194 2020-02-02 00:00:00.000000 noiftimer-2.2.0/docs/noiftimer.html
+-rw-r--r--   0        0        0    27924 2020-02-02 00:00:00.000000 noiftimer-2.2.0/docs/search.js
+-rw-r--r--   0        0        0   151271 2020-02-02 00:00:00.000000 noiftimer-2.2.0/docs/noiftimer/noiftimer.html
+-rw-r--r--   0        0        0    48439 2020-02-02 00:00:00.000000 noiftimer-2.2.0/docs/noiftimer/stopwatch.html
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 noiftimer-2.2.0/src/noiftimer/__init__.py
+-rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 noiftimer-2.2.0/src/noiftimer/noiftimer.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 noiftimer-2.2.0/src/noiftimer/stopwatch.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 noiftimer-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 noiftimer-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 noiftimer-2.2.0/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 noiftimer-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 noiftimer-2.2.0/PKG-INFO
```

### Comparing `noiftimer-2.1.0/CHANGELOG.md` & `noiftimer-2.2.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 # Changelog
 
-## 2.0.0 (2023-04-15)
+## 2.1.0 (2023-05-10)
+
+#### New Features
+
+* Add `pause` and `unpause` methods to `Timer`.
+#### Performance improvements
+
+* start() and stop() check whether the timer is running or not before performing their actions
+#### Docs
+
+* update and reformat docstrings
+#### Others
+
+* change minimum python version to 3.10
+
+
+## v2.0.0 (2023-04-15)
 
 #### New Features
 
 * add history property
 * make Self typing python 3.10 compatible
 #### Fixes
 
@@ -13,14 +29,16 @@
 #### Refactorings
 
 * convert most members to properties
 * revert datetime library usage back to time library
 * import Self from typing_extensions
 #### Others
 
+* build v2.0.0
+* update changelog
 * update readme
 * remove unused import
 * remove current_elapsed_time() making package compatible with python >=3.6
 
 
 ## v1.3.0 (2023-03-31)
```

### Comparing `noiftimer-2.1.0/docs/noiftimer.html` & `noiftimer-2.2.0/docs/noiftimer.html`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             <input type="search" placeholder="Search..." role="searchbox" aria-label="search"
                    pattern=".+" required>
 
 
         <h2>Submodules</h2>
         <ul>
                 <li><a href="noiftimer/noiftimer.html">noiftimer</a></li>
+                <li><a href="noiftimer/stopwatch.html">stopwatch</a></li>
         </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
                 alt="pdoc logo"
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 
 
   ⁰
 [Unknown INPUT type]
 ***** Submodules *****
     * noiftimer
+    * stopwatch
 built_with_pdoc[pdoc_logo]
 
 ****** noiftimer ******
 ⁰ View Source
 1from .noiftimer import Timer, time_it
```

### Comparing `noiftimer-2.1.0/docs/search.js` & `noiftimer-2.2.0/docs/search.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -812,14 +812,43 @@
     }, {
         "fullname": "noiftimer.noiftimer.Timer.stats",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.stats",
         "kind": "variable",
         "doc": "<p>Returns a string stating the currently elapsed time and the average elapsed time.</p>\n",
         "annotation": ": str"
+    }, {
+        "fullname": "noiftimer.stopwatch",
+        "modulename": "noiftimer.stopwatch",
+        "kind": "module",
+        "doc": "<p></p>\n"
+    }, {
+        "fullname": "noiftimer.stopwatch.input_",
+        "modulename": "noiftimer.stopwatch",
+        "qualname": "input_",
+        "kind": "function",
+        "doc": "<p></p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">prompt</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "noiftimer.stopwatch.stopwatch",
+        "modulename": "noiftimer.stopwatch",
+        "qualname": "stopwatch",
+        "kind": "function",
+        "doc": "<p></p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "noiftimer.stopwatch.main",
+        "modulename": "noiftimer.stopwatch",
+        "qualname": "main",
+        "kind": "function",
+        "doc": "<p></p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
     }];
 
     // mirrored in build-search-index.js (part 1)
     // Also split on html tags. this is a cheap heuristic, but good enough.
     elasticlunr.tokenizer.setSeperator(/[\s\-.;&_'"=,()]+|<[^>]*>/);
 
     let searchIndex;
```

### Comparing `noiftimer-2.1.0/docs/noiftimer/noiftimer.html` & `noiftimer-2.2.0/docs/noiftimer/noiftimer.html`

 * *Files identical despite different names*

### Comparing `noiftimer-2.1.0/src/noiftimer/noiftimer.py` & `noiftimer-2.2.0/src/noiftimer/noiftimer.py`

 * *Files identical despite different names*

### Comparing `noiftimer-2.1.0/LICENSE.txt` & `noiftimer-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `noiftimer-2.1.0/README.md` & `noiftimer-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `noiftimer-2.1.0/pyproject.toml` & `noiftimer-2.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "noiftimer"
 authors = [{name="Matt Manes"}]
 description = "Timing class for measuring elapsed time and average elapsed time."
-version = "2.1.0"
+version = "2.2.0"
 requires-python = ">=3.10"
-dependencies = ["pytest", "typing_extensions"]
+dependencies = ["pytest", "typing_extensions", "printbuddies"]
 readme = "README.md"
 keywords = [
     "timer",
     "timing"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -33,8 +33,11 @@
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     ".coverage",
     ".pytest_cache",
     ".vscode",
     "tests"
-]
+]
+
+[project.scripts]
+stopwatch = "noiftimer.stopwatch:main"
```

### Comparing `noiftimer-2.1.0/PKG-INFO` & `noiftimer-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: noiftimer
-Version: 2.1.0
+Version: 2.2.0
 Summary: Timing class for measuring elapsed time and average elapsed time.
 Project-URL: Homepage, https://github.com/matt-manes/noiftimer
 Project-URL: Documentation, https://github.com/matt-manes/noiftimer/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/noiftimer/tree/main/src/noiftimer
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: timer,timing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: printbuddies
 Requires-Dist: pytest
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # noiftimer
 Simple timer class to track elapsed time.<br>
 Install with:
```

