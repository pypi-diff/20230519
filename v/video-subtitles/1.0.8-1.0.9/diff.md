# Comparing `tmp/video-subtitles-1.0.8.tar.gz` & `tmp/video-subtitles-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video-subtitles-1.0.8.tar", last modified: Wed May 10 08:03:07 2023, max compression
+gzip compressed data, was "video-subtitles-1.0.9.tar", last modified: Wed May 10 08:19:50 2023, max compression
```

## Comparing `video-subtitles-1.0.8.tar` & `video-subtitles-1.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:03:07.501073 video-subtitles-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-10 08:03:07.448074 video-subtitles-1.0.8/.github/
-drwxrwxrwx   0        0        0        0 2023-05-10 08:03:07.468074 video-subtitles-1.0.8/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.8/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.8/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.8/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.8/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     2094 2023-05-10 02:09:59.000000 video-subtitles-1.0.8/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-10 08:03:07.471074 video-subtitles-1.0.8/.vscode/
--rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.8/.vscode/launch.json
--rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.8/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.8/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5613 2023-05-10 08:03:07.500074 video-subtitles-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4802 2023-05-10 08:02:19.000000 video-subtitles-1.0.8/README.md
--rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.8/activate.sh
--rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.8/lint.sh
--rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.8/make_venv.py
--rw-rw-rw-   0        0        0      852 2023-05-10 07:58:22.000000 video-subtitles-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       59 2023-05-09 01:29:01.000000 video-subtitles-1.0.8/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 08:03:07.501073 video-subtitles-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:03:07.450073 video-subtitles-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 08:03:07.481072 video-subtitles-1.0.8/src/video_subtitles/
--rw-rw-rw-   0        0        0       34 2023-05-10 08:02:29.000000 video-subtitles-1.0.8/src/video_subtitles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:03:07.493073 video-subtitles-1.0.8/src/video_subtitles/assets/
--rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.8/src/video_subtitles/assets/example.txt
--rw-rw-rw-   0        0        0     3728 2023-05-10 05:42:46.000000 video-subtitles-1.0.8/src/video_subtitles/cli.py
--rw-rw-rw-   0        0        0      332 2023-05-10 03:44:22.000000 video-subtitles-1.0.8/src/video_subtitles/convert_to_webvtt.py
--rw-rw-rw-   0        0        0    10587 2023-05-10 07:36:41.000000 video-subtitles-1.0.8/src/video_subtitles/gui.py
--rw-rw-rw-   0        0        0     3764 2023-05-10 06:41:10.000000 video-subtitles-1.0.8/src/video_subtitles/run.py
--rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.8/src/video_subtitles/say.py
--rw-rw-rw-   0        0        0     2314 2023-05-10 08:01:19.000000 video-subtitles-1.0.8/src/video_subtitles/settings.py
--rw-rw-rw-   0        0        0     1622 2023-05-10 06:00:11.000000 video-subtitles-1.0.8/src/video_subtitles/thread_processor.py
--rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.8/src/video_subtitles/translate.py
--rw-rw-rw-   0        0        0     3855 2023-05-10 04:55:21.000000 video-subtitles-1.0.8/src/video_subtitles/util.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:03:07.491072 video-subtitles-1.0.8/src/video_subtitles.egg-info/
--rw-rw-rw-   0        0        0     5613 2023-05-10 08:03:07.000000 video-subtitles-1.0.8/src/video_subtitles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1072 2023-05-10 08:03:07.000000 video-subtitles-1.0.8/src/video_subtitles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:03:07.000000 video-subtitles-1.0.8/src/video_subtitles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-10 08:03:07.000000 video-subtitles-1.0.8/src/video_subtitles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-05-10 08:03:07.000000 video-subtitles-1.0.8/src/video_subtitles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-10 08:03:07.000000 video-subtitles-1.0.8/src/video_subtitles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 08:03:07.499072 video-subtitles-1.0.8/tests/
--rw-rw-rw-   0        0        0     2704 2023-05-10 03:34:47.000000 video-subtitles-1.0.8/tests/test.srt
--rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.8/tests/test_cli.py
--rw-rw-rw-   0        0        0      988 2023-05-10 03:40:25.000000 video-subtitles-1.0.8/tests/test_full.py
--rw-rw-rw-   0        0        0      656 2023-05-10 03:46:07.000000 video-subtitles-1.0.8/tests/test_srt_to_webvtt.py
--rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.8/tests/test_srt_translator.py
--rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.8/tests/video.mp4
--rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.8/tox.ini
--rw-rw-rw-   0        0        0      953 2023-05-10 01:01:08.000000 video-subtitles-1.0.8/upload_package.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:19:50.254756 video-subtitles-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-05-10 08:19:50.195757 video-subtitles-1.0.9/.github/
+drwxrwxrwx   0        0        0        0 2023-05-10 08:19:50.212758 video-subtitles-1.0.9/.github/workflows/
+-rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.9/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.9/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.9/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.9/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     2094 2023-05-10 02:09:59.000000 video-subtitles-1.0.9/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-10 08:19:50.214758 video-subtitles-1.0.9/.vscode/
+-rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.9/.vscode/launch.json
+-rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.9/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.9/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5675 2023-05-10 08:19:50.253759 video-subtitles-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4863 2023-05-10 08:17:57.000000 video-subtitles-1.0.9/README.md
+-rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.9/activate.sh
+-rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.9/lint.sh
+-rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.9/make_venv.py
+-rw-rw-rw-   0        0        0      852 2023-05-10 07:58:22.000000 video-subtitles-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       59 2023-05-09 01:29:01.000000 video-subtitles-1.0.9/requirements.testing.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:19:50.254756 video-subtitles-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:19:50.196756 video-subtitles-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 08:19:50.223757 video-subtitles-1.0.9/src/video_subtitles/
+-rw-rw-rw-   0        0        0       34 2023-05-10 08:17:37.000000 video-subtitles-1.0.9/src/video_subtitles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:19:50.246760 video-subtitles-1.0.9/src/video_subtitles/assets/
+-rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.9/src/video_subtitles/assets/example.txt
+-rw-rw-rw-   0        0        0     3728 2023-05-10 05:42:46.000000 video-subtitles-1.0.9/src/video_subtitles/cli.py
+-rw-rw-rw-   0        0        0      332 2023-05-10 03:44:22.000000 video-subtitles-1.0.9/src/video_subtitles/convert_to_webvtt.py
+-rw-rw-rw-   0        0        0    10587 2023-05-10 07:36:41.000000 video-subtitles-1.0.9/src/video_subtitles/gui.py
+-rw-rw-rw-   0        0        0     3764 2023-05-10 06:41:10.000000 video-subtitles-1.0.9/src/video_subtitles/run.py
+-rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.9/src/video_subtitles/say.py
+-rw-rw-rw-   0        0        0     2355 2023-05-10 08:17:11.000000 video-subtitles-1.0.9/src/video_subtitles/settings.py
+-rw-rw-rw-   0        0        0     1622 2023-05-10 06:00:11.000000 video-subtitles-1.0.9/src/video_subtitles/thread_processor.py
+-rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.9/src/video_subtitles/translate.py
+-rw-rw-rw-   0        0        0     3855 2023-05-10 04:55:21.000000 video-subtitles-1.0.9/src/video_subtitles/util.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:19:50.245759 video-subtitles-1.0.9/src/video_subtitles.egg-info/
+-rw-rw-rw-   0        0        0     5675 2023-05-10 08:19:50.000000 video-subtitles-1.0.9/src/video_subtitles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1072 2023-05-10 08:19:50.000000 video-subtitles-1.0.9/src/video_subtitles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:19:50.000000 video-subtitles-1.0.9/src/video_subtitles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-10 08:19:50.000000 video-subtitles-1.0.9/src/video_subtitles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-05-10 08:19:50.000000 video-subtitles-1.0.9/src/video_subtitles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-10 08:19:50.000000 video-subtitles-1.0.9/src/video_subtitles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 08:19:50.252758 video-subtitles-1.0.9/tests/
+-rw-rw-rw-   0        0        0     2704 2023-05-10 03:34:47.000000 video-subtitles-1.0.9/tests/test.srt
+-rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.9/tests/test_cli.py
+-rw-rw-rw-   0        0        0      988 2023-05-10 03:40:25.000000 video-subtitles-1.0.9/tests/test_full.py
+-rw-rw-rw-   0        0        0      656 2023-05-10 03:46:07.000000 video-subtitles-1.0.9/tests/test_srt_to_webvtt.py
+-rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.9/tests/test_srt_translator.py
+-rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.9/tests/video.mp4
+-rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.9/tox.ini
+-rw-rw-rw-   0        0        0      892 2023-05-10 08:19:44.000000 video-subtitles-1.0.9/upload_package.py
```

### Comparing `video-subtitles-1.0.8/.github/workflows/lint.yml` & `video-subtitles-1.0.9/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/.github/workflows/push_macos.yml` & `video-subtitles-1.0.9/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/.github/workflows/push_ubuntu.yml` & `video-subtitles-1.0.9/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/.github/workflows/push_win.yml` & `video-subtitles-1.0.9/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/.gitignore` & `video-subtitles-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/.vscode/launch.json` & `video-subtitles-1.0.9/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/.vscode/settings.json` & `video-subtitles-1.0.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/.vscode/tasks.json` & `video-subtitles-1.0.9/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/LICENSE` & `video-subtitles-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/PKG-INFO` & `video-subtitles-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-subtitles
-Version: 1.0.8
+Version: 1.0.9
 Summary: Creates Video Subtitles
 Home-page: https://github.com/zackees/video-subtitles
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -131,14 +131,15 @@
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `ruff`, `pylint`, `flake8` and `mypy`.
 
 # Releases
 
+  * 1.0.9: Fix settings.json bug in not created directories.
   * 1.0.8: Adds password field and centralizes settings.json under appdirs.
   * 1.0.7: Adds progress bar when doing work.
   * 1.0.6: Adds gui language help for language codes.
   * 1.0.5: Adds webvtt format option.
   * 1.0.4: Adds thread processor so that multiple files can be done one at a time.
   * 1.0.3: Adds gui.
   * 1.0.2: Fix bug.
```

### Comparing `video-subtitles-1.0.8/README.md` & `video-subtitles-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `ruff`, `pylint`, `flake8` and `mypy`.
 
 # Releases
 
+  * 1.0.9: Fix settings.json bug in not created directories.
   * 1.0.8: Adds password field and centralizes settings.json under appdirs.
   * 1.0.7: Adds progress bar when doing work.
   * 1.0.6: Adds gui language help for language codes.
   * 1.0.5: Adds webvtt format option.
   * 1.0.4: Adds thread processor so that multiple files can be done one at a time.
   * 1.0.3: Adds gui.
   * 1.0.2: Fix bug.
```

### Comparing `video-subtitles-1.0.8/make_venv.py` & `video-subtitles-1.0.9/make_venv.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/pyproject.toml` & `video-subtitles-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/setup.py` & `video-subtitles-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/src/video_subtitles/cli.py` & `video-subtitles-1.0.9/src/video_subtitles/cli.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/src/video_subtitles/gui.py` & `video-subtitles-1.0.9/src/video_subtitles/gui.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/src/video_subtitles/run.py` & `video-subtitles-1.0.9/src/video_subtitles/run.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/src/video_subtitles/say.py` & `video-subtitles-1.0.9/src/video_subtitles/say.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/src/video_subtitles/settings.py` & `video-subtitles-1.0.9/src/video_subtitles/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_settings_path() -> str:
     """Get settings path"""
     env_path = user_config_dir("video-subtitles", "video-subtitles", roaming=True)
     config_file = os.path.join(env_path, "settings.json")
+    os.makedirs(env_path, exist_ok=True)
     return config_file
 
 
 SETTINGS_JSON = get_settings_path()
 
 
 class Settings:
```

### Comparing `video-subtitles-1.0.8/src/video_subtitles/thread_processor.py` & `video-subtitles-1.0.9/src/video_subtitles/thread_processor.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/src/video_subtitles/translate.py` & `video-subtitles-1.0.9/src/video_subtitles/translate.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/src/video_subtitles/util.py` & `video-subtitles-1.0.9/src/video_subtitles/util.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/src/video_subtitles.egg-info/PKG-INFO` & `video-subtitles-1.0.9/src/video_subtitles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-subtitles
-Version: 1.0.8
+Version: 1.0.9
 Summary: Creates Video Subtitles
 Home-page: https://github.com/zackees/video-subtitles
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -131,14 +131,15 @@
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `ruff`, `pylint`, `flake8` and `mypy`.
 
 # Releases
 
+  * 1.0.9: Fix settings.json bug in not created directories.
   * 1.0.8: Adds password field and centralizes settings.json under appdirs.
   * 1.0.7: Adds progress bar when doing work.
   * 1.0.6: Adds gui language help for language codes.
   * 1.0.5: Adds webvtt format option.
   * 1.0.4: Adds thread processor so that multiple files can be done one at a time.
   * 1.0.3: Adds gui.
   * 1.0.2: Fix bug.
```

### Comparing `video-subtitles-1.0.8/src/video_subtitles.egg-info/SOURCES.txt` & `video-subtitles-1.0.9/src/video_subtitles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/tests/test.srt` & `video-subtitles-1.0.9/tests/test.srt`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/tests/test_cli.py` & `video-subtitles-1.0.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/tests/test_full.py` & `video-subtitles-1.0.9/tests/test_full.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/tests/test_srt_to_webvtt.py` & `video-subtitles-1.0.9/tests/test_srt_to_webvtt.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/tests/test_srt_translator.py` & `video-subtitles-1.0.9/tests/test_srt_translator.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/tests/video.mp4` & `video-subtitles-1.0.9/tests/video.mp4`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.8/upload_package.py` & `video-subtitles-1.0.9/upload_package.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 
 import os
 import subprocess
 import shutil
 import sys
 
 PYTHON_EXE = sys.executable
-PIP_EXE = os.path.join(os.path.dirname(PYTHON_EXE), "pip")
 
 # Equivalent to 'rm -rf build dist'
 if os.path.exists('build'):
     shutil.rmtree('build', ignore_errors=True)
 if os.path.exists('dist'):
     shutil.rmtree('dist', ignore_errors=True)
 
 # Equivalent to 'pip install wheel twine'
-subprocess.check_call([PIP_EXE, 'install', 'wheel', 'twine'])
+subprocess.check_call(["pip", 'install', 'wheel', 'twine'])
 
 print("Building Source and Wheel (universal) distribution…")
 # Equivalent to 'python setup.py sdist bdist_wheel --universal'
 subprocess.check_call([PYTHON_EXE, 'setup.py', 'sdist', 'bdist_wheel', '--universal'])
 
 print("Uploading the package to PyPI via Twine…")
 # Equivalent to 'twine upload dist/* --verbose'
```

