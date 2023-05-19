# Comparing `tmp/jupyterlab_limit_output-1.0.1.tar.gz` & `tmp/jupyterlab_limit_output-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyterlab_limit_output-1.0.1.tar", last modified: Mon Mar 27 18:59:24 2023, max compression
+gzip compressed data, was "dist/jupyterlab_limit_output-2.0.0.tar", last modified: Fri May 19 13:06:09 2023, max compression
```

## Comparing `jupyterlab_limit_output-1.0.1.tar` & `jupyterlab_limit_output-2.0.0.tar`

### file list

```diff
@@ -1,53 +1,60 @@
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-03-27 18:59:24.747143 jupyterlab_limit_output-1.0.1/
--rw-r--r--   0 udoff      (501) staff       (20)     1504 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/LICENSE.txt
--rw-r--r--   0 udoff      (501) staff       (20)      466 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/MANIFEST.in
--rw-r--r--   0 udoff      (501) staff       (20)     5714 2023-03-27 18:59:24.746910 jupyterlab_limit_output-1.0.1/PKG-INFO
--rw-r--r--   0 udoff      (501) staff       (20)     4996 2022-10-24 17:50:05.000000 jupyterlab_limit_output-1.0.1/README.md
--rw-r--r--   0 udoff      (501) staff       (20)      207 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/install.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-03-27 18:59:24.724382 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/
--rw-r--r--   0 udoff      (501) staff       (20)      326 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/__init__.py
--rw-r--r--   0 udoff      (501) staff       (20)      458 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/_version.py
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-03-27 18:59:24.732883 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/
--rw-r--r--   0 udoff      (501) staff       (20)    21201 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/build_log.json
--rw-r--r--   0 udoff      (501) staff       (20)      207 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/install.json
--rw-r--r--   0 udoff      (501) staff       (20)     3216 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/package.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-03-27 18:59:24.718188 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/schemas/
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-03-27 18:59:24.733811 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/schemas/jupyterlab-limit-output/
--rw-r--r--   0 udoff      (501) staff       (20)     3074 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/schemas/jupyterlab-limit-output/package.json.orig
--rw-r--r--   0 udoff      (501) staff       (20)     1041 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/schemas/jupyterlab-limit-output/settings.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-03-27 18:59:24.739758 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/
--rw-r--r--   0 udoff      (501) staff       (20)    12167 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/lib_index_js.088e5e2afd8e68ef3f50.js
--rw-r--r--   0 udoff      (501) staff       (20)    13821 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/lib_index_js.088e5e2afd8e68ef3f50.js.map
--rw-r--r--   0 udoff      (501) staff       (20)    12740 2023-03-27 18:17:33.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/lib_index_js.8f7e72224f999b4227c6.js
--rw-r--r--   0 udoff      (501) staff       (20)    14486 2023-03-27 18:17:33.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/lib_index_js.8f7e72224f999b4227c6.js.map
--rw-r--r--   0 udoff      (501) staff       (20)    27974 2023-03-27 18:17:33.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/remoteEntry.03e3d8532caa3afb5cc7.js
--rw-r--r--   0 udoff      (501) staff       (20)    26892 2023-03-27 18:17:33.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/remoteEntry.03e3d8532caa3afb5cc7.js.map
--rw-r--r--   0 udoff      (501) staff       (20)    27998 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/remoteEntry.bc9290952d30db774139.js
--rw-r--r--   0 udoff      (501) staff       (20)    26922 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/remoteEntry.bc9290952d30db774139.js.map
--rw-r--r--   0 udoff      (501) staff       (20)      166 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/style.js
--rw-r--r--   0 udoff      (501) staff       (20)     5007 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/style_index_js.a8027a2cb024ffc2c646.js
--rw-r--r--   0 udoff      (501) staff       (20)     2382 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/style_index_js.a8027a2cb024ffc2c646.js.map
--rw-r--r--   0 udoff      (501) staff       (20)    12076 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4806e8ff31b66ffc0443.js
--rw-r--r--   0 udoff      (501) staff       (20)    13817 2023-03-27 18:30:45.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4806e8ff31b66ffc0443.js.map
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-03-27 18:59:24.732069 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output.egg-info/
--rw-r--r--   0 udoff      (501) staff       (20)     5714 2023-03-27 18:59:24.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output.egg-info/PKG-INFO
--rw-r--r--   0 udoff      (501) staff       (20)     2110 2023-03-27 18:59:24.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output.egg-info/SOURCES.txt
--rw-r--r--   0 udoff      (501) staff       (20)        1 2023-03-27 18:59:24.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output.egg-info/dependency_links.txt
--rw-r--r--   0 udoff      (501) staff       (20)        1 2023-03-27 18:59:24.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output.egg-info/not-zip-safe
--rw-r--r--   0 udoff      (501) staff       (20)       23 2023-03-27 18:59:24.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output.egg-info/requires.txt
--rw-r--r--   0 udoff      (501) staff       (20)       24 2023-03-27 18:59:24.000000 jupyterlab_limit_output-1.0.1/jupyterlab_limit_output.egg-info/top_level.txt
--rw-r--r--   0 udoff      (501) staff       (20)     3074 2023-03-27 18:58:03.000000 jupyterlab_limit_output-1.0.1/package.json
--rw-r--r--   0 udoff      (501) staff       (20)      274 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/pyproject.toml
--rw-r--r--   0 udoff      (501) staff       (20)       38 2023-03-27 18:59:24.747196 jupyterlab_limit_output-1.0.1/setup.cfg
--rw-r--r--   0 udoff      (501) staff       (20)     2135 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/setup.py
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-03-27 18:59:24.742170 jupyterlab_limit_output-1.0.1/src/
--rw-r--r--   0 udoff      (501) staff       (20)     2340 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/src/formatters.ts
--rw-r--r--   0 udoff      (501) staff       (20)     2145 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/src/index.ts
--rw-r--r--   0 udoff      (501) staff       (20)     6458 2023-03-27 18:58:03.000000 jupyterlab_limit_output-1.0.1/src/renders.ts
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-03-27 18:59:24.746500 jupyterlab_limit_output-1.0.1/style/
--rw-r--r--   0 udoff      (501) staff       (20)      290 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/style/base.css
--rw-r--r--   0 udoff      (501) staff       (20)       25 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/style/index.css
--rw-r--r--   0 udoff      (501) staff       (20)       21 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/style/index.js
--rw-r--r--   0 udoff      (501) staff       (20)      557 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/tsconfig.json
--rw-r--r--   0 udoff      (501) staff       (20)     3177 2022-02-18 23:19:00.000000 jupyterlab_limit_output-1.0.1/tslint.json
--rw-r--r--   0 udoff      (501) staff       (20)   281106 2022-02-18 23:24:54.000000 jupyterlab_limit_output-1.0.1/yarn.lock
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.431073 jupyterlab_limit_output-2.0.0/
+-rw-r--r--   0 udoff      (501) staff       (20)     1504 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/LICENSE.txt
+-rw-r--r--   0 udoff      (501) staff       (20)      466 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/MANIFEST.in
+-rw-r--r--   0 udoff      (501) staff       (20)     5999 2023-05-19 13:06:09.430847 jupyterlab_limit_output-2.0.0/PKG-INFO
+-rw-r--r--   0 udoff      (501) staff       (20)     5048 2023-05-19 12:46:57.000000 jupyterlab_limit_output-2.0.0/README.md
+-rw-r--r--   0 udoff      (501) staff       (20)      207 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/install.json
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.410929 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/
+-rw-r--r--   0 udoff      (501) staff       (20)      326 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/__init__.py
+-rw-r--r--   0 udoff      (501) staff       (20)      458 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/_version.py
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.415219 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/
+-rw-r--r--   0 udoff      (501) staff       (20)    20817 2023-05-19 13:05:09.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/build_log.json
+-rw-r--r--   0 udoff      (501) staff       (20)     3156 2023-05-19 13:05:11.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/package.json
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.399251 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/schemas/
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.416410 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/schemas/jupyterlab-limit-output/
+-rw-r--r--   0 udoff      (501) staff       (20)     3014 2023-05-19 13:05:09.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/schemas/jupyterlab-limit-output/package.json.orig
+-rw-r--r--   0 udoff      (501) staff       (20)     1041 2023-05-19 13:05:09.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/schemas/jupyterlab-limit-output/settings.json
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.422156 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/
+-rw-r--r--   0 udoff      (501) staff       (20)    12892 2023-05-19 13:05:11.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/lib_index_js.ffe2091edae0050147bf.js
+-rw-r--r--   0 udoff      (501) staff       (20)    14654 2023-05-19 13:05:11.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/lib_index_js.ffe2091edae0050147bf.js.map
+-rw-r--r--   0 udoff      (501) staff       (20)    27824 2023-05-19 13:05:11.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/remoteEntry.d8030784757a1c70623e.js
+-rw-r--r--   0 udoff      (501) staff       (20)    26714 2023-05-19 13:05:11.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/remoteEntry.d8030784757a1c70623e.js.map
+-rw-r--r--   0 udoff      (501) staff       (20)      166 2023-05-19 13:05:09.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/style.js
+-rw-r--r--   0 udoff      (501) staff       (20)    19757 2023-05-19 13:05:11.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/style_index_js.8737596b5ac0bbefe59d.js
+-rw-r--r--   0 udoff      (501) staff       (20)    15380 2023-05-19 13:05:11.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/style_index_js.8737596b5ac0bbefe59d.js.map
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.414607 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output.egg-info/
+-rw-r--r--   0 udoff      (501) staff       (20)     5999 2023-05-19 13:06:09.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output.egg-info/PKG-INFO
+-rw-r--r--   0 udoff      (501) staff       (20)     1681 2023-05-19 13:06:09.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output.egg-info/SOURCES.txt
+-rw-r--r--   0 udoff      (501) staff       (20)        1 2023-05-19 13:06:09.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output.egg-info/dependency_links.txt
+-rw-r--r--   0 udoff      (501) staff       (20)        1 2023-03-27 18:59:24.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output.egg-info/not-zip-safe
+-rw-r--r--   0 udoff      (501) staff       (20)       25 2023-05-19 13:06:09.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output.egg-info/requires.txt
+-rw-r--r--   0 udoff      (501) staff       (20)       99 2023-05-19 13:06:09.000000 jupyterlab_limit_output-2.0.0/jupyterlab_limit_output.egg-info/top_level.txt
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.399821 jupyterlab_limit_output-2.0.0/myvenv/
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.426422 jupyterlab_limit_output-2.0.0/myvenv/bin/
+-rwxr-xr-x   0 udoff      (501) staff       (20)      648 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2html.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)      770 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2html4.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)     1115 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2html5.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)      847 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2latex.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)      670 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2man.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)      836 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2odt.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)     1774 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)      655 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)      691 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2s5.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)      927 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2xetex.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)      656 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rst2xml.py
+-rwxr-xr-x   0 udoff      (501) staff       (20)      724 2023-03-27 19:00:50.000000 jupyterlab_limit_output-2.0.0/myvenv/bin/rstpep2html.py
+-rw-r--r--   0 udoff      (501) staff       (20)     3014 2023-05-19 12:59:19.000000 jupyterlab_limit_output-2.0.0/package.json
+-rw-r--r--   0 udoff      (501) staff       (20)      280 2023-05-17 15:01:08.000000 jupyterlab_limit_output-2.0.0/pyproject.toml
+-rw-r--r--   0 udoff      (501) staff       (20)       38 2023-05-19 13:06:09.431133 jupyterlab_limit_output-2.0.0/setup.cfg
+-rw-r--r--   0 udoff      (501) staff       (20)     2388 2023-05-19 12:44:14.000000 jupyterlab_limit_output-2.0.0/setup.py
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.429158 jupyterlab_limit_output-2.0.0/src/
+-rw-r--r--   0 udoff      (501) staff       (20)     2340 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/src/formatters.ts
+-rw-r--r--   0 udoff      (501) staff       (20)     2145 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/src/index.ts
+-rw-r--r--   0 udoff      (501) staff       (20)     6458 2023-03-27 18:58:03.000000 jupyterlab_limit_output-2.0.0/src/renders.ts
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:06:09.430556 jupyterlab_limit_output-2.0.0/style/
+-rw-r--r--   0 udoff      (501) staff       (20)      290 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/style/base.css
+-rw-r--r--   0 udoff      (501) staff       (20)       25 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/style/index.css
+-rw-r--r--   0 udoff      (501) staff       (20)       21 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/style/index.js
+-rw-r--r--   0 udoff      (501) staff       (20)      557 2023-05-17 15:01:08.000000 jupyterlab_limit_output-2.0.0/tsconfig.json
+-rw-r--r--   0 udoff      (501) staff       (20)     3177 2022-02-18 23:19:00.000000 jupyterlab_limit_output-2.0.0/tslint.json
+-rw-r--r--   0 udoff      (501) staff       (20)   201742 2023-05-19 12:51:50.000000 jupyterlab_limit_output-2.0.0/yarn.lock
```

### Comparing `jupyterlab_limit_output-1.0.1/LICENSE.txt` & `jupyterlab_limit_output-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_limit_output-1.0.1/PKG-INFO` & `jupyterlab_limit_output-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: jupyterlab_limit_output
-Version: 1.0.1
+Version: 2.0.0
 Summary: Limit output text mime-renders
 Home-page: https://github.com/deshaw/jupyterlab-limit-output
 Author: Marc Udoff
 License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
+Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # jupyterlab-limit-output
 
 [![PyPI version][pypi-image]][pypi-url] [![PyPI DM][pypi-dm-image]][pypi-url]
 [![Github Actions Status][github-status-image]][github-status-url] [![Binder][binder-image]][binder-url]
@@ -107,15 +111,16 @@
 git tag vX.Z.Y
 git push && git push --tags
 ```
 
 3. Create the artifacts
 
 ```
-rm -rf dist
+rm -rf dist jupyterlab_limit_output/labextension
+jlpm run build
 python setup.py sdist bdist_wheel
 ```
 
 4. Test this against the test pypi. You can then install from here to test as well:
 
 ```
 twine upload --repository-url https://test.pypi.org/legacy/ dist/*
```

### Comparing `jupyterlab_limit_output-1.0.1/README.md` & `jupyterlab_limit_output-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,16 @@
 git tag vX.Z.Y
 git push && git push --tags
 ```
 
 3. Create the artifacts
 
 ```
-rm -rf dist
+rm -rf dist jupyterlab_limit_output/labextension
+jlpm run build
 python setup.py sdist bdist_wheel
 ```
 
 4. Test this against the test pypi. You can then install from here to test as well:
 
 ```
 twine upload --repository-url https://test.pypi.org/legacy/ dist/*
```

#### html2text {}

```diff
@@ -36,22 +36,22 @@
 the source maps for this extension to make it easier to debug using the browser
 dev tools. To also generate source maps for the JupyterLab core extensions, you
 can run the following command: ```bash jupyter lab build --minimize=False ```
 #### Publishing Before starting, you'll need to have run: `pip install twine
 jupyter_packaging` 1. Update the version in `package.json` and update the
 release date in `CHANGELOG.md` 2. Commit the change in step 1, tag it, then
 push it ``` git commit -am  git tag vX.Z.Y git push && git push --tags ``` 3.
-Create the artifacts ``` rm -rf dist python setup.py sdist bdist_wheel ``` 4.
-Test this against the test pypi. You can then install from here to test as
-well: ``` twine upload --repository-url https://test.pypi.org/legacy/ dist/* #
-In a new venv pip install --index-url https://test.pypi.org/simple/
-jupyterlab_limit_output ``` 5. Upload this to pypi: ``` twine upload dist/* ```
-### Uninstall ```bash pip uninstall jupyterlab_limit_output ``` ## History This
-plugin was contributed back to the community by the [D. E. Shaw group](https://
-www.deshaw.com/).
+Create the artifacts ``` rm -rf dist jupyterlab_limit_output/labextension jlpm
+run build python setup.py sdist bdist_wheel ``` 4. Test this against the test
+pypi. You can then install from here to test as well: ``` twine upload --
+repository-url https://test.pypi.org/legacy/ dist/* # In a new venv pip install
+--index-url https://test.pypi.org/simple/ jupyterlab_limit_output ``` 5. Upload
+this to pypi: ``` twine upload dist/* ``` ### Uninstall ```bash pip uninstall
+jupyterlab_limit_output ``` ## History This plugin was contributed back to the
+community by the [D. E. Shaw group](https://www.deshaw.com/).
                                [D._E._Shaw_Logo]
 ## License This project is released under a [BSD-3-Clause license](https://
 github.com/deshaw/jupyterlab-limit-output/blob/main/LICENSE.txt). We love
 contributions! Before you can contribute, please sign and submit this
 [Contributor License Agreement (CLA)](https://www.deshaw.com/oss/cla). This CLA
 is in place to protect all users of this project. "Jupyter" is a trademark of
 the NumFOCUS foundation, of which Project Jupyter is a part. [pypi-url]: https:
```

### Comparing `jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/package.json` & `jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/package.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8905762670565301%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.0', '@jupyterlab/rendermime': '^4.0.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@types/chai': '^4.3.4', '@types/mocha': "*

 * *                      "'^10.0.1', '@typescript-eslint/eslint-plugin': '^5.55.0', "*

 * *                      "'@typescript-eslint/parser': '^5.55.0', 'chai': '^4.3.7', "*

 * *                      "'eslint-config-prettier': '^8. […]*

```diff
@@ -1,55 +1,50 @@
 {
     "bugs": {
         "url": "https://github.com/deshaw/jupyterlab-limit-output/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/rendermime": "^3.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/rendermime": "^4.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
     "description": "Limit output text mime-renders",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.12",
-        "@types/chai": "^4.2.22",
-        "@types/mocha": "^9.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.32.0",
-        "@typescript-eslint/parser": "^4.32.0",
-        "chai": "^4.3.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/chai": "^4.3.4",
+        "@types/mocha": "^10.0.1",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "chai": "^4.3.7",
         "eslint": "^7.32.0",
-        "eslint-config-prettier": "^8.3.0",
-        "eslint-plugin-prettier": "^4.0.0",
-        "husky": "^4.2.3",
-        "mocha": "^9.1.2",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "husky": "^8.0.0",
+        "mocha": "^10.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.4.1",
-        "rimraf": "^3.0.2",
-        "ts-mocha": "^8.0.0",
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "ts-mocha": "^10.0.0",
         "tslint": "^6.1.3",
         "tslint-config-prettier": "^1.18.0",
         "tslint-plugin-prettier": "^2.3.0",
-        "typescript": "~4.1.3"
+        "typescript": "~5.0.2"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-limit-output",
-    "husky": {
-        "hooks": {
-            "pre-commit": "npm run lint && npm run test"
-        }
-    },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.bc9290952d30db774139.js",
+            "load": "static/remoteEntry.d8030784757a1c70623e.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_limit_output/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -75,23 +70,23 @@
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
         "clean:labextension": "rimraf jupyterlab_limit_output/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "eslint . --ext .ts,.tsx --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "install:extension": "jlpm run build",
         "lint": "npm run prettier && npm run tslint",
-        "prepare": "jlpm run clean && jlpm run build:prod",
+        "prepare": "jlpm run clean && jlpm run build:prod && husky install",
         "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "ts-mocha -p tests/tsconfig.json tests/**/*_spec.ts",
         "tslint": "tslint --fix -c tslint.json --project tsconfig.json '**/*{.ts,.tsx}'",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter-labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "2.0.0"
 }
```

### Comparing `jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/schemas/jupyterlab-limit-output/package.json.orig` & `jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/schemas/jupyterlab-limit-output/package.json.orig`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8911549707602339%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.0', '@jupyterlab/rendermime': '^4.0.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@types/chai': '^4.3.4', '@types/mocha': "*

 * *                      "'^10.0.1', '@typescript-eslint/eslint-plugin': '^5.55.0', "*

 * *                      "'@typescript-eslint/parser': '^5.55.0', 'chai': '^4.3.7', "*

 * *                      "'eslint-config-prettier': '^8. […]*

```diff
@@ -1,51 +1,46 @@
 {
     "bugs": {
         "url": "https://github.com/deshaw/jupyterlab-limit-output/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/rendermime": "^3.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/rendermime": "^4.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
     "description": "Limit output text mime-renders",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.12",
-        "@types/chai": "^4.2.22",
-        "@types/mocha": "^9.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.32.0",
-        "@typescript-eslint/parser": "^4.32.0",
-        "chai": "^4.3.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/chai": "^4.3.4",
+        "@types/mocha": "^10.0.1",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "chai": "^4.3.7",
         "eslint": "^7.32.0",
-        "eslint-config-prettier": "^8.3.0",
-        "eslint-plugin-prettier": "^4.0.0",
-        "husky": "^4.2.3",
-        "mocha": "^9.1.2",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "husky": "^8.0.0",
+        "mocha": "^10.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.4.1",
-        "rimraf": "^3.0.2",
-        "ts-mocha": "^8.0.0",
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "ts-mocha": "^10.0.0",
         "tslint": "^6.1.3",
         "tslint-config-prettier": "^1.18.0",
         "tslint-plugin-prettier": "^2.3.0",
-        "typescript": "~4.1.3"
+        "typescript": "~5.0.2"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-limit-output",
-    "husky": {
-        "hooks": {
-            "pre-commit": "npm run lint && npm run test"
-        }
-    },
     "jupyterlab": {
         "extension": true,
         "outputDir": "jupyterlab_limit_output/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
@@ -70,23 +65,23 @@
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
         "clean:labextension": "rimraf jupyterlab_limit_output/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "eslint . --ext .ts,.tsx --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "install:extension": "jlpm run build",
         "lint": "npm run prettier && npm run tslint",
-        "prepare": "jlpm run clean && jlpm run build:prod",
+        "prepare": "jlpm run clean && jlpm run build:prod && husky install",
         "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "ts-mocha -p tests/tsconfig.json tests/**/*_spec.ts",
         "tslint": "tslint --fix -c tslint.json --project tsconfig.json '**/*{.ts,.tsx}'",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter-labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "2.0.0"
 }
```

### Comparing `jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/schemas/jupyterlab-limit-output/settings.json` & `jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/schemas/jupyterlab-limit-output/settings.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/lib_index_js.088e5e2afd8e68ef3f50.js` & `jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/lib_index_js.ffe2091edae0050147bf.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -132,15 +132,15 @@
 
                         function updateSettings(settings) {
                             const head = settings.get('head').composite;
                             const tail = settings.get('tail').composite;
                             const enabled = settings.get('enabled').composite;
                             const method = settings.get('method')
                                 .composite;
-                            renders_1.updateLimitOutputSettings({
+                            (0, renders_1.updateLimitOutputSettings)({
                                 head,
                                 tail,
                                 method,
                                 enabled
                             });
                         }
                         settingRegistry.load(`${PLUGIN_NAME}:settings`).then((settings) => {
@@ -198,29 +198,30 @@
                     }
                 };
                 exports.updateLimitOutputSettings = updateLimitOutputSettings;
                 const limitOutputRenderText = async (options, _head = 0, _tail = 0, _cleanupButtonFn = null) => {
                     if (limitSettings.enabled) {
                         // We have to clone so that we can both keep track of number of head/tail
                         // shown as well as keep the original options unchanged
-                        const clonedOptions = Object.assign(Object.assign({}, options), {
+                        const clonedOptions = {
+                            ...options,
                             head: _head || limitSettings.head,
-                            tail: _tail || limitSettings.tail
-                        });
+                            tail: _tail || limitSettings.tail,
+                        };
                         if (limitSettings.method === 'characters') {
-                            clonedOptions.source = formatters_1.limitByCharacters(options.source, clonedOptions.head, clonedOptions.tail);
+                            clonedOptions.source = (0, formatters_1.limitByCharacters)(options.source, clonedOptions.head, clonedOptions.tail);
                         } else {
-                            clonedOptions.source = formatters_1.limitByLines(options.source, clonedOptions.head, clonedOptions.tail);
+                            clonedOptions.source = (0, formatters_1.limitByLines)(options.source, clonedOptions.head, clonedOptions.tail);
                         }
                         // Add a div so we can easily remove output
                         const div = document.createElement('div');
                         options.host.append(div);
                         clonedOptions.host = div;
                         // Wait for text to render so that we can add our buttons after it
-                        const ret = await rendermime_1.renderText(clonedOptions);
+                        const ret = await (0, rendermime_1.renderText)(clonedOptions);
                         // If we need to, add buttons for expanding output
                         if (_cleanupButtonFn === null &&
                             clonedOptions.source.length !== options.source.length) {
                             const expandLines = Math.max(limitSettings.tail, limitSettings.head);
                             const span = document.createElement('span');
                             [
                                 // label, expand head, expand tail, warn on click
@@ -258,45 +259,46 @@
                                             }
                                         } else {
                                             if (options.source.length > WARN_BEFORE_EXPANDING_SOURCE_LENGTH_CH) {
                                                 warningLabel = `${options.source.length.toLocaleString()} characters`;
                                             }
                                         }
                                         if (warningLabel) {
-                                            const result = await apputils_1.showDialog({
+                                            const result = await (0, apputils_1.showDialog)({
                                                 title: 'Show all',
                                                 body: `Do you really want to show all ${warningLabel}?`,
                                             });
                                             if (!result.button.accept) {
                                                 return;
                                             }
                                         }
                                     }
                                     // This binds the first clonedOptions call
                                     // i.e. future calls will updated clonedOptions but this onclick won't change
                                     clonedOptions.head += expandUp;
                                     clonedOptions.tail += expandDown;
-                                    await limitOutputRenderText(Object.assign(Object.assign({}, options), {
-                                        host: clonedOptions.host
-                                    }), clonedOptions.head, clonedOptions.tail, cleanup);
+                                    await limitOutputRenderText({
+                                        ...options,
+                                        host: clonedOptions.host,
+                                    }, clonedOptions.head, clonedOptions.tail, cleanup);
                                     // Not the best design, but we know the prev element added is the renderText one
                                     // so we remove it before we redisplay
                                     clonedOptions.host.childNodes.forEach((n) => n.remove());
                                 };
                                 span.appendChild(button);
                             });
                             options.host.append(span);
                             // We are fully expanded!
                         } else if (clonedOptions.source.length === options.source.length &&
                             _cleanupButtonFn) {
                             _cleanupButtonFn();
                         }
                         return ret;
                     }
-                    return rendermime_1.renderText(options);
+                    return (0, rendermime_1.renderText)(options);
                 };
                 class MyRenderedText extends rendermime_1.RenderedText {
                     /**
                      * Render a mime model.
                      *
                      * @param model - The mime model to render.
                      *
@@ -306,14 +308,29 @@
                         return limitOutputRenderText({
                             host: this.node,
                             sanitizer: this.sanitizer,
                             source: String(model.data[this.mimeType]),
                             translator: this.translator,
                         });
                     }
+                    /**
+                     * Dispose the contents of node to contain potential memory leak.
+                     *
+                     * **Notes**: when user attempts to clean the output using context menu
+                     * they invoke `JupyterFrontEnd.evtContextMenu` which caches the event
+                     * to enable commands and extensions to access it later; this leads to
+                     * a memory leak as the event holds the target node reference.
+                     */
+                    dispose() {
+                        // TODO: remove ts-ignore during JupyterLab 4.0/TypeScript 5.0 migration
+                        // eslint-disable-next-line @typescript-eslint/ban-ts-comment
+                        // @ts-ignore
+                        this.node.replaceChildren();
+                        super.dispose();
+                    }
                 }
                 exports.MyRenderedText = MyRenderedText;
                 exports.rendererFactory = {
                     safe: true,
                     mimeTypes: [
                         'text/plain',
                         'application/vnd.jupyter.stdout',
@@ -324,8 +341,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.088e5e2afd8e68ef3f50.js.map
+//# sourceMappingURL=lib_index_js.ffe2091edae0050147bf.js.map
```

### Comparing `jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/lib_index_js.088e5e2afd8e68ef3f50.js.map` & `jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/lib_index_js.ffe2091edae0050147bf.js.map`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7999999999999999%*

 * *Differences: {"'file'": "'lib_index_js.ffe2091edae0050147bf.js'",*

 * * "'mappings'": "';;;;;;;;;AAAa;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,oBAAoB,GAAG,yBAAyB;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B,KAAK;AACjC;AACA;AACA,sBAAsB,oBAAoB,OAAO,KAAK;AACtD;AACA,kBAAkB,QAAQ,EAAE,mBAAmB,kCAAkC,KAAK,aAAa,mBAAmB,EAAE,QAAQ;AAChI;AACA;AACA;AACA,yBAAyB;AACzB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,+BAA+B;AAC/B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AA […]*

```diff
@@ -1,17 +1,17 @@
 {
-    "file": "lib_index_js.088e5e2afd8e68ef3f50.js",
-    "mappings": ";;;;;;;;;AAAa;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,oBAAoB,GAAG,yBAAyB;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B,KAAK;AACjC;AACA;AACA,sBAAsB,oBAAoB,OAAO,KAAK;AACtD;AACA,kBAAkB,QAAQ,EAAE,mBAAmB,kCAAkC,KAAK,aAAa,mBAAmB,EAAE,QAAQ;AAChI;AACA;AACA;AACA,yBAAyB;AACzB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,+BAA+B;AAC/B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wBAAwB,KAAK;AAC7B;AACA;AACA,kBAAkB,oBAAoB,OAAO,KAAK;AAClD;AACA,cAAc,QAAQ,EAAE,mBAAmB,kCAAkC,KAAK,QAAQ,mBAAmB,EAAE,QAAQ;AACvH;AACA,oBAAoB;;;;;;;;;;;AC/EP;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,qBAAqB,mBAAO,CAAC,sFAAwB;AACrD,0BAA0B,mBAAO,CAAC,gGAA6B;AAC/D,kBAAkB,mBAAO,CAAC,mCAAW;AACrC;AACA;AACA,WAAW,YAAY;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA,WAAW,YAAY;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kDAAkD,6BAA6B;AAC/E;AACA,gCAAgC,YAAY;AAC5C;AACA;AACA,SAAS;AACT,0EAA0E,YAAY,IAAI,IAAI;AAC9F,SAAS;AACT,KAAK;AACL;AACA,kBAAe;;;;;;;;;;;ACtCF;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,uBAAuB,GAAG,sBAAsB,GAAG,iCAAiC;AACpF,qBAAqB,mBAAO,CAAC,sFAAwB;AACrD,qBAAqB,mBAAO,CAAC,yCAAc;AAC3C,mBAAmB,mBAAO,CAAC,kFAAsB;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC;AACjC;AACA;AACA;AACA;AACA,4DAA4D,cAAc,sEAAsE;AAChJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8BAA8B,aAAa,EAAE,qBAAqB;AAClE;AACA;AACA;AACA;AACA,6BAA6B,qBAAqB;AAClD;AACA,8BAA8B,aAAa,EAAE,qBAAqB;AAClE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4CAA4C,2BAA2B;AACvE;AACA;AACA;AACA;AACA;AACA,kDAAkD,wBAAwB;AAC1E;AACA;AACA;AACA;AACA,kDAAkD,wCAAwC;AAC1F;AACA;AACA;AACA;AACA;AACA,wEAAwE,aAAa;AACrF,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8EAA8E,cAAc,0BAA0B;AACtH;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA,sBAAsB;AACtB,uBAAuB;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA",
+    "file": "lib_index_js.ffe2091edae0050147bf.js",
+    "mappings": ";;;;;;;;;AAAa;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,oBAAoB,GAAG,yBAAyB;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B,KAAK;AACjC;AACA;AACA,sBAAsB,oBAAoB,OAAO,KAAK;AACtD;AACA,kBAAkB,QAAQ,EAAE,mBAAmB,kCAAkC,KAAK,aAAa,mBAAmB,EAAE,QAAQ;AAChI;AACA;AACA;AACA,yBAAyB;AACzB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,+BAA+B;AAC/B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wBAAwB,KAAK;AAC7B;AACA;AACA,kBAAkB,oBAAoB,OAAO,KAAK;AAClD;AACA,cAAc,QAAQ,EAAE,mBAAmB,kCAAkC,KAAK,QAAQ,mBAAmB,EAAE,QAAQ;AACvH;AACA,oBAAoB;;;;;;;;;;;AC/EP;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,qBAAqB,mBAAO,CAAC,sFAAwB;AACrD,0BAA0B,mBAAO,CAAC,gGAA6B;AAC/D,kBAAkB,mBAAO,CAAC,mCAAW;AACrC;AACA;AACA,WAAW,YAAY;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA,WAAW,YAAY;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uDAAuD,6BAA6B;AACpF;AACA,gCAAgC,YAAY;AAC5C;AACA;AACA,SAAS;AACT,0EAA0E,YAAY,IAAI,IAAI;AAC9F,SAAS;AACT,KAAK;AACL;AACA,kBAAe;;;;;;;;;;;ACtCF;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,uBAAuB,GAAG,sBAAsB,GAAG,iCAAiC;AACpF,qBAAqB,mBAAO,CAAC,sFAAwB;AACrD,qBAAqB,mBAAO,CAAC,yCAAc;AAC3C,mBAAmB,mBAAO,CAAC,kFAAsB;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC;AACjC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8BAA8B,aAAa,EAAE,qBAAqB;AAClE;AACA;AACA;AACA;AACA,6BAA6B,qBAAqB;AAClD;AACA,8BAA8B,aAAa,EAAE,qBAAqB;AAClE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4CAA4C,2BAA2B;AACvE;AACA;AACA;AACA;AACA;AACA,kDAAkD,wBAAwB;AAC1E;AACA;AACA;AACA;AACA,kDAAkD,wCAAwC;AAC1F;AACA;AACA;AACA;AACA;AACA,wEAAwE,aAAa;AACrF,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,6DAA6D;AAC7D;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB;AACtB,uBAAuB;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-limit-output/./lib/formatters.js",
         "webpack://jupyterlab-limit-output/./lib/index.js",
         "webpack://jupyterlab-limit-output/./lib/renders.js"
     ],
     "sourcesContent": [
         "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.limitByLines = exports.limitByCharacters = void 0;\nconst NEW_LINE = '\\n';\nconst SPACER = '\\n\\n\\n';\n/**\n * Return a string with at most head starting characters and tail ending (plus a warning)\n */\nconst limitByCharacters = (text, head, tail) => {\n    const maxChars = head + tail;\n    if (text.length > maxChars) {\n        const headstr = text.substring(0, head);\n        const tailstr = text.substring(text.length - tail);\n        let msg = '';\n        if (head) {\n            msg = ` first ${head}`;\n        }\n        if (tail) {\n            msg += `${head ? ' and' : ''} last ${tail}`;\n        }\n        return `${headstr}${head ? SPACER : ''}WARNING: Output limited. Showing${msg} characters.${tail ? SPACER : ''}${tailstr}`;\n    }\n    return text;\n};\nexports.limitByCharacters = limitByCharacters;\n/**\n * Find the nth index of the newline character\n */\nfunction _nthNewLineIndex(text, n) {\n    let idx = 0;\n    while (n-- > 0 && idx++ < text.length) {\n        idx = text.indexOf(NEW_LINE, idx);\n        // Not found before we ran out of n\n        if (idx < 0) {\n            return null;\n        }\n    }\n    return idx;\n}\n/**\n * Find the nth newline from the end of the string (excluding a possible final new line)\n */\nfunction _nthNewLineFromLastIndex(text, n) {\n    let idx = text.length - 1; // Ignore a possible final trailing \\n\n    while (n-- > 0 && idx-- >= 0) {\n        idx = text.lastIndexOf(NEW_LINE, idx);\n        // Not found before we ran out of n\n        if (idx < 0) {\n            return null;\n        }\n    }\n    return idx;\n}\n/**\n * Return a string with at most head starting lines and tail ending (plus a warning)\n */\nconst limitByLines = (text, head, tail) => {\n    const headEndPos = head > 0 ? _nthNewLineIndex(text, head) : -1;\n    if (headEndPos === null) {\n        return text;\n    }\n    const tailStartPos = tail > 0 ? _nthNewLineFromLastIndex(text, tail) : text.length;\n    if (tailStartPos === null) {\n        return text;\n    }\n    if (tailStartPos <= headEndPos) {\n        return text;\n    }\n    const headstr = text.substring(0, headEndPos);\n    const tailstr = text.substring(tailStartPos);\n    let msg = '';\n    if (head) {\n        msg = ` first ${head}`;\n    }\n    if (tail) {\n        msg += `${head ? ' and' : ''} last ${tail}`;\n    }\n    return `${headstr}${head ? SPACER : ''}WARNING: Output limited. Showing${msg} lines.${tail ? SPACER : ''}${tailstr}`;\n};\nexports.limitByLines = limitByLines;\n",
-        "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nconst rendermime_1 = require(\"@jupyterlab/rendermime\");\nconst settingregistry_1 = require(\"@jupyterlab/settingregistry\");\nconst renders_1 = require(\"./renders\");\nconst PLUGIN_NAME = 'jupyterlab-limit-output';\nconst extension = {\n    id: `${PLUGIN_NAME}:rendertext`,\n    rendererFactory: renders_1.rendererFactory,\n    // This number is NOT random. It's just lower (more preferred) than https://github.com/jupyterlab/jupyterlab/blob/0cbfcbe8c09d2c1fbfd1912f4d36c12479893946/packages/rendermime/src/factories.ts#L68\n    // Setting the rank too low makes the text version of renders too preferred (e.g. show text instead of the widget render)\n    rank: 119,\n    dataType: 'string',\n};\nconst RenderExtension = {\n    id: `${PLUGIN_NAME}:renders`,\n    autoStart: true,\n    requires: [rendermime_1.IRenderMimeRegistry, settingregistry_1.ISettingRegistry],\n    activate: function (app, rendermime, settingRegistry) {\n        // eslint-disable-next-line no-console\n        console.log('JupyterLab extension jupyterlab-limit-output is activated!');\n        rendermime.addFactory(extension.rendererFactory, extension.rank);\n        function updateSettings(settings) {\n            const head = settings.get('head').composite;\n            const tail = settings.get('tail').composite;\n            const enabled = settings.get('enabled').composite;\n            const method = settings.get('method')\n                .composite;\n            renders_1.updateLimitOutputSettings({ head, tail, method, enabled });\n        }\n        settingRegistry.load(`${PLUGIN_NAME}:settings`).then((settings) => {\n            updateSettings(settings);\n            settings.changed.connect(updateSettings);\n        }, (err) => {\n            console.error(`Could not load settings, so did not activate ${PLUGIN_NAME}: ${err}`);\n        });\n    },\n};\nexports.default = RenderExtension;\n",
-        "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.rendererFactory = exports.MyRenderedText = exports.updateLimitOutputSettings = void 0;\nconst rendermime_1 = require(\"@jupyterlab/rendermime\");\nconst formatters_1 = require(\"./formatters\");\nconst apputils_1 = require(\"@jupyterlab/apputils\");\nconst WARN_BEFORE_EXPANDING_SOURCE_LENGTH_CH = 100000;\nconst WARN_BEFORE_EXPANDING_SOURCE_LENGTH_LINES = 1000;\nlet limitSettings = {\n    head: 50,\n    tail: 50,\n    method: 'lines',\n    enabled: true,\n};\nconst updateLimitOutputSettings = (settings) => {\n    limitSettings = settings;\n    if (limitSettings.head < 0) {\n        limitSettings.head = 0;\n    }\n    if (limitSettings.tail < 0) {\n        limitSettings.tail = 0;\n    }\n    if (limitSettings.tail === 0 && limitSettings.head === 0) {\n        limitSettings.enabled = false;\n    }\n    if (limitSettings.method !== 'lines' &&\n        limitSettings.method !== 'characters') {\n        limitSettings.method = 'lines';\n    }\n};\nexports.updateLimitOutputSettings = updateLimitOutputSettings;\nconst limitOutputRenderText = async (options, _head = 0, _tail = 0, _cleanupButtonFn = null) => {\n    if (limitSettings.enabled) {\n        // We have to clone so that we can both keep track of number of head/tail\n        // shown as well as keep the original options unchanged\n        const clonedOptions = Object.assign(Object.assign({}, options), { head: _head || limitSettings.head, tail: _tail || limitSettings.tail });\n        if (limitSettings.method === 'characters') {\n            clonedOptions.source = formatters_1.limitByCharacters(options.source, clonedOptions.head, clonedOptions.tail);\n        }\n        else {\n            clonedOptions.source = formatters_1.limitByLines(options.source, clonedOptions.head, clonedOptions.tail);\n        }\n        // Add a div so we can easily remove output\n        const div = document.createElement('div');\n        options.host.append(div);\n        clonedOptions.host = div;\n        // Wait for text to render so that we can add our buttons after it\n        const ret = await rendermime_1.renderText(clonedOptions);\n        // If we need to, add buttons for expanding output\n        if (_cleanupButtonFn === null &&\n            clonedOptions.source.length !== options.source.length) {\n            const expandLines = Math.max(limitSettings.tail, limitSettings.head);\n            const span = document.createElement('span');\n            [\n                // label, expand head, expand tail, warn on click\n                [\n                    `\u2191 Show ${expandLines} ${limitSettings.method}`,\n                    expandLines,\n                    0,\n                    false,\n                ],\n                [`Show all ${limitSettings.method}`, Infinity, Infinity, true],\n                [\n                    `\u2193 Show ${expandLines} ${limitSettings.method}`,\n                    0,\n                    expandLines,\n                    false,\n                ],\n            ].map((b) => {\n                const [label, expandUp, expandDown, warnOnClick] = b;\n                const button = document.createElement('button');\n                button.innerText = label;\n                button.className = 'bp3-button jp-Button limit-output-button';\n                const cleanup = () => span.remove();\n                button.onclick = async () => {\n                    if (warnOnClick) {\n                        let warningLabel;\n                        if (limitSettings.method === 'lines') {\n                            let count = 0;\n                            for (let i = 0; i < options.source.length; ++i) {\n                                if (options.source[i] === '\\n') {\n                                    count++;\n                                }\n                            }\n                            if (count > WARN_BEFORE_EXPANDING_SOURCE_LENGTH_LINES) {\n                                warningLabel = `${count.toLocaleString()} lines`;\n                            }\n                        }\n                        else {\n                            if (options.source.length > WARN_BEFORE_EXPANDING_SOURCE_LENGTH_CH) {\n                                warningLabel = `${options.source.length.toLocaleString()} characters`;\n                            }\n                        }\n                        if (warningLabel) {\n                            const result = await apputils_1.showDialog({\n                                title: 'Show all',\n                                body: `Do you really want to show all ${warningLabel}?`,\n                            });\n                            if (!result.button.accept) {\n                                return;\n                            }\n                        }\n                    }\n                    // This binds the first clonedOptions call\n                    // i.e. future calls will updated clonedOptions but this onclick won't change\n                    clonedOptions.head += expandUp;\n                    clonedOptions.tail += expandDown;\n                    await limitOutputRenderText(Object.assign(Object.assign({}, options), { host: clonedOptions.host }), clonedOptions.head, clonedOptions.tail, cleanup);\n                    // Not the best design, but we know the prev element added is the renderText one\n                    // so we remove it before we redisplay\n                    clonedOptions.host.childNodes.forEach((n) => n.remove());\n                };\n                span.appendChild(button);\n            });\n            options.host.append(span);\n            // We are fully expanded!\n        }\n        else if (clonedOptions.source.length === options.source.length &&\n            _cleanupButtonFn) {\n            _cleanupButtonFn();\n        }\n        return ret;\n    }\n    return rendermime_1.renderText(options);\n};\nclass MyRenderedText extends rendermime_1.RenderedText {\n    /**\n     * Render a mime model.\n     *\n     * @param model - The mime model to render.\n     *\n     * @returns A promise which resolves when rendering is complete.\n     */\n    render(model) {\n        return limitOutputRenderText({\n            host: this.node,\n            sanitizer: this.sanitizer,\n            source: String(model.data[this.mimeType]),\n            translator: this.translator,\n        });\n    }\n}\nexports.MyRenderedText = MyRenderedText;\nexports.rendererFactory = {\n    safe: true,\n    mimeTypes: [\n        'text/plain',\n        'application/vnd.jupyter.stdout',\n        'application/vnd.jupyter.stderr',\n    ],\n    createRenderer: (options) => new MyRenderedText(options),\n};\n"
+        "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nconst rendermime_1 = require(\"@jupyterlab/rendermime\");\nconst settingregistry_1 = require(\"@jupyterlab/settingregistry\");\nconst renders_1 = require(\"./renders\");\nconst PLUGIN_NAME = 'jupyterlab-limit-output';\nconst extension = {\n    id: `${PLUGIN_NAME}:rendertext`,\n    rendererFactory: renders_1.rendererFactory,\n    // This number is NOT random. It's just lower (more preferred) than https://github.com/jupyterlab/jupyterlab/blob/0cbfcbe8c09d2c1fbfd1912f4d36c12479893946/packages/rendermime/src/factories.ts#L68\n    // Setting the rank too low makes the text version of renders too preferred (e.g. show text instead of the widget render)\n    rank: 119,\n    dataType: 'string',\n};\nconst RenderExtension = {\n    id: `${PLUGIN_NAME}:renders`,\n    autoStart: true,\n    requires: [rendermime_1.IRenderMimeRegistry, settingregistry_1.ISettingRegistry],\n    activate: function (app, rendermime, settingRegistry) {\n        // eslint-disable-next-line no-console\n        console.log('JupyterLab extension jupyterlab-limit-output is activated!');\n        rendermime.addFactory(extension.rendererFactory, extension.rank);\n        function updateSettings(settings) {\n            const head = settings.get('head').composite;\n            const tail = settings.get('tail').composite;\n            const enabled = settings.get('enabled').composite;\n            const method = settings.get('method')\n                .composite;\n            (0, renders_1.updateLimitOutputSettings)({ head, tail, method, enabled });\n        }\n        settingRegistry.load(`${PLUGIN_NAME}:settings`).then((settings) => {\n            updateSettings(settings);\n            settings.changed.connect(updateSettings);\n        }, (err) => {\n            console.error(`Could not load settings, so did not activate ${PLUGIN_NAME}: ${err}`);\n        });\n    },\n};\nexports.default = RenderExtension;\n",
+        "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.rendererFactory = exports.MyRenderedText = exports.updateLimitOutputSettings = void 0;\nconst rendermime_1 = require(\"@jupyterlab/rendermime\");\nconst formatters_1 = require(\"./formatters\");\nconst apputils_1 = require(\"@jupyterlab/apputils\");\nconst WARN_BEFORE_EXPANDING_SOURCE_LENGTH_CH = 100000;\nconst WARN_BEFORE_EXPANDING_SOURCE_LENGTH_LINES = 1000;\nlet limitSettings = {\n    head: 50,\n    tail: 50,\n    method: 'lines',\n    enabled: true,\n};\nconst updateLimitOutputSettings = (settings) => {\n    limitSettings = settings;\n    if (limitSettings.head < 0) {\n        limitSettings.head = 0;\n    }\n    if (limitSettings.tail < 0) {\n        limitSettings.tail = 0;\n    }\n    if (limitSettings.tail === 0 && limitSettings.head === 0) {\n        limitSettings.enabled = false;\n    }\n    if (limitSettings.method !== 'lines' &&\n        limitSettings.method !== 'characters') {\n        limitSettings.method = 'lines';\n    }\n};\nexports.updateLimitOutputSettings = updateLimitOutputSettings;\nconst limitOutputRenderText = async (options, _head = 0, _tail = 0, _cleanupButtonFn = null) => {\n    if (limitSettings.enabled) {\n        // We have to clone so that we can both keep track of number of head/tail\n        // shown as well as keep the original options unchanged\n        const clonedOptions = {\n            ...options,\n            head: _head || limitSettings.head,\n            tail: _tail || limitSettings.tail,\n        };\n        if (limitSettings.method === 'characters') {\n            clonedOptions.source = (0, formatters_1.limitByCharacters)(options.source, clonedOptions.head, clonedOptions.tail);\n        }\n        else {\n            clonedOptions.source = (0, formatters_1.limitByLines)(options.source, clonedOptions.head, clonedOptions.tail);\n        }\n        // Add a div so we can easily remove output\n        const div = document.createElement('div');\n        options.host.append(div);\n        clonedOptions.host = div;\n        // Wait for text to render so that we can add our buttons after it\n        const ret = await (0, rendermime_1.renderText)(clonedOptions);\n        // If we need to, add buttons for expanding output\n        if (_cleanupButtonFn === null &&\n            clonedOptions.source.length !== options.source.length) {\n            const expandLines = Math.max(limitSettings.tail, limitSettings.head);\n            const span = document.createElement('span');\n            [\n                // label, expand head, expand tail, warn on click\n                [\n                    `\u2191 Show ${expandLines} ${limitSettings.method}`,\n                    expandLines,\n                    0,\n                    false,\n                ],\n                [`Show all ${limitSettings.method}`, Infinity, Infinity, true],\n                [\n                    `\u2193 Show ${expandLines} ${limitSettings.method}`,\n                    0,\n                    expandLines,\n                    false,\n                ],\n            ].map((b) => {\n                const [label, expandUp, expandDown, warnOnClick] = b;\n                const button = document.createElement('button');\n                button.innerText = label;\n                button.className = 'bp3-button jp-Button limit-output-button';\n                const cleanup = () => span.remove();\n                button.onclick = async () => {\n                    if (warnOnClick) {\n                        let warningLabel;\n                        if (limitSettings.method === 'lines') {\n                            let count = 0;\n                            for (let i = 0; i < options.source.length; ++i) {\n                                if (options.source[i] === '\\n') {\n                                    count++;\n                                }\n                            }\n                            if (count > WARN_BEFORE_EXPANDING_SOURCE_LENGTH_LINES) {\n                                warningLabel = `${count.toLocaleString()} lines`;\n                            }\n                        }\n                        else {\n                            if (options.source.length > WARN_BEFORE_EXPANDING_SOURCE_LENGTH_CH) {\n                                warningLabel = `${options.source.length.toLocaleString()} characters`;\n                            }\n                        }\n                        if (warningLabel) {\n                            const result = await (0, apputils_1.showDialog)({\n                                title: 'Show all',\n                                body: `Do you really want to show all ${warningLabel}?`,\n                            });\n                            if (!result.button.accept) {\n                                return;\n                            }\n                        }\n                    }\n                    // This binds the first clonedOptions call\n                    // i.e. future calls will updated clonedOptions but this onclick won't change\n                    clonedOptions.head += expandUp;\n                    clonedOptions.tail += expandDown;\n                    await limitOutputRenderText({\n                        ...options,\n                        host: clonedOptions.host,\n                    }, clonedOptions.head, clonedOptions.tail, cleanup);\n                    // Not the best design, but we know the prev element added is the renderText one\n                    // so we remove it before we redisplay\n                    clonedOptions.host.childNodes.forEach((n) => n.remove());\n                };\n                span.appendChild(button);\n            });\n            options.host.append(span);\n            // We are fully expanded!\n        }\n        else if (clonedOptions.source.length === options.source.length &&\n            _cleanupButtonFn) {\n            _cleanupButtonFn();\n        }\n        return ret;\n    }\n    return (0, rendermime_1.renderText)(options);\n};\nclass MyRenderedText extends rendermime_1.RenderedText {\n    /**\n     * Render a mime model.\n     *\n     * @param model - The mime model to render.\n     *\n     * @returns A promise which resolves when rendering is complete.\n     */\n    render(model) {\n        return limitOutputRenderText({\n            host: this.node,\n            sanitizer: this.sanitizer,\n            source: String(model.data[this.mimeType]),\n            translator: this.translator,\n        });\n    }\n    /**\n     * Dispose the contents of node to contain potential memory leak.\n     *\n     * **Notes**: when user attempts to clean the output using context menu\n     * they invoke `JupyterFrontEnd.evtContextMenu` which caches the event\n     * to enable commands and extensions to access it later; this leads to\n     * a memory leak as the event holds the target node reference.\n     */\n    dispose() {\n        // TODO: remove ts-ignore during JupyterLab 4.0/TypeScript 5.0 migration\n        // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n        // @ts-ignore\n        this.node.replaceChildren();\n        super.dispose();\n    }\n}\nexports.MyRenderedText = MyRenderedText;\nexports.rendererFactory = {\n    safe: true,\n    mimeTypes: [\n        'text/plain',\n        'application/vnd.jupyter.stdout',\n        'application/vnd.jupyter.stderr',\n    ],\n    createRenderer: (options) => new MyRenderedText(options),\n};\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/lib_index_js.8f7e72224f999b4227c6.js.map` & `jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/style_index_js.8737596b5ac0bbefe59d.js.map`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7142857142857143%*

 * *Differences: {"'file'": "'style_index_js.8737596b5ac0bbefe59d.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;AAAA;AAC0G;AACjB;AACzF,8BAA8B,mFAA2B,CAAC,4FAAqC;AAC/F;AACA,gEAAgE,mDAAmD,mDAAmD,GAAG,gCAAgC,mDAAmD,GAAG,iCAAiC,mDAAmD,GAAG,SAAS,iFAAiF,YAAY,aAAa,OAAO,KAAK,YAAY,OAAO,KAAK,YAAY,gDAAgD,mDAAmD,mDAAmD,GAAG,gCAAgC,mDAAmD,GAAG,iCAAiC,mDAAmD,GAAG,qBAAqB;AACp1B;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;ACP1B;;AAEb;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,qDAAqD;AACrD;AACA;AACA,gDAAgD;AAChD;AACA;AACA,qFAAqF;AACrF;AACA […]*

```diff
@@ -1,17 +1,33 @@
 {
-    "file": "lib_index_js.8f7e72224f999b4227c6.js",
-    "mappings": ";;;;;;;;;AAAa;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,oBAAoB,GAAG,yBAAyB;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B,KAAK;AACjC;AACA;AACA,sBAAsB,oBAAoB,OAAO,KAAK;AACtD;AACA,kBAAkB,QAAQ,EAAE,mBAAmB,kCAAkC,KAAK,aAAa,mBAAmB,EAAE,QAAQ;AAChI;AACA;AACA;AACA,yBAAyB;AACzB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,+BAA+B;AAC/B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wBAAwB,KAAK;AAC7B;AACA;AACA,kBAAkB,oBAAoB,OAAO,KAAK;AAClD;AACA,cAAc,QAAQ,EAAE,mBAAmB,kCAAkC,KAAK,QAAQ,mBAAmB,EAAE,QAAQ;AACvH;AACA,oBAAoB;;;;;;;;;;;AC/EP;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,qBAAqB,mBAAO,CAAC,sFAAwB;AACrD,0BAA0B,mBAAO,CAAC,gGAA6B;AAC/D,kBAAkB,mBAAO,CAAC,mCAAW;AACrC;AACA;AACA,WAAW,YAAY;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA,WAAW,YAAY;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kDAAkD,6BAA6B;AAC/E;AACA,gCAAgC,YAAY;AAC5C;AACA;AACA,SAAS;AACT,0EAA0E,YAAY,IAAI,IAAI;AAC9F,SAAS;AACT,KAAK;AACL;AACA,kBAAe;;;;;;;;;;;ACtCF;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,uBAAuB,GAAG,sBAAsB,GAAG,iCAAiC;AACpF,qBAAqB,mBAAO,CAAC,sFAAwB;AACrD,qBAAqB,mBAAO,CAAC,yCAAc;AAC3C,mBAAmB,mBAAO,CAAC,kFAAsB;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC;AACjC;AACA;AACA;AACA;AACA,4DAA4D,cAAc,sEAAsE;AAChJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8BAA8B,aAAa,EAAE,qBAAqB;AAClE;AACA;AACA;AACA;AACA,6BAA6B,qBAAqB;AAClD;AACA,8BAA8B,aAAa,EAAE,qBAAqB;AAClE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4CAA4C,2BAA2B;AACvE;AACA;AACA;AACA;AACA;AACA,kDAAkD,wBAAwB;AAC1E;AACA;AACA;AACA;AACA,kDAAkD,wCAAwC;AAC1F;AACA;AACA;AACA;AACA;AACA,wEAAwE,aAAa;AACrF,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8EAA8E,cAAc,0BAA0B;AACtH;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,6DAA6D;AAC7D;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB;AACtB,uBAAuB;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA",
+    "file": "style_index_js.8737596b5ac0bbefe59d.js",
+    "mappings": ";;;;;;;;;;;;;;;;;AAAA;AAC0G;AACjB;AACzF,8BAA8B,mFAA2B,CAAC,4FAAqC;AAC/F;AACA,gEAAgE,mDAAmD,mDAAmD,GAAG,gCAAgC,mDAAmD,GAAG,iCAAiC,mDAAmD,GAAG,SAAS,iFAAiF,YAAY,aAAa,OAAO,KAAK,YAAY,OAAO,KAAK,YAAY,gDAAgD,mDAAmD,mDAAmD,GAAG,gCAAgC,mDAAmD,GAAG,iCAAiC,mDAAmD,GAAG,qBAAqB;AACp1B;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;ACP1B;;AAEb;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,qDAAqD;AACrD;AACA;AACA,gDAAgD;AAChD;AACA;AACA,qFAAqF;AACrF;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB;AACA;AACA,KAAK;AACL;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB,iBAAiB;AACvC;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB,qBAAqB;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,sFAAsF,qBAAqB;AAC3G;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,iDAAiD,qBAAqB;AACtE;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,sDAAsD,qBAAqB;AAC3E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACpFa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uDAAuD,cAAc;AACrE;AACA;AACA;AACA;AACA;;;;;;;;;;ACfa;;AAEb;AACA;AACA;AACA,kBAAkB,wBAAwB;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,iBAAiB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA;AACA;AACA,OAAO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,4BAA4B;AAChD;AACA;AACA;AACA;AACA;AACA,qBAAqB,6BAA6B;AAClD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACnFa;;AAEb;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ;AACR;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACjCa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACTa;;AAEb;AACA;AACA,cAAc,KAAwC,GAAG,sBAAiB,GAAG,CAAI;AACjF;AACA;AACA;AACA;AACA;;;;;;;;;;ACTa;;AAEb;AACA;AACA;AACA;AACA,kDAAkD;AAClD;AACA;AACA,0CAA0C;AAC1C;AACA;AACA;AACA,iFAAiF;AACjF;AACA;AACA;AACA,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA;AACA,yDAAyD;AACzD;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,kCAAkC;AAClC;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;AC5Da;;AAEb;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;ACboB;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACCpB,MAA+F;AAC/F,MAAqF;AACrF,MAA4F;AAC5F,MAA+G;AAC/G,MAAwG;AACxG,MAAwG;AACxG,MAAkG;AAClG;AACA;;AAEA;;AAEA,4BAA4B,qGAAmB;AAC/C,wBAAwB,kHAAa;;AAErC,uBAAuB,uGAAa;AACpC;AACA,iBAAiB,+FAAM;AACvB,6BAA6B,sGAAkB;;AAE/C,aAAa,0GAAG,CAAC,qFAAO;;;;AAI4C;AACpE,OAAO,iEAAe,qFAAO,IAAI,4FAAc,GAAG,4FAAc,YAAY,EAAC",
     "names": [],
     "sourceRoot": "",
     "sources": [
-        "webpack://jupyterlab-limit-output/./lib/formatters.js",
-        "webpack://jupyterlab-limit-output/./lib/index.js",
-        "webpack://jupyterlab-limit-output/./lib/renders.js"
+        "webpack://jupyterlab-limit-output/./style/base.css",
+        "webpack://jupyterlab-limit-output/./node_modules/css-loader/dist/runtime/api.js",
+        "webpack://jupyterlab-limit-output/./node_modules/css-loader/dist/runtime/sourceMaps.js",
+        "webpack://jupyterlab-limit-output/./node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js",
+        "webpack://jupyterlab-limit-output/./node_modules/style-loader/dist/runtime/insertBySelector.js",
+        "webpack://jupyterlab-limit-output/./node_modules/style-loader/dist/runtime/insertStyleElement.js",
+        "webpack://jupyterlab-limit-output/./node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js",
+        "webpack://jupyterlab-limit-output/./node_modules/style-loader/dist/runtime/styleDomAPI.js",
+        "webpack://jupyterlab-limit-output/./node_modules/style-loader/dist/runtime/styleTagTransform.js",
+        "webpack://jupyterlab-limit-output/./style/index.js",
+        "webpack://jupyterlab-limit-output/./style/base.css?1944"
     ],
     "sourcesContent": [
-        "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.limitByLines = exports.limitByCharacters = void 0;\nconst NEW_LINE = '\\n';\nconst SPACER = '\\n\\n\\n';\n/**\n * Return a string with at most head starting characters and tail ending (plus a warning)\n */\nconst limitByCharacters = (text, head, tail) => {\n    const maxChars = head + tail;\n    if (text.length > maxChars) {\n        const headstr = text.substring(0, head);\n        const tailstr = text.substring(text.length - tail);\n        let msg = '';\n        if (head) {\n            msg = ` first ${head}`;\n        }\n        if (tail) {\n            msg += `${head ? ' and' : ''} last ${tail}`;\n        }\n        return `${headstr}${head ? SPACER : ''}WARNING: Output limited. Showing${msg} characters.${tail ? SPACER : ''}${tailstr}`;\n    }\n    return text;\n};\nexports.limitByCharacters = limitByCharacters;\n/**\n * Find the nth index of the newline character\n */\nfunction _nthNewLineIndex(text, n) {\n    let idx = 0;\n    while (n-- > 0 && idx++ < text.length) {\n        idx = text.indexOf(NEW_LINE, idx);\n        // Not found before we ran out of n\n        if (idx < 0) {\n            return null;\n        }\n    }\n    return idx;\n}\n/**\n * Find the nth newline from the end of the string (excluding a possible final new line)\n */\nfunction _nthNewLineFromLastIndex(text, n) {\n    let idx = text.length - 1; // Ignore a possible final trailing \\n\n    while (n-- > 0 && idx-- >= 0) {\n        idx = text.lastIndexOf(NEW_LINE, idx);\n        // Not found before we ran out of n\n        if (idx < 0) {\n            return null;\n        }\n    }\n    return idx;\n}\n/**\n * Return a string with at most head starting lines and tail ending (plus a warning)\n */\nconst limitByLines = (text, head, tail) => {\n    const headEndPos = head > 0 ? _nthNewLineIndex(text, head) : -1;\n    if (headEndPos === null) {\n        return text;\n    }\n    const tailStartPos = tail > 0 ? _nthNewLineFromLastIndex(text, tail) : text.length;\n    if (tailStartPos === null) {\n        return text;\n    }\n    if (tailStartPos <= headEndPos) {\n        return text;\n    }\n    const headstr = text.substring(0, headEndPos);\n    const tailstr = text.substring(tailStartPos);\n    let msg = '';\n    if (head) {\n        msg = ` first ${head}`;\n    }\n    if (tail) {\n        msg += `${head ? ' and' : ''} last ${tail}`;\n    }\n    return `${headstr}${head ? SPACER : ''}WARNING: Output limited. Showing${msg} lines.${tail ? SPACER : ''}${tailstr}`;\n};\nexports.limitByLines = limitByLines;\n",
-        "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nconst rendermime_1 = require(\"@jupyterlab/rendermime\");\nconst settingregistry_1 = require(\"@jupyterlab/settingregistry\");\nconst renders_1 = require(\"./renders\");\nconst PLUGIN_NAME = 'jupyterlab-limit-output';\nconst extension = {\n    id: `${PLUGIN_NAME}:rendertext`,\n    rendererFactory: renders_1.rendererFactory,\n    // This number is NOT random. It's just lower (more preferred) than https://github.com/jupyterlab/jupyterlab/blob/0cbfcbe8c09d2c1fbfd1912f4d36c12479893946/packages/rendermime/src/factories.ts#L68\n    // Setting the rank too low makes the text version of renders too preferred (e.g. show text instead of the widget render)\n    rank: 119,\n    dataType: 'string',\n};\nconst RenderExtension = {\n    id: `${PLUGIN_NAME}:renders`,\n    autoStart: true,\n    requires: [rendermime_1.IRenderMimeRegistry, settingregistry_1.ISettingRegistry],\n    activate: function (app, rendermime, settingRegistry) {\n        // eslint-disable-next-line no-console\n        console.log('JupyterLab extension jupyterlab-limit-output is activated!');\n        rendermime.addFactory(extension.rendererFactory, extension.rank);\n        function updateSettings(settings) {\n            const head = settings.get('head').composite;\n            const tail = settings.get('tail').composite;\n            const enabled = settings.get('enabled').composite;\n            const method = settings.get('method')\n                .composite;\n            renders_1.updateLimitOutputSettings({ head, tail, method, enabled });\n        }\n        settingRegistry.load(`${PLUGIN_NAME}:settings`).then((settings) => {\n            updateSettings(settings);\n            settings.changed.connect(updateSettings);\n        }, (err) => {\n            console.error(`Could not load settings, so did not activate ${PLUGIN_NAME}: ${err}`);\n        });\n    },\n};\nexports.default = RenderExtension;\n",
-        "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.rendererFactory = exports.MyRenderedText = exports.updateLimitOutputSettings = void 0;\nconst rendermime_1 = require(\"@jupyterlab/rendermime\");\nconst formatters_1 = require(\"./formatters\");\nconst apputils_1 = require(\"@jupyterlab/apputils\");\nconst WARN_BEFORE_EXPANDING_SOURCE_LENGTH_CH = 100000;\nconst WARN_BEFORE_EXPANDING_SOURCE_LENGTH_LINES = 1000;\nlet limitSettings = {\n    head: 50,\n    tail: 50,\n    method: 'lines',\n    enabled: true,\n};\nconst updateLimitOutputSettings = (settings) => {\n    limitSettings = settings;\n    if (limitSettings.head < 0) {\n        limitSettings.head = 0;\n    }\n    if (limitSettings.tail < 0) {\n        limitSettings.tail = 0;\n    }\n    if (limitSettings.tail === 0 && limitSettings.head === 0) {\n        limitSettings.enabled = false;\n    }\n    if (limitSettings.method !== 'lines' &&\n        limitSettings.method !== 'characters') {\n        limitSettings.method = 'lines';\n    }\n};\nexports.updateLimitOutputSettings = updateLimitOutputSettings;\nconst limitOutputRenderText = async (options, _head = 0, _tail = 0, _cleanupButtonFn = null) => {\n    if (limitSettings.enabled) {\n        // We have to clone so that we can both keep track of number of head/tail\n        // shown as well as keep the original options unchanged\n        const clonedOptions = Object.assign(Object.assign({}, options), { head: _head || limitSettings.head, tail: _tail || limitSettings.tail });\n        if (limitSettings.method === 'characters') {\n            clonedOptions.source = formatters_1.limitByCharacters(options.source, clonedOptions.head, clonedOptions.tail);\n        }\n        else {\n            clonedOptions.source = formatters_1.limitByLines(options.source, clonedOptions.head, clonedOptions.tail);\n        }\n        // Add a div so we can easily remove output\n        const div = document.createElement('div');\n        options.host.append(div);\n        clonedOptions.host = div;\n        // Wait for text to render so that we can add our buttons after it\n        const ret = await rendermime_1.renderText(clonedOptions);\n        // If we need to, add buttons for expanding output\n        if (_cleanupButtonFn === null &&\n            clonedOptions.source.length !== options.source.length) {\n            const expandLines = Math.max(limitSettings.tail, limitSettings.head);\n            const span = document.createElement('span');\n            [\n                // label, expand head, expand tail, warn on click\n                [\n                    `\u2191 Show ${expandLines} ${limitSettings.method}`,\n                    expandLines,\n                    0,\n                    false,\n                ],\n                [`Show all ${limitSettings.method}`, Infinity, Infinity, true],\n                [\n                    `\u2193 Show ${expandLines} ${limitSettings.method}`,\n                    0,\n                    expandLines,\n                    false,\n                ],\n            ].map((b) => {\n                const [label, expandUp, expandDown, warnOnClick] = b;\n                const button = document.createElement('button');\n                button.innerText = label;\n                button.className = 'bp3-button jp-Button limit-output-button';\n                const cleanup = () => span.remove();\n                button.onclick = async () => {\n                    if (warnOnClick) {\n                        let warningLabel;\n                        if (limitSettings.method === 'lines') {\n                            let count = 0;\n                            for (let i = 0; i < options.source.length; ++i) {\n                                if (options.source[i] === '\\n') {\n                                    count++;\n                                }\n                            }\n                            if (count > WARN_BEFORE_EXPANDING_SOURCE_LENGTH_LINES) {\n                                warningLabel = `${count.toLocaleString()} lines`;\n                            }\n                        }\n                        else {\n                            if (options.source.length > WARN_BEFORE_EXPANDING_SOURCE_LENGTH_CH) {\n                                warningLabel = `${options.source.length.toLocaleString()} characters`;\n                            }\n                        }\n                        if (warningLabel) {\n                            const result = await apputils_1.showDialog({\n                                title: 'Show all',\n                                body: `Do you really want to show all ${warningLabel}?`,\n                            });\n                            if (!result.button.accept) {\n                                return;\n                            }\n                        }\n                    }\n                    // This binds the first clonedOptions call\n                    // i.e. future calls will updated clonedOptions but this onclick won't change\n                    clonedOptions.head += expandUp;\n                    clonedOptions.tail += expandDown;\n                    await limitOutputRenderText(Object.assign(Object.assign({}, options), { host: clonedOptions.host }), clonedOptions.head, clonedOptions.tail, cleanup);\n                    // Not the best design, but we know the prev element added is the renderText one\n                    // so we remove it before we redisplay\n                    clonedOptions.host.childNodes.forEach((n) => n.remove());\n                };\n                span.appendChild(button);\n            });\n            options.host.append(span);\n            // We are fully expanded!\n        }\n        else if (clonedOptions.source.length === options.source.length &&\n            _cleanupButtonFn) {\n            _cleanupButtonFn();\n        }\n        return ret;\n    }\n    return rendermime_1.renderText(options);\n};\nclass MyRenderedText extends rendermime_1.RenderedText {\n    /**\n     * Render a mime model.\n     *\n     * @param model - The mime model to render.\n     *\n     * @returns A promise which resolves when rendering is complete.\n     */\n    render(model) {\n        return limitOutputRenderText({\n            host: this.node,\n            sanitizer: this.sanitizer,\n            source: String(model.data[this.mimeType]),\n            translator: this.translator,\n        });\n    }\n    /**\n     * Dispose the contents of node to contain potential memory leak.\n     *\n     * **Notes**: when user attempts to clean the output using context menu\n     * they invoke `JupyterFrontEnd.evtContextMenu` which caches the event\n     * to enable commands and extensions to access it later; this leads to\n     * a memory leak as the event holds the target node reference.\n     */\n    dispose() {\n        // TODO: remove ts-ignore during JupyterLab 4.0/TypeScript 5.0 migration\n        // @ts-ignore\n        this.node.replaceChildren();\n        super.dispose();\n    }\n}\nexports.MyRenderedText = MyRenderedText;\nexports.rendererFactory = {\n    safe: true,\n    mimeTypes: [\n        'text/plain',\n        'application/vnd.jupyter.stdout',\n        'application/vnd.jupyter.stderr',\n    ],\n    createRenderer: (options) => new MyRenderedText(options),\n};\n"
+        "// Imports\nimport ___CSS_LOADER_API_SOURCEMAP_IMPORT___ from \"../node_modules/css-loader/dist/runtime/sourceMaps.js\";\nimport ___CSS_LOADER_API_IMPORT___ from \"../node_modules/css-loader/dist/runtime/api.js\";\nvar ___CSS_LOADER_EXPORT___ = ___CSS_LOADER_API_IMPORT___(___CSS_LOADER_API_SOURCEMAP_IMPORT___);\n// Module\n___CSS_LOADER_EXPORT___.push([module.id, \".limit-output-button {\\n  color: var(--jp-content-link-color) !important;\\n  background: var(--jp-layout-color1) !important;\\n}\\n\\n.limit-output-button:hover {\\n  background: var(--jp-layout-color2) !important;\\n}\\n\\n.limit-output-button:active {\\n  background: var(--jp-layout-color3) !important;\\n}\\n\", \"\",{\"version\":3,\"sources\":[\"webpack://./style/base.css\"],\"names\":[],\"mappings\":\"AAAA;EACE,8CAA8C;EAC9C,8CAA8C;AAChD;;AAEA;EACE,8CAA8C;AAChD;;AAEA;EACE,8CAA8C;AAChD\",\"sourcesContent\":[\".limit-output-button {\\n  color: var(--jp-content-link-color) !important;\\n  background: var(--jp-layout-color1) !important;\\n}\\n\\n.limit-output-button:hover {\\n  background: var(--jp-layout-color2) !important;\\n}\\n\\n.limit-output-button:active {\\n  background: var(--jp-layout-color3) !important;\\n}\\n\"],\"sourceRoot\":\"\"}]);\n// Exports\nexport default ___CSS_LOADER_EXPORT___;\n",
+        "\"use strict\";\n\n/*\n  MIT License http://www.opensource.org/licenses/mit-license.php\n  Author Tobias Koppers @sokra\n*/\nmodule.exports = function (cssWithMappingToString) {\n  var list = [];\n\n  // return the list of modules as css string\n  list.toString = function toString() {\n    return this.map(function (item) {\n      var content = \"\";\n      var needLayer = typeof item[5] !== \"undefined\";\n      if (item[4]) {\n        content += \"@supports (\".concat(item[4], \") {\");\n      }\n      if (item[2]) {\n        content += \"@media \".concat(item[2], \" {\");\n      }\n      if (needLayer) {\n        content += \"@layer\".concat(item[5].length > 0 ? \" \".concat(item[5]) : \"\", \" {\");\n      }\n      content += cssWithMappingToString(item);\n      if (needLayer) {\n        content += \"}\";\n      }\n      if (item[2]) {\n        content += \"}\";\n      }\n      if (item[4]) {\n        content += \"}\";\n      }\n      return content;\n    }).join(\"\");\n  };\n\n  // import a list of modules into the list\n  list.i = function i(modules, media, dedupe, supports, layer) {\n    if (typeof modules === \"string\") {\n      modules = [[null, modules, undefined]];\n    }\n    var alreadyImportedModules = {};\n    if (dedupe) {\n      for (var k = 0; k < this.length; k++) {\n        var id = this[k][0];\n        if (id != null) {\n          alreadyImportedModules[id] = true;\n        }\n      }\n    }\n    for (var _k = 0; _k < modules.length; _k++) {\n      var item = [].concat(modules[_k]);\n      if (dedupe && alreadyImportedModules[item[0]]) {\n        continue;\n      }\n      if (typeof layer !== \"undefined\") {\n        if (typeof item[5] === \"undefined\") {\n          item[5] = layer;\n        } else {\n          item[1] = \"@layer\".concat(item[5].length > 0 ? \" \".concat(item[5]) : \"\", \" {\").concat(item[1], \"}\");\n          item[5] = layer;\n        }\n      }\n      if (media) {\n        if (!item[2]) {\n          item[2] = media;\n        } else {\n          item[1] = \"@media \".concat(item[2], \" {\").concat(item[1], \"}\");\n          item[2] = media;\n        }\n      }\n      if (supports) {\n        if (!item[4]) {\n          item[4] = \"\".concat(supports);\n        } else {\n          item[1] = \"@supports (\".concat(item[4], \") {\").concat(item[1], \"}\");\n          item[4] = supports;\n        }\n      }\n      list.push(item);\n    }\n  };\n  return list;\n};",
+        "\"use strict\";\n\nmodule.exports = function (item) {\n  var content = item[1];\n  var cssMapping = item[3];\n  if (!cssMapping) {\n    return content;\n  }\n  if (typeof btoa === \"function\") {\n    var base64 = btoa(unescape(encodeURIComponent(JSON.stringify(cssMapping))));\n    var data = \"sourceMappingURL=data:application/json;charset=utf-8;base64,\".concat(base64);\n    var sourceMapping = \"/*# \".concat(data, \" */\");\n    return [content].concat([sourceMapping]).join(\"\\n\");\n  }\n  return [content].join(\"\\n\");\n};",
+        "\"use strict\";\n\nvar stylesInDOM = [];\nfunction getIndexByIdentifier(identifier) {\n  var result = -1;\n  for (var i = 0; i < stylesInDOM.length; i++) {\n    if (stylesInDOM[i].identifier === identifier) {\n      result = i;\n      break;\n    }\n  }\n  return result;\n}\nfunction modulesToDom(list, options) {\n  var idCountMap = {};\n  var identifiers = [];\n  for (var i = 0; i < list.length; i++) {\n    var item = list[i];\n    var id = options.base ? item[0] + options.base : item[0];\n    var count = idCountMap[id] || 0;\n    var identifier = \"\".concat(id, \" \").concat(count);\n    idCountMap[id] = count + 1;\n    var indexByIdentifier = getIndexByIdentifier(identifier);\n    var obj = {\n      css: item[1],\n      media: item[2],\n      sourceMap: item[3],\n      supports: item[4],\n      layer: item[5]\n    };\n    if (indexByIdentifier !== -1) {\n      stylesInDOM[indexByIdentifier].references++;\n      stylesInDOM[indexByIdentifier].updater(obj);\n    } else {\n      var updater = addElementStyle(obj, options);\n      options.byIndex = i;\n      stylesInDOM.splice(i, 0, {\n        identifier: identifier,\n        updater: updater,\n        references: 1\n      });\n    }\n    identifiers.push(identifier);\n  }\n  return identifiers;\n}\nfunction addElementStyle(obj, options) {\n  var api = options.domAPI(options);\n  api.update(obj);\n  var updater = function updater(newObj) {\n    if (newObj) {\n      if (newObj.css === obj.css && newObj.media === obj.media && newObj.sourceMap === obj.sourceMap && newObj.supports === obj.supports && newObj.layer === obj.layer) {\n        return;\n      }\n      api.update(obj = newObj);\n    } else {\n      api.remove();\n    }\n  };\n  return updater;\n}\nmodule.exports = function (list, options) {\n  options = options || {};\n  list = list || [];\n  var lastIdentifiers = modulesToDom(list, options);\n  return function update(newList) {\n    newList = newList || [];\n    for (var i = 0; i < lastIdentifiers.length; i++) {\n      var identifier = lastIdentifiers[i];\n      var index = getIndexByIdentifier(identifier);\n      stylesInDOM[index].references--;\n    }\n    var newLastIdentifiers = modulesToDom(newList, options);\n    for (var _i = 0; _i < lastIdentifiers.length; _i++) {\n      var _identifier = lastIdentifiers[_i];\n      var _index = getIndexByIdentifier(_identifier);\n      if (stylesInDOM[_index].references === 0) {\n        stylesInDOM[_index].updater();\n        stylesInDOM.splice(_index, 1);\n      }\n    }\n    lastIdentifiers = newLastIdentifiers;\n  };\n};",
+        "\"use strict\";\n\nvar memo = {};\n\n/* istanbul ignore next  */\nfunction getTarget(target) {\n  if (typeof memo[target] === \"undefined\") {\n    var styleTarget = document.querySelector(target);\n\n    // Special case to return head of iframe instead of iframe itself\n    if (window.HTMLIFrameElement && styleTarget instanceof window.HTMLIFrameElement) {\n      try {\n        // This will throw an exception if access to iframe is blocked\n        // due to cross-origin restrictions\n        styleTarget = styleTarget.contentDocument.head;\n      } catch (e) {\n        // istanbul ignore next\n        styleTarget = null;\n      }\n    }\n    memo[target] = styleTarget;\n  }\n  return memo[target];\n}\n\n/* istanbul ignore next  */\nfunction insertBySelector(insert, style) {\n  var target = getTarget(insert);\n  if (!target) {\n    throw new Error(\"Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.\");\n  }\n  target.appendChild(style);\n}\nmodule.exports = insertBySelector;",
+        "\"use strict\";\n\n/* istanbul ignore next  */\nfunction insertStyleElement(options) {\n  var element = document.createElement(\"style\");\n  options.setAttributes(element, options.attributes);\n  options.insert(element, options.options);\n  return element;\n}\nmodule.exports = insertStyleElement;",
+        "\"use strict\";\n\n/* istanbul ignore next  */\nfunction setAttributesWithoutAttributes(styleElement) {\n  var nonce = typeof __webpack_nonce__ !== \"undefined\" ? __webpack_nonce__ : null;\n  if (nonce) {\n    styleElement.setAttribute(\"nonce\", nonce);\n  }\n}\nmodule.exports = setAttributesWithoutAttributes;",
+        "\"use strict\";\n\n/* istanbul ignore next  */\nfunction apply(styleElement, options, obj) {\n  var css = \"\";\n  if (obj.supports) {\n    css += \"@supports (\".concat(obj.supports, \") {\");\n  }\n  if (obj.media) {\n    css += \"@media \".concat(obj.media, \" {\");\n  }\n  var needLayer = typeof obj.layer !== \"undefined\";\n  if (needLayer) {\n    css += \"@layer\".concat(obj.layer.length > 0 ? \" \".concat(obj.layer) : \"\", \" {\");\n  }\n  css += obj.css;\n  if (needLayer) {\n    css += \"}\";\n  }\n  if (obj.media) {\n    css += \"}\";\n  }\n  if (obj.supports) {\n    css += \"}\";\n  }\n  var sourceMap = obj.sourceMap;\n  if (sourceMap && typeof btoa !== \"undefined\") {\n    css += \"\\n/*# sourceMappingURL=data:application/json;base64,\".concat(btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap)))), \" */\");\n  }\n\n  // For old IE\n  /* istanbul ignore if  */\n  options.styleTagTransform(css, styleElement, options.options);\n}\nfunction removeStyleElement(styleElement) {\n  // istanbul ignore if\n  if (styleElement.parentNode === null) {\n    return false;\n  }\n  styleElement.parentNode.removeChild(styleElement);\n}\n\n/* istanbul ignore next  */\nfunction domAPI(options) {\n  if (typeof document === \"undefined\") {\n    return {\n      update: function update() {},\n      remove: function remove() {}\n    };\n  }\n  var styleElement = options.insertStyleElement(options);\n  return {\n    update: function update(obj) {\n      apply(styleElement, options, obj);\n    },\n    remove: function remove() {\n      removeStyleElement(styleElement);\n    }\n  };\n}\nmodule.exports = domAPI;",
+        "\"use strict\";\n\n/* istanbul ignore next  */\nfunction styleTagTransform(css, styleElement) {\n  if (styleElement.styleSheet) {\n    styleElement.styleSheet.cssText = css;\n  } else {\n    while (styleElement.firstChild) {\n      styleElement.removeChild(styleElement.firstChild);\n    }\n    styleElement.appendChild(document.createTextNode(css));\n  }\n}\nmodule.exports = styleTagTransform;",
+        "import './base.css';\n",
+        "\n      import API from \"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\";\n      import domAPI from \"!../node_modules/style-loader/dist/runtime/styleDomAPI.js\";\n      import insertFn from \"!../node_modules/style-loader/dist/runtime/insertBySelector.js\";\n      import setAttributes from \"!../node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js\";\n      import insertStyleElement from \"!../node_modules/style-loader/dist/runtime/insertStyleElement.js\";\n      import styleTagTransformFn from \"!../node_modules/style-loader/dist/runtime/styleTagTransform.js\";\n      import content, * as namedExport from \"!!../node_modules/css-loader/dist/cjs.js!./base.css\";\n      \n      \n\nvar options = {};\n\noptions.styleTagTransform = styleTagTransformFn;\noptions.setAttributes = setAttributes;\n\n      options.insert = insertFn.bind(null, \"head\");\n    \noptions.domAPI = domAPI;\noptions.insertStyleElement = insertStyleElement;\n\nvar update = API(content, options);\n\n\n\nexport * from \"!!../node_modules/css-loader/dist/cjs.js!./base.css\";\n       export default content && content.locals ? content.locals : undefined;\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/remoteEntry.03e3d8532caa3afb5cc7.js` & `jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/remoteEntry.d8030784757a1c70623e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
                     "./index": () => {
                         return __webpack_require__.e("lib_index_js").then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./extension": () => {
                         return __webpack_require__.e("lib_index_js").then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./style": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("style_index_js")]).then(() => (() => ((__webpack_require__( /*! ./style/index.js */ "./style/index.js")))));
+                        return __webpack_require__.e("style_index_js").then(() => (() => ((__webpack_require__( /*! ./style/index.js */ "./style/index.js")))));
                     }
                 };
                 var get = (module, getScope) => {
                     __webpack_require__.R = getScope;
                     getScope = (
                         __webpack_require__.o(moduleMap, module) ?
                         moduleMap[module]() :
@@ -182,17 +182,16 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "8f7e72224f999b4227c6",
-                "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "4806e8ff31b66ffc0443",
-                "style_index_js": "a8027a2cb024ffc2c646"
+                "lib_index_js": "ffe2091edae0050147bf",
+                "style_index_js": "8737596b5ac0bbefe59d"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
     /******/
@@ -303,16 +302,14 @@
                 /******/
                 doneFns && doneFns.forEach((fn) => (fn(event)));
                 /******/
                 if (prev) return prev(event);
                 /******/
             }
             /******/
-            ;
-            /******/
             var timeout = setTimeout(onScriptComplete.bind(null, undefined, {
                 type: 'timeout',
                 target: script
             }), 120000);
             /******/
             script.onerror = onScriptComplete.bind(null, script.onerror);
             /******/
@@ -425,15 +422,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab-limit-output", "1.0.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab-limit-output", "2.0.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -456,15 +453,15 @@
         /******/
         var document = __webpack_require__.g.document;
         /******/
         if (!scriptUrl && document) {
             /******/
             if (document.currentScript)
                 /******/
-                scriptUrl = document.currentScript.src
+                scriptUrl = document.currentScript.src;
             /******/
             if (!scriptUrl) {
                 /******/
                 var scripts = document.getElementsByTagName("script");
                 /******/
                 if (scripts.length) scriptUrl = scripts[scripts.length - 1].src
                 /******/
@@ -814,19 +811,19 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/rendermime": () => (loadSingletonVersionCheck("default", "@jupyterlab/rendermime", [1, 3, 6, 2])),
+            "webpack/sharing/consume/default/@jupyterlab/rendermime": () => (loadSingletonVersionCheck("default", "@jupyterlab/rendermime", [1, 4, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 3, 6, 2])),
+            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 4, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 2]))
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 0, 0]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
@@ -1045,20 +1042,29 @@
         /******/
         chunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));
         /******/
         chunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));
         /******/
     })();
     /******/
+    /******/
+    /* webpack/runtime/nonce */
+    /******/
+    (() => {
+        /******/
+        __webpack_require__.nc = undefined;
+        /******/
+    })();
+    /******/
     /************************************************************************/
     /******/
     /******/ // module cache are used so entry inlining is disabled
     /******/ // startup
     /******/ // Load entry module and return exports
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-limit-output");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-limit-output"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.03e3d8532caa3afb5cc7.js.map
+//# sourceMappingURL=remoteEntry.d8030784757a1c70623e.js.map
```

### Comparing `jupyterlab_limit_output-1.0.1/jupyterlab_limit_output/labextension/static/remoteEntry.03e3d8532caa3afb5cc7.js.map` & `jupyterlab_limit_output-2.0.0/jupyterlab_limit_output/labextension/static/remoteEntry.d8030784757a1c70623e.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8144841269841271%*

 * *Differences: {"'file'": "'remoteEntry.d8030784757a1c70623e.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.03e3d8532caa3afb5cc7.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC3KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;UErFA;UACA;UACA;UACA",
+    "file": "remoteEntry.d8030784757a1c70623e.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC3KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-limit-output/webpack/container-entry",
         "webpack://jupyterlab-limit-output/webpack/bootstrap",
         "webpack://jupyterlab-limit-output/webpack/runtime/compat get default export",
         "webpack://jupyterlab-limit-output/webpack/runtime/define property getters",
@@ -14,32 +14,34 @@
         "webpack://jupyterlab-limit-output/webpack/runtime/hasOwnProperty shorthand",
         "webpack://jupyterlab-limit-output/webpack/runtime/load script",
         "webpack://jupyterlab-limit-output/webpack/runtime/make namespace object",
         "webpack://jupyterlab-limit-output/webpack/runtime/sharing",
         "webpack://jupyterlab-limit-output/webpack/runtime/publicPath",
         "webpack://jupyterlab-limit-output/webpack/runtime/consumes",
         "webpack://jupyterlab-limit-output/webpack/runtime/jsonp chunk loading",
+        "webpack://jupyterlab-limit-output/webpack/runtime/nonce",
         "webpack://jupyterlab-limit-output/webpack/before-startup",
         "webpack://jupyterlab-limit-output/webpack/startup",
         "webpack://jupyterlab-limit-output/webpack/after-startup"
     ],
     "sourcesContent": [
-        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
+        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"8f7e72224f999b4227c6\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"4806e8ff31b66ffc0443\",\"style_index_js\":\"a8027a2cb024ffc2c646\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"ffe2091edae0050147bf\",\"style_index_js\":\"8737596b5ac0bbefe59d\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
-        "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-limit-output:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
+        "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-limit-output:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab-limit-output\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-limit-output\", \"1.0.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
-        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/rendermime\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/rendermime\", [1,3,6,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,2]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/rendermime\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab-limit-output\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-limit-output\", \"2.0.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/rendermime\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/rendermime\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,0,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/rendermime\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-limit-output\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_limit_output\"] = self[\"webpackChunkjupyterlab_limit_output\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-limit-output\");\n",
         ""
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_limit_output-1.0.1/jupyterlab_limit_output.egg-info/PKG-INFO` & `jupyterlab_limit_output-2.0.0/jupyterlab_limit_output.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: jupyterlab-limit-output
-Version: 1.0.1
+Version: 2.0.0
 Summary: Limit output text mime-renders
 Home-page: https://github.com/deshaw/jupyterlab-limit-output
 Author: Marc Udoff
 License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
+Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # jupyterlab-limit-output
 
 [![PyPI version][pypi-image]][pypi-url] [![PyPI DM][pypi-dm-image]][pypi-url]
 [![Github Actions Status][github-status-image]][github-status-url] [![Binder][binder-image]][binder-url]
@@ -107,15 +111,16 @@
 git tag vX.Z.Y
 git push && git push --tags
 ```
 
 3. Create the artifacts
 
 ```
-rm -rf dist
+rm -rf dist jupyterlab_limit_output/labextension
+jlpm run build
 python setup.py sdist bdist_wheel
 ```
 
 4. Test this against the test pypi. You can then install from here to test as well:
 
 ```
 twine upload --repository-url https://test.pypi.org/legacy/ dist/*
```

### Comparing `jupyterlab_limit_output-1.0.1/package.json` & `jupyterlab_limit_output-2.0.0/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8911549707602339%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.0', '@jupyterlab/rendermime': '^4.0.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@types/chai': '^4.3.4', '@types/mocha': "*

 * *                      "'^10.0.1', '@typescript-eslint/eslint-plugin': '^5.55.0', "*

 * *                      "'@typescript-eslint/parser': '^5.55.0', 'chai': '^4.3.7', "*

 * *                      "'eslint-config-prettier': '^8. […]*

```diff
@@ -1,51 +1,46 @@
 {
     "bugs": {
         "url": "https://github.com/deshaw/jupyterlab-limit-output/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/rendermime": "^3.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/rendermime": "^4.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
     "description": "Limit output text mime-renders",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.12",
-        "@types/chai": "^4.2.22",
-        "@types/mocha": "^9.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.32.0",
-        "@typescript-eslint/parser": "^4.32.0",
-        "chai": "^4.3.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/chai": "^4.3.4",
+        "@types/mocha": "^10.0.1",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "chai": "^4.3.7",
         "eslint": "^7.32.0",
-        "eslint-config-prettier": "^8.3.0",
-        "eslint-plugin-prettier": "^4.0.0",
-        "husky": "^4.2.3",
-        "mocha": "^9.1.2",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "husky": "^8.0.0",
+        "mocha": "^10.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.4.1",
-        "rimraf": "^3.0.2",
-        "ts-mocha": "^8.0.0",
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "ts-mocha": "^10.0.0",
         "tslint": "^6.1.3",
         "tslint-config-prettier": "^1.18.0",
         "tslint-plugin-prettier": "^2.3.0",
-        "typescript": "~4.1.3"
+        "typescript": "~5.0.2"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-limit-output",
-    "husky": {
-        "hooks": {
-            "pre-commit": "npm run lint && npm run test"
-        }
-    },
     "jupyterlab": {
         "extension": true,
         "outputDir": "jupyterlab_limit_output/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
@@ -70,23 +65,23 @@
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
         "clean:labextension": "rimraf jupyterlab_limit_output/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "eslint . --ext .ts,.tsx --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "install:extension": "jlpm run build",
         "lint": "npm run prettier && npm run tslint",
-        "prepare": "jlpm run clean && jlpm run build:prod",
+        "prepare": "jlpm run clean && jlpm run build:prod && husky install",
         "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "ts-mocha -p tests/tsconfig.json tests/**/*_spec.ts",
         "tslint": "tslint --fix -c tslint.json --project tsconfig.json '**/*{.ts,.tsx}'",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter-labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "2.0.0"
 }
```

### Comparing `jupyterlab_limit_output-1.0.1/setup.py` & `jupyterlab_limit_output-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,35 +36,39 @@
     version=pkg_json["version"],
     url=pkg_json["homepage"],
     author="Marc Udoff",
     description=pkg_json["description"],
     license=pkg_json["license"],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
-    install_requires=["jupyter_server>=1.6,<2"],
+    packages=setuptools.find_namespace_packages(),
+    install_requires=["jupyter_server>=2.0.1,<3"],
     zip_safe=False,
     include_package_data=True,
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     platforms="Linux, Mac OS X, Windows",
-    keywords=["Jupyter", "JupyterLab", "JupyterLab3"],
+    keywords=["Jupyter", "JupyterLab", "JupyterLab4"],
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Framework :: Jupyter",
+        "Framework :: Jupyter :: JupyterLab",
+        "Framework :: Jupyter :: JupyterLab :: 4",
+        "Framework :: Jupyter :: JupyterLab :: Extensions",
+        "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
     ],
 )
 
 
 post_develop = npm_builder(
-    build_cmd="install:extension", source_dir="src", build_dir=lab_path
+    build_cmd="install:extension", source_dir="src", build_dir=lab_path, npm="jlpm"
 )
 setup_args["cmdclass"] = wrap_installers(
     post_develop=post_develop, ensured_targets=ensured_targets
 )
 setup_args["data_files"] = get_data_files(data_files_spec)
 
 if __name__ == "__main__":
```

### Comparing `jupyterlab_limit_output-1.0.1/src/formatters.ts` & `jupyterlab_limit_output-2.0.0/src/formatters.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_limit_output-1.0.1/src/index.ts` & `jupyterlab_limit_output-2.0.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_limit_output-1.0.1/src/renders.ts` & `jupyterlab_limit_output-2.0.0/src/renders.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_limit_output-1.0.1/tsconfig.json` & `jupyterlab_limit_output-2.0.0/tsconfig.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'compilerOptions'": "{'target': 'es2018'}"}*

```diff
@@ -13,14 +13,14 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": false,
-        "target": "es2017",
+        "target": "es2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

### Comparing `jupyterlab_limit_output-1.0.1/tslint.json` & `jupyterlab_limit_output-2.0.0/tslint.json`

 * *Files identical despite different names*

