# Comparing `tmp/pybit-5.2.0.tar.gz` & `tmp/pybit-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybit-5.2.0.tar", last modified: Tue Apr 18 19:02:58 2023, max compression
+gzip compressed data, was "pybit-5.3.0.tar", last modified: Fri May 19 19:12:35 2023, max compression
```

## Comparing `pybit-5.2.0.tar` & `pybit-5.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-18 19:02:58.257944 pybit-5.2.0/
--rw-r--r--   0 uk09002ml   (502) staff       (20)    21087 2023-04-18 19:02:46.000000 pybit-5.2.0/CHANGELOG.md
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1217 2022-05-19 15:36:12.000000 pybit-5.2.0/LICENSE
--rw-r--r--   0 uk09002ml   (502) staff       (20)       83 2021-06-17 15:56:06.000000 pybit-5.2.0/MANIFEST.in
--rw-r--r--   0 uk09002ml   (502) staff       (20)     7944 2023-04-18 19:02:58.258483 pybit-5.2.0/PKG-INFO
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6294 2023-04-06 11:15:33.000000 pybit-5.2.0/README.md
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-18 19:02:58.212828 pybit-5.2.0/examples/
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6148 2023-04-18 11:36:33.000000 pybit-5.2.0/examples/.DS_Store
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1143 2023-04-06 11:15:33.000000 pybit-5.2.0/examples/direct_session.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1450 2023-04-06 11:15:33.000000 pybit-5.2.0/examples/http_example_explanatory.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      315 2023-04-06 11:15:33.000000 pybit-5.2.0/examples/http_example_quickstart.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1861 2023-04-06 11:15:33.000000 pybit-5.2.0/examples/websocket_example_explanatory.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      258 2023-04-18 18:56:31.000000 pybit-5.2.0/examples/websocket_example_quickstart.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     2256 2023-04-06 11:15:33.000000 pybit-5.2.0/examples/wrapper_class.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-18 19:02:58.240763 pybit-5.2.0/pybit/
--rw-r--r--   0 uk09002ml   (502) staff       (20)       18 2023-04-18 19:02:46.000000 pybit-5.2.0/pybit/__init__.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1964 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_helpers.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    12518 2023-04-18 16:03:38.000000 pybit-5.2.0/pybit/_http_manager.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     7591 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_v5_account.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    14814 2023-04-18 19:02:46.000000 pybit-5.2.0/pybit/_v5_asset.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8532 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_v5_market.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8543 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_v5_position.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     2826 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_v5_spot_leverage_token.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     6176 2023-04-18 16:12:52.000000 pybit-5.2.0/pybit/_v5_spot_margin_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8521 2023-04-18 19:02:46.000000 pybit-5.2.0/pybit/_v5_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     5765 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_v5_user.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    15535 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/_websocket_stream.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      694 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/account.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1860 2023-04-18 19:02:46.000000 pybit-5.2.0/pybit/asset.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1461 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/exceptions.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-18 19:02:58.257012 pybit-5.2.0/pybit/legacy/
--rw-r--r--   0 uk09002ml   (502) staff       (20)        0 2023-04-18 15:54:54.000000 pybit-5.2.0/pybit/legacy/__init__.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1966 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/_helpers.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    32393 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/_http_manager.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    18474 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/_websocket_stream.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     9678 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/copy_trading.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1302 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/exceptions.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    13589 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/usdc_options.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)    14531 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/legacy/usdc_perpetual.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      856 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/market.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      607 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/position.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      406 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/spot_leverage_token.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      932 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/spot_margin_trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      600 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/trade.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)     8681 2023-04-12 17:27:28.000000 pybit-5.2.0/pybit/unified_trading.py
--rw-r--r--   0 uk09002ml   (502) staff       (20)      560 2023-04-06 11:15:33.000000 pybit-5.2.0/pybit/user.py
-drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-04-18 19:02:58.247269 pybit-5.2.0/pybit.egg-info/
--rw-r--r--   0 uk09002ml   (502) staff       (20)     7944 2023-04-18 19:02:58.000000 pybit-5.2.0/pybit.egg-info/PKG-INFO
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1156 2023-04-18 19:02:58.000000 pybit-5.2.0/pybit.egg-info/SOURCES.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2023-04-18 19:02:58.000000 pybit-5.2.0/pybit.egg-info/dependency_links.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2021-07-09 21:25:55.000000 pybit-5.2.0/pybit.egg-info/not-zip-safe
--rw-r--r--   0 uk09002ml   (502) staff       (20)       37 2023-04-18 19:02:58.000000 pybit-5.2.0/pybit.egg-info/requires.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)        6 2023-04-18 19:02:58.000000 pybit-5.2.0/pybit.egg-info/top_level.txt
--rw-r--r--   0 uk09002ml   (502) staff       (20)      131 2023-04-18 19:02:58.259988 pybit-5.2.0/setup.cfg
--rw-r--r--   0 uk09002ml   (502) staff       (20)     1232 2023-04-18 19:02:46.000000 pybit-5.2.0/setup.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-05-19 19:12:35.775159 pybit-5.3.0/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    21656 2023-05-19 19:10:45.000000 pybit-5.3.0/CHANGELOG.md
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1217 2022-05-19 15:36:12.000000 pybit-5.3.0/LICENSE
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       83 2021-06-17 15:56:06.000000 pybit-5.3.0/MANIFEST.in
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8093 2023-05-19 19:12:35.775743 pybit-5.3.0/PKG-INFO
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6585 2023-05-19 19:10:45.000000 pybit-5.3.0/README.md
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-05-19 19:12:35.680002 pybit-5.3.0/examples/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6148 2023-04-18 11:36:33.000000 pybit-5.3.0/examples/.DS_Store
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1143 2023-04-06 11:15:33.000000 pybit-5.3.0/examples/direct_session.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1605 2023-04-26 18:06:01.000000 pybit-5.3.0/examples/http_example_explanatory.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      315 2023-04-06 11:15:33.000000 pybit-5.3.0/examples/http_example_quickstart.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1861 2023-04-06 11:15:33.000000 pybit-5.3.0/examples/websocket_example_explanatory.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      258 2023-04-18 18:56:31.000000 pybit-5.3.0/examples/websocket_example_quickstart.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     2256 2023-04-06 11:15:33.000000 pybit-5.3.0/examples/wrapper_class.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-05-19 19:12:35.724890 pybit-5.3.0/pybit/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       18 2023-05-19 19:10:45.000000 pybit-5.3.0/pybit/__init__.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1964 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/_helpers.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    13117 2023-05-19 19:00:49.000000 pybit-5.3.0/pybit/_http_manager.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     7471 2023-04-26 18:06:01.000000 pybit-5.3.0/pybit/_v5_account.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    14814 2023-04-26 18:06:01.000000 pybit-5.3.0/pybit/_v5_asset.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8532 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/_v5_market.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8543 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/_v5_position.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     2826 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/_v5_spot_leverage_token.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     6176 2023-04-18 16:12:52.000000 pybit-5.3.0/pybit/_v5_spot_margin_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8521 2023-04-26 18:06:01.000000 pybit-5.3.0/pybit/_v5_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     5765 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/_v5_user.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    15265 2023-05-19 19:00:49.000000 pybit-5.3.0/pybit/_websocket_stream.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      694 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/account.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1860 2023-04-26 18:06:01.000000 pybit-5.3.0/pybit/asset.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1773 2023-05-19 19:00:49.000000 pybit-5.3.0/pybit/exceptions.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-05-19 19:12:35.773649 pybit-5.3.0/pybit/legacy/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        0 2023-04-18 15:54:54.000000 pybit-5.3.0/pybit/legacy/__init__.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1966 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/legacy/_helpers.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    32393 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/legacy/_http_manager.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    18474 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/legacy/_websocket_stream.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     9678 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/legacy/copy_trading.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1302 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/legacy/exceptions.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    13589 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/legacy/usdc_options.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)    14531 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/legacy/usdc_perpetual.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      856 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/market.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      607 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/position.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      406 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/spot_leverage_token.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      932 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/spot_margin_trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      600 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/trade.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8889 2023-05-19 19:00:49.000000 pybit-5.3.0/pybit/unified_trading.py
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      560 2023-04-06 11:15:33.000000 pybit-5.3.0/pybit/user.py
+drwxr-xr-x   0 uk09002ml   (502) staff       (20)        0 2023-05-19 19:12:35.742730 pybit-5.3.0/pybit.egg-info/
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     8093 2023-05-19 19:12:35.000000 pybit-5.3.0/pybit.egg-info/PKG-INFO
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1156 2023-05-19 19:12:35.000000 pybit-5.3.0/pybit.egg-info/SOURCES.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2023-05-19 19:12:35.000000 pybit-5.3.0/pybit.egg-info/dependency_links.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        1 2021-07-09 21:25:55.000000 pybit-5.3.0/pybit.egg-info/not-zip-safe
+-rw-r--r--   0 uk09002ml   (502) staff       (20)       37 2023-05-19 19:12:35.000000 pybit-5.3.0/pybit.egg-info/requires.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)        6 2023-05-19 19:12:35.000000 pybit-5.3.0/pybit.egg-info/top_level.txt
+-rw-r--r--   0 uk09002ml   (502) staff       (20)      131 2023-05-19 19:12:35.779100 pybit-5.3.0/setup.cfg
+-rw-r--r--   0 uk09002ml   (502) staff       (20)     1085 2023-05-19 19:10:45.000000 pybit-5.3.0/setup.py
```

### Comparing `pybit-5.2.0/CHANGELOG.md` & `pybit-5.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,29 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [5.3.0] - 2023-05-19
+### Added
+- Multiple symbol support for WebSocket topics (pass `symbol` as a list)
+- Extra logging (log response headers) when passing `log_requests=True`
+- Argument `return_response_headers` for `HTTP` to allow returning the response headers to the user
+
+### Modified
+- Add response headers to exceptions
+
+### Fixed
+- Update PyPI package's python version so that only =>3.9 is supported to prevent the error: `TypeError: 'type' object is not subscriptable`
+- Fix API rate limit handling
+- Remove unnecessary `print` statements in two methods
+
+
 ## [5.2.0] - 2023-04-18
 ### Added
 - New asset endpoints: `set_deposit_account()`, `get_internal_deposit_records()`, `get_withdrawable_amount()`
 
 ### Fixed
 - Ensure that `legacy` submodule is packaged by `setup.py`
 - Fix non-UTA (normal account) spot margin trading endpoints
```

### Comparing `pybit-5.2.0/LICENSE` & `pybit-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/PKG-INFO` & `pybit-5.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybit
-Version: 5.2.0
+Version: 5.3.0
 Summary: Python3 Bybit HTTP/WebSocket API Connector
 Home-page: https://github.com/bybit-exchange/pybit
 Author: Dexter Dickinson
 Author-email: dexter.dickinson@bybit.com
 License: MIT License
 Description: # pybit
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
@@ -24,15 +24,15 @@
         - [Installation](#installation)
         - [Usage](#usage)
         - [Contact](#contact)
         - [Contributors](#contributors)
         - [Donations](#donations)
         
         ## About
-        Put simply, `pybit` (Python + Bybit) is the official lightweight one-stop-shop module for the Bybit HTTP and WebSocket APIs. Originally created by [Verata Veritatis](https://github.com/verata-veritatis), it's now maintained by Bybit employees - however, you're still welcome to contribute!
+        Put simply, `pybit` (Python + Bybit) is the official lightweight one-stop-shop module for the Bybit HTTP and WebSocket APIs. Originally created by [Verata Veritatis](https://github.com/verata-veritatis), it's now maintained by Bybit employees – however, you're still welcome to contribute!
         
         It was designed with the following vision in mind:
         
         > I was personally never a fan of auto-generated connectors that used a mosh-pit of various modules you didn't want (sorry, `bravado`) and wanted to build my own Python3-dedicated connector with very little external resources. The goal of the connector is to provide traders and developers with an easy-to-use high-performing module that has an active issue and discussion board leading to consistent improvements.
         
         ## Development
         `pybit` is being actively developed, and new Bybit API changes should arrive on `pybit` very quickly. `pybit` uses `requests` and `websocket-client` for its methods, alongside other built-in modules. Anyone is welcome to branch/fork the repository and add their own upgrades. If you think you've made substantial improvements to the module, submit a pull request and we'll gladly take a look.
@@ -96,14 +96,15 @@
           <tr>
             <td align="center"><a href="https://github.com/dextertd"><img src="https://avatars.githubusercontent.com/u/54495183?v=4" width="100px;" alt=""/><br /><sub><b>dextertd</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=dextertd" title="Code">💻</a> <a href="https://github.com/bybit-exchange/pybit/commits?author=dextertd" title="Documentation">📖</a></td>
             <td align="center"><a href="https://github.com/ervuks"><img src="https://avatars.githubusercontent.com/u/17198438?v=4" width="100px;" alt=""/><br /><sub><b>ervuks</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=ervuks" title="Code">💻</a> <a href="https://github.com/bybit-exchange/pybit/commits?author=ervuks" title="Documentation">📖</a></td></td>
             <td align="center"><a href="https://github.com/verata-veritatis"><img src="https://avatars0.githubusercontent.com/u/9677388?v=4" width="100px;" alt=""/><br /><sub><b>verata-veritatis</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=verata-veritatis" title="Code">💻</a> <a href="https://github.com/bybit-exchange/pybit/commits?author=verata-veritatis" title="Documentation">📖</a></td>
             <td align="center"><a href="https://github.com/APF20"><img src="https://avatars0.githubusercontent.com/u/74583612?v=4" width="100px;" alt=""/><br /><sub><b>APF20</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=APF20" title="Code">💻</a></td>
             <td align="center"><a href="https://github.com/cameronhh"><img src="https://avatars0.githubusercontent.com/u/30434979?v=4" width="100px;" alt=""/><br /><sub><b>Cameron Harder-Hutton</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=cameronhh" title="Code">💻</a></td>
             <td align="center"><a href="https://github.com/tomcru"><img src="https://avatars0.githubusercontent.com/u/35841182?v=4" width="100px;" alt=""/><br /><sub><b>Tom Rumpf</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=tomcru" title="Code">💻</a></td>
+            <td align="center"><a href="https://github.com/sheungon"><img src="https://avatars.githubusercontent.com/u/13306724?v=4" width="100px;" alt=""/><br /><sub><b>OnJohn</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=sheungon" title="Code">💻</a></td>
             <td align="center"><a href="https://github.com/tconley"><img src="https://avatars1.githubusercontent.com/u/1893207?v=4" width="100px;" alt=""/><br /><sub><b>Todd Conley</b></sub></a><br /><a href="https://github.com/tconley/pybit/commits?author=tconley" title="Ideas">🤔</a></td>
           </tr>
         </table>
         
         <!-- markdownlint-enable -->
         <!-- prettier-ignore-end -->
         <!-- ALL-CONTRIBUTORS-LIST:END -->
@@ -112,14 +113,11 @@
         
 Keywords: bybit api connector
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pybit-5.2.0/README.md` & `pybit-5.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 - [Installation](#installation)
 - [Usage](#usage)
 - [Contact](#contact)
 - [Contributors](#contributors)
 - [Donations](#donations)
 
 ## About
-Put simply, `pybit` (Python + Bybit) is the official lightweight one-stop-shop module for the Bybit HTTP and WebSocket APIs. Originally created by [Verata Veritatis](https://github.com/verata-veritatis), it's now maintained by Bybit employees - however, you're still welcome to contribute!
+Put simply, `pybit` (Python + Bybit) is the official lightweight one-stop-shop module for the Bybit HTTP and WebSocket APIs. Originally created by [Verata Veritatis](https://github.com/verata-veritatis), it's now maintained by Bybit employees – however, you're still welcome to contribute!
 
 It was designed with the following vision in mind:
 
 > I was personally never a fan of auto-generated connectors that used a mosh-pit of various modules you didn't want (sorry, `bravado`) and wanted to build my own Python3-dedicated connector with very little external resources. The goal of the connector is to provide traders and developers with an easy-to-use high-performing module that has an active issue and discussion board leading to consistent improvements.
 
 ## Development
 `pybit` is being actively developed, and new Bybit API changes should arrive on `pybit` very quickly. `pybit` uses `requests` and `websocket-client` for its methods, alongside other built-in modules. Anyone is welcome to branch/fork the repository and add their own upgrades. If you think you've made substantial improvements to the module, submit a pull request and we'll gladly take a look.
@@ -88,14 +88,15 @@
   <tr>
     <td align="center"><a href="https://github.com/dextertd"><img src="https://avatars.githubusercontent.com/u/54495183?v=4" width="100px;" alt=""/><br /><sub><b>dextertd</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=dextertd" title="Code">💻</a> <a href="https://github.com/bybit-exchange/pybit/commits?author=dextertd" title="Documentation">📖</a></td>
     <td align="center"><a href="https://github.com/ervuks"><img src="https://avatars.githubusercontent.com/u/17198438?v=4" width="100px;" alt=""/><br /><sub><b>ervuks</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=ervuks" title="Code">💻</a> <a href="https://github.com/bybit-exchange/pybit/commits?author=ervuks" title="Documentation">📖</a></td></td>
     <td align="center"><a href="https://github.com/verata-veritatis"><img src="https://avatars0.githubusercontent.com/u/9677388?v=4" width="100px;" alt=""/><br /><sub><b>verata-veritatis</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=verata-veritatis" title="Code">💻</a> <a href="https://github.com/bybit-exchange/pybit/commits?author=verata-veritatis" title="Documentation">📖</a></td>
     <td align="center"><a href="https://github.com/APF20"><img src="https://avatars0.githubusercontent.com/u/74583612?v=4" width="100px;" alt=""/><br /><sub><b>APF20</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=APF20" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/cameronhh"><img src="https://avatars0.githubusercontent.com/u/30434979?v=4" width="100px;" alt=""/><br /><sub><b>Cameron Harder-Hutton</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=cameronhh" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/tomcru"><img src="https://avatars0.githubusercontent.com/u/35841182?v=4" width="100px;" alt=""/><br /><sub><b>Tom Rumpf</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=tomcru" title="Code">💻</a></td>
+    <td align="center"><a href="https://github.com/sheungon"><img src="https://avatars.githubusercontent.com/u/13306724?v=4" width="100px;" alt=""/><br /><sub><b>OnJohn</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=sheungon" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/tconley"><img src="https://avatars1.githubusercontent.com/u/1893207?v=4" width="100px;" alt=""/><br /><sub><b>Todd Conley</b></sub></a><br /><a href="https://github.com/tconley/pybit/commits?author=tconley" title="Ideas">🤔</a></td>
   </tr>
 </table>
 
 <!-- markdownlint-enable -->
 <!-- prettier-ignore-end -->
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -6,48 +6,48 @@
 welcome-brightgreen.svg?style=flat) Official Python3 API connector for Bybit's
 HTTP and WebSockets APIs. ## Table of Contents - [About](#about) -
 [Development](#development) - [Installation](#installation) - [Usage](#usage) -
 [Contact](#contact) - [Contributors](#contributors) - [Donations](#donations)
 ## About Put simply, `pybit` (Python + Bybit) is the official lightweight one-
 stop-shop module for the Bybit HTTP and WebSocket APIs. Originally created by
 [Verata Veritatis](https://github.com/verata-veritatis), it's now maintained by
-Bybit employees - however, you're still welcome to contribute! It was designed
-with the following vision in mind: > I was personally never a fan of auto-
-generated connectors that used a mosh-pit of various modules you didn't want
-(sorry, `bravado`) and wanted to build my own Python3-dedicated connector with
-very little external resources. The goal of the connector is to provide traders
-and developers with an easy-to-use high-performing module that has an active
-issue and discussion board leading to consistent improvements. ## Development
-`pybit` is being actively developed, and new Bybit API changes should arrive on
-`pybit` very quickly. `pybit` uses `requests` and `websocket-client` for its
-methods, alongside other built-in modules. Anyone is welcome to branch/fork the
-repository and add their own upgrades. If you think you've made substantial
-improvements to the module, submit a pull request and we'll gladly take a look.
-## Installation `pybit` requires Python 3.9.1 or higher. The module can be
-installed manually or via [PyPI](https://pypi.org/project/pybit/) with `pip`:
-``` pip install pybit ``` ## Usage You can retrieve a specific market like so:
-```python from pybit.unified_trading import HTTP ``` Create an HTTP session and
-connect via WebSocket for Inverse on mainnet: ```python session = HTTP
-( testnet=False, api_key="...", api_secret="...", ) ``` Information can be sent
-to, or retrieved from, the Bybit APIs: ```python # Get the orderbook of the
-USDT Perpetual, BTCUSDT session.get_orderbook(category="linear",
-symbol="BTCUSDT") # Create five long USDC Options orders. # (Currently, only
-USDC Options support sending orders in bulk.) payload = {"category": "option"}
-orders = [{ "symbol": "BTC-30JUN23-20000-C", "side": "Buy", "orderType":
-"Limit", "qty": "0.1", "price": i, } for i in [15000, 15500, 16000, 16500,
-16600]] payload["request"] = orders # Submit the orders in bulk.
-session.place_batch_order(payload) ``` Check out the example python files or
-the list of endpoints below for more information on available endpoints and
+Bybit employees â however, you're still welcome to contribute! It was
+designed with the following vision in mind: > I was personally never a fan of
+auto-generated connectors that used a mosh-pit of various modules you didn't
+want (sorry, `bravado`) and wanted to build my own Python3-dedicated connector
+with very little external resources. The goal of the connector is to provide
+traders and developers with an easy-to-use high-performing module that has an
+active issue and discussion board leading to consistent improvements. ##
+Development `pybit` is being actively developed, and new Bybit API changes
+should arrive on `pybit` very quickly. `pybit` uses `requests` and `websocket-
+client` for its methods, alongside other built-in modules. Anyone is welcome to
+branch/fork the repository and add their own upgrades. If you think you've made
+substantial improvements to the module, submit a pull request and we'll gladly
+take a look. ## Installation `pybit` requires Python 3.9.1 or higher. The
+module can be installed manually or via [PyPI](https://pypi.org/project/pybit/
+) with `pip`: ``` pip install pybit ``` ## Usage You can retrieve a specific
+market like so: ```python from pybit.unified_trading import HTTP ``` Create an
+HTTP session and connect via WebSocket for Inverse on mainnet: ```python
+session = HTTP( testnet=False, api_key="...", api_secret="...", ) ```
+Information can be sent to, or retrieved from, the Bybit APIs: ```python # Get
+the orderbook of the USDT Perpetual, BTCUSDT session.get_orderbook
+(category="linear", symbol="BTCUSDT") # Create five long USDC Options orders. #
+(Currently, only USDC Options support sending orders in bulk.) payload =
+{"category": "option"} orders = [{ "symbol": "BTC-30JUN23-20000-C", "side":
+"Buy", "orderType": "Limit", "qty": "0.1", "price": i, } for i in [15000,
+15500, 16000, 16500, 16600]] payload["request"] = orders # Submit the orders in
+bulk. session.place_batch_order(payload) ``` Check out the example python files
+or the list of endpoints below for more information on available endpoints and
 methods. Usage examples on the `HTTP` methods can be found in the [examples
 folder](https://github.com/bybit-exchange/pybit/tree/master/examples). ##
 Contact You can reach out for support on the [BybitAPI Telegram](https://t.me/
 BybitAPI) group chat. ## Contributors Thanks goes to these wonderful people (
 [emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
-                                                               Cameron    Tom      Todd
-    dextertd           ervuks       verata-veritatis   APF20   Harder-   Rumpf    Conley
+                                                               Cameron    Tom               Todd
+    dextertd           ervuks       verata-veritatis   APF20   Harder-   Rumpf    OnJohn   Conley
                                                                 Hutton
-    ð» ð�    ð» ð�    ð» ð�  ð�           ð�  ð¤
+    ð» ð�    ð» ð�    ð» ð�  ð�           ð�  ð�  ð¤
                                                                  ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `pybit-5.2.0/examples/.DS_Store` & `pybit-5.3.0/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/examples/direct_session.py` & `pybit-5.3.0/examples/direct_session.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/examples/http_example_explanatory.py` & `pybit-5.3.0/examples/http_example_explanatory.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 To see which endpoints are available, check the Bybit API documentation:
 https://bybit-exchange.github.io/docs/v5/market/kline
 """
 
 # Import HTTP from the unified_trading module.
 from pybit.unified_trading import HTTP
 
-"""
-You can create an authenticated or unauthenticated HTTP session. 
-You can skip authentication by not passing any value for the key and secret.
-"""
+# Set up logging (optional)
+import logging
+logging.basicConfig(filename="pybit.log", level=logging.DEBUG,
+                    format="%(asctime)s %(levelname)s %(message)s")
+
+
+# You can create an authenticated or unauthenticated HTTP session.
+# You can skip authentication by not passing any value for the key and secret.
 
-# Authenticated
 session = HTTP(
     testnet=True,
     api_key="...",
     api_secret="...",
 )
 
 # Get the orderbook of the USDT Perpetual, BTCUSDT
```

### Comparing `pybit-5.2.0/examples/websocket_example_explanatory.py` & `pybit-5.3.0/examples/websocket_example_explanatory.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/examples/wrapper_class.py` & `pybit-5.3.0/examples/wrapper_class.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/_helpers.py` & `pybit-5.3.0/pybit/_helpers.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/_http_manager.py` & `pybit-5.3.0/pybit/_http_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         default_factory=lambda: {},
         init=False,
     )
     max_retries: bool = field(default=3)
     retry_delay: bool = field(default=3)
     referral_id: bool = field(default=None)
     record_request_time: bool = field(default=False)
+    return_response_headers: bool = field(default=False)
 
     def __post_init__(self):
         subdomain = SUBDOMAIN_TESTNET if self.testnet else SUBDOMAIN_MAINNET
         domain = DOMAIN_MAIN if not self.domain else self.domain
         url = HTTP_URL.format(SUBDOMAIN=subdomain, DOMAIN=domain)
         self.endpoint = url
 
@@ -181,14 +182,15 @@
             retries_attempted -= 1
             if retries_attempted < 0:
                 raise FailedRequestError(
                     request=f"{method} {path}: {req_params}",
                     message="Bad Request. Retries exceeded maximum.",
                     status_code=400,
                     time=dt.utcnow().strftime("%H:%M:%S"),
+                    resp_headers=None,
                 )
 
             retries_remaining = f"{retries_attempted} retries remain."
 
             req_params = self.prepare_payload(method, query)
 
             # Authenticate if we are using a private endpoint.
@@ -266,14 +268,15 @@
                     error_msg = "HTTP status code is not 200."
                 self.logger.debug(f"Response text: {s.text}")
                 raise FailedRequestError(
                     request=f"{method} {path}: {req_params}",
                     message=error_msg,
                     status_code=s.status_code,
                     time=dt.utcnow().strftime("%H:%M:%S"),
+                    resp_headers=s.headers,
                 )
 
             # Convert response to dictionary, or raise if requests error.
             try:
                 s_json = s.json()
 
             # If we have trouble converting, handle the error and retry.
@@ -285,66 +288,74 @@
                 else:
                     self.logger.debug(f"Response text: {s.text}")
                     raise FailedRequestError(
                         request=f"{method} {path}: {req_params}",
                         message="Conflict. Could not decode JSON.",
                         status_code=409,
                         time=dt.utcnow().strftime("%H:%M:%S"),
+                        resp_headers=s.headers,
                     )
 
             ret_code = "retCode"
             ret_msg = "retMsg"
 
             # If Bybit returns an error, raise.
             if s_json[ret_code]:
                 # Generate error message.
                 error_msg = f"{s_json[ret_msg]} (ErrCode: {s_json[ret_code]})"
 
                 # Set default retry delay.
-                err_delay = self.retry_delay
+                delay_time = self.retry_delay
 
                 # Retry non-fatal whitelisted error requests.
                 if s_json[ret_code] in self.retry_codes:
                     # 10002, recv_window error; add 2.5 seconds and retry.
                     if s_json[ret_code] == 10002:
                         error_msg += ". Added 2.5 seconds to recv_window"
                         recv_window += 2500
 
-                    # 10006, ratelimit error; wait until rate_limit_reset_ms
-                    # and retry.
+                    # 10006, rate limit error; wait until
+                    # X-Bapi-Limit-Reset-Timestamp and retry.
                     elif s_json[ret_code] == 10006:
                         self.logger.error(
-                            f"{error_msg}. Ratelimited on current request. "
+                            f"{error_msg}. Hit the API rate limit. "
                             f"Sleeping, then trying again. Request: {path}"
                         )
 
-                        # Calculate how long we need to wait.
-                        limit_reset = s_json["rate_limit_reset_ms"] / 1000
-                        reset_str = time.strftime(
-                            "%X", time.localtime(limit_reset)
-                        )
-                        err_delay = int(limit_reset) - int(time.time())
+                        # Calculate how long we need to wait in milliseconds.
+                        limit_reset_time = int(s.headers["X-Bapi-Limit-Reset-Timestamp"])
+                        limit_reset_str = dt.fromtimestamp(limit_reset_time / 10**3).strftime(
+                            "%H:%M:%S.%f")[:-3]
+                        delay_time = (int(limit_reset_time) - _helpers.generate_timestamp()) / 10**3
                         error_msg = (
-                            f"Ratelimit will reset at {reset_str}. "
-                            f"Sleeping for {err_delay} seconds"
+                            f"API rate limit will reset at {limit_reset_str}. "
+                            f"Sleeping for {int(delay_time * 10**3)} milliseconds"
                         )
 
                     # Log the error.
                     self.logger.error(f"{error_msg}. {retries_remaining}")
-                    time.sleep(err_delay)
+                    time.sleep(delay_time)
                     continue
 
                 elif s_json[ret_code] in self.ignore_codes:
                     pass
 
                 else:
                     raise InvalidRequestError(
                         request=f"{method} {path}: {req_params}",
                         message=s_json[ret_msg],
                         status_code=s_json[ret_code],
                         time=dt.utcnow().strftime("%H:%M:%S"),
+                        resp_headers=s.headers,
                     )
             else:
-                if self.record_request_time:
+                if self.log_requests:
+                    self.logger.debug(
+                        f"Response headers: {s.headers}"
+                    )
+
+                if self.return_response_headers:
+                    return s_json, s.elapsed, s.headers,
+                elif self.record_request_time:
                     return s_json, s.elapsed
                 else:
                     return s_json
```

### Comparing `pybit-5.2.0/pybit/_v5_account.py` & `pybit-5.3.0/pybit/_v5_account.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 
         Returns:
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/account/fee-rate
         """
-        print(f"{self.endpoint}{Account.GET_ACCOUNT_INFO}")
         return self._submit_request(
             method="GET",
             path=f"{self.endpoint}{Account.GET_FEE_RATE}",
             query=kwargs,
             auth=True,
         )
 
@@ -111,15 +110,14 @@
 
         Returns:
             Request results as dictionary.
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/account/account-info
         """
-        print(f"{self.endpoint}{Account.GET_ACCOUNT_INFO}")
         return self._submit_request(
             method="GET",
             path=f"{self.endpoint}{Account.GET_ACCOUNT_INFO}",
             query=kwargs,
             auth=True,
         )
```

### Comparing `pybit-5.2.0/pybit/_v5_asset.py` & `pybit-5.3.0/pybit/_v5_asset.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/_v5_market.py` & `pybit-5.3.0/pybit/_v5_market.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/_v5_position.py` & `pybit-5.3.0/pybit/_v5_position.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/_v5_spot_leverage_token.py` & `pybit-5.3.0/pybit/_v5_spot_leverage_token.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/_v5_spot_margin_trade.py` & `pybit-5.3.0/pybit/_v5_spot_margin_trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/_v5_trade.py` & `pybit-5.3.0/pybit/_v5_trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/_v5_user.py` & `pybit-5.3.0/pybit/_v5_user.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/_websocket_stream.py` & `pybit-5.3.0/pybit/_websocket_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,54 +290,54 @@
             "position",
             "execution",
             "order",
             "wallet",
             "greeks",
         ]
 
-        self.symbol_wildcard = "*"
-        self.symbol_separator = "|"
-
-    def subscribe(self, topic, callback):
-        splitted_topic = topic.split(".")
-        if len(splitted_topic) > 1:
-            symbol = [splitted_topic[-1]]
-        else:
-            symbol = []
+    def subscribe(
+            self,
+            topic: str,
+            callback,
+            symbol: (str, list) = False
+    ):
 
         def prepare_subscription_args(list_of_symbols):
             """
             Prepares the topic for subscription by formatting it with the
             desired symbols.
             """
 
             if topic in self.private_topics:
                 # private topics do not support filters
                 return [topic]
 
             topics = []
-            for symbol in list_of_symbols:
-                topics.append(topic.format(symbol))
+            for single_symbol in list_of_symbols:
+                topics.append(topic.format(symbol=single_symbol))
             return topics
 
+        if type(symbol) == str:
+            symbol = [symbol]
+
         subscription_args = prepare_subscription_args(symbol)
         self._check_callback_directory(subscription_args)
 
-        while not self.is_connected():
-            # Wait until the connection is open before subscribing.
-            time.sleep(0.1)
-
         req_id = str(uuid4())
 
         subscription_message = json.dumps(
             {"op": "subscribe", "req_id": req_id, "args": subscription_args}
         )
+        while not self.is_connected():
+            # Wait until the connection is open before subscribing.
+            time.sleep(0.1)
         self.ws.send(subscription_message)
         self.subscriptions[req_id] = subscription_message
-        self._set_callback(topic, callback)
+        for topic in subscription_args:
+            self._set_callback(topic, callback)
 
     def _initialise_local_data(self, topic):
         # Create self.data
         try:
             self.data[topic]
         except KeyError:
             self.data[topic] = []
@@ -464,30 +464,22 @@
         if is_auth_message():
             self._process_auth_message(message)
         elif is_subscription_message():
             self._process_subscription_message(message)
         else:
             self._process_normal_message(message)
 
-    def _extract_topic(self, topic_string):
-        if topic_string in self.private_topics:
-            return topic_string
-
     def _check_callback_directory(self, topics):
         for topic in topics:
             if topic in self.callback_directory:
                 raise Exception(
                     f"You have already subscribed to this topic: " f"{topic}"
                 )
 
     def _set_callback(self, topic, callback_function):
-        topic = self._extract_topic(topic)
-
         self.callback_directory[topic] = callback_function
 
     def _get_callback(self, topic):
-        topic = self._extract_topic(topic)
         return self.callback_directory[topic]
 
     def _pop_callback(self, topic):
-        topic = self._extract_topic(topic)
         self.callback_directory.pop(topic)
```

### Comparing `pybit-5.2.0/pybit/account.py` & `pybit-5.3.0/pybit/account.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/asset.py` & `pybit-5.3.0/pybit/asset.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/exceptions.py` & `pybit-5.3.0/pybit/legacy/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,40 @@
-class UnauthorizedExceptionError(Exception):
-    pass
-
-
-class InvalidChannelTypeError(Exception):
-    pass
-
-
-class TopicMismatchError(Exception):
-    pass
-
-
 class FailedRequestError(Exception):
     """
     Exception raised for failed requests.
 
     Attributes:
         request -- The original request that caused the error.
         message -- Explanation of the error.
         status_code -- The code number returned.
         time -- The time of the error.
     """
-
     def __init__(self, request, message, status_code, time):
         self.request = request
         self.message = message
         self.status_code = status_code
         self.time = time
         super().__init__(
-            f"{message.capitalize()} (ErrCode: {status_code}) (ErrTime: {time})"
-            f".\nRequest → {request}."
+            f'{message.capitalize()} (ErrCode: {status_code}) (ErrTime: {time})'
+            f'.\nRequest → {request}.'
         )
 
 
 class InvalidRequestError(Exception):
     """
     Exception raised for returned Bybit errors.
 
     Attributes:
         request -- The original request that caused the error.
         message -- Explanation of the error.
         status_code -- The code number returned.
         time -- The time of the error.
     """
-
     def __init__(self, request, message, status_code, time):
         self.request = request
         self.message = message
         self.status_code = status_code
         self.time = time
         super().__init__(
-            f"{message} (ErrCode: {status_code}) (ErrTime: {time})"
-            f".\nRequest → {request}."
+            f'{message} (ErrCode: {status_code}) (ErrTime: {time})'
+            f'.\nRequest → {request}.'
         )
```

### Comparing `pybit-5.2.0/pybit/legacy/_helpers.py` & `pybit-5.3.0/pybit/legacy/_helpers.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/legacy/_http_manager.py` & `pybit-5.3.0/pybit/legacy/_http_manager.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/legacy/_websocket_stream.py` & `pybit-5.3.0/pybit/legacy/_websocket_stream.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/legacy/copy_trading.py` & `pybit-5.3.0/pybit/legacy/copy_trading.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/legacy/usdc_options.py` & `pybit-5.3.0/pybit/legacy/usdc_options.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/legacy/usdc_perpetual.py` & `pybit-5.3.0/pybit/legacy/usdc_perpetual.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/market.py` & `pybit-5.3.0/pybit/market.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/position.py` & `pybit-5.3.0/pybit/position.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/spot_margin_trade.py` & `pybit-5.3.0/pybit/spot_margin_trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/trade.py` & `pybit-5.3.0/pybit/trade.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit/unified_trading.py` & `pybit-5.3.0/pybit/unified_trading.py`

 * *Files 7% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         """
         self._validate_private_topic()
         topic = "greeks"
         self.subscribe(topic, callback)
 
     # Public topics
 
-    def orderbook_stream(self, depth: int, symbol: str, callback):
+    def orderbook_stream(self, depth: int, symbol: (str, list), callback):
         """Subscribe to the orderbook stream. Supports different depths.
 
         Linear & inverse:
         Level 1 data, push frequency: 10ms
         Level 50 data, push frequency: 20ms
         Level 200 data, push frequency: 100ms
         Level 500 data, push frequency: 100ms
@@ -161,126 +161,126 @@
         Level 50 data, push frequency: 20ms
 
         Option:
         Level 25 data, push frequency: 20ms
         Level 100 data, push frequency: 100ms
 
         Required args:
-            symbol (string): Symbol name
+            symbol (string/list): Symbol name(s)
             depth (int): Orderbook depth
             callback:
 
         Additional information:
             https://bybit-exchange.github.io/docs/v5/websocket/public/orderbook
         """
         self._validate_public_topic()
-        topic = f"orderbook.{depth}.{symbol}"
-        self.subscribe(topic, callback)
+        topic = f"orderbook.{depth}." + "{symbol}"
+        self.subscribe(topic, callback, symbol)
 
-    def trade_stream(self, symbol: str, callback):
+    def trade_stream(self, symbol: (str, list), callback):
         """
         Subscribe to the recent trades stream.
         After subscription, you will be pushed trade messages in real-time.
 
         Push frequency: real-time
 
         Required args:
-            symbol (string): Symbol name
+            symbol (string/list): Symbol name(s)
 
          Additional information:
             https://bybit-exchange.github.io/docs/v5/websocket/public/trade
         """
         self._validate_public_topic()
-        topic = f"publicTrade.{symbol}"
-        self.subscribe(topic, callback)
+        topic = f"publicTrade." + "{symbol}"
+        self.subscribe(topic, callback, symbol)
 
-    def ticker_stream(self, symbol: str, callback):
+    def ticker_stream(self, symbol: (str, list), callback):
         """Subscribe to the ticker stream.
 
         Push frequency: 100ms
 
         Required args:
-            symbol (string): Symbol name
+            symbol (string/list): Symbol name(s)
 
          Additional information:
             https://bybit-exchange.github.io/docs/v5/websocket/public/ticker
         """
         self._validate_public_topic()
-        topic = f"tickers.{symbol}"
-        self.subscribe(topic, callback)
+        topic = "tickers.{symbol}"
+        self.subscribe(topic, callback, symbol)
 
-    def kline_stream(self, interval: int, symbol: str, callback):
+    def kline_stream(self, interval: int, symbol: (str, list), callback):
         """Subscribe to the klines stream.
 
         Push frequency: 1-60s
 
         Required args:
-            symbol (string): Symbol name
+            symbol (string/list): Symbol name(s)
             interval (int): Kline interval
 
          Additional information:
             https://bybit-exchange.github.io/docs/v5/websocket/public/kline
         """
         self._validate_public_topic()
-        topic = f"kline.{interval}.{symbol}"
-        self.subscribe(topic, callback)
+        topic = f"kline.{interval}." + "{symbol}"
+        self.subscribe(topic, callback, symbol)
 
-    def liquidation_stream(self, symbol: str, callback):
+    def liquidation_stream(self, symbol: (str, list), callback):
         """Subscribe to the klines stream.
 
         Push frequency: 1-60s
 
         Required args:
-            symbol (string): Symbol name
+            symbol (string/list): Symbol name(s)
 
          Additional information:
             https://bybit-exchange.github.io/docs/v5/websocket/public/kline
         """
         self._validate_public_topic()
-        topic = f"liquidation.{symbol}"
-        self.subscribe(topic, callback)
+        topic = "liquidation.{symbol}"
+        self.subscribe(topic, callback, symbol)
 
-    def lt_kline_stream(self, interval: int, symbol: str, callback):
+    def lt_kline_stream(self, interval: int, symbol: (str, list), callback):
         """Subscribe to the leveraged token kline stream.
 
         Push frequency: 1-60s
 
         Required args:
-            symbol (string): Symbol name
+            symbol (string/list): Symbol name(s)
             interval (int): Leveraged token Kline stream interval
 
          Additional information:
             https://bybit-exchange.github.io/docs/v5/websocket/public/etp-kline
         """
         self._validate_public_topic()
-        topic = f"kline_lt.{interval}.{symbol}"
-        self.subscribe(topic, callback)
+        topic = f"kline_lt.{interval}." + "{symbol}"
+        self.subscribe(topic, callback, symbol)
 
-    def lt_ticker_stream(self, symbol: str, callback):
+    def lt_ticker_stream(self, symbol: (str, list), callback):
         """Subscribe to the leveraged token ticker stream.
 
         Push frequency: 300ms
 
         Required args:
-            symbol (string): Symbol name
+            symbol (string/list): Symbol name(s)
 
          Additional information:
             https://bybit-exchange.github.io/docs/v5/websocket/public/etp-ticker
         """
         self._validate_public_topic()
-        topic = f"tickers_lt.{symbol}"
-        self.subscribe(topic, callback)
+        topic = "tickers_lt.{symbol}"
+        self.subscribe(topic, callback, symbol)
 
-    def lt_nav_stream(self, symbol: str, callback):
+    def lt_nav_stream(self, symbol: (str, list), callback):
         """Subscribe to the leveraged token nav stream.
 
         Push frequency: 300ms
 
         Required args:
-            symbol (string): Symbol name
+            symbol (string/list): Symbol name(s)
 
          Additional information:
             https://bybit-exchange.github.io/docs/v5/websocket/public/etp-nav
         """
         self._validate_public_topic()
-        topic = f"lt.{symbol}"
-        self.subscribe(topic, callback)
+        topic = "lt.{symbol}"
+        self.subscribe(topic, callback, symbol)
```

### Comparing `pybit-5.2.0/pybit/user.py` & `pybit-5.3.0/pybit/user.py`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/pybit.egg-info/PKG-INFO` & `pybit-5.3.0/pybit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybit
-Version: 5.2.0
+Version: 5.3.0
 Summary: Python3 Bybit HTTP/WebSocket API Connector
 Home-page: https://github.com/bybit-exchange/pybit
 Author: Dexter Dickinson
 Author-email: dexter.dickinson@bybit.com
 License: MIT License
 Description: # pybit
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
@@ -24,15 +24,15 @@
         - [Installation](#installation)
         - [Usage](#usage)
         - [Contact](#contact)
         - [Contributors](#contributors)
         - [Donations](#donations)
         
         ## About
-        Put simply, `pybit` (Python + Bybit) is the official lightweight one-stop-shop module for the Bybit HTTP and WebSocket APIs. Originally created by [Verata Veritatis](https://github.com/verata-veritatis), it's now maintained by Bybit employees - however, you're still welcome to contribute!
+        Put simply, `pybit` (Python + Bybit) is the official lightweight one-stop-shop module for the Bybit HTTP and WebSocket APIs. Originally created by [Verata Veritatis](https://github.com/verata-veritatis), it's now maintained by Bybit employees – however, you're still welcome to contribute!
         
         It was designed with the following vision in mind:
         
         > I was personally never a fan of auto-generated connectors that used a mosh-pit of various modules you didn't want (sorry, `bravado`) and wanted to build my own Python3-dedicated connector with very little external resources. The goal of the connector is to provide traders and developers with an easy-to-use high-performing module that has an active issue and discussion board leading to consistent improvements.
         
         ## Development
         `pybit` is being actively developed, and new Bybit API changes should arrive on `pybit` very quickly. `pybit` uses `requests` and `websocket-client` for its methods, alongside other built-in modules. Anyone is welcome to branch/fork the repository and add their own upgrades. If you think you've made substantial improvements to the module, submit a pull request and we'll gladly take a look.
@@ -96,14 +96,15 @@
           <tr>
             <td align="center"><a href="https://github.com/dextertd"><img src="https://avatars.githubusercontent.com/u/54495183?v=4" width="100px;" alt=""/><br /><sub><b>dextertd</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=dextertd" title="Code">💻</a> <a href="https://github.com/bybit-exchange/pybit/commits?author=dextertd" title="Documentation">📖</a></td>
             <td align="center"><a href="https://github.com/ervuks"><img src="https://avatars.githubusercontent.com/u/17198438?v=4" width="100px;" alt=""/><br /><sub><b>ervuks</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=ervuks" title="Code">💻</a> <a href="https://github.com/bybit-exchange/pybit/commits?author=ervuks" title="Documentation">📖</a></td></td>
             <td align="center"><a href="https://github.com/verata-veritatis"><img src="https://avatars0.githubusercontent.com/u/9677388?v=4" width="100px;" alt=""/><br /><sub><b>verata-veritatis</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=verata-veritatis" title="Code">💻</a> <a href="https://github.com/bybit-exchange/pybit/commits?author=verata-veritatis" title="Documentation">📖</a></td>
             <td align="center"><a href="https://github.com/APF20"><img src="https://avatars0.githubusercontent.com/u/74583612?v=4" width="100px;" alt=""/><br /><sub><b>APF20</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=APF20" title="Code">💻</a></td>
             <td align="center"><a href="https://github.com/cameronhh"><img src="https://avatars0.githubusercontent.com/u/30434979?v=4" width="100px;" alt=""/><br /><sub><b>Cameron Harder-Hutton</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=cameronhh" title="Code">💻</a></td>
             <td align="center"><a href="https://github.com/tomcru"><img src="https://avatars0.githubusercontent.com/u/35841182?v=4" width="100px;" alt=""/><br /><sub><b>Tom Rumpf</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=tomcru" title="Code">💻</a></td>
+            <td align="center"><a href="https://github.com/sheungon"><img src="https://avatars.githubusercontent.com/u/13306724?v=4" width="100px;" alt=""/><br /><sub><b>OnJohn</b></sub></a><br /><a href="https://github.com/bybit-exchange/pybit/commits?author=sheungon" title="Code">💻</a></td>
             <td align="center"><a href="https://github.com/tconley"><img src="https://avatars1.githubusercontent.com/u/1893207?v=4" width="100px;" alt=""/><br /><sub><b>Todd Conley</b></sub></a><br /><a href="https://github.com/tconley/pybit/commits?author=tconley" title="Ideas">🤔</a></td>
           </tr>
         </table>
         
         <!-- markdownlint-enable -->
         <!-- prettier-ignore-end -->
         <!-- ALL-CONTRIBUTORS-LIST:END -->
@@ -112,14 +113,11 @@
         
 Keywords: bybit api connector
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pybit-5.2.0/pybit.egg-info/SOURCES.txt` & `pybit-5.3.0/pybit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybit-5.2.0/setup.py` & `pybit-5.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pybit',
-    version='5.2.0',
+    version='5.3.0',
     description='Python3 Bybit HTTP/WebSocket API Connector', 
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bybit-exchange/pybit",
     license="MIT License",
     author="Dexter Dickinson",
     author_email="dexter.dickinson@bybit.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     keywords="bybit api connector",
     packages=["pybit", "pybit.legacy"],
     python_requires=">=3.6",
     install_requires=[
```

