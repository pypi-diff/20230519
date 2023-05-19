# Comparing `tmp/onboardme-1.0.2.tar.gz` & `tmp/onboardme-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.0.2.tar", max compression
+gzip compressed data, was "onboardme-1.1.0.tar", max compression
```

## Comparing `onboardme-1.0.2.tar` & `onboardme-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0    11868 2023-05-12 16:18:28.185568 onboardme-1.0.2/README.md
--rwxr-xr-x   0        0        0     6667 2023-03-18 21:01:43.622076 onboardme-1.0.2/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.0.2/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.0.2/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     2671 2022-11-18 16:13:55.305455 onboardme-1.0.2/onboardme/console_logging.py
--rw-r--r--   0        0        0     1691 2023-05-19 11:53:30.594074 onboardme-1.0.2/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.0.2/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.0.2/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.0.2/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5706 2023-05-12 16:18:28.187688 onboardme-1.0.2/onboardme/help_text.py
--rw-r--r--   0        0        0     3123 2023-03-18 21:01:43.626062 onboardme-1.0.2/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.0.2/onboardme/misc.py
--rwxr-xr-x   0        0        0     8607 2023-05-12 16:18:28.188160 onboardme-1.0.2/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.0.2/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.0.2/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.0.2/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.0.2/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1919 2023-05-19 11:53:30.596668 onboardme-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    13249 1970-01-01 00:00:00.000000 onboardme-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0    12541 2023-05-19 13:59:36.158335 onboardme-1.1.0/README.md
+-rwxr-xr-x   0        0        0     6667 2023-03-18 21:01:43.622076 onboardme-1.1.0/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.0/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.0/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     2671 2022-11-18 16:13:55.305455 onboardme-1.1.0/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1691 2023-05-19 11:53:30.594074 onboardme-1.1.0/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.0/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.0/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.0/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5706 2023-05-12 16:18:28.187688 onboardme-1.1.0/onboardme/help_text.py
+-rw-r--r--   0        0        0     3034 2023-05-19 16:01:08.369863 onboardme-1.1.0/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.0/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8607 2023-05-12 16:18:28.188160 onboardme-1.1.0/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.0/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.0/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.0/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.0/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1919 2023-05-19 16:18:56.198420 onboardme-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    13922 1970-01-01 00:00:00.000000 onboardme-1.1.0/PKG-INFO
```

### Comparing `onboardme-1.0.2/LICENSE.txt` & `onboardme-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/README.md` & `onboardme-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,19 @@
 
 </details>
 
 ### Easy `yaml` config files
 - [XDG Base Directory Spec] use for [config files](#configuration)
   - Uses `$XDG_CONFIG_HOME/onboardme/config.yml` and `$XDG_CONFIG_HOME/onboardme/packages.yml`
 
+### Docker image for an on-the-go dev workspace
+
+The docker image is built daily or on push to main. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
+See the [docker](#docker) section for more info!
+
 ### Other useful (but optional) configurations
 - Enable touchID for sudo on macOS
 - Add your user to the docker group
 - Install nerdfonts (defaults to Hack and Symbols Only)
 - Set capslock to control (🚧 in the works)
 
 ### Screenshots
@@ -125,14 +130,28 @@
 ```bash
 # should also work with pipx, if you'd like to use that instead
 pip install --user onboardme
 ```
 
 You can read more in depth at the [Getting Started Docs] 💙! There's also more [docs] on basically every program that onboardme touches.
 
+#### Docker
+
+To run the image locally with onboardme already run using default settings:
+```bash
+# this image is built daily and has already run onboardme with the default settings
+docker run jessebot/onboardme:latest /bin/bash
+```
+
+To run the image locally from scratch:
+```bash
+# onbaordme is installed but has _not_ been run. this is best if you have your own dot files
+docker run jessebot/onboardme:no-install /bin/bash
+```
+
 ### Upgrades
 If you're on python 3.11, you should be able to do:
 
 ```bash
 pip3.11 install --upgrade onboardme
 ```
```

#### html2text {}

```diff
@@ -30,18 +30,21 @@
 repo use pure vim anymore, so we can't ensure it's up to standards. All of your
 knowledge from vim is still helpful in neovim though, and we highly recommend
 switching as neovim has a lot more features and a very active plugin community
 :) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/
 doc/user/nvim.html#nvim-from-vim).  ### Easy `yaml` config files - [XDG Base
 Directory Spec] use for [config files](#configuration) - Uses
 `$XDG_CONFIG_HOME/onboardme/config.yml` and `$XDG_CONFIG_HOME/onboardme/
-packages.yml` ### Other useful (but optional) configurations - Enable touchID
-for sudo on macOS - Add your user to the docker group - Install nerdfonts
-(defaults to Hack and Symbols Only) - Set capslock to control (ð§ in the
-works) ### Screenshots  Example of onboardme --help
+packages.yml` ### Docker image for an on-the-go dev workspace The docker image
+is built daily or on push to main. The base image is `debian:bookworm`, but we
+will rollout support for Ubuntu down the line :) See the [docker](#docker)
+section for more info! ### Other useful (but optional) configurations - Enable
+touchID for sudo on macOS - Add your user to the docker group - Install
+nerdfonts (defaults to Hack and Symbols Only) - Set capslock to control (ð§
+in the works) ### Screenshots  Example of onboardme --help
                 [screenshot_of_full_output_of_onboardme_--help]
   Examples of the terminal after onboardme runs
 ### neovim [screenshot of neovim with colors] ### Powerline and ls [screenshot
  of powerline and lsd] ### Powerline with git [screenshot of powerline and git
   colors] ### Image and colors [screenshot of color samples and image of dog
   using a computer using sixel] ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
@@ -50,45 +53,50 @@
 download setup.sh to your current directory and run it /bin/bash -c "$(curl -
 fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)" #
 this will display the help text for the onboardme cli onboardme --help ``` If
 you've already got brew and Python3.11 on your machine, you can just do:
 ```bash # should also work with pipx, if you'd like to use that instead pip
 install --user onboardme ``` You can read more in depth at the [Getting Started
 Docs] ð! There's also more [docs] on basically every program that onboardme
-touches. ### Upgrades If you're on python 3.11, you should be able to do:
-```bash pip3.11 install --upgrade onboardme ``` ### Configuration onboardme has
-lots of CLI options, but you can also use config files. You have to create
-these files for the time being. Config files are in `~/.config/onboardme/`
-(will use `$XDG_CONFIG_HOME`, if defined). Examples below:  ~/.config/
-onboardme/config.yml ```yaml log: # Full path to a file you'd like to log to.
-Creates file if it doesn't exist file: "" # what level of logs to output
-(DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific function
-in the list of functions we run steps: # these are mac specific steps Darwin: #
-clones dot files into home dir/git fetches updates for dot files - dot_files #
-install packages - packages # adds nerdfonts - font_setup # runs :Lazy sync to
-install all your plugins - neovim_setup # sets up touchID for sudo - sudo_setup
-# these are linux specific steps Linux: - dot_files - packages - font_setup -
-neovim_setup # add your user to the docker group - group_setup dot_files: #
-personal git repo URL for your dot files, defaults to jessebot/dot_files
-git_url: "https://github.com/jessebot/dot_files.git" # the branch to use for
-the git repo above, defaults to main git_branch: "main" # !CAREFUL: runs a `git
-reset --hard`, which will overwite/delete local files in ~ that # conflict with
-the above defined git repo url and branch. You should run # `onboardme -
-s dot_files` to get the files that would be overwritten overwrite: false #
-basic package config package: # Remove any of the below pkg managers to only
-run the remaining pkg managers managers: # these are macOS specific steps
-Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
-pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
-install groups: - default # uncomment these to add them as default installed
-package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
-tested for these operating systems: [![Tested on Ventura with an M1 and older
-generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-
-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
-[Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-
-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+touches. #### Docker To run the image locally with onboardme already run using
+default settings: ```bash # this image is built daily and has already run
+onboardme with the default settings docker run jessebot/onboardme:latest /bin/
+bash ``` To run the image locally from scratch: ```bash # onbaordme is
+installed but has _not_ been run. this is best if you have your own dot files
+docker run jessebot/onboardme:no-install /bin/bash ``` ### Upgrades If you're
+on python 3.11, you should be able to do: ```bash pip3.11 install --upgrade
+onboardme ``` ### Configuration onboardme has lots of CLI options, but you can
+also use config files. You have to create these files for the time being.
+Config files are in `~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if
+defined). Examples below:  ~/.config/onboardme/config.yml ```yaml log: # Full
+path to a file you'd like to log to. Creates file if it doesn't exist file: ""
+# what level of logs to output (DEBUG, INFO, WARN, ERROR) level: "INFO" # steps
+refer to a specific function in the list of functions we run steps: # these are
+mac specific steps Darwin: # clones dot files into home dir/git fetches updates
+for dot files - dot_files # install packages - packages # adds nerdfonts -
+font_setup # runs :Lazy sync to install all your plugins - neovim_setup # sets
+up touchID for sudo - sudo_setup # these are linux specific steps Linux: -
+dot_files - packages - font_setup - neovim_setup # add your user to the docker
+group - group_setup dot_files: # personal git repo URL for your dot files,
+defaults to jessebot/dot_files git_url: "https://github.com/jessebot/
+dot_files.git" # the branch to use for the git repo above, defaults to main
+git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will overwite/
+delete local files in ~ that # conflict with the above defined git repo url and
+branch. You should run # `onboardme -s dot_files` to get the files that would
+be overwritten overwrite: false # basic package config package: # Remove any of
+the below pkg managers to only run the remaining pkg managers managers: # these
+are macOS specific steps Darwin: - brew - pip3.11 # these are linux specific
+steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of extra existing
+packages groups to install groups: - default # uncomment these to add them as
+default installed package groups # - gui # - gaming # - devops ```  ## Under
+the Hood Made and tested for these operating systems: [![Tested on Ventura with
+an M1 and older generation](https://img.shields.io/badge/mac%20os-
+000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/
+wiki/MacOS?lang=en) [![Tested only on Debian Bookworm](https://img.shields.io/
+badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
 www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
 badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
 ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
 (https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
 badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
 (https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
```

### Comparing `onboardme-1.0.2/onboardme/__init__.py` & `onboardme-1.1.0/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/config/firewall/iptables.sh` & `onboardme-1.1.0/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/console_logging.py` & `onboardme-1.1.0/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/constants.py` & `onboardme-1.1.0/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/dot_files.py` & `onboardme-1.1.0/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/env_config.py` & `onboardme-1.1.0/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/firewall.py` & `onboardme-1.1.0/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/help_text.py` & `onboardme-1.1.0/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/ide_setup.py` & `onboardme-1.1.0/onboardme/ide_setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 NAME:    Onboardme.ide_setup
 DESC:    install vim, neovim, and fonts
-AUTHOR:  Jesse Hitch
+AUTHORS:  Jesse Hitch, Max Roby
 LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE
 """
 
 import logging as log
 from git import Repo, RemoteProgress
 from os import path
 from pathlib import Path
@@ -15,16 +15,16 @@
 from .console_logging import print_header, print_sub_header, print_msg
 from .subproc import subproc
 
 
 def font_setup() -> None:
     """
     On Linux:
-      Clones nerd-fonts repo and does a sparse checkout on only mononoki and
-      hack fonts. Also removes 70-no-bitmaps.conf and links 70-yes-bitmaps.conf
+      Clones nerd-fonts repo and does a sparse checkout on only mononoki font.
+      Also removes 70-no-bitmaps.conf and links 70-yes-bitmaps.conf
 
       Then runs install.sh from nerd-fonts repo
     """
     if 'Linux' in OS:
         print_header('📝 [i]font[/i] installations')
         # not sure if needed anymore
         # mkdir -p ~/.local/share/fonts
@@ -53,33 +53,31 @@
                 def update(self, op_code, cur_count, max_count=None,
                            message=''):
                     if message:
                         log.info(message)
 
             Repo.clone_from(fonts_repo, fonts_dir, progress=CloneProgress(),
                             multi_options=['--sparse', '--filter=blob:none'])
-            cmds = ["git sparse-checkout add patched-fonts/Mononoki",
-                    "git sparse-checkout add patched-fonts/Hack"]
+            cmds = ["git sparse-checkout add patched-fonts/Mononoki"]
             subproc(cmds, spinner=True, cwd=fonts_dir)
         else:
             subproc(["git pull"], spinner=True, cwd=fonts_dir)
 
-        subproc(['./install.sh Hack', './install.sh Mononoki'], quiet=True,
+        subproc(['./install.sh Mononoki'], quiet=True,
                 cwd=fonts_dir)
 
         print_msg('[i][dim]The fonts should be installed, however, you have ' +
                   'to set your terminal font to the new font. I rebooted too.')
 
 
 def neovim_setup() -> None:
     """
-    Installs all 
+    Installs all plugins and syncs them if needed.
     Runs this command that works via the cli:
         nvim --headless "+Lazy! sync" +qa
     """
     print_header('[green][i]NeoVim[/i][/green] plugins installation '
                  '[dim]and[/dim] upgrades via [green]lazy.nvim[/green]')
 
-    # updates all currently plugins
     subproc(['nvim --headless "+Lazy! sync" +qa'])
 
     print_sub_header('NeoVim Plugins installed.')
```

### Comparing `onboardme-1.0.2/onboardme/misc.py` & `onboardme-1.1.0/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/pkg_management.py` & `onboardme-1.1.0/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/subproc.py` & `onboardme-1.1.0/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/onboardme/sudo_setup.py` & `onboardme-1.1.0/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.0.2/pyproject.toml` & `onboardme-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.0.2"
+version       = "1.1.0"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.0.2/PKG-INFO` & `onboardme-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.0.2
+Version: 1.1.0
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
@@ -91,14 +91,19 @@
 
 </details>
 
 ### Easy `yaml` config files
 - [XDG Base Directory Spec] use for [config files](#configuration)
   - Uses `$XDG_CONFIG_HOME/onboardme/config.yml` and `$XDG_CONFIG_HOME/onboardme/packages.yml`
 
+### Docker image for an on-the-go dev workspace
+
+The docker image is built daily or on push to main. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
+See the [docker](#docker) section for more info!
+
 ### Other useful (but optional) configurations
 - Enable touchID for sudo on macOS
 - Add your user to the docker group
 - Install nerdfonts (defaults to Hack and Symbols Only)
 - Set capslock to control (🚧 in the works)
 
 ### Screenshots
@@ -155,14 +160,28 @@
 ```bash
 # should also work with pipx, if you'd like to use that instead
 pip install --user onboardme
 ```
 
 You can read more in depth at the [Getting Started Docs] 💙! There's also more [docs] on basically every program that onboardme touches.
 
+#### Docker
+
+To run the image locally with onboardme already run using default settings:
+```bash
+# this image is built daily and has already run onboardme with the default settings
+docker run jessebot/onboardme:latest /bin/bash
+```
+
+To run the image locally from scratch:
+```bash
+# onbaordme is installed but has _not_ been run. this is best if you have your own dot files
+docker run jessebot/onboardme:no-install /bin/bash
+```
+
 ### Upgrades
 If you're on python 3.11, you should be able to do:
 
 ```bash
 pip3.11 install --upgrade onboardme
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.0.2 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.1.0 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
@@ -49,18 +49,21 @@
 repo use pure vim anymore, so we can't ensure it's up to standards. All of your
 knowledge from vim is still helpful in neovim though, and we highly recommend
 switching as neovim has a lot more features and a very active plugin community
 :) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/
 doc/user/nvim.html#nvim-from-vim).  ### Easy `yaml` config files - [XDG Base
 Directory Spec] use for [config files](#configuration) - Uses
 `$XDG_CONFIG_HOME/onboardme/config.yml` and `$XDG_CONFIG_HOME/onboardme/
-packages.yml` ### Other useful (but optional) configurations - Enable touchID
-for sudo on macOS - Add your user to the docker group - Install nerdfonts
-(defaults to Hack and Symbols Only) - Set capslock to control (ð§ in the
-works) ### Screenshots  Example of onboardme --help
+packages.yml` ### Docker image for an on-the-go dev workspace The docker image
+is built daily or on push to main. The base image is `debian:bookworm`, but we
+will rollout support for Ubuntu down the line :) See the [docker](#docker)
+section for more info! ### Other useful (but optional) configurations - Enable
+touchID for sudo on macOS - Add your user to the docker group - Install
+nerdfonts (defaults to Hack and Symbols Only) - Set capslock to control (ð§
+in the works) ### Screenshots  Example of onboardme --help
                 [screenshot_of_full_output_of_onboardme_--help]
   Examples of the terminal after onboardme runs
 ### neovim [screenshot of neovim with colors] ### Powerline and ls [screenshot
  of powerline and lsd] ### Powerline with git [screenshot of powerline and git
   colors] ### Image and colors [screenshot of color samples and image of dog
   using a computer using sixel] ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
@@ -69,45 +72,50 @@
 download setup.sh to your current directory and run it /bin/bash -c "$(curl -
 fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)" #
 this will display the help text for the onboardme cli onboardme --help ``` If
 you've already got brew and Python3.11 on your machine, you can just do:
 ```bash # should also work with pipx, if you'd like to use that instead pip
 install --user onboardme ``` You can read more in depth at the [Getting Started
 Docs] ð! There's also more [docs] on basically every program that onboardme
-touches. ### Upgrades If you're on python 3.11, you should be able to do:
-```bash pip3.11 install --upgrade onboardme ``` ### Configuration onboardme has
-lots of CLI options, but you can also use config files. You have to create
-these files for the time being. Config files are in `~/.config/onboardme/`
-(will use `$XDG_CONFIG_HOME`, if defined). Examples below:  ~/.config/
-onboardme/config.yml ```yaml log: # Full path to a file you'd like to log to.
-Creates file if it doesn't exist file: "" # what level of logs to output
-(DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific function
-in the list of functions we run steps: # these are mac specific steps Darwin: #
-clones dot files into home dir/git fetches updates for dot files - dot_files #
-install packages - packages # adds nerdfonts - font_setup # runs :Lazy sync to
-install all your plugins - neovim_setup # sets up touchID for sudo - sudo_setup
-# these are linux specific steps Linux: - dot_files - packages - font_setup -
-neovim_setup # add your user to the docker group - group_setup dot_files: #
-personal git repo URL for your dot files, defaults to jessebot/dot_files
-git_url: "https://github.com/jessebot/dot_files.git" # the branch to use for
-the git repo above, defaults to main git_branch: "main" # !CAREFUL: runs a `git
-reset --hard`, which will overwite/delete local files in ~ that # conflict with
-the above defined git repo url and branch. You should run # `onboardme -
-s dot_files` to get the files that would be overwritten overwrite: false #
-basic package config package: # Remove any of the below pkg managers to only
-run the remaining pkg managers managers: # these are macOS specific steps
-Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
-pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
-install groups: - default # uncomment these to add them as default installed
-package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
-tested for these operating systems: [![Tested on Ventura with an M1 and older
-generation](https://img.shields.io/badge/mac%20os-000000?style=for-the-
-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
-[Tested only on Debian Bookworm](https://img.shields.io/badge/Debian-
-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
+touches. #### Docker To run the image locally with onboardme already run using
+default settings: ```bash # this image is built daily and has already run
+onboardme with the default settings docker run jessebot/onboardme:latest /bin/
+bash ``` To run the image locally from scratch: ```bash # onbaordme is
+installed but has _not_ been run. this is best if you have your own dot files
+docker run jessebot/onboardme:no-install /bin/bash ``` ### Upgrades If you're
+on python 3.11, you should be able to do: ```bash pip3.11 install --upgrade
+onboardme ``` ### Configuration onboardme has lots of CLI options, but you can
+also use config files. You have to create these files for the time being.
+Config files are in `~/.config/onboardme/` (will use `$XDG_CONFIG_HOME`, if
+defined). Examples below:  ~/.config/onboardme/config.yml ```yaml log: # Full
+path to a file you'd like to log to. Creates file if it doesn't exist file: ""
+# what level of logs to output (DEBUG, INFO, WARN, ERROR) level: "INFO" # steps
+refer to a specific function in the list of functions we run steps: # these are
+mac specific steps Darwin: # clones dot files into home dir/git fetches updates
+for dot files - dot_files # install packages - packages # adds nerdfonts -
+font_setup # runs :Lazy sync to install all your plugins - neovim_setup # sets
+up touchID for sudo - sudo_setup # these are linux specific steps Linux: -
+dot_files - packages - font_setup - neovim_setup # add your user to the docker
+group - group_setup dot_files: # personal git repo URL for your dot files,
+defaults to jessebot/dot_files git_url: "https://github.com/jessebot/
+dot_files.git" # the branch to use for the git repo above, defaults to main
+git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will overwite/
+delete local files in ~ that # conflict with the above defined git repo url and
+branch. You should run # `onboardme -s dot_files` to get the files that would
+be overwritten overwrite: false # basic package config package: # Remove any of
+the below pkg managers to only run the remaining pkg managers managers: # these
+are macOS specific steps Darwin: - brew - pip3.11 # these are linux specific
+steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of extra existing
+packages groups to install groups: - default # uncomment these to add them as
+default installed package groups # - gui # - gaming # - devops ```  ## Under
+the Hood Made and tested for these operating systems: [![Tested on Ventura with
+an M1 and older generation](https://img.shields.io/badge/mac%20os-
+000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/
+wiki/MacOS?lang=en) [![Tested only on Debian Bookworm](https://img.shields.io/
+badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
 www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
 badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
 ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
 (https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
 badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
 (https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
```

