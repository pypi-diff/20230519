# Comparing `tmp/musiccli-1.1.1.tar.gz` & `tmp/musiccli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musiccli-1.1.1.tar", last modified: Tue May 16 11:44:32 2023, max compression
+gzip compressed data, was "musiccli-1.2.0.tar", last modified: Fri May 19 18:25:37 2023, max compression
```

## Comparing `musiccli-1.1.1.tar` & `musiccli-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 otabekswe   (501) staff       (20)        0 2023-05-16 11:44:32.112630 musiccli-1.1.1/
--rw-r--r--   0 otabekswe   (501) staff       (20)     1072 2023-05-16 09:31:11.000000 musiccli-1.1.1/LICENSE.txt
--rw-r--r--   0 otabekswe   (501) staff       (20)       25 2023-05-16 09:28:57.000000 musiccli-1.1.1/MANIFEST.in
--rw-r--r--   0 otabekswe   (501) staff       (20)     1126 2023-05-16 11:44:32.112511 musiccli-1.1.1/PKG-INFO
--rw-r--r--   0 otabekswe   (501) staff       (20)      527 2023-05-16 11:42:26.000000 musiccli-1.1.1/README.md
--rw-r--r--   0 otabekswe   (501) staff       (20)      955 2023-05-16 11:39:22.000000 musiccli-1.1.1/pyproject.toml
--rw-r--r--   0 otabekswe   (501) staff       (20)       38 2023-05-16 11:44:32.112665 musiccli-1.1.1/setup.cfg
-drwxr-xr-x   0 otabekswe   (501) staff       (20)        0 2023-05-16 11:44:32.110046 musiccli-1.1.1/src/
-drwxr-xr-x   0 otabekswe   (501) staff       (20)        0 2023-05-16 11:44:32.111546 musiccli-1.1.1/src/musiccli/
--rw-r--r--   0 otabekswe   (501) staff       (20)       43 2023-05-16 09:05:32.000000 musiccli-1.1.1/src/musiccli/__init__.py
--rw-r--r--   0 otabekswe   (501) staff       (20)       82 2023-05-16 09:52:32.000000 musiccli-1.1.1/src/musiccli/__main__.py
--rw-r--r--   0 otabekswe   (501) staff       (20)     1790 2023-05-15 19:15:53.000000 musiccli-1.1.1/src/musiccli/crawler.py
--rw-r--r--   0 otabekswe   (501) staff       (20)     1783 2023-05-16 09:53:10.000000 musiccli-1.1.1/src/musiccli/main.py
-drwxr-xr-x   0 otabekswe   (501) staff       (20)        0 2023-05-16 11:44:32.112338 musiccli-1.1.1/src/musiccli.egg-info/
--rw-r--r--   0 otabekswe   (501) staff       (20)     1126 2023-05-16 11:44:32.000000 musiccli-1.1.1/src/musiccli.egg-info/PKG-INFO
--rw-r--r--   0 otabekswe   (501) staff       (20)      361 2023-05-16 11:44:32.000000 musiccli-1.1.1/src/musiccli.egg-info/SOURCES.txt
--rw-r--r--   0 otabekswe   (501) staff       (20)        1 2023-05-16 11:44:32.000000 musiccli-1.1.1/src/musiccli.egg-info/dependency_links.txt
--rw-r--r--   0 otabekswe   (501) staff       (20)       52 2023-05-16 11:44:32.000000 musiccli-1.1.1/src/musiccli.egg-info/entry_points.txt
--rw-r--r--   0 otabekswe   (501) staff       (20)       92 2023-05-16 11:44:32.000000 musiccli-1.1.1/src/musiccli.egg-info/requires.txt
--rw-r--r--   0 otabekswe   (501) staff       (20)        9 2023-05-16 11:44:32.000000 musiccli-1.1.1/src/musiccli.egg-info/top_level.txt
+drwxr-xr-x   0 otabekswe   (501) staff       (20)        0 2023-05-19 18:25:37.676660 musiccli-1.2.0/
+-rw-r--r--   0 otabekswe   (501) staff       (20)     1072 2023-05-16 13:59:01.000000 musiccli-1.2.0/LICENSE.txt
+-rw-r--r--   0 otabekswe   (501) staff       (20)       25 2023-05-16 13:59:01.000000 musiccli-1.2.0/MANIFEST.in
+-rw-r--r--   0 otabekswe   (501) staff       (20)     1149 2023-05-19 18:25:37.676545 musiccli-1.2.0/PKG-INFO
+-rw-r--r--   0 otabekswe   (501) staff       (20)      527 2023-05-16 13:59:01.000000 musiccli-1.2.0/README.md
+-rw-r--r--   0 otabekswe   (501) staff       (20)      981 2023-05-19 18:25:28.000000 musiccli-1.2.0/pyproject.toml
+-rw-r--r--   0 otabekswe   (501) staff       (20)       38 2023-05-19 18:25:37.676693 musiccli-1.2.0/setup.cfg
+drwxr-xr-x   0 otabekswe   (501) staff       (20)        0 2023-05-19 18:25:37.674323 musiccli-1.2.0/src/
+drwxr-xr-x   0 otabekswe   (501) staff       (20)        0 2023-05-19 18:25:37.675636 musiccli-1.2.0/src/musiccli/
+-rw-r--r--   0 otabekswe   (501) staff       (20)       43 2023-05-16 13:59:01.000000 musiccli-1.2.0/src/musiccli/__init__.py
+-rw-r--r--   0 otabekswe   (501) staff       (20)      103 2023-05-19 18:02:51.000000 musiccli-1.2.0/src/musiccli/__main__.py
+-rw-r--r--   0 otabekswe   (501) staff       (20)     3168 2023-05-19 18:23:49.000000 musiccli-1.2.0/src/musiccli/crawler.py
+-rw-r--r--   0 otabekswe   (501) staff       (20)     1725 2023-05-19 18:23:49.000000 musiccli-1.2.0/src/musiccli/main.py
+drwxr-xr-x   0 otabekswe   (501) staff       (20)        0 2023-05-19 18:25:37.676378 musiccli-1.2.0/src/musiccli.egg-info/
+-rw-r--r--   0 otabekswe   (501) staff       (20)     1149 2023-05-19 18:25:37.000000 musiccli-1.2.0/src/musiccli.egg-info/PKG-INFO
+-rw-r--r--   0 otabekswe   (501) staff       (20)      361 2023-05-19 18:25:37.000000 musiccli-1.2.0/src/musiccli.egg-info/SOURCES.txt
+-rw-r--r--   0 otabekswe   (501) staff       (20)        1 2023-05-19 18:25:37.000000 musiccli-1.2.0/src/musiccli.egg-info/dependency_links.txt
+-rw-r--r--   0 otabekswe   (501) staff       (20)       52 2023-05-19 18:25:37.000000 musiccli-1.2.0/src/musiccli.egg-info/entry_points.txt
+-rw-r--r--   0 otabekswe   (501) staff       (20)       92 2023-05-19 18:25:37.000000 musiccli-1.2.0/src/musiccli.egg-info/requires.txt
+-rw-r--r--   0 otabekswe   (501) staff       (20)        9 2023-05-19 18:25:37.000000 musiccli-1.2.0/src/musiccli.egg-info/top_level.txt
```

### Comparing `musiccli-1.1.1/LICENSE.txt` & `musiccli-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `musiccli-1.1.1/PKG-INFO` & `musiccli-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: musiccli
-Version: 1.1.1
+Version: 1.2.0
 Summary: MusicCLI is a user-friendly command-line interface that lets you download your favorite music directly from your terminal to Desktop.
 Author-email: Otabek Nurmatov <mrotabek17@gmail.com>
 Project-URL: Homepage, https://github.com/otabeknurmatov/MusicCLI
-Keywords: MusicCLI,climusic,mcli
+Keywords: MusicCLI,mcli,Music Downloader,Terminal Music
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `musiccli-1.1.1/README.md` & `musiccli-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `musiccli-1.1.1/pyproject.toml` & `musiccli-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "musiccli"
-version = "1.1.1"
+version = "1.2.0"
 description = "MusicCLI is a user-friendly command-line interface that lets you download your favorite music directly from your terminal to Desktop."
 readme = "README.md"
 authors = [{ name = "Otabek Nurmatov", email = "mrotabek17@gmail.com"  }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["MusicCLI", "climusic", "mcli"]
+keywords = ["MusicCLI", "mcli", "Music Downloader", "Terminal Music"]
 dependencies = [
     "requests >= 2.28.2",
     "bs4 >= 0.0.1",
     "lxml",
     'beautifulsoup4 >= 4.12.2',
 ]
 requires-python = ">=3.8"
```

### Comparing `musiccli-1.1.1/src/musiccli/main.py` & `musiccli-1.2.0/src/musiccli/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,53 @@
-import os
 from argparse import ArgumentParser
 
-import requests
-from .crawler import search, _download_link
+from .crawler import get_list, print_list, download_request, download
 
 
-download_path = os.path.join(os.environ['USERPROFILE'], 'Desktop') if os.name == 'nt' else os.path.join(os.path.expanduser('~'), 'Desktop')
+async def runner(song_name: str) -> None:
+    songs = await get_list(" ".join(song_name))
 
+    if songs is None:
+        print("Found nothing : (")
+        return
+    else:
+        print_list(songs)
+        print("Choose a number from the list to download the corresponding music.")
 
-def run_main() -> None:
+    while True:
+        num = int(input("Number: ")) - 1
+
+        if num < 0:
+            print("Invalid number, please give valid number from the list!")
+            continue
+
+        try:
+            song = songs[num]
+        except IndexError:
+            print("Invalid number, please give valid number from the list!")
+            continue
+        else:
+            byte_code = await download_request(song['link'])
+            download(song["song"], byte_code)
+            return
+
+
+async def main():
     desc = "MusicCLI is a command-line interface application that allows users to search and download music from a " \
-           "variety of online sources. With MusicCLI, users can easily find and download their favorite songs to their"\
+           "variety of online sources. With MusicCLI, users can easily find and download their favorite songs to their" \
            " Desktop folder."
-    epilog = "If you find this project useful, we would greatly appreciate it if you could take a moment to give it a "\
-             "star on GitHub. Your support helps us to continue improving the project and providing useful tools for "\
+    epilog = "If you find this project useful, we would greatly appreciate it if you could take a moment to give it a " \
+             "star on GitHub. Your support helps us to continue improving the project and providing useful tools for " \
              "the community. Thank you for your consideration!😉"
     parser = ArgumentParser(prog="MusicCLI", description=desc, usage="mcli [SONG]", epilog=epilog)
     parser.add_argument('song', type=str, nargs='*', help='Name of the song')
     args = parser.parse_args()
-    # For searching
-    num = 1
-    song_list = search(args.song)
-
-    for i in song_list:
-        name = f"{num}.{i['artist']} - {i['song']}"
-        print(name)
-        num += 1
 
-    while True:
-        number = int(input("Choose a number from the list to download the corresponding music: ")) - 1
-        if number <= 0 or number > len(song_list):
-            print("You choose wrong number, please do it again!")
-            continue
-        else:
-            break
-    choosen_song = song_list[number]
-    with open(f"{download_path}/{choosen_song['artist']} - {choosen_song['song']}.mp3", 'wb') as music:
-        music.write(requests.get(_download_link(song_list[number]['link'])).content)
+    await runner(args.song)
+
+
+
+
+
+
 
-    print("All done!")
```

### Comparing `musiccli-1.1.1/src/musiccli.egg-info/PKG-INFO` & `musiccli-1.2.0/src/musiccli.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: musiccli
-Version: 1.1.1
+Version: 1.2.0
 Summary: MusicCLI is a user-friendly command-line interface that lets you download your favorite music directly from your terminal to Desktop.
 Author-email: Otabek Nurmatov <mrotabek17@gmail.com>
 Project-URL: Homepage, https://github.com/otabeknurmatov/MusicCLI
-Keywords: MusicCLI,climusic,mcli
+Keywords: MusicCLI,mcli,Music Downloader,Terminal Music
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

