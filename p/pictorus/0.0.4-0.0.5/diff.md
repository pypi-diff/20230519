# Comparing `tmp/pictorus-0.0.4.tar.gz` & `tmp/pictorus-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pictorus-0.0.4.tar", last modified: Wed May 17 21:57:10 2023, max compression
+gzip compressed data, was "pictorus-0.0.5.tar", last modified: Fri May 19 20:39:24 2023, max compression
```

## Comparing `pictorus-0.0.4.tar` & `pictorus-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      554 2023-04-18 22:31:36.961706 pictorus-0.0.4/.github/workflows/test.yaml
--rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.0.4/.gitignore
--rw-r--r--   0        0        0        6 2023-02-15 19:48:07.053003 pictorus-0.0.4/.python-version
--rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.0.4/LICENSE
--rw-r--r--   0        0        0      737 2023-02-16 17:48:01.977637 pictorus-0.0.4/PUB_README.md
--rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.0.4/README.md
--rw-r--r--   0        0        0      811 2023-05-17 20:36:24.054992 pictorus-0.0.4/pyproject.toml
--rwxr-xr-x   0        0        0      340 2023-02-15 19:48:07.054532 pictorus-0.0.4/script/setup
--rw-r--r--   0        0        0       61 2023-05-09 19:07:56.160045 pictorus-0.0.4/src/pictorus/__init__.py
--rw-r--r--   0        0        0    13817 2023-05-17 21:46:40.388463 pictorus-0.0.4/src/pictorus/app_manager.py
--rw-r--r--   0        0        0     2886 2023-05-17 21:46:40.388659 pictorus-0.0.4/src/pictorus/config.py
--rw-r--r--   0        0        0      492 2023-05-09 19:07:56.162364 pictorus-0.0.4/src/pictorus/constants.py
--rw-r--r--   0        0        0      244 2023-02-15 19:48:07.055277 pictorus-0.0.4/src/pictorus/logging.py
--rw-r--r--   0        0        0     3450 2023-05-17 21:46:40.388844 pictorus-0.0.4/src/pictorus/pictorus_cli.py
--rwxr-xr-x   0        0        0     2146 2023-05-17 21:46:40.389061 pictorus-0.0.4/src/pictorus/pictorus_device_manager.py
--rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.0.4/src/pictorus/systemd.py
--rw-r--r--   0        0        0     4878 2023-05-09 19:07:56.163315 pictorus-0.0.4/src/pictorus/telemetry_manager.py
--rw-r--r--   0        0        0     9002 2023-05-09 19:07:56.163796 pictorus-0.0.4/tests/pictorus/test_app_manager.py
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 pictorus-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      554 2023-04-18 22:31:36.961706 pictorus-0.0.5/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.0.5/.gitignore
+-rw-r--r--   0        0        0        6 2023-02-15 19:48:07.053003 pictorus-0.0.5/.python-version
+-rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.0.5/LICENSE
+-rw-r--r--   0        0        0      737 2023-02-16 17:48:01.977637 pictorus-0.0.5/PUB_README.md
+-rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.0.5/README.md
+-rw-r--r--   0        0        0      828 2023-05-19 20:34:53.614814 pictorus-0.0.5/pyproject.toml
+-rwxr-xr-x   0        0        0      340 2023-02-15 19:48:07.054532 pictorus-0.0.5/script/setup
+-rw-r--r--   0        0        0       61 2023-05-19 20:35:22.132381 pictorus-0.0.5/src/pictorus/__init__.py
+-rw-r--r--   0        0        0    14247 2023-05-19 20:28:20.661444 pictorus-0.0.5/src/pictorus/app_manager.py
+-rw-r--r--   0        0        0     3153 2023-05-19 20:28:20.661876 pictorus-0.0.5/src/pictorus/config.py
+-rw-r--r--   0        0        0      492 2023-05-09 19:07:56.162364 pictorus-0.0.5/src/pictorus/constants.py
+-rw-r--r--   0        0        0      244 2023-02-15 19:48:07.055277 pictorus-0.0.5/src/pictorus/logging.py
+-rw-r--r--   0        0        0     4054 2023-05-19 20:28:20.662559 pictorus-0.0.5/src/pictorus/pictorus_cli.py
+-rwxr-xr-x   0        0        0     2390 2023-05-19 20:28:20.663228 pictorus-0.0.5/src/pictorus/pictorus_device_manager.py
+-rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.0.5/src/pictorus/systemd.py
+-rw-r--r--   0        0        0     4878 2023-05-09 19:07:56.163315 pictorus-0.0.5/src/pictorus/telemetry_manager.py
+-rw-r--r--   0        0        0     3316 2023-05-19 20:34:53.615084 pictorus-0.0.5/src/pictorus/version_manager.py
+-rw-r--r--   0        0        0     9002 2023-05-09 19:07:56.163796 pictorus-0.0.5/tests/pictorus/test_app_manager.py
+-rw-r--r--   0        0        0     2389 2023-05-19 20:34:53.615288 pictorus-0.0.5/tests/pictorus/test_version_manager.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 pictorus-0.0.5/PKG-INFO
```

### Comparing `pictorus-0.0.4/.github/workflows/test.yaml` & `pictorus-0.0.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.4/.gitignore` & `pictorus-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.4/LICENSE` & `pictorus-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.4/PUB_README.md` & `pictorus-0.0.5/PUB_README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.4/README.md` & `pictorus-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.4/pyproject.toml` & `pictorus-0.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "pictorus"
 authors = [{ name = "Pictorus Inc", email = "contact@pictor.us" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
 dynamic = ["version", "description"]
-dependencies = ["awsiotsdk~=1.11.5", "requests~=2.26.0"]
+dependencies = ["awsiotsdk~=1.11.5", "requests~=2.26.0", "semver~=3.0.0"]
 requires-python = ">=3.7"
 readme = "PUB_README.md"
 
 [project.scripts]
 pictorus-cli = "pictorus.pictorus_cli:main"
 pictorus-device-manager = "pictorus.pictorus_device_manager:main"
```

### Comparing `pictorus-0.0.4/src/pictorus/app_manager.py` & `pictorus-0.0.5/src/pictorus/app_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from concurrent.futures import ThreadPoolExecutor
 
 
 import requests
 from awscrt import mqtt
 from awsiot import iotshadow
 
+from . import __version__ as CURRENT_VERSION
+from .version_manager import VersionManager
 from .config import load_app_manifest, store_app_manifest, APP_ASSETS_DIR, Config
 from .telemetry_manager import TelemetryManager, MCAST_ADDR
 from .logging import get_logger
 from .constants import CmdType, AppLogLevel, PICTORUS_SERVICE_NAME
 
 logger = get_logger()
 config = Config()
@@ -59,27 +61,36 @@
         "err_type": "NoLogError",
         "message": "App crashed unexpectedly",
     }
 
     def __init__(self, mqtt_connection: mqtt.Connection):
         self._telemetry_manager = TelemetryManager(mqtt_connection)
         self._pictorus_app_process: Popen = None
+        self._version_manager: VersionManager = None
         self._error_log = self.EMPTY_ERROR.copy()
         self._app_manifest = load_app_manifest()
         self._mqtt_connection = mqtt_connection
         self._shadow_client = iotshadow.IotShadowClient(self._mqtt_connection)
         self._last_reported_shadow_state = None
         self._app_log_level = AppLogLevel.INFO
 
         self._update_reported_shadow_state()
 
         self.complete = threading.Event()
         self._app_watcher_thread = threading.Thread(target=self._watch_app)
         self._app_watcher_thread.start()
 
+    def set_version_mgr(self, version_mgr: VersionManager):
+        self._version_manager = version_mgr
+
+    @property
+    def app_is_running(self) -> bool:
+        """Return whether the app is currently running"""
+        return bool(self._pictorus_app_process)
+
     def _watch_app(self):
         while not self.complete.is_set():
             # If an app process has started, communicate() to catch unexpected terminations.
             if self._pictorus_app_process:
                 logger.info("AppManager watching for Pictorus App crashes...")
 
                 # Reset Error shadow state for each new app run
@@ -132,20 +143,23 @@
         self._mqtt_connection.unsubscribe(cmd_topic(self.CMD_REQUEST_SUBTOPIC))
         self._mqtt_connection.unsubscribe(cmd_topic(self.RETAINED_CMD_SUBTOPIC))
 
         if self._app_watcher_thread:
             self._app_watcher_thread.join()
 
     def _update_reported_shadow_state(self):
+        cached_version = self._version_manager.last_installed if self._version_manager else None
         shadow_state = {
             "connected": True,
             self.APP_VERSION_SHADOW_PROP: self._app_manifest,
             self.RUN_APP_SHADOW_PROP: config.run_app,
             self.ERROR_LOG_SHADOW_PROP: self._error_log,
             self.LOG_LEVEL_SHADOW_PROP: self._app_log_level.value,
+            "version": CURRENT_VERSION,
+            "cached_version": cached_version,
         }
 
         # Don't publish an update if nothing changed. Otherwise we can get in a bad state
         # where IoT backend continuously publishes deltas and we respond with the same reported state
         if self._last_reported_shadow_state == shadow_state:
             return
 
@@ -358,12 +372,7 @@
 
             if run_app:
                 self._maybe_start_app()
             else:
                 self._stop_app()
 
         self._update_reported_shadow_state()
-
-    @property
-    def app_is_running(self) -> bool:
-        """Return whether the app is currently running"""
-        return bool(self._pictorus_app_process)
```

### Comparing `pictorus-0.0.4/src/pictorus/config.py` & `pictorus-0.0.5/src/pictorus/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 APP_MANIFEST_PATH = os.path.join(DEVICE_MGR_DIR, "app_manifest.json")
 
 
 class Config:
     """Device manager configuration"""
 
     RUN_APP_KEY = "runApp"
+    AUTO_UPDATE_KEY = "autoUpdate"
 
     _instance = None
 
     def __init__(self):
         self._config = self._load_config()
 
     def __new__(cls):
@@ -64,14 +65,22 @@
     def run_app(self) -> bool:
         return self._config.get(self.RUN_APP_KEY, False)
 
     @run_app.setter
     def run_app(self, value: bool):
         self._update_config(self.RUN_APP_KEY, value)
 
+    @property
+    def auto_update(self) -> bool:
+        return self._config.get(self.AUTO_UPDATE_KEY, True)
+
+    @auto_update.setter
+    def auto_update(self, value: bool):
+        self._update_config(self.AUTO_UPDATE_KEY, value)
+
     @staticmethod
     def _load_config():
         """Load the config file"""
         if not os.path.exists(CONFIG_PATH):
             return {}
 
         with open(CONFIG_PATH, "r", encoding="utf-8") as f:
```

### Comparing `pictorus-0.0.4/src/pictorus/pictorus_cli.py` & `pictorus-0.0.5/src/pictorus/pictorus_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,18 +35,35 @@
 def get_credentials():
     """Prompt user for username and password"""
     username = input("Enter username for pictorus: ")
     passwd = getpass("Enter password for pictorus: ")
     return username, passwd
 
 
+def prompt_auto_update() -> bool:
+    """Prompt the user to ask if they want to update automatically"""
+    auto_update = input("Would you like to update pictorus automatically on this device [Y/n]? ")
+    if auto_update.lower() in ("y", "yes", ""):
+        printf("Automatic updates enabled", TextFormat.OKGREEN)
+        return True
+
+    printf("Automatic updates disabled", TextFormat.WARNING)
+    return False
+
+
+def configure_additional_settings():
+    """Configure any additional settings that require user input"""
+    config.auto_update = prompt_auto_update()
+
+
 def configure():
     """Configure the device manager"""
     configure_device()
     setup_device_manager()
+    configure_additional_settings()
 
 
 def setup_device_manager():
     """Setup and start the device manager service"""
     print("Setting up device manager service")
     bin_path = shutil.which("pictorus-device-manager")
     if not bin_path:
```

### Comparing `pictorus-0.0.4/src/pictorus/pictorus_device_manager.py` & `pictorus-0.0.5/src/pictorus/pictorus_device_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python3
 
 """ Daemon process for handling IoT interactions """
 import json
 import sys
 import time
+import os
 
 from awsiot import mqtt_connection_builder
 from awscrt import mqtt
 from awscrt.exceptions import AwsCrtError
 
 from pictorus.config import Config
 from pictorus.logging import get_logger
 from pictorus.app_manager import AppManager
+from pictorus.version_manager import VersionManager
 
 logger = get_logger()
 config = Config()
 
 CONNECT_RETRY_TIMEOUT_S = 15
 
 
@@ -41,19 +43,22 @@
     )
 
     return mqtt_connection
 
 
 def main():
     """Main run function"""
-    logger.info(f"Starting device manager for device: {config.client_id}")
+    log_level = os.environ.get(key="LOG_LEVEL", default="INFO").upper()
+    logger.setLevel(log_level)
+    logger.info("Starting device manager for device: %s", config.client_id)
     mqtt_connection = create_mqtt_connection()
     connect_future = mqtt_connection.connect()
 
-    with AppManager(mqtt_connection) as app_mgr:
+    with AppManager(mqtt_connection) as app_mgr, VersionManager() as version_mgr:
+        app_mgr.set_version_mgr(version_mgr)
         while True:
             try:
                 connect_future.result()
                 break
             except AwsCrtError:
                 logger.warning(
                     "Connection failed. Retrying in: %ss", CONNECT_RETRY_TIMEOUT_S, exc_info=True
```

### Comparing `pictorus-0.0.4/src/pictorus/systemd.py` & `pictorus-0.0.5/src/pictorus/systemd.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.4/src/pictorus/telemetry_manager.py` & `pictorus-0.0.5/src/pictorus/telemetry_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.4/tests/pictorus/test_app_manager.py` & `pictorus-0.0.5/tests/pictorus/test_app_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.4/PKG-INFO` & `pictorus-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pictorus
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pictorus device manager package
 Author-email: Pictorus Inc <contact@pictor.us>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: awsiotsdk~=1.11.5
 Requires-Dist: requests~=2.26.0
+Requires-Dist: semver~=3.0.0
 Requires-Dist: black==22.3.0 ; extra == "dev"
 Requires-Dist: responses==0.22.0 ; extra == "test"
 Requires-Dist: pytest==7.2.1 ; extra == "test"
 Project-URL: Home, https://pictor.us
 Provides-Extra: dev
 Provides-Extra: test
```

