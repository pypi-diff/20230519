# Comparing `tmp/hspylib-cfman-0.9.9.tar.gz` & `tmp/hspylib-cfman-0.9.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-cfman-0.9.9.tar", last modified: Tue Feb 22 22:53:31 2022, max compression
+gzip compressed data, was "hspylib-cfman-0.9.90.tar", last modified: Fri May 19 18:15:24 2023, max compression
```

## Comparing `hspylib-cfman-0.9.9.tar` & `hspylib-cfman-0.9.90.tar`

### file list

```diff
@@ -1,31 +1,28 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.889535 hspylib-cfman-0.9.9/
--rw-r--r--   0 hjunior    (504) staff       (20)      125 2022-02-18 20:26:15.000000 hspylib-cfman-0.9.9/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)      692 2022-02-22 22:53:31.888630 hspylib-cfman-0.9.9/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)       56 2022-02-13 18:53:57.000000 hspylib-cfman-0.9.9/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.853447 hspylib-cfman-0.9.9/cfman/
--rw-r--r--   0 hjunior    (504) staff       (20)        5 2022-02-22 22:53:29.000000 hspylib-cfman-0.9.9/cfman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      180 2022-02-22 19:08:33.000000 hspylib-cfman-0.9.9/cfman/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2857 2022-02-22 01:53:41.000000 hspylib-cfman-0.9.9/cfman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.861883 hspylib-cfman-0.9.9/cfman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      208 2022-02-22 19:08:33.000000 hspylib-cfman-0.9.9/cfman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3953 2022-02-15 20:32:21.000000 hspylib-cfman-0.9.9/cfman/core/cf.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2343 2022-02-22 02:28:30.000000 hspylib-cfman-0.9.9/cfman/core/cf_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)      721 2022-02-15 20:32:22.000000 hspylib-cfman-0.9.9/cfman/core/cf_endpoint.py
--rw-r--r--   0 hjunior    (504) staff       (20)    10821 2022-02-22 02:29:52.000000 hspylib-cfman-0.9.9/cfman/core/cf_manager.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.865348 hspylib-cfman-0.9.9/cfman/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      165 2022-02-22 19:08:33.000000 hspylib-cfman-0.9.9/cfman/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      771 2022-02-11 19:26:38.000000 hspylib-cfman-0.9.9/cfman/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.866996 hspylib-cfman-0.9.9/cfman/resources/
--rw-r--r--   0 hjunior    (504) staff       (20)        0 2022-02-02 16:37:07.000000 hspylib-cfman-0.9.9/cfman/resources/application.properties
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.871837 hspylib-cfman-0.9.9/cfman/resources/log/
--rw-r--r--   0 hjunior    (504) staff       (20)        0 2022-02-02 16:37:07.000000 hspylib-cfman-0.9.9/cfman/resources/log/.gitkeep
--rw-r--r--   0 hjunior    (504) staff       (20)     1180 2022-02-22 06:29:07.000000 hspylib-cfman-0.9.9/cfman/resources/log/application.log
--rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.9/cfman/welcome.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.887321 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)      692 2022-02-22 22:53:31.000000 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      565 2022-02-22 22:53:31.000000 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2022-02-22 22:53:31.000000 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       36 2022-02-22 22:53:31.000000 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2022-02-22 22:53:31.000000 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2022-02-22 22:53:31.889698 hspylib-cfman-0.9.9/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1572 2022-02-15 20:32:22.000000 hspylib-cfman-0.9.9/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:15:24.774511 hspylib-cfman-0.9.90/
+-rw-r--r--   0 hjunior    (504) staff       (20)       49 2022-02-23 03:43:53.000000 hspylib-cfman-0.9.90/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-05-19 18:15:24.772963 hspylib-cfman-0.9.90/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      677 2023-05-19 18:15:23.000000 hspylib-cfman-0.9.90/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:15:24.707268 hspylib-cfman-0.9.90/cfman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-05-19 18:15:23.000000 hspylib-cfman-0.9.90/cfman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      716 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.90/cfman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-05-19 18:15:23.000000 hspylib-cfman-0.9.90/cfman/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3595 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.90/cfman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:15:24.727146 hspylib-cfman-0.9.90/cfman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      238 2023-05-19 18:15:23.000000 hspylib-cfman-0.9.90/cfman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7619 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.90/cfman/core/cf.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2950 2023-05-17 21:37:29.000000 hspylib-cfman-0.9.90/cfman/core/cf_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5534 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.90/cfman/core/cf_blue_green_checker.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1234 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.90/cfman/core/cf_endpoint.py
+-rw-r--r--   0 hjunior    (504) staff       (20)    15395 2023-05-17 21:37:29.000000 hspylib-cfman-0.9.90/cfman/core/cf_manager.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:15:24.736126 hspylib-cfman-0.9.90/cfman/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-05-19 18:15:23.000000 hspylib-cfman-0.9.90/cfman/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      845 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.90/cfman/exception/exceptions.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.90/cfman/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:15:24.769586 hspylib-cfman-0.9.90/hspylib_cfman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-05-19 18:15:24.000000 hspylib-cfman-0.9.90/hspylib_cfman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      520 2023-05-19 18:15:24.000000 hspylib-cfman-0.9.90/hspylib_cfman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-05-19 18:15:24.000000 hspylib-cfman-0.9.90/hspylib_cfman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       28 2023-05-19 18:15:24.000000 hspylib-cfman-0.9.90/hspylib_cfman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-05-19 18:15:24.000000 hspylib-cfman-0.9.90/hspylib_cfman.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-05-19 18:15:24.774722 hspylib-cfman-0.9.90/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1934 2023-04-19 22:13:46.000000 hspylib-cfman-0.9.90/setup.py
```

### Comparing `hspylib-cfman-0.9.9/cfman/__main__.py` & `hspylib-cfman-0.9.90/cfman/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,98 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   TODO Purpose of the file
-   @project: HSPyLib
-   hspylib.app.cfman.src.main
+   @project: HsPyLib-CFMan
+   @package: cfman
       @file: __main__.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2021, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
+from cfman.__classpath__ import _Classpath
+from cfman.core.cf_manager import CFManager
+from clitt.core.tui.tui_application import TUIApplication
+from hspylib.core.enums.charset import Charset
+from hspylib.core.zoned_datetime import now
+from hspylib.modules.application.argparse.parser_action import ParserAction
+from hspylib.modules.application.exit_status import ExitStatus
+from hspylib.modules.application.version import Version
+from hspylib.modules.cli.vt100.vt_utils import clear_screen, prepare_render
+from textwrap import dedent
+
 import logging as log
 import os
 import sys
-from datetime import datetime
-from textwrap import dedent
-
-from hspylib.core.tools.commons import get_path
-from hspylib.modules.cli.application.application import Application
-from hspylib.modules.cli.application.version import AppVersion
-
-from cfman.core.cf_manager import CFManager
 
-HERE = get_path(__file__)
 
-log.captureWarnings(True)
-
-
-class Main(Application):
+class Main(TUIApplication):
     """Cloud Foundry Manager - Manage PCF applications."""
 
     # The welcome message
-    DESCRIPTION = (HERE / "welcome.txt").read_text()
+    DESCRIPTION = _Classpath.get_source_path("welcome.txt").read_text(encoding=Charset.UTF_8.val)
+
+    # location of the .version file
+    VERSION_DIR = _Classpath.source_path()
 
     def __init__(self, app_name: str):
-        version = AppVersion.load()
+        version = Version.load(load_dir=self.VERSION_DIR)
         super().__init__(app_name, version, self.DESCRIPTION.format(version))
-        self.cfman = None
+        self._cf_manager = None
 
     def _setup_arguments(self) -> None:
-        """Initialize application parameters and options"""
+        """Initialize application parameters and options."""
+        # fmt: off
         self._with_options() \
-            .option('api', 'a', 'api', 'the API endpoint to connect to (e.g. https://api.example.com)', nargs='?') \
-            .option('org', 'o', 'org', 'the organization to connect to (Target organization)', nargs='?') \
-            .option('space', 's', 'space', 'the space to connect to (Target organization space)', nargs='?') \
-            .option('username', 'u', 'username', 'the PCF username', nargs='?') \
-            .option('password', 'p', 'password', 'the PCF password', nargs='?') \
+            .option("api", "a", "api", "the API endpoint to connect to (e.g. https://api.example.com)", nargs="?")\
+            .option("org", "o", "org", "the organization to connect to (Target organization)", nargs="?")\
+            .option("space", "s", "space", "the space to connect to (Target organization space)", nargs="?")\
+            .option("username", "u", "username", "the PCF username", nargs="?")\
+            .option("password", "p", "password", "the PCF password", nargs="?")\
             .option(
-                'endpoints', 'f', 'endpoints',
-                'the file containing the CF API endpoint entries. If not provided, '
-                '$HOME/cf_endpoints.txt will be used instead.', nargs=1)
-
-    def _main(self, *params, **kwargs) -> None:
-        """Run the application with the command line arguments"""
-        self.cfman = CFManager(
-            self.getarg('api'), self.getarg('org'), self.getarg('space'),
-            self.getarg('username'), self.getarg('password'),
-            self.getarg('endpoints') or os.getenv('HOME', os.getcwd()) + '/cf_endpoints.txt'
+                "no-cache", "r", "no-cache", "avoiding using cached apps",
+                nargs="?", action=ParserAction.STORE_TRUE)\
+            .option(
+                "endpoints", "f", "endpoints",
+                "the file containing the CF API endpoint entries. "
+                "If not provided, '$HOME/cf_endpoints.txt' will be used instead.",
+                nargs=1
+            )
+        # fmt: on
+
+    def _main(self, *params, **kwargs) -> ExitStatus:
+        """Run the application with the command line arguments."""
+        self._cf_manager = CFManager(
+            self.get_arg("api"),
+            self.get_arg("org"),
+            self.get_arg("space"),
+            self.get_arg("username"),
+            self.get_arg("password"),
+            self.get_arg("no-cache"),
+            self.get_arg("endpoints") or f"{os.getenv('HOME', os.getcwd())}/.cfman_endpoints.txt",
         )
-        log.info(dedent('''
-        {} v{}
+        log.info(
+            dedent(
+                f"""
+        {self._app_name} v{self._app_version}
 
         Settings ==============================
-                STARTED: {}
-        ''').format(self._app_name, self._app_version, datetime.now().strftime("%Y-%m-%d %H:%M:%S")))
-        self._exec_application()
-
-    def _exec_application(self) -> None:
-        """Execute the application"""
-        self.cfman.run()
+                STARTED: {now("%Y-%m-%d %H:%M:%S")}
+        """
+            )
+        )
+        return self._exec_application()
+
+    def _exec_application(self) -> ExitStatus:
+        """Execute the application."""
+        prepare_render()
+        self._cf_manager.run()
+        clear_screen()
+        return ExitStatus.SUCCESS
 
 
 if __name__ == "__main__":
     # Application entry point
-    Main('HSPyLib Cloud Foundry Manager').INSTANCE.run(sys.argv[1:])
+    Main("cfman").INSTANCE.run(sys.argv[1:])
```

### Comparing `hspylib-cfman-0.9.9/cfman/core/cf_application.py` & `hspylib-cfman-0.9.90/cfman/core/cf_application.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   TODO Purpose of the file
-   @project: HSPyLib
-   hspylib.app.cfman.core
+   @project: HsPyLib-CFMan
+   @package: cfman.core
       @file: cf_application.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2021, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
-
-import re
-from typing import List
-
+from clitt.core.tui.tui_preferences import TUIPreferences
 from hspylib.core.exception.exceptions import InvalidArgumentError
 from hspylib.core.tools.commons import sysout
+from typing import List
+
+import re
 
 
 class CFApplication:
+    """Represent a PCF application."""
+
     max_name_length = 70
 
     @classmethod
     def of(cls, app_line: str):
-        """TODO"""
-        parts = re.split(r' {2,}', app_line)
+        """Create a cf application entry from the cf apps output line."""
+        parts = re.split(r" {2,}", app_line)
         # format: name | state | instances | memory | disk | urls
-        if len(parts) == 6:
-            return CFApplication(parts[0], parts[1], parts[2], parts[3], parts[4], parts[5].split(', '))
-        # format: name | state | type:i/o | urls
-        elif len(parts) == 4:
-            mat = re.search("(\w+):(\d+/\d+)", parts[2])
-            if not mat:
-                raise InvalidArgumentError(f"Invalid application line: {app_line}")
+        if len(parts) == 6:  # Old CF command output
+            return CFApplication(parts[0], parts[1], parts[2], parts[3], parts[4], parts[5].split(", "))
+        # format: name | requested state | processes | routes
+        elif len(parts) == 4:  # New CF command output
+            if not (mat := re.search(r"(\w+):(\d+/\d+)", parts[2])):
+                raise InvalidArgumentError(f'Invalid application line: "{app_line}"')
             instances = mat.group(2)
-            memory = '-'
-            disk = '-'
-            return CFApplication(parts[0], parts[1], instances, memory, disk, parts[3].split(', '))
-        else:
-            raise InvalidArgumentError(f"Invalid application line: {app_line}")
-
-    def __init__(
-        self,
-        name: str,
-        state: str,
-        instances: str,
-        memory: str,
-        disk: str,
-        urls: List[str]):
+            memory = disk = "-"
+            return CFApplication(parts[0], parts[1], instances, memory, disk, parts[3].split(","))
+
+        raise InvalidArgumentError(
+            f"Invalid application line: " f"{app_line}" f"Probably CF APPS command changed the command output."
+        )
+
+    def __init__(self, name: str, state: str, instances: str, memory: str, disk: str, routes: List[str]) -> None:
+        self.prefs: TUIPreferences = TUIPreferences.INSTANCE or TUIPreferences()
         self.name = name
         self.state = state
         self.instances = instances
         self.memory = memory
         self.disk = disk
-        self.urls = urls
+        self.routes = routes
         self.max_name_length = max(self.max_name_length, len(self.name))
 
-    def __str__(self):
-        return self.name
+    def __str__(self) -> str:
+        return f"[{self.colored_state}] {self.name}"
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return str(self)
 
-    # pylint: disable=consider-using-f-string
-    def print_status(self):
-        """TODO"""
-        sysout("%CYAN%{}  %{}%{:5}  %NC%{:10}  {:4}  {:4}  {}".format(
-            self.name.ljust(self.max_name_length),
-            'GREEN' if self.state == 'started' else 'RED',
-            self.state,
-            self.instances,
-            self.memory,
-            self.disk,
-            self.urls
-        ))
-
+    @property
+    def colored_state(self) -> str:
+        """Return the actual application state using colors."""
+        state = self.state.upper()
+        return (
+            f"{self.prefs.success_color if self.is_started else self.prefs.error_color}"
+            f"{state:<7}{self.prefs.text_color.code}"
+        )
+
+    @property
+    def is_started(self) -> bool:
+        return self.state.lower() == "started"
+
+    def print_status(self) -> None:
+        """Print the actual application status line."""
+        sysout(
+            f"%CYAN%{self.name:<{self.max_name_length + 2}}"
+            f"{self.colored_state:}  %NC%{self.instances:<12}{self.memory:<6}{self.disk:<6}{len(self.routes)}"
+        )
```

### Comparing `hspylib-cfman-0.9.9/cfman/core/cf_manager.py` & `hspylib-cfman-0.9.90/cfman/core/cf_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,266 +1,378 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   TODO Purpose of the file
-   @project: HSPyLib
-   hspylib.app.cfman.core
+   @project: HsPyLib-CFMan
+   @package: cfman.core
       @file: cf_manager.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2021, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
-import sys
-from time import sleep
-from typing import List, Optional
-
-from hspylib.core.config.app_config import AppConfigs
-from hspylib.core.enums.http_code import HttpCode
-from hspylib.core.tools.commons import file_is_not_empty, syserr, sysout
-from hspylib.modules.cli.tui.extra.mchoose import mchoose
-from hspylib.modules.cli.tui.extra.minput.minput import MenuInput, minput
-from hspylib.modules.cli.tui.extra.mselect import mselect
-from hspylib.modules.cli.tui.menu.menu_utils import MenuUtils
-from hspylib.modules.fetch.fetch import head
-
 from cfman.core.cf import CloudFoundry
 from cfman.core.cf_application import CFApplication
+from cfman.core.cf_blue_green_checker import CFBlueGreenChecker
 from cfman.core.cf_endpoint import CFEndpoint
 from cfman.exception.exceptions import CFAuthenticationError, CFConnectionError, CFExecutionError
+from clitt.core.tui.mchoose.mchoose import mchoose
+from clitt.core.tui.menu.tui_menu_utils import TUIMenuUtils
+from clitt.core.tui.minput.minput import MenuInput, minput
+from clitt.core.tui.mselect.mselect import mselect
+from functools import partial
+from hspylib.core.enums.http_code import HttpCode
+from hspylib.core.preconditions import check_state
+from hspylib.core.tools.commons import syserr, sysout
+from hspylib.modules.cache.ttl_cache import TTLCache
+from hspylib.modules.cli.vt100.vt_utils import clear_screen
+from hspylib.modules.fetch.fetch import head
+from retry import retry
+from time import sleep
+from typing import List, Optional, Tuple
+
+import requests
+import sys
 
 
 class CFManager:
-    """Represents the cloud foundry manager application and it's functionalities"""
+    """Responsible for the CloudFoundry application functionalities."""
 
-    CF_ACTIONS = [
-        'Logs',
-        'Restart',
-        'Restage',
-        'Status',
-        'Start',
-        'Stop',
-        'Target',
+    CFMAN_ACTIONS = [
+        "Information",
+        "Target",
+        "Logs",
+        "Start",
+        "Stop",
+        "Restart",
+        "Restage",
+        "Status",
+        "Blue-Green-Check",
     ]
 
     @staticmethod
     def _abort():
+        """Abort the execution and exit."""
         sys.exit(1)
 
     @staticmethod
     def _allow_multiple(action: str) -> bool:
-        """Checks whether the action allows multiple apps selection or not"""
-        return action.lower() not in ['logs', 'target']
+        """Whether the action allows multiple application selection or not.
+        :param action the action to check
+        """
+        return action.lower() in ["start", "stop", "restart", "restage"]
 
     @staticmethod
     def _is_callable(action: str) -> bool:
-        """Checks whether the action is callable or not"""
-        return action.lower() not in ['status', 'target']
+        """Whether the provided action is callable or not.
+        :param action the action to check
+        """
+        return action.lower() in ["logs", "start", "stop", "restart", "restage"]
+
+    @staticmethod
+    def required_states(action: str) -> str | Tuple[str, str]:
+        """Return the required application statue of the provided action
+        :param action the action to check
+        """
+        match action:
+            case "start":
+                return "stopped"
+            case "logs" | "stop" | "restart":
+                return "started"
+            case _:
+                return "started", "stopped"
 
-    def __init__(self, api: str, org: str, space: str, username: str, password: str, cf_endpoints: str):
-        assert file_is_not_empty(cf_endpoints), \
-            f'CF Endpoints file {cf_endpoints} is empty or does not exist !'
-        self.configs = AppConfigs.INSTANCE
+    def __init__(self, api: str, org: str, space: str, username: str, password: str, no_cache: str, cf_endpoints: str):
         self._cf = CloudFoundry()
+        self._cache = TTLCache()
         self._api = api
         self._org = org
         self._space = space
         self._username = username
         self._password = password
+        self._no_cache = no_cache or False
         self._cf_endpoints_file = cf_endpoints
         self._cf_apps = None
         self._done = False
 
+    def __str__(self) -> str:
+        return (
+            f"%EOL%%GREEN%"
+            f"{'-=' * 40} %EOL%"
+            f"{self._api} %EOL%"
+            f"{'--' * 40} %EOL%"
+            f"{'USER:':>6} {self._username}%EOL%"
+            f"{'ORG:':>6} {self._org}%EOL%"
+            f"{'SPACE:':>6} {self._space}%EOL%"
+            f"{'-=' * 40}"
+        )
+
+    def __repr__(self) -> str:
+        return str(self)
+
+    @property
+    def apps(self) -> List[CFApplication]:
+        return self._get_apps() or []
+
     def run(self) -> None:
-        """Execute main cf manager routines"""
-        sysout('%GREEN%Checking CloudFoundry authorization...')
-        if self._cf.connect():
-            sysout('%GREEN%Already authorized to CloudFoundry!')
+        """Run the main cf manager application flow."""
+        sysout("%BLUE%Checking CloudFoundry authorization...")
+        if self._cf.is_logged():
+            self._api = self._cf.api()
+            target = self._cf.target()
+            self._username, self._org, self._space = target.user, target.org, target.space
+            sysout("%YELLOW%Already authorized to CloudFoundry!")
         else:
             authorized = False
-            sysout('%YELLOW%Not authorized to CloudFoundry, login required...')
+            sysout("%YELLOW%Unauthorized to CloudFoundry, login required...")
+            sleep(2)
             while not authorized:
                 if not self._api:
-                    sleep(1)
                     self._select_endpoint()
                 if not self._username or not self._password:
-                    sleep(1)
-                    self._require_credentials()
-                sysout(f'%GREEN%Authorizing {self._username}@{self._api}...')
+                    self._prompt_credentials()
+                sysout(f"%BLUE%Authorizing {self._username}@{self._api}...")
                 authorized = self._authorize()
                 if not authorized:
                     self._password = None
-                    sleep(1)
-            sysout('%GREEN%Successfully authorized!')
-
+                    syserr("Not authorized !")
+                    self._abort()
+            sysout("%GREEN%Successfully authorized!")
+        sysout(f"%HOM%%ED0%%WHITE%--- Target information ---%EOL%{self}")
+        TUIMenuUtils.wait_keystroke()
         self._loop_actions()
 
-    def _get_apps(self, refresh: bool = False) -> List[CFApplication]:
-        """Retrieve all cf applications under the target/org"""
-        if refresh or not self._cf_apps:
-            sysout(f'%GREEN%Retrieving applications from space: "{self._space}"...')
-            apps = self._cf.apps()
-            apps = list(map(CFApplication.of, apps if apps else []))
-            if not apps:
-                if "OK" not in self._cf.last_result:
-                    raise CFExecutionError(f'Unable to retrieve applications: => {self._cf.last_result}')
-                sysout('%YELLOW%No apps found')
-            self._cf_apps = apps
-
-        return self._cf_apps
-
+    @retry(exceptions=CFConnectionError, tries=3, delay=2, backoff=3, max_delay=30)
     def _select_endpoint(self) -> None:
-        """Select the PCF endpoint to connect to"""
+        """Select the PCF endpoint to connect to."""
         try:
-            with open(self._cf_endpoints_file, 'r', encoding='utf-8') as f_hosts:
-                endpoints = list(map(lambda l: CFEndpoint(l.split(',')), f_hosts.readlines()))
+            with open(self._cf_endpoints_file, "r", encoding="utf-8") as f_hosts:
+                endpoints = list(map(lambda l: CFEndpoint(*l.strip().split(",")), f_hosts.readlines()))
                 if len(endpoints) > 0:
-                    selected = mselect(endpoints, title='Please select an endpoint')
+                    selected = mselect(endpoints, title="Please select an endpoint")
                     if not selected:
                         self._abort()
-                    sysout(f"%GREEN%Connecting to endpoint: {selected}...")
+                    sysout(f"%BLUE%Connecting to endpoint: {selected}...")
                     try:
                         response = head(selected.host)
                         if response.status_code and HttpCode.OK:
                             self._api = selected.host
                         else:
-                            syserr(f'Failed to connect to API ({response.status_code}): {selected}')
+                            syserr(
+                                CFConnectionError(
+                                    f"Failed to contact CF API %EOL%" f"  Status: ({response.status_code}): {selected}"
+                                )
+                            )
                             self._abort()
-                    except Exception as err:
-                        raise CFConnectionError(f'Failed to connect to API => {selected.host}') from err
+                    except requests.exceptions.ConnectionError as err:
+                        syserr(
+                            CFConnectionError(
+                                f"Failed to connect to CloudFoundry API%EOL%"
+                                f"  Host: '{selected.host}'%EOL%"
+                                f"  => {err.__class__.__name__}"
+                            )
+                        )
+                        self._abort()
                 else:
-                    syserr(f"No endpoint yet configured. Please create the file {self._cf_endpoints_file} "
-                           f"with at least one endpoint configured and try again.")
+                    syserr(
+                        CFExecutionError(
+                            f'No endpoint yet configured. Please create the file "{self._cf_endpoints_file}" '
+                            f"with at least one endpoint and try again!"
+                        )
+                    )
                     self._abort()
-        except IndexError:
-            syserr(f'{self._cf_endpoints_file} '
-                   f'has invalid cf endpoints format. Please use: <alias>, <url>, <protected [true,false]>')
+        except (IndexError, FileNotFoundError) as err:
+            syserr(
+                CFExecutionError(
+                    f'Endpoint file "{self._cf_endpoints_file}" is invalid: %EOL%'
+                    f"  => {str(err)}! %EOL%"
+                    f"Make sure it exists contains the following: %EOL%"
+                    f"<alias>,<cf_api_url>,<protected [true|false]>%EOL%"
+                )
+            )
             self._abort()
 
-    def _require_credentials(self) -> None:
-        """Prompt the user for PCF credentials"""
-        form_fields = MenuInput.builder() \
-            .field().label('Username').value(self._username).build() \
-            .field().label('Password').itype('password').value(self._password).build() \
+    def _prompt_credentials(self) -> None:
+        """Prompt the user for his PCF credentials."""
+        # fmt: off
+        form_fields = (
+            MenuInput.builder()
+                .field()
+                    .label("Username")
+                    .value(self._username)
+                    .build()
+                .field()
+                    .label("Password")
+                    .itype("password")
+                    .value(self._password)
+                    .build()
             .build()
-        result = minput(form_fields, title='Please type your Cloud Foundry credentials')
+        )
+        # fmt: on
+        result = minput(form_fields, title="Please type your Cloud Foundry credentials")
         if result:
             self._username = result.username
             self._password = result.password
         else:
             self._abort()
 
     def _authorize(self) -> bool:
-        """Send an authorization request to PCF"""
+        """Send an authorization request to PCF."""
         if not self._cf.api(self._api):
-            raise CFExecutionError(f'Unable to set API: => {self._cf.last_result}')
+            raise CFExecutionError(f"Unable to set API: => {self._cf.last_output}")
         if not self._cf.auth(self._username, self._password):
-            raise CFAuthenticationError(f'Unable to authenticate to => {self._api}')
+            raise CFAuthenticationError(f"Unable to authenticate to => {self._api}")
 
         return True
 
     def _set_org(self) -> None:
-        """Set the active organization"""
+        """Set the active PCF organization."""
         if not self._org:
-            sysout('%YELLOW%Checking organization...')
-            orgs = self._cf.orgs()
-            if not orgs:
-                raise CFExecutionError(f'Unable to retrieve organizations: => {self._cf.last_result}')
-            self._org = mselect(orgs, title='Please select the organization')
+            sysout(f'%BLUE%Retrieving all organizations from api: "{self._api}"...')
+            if not (orgs := self._cf.orgs()):
+                raise CFExecutionError(f"Unable to retrieve organizations: => {self._cf.last_output}")
+            self._org = mselect(orgs, title="Please select the PCF organization")
             if not self._org:
                 self._abort()
             else:
                 self._target()
 
     def _set_space(self) -> None:
-        """Set the active space"""
+        """Set the active PCF space."""
         if not self._space:
-            sysout('%YELLOW%Checking space...')
-            spaces = self._cf.spaces()
+            if self._no_cache or not (spaces := self._cache.read(f"cf-spaces-{self._org}")):
+                sysout(f'%BLUE%Retrieving all spaces from org: "{self._org}"...')
+                spaces = self._cf.spaces()
+                self._cache.save(f"cf-spaces-{self._org}", spaces)
             if not spaces:
-                raise CFExecutionError(f'Unable to retrieve spaces: => {self._cf.last_result}')
-            self._space = mselect(spaces, title='Please select a space')
+                raise CFExecutionError(f"Unable to retrieve org={self._org} spaces: => {self._cf.last_output}")
+            self._space = mselect(spaces, title="Please select the PCF space")
             if not self._space:
                 self._abort()
             else:
                 self._target()
 
-    def _choose_apps(self) -> Optional[List[CFApplication]]:
-        """Choose multiple PCF apps from the available list"""
+    def _get_apps(self) -> List[CFApplication]:
+        """Retrieve all cf applications under the targeted org-space."""
+        if self._no_cache or not (apps := self._cache.read(f"cf-apps-{self._space}")):
+            sysout(f'%BLUE%Retrieving applications from space: "{self._space}"...')
+            apps = self._cf.apps()
+            sysout(f'%GREEN%Found {len(apps)} apps in space: "{self._space}"')
+            self._cache.save(f"cf-apps-{self._space}", apps)
+        if not apps:
+            if "OK" not in self._cf.last_output:
+                raise CFExecutionError(f"Unable to retrieve applications: => {self._cf.last_output}")
+            syserr(f'%YELLOW%No applications found for space: "{self._space}"')
+        cf_apps = list(map(CFApplication.of, apps if apps else []))
+        self._cf_apps = cf_apps
+
+        return self._cf_apps
+
+    def _choose_apps(self, required_states: str | Tuple[str, str]) -> Optional[List[CFApplication]]:
+        """Choose multiple PCF apps from the available list.
+        :param required_states used to filter the apps to choose by the application state.
+        """
+        self._cf_apps = list(filter(lambda app: app.state.lower() in required_states, self.apps))
         if not self._cf_apps:
-            self._cf_apps = self._get_apps()
-        return mchoose(self._cf_apps, checked=False, title='Please choose the applications you want to manage')
+            return None
+        return mchoose(self._cf_apps, checked=False, title="Please choose the applications you want to manage")
 
-    def _select_app(self) -> Optional[CFApplication]:
-        """Select a single PCF app from the available list"""
+    def _select_app(self, required_states: str | Tuple[str, str]) -> Optional[CFApplication]:
+        """Select a single PCF app from the available list.
+        :param required_states used to filter the apps to choose by the application state.
+        """
+        self._cf_apps = list(filter(lambda app: app.state.lower() in required_states, self.apps))
         if not self._cf_apps:
-            self._cf_apps = self._get_apps()
-        return mselect(self._cf_apps, title='Please select the application you want to manage')
+            return None
+        return mselect(self._cf_apps, title="Please select the application you want to manage")
 
     def _target(self) -> None:
-        """Send a target request to PCF"""
-        sysout(f"%GREEN%Targeting ORG={self._org} and SPACE={self._space}...")
-        if not self._cf.target(org=self._org, space=self._space):
-            raise CFExecutionError(f"Unable to target ORG: {self._org} => {self._cf.last_result}")
+        """Attempt to target to a PCF org-space."""
+        if not self._cf.target(user=self._username, org=self._org, space=self._space):
+            raise CFExecutionError(f"Unable to target ORG: {self._org} => {self._cf.last_output}")
+        sleep(1)
 
     def _loop_actions(self) -> None:
-        """Wait for the user interactions"""
-        while not self._done:
-            if self._org and self._space and not self._cf.is_targeted():
-                self._target()
-            else:
-                self._set_org()
-                self._set_space()
-
-            if not self._org or not self._space or not self._cf.is_targeted():
-                raise CFExecutionError(
-                    f"Unable to target ORG={self._org}  SPACE={self._space} => {self._cf.last_result}")
-
-            action = mselect(CFManager.CF_ACTIONS, 'Please select an action to perform')
-
-            if not action:
+        """Wait for the user interactions."""
+        while self._assert_target():
+            if not (action := mselect(CFManager.CFMAN_ACTIONS, "Please select an action to perform")):
                 self._done = True
+                return
+            if self._is_callable(action):
+                self._perform_callable(action)
             else:
-                if self._is_callable(action):
-                    self._perform_callable(action)
-                else:
-                    if action.lower() == 'status':
+                match action.lower():
+                    case "status":
                         self._display_app_status()
-                    elif action.lower() == 'target':
+                    case "target":
                         self._space = self._org = self._cf_apps = None
-                        self._cf.targeted = {'org': None, 'space': None, 'targeted': False}
+                        self._cf.clear_target()
                         continue
+                    case "blue-green-check":
+                        self._blue_green_check()
+                    case "information":
+                        sysout(f"%HOM%%ED0%%WHITE%--- Target information ---%EOL%{self}")
+
+                TUIMenuUtils.wait_keystroke()
 
-                    MenuUtils.wait_enter()
+    def _assert_target(self) -> bool:
+        if not self._org:
+            self._set_org()
+        if not self._space:
+            self._set_space()
+        if not self._cf.is_targeted():
+            self._target()
+        if not self._org or not self._space or not self._cf.is_targeted():
+            raise CFExecutionError(f"Unable to target ORG={self._org}  SPACE={self._space} => {self._cf.last_output}")
+        return not self._done
+
+    def _display_app_status(self) -> None:
+        """Display all PCF space-application statuses."""
+        apps = self.apps
 
-    def _display_app_status(self):
-        """Display select apps status"""
-        apps = self._get_apps(refresh=True)
         if len(apps) > 0:
-            # pylint: disable=consider-using-f-string
-            sysout("%WHITE%{}  {}  {}  {}  {}  {}".format(
-                'Name'.ljust(CFApplication.max_name_length),
-                'State'.ljust(7), 'Instances'.ljust(10), 'Mem'.ljust(4),
-                'Disk'.ljust(4), 'URLs',
-            ))
-            for app in apps:
-                app.print_status()
-
-    def _perform_callable(self, action):
-        """Perform the selected callable action"""
-        if self._allow_multiple(action.lower()):
-            apps = self._choose_apps()
+            clear_screen()
+            # fmt: off
+            sysout(
+                f"%BLUE%Listing '{self._org}::{self._space}' applications ...%EOL%%WHITE%"
+                f"{'-=' * 60 + '%EOL%'}"
+                f"{'Name':{CFApplication.max_name_length + 2}}"
+                f"{'State':<9}{'Instances':<12}{'Mem':<6}{'Disk':<6}Routes%EOL%")
+            # fmt: on
+            list(map(CFApplication.print_status, apps))
+            sysout("-=" * 60 + "%EOL%")
+
+    def _blue_green_check(self) -> None:
+        """Display all PCF space-application blue/green check."""
+        if len(self.apps) > 0:
+            clear_screen()
+            sysout(f"%BLUE%Checking blue/green deployments ...%EOL%")
+            CFBlueGreenChecker.check(self._org, self._space, self.apps)
+
+    def _perform_callable(self, action: str) -> None:
+        """Wrapper of the _perform method.
+        :param action the action to perform.
+        """
+        act = action.lower()
+        if self._allow_multiple(act):
+            apps = self._choose_apps(self.required_states(act))
         else:
-            app = self._select_app()
+            app = self._select_app(self.required_states(act))
             apps = [app] if app else None
         if apps:
-            for app in apps:
-                self._perform(action, app=app.name, org=self._org, space=self._space)
+            perform = partial(self._perform, action=act, org=self._org, space=self._space)
+            list(map(lambda a: perform(app=a.name), apps))
 
-    def _perform(self, action: str, **kwargs):
-        """Perform the selected PCF action"""
-        sysout(f'%GREEN%Performing {action.lower()} {str(kwargs)}...')
-        method_to_call = getattr(self._cf, action.lower())
-        sysout(method_to_call(**kwargs))
+    def _perform(self, action: str, **kwargs) -> None:
+        """Perform the selected PCF action.
+        Kwargs:
+              org (str): the PCF organization name.
+            space (str): the PCF space name.
+        :param kwargs arbitrary PCF action arguments.
+        :param action the action to perform.
+        """
+        sysout(f"%BLUE%Performing {action} {str(kwargs)}...")
+        action_method = getattr(self._cf, action)
+        check_state(callable(action_method))
+        sysout(action_method(**kwargs))
```

### Comparing `hspylib-cfman-0.9.9/cfman/exception/exceptions.py` & `hspylib-cfman-0.9.90/cfman/exception/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   TODO Purpose of the file
-   @project: HSPyLib
-   hspylib.app.cfman.exception
+   @project: HsPyLib-CFMan
+   @package: cfman.exception
       @file: exceptions.py
    @created: Tue, 11 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2021, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
 from hspylib.core.exception.exceptions import HSBaseException
 
 
 class CFConnectionError(HSBaseException):
     """Raised when failed to connect to CloudFoundry"""
@@ -23,7 +22,11 @@
 
 class CFExecutionError(HSBaseException):
     """Raised when failed to execute a cf command"""
 
 
 class CFAuthenticationError(HSBaseException):
     """Raised when failed to authenticate to CloudFoundry"""
+
+
+class CFInvalidEndpoint(HSBaseException):
+    """Raised when an invalid endpoint is provided"""
```

### Comparing `hspylib-cfman-0.9.9/hspylib_cfman.egg-info/SOURCES.txt` & `hspylib-cfman-0.9.90/hspylib_cfman.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 MANIFEST.in
 README.md
 setup.py
 cfman/.version
+cfman/__classpath__.py
 cfman/__init__.py
 cfman/__main__.py
 cfman/welcome.txt
 cfman/core/__init__.py
 cfman/core/cf.py
 cfman/core/cf_application.py
+cfman/core/cf_blue_green_checker.py
 cfman/core/cf_endpoint.py
 cfman/core/cf_manager.py
 cfman/exception/__init__.py
 cfman/exception/exceptions.py
-cfman/resources/application.properties
-cfman/resources/log/.gitkeep
-cfman/resources/log/application.log
 hspylib_cfman.egg-info/PKG-INFO
 hspylib_cfman.egg-info/SOURCES.txt
 hspylib_cfman.egg-info/dependency_links.txt
 hspylib_cfman.egg-info/requires.txt
 hspylib_cfman.egg-info/top_level.txt
```

