# Comparing `tmp/oddsjam-api-0.2.8.tar.gz` & `tmp/oddsjam-api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oddsjam-api-0.2.8.tar", last modified: Thu May 18 15:09:14 2023, max compression
+gzip compressed data, was "oddsjam-api-0.2.9.tar", last modified: Fri May 19 18:12:20 2023, max compression
```

## Comparing `oddsjam-api-0.2.8.tar` & `oddsjam-api-0.2.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.155375 oddsjam-api-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-18 15:09:14.151375 oddsjam-api-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 15:09:04.000000 oddsjam-api-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:09:14.155375 oddsjam-api-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.139375 oddsjam-api-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.139375 oddsjam-api-0.2.8/src/Base/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/CustomExceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/EnforceTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/ModelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/RequestBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/ResponseBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/ValidParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.139375 oddsjam-api-0.2.8/src/Models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.143375 oddsjam-api-0.2.8/src/Models/V1/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/Future.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/FutureOdds.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/Game.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/League.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/Market.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/Odds.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/PeriodScore.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/Score.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.143375 oddsjam-api-0.2.8/src/Models/V2/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/Future.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/FutureOdds.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/Game.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/League.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/Market.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/Odds.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/PeriodScore.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/Score.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/V2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.143375 oddsjam-api-0.2.8/src/OddsJamClient/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/OddsJamClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.143375 oddsjam-api-0.2.8/src/OddsJamClient/V1/
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/V1/Requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/V1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.147375 oddsjam-api-0.2.8/src/OddsJamClient/V2/
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/V2/Requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/V2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/OddsJamClient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.147375 oddsjam-api-0.2.8/src/Request/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.147375 oddsjam-api-0.2.8/src/Request/V1/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetFutureOddsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetFuturesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetGamesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetLeaguesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetMarketsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetOddsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/GetScoresRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.147375 oddsjam-api-0.2.8/src/Request/V2/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetFutureOddsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetFuturesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetGamesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetLeaguesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetMarketsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetOddsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/GetScoresRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/V2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.147375 oddsjam-api-0.2.8/src/Response/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.151375 oddsjam-api-0.2.8/src/Response/V1/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetFutureOddsResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetFuturesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetGamesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetLeaguesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetMarketsResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetOddsResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/GetScoresResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.151375 oddsjam-api-0.2.8/src/Response/V2/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetFutureOddsResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetFuturesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetGamesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetLeaguesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetMarketsResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetOddsResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/GetScoresResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/V2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/Response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 15:09:02.000000 oddsjam-api-0.2.8/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:09:14.151375 oddsjam-api-0.2.8/src/oddsjam_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-18 15:09:14.000000 oddsjam-api-0.2.8/src/oddsjam_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-18 15:09:14.000000 oddsjam-api-0.2.8/src/oddsjam_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:09:14.000000 oddsjam-api-0.2.8/src/oddsjam_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-18 15:09:14.000000 oddsjam-api-0.2.8/src/oddsjam_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.126984 oddsjam-api-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-19 18:12:20.126984 oddsjam-api-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-19 18:12:12.000000 oddsjam-api-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:12:20.126984 oddsjam-api-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.110984 oddsjam-api-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.110984 oddsjam-api-0.2.9/src/Base/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Base/CustomExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Base/EnforceTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Base/ModelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Base/RequestBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Base/ResponseBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Base/ValidParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.110984 oddsjam-api-0.2.9/src/Models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.114984 oddsjam-api-0.2.9/src/Models/V1/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V1/Future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V1/FutureOdds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V1/Game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V1/League.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V1/Market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V1/Odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V1/PeriodScore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V1/Score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.114984 oddsjam-api-0.2.9/src/Models/V2/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V2/Future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V2/FutureOdds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V2/Game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V2/League.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V2/Market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V2/Odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V2/PeriodScore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V2/Score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.114984 oddsjam-api-0.2.9/src/OddsJamClient/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/OddsJamClient/OddsJamClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.118984 oddsjam-api-0.2.9/src/OddsJamClient/V1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/OddsJamClient/V1/Requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/OddsJamClient/V1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.118984 oddsjam-api-0.2.9/src/OddsJamClient/V2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/OddsJamClient/V2/Requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/OddsJamClient/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/OddsJamClient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.118984 oddsjam-api-0.2.9/src/Request/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.118984 oddsjam-api-0.2.9/src/Request/V1/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V1/GetFutureOddsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V1/GetFuturesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V1/GetGamesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V1/GetLeaguesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V1/GetMarketsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V1/GetOddsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V1/GetScoresRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.122984 oddsjam-api-0.2.9/src/Request/V2/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V2/GetFutureOddsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V2/GetFuturesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V2/GetGamesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V2/GetLeaguesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V2/GetMarketsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V2/GetOddsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V2/GetScoresRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.122984 oddsjam-api-0.2.9/src/Response/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.122984 oddsjam-api-0.2.9/src/Response/V1/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V1/GetFutureOddsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V1/GetFuturesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V1/GetGamesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V1/GetLeaguesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V1/GetMarketsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V1/GetOddsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V1/GetScoresResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.126984 oddsjam-api-0.2.9/src/Response/V2/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V2/GetFutureOddsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V2/GetFuturesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V2/GetGamesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V2/GetLeaguesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V2/GetMarketsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V2/GetOddsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V2/GetScoresResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/V2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/Response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 18:12:09.000000 oddsjam-api-0.2.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:20.126984 oddsjam-api-0.2.9/src/oddsjam_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-19 18:12:20.000000 oddsjam-api-0.2.9/src/oddsjam_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-19 18:12:20.000000 oddsjam-api-0.2.9/src/oddsjam_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:12:20.000000 oddsjam-api-0.2.9/src/oddsjam_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 18:12:20.000000 oddsjam-api-0.2.9/src/oddsjam_api.egg-info/top_level.txt
```

### Comparing `oddsjam-api-0.2.8/LICENSE` & `oddsjam-api-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/PKG-INFO` & `oddsjam-api-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oddsjam-api
-Version: 0.2.8
+Version: 0.2.9
 Summary: A lightweight OddsJam API wrapper
 Author-email: Rohan Challa <rchalla769@gmail.com>, Brandon Cooper <cooper.brandon@outlook.com>
 Project-URL: Homepage, https://github.com/oddsjam/api-python
 Project-URL: Bug Tracker, https://github.com/oddsjam/api-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oddsjam-api-0.2.8/README.md` & `oddsjam-api-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/pyproject.toml` & `oddsjam-api-0.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "oddsjam-api"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
     { name="Rohan Challa", email="rchalla769@gmail.com" },
     { name="Brandon Cooper", email="cooper.brandon@outlook.com" },
 ]
 description = "A lightweight OddsJam API wrapper"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `oddsjam-api-0.2.8/src/Base/CustomExceptions.py` & `oddsjam-api-0.2.9/src/Base/CustomExceptions.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Base/EnforceTypes.py` & `oddsjam-api-0.2.9/src/Base/EnforceTypes.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Base/RequestBase.py` & `oddsjam-api-0.2.9/src/Base/RequestBase.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Models/V1/Odds.py` & `oddsjam-api-0.2.9/src/Models/V1/Odds.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Models/V1/Score.py` & `oddsjam-api-0.2.9/src/Models/V1/Score.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Models/V2/Odds.py` & `oddsjam-api-0.2.9/src/Models/V2/Odds.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Models/V2/Score.py` & `oddsjam-api-0.2.9/src/Models/V2/Score.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/OddsJamClient/OddsJamClient.py` & `oddsjam-api-0.2.9/src/OddsJamClient/OddsJamClient.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/OddsJamClient/V1/Requestor.py` & `oddsjam-api-0.2.9/src/OddsJamClient/V1/Requestor.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/OddsJamClient/V2/Requestor.py` & `oddsjam-api-0.2.9/src/OddsJamClient/V2/Requestor.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V1/GetFutureOddsResponse.py` & `oddsjam-api-0.2.9/src/Response/V1/GetFutureOddsResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V1/GetLeaguesResponse.py` & `oddsjam-api-0.2.9/src/Response/V1/GetLeaguesResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V1/GetMarketsResponse.py` & `oddsjam-api-0.2.9/src/Response/V1/GetMarketsResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V1/GetOddsResponse.py` & `oddsjam-api-0.2.9/src/Response/V1/GetOddsResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V1/GetScoresResponse.py` & `oddsjam-api-0.2.9/src/Response/V1/GetScoresResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V2/GetFutureOddsResponse.py` & `oddsjam-api-0.2.9/src/Response/V2/GetFutureOddsResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V2/GetFuturesResponse.py` & `oddsjam-api-0.2.9/src/Response/V2/GetFuturesResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V2/GetGamesResponse.py` & `oddsjam-api-0.2.9/src/Response/V2/GetGamesResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V2/GetMarketsResponse.py` & `oddsjam-api-0.2.9/src/Response/V2/GetMarketsResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V2/GetOddsResponse.py` & `oddsjam-api-0.2.9/src/Response/V2/GetOddsResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/Response/V2/GetScoresResponse.py` & `oddsjam-api-0.2.9/src/Response/V2/GetScoresResponse.py`

 * *Files identical despite different names*

### Comparing `oddsjam-api-0.2.8/src/oddsjam_api.egg-info/PKG-INFO` & `oddsjam-api-0.2.9/src/oddsjam_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oddsjam-api
-Version: 0.2.8
+Version: 0.2.9
 Summary: A lightweight OddsJam API wrapper
 Author-email: Rohan Challa <rchalla769@gmail.com>, Brandon Cooper <cooper.brandon@outlook.com>
 Project-URL: Homepage, https://github.com/oddsjam/api-python
 Project-URL: Bug Tracker, https://github.com/oddsjam/api-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oddsjam-api-0.2.8/src/oddsjam_api.egg-info/SOURCES.txt` & `oddsjam-api-0.2.9/src/oddsjam_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

