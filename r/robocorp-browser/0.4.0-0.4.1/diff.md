# Comparing `tmp/robocorp_browser-0.4.0.tar.gz` & `tmp/robocorp_browser-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-0.4.0.tar", max compression
+gzip compressed data, was "robocorp_browser-0.4.1.tar", max compression
```

## Comparing `robocorp_browser-0.4.0.tar` & `robocorp_browser-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       94 2023-05-10 18:39:41.395091 robocorp_browser-0.4.0/README.md
--rw-r--r--   0        0        0      640 2023-05-10 18:39:41.395091 robocorp_browser-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7225 2023-05-10 18:39:41.395091 robocorp_browser-0.4.0/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0     6959 2023-05-10 18:39:41.395091 robocorp_browser-0.4.0/src/robocorp/browser/_browser_context.py
--rw-r--r--   0        0        0        0 2023-05-10 18:39:41.395091 robocorp_browser-0.4.0/src/robocorp/browser/py.typed
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 robocorp_browser-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-05-19 08:55:34.397861 robocorp_browser-0.4.1/README.md
+-rw-r--r--   0        0        0      640 2023-05-19 08:55:34.401862 robocorp_browser-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7225 2023-05-19 08:55:34.401862 robocorp_browser-0.4.1/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0     6898 2023-05-19 08:55:34.401862 robocorp_browser-0.4.1/src/robocorp/browser/_browser_context.py
+-rw-r--r--   0        0        0        0 2023-05-19 08:55:34.401862 robocorp_browser-0.4.1/src/robocorp/browser/py.typed
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 robocorp_browser-0.4.1/PKG-INFO
```

### Comparing `robocorp_browser-0.4.0/pyproject.toml` & `robocorp_browser-0.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "0.4.0"
+version = "0.4.1"
 description = "Robocorp browser automation library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
```

### Comparing `robocorp_browser-0.4.0/src/robocorp/browser/__init__.py` & `robocorp_browser-0.4.1/src/robocorp/browser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal, Optional
 
 from playwright.sync_api import Browser, BrowserContext, Page, Playwright
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def configure(**kwargs) -> None:
     """
     May be called before any other method to configure the browser settings.
```

### Comparing `robocorp_browser-0.4.0/src/robocorp/browser/_browser_context.py` & `robocorp_browser-0.4.1/src/robocorp/browser/_browser_context.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,56 +10,59 @@
     Error,
     Page,
     Playwright,
     sync_playwright,
 )
 from robocorp.tasks import session_cache, task_cache
 
-
-def _registry_path(browser: Literal["chrome", "firefox"]) -> str:
-    if sys.platform == "win32":
-        import winreg
-
-        location = winreg.HKEY_LOCAL_MACHINE
-        browser_registry = (
-            rf"SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths\{browser}.exe"
-        )
-        key = winreg.OpenKeyEx(location, browser_registry)
-        # empty string key gets the (Default) value
-        path = winreg.QueryValueEx(key, "")
-        if isinstance(path, tuple):
-            path = path[0]
-        assert path, f"Could not find {browser} path"
-        return str(path)
-    raise RuntimeError("Not implemented for this OS")
-
-
-EXECUTABLE_PATHS: Dict[str, Dict[str, str]] = {
+EXECUTABLE_PATHS = {
     "chrome": {
         "Linux": "/usr/bin/google-chrome",
         "Darwin": "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
     },
     "firefox": {
         "Linux": "/usr/bin/firefox",
         "Windows": "C:\\Program Files\\Mozilla Firefox\\firefox.exe",
         "Darwin": "/Applications/Firefox.app/Contents/MacOS/firefox",
     },
 }
 
 
 def _get_executable_path(browser: Literal["firefox", "chrome"]) -> str:
-    if sys.platform == "win32":
+    system = platform.system()
+
+    if system == "Windows":
         return _registry_path(browser)
 
-    system = platform.system()
-    assert browser in EXECUTABLE_PATHS
-    executable_path = EXECUTABLE_PATHS[browser][system]
-    if not Path(executable_path).exists():
-        raise AssertionError()
-    return executable_path
+    if browser not in EXECUTABLE_PATHS:
+        raise ValueError(f"Unsupported browser: {browser}")
+
+    path = EXECUTABLE_PATHS[browser][system]
+    if not Path(path).exists():
+        raise RuntimeError(f"Browser executable not found: {path}")
+
+    return path
+
+
+def _registry_path(browser: Literal["chrome", "firefox"]) -> str:
+    if sys.platform != "win32":
+        raise NotImplementedError("Not implemented for non-Windows")
+
+    import winreg
+
+    parent = winreg.HKEY_LOCAL_MACHINE
+    key = rf"SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths\{browser}.exe"
+
+    handle = winreg.OpenKeyEx(parent, key)
+    path, _ = winreg.QueryValueEx(handle, "")  # Empty string is (Default) value
+
+    if not path:
+        raise RuntimeError(f"Failed to read browser path: {browser}")
+
+    return str(path)
 
 
 class _BrowserConfig:
     __slots__ = "_browser_engine _headless _slowmo _screenshot __weakref__".split()
 
     def __init__(
         self,
```

### Comparing `robocorp_browser-0.4.0/PKG-INFO` & `robocorp_browser-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-browser
-Version: 0.4.0
+Version: 0.4.1
 Summary: Robocorp browser automation library
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

