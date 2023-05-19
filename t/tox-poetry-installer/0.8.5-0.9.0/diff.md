# Comparing `tmp/tox-poetry-installer-0.8.5.tar.gz` & `tmp/tox-poetry-installer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-poetry-installer-0.8.5.tar", max compression
+gzip compressed data, was "tox-poetry-installer-0.9.0.tar", max compression
```

## Comparing `tox-poetry-installer-0.8.5.tar` & `tox-poetry-installer-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1059 2022-09-06 20:46:03.430923 tox-poetry-installer-0.8.5/LICENSE.md
--rw-r--r--   0        0        0    23632 2022-09-06 20:46:03.573924 tox-poetry-installer-0.8.5/README.md
--rw-r--r--   0        0        0     1982 2022-09-06 20:38:16.566042 tox-poetry-installer-0.8.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tests/__init__.py
--rw-r--r--   0        0        0     1937 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tests/fixtures.py
--rw-r--r--   0        0        0     2081 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tests/test_installer.py
--rw-r--r--   0        0        0     1219 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tests/test_metadata.py
--rw-r--r--   0        0        0     2731 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tests/test_transients.py
--rw-r--r--   0        0        0      355 2022-09-06 20:38:16.566042 tox-poetry-installer-0.8.5/tox_poetry_installer/__about__.py
--rw-r--r--   0        0        0      153 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tox_poetry_installer/__init__.py
--rw-r--r--   0        0        0     2085 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tox_poetry_installer/_poetry.py
--rw-r--r--   0        0        0      966 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tox_poetry_installer/constants.py
--rw-r--r--   0        0        0     1491 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tox_poetry_installer/exceptions.py
--rw-r--r--   0        0        0    10399 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tox_poetry_installer/hooks.py
--rw-r--r--   0        0        0     2855 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tox_poetry_installer/installer.py
--rw-r--r--   0        0        0      937 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tox_poetry_installer/logger.py
--rw-r--r--   0        0        0        0 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tox_poetry_installer/py.typed
--rw-r--r--   0        0        0    10823 2022-05-31 03:01:10.435532 tox-poetry-installer-0.8.5/tox_poetry_installer/utilities.py
--rw-r--r--   0        0        0    25154 2022-09-06 20:46:34.803840 tox-poetry-installer-0.8.5/setup.py
--rw-r--r--   0        0        0    24939 2022-09-06 20:46:34.805592 tox-poetry-installer-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1059 2022-09-07 20:03:49.587295 tox-poetry-installer-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0    23370 2022-09-07 20:03:49.707295 tox-poetry-installer-0.9.0/README.md
+-rw-r--r--   0        0        0     1867 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1945 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tests/fixtures.py
+-rw-r--r--   0        0        0     2071 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tests/test_installer.py
+-rw-r--r--   0        0        0     1219 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tests/test_metadata.py
+-rw-r--r--   0        0        0     2731 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tests/test_transients.py
+-rw-r--r--   0        0        0      355 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/__about__.py
+-rw-r--r--   0        0        0      153 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tox_poetry_installer/__init__.py
+-rw-r--r--   0        0        0     2083 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/_poetry.py
+-rw-r--r--   0        0        0     1009 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/constants.py
+-rw-r--r--   0        0        0     1491 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tox_poetry_installer/exceptions.py
+-rw-r--r--   0        0        0    10426 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/hooks.py
+-rw-r--r--   0        0        0     2867 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/installer.py
+-rw-r--r--   0        0        0      937 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tox_poetry_installer/logger.py
+-rw-r--r--   0        0        0        0 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tox_poetry_installer/py.typed
+-rw-r--r--   0        0        0    11705 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/utilities.py
+-rw-r--r--   0        0        0    24911 1970-01-01 00:00:00.000000 tox-poetry-installer-0.9.0/setup.py
+-rw-r--r--   0        0        0    24932 1970-01-01 00:00:00.000000 tox-poetry-installer-0.9.0/PKG-INFO
```

### Comparing `tox-poetry-installer-0.8.5/LICENSE.md` & `tox-poetry-installer-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tox-poetry-installer-0.8.5/README.md` & `tox-poetry-installer-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 - [Developing the Plugin](#developer-documentation)
 - [Road Map](#road-map)
 
 See the
 [Changelog](https://github.com/enpaul/tox-poetry-installer/blob/devel/CHANGELOG.md) for
 release history.
 
-*See also: [official Tox plugins](https://tox.readthedocs.io/en/latest/plugins.html), [Poetry-Dev-Dependencies Tox plugin](https://github.com/sinoroc/tox-poetry-dev-dependencies), [Poetry Tox plugin](https://github.com/tkukushkin/tox-poetry)*
+*See also: [official Tox plugins](https://tox.readthedocs.io/en/latest/plugins.html), [Poetry Tox plugin](https://github.com/tkukushkin/tox-poetry)*
 
 ## Feature Overview
 
 - Manage package versions in exactly one place and with exactly one tool: Poetry.
 - Ensure CI/CD and other automation tools are using the same package versions that you are
   in your local development environment.
 - Add only the packages you need to a Tox test environment, instead of everything in your
@@ -349,41 +349,34 @@
 - To report a security concern or code of conduct violation, please contact the project
   author directly at **‌me \[at‌\] enp dot‎ ‌one**.
 - To submit an update, please
   [fork the repository](https://docs.github.com/en/enterprise/2.20/user/github/getting-started-with-github/fork-a-repo)
   and [open a pull request](https://github.com/enpaul/tox-poetry-installer/compare).
 
 Developing this project requires [Python 3.7+](https://www.python.org/downloads/) and
-[Poetry 1.0](https://python-poetry.org/docs/#installation) or later. GNU Make can
+[Poetry 1.2](https://python-poetry.org/docs/#installation) or later. GNU Make can
 optionally be used to quickly setup a local development environment, but this is not
 required.
 
 To setup a local development environment:
 
 ```bash
 # Clone the repository...
 # ...over HTTPS
 git clone https://github.com/enpaul/tox-poetry-installer.git
 # ...over SSH
 git clone git@github.com:enpaul/tox-poetry-installer.git
 
 cd tox-poetry-installer/
 
-# Create and configure the local development environment...
-# ...with make:
+# Create and configure the local development environment
 make dev
-# ...manually:
-poetry install -E poetry --remove-untracked
-poetry run pre-commit install
 
-# Run tests and CI locally...
-# ...with make:
+# Run tests and CI locally
 make test
-# ...manually:
-poetry run tox --recreate
 
 # See additional make targets
 make help
 ```
 
 > **Note:** The pre-commit hooks require dependencies in the Poetry environment to run. To
 > make a commit with the pre-commit hooks, you will need to run `poetry run git commit` or,
```

### Comparing `tox-poetry-installer-0.8.5/pyproject.toml` & `tox-poetry-installer-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tox-poetry-installer"
-version = "0.8.5"
+version = "0.9.0"
 license = "MIT"
 authors = ["Ethan Paul <24588726+enpaul@users.noreply.github.com>"]
 description = "A plugin for Tox that lets you install test environment dependencies from the Poetry lockfile"
 repository = "https://github.com/enpaul/tox-poetry-installer/"
 packages = [
   {include = "tox_poetry_installer"},
   {include = "tests/*.py", format = "sdist"}
@@ -19,49 +19,49 @@
   "Environment :: Plugins",
   "Framework :: tox",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 [tool.poetry.plugins.tox]
 poetry_installer = "tox_poetry_installer"
 
 [tool.poetry.extras]
-poetry = ["poetry"]
+poetry = ["poetry", "cleo"]
 
 [tool.poetry.dependencies]
-python = "^3.6.1"
-poetry = {version = ">=1.0.0,<1.2", optional = true}
-poetry-core = "^1.0.0"
+python = "^3.7"
+cleo = {version = "^1.0.0a5", optional = true, allow-prereleases = true}
+poetry = {version = "^1.2.0", optional = true}
+poetry-core = "^1.1.0"
 tox = "^3.8.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 bandit = "^1.6.2"
-black = { version = "^21.12b0", allow-prereleases = true, python = "^3.7" }
-blacken-docs = { version = "^1.8.0", python = "^3.7" }
-ipython = { version = "^7.18.1", python = "^3.7" }
+black = "^22.3.0"
+blacken-docs = "^1.8.0"
+ipython = "^7.18.1"
 mdformat = "^0.6"
 mdformat-gfm = "^0.2"
 mypy = "^0.930"
 pre-commit = "^2.7.1"
 pre-commit-hooks = "^3.3.0"
-pylint = { version = "^2.13.0", python = "^3.7" }
+pylint = "^2.13.0"
 pytest = "^6.0.2"
 pytest-cov = "^2.10.1"
 reorder-python-imports = "^2.3.5"
 safety = "^1.9.0"
 toml = "^0.10.1"
 tox = "^3.20.0"
 types-toml = "^0.10.1"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tox-poetry-installer-0.8.5/tests/fixtures.py` & `tox-poetry-installer-0.9.0/tests/fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import poetry.factory
 import poetry.installation.pip_installer
 import poetry.utils.env
 import pytest
 import tox
-from poetry.core.packages import Package as PoetryPackage
+from poetry.core.packages.package import Package as PoetryPackage
 
 from tox_poetry_installer import utilities
 
 
 TEST_PROJECT_PATH = Path(__file__).parent.resolve() / "test-project"
 
 FAKE_VENV_PATH = Path("nowhere")
```

### Comparing `tox-poetry-installer-0.8.5/tests/test_installer.py` & `tox-poetry-installer-0.9.0/tests/test_installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 from tox_poetry_installer import utilities
 
 
 def test_deduplication(mock_venv, mock_poetry_factory):
     """Test that the installer does not install duplicate dependencies"""
     poetry = Factory().create_poetry(None)
     packages: utilities.PackageMap = {
-        item.name: item for item in poetry.locker.locked_repository(False).packages
+        item.name: item for item in poetry.locker.locked_repository().packages
     }
 
     venv = tox.venv.VirtualEnv()
     to_install = [packages["toml"], packages["toml"]]
 
     installer.install(poetry, venv, to_install)
 
     assert len(set(to_install)) == len(venv.installed)  # pylint: disable=no-member
 
 
 def test_parallelization(mock_venv, mock_poetry_factory):
     """Test that behavior is consistent between parallel and non-parallel usage"""
     poetry = Factory().create_poetry(None)
     packages: utilities.PackageMap = {
-        item.name: item for item in poetry.locker.locked_repository(False).packages
+        item.name: item for item in poetry.locker.locked_repository().packages
     }
 
     to_install = [
         packages["toml"],
         packages["toml"],
         packages["tox"],
         packages["requests"],
```

### Comparing `tox-poetry-installer-0.8.5/tests/test_metadata.py` & `tox-poetry-installer-0.9.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `tox-poetry-installer-0.8.5/tests/test_transients.py` & `tox-poetry-installer-0.9.0/tests/test_transients.py`

 * *Files identical despite different names*

### Comparing `tox-poetry-installer-0.8.5/tox_poetry_installer/_poetry.py` & `tox-poetry-installer-0.9.0/tox_poetry_installer/_poetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 # pylint: disable=unused-import
 import sys
 
 from tox_poetry_installer import exceptions
 
 
 try:
+    from cleo.io.null_io import NullIO
     from poetry.factory import Factory
     from poetry.installation.pip_installer import PipInstaller
-    from poetry.io.null_io import NullIO
     from poetry.poetry import Poetry
     from poetry.utils.env import VirtualEnv
 except ImportError:
     raise exceptions.PoetryNotInstalledError(
         f"No version of Poetry could be imported under the current environment for '{sys.executable}'"
     ) from None
```

### Comparing `tox-poetry-installer-0.8.5/tox_poetry_installer/constants.py` & `tox-poetry-installer-0.9.0/tox_poetry_installer/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 PEP508_VERSION_DELIMITERS: Tuple[str, ...] = ("~=", "==", "!=", ">", "<")
 
 # Prefix all reporter messages should include to indicate that they came from this module in the
 # console output.
 REPORTER_PREFIX: str = f"{__about__.__title__}:"
 
 # Internal list of packages that poetry has deemed unsafe and are excluded from the lockfile
-UNSAFE_PACKAGES: Set[str] = {"distribute", "pip", "setuptools", "wheel"}
+# TODO: This functionality is no longer needed, should remove in a future update.
+UNSAFE_PACKAGES: Set[str] = set()
 
 # Number of threads to use for installing dependencies by default
 DEFAULT_INSTALL_THREADS: int = 10
```

### Comparing `tox-poetry-installer-0.8.5/tox_poetry_installer/exceptions.py` & `tox-poetry-installer-0.9.0/tox_poetry_installer/exceptions.py`

 * *Files identical despite different names*

### Comparing `tox-poetry-installer-0.8.5/tox_poetry_installer/hooks.py` & `tox-poetry-installer-0.9.0/tox_poetry_installer/hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         logger.error(str(err))
         return False
     except Exception as err:
         venv.status = "InternalError"
         logger.error(f"Internal plugin error: {err}")
         raise err
 
-    dependencies = dev_deps + env_deps + project_deps
+    dependencies = utilities.dedupe_packages(dev_deps + env_deps + project_deps)
     if (
         venv.envconfig.config.option.parallel_install_threads
         != constants.DEFAULT_INSTALL_THREADS
     ):
         parallel_threads = venv.envconfig.config.option.parallel_install_threads
     else:
         parallel_threads = (
```

### Comparing `tox-poetry-installer-0.8.5/tox_poetry_installer/installer.py` & `tox-poetry-installer-0.9.0/tox_poetry_installer/installer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 # Silence this one globally to support the internal function imports for the proxied poetry module.
 # See the docstring in 'tox_poetry_installer._poetry' for more context.
 # pylint: disable=import-outside-toplevel
 import concurrent.futures
 import contextlib
 import typing
 from datetime import datetime
-from typing import Sequence
+from typing import Collection
 from typing import Set
 
-from poetry.core.packages import Package as PoetryPackage
+from poetry.core.packages.package import Package as PoetryPackage
 from tox.venv import VirtualEnv as ToxVirtualEnv
 
 from tox_poetry_installer import logger
 from tox_poetry_installer import utilities
 
 if typing.TYPE_CHECKING:
     from tox_poetry_installer import _poetry
 
 
 def install(
     poetry: "_poetry.Poetry",
     venv: ToxVirtualEnv,
-    packages: Sequence[PoetryPackage],
+    packages: Collection[PoetryPackage],
     parallels: int = 0,
 ):
     """Install a bunch of packages to a virtualenv
 
     :param poetry: Poetry object the packages were sourced from
     :param venv: Tox virtual environment to install the packages to
     :param packages: List of packages to install to the virtual environment
```

### Comparing `tox-poetry-installer-0.8.5/tox_poetry_installer/logger.py` & `tox-poetry-installer-0.9.0/tox_poetry_installer/logger.py`

 * *Files identical despite different names*

### Comparing `tox-poetry-installer-0.8.5/tox_poetry_installer/utilities.py` & `tox-poetry-installer-0.9.0/tox_poetry_installer/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import typing
 from pathlib import Path
 from typing import Dict
 from typing import List
 from typing import Sequence
 from typing import Set
 
-from poetry.core.packages import Dependency as PoetryDependency
-from poetry.core.packages import Package as PoetryPackage
+from poetry.core.packages.dependency import Dependency as PoetryDependency
+from poetry.core.packages.package import Package as PoetryPackage
 from tox.action import Action as ToxAction
 from tox.venv import VirtualEnv as ToxVirtualEnv
 
 from tox_poetry_installer import constants
 from tox_poetry_installer import exceptions
 from tox_poetry_installer import logger
 
@@ -88,15 +88,15 @@
 def build_package_map(poetry: "_poetry.Poetry") -> PackageMap:
     """Build the mapping of package names to objects
 
     :param poetry: Populated poetry object to load locked packages from
     :returns: Mapping of package names to Poetry package objects
     """
     packages = collections.defaultdict(list)
-    for package in poetry.locker.locked_repository(True).packages:
+    for package in poetry.locker.locked_repository().packages:
         packages[package.name].append(package)
 
     return packages
 
 
 def identify_transients(
     dep_name: str,
@@ -214,15 +214,15 @@
 
     dependencies: List[PoetryPackage] = []
     for dep_name in required_dep_names + extra_dep_names:
         dependencies += identify_transients(
             dep_name.lower(), packages, venv, allow_missing=[poetry.package.name]
         )
 
-    return dependencies
+    return dedupe_packages(dependencies)
 
 
 def find_additional_deps(
     packages: PackageMap,
     venv: "_poetry.VirtualEnv",
     poetry: "_poetry.Poetry",
     dep_names: Sequence[str],
@@ -239,27 +239,53 @@
     """
     dependencies: List[PoetryPackage] = []
     for dep_name in dep_names:
         dependencies += identify_transients(
             dep_name.lower(), packages, venv, allow_missing=[poetry.package.name]
         )
 
-    return dependencies
+    return dedupe_packages(dependencies)
 
 
 def find_dev_deps(
     packages: PackageMap, venv: "_poetry.VirtualEnv", poetry: "_poetry.Poetry"
 ) -> List[PoetryPackage]:
     """Find the dev dependencies
 
     Recursively identify the Poetry dev dependencies
 
     :param packages: Mapping of all locked package names to their corresponding package object
     :param venv: Poetry virtual environment to use for package compatibility checks
     :param poetry: Poetry object for the current project
     """
-    return find_additional_deps(
+    dev_group_deps = find_additional_deps(
+        packages,
+        venv,
+        poetry,
+        poetry.pyproject.data["tool"]["poetry"]
+        .get("group", {})
+        .get("dev", {})
+        .get("dependencies", {})
+        .keys(),
+    )
+
+    # Legacy pyproject.toml poetry format:
+    legacy_dev_group_deps = find_additional_deps(
         packages,
         venv,
         poetry,
         poetry.pyproject.data["tool"]["poetry"].get("dev-dependencies", {}).keys(),
     )
+
+    # Poetry 1.2 unions these two toml sections.
+    return dedupe_packages(dev_group_deps + legacy_dev_group_deps)
+
+
+def dedupe_packages(packages: Sequence[PoetryPackage]) -> List[PoetryPackage]:
+    """Deduplicates a sequence of PoetryPackages while preserving ordering
+
+    Adapted from StackOverflow: https://stackoverflow.com/a/480227
+    """
+    seen: Set[PoetryPackage] = set()
+    # Make this faster, avoid method lookup below
+    seen_add = seen.add
+    return [p for p in packages if not (p in seen or seen_add(p))]
```

### Comparing `tox-poetry-installer-0.8.5/setup.py` & `tox-poetry-installer-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 packages = \
 ['tests', 'tests.test-project.test_project', 'tox_poetry_installer']
 
 package_data = \
 {'': ['*'], 'tests': ['test-project/*']}
 
 install_requires = \
-['poetry-core>=1.0.0,<2.0.0', 'tox>=3.8.0,<4.0.0']
+['poetry-core>=1.1.0,<2.0.0', 'tox>=3.8.0,<4.0.0']
 
 extras_require = \
-{'poetry': ['poetry>=1.0.0,<1.2']}
+{'poetry': ['cleo>=1.0.0a5,<2.0.0', 'poetry>=1.2.0,<2.0.0']}
 
 entry_points = \
 {'tox': ['poetry_installer = tox_poetry_installer']}
 
 setup_kwargs = {
     'name': 'tox-poetry-installer',
-    'version': '0.8.5',
+    'version': '0.9.0',
     'description': 'A plugin for Tox that lets you install test environment dependencies from the Poetry lockfile',
-    'long_description': '# tox-poetry-installer\n\nA plugin for [Tox](https://tox.readthedocs.io/en/latest/) that lets you install test\nenvironment dependencies from the [Poetry](https://python-poetry.org/) lockfile.\n\n[![CI Status](https://github.com/enpaul/tox-poetry-installer/workflows/CI/badge.svg?event=push)](https://github.com/enpaul/tox-poetry-installer/actions)\n[![PyPI Version](https://img.shields.io/pypi/v/tox-poetry-installer)](https://pypi.org/project/tox-poetry-installer/)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/tox-poetry-installer)](https://libraries.io/pypi/tox-poetry-installer)\n[![License](https://img.shields.io/pypi/l/tox-poetry-installer)](https://opensource.org/licenses/MIT)\n[![Python Supported Versions](https://img.shields.io/pypi/pyversions/tox-poetry-installer)](https://www.python.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n⚠️ **This project is beta software and is under active development** ⚠️\n\n## Documentation\n\n- [Feature Overview](#feature-overview)\n- [Using the Plugin](#user-documentation)\n  - [Installing](#installing)\n  - [Quick Start](#quick-start)\n  - [References](#references)\n    - [Config Options](#configuration-options)\n    - [Runtime Options](#runtime-options)\n    - [Errors](#errors)\n  - [Other Notes](#other-notes)\n    - [Unsupported Tox config options](#unsupported-tox-config-options)\n    - [Updating locked dependencies in a testenv](#updating-locked-dependencies-in-a-testenv)\n    - [Installing unsafe dependencies](#installing-unsafe-dependencies)\n    - [Using with an unmanaged Poetry installation](#using-with-an-unmanaged-poetry-installation)\n- [Developing the Plugin](#developer-documentation)\n- [Road Map](#road-map)\n\nSee the\n[Changelog](https://github.com/enpaul/tox-poetry-installer/blob/devel/CHANGELOG.md) for\nrelease history.\n\n*See also: [official Tox plugins](https://tox.readthedocs.io/en/latest/plugins.html), [Poetry-Dev-Dependencies Tox plugin](https://github.com/sinoroc/tox-poetry-dev-dependencies), [Poetry Tox plugin](https://github.com/tkukushkin/tox-poetry)*\n\n## Feature Overview\n\n- Manage package versions in exactly one place and with exactly one tool: Poetry.\n- Ensure CI/CD and other automation tools are using the same package versions that you are\n  in your local development environment.\n- Add only the packages you need to a Tox test environment, instead of everything in your\n  lockfile.\n- Directly integrate with Poetry, re-using your existing package indexes and credentials\n  with no additional configuration.\n- Wherever possible, built-in Tox config options are always respected and their behavior\n  kept consistent.\n- Extremely configurable. Every feature can be disabled or enabled for any given Tox test\n  environment.\n- Friendly to other Tox plugins and supports a wide range of environments.\n\n## User Documentation\n\n*This section is for users looking to integrate the plugin with their project or CI system. For information on contributing to the plugin please see the [Developer Docs](#developer-documentation)*\n\n### Installing\n\nThe recommended way to install the plugin is to add it to a project using Poetry:\n\n```bash\npoetry add tox-poetry-installer[poetry] --dev\n```\n\n> **Note:** Always install the plugin with the `[poetry]` extra, unless you are\n> [managing the Poetry installation yourself](#externally-managed-poetry-installation).\n\nAlternatively, it can be installed directly to a virtual environment using Pip, though\nthis is not recommended:\n\n```bash\nsource somevenv/bin/activate\npip install tox-poetry-installer\n```\n\nAlternatively alternatively, it can be installed using the Tox\n[`requires`](https://tox.readthedocs.io/en/latest/config.html#conf-requires) option by\nadding the below to `tox.ini`, though this is also not recommended:\n\n```ini\nrequires =\n    tox-poetry-installer[poetry] == 0.8.0\n```\n\nAfter installing, check that Tox recognizes the plugin by running\n`poetry run tox --version`. The command should give output similar to below:\n\n```\n3.20.0 imported from .venv/lib64/python3.8/site-packages/tox/__init__.py\nregistered plugins:\n    tox-poetry-installer-0.8.0 at .venv/lib64/python3.8/site-packages/tox_poetry_installer/__init__.py\n```\n\n### Quick Start\n\nCongratulations! 🎉 Just by installing the plugin your Tox config is already using locked\ndependencies: when Tox builds and installs your project package to a test environment,\nyour project package\'s dependencies will be installed from the lockfile.\n\nNow lets update an example `tox.ini` to install the other test environment dependencies\nfrom the lockfile.\n\nA `testenv` from the example `tox.ini` we\'re starting with is below:\n\n```ini\n[testenv]\ndescription = Some very cool tests\ndeps =\n    black == 20.8b1\n    pylint >=2.4.4,<2.7.0\n    mypy <0.800\ncommands = ...\n```\n\nTo update the config so that the testenv dependencies are installed from the lockfile, we\ncan replace the built-in\n[`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option with the\n`locked_deps` option provided by the plugin, and then remove the inline version\nspecifiers. With these changes the three testenv dependencies (as well as all of their\ndependencies) will be installed from the lockfile when the test environment is recreated:\n\n```ini\n[testenv]\ndescription = Some very cool tests\nlocked_deps =\n    black\n    pylint\n    mypy\ncommands = ...\n```\n\nWe can also add the `require_locked_deps` option to the test environment. This will both\nblock any other install tools (another plugin or Tox itself) from installing dependencies\nto the Tox environment and also cause Tox to fail if the test environment also uses the\nbuilt-in [`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option:\n\n```ini\n[testenv]\ndescription = Some very cool tests\nrequire_locked_deps = true\nlocked_deps =\n    black\n    pylint\n    mypy\ncommands = ...\n```\n\n> **Note:** Settings configured on the main `testenv` environment are inherited by child\n> test environments (for example, `testenv:foo`). To override this, specify the setting in\n> the child environment with a different value.\n\nAlternatively, we can skip specifying all of our dependencies for a test environment in\nthe Tox config and just install all of our Poetry dev-dependencies automatically:\n\n```ini\n[testenv]\ndescription = Some very cool tests\nrequire_locked_deps = true\ninstall_dev_deps = true\ncommands = ...\n```\n\n> **Note:** Setting `install_dev_deps = true` on an environment that also installs the\n> project package is functionally equivalent to running `poetry install`.\n\nFinally, we can also install an unlocked dependency (a dependency which doesn\'t take its\nversion from the Poetry lockfile) into the test environment alongside the locked ones. We\nneed to remove the `require_locked_deps = true` option, otherwise the environment will\nerror, and then we can add the unlocked dependency using the built-in\n[`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option:\n\n```ini\n[testenv]\ndescription = Some very cool tests\ndeps =\n    pytest >= 5.6.0,<6.0.0\nlocked_deps =\n    black\n    pylint\n    mypy\ncommands = ...\n```\n\n## References\n\n### Configuration Options\n\nAll options listed below are Tox environment options and can be applied to one or more\nenvironment sections of the `tox.ini` file. They cannot be applied to the global Tox\nconfiguration section.\n\n> **Note:** Settings configured on the main `testenv` environment are inherited by child\n> test environments (for example, `testenv:foo`). To override this, specify the setting in\n> the child environment with a different value.\n\n| Option                 |  Type   | Default | Description                                                                                                                                                                                                                                                                                                                                                          |\n| :--------------------- | :-----: | :-----: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| `locked_deps`          |  List   |  `[]`   | Names of packages to install to the test environment from the Poetry lockfile. Transient dependencies (packages required by these dependencies) are automatically included.                                                                                                                                                                                          |\n| `require_locked_deps`  | Boolean |  False  | Whether the plugin should block attempts to install unlocked dependencies to the test environment. If enabled, then the [`tox_testenv_install_deps`](https://tox.readthedocs.io/en/latest/plugins.html#tox.hookspecs.tox_testenv_install_deps) plugin hook will be intercepted and an error will be raised if the test environment has the `deps` option configured. |\n| `install_dev_deps`     | Boolean |  False  | Whether all of the Poetry dev-dependencies should be installed to the test environment.                                                                                                                                                                                                                                                                              |\n| `install_project_deps` | Boolean |  True   | Whether all of the Poetry primary dependencies for the project package should be installed to the test environment.                                                                                                                                                                                                                                                  |\n| `require_poetry`       | Boolean |  False  | Whether Tox should be forced to fail if the plugin cannot import Poetry locally. If `False` then the plugin will be skipped for the test environment if Poetry cannot be imported. If `True` then the plugin will force the environment to error and the Tox run to fail.                                                                                            |\n\n### Runtime Options\n\nAll arguments listed below can be passed to the `tox` command to modify runtime behavior\nof the plugin.\n\n| Argument                     |  Type   | Default | Description                                                                                                                                                                                                                                                                          |\n| :--------------------------- | :-----: | :-----: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| `--parallel-install-threads` | Integer |  `10`   | Number of worker threads to use to install dependencies in parallel. Installing in parallel with more threads can greatly speed up the install process, but can cause race conditions during install. Pass this option with the value `0` to entirely disable parallel installation. |\n\n> **Note:** The `--require-poetry` runtime option is deprecated and will be removed in\n> version 1.0.0. Please set `require_poetry = true` in `tox.ini` for environments that\n> should fail if Poetry is not available.\n\n> **Note:** The `--parallelize-locked-install` option is deprecated and will be removed in\n> version 1.0.0. Please use the `--parallel-install-threads` option.\n\n### Errors\n\nThere are several errors that the plugin can encounter for a test environment when Tox is\nrun. If an error is encountered then the status of the test environment that caused the\nerror will be set to one of the "Status" values below to indicate what the error was.\n\n| Status/Name                     | Cause                                                                                                                                                                                                                           |\n| :------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |\n| `ExtraNotFoundError`            | Indicates that the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras) config option specified an extra that is not configured by Poetry in `pyproject.toml`.                                              |\n| `LockedDepVersionConflictError` | Indicates that an item in the `locked_deps` config option includes a [PEP-508 version specifier](https://www.python.org/dev/peps/pep-0508/#grammar) (ex: `pytest >=6.0, <6.1`).                                                 |\n| `LockedDepNotFoundError`        | Indicates that an item specified in the `locked_deps` config option does not match the name of a package in the Poetry lockfile.                                                                                                |\n| `LockedDepsRequiredError`       | Indicates that a test environment with the `require_locked_deps` config option set to `true` also specified unlocked dependencies using the [`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) config option. |\n| `PoetryNotInstalledError`       | Indicates that the `poetry` module could not be imported under the current runtime environment, and `require_poetry = true` was specified.                                                                                      |\n| `RequiresUnsafeDepError`        | Indicates that the package-under-test depends on a package that Poetry has classified as unsafe and cannot be installed.                                                                                                        |\n\n> **Note:** One or more of these errors can be caused by the `pyproject.toml` being out of\n> sync with the Poetry lockfile. If this is the case, than a warning will be logged when Tox\n> is run.\n\n### Other Notes\n\n#### Unsupported Tox config options\n\nBelow are the built-in Tox config options that are not respected by this plugin. All of\nthese options are made obsolete by the Poetry lockfile: either they aren\'t needed or their\nequivalent functionality is instead taken directly from the package details Poetry stores\nin its lockfile.\n\n> **Note:** The unsupported Tox config options will still apply to unlocked dependencies\n> being installed with the default Tox installation backend.\n\n- [`install_command`](https://tox.readthedocs.io/en/latest/config.html#conf-install_command)\n- [`pip_pre`](https://tox.readthedocs.io/en/latest/config.html#conf-pip_pre)\n- [`download`](https://tox.readthedocs.io/en/latest/config.html#conf-download)\n- [`indexserver`](https://tox.readthedocs.io/en/latest/config.html#conf-indexserver)\n- [`usedevelop`](https://tox.readthedocs.io/en/latest/config.html#conf-indexserver)\n\n#### Updating locked dependencies in a testenv\n\nWhen Poetry updates the version of a package in the lockfile (using either `poetry lock`\nor `poetry update`) then the plugin will automatically use this new version to install the\npackage to a test environment; there is no need to manually update `tox.ini` after\nupdating the Poetry lockfile.\n\nHowever, the plugin cannot determine when the lockfile is updated. If a Tox test\nenvironment has already been created then it will need to be recreated (using Tox\'s\nbuilt-in\n[`--recreate`](https://tox.readthedocs.io/en/latest/example/basic.html#forcing-re-creation-of-virtual-environments)\noption) for the new version to be found and installed.\n\n> **Note:** To force Tox to always recreate a test environment the\n> [`recreate`](https://tox.readthedocs.io/en/latest/config.html#conf-recreate) config option\n> can be set.\n\n#### Installing unsafe dependencies\n\nThere are several packages that cannot be installed from the lockfile because they are\nexcluded by Poetry itself. As a result these packages cannot be installed by this plugin\neither as test environment dependencies passed directly to `locked_deps` or as a transient\ndependency. When one of these packages is encountered by the plugin a warning will be\nlogged to the console and\n**the unsafe package will not be installed to the test environment**.\n\nThis list can be found in the Poetry source code\n[here](https://github.com/python-poetry/poetry/blob/master/poetry/puzzle/provider.py). As\nof [Poetry 1.1.6](https://github.com/python-poetry/poetry/releases/tag/1.1.6) there are\nfour packages classified as "unsafe" by Poetry and excluded from the lockfile:\n\n- `setuptools`\n- `distribute`\n- `pip`\n- `wheel`\n\n#### Using with an unmanaged Poetry installation\n\nIn CI/CD systems, automation environments, or other Python environments where the loaded\nsite packages are not managed by Poetry, it can be useful to manage the local installation\nof Poetry externally. This also helps to avoid problems that can be caused by the\n`--no-root`, `--no-dev`, or `--remove-untracked` arguments to the `poetry install` command\nwhich, in some situations, can cause Poetry to uninstall itself if Poetry is specified as\na dependency of one of the packages it is managing (like this plugin). To support these\nuse cases, this plugin specifies the `poetry` package as an optional dependency that can\nbe installed using a setuptools extra also named `poetry`.\n\n**Critical Warning: This plugin requires Poetry to function. If the plugin is installed without the `poetry` setuptools extra then Poetry must be installed independently for the plugin to function properly.**\n\nTo skip installing the `poetry` package as a dependency of `tox-poetry-installer`, do not\nspecify the `poetry` extra when adding the plugin:\n\n```bash\n# Adding the package without the "[poetry]" extra specifier so that\n# Poetry is not added as a transient dev-dependency:\npoetry add tox-poetry-installer --dev\n\n# Adding the package with the "[poetry]" extra specifier, so the Poetry\n# package will be added to the environment and tracked in the lockfile:\npoetry add tox-poetry-installer[poetry] --dev\n```\n\nOnce the plugin is installed- either with or without the Poetry extra- you can validate\nthat the plugin will run correctly with the following command. This command checks that\nall three required components (Tox, Poetry, and the plugin itself) are available in the\ncurrent Python environment:\n\n```bash\npython -c \'\\\n  import tox;\\\n  import tox_poetry_installer;\\\n  from poetry.poetry import Poetry;\\\n\'\n```\n\n> **Note:** To force Tox to fail if Poetry is not installed, add the `require_poetry = true`\n> option to the tox `[testenv]` configuration. See the\n> [Config Options](#configuration-options) for more information.\n\n## Developer Documentation\n\nAll project contributors and participants are expected to adhere to the\n[Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md) ([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).\n\nThe `devel` branch has the latest (and potentially unstable) changes. The stable releases\nare tracked on [Github](https://github.com/enpaul/tox-poetry-installer/releases),\n[PyPi](https://pypi.org/project/tox-poetry-installer/#history), and in the\n[Changelog](CHANGELOG.md).\n\n- To report a bug, request a feature, or ask for assistance, please\n  [open an issue on the Github repository](https://github.com/enpaul/tox-poetry-installer/issues/new).\n- To report a security concern or code of conduct violation, please contact the project\n  author directly at **\u200cme \\[at\u200c\\] enp dot\u200e \u200cone**.\n- To submit an update, please\n  [fork the repository](https://docs.github.com/en/enterprise/2.20/user/github/getting-started-with-github/fork-a-repo)\n  and [open a pull request](https://github.com/enpaul/tox-poetry-installer/compare).\n\nDeveloping this project requires [Python 3.7+](https://www.python.org/downloads/) and\n[Poetry 1.0](https://python-poetry.org/docs/#installation) or later. GNU Make can\noptionally be used to quickly setup a local development environment, but this is not\nrequired.\n\nTo setup a local development environment:\n\n```bash\n# Clone the repository...\n# ...over HTTPS\ngit clone https://github.com/enpaul/tox-poetry-installer.git\n# ...over SSH\ngit clone git@github.com:enpaul/tox-poetry-installer.git\n\ncd tox-poetry-installer/\n\n# Create and configure the local development environment...\n# ...with make:\nmake dev\n# ...manually:\npoetry install -E poetry --remove-untracked\npoetry run pre-commit install\n\n# Run tests and CI locally...\n# ...with make:\nmake test\n# ...manually:\npoetry run tox --recreate\n\n# See additional make targets\nmake help\n```\n\n> **Note:** The pre-commit hooks require dependencies in the Poetry environment to run. To\n> make a commit with the pre-commit hooks, you will need to run `poetry run git commit` or,\n> alternatively, [launch an environment shell](https://python-poetry.org/docs/cli/#shell).\n\n## Road Map\n\nThis project is under active development and is classified as beta software, ready for\nproduction environments on a provisional basis only.\n\n- Beta classification was assigned with\n  [v0.6.0](https://github.com/enpaul/tox-poetry-installer/releases/tag/0.6.0)\n- Stable classification will be assigned when the test suite covers an acceptable number of\n  use cases\n\n### Path to Beta\n\n- [x] Verify that primary package dependencies (from the `.package` env) are installed\n  correctly using the Poetry backend.\n- [x] Support the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras) Tox\n  configuration option ([#4](https://github.com/enpaul/tox-poetry-installer/issues/4))\n- [x] Add per-environment Tox configuration option to fall back to default installation\n  backend.\n- [ ] ~Add warnings when an unsupported Tox configuration option is detected while using the\n  Poetry backend.~ ([#5](https://github.com/enpaul/tox-poetry-installer/issues/5))\n- [x] Add trivial tests to ensure the project metadata is consistent between the pyproject.toml\n  and the module constants.\n- [x] Update to use [poetry-core](https://github.com/python-poetry/poetry-core) and improve\n  robustness of the Tox and Poetry module imports to avoid potentially breaking API changes\n  in upstream packages. ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))\n- [ ] ~Find and implement a way to mitigate the\n  [UNSAFE_DEPENDENCIES issue](https://github.com/python-poetry/poetry/issues/1584) in\n  Poetry.~ ([#6](https://github.com/enpaul/tox-poetry-installer/issues/6))\n- [x] Fix logging to make proper use of Tox\'s logging reporter infrastructure ([#3](https://github.com/enpaul/tox-poetry-installer/issues/3))\n- [x] Add configuration option for installing all dev-dependencies to a testenv ([#14](https://github.com/enpaul/tox-poetry-installer/issues/14))\n\n### Path to Stable\n\nEverything in Beta plus...\n\n- [ ] Fully replace dependency on `poetry` with dependency on `poetry-core` ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))\n- [x] Add comprehensive unit tests\n- [ ] ~Add tests for each feature version of Tox between 3.8 and 3.20~\n- [x] Add tests for Python-3.6, 3.7, 3.8, and 3.9\n- [x] Add Github Actions based CI\n',
+    'long_description': '# tox-poetry-installer\n\nA plugin for [Tox](https://tox.readthedocs.io/en/latest/) that lets you install test\nenvironment dependencies from the [Poetry](https://python-poetry.org/) lockfile.\n\n[![CI Status](https://github.com/enpaul/tox-poetry-installer/workflows/CI/badge.svg?event=push)](https://github.com/enpaul/tox-poetry-installer/actions)\n[![PyPI Version](https://img.shields.io/pypi/v/tox-poetry-installer)](https://pypi.org/project/tox-poetry-installer/)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/tox-poetry-installer)](https://libraries.io/pypi/tox-poetry-installer)\n[![License](https://img.shields.io/pypi/l/tox-poetry-installer)](https://opensource.org/licenses/MIT)\n[![Python Supported Versions](https://img.shields.io/pypi/pyversions/tox-poetry-installer)](https://www.python.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n⚠️ **This project is beta software and is under active development** ⚠️\n\n## Documentation\n\n- [Feature Overview](#feature-overview)\n- [Using the Plugin](#user-documentation)\n  - [Installing](#installing)\n  - [Quick Start](#quick-start)\n  - [References](#references)\n    - [Config Options](#configuration-options)\n    - [Runtime Options](#runtime-options)\n    - [Errors](#errors)\n  - [Other Notes](#other-notes)\n    - [Unsupported Tox config options](#unsupported-tox-config-options)\n    - [Updating locked dependencies in a testenv](#updating-locked-dependencies-in-a-testenv)\n    - [Installing unsafe dependencies](#installing-unsafe-dependencies)\n    - [Using with an unmanaged Poetry installation](#using-with-an-unmanaged-poetry-installation)\n- [Developing the Plugin](#developer-documentation)\n- [Road Map](#road-map)\n\nSee the\n[Changelog](https://github.com/enpaul/tox-poetry-installer/blob/devel/CHANGELOG.md) for\nrelease history.\n\n*See also: [official Tox plugins](https://tox.readthedocs.io/en/latest/plugins.html), [Poetry Tox plugin](https://github.com/tkukushkin/tox-poetry)*\n\n## Feature Overview\n\n- Manage package versions in exactly one place and with exactly one tool: Poetry.\n- Ensure CI/CD and other automation tools are using the same package versions that you are\n  in your local development environment.\n- Add only the packages you need to a Tox test environment, instead of everything in your\n  lockfile.\n- Directly integrate with Poetry, re-using your existing package indexes and credentials\n  with no additional configuration.\n- Wherever possible, built-in Tox config options are always respected and their behavior\n  kept consistent.\n- Extremely configurable. Every feature can be disabled or enabled for any given Tox test\n  environment.\n- Friendly to other Tox plugins and supports a wide range of environments.\n\n## User Documentation\n\n*This section is for users looking to integrate the plugin with their project or CI system. For information on contributing to the plugin please see the [Developer Docs](#developer-documentation)*\n\n### Installing\n\nThe recommended way to install the plugin is to add it to a project using Poetry:\n\n```bash\npoetry add tox-poetry-installer[poetry] --dev\n```\n\n> **Note:** Always install the plugin with the `[poetry]` extra, unless you are\n> [managing the Poetry installation yourself](#externally-managed-poetry-installation).\n\nAlternatively, it can be installed directly to a virtual environment using Pip, though\nthis is not recommended:\n\n```bash\nsource somevenv/bin/activate\npip install tox-poetry-installer\n```\n\nAlternatively alternatively, it can be installed using the Tox\n[`requires`](https://tox.readthedocs.io/en/latest/config.html#conf-requires) option by\nadding the below to `tox.ini`, though this is also not recommended:\n\n```ini\nrequires =\n    tox-poetry-installer[poetry] == 0.8.0\n```\n\nAfter installing, check that Tox recognizes the plugin by running\n`poetry run tox --version`. The command should give output similar to below:\n\n```\n3.20.0 imported from .venv/lib64/python3.8/site-packages/tox/__init__.py\nregistered plugins:\n    tox-poetry-installer-0.8.0 at .venv/lib64/python3.8/site-packages/tox_poetry_installer/__init__.py\n```\n\n### Quick Start\n\nCongratulations! 🎉 Just by installing the plugin your Tox config is already using locked\ndependencies: when Tox builds and installs your project package to a test environment,\nyour project package\'s dependencies will be installed from the lockfile.\n\nNow lets update an example `tox.ini` to install the other test environment dependencies\nfrom the lockfile.\n\nA `testenv` from the example `tox.ini` we\'re starting with is below:\n\n```ini\n[testenv]\ndescription = Some very cool tests\ndeps =\n    black == 20.8b1\n    pylint >=2.4.4,<2.7.0\n    mypy <0.800\ncommands = ...\n```\n\nTo update the config so that the testenv dependencies are installed from the lockfile, we\ncan replace the built-in\n[`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option with the\n`locked_deps` option provided by the plugin, and then remove the inline version\nspecifiers. With these changes the three testenv dependencies (as well as all of their\ndependencies) will be installed from the lockfile when the test environment is recreated:\n\n```ini\n[testenv]\ndescription = Some very cool tests\nlocked_deps =\n    black\n    pylint\n    mypy\ncommands = ...\n```\n\nWe can also add the `require_locked_deps` option to the test environment. This will both\nblock any other install tools (another plugin or Tox itself) from installing dependencies\nto the Tox environment and also cause Tox to fail if the test environment also uses the\nbuilt-in [`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option:\n\n```ini\n[testenv]\ndescription = Some very cool tests\nrequire_locked_deps = true\nlocked_deps =\n    black\n    pylint\n    mypy\ncommands = ...\n```\n\n> **Note:** Settings configured on the main `testenv` environment are inherited by child\n> test environments (for example, `testenv:foo`). To override this, specify the setting in\n> the child environment with a different value.\n\nAlternatively, we can skip specifying all of our dependencies for a test environment in\nthe Tox config and just install all of our Poetry dev-dependencies automatically:\n\n```ini\n[testenv]\ndescription = Some very cool tests\nrequire_locked_deps = true\ninstall_dev_deps = true\ncommands = ...\n```\n\n> **Note:** Setting `install_dev_deps = true` on an environment that also installs the\n> project package is functionally equivalent to running `poetry install`.\n\nFinally, we can also install an unlocked dependency (a dependency which doesn\'t take its\nversion from the Poetry lockfile) into the test environment alongside the locked ones. We\nneed to remove the `require_locked_deps = true` option, otherwise the environment will\nerror, and then we can add the unlocked dependency using the built-in\n[`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option:\n\n```ini\n[testenv]\ndescription = Some very cool tests\ndeps =\n    pytest >= 5.6.0,<6.0.0\nlocked_deps =\n    black\n    pylint\n    mypy\ncommands = ...\n```\n\n## References\n\n### Configuration Options\n\nAll options listed below are Tox environment options and can be applied to one or more\nenvironment sections of the `tox.ini` file. They cannot be applied to the global Tox\nconfiguration section.\n\n> **Note:** Settings configured on the main `testenv` environment are inherited by child\n> test environments (for example, `testenv:foo`). To override this, specify the setting in\n> the child environment with a different value.\n\n| Option                 |  Type   | Default | Description                                                                                                                                                                                                                                                                                                                                                          |\n| :--------------------- | :-----: | :-----: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| `locked_deps`          |  List   |  `[]`   | Names of packages to install to the test environment from the Poetry lockfile. Transient dependencies (packages required by these dependencies) are automatically included.                                                                                                                                                                                          |\n| `require_locked_deps`  | Boolean |  False  | Whether the plugin should block attempts to install unlocked dependencies to the test environment. If enabled, then the [`tox_testenv_install_deps`](https://tox.readthedocs.io/en/latest/plugins.html#tox.hookspecs.tox_testenv_install_deps) plugin hook will be intercepted and an error will be raised if the test environment has the `deps` option configured. |\n| `install_dev_deps`     | Boolean |  False  | Whether all of the Poetry dev-dependencies should be installed to the test environment.                                                                                                                                                                                                                                                                              |\n| `install_project_deps` | Boolean |  True   | Whether all of the Poetry primary dependencies for the project package should be installed to the test environment.                                                                                                                                                                                                                                                  |\n| `require_poetry`       | Boolean |  False  | Whether Tox should be forced to fail if the plugin cannot import Poetry locally. If `False` then the plugin will be skipped for the test environment if Poetry cannot be imported. If `True` then the plugin will force the environment to error and the Tox run to fail.                                                                                            |\n\n### Runtime Options\n\nAll arguments listed below can be passed to the `tox` command to modify runtime behavior\nof the plugin.\n\n| Argument                     |  Type   | Default | Description                                                                                                                                                                                                                                                                          |\n| :--------------------------- | :-----: | :-----: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| `--parallel-install-threads` | Integer |  `10`   | Number of worker threads to use to install dependencies in parallel. Installing in parallel with more threads can greatly speed up the install process, but can cause race conditions during install. Pass this option with the value `0` to entirely disable parallel installation. |\n\n> **Note:** The `--require-poetry` runtime option is deprecated and will be removed in\n> version 1.0.0. Please set `require_poetry = true` in `tox.ini` for environments that\n> should fail if Poetry is not available.\n\n> **Note:** The `--parallelize-locked-install` option is deprecated and will be removed in\n> version 1.0.0. Please use the `--parallel-install-threads` option.\n\n### Errors\n\nThere are several errors that the plugin can encounter for a test environment when Tox is\nrun. If an error is encountered then the status of the test environment that caused the\nerror will be set to one of the "Status" values below to indicate what the error was.\n\n| Status/Name                     | Cause                                                                                                                                                                                                                           |\n| :------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |\n| `ExtraNotFoundError`            | Indicates that the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras) config option specified an extra that is not configured by Poetry in `pyproject.toml`.                                              |\n| `LockedDepVersionConflictError` | Indicates that an item in the `locked_deps` config option includes a [PEP-508 version specifier](https://www.python.org/dev/peps/pep-0508/#grammar) (ex: `pytest >=6.0, <6.1`).                                                 |\n| `LockedDepNotFoundError`        | Indicates that an item specified in the `locked_deps` config option does not match the name of a package in the Poetry lockfile.                                                                                                |\n| `LockedDepsRequiredError`       | Indicates that a test environment with the `require_locked_deps` config option set to `true` also specified unlocked dependencies using the [`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) config option. |\n| `PoetryNotInstalledError`       | Indicates that the `poetry` module could not be imported under the current runtime environment, and `require_poetry = true` was specified.                                                                                      |\n| `RequiresUnsafeDepError`        | Indicates that the package-under-test depends on a package that Poetry has classified as unsafe and cannot be installed.                                                                                                        |\n\n> **Note:** One or more of these errors can be caused by the `pyproject.toml` being out of\n> sync with the Poetry lockfile. If this is the case, than a warning will be logged when Tox\n> is run.\n\n### Other Notes\n\n#### Unsupported Tox config options\n\nBelow are the built-in Tox config options that are not respected by this plugin. All of\nthese options are made obsolete by the Poetry lockfile: either they aren\'t needed or their\nequivalent functionality is instead taken directly from the package details Poetry stores\nin its lockfile.\n\n> **Note:** The unsupported Tox config options will still apply to unlocked dependencies\n> being installed with the default Tox installation backend.\n\n- [`install_command`](https://tox.readthedocs.io/en/latest/config.html#conf-install_command)\n- [`pip_pre`](https://tox.readthedocs.io/en/latest/config.html#conf-pip_pre)\n- [`download`](https://tox.readthedocs.io/en/latest/config.html#conf-download)\n- [`indexserver`](https://tox.readthedocs.io/en/latest/config.html#conf-indexserver)\n- [`usedevelop`](https://tox.readthedocs.io/en/latest/config.html#conf-indexserver)\n\n#### Updating locked dependencies in a testenv\n\nWhen Poetry updates the version of a package in the lockfile (using either `poetry lock`\nor `poetry update`) then the plugin will automatically use this new version to install the\npackage to a test environment; there is no need to manually update `tox.ini` after\nupdating the Poetry lockfile.\n\nHowever, the plugin cannot determine when the lockfile is updated. If a Tox test\nenvironment has already been created then it will need to be recreated (using Tox\'s\nbuilt-in\n[`--recreate`](https://tox.readthedocs.io/en/latest/example/basic.html#forcing-re-creation-of-virtual-environments)\noption) for the new version to be found and installed.\n\n> **Note:** To force Tox to always recreate a test environment the\n> [`recreate`](https://tox.readthedocs.io/en/latest/config.html#conf-recreate) config option\n> can be set.\n\n#### Installing unsafe dependencies\n\nThere are several packages that cannot be installed from the lockfile because they are\nexcluded by Poetry itself. As a result these packages cannot be installed by this plugin\neither as test environment dependencies passed directly to `locked_deps` or as a transient\ndependency. When one of these packages is encountered by the plugin a warning will be\nlogged to the console and\n**the unsafe package will not be installed to the test environment**.\n\nThis list can be found in the Poetry source code\n[here](https://github.com/python-poetry/poetry/blob/master/poetry/puzzle/provider.py). As\nof [Poetry 1.1.6](https://github.com/python-poetry/poetry/releases/tag/1.1.6) there are\nfour packages classified as "unsafe" by Poetry and excluded from the lockfile:\n\n- `setuptools`\n- `distribute`\n- `pip`\n- `wheel`\n\n#### Using with an unmanaged Poetry installation\n\nIn CI/CD systems, automation environments, or other Python environments where the loaded\nsite packages are not managed by Poetry, it can be useful to manage the local installation\nof Poetry externally. This also helps to avoid problems that can be caused by the\n`--no-root`, `--no-dev`, or `--remove-untracked` arguments to the `poetry install` command\nwhich, in some situations, can cause Poetry to uninstall itself if Poetry is specified as\na dependency of one of the packages it is managing (like this plugin). To support these\nuse cases, this plugin specifies the `poetry` package as an optional dependency that can\nbe installed using a setuptools extra also named `poetry`.\n\n**Critical Warning: This plugin requires Poetry to function. If the plugin is installed without the `poetry` setuptools extra then Poetry must be installed independently for the plugin to function properly.**\n\nTo skip installing the `poetry` package as a dependency of `tox-poetry-installer`, do not\nspecify the `poetry` extra when adding the plugin:\n\n```bash\n# Adding the package without the "[poetry]" extra specifier so that\n# Poetry is not added as a transient dev-dependency:\npoetry add tox-poetry-installer --dev\n\n# Adding the package with the "[poetry]" extra specifier, so the Poetry\n# package will be added to the environment and tracked in the lockfile:\npoetry add tox-poetry-installer[poetry] --dev\n```\n\nOnce the plugin is installed- either with or without the Poetry extra- you can validate\nthat the plugin will run correctly with the following command. This command checks that\nall three required components (Tox, Poetry, and the plugin itself) are available in the\ncurrent Python environment:\n\n```bash\npython -c \'\\\n  import tox;\\\n  import tox_poetry_installer;\\\n  from poetry.poetry import Poetry;\\\n\'\n```\n\n> **Note:** To force Tox to fail if Poetry is not installed, add the `require_poetry = true`\n> option to the tox `[testenv]` configuration. See the\n> [Config Options](#configuration-options) for more information.\n\n## Developer Documentation\n\nAll project contributors and participants are expected to adhere to the\n[Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md) ([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).\n\nThe `devel` branch has the latest (and potentially unstable) changes. The stable releases\nare tracked on [Github](https://github.com/enpaul/tox-poetry-installer/releases),\n[PyPi](https://pypi.org/project/tox-poetry-installer/#history), and in the\n[Changelog](CHANGELOG.md).\n\n- To report a bug, request a feature, or ask for assistance, please\n  [open an issue on the Github repository](https://github.com/enpaul/tox-poetry-installer/issues/new).\n- To report a security concern or code of conduct violation, please contact the project\n  author directly at **\u200cme \\[at\u200c\\] enp dot\u200e \u200cone**.\n- To submit an update, please\n  [fork the repository](https://docs.github.com/en/enterprise/2.20/user/github/getting-started-with-github/fork-a-repo)\n  and [open a pull request](https://github.com/enpaul/tox-poetry-installer/compare).\n\nDeveloping this project requires [Python 3.7+](https://www.python.org/downloads/) and\n[Poetry 1.2](https://python-poetry.org/docs/#installation) or later. GNU Make can\noptionally be used to quickly setup a local development environment, but this is not\nrequired.\n\nTo setup a local development environment:\n\n```bash\n# Clone the repository...\n# ...over HTTPS\ngit clone https://github.com/enpaul/tox-poetry-installer.git\n# ...over SSH\ngit clone git@github.com:enpaul/tox-poetry-installer.git\n\ncd tox-poetry-installer/\n\n# Create and configure the local development environment\nmake dev\n\n# Run tests and CI locally\nmake test\n\n# See additional make targets\nmake help\n```\n\n> **Note:** The pre-commit hooks require dependencies in the Poetry environment to run. To\n> make a commit with the pre-commit hooks, you will need to run `poetry run git commit` or,\n> alternatively, [launch an environment shell](https://python-poetry.org/docs/cli/#shell).\n\n## Road Map\n\nThis project is under active development and is classified as beta software, ready for\nproduction environments on a provisional basis only.\n\n- Beta classification was assigned with\n  [v0.6.0](https://github.com/enpaul/tox-poetry-installer/releases/tag/0.6.0)\n- Stable classification will be assigned when the test suite covers an acceptable number of\n  use cases\n\n### Path to Beta\n\n- [x] Verify that primary package dependencies (from the `.package` env) are installed\n  correctly using the Poetry backend.\n- [x] Support the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras) Tox\n  configuration option ([#4](https://github.com/enpaul/tox-poetry-installer/issues/4))\n- [x] Add per-environment Tox configuration option to fall back to default installation\n  backend.\n- [ ] ~Add warnings when an unsupported Tox configuration option is detected while using the\n  Poetry backend.~ ([#5](https://github.com/enpaul/tox-poetry-installer/issues/5))\n- [x] Add trivial tests to ensure the project metadata is consistent between the pyproject.toml\n  and the module constants.\n- [x] Update to use [poetry-core](https://github.com/python-poetry/poetry-core) and improve\n  robustness of the Tox and Poetry module imports to avoid potentially breaking API changes\n  in upstream packages. ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))\n- [ ] ~Find and implement a way to mitigate the\n  [UNSAFE_DEPENDENCIES issue](https://github.com/python-poetry/poetry/issues/1584) in\n  Poetry.~ ([#6](https://github.com/enpaul/tox-poetry-installer/issues/6))\n- [x] Fix logging to make proper use of Tox\'s logging reporter infrastructure ([#3](https://github.com/enpaul/tox-poetry-installer/issues/3))\n- [x] Add configuration option for installing all dev-dependencies to a testenv ([#14](https://github.com/enpaul/tox-poetry-installer/issues/14))\n\n### Path to Stable\n\nEverything in Beta plus...\n\n- [ ] Fully replace dependency on `poetry` with dependency on `poetry-core` ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))\n- [x] Add comprehensive unit tests\n- [ ] ~Add tests for each feature version of Tox between 3.8 and 3.20~\n- [x] Add tests for Python-3.6, 3.7, 3.8, and 3.9\n- [x] Add Github Actions based CI\n',
     'author': 'Ethan Paul',
     'author_email': '24588726+enpaul@users.noreply.github.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/enpaul/tox-poetry-installer/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.6.1,<4.0.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `tox-poetry-installer-0.8.5/PKG-INFO` & `tox-poetry-installer-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 Metadata-Version: 2.1
 Name: tox-poetry-installer
-Version: 0.8.5
+Version: 0.9.0
 Summary: A plugin for Tox that lets you install test environment dependencies from the Poetry lockfile
 Home-page: https://github.com/enpaul/tox-poetry-installer/
 License: MIT
 Keywords: tox,poetry,plugin
 Author: Ethan Paul
 Author-email: 24588726+enpaul@users.noreply.github.com
-Requires-Python: >=3.6.1,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Provides-Extra: poetry
-Requires-Dist: poetry (>=1.0.0,<1.2); extra == "poetry"
-Requires-Dist: poetry-core (>=1.0.0,<2.0.0)
+Requires-Dist: cleo (>=1.0.0a5,<2.0.0); extra == "poetry"
+Requires-Dist: poetry (>=1.2.0,<2.0.0); extra == "poetry"
+Requires-Dist: poetry-core (>=1.1.0,<2.0.0)
 Requires-Dist: tox (>=3.8.0,<4.0.0)
 Project-URL: Repository, https://github.com/enpaul/tox-poetry-installer/
 Description-Content-Type: text/markdown
 
 # tox-poetry-installer
 
 A plugin for [Tox](https://tox.readthedocs.io/en/latest/) that lets you install test
@@ -61,15 +66,15 @@
 - [Developing the Plugin](#developer-documentation)
 - [Road Map](#road-map)
 
 See the
 [Changelog](https://github.com/enpaul/tox-poetry-installer/blob/devel/CHANGELOG.md) for
 release history.
 
-*See also: [official Tox plugins](https://tox.readthedocs.io/en/latest/plugins.html), [Poetry-Dev-Dependencies Tox plugin](https://github.com/sinoroc/tox-poetry-dev-dependencies), [Poetry Tox plugin](https://github.com/tkukushkin/tox-poetry)*
+*See also: [official Tox plugins](https://tox.readthedocs.io/en/latest/plugins.html), [Poetry Tox plugin](https://github.com/tkukushkin/tox-poetry)*
 
 ## Feature Overview
 
 - Manage package versions in exactly one place and with exactly one tool: Poetry.
 - Ensure CI/CD and other automation tools are using the same package versions that you are
   in your local development environment.
 - Add only the packages you need to a Tox test environment, instead of everything in your
@@ -380,41 +385,34 @@
 - To report a security concern or code of conduct violation, please contact the project
   author directly at **‌me \[at‌\] enp dot‎ ‌one**.
 - To submit an update, please
   [fork the repository](https://docs.github.com/en/enterprise/2.20/user/github/getting-started-with-github/fork-a-repo)
   and [open a pull request](https://github.com/enpaul/tox-poetry-installer/compare).
 
 Developing this project requires [Python 3.7+](https://www.python.org/downloads/) and
-[Poetry 1.0](https://python-poetry.org/docs/#installation) or later. GNU Make can
+[Poetry 1.2](https://python-poetry.org/docs/#installation) or later. GNU Make can
 optionally be used to quickly setup a local development environment, but this is not
 required.
 
 To setup a local development environment:
 
 ```bash
 # Clone the repository...
 # ...over HTTPS
 git clone https://github.com/enpaul/tox-poetry-installer.git
 # ...over SSH
 git clone git@github.com:enpaul/tox-poetry-installer.git
 
 cd tox-poetry-installer/
 
-# Create and configure the local development environment...
-# ...with make:
+# Create and configure the local development environment
 make dev
-# ...manually:
-poetry install -E poetry --remove-untracked
-poetry run pre-commit install
 
-# Run tests and CI locally...
-# ...with make:
+# Run tests and CI locally
 make test
-# ...manually:
-poetry run tox --recreate
 
 # See additional make targets
 make help
 ```
 
 > **Note:** The pre-commit hooks require dependencies in the Poetry environment to run. To
 > make a commit with the pre-commit hooks, you will need to run `poetry run git commit` or,
```

