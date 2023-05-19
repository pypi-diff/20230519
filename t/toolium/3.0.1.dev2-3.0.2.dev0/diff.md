# Comparing `tmp/toolium-3.0.1.dev2.tar.gz` & `tmp/toolium-3.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolium-3.0.1.dev2.tar", last modified: Fri May  5 14:58:07 2023, max compression
+gzip compressed data, was "toolium-3.0.2.dev0.tar", last modified: Fri May 19 09:08:23 2023, max compression
```

## Comparing `toolium-3.0.1.dev2.tar` & `toolium-3.0.2.dev0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.252834 toolium-3.0.1.dev2/
--rw-rw-rw-   0        0        0    29956 2023-05-05 14:55:10.000000 toolium-3.0.1.dev2/CHANGELOG.rst
--rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.1.dev2/LICENSE
--rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.1.dev2/MANIFEST.in
--rw-rw-rw-   0        0        0     5526 2023-05-05 14:58:07.252834 toolium-3.0.1.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     4031 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/README.rst
--rw-rw-rw-   0        0        0       12 2023-05-05 14:55:10.000000 toolium-3.0.1.dev2/VERSION
--rw-rw-rw-   0        0        0      225 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/requirements.txt
--rw-rw-rw-   0        0        0      205 2023-05-05 08:33:04.000000 toolium-3.0.1.dev2/requirements_dev.txt
--rw-rw-rw-   0        0        0       70 2023-05-05 14:58:07.253833 toolium-3.0.1.dev2/setup.cfg
--rw-rw-rw-   0        0        0     3229 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.119833 toolium-3.0.1.dev2/toolium/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev2/toolium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.135837 toolium-3.0.1.dev2/toolium/behave/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev2/toolium/behave/__init__.py
--rw-rw-rw-   0        0        0    12432 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/behave/env_utils.py
--rw-rw-rw-   0        0        0    10973 2023-05-05 14:55:10.000000 toolium-3.0.1.dev2/toolium/behave/environment.py
--rw-rw-rw-   0        0        0    21012 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/config_driver.py
--rw-rw-rw-   0        0        0     2461 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/config_files.py
--rw-rw-rw-   0        0        0     8412 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/config_parser.py
--rw-rw-rw-   0        0        0    16655 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/driver_wrapper.py
--rw-rw-rw-   0        0        0    18000 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/driver_wrappers_pool.py
--rw-rw-rw-   0        0        0     6669 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/jira.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.188834 toolium-3.0.1.dev2/toolium/pageelements/
--rw-rw-rw-   0        0        0     1645 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/button_page_element.py
--rw-rw-rw-   0        0        0     1556 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/checkbox_page_element.py
--rw-rw-rw-   0        0        0     4013 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/group_page_element.py
--rw-rw-rw-   0        0        0     1290 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/input_radio_page_element.py
--rw-rw-rw-   0        0        0     2731 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/input_text_page_element.py
--rw-rw-rw-   0        0        0      942 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/link_page_element.py
--rw-rw-rw-   0        0        0    14652 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/page_element.py
--rw-rw-rw-   0        0        0     6195 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/page_elements.py
--rw-rw-rw-   0        0        0     1517 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/select_page_element.py
--rw-rw-rw-   0        0        0      930 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageelements/text_page_element.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.203874 toolium-3.0.1.dev2/toolium/pageobjects/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev2/toolium/pageobjects/__init__.py
--rw-rw-rw-   0        0        0     1996 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageobjects/common_object.py
--rw-rw-rw-   0        0        0     2273 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageobjects/mobile_page_object.py
--rw-rw-rw-   0        0        0     3535 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pageobjects/page_object.py
--rw-rw-rw-   0        0        0     2086 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/pytest_fixtures.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.212835 toolium-3.0.1.dev2/toolium/resources/
--rw-rw-rw-   0        0        0     1383 2023-04-27 16:56:50.000000 toolium-3.0.1.dev2/toolium/resources/VisualTests.css
--rw-rw-rw-   0        0        0      757 2023-04-27 16:56:50.000000 toolium-3.0.1.dev2/toolium/resources/VisualTests.js
--rw-rw-rw-   0        0        0      752 2023-04-27 16:56:50.000000 toolium-3.0.1.dev2/toolium/resources/VisualTestsTemplate.html
--rw-rw-rw-   0        0        0    12193 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/selenoid.py
--rw-rw-rw-   0        0        0     8668 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/test_cases.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.250835 toolium-3.0.1.dev2/toolium/utils/
--rw-rw-rw-   0        0        0        0 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/__init__.py
--rw-rw-rw-   0        0        0     4089 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/data_generator.py
--rw-rw-rw-   0        0        0    31957 2023-05-05 08:33:04.000000 toolium-3.0.1.dev2/toolium/utils/dataset.py
--rw-rw-rw-   0        0        0     9480 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/download_files.py
--rw-rw-rw-   0        0        0    18455 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/driver_utils.py
--rw-rw-rw-   0        0        0    19112 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/driver_wait_utils.py
--rw-rw-rw-   0        0        0     1608 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/path_utils.py
--rw-rw-rw-   0        0        0    12916 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/utils/poeditor.py
--rw-rw-rw-   0        0        0    22678 2023-04-27 16:57:03.000000 toolium-3.0.1.dev2/toolium/visual_test.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:07.126835 toolium-3.0.1.dev2/toolium.egg-info/
--rw-rw-rw-   0        0        0     5526 2023-05-05 14:58:07.000000 toolium-3.0.1.dev2/toolium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-05-05 14:58:07.000000 toolium-3.0.1.dev2/toolium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:58:07.000000 toolium-3.0.1.dev2/toolium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-05-05 14:58:07.000000 toolium-3.0.1.dev2/toolium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 14:58:07.000000 toolium-3.0.1.dev2/toolium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.986533 toolium-3.0.2.dev0/
+-rw-rw-rw-   0        0        0    30389 2023-05-19 07:42:34.000000 toolium-3.0.2.dev0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.2.dev0/LICENSE
+-rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.2.dev0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5526 2023-05-19 09:08:22.986533 toolium-3.0.2.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     4031 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/README.rst
+-rw-rw-rw-   0        0        0       12 2023-05-09 09:50:47.000000 toolium-3.0.2.dev0/VERSION
+-rw-rw-rw-   0        0        0      225 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/requirements.txt
+-rw-rw-rw-   0        0        0      236 2023-05-19 07:42:34.000000 toolium-3.0.2.dev0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       70 2023-05-19 09:08:22.988535 toolium-3.0.2.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.630532 toolium-3.0.2.dev0/toolium/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2.dev0/toolium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.669533 toolium-3.0.2.dev0/toolium/behave/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2.dev0/toolium/behave/__init__.py
+-rw-rw-rw-   0        0        0    12880 2023-05-19 07:42:34.000000 toolium-3.0.2.dev0/toolium/behave/env_utils.py
+-rw-rw-rw-   0        0        0    11018 2023-05-17 13:54:12.000000 toolium-3.0.2.dev0/toolium/behave/environment.py
+-rw-rw-rw-   0        0        0    21019 2023-05-08 11:36:54.000000 toolium-3.0.2.dev0/toolium/config_driver.py
+-rw-rw-rw-   0        0        0     2461 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/config_files.py
+-rw-rw-rw-   0        0        0     8412 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/config_parser.py
+-rw-rw-rw-   0        0        0    16655 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/driver_wrapper.py
+-rw-rw-rw-   0        0        0    18000 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/driver_wrappers_pool.py
+-rw-rw-rw-   0        0        0     6669 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/jira.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.801534 toolium-3.0.2.dev0/toolium/pageelements/
+-rw-rw-rw-   0        0        0     1645 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/button_page_element.py
+-rw-rw-rw-   0        0        0     1556 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/checkbox_page_element.py
+-rw-rw-rw-   0        0        0     4013 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/group_page_element.py
+-rw-rw-rw-   0        0        0     1290 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/input_radio_page_element.py
+-rw-rw-rw-   0        0        0     2731 2023-05-10 11:35:00.000000 toolium-3.0.2.dev0/toolium/pageelements/input_text_page_element.py
+-rw-rw-rw-   0        0        0      942 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/link_page_element.py
+-rw-rw-rw-   0        0        0    14652 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/page_element.py
+-rw-rw-rw-   0        0        0     6195 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/page_elements.py
+-rw-rw-rw-   0        0        0     1517 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/select_page_element.py
+-rw-rw-rw-   0        0        0      930 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/text_page_element.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.852537 toolium-3.0.2.dev0/toolium/pageobjects/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2.dev0/toolium/pageobjects/__init__.py
+-rw-rw-rw-   0        0        0     1996 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageobjects/common_object.py
+-rw-rw-rw-   0        0        0     2273 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageobjects/mobile_page_object.py
+-rw-rw-rw-   0        0        0     3535 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageobjects/page_object.py
+-rw-rw-rw-   0        0        0     2086 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pytest_fixtures.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.882536 toolium-3.0.2.dev0/toolium/resources/
+-rw-rw-rw-   0        0        0     1383 2023-04-27 16:56:50.000000 toolium-3.0.2.dev0/toolium/resources/VisualTests.css
+-rw-rw-rw-   0        0        0      757 2023-04-27 16:56:50.000000 toolium-3.0.2.dev0/toolium/resources/VisualTests.js
+-rw-rw-rw-   0        0        0      752 2023-04-27 16:56:50.000000 toolium-3.0.2.dev0/toolium/resources/VisualTestsTemplate.html
+-rw-rw-rw-   0        0        0    12193 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/selenoid.py
+-rw-rw-rw-   0        0        0     8733 2023-05-08 11:36:54.000000 toolium-3.0.2.dev0/toolium/test_cases.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.983535 toolium-3.0.2.dev0/toolium/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/__init__.py
+-rw-rw-rw-   0        0        0     4089 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/data_generator.py
+-rw-rw-rw-   0        0        0    31957 2023-05-05 08:33:04.000000 toolium-3.0.2.dev0/toolium/utils/dataset.py
+-rw-rw-rw-   0        0        0     9480 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/download_files.py
+-rw-rw-rw-   0        0        0    18455 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/driver_utils.py
+-rw-rw-rw-   0        0        0    19112 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/driver_wait_utils.py
+-rw-rw-rw-   0        0        0     1608 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/path_utils.py
+-rw-rw-rw-   0        0        0    12916 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/poeditor.py
+-rw-rw-rw-   0        0        0    22678 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/visual_test.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.649538 toolium-3.0.2.dev0/toolium.egg-info/
+-rw-rw-rw-   0        0        0     5526 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/top_level.txt
```

### Comparing `toolium-3.0.1.dev2/CHANGELOG.rst` & `toolium-3.0.2.dev0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 Toolium Changelog
 =================
 
-v3.0.1
+v3.0.2
 ------
 
 *Release date: In development*
 
+- `context.storage` must be initialized before dynamic environment steps in `before_feature` method
+- Mark scenario as failed when a dynamic environment step fails in `before_scenario`
+- Mark all feature scenarios as failed when a dynamic environment step fails in `before_feature` and `after_feature`
+
+v3.0.1
+------
+
+*Release date: 2023-05-09*
+
 - Allow to search in `context.storage` using `[CONTEXT:a.b.c]` replacement when `before_feature` method is not used
 - Execute after scenario methods also when a scenario is skipped to assure that scenario preconditions are cleaned
 - Fix `[LANG:key]` replacement bug when it contains carriage returns
-- `context.storage` must be initialized before dynamic environment steps
+- `context.storage` must be initialized before dynamic environment steps in `before_scenario` method
+- Fix error in Python 3.11 executing nose2 tests
 
 v3.0.0
 ------
 
 *Release date: 2023-05-03*
 
 - Add support for Python 3.11
```

### Comparing `toolium-3.0.1.dev2/LICENSE` & `toolium-3.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/PKG-INFO` & `toolium-3.0.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.1.dev2
+Version: 3.0.2.dev0
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.1.dev2/README.rst` & `toolium-3.0.2.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/setup.py` & `toolium-3.0.2.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/behave/env_utils.py` & `toolium-3.0.2.dev0/toolium/behave/env_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,22 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import sys
 import warnings
-from pkg_resources import parse_version
 
-# constants
-# pre-actions in feature files
+# Actions types defined in feature files
 ACTIONS_BEFORE_FEATURE = 'actions before the feature'
 ACTIONS_BEFORE_SCENARIO = 'actions before each scenario'
 ACTIONS_AFTER_SCENARIO = 'actions after each scenario'
 ACTIONS_AFTER_FEATURE = 'actions after the feature'
-KEYWORDS = ['Setup', 'Check', 'Given', 'When', 'Then', 'And', 'But']  # prefix in steps to actions
+# Valid prefix in action steps
+KEYWORDS = ['Setup', 'Check', 'Given', 'When', 'Then', 'And', 'But']
 GIVEN_PREFIX = 'Given'
 TABLE_SEPARATOR = '|'
 STEP_TEXT_SEPARATORS = ['"""', "'''"]
 EMPTY = ''
 
 warnings.filterwarnings('ignore')
 
@@ -114,14 +113,27 @@
             # ---- actions after each scenario ----
             context.dyn_env.execute_after_scenario_steps(context)
 
 
         def after_feature(context, feature):
             # ---- actions after feature ----
             context.dyn_env.execute_after_feature_steps(context)
+
+    Error management with behave and dynamic environment:
+        * Error in before_feature:
+                before_scenario and after_scenario are not executed
+                after_feature is executed
+                each scenario is marked as failed
+        * Error in before_scenario:
+                after_scenario is executed
+                the scenario is marked as failed
+        * Error in after_scenario:
+                the scenario status is not changed
+        * Error in after_feature:
+                the scenarios status are not changed
     """
 
     def __init__(self, **kwargs):
         """
         constructor
         :param kwargs: parameters set
         :param logger: logger instance
@@ -130,14 +142,15 @@
         logger_class = kwargs.get("logger", None)
         self.show = kwargs.get("show", True)
         self.logger = Logger(logger_class, self.show)
         self.init_actions()
         self.scenario_counter = 0
         self.feature_error = False
         self.scenario_error = False
+        self.before_error_message = None
 
     def init_actions(self):
         """clear actions lists"""
         self.actions = {ACTIONS_BEFORE_FEATURE: [],
                         ACTIONS_BEFORE_SCENARIO: [],
                         ACTIONS_AFTER_SCENARIO: [],
                         ACTIONS_AFTER_FEATURE: []}
@@ -208,105 +221,95 @@
                 self.logger.by_console(
                     "  ------------------ Scenario Nº: %d ------------------" % self.scenario_counter)
                 self.logger.by_console('  %s:' % action)
             elif action in [ACTIONS_BEFORE_FEATURE, ACTIONS_AFTER_FEATURE]:
                 self.logger.by_console('\n')
 
             for item in self.actions[action]:
-                self.scenario_error = False
                 try:
                     self.__print_step_by_console(item)
+                    self.logger.debug('Executing step defined in %s: %s' % (action, repr(item)))
                     context.execute_steps('''%s%s''' % (GIVEN_PREFIX, self.__remove_prefix(item)))
-                    self.logger.debug('step defined in pre-actions: %s' % repr(item))
                 except Exception as exc:
-                    self.feature_error = action in [ACTIONS_BEFORE_FEATURE]
-                    self.scenario_error = action in [ACTIONS_BEFORE_SCENARIO]
+                    if action == ACTIONS_BEFORE_FEATURE:
+                        self.feature_error = True
+                        self.before_error_message = exc
+                    elif action == ACTIONS_BEFORE_SCENARIO:
+                        self.scenario_error = True
+                        self.before_error_message = exc
                     self.logger.error(exc)
-                    self.error_exception = exc
                     break
 
-    def reset_error_status(self):
-        """
-        Check if the dyn_env has got any exception when executing the steps and restore the value of status to False.
-        :return: True if any exception has been raised when executing steps
-        """
-        try:
-            return self.feature_error or self.scenario_error
-        finally:
-            self.feature_error = False
-            self.scenario_error = False
-
     def execute_before_feature_steps(self, context):
         """
         actions before the feature
         :param context: It’s a clever place where you and behave can store information to share around,
                         automatically managed by behave.
         """
         self.__execute_steps_by_action(context, ACTIONS_BEFORE_FEATURE)
 
-        if context.dyn_env.feature_error:
-            # Mark this Feature as skipped. Steps will not be executed.
+        if self.feature_error:
+            # Mark this Feature as skipped to do not execute any Scenario
+            # Status will be changed to failed in after_feature method
             context.feature.mark_skipped()
 
     def execute_before_scenario_steps(self, context):
         """
         actions before each scenario
         :param context: It’s a clever place where you and behave can store information to share around,
                         automatically managed by behave.
         """
-        if not self.feature_error:
-            self.__execute_steps_by_action(context, ACTIONS_BEFORE_SCENARIO)
+        self.__execute_steps_by_action(context, ACTIONS_BEFORE_SCENARIO)
 
-        if context.dyn_env.scenario_error:
-            # Mark this Scenario as skipped. Steps will not be executed.
+        if self.scenario_error:
+            # Mark this Scenario as skipped to do not execute any step
+            # Status will be changed to failed in after_scenario method
             context.scenario.mark_skipped()
 
     def execute_after_scenario_steps(self, context):
         """
         actions after each scenario
         :param context: It’s a clever place where you and behave can store information to share around,
                         automatically managed by behave.
         """
-        if not self.feature_error:
-            self.__execute_steps_by_action(context, ACTIONS_AFTER_SCENARIO)
+        self.__execute_steps_by_action(context, ACTIONS_AFTER_SCENARIO)
 
-        # Behave dynamic environment: Fail all steps if dyn_env has got any error and reset it
-        if self.reset_error_status():
+        # Mark first step as failed when before_scenario has failed
+        if self.scenario_error:
+            error_message = self.before_error_message
+            self.scenario_error = False
+            self.before_error_message = None
             context.scenario.reset()
-            context.dyn_env.fail_first_step_precondition_exception(context.scenario)
+            self.fail_first_step_precondition_exception(context.scenario)
+            raise Exception(f'Before scenario steps have failed: {error_message}')
 
     def execute_after_feature_steps(self, context):
         """
         actions after the feature
         :param context: It’s a clever place where you and behave can store information to share around,
                         automatically managed by behave.
         """
         self.__execute_steps_by_action(context, ACTIONS_AFTER_FEATURE)
 
-        # Behave dynamic environment: Fail all steps if dyn_env has got any error and reset it
-        if self.reset_error_status():
+        # Mark first step of each scenario as failed when before_feature has failed
+        if self.feature_error:
+            error_message = self.before_error_message
+            self.feature_error = False
+            self.before_error_message = None
             context.feature.reset()
             for scenario in context.feature.walk_scenarios():
                 if scenario.should_run(context.config):
-                    context.dyn_env.fail_first_step_precondition_exception(scenario)
-            raise Exception("Preconditions failed during the execution")
+                    self.fail_first_step_precondition_exception(scenario)
+            raise Exception(f'Before feature steps have failed: {error_message}')
 
     def fail_first_step_precondition_exception(self, scenario):
         """
         Fail first step in the given Scenario and add exception message for the output.
         This is needed because xUnit exporter in Behave fails if there are not failed steps.
         :param scenario: Behave's Scenario
         """
-
-        try:
-            import behave
-            if parse_version(behave.__version__) < parse_version('1.2.6'):
-                status = 'failed'
-            else:
-                status = behave.model_core.Status.failed
-        except ImportError as exc:
-            self.logger.error(exc)
-            raise
-
-        scenario.steps[0].status = status
-        scenario.steps[0].exception = Exception("Preconditions failed")
-        scenario.steps[0].error_message = str(self.error_exception)
+        if len(scenario.steps) > 0:
+            # Behave is an optional dependency in toolium, so it is imported here
+            from behave.model_core import Status
+            scenario.steps[0].status = Status.failed
+            scenario.steps[0].exception = Exception('Preconditions failed')
+            scenario.steps[0].error_message = str(self.before_error_message)
```

### Comparing `toolium-3.0.1.dev2/toolium/behave/environment.py` & `toolium-3.0.2.dev0/toolium/behave/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,22 +68,23 @@
 
     # Start driver if it should be reused in feature
     context.reuse_driver_from_tags = 'reuse_driver' in feature.tags
     if context.toolium_config.getboolean_optional('Driver', 'reuse_driver') or context.reuse_driver_from_tags:
         no_driver = 'no_driver' in feature.tags
         start_driver(context, no_driver)
 
-    # Behave dynamic environment
-    context.dyn_env.get_steps_from_feature_description(feature.description)
-    context.dyn_env.execute_before_feature_steps(context)
     # Dictionary to store information between steps
     context.storage = dict()
     # Dictionary to store information between features
     context.feature_storage = dict()
 
+    # Behave dynamic environment
+    context.dyn_env.get_steps_from_feature_description(feature.description)
+    context.dyn_env.execute_before_feature_steps(context)
+
 
 def before_scenario(context, scenario):
     """Scenario initialization
 
     :param context: behave context
     :param scenario: running scenario
     """
@@ -203,33 +204,34 @@
 
 def after_scenario(context, scenario):
     """Clean method that will be executed after each scenario
 
     :param context: behave context
     :param scenario: running scenario
     """
+    jira_test_status = None
+    jira_test_comment = None
     if scenario.status == 'skipped':
         context.logger.info("The scenario '%s' has been skipped", scenario.name)
     elif scenario.status == 'passed':
-        test_status = 'Pass'
-        test_comment = None
+        jira_test_status = 'Pass'
         context.logger.info("The scenario '%s' has passed", scenario.name)
     else:
-        test_status = 'Fail'
-        test_comment = "The scenario '%s' has failed" % scenario.name
+        jira_test_status = 'Fail'
+        jira_test_comment = "The scenario '%s' has failed" % scenario.name
         context.logger.error("The scenario '%s' has failed", scenario.name)
         context.global_status['test_passed'] = False
 
     # Close drivers
     DriverWrappersPool.close_drivers(scope='function', test_name=scenario.name,
                                      test_passed=scenario.status in ['passed', 'skipped'], context=context)
 
     # Save test status to be updated later
-    if scenario.status != 'skipped':
-        add_jira_status(get_jira_key_from_scenario(scenario), test_status, test_comment)
+    if jira_test_status:
+        add_jira_status(get_jira_key_from_scenario(scenario), jira_test_status, jira_test_comment)
 
 
 def get_jira_key_from_scenario(scenario):
     """Extract Jira Test Case key from scenario tags.
     Two tag formats are allowed:
     @jira('PROJECT-32')
     @jira=PROJECT-32
```

### Comparing `toolium-3.0.1.dev2/toolium/config_driver.py` & `toolium-3.0.2.dev0/toolium/config_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
     def _add_chrome_additional_options(self, options):
         """Add Chrome additional options from properties file
 
         :param options: Chrome options object
         """
         chrome_options = self.config.get_optional('Chrome', 'options')
-        if options:
+        if chrome_options:
             try:
                 for key, value in ast.literal_eval(chrome_options).items():
                     self.logger.debug("Added Chrome additional option: %s = %s", key, value)
                     options.add_experimental_option(key, value)
             except Exception as exc:
                 self.logger.warning(f'Chrome options "{chrome_options}" can not be added: {exc}')
```

### Comparing `toolium-3.0.1.dev2/toolium/config_files.py` & `toolium-3.0.2.dev0/toolium/config_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/config_parser.py` & `toolium-3.0.2.dev0/toolium/config_parser.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/driver_wrapper.py` & `toolium-3.0.2.dev0/toolium/driver_wrapper.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/driver_wrappers_pool.py` & `toolium-3.0.2.dev0/toolium/driver_wrappers_pool.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/jira.py` & `toolium-3.0.2.dev0/toolium/jira.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/__init__.py` & `toolium-3.0.2.dev0/toolium/pageelements/__init__.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/button_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/button_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/checkbox_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/checkbox_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/group_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/group_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/input_radio_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/input_radio_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/input_text_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/input_text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/link_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/link_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/page_elements.py` & `toolium-3.0.2.dev0/toolium/pageelements/page_elements.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/select_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/select_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageelements/text_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageobjects/common_object.py` & `toolium-3.0.2.dev0/toolium/pageobjects/common_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageobjects/mobile_page_object.py` & `toolium-3.0.2.dev0/toolium/pageobjects/mobile_page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pageobjects/page_object.py` & `toolium-3.0.2.dev0/toolium/pageobjects/page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/pytest_fixtures.py` & `toolium-3.0.2.dev0/toolium/pytest_fixtures.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/resources/VisualTests.css` & `toolium-3.0.2.dev0/toolium/resources/VisualTests.css`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/resources/VisualTests.js` & `toolium-3.0.2.dev0/toolium/resources/VisualTests.js`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/resources/VisualTestsTemplate.html` & `toolium-3.0.2.dev0/toolium/resources/VisualTestsTemplate.html`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/selenoid.py` & `toolium-3.0.2.dev0/toolium/selenoid.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/test_cases.py` & `toolium-3.0.2.dev0/toolium/test_cases.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,16 @@
         error_message = ''
         if hasattr(self._outcome, 'errors') and len(self._outcome.errors) > 0:
             # Python <3.11
             exception_info = self._outcome.errors[-1][1]
             if exception_info:
                 exception = exception_info[1]
                 error_message = get_error_message_from_exception(exception)
-        elif not hasattr(self._outcome, 'errors') and len(self._outcome.result.failures) > 0:
+        elif not hasattr(self._outcome, 'errors') and hasattr(self._outcome.result, 'failures') \
+                and len(self._outcome.result.failures) > 0:
             # Python 3.11
             traceback = self._outcome.result.failures[0][1]
             error_message = get_error_message_from_traceback(traceback)
 
         # Change test status
         if not error_message:
             self._test_passed = True
```

### Comparing `toolium-3.0.1.dev2/toolium/utils/data_generator.py` & `toolium-3.0.2.dev0/toolium/utils/data_generator.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/utils/dataset.py` & `toolium-3.0.2.dev0/toolium/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/utils/download_files.py` & `toolium-3.0.2.dev0/toolium/utils/download_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/utils/driver_utils.py` & `toolium-3.0.2.dev0/toolium/utils/driver_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/utils/driver_wait_utils.py` & `toolium-3.0.2.dev0/toolium/utils/driver_wait_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/utils/path_utils.py` & `toolium-3.0.2.dev0/toolium/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/utils/poeditor.py` & `toolium-3.0.2.dev0/toolium/utils/poeditor.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium/visual_test.py` & `toolium-3.0.2.dev0/toolium/visual_test.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.1.dev2/toolium.egg-info/PKG-INFO` & `toolium-3.0.2.dev0/toolium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.1.dev2
+Version: 3.0.2.dev0
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.1.dev2/toolium.egg-info/SOURCES.txt` & `toolium-3.0.2.dev0/toolium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

