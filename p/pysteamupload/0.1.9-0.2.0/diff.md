# Comparing `tmp/pysteamupload-0.1.9.tar.gz` & `tmp/pysteamupload-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pysteamupload-0.1.9.tar", last modified: Mon Jun  6 18:25:28 2022, max compression
+gzip compressed data, was "pysteamupload-0.2.0.tar", last modified: Fri May 19 12:20:39 2023, max compression
```

## Comparing `pysteamupload-0.1.9.tar` & `pysteamupload-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-06-06 18:25:28.318669 pysteamupload-0.1.9/
--rw-rw-rw-   0        0        0    35823 2022-05-26 09:23:03.000000 pysteamupload-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     2496 2022-06-06 18:25:28.318669 pysteamupload-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1650 2022-05-26 15:20:43.000000 pysteamupload-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2022-06-06 18:25:28.304670 pysteamupload-0.1.9/pysteamupload/
--rw-rw-rw-   0        0        0     1981 2022-06-06 18:17:57.000000 pysteamupload-0.1.9/pysteamupload/__main__.py
--rw-rw-rw-   0        0        0     7194 2022-06-06 18:15:45.000000 pysteamupload-0.1.9/pysteamupload/generic_pysteamupload.py
--rw-rw-rw-   0        0        0      578 2022-06-06 15:14:48.000000 pysteamupload-0.1.9/pysteamupload/linux_pysteamupload.py
--rw-rw-rw-   0        0        0     1392 2022-06-06 14:57:28.000000 pysteamupload-0.1.9/pysteamupload/pysteamupload_templates.py
--rw-rw-rw-   0        0        0      572 2022-06-06 15:14:48.000000 pysteamupload-0.1.9/pysteamupload/windows_pysteamupload.py
-drwxrwxrwx   0        0        0        0 2022-06-06 18:25:28.317672 pysteamupload-0.1.9/pysteamupload.egg-info/
--rw-rw-rw-   0        0        0     2496 2022-06-06 18:25:27.000000 pysteamupload-0.1.9/pysteamupload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2022-06-06 18:25:28.000000 pysteamupload-0.1.9/pysteamupload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-06 18:25:27.000000 pysteamupload-0.1.9/pysteamupload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2022-06-06 18:25:28.000000 pysteamupload-0.1.9/pysteamupload.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-06-06 18:25:28.000000 pysteamupload-0.1.9/pysteamupload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-06 18:25:28.318669 pysteamupload-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1189 2022-06-06 18:23:46.000000 pysteamupload-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:20:39.639826 pysteamupload-0.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-17 17:29:14.000000 pysteamupload-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1474 2023-05-19 12:20:39.639826 pysteamupload-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      651 2023-05-19 12:04:26.000000 pysteamupload-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 12:20:39.628317 pysteamupload-0.2.0/pysteamupload/
+-rw-rw-rw-   0        0        0     2297 2023-05-19 11:47:07.000000 pysteamupload-0.2.0/pysteamupload/__main__.py
+-rw-rw-rw-   0        0        0     7590 2023-05-19 11:55:07.000000 pysteamupload-0.2.0/pysteamupload/generic_pysteamupload.py
+-rw-rw-rw-   0        0        0     1385 2023-05-19 12:19:06.000000 pysteamupload-0.2.0/pysteamupload/linux_pysteamupload.py
+-rw-rw-rw-   0        0        0     1392 2023-05-17 17:29:14.000000 pysteamupload-0.2.0/pysteamupload/pysteamupload_templates.py
+-rw-rw-rw-   0        0        0      572 2023-05-17 17:29:14.000000 pysteamupload-0.2.0/pysteamupload/windows_pysteamupload.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:20:39.638826 pysteamupload-0.2.0/pysteamupload.egg-info/
+-rw-rw-rw-   0        0        0     1474 2023-05-19 12:20:39.000000 pysteamupload-0.2.0/pysteamupload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-05-19 12:20:39.000000 pysteamupload-0.2.0/pysteamupload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 12:20:39.000000 pysteamupload-0.2.0/pysteamupload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-19 12:20:39.000000 pysteamupload-0.2.0/pysteamupload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-19 12:20:39.000000 pysteamupload-0.2.0/pysteamupload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 12:20:39.639826 pysteamupload-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1189 2023-05-19 12:05:49.000000 pysteamupload-0.2.0/setup.py
```

### Comparing `pysteamupload-0.1.9/LICENSE` & `pysteamupload-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysteamupload-0.1.9/pysteamupload/generic_pysteamupload.py` & `pysteamupload-0.2.0/pysteamupload/generic_pysteamupload.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def __init__(self):
         self.root_directory: Path = Path(tempfile.gettempdir(), "SteamCMD")
         if not self.is_steamcmd_available():
             logger.info("SteamCMD seems not installed, downloading it.")
             self.download_steamcmd()
             self.extract_steamcmd()
-        self.setup_steam_guard()
+        # self.setup_steam_guard()
 
     def get_archive_path(self) -> Path:
         # Windows example: C:\Users\rdall\AppData\Local\Temp\SteamCMD\steamcmd.zip
         return Path(self.root_directory, self.get_steamcmd_remote_filename())
 
     def get_steamcmd_path(self) -> Path:
         # Windows example: C:\Users\rdall\AppData\Local\Temp\SteamCMD\steamcmd.exe
@@ -51,27 +51,33 @@
 
     def extract_steamcmd(self) -> None:
         self.extract_steamcmd_archive()
         os.remove(self.get_archive_path())
         logger.info("Extraction is complete.")
 
     def setup_steam_guard(self) -> None:
+        """
+        DEPRECATED
+        """
         if not self.get_config_vdf_path().exists():
             self._create_config_vdf()
         if not self.get_ssfn_path().exists():
             self._create_ssfn()
 
     @staticmethod
     def get_config_vdf_filename() -> str:
         return "config.vdf"
 
     def get_config_vdf_path(self) -> Path:
         return self.root_directory / "config" / self.get_config_vdf_filename()
 
     def _create_config_vdf(self) -> None:
+        """
+        DEPRECATED
+        """
         config_dir = Path(self.root_directory, "config")
         config_dir.mkdir(exist_ok=True)
         self._create_file_from_base64(
             environ_key="STEAM_CONFIG_VDF_FILE_CONTENT",
             destination=self.get_config_vdf_path(),
             binary_file=False,
         )
@@ -81,14 +87,17 @@
     def get_ssfn_filename() -> str:
         return os.getenv("STEAM_SSFN_FILENAME")
 
     def get_ssfn_path(self) -> Path:
         return self.root_directory / self.get_ssfn_filename()
 
     def _create_ssfn(self) -> None:
+        """
+        DEPRECATED
+        """
         self._create_file_from_base64(
             environ_key="STEAM_SSFN_FILE_CONTENT",
             destination=self.get_ssfn_path(),
             binary_file=True,
         )
         logger.info("ssfn file created")
 
@@ -106,15 +115,15 @@
     def call_steamcmd(self, args) -> int:
         timeout_in_seconds = 30
         try:
             subprocess_args = (self.get_steamcmd_path(), *args, "+quit")
             subprocess.check_call(subprocess_args, timeout=timeout_in_seconds)
             return 0
         except subprocess.TimeoutExpired:
-            # SteamGuard is probably waiting asking for a 2 factor authentication password
+            # SteamGuard is probably waiting asking for a 2-factor authentication password
             logger.error(f"SteamCMD timed out ({timeout_in_seconds} seconds)")
         except subprocess.CalledProcessError as exception:
             if exception.returncode != 7:
                 logger.error(exception)
             return exception.returncode
         return 1
 
@@ -160,14 +169,19 @@
         app_build["appbuild"]["depots"][depot_id] = "depot.vdf"
 
         # Dump output
         filename = self.get_app_build_path()
         with open(filename, "w") as f:
             vdf.dump(app_build, f, pretty=True)
 
+    def initialize_only(self) -> int:
+        logger.info(f"Initialize SteamCMD with your password/SteamGuard.")
+        logger.info(f"Execute to initialize your steamcmd : {self.get_steamcmd_path()} +login username password +quit")
+        return 0
+
     def upload(
             self,
             app_id: str,
             depot_id: str,
             build_description: str,
             content_path: Path,
     ) -> int:
```

### Comparing `pysteamupload-0.1.9/pysteamupload/linux_pysteamupload.py` & `pysteamupload-0.2.0/pysteamupload/windows_pysteamupload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import tarfile
+import zipfile
 from abc import abstractmethod
 from pysteamupload.generic_pysteamupload import GenericPySteamUpload
 
 
-class LinuxPySteamUpload(GenericPySteamUpload):
+class WindowsPySteamUpload(GenericPySteamUpload):
     @abstractmethod
     def get_steamcmd_local_filename(self) -> str:
-        return "steamcmd.sh"
+        return "steamcmd.exe"
 
     @abstractmethod
     def get_steamcmd_remote_filename(self) -> str:
-        return "steamcmd_linux.tar.gz"
+        return "steamcmd.zip"
 
     @abstractmethod
     def extract_steamcmd_archive(self) -> None:
-        with tarfile.open(self.get_archive_path(), 'r:gz') as f:
+        with zipfile.ZipFile(self.get_archive_path(), "r") as f:
             f.extractall(path=self.root_directory)
```

### Comparing `pysteamupload-0.1.9/pysteamupload/pysteamupload_templates.py` & `pysteamupload-0.2.0/pysteamupload/pysteamupload_templates.py`

 * *Files identical despite different names*

### Comparing `pysteamupload-0.1.9/setup.py` & `pysteamupload-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     author="Richard Dally",
     name="pysteamupload",
-    version="0.1.9",
+    version="0.2.0",
     description="SteamCMD leveraged by CPython to upload binaries",
     url="https://github.com/RichardDally/PySteamUpload",
     license="GNU Lesser General Public License v3.0",
     install_requires=requirements,
     packages=["pysteamupload"],
     author_email="r.dally@proton.me",
     long_description=long_description,
```

