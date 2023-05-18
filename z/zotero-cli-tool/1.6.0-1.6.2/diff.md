# Comparing `tmp/zotero-cli-tool-1.6.0.tar.gz` & `tmp/zotero-cli-tool-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zotero-cli-tool-1.6.0.tar", last modified: Thu May 18 22:46:00 2023, max compression
+gzip compressed data, was "zotero-cli-tool-1.6.2.tar", last modified: Thu May 18 23:14:26 2023, max compression
```

## Comparing `zotero-cli-tool-1.6.0.tar` & `zotero-cli-tool-1.6.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2023-05-18 22:46:00.079406 zotero-cli-tool-1.6.0/
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2023-05-18 22:46:00.075406 zotero-cli-tool-1.6.0/.github/
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2023-05-18 22:46:00.075406 zotero-cli-tool-1.6.0/.github/workflows/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     2228 2023-05-18 22:39:49.000000 zotero-cli-tool-1.6.0/.github/workflows/publish-package.yml
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1829 2023-05-17 17:38:52.000000 zotero-cli-tool-1.6.0/.gitignore
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      115 2022-07-23 09:33:59.000000 zotero-cli-tool-1.6.0/.readthedocs.yml
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    35149 2023-05-17 17:38:52.000000 zotero-cli-tool-1.6.0/LICENSE
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    50428 2023-05-18 22:46:00.079406 zotero-cli-tool-1.6.0/PKG-INFO
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     8811 2023-05-18 22:24:10.000000 zotero-cli-tool-1.6.0/README.md
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2023-05-18 22:46:00.079406 zotero-cli-tool-1.6.0/docs/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1182 2023-05-17 21:14:29.000000 zotero-cli-tool-1.6.0/docs/mkdocs.yml
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2023-05-18 22:46:00.079406 zotero-cli-tool-1.6.0/docs/pages/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     3567 2023-05-17 17:38:52.000000 zotero-cli-tool-1.6.0/docs/pages/faq.md
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2023-05-18 22:46:00.079406 zotero-cli-tool-1.6.0/docs/pages/imgs/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     7451 2023-05-17 21:16:25.000000 zotero-cli-tool-1.6.0/docs/pages/imgs/icon.png
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    21129 2023-05-17 17:38:52.000000 zotero-cli-tool-1.6.0/docs/pages/imgs/logo.png
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1066 2023-05-17 17:38:52.000000 zotero-cli-tool-1.6.0/docs/pages/index.md
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    11147 2023-05-17 17:38:52.000000 zotero-cli-tool-1.6.0/docs/pages/usage.md
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      100 2022-07-22 21:06:38.000000 zotero-cli-tool-1.6.0/docs/requirements.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1498 2023-05-18 22:16:27.000000 zotero-cli-tool-1.6.0/pyproject.toml
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       50 2023-05-18 22:16:19.000000 zotero-cli-tool-1.6.0/requirements.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       38 2023-05-18 22:46:00.079406 zotero-cli-tool-1.6.0/setup.cfg
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2023-05-18 22:46:00.075406 zotero-cli-tool-1.6.0/src/
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2023-05-18 22:46:00.079406 zotero-cli-tool-1.6.0/src/zotero/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        6 2023-05-17 20:46:41.000000 zotero-cli-tool-1.6.0/src/zotero/VERSION.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      313 2023-05-17 20:53:42.000000 zotero-cli-tool-1.6.0/src/zotero/__info__.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    39890 2023-05-18 19:49:01.000000 zotero-cli-tool-1.6.0/src/zotero/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     7173 2023-05-18 20:31:01.000000 zotero-cli-tool-1.6.0/src/zotero/__main__.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2023-05-18 22:46:00.079406 zotero-cli-tool-1.6.0/src/zotero_cli_tool.egg-info/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    50428 2023-05-18 22:46:00.000000 zotero-cli-tool-1.6.0/src/zotero_cli_tool.egg-info/PKG-INFO
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      613 2023-05-18 22:46:00.000000 zotero-cli-tool-1.6.0/src/zotero_cli_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        1 2023-05-18 22:46:00.000000 zotero-cli-tool-1.6.0/src/zotero_cli_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       52 2023-05-18 22:46:00.000000 zotero-cli-tool-1.6.0/src/zotero_cli_tool.egg-info/entry_points.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       50 2023-05-18 22:46:00.000000 zotero-cli-tool-1.6.0/src/zotero_cli_tool.egg-info/requires.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        7 2023-05-18 22:46:00.000000 zotero-cli-tool-1.6.0/src/zotero_cli_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:26.801484 zotero-cli-tool-1.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:26.793484 zotero-cli-tool-1.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:26.797484 zotero-cli-tool-1.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/.github/workflows/publish-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    49919 2023-05-18 23:14:26.801484 zotero-cli-tool-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:26.797484 zotero-cli-tool-1.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:26.797484 zotero-cli-tool-1.6.2/docs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/docs/pages/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:26.797484 zotero-cli-tool-1.6.2/docs/pages/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/docs/pages/imgs/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21129 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/docs/pages/imgs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/docs/pages/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/docs/pages/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:14:26.801484 zotero-cli-tool-1.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:26.797484 zotero-cli-tool-1.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:26.797484 zotero-cli-tool-1.6.2/src/zotero/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/src/zotero/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/src/zotero/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39890 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/src/zotero/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7173 2023-05-18 23:14:17.000000 zotero-cli-tool-1.6.2/src/zotero/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:14:26.801484 zotero-cli-tool-1.6.2/src/zotero_cli_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49919 2023-05-18 23:14:26.000000 zotero-cli-tool-1.6.2/src/zotero_cli_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-18 23:14:26.000000 zotero-cli-tool-1.6.2/src/zotero_cli_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:14:26.000000 zotero-cli-tool-1.6.2/src/zotero_cli_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-18 23:14:26.000000 zotero-cli-tool-1.6.2/src/zotero_cli_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-18 23:14:26.000000 zotero-cli-tool-1.6.2/src/zotero_cli_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 23:14:26.000000 zotero-cli-tool-1.6.2/src/zotero_cli_tool.egg-info/top_level.txt
```

### Comparing `zotero-cli-tool-1.6.0/.github/workflows/publish-package.yml` & `zotero-cli-tool-1.6.2/.github/workflows/publish-package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -58,10 +58,9 @@
     - if: steps.filter.outputs.version == 'true'
       run: python3 -m pip install --upgrade build && python3 -m build
     - if: steps.filter.outputs.version == 'true'
       name: Upload to PyPi
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.PYPI_API_TOKEN }}
-        repository-url: https://pypi.org/project/zotero-cli-tool/
         verbose: true
         verify_metadata: false
```

### Comparing `zotero-cli-tool-1.6.0/.gitignore` & `zotero-cli-tool-1.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/LICENSE` & `zotero-cli-tool-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/PKG-INFO` & `zotero-cli-tool-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zotero-cli-tool
-Version: 1.6.0
+Version: 1.6.2
 Summary: Tinyscript tool for sorting and exporting Zotero references based on pyzotero
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,28 +699,28 @@
 <p align="center"><img src="https://github.com/dhondta/zotero-cli/raw/main/docs/pages/imgs/logo.png"></p>
 <h1 align="center">Zotero CLI <a href="https://twitter.com/intent/tweet?text=Zotero%20CLI%20-%20A%20Tinyscript%20tool%20for%20sorting,%20ranking%20and%20exporting%20Zotero%20references%20based%20on%20pyzotero.%0D%0Ahttps%3a%2f%2fgithub%2ecom%2fdhondta%2fzotero-cli%0D%0A&hashtags=python,zotero,cli,pyzotero,pagerank"><img src="https://img.shields.io/badge/Tweet--lightgrey?logo=twitter&style=social" alt="Tweet" height="20"/></a></h1>
 <h3 align="center">Sort and rank your Zotero references easy from your CLI.</h3>
 
 [![PyPi](https://img.shields.io/pypi/v/zotero-cli-tool.svg)](https://pypi.python.org/pypi/zotero-cli-tool/)
 ![Platform](https://img.shields.io/badge/platform-linux-yellow.svg)
 [![Python Versions](https://img.shields.io/pypi/pyversions/peid.svg)](https://pypi.python.org/pypi/zotero-cli-tool/)
-[![Build Status](https://github.com/dhondta/zotero-cli/actions/workflows/python-package.yml/badge.svg)](https://github.com/dhondta/zotero-cli/actions/workflows/python-package.yml)
+[![Build Status](https://github.com/dhondta/zotero-cli/actions/workflows/publish-package.yml/badge.svg)](https://github.com/dhondta/zotero-cli/actions/workflows/publish-package.yml)
 [![Read The Docs](https://readthedocs.org/projects/zotero-cli/badge/?version=latest)](https://zotero-cli.readthedocs.io/en/latest/?badge=latest)
 [![Known Vulnerabilities](https://snyk.io/test/github/dhondta/zotero-cli/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/dhondta/zotero-cli?targetFile=requirements.txt)
 [![DOI](https://zenodo.org/badge/321932121.svg)](https://zenodo.org/badge/latestdoi/321932121)
 [![License](https://img.shields.io/pypi/l/zotero-cli-tool.svg)](https://pypi.python.org/pypi/zotero-cli-tool/)
 
 This [Tinyscript](https://github.com/dhondta/python-tinyscript) tool relies on [`pyzotero`](https://github.com/urschrei/pyzotero) for communicating with [Zotero's Web API](https://www.zotero.org/support/dev/web_api/v3/start). It allows to list field values, show items in tables in the CLI or also export sorted items to an Excel file.
 
 
 ```session
 $ pip install zotero-cli-tool
 ```
 
-## :fast_forward: Quick Start
+## Quick Start
 
 The first time you start it, the tool will ask for your API identifier and key. It will cache it to `~/.zotero/creds.txt` with permissions set to `rw` for your user only. Data is cached to `~/.zotero/cache/`. If you are using a shared group library, you can either pass the "`-g`" ("`--group`") option in your `zotero-cli` command or, for setting it permanently, touch an empty file `~/.zotero/group`.
 
 - Manually update cached data
 
 ```sh
 $ zotero-cli reset
@@ -811,15 +811,15 @@
 > **Markers**:
 > 
 > - `read` / `unread`: by default, items are displayed in bold ; marking an item as read will make it display as normal
 > - `irrelevant` / `relevant`: this allows to exclude a result from the output list of items
 > - `ignore` / `unignore`: this allows to completely ignore an item, including in the ranking algorithm
 
 
-## :bulb: Special Features
+## Special Features
 
 Some additional fields can be used for listing/filtering/showing/exporting data.
 
 - Computed fields
 
   - `authors`: the list of `creators` with `creatorType` equal to `author`
   - `citations`: the number of relations the item has to other items with a later date
@@ -841,14 +841,7 @@
   - `zscc`: number of Scholar citations, computed with the [Zotero Google Scholar Citations](https://github.com/beloglazov/zotero-scholar-citations) plugin
 
 - PageRank-based reference ranking algorithm
 
   - `rank`: computed field aimed to rank references in order of relevance ; this uses an algorithm similar to Google's PageRank while weighting references in function of their year of publication (giving more importance to recent references, which cannot have as much citations as older references anyway)
 
 
-## :clap:  Supporters
-
-[![Stargazers repo roster for @dhondta/zotero-cli](https://reporoster.com/stars/dark/dhondta/zotero-cli)](https://github.com/dhondta/zotero-cli/stargazers)
-
-[![Forkers repo roster for @dhondta/zotero-cli](https://reporoster.com/forks/dark/dhondta/zotero-cli)](https://github.com/dhondta/zotero-cli/network/members)
-
-<p align="center"><a href="#"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>
```

### Comparing `zotero-cli-tool-1.6.0/README.md` & `zotero-cli-tool-1.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 <p align="center"><img src="https://github.com/dhondta/zotero-cli/raw/main/docs/pages/imgs/logo.png"></p>
 <h1 align="center">Zotero CLI <a href="https://twitter.com/intent/tweet?text=Zotero%20CLI%20-%20A%20Tinyscript%20tool%20for%20sorting,%20ranking%20and%20exporting%20Zotero%20references%20based%20on%20pyzotero.%0D%0Ahttps%3a%2f%2fgithub%2ecom%2fdhondta%2fzotero-cli%0D%0A&hashtags=python,zotero,cli,pyzotero,pagerank"><img src="https://img.shields.io/badge/Tweet--lightgrey?logo=twitter&style=social" alt="Tweet" height="20"/></a></h1>
 <h3 align="center">Sort and rank your Zotero references easy from your CLI.</h3>
 
 [![PyPi](https://img.shields.io/pypi/v/zotero-cli-tool.svg)](https://pypi.python.org/pypi/zotero-cli-tool/)
 ![Platform](https://img.shields.io/badge/platform-linux-yellow.svg)
 [![Python Versions](https://img.shields.io/pypi/pyversions/peid.svg)](https://pypi.python.org/pypi/zotero-cli-tool/)
-[![Build Status](https://github.com/dhondta/zotero-cli/actions/workflows/python-package.yml/badge.svg)](https://github.com/dhondta/zotero-cli/actions/workflows/python-package.yml)
+[![Build Status](https://github.com/dhondta/zotero-cli/actions/workflows/publish-package.yml/badge.svg)](https://github.com/dhondta/zotero-cli/actions/workflows/publish-package.yml)
 [![Read The Docs](https://readthedocs.org/projects/zotero-cli/badge/?version=latest)](https://zotero-cli.readthedocs.io/en/latest/?badge=latest)
 [![Known Vulnerabilities](https://snyk.io/test/github/dhondta/zotero-cli/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/dhondta/zotero-cli?targetFile=requirements.txt)
 [![DOI](https://zenodo.org/badge/321932121.svg)](https://zenodo.org/badge/latestdoi/321932121)
 [![License](https://img.shields.io/pypi/l/zotero-cli-tool.svg)](https://pypi.python.org/pypi/zotero-cli-tool/)
 
 This [Tinyscript](https://github.com/dhondta/python-tinyscript) tool relies on [`pyzotero`](https://github.com/urschrei/pyzotero) for communicating with [Zotero's Web API](https://www.zotero.org/support/dev/web_api/v3/start). It allows to list field values, show items in tables in the CLI or also export sorted items to an Excel file.
 
 
 ```session
 $ pip install zotero-cli-tool
 ```
 
-## :fast_forward: Quick Start
+## Quick Start
 
 The first time you start it, the tool will ask for your API identifier and key. It will cache it to `~/.zotero/creds.txt` with permissions set to `rw` for your user only. Data is cached to `~/.zotero/cache/`. If you are using a shared group library, you can either pass the "`-g`" ("`--group`") option in your `zotero-cli` command or, for setting it permanently, touch an empty file `~/.zotero/group`.
 
 - Manually update cached data
 
 ```sh
 $ zotero-cli reset
@@ -113,15 +113,15 @@
 > **Markers**:
 > 
 > - `read` / `unread`: by default, items are displayed in bold ; marking an item as read will make it display as normal
 > - `irrelevant` / `relevant`: this allows to exclude a result from the output list of items
 > - `ignore` / `unignore`: this allows to completely ignore an item, including in the ranking algorithm
 
 
-## :bulb: Special Features
+## Special Features
 
 Some additional fields can be used for listing/filtering/showing/exporting data.
 
 - Computed fields
 
   - `authors`: the list of `creators` with `creatorType` equal to `author`
   - `citations`: the number of relations the item has to other items with a later date
@@ -143,14 +143,7 @@
   - `zscc`: number of Scholar citations, computed with the [Zotero Google Scholar Citations](https://github.com/beloglazov/zotero-scholar-citations) plugin
 
 - PageRank-based reference ranking algorithm
 
   - `rank`: computed field aimed to rank references in order of relevance ; this uses an algorithm similar to Google's PageRank while weighting references in function of their year of publication (giving more importance to recent references, which cannot have as much citations as older references anyway)
 
 
-## :clap:  Supporters
-
-[![Stargazers repo roster for @dhondta/zotero-cli](https://reporoster.com/stars/dark/dhondta/zotero-cli)](https://github.com/dhondta/zotero-cli/stargazers)
-
-[![Forkers repo roster for @dhondta/zotero-cli](https://reporoster.com/forks/dark/dhondta/zotero-cli)](https://github.com/dhondta/zotero-cli/network/members)
-
-<p align="center"><a href="#"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>
```

#### html2text {}

```diff
@@ -1,59 +1,58 @@
    [https://github.com/dhondta/zotero-cli/raw/main/docs/pages/imgs/logo.png]
                        ****** Zotero CLI [Tweet] ******
       **** Sort and rank your Zotero references easy from your CLI. ****
 [![PyPi](https://img.shields.io/pypi/v/zotero-cli-tool.svg)](https://
 pypi.python.org/pypi/zotero-cli-tool/) ![Platform](https://img.shields.io/
 badge/platform-linux-yellow.svg) [![Python Versions](https://img.shields.io/
 pypi/pyversions/peid.svg)](https://pypi.python.org/pypi/zotero-cli-tool/) [!
-[Build Status](https://github.com/dhondta/zotero-cli/actions/workflows/python-
+[Build Status](https://github.com/dhondta/zotero-cli/actions/workflows/publish-
 package.yml/badge.svg)](https://github.com/dhondta/zotero-cli/actions/
-workflows/python-package.yml) [![Read The Docs](https://readthedocs.org/
+workflows/publish-package.yml) [![Read The Docs](https://readthedocs.org/
 projects/zotero-cli/badge/?version=latest)](https://zotero-cli.readthedocs.io/
 en/latest/?badge=latest) [![Known Vulnerabilities](https://snyk.io/test/github/
 dhondta/zotero-cli/badge.svg?targetFile=requirements.txt)](https://snyk.io/
 test/github/dhondta/zotero-cli?targetFile=requirements.txt) [![DOI](https://
 zenodo.org/badge/321932121.svg)](https://zenodo.org/badge/latestdoi/321932121)
 [![License](https://img.shields.io/pypi/l/zotero-cli-tool.svg)](https://
 pypi.python.org/pypi/zotero-cli-tool/) This [Tinyscript](https://github.com/
 dhondta/python-tinyscript) tool relies on [`pyzotero`](https://github.com/
 urschrei/pyzotero) for communicating with [Zotero's Web API](https://
 www.zotero.org/support/dev/web_api/v3/start). It allows to list field values,
 show items in tables in the CLI or also export sorted items to an Excel file.
-```session $ pip install zotero-cli-tool ``` ## :fast_forward: Quick Start The
-first time you start it, the tool will ask for your API identifier and key. It
-will cache it to `~/.zotero/creds.txt` with permissions set to `rw` for your
-user only. Data is cached to `~/.zotero/cache/`. If you are using a shared
-group library, you can either pass the "`-g`" ("`--group`") option in your
-`zotero-cli` command or, for setting it permanently, touch an empty file
-`~/.zotero/group`. - Manually update cached data ```sh $ zotero-cli reset ```
-Note that it could take a while. That's why caching is interesting for further
-use. - Count items in a collection ```sh $ zotero-cli count --filter
-"collections:biblio" 123 ``` - List values for a given field ```sh $ zotero-cli
-list itemType Type ---- computer program conference paper document journal
-article manuscript thesis webpage ``` - Show entries with the given set of
-fields, filtered based on multiple critera and limited to a given number of
-items ```sh $ zotero-cli show year title itemType numPages --filter
-"collections:biblio" --filter "title:detect" --limit ">date:10" Year Title Type
-#Pages ---- ----- ---- ------ 2016 Classifying Packed Programs as Malicious
-Software Detected conference paper 3 2016 Detecting Packed Executable File:
-Supervised or Anomaly Detection Method? conference paper 5 2016 Entropy
-analysis to classify unknown packing algorithms for malware detection
-conference paper 21 2017 Packer Detection for Multi-Layer Executables Using
-Entropy Analysis journal article 18 2018 Sensitive system calls based packed
-malware variants detection using principal component initialized MultiLayers
-neural networks journal article 13 2018 Effective, efficient, and robust
-packing detection and classification journal article 15 2019 Efficient
-automatic original entry point detection journal article 14 2019 All-in-One
-Framework for Detection, Unpacking, and Verification for Malware Analysis
-journal article 16 2020 Experimental Comparison of Machine Learning Models in
-Malware Packing Detection conference paper 3 2020 Building a smart and
-automated tool for packed malware detections using machine learning thesis 99
-``` - Export entries ```sh $ zotero-cli export year title itemType numPages --
-filter "collections:biblio" --filter "title:detect" --limit ">date:10" $ file
+```session $ pip install zotero-cli-tool ``` ## Quick Start The first time you
+start it, the tool will ask for your API identifier and key. It will cache it
+to `~/.zotero/creds.txt` with permissions set to `rw` for your user only. Data
+is cached to `~/.zotero/cache/`. If you are using a shared group library, you
+can either pass the "`-g`" ("`--group`") option in your `zotero-cli` command
+or, for setting it permanently, touch an empty file `~/.zotero/group`. -
+Manually update cached data ```sh $ zotero-cli reset ``` Note that it could
+take a while. That's why caching is interesting for further use. - Count items
+in a collection ```sh $ zotero-cli count --filter "collections:biblio" 123 ```
+- List values for a given field ```sh $ zotero-cli list itemType Type ---
+- computer program conference paper document journal article manuscript thesis
+webpage ``` - Show entries with the given set of fields, filtered based on
+multiple critera and limited to a given number of items ```sh $ zotero-cli show
+year title itemType numPages --filter "collections:biblio" --filter "title:
+detect" --limit ">date:10" Year Title Type #Pages ---- ----- ---- ------ 2016
+Classifying Packed Programs as Malicious Software Detected conference paper 3
+2016 Detecting Packed Executable File: Supervised or Anomaly Detection Method?
+conference paper 5 2016 Entropy analysis to classify unknown packing algorithms
+for malware detection conference paper 21 2017 Packer Detection for Multi-Layer
+Executables Using Entropy Analysis journal article 18 2018 Sensitive system
+calls based packed malware variants detection using principal component
+initialized MultiLayers neural networks journal article 13 2018 Effective,
+efficient, and robust packing detection and classification journal article 15
+2019 Efficient automatic original entry point detection journal article 14 2019
+All-in-One Framework for Detection, Unpacking, and Verification for Malware
+Analysis journal article 16 2020 Experimental Comparison of Machine Learning
+Models in Malware Packing Detection conference paper 3 2020 Building a smart
+and automated tool for packed malware detections using machine learning thesis
+99 ``` - Export entries ```sh $ zotero-cli export year title itemType numPages
+--filter "collections:biblio" --filter "title:detect" --limit ">date:10" $ file
 export.xlsx export.xlsx: Microsoft Excel 2007+ ``` - Use a predefined query
 ```sh $ zotero-cli show - --query "top-50-most-relevants" ``` > **Note**: "`-`"
 is used for the `field` positional argument to tell the tool to select the
 predefined list of fields included in the query. This is equivalent to: ```sh $
 zotero-cli show year title numPages itemType --limit ">rank:50" ``` Available
 queries: - `no-attachment`: list of all items with no attachment ; displayed
 fields: `title` - `no-url`: list of all items with no URL ; displayed fields:
@@ -61,18 +60,18 @@
 fields: `year`, `title`, `numPages`, `itemType` - `top-50-most-relevants`: same
 as top-10 but with the top-50 - Mark items ```sh $ zotero-cli mark read --
 filter "title:a nice paper" $ zotero-cli mark unread --filter "title:a nice
 paper" ``` > **Markers**: > > - `read` / `unread`: by default, items are
 displayed in bold ; marking an item as read will make it display as normal > -
 `irrelevant` / `relevant`: this allows to exclude a result from the output list
 of items > - `ignore` / `unignore`: this allows to completely ignore an item,
-including in the ranking algorithm ## :bulb: Special Features Some additional
-fields can be used for listing/filtering/showing/exporting data. - Computed
-fields - `authors`: the list of `creators` with `creatorType` equal to `author`
-- `citations`: the number of relations the item has to other items with a later
+including in the ranking algorithm ## Special Features Some additional fields
+can be used for listing/filtering/showing/exporting data. - Computed fields -
+`authors`: the list of `creators` with `creatorType` equal to `author` -
+`citations`: the number of relations the item has to other items with a later
 date - `editors`: the list of `creators` with `creatorType` equal to `editor` -
 `numAttachments`: the number of child items with `itemType` equal to
 `attachment` - `numAuthors`: the number of `creators` with `creatorType` equal
 to `author` - `numCreators`: the number of `creators` - `numEditors`: the
 number of `creators` with `creatorType` equal to `editor` - `numNotes`: the
 number of child items with `itemType` equal to `note` - `numPages`: the
 (corrected) number of pages, either got from the original or `pages` field -
@@ -83,14 +82,8 @@
 related to the item - `what`: custom field for a short description of what the
 item is about - `zscc`: number of Scholar citations, computed with the [Zotero
 Google Scholar Citations](https://github.com/beloglazov/zotero-scholar-
 citations) plugin - PageRank-based reference ranking algorithm - `rank`:
 computed field aimed to rank references in order of relevance ; this uses an
 algorithm similar to Google's PageRank while weighting references in function
 of their year of publication (giving more importance to recent references,
-which cannot have as much citations as older references anyway) ## :clap:
-Supporters [![Stargazers repo roster for @dhondta/zotero-cli](https://
-reporoster.com/stars/dark/dhondta/zotero-cli)](https://github.com/dhondta/
-zotero-cli/stargazers) [![Forkers repo roster for @dhondta/zotero-cli](https://
-reporoster.com/forks/dark/dhondta/zotero-cli)](https://github.com/dhondta/
-zotero-cli/network/members)
-                                 [Back_to_top]
+which cannot have as much citations as older references anyway)
```

### Comparing `zotero-cli-tool-1.6.0/docs/mkdocs.yml` & `zotero-cli-tool-1.6.2/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/docs/pages/faq.md` & `zotero-cli-tool-1.6.2/docs/pages/faq.md`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/docs/pages/imgs/icon.png` & `zotero-cli-tool-1.6.2/docs/pages/imgs/icon.png`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/docs/pages/imgs/logo.png` & `zotero-cli-tool-1.6.2/docs/pages/imgs/logo.png`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/docs/pages/index.md` & `zotero-cli-tool-1.6.2/docs/pages/index.md`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/docs/pages/usage.md` & `zotero-cli-tool-1.6.2/docs/pages/usage.md`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/pyproject.toml` & `zotero-cli-tool-1.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/src/zotero/__init__.py` & `zotero-cli-tool-1.6.2/src/zotero/__init__.py`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/src/zotero/__main__.py` & `zotero-cli-tool-1.6.2/src/zotero/__main__.py`

 * *Files identical despite different names*

### Comparing `zotero-cli-tool-1.6.0/src/zotero_cli_tool.egg-info/PKG-INFO` & `zotero-cli-tool-1.6.2/src/zotero_cli_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zotero-cli-tool
-Version: 1.6.0
+Version: 1.6.2
 Summary: Tinyscript tool for sorting and exporting Zotero references based on pyzotero
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,28 +699,28 @@
 <p align="center"><img src="https://github.com/dhondta/zotero-cli/raw/main/docs/pages/imgs/logo.png"></p>
 <h1 align="center">Zotero CLI <a href="https://twitter.com/intent/tweet?text=Zotero%20CLI%20-%20A%20Tinyscript%20tool%20for%20sorting,%20ranking%20and%20exporting%20Zotero%20references%20based%20on%20pyzotero.%0D%0Ahttps%3a%2f%2fgithub%2ecom%2fdhondta%2fzotero-cli%0D%0A&hashtags=python,zotero,cli,pyzotero,pagerank"><img src="https://img.shields.io/badge/Tweet--lightgrey?logo=twitter&style=social" alt="Tweet" height="20"/></a></h1>
 <h3 align="center">Sort and rank your Zotero references easy from your CLI.</h3>
 
 [![PyPi](https://img.shields.io/pypi/v/zotero-cli-tool.svg)](https://pypi.python.org/pypi/zotero-cli-tool/)
 ![Platform](https://img.shields.io/badge/platform-linux-yellow.svg)
 [![Python Versions](https://img.shields.io/pypi/pyversions/peid.svg)](https://pypi.python.org/pypi/zotero-cli-tool/)
-[![Build Status](https://github.com/dhondta/zotero-cli/actions/workflows/python-package.yml/badge.svg)](https://github.com/dhondta/zotero-cli/actions/workflows/python-package.yml)
+[![Build Status](https://github.com/dhondta/zotero-cli/actions/workflows/publish-package.yml/badge.svg)](https://github.com/dhondta/zotero-cli/actions/workflows/publish-package.yml)
 [![Read The Docs](https://readthedocs.org/projects/zotero-cli/badge/?version=latest)](https://zotero-cli.readthedocs.io/en/latest/?badge=latest)
 [![Known Vulnerabilities](https://snyk.io/test/github/dhondta/zotero-cli/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/dhondta/zotero-cli?targetFile=requirements.txt)
 [![DOI](https://zenodo.org/badge/321932121.svg)](https://zenodo.org/badge/latestdoi/321932121)
 [![License](https://img.shields.io/pypi/l/zotero-cli-tool.svg)](https://pypi.python.org/pypi/zotero-cli-tool/)
 
 This [Tinyscript](https://github.com/dhondta/python-tinyscript) tool relies on [`pyzotero`](https://github.com/urschrei/pyzotero) for communicating with [Zotero's Web API](https://www.zotero.org/support/dev/web_api/v3/start). It allows to list field values, show items in tables in the CLI or also export sorted items to an Excel file.
 
 
 ```session
 $ pip install zotero-cli-tool
 ```
 
-## :fast_forward: Quick Start
+## Quick Start
 
 The first time you start it, the tool will ask for your API identifier and key. It will cache it to `~/.zotero/creds.txt` with permissions set to `rw` for your user only. Data is cached to `~/.zotero/cache/`. If you are using a shared group library, you can either pass the "`-g`" ("`--group`") option in your `zotero-cli` command or, for setting it permanently, touch an empty file `~/.zotero/group`.
 
 - Manually update cached data
 
 ```sh
 $ zotero-cli reset
@@ -811,15 +811,15 @@
 > **Markers**:
 > 
 > - `read` / `unread`: by default, items are displayed in bold ; marking an item as read will make it display as normal
 > - `irrelevant` / `relevant`: this allows to exclude a result from the output list of items
 > - `ignore` / `unignore`: this allows to completely ignore an item, including in the ranking algorithm
 
 
-## :bulb: Special Features
+## Special Features
 
 Some additional fields can be used for listing/filtering/showing/exporting data.
 
 - Computed fields
 
   - `authors`: the list of `creators` with `creatorType` equal to `author`
   - `citations`: the number of relations the item has to other items with a later date
@@ -841,14 +841,7 @@
   - `zscc`: number of Scholar citations, computed with the [Zotero Google Scholar Citations](https://github.com/beloglazov/zotero-scholar-citations) plugin
 
 - PageRank-based reference ranking algorithm
 
   - `rank`: computed field aimed to rank references in order of relevance ; this uses an algorithm similar to Google's PageRank while weighting references in function of their year of publication (giving more importance to recent references, which cannot have as much citations as older references anyway)
 
 
-## :clap:  Supporters
-
-[![Stargazers repo roster for @dhondta/zotero-cli](https://reporoster.com/stars/dark/dhondta/zotero-cli)](https://github.com/dhondta/zotero-cli/stargazers)
-
-[![Forkers repo roster for @dhondta/zotero-cli](https://reporoster.com/forks/dark/dhondta/zotero-cli)](https://github.com/dhondta/zotero-cli/network/members)
-
-<p align="center"><a href="#"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>
```

### Comparing `zotero-cli-tool-1.6.0/src/zotero_cli_tool.egg-info/SOURCES.txt` & `zotero-cli-tool-1.6.2/src/zotero_cli_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

