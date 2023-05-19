# Comparing `tmp/onboardme-1.0.1.tar.gz` & `tmp/onboardme-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.0.1.tar", max compression
+gzip compressed data, was "onboardme-1.0.2.tar", max compression
```

## Comparing `onboardme-1.0.1.tar` & `onboardme-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0    11868 2023-05-12 16:18:28.185568 onboardme-1.0.1/README.md
--rwxr-xr-x   0        0        0     6667 2023-03-18 21:01:43.622076 onboardme-1.0.1/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.0.1/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.0.1/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     2671 2022-11-18 16:13:55.305455 onboardme-1.0.1/onboardme/console_logging.py
--rw-r--r--   0        0        0     1544 2023-03-18 21:01:43.623119 onboardme-1.0.1/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.0.1/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.0.1/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.0.1/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5706 2023-05-12 16:18:28.187688 onboardme-1.0.1/onboardme/help_text.py
--rw-r--r--   0        0        0     3123 2023-03-18 21:01:43.626062 onboardme-1.0.1/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.0.1/onboardme/misc.py
--rwxr-xr-x   0        0        0     8607 2023-05-12 16:18:28.188160 onboardme-1.0.1/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.0.1/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.0.1/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.0.1/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.0.1/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1913 2023-05-12 16:18:28.189143 onboardme-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    13249 1970-01-01 00:00:00.000000 onboardme-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0    11868 2023-05-12 16:18:28.185568 onboardme-1.0.2/README.md
+-rwxr-xr-x   0        0        0     6667 2023-03-18 21:01:43.622076 onboardme-1.0.2/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.0.2/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.0.2/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     2671 2022-11-18 16:13:55.305455 onboardme-1.0.2/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1691 2023-05-19 11:53:30.594074 onboardme-1.0.2/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.0.2/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.0.2/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.0.2/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5706 2023-05-12 16:18:28.187688 onboardme-1.0.2/onboardme/help_text.py
+-rw-r--r--   0        0        0     3123 2023-03-18 21:01:43.626062 onboardme-1.0.2/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.0.2/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8607 2023-05-12 16:18:28.188160 onboardme-1.0.2/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.0.2/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.0.2/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.0.2/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.0.2/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1919 2023-05-19 11:53:30.596668 onboardme-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13249 1970-01-01 00:00:00.000000 onboardme-1.0.2/PKG-INFO
```

### Comparing `onboardme-1.0.1/LICENSE.txt` & `onboardme-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/README.md` & `onboardme-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/__init__.py` & `onboardme-1.0.2/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/config/firewall/iptables.sh` & `onboardme-1.0.2/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/console_logging.py` & `onboardme-1.0.2/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/constants.py` & `onboardme-1.0.2/onboardme/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
        Name:
 DESCRIPTION:
      AUTHOR:
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version 3
 """
 from importlib.metadata import version as get_version
+import logging as log
 from xdg_base_dirs import xdg_config_home
 from os import getenv, path, uname
 from pathlib import Path
 import wget
 import yaml
 
 
@@ -34,27 +35,28 @@
 # package manager config is different per OS
 PKG_MNGRS = ['brew','pip3.11']
 if OS[0] == 'Linux':
     PKG_MNGRS.extend(['apt','snap','flatpak'])
 
 
 default_dotfiles = ("https://raw.githubusercontent.com/jessebot/dot_files/"
-                    "main/.config/onboardme/")
+                    "main/.config/onboardme/config.yml")
 
 
 def load_cfg(config_file='config.yml') -> dict:
     """
     load yaml config files for onboardme
     """
     config_dir = path.join(xdg_config_home(), 'onboardme')
     config_full_path = path.join(config_dir, config_file)
 
-    # defaults
+    # create default pathing and config file if it doesn't exist
     if not path.exists(config_full_path):
-        Path(config_dir).mkdir(exist_ok=True)
-        wget.download(default_dotfiles + config_file, config_full_path)
+        Path(config_dir).mkdir(parents=True, exist_ok=True)
+        # downloads a default config file from default dot files
+        wget.download(default_dotfiles, config_full_path)
 
     with open(config_full_path, 'r') as yaml_file:
         return yaml.safe_load(yaml_file)
 
 
 USR_CONFIG_FILE = load_cfg()
```

### Comparing `onboardme-1.0.1/onboardme/dot_files.py` & `onboardme-1.0.2/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/env_config.py` & `onboardme-1.0.2/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/firewall.py` & `onboardme-1.0.2/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/help_text.py` & `onboardme-1.0.2/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/ide_setup.py` & `onboardme-1.0.2/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/misc.py` & `onboardme-1.0.2/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/pkg_management.py` & `onboardme-1.0.2/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/subproc.py` & `onboardme-1.0.2/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/onboardme/sudo_setup.py` & `onboardme-1.0.2/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.1/pyproject.toml` & `onboardme-1.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.0.1"
+version       = "1.0.2"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
-authors       = ["Jesse Hitch <jessebot@linux.com>",
-                 "Max Roby <emax@cloudydev.net>"]
+authors       = [
+    "Jesse Hitch <jessebot@linux.com>",
+    "Max Roby <emax@cloudydev.net>"
+]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
 documentation = "https://jessebot.github.io/onboardme/onboardme"
 repository    = "http://github.com/jessebot/onboardme"
 keywords      = ["onboardme", "onboarding", "desktop-setup", "development-environment"]
 classifiers   = ["Development Status :: 3 - Alpha",
                  "Programming Language :: Python :: 3.11",
@@ -29,17 +31,17 @@
 wget                = "^3.2"
 xdg-base-dirs       = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1"
 
 [[tool.poetry.source]]
-name = "testpypi"
-url = "https://test.pypi.org/simple/"
-default = false
+name      = "testpypi"
+url       = "https://test.pypi.org/simple/"
+default   = false
 secondary = false
 
 [tool.poetry.plugins."onboardme.application.plugin"]
 "onboardme" = "onboardme:main"
 
 [tool.poetry.scripts]
 onboardme = 'onboardme:main'
```

### Comparing `onboardme-1.0.1/PKG-INFO` & `onboardme-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.0.1
+Version: 1.0.2
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.0.1 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.0.2 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
```

