# Comparing `tmp/streaming_jupyter_integrations-0.9.0.tar.gz` & `tmp/streaming_jupyter_integrations-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming_jupyter_integrations-0.9.0.tar", last modified: Thu Oct 20 07:10:20 2022, max compression
+gzip compressed data, was "streaming_jupyter_integrations-0.9.1.tar", last modified: Tue Oct 25 06:44:03 2022, max compression
```

## Comparing `streaming_jupyter_integrations-0.9.0.tar` & `streaming_jupyter_integrations-0.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:10:20.509444 streaming_jupyter_integrations-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3929 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3531 2022-10-20 07:10:20.509444 streaming_jupyter_integrations-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2958 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/install.json
--rw-r--r--   0 runner    (1001) docker     (121)     3368 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/package.json
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-10-20 07:10:20.509444 streaming_jupyter_integrations-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:10:20.505444 streaming_jupyter_integrations-0.9.0/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/src/extractors.ts
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:10:20.505444 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/deployment_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/jar_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:10:20.509444 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/labextension/
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-10-20 07:10:20.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:10:20.509444 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-10-20 07:10:20.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/labextension/static/475.73d1c5756e0a21e08d7c.js
--rw-r--r--   0 runner    (1001) docker     (121)     6235 2022-10-20 07:10:20.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/labextension/static/remoteEntry.850f660cc32e4df795fe.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-20 07:10:19.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-20 07:10:20.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (121)    23422 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/magics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/reflection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/sql_syntax_highlighting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4749 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/variable_substitution.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 07:10:20.509444 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3531 2022-10-20 07:10:20.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-10-20 07:10:20.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 07:10:20.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-20 07:10:20.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-20 07:10:20.000000 streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-10-20 07:09:03.000000 streaming_jupyter_integrations-0.9.0/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (121)   285060 2022-10-20 07:10:06.000000 streaming_jupyter_integrations-0.9.0/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:44:03.289077 streaming_jupyter_integrations-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     4182 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3531 2022-10-25 06:44:03.289077 streaming_jupyter_integrations-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2958 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/install.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3368 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-10-25 06:44:03.289077 streaming_jupyter_integrations-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:44:03.289077 streaming_jupyter_integrations-0.9.1/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/src/extractors.ts
+-rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:44:03.289077 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/deployment_bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/jar_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:44:03.289077 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/labextension/
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-10-25 06:44:03.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:44:03.289077 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-10-25 06:44:03.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/labextension/static/475.2dfb31799d45d3c229a6.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6235 2022-10-25 06:44:03.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/labextension/static/remoteEntry.1416e850b5547380e0e5.js
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-25 06:44:01.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-25 06:44:03.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (121)    24012 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/magics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/sql_syntax_highlighting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5111 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/variable_substitution.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 06:44:03.289077 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3531 2022-10-25 06:44:03.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-10-25 06:44:03.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 06:44:03.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-25 06:44:03.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-25 06:44:03.000000 streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-10-25 06:42:34.000000 streaming_jupyter_integrations-0.9.1/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (121)   285060 2022-10-25 06:43:46.000000 streaming_jupyter_integrations-0.9.1/yarn.lock
```

### Comparing `streaming_jupyter_integrations-0.9.0/CHANGELOG.md` & `streaming_jupyter_integrations-0.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.9.1] - 2022-10-25
+
+### Added
+
+-   Show functions & change icon for views in `%flink_show_table_tree`
+
+### Fixed
+
+-   Skip curly brackets without variable
+
 ## [0.9.0] - 2022-10-20
 
 ### Added
 
 -   Support for batch mode
 
 ### Fixed
@@ -109,15 +119,17 @@
 
 ## [0.1.4] - 2022-05-10
 
 ## [0.1.3] - 2022-05-09
 
 -   First release
 
-[Unreleased]: https://github.com/getindata/streaming-jupyter-integrations/compare/0.9.0...HEAD
+[Unreleased]: https://github.com/getindata/streaming-jupyter-integrations/compare/0.9.1...HEAD
+
+[0.9.1]: https://github.com/getindata/streaming-jupyter-integrations/compare/0.9.0...0.9.1
 
 [0.9.0]: https://github.com/getindata/streaming-jupyter-integrations/compare/0.8.2...0.9.0
 
 [0.8.2]: https://github.com/getindata/streaming-jupyter-integrations/compare/0.8.1...0.8.2
 
 [0.8.1]: https://github.com/getindata/streaming-jupyter-integrations/compare/0.8.0...0.8.1
```

### Comparing `streaming_jupyter_integrations-0.9.0/LICENSE` & `streaming_jupyter_integrations-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/PKG-INFO` & `streaming_jupyter_integrations-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming_jupyter_integrations
-Version: 0.9.0
+Version: 0.9.1
 Summary: JupyterNotebook Flink magics
 Home-page: https://github.com/getindata/streaming-jupyter-integrations
 Author: GetInData
 Author-email: office@getindata.com
 License: Apache Software License (Apache 2.0)
 Keywords: jupyter flink sql ipython
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `streaming_jupyter_integrations-0.9.0/README.md` & `streaming_jupyter_integrations-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/package.json` & `streaming_jupyter_integrations-0.9.1/package.json`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/setup.cfg` & `streaming_jupyter_integrations-0.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.0
+current_version = 0.9.1
 
 [tox:tox]
 envlist = py38
 
 [testenv]
 extras = tests
 commands = python -m pytest --cov streaming_jupyter_integrations --cov-report xml --cov-report term-missing --ignore=venv
```

### Comparing `streaming_jupyter_integrations-0.9.0/setup.py` & `streaming_jupyter_integrations-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 from pathlib import Path
 from typing import List
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 HERE = Path(__file__).parent.resolve()
 
 # Get the package info from package.json
 pkg_json = json.loads((HERE / "package.json").read_bytes())
 lab_path = (HERE / pkg_json["jupyterlab"]["outputDir"])
```

### Comparing `streaming_jupyter_integrations-0.9.0/src/extractors.ts` & `streaming_jupyter_integrations-0.9.1/src/extractors.ts`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/src/index.ts` & `streaming_jupyter_integrations-0.9.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/deployment_bar.py` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/deployment_bar.py`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/jar_handler.py` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/jar_handler.py`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/labextension/package.json` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992559523809523%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.1416e850b5547380e0e5.js'}}"}*

```diff
@@ -43,15 +43,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.850f660cc32e4df795fe.js"
+            "load": "static/remoteEntry.1416e850b5547380e0e5.js"
         },
         "extension": true,
         "outputDir": "streaming_jupyter_integrations/labextension",
         "sharedPackages": {
             "@krassowski/jupyterlab-lsp": {
                 "bundled": false,
                 "singleton": true
```

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/labextension/static/475.73d1c5756e0a21e08d7c.js` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/labextension/static/475.2dfb31799d45d3c229a6.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunkflink_sql_lsp_extension = self.webpackChunkflink_sql_lsp_extension || []).push([
     [475], {
         475: (e, n, o) => {
             o.r(n), o.d(n, {
                 default: () => p
             });
-            var r = o(177),
+            var r = o(905),
                 t = o(252);
             const s = "(?:(?:.*?)://(?:.*))",
                 i = "(?:" + ["-l", "--connections"].join("|") + "|" + ["-x", "--close", "-c", "--creator", "-p", "--persist", "--append"].map((e => e + " \\w+")).join("|") + ")",
                 a = {
                     python: [new t.RegExpForeignCodeExtractor({
                         language: "sql",
                         pattern: `^%%flink_execute_sql(?: (?:${s}|${i}|(?:\\w+ << )|(?:\\w+@\\w+)))?\n?((?:.+\n)?(?:[^]*))`,
```

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/labextension/static/remoteEntry.850f660cc32e4df795fe.js` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/labextension/static/remoteEntry.1416e850b5547380e0e5.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, l, s, u, f, d, p, c, h, v = {
+    var e, r, t, n, o, i, a, l, s, u, f, p, d, c, h, v = {
             999: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(475).then((() => () => t(475))),
                         "./extension": () => t.e(475).then((() => () => t(475)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -35,15 +35,15 @@
         return v[e](t, t.exports, m), t.exports
     }
     m.m = v, m.c = g, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + ".73d1c5756e0a21e08d7c.js?v=73d1c5756e0a21e08d7c", m.g = function() {
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + ".2dfb31799d45d3c229a6.js?v=2dfb31799d45d3c229a6", m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "flink_sql_lsp_extension:", m.l = (t, n, o, i) => {
@@ -55,24 +55,24 @@
                     var f = s[u];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
                         a = f;
                         break
                     }
                 }
             a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, m.nc && a.setAttribute("nonce", m.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(p);
+            var p = (r, n) => {
+                    a.onerror = a.onload = null, clearTimeout(d);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                d = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = d.bind(null, a.onerror), a.onload = d.bind(null, a.onload), l && document.head.appendChild(a)
+            a.onerror = p.bind(null, a.onerror), a.onload = p.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -150,76 +150,76 @@
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var a = 0, l = 1, s = !0;; l++, a++) {
-                var u, f, d = l < e.length ? (typeof e[l])[0] : "";
-                if (a >= r.length || "o" == (f = (typeof(u = r[a]))[0])) return !s || ("u" == d ? l > n && !o : "" == d != o);
+                var u, f, p = l < e.length ? (typeof e[l])[0] : "";
+                if (a >= r.length || "o" == (f = (typeof(u = r[a]))[0])) return !s || ("u" == p ? l > n && !o : "" == p != o);
                 if ("u" == f) {
-                    if (!s || "u" != d) return !1
+                    if (!s || "u" != p) return !1
                 } else if (s)
-                    if (d == f)
+                    if (p == f)
                         if (l <= n) {
                             if (u != e[l]) return !1
                         } else {
                             if (o ? u > e[l] : u < e[l]) return !1;
                             u != e[l] && (s = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != p && "n" != p) {
                     if (o || l <= n) return !1;
                     s = !1, l--
                 } else {
-                    if (l <= n || f < d != o) return !1;
+                    if (l <= n || f < p != o) return !1;
                     s = !1
-                } else "s" != d && "n" != d && (s = !1, l--)
+                } else "s" != p && "n" != p && (s = !1, l--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var d = [],
+            c = d.pop.bind(d);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
+            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
         }
         return !!c()
     }, a = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", u = (e, r, t, n) => {
         var o = l(e, t);
         return i(n, o) || "undefined" != typeof console && console.warn && console.warn(s(e, t, o, n)), f(e[t][o])
-    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+    }, f = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
         var i = m.I(r);
         return i && i.then ? i.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), p = {}, c = {
-        177: () => d("default", "@jupyterlab/codemirror", [1, 3, 4, 8]),
-        252: () => d("default", "@krassowski/jupyterlab-lsp", [1, 3, 7, 0])
+    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), d = {}, c = {
+        905: () => p("default", "@jupyterlab/codemirror", [1, 3, 5, 0]),
+        252: () => p("default", "@krassowski/jupyterlab-lsp", [1, 3, 7, 0])
     }, h = {
-        475: [177, 252]
+        475: [905, 252]
     }, m.f.consumes = (e, r) => {
         m.o(h, e) && h[e].forEach((e => {
-            if (m.o(p, e)) return r.push(p[e]);
+            if (m.o(d, e)) return r.push(d[e]);
             var t = r => {
-                    p[e] = 0, m.m[e] = t => {
+                    d[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], m.m[e] = t => {
+                    delete d[e], m.m[e] = t => {
                         throw delete m.c[e], r
                     }
                 };
             try {
                 var o = c[e]();
-                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
+                o.then ? r.push(d[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             239: 0
```

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/magics.py` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/magics.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,27 +497,36 @@
         return tree
 
     def _build_catalog_node(self, catalog: Row) -> Node:
         catalog_name = catalog[0]
         self.st_env.execute_sql(f"USE CATALOG `{catalog_name}`")
         databases = self.st_env.execute_sql("SHOW DATABASES").collect()
         tree_databases = [self._build_database_node(catalog_name, database) for database in databases]
-        return Node(catalog_name, tree_databases, opened=False, icon="database")
+        return Node(catalog_name, tree_databases, opened=False, icon="folder")
 
     def _build_database_node(self, catalog_name: str, database: Row) -> Node:
         database_name = database[0]
-        tables = self.st_env.execute_sql(f"SHOW TABLES FROM `{catalog_name}`.`{database_name}`").collect()
-        tree_tables = [self._build_table_node(catalog_name, database_name, table) for table in tables]
+        self.st_env.execute_sql(f"USE `{database_name}`")
+        tables = [table[0] for table in self.st_env.execute_sql("SHOW TABLES").collect()]
+        views = [view[0] for view in self.st_env.execute_sql("SHOW VIEWS").collect()]
+        tree_tables = [self._build_table_node(catalog_name, database_name, table,
+                                              "eye" if table in views else "table") for table in tables]
+        functions_node = self._build_functions_node()
+        tree_tables.append(functions_node)
         return Node(database_name, tree_tables, opened=False, icon="database")
 
-    def _build_table_node(self, catalog_name: str, database_name: str, table: Row) -> Node:
-        table_name = table[0]
+    def _build_functions_node(self) -> Node:
+        functions = self.st_env.execute_sql("SHOW USER FUNCTIONS").collect()
+        tree_functions = [Node(function[0], opened=False, icon="terminal") for function in functions]
+        return Node("Functions", tree_functions, opened=False, icon="list")
+
+    def _build_table_node(self, catalog_name: str, database_name: str, table_name: str, icon: str) -> Node:
         columns = self.st_env.execute_sql(f"DESCRIBE `{catalog_name}`.`{database_name}`.`{table_name}`").collect()
         tree_columns = [self._build_column_node(column) for column in columns]
-        return Node(table_name, tree_columns, opened=False, icon="table")
+        return Node(table_name, tree_columns, opened=False, icon=icon)
 
     def _build_column_node(self, column: Row) -> Node:
         column_name = column[0]
         column_type = column[1]
         column_null = column[2]
         column_key = column[3]
         column_extras = column[4]
```

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/reflection.py` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/reflection.py`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/sql_syntax_highlighting.py` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/sql_syntax_highlighting.py`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/sql_utils.py` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/sql_utils.py`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations/variable_substitution.py` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations/variable_substitution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import getpass
 import os
 import re
 import string
+import sys
 from typing import Any, Dict, List, Optional, cast
 
 
 def _match_forwards(full_string: str, match: Any, complimentary_regexp: str) -> str:
     start_pos = match.start()
     cut_string = full_string[start_pos:]
     full_match = re.match(complimentary_regexp, cut_string)
@@ -35,14 +36,22 @@
         _match_backwards,
     ),  # any non-whitespace character followed by two braces
     r"\{\s+\{": (r"[^\}]*\}", _match_forwards),  # catch some attempted nesting cases
     r"\}\s+\}": (r"[^\{]*\{", _match_backwards),  # catch some attempted nesting cases
 }
 
 
+# We need to skip curly brackets if there's no variable within, it can be regexp etc
+class SafeDict(Dict[Any, Any]):
+    def __missing__(self, key: str) -> str:
+        if any(c.isalpha() for c in key):
+            print(f"Variable '{key}' not found. The substitution will be skipped.", file=sys.stderr)
+        return '{' + key + '}'
+
+
 class CellContentFormatter(string.Formatter):
     def __init__(self, input_string: str, user_ns: Dict[Any, Any]):
         self.input_string = input_string
         self.user_ns = user_ns
         self.hidden_vars: Dict[str, str] = {}
 
     def substitute_user_variables(self) -> str:
@@ -92,15 +101,15 @@
                 var_val = getpass.getpass()
                 self.hidden_vars[var_name] = var_val
         return escaped_string.replace("${", "{")
 
     def _substitute_variables(self, escaped_string: str) -> str:
         try:
             merged_vars = {**self.user_ns, **self.hidden_vars}  # hidden_vars takes precedence
-            result = escaped_string.format(**merged_vars)
+            result = escaped_string.format_map(SafeDict(**merged_vars))
             self.hidden_vars.clear()  # ensure it gets wiped out after using
             return result
         except KeyError as error:
             raise NonExistentVariableException(
                 error.args[0],
                 message="The variable {} is not defined but is referenced in the cell.".format(
                     error
```

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations.egg-info/PKG-INFO` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming-jupyter-integrations
-Version: 0.9.0
+Version: 0.9.1
 Summary: JupyterNotebook Flink magics
 Home-page: https://github.com/getindata/streaming-jupyter-integrations
 Author: GetInData
 Author-email: office@getindata.com
 License: Apache Software License (Apache 2.0)
 Keywords: jupyter flink sql ipython
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `streaming_jupyter_integrations-0.9.0/streaming_jupyter_integrations.egg-info/SOURCES.txt` & `streaming_jupyter_integrations-0.9.1/streaming_jupyter_integrations.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,11 +24,11 @@
 streaming_jupyter_integrations/variable_substitution.py
 streaming_jupyter_integrations.egg-info/PKG-INFO
 streaming_jupyter_integrations.egg-info/SOURCES.txt
 streaming_jupyter_integrations.egg-info/dependency_links.txt
 streaming_jupyter_integrations.egg-info/requires.txt
 streaming_jupyter_integrations.egg-info/top_level.txt
 streaming_jupyter_integrations/labextension/package.json
-streaming_jupyter_integrations/labextension/static/475.73d1c5756e0a21e08d7c.js
-streaming_jupyter_integrations/labextension/static/remoteEntry.850f660cc32e4df795fe.js
+streaming_jupyter_integrations/labextension/static/475.2dfb31799d45d3c229a6.js
+streaming_jupyter_integrations/labextension/static/remoteEntry.1416e850b5547380e0e5.js
 streaming_jupyter_integrations/labextension/static/style.js
 streaming_jupyter_integrations/labextension/static/third-party-licenses.json
```

### Comparing `streaming_jupyter_integrations-0.9.0/tsconfig.json` & `streaming_jupyter_integrations-0.9.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `streaming_jupyter_integrations-0.9.0/yarn.lock` & `streaming_jupyter_integrations-0.9.1/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,17 @@
   version "7.19.4"
   resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.19.4.tgz#a42f814502ee467d55b38dd1c256f53a7b885c78"
   integrity sha512-EXpLCrk55f+cYqmHsSR+yD/0gAIMxxA9QK9lnQWzhMCvt+YmoBN7Zx94s++Kv0+unHk39vxNO8t+CMA2WSS3wA==
   dependencies:
     regenerator-runtime "^0.13.4"
 
 "@blueprintjs/colors@^4.0.0-alpha.3":
-  version "4.1.7"
-  resolved "https://registry.yarnpkg.com/@blueprintjs/colors/-/colors-4.1.7.tgz#3ccac41eabc3245da20669e6aafafe6c0271d264"
-  integrity sha512-4qmwwNabzJ6TbdWLjfVFqoCz6OPZpPDV6xvSmnEnS6tWSQ+bepi/ybzx3kKOGtNk1lu0tFDU6tnVti7uz23XaQ==
+  version "4.1.8"
+  resolved "https://registry.yarnpkg.com/@blueprintjs/colors/-/colors-4.1.8.tgz#ebab4e6fe9d4e2a3bb958ae0e2385b0675a0754a"
+  integrity sha512-J3N3PIBlmZS7+br+8KkR0yilGp74Fwp8SXfs0Bf4OGgLcqrBixqCqAs+YnpS2iOV0m2D22cZc8YsnPVdx0kH7w==
 
 "@blueprintjs/core@^3.36.0", "@blueprintjs/core@^3.54.0":
   version "3.54.0"
   resolved "https://registry.yarnpkg.com/@blueprintjs/core/-/core-3.54.0.tgz#7269f34eccdf0d2874377c5ad973ca2a31562221"
   integrity sha512-u2c1s6MNn0ocxhnC6CuiG5g3KV6b4cKUvSobznepA9SC3/AL1s3XOvT7DLWoHRv2B/vBOHFYEDzLw2/vlcGGZg==
   dependencies:
     "@blueprintjs/colors" "^4.0.0-alpha.3"
@@ -163,29 +163,29 @@
     "@jridgewell/sourcemap-codec" "1.4.14"
 
 "@juggle/resize-observer@^3.3.1":
   version "3.4.0"
   resolved "https://registry.yarnpkg.com/@juggle/resize-observer/-/resize-observer-3.4.0.tgz#08d6c5e20cf7e4cc02fd181c4b0c225cd31dbb60"
   integrity sha512-dfLbk+PwWvFzSxwk3n5ySL0hfBog779o8h68wK/7/APo/7cgyWp5jcXockbxdk5kFRkbeXWm4Fbi9FrdN381sA==
 
-"@jupyterlab/application@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/application/-/application-3.4.8.tgz#834ed31718f13c34e62ac37479e75a7ed105f477"
-  integrity sha512-h27vGjR3tqZ1636XSshzn6VCO4b11b353L13+C1PGU0IrlUg+80FH3uy+Frjlt3AJynHFWZqg1U68WwOMfDJRw==
+"@jupyterlab/application@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/application/-/application-3.5.0.tgz#44705368565c82c8effd07132994c6401d24e152"
+  integrity sha512-cXqxYW74HjMaMkEzjw53KSKQOQ/FSRY8fmBM+pVYUNFf281M8d5VAa96L7JNSMQaJ/i/M/fnpuH1QbldYjumkg==
   dependencies:
     "@fortawesome/fontawesome-free" "^5.12.0"
-    "@jupyterlab/apputils" "^3.4.8"
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/docregistry" "^3.4.8"
-    "@jupyterlab/rendermime" "^3.4.8"
-    "@jupyterlab/rendermime-interfaces" "^3.4.8"
-    "@jupyterlab/services" "^6.4.8"
-    "@jupyterlab/statedb" "^3.4.8"
-    "@jupyterlab/translation" "^3.4.8"
-    "@jupyterlab/ui-components" "^3.4.8"
+    "@jupyterlab/apputils" "^3.5.0"
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/docregistry" "^3.5.0"
+    "@jupyterlab/rendermime" "^3.5.0"
+    "@jupyterlab/rendermime-interfaces" "^3.5.0"
+    "@jupyterlab/services" "^6.5.0"
+    "@jupyterlab/statedb" "^3.5.0"
+    "@jupyterlab/translation" "^3.5.0"
+    "@jupyterlab/ui-components" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/application" "^1.27.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
@@ -215,26 +215,26 @@
     "@lumino/disposable" "^1.4.3"
     "@lumino/messaging" "^1.4.3"
     "@lumino/polling" "^1.3.3"
     "@lumino/properties" "^1.2.3"
     "@lumino/signaling" "^1.4.3"
     "@lumino/widgets" "^1.16.1"
 
-"@jupyterlab/apputils@^3.0.10", "@jupyterlab/apputils@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/apputils/-/apputils-3.4.8.tgz#09126a7628958ab2409379d3b691a00d144eee90"
-  integrity sha512-b7vvPQUdkXcrZnfPUXJVYw4vpKl5HmPqFtFTGmatY+F734FSLYkZeIrNxByinI2DJg35I1p1NfSQW/3DVVwpog==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/observables" "^4.4.8"
-    "@jupyterlab/services" "^6.4.8"
-    "@jupyterlab/settingregistry" "^3.4.8"
-    "@jupyterlab/statedb" "^3.4.8"
-    "@jupyterlab/translation" "^3.4.8"
-    "@jupyterlab/ui-components" "^3.4.8"
+"@jupyterlab/apputils@^3.0.10", "@jupyterlab/apputils@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/apputils/-/apputils-3.5.0.tgz#9ce715f6d56d3647798dc8d1108c638466459d3f"
+  integrity sha512-brL1CR0F2ocxt+YSWQGRh9OoJWxlqQb5BxQNJy+qJceCpwkMyZmZyf2gxHc9bu67HkL96Sa46wGIn6WKobARrA==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/observables" "^4.5.0"
+    "@jupyterlab/services" "^6.5.0"
+    "@jupyterlab/settingregistry" "^3.5.0"
+    "@jupyterlab/statedb" "^3.5.0"
+    "@jupyterlab/translation" "^3.5.0"
+    "@jupyterlab/ui-components" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
@@ -245,19 +245,19 @@
     "@types/react" "^17.0.0"
     react "^17.0.1"
     react-dom "^17.0.1"
     sanitize-html "~2.5.3"
     url "^0.11.0"
 
 "@jupyterlab/builder@^3.0.0":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.4.8.tgz#68877818d327d98087e2029a360314cffe0f0c9f"
-  integrity sha512-PjSpzcVFVyk6u2EENX9JrTdXelL+a90n668pkns8NoEKZVRE3KjZoBUO6WMLS/c4mI7h3TWQhByghKpmjxflAQ==
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.5.0.tgz#f7f92a39496e058ab01a8b1d8d169e4deca3e073"
+  integrity sha512-5nPZI29kAGhCGzDIU1NGmcwodVj/1hSqRuasozZEQYGxhEMUs3Nf3YRUbQrXrg2XnsWWhlZFOOUb1DZ8MkM+rw==
   dependencies:
-    "@jupyterlab/buildutils" "^3.4.8"
+    "@jupyterlab/buildutils" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/application" "^1.27.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
@@ -285,18 +285,18 @@
     to-string-loader "^1.1.6"
     url-loader "~4.1.0"
     webpack "^5.41.1"
     webpack-cli "^4.1.0"
     webpack-merge "^5.1.2"
     worker-loader "^3.0.2"
 
-"@jupyterlab/buildutils@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/buildutils/-/buildutils-3.4.8.tgz#97b9c123021ba0f35ba6b3c5f2227fb2465bcecf"
-  integrity sha512-1+OyQaheW+ZWiUS8SBeZ+TB9Iowx7gqxFGIL9jd3yYK2D5UkdZNPc4NEs9BmOTUnhUD3rySNTSCu3gZU0hRQYw==
+"@jupyterlab/buildutils@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/buildutils/-/buildutils-3.5.0.tgz#640990c4504880dadd6f57c609ee1facbb9cc114"
+  integrity sha512-NueiFvybuV2cfg4WRIyhrfuJ80cKwCgiwnMYX5pwCR7LkZ8OQAwDC/HQlkZSxPOCJGNK6ogUNxzARLQHLTJ/Ww==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
     "@yarnpkg/lockfile" "^1.1.0"
     child_process "~1.0.2"
     commander "~6.0.0"
     crypto "~1.0.1"
     dependency-graph "^0.9.0"
@@ -309,350 +309,350 @@
     prettier "~2.1.1"
     process "^0.11.10"
     semver "^7.3.2"
     sort-package-json "~1.44.0"
     typescript "~4.1.3"
     verdaccio "^5.13.3"
 
-"@jupyterlab/codeeditor@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codeeditor/-/codeeditor-3.4.8.tgz#2684c9a6f40192f5144937951e1852d1b652dd9e"
-  integrity sha512-1ymmnK6zE40ivJRpVRd3XI/p7WydqTyD/qbgcYK4JHRzDUvfIJz0OQkei4Rq1oOD9DsMdJOIuyyEXgA8FPE4/g==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/nbformat" "^3.4.8"
-    "@jupyterlab/observables" "^4.4.8"
-    "@jupyterlab/shared-models" "^3.4.8"
-    "@jupyterlab/translation" "^3.4.8"
-    "@jupyterlab/ui-components" "^3.4.8"
+"@jupyterlab/codeeditor@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codeeditor/-/codeeditor-3.5.0.tgz#b5345f028196c68077424b4a9f33ca315ec49828"
+  integrity sha512-imdYuovxyIIQqZdoRnZAr0VQHqiIVPPFwk8hAgDYtfl8VxFOPMTh203Z6y+CLv5V62J03OU7HZutP/f5u1nZ1w==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/nbformat" "^3.5.0"
+    "@jupyterlab/observables" "^4.5.0"
+    "@jupyterlab/shared-models" "^3.5.0"
+    "@jupyterlab/translation" "^3.5.0"
+    "@jupyterlab/ui-components" "^3.5.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.33.0"
 
 "@jupyterlab/codemirror-extension@^3.4.4":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror-extension/-/codemirror-extension-3.4.8.tgz#6e2c1c1d92a742143e139ce3839f6f23427f2d69"
-  integrity sha512-qyV+aDFsIADBwjuQ5LV+t0dsdfuVywlGbxGLrPnFsDp48kluP3pkm0H56dNNZjUu9m9uzY9IJN/uiR+2WbS7hg==
-  dependencies:
-    "@jupyterlab/application" "^3.4.8"
-    "@jupyterlab/codeeditor" "^3.4.8"
-    "@jupyterlab/codemirror" "^3.4.8"
-    "@jupyterlab/docregistry" "^3.4.8"
-    "@jupyterlab/fileeditor" "^3.4.8"
-    "@jupyterlab/mainmenu" "^3.4.8"
-    "@jupyterlab/settingregistry" "^3.4.8"
-    "@jupyterlab/statusbar" "^3.4.8"
-    "@jupyterlab/translation" "^3.4.8"
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror-extension/-/codemirror-extension-3.5.0.tgz#c60144ccbe7de4bf1fb2d9c3944ab92f2c2cc32f"
+  integrity sha512-YseP48RCYL0pTql7TU4ml/TeA2zj/ZxsNK7x60UvrY9QBHEx7MvKq61d8BSHsq07Cz3RCAUPO+YzsGax5sqUtg==
+  dependencies:
+    "@jupyterlab/application" "^3.5.0"
+    "@jupyterlab/codeeditor" "^3.5.0"
+    "@jupyterlab/codemirror" "^3.5.0"
+    "@jupyterlab/docregistry" "^3.5.0"
+    "@jupyterlab/fileeditor" "^3.5.0"
+    "@jupyterlab/mainmenu" "^3.5.0"
+    "@jupyterlab/settingregistry" "^3.5.0"
+    "@jupyterlab/statusbar" "^3.5.0"
+    "@jupyterlab/translation" "^3.5.0"
     codemirror "~5.61.0"
 
-"@jupyterlab/codemirror@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror/-/codemirror-3.4.8.tgz#fe72b58d5d01da83da9725f59393326a6bf8ca90"
-  integrity sha512-HojL7+vaUTBPIgg0gzCJKBbsN8TdVR+DxXfeGII1RoQf5uUCQdBz9/Ksyt96uHCS+EmYRWkLik2dU94LIEr4dw==
-  dependencies:
-    "@jupyterlab/apputils" "^3.4.8"
-    "@jupyterlab/codeeditor" "^3.4.8"
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/nbformat" "^3.4.8"
-    "@jupyterlab/observables" "^4.4.8"
-    "@jupyterlab/shared-models" "^3.4.8"
-    "@jupyterlab/statusbar" "^3.4.8"
-    "@jupyterlab/translation" "^3.4.8"
+"@jupyterlab/codemirror@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror/-/codemirror-3.5.0.tgz#b16190e99584acfb0b18c44dd1c005366a829062"
+  integrity sha512-i6rGYLnWsBuL8zkCpPTCMeZc2lHI5pIgtEpO/CEfeigYhZI9NkaLSiF64Jwt8bgurS10O02bxl+3hIgU3mSSQA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.5.0"
+    "@jupyterlab/codeeditor" "^3.5.0"
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/nbformat" "^3.5.0"
+    "@jupyterlab/observables" "^4.5.0"
+    "@jupyterlab/shared-models" "^3.5.0"
+    "@jupyterlab/statusbar" "^3.5.0"
+    "@jupyterlab/translation" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.33.0"
     codemirror "~5.61.0"
     react "^17.0.1"
     y-codemirror "^3.0.1"
 
-"@jupyterlab/coreutils@^5.0.7", "@jupyterlab/coreutils@^5.4.8":
-  version "5.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.4.8.tgz#e3a81a8edb51c9a8d40f9baf4149f86c5e5109d0"
-  integrity sha512-UICv9nBCL+thSSOFlLWGjPm+UTT1ioPq+pOMjgn0E/DPliUMAMKtrAU5viAbRhITGAU55uL2KH9ijMUIc6o3xA==
+"@jupyterlab/coreutils@^5.0.7", "@jupyterlab/coreutils@^5.5.0":
+  version "5.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.5.0.tgz#0cbceb74e75a96cc69c8dd14b61f37d8ea940d75"
+  integrity sha512-mVBuVDUA87hvtS5DfbjfLIE1EFdhAGEU8f19G33QfhD/w2vYDi7vE4ro4arNT47r17MzXW4XfaE4LwatR6uvPw==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     minimist "~1.2.0"
     moment "^2.24.0"
     path-browserify "^1.0.0"
     url-parse "~1.5.1"
 
 "@jupyterlab/docmanager@^3.0.0":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docmanager/-/docmanager-3.4.8.tgz#3d4a4d84c8b2d950aa7373124b8268b19b9620fe"
-  integrity sha512-vYEoO57nP1+HYhToYM+8Rxa0jYob9+ALXDqaX/hSyG1EUroVeKcfc8sfErWYV1qQLN0T3yX4cpVYtx99Ij36eQ==
-  dependencies:
-    "@jupyterlab/apputils" "^3.4.8"
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/docprovider" "^3.4.8"
-    "@jupyterlab/docregistry" "^3.4.8"
-    "@jupyterlab/services" "^6.4.8"
-    "@jupyterlab/statusbar" "^3.4.8"
-    "@jupyterlab/translation" "^3.4.8"
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docmanager/-/docmanager-3.5.0.tgz#80dd3ffe688436b5d98f73b7de1de588f7929fce"
+  integrity sha512-IkPUXpI6zcGufGwetge6F/b5pyF9CLYb/xdK+fuN61jub8aEWFE4vebXNhb1rhmyjynjDwSmLcUTX3slFTItRA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.5.0"
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/docprovider" "^3.5.0"
+    "@jupyterlab/docregistry" "^3.5.0"
+    "@jupyterlab/services" "^6.5.0"
+    "@jupyterlab/statusbar" "^3.5.0"
+    "@jupyterlab/translation" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.33.0"
     react "^17.0.1"
 
-"@jupyterlab/docprovider@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docprovider/-/docprovider-3.4.8.tgz#d75e8ccfc9d3f08cf13c6b9b97cd987bdbdcd6d2"
-  integrity sha512-srOLhPzP+pfOjpQNtXmKuSyBsQzTxf087+MpUdTMPt177PCGG7eyMcCNcDTkBXo6QzuwQuJIj+uESQjVYmQ7Hw==
+"@jupyterlab/docprovider@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docprovider/-/docprovider-3.5.0.tgz#8593ada08c0e7ec014084e16e918d26aac14c441"
+  integrity sha512-F5VtIIDUpWEFKc0S/xDs8GIjEZC/xn6SVrdNY0+ixDPyC5VNJo+IU5JmqrcU25DlJ+jMbnKlPdRLYsRtJTDKrw==
   dependencies:
-    "@jupyterlab/shared-models" "^3.4.8"
+    "@jupyterlab/shared-models" "^3.5.0"
     "@lumino/coreutils" "^1.11.0"
     lib0 "^0.2.42"
     y-websocket "^1.3.15"
     yjs "^13.5.17"
 
-"@jupyterlab/docregistry@^3.0.13", "@jupyterlab/docregistry@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docregistry/-/docregistry-3.4.8.tgz#d9e4c3d7a69b718ce3e6a57f1c4a76bca7cb95b7"
-  integrity sha512-4DRy4zMrUIhdlEsStbKSOrUUe27EtJBMhwFqTIiKQdaQp4QHgMaHYTLqX/DomGJd4FPmXtcgNfkTr+nM2Tf3yw==
-  dependencies:
-    "@jupyterlab/apputils" "^3.4.8"
-    "@jupyterlab/codeeditor" "^3.4.8"
-    "@jupyterlab/codemirror" "^3.4.8"
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/docprovider" "^3.4.8"
-    "@jupyterlab/observables" "^4.4.8"
-    "@jupyterlab/rendermime" "^3.4.8"
-    "@jupyterlab/rendermime-interfaces" "^3.4.8"
-    "@jupyterlab/services" "^6.4.8"
-    "@jupyterlab/shared-models" "^3.4.8"
-    "@jupyterlab/translation" "^3.4.8"
-    "@jupyterlab/ui-components" "^3.4.8"
+"@jupyterlab/docregistry@^3.0.13", "@jupyterlab/docregistry@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docregistry/-/docregistry-3.5.0.tgz#aa3ebc2cd676f7ff564dd055fdd629f0dd16b5b1"
+  integrity sha512-OdP+q4rvZARqJvZWCyae23K8IHN+TvSP0xPyTVHd1aXFXi6cWlNUOUGRHd9TlEUNqyJxKjkZNuhozMu8ANEBAQ==
+  dependencies:
+    "@jupyterlab/apputils" "^3.5.0"
+    "@jupyterlab/codeeditor" "^3.5.0"
+    "@jupyterlab/codemirror" "^3.5.0"
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/docprovider" "^3.5.0"
+    "@jupyterlab/observables" "^4.5.0"
+    "@jupyterlab/rendermime" "^3.5.0"
+    "@jupyterlab/rendermime-interfaces" "^3.5.0"
+    "@jupyterlab/services" "^6.5.0"
+    "@jupyterlab/shared-models" "^3.5.0"
+    "@jupyterlab/translation" "^3.5.0"
+    "@jupyterlab/ui-components" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.33.0"
     yjs "^13.5.17"
 
-"@jupyterlab/fileeditor@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/fileeditor/-/fileeditor-3.4.8.tgz#33765cfe4c134f725e79996fe1291fb622e0b0ec"
-  integrity sha512-5YA0dZbeDNCJhi9zxP3MKxpFZKBUd3s4v6VaoY8w/D7Ldeg8gB0q4bjojLEAQ6VnQ1ZaI0J2JzGtWrRcDrSIcA==
-  dependencies:
-    "@jupyterlab/apputils" "^3.4.8"
-    "@jupyterlab/codeeditor" "^3.4.8"
-    "@jupyterlab/docregistry" "^3.4.8"
-    "@jupyterlab/statusbar" "^3.4.8"
-    "@jupyterlab/translation" "^3.4.8"
-    "@jupyterlab/ui-components" "^3.4.8"
+"@jupyterlab/fileeditor@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/fileeditor/-/fileeditor-3.5.0.tgz#23f48f4dbe8f58e49cb0812fd92d4cfca37773e1"
+  integrity sha512-xahPO68ylMf5hkUMZv+M4f2MIA1vJBr0Eg8IMykCaD8o/ssc2oEaMcYkJIoBq9E5/wr5iS4TNcT9CmMld2sK0Q==
+  dependencies:
+    "@jupyterlab/apputils" "^3.5.0"
+    "@jupyterlab/codeeditor" "^3.5.0"
+    "@jupyterlab/docregistry" "^3.5.0"
+    "@jupyterlab/statusbar" "^3.5.0"
+    "@jupyterlab/translation" "^3.5.0"
+    "@jupyterlab/ui-components" "^3.5.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/widgets" "^1.33.0"
     react "^17.0.1"
 
 "@jupyterlab/logconsole@^3.0.0":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/logconsole/-/logconsole-3.4.8.tgz#834030ad79242b50b538cbebb425f32180ac8a99"
-  integrity sha512-zLUzNElqkXqKs8Fq7NGoyl1IwEP5QkiNH+q9AmXZFKp64Xakvd0QSnvNNT2iMvx/5LXUGgzbu4Jy3eDwJwMQlA==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/nbformat" "^3.4.8"
-    "@jupyterlab/outputarea" "^3.4.8"
-    "@jupyterlab/rendermime" "^3.4.8"
-    "@jupyterlab/services" "^6.4.8"
-    "@jupyterlab/translation" "^3.4.8"
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/logconsole/-/logconsole-3.5.0.tgz#bb2a5af02ed5f05de6674a65a36776bfd7d06c6f"
+  integrity sha512-njQEGLzK+JOOYoyCPYFWtnj13A9eYPhmjOuNrfzzFnM2mVYSN6BspqpY762l0W2afkc5de+cCZrrBdYUDHdFKw==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/nbformat" "^3.5.0"
+    "@jupyterlab/outputarea" "^3.5.0"
+    "@jupyterlab/rendermime" "^3.5.0"
+    "@jupyterlab/services" "^6.5.0"
+    "@jupyterlab/translation" "^3.5.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.33.0"
 
-"@jupyterlab/mainmenu@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.4.8.tgz#dfa3bcffacaaf54c8b982836a9b5647eeb33fb06"
-  integrity sha512-rz6nJnwXI2SktjuaJuoXfiBURSG77a/nrmpCDZ+bWunV7vyjb6jNsA7Xuq32aWc/tlWcGBYamtWbUlVHPPm4jQ==
-  dependencies:
-    "@jupyterlab/apputils" "^3.4.8"
-    "@jupyterlab/services" "^6.4.8"
-    "@jupyterlab/translation" "^3.4.8"
-    "@jupyterlab/ui-components" "^3.4.8"
+"@jupyterlab/mainmenu@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.5.0.tgz#a49cd2efec1eb42ab45033bebe0c3c88d6f4ac3e"
+  integrity sha512-Sl94dcwGe2Dqt+9mIIcwymtBtymmzMOPaqrEnJSgVET4a42SFgmeS1JBXGAFj4djbCB8VDzGHe+IbBlKLX8IaQ==
+  dependencies:
+    "@jupyterlab/apputils" "^3.5.0"
+    "@jupyterlab/services" "^6.5.0"
+    "@jupyterlab/translation" "^3.5.0"
+    "@jupyterlab/ui-components" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/widgets" "^1.33.0"
 
-"@jupyterlab/nbformat@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.4.8.tgz#8552c9d32e8f04bd3e9be468be57662f0c5307c2"
-  integrity sha512-RcyITAagwXMIWqehpctb43mVB1H3LrTfikGvykLICmA5AfT+byhooCDN4d+ipg4rkeioUmEgX+2uTfForCsJWQ==
+"@jupyterlab/nbformat@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.5.0.tgz#ea3d926b90db9ff2da988db1ea3c8ac1dc3ba9fa"
+  integrity sha512-tQ0MCJ2NSlGTYM7auiL2vdqirIv39Pd2/gfFd4XdHClJgvT65b7XkNDOwBv6mqIuhNdHo3Mc3RXiODTo1tle7Q==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
 
-"@jupyterlab/observables@^4.4.8":
-  version "4.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.4.8.tgz#a73833e4f33b3d7e9c2a59306e8f526e13c043d9"
-  integrity sha512-TT7YQNxvLnfuzbHQjoovfVN02dXDG/zxfWiA1RkycAJnQ/aTgRtEMlLMs7dUqNCh6ej6zNQOUEduJInro/OL4A==
+"@jupyterlab/observables@^4.5.0":
+  version "4.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.5.0.tgz#3cba31bf2358c11f3c7ba39b7aa840e727733405"
+  integrity sha512-YiUljeHNz80YpIPDi0zoUC26AwAhyDu1UXm2kH5J/lPViycz8X22RWXkIBc40kvWoasUTSomZiEv/W2hFUs0Vw==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/outputarea@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/outputarea/-/outputarea-3.4.8.tgz#32b54d0fb1ed5422436b74e869a90c1da499294d"
-  integrity sha512-kKPwUbqNDMJ9xnVRrBjNkLY75fH+U/K7phAmteEVWE04qYNAizwopcMA+TdW9IfHMAhcVoI1nTrShwoWgn7YrQ==
-  dependencies:
-    "@jupyterlab/apputils" "^3.4.8"
-    "@jupyterlab/nbformat" "^3.4.8"
-    "@jupyterlab/observables" "^4.4.8"
-    "@jupyterlab/rendermime" "^3.4.8"
-    "@jupyterlab/rendermime-interfaces" "^3.4.8"
-    "@jupyterlab/services" "^6.4.8"
+"@jupyterlab/outputarea@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/outputarea/-/outputarea-3.5.0.tgz#9ecab47c4ce512a0c6d3ac3235ae924a8edcad09"
+  integrity sha512-GF9jXeQDUQw93w4+Oh7J8AjFzBjcXL9f0CmGCao0H4rjni1EFByU5eLPe0FM7YRubU9ike7JMu3+9dJDlnpdAA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.5.0"
+    "@jupyterlab/nbformat" "^3.5.0"
+    "@jupyterlab/observables" "^4.5.0"
+    "@jupyterlab/rendermime" "^3.5.0"
+    "@jupyterlab/rendermime-interfaces" "^3.5.0"
+    "@jupyterlab/services" "^6.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.33.0"
     resize-observer-polyfill "^1.5.1"
 
-"@jupyterlab/rendermime-interfaces@^3.0.10", "@jupyterlab/rendermime-interfaces@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.4.8.tgz#2ed70bf936a03523fbd0a8838cded9c23af6211f"
-  integrity sha512-zaJbCv9fhgwAlNOcmWnz2rSmoRPR3QLUvhEQ7e08k0jrG6O3Zf19SObEOcp1TM0qwPNSEFT71AbAa81ari13Jg==
+"@jupyterlab/rendermime-interfaces@^3.0.10", "@jupyterlab/rendermime-interfaces@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.5.0.tgz#e833b1304ff1e86934fcb039dec7b5ffbf374ae9"
+  integrity sha512-SWpNX8dwRuAH0GMeuamN1O096Ypn2XcosNbo60P8860qi2KzTXgxADt5xcOf6FK+tXVQ+qi3hJi+055+1xjq+g==
   dependencies:
-    "@jupyterlab/translation" "^3.4.8"
+    "@jupyterlab/translation" "^3.5.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/widgets" "^1.33.0"
 
-"@jupyterlab/rendermime@^3.0.12", "@jupyterlab/rendermime@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.4.8.tgz#9775185c6d71f4159feebeec3d936c00c73d298b"
-  integrity sha512-9GrfLst9BRJpVAng2mcVCIt2zCIw0+ho8CEMnlq/gwUMUxW8fpstaUnxkLoW7yIvtSnFAYbUZ3GBKenc084nOQ==
-  dependencies:
-    "@jupyterlab/apputils" "^3.4.8"
-    "@jupyterlab/codemirror" "^3.4.8"
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/nbformat" "^3.4.8"
-    "@jupyterlab/observables" "^4.4.8"
-    "@jupyterlab/rendermime-interfaces" "^3.4.8"
-    "@jupyterlab/services" "^6.4.8"
-    "@jupyterlab/translation" "^3.4.8"
+"@jupyterlab/rendermime@^3.0.12", "@jupyterlab/rendermime@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.5.0.tgz#279a2672690b63ac23990b366f2dc5cdc786dacc"
+  integrity sha512-vA5bQA/v7/P/6a3WXdrSoTeGgIJy1iLvpVpJ3DfR9NIpPrXzazDtRplipwcHsNjtUn4P2oS8C46s/eTOEPsQOw==
+  dependencies:
+    "@jupyterlab/apputils" "^3.5.0"
+    "@jupyterlab/codemirror" "^3.5.0"
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/nbformat" "^3.5.0"
+    "@jupyterlab/observables" "^4.5.0"
+    "@jupyterlab/rendermime-interfaces" "^3.5.0"
+    "@jupyterlab/services" "^6.5.0"
+    "@jupyterlab/translation" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.33.0"
     lodash.escape "^4.0.1"
     marked "^4.0.17"
 
-"@jupyterlab/services@^6.0.10", "@jupyterlab/services@^6.4.8":
-  version "6.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.4.8.tgz#2da20fd5a5c94ab8f8200da633a252792927318a"
-  integrity sha512-/acj4d1A1V9KDN+k4CUokOA8e/IxaoJW2B+FJxVnTZvVOBh7093EIG+HYL1SQuQ8CUc2T4DNiq9mG3skiSe2fQ==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/nbformat" "^3.4.8"
-    "@jupyterlab/observables" "^4.4.8"
-    "@jupyterlab/settingregistry" "^3.4.8"
-    "@jupyterlab/statedb" "^3.4.8"
+"@jupyterlab/services@^6.0.10", "@jupyterlab/services@^6.5.0":
+  version "6.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.5.0.tgz#cf89407d8f39ed708394e8ba14b5cba5b65b9cba"
+  integrity sha512-g5fa7oFu1I6i0agOmx6ud/1fjYAsr3zHzoymE4oAGN3nIbt8HTcmzLbiwmaWssGCVUF4h06GOYWcAe/x/ND8JA==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/nbformat" "^3.5.0"
+    "@jupyterlab/observables" "^4.5.0"
+    "@jupyterlab/settingregistry" "^3.5.0"
+    "@jupyterlab/statedb" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     node-fetch "^2.6.0"
     ws "^7.4.6"
 
-"@jupyterlab/settingregistry@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.4.8.tgz#10f52898b8553639ed4d9d786294617ac599c4a9"
-  integrity sha512-w9MNFivKXUOLrEvWckpcYm3XAZr0sbcKQ33SkftaLSQODsFlUwkcsjCPJJATVyxiWXAsCAgUlOKdNcqWxYXvOA==
+"@jupyterlab/settingregistry@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.5.0.tgz#2a6a0c2771c61643ab4aff9355ac863b4c8fc0ab"
+  integrity sha512-y9H9U4iMVfe2btImp5DR9mGAs36Sow0hI6ajK61bhHVJ4CumYdFBd8drrQGuYcyk/Y4ypU5HO9EaLBQU3CLCug==
   dependencies:
-    "@jupyterlab/statedb" "^3.4.8"
+    "@jupyterlab/statedb" "^3.5.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     ajv "^6.12.3"
     json5 "^2.1.1"
 
-"@jupyterlab/shared-models@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/shared-models/-/shared-models-3.4.8.tgz#88156a1c584e50f03cb378ea56f42e8800ba8c3d"
-  integrity sha512-sUBGyYTAYDOG6S5537ZLTTlqR/ut6XU1sLz/khjQOjROhyAC5kH7Vs7oUoGoGfSCLIwCAlCX2NZHXcvhElNbIg==
+"@jupyterlab/shared-models@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/shared-models/-/shared-models-3.5.0.tgz#d34b5ac6d0121ea8daf3862bb92926959aade209"
+  integrity sha512-QZL9BPCC+iV12AsUbUAwQvZeeo3fKh1X8h9odtlc+Oc+dyZAqREYXuZGjVlaG9qwbF62xDr7acfO4HqCK6Kjyw==
   dependencies:
-    "@jupyterlab/nbformat" "^3.4.8"
+    "@jupyterlab/nbformat" "^3.5.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     y-protocols "^1.0.5"
     yjs "^13.5.17"
 
-"@jupyterlab/statedb@^3.0.7", "@jupyterlab/statedb@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.4.8.tgz#78654b5563f97e8f63683c54403bdc391f4c8df3"
-  integrity sha512-PMlo+x4R8uXPH1BgCJUVVIj/H8SY9scGJU0pqHhYa6mm3R2EHNAwr8JxyqGjAqT3C0VCCCIDzHtQ3f9inW+OXg==
+"@jupyterlab/statedb@^3.0.7", "@jupyterlab/statedb@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.5.0.tgz#6118a7cf339a3d5f033b7b61c3480bfd9bb97a48"
+  integrity sha512-S4/BjcfSN8tGMyL4jjrD4TMoLTABI3zkLjaqSNRfT6iyKnqN8VKcMHBZXOq90uWGkw+caQZ5GiL+L7uEtahE4w==
   dependencies:
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/statusbar@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statusbar/-/statusbar-3.4.8.tgz#ac99f5304cf54ec06b7fb02badde8f22201f713e"
-  integrity sha512-WdeiqMmUEfxfOSMyOTRHQwPKSpcE9ucmq8SL0KN5pY5jcEfw3JTJGSb1tKV3WpI6lqErCQITcu29i1jiP/p+Vg==
-  dependencies:
-    "@jupyterlab/apputils" "^3.4.8"
-    "@jupyterlab/codeeditor" "^3.4.8"
-    "@jupyterlab/services" "^6.4.8"
-    "@jupyterlab/translation" "^3.4.8"
-    "@jupyterlab/ui-components" "^3.4.8"
+"@jupyterlab/statusbar@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statusbar/-/statusbar-3.5.0.tgz#62155a3938f6aff6081820c54007d7cbae93bf68"
+  integrity sha512-kXgMN7x5V3bTWP45mahOt2SaNOMXgeohlMsIou9f+OHZeR++6dmMMKyHPnE7QXES4At26FQu3swRI+8+A2klgA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.5.0"
+    "@jupyterlab/codeeditor" "^3.5.0"
+    "@jupyterlab/services" "^6.5.0"
+    "@jupyterlab/translation" "^3.5.0"
+    "@jupyterlab/ui-components" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.33.0"
     csstype "~3.0.3"
     react "^17.0.1"
     typestyle "^2.0.4"
 
-"@jupyterlab/translation@^3.0.10", "@jupyterlab/translation@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/translation/-/translation-3.4.8.tgz#9958bbbcabdcf913e96fcb267b223dccfa4d1151"
-  integrity sha512-5hIdMcA33qQpa2jR2Ho+bslfrf+feMyZbu37eCV58kHZjG3BsW47PWe5M0PCCe8WEIkTDu9z7BAmIUtbfwaZgA==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/services" "^6.4.8"
-    "@jupyterlab/statedb" "^3.4.8"
+"@jupyterlab/translation@^3.0.10", "@jupyterlab/translation@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/translation/-/translation-3.5.0.tgz#4f8cfd7382009365297df112abb51b7a8d531081"
+  integrity sha512-68Cyc9gVKef/Gr9tx9YisiPEIzXUk+mnM7u9huthq5A0aHh1W0E51CM/m0BwJDBurbY+W7erphy0nSWSEk7vCg==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/services" "^6.5.0"
+    "@jupyterlab/statedb" "^3.5.0"
     "@lumino/coreutils" "^1.11.0"
 
-"@jupyterlab/ui-components@^3.0.8", "@jupyterlab/ui-components@^3.4.8":
-  version "3.4.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/ui-components/-/ui-components-3.4.8.tgz#1aec1b7c6a07abe8d84424d8b3085d8f5627b360"
-  integrity sha512-mkbJnllKCHaKEtUAtCwQAHrJjoD13njlcaDM2Ml9x8vF7PQB8bwRfp/ml4d6n1jOEJjd+a8HRrpzD2X1mTneZQ==
+"@jupyterlab/ui-components@^3.0.8", "@jupyterlab/ui-components@^3.5.0":
+  version "3.5.0"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/ui-components/-/ui-components-3.5.0.tgz#329d0d0b3db666c041fa1a647af68400909d09e9"
+  integrity sha512-1AIKMUhyLgPYh3R3qvEPRhLKkiVwBtPg571If9UxTvDEJqVwtNTayn47sRsWlOKlueLVwebgEHVSkk2ahxgF6Q==
   dependencies:
     "@blueprintjs/core" "^3.36.0"
     "@blueprintjs/select" "^3.15.0"
-    "@jupyterlab/coreutils" "^5.4.8"
-    "@jupyterlab/translation" "^3.4.8"
+    "@jupyterlab/coreutils" "^5.5.0"
+    "@jupyterlab/translation" "^3.5.0"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
     "@lumino/widgets" "^1.33.0"
@@ -901,17 +901,17 @@
   resolved "https://registry.yarnpkg.com/@types/eslint-scope/-/eslint-scope-3.7.4.tgz#37fc1223f0786c39627068a12e94d6e6fc61de16"
   integrity sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==
   dependencies:
     "@types/eslint" "*"
     "@types/estree" "*"
 
 "@types/eslint@*":
-  version "8.4.6"
-  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.4.6.tgz#7976f054c1bccfcf514bff0564c0c41df5c08207"
-  integrity sha512-/fqTbjxyFUaYNO7VcW5g+4npmqVACz1bB7RTHYuLj+PRjw9hrCwrUXVQFpChUS0JsyEFvMZ7U/PfmvWgxJhI9g==
+  version "8.4.7"
+  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.4.7.tgz#0f05a2677d1a394ff70c21a964a32d3efa05f966"
+  integrity sha512-ehM7cCt2RSFs42mb+lcmhFT9ouIlV92PuaeRGn8N8c98oMjG4Z5pJHA9b1QiCcuqnbPSHcyfiD3mlhqMaHsQIw==
   dependencies:
     "@types/estree" "*"
     "@types/json-schema" "*"
 
 "@types/estree@*":
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/@types/estree/-/estree-1.0.0.tgz#5fb2e536c1ae9bf35366eed879e827fa59ca41c2"
@@ -937,17 +937,17 @@
 
 "@types/minimatch@*":
   version "5.1.2"
   resolved "https://registry.yarnpkg.com/@types/minimatch/-/minimatch-5.1.2.tgz#07508b45797cb81ec3f273011b054cd0755eddca"
   integrity sha512-K0VQKziLUWkVKiRVrx4a40iPaxTUefQmjtkQofBkYRcoaaL/8rhwDWww9qWbrgicNOgnpIsMxyNIUM4+n6dUIA==
 
 "@types/node@*":
-  version "18.11.2"
-  resolved "https://registry.yarnpkg.com/@types/node/-/node-18.11.2.tgz#c59b7641832531264fda3f1ba610362dc9a7dfc8"
-  integrity sha512-BWN3M23gLO2jVG8g/XHIRFWiiV4/GckeFIqbU/C4V3xpoBBWSMk4OZomouN0wCkfQFPqgZikyLr7DOYDysIkkw==
+  version "18.11.5"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-18.11.5.tgz#1bc94cf2f9ab5fe33353bc7c79c797dcc5325bef"
+  integrity sha512-3JRwhbjI+cHLAkUorhf8RnqUbFXajvzX4q6fMn5JwkgtuwfYtRQYI3u4V92vI6NJuTsbBQWWh3RZjFsuevyMGQ==
 
 "@types/prop-types@*":
   version "15.7.5"
   resolved "https://registry.yarnpkg.com/@types/prop-types/-/prop-types-15.7.5.tgz#5f19d2b85a98e9558036f6a3cacc8819420f05cf"
   integrity sha512-JCB8C6SnDoQf0cNycqd/35A7MjcnK+ZTqE7judS6o7utxUCg6imJg3QK2qzHKszlTjcj2cn+NwMB2i96ubpj7w==
 
 "@types/react@^17.0.0":
@@ -987,93 +987,93 @@
   integrity sha512-bvzMnzqoK16PQIC8AYHNdW45eREJQMd6WG/msQWX5V2+vZmODCOPb4TJcbgRljTZZTwTM4wUMcsI8FftNA7new==
   dependencies:
     "@types/node" "*"
     "@types/source-list-map" "*"
     source-map "^0.6.1"
 
 "@typescript-eslint/eslint-plugin@^5.32.0":
-  version "5.40.1"
-  resolved "https://registry.yarnpkg.com/@typescript-eslint/eslint-plugin/-/eslint-plugin-5.40.1.tgz#3203a6ff396b1194083faaa6e5110c401201d7d5"
-  integrity sha512-FsWboKkWdytGiXT5O1/R9j37YgcjO8MKHSUmWnIEjVaz0krHkplPnYi7mwdb+5+cs0toFNQb0HIrN7zONdIEWg==
-  dependencies:
-    "@typescript-eslint/scope-manager" "5.40.1"
-    "@typescript-eslint/type-utils" "5.40.1"
-    "@typescript-eslint/utils" "5.40.1"
+  version "5.41.0"
+  resolved "https://registry.yarnpkg.com/@typescript-eslint/eslint-plugin/-/eslint-plugin-5.41.0.tgz#f8eeb1c6bb2549f795f3ba71aec3b38d1ab6b1e1"
+  integrity sha512-DXUS22Y57/LAFSg3x7Vi6RNAuLpTXwxB9S2nIA7msBb/Zt8p7XqMwdpdc1IU7CkOQUPgAqR5fWvxuKCbneKGmA==
+  dependencies:
+    "@typescript-eslint/scope-manager" "5.41.0"
+    "@typescript-eslint/type-utils" "5.41.0"
+    "@typescript-eslint/utils" "5.41.0"
     debug "^4.3.4"
     ignore "^5.2.0"
     regexpp "^3.2.0"
     semver "^7.3.7"
     tsutils "^3.21.0"
 
 "@typescript-eslint/parser@^5.32.0":
-  version "5.40.1"
-  resolved "https://registry.yarnpkg.com/@typescript-eslint/parser/-/parser-5.40.1.tgz#e7f8295dd8154d0d37d661ddd8e2f0ecfdee28dd"
-  integrity sha512-IK6x55va5w4YvXd4b3VrXQPldV9vQTxi5ov+g4pMANsXPTXOcfjx08CRR1Dfrcc51syPtXHF5bgLlMHYFrvQtg==
-  dependencies:
-    "@typescript-eslint/scope-manager" "5.40.1"
-    "@typescript-eslint/types" "5.40.1"
-    "@typescript-eslint/typescript-estree" "5.40.1"
+  version "5.41.0"
+  resolved "https://registry.yarnpkg.com/@typescript-eslint/parser/-/parser-5.41.0.tgz#0414a6405007e463dc527b459af1f19430382d67"
+  integrity sha512-HQVfix4+RL5YRWZboMD1pUfFN8MpRH4laziWkkAzyO1fvNOY/uinZcvo3QiFJVS/siNHupV8E5+xSwQZrl6PZA==
+  dependencies:
+    "@typescript-eslint/scope-manager" "5.41.0"
+    "@typescript-eslint/types" "5.41.0"
+    "@typescript-eslint/typescript-estree" "5.41.0"
     debug "^4.3.4"
 
-"@typescript-eslint/scope-manager@5.40.1":
-  version "5.40.1"
-  resolved "https://registry.yarnpkg.com/@typescript-eslint/scope-manager/-/scope-manager-5.40.1.tgz#a7a5197dfd234622a2421ea590ee0ccc02e18dfe"
-  integrity sha512-jkn4xsJiUQucI16OLCXrLRXDZ3afKhOIqXs4R3O+M00hdQLKR58WuyXPZZjhKLFCEP2g+TXdBRtLQ33UfAdRUg==
-  dependencies:
-    "@typescript-eslint/types" "5.40.1"
-    "@typescript-eslint/visitor-keys" "5.40.1"
-
-"@typescript-eslint/type-utils@5.40.1":
-  version "5.40.1"
-  resolved "https://registry.yarnpkg.com/@typescript-eslint/type-utils/-/type-utils-5.40.1.tgz#091e4ce3bebbdb68f4980bae9dee2e4e1725f601"
-  integrity sha512-DLAs+AHQOe6n5LRraXiv27IYPhleF0ldEmx6yBqBgBLaNRKTkffhV1RPsjoJBhVup2zHxfaRtan8/YRBgYhU9Q==
+"@typescript-eslint/scope-manager@5.41.0":
+  version "5.41.0"
+  resolved "https://registry.yarnpkg.com/@typescript-eslint/scope-manager/-/scope-manager-5.41.0.tgz#28e3a41d626288d0628be14cf9de8d49fc30fadf"
+  integrity sha512-xOxPJCnuktUkY2xoEZBKXO5DBCugFzjrVndKdUnyQr3+9aDWZReKq9MhaoVnbL+maVwWJu/N0SEtrtEUNb62QQ==
+  dependencies:
+    "@typescript-eslint/types" "5.41.0"
+    "@typescript-eslint/visitor-keys" "5.41.0"
+
+"@typescript-eslint/type-utils@5.41.0":
+  version "5.41.0"
+  resolved "https://registry.yarnpkg.com/@typescript-eslint/type-utils/-/type-utils-5.41.0.tgz#2371601171e9f26a4e6da918a7913f7266890cdf"
+  integrity sha512-L30HNvIG6A1Q0R58e4hu4h+fZqaO909UcnnPbwKiN6Rc3BUEx6ez2wgN7aC0cBfcAjZfwkzE+E2PQQ9nEuoqfA==
   dependencies:
-    "@typescript-eslint/typescript-estree" "5.40.1"
-    "@typescript-eslint/utils" "5.40.1"
+    "@typescript-eslint/typescript-estree" "5.41.0"
+    "@typescript-eslint/utils" "5.41.0"
     debug "^4.3.4"
     tsutils "^3.21.0"
 
-"@typescript-eslint/types@5.40.1":
-  version "5.40.1"
-  resolved "https://registry.yarnpkg.com/@typescript-eslint/types/-/types-5.40.1.tgz#de37f4f64de731ee454bb2085d71030aa832f749"
-  integrity sha512-Icg9kiuVJSwdzSQvtdGspOlWNjVDnF3qVIKXdJ103o36yRprdl3Ge5cABQx+csx960nuMF21v8qvO31v9t3OHw==
-
-"@typescript-eslint/typescript-estree@5.40.1":
-  version "5.40.1"
-  resolved "https://registry.yarnpkg.com/@typescript-eslint/typescript-estree/-/typescript-estree-5.40.1.tgz#9a7d25492f02c69882ce5e0cd1857b0c55645d72"
-  integrity sha512-5QTP/nW5+60jBcEPfXy/EZL01qrl9GZtbgDZtDPlfW5zj/zjNrdI2B5zMUHmOsfvOr2cWqwVdWjobCiHcedmQA==
+"@typescript-eslint/types@5.41.0":
+  version "5.41.0"
+  resolved "https://registry.yarnpkg.com/@typescript-eslint/types/-/types-5.41.0.tgz#6800abebc4e6abaf24cdf220fb4ce28f4ab09a85"
+  integrity sha512-5BejraMXMC+2UjefDvrH0Fo/eLwZRV6859SXRg+FgbhA0R0l6lDqDGAQYhKbXhPN2ofk2kY5sgGyLNL907UXpA==
+
+"@typescript-eslint/typescript-estree@5.41.0":
+  version "5.41.0"
+  resolved "https://registry.yarnpkg.com/@typescript-eslint/typescript-estree/-/typescript-estree-5.41.0.tgz#bf5c6b3138adbdc73ba4871d060ae12c59366c61"
+  integrity sha512-SlzFYRwFSvswzDSQ/zPkIWcHv8O5y42YUskko9c4ki+fV6HATsTODUPbRbcGDFYP86gaJL5xohUEytvyNNcXWg==
   dependencies:
-    "@typescript-eslint/types" "5.40.1"
-    "@typescript-eslint/visitor-keys" "5.40.1"
+    "@typescript-eslint/types" "5.41.0"
+    "@typescript-eslint/visitor-keys" "5.41.0"
     debug "^4.3.4"
     globby "^11.1.0"
     is-glob "^4.0.3"
     semver "^7.3.7"
     tsutils "^3.21.0"
 
-"@typescript-eslint/utils@5.40.1":
-  version "5.40.1"
-  resolved "https://registry.yarnpkg.com/@typescript-eslint/utils/-/utils-5.40.1.tgz#3204fb73a559d3b7bab7dc9d3c44487c2734a9ca"
-  integrity sha512-a2TAVScoX9fjryNrW6BZRnreDUszxqm9eQ9Esv8n5nXApMW0zeANUYlwh/DED04SC/ifuBvXgZpIK5xeJHQ3aw==
+"@typescript-eslint/utils@5.41.0":
+  version "5.41.0"
+  resolved "https://registry.yarnpkg.com/@typescript-eslint/utils/-/utils-5.41.0.tgz#f41ae5883994a249d00b2ce69f4188f3a23fa0f9"
+  integrity sha512-QlvfwaN9jaMga9EBazQ+5DDx/4sAdqDkcs05AsQHMaopluVCUyu1bTRUVKzXbgjDlrRAQrYVoi/sXJ9fmG+KLQ==
   dependencies:
     "@types/json-schema" "^7.0.9"
     "@types/semver" "^7.3.12"
-    "@typescript-eslint/scope-manager" "5.40.1"
-    "@typescript-eslint/types" "5.40.1"
-    "@typescript-eslint/typescript-estree" "5.40.1"
+    "@typescript-eslint/scope-manager" "5.41.0"
+    "@typescript-eslint/types" "5.41.0"
+    "@typescript-eslint/typescript-estree" "5.41.0"
     eslint-scope "^5.1.1"
     eslint-utils "^3.0.0"
     semver "^7.3.7"
 
-"@typescript-eslint/visitor-keys@5.40.1":
-  version "5.40.1"
-  resolved "https://registry.yarnpkg.com/@typescript-eslint/visitor-keys/-/visitor-keys-5.40.1.tgz#f3d2bf5af192f4432b84cec6fdcb387193518754"
-  integrity sha512-A2DGmeZ+FMja0geX5rww+DpvILpwo1OsiQs0M+joPWJYsiEFBLsH0y1oFymPNul6Z5okSmHpP4ivkc2N0Cgfkw==
+"@typescript-eslint/visitor-keys@5.41.0":
+  version "5.41.0"
+  resolved "https://registry.yarnpkg.com/@typescript-eslint/visitor-keys/-/visitor-keys-5.41.0.tgz#d3510712bc07d5540160ed3c0f8f213b73e3bcd9"
+  integrity sha512-vilqeHj267v8uzzakbm13HkPMl7cbYpKVjgFWZPIOHIJHZtinvypUhJ5xBXfWYg4eFKqztbMMpOgFpT9Gfx4fw==
   dependencies:
-    "@typescript-eslint/types" "5.40.1"
+    "@typescript-eslint/types" "5.41.0"
     eslint-visitor-keys "^3.3.0"
 
 "@verdaccio/commons-api@10.2.0":
   version "10.2.0"
   resolved "https://registry.yarnpkg.com/@verdaccio/commons-api/-/commons-api-10.2.0.tgz#3b684c31749837b0574375bb2e10644ecea9fcca"
   integrity sha512-F/YZANu4DmpcEV0jronzI7v2fGVWkQ5Mwi+bVmV+ACJ+EzR0c9Jbhtbe5QyLUuzR97t8R5E/Xe53O0cc2LukdQ==
   dependencies:
@@ -1341,17 +1341,17 @@
 
 acorn@^7.1.1, acorn@^7.4.0:
   version "7.4.1"
   resolved "https://registry.yarnpkg.com/acorn/-/acorn-7.4.1.tgz#feaed255973d2e77555b83dbc08851a6c63520fa"
   integrity sha512-nQyp0o1/mNdbTO1PO6kHkwSrmgZ0MT/jCCpNiwbUjGoRN4dlBhqJtoQuCnEOKzgTVwg0ZWiCoQy6SxMebQVh8A==
 
 acorn@^8.2.4, acorn@^8.5.0, acorn@^8.7.1:
-  version "8.8.0"
-  resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.8.0.tgz#88c0187620435c7f6015803f5539dae05a9dbea8"
-  integrity sha512-QOxyigPVrpZ2GXT+PFyZTl6TtOFc5egxHIP9IlQ+RbupQuX4RkT/Bee4/kQuC02Xkzg84JcT7oLYtDIQxp+v7w==
+  version "8.8.1"
+  resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.8.1.tgz#0a3f9cbecc4ec3bea6f0a80b66ae8dd2da250b73"
+  integrity sha512-7zFpHzhnqYKrkYdUjF1HI1bzd0VygEGX8lFk4k5zVMqHEoES+P+7TKI+EvLO9WVMJ8eekdO0aDEK044xTXwPPA==
 
 agent-base@6:
   version "6.0.2"
   resolved "https://registry.yarnpkg.com/agent-base/-/agent-base-6.0.2.tgz#49fff58577cfee3f37176feab4c22e00f86d7f77"
   integrity sha512-RZNwNclF7+MS/8bDg70amg32dyeZGZxiDuQmZxKLAlQjr3jGyLx+4Kkk58UO7D2QdgFIQCovuSuZESne6RG6XQ==
   dependencies:
     debug "4"
@@ -1656,17 +1656,17 @@
 
 callsites@^3.0.0:
   version "3.1.0"
   resolved "https://registry.yarnpkg.com/callsites/-/callsites-3.1.0.tgz#b3630abd8943432f54b3f0519238e33cd7df2f73"
   integrity sha512-P8BjAsXvZS+VIDUI11hHCQEv74YT67YUi5JJFNWIqL235sBmjX4+qx9Muvls5ivyNENctx46xQLQ3aTuE7ssaQ==
 
 caniuse-lite@^1.0.30001400:
-  version "1.0.30001422"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001422.tgz#f2d7c6202c49a8359e6e35add894d88ef93edba1"
-  integrity sha512-hSesn02u1QacQHhaxl/kNMZwqVG35Sz/8DgvmgedxSH8z9UUpcDYSPYgsj3x5dQNRcNp6BwpSfQfVzYUTm+fog==
+  version "1.0.30001425"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001425.tgz#52917791a453eb3265143d2cd08d80629e82c735"
+  integrity sha512-/pzFv0OmNG6W0ym80P3NtapU0QEiDS3VuYAZMGoLLqiC7f6FJFe1MjpQDREGApeenD9wloeytmVDj+JLXPC6qw==
 
 caseless@~0.12.0:
   version "0.12.0"
   resolved "https://registry.yarnpkg.com/caseless/-/caseless-0.12.0.tgz#1b681c21ff84033c826543090689420d187151dc"
   integrity sha512-4tYFyifaFfGacoiObjJegolkwSU4xQNGbVgUiNYVUxbQ2x2lUsFvY4hVgVzGiIe6WLOPqycWXA40l+PWsxthUw==
 
 chalk@^2.0.0, chalk@^2.3.0, chalk@^2.4.1:
@@ -1888,17 +1888,17 @@
   resolved "https://registry.yarnpkg.com/cookies/-/cookies-0.8.0.tgz#1293ce4b391740a8406e3c9870e828c4b54f3f90"
   integrity sha512-8aPsApQfebXnuI+537McwYsDtjVxGm8gTIzQI3FDW6t5t/DAhERxtnbEPN/8RX+uZthoz4eCOgloXaE5cYyNow==
   dependencies:
     depd "~2.0.0"
     keygrip "~1.1.0"
 
 core-js-pure@^3.6.5:
-  version "3.25.5"
-  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.25.5.tgz#79716ba54240c6aa9ceba6eee08cf79471ba184d"
-  integrity sha512-oml3M22pHM+igfWHDfdLVq2ShWmjM2V4L+dQEBs0DWVIqEm9WHCwGAlZ6BmyBQGy5sFrJmcx+856D9lVKyGWYg==
+  version "3.26.0"
+  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.26.0.tgz#7ad8a5dd7d910756f3124374b50026e23265ca9a"
+  integrity sha512-LiN6fylpVBVwT8twhhluD9TzXmZQQsr2I2eIKtWNbZI1XMfBT7CV18itaN6RA7EtQd/SDdRx/wzvAShX2HvhQA==
 
 core-util-is@1.0.2:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/core-util-is/-/core-util-is-1.0.2.tgz#b5fd54220aa2bc5ab57aab7140c940754503c1a7"
   integrity sha512-3lqz5YjWTYnW6dlDa5TLaTCcShfar1e40rmcJVwCBJC6mWlFuj0eCHIElmG1g5kyuJ/GD+8Wn4FFCcz4gJPfaQ==
 
 cors@2.8.5:
@@ -3819,17 +3819,17 @@
   integrity sha512-qH0WSMBtn/oHuwjy/NucEgbx5dbxxnxup9s4PVXJUDHZBQY+s0NWA9rJf53RBnQZxfch7euUui7hpoAPvALZdA==
   dependencies:
     big.js "^5.2.2"
     emojis-list "^3.0.0"
     json5 "^1.0.1"
 
 loader-utils@^2.0.0, loader-utils@~2.0.0:
-  version "2.0.2"
-  resolved "https://registry.yarnpkg.com/loader-utils/-/loader-utils-2.0.2.tgz#d6e3b4fb81870721ae4e0868ab11dd638368c129"
-  integrity sha512-TM57VeHptv569d/GKh6TAYdzKblwDNiumOdkFnejjD0XwTH87K90w3O7AiJRqdQoXygvi1VQTJTLGhJl7WqA7A==
+  version "2.0.3"
+  resolved "https://registry.yarnpkg.com/loader-utils/-/loader-utils-2.0.3.tgz#d4b15b8504c63d1fc3f2ade52d41bc8459d6ede1"
+  integrity sha512-THWqIsn8QRnvLl0shHYVBN9syumU8pYWEHPTmkiVGd+7K5eFNVSY6AJhRvgGF70gg1Dz+l/k8WicvFCxdEs60A==
   dependencies:
     big.js "^5.2.2"
     emojis-list "^3.0.0"
     json5 "^2.1.2"
 
 locate-path@^5.0.0:
   version "5.0.0"
@@ -5735,17 +5735,17 @@
   resolved "https://registry.yarnpkg.com/typestyle/-/typestyle-2.4.0.tgz#df5bae6ff15093f5ce51f0caac5ef79428f64e78"
   integrity sha512-/d1BL6Qi+YlMLEydnUEB8KL/CAjAN8cyt3/UyGnOyBrWf7bLGcR/6yhmsaUstO2IcYwZfagjE7AIzuI2vUW9mg==
   dependencies:
     csstype "3.0.10"
     free-style "3.1.0"
 
 uglify-js@^3.1.4:
-  version "3.17.3"
-  resolved "https://registry.yarnpkg.com/uglify-js/-/uglify-js-3.17.3.tgz#f0feedf019c4510f164099e8d7e72ff2d7304377"
-  integrity sha512-JmMFDME3iufZnBpyKL+uS78LRiC+mK55zWfM5f/pWBJfpOttXAqYfdDGRukYhJuyRinvPVAtUhvy7rlDybNtFg==
+  version "3.17.4"
+  resolved "https://registry.yarnpkg.com/uglify-js/-/uglify-js-3.17.4.tgz#61678cf5fa3f5b7eb789bb345df29afb8257c22c"
+  integrity sha512-T9q82TJI9e/C1TAxYvfb16xO120tMVFZrGA3f9/P4424DNu6ypK103y0GPFVa17yotwSyZW5iYXgjYHkGrJW/g==
 
 unbox-primitive@^1.0.2:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/unbox-primitive/-/unbox-primitive-1.0.2.tgz#29032021057d5e6cdbd08c5129c226dff8ed6f9e"
   integrity sha512-61pPlCD9h51VoreyJ0BReideM3MDKMKnh6+V9L08331ipq6Q8OFXZYiqP6n/tbHx4s5I9uRhcye6BrbkizkBDw==
   dependencies:
     call-bind "^1.0.2"
```

