# Comparing `tmp/pynut3-1.2.5.tar.gz` & `tmp/pynut3-1.4.1.tar.gz`

## Comparing `pynut3-1.2.5.tar` & `pynut3-1.4.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pynut3-1.2.5/.editorconfig
--rw-r--r--   0        0        0    20692 2020-02-02 00:00:00.000000 pynut3-1.2.5/.pylintrc
--rwxr-xr-x   0        0        0     2217 2020-02-02 00:00:00.000000 pynut3-1.2.5/build
--rwxr-xr-x   0        0        0      817 2020-02-02 00:00:00.000000 pynut3-1.2.5/check
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pynut3-1.2.5/tox.ini
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 pynut3-1.2.5/.github/dependabot.yml
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 pynut3-1.2.5/demo/upsdemo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynut3-1.2.5/src/pynut3/__init__.py
--rw-r--r--   0        0        0    20468 2020-02-02 00:00:00.000000 pynut3-1.2.5/src/pynut3/nut3.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pynut3-1.2.5/.gitignore
--rw-r--r--   0        0        0    35068 2020-02-02 00:00:00.000000 pynut3-1.2.5/LICENSE
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 pynut3-1.2.5/README.md
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pynut3-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 pynut3-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pynut3-1.4.1/.editorconfig
+-rw-r--r--   0        0        0    20692 2020-02-02 00:00:00.000000 pynut3-1.4.1/.pylintrc
+-rwxr-xr-x   0        0        0     2217 2020-02-02 00:00:00.000000 pynut3-1.4.1/build
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pynut3-1.4.1/tox.ini
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 pynut3-1.4.1/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 pynut3-1.4.1/demo/upsdemo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynut3-1.4.1/src/pynut3/__init__.py
+-rw-r--r--   0        0        0    20270 2020-02-02 00:00:00.000000 pynut3-1.4.1/src/pynut3/nut3.py
+-rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 pynut3-1.4.1/.gitignore
+-rw-r--r--   0        0        0    35068 2020-02-02 00:00:00.000000 pynut3-1.4.1/LICENSE
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pynut3-1.4.1/README.md
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pynut3-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pynut3-1.4.1/PKG-INFO
```

### Comparing `pynut3-1.2.5/.pylintrc` & `pynut3-1.4.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `pynut3-1.2.5/build` & `pynut3-1.4.1/build`

 * *Files identical despite different names*

### Comparing `pynut3-1.2.5/.github/dependabot.yml` & `pynut3-1.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pynut3-1.2.5/demo/upsdemo.py` & `pynut3-1.4.1/demo/upsdemo.py`

 * *Files identical despite different names*

### Comparing `pynut3-1.2.5/src/pynut3/nut3.py` & `pynut3-1.4.1/src/pynut3/nut3.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 * PyNUT3Error: Base class for custom exceptions.
 * PyNUT3Client: Allows connecting to and communicating with PyNUT servers.
 
 Copyright (C) 2013 george2
 
 Modifications by mezz64 - 2016
-Modifications by Mausy5043 - 2022
+Modifications by Mausy5043 - 2023
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation; either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -28,15 +28,15 @@
 import logging
 import socket
 
 # TODO: implement telnetlib3 to replace deprecated telnetlib (PEP-594)
 from telnetlib import Telnet
 from typing import Any, Dict, List, Optional
 
-__version__ = "1.2.5"
+__version__ = "1.4.1"
 __all__ = ["PyNUT3Error", "PyNUT3Client"]
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class PyNUT3Error(Exception):
     """Base class for custom exceptions."""
@@ -67,17 +67,15 @@
                         to 5 seconds).
         persistent  : Boolean, when true connection will be made in init method
                         and be held open, when false connection is open/closed
                         when calling each method
         debug       : Boolean, put class in debug mode (prints everything
                         on console, defaults to False).
         """
-        _LOGGER.debug(
-            f"NUT Class initialization, Host/Port: {host}:{port}, Login: {login}"
-        )
+        _LOGGER.debug(f"NUT Class initialization, Host/Port: {host}:{port}, Login: {login}")
 
         self._debug = debug
         self._host: str = host
         self._port: int = port
         self._login: Optional[str] = login
         self._password: Optional[str] = password
         self._timeout: float = timeout
@@ -133,17 +131,15 @@
             raise PyNUT3Error("Socket error.") from exc
 
     def _read_until(self, string: str) -> str:
         """Wrapper for _srv_handler read_until method."""
         try:
             if self._srv_handler is None:
                 raise RuntimeError("NUT3 connection has not been opened.")
-            return self._srv_handler.read_until(
-                string.encode("ascii"), self._timeout
-            ).decode()
+            return self._srv_handler.read_until(string.encode("ascii"), self._timeout).decode()
         except (EOFError, BrokenPipeError):
             _LOGGER.error("NUT3 problem reading from server.")
             return ""
 
     def _write(self, string: str) -> None:
         """Wrapper for _srv_handler write method."""
         try:
@@ -384,19 +380,15 @@
         offset: int = len(f"ENUM {ups} {var}")
         end_offset: int = 0 - (len(f"END LIST ENUM {ups} {var}\n") + 1)
 
         if not self._persistent:
             self._disconnect()
 
         try:
-            return [
-                c[offset:].split('"')[1].strip()
-                for c in result[:end_offset].split("\n")
-                if '"' in c[offset:]
-            ]
+            return [c[offset:].split('"')[1].strip() for c in result[:end_offset].split("\n") if '"' in c[offset:]]
         except IndexError as exc:
             raise PyNUT3Error(result.replace("\n", "")) from exc
 
     def list_range(self, ups: str, var: str) -> List[str]:
         """Get a list of valid values for an range variable.
 
         The result is presented as a list.
@@ -415,19 +407,15 @@
         offset: int = len(f"RANGE {ups} {var}")
         end_offset: int = 0 - (len(f"END LIST RANGE {ups} {var}\n") + 1)
 
         if not self._persistent:
             self._disconnect()
 
         try:
-            return [
-                c[offset:].split('"')[1].strip()
-                for c in result[:end_offset].split("\n")
-                if '"' in c[offset:]
-            ]
+            return [c[offset:].split('"')[1].strip() for c in result[:end_offset].split("\n") if '"' in c[offset:]]
         except IndexError as exc:
             raise PyNUT3Error(result.replace("\n", "")) from exc
 
     def set_var(self, ups: str, var: str, value: str) -> None:
         """Set a variable to the specified value on selected UPS.
 
         The variable must be a writable value (cf list_rw_vars) and you
@@ -508,17 +496,15 @@
             assert result.startswith("TYPE")
             return type_
         except AssertionError as exc:
             raise PyNUT3Error(result.replace("\n", "")) from exc
 
     def command_description(self, ups: str, command: str) -> str:
         """Get a command's description."""
-        _LOGGER.debug(
-            f"NUT3 requesting command_description '{command}' on '{self._host}'."
-        )
+        _LOGGER.debug(f"NUT3 requesting command_description '{command}' on '{self._host}'.")
 
         if not self._persistent:
             self._connect()
 
         self._write(f"GET CMDDESC {ups} {command}\n")
         result: str = self._read_until("\n")
```

### Comparing `pynut3-1.2.5/.gitignore` & `pynut3-1.4.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Created by https://www.gitignore.io/api/python,pycharm
 # Edit at https://www.gitignore.io/?templates=python,pycharm
 
 ### local linting
 FIXME
 FIXME-2
+FIXME-SECURITY
+
 
 ### PyCharm ###
 .idea/
 
 ### Visual Studio ###
 .vscode/
```

### Comparing `pynut3-1.2.5/LICENSE` & `pynut3-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynut3-1.2.5/README.md` & `pynut3-1.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 Uninterruptible Power Supply servers.
 
 **Note**: This is an unofficial project, and is in no way supported or
 endorsed by the [Network UPS Tools developers](https://github.com/networkupstools).
 
 ## Requirements
 
-The module itself requires only Python3 (Python2 may work but is nolonger supported).
+The module itself requires only Python3. Python2 and all Python3 versions that have past their end-of-life date may still work but are nolonger supported.  
 
-## Installation
 
-    pip install pynut3
+## Installation
+```bash
+pip install pynut3
+```
 
 ## Usage
 
 Assuming you have a UPS which is connected to a host on the network with IP `192.168.2.17` it can be interogated as follows:
 
 ```python3
 from pynut3 import nut3
@@ -34,15 +36,15 @@
 for k1, v1 in ups_dict.items():
     print(f"{v1} is called with id {k1}")
     vars_dict = client.list_vars(k)
     for k2, v2 in vars_dict.items():
         print(f"{k2}\t:\t{v2}")
 ```
 
-Please note that this module has completely and intentionally broken backwards compatibility with previous versions of PyNUT.
+Please note that this module has completely and intentionally broken backwards compatibility with (previous) versions of PyNUT.
 
 ## Acknowledgements
 
 Based on various NUT Client related Python scripts, written by David Goncalves as [PyNUT](https://github.com/networkupstools/nut/tree/master/scripts/python), and released under GPL v3.   
 Later overhauled by rshipp with Python3 modifications by hordurk, george2 and mezz64.
 Others will have contributed along the way. I was not able to reliably find their names.
```

### Comparing `pynut3-1.2.5/pyproject.toml` & `pynut3-1.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pynut3"
 description = "A Python3 abstraction class to access NUT servers for uninterruptible power supplies (UPS)."
-version = "1.2.5"
+version = "1.4.1"
 dependencies = []
 license = "GPL-3.0-only"
 authors = [
   { name="Mausy5043" },
 ]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Power (UPS)"
 ]
```

### Comparing `pynut3-1.2.5/PKG-INFO` & `pynut3-1.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: pynut3
-Version: 1.2.5
+Version: 1.4.1
 Summary: A Python3 abstraction class to access NUT servers for uninterruptible power supplies (UPS).
 Project-URL: Homepage, https://github.com/Mausy5043/python-nut3
 Project-URL: Bug Tracker, https://github.com/Mausy5043/python-nut3/issues
 Author: Mausy5043
 License-Expression: GPL-3.0-only
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Power (UPS)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # pynut3 
 #### (aka python-nut3)
 
 
 [![PyPI version](https://img.shields.io/pypi/v/pynut3.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/pynut3)
@@ -33,19 +32,21 @@
 Uninterruptible Power Supply servers.
 
 **Note**: This is an unofficial project, and is in no way supported or
 endorsed by the [Network UPS Tools developers](https://github.com/networkupstools).
 
 ## Requirements
 
-The module itself requires only Python3 (Python2 may work but is nolonger supported).
+The module itself requires only Python3. Python2 and all Python3 versions that have past their end-of-life date may still work but are nolonger supported.  
 
-## Installation
 
-    pip install pynut3
+## Installation
+```bash
+pip install pynut3
+```
 
 ## Usage
 
 Assuming you have a UPS which is connected to a host on the network with IP `192.168.2.17` it can be interogated as follows:
 
 ```python3
 from pynut3 import nut3
@@ -55,15 +56,15 @@
 for k1, v1 in ups_dict.items():
     print(f"{v1} is called with id {k1}")
     vars_dict = client.list_vars(k)
     for k2, v2 in vars_dict.items():
         print(f"{k2}\t:\t{v2}")
 ```
 
-Please note that this module has completely and intentionally broken backwards compatibility with previous versions of PyNUT.
+Please note that this module has completely and intentionally broken backwards compatibility with (previous) versions of PyNUT.
 
 ## Acknowledgements
 
 Based on various NUT Client related Python scripts, written by David Goncalves as [PyNUT](https://github.com/networkupstools/nut/tree/master/scripts/python), and released under GPL v3.   
 Later overhauled by rshipp with Python3 modifications by hordurk, george2 and mezz64.
 Others will have contributed along the way. I was not able to reliably find their names.
```

