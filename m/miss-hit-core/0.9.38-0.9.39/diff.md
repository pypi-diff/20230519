# Comparing `tmp/miss_hit_core-0.9.38.tar.gz` & `tmp/miss_hit_core-0.9.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miss_hit_core-0.9.38.tar", last modified: Thu Apr 27 13:22:02 2023, max compression
+gzip compressed data, was "miss_hit_core-0.9.39.tar", last modified: Fri May 19 08:49:30 2023, max compression
```

## Comparing `miss_hit_core-0.9.38.tar` & `miss_hit_core-0.9.39.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 13:22:02.395142 miss_hit_core-0.9.38/
--rw-r--r--   0 florian   (1000) florian   (1000)    35149 2019-11-17 11:29:52.000000 miss_hit_core-0.9.38/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)    34523 2020-08-01 08:20:05.000000 miss_hit_core-0.9.38/LICENSE.AGPL
--rw-r--r--   0 florian   (1000) florian   (1000)     7105 2023-04-27 13:22:02.395142 miss_hit_core-0.9.38/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     6013 2022-09-18 09:39:54.000000 miss_hit_core-0.9.38/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 13:22:02.391142 miss_hit_core-0.9.38/miss_hit_core/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-08-16 07:52:19.000000 miss_hit_core-0.9.38/miss_hit_core/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    17465 2022-08-21 10:31:44.000000 miss_hit_core-0.9.38/miss_hit_core/cfg_ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)    21616 2022-08-21 10:02:24.000000 miss_hit_core-0.9.38/miss_hit_core/cfg_parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16418 2022-08-21 10:17:29.000000 miss_hit_core-0.9.38/miss_hit_core/cfg_tree.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18733 2023-04-27 13:12:57.000000 miss_hit_core-0.9.38/miss_hit_core/command_line.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18974 2022-08-21 08:54:39.000000 miss_hit_core-0.9.38/miss_hit_core/config.py
--rw-r--r--   0 florian   (1000) florian   (1000)    28769 2022-09-18 10:39:23.000000 miss_hit_core-0.9.38/miss_hit_core/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)   112055 2022-09-18 10:38:40.000000 miss_hit_core-0.9.38/miss_hit_core/m_ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2182 2021-03-18 19:12:14.000000 miss_hit_core-0.9.38/miss_hit_core/m_entity_root.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11754 2022-09-18 09:26:58.000000 miss_hit_core-0.9.38/miss_hit_core/m_language.py
--rw-r--r--   0 florian   (1000) florian   (1000)    33495 2020-08-16 07:52:19.000000 miss_hit_core-0.9.38/miss_hit_core/m_language_builtins.py
--rw-r--r--   0 florian   (1000) florian   (1000)    63616 2022-09-18 10:33:17.000000 miss_hit_core-0.9.38/miss_hit_core/m_lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4033 2022-08-13 12:46:59.000000 miss_hit_core-0.9.38/miss_hit_core/m_parse_utils.py
--rw-r--r--   0 florian   (1000) florian   (1000)    81627 2022-09-18 10:33:45.000000 miss_hit_core-0.9.38/miss_hit_core/m_parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4413 2020-09-12 11:41:10.000000 miss_hit_core-0.9.38/miss_hit_core/m_types.py
--rw-r--r--   0 florian   (1000) florian   (1000)    43076 2022-09-18 10:28:55.000000 miss_hit_core-0.9.38/miss_hit_core/mh_metric.py
--rw-r--r--   0 florian   (1000) florian   (1000)    52025 2022-09-18 10:05:58.000000 miss_hit_core-0.9.38/miss_hit_core/mh_style.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2450 2021-10-30 16:34:20.000000 miss_hit_core-0.9.38/miss_hit_core/pathutil.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 13:22:02.391142 miss_hit_core-0.9.38/miss_hit_core/resources/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 13:22:02.395142 miss_hit_core-0.9.38/miss_hit_core/resources/assets/
--rw-r--r--   0 florian   (1000) florian   (1000)      424 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/alert-triangle.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      355 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/bar-chart-2.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      345 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/check-square.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      370 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/download.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/edit.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      388 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/external-link.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      473 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/file-text.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/help-circle.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      517 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/package.svg
--rw-r--r--   0 florian   (1000) florian   (1000)     1011 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/settings.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      310 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/assets/terminal.svg
--rw-r--r--   0 florian   (1000) florian   (1000)     3101 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core/resources/style.css
--rw-r--r--   0 florian   (1000) florian   (1000)     3518 2020-11-30 09:06:20.000000 miss_hit_core-0.9.38/miss_hit_core/resources.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9895 2023-04-27 13:12:57.000000 miss_hit_core-0.9.38/miss_hit_core/s_ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)    23398 2023-04-27 13:12:57.000000 miss_hit_core-0.9.38/miss_hit_core/s_parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2150 2023-04-27 13:21:29.000000 miss_hit_core-0.9.38/miss_hit_core/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)     8074 2023-03-23 13:17:08.000000 miss_hit_core-0.9.38/miss_hit_core/work_package.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 13:22:02.391142 miss_hit_core-0.9.38/miss_hit_core.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     7105 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1391 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       98 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       14 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/miss_hit_core.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-04-27 13:22:02.395142 miss_hit_core-0.9.38/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     1662 2023-04-27 13:22:02.000000 miss_hit_core-0.9.38/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-19 08:49:30.628721 miss_hit_core-0.9.39/
+-rw-r--r--   0 florian   (1000) florian   (1000)    35149 2019-11-17 11:29:52.000000 miss_hit_core-0.9.39/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)    34523 2020-08-01 08:20:05.000000 miss_hit_core-0.9.39/LICENSE.AGPL
+-rw-r--r--   0 florian   (1000) florian   (1000)     7254 2023-05-19 08:49:30.628721 miss_hit_core-0.9.39/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     6162 2023-05-19 08:46:33.000000 miss_hit_core-0.9.39/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-19 08:49:30.628721 miss_hit_core-0.9.39/miss_hit_core/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-08-16 07:52:19.000000 miss_hit_core-0.9.39/miss_hit_core/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    17465 2022-08-21 10:31:44.000000 miss_hit_core-0.9.39/miss_hit_core/cfg_ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    21634 2023-05-19 08:46:33.000000 miss_hit_core-0.9.39/miss_hit_core/cfg_parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16418 2022-08-21 10:17:29.000000 miss_hit_core-0.9.39/miss_hit_core/cfg_tree.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    18768 2023-05-19 08:46:33.000000 miss_hit_core-0.9.39/miss_hit_core/command_line.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    19019 2023-05-19 08:46:33.000000 miss_hit_core-0.9.39/miss_hit_core/config.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    28905 2023-05-19 08:46:33.000000 miss_hit_core-0.9.39/miss_hit_core/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)   112073 2023-05-19 08:46:33.000000 miss_hit_core-0.9.39/miss_hit_core/m_ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2182 2021-03-18 19:12:14.000000 miss_hit_core-0.9.39/miss_hit_core/m_entity_root.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11754 2022-09-18 09:26:58.000000 miss_hit_core-0.9.39/miss_hit_core/m_language.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    33495 2020-08-16 07:52:19.000000 miss_hit_core-0.9.39/miss_hit_core/m_language_builtins.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    63636 2023-05-19 08:46:33.000000 miss_hit_core-0.9.39/miss_hit_core/m_lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4033 2022-08-13 12:46:59.000000 miss_hit_core-0.9.39/miss_hit_core/m_parse_utils.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    81627 2022-09-18 10:33:45.000000 miss_hit_core-0.9.39/miss_hit_core/m_parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4413 2020-09-12 11:41:10.000000 miss_hit_core-0.9.39/miss_hit_core/m_types.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    43130 2023-05-19 08:46:33.000000 miss_hit_core-0.9.39/miss_hit_core/mh_metric.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    52197 2023-05-19 08:46:33.000000 miss_hit_core-0.9.39/miss_hit_core/mh_style.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2450 2021-10-30 16:34:20.000000 miss_hit_core-0.9.39/miss_hit_core/pathutil.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-19 08:49:30.628721 miss_hit_core-0.9.39/miss_hit_core/resources/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-19 08:49:30.628721 miss_hit_core-0.9.39/miss_hit_core/resources/assets/
+-rw-r--r--   0 florian   (1000) florian   (1000)      424 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/alert-triangle.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      355 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/bar-chart-2.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      345 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/check-square.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      370 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/download.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/edit.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      388 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/external-link.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      473 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/file-text.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/help-circle.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      517 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/package.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)     1011 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/settings.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      310 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/assets/terminal.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)     3101 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core/resources/style.css
+-rw-r--r--   0 florian   (1000) florian   (1000)     3518 2020-11-30 09:06:20.000000 miss_hit_core-0.9.39/miss_hit_core/resources.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10267 2023-05-16 12:34:12.000000 miss_hit_core-0.9.39/miss_hit_core/s_ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    23932 2023-05-19 08:46:33.000000 miss_hit_core-0.9.39/miss_hit_core/s_parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2150 2023-05-19 08:49:15.000000 miss_hit_core-0.9.39/miss_hit_core/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     8074 2023-03-23 13:17:08.000000 miss_hit_core-0.9.39/miss_hit_core/work_package.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-19 08:49:30.628721 miss_hit_core-0.9.39/miss_hit_core.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     7254 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1391 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       98 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       14 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/miss_hit_core.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-05-19 08:49:30.632721 miss_hit_core-0.9.39/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     1662 2023-05-19 08:49:30.000000 miss_hit_core-0.9.39/setup.py
```

### Comparing `miss_hit_core-0.9.38/LICENSE` & `miss_hit_core-0.9.39/LICENSE`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/LICENSE.AGPL` & `miss_hit_core-0.9.39/LICENSE.AGPL`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/PKG-INFO` & `miss_hit_core-0.9.39/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miss_hit_core
-Version: 0.9.38
+Version: 0.9.39
 Summary: Code formatting and code metrics for programs written in the MATLAB/Simulink and Octave languages.
 Home-page: https://misshit.org
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/miss_hit/issues
 Project-URL: Documentation, https://florianschanda.github.io/miss_hit/
@@ -111,23 +111,31 @@
 $ mh_style --process-slx my_model.slx
 $ mh_style src/
 ```
 
 Configuration and setup is described in the
 [user manuals](https://florianschanda.github.io/miss_hit)
 
+### Installation via pipx
+
+Very similar to the above:
+
+```
+$ pipx install miss_hit --include-deps
+```
+
 ### Installation by checkout
 
-It is recommended to use pip, as that gets you the latest stable
-release. However, it is possible to directly use MISS_HIT from a
-checkout.  MISS_HIT does not require *any* python packages or
-libraries. Just check out the repository and put it on your
-path. That's it.
+It is recommended to use pip or pipx, as that gets you the latest
+stable release. However, it is possible to directly use MISS_HIT from
+a checkout. MISS_HIT currently does not require *any* non-standard
+python packages or libraries as dependencies. Just check out the
+repository and put it on your path. That's it.
 
-The version of Python I am using is `3.6` but any later version should
+The version of Python I am using is `3.7` but any later version should
 also work. I am not using any overly fancy language features.
 
 ### Additional requirements for developing MISS_HIT
 
 If you want to help develop you will need Linux as the test-suite
 doesn't really work on Windows. You will also need Pylint,
 PyCodeStyle, Coverage, and Graphviz. Install as follows:
```

### Comparing `miss_hit_core-0.9.38/README.md` & `miss_hit_core-0.9.39/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,23 +86,31 @@
 $ mh_style --process-slx my_model.slx
 $ mh_style src/
 ```
 
 Configuration and setup is described in the
 [user manuals](https://florianschanda.github.io/miss_hit)
 
+### Installation via pipx
+
+Very similar to the above:
+
+```
+$ pipx install miss_hit --include-deps
+```
+
 ### Installation by checkout
 
-It is recommended to use pip, as that gets you the latest stable
-release. However, it is possible to directly use MISS_HIT from a
-checkout.  MISS_HIT does not require *any* python packages or
-libraries. Just check out the repository and put it on your
-path. That's it.
+It is recommended to use pip or pipx, as that gets you the latest
+stable release. However, it is possible to directly use MISS_HIT from
+a checkout. MISS_HIT currently does not require *any* non-standard
+python packages or libraries as dependencies. Just check out the
+repository and put it on your path. That's it.
 
-The version of Python I am using is `3.6` but any later version should
+The version of Python I am using is `3.7` but any later version should
 also work. I am not using any overly fancy language features.
 
 ### Additional requirements for developing MISS_HIT
 
 If you want to help develop you will need Linux as the test-suite
 doesn't really work on Windows. You will also need Pylint,
 PyCodeStyle, Coverage, and Graphviz. Install as follows:
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/cfg_ast.py` & `miss_hit_core-0.9.39/miss_hit_core/cfg_ast.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/cfg_parser.py` & `miss_hit_core-0.9.39/miss_hit_core/cfg_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         self.language = Config_Language()
         self.filename = config_file
         self.dirname = os.path.dirname(pathutil.abspath(config_file))
         self.mh = mh
 
         self.mh.register_file(self.filename)
-        with open(config_file, "r") as fd:
+        with open(config_file, "r", encoding="UTF-8") as fd:
             content = fd.read()
         self.lexer = m_lexer.MATLAB_Lexer(self.language,
                                           mh, content, self.filename)
         self.lexer.process_pragmas = False
 
         # pylint: disable=invalid-name
         self.ct = None
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/cfg_tree.py` & `miss_hit_core-0.9.39/miss_hit_core/cfg_tree.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/command_line.py` & `miss_hit_core-0.9.39/miss_hit_core/command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,22 +424,22 @@
                 assert isinstance(result, work_package.Result)
                 mh.integrate(result.wp.mh)
                 if result.processed:
                     mh.finalize_file(result.wp.filename)
                     back_end.process_result(result)
 
     else:
-        pool = multiprocessing.Pool()
-        for results in pool.imap(process_fn, work_list, 5):
-            for result in results:
-                assert isinstance(result, work_package.Result)
-                mh.integrate(result.wp.mh)
-                if result.processed:
-                    mh.finalize_file(result.wp.filename)
-                    back_end.process_result(result)
+        with multiprocessing.Pool() as pool:
+            for results in pool.imap(process_fn, work_list, 5):
+                for result in results:
+                    assert isinstance(result, work_package.Result)
+                    mh.integrate(result.wp.mh)
+                    if result.processed:
+                        mh.finalize_file(result.wp.filename)
+                        back_end.process_result(result)
 
     # Call hook for final work and issue summary message
 
     back_end.post_process()
     mh.summary_and_exit()
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/config.py` & `miss_hit_core-0.9.39/miss_hit_core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 ##  GNU General Public License for more details.                            ##
 ##                                                                          ##
 ##  You should have received a copy of the GNU General Public License       ##
 ##  along with MISS_HIT. If not, see <http://www.gnu.org/licenses/>.        ##
 ##                                                                          ##
 ##############################################################################
 
+# pylint: disable=consider-using-dict-items
+
 from copy import deepcopy
 from miss_hit_core.m_language import MATLAB_Latest_Language
 
 
 ##############################################################################
 # Configuration class. This will be passed to every bit of code that
 # analyzes anything.
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/errors.py` & `miss_hit_core-0.9.39/miss_hit_core/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         self.sort_messages = True
 
         self.messages = {}        # file -> line -> [message]
         self.justifications = {}  # file -> line -> [justification]
 
     def debug_dump(self):
         print("Debug dump for Message_Handler object")
-        for file_name in self.messages:
+        for file_name in sorted(self.messages):
             print("> File name: %s" % file_name)
             for line in sorted(self.messages[file_name]):
                 print("  Line: %u" % line)
                 for msg in self.messages[file_name][line]:
                     print("    ", str(msg))
 
     def reset_seen(self):
@@ -642,18 +642,19 @@
 
     def fork(self):
         rv = HTML_Message_Handler(self.tool_id, self.filename)
         self.fork_copy_attributes(rv)
         return rv
 
     def setup_fd(self):
+        # pylint: disable=consider-using-with
         if self.fd is not None:
             return
 
-        self.fd = open(self.filename, "w")
+        self.fd = open(self.filename, "w", encoding="UTF-8")
         self.fd.write("<!DOCTYPE html>\n")
         self.fd.write("<html>\n")
         self.fd.write("<head>\n")
         self.fd.write("<meta charset=\"UTF-8\">\n")
         # Link style-sheet with a relative path based on where the
         # output report file will be
         self.fd.write("<link rel=\"stylesheet\" href=\"file:%s\">\n" %
@@ -733,18 +734,19 @@
 
     def fork(self):
         rv = JSON_Message_Handler(self.tool_id, self.filename)
         self.fork_copy_attributes(rv)
         return rv
 
     def setup_fd(self):
+        # pylint: disable=consider-using-with
         if self.fd is not None:
             return
 
-        self.fd = open(self.filename, "w")
+        self.fd = open(self.filename, "w", encoding="UTF-8")
         self.blob = {}
 
     def emit_message(self, message):
         self.setup_fd()
 
         if message.location.filename not in self.blob:
             self.blob[message.location.filename] = []
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/m_ast.py` & `miss_hit_core-0.9.39/miss_hit_core/m_ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -3343,11 +3343,11 @@
                                                  hash(node),
                                                  annotation))
 
 
 def dotpr(filename, root_node):
     assert isinstance(filename, str)
     assert isinstance(root_node, Node)
-    with open(filename, "w") as fd:
+    with open(filename, "w", encoding="UTF-8") as fd:
         fd.write("digraph G {\n")
         dot(fd, None, "", root_node)
         fd.write("}\n")
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/m_entity_root.py` & `miss_hit_core-0.9.39/miss_hit_core/m_entity_root.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/m_language.py` & `miss_hit_core-0.9.39/miss_hit_core/m_language.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/m_language_builtins.py` & `miss_hit_core-0.9.39/miss_hit_core/m_language_builtins.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/m_lexer.py` & `miss_hit_core-0.9.39/miss_hit_core/m_lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,17 +537,17 @@
                     while self.nc in "0123456789":
                         self.skip()
                         suffix += self.cc
 
                     if suffix not in ("8", "16", "32", "64"):
                         self.lex_error("suffix must be 8, 16, 32, or 64")
                     else:
-                        max_digits = int(suffix) / bits_per_digit
+                        max_digits = int(suffix) // bits_per_digit
                 else:
-                    max_digits = 64 / bits_per_digit
+                    max_digits = 64 // bits_per_digit
 
                 if len(digits) > max_digits:
                     self.lex_error(
                         "too many digits for %u-bit %s literal" %
                         (max_digits * bits_per_digit,
                          "binary" if bits_per_digit == 1 else "hex"))
 
@@ -1520,15 +1520,15 @@
             elif token.ast_link is None:
                 self.mh.info(token.location,
                              "this token is not linked to the ast")
 
 
 def sanity_test(mh, filename):
     mh.register_file(filename)
-    with open(filename, "r") as fd:
+    with open(filename, "r", encoding="UTF-8") as fd:
         content = fd.read()
     try:
         language = MATLAB_Latest_Language()
         lexer = MATLAB_Lexer(language, mh, content, filename)
         lexer.debug_comma = True
         while True:
             tok = lexer.token()
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/m_parse_utils.py` & `miss_hit_core-0.9.39/miss_hit_core/m_parse_utils.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/m_parser.py` & `miss_hit_core-0.9.39/miss_hit_core/m_parser.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/m_types.py` & `miss_hit_core-0.9.39/miss_hit_core/m_types.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/mh_metric.py` & `miss_hit_core-0.9.39/miss_hit_core/mh_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1043,29 +1043,29 @@
         # Build ticket summary
 
         ticket_summary = build_ticket_summary(self.metrics)
 
         # Generate report
 
         if self.options.text:
-            with open(self.options.text, "w") as fd:
+            with open(self.options.text, "w", encoding="UTF-8") as fd:
                 write_text_report(fd,
                                   self.metrics,
                                   ticket_summary,
                                   worst_offenders)
         elif self.options.html:
-            with open(self.options.html, "w") as fd:
+            with open(self.options.html, "w", encoding="UTF-8") as fd:
                 write_html_report(fd,
                                   self.options.entry_point,
                                   self.options.portable_html,
                                   self.metrics,
                                   ticket_summary,
                                   worst_offenders)
         elif self.options.json:
-            with open(self.options.json, "w") as fd:
+            with open(self.options.json, "w", encoding="UTF-8") as fd:
                 json.dump(build_json_report(self.metrics, worst_offenders),
                           fd,
                           indent=4,
                           sort_keys=True)
         elif self.options.ci:
             # In the CI mode we don't produce any report at all
             pass
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/mh_style.py` & `miss_hit_core-0.9.39/miss_hit_core/mh_style.py`

 * *Files 1% similar despite different names*

```diff
@@ -1230,16 +1230,16 @@
         action="store_true",
         default=False,
         help="Debug option to check AST links")
 
     style_option = clp["ap"].add_argument_group("rule options")
 
     # Add any parameters from rules
-    for rule_kind in rule_set:
-        for rule in rule_set[rule_kind]:
+    for rules in rule_set.values():
+        for rule in rules:
             rule_params = getattr(rule, "parameters", None)
             if not rule_params:
                 continue
             for p_name in rule_params:
                 style_option.add_argument("--" + p_name,
                                           **rule_params[p_name])
 
@@ -1273,16 +1273,20 @@
     mh.autofix      = options.fix
 
     extra_options = {
         "fd_tree"  : None,
         "rule_set" : rule_set,
     }
 
+    # pylint: disable=consider-using-with
     if options.debug_dump_tree:
-        extra_options["fd_tree"] = open(options.debug_dump_tree, "w")
+        extra_options["fd_tree"] = open(options.debug_dump_tree,
+                                        "w",
+                                        encoding="UTF-8")
+    # pylint: enable=consider-using-with
 
     style_backend = MH_Style()
     command_line.execute(mh, options, extra_options,
                          style_backend,
                          options.process_slx)
 
     if options.debug_dump_tree:
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/pathutil.py` & `miss_hit_core-0.9.39/miss_hit_core/pathutil.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/resources/assets/package.svg` & `miss_hit_core-0.9.39/miss_hit_core/resources/assets/package.svg`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/resources/assets/settings.svg` & `miss_hit_core-0.9.39/miss_hit_core/resources/assets/settings.svg`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/resources/style.css` & `miss_hit_core-0.9.39/miss_hit_core/resources/style.css`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/resources.py` & `miss_hit_core-0.9.39/miss_hit_core/resources.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core/s_ast.py` & `miss_hit_core-0.9.39/miss_hit_core/s_ast.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,27 +161,31 @@
 
     def iter_all_blocks(self):
         for n_block in self.d_blocks.values():
             yield from n_block.iter_all_blocks()
 
 
 class Block(Node):
-    def __init__(self, sid, name, kind):
+    def __init__(self, sid, name, kind, custom_attr):
         assert isinstance(sid, str), "expected string, got %s" % type(sid)
         assert isinstance(name, str)
         assert isinstance(kind, str)
+        assert isinstance(custom_attr, list)
 
         super().__init__()
 
-        self.sid  = sid
-        self.name = name
-        self.kind = kind
+        self.sid         = sid
+        self.name        = name
+        self.kind        = kind
+        self.custom_attr = custom_attr
 
     def dump_hierarchy(self, indent=0):
         print(" " * indent, "Block %s (%s)" % (self.kind, repr(self.name)))
+        for attr in self.custom_attr:
+            print(" " * (indent + 1), "Attribute (%s)" % attr)
 
     def set_parent(self, n_parent):
         assert isinstance(n_parent, System)
         super().set_parent(n_parent)
 
     def get_container(self):
         ptr = self.n_parent
@@ -220,38 +224,40 @@
                         blockname = self.local_name())
 
     def iter_all_blocks(self):
         yield self
 
 
 class Sub_System(Block):
-    def __init__(self, sid, name, n_system):
-        super().__init__(sid, name, "SubSystem")
+    def __init__(self, sid, name, n_system, custom_attr):
+        super().__init__(sid, name, "SubSystem", custom_attr)
         assert isinstance(n_system, System)
 
         self.n_system = n_system
         self.n_system.set_parent(self)
 
     def dump_hierarchy(self, indent=0):
         print(" " * indent, "Block %s (%s)" % (self.kind, repr(self.name)))
+        for attr in self.custom_attr:
+            print(" " * (indent + 1), "Attribute (%s)" % attr)
         self.n_system.dump_hierarchy(indent + 1)
 
     def iter_all_blocks(self):
         yield self
         yield from self.n_system.iter_all_blocks()
 
 
 class Matlab_Function(Block):
     # In Simulink this is actually a magic Subsystem that you cannot
     # enter, that contains an S-Function block referencing a Stateflow
     # MATLAB function. We hide this as well, but in a different way:
     # we pretend it's a distinct top-level object (and not a special
     # kind of sub-system).
-    def __init__(self, sid, name, sref):
-        super().__init__(sid, name, "SubSystem")
+    def __init__(self, sid, name, sref, custom_attr):
+        super().__init__(sid, name, "SubSystem", custom_attr)
         assert isinstance(sref, Source_Reference)
 
         self.sref = sref
 
     def get_encoding(self):
         n_container = self.get_container()
         return n_container.encoding
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/s_parser.py` & `miss_hit_core-0.9.39/miss_hit_core/s_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,28 +31,27 @@
 """
 
 import os.path
 import zipfile
 import xml.etree.ElementTree as ET
 
 from abc import ABCMeta, abstractmethod
-from io import StringIO
 from html.parser import HTMLParser
 
 from miss_hit_core.config import Config
 from miss_hit_core.s_ast import *
 from miss_hit_core.errors import Message_Handler, ICE
 from miss_hit_core.m_language import MATLAB_Latest_Language
 
 # pylint: disable=invalid-name
 anatomy = {}
 # pylint: enable=invalid-name
 
 
-class HTML_Text_Extractor(HTMLParser):
+class HTML_Text_Extractor(HTMLParser):  # pylint: disable=abstract-method
     def __init__(self):
         super().__init__()
         self.reset()
         self.strict = False
         self.convert_charrefs = True
         self.text = ""
         self.processing = False
@@ -69,17 +68,17 @@
         if tag == "body":
             self.processing = False
         if not self.processing:
             return
         if tag in ("p", "div"):
             self.text += "\n"
 
-    def handle_data(self, d):
+    def handle_data(self, data):
         if self.processing:
-            self.text += d
+            self.text += data
 
 
 class Simulink_Parser(metaclass=ABCMeta):
     def __init__(self, mh, filename, cfg):
         assert isinstance(mh, Message_Handler)
         assert isinstance(filename, str)
         assert isinstance(cfg, Config)
@@ -191,22 +190,22 @@
                     self.xml_blockdiagram.write(fd)
             if self.xml_stateflow:
                 with zfd.open("simulink/stateflow.xml", mode="w") as fd:
                     self.xml_stateflow.write(fd)
             if self.xml_coreproperties:
                 with zfd.open("metadata/coreProperties.xml", mode="w") as fd:
                     self.xml_coreproperties.write(fd)
-            for sys_id in self.xml_ref_systems:
+            for sys_id, et_node in self.xml_ref_systems.items():
                 with zfd.open("simulink/systems/%s.xml" % sys_id,
                               mode="w") as fd:
-                    self.xml_ref_systems[sys_id].write(fd)
-            for sf_id in self.xml_ref_stateflow:
+                    et_node.write(fd)
+            for sf_id, et_node in self.xml_ref_stateflow.items():
                 with zfd.open("simulink/systems/%s.xml" % sf_id,
                               mode="w") as fd:
-                    self.xml_ref_stateflow[sf_id].write(fd)
+                    et_node.write(fd)
             for name in sorted(self.other_content):
                 with zfd.open(name, mode="w") as fd:
                     fd.write(self.other_content[name])
 
     def loc(self):
         return Location(self.filename,
                         blockname = "/".join(self.name_stack))
@@ -237,16 +236,15 @@
                 name, info = self.parse_instance(et_item)
                 d_instances[name] = info
             else:
                 self.mh.error(self.loc(),
                               "unknown top-level stateflow item %s" %
                               et_item.tag)
 
-        for name in d_instances:
-            machine_id, chart_id = d_instances[name]
+        for name, (machine_id, chart_id) in d_instances.items():
             self.sf_names[name] = d_machines[machine_id][chart_id]
 
     def parse_instance(self, et_instance):
         assert isinstance(et_instance, ET.Element)
         assert et_instance.tag == "instance"
 
         props = self.parse_p_tags(et_instance)
@@ -301,15 +299,15 @@
 
         return d_machine
 
     ######################################################################
     # Simulink parsing
     ######################################################################
 
-    def parse_block_matlab_function(self, et_block, props):
+    def parse_block_matlab_function(self, et_block, props, custom_attr):
         assert isinstance(et_block, ET.Element)
         assert isinstance(props, dict)
         assert et_block.tag == "Block"
         assert et_block.attrib["BlockType"] == "SubSystem"
         assert props.get("SFBlockType", None) == "MATLAB Function"
         assert not self.is_external_harness
 
@@ -345,30 +343,33 @@
                 if et_script and not is_eml:
                     raise ICE("script found, but isEML is not true")
         if et_script is None:
             raise ICE("referenced script for %s not found" % sf_base_name)
 
         return Matlab_Function(et_block.attrib["SID"],
                                et_block.attrib["Name"],
-                               SLX_Reference(et_script))
+                               SLX_Reference(et_script),
+                               custom_attr)
 
-    def parse_block_subsystem(self, et_block):
+    def parse_block_subsystem(self, et_block, custom_attr):
         assert isinstance(et_block, ET.Element)
         assert et_block.tag == "Block"
         assert et_block.attrib["BlockType"] == "SubSystem"
 
         n_system    = None
         system_name = et_block.attrib["Name"]
 
         props = self.parse_p_tags(et_block)
 
         if props.get("SFBlockType", None) == "MATLAB Function":
             # This could be a special "MATLAB Function" sub-system, in
             # which case we special case
-            n_block = self.parse_block_matlab_function(et_block, props)
+            n_block = self.parse_block_matlab_function(et_block,
+                                                       props,
+                                                       custom_attr)
 
         else:
             # This is a normal sub-system. First we're finding the system
             # nested.
             for et_item in et_block:
                 if et_item.tag == "System":
                     if n_system:
@@ -376,15 +377,16 @@
                     self.name_stack.append(system_name)
                     n_system = self.parse_system(et_item)
                     self.name_stack.pop()
 
             # Then we build a sub-system block referencing the system
             n_block = Sub_System(et_block.attrib["SID"],
                                  system_name,
-                                 n_system)
+                                 n_system,
+                                 custom_attr)
 
         return n_block
 
     def parse_block(self, et_block):
         assert isinstance(et_block, ET.Element)
         assert et_block.tag == "Block"
 
@@ -394,23 +396,30 @@
 
         if block_type not in anatomy:
             anatomy[block_type] = set()
         for et_child in et_block:
             if et_child.tag not in ("P", "Port"):
                 anatomy[block_type].add(et_child.tag)
 
-        # Parse block
+        # Get custom attributes
+        custom_attr = []
+        for et_item in et_block:
+            if et_item.tag == "P":
+                if et_item.attrib["Name"] == "AttributesFormatString":
+                    custom_attr = et_item.text.splitlines()
 
+        # Parse block
         if block_type == "SubSystem":
-            n_block = self.parse_block_subsystem(et_block)
+            return self.parse_block_subsystem(et_block, custom_attr)
         else:
-            # Some other generic block
+            # Some other generic block.
             n_block = Block(et_block.attrib["SID"],
                             et_block.attrib["Name"],
-                            block_type)
+                            block_type,
+                            custom_attr)
 
         return n_block
 
     def parse_annotation(self, et_anno):
         assert isinstance(et_anno, ET.Element)
         assert et_anno.tag == "Annotation"
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/version.py` & `miss_hit_core-0.9.39/miss_hit_core/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 ##                                                                          ##
 ##############################################################################
 
 # Some constants we use for tool version and URLs
 
 GITHUB_ISSUES = "https://github.com/florianschanda/miss_hit/issues"
 
-VERSION_TUPLE = (0, 9, 38)
+VERSION_TUPLE = (0, 9, 39)
 VERSION_SUFFIX = ""
 
 VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
           ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "MISS_HIT %s" % VERSION
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core/work_package.py` & `miss_hit_core-0.9.39/miss_hit_core/work_package.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/miss_hit_core.egg-info/PKG-INFO` & `miss_hit_core-0.9.39/miss_hit_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miss-hit-core
-Version: 0.9.38
+Version: 0.9.39
 Summary: Code formatting and code metrics for programs written in the MATLAB/Simulink and Octave languages.
 Home-page: https://misshit.org
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/miss_hit/issues
 Project-URL: Documentation, https://florianschanda.github.io/miss_hit/
@@ -111,23 +111,31 @@
 $ mh_style --process-slx my_model.slx
 $ mh_style src/
 ```
 
 Configuration and setup is described in the
 [user manuals](https://florianschanda.github.io/miss_hit)
 
+### Installation via pipx
+
+Very similar to the above:
+
+```
+$ pipx install miss_hit --include-deps
+```
+
 ### Installation by checkout
 
-It is recommended to use pip, as that gets you the latest stable
-release. However, it is possible to directly use MISS_HIT from a
-checkout.  MISS_HIT does not require *any* python packages or
-libraries. Just check out the repository and put it on your
-path. That's it.
+It is recommended to use pip or pipx, as that gets you the latest
+stable release. However, it is possible to directly use MISS_HIT from
+a checkout. MISS_HIT currently does not require *any* non-standard
+python packages or libraries as dependencies. Just check out the
+repository and put it on your path. That's it.
 
-The version of Python I am using is `3.6` but any later version should
+The version of Python I am using is `3.7` but any later version should
 also work. I am not using any overly fancy language features.
 
 ### Additional requirements for developing MISS_HIT
 
 If you want to help develop you will need Linux as the test-suite
 doesn't really work on Windows. You will also need Pylint,
 PyCodeStyle, Coverage, and Graphviz. Install as follows:
```

### Comparing `miss_hit_core-0.9.38/miss_hit_core.egg-info/SOURCES.txt` & `miss_hit_core-0.9.39/miss_hit_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.38/setup.py` & `miss_hit_core-0.9.39/setup.py`

 * *Files identical despite different names*

