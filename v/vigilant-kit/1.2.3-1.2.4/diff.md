# Comparing `tmp/vigilant_kit-1.2.3.tar.gz` & `tmp/vigilant_kit-1.2.4.tar.gz`

## Comparing `vigilant_kit-1.2.3.tar` & `vigilant_kit-1.2.4.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/.vigilant.env.example
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/bin/doc_generator.py
--rw-r--r--   0        0        0    28724 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/actions.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/browser_options.md
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/native_selenium.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/selenium_install.md
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/tutorial_pytest.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/vigilant_pytest.md
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/vigilant_unittest.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vgl_cli/install_dev_kit_command.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vgl_cli/install_standalone_command.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vgl_cli/install_webdriver_command.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vgl_cli/run_selenium_command.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vgl_cli/vgl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/actions/__init__.py
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/actions/assertions.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/actions/finder.py
--rw-r--r--   0        0        0    11684 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/actions/vigilant_actions.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/actions/waiter.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/driver/__init__.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/driver/vigilant_driver.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/.gitignore
--rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/LICENSE
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/.vigilant.env.example
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/vigilant.json.example
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/bin/doc_generator.py
+-rw-r--r--   0        0        0    28724 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/docs/actions.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/docs/browser_options.md
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/docs/configuration.md
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/docs/native_selenium.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/docs/selenium_install.md
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/docs/tutorial_pytest.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/docs/vigilant_pytest.md
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/docs/vigilant_unittest.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vgl_cli/install_dev_kit_command.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vgl_cli/install_standalone_command.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vgl_cli/install_webdriver_command.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vgl_cli/run_selenium_command.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vgl_cli/vgl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vigilant/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vigilant/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vigilant/actions/__init__.py
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vigilant/actions/assertions.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vigilant/actions/finder.py
+-rw-r--r--   0        0        0    11684 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vigilant/actions/vigilant_actions.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vigilant/actions/waiter.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vigilant/driver/__init__.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/src/vigilant/driver/vigilant_driver.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/.gitignore
+-rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/LICENSE
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 vigilant_kit-1.2.4/PKG-INFO
```

### Comparing `vigilant_kit-1.2.3/bin/doc_generator.py` & `vigilant_kit-1.2.4/bin/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/docs/actions.md` & `vigilant_kit-1.2.4/docs/actions.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/docs/browser_options.md` & `vigilant_kit-1.2.4/docs/browser_options.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/docs/native_selenium.md` & `vigilant_kit-1.2.4/docs/native_selenium.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/docs/selenium_install.md` & `vigilant_kit-1.2.4/docs/selenium_install.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/docs/tutorial_pytest.md` & `vigilant_kit-1.2.4/docs/tutorial_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/docs/vigilant_pytest.md` & `vigilant_kit-1.2.4/docs/vigilant_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/docs/vigilant_unittest.md` & `vigilant_kit-1.2.4/docs/vigilant_unittest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/src/vgl_cli/install_dev_kit_command.py` & `vigilant_kit-1.2.4/src/vgl_cli/install_dev_kit_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/src/vgl_cli/install_standalone_command.py` & `vigilant_kit-1.2.4/src/vgl_cli/install_standalone_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/src/vgl_cli/install_webdriver_command.py` & `vigilant_kit-1.2.4/src/vgl_cli/install_webdriver_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/src/vgl_cli/run_selenium_command.py` & `vigilant_kit-1.2.4/src/vgl_cli/run_selenium_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/src/vgl_cli/vgl.py` & `vigilant_kit-1.2.4/src/vgl_cli/vgl.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/src/vigilant/actions/assertions.py` & `vigilant_kit-1.2.4/src/vigilant/actions/assertions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/src/vigilant/actions/finder.py` & `vigilant_kit-1.2.4/src/vigilant/actions/finder.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/src/vigilant/actions/vigilant_actions.py` & `vigilant_kit-1.2.4/src/vigilant/actions/vigilant_actions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/src/vigilant/actions/waiter.py` & `vigilant_kit-1.2.4/src/vigilant/actions/waiter.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/src/vigilant/driver/vigilant_driver.py` & `vigilant_kit-1.2.4/src/vigilant/driver/vigilant_driver.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/.gitignore` & `vigilant_kit-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/LICENSE` & `vigilant_kit-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.3/README.md` & `vigilant_kit-1.2.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -25,17 +25,22 @@
 
 ## Install
 ```shell
 pip install vigilant-kit
 ```
 
 ## Docs
- - [How to install Selenium server & browser drivers](docs/selenium_install.md)
- - [Quick start example using `unittest` library](docs/vigilant_unittest.md) 
- - [Quick start example using `pytest`](docs/vigilant_pytest.md) 
- - [How to add custom browser options](docs/browser_options.md)
- - [Access native Selenium WebDriver methods](docs/native_selenium.md)
- - [List of actions](docs/actions.md).
+### Install
+- [How to install Selenium server & browser drivers](docs/selenium_install.md)
 
-## Tutorials
- - [Testing ecommerce project using `vigilant-kit` and `pytest`](docs/tutorial_pytest.md)
- 
+### Configuration
+- [Vigilant configuration](docs/configuration.md)
+- [How to add custom browser options](docs/browser_options.md)
+- [Access native Selenium WebDriver methods](docs/native_selenium.md)
+
+### Examples & tutorials
+- [Quick start example using `unittest` library](docs/vigilant_unittest.md) 
+- [Quick start example using `pytest`](docs/vigilant_pytest.md) 
+- [Testing ecommerce project using `vigilant-kit` and `pytest`](docs/tutorial_pytest.md)
+
+### Actions
+- [List of actions](docs/actions.md)
```

### Comparing `vigilant_kit-1.2.3/pyproject.toml` & `vigilant_kit-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vigilant_kit"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="Pelykh Ivan", email="ivan.pelykh@protonmail.com" },
 ]
 description = "Library that makes functional testing with Selenium WebDriver fast and easy. "
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `vigilant_kit-1.2.3/PKG-INFO` & `vigilant_kit-1.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vigilant_kit
-Version: 1.2.3
+Version: 1.2.4
 Summary: Library that makes functional testing with Selenium WebDriver fast and easy. 
 Project-URL: Homepage, https://github.com/ivpel/vigilant
 Project-URL: Bug Tracker, https://github.com/ivpel/vigilant/issues
 Author-email: Pelykh Ivan <ivan.pelykh@protonmail.com>
 License-File: LICENSE
 Keywords: bdd,functional,functional-testing,pytest,selenium,tdd,testing,unittest,webdriver
 Requires-Python: >=3.7
@@ -41,17 +41,22 @@
 
 ## Install
 ```shell
 pip install vigilant-kit
 ```
 
 ## Docs
- - [How to install Selenium server & browser drivers](docs/selenium_install.md)
- - [Quick start example using `unittest` library](docs/vigilant_unittest.md) 
- - [Quick start example using `pytest`](docs/vigilant_pytest.md) 
- - [How to add custom browser options](docs/browser_options.md)
- - [Access native Selenium WebDriver methods](docs/native_selenium.md)
- - [List of actions](docs/actions.md).
-
-## Tutorials
- - [Testing ecommerce project using `vigilant-kit` and `pytest`](docs/tutorial_pytest.md)
- 
+### Install
+- [How to install Selenium server & browser drivers](docs/selenium_install.md)
+
+### Configuration
+- [Vigilant configuration](docs/configuration.md)
+- [How to add custom browser options](docs/browser_options.md)
+- [Access native Selenium WebDriver methods](docs/native_selenium.md)
+
+### Examples & tutorials
+- [Quick start example using `unittest` library](docs/vigilant_unittest.md) 
+- [Quick start example using `pytest`](docs/vigilant_pytest.md) 
+- [Testing ecommerce project using `vigilant-kit` and `pytest`](docs/tutorial_pytest.md)
+
+### Actions
+- [List of actions](docs/actions.md)
```

