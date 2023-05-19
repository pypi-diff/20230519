# Comparing `tmp/alfred-cli-1.2.0.tar.gz` & `tmp/alfred_cli-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred-cli-1.2.0.tar", last modified: Sat Nov 12 07:58:12 2022, max compression
+gzip compressed data, was "alfred_cli-2.0.0b1.tar", max compression
```

## Comparing `alfred-cli-1.2.0.tar` & `alfred_cli-2.0.0b1.tar`

### file list

```diff
@@ -1,29 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 07:58:12.565201 alfred-cli-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11124 2022-11-12 07:58:12.565201 alfred-cli-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10500 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-11-12 07:58:12.565201 alfred-cli-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 07:58:12.561200 alfred-cli-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 07:58:12.565201 alfred-cli-1.2.0/src/alfred/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4245 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/lib.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     8149 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/os.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 07:58:12.565201 alfred-cli-1.2.0/src/alfred/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/resources/cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-11-12 07:57:29.000000 alfred-cli-1.2.0/src/alfred/type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 07:58:12.565201 alfred-cli-1.2.0/src/alfred_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11124 2022-11-12 07:58:12.000000 alfred-cli-1.2.0/src/alfred_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-11-12 07:58:12.000000 alfred-cli-1.2.0/src/alfred_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 07:58:12.000000 alfred-cli-1.2.0/src/alfred_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-11-12 07:58:12.000000 alfred-cli-1.2.0/src/alfred_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-12 07:58:12.000000 alfred-cli-1.2.0/src/alfred_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-12 07:58:12.000000 alfred-cli-1.2.0/src/alfred_cli.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1072 2023-05-18 12:57:42.409315 alfred_cli-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0     9788 2023-05-18 12:57:42.409315 alfred_cli-2.0.0b1/README.md
+-rw-r--r--   0        0        0     1584 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      284 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/__init__.py
+-rw-r--r--   0        0        0     1483 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/alfred_command.py
+-rw-r--r--   0        0        0     5118 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/cli.py
+-rw-r--r--   0        0        0     4636 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/commands.py
+-rw-r--r--   0        0        0     3406 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/ctx.py
+-rw-r--r--   0        0        0      682 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/decorator.py
+-rw-r--r--   0        0        0        0 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/domain/__init__.py
+-rw-r--r--   0        0        0     2404 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/domain/command.py
+-rw-r--r--   0        0        0     1470 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/domain/manifest.py
+-rw-r--r--   0        0        0      605 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/echo.py
+-rw-r--r--   0        0        0      590 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/exceptions.py
+-rw-r--r--   0        0        0     1267 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/interpreter.py
+-rw-r--r--   0        0        0     2308 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/lib.py
+-rw-r--r--   0        0        0      208 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/logger.py
+-rw-r--r--   0        0        0     9418 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/main.py
+-rw-r--r--   0        0        0     7872 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/manifest.py
+-rw-r--r--   0        0        0      619 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/os.py
+-rw-r--r--   0        0        0        9 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/resources/.alfred.toml
+-rw-r--r--   0        0        0        0 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/resources/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-18 12:57:42.413315 alfred_cli-2.0.0b1/src/alfred/resources/cmd.py
+-rw-r--r--   0        0        0    11178 1970-01-01 00:00:00.000000 alfred_cli-2.0.0b1/PKG-INFO
```

### Comparing `alfred-cli-1.2.0/LICENSE` & `alfred_cli-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred-cli-1.2.0/PKG-INFO` & `alfred_cli-2.0.0b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,76 @@
 Metadata-Version: 2.1
 Name: alfred-cli
-Version: 1.2.0
-Summary: alfred is a building tool to make engineering tasks easier to develop and to maintain
+Version: 2.0.0b1
+Summary: alfred is an extensible building tool that can replace a Makefile or Fabric. Writing commands in python is done in minutes.
 Home-page: https://github.com/FabienArcellier/alfred-cli#alfred
 License: MIT
-Project-URL: Source, https://github.com/FabienArcellier/alfred-cli
-Classifier: Programming Language :: Python :: 3
+Keywords: building tool,makefile,productivity,automation,continuous integration,developper friendly
+Author: Fabien Arcellier
+Author-email: fabien.arcellier@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: plumbum (>=1.8.1,<2.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Documentation, https://alfred-cli.readthedocs.io/en/latest
+Project-URL: Repository, https://github.com/FabienArcellier/alfred-cli
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
 
 ## Alfred
 
 Alfred is an extensible building tool that can replace a Makefile or Fabric.
-Writing commands in python is done in a few minutes, even in the case of a mono-repository
-which contains several products.
-
-In this dev, we are eating our own dog food. We are using `alfred` for the continuous integration process
-of itself instead of `Makefile` as I usually do.
+Writing commands in python is done in a few minutes, even in the case of a mono-repository.
 
 ```bash
-# run the continuous integration process
+# use alfred to run continuous integration process
 alfred ci
 
-# publish the package on pypi
+# use alfred to publish a package on pypi
 alfred publish
 ```
 
 [![version](https://img.shields.io/pypi/v/alfred-cli.svg?label=version)](https://pypi.org/project/alfred-cli/) [![MIT](https://img.shields.io/badge/license-MIT-007EC7.svg)](LICENSE.md)
 
 [![ci](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci.yml/badge.svg)](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci.yml) [![ci-windows](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci-windows.yml/badge.svg)](https://github.com/FabienArcellier/pyalfred/actions/workflows/ci-windows.yml)
 
+<!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->
+
 - [Getting started](#getting-started)
-  * [Add your own command](#add-your-own-command)
+- [Links](#links)
+- [Cookbook](#cookbook)
+  * [Add a new build command](#add-a-new-build-command)
 - [Behind the scene](#behind-the-scene)
 - [Why using alfred instead of Makefile or Bash scripts](#why-using-alfred-instead-of-makefile-or-bash-scripts)
 - [Why not using alfred](#why-not-using-alfred)
 - [The latest version](#the-latest-version)
-- [Reference](#reference)
-  * [`.Alfred.yml`](#-alfredyml-)
-    + [`Plugins` section](#-plugins--section)
-    + [`Environment` section](#-environment--section)
-- [Cookbook](#cookbook)
+- [Cookbook](#cookbook-1)
   * [Display the commands really executed behind the scene](#display-the-commands-really-executed-behind-the-scene)
   * [Customize a command for a specific OS](#customize-a-command-for-a-specific-os)
+  * [Override environment variables](#override-environment-variables)
+    + [Add directories into pythonpath](#add-directories-into-pythonpath)
 - [Developper guideline](#developper-guideline)
-  * [Install development environment](#install-development-environment)
-  * [Install production environment](#install-production-environment)
-  * [Initiate or update the library requirements](#initiate-or-update-the-library-requirements)
-  * [Activate the python environment](#activate-the-python-environment)
   * [Run the linter and the unit tests](#run-the-linter-and-the-unit-tests)
 - [Contributors](#contributors)
 - [License](#license)
 
+<!-- TOC end -->
+
 ## Getting started
 
 To configure a python project to use alfred, here is the procedure:
 
 ```bash
 pip3 install alfred-cli
 alfred init
@@ -71,37 +80,42 @@
 
 ```bash
 alfred hello_world --name "Fabien"
 ```
 
 A file `.alfred.yml` will be initialized at the root of the repository.
 
-### Add a new build command
+## Links
+
+* Documentation : https://alfred-cli.readthedocs.io/en/latest
+* PyPI Release : https://pypi.org/project/alfred-cli
+* Source code: https://github.com/FabienArcellier/alfred-cli
+* Chat: https://discord.gg/nMn9YPRGSY
+
+## Cookbook
+
+### Add a new command
 
 You can add your command in a new module in `./alfred`.
 In this example we will add the command `alfred lint` :
 
 ```python
 import os
 
 import alfred
 
 ROOT_DIR = os.path.realpath(os.path.join(__file__, "..", ".."))
 
-
 @alfred.command('lint', help="validate alfred using pylint on the package alfred")
 def lint():
     # get the command pylint in the user system or show error message if it's missing
     pylint = alfred.sh('pylint', "pylint is not installed")
-    os.chdir(ROOT_DIR)
-    src_dir = "src/alfred"
-    args = [src_dir]
 
     # behind the scene, it invokes the command `pylint alfred`
-    alfred.run(pylint, args)
+    alfred.run(pylint, ["src/alfred"])
 ```
 
 ## Behind the scene
 
 Alfred rely heavily on click and plumblum :
 
 * [click](https://click.palletsprojects.com/en/8.0.x/)
@@ -141,55 +155,14 @@
 
 You can find the latest version to ...
 
 ```bash
 git clone https://github.com/FabienArcellier/alfred-cli.git
 ```
 
-## Reference
-
-### `.Alfred.yml`
-
-The configuration file supports several attributes to tune the behavior of
-Alfred. It is required to add
-
-#### `Plugins` section
-
-the `plugins` section tells Alfred where to look for commands to render
-accessible to the user. The pointed folder contains several python modules which
-are loaded one by one. The `__init __. Py` module is ignored.
-
-If you specify a prefix, the commands configured in the imported modules
-will be prefixed by this label in alfred. This feature is useful in a mono-repository
-when you want to have an .alfred.yml file for each project and an .alfred.yml file
-at the root of the project.
-
-```yaml
-plugins:
-    - path: alfred
-
-    - path: sofware1/alfred
-      prefix: "software1:"
-```
-
-#### `Environment` section
-
-`environment` section allows you to hard configure environment variables to load
-before executing a command.
-
-This feature facilitates the integration with `pipenv` for example which has a behavior
-different between mac and linux. In this case, it allows you to set the necessary flags
-to erase these differences.
-
-```yaml
-environment:
-    - "VAR=1"
-    - "VAR"
-```
-
 ## Cookbook
 
 ### Display the commands really executed behind the scene
 
 You can display the commands really executed, either to debug the arguments,
 either to run in your terminal again with other attributes.
 
@@ -223,19 +196,62 @@
 
     alfred.invoke_command('tests', verbose=verbose)
 ```
 
 the ``alfred.is_posix``, ``alfred.is_linux``, ``alfred.is_macos``, ``alfred.is_windows`` functions allow you to quickly
 target the environment on which specific processing must be performed.
 
+### Override environment variables
+
+```python
+@alfred.command('ci', help="execute continuous integration process of alfred")
+def ci():
+    with alfred.env(SCREEN="display"):
+        bash = alfred.sh("bash")
+        bash.run("-c" "echo $SCREEN")
+```
+
+#### Add directories into pythonpath
+
+Adding a folder in the pythonpath variable allows you to expose packages without declaring them in the manifest.
+
+This pattern is useful with poetry to be able to reuse the code of the package tests in this one for example.
+
+The ``alfred.pythonpath`` decorator adds the project root. You can save specific folders here.
+
+```python
+@alfred.command('ci', help="execute continuous integration process of alfred")
+@alfred.pythonpath()
+def ci():
+    bash = alfred.sh("bash")
+    alfred.run(bash, ["-c" "echo $SCREEN"])
+```
+
+```python
+@alfred.command('ci', help="execute continuous integration process of alfred")
+@alfred.pythonpath(['tests'], append_project=False)
+def ci():
+    bash = alfred.sh("bash")
+    alfred.run(bash, ["-c", "echo $SCREEN"])
+```
+
+```python
+@alfred.command('ci', help="execute continuous integration process of alfred")
+def ci():
+    with alfred.pythonpath():
+        bash = alfred.sh("bash")
+        alfred.run(bash, ["-c", "echo $SCREEN"])
+```
+
+
 ## Developper guideline
 
 ```bash
-pipenv install
-pipenv shell
+poetry install
+poetry shell
 ```
 
 ```
 $ alfred
 Usage: alfred [OPTIONS] COMMAND [ARGS]...
 
   alfred is a building tool to make engineering tasks easier to develop and to
@@ -252,47 +268,14 @@
   lint               validate alfred using pylint on the package alfred
   publish            tag a new release and trigger pypi publication
   tests              validate alfred with all the automatic testing
   tests:acceptances  validate alfred with acceptances testing
   tests:units        validate alfred with unit testing
 ```
 
-### Install development environment
-
-Use make to instanciate a python virtual environment in ./venv and install the
-python dependencies.
-
-```bash
-pipenv install --dev
-```
-
-### Install production environment
-
-```bash
-pipenv install
-```
-
-### Initiate or update the library requirements
-
-If you want to initiate or update all the requirements `install_requires` declared in `setup.py`
-and freeze a new `Pipfile.lock`, use this command
-
-```bash
-pipenv update
-```
-
-### Activate the python environment
-
-When you setup the requirements, a `venv` directory on python 3 is created.
-To activate the venv, you have to execute :
-
-```bash
-pipenv shell
-```
-
 ### Run the linter and the unit tests
 
 Before commit or send a pull request, you have to execute `pylint` to check the syntax
 of your code and run the unit tests to validate the behavior.
 
 ```bash
 alfred ci
@@ -302,15 +285,15 @@
 
 * Fabien Arcellier
 
 ## License
 
 MIT License
 
-Copyright (c) 2021-2022 Fabien Arcellier
+Copyright (c) 2021-2023 Fabien Arcellier
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -321,7 +304,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
```

### Comparing `alfred-cli-1.2.0/README.md` & `alfred_cli-2.0.0b1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 ## Alfred
 
 Alfred is an extensible building tool that can replace a Makefile or Fabric.
-Writing commands in python is done in a few minutes, even in the case of a mono-repository
-which contains several products.
-
-In this dev, we are eating our own dog food. We are using `alfred` for the continuous integration process
-of itself instead of `Makefile` as I usually do.
+Writing commands in python is done in a few minutes, even in the case of a mono-repository.
 
 ```bash
-# run the continuous integration process
+# use alfred to run continuous integration process
 alfred ci
 
-# publish the package on pypi
+# use alfred to publish a package on pypi
 alfred publish
 ```
 
 [![version](https://img.shields.io/pypi/v/alfred-cli.svg?label=version)](https://pypi.org/project/alfred-cli/) [![MIT](https://img.shields.io/badge/license-MIT-007EC7.svg)](LICENSE.md)
 
 [![ci](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci.yml/badge.svg)](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci.yml) [![ci-windows](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci-windows.yml/badge.svg)](https://github.com/FabienArcellier/pyalfred/actions/workflows/ci-windows.yml)
 
+<!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->
+
 - [Getting started](#getting-started)
-  * [Add your own command](#add-your-own-command)
+- [Links](#links)
+- [Cookbook](#cookbook)
+  * [Add a new build command](#add-a-new-build-command)
 - [Behind the scene](#behind-the-scene)
 - [Why using alfred instead of Makefile or Bash scripts](#why-using-alfred-instead-of-makefile-or-bash-scripts)
 - [Why not using alfred](#why-not-using-alfred)
 - [The latest version](#the-latest-version)
-- [Reference](#reference)
-  * [`.Alfred.yml`](#-alfredyml-)
-    + [`Plugins` section](#-plugins--section)
-    + [`Environment` section](#-environment--section)
-- [Cookbook](#cookbook)
+- [Cookbook](#cookbook-1)
   * [Display the commands really executed behind the scene](#display-the-commands-really-executed-behind-the-scene)
   * [Customize a command for a specific OS](#customize-a-command-for-a-specific-os)
+  * [Override environment variables](#override-environment-variables)
+    + [Add directories into pythonpath](#add-directories-into-pythonpath)
 - [Developper guideline](#developper-guideline)
-  * [Install development environment](#install-development-environment)
-  * [Install production environment](#install-production-environment)
-  * [Initiate or update the library requirements](#initiate-or-update-the-library-requirements)
-  * [Activate the python environment](#activate-the-python-environment)
   * [Run the linter and the unit tests](#run-the-linter-and-the-unit-tests)
 - [Contributors](#contributors)
 - [License](#license)
 
+<!-- TOC end -->
+
 ## Getting started
 
 To configure a python project to use alfred, here is the procedure:
 
 ```bash
 pip3 install alfred-cli
 alfred init
@@ -54,37 +50,42 @@
 
 ```bash
 alfred hello_world --name "Fabien"
 ```
 
 A file `.alfred.yml` will be initialized at the root of the repository.
 
-### Add a new build command
+## Links
+
+* Documentation : https://alfred-cli.readthedocs.io/en/latest
+* PyPI Release : https://pypi.org/project/alfred-cli
+* Source code: https://github.com/FabienArcellier/alfred-cli
+* Chat: https://discord.gg/nMn9YPRGSY
+
+## Cookbook
+
+### Add a new command
 
 You can add your command in a new module in `./alfred`.
 In this example we will add the command `alfred lint` :
 
 ```python
 import os
 
 import alfred
 
 ROOT_DIR = os.path.realpath(os.path.join(__file__, "..", ".."))
 
-
 @alfred.command('lint', help="validate alfred using pylint on the package alfred")
 def lint():
     # get the command pylint in the user system or show error message if it's missing
     pylint = alfred.sh('pylint', "pylint is not installed")
-    os.chdir(ROOT_DIR)
-    src_dir = "src/alfred"
-    args = [src_dir]
 
     # behind the scene, it invokes the command `pylint alfred`
-    alfred.run(pylint, args)
+    alfred.run(pylint, ["src/alfred"])
 ```
 
 ## Behind the scene
 
 Alfred rely heavily on click and plumblum :
 
 * [click](https://click.palletsprojects.com/en/8.0.x/)
@@ -124,55 +125,14 @@
 
 You can find the latest version to ...
 
 ```bash
 git clone https://github.com/FabienArcellier/alfred-cli.git
 ```
 
-## Reference
-
-### `.Alfred.yml`
-
-The configuration file supports several attributes to tune the behavior of
-Alfred. It is required to add
-
-#### `Plugins` section
-
-the `plugins` section tells Alfred where to look for commands to render
-accessible to the user. The pointed folder contains several python modules which
-are loaded one by one. The `__init __. Py` module is ignored.
-
-If you specify a prefix, the commands configured in the imported modules
-will be prefixed by this label in alfred. This feature is useful in a mono-repository
-when you want to have an .alfred.yml file for each project and an .alfred.yml file
-at the root of the project.
-
-```yaml
-plugins:
-    - path: alfred
-
-    - path: sofware1/alfred
-      prefix: "software1:"
-```
-
-#### `Environment` section
-
-`environment` section allows you to hard configure environment variables to load
-before executing a command.
-
-This feature facilitates the integration with `pipenv` for example which has a behavior
-different between mac and linux. In this case, it allows you to set the necessary flags
-to erase these differences.
-
-```yaml
-environment:
-    - "VAR=1"
-    - "VAR"
-```
-
 ## Cookbook
 
 ### Display the commands really executed behind the scene
 
 You can display the commands really executed, either to debug the arguments,
 either to run in your terminal again with other attributes.
 
@@ -206,19 +166,62 @@
 
     alfred.invoke_command('tests', verbose=verbose)
 ```
 
 the ``alfred.is_posix``, ``alfred.is_linux``, ``alfred.is_macos``, ``alfred.is_windows`` functions allow you to quickly
 target the environment on which specific processing must be performed.
 
+### Override environment variables
+
+```python
+@alfred.command('ci', help="execute continuous integration process of alfred")
+def ci():
+    with alfred.env(SCREEN="display"):
+        bash = alfred.sh("bash")
+        bash.run("-c" "echo $SCREEN")
+```
+
+#### Add directories into pythonpath
+
+Adding a folder in the pythonpath variable allows you to expose packages without declaring them in the manifest.
+
+This pattern is useful with poetry to be able to reuse the code of the package tests in this one for example.
+
+The ``alfred.pythonpath`` decorator adds the project root. You can save specific folders here.
+
+```python
+@alfred.command('ci', help="execute continuous integration process of alfred")
+@alfred.pythonpath()
+def ci():
+    bash = alfred.sh("bash")
+    alfred.run(bash, ["-c" "echo $SCREEN"])
+```
+
+```python
+@alfred.command('ci', help="execute continuous integration process of alfred")
+@alfred.pythonpath(['tests'], append_project=False)
+def ci():
+    bash = alfred.sh("bash")
+    alfred.run(bash, ["-c", "echo $SCREEN"])
+```
+
+```python
+@alfred.command('ci', help="execute continuous integration process of alfred")
+def ci():
+    with alfred.pythonpath():
+        bash = alfred.sh("bash")
+        alfred.run(bash, ["-c", "echo $SCREEN"])
+```
+
+
 ## Developper guideline
 
 ```bash
-pipenv install
-pipenv shell
+poetry install
+poetry shell
 ```
 
 ```
 $ alfred
 Usage: alfred [OPTIONS] COMMAND [ARGS]...
 
   alfred is a building tool to make engineering tasks easier to develop and to
@@ -235,47 +238,14 @@
   lint               validate alfred using pylint on the package alfred
   publish            tag a new release and trigger pypi publication
   tests              validate alfred with all the automatic testing
   tests:acceptances  validate alfred with acceptances testing
   tests:units        validate alfred with unit testing
 ```
 
-### Install development environment
-
-Use make to instanciate a python virtual environment in ./venv and install the
-python dependencies.
-
-```bash
-pipenv install --dev
-```
-
-### Install production environment
-
-```bash
-pipenv install
-```
-
-### Initiate or update the library requirements
-
-If you want to initiate or update all the requirements `install_requires` declared in `setup.py`
-and freeze a new `Pipfile.lock`, use this command
-
-```bash
-pipenv update
-```
-
-### Activate the python environment
-
-When you setup the requirements, a `venv` directory on python 3 is created.
-To activate the venv, you have to execute :
-
-```bash
-pipenv shell
-```
-
 ### Run the linter and the unit tests
 
 Before commit or send a pull request, you have to execute `pylint` to check the syntax
 of your code and run the unit tests to validate the behavior.
 
 ```bash
 alfred ci
@@ -285,15 +255,15 @@
 
 * Fabien Arcellier
 
 ## License
 
 MIT License
 
-Copyright (c) 2021-2022 Fabien Arcellier
+Copyright (c) 2021-2023 Fabien Arcellier
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `alfred-cli-1.2.0/src/alfred/lib.py` & `alfred_cli-2.0.0b1/src/alfred/lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+import contextlib
+import glob
 import io
 import os
 import sys
 from typing import List, Iterator
 
-import click
+from plumbum import local
 
-from alfred.type import path
+from alfred.logger import get_logger
 
 ROOT_DIR = os.path.realpath(os.path.join(__file__, '..'))
 
 
 class InvalidPythonModule(Exception):
     pass
 
 
-def import_python(python_path: path) -> dict:
+def import_python(python_path: str) -> dict:
 
     module = {"__file__": python_path}
     with io.open(python_path, encoding="utf8") as file:
         content = file.read()
         try:
             code = compile(content, python_path, 'exec')
             eval(code, module, module)  # pylint: disable=eval-used
@@ -31,31 +33,49 @@
             raise InvalidPythonModule(f"""Invalid command module : "{python_path}", Line {line}
   {rows[line - 1]}\n
   {exc_type.__name__} : {exception}\n""") from exception
 
     return module
 
 
-def list_python_modules(folder_path: path) -> Iterator[path]:
-    for filename in os.listdir(folder_path):
+def list_python_modules(glob_expression: str) -> Iterator[str]:
+    for filename in glob.glob(glob_expression):
         if filename.endswith('.py') and filename != '__init__.py':
-            python_path = path(os.path.join(folder_path, filename))
-            yield python_path
+            yield filename
 
 
-def list_hierarchy_directory(workingdir: path) -> List[path]:
+def list_hierarchy_directory(workingdir: str) -> List[str]:
     workingdir = os.path.realpath(workingdir)
     all_parts = workingdir.split(os.sep)
 
     result = [workingdir]
     while len(all_parts) != 1:
         all_parts.pop()
         if len(all_parts) == 1:
             result.append(os.sep)
         else:
             result.append(os.sep.join(all_parts))
 
     return result
 
 
-def print_error(msg: str):
-    click.echo(click.style(msg, fg="red", bold=True), err=True)
+@contextlib.contextmanager
+def override_pythonpath(pythonpath: str):
+    """
+    Override the pythonpath variable in a generalized way
+
+    * override the environment variable in python
+    * override pythonpath environment variable in plumbum
+    * override sys.path
+    """
+    logger = get_logger()
+    logger.debug(f"override PYTHONPATH: {pythonpath}")
+
+    previous_pythonpath = os.getenv('PYTHONPATH', '')
+    with local.env(PYTHONPATH=pythonpath):
+        os.environ['PYTHONPATH'] = pythonpath
+        sys.path = pythonpath.split(':')
+        try:
+            yield
+        finally:
+            os.environ['PYTHONPATH'] = previous_pythonpath
+            sys.path = previous_pythonpath.split(':')
```

### Comparing `alfred-cli-1.2.0/src/alfred/main.py` & `alfred_cli-2.0.0b1/src/alfred/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-import io
+import contextlib
 import os
-from typing import Optional, Union, List
+from functools import wraps
+from typing import Union, List, Callable
 
 import click
 import plumbum
-import yaml
-from click import BaseCommand
 from click.exceptions import Exit
-from plumbum import CommandNotFound, ProcessExecutionError, FG
+from plumbum import CommandNotFound, ProcessExecutionError, FG, local
 from plumbum.machines import LocalCommand
-from yaml import SafeLoader
 
-from alfred.decorator import ALFRED_COMMANDS
-from alfred.exceptions import NotInitialized
-from alfred.lib import list_hierarchy_directory
-from alfred.logger import logger
-from alfred.type import path, AlfredConfiguration
+from alfred import ctx as alfred_ctx, commands, echo, lib, manifest, alfred_command
+from alfred.logger import get_logger
 
 
 def call(command: LocalCommand, args: [str], exit_on_error=True) -> str:  #pylint: disable=inconsistent-return-statements
     """
     Most of the process run by alfred are supposed to stop
     if the excecution process is finishing with an exit code of 0
 
@@ -32,14 +27,15 @@
     >>> # show `hello world`
 
 
     :param command: shell program to execute
     :param exit_on_error: break the flow if the exit code is different of 0 (active by default)
     """
     try:
+        logger = get_logger()
         complete_command = command[args]
         working_directory = os.getcwd()
         logger.debug(f'{complete_command} - wd: {working_directory}')
         output = complete_command()
 
         """
         the output of the command is already parsed but the parsing is
@@ -49,45 +45,140 @@
         return "".join(output)
     except ProcessExecutionError as exception:
         if exit_on_error:
             click.echo(exception.stdout)
             raise Exit(code=exception.retcode) from exception
 
 
+def project_directory() -> str:
+    """
+    Returns the project directory of alfred relative to the current command.
+    This is the first parent where the `.alfred.yml` file is present.
+
+    >>> @alfred.command("project_directory")
+    >>> def project_directory_command():
+    >>>     project_directory = alfred.project_directory()
+    >>>     print(project_directory)
+    """
+    current_cmd = alfred_ctx.current_command()
+    return current_cmd.project_dir
+
+
+@contextlib.contextmanager
+def env(**kwargs) -> None:
+    """
+    Assign environment variables in a build command
+
+    >>> with alfred.env(ENV="prod"):
+    >>>     echo = alfred.sh("echo")
+    >>>     echo("hello world")
+
+    This instruction should update the python environment and the environment
+     from plumbum.
+    """
+    previous_environ = os.environ.copy()
+    try:
+        local.env.update(**kwargs)
+        os.environ.update(kwargs)
+        yield
+    finally:
+        local.env.clear()
+        local.env.update(previous_environ)
+        os.environ.clear()
+        os.environ.update(previous_environ)
+
 
 @click.pass_context
-def invoke_command(ctx, command_label: str, **kwargs) -> None:
-    click_command = None
-    origin_alfred_command = None
-    for alfred_command in ALFRED_COMMANDS:
-        if ctx.command.name == alfred_command.name:
-            origin_alfred_command = alfred_command
-
-    plugin = origin_alfred_command.plugin
-    plugin_click_command=_lookup_plugin_command(ALFRED_COMMANDS, command_label, plugin)
-    global_click_command=_lookup_global_command(ALFRED_COMMANDS, command_label)
-
-    available_plugins_commands = [command.original_name for command in ALFRED_COMMANDS if command.plugin == plugin]
-    available_global_commands = [command.name for command in ALFRED_COMMANDS]
-    if plugin_click_command is None and global_click_command is None:
-        message = [
-            f"command {command_label} does not exists.",
-            f"Available plugin commands for plugin `{plugin}`: {available_plugins_commands}",
-            f"Available global commands: {available_global_commands}",
-        ]
-
-        raise click.ClickException("\n".join(message))
-
-    if plugin_click_command:
-        click_command = plugin_click_command
-    elif global_click_command:
-        click_command = global_click_command
+def invoke_command(ctx, command: str or List[str], **kwargs) -> None:
+    """
+    Invokes a command as a subcommand.
+
+    >>> alfred.invoke_command("test"])
+
+    Command arguments are passed as named parameters.
+
+    >>> alfred.invoke_command("hello_world", name="fabien"])
+
+    To invoke a command from a sub-project, it is possible to pass the fullname of a command as
+    an array as an argument.
+
+    >>> alfred.invoke_command(["product1", "hello_world"], name="fabien"])
+    """
+
+    _calling_commmand = alfred_ctx.current_command()
+    if _calling_commmand is not None:
+        project_dir = _calling_commmand.project_dir
+    else:
+        project_dir = manifest.lookup_project_dir()
+
+    _command = commands.lookup(command, project_dir)
+    if _command is None:
+        raise click.ClickException(f"command {command} does not exists.")
+
+
+    click_command = _command.command
+    if hasattr(click_command, "help"):
+        echo.subcommand(f"$ alfred {click_command.name} : {click_command.help}")
+    else:
+        echo.subcommand(f"$ alfred {click_command.name}")
+
+    with alfred_ctx.stack_subcommand(_command):
+        args = alfred_command.format_cli_arguments(_command, kwargs)
+        if alfred_ctx.should_use_external_venv():
+            alfred_ctx.invoke_through_external_venv(args)
+        else:
+            ctx.invoke(click_command, **kwargs)
+
+
+class pythonpath:  #pylint: disable=invalid-name
+    """
+    Add the project folder, i.e. the root folder which corresponds to the alfred command used,
+    to pythonpath to make available the packages present at this level.
+
+    >>> @alfred.command()
+    >>> @alfred.pythonpath()
+    >>> def my_command():
+    >>>     pass
+
+    It is possible to add other directories to the pythonpath with the `directories` parameter.
+    The path of the added folders is relative to the root folder of the alfred command used, ie
+    the location of the `.alfred.yml` file.
+
+    >>> @alfred.command()
+    >>> @alfred.pythonpath(['src'])
+    >>> def my_command():
+    >>>     pass
+    """
 
-    click.echo(click.style(f"$ alfred {click_command.name} : {click_command.help}", fg='green'))
-    ctx.invoke(click_command, **kwargs)
+    def __init__(self, directories: List[str] = None, append_project=True):
+        """
+        manage the case where the decorator is used without parenthesis
+
+        """
+        if isinstance(directories, Callable):
+            raise TypeError("alfred.pythonpath decoratore must be called with parenthesis as @alfred.pythonpath()")
+
+        self.directories = directories
+        self.append_project = append_project
+        self._generator = None
+
+    def __enter__(self):
+        self._generator = _pythonpath(self.directories, self.append_project)
+        self._generator.__enter__()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._generator.__exit__(exc_type, exc_val, exc_tb)
+
+    def __call__(self, func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            with _pythonpath(self.directories, self.append_project):
+                return func(*args, **kwargs)
+
+        return wrapper
 
 
 def sh(command: Union[str, List[str]], fail_message: str = None) -> LocalCommand:  # pylint: disable=invalid-name
     """
     Load a shell program from the local system. If the command does not exists, it
     will show an error `fail_message` to the console.
 
@@ -143,68 +234,38 @@
     >>> alfred.run(mv, ["/var/yolo", "/var/yolo1"], exit_on_error=False)
 
 
     :param command: shell program to execute
     :param exit_on_error: break the flow if the exit code is different of 0 (active by default)
     """
     try:
+        logger = get_logger()
         complete_command = command[args]
         working_directory = os.getcwd()
         logger.debug(f'{complete_command} - wd: {working_directory}')
         complete_command & FG  # pylint: disable=pointless-statement
     except ProcessExecutionError as exception:
         if exit_on_error:
             raise Exit(code=exception.retcode) from exception
 
 
-def lookup_alfred_configuration_path() -> path:
-    workingdir = path(os.getcwd())
-    hierarchy_directories = list_hierarchy_directory(workingdir)
-
-    alfred_configuration_path = None
-    for directory in hierarchy_directories:
-        alfred_configuration_path = path_contains_alfred_configuration(directory)
-        if alfred_configuration_path is not None:
-            break
-
-    if not alfred_configuration_path:
-        raise NotInitialized("not an alfred project (or any of the parent directories), you should run alfred init")
-
-    logger.debug(f"alfred configuration file : {alfred_configuration_path}")
-
-    return alfred_configuration_path
-
-
-def lookup_alfred_configuration() -> AlfredConfiguration:
-    alfred_configuration_path = lookup_alfred_configuration_path()
-
-    with io.open(alfred_configuration_path,  encoding="utf8") as file:
-        alfred_configuration = yaml.load(file, Loader=SafeLoader)
-        for plugin in alfred_configuration["plugins"]:
-            plugin['path'] =  os.path.realpath(os.path.join(alfred_configuration_path, '..', plugin['path']))
-            logger.debug(f"alfred plugin : {plugin}")
-
-        return AlfredConfiguration(alfred_configuration)
-
-
-def path_contains_alfred_configuration(alfred_configuration_path: path) -> Optional[path]:
-    alfred_configuration_path = path(os.path.join(alfred_configuration_path, ".alfred.yml"))
-    if os.path.isfile(alfred_configuration_path):
-        return alfred_configuration_path
-
-    return None
+@contextlib.contextmanager
+def _pythonpath(directories: List[str] = None, append_project=True) -> None:
+    """
+    See the pythonpath class above which implements the pattern
+    to support a decorator and a context manager.
+    """
+    alfred_ctx.assert_in_command("alfred.pythonpath")
 
+    if directories is None:
+        directories = []
 
-def _lookup_plugin_command(all_commands, command_label, plugin) -> Optional[BaseCommand]:
-    click_command = None
-    for alfred_command in all_commands:
-        if alfred_command.original_name == command_label and alfred_command.plugin == plugin:
-            click_command = alfred_command.command
-    return click_command
+    _pythonpath = os.environ.get("PYTHONPATH", "").split(':')
+    root_directory = project_directory()
+    real_directories = [os.path.realpath(directory) for directory in directories]
 
+    if append_project:
+        real_directories += [root_directory]
 
-def _lookup_global_command(all_commands, command_label) -> Optional[BaseCommand]:
-    click_command = None
-    for alfred_command in all_commands:
-        if alfred_command.name == command_label:
-            click_command = alfred_command.command
-    return click_command
+    new_pythonpath = ":".join(real_directories + _pythonpath)
+    with lib.override_pythonpath(new_pythonpath):
+        yield
```

### Comparing `alfred-cli-1.2.0/src/alfred/os.py` & `alfred_cli-2.0.0b1/src/alfred/os.py`

 * *Files identical despite different names*

### Comparing `alfred-cli-1.2.0/src/alfred/type.py` & `alfred_cli-2.0.0b1/src/alfred/domain/manifest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-# pylint: disable=pointless-string-statement
+import logging
+import os.path
+from typing import List
 
-from typing import NewType, List
-
-import click
-
-"""
-path of object (directory or file) in filesystem
-/root
-"""
-path = NewType('path', str)  # pylint: disable=invalid-name
-
-
-class Environment:
+class Environment:  # pylint: disable=too-few-public-methods
 
     def __init__(self, key: str, value: str):
         self.key = key
         self.value = value
 
 
-class AlfredConfiguration:
+class AlfredManifest:
 
-    def __init__(self, alfred_configuration: dict):
+    def __init__(self, path: str, alfred_configuration: dict):
+        self.path = os.path.realpath(path)
         self._alfred_configuration = alfred_configuration
 
+    @property
+    def configuration(self) -> dict:
+        return self._alfred_configuration
+
+    @property
+    def project_directory(self) -> str:
+        return os.path.dirname(self.path)
+
     def environments(self) -> List[Environment]:
         environments = []
         if 'environment' in self._alfred_configuration:
             environment_values: List[str] = self._alfred_configuration['environment']
             if isinstance(environment_values, list):
                 for environment in environment_values:
                     try:
                         environment_splitted = environment.split("=")
                         if len(environment_splitted) == 1:
                             environments.append(Environment(environment_splitted[0], ""))
                         else:
                             environments.append(Environment(environment_splitted[0], environment_splitted[1]))
 
                     except Exception as exception:  # pylint: disable=broad-except
-                        click.echo(exception, err=True)
+                        logging.exception(exception)
 
         return environments
-
-    def plugins(self) -> List[str]:
-        alfred_configuration = self._alfred_configuration
-        return alfred_configuration["plugins"]
```

