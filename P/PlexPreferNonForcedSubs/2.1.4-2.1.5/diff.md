# Comparing `tmp/PlexPreferNonForcedSubs-2.1.4.tar.gz` & `tmp/PlexPreferNonForcedSubs-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexPreferNonForcedSubs-2.1.4.tar", last modified: Tue May  9 15:10:45 2023, max compression
+gzip compressed data, was "PlexPreferNonForcedSubs-2.1.5.tar", last modified: Thu May 18 22:07:46 2023, max compression
```

## Comparing `PlexPreferNonForcedSubs-2.1.4.tar` & `PlexPreferNonForcedSubs-2.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 15:10:45.048911 PlexPreferNonForcedSubs-2.1.4/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.1.4/LICENSE
--rw-rw-rw-   0        0        0     5436 2023-05-09 15:10:45.047913 PlexPreferNonForcedSubs-2.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 15:10:45.009962 PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs/
--rw-rw-rw-   0        0        0     6525 2023-05-09 15:09:54.000000 PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
--rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:10:45.045915 PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs.egg-info/
--rw-rw-rw-   0        0        0     5436 2023-05-09 15:10:44.000000 PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-05-09 15:10:44.000000 PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 15:10:44.000000 PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-05-09 15:10:44.000000 PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-05-09 15:10:44.000000 PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-09 15:10:44.000000 PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4792 2023-05-09 14:55:37.000000 PlexPreferNonForcedSubs-2.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 15:10:45.048911 PlexPreferNonForcedSubs-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1516 2023-05-09 15:10:11.000000 PlexPreferNonForcedSubs-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:07:46.249098 PlexPreferNonForcedSubs-2.1.5/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6139 2023-05-18 22:07:46.247098 PlexPreferNonForcedSubs-2.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 22:07:46.207098 PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs/
+-rw-rw-rw-   0        0        0     7502 2023-05-18 21:59:15.000000 PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 18:48:34.000000 PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:07:46.245096 PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs.egg-info/
+-rw-rw-rw-   0        0        0     6139 2023-05-18 22:07:46.000000 PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-05-18 22:07:46.000000 PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 22:07:46.000000 PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-05-18 22:07:46.000000 PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 22:07:46.000000 PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-18 22:07:46.000000 PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5455 2023-05-18 22:03:50.000000 PlexPreferNonForcedSubs-2.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 22:07:46.249098 PlexPreferNonForcedSubs-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2023-05-18 22:07:23.000000 PlexPreferNonForcedSubs-2.1.5/setup.py
```

### Comparing `PlexPreferNonForcedSubs-2.1.4/LICENSE` & `PlexPreferNonForcedSubs-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.1.4/PKG-INFO` & `PlexPreferNonForcedSubs-2.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,101 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.1.4
+Version: 2.1.5
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PlexPreferNonForcedSubs
 
+## Short Description
+This Python script sets all movies and shows in your local Plex library to English non-forced subtitles by default. It is compatible with Python 3.5 or later and designed to work on any operating system where Python is installed (Windows, macOS, Linux, etc).
 
-## Short description:
-This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. This script should work on any OS where Python is installed (Windows, MacOS and Linux etc).
+## Long Description
+This script utilizes the Plex Python API and sets all movies and shows in your local Plex library to English non-forced subtitles by default. The subtitle preferences will be applied to your Plex profile and remembered on other devices. By default, Plex prefers forced subtitles when available for a given item. However, Plex does not natively allow you to prefer non-forced subtitles, which is why this script was created.
 
-## Long description:
-This script was created with the help of [ChatGPT Open AI](https://chat.openai.com/chat) and further edited and completed by me. It uses [Plex Python Api](https://python-plexapi.readthedocs.io/en/latest/). It will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. Assuming your Plex subtitles settings are setup in your server settings Plex will default to Forced Subtitles by default when they are available for a given item. Plex will not allow you to prefer non forced subtitles natively hence why this script was created.
-
-This script is confirmed tested and working. Feel free to use this code for your own purposes. I will be running this code periodically on my home server along with some of my other neat little plex scripts like [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Thanks to [all](https://stackoverflow.com/questions/75027919/python-script-to-set-all-subtitles-for-movies-shows-in-plex-to-english-non-for) who helped! If you use this script and run into any bugs feel free to open an issue. Cheers!
+The script has been thoroughly tested and confirmed to be working. Feel free to use the code for your own purposes. I will be running this code periodically on my home server along with some other Plex scripts, such as [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Special thanks to everyone who provided assistance! If you encounter any bugs while using this script, please open an issue. Cheers!
 
 ## What are "non-forced" subtitles?
 Non-forced subtitles provide subtitles everytime a characters speaks.
 
 ## What are "forced" subtitles?
 Forced subtitles only provide subtitles when the characters speak a foreign or alien language.
 
-
-## Install Instructions:
-1. Install [Python](https://www.python.org/downloads/).
-2. Run `python -m pip install PlexPreferNonForcedSubs` in command line.
-3. Make sure Plex media server is running then run the script using `PlexPreferNonForcedSubs` in command line.
-4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
+## Installation Instructions
+1. Install [Python](https://www.python.org/downloads/) (v3.5 or later).
+2. Install the script by executing the following in the command line: `python -m pip install PlexPreferNonForcedSubs`.
+3. Ensure that your Plex media server is running, then run the script using `PlexPreferNonForcedSubs` in the command line.
+4. On the first run, the script will prompt you to enter your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). The token will be saved locally in the same folder as `token.txt`.
+5. Done, setup complete. The script will continue to run and set all movies and shows in your local Plex library to use English non-forced subtitles.
+
+See the section below for instructions on how to run, update, and uninstall the script.
+
+## Installing the Script:
+```
+python -m pip install PlexPreferNonForcedSubs
+```
+_Execute in your operating system's native command line._
+## Running the Script:
+```
+PlexPreferNonForcedSubs
+```
+_Execute in your operating system's native command line._
+## Updating the Script:
+```
+python -m pip install PlexPreferNonForcedSubs --upgrade
+```
+_Execute in your operating system's native command line._
+## Uninstalling the Script:
+```
+python -m pip uninstall PlexPreferNonForcedSubs
+```
+_Execute in your operating system's native command line._
+
+## Installing a Specific Version:
+```
+python -m pip install PlexPreferNonForcedSubs==VERSION_NUMBER
+```
+_Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) (e.g. 2.1.4) and execute in your operating system's native command line._
+
+## Alternative Manual Installation Method (without pip install):
+1. Install [Python](https://www.python.org/downloads/) (v3.5 or later).
+2. Download the latest `.py` script from the [releases page](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) and move it to the desired directory.
+3. Execute the script by running `PlexPreferNonForcedSubs.py`, or open the terminal and navigate to the folder where `PlexPreferNonForcedSubs.py` is located, then run `PlexPreferNonForcedSubs.py` in the terminal.
+4. On the first run, the script will prompt you to enter your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). The token will be saved locally in the same folder as `token.txt`.
 5. Done.
 
-_See [below](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
+See the section above for instructions on how to run, update, and uninstall the script.
 
-### Run:
-`PlexPreferNonForcedSubs` in command line.
+## Known Issues/Future Outlook
+- Some lines of redundant code can be shortened and/or removed. Refer to [this issue](https://github.com/RileyXX/PlexPreferNonForcedSubs/issues/4) for more details.
 
-### Update:
-`python -m pip install PlexPreferNonForcedSubs --upgrade` in command line.
-### Uninstall:
-`python -m pip uninstall PlexPreferNonForcedSubs` in command line.
-
-## Alternative manual no install method:
-1. Download the latest .py script from the [releases page](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) and move it to the file directory of your choice.
-2. Run the script by running `PlexPreferNonForcedSubs.py` OR open terminal and navigate to folder where `PlexPreferNonForcedSubs.py` is located. Run `PlexPreferNonForcedSubs.py` in terminal. 
-4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
-3. Done.
-
-_See [above](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
-
-## Known issues/future outlook:
-* Several lines of redundant code can be shortened and/or removed
-
-## Also posted on:
-* [Stackoverflow](https://stackoverflow.com/q/75027919/9196825)
-* [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
-* [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
+## Also Posted On
+- [PyPi](https://pypi.org/project/PlexPreferNonForcedSubs/)
+- [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
+- [Stack Overflow](https://stackoverflow.com/q/75027919/9196825)
+- [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
 
 ## Screenshots:
 ##### Plex subtitle dropdown after script is done running:
 ![Plex Subtitle Dropdown](https://i.imgur.com/BNOlwtL.png)
 ##### PlexPreferNonForcedSubs.py script in action:
 ![PlexPreferNonForcedSubs.py Script in Action](https://github.com/RileyXX/PlexPreferNonForcedSubs/raw/main/demo.gif)
 
-## Sponsorships, Donations and Custom Projects:
-Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
+## Sponsorships, Donations, and Custom Projects
+If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
 
-#### More donation options:
+#### More Donation Options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
-<br>
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
```

### Comparing `PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py` & `PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,111 @@
 from plexapi.server import PlexServer
 from plexapi.media import SubtitleStream
 import os
+import traceback
+
+def report_error(error_message):
+    github_issue_url = "https://github.com/RileyXX/PlexPreferNonForcedSubs/issues/new?assignees=&labels=&projects=&template=bug_report.yml"
+    traceback_info = traceback.format_exc()
+
+    print("\n--- ERROR ---")
+    print(error_message)
+    print("Please submit the error to GitHub with the following information:")
+    print("-" * 50)
+    print(traceback_info)
+    print("-" * 50)
+    print(f"Submit the error here: {github_issue_url}")
+    print("-" * 50)
 
 def main():
-    # Connect to Plex Media Server. Replace PLEX_TOKEN below with your Plex token. How to get token: https://www.plexopedia.com/plex-media-server/general/plex-token/
-    baseurl = 'http://localhost:32400'
-    token = 'PLEX_TOKEN'
-
-    script_dir = os.path.dirname(os.path.abspath(__file__))
-    token_file = os.path.join(script_dir, 'token.txt')
-
-    try:
-        with open(token_file, 'r') as f:
-            token = f.read().strip()
-    except FileNotFoundError:
-        pass
-
-    if token == 'PLEX_TOKEN':
-        print(f'\nHow to get your Plex token: https://www.plexopedia.com/plex-media-server/general/plex-token/\n')
-        token = input("Enter your Plex token: ")
-        with open(token_file, 'w') as f:
-            f.write(token)
-
-    plex = PlexServer(baseurl, token)
-
-    # Movies
-    table_headers = ['Title', 'Year', 'Status', 'Changes']
-    title_width = 70
-    year_width = 5
-    status_width = 20
-    changes_width = 8
-
-    print("\n" + "-" * 114 + "\nMovies\n" + "-" * 114)
-    print(f'\033[1m\033[96m{" | ".join([h.ljust(title_width if i == 0 else year_width if i == 1 else status_width if i == 2 else changes_width) for i, h in enumerate(table_headers)])}\033[0m')
-
-    for section in plex.library.sections():
-        if section.type == 'movie':
-            for movie in section.all():
-                english_subs = movie.subtitleStreams()
-                if english_subs is not None:
-                    english_subs = [stream for stream in english_subs if stream is not None and stream.languageCode == 'eng']
-                    non_forced_english_subs = [stream for stream in english_subs if stream is not None and (not stream.forced or ('forced' not in getattr(stream, 'title', '').lower()))]
-                    forced_english_subs = [stream for stream in english_subs if stream is not None and (hasattr(stream, 'title') and stream.title is not None and 'forced' in stream.title.lower())]
-                    part = movie.media[0].parts[0]
-                    partsid = part.id
-                    if forced_english_subs and non_forced_english_subs:
-                        non_forced_english_subs[0].setDefault()
-                        print(f'\033[92m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English (Non-Forced)".ljust(status_width)} | {"Y".ljust(changes_width)}\033[0m')
-                    elif non_forced_english_subs and not forced_english_subs:
-                        print(f'{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English".ljust(status_width)} | {"N".ljust(changes_width)}')
-                    elif not non_forced_english_subs and not forced_english_subs:
-                        print(f'\033[91m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"No Subtitles Found".ljust(status_width)} | {"N".ljust(changes_width)}\033[0m')
-                    else:
-                        print(f'\033[91m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English (Forced)".ljust(status_width)} | {"N (Error)".ljust(changes_width)}\033[0m')
-
-    # Shows
-    table_headers = ['Title', 'Year', 'Season #', 'Episode #', 'Status', 'Changes']
-    title_width = 42
-    year_width = 5
-    season_width = 11
-    episode_width = 11
-    status_width = 20
-    changes_width = 8
-    season_row_width = 4
-    episode_row_width = 3
-
-    print("\n" + "-" * 114 + "\nShows\n" + "-" * 114)
-    print(f'\033[1m\033[96m{" | ".join([h.ljust(title_width if i == 0 else year_width if i == 1 else season_width if i == 2 else episode_width if i == 3 else status_width if i == 4 else changes_width) for i, h in enumerate(table_headers)])}\033[0m')
-
-    for section in plex.library.sections():
-        if section.type == 'show':
-            for show in section.all():
-                for episode in show.episodes():
-                    english_subs = episode.subtitleStreams()
+        # Connect to Plex Media Server. Replace PLEX_TOKEN below with your Plex token. How to get token: https://www.plexopedia.com/plex-media-server/general/plex-token/
+        baseurl = 'http://localhost:32400'
+        token = 'PLEX_TOKEN'
+
+        script_dir = os.path.dirname(os.path.abspath(__file__))
+        token_file = os.path.join(script_dir, 'token.txt')
+
+        try:
+            with open(token_file, 'r') as f:
+                token = f.read().strip()
+        except FileNotFoundError:
+            pass
+
+        if token == 'PLEX_TOKEN':
+            print(f'\nHow to get your Plex token: https://www.plexopedia.com/plex-media-server/general/plex-token/\n')
+            token = input("Enter your Plex token: ")
+            with open(token_file, 'w') as f:
+                f.write(token)
+
+        plex = PlexServer(baseurl, token)
+
+        # Movies
+        table_headers = ['Title', 'Year', 'Status', 'Changes']
+        title_width = 70
+        year_width = 5
+        status_width = 20
+        changes_width = 8
+
+        print("\n" + "-" * 114 + "\nMovies\n" + "-" * 114)
+        print(f'\033[1m\033[96m{" | ".join([h.ljust(title_width if i == 0 else year_width if i == 1 else status_width if i == 2 else changes_width) for i, h in enumerate(table_headers)])}\033[0m')
+
+        for section in plex.library.sections():
+            if section.type == 'movie':
+                for movie in section.all():
+                    english_subs = movie.subtitleStreams()
                     if english_subs is not None:
                         english_subs = [stream for stream in english_subs if stream is not None and stream.languageCode == 'eng']
                         non_forced_english_subs = [stream for stream in english_subs if stream is not None and (not stream.forced or ('forced' not in getattr(stream, 'title', '').lower()))]
                         forced_english_subs = [stream for stream in english_subs if stream is not None and (hasattr(stream, 'title') and stream.title is not None and 'forced' in stream.title.lower())]
-                        part = episode.media[0].parts[0]
+                        part = movie.media[0].parts[0]
                         partsid = part.id
                         if forced_english_subs and non_forced_english_subs:
                             non_forced_english_subs[0].setDefault()
-                            print(f'\033[92m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English (Non-Forced)".ljust(status_width)} | {"Y".ljust(changes_width)}\033[0m')
+                            print(f'\033[92m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English (Non-Forced)".ljust(status_width)} | {"Y".ljust(changes_width)}\033[0m')
                         elif non_forced_english_subs and not forced_english_subs:
-                            print(f'{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English".ljust(status_width)} | {"N".ljust(changes_width)}')
+                            print(f'{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English".ljust(status_width)} | {"N".ljust(changes_width)}')
                         elif not non_forced_english_subs and not forced_english_subs:
-                            print(f'\033[91m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"No Subtitles Found".ljust(status_width)} | {"N".ljust(changes_width)}\033[0m')
+                            print(f'\033[91m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"No Subtitles Found".ljust(status_width)} | {"N".ljust(changes_width)}\033[0m')
                         else:
-                            print(f'\033[91m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English (Forced)".ljust(status_width)} | {"N (Error)".ljust(changes_width)}\033[0m')
+                            print(f'\033[91m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English (Forced)".ljust(status_width)} | {"N (Error)".ljust(changes_width)}\033[0m')
+
+        # Shows
+        table_headers = ['Title', 'Year', 'Season #', 'Episode #', 'Status', 'Changes']
+        title_width = 42
+        year_width = 5
+        season_width = 11
+        episode_width = 11
+        status_width = 20
+        changes_width = 8
+        season_row_width = 4
+        episode_row_width = 3
+
+        print("\n" + "-" * 114 + "\nShows\n" + "-" * 114)
+        print(f'\033[1m\033[96m{" | ".join([h.ljust(title_width if i == 0 else year_width if i == 1 else season_width if i == 2 else episode_width if i == 3 else status_width if i == 4 else changes_width) for i, h in enumerate(table_headers)])}\033[0m')
+
+        for section in plex.library.sections():
+            if section.type == 'show':
+                for show in section.all():
+                    for episode in show.episodes():
+                        english_subs = episode.subtitleStreams()
+                        if english_subs is not None:
+                            english_subs = [stream for stream in english_subs if stream is not None and stream.languageCode == 'eng']
+                            non_forced_english_subs = [stream for stream in english_subs if stream is not None and (not stream.forced or ('forced' not in getattr(stream, 'title', '').lower()))]
+                            forced_english_subs = [stream for stream in english_subs if stream is not None and (hasattr(stream, 'title') and stream.title is not None and 'forced' in stream.title.lower())]
+                            part = episode.media[0].parts[0]
+                            partsid = part.id
+                            if forced_english_subs and non_forced_english_subs:
+                                non_forced_english_subs[0].setDefault()
+                                print(f'\033[92m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English (Non-Forced)".ljust(status_width)} | {"Y".ljust(changes_width)}\033[0m')
+                            elif non_forced_english_subs and not forced_english_subs:
+                                print(f'{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English".ljust(status_width)} | {"N".ljust(changes_width)}')
+                            elif not non_forced_english_subs and not forced_english_subs:
+                                print(f'\033[91m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"No Subtitles Found".ljust(status_width)} | {"N".ljust(changes_width)}\033[0m')
+                            else:
+                                print(f'\033[91m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English (Forced)".ljust(status_width)} | {"N (Error)".ljust(changes_width)}\033[0m')
+
+    except Exception as e:
+        error_message = "An error occurred while running the script."
+        errorHandling.report_error(error_message)
 
 if __name__ == '__main__':
     main()
```

### Comparing `PlexPreferNonForcedSubs-2.1.4/PlexPreferNonForcedSubs.egg-info/PKG-INFO` & `PlexPreferNonForcedSubs-2.1.5/PlexPreferNonForcedSubs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,101 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.1.4
+Version: 2.1.5
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PlexPreferNonForcedSubs
 
+## Short Description
+This Python script sets all movies and shows in your local Plex library to English non-forced subtitles by default. It is compatible with Python 3.5 or later and designed to work on any operating system where Python is installed (Windows, macOS, Linux, etc).
 
-## Short description:
-This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. This script should work on any OS where Python is installed (Windows, MacOS and Linux etc).
+## Long Description
+This script utilizes the Plex Python API and sets all movies and shows in your local Plex library to English non-forced subtitles by default. The subtitle preferences will be applied to your Plex profile and remembered on other devices. By default, Plex prefers forced subtitles when available for a given item. However, Plex does not natively allow you to prefer non-forced subtitles, which is why this script was created.
 
-## Long description:
-This script was created with the help of [ChatGPT Open AI](https://chat.openai.com/chat) and further edited and completed by me. It uses [Plex Python Api](https://python-plexapi.readthedocs.io/en/latest/). It will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. Assuming your Plex subtitles settings are setup in your server settings Plex will default to Forced Subtitles by default when they are available for a given item. Plex will not allow you to prefer non forced subtitles natively hence why this script was created.
-
-This script is confirmed tested and working. Feel free to use this code for your own purposes. I will be running this code periodically on my home server along with some of my other neat little plex scripts like [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Thanks to [all](https://stackoverflow.com/questions/75027919/python-script-to-set-all-subtitles-for-movies-shows-in-plex-to-english-non-for) who helped! If you use this script and run into any bugs feel free to open an issue. Cheers!
+The script has been thoroughly tested and confirmed to be working. Feel free to use the code for your own purposes. I will be running this code periodically on my home server along with some other Plex scripts, such as [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Special thanks to everyone who provided assistance! If you encounter any bugs while using this script, please open an issue. Cheers!
 
 ## What are "non-forced" subtitles?
 Non-forced subtitles provide subtitles everytime a characters speaks.
 
 ## What are "forced" subtitles?
 Forced subtitles only provide subtitles when the characters speak a foreign or alien language.
 
-
-## Install Instructions:
-1. Install [Python](https://www.python.org/downloads/).
-2. Run `python -m pip install PlexPreferNonForcedSubs` in command line.
-3. Make sure Plex media server is running then run the script using `PlexPreferNonForcedSubs` in command line.
-4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
+## Installation Instructions
+1. Install [Python](https://www.python.org/downloads/) (v3.5 or later).
+2. Install the script by executing the following in the command line: `python -m pip install PlexPreferNonForcedSubs`.
+3. Ensure that your Plex media server is running, then run the script using `PlexPreferNonForcedSubs` in the command line.
+4. On the first run, the script will prompt you to enter your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). The token will be saved locally in the same folder as `token.txt`.
+5. Done, setup complete. The script will continue to run and set all movies and shows in your local Plex library to use English non-forced subtitles.
+
+See the section below for instructions on how to run, update, and uninstall the script.
+
+## Installing the Script:
+```
+python -m pip install PlexPreferNonForcedSubs
+```
+_Execute in your operating system's native command line._
+## Running the Script:
+```
+PlexPreferNonForcedSubs
+```
+_Execute in your operating system's native command line._
+## Updating the Script:
+```
+python -m pip install PlexPreferNonForcedSubs --upgrade
+```
+_Execute in your operating system's native command line._
+## Uninstalling the Script:
+```
+python -m pip uninstall PlexPreferNonForcedSubs
+```
+_Execute in your operating system's native command line._
+
+## Installing a Specific Version:
+```
+python -m pip install PlexPreferNonForcedSubs==VERSION_NUMBER
+```
+_Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) (e.g. 2.1.4) and execute in your operating system's native command line._
+
+## Alternative Manual Installation Method (without pip install):
+1. Install [Python](https://www.python.org/downloads/) (v3.5 or later).
+2. Download the latest `.py` script from the [releases page](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) and move it to the desired directory.
+3. Execute the script by running `PlexPreferNonForcedSubs.py`, or open the terminal and navigate to the folder where `PlexPreferNonForcedSubs.py` is located, then run `PlexPreferNonForcedSubs.py` in the terminal.
+4. On the first run, the script will prompt you to enter your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). The token will be saved locally in the same folder as `token.txt`.
 5. Done.
 
-_See [below](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
+See the section above for instructions on how to run, update, and uninstall the script.
 
-### Run:
-`PlexPreferNonForcedSubs` in command line.
+## Known Issues/Future Outlook
+- Some lines of redundant code can be shortened and/or removed. Refer to [this issue](https://github.com/RileyXX/PlexPreferNonForcedSubs/issues/4) for more details.
 
-### Update:
-`python -m pip install PlexPreferNonForcedSubs --upgrade` in command line.
-### Uninstall:
-`python -m pip uninstall PlexPreferNonForcedSubs` in command line.
-
-## Alternative manual no install method:
-1. Download the latest .py script from the [releases page](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) and move it to the file directory of your choice.
-2. Run the script by running `PlexPreferNonForcedSubs.py` OR open terminal and navigate to folder where `PlexPreferNonForcedSubs.py` is located. Run `PlexPreferNonForcedSubs.py` in terminal. 
-4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
-3. Done.
-
-_See [above](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
-
-## Known issues/future outlook:
-* Several lines of redundant code can be shortened and/or removed
-
-## Also posted on:
-* [Stackoverflow](https://stackoverflow.com/q/75027919/9196825)
-* [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
-* [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
+## Also Posted On
+- [PyPi](https://pypi.org/project/PlexPreferNonForcedSubs/)
+- [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
+- [Stack Overflow](https://stackoverflow.com/q/75027919/9196825)
+- [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
 
 ## Screenshots:
 ##### Plex subtitle dropdown after script is done running:
 ![Plex Subtitle Dropdown](https://i.imgur.com/BNOlwtL.png)
 ##### PlexPreferNonForcedSubs.py script in action:
 ![PlexPreferNonForcedSubs.py Script in Action](https://github.com/RileyXX/PlexPreferNonForcedSubs/raw/main/demo.gif)
 
-## Sponsorships, Donations and Custom Projects:
-Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
+## Sponsorships, Donations, and Custom Projects
+If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
 
-#### More donation options:
+#### More Donation Options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
-<br>
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
```

### Comparing `PlexPreferNonForcedSubs-2.1.4/README.md` & `PlexPreferNonForcedSubs-2.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,86 @@
 # PlexPreferNonForcedSubs
 
+## Short Description
+This Python script sets all movies and shows in your local Plex library to English non-forced subtitles by default. It is compatible with Python 3.5 or later and designed to work on any operating system where Python is installed (Windows, macOS, Linux, etc).
 
-## Short description:
-This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. This script should work on any OS where Python is installed (Windows, MacOS and Linux etc).
+## Long Description
+This script utilizes the Plex Python API and sets all movies and shows in your local Plex library to English non-forced subtitles by default. The subtitle preferences will be applied to your Plex profile and remembered on other devices. By default, Plex prefers forced subtitles when available for a given item. However, Plex does not natively allow you to prefer non-forced subtitles, which is why this script was created.
 
-## Long description:
-This script was created with the help of [ChatGPT Open AI](https://chat.openai.com/chat) and further edited and completed by me. It uses [Plex Python Api](https://python-plexapi.readthedocs.io/en/latest/). It will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. Assuming your Plex subtitles settings are setup in your server settings Plex will default to Forced Subtitles by default when they are available for a given item. Plex will not allow you to prefer non forced subtitles natively hence why this script was created.
-
-This script is confirmed tested and working. Feel free to use this code for your own purposes. I will be running this code periodically on my home server along with some of my other neat little plex scripts like [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Thanks to [all](https://stackoverflow.com/questions/75027919/python-script-to-set-all-subtitles-for-movies-shows-in-plex-to-english-non-for) who helped! If you use this script and run into any bugs feel free to open an issue. Cheers!
+The script has been thoroughly tested and confirmed to be working. Feel free to use the code for your own purposes. I will be running this code periodically on my home server along with some other Plex scripts, such as [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Special thanks to everyone who provided assistance! If you encounter any bugs while using this script, please open an issue. Cheers!
 
 ## What are "non-forced" subtitles?
 Non-forced subtitles provide subtitles everytime a characters speaks.
 
 ## What are "forced" subtitles?
 Forced subtitles only provide subtitles when the characters speak a foreign or alien language.
 
-
-## Install Instructions:
-1. Install [Python](https://www.python.org/downloads/).
-2. Run `python -m pip install PlexPreferNonForcedSubs` in command line.
-3. Make sure Plex media server is running then run the script using `PlexPreferNonForcedSubs` in command line.
-4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
+## Installation Instructions
+1. Install [Python](https://www.python.org/downloads/) (v3.5 or later).
+2. Install the script by executing the following in the command line: `python -m pip install PlexPreferNonForcedSubs`.
+3. Ensure that your Plex media server is running, then run the script using `PlexPreferNonForcedSubs` in the command line.
+4. On the first run, the script will prompt you to enter your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). The token will be saved locally in the same folder as `token.txt`.
+5. Done, setup complete. The script will continue to run and set all movies and shows in your local Plex library to use English non-forced subtitles.
+
+See the section below for instructions on how to run, update, and uninstall the script.
+
+## Installing the Script:
+```
+python -m pip install PlexPreferNonForcedSubs
+```
+_Execute in your operating system's native command line._
+## Running the Script:
+```
+PlexPreferNonForcedSubs
+```
+_Execute in your operating system's native command line._
+## Updating the Script:
+```
+python -m pip install PlexPreferNonForcedSubs --upgrade
+```
+_Execute in your operating system's native command line._
+## Uninstalling the Script:
+```
+python -m pip uninstall PlexPreferNonForcedSubs
+```
+_Execute in your operating system's native command line._
+
+## Installing a Specific Version:
+```
+python -m pip install PlexPreferNonForcedSubs==VERSION_NUMBER
+```
+_Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) (e.g. 2.1.4) and execute in your operating system's native command line._
+
+## Alternative Manual Installation Method (without pip install):
+1. Install [Python](https://www.python.org/downloads/) (v3.5 or later).
+2. Download the latest `.py` script from the [releases page](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) and move it to the desired directory.
+3. Execute the script by running `PlexPreferNonForcedSubs.py`, or open the terminal and navigate to the folder where `PlexPreferNonForcedSubs.py` is located, then run `PlexPreferNonForcedSubs.py` in the terminal.
+4. On the first run, the script will prompt you to enter your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). The token will be saved locally in the same folder as `token.txt`.
 5. Done.
 
-_See [below](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
+See the section above for instructions on how to run, update, and uninstall the script.
 
-### Run:
-`PlexPreferNonForcedSubs` in command line.
+## Known Issues/Future Outlook
+- Some lines of redundant code can be shortened and/or removed. Refer to [this issue](https://github.com/RileyXX/PlexPreferNonForcedSubs/issues/4) for more details.
 
-### Update:
-`python -m pip install PlexPreferNonForcedSubs --upgrade` in command line.
-### Uninstall:
-`python -m pip uninstall PlexPreferNonForcedSubs` in command line.
-
-## Alternative manual no install method:
-1. Download the latest .py script from the [releases page](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) and move it to the file directory of your choice.
-2. Run the script by running `PlexPreferNonForcedSubs.py` OR open terminal and navigate to folder where `PlexPreferNonForcedSubs.py` is located. Run `PlexPreferNonForcedSubs.py` in terminal. 
-4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
-3. Done.
-
-_See [above](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
-
-## Known issues/future outlook:
-* Several lines of redundant code can be shortened and/or removed
-
-## Also posted on:
-* [Stackoverflow](https://stackoverflow.com/q/75027919/9196825)
-* [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
-* [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
+## Also Posted On
+- [PyPi](https://pypi.org/project/PlexPreferNonForcedSubs/)
+- [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
+- [Stack Overflow](https://stackoverflow.com/q/75027919/9196825)
+- [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
 
 ## Screenshots:
 ##### Plex subtitle dropdown after script is done running:
 ![Plex Subtitle Dropdown](https://i.imgur.com/BNOlwtL.png)
 ##### PlexPreferNonForcedSubs.py script in action:
 ![PlexPreferNonForcedSubs.py Script in Action](https://github.com/RileyXX/PlexPreferNonForcedSubs/raw/main/demo.gif)
 
-## Sponsorships, Donations and Custom Projects:
-Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
+## Sponsorships, Donations, and Custom Projects
+If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
 
-#### More donation options:
+#### More Donation Options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
-<br>
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
```

### Comparing `PlexPreferNonForcedSubs-2.1.4/setup.py` & `PlexPreferNonForcedSubs-2.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.1.4'
+VERSION = '2.1.5'
 DESCRIPTION = 'This script will set all movies and shows in your local Plex library to English non forced subtitles by default.'
 LONG_DESCRIPTION = 'This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices.'
 
 # Setting up
 setup(
     name="PlexPreferNonForcedSubs",
     version=VERSION,
@@ -31,9 +31,10 @@
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
             'PlexPreferNonForcedSubs = PlexPreferNonForcedSubs.PlexPreferNonForcedSubs:main'
         ]
-    }
+    },
+    python_requires='>=3.6'
 )
```

