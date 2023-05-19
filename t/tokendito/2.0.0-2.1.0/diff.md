# Comparing `tmp/tokendito-2.0.0.tar.gz` & `tmp/tokendito-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokendito-2.0.0.tar", last modified: Wed Jan 18 16:32:57 2023, max compression
+gzip compressed data, was "tokendito-2.1.0.tar", last modified: Fri May 19 19:24:25 2023, max compression
```

## Comparing `tokendito-2.0.0.tar` & `tokendito-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 16:32:57.092259 tokendito-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-18 16:32:44.000000 tokendito-2.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-01-18 16:32:44.000000 tokendito-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-18 16:32:44.000000 tokendito-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-01-18 16:32:57.092259 tokendito-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-01-18 16:32:44.000000 tokendito-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-18 16:32:44.000000 tokendito-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-18 16:32:44.000000 tokendito-2.0.0/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-01-18 16:32:44.000000 tokendito-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 16:32:57.092259 tokendito-2.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2213 2023-01-18 16:32:44.000000 tokendito-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 16:32:57.092259 tokendito-2.0.0/tokendito/
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-01-18 16:32:44.000000 tokendito-2.0.0/tokendito/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-01-18 16:32:44.000000 tokendito-2.0.0/tokendito/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-01-18 16:32:44.000000 tokendito-2.0.0/tokendito/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-01-18 16:32:44.000000 tokendito-2.0.0/tokendito/duo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-01-18 16:32:44.000000 tokendito-2.0.0/tokendito/okta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-01-18 16:32:44.000000 tokendito-2.0.0/tokendito/tokendito.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-01-18 16:32:44.000000 tokendito-2.0.0/tokendito/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    40744 2023-01-18 16:32:44.000000 tokendito-2.0.0/tokendito/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 16:32:57.092259 tokendito-2.0.0/tokendito.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-01-18 16:32:57.000000 tokendito-2.0.0/tokendito.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-18 16:32:57.000000 tokendito-2.0.0/tokendito.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 16:32:57.000000 tokendito-2.0.0/tokendito.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-18 16:32:57.000000 tokendito-2.0.0/tokendito.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 16:32:57.000000 tokendito-2.0.0/tokendito.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-18 16:32:57.000000 tokendito-2.0.0/tokendito.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-18 16:32:57.000000 tokendito-2.0.0/tokendito.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:25.433522 tokendito-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-19 19:24:15.000000 tokendito-2.1.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-19 19:24:15.000000 tokendito-2.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-19 19:24:15.000000 tokendito-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-19 19:24:25.429522 tokendito-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-19 19:24:15.000000 tokendito-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-19 19:24:15.000000 tokendito-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-19 19:24:15.000000 tokendito-2.1.0/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-05-19 19:24:15.000000 tokendito-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 19:24:25.433522 tokendito-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2213 2023-05-19 19:24:15.000000 tokendito-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:25.429522 tokendito-2.1.0/tokendito/
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/duo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/okta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/tokendito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:25.429522 tokendito-2.1.0/tokendito.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/top_level.txt
```

### Comparing `tokendito-2.0.0/LICENSE.txt` & `tokendito-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tokendito-2.0.0/setup.py` & `tokendito-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.0.0/tokendito/__init__.py` & `tokendito-2.1.0/tokendito/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,36 +4,41 @@
 import json
 import os
 from os.path import expanduser
 import sys
 
 from platformdirs import user_config_dir
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 __title__ = "tokendito"
 __description__ = "Get AWS STS tokens from Okta SSO"
 __long_description_content_type__ = "text/markdown"
 __url__ = "https://github.com/dowjones/tokendito"
 __author__ = "tokendito"
 __author_email__ = "tokendito@dowjones.com"
 __license__ = "Apache 2.0"
 
 
 class Config(object):
     """Creates configuration variables for the application."""
 
+    _default_encoding = "utf-8"
+    if hasattr(sys, "stdin") and getattr(sys, "stdin") is not None:
+        if getattr(sys.stdin, "encoding") is not None:
+            _default_encoding = sys.stdin.encoding
+
     # Instantiated objects can get Class defaults with get_defaults()
     _defaults = dict(
         user=dict(
             config_dir=user_config_dir(appname=__title__, appauthor=False),
             config_file=os.path.join(
                 user_config_dir(appname=__title__, appauthor=False), f"{__title__}.ini"
             ),
             config_profile="default",
-            encoding=sys.stdin.encoding,
+            encoding=_default_encoding,
             loglevel="INFO",
             log_output_file="",
             mask_items=[],
             quiet=False,
         ),
         aws=dict(
             config_file=os.path.join(expanduser("~"), ".aws", "config"),
@@ -67,15 +72,15 @@
         self.user = dict()
         self.okta = dict()
 
         if kwargs:
             # Argument validation
             self._check_constraints(**kwargs)
             # We create an object that contains only the values passed in.
-            for (key, val) in kwargs.items():
+            for key, val in kwargs.items():
                 self.__dict__[key].update(val)
         else:
             self.set_defaults()
 
     def __repr__(self):
         """Provide a reusable representation of the object."""
         return json.dumps(self.__dict__, sort_keys=True, indent=4)
@@ -85,15 +90,15 @@
         return f"{json.dumps(self.__dict__, sort_keys=True)}"
 
     def __eq__(self, other):
         """Test equality with another object, using the JSON representation."""
         return repr(other) == repr(self)
 
     def update(self, other):
-        """Copy values from another Config object."""
+        """Update values from another Config object."""
         self._check_constraints(**other.__dict__)
         for key in other.__dict__.keys():
             self.__dict__[key].update(other.__dict__[key])
         return self
 
     def _check_constraints(self, **kwargs):
         """Ensure dictionaries that are part of the object are valid.
@@ -101,15 +106,15 @@
         :param self: Implicit reference to object.
         :param kwargs: dictionaries to check.
         :return: boolean on success, or raises an error
         :raises AttributeError: raised if the keyword passed does not exist.
         :raises KeyError: raised if the value passed for a keyword is not a dictionary.
         :raises ValueError: raised if the configuration value does not exist in the object.
         """
-        for (key, val) in kwargs.items():
+        for key, val in kwargs.items():
             # Guard against improper initialization.
             if key not in self._defaults:
                 raise AttributeError(f"'{type(self).__name__}' object has no attribute '{key}'")
             if type(val) is not dict:
                 raise KeyError(f"'{key}' must be a {type(dict())}, not '{type(val)}'")
             for subkey in val.keys():
                 if subkey not in self._defaults[key]:
```

### Comparing `tokendito-2.0.0/tokendito/__main__.py` & `tokendito-2.1.0/tokendito/__main__.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.0.0/tokendito/aws.py` & `tokendito-2.1.0/tokendito/aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 import logging
 import sys
 
 from botocore import UNSIGNED
 from botocore.client import Config
 from botocore.exceptions import ClientError
 import botocore.session
-import requests
+from tokendito import okta
 from tokendito import user
 
-
 logger = logging.getLogger(__name__)
 
 
 def get_regions(profile=None):
     """Get avaliable regions from botocore.
 
     :return: List of available regions.
@@ -43,44 +42,47 @@
 
     Currently, this cannot be done dynamically.
     :return: List of available output types.
     """
     return ["json", "text", "csv", "yaml", "yaml-stream"]
 
 
-def authenticate_to_roles(secret_session_token, urls, cookies=None):
+def authenticate_to_roles(urls, cookies=None):
     """Authenticate AWS user with saml.
 
-    :param secret_session_token: secret session token
     :param urls: list of tuples or tuple, with tiles info
     :param cookies: html cookies
     :return: response text
 
     """
-    payload = {"onetimetoken": secret_session_token}
     url_list = [urls] if isinstance(urls, tuple) else urls
     responses = []
     tile_count = len(url_list)
     plural = ""
     if tile_count > 1:
         plural = "s"
 
     logger.info(f"Discovering roles in {tile_count} tile{plural}.")
     for url, label in url_list:
-        try:
-            logger.debug(f"Performing role discovery in {url}")
+        response = user.request_wrapper("GET", url, cookies=cookies)
+        saml_response_string = response.text
 
-            response = requests.get(url, params=payload, cookies=cookies)
-            response.raise_for_status()
-            saml_response_string = response.text
-        except Exception as err:
-            logger.error(f"There was an error with the call to {url}: {err}")
+        saml_xml = okta.extract_saml_response(saml_response_string)
+        if not saml_xml:
+            if "Extra Verification" in saml_response_string:
+                logger.error("Step-Up Authentication required, but not supported.")
+            elif "App Access Locked" in saml_response_string:
+                logger.error(
+                    "Access to this application is not allowed at this time."
+                    " Please contact your administrator for details."
+                )
+            else:
+                logger.error("Invalid data detected in SAML response. Aborting.")
+            logger.debug(saml_response_string)
             sys.exit(1)
-
-        saml_xml = user.validate_saml_response(saml_response_string)
         responses.append((url, saml_response_string, saml_xml, label))
 
     return responses
 
 
 def assume_role(role_arn, provider_arn, saml):
     """Return AssumeRoleWithSaml API response.
```

### Comparing `tokendito-2.0.0/tokendito/duo.py` & `tokendito-2.1.0/tokendito/duo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # vim: set filetype=python ts=4 sw=4
 # -*- coding: utf-8 -*-
 """This module handles Duo operations."""
 import json
 import logging
 import sys
 import time
-from urllib.parse import unquote, urlparse
+from urllib.parse import unquote
+from urllib.parse import urlparse
 
 from bs4 import BeautifulSoup
 import requests
 from tokendito import config
 from tokendito import user
 
-
 logger = logging.getLogger(__name__)
 
 
 def prepare_duo_info(selected_okta_factor):
     """Aggregate most of the parameters needed throughout the Duo authentication process.
 
     :param selected_okta_factor: dict response describing Duo factor in Okta.
```

### Comparing `tokendito-2.0.0/tokendito/tokendito.py` & `tokendito-2.1.0/tokendito/tokendito.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.0.0/tokendito/tool.py` & `tokendito-2.1.0/tokendito/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import sys
 
 from tokendito import aws
 from tokendito import config
 from tokendito import okta
 from tokendito import user
 
-
 logger = logging.getLogger(__name__)
 
 
 def cli(args):
     """Tokendito retrieves AWS credentials after authenticating with Okta."""
     args = user.parse_cli_args(args)
 
@@ -34,40 +33,36 @@
             quiet_msg = " to run in quiet mode"
         logger.error(
             f"Could not validate configuration{quiet_msg}: {'. '.join(message)}. "
             "Please check your settings, and try again."
         )
         sys.exit(1)
 
-    # Authenticate okta and AWS also use assumerole to assign the role
-    session_token = okta.authenticate_user(config)
-
-    session_cookies = None
+    # Authenticate to okta
+    session_cookies = okta.authenticate(config)
 
     if config.okta["tile"]:
         tile_label = ""
         config.okta["tile"] = (config.okta["tile"], tile_label)
     else:
-        session_cookies = user.request_cookies(config.okta["org"], session_token)
-        config.okta["tile"] = user.discover_tile(config.okta["org"], session_cookies)
+        config.okta["tile"] = user.discover_tiles(config.okta["org"], session_cookies)
 
-    auth_tiles = aws.authenticate_to_roles(
-        session_token, config.okta["tile"], cookies=session_cookies
-    )
+    # Authenticate to AWS roles
+    auth_tiles = aws.authenticate_to_roles(config.okta["tile"], cookies=session_cookies)
 
     (role_response, role_name) = aws.select_assumeable_role(auth_tiles)
 
     identity = aws.assert_credentials(role_response=role_response)
     if "Arn" not in identity and "UserId" not in identity:
         logger.error(
             f"There was an error retrieving and verifying AWS credentials: {role_response}"
         )
         sys.exit(1)
 
-    user.set_role_name(config, role_name)
+    user.set_profile_name(config, role_name)
 
     user.set_local_credentials(
         response=role_response,
         role=config.aws["profile"],
         region=config.aws["region"],
         output=config.aws["output"],
     )
```

### Comparing `tokendito-2.0.0/tokendito/user.py` & `tokendito-2.1.0/tokendito/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,21 +68,21 @@
         action="store_true",
         help="Prompt user for configuration parameters",
     )
     parser.add_argument(
         "--username",
         dest="okta_username",
         help="username to log in to Okta. You can "
-        "also use the OKTA_USERNAME environment variable.",
+        "also use the TOKENDITO_OKTA_USERNAME environment variable.",
     )
     parser.add_argument(
         "--password",
         dest="okta_password",
         help="password to log in to Okta. You "
-        "can also use the OKTA_PASSWORD environment variable.",
+        "can also use the TOKENDITO_OKTA_PASSWORD environment variable.",
     )
     parser.add_argument(
         "--profile",
         dest="user_config_profile",
         default=config.user["config_profile"],
         help="Tokendito configuration profile to use.",
     )
@@ -164,19 +164,17 @@
     return local_time
 
 
 def create_directory(dir_name):
     """Create directories on the local machine."""
     if os.path.isdir(dir_name) is False:
         try:
-            os.mkdir(dir_name)
+            os.makedirs(dir_name, exist_ok=True)
         except OSError as error:
-            logger.error(
-                f"Cannot continue creating directory: {config.user['config_dir']}: {error.strerror}"
-            )
+            logger.error(f"Cannot continue creating directory: {dir_name}: {error.strerror}")
             sys.exit(1)
 
 
 def get_submodule_names():
     """Inspect the current module and find any submodules.
 
     :return: List of submodule names
@@ -355,15 +353,15 @@
     print("\nSelect your preferred MFA method and press Enter:")
 
     longest_index = len(str(len(mfa_options)))
     longest_factor_name = max([len(d[factor_key]) for d in mfa_options])
     longest_subfactor_name = max([len(d[subfactor_key]) for d in mfa_options])
     factor_info_indent = max([len(mfa_option_info(d)) for d in mfa_options])
 
-    for (i, mfa_option) in enumerate(mfa_options):
+    for i, mfa_option in enumerate(mfa_options):
         factor_id = mfa_option.get("id", "Not presented")
         factor_info = mfa_option_info(mfa_option)
         mfa = mfa_option.get(subfactor_key, "Not presented")
         provider = mfa_option.get(factor_key, "Not presented")
         print(
             f"[{i: >{longest_index}}]  "
             f"{provider: <{longest_factor_name}}  "
@@ -471,33 +469,14 @@
     roles_and_providers = {i.split(",")[1]: i.split(",")[0] for i in arns}
 
     logger.debug(f"Collected ARNs: {json.dumps(roles_and_providers)}")
 
     return roles_and_providers
 
 
-def validate_saml_response(html):
-    """Parse html to validate that saml a saml response was returned."""
-    soup = BeautifulSoup(html, "html.parser")
-
-    xml = None
-    for elem in soup.find_all("input", attrs={"name": "SAMLResponse"}):
-        saml_base64 = elem.get("value")
-        xml = codecs.decode(saml_base64.encode("ascii"), "base64").decode("utf-8")
-
-    if xml is None:
-        logger.error(
-            "Invalid data detected in SAML response. View the response with the DEBUG loglevel."
-        )
-        logger.debug(html)
-        sys.exit(1)
-
-    return xml
-
-
 def validate_okta_org(input_url=None):
     """Validate whether a given URL is a valid AWS Org URL in Okta.
 
     :param input_url: string
     :return: bool. True if valid, False otherwise
     """
     logger.debug(f"Will try to match '{input_url}' to a valid URL")
@@ -605,15 +584,15 @@
     res = dict()
     pattern = re.compile(r"^(.*?)_(.*)")
 
     ini = configparser.ConfigParser(default_section=config.user["config_profile"])
     # Here, group(1) is the dictionary key, and group(2) the configuration element
     try:
         ini.read(file)
-        for (key, val) in ini.items(profile):
+        for key, val in ini.items(profile):
             match = re.search(pattern, key.lower())
             if match:
                 if match.group(1) not in res:
                     res[match.group(1)] = dict()
                 res[match.group(1)][match.group(2)] = val
                 add_sensitive_value_to_be_masked(val, match.group(2))
     except configparser.Error as err:
@@ -638,15 +617,15 @@
 
     :param args: argparse object
     :return: Config object with configuration values
     """
     res = dict()
     pattern = re.compile(r"^(.*?)_(.*)")
 
-    for (key, val) in vars(args).items():
+    for key, val in vars(args).items():
         match = re.search(pattern, key.lower())
         if match:
             if match.group(1) not in get_submodule_names():
                 continue
             if match.group(1) not in res:
                 res[match.group(1)] = dict()
             if val:
@@ -671,15 +650,15 @@
 
     :return: Config object with configuration values.
     """
     res = dict()
     pattern = re.compile(rf"^({prefix})_(.*?)_(.*)")
     # Here, group(1) is the prefix variable, group(2) is the dictionary key,
     # and group(3) the configuration element.
-    for (key, val) in os.environ.items():
+    for key, val in os.environ.items():
         match = re.search(pattern, key.lower())
         if match:
             if match.group(2) not in res:
                 res[match.group(2)] = dict()
             if val:
                 res[match.group(2)][match.group(3)] = val
                 add_sensitive_value_to_be_masked(val, match.group(3))
@@ -748,15 +727,14 @@
     :return: dictionary with values
     """
     logger.debug("Obtain user input for the user.")
     details = {}
 
     # We need either one of these two:
     while not validate_okta_org(org) and not validate_okta_tile(tile):
-        print("\n\nPlease enter either your Organization URL, a tile URL, or both.")
         org = get_org()
         tile = get_tile()
 
     while username == "":
         username = get_username()
 
     if org is not None:
@@ -853,32 +831,53 @@
     :param args: command line arguments
     :return: okta_password
 
     """
     res = ""
     logger.debug("Set password.")
 
+    tty_assertion()
     while res == "":
         password = getpass.getpass()
         res = password
         logger.debug("password set interactively")
     return res
 
 
-def set_role_name(config_obj, name):
+def get_interactive_profile_name(default):
+    """Get AWS profile name from user.
+
+    :return: string with sanitized value, or the default string.
+    """
+    message = f"Enter a profile name or leave blank to use '{default}': "
+    res = ""
+
+    while res == "":
+        user_data = get_input(prompt=message)
+        user_data = user_data.strip()
+        if user_data == "":
+            res = default
+            break
+        if re.fullmatch("[a-zA-Z][a-zA-Z0-9_-]*", user_data):
+            res = user_data
+        else:
+            print("Invalid input, try again.")
+    logger.debug(f"Profile name is: {res}")
+    return res
+
+
+def set_profile_name(config_obj, role_name):
     """Set AWS Role alias name based on user preferences.
 
     :param config: Config object.
-    :param name: Role name. Defaults to the string "default"
+    :param role_name: Role name.
     :return: Config object.
     """
-    if name is None or name == "":
-        name = "default"
-    if config_obj.aws["profile"] is None:
-        config_obj.aws["profile"] = str(name)
+    if config_obj.aws["profile"] is None or config_obj.aws["profile"] == "":
+        config_obj.aws["profile"] = get_interactive_profile_name(role_name)
 
     return config_obj
 
 
 def update_configuration(config):
     """Update configuration file on local system.
 
@@ -1017,20 +1016,34 @@
     """
     integer_validation = check_integer(value)
     if integer_validation and valid_range:
         integer_validation = check_within_range(value, valid_range)
     return integer_validation
 
 
+def tty_assertion():
+    """Ensure that a TTY is present."""
+    try:
+        assert os.isatty(sys.stdin.fileno()) is True
+    except (AttributeError, AssertionError, EOFError, OSError, RuntimeError):
+        logger.error(
+            "sys.stdin is not available, and interactive invocation requires stdin to be present. "
+            "Please check the --help argument and documentation for more details.",
+        )
+        sys.exit(1)
+
+
 def get_input(prompt="-> "):
     """Collect user input for TOTP.
 
     :param prompt: optional string with prompt.
     :return user_input: raw from user.
     """
+    tty_assertion()
+
     user_input = input(f"{prompt}")
     logger.debug(f"User input: {user_input}")
 
     return user_input
 
 
 def collect_integer(valid_range=0):
@@ -1161,54 +1174,65 @@
         config.aws["output"] = config.get_defaults()["aws"]["output"]
         logger.warning(f"AWS Output reset to {config.aws['output']}")
 
     if config.aws["region"] not in aws.get_regions():
         config.aws["region"] = config.get_defaults()["aws"]["region"]
         logger.warning(f"AWS Region reset to {config.aws['region']}")
 
+    # Expand any "~", if given by the user
+    if "config_dir" in config.user:
+        config.user["config_dir"] = os.path.expanduser(config.user["config_dir"])
+    if "config_file" in config.user:
+        config.user["config_file"] = os.path.expanduser(config.user["config_file"])
+    if "config_file" in config.aws:
+        config.aws["config_file"] = os.path.expanduser(config.aws["config_file"])
+    if "shared_credentials_file" in config.aws:
+        config.aws["shared_credentials_file"] = os.path.expanduser(
+            config.aws["shared_credentials_file"]
+        )
     return config
 
 
 def request_cookies(url, session_token):
     """
     Request session cookie.
 
     :param url: okta org url, str
     :param session_token: session token, str
     :returns: cookies object
     """
     url = f"{url}/api/v1/sessions"
     data = json.dumps({"sessionToken": f"{session_token}"})
 
-    response_with_cookie = make_request(method="POST", url=url, data=data)
+    response_with_cookie = request_wrapper(method="POST", url=url, data=data)
     sess_id = response_with_cookie.json()["id"]
     add_sensitive_value_to_be_masked(sess_id)
 
     cookies = response_with_cookie.cookies
     cookies.update({"sid": f"{sess_id}"})
     logger.debug(f"Session cookies: {cookies}")
 
     return cookies
 
 
-def discover_tile(url, cookies):
+def discover_tiles(url, cookies):
     """
     Discover aws tile url on user's okta dashboard.
 
     :param url: okta org url
     :param cookies: HTML cookies
     :returns: aws tile url. str
     """
     url = f"{url}/api/v1/users/me/home/tabs"
     params = {
         "type": "all",
         "expand": ["items", "items.resource"],
     }
     logger.debug(f"Performing auto-discovery on {url}.")
-    response_with_tabs = make_request(method="GET", url=url, cookies=cookies, params=params)
+    response_with_tabs = request_wrapper(method="GET", url=url, cookies=cookies, params=params)
     tabs = response_with_tabs.json()
 
     aws_tiles = []
     for tab in tabs:
         for tile in tab["_embedded"]["items"]:
             if "amazon_aws" in tile["_embedded"]["resource"]["linkUrl"]:
                 aws_tiles.append(tile["_embedded"]["resource"])
@@ -1223,29 +1247,35 @@
         else (aws_tiles[0]["linkUrl"], aws_tiles[0]["label"])
     )
     logger.debug(f"Discovered {len(tile)} URLs.")
 
     return tile
 
 
-def make_request(method, url, headers=None, **kwargs):
+def request_wrapper(method, url, headers=None, **kwargs):
     """
     Wrap 'requests.request' and perform response checks.
 
     :param method: request method
     :param url: request URL
     :param headers: request headers
     :param kwargs: additional parameters passed to request
     :returns: response object
     """
     if headers is None:
         headers = {"content-type": "application/json", "accept": "application/json"}
 
-    response = requests.request(method=method, url=url, headers=headers, **kwargs)
-
-    if response.status_code != 200:
+    logger.debug(f"Issuing {method} request to {url} with {headers} and {kwargs}")
+    try:
+        response = requests.request(method=method, url=url, headers=headers, **kwargs)
+        response.raise_for_status()
+    except requests.exceptions.HTTPError as err:
         logger.error(
-            f"Your {method} request failed with status_code {response.status_code}.\n"
-            f"{response.content}\n"
+            f"The {method} request to {url} failed ({err.response.status_code}): "
+            f"{err.response.text}"
         )
+        sys.exit(1)
+    except Exception as err:
+        logger.error(f"The {method} request to {url} failed with {err}")
+        sys.exit(1)
 
     return response
```

