# Comparing `tmp/nsdotpy-1.2.8.tar.gz` & `tmp/nsdotpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.2.8.tar", max compression
+gzip compressed data, was "nsdotpy-1.3.0.tar", max compression
```

## Comparing `nsdotpy-1.2.8.tar` & `nsdotpy-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-12 03:19:53.212307 nsdotpy-1.2.8/LICENSE.md
--rw-r--r--   0        0        0     2436 2023-05-12 03:19:53.212307 nsdotpy-1.2.8/README.md
--rw-r--r--   0        0        0      790 2023-05-12 03:19:53.224307 nsdotpy-1.2.8/nsdotpy/__init__.py
--rw-r--r--   0        0        0    41448 2023-05-12 03:19:53.224307 nsdotpy-1.2.8/nsdotpy/session.py
--rw-r--r--   0        0        0     4963 2023-05-12 03:19:53.224307 nsdotpy-1.2.8/nsdotpy/valid.py
--rw-r--r--   0        0        0      703 2023-05-12 03:19:53.224307 nsdotpy-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 nsdotpy-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-05-19 00:19:03.509539 nsdotpy-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2440 2023-05-19 00:19:03.509539 nsdotpy-1.3.0/README.md
+-rw-r--r--   0        0        0      790 2023-05-19 00:19:03.521539 nsdotpy-1.3.0/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    44794 2023-05-19 00:19:03.521539 nsdotpy-1.3.0/nsdotpy/session.py
+-rw-r--r--   0        0        0     4963 2023-05-19 00:19:03.521539 nsdotpy-1.3.0/nsdotpy/valid.py
+-rw-r--r--   0        0        0      719 2023-05-19 00:19:03.521539 nsdotpy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nsdotpy-1.3.0/PKG-INFO
```

### Comparing `nsdotpy-1.2.8/LICENSE.md` & `nsdotpy-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.8/README.md` & `nsdotpy-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 - Dossier and reports handling
 - More fleshed out API Client
 - ~~Cards support~~ Shoutouts to 9003
 - ~~Migrate automatic docs generation, code formatting, and PyPI uploading to GitHub Actions for better CI~~
 
 ## Docs
 
-https://sw33ze.github.io/NSDotPy/nsdotpy/session.html#NSSession
+https://audreyreal.github.io/NSDotPy/nsdotpy/session.html#NSSession
 
 ## Generating Docs
 
 1. [Ensure poetry is installed](https://python-poetry.org/docs/#installation), or your system's package manager if applicable.
 2. Run `poetry install` in the root directory of the project to install dependencies if you haven't already.
 3. Run `poetry run pdoc nsdotpy/session.py -d=google -o=docs/` to generate the docs
```

### Comparing `nsdotpy-1.2.8/nsdotpy/__init__.py` & `nsdotpy-1.3.0/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.8/nsdotpy/session.py` & `nsdotpy-1.3.0/nsdotpy/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import logging.config  # for logging configuration
 import mimetypes  # for flag and banner uploading
 
 # external library imports
 import keyboard  # for the required user input
 import httpx  # for http stuff
 from tendo.singleton import SingleInstance  # so it can only be run once at a time
-from bs4 import BeautifulSoup  # for parsing html and xml
+from bs4 import BeautifulSoup, Tag  # for parsing html and xml
 
 # local imports
 from . import valid  # for valid region tags
 
 
 def canonicalize(string: str) -> str:
     """Converts a string to its canonical form used by the nationstates api.
@@ -62,15 +62,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.2.8"
+        self.VERSION = "1.3.0"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -80,16 +80,21 @@
         # Set the user agent to the script name, version, author, and user as recommended in the script rules thread:
         # https://forum.nationstates.net/viewtopic.php?p=16394966&sid=be37623536dbc8cee42d8d043945b887#p16394966
         self._lock: bool = False
         self._set_user_agent(
             script_name, script_version, script_author, script_user, link_to_src
         )
         # If a link to the source code is provided, add it to the user agent
-        # Initialize nationstates specific stuff
         self._ns_server = "1"
+        # Make sure the nations in the user agent actually exist
+        if not self._validate_nations([script_author, script_user]):
+            raise ValueError(
+                "One of, or both, of the nations in the user agent do not exist. Make sure you're only including the nation name in the constructor, e.g. 'Thorn1000' instead of 'Devved by Thorn1000'"
+            )
+        # Initialize nationstates specific stuff
         self._auth_region = "rwby"
         self.chk: str = ""
         self.localid: str = ""
         self.pin: str = ""
         self.nation: str = ""
         self.region: str = ""
         self.current_page: tuple[str, str] = ("", "")
@@ -108,14 +113,34 @@
             f"{script_name}/{script_version} (by:{script_author}; usedBy:{script_user})"
         )
         if link_to_src:
             self.user_agent = f"{self.user_agent}; src:{link_to_src}"
         self.user_agent = f"{self.user_agent}; Written with NSDotPy/{self.VERSION} (by:Sweeze; src:github.com/sw33ze/NSDotPy)"
         self._session.headers.update({"User-Agent": self.user_agent})
 
+    def _validate_nations(self, nations: list[str]) -> bool:
+        """Checks if a list of nations exist using the NationStates API.
+
+        Args:
+            nations (list[str]): List of nations to check
+
+        Returns:
+            bool: True if all nations in the list exist, False otherwise.
+        """
+        url = "https://www.nationstates.net/cgi-bin/api.cgi"
+        data = {"q": "nations"}
+        response = self.request(url, data)
+        soup = BeautifulSoup(response.text, "lxml-xml")
+        # the list of nations is inside the <NATIONS> tag
+        world_nations_tag: Tag = soup.find("NATIONS")  # type: ignore
+        # get the list of nations from the <NATIONS> tag
+        world_nations: list[str] = world_nations_tag.text.split(",")
+        # check if all nations in the list exist in the world nations
+        return all(canonicalize(nation) in world_nations for nation in nations)
+
     def _init_logger(self):
         self.logger = logging.getLogger("NSDotPy")
         config = {
             "version": 1,
             "disable_existing_loggers": False,
             "formatters": {
                 "f": {
@@ -137,29 +162,30 @@
         logging.config.dictConfig(config)
 
     def _get_auth_values(self, response: httpx.Response):
         # make sure it's actually html first
         if not response.headers["Content-Type"].startswith("text/html"):
             return
         # parse the html
-        soup = BeautifulSoup(response.text, "html.parser")
+        soup = BeautifulSoup(response.text, "lxml")
         # gathering chk and localid so i dont have to worry about authenticating l8r
         if chk := soup.find("input", {"name": "chk"}):
             self.chk = chk["value"].strip()  # type: ignore
         if localid := soup.find("input", {"name": "localid"}):
             self.localid = localid["value"].strip()  # type: ignore
         if pin := self._session.cookies.get("pin"):
             # you should never really need the pin but just in case i'll store it
             self.pin = pin
         if soup.find("a", {"class": "STANDOUT"}):
             self.region = canonicalize(
                 soup.find_all("a", {"class": "STANDOUT"})[1].attrs["href"].split("=")[1]
             )
 
     def _refresh_auth_values(self):
+        self.logger.info("Refreshing authentication values...")
         response = self.request(
             f"https://www.nationstates.net/page=display_region/region={self._auth_region}",
             data={"theme": "century"},
         )
         self._get_auth_values(response)
 
     def _wait_for_input(self, key: str) -> int:
@@ -182,15 +208,15 @@
 
         Returns:
             str: The detagged WFE"""
         self.logger.info(f"Getting detagged WFE for {self.region}...")
         response = self.request(
             f"https://greywardens.xyz/tools/wfe_index/region={self.region}",
         )
-        soup = BeautifulSoup(response.text, "html.parser")
+        soup = BeautifulSoup(response.text, "lxml")
         # the safest bet for a detag wfe is the first wfe of the region
         return soup.find_all("pre")[-1].text
 
     def _validate_fields(self, data: dict):
         max_lengths = {
             "pretitle": 28,
             "slogan": 55,
@@ -365,15 +391,15 @@
             "theme": "century",
             "logging_in": "1",
             "submit": "Login",
         }
 
         response = self.request(url, data)
 
-        soup = BeautifulSoup(response.text, "html.parser")
+        soup = BeautifulSoup(response.text, "lxml")
         # checks if the body tag has your nation name in it; if it does, you're logged in
         if not soup.find("body", {"data-nname": canonicalize(nation)}):
             return False
 
         self.nation = canonicalize(nation)
         return True
 
@@ -426,15 +452,15 @@
         new_password: str = "",
     ) -> bool:
         """Given a logged in session, changes customizable fields and settings of the logged in nation.
         Variables must be explicitly named in the call to the function, e.g. "session.change_nation_settings(pretitle='Join Lily', currency='Join Lily')"
 
         Args:
             email (str, optional): New email for WA apps.
-            pretitle (str, optional): New pretitle of the nation. Max length of 28.
+            pretitle (str, optional): New pretitle of the nation. Max length of 28. Nation must have minimum population of 250 million.
             slogan (str, optional): New Slogan/Motto of the nation. Max length of 55.
             currency (str, optional): New currency of the nation. Max length of 40.
             animal (str, optional): New national animal of the nation. Max length of 40.
             demonym_noun (str, optional): Noun the nation will refer to its citizens as. Max length of 44.
             demonym_adjective (str, optional): Adjective the nation will refer to its citizens as. Max length of 44.
             demonym_plural (str, optional): Plural form of "demonym_noun". Max length of 44.
             new_password (str, optional): New password to assign to the nation.
@@ -602,14 +628,38 @@
         self.logger.info(f"Clearing dossier on {self.nation}")
         url = "https://www.nationstates.net/template-overall=none/page=dossier"
         data = {"clear_dossier": "1"}
         response = self.request(url, data)
 
         return "Dossier cleared of nations." in response.text
 
+    def add_to_dossier(self, nations: list[str]) -> bool:
+        """Adds nations to the logged in nation's dossier.
+
+        Args:
+            nations (list[str]): List of nations to add
+
+        Returns:
+            bool: Whether it was successful or not
+        """
+
+        self.logger.info(f"Adding {nations} to dossier on {self.nation}")
+        url = "https://www.nationstates.net/template-overall=none/page=dossier"
+        data = {
+            "currentnation": canonicalize(self.nation),
+            "action_append": "Upload Nation Dossier File",
+        }
+        files = {
+            "file": ("dossier.txt", "\n".join(nations), "text/plain"),
+        }
+        response = self.request(url, data, files=files)
+
+        self._refresh_auth_values()
+        return "appended=1" in response.headers["location"]
+
     def wa_vote(self, council: str, vote: str) -> bool:
         """Votes on the current WA resolution.
 
         Args:
             council (str): Must be "ga" for general assembly, "sc" for security council.
             vote (str): Must be "for" or "against".
 
@@ -856,14 +906,44 @@
         data = {
             f"{action}_tag": canonicalize(tag),
             "updatetagsbutton": "1",
         }
         response = self.request(url, data)
         return "Region Tags updated!" in response.text
 
+    def eject(self, nation: str) -> bool:
+        """Ejects a nation from the current region.
+
+        Args:
+            nation (str): The nation to eject.
+
+        Returns:
+            bool: Whether the nation was successfully ejected or not
+        """
+        self.logger.info(f"Ejecting {nation} from {self.region}")
+        url = "https://www.nationstates.net/template-overall=none/page=region_control/"
+        data = {"nation_name": nation, "eject": "1"}
+        response = self.request(url, data)
+        return "has been ejected from " in response.text
+
+    def banject(self, nation: str) -> bool:
+        """Bans a nation from the current region.
+
+        Args:
+            nation (str): The nation to banject.
+
+        Returns:
+            bool: Whether the nation was successfully banjected or not
+        """
+        self.logger.info(f"Banjecting {nation} from {self.region}")
+        url = "https://www.nationstates.net/template-overall=none/page=region_control/"
+        data = {"nation_name": nation, "ban": "1"}
+        response = self.request(url, data)
+        return "has been ejected and banned from " in response.text
+
     # end methods for region control
 
     def junk_card(self, id: str, season: str) -> bool:
         """Junks a card from the current nation's deck.
         Args:
             id (str): ID of the card to junk
             season (str): Season of the card to junk
```

### Comparing `nsdotpy-1.2.8/nsdotpy/valid.py` & `nsdotpy-1.3.0/nsdotpy/valid.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.8/pyproject.toml` & `nsdotpy-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.2.8"
+version = "1.3.0"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 httpx = { extras = ["http2"], version = "^0.24.0" }
 beautifulsoup4 = "^4.12.2"
 keyboard = "^0.13.5"
 tendo = "^0.3.0"
+lxml = "^4.9.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pdoc = "^13.1.1"
 pyinstaller = "^5.10.1"
 
 [build-system]
```

### Comparing `nsdotpy-1.2.8/PKG-INFO` & `nsdotpy-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.2.8
+Version: 1.3.0
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
 Requires-Dist: keyboard (>=0.13.5,<0.14.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: tendo (>=0.3.0,<0.4.0)
 Project-URL: Repository, https://github.com/sw33ze/NSDotPy
 Description-Content-Type: text/markdown
 
 # NSDotPy
 
 A Python wrapper around httpx for legally interacting with the HTML NationStates site, as well as a barebones API client. Built for legality first and foremost, as well as ease of use.
@@ -43,15 +44,15 @@
 - Dossier and reports handling
 - More fleshed out API Client
 - ~~Cards support~~ Shoutouts to 9003
 - ~~Migrate automatic docs generation, code formatting, and PyPI uploading to GitHub Actions for better CI~~
 
 ## Docs
 
-https://sw33ze.github.io/NSDotPy/nsdotpy/session.html#NSSession
+https://audreyreal.github.io/NSDotPy/nsdotpy/session.html#NSSession
 
 ## Generating Docs
 
 1. [Ensure poetry is installed](https://python-poetry.org/docs/#installation), or your system's package manager if applicable.
 2. Run `poetry install` in the root directory of the project to install dependencies if you haven't already.
 3. Run `poetry run pdoc nsdotpy/session.py -d=google -o=docs/` to generate the docs
```

